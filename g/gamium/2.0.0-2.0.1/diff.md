# Comparing `tmp/gamium-2.0.0.tar.gz` & `tmp/gamium-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamium-2.0.0.tar", max compression
+gzip compressed data, was "gamium-2.0.1.tar", max compression
```

## Comparing `gamium-2.0.0.tar` & `gamium-2.0.1.tar`

### file list

```diff
@@ -1,104 +1,106 @@
--rw-r--r--   0        0        0     1007 2023-05-30 02:32:02.321529 gamium-2.0.0/README.md
--rw-r--r--   0        0        0      626 2023-05-25 07:46:40.594452 gamium-2.0.0/gamium/__init__.py
--rw-r--r--   0        0        0      500 2023-05-24 13:45:20.085940 gamium-2.0.0/gamium/__main__.py
--rw-r--r--   0        0        0    11229 2023-05-27 16:29:57.716876 gamium-2.0.0/gamium/actions/action_chain.py
--rw-r--r--   0        0        0     1449 2023-05-27 15:57:54.253933 gamium-2.0.0/gamium/actions/key_by.py
--rw-r--r--   0        0        0      471 2023-05-27 16:37:25.765448 gamium-2.0.0/gamium/condition/condition.py
--rw-r--r--   0        0        0     2138 2023-05-27 17:05:44.381885 gamium-2.0.0/gamium/condition/until.py
--rw-r--r--   0        0        0      245 2023-05-27 15:36:03.742756 gamium-2.0.0/gamium/condition/wait_condition.py
--rw-r--r--   0        0        0      269 2023-05-28 09:47:38.321943 gamium-2.0.0/gamium/errors/gamium_error.py
--rw-r--r--   0        0        0     6303 2023-05-27 16:57:16.462228 gamium-2.0.0/gamium/gamium_client.py
--rw-r--r--   0        0        0     8498 2023-05-27 16:29:22.380147 gamium-2.0.0/gamium/gamium_service.py
--rw-r--r--   0        0        0     1248 2023-05-27 16:48:14.859904 gamium-2.0.0/gamium/igamium_client.py
--rw-r--r--   0        0        0       62 2023-05-20 09:32:59.575340 gamium-2.0.0/gamium/internal/__init__.py
--rw-r--r--   0        0        0     1147 2023-05-20 09:32:59.575844 gamium-2.0.0/gamium/internal/logger.py
--rw-r--r--   0        0        0      672 2023-05-24 10:00:22.753241 gamium-2.0.0/gamium/internal/size_prefixed_recv_queue.py
--rw-r--r--   0        0        0      349 2023-05-27 15:45:16.895951 gamium-2.0.0/gamium/locator/by.py
--rw-r--r--   0        0        0       59 2023-05-20 09:32:59.576661 gamium-2.0.0/gamium/locator/locator.py
--rw-r--r--   0        0        0      906 2023-05-27 15:44:54.654718 gamium-2.0.0/gamium/locator/rpc_by.py
--rw-r--r--   0        0        0       47 2023-05-22 13:59:37.380671 gamium-2.0.0/gamium/locator/rpc_locator.py
--rw-r--r--   0        0        0     1996 2023-05-27 16:48:30.437448 gamium-2.0.0/gamium/object/player.py
--rw-r--r--   0        0        0     3925 2023-05-27 16:48:34.013675 gamium-2.0.0/gamium/object/ui_element.py
--rw-r--r--   0        0        0      390 2023-05-23 10:45:11.917741 gamium-2.0.0/gamium/options/__init__.py
--rw-r--r--   0        0        0      142 2023-05-27 16:07:06.395341 gamium-2.0.0/gamium/options/action_click_options.py
--rw-r--r--   0        0        0      204 2023-05-27 16:19:40.425215 gamium-2.0.0/gamium/options/action_drag_options.py
--rw-r--r--   0        0        0       92 2023-05-24 12:03:15.929711 gamium-2.0.0/gamium/options/action_move_options.py
--rw-r--r--   0        0        0      144 2023-05-27 16:20:01.758848 gamium-2.0.0/gamium/options/action_scroll_options.py
--rw-r--r--   0        0        0      171 2023-05-27 16:20:08.327138 gamium-2.0.0/gamium/options/execute_rpc_options.py
--rw-r--r--   0        0        0      132 2023-05-27 16:20:12.178882 gamium-2.0.0/gamium/options/find_objects_options.py
--rw-r--r--   0        0        0      374 2023-05-27 16:20:21.453410 gamium-2.0.0/gamium/options/move_player_options.py
--rw-r--r--   0        0        0      262 2023-05-27 16:20:28.044046 gamium-2.0.0/gamium/options/query_object_interactable_options.py
--rw-r--r--   0        0        0      139 2023-05-27 16:20:31.256151 gamium-2.0.0/gamium/options/send_key_options.py
--rw-r--r--   0        0        0       89 2023-05-22 09:57:37.806139 gamium-2.0.0/gamium/options/set_text_options.py
--rw-r--r--   0        0        0      362 2023-05-27 16:20:41.882990 gamium-2.0.0/gamium/options/wait_options.py
--rw-r--r--   0        0        0        0 2023-05-24 06:56:59.787754 gamium-2.0.0/gamium/protocol/__init__.py
--rw-r--r--   0        0        0      597 2023-05-27 15:36:07.575552 gamium-2.0.0/gamium/protocol/functions.py
--rw-r--r--   0        0        0     1988 2023-05-24 06:56:59.780237 gamium-2.0.0/gamium/protocol/generated/Packets/ActionParam.py
--rw-r--r--   0        0        0     4353 2023-05-24 06:56:59.778280 gamium-2.0.0/gamium/protocol/generated/Packets/ActionParamSingle.py
--rw-r--r--   0        0        0     2917 2023-05-24 06:56:59.787464 gamium-2.0.0/gamium/protocol/generated/Packets/ActionResult.py
--rw-r--r--   0        0        0     2909 2023-05-24 06:56:59.781650 gamium-2.0.0/gamium/protocol/generated/Packets/Actions/AppQuitParam.py
--rw-r--r--   0        0        0     4175 2023-05-24 06:56:59.782913 gamium-2.0.0/gamium/protocol/generated/Packets/Actions/InputKeyParam.py
--rw-r--r--   0        0        0     5031 2023-05-24 06:56:59.782321 gamium-2.0.0/gamium/protocol/generated/Packets/Actions/InputMouseParam.py
--rw-r--r--   0        0        0     3357 2023-05-24 06:56:59.783213 gamium-2.0.0/gamium/protocol/generated/Packets/Actions/InputSetTextParam.py
--rw-r--r--   0        0        0      156 2023-05-24 06:56:59.783916 gamium-2.0.0/gamium/protocol/generated/Packets/Actions/MovePlayerBy.py
--rw-r--r--   0        0        0     6404 2023-05-24 06:56:59.783443 gamium-2.0.0/gamium/protocol/generated/Packets/Actions/MovePlayerParam.py
--rw-r--r--   0        0        0     2213 2023-05-24 06:56:59.783639 gamium-2.0.0/gamium/protocol/generated/Packets/Actions/SleepParam.py
--rw-r--r--   0        0        0        0 2023-05-24 06:56:59.782546 gamium-2.0.0/gamium/protocol/generated/Packets/Actions/__init__.py
--rw-r--r--   0        0        0     3665 2023-05-24 06:56:59.776569 gamium-2.0.0/gamium/protocol/generated/Packets/ActionsParam.py
--rw-r--r--   0        0        0     4251 2023-05-24 06:56:59.772285 gamium-2.0.0/gamium/protocol/generated/Packets/ActionsResult.py
--rw-r--r--   0        0        0     3323 2023-05-24 06:56:59.786993 gamium-2.0.0/gamium/protocol/generated/Packets/ChangeConfigurationParam.py
--rw-r--r--   0        0        0     2116 2023-05-24 06:56:59.771624 gamium-2.0.0/gamium/protocol/generated/Packets/ChangeConfigurationResult.py
--rw-r--r--   0        0        0     3503 2023-05-24 06:56:59.785128 gamium-2.0.0/gamium/protocol/generated/Packets/DumpObjectsHierarchyParam.py
--rw-r--r--   0        0        0     4913 2023-05-24 06:56:59.786343 gamium-2.0.0/gamium/protocol/generated/Packets/DumpObjectsHierarchyResult.py
--rw-r--r--   0        0        0     2799 2023-05-24 06:56:59.773129 gamium-2.0.0/gamium/protocol/generated/Packets/Env.py
--rw-r--r--   0        0        0     6064 2023-05-24 06:56:59.776810 gamium-2.0.0/gamium/protocol/generated/Packets/ExecuteRpcParam.py
--rw-r--r--   0        0        0     2634 2023-05-24 06:56:59.771993 gamium-2.0.0/gamium/protocol/generated/Packets/ExecuteRpcResult.py
--rw-r--r--   0        0        0     3093 2023-05-24 06:56:59.774604 gamium-2.0.0/gamium/protocol/generated/Packets/FindObjectsParam.py
--rw-r--r--   0        0        0     4307 2023-05-24 06:56:59.775272 gamium-2.0.0/gamium/protocol/generated/Packets/FindObjectsResult.py
--rw-r--r--   0        0        0     2437 2023-05-24 06:56:59.785762 gamium-2.0.0/gamium/protocol/generated/Packets/HelloParam.py
--rw-r--r--   0        0        0     8271 2023-05-24 06:56:59.786610 gamium-2.0.0/gamium/protocol/generated/Packets/HelloResult.py
--rw-r--r--   0        0        0     4330 2023-05-24 06:56:59.781201 gamium-2.0.0/gamium/protocol/generated/Packets/InspectObjectOnScreenParam.py
--rw-r--r--   0        0        0     5826 2023-05-24 06:56:59.777393 gamium-2.0.0/gamium/protocol/generated/Packets/InspectObjectOnScreenResult.py
--rw-r--r--   0        0        0     2874 2023-05-24 06:56:59.774317 gamium-2.0.0/gamium/protocol/generated/Packets/InspectObjectWithIdParam.py
--rw-r--r--   0        0        0     3294 2023-05-24 06:56:59.772556 gamium-2.0.0/gamium/protocol/generated/Packets/InspectObjectWithIdResult.py
--rw-r--r--   0        0        0     4413 2023-05-24 06:56:59.780925 gamium-2.0.0/gamium/protocol/generated/Packets/QueryObjectInteractableParam.py
--rw-r--r--   0        0        0     2950 2023-05-24 06:56:59.786116 gamium-2.0.0/gamium/protocol/generated/Packets/QueryObjectInteractableResult.py
--rw-r--r--   0        0        0     1916 2023-05-24 06:56:59.774074 gamium-2.0.0/gamium/protocol/generated/Packets/QueryProfileParam.py
--rw-r--r--   0        0        0     2466 2023-05-24 06:56:59.773381 gamium-2.0.0/gamium/protocol/generated/Packets/QueryProfileResult.py
--rw-r--r--   0        0        0     1891 2023-05-24 06:56:59.779376 gamium-2.0.0/gamium/protocol/generated/Packets/QueryScreenParam.py
--rw-r--r--   0        0        0     3030 2023-05-24 06:56:59.787227 gamium-2.0.0/gamium/protocol/generated/Packets/QueryScreenResult.py
--rw-r--r--   0        0        0        0 2023-05-24 06:56:59.775993 gamium-2.0.0/gamium/protocol/generated/Packets/__init__.py
--rw-r--r--   0        0        0     3468 2023-05-24 06:56:59.766267 gamium-2.0.0/gamium/protocol/generated/Param.py
--rw-r--r--   0        0        0     5120 2023-05-24 06:56:59.765275 gamium-2.0.0/gamium/protocol/generated/Request.py
--rw-r--r--   0        0        0     6299 2023-05-24 06:56:59.768250 gamium-2.0.0/gamium/protocol/generated/Response.py
--rw-r--r--   0        0        0     3536 2023-05-24 06:56:59.770804 gamium-2.0.0/gamium/protocol/generated/Result.py
--rw-r--r--   0        0        0     3222 2023-05-24 06:56:59.755793 gamium-2.0.0/gamium/protocol/generated/Types/Configuration.py
--rw-r--r--   0        0        0     1146 2023-05-24 06:56:59.764593 gamium-2.0.0/gamium/protocol/generated/Types/ErrorCode.py
--rw-r--r--   0        0        0     2962 2023-05-24 06:56:59.756771 gamium-2.0.0/gamium/protocol/generated/Types/ErrorResult.py
--rw-r--r--   0        0        0      164 2023-05-24 06:56:59.764892 gamium-2.0.0/gamium/protocol/generated/Types/ExecuteRpcBy.py
--rw-r--r--   0        0        0      161 2023-05-24 06:56:59.761605 gamium-2.0.0/gamium/protocol/generated/Types/InputKeyBy.py
--rw-r--r--   0        0        0      147 2023-05-24 06:56:59.762868 gamium-2.0.0/gamium/protocol/generated/Types/InputKeyPressType.py
--rw-r--r--   0        0        0      168 2023-05-24 06:56:59.760225 gamium-2.0.0/gamium/protocol/generated/Types/InputMouseButtonCode.py
--rw-r--r--   0        0        0      177 2023-05-24 06:56:59.757942 gamium-2.0.0/gamium/protocol/generated/Types/InputMousePressType.py
--rw-r--r--   0        0        0     5920 2023-05-24 06:56:59.762417 gamium-2.0.0/gamium/protocol/generated/Types/ObjectHierarchyNode.py
--rw-r--r--   0        0        0    10803 2023-05-24 06:56:59.759371 gamium-2.0.0/gamium/protocol/generated/Types/ObjectInfo.py
--rw-r--r--   0        0        0     2955 2023-05-24 06:56:59.760908 gamium-2.0.0/gamium/protocol/generated/Types/ObjectLocator.py
--rw-r--r--   0        0        0      146 2023-05-24 06:56:59.763178 gamium-2.0.0/gamium/protocol/generated/Types/ObjectLocatorBy.py
--rw-r--r--   0        0        0      158 2023-05-24 06:56:59.756438 gamium-2.0.0/gamium/protocol/generated/Types/ObjectType.py
--rw-r--r--   0        0        0     5147 2023-05-24 06:56:59.755545 gamium-2.0.0/gamium/protocol/generated/Types/ObjectsHierarchy.py
--rw-r--r--   0        0        0     7471 2023-05-24 06:56:59.754685 gamium-2.0.0/gamium/protocol/generated/Types/Unity/UnityKeyCode.py
--rw-r--r--   0        0        0     1944 2023-05-24 06:56:59.755240 gamium-2.0.0/gamium/protocol/generated/Types/Unity/UnityKeyboard.py
--rw-r--r--   0        0        0        0 2023-05-24 06:56:59.754971 gamium-2.0.0/gamium/protocol/generated/Types/Unity/__init__.py
--rw-r--r--   0        0        0     1681 2023-05-24 06:56:59.757019 gamium-2.0.0/gamium/protocol/generated/Types/Vector2.py
--rw-r--r--   0        0        0     1947 2023-05-24 06:56:59.757558 gamium-2.0.0/gamium/protocol/generated/Types/Vector3.py
--rw-r--r--   0        0        0     2212 2023-05-24 06:56:59.758210 gamium-2.0.0/gamium/protocol/generated/Types/Vector4.py
--rw-r--r--   0        0        0        0 2023-05-24 06:56:59.757234 gamium-2.0.0/gamium/protocol/generated/Types/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 06:56:59.766005 gamium-2.0.0/gamium/protocol/generated/__init__.py
--rw-r--r--   0        0        0     3296 2023-05-29 05:36:44.760410 gamium-2.0.0/gamium/protocol/types.py
--rw-r--r--   0        0        0     3887 2023-05-27 16:45:21.559031 gamium-2.0.0/gamium/ui/ui.py
--rw-r--r--   0        0        0       80 2023-05-27 15:33:39.715322 gamium-2.0.0/gamium/utils/generics.py
--rw-r--r--   0        0        0       79 2023-05-24 13:28:31.670844 gamium-2.0.0/gamium/utils/time.py
--rw-r--r--   0        0        0      598 2023-05-27 16:56:44.654557 gamium-2.0.0/gamium/utils/try_utils.py
--rw-r--r--   0        0        0     1873 2023-05-27 17:12:44.836551 gamium-2.0.0/gamium/utils/wait.py
--rw-r--r--   0        0        0      278 2023-05-30 02:42:13.659978 gamium-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1429 1970-01-01 00:00:00.000000 gamium-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1007 2023-06-14 11:50:40.607475 gamium-2.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-14 11:59:45.413417 gamium-2.0.1/gamium/Protocol/__init__.py
+-rw-r--r--   0        0        0      597 2023-06-14 11:50:40.607909 gamium-2.0.1/gamium/Protocol/functions.py
+-rw-r--r--   0        0        0     1988 2023-06-14 11:59:45.407630 gamium-2.0.1/gamium/Protocol/generated/Packets/ActionParam.py
+-rw-r--r--   0        0        0     4353 2023-06-14 11:59:45.407148 gamium-2.0.1/gamium/Protocol/generated/Packets/ActionParamSingle.py
+-rw-r--r--   0        0        0     2917 2023-06-14 11:59:45.413162 gamium-2.0.1/gamium/Protocol/generated/Packets/ActionResult.py
+-rw-r--r--   0        0        0     2909 2023-06-14 11:59:45.408963 gamium-2.0.1/gamium/Protocol/generated/Packets/Actions/AppQuitParam.py
+-rw-r--r--   0        0        0     4175 2023-06-14 11:59:45.409943 gamium-2.0.1/gamium/Protocol/generated/Packets/Actions/InputKeyParam.py
+-rw-r--r--   0        0        0     5031 2023-06-14 11:59:45.409283 gamium-2.0.1/gamium/Protocol/generated/Packets/Actions/InputMouseParam.py
+-rw-r--r--   0        0        0     3357 2023-06-14 11:59:45.410280 gamium-2.0.1/gamium/Protocol/generated/Packets/Actions/InputSetTextParam.py
+-rw-r--r--   0        0        0      156 2023-06-14 11:59:45.411002 gamium-2.0.1/gamium/Protocol/generated/Packets/Actions/MovePlayerBy.py
+-rw-r--r--   0        0        0     6404 2023-06-14 11:59:45.410508 gamium-2.0.1/gamium/Protocol/generated/Packets/Actions/MovePlayerParam.py
+-rw-r--r--   0        0        0     2213 2023-06-14 11:59:45.410751 gamium-2.0.1/gamium/Protocol/generated/Packets/Actions/SleepParam.py
+-rw-r--r--   0        0        0        0 2023-06-14 11:59:45.409542 gamium-2.0.1/gamium/Protocol/generated/Packets/Actions/__init__.py
+-rw-r--r--   0        0        0     3665 2023-06-14 11:59:45.406358 gamium-2.0.1/gamium/Protocol/generated/Packets/ActionsParam.py
+-rw-r--r--   0        0        0     4251 2023-06-14 11:59:45.402853 gamium-2.0.1/gamium/Protocol/generated/Packets/ActionsResult.py
+-rw-r--r--   0        0        0     3323 2023-06-14 11:59:45.412560 gamium-2.0.1/gamium/Protocol/generated/Packets/ChangeConfigurationParam.py
+-rw-r--r--   0        0        0     2116 2023-06-14 11:59:45.402267 gamium-2.0.1/gamium/Protocol/generated/Packets/ChangeConfigurationResult.py
+-rw-r--r--   0        0        0     3503 2023-06-14 11:59:45.411302 gamium-2.0.1/gamium/Protocol/generated/Packets/DumpObjectsHierarchyParam.py
+-rw-r--r--   0        0        0     4913 2023-06-14 11:59:45.412047 gamium-2.0.1/gamium/Protocol/generated/Packets/DumpObjectsHierarchyResult.py
+-rw-r--r--   0        0        0     2799 2023-06-14 11:59:45.403403 gamium-2.0.1/gamium/Protocol/generated/Packets/Env.py
+-rw-r--r--   0        0        0     6064 2023-06-14 11:59:45.406652 gamium-2.0.1/gamium/Protocol/generated/Packets/ExecuteRpcParam.py
+-rw-r--r--   0        0        0     2634 2023-06-14 11:59:45.402566 gamium-2.0.1/gamium/Protocol/generated/Packets/ExecuteRpcResult.py
+-rw-r--r--   0        0        0     3093 2023-06-14 11:59:45.405499 gamium-2.0.1/gamium/Protocol/generated/Packets/FindObjectsParam.py
+-rw-r--r--   0        0        0     4307 2023-06-14 11:59:45.405841 gamium-2.0.1/gamium/Protocol/generated/Packets/FindObjectsResult.py
+-rw-r--r--   0        0        0     1941 2023-06-15 10:22:12.091336 gamium-2.0.1/gamium/Protocol/generated/Packets/GetPageSourceParam.py
+-rw-r--r--   0        0        0     2758 2023-06-15 10:22:12.091550 gamium-2.0.1/gamium/Protocol/generated/Packets/GetPageSourceResult.py
+-rw-r--r--   0        0        0     2437 2023-06-14 11:59:45.411552 gamium-2.0.1/gamium/Protocol/generated/Packets/HelloParam.py
+-rw-r--r--   0        0        0     8271 2023-06-14 11:59:45.412289 gamium-2.0.1/gamium/Protocol/generated/Packets/HelloResult.py
+-rw-r--r--   0        0        0     4330 2023-06-14 11:59:45.408172 gamium-2.0.1/gamium/Protocol/generated/Packets/InspectObjectOnScreenParam.py
+-rw-r--r--   0        0        0     5826 2023-06-14 11:59:45.406925 gamium-2.0.1/gamium/Protocol/generated/Packets/InspectObjectOnScreenResult.py
+-rw-r--r--   0        0        0     2874 2023-06-14 11:59:45.405007 gamium-2.0.1/gamium/Protocol/generated/Packets/InspectObjectWithIdParam.py
+-rw-r--r--   0        0        0     3294 2023-06-14 11:59:45.403128 gamium-2.0.1/gamium/Protocol/generated/Packets/InspectObjectWithIdResult.py
+-rw-r--r--   0        0        0     4413 2023-06-14 11:59:45.407902 gamium-2.0.1/gamium/Protocol/generated/Packets/QueryObjectInteractableParam.py
+-rw-r--r--   0        0        0     2950 2023-06-14 11:59:45.411794 gamium-2.0.1/gamium/Protocol/generated/Packets/QueryObjectInteractableResult.py
+-rw-r--r--   0        0        0     1916 2023-06-14 11:59:45.404713 gamium-2.0.1/gamium/Protocol/generated/Packets/QueryProfileParam.py
+-rw-r--r--   0        0        0     2466 2023-06-14 11:59:45.403789 gamium-2.0.1/gamium/Protocol/generated/Packets/QueryProfileResult.py
+-rw-r--r--   0        0        0     1891 2023-06-14 11:59:45.407377 gamium-2.0.1/gamium/Protocol/generated/Packets/QueryScreenParam.py
+-rw-r--r--   0        0        0     3030 2023-06-14 11:59:45.412918 gamium-2.0.1/gamium/Protocol/generated/Packets/QueryScreenResult.py
+-rw-r--r--   0        0        0        0 2023-06-14 11:59:45.406071 gamium-2.0.1/gamium/Protocol/generated/Packets/__init__.py
+-rw-r--r--   0        0        0     3752 2023-06-15 10:22:12.091870 gamium-2.0.1/gamium/Protocol/generated/Param.py
+-rw-r--r--   0        0        0     5254 2023-06-15 10:22:12.092092 gamium-2.0.1/gamium/Protocol/generated/Request.py
+-rw-r--r--   0        0        0     6436 2023-06-15 10:22:12.092491 gamium-2.0.1/gamium/Protocol/generated/Response.py
+-rw-r--r--   0        0        0     3826 2023-06-15 10:22:12.092670 gamium-2.0.1/gamium/Protocol/generated/Result.py
+-rw-r--r--   0        0        0     3222 2023-06-14 11:59:45.391446 gamium-2.0.1/gamium/Protocol/generated/Types/Configuration.py
+-rw-r--r--   0        0        0     1146 2023-06-14 11:59:45.399969 gamium-2.0.1/gamium/Protocol/generated/Types/ErrorCode.py
+-rw-r--r--   0        0        0     2962 2023-06-14 11:59:45.392202 gamium-2.0.1/gamium/Protocol/generated/Types/ErrorResult.py
+-rw-r--r--   0        0        0      164 2023-06-14 11:59:45.400261 gamium-2.0.1/gamium/Protocol/generated/Types/ExecuteRpcBy.py
+-rw-r--r--   0        0        0      161 2023-06-14 11:59:45.397831 gamium-2.0.1/gamium/Protocol/generated/Types/InputKeyBy.py
+-rw-r--r--   0        0        0      147 2023-06-14 11:59:45.399355 gamium-2.0.1/gamium/Protocol/generated/Types/InputKeyPressType.py
+-rw-r--r--   0        0        0      168 2023-06-14 11:59:45.397135 gamium-2.0.1/gamium/Protocol/generated/Types/InputMouseButtonCode.py
+-rw-r--r--   0        0        0      177 2023-06-14 11:59:45.393382 gamium-2.0.1/gamium/Protocol/generated/Types/InputMousePressType.py
+-rw-r--r--   0        0        0     5920 2023-06-14 11:59:45.398187 gamium-2.0.1/gamium/Protocol/generated/Types/ObjectHierarchyNode.py
+-rw-r--r--   0        0        0    10803 2023-06-14 11:59:45.394070 gamium-2.0.1/gamium/Protocol/generated/Types/ObjectInfo.py
+-rw-r--r--   0        0        0     2955 2023-06-14 11:59:45.397463 gamium-2.0.1/gamium/Protocol/generated/Types/ObjectLocator.py
+-rw-r--r--   0        0        0      146 2023-06-14 11:59:45.399660 gamium-2.0.1/gamium/Protocol/generated/Types/ObjectLocatorBy.py
+-rw-r--r--   0        0        0      158 2023-06-14 11:59:45.391879 gamium-2.0.1/gamium/Protocol/generated/Types/ObjectType.py
+-rw-r--r--   0        0        0     5147 2023-06-14 11:59:45.391131 gamium-2.0.1/gamium/Protocol/generated/Types/ObjectsHierarchy.py
+-rw-r--r--   0        0        0     7471 2023-06-14 11:59:45.390142 gamium-2.0.1/gamium/Protocol/generated/Types/Unity/UnityKeyCode.py
+-rw-r--r--   0        0        0     1944 2023-06-14 11:59:45.390771 gamium-2.0.1/gamium/Protocol/generated/Types/Unity/UnityKeyboard.py
+-rw-r--r--   0        0        0        0 2023-06-14 11:59:45.390471 gamium-2.0.1/gamium/Protocol/generated/Types/Unity/__init__.py
+-rw-r--r--   0        0        0     1681 2023-06-14 11:59:45.392495 gamium-2.0.1/gamium/Protocol/generated/Types/Vector2.py
+-rw-r--r--   0        0        0     1947 2023-06-14 11:59:45.393090 gamium-2.0.1/gamium/Protocol/generated/Types/Vector3.py
+-rw-r--r--   0        0        0     2212 2023-06-14 11:59:45.393747 gamium-2.0.1/gamium/Protocol/generated/Types/Vector4.py
+-rw-r--r--   0        0        0        0 2023-06-14 11:59:45.392754 gamium-2.0.1/gamium/Protocol/generated/Types/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 11:59:45.400870 gamium-2.0.1/gamium/Protocol/generated/__init__.py
+-rw-r--r--   0        0        0     3296 2023-06-14 11:50:40.613066 gamium-2.0.1/gamium/Protocol/types.py
+-rw-r--r--   0        0        0      626 2023-06-14 11:50:40.613159 gamium-2.0.1/gamium/__init__.py
+-rw-r--r--   0        0        0      500 2023-06-14 11:50:40.613219 gamium-2.0.1/gamium/__main__.py
+-rw-r--r--   0        0        0    11229 2023-06-14 11:50:40.613344 gamium-2.0.1/gamium/actions/action_chain.py
+-rw-r--r--   0        0        0     1449 2023-06-14 11:50:40.613418 gamium-2.0.1/gamium/actions/key_by.py
+-rw-r--r--   0        0        0      471 2023-06-14 11:50:40.613535 gamium-2.0.1/gamium/condition/condition.py
+-rw-r--r--   0        0        0     2138 2023-06-14 11:50:40.613608 gamium-2.0.1/gamium/condition/until.py
+-rw-r--r--   0        0        0      245 2023-06-14 11:50:40.613675 gamium-2.0.1/gamium/condition/wait_condition.py
+-rw-r--r--   0        0        0      269 2023-06-14 11:50:40.613784 gamium-2.0.1/gamium/errors/gamium_error.py
+-rw-r--r--   0        0        0     6303 2023-06-14 11:50:40.613864 gamium-2.0.1/gamium/gamium_client.py
+-rw-r--r--   0        0        0     8498 2023-06-14 11:50:40.613955 gamium-2.0.1/gamium/gamium_service.py
+-rw-r--r--   0        0        0     1248 2023-06-14 11:50:40.614021 gamium-2.0.1/gamium/igamium_client.py
+-rw-r--r--   0        0        0       62 2023-06-14 11:50:40.614114 gamium-2.0.1/gamium/internal/__init__.py
+-rw-r--r--   0        0        0     1147 2023-06-14 11:50:40.614187 gamium-2.0.1/gamium/internal/logger.py
+-rw-r--r--   0        0        0      672 2023-06-14 11:50:40.614244 gamium-2.0.1/gamium/internal/size_prefixed_recv_queue.py
+-rw-r--r--   0        0        0      349 2023-06-14 11:50:40.614339 gamium-2.0.1/gamium/locator/by.py
+-rw-r--r--   0        0        0       59 2023-06-14 11:50:40.614392 gamium-2.0.1/gamium/locator/locator.py
+-rw-r--r--   0        0        0      906 2023-06-14 11:50:40.614465 gamium-2.0.1/gamium/locator/rpc_by.py
+-rw-r--r--   0        0        0       47 2023-06-14 11:50:40.614515 gamium-2.0.1/gamium/locator/rpc_locator.py
+-rw-r--r--   0        0        0     1996 2023-06-14 11:50:40.614611 gamium-2.0.1/gamium/object/player.py
+-rw-r--r--   0        0        0     3925 2023-06-14 11:50:40.614688 gamium-2.0.1/gamium/object/ui_element.py
+-rw-r--r--   0        0        0      390 2023-06-14 11:50:40.614806 gamium-2.0.1/gamium/options/__init__.py
+-rw-r--r--   0        0        0      142 2023-06-14 11:50:40.614872 gamium-2.0.1/gamium/options/action_click_options.py
+-rw-r--r--   0        0        0      204 2023-06-14 11:50:40.614933 gamium-2.0.1/gamium/options/action_drag_options.py
+-rw-r--r--   0        0        0       92 2023-06-14 11:50:40.614988 gamium-2.0.1/gamium/options/action_move_options.py
+-rw-r--r--   0        0        0      144 2023-06-14 11:50:40.615054 gamium-2.0.1/gamium/options/action_scroll_options.py
+-rw-r--r--   0        0        0      171 2023-06-14 11:50:40.615119 gamium-2.0.1/gamium/options/execute_rpc_options.py
+-rw-r--r--   0        0        0      132 2023-06-14 11:50:40.615176 gamium-2.0.1/gamium/options/find_objects_options.py
+-rw-r--r--   0        0        0      374 2023-06-14 11:50:40.615231 gamium-2.0.1/gamium/options/move_player_options.py
+-rw-r--r--   0        0        0      262 2023-06-14 11:50:40.615305 gamium-2.0.1/gamium/options/query_object_interactable_options.py
+-rw-r--r--   0        0        0      139 2023-06-14 11:50:40.615367 gamium-2.0.1/gamium/options/send_key_options.py
+-rw-r--r--   0        0        0       89 2023-06-14 11:50:40.615419 gamium-2.0.1/gamium/options/set_text_options.py
+-rw-r--r--   0        0        0      362 2023-06-14 11:50:40.615480 gamium-2.0.1/gamium/options/wait_options.py
+-rw-r--r--   0        0        0     3887 2023-06-14 11:50:40.615607 gamium-2.0.1/gamium/ui/ui.py
+-rw-r--r--   0        0        0       80 2023-06-14 11:50:40.615691 gamium-2.0.1/gamium/utils/generics.py
+-rw-r--r--   0        0        0       79 2023-06-14 11:50:40.615755 gamium-2.0.1/gamium/utils/time.py
+-rw-r--r--   0        0        0      598 2023-06-14 11:50:40.615818 gamium-2.0.1/gamium/utils/try_utils.py
+-rw-r--r--   0        0        0     1873 2023-06-14 11:50:40.615906 gamium-2.0.1/gamium/utils/wait.py
+-rw-r--r--   0        0        0      278 2023-06-15 10:22:12.092829 gamium-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1429 1970-01-01 00:00:00.000000 gamium-2.0.1/PKG-INFO
```

### Comparing `gamium-2.0.0/README.md` & `gamium-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/__init__.py` & `gamium-2.0.1/gamium/__init__.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/actions/action_chain.py` & `gamium-2.0.1/gamium/actions/action_chain.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/actions/key_by.py` & `gamium-2.0.1/gamium/actions/key_by.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/condition/until.py` & `gamium-2.0.1/gamium/condition/until.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/gamium_client.py` & `gamium-2.0.1/gamium/gamium_client.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/gamium_service.py` & `gamium-2.0.1/gamium/gamium_service.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/igamium_client.py` & `gamium-2.0.1/gamium/igamium_client.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/internal/logger.py` & `gamium-2.0.1/gamium/internal/logger.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/internal/size_prefixed_recv_queue.py` & `gamium-2.0.1/gamium/internal/size_prefixed_recv_queue.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/locator/rpc_by.py` & `gamium-2.0.1/gamium/locator/rpc_by.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/object/player.py` & `gamium-2.0.1/gamium/object/player.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/object/ui_element.py` & `gamium-2.0.1/gamium/object/ui_element.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/functions.py` & `gamium-2.0.1/gamium/Protocol/functions.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/ActionParam.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/ActionParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/ActionParamSingle.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/ActionParamSingle.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/ActionResult.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/ActionResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/Actions/AppQuitParam.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/Actions/AppQuitParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/Actions/InputKeyParam.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/Actions/InputKeyParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/Actions/InputMouseParam.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/Actions/InputMouseParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/Actions/InputSetTextParam.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/Actions/InputSetTextParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/Actions/MovePlayerParam.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/Actions/MovePlayerParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/Actions/SleepParam.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/Actions/SleepParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/ActionsParam.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/ActionsParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/ActionsResult.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/ActionsResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/ChangeConfigurationParam.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/ChangeConfigurationParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/ChangeConfigurationResult.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/ChangeConfigurationResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/DumpObjectsHierarchyParam.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/DumpObjectsHierarchyParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/DumpObjectsHierarchyResult.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/DumpObjectsHierarchyResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/Env.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/Env.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/ExecuteRpcParam.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/ExecuteRpcParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/ExecuteRpcResult.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/ExecuteRpcResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/FindObjectsParam.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/FindObjectsParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/FindObjectsResult.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/FindObjectsResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/HelloParam.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/HelloParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/HelloResult.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/HelloResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/InspectObjectOnScreenParam.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/InspectObjectOnScreenParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/InspectObjectOnScreenResult.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/InspectObjectOnScreenResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/InspectObjectWithIdParam.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/InspectObjectWithIdParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/InspectObjectWithIdResult.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/InspectObjectWithIdResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/QueryObjectInteractableParam.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/QueryObjectInteractableParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/QueryObjectInteractableResult.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/QueryObjectInteractableResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/QueryProfileParam.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/QueryProfileParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/QueryProfileResult.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/QueryProfileResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/QueryScreenParam.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/QueryScreenParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Packets/QueryScreenResult.py` & `gamium-2.0.1/gamium/Protocol/generated/Packets/QueryScreenResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Param.py` & `gamium-2.0.1/gamium/Protocol/generated/Param.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     Packets_ActionsParam = 5
     Packets_ExecuteRpcParam = 6
     Packets_InspectObjectOnScreenParam = 7
     Packets_InspectObjectWithIdParam = 8
     Packets_DumpObjectsHierarchyParam = 9
     Packets_ChangeConfigurationParam = 10
     Packets_QueryProfileParam = 11
