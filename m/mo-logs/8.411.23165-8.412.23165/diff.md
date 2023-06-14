# Comparing `tmp/mo_logs-8.411.23165-py2.py3-none-any.whl.zip` & `tmp/mo_logs-8.412.23165-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 43030 bytes, number of entries: 21
--rw-rw-rw-  2.0 fat    15496 b- defN 23-Jun-14 02:49 mo_logs/__init__.py
+Zip file size: 43117 bytes, number of entries: 21
+-rw-rw-rw-  2.0 fat    15892 b- defN 23-Jun-14 22:50 mo_logs/__init__.py
 -rw-rw-rw-  2.0 fat     2329 b- defN 23-Apr-30 18:00 mo_logs/constants.py
 -rw-rw-rw-  2.0 fat     2407 b- defN 23-May-30 00:22 mo_logs/convert.py
 -rw-rw-rw-  2.0 fat     8762 b- defN 23-Jun-14 02:49 mo_logs/exceptions.py
 -rw-rw-rw-  2.0 fat     3524 b- defN 23-Apr-30 18:00 mo_logs/log_usingEmail.py
 -rw-rw-rw-  2.0 fat     1099 b- defN 23-Apr-30 18:00 mo_logs/log_usingFile.py
 -rw-rw-rw-  2.0 fat     3301 b- defN 23-May-09 22:44 mo_logs/log_usingHandler.py
 -rw-rw-rw-  2.0 fat     2013 b- defN 23-Apr-30 18:00 mo_logs/log_usingLogger.py
@@ -11,13 +11,13 @@
 -rw-rw-rw-  2.0 fat     1454 b- defN 23-Apr-30 18:00 mo_logs/log_usingMulti.py
 -rw-rw-rw-  2.0 fat      450 b- defN 23-Apr-30 18:00 mo_logs/log_usingNothing.py
 -rw-rw-rw-  2.0 fat     4069 b- defN 23-Apr-30 18:00 mo_logs/log_usingSES.py
 -rw-rw-rw-  2.0 fat     1525 b- defN 23-May-30 00:22 mo_logs/log_usingStream.py
 -rw-rw-rw-  2.0 fat     2325 b- defN 23-Apr-30 18:00 mo_logs/log_usingThread.py
 -rw-rw-rw-  2.0 fat     6310 b- defN 23-May-30 00:22 mo_logs/startup.py
 -rw-rw-rw-  2.0 fat    25364 b- defN 23-Jun-14 02:49 mo_logs/strings.py
--rw-rw-rw-  2.0 fat    16725 b- defN 23-Jun-14 02:49 mo_logs-8.411.23165.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    17648 b- defN 23-Jun-14 02:49 mo_logs-8.411.23165.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-14 02:49 mo_logs-8.411.23165.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-14 02:49 mo_logs-8.411.23165.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1700 b- defN 23-Jun-14 02:49 mo_logs-8.411.23165.dist-info/RECORD
-21 files, 119208 bytes uncompressed, 40296 bytes compressed:  66.2%
+-rw-rw-rw-  2.0 fat    16725 b- defN 23-Jun-14 22:50 mo_logs-8.412.23165.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    17648 b- defN 23-Jun-14 22:50 mo_logs-8.412.23165.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-14 22:50 mo_logs-8.412.23165.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-14 22:50 mo_logs-8.412.23165.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1700 b- defN 23-Jun-14 22:50 mo_logs-8.412.23165.dist-info/RECORD
+21 files, 119604 bytes uncompressed, 40383 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: mo_logs/startup.py
 Comment: 
 
 Filename: mo_logs/strings.py
 Comment: 
 
-Filename: mo_logs-8.411.23165.dist-info/LICENSE
+Filename: mo_logs-8.412.23165.dist-info/LICENSE
 Comment: 
 
-Filename: mo_logs-8.411.23165.dist-info/METADATA
+Filename: mo_logs-8.412.23165.dist-info/METADATA
 Comment: 
 
-Filename: mo_logs-8.411.23165.dist-info/WHEEL
+Filename: mo_logs-8.412.23165.dist-info/WHEEL
 Comment: 
 
-Filename: mo_logs-8.411.23165.dist-info/top_level.txt
+Filename: mo_logs-8.412.23165.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_logs-8.411.23165.dist-info/RECORD
+Filename: mo_logs-8.412.23165.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_logs/__init__.py

