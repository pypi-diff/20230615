# Comparing `tmp/Echoo-0.0.2.post2306141219-py3-none-any.whl.zip` & `tmp/Echoo-0.0.2.post2306152330-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4462 bytes, number of entries: 9
+Zip file size: 4559 bytes, number of entries: 9
 -rw-r--r--  2.0 unx       24 b- defN 23-Jun-14 04:12 Echoo/__init__.py
--rw-r--r--  2.0 unx     3360 b- defN 23-Jun-14 04:19 Echoo/echoo.py
--rwxr-xr-x  2.0 unx       77 b- defN 23-Jun-14 04:19 Echoo-0.0.2_2306141219.data/scripts/echoo
--rw-r--r--  2.0 unx     1067 b- defN 23-Jun-14 04:19 Echoo-0.0.2.post2306141219.dist-info/LICENSE
--rw-r--r--  2.0 unx     1385 b- defN 23-Jun-14 04:19 Echoo-0.0.2.post2306141219.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-14 04:19 Echoo-0.0.2.post2306141219.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-14 04:19 Echoo-0.0.2.post2306141219.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-14 04:19 Echoo-0.0.2.post2306141219.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      788 b- defN 23-Jun-14 04:19 Echoo-0.0.2.post2306141219.dist-info/RECORD
-9 files, 6800 bytes uncompressed, 3074 bytes compressed:  54.8%
+-rw-r--r--  2.0 unx     3732 b- defN 23-Jun-15 15:26 Echoo/echoo.py
+-rwxr-xr-x  2.0 unx       77 b- defN 23-Jun-15 15:30 Echoo-0.0.2_2306152330.data/scripts/echoo
+-rw-r--r--  2.0 unx     1067 b- defN 23-Jun-15 15:30 Echoo-0.0.2.post2306152330.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1385 b- defN 23-Jun-15 15:30 Echoo-0.0.2.post2306152330.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 15:30 Echoo-0.0.2.post2306152330.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-15 15:30 Echoo-0.0.2.post2306152330.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-14 04:19 Echoo-0.0.2.post2306152330.dist-info/zip-safe
+?rw-rw-r--  2.0 unx      788 b- defN 23-Jun-15 15:30 Echoo-0.0.2.post2306152330.dist-info/RECORD
+9 files, 7172 bytes uncompressed, 3171 bytes compressed:  55.8%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: Echoo/__init__.py
 Comment: 
 
 Filename: Echoo/echoo.py
 Comment: 
 
-Filename: Echoo-0.0.2_2306141219.data/scripts/echoo
+Filename: Echoo-0.0.2_2306152330.data/scripts/echoo
 Comment: 
 
-Filename: Echoo-0.0.2.post2306141219.dist-info/LICENSE
+Filename: Echoo-0.0.2.post2306152330.dist-info/LICENSE
 Comment: 
 
-Filename: Echoo-0.0.2.post2306141219.dist-info/METADATA
+Filename: Echoo-0.0.2.post2306152330.dist-info/METADATA
 Comment: 
 
-Filename: Echoo-0.0.2.post2306141219.dist-info/WHEEL
+Filename: Echoo-0.0.2.post2306152330.dist-info/WHEEL
 Comment: 
 
-Filename: Echoo-0.0.2.post2306141219.dist-info/top_level.txt
+Filename: Echoo-0.0.2.post2306152330.dist-info/top_level.txt
 Comment: 
 
-Filename: Echoo-0.0.2.post2306141219.dist-info/zip-safe
+Filename: Echoo-0.0.2.post2306152330.dist-info/zip-safe
 Comment: 
 
-Filename: Echoo-0.0.2.post2306141219.dist-info/RECORD
+Filename: Echoo-0.0.2.post2306152330.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Echoo/echoo.py

