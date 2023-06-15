# Comparing `tmp/thundra-3.0.7rc20230615142459.tar.gz` & `tmp/thundra-3.0.7rc20230615142505-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thundra-3.0.7rc20230615142459.tar", last modified: Thu Jun 15 14:24:59 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

