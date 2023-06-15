# Comparing `tmp/xoa-utils-1.2.1.tar.gz` & `tmp/xoa-utils-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xoa-utils-1.2.1.tar", last modified: Thu Apr 27 18:51:46 2023, max compression
+gzip compressed data, was "xoa-utils-2.0.0.tar", last modified: Thu Jun 15 09:57:01 2023, max compression
```

## Comparing `xoa-utils-1.2.1.tar` & `xoa-utils-2.0.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:51:46.769476 xoa-utils-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-27 18:51:30.000000 xoa-utils-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-27 18:51:46.769476 xoa-utils-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-27 18:51:30.000000 xoa-utils-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 18:51:46.773476 xoa-utils-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-27 18:51:31.000000 xoa-utils-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:51:46.761476 xoa-utils-1.2.1/xoa_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-27 18:51:31.000000 xoa-utils-1.2.1/xoa_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:51:46.765476 xoa-utils-1.2.1/xoa_utils/clicks/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-27 18:51:31.000000 xoa-utils-1.2.1/xoa_utils/clicks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-27 18:51:31.000000 xoa-utils-1.2.1/xoa_utils/clicks/click_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:51:46.769476 xoa-utils-1.2.1/xoa_utils/clicks/click_commands/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-27 18:51:31.000000 xoa-utils-1.2.1/xoa_utils/clicks/click_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-27 18:51:31.000000 xoa-utils-1.2.1/xoa_utils/clicks/click_commands/an.py
--rw-r--r--   0 runner    (1001) docker     (123)    16236 2023-04-27 18:51:31.000000 xoa-utils-1.2.1/xoa_utils/clicks/click_commands/anlt.py
--rw-r--r--   0 runner    (1001) docker     (123)    27448 2023-04-27 18:51:31.000000 xoa-utils-1.2.1/xoa_utils/clicks/click_commands/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-27 18:51:31.000000 xoa-utils-1.2.1/xoa_utils/clicks/click_commands/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10833 2023-04-27 18:51:31.000000 xoa-utils-1.2.1/xoa_utils/clicks/click_commands/lt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9068 2023-04-27 18:51:31.000000 xoa-utils-1.2.1/xoa_utils/clicks/click_commands/management.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-27 18:51:31.000000 xoa-utils-1.2.1/xoa_utils/clicks/click_help.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:51:46.769476 xoa-utils-1.2.1/xoa_utils/clis/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-27 18:51:31.000000 xoa-utils-1.2.1/xoa_utils/clis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16187 2023-04-27 18:51:31.000000 xoa-utils-1.2.1/xoa_utils/clis/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:51:46.769476 xoa-utils-1.2.1/xoa_utils/cmds/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-27 18:51:31.000000 xoa-utils-1.2.1/xoa_utils/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12158 2023-04-27 18:51:31.000000 xoa-utils-1.2.1/xoa_utils/cmds/cmd_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-04-27 18:51:31.000000 xoa-utils-1.2.1/xoa_utils/cmds/cmd_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-27 18:51:31.000000 xoa-utils-1.2.1/xoa_utils/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:51:46.769476 xoa-utils-1.2.1/xoa_utils/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-27 18:51:31.000000 xoa-utils-1.2.1/xoa_utils/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-27 18:51:31.000000 xoa-utils-1.2.1/xoa_utils/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:51:46.769476 xoa-utils-1.2.1/xoa_utils/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-27 18:51:31.000000 xoa-utils-1.2.1/xoa_utils/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-27 18:51:31.000000 xoa-utils-1.2.1/xoa_utils/hub/hub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:51:46.769476 xoa-utils-1.2.1/xoa_utils/ssh_server/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-27 18:51:31.000000 xoa-utils-1.2.1/xoa_utils/ssh_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-27 18:51:31.000000 xoa-utils-1.2.1/xoa_utils/ssh_server/xena_ssh_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:51:46.765476 xoa-utils-1.2.1/xoa_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-27 18:51:46.000000 xoa-utils-1.2.1/xoa_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-27 18:51:46.000000 xoa-utils-1.2.1/xoa_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 18:51:46.000000 xoa-utils-1.2.1/xoa_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-27 18:51:46.000000 xoa-utils-1.2.1/xoa_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-27 18:51:46.000000 xoa-utils-1.2.1/xoa_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 18:51:46.000000 xoa-utils-1.2.1/xoa_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:57:01.537771 xoa-utils-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-15 09:56:49.000000 xoa-utils-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-15 09:57:01.537771 xoa-utils-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-15 09:56:49.000000 xoa-utils-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-15 09:57:01.537771 xoa-utils-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:57:01.529770 xoa-utils-2.0.0/xoa_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:57:01.533770 xoa-utils-2.0.0/xoa_utils/clicks/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/clicks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/clicks/click_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:57:01.533770 xoa-utils-2.0.0/xoa_utils/clicks/click_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/clicks/click_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/clicks/click_commands/an.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16636 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/clicks/click_commands/anlt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27448 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/clicks/click_commands/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/clicks/click_commands/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/clicks/click_commands/lt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/clicks/click_commands/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/clicks/click_help.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:57:01.537771 xoa-utils-2.0.0/xoa_utils/clis/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/clis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16571 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/clis/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:57:01.537771 xoa-utils-2.0.0/xoa_utils/cmds/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12158 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/cmds/cmd_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/cmds/cmd_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:57:01.537771 xoa-utils-2.0.0/xoa_utils/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:57:01.537771 xoa-utils-2.0.0/xoa_utils/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/hub/hub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:57:01.537771 xoa-utils-2.0.0/xoa_utils/ssh_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/ssh_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/ssh_server/xena_ssh_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:57:01.533770 xoa-utils-2.0.0/xoa_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-15 09:57:01.000000 xoa-utils-2.0.0/xoa_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-15 09:57:01.000000 xoa-utils-2.0.0/xoa_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:57:01.000000 xoa-utils-2.0.0/xoa_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 09:57:01.000000 xoa-utils-2.0.0/xoa_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-15 09:57:01.000000 xoa-utils-2.0.0/xoa_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 09:57:01.000000 xoa-utils-2.0.0/xoa_utils.egg-info/top_level.txt
```

### Comparing `xoa-utils-1.2.1/LICENSE` & `xoa-utils-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xoa-utils-1.2.1/PKG-INFO` & `xoa-utils-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xoa-utils
-Version: 1.2.1
+Version: 2.0.0
 Summary: Xena OpenAutomation Utilities provides a shell-like command-line interface for users to do explorative tests interactively, such as ANLT test.
 Home-page: https://github.com/xenanetworks/open-automation-utilities
 Author: Ron Ding, Leonard Yu
 Author-email: rdi@xenanetworks.com, hyu@xenanetworks.com
 Maintainer: Xena Networks
 Maintainer-email: support@xenanetworks.com
 License: Apache 2.0
