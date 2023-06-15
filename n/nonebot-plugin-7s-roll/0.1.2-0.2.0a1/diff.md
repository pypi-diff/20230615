# Comparing `tmp/nonebot-plugin-7s-roll-0.1.2.tar.gz` & `tmp/nonebot_plugin_7s_roll-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-7s-roll-0.1.2.tar", last modified: Mon Feb  8 12:51:42 2021, max compression
+gzip compressed data, was "nonebot_plugin_7s_roll-0.2.0a1.tar", max compression
```

## Comparing `nonebot-plugin-7s-roll-0.1.2.tar` & `nonebot_plugin_7s_roll-0.2.0a1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1059 2021-02-07 18:47:13.900478 nonebot-plugin-7s-roll-0.1.2/LICENSE
--rw-r--r--   0        0        0     1757 2021-02-07 20:12:06.494829 nonebot-plugin-7s-roll-0.1.2/README.md
--rw-r--r--   0        0        0      154 2021-02-08 12:51:13.277120 nonebot-plugin-7s-roll-0.1.2/nonebot_plugin_7s_roll/__init__.py
--rw-r--r--   0        0        0     1991 2021-02-08 12:49:54.855631 nonebot-plugin-7s-roll-0.1.2/nonebot_plugin_7s_roll/command.py
--rw-r--r--   0        0        0      289 2021-02-07 19:41:14.102505 nonebot-plugin-7s-roll-0.1.2/nonebot_plugin_7s_roll/common.py
--rw-r--r--   0        0        0      178 2021-02-07 18:14:08.402502 nonebot-plugin-7s-roll-0.1.2/nonebot_plugin_7s_roll/config.py
--rw-r--r--   0        0        0     5447 2021-02-07 19:17:58.026673 nonebot-plugin-7s-roll-0.1.2/nonebot_plugin_7s_roll/expr.py
--rw-r--r--   0        0        0     2003 2021-02-07 20:10:09.812141 nonebot-plugin-7s-roll-0.1.2/nonebot_plugin_7s_roll/roll.py
--rw-r--r--   0        0        0     1069 2021-02-08 12:51:05.016244 nonebot-plugin-7s-roll-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2527 2021-02-08 12:51:42.483038 nonebot-plugin-7s-roll-0.1.2/setup.py
--rw-r--r--   0        0        0     2654 2021-02-08 12:51:42.483287 nonebot-plugin-7s-roll-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-06-15 14:37:09.263085 nonebot_plugin_7s_roll-0.2.0a1/LICENSE
+-rw-r--r--   0        0        0      317 2023-06-15 15:20:26.275167 nonebot_plugin_7s_roll-0.2.0a1/nonebot_plugin_7s_roll/__init__.py
+-rw-r--r--   0        0        0     2067 2023-06-15 15:16:46.889258 nonebot_plugin_7s_roll-0.2.0a1/nonebot_plugin_7s_roll/command.py
+-rw-r--r--   0        0        0      212 2023-06-15 15:04:46.601369 nonebot_plugin_7s_roll-0.2.0a1/nonebot_plugin_7s_roll/common.py
+-rw-r--r--   0        0        0      178 2023-06-15 14:37:09.264086 nonebot_plugin_7s_roll-0.2.0a1/nonebot_plugin_7s_roll/config.py
+-rw-r--r--   0        0        0     5736 2023-06-15 15:12:01.427116 nonebot_plugin_7s_roll-0.2.0a1/nonebot_plugin_7s_roll/expr.py
+-rw-r--r--   0        0        0     2003 2023-06-15 14:37:09.265086 nonebot_plugin_7s_roll-0.2.0a1/nonebot_plugin_7s_roll/roll.py
+-rw-r--r--   0        0        0     1123 2023-06-15 15:20:50.587710 nonebot_plugin_7s_roll-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0     1701 2023-06-15 14:38:13.472977 nonebot_plugin_7s_roll-0.2.0a1/README.md
+-rw-r--r--   0        0        0     2593 1970-01-01 00:00:00.000000 nonebot_plugin_7s_roll-0.2.0a1/PKG-INFO
```

### Comparing `nonebot-plugin-7s-roll-0.1.2/LICENSE` & `nonebot_plugin_7s_roll-0.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-7s-roll-0.1.2/README.md` & `nonebot_plugin_7s_roll-0.2.0a1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 # Roll Dice
 
 扔骰子小工具。
 
 ## 使用
 
 ```python
-import nonebot
-from nonebot.adapters.cqhttp import Bot as CQHTTPBot
-
-nonebot.init(_env_file=".env")
-driver = nonebot.get_driver()
-driver.register_adapter("cqhttp", CQHTTPBot)
-nonebot.load_builtin_plugins()
-
-# load other plugins
-
+# load your driver, set adapter, builtin plugin etc.
 nonebot.load_plugin("nonebot_plugin_7s_roll")
-
 nonebot.run()
 ```
 
 其中 .env 文件除了 nonebot 的常规配置项外，还有可添加以下配置属性（示例中的是默认值）：
 
 ```env
 # 命令名（在 at 机器人时使用， `@bot /roll 1d10`）
@@ -76,10 +66,16 @@
 `roll 3d100max+4d10`
 
 ```text
 3d100max+4d10 投掷结果
 (max[35, 60, 29] = 60) + (1 + 1 + 5 + 8) = 75
 ```
 
+## 截图
+
+![screenshot-dice]
+
 ## LICENSE
 
 MIT.
+
+[screenshot-dice]: https://rikka.7sdre.am/files/8c6c5b15-0343-4d14-a203-422c7d6c634e.png
```

