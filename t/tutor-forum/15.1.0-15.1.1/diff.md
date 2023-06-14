# Comparing `tmp/tutor-forum-15.1.0.tar.gz` & `tmp/tutor-forum-15.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tutor-forum-15.1.0.tar", last modified: Tue Feb  7 12:19:02 2023, max compression
+gzip compressed data, was "dist/tutor-forum-15.1.1.tar", last modified: Wed Mar 15 11:21:59 2023, max compression
```

## Comparing `tutor-forum-15.1.0.tar` & `tutor-forum-15.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-02-07 12:19:02.000000 tutor-forum-15.1.0/
--rw-r--r--   0 ci        (1000) ci        (1000)       79 2023-02-07 12:18:52.000000 tutor-forum-15.1.0/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)     3447 2023-02-07 12:19:02.000000 tutor-forum-15.1.0/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     2458 2023-02-07 12:18:52.000000 tutor-forum-15.1.0/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-02-07 12:19:02.000000 tutor-forum-15.1.0/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     1863 2023-02-07 12:18:52.000000 tutor-forum-15.1.0/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-02-07 12:19:02.000000 tutor-forum-15.1.0/tutor_forum.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)     3447 2023-02-07 12:19:02.000000 tutor-forum-15.1.0/tutor_forum.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)      899 2023-02-07 12:19:02.000000 tutor-forum-15.1.0/tutor_forum.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-02-07 12:19:02.000000 tutor-forum-15.1.0/tutor_forum.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       44 2023-02-07 12:19:02.000000 tutor-forum-15.1.0/tutor_forum.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-02-07 12:19:02.000000 tutor-forum-15.1.0/tutor_forum.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       11 2023-02-07 12:19:02.000000 tutor-forum-15.1.0/tutor_forum.egg-info/top_level.txt
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-02-07 12:19:02.000000 tutor-forum-15.1.0/tutorforum/
--rw-r--r--   0 ci        (1000) ci        (1000)       23 2023-02-07 12:18:52.000000 tutor-forum-15.1.0/tutorforum/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-02-07 12:18:52.000000 tutor-forum-15.1.0/tutorforum/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-02-07 12:19:02.000000 tutor-forum-15.1.0/tutorforum/patches/
--rw-r--r--   0 ci        (1000) ci        (1000)     1334 2023-02-07 12:18:52.000000 tutor-forum-15.1.0/tutorforum/patches/k8s-deployments
--rw-r--r--   0 ci        (1000) ci        (1000)     1057 2023-02-07 12:18:52.000000 tutor-forum-15.1.0/tutorforum/patches/k8s-jobs
--rw-r--r--   0 ci        (1000) ci        (1000)      184 2023-02-07 12:18:52.000000 tutor-forum-15.1.0/tutorforum/patches/k8s-services
--rw-r--r--   0 ci        (1000) ci        (1000)       95 2023-02-07 12:18:52.000000 tutor-forum-15.1.0/tutorforum/patches/lms-env
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-02-07 12:18:52.000000 tutor-forum-15.1.0/tutorforum/patches/local-docker-compose-dev-services
--rw-r--r--   0 ci        (1000) ci        (1000)      700 2023-02-07 12:18:52.000000 tutor-forum-15.1.0/tutorforum/patches/local-docker-compose-jobs-services
--rw-r--r--   0 ci        (1000) ci        (1000)        8 2023-02-07 12:18:52.000000 tutor-forum-15.1.0/tutorforum/patches/local-docker-compose-lms-dependencies
--rw-r--r--   0 ci        (1000) ci        (1000)      722 2023-02-07 12:18:52.000000 tutor-forum-15.1.0/tutorforum/patches/local-docker-compose-services
--rw-r--r--   0 ci        (1000) ci        (1000)       45 2023-02-07 12:18:52.000000 tutor-forum-15.1.0/tutorforum/patches/openedx-common-settings
--rw-r--r--   0 ci        (1000) ci        (1000)       55 2023-02-07 12:18:52.000000 tutor-forum-15.1.0/tutorforum/patches/openedx-lms-development-settings
--rw-r--r--   0 ci        (1000) ci        (1000)     3082 2023-02-07 12:18:52.000000 tutor-forum-15.1.0/tutorforum/plugin.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-02-07 12:19:02.000000 tutor-forum-15.1.0/tutorforum/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-02-07 12:19:02.000000 tutor-forum-15.1.0/tutorforum/templates/forum/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-02-07 12:19:02.000000 tutor-forum-15.1.0/tutorforum/templates/forum/build/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-02-07 12:19:02.000000 tutor-forum-15.1.0/tutorforum/templates/forum/build/forum/
--rw-r--r--   0 ci        (1000) ci        (1000)     1638 2023-02-07 12:18:52.000000 tutor-forum-15.1.0/tutorforum/templates/forum/build/forum/Dockerfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-02-07 12:19:02.000000 tutor-forum-15.1.0/tutorforum/templates/forum/build/forum/bin/
--rw-r--r--   0 ci        (1000) ci        (1000)      654 2023-02-07 12:18:52.000000 tutor-forum-15.1.0/tutorforum/templates/forum/build/forum/bin/docker-entrypoint.sh
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-02-07 12:19:02.000000 tutor-forum-15.1.0/tutorforum/templates/forum/tasks/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-02-07 12:19:02.000000 tutor-forum-15.1.0/tutorforum/templates/forum/tasks/forum/
--rw-r--r--   0 ci        (1000) ci        (1000)       75 2023-02-07 12:18:52.000000 tutor-forum-15.1.0/tutorforum/templates/forum/tasks/forum/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-15 11:21:59.000000 tutor-forum-15.1.1/
+-rw-r--r--   0 ci        (1000) ci        (1000)       79 2023-03-15 11:21:48.000000 tutor-forum-15.1.1/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     3611 2023-03-15 11:21:59.000000 tutor-forum-15.1.1/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     2622 2023-03-15 11:21:48.000000 tutor-forum-15.1.1/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-03-15 11:21:59.000000 tutor-forum-15.1.1/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     1863 2023-03-15 11:21:48.000000 tutor-forum-15.1.1/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-15 11:21:59.000000 tutor-forum-15.1.1/tutor_forum.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)     3611 2023-03-15 11:21:59.000000 tutor-forum-15.1.1/tutor_forum.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)      899 2023-03-15 11:21:59.000000 tutor-forum-15.1.1/tutor_forum.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-03-15 11:21:59.000000 tutor-forum-15.1.1/tutor_forum.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       44 2023-03-15 11:21:59.000000 tutor-forum-15.1.1/tutor_forum.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-03-15 11:21:59.000000 tutor-forum-15.1.1/tutor_forum.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       11 2023-03-15 11:21:59.000000 tutor-forum-15.1.1/tutor_forum.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-15 11:21:59.000000 tutor-forum-15.1.1/tutorforum/
+-rw-r--r--   0 ci        (1000) ci        (1000)       23 2023-03-15 11:21:48.000000 tutor-forum-15.1.1/tutorforum/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-03-15 11:21:48.000000 tutor-forum-15.1.1/tutorforum/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-15 11:21:59.000000 tutor-forum-15.1.1/tutorforum/patches/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1334 2023-03-15 11:21:48.000000 tutor-forum-15.1.1/tutorforum/patches/k8s-deployments
+-rw-r--r--   0 ci        (1000) ci        (1000)     1057 2023-03-15 11:21:48.000000 tutor-forum-15.1.1/tutorforum/patches/k8s-jobs
+-rw-r--r--   0 ci        (1000) ci        (1000)      184 2023-03-15 11:21:48.000000 tutor-forum-15.1.1/tutorforum/patches/k8s-services
+-rw-r--r--   0 ci        (1000) ci        (1000)       95 2023-03-15 11:21:48.000000 tutor-forum-15.1.1/tutorforum/patches/lms-env
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-03-15 11:21:48.000000 tutor-forum-15.1.1/tutorforum/patches/local-docker-compose-dev-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      700 2023-03-15 11:21:48.000000 tutor-forum-15.1.1/tutorforum/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 ci        (1000) ci        (1000)        8 2023-03-15 11:21:48.000000 tutor-forum-15.1.1/tutorforum/patches/local-docker-compose-lms-dependencies
+-rw-r--r--   0 ci        (1000) ci        (1000)      722 2023-03-15 11:21:48.000000 tutor-forum-15.1.1/tutorforum/patches/local-docker-compose-services
+-rw-r--r--   0 ci        (1000) ci        (1000)       45 2023-03-15 11:21:48.000000 tutor-forum-15.1.1/tutorforum/patches/openedx-common-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)       55 2023-03-15 11:21:48.000000 tutor-forum-15.1.1/tutorforum/patches/openedx-lms-development-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)     3219 2023-03-15 11:21:48.000000 tutor-forum-15.1.1/tutorforum/plugin.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-15 11:21:59.000000 tutor-forum-15.1.1/tutorforum/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-15 11:21:59.000000 tutor-forum-15.1.1/tutorforum/templates/forum/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-15 11:21:59.000000 tutor-forum-15.1.1/tutorforum/templates/forum/build/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-15 11:21:59.000000 tutor-forum-15.1.1/tutorforum/templates/forum/build/forum/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1708 2023-03-15 11:21:48.000000 tutor-forum-15.1.1/tutorforum/templates/forum/build/forum/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-15 11:21:59.000000 tutor-forum-15.1.1/tutorforum/templates/forum/build/forum/bin/
+-rw-r--r--   0 ci        (1000) ci        (1000)      654 2023-03-15 11:21:48.000000 tutor-forum-15.1.1/tutorforum/templates/forum/build/forum/bin/docker-entrypoint.sh
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-15 11:21:59.000000 tutor-forum-15.1.1/tutorforum/templates/forum/tasks/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-15 11:21:59.000000 tutor-forum-15.1.1/tutorforum/templates/forum/tasks/forum/
+-rw-r--r--   0 ci        (1000) ci        (1000)       75 2023-03-15 11:21:48.000000 tutor-forum-15.1.1/tutorforum/templates/forum/tasks/forum/init
```

### Comparing `tutor-forum-15.1.0/PKG-INFO` & `tutor-forum-15.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-forum
-Version: 15.1.0
+Version: 15.1.1
 Summary: forum plugin for Tutor
 Home-page: https://github.com/overhangio/tutor-forum
 Author: Overhang.IO
 Maintainer: Zaat.dev
 Maintainer-email: ghassan@zaat.dev
 License: AGPLv3
 Project-URL: Code, https://github.com/overhangio/tutor-forum
