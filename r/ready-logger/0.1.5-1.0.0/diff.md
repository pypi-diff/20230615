# Comparing `tmp/ready_logger-0.1.5.tar.gz` & `tmp/ready_logger-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ready_logger-0.1.5.tar", max compression
+gzip compressed data, was "ready_logger-1.0.0.tar", max compression
```

## Comparing `ready_logger-0.1.5.tar` & `ready_logger-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      558 2022-10-01 19:40:30.714801 ready_logger-0.1.5/README.md
--rw-r--r--   0        0        0      678 2022-10-01 19:38:32.574800 ready_logger-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       69 2022-09-02 15:03:53.868430 ready_logger-0.1.5/ready_logger/__init__.py
--rw-r--r--   0        0        0     3477 2022-10-01 19:40:36.234801 ready_logger-0.1.5/ready_logger/configure.py
--rw-r--r--   0        0        0     1242 2022-10-01 19:45:39.228471 ready_logger-0.1.5/setup.py
--rw-r--r--   0        0        0     1425 2022-10-01 19:45:39.228682 ready_logger-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1515 2023-06-15 14:32:08.744657 ready_logger-1.0.0/README.md
+-rw-r--r--   0        0        0      800 2023-06-15 15:03:58.267074 ready_logger-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-06-15 12:53:18.989774 ready_logger-1.0.0/ready_logger/__init__.py
+-rw-r--r--   0        0        0     3974 2023-06-15 14:31:48.664787 ready_logger-1.0.0/ready_logger/ready_logger.py
+-rw-r--r--   0        0        0     2130 1970-01-01 00:00:00.000000 ready_logger-1.0.0/setup.py
+-rw-r--r--   0        0        0     2560 1970-01-01 00:00:00.000000 ready_logger-1.0.0/PKG-INFO
```

### Comparing `ready_logger-0.1.5/ready_logger/configure.py` & `ready_logger-1.0.0/ready_logger/ready_logger.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,89 +1,103 @@
 import logging
 import os
 from logging import Logger
 from logging.handlers import RotatingFileHandler
 from pathlib import Path
 from typing import Optional, Union
 
-from psutil import Process
+
+def any_case_env_var(var: str, default: Optional[str] = None) -> Union[str, None]:
+    return os.getenv(var) or os.getenv(var.lower()) or os.getenv(var.upper()) or default
 
 
 def get_logger(
     name: Optional[str] = None,
-    log_level: Optional[Union[str, int]] = None,
+    level: Optional[Union[str, int]] = None,
     show_file_path: Optional[bool] = None,
-    log_dir: Optional[Union[str, Path]] = None,
-    max_bytes: int = 20_000_000,
-    backup_count: int = 2,
+    file_dir: Optional[Union[str, Path]] = None,
+    max_bytes: Optional[int] = 20_000_000,
+    backup_count: Optional[int] = 2,
 ) -> Logger:
-    """Create a logger.
+    """Create a new logger or return an existing logger with the given name.
+
+    All arguments besides for `name` can be set via environment variables in the form `{LOGGER NAME}_{VARIABLE NAME}` or `READY_LOGGER_{VARIABLE NAME}`.
+    Variables including logger name will be chosen before `READY_LOGGER_` variables. Variables can be uppercase or lowercase.
 
     Args:
-        name (Optional[str], optional): Name for the logger (this is included in log string prefix). Defaults to None.
-        log_level (Optional[Union[str, int]], optional): Logging level -- CRITICAL: 50, ERROR: 40, WARNING: 30, INFO: 20, DEBUG: 10. Defaults to f"{name.upper()}_LOG_LEVEL" environment variable or INFO.
-        show_file_path (Optional[bool], optional): Show complete file path in log string prefix, rather than just filename. Defaults to level == DEBUG.
-        log_dir (Optional[Union[str, Path]], optional): Directory to write log files to.
+        name (Optional[str], optional): Name for the logger. Defaults to None.
+        level (Optional[Union[str, int]], optional): Logging level -- CRITICAL: 50, ERROR: 40, WARNING: 30, INFO: 20, DEBUG: 10.
+        show_file_path (Optional[bool], optional): Show absolute file path in log string prefix rather than just filename. Defaults to True if level is DEBUG, else False.
+        file_dir (Optional[Union[str, Path]], optional): Directory where log files should be written.
         max_bytes (int): Max number of bytes to store in one log file.
         backup_count (int): Number of log rotations to keep.