```

### Comparing `xoa-utils-1.2.1/README.md` & `xoa-utils-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `xoa-utils-1.2.1/setup.py` & `xoa-utils-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             "asyncclick>=8.1.3.4",
             "anyio>=3.6.2",
             "loguru>=0.6.0",
             "pdoc>=12.3.1",
             "pytest>=7.2.1",
             "asyncclick>=8.1.3.4",
             "psutil>=5.9.4",
-            "xoa-driver>=1.3",
+            "xoa-driver>=2.1",
         ],
         classifiers=[
             "Development Status :: 5 - Production/Stable",
             "Intended Audience :: Developers",
             "Topic :: Software Development :: Libraries :: Python Modules",
             "License :: OSI Approved :: Apache Software License",
             "Programming Language :: Python :: 3.8",
```

### Comparing `xoa-utils-1.2.1/xoa_utils/clicks/click_backend.py` & `xoa-utils-2.0.0/xoa_utils/clicks/click_backend.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-1.2.1/xoa_utils/clicks/click_commands/__init__.py` & `xoa-utils-2.0.0/xoa_utils/clicks/click_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-1.2.1/xoa_utils/clicks/click_commands/an.py` & `xoa-utils-2.0.0/xoa_utils/clicks/click_commands/an.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-1.2.1/xoa_utils/clicks/click_commands/anlt.py` & `xoa-utils-2.0.0/xoa_utils/clicks/click_commands/anlt.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,23 +127,26 @@
 # command: log
 # --------------------------
 @anlt.command(cls=cb.XenaCommand, name="log")
 @ac.option(
     "-f", "--filename", type=ac.STRING, help=h.HELP_ANLT_LOG_FILENAME, default=""
 )
 @ac.option(
+    "--read", is_flag=True, help="Read the file", default=False
+)
+@ac.option(
     "-k",
     "--keep",
     type=ac.Choice(["all", "an", "lt"]),
     help=h.HELP_ANLT_LOG_KEEP,
     default="all",
 )
 @ac.option("-s", "--serdes", type=ac.STRING, help=h.HELP_ANLT_LOG_SERDES, default="")
 @ac.pass_context
