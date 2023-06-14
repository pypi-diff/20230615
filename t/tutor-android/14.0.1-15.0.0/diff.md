# Comparing `tmp/tutor-android-14.0.1.tar.gz` & `tmp/tutor-android-15.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tutor-android-14.0.1.tar", last modified: Fri Nov 25 15:34:39 2022, max compression
+gzip compressed data, was "dist/tutor-android-15.0.0.tar", last modified: Mon Dec 12 17:55:56 2022, max compression
```

## Comparing `tutor-android-14.0.1.tar` & `tutor-android-15.0.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-11-25 15:34:39.000000 tutor-android-14.0.1/
--rw-r--r--   0 ci        (1000) ci        (1000)       84 2022-11-25 15:34:34.000000 tutor-android-14.0.1/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)     4092 2022-11-25 15:34:39.000000 tutor-android-14.0.1/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     2588 2022-11-25 15:34:34.000000 tutor-android-14.0.1/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2022-11-25 15:34:39.000000 tutor-android-14.0.1/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     1837 2022-11-25 15:34:34.000000 tutor-android-14.0.1/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-11-25 15:34:39.000000 tutor-android-14.0.1/tutor_android.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)     4092 2022-11-25 15:34:39.000000 tutor-android-14.0.1/tutor_android.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     1011 2022-11-25 15:34:39.000000 tutor-android-14.0.1/tutor_android.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2022-11-25 15:34:39.000000 tutor-android-14.0.1/tutor_android.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       49 2022-11-25 15:34:39.000000 tutor-android-14.0.1/tutor_android.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       22 2022-11-25 15:34:39.000000 tutor-android-14.0.1/tutor_android.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       13 2022-11-25 15:34:39.000000 tutor-android-14.0.1/tutor_android.egg-info/top_level.txt
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-11-25 15:34:39.000000 tutor-android-14.0.1/tutorandroid/
--rw-r--r--   0 ci        (1000) ci        (1000)       23 2022-11-25 15:34:34.000000 tutor-android-14.0.1/tutorandroid/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2022-11-25 15:34:34.000000 tutor-android-14.0.1/tutorandroid/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-11-25 15:34:39.000000 tutor-android-14.0.1/tutorandroid/patches/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2022-11-25 15:34:34.000000 tutor-android-14.0.1/tutorandroid/patches/.gitignore
--rw-r--r--   0 ci        (1000) ci        (1000)       83 2022-11-25 15:34:34.000000 tutor-android-14.0.1/tutorandroid/patches/caddyfile
--rw-r--r--   0 ci        (1000) ci        (1000)      614 2022-11-25 15:34:34.000000 tutor-android-14.0.1/tutorandroid/patches/k8s-deployments
--rw-r--r--   0 ci        (1000) ci        (1000)      184 2022-11-25 15:34:34.000000 tutor-android-14.0.1/tutorandroid/patches/k8s-services
--rw-r--r--   0 ci        (1000) ci        (1000)      155 2022-11-25 15:34:34.000000 tutor-android-14.0.1/tutorandroid/patches/local-docker-compose-services
--rw-r--r--   0 ci        (1000) ci        (1000)     3624 2022-11-25 15:34:34.000000 tutor-android-14.0.1/tutorandroid/plugin.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-11-25 15:34:39.000000 tutor-android-14.0.1/tutorandroid/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-11-25 15:34:39.000000 tutor-android-14.0.1/tutorandroid/templates/android/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-11-25 15:34:39.000000 tutor-android-14.0.1/tutorandroid/templates/android/build/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2022-11-25 15:34:34.000000 tutor-android-14.0.1/tutorandroid/templates/android/build/.gitignore
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-11-25 15:34:39.000000 tutor-android-14.0.1/tutorandroid/templates/android/build/android/
--rw-r--r--   0 ci        (1000) ci        (1000)     1507 2022-11-25 15:34:34.000000 tutor-android-14.0.1/tutorandroid/templates/android/build/android/Dockerfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-11-25 15:34:39.000000 tutor-android-14.0.1/tutorandroid/templates/android/build/app/
--rw-r--r--   0 ci        (1000) ci        (1000)     1081 2022-11-25 15:34:34.000000 tutor-android-14.0.1/tutorandroid/templates/android/build/app/Dockerfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-11-25 15:34:39.000000 tutor-android-14.0.1/tutorandroid/templates/android/build/app/config/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2022-11-25 15:34:34.000000 tutor-android-14.0.1/tutorandroid/templates/android/build/app/config/.gitignore
--rw-r--r--   0 ci        (1000) ci        (1000)       49 2022-11-25 15:34:34.000000 tutor-android-14.0.1/tutorandroid/templates/android/build/app/config/edx.properties
--rw-r--r--   0 ci        (1000) ci        (1000)      233 2022-11-25 15:34:34.000000 tutor-android-14.0.1/tutorandroid/templates/android/build/app/config/gradle.properties
--rw-r--r--   0 ci        (1000) ci        (1000)      608 2022-11-25 15:34:34.000000 tutor-android-14.0.1/tutorandroid/templates/android/build/app/config/tutor.yaml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-11-25 15:34:39.000000 tutor-android-14.0.1/tutorandroid/templates/android/tasks/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2022-11-25 15:34:34.000000 tutor-android-14.0.1/tutorandroid/templates/android/tasks/.gitignore
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-11-25 15:34:39.000000 tutor-android-14.0.1/tutorandroid/templates/android/tasks/lms/
--rw-r--r--   0 ci        (1000) ci        (1000)      510 2022-11-25 15:34:34.000000 tutor-android-14.0.1/tutorandroid/templates/android/tasks/lms/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:55:56.000000 tutor-android-15.0.0/
+-rw-r--r--   0 ci        (1000) ci        (1000)       84 2022-12-12 17:55:50.000000 tutor-android-15.0.0/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     4088 2022-12-12 17:55:56.000000 tutor-android-15.0.0/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     2584 2022-12-12 17:55:50.000000 tutor-android-15.0.0/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2022-12-12 17:55:56.000000 tutor-android-15.0.0/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     1837 2022-12-12 17:55:50.000000 tutor-android-15.0.0/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:55:56.000000 tutor-android-15.0.0/tutor_android.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)     4088 2022-12-12 17:55:56.000000 tutor-android-15.0.0/tutor_android.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     1011 2022-12-12 17:55:56.000000 tutor-android-15.0.0/tutor_android.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2022-12-12 17:55:56.000000 tutor-android-15.0.0/tutor_android.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       49 2022-12-12 17:55:56.000000 tutor-android-15.0.0/tutor_android.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       22 2022-12-12 17:55:56.000000 tutor-android-15.0.0/tutor_android.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       13 2022-12-12 17:55:56.000000 tutor-android-15.0.0/tutor_android.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:55:56.000000 tutor-android-15.0.0/tutorandroid/
+-rw-r--r--   0 ci        (1000) ci        (1000)       24 2022-12-12 17:55:50.000000 tutor-android-15.0.0/tutorandroid/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2022-12-12 17:55:50.000000 tutor-android-15.0.0/tutorandroid/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:55:56.000000 tutor-android-15.0.0/tutorandroid/patches/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2022-12-12 17:55:50.000000 tutor-android-15.0.0/tutorandroid/patches/.gitignore
+-rw-r--r--   0 ci        (1000) ci        (1000)       83 2022-12-12 17:55:50.000000 tutor-android-15.0.0/tutorandroid/patches/caddyfile
+-rw-r--r--   0 ci        (1000) ci        (1000)      614 2022-12-12 17:55:50.000000 tutor-android-15.0.0/tutorandroid/patches/k8s-deployments
+-rw-r--r--   0 ci        (1000) ci        (1000)      184 2022-12-12 17:55:50.000000 tutor-android-15.0.0/tutorandroid/patches/k8s-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      155 2022-12-12 17:55:50.000000 tutor-android-15.0.0/tutorandroid/patches/local-docker-compose-services
+-rw-r--r--   0 ci        (1000) ci        (1000)     4000 2022-12-12 17:55:50.000000 tutor-android-15.0.0/tutorandroid/plugin.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:55:56.000000 tutor-android-15.0.0/tutorandroid/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:55:56.000000 tutor-android-15.0.0/tutorandroid/templates/android/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:55:56.000000 tutor-android-15.0.0/tutorandroid/templates/android/build/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2022-12-12 17:55:50.000000 tutor-android-15.0.0/tutorandroid/templates/android/build/.gitignore
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:55:56.000000 tutor-android-15.0.0/tutorandroid/templates/android/build/android/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1519 2022-12-12 17:55:50.000000 tutor-android-15.0.0/tutorandroid/templates/android/build/android/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:55:56.000000 tutor-android-15.0.0/tutorandroid/templates/android/build/app/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1081 2022-12-12 17:55:50.000000 tutor-android-15.0.0/tutorandroid/templates/android/build/app/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:55:56.000000 tutor-android-15.0.0/tutorandroid/templates/android/build/app/config/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2022-12-12 17:55:50.000000 tutor-android-15.0.0/tutorandroid/templates/android/build/app/config/.gitignore
+-rw-r--r--   0 ci        (1000) ci        (1000)       49 2022-12-12 17:55:50.000000 tutor-android-15.0.0/tutorandroid/templates/android/build/app/config/edx.properties
+-rw-r--r--   0 ci        (1000) ci        (1000)      233 2022-12-12 17:55:50.000000 tutor-android-15.0.0/tutorandroid/templates/android/build/app/config/gradle.properties
+-rw-r--r--   0 ci        (1000) ci        (1000)      608 2022-12-12 17:55:50.000000 tutor-android-15.0.0/tutorandroid/templates/android/build/app/config/tutor.yaml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:55:56.000000 tutor-android-15.0.0/tutorandroid/templates/android/tasks/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2022-12-12 17:55:50.000000 tutor-android-15.0.0/tutorandroid/templates/android/tasks/.gitignore
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:55:56.000000 tutor-android-15.0.0/tutorandroid/templates/android/tasks/lms/
+-rw-r--r--   0 ci        (1000) ci        (1000)      510 2022-12-12 17:55:50.000000 tutor-android-15.0.0/tutorandroid/templates/android/tasks/lms/init
```

### Comparing `tutor-android-14.0.1/PKG-INFO` & `tutor-android-15.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: tutor-android
-Version: 14.0.1
+Version: 15.0.0
 Summary: Android mobile app plugin for Tutor
 Home-page: https://github.com/overhangio/tutor-android
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: Overhang.IO
 Maintainer-email: regis@overhang.io
 License: AGPLv3
