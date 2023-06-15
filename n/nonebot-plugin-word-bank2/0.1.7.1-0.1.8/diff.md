# Comparing `tmp/nonebot_plugin_word_bank2-0.1.7.1.tar.gz` & `tmp/nonebot_plugin_word_bank2-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_word_bank2-0.1.7.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_word_bank2-0.1.8.tar", max compression
```

## Comparing `nonebot_plugin_word_bank2-0.1.7.1.tar` & `nonebot_plugin_word_bank2-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-04-15 12:39:44.470098 nonebot_plugin_word_bank2-0.1.7.1/LICENSE
--rw-r--r--   0        0        0     3735 2023-04-15 12:39:44.470098 nonebot_plugin_word_bank2-0.1.7.1/README.md
--rw-r--r--   0        0        0     8904 2023-04-15 12:39:44.470098 nonebot_plugin_word_bank2-0.1.7.1/nonebot_plugin_word_bank2/__init__.py
--rw-r--r--   0        0        0     9334 2023-04-15 12:39:44.470098 nonebot_plugin_word_bank2-0.1.7.1/nonebot_plugin_word_bank2/data_source.py
--rw-r--r--   0        0        0      225 2023-04-15 12:39:44.470098 nonebot_plugin_word_bank2-0.1.7.1/nonebot_plugin_word_bank2/models.py
--rw-r--r--   0        0        0     4438 2023-04-15 12:39:44.470098 nonebot_plugin_word_bank2-0.1.7.1/nonebot_plugin_word_bank2/util.py
--rw-r--r--   0        0        0     2303 2023-04-15 12:39:44.470098 nonebot_plugin_word_bank2-0.1.7.1/nonebot_plugin_word_bank2/word_entry.py
--rw-r--r--   0        0        0      547 2023-04-15 12:39:44.470098 nonebot_plugin_word_bank2-0.1.7.1/pyproject.toml
--rw-r--r--   0        0        0     4489 1970-01-01 00:00:00.000000 nonebot_plugin_word_bank2-0.1.7.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-15 04:19:43.072460 nonebot_plugin_word_bank2-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3735 2023-06-15 04:19:43.072460 nonebot_plugin_word_bank2-0.1.8/README.md
+-rw-r--r--   0        0        0     9541 2023-06-15 04:19:43.072460 nonebot_plugin_word_bank2-0.1.8/nonebot_plugin_word_bank2/__init__.py
+-rw-r--r--   0        0        0     9334 2023-06-15 04:19:43.072460 nonebot_plugin_word_bank2-0.1.8/nonebot_plugin_word_bank2/data_source.py
+-rw-r--r--   0        0        0      225 2023-06-15 04:19:43.072460 nonebot_plugin_word_bank2-0.1.8/nonebot_plugin_word_bank2/models.py
+-rw-r--r--   0        0        0     4438 2023-06-15 04:19:43.072460 nonebot_plugin_word_bank2-0.1.8/nonebot_plugin_word_bank2/util.py
+-rw-r--r--   0        0        0     2303 2023-06-15 04:19:43.072460 nonebot_plugin_word_bank2-0.1.8/nonebot_plugin_word_bank2/word_entry.py
+-rw-r--r--   0        0        0      538 2023-06-15 04:19:43.072460 nonebot_plugin_word_bank2-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     4480 1970-01-01 00:00:00.000000 nonebot_plugin_word_bank2-0.1.8/PKG-INFO
```

### Comparing `nonebot_plugin_word_bank2-0.1.7.1/LICENSE` & `nonebot_plugin_word_bank2-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_word_bank2-0.1.7.1/README.md` & `nonebot_plugin_word_bank2-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_word_bank2-0.1.7.1/nonebot_plugin_word_bank2/__init__.py` & `nonebot_plugin_word_bank2-0.1.8/nonebot_plugin_word_bank2/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,19 +10,35 @@
 from nonebot.permission import SUPERUSER
 from nonebot.adapters.onebot.v11 import Bot, Message, MessageEvent, GroupMessageEvent
 from nonebot.adapters.onebot.v11.permission import (
     GROUP_ADMIN,
     GROUP_OWNER,
     PRIVATE_FRIEND,
 )
+from nonebot.plugin import PluginMetadata
 
 from .util import to_json, parse_msg, save_and_convert_img
 from .models import MatchType, IncludeCQCodeError
 from .data_source import word_bank as wb
 
