# Comparing `tmp/Wavelink-2.4.0.tar.gz` & `tmp/Wavelink-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Wavelink-2.4.0.tar", last modified: Fri Jun  9 02:56:36 2023, max compression
+gzip compressed data, was "Wavelink-2.5.0.tar", last modified: Thu Jun 15 02:34:49 2023, max compression
```

## Comparing `Wavelink-2.4.0.tar` & `Wavelink-2.5.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 02:56:36.083344 Wavelink-2.4.0/
--rw-rw-rw-   0        0        0     1108 2023-03-09 18:26:07.000000 Wavelink-2.4.0/LICENSE
--rw-rw-rw-   0        0        0     5772 2023-06-09 02:56:36.083344 Wavelink-2.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     4969 2023-03-09 18:33:50.000000 Wavelink-2.4.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-09 02:56:36.069282 Wavelink-2.4.0/Wavelink.egg-info/
--rw-rw-rw-   0        0        0     5772 2023-06-09 02:56:36.000000 Wavelink-2.4.0/Wavelink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-06-09 02:56:36.000000 Wavelink-2.4.0/Wavelink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 02:56:36.000000 Wavelink-2.4.0/Wavelink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-09 02:56:36.000000 Wavelink-2.4.0/Wavelink.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-09 02:56:36.000000 Wavelink-2.4.0/Wavelink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1006 2023-06-05 09:48:12.000000 Wavelink-2.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       49 2023-03-09 18:26:07.000000 Wavelink-2.4.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 02:56:36.083344 Wavelink-2.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-09 02:56:36.078839 Wavelink-2.4.0/wavelink/
--rw-rw-rw-   0        0        0     1495 2023-06-05 09:48:12.000000 Wavelink-2.4.0/wavelink/__init__.py
--rw-rw-rw-   0        0        0     2701 2023-03-09 18:26:07.000000 Wavelink-2.4.0/wavelink/backoff.py
--rw-rw-rw-   0        0        0     3689 2023-06-05 10:25:32.000000 Wavelink-2.4.0/wavelink/enums.py
--rw-rw-rw-   0        0        0     3028 2023-06-05 09:44:43.000000 Wavelink-2.4.0/wavelink/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-09 02:56:36.052882 Wavelink-2.4.0/wavelink/ext/
-drwxrwxrwx   0        0        0        0 2023-06-09 02:56:36.079340 Wavelink-2.4.0/wavelink/ext/spotify/
--rw-rw-rw-   0        0        0    17854 2023-06-05 11:43:40.000000 Wavelink-2.4.0/wavelink/ext/spotify/__init__.py
--rw-rw-rw-   0        0        0    20203 2023-03-09 18:26:07.000000 Wavelink-2.4.0/wavelink/filters.py
--rw-rw-rw-   0        0        0    17836 2023-06-05 08:54:30.000000 Wavelink-2.4.0/wavelink/node.py
--rw-rw-rw-   0        0        0     3461 2023-05-20 08:41:44.000000 Wavelink-2.4.0/wavelink/payloads.py
--rw-rw-rw-   0        0        0    21928 2023-06-05 13:30:06.000000 Wavelink-2.4.0/wavelink/player.py
--rw-rw-rw-   0        0        0    12384 2023-03-15 08:08:05.000000 Wavelink-2.4.0/wavelink/queue.py
--rw-rw-rw-   0        0        0    10222 2023-06-05 10:36:36.000000 Wavelink-2.4.0/wavelink/tracks.py
-drwxrwxrwx   0        0        0        0 2023-06-09 02:56:36.082342 Wavelink-2.4.0/wavelink/types/
--rw-rw-rw-   0        0        0      860 2023-03-09 18:26:07.000000 Wavelink-2.4.0/wavelink/types/events.py
--rw-rw-rw-   0        0        0      635 2023-03-09 18:26:07.000000 Wavelink-2.4.0/wavelink/types/request.py
--rw-rw-rw-   0        0        0      424 2023-03-09 18:26:07.000000 Wavelink-2.4.0/wavelink/types/state.py
--rw-rw-rw-   0        0        0      343 2023-03-09 18:26:07.000000 Wavelink-2.4.0/wavelink/types/track.py
--rw-rw-rw-   0        0        0     9570 2023-05-20 08:53:53.000000 Wavelink-2.4.0/wavelink/websocket.py
+drwxrwxrwx   0        0        0        0 2023-06-15 02:34:49.423637 Wavelink-2.5.0/
+-rw-rw-rw-   0        0        0     1108 2023-03-09 18:26:07.000000 Wavelink-2.5.0/LICENSE
+-rw-rw-rw-   0        0        0     5772 2023-06-15 02:34:49.423637 Wavelink-2.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4969 2023-03-09 18:33:50.000000 Wavelink-2.5.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-15 02:34:49.407184 Wavelink-2.5.0/Wavelink.egg-info/
+-rw-rw-rw-   0        0        0     5772 2023-06-15 02:34:49.000000 Wavelink-2.5.0/Wavelink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-06-15 02:34:49.000000 Wavelink-2.5.0/Wavelink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 02:34:49.000000 Wavelink-2.5.0/Wavelink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-15 02:34:49.000000 Wavelink-2.5.0/Wavelink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-15 02:34:49.000000 Wavelink-2.5.0/Wavelink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1006 2023-06-15 00:30:25.000000 Wavelink-2.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       49 2023-03-09 18:26:07.000000 Wavelink-2.5.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 02:34:49.424137 Wavelink-2.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-15 02:34:49.418133 Wavelink-2.5.0/wavelink/
+-rw-rw-rw-   0        0        0     1495 2023-06-15 00:30:25.000000 Wavelink-2.5.0/wavelink/__init__.py
+-rw-rw-rw-   0        0        0     2701 2023-03-09 18:26:07.000000 Wavelink-2.5.0/wavelink/backoff.py
+-rw-rw-rw-   0        0        0     3689 2023-06-05 10:25:32.000000 Wavelink-2.5.0/wavelink/enums.py
+-rw-rw-rw-   0        0        0     3028 2023-06-05 09:44:43.000000 Wavelink-2.5.0/wavelink/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-15 02:34:49.389981 Wavelink-2.5.0/wavelink/ext/
+drwxrwxrwx   0        0        0        0 2023-06-15 02:34:49.419134 Wavelink-2.5.0/wavelink/ext/spotify/
+-rw-rw-rw-   0        0        0    17743 2023-06-15 00:16:21.000000 Wavelink-2.5.0/wavelink/ext/spotify/__init__.py
+-rw-rw-rw-   0        0        0    20203 2023-03-09 18:26:07.000000 Wavelink-2.5.0/wavelink/filters.py
+-rw-rw-rw-   0        0        0    17836 2023-06-05 08:54:30.000000 Wavelink-2.5.0/wavelink/node.py
+-rw-rw-rw-   0        0        0     3461 2023-05-20 08:41:44.000000 Wavelink-2.5.0/wavelink/payloads.py
+-rw-rw-rw-   0        0        0    22017 2023-06-12 11:33:29.000000 Wavelink-2.5.0/wavelink/player.py
+-rw-rw-rw-   0        0        0    12545 2023-06-15 00:04:14.000000 Wavelink-2.5.0/wavelink/queue.py
+-rw-rw-rw-   0        0        0     9954 2023-06-15 00:00:10.000000 Wavelink-2.5.0/wavelink/tracks.py
+drwxrwxrwx   0        0        0        0 2023-06-15 02:34:49.422636 Wavelink-2.5.0/wavelink/types/
+-rw-rw-rw-   0        0        0      860 2023-03-09 18:26:07.000000 Wavelink-2.5.0/wavelink/types/events.py
+-rw-rw-rw-   0        0        0      635 2023-03-09 18:26:07.000000 Wavelink-2.5.0/wavelink/types/request.py
+-rw-rw-rw-   0        0        0      424 2023-03-09 18:26:07.000000 Wavelink-2.5.0/wavelink/types/state.py
+-rw-rw-rw-   0        0        0      343 2023-03-09 18:26:07.000000 Wavelink-2.5.0/wavelink/types/track.py
+-rw-rw-rw-   0        0        0     9570 2023-05-20 08:53:53.000000 Wavelink-2.5.0/wavelink/websocket.py
```

### Comparing `Wavelink-2.4.0/LICENSE` & `Wavelink-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Wavelink-2.4.0/PKG-INFO` & `Wavelink-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Wavelink
-Version: 2.4.0
+Version: 2.5.0
 Summary: A robust and powerful Lavalink wrapper for discord.py
 Author-email: EvieePy <evieepy@gmail.com>
 Project-URL: Homepage, https://github.com/PythonistaGuild/Wavelink
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `Wavelink-2.4.0/README.rst` & `Wavelink-2.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `Wavelink-2.4.0/Wavelink.egg-info/PKG-INFO` & `Wavelink-2.5.0/Wavelink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Wavelink
-Version: 2.4.0
+Version: 2.5.0
 Summary: A robust and powerful Lavalink wrapper for discord.py
 Author-email: EvieePy <evieepy@gmail.com>
 Project-URL: Homepage, https://github.com/PythonistaGuild/Wavelink
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `Wavelink-2.4.0/Wavelink.egg-info/SOURCES.txt` & `Wavelink-2.5.0/Wavelink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Wavelink-2.4.0/pyproject.toml` & `Wavelink-2.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Wavelink"
-version = "2.4.0"
+version = "2.5.0"
 authors = [
   { name="EvieePy", email="evieepy@gmail.com" },
 ]
 dynamic = ["dependencies"]
 description = "A robust and powerful Lavalink wrapper for discord.py"
 readme = "README.rst"
 requires-python = ">=3.10"
```

