# Comparing `tmp/tutor-cairn-15.0.6.tar.gz` & `tmp/tutor-cairn-16.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-cairn-15.0.6.tar", last modified: Fri May 19 08:15:29 2023, max compression
+gzip compressed data, was "tutor-cairn-16.0.0.tar", last modified: Wed Jun 14 22:26:22 2023, max compression
```

## Comparing `tutor-cairn-15.0.6.tar` & `tutor-cairn-16.0.0.tar`

### file list

```diff
@@ -1,77 +1,83 @@
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/
--rw-rw-r--   0 regis     (1000) regis     (1000)       80 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/MANIFEST.in
--rw-rw-r--   0 regis     (1000) regis     (1000)    16700 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/PKG-INFO
--rw-rw-r--   0 regis     (1000) regis     (1000)    15886 2023-05-19 08:15:25.000000 tutor-cairn-15.0.6/README.rst
--rw-rw-r--   0 regis     (1000) regis     (1000)       38 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/setup.cfg
--rw-rw-r--   0 regis     (1000) regis     (1000)     1610 2023-05-19 08:15:25.000000 tutor-cairn-15.0.6/setup.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.912021 tutor-cairn-15.0.6/tutor_cairn.egg-info/
--rw-rw-r--   0 regis     (1000) regis     (1000)    16700 2023-05-19 08:15:29.000000 tutor-cairn-15.0.6/tutor_cairn.egg-info/PKG-INFO
--rw-rw-r--   0 regis     (1000) regis     (1000)     2500 2023-05-19 08:15:29.000000 tutor-cairn-15.0.6/tutor_cairn.egg-info/SOURCES.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)        1 2023-05-19 08:15:29.000000 tutor-cairn-15.0.6/tutor_cairn.egg-info/dependency_links.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)       45 2023-05-19 08:15:29.000000 tutor-cairn-15.0.6/tutor_cairn.egg-info/entry_points.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)       22 2023-05-19 08:15:29.000000 tutor-cairn-15.0.6/tutor_cairn.egg-info/requires.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)       11 2023-05-19 08:15:29.000000 tutor-cairn-15.0.6/tutor_cairn.egg-info/top_level.txt
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.912021 tutor-cairn-15.0.6/tutorcairn/
--rw-rw-r--   0 regis     (1000) regis     (1000)       24 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/__about__.py
--rw-rw-r--   0 regis     (1000) regis     (1000)        0 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/__init__.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/patches/
--rw-rw-r--   0 regis     (1000) regis     (1000)        0 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/patches/.gitignore
--rw-rw-r--   0 regis     (1000) regis     (1000)       87 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/patches/caddyfile
--rw-rw-r--   0 regis     (1000) regis     (1000)     9124 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/patches/k8s-deployments
--rw-rw-r--   0 regis     (1000) regis     (1000)     3003 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/patches/k8s-jobs
--rw-rw-r--   0 regis     (1000) regis     (1000)      759 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/patches/k8s-services
--rw-rw-r--   0 regis     (1000) regis     (1000)      868 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/patches/k8s-volumes
--rw-rw-r--   0 regis     (1000) regis     (1000)      981 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/patches/kustomization-configmapgenerator
--rw-rw-r--   0 regis     (1000) regis     (1000)     1858 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/patches/local-docker-compose-jobs-services
--rw-rw-r--   0 regis     (1000) regis     (1000)     3256 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/patches/local-docker-compose-services
--rw-rw-r--   0 regis     (1000) regis     (1000)     4838 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/plugin.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.912021 tutor-cairn-15.0.6/tutorcairn/templates/
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.912021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/
--rw-rw-r--   0 regis     (1000) regis     (1000)        0 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/.gitignore
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/
--rw-rw-r--   0 regis     (1000) regis     (1000)      350 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/auth.json
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/
--rw-rw-r--   0 regis     (1000) regis     (1000)      734 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0001_create.sql
--rw-rw-r--   0 regis     (1000) regis     (1000)      430 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0002_grades.sql
--rw-rw-r--   0 regis     (1000) regis     (1000)     2121 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0003_course_enrollments.sql
--rw-rw-r--   0 regis     (1000) regis     (1000)     2250 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0004_video_views.sql
--rw-rw-r--   0 regis     (1000) regis     (1000)      343 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0005_course_blocks.sql
--rw-rw-r--   0 regis     (1000) regis     (1000)     1093 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0006_course_block_completion.sql
--rw-rw-r--   0 regis     (1000) regis     (1000)      985 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0007_fix_video_segments.sql
--rw-rw-r--   0 regis     (1000) regis     (1000)     1277 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0008_rename_openedx_tables.sql
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/users.d/
--rw-rw-r--   0 regis     (1000) regis     (1000)      269 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/users.d/cairn.xml
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.912021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/openedx/
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/openedx/scripts/
--rw-rw-r--   0 regis     (1000) regis     (1000)     3245 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/openedx/scripts/importcoursedata.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/superset/
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/superset/bootstrap/
--rw-rw-r--   0 regis     (1000) regis     (1000)   115036 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/superset/bootstrap/courseoverview.json
--rw-rw-r--   0 regis     (1000) regis     (1000)     4316 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/superset/superset_config.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/vector/
--rw-rw-r--   0 regis     (1000) regis     (1000)      405 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/vector/file.toml
--rw-rw-r--   0 regis     (1000) regis     (1000)      413 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/vector/k8s.toml
--rw-rw-r--   0 regis     (1000) regis     (1000)      367 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/vector/local.toml
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/vector/partials/
--rw-rw-r--   0 regis     (1000) regis     (1000)     1929 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/vector/partials/common-post.toml
--rw-rw-r--   0 regis     (1000) regis     (1000)      112 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/vector/partials/common-pre.toml
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/
--rw-rw-r--   0 regis     (1000) regis     (1000)        0 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/.gitignore
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/cairn-clickhouse/
--rw-rw-r--   0 regis     (1000) regis     (1000)      554 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/cairn-clickhouse/Dockerfile
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/cairn-clickhouse/scripts/
--rwxrwxr-x   0 regis     (1000) regis     (1000)     5017 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/cairn-clickhouse/scripts/cairn
--rwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/cairn-clickhouse/scripts/clickhouse-auth.json
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/cairn-superset/
--rw-rw-r--   0 regis     (1000) regis     (1000)     1209 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/cairn-superset/Dockerfile
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/cairn-superset/scripts/
--rw-rw-r--   0 regis     (1000) regis     (1000)     9638 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/cairn-superset/scripts/cairn
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/tasks/
--rw-rw-r--   0 regis     (1000) regis     (1000)        0 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/tasks/.gitignore
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/tasks/cairn-clickhouse/
--rw-rw-r--   0 regis     (1000) regis     (1000)       57 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/tasks/cairn-clickhouse/init
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/tasks/cairn-openedx/
--rw-rw-r--   0 regis     (1000) regis     (1000)       44 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/tasks/cairn-openedx/init
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/tasks/cairn-superset/
--rw-rw-r--   0 regis     (1000) regis     (1000)      390 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/tasks/cairn-superset/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.639647 tutor-cairn-16.0.0/
+-rw-r--r--   0 ci        (1000) ci        (1000)       80 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)    17285 2023-06-14 22:26:22.639647 tutor-cairn-16.0.0/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)    16470 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/pyproject.toml
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-06-14 22:26:22.642980 tutor-cairn-16.0.0/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     1631 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.626314 tutor-cairn-16.0.0/tutor_cairn.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)    17285 2023-06-14 22:26:22.000000 tutor-cairn-16.0.0/tutor_cairn.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     2802 2023-06-14 22:26:22.000000 tutor-cairn-16.0.0/tutor_cairn.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-06-14 22:26:22.000000 tutor-cairn-16.0.0/tutor_cairn.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       44 2023-06-14 22:26:22.000000 tutor-cairn-16.0.0/tutor_cairn.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-06-14 22:26:22.000000 tutor-cairn-16.0.0/tutor_cairn.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       11 2023-06-14 22:26:22.000000 tutor-cairn-16.0.0/tutor_cairn.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.629647 tutor-cairn-16.0.0/tutorcairn/
+-rw-r--r--   0 ci        (1000) ci        (1000)      176 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.632980 tutor-cairn-16.0.0/tutorcairn/patches/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/patches/.gitignore
+-rw-r--r--   0 ci        (1000) ci        (1000)       87 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/patches/caddyfile
+-rw-r--r--   0 ci        (1000) ci        (1000)     9135 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/patches/k8s-deployments
+-rw-r--r--   0 ci        (1000) ci        (1000)     3014 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/patches/k8s-jobs
+-rw-r--r--   0 ci        (1000) ci        (1000)      759 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/patches/k8s-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      868 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/patches/k8s-volumes
+-rw-r--r--   0 ci        (1000) ci        (1000)      981 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/patches/kustomization-configmapgenerator
+-rw-r--r--   0 ci        (1000) ci        (1000)      313 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/patches/local-docker-compose-dev-services
+-rw-r--r--   0 ci        (1000) ci        (1000)     1869 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      112 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/patches/local-docker-compose-permissions-command
+-rw-r--r--   0 ci        (1000) ci        (1000)      146 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/patches/local-docker-compose-permissions-volumes
+-rw-r--r--   0 ci        (1000) ci        (1000)     3157 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/patches/local-docker-compose-services
+-rw-r--r--   0 ci        (1000) ci        (1000)     5783 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/plugin.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.619647 tutor-cairn-16.0.0/tutorcairn/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.622980 tutor-cairn-16.0.0/tutorcairn/templates/cairn/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.632980 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/.gitignore
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.632980 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/
+-rw-r--r--   0 ci        (1000) ci        (1000)      350 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/auth.json
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.632980 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/
+-rw-r--r--   0 ci        (1000) ci        (1000)      734 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0001_create.sql
+-rw-r--r--   0 ci        (1000) ci        (1000)      430 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0002_grades.sql
+-rw-r--r--   0 ci        (1000) ci        (1000)     2121 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0003_course_enrollments.sql
+-rw-r--r--   0 ci        (1000) ci        (1000)     2250 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0004_video_views.sql
+-rw-r--r--   0 ci        (1000) ci        (1000)      343 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0005_course_blocks.sql
+-rw-r--r--   0 ci        (1000) ci        (1000)     1093 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0006_course_block_completion.sql
+-rw-r--r--   0 ci        (1000) ci        (1000)      985 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0007_fix_video_segments.sql
+-rw-r--r--   0 ci        (1000) ci        (1000)     1277 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0008_rename_openedx_tables.sql
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.632980 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/users.d/
+-rw-r--r--   0 ci        (1000) ci        (1000)      269 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/users.d/cairn.xml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.619647 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/openedx/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.636314 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/openedx/scripts/
+-rw-r--r--   0 ci        (1000) ci        (1000)     3245 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/openedx/scripts/importcoursedata.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.636314 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/superset/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.636314 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/superset/bootstrap/
+-rw-r--r--   0 ci        (1000) ci        (1000)   115036 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/superset/bootstrap/courseoverview.json
+-rw-r--r--   0 ci        (1000) ci        (1000)     5936 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/superset/superset_config.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.636314 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/vector/
+-rw-r--r--   0 ci        (1000) ci        (1000)      405 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/vector/file.toml
+-rw-r--r--   0 ci        (1000) ci        (1000)      413 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/vector/k8s.toml
+-rw-r--r--   0 ci        (1000) ci        (1000)      367 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/vector/local.toml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.636314 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/vector/partials/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1929 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/vector/partials/common-post.toml
+-rw-r--r--   0 ci        (1000) ci        (1000)      112 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/vector/partials/common-pre.toml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.636314 tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/.gitignore
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.639647 tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-clickhouse/
+-rw-r--r--   0 ci        (1000) ci        (1000)      554 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-clickhouse/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.639647 tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-clickhouse/scripts/
+-rwxr-xr-x   0 ci        (1000) ci        (1000)     3422 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-clickhouse/scripts/cairn
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.639647 tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-superset/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1342 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-superset/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.639647 tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-superset/cairn/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-superset/cairn/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     5499 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-superset/cairn/bootstrap.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     8407 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-superset/cairn/ctl.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     3299 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-superset/cairn/sso.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.639647 tutor-cairn-16.0.0/tutorcairn/templates/cairn/tasks/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/tasks/.gitignore
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.639647 tutor-cairn-16.0.0/tutorcairn/templates/cairn/tasks/cairn-clickhouse/
+-rw-r--r--   0 ci        (1000) ci        (1000)       57 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/tasks/cairn-clickhouse/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.639647 tutor-cairn-16.0.0/tutorcairn/templates/cairn/tasks/cairn-openedx/
+-rw-r--r--   0 ci        (1000) ci        (1000)      938 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/tasks/cairn-openedx/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.639647 tutor-cairn-16.0.0/tutorcairn/templates/cairn/tasks/cairn-superset/
+-rw-r--r--   0 ci        (1000) ci        (1000)      390 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/tasks/cairn-superset/init
```

### Comparing `tutor-cairn-15.0.6/PKG-INFO` & `tutor-cairn-16.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: tutor-cairn
-Version: 15.0.6
-Summary: cairn plugin for Tutor
+Version: 16.0.0
+Summary: Scalable, real-time analytics for Open edX
 Home-page: https://github.com/overhangio/tutor-cairn
 Author: Overhang.IO
 License: AGPLv3
 Project-URL: Code, https://github.com/overhangio/tutor-cairn
 Project-URL: Issue tracker, https://github.com/overhangio/tutor-cairn/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 
 Cairn: scalable, real-time analytics for Open edX
 ==================================================
 
 Analytics are an essential component of an online learning platform: you need to know whether your courses are effective and which parts need some improvement. You need to know if your students are falling by, and if they do, you need to detect the early warning signs. When your courses are successful, you want to get periodical engagement reports.
 
 We created a tool to help you answer all these questions. Cairn is a Tutor plugin that you install on top of an Open edX platform and that gives you access to a powerful, full-blown analytics stack. Cairn comes with the following features out of the box:
 