-async def anlt_log(ctx: ac.Context, filename: str, keep: str, serdes: str) -> str:
+async def anlt_log(ctx: ac.Context, filename: str, read: bool, keep: str, serdes: str) -> str:
     """
     Start AN/LT logging.
     """
 
     def _filter_log(log: str, keep: str, serdes: list[int]) -> list[dict]:
         all_logs = []
         for lg in log.split("\n"):
@@ -291,30 +294,37 @@
                 b_str = f"{common:<32}{(log_xla + ': '):<5}{log_log}"
 
             if b_str:
                 real.append(b_str)
         return "\n".join(real)
 
     async def log(
-        storage: CmdContext, filename: str, keep: str, serdes: list[int]
+        storage: CmdContext, filename: str, read: bool, keep: str, serdes: list[int]
     ) -> str:
-        port_obj = storage.retrieve_port()
-        log_str = await anlt_utils.anlt_log(port_obj)
+        if read:
+            with open(filename, "r") as f:
+                log_str = f.read()
+        else:
+            port_obj = storage.retrieve_port()
+            log_str = await anlt_utils.anlt_log(port_obj)
         filtered = _filter_log(log_str, keep, serdes)
         string = _beautify(filtered)
-        if filename and log_str:
+        if not read and filename and log_str:
             with open(filename, "a") as f:
                 f.write(f"{log_str}\n")
         return string
 
     real_serdes_list = [int(i.strip()) for i in serdes.split(",")] if serdes else []
-    kw = {"filename": filename, "keep": keep, "serdes": real_serdes_list}
-    storage: CmdContext = ctx.obj
-    storage.set_loop_coro(log, kw)
-    return ""
+    if read:
+        return await log(storage=None, filename=filename, read=read, keep=keep, serdes=real_serdes_list)
+    else:
+        kw = {"filename": filename, "read": read, "keep": keep, "serdes": real_serdes_list}
+        storage: CmdContext = ctx.obj
+        storage.set_loop_coro(log, kw)
+        return ""
 
 
 # --------------------------
 # command: strict
 # --------------------------
 @anlt.command(cls=cb.XenaCommand)
 @ac.option("--on/--off", type=ac.BOOL, help=h.HELP_STRICT_ON, default=True)
