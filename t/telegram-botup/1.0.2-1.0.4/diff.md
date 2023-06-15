# Comparing `tmp/telegram_botup-1.0.2-py3-none-any.whl.zip` & `tmp/telegram_botup-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,50 +1,48 @@
-Zip file size: 41928 bytes, number of entries: 48
--rw-rw-r--  2.0 unx       89 b- defN 23-Jun-13 09:39 botup/__init__.py
--rw-rw-r--  2.0 unx      905 b- defN 23-Jun-13 09:12 botup/bot.py
+Zip file size: 41317 bytes, number of entries: 46
+-rw-rw-r--  2.0 unx      148 b- defN 23-Jun-15 18:16 botup/__init__.py
+-rw-rw-r--  2.0 unx    52863 b- defN 23-Jun-15 17:56 botup/api.py
+-rw-rw-r--  2.0 unx      895 b- defN 23-Jun-15 17:57 botup/bot.py
+-rw-rw-r--  2.0 unx    15290 b- defN 23-Jun-15 18:02 botup/dispatcher.py
+-rw-rw-r--  2.0 unx     9769 b- defN 23-Jun-15 18:01 botup/handlers.py
 -rw-rw-r--  2.0 unx     1266 b- defN 23-Jun-13 09:13 botup/navigation.py
--rw-rw-r--  2.0 unx      331 b- defN 23-Jun-13 09:13 botup/utils.py
--rw-rw-r--  2.0 unx     1948 b- defN 23-Jun-13 09:13 botup/widget.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Jun-13 09:53 botup/core/__init__.py
--rw-rw-r--  2.0 unx    52888 b- defN 23-Jun-13 09:14 botup/core/api.py
--rw-rw-r--  2.0 unx    15305 b- defN 23-Jun-13 09:14 botup/core/dispatcher.py
--rw-rw-r--  2.0 unx     9774 b- defN 23-Jun-13 09:15 botup/core/handlers.py
--rw-rw-r--  2.0 unx    47430 b- defN 23-Jun-13 09:15 botup/core/types.py
--rw-rw-r--  2.0 unx      228 b- defN 23-Jun-13 08:57 botup/core/utils.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Jun-13 09:53 botup/core/constants/__init__.py
--rw-rw-r--  2.0 unx     5243 b- defN 23-Jun-13 08:57 botup/core/constants/api_method.py
--rw-rw-r--  2.0 unx      115 b- defN 23-Jun-13 08:57 botup/core/constants/base.py
--rw-rw-r--  2.0 unx      470 b- defN 23-Jun-13 08:57 botup/core/constants/bot_command_scope_type.py
--rw-rw-r--  2.0 unx      562 b- defN 23-Jun-13 08:57 botup/core/constants/chat_action.py
--rw-rw-r--  2.0 unx      322 b- defN 23-Jun-13 08:57 botup/core/constants/chat_member_status.py
--rw-rw-r--  2.0 unx      200 b- defN 23-Jun-13 08:57 botup/core/constants/chat_type.py
--rw-rw-r--  2.0 unx      920 b- defN 23-Jun-13 08:57 botup/core/constants/encrypted_passport_element_type.py
--rw-rw-r--  2.0 unx      294 b- defN 23-Jun-13 08:57 botup/core/constants/inline_query_chat_type.py
--rw-rw-r--  2.0 unx      624 b- defN 23-Jun-13 08:57 botup/core/constants/inline_query_result_type.py
--rw-rw-r--  2.0 unx      172 b- defN 23-Jun-13 08:57 botup/core/constants/input_file_type.py
--rw-rw-r--  2.0 unx      258 b- defN 23-Jun-13 08:57 botup/core/constants/input_media_type.py
--rw-rw-r--  2.0 unx      229 b- defN 23-Jun-13 08:57 botup/core/constants/mask_position_point.py
--rw-rw-r--  2.0 unx      194 b- defN 23-Jun-13 08:57 botup/core/constants/menu_button_type.py
--rw-rw-r--  2.0 unx      774 b- defN 23-Jun-13 08:57 botup/core/constants/message_entity_type.py
--rw-rw-r--  2.0 unx      572 b- defN 23-Jun-13 08:57 botup/core/constants/passport_element_error_source.py
--rw-rw-r--  2.0 unx      132 b- defN 23-Jun-13 08:57 botup/core/constants/poll_type.py
--rw-rw-r--  2.0 unx      184 b- defN 23-Jun-13 08:57 botup/core/constants/sticker_type.py
--rw-rw-r--  2.0 unx     1622 b- defN 23-Jun-13 08:57 botup/core/constants/update_type.py
+-rw-rw-r--  2.0 unx    47350 b- defN 23-Jun-15 18:09 botup/types.py
+-rw-rw-r--  2.0 unx      505 b- defN 23-Jun-15 17:55 botup/utils.py
+-rw-rw-r--  2.0 unx     1933 b- defN 23-Jun-15 17:57 botup/widget.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jun-13 09:53 botup/constants/__init__.py
+-rw-rw-r--  2.0 unx     5243 b- defN 23-Jun-13 08:57 botup/constants/api_method.py
+-rw-rw-r--  2.0 unx      115 b- defN 23-Jun-13 08:57 botup/constants/base.py
+-rw-rw-r--  2.0 unx      470 b- defN 23-Jun-13 08:57 botup/constants/bot_command_scope_type.py
+-rw-rw-r--  2.0 unx      562 b- defN 23-Jun-13 08:57 botup/constants/chat_action.py
+-rw-rw-r--  2.0 unx      322 b- defN 23-Jun-13 08:57 botup/constants/chat_member_status.py
+-rw-rw-r--  2.0 unx      200 b- defN 23-Jun-13 08:57 botup/constants/chat_type.py
+-rw-rw-r--  2.0 unx      920 b- defN 23-Jun-13 08:57 botup/constants/encrypted_passport_element_type.py
+-rw-rw-r--  2.0 unx      294 b- defN 23-Jun-13 08:57 botup/constants/inline_query_chat_type.py
+-rw-rw-r--  2.0 unx      624 b- defN 23-Jun-13 08:57 botup/constants/inline_query_result_type.py
+-rw-rw-r--  2.0 unx      172 b- defN 23-Jun-13 08:57 botup/constants/input_file_type.py
+-rw-rw-r--  2.0 unx      258 b- defN 23-Jun-13 08:57 botup/constants/input_media_type.py
+-rw-rw-r--  2.0 unx      229 b- defN 23-Jun-13 08:57 botup/constants/mask_position_point.py
+-rw-rw-r--  2.0 unx      194 b- defN 23-Jun-13 08:57 botup/constants/menu_button_type.py
+-rw-rw-r--  2.0 unx      774 b- defN 23-Jun-13 08:57 botup/constants/message_entity_type.py
+-rw-rw-r--  2.0 unx      572 b- defN 23-Jun-13 08:57 botup/constants/passport_element_error_source.py
+-rw-rw-r--  2.0 unx      132 b- defN 23-Jun-13 08:57 botup/constants/poll_type.py
+-rw-rw-r--  2.0 unx      184 b- defN 23-Jun-13 08:57 botup/constants/sticker_type.py
+-rw-rw-r--  2.0 unx     1622 b- defN 23-Jun-13 08:57 botup/constants/update_type.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-13 09:53 botup/mixins/__init__.py
--rw-rw-r--  2.0 unx      409 b- defN 23-Jun-13 09:14 botup/mixins/echo.py
+-rw-rw-r--  2.0 unx      404 b- defN 23-Jun-15 18:02 botup/mixins/echo.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-13 09:53 botup/state_manager/__init__.py
 -rw-rw-r--  2.0 unx     2045 b- defN 23-Jun-13 08:57 botup/state_manager/base.py