-🖴 **Unified datalake of learner events and stateful data**: both learner-triggered events, coming from the Open edX tracking logs, and stateful data, coming from the existing databases, are available for querying in a single unified interface. This means that you can, for instance, query the grades of the students that visited your platform in the past 24 hours, or collect the email addresses of the students who did not yet complete the latest assignment.
+❄️ **Unified data lake of learner events and stateful data**: both learner-triggered events, coming from the Open edX tracking logs, and stateful data, coming from the existing databases, are available for querying in a single unified interface. This means that you can, for instance, query the grades of the students that visited your platform in the past 24 hours, or collect the email addresses of the students who did not yet complete the latest assignment.
 
 ⚡﻿ **Real-time:** new events are visible immediately in your analytics interface. No more waiting for slow batch jobs to complete!
 
 🔑 **Course- and org-based data access rights:** your course staff is granted access only to the data rows that concern them. Cairn makes it easy to create new users with granular access permissions.
 
 🎁 **Working dashboards out of the box:** Cairn comes with a fully functional dashboard that you can start playing with right away.
 
@@ -60,57 +59,48 @@
 - On the server side, tracking logs are collected by `Vector <https://vector.dev/>`__, an efficient, cloud-native log collector.
 - Tracking log events are then stored in a `Clickhouse <https://clickhouse.tech/>`__ table, which is the cornerstone of Cairn. Clickhouse also exposes MySQL data via live and materialized views. This is the magic piece of the puzzle which allows us to join event and MySQL data.
 - The data inside Clickhouse is made visible to the end-users in a `Superset <https://superset.apache.org/>`__ frontend.
 
 Installation
 ------------
 
-Cairn requires a `Tutor Wizard Edition license <https://overhang.io/tutor/wizardedition>`__. Once you have enabled your license, installing the plugin is as simple as running::
+Cairn used to be a commercial plugin, but is now available for free to all Tutor users. Install the plugin with::
 
-    tutor license install tutor-cairn
+    tutor plugins install cairn
 
 Usage
 -----
 
 Getting started
 ~~~~~~~~~~~~~~~
 
 Enable the plugin with::
 
     tutor plugins enable cairn
 
 Then, restart your platform and run the initialization scripts::
 
-    tutor local quickstart
+    tutor local launch
 
-Create a user to access both in the Clickhouse database and the Superset frontend::
-
-    tutor local do cairn-createuser YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
-
-You can use the ``--password=<PASSWORD>`` option to provide a password on the command line.
-
-To make this user an administrator, add the ``--admin`` option::
+Open http(s)://data.<YOUR_LMS_HOST> in your browser. When running locally, this will be http://data.local.overhang.io. (http://data.local.overhang.io:2247 in development). Users authenticate with their LMS user. By default, they have access to the data generated by the courses in which they have the "staff role". To convert an existing user to administrator status, run::
 
     tutor local do cairn-createuser --admin YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
 
-To add the default dashboards to the new user, add the ``--bootstrap-dashboards`` option::
-
-    tutor local do cairn-createuser --bootstrap-dashboards YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
-
-You can then access the frontend with the user credentials you just created. Open http(s)://data.<YOUR_LMS_HOST> in your browser. When running locally, this will be http://data.local.overhang.io. The admin user will automatically be granted access to the "openedx" database in Superset and will be able to query all tables.
-
 Some event data might be missing from your dashboards: just start using your LMS and refresh your dashboard. The new events should appear immediately.
 
-.. image:: https://overhang.io/static/catalog/img/cairn/courseoverview-01.png
+.. image:: https://raw.githubusercontent.com/overhangio/tutor-cairn/master/screenshots/courseoverview-01.png
     :alt: Course overview dashboard part 1
-.. image:: https://overhang.io/static/catalog/img/cairn/courseoverview-02.png
+.. image:: https://raw.githubusercontent.com/overhangio/tutor-cairn/master/screenshots/courseoverview-02.png
     :alt: Course overview dashboard part 2
-.. image:: https://overhang.io/static/catalog/img/cairn/courseoverview-03.png
+.. image:: https://raw.githubusercontent.com/overhangio/tutor-cairn/master/screenshots/courseoverview-03.png
     :alt: Course overview dashboard part 3
 
+⚠️ WARNING ⚠️ Previous versions of Cairn required manual user management. If you have an existing installation of Cairn, this behaviour will change when you upgrade to v16. To revert to the previous behaviour, see `"manual user management" <#manual-user-management>`__ below.
+
+
 Available metrics
 ~~~~~~~~~~~~~~~~~
 
 Cairn allows you to collect and view just any metric from your Open edX platform, as long as the data is available from the tracking logs or the MySQL database. Out of the box, the default Cairn dashboard comes with visualizations for the following metrics:
 
 - Weekly course engagement:
     - Number of enrolled learners
@@ -126,46 +116,59 @@
     - Level of education distribution
 - Video engagement:
     - Number of unique viewers
     - Average watch time
     - Total watch time
     - Second-per-second statistics: Number of unique viewers, Total number of views
 
+.. _manual_user_management:
 
-Data-based access control
-~~~~~~~~~~~~~~~~~~~~~~~~~
+Manual user management
+~~~~~~~~~~~~~~~~~~~~~~
 
-Most of your users should probably not have access to all data from all courses. To restrict a given user to one or more courses or organizations, select the course IDs and/or organization IDS to which the user should have access and create a user with limited access to the datalake::
+By default, authentication uses single sign-on (SSO) with the LMS such that users do not have to create separate accounts in Superset. In previous versions of Cairn (v15 and earlier), user accounts had to be created manually. To restore this behaviour, modify the ``CAIRN_ENABLE_SSO`` setting::
 
-    tutor local run cairn-clickhouse cairn createuser --course-id='course-v1:edX+DemoX+Demo_Course' --org-id='edX' YOURUSERNAME
+    tutor config save --set CAIRN_ENABLE_SSO=false
+    tutor local restart
 
-Then, create the corresponding user on the frontend with the same command as above (but without the ``--admin`` option)::
+SSO will then disabled, and only manually created users will be able to login. To create a user, run::
 
-    tutor local run cairn-superset cairn createuser YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
+    tutor local do cairn-createuser --password=yourpassword YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
+
+To make this user an administrator, add the ``--admin`` option::
+
+    tutor local do cairn-createuser --admin YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
+
+To add the default dashboards to the new user, add the ``--bootstrap-dashboards`` option::
+
+    tutor local do cairn-createuser --bootstrap-dashboards YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
+
+ To restrict a given user to one or more courses or organizations, select the course IDs and/or organization IDS to which the user should have access::
+
+    tutor local do cairn-createuser --course-id='course-v1:edX+DemoX+Demo_Course' YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
 
