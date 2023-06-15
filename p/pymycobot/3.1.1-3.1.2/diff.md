# Comparing `tmp/pymycobot-3.1.1.tar.gz` & `tmp/pymycobot-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymycobot-3.1.1.tar", last modified: Wed Jun 14 03:12:55 2023, max compression
+gzip compressed data, was "pymycobot-3.1.2.tar", last modified: Thu Jun 15 07:11:33 2023, max compression
```

## Comparing `pymycobot-3.1.1.tar` & `pymycobot-3.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 03:12:55.873676 pymycobot-3.1.1/
--rw-rw-rw-   0        0        0     1096 2022-06-28 10:55:58.000000 pymycobot-3.1.1/LICENSE
--rw-rw-rw-   0        0        0       51 2022-06-28 10:55:58.000000 pymycobot-3.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0    55974 2023-06-14 03:12:55.872652 pymycobot-3.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1867 2022-07-22 06:29:08.000000 pymycobot-3.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 03:12:55.841543 pymycobot-3.1.1/pymycobot/
--rw-rw-rw-   0        0        0    35112 2023-02-16 10:13:33.000000 pymycobot-3.1.1/pymycobot/Interface.py
--rw-rw-rw-   0        0        0     1554 2023-06-14 03:09:18.000000 pymycobot-3.1.1/pymycobot/__init__.py
--rw-rw-rw-   0        0        0     1968 2023-05-24 03:41:47.000000 pymycobot-3.1.1/pymycobot/bluet.py
--rw-rw-rw-   0        0        0    12276 2023-06-14 02:54:52.000000 pymycobot-3.1.1/pymycobot/common.py
--rw-rw-rw-   0        0        0     3053 2022-06-28 10:55:58.000000 pymycobot-3.1.1/pymycobot/error.py
--rw-rw-rw-   0        0        0    33724 2023-06-14 02:59:25.000000 pymycobot-3.1.1/pymycobot/generate.py
--rw-rw-rw-   0        0        0      230 2022-06-28 10:55:58.000000 pymycobot-3.1.1/pymycobot/genre.py
--rw-rw-rw-   0        0        0      557 2022-06-28 10:55:58.000000 pymycobot-3.1.1/pymycobot/log.py
--rw-rw-rw-   0        0        0      206 2022-11-14 03:29:13.000000 pymycobot-3.1.1/pymycobot/mecharm.py
--rw-rw-rw-   0        0        0     9015 2023-06-12 07:33:26.000000 pymycobot-3.1.1/pymycobot/myarm.py
--rw-rw-rw-   0        0        0    13315 2023-04-14 05:34:53.000000 pymycobot-3.1.1/pymycobot/mybuddy.py
--rw-rw-rw-   0        0        0     4768 2022-07-20 06:10:10.000000 pymycobot-3.1.1/pymycobot/mybuddybluetooth.py
--rw-rw-rw-   0        0        0     4588 2022-10-14 05:56:03.000000 pymycobot-3.1.1/pymycobot/mybuddyemoticon.py
--rw-rw-rw-   0        0        0     7190 2022-09-13 08:59:04.000000 pymycobot-3.1.1/pymycobot/mybuddysocket.py
--rw-rw-rw-   0        0        0     7503 2023-06-09 06:51:47.000000 pymycobot-3.1.1/pymycobot/mycobot.py
--rw-rw-rw-   0        0        0     7385 2023-06-09 07:23:49.000000 pymycobot-3.1.1/pymycobot/mycobotsocket.py
--rw-rw-rw-   0        0        0     8483 2023-05-23 05:43:01.000000 pymycobot-3.1.1/pymycobot/mypalletizer.py
--rw-rw-rw-   0        0        0     7500 2023-05-24 08:28:04.000000 pymycobot-3.1.1/pymycobot/mypalletizersocket.py
--rw-rw-rw-   0        0        0    19631 2023-05-24 08:27:45.000000 pymycobot-3.1.1/pymycobot/ultraArm.py
--rw-rw-rw-   0        0        0      674 2022-06-28 10:55:58.000000 pymycobot-3.1.1/pymycobot/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:12:55.871026 pymycobot-3.1.1/pymycobot.egg-info/
--rw-rw-rw-   0        0        0    55974 2023-06-14 03:12:55.000000 pymycobot-3.1.1/pymycobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      674 2023-06-14 03:12:55.000000 pymycobot-3.1.1/pymycobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 03:12:55.000000 pymycobot-3.1.1/pymycobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 03:12:55.000000 pymycobot-3.1.1/pymycobot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-14 03:12:55.000000 pymycobot-3.1.1/pymycobot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       26 2022-06-28 10:55:58.000000 pymycobot-3.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 03:12:55.873676 pymycobot-3.1.1/setup.cfg
--rw-rw-rw-   0        0        0     3055 2022-08-30 07:24:54.000000 pymycobot-3.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:11:33.694346 pymycobot-3.1.2/
+-rw-rw-rw-   0        0        0     1096 2022-06-28 10:55:58.000000 pymycobot-3.1.2/LICENSE
+-rw-rw-rw-   0        0        0       51 2022-06-28 10:55:58.000000 pymycobot-3.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    59099 2023-06-15 07:11:33.693335 pymycobot-3.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1867 2022-07-22 06:29:08.000000 pymycobot-3.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 07:11:33.663475 pymycobot-3.1.2/pymycobot/
+-rw-rw-rw-   0        0        0    35112 2023-02-16 10:13:33.000000 pymycobot-3.1.2/pymycobot/Interface.py
+-rw-rw-rw-   0        0        0     1554 2023-06-15 07:09:04.000000 pymycobot-3.1.2/pymycobot/__init__.py
+-rw-rw-rw-   0        0        0     1968 2023-05-24 03:41:47.000000 pymycobot-3.1.2/pymycobot/bluet.py
+-rw-rw-rw-   0        0        0    12276 2023-06-15 06:45:38.000000 pymycobot-3.1.2/pymycobot/common.py
+-rw-rw-rw-   0        0        0     3053 2022-06-28 10:55:58.000000 pymycobot-3.1.2/pymycobot/error.py
+-rw-rw-rw-   0        0        0    33758 2023-06-15 06:42:33.000000 pymycobot-3.1.2/pymycobot/generate.py
+-rw-rw-rw-   0        0        0      230 2022-06-28 10:55:58.000000 pymycobot-3.1.2/pymycobot/genre.py
+-rw-rw-rw-   0        0        0      557 2022-06-28 10:55:58.000000 pymycobot-3.1.2/pymycobot/log.py
+-rw-rw-rw-   0        0        0      206 2022-11-14 03:29:13.000000 pymycobot-3.1.2/pymycobot/mecharm.py
+-rw-rw-rw-   0        0        0     9015 2023-06-12 07:33:26.000000 pymycobot-3.1.2/pymycobot/myarm.py
+-rw-rw-rw-   0        0        0    13315 2023-04-14 05:34:53.000000 pymycobot-3.1.2/pymycobot/mybuddy.py
+-rw-rw-rw-   0        0        0     4768 2022-07-20 06:10:10.000000 pymycobot-3.1.2/pymycobot/mybuddybluetooth.py
+-rw-rw-rw-   0        0        0     4588 2022-10-14 05:56:03.000000 pymycobot-3.1.2/pymycobot/mybuddyemoticon.py
+-rw-rw-rw-   0        0        0     7190 2022-09-13 08:59:04.000000 pymycobot-3.1.2/pymycobot/mybuddysocket.py
+-rw-rw-rw-   0        0        0     7503 2023-06-15 06:42:39.000000 pymycobot-3.1.2/pymycobot/mycobot.py
+-rw-rw-rw-   0        0        0     7385 2023-06-09 07:23:49.000000 pymycobot-3.1.2/pymycobot/mycobotsocket.py
+-rw-rw-rw-   0        0        0     8483 2023-05-23 05:43:01.000000 pymycobot-3.1.2/pymycobot/mypalletizer.py
+-rw-rw-rw-   0        0        0     7500 2023-05-24 08:28:04.000000 pymycobot-3.1.2/pymycobot/mypalletizersocket.py
+-rw-rw-rw-   0        0        0    19631 2023-05-24 08:27:45.000000 pymycobot-3.1.2/pymycobot/ultraArm.py
+-rw-rw-rw-   0        0        0      674 2022-06-28 10:55:58.000000 pymycobot-3.1.2/pymycobot/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:11:33.691332 pymycobot-3.1.2/pymycobot.egg-info/
+-rw-rw-rw-   0        0        0    59099 2023-06-15 07:11:33.000000 pymycobot-3.1.2/pymycobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      674 2023-06-15 07:11:33.000000 pymycobot-3.1.2/pymycobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 07:11:33.000000 pymycobot-3.1.2/pymycobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-15 07:11:33.000000 pymycobot-3.1.2/pymycobot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-15 07:11:33.000000 pymycobot-3.1.2/pymycobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       26 2022-06-28 10:55:58.000000 pymycobot-3.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 07:11:33.695731 pymycobot-3.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     3055 2022-08-30 07:24:54.000000 pymycobot-3.1.2/setup.py
```

### Comparing `pymycobot-3.1.1/LICENSE` & `pymycobot-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.1/PKG-INFO` & `pymycobot-3.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.1.1
+Version: 3.1.2
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -89,40 +89,43 @@
 
 <details>
 <summary>Catalogue:</summary>
 
 <!-- vim-markdown-toc GFM -->
 
 - [pymycobot](#pymycobot)
-- [MyCobot / Mypalletizer / MechArm](#mycobot--mypalletizer--mecharm)
+- [MyCobot / Mypalletizer / MechArm / MyArm](#mycobot--mypalletizer--mecharm--myarm)
   - [Overall status](#overall-status)
     - [power\_on](#power_on)
     - [power\_off](#power_off)
     - [is\_power\_on](#is_power_on)
     - [read\_next\_error](#read_next_error)
     - [release\_all\_servos](#release_all_servos)
     - [is\_controller\_connected](#is_controller_connected)
     - [get\_error\_information](#get_error_information)
     - [clear\_error\_information](#clear_error_information)
   - [MDI mode and operation](#mdi-mode-and-operation)
     - [get\_angles](#get_angles)
     - [set\_fresh\_mode(mode)](#set_fresh_modemode)
+    - [get\_fresh\_mode()](#get_fresh_mode)
     - [send\_angle](#send_angle)
     - [send\_angles()](#send_angles)
     - [get\_radians](#get_radians)
     - [send\_radians](#send_radians)
     - [get\_coords](#get_coords)
     - [send\_coord](#send_coord)
     - [send\_coords](#send_coords)
     - [sync\_send\_angles](#sync_send_angles)
     - [sync\_send\_coords](#sync_send_coords)
     - [is\_in\_position](#is_in_position)
+    - [is\_moving](#is_moving)
   - [JOG mode and operation](#jog-mode-and-operation)
     - [jog\_angle](#jog_angle)
     - [jog\_coord](#jog_coord)
+    - [jog\_absolute](#jog_absolute)
     - [jog\_increment](#jog_increment)
     - [jog\_stop](#jog_stop)
     - [pause](#pause)
     - [resume](#resume)
     - [stop](#stop)
     - [is\_paused](#is_paused)
     - [set\_encoder](#set_encoder)
@@ -146,18 +149,18 @@
     - [focus\_servo](#focus_servo)
   - [Atom IO](#atom-io)
     - [set\_color](#set_color)
     - [set\_pin\_mode](#set_pin_mode)
     - [set\_digital\_output()](#set_digital_output)
     - [get\_digital\_input()](#get_digital_input)
     - [set\_pwm\_output()](#set_pwm_output)
+    - [set\_gripper\_calibration](#set_gripper_calibration)
     - [get\_gripper\_value](#get_gripper_value)
     - [set\_gripper\_state](#set_gripper_state)
     - [set\_gripper\_value](#set_gripper_value)
-    - [set\_gripper\_ini](#set_gripper_ini)
     - [is\_gripper\_moving](#is_gripper_moving)
     - [get\_basic\_input](#get_basic_input)
     - [set\_basic\_output](#set_basic_output)
     - [set\_ssid\_pwd](#set_ssid_pwd)
     - [get\_ssid\_pwd](#get_ssid_pwd)
     - [set\_server\_port](#set_server_port)
     - [get\_tof\_distance](#get_tof_distance)
@@ -179,16 +182,22 @@
     - [get\_servo\_speeds](#get_servo_speeds)
     - [get\_servo\_currents](#get_servo_currents)
     - [get\_servo\_voltages](#get_servo_voltages)
     - [get\_servo\_status](#get_servo_status)
     - [get\_servo\_temps](#get_servo_temps)
     - [init\_eletric\_gripper](#init_eletric_gripper)
     - [set\_eletric\_gripper](#set_eletric_gripper)
+    - [set\_gripper\_mode](#set_gripper_mode)
+    - [get\_gripper\_mode](#get_gripper_mode)
     - [set\_encoders\_drag](#set_encoders_drag)
-    - [set\_refresh\_mode](#set_refresh_mode)
+    - [get\_solution\_angles](#get_solution_angles)
+    - [set\_solution\_angles](#set_solution_angles)
+    - [joint\_brake](#joint_brake)
+    - [get\_transpoendr\_mode](#get_transpoendr_mode)
+    - [set\_transpoendr\_mode](#set_transpoendr_mode)
   - [Raspberry pi -- GPIO](#raspberry-pi----gpio)
     - [gpio\_init](#gpio_init)
     - [gpio\_output](#gpio_output)
 - [Angle](#angle)
 - [Coord](#coord)
 - [utils (Module)](#utils-module)
   - [get\_port\_list](#get_port_list)
@@ -310,15 +319,15 @@
     - [pause()](#pause-1)
     - [run()](#run)
     - [start()](#start)
   
 <!-- vim-markdown-toc -->
 </details>
 
-# MyCobot / Mypalletizer / MechArm
+# MyCobot / Mypalletizer / MechArm / MyArm
 
 **Import to your project**:
 
 ```python
 # for mycobot
 from pymycobot import MyCobot
 
@@ -428,14 +437,22 @@
 
 * **Parameters**
 
   * **mode** – int
     1 - Always execute the latest command first.
     0 - Execute instructions sequentially in the form of a queue.
 
+### get_fresh_mode()
+
+get command refresh mode
+
+  * **return**
+      - 1 - Always execute the latest command first.
+      - 0 - Execute instructions sequentially in the form of a queue.
+
 ### send_angle
 
 - **Prototype**: `send_angles(id, degree, speed)`
 
 - **Description**: Send one degree of joint to robot arm.
 
 - **Parameters**
@@ -600,14 +617,25 @@
 
 - **Returns**
 
   - `1` - true
   - `0` - false
   - `-1` - error
 
+### is_moving
+
+- **Prototype**: `is_moving()`
+
+- **Description**: Detect if the robot is moving.
+
+- **Returns**
+  - `1` - is moving
+  - `0` - not moving
+  - `-1` - error data
+
 ## JOG mode and operation
 
 ### jog_angle
 
 - **Prototype**: `jog_angle(joint_id, direction, speed)`
 
 - **Description**: Jog control angle
@@ -626,14 +654,29 @@
 
 - **Parameters**
 
   - `coord_id`: (`int`) 1 ~ 6
   - `direction`: `0` - decrease, `1` - increase
   - `speed`: 0 ~ 100
 
+### jog_absolute
+
+- **Prototype**: `jog_absolute(joint_id, angle, speed)`
+
+- **Description**: Jog absolute angle.
+
+- **Parameters**
+
+  - `joint_id`: (`int`) 
+    - for mycobot: int 1-6.
+    - for mypalletizer: int 1-4.
+    - for myArm: int 1 - 7.
+  - `direction`: 
+  - `speed`: 0 ~ 100
+
 ### jog_increment
 
 - **Prototype**: `jog_increment(coord_id, direction, speed)`
 
 - **Description**: Step mode.
 
 - **Parameters**
@@ -870,15 +913,15 @@
 - **Description**: Set the state mode of the specified pin in atom.
 - **Parameters**
 
   - `pin_no` (int): Pin number.
   - `pin_mode` (int): 0 - input, 1 - output, 2 - input_pullup
 
 ### set_digital_output()
-
+Set the terminal atom io status
 - **Parameters**
 
   - `pin_no` (int):
   - `pin_signal` (int): 0 / 1
 
 ### get_digital_input()
 
@@ -899,14 +942,21 @@
 
 - **Parameters**
 
   - `channel` (`int`): IO number.
   - `frequency` (`int`): clock frequency
   - `pin_val` (`int`): Duty cycle 0 ~ 256; 128 means 50%
 
+### set_gripper_calibration
+
+- **Prototype**: `set_gripper_calibration()`
+
+- **Description**: Set the current position to zero, set current position value is `2048`.
+
+
 ### get_gripper_value
 
 - **Prototype**: `get_gripper_value()`
 
 - **Description**: Get gripper value
 
 - **Return**: gripper value (int)
@@ -929,19 +979,19 @@
 - **Description**: Set gripper value
 
 - **Parameters**
 
   - `value` (int): 0 ~ 100
   - `speed` (int): 0 ~ 100
 
-### set_gripper_ini
+<!-- ### set_gripper_ini
 
 - **Prototype**: `set_gripper_ini()`
 
-- **Description**: Set the current position to zero, set current position value is `2048`.
+- **Description**: Set the current position to zero, set current position value is `2048`. -->
 
 ### is_gripper_moving
 
 - **Prototype**: `is_gripper_moving()`
 
 - **Description**: Judge whether the gripper is moving or not
 
@@ -1193,34 +1243,95 @@
 
 - **Description**: Set Electric Gripper Mode (only for 350).
 
 - **Parameters**
 
   - `status` (`int`): 0 - open, 1 - close.
 
+### set_gripper_mode
+
+- **Prototype**: `set_gripper_mode(status)`
+
+- **Description**: Set gripper mode.
+
+- **Parameters**
+
+  - `status` (`int`): 0 - transparent transmission. 1 - Port Mode.
+
+### get_gripper_mode
+
+- **Prototype**: `get_gripper_mode()`
+
+- **Description**: Get gripper mode.
+
+- **Return**
+
+  - `status` (`int`): 0 - transparent transmission. 1 - Port Mode.
+
 ### set_encoders_drag
 
 - **Prototype**: `set_encoders_drag(encoders, speeds)`
 
 - **Description**: Send all encoders and speeds
 
 - **Parameters**
 
   - `encoders` (`list`) : encoders list.
   - `speeds`: Obtained by the get_servo_speeds() method
 
-### set_refresh_mode
 
-- **Prototype**: `set_refresh_mode(mode)`
+### get_solution_angles
+
+- **Prototype**: `get_solution_angles()`
+
+- **Description**: Get zero space deflection angle value.(`This interface is only applicable to MyArm`)
+
+### set_solution_angles
+
+- **Prototype**: `set_solution_angles(angle, speed)`
+
+- **Description**: Set zero space deflection angle value.(`This interface is only applicable to MyArm`)
+
+- **Parameters**
+
+  - `angle`: Angle of joint 1.
+  - `speed`: 1 - 100.
+
+### joint_brake
+
+- **Prototype**: `joint_brake(joint_id)`
 
-- **Description**: Set command refresh mode
+- **Description**: Make it stop when the joint is in motion, and the buffer distance is positively related to the existing speed
 
 - **Parameters**
 
-  - `mode`: 0 - with interpolation  1 - No interpolation
+  - `joint_id`: 1 - 7.
+
+### get_transpoendr_mode
+
+- **Prototype**: `get_transpoendr_mode()`
+
+- **Description**: Obtain the configuration information of serial transmission mode.(`This interface is only applicable to MyArm`)
+
+- **Return**
+  - `0`: Turn off transparent transmission
+  - `1`: Turn on transparent transmission, verify all data
+  - `2`: Turn on transparent transmission, only verify communication forwarding mode configuration information (default is 0)
+
+### set_transpoendr_mode
+
+- **Prototype**: `set_transpoendr_mode(mode)`
+
+- **Description**: Set serial port transmission mode.(`This interface is only applicable to MyArm`)
+
+- **Parameters**
+  - `mode`:
+    - `0`: Turn off transparent transmission
+    - `1`: Turn on transparent transmission, verify all data
+    - `2`: Turn on transparent transmission, only verify communication forwarding mode configuration information
 
 ## Raspberry pi -- GPIO
 
 ### gpio_init
 
 - **Prototype**: `gpio_init()`
```

### Comparing `pymycobot-3.1.1/README.md` & `pymycobot-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.1/pymycobot/Interface.py` & `pymycobot-3.1.2/pymycobot/Interface.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.1/pymycobot/__init__.py` & `pymycobot-3.1.2/pymycobot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 ]
 
 
 if sys.platform == "linux":
     from pymycobot.mybuddyemoticon import MyBuddyEmoticon
     __all__.append("MyBuddyEmoticon")
 
-__version__ = "3.1.1"
+__version__ = "3.1.2"
 __author__ = "Elephantrobotics"
 __email__ = "weiquan.xu@elephantrobotics.com"
 __git_url__ = "https://github.com/elephantrobotics/pymycobot"
 __copyright__ = "CopyRight (c) 2020-{0} Shenzhen Elephantrobotics technology".format(
     datetime.datetime.now().year
 )
```

### Comparing `pymycobot-3.1.1/pymycobot/bluet.py` & `pymycobot-3.1.2/pymycobot/bluet.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.1/pymycobot/common.py` & `pymycobot-3.1.2/pymycobot/common.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.1/pymycobot/error.py` & `pymycobot-3.1.2/pymycobot/error.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.1/pymycobot/generate.py` & `pymycobot-3.1.2/pymycobot/generate.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         command_data = self._process_data_command(args)
 
         if genre == 178:
             # 修改wifi端口
             command_data = self._encode_int16(command_data)
             
         elif genre in [76, 77]:
-            command_data = [command_data[0]] + self._encode_int16(command_data[1])
+            command_data = [command_data[0]] + self._encode_int16(command_data[1]*10)
         elif genre == 115:
             command_data = [command_data[1],command_data[3]]
 
         LEN = len(command_data) + 2
         command = [
             ProtocolCode.HEADER,
             ProtocolCode.HEADER,
@@ -638,15 +638,15 @@
         Args:
             pin_no   (int): pin number.
             pin_mode (int): 0 - input, 1 - output, 2 - input_pullup
         """
         return self._mesg(ProtocolCode.SET_PIN_MODE, pin_no, pin_mode)
 
     def set_digital_output(self, pin_no, pin_signal):
-        """
+        """Set the terminal atom io status
 
         Args:
             pin_no     (int):
             pin_signal (int): 0 / 1
         """
         return self._mesg(ProtocolCode.SET_DIGITAL_OUTPUT, pin_no, pin_signal)
```

### Comparing `pymycobot-3.1.1/pymycobot/log.py` & `pymycobot-3.1.2/pymycobot/log.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.1/pymycobot/myarm.py` & `pymycobot-3.1.2/pymycobot/myarm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.1/pymycobot/mybuddy.py` & `pymycobot-3.1.2/pymycobot/mybuddy.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.1/pymycobot/mybuddybluetooth.py` & `pymycobot-3.1.2/pymycobot/mybuddybluetooth.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.1/pymycobot/mybuddyemoticon.py` & `pymycobot-3.1.2/pymycobot/mybuddyemoticon.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.1/pymycobot/mybuddysocket.py` & `pymycobot-3.1.2/pymycobot/mybuddysocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.1/pymycobot/mycobot.py` & `pymycobot-3.1.2/pymycobot/mycobot.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.1/pymycobot/mycobotsocket.py` & `pymycobot-3.1.2/pymycobot/mycobotsocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.1/pymycobot/mypalletizer.py` & `pymycobot-3.1.2/pymycobot/mypalletizer.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.1/pymycobot/mypalletizersocket.py` & `pymycobot-3.1.2/pymycobot/mypalletizersocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.1/pymycobot/ultraArm.py` & `pymycobot-3.1.2/pymycobot/ultraArm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.1/pymycobot/utils.py` & `pymycobot-3.1.2/pymycobot/utils.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.1/pymycobot.egg-info/PKG-INFO` & `pymycobot-3.1.2/pymycobot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.1.1
+Version: 3.1.2
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -89,40 +89,43 @@
 
 <details>
 <summary>Catalogue:</summary>
 
 <!-- vim-markdown-toc GFM -->
 
 - [pymycobot](#pymycobot)
-- [MyCobot / Mypalletizer / MechArm](#mycobot--mypalletizer--mecharm)
+- [MyCobot / Mypalletizer / MechArm / MyArm](#mycobot--mypalletizer--mecharm--myarm)
   - [Overall status](#overall-status)
     - [power\_on](#power_on)
     - [power\_off](#power_off)
     - [is\_power\_on](#is_power_on)
     - [read\_next\_error](#read_next_error)
     - [release\_all\_servos](#release_all_servos)
     - [is\_controller\_connected](#is_controller_connected)
     - [get\_error\_information](#get_error_information)
     - [clear\_error\_information](#clear_error_information)
   - [MDI mode and operation](#mdi-mode-and-operation)
     - [get\_angles](#get_angles)
     - [set\_fresh\_mode(mode)](#set_fresh_modemode)
+    - [get\_fresh\_mode()](#get_fresh_mode)
     - [send\_angle](#send_angle)
     - [send\_angles()](#send_angles)
     - [get\_radians](#get_radians)
     - [send\_radians](#send_radians)
     - [get\_coords](#get_coords)
     - [send\_coord](#send_coord)
     - [send\_coords](#send_coords)
     - [sync\_send\_angles](#sync_send_angles)
     - [sync\_send\_coords](#sync_send_coords)
     - [is\_in\_position](#is_in_position)
+    - [is\_moving](#is_moving)
   - [JOG mode and operation](#jog-mode-and-operation)
     - [jog\_angle](#jog_angle)
     - [jog\_coord](#jog_coord)
+    - [jog\_absolute](#jog_absolute)
     - [jog\_increment](#jog_increment)
     - [jog\_stop](#jog_stop)
     - [pause](#pause)
     - [resume](#resume)
     - [stop](#stop)
     - [is\_paused](#is_paused)
     - [set\_encoder](#set_encoder)
@@ -146,18 +149,18 @@
     - [focus\_servo](#focus_servo)
   - [Atom IO](#atom-io)
     - [set\_color](#set_color)
     - [set\_pin\_mode](#set_pin_mode)
     - [set\_digital\_output()](#set_digital_output)
     - [get\_digital\_input()](#get_digital_input)
     - [set\_pwm\_output()](#set_pwm_output)
+    - [set\_gripper\_calibration](#set_gripper_calibration)
     - [get\_gripper\_value](#get_gripper_value)
     - [set\_gripper\_state](#set_gripper_state)
     - [set\_gripper\_value](#set_gripper_value)
-    - [set\_gripper\_ini](#set_gripper_ini)
     - [is\_gripper\_moving](#is_gripper_moving)
     - [get\_basic\_input](#get_basic_input)
     - [set\_basic\_output](#set_basic_output)
     - [set\_ssid\_pwd](#set_ssid_pwd)
     - [get\_ssid\_pwd](#get_ssid_pwd)
     - [set\_server\_port](#set_server_port)
     - [get\_tof\_distance](#get_tof_distance)
@@ -179,16 +182,22 @@
     - [get\_servo\_speeds](#get_servo_speeds)
     - [get\_servo\_currents](#get_servo_currents)
     - [get\_servo\_voltages](#get_servo_voltages)
     - [get\_servo\_status](#get_servo_status)
     - [get\_servo\_temps](#get_servo_temps)
     - [init\_eletric\_gripper](#init_eletric_gripper)
     - [set\_eletric\_gripper](#set_eletric_gripper)
+    - [set\_gripper\_mode](#set_gripper_mode)
+    - [get\_gripper\_mode](#get_gripper_mode)
     - [set\_encoders\_drag](#set_encoders_drag)
-    - [set\_refresh\_mode](#set_refresh_mode)
+    - [get\_solution\_angles](#get_solution_angles)
+    - [set\_solution\_angles](#set_solution_angles)
+    - [joint\_brake](#joint_brake)
+    - [get\_transpoendr\_mode](#get_transpoendr_mode)
+    - [set\_transpoendr\_mode](#set_transpoendr_mode)
   - [Raspberry pi -- GPIO](#raspberry-pi----gpio)
     - [gpio\_init](#gpio_init)
     - [gpio\_output](#gpio_output)
 - [Angle](#angle)
 - [Coord](#coord)
 - [utils (Module)](#utils-module)
   - [get\_port\_list](#get_port_list)
@@ -310,15 +319,15 @@
     - [pause()](#pause-1)
     - [run()](#run)
     - [start()](#start)
   
 <!-- vim-markdown-toc -->
 </details>
 
-# MyCobot / Mypalletizer / MechArm
+# MyCobot / Mypalletizer / MechArm / MyArm
 
 **Import to your project**:
 
 ```python
 # for mycobot
 from pymycobot import MyCobot
 
@@ -428,14 +437,22 @@
 
 * **Parameters**
 
   * **mode** – int
     1 - Always execute the latest command first.
     0 - Execute instructions sequentially in the form of a queue.
 
+### get_fresh_mode()
+
+get command refresh mode
+
+  * **return**
+      - 1 - Always execute the latest command first.
+      - 0 - Execute instructions sequentially in the form of a queue.
+
 ### send_angle
 
 - **Prototype**: `send_angles(id, degree, speed)`
 
 - **Description**: Send one degree of joint to robot arm.
 
 - **Parameters**
@@ -600,14 +617,25 @@
 
 - **Returns**
 
   - `1` - true
   - `0` - false
   - `-1` - error
 
+### is_moving
+
+- **Prototype**: `is_moving()`
+
+- **Description**: Detect if the robot is moving.
+
+- **Returns**
+  - `1` - is moving
+  - `0` - not moving
+  - `-1` - error data
+
 ## JOG mode and operation
 
 ### jog_angle
 
 - **Prototype**: `jog_angle(joint_id, direction, speed)`
 
 - **Description**: Jog control angle
@@ -626,14 +654,29 @@
 
 - **Parameters**
 
   - `coord_id`: (`int`) 1 ~ 6
   - `direction`: `0` - decrease, `1` - increase
   - `speed`: 0 ~ 100
 
+### jog_absolute
+
+- **Prototype**: `jog_absolute(joint_id, angle, speed)`
+
+- **Description**: Jog absolute angle.
+
+- **Parameters**
+
+  - `joint_id`: (`int`) 
+    - for mycobot: int 1-6.
+    - for mypalletizer: int 1-4.
+    - for myArm: int 1 - 7.
+  - `direction`: 
+  - `speed`: 0 ~ 100
+
 ### jog_increment
 
 - **Prototype**: `jog_increment(coord_id, direction, speed)`
 
 - **Description**: Step mode.
 
 - **Parameters**
@@ -870,15 +913,15 @@
 - **Description**: Set the state mode of the specified pin in atom.
 - **Parameters**
 
   - `pin_no` (int): Pin number.
   - `pin_mode` (int): 0 - input, 1 - output, 2 - input_pullup
 
 ### set_digital_output()
-
+Set the terminal atom io status
 - **Parameters**
 
   - `pin_no` (int):
   - `pin_signal` (int): 0 / 1
 
 ### get_digital_input()
 
@@ -899,14 +942,21 @@
 
 - **Parameters**
 
   - `channel` (`int`): IO number.
   - `frequency` (`int`): clock frequency
   - `pin_val` (`int`): Duty cycle 0 ~ 256; 128 means 50%
 
+### set_gripper_calibration
+
+- **Prototype**: `set_gripper_calibration()`
+
+- **Description**: Set the current position to zero, set current position value is `2048`.
+
+
 ### get_gripper_value
 
 - **Prototype**: `get_gripper_value()`
 
 - **Description**: Get gripper value
 
 - **Return**: gripper value (int)
@@ -929,19 +979,19 @@
 - **Description**: Set gripper value
 
 - **Parameters**
 
   - `value` (int): 0 ~ 100
   - `speed` (int): 0 ~ 100
 
-### set_gripper_ini
+<!-- ### set_gripper_ini
 
 - **Prototype**: `set_gripper_ini()`
 
-- **Description**: Set the current position to zero, set current position value is `2048`.
+- **Description**: Set the current position to zero, set current position value is `2048`. -->
 
 ### is_gripper_moving
 
 - **Prototype**: `is_gripper_moving()`
 
 - **Description**: Judge whether the gripper is moving or not
 
@@ -1193,34 +1243,95 @@
 
 - **Description**: Set Electric Gripper Mode (only for 350).
 
 - **Parameters**
 
   - `status` (`int`): 0 - open, 1 - close.
 
+### set_gripper_mode
+
+- **Prototype**: `set_gripper_mode(status)`
+
+- **Description**: Set gripper mode.
+
+- **Parameters**
+
+  - `status` (`int`): 0 - transparent transmission. 1 - Port Mode.
+
+### get_gripper_mode
+
+- **Prototype**: `get_gripper_mode()`
+
+- **Description**: Get gripper mode.
+
+- **Return**
+
+  - `status` (`int`): 0 - transparent transmission. 1 - Port Mode.
+
 ### set_encoders_drag
 
 - **Prototype**: `set_encoders_drag(encoders, speeds)`
 
 - **Description**: Send all encoders and speeds
 
 - **Parameters**
 
   - `encoders` (`list`) : encoders list.
   - `speeds`: Obtained by the get_servo_speeds() method
 
-### set_refresh_mode
 
-- **Prototype**: `set_refresh_mode(mode)`
+### get_solution_angles
+
+- **Prototype**: `get_solution_angles()`
+
+- **Description**: Get zero space deflection angle value.(`This interface is only applicable to MyArm`)
+
+### set_solution_angles
+
+- **Prototype**: `set_solution_angles(angle, speed)`
+
+- **Description**: Set zero space deflection angle value.(`This interface is only applicable to MyArm`)
+
+- **Parameters**
+
+  - `angle`: Angle of joint 1.
+  - `speed`: 1 - 100.
+
+### joint_brake
+
+- **Prototype**: `joint_brake(joint_id)`
 
-- **Description**: Set command refresh mode
+- **Description**: Make it stop when the joint is in motion, and the buffer distance is positively related to the existing speed
 
 - **Parameters**
 
-  - `mode`: 0 - with interpolation  1 - No interpolation
+  - `joint_id`: 1 - 7.
+
+### get_transpoendr_mode
+
+- **Prototype**: `get_transpoendr_mode()`
+
+- **Description**: Obtain the configuration information of serial transmission mode.(`This interface is only applicable to MyArm`)
+
+- **Return**
+  - `0`: Turn off transparent transmission
+  - `1`: Turn on transparent transmission, verify all data
+  - `2`: Turn on transparent transmission, only verify communication forwarding mode configuration information (default is 0)
+
+### set_transpoendr_mode
+
+- **Prototype**: `set_transpoendr_mode(mode)`
+
+- **Description**: Set serial port transmission mode.(`This interface is only applicable to MyArm`)
+
+- **Parameters**
+  - `mode`:
+    - `0`: Turn off transparent transmission
+    - `1`: Turn on transparent transmission, verify all data
+    - `2`: Turn on transparent transmission, only verify communication forwarding mode configuration information
 
 ## Raspberry pi -- GPIO
 
 ### gpio_init
 
 - **Prototype**: `gpio_init()`
```

### Comparing `pymycobot-3.1.1/pymycobot.egg-info/SOURCES.txt` & `pymycobot-3.1.2/pymycobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymycobot-3.1.1/setup.py` & `pymycobot-3.1.2/setup.py`

 * *Files identical despite different names*

