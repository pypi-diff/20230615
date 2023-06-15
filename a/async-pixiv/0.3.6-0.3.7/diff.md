# Comparing `tmp/async_pixiv-0.3.6.tar.gz` & `tmp/async_pixiv-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_pixiv-0.3.6.tar", max compression
+gzip compressed data, was "async_pixiv-0.3.7.tar", max compression
```

## Comparing `async_pixiv-0.3.6.tar` & `async_pixiv-0.3.7.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0     1069 2023-03-16 16:45:33.431856 async_pixiv-0.3.6/LICENSE
--rw-r--r--   0        0        0       46 2023-03-16 16:45:33.431856 async_pixiv-0.3.6/README.md
--rw-r--r--   0        0        0     1745 2023-03-16 16:45:33.431856 async_pixiv-0.3.6/pyproject.toml
--rw-r--r--   0        0        0       43 2023-03-16 16:45:33.431856 async_pixiv-0.3.6/src/async_pixiv/__init__.py
--rw-r--r--   0        0        0      117 2023-03-16 16:45:33.431856 async_pixiv-0.3.6/src/async_pixiv/client/__init__.py
--rw-r--r--   0        0        0    13973 2023-03-16 16:45:33.431856 async_pixiv-0.3.6/src/async_pixiv/client/_client.py
--rw-r--r--   0        0        0      217 2023-03-16 16:45:33.431856 async_pixiv-0.3.6/src/async_pixiv/client/_section/__init__.py
--rw-r--r--   0        0        0     2673 2023-03-16 16:45:33.431856 async_pixiv-0.3.6/src/async_pixiv/client/_section/_base.py
--rw-r--r--   0        0        0     9789 2023-03-16 16:45:33.431856 async_pixiv-0.3.6/src/async_pixiv/client/_section/_illust.py
--rw-r--r--   0        0        0     3759 2023-03-16 16:45:33.431856 async_pixiv-0.3.6/src/async_pixiv/client/_section/_novel.py
--rw-r--r--   0        0        0     5066 2023-03-16 16:45:33.431856 async_pixiv-0.3.6/src/async_pixiv/client/_section/_user.py
--rw-r--r--   0        0        0      176 2023-03-16 16:45:33.431856 async_pixiv-0.3.6/src/async_pixiv/client/config
--rw-r--r--   0        0        0     1460 2023-03-16 16:45:33.431856 async_pixiv-0.3.6/src/async_pixiv/error.py
--rw-r--r--   0        0        0        0 2023-03-16 16:45:33.431856 async_pixiv-0.3.6/src/async_pixiv/model/__init__.py
--rw-r--r--   0        0        0     1715 2023-03-16 16:45:33.431856 async_pixiv-0.3.6/src/async_pixiv/model/_base.py
--rw-r--r--   0        0        0    11432 2023-03-16 16:45:33.431856 async_pixiv-0.3.6/src/async_pixiv/model/illust.py
--rw-r--r--   0        0        0     4752 2023-03-16 16:45:33.431856 async_pixiv-0.3.6/src/async_pixiv/model/novel.py
--rw-r--r--   0        0        0     1878 2023-03-16 16:45:33.431856 async_pixiv-0.3.6/src/async_pixiv/model/other.py
--rw-r--r--   0        0        0     4445 2023-03-16 16:45:33.431856 async_pixiv-0.3.6/src/async_pixiv/model/result.py
--rw-r--r--   0        0        0     4842 2023-03-16 16:45:33.431856 async_pixiv-0.3.6/src/async_pixiv/model/user.py
--rw-r--r--   0        0        0        0 2023-03-16 16:45:33.431856 async_pixiv-0.3.6/src/async_pixiv/utils/__init__.py
--rw-r--r--   0        0        0     1163 2023-03-16 16:45:33.431856 async_pixiv-0.3.6/src/async_pixiv/utils/context.py
--rw-r--r--   0        0        0      819 2023-03-16 16:45:33.431856 async_pixiv-0.3.6/src/async_pixiv/utils/enums.py
--rw-r--r--   0        0        0       65 2023-03-16 16:45:33.431856 async_pixiv-0.3.6/src/async_pixiv/utils/ffmpeg/__init__.py
--rw-r--r--   0        0        0     4884 2023-03-16 16:45:33.435856 async_pixiv-0.3.6/src/async_pixiv/utils/ffmpeg/_ffmpeg.py
--rw-r--r--   0        0        0      180 2023-03-16 16:45:33.435856 async_pixiv-0.3.6/src/async_pixiv/utils/ffmpeg/typing.py
--rw-r--r--   0        0        0     2193 2023-03-16 16:45:33.435856 async_pixiv-0.3.6/src/async_pixiv/utils/ffmpeg/utils.py
--rw-r--r--   0        0        0      421 2023-03-16 16:45:33.435856 async_pixiv-0.3.6/src/async_pixiv/utils/func.py
--rw-r--r--   0        0        0     7705 2023-03-16 16:45:33.435856 async_pixiv-0.3.6/src/async_pixiv/utils/net.py
--rw-r--r--   0        0        0     4035 2023-03-16 16:45:33.435856 async_pixiv-0.3.6/src/async_pixiv/utils/overwrite.py
--rw-r--r--   0        0        0      237 2023-03-16 16:45:33.435856 async_pixiv-0.3.6/src/async_pixiv/utils/typedefs.py
--rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 async_pixiv-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-15 16:17:31.890124 async_pixiv-0.3.7/LICENSE
+-rw-r--r--   0        0        0    10093 2023-06-15 16:17:31.890124 async_pixiv-0.3.7/README.md
+-rw-r--r--   0        0        0     1745 2023-06-15 16:17:31.890124 async_pixiv-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-06-15 16:17:31.890124 async_pixiv-0.3.7/src/async_pixiv/__init__.py
+-rw-r--r--   0        0        0      117 2023-06-15 16:17:31.890124 async_pixiv-0.3.7/src/async_pixiv/client/__init__.py
+-rw-r--r--   0        0        0    14070 2023-06-15 16:17:31.890124 async_pixiv-0.3.7/src/async_pixiv/client/_client.py
+-rw-r--r--   0        0        0      217 2023-06-15 16:17:31.890124 async_pixiv-0.3.7/src/async_pixiv/client/_section/__init__.py
+-rw-r--r--   0        0        0     2673 2023-06-15 16:17:31.890124 async_pixiv-0.3.7/src/async_pixiv/client/_section/_base.py
+-rw-r--r--   0        0        0     8979 2023-06-15 16:17:31.890124 async_pixiv-0.3.7/src/async_pixiv/client/_section/_illust.py
+-rw-r--r--   0        0        0     3759 2023-06-15 16:17:31.890124 async_pixiv-0.3.7/src/async_pixiv/client/_section/_novel.py
+-rw-r--r--   0        0        0     5066 2023-06-15 16:17:31.890124 async_pixiv-0.3.7/src/async_pixiv/client/_section/_user.py
+-rw-r--r--   0        0        0      176 2023-06-15 16:17:31.890124 async_pixiv-0.3.7/src/async_pixiv/client/config
+-rw-r--r--   0        0        0     1460 2023-06-15 16:17:31.890124 async_pixiv-0.3.7/src/async_pixiv/error.py
+-rw-r--r--   0        0        0        0 2023-06-15 16:17:31.890124 async_pixiv-0.3.7/src/async_pixiv/model/__init__.py
+-rw-r--r--   0        0        0     1715 2023-06-15 16:17:31.894124 async_pixiv-0.3.7/src/async_pixiv/model/_base.py
+-rw-r--r--   0        0        0    11548 2023-06-15 16:17:31.894124 async_pixiv-0.3.7/src/async_pixiv/model/illust.py
+-rw-r--r--   0        0        0     4752 2023-06-15 16:17:31.894124 async_pixiv-0.3.7/src/async_pixiv/model/novel.py
+-rw-r--r--   0        0        0     1934 2023-06-15 16:17:31.894124 async_pixiv-0.3.7/src/async_pixiv/model/other.py
+-rw-r--r--   0        0        0     4445 2023-06-15 16:17:31.894124 async_pixiv-0.3.7/src/async_pixiv/model/result.py
+-rw-r--r--   0        0        0     4842 2023-06-15 16:17:31.894124 async_pixiv-0.3.7/src/async_pixiv/model/user.py
+-rw-r--r--   0        0        0        0 2023-06-15 16:17:31.894124 async_pixiv-0.3.7/src/async_pixiv/utils/__init__.py
+-rw-r--r--   0        0        0     4853 2023-06-15 16:17:31.894124 async_pixiv-0.3.7/src/async_pixiv/utils/bypass.py
+-rw-r--r--   0        0        0       76 2023-06-15 16:17:31.894124 async_pixiv-0.3.7/src/async_pixiv/utils/const.py
+-rw-r--r--   0        0        0     1163 2023-06-15 16:17:31.894124 async_pixiv-0.3.7/src/async_pixiv/utils/context.py
+-rw-r--r--   0        0        0      819 2023-06-15 16:17:31.894124 async_pixiv-0.3.7/src/async_pixiv/utils/enums.py
+-rw-r--r--   0        0        0       65 2023-06-15 16:17:31.894124 async_pixiv-0.3.7/src/async_pixiv/utils/ffmpeg/__init__.py
+-rw-r--r--   0        0        0     4888 2023-06-15 16:17:31.894124 async_pixiv-0.3.7/src/async_pixiv/utils/ffmpeg/_ffmpeg.py
+-rw-r--r--   0        0        0      180 2023-06-15 16:17:31.894124 async_pixiv-0.3.7/src/async_pixiv/utils/ffmpeg/typing.py
+-rw-r--r--   0        0        0     2193 2023-06-15 16:17:31.894124 async_pixiv-0.3.7/src/async_pixiv/utils/ffmpeg/utils.py
+-rw-r--r--   0        0        0      421 2023-06-15 16:17:31.894124 async_pixiv-0.3.7/src/async_pixiv/utils/func.py
+-rw-r--r--   0        0        0     8327 2023-06-15 16:17:31.894124 async_pixiv-0.3.7/src/async_pixiv/utils/net.py
+-rw-r--r--   0        0        0     4035 2023-06-15 16:17:31.894124 async_pixiv-0.3.7/src/async_pixiv/utils/overwrite.py
+-rw-r--r--   0        0        0      339 2023-06-15 16:17:31.894124 async_pixiv-0.3.7/src/async_pixiv/utils/typedefs.py
+-rw-r--r--   0        0        0    11828 1970-01-01 00:00:00.000000 async_pixiv-0.3.7/PKG-INFO
```

### Comparing `async_pixiv-0.3.6/LICENSE` & `async_pixiv-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `async_pixiv-0.3.6/pyproject.toml` & `async_pixiv-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-pixiv"
-version = "0.3.6"
+version = "0.3.7"
 description = "Async Pixiv API"
 license = "MIT"
 authors = ["Arko <arko.space.cc@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/ArkoClub/async-pixiv"
 repository = "https://github.com/ArkoClub/async-pixiv"
 keywords = ["pixiv", "async", "pixiv-api"]
```