### Comparing `nonebot-plugin-7s-roll-0.1.2/nonebot_plugin_7s_roll/command.py` & `nonebot_plugin_7s_roll-0.2.0a1/nonebot_plugin_7s_roll/command.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import re
+from typing import Annotated
 
-from nonebot import on_message, on_command
-from nonebot.adapters import Bot, Event
+from nonebot import on_command, on_message
+from nonebot.adapters import Event
+from nonebot.consts import REGEX_MATCHED
 from nonebot.log import logger
-from nonebot.adapters.cqhttp.permission import GROUP
-from nonebot.adapters.cqhttp.message import Message
+from nonebot.params import EventPlainText
 from nonebot.rule import regex
+from nonebot.typing import T_State
 
-from .common import START, SEP, CONF
+from .common import CONF, START
 from .roll import roll
 
 RE_ROLL_STR = (
     "^("  # 1
     + START
     + CONF.i7s_roll_command
     + " |"
@@ -19,43 +21,43 @@
     #      2                     3  4      5                                    6
     + r" )([0-9adgimnsuvx+\- ]+)( ?(结果)?(大于|小于|大于等于|小于等于|>=|>|<|<=) ?(-?\d{1,10}))?"
 )
 
 RE_ROLL_CMD = re.compile(RE_ROLL_STR)
 
 
-async def roll_command_handler(bot: Bot, event: Event, state: dict):
+async def roll_command_handler(event: Event, msg: Annotated[str, EventPlainText()], state: T_State):
     messages = []
 
-    logger.info(f"[7sRoll] received roll command: {event.raw_message}")
+    logger.info(f"[7sRoll] received roll command: {msg}")
 
-    if await GROUP(bot, event):
-        messages.append(f"[CQ:at,qq={event.user_id}]")
+    if event.get_event_name().startswith("message.group"): # onebot v11
+        messages.append(f"[CQ:at,qq={event.user_id}]") # type: ignore
 
     match = None
-    if "_match" in state:
-        match = state["_matched"]
+    if REGEX_MATCHED in state:
+        match = state[REGEX_MATCHED]
     else:
-        args = str(event.raw_message).strip()
+        args = msg.strip()
         match = RE_ROLL_CMD.match(args)
         if not match:
             messages.append("roll 命令格式错误")
             messages.append("格式为：roll <表达式>[ <判断方式><目标>]")
             messages.append("表达式举例：3d6+1d3-1")
             messages.append("判断方式可选：>, <, <=, >=, 或对应中文")
             messages.append("目标：需要达成的点数")
-            return await cmd_roll.finish(Message("\n".join(messages)))
+            return await cmd_roll.finish("\n".join(messages))
         if match.group(1) is None:
             return
 
     expr_str, op_str, target = match.group(2, 5, 6)
 
     messages.extend(roll(expr_str, op_str, target))
 
-    return await cmd_roll.finish(Message("\n".join(messages)))
+    return await cmd_roll.finish("\n".join(messages))
 
 
 cmd_roll = on_command(CONF.i7s_roll_command, priority=1, block=True)
 cmd_roll.handle()(roll_command_handler)
 
 message_cmd_roll = on_message(rule=regex(RE_ROLL_STR), priority=2, block=True)
 message_cmd_roll.handle()(roll_command_handler)
```

### Comparing `nonebot-plugin-7s-roll-0.1.2/nonebot_plugin_7s_roll/expr.py` & `nonebot_plugin_7s_roll-0.2.0a1/nonebot_plugin_7s_roll/expr.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import enum
 import abc
 import math
 import random
 import re
+from typing import Dict, List, Optional, Tuple
 
 
 class Op(abc.ABC):
     @abc.abstractmethod
-    def __call__(self, left: (int, str), right: (int, str)) -> (int, str):
+    def __call__(self, left: Tuple[int, str], right: Tuple[int, str]) -> Tuple[int, str]:
         pass
 
 
 class __Add(Op):
