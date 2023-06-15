# Comparing `tmp/rustplus-5.6.5.tar.gz` & `tmp/rustplus-5.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rustplus-5.6.5.tar", last modified: Wed Jun 14 14:01:27 2023, max compression
+gzip compressed data, was "rustplus-5.6.6.tar", last modified: Thu Jun 15 19:51:56 2023, max compression
```

## Comparing `rustplus-5.6.5.tar` & `rustplus-5.6.6.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.445625 rustplus-5.6.5/
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-06-14 14:01:10.000000 rustplus-5.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-14 14:01:10.000000 rustplus-5.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-06-14 14:01:27.449625 rustplus-5.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2005 2023-06-14 14:01:10.000000 rustplus-5.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.421625 rustplus-5.6.5/rustplus/
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.421625 rustplus-5.6.5/rustplus/api/
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20349 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/base_rust_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.433625 rustplus-5.6.5/rustplus/api/icons/
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    23598 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/airfield.png
--rw-r--r--   0 runner    (1001) docker     (122)    13944 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/arctic_base.png
--rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/bandit.png
--rw-r--r--   0 runner    (1001) docker     (122)    35348 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/barn.png
--rw-r--r--   0 runner    (1001) docker     (122)     2553 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/cargo.png
--rw-r--r--   0 runner    (1001) docker     (122)     2058 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/chinook.png
--rw-r--r--   0 runner    (1001) docker     (122)     4228 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/chinook_blades.png
--rw-r--r--   0 runner    (1001) docker     (122)    23420 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/crate.png
--rw-r--r--   0 runner    (1001) docker     (122)    12339 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/desert_base.png
--rw-r--r--   0 runner    (1001) docker     (122)    34156 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/dome.png
--rw-r--r--   0 runner    (1001) docker     (122)    34662 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/excavator.png
--rw-r--r--   0 runner    (1001) docker     (122)     4934 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/explosion.png
--rw-r--r--   0 runner    (1001) docker     (122)    24176 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/fishing.png
--rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/harbour.png
--rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/icon.png
--rw-r--r--   0 runner    (1001) docker     (122)    41087 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/junkyard.png
--rw-r--r--   0 runner    (1001) docker     (122)     9091 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/large_oil_rig.png
--rw-r--r--   0 runner    (1001) docker     (122)    23696 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/launchsite.png
--rw-r--r--   0 runner    (1001) docker     (122)    27391 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/lighthouse.png
--rw-r--r--   0 runner    (1001) docker     (122)    23532 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/military_tunnels.png
--rw-r--r--   0 runner    (1001) docker     (122)    27923 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/mining_outpost.png
--rw-r--r--   0 runner    (1001) docker     (122)    30573 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/outpost.png
--rw-r--r--   0 runner    (1001) docker     (122)     2384 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/oxums.png
--rw-r--r--   0 runner    (1001) docker     (122)     2742 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/patrol.png
--rw-r--r--   0 runner    (1001) docker     (122)    23513 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/power_plant.png
--rw-r--r--   0 runner    (1001) docker     (122)    36433 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/quarry.png
--rw-r--r--   0 runner    (1001) docker     (122)    28365 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/satellite.png
--rw-r--r--   0 runner    (1001) docker     (122)    17804 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/sewer.png
--rw-r--r--   0 runner    (1001) docker     (122)     8114 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/small_oil_rig.png
--rw-r--r--   0 runner    (1001) docker     (122)    30710 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/stable.png
--rw-r--r--   0 runner    (1001) docker     (122)    28458 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/supermarket.png
--rw-r--r--   0 runner    (1001) docker     (122)     2049 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/swamp.png
--rw-r--r--   0 runner    (1001) docker     (122)     5300 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/train.png
--rw-r--r--   0 runner    (1001) docker     (122)    20587 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/train_yard.png
--rw-r--r--   0 runner    (1001) docker     (122)     3066 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/underwater_lab.png
--rw-r--r--   0 runner    (1001) docker     (122)     5705 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/vending_machine.png
--rw-r--r--   0 runner    (1001) docker     (122)    23907 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/icons/water_treatment.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.437625 rustplus-5.6.5/rustplus/api/remote/
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.437625 rustplus-5.6.5/rustplus/api/remote/camera/
--rw-r--r--   0 runner    (1001) docker     (122)      147 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/camera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   118649 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/camera/camera_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     5711 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/camera/camera_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)    24457 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/camera/camera_parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     3354 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/camera/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.441625 rustplus-5.6.5/rustplus/api/remote/events/
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/events/event_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/events/event_loop_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     3325 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/events/events.py
--rw-r--r--   0 runner    (1001) docker     (122)     2285 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/events/handler_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/events/map_event_listener.py
--rw-r--r--   0 runner    (1001) docker     (122)      776 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/events/registered_listener.py
--rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/expo_bundle_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)      664 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/fcm_listener.py
--rw-r--r--   0 runner    (1001) docker     (122)      799 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (122)     4114 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/rust_remote_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.441625 rustplus-5.6.5/rustplus/api/remote/rustplus_proto/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/rustplus_proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16144 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/rustplus_proto/rustplus.py
--rw-r--r--   0 runner    (1001) docker     (122)    12369 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/rustws.py
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/remote/server_checker.py
--rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/rust_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.441625 rustplus-5.6.5/rustplus/api/structures/
--rw-r--r--   0 runner    (1001) docker     (122)      390 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/structures/rust_chat_message.py
--rw-r--r--   0 runner    (1001) docker     (122)      852 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/structures/rust_contents.py
--rw-r--r--   0 runner    (1001) docker     (122)     2048 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/structures/rust_entity_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     2004 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/structures/rust_info.py
--rw-r--r--   0 runner    (1001) docker     (122)      824 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/structures/rust_item.py
--rw-r--r--   0 runner    (1001) docker     (122)     1813 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/structures/rust_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     4805 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/structures/rust_marker.py
--rw-r--r--   0 runner    (1001) docker     (122)     3008 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/structures/rust_team_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/structures/rust_time.py
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/api/structures/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.445625 rustplus-5.6.5/rustplus/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/commands/command.py
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/commands/command_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2435 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/commands/command_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)      444 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/commands/command_options.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.445625 rustplus-5.6.5/rustplus/conversation/
--rw-r--r--   0 runner    (1001) docker     (122)      145 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/conversation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1885 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/conversation/conversation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1550 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/conversation/conversation_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/conversation/conversation_prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.445625 rustplus-5.6.5/rustplus/exceptions/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.445625 rustplus-5.6.5/rustplus/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      181 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/utils/deprecated.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.445625 rustplus-5.6.5/rustplus/utils/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)    74752 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/utils/fonts/PermanentMarker.ttf
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/utils/fonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    26480 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/utils/grab_items.py
--rw-r--r--   0 runner    (1001) docker     (122)     5388 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/utils/rust_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      752 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/utils/server_id.py
--rw-r--r--   0 runner    (1001) docker     (122)      770 2023-06-14 14:01:10.000000 rustplus-5.6.5/rustplus/utils/yielding_event.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:01:27.421625 rustplus-5.6.5/rustplus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-06-14 14:01:27.000000 rustplus-5.6.5/rustplus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3536 2023-06-14 14:01:27.000000 rustplus-5.6.5/rustplus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 14:01:27.000000 rustplus-5.6.5/rustplus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       96 2023-06-14 14:01:27.000000 rustplus-5.6.5/rustplus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-14 14:01:27.000000 rustplus-5.6.5/rustplus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-14 14:01:27.449625 rustplus-5.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-06-14 14:01:10.000000 rustplus-5.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:51:56.964550 rustplus-5.6.6/
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-06-15 19:51:45.000000 rustplus-5.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-15 19:51:45.000000 rustplus-5.6.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-06-15 19:51:56.964550 rustplus-5.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2005 2023-06-15 19:51:45.000000 rustplus-5.6.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:51:56.948550 rustplus-5.6.6/rustplus/
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:51:56.948550 rustplus-5.6.6/rustplus/api/
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20421 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/base_rust_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:51:56.956550 rustplus-5.6.6/rustplus/api/icons/
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23598 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/airfield.png
+-rw-r--r--   0 runner    (1001) docker     (122)    13944 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/arctic_base.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/bandit.png
+-rw-r--r--   0 runner    (1001) docker     (122)    35348 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/barn.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2553 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/cargo.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2058 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/chinook.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4228 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/chinook_blades.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23420 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/crate.png
+-rw-r--r--   0 runner    (1001) docker     (122)    12339 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/desert_base.png
+-rw-r--r--   0 runner    (1001) docker     (122)    34156 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/dome.png
+-rw-r--r--   0 runner    (1001) docker     (122)    34662 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/excavator.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4934 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/explosion.png
+-rw-r--r--   0 runner    (1001) docker     (122)    24176 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/fishing.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/harbour.png
+-rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/icon.png
+-rw-r--r--   0 runner    (1001) docker     (122)    41087 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/junkyard.png
+-rw-r--r--   0 runner    (1001) docker     (122)     9091 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/large_oil_rig.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23696 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/launchsite.png
+-rw-r--r--   0 runner    (1001) docker     (122)    27391 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/lighthouse.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23532 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/military_tunnels.png
+-rw-r--r--   0 runner    (1001) docker     (122)    27923 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/mining_outpost.png
+-rw-r--r--   0 runner    (1001) docker     (122)    30573 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/outpost.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2384 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/oxums.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2742 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/patrol.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23513 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/power_plant.png
+-rw-r--r--   0 runner    (1001) docker     (122)    36433 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/quarry.png
+-rw-r--r--   0 runner    (1001) docker     (122)    28365 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/satellite.png
+-rw-r--r--   0 runner    (1001) docker     (122)    17804 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/sewer.png
+-rw-r--r--   0 runner    (1001) docker     (122)     8114 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/small_oil_rig.png
+-rw-r--r--   0 runner    (1001) docker     (122)    30710 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/stable.png
+-rw-r--r--   0 runner    (1001) docker     (122)    28458 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/supermarket.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2049 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/swamp.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5300 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/train.png
+-rw-r--r--   0 runner    (1001) docker     (122)    20587 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/train_yard.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3066 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/underwater_lab.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5705 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/vending_machine.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23907 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/icons/water_treatment.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:51:56.956550 rustplus-5.6.6/rustplus/api/remote/
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/remote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:51:56.960550 rustplus-5.6.6/rustplus/api/remote/camera/
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/remote/camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   118649 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/remote/camera/camera_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5711 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/remote/camera/camera_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24457 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/remote/camera/camera_parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3354 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/remote/camera/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:51:56.960550 rustplus-5.6.6/rustplus/api/remote/events/
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/remote/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/remote/events/event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/remote/events/event_loop_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3325 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/remote/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2285 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/remote/events/handler_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/remote/events/map_event_listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)      776 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/remote/events/registered_listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/remote/expo_bundle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      664 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/remote/fcm_listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/remote/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4210 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/remote/ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8238 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/remote/rust_remote_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:51:56.960550 rustplus-5.6.6/rustplus/api/remote/rustplus_proto/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/remote/rustplus_proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16144 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/remote/rustplus_proto/rustplus.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12816 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/remote/rustws.py
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/remote/server_checker.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13828 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/rust_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:51:56.960550 rustplus-5.6.6/rustplus/api/structures/
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/structures/rust_chat_message.py
+-rw-r--r--   0 runner    (1001) docker     (122)      852 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/structures/rust_contents.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2048 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/structures/rust_entity_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2004 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/structures/rust_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/structures/rust_item.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1813 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/structures/rust_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4805 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/structures/rust_marker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3008 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/structures/rust_team_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/structures/rust_time.py
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/api/structures/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:51:56.960550 rustplus-5.6.6/rustplus/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/commands/command_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/commands/command_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      444 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/commands/command_options.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:51:56.960550 rustplus-5.6.6/rustplus/conversation/
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/conversation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1885 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/conversation/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1550 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/conversation/conversation_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/conversation/conversation_prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:51:56.964550 rustplus-5.6.6/rustplus/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:51:56.964550 rustplus-5.6.6/rustplus/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/utils/deprecated.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:51:56.964550 rustplus-5.6.6/rustplus/utils/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)    74752 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/utils/fonts/PermanentMarker.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/utils/fonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26480 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/utils/grab_items.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5388 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/utils/rust_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      752 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/utils/server_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2023-06-15 19:51:45.000000 rustplus-5.6.6/rustplus/utils/yielding_event.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:51:56.948550 rustplus-5.6.6/rustplus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-06-15 19:51:56.000000 rustplus-5.6.6/rustplus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3536 2023-06-15 19:51:56.000000 rustplus-5.6.6/rustplus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 19:51:56.000000 rustplus-5.6.6/rustplus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-06-15 19:51:56.000000 rustplus-5.6.6/rustplus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-15 19:51:56.000000 rustplus-5.6.6/rustplus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-15 19:51:56.964550 rustplus-5.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-06-15 19:51:45.000000 rustplus-5.6.6/setup.py
```

### Comparing `rustplus-5.6.5/LICENSE` & `rustplus-5.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/PKG-INFO` & `rustplus-5.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustplus
-Version: 5.6.5
+Version: 5.6.6
 Summary: A python wrapper for the Rust Plus API
 Home-page: https://github.com/olijeffers0n/rustplus
 Author: olijeffers0n
 License: MIT
 Project-URL: Issue tracker, https://github.com/olijeffers0n/rustplus/issues
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `rustplus-5.6.5/README.md` & `rustplus-5.6.6/README.md`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/__init__.py` & `rustplus-5.6.6/rustplus/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,9 +18,9 @@
 from .commands import CommandOptions, Command
 from .exceptions import *
 from .conversation import ConversationFactory, Conversation, ConversationPrompt
 from .utils import *
 
 __name__ = "rustplus"
 __author__ = "olijeffers0n"
