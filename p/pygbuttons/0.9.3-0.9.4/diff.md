# Comparing `tmp/pygbuttons-0.9.3.tar.gz` & `tmp/pygbuttons-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jarnodewit/Documents/Python/Utils/Buttons2/dist/.tmp-62mxbrgu/pygbuttons-0.9.3.tar", last modified: Fri Dec  9 18:24:47 2022, max compression
+gzip compressed data, was "/Users/jarnodewit/Documents/Python/Utils/Buttons2/dist/.tmp-qnvwddty/pygbuttons-0.9.4.tar", last modified: Thu Jun 15 21:03:37 2023, max compression
```

## Comparing `pygbuttons-0.9.3.tar` & `pygbuttons-0.9.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 jarnodewit   (501) staff       (20)        0 2022-12-09 18:24:47.761753 pygbuttons-0.9.3/
--rw-r--r--   0 jarnodewit   (501) staff       (20)     1069 2022-03-28 20:21:43.000000 pygbuttons-0.9.3/LICENSE
--rw-r--r--   0 jarnodewit   (501) staff       (20)     1905 2022-12-09 18:24:47.762023 pygbuttons-0.9.3/PKG-INFO
--rw-r--r--   0 jarnodewit   (501) staff       (20)     1425 2022-12-09 18:11:51.000000 pygbuttons-0.9.3/README.md
--rw-r--r--   0 jarnodewit   (501) staff       (20)      108 2022-09-14 12:30:19.000000 pygbuttons-0.9.3/pyproject.toml
--rw-r--r--   0 jarnodewit   (501) staff       (20)      641 2022-12-09 18:24:47.763349 pygbuttons-0.9.3/setup.cfg
-drwxr-xr-x   0 jarnodewit   (501) staff       (20)        0 2022-12-09 18:24:47.730793 pygbuttons-0.9.3/src/
-drwxr-xr-x   0 jarnodewit   (501) staff       (20)        0 2022-12-09 18:24:47.750308 pygbuttons-0.9.3/src/pygbuttons/
--rw-r--r--   0 jarnodewit   (501) staff       (20)    43951 2022-11-30 20:39:53.000000 pygbuttons-0.9.3/src/pygbuttons/Base.py
--rw-r--r--   0 jarnodewit   (501) staff       (20)    12754 2022-11-30 20:48:55.000000 pygbuttons-0.9.3/src/pygbuttons/Button.py
--rw-r--r--   0 jarnodewit   (501) staff       (20)    30671 2022-11-30 20:46:47.000000 pygbuttons-0.9.3/src/pygbuttons/DropdownBox.py
--rw-r--r--   0 jarnodewit   (501) staff       (20)    20357 2022-11-30 16:51:14.000000 pygbuttons-0.9.3/src/pygbuttons/Slider.py
--rw-r--r--   0 jarnodewit   (501) staff       (20)    16406 2022-11-30 18:40:52.000000 pygbuttons-0.9.3/src/pygbuttons/Text.py
--rw-r--r--   0 jarnodewit   (501) staff       (20)    18275 2022-11-30 21:13:53.000000 pygbuttons-0.9.3/src/pygbuttons/TextBox.py
--rw-r--r--   0 jarnodewit   (501) staff       (20)      379 2022-12-09 18:06:04.000000 pygbuttons-0.9.3/src/pygbuttons/__init__.py
-drwxr-xr-x   0 jarnodewit   (501) staff       (20)        0 2022-12-09 18:24:47.760833 pygbuttons-0.9.3/src/pygbuttons.egg-info/
--rw-r--r--   0 jarnodewit   (501) staff       (20)     1905 2022-12-09 18:24:47.000000 pygbuttons-0.9.3/src/pygbuttons.egg-info/PKG-INFO
--rw-r--r--   0 jarnodewit   (501) staff       (20)      410 2022-12-09 18:24:47.000000 pygbuttons-0.9.3/src/pygbuttons.egg-info/SOURCES.txt
--rw-r--r--   0 jarnodewit   (501) staff       (20)        1 2022-12-09 18:24:47.000000 pygbuttons-0.9.3/src/pygbuttons.egg-info/dependency_links.txt
--rw-r--r--   0 jarnodewit   (501) staff       (20)       14 2022-12-09 18:24:47.000000 pygbuttons-0.9.3/src/pygbuttons.egg-info/requires.txt
--rw-r--r--   0 jarnodewit   (501) staff       (20)       11 2022-12-09 18:24:47.000000 pygbuttons-0.9.3/src/pygbuttons.egg-info/top_level.txt
+drwxr-xr-x   0 jarnodewit   (501) staff       (20)        0 2023-06-15 21:03:37.019439 pygbuttons-0.9.4/
+-rw-r--r--   0 jarnodewit   (501) staff       (20)     1069 2022-03-28 20:21:43.000000 pygbuttons-0.9.4/LICENSE
+-rw-r--r--   0 jarnodewit   (501) staff       (20)     1815 2023-06-15 21:03:37.021003 pygbuttons-0.9.4/PKG-INFO
+-rw-r--r--   0 jarnodewit   (501) staff       (20)     1335 2023-04-28 17:23:39.000000 pygbuttons-0.9.4/README.md
+-rw-r--r--   0 jarnodewit   (501) staff       (20)      108 2022-09-14 12:30:19.000000 pygbuttons-0.9.4/pyproject.toml
+-rw-r--r--   0 jarnodewit   (501) staff       (20)      641 2023-06-15 21:03:37.030802 pygbuttons-0.9.4/setup.cfg
+drwxr-xr-x   0 jarnodewit   (501) staff       (20)        0 2023-06-15 21:03:36.528286 pygbuttons-0.9.4/src/
+drwxr-xr-x   0 jarnodewit   (501) staff       (20)        0 2023-06-15 21:03:36.944302 pygbuttons-0.9.4/src/pygbuttons/
+-rw-r--r--   0 jarnodewit   (501) staff       (20)    27031 2023-04-28 17:26:11.000000 pygbuttons-0.9.4/src/pygbuttons/Base.py
+-rw-r--r--   0 jarnodewit   (501) staff       (20)    13906 2023-06-15 21:02:51.000000 pygbuttons-0.9.4/src/pygbuttons/Button.py
+-rw-r--r--   0 jarnodewit   (501) staff       (20)    26062 2023-06-15 21:02:51.000000 pygbuttons-0.9.4/src/pygbuttons/Control.py
+-rw-r--r--   0 jarnodewit   (501) staff       (20)    30895 2023-06-15 21:02:51.000000 pygbuttons-0.9.4/src/pygbuttons/DropdownBox.py
+-rw-r--r--   0 jarnodewit   (501) staff       (20)    21087 2023-06-15 21:02:51.000000 pygbuttons-0.9.4/src/pygbuttons/Slider.py
+-rw-r--r--   0 jarnodewit   (501) staff       (20)    16793 2023-06-15 21:02:51.000000 pygbuttons-0.9.4/src/pygbuttons/Text.py
+-rw-r--r--   0 jarnodewit   (501) staff       (20)    18448 2023-06-15 21:02:51.000000 pygbuttons-0.9.4/src/pygbuttons/TextBox.py
+-rw-r--r--   0 jarnodewit   (501) staff       (20)      585 2023-06-15 17:10:28.000000 pygbuttons-0.9.4/src/pygbuttons/__init__.py
+drwxr-xr-x   0 jarnodewit   (501) staff       (20)        0 2023-06-15 21:03:37.007172 pygbuttons-0.9.4/src/pygbuttons.egg-info/
+-rw-r--r--   0 jarnodewit   (501) staff       (20)     1815 2023-06-15 21:03:36.000000 pygbuttons-0.9.4/src/pygbuttons.egg-info/PKG-INFO
+-rw-r--r--   0 jarnodewit   (501) staff       (20)      436 2023-06-15 21:03:36.000000 pygbuttons-0.9.4/src/pygbuttons.egg-info/SOURCES.txt
+-rw-r--r--   0 jarnodewit   (501) staff       (20)        1 2023-06-15 21:03:36.000000 pygbuttons-0.9.4/src/pygbuttons.egg-info/dependency_links.txt
+-rw-r--r--   0 jarnodewit   (501) staff       (20)       14 2023-06-15 21:03:36.000000 pygbuttons-0.9.4/src/pygbuttons.egg-info/requires.txt
+-rw-r--r--   0 jarnodewit   (501) staff       (20)       11 2023-06-15 21:03:36.000000 pygbuttons-0.9.4/src/pygbuttons.egg-info/top_level.txt
```

### Comparing `pygbuttons-0.9.3/LICENSE` & `pygbuttons-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pygbuttons-0.9.3/PKG-INFO` & `pygbuttons-0.9.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygbuttons
-Version: 0.9.3
+Version: 0.9.4
 Summary: Adds basic UI elements for pygame
 Home-page: https://github.com/Jarno-de-Wit/PygButtons
 Author: Jarno de Wit
 Project-URL: Bug Tracker, https://github.com/Jarno-de-Wit/PygButtons/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,17 +32,16 @@
 To use the Buttons in a program, it is recommended to perform the following steps:
 - Setup
   1. Import the module / the contents of the module.
   2. Set the settings for the Buttons module (framerate, scroll factor, scaling limits) where appropriate
   3. Create the required Buttons
 - While running
   1. Pass all (relevant) Pygame.Events to the active Buttons in the input loop
