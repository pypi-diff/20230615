# Comparing `tmp/Deepurify-1.1.0.3.tar.gz` & `tmp/Deepurify-1.1.0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Deepurify-1.1.0.3.tar", last modified: Thu Apr 13 03:35:10 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