-Your frontend user will automatically be associated to the datalake database you created.
 
 Refreshing course block data
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Course block IDs and names are loaded from the Open edX modulestore into the datalake. After making changes to your course, you might want to refresh the course structure stored in the datalake. To do so, run::
 
-    tutor local init --limit=cairn
+    tutor local do init --limit=cairn
 
 Or, if you want to avoid running the full plugin initialization::
 
     tutor local run \
         -v $(tutor config printroot)/env/plugins/cairn/apps/openedx/scripts/:/openedx/scripts \
         -v $(tutor config printroot)/env/plugins/cairn/apps/clickhouse/auth.json:/openedx/clickhouse-auth.json \
         lms python /openedx/scripts/importcoursedata.py
 
 Running on Kubernetes
 ~~~~~~~~~~~~~~~~~~~~~
 
-When running on Kubernetes instead of locally, most commands above can be re-written with `tutor k8s exec service "command"` instead of `tutor local run service command`. For instance::
+When running on Kubernetes instead of locally, most commands above can be re-written with ``tutor k8s exec service "command"`` instead of ``tutor local run service command``. For instance::
 
     # Privileged user creation
     tutor k8s exec cairn-superset "superset fab create-admin --username YOURUSERNAME --email user@example.com"
     # Unprivileged user creation
     tutor k8s exec cairn-clickhouse "cairn createuser --course-id='course-v1:edX+DemoX+Demo_Course' --org-id='edX' YOURUSERNAME"
     tutor k8s exec cairn-superset "cairn createuser YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM"
 
@@ -183,27 +186,29 @@
 The latter command will parse tracking log events from the ``$(tutor config printroot)/data/lms/logs/tracking.log`` file that contains all the tracking logs since the creation of your platform. The command will take a while to run if you have a large platform that has been running for a long time. It can be interrupted at any time and started again, as the log collector keeps track of its position within the tracking log file.
 
 Adding data to your data lake
 -----------------------------
 
 Tables created in Clickhouse are managed by a lightweight migration system. You can view existing migrations that ship by default with Cairn in the following folder: ``$VIRTUAL_ENV/lib/python3.8/site-packages/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/``.
 
-You are free to create your own migrations that will automatically be created in Clickhouse every time the ``tutor local quickstart`` or ``tutor local init`` commands are run. To do so, as usual in Tutor, you should create a `Tutor plugin <https://docs.tutor.overhang.io/plugins.html>`__. This plugin should include the ``CAIRN_MIGRATIONS_FOLDER`` configuration. This setting should point to a template folder, inside the plugin, where migration templates are defined. For instance, assuming you created the "customcairn" plugin::
+You are free to create your own migrations that will automatically be created in Clickhouse every time the ``tutor local launch`` or ``tutor local do init`` commands are run. To do so, as usual in Tutor, you should create a `Tutor plugin <https://docs.tutor.overhang.io/plugins.html>`__. This plugin should include the ``CAIRN_MIGRATIONS_FOLDER`` configuration. This setting should point to a template folder, inside the plugin, where migration templates are defined. For instance, assuming you created the "customcairn" plugin::
 
     config = {
         "defaults": {
             "CAIRN_MIGRATIONS_FOLDER": "customcairn/apps/migrations.d"
         }
     }
 
-In this example, the following folder should be created in the plugin:: ``tutorcustomcairn/templates/customcairn/apps/migrations.d/``. Then, you should add your migration files there. Migrations will be applied in alphabetical order whenever you run ``tutor local quickstart`` or ``tutor local init``.
+In this example, the following folder should be created in the plugin:: ``tutorcustomcairn/templates/customcairn/apps/migrations.d/``. Then, you should add your migration files there. Migrations will be applied in alphabetical order whenever you run ``tutor local launch`` or ``tutor local do init``.
 
 Development
 -----------
 
+In development, the Superset user interface will be available at http://data.local.overhang.io:2247.
+
 To reload Vector configuration after changes to vector.toml, run::
 
     tutor config save && tutor local exec cairn-vector sh -c "kill -s HUP 1"
 
 To explore the clickhouse database as root, run::
 
     tutor local run cairn-clickhouse cairn client
@@ -217,15 +222,15 @@
 
 Cairn is configured by several Tutor settings. Each one of these settings may be modified individually by running::
 
     tutor config save --set SETTING_NAME=settingvalue
 
 Then apply changes with::
 
-    tutor local quickstart
+    tutor local launch
 
 General settings
 ~~~~~~~~~~~~~~~~
 
 - ``CAIRN_HOST`` (default: ``"data.{{ LMS_HOST }}"``): hostname at which the Cairn frontend (i.e: Superset) will be accessible. By default, this is the "data" subdomain of the LMS. Thus, if your students access the LMS at https://learn.mydomain.com then Cairn will be accessible at https://data.learn.mydomain.com.
 - ``CAIRN_DOCKER_HOST_SOCK_PATH`` (default: ``"/var/run/docker.sock"``): path to the Docker host socket on the host. This is required to collect logs from Docker when running locally, but it is not used when running on Kubernetes.
 
@@ -249,22 +254,19 @@
 - ``CAIRN_SUPERSET_LANGUAGE_CODE`` (default: ``"{{ LANGUAGE_CODE[:2] }}"``): 2-letter code of the default language for the Superset frontend. View the list of all supported languages `here <https://github.com/apache/superset/blob/dc575080d7e43d40b1734bb8f44fdc291cb95b11/superset/config.py#L324>`__. When different than "en", users will have the opportunity to switch from English to this language via a flag icon in the top-right corner.
 - ``CAIRN_SUPERSET_DOCKER_IMAGE`` (default: ``"{{ DOCKER_REGISTRY }}overhangio/cairn-superset:{{ CAIRN_VERSION }}"``): name of the Docker image that runs Postgresql.
 - ``CAIRN_POSTGRESQL_DATABASE`` (default: ``"superset"``): name of the Postgresql database.
 - ``CAIRN_POSTGRESQL_USERNAME`` (default: ``"superset"``): Postgresql username.
 - ``CAIRN_POSTGRESQL_PASSWORD`` (default: ``"{{ 20|random_string }}"``): Postgresql password.
 - ``CAIRN_SUPERSET_SECRET_KEY`` (default: ``"{{ 20|random_string }}"``): randomly-generated secret key for the Superset frontend.
 
+Troubleshooting
+---------------
 
-Support
--------
-
-Are you having trouble with Cairn? Do you have questions about this plugin? Please get in touch with us at contact@overhang.io. Community support is also available on the official Tutor forums: https://discuss.overhang.io
+This Tutor plugin is maintained by Régis Behmo from `Overhang.IO <https://overhang.io>`__. Community support is available from the official `Open edX forum <https://discuss.openedx.org>`__. Do you need help with this plugin? See the `troubleshooting <https://docs.tutor.overhang.io/troubleshooting.html>`__ section from the Tutor documentation.
 
 License
 -------
 
 This software is licensed under the terms of the AGPLv3.
 
 .. image:: https://overhang.io/static/catalog/img/cairn.png
     :alt: Alpine cairn
-
-
```

### Comparing `tutor-cairn-15.0.6/README.rst` & `tutor-cairn-16.0.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Cairn: scalable, real-time analytics for Open edX
 ==================================================
 
 Analytics are an essential component of an online learning platform: you need to know whether your courses are effective and which parts need some improvement. You need to know if your students are falling by, and if they do, you need to detect the early warning signs. When your courses are successful, you want to get periodical engagement reports.
 
 We created a tool to help you answer all these questions. Cairn is a Tutor plugin that you install on top of an Open edX platform and that gives you access to a powerful, full-blown analytics stack. Cairn comes with the following features out of the box:
 
-🖴 **Unified datalake of learner events and stateful data**: both learner-triggered events, coming from the Open edX tracking logs, and stateful data, coming from the existing databases, are available for querying in a single unified interface. This means that you can, for instance, query the grades of the students that visited your platform in the past 24 hours, or collect the email addresses of the students who did not yet complete the latest assignment.
+❄️ **Unified data lake of learner events and stateful data**: both learner-triggered events, coming from the Open edX tracking logs, and stateful data, coming from the existing databases, are available for querying in a single unified interface. This means that you can, for instance, query the grades of the students that visited your platform in the past 24 hours, or collect the email addresses of the students who did not yet complete the latest assignment.
 
 ⚡﻿ **Real-time:** new events are visible immediately in your analytics interface. No more waiting for slow batch jobs to complete!
 
 🔑 **Course- and org-based data access rights:** your course staff is granted access only to the data rows that concern them. Cairn makes it easy to create new users with granular access permissions.
 
 🎁 **Working dashboards out of the box:** Cairn comes with a fully functional dashboard that you can start playing with right away.
 
@@ -39,57 +39,48 @@
 - On the server side, tracking logs are collected by `Vector <https://vector.dev/>`__, an efficient, cloud-native log collector.
 - Tracking log events are then stored in a `Clickhouse <https://clickhouse.tech/>`__ table, which is the cornerstone of Cairn. Clickhouse also exposes MySQL data via live and materialized views. This is the magic piece of the puzzle which allows us to join event and MySQL data.
 - The data inside Clickhouse is made visible to the end-users in a `Superset <https://superset.apache.org/>`__ frontend.
 
 Installation
 ------------
 
-Cairn requires a `Tutor Wizard Edition license <https://overhang.io/tutor/wizardedition>`__. Once you have enabled your license, installing the plugin is as simple as running::
+Cairn used to be a commercial plugin, but is now available for free to all Tutor users. Install the plugin with::
 
-    tutor license install tutor-cairn
+    tutor plugins install cairn
 
 Usage
 -----
 
 Getting started
 ~~~~~~~~~~~~~~~
 
 Enable the plugin with::
 
     tutor plugins enable cairn
 
 Then, restart your platform and run the initialization scripts::
 
-    tutor local quickstart
+    tutor local launch
 
-Create a user to access both in the Clickhouse database and the Superset frontend::
-
-    tutor local do cairn-createuser YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
-
-You can use the ``--password=<PASSWORD>`` option to provide a password on the command line.
-
-To make this user an administrator, add the ``--admin`` option::
+Open http(s)://data.<YOUR_LMS_HOST> in your browser. When running locally, this will be http://data.local.overhang.io. (http://data.local.overhang.io:2247 in development). Users authenticate with their LMS user. By default, they have access to the data generated by the courses in which they have the "staff role". To convert an existing user to administrator status, run::
 
     tutor local do cairn-createuser --admin YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
 
