# Comparing `tmp/mozilla_nimbus_schemas-0.1.0.tar.gz` & `tmp/mozilla_nimbus_schemas-2023.6.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla_nimbus_schemas-0.1.0.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