```

### Comparing `xoa-utils-1.2.1/xoa_utils/clicks/click_commands/debug.py` & `xoa-utils-2.0.0/xoa_utils/clicks/click_commands/debug.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-1.2.1/xoa_utils/clicks/click_commands/lt.py` & `xoa-utils-2.0.0/xoa_utils/clicks/click_commands/lt.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from xoa_driver.hlfuncs import anlt as anlt_utils
 from xoa_driver import enums
 from xoa_utils.clis import (
     format_lt_algorithm,
     format_lt_config,
     format_lt_im,
     format_lt_inc_dec,
+    format_lt_no_eq,
     format_lt_encoding,
     format_lt_preset,
     format_lt_trained,
     format_txtap_get,
     format_txtap_set,
     format_lt_status,
 )
@@ -157,14 +158,41 @@
     resp = await anlt_utils.lt_coeff_dec(
         port_obj, serdes, enums.LinkTrainCoeffs[emphasis.upper()]
     )
     return format_lt_inc_dec(storage, serdes, emphasis, False, resp.name)
 
 
 # **************************
+# Type: Control
+# **************************
+# **************************
+# sub-command: lt no-eq
+# **************************
+@lt.command(cls=cb.XenaCommand, name="no-eq")
+@ac.argument("serdes", type=ac.INT)
+@ac.argument("emphasis", type=ac.Choice(["pre3", "pre2", "pre", "main", "post"]))
+@ac.pass_context
+async def lt_no_eq(context: ac.Context, serdes: int, emphasis: str) -> str:
+    """
+    Request the remote port's serdes to turn off equalizing.
+
+        <SERDES>: Specifies the transceiver serdes index.
+
+        <EMPHASIS>: The emphasis (coefficient) of the link partner. Allowed values: pre3 | pre2 | pre | main | post
+    """
+    storage: CmdContext = context.obj
+    port_obj = storage.retrieve_port()
+    storage.validate_current_serdes(serdes)
+    resp = await anlt_utils.lt_coeff_no_eq(
+        port_obj, serdes, enums.LinkTrainCoeffs[emphasis.upper()]
+    )
+    return format_lt_no_eq(storage, serdes, emphasis, resp.name)
+
+
+# **************************
 # sub-command: lt encoding
 # **************************
 @lt.command(cls=cb.XenaCommand, name="encoding")
 @ac.argument("serdes", type=ac.INT)
 @ac.argument("encoding", type=ac.Choice(["nrz", "pam4", "pam4pre"]))
 @ac.pass_context
 async def lt_encoding(context: ac.Context, serdes: int, encoding: str) -> str:
```

### Comparing `xoa-utils-1.2.1/xoa_utils/clicks/click_commands/management.py` & `xoa-utils-2.0.0/xoa_utils/clicks/click_commands/management.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from xoa_utils.clicks import click_help as h
 from xoa_utils.cmds import CmdContext
 from xoa_utils import exceptions as ex
 
 # --------------------------
 # command: connect
 # --------------------------
+
+
 @xoa_util.command(cls=cb.XenaCommand)
 @ac.argument("device", type=ac.STRING)
 @ac.argument("username", type=ac.STRING)
 @ac.option("-p", "--ports", type=ac.STRING, help=h.HELP_CONNECT_PORT_LIST, default="")
 @ac.option("--reset/--no-reset", type=ac.BOOL, help=h.HELP_CONNECT_RESET, default=True)
 @ac.option("--force/--no-force", type=ac.BOOL, help=h.HELP_CONNECT_FORCE, default=True)
 @ac.option("-P", "--password", type=ac.STRING, help=h.HELP_CONNECT_PWD, default="xena")