### Comparing `Wavelink-2.4.0/wavelink/__init__.py` & `Wavelink-2.5.0/wavelink/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 __title__ = "WaveLink"
 __author__ = "PythonistaGuild, EvieePy"
 __license__ = "MIT"
 __copyright__ = "Copyright 2019-Present (c) PythonistaGuild, EvieePy"
-__version__ = "2.4.0"
+__version__ = "2.5.0"
 
 from .enums import *
 from .exceptions import *
 from .node import *
 from .payloads import *
 from .player import Player as Player
 from .tracks import *
```

### Comparing `Wavelink-2.4.0/wavelink/backoff.py` & `Wavelink-2.5.0/wavelink/backoff.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.4.0/wavelink/enums.py` & `Wavelink-2.5.0/wavelink/enums.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.4.0/wavelink/exceptions.py` & `Wavelink-2.5.0/wavelink/exceptions.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.4.0/wavelink/ext/spotify/__init__.py` & `Wavelink-2.5.0/wavelink/ext/spotify/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,44 +241,49 @@
         self.uri: str = data['uri']
         self.id: str = data['id']
         self.length: int = data['duration_ms']
         self.duration: int = self.length
 
         self.isrc: str | None = data["external_ids"].get("isrc")
 
+    def __str__(self) -> str:
+        return f'{self.name} - {self.artists[0]}'
+
+    def __repr__(self) -> str:
+        return f'SpotifyTrack(id={self.id}, isrc={self.isrc}, name={self.name}, duration={self.duration})'
+
     def __eq__(self, other) -> bool:
-        return self.id == other.id
+        if isinstance(other, SpotifyTrack):
+            return self.id == other.id
+        raise NotImplemented
 
     @classmethod
     async def search(
         cls: Type[ST],
             query: str,
             *,
             type: SpotifySearchType = SpotifySearchType.track,
             node: Node | None = None,
-            return_first: bool = False,
     ) -> Union[Optional[ST], List[ST]]:
         """|coro|
 
         Search for tracks with the given query.
 
         Parameters
         ----------
         query: str
             The song to search for.
         type: Optional[:class:`~SpotifySearchType`]
             An optional enum value to use when searching with Spotify. Defaults to track.
         node: Optional[:class:`wavelink.Node`]
             An optional Node to use to make the search with.
-        return_first: Optional[bool]
-            An optional bool which when set to True will return only the first track found. Defaults to False.
 
         Returns
         -------
-        Union[Optional[:class:`SpotifyTrack`], List[:class:`SpotifyTrack`]]
+        List[:class:`SpotifyTrack`]
 
         Examples
         --------
         Searching for a singular tack to play...
 
         .. code:: python3
 
@@ -297,18 +302,14 @@
 
             See :func:`~.decode_url` for gathering information about the supplied URL, including search type.
             Before using this method.
         """
         if node is None:
             node: Node = NodePool.get_connected_node()
 