-__version__ = "5.6.5"
+__version__ = "5.6.6"
 __support__ = "Discord: https://discord.gg/nQqJe8qvP8"
```

### Comparing `rustplus-5.6.5/rustplus/api/base_rust_api.py` & `rustplus-5.6.6/rustplus/api/base_rust_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,17 @@
                 await self.remote.ratelimiter.consume(self.server_id, amount)
                 break
 
             if self.raise_ratelimit_exception:
                 raise RateLimitError("Out of tokens")
 
             await asyncio.sleep(
-                await self.remote.ratelimiter.get_estimated_delay_time(self.server_id, amount)
+                await self.remote.ratelimiter.get_estimated_delay_time(
+                    self.server_id, amount
+                )
             )
 
         self.heartbeat.reset_rhythm()
 
     def _generate_protobuf(self) -> AppRequest:
         """
         Generates the default protobuf for a request
@@ -104,15 +106,19 @@
         app_request.player_token = self.server_id.player_token
 
         self.seq += 1
 
         return app_request
 
     async def connect(
-        self, retries: int = float("inf"), delay: int = 20, on_failure=None, on_success=None
+        self,
+        retries: int = float("inf"),
+        delay: int = 20,
+        on_failure=None,
+        on_success=None,
     ) -> None:
         """
         Attempts to open a connection to the rust game server specified in the constructor
 
         :param retries: The number of times to attempt reconnecting. Defaults to infinite.
         :param delay: The delay (in seconds) between reconnection attempts.
         :param on_failure: Optional function to be called when connecting fails.