--rw-rw-r--  2.0 unx      990 b- defN 23-Jun-13 09:13 botup/state_manager/redis.py
+-rw-rw-r--  2.0 unx     1003 b- defN 23-Jun-15 18:22 botup/state_manager/redis.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-13 09:53 botup/widgets/__init__.py
--rw-rw-r--  2.0 unx     8930 b- defN 23-Jun-13 08:57 botup/widgets/date_picker.py
+-rw-rw-r--  2.0 unx     8920 b- defN 23-Jun-15 18:02 botup/widgets/date_picker.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-May-15 21:45 tests/__init__.py
 -rw-rw-r--  2.0 unx      119 b- defN 23-Jun-13 09:17 tests/conftest.py
 -rw-rw-r--  2.0 unx    32361 b- defN 22-Aug-26 20:36 tests/test_dispatcher.py
 -rw-rw-r--  2.0 unx    10599 b- defN 22-Aug-26 20:36 tests/test_dispatcher_decorator.py
 -rw-rw-r--  2.0 unx     6708 b- defN 23-Jun-13 08:57 tests/test_dispatcher_registration.py
 -rw-rw-r--  2.0 unx      441 b- defN 23-Jun-13 08:57 tests/test_serializing.py
 -rw-rw-r--  2.0 unx    35379 b- defN 23-Jun-13 08:57 tests/utils.py
--rw-rw-r--  2.0 unx     4496 b- defN 23-Jun-13 09:54 telegram_botup-1.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-13 09:54 telegram_botup-1.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       12 b- defN 23-Jun-13 09:54 telegram_botup-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4109 b- defN 23-Jun-13 09:54 telegram_botup-1.0.2.dist-info/RECORD
-48 files, 249741 bytes uncompressed, 35322 bytes compressed:  85.9%
+-rw-rw-r--  2.0 unx     4441 b- defN 23-Jun-15 18:33 telegram_botup-1.0.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-15 18:33 telegram_botup-1.0.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       12 b- defN 23-Jun-15 18:33 telegram_botup-1.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3845 b- defN 23-Jun-15 18:33 telegram_botup-1.0.4.dist-info/RECORD
+46 files, 249275 bytes uncompressed, 35175 bytes compressed:  85.9%
```

## zipnote {}

```diff
@@ -1,95 +1,89 @@
 Filename: botup/__init__.py
 Comment: 
 
-Filename: botup/bot.py
-Comment: 
-
-Filename: botup/navigation.py
-Comment: 
-
-Filename: botup/utils.py
+Filename: botup/api.py
 Comment: 
 
-Filename: botup/widget.py
+Filename: botup/bot.py
 Comment: 
 
-Filename: botup/core/__init__.py
+Filename: botup/dispatcher.py
 Comment: 
 
-Filename: botup/core/api.py
+Filename: botup/handlers.py
 Comment: 
 
-Filename: botup/core/dispatcher.py
+Filename: botup/navigation.py
 Comment: 
 
-Filename: botup/core/handlers.py
+Filename: botup/types.py
 Comment: 
 
-Filename: botup/core/types.py
+Filename: botup/utils.py
 Comment: 
 
-Filename: botup/core/utils.py
+Filename: botup/widget.py
 Comment: 
 
-Filename: botup/core/constants/__init__.py
+Filename: botup/constants/__init__.py
 Comment: 
 
