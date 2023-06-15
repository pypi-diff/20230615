# Comparing `tmp/mkdpdf-0.2.4.tar.gz` & `tmp/mkdpdf-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdpdf-0.2.4.tar", last modified: Mon Jun 12 22:10:29 2023, max compression
+gzip compressed data, was "mkdpdf-0.2.5.tar", last modified: Thu Jun 15 00:30:33 2023, max compression
```

## Comparing `mkdpdf-0.2.4.tar` & `mkdpdf-0.2.5.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.709650 mkdpdf-0.2.4/
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      303 2023-06-12 22:10:29.708649 mkdpdf-0.2.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.701650 mkdpdf-0.2.4/mkdpdf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      671 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.703650 mkdpdf-0.2.4/mkdpdf/document/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/document/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11411 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/document/document.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.699650 mkdpdf-0.2.4/mkdpdf/document/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.699650 mkdpdf-0.2.4/mkdpdf/document/templates/pdf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.704650 mkdpdf-0.2.4/mkdpdf/document/templates/pdf/style/
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/document/templates/pdf/style/document.css
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/document/templates/pdf/style/footer.css
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/document/templates/pdf/style/header.css
--rw-rw-rw-   0 root         (0) root         (0)     6683 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/document/templates/pdf/style/mermaid.css
--rw-rw-rw-   0 root         (0) root         (0)     2193 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/document/templates/pdf/style/pdf.css
--rw-rw-rw-   0 root         (0) root         (0)     3199 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/document/templates/pdf/style/reset.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.704650 mkdpdf-0.2.4/mkdpdf/documentation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/documentation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8053 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/documentation/documentation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.699650 mkdpdf-0.2.4/mkdpdf/documentation/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.704650 mkdpdf-0.2.4/mkdpdf/documentation/templates/md/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.705650 mkdpdf-0.2.4/mkdpdf/documentation/templates/md/class/
--rw-rw-rw-   0 root         (0) root         (0)      564 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/documentation/templates/md/class/header.md
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/documentation/templates/md/class/main.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.705650 mkdpdf-0.2.4/mkdpdf/documentation/templates/md/functions/
--rw-rw-rw-   0 root         (0) root         (0)      517 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/documentation/templates/md/functions/header.md
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/documentation/templates/md/functions/main.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/documentation/templates/md/header.md
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/documentation/templates/md/main.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.699650 mkdpdf-0.2.4/mkdpdf/documentation/templates/pdf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.706650 mkdpdf-0.2.4/mkdpdf/documentation/templates/pdf/style/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/documentation/templates/pdf/style/document.css
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/documentation/templates/pdf/style/footer.css
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/documentation/templates/pdf/style/header.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.706650 mkdpdf-0.2.4/mkdpdf/md/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/md/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1246 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/md/md.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.706650 mkdpdf-0.2.4/mkdpdf/pdf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/pdf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4763 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/pdf/pdf.py
--rw-rw-rw-   0 root         (0) root         (0)     3234 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/pdf/publisher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.707650 mkdpdf-0.2.4/mkdpdf/report/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/report/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/report/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.700650 mkdpdf-0.2.4/mkdpdf/report/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.707650 mkdpdf-0.2.4/mkdpdf/report/templates/md/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/report/templates/md/footer.md
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/report/templates/md/header.md
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/report/templates/md/main.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.708649 mkdpdf-0.2.4/mkdpdf/report/templates/pdf/
--rw-rw-rw-   0 root         (0) root         (0)      333 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/report/templates/pdf/footer.html
--rw-rw-rw-   0 root         (0) root         (0)      809 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/report/templates/pdf/header.html
--rw-rw-rw-   0 root         (0) root         (0)     1338 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/report/templates/pdf/main.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.708649 mkdpdf-0.2.4/mkdpdf/report/templates/pdf/style/
--rw-rw-rw-   0 root         (0) root         (0)      398 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/report/templates/pdf/style/document.css
--rw-rw-rw-   0 root         (0) root         (0)      755 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/report/templates/pdf/style/footer.css
--rw-rw-rw-   0 root         (0) root         (0)     1518 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/report/templates/pdf/style/header.css
--rw-rw-rw-   0 root         (0) root         (0)     1027 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/mkdpdf/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 22:10:29.702650 mkdpdf-0.2.4/mkdpdf.egg-info/
--rw-r--r--   0 root         (0) root         (0)      303 2023-06-12 22:10:29.000000 mkdpdf-0.2.4/mkdpdf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1695 2023-06-12 22:10:29.000000 mkdpdf-0.2.4/mkdpdf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 22:10:29.000000 mkdpdf-0.2.4/mkdpdf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-06-12 22:10:29.000000 mkdpdf-0.2.4/mkdpdf.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-06-12 22:10:29.000000 mkdpdf-0.2.4/mkdpdf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-12 22:10:29.000000 mkdpdf-0.2.4/mkdpdf.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 22:10:29.709650 mkdpdf-0.2.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      976 2023-06-12 22:10:22.000000 mkdpdf-0.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.477287 mkdpdf-0.2.5/
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      303 2023-06-15 00:30:33.476287 mkdpdf-0.2.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.468288 mkdpdf-0.2.5/mkdpdf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      671 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.470287 mkdpdf-0.2.5/mkdpdf/document/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/document/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12516 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/document/document.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.464288 mkdpdf-0.2.5/mkdpdf/document/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.464288 mkdpdf-0.2.5/mkdpdf/document/templates/pdf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.471288 mkdpdf-0.2.5/mkdpdf/document/templates/pdf/style/
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/document/templates/pdf/style/document.css
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/document/templates/pdf/style/footer.css
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/document/templates/pdf/style/header.css
+-rw-rw-rw-   0 root         (0) root         (0)     6683 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/document/templates/pdf/style/mermaid.css
+-rw-rw-rw-   0 root         (0) root         (0)     2193 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/document/templates/pdf/style/pdf.css
+-rw-rw-rw-   0 root         (0) root         (0)     3199 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/document/templates/pdf/style/reset.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.471288 mkdpdf-0.2.5/mkdpdf/documentation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/documentation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8053 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/documentation/documentation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.465288 mkdpdf-0.2.5/mkdpdf/documentation/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.472288 mkdpdf-0.2.5/mkdpdf/documentation/templates/md/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.472288 mkdpdf-0.2.5/mkdpdf/documentation/templates/md/class/
+-rw-rw-rw-   0 root         (0) root         (0)      564 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/documentation/templates/md/class/header.md
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/documentation/templates/md/class/main.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.472288 mkdpdf-0.2.5/mkdpdf/documentation/templates/md/functions/
+-rw-rw-rw-   0 root         (0) root         (0)      517 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/documentation/templates/md/functions/header.md
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/documentation/templates/md/functions/main.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/documentation/templates/md/header.md
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/documentation/templates/md/main.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.465288 mkdpdf-0.2.5/mkdpdf/documentation/templates/pdf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.473287 mkdpdf-0.2.5/mkdpdf/documentation/templates/pdf/style/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/documentation/templates/pdf/style/document.css
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/documentation/templates/pdf/style/footer.css
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/documentation/templates/pdf/style/header.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.473287 mkdpdf-0.2.5/mkdpdf/md/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/md/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1298 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/md/md.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.474287 mkdpdf-0.2.5/mkdpdf/pdf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/pdf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5935 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/pdf/pdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3234 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/pdf/publisher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.474287 mkdpdf-0.2.5/mkdpdf/report/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/report/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/report/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.466287 mkdpdf-0.2.5/mkdpdf/report/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.475287 mkdpdf-0.2.5/mkdpdf/report/templates/md/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/report/templates/md/footer.md
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/report/templates/md/header.md
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/report/templates/md/main.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.476287 mkdpdf-0.2.5/mkdpdf/report/templates/pdf/
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/report/templates/pdf/footer.html
+-rw-rw-rw-   0 root         (0) root         (0)      809 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/report/templates/pdf/header.html
+-rw-rw-rw-   0 root         (0) root         (0)     1338 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/report/templates/pdf/main.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.476287 mkdpdf-0.2.5/mkdpdf/report/templates/pdf/style/
+-rw-rw-rw-   0 root         (0) root         (0)      358 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/report/templates/pdf/style/document.css
+-rw-rw-rw-   0 root         (0) root         (0)      755 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/report/templates/pdf/style/footer.css
+-rw-rw-rw-   0 root         (0) root         (0)     1518 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/report/templates/pdf/style/header.css
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/report/templates/pdf/style/pdf.css
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.469287 mkdpdf-0.2.5/mkdpdf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      303 2023-06-15 00:30:33.000000 mkdpdf-0.2.5/mkdpdf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1737 2023-06-15 00:30:33.000000 mkdpdf-0.2.5/mkdpdf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 00:30:33.000000 mkdpdf-0.2.5/mkdpdf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-06-15 00:30:33.000000 mkdpdf-0.2.5/mkdpdf.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-15 00:30:33.000000 mkdpdf-0.2.5/mkdpdf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-15 00:30:33.000000 mkdpdf-0.2.5/mkdpdf.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 00:30:33.477287 mkdpdf-0.2.5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      976 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/setup.py
```

### Comparing `mkdpdf-0.2.4/mkdpdf/configuration.py` & `mkdpdf-0.2.5/mkdpdf/configuration.py`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.4/mkdpdf/document/document.py` & `mkdpdf-0.2.5/mkdpdf/document/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,28 +153,35 @@
         # send message
         server = smtplib.SMTP(HOST, port=587)
         server.starttls()
         server.login(sender, os.environ["EMAIL_PASSWORD"])
         server.sendmail(sender, TO, msg.as_string())
         server.quit()
 
-    def generate(self, main = None, header = None, footer = None, to_file: bool = False):
+    def generate(self, main = None, header = None, footer = None, to_file: bool = False, data: dict = None):
         """
         Generate document.
 
         Args:
+            data (dictonary): key/value pairs to inject before template is transpiled
             footer (string || dictionary): partial or file path for footer template or key/value pairs to find/replace in package template
             header (string || dictionary): partial or file path for header template or key/value pairs to find/replace in package template
             main (string || dictionary): partial or file path for main template or key/value pairs to find/replace in package template
             to_file (boolean): TRUE if content should be written to file
 
         Returns:
             A string representing the full content.
         """
 
+        # inject any data-driven components
+        _footer, _header, _main = self.prep(data)
+
+        # get base
+        f, h, m = self.assemble(_main, _header, _footer) if _footer and _header and _main else self.assemble(main, header, footer)
+
         # get base
         f, h, m = self.assemble(
             main=main,
             header=header,
             footer=footer
         )
 
@@ -182,14 +189,27 @@
         content = self.construct(h, m, f)
 
         # render
         if to_file: self.render(content, self.file_path)
 
         return content
 
+    def prep(self, data: dict = None) -> tuple:
+        """
+        Prepare document by injecting data-driven partials prior to template transpilation.
+
+        Args:
+            data (dictionary): key/value pairs to inject to pre-compiled template partials.
+
+        Returns:
+            A tuple of (footer, header, main) where each is a template partial with any data-driven components injected.
+        """
+
+        return None, None, None
+
     def render(self, content, file_path: str):
         """
         Render document to filesystem.
 
         Args:
             content (string): partial of Markdown or HTML
             file_path (string): output file path
@@ -214,15 +234,18 @@
         result = section
 
         # template is considered to be a string partial
         # it may or may not actually be a template with values to be replaced
         is_template = isinstance(section, str) and os.path.exists(section)
 
         # get core template path
-        file_path = os.path.join(self.directory_path_templates, "%s.%s" % (type, configuration.TEMPLATES[self.format]))
+        document_file_path = os.path.join(self.directory_path_templates, "%s.%s" % (type, configuration.TEMPLATES[self.format]))
+        
+        # determine file path for top-level template
+        file_path = document_file_path if os.path.exists(document_file_path) else os.path.join(configuration.DIRECTORY_PATH_PACKAGE, self.document.template, "templates", self.format, "%s.%s" % (type, configuration.TEMPLATES[self.format]))
 
         # provided template is valid
         if is_template:
 
             # get provided template path
             file_path = section if section.startswith("/") else os.path.join(os.path.dirname(__file__), section)
```