+__plugin_meta__ = PluginMetadata(
+    name="nonebot-plugin-word-bank2",
+    description=r"无数据库的轻量问答插件",
+    usage="""具体看文档
+    问答教学: [模糊|全局|正则|@]问...答...
+    删除词条: 删除[模糊|全局|正则|@]词条 问句
+    删除词库: /删除词库 /删除全局词库 /删除全部词库
+    查询词条: 查询[群|用户]{id}[全局][模糊|正则]词库
+        查询[模糊|正则]词库
+    """,
+    type="application",
+    supported_adapters={"~onebot.v11"},
+    homepage="https://github.com/kexue-z/nonebot-plugin-word-bank2",
+)
+
 reply_type = "random"
 
 
 def get_session_id(event: MessageEvent) -> str:
     if isinstance(event, GroupMessageEvent):
         return f"group_{event.group_id}"
     else:
@@ -106,15 +122,15 @@
     await save_and_convert_img(value, wb.img_dir)  # 保存回答中的图片
 
     index = get_session_id(event)
     index = "0" if "全局" in flag else index
     try:
         # 这个问题很奇怪, 有的设备上没有问题, 有的设备有问题
         # 替换掉莫名出现的 amp; 来解决
-        wb.set(index, type_, Message(key.replace("amp;", '')), value, require_to_me)
+        wb.set(index, type_, Message(key.replace("amp;", "")), value, require_to_me)
         await matcher.finish(message="我记住了~")
     except IncludeCQCodeError:
         await matcher.finish("正则匹配中不允许带有CQ码")
 
 
 wb_del_cmd = on_regex(
     r"^删除\s*((?:模糊|正则|@)*)\s*词条\s*(\S+.*?)\s*$",
@@ -157,15 +173,15 @@
             if key.startswith(name):
                 key = key.replace(name, "", 1)
                 require_to_me = True
                 break
 
     index = get_session_id(event)
     index = "0" if "全局" in flag else index
-    res = wb.delete(index, type_, Message(key.replace("amp;", '')), require_to_me)
+    res = wb.delete(index, type_, Message(key.replace("amp;", "")), require_to_me)
     if res:
         await matcher.finish("删除成功~")
 
 
 def wb_clear(type_: str = "") -> T_Handler:
     async def wb_clear_(
         event: MessageEvent, state: T_State, arg: Message = CommandArg()
@@ -271,15 +287,15 @@
     if not (require_to_me := "@" in flag):
         for name in bot.config.nickname:
             if key.startswith(name):
                 key = key.replace(name, "", 1)
                 require_to_me = True
                 break
 
-    entrys = wb.select(index, type_, Message(key.replace("amp;", '')), require_to_me)
+    entrys = wb.select(index, type_, Message(key.replace("amp;", "")), require_to_me)
 
     if not entrys:
         await matcher.finish("词库中未找到词条~")
 
     if isinstance(event, GroupMessageEvent):
         forward_msg: List[Dict] = []
         for entry in entrys:
```

### Comparing `nonebot_plugin_word_bank2-0.1.7.1/nonebot_plugin_word_bank2/data_source.py` & `nonebot_plugin_word_bank2-0.1.8/nonebot_plugin_word_bank2/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_word_bank2-0.1.7.1/nonebot_plugin_word_bank2/util.py` & `nonebot_plugin_word_bank2-0.1.8/nonebot_plugin_word_bank2/util.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_word_bank2-0.1.7.1/nonebot_plugin_word_bank2/word_entry.py` & `nonebot_plugin_word_bank2-0.1.8/nonebot_plugin_word_bank2/word_entry.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_word_bank2-0.1.7.1/pyproject.toml` & `nonebot_plugin_word_bank2-0.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 authors = ["kexue <x@kexue.io>"]
 description = "无数据问答插件"
 homepage = "https://github.com/kexue-z/nonebot-plugin-word-bank2"
 license = "GPL-3.0"
 name = "nonebot-plugin-word-bank2"
 readme = "README.md"
-version = "0.1.7.1"
+version = "0.1.8"
 
 [tool.poetry.dependencies]
 httpx = ">=0.18.0,<1.0.0"
 nonebot-adapter-onebot = ">=2.0.0-beta.1"
-nonebot2 = ">=2.0.0-beta.4"
+nonebot2 = ">=2.0.0"
 python = "^3.8"
 
 [tool.poetry.dev-dependencies]
 black = "^22.1.0"
 flake8 = "^4.0.1"
 
 [build-system]
```

### Comparing `nonebot_plugin_word_bank2-0.1.7.1/PKG-INFO` & `nonebot_plugin_word_bank2-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-word-bank2
-Version: 0.1.7.1
+Version: 0.1.8
 Summary: 无数据问答插件
 Home-page: https://github.com/kexue-z/nonebot-plugin-word-bank2
 License: GPL-3.0
 Author: kexue
 Author-email: x@kexue.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.18.0,<1.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.0.0-beta.1)
-Requires-Dist: nonebot2 (>=2.0.0-beta.4)
+Requires-Dist: nonebot2 (>=2.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # nonebot-plugin-word-bank2
 
 _✨ 无数据库的轻量问答插件 ✨_
```