-To add the default dashboards to the new user, add the ``--bootstrap-dashboards`` option::
-
-    tutor local do cairn-createuser --bootstrap-dashboards YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
-
-You can then access the frontend with the user credentials you just created. Open http(s)://data.<YOUR_LMS_HOST> in your browser. When running locally, this will be http://data.local.overhang.io. The admin user will automatically be granted access to the "openedx" database in Superset and will be able to query all tables.
-
 Some event data might be missing from your dashboards: just start using your LMS and refresh your dashboard. The new events should appear immediately.
 
-.. image:: https://overhang.io/static/catalog/img/cairn/courseoverview-01.png
+.. image:: https://raw.githubusercontent.com/overhangio/tutor-cairn/master/screenshots/courseoverview-01.png
     :alt: Course overview dashboard part 1
-.. image:: https://overhang.io/static/catalog/img/cairn/courseoverview-02.png
+.. image:: https://raw.githubusercontent.com/overhangio/tutor-cairn/master/screenshots/courseoverview-02.png
     :alt: Course overview dashboard part 2
-.. image:: https://overhang.io/static/catalog/img/cairn/courseoverview-03.png
+.. image:: https://raw.githubusercontent.com/overhangio/tutor-cairn/master/screenshots/courseoverview-03.png
     :alt: Course overview dashboard part 3
 
+⚠️ WARNING ⚠️ Previous versions of Cairn required manual user management. If you have an existing installation of Cairn, this behaviour will change when you upgrade to v16. To revert to the previous behaviour, see `"manual user management" <#manual-user-management>`__ below.
+
+
 Available metrics
 ~~~~~~~~~~~~~~~~~
 
 Cairn allows you to collect and view just any metric from your Open edX platform, as long as the data is available from the tracking logs or the MySQL database. Out of the box, the default Cairn dashboard comes with visualizations for the following metrics:
 
 - Weekly course engagement:
     - Number of enrolled learners
@@ -105,46 +96,59 @@
     - Level of education distribution
 - Video engagement:
     - Number of unique viewers
     - Average watch time
     - Total watch time
     - Second-per-second statistics: Number of unique viewers, Total number of views
 
+.. _manual_user_management:
 
-Data-based access control
-~~~~~~~~~~~~~~~~~~~~~~~~~
+Manual user management
+~~~~~~~~~~~~~~~~~~~~~~
 
-Most of your users should probably not have access to all data from all courses. To restrict a given user to one or more courses or organizations, select the course IDs and/or organization IDS to which the user should have access and create a user with limited access to the datalake::
+By default, authentication uses single sign-on (SSO) with the LMS such that users do not have to create separate accounts in Superset. In previous versions of Cairn (v15 and earlier), user accounts had to be created manually. To restore this behaviour, modify the ``CAIRN_ENABLE_SSO`` setting::
 
-    tutor local run cairn-clickhouse cairn createuser --course-id='course-v1:edX+DemoX+Demo_Course' --org-id='edX' YOURUSERNAME
+    tutor config save --set CAIRN_ENABLE_SSO=false
+    tutor local restart
 
-Then, create the corresponding user on the frontend with the same command as above (but without the ``--admin`` option)::
+SSO will then disabled, and only manually created users will be able to login. To create a user, run::
 
-    tutor local run cairn-superset cairn createuser YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
+    tutor local do cairn-createuser --password=yourpassword YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
+
+To make this user an administrator, add the ``--admin`` option::
+
+    tutor local do cairn-createuser --admin YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
+
+To add the default dashboards to the new user, add the ``--bootstrap-dashboards`` option::
+
+    tutor local do cairn-createuser --bootstrap-dashboards YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
+
+ To restrict a given user to one or more courses or organizations, select the course IDs and/or organization IDS to which the user should have access::
+
+    tutor local do cairn-createuser --course-id='course-v1:edX+DemoX+Demo_Course' YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
 
-Your frontend user will automatically be associated to the datalake database you created.
 
 Refreshing course block data
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Course block IDs and names are loaded from the Open edX modulestore into the datalake. After making changes to your course, you might want to refresh the course structure stored in the datalake. To do so, run::
 
-    tutor local init --limit=cairn
+    tutor local do init --limit=cairn
 
 Or, if you want to avoid running the full plugin initialization::
 
     tutor local run \
         -v $(tutor config printroot)/env/plugins/cairn/apps/openedx/scripts/:/openedx/scripts \
         -v $(tutor config printroot)/env/plugins/cairn/apps/clickhouse/auth.json:/openedx/clickhouse-auth.json \
         lms python /openedx/scripts/importcoursedata.py
 
 Running on Kubernetes
 ~~~~~~~~~~~~~~~~~~~~~
 
-When running on Kubernetes instead of locally, most commands above can be re-written with `tutor k8s exec service "command"` instead of `tutor local run service command`. For instance::
+When running on Kubernetes instead of locally, most commands above can be re-written with ``tutor k8s exec service "command"`` instead of ``tutor local run service command``. For instance::
 
     # Privileged user creation
     tutor k8s exec cairn-superset "superset fab create-admin --username YOURUSERNAME --email user@example.com"
     # Unprivileged user creation
     tutor k8s exec cairn-clickhouse "cairn createuser --course-id='course-v1:edX+DemoX+Demo_Course' --org-id='edX' YOURUSERNAME"
     tutor k8s exec cairn-superset "cairn createuser YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM"
 
@@ -162,27 +166,29 @@
 The latter command will parse tracking log events from the ``$(tutor config printroot)/data/lms/logs/tracking.log`` file that contains all the tracking logs since the creation of your platform. The command will take a while to run if you have a large platform that has been running for a long time. It can be interrupted at any time and started again, as the log collector keeps track of its position within the tracking log file.
 
 Adding data to your data lake
 -----------------------------
 
 Tables created in Clickhouse are managed by a lightweight migration system. You can view existing migrations that ship by default with Cairn in the following folder: ``$VIRTUAL_ENV/lib/python3.8/site-packages/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/``.
 
-You are free to create your own migrations that will automatically be created in Clickhouse every time the ``tutor local quickstart`` or ``tutor local init`` commands are run. To do so, as usual in Tutor, you should create a `Tutor plugin <https://docs.tutor.overhang.io/plugins.html>`__. This plugin should include the ``CAIRN_MIGRATIONS_FOLDER`` configuration. This setting should point to a template folder, inside the plugin, where migration templates are defined. For instance, assuming you created the "customcairn" plugin::
+You are free to create your own migrations that will automatically be created in Clickhouse every time the ``tutor local launch`` or ``tutor local do init`` commands are run. To do so, as usual in Tutor, you should create a `Tutor plugin <https://docs.tutor.overhang.io/plugins.html>`__. This plugin should include the ``CAIRN_MIGRATIONS_FOLDER`` configuration. This setting should point to a template folder, inside the plugin, where migration templates are defined. For instance, assuming you created the "customcairn" plugin::
 
     config = {
         "defaults": {
             "CAIRN_MIGRATIONS_FOLDER": "customcairn/apps/migrations.d"
         }
     }
 
-In this example, the following folder should be created in the plugin:: ``tutorcustomcairn/templates/customcairn/apps/migrations.d/``. Then, you should add your migration files there. Migrations will be applied in alphabetical order whenever you run ``tutor local quickstart`` or ``tutor local init``.
+In this example, the following folder should be created in the plugin:: ``tutorcustomcairn/templates/customcairn/apps/migrations.d/``. Then, you should add your migration files there. Migrations will be applied in alphabetical order whenever you run ``tutor local launch`` or ``tutor local do init``.
 
 Development
 -----------
 
+In development, the Superset user interface will be available at http://data.local.overhang.io:2247.
+
 To reload Vector configuration after changes to vector.toml, run::
 
     tutor config save && tutor local exec cairn-vector sh -c "kill -s HUP 1"
 
 To explore the clickhouse database as root, run::
 
     tutor local run cairn-clickhouse cairn client
@@ -196,15 +202,15 @@
 
 Cairn is configured by several Tutor settings. Each one of these settings may be modified individually by running::
 
     tutor config save --set SETTING_NAME=settingvalue
 
 Then apply changes with::
 
-    tutor local quickstart
+    tutor local launch
 
 General settings
 ~~~~~~~~~~~~~~~~
 
 - ``CAIRN_HOST`` (default: ``"data.{{ LMS_HOST }}"``): hostname at which the Cairn frontend (i.e: Superset) will be accessible. By default, this is the "data" subdomain of the LMS. Thus, if your students access the LMS at https://learn.mydomain.com then Cairn will be accessible at https://data.learn.mydomain.com.
 - ``CAIRN_DOCKER_HOST_SOCK_PATH`` (default: ``"/var/run/docker.sock"``): path to the Docker host socket on the host. This is required to collect logs from Docker when running locally, but it is not used when running on Kubernetes.
 
@@ -228,19 +234,18 @@
 - ``CAIRN_SUPERSET_LANGUAGE_CODE`` (default: ``"{{ LANGUAGE_CODE[:2] }}"``): 2-letter code of the default language for the Superset frontend. View the list of all supported languages `here <https://github.com/apache/superset/blob/dc575080d7e43d40b1734bb8f44fdc291cb95b11/superset/config.py#L324>`__. When different than "en", users will have the opportunity to switch from English to this language via a flag icon in the top-right corner.
 - ``CAIRN_SUPERSET_DOCKER_IMAGE`` (default: ``"{{ DOCKER_REGISTRY }}overhangio/cairn-superset:{{ CAIRN_VERSION }}"``): name of the Docker image that runs Postgresql.
 - ``CAIRN_POSTGRESQL_DATABASE`` (default: ``"superset"``): name of the Postgresql database.
 - ``CAIRN_POSTGRESQL_USERNAME`` (default: ``"superset"``): Postgresql username.
 - ``CAIRN_POSTGRESQL_PASSWORD`` (default: ``"{{ 20|random_string }}"``): Postgresql password.
 - ``CAIRN_SUPERSET_SECRET_KEY`` (default: ``"{{ 20|random_string }}"``): randomly-generated secret key for the Superset frontend.
 
+Troubleshooting
+---------------
 