### Comparing `mkdpdf-0.2.4/mkdpdf/document/templates/pdf/style/mermaid.css` & `mkdpdf-0.2.5/mkdpdf/document/templates/pdf/style/mermaid.css`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.4/mkdpdf/document/templates/pdf/style/pdf.css` & `mkdpdf-0.2.5/mkdpdf/document/templates/pdf/style/pdf.css`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.4/mkdpdf/document/templates/pdf/style/reset.css` & `mkdpdf-0.2.5/mkdpdf/document/templates/pdf/style/reset.css`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.4/mkdpdf/documentation/documentation.py` & `mkdpdf-0.2.5/mkdpdf/documentation/documentation.py`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.4/mkdpdf/documentation/templates/md/class/header.md` & `mkdpdf-0.2.5/mkdpdf/documentation/templates/md/class/header.md`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.4/mkdpdf/documentation/templates/md/functions/header.md` & `mkdpdf-0.2.5/mkdpdf/documentation/templates/md/functions/header.md`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.4/mkdpdf/md/md.py` & `mkdpdf-0.2.5/mkdpdf/md/md.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         """
         Args:
             directory_path_templates (string): path of templates directory
         """
 
         # update self
         self.directory_path_templates = directory_path_templates
+        self.template = directory_path_templates.split("/")[-3]
 
     def construct(self, header: str, main: str, footer: str) -> str:
         """
         Construct complete document.
 
         Args:
             footer (string): Markdown partial