```diff
@@ -53,27 +53,31 @@
         def wrapper( *args, **kwds):
             self.send_msg(escape_fn(f'''Start {str(function)}'''))
             res = function(*args, **kwds)
             self.send_msg(escape_fn(f'''Finish {str(function)}'''))
             return res
         return wrapper
 
-def main(token, chat_id, msg="Are u ok", parse_mode="MarkdownV2"):
+def main(token, chat_id, msg="Are u ok", parse_mode="MarkdownV2", reply_to_message_id=None):
     bot = telegram.Bot(token=token)
-    asyncio.run(
-        bot.send_message(chat_id=chat_id, text=escape_fn(msg), parse_mode=parse_mode)
+    msg_info = asyncio.run(
+        bot.send_message(chat_id=chat_id, text=escape_fn(msg), 
+                         parse_mode=parse_mode, reply_to_message_id=reply_to_message_id)
     )
+    return msg_info.id
 
 def run():
     parser = argparse.ArgumentParser(description=r'''Echoo: A tool let's your program echo to Telegram.''')
 
     parser.add_argument("-t", "--token", default=None, type=str, help="Token for your bot.")
     parser.add_argument("-id", "--chat_id", default=None, type=str, help="Chat_id of your audience.")
     parser.add_argument("--parse-mode", default="Markdown", type=str, help='''Send Markdown or HTML, if you want Telegram apps to show bold,
                 italic, fixed-width text or inline URLs in your bot's message''')
+    parser.add_argument("-rid", "--reply-to-id", default=None, type=int, help='''''')
+    parser.add_argument("--return-id", action="store_true")
     parser.add_argument("msg", default="Are u ok?", type=str, help="Message to send")
 
     args = parser.parse_args()
     if args.token is None:
         try:
             args.token = os.environ["TG_TOKEN"]
         except KeyError:
@@ -81,12 +85,15 @@
 
     if args.chat_id is None:
         try:
             args.chat_id = os.environ["TG_CHAT_ID"]
         except KeyError:
             raise KeyError("Neither --chat_id nor TG_CHAT_ID is set.")
 
-    main(token=args.token, chat_id=args.chat_id, msg=args.msg, parse_mode=args.parse_mode)
+    id = main(token=args.token, chat_id=args.chat_id, msg=args.msg, 
+              parse_mode=args.parse_mode, reply_to_message_id=args.reply_to_id)
+    if args.return_id:
+        print(id)
 
 
 if __name__ == '__main__':
     run()
```

## Comparing `Echoo-0.0.2.post2306141219.dist-info/LICENSE` & `Echoo-0.0.2.post2306152330.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Echoo-0.0.2.post2306141219.dist-info/METADATA` & `Echoo-0.0.2.post2306152330.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Echoo
-Version: 0.0.2-2306141219
+Version: 0.0.2-2306152330
 Summary: Let your program echo to you~
 Home-page: https://github.com/Lyken17/Echoo/
 Author: Ligeng Zhu
 Author-email: lykensyu+github@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `Echoo-0.0.2.post2306141219.dist-info/RECORD` & `Echoo-0.0.2.post2306152330.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Echoo/__init__.py,sha256=brP4byVZwlMnNfX5fJv_BVbUd0aJRVrISti4-NA2nBQ,24
-Echoo/echoo.py,sha256=t-G8wc3X4khRhKRxmU6PH3s9ezKutTU30GespeGvHho,3360
-Echoo-0.0.2_2306141219.data/scripts/echoo,sha256=JGNpFj2uGAye3Z0IvoE_UkJ4xzuDvpO3SG9CIhWcPMw,77
-Echoo-0.0.2.post2306141219.dist-info/LICENSE,sha256=NvV3rSiPG-roGItuwJgI6u0njAi4KEusxpS7Vv-_Pfw,1067
-Echoo-0.0.2.post2306141219.dist-info/METADATA,sha256=eSRtusuBHTt-mBu3wwlHP93I_gFMDPp_sQIabtR7vUg,1385
-Echoo-0.0.2.post2306141219.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-Echoo-0.0.2.post2306141219.dist-info/top_level.txt,sha256=0Nw7QC7eZkxPz2KKJSlO1D5uXG6VjoSpzmxoKP2ZByE,6
-Echoo-0.0.2.post2306141219.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-Echoo-0.0.2.post2306141219.dist-info/RECORD,,
+Echoo/echoo.py,sha256=J4dQI_HwgNijxWU1V65TOSN-FF1wQwmb2LigKorzRlA,3732
+Echoo-0.0.2_2306152330.data/scripts/echoo,sha256=JGNpFj2uGAye3Z0IvoE_UkJ4xzuDvpO3SG9CIhWcPMw,77
+Echoo-0.0.2.post2306152330.dist-info/LICENSE,sha256=NvV3rSiPG-roGItuwJgI6u0njAi4KEusxpS7Vv-_Pfw,1067
+Echoo-0.0.2.post2306152330.dist-info/METADATA,sha256=QBJJJLzl9woa3-6t5N4iA36BTXhcApd9ijiwTxJ_HWY,1385
+Echoo-0.0.2.post2306152330.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+Echoo-0.0.2.post2306152330.dist-info/top_level.txt,sha256=0Nw7QC7eZkxPz2KKJSlO1D5uXG6VjoSpzmxoKP2ZByE,6
+Echoo-0.0.2.post2306152330.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+Echoo-0.0.2.post2306152330.dist-info/RECORD,,
```