@@ -40,26 +40,28 @@
 
 Usage
 -----
 
 ::
 
     tutor plugins enable forum
-    tutor local quickstart
+    tutor local launch
 
 Configuration
 -------------
 
 - ``FORUM_DOCKER_IMAGE`` (default: ``""{{ DOCKER_REGISTRY }}overhangio/openedx-forum:{{ FORUM_VERSION }}"``)
 - ``FORUM_MONGODB_DATABASE`` (default: ``"cs_comments_service"``)
 - ``FORUM_PORT`` (default: ``"4567""``)
 - ``FORUM_API_KEY`` (default: ``"forumapikey"``)
 - ``FORUM_MONGODB_USE_SSL``: (default: ``False``)
 - ``FORUM_MONGODB_AUTH_SOURCE``: (default: ``""``)
 - ``FORUM_MONGODB_AUTH_MECH``: (default: ``""``)
+- ``FORUM_REPOSITORY`` (default: ``"https://github.com/openedx/cs_comments_service.git"``)
+- ``FORUM_REPOSITORY_VERSION`` (default: ``"{{ OPENEDX_COMMON_VERSION }}"``)
 
 Caveats for the `mongodb+srv://` syntax
 ---------------------------------------
 
 While the newer [`mongodb+srv://`](https://www.mongodb.com/developer/products/mongodb/srv-connection-strings/) syntax for the `MONGODB_HOST` is supported, there are some tradeoffs:
 
 - Query paramaters in the URL are not supported. For example, the URL `mongodb+srv://test:test@tutor.local/?ssl=true&authSource=admin` is invalid. Please use the provided configuration options instead.
```

### Comparing `tutor-forum-15.1.0/README.rst` & `tutor-forum-15.1.1/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -15,26 +15,28 @@
 
 Usage
 -----
 
 ::
 
     tutor plugins enable forum
-    tutor local quickstart
+    tutor local launch
 
 Configuration
 -------------
 
 - ``FORUM_DOCKER_IMAGE`` (default: ``""{{ DOCKER_REGISTRY }}overhangio/openedx-forum:{{ FORUM_VERSION }}"``)
 - ``FORUM_MONGODB_DATABASE`` (default: ``"cs_comments_service"``)
 - ``FORUM_PORT`` (default: ``"4567""``)
 - ``FORUM_API_KEY`` (default: ``"forumapikey"``)
 - ``FORUM_MONGODB_USE_SSL``: (default: ``False``)
 - ``FORUM_MONGODB_AUTH_SOURCE``: (default: ``""``)
 - ``FORUM_MONGODB_AUTH_MECH``: (default: ``""``)
+- ``FORUM_REPOSITORY`` (default: ``"https://github.com/openedx/cs_comments_service.git"``)
+- ``FORUM_REPOSITORY_VERSION`` (default: ``"{{ OPENEDX_COMMON_VERSION }}"``)
 
 Caveats for the `mongodb+srv://` syntax
 ---------------------------------------
 
 While the newer [`mongodb+srv://`](https://www.mongodb.com/developer/products/mongodb/srv-connection-strings/) syntax for the `MONGODB_HOST` is supported, there are some tradeoffs:
 
 - Query paramaters in the URL are not supported. For example, the URL `mongodb+srv://test:test@tutor.local/?ssl=true&authSource=admin` is invalid. Please use the provided configuration options instead.
```

### Comparing `tutor-forum-15.1.0/setup.py` & `tutor-forum-15.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-forum-15.1.0/tutor_forum.egg-info/PKG-INFO` & `tutor-forum-15.1.1/tutor_forum.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-forum
-Version: 15.1.0
+Version: 15.1.1
 Summary: forum plugin for Tutor
 Home-page: https://github.com/overhangio/tutor-forum
 Author: Overhang.IO
 Maintainer: Zaat.dev
 Maintainer-email: ghassan@zaat.dev
 License: AGPLv3
 Project-URL: Code, https://github.com/overhangio/tutor-forum
@@ -40,26 +40,28 @@
 
 Usage
 -----
 
 ::
 
     tutor plugins enable forum
-    tutor local quickstart
+    tutor local launch
 
 Configuration
 -------------
 
 - ``FORUM_DOCKER_IMAGE`` (default: ``""{{ DOCKER_REGISTRY }}overhangio/openedx-forum:{{ FORUM_VERSION }}"``)
 - ``FORUM_MONGODB_DATABASE`` (default: ``"cs_comments_service"``)
 - ``FORUM_PORT`` (default: ``"4567""``)
 - ``FORUM_API_KEY`` (default: ``"forumapikey"``)
 - ``FORUM_MONGODB_USE_SSL``: (default: ``False``)
 - ``FORUM_MONGODB_AUTH_SOURCE``: (default: ``""``)
 - ``FORUM_MONGODB_AUTH_MECH``: (default: ``""``)
+- ``FORUM_REPOSITORY`` (default: ``"https://github.com/openedx/cs_comments_service.git"``)
+- ``FORUM_REPOSITORY_VERSION`` (default: ``"{{ OPENEDX_COMMON_VERSION }}"``)
 
 Caveats for the `mongodb+srv://` syntax
 ---------------------------------------
 
 While the newer [`mongodb+srv://`](https://www.mongodb.com/developer/products/mongodb/srv-connection-strings/) syntax for the `MONGODB_HOST` is supported, there are some tradeoffs:
 
 - Query paramaters in the URL are not supported. For example, the URL `mongodb+srv://test:test@tutor.local/?ssl=true&authSource=admin` is invalid. Please use the provided configuration options instead.
```

### Comparing `tutor-forum-15.1.0/tutor_forum.egg-info/SOURCES.txt` & `tutor-forum-15.1.1/tutor_forum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tutor-forum-15.1.0/tutorforum/patches/k8s-deployments` & `tutor-forum-15.1.1/tutorforum/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-forum-15.1.0/tutorforum/patches/k8s-jobs` & `tutor-forum-15.1.1/tutorforum/patches/k8s-jobs`

 * *Files identical despite different names*

### Comparing `tutor-forum-15.1.0/tutorforum/patches/local-docker-compose-jobs-services` & `tutor-forum-15.1.1/tutorforum/patches/local-docker-compose-jobs-services`

 * *Files identical despite different names*

### Comparing `tutor-forum-15.1.0/tutorforum/patches/local-docker-compose-services` & `tutor-forum-15.1.1/tutorforum/patches/local-docker-compose-services`

 * *Files identical despite different names*

### Comparing `tutor-forum-15.1.0/tutorforum/plugin.py` & `tutor-forum-15.1.1/tutorforum/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 config = {
     "defaults": {
         "VERSION": __version__,
         "DOCKER_IMAGE": "{{ DOCKER_REGISTRY }}overhangio/openedx-forum:{{ FORUM_VERSION }}",
         "MONGODB_DATABASE": "cs_comments_service",
         "PORT": "4567",
         "API_KEY": "forumapikey",
+        "REPOSITORY": "https://github.com/openedx/cs_comments_service.git",
+        "REPOSITORY_VERSION": "{{ OPENEDX_COMMON_VERSION }}"
     },
 }
 
 tutor_hooks.Filters.COMMANDS_INIT.add_item((
     "forum",
     ("forum", "tasks", "forum", "init"),
 ))
```

### Comparing `tutor-forum-15.1.0/tutorforum/templates/forum/build/forum/Dockerfile` & `tutor-forum-15.1.1/tutorforum/templates/forum/build/forum/Dockerfile`

 * *Files 14% similar despite different names*

```diff
@@ -25,15 +25,19 @@
 # Install rake and bundler
 ENV PATH "/app/bin:/app/.gem/ruby/3.0.4/bin:$PATH"
 RUN gem install --user-install bundler --version 1.17.3
 RUN gem install --user-install rake --version 13.0.6
 
 # Install forum
 ENV BUNDLE_GEMFILE Gemfile3
-RUN git clone https://github.com/openedx/cs_comments_service.git --branch {{ OPENEDX_COMMON_VERSION }} --depth 1 /app/cs_comments_service
+
+ARG FORUM_REPOSITORY={{ FORUM_REPOSITORY }}
+ARG FORUM_REPOSITORY_VERSION={{ FORUM_REPOSITORY_VERSION }}
+RUN git clone $FORUM_REPOSITORY --branch $FORUM_REPOSITORY_VERSION --depth 1 /app/cs_comments_service
+
 WORKDIR /app/cs_comments_service
 RUN bundle install --deployment
 
 ENTRYPOINT ["docker-entrypoint.sh"]
 
 ENV SINATRA_ENV staging
 ENV NEW_RELIC_ENABLE false
```

### Comparing `tutor-forum-15.1.0/tutorforum/templates/forum/build/forum/bin/docker-entrypoint.sh` & `tutor-forum-15.1.1/tutorforum/templates/forum/build/forum/bin/docker-entrypoint.sh`

 * *Files identical despite different names*