### Comparing `async_pixiv-0.3.6/src/async_pixiv/client/_client.py` & `async_pixiv-0.3.7/src/async_pixiv/client/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,18 @@
     @classmethod
     def get_client(cls) -> "PixivClient":
         if cls._instances:
             return cls._instances[0]
         else:
             raise ValueError("请先实列化一个 PixivClient ")
 
+    @classmethod
+    def get_clients(cls) -> List["PixivClient"]:
+        return cls._instances
+
     _lock: ThreadLock = ThreadLock()
 
     class Config(NamedTuple):
         client_id: str
         client_secret: str
         user_agent: str
         accept_language: str
```

### Comparing `async_pixiv-0.3.6/src/async_pixiv/client/_section/_base.py` & `async_pixiv-0.3.7/src/async_pixiv/client/_section/_base.py`

 * *Files identical despite different names*

### Comparing `async_pixiv-0.3.6/src/async_pixiv/client/_section/_illust.py` & `async_pixiv-0.3.7/src/async_pixiv/client/_section/_illust.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,11 @@
 from datetime import date
 from io import BytesIO
 from pathlib import Path
-from typing import (
-    Dict,
-    Iterator,
-    List,
-    Optional,
-    Union,
-)
-from zipfile import ZipFile
+from typing import List, Optional, Union
 
 from typing_extensions import Literal
 
 from async_pixiv.client._section._base import (
     IllustType,
     SearchDuration,
     SearchFilter,
@@ -30,14 +23,15 @@
     IllustNewResult,
     IllustRelatedResult,
     IllustSearchResult,
     RecommendedResult,
     UgoiraMetadataResult,
 )
 from async_pixiv.utils.context import set_pixiv_client
