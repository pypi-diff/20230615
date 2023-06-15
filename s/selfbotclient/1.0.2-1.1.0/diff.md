# Comparing `tmp/selfbotclient-1.0.2.tar.gz` & `tmp/selfbotclient-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selfbotclient-1.0.2.tar", last modified: Mon Jun 12 19:42:16 2023, max compression
+gzip compressed data, was "selfbotclient-1.1.0.tar", last modified: Thu Jun 15 17:20:37 2023, max compression
```

## Comparing `selfbotclient-1.0.2.tar` & `selfbotclient-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 19:42:16.776562 selfbotclient-1.0.2/
--rw-rw-rw-   0        0        0     1459 2023-06-12 19:42:16.776562 selfbotclient-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      860 2023-06-12 19:38:25.000000 selfbotclient-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 19:42:16.766562 selfbotclient-1.0.2/SelfBotClient/
--rw-rw-rw-   0        0        0      376 2023-06-12 19:28:12.000000 selfbotclient-1.0.2/SelfBotClient/__init__.py
--rw-rw-rw-   0        0        0      472 2023-06-09 23:04:28.000000 selfbotclient-1.0.2/SelfBotClient/__main__.py
--rw-rw-rw-   0        0        0    17005 2023-06-12 19:35:33.000000 selfbotclient-1.0.2/SelfBotClient/client.py
--rw-rw-rw-   0        0        0     1399 2023-06-07 23:57:30.000000 selfbotclient-1.0.2/SelfBotClient/enums.py
--rw-rw-rw-   0        0        0      826 2023-06-06 22:37:48.000000 selfbotclient-1.0.2/SelfBotClient/errors.py
--rw-rw-rw-   0        0        0    11955 2023-06-09 21:57:25.000000 selfbotclient-1.0.2/SelfBotClient/http.py
--rw-rw-rw-   0        0        0     1046 2023-06-08 23:49:03.000000 selfbotclient-1.0.2/SelfBotClient/logger.py
--rw-rw-rw-   0        0        0      807 2023-06-09 13:27:08.000000 selfbotclient-1.0.2/SelfBotClient/permissionbuilder.py
--rw-rw-rw-   0        0        0     1124 2023-06-12 19:29:03.000000 selfbotclient-1.0.2/SelfBotClient/threads.py
--rw-rw-rw-   0        0        0      313 2023-06-07 23:24:53.000000 selfbotclient-1.0.2/SelfBotClient/typings.py
--rw-rw-rw-   0        0        0    17057 2023-06-09 21:55:30.000000 selfbotclient-1.0.2/SelfBotClient/user.py
-drwxrwxrwx   0        0        0        0 2023-06-12 19:42:16.775563 selfbotclient-1.0.2/selfbotclient.egg-info/
--rw-rw-rw-   0        0        0     1459 2023-06-12 19:42:16.000000 selfbotclient-1.0.2/selfbotclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      478 2023-06-12 19:42:16.000000 selfbotclient-1.0.2/selfbotclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 19:42:16.000000 selfbotclient-1.0.2/selfbotclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-12 19:42:16.000000 selfbotclient-1.0.2/selfbotclient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-12 19:42:16.000000 selfbotclient-1.0.2/selfbotclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 19:42:16.777562 selfbotclient-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1243 2023-06-12 19:42:13.000000 selfbotclient-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 17:20:37.132355 selfbotclient-1.1.0/
+-rw-rw-rw-   0        0        0     1890 2023-06-15 17:20:37.132355 selfbotclient-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1286 2023-06-15 16:58:24.000000 selfbotclient-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 17:20:37.116356 selfbotclient-1.1.0/SelfBotClient/
+-rw-rw-rw-   0        0        0      376 2023-06-14 23:07:30.000000 selfbotclient-1.1.0/SelfBotClient/__init__.py
+-rw-rw-rw-   0        0        0      472 2023-06-09 23:04:28.000000 selfbotclient-1.1.0/SelfBotClient/__main__.py
+-rw-rw-rw-   0        0        0    16059 2023-06-15 17:18:55.000000 selfbotclient-1.1.0/SelfBotClient/client.py
+-rw-rw-rw-   0        0        0     1463 2023-06-15 15:43:34.000000 selfbotclient-1.1.0/SelfBotClient/enums.py
+-rw-rw-rw-   0        0        0      795 2023-06-12 22:50:06.000000 selfbotclient-1.1.0/SelfBotClient/errors.py
+-rw-rw-rw-   0        0        0    11687 2023-06-15 16:10:23.000000 selfbotclient-1.1.0/SelfBotClient/http.py
+-rw-rw-rw-   0        0        0     1046 2023-06-12 22:50:54.000000 selfbotclient-1.1.0/SelfBotClient/logger.py
+-rw-rw-rw-   0        0        0      609 2023-06-15 15:59:48.000000 selfbotclient-1.1.0/SelfBotClient/permissionbuilder.py
+-rw-rw-rw-   0        0        0     2713 2023-06-15 16:38:57.000000 selfbotclient-1.1.0/SelfBotClient/thread.py
+-rw-rw-rw-   0        0        0      313 2023-06-15 01:26:01.000000 selfbotclient-1.1.0/SelfBotClient/typings.py
+-rw-rw-rw-   0        0        0    18892 2023-06-15 17:17:27.000000 selfbotclient-1.1.0/SelfBotClient/user.py
+drwxrwxrwx   0        0        0        0 2023-06-15 17:20:37.131355 selfbotclient-1.1.0/selfbotclient.egg-info/
+-rw-rw-rw-   0        0        0     1890 2023-06-15 17:20:37.000000 selfbotclient-1.1.0/selfbotclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      477 2023-06-15 17:20:37.000000 selfbotclient-1.1.0/selfbotclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 17:20:37.000000 selfbotclient-1.1.0/selfbotclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-15 17:20:37.000000 selfbotclient-1.1.0/selfbotclient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-15 17:20:37.000000 selfbotclient-1.1.0/selfbotclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 17:20:37.132355 selfbotclient-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1243 2023-06-15 17:20:36.000000 selfbotclient-1.1.0/setup.py
```

### Comparing `selfbotclient-1.0.2/README.md` & `selfbotclient-1.1.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,28 @@
+**Project only for educational purposes! 🤓**
+
+![Downloads](https://pepy.tech/badge/selfbotclient)
+[![Documentation Status](https://readthedocs.org/projects/selfbotclient/badge/?version=latest)](https://selfbotclient.readthedocs.io/en/latest/?badge=latest)
+![master](https://img.shields.io/github/last-commit/badges/shields/master)
+![commits](https://badgen.net/github/commits/xXenvy/selfbotclient/master)
 
 # ⚡ Fast Self Bot Client
 - Token Checker | `1` token / `140`ms
-- 3 requests / 1s `(in feature 10 requests / 1s using threads)`
-
+- +10 requests / 1s `(using threads)`
 
-https://github.com/xXenvy/SelfBotClient/assets/111158232/eb5961eb-0a8d-44f1-93b0-48d7a1f6fce0
+https://github.com/xXenvy/SelfBotClient/assets/111158232/ede9fb47-d489-4d9a-b58d-95c06dea6fe9
 
 
 # 🔧 Full control
 - A separate method to send your own requests
 - Ability to manage individual selfbots
 
 # 📌 Ratelimit handler
-
 - The library itself detects whether you have reached the ratelimit of the discord and, if so, forces you to wait a certain time.
+![Test](https://i.imgur.com/hTUFQKF.png)
 # 🛠️ Installation
 ```shell
 pip install -U selfbotclient
 ```
 # 💫 Usage
 ```py
 from SelfBotClient import Client
```

### Comparing `selfbotclient-1.0.2/SelfBotClient/client.py` & `selfbotclient-1.1.0/SelfBotClient/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,139 +1,125 @@
 from .http import HTTPClient
 from .typings import API_VERSION, ClientResponse, RGB_COLOR
 from .enums import ChannelType
 from .permissionbuilder import PermissionBuilder
-from .threads import Threads
+from .thread import Thread
 
 from collections.abc import AsyncIterable
 
 from typing import Union
 from asyncio import AbstractEventLoop
 
 
 class Client(HTTPClient):
-    __version__: str = "1.0.2"
+    """
+    :class:`Client` supports all services of the :class:`SelfBotClient.user`.
+    It has methods such as :class:`Client.send_message` which it calls in all users.
+
+    :param api_version: version of the discord api used by the client
+    :param loop: Set the event loop that will be used by the client
+    :param logger: Enable/disable the logger
+    :param request_latency: Control the rate of requests sent to discord
+    :param ratelimit_additional_cooldown: Add a cooldown to the ratelimit
+    :param use_threading: Enable or disable the threading option (:class:`SelfBotClient.thread`), which for now is in beta.
+
+    """
+
+    __version__: str = "1.1.0"
 
     def __init__(
             self,
             api_version: API_VERSION,
             loop: AbstractEventLoop = None,
             logger: bool = True,
             request_latency: float = 0.1,
             ratelimit_additional_cooldown: float = 10,
             use_threading: bool = False
     ):
-        """
-        The __init__ function is called when the class is instantiated.
-        It sets up all of the attributes that are needed for the class to function properly.
-
-
-        :param self: Represent the instance of the class
-        :param api_version: API_VERSION: Set the api version of the client
-        :param loop: AbstractEventLoop: Specify the event loop that the client will use
-        :param logger: bool: Enable/disable logging
-        :param request_latency: float: Set the time between requests
-        :param ratelimit_additional_cooldown: float: Add a cooldown to the ratelimit
-        :param use_threading: bool: Determine if the client should use threading
-        :return: None
-        """
 
         super().__init__(api_version, loop, logger, request_latency, ratelimit_additional_cooldown)
 
         if use_threading:
-            self.thread: Threads = Threads(client=self)
+            self.thread: Thread = Thread(client=self)
 
     def login(self, token: Union[str, list[str]]) -> None:
         """
         The login function is used to check the provided tokens.
 
-        :param self: Represent the instance of the class
-        :param token: Union[str, list[str]] tokens to check
-        :return: None
+        :param token: tokens to check
         """
 
         if self.logger._status:
             self.logger.info("Checking the provided tokens")
 
         self._tokens: Union[str, list[str]] = token
         self._check_tokens()
 
     async def send_message(self, channel_id: int, message_content: str) -> Union[None, AsyncIterable[ClientResponse]]:
         """
         The send_message function sends a message to the specified channel.
 
-        :param self: Refer to the current instance of a class
-        :param channel_id: int: Specify the channel to send the message to
-        :param message_content: str: Specify the message that will be sent to each user
-        :return: An asynciterable of clientresponse objects or None
+        :param channel_id: Specify the channel to send the message to
+        :param message_content: content of the message
         """
 
         for user in self.users:
             response: ClientResponse = await user.send_message(channel_id, message_content)
             yield response
 
     async def delete_channel(self, channel_id: int) -> Union[None, ClientResponse]:
         """
         The delete_channel function deletes a channel from the server.
 
-        :param self: Refer to the object itself
-        :param channel_id: int: Specify the channel that is to be deleted
-        :return: A clientresponse object or None
+        :param channel_id: Specify the channel that is to be deleted
         """
 
         for user in self.users:
             response: ClientResponse = await user.delete_channel(channel_id)
             if response.status == 200:
                 return response
 
     async def delete_channels(self, channel_ids: list[int]) -> Union[None, AsyncIterable[ClientResponse]]:
         """
         The delete_channels function takes a list of channel_ids and deletes them.
-            It returns an AsyncIterable of ClientResponse objects, which can be used to check the status code for each request.
+        It returns an AsyncIterable of ClientResponse objects, which can be used to check the status code for each request.
 
-        :param self: Access the class variables and methods
-        :param channel_ids: list[int]: Specify the list of channel ids that will be deleted
-        :return: An asynciterable of clientresponse objects or None
+        :param channel_ids: Specify the list of channel ids that will be deleted
         """
 
         while len(channel_ids):
             for user in self.users:
                 channel_id: int = channel_ids.pop(0)
                 response: ClientResponse = await user.delete_channel(channel_id)
                 yield response
 
     async def create_channel(self, guild_id: int, name: str, channel_type: ChannelType,
                              topic: str = None, user_limit: int = None, position: int = None, nsfw: bool = False) -> Union[None, AsyncIterable[ClientResponse]]:
         """
         The create_channel function creates a channel in the specified guild.
 
-        :param self: Refer to the object itself
-        :param guild_id: int: Specify the guild id of the server you want to create a channel in
-        :param name: str: Specify the name of the channel
-        :param channel_type: ChannelType: Specify what type of channel you want to create
-        :param topic: str: Set the topic of the channel
-        :param user_limit: int: Set the maximum number of users allowed in a voice channel
-        :param position: int: Set the position of the channel in the list
-        :param nsfw: bool: Determine whether the channel is nsfw or not
-        :return: An asynciterable of clientresponse objects or None
+        :param guild_id: Specify the guild id of the server you want to create a channel in
+        :param name: Specify the name of the channel
+        :param channel_type: Specify what type of channel you want to create
+        :param topic: Set the topic of the channel
+        :param user_limit: Set the maximum number of users allowed in a voice channel
+        :param position: Set the position of the channel in the list
+        :param nsfw: Determine whether the channel is nsfw or not
         """
 
         for user in self.users:
             response: ClientResponse = await user.create_channel(guild_id, name, channel_type, topic, user_limit, position, nsfw)
             yield response
 
     async def get_channels(self, guild_id: int) -> Union[None, AsyncIterable[ClientResponse]]:
         """
         The get_channels function is a coroutine that takes in a guild_id and returns an AsyncIterable of ClientResponse objects.
-        The function iterates through the users list, calling get_channels on each user object with the given guild_id as its argument.
-        It then yields each response to be used by other functions.
+        The function can return the data of all channels on the server
 
-        :param self: Refer to the current instance of a class
-        :param guild_id: int: Specify the guild id of the channels you want to get
-        :return: An asynciterable of clientresponse objects or None
+        :param guild_id: Specify the guild id of the server you want to get channels from
         """
 
         for user in self.users:
             response: ClientResponse = await user.get_channels(guild_id)
             yield response
 
     async def create_role(self,
@@ -141,98 +127,81 @@
                                 name: str,
                                 color: RGB_COLOR = None,
                                 hoist: bool = False,
                                 permissions: PermissionBuilder = None) -> Union[None, AsyncIterable[ClientResponse]]:
         """
         The create_role function creates a role in the specified guild.
 
-        :param self: Access the attributes and methods of the class
-        :param guild_id: int: Specify the guild in which you want to create a role
-        :param name: str: Set the name of the role
-        :param color: RGB_COLOR: Set the color of the role
-        :param hoist: bool: Determine whether the role should be displayed separately in the user list
-        :param permissions: PermissionBuilder: Set the permissions for the role
-        :return: An asynciterable of clientresponse objects or None
+        :param guild_id: Specify the guild in which you want to create a role
+        :param name: Set the name of the role
+        :param color: Set the color of the role
+        :param hoist: Determine whether the role should be displayed separately in the user list
+        :param permissions: Set the permissions for the role
         """
 
         for user in self.users:
             response: ClientResponse = await user.create_role(guild_id, name, color, hoist, permissions)
             yield response
 
     async def get_roles(self, guild_id: int) -> Union[None, AsyncIterable[ClientResponse]]:
         """
-        The get_roles function is a coroutine that takes in a guild_id and returns an AsyncIterable of ClientResponse objects.
-        The function iterates through the users attribute, which is an array of User objects, and calls the get_roles function on each user object.
-        The get_roles function returns a ClientResponse object for each user.
-
-        :param self: Refer to the current instance of the class
-        :param guild_id: int: Specify the guild id of the server you want to get roles from
-        :return: An asynciterable of clientresponse objects or None
+        get_roles returns a list of data with all the roles on the server
+
+        :param guild_id: Specify the guild id of the server you want to get roles from
         """
         for user in self.users:
             response: ClientResponse = await user.get_roles(guild_id)
             yield response
 
     async def delete_roles(self, guild_id: int, role_ids: list[int]) -> Union[None, AsyncIterable[ClientResponse]]:
 
         """
-        The delete_roles function is a coroutine that takes in two arguments:
-            1. guild_id - the id of the server to delete roles from
-            2. role_ids - a list of ids for each role to be deleted
-
-        :param self: Represent the instance of the class
-        :param guild_id: int: Specify the guild that the roles are being deleted from
-        :param role_ids: list[int]: Specify the roles that are to be deleted
-        :return: An asynciterable of clientresponse objects or None
+        delete_roles function removes all roles with id in the list
+
+        :param guild_id: Specify the guild that the roles are being deleted from
+        :param role_ids: Specify the roles that are to be deleted
         """
 
         while len(role_ids):
             for user in self.users:
                 role_id: int = role_ids.pop(0)
                 response: ClientResponse = await user.delete_role(guild_id, role_id)
                 yield response
 
     async def delete_role(self, guild_id: int, role_id: int) -> Union[None, ClientResponse]:
         """
         The delete_role function deletes a role from the guild.
 
-        :param self: Refer to the current object
         :param guild_id: int: Specify the guild that you want to delete a role from
-        :param role_id: int: Specify the role to be deleted
-        :return: clientresponse object or None
+        :param role_id: int: Specify the role_id to be deleted
         """
 
         for user in self.users:
             response: ClientResponse = await user.delete_role(guild_id, role_id)
             if response.status == 204:
                 return response
 
     async def get_bans(self, guild_id: int) -> Union[None, ClientResponse]:
         """
         The get_bans function returns a list of banned users in the guild.
 
-
-        :param self: Represent the instance of the class
-        :param guild_id: int: Specify the guild id of the server you want to get banned users from
-        :return: A clientresponse object or None
+        :param guild_id: Specify the guild id of the server you want to get banned users from
         """
 
         for user in self.users:
             response: ClientResponse = await user.get_bans(guild_id)
             if response.status == 200:
                 return response
 
     async def ban_member(self, guild_id: int, user_id: int) -> Union[None, ClientResponse]:
         """
         The ban_member function is used to ban a member from the guild.
 
-        :param self: Represent the instance of the class
-        :param guild_id: int: Specify the guild that you want to ban a user from
-        :param user_id: int: Specify the user that is to be banned
-        :return: clientresponse object or None
+        :param guild_id: Specify the guild that you want to ban a user from
+        :param user_id: Specify the user that is to be banned
         """
 
         for user in self.users:
             response: ClientResponse = await user.ban_member(guild_id, user_id)
             if response.status == 204:
                 return response
 
@@ -240,35 +209,31 @@
         """
         The unban_members function is a coroutine that takes in a guild_id and user_ids list.
         It then iterates through the users list, popping off the first user id from the
         user_ids list and passing it to unban_member function of each client. If there is no
         response or if there was an error, it will return None. Otherwise, it will yield back
         the response.
 
-        :param self: Represent the instance of the class
-        :param guild_id: int: Specify the guild id of the server you want to unban members from
-        :param user_ids: list[int]: Store the list of user ids to unban
-        :return: A union of none or asynciterable[clientresponse]
+        :param guild_id: Specify the guild id of the server you want to unban members from
+        :param user_ids: Store the list of user ids to unban
         """
 
         while len(user_ids):
             for user in self.users:
                 user_id: int = user_ids.pop(0)
                 response: ClientResponse = await user.unban_member(guild_id, user_id)
                 if response.status == 204:
                     yield response
 
     async def unban_member(self, guild_id: int, user_id: int) -> Union[None, ClientResponse]:
         """
         The unban_member function unban a user from the guild.
 
-        :param self: Represent the instance of the class
-        :param guild_id: int: Specify the guild that you want to unban a member from
-        :param user_id: int: Specify the user id of the member to unban
-        :return: A clientresponse object or None
+        :param guild_id: Specify the guild that you want to unban a member from
+        :param user_id: Specify the user id of the member to unban
         """
 
         for user in self.users:
             response: ClientResponse = await user.unban_member(guild_id, user_id)
             if response.status == 204:
                 return response
 
@@ -276,67 +241,58 @@
 
         """
         The ban_members function is a coroutine that takes in a guild_id and user_ids list.
         It then iterates through the users list, popping off the first user id from the
         user_ids list and passing it to ban_member function of each client. The response
         from each client is yielded back to whatever called this function.
 
-        :param self: Represent the instance of the class
-        :param guild_id: int: Specify the guild to ban the user from
-        :param user_ids: list[int]: Store the list of user ids that will be banned
-        :return: A union of none or an asynciterable[clientresponse]
+        :param guild_id: Specify the guild to ban the user from
+        :param user_ids: Store the list of user ids that will be banned
         """
 
         while len(user_ids):
             for user in self.users:
                 user_id: int = user_ids.pop(0)
                 response: ClientResponse = await user.ban_member(guild_id, user_id)
                 yield response
 
     async def kick_member(self, guild_id: int, user_id: int) -> Union[None, ClientResponse]:
         """
         The kick_member function kicks a member from the guild.
 
-        :param self: Represent the instance of the class
-        :param guild_id: int: Specify the guild that you want to kick a user from
-        :param user_id: int: Identify the user to be kicked
-        :return: clientresponse object or None
+        :param guild_id: Specify the guild that you want to kick a user from
+        :param user_id: Identify the user to be kicked
         """
         for user in self.users:
             response: ClientResponse = await user.kick_member(guild_id, user_id)
             if response.status == 204:
                 return response
 
     async def kick_members(self, guild_id: int, user_ids: list[int]) -> Union[None, AsyncIterable[ClientResponse]]:
         """
-        The kick_member function kicks a member from the guild.
+        The kick_members function is a coroutine that takes in a guild_id and user_ids list.
+        It then iterates through the users list, popping off the first user id from the
+        user_ids list and kicking them from the specified guild. It yields each response as it goes.
 
-        :param self: Represent the instance of the class
-        :param guild_id: int: Specify the guild that you want to kick a user from
-        :param user_ids: list[int]: Identify the user to be kicked
-        :return: A union of none or an asynciterable[clientresponse]
+        :param guild_id: int: Specify which guild the user is in
+        :param user_ids: list[int]: list with id of people to kick out
         """
 
         while len(user_ids):
             for user in self.users:
                 user_id: int = user_ids.pop(0)
                 response: ClientResponse = await user.kick_member(guild_id, user_id)
                 yield response
 
     async def get_member(self, guild_id: int, user_id: int) -> Union[None, ClientResponse]:
         """
         The get_member function is used to get a member from the guild.
-            Parameters:
-                guild_id (int): The ID of the guild to get the member from.
-                user_id (int): The ID of the user to get as a member.
-
-        :param self: Access the class variables and methods
-        :param guild_id: int: Specify the guild that you want to get a member from
-        :param user_id: int: Specify the user id of the member you want to get
-        :return: A clientresponse object or None
+
+        :param guild_id: Specify the guild that you want to get a member from
+        :param user_id: Specify the user id of the member you want to get
         """
 
         for user in self.users:
             response: ClientResponse = await user.get_member(guild_id, user_id)
             if response.status == 200:
                 return response
 
@@ -344,20 +300,62 @@
                                                                 nickname: str = None,
                                                                 add_roles: list[int] = None,
                                                                 remove_roles: list[int] = None) -> Union[None, ClientResponse]:
 
         """
         The edit_member function allows you to edit a member of a guild.
 
-        :param self: Refer to the object itself
-        :param guild_id: int: Specify the guild that you want to edit a member in
-        :param user_id: int: Specify the user that you want to edit
-        :param nickname: str: Change the nickname of a user in a guild
-        :param add_roles: list[int]: Add roles to a user
-        :param remove_roles: list[int]: Remove roles from a user
-        :return: A clientresponse object or None
+        :param guild_id: Specify the guild that you want to edit a member in
+        :param user_id: Specify the user that you want to edit
+        :param nickname: Change the nickname of a user in a guild
+        :param add_roles: Add roles to a user
+        :param remove_roles: Remove roles from a user
         """
 
         for user in self.users:
             response: ClientResponse = await user.edit_member(guild_id, user_id, nickname, add_roles, remove_roles)
             if response and response.status == 200:
                 return response
+
+    async def add_reaction(self, channel_id: int, message_id: int, emoji: str) -> Union[None, AsyncIterable[ClientResponse]]:
+        """
+        The add_reaction function adds a reaction to the message with the given ID in the channel with
+        the given ID. The emoji parameter is a string that must be an emoticon. Example: \N{FIRE}
+
+        :param channel_id: Specify which channel_id the message is in
+        :param message_id: Message ID that you want to add a reaction to
+        :param emoji: A reaction to add to the message
+        """
+
+        for user in self.users:
+            response: ClientResponse = await user.add_reaction(channel_id, message_id, emoji)
+            yield response
+
+    async def get_reactions(self, channel_id: int, message_id: int, emoji: str) -> Union[None, ClientResponse]:
+        """
+        The get_reactions function returns a ClientResponse with
+        list of users that reacted with the specified emoji.
+
+        :param channel_id: Identify the channel that contains the message
+        :param message_id: Identify the message that is being reacted to
+        :param emoji: Specify the emoji to get reactions for
+        """
+
+        for user in self.users:
+            response: ClientResponse = await user.get_reactions(channel_id, message_id, emoji)
+            if response.status == 204:
+                return response
+
+    async def delete_reaction(self, channel_id: int, message_id: int, user_id: int, emoji: str) -> Union[None, ClientResponse]:
+        """
+        The delete_reaction function is used to delete a reaction from a message.
+
+        :param channel_id: int: Specify the channel where the message is located
+        :param message_id: int: Identify the message that you want to delete a reaction from
+        :param user_id: int: Specify the user whose reaction is to be deleted
+        :param emoji: str: Specify the emoji to be deleted
+        """
+
+        for user in self.users:
+            response: ClientResponse = await user.delete_reaction(channel_id, message_id, user_id, emoji)
+            if response.status == 204:
+                return response
```

### Comparing `selfbotclient-1.0.2/SelfBotClient/enums.py` & `selfbotclient-1.1.0/SelfBotClient/enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from enum import Enum
 
 
+__all__: tuple = ("ChannelType", "Permissions", "Discord")
+
+
 class Discord(Enum):
     ENDPOINT: str = "https://discord.com/api/v{}/"
 
 
 class ChannelType(Enum):
 
     TEXT_CHANNEL: int = 0
```

### Comparing `selfbotclient-1.0.2/SelfBotClient/errors.py` & `selfbotclient-1.1.0/SelfBotClient/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 __all__: tuple[str, ...] = (
     "UnSupportedApiVersion",
     "UnSupportedTokenType",
-    "SelfBotClientException",
     "InvalidMethodType"
 )
 
 
 class SelfBotClientException(Exception):
     pass
```

### Comparing `selfbotclient-1.0.2/SelfBotClient/http.py` & `selfbotclient-1.1.0/SelfBotClient/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 from .user import UserClient
 
 from typing import Union, Awaitable, Any
 from aiohttp import ClientSession, ClientResponse, client_exceptions
 from asyncio import AbstractEventLoop, sleep, get_event_loop
 
 
+__all__: tuple[str, ...] = ("HTTPClient", "ClientResponse")
+
+
 class CustomSession(ClientSession):
 
     def __init__(self, logger: Logger, *args: Any, **kwargs: Any):
         """
         The __init__ function is called when the class is instantiated.
         It sets up all of the variables that are needed for other functions to work properly.
         The super() function calls __init__ from the parent class, which in this case is ClientSession.
@@ -95,37 +98,34 @@
         """
 
         response = await super().get(url=url, allow_redirects=allow_redirects, **kwargs)
         return response
 
 
 class HTTPClient:
+    """
+    HTTPClient handles all requests related to the client.
+    It also has methods from checking tokens or creating a new session.
+
+    :param api_version: version of the discord api used by the client
+    :param loop: Set the event loop that will be used by the client
+    :param logger: Enable/disable the logger
+    :param request_latency: Control the rate of requests sent to discord
+    :param ratelimit_additional_cooldown: Add a cooldown to the ratelimit
+    """
 
     def __init__(
             self,
             api_version: API_VERSION,
             loop: AbstractEventLoop = None,
             logger: bool = True,
             request_latency: float = 0.1,
             ratelimit_additional_cooldown: float = 10
 
     ):
-        """
-        The __init__ function is called when the class is instantiated.
-        It allows the class to initialize its attributes, and do any other necessary setup.
-        The __init__ function can accept arguments, which will be passed on from the object creation.
-
-        :param self: Represent the instance of the class
-        :param api_version: API_VERSION: Set the api version of discord
-        :param loop: AbstractEventLoop: Set the event loop that will be used by the client
-        :param logger: bool: Enable/disable the logger
-        :param request_latency: float: Control the rate of requests sent to discord
-        :param ratelimit_additional_cooldown: float: Add a cooldown to the ratelimit
-        :return: Nothing, so the return type is none
-        """
 
         if api_version not in (9, 10):
             raise UnSupportedApiVersion
 
         self.request_latency: float = request_latency
         self.ratelimit_additional_cooldown: float = ratelimit_additional_cooldown
 
@@ -178,15 +178,15 @@
                     if self._logger_status:
                         self.logger.warning(
                             f"An invalid token has been provided: {self._tokens} | The token will be automatically deleted")
                 else:
                     data = await response.json()
                     data["token"] = self._tokens
                     data["endpoint"] = self.endpoint
-                    self.users.append(UserClient(data, self.session, self.loop))
+                    self.users.append(UserClient(data, self.session))
 
                     self._tokens = [self._tokens]
 
             elif _type == list:
                 for token in self._tokens:
 
                     header: AUTH_HEADER = AUTH_HEADER(authorization=token)
@@ -197,18 +197,18 @@
                                 f"An invalid token has been provided: {token} | The token will be automatically deleted")
 
                     else:
                         data = await response.json()
                         data["token"] = token
                         data["endpoint"] = self.endpoint
 
-                        self.users.append(UserClient(data, self.session, self.loop))
+                        self.users.append(UserClient(data, self.session))
 
             if self._logger_status:
-                self.logger.info(f"Checking of tokens successfully completed | Loaded ({len(self.users)}) tokens")
+                self.logger.info(f"Checking of tokens successfully completed | Loaded ({len(self.users)}) tokens\n")
 
         if not isinstance(self._tokens, list) and not isinstance(self._tokens, str):
             raise UnSupportedTokenType
 
         self.loop.run_until_complete(_check(type(self._tokens)))
 
     def __del__(self) -> None:
```

### Comparing `selfbotclient-1.0.2/SelfBotClient/logger.py` & `selfbotclient-1.1.0/SelfBotClient/logger.py`

 * *Files identical despite different names*

### Comparing `selfbotclient-1.0.2/SelfBotClient/user.py` & `selfbotclient-1.1.0/SelfBotClient/user.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,36 +6,30 @@
     from .http import CustomSession
 
 from .typings import AUTH_HEADER, RGB_COLOR
 from .logger import Logger
 from .enums import ChannelType
 from .permissionbuilder import PermissionBuilder
 
+from urllib.parse import quote
 from asyncio import AbstractEventLoop
 from aiohttp import ClientResponse
 from logging import getLogger
 
 
 class UserClient:
+    """
+    :class:`UserClient` Is the class responsible for the user account.
 
-    def __init__(self, data: dict, session: CustomSession, loop: AbstractEventLoop):
-        """
-        The __init__ function is called when the class is instantiated.
-        It sets up all of the variables that are needed for other functions to work properly.
-
-
-        :param self: Represent the instance of the class
-        :param data: dict: Store the data that is passed into the class
-        :param session: CustomSession: Pass the session to the class
-        :param loop: AbstractEventLoop: Create a new event loop
-        :return: None
-        """
+    :param data: Dict with account data - such as token, name, id.
+    :param session: Session to send requests in methods
+    """
 
+    def __init__(self, data: dict, session: CustomSession):
         self._session: CustomSession = session
-        self._loop: AbstractEventLoop = loop
         self._logger: Logger = getLogger("Logger")
 
         self.data: dict = data
         self._endpoint: str = self.data.get("endpoint")
         self.token: str = self.data.get("token")
         self.name: str = self.data.get("username")
         self.discriminator: str = f"#{self.data.get('discriminator')}"
@@ -48,18 +42,16 @@
     def __repr__(self):
         return f"<UserClient(name={self.name}, discriminator={self.discriminator}, id={self.id})>"
 
     async def send_message(self, channel_id: int, message_content: str) -> ClientResponse:
         """
         The send_message function sends a message to the specified channel.
 
-        :param self: Represent the instance of the class
-        :param channel_id: int: Specify the channel that you want to send a message to
-        :param message_content: str: Send a message to the channel
-        :return: A clientresponse object
+        :param channel_id: Specify the channel to send the message to
+        :param message_content: content of the message
         """
 
         _url = self._endpoint + f"channels/{channel_id}/messages"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: POST -> {_url}")
 
@@ -74,21 +66,17 @@
             self._logger.warning(
                 f"Request POST channels/{channel_id}/messages failed.\n -> {self} {await response.json()}")
 
         return response
 
     async def delete_channel(self, channel_id: int) -> ClientResponse:
         """
-        The delete_channel function deletes a channel.
-            Parameters:
-                channel_id (int): The ID of the channel to delete.
-
-        :param self: Access the class attributes and methods
-        :param channel_id: int: Specify which channel to delete
-        :return: A clientresponse object
+        The delete_channel function deletes a channel from the server.
+
+        :param channel_id: Specify the channel that is to be deleted
         """
 
         _url = self._endpoint + f"channels/{channel_id}"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: DELETE -> {_url}")
 
@@ -100,25 +88,23 @@
                 f"Request DELETE channels/{channel_id} failed.\n -> {self} {await response.json()}")
 
         return response
 
     async def create_channel(self, guild_id: int, name: str, channel_type: ChannelType,
                              topic: str = None, user_limit: int = None, position: int = None, nsfw: bool = False) -> ClientResponse:
         """
-        The create_channel function creates a new channel in the specified guild.
+        The create_channel function creates a channel in the specified guild.
 
-        :param self: Refer to the current instance of a class
-        :param guild_id: int: Specify the server that you want to create a channel in
-        :param name: str: Set the name of the channel
-        :param channel_type: ChannelType: Specify the type of channel that is being created
-        :param topic: str: Set the topic of the channel
-        :param user_limit: int: Set the maximum number of users that can be in a voice channel
-        :param position: int: Set the position of the channel in the server
-        :param nsfw: bool: Determine if the channel is nsfw or not
-        :return: A clientresponse object
+        :param guild_id: Specify the guild id of the server you want to create a channel in
+        :param name: Specify the name of the channel
+        :param channel_type: Specify what type of channel you want to create
+        :param topic: Set the topic of the channel
+        :param user_limit: Set the maximum number of users allowed in a voice channel
+        :param position: Set the position of the channel in the list
+        :param nsfw: Determine whether the channel is nsfw or not
         """
 
         _url = self._endpoint + f"guilds/{guild_id}/channels"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: POST -> {_url}")
 
@@ -138,21 +124,18 @@
             self._logger.error(
                 f"Request POST /guilds/{guild_id}/channels failed.\n -> {self} {await response.json()}")
 
         return response
 
     async def get_channels(self, guild_id: int) -> ClientResponse:
         """
-        The get_channels function returns a list of channel objects for the guild.
-            Args:
-                guild_id (int): The id of the server to get channels from.
-
-        :param self: Represent the instance of the class
-        :param guild_id: int: Get the channels of a specific guild
-        :return: A clientresponse object
+        The get_channels function is a coroutine that takes in a guild_id and returns an ClientResponse object.
+        The function can return the data of all channels on the server
+
+        :param guild_id: Specify the guild id of the server you want to get channels from
         """
 
         _url = self._endpoint + f"guilds/{guild_id}/channels"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: GET -> {_url}")
 
@@ -169,23 +152,21 @@
                                 guild_id: int,
                                 name: str,
                                 color: RGB_COLOR = None,
                                 hoist: bool = False,
                                 permissions: PermissionBuilder = None) -> ClientResponse:
 
         """
-        The create_role function creates a new role in the specified guild.
+        The create_role function creates a role in the specified guild.
 
-        :param self: Represent the instance of the class
-        :param guild_id: int: Specify the server you want to create a role in
-        :param name: str: Set the name of the role
-        :param color: RGB_COLOR: Set the color of the role
-        :param hoist: bool: Determine if the role should be displayed separately in the user list
-        :param permissions: PermissionBuilder: Set the permissions of the role
-        :return: A clientresponse object
+        :param guild_id: Specify the guild in which you want to create a role
+        :param name: Set the name of the role
+        :param color: Set the color of the role
+        :param hoist: Determine whether the role should be displayed separately in the user list
+        :param permissions: Set the permissions for the role
         """
 
         _url = self._endpoint + f"guilds/{guild_id}/roles"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: POST -> {_url}")
 
@@ -214,21 +195,17 @@
             self._logger.error(
                 f"Request POST guilds/{guild_id}/roles failed.\n -> {self} {await response.json()}")
 
         return response
 
     async def get_roles(self, guild_id: int) -> ClientResponse:
         """
-        The get_roles function returns a list of roles for the specified guild.
-            Parameters:
-                guild_id (int): The ID of the guild to get roles from.
-
-        :param self: Represent the instance of the class
-        :param guild_id: int: Specify which guild you want to get the roles from
-        :return: A clientresponse object
+        get_roles returns a list of data with all the roles on the server
+
+        :param guild_id: Specify the guild id of the server you want to get roles from
         """
 
         _url = self._endpoint + f"guilds/{guild_id}/roles"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: GET -> {_url}")
 
@@ -241,18 +218,16 @@
 
         return response
 
     async def delete_role(self, guild_id: int, role_id: int) -> ClientResponse:
         """
         The delete_role function deletes a role from the guild.
 
-        :param self: Represent the instance of the class
-        :param guild_id: int: Specify the guild id of the role you want to delete
-        :param role_id: int: Specify which role to delete
-        :return: A clientresponse object
+        :param guild_id: int: Specify the guild that you want to delete a role from
+        :param role_id: int: Specify the role_id to be deleted
         """
 
         _url = self._endpoint + f"guilds/{guild_id}/roles/{role_id}"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: DELETE -> {_url}")
 
@@ -262,14 +237,20 @@
         if response.status not in (204, 429) and self._logger._status:
             self._logger.error(
                 f"Request DELETE guilds/{guild_id}/roles/{role_id} failed.\n -> {self} {await response.json()}")
 
         return response
 
     async def get_bans(self, guild_id: int) -> ClientResponse:
+        """
+        The get_bans function returns a list of banned users in the guild.
+
+        :param guild_id: Specify the guild id of the server you want to get banned users from
+
+        """
         _url = self._endpoint + f"guilds/{guild_id}/bans"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: GET -> {_url}")
 
         response: ClientResponse = await self._session.request(
             method="GET", url=_url, headers=self._auth_header)
@@ -278,20 +259,18 @@
             self._logger.error(
                 f"Request GET guilds/{guild_id}/bans failed.\n -> {self} {await response.json()}")
 
         return response
 
     async def unban_member(self, guild_id: int, user_id: int) -> ClientResponse:
         """
-        The unban_member function is used to unban a member from the guild.
+        The unban_member function unban a user from the guild.
 
-        :param self: Represent the instance of the class
-        :param guild_id: int: Specify the guild that you want to unban a member from
-        :param user_id: int: Specify the user id of the member that you want to unban
-        :return: A clientresponse object
+        :param guild_id: Specify the guild that you want to unban a member from
+        :param user_id: Specify the user id of the member to unban
         """
 
         _url = self._endpoint + f"guilds/{guild_id}/bans/{user_id}"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: DELETE -> {_url}")
 
@@ -304,18 +283,16 @@
 
         return response
 
     async def ban_member(self, guild_id: int, user_id: int) -> ClientResponse:
         """
         The ban_member function is used to ban a member from the guild.
 
-        :param self: Represent the instance of the class
-        :param guild_id: int: Specify the guild id of the server you want to ban a member from
-        :param user_id: int: Specify the user id of the person you want to ban
-        :return: A clientresponse object
+        :param guild_id: Specify the guild that you want to ban a user from
+        :param user_id: Specify the user that is to be banned
         """
 
         _url = self._endpoint + f"guilds/{guild_id}/bans/{user_id}"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: PUT -> {_url}")
 
@@ -326,20 +303,18 @@
             self._logger.error(
                 f"Request PUT guilds/{guild_id}/bans/{user_id} failed.\n -> {self} {await response.json()}")
 
         return response
 
     async def kick_member(self, guild_id: int, user_id: int) -> ClientResponse:
         """
-        The kick_member function is used to kick a member from the guild.
+        The kick_member function kicks a member from the guild.
 
-        :param self: Represent the instance of the class
-        :param guild_id: int: The ID of the guild you want to kick a member from.
-        :param user_id: int: The ID of the user you want to kick.
-        :return: A clientresponse object
+        :param guild_id: Specify the guild that you want to kick a user from
+        :param user_id: Identify the user to be kicked
         """
 
         _url = self._endpoint + f"guilds/{guild_id}/members/{user_id}"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: DELETE -> {_url}")
 
@@ -350,20 +325,18 @@
             self._logger.error(
                 f"Request DELETE guilds/{guild_id}/members/{user_id} failed.\n -> {self} {await response.json()}")
 
         return response
 
     async def get_member(self, guild_id: int, user_id: int) -> ClientResponse:
         """
-        The get_member function is used to get a member of the guild.
+        The get_member function is used to get a member from the guild.
 
-        :param self: Access the class attributes and methods
-        :param guild_id: int: Specify the guild id of the server you want to get a member from
-        :param user_id: int: Get the user's id
-        :return: A clientresponse object
+        :param guild_id: Specify the guild that you want to get a member from
+        :param user_id: Specify the user id of the member you want to get
         """
 
         _url = self._endpoint + f"guilds/{guild_id}/members/{user_id}"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: GET -> {_url}")
 
@@ -378,23 +351,21 @@
 
     async def edit_member(self, guild_id: int, user_id: int,
                           nickname: str = None,
                           add_roles: list[int] = None,
                           remove_roles: list[int] = None) -> ClientResponse:
 
         """
-        The edit_member function allows you to edit a member of the guild.
+        The edit_member function allows you to edit a member of a guild.
 
-        :param self: Represent the instance of the class
-        :param guild_id: int: Specify the guild id of the server you want to edit
-        :param user_id: int: Specify the user to edit
-        :param nickname: str: Set the nickname of a member
-        :param add_roles: list[int]: Add roles to a user
-        :param remove_roles: list[int]: Remove roles from a user
-        :return: A clientresponse object or None
+        :param guild_id: Specify the guild that you want to edit a member in
+        :param user_id: Specify the user that you want to edit
+        :param nickname: Change the nickname of a user in a guild
+        :param add_roles: Add roles to a user
+        :param remove_roles: Remove roles from a user
         """
 
         json: dict = {}
 
         if add_roles or remove_roles:
             user_response: ClientResponse = await self.get_member(guild_id, user_id)
             user_data: dict = await user_response.json()
@@ -427,7 +398,86 @@
 
         if response.status not in (200, 429) and self._logger._status:
             self._logger.error(
                 f"Request PATCH guilds/{guild_id}/members/{user_id} failed.\n -> {self} {await response.json()}")
 
         return response
 
+    async def add_reaction(self, channel_id: int, message_id: int, emoji: str) -> ClientResponse:
+        """
+        The add_reaction function adds a reaction to the message with the given ID in the channel with
+        the given ID. The emoji parameter is a string that must be an emoticon. Example: \N{FIRE}
+
+        :param channel_id: Specify which channel_id the message is in
+        :param message_id: Message ID that you want to add a reaction to
+        :param emoji: A reaction to add to the message
+        """
+
+        emoji = quote(emoji)
+
+        _url = self._endpoint + f"channels/{channel_id}/messages/{message_id}/reactions/{emoji}/@me"
+
+        if self._logger._status:
+            self._logger.debug(f"Sending request: PUT -> {_url}")
+
+        response: ClientResponse = await self._session.request(
+            method="PUT", url=_url, headers=self._auth_header)
+
+        if response.status not in (204, 429) and self._logger._status:
+            self._logger.error(
+                f"Request PUT channels/{channel_id}/messages/{message_id}/reactions/{emoji}/@me failed.\n -> {self} {await response.json()}")
+
+        return response
+
+    async def get_reactions(self, channel_id: int, message_id: int, emoji: str) -> ClientResponse:
+        """
+        The get_reactions function returns a ClientResponse with
+        list of users that reacted with the specified emoji.
+
+        :param channel_id: Identify the channel that contains the message
+        :param message_id: Identify the message that is being reacted to
+        :param emoji: Specify the emoji to get reactions for
+        """
+
+        emoji = quote(emoji)
+
+        _url = self._endpoint + f"channels/{channel_id}/messages/{message_id}/reactions/{emoji}"
+
+        if self._logger._status:
+            self._logger.debug(f"Sending request: GET -> {_url}")
+
+        response: ClientResponse = await self._session.request(
+            method="GET", url=_url, headers=self._auth_header)
+
+        if response.status not in (200, 429) and self._logger._status:
+            self._logger.error(
+                f"Request GET channels/{channel_id}/messages/{message_id}/reactions/{emoji}/ failed.\n -> {self} {await response.json()}")
+
+        return response
+
+    async def delete_reaction(self, channel_id: int, message_id: int, user_id: int, emoji: str) -> ClientResponse:
+        """
+        The delete_reaction function is used to delete a reaction from a message.
+
+        :param channel_id: int: Specify the channel where the message is located
+        :param message_id: int: Identify the message that you want to delete a reaction from
+        :param user_id: int: Specify the user whose reaction is to be deleted
+        :param emoji: str: Specify the emoji to be deleted
+        """
+
+        emoji = quote(emoji)
+
+        _url = self._endpoint + f"channels/{channel_id}/messages/{message_id}/reactions/{emoji}/{user_id}"
+
+        if self._logger._status:
+            self._logger.debug(f"Sending request: DELETE -> {_url}")
+
+        response: ClientResponse = await self._session.request(
+            method="DELETE", url=_url, headers=self._auth_header)
+
+        if response.status not in (204, 429) and self._logger._status:
+            self._logger.error(
+                f"Request DELETE channels/{channel_id}/messages/{message_id}/reactions/{emoji}/{user_id} failed.\n -> {self} {await response.json()}")
+
+        return response
+
+
```

### Comparing `selfbotclient-1.0.2/setup.py` & `selfbotclient-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.2'
+VERSION = '1.1.0'
 DESCRIPTION = 'Library that will allow you to manage selfbots'
 LONG_DESCRIPTION = 'The library logs into your account thanks to the entered tokens and can manage them. ' \
                    'such as sending messages, deleting roles, etc.'
 
 # Setting up
 setup(
     name="selfbotclient",
```

