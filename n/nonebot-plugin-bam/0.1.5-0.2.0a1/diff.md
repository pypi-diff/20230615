# Comparing `tmp/nonebot_plugin_bam-0.1.5.tar.gz` & `tmp/nonebot_plugin_bam-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bam-0.1.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_bam-0.2.0a1.tar", max compression
```

## Comparing `nonebot_plugin_bam-0.1.5.tar` & `nonebot_plugin_bam-0.2.0a1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1059 2021-02-07 09:56:09.611375 nonebot_plugin_bam-0.1.5/LICENSE
--rw-r--r--   0        0        0     4863 2021-04-04 08:10:14.556405 nonebot_plugin_bam-0.1.5/README.md
--rw-r--r--   0        0        0      515 2021-04-04 08:15:20.681927 nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/__init__.py
--rw-r--r--   0        0        0     1633 2021-04-04 08:12:03.590747 nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/activity.py
--rw-r--r--   0        0        0        0 2021-04-04 08:12:26.188806 nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/bilibili/__init__.py
--rw-r--r--   0        0        0    11473 2021-04-04 08:12:28.896608 nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/bilibili/activity.py
--rw-r--r--   0        0        0     1907 2021-04-04 08:12:31.721031 nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/bilibili/api.py
--rw-r--r--   0        0        0      766 2021-04-04 08:12:35.493641 nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/bilibili/live1.py
--rw-r--r--   0        0        0      731 2021-04-04 08:12:37.711197 nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/bilibili/live2.py
--rw-r--r--   0        0        0      515 2021-04-04 08:12:39.695087 nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/bilibili/user.py
--rw-r--r--   0        0        0     1186 2021-04-04 08:12:09.575828 nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/common.py
--rw-r--r--   0        0        0      318 2021-04-04 08:12:11.542632 nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/config.py
--rw-r--r--   0        0        0       91 2021-04-04 08:12:46.161461 nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/database/__init__.py
--rw-r--r--   0        0        0     1338 2021-04-04 08:12:48.122266 nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/database/db.py
--rw-r--r--   0        0        0     3016 2021-04-04 08:12:51.546944 nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/database/helper.py
--rw-r--r--   0        0        0      154 2020-11-27 14:00:17.000000 nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/database/tables/__init__.py
--rw-r--r--   0        0        0      336 2020-11-27 14:00:18.000000 nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/database/tables/bilibili_user.py
--rw-r--r--   0        0        0      468 2020-11-27 14:00:16.000000 nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/database/tables/bilibili_user_status.py
--rw-r--r--   0        0        0      481 2021-04-04 08:08:48.651306 nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/database/tables/follow_link.py
--rw-r--r--   0        0        0      311 2020-12-13 08:42:51.000000 nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/database/tables/group.py
--rw-r--r--   0        0        0     5137 2021-04-04 08:12:13.707226 nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/follow.py
--rw-r--r--   0        0        0     3037 2021-04-04 08:12:17.122767 nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/group.py
--rw-r--r--   0        0        0        0 2020-11-27 14:00:21.000000 nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/tasks/__init__.py
--rw-r--r--   0        0        0     5202 2021-04-04 08:12:58.732307 nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/tasks/activity_monitor.py
--rw-r--r--   0        0        0     4186 2021-04-04 08:13:05.428836 nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/tasks/live_monitor.py
--rw-r--r--   0        0        0     1115 2021-04-04 08:12:20.358522 nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/user.py
--rw-r--r--   0        0        0     1067 2021-04-04 08:15:15.525516 nonebot_plugin_bam-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     5983 2021-04-04 08:16:30.611010 nonebot_plugin_bam-0.1.5/setup.py
--rw-r--r--   0        0        0     5833 2021-04-04 08:16:30.611348 nonebot_plugin_bam-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/LICENSE
+-rw-r--r--   0        0        0      663 2023-06-15 14:22:23.241393 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/__init__.py
+-rw-r--r--   0        0        0     1574 2023-06-15 13:02:15.074738 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/activity.py
+-rw-r--r--   0        0        0        0 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/bilibili/__init__.py
+-rw-r--r--   0        0        0    11587 2023-06-15 13:28:21.379404 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/bilibili/activity.py
+-rw-r--r--   0        0        0     2623 2023-06-15 13:30:12.670071 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/bilibili/api.py
+-rw-r--r--   0        0        0      766 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/bilibili/live1.py
+-rw-r--r--   0        0        0      832 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/bilibili/live2.py
+-rw-r--r--   0        0        0      624 2023-06-15 13:30:55.101501 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/bilibili/user.py
+-rw-r--r--   0        0        0     1836 2023-06-15 13:31:00.559739 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/bilibili/wbi.py
+-rw-r--r--   0        0        0      947 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/common.py
+-rw-r--r--   0        0        0      371 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/config.py
+-rw-r--r--   0        0        0       91 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/database/__init__.py
+-rw-r--r--   0        0        0     1404 2023-06-14 18:24:18.904298 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/database/db.py
+-rw-r--r--   0        0        0     3454 2023-06-15 13:08:52.469278 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/database/helper.py
+-rw-r--r--   0        0        0      154 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/database/tables/__init__.py
+-rw-r--r--   0        0        0      336 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/database/tables/bilibili_user.py
+-rw-r--r--   0        0        0      468 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/database/tables/bilibili_user_status.py
+-rw-r--r--   0        0        0      481 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/database/tables/follow_link.py
+-rw-r--r--   0        0        0      311 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/database/tables/group.py
+-rw-r--r--   0        0        0     5533 2023-06-15 13:05:10.058734 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/follow.py
+-rw-r--r--   0        0        0     3192 2023-06-15 12:58:16.897376 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/group.py
+-rw-r--r--   0        0        0        0 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/tasks/__init__.py
+-rw-r--r--   0        0        0     5208 2023-06-15 13:29:49.270283 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/tasks/activity_monitor.py
+-rw-r--r--   0        0        0     4166 2023-06-14 16:28:40.055159 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/tasks/live_monitor.py
+-rw-r--r--   0        0        0     1131 2023-06-15 13:00:44.289439 nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/user.py
+-rw-r--r--   0        0        0     1223 2023-06-15 14:22:29.663608 nonebot_plugin_bam-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0     4854 2023-06-15 14:10:02.101887 nonebot_plugin_bam-0.2.0a1/README.md
+-rw-r--r--   0        0        0     5994 1970-01-01 00:00:00.000000 nonebot_plugin_bam-0.2.0a1/PKG-INFO
```

### Comparing `nonebot_plugin_bam-0.1.5/LICENSE` & `nonebot_plugin_bam-0.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.1.5/README.md` & `nonebot_plugin_bam-0.2.0a1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 
 ```bash
 poetry add nonebot-plugin-bam
 ```
 
 ```python
 import nonebot
-from nonebot.adapters.cqhttp import Bot as CQHTTPBot
+from nonebot.adapters.onebot.v11 import Adapter
 
 nonebot.init(_env_file=".env")
 
 driver = nonebot.get_driver()
-driver.register_adapter("cqhttp", CQHTTPBot)
+driver.register_adapter(Adapter)
 
 nonebot.load_builtin_plugins()
 
 # load other plugins
 
 # bam need this to manage background tasks
 nonebot.load_plugin("nonebot_plugin_apscheduler")
@@ -59,15 +59,15 @@
 # 正常使用不要打开此选项，是调试用的
 BAM_ON_STARTUP_CLEAN_LIVE_STATUS=false 
 
 # 监控任务的间隔，这里设置的是每个用户间的间隔，而不是一轮的间隔。
 # 所以如果一共关注了 N 个人（多个群关注同一个人只算一个）
 # 那对于每个人来说，两次检测之间的间隔就是 N * interval
 # 一般来说不要设置在 5 以下，可能会被 B 站 API 反爬而拒绝响应
-BAM_TASK_INTERVAL=5
+BAM_MONITOR_TASK_INTERVAL=5
 
 # 使用那一个直播间状态查询 API，默认为 2，如果发现被封禁了可以临时调到 1 试试
 BAM_LIVE_API=2
 
 # 动态内容在发送到 QQ 时的最大长度，超过长度会截断，设置为 0 或负数表示不截断
 BAM_ACTIVITY_CONTENT_MAX_LENGTH=0
 ```