-Support
--------
-
-Are you having trouble with Cairn? Do you have questions about this plugin? Please get in touch with us at contact@overhang.io. Community support is also available on the official Tutor forums: https://discuss.overhang.io
+This Tutor plugin is maintained by Régis Behmo from `Overhang.IO <https://overhang.io>`__. Community support is available from the official `Open edX forum <https://discuss.openedx.org>`__. Do you need help with this plugin? See the `troubleshooting <https://docs.tutor.overhang.io/troubleshooting.html>`__ section from the Tutor documentation.
 
 License
 -------
 
 This software is licensed under the terms of the AGPLv3.
 
 .. image:: https://overhang.io/static/catalog/img/cairn.png
```

### Comparing `tutor-cairn-15.0.6/setup.py` & `tutor-cairn-16.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,26 +30,26 @@
     url="https://github.com/overhangio/tutor-cairn",
     project_urls={
         "Code": "https://github.com/overhangio/tutor-cairn",
         "Issue tracker": "https://github.com/overhangio/tutor-cairn/issues",
     },
     license="AGPLv3",
     author="Overhang.IO",
-    description="cairn plugin for Tutor",
+    description="Scalable, real-time analytics for Open edX",
     long_description=load_readme(),
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
     python_requires=">=3.7",
-    install_requires=["tutor>=15.0.0,<16.0.0"],
+    install_requires=["tutor>=16.0.0,<17.0.0"],
     entry_points={"tutor.plugin.v1": ["cairn = tutorcairn.plugin"]},
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `tutor-cairn-15.0.6/tutor_cairn.egg-info/PKG-INFO` & `tutor-cairn-16.0.0/tutor_cairn.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: tutor-cairn
-Version: 15.0.6
-Summary: cairn plugin for Tutor
+Version: 16.0.0
+Summary: Scalable, real-time analytics for Open edX
 Home-page: https://github.com/overhangio/tutor-cairn
 Author: Overhang.IO
 License: AGPLv3
 Project-URL: Code, https://github.com/overhangio/tutor-cairn
 Project-URL: Issue tracker, https://github.com/overhangio/tutor-cairn/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 
 Cairn: scalable, real-time analytics for Open edX
 ==================================================
 
 Analytics are an essential component of an online learning platform: you need to know whether your courses are effective and which parts need some improvement. You need to know if your students are falling by, and if they do, you need to detect the early warning signs. When your courses are successful, you want to get periodical engagement reports.
 
 We created a tool to help you answer all these questions. Cairn is a Tutor plugin that you install on top of an Open edX platform and that gives you access to a powerful, full-blown analytics stack. Cairn comes with the following features out of the box:
 
-🖴 **Unified datalake of learner events and stateful data**: both learner-triggered events, coming from the Open edX tracking logs, and stateful data, coming from the existing databases, are available for querying in a single unified interface. This means that you can, for instance, query the grades of the students that visited your platform in the past 24 hours, or collect the email addresses of the students who did not yet complete the latest assignment.
+❄️ **Unified data lake of learner events and stateful data**: both learner-triggered events, coming from the Open edX tracking logs, and stateful data, coming from the existing databases, are available for querying in a single unified interface. This means that you can, for instance, query the grades of the students that visited your platform in the past 24 hours, or collect the email addresses of the students who did not yet complete the latest assignment.
 
 ⚡﻿ **Real-time:** new events are visible immediately in your analytics interface. No more waiting for slow batch jobs to complete!
 
 🔑 **Course- and org-based data access rights:** your course staff is granted access only to the data rows that concern them. Cairn makes it easy to create new users with granular access permissions.
 
 🎁 **Working dashboards out of the box:** Cairn comes with a fully functional dashboard that you can start playing with right away.
 
@@ -60,57 +59,48 @@
 - On the server side, tracking logs are collected by `Vector <https://vector.dev/>`__, an efficient, cloud-native log collector.
 - Tracking log events are then stored in a `Clickhouse <https://clickhouse.tech/>`__ table, which is the cornerstone of Cairn. Clickhouse also exposes MySQL data via live and materialized views. This is the magic piece of the puzzle which allows us to join event and MySQL data.
 - The data inside Clickhouse is made visible to the end-users in a `Superset <https://superset.apache.org/>`__ frontend.
 
 Installation
 ------------
 
-Cairn requires a `Tutor Wizard Edition license <https://overhang.io/tutor/wizardedition>`__. Once you have enabled your license, installing the plugin is as simple as running::
+Cairn used to be a commercial plugin, but is now available for free to all Tutor users. Install the plugin with::
 
-    tutor license install tutor-cairn
+    tutor plugins install cairn
 
 Usage
 -----
 
 Getting started
 ~~~~~~~~~~~~~~~
 
 Enable the plugin with::
 
     tutor plugins enable cairn
 
 Then, restart your platform and run the initialization scripts::
 
-    tutor local quickstart
+    tutor local launch
 
-Create a user to access both in the Clickhouse database and the Superset frontend::
-
-    tutor local do cairn-createuser YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
-
-You can use the ``--password=<PASSWORD>`` option to provide a password on the command line.
-
-To make this user an administrator, add the ``--admin`` option::
+Open http(s)://data.<YOUR_LMS_HOST> in your browser. When running locally, this will be http://data.local.overhang.io. (http://data.local.overhang.io:2247 in development). Users authenticate with their LMS user. By default, they have access to the data generated by the courses in which they have the "staff role". To convert an existing user to administrator status, run::
 
     tutor local do cairn-createuser --admin YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
 
-To add the default dashboards to the new user, add the ``--bootstrap-dashboards`` option::
-
-    tutor local do cairn-createuser --bootstrap-dashboards YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
-
-You can then access the frontend with the user credentials you just created. Open http(s)://data.<YOUR_LMS_HOST> in your browser. When running locally, this will be http://data.local.overhang.io. The admin user will automatically be granted access to the "openedx" database in Superset and will be able to query all tables.
-
 Some event data might be missing from your dashboards: just start using your LMS and refresh your dashboard. The new events should appear immediately.
 
-.. image:: https://overhang.io/static/catalog/img/cairn/courseoverview-01.png
+.. image:: https://raw.githubusercontent.com/overhangio/tutor-cairn/master/screenshots/courseoverview-01.png
     :alt: Course overview dashboard part 1
-.. image:: https://overhang.io/static/catalog/img/cairn/courseoverview-02.png
+.. image:: https://raw.githubusercontent.com/overhangio/tutor-cairn/master/screenshots/courseoverview-02.png
     :alt: Course overview dashboard part 2
-.. image:: https://overhang.io/static/catalog/img/cairn/courseoverview-03.png
+.. image:: https://raw.githubusercontent.com/overhangio/tutor-cairn/master/screenshots/courseoverview-03.png
     :alt: Course overview dashboard part 3
 
+⚠️ WARNING ⚠️ Previous versions of Cairn required manual user management. If you have an existing installation of Cairn, this behaviour will change when you upgrade to v16. To revert to the previous behaviour, see `"manual user management" <#manual-user-management>`__ below.
+
+
 Available metrics
 ~~~~~~~~~~~~~~~~~
 
 Cairn allows you to collect and view just any metric from your Open edX platform, as long as the data is available from the tracking logs or the MySQL database. Out of the box, the default Cairn dashboard comes with visualizations for the following metrics:
 
 - Weekly course engagement:
     - Number of enrolled learners
@@ -126,46 +116,59 @@
     - Level of education distribution
 - Video engagement:
     - Number of unique viewers
     - Average watch time
     - Total watch time
     - Second-per-second statistics: Number of unique viewers, Total number of views
 
+.. _manual_user_management:
 
-Data-based access control
-~~~~~~~~~~~~~~~~~~~~~~~~~
+Manual user management
+~~~~~~~~~~~~~~~~~~~~~~
 
-Most of your users should probably not have access to all data from all courses. To restrict a given user to one or more courses or organizations, select the course IDs and/or organization IDS to which the user should have access and create a user with limited access to the datalake::
+By default, authentication uses single sign-on (SSO) with the LMS such that users do not have to create separate accounts in Superset. In previous versions of Cairn (v15 and earlier), user accounts had to be created manually. To restore this behaviour, modify the ``CAIRN_ENABLE_SSO`` setting::
 
-    tutor local run cairn-clickhouse cairn createuser --course-id='course-v1:edX+DemoX+Demo_Course' --org-id='edX' YOURUSERNAME
+    tutor config save --set CAIRN_ENABLE_SSO=false
+    tutor local restart
 
-Then, create the corresponding user on the frontend with the same command as above (but without the ``--admin`` option)::
+SSO will then disabled, and only manually created users will be able to login. To create a user, run::
 
-    tutor local run cairn-superset cairn createuser YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
+    tutor local do cairn-createuser --password=yourpassword YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
+
+To make this user an administrator, add the ``--admin`` option::
+
+    tutor local do cairn-createuser --admin YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
+
+To add the default dashboards to the new user, add the ``--bootstrap-dashboards`` option::
+
+    tutor local do cairn-createuser --bootstrap-dashboards YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
+
+ To restrict a given user to one or more courses or organizations, select the course IDs and/or organization IDS to which the user should have access::
+
+    tutor local do cairn-createuser --course-id='course-v1:edX+DemoX+Demo_Course' YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
 
-Your frontend user will automatically be associated to the datalake database you created.
 
 Refreshing course block data
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Course block IDs and names are loaded from the Open edX modulestore into the datalake. After making changes to your course, you might want to refresh the course structure stored in the datalake. To do so, run::
 
-    tutor local init --limit=cairn
+    tutor local do init --limit=cairn
 
 Or, if you want to avoid running the full plugin initialization::
 
     tutor local run \
         -v $(tutor config printroot)/env/plugins/cairn/apps/openedx/scripts/:/openedx/scripts \
         -v $(tutor config printroot)/env/plugins/cairn/apps/clickhouse/auth.json:/openedx/clickhouse-auth.json \
         lms python /openedx/scripts/importcoursedata.py
 
 Running on Kubernetes
 ~~~~~~~~~~~~~~~~~~~~~
 
-When running on Kubernetes instead of locally, most commands above can be re-written with `tutor k8s exec service "command"` instead of `tutor local run service command`. For instance::
+When running on Kubernetes instead of locally, most commands above can be re-written with ``tutor k8s exec service "command"`` instead of ``tutor local run service command``. For instance::
 
     # Privileged user creation
     tutor k8s exec cairn-superset "superset fab create-admin --username YOURUSERNAME --email user@example.com"
     # Unprivileged user creation
     tutor k8s exec cairn-clickhouse "cairn createuser --course-id='course-v1:edX+DemoX+Demo_Course' --org-id='edX' YOURUSERNAME"
     tutor k8s exec cairn-superset "cairn createuser YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM"
 
