# Comparing `tmp/skulk-2.1.2-py2.py3-none-any.whl.zip` & `tmp/skulk-2.1.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 10450 bytes, number of entries: 11
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-13 18:26 skulk/VERSION
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 18:25 skulk/__init__.py
--rw-r--r--  2.0 unx    11487 b- defN 23-Jun-13 18:25 skulk/bumper.py
--rw-r--r--  2.0 unx     2325 b- defN 23-Jun-13 18:25 skulk/questions.py
--rw-r--r--  2.0 unx    10044 b- defN 23-Jun-13 18:25 skulk/skulk.py
--rw-r--r--  2.0 unx     3586 b- defN 23-Jun-13 18:25 skulk/util.py
--rw-r--r--  2.0 unx      675 b- defN 23-Jun-13 18:26 skulk-2.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-13 18:26 skulk-2.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       43 b- defN 23-Jun-13 18:26 skulk-2.1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-13 18:26 skulk-2.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      810 b- defN 23-Jun-13 18:26 skulk-2.1.2.dist-info/RECORD
-11 files, 29091 bytes uncompressed, 9096 bytes compressed:  68.7%
+Zip file size: 11639 bytes, number of entries: 12
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-15 06:13 skulk/VERSION
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-15 06:13 skulk/__init__.py
+-rw-r--r--  2.0 unx    11487 b- defN 23-Jun-15 06:13 skulk/bumper.py
+-rw-r--r--  2.0 unx     2294 b- defN 23-Jun-15 06:13 skulk/questions.py
+-rw-r--r--  2.0 unx     2601 b- defN 23-Jun-15 06:13 skulk/questions_fallback.py
+-rw-r--r--  2.0 unx    10237 b- defN 23-Jun-15 06:13 skulk/skulk.py
+-rw-r--r--  2.0 unx     3586 b- defN 23-Jun-15 06:13 skulk/util.py
+-rw-r--r--  2.0 unx      675 b- defN 23-Jun-15 06:13 skulk-2.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-15 06:13 skulk-2.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-15 06:13 skulk-2.1.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-15 06:13 skulk-2.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      894 b- defN 23-Jun-15 06:13 skulk-2.1.5.dist-info/RECORD
+12 files, 31938 bytes uncompressed, 10155 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -6,29 +6,32 @@
 
 Filename: skulk/bumper.py
 Comment: 
 
 Filename: skulk/questions.py
 Comment: 
 
+Filename: skulk/questions_fallback.py
+Comment: 
+
 Filename: skulk/skulk.py
 Comment: 
 
 Filename: skulk/util.py
 Comment: 
 
-Filename: skulk-2.1.2.dist-info/METADATA
+Filename: skulk-2.1.5.dist-info/METADATA
 Comment: 
 
-Filename: skulk-2.1.2.dist-info/WHEEL
+Filename: skulk-2.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: skulk-2.1.2.dist-info/entry_points.txt
+Filename: skulk-2.1.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: skulk-2.1.2.dist-info/top_level.txt
+Filename: skulk-2.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: skulk-2.1.2.dist-info/RECORD
+Filename: skulk-2.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## skulk/VERSION

```diff
@@ -1 +1 @@
-2.1.2
+2.1.5
```

## skulk/questions.py

```diff
@@ -39,21 +39,21 @@
 def wait(prompt):
     
     choose(
          util.yellow(f"{prompt}\nChoose 'Continue' when you are ready"), 
            [{"label": "Continue", "value":"continue"}],
            echo=False)
     
-def input_string(prompt, validator=None, default=None, echo=True):
+def input_string(prompt, validator=None, echo=True):
     
     prompt = util.yellow(f"{prompt} Type 'exit' to quit: ")
     valid = False
     while not valid:
         cli = Input(
-            prompt, default=default,
+            prompt,
             word_color = colors.bright(colors.foreground["green"])
         )
         
         answer = cli.launch()
         if not answer:
             print("\n")
             continue
```