```

### Comparing `nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/activity.py` & `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/activity.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,40 @@
-import operator
-import random
-import re
-
-from nonebot import on_command, on_message
-from nonebot.adapters.cqhttp import Bot, Event, Message
-from nonebot.adapters.cqhttp.permission import GROUP, PRIVATE
-from nonebot.log import logger
-from nonebot.rule import regex, to_me
+from nonebot import on_command
+from nonebot.params import CommandArg
+from nonebot.adapters.onebot.v11 import Bot, MessageEvent, Message, GROUP, PRIVATE
+from nonebot.rule import to_me
 
 from .bilibili.activity import H5Activity, activity
 from .common import RE_NUMBER
 
 cmd_bilibili_activity_info = on_command(
     ("bam", "act"), rule=to_me(), permission=GROUP | PRIVATE, block=True
 )
 
 
 @cmd_bilibili_activity_info.handle()
-async def bilibili_activity_info(bot: Bot, event: Event, state: dict):
+async def bilibili_activity_info(bot: Bot, event: MessageEvent, args: Message = CommandArg()):
     messages = []
 
     if await GROUP(bot, event):
         messages.append(f"[CQ:at,qq={event.user_id}]")
 
-    args = str(event.message).strip()
+    arg_text = args.extract_plain_text().strip()
 
-    if RE_NUMBER.match(args) is None:
+    if RE_NUMBER.match(arg_text) is None:
         messages.append("参数错误，请输入正确的动态 ID")
-        return await cmd_bilibili_activity_info.finish("\n".join(messages))
+        await cmd_bilibili_activity_info.finish("\n".join(messages))
 
-    act_id = int(args)
+    act_id = int(arg_text)
 
     act = await activity(act_id)
 
     if act is None:
         messages.append("获取动态信息失败")
-        return await cmd_bilibili_activity_info.finish("\n".join(messages))
+        await cmd_bilibili_activity_info.finish("\n".join(messages))
 
     username = getattr(act, "username", f"ID 为 {act.uid} 的用户")
     messages.extend([f"{username} 的动态", "", act.display()])
 
     h5_share_card = None
     if isinstance(act, H5Activity):
         h5_share_card = act.h5_share_card()
```

### Comparing `nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/bilibili/activity.py` & `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/bilibili/activity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 
 from nonebot.log import logger
 
-from ..common import CONF, cq_encode
+from ..common import cq_encode
+from ..config import CONF
 from .api import APIResult
 
 MAX_LENGTH = CONF.bam_activity_content_max_length
 
 
 def shorten(s):
     if MAX_LENGTH > 0 and len(s) > MAX_LENGTH:
@@ -47,17 +48,17 @@
             return cls.KNOWN_TYPES_MAP[t]
         else:
             return UnTestedActivity
 
     @classmethod
     def build_known_types_map(cls):
         return {
-            sub.TYPE_VALUE: sub
+            getattr(sub, "TYPE_VALUE"): sub
             for sub in cls.__subclasses__()
-            if getattr(sub, "TYPE_VALUE", None) is not None
+            if hasattr(sub, "TYPE_VALUE")
         }
 
     def __init__(self, card):
         self._desc_data = card["desc"]
         if isinstance(card["card"], str):
             self._card_data = json.loads(card["card"])
         else:
@@ -66,16 +67,16 @@
         self.uid = self._desc_data["uid"]
         if "user" in self._card_data:
             if "uname" in self._card_data["user"]:
                 self.username = self._card_data["user"]["uname"]
             if "name" in self._card_data["user"]:
                 self.username = self._card_data["user"]["name"]
 
-    def display(self):
-        pass
+    def display(self) -> str:
+        raise NotImplementedError
 
     def url(self):
         return f"https://t.bilibili.com/{self.id}"
 
 
 class InvalidActivity(Activity):
     def __init__(self, card):
@@ -316,14 +317,16 @@
     URL = "https://api.vc.bilibili.com/dynamic_svr/v1/dynamic_svr/space_history?visitor_uid=0&host_uid={uid}&offset_dynamic_id={offset}&need_top=0&platform=web&ts={ts}"
 
     def __init__(self):
         super().__init__()
 
     def __initialize__(self, body, *, uid, offset):
         self.uid = uid
