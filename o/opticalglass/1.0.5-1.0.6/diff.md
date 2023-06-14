# Comparing `tmp/opticalglass-1.0.5.tar.gz` & `tmp/opticalglass-1.0.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opticalglass-1.0.5.tar", last modified: Mon May 15 18:06:56 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