-  2. Update the Buttons with information which is not event driven (e.g. cursor position)
-  3. Draw the Buttons to the active screen
-  4. Repeat
+  2. Draw the Buttons to the active screen
+  3. Repeat
 
 Getting an output from a Button can be done either by binding a function to the Button (which is then automatically executed when a certain action takes place), or by polling the Buttons value / status.
 
 For a practical implementation, see the [example.py](https://github.com/Jarno-de-Wit/PygButtons/blob/main/Example.py) file.
 
 ## Support
 For support / issues, please visit the issue tracker on [GitHub](https://github.com/Jarno-de-Wit/PygButtons/issues).
```

### Comparing `pygbuttons-0.9.3/README.md` & `pygbuttons-0.9.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -18,17 +18,16 @@
 To use the Buttons in a program, it is recommended to perform the following steps:
 - Setup
   1. Import the module / the contents of the module.
   2. Set the settings for the Buttons module (framerate, scroll factor, scaling limits) where appropriate
   3. Create the required Buttons
 - While running
   1. Pass all (relevant) Pygame.Events to the active Buttons in the input loop
-  2. Update the Buttons with information which is not event driven (e.g. cursor position)
-  3. Draw the Buttons to the active screen
-  4. Repeat
+  2. Draw the Buttons to the active screen
+  3. Repeat
 
 Getting an output from a Button can be done either by binding a function to the Button (which is then automatically executed when a certain action takes place), or by polling the Buttons value / status.
 
 For a practical implementation, see the [example.py](https://github.com/Jarno-de-Wit/PygButtons/blob/main/Example.py) file.
 
 ## Support
 For support / issues, please visit the issue tracker on [GitHub](https://github.com/Jarno-de-Wit/PygButtons/issues).
```

### Comparing `pygbuttons-0.9.3/setup.cfg` & `pygbuttons-0.9.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pygbuttons
-version = 0.9.3
+version = 0.9.4
 author = Jarno de Wit
 description = Adds basic UI elements for pygame
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Jarno-de-Wit/PygButtons
 project_urls = 
 	Bug Tracker = https://github.com/Jarno-de-Wit/PygButtons/issues
```

### Comparing `pygbuttons-0.9.3/src/pygbuttons/Base.py` & `pygbuttons-0.9.4/src/pygbuttons/Base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,42 @@
 import os
 os.environ["PYGAME_HIDE_SUPPORT_PROMPT"] = ""
 import pygame
 
+from .Control import Buttons
+from .utils.WeakCache import weak_cache
+
 import math
 
 pygame.font.init() #Required to set a font
 
 
 
-class Buttons():
+class ButtonBase():
     """
     A class to serve as a base for all Button classes. Also provides interfaces for button-to-button "communication" (e.g. claiming a cursor lock)
-    Furthermore, provides certain functionalities that make it easier to implement buttons into a program. (E.G. a way to Click all relevant buttons)
-
-    Capitalisation:
-    All actions that can be applied to a button (e.g. LMB_down) are capitalised.
-    All attributes and functions that do not directly alter anything about the button itself (e.g. scaling a variable to the Buttons' scale) are not capitalised.
-
-    Available Actions - for more detailed information, see help(Buttons.*function_name*):
-    Buttons.Event(pygame.Event, group) - Allows for a pygame.event to be processed completely autonomously, and be diverted to the correct buttons. No further intervention is required if this function is used.
-    Buttons.Update(group) - Updates all Buttons in the given group wherever necessary, such as updating the current cursor position for active sliders. Should be called once at the end of each input / event cycle.
-    Buttons.Draw(screen, group) - Draw all Buttons in the given group(s) to the given screen / pygame.Surface
-    Buttons.Scale(scale, group) - Scales all Buttons in the given group to / by the given factor.
-    Buttons.Move(offset, group) - Moves all Buttons in the given group by the given offset.
-    Buttons.Clear(group) - Clears all user inputs from Buttons. Note: Does NOT remove the text from Text objects.
-
-    Other Actions (automatically called by Buttons.Event() / Buttons.Update() when required):
-    Buttons.LMB_down(pos, group) - Perform a LMB_down (normal mouse click) at a certain position.
-    Buttons.LMB_up(pos, group) - Perform a LMB_up (releasing a normal mouse click) at a certain position.
-    Buttons.Scroll(value, pos, group) - Perform a Scrolling action at a certain position.
-    Buttons.Key_down(event, group) - Perform a Key_down (typing) action.
-    Buttons.Set_cursor_pos(pos, group) - Update the cursor position.
 
     Available functions:
     Buttons.get_group(group) - Will return a list of all Buttons that are in the given group(s). Also used internally when getting all buttons for which an Action should be applied.
 
     Class attributes:
     Buttons.input_claim - Contains whether or not the last input was fully claimed by a Button. E.G. If a DropdownBox was extended by clicking on  the Arrow button.
     Buttons.input_processed - Contains whether or not the last input was handled by a Button, even if they did not fully claim it. E.G. when exiting a TextBox by clicking outside of the TextBox area.
 
 
     Individual Button functions:
     *.get_rect() - Get a pygame.Rect object for the Button.
     *.get_scaled_rect() - Get a pygame.Rect object for the Button at its current scale.
     *.Add_to_group(group) - Add the Button on which this is called to the given group(s).
     """
-    #A base class for all buttons
-    input_lock = None #Either None, or the currently selected button. Used to give the currently selected button input priority.
-    input_claim = False #Set to True if a button has claimed the input, to prevent an input from affecting multiple buttons.
-    input_processed = False
     #Flags determining whether callbacks should be made and update_flags should be set.
     #Can be set using Buttons.Callbacks() and Buttons.Update_flags()
     _callbacks = False
     _update_flags = False
-    list_all = [] #A list containing all buttons, except those marked as independent. Can be used for debugging, or just to keep a nice list of all buttons.
-    groups = {} #Groups to be used for getting certain buttons.
-    scroll_factor = 1 #A factor to multiply scrolling with. Should be set based on the target DPI / resolution of the program
-    #A framerate variable to help with timing animations
-    framerate = 30
+
     min_scale = 0.05
     max_scale = 5
 
     def __init__(self, pos, size, font_name = pygame.font.get_default_font(), font_size = 22, groups = None, root = None, independent = False):
         #Tasks that are the same for all sub-classes
         self.updated = True
         self.children = []
@@ -73,344 +48,75 @@
         self.topleft = pos
         #Font size has to be set before font name, as setting font name prompts the font object to be built
         self.font_size = font_size
         self.font_name = font_name
         self.Add_to_group(groups)
         self.root = self if root is None else root
         if not independent:
-            self.Buttons.list_all.append(self)
+            Buttons.list_all.append(self)
         self.independent = independent
 
-
     def __str__(self):
         return f"{type(self).__name__} object"
     def __repr__(self):
-        return f"<{self.__str__()} at {self.topleft}>"
-
+        try:
+            return f"<{self.__str__()} at {self.topleft}>"
+        except AttributeError:
+            return f"Partially initialised <{self.__str__()}>"
 
 
-    @classmethod
-    def get_group(cls, group):
-        """
-        Returns all buttons inside the given group / groups.
-        """
-        #If a list of groups is given, return the buttons in all the groups combined.
-        if isinstance(group, (tuple, list)):
-            lst = []
-            for grp in group:
-                if grp in cls.groups:
-                    for button in cls.groups[grp]:
-                        #Append all buttons in the group to the original group, if it is not a duplicate
-                        if button not in lst:
-                            lst.append(button)
-                #Else, if the group is already a Button, append that Button to the list instead
-                elif isinstance(grp, Buttons):
-                    lst.append(grp)
-            return lst
-        #Select the correct button group
-        elif group is all: #If the group is the default 'all', return all buttons
-            return cls.list_all
-        elif group in cls.groups:
-            return cls.groups[group] #Return all buttons in the group.
-        elif isinstance(group, Buttons):
-            return [group]
-        else: #If the group doesn't exist, return an empty list
-            return []
-
     def Add_to_group(self, groups):
         """
-        Add a button to a group.
+        Add this button to a group.
         Allows for assignment of multiple groups simultaniously by passing in a list or tuple of groups.
         """
         if not isinstance(groups, (list, tuple)):
             groups = [groups]
         for grp in groups:
             if grp is None:
                 continue
             #Store the button in the global groups dict
-            if grp in self.Buttons.groups:
+            if grp in Buttons.groups:
                 #If the group exists, add self to the group, unless self is already in this group.
-                if not self in self.Buttons.groups[grp]:
-                    self.Buttons.groups[grp].append(self)
+                if not self in Buttons.groups[grp]:
+                    Buttons.groups[grp].append(self)
             #If the group doesn't exist, make a new group with self as the first list entry.
             else:
-                self.Buttons.groups[grp] = [self]
+                Buttons.groups[grp] = [self]
 
             #Track the joined groups in the buttons' own groups list
             if grp not in self.groups:
                 self.groups.append(grp)
 
     def Set_lock(self, claim = True):
         """
         Set the input lock (if possible).
         If claim = True, automatically set Buttons.input_claim as well.
         """
-        self.Buttons.input_processed = True
-        if not self.Buttons.input_lock and not self.independent:
-            self.Buttons.input_lock = self
+        Buttons.input_processed = True
+        if not Buttons._input_lock and not self.independent:
+            Buttons._input_lock = self
         if claim:
-            self.Buttons.input_claim = True
+            Buttons.input_claim = True
 
     def Release_lock(self, claim = True):
         """
         Release the input lock (if necessary / possible).
         If claim = True, automatically set Buttons.input_claim as well.
         """
-        self.Buttons.input_processed = False
-        if self is self.Buttons.input_lock and not self.independent:
-            self.Buttons.input_lock = None
+        Buttons.input_processed = True
+        if self is Buttons._input_lock and not self.independent:
+            Buttons._input_lock = None
         if claim:
-            self.Buttons.input_claim = True
+            Buttons.input_claim = True
 
     @classmethod
     def Claim_input(cls):
-        cls.Buttons.input_claim = True
-        cls.Buttons.input_processed = True
-
-
-    @classmethod
-    def Event(cls, event, group = all):
-        """
-        A method to handle all events a button might need to be informed of.
-        """
-        #Reset the input_claim and input_processed attributes
-        cls.input_claim = False
-        cls.input_processed = False
-
-        #Handle the Event appropriately
-        if not isinstance(event, pygame.event.EventType):
-            raise TypeError(f"Event should be type 'Event', not type {type(event).__name__}")
-        if event.type == pygame.MOUSEBUTTONDOWN:
-            if event.button == 1:
-                cls.LMB_down(event.pos, group)
-            elif event.button == 2:
-                return
-                cls.MMB_down(event.pos, group)
-            elif event.button == 3:
-                return
-                cls.RMB_down(event.pos, group)
-            elif event.button > 3:
-                cls.Scroll(cls.convert_scroll(event.button), event.pos, group)
-        elif event.type == pygame.MOUSEBUTTONUP:
-            if event.button == 1:
-                cls.LMB_up(event.pos, group)
-            elif event.button == 2:
-                return
-                cls.MMB_up(event.pos, group)
-            elif event.button == 3:
-                return
-                cls.RMB_up(event.pos, group)
-        elif event.type == pygame.KEYDOWN:
-            cls.Key_down(event, group)
-
-
-    @classmethod
-    def Update(cls, group = all):
-        """
-        A method that will run any updates that have to be performed each cycle, such as updating the cursor position for sliders.
-        """
-        if cls.input_lock:
-            if "Set_cursor_pos" in cls.input_lock.actions:
-                cls.Set_cursor_pos(pygame.mouse.get_pos(), group)
-
-
-    @classmethod
-    def LMB_down(cls, pos, group = all):
-        """
-        Left Mouse Button down; A.K.A. a normal click.
-        """
-        cls.input_claim = False
-        cls.input_processed = False
-        group_list = cls.get_group(group)
-
-        #If a button has claimed an input lock
-        if cls.input_lock in group_list:
-            if "LMB_down" in cls.input_lock.actions:
-                cls.input_lock.LMB_down(pos)
-                if cls.input_claim:
-                    return
-
-        for button in group_list:
-            if "LMB_down" in button.actions and button is not cls.input_lock:
-                button.LMB_down(pos)
-                if cls.input_claim:
-                    return
-        return
-
-
-    @classmethod
-    def LMB_up(cls, pos, group = all):
-        """
-        Left Mouse Button up; A.K.A. releasing a click.
-        """
-        cls.input_claim = False
-        cls.input_processed = False
-        group_list = cls.get_group(group)
-
-        #If a button has claimed an input lock
-        if cls.input_lock in group_list:
-            if "LMB_up" in cls.input_lock.actions:
-                cls.input_lock.LMB_up(pos)
-                if cls.input_claim:
-                    return
-
-        for button in group_list:
-            if "LMB_up" in button.actions and button is not cls.input_lock:
-                button.LMB_up(pos)
-                if cls.input_claim:
-                    return
-        return
-
-
-    @classmethod
-    def Scroll(cls, value, pos, group):
-        """
-        Handles all scroll events for all buttons.
-        """
-        cls.input_claim = False
-        cls.input_processed = False
-        group_list = cls.get_group(group)
-
-        if cls.input_lock in group_list:
-            if "Scroll" in cls.input_lock.actions:
-                cls.input_lock.Scroll(value, pos)
-                if cls.input_claim:
-                    return
-
-        for button in group_list:
-            #If the button hasn't been processed yet in the input_lock section, and has the "Scroll" attribute:
-            if "Scroll" in button.actions and button is not cls.input_lock:
-                button.Scroll(value, pos)
-                if cls.input_claim:
-                    return
-        return
-
-
-    @classmethod
-    def Key_down(cls, event, group = all):
-        """
-        Processes any KEYDOWN events for buttons which require these.
-        """
-        cls.input_processed = False
-        group_list = cls.get_group(group)
-        #If any button in the current scope requires keyboard inputs / has focus:
-        if cls.input_lock in group_list:
-            if "Key_down" in cls.input_lock.actions:
-                cls.input_lock.Key_down(event)
-        return
-
-
-    @classmethod
-    def Set_cursor_pos(cls, pos, group = all):
-        """
-        Updates the cursor position. Required for e.g. sliders.
-        """
-        group_list = cls.get_group(group)
-        if not cls.input_lock:
-            for button in group_list:
-                if "Set_cursor_pos" in button.actions:
-                    button.Set_cursor_pos(pos)
-        elif cls.input_lock in group_list:
-            if "Set_cursor_pos" in cls.input_lock.actions:
-                cls.input_lock.Set_cursor_pos(pos)
-
-
-    @classmethod
-    def convert_scroll(cls, value):
-        """
-        Converts a mouse button value into a scroll value.
-        Scrolling down gives negative scroll values.
-        """
-        if value < 4:
-            return 0
-        elif value % 2:
-            return round((value - 2) / 2) * cls.scroll_factor
-        else:
-            return round(-(value - 3) / 2) * cls.scroll_factor
-
-
-    @classmethod
-    def Scale(cls, scale, group = all, relative_scale = True, *, center = (0, 0), px_center = None):
-        """
-        Scales all buttons in the given group by / to a certain scaling factor.
-
-        relative_scale: bool - Determines whether the given scale value is absolute (Button.scale = val), or is a scaling factor relative to their current scale.
-        center: tuple - The absolute coordinates around which the scaling should take place.
-        px_center: Tuple - The display coordinates around which the scaling should take place. If these are passed in, the 'center' coordinates are ignored.
-        """
-        if not isinstance(scale, (float, int)):
-            raise TypeError(f"scale must be type 'int' or 'float', not type '{type(scale).__name__}'")
-        elif scale == 0:
-            raise ValueError(f"Cannot scale buttons to scale '0'")
-
-        if px_center:
-            px_center = cls.Verify_iterable(px_center, 2)
-        else:
-            center = cls.Verify_iterable(center, 2)
-
-        for button in cls.get_group(group):
-            if not relative_scale:
-                scale_factor = cls.Clamp(scale, button.min_scale, button.max_scale) / button.scale
-            else:
-                scale_factor = cls.Clamp(scale, button.min_scale / button.scale, button.max_scale / button.scale)
-            if px_center: #Transform the pixel coordinates to raw coordinates
-                center = tuple(i / button.scale for i in px_center)
-
-            #Apply the translation to make sure the given coordinates stay at the same place
-            button._move(tuple(i * (1 / scale_factor - 1) for i in center))
-
-            button.scale *= scale_factor
-
-    @classmethod
-    def Move(cls, offset, group = all, scale = False):
-        """
-        Moves all buttons in the given group by a certain offset.
-
-        offset: int / float / tuple - An number, or iterable containing two numbers, for how much the Buttons in the group should be moved. If a number is given, this movement is applied in both directions.
-        group: * - The group to which the translation should be applied.
-        scale: bool - Determines whether the given values should be scaled to the Buttons' scale before they are applied.
-        """
-        if hasattr(offset, "__iter__"):
-            cls.Verify_iterable(offset, 2, (int, float))
-        else:
-            offset = (offset, offset)
-        #Set the "button_offset" variable to prevent scaling to affect other buttons too.
-        b_offset = offset
-
-        for button in cls.get_group(group):
-            if scale:
-                b_offset = button.scaled(offset, False)
-            button._move(b_offset)
-
-
-    @classmethod
-    def Clear(cls, group = all):
-        """
-        Clears all user inputs from the buttons in the given group.
-
-        group: * - The group of Buttons which should be cleared.
-        """
-        for button in cls.get_group(group):
-            button.Clear()
-
-    @classmethod
-    def Draw(cls, screen, group = all):
-        """
-        Draw all buttons in the specified group to the screen / Surface provided.
-        """
-        #Select the correct button group
-        group_list = cls.get_group(group)
-        #Click all buttons without the "Cursor Lock".
-        for button in reversed(group_list):
-            if button is not cls.input_lock:
-                button.Draw(screen)
-        #Draw the button with the "Input Lock" last, to make it always appear on top.
-        if cls.input_lock:
-            if cls.input_lock in group_list:
-                cls.input_lock.Draw(screen)
+        Buttons.input_claim = True
+        Buttons.input_processed = True
 
 
     @classmethod
     def Align(cls, rect, limit_size, pos):
         """
         Creates an aligned Rect, with the given size when placed onto a surface with size 'limit_size'.
         Functionally just a wrapper around AlignX and AlignY.
@@ -480,15 +186,15 @@
         if isinstance(max, pygame.Rect):
             max = max.height
         pos = pos.lower()
 
         if "top" in pos:
             pass
         elif "bottom" in pos:
-            rect.right = max
+            rect.bottom = max
         else:
             rect.centery = math.floor(max / 2)
 
         return rect
 
 
     def contains(self, position):
@@ -747,113 +453,45 @@
             child.font_size = value
 
 
     def __Make_font(self):
         """
         Re-builds a font object based on self.font_name and self.font_size, as well as the current self.scale.
         """
+        self.__font = self.__get_font(self.font_name, round(self.scale * self.font_size))
+        return
+
+    @staticmethod
+    @weak_cache
+    def __get_font(name, size):
         #pygame.font.Font is used in favor of pygame.font.SysFont, as SysFont's font sizes are inconsistent with the value given for the font.
         try:
-            self.__font = pygame.font.Font(self.font_name, round(self.scale * self.font_size))
+            return pygame.font.Font(name, size)
         except FileNotFoundError:
-            font = pygame.font.match_font(self.font_name)
+            font = pygame.font.match_font(name)
             if font is None: #If no matching font was found
-                raise FileNotFoundError(f"No such font: '{self.font_name}'")
-            self.__font = pygame.font.Font(font, round(self.scale * self.font_size))
-
+                raise FileNotFoundError(f"No such font: '{name}'")
+            return pygame.font.Font(font, size)
 
     def _Call(self, action):
         """
         Calls a function, if it exists, for the action specified
         """
-        if not Buttons._callbacks:
+        if not self._callbacks:
             return
         root = self.root #Transfer the function call over to the Buttons' root
         if not action in root.functions: #If no function was specified for this action, ignore the fact that this function was called anyway
             return
-        if isinstance(root.functions[action], (tuple, list)):
-            root.functions[action][0](*(arg if arg != "*self*" else root for arg in root.functions[action][1:]))
-        else:
-            root.functions[action]()
+        with Buttons.Callbacks(False, False), Buttons.Update_flags(False, False):
+            if isinstance(root.functions[action], (tuple, list)):
+                root.functions[action][0](*(arg if arg != "*self*" else root for arg in root.functions[action][1:]))
+            else:
+                root.functions[action]()
         return
 
-    class Callbacks:
-        """
-        Whether Buttons should trigger function callbacks on events
-
-        value: Whether function calls should be enabled. Can be any of:
-            True / Truthy - All state changes trigger function calls.
-            False / Falsy (except None) - No functions are called, regardless of the originator.
-            None (Default behavior): Disables enforcement, meaning only event based changes trigger functions.
-
-        enforce: Whether the rule should be enforced for all nested statements. Note: nested statements with enforce = True will still overwrite this.
-        """
-        suppressor = None #A reference to the currently enforcing flag
-        def __init__(self, value, enforce = True, /):
-            #Store the initial value and suppressor to set them back upon __exit__ (if called)
-            self.__prev_value = Buttons._callbacks
-            self.__prev_suppressor = Buttons.Callbacks.suppressor
-            #Clearing the flag (set to default)
-            if value is None:
-                Buttons.Callbacks.suppressor = None
-                Buttons._callbacks = False #False by default, unless set to true by events' with statement
-            #Setting the flag as enforcer
-            elif enforce:
-                Buttons._callbacks = value
-                Buttons.Callbacks.suppressor = self
-            #Setting the flag, without becoming the enforcer
-            elif Buttons.Callbacks.suppressor is None:
-                Buttons._callbacks = value
-            #else: Do nothing. This instance is not enforcing, and a pre-existing instance is, so that one takes precedence.
-        def __enter__(self):
-            #Don't do anything inside __enter__(). All actions are already done in __init__().
-            pass
-        def __exit__(self, exc_type, exc_val, exc_tb):
-            if self is Buttons.Callbacks.suppressor or Buttons.Callbacks.suppressor is None:
-                Buttons._callbacks = self.__prev_value
-                #Remove self as the suppressor, since we exit the scope of this with value
-                Buttons.Callbacks.suppressor = self.__prev_suppressor
-
-
-    class Update_flags:
-        """
-        Whether Buttons should update the event flags
-
-        value: Whether event flag updates should be enabled. Can be any of:
-            True / Truthy - All state changes trigger function calls.
-            False / Falsy (except None) - No functions are called, regardless of the originator.
-            None (Default behavior): Disables enforcement, meaning only event based changes trigger functions.
-
-        enforce: Whether the rule should be enforced for all nested statements. Note: nested statements with enforce = True will still overwrite this.
-        """
-        suppressor = None #A reference to the currently enforcing flag
-        def __init__(self, value, enforce = True, /):
-            self.__prev_value = Buttons._update_flags
-            self.__prev_suppressor = Buttons.Update_flags.suppressor
-            #Clearing the flag (set to default)
-            if value is None:
-                Buttons.Update_flags.suppressor = None
-                Buttons._update_flags = False #False by default, unless set to true by events' with statement
-            #Setting the flag as enforcer
-            elif enforce:
-                Buttons._update_flags = value
-                Buttons.Update_flags.suppressor = self
-            #Setting the flag, without becoming the enforcer
-            elif Buttons.Update_flags.suppressor is None:
-                Buttons._update_flags = value
-            #else: Do nothing. This instance is not enforcing, and a pre-existing instance is, so that one takes precedence.
-        def __enter__(self):
-            #Don't do anything inside __enter__(). All actions are already done in __init__().
-            pass
-        def __exit__(self, exc_type, exc_val, exc_tb):
-            if self is Buttons.Update_flags.suppressor or Buttons.Update_flags.suppressor is None:
-                Buttons._update_flags = self.__prev_value
-                #Remove self as the suppressor, since we exit the scope of this with value
-                Buttons.Update_flags.suppressor = self.__prev_suppressor
-
 
     @property
     def functions(self):
         return self.__functions
     @functions.setter
     def functions(self, value):
         self.__functions = self.Verify_functions(value)
@@ -1069,12 +707,7 @@
             else:
                 return value * self.scale
         else:
             raise TypeError(f"Cannot scale type '{type(value).__name__}'.")
 
     def relative(self, pos):
         return self.offset(pos, self.scaled(self.topleft, False), (-1, -1))
-
-
-#Add an attribute to this class that references itself, so other subclasses can easily acces the parent class object
-#This is useful for allowing communications between subclasses
-Buttons.Buttons = Buttons
```

### Comparing `pygbuttons-0.9.3/src/pygbuttons/Button.py` & `pygbuttons-0.9.4/src/pygbuttons/Button.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from .Base import Buttons
+from .Base import ButtonBase
+from .Control import Buttons
 
 import os
 os.environ["PYGAME_HIDE_SUPPORT_PROMPT"] = ""
 import pygame
 import math
 
 
-class Button(Buttons):
+class Button(ButtonBase):
     """
     Creates a Button, an object which can detect Left Mouse Button inputs from the user.
 
     pos: (left, top) - The topleft position before scaling.
     size: (width, height) - The size before scaling.
-    text: str -
+    text: str - The text to be displayed on the Button.
     mode: str - "None": Does not change *.value when clicked. Will set *.clicked and execute any assigned functions.
               - "Count": Count the number of inputs that have occured.
               - "Toggle": Toggle value from True to False and back.
               - "Hold": Stays True until the Mouse Button is released.
     orientation: int - The orientation of the text. If orientation == 0, the text will be horizontal; if orientation == 1, the text will be vertical.
     style: "Square", "Round", int - Defines the radius of curvature of the buttons' corners.
     font_name: str - The name of the font that should be used for the Button.
@@ -41,24 +42,25 @@
     *.value: int, bool - The current state of the button.
 
     Outputs:
     *.value: int, bool - The current state in the Button. If mode == "count", the amount of times (int) the Button was clicked. If mode == "Toggle" or "hold", whether the button is currently in the pressed / down state (bool).
     *.clicked: bool - Whether the Button has been set to a new state since the last time this variable was checked. Automatically resets once it is querried.
     *.moved: bool - Whether the Button has been dragged to a different location since the last time this variable was checked. Automatically resets once it is querried.
     """
-    actions = ["LMB_down", "LMB_up", "RMB_down", "Set_cursor_pos"]
+    actions = ["LMB_down", "LMB_up", "Set_cursor_pos", "Mouse_motion"]
     def __init__(self, pos, size,
                  text = "",
                  mode = "None",
                  orientation = 0,
                  style = "Square",
                  font_name = pygame.font.get_default_font(),
                  font_size = 22,
                  text_colour = (0, 0, 0),
                  text_align = "Center",
+                 text_offset = "auto",
                  background = (255, 255, 255),
                  border = ((63, 63, 63), 1, 0),
                  accent_background = (220, 220, 220),
                  dragable = (False, False),
                  limits = (None, None, None, None),
                  snap = ((), (), 0),
                  functions = {},
@@ -87,55 +89,75 @@
         self.text_align = text_align
         self.bg = self.Verify_background(background)
         if accent_background:
             self.accent_bg = self.Verify_background(accent_background)
         else:
             self.accent_bg = self.bg
         self.border = self.Verify_border(border)
+
+        #Set the offset the text has from the sides of the text_box
+        if isinstance(text_offset, int):
+            self.text_offset = 2 * (text_offset,)
+        elif not isinstance(text_offset, str):
+            self.text_offset = self.Verify_iterable(text_offset, 2)
+        elif text_offset.lower() == "auto":
+            #The automatic offset is calculated as 0.25 * font_size + (border_width + border_offset if there is a border)
+            #Offset is not 0 if no border is given, to be consistent with TextBox Buttons
+            #It can of course still be 0 if the user sets text_offset = 0
+            self.text_offset = 2 * (round(self.font_size / 4) + ((self.border[1] + self.border[2]) if self.border else 0),)
+
         self.dragable = self.Verify_iterable(dragable, 2, bool)
         limits = self.Verify_iterable(limits, 4)
         self.limits = list(value if value is not None else ( (-1) ** (i + 1) * math.inf) for i, value in enumerate(limits))
         self.snap = self.Verify_iterable(snap, 3)
         self.moved = False
         self.clicked = False
         self.Draw(pygame.Surface((1, 1))) #Makes sure all attributes are prepared and set-up correctly
 
 
     def LMB_down(self, pos):
         if self.contains(pos):
             with Buttons.Callbacks(True, False), Buttons.Update_flags(True, False):
                 if self.mode == "none":
                     self._Call("Click") #Call "Click" separately since "none" does not change self.value
-                    if Buttons._update_flags:
+                    if self._update_flags:
                         self.clicked = True
                 elif self.mode == "count":
                     self.value += 1
                 elif self.mode == "toggle":
                     self.value = not self.value
                 elif self.mode == "hold":
                     self.Set_lock()
                     self.value = True
                     if any(self.dragable):
                         self.drag_pos = self.relative(pos)
                 self.Claim_input()
             return
 
     def LMB_up(self, pos):
-        if any(self.dragable):
-            self.Set_cursor_pos(pos)
         if self.mode == "hold" and self.value:
             with Buttons.Callbacks(True, False), Buttons.Update_flags(True, False):
                 self.value = False
                 self.Release_lock()
         return
 
-    def Set_cursor_pos(self, pos):
+    def Mouse_motion(self, event):
+        """
+        If the button supports dragging, this function is used to move the button to a new position.
+
+        event: pygame.event.EventType, tuple - The event or global position the cursor moved to.
+        """
+        # If required, extract the position from the event
+        if isinstance(event, pygame.event.EventType):
+            pos = event.pos
+        else:
+            pos = event
+
         if self.value:
             if any(self.dragable):
-                topleft = self.topleft
                 hori, verti = self.offset(self.relative(pos), self.drag_pos, (-1, -1)) #Determine the offsets of the cursor from where the user originally clicked
 
                 left = self.left + hori / self.scale * self.dragable[0] #Scale the offsets down to the original scale
                 top = self.top + verti / self.scale * self.dragable[1]
                 #Perform snapping
                 distances = sorted(zip((abs(left - snap_point) for snap_point in self.snap[0]), self.snap[0]))
                 if distances: #If there are any snap point:
@@ -147,19 +169,21 @@
                 if distances: #If there are any snap point:
                     closest = distances[0]
                     if closest[0] <= self.snap[2]: #If the distance <= the snapping range
                         top = round(closest[1]) #Snap!
                 #Confine the button within the limits
                 self.left = self.Clamp(left, self.limits[0], self.limits[1] - self.width)
                 self.top = self.Clamp(top, self.limits[2], self.limits[3] - self.height)
-                if self.topleft != topleft: #If the Button moved:
-                    with Buttons.Callbacks(True, False), Buttons.Update_flags(True, False):
-                        self._Call("Move")
-                        if Buttons._update_flags:
-                            self.moved = True
+                with Buttons.Callbacks(True, False), Buttons.Update_flags(True, False):
+                    self._Call("Move")
+                    if self._update_flags:
+                        self.moved = True
+
+    def Set_cursor_pos(self, pos):
+        self.Mouse_motion(pos)
 
 
     def Scale(self, scale, relative_scale = True, *, center = (0, 0), px_center = None):
         super().Scale(scale, self, relative_scale, center = center, px_center = px_center)
 
 
     def Move(self, offset, scale = False):
@@ -183,22 +207,24 @@
                 self.surface = self.Make_background_surface(self.accent_bg)
             #Draw a border, if it is enabled
             if self.border:
                 self.Draw_border(self.surface, *self.border)
             #Draw the text onto the surface
             if self.text:
                 #Make a surface that fits within the border
-                text_offset = self.scaled(self.border[1] + self.border[2] + self.font_size / 4 if self.border else self.font_size / 4)
-                text_limiter = pygame.Surface(self.Clamp(self.offset(self.true_size, 2 * (text_offset,), (-2, -2)), 0, math.inf), pygame.SRCALPHA)
+                text_offset = self.scaled(self.text_offset)
+                text_limiter = pygame.Surface(self.Clamp(self.offset(self.true_size, text_offset, (-2, -2)), 0, math.inf), pygame.SRCALPHA)
                 limiter_rect = text_limiter.get_rect()
                 text_surface = self.font.render(self.text, True, self.text_colour)
 
                 if self.orientation:
                     text_surface = pygame.transform.rotate(text_surface, -90 * self.orientation)
                 text_rect = text_surface.get_rect()
+                if not "bottom" in self.text_align:
+                    text_rect.height = self.font.get_height()
                 #Align the text properly
                 self.Align(text_rect, limiter_rect, self.text_align)
                 #Blit the text to the limiter surface, and then onto the screen
                 text_limiter.blit(text_surface, text_rect)
                 limiter_rect.center = self.middle
                 self.surface.blit(text_limiter, limiter_rect)
 
@@ -240,15 +266,15 @@
     def value(self, value):
         self.__value = value
         if value:
             self._Call("Click")
         else:
             self._Call("Release")
         self.updated = True
-        if Buttons._update_flags:
+        if self._update_flags:
             self.clicked = True
 
     @property
     def clicked(self):
         clicked_ = self.__clicked
         self.__clicked = False
         return clicked_
```

### Comparing `pygbuttons-0.9.3/src/pygbuttons/DropdownBox.py` & `pygbuttons-0.9.4/src/pygbuttons/DropdownBox.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from .Base import Buttons
+from .Base import ButtonBase
+from .Control import Buttons
 from .Button  import Button
 from .Slider import Slider
 
 import os
 os.environ["PYGAME_HIDE_SUPPORT_PROMPT"] = ""
 import pygame
 
 
-class DropdownBox(Buttons):
+class DropdownBox(ButtonBase):
     """
     Creates a DropdownBox, in which a user can select an input from a list of options.
 
     pos: (left, top) - The topleft position before scaling.
     size: (width, height) - The size before scaling.
     options: list, tuple - A list containing the values of all options to be added to the DropdownBox.
     hint: str - The text that is displayed in the main box when no option is selected.
@@ -49,15 +50,15 @@
     *.value: * - The value of the currently selected item. Type can be wathever was given as the value.
     *.state: int - The index of the currently selected option. Is -1 if no option is selected.
     *.new_state: bool - Whether the DropdownBox has been set to a new state since the last time this variable was checked. Automatically resets once it is querried.
 
     *.is_selected: bool - Whether this DropdownBox object is selected at this point in time. I.E. Whether DropdownBox is expanded.
     *.clicked: bool - Whether the DropdownBox has been clicked anywhere (except the scroll bar), thus changing from selected to deselected (or vice versa).
     """
-    actions = ["LMB_down", "LMB_up", "Set_cursor_pos", "Scroll"]
+    actions = ["LMB_down", "LMB_up", "Set_cursor_pos", "Scroll", "Mouse_motion"]
     def __init__(self, pos, size,
                  options = [],
                  hint = "",
                  option_align = "center",
                  value_align = "left",
                  hint_align = "left", #Align left for consistency with text boxes
                  display_length = 0,
@@ -166,26 +167,31 @@
                 self.is_selected = False
 
     def LMB_up(self, pos):
         if self.is_selected and self.scroll_bar:
             with Buttons.Update_flags(True, True):
                 self.scroll_bar.LMB_up(pos)
 
+    def Mouse_motion(self, pos):
+        if self.is_selected and self.scroll_bar:
+            with Buttons.Update_flags(True, True):
+                self.scroll_bar.Mouse_motion(pos)
+
     def Set_cursor_pos(self, pos):
         if self.is_selected and self.scroll_bar:
             with Buttons.Update_flags(True, True):
                 self.scroll_bar.Set_cursor_pos(pos)
 
 
     def Scroll(self, value, pos):
         if self.arrow.value: #If self is selected / the menu is expanded downwards
             if self.contains(pos):
                 pass
             elif self.is_within(pos, (self.scaled(self.left), self.scaled(self.bottom) + self.scaled(self.spacing[1])), (self.scaled(self.right), self.scaled(self.bottom) + self.scaled(self.spacing[1]) + self._true_pixel_length)): #If the position lies withing the expanded section, perform scrolling.
-                self.scrolled_px += self.Buttons.scroll_factor * value
+                self.scrolled_px += Buttons.scroll_factor * value
                 self.Claim_input()
 
 
     def Scale(self, scale, relative_scale = True, *, center = (0, 0), px_center = None):
         super().Scale(scale, self, relative_scale, center = center, px_center = px_center)
 
 
@@ -435,15 +441,15 @@
             self.__state = -1
             self.main_button.text = self.hint
             self.main_button.text_colour = self.hint_colour
             self.main_button.text_align = self.hint_align
         self.updated = True
         self._moved = True
         self._Call("Update")
-        if Buttons._update_flags:
+        if self._update_flags:
             self.new_state = True
 
 
     @property
     def new_state(self):
         new_state = self.__new_state
         self.__new_state = False
@@ -510,15 +516,15 @@
         else:
             self.arrow.value = False
             self.scrolled = 0
             self._moved = True
             self.Release_lock(False)
             self._Call("Deselect")
         self.updated = True
-        if Buttons._update_flags:
+        if self._update_flags:
             self.clicked = True
 
 
     @property
     def option_align(self):
         return self.__option_align
     @option_align.setter
```

### Comparing `pygbuttons-0.9.3/src/pygbuttons/Slider.py` & `pygbuttons-0.9.4/src/pygbuttons/Slider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from .Base import Buttons
+from .Base import ButtonBase
+from .Control import Buttons
 from .Button import Button
 
 import os
 os.environ["PYGAME_HIDE_SUPPORT_PROMPT"] = ""
 import pygame
 
 
-class Slider(Buttons):
+class Slider(ButtonBase):
     """
     Creates a Slider, which allows the user to input a value within a given range.
 
     pos: (left, top) - The topleft position before scaling.
     size: (width, height) - The size before scaling.
     value_range: (a, b) - The range between which values the slider should (linearly) interpolate.
     orientation: "auto", int - The orientation of the Slider. In case orientation == "auto", the longest direction will be seen as the primary direction. If orientation == 0, the Slider will be horizontal; if orientation == 1, the Slider will be vertical.
@@ -45,15 +46,15 @@
 
     Outputs:
     *.value: float - The current value of the slider.
     *.moved: bool - Whether the slider has been moved since the last time this property has been checked. Automatically resets once it is querried.
 
     *.is_selected: bool - Whether this Slider object is selected at this point in time. I.E. Whether the user is currently moving the Slider.
     """
-    actions = ["LMB_down", "LMB_up", "Set_cursor_pos"]
+    actions = ["LMB_down", "LMB_up", "Set_cursor_pos", "Mouse_motion"]
     def __init__(self, pos, size,
                  value_range = (0, 1),
                  start_value = 0,
                  orientation = "auto", #0 for horizontal, 1 for vertical
                  style = "Square",
                  #Background settings
                  background = (255, 255, 255), #Colour or pygame.Surface
@@ -90,15 +91,15 @@
         self.__value_range = self.Verify_iterable(value_range, 2) #Directly written to the private property, to prevent a chicken - egg problem with self.value
         if isinstance(orientation, int):
             self.orientation = orientation
         elif orientation.lower() == "auto":
             self.orientation = int(self.width < self.height)
         self.style = style
         #Set the background parameters for the Slider
-        self.bg = self.Buttons.Verify_background(background)
+        self.bg = self.Verify_background(background)
         self.border = self.Verify_border(border)
 
         #Initialise any markers - Has to be done before making the slider object
         if markings == 1 and edge_markings:
             raise ValueError("Edge markings require at least 2 markings to be present")
         self.markings = markings
         self.edge_markings = edge_markings
@@ -121,40 +122,50 @@
     def LMB_down(self, pos):
         if self.slider.contains(pos):
             self.slider.LMB_down(pos)
             self.Set_lock()
             self._moved = True #Instruct the button that value is no longer equal to the value stored in __value
             with Buttons.Callbacks(True, False), Buttons.Update_flags(True, False):
                 self.is_selected = True
-                if Buttons._update_flags:
+                if self._update_flags:
                     self.moved = True
         elif self.contains(pos):
             #Move the slider to where we clicked (within limits of course)
             self.slider.LMB_down(self.slider.scaled(self.slider.center))
-            self.Set_cursor_pos(pos)
+            self._moved = True
+            self.slider.Mouse_motion(pos)
             self.Set_lock()
             with Buttons.Callbacks(True, False), Buttons.Update_flags(True, False):
                 self.is_selected = True
-                if Buttons._update_flags:
+                if self._update_flags:
                     self.moved = True
 
     def LMB_up(self, pos):
         if self.is_selected:
             self.slider.LMB_up(pos)
             with Buttons.Callbacks(True, False), Buttons.Update_flags(True, False):
                 self.is_selected = False
 
+    def Mouse_motion(self, event):
+        if self.is_selected:
+            slider_pos = self.slider.topleft
+            self._moved = True
+            self.slider.Mouse_motion(event)
+            with Buttons.Callbacks(True, False), Buttons.Update_flags(True, False):
+                if self._update_flags:
+                    self.moved = True
+
     def Set_cursor_pos(self, pos):
         if self.is_selected:
             slider_pos = self.slider.topleft
             self.slider.Set_cursor_pos(pos)
             if self.slider.topleft != slider_pos:
                 self._moved = True
                 with Buttons.Callbacks(True, False), Buttons.Update_flags(True, False):
-                    if Buttons._update_flags:
+                    if self._update_flags:
                         self.moved = True
 
 
     def Scale(self, scale, relative_scale = True, *, center = (0, 0), px_center = None):
         super().Scale(scale, self, relative_scale, center = center, px_center = px_center)
 
 
@@ -253,19 +264,21 @@
             self.value_range = tuple(range) #Update the slider range
         self.value = self.Clamp(self.value, *sorted(self.value_range)) #Reset the value, to update the sliders' position
 
     def Set_slider_primary(self, value, limit_size = True):
         """
         Set the sliders' primary dimension / size (in the direction of travel).
         Set_slider_primary(value).
-        If limit_size == True, the primary dimension cannot go below 1/2 the secondary dimension. This is to prevent the slider from disappearing completely if the primary is set too low.
+        If limit_size == True, the primary dimension cannot go below 1/2 the secondary dimension, nor above the Slider bars' primary dimension. This is to prevent the slider from disappearing completely if the primary is set too low.
         """
         if limit_size:
-            #Make sure the slider primary can not accidentally be set too low.
-            value = max(value, round(self.rotated(self.slider.size)[1] / 2))
+            #Make sure the slider primary can not accidentally be set too low or too high.
+            value = min(max(value, round(self.rotated(self.slider.size)[1] / 2)), self.rotated(self.size)[0])
+            # Note: min(max()) is used instead of Clamp since it is possible that the lower_limit > upper_limit
+            # In this case, the upper limit is seen as more important, since exceeding this limit can result in a crash
         self.value #Flush any _moved arguments, in case they haven't been processed yet.
         if self.orientation % 2: #Update the sliders' size
             if self.slider.height != value:
                 self.slider.height = value
         else:
             if self.slider.width != value:
                 self.slider.width = value
@@ -280,20 +293,20 @@
     def is_selected(self):
         return self.__is_selected
     @is_selected.setter
     def is_selected(self, value):
         if value: #If the user selects the text box:
             self.__is_selected = True
             self.Set_lock()
-            if Buttons._update_flags:
+            if self._update_flags:
                 self.clicked = True
         else: #If the user deselects the box:
             self.__is_selected = False
             self.Release_lock()
-            if Buttons._update_flags:
+            if self._update_flags:
                 self.clicked = True
 
     @property
     def value(self):
         #Note: No need to run ._Call() anywhere in this code. The fact that the .__value is only updated here isn't important. It was already called by the slider when it was actually moved.
         if self._moved: #If the user clicked on the slider, the value should be re-calculated from the slider position. If not, the value should be exactly what the user set.
             pos = round(self.rotated(self.offset(self.slider.topleft, self.topleft, (-1, -1)))[0])
@@ -311,15 +324,15 @@
             self.slider.center = self.center
         else:
             coord_range = self.rotated(self.size)[0] - self.rotated(self.slider.size)[0] #The available pixels for the slider to move in
             self.slider.topleft = self.rotated(self.rotated(self.topleft)[0] + (val - self.value_range[0]) / (self.value_range[1] - self.value_range[0]) * coord_range, self.rotated(self.center)[1] - self.rotated(self.slider.size)[1] / 2)
         self.__value = val
         self._moved = False
         self._Call("Move")
-        if Buttons._update_flags:
+        if self._update_flags:
             self.moved = True
 
 
     @property
     def value_range(self):
         return self.__value_range
     @value_range.setter
```

### Comparing `pygbuttons-0.9.3/src/pygbuttons/Text.py` & `pygbuttons-0.9.4/src/pygbuttons/Text.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from .Base import Buttons
+from .Base import ButtonBase
+from .Control import Buttons
 from .Slider import Slider
 
 import os
 os.environ["PYGAME_HIDE_SUPPORT_PROMPT"] = ""
 import pygame
 import math
 
 
-class Text(Buttons):
+class Text(ButtonBase):
     """
     A simple (multi-line) text object, with scrolling support.
 
     pos: (left, top) - The topleft position before scaling.
     size: (width, height) - The size before scaling.
     text: str - The text that will be rendered to the surface.
     style: "Square", "Round", int - Defines the radius of curvature of the buttons' corners.
@@ -36,15 +37,15 @@
     *.write(value) - Appends text to self.text. Allows this button to be used as an output for e.g. the print() function.
 
     Outputs:
     *.value: str - Synonymous with *.text.
     *.text: str - The current text being rendered to the surface.
     *.lines: tuple - The current text being rendered to the surface, as it is split to prevent it from exceeding the Surface borders.
     """
-    actions = ["Scroll", "LMB_down", "LMB_up", "Set_cursor_pos"]
+    actions = ["Scroll", "LMB_down", "LMB_up", "Set_cursor_pos", "Mouse_motion"]
     def __init__(self, pos, size,
                  text = "",
                  style = "Square",
                  font_name = pygame.font.get_default_font(),
                  font_size = 22,
                  text_colour = (0, 0, 0),
                  text_align = "topleft",
@@ -74,15 +75,15 @@
             self.text_offset = 2 * (text_offset,)
         elif not isinstance(text_offset, str):
             self.text_offset = self.Verify_iterable(text_offset, 2)
         elif text_offset.lower() == "auto":
             #The automatic offset is calculated as 0.25 * font_size + (border_width + border_offset if there is a border)
             #Offset is not 0 if no border is given, to be consistent with TextBox Buttons
             #It can of course still be 0 if the user sets text_offset = 0
-            self.text_offset = 2 * (round(self.font_size / 4) + ((border[1] + border[2]) if self.border else 0),)
+            self.text_offset = 2 * (round(self.font_size / 4) + ((self.border[1] + self.border[2]) if self.border else 0),)
 
         if scroll_bar:
             self.scroll_bar = Make_scroll_bar(self, scroll_bar)
             self.children.append(self.scroll_bar)
         else:
             self.scroll_bar = None
         self.__scrolled = 0
@@ -93,37 +94,43 @@
 
 
     def LMB_down(self, pos):
         if self.scroll_bar:
             #Force flags to True, since flags are used internally to check for movement
             with Buttons.Update_flags(True, True):
                 self.scroll_bar.LMB_down(pos)
-            if self.Buttons.input_claim: #If the slider contained the position, and now claimed the input, set self as the lock
+            if Buttons.input_claim: #If the slider contained the position, and now claimed the input, set self as the lock
                 self.Set_lock()
 
 
     def LMB_up(self, pos):
         if self.scroll_bar:
             with Buttons.Update_flags(True, True):
                 self.scroll_bar.LMB_up(pos)
-            if self.Buttons.input_claim:
+            if Buttons.input_claim:
                 self.Release_lock()
 
 
+    def Mouse_motion(self, pos):
+        if self.scroll_bar:
+            with Buttons.Update_flags(True, True):
+                self.scroll_bar.Mouse_motion(pos)
+
+
     def Set_cursor_pos(self, pos):
         if self.scroll_bar:
             with Buttons.Update_flags(True, True):
                 self.scroll_bar.Set_cursor_pos(pos)
 
 
     def Scroll(self, value, pos):
         if not self.contains(pos): #If the mouse was not within the text box:
             return
         with Buttons.Callbacks(True, False), Buttons.Update_flags(True, False):
-            self.scrolled_px += self.Buttons.scroll_factor * value
+            self.scrolled_px += Buttons.scroll_factor * value
         self.Claim_input()
 
 
     def Scale(self, scale, relative_scale = True, *, center = (0, 0), px_center = None):
         super().Scale(scale, self, relative_scale, center = center, px_center = px_center)
 
 
@@ -322,15 +329,16 @@
                 else: #If the word is too long to fit on the line:
                     lines.append(line_string.rstrip(" "))
                     line_string = word #Place it on the next line.
             #Once all words are exhausted, append the remaining string to lines as well
             lines.append(line_string.rstrip(" "))
         self.__lines = tuple(lines)
 
-        self.text_px_height = len(self.lines) * font_height - self.text.count("\r") * math.ceil(font_height / 2)
+        # Conditional part to account for text sometimes being larger than the font size
+        self.text_px_height = len(self.lines) * font_height - self.text.rstrip("\n\r").count("\r") * math.ceil(font_height / 2) + (self.font.size(self.lines[-1])[1] - font_height if self.lines else 0)
 
         if self.scroll_bar:
             self.scroll_bar.Set_slider_primary(round(self.scroll_bar.height * min(1, (self.height - 2 * self.text_offset[1]) / self.text_px_height)))
 
         self.scrolled += 0 #Update the 'scrolled' value, to take into account that after rebuilding, the length of 'lines' might be different
 
     @property
```

### Comparing `pygbuttons-0.9.3/src/pygbuttons/TextBox.py` & `pygbuttons-0.9.4/src/pygbuttons/TextBox.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from .Base import Buttons
+from .Base import ButtonBase
+from .Control import Buttons
 
 import os
 os.environ["PYGAME_HIDE_SUPPORT_PROMPT"] = ""
 import pygame
 
 
-class TextBox(Buttons):
+class TextBox(ButtonBase):
     """
     Creates a TextBox, in which a user can input text.
 
     pos: (left, top) - The topleft position before scaling.
     size: (width, height) - The size before scaling.
     hint: str - The text that will be shown if no text is input by the user.
     style: "Square", "Round", int - Defines the radius of curvature of the buttons' corners.
@@ -138,46 +139,47 @@
             else:
                 with Buttons.Callbacks(True, False), Buttons.Update_flags(True, False):
                     self._is_selected = True
                 self.cursor = len(self._text)
         elif self._is_selected:
             with Buttons.Callbacks(True, False), Buttons.Update_flags(True, False):
                 self._is_selected = False
-            self.Buttons.input_processed = True
+            Buttons.input_processed = True
 
         return
 
 
     def Key_down(self, event):
-        if event.key in (pygame.K_RETURN, pygame.K_ESCAPE):
-            with Buttons.Callbacks(True, False), Buttons.Update_flags(True, False):
-                self._is_selected = False
-        elif event.key == pygame.K_BACKSPACE:
-            with Buttons.Callbacks(True, False), Buttons.Update_flags(True, False):
-                self._text = self._text[:max(self.cursor - 1, 0)] + self._text[self.cursor:]
-            #Move the cursor back one item
-            self.cursor -= 1
-        elif event.key == pygame.K_DELETE:
-            with Buttons.Callbacks(True, False), Buttons.Update_flags(True, False):
-                self._text = self._text[:self.cursor] + self._text[self.cursor + 1:]
-        elif event.key == pygame.K_LEFT:
-            self.cursor -= 1
-        elif event.key == pygame.K_RIGHT:
-            self.cursor += 1
-        elif event.unicode:
-            with Buttons.Callbacks(True, False), Buttons.Update_flags(True, False):
-                self._text = self._text[:self.cursor] + event.unicode + self._text[self.cursor:]
-            #Scroll the item sideways
-            #self.text_scroll += self.font.size(event.unicode)[0]
-            self.cursor += 1
-        else:
+        if self._is_selected:
+            if event.key in (pygame.K_RETURN, pygame.K_ESCAPE):
+                with Buttons.Callbacks(True, False), Buttons.Update_flags(True, False):
+                    self._is_selected = False
+            elif event.key == pygame.K_BACKSPACE:
+                with Buttons.Callbacks(True, False), Buttons.Update_flags(True, False):
+                    self._text = self._text[:max(self.cursor - 1, 0)] + self._text[self.cursor:]
+                #Move the cursor back one item
+                self.cursor -= 1
+            elif event.key == pygame.K_DELETE:
+                with Buttons.Callbacks(True, False), Buttons.Update_flags(True, False):
+                    self._text = self._text[:self.cursor] + self._text[self.cursor + 1:]
+            elif event.key == pygame.K_LEFT:
+                self.cursor -= 1
+            elif event.key == pygame.K_RIGHT:
+                self.cursor += 1
+            elif event.unicode:
+                with Buttons.Callbacks(True, False), Buttons.Update_flags(True, False):
+                    self._text = self._text[:self.cursor] + event.unicode + self._text[self.cursor:]
+                #Scroll the item sideways
+                #self.text_scroll += self.font.size(event.unicode)[0]
+                self.cursor += 1
+            else:
+                return
+            #Inform Buttons that the input has been processed / used
+            self.Claim_input()
             return
-        #Inform Buttons that the input has been processed / used
-        self.Buttons.input_processed = True
-        return
 
 
     def Scale(self, scale, relative_scale = True, *, center = (0, 0), px_center = None):
         super().Scale(scale, self, relative_scale, center = center, px_center = px_center)
 
 
     def Move(self, offset, scale = False):
@@ -214,17 +216,17 @@
             #Add the text to the surface
             text_limiter = pygame.Surface(self.offset(self.true_size, self.scaled(self.text_offset), (-2, -2)), pygame.SRCALPHA)
             limiter_rect = text_limiter.get_rect()
             if self._text:
                 text_surface = self.font.render(self._text, True, self.text_colour)
             else:
                 text_surface = self.font.render(self.hint, True, self.hint_colour)
-            text_rect = text_surface.get_rect()
             #Align the text rect
-            text_rect = self.AlignY(text_rect, limiter_rect, self.text_align)
+            text_rect = self.AlignY(self.font.get_height(), limiter_rect, self.text_align)
+            text_rect.width = text_surface.get_width()
             if text_rect.width < limiter_rect.width:
                 #If the text is smaller than the limiter, perform alignment in the X direction
                 #Available width -= 1 to account for the cursor potentially being on the right side of the text
                 self.AlignX(text_rect, limiter_rect.width - 1, self.text_align)
             else:
                 #If the text is wider than the limiter, all alignment is taken care of inside text_scroll
                 text_rect.left = - self.text_scroll
@@ -244,16 +246,16 @@
             self.cursor_surface.blit(text_limiter, limiter_rect)
 
             #Clear self.updated again, as the surface has been remade.
             self.updated = False
 
         if self._is_selected:
             #Update the cursor animation
-            self.cursor_animation = (self.cursor_animation + 1) % self.framerate
-        if self.cursor_animation < round(self.framerate / 2):
+            self.cursor_animation = (self.cursor_animation + 1) % Buttons.framerate
+        if self.cursor_animation < Buttons.framerate // 2:
             screen.blit(self.cursor_surface, pos)
         else:
             screen.blit(self.surface, pos)
         return
 
     @property
     def is_selected(self):
@@ -275,15 +277,15 @@
             self.Set_lock()
             self._Call("Select")
             if self._update_flags:
                 self.selected = True
         else:
             self.__is_selected = False
             self.cursor = 0
-            self.cursor_animation = self.framerate
+            self.cursor_animation = Buttons.framerate
             self.Release_lock(False) #Release without claiming the input
             self._Call("Deselect")
             if self._update_flags:
                 self.deselected = True
 
 
     @property
@@ -301,15 +303,15 @@
     def cursor(self):
         return self.__cursor
 
     @cursor.setter
     def cursor(self, value):
         #Make sure the cursor cannot be set to negative points, nor can it go further than directly after the last character.
         self.__cursor = self.Clamp(int(value), 0, len(self._text))
-        self.cursor_animation = self.framerate - 1
+        self.cursor_animation = Buttons.framerate - 1
         self.updated = True
         self.update_scroll()
 
 
     @property
     def text_scroll(self):
         return self.__text_scroll
```

### Comparing `pygbuttons-0.9.3/src/pygbuttons.egg-info/PKG-INFO` & `pygbuttons-0.9.4/src/pygbuttons.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygbuttons
-Version: 0.9.3
+Version: 0.9.4
 Summary: Adds basic UI elements for pygame
 Home-page: https://github.com/Jarno-de-Wit/PygButtons
 Author: Jarno de Wit
 Project-URL: Bug Tracker, https://github.com/Jarno-de-Wit/PygButtons/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,17 +32,16 @@
 To use the Buttons in a program, it is recommended to perform the following steps:
 - Setup
   1. Import the module / the contents of the module.
   2. Set the settings for the Buttons module (framerate, scroll factor, scaling limits) where appropriate
   3. Create the required Buttons
 - While running
   1. Pass all (relevant) Pygame.Events to the active Buttons in the input loop
-  2. Update the Buttons with information which is not event driven (e.g. cursor position)
-  3. Draw the Buttons to the active screen
-  4. Repeat
+  2. Draw the Buttons to the active screen
+  3. Repeat
 
 Getting an output from a Button can be done either by binding a function to the Button (which is then automatically executed when a certain action takes place), or by polling the Buttons value / status.
 
 For a practical implementation, see the [example.py](https://github.com/Jarno-de-Wit/PygButtons/blob/main/Example.py) file.
 
 ## Support
 For support / issues, please visit the issue tracker on [GitHub](https://github.com/Jarno-de-Wit/PygButtons/issues).
```