-        if type == SpotifySearchType.track:
-            tracks = await node._spotify._search(query=query, type=type)
-
-            return tracks[0] if return_first else tracks
         return await node._spotify._search(query=query, type=type)
 
     @classmethod
     def iterator(cls,
                  *,
                  query: str,
                  limit: int | None = None,
@@ -359,15 +360,15 @@
 
         Used as a type hint in a
         `discord.py command <https://discordpy.readthedocs.io/en/stable/ext/commands/commands.html>`_.
         """
         results = await cls.search(argument)
 
         if not results:
-            raise commands.BadArgument("Could not find any songs matching that query.")
+            raise commands.BadArgument(f"Could not find any songs matching query: {argument}")
 
         return results[0]
 
     async def fulfill(self, *, player: Player, cls: Playable, populate: bool) -> Playable:
         """Used to fulfill the :class:`wavelink.Player` Auto Play Queue.
 
         .. warning::
@@ -458,15 +459,15 @@
             self._bearer_token = data['access_token']
             self._expiry = time.time() + (int(data['expires_in']) - 10)
 
     async def _search(self,
                       query: str,
                       type: SpotifySearchType = SpotifySearchType.track,
                       iterator: bool = False,
-                      ) -> SpotifyTrack | list[SpotifyTrack]:
+                      ) -> list[SpotifyTrack]:
 
         if not self._bearer_token or time.time() >= self._expiry:
             await self._get_bearer_token()
 
         regex_result = URLREGEX.match(query)
 
         url = (
@@ -479,15 +480,15 @@
         async with self.session.get(url, headers=self.bearer_headers) as resp:
             if resp.status != 200:
                 raise SpotifyRequestError(resp.status, resp.reason)
 
             data = await resp.json()
 
         if data['type'] == 'track':
-            return SpotifyTrack(data)
+            return [SpotifyTrack(data)]
 
         elif data['type'] == 'album':
             album_data: dict[str, Any]= {
                                         'album_type': data['album_type'],
                                         'artists': data['artists'],
                                         'available_markets': data['available_markets'],
                                         'external_urls': data['external_urls'],
```

### Comparing `Wavelink-2.4.0/wavelink/filters.py` & `Wavelink-2.5.0/wavelink/filters.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.4.0/wavelink/node.py` & `Wavelink-2.5.0/wavelink/node.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.4.0/wavelink/payloads.py` & `Wavelink-2.5.0/wavelink/payloads.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.4.0/wavelink/player.py` & `Wavelink-2.5.0/wavelink/player.py`

 * *Files 1% similar despite different names*

```diff
@@ -575,38 +575,39 @@
                                                              data=data)        
 
         if self.is_playing() and seek:
             await self.seek(int(self.position))
         logger.debug(f"Set filter:: {self._filter} ({self.channel.id})")
 
     def _invalidate(self) -> None:
+        try:
+            self.cleanup()
+        except Exception as e:
+            logger.debug(f'Failed to cleanup player, most likely due to never having been connected: {e}')
+
         self._voice_state = {}
         self._player_state = {}
         self.channel = None
 
     async def _destroy(self) -> None:
-        self.autoplay = False
-        self._voice_state = {}
-        self._player_state = {}
-
-        self.cleanup()
-        self.channel = None
+        self._invalidate()
 
         await self.current_node._send(method='DELETE',
                                       path=f'sessions/{self.current_node._session_id}/players',
                                       guild_id=self._guild.id)
 
         del self.current_node._players[self._guild.id]
         logger.debug(f'Player {self._guild.id} was destroyed.')
 
     async def disconnect(self, **kwargs) -> None:
         """|coro|
 
         Disconnect the Player from voice and cleanup the Player state.
         """
+        self._invalidate()
         await self.guild.change_voice_state(channel=None)
 
     async def _swap_state(self) -> None:
         assert self._guild is not None
 
         try:
             self._player_state['track']
```

### Comparing `Wavelink-2.4.0/wavelink/queue.py` & `Wavelink-2.5.0/wavelink/queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 """
 from __future__ import annotations
 
 import asyncio
 from collections import deque
 from collections.abc import AsyncIterator, Iterable, Iterator
 from copy import copy
+import random
 
 from .exceptions import QueueEmpty
 from .tracks import Playable
 from .ext import spotify
 
 
 __all__ = (
@@ -203,14 +204,18 @@
         """Put the given item into the queue at the specified index."""
         self._insert(index, self._check_playable(item))
 
     def put_at_front(self, item: Playable | spotify.SpotifyTrack) -> None:
         """Put the given item into the front of the queue."""
         self.put_at_index(0, item)
 
+    def shuffle(self) -> None:
+        """Shuffles the queue in place. This does not return anything."""
+        random.shuffle(self._queue)
+
     def extend(self, iterable: Iterable[Playable | spotify.SpotifyTrack], *, atomic: bool = True) -> None:
         """Add the members of the given iterable to the end of the queue.
 
         If atomic is set to True, no tracks will be added upon any exceptions.
         If atomic is set to False, as many tracks will be added as possible.
 
         """
```

### Comparing `Wavelink-2.4.0/wavelink/tracks.py` & `Wavelink-2.5.0/wavelink/tracks.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,90 +134,77 @@
     
     @overload
     @classmethod
     async def search(cls,
                      query: str,
                      /,
                      *,
-                     return_first: Literal[False] = ...,
                      node: Node | None = ...
                      ) -> list[Self]:
         ...
 
     @overload
     @classmethod
     async def search(cls,
                      query: str,
                      /,
                      *,
-                     return_first: Literal[True] = ...,
                      node: Node | None = ...
                      ) -> Self:
         ...
 
     @overload
     @classmethod
     async def search(cls,
                      query: str,
                      /,
                      *,
-                     return_first: bool = ...,
                      node: Node | None = ...
                      ) -> Self | list[Self]:
         ...
 
     @overload
     @classmethod
     async def search(cls,
                      query: str,
                      /,
                      *,
-                     return_first: bool = ...,
                      node: Node | None = ...
                      ) -> YouTubePlaylist:
         ...
 
     @classmethod
     async def search(cls,
                      query: str,
                      /,
                      *,
-                     return_first: bool = False,
                      node: Node | None = None
                      ) -> Self | list[Self]:
         """Search and retrieve tracks for the given query.
 
         Parameters
         ----------
         query: str
             The query to search for.
-        return_first: Optional[bool]
-            Whether to return the first track from the search results. Defaults to False.
         node: Optional[:class:`wavelink.Node`]
             The node to use when searching for tracks. If no :class:`wavelink.Node` is passed,
             one will be fetched via the :class:`wavelink.NodePool`.
         """
 
         check = yarl.URL(query)
 
         if str(check.host) == 'youtube.com' or str(check.host) == 'www.youtube.com' and check.query.get("list") or \
                 cls.PREFIX == 'ytpl:':
 
             playlist = await NodePool.get_playlist(query, cls=YouTubePlaylist, node=node)
             return playlist
+        elif check.host:
+            tracks = await NodePool.get_tracks(query, cls=cls, node=node)
         else:
             tracks = await NodePool.get_tracks(f'{cls.PREFIX}{query}', cls=cls, node=node)
-        
-        try:
-            track = tracks[0]
-        except IndexError:
-            raise NoTracksError(f'Your search query "{query}" returned no tracks.')
-
-        if return_first:
-            return track
 
         return tracks
 
     @classmethod
     async def convert(cls, ctx: commands.Context, argument: str) -> Self:
         """Converter which searches for and returns the first track.
 
@@ -243,35 +230,42 @@
     ...
 
 
 class YouTubeTrack(Playable):
 
     PREFIX: str = 'ytsearch:'
 
+    def __init__(self, data: TrackPayload) -> None:
+        super().__init__(data)
+
+        self._thumb: str = f"https://img.youtube.com/vi/{self.identifier}/maxresdefault.jpg"
+
     @property
     def thumbnail(self) -> str:
         """The URL to the thumbnail of this video.
 
         .. note::
 
             Due to YouTube limitations this may not always return a valid thumbnail.
             Use :meth:`.fetch_thumbnail` to fallback.
 
         Returns
         -------
         str
             The URL to the video thumbnail.
         """
-        return f"https://img.youtube.com/vi/{self.identifier}/maxresdefault.jpg"
+        return self._thumb
 
     thumb = thumbnail
 
     async def fetch_thumbnail(self, *, node: Node | None = None) -> str:
         """Fetch the max resolution thumbnail with a fallback if it does not exist.
 
+        This sets and overrides the default ``thumbnail`` and ``thumb`` properties.
+
         .. note::
 
             This method uses an API request to fetch the thumbnail.
 
         Returns
         -------
         str
@@ -283,14 +277,15 @@
         session: aiohttp.ClientSession = node._session
         url: str = f"https://img.youtube.com/vi/{self.identifier}/maxresdefault.jpg"
 
         async with session.get(url=url) as resp:
             if resp.status == 404:
                 url = f'https://img.youtube.com/vi/{self.identifier}/hqdefault.jpg'
 
+        self._thumb = url
         return url
 
 
 class YouTubeMusicTrack(YouTubeTrack):
     """A track created using a search to YouTube Music."""
 
     PREFIX: str = "ytmsearch:"
```

### Comparing `Wavelink-2.4.0/wavelink/types/events.py` & `Wavelink-2.5.0/wavelink/types/events.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.4.0/wavelink/types/request.py` & `Wavelink-2.5.0/wavelink/types/request.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.4.0/wavelink/websocket.py` & `Wavelink-2.5.0/wavelink/websocket.py`

 * *Files identical despite different names*