+from async_pixiv.utils.typedefs import UGOIRA_RESULT_TYPE
 
 __all__ = ("ILLUST",)
 
 
 # noinspection PyShadowingBuiltins
 class ILLUST(_Section):
     async def follow(self, *, offset: Optional[int] = None) -> IllustSearchResult:
@@ -259,39 +253,10 @@
                         ),
                         output=output,
                     )
                 )
             return result
 
     async def download_ugoira(
-        self,
-        id: int,
-        *,
-        type: Literal["zip", "jpg", "all", "iter"] = "zip",
-    ) -> Optional[
-        Union[
-            ZipFile,
-            List[bytes],
-            Dict[str, Union[ZipFile, List[bytes]]],
-            Iterator[bytes],
-        ]
-    ]:
-        metadata = (await self.ugoira_metadata(id)).metadata
-        zip_url = metadata.zip_url
-        data = await self._client.download(
-            zip_url.original or zip_url.large or zip_url.medium,
-        )
-        if data is None:
-            return None
-        zip_file = ZipFile(BytesIO(data))
-        if type == "zip":
-            return zip_file
-        frames = []
-        for frame_info in metadata.frames:
-            with zip_file.open(frame_info.file) as f:
-                frames.append(f.read())
-        if type == "jpg":
-            return frames
-        elif type == "iter":
-            return iter(frames)
-        else:
-            return {"zip": zip_file, "frames": frames}
+        self, id: int, *, type: UGOIRA_RESULT_TYPE = "zip"
+    ) -> Union[bytes, List[bytes], None]:
+        return await (await self.detail(id)).illust.download_ugoira(type=type)
```

### Comparing `async_pixiv-0.3.6/src/async_pixiv/client/_section/_novel.py` & `async_pixiv-0.3.7/src/async_pixiv/client/_section/_novel.py`

 * *Files identical despite different names*

### Comparing `async_pixiv-0.3.6/src/async_pixiv/client/_section/_user.py` & `async_pixiv-0.3.7/src/async_pixiv/client/_section/_user.py`

 * *Files identical despite different names*

### Comparing `async_pixiv-0.3.6/src/async_pixiv/error.py` & `async_pixiv-0.3.7/src/async_pixiv/error.py`

 * *Files identical despite different names*

### Comparing `async_pixiv-0.3.6/src/async_pixiv/model/_base.py` & `async_pixiv-0.3.7/src/async_pixiv/model/_base.py`

 * *Files identical despite different names*

### Comparing `async_pixiv-0.3.6/src/async_pixiv/model/illust.py` & `async_pixiv-0.3.7/src/async_pixiv/model/illust.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     AIType,
     ImageUrl,
     Series,
     Tag,
 )
 from async_pixiv.model.user import User
 from async_pixiv.utils.ffmpeg import FFmpeg