+    Packets_GetPageSourceParam = 12
 
 def ParamCreator(unionType, table):
     from flatbuffers.table import Table
     if not isinstance(table, Table):
         return None
     if unionType == Param().Packets_HelloParam:
         import gamium.protocol.generated.Packets.HelloParam
@@ -49,8 +50,11 @@
         return gamium.protocol.generated.Packets.DumpObjectsHierarchyParam.DumpObjectsHierarchyParamT.InitFromBuf(table.Bytes, table.Pos)
     if unionType == Param().Packets_ChangeConfigurationParam:
         import gamium.protocol.generated.Packets.ChangeConfigurationParam
         return gamium.protocol.generated.Packets.ChangeConfigurationParam.ChangeConfigurationParamT.InitFromBuf(table.Bytes, table.Pos)
     if unionType == Param().Packets_QueryProfileParam:
         import gamium.protocol.generated.Packets.QueryProfileParam
         return gamium.protocol.generated.Packets.QueryProfileParam.QueryProfileParamT.InitFromBuf(table.Bytes, table.Pos)
+    if unionType == Param().Packets_GetPageSourceParam:
+        import gamium.protocol.generated.Packets.GetPageSourceParam
+        return gamium.protocol.generated.Packets.GetPageSourceParam.GetPageSourceParamT.InitFromBuf(table.Bytes, table.Pos)
     return None