+        self.code = body["code"]
+        self.message = body["message"]
         self.ok = body["code"] == 0
         self.__data = []
         if self.ok and "cards" in body["data"]:
             for card in body["data"]["cards"]:
                 act = None
                 try:
                     act = Activity(card)
```

### Comparing `nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/bilibili/api.py` & `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/bilibili/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,83 @@
 import abc
-import asyncio
 import time
+import urllib.parse
 from http.cookies import SimpleCookie
+from typing import ClassVar, Dict, Optional
 
 from aiohttp import ClientSession, ClientTimeout, CookieJar, TCPConnector
+from nonebot import get_driver
 from nonebot.log import logger
 
-from ..common import DRIVER
-
-client: ClientSession = None
+client: ClientSession = None # type: ignore
 
 LOGNAME = "BILIBILI:API"
 
 
 async def init_client():
     global client
+    if client is not None:
+        return
+
     cookie = CookieJar()
     cookie.update_cookies(SimpleCookie("PVID=2; Domain=live.bilibili.com; Path=/;"))
 
     timeout = ClientTimeout(total=3)
 
     client = ClientSession(
         headers={
             "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/86.0.4240.183 Safari/537.36",
         },
         cookie_jar=cookie,
         timeout=timeout,
         connector=TCPConnector(force_close=True),
     )
 
-    logger.info(f"[{LOGNAME}] Client initalited")
+    logger.success(f"[{LOGNAME}] init HTTP client ok")
 
 
 class APIResult(abc.ABC):
-    URL = None
+    URL: ClassVar[str]
+    QUERY: ClassVar[Dict[str, str]]
+    WBI: ClassVar[Optional[bool]]
 
     def __init__(self):
         self.ok = False
 
     @abc.abstractmethod
     def __initialize__(self, body, **params):
         pass
 
     @classmethod
     async def of(cls, **params):
         instance = cls()
         params["ts"] = str(time.time())
         try:
             url = cls.URL.format(**params)
+            if hasattr(cls, "QUERY"):
+                query = {k: v.format(**params) for k, v in cls.QUERY.items()}
+                if getattr(cls, "WBI", False):
+                    from .wbi import wbi_token
+                    token = await wbi_token()
+                    token.add_signature(query)
+                url += '?' + urllib.parse.urlencode(query)
             logger.info(f"[{LOGNAME}] request: {url}")
             async with client.get(url) as resp:
+                logger.debug(f"[{LOGNAME}:{cls.__name__}] {url}: response {resp}")
                 data = await resp.json()
+                logger.debug(f"[{LOGNAME}:{cls.__name__}] {url}: body {data}")
                 try:
                     del params["ts"]
                     instance.__initialize__(data, **params)
                 except Exception as e:
                     instance.ok = False
