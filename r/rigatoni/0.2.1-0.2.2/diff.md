# Comparing `tmp/rigatoni-0.2.1.tar.gz` & `tmp/rigatoni-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rigatoni-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rigatoni-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rigatoni-0.2.1.tar` & `rigatoni-0.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     6513 2023-06-14 13:35:53.350039 rigatoni-0.2.1/README.md
--rw-r--r--   0        0        0      780 2023-06-14 13:35:53.350039 rigatoni-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      930 2023-06-14 13:35:53.350039 rigatoni-0.2.1/rigatoni/__init__.py
--rw-r--r--   0        0        0    31886 2023-06-14 13:35:53.350039 rigatoni-0.2.1/rigatoni/core.py
--rw-r--r--   0        0        0      522 2023-06-14 13:35:53.350039 rigatoni-0.2.1/rigatoni/geometry/__init__.py
--rw-r--r--   0        0        0     4261 2023-06-14 13:35:53.350039 rigatoni-0.2.1/rigatoni/geometry/byte_server.py
--rw-r--r--   0        0        0    23849 2023-06-14 13:35:53.350039 rigatoni-0.2.1/rigatoni/geometry/geometry_creation.py
--rw-r--r--   0        0        0      836 2023-06-14 13:35:53.350039 rigatoni-0.2.1/rigatoni/geometry/geometry_objects.py
--rw-r--r--   0        0        0    15605 2023-06-14 13:35:53.350039 rigatoni-0.2.1/rigatoni/noodle_objects.py
--rw-r--r--   0        0        0     7363 1970-01-01 00:00:00.000000 rigatoni-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1905 2023-06-15 00:16:12.422002 rigatoni-0.2.2/README.md
+-rw-r--r--   0        0        0      780 2023-06-15 00:16:12.422002 rigatoni-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      930 2023-06-15 00:16:12.426002 rigatoni-0.2.2/rigatoni/__init__.py
+-rw-r--r--   0        0        0    41908 2023-06-15 00:16:12.426002 rigatoni-0.2.2/rigatoni/core.py
+-rw-r--r--   0        0        0      522 2023-06-15 00:16:12.426002 rigatoni-0.2.2/rigatoni/geometry/__init__.py
+-rw-r--r--   0        0        0     4452 2023-06-15 00:16:12.426002 rigatoni-0.2.2/rigatoni/geometry/byte_server.py
+-rw-r--r--   0        0        0    24399 2023-06-15 00:16:12.426002 rigatoni-0.2.2/rigatoni/geometry/geometry_creation.py
+-rw-r--r--   0        0        0      837 2023-06-15 00:16:12.426002 rigatoni-0.2.2/rigatoni/geometry/geometry_objects.py
+-rw-r--r--   0        0        0    20787 2023-06-15 00:16:12.426002 rigatoni-0.2.2/rigatoni/noodle_objects.py
+-rw-r--r--   0        0        0     2755 1970-01-01 00:00:00.000000 rigatoni-0.2.2/PKG-INFO
```

### Comparing `rigatoni-0.2.1/pyproject.toml` & `rigatoni-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.1/rigatoni/__init__.py` & `rigatoni-0.2.2/rigatoni/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         geometry_objects.py
     delegates.py
     noodle_objects.py
     server.py
 """
 
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 from .core import Server
 from .noodle_objects import *
 
 # Ensure that dependencies are installed for optional module
 try:
     import numpy
```

### Comparing `rigatoni-0.2.1/rigatoni/core.py` & `rigatoni-0.2.2/rigatoni/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Module with core implementation of Server Object"""
 
 from __future__ import annotations
-from typing import Type, TypeVar, Literal
+from typing import Type, TypeVar, Literal, Union
 import asyncio
 import functools
 import logging
 import threading
 
 import websockets
 from cbor2 import loads, dumps
@@ -19,30 +19,49 @@
 
 
 def default_json_encoder(value):
     return str(value)
 
 
 class Server(object):
-    """NOODLES Server
+    """Overarching object for managing the state of a NOODLES session
+
+    Handles communication and multiple client connections. The server provides several
+    methods for interacting with and creating delegates. These are especially useful for
+    defining custom methods that the server will expose to clients.
     
-    Attributes;
-        clients (set): client connections
-        custom_delegates (dict): 
-            maps noodle object to its delegate class, empty by default
-        delegates (dict):
-            maps component ID to its delegate instance
+    Attributes:
+        port (int):
+            port server is running on
+        clients (set):
+            client connections
         ids (dict): 
             maps object type to slot tracking info (next_slot, on_deck)
-        components (dict):
+        state (dict):
             document's current state, contains all components with component ID as the key
+        client_state (dict):
+            lagging state to keep track of how up to date clients are
         references (dict):
             maps component ID to all the component ID's that reference it
         delete_queue (set):
             components that are referenced but have been requested to be deleted
+        ready (threading.Event):
+            event to signal when server is ready to accept connections
+        shutdown_event (asyncio.Event):
+            event to signal when server is shutting down
+        thread (threading.Thread):
+            thread server is running on if using context manager
+        json_output (str):
+            path to json file to output message logs
+        custom_delegates (dict):
+            maps component type to delegate class
+        id_map (dict):
+            maps component type to ID type
+        id_decoder (dict):
+            maps ID type to base component type, useful for getting base class from ID
         message_map (dict):
             maps action and type to message ID
     """
 
     def __init__(self, port: int, starting_state: list[StartingComponent],
                  delegate_map: dict[Type[Delegate], Type[Delegate]] = None, json_output: str = None):
         """Constructor
@@ -53,15 +72,16 @@
             starting_state (list[StartingComponent]):
                 list of objects containing the info to create components on initialization
             delegate_map (dict):
                 maps noodles component type to instance of delegate class
             json_output (str):
                 path to json file to output message logs
         Raises:
-            Exception: Invalid Arguments or Method Not Specified when filling in starting state
+            TypeError: invalid arguments to create starting component
+            ValueError: no method specified for method starting component
         """
 
         self.port = port
         self.clients = set()
         self.ids = {}
         self.state = {}
         self.client_state = {}
@@ -149,59 +169,62 @@
 
     def __exit__(self, exc_type, exc_value, traceback):
         """Exit context manager"""
         self.shutdown()
         self.thread.join()
 
     def run(self):
-        """Run the server"""
-        return asyncio.run(self.start_server())
+        """Run the server
+
+        This will run indefinitely until the server is shutdown"""
+        return asyncio.run(self._start_server())
 
-    async def start_server(self):
+    async def _start_server(self):
         """Run the server and listen for connections"""
+
         # Create partial to pass server to handler
-        handler = functools.partial(self.handle_client)
+        handler = functools.partial(self._handle_client)
 
         logging.info("Starting up Server...")
         async with websockets.serve(handler, "", self.port):
             self.ready.set()
             while not self.shutdown_event.is_set():
                 await asyncio.sleep(.1)
 
     def shutdown(self):
-        """Shutdown the server"""
+        """Shuts down the server and closes off communication with clients"""
         logging.info("Shutting down server...")
         self.shutdown_event.set()
 
-    def log_json(self, message: list):
+    def _log_json(self, message: list):
         json_message = json.dumps(message, default=default_json_encoder)
         formatted_message = f"{json_message}\n"
         with open(self.json_output, "a") as outfile:
             outfile.write(formatted_message)
 
-    async def send(self, websocket, message: list):
+    async def _send(self, websocket, message: list):
         """Send CBOR message using websocket
 
         Args:
             websocket (WebSocketClientProtocol):
                 recipient of this data
             message (list):
                 message to be sent, in list format
                 [id, content, id, content...]
         """
 
         # Log message in json file if applicable
         if self.json_output:
-            self.log_json(message)
+            self._log_json(message)
 
         # Log message and send
         logging.debug(f"Sending Message: ID's {message[::2]}")
         await websocket.send(dumps(message))
 
-    async def handle_client(self, websocket):
+    async def _handle_client(self, websocket):
         """Coroutine for handling a client's connection
 
         Receives and delegates message handling to server
 
         args:
             websocket (WebSocketClientProtocol):
                 client connection being handled
@@ -214,80 +237,116 @@
 
         # Handle intro and update client
         raw_intro_msg = await websocket.recv()
         intro_msg = loads(raw_intro_msg)
         client_name = intro_msg[1]["client_name"]
         logging.info(f"Client '{client_name}' Connecting...")
 
-        init_message = self.handle_intro()
-        await self.send(websocket, init_message)
+        init_message = self._handle_intro()
+        await self._send(websocket, init_message)
 
         # Listen for method invocation and keep all clients informed
         async for message in websocket:
             # Decode and log raw message
             message = loads(message)
             logging.debug(f"Message from client: {message}")
 
             # Handle the method invocation
-            reply = self.handle_invoke(message[1])
+            reply = self._handle_invoke(message[1])
 
             # Send method reply to client
-            await self.send(websocket, list(reply))
+            await self._send(websocket, list(reply))
 
         # Remove client if disconnected
         logging.debug(f"Client 'client_name' disconnected")
         self.clients.remove(websocket)
 
     def get_ids_by_type(self, component: Type[Delegate]) -> list:
-        """Helper to get all ids for certain component type
+        """Get all ids for certain component type
         
         Args:
             component (type): type of component to get ID's for
+
+        Returns:
+            ids: list of ids for components of specified type
         """
 
         return [key for key, val in self.state.items() if isinstance(val, component)]
 
     def get_delegate_id(self, name: str):
-        """Helper to get a component with a type and name"""
+        """Get a component by using its name
+
+        Args:
+            name (str): name of component to get
+
+        Returns:
+            id: id of component with specified name
+
+        Raises:
+            ValueError: if no component with specified name is found
+        """
 
         for delegate in self.state.values():
             if delegate.name == name:
                 return delegate.id
         raise ValueError("No Component Found")
 
     def get_delegate(self, identifier: Union[ID, str, Dict[str, ID]]):
-        """Getter for users to access components in state
+        """Access components in state
 
         Can be called with an ID, name, or context of the delegate
+
+        Args:
+            identifier (Union[ID, str, Dict[str, ID]]): identifier for component
+
+        Returns:
+            delegate: delegate with specified identifier
+
+        Raises:
+            TypeError: if identifier is not of type ID, str, or dict
+            ValueError: if no component with specified identifier is found or context is invalid
         """
         if isinstance(identifier, ID):
             return self.state[identifier]
         elif isinstance(identifier, str):
             return self.state[self.get_delegate_id(identifier)]
         elif isinstance(identifier, dict):
             return self.get_delegate_by_context(identifier)
         else:
             raise TypeError(f"Invalid type for identifier: {type(identifier)}")
 
     def get_delegate_by_context(self, context: dict):
-        """Helper to get a component by context"""
+        """Get a component using a context object
+
+        This is especially useful in methods that are invoked in a certain context. Note contexts
+        are only used when working with entities, tables, and plots.
+
+        Args:
+            context (dict): context of the form {str: ID}
+
+        Returns:
+            delegate: delegate from specified context
+
+        Raises:
+            ValueError: if context is invalid
+        """
 
         entity = context.get("entity")
         table = context.get("table")
         plot = context.get("plot")
         if entity:
             return self.get_delegate(EntityID(*entity))
         elif table:
             return self.get_delegate(TableID(*table))
         elif plot:
             return self.get_delegate(PlotID(*plot))
         else:
             raise ValueError(f"Invalid context: {context}")
 
-    def get_message_contents(self, action: str, noodle_object: NoodleObject, delta: set[str] = None):
+    def _get_message_contents(self, action: str, noodle_object: NoodleObject, delta: set[str] = None):
         """Helper to handle construction of message dict
         
         Args:
             action (str): action taken with message
             noodle_object (NoodleObject): Delegate, Reply, or Invoke object
             delta (set): field names to be included in update
         """
@@ -323,89 +382,89 @@
             try:
                 contents["id"] = noodle_object.id
             except AttributeError:
                 raise Exception(f"Cannot delete a {noodle_object}")
 
         return contents
 
-    def prepare_message(self, action: str, noodle_object: NoodleObject = None, delta: set[str] = None):
+    def _prepare_message(self, action: str, noodle_object: NoodleObject = None, delta: set[str] = None):
         """Given object and action, get id and message contents as dict
 
         Args:
             action (str): action taken with message
             noodle_object (NoodleObject): Component, Reply, or Invoke object
             delta (set): field names to be included in update
         """
 
         delegate_type = None if not isinstance(noodle_object, Delegate) else type(noodle_object.id)
         key = (action, delegate_type)
         message_id = self.message_map[key]
-        contents = self.get_message_contents(action, noodle_object, delta)
+        contents = self._get_message_contents(action, noodle_object, delta)
 
         return message_id, contents
 
     def broadcast(self, message: list):
         """Broadcast message to all connected clients
         
         Args:
             message [tuple]: fully constructed message in form (tag/id, contents)
         """
 
         # Log message in json file if applicable
         if self.json_output:
-            self.log_json(message)
+            self._log_json(message)
 
         logging.debug(f"Broadcasting Message: ID's {message[::2]}")
         encoded = dumps(message)
         websockets.broadcast(self.clients, encoded)
 
-    def handle_intro(self):
+    def _handle_intro(self):
         """Formulate response for new client"""
 
         # Add create message for every object in state
         message = []
         ordered_components = order_components(self.state, self.references)
         for component in ordered_components:
-            msg_id, content = self.prepare_message("create", component)
+            msg_id, content = self._prepare_message("create", component)
             message.extend([msg_id, content])
 
         # Add document update