-Filename: botup/core/constants/api_method.py
+Filename: botup/constants/api_method.py
 Comment: 
 
-Filename: botup/core/constants/base.py
+Filename: botup/constants/base.py
 Comment: 
 
-Filename: botup/core/constants/bot_command_scope_type.py
+Filename: botup/constants/bot_command_scope_type.py
 Comment: 
 
-Filename: botup/core/constants/chat_action.py
+Filename: botup/constants/chat_action.py
 Comment: 
 
-Filename: botup/core/constants/chat_member_status.py
+Filename: botup/constants/chat_member_status.py
 Comment: 
 
-Filename: botup/core/constants/chat_type.py
+Filename: botup/constants/chat_type.py
 Comment: 
 
-Filename: botup/core/constants/encrypted_passport_element_type.py
+Filename: botup/constants/encrypted_passport_element_type.py
 Comment: 
 
-Filename: botup/core/constants/inline_query_chat_type.py
+Filename: botup/constants/inline_query_chat_type.py
 Comment: 
 
-Filename: botup/core/constants/inline_query_result_type.py
+Filename: botup/constants/inline_query_result_type.py
 Comment: 
 
-Filename: botup/core/constants/input_file_type.py
+Filename: botup/constants/input_file_type.py
 Comment: 
 
-Filename: botup/core/constants/input_media_type.py
+Filename: botup/constants/input_media_type.py
 Comment: 
 
-Filename: botup/core/constants/mask_position_point.py
+Filename: botup/constants/mask_position_point.py
 Comment: 
 
-Filename: botup/core/constants/menu_button_type.py
+Filename: botup/constants/menu_button_type.py
 Comment: 
 
-Filename: botup/core/constants/message_entity_type.py
+Filename: botup/constants/message_entity_type.py
 Comment: 
 
-Filename: botup/core/constants/passport_element_error_source.py
+Filename: botup/constants/passport_element_error_source.py
 Comment: 
 
-Filename: botup/core/constants/poll_type.py
+Filename: botup/constants/poll_type.py
 Comment: 
 
-Filename: botup/core/constants/sticker_type.py
+Filename: botup/constants/sticker_type.py
 Comment: 
 
-Filename: botup/core/constants/update_type.py
+Filename: botup/constants/update_type.py
 Comment: 
 
 Filename: botup/mixins/__init__.py
 Comment: 
 
 Filename: botup/mixins/echo.py
 Comment: 
@@ -126,20 +120,20 @@
 
 Filename: tests/test_serializing.py
 Comment: 
 
 Filename: tests/utils.py
 Comment: 
 
-Filename: telegram_botup-1.0.2.dist-info/METADATA
+Filename: telegram_botup-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: telegram_botup-1.0.2.dist-info/WHEEL
+Filename: telegram_botup-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: telegram_botup-1.0.2.dist-info/top_level.txt
+Filename: telegram_botup-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: telegram_botup-1.0.2.dist-info/RECORD
+Filename: telegram_botup-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## botup/__init__.py

```diff
@@ -1,4 +1,5 @@
-__version__ = "1.0.2"
-
-from .core.api import Api
-from .core.dispatcher import Dispatcher
+from .api import Api
+from .dispatcher import Dispatcher
+from .bot import Bot
+from .widget import Widget, Context
+from .navigation import Navigation
```

## botup/bot.py

```diff
@@ -1,9 +1,9 @@
-from botup.core.api import Api
-from botup.core.types import Update
+from botup.api import Api
+from botup.types import Update
 from botup.navigation import Navigation
 from botup.state_manager.base import StateManager, DictStateManager
 from botup.widget import Widget, Context
 
 
 class Bot:
```

## botup/utils.py

```diff
@@ -1,16 +1,27 @@
-from botup.core.utils import get_logger, setup_logging
+import logging
+
 
 __all__ = [
     'get_logger',
     'setup_logging',
     'start_group_link',
     'start_link'
 ]
 
 
+def get_logger():
+    return logging.getLogger('botup')
+
+
+def setup_logging(level=logging.INFO):
+    logger = logging.getLogger('botup')
+    logger.addHandler(logging.StreamHandler())
+    logger.setLevel(level)
+
+
 def start_group_link(bot_name: str):
     return f'https://telegram.me/{bot_name}?startgroup='
 
 
 def start_link(bot_name: str):
     return f'https://telegram.me/{bot_name}?start='
```

## botup/widget.py

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import Dict, Optional, List
 
-from botup.core.api import Api
-from botup.core.dispatcher import Dispatcher
-from botup.core.types import Update, CoreContext
+from botup.api import Api
+from botup.dispatcher import Dispatcher
+from botup.types import Update, BaseContext
 from botup.state_manager.base import Singleton, StateManager
 
 
 class WidgetRegistry(metaclass=Singleton):
 
     def __init__(self):
         self._data: Dict[str, Widget] = {}
@@ -35,15 +35,15 @@
     def build(self, dispatcher: Dispatcher):
         pass
 
     async def handle(self, ctx: Context):
         await self._dispatcher.handle_context(ctx)
 
 