-    def __call__(self, left: (int, str), right: (int, str)) -> (int, str):
+    def __call__(self, left: Tuple[int, str], right: Tuple[int, str]) -> Tuple[int, str]:
         val = left[0] + right[0]
         return val, f"{left[1]} + {right[1]}"
 
 
 class __Minus(Op):
-    def __call__(self, left: (int, str), right: (int, str)) -> (int, str):
+    def __call__(self, left: Tuple[int, str], right: Tuple[int, str]) -> Tuple[int, str]:
         val = left[0] - right[0]
         return val, f"{left[1]} - {right[1]}"
 
 
 ADD = __Add()
 MINUS = __Minus()
 
@@ -34,131 +34,133 @@
 
 class PostProcessor(abc.ABC):
     @abc.abstractproperty
     def prefix(self):
         pass
 
     @abc.abstractmethod
-    def __call__(self, values: [int]) -> (int, str):
+    def __call__(self, values: List[int]) -> Tuple[int, str]:
         pass
 
 
 class __MaxPostProcessor(PostProcessor):
     @property
     def prefix(self):
         return "最大值为"
 
-    def __call__(self, values: [int]) -> (int, str):
+    def __call__(self, values: List[int]) -> Tuple[int, str]:
         val = max(values)
         if len(values) == 1:
             s = str(val)
         else:
             s = "".join(["(max[", ", ".join(map(str, values)), "] = ", str(val), ")"])
         return val, s
 
 
 class __MinPostProcessor(PostProcessor):
     @property
     def prefix(self):
         return "最小值为"
 
-    def __call__(self, values: [int]) -> (int, str):
+    def __call__(self, values: List[int]) -> Tuple[int, str]:
         val = min(values)
         if len(values) == 1:
             s = str(val)
         else:
             s = "".join(["(min[", ", ".join(map(str, values)), "] = ", str(val), ")"])
         return val, s
 
 
 class __AvgPostProcessor(PostProcessor):
     @property
     def prefix(self):
         return "平均值为"
 
-    def __call__(self, values: [int]) -> (int, str):
+    def __call__(self, values: List[int]) -> Tuple[int, str]:
         val = math.floor(sum(values) / len(values))
         if len(values) == 1:
             s = str(val)
         else:
             s = "".join(["(avg[", ", ".join(map(str, values)), "] = ", str(val), ")"])
         return val, s
 
 
 class __SumPostProcessor(PostProcessor):
     @property
     def prefix(self):
         return "总和为"
 
-    def __call__(self, values: [int]) -> (int, str):
+    def __call__(self, values: List[int]) -> Tuple[int, str]:
         val = sum(values)
         if len(values) == 1:
             s = str(val)
         else:
             s = "".join(["(", " + ".join(map(str, values)), ")"])
         return val, s
 
 
 MAX = __MaxPostProcessor()
 MIN = __MinPostProcessor()
 AVG = __AvgPostProcessor()
 SUM = __SumPostProcessor()
 