@@ -25,15 +25,15 @@
         
         Usage
         -----
         
         Enable the plugin and start the platform::
         
             tutor plugins enable android
-            tutor local quickstart
+            tutor local launch
         
         
         The ``.apk`` file will then be available for download at http(s)://mobile.LMS_HOST/app.apk. When running locally, this will be: http://mobile.local.overhang.io/app.apk. You can forward this address to your students for download.
         
         Building a custom Android app
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `tutor-android-14.0.1/README.rst` & `tutor-android-15.0.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 Usage
 -----
 
 Enable the plugin and start the platform::
 
     tutor plugins enable android
-    tutor local quickstart
+    tutor local launch
 
 
 The ``.apk`` file will then be available for download at http(s)://mobile.LMS_HOST/app.apk. When running locally, this will be: http://mobile.local.overhang.io/app.apk. You can forward this address to your students for download.
 
 Building a custom Android app
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `tutor-android-14.0.1/setup.py` & `tutor-android-15.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     maintainer="Overhang.IO",
     maintainer_email="regis@overhang.io",
     description="Android mobile app plugin for Tutor",
     long_description=load_readme(),
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
     python_requires=">=3.7",
-    install_requires=["tutor>=14.0.0,<15.0.0"],
+    install_requires=["tutor>=15.0.0,<16.0.0"],
     entry_points={
         "tutor.plugin.v1": [
             "android = tutorandroid.plugin"
         ]
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
```

### Comparing `tutor-android-14.0.1/tutor_android.egg-info/PKG-INFO` & `tutor-android-15.0.0/tutor_android.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: tutor-android
-Version: 14.0.1
+Version: 15.0.0
 Summary: Android mobile app plugin for Tutor
 Home-page: https://github.com/overhangio/tutor-android
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: Overhang.IO
 Maintainer-email: regis@overhang.io
 License: AGPLv3
@@ -25,15 +25,15 @@
         
         Usage
         -----
         
         Enable the plugin and start the platform::
         
             tutor plugins enable android
-            tutor local quickstart
+            tutor local launch
         
         
         The ``.apk`` file will then be available for download at http(s)://mobile.LMS_HOST/app.apk. When running locally, this will be: http://mobile.local.overhang.io/app.apk. You can forward this address to your students for download.
         
         Building a custom Android app
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `tutor-android-14.0.1/tutor_android.egg-info/SOURCES.txt` & `tutor-android-15.0.0/tutor_android.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tutor-android-14.0.1/tutorandroid/patches/k8s-deployments` & `tutor-android-15.0.0/tutorandroid/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-android-14.0.1/tutorandroid/plugin.py` & `tutor-android-15.0.0/tutorandroid/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,30 +7,42 @@
 from .__about__ import __version__
 
 config = {
     "unique": {"OAUTH2_SECRET": "{{ 24|random_string }}"},
     "defaults": {
         "VERSION": __version__,
         "APP_HOST": "mobile.{{ LMS_HOST }}",
-        "APP_VERSION": "3.0.2",  # https://github.com/edx/edx-app-android/releases
+        # Unfortunately 3.2.2 is not functional: https://github.com/openedx/build-test-release-wg/issues/211#issuecomment-1344311500
+        # "APP_VERSION": "3.2.2",  # https://github.com/openedx/edx-app-android/releases
+        "APP_VERSION": "3.0.2",
         "DOCKER_IMAGE": "{{ DOCKER_REGISTRY }}overhangio/openedx-android:{{ ANDROID_VERSION }}",
         "APP_DOCKER_IMAGE": "{{ DOCKER_REGISTRY }}overhangio/openedx-android-app:{{ ANDROID_VERSION }}",
         "ENABLE_RELEASE_MODE": False,
         "RELEASE_STORE_PASSWORD": "android store password",
         "RELEASE_KEY_PASSWORD": "android release key password",
         "RELEASE_KEY_ALIAS": "android release key alias",
     },
 }
 
-tutor_hooks.Filters.COMMANDS_INIT.add_item(
-    (
+with open(
+    os.path.join(
+        pkg_resources.resource_filename("tutorandroid", "templates"),
+        "android",
+        "tasks",
         "lms",
-        ("android", "tasks", "lms", "init"),
+        "init",
+    ),
+    encoding="utf8",
+) as fi:
+    tutor_hooks.Filters.CLI_DO_INIT_TASKS.add_item(
+        (
+            "lms",
+            fi.read(),
+        )
     )
-)
 tutor_hooks.Filters.IMAGES_BUILD.add_items(
     [
         (
             "android",
             ("plugins", "android", "build", "android"),
             "{{ ANDROID_DOCKER_IMAGE }}",
             (),
```

### Comparing `tutor-android-14.0.1/tutorandroid/templates/android/build/android/Dockerfile` & `tutor-android-15.0.0/tutorandroid/templates/android/build/android/Dockerfile`

 * *Files 4% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 # Inspired from https://github.com/LiveXP/docker-android-sdk/blob/master/Dockerfile
 # Get sdk version from here: https://developer.android.com/studio#command-tools
 ENV ANDROID_SDK_VERSION 7583922
 ENV ANDROID_SDK_PATH /app/android-sdk
 ENV ANDROID_HOME /app/android-sdk
 RUN mkdir ${ANDROID_HOME}
 WORKDIR /app/android-sdk
-RUN wget https://dl.google.com/android/repository/commandlinetools-linux-${ANDROID_SDK_VERSION}_latest.zip && \
+RUN wget --quiet https://dl.google.com/android/repository/commandlinetools-linux-${ANDROID_SDK_VERSION}_latest.zip && \
     unzip commandlinetools-linux-${ANDROID_SDK_VERSION}_latest.zip && \
     rm commandlinetools-linux-${ANDROID_SDK_VERSION}_latest.zip
 
 # Accept licenses
 # https://developer.android.com/studio/command-line/sdkmanager
 # Check target version: https://github.com/edx/edx-app-android/blob/master/constants.gradle
 ARG ANDROID_API_LEVEL=30
 RUN yes | /app/android-sdk/cmdline-tools/bin/sdkmanager --sdk_root=${ANDROID_HOME} --install "platforms;android-$ANDROID_API_LEVEL" 1> /dev/null
 
 # Install android app repo
-ARG ANDROID_APP_REPOSITORY=https://github.com/edx/edx-app-android
+ARG ANDROID_APP_REPOSITORY=https://github.com/openedx/edx-app-android
 ARG ANDROID_APP_VERSION=release/{{ ANDROID_APP_VERSION }}
 RUN git clone $ANDROID_APP_REPOSITORY --branch $ANDROID_APP_VERSION /app/edx-app-android
 WORKDIR /app/edx-app-android
 
 # Install gradle and all dependencies
 RUN ./gradlew -v
 RUN ./gradlew tasks
```

### Comparing `tutor-android-14.0.1/tutorandroid/templates/android/build/app/Dockerfile` & `tutor-android-15.0.0/tutorandroid/templates/android/build/app/Dockerfile`

 * *Files 8% similar despite different names*

```diff
@@ -11,10 +11,10 @@
 {% endif %}
 
 RUN sed -i "s/APPLICATION_ID = .*/APPLICATION_ID = \"{{ LMS_HOST|reverse_host|replace("-", "_") }}\"/g" constants.gradle
 RUN ./gradlew assembleProd{{ "Release" if ANDROID_ENABLE_RELEASE_MODE else "Debuggable" }}
 
 #### File server to serve apk file
 # https://hub.docker.com/_/caddy?tab=tags
-FROM docker.io/caddy:2.5.1-alpine as production
+FROM docker.io/caddy:2.6.2-alpine as production
 COPY --from=build /app/edx-app-android/OpenEdXMobile/build/outputs/apk/prod/{{ "release" if ANDROID_ENABLE_RELEASE_MODE else "debuggable" }}/edx-{{ "release" if ANDROID_ENABLE_RELEASE_MODE else "debuggable" }}-{{ ANDROID_APP_VERSION }}.apk /srv/app.apk
 CMD caddy file-server --listen=:8000 --root=/srv
```

### Comparing `tutor-android-14.0.1/tutorandroid/templates/android/build/app/config/tutor.yaml` & `tutor-android-15.0.0/tutorandroid/templates/android/build/app/config/tutor.yaml`

 * *Files identical despite different names*

