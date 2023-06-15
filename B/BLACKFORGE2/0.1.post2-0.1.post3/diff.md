# Comparing `tmp/BLACKFORGE2-0.1.post2.tar.gz` & `tmp/BLACKFORGE2-0.1.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BLACKFORGE2-0.1.post2.tar", last modified: Tue Jun 13 07:30:29 2023, max compression
+gzip compressed data, was "BLACKFORGE2-0.1.post3.tar", last modified: Thu Jun 15 14:15:10 2023, max compression
```

## Comparing `BLACKFORGE2-0.1.post2.tar` & `BLACKFORGE2-0.1.post3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 07:30:29.908442 BLACKFORGE2-0.1.post2/
-drwxrwxrwx   0        0        0        0 2023-06-13 07:30:29.881263 BLACKFORGE2-0.1.post2/BLACKFORGE2/
--rw-rw-rw-   0        0        0    14204 2023-06-13 02:34:43.000000 BLACKFORGE2-0.1.post2/BLACKFORGE2/FORGE.py
--rw-rw-rw-   0        0        0       20 2023-06-13 01:21:24.000000 BLACKFORGE2-0.1.post2/BLACKFORGE2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:30:29.905450 BLACKFORGE2-0.1.post2/BLACKFORGE2.egg-info/
--rw-rw-rw-   0        0        0      315 2023-06-13 07:30:29.000000 BLACKFORGE2-0.1.post2/BLACKFORGE2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-06-13 07:30:29.000000 BLACKFORGE2-0.1.post2/BLACKFORGE2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 07:30:29.000000 BLACKFORGE2-0.1.post2/BLACKFORGE2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-13 07:30:29.000000 BLACKFORGE2-0.1.post2/BLACKFORGE2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-13 07:30:29.000000 BLACKFORGE2-0.1.post2/BLACKFORGE2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2023-06-13 00:44:16.000000 BLACKFORGE2-0.1.post2/LICENSE
--rw-rw-rw-   0        0        0      315 2023-06-13 07:30:29.907446 BLACKFORGE2-0.1.post2/PKG-INFO
--rw-rw-rw-   0        0        0     8041 2023-06-13 07:29:39.000000 BLACKFORGE2-0.1.post2/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-13 07:30:29.908442 BLACKFORGE2-0.1.post2/setup.cfg
--rw-rw-rw-   0        0        0      495 2023-06-13 07:30:15.000000 BLACKFORGE2-0.1.post2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 14:15:10.928119 BLACKFORGE2-0.1.post3/
+drwxrwxrwx   0        0        0        0 2023-06-15 14:15:10.916617 BLACKFORGE2-0.1.post3/BLACKFORGE2/
+-rw-rw-rw-   0        0        0    14363 2023-06-15 14:13:08.000000 BLACKFORGE2-0.1.post3/BLACKFORGE2/FORGE.py
+-rw-rw-rw-   0        0        0       20 2023-06-13 01:21:24.000000 BLACKFORGE2-0.1.post3/BLACKFORGE2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 14:15:10.926128 BLACKFORGE2-0.1.post3/BLACKFORGE2.egg-info/
+-rw-rw-rw-   0        0        0      316 2023-06-15 14:15:10.000000 BLACKFORGE2-0.1.post3/BLACKFORGE2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-06-15 14:15:10.000000 BLACKFORGE2-0.1.post3/BLACKFORGE2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 14:15:10.000000 BLACKFORGE2-0.1.post3/BLACKFORGE2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-15 14:15:10.000000 BLACKFORGE2-0.1.post3/BLACKFORGE2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-15 14:15:10.000000 BLACKFORGE2-0.1.post3/BLACKFORGE2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2023-06-13 00:44:16.000000 BLACKFORGE2-0.1.post3/LICENSE
+-rw-rw-rw-   0        0        0      316 2023-06-15 14:15:10.927123 BLACKFORGE2-0.1.post3/PKG-INFO
+-rw-rw-rw-   0        0        0     8041 2023-06-13 07:29:39.000000 BLACKFORGE2-0.1.post3/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-15 14:15:10.928119 BLACKFORGE2-0.1.post3/setup.cfg
+-rw-rw-rw-   0        0        0      496 2023-06-15 14:15:04.000000 BLACKFORGE2-0.1.post3/setup.py
```

### Comparing `BLACKFORGE2-0.1.post2/BLACKFORGE2/FORGE.py` & `BLACKFORGE2-0.1.post3/BLACKFORGE2/FORGE.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 """ PHYSICS """
 class Physics():
 
 	def __init__(self):
 		pass
 
