# Comparing `tmp/guardshield-1.0.4.tar.gz` & `tmp/guardshield-1.0.5-py3.9.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\guardshield-1.0.4.tar", last modified: Fri Jun  2 22:42:52 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

