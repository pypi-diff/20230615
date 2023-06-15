# Comparing `tmp/dagshub-0.2.9.tar.gz` & `tmp/dagshub-0.2.9.post1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagshub-0.2.9.tar", last modified: Wed Jan  4 09:04:53 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