@@ -43,10 +44,10 @@
         Args:
             content (string): markdown document
             file_path (string): ouput file path
         """
 
         # create file
         with open(file_path, "w") as file:
-            
+
             # write content to file
             file.write(content)
```

### Comparing `mkdpdf-0.2.4/mkdpdf/pdf/pdf.py` & `mkdpdf-0.2.5/mkdpdf/pdf/pdf.py`

 * *Files 17% similar despite different names*

```diff
@@ -35,20 +35,29 @@
             content (string): HTML partial
             type (enum): header || footer
 
         Returns:
             A tuple where 0 == element, 1 == height for the element.
         """
 
-        # add core partial style
-        styles = self.stylesheets + [os.path.join(configuration.DIRECTORY_PATH_PACKAGE, "document", "templates", "pdf", "style", "%s.css" % type)]
+        # get top-level style file path
+        pdf_file_path = os.path.join(self.directory_path_templates, "style", "pdf.css")
 
-        # update stylesheets
-        styles += [os.path.join(self.directory_path_templates, "style", "%s.css" % type)]
+        # add to core styles
+        styles = self.stylesheets + [pdf_file_path if os.path.exists(pdf_file_path) else os.path.join(configuration.DIRECTORY_PATH_PACKAGE, self.template, "templates", "pdf", "style", "pdf.css")]
+
+        # add core partial type style
+        styles += [os.path.join(configuration.DIRECTORY_PATH_PACKAGE, "document", "templates", "pdf", "style", "%s.css" % type)]
 