```

### Comparing `gamium-2.0.0/gamium/protocol/generated/Request.py` & `gamium-2.0.1/gamium/Protocol/generated/Request.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 def End(builder):
     return RequestEnd(builder)
 import gamium.protocol.generated.Packets.ActionsParam
 import gamium.protocol.generated.Packets.ChangeConfigurationParam
 import gamium.protocol.generated.Packets.DumpObjectsHierarchyParam
 import gamium.protocol.generated.Packets.ExecuteRpcParam
 import gamium.protocol.generated.Packets.FindObjectsParam
+import gamium.protocol.generated.Packets.GetPageSourceParam
 import gamium.protocol.generated.Packets.HelloParam
 import gamium.protocol.generated.Packets.InspectObjectOnScreenParam
 import gamium.protocol.generated.Packets.InspectObjectWithIdParam
 import gamium.protocol.generated.Packets.QueryObjectInteractableParam
 import gamium.protocol.generated.Packets.QueryProfileParam
 import gamium.protocol.generated.Packets.QueryScreenParam
 import gamium.protocol.generated.Param
@@ -82,15 +83,15 @@
 
 class RequestT(object):
 
     # RequestT
     def __init__(self):
         self.seq = 0  # type: int
         self.paramType = 0  # type: int
-        self.param = None  # type: Union[None, gamium.protocol.generated.Packets.HelloParam.HelloParamT, gamium.protocol.generated.Packets.QueryScreenParam.QueryScreenParamT, gamium.protocol.generated.Packets.FindObjectsParam.FindObjectsParamT, gamium.protocol.generated.Packets.QueryObjectInteractableParam.QueryObjectInteractableParamT, gamium.protocol.generated.Packets.ActionsParam.ActionsParamT, gamium.protocol.generated.Packets.ExecuteRpcParam.ExecuteRpcParamT, gamium.protocol.generated.Packets.InspectObjectOnScreenParam.InspectObjectOnScreenParamT, gamium.protocol.generated.Packets.InspectObjectWithIdParam.InspectObjectWithIdParamT, gamium.protocol.generated.Packets.DumpObjectsHierarchyParam.DumpObjectsHierarchyParamT, gamium.protocol.generated.Packets.ChangeConfigurationParam.ChangeConfigurationParamT, gamium.protocol.generated.Packets.QueryProfileParam.QueryProfileParamT]
+        self.param = None  # type: Union[None, gamium.protocol.generated.Packets.HelloParam.HelloParamT, gamium.protocol.generated.Packets.QueryScreenParam.QueryScreenParamT, gamium.protocol.generated.Packets.FindObjectsParam.FindObjectsParamT, gamium.protocol.generated.Packets.QueryObjectInteractableParam.QueryObjectInteractableParamT, gamium.protocol.generated.Packets.ActionsParam.ActionsParamT, gamium.protocol.generated.Packets.ExecuteRpcParam.ExecuteRpcParamT, gamium.protocol.generated.Packets.InspectObjectOnScreenParam.InspectObjectOnScreenParamT, gamium.protocol.generated.Packets.InspectObjectWithIdParam.InspectObjectWithIdParamT, gamium.protocol.generated.Packets.DumpObjectsHierarchyParam.DumpObjectsHierarchyParamT, gamium.protocol.generated.Packets.ChangeConfigurationParam.ChangeConfigurationParamT, gamium.protocol.generated.Packets.QueryProfileParam.QueryProfileParamT, gamium.protocol.generated.Packets.GetPageSourceParam.GetPageSourceParamT]
 
     @classmethod
     def InitFromBuf(cls, buf, pos):
         request = Request()
         request.Init(buf, pos)
         return cls.InitFromObj(request)
