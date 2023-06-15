# Comparing `tmp/BLACKFORGE2-0.1.3.tar.gz` & `tmp/BLACKFORGE2-0.1.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BLACKFORGE2-0.1.3.tar", last modified: Thu Jun 15 14:09:46 2023, max compression
+gzip compressed data, was "BLACKFORGE2-0.1.post2.tar", last modified: Tue Jun 13 07:30:29 2023, max compression
```

## Comparing `BLACKFORGE2-0.1.3.tar` & `BLACKFORGE2-0.1.post2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 14:09:46.392017 BLACKFORGE2-0.1.3/
-drwxrwxrwx   0        0        0        0 2023-06-15 14:09:46.367676 BLACKFORGE2-0.1.3/BLACKFORGE2/
--rw-rw-rw-   0        0        0    14018 2023-06-15 14:09:09.000000 BLACKFORGE2-0.1.3/BLACKFORGE2/FORGE.py
--rw-rw-rw-   0        0        0       20 2023-06-13 01:21:24.000000 BLACKFORGE2-0.1.3/BLACKFORGE2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 14:09:46.389026 BLACKFORGE2-0.1.3/BLACKFORGE2.egg-info/
--rw-rw-rw-   0        0        0      312 2023-06-15 14:09:45.000000 BLACKFORGE2-0.1.3/BLACKFORGE2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-06-15 14:09:45.000000 BLACKFORGE2-0.1.3/BLACKFORGE2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 14:09:45.000000 BLACKFORGE2-0.1.3/BLACKFORGE2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-15 14:09:45.000000 BLACKFORGE2-0.1.3/BLACKFORGE2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-15 14:09:45.000000 BLACKFORGE2-0.1.3/BLACKFORGE2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2023-06-13 00:44:16.000000 BLACKFORGE2-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      312 2023-06-15 14:09:46.391022 BLACKFORGE2-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     8041 2023-06-13 07:29:39.000000 BLACKFORGE2-0.1.3/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-15 14:09:46.393018 BLACKFORGE2-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      492 2023-06-15 14:09:26.000000 BLACKFORGE2-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:30:29.908442 BLACKFORGE2-0.1.post2/
+drwxrwxrwx   0        0        0        0 2023-06-13 07:30:29.881263 BLACKFORGE2-0.1.post2/BLACKFORGE2/
+-rw-rw-rw-   0        0        0    14204 2023-06-13 02:34:43.000000 BLACKFORGE2-0.1.post2/BLACKFORGE2/FORGE.py
+-rw-rw-rw-   0        0        0       20 2023-06-13 01:21:24.000000 BLACKFORGE2-0.1.post2/BLACKFORGE2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:30:29.905450 BLACKFORGE2-0.1.post2/BLACKFORGE2.egg-info/
+-rw-rw-rw-   0        0        0      315 2023-06-13 07:30:29.000000 BLACKFORGE2-0.1.post2/BLACKFORGE2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-06-13 07:30:29.000000 BLACKFORGE2-0.1.post2/BLACKFORGE2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 07:30:29.000000 BLACKFORGE2-0.1.post2/BLACKFORGE2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-13 07:30:29.000000 BLACKFORGE2-0.1.post2/BLACKFORGE2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-13 07:30:29.000000 BLACKFORGE2-0.1.post2/BLACKFORGE2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2023-06-13 00:44:16.000000 BLACKFORGE2-0.1.post2/LICENSE
+-rw-rw-rw-   0        0        0      315 2023-06-13 07:30:29.907446 BLACKFORGE2-0.1.post2/PKG-INFO
+-rw-rw-rw-   0        0        0     8041 2023-06-13 07:29:39.000000 BLACKFORGE2-0.1.post2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-13 07:30:29.908442 BLACKFORGE2-0.1.post2/setup.cfg
+-rw-rw-rw-   0        0        0      495 2023-06-13 07:30:15.000000 BLACKFORGE2-0.1.post2/setup.py
```

### Comparing `BLACKFORGE2-0.1.3/BLACKFORGE2/FORGE.py` & `BLACKFORGE2-0.1.post2/BLACKFORGE2/FORGE.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,26 @@
 import math, random, sys
 
 from pygame.locals import *
 from os import walk,sep
 from csv import reader
 
 pygame.font.init()