-        message.extend(self.prepare_message("update", None))
+        message.extend(self._prepare_message("update", None))
 
         # Finish with initialization message
-        message.extend(self.prepare_message("initialized"))
+        message.extend(self._prepare_message("initialized"))
         return message
 
-    def handle_invoke(self, message: dict):
+    def _handle_invoke(self, message: dict):
         """Handle all invokes coming from the client
         
         Take message and formulate response for clients. Tries to invoke and
         raises appropriate error codes if unsuccessful. Note that the method 
         technically doesn't raise any exceptions, instead the exception is 
         captured in a message and sent to the client.
         
         Args:
             message (dict): dict form of message from client
         """
 
         # Create generic reply with invalid invoke ID and attempt invoke
         reply_obj = Reply(invoke_id="-1")
         try:
-            self.invoke_method(message, reply_obj)
+            self._invoke_method(message, reply_obj)
 
         except Exception as e:
             if type(e) is MethodException:
                 reply_obj.method_exception = e
             else:
                 logging.error(f"\033[91mServerside Error: {e}\033[0m")
                 reply_obj.method_exception = MethodException(code=-32603, message="Internal Error")
 
-        return self.prepare_message("reply", reply_obj)
+        return self._prepare_message("reply", reply_obj)
 
-    def invoke_method(self, message: dict, reply: Reply):
+    def _invoke_method(self, message: dict, reply: Reply):
         """Invoke method and build out reply object
         
         Mostly a helper for handle_invoke to raise proper method exceptions
 
         Args:
             message (dict): Invoke message in dict form
             reply (Reply): Practically empty reply object to be updated 
@@ -427,15 +486,15 @@
             method = getattr(self, method_name)
         except Exception:
             raise MethodException(code=-32601, message="Method Not Found")
 
         # Invoke
         reply.result = method(context, *args)
 
-    def update_references(self, parent_delegate: Delegate, current: NoodleObject, removing=False):
+    def _update_references(self, parent_delegate: Delegate, current: NoodleObject, removing=False):
         """Update in-degree for all objects referenced by this one
 
         Recursively updates references for all components under a parent one. Here,
         the current object changes through the recursion while comp keeps track of 
         the parent. Essentially finds all the objects that delegate points to
         
         Args:
@@ -451,33 +510,33 @@
                 if removing:
                     self.references[val].remove(parent_delegate.id)
                 else:
                     self.references.setdefault(val, set()).add(parent_delegate.id)
 
             # Found another object to recurse on
             elif isinstance(val, NoodleObject):
-                self.update_references(parent_delegate, val, removing)
+                self._update_references(parent_delegate, val, removing)
 
             # Found list of objects or id's to recurse on 
             elif val is not None and isinstance(val, list):
 
                 # Objects
                 if len(val) > 0 and isinstance(val[0], NoodleObject):
                     for obj in val:
-                        self.update_references(parent_delegate, obj, removing)
+                        self._update_references(parent_delegate, obj, removing)
 
                 # ID's
                 elif len(val) > 0 and isinstance(val[0], ID):
                     for id in val:
                         if removing:
                             self.references[id].remove(parent_delegate.id)
                         else:
                             self.references.setdefault(id, set()).add(parent_delegate.id)
 
-    def get_id(self, delegate_type: Type[Delegate]) -> ID:
+    def _get_id(self, delegate_type: Type[Delegate]) -> ID:
         """Get next open ID
         
         Check for open slots then take the closest available slot
 
         Args:
             delegate_type (Type): type for desired ID
         """
@@ -501,72 +560,84 @@
     # Interface methods to build server methods ===============================================
 
     def create_component(self, comp_type: Type[T], **kwargs) -> T:
         """Officially create new component in state
         
         This method updates state, updates references, and broadcasts msg to clients.
         It also handles the acquisition of a valid ID. This is a general creator method, but
-        more specific versions exist for each component type
+        more specific versions exist for each component type. Keyword arguments should be
+        used for specifying the attributes of the component. Any deviation from the spec will
+        raise a validation exception. Note that since this method
+        handles the ID, it should not be specified as one of the keyword arguments.
         
         Args:
             comp_type (Component Type): type of component to be created
             **kwargs: the user should specify the attributes of the component using 
                 keyword arguments. Refer to the noodle objects to see which attributes
                 are required and optional. Any deviation from the spec will raise a 
                 validation exception. Note that since this method handles the ID, it 
                 should not be specified as one of the keyword arguments.
+
+        Returns:
+            Delegate: delegate for the newly created component
+
+        Raises:
+            ValueError: if the user specifies an invalid attribute for the component
         """
 
         # Get ID and try to create delegate from args
         comp_type = self.custom_delegates.get(comp_type, comp_type)
-        comp_id = self.get_id(comp_type)
+        comp_id = self._get_id(comp_type)
         try:
             new_delegate = comp_type(server=self, id=comp_id, **kwargs)
         except Exception as e:
-            raise Exception(f"Args: {kwargs}, invalid for initializing a {comp_type}: {e}")
+            raise ValueError(f"Args: {kwargs}, invalid for initializing a {comp_type}: {e}")
 
         # Update state and keep track of initial version for changes / update messages
         self.state[comp_id] = new_delegate
         self.client_state[comp_id] = new_delegate.copy()
 
         # Update references for each component referenced by this one
-        self.update_references(new_delegate, new_delegate)
+        self._update_references(new_delegate, new_delegate)
 
         # Create message and broadcast
-        message = self.prepare_message("create", new_delegate)
+        message = self._prepare_message("create", new_delegate)
         self.broadcast(message)
 
         # Return component or delegate instance if applicable
         return new_delegate
 
     def delete_component(self, delegate: Union[Delegate, ID]):
         """Delete object in state and update clients
         
-        This method excepts a delegate, component, or component ID, and will attempt
+        This method excepts a delegate, or component ID, and will attempt
         to delete the component as long as it is not referenced by any other component.
         If this component is still being used by another, it will be added to a queue so that
         it can be deleted later once that reference is no longer being used.
 
         Args:
             delegate (Component, Delegate, or ID): component / delegate to be deleted
+
+        Raises:
+            TypeError: if the user specifies an invalid input type
         """
 
         # Handle cases so can except different input types - cast to ID
         if isinstance(delegate, Delegate):
             delegate = delegate
             del_id = delegate.id
         elif isinstance(delegate, ID):
             delegate = self.state[delegate]
             del_id = delegate.id
         else:
             raise TypeError(f"Invalid type for delegate when deleting: {type(delegate)}")
 
         # Delete if no references, or else queue it up for later
         if not self.references.get(del_id):