```

### Comparing `gamium-2.0.0/gamium/protocol/generated/Response.py` & `gamium-2.0.1/gamium/Protocol/generated/Response.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 def End(builder):
     return ResponseEnd(builder)
 import gamium.protocol.generated.Packets.ActionsResult
 import gamium.protocol.generated.Packets.ChangeConfigurationResult
 import gamium.protocol.generated.Packets.DumpObjectsHierarchyResult
 import gamium.protocol.generated.Packets.ExecuteRpcResult
 import gamium.protocol.generated.Packets.FindObjectsResult
+import gamium.protocol.generated.Packets.GetPageSourceResult
 import gamium.protocol.generated.Packets.HelloResult
 import gamium.protocol.generated.Packets.InspectObjectOnScreenResult
 import gamium.protocol.generated.Packets.InspectObjectWithIdResult
 import gamium.protocol.generated.Packets.QueryObjectInteractableResult
 import gamium.protocol.generated.Packets.QueryProfileResult
 import gamium.protocol.generated.Packets.QueryScreenResult
 import gamium.protocol.generated.Result
@@ -98,15 +99,15 @@
 class ResponseT(object):
 
     # ResponseT
     def __init__(self):
         self.seq = 0  # type: int
         self.error = None  # type: Optional[gamium.protocol.generated.Types.ErrorResult.ErrorResultT]
         self.resultType = 0  # type: int