@@ -183,27 +186,29 @@
 The latter command will parse tracking log events from the ``$(tutor config printroot)/data/lms/logs/tracking.log`` file that contains all the tracking logs since the creation of your platform. The command will take a while to run if you have a large platform that has been running for a long time. It can be interrupted at any time and started again, as the log collector keeps track of its position within the tracking log file.
 
 Adding data to your data lake
 -----------------------------
 
 Tables created in Clickhouse are managed by a lightweight migration system. You can view existing migrations that ship by default with Cairn in the following folder: ``$VIRTUAL_ENV/lib/python3.8/site-packages/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/``.
 
-You are free to create your own migrations that will automatically be created in Clickhouse every time the ``tutor local quickstart`` or ``tutor local init`` commands are run. To do so, as usual in Tutor, you should create a `Tutor plugin <https://docs.tutor.overhang.io/plugins.html>`__. This plugin should include the ``CAIRN_MIGRATIONS_FOLDER`` configuration. This setting should point to a template folder, inside the plugin, where migration templates are defined. For instance, assuming you created the "customcairn" plugin::
+You are free to create your own migrations that will automatically be created in Clickhouse every time the ``tutor local launch`` or ``tutor local do init`` commands are run. To do so, as usual in Tutor, you should create a `Tutor plugin <https://docs.tutor.overhang.io/plugins.html>`__. This plugin should include the ``CAIRN_MIGRATIONS_FOLDER`` configuration. This setting should point to a template folder, inside the plugin, where migration templates are defined. For instance, assuming you created the "customcairn" plugin::
 
     config = {
         "defaults": {
             "CAIRN_MIGRATIONS_FOLDER": "customcairn/apps/migrations.d"
         }
     }
 
-In this example, the following folder should be created in the plugin:: ``tutorcustomcairn/templates/customcairn/apps/migrations.d/``. Then, you should add your migration files there. Migrations will be applied in alphabetical order whenever you run ``tutor local quickstart`` or ``tutor local init``.
+In this example, the following folder should be created in the plugin:: ``tutorcustomcairn/templates/customcairn/apps/migrations.d/``. Then, you should add your migration files there. Migrations will be applied in alphabetical order whenever you run ``tutor local launch`` or ``tutor local do init``.
 
 Development
 -----------
 
+In development, the Superset user interface will be available at http://data.local.overhang.io:2247.
+
 To reload Vector configuration after changes to vector.toml, run::
 
     tutor config save && tutor local exec cairn-vector sh -c "kill -s HUP 1"
 
 To explore the clickhouse database as root, run::
 
     tutor local run cairn-clickhouse cairn client
@@ -217,15 +222,15 @@
 
 Cairn is configured by several Tutor settings. Each one of these settings may be modified individually by running::
 
     tutor config save --set SETTING_NAME=settingvalue
 
 Then apply changes with::
 
-    tutor local quickstart
+    tutor local launch
 
 General settings
 ~~~~~~~~~~~~~~~~
 
 - ``CAIRN_HOST`` (default: ``"data.{{ LMS_HOST }}"``): hostname at which the Cairn frontend (i.e: Superset) will be accessible. By default, this is the "data" subdomain of the LMS. Thus, if your students access the LMS at https://learn.mydomain.com then Cairn will be accessible at https://data.learn.mydomain.com.
 - ``CAIRN_DOCKER_HOST_SOCK_PATH`` (default: ``"/var/run/docker.sock"``): path to the Docker host socket on the host. This is required to collect logs from Docker when running locally, but it is not used when running on Kubernetes.
 
@@ -249,22 +254,19 @@
 - ``CAIRN_SUPERSET_LANGUAGE_CODE`` (default: ``"{{ LANGUAGE_CODE[:2] }}"``): 2-letter code of the default language for the Superset frontend. View the list of all supported languages `here <https://github.com/apache/superset/blob/dc575080d7e43d40b1734bb8f44fdc291cb95b11/superset/config.py#L324>`__. When different than "en", users will have the opportunity to switch from English to this language via a flag icon in the top-right corner.
 - ``CAIRN_SUPERSET_DOCKER_IMAGE`` (default: ``"{{ DOCKER_REGISTRY }}overhangio/cairn-superset:{{ CAIRN_VERSION }}"``): name of the Docker image that runs Postgresql.
 - ``CAIRN_POSTGRESQL_DATABASE`` (default: ``"superset"``): name of the Postgresql database.
 - ``CAIRN_POSTGRESQL_USERNAME`` (default: ``"superset"``): Postgresql username.
 - ``CAIRN_POSTGRESQL_PASSWORD`` (default: ``"{{ 20|random_string }}"``): Postgresql password.
 - ``CAIRN_SUPERSET_SECRET_KEY`` (default: ``"{{ 20|random_string }}"``): randomly-generated secret key for the Superset frontend.
 
+Troubleshooting
+---------------
 
-Support
--------
-
-Are you having trouble with Cairn? Do you have questions about this plugin? Please get in touch with us at contact@overhang.io. Community support is also available on the official Tutor forums: https://discuss.overhang.io
+This Tutor plugin is maintained by Régis Behmo from `Overhang.IO <https://overhang.io>`__. Community support is available from the official `Open edX forum <https://discuss.openedx.org>`__. Do you need help with this plugin? See the `troubleshooting <https://docs.tutor.overhang.io/troubleshooting.html>`__ section from the Tutor documentation.
 
 License
 -------
 
 This software is licensed under the terms of the AGPLv3.
 
 .. image:: https://overhang.io/static/catalog/img/cairn.png
     :alt: Alpine cairn
-
-
```

### Comparing `tutor-cairn-15.0.6/tutor_cairn.egg-info/SOURCES.txt` & `tutor-cairn-16.0.0/tutor_cairn.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.py
 tutor_cairn.egg-info/PKG-INFO
 tutor_cairn.egg-info/SOURCES.txt
 tutor_cairn.egg-info/dependency_links.txt
 tutor_cairn.egg-info/entry_points.txt
 tutor_cairn.egg-info/requires.txt
 tutor_cairn.egg-info/top_level.txt
@@ -13,15 +14,18 @@
 tutorcairn/patches/.gitignore
 tutorcairn/patches/caddyfile
 tutorcairn/patches/k8s-deployments
 tutorcairn/patches/k8s-jobs
 tutorcairn/patches/k8s-services
 tutorcairn/patches/k8s-volumes
 tutorcairn/patches/kustomization-configmapgenerator
+tutorcairn/patches/local-docker-compose-dev-services
 tutorcairn/patches/local-docker-compose-jobs-services
+tutorcairn/patches/local-docker-compose-permissions-command
+tutorcairn/patches/local-docker-compose-permissions-volumes
 tutorcairn/patches/local-docker-compose-services
 tutorcairn/templates/cairn/apps/.gitignore
 tutorcairn/templates/cairn/apps/clickhouse/auth.json
 tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0001_create.sql
 tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0002_grades.sql
 tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0003_course_enrollments.sql
 tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0004_video_views.sql
@@ -37,14 +41,16 @@
 tutorcairn/templates/cairn/apps/vector/k8s.toml
 tutorcairn/templates/cairn/apps/vector/local.toml
 tutorcairn/templates/cairn/apps/vector/partials/common-post.toml
 tutorcairn/templates/cairn/apps/vector/partials/common-pre.toml
 tutorcairn/templates/cairn/build/.gitignore
 tutorcairn/templates/cairn/build/cairn-clickhouse/Dockerfile
 tutorcairn/templates/cairn/build/cairn-clickhouse/scripts/cairn
-tutorcairn/templates/cairn/build/cairn-clickhouse/scripts/clickhouse-auth.json
 tutorcairn/templates/cairn/build/cairn-superset/Dockerfile
-tutorcairn/templates/cairn/build/cairn-superset/scripts/cairn
+tutorcairn/templates/cairn/build/cairn-superset/cairn/__init__.py
+tutorcairn/templates/cairn/build/cairn-superset/cairn/bootstrap.py
+tutorcairn/templates/cairn/build/cairn-superset/cairn/ctl.py
+tutorcairn/templates/cairn/build/cairn-superset/cairn/sso.py
 tutorcairn/templates/cairn/tasks/.gitignore
 tutorcairn/templates/cairn/tasks/cairn-clickhouse/init
 tutorcairn/templates/cairn/tasks/cairn-openedx/init
 tutorcairn/templates/cairn/tasks/cairn-superset/init
```

### Comparing `tutor-cairn-15.0.6/tutorcairn/patches/k8s-deployments` & `tutor-cairn-16.0.0/tutorcairn/patches/k8s-deployments`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,15 @@
           image: {{ CAIRN_SUPERSET_DOCKER_IMAGE }}
           volumeMounts:
             - mountPath: /app/superset_config.py
               name: config
               subPath: superset_config.py
             - mountPath: /app/bootstrap/
               name: bootstrap
-            - mountPath: /scripts/clickhouse-auth.json
+            - mountPath: /app/superset/cairn/clickhouse-auth.json
               name: clickhouse-auth
               subPath: auth.json
           securityContext:
             allowPrivilegeEscalation: false
       volumes:
         - name: config
           configMap:
```

### Comparing `tutor-cairn-15.0.6/tutorcairn/patches/k8s-jobs` & `tutor-cairn-16.0.0/tutorcairn/patches/k8s-jobs`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
           image: {{ CAIRN_SUPERSET_DOCKER_IMAGE }}
           volumeMounts:
             - mountPath: /app/superset_config.py
               name: config
               subPath: superset_config.py
             - mountPath: /app/bootstrap/
               name: bootstrap
-            - mountPath: /scripts/clickhouse-auth.json
+            - mountPath: /app/superset/cairn/clickhouse-auth.json
               name: clickhouse-auth
               subPath: auth.json
       volumes:
         - name: config
           configMap:
             name: cairn-superset-config
         - name: bootstrap