-            self.broadcast(self.prepare_message("delete", delegate))
+            self.broadcast(self._prepare_message("delete", delegate))
             del self.state[del_id]
             del self.client_state[del_id]
 
             # Free up the ID
             self.ids[type(delegate)].on_deck.put(del_id)
 
             # Clean out references from this object
@@ -580,15 +651,15 @@
                     self.delete_queue.remove(comp_id)
                     self.delete_component(comp_id)
 
         else:
             logging.warning(f"Couldn't delete {delegate}, referenced by {self.references[del_id]}, added to queue")
             self.delete_queue.add(del_id)
 
-    def find_delta(self, state, edited):
+    def _find_delta(self, state, edited):
         """Helper to find differences between two objects
         
         Also checks to find recursive cases and cases where references
         should be updated, Does this get recursive deltas tho? should it?
         """
 
         delta = set()
@@ -598,73 +669,97 @@
                 delta.add(field_name)
         return delta
 
     def update_component(self, current: Delegate):
         """Update clients with changes to a component
         
         This method broadcasts changes to all clients including only fields
-        specified in the set delta
+        specified in the set delta. Local changes to delegates will be saved
+        in the server's state, but this method must be called to update clients.
 
         Args:
             current (Delegate): component that has been updated,
                 should be a component with an update message
         """
 
         # Find difference between two states
         outdated = self.client_state[current.id]
-        delta = self.find_delta(outdated, current)
+        delta = self._find_delta(outdated, current)
 
         # Update references
-        self.update_references(outdated, outdated, removing=True)
-        self.update_references(current, current)
+        self._update_references(outdated, outdated, removing=True)
+        self._update_references(current, current)
 
         # Update tracking state
         self.client_state[current.id] = current.copy()
 
         # Form message and broadcast
         try:
-            message = self.prepare_message("update", current, delta)
+            message = self._prepare_message("update", current, delta)
             self.broadcast(message)
         except Exception as e:
             raise Exception(f"This obj can not be updated: {e}")
 
     def invoke_signal(self, signal: SignalID, on_component: Delegate, signal_data: list):
         """Send signal to target component
         
         Args:
             signal (ID): signal to be invoked
             on_component (Delegate): component to receive the signal
-            signal_data (dict): 
-        Takes Signal ID, on_component, and the data
+            signal_data (dict): data to be sent with the signal
+
+        Raises:
+            ValueError: if the user specifies an invalid on_component type
         """
 
         # Get context from on_component
         if isinstance(on_component, Entity):
             context = InvokeIDType(entity=on_component.id)
         elif isinstance(on_component, Table):
             context = InvokeIDType(table=on_component.id)
         elif isinstance(on_component, Plot):
             context = InvokeIDType(plot=on_component.id)
         else:
-            raise Exception(f"Invalid on_component type: {type(on_component)}")
+            raise ValueError(f"Invalid on_component type: {type(on_component)}")
 
         # Create invoke object and broadcast message
         invoke = Invoke(id=signal, context=context, signal_data=signal_data)
-        message = self.prepare_message("invoke", invoke)
+        message = self._prepare_message("invoke", invoke)
         self.broadcast(message)
 
     def create_method(self, name: str,
                       arg_doc: list[MethodArg],
                       doc: Optional[str] = None,
                       return_doc: Optional[str] = None) -> Method:
+        """Add a Method object to the scene and return it. Will use a custom delegate if applicable.
+
+        Args:
+            name (str): name of the method
+            arg_doc (list[MethodArg]): list of arguments and documentation for the method
+            doc (str, optional): documentation for the method
+            return_doc (str, optional): documentation for the return value
+
+        Returns:
+            Method: method delegate that was created
+        """
         return self.create_component(Method, name=name, doc=doc, return_doc=return_doc, arg_doc=arg_doc)
 
     def create_signal(self, name: str,
                       doc: Optional[str] = None,
                       arg_doc: list[MethodArg] = None) -> Signal:
+        """Add a Signal object to the session. Will use a custom delegate if applicable.
+
+        Args:
+            name (str): name of the signal
+            doc (str, optional): documentation for the signal
+            arg_doc (list[MethodArg], optional): list of arguments and documentation for the signal
+
+        Returns:
+            Signal: signal delegate that was created
+        """
         return self.create_component(Signal, name=name, doc=doc, arg_doc=arg_doc)
 
     def create_entity(self, name: Optional[str],
                       parent: Optional[EntityID] = None,
                       transform: Optional[Mat4] = None,
                       text_rep: Optional[TextRepresentation] = None,
                       web_rep: Optional[WebRepresentation] = None,
@@ -672,96 +767,234 @@
                       lights: Optional[list[LightID]] = None,
                       tables: Optional[list[TableID]] = None,
                       plots: Optional[list[PlotID]] = None,
                       tags: Optional[list[str]] = None,
                       methods_list: Optional[list[MethodID]] = None,
                       signals_list: Optional[list[SignalID]] = None,
                       influence: Optional[BoundingBox] = None) -> Entity:
+        """Add an Entity object to the session. Will use a custom delegate if applicable.
 
+        Args:
+            name (str): name of the entity
+            parent (EntityID, optional): parent entity
+            transform (Mat4, optional): transform for the entity
+            text_rep (TextRepresentation, optional): text representation for the entity
+            web_rep (WebRepresentation, optional): web representation for the entity
+            render_rep (RenderRepresentation, optional): render representation that links to geometry info
+            lights (list[LightID], optional): list of attached lights
+            tables (list[TableID], optional): list of attached tables
+            plots (list[PlotID], optional): list of attached plots
+            tags (list[str], optional): list of applicable tags
+            methods_list (list[MethodID], optional): list of methods attached to the entity
+            signals_list (list[SignalID], optional): list of signals attached to the entity
+            influence (BoundingBox, optional): bounding box for the entity
+
+        Returns:
+            Entity: entity delegate that was created
+        """
         return self.create_component(Entity, name=name, parent=parent, transform=transform, text_rep=text_rep,
                                      web_rep=web_rep, render_rep=render_rep, lights=lights, tables=tables, plots=plots,
                                      tags=tags, methods_list=methods_list, signals_list=signals_list,
                                      influence=influence)
 
     def create_plot(self, name: Optional[str] = None,
                     table: Optional[TableID] = None,
                     simple_plot: Optional[str] = None,
                     url_plot: Optional[str] = None,
                     methods_list: Optional[list[MethodID]] = None,
                     signals_list: Optional[list[SignalID]] = None) -> Plot:
+        """Add a Plot object to the session. Will use a custom delegate if applicable.
 
+        Args:
+            name (str, optional): name of the plot
+            table (TableID, optional): table to be plotted
+            simple_plot (str, optional): simple plot to be plotted
+            url_plot (str, optional): url for the plot
+            methods_list (list[MethodID], optional): attached methods
+            signals_list (list[SignalID], optional): attached signals
+
+        Returns:
+            Plot: plot delegate that was created
+        """
         return self.create_component(Plot, name=name, table=table, simple_plot=simple_plot, url_plot=url_plot,
                                      methods_list=methods_list, signals_list=signals_list)
 
     def create_buffer(self, name: Optional[str] = None,
                       size: int = None,
                       inline_bytes: bytes = None,
                       uri_bytes: str = None) -> Buffer:
+        """Add a Buffer object for the session. Will use a custom delegate if applicable.
+
+        Args:
+            name (str, optional): name of the buffer, defaults to "No-Name
+            size (int, optional): size of the buffer in bytes
+            inline_bytes (bytes, optional): bytes for the buffer
+            uri_bytes (str, optional): uri to get the bytes from the web
+
+        Returns:
+            Buffer: buffer delegate that was created
+        """
         return self.create_component(Buffer, name=name, size=size, inline_bytes=inline_bytes, uri_bytes=uri_bytes)
 
     def create_bufferview(self,
                           source_buffer: BufferID,
                           offset: int,
                           length: int,
                           name: Optional[str] = None,
                           type: Literal["UNK", "GEOMETRY", "IMAGE"] = "UNK") -> BufferView:
+        """Add a BufferView object to the session. Will use a custom delegate if applicable.
+
+        Args:
+            source_buffer (BufferID): buffer that the view is based on
+            offset (int): offset in bytes from the start of the buffer
+            length (int): length of the view in bytes
+            name (str, optional): name of the buffer view
+            type (str, optional): type of the buffer view
+
+        Returns:
+            BufferView: buffer view delegate that was created
+        """
         return self.create_component(BufferView, name=name, source_buffer=source_buffer,
                                      offset=offset, length=length, type=type)
 
     def create_material(self, name: Optional[str] = None,
                         pbr_info: Optional[PBRInfo] = PBRInfo(),
                         normal_texture: Optional[TextureRef] = None,
                         occlusion_texture: Optional[TextureRef] = None,
                         occlusion_texture_factor: Optional[float] = 1.0,
                         emissive_texture: Optional[TextureRef] = None,
                         emissive_factor: Optional[Vec3] = (1.0, 1.0, 1.0),
                         use_alpha: Optional[bool] = False,
                         alpha_cutoff: Optional[float] = .5,
                         double_sided: Optional[bool] = False) -> Material:
+        """Add a Material object to the session. Will use a custom delegate if applicable.
+
+        Args:
+            name (str, optional): name of the material
+            pbr_info (PBRInfo, optional): physically based rendering information
+            normal_texture (TextureRef, optional): texture for normal mapping
+            occlusion_texture (TextureRef, optional): texture for occlusion mapping
+            occlusion_texture_factor (float, optional): factor for occlusion mapping
+            emissive_texture (TextureRef, optional): texture for emissive mapping
+            emissive_factor (Vec3, optional): factor for emissive mapping
+            use_alpha (bool, optional): whether to use alpha
+            alpha_cutoff (float, optional): alpha cutoff value
+            double_sided (bool, optional): whether the material is double-sided
+
+        Returns:
+            Material: material delegate that was created
+        """
         return self.create_component(Material, name=name, pbr_info=pbr_info, normal_texture=normal_texture,
                                      occlusion_texture=occlusion_texture,
                                      occlusion_texture_factor=occlusion_texture_factor,
                                      emissive_texture=emissive_texture, emissive_factor=emissive_factor,
                                      use_alpha=use_alpha, alpha_cutoff=alpha_cutoff, double_sided=double_sided)
 
     def create_image(self, name: Optional[str] = None,
                      buffer_source: BufferID = None,
                      uri_source: str = None) -> Image:
+        """Add an Image object to the session.
+
+        Will use a custom delegate if applicable. Must specify either a buffer_source or a uri_source.
+
+        Args:
+            name (str, optional): name of the image
+            buffer_source (BufferID, optional): buffer data that for image
+            uri_source (str, optional): uri to get the image bytes from
+
+        Returns:
+            Image: image delegate that was created
+        """
         return self.create_component(Image, name=name, buffer_source=buffer_source, uri_source=uri_source)
 
     def create_texture(self, image: ImageID,
                        name: Optional[str] = None,
                        sampler: Optional[SamplerID] = None) -> Texture:
+        """Add a Texture object to the session. Will use a custom delegate if applicable.
+
+        Args:
+            image (ImageID): image to be used for the texture
+            name (str, optional): name of the texture
+            sampler (SamplerID, optional): sampler to be used for the texture
+
+        Returns:
+            Texture: texture delegate that was created
+        """
         return self.create_component(Texture, name=name, image=image, sampler=sampler)
 
     def create_sampler(self, name: Optional[str] = None,
                        mag_filter: Optional[Literal["NEAREST", "LINEAR"]] = "LINEAR",
                        min_filter: Optional[
                            Literal["NEAREST", "LINEAR", "LINEAR_MIPMAP_LINEAR"]] = "LINEAR_MIPMAP_LINEAR",
                        wrap_s: Optional[SamplerMode] = "REPEAT",
                        wrap_t: Optional[SamplerMode] = "REPEAT") -> Sampler:
+        """Add a Sampler object to the session. Will use a custom delegate if applicable.
+
+        Args:
+            name (str, optional): name of the sampler
+            mag_filter (str, optional): magnification filter
+            min_filter (str, optional): minification filter
+            wrap_s (str, optional): wrap mode for s coordinate
+            wrap_t (str, optional): wrap mode for t coordinate
+
+        Returns:
+            Sampler: sampler delegate that was created
+        """
         return self.create_component(Sampler, name=name, mag_filter=mag_filter, min_filter=min_filter,
                                      wrap_s=wrap_s, wrap_t=wrap_t)
 
     def create_light(self, name: Optional[str] = None,
                      color: Optional[RGB] = (1.0, 1.0, 1.0),
                      intensity: Optional[float] = 1.0,
                      point: PointLight = None,
                      spot: SpotLight = None,
                      directional: DirectionalLight = None) -> Light:
+        """Add a Light object to the session. Will use a custom delegate if applicable.
+
+        Args:
+            name (str, optional): name of the light
+            color (RGB, optional): color of the light
+            intensity (float, optional): intensity of the light on scale from 0-1
+            point (PointLight, optional): point light information
+            spot (SpotLight, optional): spot light information
+            directional (DirectionalLight, optional): directional light information
+
+        Returns:
+            Light: light delegate that was created
+        """
         return self.create_component(Light, name=name, color=color, intensity=intensity,
                                      point=point, spot=spot, directional=directional)
 
     def create_geometry(self, patches: list[GeometryPatch], name: Optional[str] = None) -> Geometry:
+        """Add a Geometry object to the session. Will use a custom delegate if applicable.
+
+        Args:
+            patches (list[GeometryPatch]): list of geometry patches
+            name (str, optional): name of the geometry
+
+        Returns:
+            Geometry: geometry delegate that was created
+        """
         return self.create_component(Geometry, name=name, patches=patches)
 
     def create_table(self, name: Optional[str] = None,
                      meta: Optional[str] = None,
                      methods_list: Optional[list[MethodID]] = None,
                      signals_list: Optional[list[SignalID]] = None) -> Table:
+        """Add a Table object to the session. Will use a custom delegate if applicable.
+
+        Args:
+            name (str, optional): name of the table
+            meta (str, optional): meta description for the table
+            methods_list (list[MethodID], optional): list of methods for the table
+            signals_list (list[SignalID], optional): list of signals for the table
+
+        Returns:
+            Table: table delegate that was created
+        """
         return self.create_component(Table, name=name, meta=meta, methods_list=methods_list, signals_list=signals_list)
 
 
 # Helpers for ordering messages
 def top_sort_recurse(id, refs, visited, components, stack):
     """Helper for order_components to recurse"""
```

### Comparing `rigatoni-0.2.1/rigatoni/geometry/__init__.py` & `rigatoni-0.2.2/rigatoni/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.1/rigatoni/geometry/byte_server.py` & `rigatoni-0.2.2/rigatoni/geometry/byte_server.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,59 @@
 import socket
 import re
 import threading
 
 
 class ByteServer(object):
-    """Server to Host URI Bytes
+    """Server to Host URI Bytes.
+
+    This is helpful for large meshes and images that would
+    otherwise be too large to send using CBOR and the websocket connection. The server maps
+    a tag to a buffer, and the client can request the buffer using the url that includes the
+    tag.
     
     Attributes:
         host (str): IP address for server
         port (int): port server is listening on
         socket (socket): socket connection 
         buffers (dict): mapping tag to buffer
-        next_tag (int): next available tag for a buffer
+        _next_tag (int): next available tag for a buffer
         url (str): base url to reach server without tag
         thread (Thread): background thread server is running in
         running (bool): flag indicating whether server is running
     """
 
     def __init__(self, port: int = 8000):
-        """Constructor
+        """Constructor to create the server
         
         Args:
-            port (int): port to listen on
+            port (int): port to listen and host on
         """
 
         name = socket.gethostname()
         try:  # supposed to work without .local, but had to add to match system preferences - sharing
             self.host = socket.gethostbyname(name)
         except socket.gaierror:
             self.host = socket.gethostbyname(f"{name}.local")
 
         self.port = port
         self.socket = None
         self.buffers = {}
-        self.next_tag = 0
+        self._next_tag = 0
         self.url = f"http://{self.host}:{port}"
 
         self.thread = threading.Thread(target=self.run, args=())
         self.running = True
         self.thread.start()
 
-    def get_tag(self):
-        """Helper to get next tag"""
+    def _get_tag(self):
+        """Helper to get next tag for a buffer"""
 
-        tag = self.next_tag
-        self.next_tag += 1
+        tag = self._next_tag
+        self._next_tag += 1
         return str(tag)
 
     def get_buffer(self, uri: str):
         """Helper to get bytes for a URI
         
         Mostly used in geometry creation for exporting as of right now
 
@@ -63,16 +68,15 @@
             return buffer_bytes
         else:
             raise Exception("Invalid HTTP Request")
 
     def run(self):
         """Main loop to run in thread
         
-        Runs the server and listens for byte requests
-        Uses HTTP protocol 
+        Runs the server and listens for byte requests using HTTP protocol
         """
 
         # Create socket
         server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         server_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         server_socket.bind((self.host, self.port))
 
@@ -100,30 +104,28 @@
                 header = f'HTTP/1.0 200 OK\r\nContent-Type: application/octet-stream\r\nContent-Length: {len(select_bytes)}\n\n'
                 response = bytearray(header.encode()) + select_bytes
             else:
                 header = f'HTTP/1.0 500 FAIL'
                 response = header.encode()
 
             # Send HTTP response
-            # client_connection.sendall(response.encode())
-            # print(f'Response:\n{response}')
             client_connection.sendall(response)
             client_connection.close()
 
         # Clean up and close socket
         self.socket.close()
 
     def add_buffer(self, buffer) -> str:
         """Add buffer to server and return url to reach it
         
         Args:
             buffer (bytes): bytes to add as buffer
         """
 
-        tag = self.get_tag()
+        tag = self._get_tag()
         self.buffers[tag] = buffer
         url = f"{self.url}/{tag}"
         print(f"Adding Buffer: {url}")
 
         return url
 
     def shutdown(self):
```

### Comparing `rigatoni-0.2.1/rigatoni/geometry/geometry_creation.py` & `rigatoni-0.2.2/rigatoni/geometry/geometry_creation.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,14 +270,17 @@
 def build_entity(server: Server, geometry: nooobs.Geometry, instances: list[list] = None):
     """Build Entity from Geometry
     
     Args:
         server (Server): server to build entity component on
         geometry (Geometry): geometry to link entity to
         instances (Mat4): optional instance matrix, can use create_instances to generate
+
+    Returns:
+        Entity: newly created entity delegate
     """
 
     # Set name to match geometry
     name = geometry.name if geometry.name else None
 
     # Create instance buffer and view if specified
     if instances:
@@ -304,23 +307,26 @@
 def create_instances(
         positions: list[list] = None,
         colors: list[list] = None,
         rotations: list[list] = None,
         scales: list[list] = None) -> list[list]:
     """Create new instances for an entity
     
-    All lists are optional and will be filled with defaults
-    By default one instance is created at least
-    Lists are padded out to 4 values
+    All lists are optional and will be filled with defaults.
+    By default, one instance is created at least.
+    Lists are padded out to 4 values.
 
     Args:
         positions (list[Vec3]): positions for each instance
         colors (list[Vec4]): Colors for each instance
         rotations (list[Vec4]): Rotations for each instance
         scales (list[Vec3]): Scales for each instance
+
+    Returns:
+        list[list]: 2d array representing instance data
     """
 
     def padded(lst: list, default_val: float = 1.0):
         """Helper to pad the lists"""
 
         lst = list(lst)
         if len(lst) < 4:
@@ -498,24 +504,34 @@
 
 
 def geometry_from_mesh(server: Server, file, material: nooobs.Material,
                        mesh_name: Optional[str] = None, byte_server: ByteServer = None, generate_normals: bool = True):
     """Construct geometry from mesh file
     
     Can specify byte server if it is a big mesh and needs uri bytes
