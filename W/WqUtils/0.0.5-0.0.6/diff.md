# Comparing `tmp/WqUtils-0.0.5-py3-none-any.whl.zip` & `tmp/WqUtils-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2985 bytes, number of entries: 6
--rw-r--r--  2.0 unx     4339 b- defN 23-Jun-14 09:18 WqUtils/Utils.py
+Zip file size: 2977 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     4318 b- defN 23-Jun-15 02:22 WqUtils/Utils.py
 -rw-r--r--  2.0 unx      250 b- defN 22-Nov-25 08:56 WqUtils/__init__.py
--rw-r--r--  2.0 unx      208 b- defN 23-Jun-14 09:32 WqUtils-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-14 09:32 WqUtils-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-14 09:32 WqUtils-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      444 b- defN 23-Jun-14 09:32 WqUtils-0.0.5.dist-info/RECORD
-6 files, 5341 bytes uncompressed, 2181 bytes compressed:  59.2%
+-rw-r--r--  2.0 unx      208 b- defN 23-Jun-15 02:24 WqUtils-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 02:24 WqUtils-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-15 02:24 WqUtils-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      444 b- defN 23-Jun-15 02:24 WqUtils-0.0.6.dist-info/RECORD
+6 files, 5320 bytes uncompressed, 2173 bytes compressed:  59.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: WqUtils/Utils.py
 Comment: 
 
 Filename: WqUtils/__init__.py
 Comment: 
 
-Filename: WqUtils-0.0.5.dist-info/METADATA
+Filename: WqUtils-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: WqUtils-0.0.5.dist-info/WHEEL
+Filename: WqUtils-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: WqUtils-0.0.5.dist-info/top_level.txt
+Filename: WqUtils-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: WqUtils-0.0.5.dist-info/RECORD
+Filename: WqUtils-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## WqUtils/Utils.py

```diff
@@ -24,15 +24,15 @@
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
             cls._instances[cls] = super(Singleton, cls).__call__(*args, **kwargs)
         return cls._instances[cls]
 
 
-class Log(metaclass=Singleton):
+class Log:
     def __init__(self, filename=None):
         """日志logger类"""
         # 创建logs文件夹
         self.file_name = filename
         cur_path = os.path.dirname(os.path.realpath(self.file_name))
         self.log_path = os.path.join(cur_path, 'logs')
         # 如果不存在这个logs文件夹，就自动创建一个
```