-pygame.mixer.init()
+
+# IMPORT YOUR SETTINGS FILE
+#from settings import *
 
 """ PHYSICS """
 class Physics():
 
 	def __init__(self):
 		pass
 
-	def apply_gravity(self, entity, gravity_value, dt):
-		entity.velocity.y += gravity_value * dt
+	def apply_gravity(self, entity, gravity_value):
+		entity.velocity.y += gravity_value
 		entity.rect.y += entity.velocity.y
 
 	def horizontal_movement_collision(self, entity, collision_tiles:pygame.sprite.Group):
 		entity = entity
 		entity.rect.x += entity.velocity.x * entity.speed
 
 		for sprite in collision_tiles.sprites():
@@ -143,21 +145,24 @@
 			self.frame_index = 0
 		self.image = self.frames[int(self.frame_index)]
 
 	def update(self) -> None:
 		self.animate()
 
 class Light():
-	def __init__(self, radius:int, color:str, intensity:float, manual_pos=(0,0)):
+	def __init__(self, radius:int, color:str, intensity:float, screen_width:int, screen_height:int, world_brightness:int, manual_pos=(0,0)):
 		# Initialize the Light object
 		self.position = pygame.math.Vector2(manual_pos)  # Set the position of the light
 		self.radius = radius  # Radius of the light
 		self.color = color  # Color of the light
 		self.intensity = intensity  # Intensity of the light
-		self.world_brightness = WORLD_BRIGHTNESS  # Brightness of the world
+		self.world_brightness = world_brightness  # Brightness of the world
+		self.screen_width = screen_width
+		self.screen_height = screen_height
+
 
 	def generate_glow(self, glow:int, radius:int) -> pygame.Surface:
 		# Generate a surface for the light glow effect
 		surface = pygame.Surface((int(radius)*2, int(radius)*2), pygame.SRCALPHA)
 
 		layers = 30  # Number of layers for the glow effect
 
@@ -166,15 +171,15 @@
 			pygame.draw.circle(
 				surface, self.color, surface.get_rect().center, radius - i * 3
 			)
 		return surface
 
 	def world_light(self):
 		# Create the overlay with the world brightness
-		self.light_layer = pygame.Surface((SCREEN_WIDTH, SCREEN_HEIGHT), pygame.SRCALPHA, 32)
+		self.light_layer = pygame.Surface((self.screen_width, self.screen_height), pygame.SRCALPHA, 32)
 		self.light_layer.convert_alpha()
 		self.light_layer.fill((self.world_brightness, self.world_brightness, self.world_brightness))
 
 	def apply_lighting(self, surface:pygame.Surface, light_layer:pygame.Surface, light_source_list=None) -> None:
 		# Apply lighting effects to the given surface
 
 		if self.position.x > 0:
@@ -333,15 +338,15 @@
 	terrain_map = []
 	with open(path) as map:
 		level = reader(map, delimiter=',')
 		for row in level:
 			terrain_map.append(list(row))
 		return terrain_map
 
-def import_cut_graphics(path:str) -> list:
+def import_cut_graphics(path:str, TILE_SIZE:int) -> list:
 	surface = get_image(path)
 	tile_num_x = int(surface.get_size()[0] / TILE_SIZE)
 	tile_num_y = int(surface.get_size()[1] / TILE_SIZE)
 
 	cut_tiles = []
 	for row in range(tile_num_y):
 		for col in range(tile_num_x):
```

### Comparing `BLACKFORGE2-0.1.3/LICENSE` & `BLACKFORGE2-0.1.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `BLACKFORGE2-0.1.3/README.rst` & `BLACKFORGE2-0.1.post2/README.rst`

 * *Files identical despite different names*