-        self.result = None  # type: Union[None, gamium.protocol.generated.Packets.HelloResult.HelloResultT, gamium.protocol.generated.Packets.QueryScreenResult.QueryScreenResultT, gamium.protocol.generated.Packets.FindObjectsResult.FindObjectsResultT, gamium.protocol.generated.Packets.QueryObjectInteractableResult.QueryObjectInteractableResultT, gamium.protocol.generated.Packets.ActionsResult.ActionsResultT, gamium.protocol.generated.Packets.ExecuteRpcResult.ExecuteRpcResultT, gamium.protocol.generated.Packets.InspectObjectOnScreenResult.InspectObjectOnScreenResultT, gamium.protocol.generated.Packets.InspectObjectWithIdResult.InspectObjectWithIdResultT, gamium.protocol.generated.Packets.DumpObjectsHierarchyResult.DumpObjectsHierarchyResultT, gamium.protocol.generated.Packets.ChangeConfigurationResult.ChangeConfigurationResultT, gamium.protocol.generated.Packets.QueryProfileResult.QueryProfileResultT]
+        self.result = None  # type: Union[None, gamium.protocol.generated.Packets.HelloResult.HelloResultT, gamium.protocol.generated.Packets.QueryScreenResult.QueryScreenResultT, gamium.protocol.generated.Packets.FindObjectsResult.FindObjectsResultT, gamium.protocol.generated.Packets.QueryObjectInteractableResult.QueryObjectInteractableResultT, gamium.protocol.generated.Packets.ActionsResult.ActionsResultT, gamium.protocol.generated.Packets.ExecuteRpcResult.ExecuteRpcResultT, gamium.protocol.generated.Packets.InspectObjectOnScreenResult.InspectObjectOnScreenResultT, gamium.protocol.generated.Packets.InspectObjectWithIdResult.InspectObjectWithIdResultT, gamium.protocol.generated.Packets.DumpObjectsHierarchyResult.DumpObjectsHierarchyResultT, gamium.protocol.generated.Packets.ChangeConfigurationResult.ChangeConfigurationResultT, gamium.protocol.generated.Packets.QueryProfileResult.QueryProfileResultT, gamium.protocol.generated.Packets.GetPageSourceResult.GetPageSourceResultT]
 
     @classmethod
     def InitFromBuf(cls, buf, pos):
         response = Response()
         response.Init(buf, pos)
         return cls.InitFromObj(response)