```diff
@@ -142,19 +142,20 @@
         else:
             from mo_logs.log_usingThread import StructuredLogger_usingThread
 
             old_log, cls.main_log = cls.main_log, StructuredLogger_usingThread(logger)
             old_log.stop()
 
     @classmethod
-    def note(cls, template, default_params={}, *, stack_depth=0, **more_params):
+    def note(cls, template, default_params={}, *, stack_depth=0, static_template=True, **more_params):
         """
         :param template: *string* human readable string with placeholders for parameters
         :param default_params: *dict* parameters to fill in template
         :param stack_depth:  *int* how many calls you want popped off the stack to report the *true* caller
+        :param static_template: *bool* if True, then the template is static, and optimization can be done
         :param more_params: *any more parameters (which will overwrite default_params)
         :return:
         """
         timestamp = datetime.utcnow()
         if not is_text(template):
             logger.error("logger.info was expecting a string template")
 
@@ -162,20 +163,21 @@
             LogItem(
                 severity=exceptions.NOTE,
                 template=template,
                 params=dict(default_params, **more_params),
                 timestamp=timestamp,
             ),
             stack_depth + 1,
+            static_template=static_template
         )
 
     info = note
 
     @classmethod
-    def alarm(cls, template, default_params={}, *, stack_depth=0, **more_params):
+    def alarm(cls, template, default_params={}, *, stack_depth=0, static_template=True, **more_params):
         """
         :param template: *string* human readable string with placeholders for parameters
         :param default_params: *dict* parameters to fill in template
         :param stack_depth:  *int* how many calls you want popped off the stack to report the *true* caller
         :param more_params: more parameters (which will overwrite default_params)
         :return:
         """
@@ -185,28 +187,30 @@
             LogItem(
                 severity=exceptions.ALARM,
                 template=template,
                 params=dict(default_params, **more_params),
                 timestamp=timestamp,
             ),
             stack_depth + 1,
+            static_template=static_template
         )
 
     alert = alarm
 
     @classmethod
     def warning(
         cls,
         template: str,  # human readable string with placeholders for parameters
         default_params={},  # parameters to fill in template
         cause=None,  # for chaining
         *,
         stack_depth=0,  # how many calls you want popped off the stack to report the *true* caller
         log_severity=WARNING,  # set the logging severity
         exc_info=None,  # used by python logging as the cause
+        static_template=True,
         **more_params,  # any more parameters (which will overwrite default_params)
     ):
         if exc_info is True:
             exc_type, exc_value, exc_traceback = sys.exc_info()
             exc_info = Except.wrap(exc_value)
         if not is_text(template):
             logger.error("logger.warning was expecting a string template")
@@ -218,15 +222,15 @@
             default_params = {}
 
         params = to_data(dict(default_params, **more_params))
         cause = unwraplist([Except.wrap(c, stack_depth=2) for c in listwrap(cause or exc_info)])
         trace = exceptions.get_stacktrace(stack_depth + 1)
 
         e = Except(severity=log_severity, template=template, params=params, cause=cause, trace=trace,)
-        Log._annotate(e, stack_depth + 1)
+        Log._annotate(e, stack_depth + 1, static_template=static_template)
 
     warn = warning
 
     @classmethod
     def error(
         cls,
         template,  # human readable template
@@ -264,15 +268,15 @@
         cause = unwraplist([Except.wrap(c, stack_depth=2) for c in listwrap(cause or exc_info)])
         trace = exceptions.get_stacktrace(stack_depth + 1)
 
         e = Except(severity=exceptions.ERROR, template=template, params=params, cause=cause, trace=trace,)
         raise_from_none(e)
 
     @classmethod
-    def _annotate(cls, item, stack_depth):
+    def _annotate(cls, item, stack_depth, static_template=False):
         """
         :param item:  A LogItem THE TYPE OF MESSAGE
         :param stack_depth: FOR TRACKING WHAT LINE THIS CAME FROM
         :return:
         """
         given_template = item.template
         given_template = strings.limit(given_template, 10000)
@@ -300,24 +304,25 @@
             )
             f = sys._getframe(stack_depth + 1)
             item.location = {
                 "line": f.f_lineno,
                 "file": f.f_code.co_filename,
                 "method": f.f_code.co_name,
             }
-            last_caller_loc = (f.f_code.co_filename, f.f_lineno)
-            prev_template = all_log_callers.get(last_caller_loc)
-            if prev_template != given_template:
-                if prev_template:
-                    raise Except(
-                        template="Expecting logger call to be static: was {a|quote} now {b|quote}",
-                        params={"a": prev_template, "b": given_template},
-                        trace=get_stacktrace(stack_depth + 1),
-                    )
-                all_log_callers[last_caller_loc] = given_template
+            if static_template:
+                last_caller_loc = (f.f_code.co_filename, f.f_lineno)
+                prev_template = all_log_callers.get(last_caller_loc)
+                if prev_template != given_template:
+                    if prev_template:
+                        raise Except(
+                            template="Expecting logger call to be static: was {a|quote} now {b|quote}",
+                            params={"a": prev_template, "b": given_template},
+                            trace=get_stacktrace(stack_depth + 1),
+                        )
+                    all_log_callers[last_caller_loc] = given_template
             thread = _Thread.current()
             item.thread = {"name": thread.name, "id": thread.id}
         else:
             log_format = param_template
             # log_format = item.template = "{timestamp|datetime} - " + template
 
         item.params = {**cls.extra, **item.params}
```