-class Context(CoreContext):
+class Context(BaseContext):
 
     def __init__(
             self,
             update: Update,
             api: Api,
             root_widget: Widget,
             state_manager: StateManager
```

## botup/mixins/echo.py

```diff
@@ -1,10 +1,10 @@
 import re
 
-from botup.core.dispatcher import Dispatcher
+from botup.dispatcher import Dispatcher
 from botup.widget import Context
 
 
 class EchoMixin:
 
     def build(self, dispatcher: Dispatcher):
         dispatcher.register_message_handler(re.compile(r'.*'), self.msg_echo)
```

## botup/state_manager/redis.py

```diff
@@ -1,19 +1,19 @@
 from typing import Optional
 
-import aioredis
+from redis.asyncio import Redis
 
 from botup.state_manager.base import Singleton, StateManager
 
 
 class RedisStateManager(StateManager, metaclass=Singleton):
 
     def __init__(self, url: str):
         super().__init__()
-        self.redis = aioredis.from_url(url, decode_responses=True)
+        self.redis = Redis.from_url(url, decode_responses=True)
 
     async def get_path(self, chat_id: int) -> Optional[str]:
         return await self.get(chat_id, 'path', 'botup')
 
     async def set_path(self, chat_id: int, path: str):
         await self.set(chat_id, 'path', path, 'botup')
```

## botup/widgets/date_picker.py

```diff
@@ -2,16 +2,16 @@
 import re
 from calendar import Calendar, month_name
 from datetime import datetime, timedelta
 from asyncio import gather
 
 from botup.navigation import Navigation
 from botup.widget import Widget, Context
-from botup.core.dispatcher import Dispatcher
-from botup.core.types import InlineKeyboardMarkup, InlineKeyboardButton
+from botup.dispatcher import Dispatcher
+from botup.types import InlineKeyboardMarkup, InlineKeyboardButton
 
 
 class DatePicker(Widget):
 
     def __init__(
             self,
             key: str,
```

## Comparing `botup/core/api.py` & `botup/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     get_type_hints,
     get_origin,
     get_args
 )
 
 from aiohttp import ClientSession
 
-from botup.core.constants import api_method
-from botup.core.constants.chat_action import ChatAction
-from botup.core.constants.sticker_type import StickerType
-from botup.core.types import (
+from botup.constants import api_method
+from botup.constants.chat_action import ChatAction
+from botup.constants.sticker_type import StickerType
+from botup.types import (
     Update,
     InputFile,
     WebhookInfo,
     User,
     Message,
     MessageEntity,
     InlineKeyboardMarkup,
@@ -53,15 +53,15 @@
     GameHighScore,
     InputFilePath,
     InputFileStored,
     InputFileUrl,
     BaseObject,
     Keyboard
 )
-from botup.core.utils import get_logger
+from botup.utils import get_logger
 
 logger = get_logger()
 
 
 class Api:
     def __init__(self, token: str, timeout: int = 5):
         self.token = token
```

## Comparing `botup/core/dispatcher.py` & `botup/dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Callable, Set, Pattern, Union
 
-from botup.core.constants.update_type import (
+from botup.constants.update_type import (
     UpdateType,
     CALLBACK_QUERY,
     INLINE_QUERY,
     CHANNEL_POST,
     EDITED_MESSAGE,
     EDITED_CHANNEL_POST,
     CHOSEN_INLINE_RESULT,
@@ -30,15 +30,15 @@
     MESSAGE_STICKER,
     MESSAGE_SUCCESSFUL_PAYMENT,
     MESSAGE_VENUE,
     MESSAGE_VIDEO,
     MESSAGE_VIDEO_NOTE,
     MESSAGE_VOICE
 )
-from botup.core.handlers import (
+from botup.handlers import (
     MessageCommandHandler,
     CallbackQueryHandler,
     MessageTextHandler,
     InlineQueryHandler,
     EditedMessageHandler,
     ChannelPostHandler,
     ChosenInlineResultHandler,
@@ -63,15 +63,15 @@
     MessageStickerHandler,
     MessageSuccessfulPaymentHandler,
     MessageVenueHandler,
     MessageVideoHandler,
     MessageVideoNoteHandler,
     MessageVoiceHandler
 )
-from botup.core.types import Update, HandleFunction, MiddlewareFunction, CoreContext
+from botup.types import Update, HandleFunction, MiddlewareFunction, BaseContext
 
 
 class Dispatcher:
 
     def __init__(self):
         self._middlewares: Set[MiddlewareFunction] = set()
         self._update_types: Set[UpdateType] = set()
@@ -372,32 +372,32 @@
         self._update_types.add(MESSAGE_VIDEO_NOTE)
         self._message_video_note_handler.register(handler)
 
     def register_voice_handler(self, handler: HandleFunction):
         self._update_types.add(MESSAGE_VOICE)
         self._message_voice_handler.register(handler)
 
-    async def _run_statements(self, context: CoreContext):
+    async def _run_statements(self, context: BaseContext):
         for update_type in self._update_types:
             statement_key = f'is_{update_type}'
             handler_key = f'_{update_type}_handler'
 
             if getattr(context, statement_key):
                 handler = getattr(self, handler_key)
                 context.update_type = update_type
                 await handler.handle(context)
 
-    async def _run_middlewares(self, context: CoreContext) -> bool:
+    async def _run_middlewares(self, context: BaseContext) -> bool:
         for middleware in self._middlewares:
             if await middleware(context):
                 return True
 
         return False
 
     async def handle(self, update: dict):
-        await self.handle_context(CoreContext(Update.from_dict(update)))
+        await self.handle_context(BaseContext(Update.from_dict(update)))
 
-    async def handle_context(self, context: CoreContext):
+    async def handle_context(self, context: BaseContext):
         if await self._run_middlewares(context):
             return
 
         await self._run_statements(context)
```

## Comparing `botup/core/handlers.py` & `botup/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, Optional, Union, Pattern
 
-from botup.core.types import Update, HandleFunction, CoreContext
+from botup.types import Update, HandleFunction, BaseContext
 
 
 class Handler:
 
     @staticmethod
     def get_user_id(update: Update) -> Optional[int]:
         return None
@@ -26,15 +26,15 @@
         if key in self._handlers:
             return self._handlers[key]
 
         for pattern in self._handlers.keys():
             if isinstance(pattern, Pattern) and pattern.match(key):
                 return self._handlers[pattern]
 
-    async def handle(self, context: CoreContext):
+    async def handle(self, context: BaseContext):
         handler = self.get_handler(self.get_key(context.update))
 
         if not handler:
             return
 
         context.chat_id = self.get_chat_id(context.update)
         context.user_id = self.get_user_id(context.update)
@@ -50,15 +50,15 @@
 
     def __init__(self):
         self._handler: Optional[HandleFunction] = None
 
     def register(self, function: HandleFunction):
         self._handler = function
 
-    async def handle(self, context: CoreContext):
+    async def handle(self, context: BaseContext):
         if not self._handler:
             return
 
         context.chat_id = self.get_chat_id(context.update)
         context.user_id = self.get_user_id(context.update)
 
         await self._handler(context)
```

## Comparing `botup/core/types.py` & `botup/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,38 +11,38 @@
     Callable,
     Awaitable,
     get_type_hints,
     get_origin,
     get_args
 )
 
-from botup.core.constants import (
+from botup.constants import (
     chat_member_status,
     bot_command_scope_type,
     menu_button_type,
     input_media_type,
     input_file_type,
     inline_query_result_type,
     passport_element_error_source
 )
-from botup.core.constants.bot_command_scope_type import BotCommandScopeType
-from botup.core.constants.chat_member_status import ChatMemberStatus
-from botup.core.constants.chat_type import ChatType
-from botup.core.constants.encrypted_passport_element_type import EncryptedPassportElementType
-from botup.core.constants.inline_query_chat_type import InlineQueryChatType
-from botup.core.constants.inline_query_result_type import InlineQueryResultType
-from botup.core.constants.input_file_type import InputFileType
-from botup.core.constants.input_media_type import InputMediaType
-from botup.core.constants.mask_position_point import MaskPositionPoint
-from botup.core.constants.menu_button_type import MenuButtonType
-from botup.core.constants.message_entity_type import MessageEntityType
-from botup.core.constants.passport_element_error_source import PassportElementErrorSource
-from botup.core.constants.poll_type import PollType
-from botup.core.constants.sticker_type import StickerType
-from botup.core.constants.update_type import UpdateType
+from botup.constants.bot_command_scope_type import BotCommandScopeType
+from botup.constants.chat_member_status import ChatMemberStatus
+from botup.constants.chat_type import ChatType
+from botup.constants.encrypted_passport_element_type import EncryptedPassportElementType
+from botup.constants.inline_query_chat_type import InlineQueryChatType
+from botup.constants.inline_query_result_type import InlineQueryResultType
+from botup.constants.input_file_type import InputFileType
+from botup.constants.input_media_type import InputMediaType
+from botup.constants.mask_position_point import MaskPositionPoint
+from botup.constants.menu_button_type import MenuButtonType
+from botup.constants.message_entity_type import MessageEntityType
+from botup.constants.passport_element_error_source import PassportElementErrorSource
+from botup.constants.poll_type import PollType
+from botup.constants.sticker_type import StickerType
+from botup.constants.update_type import UpdateType
 
 NoneType = type(None)
 _rename_key_mapping = {
     'from_': 'from'
 }
 
 
@@ -1575,15 +1575,15 @@
 class GameHighScore(BaseObject):
     position: int
     user: User
     score: int
 
 
 @dataclass
-class CoreContext:
+class BaseContext:
     update: Update
     update_type: Optional[UpdateType] = None
     chat_id: Optional[int] = None
     user_id: Optional[int] = None
 
     @property
     def is_message(self) -> bool:
@@ -1726,9 +1726,9 @@
         return self.is_message and self.update.message.voice is not None
 
     @property
     def is_message_poll(self) -> bool:
         return self.is_message and self.update.message.poll is not None
 
 
-HandleFunction = Callable[[CoreContext], Awaitable[None]]
-MiddlewareFunction = Callable[[CoreContext], Awaitable[bool]]
+HandleFunction = Callable[[BaseContext], Awaitable[None]]
+MiddlewareFunction = Callable[[BaseContext], Awaitable[bool]]
```

## Comparing `botup/core/constants/api_method.py` & `botup/constants/api_method.py`

 * *Files identical despite different names*

## Comparing `botup/core/constants/chat_action.py` & `botup/constants/chat_action.py`

 * *Files identical despite different names*

## Comparing `botup/core/constants/encrypted_passport_element_type.py` & `botup/constants/encrypted_passport_element_type.py`

 * *Files identical despite different names*

## Comparing `botup/core/constants/inline_query_result_type.py` & `botup/constants/inline_query_result_type.py`

 * *Files identical despite different names*

## Comparing `botup/core/constants/message_entity_type.py` & `botup/constants/message_entity_type.py`

 * *Files identical despite different names*

## Comparing `botup/core/constants/passport_element_error_source.py` & `botup/constants/passport_element_error_source.py`

 * *Files identical despite different names*

## Comparing `botup/core/constants/update_type.py` & `botup/constants/update_type.py`

 * *Files identical despite different names*

## Comparing `telegram_botup-1.0.2.dist-info/METADATA` & `telegram_botup-1.0.4.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,99 +1,99 @@
 Metadata-Version: 2.1
 Name: telegram-botup
-Version: 1.0.2
-Summary: Telegram bot API
+Version: 1.0.4
+Summary: Python library for building Telegram bots
 Home-page: UNKNOWN
-Author: Dima Shebotinov
+Author: Dmitry Shebotinov
 Author-email: groovestreetmagic@gmail.com
 License: UNKNOWN
 Project-URL: Source Code, https://github.com/spirtum/telegram-botup
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Python Software Foundation License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Provides-Extra: redis
-Requires-Dist: aioredis ; extra == 'redis'
+Requires-Dist: redis ; extra == 'redis'
 
 # Telegram-botup
 
+Python library for building Telegram bots
+
 
 ## Install
 ```
 $ pip install telegram-botup
 ```
 
 ## Example
 ```python
 # app.py
 
 from web_lib import App, Request
-from botup.core.dispatcher import Dispatcher
-from botup.core.api import Api
-from botup.core.types import CoreContext
+
+from botup.dispatcher import Dispatcher
+from botup.api import Api
+from botup.types import BaseContext
 
 TOKEN = "token"
 
 app = App()
-dispatcher = Dispatcher()
 api = Api(TOKEN)
+dispatcher = Dispatcher()
 
 
 @dispatcher.message_handler('hello')
-async def hello_handler(ctx: CoreContext):
+async def hello_handler(ctx: BaseContext):
     await api.send_message(ctx.chat_id, f'Hello {ctx.update.message.from_.first_name}')
 
 
 @app.post(f'/{TOKEN}')
 async def index(request: Request):
     await dispatcher.handle(await request.json())
-    return "!"
+    return ""
 ```
 
 
 ## Widgets example
 ```python
 # app.py
 
 from asyncio import gather
 
 from web_lib import App, Request
 
-from botup.widget import Widget, Context
-from botup.core.dispatcher import Dispatcher
-from botup.core.api import Api
-from botup.bot import Bot
-from botup.navigation import Navigation
+from botup import Widget, Context, Dispatcher, Api, Bot, Navigation
 from botup.widgets.date_picker import DatePicker
 from botup.mixins.echo import EchoMixin
-from botup.core.types import InlineKeyboardMarkup, InlineKeyboardButton
+from botup.types import InlineKeyboardMarkup, InlineKeyboardButton
 
-TOKEN = ""
-WEBHOOK = f'https:///{TOKEN}'
+TOKEN = "token"
+WEBHOOK = f'https://url/{TOKEN}'
 
-app = App(docs_url=None, redoc_url=None)
+app = App()
 
 
-class MyCustomMixin:
+class TestMixin:
 
     def build(self, dispatcher: Dispatcher):
+        print('TestMixin build')
         dispatcher.register_command_handler('/test', self.cmd_test)
 
     @staticmethod
     async def cmd_test(ctx: Context):
         await ctx.api.send_message(
             chat_id=ctx.chat_id,
             text='Test'
         )
 
 
-class RootWidget(Widget, MyCustomMixin, EchoMixin):
+class RootWidget(Widget, TestMixin, EchoMixin):
     """
-    Type "/start"
+    Type "go" message
     """
 
     KEY = 'root'
     DATE_PICKER_KEY = 'date_picker'
     DATE_PICKER_RESULT_KEY = 'dp_result'
 
     async def entry(self, ctx: Context, **kwargs):
@@ -102,15 +102,15 @@
             await ctx.api.send_message(
                 chat_id=ctx.chat_id,
                 text=f'date: {botup_date_picker_result}'
             )
             return
 
     def build(self, dispatcher: Dispatcher):
-        MyCustomMixin.build(self, dispatcher)
+        TestMixin.build(self, dispatcher)
         dispatcher.register_message_handler('go', self.go_handler)
         dispatcher.register_command_handler('/start', self.cmd_start)
         dispatcher.register_callback_handler('ready', self.clb_ready)
         EchoMixin.build(self, dispatcher)
 
     @staticmethod
     async def cmd_start(ctx: Context):
@@ -120,14 +120,15 @@
             reply_markup=InlineKeyboardMarkup([[InlineKeyboardButton(callback_data='ready', text='Yeah!')]])
         )
         await ctx.state_manager.set(
             chat_id=ctx.chat_id,
             key='message_id',
             value=str(message.message_id)
         )
+        return None
 
     @staticmethod
     async def clb_ready(ctx: Context):
         _, message_id, nav = await gather(
             ctx.api.answer_callback_query(ctx.update.callback_query.id),
             ctx.state_manager.get(
                 chat_id=ctx.chat_id,
@@ -173,11 +174,10 @@
 
     await bot.close_session()
 
 
 @app.post(f'/{TOKEN}')
 async def index(request: Request):
     await bot.handle(await request.json())
-    return {'ok': True}
-
+    return ""
 ```
```

## Comparing `telegram_botup-1.0.2.dist-info/RECORD` & `telegram_botup-1.0.4.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,46 @@
-botup/__init__.py,sha256=ojHiS9pPT0phBisKcicxG_P_vNcHOa_K-fYEQBOQcDU,89
-botup/bot.py,sha256=WydZRSYhH9i7Xo3XRrR-6YwaKBe6OWS_tAR9MFaW37o,905
+botup/__init__.py,sha256=SqkgBNCPv-Ds2BREZ1kpe_eOe9fwjKFvfuKOsw7Pilg,148
+botup/api.py,sha256=kOWQdpDi7ivm78xd_ewbxqswxB98Tj90pPx3kIBcn3o,52863
+botup/bot.py,sha256=V5NK2Zikej5_KYwOAfZqM1oM7fP6uIWUGgdtkLGj550,895
+botup/dispatcher.py,sha256=i_MH623jMWYlzekXjNUSQ6AJ6TJammlzx_oxdR83e0c,15290
+botup/handlers.py,sha256=esLE1MlSEsYGpLWROwho_-dH5OJKVZXqFV05WuZCmkg,9769
 botup/navigation.py,sha256=pEE4Jo0olM9ZvHsvag2HNrSyLjSW9mvtw0VFBLNkACE,1266
-botup/utils.py,sha256=79UXKDZmEjjKjrleFBEKyiT6wWDwbOFGDpeHn2-ehqw,331
-botup/widget.py,sha256=pGKgwWMvbdVnWS0pR7NjG7GCiAXxlyDFtkQC3c4yT4s,1948
-botup/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-botup/core/api.py,sha256=vINvuE3ltBjASao-W9x_rTbXzQP7OP_AITnGugv9b0U,52888
-botup/core/dispatcher.py,sha256=NsQHaJ4U-RrS8KTO9J7QlftJTXv5kfXuAYyhgWodQic,15305
-botup/core/handlers.py,sha256=-QwnYrj6g4TEJVKHLD12xqGOCZ-lFSXh8BqKaEwIHjQ,9774
-botup/core/types.py,sha256=CkT9gjzRY2V-A98nFFQHDvi6BbwpK0QRTw14HP21nt4,47430
-botup/core/utils.py,sha256=8SqkCH-PR0PtYRH0uXUCe5teNIVR7kysGiKcqkf1ewQ,228
-botup/core/constants/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-botup/core/constants/api_method.py,sha256=QPXt4RZLfhZWvV-3tAzQ9xYvHiEg0hKLcvrvbwTVryc,5243
-botup/core/constants/base.py,sha256=HueKF2ErW9pr3FeoDA61T7uTGvytUgRtEX8ycsNezg0,115
-botup/core/constants/bot_command_scope_type.py,sha256=bTyvL9n0DGas6mVsd1N0xpQhkOVhpwGY496aa4csUA4,470
-botup/core/constants/chat_action.py,sha256=sK2cLy0MurlJoqakVLHwjnsljw4Jo0kTERnPvX4-zNs,562
-botup/core/constants/chat_member_status.py,sha256=ArHrDTx0LYYCB1bPkfpqqr5Jqm8h3Di3wF6-yLzeRtY,322
-botup/core/constants/chat_type.py,sha256=W_eIJoHA5MB0r-XAI2dbgPqkE-W5C3QYrQu8bM_TlZo,200
-botup/core/constants/encrypted_passport_element_type.py,sha256=L0wSZzhNn8ORI8Qva798fnTzdYY3HnKtGMiyqL_pxYQ,920
-botup/core/constants/inline_query_chat_type.py,sha256=GVWlRWVEuuSH42zqR0ItDgjv3KZI2lWrwPBixFY8To4,294
-botup/core/constants/inline_query_result_type.py,sha256=QI5QhwMvdRKpQjnic1-ZOQ1Bm57VeWal9SwU6F_DS1g,624
-botup/core/constants/input_file_type.py,sha256=x2scBhaIULv5jAD3Yp_qHjdWhcFbBnsXILE_LOl3aSE,172
-botup/core/constants/input_media_type.py,sha256=VIy-RqAhnpTKVJx0wmrXRx8EJWOE1uDtzMsT6yAAQw4,258
-botup/core/constants/mask_position_point.py,sha256=VW0vJZXZWJW2bMnH8d0uLbQL82nve1BGuJVIbOIWc4w,229
-botup/core/constants/menu_button_type.py,sha256=ajRG3RkhoBDpPamvPjcqLEc9Kn0Xk1toChjIKIywEKM,194
-botup/core/constants/message_entity_type.py,sha256=NmmZvzj9CYd3PHKjY2DUMc5B2t4xXVIl3Pmw0qo_wrE,774
-botup/core/constants/passport_element_error_source.py,sha256=RAfP85NLnYJoqBbQVqVLTFJxIdJ6ZMsGKxpVYjMwoMY,572
-botup/core/constants/poll_type.py,sha256=M1ucrqpWI2pU40hfJFSoyN7jHWWtNEUNHahqIKS9d5Q,132
-botup/core/constants/sticker_type.py,sha256=U7ZB0dTBkNa3Ehipt9WaJPOgDNBmTqB182l3QvHt_xY,184
-botup/core/constants/update_type.py,sha256=2rrlazsxhmGjcfSLRZ2ygHn1wfFJormlcTEDBSndWBc,1622
+botup/types.py,sha256=IaFW392DwQnepHG38tOE0sUQmfV2_8hqe1xg4qux64I,47350
+botup/utils.py,sha256=1TByBVg8jNmadrc0WfxavnhQOhZl3D3LslQg2riBauE,505
+botup/widget.py,sha256=-FxEaY_PrGpSi-dqM_3AivclSE2JTRUtfiM6J46_ZbI,1933
+botup/constants/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+botup/constants/api_method.py,sha256=QPXt4RZLfhZWvV-3tAzQ9xYvHiEg0hKLcvrvbwTVryc,5243
+botup/constants/base.py,sha256=HueKF2ErW9pr3FeoDA61T7uTGvytUgRtEX8ycsNezg0,115
+botup/constants/bot_command_scope_type.py,sha256=bTyvL9n0DGas6mVsd1N0xpQhkOVhpwGY496aa4csUA4,470
+botup/constants/chat_action.py,sha256=sK2cLy0MurlJoqakVLHwjnsljw4Jo0kTERnPvX4-zNs,562
+botup/constants/chat_member_status.py,sha256=ArHrDTx0LYYCB1bPkfpqqr5Jqm8h3Di3wF6-yLzeRtY,322
+botup/constants/chat_type.py,sha256=W_eIJoHA5MB0r-XAI2dbgPqkE-W5C3QYrQu8bM_TlZo,200
+botup/constants/encrypted_passport_element_type.py,sha256=L0wSZzhNn8ORI8Qva798fnTzdYY3HnKtGMiyqL_pxYQ,920
+botup/constants/inline_query_chat_type.py,sha256=GVWlRWVEuuSH42zqR0ItDgjv3KZI2lWrwPBixFY8To4,294
+botup/constants/inline_query_result_type.py,sha256=QI5QhwMvdRKpQjnic1-ZOQ1Bm57VeWal9SwU6F_DS1g,624
+botup/constants/input_file_type.py,sha256=x2scBhaIULv5jAD3Yp_qHjdWhcFbBnsXILE_LOl3aSE,172
+botup/constants/input_media_type.py,sha256=VIy-RqAhnpTKVJx0wmrXRx8EJWOE1uDtzMsT6yAAQw4,258
+botup/constants/mask_position_point.py,sha256=VW0vJZXZWJW2bMnH8d0uLbQL82nve1BGuJVIbOIWc4w,229
+botup/constants/menu_button_type.py,sha256=ajRG3RkhoBDpPamvPjcqLEc9Kn0Xk1toChjIKIywEKM,194
+botup/constants/message_entity_type.py,sha256=NmmZvzj9CYd3PHKjY2DUMc5B2t4xXVIl3Pmw0qo_wrE,774
+botup/constants/passport_element_error_source.py,sha256=RAfP85NLnYJoqBbQVqVLTFJxIdJ6ZMsGKxpVYjMwoMY,572
+botup/constants/poll_type.py,sha256=M1ucrqpWI2pU40hfJFSoyN7jHWWtNEUNHahqIKS9d5Q,132
+botup/constants/sticker_type.py,sha256=U7ZB0dTBkNa3Ehipt9WaJPOgDNBmTqB182l3QvHt_xY,184
+botup/constants/update_type.py,sha256=2rrlazsxhmGjcfSLRZ2ygHn1wfFJormlcTEDBSndWBc,1622
 botup/mixins/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-botup/mixins/echo.py,sha256=ovRseWwXzJgjMcgHsdB45KNtk7MKSbWiXzPU4ma__Bc,409
+botup/mixins/echo.py,sha256=GnzvDuZexW73MG-ENwR0Pd0V1lT1i9Vzd1rSJlcf7ZM,404
 botup/state_manager/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 botup/state_manager/base.py,sha256=b1Cyze7vcQEXeg8TLenPN0cNnv7W-GO4yxe5usAQGOM,2045
-botup/state_manager/redis.py,sha256=UrVYx71obRbZfXIbh0MLbVssMRlVnvbrDyfPujc-6Yk,990
+botup/state_manager/redis.py,sha256=s95y41ZmBmY6e0g8VG3tpngt5CYtkbx-L9C5PI63exo,1003
 botup/widgets/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-botup/widgets/date_picker.py,sha256=bBCDNmGii9xPJC54NyED8KnmivPDwUO1tBkrbj1S9-E,8930
+botup/widgets/date_picker.py,sha256=64DdooqE5z0khhuzjHDhO2GjTkSi7-RfoYWqUpQIL9k,8920
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/conftest.py,sha256=kvSuN6G_9iR8TyLWIHr437h6H91DOaX80d926VHJ-9Y,119
 tests/test_dispatcher.py,sha256=g8sHIub-5t46fqGNnrgkvlD-_mZdQboPxvByIaeNQwY,32361
 tests/test_dispatcher_decorator.py,sha256=Dm8M56aE5FI48Xxcm-1DmhlrEKPUr5nwiamHB0YLe7Q,10599
 tests/test_dispatcher_registration.py,sha256=iHYq-NEig8aHbjCh5u-vQuxC0AK-f_71BTLozQOY3YA,6708
 tests/test_serializing.py,sha256=otX8e4hKzrrbq8V5JSyKh5DewhrSRTwit9Q4rhb4XoY,441
 tests/utils.py,sha256=ZJesYuEPqLPP2PWVIJyD8vatfQLybVreJsg3Qd0R9-k,35379
-telegram_botup-1.0.2.dist-info/METADATA,sha256=U4-aBiAsEZkF9mpJjq1liPb6Ol_nd1mJ51fYeMwOet0,4496
-telegram_botup-1.0.2.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-telegram_botup-1.0.2.dist-info/top_level.txt,sha256=5xSddxEvjN25GjUZSsBTJZ1OyYrsPAApb5FXZUYYoLU,12
-telegram_botup-1.0.2.dist-info/RECORD,,
+telegram_botup-1.0.4.dist-info/METADATA,sha256=Oc-1dmqVhKjqoLVc6Eh_sTzeV52ms2wm3S_5t5jazvs,4441
+telegram_botup-1.0.4.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+telegram_botup-1.0.4.dist-info/top_level.txt,sha256=5xSddxEvjN25GjUZSsBTJZ1OyYrsPAApb5FXZUYYoLU,12
+telegram_botup-1.0.4.dist-info/RECORD,,
```