```

### Comparing `tutor-cairn-15.0.6/tutorcairn/patches/k8s-services` & `tutor-cairn-16.0.0/tutorcairn/patches/k8s-services`

 * *Files identical despite different names*

### Comparing `tutor-cairn-15.0.6/tutorcairn/patches/k8s-volumes` & `tutor-cairn-16.0.0/tutorcairn/patches/k8s-volumes`

 * *Files identical despite different names*

### Comparing `tutor-cairn-15.0.6/tutorcairn/patches/kustomization-configmapgenerator` & `tutor-cairn-16.0.0/tutorcairn/patches/kustomization-configmapgenerator`

 * *Files identical despite different names*

### Comparing `tutor-cairn-15.0.6/tutorcairn/patches/local-docker-compose-jobs-services` & `tutor-cairn-16.0.0/tutorcairn/patches/local-docker-compose-jobs-services`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         {%- endfor %}
     environment:
         CLICKHOUSE_DO_NOT_CHOWN: "1"
 cairn-superset-job:
     image: {{ CAIRN_SUPERSET_DOCKER_IMAGE }}
     volumes:
         - ../plugins/cairn/apps/superset/superset_config.py:/app/superset_config.py:ro
-        - ../plugins/cairn/apps/clickhouse/auth.json:/scripts/clickhouse-auth.json:ro
+        - ../plugins/cairn/apps/clickhouse/auth.json:/app/superset/cairn/clickhouse-auth.json:ro
         - ../plugins/cairn/apps/superset/bootstrap:/app/bootstrap:ro
     healthcheck:
         disable: true
     depends_on:
         {% if RUN_REDIS %}- redis{% endif %}
         - cairn-postgresql
 cairn-openedx-job:
```

### Comparing `tutor-cairn-15.0.6/tutorcairn/patches/local-docker-compose-services` & `tutor-cairn-16.0.0/tutorcairn/patches/local-docker-compose-services`

 * *Files 10% similar despite different names*

```diff
@@ -24,47 +24,50 @@
         CLICKHOUSE_DO_NOT_CHOWN: "1"
     ulimits:
         nofile:
             soft: 262144
             hard: 262144
     restart: unless-stopped
     depends_on:
-        - cairn-clickhouse-permissions
-cairn-clickhouse-permissions:
-    image: {{ DOCKER_IMAGE_PERMISSIONS }}
-    command: ["1000", "/data/clickhouse"]
-    restart: on-failure
-    volumes:
-      - ../../data/cairn/clickhouse:/data/clickhouse
+        - permissions
 {% endif %}
 cairn-superset:
     image: {{ CAIRN_SUPERSET_DOCKER_IMAGE }}
     volumes:
         - ../plugins/cairn/apps/superset/superset_config.py:/app/superset_config.py:ro
-        - ../plugins/cairn/apps/clickhouse/auth.json:/scripts/clickhouse-auth.json:ro
+        - ../plugins/cairn/apps/clickhouse/auth.json:/app/superset/cairn/clickhouse-auth.json:ro
         - ../plugins/cairn/apps/superset/bootstrap:/app/bootstrap:ro
+        {%- for mount in iter_mounts(MOUNTS, "cairn-superset") %}
+        - {{ mount }}
+        {%- endfor %}
     restart: unless-stopped
     depends_on:
         {% if RUN_REDIS %}- redis{% endif %}
         - cairn-postgresql
 cairn-superset-worker:
     image: {{ CAIRN_SUPERSET_DOCKER_IMAGE }}
     volumes:
         - ../plugins/cairn/apps/superset/superset_config.py:/app/superset_config.py:ro
+        {%- for mount in iter_mounts(MOUNTS, "cairn-superset") %}
+        - {{ mount }}
+        {%- endfor %}
     command: celery --app=superset.tasks.celery_app:app worker -Ofair -l INFO
     restart: unless-stopped
     healthcheck:
         disable: true
     depends_on:
         {% if RUN_REDIS %}- redis{% endif %}
         - cairn-postgresql
 cairn-superset-worker-beat:
     image: {{ CAIRN_SUPERSET_DOCKER_IMAGE }}
     volumes:
         - ../plugins/cairn/apps/superset/superset_config.py:/app/superset_config.py:ro
+        {%- for mount in iter_mounts(MOUNTS, "cairn-superset") %}
+        - {{ mount }}
+        {%- endfor %}
     command: celery --app=superset.tasks.celery_app:app beat --pidfile /tmp/celerybeat.pid -l INFO --schedule=/tmp/celerybeat-schedule
     restart: unless-stopped
     healthcheck:
         disable: true
     depends_on:
         {% if RUN_REDIS %}- redis{% endif %}
         - cairn-postgresql
@@ -76,15 +79,9 @@
         POSTGRES_PASSWORD: "{{ CAIRN_POSTGRESQL_PASSWORD }}"
         POSTGRES_DB: "{{ CAIRN_POSTGRESQL_DATABASE }}"
     volumes:
         - ../../data/cairn/postgresql:/var/lib/postgresql/data
     restart: unless-stopped
     user: "70:70"
     depends_on:
-        - cairn-postgresql-permissions
-cairn-postgresql-permissions:
-    image: {{ DOCKER_IMAGE_PERMISSIONS }}
-    command: ["70", "/data/postgresql"]
-    restart: on-failure
-    volumes:
-      - ../../data/cairn/postgresql:/data/postgresql
+        - permissions
 {% endif %}
```

### Comparing `tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0001_create.sql` & `tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0001_create.sql`

 * *Files identical despite different names*

### Comparing `tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0003_course_enrollments.sql` & `tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0003_course_enrollments.sql`

 * *Files identical despite different names*

### Comparing `tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0004_video_views.sql` & `tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0004_video_views.sql`

 * *Files identical despite different names*

### Comparing `tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0006_course_block_completion.sql` & `tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0006_course_block_completion.sql`

 * *Files identical despite different names*

### Comparing `tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0007_fix_video_segments.sql` & `tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0007_fix_video_segments.sql`

 * *Files identical despite different names*

### Comparing `tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0008_rename_openedx_tables.sql` & `tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0008_rename_openedx_tables.sql`

 * *Files identical despite different names*

### Comparing `tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/openedx/scripts/importcoursedata.py` & `tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/openedx/scripts/importcoursedata.py`

 * *Files identical despite different names*

### Comparing `tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/superset/bootstrap/courseoverview.json` & `tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/superset/bootstrap/courseoverview.json`

 * *Files identical despite different names*

### Comparing `tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/superset/superset_config.py` & `tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/superset/superset_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 import logging
+import os
+import typing as t
 
 from cachelib.redis import RedisCache
 from celery.schedules import crontab
 
+from superset.extensions import security_manager
+from superset.cairn import bootstrap as cairn_bootstrap
+from superset.cairn import sso as cairn_sso
+
 # https://superset.apache.org/docs/installation/configuring-superset
 SECRET_KEY = "{{ CAIRN_SUPERSET_SECRET_KEY }}"
 SQLALCHEMY_DATABASE_URI = "postgresql+psycopg2://{{ CAIRN_POSTGRESQL_USERNAME }}:{{ CAIRN_POSTGRESQL_PASSWORD }}@cairn-postgresql/{{ CAIRN_POSTGRESQL_DATABASE }}"
 
 {% if not ENABLE_WEB_PROXY %}
 # Caddy is running behind a proxy: Superset needs to handle x-forwarded-* headers
 # https://flask.palletsprojects.com/en/latest/deploying/proxy_fix/
@@ -42,32 +48,73 @@
 # Borrowed from superset/docker/pythonpath_dev/superset_config.py
 REDIS_HOST = "{{ REDIS_HOST }}"
 REDIS_PORT = "{{ REDIS_PORT }}"
 # Be careful not to conflict with Open edX here
 REDIS_CELERY_DB = {{ OPENEDX_CELERY_REDIS_DB + 2 }}
 REDIS_CACHE_DB = {{ OPENEDX_CACHE_REDIS_DB + 2 }}
 