```

### Comparing `gamium-2.0.0/gamium/protocol/generated/Result.py` & `gamium-2.0.1/gamium/Protocol/generated/Result.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     Packets_ActionsResult = 5
     Packets_ExecuteRpcResult = 6
     Packets_InspectObjectOnScreenResult = 7
     Packets_InspectObjectWithIdResult = 8
     Packets_DumpObjectsHierarchyResult = 9
     Packets_ChangeConfigurationResult = 10
     Packets_QueryProfileResult = 11
+    Packets_GetPageSourceResult = 12
 
 def ResultCreator(unionType, table):
     from flatbuffers.table import Table
     if not isinstance(table, Table):
         return None
     if unionType == Result().Packets_HelloResult:
         import gamium.protocol.generated.Packets.HelloResult
@@ -49,8 +50,11 @@
         return gamium.protocol.generated.Packets.DumpObjectsHierarchyResult.DumpObjectsHierarchyResultT.InitFromBuf(table.Bytes, table.Pos)
     if unionType == Result().Packets_ChangeConfigurationResult:
         import gamium.protocol.generated.Packets.ChangeConfigurationResult
         return gamium.protocol.generated.Packets.ChangeConfigurationResult.ChangeConfigurationResultT.InitFromBuf(table.Bytes, table.Pos)
     if unionType == Result().Packets_QueryProfileResult:
         import gamium.protocol.generated.Packets.QueryProfileResult
         return gamium.protocol.generated.Packets.QueryProfileResult.QueryProfileResultT.InitFromBuf(table.Bytes, table.Pos)