## Comparing `mo_logs-8.411.23165.dist-info/LICENSE` & `mo_logs-8.412.23165.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_logs-8.411.23165.dist-info/METADATA` & `mo_logs-8.412.23165.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-logs
-Version: 8.411.23165
+Version: 8.412.23165
 Summary: More Logs! Structured Logging and Exception Handling
 Home-page: https://github.com/klahnakoski/mo-logs
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
```

## Comparing `mo_logs-8.411.23165.dist-info/RECORD` & `mo_logs-8.412.23165.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-mo_logs/__init__.py,sha256=KYKMsFdMyGXae7XHQX_OjOa23UNs9aLpAcAegWkLBQ4,15496
+mo_logs/__init__.py,sha256=WBV1vTuSDDPDro6kSd98Wefype4VaPfIqV5eiq_90DU,15892
 mo_logs/constants.py,sha256=uYmXrreY2PJ4nXwFhRCySuqvBJmwRsrjFoTpy6dSf1I,2329
 mo_logs/convert.py,sha256=LjY9G-sgb64KctRkMQA2bYLMZj8iK226bwgS52wvMyA,2407
 mo_logs/exceptions.py,sha256=T0zXkl5v-M0IOL5LmMOxGNGI_He565uGU4Fm9wq_2rs,8762
 mo_logs/log_usingEmail.py,sha256=R2wxQX0KolEQt_qtkwhISICAAlSQSU1Xus9iWaoDaW8,3524
 mo_logs/log_usingFile.py,sha256=wDRvM45WarKZqAfTZKqPkO6fleGwZaM0M_qFPRVmC-k,1099
 mo_logs/log_usingHandler.py,sha256=h67fvo7PJCKx85TrE-QOMCZe2lLyCvBHBcr6BUo-2Gs,3301
 mo_logs/log_usingLogger.py,sha256=4OOsUZPemh27cUOYdLetHuI9KmF47Ut0IRmdRU0p7EM,2013
@@ -10,12 +10,12 @@
 mo_logs/log_usingMulti.py,sha256=2uUM3zHgpviKL5xJUIhi-5ReFEC51Zqv9-imi0xjBi0,1454
 mo_logs/log_usingNothing.py,sha256=RAJGGPwg4bw-eX4kDFT0kdEHH4hFsLicnJeq9Pf4Y3Q,450
 mo_logs/log_usingSES.py,sha256=hzfmQSiMnBudy4ptn73nGLUOXB-uhBXbOdUpv42HYjs,4069
 mo_logs/log_usingStream.py,sha256=t9q7Ju7F9wMKjReWXkUIcpkKRkiat2FHa---s8gdJ4s,1525
 mo_logs/log_usingThread.py,sha256=LbWlEBNGbjPBEFFIegmXhuT1_AA7H18Lv8YGDRVUpMc,2325
 mo_logs/startup.py,sha256=sMOxbRnsb-GPoMidGoTYAS9ooasv4BfwJRvyklY7fKM,6310
 mo_logs/strings.py,sha256=d63f-90qN-YlyqSDU8YqSS3HzcN18OT8zY-UMk6HF5I,25364
-mo_logs-8.411.23165.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
-mo_logs-8.411.23165.dist-info/METADATA,sha256=JkCYPImeOd4EVyhQh9xLp0RnEnpdlM7z2dQB-KAR9vY,17648
-mo_logs-8.411.23165.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-mo_logs-8.411.23165.dist-info/top_level.txt,sha256=yqpeBBL3Yw2CDh1_FthlIK34KbT5cyZcAEjxlQ3MpDA,8
-mo_logs-8.411.23165.dist-info/RECORD,,
+mo_logs-8.412.23165.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
+mo_logs-8.412.23165.dist-info/METADATA,sha256=T37CdE3LWxVhLNOZPrbLBgM3Rb4UuGF_DT0UkjZsqFQ,17648
+mo_logs-8.412.23165.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+mo_logs-8.412.23165.dist-info/top_level.txt,sha256=yqpeBBL3Yw2CDh1_FthlIK34KbT5cyZcAEjxlQ3MpDA,8
+mo_logs-8.412.23165.dist-info/RECORD,,
```