+from async_pixiv.utils.typedefs import UGOIRA_RESULT_TYPE
 
 try:
     import regex as re
 except ImportError:
     import re
 
 if TYPE_CHECKING:
@@ -49,16 +50,14 @@
 __all__ = [
     "Illust",
     "IllustType",
     "Comment",
     "UgoiraMetadata",
 ]
 
-UGOIRA_RESULT_TYPE = Literal["zip", "jpg", "iter", "gif", "mp4"]
-
 session = Session()
 
 
 class IllustType(Enum):
     illust = "illust"
     ugoira = "ugoira"
     manga = "manga"
@@ -301,15 +300,16 @@
                     .option("y")
                     .option("f", "lavfi")
                     .option("i", "anullsrc")
                     .option("f", "concat")
                     .option("safe", 0)
                     .option(
                         "filter_complex",
-                        "crop='iw-mod(iw,2)':'ih-mod(ih,2)'[main];"
+                        "colormatrix=bt470bg:bt709[0];"
+                        "[0]crop='iw-mod(iw,2)':'ih-mod(ih,2)'[main];"
                         "[main]split[v1][v2];"
                         "[v1]palettegen[pal];"
                         "[v2][pal]paletteuse=dither=sierra2_4a",
                     )
                     .option("i", str(connect_config_file_path.resolve()))
                     .option("pix_fmt", "yuv420p10le")
                     .option("c:v", "libx265")