-POST_PROCESS_MAP = {
+POST_PROCESS_MAP: Dict[str, PostProcessor] = {
     "max": MAX,
     "min": MIN,
     "avg": AVG,
     "sum": SUM,
 }
 
 
 class Expr(abc.ABC):
     @abc.abstractmethod
-    def __call__(self) -> (int, str):
+    def __call__(self) -> Tuple[int, str]:
         pass
 
 
 class OpExpr(Expr):
     def __init__(self, left: Expr, op: Op, right: Expr):
         self.left = left
         self.op = op
         self.right = right
 
-    def __call__(self) -> (int, str):
+    def __call__(self) -> Tuple[int, str]:
         return self.op(self.left(), self.right())
 
 
 class Num(Expr):
     def __init__(self, val):
         self.val = val
 
     def __call__(self):
         return self.val, str(self.val)
 
 
 class Roll(Expr):
-    def __init__(self, times: int, faces: int, postprocessor: PostProcessor = None):
+    post_processor: PostProcessor
+
+    def __init__(self, times: int, faces: int, postprocessor: Optional[PostProcessor] = None):
         self.times = times
         self.faces = faces
-        self.post_processor = postprocessor
-        if self.post_processor is None:
-            self.post_processor = SUM
+        self.post_processor = SUM
+        if postprocessor is not None:
+            self.post_processor = postprocessor
         self.values = []
 
     def __call__(self):
         self.values = [random.randint(1, self.faces) for _ in range(self.times)]
         return self.post_processor(self.values)
 
 
 RE_ROLL = re.compile(r"(\d+){1,2}[dD](\d+){1,4}(min|max|avg|sum|取小|取大|平均|求和)?")
 RE_OP = re.compile(r"[+\-]")
 RE_NUM = re.compile(r"\d+")
 
 
-def tokenize(s: str):
+def tokenize(s: str) -> Optional[List[Expr]]:
     s = s.replace(" ", "")
     tokens = []
     pos = 0
     roll_count = 0
     while pos < len(s):
         match = RE_ROLL.match(s, pos)
         if match:
@@ -166,15 +168,15 @@
             times, faces, post = match.group(1, 2, 3)
             times = int(times)
             faces = int(faces)
             if times == 0 or times > 20:
                 return None
             if faces == 0 or faces > 1000:
                 return None
-            if post:
+            if isinstance(post, str):
                 post = POST_PROCESS_MAP[post]
             tokens.append(Roll(times, faces, post))
             roll_count += 1
             if roll_count > 20:
                 return None
             continue
         match = RE_OP.match(s, pos)
@@ -187,15 +189,15 @@
             pos = match.end()
             tokens.append(Num(int(match.group(0))))
             continue
         return None
     return tokens
 
 
-def parse(tokens: list) -> Expr:
+def parse(tokens: Optional[List[Expr]]) -> Optional[Expr]:
     if tokens is None:
         return None
     while True:
         i = 0
         expr = None
         for i, item in enumerate(tokens):
             if isinstance(item, Op):
@@ -217,9 +219,9 @@
 
     if not isinstance(ast, Expr) or isinstance(ast, Num):
         return None
 
     return ast
 
 
-def compile(s):
+def compile(s) -> Optional[Expr]:
     return parse(tokenize(s))
```

### Comparing `nonebot-plugin-7s-roll-0.1.2/nonebot_plugin_7s_roll/roll.py` & `nonebot_plugin_7s_roll-0.2.0a1/nonebot_plugin_7s_roll/roll.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-7s-roll-0.1.2/pyproject.toml` & `nonebot_plugin_7s_roll-0.2.0a1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 [tool.poetry]
 name = "nonebot-plugin-7s-roll"
-version = "0.1.2"
+version = "0.2.0a1"
 description = "A roll dice plugin for nonebot"
 authors = ["7sDream <i@7sdre.am>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/7sDream/nonebot_plugin_7s_roll"
 repository = "https://github.com/7sDream/nonebot_plugin_7s_roll"
 keywords = ["nonebot", "dice", "roll", "trpg"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Plugins",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-nonebot2 = {version = "^2.0.0-alpha.10", allow-prereleases = true}
+python = "^3.9"
+nonebot2 = "^2.0.0"
 
-[tool.poetry.dev-dependencies]
-pytest = "^5.2"
-pylint = "^2.6.0"
-black = "^20.8b1"
-rope = "^0.18.0"
+[tool.poetry.group.dev.dependencies]
+pylint = "^2.17.4"
+black = "^23.3.0"
+rope = "^1.8.0"
+pytest = "^7.3.2"
+nonebot-adapter-console = "^0.3.2"
+nonebot2 = {version = "^2.0.0", extras = ["fastapi"]}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot-plugin-7s-roll-0.1.2/PKG-INFO` & `nonebot_plugin_7s_roll-0.2.0a1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,39 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-7s-roll
-Version: 0.1.2
+Version: 0.2.0a1
 Summary: A roll dice plugin for nonebot
 Home-page: https://github.com/7sDream/nonebot_plugin_7s_roll
 License: MIT
 Keywords: nonebot,dice,roll,trpg
 Author: 7sDream
 Author-email: i@7sdre.am
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: nonebot2 (>=2.0.0-alpha.10,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/7sDream/nonebot_plugin_7s_roll
 Description-Content-Type: text/markdown
 
 # Roll Dice
 
 扔骰子小工具。
 
 ## 使用
 
 ```python
-import nonebot
-from nonebot.adapters.cqhttp import Bot as CQHTTPBot
-
-nonebot.init(_env_file=".env")
-driver = nonebot.get_driver()
-driver.register_adapter("cqhttp", CQHTTPBot)
-nonebot.load_builtin_plugins()
-
-# load other plugins
-
+# load your driver, set adapter, builtin plugin etc.
 nonebot.load_plugin("nonebot_plugin_7s_roll")
-
 nonebot.run()
 ```
 
 其中 .env 文件除了 nonebot 的常规配置项外，还有可添加以下配置属性（示例中的是默认值）：
 
 ```env
 # 命令名（在 at 机器人时使用， `@bot /roll 1d10`）
@@ -99,11 +89,17 @@
 `roll 3d100max+4d10`
 
 ```text
 3d100max+4d10 投掷结果
 (max[35, 60, 29] = 60) + (1 + 1 + 5 + 8) = 75
 ```
 
+## 截图
+
+![screenshot-dice]
+
 ## LICENSE
 
 MIT.
 
+[screenshot-dice]: https://rikka.7sdre.am/files/8c6c5b15-0343-4d14-a203-422c7d6c634e.png
+
```