-                    logger.warning(
+                    logger.info(
                         f"[{LOGNAME}:{cls.__name__}] {url} {type(e).__name__} {repr(e)}, response json {data}"
                     )
         except Exception as e:
-            logger.warning(
+            logger.info(
                 f"[{LOGNAME}:{cls.__name__}] request failed {type(e).__name__}: {repr(e)}"
             )
         return instance
 
 
-DRIVER.on_startup(init_client)
+get_driver().on_startup(init_client)
```

### Comparing `nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/bilibili/live1.py` & `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/bilibili/live1.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/bilibili/live2.py` & `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/bilibili/live2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from .api import APIResult
 
 
 class RoomInfo(APIResult):
-    URL = "https://api.bilibili.com/x/space/acc/info?mid={uid}&ts={ts}"
+    URL = "https://api.bilibili.com/x/space/wbi/acc/info"
+    # URL = "https://api.bilibili.com/x/space/acc/info"
+    QUERY = {
+        "mid": "{uid}",
+    }
+    WBI = True
 
     def __init__(self):
         super().__init__()
 
     def __initialize__(self, body, *, uid):
         self.uid = uid
         self.code = body["code"]
```

### Comparing `nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/bilibili/user.py` & `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/bilibili/user.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from .api import APIResult
 
 
 class UserInfo(APIResult):
-    URL = "https://api.bilibili.com/x/space/acc/info?mid={uid}"
+    URL = "https://api.bilibili.com/x/space/wbi/acc/info"
+    # URL = "https://api.bilibili.com/x/space/acc/info"
+    QUERY = {
+        "mid": "{uid}",
+    }
+    WBI = True
 
     def __init__(self):
         super().__init__()
 
     def __initialize__(self, body, *, uid):
         self.uid = uid
         self.ok = body["code"] == 0
```

### Comparing `nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/common.py` & `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/common.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,11 @@
 import re
 from asyncio import create_task
 
-import nonebot
-from nonebot.adapters.cqhttp import Bot
-
-from .config import Config
-
-DRIVER = G_CONF = CONF = None
-try:
-    DRIVER = nonebot.get_driver()
-    G_CONF = DRIVER.config
-    CONF = Config(**G_CONF.dict())
-except ValueError:
-    pass
-
-
-def get_bot() -> Bot:
-    for bot in DRIVER.bots.values():
-        return bot
-    return None
-
+from nonebot import get_bot, get_driver
 
 # Common regexes
 
 RE_NUMBER = re.compile(r"^\d+$")
 
 # Common functions
 
@@ -35,21 +17,22 @@
     return s.replace(",", "&#44;")
 
 
 async def exception_to_su_real(e, *messages):
     etype = type(e).__name__
     emsg = getattr(e, "message", repr(e))
     await get_bot().send_private_msg(
-        user_id=next(iter(G_CONF.superusers)),
+        user_id=next(iter(get_driver().config.superusers)),
         message=f"Exception {etype}: {emsg}",
         auto_escape=True,
     )
     for message in messages:
         await get_bot().send_private_msg(
-            user_id=next(iter(G_CONF.superusers)),
+            detail_type="private",
+            user_id=next(iter(get_driver().config.superusers)),
             message=message,
             auto_escape=False,
         )
 
 
 def send_exception_to_su(e, *messages):
     create_task(exception_to_su_real(e, *messages))
```

### Comparing `nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/database/db.py` & `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/database/db.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import importlib.resources
-
+from nonebot import get_driver
 from nonebot.log import logger
 from peewee import Model, PeeweeException, SqliteDatabase
 
-from ..common import CONF, DRIVER
+from ..config import CONF
+
+LOGNAME = "DATABASE"
 
 DB = SqliteDatabase(
     CONF.bam_db_file,
     pragmas={
         "journal_mode": "wal",
         "foreign_keys": 1,
         "ignore_check_constraints": 0,
@@ -30,14 +31,15 @@
             # at startup, treat everyone as having not started live streaming
             helper.clean_users_live_status()
     except PeeweeException as e:
         logger.error(f"init database failed")
         logger.error(str(e))
         raise e
 
+    logger.success(f"[{LOGNAME}] init ok")
 
 def connect_database():
     if CONF.bam_db_file == ":memory:":
         logger.warning("use memory db will lost all data after restart")
         logger.warning("set db location to a file path is highly recommended")
 
     try:
@@ -46,8 +48,8 @@
         logger.error(f"connect to {CONF.bam_db_file} failed")
         logger.error(str(e))
         raise e
 
     init_database()
 
 
-DRIVER.on_startup(connect_database)
+get_driver().on_startup(connect_database)
```

### Comparing `nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/follow.py` & `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/follow.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,80 +1,81 @@
-from nonebot import get_driver, on_command
-from nonebot.adapters.cqhttp import Bot, Event
-from nonebot.adapters.cqhttp.permission import GROUP
-from nonebot.log import logger
+from nonebot import on_command
+from nonebot.adapters.onebot.v11 import (Bot, GroupMessageEvent, Message,
+                                         MessageEvent)
+from nonebot.adapters.onebot.v11.permission import GROUP
+from nonebot.params import CommandArg
 from nonebot.permission import SUPERUSER
 
 from .bilibili.user import user_info
 from .common import RE_NUMBER
 from .database import helper
 
 # ===== Follower list =====
 
 cmd_follower_list = on_command(
     ("bam", "follower", "list"), permission=SUPERUSER | GROUP
 )
 
 
 @cmd_follower_list.handle()
-async def follower_list(bot: Bot, event: Event, state: dict):
+async def follower_list(event: MessageEvent, args: Message = CommandArg()):
     gid = None
-    if await GROUP(bot, event):
+    if isinstance(event, GroupMessageEvent):
         gid = event.group_id
     else:  # private, superuser
-        args = str(event.message).strip()
-        if RE_NUMBER.match(args):
-            gid = int(args)
+        args_text = args.extract_plain_text().strip()
+        if RE_NUMBER.match(args_text):
+            gid = int(args_text)
         else:
-            return await cmd_follower_list.finish("此命令需要一个群号参数")
+            await cmd_follower_list.finish("此命令需要一个群号参数")
 
     group = helper.get_group_with_following_users(gid)
 
     if group is None:
-        return await cmd_follower_list.finish("此群不在服务列表中")
+        await cmd_follower_list.finish("此群不在服务列表中")
 
     message = ["关注用户列表:"]
 
-    for following in group.followings:
+    for following in group.followings: # type: ignore
         following = following.bilibili_user
         message.append(f"{following.uid}({following.nickname})")
 
     if len(message) == 1:
         message.append("空")
 
     await cmd_follower_list.finish("\n".join(message))
 
 
 # Common command check and info for follower commands
 
 
 class CommandInfo:
-    def __init__(self, cmd, bot, event):
+    def __init__(self, cmd, bot: Bot, event: MessageEvent, args: Message):
         self.cmd = cmd
         self.bot = bot
         self.event = event
+        self.args = args.extract_plain_text().strip()
         self.gid = self.uid = None
 
     async def check(self):
         self.is_su = await SUPERUSER(self.bot, self.event)
         self.in_group = await GROUP(self.bot, self.event)
         self.message_type = "group" if self.in_group else "private"
         self.sender_id = self.event.user_id
 
-        args = str(self.event.message).strip()
-
         if self.in_group:
+            assert isinstance(self.event, GroupMessageEvent)
             self.gid = self.event.group_id
-            if RE_NUMBER.match(args):
-                self.uid = int(args)
+            if RE_NUMBER.match(self.args):
+                self.uid = int(self.args)
             else:
                 await self.cmd.finish("用户 UID 无效")
                 return False
         elif self.is_su:  # private, su
-            parts = args.split(" ")
+            parts = self.args.split(" ")
             if len(parts) != 2:
                 return await self.cmd.finish("缺少参数，需要群号和 UID")
             if RE_NUMBER.match(parts[0]):
                 self.gid = int(parts[0])
             else:
                 await self.cmd.finish("群号无效")
                 return False
@@ -106,21 +107,23 @@
 
 # ===== Follower add =====
 
 cmd_follower_add = on_command(("bam", "follower", "add"), permission=SUPERUSER | GROUP)
 
 
 @cmd_follower_add.handle()
-async def follower_add(bot: Bot, event: Event, state: dict):
+async def follower_add(bot: Bot, event: MessageEvent, args: Message = CommandArg()):
 
-    command = CommandInfo(cmd_follower_add, bot, event)
+    command = CommandInfo(cmd_follower_add, bot, event, args)
 
     if not await command.check():
         return
 
+    assert(command.group is not None)
+
     for following in command.group.followings:
         following = following.bilibili_user
         if following.uid == command.uid:
             return await cmd_follower_add.finish(f"用户 {command.uid} 已在关注列表内")
 
     user = helper.get_user(command.uid)
 
@@ -134,30 +137,32 @@
             return await cmd_follower_add.finish(f"获取 {command.uid} 用户信息失败")
 
     await command.send(f"UID: {user.uid}, 昵称: {user.nickname}, 直播间: {user.rid}")
 
     helper.add_link(command.group, user)
     return await cmd_follower_add.finish(f"成功加入关注列表")
 
+# ===== Follower remove =====
 
 cmd_follower_remove = on_command(
     ("bam", "follower", "remove"), permission=SUPERUSER | GROUP
 )
 
 
 @cmd_follower_remove.handle()
-async def follower_remove(bot: Bot, event: Event, state: dict):
-    command = CommandInfo(cmd_follower_remove, bot, event)
+async def follower_remove(bot: Bot, event: MessageEvent, args: Message = CommandArg()):
+    command = CommandInfo(cmd_follower_remove, bot, event, args)
 
     if not await command.check():
         return
 
+    assert(command.group is not None)
+
     for following in command.group.followings:
         following = following.bilibili_user
         if following.uid == command.uid:
             helper.remove_link(command.gid, command.uid)
             await cmd_follower_remove.finish(
                 f"成功将用户 {following.uid}({following.nickname}) 从关注列表移除"
             )
-            return
 
     await cmd_follower_remove.finish(f"用户 {command.uid} 不在关注列表中")
```

### Comparing `nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/group.py` & `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/group.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import random
 
-from nonebot import get_driver, on_command
-from nonebot.adapters.cqhttp import Bot, Event
-from nonebot.adapters.cqhttp.permission import GROUP, PRIVATE
+from nonebot import on_command
+from nonebot.adapters.onebot.v11 import (GROUP, PRIVATE, Bot,
+                                         GroupMessageEvent, Message,
+                                         MessageEvent)
 from nonebot.log import logger
+from nonebot.params import ArgPlainText, CommandArg
 from nonebot.permission import SUPERUSER
-from nonebot.rule import to_me
+from nonebot.typing import T_State
 
 from .common import RE_NUMBER
 from .database import helper
 
 # ===== Group list =====
 
 cmd_group_list = on_command(("bam", "group", "list"), permission=SUPERUSER)
 
 
 @cmd_group_list.handle()
-async def group_list(bot: Bot, event: Event, state: dict):
+async def group_list(bot: Bot, event: MessageEvent):
     if not await PRIVATE(bot, event):
-        return await cmd_group_list.finish("只能在私聊中使用此命令")
+        await cmd_group_list.finish("只能在私聊中使用此命令")
 
     message = ["当前正为以下群提供服务:"]
     message.extend(
         f"{group.gid}, 管理员: {group.super_user}" for group in helper.get_all_groups()
     )
     if len(message) == 1:
         message.append("空")
@@ -31,25 +33,26 @@
 
 # ===== Group add =====
 
 cmd_group_add = on_command(("bam", "group", "add"), permission=SUPERUSER)
 
 
 @cmd_group_add.handle()
-async def group_add(bot: Bot, event: Event, state: dict):
+async def group_add(bot: Bot, event: MessageEvent):
     if not await GROUP(bot, event):
         return await cmd_group_add.finish("只能在群聊中使用此命令")
 
+    assert(isinstance(event, GroupMessageEvent))
+
     gid = event.group_id
 
     group = helper.get_group(gid)
 
     if group is not None:
         await cmd_group_add.finish("此群已在服务列表中")
-        return
 
     group_suid = None
 
     args = str(event.message).strip()
     if RE_NUMBER.match(args):
         group_suid = int(args)
     else:
@@ -62,42 +65,38 @@
 
 # ===== Group remove =====
 
 cmd_group_remove = on_command(("bam", "group", "remove"), permission=SUPERUSER)
 
 
 @cmd_group_remove.handle()
-async def group_remove(bot: Bot, event: Event, state: dict):
+async def group_remove(bot: Bot, event: MessageEvent, state: T_State, args: Message = CommandArg()):
     if not await GROUP(bot, event):
-        return await cmd_group_remove.finish("只能在群聊中使用此命令")
+        await cmd_group_remove.finish("只能在群聊中使用此命令")
 
-    args = str(event.message).strip()
-    if args == "confirm":
+    args_text = args.extract_plain_text()
+    if args_text == "confirm":
         state["code"] = state["input_code"] = 0
     else:
         code = random.randint(10000000, 99999999)
         state["code"] = code
         await cmd_group_remove.pause(f"请回复以下随机码来确认删除操作: {code}")
 
-
 @cmd_group_remove.got("input_code")
-async def group_remove_confirm(bot: Bot, event: Event, state: dict):
+async def group_remove_confirm(event: GroupMessageEvent, state: T_State, input_code_arg: str = ArgPlainText()):
     code = state["code"]
-    input_code = state["input_code"].strip()
 
-    if not RE_NUMBER.match(input_code):
-        input_code = 0
-    else:
-        input_code = int(input_code)
+    logger.debug(f"code: {code}, input: {input_code_arg}")
 
-    logger.debug(f"code: {code}, input: {input_code}")
+    input_code = 0
+    if RE_NUMBER.match(input_code_arg):
+        input_code = int(input_code_arg)
 
     if input_code != code:
         await cmd_group_remove.finish("随机码不匹配，操作取消")
-        return
 
     group = helper.get_group(event.group_id)
 
     if group is None:
         await cmd_group_remove.finish("此群不在服务列表中，无操作")
     else:
         helper.remove_group(group)
```

### Comparing `nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/tasks/activity_monitor.py` & `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/tasks/activity_monitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import asyncio
-import json
 import traceback
 from datetime import datetime, timedelta
+from typing import Optional
 
-from nonebot import require
-from nonebot.adapters.cqhttp import Bot
+from nonebot import get_bot, require
 from nonebot.log import logger
 
 from ..bilibili.activity import ActivityList, H5Activity, activity_list
-from ..common import CONF, get_bot, send_exception_to_su
+from ..common import send_exception_to_su
+from ..config import CONF
 from ..database import helper
 
 scheduler = require("nonebot_plugin_apscheduler").scheduler
 
 JOB_ID = "activity_monitor"
 LOGNAME = "TASK:ACTIVITY"
 INTERVAL = CONF.bam_monitor_task_interval
@@ -33,15 +33,15 @@
     except Exception as e:
         logger.warning(f"[{LOGNAME}] Outer Exception {type(e).__name__}: {repr(e)}")
         logger.warning(f"[{LOGNAME}] {traceback.format_exc()}")
         send_exception_to_su(e)
     scheduler.resume_job(JOB_ID)
 
 
-async def process_user_actlist(user, actlist: ActivityList):
+async def process_user_actlist(user, actlist: Optional[ActivityList]):
     has_new = False
     latest = 0
     if actlist is None:
         return has_new, latest
 
     latest = user.status.newest_activity_id
     if actlist.ok:
```

### Comparing `nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/tasks/live_monitor.py` & `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/tasks/live_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import asyncio
 import json
 import traceback
 
-from nonebot import require
-from nonebot.adapters.cqhttp import Bot
+from nonebot import get_bot, require
 from nonebot.log import logger
 
-from ..common import CONF, get_bot, send_exception_to_su
+from ..common import send_exception_to_su
+from ..config import CONF
 from ..database import helper
 
 scheduler = require("nonebot_plugin_apscheduler").scheduler
 
 JOB_ID = "live_monitor"
 LOGNAME = "BTASK:LIVE"
 INTERVAL = CONF.bam_monitor_task_interval
```

### Comparing `nonebot_plugin_bam-0.1.5/nonebot_plugin_bam/user.py` & `nonebot_plugin_bam-0.2.0a1/nonebot_plugin_bam/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-from nonebot import get_driver, on_command
-from nonebot.adapters.cqhttp import Bot, Event
-from nonebot.adapters.cqhttp.permission import GROUP, PRIVATE
+from nonebot import on_command
+from nonebot.adapters.onebot.v11 import Message, MessageEvent
+from nonebot.params import CommandArg
 from nonebot.permission import SUPERUSER
 from nonebot.rule import to_me
 
 from .bilibili.user import user_info
 from .common import RE_NUMBER
 from .database import helper
 
 cmd_user_fetch = on_command(
     ("bam", "user", "fetch"), rule=to_me(), permission=SUPERUSER
 )
 
 
 @cmd_user_fetch.handle()
-async def user_fetch(bot: Bot, event: Event, state: dict):
-    args = str(event.message).strip()
+async def user_fetch(event: MessageEvent, args: Message = CommandArg()):
+    arg_text = args.extract_plain_text().strip()
 
-    if RE_NUMBER.match(args):
-        uid = int(args)
+    if RE_NUMBER.match(arg_text):
+        uid = int(arg_text)
 
-        bot.send_private_msg(user_id=event.user_id, message=f"开始获取 {uid} 用户信息")
+        await cmd_user_fetch.send(user_id=event.user_id, message=f"开始获取 {uid} 用户信息")
 
         user = await user_info(uid)
 
         if user.ok:
             helper.add_user(uid, user.nickname, user.rid)
             await cmd_user_fetch.finish(
                 f"UID: {uid}, 昵称: {user.nickname}, 直播间: {user.rid}, 已储存/更新完成。"
             )
-
         else:
             await cmd_user_fetch.finish(f"获取用户信息失败")
     else:
         await cmd_user_fetch.finish(f"UID 无效")
```

### Comparing `nonebot_plugin_bam-0.1.5/pyproject.toml` & `nonebot_plugin_bam-0.2.0a1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_bam"
-version = "0.1.5"
+version = "0.2.0a1"
 description = "Bilibili activity monitor plugin for nonebot"
 authors = ["7sDream <i@7sdre.am>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/7sDream/nonebot-plugin-bam"
 repository = "https://github.com/7sDream/nonebot-plugin-bam"
 keywords = ["nonebot", "bilibili", "qqbot"]
@@ -18,23 +18,26 @@
 ]
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-peewee = "^3.14.4"
-nonebot2 = "2.0.0.a10"
-aiohttp = {extras = ["speedups"], version = "^3.7.4"}
-nonebot-plugin-apscheduler = "^0.1.2"
-pydantic = "1.7.3"
+peewee = "^3.16.2"
+nonebot2 = "^2.0.0"
+aiohttp = {extras = ["speedups"], version = "^3.8.4"}
+nonebot-plugin-apscheduler = "^0.3.0"
+pydantic = "^1.10.9"
+nonebot-adapter-onebot = "^2.2.3"
 
-
-[tool.poetry.dev-dependencies]
-pylint = "^2.7.4"
-black = "^20.8b1"
-rope = "^0.18.0"
-pytest = "^6.2.3"
+[tool.poetry.group.dev.dependencies]
+pylint = "^2.17.4"
+black = "^23.3.0"
+rope = "^1.8.0"
+pytest = "^7.3.2"
+nonebot-adapter-console = "^0.3.2"
+pytest-asyncio = "^0.21.0"
+nonebot2 = {version = "^2.0.0", extras = ["fastapi"]}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_bam-0.1.5/setup.py` & `nonebot_plugin_bam-0.2.0a1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,215 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nonebot-plugin-bam
+Version: 0.2.0a1
+Summary: Bilibili activity monitor plugin for nonebot
+Home-page: https://github.com/7sDream/nonebot-plugin-bam
+License: MIT
+Keywords: nonebot,bilibili,qqbot
+Author: 7sDream
+Author-email: i@7sdre.am
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: aiohttp[speedups] (>=3.8.4,<4.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
+Requires-Dist: nonebot-plugin-apscheduler (>=0.3.0,<0.4.0)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
+Requires-Dist: peewee (>=3.16.2,<4.0.0)
+Requires-Dist: pydantic (>=1.10.9,<2.0.0)
+Project-URL: Repository, https://github.com/7sDream/nonebot-plugin-bam
+Description-Content-Type: text/markdown
 
-packages = \
-['nonebot_plugin_bam',
- 'nonebot_plugin_bam.bilibili',
- 'nonebot_plugin_bam.database',
- 'nonebot_plugin_bam.database.tables',
- 'nonebot_plugin_bam.tasks']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['aiohttp[speedups]>=3.7.4,<4.0.0',
- 'nonebot-plugin-apscheduler>=0.1.2,<0.2.0',
- 'nonebot2==2.0.0.a10',
- 'peewee>=3.14.4,<4.0.0',
- 'pydantic==1.7.3']
-
-setup_kwargs = {
-    'name': 'nonebot-plugin-bam',
-    'version': '0.1.5',
-    'description': 'Bilibili activity monitor plugin for nonebot',
-    'long_description': '# Bilibili Activity Monitor\n\nB 站用户监视器，自动监控用户的动态和直播状态，在有新动态和直播状态改变时向关注群发送提示信息。\n\n可多群共用，每个群可以有不同的关注列表。自带数据落地存储机制，重启后可保留各群关注状态。\n\n## 功能示例\n\n### 直播提醒\n\n![screenshot-live]\n\n### 动态提醒\n\n![screenshot-act-normal]\n\n![screenshot-act-repost]\n\n*特定用户 at 特定群友功能暂时没来得及做命令，目前需要直接改数据库，目前可以假装这个功能不存在。*\n\n## 使用\n\n```bash\npoetry add nonebot-plugin-bam\n```\n\n```python\nimport nonebot\nfrom nonebot.adapters.cqhttp import Bot as CQHTTPBot\n\nnonebot.init(_env_file=".env")\n\ndriver = nonebot.get_driver()\ndriver.register_adapter("cqhttp", CQHTTPBot)\n\nnonebot.load_builtin_plugins()\n\n# load other plugins\n\n# bam need this to manage background tasks\nnonebot.load_plugin("nonebot_plugin_apscheduler")\nnonebot.load_plugin("nonebot_plugin_bam")\n\nnonebot.run()\n```\n\n其中 `.env` 文件除了 nonebot 的常规配置项外，还有可添加以下配置属性（下面展示的是默认值）：\n\n```env\n# 我个人喜欢用 / 来做分隔符，下面的命令列表也是以 / 为例，可以按照自己喜欢的调整\nCOMMAND_START=["/"]\nCOMMAND_SEP=["/"]\n\n# 数据落地文件路径，建议设置一下。\n# 用默认值（储存在内存中）的话一重启数据就没了\nBAM_DB_FILE=":memory:"\n\n# 重启时将所有用户的直播状态设置为未开播，而不是使用上次记录的状态。\n# 正常使用不要打开此选项，是调试用的\nBAM_ON_STARTUP_CLEAN_LIVE_STATUS=false \n\n# 监控任务的间隔，这里设置的是每个用户间的间隔，而不是一轮的间隔。\n# 所以如果一共关注了 N 个人（多个群关注同一个人只算一个）\n# 那对于每个人来说，两次检测之间的间隔就是 N * interval\n# 一般来说不要设置在 5 以下，可能会被 B 站 API 反爬而拒绝响应\nBAM_TASK_INTERVAL=5\n\n# 使用那一个直播间状态查询 API，默认为 2，如果发现被封禁了可以临时调到 1 试试\nBAM_LIVE_API=2\n\n# 动态内容在发送到 QQ 时的最大长度，超过长度会截断，设置为 0 或负数表示不截断\nBAM_ACTIVITY_CONTENT_MAX_LENGTH=0\n```\n\n## 命令列表\n\n<details>\n<summary>点击展开</summary>\n\n### 群相关\n\n#### 群初始化\n\n命令：`@bot /bam/group/add [superuser_qq]`\n\nSUPERUSER ONLY，GROUP ONLY。\n\n在机器人加入群之后，首先使用此命令将群加入服务列表。\n\n参数：\n\n- superuser_qq：此群的 SUPERUSER，可以管理 Bot 在这个群的行为。可选参数，不填时则设置为使用此命令的人。\n\n#### 删除群\n\n命令：`@bot /bam/group/remove`\n\nSUPERUSER ONLY，GROUP ONLY。\n\n将当前群从服务列表中删除。\n\n#### 群列表\n\n命令：`/bam/group/list`\n\nSUPERUSER ONLY，PRIVATE ONLY。\n\n显示当前机器人服务的群列表。\n\n### 关注相关\n\n#### 添加关注\n\n命令：`[@bot] /bam/follower/add [qq_group_id] <bilibili_uid>`\n\nSUPERUSER ONLY, PRIVATE OR GROUP\n\n为群 `qq_group_id` 添加对 B 站用户 `bilibili_uid` 的监控。\n\n参数：\n\n- `qq_group_id`：操作群号。可选参数，如果在群聊中使用此命令则不能加此参数，默认为当前群。\n- `bilibili_uid`：B 站用户 UID，必填。\n\n注：`[@bot]` 表示在私聊中使用时不用(无法) at 机器人，下略。\n\n#### 删除关注\n\n命令：`[@bot] /bam/follower/remove [qq_group_id] <bilibili_uid>`\n\nSUPERUSER ONLY, PRIVATE OR GROUP\n\n为群 `qq_group_id` 删除对 B 站用户 `bilibili_uid` 的监控。\n\n参数：\n\n- `qq_group_id`：操作群号。可选参数，如果在群聊中使用此命令则不能加此参数，默认为当前群。\n- `bilibili_uid`：B 站用户 UID，必填。\n\n#### 群关注列表\n\n命令：`[@bot] /bam/follower/list [qq_group_id]`\n\nSUPERUSER ONLY, PRIVATE OR GROUP\n\n列出群 `qq_group_id` 的关注列表。\n\n参数：\n\n- `qq_group_id`：操作群号。可选参数，如果在群聊中使用此命令则不能加此参数，默认为当前群。\n\n### B 站相关\n\n#### 获取/更新用户数据\n\n命令：`[@bot] /bam/user/fetch <bilibili_uid>`\n\nSUPERUSER ONLY, PRIVATE OR GROUP\n\n获取或更新 B 站用户 `bilibili_uid` 的信息。\n\n参数：\n\n- `bilibili_uid`：B 站用户 UID，必填。\n\n#### 获取一个动态信息\n\n命令：`[@bot] /bam/act <bilibili_activity_id>`\n\nANYONE\n\n获取 B 站动态 `bilibili_activity_id` 的信息。\n\n参数：\n\n- `bilibili_activity_id`：B 站动态 ID。\n\n</details>\n\n## LICENSE\n\nMIT.\n\n[screenshot-live]: https://rikka.7sdre.am/files/af1c9c5a-5f8c-40df-b199-e97525368ec9.png\n[screenshot-act-normal]: https://rikka.7sdre.am/files/5350ce1c-63f6-4f43-abcc-004e9c722063.png\n[screenshot-act-repost]: https://rikka.7sdre.am/files/9c43a32b-2df7-4b93-be53-22c50a981c63.png\n',
-    'author': '7sDream',
-    'author_email': 'i@7sdre.am',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/7sDream/nonebot-plugin-bam',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+# Bilibili Activity Monitor
 
+B 站用户监视器，自动监控用户的动态和直播状态，在有新动态和直播状态改变时向关注群发送提示信息。
+
+可多群共用，每个群可以有不同的关注列表。自带数据落地存储机制，重启后可保留各群关注状态。
+
+## 功能示例
+
+### 直播提醒
+
+![screenshot-live]
+
+### 动态提醒
+
+![screenshot-act-normal]
+
+![screenshot-act-repost]
+
+*特定用户 at 特定群友功能暂时没来得及做命令，目前需要直接改数据库，目前可以假装这个功能不存在。*
+
+## 使用
+
+```bash
+poetry add nonebot-plugin-bam
+```
+
+```python
+import nonebot
+from nonebot.adapters.onebot.v11 import Adapter
+
+nonebot.init(_env_file=".env")
+
+driver = nonebot.get_driver()
+driver.register_adapter(Adapter)
+
+nonebot.load_builtin_plugins()
+
+# load other plugins
+
+# bam need this to manage background tasks
+nonebot.load_plugin("nonebot_plugin_apscheduler")
+nonebot.load_plugin("nonebot_plugin_bam")
+
+nonebot.run()
+```
+
+其中 `.env` 文件除了 nonebot 的常规配置项外，还有可添加以下配置属性（下面展示的是默认值）：
+
+```env
+# 我个人喜欢用 / 来做分隔符，下面的命令列表也是以 / 为例，可以按照自己喜欢的调整
+COMMAND_START=["/"]
+COMMAND_SEP=["/"]
+
+# 数据落地文件路径，建议设置一下。
+# 用默认值（储存在内存中）的话一重启数据就没了
+BAM_DB_FILE=":memory:"
+
+# 重启时将所有用户的直播状态设置为未开播，而不是使用上次记录的状态。
+# 正常使用不要打开此选项，是调试用的
+BAM_ON_STARTUP_CLEAN_LIVE_STATUS=false 
+
+# 监控任务的间隔，这里设置的是每个用户间的间隔，而不是一轮的间隔。
+# 所以如果一共关注了 N 个人（多个群关注同一个人只算一个）
+# 那对于每个人来说，两次检测之间的间隔就是 N * interval
+# 一般来说不要设置在 5 以下，可能会被 B 站 API 反爬而拒绝响应
+BAM_MONITOR_TASK_INTERVAL=5
+
+# 使用那一个直播间状态查询 API，默认为 2，如果发现被封禁了可以临时调到 1 试试
+BAM_LIVE_API=2
+
+# 动态内容在发送到 QQ 时的最大长度，超过长度会截断，设置为 0 或负数表示不截断
+BAM_ACTIVITY_CONTENT_MAX_LENGTH=0
+```
+
+## 命令列表
+
+<details>
+<summary>点击展开</summary>
+
+### 群相关
+
+#### 群初始化
+
+命令：`@bot /bam/group/add [superuser_qq]`
+
+SUPERUSER ONLY，GROUP ONLY。
+
+在机器人加入群之后，首先使用此命令将群加入服务列表。
+
+参数：
+
+- superuser_qq：此群的 SUPERUSER，可以管理 Bot 在这个群的行为。可选参数，不填时则设置为使用此命令的人。
+
+#### 删除群
+
+命令：`@bot /bam/group/remove`
+
+SUPERUSER ONLY，GROUP ONLY。
+
+将当前群从服务列表中删除。
+
+#### 群列表
+
+命令：`/bam/group/list`
+
+SUPERUSER ONLY，PRIVATE ONLY。
+
+显示当前机器人服务的群列表。
+
+### 关注相关
+
+#### 添加关注
+
+命令：`[@bot] /bam/follower/add [qq_group_id] <bilibili_uid>`
+
+SUPERUSER ONLY, PRIVATE OR GROUP
+
+为群 `qq_group_id` 添加对 B 站用户 `bilibili_uid` 的监控。
+
+参数：
+
+- `qq_group_id`：操作群号。可选参数，如果在群聊中使用此命令则不能加此参数，默认为当前群。
+- `bilibili_uid`：B 站用户 UID，必填。
+
+注：`[@bot]` 表示在私聊中使用时不用(无法) at 机器人，下略。
+
+#### 删除关注
+
+命令：`[@bot] /bam/follower/remove [qq_group_id] <bilibili_uid>`
+
+SUPERUSER ONLY, PRIVATE OR GROUP
+
+为群 `qq_group_id` 删除对 B 站用户 `bilibili_uid` 的监控。
+
+参数：
+
+- `qq_group_id`：操作群号。可选参数，如果在群聊中使用此命令则不能加此参数，默认为当前群。
+- `bilibili_uid`：B 站用户 UID，必填。
+
+#### 群关注列表
+
+命令：`[@bot] /bam/follower/list [qq_group_id]`
+
+SUPERUSER ONLY, PRIVATE OR GROUP
+
+列出群 `qq_group_id` 的关注列表。
+
+参数：
+
+- `qq_group_id`：操作群号。可选参数，如果在群聊中使用此命令则不能加此参数，默认为当前群。
+
+### B 站相关
+
+#### 获取/更新用户数据
+
+命令：`[@bot] /bam/user/fetch <bilibili_uid>`
+
+SUPERUSER ONLY, PRIVATE OR GROUP
+
+获取或更新 B 站用户 `bilibili_uid` 的信息。
+
+参数：
+
+- `bilibili_uid`：B 站用户 UID，必填。
+
+#### 获取一个动态信息
+
+命令：`[@bot] /bam/act <bilibili_activity_id>`
+
+ANYONE
+
+获取 B 站动态 `bilibili_activity_id` 的信息。
+
+参数：
+
+- `bilibili_activity_id`：B 站动态 ID。
+
+</details>
+
+## LICENSE
+
+MIT.
+
+[screenshot-live]: https://rikka.7sdre.am/files/af1c9c5a-5f8c-40df-b199-e97525368ec9.png
+[screenshot-act-normal]: https://rikka.7sdre.am/files/5350ce1c-63f6-4f43-abcc-004e9c722063.png
+[screenshot-act-repost]: https://rikka.7sdre.am/files/9c43a32b-2df7-4b93-be53-22c50a981c63.png
 
-setup(**setup_kwargs)
```