-        
+
     Returns:
         Logger: The configured logger.
     """
-    # create a new logger or return a reference to an already configured logger.
     logger = logging.getLogger(name)
     # if this is not the first call, the logger will already have handlers.
     if logger.handlers:
+        # return the already configured logger.
         return logger
 
-    # determine variable values.
-    if log_level is None:
+    if level is None:
         if name:
-            log_level = os.getenv(f"{name.upper()}_LOG_LEVEL")
-        log_level = log_level or os.getenv("READY_LOGGER_LOG_LEVEL", logging.INFO)
+            level = any_case_env_var(f"{name}_LOG_LEVEL")
+        level = level or any_case_env_var("READY_LOGGER_LOG_LEVEL", logging.INFO)
+
     if show_file_path is None:
         if name:
-            show_file_path = os.getenv(f"{name}_SHOW_FILE_PATH")
-        show_file_path = show_file_path or os.getenv("READY_LOGGER_SHOW_FILE_PATH")
-    if log_dir is None:
+            show_file_path = any_case_env_var(f"{name}_SHOW_FILE_PATH")
+        show_file_path = show_file_path or any_case_env_var(
+            "READY_LOGGER_SHOW_FILE_PATH"
+        )
+
+    if file_dir is None:
         if name:
-            log_dir = os.getenv(f"{name}_log_dir")
-        log_dir = log_dir or os.getenv("READY_LOGGER_log_dir")
+            file_dir = any_case_env_var(f"{name}_FILE_DIR")
+        file_dir = file_dir or any_case_env_var("READY_LOGGER_FILE_DIR")
+
     if max_bytes is None:
         if name:
-            max_bytes = os.getenv(f"{name}_MAX_BYTES")
-        max_bytes = max_bytes or os.getenv("READY_LOGGER_MAX_BYTES")
+            max_bytes = any_case_env_var(f"{name}_MAX_BYTES")
+        max_bytes = max_bytes or any_case_env_var("READY_LOGGER_MAX_BYTES")
+    if max_bytes:
+        max_bytes = int(max_bytes)
+
     if backup_count is None:
         if name:
-            backup_count = os.getenv(f"{name}_BACKUP_COUNT")
-        backup_count = backup_count or os.getenv("READY_LOGGER_BACKUP_COUNT")
+            backup_count = any_case_env_var(f"{name}_BACKUP_COUNT")
+        backup_count = backup_count or any_case_env_var("READY_LOGGER_BACKUP_COUNT")
+    if backup_count:
+        backup_count = int(backup_count)
 
     # set log level.
-    if isinstance(log_level, str):
-        log_level = logging.getLevelName(log_level.upper())
-    logger.setLevel(log_level)
+    logger.setLevel(
+        logging.getLevelName(level.upper()) if isinstance(level, str) else level
+    )
 
     # set formatting and handling.
     file_name_fmt = "pathname" if show_file_path else "filename"
+    name_fmt = "[%(name)s]" if name else ""
     formatter = logging.Formatter(
-        f"[%(asctime)s][%(levelname)s]{'[%(name)s]' if name else ''}[%({file_name_fmt})s:%(lineno)d] %(message)s"
+        f"[%(asctime)s][%(levelname)s]{name_fmt}[%({file_name_fmt})s:%(lineno)d] %(message)s"
     )
-    sh = logging.StreamHandler()
-    sh.setFormatter(formatter)
-    logger.addHandler(sh)
-
-    if log_dir:
-        stem = name or f"{(p := Process(os.getpid())).name()}_{p.pid}"
-        file = Path(log_dir) / f"{stem}.log"
+    handler = logging.StreamHandler()
+    handler.setFormatter(formatter)
+    logger.addHandler(handler)
+
+    if file_dir:
+        file = Path(file_dir) / f"{name or f'python_{os.getpid()}'}.log"
         # create log directory if it doesn't currently exist.
         file.parent.mkdir(exist_ok=True, parents=True)
         # add file handler.
-        file_handler = RotatingFileHandler(
+        handler = RotatingFileHandler(
             file, maxBytes=max_bytes, backupCount=backup_count
         )
-        file_handler.setFormatter(formatter)
-        logger.addHandler(file_handler)
+        handler.setFormatter(formatter)
+        logger.addHandler(handler)
 
     # don't duplicate log messages.
     logger.propagate = False
 
     return logger
```

