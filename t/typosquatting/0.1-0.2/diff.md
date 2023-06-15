# Comparing `tmp/typosquatting-0.1.tar.gz` & `tmp/typosquatting-0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typosquatting-0.1.tar", last modified: Thu Jun 15 07:55:11 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

