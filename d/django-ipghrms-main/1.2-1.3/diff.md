# Comparing `tmp/django-ipghrms-main-1.2.tar.gz` & `tmp/django_ipghrms_main-1.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ipghrms-main-1.2.tar", last modified: Tue Jun 13 13:19:22 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