-	def apply_gravity(self, entity, gravity_value):
-		entity.velocity.y += gravity_value
+	def apply_gravity(self, entity, gravity_value:float, delta_time:float):
+		entity.velocity.y += gravity_value * delta_time
 		entity.rect.y += entity.velocity.y
 
 	def horizontal_movement_collision(self, entity, collision_tiles:pygame.sprite.Group):
 		entity = entity
 		entity.rect.x += entity.velocity.x * entity.speed
 
 		for sprite in collision_tiles.sprites():
@@ -97,17 +97,18 @@
 		self.pos = pygame.math.Vector2(pos)  # Initial position of the tile
 
 	def update(self, world_shift):
 		self.rect.x += world_shift.x
 		self.rect.y += world_shift.y
 
 class MovingTile(StaticTile):
-	def __init__(self, pos:tuple, groups:list, direction:str, speed:int, surface:pygame.Surface):
+	def __init__(self, pos:tuple, groups:list, direction:str, speed:int, delta_time:float, surface:pygame.Surface):
 		super().__init__(pos, groups, surface)
 		self.image = surface
+		self.delta_time = delta_time
 		self.direction = direction  # Movement direction ('up', 'down', 'left', 'right')
 		self.speed = speed  # Movement speed (pixels per frame)
 
 	def move(self, constraints:list):
 		for constraint in constraints:
 			if self.rect.colliderect(constraint.rect):
 				if self.direction == 'up':
@@ -120,21 +121,21 @@
 					print("at right")
 					self.direction = "left"
 				elif self.direction == 'left':
 					print("at left")
 					self.direction = "right"
 			
 			if self.direction == 'up':
-				self.rect.y -= self.speed
+				self.rect.y -= self.speed * self.delta_time
 			elif self.direction == 'down':
-				self.rect.y += self.speed
+				self.rect.y += self.speed * self.delta_time
 			elif self.direction == 'left':
-				self.rect.x -= self.speed
+				self.rect.x -= self.speed * self.delta_time
 			elif self.direction == 'right':
-				self.rect.x += self.speed
+				self.rect.x += self.speed * self.delta_time
 
 class AnimatedTile(StaticTile):
 	def __init__(self,size:int,x:int,y:int,path:str):
 		super().__init__(size,x,y)
 		self.frames = import_folder(path)
 		self.frame_index = 0
 		self.image = self.frames[self.frame_index]
@@ -338,28 +339,28 @@
 	terrain_map = []
 	with open(path) as map:
 		level = reader(map, delimiter=',')
 		for row in level:
 			terrain_map.append(list(row))
 		return terrain_map
 
-def import_cut_graphics(path:str, TILE_SIZE:int) -> list:
+def import_cut_graphics(path:str, tile_size:int) -> list:
 	surface = get_image(path)
-	tile_num_x = int(surface.get_size()[0] / TILE_SIZE)
-	tile_num_y = int(surface.get_size()[1] / TILE_SIZE)
+	tile_num_x = int(surface.get_size()[0] / tile_size)
+	tile_num_y = int(surface.get_size()[1] / tile_size)
 
 	cut_tiles = []
 	for row in range(tile_num_y):
 		for col in range(tile_num_x):
-			x = col * TILE_SIZE
-			y = row * TILE_SIZE
+			x = col * tile_size
+			y = row * tile_size
 			new_surf = pygame.Surface(
-				(TILE_SIZE, TILE_SIZE), flags=pygame.SRCALPHA)
+				(tile_size, tile_size), flags=pygame.SRCALPHA)
 			new_surf.blit(surface, (0, 0), pygame.Rect(
-				x, y, TILE_SIZE, TILE_SIZE))
+				x, y, tile_size, tile_size))
 			cut_tiles.append(new_surf)
 
 	return cut_tiles
 
 _text_library = {}
 def draw_text(surface:pygame.Surface, text:str, pos:tuple, size=30, color=(255,255,255), bg_color=None):
 	global _text_library
```

### Comparing `BLACKFORGE2-0.1.post2/LICENSE` & `BLACKFORGE2-0.1.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `BLACKFORGE2-0.1.post2/README.rst` & `BLACKFORGE2-0.1.post3/README.rst`

 * *Files identical despite different names*