## skulk/skulk.py

```diff
@@ -36,17 +36,24 @@
 from skulk import util
 from skulk.bumper import (
     Bumper,
     RELEASE_SCOPE_BETA,
     RELEASE_SCOPE_CANDIDATE,
     RELEASE_SCOPE_RELEASE,
 )
-from skulk import questions as q
+
 from tabulate import tabulate
 
+# Termios is not available on Windows, so we use our own homegrown, less elegant, solution.
+try:
+    from skulk import questions as q
+except (ImportError, ModuleNotFoundError):
+    from skulk import questions_fallback as q
+
+
 
 class Skulk(object):
     """A wizard to guide the user to a good version and changelog."""
 
     def __init__(self):
         self.repo = util.get_repo()
         self.branch = self.repo.active_branch
```

## Comparing `skulk-2.1.2.dist-info/METADATA` & `skulk-2.1.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skulk
-Version: 2.1.2
+Version: 2.1.5
 Summary: Streamline release for Conductor client tools and others
 Home-page: https://github.com/ConductorTechnologies/skulk
 Author: Julian Mann
 Author-email: julian@conductortech.com
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python
```

## Comparing `skulk-2.1.2.dist-info/RECORD` & `skulk-2.1.5.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-skulk/VERSION,sha256=P_yDzF7mglQfHrNrG3774VSyqYLfjq7rdsUEPwejXH0,5
+skulk/VERSION,sha256=6DJJIC6-I4JujB_SFuezjGoHSxyp8MU4C1njGUIJS7g,5
 skulk/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 skulk/bumper.py,sha256=lIg6y4Nrzf7-in1kqnZP9XosjqK0BhprgImejvGdsks,11487
-skulk/questions.py,sha256=08ujtmpZss7VmNwlFMYVJZx_sJG_GsCjloURUrFG1ok,2325
-skulk/skulk.py,sha256=4Ytv48qPDy_uAucHz1mTZv9ew2RsHN3IY98hDVbESdo,10044
+skulk/questions.py,sha256=ihDx7B1JNw4wQnwjox6BRHpDUM_VzTajmf867IugP-U,2294
+skulk/questions_fallback.py,sha256=aQrtgxnHr6VUlJHO4OcVvPbzJj5V8U2OwXyJ4hBwHi8,2601
+skulk/skulk.py,sha256=OfT4HjKv_1PhjNW2RRs--P6D2GUULrcFXptpQdgjDoY,10237
 skulk/util.py,sha256=uBlyNpq_8RsuD2oOKxk4cL7-2zqXotcBPjI-QHacsHo,3586
-skulk-2.1.2.dist-info/METADATA,sha256=kvmx7RfBszzFU2Iv4Yziv9EqHEKGm_qBsHPvL3EHAH0,675
-skulk-2.1.2.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-skulk-2.1.2.dist-info/entry_points.txt,sha256=8DGRFZ3C46ZQBYFsfNj4eYw5ZGq8NWW8uKe-2xC-c34,43
-skulk-2.1.2.dist-info/top_level.txt,sha256=EOnQuA1Vdf2WjOz9xLTPLCynTq2IdzLPGQ54LdhP7oY,6
-skulk-2.1.2.dist-info/RECORD,,
+skulk-2.1.5.dist-info/METADATA,sha256=xoh4l6zr1pJMgeG1pOIn3wWli6w39hZuEJVQC12dz0U,675
+skulk-2.1.5.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+skulk-2.1.5.dist-info/entry_points.txt,sha256=8DGRFZ3C46ZQBYFsfNj4eYw5ZGq8NWW8uKe-2xC-c34,43
+skulk-2.1.5.dist-info/top_level.txt,sha256=EOnQuA1Vdf2WjOz9xLTPLCynTq2IdzLPGQ54LdhP7oY,6
+skulk-2.1.5.dist-info/RECORD,,
```