@@ -39,15 +41,15 @@
 
         <DEVICE>: The chassis address to connect. Address can be in IPv4 format (e.g. 10.10.10.10), or a host name (e.g. demo.xenanetworks.com)
 
         <USERNAME>: Username for port reservation.
     """
     storage: CmdContext = context.obj
     real_port_list = [i.strip() for i in ports.split(",")] if ports else []
-    tester = await L23Tester(device, username, password, tcp, debug=False)
+    tester = await L23Tester(device, username, password, tcp)
     con_info = f"{device}:{tcp}"
     storage.store_current_tester(username, con_info, tester)
     count = 0
     first_id = ""
     for id_str in real_port_list:
         this_module_dic = storage.obtain_physical_modules(id_str)
         for module_id, module_obj in this_module_dic.items():
@@ -188,26 +190,33 @@
             "qsfpdd_nrz",
             "cfp",
             "base_t1",
             "base_t1s",
             "qsfpdd800",
             "qsfp112",
             "osfp800",
+            "qsfpdd800_anlt",
+            "qsfp112_anlt",
+            "osfp800_anlt"
         ]
     ),
 )
 @ac.argument("port_count", type=ac.INT)
 @ac.argument(
     "port_speed",
     type=ac.Choice(
         [
-            "800g",
-            "400g",
-            "200g",
+            "10g",
+            "25g",
+            "50g",
             "100g",
+            "200g",
+            "400g",
+            "800g",
+
         ]
     ),
 )
 @ac.option("--force/--no-force", type=ac.BOOL, help=h.HELP_CONNECT_FORCE, default=True)
 @ac.pass_context
 async def module_config(
     context: ac.Context,
@@ -218,25 +227,25 @@
     force: bool,
 ) -> str:
     """
     Change module media configuration
 
         <MODULE>: Specifies the module on the specified device host. Specify a module using the format slot, e.g. 0
 
-        <MEDIA>: Specifies the media configuration type of the module. Allowed values: qsfpddpam4 | sfpdd | sfp112 | qsfpddnrz | qsfpdd800 | qsfp112 | osfp800
+        <MEDIA>: Specifies the media configuration type of the module. Allowed values: cfp4 | cxp | sfp28 | qsfp28_nrz | qsfp28_pam4 | qsfp56_pam4 | qsfpdd_pam4 | sfp56 | sfpdd | sfp112 | qsfpdd_nrz | cfp | base_t1 | base_t1s | qsfpdd800 | qsfp112 | osfp800 | qsfpdd800_anlt | qsfp112_anlt | osfp800_anlt
 
         <PORT_COUNT>: Specifies the port count of the module.
 
