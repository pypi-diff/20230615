# Comparing `tmp/dushyanth-1.0.0.tar.gz` & `tmp/dushyanth-1.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dushyanth-1.0.0.tar", last modified: Thu Jun 15 05:47:06 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