@@ -140,15 +146,15 @@
 
         try:
             if self.remote.ws is None:
                 await self.remote.connect(
                     retries=retries,
                     delay=delay,
                     on_failure=on_failure,
-                    on_success=on_success
+                    on_success=on_success,
                 )
                 await self.heartbeat.start_beat()
         except ConnectionRefusedError:
             raise ServerNotResponsiveError("Cannot Connect")
 
     async def close_connection(self) -> None:
         """
```

### Comparing `rustplus-5.6.5/rustplus/api/icons/airfield.png` & `rustplus-5.6.6/rustplus/api/icons/airfield.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/arctic_base.png` & `rustplus-5.6.6/rustplus/api/icons/arctic_base.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/bandit.png` & `rustplus-5.6.6/rustplus/api/icons/bandit.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/barn.png` & `rustplus-5.6.6/rustplus/api/icons/barn.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/cargo.png` & `rustplus-5.6.6/rustplus/api/icons/cargo.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/chinook.png` & `rustplus-5.6.6/rustplus/api/icons/chinook.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/chinook_blades.png` & `rustplus-5.6.6/rustplus/api/icons/chinook_blades.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/crate.png` & `rustplus-5.6.6/rustplus/api/icons/crate.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/desert_base.png` & `rustplus-5.6.6/rustplus/api/icons/desert_base.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/dome.png` & `rustplus-5.6.6/rustplus/api/icons/dome.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/excavator.png` & `rustplus-5.6.6/rustplus/api/icons/excavator.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/explosion.png` & `rustplus-5.6.6/rustplus/api/icons/explosion.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/fishing.png` & `rustplus-5.6.6/rustplus/api/icons/fishing.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/harbour.png` & `rustplus-5.6.6/rustplus/api/icons/harbour.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/icon.png` & `rustplus-5.6.6/rustplus/api/icons/icon.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/junkyard.png` & `rustplus-5.6.6/rustplus/api/icons/junkyard.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/large_oil_rig.png` & `rustplus-5.6.6/rustplus/api/icons/large_oil_rig.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/launchsite.png` & `rustplus-5.6.6/rustplus/api/icons/launchsite.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/lighthouse.png` & `rustplus-5.6.6/rustplus/api/icons/lighthouse.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/military_tunnels.png` & `rustplus-5.6.6/rustplus/api/icons/military_tunnels.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/mining_outpost.png` & `rustplus-5.6.6/rustplus/api/icons/mining_outpost.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/outpost.png` & `rustplus-5.6.6/rustplus/api/icons/outpost.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/oxums.png` & `rustplus-5.6.6/rustplus/api/icons/oxums.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/patrol.png` & `rustplus-5.6.6/rustplus/api/icons/patrol.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/power_plant.png` & `rustplus-5.6.6/rustplus/api/icons/power_plant.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/quarry.png` & `rustplus-5.6.6/rustplus/api/icons/quarry.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/satellite.png` & `rustplus-5.6.6/rustplus/api/icons/satellite.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/sewer.png` & `rustplus-5.6.6/rustplus/api/icons/sewer.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/small_oil_rig.png` & `rustplus-5.6.6/rustplus/api/icons/small_oil_rig.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/stable.png` & `rustplus-5.6.6/rustplus/api/icons/stable.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/supermarket.png` & `rustplus-5.6.6/rustplus/api/icons/supermarket.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/swamp.png` & `rustplus-5.6.6/rustplus/api/icons/swamp.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/train.png` & `rustplus-5.6.6/rustplus/api/icons/train.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/train_yard.png` & `rustplus-5.6.6/rustplus/api/icons/train_yard.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/underwater_lab.png` & `rustplus-5.6.6/rustplus/api/icons/underwater_lab.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/vending_machine.png` & `rustplus-5.6.6/rustplus/api/icons/vending_machine.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/icons/water_treatment.png` & `rustplus-5.6.6/rustplus/api/icons/water_treatment.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/remote/camera/camera_constants.py` & `rustplus-5.6.6/rustplus/api/remote/camera/camera_constants.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/remote/camera/camera_manager.py` & `rustplus-5.6.6/rustplus/api/remote/camera/camera_manager.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/remote/camera/camera_parser.py` & `rustplus-5.6.6/rustplus/api/remote/camera/camera_parser.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/remote/camera/structures.py` & `rustplus-5.6.6/rustplus/api/remote/camera/structures.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/remote/events/event_handler.py` & `rustplus-5.6.6/rustplus/api/remote/events/event_handler.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/remote/events/event_loop_manager.py` & `rustplus-5.6.6/rustplus/api/remote/events/event_loop_manager.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/remote/events/events.py` & `rustplus-5.6.6/rustplus/api/remote/events/events.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/remote/events/handler_list.py` & `rustplus-5.6.6/rustplus/api/remote/events/handler_list.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/remote/events/map_event_listener.py` & `rustplus-5.6.6/rustplus/api/remote/events/map_event_listener.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/remote/events/registered_listener.py` & `rustplus-5.6.6/rustplus/api/remote/events/registered_listener.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/remote/expo_bundle_handler.py` & `rustplus-5.6.6/rustplus/api/remote/expo_bundle_handler.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/remote/fcm_listener.py` & `rustplus-5.6.6/rustplus/api/remote/fcm_listener.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/remote/heartbeat.py` & `rustplus-5.6.6/rustplus/api/remote/heartbeat.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/remote/ratelimiter.py` & `rustplus-5.6.6/rustplus/api/remote/ratelimiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,27 +96,32 @@
             ]:
                 bucket.refresh()
                 if not bucket.can_consume(amount):
                     self.lock.release()
                     raise RateLimitError("Not Enough Tokens")
                 bucket.consume(amount)
 
-    async def get_estimated_delay_time(self, server_id: ServerID, target_cost: int) -> float:
+    async def get_estimated_delay_time(
+        self, server_id: ServerID, target_cost: int
+    ) -> float:
         """
         Returns how long until the amount of tokens needed will be available
         """
         async with self.lock:
             delay = 0
             for bucket in [
                 self.socket_buckets.get(server_id),
                 self.server_buckets.get(server_id.get_server_string()),
             ]:
                 val = (
                     math.ceil(
-                        (((target_cost - bucket.current) / bucket.refresh_per_second) + 0.1)
+                        (
+                            ((target_cost - bucket.current) / bucket.refresh_per_second)
+                            + 0.1
+                        )
                         * 100
                     )
                     / 100
                 )
                 if val > delay:
                     delay = val
         return delay
```

### Comparing `rustplus-5.6.5/rustplus/api/remote/rust_remote_interface.py` & `rustplus-5.6.6/rustplus/api/remote/rust_remote_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,17 @@
 
             while True:
                 if await self.ratelimiter.can_consume(self.server_id, cost):
                     await self.ratelimiter.consume(self.server_id, cost)
                     break
 
                 await asyncio.sleep(
-                    await self.ratelimiter.get_estimated_delay_time(self.server_id, cost)
+                    await self.ratelimiter.get_estimated_delay_time(
+                        self.server_id, cost
+                    )
                 )
 
             await self.send_message(app_request)
             response = await self.get_response(seq, app_request)
 
         elif self.ws.error_present(response.response.error.error) and error_check:
             raise RequestError(response.response.error.error)
```

### Comparing `rustplus-5.6.5/rustplus/api/remote/rustplus_proto/rustplus.py` & `rustplus-5.6.6/rustplus/api/remote/rustplus_proto/rustplus.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/remote/rustws.py` & `rustplus-5.6.6/rustplus/api/remote/rustws.py`

 * *Files 9% similar despite different names*

```diff
@@ -75,15 +75,17 @@
                         else (
                             f"wss://companion-rust.facepunch.com/game/{self.server_id.ip}/{self.server_id.port}"
                             if self.use_proxy
                             else f"ws://{self.server_id.ip}:{self.server_id.port}"
                         )
                     )
                     address += f"?v={str(self.magic_value)}"
-                    self.connection = await connect(address, close_timeout=0, ping_interval=None)
+                    self.connection = await connect(
+                        address, close_timeout=0, ping_interval=None
+                    )
                     self.connected_time = time.time()
 
                     if self.on_success is not None:
                         try:
                             if asyncio.iscoroutinefunction(self.on_success):
                                 await self.on_success()
                             else:
@@ -156,15 +158,18 @@
             return await self.send_message(message)
 
     async def run(self) -> None:
         while self.connection_status == CONNECTED:
             try:
                 data = await self.connection.recv()
 
-                await self.run_coroutine_non_blocking(EventHandler.run_proto_event(data, self.server_id))
+                # See below for context on why this is needed
+                await self.run_coroutine_non_blocking(
+                    EventHandler.run_proto_event(data, self.server_id)
+                )
 
                 app_message = AppMessage()
                 app_message.parse(
                     base64.b64decode(data) if self.use_test_server else data
                 )
 
             except Exception as e:
@@ -175,51 +180,57 @@
                     )
                     await self.connect(ignore_open_value=True)
 
                     continue
                 return
 
             try:
-                await self.handle_message(app_message)
+                # This creates an asyncio task rather than awaiting the coroutine directly.
+                # This fixes the bug where if you called a BaseRustSocket#get... from within a RegisteredListener or callback,
+                # It would hang the websocket. This is because the websocket event loop would be stuck on the callback rather than polling the socket.
+                # This way, we can schedule the execution of all logic for this message, but continue polling the WS
+                await self.run_coroutine_non_blocking(self.handle_message(app_message))
             except Exception:
-                self.logger.exception("An Error occurred whilst handling the message from the server")
+                self.logger.exception(
+                    "An Error occurred whilst handling the message from the server"
+                )
 
     async def handle_message(self, app_message: AppMessage) -> None:
         if app_message.response.seq in self.remote.ignored_responses:
             self.remote.ignored_responses.remove(app_message.response.seq)
             return
 
         prefix = self.get_prefix(
             str(app_message.broadcast.team_message.message.message)
         )
 
         if prefix is not None:
             # This means it is a command
 
             message = RustChatMessage(app_message.broadcast.team_message.message)
-            await self.run_coroutine_non_blocking(self.remote.command_handler.run_command(message, prefix))
+            await self.remote.command_handler.run_command(message, prefix)
 
         if self.is_entity_broadcast(app_message):
             # This means that an entity has changed state
 
-            await self.run_coroutine_non_blocking(EventHandler.run_entity_event(
+            await EventHandler.run_entity_event(
                 app_message.broadcast.entity_changed.entity_id,
                 app_message,
                 self.server_id,
-            ))
+            )
 
         elif self.is_camera_broadcast(app_message):
             if self.remote.camera_manager is not None:
-                await self.run_coroutine_non_blocking(self.remote.camera_manager.add_packet(
+                await self.remote.camera_manager.add_packet(
                     RayPacket(app_message.broadcast.camera_rays)
-                ))
+                )
 
         elif self.is_team_broadcast(app_message):
             # This means that the team of the current player has changed
-            await self.run_coroutine_non_blocking(EventHandler.run_team_event(app_message, self.server_id))
+            await EventHandler.run_team_event(app_message, self.server_id)
 
         elif self.is_message(app_message):
             # This means that a message has been sent to the team chat
 
             steam_id = int(app_message.broadcast.team_message.message.steam_id)
             message = str(app_message.broadcast.team_message.message.message)
 
@@ -227,34 +238,34 @@
             if self.remote.conversation_factory.has_conversation(steam_id):
                 if message not in self.outgoing_conversation_messages:
                     conversation: Conversation = (
                         self.remote.conversation_factory.get_conversation(steam_id)
                     )
 
                     conversation.get_answers().append(message)
-                    await self.run_coroutine_non_blocking(conversation.get_current_prompt().on_response(message))
+                    await conversation.get_current_prompt().on_response(message)
 
                     if conversation.has_next():
                         conversation.increment_prompt()
                         prompt = conversation.get_current_prompt()
                         prompt_string = await prompt.prompt()
-                        await self.run_coroutine_non_blocking(conversation.send_prompt(prompt_string))
+                        await conversation.send_prompt(prompt_string)
 
                     else:
                         prompt = conversation.get_current_prompt()
                         prompt_string = await prompt.on_finish()
                         if prompt_string != "":
-                            await self.run_coroutine_non_blocking(conversation.send_prompt(prompt_string))
+                            await conversation.send_prompt(prompt_string)
                         self.remote.conversation_factory.abort_conversation(steam_id)
                 else:
                     self.outgoing_conversation_messages.remove(message)
 
                 # Conversation API end
 
-            await self.run_coroutine_non_blocking(EventHandler.run_chat_event(app_message, self.server_id))
+            await EventHandler.run_chat_event(app_message, self.server_id)
 
         else:
             # This means that it wasn't sent by the server and is a message from the server in response to an action
             event: YieldingEvent = self.remote.pending_response_events[
                 app_message.response.seq
             ]
             event.set_with_value(app_message)
@@ -317,10 +328,10 @@
     def error_present(message) -> bool:
         """
         Checks message for error
         """
         return message != ""
 
     @staticmethod
-    async def run_coroutine_non_blocking(coroutine: Coroutine) -> None:
+    async def run_coroutine_non_blocking(coroutine: Coroutine) -> Task:
         loop: AbstractEventLoop = asyncio.get_event_loop_policy().get_event_loop()
-        loop.create_task(coroutine)
+        return loop.create_task(coroutine)
```

### Comparing `rustplus-5.6.5/rustplus/api/remote/server_checker.py` & `rustplus-5.6.6/rustplus/api/remote/server_checker.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/rust_api.py` & `rustplus-5.6.6/rustplus/api/rust_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 import requests
-from typing import List
+from typing import List, Union
 from PIL import Image
 from io import BytesIO
 from datetime import datetime
 from collections import defaultdict
 from importlib import resources
 
 from .base_rust_api import BaseRustSocket
@@ -80,15 +80,15 @@
 
         await self.remote.send_message(app_request)
 
         response = await self.remote.get_response(app_request.seq, app_request)
 
         return format_time(response)
 
-    async def send_team_message(self, message: str) -> None:
+    async def send_team_message(self, message: Union[str, object]) -> None:
         await self._handle_ratelimit(2)
 
         app_send_message = AppSendMessage()
         app_send_message.message = str(message)
 
         app_request = self._generate_protobuf()
         app_request.send_team_message = app_send_message
```

### Comparing `rustplus-5.6.5/rustplus/api/structures/rust_chat_message.py` & `rustplus-5.6.6/rustplus/api/structures/rust_chat_message.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/structures/rust_contents.py` & `rustplus-5.6.6/rustplus/api/structures/rust_contents.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/structures/rust_entity_info.py` & `rustplus-5.6.6/rustplus/api/structures/rust_entity_info.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/structures/rust_info.py` & `rustplus-5.6.6/rustplus/api/structures/rust_info.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/structures/rust_item.py` & `rustplus-5.6.6/rustplus/api/structures/rust_item.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/structures/rust_map.py` & `rustplus-5.6.6/rustplus/api/structures/rust_map.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/structures/rust_marker.py` & `rustplus-5.6.6/rustplus/api/structures/rust_marker.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/structures/rust_team_info.py` & `rustplus-5.6.6/rustplus/api/structures/rust_team_info.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/api/structures/rust_time.py` & `rustplus-5.6.6/rustplus/api/structures/rust_time.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/commands/command.py` & `rustplus-5.6.6/rustplus/commands/command.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/commands/command_data.py` & `rustplus-5.6.6/rustplus/commands/command_data.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/commands/command_handler.py` & `rustplus-5.6.6/rustplus/commands/command_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             )
         else:
             for command_name, data in self.commands.items():
                 # Loop through all the commands and see if the command is in the data aliases list
                 # or if it matches the callable function
 
                 if command in data.aliases or data.callable_func(command):
-                    data.coro(
+                    await data.coro(
                         Command(
                             message.name,
                             message.steam_id,
                             CommandTime(
                                 datetime.utcfromtimestamp(message.time), message.time
                             ),
                             command,
```

### Comparing `rustplus-5.6.5/rustplus/conversation/conversation.py` & `rustplus-5.6.6/rustplus/conversation/conversation.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/conversation/conversation_factory.py` & `rustplus-5.6.6/rustplus/conversation/conversation_factory.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/exceptions/exceptions.py` & `rustplus-5.6.6/rustplus/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/utils/deprecated.py` & `rustplus-5.6.6/rustplus/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/utils/fonts/PermanentMarker.ttf` & `rustplus-5.6.6/rustplus/utils/fonts/PermanentMarker.ttf`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/utils/grab_items.py` & `rustplus-5.6.6/rustplus/utils/grab_items.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/utils/rust_utils.py` & `rustplus-5.6.6/rustplus/utils/rust_utils.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/utils/server_id.py` & `rustplus-5.6.6/rustplus/utils/server_id.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus/utils/yielding_event.py` & `rustplus-5.6.6/rustplus/utils/yielding_event.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/rustplus.egg-info/PKG-INFO` & `rustplus-5.6.6/rustplus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustplus
-Version: 5.6.5
+Version: 5.6.6
 Summary: A python wrapper for the Rust Plus API
 Home-page: https://github.com/olijeffers0n/rustplus
 Author: olijeffers0n
 License: MIT
 Project-URL: Issue tracker, https://github.com/olijeffers0n/rustplus/issues
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `rustplus-5.6.5/rustplus.egg-info/SOURCES.txt` & `rustplus-5.6.6/rustplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.5/setup.py` & `rustplus-5.6.6/setup.py`

 * *Files identical despite different names*

