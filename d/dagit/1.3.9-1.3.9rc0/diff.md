# Comparing `tmp/dagit-1.3.9.tar.gz` & `tmp/dagit-1.3.9rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagit-1.3.9.tar", last modified: Thu Jun  8 18:49:57 2023, max compression
+gzip compressed data, was "dagit-1.3.9rc0.tar", last modified: Thu Jun  8 18:27:20 2023, max compression
```

## Comparing `dagit-1.3.9.tar` & `dagit-1.3.9rc0.tar`

### file list

```diff
@@ -1,349 +1,349 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:49:57.409371 dagit-1.3.9/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:43:17.000000 dagit-1.3.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)      185 2023-06-08 18:43:17.000000 dagit-1.3.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      878 2023-06-08 18:49:57.409371 dagit-1.3.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      210 2023-06-08 18:43:17.000000 dagit-1.3.9/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:49:57.321370 dagit-1.3.9/dagit/
--rw-r--r--   0 root         (0) root         (0)      148 2023-06-08 18:43:17.000000 dagit-1.3.9/dagit/__init__.py
--rw-r--r--   0 root         (0) root         (0)       70 2023-06-08 18:43:17.000000 dagit-1.3.9/dagit/__main__.py
--rw-r--r--   0 root         (0) root         (0)     1230 2023-06-08 18:43:17.000000 dagit-1.3.9/dagit/app.py
--rw-r--r--   0 root         (0) root         (0)     7176 2023-06-08 18:43:17.000000 dagit-1.3.9/dagit/cli.py
--rw-r--r--   0 root         (0) root         (0)     3098 2023-06-08 18:43:17.000000 dagit-1.3.9/dagit/debug.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:49:57.321370 dagit-1.3.9/dagit/graphql-playground/
--rw-r--r--   0 root         (0) root         (0)     5057 2023-06-08 18:43:17.000000 dagit-1.3.9/dagit/graphql-playground/favicon.png
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-08 18:43:17.000000 dagit-1.3.9/dagit/graphql-playground/index.css
--rw-r--r--   0 root         (0) root         (0)  2144248 2023-06-08 18:43:17.000000 dagit-1.3.9/dagit/graphql-playground/middleware.js
--rw-r--r--   0 root         (0) root         (0)    12258 2023-06-08 18:43:17.000000 dagit-1.3.9/dagit/graphql.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:17.000000 dagit-1.3.9/dagit/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:49:57.321370 dagit-1.3.9/dagit/schema/
--rw-r--r--   0 root         (0) root         (0)       66 2023-06-08 18:43:17.000000 dagit-1.3.9/dagit/schema/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:49:57.321370 dagit-1.3.9/dagit/templates/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:17.000000 dagit-1.3.9/dagit/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19263 2023-06-08 18:43:17.000000 dagit-1.3.9/dagit/templates/playground.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-08 18:43:17.000000 dagit-1.3.9/dagit/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:49:57.317369 dagit-1.3.9/dagit/webapp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:49:57.325369 dagit-1.3.9/dagit/webapp/build/
--rw-r--r--   0 root         (0) root         (0)  2430052 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/Dagster_world.mp4
--rw-r--r--   0 root         (0) root         (0)    26072 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/asset-manifest.json
--rw-r--r--   0 root         (0) root         (0)      166 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/csp-header.conf
--rw-r--r--   0 root         (0) root         (0)     6474 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/favicon-run-failed.svg
--rw-r--r--   0 root         (0) root         (0)     7630 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/favicon-run-pending.svg
--rw-r--r--   0 root         (0) root         (0)     6008 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/favicon-run-success.svg
--rw-r--r--   0 root         (0) root         (0)    15086 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/favicon.ico
--rw-r--r--   0 root         (0) root         (0)     5396 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/favicon.png
--rw-r--r--   0 root         (0) root         (0)     5977 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/favicon.svg
--rw-r--r--   0 root         (0) root         (0)      887 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/index.html
--rw-r--r--   0 root         (0) root         (0)      299 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/manifest.json
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/robots.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:49:57.317369 dagit-1.3.9/dagit/webapp/build/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:49:57.329370 dagit-1.3.9/dagit/webapp/build/static/css/
--rw-r--r--   0 root         (0) root         (0)     6332 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/css/110.bd613440.chunk.css
--rw-r--r--   0 root         (0) root         (0)    12755 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/css/110.bd613440.chunk.css.map
--rw-r--r--   0 root         (0) root         (0)     6331 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/css/39.bd613440.chunk.css
--rw-r--r--   0 root         (0) root         (0)    12754 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/css/39.bd613440.chunk.css.map
--rw-r--r--   0 root         (0) root         (0)     3592 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/css/428.d9dd5944.chunk.css
--rw-r--r--   0 root         (0) root         (0)     5584 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/css/428.d9dd5944.chunk.css.map
--rw-r--r--   0 root         (0) root         (0)     3592 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/css/596.d9dd5944.chunk.css
--rw-r--r--   0 root         (0) root         (0)     5584 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/css/596.d9dd5944.chunk.css.map
--rw-r--r--   0 root         (0) root         (0)     3592 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/css/619.d9dd5944.chunk.css
--rw-r--r--   0 root         (0) root         (0)     5584 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/css/619.d9dd5944.chunk.css.map
--rw-r--r--   0 root         (0) root         (0)     3592 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/css/741.d9dd5944.chunk.css
--rw-r--r--   0 root         (0) root         (0)     5584 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/css/741.d9dd5944.chunk.css.map
--rw-r--r--   0 root         (0) root         (0)    20921 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/css/897.ca402420.chunk.css
--rw-r--r--   0 root         (0) root         (0)    38042 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/css/897.ca402420.chunk.css.map
--rw-r--r--   0 root         (0) root         (0)     3592 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/css/934.d9dd5944.chunk.css
--rw-r--r--   0 root         (0) root         (0)     5584 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/css/934.d9dd5944.chunk.css.map
--rw-r--r--   0 root         (0) root         (0)   310949 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/css/main.cc1499ae.css
--rw-r--r--   0 root         (0) root         (0)   562339 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/css/main.cc1499ae.css.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:49:57.357370 dagit-1.3.9/dagit/webapp/build/static/js/
--rw-r--r--   0 root         (0) root         (0)    18222 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/110.d9a11a6b.chunk.js
--rw-r--r--   0 root         (0) root         (0)    55239 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/110.d9a11a6b.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)    22784 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/115.d6bdac6b.chunk.js
--rw-r--r--   0 root         (0) root         (0)    68097 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/115.d6bdac6b.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)    57956 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/13.2c6ea5ff.chunk.js
--rw-r--r--   0 root         (0) root         (0)   179575 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/13.2c6ea5ff.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)    19035 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/16.a8349d52.chunk.js
--rw-r--r--   0 root         (0) root         (0)    61169 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/16.a8349d52.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)    12086 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/164.59685ab3.chunk.js
--rw-r--r--   0 root         (0) root         (0)    64438 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/164.59685ab3.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)     7418 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/222.2572a1f8.chunk.js
--rw-r--r--   0 root         (0) root         (0)    23085 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/222.2572a1f8.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)     5054 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/236.1a523fc8.chunk.js
--rw-r--r--   0 root         (0) root         (0)    14826 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/236.1a523fc8.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)    60060 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/351.ab49f740.chunk.js
--rw-r--r--   0 root         (0) root         (0)   187023 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/351.ab49f740.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)    21744 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/369.a58c9f0a.chunk.js
--rw-r--r--   0 root         (0) root         (0)    61199 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/369.a58c9f0a.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)    25876 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/380.962dfd80.chunk.js
--rw-r--r--   0 root         (0) root         (0)    82834 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/380.962dfd80.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)     7892 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/39.18be792d.chunk.js
--rw-r--r--   0 root         (0) root         (0)    22523 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/39.18be792d.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)    41511 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/399.8468b27c.chunk.js
--rw-r--r--   0 root         (0) root         (0)   143394 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/399.8468b27c.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)     2005 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/404.6dacb013.chunk.js
--rw-r--r--   0 root         (0) root         (0)     9341 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/404.6dacb013.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)     1564 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/42.525c0d7e.chunk.js
--rw-r--r--   0 root         (0) root         (0)     5382 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/42.525c0d7e.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)    79726 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/428.1fdcb5aa.chunk.js
--rw-r--r--   0 root         (0) root         (0)   257529 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/428.1fdcb5aa.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)    33710 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/433.34442e76.chunk.js
--rw-r--r--   0 root         (0) root         (0)    82570 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/433.34442e76.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)     4705 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/488.eef691b5.chunk.js
--rw-r--r--   0 root         (0) root         (0)    23141 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/488.eef691b5.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)   135835 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/499.6709b03f.chunk.js
--rw-r--r--   0 root         (0) root         (0)   415267 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/499.6709b03f.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)    20897 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/500.28daa8f6.chunk.js
--rw-r--r--   0 root         (0) root         (0)    65547 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/500.28daa8f6.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)     4596 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/545.7bd7c8c8.chunk.js
--rw-r--r--   0 root         (0) root         (0)    20793 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/545.7bd7c8c8.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)    12003 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/596.3474ee68.chunk.js
--rw-r--r--   0 root         (0) root         (0)    45168 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/596.3474ee68.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)     2005 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/616.f129579c.chunk.js
--rw-r--r--   0 root         (0) root         (0)     9341 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/616.f129579c.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)    73230 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/619.26cee782.chunk.js
--rw-r--r--   0 root         (0) root         (0)   232731 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/619.26cee782.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)    47693 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/620.b8047750.chunk.js
--rw-r--r--   0 root         (0) root         (0)   149962 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/620.b8047750.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)    26170 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/65.ad438c4b.chunk.js
--rw-r--r--   0 root         (0) root         (0)    88717 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/65.ad438c4b.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)   344178 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/66.59ee76a5.chunk.js
--rw-r--r--   0 root         (0) root         (0)  1292068 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/66.59ee76a5.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)     7460 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/676.752162d8.chunk.js
--rw-r--r--   0 root         (0) root         (0)    21178 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/676.752162d8.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)    33707 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/709.1842d480.chunk.js
--rw-r--r--   0 root         (0) root         (0)      145 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/709.1842d480.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   172093 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/709.1842d480.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)    41029 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/723.e5235d0b.chunk.js
--rw-r--r--   0 root         (0) root         (0)   146835 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/723.e5235d0b.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)   123854 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/741.97b02620.chunk.js
--rw-r--r--   0 root         (0) root         (0)   407660 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/741.97b02620.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)     6690 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/833.c37a676f.chunk.js
--rw-r--r--   0 root         (0) root         (0)    24242 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/833.c37a676f.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)   280897 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/867.e1fc3ba4.chunk.js
--rw-r--r--   0 root         (0) root         (0)  1118630 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/867.e1fc3ba4.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)  1087969 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/897.81aba1e7.chunk.js
--rw-r--r--   0 root         (0) root         (0)      421 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/897.81aba1e7.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)  1218213 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/897.81aba1e7.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)     4634 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/934.c4e4c589.chunk.js
--rw-r--r--   0 root         (0) root         (0)    20224 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/934.c4e4c589.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)    13076 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/951.2ea2e357.chunk.js
--rw-r--r--   0 root         (0) root         (0)    51490 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/951.2ea2e357.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)   376742 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/964.53045bbc.chunk.js
--rw-r--r--   0 root         (0) root         (0)      412 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/964.53045bbc.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)  1558252 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/964.53045bbc.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)    24447 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/972.70043f36.chunk.js
--rw-r--r--   0 root         (0) root         (0)   152318 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/972.70043f36.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)    60372 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/975.c9c6f0fc.chunk.js
--rw-r--r--   0 root         (0) root         (0)   311943 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/975.c9c6f0fc.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)    20411 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/984.5a2e0916.chunk.js
--rw-r--r--   0 root         (0) root         (0)    77065 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/984.5a2e0916.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)  2213632 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/main.751d2cd1.js
--rw-r--r--   0 root         (0) root         (0)     3412 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/main.751d2cd1.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)  8015474 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/js/main.751d2cd1.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:49:57.405371 dagit-1.3.9/dagit/webapp/build/static/media/
--rw-r--r--   0 root         (0) root         (0)      616 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/account_circle.a296afc6f576da859ad3a6147e33871e.svg
--rw-r--r--   0 root         (0) root         (0)      201 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/account_tree.ba660f04282e2e65c2cc823247f9957f.svg
--rw-r--r--   0 root         (0) root         (0)      129 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/add.46ae0e09d1132337aa923311b95c4996.svg
--rw-r--r--   0 root         (0) root         (0)      201 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/add_circle.8e9483f8462e800131836e8f0b34f3a9.svg
--rw-r--r--   0 root         (0) root         (0)     3308 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/airbyte.779d254c0ba624daede4c5d0c6986271.svg
--rw-r--r--   0 root         (0) root         (0)     4143 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/airflow.27b7a8ef4b669a18428a07e32292421e.svg
--rw-r--r--   0 root         (0) root         (0)      450 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/alternate_email.48d738adfd01c8b06694a4bdfe3a1c2e.svg
--rw-r--r--   0 root         (0) root         (0)      161 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/arrow_back.6c6d6aeb972d1ae6f7f040c891891aa9.svg
--rw-r--r--   0 root         (0) root         (0)      162 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/arrow_downward.59141210289842787eac557a5a5379af.svg
--rw-r--r--   0 root         (0) root         (0)      117 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/arrow_drop_down.b8b0668b2388799982b3b8a4b8e5674e.svg
--rw-r--r--   0 root         (0) root         (0)      161 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/arrow_forward.9ab56a3225a8d37fccc930301a070887.svg
--rw-r--r--   0 root         (0) root         (0)      745 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/arrow_indent.c8ec491f5a8173b69d086e614217b07d.svg
--rw-r--r--   0 root         (0) root         (0)      160 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/arrow_upward.f9c01d16faaf56fa4247e5bc370c8dda.svg
--rw-r--r--   0 root         (0) root         (0)      721 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/asset.f8acbd2137d80d3ca9ab9f8b946a235c.svg
--rw-r--r--   0 root         (0) root         (0)      856 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/asset_group.d808b2a704c5cd3056c829623d1d8141.svg
--rw-r--r--   0 root         (0) root         (0)     1386 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/asset_non_sda.f7d7d6bf33b22a3368dc32c3fda88b58.svg
--rw-r--r--   0 root         (0) root         (0)     1057 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/asset_plot.06d8855959d1a55dfd189120698be6eb.svg
--rw-r--r--   0 root         (0) root         (0)      459 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/assignment.47b72a44d27bd4c7339c194f03eeac7b.svg
--rw-r--r--   0 root         (0) root         (0)      467 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/assignment_turned_in.54b15bd77d2c623358f7dc4e853abd6f.svg
--rw-r--r--   0 root         (0) root         (0)      307 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/attach_file.85a8c164adaaef23ca175fd0acf24c96.svg
--rw-r--r--   0 root         (0) root         (0)     1185 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/auto-materialize-policy.76a0aa20d7d1694fc479044427ae6739.svg
--rw-r--r--   0 root         (0) root         (0)     5789 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/aws.b54cfc5c1dbb5db2d375ae0811bd940d.svg
--rw-r--r--   0 root         (0) root         (0)     1603 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/azure.11cd3e6f3ed1e9c20797abdd0e6fe2b9.svg
--rw-r--r--   0 root         (0) root         (0)      379 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/azureml.cd3862a40eae4adae185b69e857a9eb9.svg
--rw-r--r--   0 root         (0) root         (0)      460 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/backfill.2b883493b21d31862e5ea81594acc619.svg
--rw-r--r--   0 root         (0) root         (0)     1301 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/bigquery.10f416964937a8ca8bb72acb7bc1e428.svg
--rw-r--r--   0 root         (0) root         (0)      225 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/bolt.18e59be2e03f99fafce7abd9e2b95e62.svg
--rw-r--r--   0 root         (0) root         (0)     1310 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/bp-automatic-updates.7902e250fc949ee071b0d06c0f1df4f4.svg
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/bp-git-commit.db7e12e370614d24e099fed47a6d0a56.svg
--rw-r--r--   0 root         (0) root         (0)     1275 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/bp-send-to-graph.745d2a16f679560887e8cac4c5693919.svg
--rw-r--r--   0 root         (0) root         (0)      319 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/cached.798a2e4097d2fd2d70b96fcab3e29b40.svg
--rw-r--r--   0 root         (0) root         (0)      524 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/calendar.b3faf1862a94dc0239e88f07ba2a2411.svg
--rw-r--r--   0 root         (0) root         (0)      326 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/cancel.6119d754c6689cdb7e5333399d077259.svg
--rw-r--r--   0 root         (0) root         (0)      553 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/census.06160001b14e6c029957bc41169fab37.svg
--rw-r--r--   0 root         (0) root         (0)      585 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/changes-present.8b7c8e199028b6dc9bde78e5990bb6e5.svg
--rw-r--r--   0 root         (0) root         (0)      803 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/chat-support.66bf5aa420673f879868088f0c1f4e2b.svg
--rw-r--r--   0 root         (0) root         (0)      270 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/check_circle.1a1417a5b7c4c5d529c3c4ea5d3853b4.svg
--rw-r--r--   0 root         (0) root         (0)      361 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/checklist.f7f3c64ddee31c87683a8c697b38c488.svg
--rw-r--r--   0 root         (0) root         (0)      156 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/chevron_left.6cc48cf3b53ae86b701cbedc4566fc8f.svg
--rw-r--r--   0 root         (0) root         (0)      151 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/chevron_right.2781d6691940f521bd3426220fe931cc.svg
--rw-r--r--   0 root         (0) root         (0)      210 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/close.007e5026f398137d3180148fc51c743c.svg
--rw-r--r--   0 root         (0) root         (0)     1914 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/concept-book.e16f06698276074121692a7fc882d425.svg
--rw-r--r--   0 root         (0) root         (0)      228 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/content_copy.33179d16ae8d1fc5c694543298d2340d.svg
--rw-r--r--   0 root         (0) root         (0)      748 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/databricks.4f18e1a6a7c5227669ff5113fa2fc450.svg
--rw-r--r--   0 root         (0) root         (0)     5211 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/datadog.decfedd06fc5691072f9cf26e8729010.svg
--rw-r--r--   0 root         (0) root         (0)      508 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/date.a9710c095281f9d1b26d6dd62102fb6a.svg
--rw-r--r--   0 root         (0) root         (0)     2437 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/dbt.5a481bda0c7a769457895bc8a6793424.svg
--rw-r--r--   0 root         (0) root         (0)      194 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/delete.221b3b8c7885c32b603f7ce66b778493.svg
--rw-r--r--   0 root         (0) root         (0)      151 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/done.3030abf3ef824cc6fef0f53d16bcd6b7.svg
--rw-r--r--   0 root         (0) root         (0)      307 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/download_for_offline.17a54471efe39faba8567883069bac06.svg
--rw-r--r--   0 root         (0) root         (0)      132 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/drag_handle.40a5a947ca33faaece095145a17b5c0e.svg
--rw-r--r--   0 root         (0) root         (0)     1134 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/duckdb.9b611ab7159d4917c1ac32a8cb450025.svg
--rw-r--r--   0 root         (0) root         (0)      268 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/dynamic_feed.d8ec571295064f9252867f506e0e2ea7.svg
--rw-r--r--   0 root         (0) root         (0)      307 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/edit.76c8258f928173cfe9b7abd04506bc9c.svg
--rw-r--r--   0 root         (0) root         (0)     1191 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/editor-role.78f067ed2b23adf143e62d632f30ee0b.svg
--rw-r--r--   0 root         (0) root         (0)      274 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/email.7be6e02d7bdf46a5f64e94b42b255696.svg
--rw-r--r--   0 root         (0) root         (0)      197 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/error.3bb67f155055c78cdcc3a25d2e9df4ac.svg
--rw-r--r--   0 root         (0) root         (0)      292 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/error_outline.17ca952d7ce7157956734ee3c4e900e0.svg
--rw-r--r--   0 root         (0) root         (0)      151 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/expand_less.03ee089a5493b26aa60bc62e46d5a390.svg
--rw-r--r--   0 root         (0) root         (0)      155 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/expand_more.c8291f3dbbf3e4a4817950d8be7d2036.svg
--rw-r--r--   0 root         (0) root         (0)      263 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/filter_alt.d0a1c15d1f866e3a0ffaa7603cd80922.svg
--rw-r--r--   0 root         (0) root         (0)     3755 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/fivetran.1892e251b246995424c923774d3cbad9.svg
--rw-r--r--   0 root         (0) root         (0)     1080 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/folder.cf72301142f728e26bf338fd4d8df0d8.svg
--rw-r--r--   0 root         (0) root         (0)      208 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/folder_open.773a19ca1b014538da68485ea1764f4c.svg
--rw-r--r--   0 root         (0) root         (0)      281 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/forum.486f8dcee5610fcfa9b6edfd718bc57a.svg
--rw-r--r--   0 root         (0) root         (0)      606 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/gantt_flat.dc1146a31e69bc02d575713d02ae97b0.svg
--rw-r--r--   0 root         (0) root         (0)      965 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/gantt_waterfall.a8ca5d2d37836df22fdf7d509648a328.svg
--rw-r--r--   0 root         (0) root         (0)     3295 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/github.a851fc867a6e9f3bfe5a29dd33a816fb.svg
--rw-r--r--   0 root         (0) root         (0)     3270 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/github.e9d79da1f6a092a16efe73753e4ca07b.svg
--rw-r--r--   0 root         (0) root         (0)     4596 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/github_pr_closed.f51521840cf693ed0faa12e77e558b41.svg
--rw-r--r--   0 root         (0) root         (0)     3375 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/github_pr_merged.de19ac75b0be63127897e4e18bd05f03.svg
--rw-r--r--   0 root         (0) root         (0)     4106 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/github_pr_open.989b0b33bb4b1725699c5d9f67901771.svg
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/gitlab.283b8c73a74dab8272dcaa85196258d4.svg
--rw-r--r--   0 root         (0) root         (0)      656 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/gitlab.66ec60e846c6f95ff8cbeb12fe14ffc1.svg
--rw-r--r--   0 root         (0) root         (0)     2367 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/googlecloud.9b1271728a87dde0ee8156db230464ef.svg
--rw-r--r--   0 root         (0) root         (0)     1943 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/googlesheets.32beed255c2e96a272fb7e6998696b57.svg
--rw-r--r--   0 root         (0) root         (0)      525 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/graph.24dda4efeffe4dc332392b6bff8f7b1c.svg
--rw-r--r--   0 root         (0) root         (0)      813 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/graph_downstream.92fa32acf8341b884b9aa22ebe6d4808.svg
--rw-r--r--   0 root         (0) root         (0)      417 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/graph_neighbors.3be0c905178236690d885fa991e29f7e.svg
--rw-r--r--   0 root         (0) root         (0)      773 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/graph_upstream.63fbd8803ed43c511959712fee10a37e.svg
--rw-r--r--   0 root         (0) root         (0)     2053 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/great_expectations.6c9ebe25f1ca41bc6bddf5c93353f7bb.svg
--rw-r--r--   0 root         (0) root         (0)      613 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/hex.8a779d5337cbda6f4199bccebf9f7d0e.svg
--rw-r--r--   0 root         (0) root         (0)      503 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/hightouch.e5615cb08e37f9e95af96d2d28aae0ff.svg
--rw-r--r--   0 root         (0) root         (0)      301 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/history.1ef0bfda4ed3e5bd4485c81a8d882bbf.svg
--rw-r--r--   0 root         (0) root         (0)     1308 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/history_toggle_off.f9dfde4bb9d1627dc361876aa1fa8a1d.svg
--rw-r--r--   0 root         (0) root         (0)      295 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/hourglass_bottom.f4e64f944566bdb787a0e9bab12229a4.svg
--rw-r--r--   0 root         (0) root         (0)     1508 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/infinity.0ecb0d166e89cd670ca4a6e58e2a3ee4.svg
--rw-r--r--   0 root         (0) root         (0)      249 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/info.c369ea7f5795cb944d716e65fb7adf2a.svg
--rw-r--r--   0 root         (0) root         (0)     1061 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/job.4a5aef0794e7e02b4ac3c68c048bdaa0.svg
--rw-r--r--   0 root         (0) root         (0)     3277 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/jupyter.51154b82b31513aa7792b83b17f9a693.svg
--rw-r--r--   0 root         (0) root         (0)     8888 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/k8s.a08f945a89acf780bdb0c1ec2d09a052.svg
--rw-r--r--   0 root         (0) root         (0)     1445 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/keras.db48ad9de6ea4a6cfd9d2e7eb7f316a9.svg
--rw-r--r--   0 root         (0) root         (0)      238 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/layers.2cece577e1094424c6deb3cd3b1d06d3.svg
--rw-r--r--   0 root         (0) root         (0)      269 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/line_style.cadefcb195e256e49d5174b308a63acc.svg
--rw-r--r--   0 root         (0) root         (0)      354 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/linear_scale.f4495915c49187bb0e80cce390de2f50.svg
--rw-r--r--   0 root         (0) root         (0)      272 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/link.056cf0694609868aa963fd4dec72601c.svg
--rw-r--r--   0 root         (0) root         (0)      288 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/list.0110a855b71f6a9bccad3a9d41cf36d5.svg
--rw-r--r--   0 root         (0) root         (0)      285 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/location_on.45bee388337acc3c028778d8d2057826.svg
--rw-r--r--   0 root         (0) root         (0)      426 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/lock.659e94a439af79fbf527b47756a7fa06.svg
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/logout.c99a6b9dce578e2f5999f3a1dc891f47.svg
--rw-r--r--   0 root         (0) root         (0)     1866 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/looker.6540e1606753910ae6c9c6d9cff50207.svg
--rw-r--r--   0 root         (0) root         (0)      450 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/materialization.afde2027d3cb7b58f220d1bd54d8f093.svg
--rw-r--r--   0 root         (0) root         (0)     1276 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/matplotlib.bbcf886e4954de565e736fb624b59c5a.svg
--rw-r--r--   0 root         (0) root         (0)     2751 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/meltano.9830a17a48cd84a7fd2add476a16ba81.svg
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/menu.57fbb7a17b2b905077319bd9a544ac38.svg
--rw-r--r--   0 root         (0) root         (0)      841 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/menu_book.5c51721988ed1fc83992d837fc30e050.svg
--rw-r--r--   0 root         (0) root         (0)      734 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/mlflow.97f9639b830263bfa8a29a01102ea5f3.svg
--rw-r--r--   0 root         (0) root         (0)      881 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/modal.a49a47a7d6edd5445754c18a2fd938d6.svg
--rw-r--r--   0 root         (0) root         (0)      248 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/more_horiz.e4632771af1a48e1ef71cac26b0deac0.svg
--rw-r--r--   0 root         (0) root         (0)     1506 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/msteams.a30e33e8be028fb5d4cd8521cc60e5a2.svg
--rw-r--r--   0 root         (0) root         (0)      489 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/nightlight.990ebfc19824703b04cc4ad28365a977.svg
--rw-r--r--   0 root         (0) root         (0)      463 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/no_access.92711c6baf66ba927401c47e02797377.svg
--rw-r--r--   0 root         (0) root         (0)     4402 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/noteable.e70e2c13aa1a831e02ccefbba156ef63.svg
--rw-r--r--   0 root         (0) root         (0)     1300 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/numpy.8e82f8598d4944ae78c3f5b69f767e4f.svg
--rw-r--r--   0 root         (0) root         (0)      514 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/observation.f1be1e977b7173c72337468de8f2cb40.svg
--rw-r--r--   0 root         (0) root         (0)     1757 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/open_in_new.2e785324d0d98072b71d671c21c4d790.svg
--rw-r--r--   0 root         (0) root         (0)     3426 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/openai.7bb687d59f333c0ec9eca4ce2b21b65b.svg
--rw-r--r--   0 root         (0) root         (0)     1333 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/pandas.6c58acfedca1947b166b39e0a71d5d7b.svg
--rw-r--r--   0 root         (0) root         (0)      812 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/panel_hide_right.2028e7b131059b1e1c669a010de7717b.svg
--rw-r--r--   0 root         (0) root         (0)      270 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/panel_show_both.76f4b18294ee5fcec688a576bff88b71.svg
--rw-r--r--   0 root         (0) root         (0)      671 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/panel_show_bottom.970e781799aa8e58ee4a543b29139b9d.svg
--rw-r--r--   0 root         (0) root         (0)      799 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/panel_show_left.ff37d58a46745ed97499b5f741fedb5d.svg
--rw-r--r--   0 root         (0) root         (0)      826 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/panel_show_right.931b96c4f6504bfbbe0f81d2f9a08931.svg
--rw-r--r--   0 root         (0) root         (0)      766 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/panel_show_top.b89932289cb00668982ef4a749cfa0c9.svg
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/partition.a348f234b626b7fcc869de5dc9bd681c.svg
--rw-r--r--   0 root         (0) root         (0)      167 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/partition_failure.f6e26b9becf16a002884878b47fd60ee.svg
--rw-r--r--   0 root         (0) root         (0)      173 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/partition_missing.845ec0fb132755728503af0182bef617.svg
--rw-r--r--   0 root         (0) root         (0)      369 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/partition_stale.8e6badf4b43cbcf76a95a77984cf185e.svg
--rw-r--r--   0 root         (0) root         (0)      154 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/partition_success.4792b7c064065f8771d6d86e46591d2b.svg
--rw-r--r--   0 root         (0) root         (0)      621 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/people.cc1aa8314a46643a3364a9a750466580.svg
--rw-r--r--   0 root         (0) root         (0)      819 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/plotly.0c6b502c8a9f8aa0c4c576555252ed72.svg
--rw-r--r--   0 root         (0) root         (0)    12630 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/polars.a23f165351e16be9ed56ad27db12e77b.svg
--rw-r--r--   0 root         (0) root         (0)    10657 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/postgres.37e2f7232240b06e4c71dfd924b934ba.svg
--rw-r--r--   0 root         (0) root         (0)     3109 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/powerbi.c6084367295ea652a4d3dc1240f33005.svg
--rw-r--r--   0 root         (0) root         (0)     1574 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/pyspark.26d4f6a6058852f927349f005044fcfc.svg
--rw-r--r--   0 root         (0) root         (0)     1955 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/python.5974f9aa9701613dc227bfe1c7e6bcf0.svg
--rw-r--r--   0 root         (0) root         (0)     1200 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/pytorch.bfa44d92221183d18177e3b1551267a4.svg
--rw-r--r--   0 root         (0) root         (0)      303 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/refresh.2ae2dcc81401d3bff305c9bd51ec9d10.svg
--rw-r--r--   0 root         (0) root         (0)      402 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/replay.6e6c3741d5e312e7fad295c63d20a509.svg
--rw-r--r--   0 root         (0) root         (0)     3378 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/sagemaker.21f0ed59e6a24db1a61bb4ee20380bb3.svg
--rw-r--r--   0 root         (0) root         (0)      283 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/schedule.e5f3415364955a37670c97f0dc54b834.svg
--rw-r--r--   0 root         (0) root         (0)      236 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/schema.42ee8c3cf75a42357d99d65820a22937.svg
--rw-r--r--   0 root         (0) root         (0)      575 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/scikitlearn.d812aca93b2ca0ad2ca0d8b970f7d582.svg
--rw-r--r--   0 root         (0) root         (0)     2486 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/scipy.69dca57b7cdb034187090b416e8c79f0.svg
--rw-r--r--   0 root         (0) root         (0)      303 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/search.9eb64800a329d1571f77113ecb5548b8.svg
--rw-r--r--   0 root         (0) root         (0)     2550 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/segment.541ddbc63cea9a27c8862845c52ce283.svg
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/sensors.77c9e5a5865d388e26d1d633955b0926.svg
--rw-r--r--   0 root         (0) root         (0)     1352 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/settings.1bd4892609f13a2e60546321b7f13314.svg
--rw-r--r--   0 root         (0) root         (0)      266 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/settings_backup_restore.ee506e4766d1e035f4811e836edf2094.svg
--rw-r--r--   0 root         (0) root         (0)     1394 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/slack.044efd1bb71a81557b7b948bc341a6c5.svg
--rw-r--r--   0 root         (0) root         (0)     3040 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/slack.af9af09e3f249db84d15f08fd5e2f5a9.svg
--rw-r--r--   0 root         (0) root         (0)     5275 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/snowflake.ef32001ccd5f9971225e1ab87ebafd36.svg
--rw-r--r--   0 root         (0) root         (0)      355 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/sort_by_alpha.532f6d73bb467bd7f37d93a04a312b08.svg
--rw-r--r--   0 root         (0) root         (0)      248 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/source.158280a3afe08adda49ed3db862c58d1.svg
--rw-r--r--   0 root         (0) root         (0)     1098 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/source_asset.5e7dd17788ede963d1b88f0d6b0a3e22.svg
--rw-r--r--   0 root         (0) root         (0)      339 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/speed.f28b605ed207a5107d67f4cc61036cf7.svg
--rw-r--r--   0 root         (0) root         (0)      279 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/splitscreen.343bb8a29fbb0964d23340c6803a12d5.svg
--rw-r--r--   0 root         (0) root         (0)      617 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/sql.91e23fd4d8ab00ba5cce382a54bb411c.svg
--rw-r--r--   0 root         (0) root         (0)      198 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/star.d74f54c52a4d3349dacb2f0a0984563a.svg
--rw-r--r--   0 root         (0) root         (0)      456 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/star_outline.6661f4a09f915fd8a5e06270c876c301.svg
--rw-r--r--   0 root         (0) root         (0)     2052 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/status.f029e1e93dd914331f3432eedf6a9e16.svg
--rw-r--r--   0 root         (0) root         (0)      753 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/stitch.f574efb807adf97d9c41fbd7f4daff8c.svg
--rw-r--r--   0 root         (0) root         (0)      867 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/stripe.9fd4519d0043d6764806c7698279384a.svg
--rw-r--r--   0 root         (0) root         (0)       98 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/subtract.260546d7dd2eaed533a43b363180d557.svg
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/sync_problem.adc729b0d77fdce3b45874d91b524127.svg
--rw-r--r--   0 root         (0) root         (0)      371 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/table_view.bf6d93a38d090a6cba9eff7ce728c56a.svg
--rw-r--r--   0 root         (0) root         (0)     1551 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/tableau.5a4ab40d34dcf8f7edf243375413f10a.svg
--rw-r--r--   0 root         (0) root         (0)      901 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/tag.1d6d850ea4698643e02e3f600561a821.svg
--rw-r--r--   0 root         (0) root         (0)     1579 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/tensorflow.b6cf40a201adf268307f3a4d645c447b.svg
--rw-r--r--   0 root         (0) root         (0)      356 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/timer.ef79edd521a1856787feb000f0900b19.svg
--rw-r--r--   0 root         (0) root         (0)      300 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/toggle_off.5666d0e5f69a451e0cd3db4146202477.svg
--rw-r--r--   0 root         (0) root         (0)      300 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/toggle_on.ffc5eacfd2ffa36d9c8bef5f895b58d5.svg
--rw-r--r--   0 root         (0) root         (0)      674 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/toggle_whitespace.90f118f10312bfc3ef64155412cfc370.svg
--rw-r--r--   0 root         (0) root         (0)      220 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/tune.4b840c1ef11a9f1250369d0f786d6ba8.svg
--rw-r--r--   0 root         (0) root         (0)      300 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/unfold_less.16a806357025e4c17864dac51600129b.svg
--rw-r--r--   0 root         (0) root         (0)      220 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/unfold_more.07df1f54ba8982f64bff81c08f2c319f.svg
--rw-r--r--   0 root         (0) root         (0)      341 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/vercel.6cd9f804a71ca1f104effc3fbb382523.svg
--rw-r--r--   0 root         (0) root         (0)      145 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/vertical_align_bottom.1baf9645d902b2ceacf46a044b4f9d7f.svg
--rw-r--r--   0 root         (0) root         (0)      169 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/vertical_align_center.6a2e7a10cb3045d84b224e86e62c92e8.svg
--rw-r--r--   0 root         (0) root         (0)      142 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/vertical_align_top.3d2ab8f3b496675a0eb294a94975a96c.svg
--rw-r--r--   0 root         (0) root         (0)      210 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/view_list.a2af6983d2e792473a58a65f9e146e2e.svg
--rw-r--r--   0 root         (0) root         (0)      399 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/visibility.6f62021171d5123f17f557e8b9a92b19.svg
--rw-r--r--   0 root         (0) root         (0)      772 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/visibility_off.e276c4f81d3ab0d87be83ebb13d0f647.svg
--rw-r--r--   0 root         (0) root         (0)      151 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/warning.0b3db3c7e58c768cfa8f42c1ead1eda7.svg
--rw-r--r--   0 root         (0) root         (0)      177 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/waterfall_chart.ff3d7da784a217362164436432c00545.svg
--rw-r--r--   0 root         (0) root         (0)     2862 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/weights_and_biases.89d763e7978e7d4da207359969008aac.svg
--rw-r--r--   0 root         (0) root         (0)      682 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/workspaces.f030e273f2b0e3c25966278c2309c5b7.svg
--rw-r--r--   0 root         (0) root         (0)      221 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/wysiwyg.e3466d16e45f14923756d135524d90dd.svg
--rw-r--r--   0 root         (0) root         (0)      633 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/youtube.2e616e27606d325ca9f150fdb469a0b2.svg
--rw-r--r--   0 root         (0) root         (0)      333 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/zoom_in.3fa111d9e1e5f635e59283ebc32c78d2.svg
--rw-r--r--   0 root         (0) root         (0)      314 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/static/media/zoom_out.f4b85a89fd775eac6dd897c3ba96ff60.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:49:57.317369 dagit-1.3.9/dagit/webapp/build/vendor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:49:57.405371 dagit-1.3.9/dagit/webapp/build/vendor/graphql-playground/
--rw-r--r--   0 root         (0) root         (0)     5057 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/vendor/graphql-playground/favicon.png
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/vendor/graphql-playground/index.css
--rw-r--r--   0 root         (0) root         (0)  2144248 2023-06-08 18:49:56.000000 dagit-1.3.9/dagit/webapp/build/vendor/graphql-playground/middleware.js
--rw-r--r--   0 root         (0) root         (0)    13040 2023-06-08 18:43:17.000000 dagit-1.3.9/dagit/webserver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:49:57.321370 dagit-1.3.9/dagit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      878 2023-06-08 18:49:57.000000 dagit-1.3.9/dagit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    21808 2023-06-08 18:49:57.000000 dagit-1.3.9/dagit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:49:57.000000 dagit-1.3.9/dagit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       72 2023-06-08 18:49:57.000000 dagit-1.3.9/dagit.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      128 2023-06-08 18:49:57.000000 dagit-1.3.9/dagit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-08 18:49:57.000000 dagit-1.3.9/dagit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      153 2023-06-08 18:49:57.409371 dagit-1.3.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1780 2023-06-08 18:43:17.000000 dagit-1.3.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:20.761860 dagit-1.3.9rc0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:45.000000 dagit-1.3.9rc0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      185 2023-06-08 18:20:45.000000 dagit-1.3.9rc0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      881 2023-06-08 18:27:20.761860 dagit-1.3.9rc0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      210 2023-06-08 18:20:45.000000 dagit-1.3.9rc0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:20.681859 dagit-1.3.9rc0/dagit/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-06-08 18:20:45.000000 dagit-1.3.9rc0/dagit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       70 2023-06-08 18:20:45.000000 dagit-1.3.9rc0/dagit/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1230 2023-06-08 18:20:45.000000 dagit-1.3.9rc0/dagit/app.py
+-rw-r--r--   0 root         (0) root         (0)     7176 2023-06-08 18:20:45.000000 dagit-1.3.9rc0/dagit/cli.py
+-rw-r--r--   0 root         (0) root         (0)     3098 2023-06-08 18:20:45.000000 dagit-1.3.9rc0/dagit/debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:20.681859 dagit-1.3.9rc0/dagit/graphql-playground/
+-rw-r--r--   0 root         (0) root         (0)     5057 2023-06-08 18:20:45.000000 dagit-1.3.9rc0/dagit/graphql-playground/favicon.png
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-08 18:20:45.000000 dagit-1.3.9rc0/dagit/graphql-playground/index.css
+-rw-r--r--   0 root         (0) root         (0)  2144248 2023-06-08 18:20:45.000000 dagit-1.3.9rc0/dagit/graphql-playground/middleware.js
+-rw-r--r--   0 root         (0) root         (0)    12258 2023-06-08 18:20:45.000000 dagit-1.3.9rc0/dagit/graphql.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:45.000000 dagit-1.3.9rc0/dagit/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:20.685859 dagit-1.3.9rc0/dagit/schema/
+-rw-r--r--   0 root         (0) root         (0)       66 2023-06-08 18:20:45.000000 dagit-1.3.9rc0/dagit/schema/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:20.685859 dagit-1.3.9rc0/dagit/templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:45.000000 dagit-1.3.9rc0/dagit/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19263 2023-06-08 18:20:45.000000 dagit-1.3.9rc0/dagit/templates/playground.py
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-08 18:20:45.000000 dagit-1.3.9rc0/dagit/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:20.673859 dagit-1.3.9rc0/dagit/webapp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:20.689859 dagit-1.3.9rc0/dagit/webapp/build/
+-rw-r--r--   0 root         (0) root         (0)  2430052 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/Dagster_world.mp4
+-rw-r--r--   0 root         (0) root         (0)    26072 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/asset-manifest.json
+-rw-r--r--   0 root         (0) root         (0)      166 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/csp-header.conf
+-rw-r--r--   0 root         (0) root         (0)     6474 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/favicon-run-failed.svg
+-rw-r--r--   0 root         (0) root         (0)     7630 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/favicon-run-pending.svg
+-rw-r--r--   0 root         (0) root         (0)     6008 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/favicon-run-success.svg
+-rw-r--r--   0 root         (0) root         (0)    15086 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)     5396 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/favicon.png
+-rw-r--r--   0 root         (0) root         (0)     5977 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/favicon.svg
+-rw-r--r--   0 root         (0) root         (0)      887 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/index.html
+-rw-r--r--   0 root         (0) root         (0)      299 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/manifest.json
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/robots.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:20.673859 dagit-1.3.9rc0/dagit/webapp/build/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:20.689859 dagit-1.3.9rc0/dagit/webapp/build/static/css/
+-rw-r--r--   0 root         (0) root         (0)     6332 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/css/110.bd613440.chunk.css
+-rw-r--r--   0 root         (0) root         (0)    12755 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/css/110.bd613440.chunk.css.map
+-rw-r--r--   0 root         (0) root         (0)     6331 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/css/39.bd613440.chunk.css
+-rw-r--r--   0 root         (0) root         (0)    12754 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/css/39.bd613440.chunk.css.map
+-rw-r--r--   0 root         (0) root         (0)     3592 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/css/428.d9dd5944.chunk.css
+-rw-r--r--   0 root         (0) root         (0)     5584 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/css/428.d9dd5944.chunk.css.map
+-rw-r--r--   0 root         (0) root         (0)     3592 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/css/596.d9dd5944.chunk.css
+-rw-r--r--   0 root         (0) root         (0)     5584 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/css/596.d9dd5944.chunk.css.map
+-rw-r--r--   0 root         (0) root         (0)     3592 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/css/619.d9dd5944.chunk.css
+-rw-r--r--   0 root         (0) root         (0)     5584 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/css/619.d9dd5944.chunk.css.map
+-rw-r--r--   0 root         (0) root         (0)     3592 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/css/741.d9dd5944.chunk.css
+-rw-r--r--   0 root         (0) root         (0)     5584 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/css/741.d9dd5944.chunk.css.map
+-rw-r--r--   0 root         (0) root         (0)    20921 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/css/897.ca402420.chunk.css
+-rw-r--r--   0 root         (0) root         (0)    38042 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/css/897.ca402420.chunk.css.map
+-rw-r--r--   0 root         (0) root         (0)     3592 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/css/934.d9dd5944.chunk.css
+-rw-r--r--   0 root         (0) root         (0)     5584 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/css/934.d9dd5944.chunk.css.map
+-rw-r--r--   0 root         (0) root         (0)   310949 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/css/main.cc1499ae.css
+-rw-r--r--   0 root         (0) root         (0)   562339 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/css/main.cc1499ae.css.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:20.713860 dagit-1.3.9rc0/dagit/webapp/build/static/js/
+-rw-r--r--   0 root         (0) root         (0)    18222 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/110.d9a11a6b.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    55239 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/110.d9a11a6b.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)    22784 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/115.d6bdac6b.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    68097 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/115.d6bdac6b.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)    57956 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/13.2c6ea5ff.chunk.js
+-rw-r--r--   0 root         (0) root         (0)   179575 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/13.2c6ea5ff.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)    19035 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/16.a8349d52.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    61169 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/16.a8349d52.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)    12086 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/164.59685ab3.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    64438 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/164.59685ab3.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)     7418 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/222.2572a1f8.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    23085 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/222.2572a1f8.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)     5054 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/236.1a523fc8.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    14826 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/236.1a523fc8.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)    60060 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/351.ab49f740.chunk.js
+-rw-r--r--   0 root         (0) root         (0)   187023 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/351.ab49f740.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)    21744 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/369.a58c9f0a.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    61199 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/369.a58c9f0a.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)    25876 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/380.962dfd80.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    82834 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/380.962dfd80.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)     7892 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/39.18be792d.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    22523 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/39.18be792d.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)    41511 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/399.8468b27c.chunk.js
+-rw-r--r--   0 root         (0) root         (0)   143394 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/399.8468b27c.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/404.6dacb013.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     9341 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/404.6dacb013.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)     1564 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/42.525c0d7e.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     5382 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/42.525c0d7e.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)    79726 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/428.1fdcb5aa.chunk.js
+-rw-r--r--   0 root         (0) root         (0)   257529 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/428.1fdcb5aa.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)    33710 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/433.34442e76.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    82570 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/433.34442e76.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)     4705 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/488.eef691b5.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    23141 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/488.eef691b5.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)   135835 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/499.6709b03f.chunk.js
+-rw-r--r--   0 root         (0) root         (0)   415267 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/499.6709b03f.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)    20897 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/500.28daa8f6.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    65547 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/500.28daa8f6.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)     4596 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/545.7bd7c8c8.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    20793 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/545.7bd7c8c8.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)    12003 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/596.3474ee68.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    45168 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/596.3474ee68.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/616.f129579c.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     9341 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/616.f129579c.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)    73230 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/619.26cee782.chunk.js
+-rw-r--r--   0 root         (0) root         (0)   232731 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/619.26cee782.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)    47693 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/620.b8047750.chunk.js
+-rw-r--r--   0 root         (0) root         (0)   149962 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/620.b8047750.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)    26170 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/65.ad438c4b.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    88717 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/65.ad438c4b.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)   344178 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/66.59ee76a5.chunk.js
+-rw-r--r--   0 root         (0) root         (0)  1292068 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/66.59ee76a5.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)     7460 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/676.752162d8.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    21178 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/676.752162d8.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)    33707 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/709.1842d480.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      145 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/709.1842d480.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   172093 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/709.1842d480.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)    41029 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/723.e5235d0b.chunk.js
+-rw-r--r--   0 root         (0) root         (0)   146835 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/723.e5235d0b.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)   123854 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/741.97b02620.chunk.js
+-rw-r--r--   0 root         (0) root         (0)   407660 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/741.97b02620.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)     6690 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/833.c37a676f.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    24242 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/833.c37a676f.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)   280897 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/867.e1fc3ba4.chunk.js
+-rw-r--r--   0 root         (0) root         (0)  1118630 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/867.e1fc3ba4.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)  1087969 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/897.81aba1e7.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      421 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/897.81aba1e7.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)  1218213 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/897.81aba1e7.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)     4634 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/934.c4e4c589.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    20224 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/934.c4e4c589.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)    13076 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/951.2ea2e357.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    51490 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/951.2ea2e357.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)   376742 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/964.53045bbc.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      412 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/964.53045bbc.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)  1558252 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/964.53045bbc.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)    24447 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/972.70043f36.chunk.js
+-rw-r--r--   0 root         (0) root         (0)   152318 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/972.70043f36.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)    60372 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/975.c9c6f0fc.chunk.js
+-rw-r--r--   0 root         (0) root         (0)   311943 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/975.c9c6f0fc.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)    20411 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/984.5a2e0916.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    77065 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/984.5a2e0916.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)  2213632 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/main.751d2cd1.js
+-rw-r--r--   0 root         (0) root         (0)     3412 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/main.751d2cd1.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)  8015474 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/js/main.751d2cd1.js.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:20.757860 dagit-1.3.9rc0/dagit/webapp/build/static/media/
+-rw-r--r--   0 root         (0) root         (0)      616 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/account_circle.a296afc6f576da859ad3a6147e33871e.svg
+-rw-r--r--   0 root         (0) root         (0)      201 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/account_tree.ba660f04282e2e65c2cc823247f9957f.svg
+-rw-r--r--   0 root         (0) root         (0)      129 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/add.46ae0e09d1132337aa923311b95c4996.svg
+-rw-r--r--   0 root         (0) root         (0)      201 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/add_circle.8e9483f8462e800131836e8f0b34f3a9.svg
+-rw-r--r--   0 root         (0) root         (0)     3308 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/airbyte.779d254c0ba624daede4c5d0c6986271.svg
+-rw-r--r--   0 root         (0) root         (0)     4143 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/airflow.27b7a8ef4b669a18428a07e32292421e.svg
+-rw-r--r--   0 root         (0) root         (0)      450 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/alternate_email.48d738adfd01c8b06694a4bdfe3a1c2e.svg
+-rw-r--r--   0 root         (0) root         (0)      161 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/arrow_back.6c6d6aeb972d1ae6f7f040c891891aa9.svg
+-rw-r--r--   0 root         (0) root         (0)      162 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/arrow_downward.59141210289842787eac557a5a5379af.svg
+-rw-r--r--   0 root         (0) root         (0)      117 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/arrow_drop_down.b8b0668b2388799982b3b8a4b8e5674e.svg
+-rw-r--r--   0 root         (0) root         (0)      161 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/arrow_forward.9ab56a3225a8d37fccc930301a070887.svg
+-rw-r--r--   0 root         (0) root         (0)      745 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/arrow_indent.c8ec491f5a8173b69d086e614217b07d.svg
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/arrow_upward.f9c01d16faaf56fa4247e5bc370c8dda.svg
+-rw-r--r--   0 root         (0) root         (0)      721 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/asset.f8acbd2137d80d3ca9ab9f8b946a235c.svg
+-rw-r--r--   0 root         (0) root         (0)      856 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/asset_group.d808b2a704c5cd3056c829623d1d8141.svg
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/asset_non_sda.f7d7d6bf33b22a3368dc32c3fda88b58.svg
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/asset_plot.06d8855959d1a55dfd189120698be6eb.svg
+-rw-r--r--   0 root         (0) root         (0)      459 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/assignment.47b72a44d27bd4c7339c194f03eeac7b.svg
+-rw-r--r--   0 root         (0) root         (0)      467 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/assignment_turned_in.54b15bd77d2c623358f7dc4e853abd6f.svg
+-rw-r--r--   0 root         (0) root         (0)      307 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/attach_file.85a8c164adaaef23ca175fd0acf24c96.svg
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/auto-materialize-policy.76a0aa20d7d1694fc479044427ae6739.svg
+-rw-r--r--   0 root         (0) root         (0)     5789 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/aws.b54cfc5c1dbb5db2d375ae0811bd940d.svg
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/azure.11cd3e6f3ed1e9c20797abdd0e6fe2b9.svg
+-rw-r--r--   0 root         (0) root         (0)      379 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/azureml.cd3862a40eae4adae185b69e857a9eb9.svg
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/backfill.2b883493b21d31862e5ea81594acc619.svg
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/bigquery.10f416964937a8ca8bb72acb7bc1e428.svg
+-rw-r--r--   0 root         (0) root         (0)      225 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/bolt.18e59be2e03f99fafce7abd9e2b95e62.svg
+-rw-r--r--   0 root         (0) root         (0)     1310 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/bp-automatic-updates.7902e250fc949ee071b0d06c0f1df4f4.svg
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/bp-git-commit.db7e12e370614d24e099fed47a6d0a56.svg
+-rw-r--r--   0 root         (0) root         (0)     1275 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/bp-send-to-graph.745d2a16f679560887e8cac4c5693919.svg
+-rw-r--r--   0 root         (0) root         (0)      319 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/cached.798a2e4097d2fd2d70b96fcab3e29b40.svg
+-rw-r--r--   0 root         (0) root         (0)      524 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/calendar.b3faf1862a94dc0239e88f07ba2a2411.svg
+-rw-r--r--   0 root         (0) root         (0)      326 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/cancel.6119d754c6689cdb7e5333399d077259.svg
+-rw-r--r--   0 root         (0) root         (0)      553 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/census.06160001b14e6c029957bc41169fab37.svg
+-rw-r--r--   0 root         (0) root         (0)      585 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/changes-present.8b7c8e199028b6dc9bde78e5990bb6e5.svg
+-rw-r--r--   0 root         (0) root         (0)      803 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/chat-support.66bf5aa420673f879868088f0c1f4e2b.svg
+-rw-r--r--   0 root         (0) root         (0)      270 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/check_circle.1a1417a5b7c4c5d529c3c4ea5d3853b4.svg
+-rw-r--r--   0 root         (0) root         (0)      361 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/checklist.f7f3c64ddee31c87683a8c697b38c488.svg
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/chevron_left.6cc48cf3b53ae86b701cbedc4566fc8f.svg
+-rw-r--r--   0 root         (0) root         (0)      151 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/chevron_right.2781d6691940f521bd3426220fe931cc.svg
+-rw-r--r--   0 root         (0) root         (0)      210 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/close.007e5026f398137d3180148fc51c743c.svg
+-rw-r--r--   0 root         (0) root         (0)     1914 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/concept-book.e16f06698276074121692a7fc882d425.svg
+-rw-r--r--   0 root         (0) root         (0)      228 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/content_copy.33179d16ae8d1fc5c694543298d2340d.svg
+-rw-r--r--   0 root         (0) root         (0)      748 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/databricks.4f18e1a6a7c5227669ff5113fa2fc450.svg
+-rw-r--r--   0 root         (0) root         (0)     5211 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/datadog.decfedd06fc5691072f9cf26e8729010.svg
+-rw-r--r--   0 root         (0) root         (0)      508 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/date.a9710c095281f9d1b26d6dd62102fb6a.svg
+-rw-r--r--   0 root         (0) root         (0)     2437 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/dbt.5a481bda0c7a769457895bc8a6793424.svg
+-rw-r--r--   0 root         (0) root         (0)      194 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/delete.221b3b8c7885c32b603f7ce66b778493.svg
+-rw-r--r--   0 root         (0) root         (0)      151 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/done.3030abf3ef824cc6fef0f53d16bcd6b7.svg
+-rw-r--r--   0 root         (0) root         (0)      307 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/download_for_offline.17a54471efe39faba8567883069bac06.svg
+-rw-r--r--   0 root         (0) root         (0)      132 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/drag_handle.40a5a947ca33faaece095145a17b5c0e.svg
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/duckdb.9b611ab7159d4917c1ac32a8cb450025.svg
+-rw-r--r--   0 root         (0) root         (0)      268 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/dynamic_feed.d8ec571295064f9252867f506e0e2ea7.svg
+-rw-r--r--   0 root         (0) root         (0)      307 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/edit.76c8258f928173cfe9b7abd04506bc9c.svg
+-rw-r--r--   0 root         (0) root         (0)     1191 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/editor-role.78f067ed2b23adf143e62d632f30ee0b.svg
+-rw-r--r--   0 root         (0) root         (0)      274 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/email.7be6e02d7bdf46a5f64e94b42b255696.svg
+-rw-r--r--   0 root         (0) root         (0)      197 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/error.3bb67f155055c78cdcc3a25d2e9df4ac.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/error_outline.17ca952d7ce7157956734ee3c4e900e0.svg
+-rw-r--r--   0 root         (0) root         (0)      151 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/expand_less.03ee089a5493b26aa60bc62e46d5a390.svg
+-rw-r--r--   0 root         (0) root         (0)      155 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/expand_more.c8291f3dbbf3e4a4817950d8be7d2036.svg
+-rw-r--r--   0 root         (0) root         (0)      263 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/filter_alt.d0a1c15d1f866e3a0ffaa7603cd80922.svg
+-rw-r--r--   0 root         (0) root         (0)     3755 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/fivetran.1892e251b246995424c923774d3cbad9.svg
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/folder.cf72301142f728e26bf338fd4d8df0d8.svg
+-rw-r--r--   0 root         (0) root         (0)      208 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/folder_open.773a19ca1b014538da68485ea1764f4c.svg
+-rw-r--r--   0 root         (0) root         (0)      281 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/forum.486f8dcee5610fcfa9b6edfd718bc57a.svg
+-rw-r--r--   0 root         (0) root         (0)      606 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/gantt_flat.dc1146a31e69bc02d575713d02ae97b0.svg
+-rw-r--r--   0 root         (0) root         (0)      965 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/gantt_waterfall.a8ca5d2d37836df22fdf7d509648a328.svg
+-rw-r--r--   0 root         (0) root         (0)     3295 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/github.a851fc867a6e9f3bfe5a29dd33a816fb.svg
+-rw-r--r--   0 root         (0) root         (0)     3270 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/github.e9d79da1f6a092a16efe73753e4ca07b.svg
+-rw-r--r--   0 root         (0) root         (0)     4596 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/github_pr_closed.f51521840cf693ed0faa12e77e558b41.svg
+-rw-r--r--   0 root         (0) root         (0)     3375 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/github_pr_merged.de19ac75b0be63127897e4e18bd05f03.svg
+-rw-r--r--   0 root         (0) root         (0)     4106 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/github_pr_open.989b0b33bb4b1725699c5d9f67901771.svg
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/gitlab.283b8c73a74dab8272dcaa85196258d4.svg
+-rw-r--r--   0 root         (0) root         (0)      656 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/gitlab.66ec60e846c6f95ff8cbeb12fe14ffc1.svg
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/googlecloud.9b1271728a87dde0ee8156db230464ef.svg
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/googlesheets.32beed255c2e96a272fb7e6998696b57.svg
+-rw-r--r--   0 root         (0) root         (0)      525 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/graph.24dda4efeffe4dc332392b6bff8f7b1c.svg
+-rw-r--r--   0 root         (0) root         (0)      813 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/graph_downstream.92fa32acf8341b884b9aa22ebe6d4808.svg
+-rw-r--r--   0 root         (0) root         (0)      417 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/graph_neighbors.3be0c905178236690d885fa991e29f7e.svg
+-rw-r--r--   0 root         (0) root         (0)      773 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/graph_upstream.63fbd8803ed43c511959712fee10a37e.svg
+-rw-r--r--   0 root         (0) root         (0)     2053 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/great_expectations.6c9ebe25f1ca41bc6bddf5c93353f7bb.svg
+-rw-r--r--   0 root         (0) root         (0)      613 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/hex.8a779d5337cbda6f4199bccebf9f7d0e.svg
+-rw-r--r--   0 root         (0) root         (0)      503 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/hightouch.e5615cb08e37f9e95af96d2d28aae0ff.svg
+-rw-r--r--   0 root         (0) root         (0)      301 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/history.1ef0bfda4ed3e5bd4485c81a8d882bbf.svg
+-rw-r--r--   0 root         (0) root         (0)     1308 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/history_toggle_off.f9dfde4bb9d1627dc361876aa1fa8a1d.svg
+-rw-r--r--   0 root         (0) root         (0)      295 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/hourglass_bottom.f4e64f944566bdb787a0e9bab12229a4.svg
+-rw-r--r--   0 root         (0) root         (0)     1508 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/infinity.0ecb0d166e89cd670ca4a6e58e2a3ee4.svg
+-rw-r--r--   0 root         (0) root         (0)      249 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/info.c369ea7f5795cb944d716e65fb7adf2a.svg
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/job.4a5aef0794e7e02b4ac3c68c048bdaa0.svg
+-rw-r--r--   0 root         (0) root         (0)     3277 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/jupyter.51154b82b31513aa7792b83b17f9a693.svg
+-rw-r--r--   0 root         (0) root         (0)     8888 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/k8s.a08f945a89acf780bdb0c1ec2d09a052.svg
+-rw-r--r--   0 root         (0) root         (0)     1445 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/keras.db48ad9de6ea4a6cfd9d2e7eb7f316a9.svg
+-rw-r--r--   0 root         (0) root         (0)      238 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/layers.2cece577e1094424c6deb3cd3b1d06d3.svg
+-rw-r--r--   0 root         (0) root         (0)      269 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/line_style.cadefcb195e256e49d5174b308a63acc.svg
+-rw-r--r--   0 root         (0) root         (0)      354 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/linear_scale.f4495915c49187bb0e80cce390de2f50.svg
+-rw-r--r--   0 root         (0) root         (0)      272 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/link.056cf0694609868aa963fd4dec72601c.svg
+-rw-r--r--   0 root         (0) root         (0)      288 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/list.0110a855b71f6a9bccad3a9d41cf36d5.svg
+-rw-r--r--   0 root         (0) root         (0)      285 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/location_on.45bee388337acc3c028778d8d2057826.svg
+-rw-r--r--   0 root         (0) root         (0)      426 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/lock.659e94a439af79fbf527b47756a7fa06.svg
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/logout.c99a6b9dce578e2f5999f3a1dc891f47.svg
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/looker.6540e1606753910ae6c9c6d9cff50207.svg
+-rw-r--r--   0 root         (0) root         (0)      450 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/materialization.afde2027d3cb7b58f220d1bd54d8f093.svg
+-rw-r--r--   0 root         (0) root         (0)     1276 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/matplotlib.bbcf886e4954de565e736fb624b59c5a.svg
+-rw-r--r--   0 root         (0) root         (0)     2751 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/meltano.9830a17a48cd84a7fd2add476a16ba81.svg
+-rw-r--r--   0 root         (0) root         (0)      146 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/menu.57fbb7a17b2b905077319bd9a544ac38.svg
+-rw-r--r--   0 root         (0) root         (0)      841 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/menu_book.5c51721988ed1fc83992d837fc30e050.svg
+-rw-r--r--   0 root         (0) root         (0)      734 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/mlflow.97f9639b830263bfa8a29a01102ea5f3.svg
+-rw-r--r--   0 root         (0) root         (0)      881 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/modal.a49a47a7d6edd5445754c18a2fd938d6.svg
+-rw-r--r--   0 root         (0) root         (0)      248 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/more_horiz.e4632771af1a48e1ef71cac26b0deac0.svg
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/msteams.a30e33e8be028fb5d4cd8521cc60e5a2.svg
+-rw-r--r--   0 root         (0) root         (0)      489 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/nightlight.990ebfc19824703b04cc4ad28365a977.svg
+-rw-r--r--   0 root         (0) root         (0)      463 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/no_access.92711c6baf66ba927401c47e02797377.svg
+-rw-r--r--   0 root         (0) root         (0)     4402 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/noteable.e70e2c13aa1a831e02ccefbba156ef63.svg
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/numpy.8e82f8598d4944ae78c3f5b69f767e4f.svg
+-rw-r--r--   0 root         (0) root         (0)      514 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/observation.f1be1e977b7173c72337468de8f2cb40.svg
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/open_in_new.2e785324d0d98072b71d671c21c4d790.svg
+-rw-r--r--   0 root         (0) root         (0)     3426 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/openai.7bb687d59f333c0ec9eca4ce2b21b65b.svg
+-rw-r--r--   0 root         (0) root         (0)     1333 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/pandas.6c58acfedca1947b166b39e0a71d5d7b.svg
+-rw-r--r--   0 root         (0) root         (0)      812 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/panel_hide_right.2028e7b131059b1e1c669a010de7717b.svg
+-rw-r--r--   0 root         (0) root         (0)      270 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/panel_show_both.76f4b18294ee5fcec688a576bff88b71.svg
+-rw-r--r--   0 root         (0) root         (0)      671 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/panel_show_bottom.970e781799aa8e58ee4a543b29139b9d.svg
+-rw-r--r--   0 root         (0) root         (0)      799 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/panel_show_left.ff37d58a46745ed97499b5f741fedb5d.svg
+-rw-r--r--   0 root         (0) root         (0)      826 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/panel_show_right.931b96c4f6504bfbbe0f81d2f9a08931.svg
+-rw-r--r--   0 root         (0) root         (0)      766 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/panel_show_top.b89932289cb00668982ef4a749cfa0c9.svg
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/partition.a348f234b626b7fcc869de5dc9bd681c.svg
+-rw-r--r--   0 root         (0) root         (0)      167 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/partition_failure.f6e26b9becf16a002884878b47fd60ee.svg
+-rw-r--r--   0 root         (0) root         (0)      173 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/partition_missing.845ec0fb132755728503af0182bef617.svg
+-rw-r--r--   0 root         (0) root         (0)      369 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/partition_stale.8e6badf4b43cbcf76a95a77984cf185e.svg
+-rw-r--r--   0 root         (0) root         (0)      154 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/partition_success.4792b7c064065f8771d6d86e46591d2b.svg
+-rw-r--r--   0 root         (0) root         (0)      621 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/people.cc1aa8314a46643a3364a9a750466580.svg
+-rw-r--r--   0 root         (0) root         (0)      819 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/plotly.0c6b502c8a9f8aa0c4c576555252ed72.svg
+-rw-r--r--   0 root         (0) root         (0)    12630 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/polars.a23f165351e16be9ed56ad27db12e77b.svg
+-rw-r--r--   0 root         (0) root         (0)    10657 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/postgres.37e2f7232240b06e4c71dfd924b934ba.svg
+-rw-r--r--   0 root         (0) root         (0)     3109 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/powerbi.c6084367295ea652a4d3dc1240f33005.svg
+-rw-r--r--   0 root         (0) root         (0)     1574 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/pyspark.26d4f6a6058852f927349f005044fcfc.svg
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/python.5974f9aa9701613dc227bfe1c7e6bcf0.svg
+-rw-r--r--   0 root         (0) root         (0)     1200 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/pytorch.bfa44d92221183d18177e3b1551267a4.svg
+-rw-r--r--   0 root         (0) root         (0)      303 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/refresh.2ae2dcc81401d3bff305c9bd51ec9d10.svg
+-rw-r--r--   0 root         (0) root         (0)      402 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/replay.6e6c3741d5e312e7fad295c63d20a509.svg
+-rw-r--r--   0 root         (0) root         (0)     3378 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/sagemaker.21f0ed59e6a24db1a61bb4ee20380bb3.svg
+-rw-r--r--   0 root         (0) root         (0)      283 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/schedule.e5f3415364955a37670c97f0dc54b834.svg
+-rw-r--r--   0 root         (0) root         (0)      236 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/schema.42ee8c3cf75a42357d99d65820a22937.svg
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/scikitlearn.d812aca93b2ca0ad2ca0d8b970f7d582.svg
+-rw-r--r--   0 root         (0) root         (0)     2486 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/scipy.69dca57b7cdb034187090b416e8c79f0.svg
+-rw-r--r--   0 root         (0) root         (0)      303 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/search.9eb64800a329d1571f77113ecb5548b8.svg
+-rw-r--r--   0 root         (0) root         (0)     2550 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/segment.541ddbc63cea9a27c8862845c52ce283.svg
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/sensors.77c9e5a5865d388e26d1d633955b0926.svg
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/settings.1bd4892609f13a2e60546321b7f13314.svg
+-rw-r--r--   0 root         (0) root         (0)      266 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/settings_backup_restore.ee506e4766d1e035f4811e836edf2094.svg
+-rw-r--r--   0 root         (0) root         (0)     1394 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/slack.044efd1bb71a81557b7b948bc341a6c5.svg
+-rw-r--r--   0 root         (0) root         (0)     3040 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/slack.af9af09e3f249db84d15f08fd5e2f5a9.svg
+-rw-r--r--   0 root         (0) root         (0)     5275 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/snowflake.ef32001ccd5f9971225e1ab87ebafd36.svg
+-rw-r--r--   0 root         (0) root         (0)      355 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/sort_by_alpha.532f6d73bb467bd7f37d93a04a312b08.svg
+-rw-r--r--   0 root         (0) root         (0)      248 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/source.158280a3afe08adda49ed3db862c58d1.svg
+-rw-r--r--   0 root         (0) root         (0)     1098 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/source_asset.5e7dd17788ede963d1b88f0d6b0a3e22.svg
+-rw-r--r--   0 root         (0) root         (0)      339 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/speed.f28b605ed207a5107d67f4cc61036cf7.svg
+-rw-r--r--   0 root         (0) root         (0)      279 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/splitscreen.343bb8a29fbb0964d23340c6803a12d5.svg
+-rw-r--r--   0 root         (0) root         (0)      617 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/sql.91e23fd4d8ab00ba5cce382a54bb411c.svg
+-rw-r--r--   0 root         (0) root         (0)      198 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/star.d74f54c52a4d3349dacb2f0a0984563a.svg
+-rw-r--r--   0 root         (0) root         (0)      456 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/star_outline.6661f4a09f915fd8a5e06270c876c301.svg
+-rw-r--r--   0 root         (0) root         (0)     2052 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/status.f029e1e93dd914331f3432eedf6a9e16.svg
+-rw-r--r--   0 root         (0) root         (0)      753 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/stitch.f574efb807adf97d9c41fbd7f4daff8c.svg
+-rw-r--r--   0 root         (0) root         (0)      867 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/stripe.9fd4519d0043d6764806c7698279384a.svg
+-rw-r--r--   0 root         (0) root         (0)       98 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/subtract.260546d7dd2eaed533a43b363180d557.svg
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/sync_problem.adc729b0d77fdce3b45874d91b524127.svg
+-rw-r--r--   0 root         (0) root         (0)      371 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/table_view.bf6d93a38d090a6cba9eff7ce728c56a.svg
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/tableau.5a4ab40d34dcf8f7edf243375413f10a.svg
+-rw-r--r--   0 root         (0) root         (0)      901 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/tag.1d6d850ea4698643e02e3f600561a821.svg
+-rw-r--r--   0 root         (0) root         (0)     1579 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/tensorflow.b6cf40a201adf268307f3a4d645c447b.svg
+-rw-r--r--   0 root         (0) root         (0)      356 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/timer.ef79edd521a1856787feb000f0900b19.svg
+-rw-r--r--   0 root         (0) root         (0)      300 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/toggle_off.5666d0e5f69a451e0cd3db4146202477.svg
+-rw-r--r--   0 root         (0) root         (0)      300 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/toggle_on.ffc5eacfd2ffa36d9c8bef5f895b58d5.svg
+-rw-r--r--   0 root         (0) root         (0)      674 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/toggle_whitespace.90f118f10312bfc3ef64155412cfc370.svg
+-rw-r--r--   0 root         (0) root         (0)      220 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/tune.4b840c1ef11a9f1250369d0f786d6ba8.svg
+-rw-r--r--   0 root         (0) root         (0)      300 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/unfold_less.16a806357025e4c17864dac51600129b.svg
+-rw-r--r--   0 root         (0) root         (0)      220 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/unfold_more.07df1f54ba8982f64bff81c08f2c319f.svg
+-rw-r--r--   0 root         (0) root         (0)      341 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/vercel.6cd9f804a71ca1f104effc3fbb382523.svg
+-rw-r--r--   0 root         (0) root         (0)      145 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/vertical_align_bottom.1baf9645d902b2ceacf46a044b4f9d7f.svg
+-rw-r--r--   0 root         (0) root         (0)      169 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/vertical_align_center.6a2e7a10cb3045d84b224e86e62c92e8.svg
+-rw-r--r--   0 root         (0) root         (0)      142 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/vertical_align_top.3d2ab8f3b496675a0eb294a94975a96c.svg
+-rw-r--r--   0 root         (0) root         (0)      210 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/view_list.a2af6983d2e792473a58a65f9e146e2e.svg
+-rw-r--r--   0 root         (0) root         (0)      399 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/visibility.6f62021171d5123f17f557e8b9a92b19.svg
+-rw-r--r--   0 root         (0) root         (0)      772 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/visibility_off.e276c4f81d3ab0d87be83ebb13d0f647.svg
+-rw-r--r--   0 root         (0) root         (0)      151 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/warning.0b3db3c7e58c768cfa8f42c1ead1eda7.svg
+-rw-r--r--   0 root         (0) root         (0)      177 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/waterfall_chart.ff3d7da784a217362164436432c00545.svg
+-rw-r--r--   0 root         (0) root         (0)     2862 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/weights_and_biases.89d763e7978e7d4da207359969008aac.svg
+-rw-r--r--   0 root         (0) root         (0)      682 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/workspaces.f030e273f2b0e3c25966278c2309c5b7.svg
+-rw-r--r--   0 root         (0) root         (0)      221 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/wysiwyg.e3466d16e45f14923756d135524d90dd.svg
+-rw-r--r--   0 root         (0) root         (0)      633 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/youtube.2e616e27606d325ca9f150fdb469a0b2.svg
+-rw-r--r--   0 root         (0) root         (0)      333 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/zoom_in.3fa111d9e1e5f635e59283ebc32c78d2.svg
+-rw-r--r--   0 root         (0) root         (0)      314 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/static/media/zoom_out.f4b85a89fd775eac6dd897c3ba96ff60.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:20.673859 dagit-1.3.9rc0/dagit/webapp/build/vendor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:20.757860 dagit-1.3.9rc0/dagit/webapp/build/vendor/graphql-playground/
+-rw-r--r--   0 root         (0) root         (0)     5057 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/vendor/graphql-playground/favicon.png
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/vendor/graphql-playground/index.css
+-rw-r--r--   0 root         (0) root         (0)  2144248 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit/webapp/build/vendor/graphql-playground/middleware.js
+-rw-r--r--   0 root         (0) root         (0)    13040 2023-06-08 18:20:45.000000 dagit-1.3.9rc0/dagit/webserver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:20.681859 dagit-1.3.9rc0/dagit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      881 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    21808 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-08 18:27:20.000000 dagit-1.3.9rc0/dagit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      153 2023-06-08 18:27:20.761860 dagit-1.3.9rc0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1786 2023-06-08 18:20:45.000000 dagit-1.3.9rc0/setup.py
```

### Comparing `dagit-1.3.9/LICENSE` & `dagit-1.3.9rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/PKG-INFO` & `dagit-1.3.9rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagit
-Version: 1.3.9
+Version: 1.3.9rc0
 Summary: Web UI for dagster.
 Home-page: https://github.com/dagster-io/dagster
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagit-1.3.9/dagit/app.py` & `dagit-1.3.9rc0/dagit/app.py`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/cli.py` & `dagit-1.3.9rc0/dagit/cli.py`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/debug.py` & `dagit-1.3.9rc0/dagit/debug.py`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/graphql-playground/favicon.png` & `dagit-1.3.9rc0/dagit/graphql-playground/favicon.png`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/graphql-playground/index.css` & `dagit-1.3.9rc0/dagit/graphql-playground/index.css`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/graphql-playground/middleware.js` & `dagit-1.3.9rc0/dagit/graphql-playground/middleware.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/graphql.py` & `dagit-1.3.9rc0/dagit/graphql.py`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/templates/playground.py` & `dagit-1.3.9rc0/dagit/templates/playground.py`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/Dagster_world.mp4` & `dagit-1.3.9rc0/dagit/webapp/build/Dagster_world.mp4`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/asset-manifest.json` & `dagit-1.3.9rc0/dagit/webapp/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/favicon-run-failed.svg` & `dagit-1.3.9rc0/dagit/webapp/build/favicon-run-failed.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/favicon-run-pending.svg` & `dagit-1.3.9rc0/dagit/webapp/build/favicon-run-pending.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/favicon-run-success.svg` & `dagit-1.3.9rc0/dagit/webapp/build/favicon-run-success.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/favicon.ico` & `dagit-1.3.9rc0/dagit/webapp/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/favicon.png` & `dagit-1.3.9rc0/dagit/webapp/build/favicon.png`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/favicon.svg` & `dagit-1.3.9rc0/dagit/webapp/build/favicon.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/index.html` & `dagit-1.3.9rc0/dagit/webapp/build/index.html`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/css/110.bd613440.chunk.css` & `dagit-1.3.9rc0/dagit/webapp/build/static/css/110.bd613440.chunk.css`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/css/110.bd613440.chunk.css.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/css/110.bd613440.chunk.css.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/css/39.bd613440.chunk.css` & `dagit-1.3.9rc0/dagit/webapp/build/static/css/39.bd613440.chunk.css`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/css/39.bd613440.chunk.css.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/css/39.bd613440.chunk.css.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/css/428.d9dd5944.chunk.css` & `dagit-1.3.9rc0/dagit/webapp/build/static/css/428.d9dd5944.chunk.css`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/css/428.d9dd5944.chunk.css.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/css/428.d9dd5944.chunk.css.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/css/596.d9dd5944.chunk.css` & `dagit-1.3.9rc0/dagit/webapp/build/static/css/596.d9dd5944.chunk.css`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/css/596.d9dd5944.chunk.css.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/css/596.d9dd5944.chunk.css.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/css/619.d9dd5944.chunk.css` & `dagit-1.3.9rc0/dagit/webapp/build/static/css/619.d9dd5944.chunk.css`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/css/619.d9dd5944.chunk.css.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/css/619.d9dd5944.chunk.css.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/css/741.d9dd5944.chunk.css` & `dagit-1.3.9rc0/dagit/webapp/build/static/css/741.d9dd5944.chunk.css`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/css/741.d9dd5944.chunk.css.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/css/741.d9dd5944.chunk.css.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/css/897.ca402420.chunk.css` & `dagit-1.3.9rc0/dagit/webapp/build/static/css/897.ca402420.chunk.css`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/css/897.ca402420.chunk.css.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/css/897.ca402420.chunk.css.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/css/934.d9dd5944.chunk.css` & `dagit-1.3.9rc0/dagit/webapp/build/static/css/934.d9dd5944.chunk.css`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/css/934.d9dd5944.chunk.css.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/css/934.d9dd5944.chunk.css.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/css/main.cc1499ae.css` & `dagit-1.3.9rc0/dagit/webapp/build/static/css/main.cc1499ae.css`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/css/main.cc1499ae.css.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/css/main.cc1499ae.css.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/110.d9a11a6b.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/110.d9a11a6b.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/110.d9a11a6b.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/110.d9a11a6b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/115.d6bdac6b.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/115.d6bdac6b.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/115.d6bdac6b.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/115.d6bdac6b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/13.2c6ea5ff.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/13.2c6ea5ff.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/13.2c6ea5ff.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/13.2c6ea5ff.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/16.a8349d52.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/16.a8349d52.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/16.a8349d52.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/16.a8349d52.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/164.59685ab3.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/164.59685ab3.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/164.59685ab3.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/164.59685ab3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/222.2572a1f8.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/222.2572a1f8.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/222.2572a1f8.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/222.2572a1f8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/236.1a523fc8.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/236.1a523fc8.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/236.1a523fc8.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/236.1a523fc8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/351.ab49f740.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/351.ab49f740.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/351.ab49f740.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/351.ab49f740.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/369.a58c9f0a.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/369.a58c9f0a.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/369.a58c9f0a.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/369.a58c9f0a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/380.962dfd80.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/380.962dfd80.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/380.962dfd80.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/380.962dfd80.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/39.18be792d.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/39.18be792d.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/39.18be792d.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/39.18be792d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/399.8468b27c.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/399.8468b27c.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/399.8468b27c.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/399.8468b27c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/404.6dacb013.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/404.6dacb013.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/404.6dacb013.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/404.6dacb013.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/42.525c0d7e.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/42.525c0d7e.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/42.525c0d7e.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/42.525c0d7e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/428.1fdcb5aa.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/428.1fdcb5aa.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/428.1fdcb5aa.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/428.1fdcb5aa.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/433.34442e76.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/433.34442e76.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/433.34442e76.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/433.34442e76.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/488.eef691b5.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/488.eef691b5.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/488.eef691b5.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/488.eef691b5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/499.6709b03f.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/499.6709b03f.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/499.6709b03f.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/499.6709b03f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/500.28daa8f6.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/500.28daa8f6.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/500.28daa8f6.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/500.28daa8f6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/545.7bd7c8c8.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/545.7bd7c8c8.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/545.7bd7c8c8.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/545.7bd7c8c8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/596.3474ee68.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/596.3474ee68.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/596.3474ee68.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/596.3474ee68.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/616.f129579c.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/616.f129579c.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/616.f129579c.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/616.f129579c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/619.26cee782.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/619.26cee782.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/619.26cee782.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/619.26cee782.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/620.b8047750.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/620.b8047750.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/620.b8047750.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/620.b8047750.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/65.ad438c4b.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/65.ad438c4b.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/65.ad438c4b.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/65.ad438c4b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/66.59ee76a5.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/66.59ee76a5.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/66.59ee76a5.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/66.59ee76a5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/676.752162d8.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/676.752162d8.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/676.752162d8.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/676.752162d8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/709.1842d480.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/709.1842d480.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/709.1842d480.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/709.1842d480.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/723.e5235d0b.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/723.e5235d0b.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/723.e5235d0b.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/723.e5235d0b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/741.97b02620.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/741.97b02620.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/741.97b02620.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/741.97b02620.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/833.c37a676f.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/833.c37a676f.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/833.c37a676f.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/833.c37a676f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/867.e1fc3ba4.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/867.e1fc3ba4.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/867.e1fc3ba4.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/867.e1fc3ba4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/897.81aba1e7.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/897.81aba1e7.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/897.81aba1e7.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/897.81aba1e7.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/934.c4e4c589.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/934.c4e4c589.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/934.c4e4c589.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/934.c4e4c589.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/951.2ea2e357.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/951.2ea2e357.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/951.2ea2e357.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/951.2ea2e357.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/964.53045bbc.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/964.53045bbc.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/964.53045bbc.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/964.53045bbc.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/972.70043f36.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/972.70043f36.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/972.70043f36.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/972.70043f36.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/975.c9c6f0fc.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/975.c9c6f0fc.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/975.c9c6f0fc.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/975.c9c6f0fc.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/984.5a2e0916.chunk.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/984.5a2e0916.chunk.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/984.5a2e0916.chunk.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/984.5a2e0916.chunk.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/main.751d2cd1.js` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/main.751d2cd1.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/main.751d2cd1.js.LICENSE.txt` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/main.751d2cd1.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/js/main.751d2cd1.js.map` & `dagit-1.3.9rc0/dagit/webapp/build/static/js/main.751d2cd1.js.map`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/account_circle.a296afc6f576da859ad3a6147e33871e.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/account_circle.a296afc6f576da859ad3a6147e33871e.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/airbyte.779d254c0ba624daede4c5d0c6986271.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/airbyte.779d254c0ba624daede4c5d0c6986271.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/airflow.27b7a8ef4b669a18428a07e32292421e.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/airflow.27b7a8ef4b669a18428a07e32292421e.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/arrow_indent.c8ec491f5a8173b69d086e614217b07d.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/arrow_indent.c8ec491f5a8173b69d086e614217b07d.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/asset.f8acbd2137d80d3ca9ab9f8b946a235c.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/asset.f8acbd2137d80d3ca9ab9f8b946a235c.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/asset_group.d808b2a704c5cd3056c829623d1d8141.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/asset_group.d808b2a704c5cd3056c829623d1d8141.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/asset_non_sda.f7d7d6bf33b22a3368dc32c3fda88b58.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/asset_non_sda.f7d7d6bf33b22a3368dc32c3fda88b58.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/asset_plot.06d8855959d1a55dfd189120698be6eb.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/asset_plot.06d8855959d1a55dfd189120698be6eb.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/auto-materialize-policy.76a0aa20d7d1694fc479044427ae6739.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/auto-materialize-policy.76a0aa20d7d1694fc479044427ae6739.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/aws.b54cfc5c1dbb5db2d375ae0811bd940d.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/aws.b54cfc5c1dbb5db2d375ae0811bd940d.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/azure.11cd3e6f3ed1e9c20797abdd0e6fe2b9.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/azure.11cd3e6f3ed1e9c20797abdd0e6fe2b9.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/bigquery.10f416964937a8ca8bb72acb7bc1e428.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/bigquery.10f416964937a8ca8bb72acb7bc1e428.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/bp-automatic-updates.7902e250fc949ee071b0d06c0f1df4f4.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/bp-automatic-updates.7902e250fc949ee071b0d06c0f1df4f4.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/bp-git-commit.db7e12e370614d24e099fed47a6d0a56.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/bp-git-commit.db7e12e370614d24e099fed47a6d0a56.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/bp-send-to-graph.745d2a16f679560887e8cac4c5693919.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/bp-send-to-graph.745d2a16f679560887e8cac4c5693919.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/calendar.b3faf1862a94dc0239e88f07ba2a2411.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/calendar.b3faf1862a94dc0239e88f07ba2a2411.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/census.06160001b14e6c029957bc41169fab37.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/census.06160001b14e6c029957bc41169fab37.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/changes-present.8b7c8e199028b6dc9bde78e5990bb6e5.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/changes-present.8b7c8e199028b6dc9bde78e5990bb6e5.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/chat-support.66bf5aa420673f879868088f0c1f4e2b.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/chat-support.66bf5aa420673f879868088f0c1f4e2b.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/concept-book.e16f06698276074121692a7fc882d425.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/concept-book.e16f06698276074121692a7fc882d425.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/databricks.4f18e1a6a7c5227669ff5113fa2fc450.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/databricks.4f18e1a6a7c5227669ff5113fa2fc450.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/datadog.decfedd06fc5691072f9cf26e8729010.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/datadog.decfedd06fc5691072f9cf26e8729010.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/dbt.5a481bda0c7a769457895bc8a6793424.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/dbt.5a481bda0c7a769457895bc8a6793424.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/duckdb.9b611ab7159d4917c1ac32a8cb450025.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/duckdb.9b611ab7159d4917c1ac32a8cb450025.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/editor-role.78f067ed2b23adf143e62d632f30ee0b.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/editor-role.78f067ed2b23adf143e62d632f30ee0b.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/fivetran.1892e251b246995424c923774d3cbad9.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/fivetran.1892e251b246995424c923774d3cbad9.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/folder.cf72301142f728e26bf338fd4d8df0d8.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/folder.cf72301142f728e26bf338fd4d8df0d8.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/gantt_flat.dc1146a31e69bc02d575713d02ae97b0.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/gantt_flat.dc1146a31e69bc02d575713d02ae97b0.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/gantt_waterfall.a8ca5d2d37836df22fdf7d509648a328.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/gantt_waterfall.a8ca5d2d37836df22fdf7d509648a328.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/github.a851fc867a6e9f3bfe5a29dd33a816fb.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/github.a851fc867a6e9f3bfe5a29dd33a816fb.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/github.e9d79da1f6a092a16efe73753e4ca07b.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/github.e9d79da1f6a092a16efe73753e4ca07b.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/github_pr_closed.f51521840cf693ed0faa12e77e558b41.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/github_pr_closed.f51521840cf693ed0faa12e77e558b41.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/github_pr_merged.de19ac75b0be63127897e4e18bd05f03.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/github_pr_merged.de19ac75b0be63127897e4e18bd05f03.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/github_pr_open.989b0b33bb4b1725699c5d9f67901771.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/github_pr_open.989b0b33bb4b1725699c5d9f67901771.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/gitlab.283b8c73a74dab8272dcaa85196258d4.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/gitlab.283b8c73a74dab8272dcaa85196258d4.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/gitlab.66ec60e846c6f95ff8cbeb12fe14ffc1.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/gitlab.66ec60e846c6f95ff8cbeb12fe14ffc1.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/googlecloud.9b1271728a87dde0ee8156db230464ef.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/googlecloud.9b1271728a87dde0ee8156db230464ef.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/googlesheets.32beed255c2e96a272fb7e6998696b57.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/googlesheets.32beed255c2e96a272fb7e6998696b57.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/graph.24dda4efeffe4dc332392b6bff8f7b1c.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/graph.24dda4efeffe4dc332392b6bff8f7b1c.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/graph_downstream.92fa32acf8341b884b9aa22ebe6d4808.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/graph_downstream.92fa32acf8341b884b9aa22ebe6d4808.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/graph_upstream.63fbd8803ed43c511959712fee10a37e.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/graph_upstream.63fbd8803ed43c511959712fee10a37e.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/great_expectations.6c9ebe25f1ca41bc6bddf5c93353f7bb.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/great_expectations.6c9ebe25f1ca41bc6bddf5c93353f7bb.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/hex.8a779d5337cbda6f4199bccebf9f7d0e.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/hex.8a779d5337cbda6f4199bccebf9f7d0e.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/history_toggle_off.f9dfde4bb9d1627dc361876aa1fa8a1d.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/history_toggle_off.f9dfde4bb9d1627dc361876aa1fa8a1d.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/infinity.0ecb0d166e89cd670ca4a6e58e2a3ee4.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/infinity.0ecb0d166e89cd670ca4a6e58e2a3ee4.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/job.4a5aef0794e7e02b4ac3c68c048bdaa0.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/job.4a5aef0794e7e02b4ac3c68c048bdaa0.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/jupyter.51154b82b31513aa7792b83b17f9a693.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/jupyter.51154b82b31513aa7792b83b17f9a693.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/k8s.a08f945a89acf780bdb0c1ec2d09a052.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/k8s.a08f945a89acf780bdb0c1ec2d09a052.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/keras.db48ad9de6ea4a6cfd9d2e7eb7f316a9.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/keras.db48ad9de6ea4a6cfd9d2e7eb7f316a9.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/looker.6540e1606753910ae6c9c6d9cff50207.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/looker.6540e1606753910ae6c9c6d9cff50207.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/matplotlib.bbcf886e4954de565e736fb624b59c5a.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/matplotlib.bbcf886e4954de565e736fb624b59c5a.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/meltano.9830a17a48cd84a7fd2add476a16ba81.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/meltano.9830a17a48cd84a7fd2add476a16ba81.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/menu_book.5c51721988ed1fc83992d837fc30e050.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/menu_book.5c51721988ed1fc83992d837fc30e050.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/mlflow.97f9639b830263bfa8a29a01102ea5f3.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/mlflow.97f9639b830263bfa8a29a01102ea5f3.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/modal.a49a47a7d6edd5445754c18a2fd938d6.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/modal.a49a47a7d6edd5445754c18a2fd938d6.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/msteams.a30e33e8be028fb5d4cd8521cc60e5a2.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/msteams.a30e33e8be028fb5d4cd8521cc60e5a2.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/noteable.e70e2c13aa1a831e02ccefbba156ef63.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/noteable.e70e2c13aa1a831e02ccefbba156ef63.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/numpy.8e82f8598d4944ae78c3f5b69f767e4f.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/numpy.8e82f8598d4944ae78c3f5b69f767e4f.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/observation.f1be1e977b7173c72337468de8f2cb40.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/observation.f1be1e977b7173c72337468de8f2cb40.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/open_in_new.2e785324d0d98072b71d671c21c4d790.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/open_in_new.2e785324d0d98072b71d671c21c4d790.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/openai.7bb687d59f333c0ec9eca4ce2b21b65b.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/openai.7bb687d59f333c0ec9eca4ce2b21b65b.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/pandas.6c58acfedca1947b166b39e0a71d5d7b.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/pandas.6c58acfedca1947b166b39e0a71d5d7b.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/panel_hide_right.2028e7b131059b1e1c669a010de7717b.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/panel_hide_right.2028e7b131059b1e1c669a010de7717b.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/panel_show_bottom.970e781799aa8e58ee4a543b29139b9d.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/panel_show_bottom.970e781799aa8e58ee4a543b29139b9d.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/panel_show_left.ff37d58a46745ed97499b5f741fedb5d.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/panel_show_left.ff37d58a46745ed97499b5f741fedb5d.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/panel_show_right.931b96c4f6504bfbbe0f81d2f9a08931.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/panel_show_right.931b96c4f6504bfbbe0f81d2f9a08931.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/panel_show_top.b89932289cb00668982ef4a749cfa0c9.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/panel_show_top.b89932289cb00668982ef4a749cfa0c9.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/partition.a348f234b626b7fcc869de5dc9bd681c.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/partition.a348f234b626b7fcc869de5dc9bd681c.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/people.cc1aa8314a46643a3364a9a750466580.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/people.cc1aa8314a46643a3364a9a750466580.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/plotly.0c6b502c8a9f8aa0c4c576555252ed72.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/plotly.0c6b502c8a9f8aa0c4c576555252ed72.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/polars.a23f165351e16be9ed56ad27db12e77b.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/polars.a23f165351e16be9ed56ad27db12e77b.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/postgres.37e2f7232240b06e4c71dfd924b934ba.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/postgres.37e2f7232240b06e4c71dfd924b934ba.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/powerbi.c6084367295ea652a4d3dc1240f33005.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/powerbi.c6084367295ea652a4d3dc1240f33005.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/pyspark.26d4f6a6058852f927349f005044fcfc.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/pyspark.26d4f6a6058852f927349f005044fcfc.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/python.5974f9aa9701613dc227bfe1c7e6bcf0.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/python.5974f9aa9701613dc227bfe1c7e6bcf0.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/pytorch.bfa44d92221183d18177e3b1551267a4.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/pytorch.bfa44d92221183d18177e3b1551267a4.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/sagemaker.21f0ed59e6a24db1a61bb4ee20380bb3.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/sagemaker.21f0ed59e6a24db1a61bb4ee20380bb3.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/scikitlearn.d812aca93b2ca0ad2ca0d8b970f7d582.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/scikitlearn.d812aca93b2ca0ad2ca0d8b970f7d582.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/scipy.69dca57b7cdb034187090b416e8c79f0.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/scipy.69dca57b7cdb034187090b416e8c79f0.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/segment.541ddbc63cea9a27c8862845c52ce283.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/segment.541ddbc63cea9a27c8862845c52ce283.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/sensors.77c9e5a5865d388e26d1d633955b0926.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/sensors.77c9e5a5865d388e26d1d633955b0926.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/settings.1bd4892609f13a2e60546321b7f13314.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/settings.1bd4892609f13a2e60546321b7f13314.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/slack.044efd1bb71a81557b7b948bc341a6c5.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/slack.044efd1bb71a81557b7b948bc341a6c5.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/slack.af9af09e3f249db84d15f08fd5e2f5a9.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/slack.af9af09e3f249db84d15f08fd5e2f5a9.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/snowflake.ef32001ccd5f9971225e1ab87ebafd36.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/snowflake.ef32001ccd5f9971225e1ab87ebafd36.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/source_asset.5e7dd17788ede963d1b88f0d6b0a3e22.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/source_asset.5e7dd17788ede963d1b88f0d6b0a3e22.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/sql.91e23fd4d8ab00ba5cce382a54bb411c.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/sql.91e23fd4d8ab00ba5cce382a54bb411c.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/status.f029e1e93dd914331f3432eedf6a9e16.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/status.f029e1e93dd914331f3432eedf6a9e16.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/stitch.f574efb807adf97d9c41fbd7f4daff8c.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/stitch.f574efb807adf97d9c41fbd7f4daff8c.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/stripe.9fd4519d0043d6764806c7698279384a.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/stripe.9fd4519d0043d6764806c7698279384a.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/tableau.5a4ab40d34dcf8f7edf243375413f10a.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/tableau.5a4ab40d34dcf8f7edf243375413f10a.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/tag.1d6d850ea4698643e02e3f600561a821.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/tag.1d6d850ea4698643e02e3f600561a821.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/tensorflow.b6cf40a201adf268307f3a4d645c447b.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/tensorflow.b6cf40a201adf268307f3a4d645c447b.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/toggle_whitespace.90f118f10312bfc3ef64155412cfc370.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/toggle_whitespace.90f118f10312bfc3ef64155412cfc370.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/visibility_off.e276c4f81d3ab0d87be83ebb13d0f647.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/visibility_off.e276c4f81d3ab0d87be83ebb13d0f647.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/weights_and_biases.89d763e7978e7d4da207359969008aac.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/weights_and_biases.89d763e7978e7d4da207359969008aac.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/workspaces.f030e273f2b0e3c25966278c2309c5b7.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/workspaces.f030e273f2b0e3c25966278c2309c5b7.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/static/media/youtube.2e616e27606d325ca9f150fdb469a0b2.svg` & `dagit-1.3.9rc0/dagit/webapp/build/static/media/youtube.2e616e27606d325ca9f150fdb469a0b2.svg`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/vendor/graphql-playground/favicon.png` & `dagit-1.3.9rc0/dagit/webapp/build/vendor/graphql-playground/favicon.png`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/vendor/graphql-playground/index.css` & `dagit-1.3.9rc0/dagit/webapp/build/vendor/graphql-playground/index.css`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webapp/build/vendor/graphql-playground/middleware.js` & `dagit-1.3.9rc0/dagit/webapp/build/vendor/graphql-playground/middleware.js`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit/webserver.py` & `dagit-1.3.9rc0/dagit/webserver.py`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/dagit.egg-info/PKG-INFO` & `dagit-1.3.9rc0/dagit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagit
-Version: 1.3.9
+Version: 1.3.9rc0
 Summary: Web UI for dagster.
 Home-page: https://github.com/dagster-io/dagster
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagit-1.3.9/dagit.egg-info/SOURCES.txt` & `dagit-1.3.9rc0/dagit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagit-1.3.9/setup.py` & `dagit-1.3.9rc0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,16 @@
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagit_tests*"]),
     include_package_data=True,
     install_requires=[
         # cli
         "click>=7.0,<9.0",
-        "dagster==1.3.9",
-        "dagster-graphql==1.3.9",
+        "dagster==1.3.9rc0",
+        "dagster-graphql==1.3.9rc0",
         "starlette",
         "uvicorn[standard]",
     ],
     extras_require={
         "notebook": ["nbconvert"],  # notebooks support
         "test": ["starlette[full]"],  # TestClient deps in full
     },
```