-        <PORT_SPEED>: Specifies the port speed in Gbps of the module. Allowed values: 800g | 400g | 200g | 100g
+        <PORT_SPEED>: Specifies the port speed in Gbps of the module. Allowed values: 800g | 400g | 200g | 100g | 50g | 25g | 10g
 
     """
     storage: CmdContext = context.obj
     module_obj = storage.retrieve_module(str(module))
     await mgmt_utils.set_module_media_config(
         module_obj, MediaConfigurationType[media.upper()], force
     )
     await mgmt_utils.set_module_port_config(
-        module_obj, port_count, int(port_speed.replace("g", "000000000")), force
+        module_obj, port_count, int(
+            port_speed.replace("g", "000")), force
     )
-    await module_obj._setup()
     storage.remove_ports()
     return ""
```

### Comparing `xoa-utils-1.2.1/xoa_utils/clicks/click_help.py` & `xoa-utils-2.0.0/xoa_utils/clicks/click_help.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-1.2.1/xoa_utils/clis/__init__.py` & `xoa-utils-2.0.0/xoa_utils/clis/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     format_recovery,
     format_lt_algorithm,
     format_lt_config,
     format_lt_im,
     format_error,
     format_an_config,
     format_lt_inc_dec,
+    format_lt_no_eq,
     format_lt_encoding,
     format_lt_preset,
     format_lt_trained,
     format_txtap_get,
     format_txtap_set,
     format_lt_status,
     format_debug_init,
```

### Comparing `xoa-utils-1.2.1/xoa_utils/clis/cli_utils.py` & `xoa-utils-2.0.0/xoa_utils/clis/cli_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -228,14 +228,27 @@
         "main": "c(0)",
         "post": "c(1)",
     }[emphasis]
     action = "increase" if increase else "decrease"
     return f"Port {storage.retrieve_port_str()}: {action} {change} by 1 on Serdes {serdes} ({response})\n"
 
 
+def format_lt_no_eq(
+    storage: CmdContext, serdes: int, emphasis: str, response: str
+) -> str:
+    change = {
+        "pre3": "c(-3)",
+        "pre2": "c(-2)",
+        "pre": "c(-1)",
+        "main": "c(0)",
+        "post": "c(1)",
+    }[emphasis]
+    return f"Port {storage.retrieve_port_str()}: Turning off equalizer on {change} on Serdes {serdes} ({response})\n"
+
+
 def format_lt_encoding(
     storage: CmdContext, serdes: int, encoding: str, response: str
 ) -> str:
     e = enums.LinkTrainEncoding[
         {"pam4pre": "PAM4_WITH_PRECODING"}.get(encoding, encoding).upper()
     ]
     return f"Port {storage.retrieve_port_str()}: use {e.name} on Serdes {serdes} ({response})\n"
```

### Comparing `xoa-utils-1.2.1/xoa_utils/cmds/cmd_context.py` & `xoa-utils-2.0.0/xoa_utils/cmds/cmd_context.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-1.2.1/xoa_utils/cmds/cmd_worker.py` & `xoa-utils-2.0.0/xoa_utils/cmds/cmd_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,19 +150,19 @@
             success = True
             if isinstance(response, int):
                 response = self.context.get_error()
                 success = False
         except ac.UsageError as error:
             response = format_error(error)
             success = False
-        except driver_ex.BadStatus as ee:
-            response = f"{type(ee).__name__}: Driver BadStatus error.\n"
+        except driver_ex.XoaException as ee:
+            response = f"{type(ee).__name__}: Driver error.\n"
             success = False
         except Exception as e:
-            response = f"{type(e).__name__}: {e}\n"
+            response = f"{type(e).__name__}: {getattr(e, 'msg', str(e))}\n"
             success = False
         if response is not None:
             self.write(f"{response}")
             self.put_hub_record(request, response, success)
 
     async def run_coroutine(self) -> None:
         async_func, kw = self.context.get_loop_coro()
```

### Comparing `xoa-utils-1.2.1/xoa_utils/entry.py` & `xoa-utils-2.0.0/xoa_utils/entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,12 +53,14 @@
     try:
         await start_server(config)
     except (OSError, asyncssh.Error) as exc:
         sys.exit(f"Error starting server: <{type(str(exc))}> {exc}")
     except KeyboardInterrupt:
         os.remove(config.hub_pid_path)
 
+
 def main() -> None:
     asyncio.run(xoa_utility())
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `xoa-utils-1.2.1/xoa_utils/exceptions/exceptions.py` & `xoa-utils-2.0.0/xoa_utils/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-1.2.1/xoa_utils/hub/hub.py` & `xoa-utils-2.0.0/xoa_utils/hub/hub.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-1.2.1/xoa_utils/ssh_server/xena_ssh_server.py` & `xoa-utils-2.0.0/xoa_utils/ssh_server/xena_ssh_server.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-1.2.1/xoa_utils.egg-info/PKG-INFO` & `xoa-utils-2.0.0/xoa_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xoa-utils
-Version: 1.2.1
+Version: 2.0.0
 Summary: Xena OpenAutomation Utilities provides a shell-like command-line interface for users to do explorative tests interactively, such as ANLT test.
 Home-page: https://github.com/xenanetworks/open-automation-utilities
 Author: Ron Ding, Leonard Yu
 Author-email: rdi@xenanetworks.com, hyu@xenanetworks.com
 Maintainer: Xena Networks
 Maintainer-email: support@xenanetworks.com
 License: Apache 2.0
```

### Comparing `xoa-utils-1.2.1/xoa_utils.egg-info/SOURCES.txt` & `xoa-utils-2.0.0/xoa_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