+
+    Args:
+        server (Server): server to load geometry onto
+        file (str, path): file to load mesh from
+        material (Material): material to use in geometry
+        mesh_name (str): optional name
+        byte_server (ByteServer): server to support URI bytes if needed
+        generate_normals (bool): whether to calculate normals for the mesh
+
+    Returns:
+        Geometry: newly created geometry delegate
     """
 
     # Create meshio mesh object to extract data from file, if unsupported file type use meshlab
     try:
         mesh = meshio.read(file)
     except Exception as e:
         return meshlab_load(server, byte_server, file, material, mesh_name, generate_normals=generate_normals)
 
-        # Define Meshio helper functions
-
+    # Define Meshio helper functions
     def get_point_attr(mesh_obj, attr: str):
         """Helper to get attribute from mesh object"""
 
         data = mesh_obj.point_data.get(attr)
         try:
             return data.tolist()
         except:
```

### Comparing `rigatoni-0.2.1/rigatoni/geometry/geometry_objects.py` & `rigatoni-0.2.2/rigatoni/geometry/geometry_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 These are based on the noodle_objects.py module and implement validation
 """
 
 from typing import Optional
 
 from .. import noodle_objects as nooobs
 
+
 class AttributeInput(nooobs.NoodleObject):
     """Input for setting attributes of a buffer 
     
     User should not have to concern themselves with this input
     """
 
     semantic: nooobs.AttributeSemantic
```

### Comparing `rigatoni-0.2.1/rigatoni/noodle_objects.py` & `rigatoni-0.2.2/rigatoni/noodle_objects.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Follows the specification in the cddl document, and
 implements strict validation
 """
 
 from enum import Enum
 from math import pi
 from queue import Queue
-from typing import Callable, Optional, Any, Union, List, Tuple, Dict, NamedTuple
+from typing import Callable, Optional, Any, List, Tuple, Dict, NamedTuple
 
 from pydantic import BaseModel, root_validator
 
 """ =============================== ID's ============================= """
 
 
 class ID(NamedTuple):
@@ -104,15 +104,15 @@
         arbitrary_types_allowed = True
         use_enum_values = True
 
 
 class Delegate(NoodleObject):
     """Parent class for all delegates
 
-    Defines general methods that should be available for all delegates
+    Defines general methods that should be available for all delegates.
 
     Attributes:
         server (Server): server delegate is attached to
         id: (ID): Unique identifier for delegate
         name (str): Name of delegate
         signals (dict): Signals that can be called on delegate, method name to callable
     """
@@ -313,15 +313,15 @@
 
 
 class InvokeIDType(NoodleObject):
     entity: Optional[EntityID] = None
     table: Optional[TableID] = None
     plot: Optional[PlotID] = None
 
-    @root_validator
+    @root_validator(allow_reuse=True)
     def one_of_three(cls, values):
         already_found = False
         for field in values:
             if values[field] and already_found:
                 raise ValueError("More than one field entered")
             elif values[field]:
                 already_found = True
@@ -340,15 +340,15 @@
 class TableInitData(NoodleObject):
     columns: List[TableColumnInfo]
     keys: List[int]
     data: List[List[Any]]  # Originally tried union, but currently order is used to coerce by pydantic
     selections: Optional[List[Selection]] = None
 
     # too much overhead? - strict mode
-    @root_validator
+    @root_validator(allow_reuse=True)
     def types_match(cls, values):
         for row in values['data']:
             for col, i in zip(values['columns'], range(len(row))):
                 text_mismatch = isinstance(row[i], str) and col.type != "TEXT"
                 real_mismatch = isinstance(row[i], float) and col.type != "REAL"
                 int_mismatch = isinstance(row[i], int) and col.type != "INTEGER"
                 if text_mismatch or real_mismatch or int_mismatch:
@@ -356,29 +356,67 @@
         return values
 
 
 """ ====================== NOODLE COMPONENTS / DELEGATES ====================== """
 
 
 class Method(Delegate):
+    """A method that clients can request the server to call.
+
+    Attributes:
+        id: ID for the method
+        name: Name of the method
+        doc: Documentation for the method
+        return_doc: Documentation for the return value
+        arg_doc: Documentation for the arguments
+    """
+
     id: MethodID
     name: str
     doc: Optional[str] = None
     return_doc: Optional[str] = None
     arg_doc: List[MethodArg] = []
 
 
 class Signal(Delegate):
+    """A signal that the server can send to update clients.
+
+    Attributes:
+        id: ID for the signal
+        name: Name of the signal
+        doc: Documentation for the signal
+        arg_doc: Documentation for the arguments
+    """
+
     id: SignalID
     name: str
     doc: Optional[str] = None
     arg_doc: List[MethodArg] = None
 
 
 class Entity(Delegate):
+    """Container for other entities, possibly renderable, has associated methods and signals
+
+    Args:
+        id (EntityID): ID for the entity
+        name (str): Name of the entity
+        parent (EntityID): Parent entity
+        transform (Mat4): Local transform for the entity
+        text_rep (TextRepresentation): Text representation for the entity
+        web_rep (WebRepresentation): Web representation for the entity
+        render_rep (RenderRepresentation): Render representation for the entity
+        lights (List[LightID]): List of lights attached to the entity
+        tables (List[TableID]): List of tables attached to the entity
+        plots (List[PlotID]): List of plots attached to the entity
+        tags (List[str]): List of tags for the entity
+        methods_list (List[MethodID]): List of methods attached to the entity
+        signals_list (List[SignalID]): List of signals attached to the entity
+        influence (Optional[BoundingBox]): Bounding box for the entity
+    """
+
     id: EntityID
     name: Optional[str] = None
 
     parent: Optional[EntityID] = None
     transform: Optional[Mat4] = None
 
     text_rep: Optional[TextRepresentation] = None
@@ -392,60 +430,106 @@
     methods_list: Optional[List[MethodID]] = None
     signals_list: Optional[List[SignalID]] = None
 
     influence: Optional[BoundingBox] = None
 
 
 class Plot(Delegate):
+    """An abstract plot object.
+
+    Attributes:
+        id: ID for the plot
+        name: Name of the plot
+        table: Table to plot
+        simple_plot: Simple plot to render
+        url_plot: URL for plot to render
+        methods_list: List of methods attached to the plot
+        signals_list: List of signals attached to the plot
+    """
+
     id: PlotID
     name: Optional[str] = None
 
     table: Optional[TableID] = None
 
     simple_plot: Optional[str] = None
     url_plot: Optional[str] = None
 
     methods_list: Optional[List[MethodID]] = None
     signals_list: Optional[List[SignalID]] = None
 
-    @root_validator
+    @root_validator(allow_reuse=True)
     def one_of(cls, values):
         if bool(values['simple_plot']) != bool(values['url_plot']):
             return values
         else:
             raise ValueError("One plot type must be specified")
 
 
 class Buffer(Delegate):
+    """A buffer of bytes containing data for an image or a mesh.
+
+    Attributes:
+        id: ID for the buffer
+        name: Name of the buffer
+        size: Size of the buffer in bytes
+        inline_bytes: Bytes of the buffer
+        uri_bytes: URI for the bytes
+    """
     id: BufferID
     name: Optional[str] = None
     size: int = None
 
     inline_bytes: bytes = None
     uri_bytes: str = None
 