-# Charting data queried from datasets cache (optional)
-DATA_CACHE_CONFIG = {
+# Cache configuration
+CACHE_CONFIG = {
     "CACHE_TYPE": "redis",
-    "CACHE_DEFAULT_TIMEOUT": 60 * 60 * 24,  # 1 day default (in secs)
+    "CACHE_DEFAULT_TIMEOUT": 60 * 60 * 24 * 1,  # 1 day default (in secs)
     "CACHE_KEY_PREFIX": "superset_data_cache",
     "CACHE_REDIS_URL": f"redis://{REDIS_HOST}:{REDIS_PORT}/{REDIS_CACHE_DB}",
 }
-# Metadata cache (optional)
-CACHE_CONFIG = DATA_CACHE_CONFIG
-# SQL Lab query results cache (optional)
+DATA_CACHE_CONFIG = CACHE_CONFIG.copy()
+FILTER_STATE_CACHE_CONFIG = CACHE_CONFIG.copy()
+FILTER_STATE_CACHE_CONFIG.update({
+    "CACHE_DEFAULT_TIMEOUT": 60 * 60 * 24 * 90,  # 90 days
+    "REFRESH_TIMEOUT_ON_RETRIEVAL": True,
+})
+EXPLORE_FORM_DATA_CACHE_CONFIG  = CACHE_CONFIG.copy()
+EXPLORE_FORM_DATA_CACHE_CONFIG.update({
+    "CACHE_DEFAULT_TIMEOUT": 60 * 60 * 24 * 7,  # 7 days
+    "REFRESH_TIMEOUT_ON_RETRIEVAL": True,
+})
 RESULTS_BACKEND = RedisCache(
     host=REDIS_HOST,
     port=REDIS_PORT,
     db=REDIS_CACHE_DB,
     key_prefix="superset_results",
 )
 
-# TODO implement FILTER_STATE_CACHE_CONFIG and EXPLORE_FORM_DATA_CACHE_CONFIG such that we get rid of the warning messages
+{% if CAIRN_ENABLE_SSO %}
+# Authentication
+# https://superset.apache.org/docs/installation/configuring-superset/#custom-oauth2-configuration
+# https://flask-appbuilder.readthedocs.io/en/latest/security.html#authentication-oauth
+from flask_appbuilder.security.manager import AUTH_OAUTH
+AUTH_TYPE = AUTH_OAUTH
+OPENEDX_LMS_ROOT_URL = "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ LMS_HOST }}"
+OPENEDX_SSO_CLIENT_ID = "{{ CAIRN_SSO_CLIENT_ID }}"
+if os.environ.get("FLASK_ENV") == "development":
+    OPENEDX_LMS_ROOT_URL = "http://{{ LMS_HOST }}:8000"
+    OPENEDX_SSO_CLIENT_ID = "{{ CAIRN_SSO_CLIENT_ID }}-dev"
+OAUTH_PROVIDERS = [
+    {
+        "name": cairn_sso.OPENEDX_SSO_PROVIDER,
+        "token_key": "access_token",
+        "icon": "fa-right-to-bracket",
+        "remote_app": {
+            "client_id": OPENEDX_SSO_CLIENT_ID,
+            "client_secret": "{{ CAIRN_SSO_CLIENT_SECRET }}",
+            "client_kwargs": {"scope": "read"},
+            "access_token_method": "POST",
+            "api_base_url": f"{OPENEDX_LMS_ROOT_URL}",
+            "access_token_url": f"{OPENEDX_LMS_ROOT_URL}/oauth2/access_token/",
+            "authorize_url": f"{OPENEDX_LMS_ROOT_URL}/oauth2/authorize/",
+        }
+    }
+]
+CUSTOM_SECURITY_MANAGER = cairn_sso.OpenEdxSsoSecurityManager
+# Update roles on login: this will cause all roles (except those that are preserved) to
+# be ovewritten.
+AUTH_ROLES_SYNC_AT_LOGIN = True
+# Login will create user
+AUTH_USER_REGISTRATION = True
+{% endif %}
 
 class CeleryConfig:  # pylint: disable=too-few-public-methods
     BROKER_URL = f"redis://{REDIS_HOST}:{REDIS_PORT}/{REDIS_CELERY_DB}"
     CELERY_IMPORTS = ("superset.sql_lab", "superset.tasks")
     CELERYD_LOG_LEVEL = "DEBUG"
     CELERYD_PREFETCH_MULTIPLIER = 1
     CELERY_ACKS_LATE = False
@@ -97,20 +144,14 @@
 
 
 CELERY_CONFIG = CeleryConfig
 
 # Avoid duplicate logging because of propagation to root logger
 logging.getLogger("superset").propagate = False
 
-# Enable dashboard embedding
+# https://github.com/apache/superset/blob/master/RESOURCES/FEATURE_FLAGS.md
 FEATURE_FLAGS = {
+    # Enable dashboard embedding
     "EMBEDDED_SUPERSET": True
 }
 
-# Enable some custom feature flags
-# Do this once native filters are fully functional https://github.com/apache/superset/projects/15+
-# def get_cairn_feature_flags(flags):
-#     flags["DASHBOARD_NATIVE_FILTERS"] = True
-#     return flags
-# GET_FEATURE_FLAGS_FUNC = get_cairn_feature_flags
-
 {{ patch("cairn-superset-settings") }}
```

### Comparing `tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/vector/partials/common-post.toml` & `tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/vector/partials/common-post.toml`

 * *Files identical despite different names*

### Comparing `tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/cairn-clickhouse/Dockerfile` & `tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-clickhouse/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/cairn-superset/Dockerfile` & `tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-superset/Dockerfile`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 # Superset image with additional database drivers
 # https://hub.docker.com/r/apache/superset
 # https://github.com/apache/superset/releases
 # https://github.com/apache/superset/blob/master/Dockerfile
 # https://superset.apache.org/docs/databases/installing-database-drivers
-FROM docker.io/apache/superset:2.0.0
+FROM docker.io/apache/superset:2.1.0
 
 USER root
 
 # https://pypi.org/project/clickhouse-driver/
 # https://pypi.org/project/mysqlclient/
+# https://pypi.org/project/clickhouse-connect/
 # https://pypi.org/project/clickhouse-sqlalchemy/
-RUN pip install clickhouse-driver==0.2.4 mysqlclient==2.1.1
-# Later versions of clickhouse-sqlalchemy will not work.
-# Note that this connector be replaced by clickhouse-connect in v2.0.1:
-# https://github.com/apache/superset/pull/22039
-RUN pip install clickhouse-sqlalchemy==0.1.10
-
-COPY --chown=superset:superset ./scripts /scripts
-RUN chmod a+x /scripts/*
-ENV PATH /scripts:${PATH}
+# https://pypi.org/project/Authlib/
+# We preserve the clickhouse-sqlalchemy package to keep backward compatibility with existing dashboards
+RUN {% if is_buildkit_enabled() %}--mount=type=cache,target=/root/.cache/pip,sharing=shared {% endif %}pip install \
+    clickhouse-driver==0.2.6 \
+    mysqlclient==2.1.1 \
+    clickhouse-connect==0.5.24 \
+    clickhouse-sqlalchemy==0.2.4 \
+    authlib==1.2.0
 
 USER superset
 
+# Copy lib
+COPY --chown=superset:superset ./cairn /app/superset/cairn
+
 # This is required to have a proper healthcheck
 ENV SUPERSET_PORT=8000
 
 ENTRYPOINT []
 CMD gunicorn \
     --bind  "0.0.0.0:8000" \
     --access-logfile '-' \
```

### Comparing `tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/cairn-superset/scripts/cairn` & `tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-superset/cairn/ctl.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #! /usr/bin/env python3
 
 import argparse
-from getpass import getpass
 import json
-import os
 from time import time
 
 from superset.app import create_app
 
 app = create_app()
 app.app_context().push()
 
 from superset.connectors.sqla.models import SqlaTable
 from superset.models.core import Database
 from superset.models.slice import Slice
 from superset.extensions import db, security_manager
 import superset.dashboards.commands.importers.v0 as importers
-from superset.utils.database import get_or_create_db
 from werkzeug.security import generate_password_hash
 
+# Our convenient library
+from superset.cairn import bootstrap as cairn_bootstrap
+
 
 now = time()
 
 
 def main():
     parser = argparse.ArgumentParser(
         description="Bootstrap user creation and dashboards"
@@ -42,32 +42,30 @@
     )
     parser_user.add_argument(
         "--admin",
         action="store_true",
         help=("Make the user an administrator."),
     )
     parser_user.add_argument(
-        "-r",
-        "--role",
-        help=(
-            "Name of the role to which the user should be assigned."
-            " Defaults to the username."
-        ),
-    )
-    parser_user.add_argument(
         "-p",
         "--password",
-        help="User password. If undefined, you will be prompted for one.",
+        help="User password.",
     )
     parser_user.add_argument(
         "--firstname", default="", help="User first name (optional)."
     )
     parser_user.add_argument(
         "--lastname", default="", help="User last name (optional)."
     )
+    parser_user.add_argument(
+        "-c",
+        "--course-id",
+        action="append",
+        help="Restrict user to access data only from these courses.",
+    )
     parser_user.add_argument("username")
     parser_user.add_argument("email")
     parser_user.set_defaults(func=bootstrap_user)
 
     # Bootstrap dashboards
     parser_dashboards = subparsers.add_parser(
         "bootstrap-dashboards",
@@ -91,92 +89,61 @@
 
 
 # Note: we'd like to get rid of this command by relying on `superset fab create-user`
 # but the "create-user" command fails if the user already exists.
 def bootstrap_user(args):
     # Bootstrap database
     database_name = args.db or args.username
-    bootstrap_database(args.username, database_name)
+    cairn_bootstrap.create_superset_db(args.username, database_name)
 
     # Get or create user
     user = security_manager.find_user(args.username)
     if user:
         print(f"User '{args.username}' already exists. Skipping creation.")
-        if args.password:
-            print("Setting user password...")
-            user.password = generate_password_hash(args.password)
-            db.session.add(user)
-            db.session.commit()
     else:
         print(f"Creating user '{args.username}'...")
-        password = args.password
-        while not password:
-            password = getpass()
-        base_role_name = "Admin" if args.admin else "Gamma"
         user = security_manager.add_user(
             args.username,
             args.firstname,
             args.lastname,
             args.email,
-            security_manager.find_role(base_role_name),
-            password=password,
+            "Gamma",
         )
         if user is None or user is False:
             # This may happen for instance when the email address is already associated
             # to a different username
             raise RuntimeError(
                 f"Failed to create user '{args.username}' email='{args.email}'"
             )
 
-    # Associate role with the same name to user, if it exists
-    role_name = args.role or args.username
-
-    def check_permission(permission_view):
-        permission_name = str(permission_view)
-        if permission_name in [
-            "can save on Datasource",
-            "can sqllab on Superset",
-            "can sql json on Superset",
-            "menu access on Datasets",
-            "menu access on SQL Lab",
-        ]:
-            return True
-        if permission_name.startswith(f"database access on [{database_name}]"):
-            return True
-        if permission_name.startswith(f"schema access on [{database_name}]"):
-            return True
-        return False
-
-    security_manager.set_role(role_name, check_permission)
-    role = security_manager.find_role(role_name)
-    if role in user.roles:
-        print(f"Role '{role_name}' is already associated to user.")
-    else:
-        print(f"Associating role '{role_name}' to user...")
-        user.roles.append(role)
+    # Set password
+    if args.password:
+        print("Setting user password...")
+        user.password = generate_password_hash(args.password)
         db.session.add(user)
         db.session.commit()
-    print("Done.")
 
+    # Create user role, clickhouse db, etc.
+    cairn_bootstrap.setup_user(args.username, course_ids=args.course_id)
 
-def bootstrap_database(username, database_name):
-    with open(
-        os.path.join(os.path.dirname(__file__), "clickhouse-auth.json"),
-        encoding="utf-8",
-    ) as f:
-        CLICKHOUSE_AUTH = json.load(f)
-
-    host = CLICKHOUSE_AUTH["host"]
-    port = CLICKHOUSE_AUTH["port"]
-    database = CLICKHOUSE_AUTH["database"]
-    uri = f"clickhouse+native://{username}:@{host}:{port}/{database}"
-    database = get_or_create_db(database_name, uri, always_create=True)
+    # Associate user to roles
+    user_roles = cairn_bootstrap.get_role_names(args.username)
+    if args.admin:
+        user_roles.append("Admin")
+    for role_name in user_roles:
+        role = security_manager.find_role(role_name)
+        if role in user.roles:
+            print(f"Role '{role_name}' is already associated to user.")
+        else:
+            print(f"Associating role '{role_name}' to user...")
+            user.roles.append(role)
+            db.session.add(user)
+            db.session.commit()
 
-    db.session.add(database)
-    db.session.commit()
+    print("Done.")
 
 
 # Note: we would like to start using superset's native export/import-dashboards command
 # but we failed to get it to work.
 def bootstrap_dashboards(args):
     database_name = args.db or args.username
     database = load_database(database_name)
```