@@ -325,15 +325,16 @@
                     FFmpeg()
                     .option("y")
                     .option("f", "concat")
                     .option("safe", 0)
                     .option("i", str(connect_config_file_path.resolve()))
                     .option(
                         "filter_complex",
-                        "split[v1][v2];"
+                        "colormatrix=bt470bg:bt709[main];"
+                        "[main]split[v1][v2];"
                         "[v1]palettegen[pal];"
                         "[v2][pal]paletteuse=dither=sierra2_4a",
                     )
                     .option("crf", 0)
                     .output(str(output_path))
                 )
             ffmpeg.on("completed", lambda: event.set())
```

### Comparing `async_pixiv-0.3.6/src/async_pixiv/model/novel.py` & `async_pixiv-0.3.7/src/async_pixiv/model/novel.py`

 * *Files identical despite different names*

### Comparing `async_pixiv-0.3.6/src/async_pixiv/model/other.py` & `async_pixiv-0.3.7/src/async_pixiv/model/other.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,14 +64,17 @@
     ) -> None:
         super().__init__(
             name=name,
             translated_name=translated_name,
             added_by_uploaded_user=added_by_uploaded_user,
         )
 
+    def __str__(self) -> str:
+        return self.name
+
 
 class AIType(IntEnum):
     NONE = 0
     """没有使用AI"""
 
     HALF = 1
     """使用了AI进行辅助"""
```

### Comparing `async_pixiv-0.3.6/src/async_pixiv/model/result.py` & `async_pixiv-0.3.7/src/async_pixiv/model/result.py`

 * *Files identical despite different names*

### Comparing `async_pixiv-0.3.6/src/async_pixiv/model/user.py` & `async_pixiv-0.3.7/src/async_pixiv/model/user.py`

 * *Files identical despite different names*

### Comparing `async_pixiv-0.3.6/src/async_pixiv/utils/context.py` & `async_pixiv-0.3.7/src/async_pixiv/utils/context.py`

 * *Files identical despite different names*

### Comparing `async_pixiv-0.3.6/src/async_pixiv/utils/enums.py` & `async_pixiv-0.3.7/src/async_pixiv/utils/enums.py`

 * *Files identical despite different names*

### Comparing `async_pixiv-0.3.6/src/async_pixiv/utils/ffmpeg/_ffmpeg.py` & `async_pixiv-0.3.7/src/async_pixiv/utils/ffmpeg/_ffmpeg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import asyncio
 import signal
-import sys
 from codecs import StreamReader
 from collections import namedtuple
 from typing import Any, Coroutine, Dict, List, Optional, TYPE_CHECKING
 
 from pyee import EventEmitter
 
+from async_pixiv.utils.const import IS_WINDOWS
 from async_pixiv.utils.ffmpeg.typing import Option
 from async_pixiv.utils.ffmpeg.utils import build_options, parse_progress, read_lines
 
 if TYPE_CHECKING:
     # noinspection PyProtectedMember
     from asyncio.subprocess import Process
 
-_windows = sys.platform == "win32"
-
 
 def _create_subprocess(*args, **kwargs) -> Coroutine[Any, Any, "Process"]:
-    if _windows:
+    if IS_WINDOWS:
         # https://docs.python.org/3/library/asyncio-subprocess.html#asyncio.asyncio.subprocess.Process.send_signal
         from subprocess import CREATE_NEW_PROCESS_GROUP
 
         kwargs["creationflags"] = CREATE_NEW_PROCESS_GROUP
 
     return asyncio.create_subprocess_exec(*args, **kwargs)
 
@@ -101,15 +99,15 @@
             self.emit("error", self._process.returncode)
 
     def terminate(self):
         if not self._executed:
             raise FFmpegError("FFmpeg is not executed")
 
         sigterm = signal.SIGTERM
-        if _windows:  # On Windows, SIGTERM -> TerminateProcess()
+        if IS_WINDOWS:  # On Windows, SIGTERM -> TerminateProcess()
             # https://github.com/FFmpeg/FFmpeg/blob/master/fftools/ffmpeg.c#L356
             sigterm = signal.CTRL_BREAK_EVENT
 
         self._terminated = True
         self._process.send_signal(sigterm)
 
     async def drain(self):