+    if unionType == Result().Packets_GetPageSourceResult:
+        import gamium.protocol.generated.Packets.GetPageSourceResult
+        return gamium.protocol.generated.Packets.GetPageSourceResult.GetPageSourceResultT.InitFromBuf(table.Bytes, table.Pos)
     return None
```

### Comparing `gamium-2.0.0/gamium/protocol/generated/Types/Configuration.py` & `gamium-2.0.1/gamium/Protocol/generated/Types/Configuration.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Types/ErrorCode.py` & `gamium-2.0.1/gamium/Protocol/generated/Types/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Types/ErrorResult.py` & `gamium-2.0.1/gamium/Protocol/generated/Types/ErrorResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Types/ObjectHierarchyNode.py` & `gamium-2.0.1/gamium/Protocol/generated/Types/ObjectHierarchyNode.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Types/ObjectInfo.py` & `gamium-2.0.1/gamium/Protocol/generated/Types/ObjectInfo.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Types/ObjectLocator.py` & `gamium-2.0.1/gamium/Protocol/generated/Types/ObjectLocator.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Types/ObjectsHierarchy.py` & `gamium-2.0.1/gamium/Protocol/generated/Types/ObjectsHierarchy.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Types/Unity/UnityKeyCode.py` & `gamium-2.0.1/gamium/Protocol/generated/Types/Unity/UnityKeyCode.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Types/Unity/UnityKeyboard.py` & `gamium-2.0.1/gamium/Protocol/generated/Types/Unity/UnityKeyboard.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Types/Vector2.py` & `gamium-2.0.1/gamium/Protocol/generated/Types/Vector2.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Types/Vector3.py` & `gamium-2.0.1/gamium/Protocol/generated/Types/Vector3.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/generated/Types/Vector4.py` & `gamium-2.0.1/gamium/Protocol/generated/Types/Vector4.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/protocol/types.py` & `gamium-2.0.1/gamium/Protocol/types.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/ui/ui.py` & `gamium-2.0.1/gamium/ui/ui.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/utils/try_utils.py` & `gamium-2.0.1/gamium/utils/try_utils.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/gamium/utils/wait.py` & `gamium-2.0.1/gamium/utils/wait.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.0/PKG-INFO` & `gamium-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamium
-Version: 2.0.0
+Version: 2.0.1
 Summary: 
 Author: dogu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