-    @root_validator
+    @root_validator(allow_reuse=True)
     def one_of(cls, values):
         if bool(values['inline_bytes']) != bool(values['uri_bytes']):
             return values
         else:
             raise ValueError("One plot type must be specified")
 
 
 class BufferView(Delegate):
+    """A view into a buffer, specifying a subset of the buffer and how to interpret it.
+
+    Attributes:
+        id: ID for the buffer view
+        name: Name of the buffer view
+        source_buffer: Buffer that the view is referring to
+        type: Type of the buffer view
+        offset: Offset into the buffer in bytes
+        length: Length of the buffer view in bytes
+    """
     id: BufferViewID
     name: Optional[str] = None
     source_buffer: BufferID
 
     type: BufferType = BufferType.unknown
     offset: int
     length: int
 
 
 class Material(Delegate):
+    """A material that can be applied to a mesh.
+
+    Attributes:
+        id: ID for the material
+        name: Name of the material
+        pbr_info: Information for physically based rendering
+        normal_texture: Texture for normals
+        occlusion_texture: Texture for occlusion
+        occlusion_texture_factor: Factor for occlusion
+        emissive_texture: Texture for emissive
+        emissive_factor: Factor for emissive
+        use_alpha: Whether to use alpha
+        alpha_cutoff: Alpha cutoff
+        double_sided: Whether the material is double-sided
+    """
     id: MaterialID
     name: Optional[str] = None
 
     pbr_info: Optional[PBRInfo] = PBRInfo()
     normal_texture: Optional[TextureRef] = None
 
     occlusion_texture: Optional[TextureRef] = None  # assumed to be linear, ONLY R used
@@ -457,58 +541,95 @@
     use_alpha: Optional[bool] = False
     alpha_cutoff: Optional[float] = .5
 
     double_sided: Optional[bool] = False
 
 
 class Image(Delegate):
+    """An image, can be used for a texture
+
+    Attributes:
+        id: ID for the image
+        name: Name of the image
+        buffer_source: Buffer that the image is stored in
+        uri_source: URI for the bytes if they are hosted externally
+    """
     id: ImageID
     name: Optional[str] = None
 
     buffer_source: BufferID = None
     uri_source: str = None
 
-    @root_validator
+    @root_validator(allow_reuse=True)
     def one_of(cls, values):
         if bool(values['buffer_source']) != bool(values['uri_source']):
             return values
         else:
             raise ValueError("One plot type must be specified")
 
 
 class Texture(Delegate):
+    """A texture, can be used for a material
+
+    Attributes:
+        id: ID for the texture
+        name: Name of the texture
+        image: Image to use for the texture
+        sampler: Sampler to use for the texture
+    """
     id: TextureID
     name: Optional[str] = None
     image: ImageID  # Image ID
     sampler: Optional[SamplerID] = None
 
 
 class Sampler(Delegate):
+    """A sampler to use for a texture
+
+    Attributes:
+        id: ID for the sampler
+        name: Name of the sampler
+        mag_filter: Magnification filter
+        min_filter: Minification filter
+        wrap_s: Wrap mode for S
+        wrap_t: Wrap mode for T
+    """
     id: SamplerID
     name: Optional[str] = None
 
     mag_filter: Optional[MagFilterTypes] = MagFilterTypes.linear
     min_filter: Optional[MinFilterTypes] = MinFilterTypes.linear_mipmap_linear
 
     wrap_s: Optional[SamplerMode] = "REPEAT"
     wrap_t: Optional[SamplerMode] = "REPEAT"
 
 
 class Light(Delegate):
+    """Represents a light in the scene
+
+    Attributes:
+        id: ID for the light
+        name: Name of the light
+        color: Color of the light
+        intensity: Intensity of the light
+        point: Point light information
+        spot: Spotlight information
+        directional: Directional light information
+    """
     id: LightID
     name: Optional[str] = None
 
     color: Optional[RGB] = [1.0, 1.0, 1.0]
     intensity: Optional[float] = 1.0
 
     point: PointLight = None
     spot: SpotLight = None
     directional: DirectionalLight = None
 
-    @root_validator
+    @root_validator(allow_reuse=True)
     def one_of(cls, values):
         already_found = False
         for field in ['point', 'spot', 'directional']:
             if values[field] and already_found:
                 raise ValueError("More than one field entered")
             elif values[field]:
                 already_found = True
@@ -516,54 +637,78 @@
         if not already_found:
             raise ValueError("No field provided")
         else:
             return values
 
 
 class Geometry(Delegate):
+    """Represents geometry in the scene and can be used for meshes
+
+    Attributes:
+        id: ID for the geometry
+        name: Name of the geometry
+        patches: Patches that make up the geometry
+    """
     id: GeometryID
     name: Optional[str] = None
     patches: List[GeometryPatch]
 
 
 class Table(Delegate):
+    """Object to store tabular data.
+
+    Attributes:
+        id: ID for the table
+        name: Name of the table
+        meta: Metadata for the table
+        methods_list: List of methods for the table
+        signals_list: List of signals for the table
+    """
     id: TableID
     name: Optional[str] = None
 
     meta: Optional[str] = None
     methods_list: Optional[List[MethodID]] = None
     signals_list: Optional[List[SignalID]] = None
 
-    def handle_insert(self, new_rows: list[list[int]]):
+    def handle_insert(self, new_rows: List[List[int]]):
+        """Method to handle inserting into the table"""
         pass
 
-    def handle_update(self, keys: list[int], rows: list[list[int]]):
+    def handle_update(self, keys: List[int], rows: List[List[int]]):
+        """Method to handle updating the table"""
         pass
 
-    def handle_delete(self, keys: list[int]):
+    def handle_delete(self, keys: List[int]):
+        """Method to handle deleting from the table"""
         pass
 
     def handle_clear(self):
+        """Method to handle clearing the table"""
         pass
 
     def handle_set_selection(self, selection: Selection):
+        """Method to handle setting a selection"""
         pass
 
     # Signals ---------------------------------------------------
     def table_reset(self, tbl_init: TableInitData):
         """Invoke table reset signal"""
         pass
 
-    def table_updated(self, keys: list[int], rows: list[list[int]]):
+    def table_updated(self, keys: List[int], rows: List[List[int]]):
+        """Invoke table updated signal"""
         pass
 
-    def table_rows_removed(self, keys: list[int]):
+    def table_rows_removed(self, keys: List[int]):
+        """Invoke table rows removed signal"""
         pass
 
     def table_selection_updated(self, selection: Selection):
+        """Invoke table selection updated signal"""
         pass
 
 
 """ ====================== Communication Objects ====================== """
 
 
 class Invoke(NoodleObject):
```

