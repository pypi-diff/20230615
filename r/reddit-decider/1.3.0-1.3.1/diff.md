# Comparing `tmp/reddit_decider-1.3.0.tar.gz` & `tmp/reddit_decider-1.3.1-cp37-abi3-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