```

### Comparing `async_pixiv-0.3.6/src/async_pixiv/utils/ffmpeg/utils.py` & `async_pixiv-0.3.7/src/async_pixiv/utils/ffmpeg/utils.py`

 * *Files identical despite different names*

### Comparing `async_pixiv-0.3.6/src/async_pixiv/utils/net.py` & `async_pixiv-0.3.7/src/async_pixiv/utils/net.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 from contextlib import asynccontextmanager
 from logging import getLogger
-from typing import Any, AsyncIterator, Optional, Union
+from typing import Any, AsyncIterator, Dict, Optional, Union
 
 from aiolimiter import AsyncLimiter
 
 # noinspection PyProtectedMember
 from httpx import AsyncClient, URL
 
 # noinspection PyProtectedMember
@@ -30,27 +30,28 @@
 )
 
 # noinspection PyProtectedMember
 from httpx._utils import get_environment_proxies
 from yarl import URL
 
 from async_pixiv.utils.context import async_do_nothing
+from async_pixiv.utils.bypass import BypassAsyncHTTPTransport
 from async_pixiv.utils.overwrite import AsyncHTTPTransport, Response
 
 try:
     import regex as re
 except ImportError:
     import re
 
 try:
-    from uvloop import EventLoopPolicy
+    import uvloop
 
-    asyncio.set_event_loop_policy(EventLoopPolicy())
+    asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
 except ImportError:
-    EventLoopPolicy = None
+    uvloop = None
 
 __all__ = ["Net"]
 
 logger = getLogger(__name__)
 
 
 class Net:
@@ -64,16 +65,19 @@
     def __init__(
         self,
         *,
         rate_limiter: Optional[AsyncLimiter] = AsyncLimiter(100),
         proxies: Optional[ProxiesTypes] = None,
         retry: Optional[int] = 5,
         retry_sleep: float = 1,
+        bypass: bool = False,
+        transport_kwargs: Optional[Dict[str, Any]] = None,
         **kwargs,
     ):
+        transport_kwargs = transport_kwargs or {}
         self._rate_limiter = rate_limiter
         if proxies is None:
             proxy_map = {
                 key: None if url is None else Proxy(url=url)
                 for key, url in get_environment_proxies().items()
             }
         elif isinstance(proxies, dict):
@@ -86,19 +90,31 @@
             proxy = Proxy(url=proxies) if isinstance(proxies, (str, URL)) else proxies
             proxy_map = {"all://": proxy}
 
         for i in filter(lambda x: x in kwargs, ["mounts", "transport", "proxies"]):
             del kwargs[i]
         self._retry = retry
         self._retry_sleep = max(retry_sleep, 0)
-        self._client = AsyncClient(
-            mounts={k: AsyncHTTPTransport(proxy=v) for k, v in proxy_map.items()},
-            transport=AsyncHTTPTransport(),
-            **kwargs,
-        )
+        if bypass:
+            self._client = AsyncClient(
+                mounts={
+                    k: BypassAsyncHTTPTransport(proxy=v) for k, v in proxy_map.items()
+                },
+                transport=BypassAsyncHTTPTransport(),
+                **kwargs,
+            )
+        else:
+            self._client = AsyncClient(
+                mounts={
+                    k: AsyncHTTPTransport(proxy=v, **transport_kwargs)
+                    for k, v in proxy_map.items()
+                },
+                transport=AsyncHTTPTransport(**transport_kwargs),
+                **kwargs,
+            )
 
     async def request(
         self,
         method: str,
         url: URLTypes,
         *,
         content: Optional[RequestContent] = None,
@@ -133,15 +149,16 @@
                 async with (self._rate_limiter or async_do_nothing()):
                     return await self._client.send(
                         request, auth=auth, follow_redirects=follow_redirects
                     )
             except Exception as e:
                 error = e
                 logger.warning(
-                    f"Request Error: {e}. Will retry in {self._retry_sleep}s. ({n + 1}th retry)"
+                    f"Request Error: {e}. "
+                    f"Will retry in {self._retry_sleep}s. ({n + 1}th retry)"
                 )
                 await asyncio.sleep(self._retry_sleep)
         if error is not None:
             raise error
 
     async def get(
         self,
```

### Comparing `async_pixiv-0.3.6/src/async_pixiv/utils/overwrite.py` & `async_pixiv-0.3.7/src/async_pixiv/utils/overwrite.py`

 * *Files identical despite different names*