+        # get top-level style file path
+        type_file_path = os.path.join(self.directory_path_templates, "style", "%s.css" % type)
+
+        # update stylesheets
+        styles += [type_file_path if os.path.exists(type_file_path) else os.path.join(configuration.DIRECTORY_PATH_PACKAGE, self.template, "templates", "pdf", "style", "%s.css" % type)]
+        
         # calculate space requirement
         element, height = self._compute_overlay_element(type, content, styles)
 
         return (element, height)
 
     def construct(self, header: str, main: str, footer: str) -> str:
         """
@@ -89,16 +98,25 @@
 
         # if not core document class
         if self.template != "document":
 
             # add core partial style
             self.stylesheets += [os.path.join(configuration.DIRECTORY_PATH_PACKAGE, "document", "templates", "pdf", "style", "document.css")]
 
+        # get top-level style file path
+        pdf_file_path = os.path.join(self.directory_path_templates, "style", "pdf.css")
+
+        # update stylesheets
+        self.stylesheets += [pdf_file_path if os.path.exists(pdf_file_path) else os.path.join(configuration.DIRECTORY_PATH_PACKAGE, self.template, "templates", "pdf", "style", "pdf.css")]
+
+        # get top-level style file path
+        document_file_path = os.path.join(self.directory_path_templates, "style", "document.css")
+
         # update stylesheets
-        self.stylesheets += [os.path.join(self.directory_path_templates, "style", "document.css")]
+        self.stylesheets += [document_file_path if os.path.exists(document_file_path) else os.path.join(configuration.DIRECTORY_PATH_PACKAGE, self.template, "templates", "pdf", "style", "document.css")]
 
         if main:
 
             # wrap in required tag if not already
             if (isinstance(main, str) and not main.startswith("<main>")) or (isinstance(main, str) and not main.endswith("</main>")):
                 main = "<main>%s</main>" % main
```

### Comparing `mkdpdf-0.2.4/mkdpdf/pdf/publisher.py` & `mkdpdf-0.2.5/mkdpdf/pdf/publisher.py`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.4/mkdpdf/report/report.py` & `mkdpdf-0.2.5/mkdpdf/report/report.py`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.4/mkdpdf/report/templates/pdf/header.html` & `mkdpdf-0.2.5/mkdpdf/report/templates/pdf/header.html`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.4/mkdpdf/report/templates/pdf/main.html` & `mkdpdf-0.2.5/mkdpdf/report/templates/pdf/main.html`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.4/mkdpdf/report/templates/pdf/style/footer.css` & `mkdpdf-0.2.5/mkdpdf/report/templates/pdf/style/footer.css`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.4/mkdpdf/report/templates/pdf/style/header.css` & `mkdpdf-0.2.5/mkdpdf/report/templates/pdf/style/header.css`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.4/mkdpdf/utilities.py` & `mkdpdf-0.2.5/mkdpdf/utilities.py`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.4/mkdpdf.egg-info/SOURCES.txt` & `mkdpdf-0.2.5/mkdpdf.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,8 +43,9 @@
 mkdpdf/report/templates/md/header.md
 mkdpdf/report/templates/md/main.md
 mkdpdf/report/templates/pdf/footer.html
 mkdpdf/report/templates/pdf/header.html
 mkdpdf/report/templates/pdf/main.html
 mkdpdf/report/templates/pdf/style/document.css
 mkdpdf/report/templates/pdf/style/footer.css
-mkdpdf/report/templates/pdf/style/header.css
+mkdpdf/report/templates/pdf/style/header.css
+mkdpdf/report/templates/pdf/style/pdf.css
```

### Comparing `mkdpdf-0.2.4/setup.py` & `mkdpdf-0.2.5/setup.py`

 * *Files identical despite different names*

