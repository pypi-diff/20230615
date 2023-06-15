# Comparing `tmp/politico-staff-auth-0.0.5.tar.gz` & `tmp/politico-staff-auth-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/politico-staff-auth-0.0.5.tar", last modified: Mon Sep 23 20:18:19 2019, max compression
+gzip compressed data, was "politico-staff-auth-0.0.6.tar", last modified: Thu Jun 15 03:01:29 2023, max compression
```

## Comparing `politico-staff-auth-0.0.5.tar` & `politico-staff-auth-0.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 ajvestal (1314301173) 1534107694        0 2019-09-23 20:18:19.000000 politico-staff-auth-0.0.5/
--rw-r--r--   0 ajvestal (1314301173) 1534107694    12722 2019-09-23 20:18:19.000000 politico-staff-auth-0.0.5/PKG-INFO
--rw-r--r--   0 ajvestal (1314301173) 1534107694     1061 2019-09-17 18:15:53.000000 politico-staff-auth-0.0.5/LICENSE
--rw-r--r--   0 ajvestal (1314301173) 1534107694      113 2019-09-18 19:07:48.000000 politico-staff-auth-0.0.5/MANIFEST.in
--rw-r--r--   0 ajvestal (1314301173) 1534107694     9753 2019-09-18 17:58:44.000000 politico-staff-auth-0.0.5/README.md
--rw-r--r--   0 ajvestal (1314301173) 1534107694     1490 2019-09-17 18:53:08.000000 politico-staff-auth-0.0.5/setup.py
-drwxr-xr-x   0 ajvestal (1314301173) 1534107694        0 2019-09-23 20:18:19.000000 politico-staff-auth-0.0.5/politico_staff_auth.egg-info/
--rw-r--r--   0 ajvestal (1314301173) 1534107694    12722 2019-09-23 20:18:19.000000 politico-staff-auth-0.0.5/politico_staff_auth.egg-info/PKG-INFO
--rw-r--r--   0 ajvestal (1314301173) 1534107694      632 2019-09-23 20:18:19.000000 politico-staff-auth-0.0.5/politico_staff_auth.egg-info/SOURCES.txt
--rw-r--r--   0 ajvestal (1314301173) 1534107694       70 2019-09-23 20:18:19.000000 politico-staff-auth-0.0.5/politico_staff_auth.egg-info/requires.txt
--rw-r--r--   0 ajvestal (1314301173) 1534107694       11 2019-09-23 20:18:19.000000 politico-staff-auth-0.0.5/politico_staff_auth.egg-info/top_level.txt
--rw-r--r--   0 ajvestal (1314301173) 1534107694        1 2019-09-23 20:18:19.000000 politico-staff-auth-0.0.5/politico_staff_auth.egg-info/dependency_links.txt
--rw-r--r--   0 ajvestal (1314301173) 1534107694      108 2019-09-23 20:18:19.000000 politico-staff-auth-0.0.5/setup.cfg
-drwxr-xr-x   0 ajvestal (1314301173) 1534107694        0 2019-09-23 20:18:19.000000 politico-staff-auth-0.0.5/staff_auth/
--rw-r--r--   0 ajvestal (1314301173) 1534107694      733 2019-09-23 20:17:50.000000 politico-staff-auth-0.0.5/staff_auth/backend.py
--rw-r--r--   0 ajvestal (1314301173) 1534107694       80 2019-09-23 20:00:58.000000 politico-staff-auth-0.0.5/staff_auth/__init__.py
--rw-r--r--   0 ajvestal (1314301173) 1534107694      176 2019-09-17 17:32:51.000000 politico-staff-auth-0.0.5/staff_auth/apps.py
--rw-r--r--   0 ajvestal (1314301173) 1534107694      556 2019-09-18 19:17:39.000000 politico-staff-auth-0.0.5/staff_auth/pipeline.py
-drwxr-xr-x   0 ajvestal (1314301173) 1534107694        0 2019-09-23 20:18:19.000000 politico-staff-auth-0.0.5/staff_auth/static/
-drwxr-xr-x   0 ajvestal (1314301173) 1534107694        0 2019-09-23 20:18:19.000000 politico-staff-auth-0.0.5/staff_auth/static/staff_auth/
-drwxr-xr-x   0 ajvestal (1314301173) 1534107694        0 2019-09-23 20:18:19.000000 politico-staff-auth-0.0.5/staff_auth/static/staff_auth/css/
--rw-r--r--   0 ajvestal (1314301173) 1534107694     6075 2019-09-17 17:36:00.000000 politico-staff-auth-0.0.5/staff_auth/static/staff_auth/css/page-styles.css
--rw-r--r--   0 ajvestal (1314301173) 1534107694     1259 2019-09-17 17:35:52.000000 politico-staff-auth-0.0.5/staff_auth/static/staff_auth/css/custom-login.css
-drwxr-xr-x   0 ajvestal (1314301173) 1534107694        0 2019-09-23 20:18:19.000000 politico-staff-auth-0.0.5/staff_auth/templates/
-drwxr-xr-x   0 ajvestal (1314301173) 1534107694        0 2019-09-23 20:18:19.000000 politico-staff-auth-0.0.5/staff_auth/templates/admin/
--rw-r--r--   0 ajvestal (1314301173) 1534107694     2055 2019-09-17 18:59:54.000000 politico-staff-auth-0.0.5/staff_auth/templates/admin/login.html
-drwxr-xr-x   0 ajvestal (1314301173) 1534107694        0 2019-09-23 20:18:19.000000 politico-staff-auth-0.0.5/staff_auth/templates/staff_auth/
--rw-r--r--   0 ajvestal (1314301173) 1534107694     3641 2019-09-18 19:16:18.000000 politico-staff-auth-0.0.5/staff_auth/templates/staff_auth/auth-error.html
--rw-r--r--   0 ajvestal (1314301173) 1534107694     1179 2019-09-18 17:13:14.000000 politico-staff-auth-0.0.5/staff_auth/configured_settings.py
--rw-r--r--   0 ajvestal (1314301173) 1534107694      455 2019-09-17 17:32:07.000000 politico-staff-auth-0.0.5/staff_auth/urls.py
--rw-r--r--   0 ajvestal (1314301173) 1534107694     1130 2019-09-18 19:06:15.000000 politico-staff-auth-0.0.5/staff_auth/middleware.py
--rw-r--r--   0 ajvestal (1314301173) 1534107694      608 2019-09-18 17:46:53.000000 politico-staff-auth-0.0.5/staff_auth/views.py
+drwxr-xr-x   0 ajvestal   (503) staff       (20)        0 2023-06-15 03:01:29.579468 politico-staff-auth-0.0.6/
+-rw-r--r--   0 ajvestal   (503) staff       (20)     1061 2023-06-15 01:07:55.000000 politico-staff-auth-0.0.6/LICENSE
+-rw-r--r--   0 ajvestal   (503) staff       (20)      113 2023-06-15 01:07:55.000000 politico-staff-auth-0.0.6/MANIFEST.in
+-rw-r--r--   0 ajvestal   (503) staff       (20)    10877 2023-06-15 03:01:29.579571 politico-staff-auth-0.0.6/PKG-INFO
+-rw-r--r--   0 ajvestal   (503) staff       (20)     9997 2023-06-15 02:59:42.000000 politico-staff-auth-0.0.6/README.md
+drwxr-xr-x   0 ajvestal   (503) staff       (20)        0 2023-06-15 03:01:29.576549 politico-staff-auth-0.0.6/politico_staff_auth.egg-info/
+-rw-r--r--   0 ajvestal   (503) staff       (20)    10877 2023-06-15 03:01:29.000000 politico-staff-auth-0.0.6/politico_staff_auth.egg-info/PKG-INFO
+-rw-r--r--   0 ajvestal   (503) staff       (20)      632 2023-06-15 03:01:29.000000 politico-staff-auth-0.0.6/politico_staff_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 ajvestal   (503) staff       (20)        1 2023-06-15 03:01:29.000000 politico-staff-auth-0.0.6/politico_staff_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 ajvestal   (503) staff       (20)       70 2023-06-15 03:01:29.000000 politico-staff-auth-0.0.6/politico_staff_auth.egg-info/requires.txt
+-rw-r--r--   0 ajvestal   (503) staff       (20)       11 2023-06-15 03:01:29.000000 politico-staff-auth-0.0.6/politico_staff_auth.egg-info/top_level.txt
+-rw-r--r--   0 ajvestal   (503) staff       (20)      108 2023-06-15 03:01:29.579942 politico-staff-auth-0.0.6/setup.cfg
+-rw-r--r--   0 ajvestal   (503) staff       (20)     1490 2023-06-15 01:07:55.000000 politico-staff-auth-0.0.6/setup.py
+drwxr-xr-x   0 ajvestal   (503) staff       (20)        0 2023-06-15 03:01:29.578533 politico-staff-auth-0.0.6/staff_auth/
+-rw-r--r--   0 ajvestal   (503) staff       (20)       80 2023-06-15 02:34:24.000000 politico-staff-auth-0.0.6/staff_auth/__init__.py
+-rw-r--r--   0 ajvestal   (503) staff       (20)      176 2023-06-15 01:07:55.000000 politico-staff-auth-0.0.6/staff_auth/apps.py
+-rw-r--r--   0 ajvestal   (503) staff       (20)      733 2023-06-15 01:07:55.000000 politico-staff-auth-0.0.6/staff_auth/backend.py
+-rw-r--r--   0 ajvestal   (503) staff       (20)     1179 2023-06-15 01:07:55.000000 politico-staff-auth-0.0.6/staff_auth/configured_settings.py
+-rw-r--r--   0 ajvestal   (503) staff       (20)     1130 2023-06-15 01:07:55.000000 politico-staff-auth-0.0.6/staff_auth/middleware.py
+-rw-r--r--   0 ajvestal   (503) staff       (20)     1837 2023-06-15 03:00:39.000000 politico-staff-auth-0.0.6/staff_auth/pipeline.py
+drwxr-xr-x   0 ajvestal   (503) staff       (20)        0 2023-06-15 03:01:29.574300 politico-staff-auth-0.0.6/staff_auth/static/
+drwxr-xr-x   0 ajvestal   (503) staff       (20)        0 2023-06-15 03:01:29.574361 politico-staff-auth-0.0.6/staff_auth/static/staff_auth/
+drwxr-xr-x   0 ajvestal   (503) staff       (20)        0 2023-06-15 03:01:29.578911 politico-staff-auth-0.0.6/staff_auth/static/staff_auth/css/
+-rw-r--r--   0 ajvestal   (503) staff       (20)     1259 2023-06-15 01:07:55.000000 politico-staff-auth-0.0.6/staff_auth/static/staff_auth/css/custom-login.css
+-rw-r--r--   0 ajvestal   (503) staff       (20)     6075 2023-06-15 01:07:55.000000 politico-staff-auth-0.0.6/staff_auth/static/staff_auth/css/page-styles.css
+drwxr-xr-x   0 ajvestal   (503) staff       (20)        0 2023-06-15 03:01:29.574635 politico-staff-auth-0.0.6/staff_auth/templates/
+drwxr-xr-x   0 ajvestal   (503) staff       (20)        0 2023-06-15 03:01:29.579104 politico-staff-auth-0.0.6/staff_auth/templates/admin/
+-rw-r--r--   0 ajvestal   (503) staff       (20)     2055 2023-06-15 01:07:55.000000 politico-staff-auth-0.0.6/staff_auth/templates/admin/login.html
+drwxr-xr-x   0 ajvestal   (503) staff       (20)        0 2023-06-15 03:01:29.579297 politico-staff-auth-0.0.6/staff_auth/templates/staff_auth/
+-rw-r--r--   0 ajvestal   (503) staff       (20)     3641 2023-06-15 01:07:55.000000 politico-staff-auth-0.0.6/staff_auth/templates/staff_auth/auth-error.html
+-rw-r--r--   0 ajvestal   (503) staff       (20)      455 2023-06-15 01:07:55.000000 politico-staff-auth-0.0.6/staff_auth/urls.py
+-rw-r--r--   0 ajvestal   (503) staff       (20)      608 2023-06-15 01:07:55.000000 politico-staff-auth-0.0.6/staff_auth/views.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `politico-staff-auth-0.0.5/PKG-INFO` & `politico-staff-auth-0.0.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,284 +1,288 @@
 Metadata-Version: 2.1
 Name: politico-staff-auth
-Version: 0.0.5
+Version: 0.0.6
 Summary: Staff authentication via Slack, the POLITICO way.
 Home-page: https://github.com/The-Politico/politico-staff-auth/
 Author: POLITICO interactive news
 Author-email: interactives@politico.com
 License: MIT
-Description: ![POLITICO](https://politico.com/interactives/cdn/images/badge.svg)
-        
-        ```
-                  __          _____  _____                 __  .__         
-          _______/  |______ _/ ____\/ ____\ _____   __ ___/  |_|  |__      
-         /  ___/\   __\__  \\   __\\   __\  \__  \ |  |  \   __\  |  \     
-         \___ \  |  |  / __ \|  |   |  |     / __ \|  |  /|  | |   Y  \    
-        /____  > |__| (____  /__|   |__|    (____  /____/ |__| |___|  / /\
-             \/            \/                    \/                 \/  \/
-        ```
-        
-        # POLITICO staff auth
-        
-        This app stores a handful of useful utilities we use across our various Django apps at POLITICO to integrate our staff authorization and authentication, which is implemented with Slack via [`Python Social Auth`](https://python-social-auth.readthedocs.io/).
-        
-        
-        ## Requirements
-        
-        - Python 3.6 — `brew install python`
-        
-        - Pipenv — `brew install pipenv`
-        
-        - Django (tested on versions 2.1.x and 2.2.x)
-        
-        - A Slack workspace with users
-        
-        - A Slack app connected to that workspace, with a "Redirect URL" entry matching the following pattern:
-        
-          `http://<your server name>/social/complete/slack/`
-        
-          (**Note:** you can have multiple "Redirect URLs" for the same app. For local development, you'll be aliasing `localhost` to a subdomain of your choosing, as described in the ["Domain resolution"](#domain-resolution) section below.)
-        
-        - _Optional:_ PostgreSQL — `brew install postgresql`
-        
-        
-        ## What's inside
-        
-        #### `./staff_auth/`
-        
-        The app that handles staff Slack authorization and authentication.
-        
-        ###### `./staff_auth/templates/admin/login.html` and `./staff_auth/static/staff_auth/css/custom-login.css`
-        
-        Custom HTML and CSS to add a "Staff login (with Slack)" button to the standard Django admin login form.
-        
-        ###### `staff_auth.backend.WorkspaceSpecificSlackOAuth2`
-        
-        A subclass of Python Social Auth's Slack authentication backend. Unlike the original, this variant forces users to log in with credentials from the specified Slack workspace (rather than from any Slack workspace).
-        
-        ###### `staff_auth.middleware.InvalidWorkspaceErrorMiddleware`
-        
-        A middleware that listens for Python Social Auth's `AuthForbidden` exceptions and maps them to rich output in a [`StaffAuthErrorView`](#staff_authviewsstaffautherrorview) page.
-        
-        ###### `staff_auth.pipeline.promote_staffer_to_staff`
-        
-        A function that promotes all Slack-authenticated users to "staff" status (meaning they can log into the Django admin) when they first sign in with their Slack credentials.
-        
-        ###### `staff_auth.pipeline.promote_manager_to_superuser`
-        
-        A function that promotes all Slack-authenticated users to "superuser" status (meaning they can log into the Django admin) when they first sign in with their Slack credentials — if the email address on their Slack account matches an email address found in the `settings.MANAGERS` list.
-        
-        ###### `staff_auth.views.StaffAuthErrorView`
-        
-        An error page shown to users if they try and log in via a different Slack workspace.
-        
-        (Note that the HTML and CSS for this view live at `./staff_auth/templates/staff_auth/auth-error.html` and `./staff_auth/static/staff_auth/css/page-styles.css`, respectively.)
-        
-        #### `./example/`
-        
-        An example Django project that shows how we implement staff Slack access.
-        
-        Inside this directory you'll find a standard (if threadbare) Django app, with an example `.env` file, a `Pipfile` and a `manage.py` script at the top level.
-        
-        Inside the `exampleapp` subdirectory is this example app's `settings.py` file (where you can see an example implementation of `politico-staff-auth`'s required configuration variables), along with a `urls.py` file to demonstrate how that piece of wiring should be performed. Standard helper files including `wsgi.py` can also be found in this subdirectory.
-        
-        
-        ## Launching the example app
-        
-        1.  Change into the `./example/` directory one level below this README and install dependencies.
-        
-            ```sh
-            cd ./example/
-            pipenv install
-            ```
-        
-        2.  Create a `.env` file from the `.env.example` template, and insert appropriate values.
-        
-            ```sh
-            cp .env.example .env
-            ```
-        
-            See the ["Configuration"](#configuration) section below for more information about what goes in each setting.
-        
-        3.  Create a new blank database, then populate it with the necessary tables.
-        
-            ```sh
-            make database
-            pipenv run python manage.py migrate
-            ```
-        
-        4.  Start the Django test server.
-        
-            ```sh
-            pipenv run python manage.py runserver
-            ```
-        
-        5.  Navigate to [the admin site on your test server](http://local-dev.politicoapps.com:8000/admin/) and click the "Staff login" button.
-        
-        ## Installation
-        
-        1.  Install from PyPI:
-        
-            ```sh
-            pipenv install politico-staff-auth
-            ```
-        
-        2.  Add `staff_auth` and `social_django` to the list of apps installed into Django.
-        
-            _In your project's `settings.py`:_
-        
-            ```python
-            INSTALLED_APPS = [
-              "staff_auth",
-        
-              # ...
-              # Existing installed apps
-              # ...
-        
-              "social_django",
-            ]
-            ```
-        
-            **NOTE:** The `staff_auth` app must be first in this list (or, at least, must appear before the pre-existing line `django.contrib.admin`). The `social_django` line should appear after all apps that are distributed with Django itself.
-        
-        3.  Add the credentials for your staff's Slack workspace.
-        
-            _In your project's `settings.py`:_
-        
-            ```python
-            STAFF_AUTH_SLACK_KEY = "auth-key"
-        
-            STAFF_AUTH_SLACK_SECRET = "secret-key"
-        
-            STAFF_AUTH_SLACK_TEAM = "my-value-here"
-            ```
-        
-            For more on these values, see the ["Configuration"](#configuration) section below.
-        
-            **NOTE:** We recommend reading these values from environment variables, but there's no accounting for taste.
-        
-        4.  Add the required middleware for rich login error messages.
-        
-            _In your project's `settings.py`:_
-        
-            ```python
-            MIDDLEWARE = [
-                # ...
-                # Existing middleware
-                # ...
-        
-                "staff_auth.middleware.InvalidWorkspaceErrorMiddleware",
-            ]
-            ```
-        
-            **NOTE:** The `staff_auth.middleware.InvalidWorkspaceErrorMiddleware` entry should go at the end of the existing `MIDDLEWARE` list.
-        
-        5.  With the previous steps complete, you can now implement the basic staff auth settings.
-        
-            _In your project's `settings.py`:_
-        
-            ```python
-            from staff_auth.configured_settings import configure_staff_auth
-        
-            staff_auth_settings = configure_staff_auth(
-                key=STAFF_AUTH_SLACK_KEY,
-                secret=STAFF_AUTH_SLACK_SECRET,
-                team=STAFF_AUTH_SLACK_TEAM,
-            )
-        
-            for setting_name, setting_value in staff_auth_settings.items():
-                globals()[setting_name] = setting_value
-            ```
-        
-        6.  Set Django to use the Slack auth backend whenever users are asked to log in.
-        
-            _In your project's `settings.py`:_
-        
-            ```python
-            LOGIN_URL = "staff_auth:slack-login"
-            ```
-        
-        7.  Wire up the `staff_auth` and `social_django` URLs.
-        
-            _In your project's top-level URLconf (`urls.py` file):_
-        
-            ```python
-            urlpatterns = [
-              # ...
-              # Existing URL patterns
-              # ...
-        
-              path("social/", include("social_django.urls", namespace="social")),
-              path("staff-auth/", include("staff_auth.urls")),
-            ]
-            ```
-        
-        
-        8.  _**Optional:**_ Add pipelines.
-        
-            _In your project's `settings.py`:_
-        
-            ```python
-            SOCIAL_AUTH_PIPELINE = (
-                "social_core.pipeline.social_auth.social_details",
-                "social_core.pipeline.social_auth.social_uid",
-                "social_core.pipeline.social_auth.auth_allowed",
-                "social_core.pipeline.social_auth.social_user",
-                "social_core.pipeline.user.get_username",
-                "social_core.pipeline.user.create_user",
-                "social_core.pipeline.social_auth.associate_user",
-                "social_core.pipeline.social_auth.load_extra_data",
-                "staff_auth.pipeline.promote_staffer_to_staff",
-                "staff_auth.pipeline.promote_manager_to_superuser",
-                "social_core.pipeline.user.user_details",
-            )
-            ```
-        
-            You can disable either or both of the `staff_auth.pipeline` classes listed above, but please take care to preserve the order seen here — re-ordering these pipelines could produce unintended and hard-to-debug consequences.
-        
-            **NOTE:** The behaviors of `staff_auth.pipeline.promote_staffer_to_staff` and `staff_auth.pipeline.promote_manager_to_superuser` are described in the ["What's inside"](#whats-inside) section above.
-        
-            **NOTE 2:** If you're not using either `staff_auth.pipeline` class, skip this step and ensure your project's `settings.py` file has no `SOCIAL_AUTH_PIPELINE` value set.
-        
-        9.  _**Optional:**_ Modify the URLs where users are bounced to when they successfully log in or log out.
-        
-            These are standard Django settings, and can take either URLs or named URL patterns (as you would pass to the `{% url %}` template tag).
-        
-            _In your project's `settings.py`:_
-        
-            ```python
-            LOGIN_REDIRECT_URL = "/my/url/pattern/"
-        
-            LOGOUT_REDIRECT_URL = "/namespace:view-name/"
-            ```
-        
-            **NOTE:** For more information, see the Django documentation entries [here](https://docs.djangoproject.com/en/2.2/ref/settings/#login-redirect-url) and [here](https://docs.djangoproject.com/en/2.2/ref/settings/#logout-redirect-url).
-        
-        
-        ## Configuration
-        
-        | Setting | What it does |
-        |:--|:--|
-        | `STAFF_AUTH_SLACK_KEY` | The **'Client ID'** from the Slack "app" you've connected to your workspace for authenticating users. Passed to Python Social Auth as `SOCIAL_AUTH_SLACK_KEY`. |
-        | `STAFF_AUTH_SLACK_SECRET` | The `Client Secret` from this Slack "app". Passed to Python Social Auth as `SOCIAL_AUTH_SLACK_SECRET`. |
-        | `STAFF_AUTH_SLACK_TEAM` | The name of the Slack workspace where your users have accounts. (A handy way of remembering this: it's also the subdomain of slack.com where users log in to use Slack itself.) Passed to Python Social Auth as `SOCIAL_AUTH_SLACK_TEAM`. |
-        
-        
-        ## Copyright
-        
-        &copy; 2019&ndash;present POLITICO LLC
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Internet :: WWW/HTTP
 Description-Content-Type: text/markdown
-Provides-Extra: test
 Provides-Extra: dev
+Provides-Extra: test
+License-File: LICENSE
+
+![POLITICO](https://politico.com/interactives/cdn/images/badge.svg)
+
+```
+          __          _____  _____                 __  .__
+  _______/  |______ _/ ____\/ ____\ _____   __ ___/  |_|  |__
+ /  ___/\   __\__  \\   __\\   __\  \__  \ |  |  \   __\  |  \
+ \___ \  |  |  / __ \|  |   |  |     / __ \|  |  /|  | |   Y  \
+/____  > |__| (____  /__|   |__|    (____  /____/ |__| |___|  / /\
+     \/            \/                    \/                 \/  \/
+```
+
+# POLITICO staff auth
+
+This app stores a handful of useful utilities we use across our various Django apps at POLITICO to integrate our staff authorization and authentication, which is implemented with Slack via [`Python Social Auth`](https://python-social-auth.readthedocs.io/).
+
+
+## Requirements
+
+- Python 3.6 — `brew install python`
+
+- Pipenv — `brew install pipenv`
+
+- Django (tested on versions 2.1.x and 2.2.x)
+
+- A Slack workspace with users
+
+- A Slack app connected to that workspace, with a "Redirect URL" entry matching the following pattern:
+
+  `http://<your server name>/social/complete/slack/`
+
+  (**Note:** you can have multiple "Redirect URLs" for the same app. For local development, you'll be aliasing `localhost` to a subdomain of your choosing, as described in the ["Domain resolution"](#domain-resolution) section below.)
+
+- _Optional:_ PostgreSQL — `brew install postgresql`
+
+
+## What's inside
+
+#### `./staff_auth/`
+
+The app that handles staff Slack authorization and authentication.
+
+###### `./staff_auth/templates/admin/login.html` and `./staff_auth/static/staff_auth/css/custom-login.css`
+
+Custom HTML and CSS to add a "Staff login (with Slack)" button to the standard Django admin login form.
+
+###### `staff_auth.backend.WorkspaceSpecificSlackOAuth2`
+
+A subclass of Python Social Auth's Slack authentication backend. Unlike the original, this variant forces users to log in with credentials from the specified Slack workspace (rather than from any Slack workspace).
+
+###### `staff_auth.middleware.InvalidWorkspaceErrorMiddleware`
+
+A middleware that listens for Python Social Auth's `AuthForbidden` exceptions and maps them to rich output in a [`StaffAuthErrorView`](#staff_authviewsstaffautherrorview) page.
+
+###### `staff_auth.pipeline.associate_by_email`
+
+A function that finds any existing Django users with the same email address as the sign-er in-er, and ties this new sign-in to the same account — but only if that user has previously had a separate social-auth tie in.
+
+###### `staff_auth.pipeline.promote_staffer_to_staff`
+
+A function that promotes all Slack-authenticated users to "staff" status (meaning they can log into the Django admin) when they first sign in with their Slack credentials.
+
+###### `staff_auth.pipeline.promote_manager_to_superuser`
+
+A function that promotes all Slack-authenticated users to "superuser" status (meaning they can log into the Django admin) when they first sign in with their Slack credentials — if the email address on their Slack account matches an email address found in the `settings.MANAGERS` list.
+
+###### `staff_auth.views.StaffAuthErrorView`
+
+An error page shown to users if they try and log in via a different Slack workspace.
+
+(Note that the HTML and CSS for this view live at `./staff_auth/templates/staff_auth/auth-error.html` and `./staff_auth/static/staff_auth/css/page-styles.css`, respectively.)
+
+#### `./example/`
+
+An example Django project that shows how we implement staff Slack access.
+
+Inside this directory you'll find a standard (if threadbare) Django app, with an example `.env` file, a `Pipfile` and a `manage.py` script at the top level.
+
+Inside the `exampleapp` subdirectory is this example app's `settings.py` file (where you can see an example implementation of `politico-staff-auth`'s required configuration variables), along with a `urls.py` file to demonstrate how that piece of wiring should be performed. Standard helper files including `wsgi.py` can also be found in this subdirectory.
+
+
+## Launching the example app
+
+1.  Change into the `./example/` directory one level below this README and install dependencies.
+
+    ```sh
+    cd ./example/
+    pipenv install
+    ```
+
+2.  Create a `.env` file from the `.env.example` template, and insert appropriate values.
+
+    ```sh
+    cp .env.example .env
+    ```
+
+    See the ["Configuration"](#configuration) section below for more information about what goes in each setting.
+
+3.  Create a new blank database, then populate it with the necessary tables.
+
+    ```sh
+    make database
+    pipenv run python manage.py migrate
+    ```
+
+4.  Start the Django test server.
+
+    ```sh
+    pipenv run python manage.py runserver
+    ```
+
+5.  Navigate to [the admin site on your test server](http://local-dev.politicoapps.com:8000/admin/) and click the "Staff login" button.
+
+## Installation
+
+1.  Install from PyPI:
+
+    ```sh
+    pipenv install politico-staff-auth
+    ```
+
+2.  Add `staff_auth` and `social_django` to the list of apps installed into Django.
+
+    _In your project's `settings.py`:_
+
+    ```python
+    INSTALLED_APPS = [
+      "staff_auth",
+
+      # ...
+      # Existing installed apps
+      # ...
+
+      "social_django",
+    ]
+    ```
+
+    **NOTE:** The `staff_auth` app must be first in this list (or, at least, must appear before the pre-existing line `django.contrib.admin`). The `social_django` line should appear after all apps that are distributed with Django itself.
+
+3.  Add the credentials for your staff's Slack workspace.
+
+    _In your project's `settings.py`:_
+
+    ```python
+    STAFF_AUTH_SLACK_KEY = "auth-key"
+
+    STAFF_AUTH_SLACK_SECRET = "secret-key"
+
+    STAFF_AUTH_SLACK_TEAM = "my-value-here"
+    ```
+
+    For more on these values, see the ["Configuration"](#configuration) section below.
+
+    **NOTE:** We recommend reading these values from environment variables, but there's no accounting for taste.
+
+4.  Add the required middleware for rich login error messages.
+
+    _In your project's `settings.py`:_
+
+    ```python
+    MIDDLEWARE = [
+        # ...
+        # Existing middleware
+        # ...
+
+        "staff_auth.middleware.InvalidWorkspaceErrorMiddleware",
+    ]
+    ```
+
+    **NOTE:** The `staff_auth.middleware.InvalidWorkspaceErrorMiddleware` entry should go at the end of the existing `MIDDLEWARE` list.
+
+5.  With the previous steps complete, you can now implement the basic staff auth settings.
+
+    _In your project's `settings.py`:_
+
+    ```python
+    from staff_auth.configured_settings import configure_staff_auth
+
+    staff_auth_settings = configure_staff_auth(
+        key=STAFF_AUTH_SLACK_KEY,
+        secret=STAFF_AUTH_SLACK_SECRET,
+        team=STAFF_AUTH_SLACK_TEAM,
+    )
+
+    for setting_name, setting_value in staff_auth_settings.items():
+        globals()[setting_name] = setting_value
+    ```
+
+6.  Set Django to use the Slack auth backend whenever users are asked to log in.
+
+    _In your project's `settings.py`:_
+
+    ```python
+    LOGIN_URL = "staff_auth:slack-login"
+    ```
+
+7.  Wire up the `staff_auth` and `social_django` URLs.
+
+    _In your project's top-level URLconf (`urls.py` file):_
+
+    ```python
+    urlpatterns = [
+      # ...
+      # Existing URL patterns
+      # ...
+
+      path("social/", include("social_django.urls", namespace="social")),
+      path("staff-auth/", include("staff_auth.urls")),
+    ]
+    ```
+
+
+8.  _**Optional:**_ Add pipelines.
+
+    _In your project's `settings.py`:_
+
+    ```python
+    SOCIAL_AUTH_PIPELINE = (
+        "social_core.pipeline.social_auth.social_details",
+        "social_core.pipeline.social_auth.social_uid",
+        "social_core.pipeline.social_auth.auth_allowed",
+        "social_core.pipeline.social_auth.social_user",
+        "social_core.pipeline.user.get_username",
+        "social_core.pipeline.user.create_user",
+        "social_core.pipeline.social_auth.associate_user",
+        "social_core.pipeline.social_auth.load_extra_data",
+        "staff_auth.pipeline.promote_staffer_to_staff",
+        "staff_auth.pipeline.promote_manager_to_superuser",
+        "social_core.pipeline.user.user_details",
+    )
+    ```
+
+    You can disable either or both of the `staff_auth.pipeline` classes listed above, but please take care to preserve the order seen here — re-ordering these pipelines could produce unintended and hard-to-debug consequences.
+
+    **NOTE:** The behaviors of `staff_auth.pipeline.promote_staffer_to_staff` and `staff_auth.pipeline.promote_manager_to_superuser` are described in the ["What's inside"](#whats-inside) section above.
+
+    **NOTE 2:** If you're not using either `staff_auth.pipeline` class, skip this step and ensure your project's `settings.py` file has no `SOCIAL_AUTH_PIPELINE` value set.
+
+9.  _**Optional:**_ Modify the URLs where users are bounced to when they successfully log in or log out.
+
+    These are standard Django settings, and can take either URLs or named URL patterns (as you would pass to the `{% url %}` template tag).
+
+    _In your project's `settings.py`:_
+
+    ```python
+    LOGIN_REDIRECT_URL = "/my/url/pattern/"
+
+    LOGOUT_REDIRECT_URL = "namespace:view-name"
+    ```
+
+    **NOTE:** For more information, see the Django documentation entries [here](https://docs.djangoproject.com/en/2.2/ref/settings/#login-redirect-url) and [here](https://docs.djangoproject.com/en/2.2/ref/settings/#logout-redirect-url).
+
+
+## Configuration
+
+| Setting | What it does |
+|:--|:--|
+| `STAFF_AUTH_SLACK_KEY` | The **'Client ID'** from the Slack "app" you've connected to your workspace for authenticating users. Passed to Python Social Auth as `SOCIAL_AUTH_SLACK_KEY`. |
+| `STAFF_AUTH_SLACK_SECRET` | The `Client Secret` from this Slack "app". Passed to Python Social Auth as `SOCIAL_AUTH_SLACK_SECRET`. |
+| `STAFF_AUTH_SLACK_TEAM` | The name of the Slack workspace where your users have accounts. (A handy way of remembering this: it's also the subdomain of slack.com where users log in to use Slack itself.) Passed to Python Social Auth as `SOCIAL_AUTH_SLACK_TEAM`. |
+
+
+## Copyright
+
+&copy; 2019&ndash;present POLITICO LLC
```

### Comparing `politico-staff-auth-0.0.5/LICENSE` & `politico-staff-auth-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `politico-staff-auth-0.0.5/README.md` & `politico-staff-auth-0.0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ![POLITICO](https://politico.com/interactives/cdn/images/badge.svg)
 
 ```
-          __          _____  _____                 __  .__         
-  _______/  |______ _/ ____\/ ____\ _____   __ ___/  |_|  |__      
- /  ___/\   __\__  \\   __\\   __\  \__  \ |  |  \   __\  |  \     
- \___ \  |  |  / __ \|  |   |  |     / __ \|  |  /|  | |   Y  \    
+          __          _____  _____                 __  .__
+  _______/  |______ _/ ____\/ ____\ _____   __ ___/  |_|  |__
+ /  ___/\   __\__  \\   __\\   __\  \__  \ |  |  \   __\  |  \
+ \___ \  |  |  / __ \|  |   |  |     / __ \|  |  /|  | |   Y  \
 /____  > |__| (____  /__|   |__|    (____  /____/ |__| |___|  / /\
      \/            \/                    \/                 \/  \/
 ```
 
 # POLITICO staff auth
 
 This app stores a handful of useful utilities we use across our various Django apps at POLITICO to integrate our staff authorization and authentication, which is implemented with Slack via [`Python Social Auth`](https://python-social-auth.readthedocs.io/).
@@ -47,14 +47,18 @@
 
 A subclass of Python Social Auth's Slack authentication backend. Unlike the original, this variant forces users to log in with credentials from the specified Slack workspace (rather than from any Slack workspace).
 
 ###### `staff_auth.middleware.InvalidWorkspaceErrorMiddleware`
 
 A middleware that listens for Python Social Auth's `AuthForbidden` exceptions and maps them to rich output in a [`StaffAuthErrorView`](#staff_authviewsstaffautherrorview) page.
 
+###### `staff_auth.pipeline.associate_by_email`
+
+A function that finds any existing Django users with the same email address as the sign-er in-er, and ties this new sign-in to the same account — but only if that user has previously had a separate social-auth tie in.
+
 ###### `staff_auth.pipeline.promote_staffer_to_staff`
 
 A function that promotes all Slack-authenticated users to "staff" status (meaning they can log into the Django admin) when they first sign in with their Slack credentials.
 
 ###### `staff_auth.pipeline.promote_manager_to_superuser`
 
 A function that promotes all Slack-authenticated users to "superuser" status (meaning they can log into the Django admin) when they first sign in with their Slack credentials — if the email address on their Slack account matches an email address found in the `settings.MANAGERS` list.
@@ -236,15 +240,15 @@
     These are standard Django settings, and can take either URLs or named URL patterns (as you would pass to the `{% url %}` template tag).
 
     _In your project's `settings.py`:_
 
     ```python
     LOGIN_REDIRECT_URL = "/my/url/pattern/"
 
-    LOGOUT_REDIRECT_URL = "/namespace:view-name/"
+    LOGOUT_REDIRECT_URL = "namespace:view-name"
     ```
 
     **NOTE:** For more information, see the Django documentation entries [here](https://docs.djangoproject.com/en/2.2/ref/settings/#login-redirect-url) and [here](https://docs.djangoproject.com/en/2.2/ref/settings/#logout-redirect-url).
 
 
 ## Configuration
```

### Comparing `politico-staff-auth-0.0.5/setup.py` & `politico-staff-auth-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `politico-staff-auth-0.0.5/politico_staff_auth.egg-info/PKG-INFO` & `politico-staff-auth-0.0.6/politico_staff_auth.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,284 +1,288 @@
 Metadata-Version: 2.1
 Name: politico-staff-auth
-Version: 0.0.5
+Version: 0.0.6
 Summary: Staff authentication via Slack, the POLITICO way.
 Home-page: https://github.com/The-Politico/politico-staff-auth/
 Author: POLITICO interactive news
 Author-email: interactives@politico.com
 License: MIT
-Description: ![POLITICO](https://politico.com/interactives/cdn/images/badge.svg)
-        
-        ```
-                  __          _____  _____                 __  .__         
-          _______/  |______ _/ ____\/ ____\ _____   __ ___/  |_|  |__      
-         /  ___/\   __\__  \\   __\\   __\  \__  \ |  |  \   __\  |  \     
-         \___ \  |  |  / __ \|  |   |  |     / __ \|  |  /|  | |   Y  \    
-        /____  > |__| (____  /__|   |__|    (____  /____/ |__| |___|  / /\
-             \/            \/                    \/                 \/  \/
-        ```
-        
-        # POLITICO staff auth
-        
-        This app stores a handful of useful utilities we use across our various Django apps at POLITICO to integrate our staff authorization and authentication, which is implemented with Slack via [`Python Social Auth`](https://python-social-auth.readthedocs.io/).
-        
-        
-        ## Requirements
-        
-        - Python 3.6 — `brew install python`
-        
-        - Pipenv — `brew install pipenv`
-        
-        - Django (tested on versions 2.1.x and 2.2.x)
-        
-        - A Slack workspace with users
-        
-        - A Slack app connected to that workspace, with a "Redirect URL" entry matching the following pattern:
-        
-          `http://<your server name>/social/complete/slack/`
-        
-          (**Note:** you can have multiple "Redirect URLs" for the same app. For local development, you'll be aliasing `localhost` to a subdomain of your choosing, as described in the ["Domain resolution"](#domain-resolution) section below.)
-        
-        - _Optional:_ PostgreSQL — `brew install postgresql`
-        
-        
-        ## What's inside
-        
-        #### `./staff_auth/`
-        
-        The app that handles staff Slack authorization and authentication.
-        
-        ###### `./staff_auth/templates/admin/login.html` and `./staff_auth/static/staff_auth/css/custom-login.css`
-        
-        Custom HTML and CSS to add a "Staff login (with Slack)" button to the standard Django admin login form.
-        
-        ###### `staff_auth.backend.WorkspaceSpecificSlackOAuth2`
-        
-        A subclass of Python Social Auth's Slack authentication backend. Unlike the original, this variant forces users to log in with credentials from the specified Slack workspace (rather than from any Slack workspace).
-        
-        ###### `staff_auth.middleware.InvalidWorkspaceErrorMiddleware`
-        
-        A middleware that listens for Python Social Auth's `AuthForbidden` exceptions and maps them to rich output in a [`StaffAuthErrorView`](#staff_authviewsstaffautherrorview) page.
-        
-        ###### `staff_auth.pipeline.promote_staffer_to_staff`
-        
-        A function that promotes all Slack-authenticated users to "staff" status (meaning they can log into the Django admin) when they first sign in with their Slack credentials.
-        
-        ###### `staff_auth.pipeline.promote_manager_to_superuser`
-        
-        A function that promotes all Slack-authenticated users to "superuser" status (meaning they can log into the Django admin) when they first sign in with their Slack credentials — if the email address on their Slack account matches an email address found in the `settings.MANAGERS` list.
-        
-        ###### `staff_auth.views.StaffAuthErrorView`
-        
-        An error page shown to users if they try and log in via a different Slack workspace.
-        
-        (Note that the HTML and CSS for this view live at `./staff_auth/templates/staff_auth/auth-error.html` and `./staff_auth/static/staff_auth/css/page-styles.css`, respectively.)
-        
-        #### `./example/`
-        
-        An example Django project that shows how we implement staff Slack access.
-        
-        Inside this directory you'll find a standard (if threadbare) Django app, with an example `.env` file, a `Pipfile` and a `manage.py` script at the top level.
-        
-        Inside the `exampleapp` subdirectory is this example app's `settings.py` file (where you can see an example implementation of `politico-staff-auth`'s required configuration variables), along with a `urls.py` file to demonstrate how that piece of wiring should be performed. Standard helper files including `wsgi.py` can also be found in this subdirectory.
-        
-        
-        ## Launching the example app
-        
-        1.  Change into the `./example/` directory one level below this README and install dependencies.
-        
-            ```sh
-            cd ./example/
-            pipenv install
-            ```
-        
-        2.  Create a `.env` file from the `.env.example` template, and insert appropriate values.
-        
-            ```sh
-            cp .env.example .env
-            ```
-        
-            See the ["Configuration"](#configuration) section below for more information about what goes in each setting.
-        
-        3.  Create a new blank database, then populate it with the necessary tables.
-        
-            ```sh
-            make database
-            pipenv run python manage.py migrate
-            ```
-        
-        4.  Start the Django test server.
-        
-            ```sh
-            pipenv run python manage.py runserver
-            ```
-        
-        5.  Navigate to [the admin site on your test server](http://local-dev.politicoapps.com:8000/admin/) and click the "Staff login" button.
-        
-        ## Installation
-        
-        1.  Install from PyPI:
-        
-            ```sh
-            pipenv install politico-staff-auth
-            ```
-        
-        2.  Add `staff_auth` and `social_django` to the list of apps installed into Django.
-        
-            _In your project's `settings.py`:_
-        
-            ```python
-            INSTALLED_APPS = [
-              "staff_auth",
-        
-              # ...
-              # Existing installed apps
-              # ...
-        
-              "social_django",
-            ]
-            ```
-        
-            **NOTE:** The `staff_auth` app must be first in this list (or, at least, must appear before the pre-existing line `django.contrib.admin`). The `social_django` line should appear after all apps that are distributed with Django itself.
-        
-        3.  Add the credentials for your staff's Slack workspace.
-        
-            _In your project's `settings.py`:_
-        
-            ```python
-            STAFF_AUTH_SLACK_KEY = "auth-key"
-        
-            STAFF_AUTH_SLACK_SECRET = "secret-key"
-        
-            STAFF_AUTH_SLACK_TEAM = "my-value-here"
-            ```
-        
-            For more on these values, see the ["Configuration"](#configuration) section below.
-        
-            **NOTE:** We recommend reading these values from environment variables, but there's no accounting for taste.
-        
-        4.  Add the required middleware for rich login error messages.
-        
-            _In your project's `settings.py`:_
-        
-            ```python
-            MIDDLEWARE = [
-                # ...
-                # Existing middleware
-                # ...
-        
-                "staff_auth.middleware.InvalidWorkspaceErrorMiddleware",
-            ]
-            ```
-        
-            **NOTE:** The `staff_auth.middleware.InvalidWorkspaceErrorMiddleware` entry should go at the end of the existing `MIDDLEWARE` list.
-        
-        5.  With the previous steps complete, you can now implement the basic staff auth settings.
-        
-            _In your project's `settings.py`:_
-        
-            ```python
-            from staff_auth.configured_settings import configure_staff_auth
-        
-            staff_auth_settings = configure_staff_auth(
-                key=STAFF_AUTH_SLACK_KEY,
-                secret=STAFF_AUTH_SLACK_SECRET,
-                team=STAFF_AUTH_SLACK_TEAM,
-            )
-        
-            for setting_name, setting_value in staff_auth_settings.items():
-                globals()[setting_name] = setting_value
-            ```
-        
-        6.  Set Django to use the Slack auth backend whenever users are asked to log in.
-        
-            _In your project's `settings.py`:_
-        
-            ```python
-            LOGIN_URL = "staff_auth:slack-login"
-            ```
-        
-        7.  Wire up the `staff_auth` and `social_django` URLs.
-        
-            _In your project's top-level URLconf (`urls.py` file):_
-        
-            ```python
-            urlpatterns = [
-              # ...
-              # Existing URL patterns
-              # ...
-        
-              path("social/", include("social_django.urls", namespace="social")),
-              path("staff-auth/", include("staff_auth.urls")),
-            ]
-            ```
-        
-        
-        8.  _**Optional:**_ Add pipelines.
-        
-            _In your project's `settings.py`:_
-        
-            ```python
-            SOCIAL_AUTH_PIPELINE = (
-                "social_core.pipeline.social_auth.social_details",
-                "social_core.pipeline.social_auth.social_uid",
-                "social_core.pipeline.social_auth.auth_allowed",
-                "social_core.pipeline.social_auth.social_user",
-                "social_core.pipeline.user.get_username",
-                "social_core.pipeline.user.create_user",
-                "social_core.pipeline.social_auth.associate_user",
-                "social_core.pipeline.social_auth.load_extra_data",
-                "staff_auth.pipeline.promote_staffer_to_staff",
-                "staff_auth.pipeline.promote_manager_to_superuser",
-                "social_core.pipeline.user.user_details",
-            )
-            ```
-        
-            You can disable either or both of the `staff_auth.pipeline` classes listed above, but please take care to preserve the order seen here — re-ordering these pipelines could produce unintended and hard-to-debug consequences.
-        
-            **NOTE:** The behaviors of `staff_auth.pipeline.promote_staffer_to_staff` and `staff_auth.pipeline.promote_manager_to_superuser` are described in the ["What's inside"](#whats-inside) section above.
-        
-            **NOTE 2:** If you're not using either `staff_auth.pipeline` class, skip this step and ensure your project's `settings.py` file has no `SOCIAL_AUTH_PIPELINE` value set.
-        
-        9.  _**Optional:**_ Modify the URLs where users are bounced to when they successfully log in or log out.
-        
-            These are standard Django settings, and can take either URLs or named URL patterns (as you would pass to the `{% url %}` template tag).
-        
-            _In your project's `settings.py`:_
-        
-            ```python
-            LOGIN_REDIRECT_URL = "/my/url/pattern/"
-        
-            LOGOUT_REDIRECT_URL = "/namespace:view-name/"
-            ```
-        
-            **NOTE:** For more information, see the Django documentation entries [here](https://docs.djangoproject.com/en/2.2/ref/settings/#login-redirect-url) and [here](https://docs.djangoproject.com/en/2.2/ref/settings/#logout-redirect-url).
-        
-        
-        ## Configuration
-        
-        | Setting | What it does |
-        |:--|:--|
-        | `STAFF_AUTH_SLACK_KEY` | The **'Client ID'** from the Slack "app" you've connected to your workspace for authenticating users. Passed to Python Social Auth as `SOCIAL_AUTH_SLACK_KEY`. |
-        | `STAFF_AUTH_SLACK_SECRET` | The `Client Secret` from this Slack "app". Passed to Python Social Auth as `SOCIAL_AUTH_SLACK_SECRET`. |
-        | `STAFF_AUTH_SLACK_TEAM` | The name of the Slack workspace where your users have accounts. (A handy way of remembering this: it's also the subdomain of slack.com where users log in to use Slack itself.) Passed to Python Social Auth as `SOCIAL_AUTH_SLACK_TEAM`. |
-        
-        
-        ## Copyright
-        
-        &copy; 2019&ndash;present POLITICO LLC
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Internet :: WWW/HTTP
 Description-Content-Type: text/markdown
-Provides-Extra: test
 Provides-Extra: dev
+Provides-Extra: test
+License-File: LICENSE
+
+![POLITICO](https://politico.com/interactives/cdn/images/badge.svg)
+
+```
+          __          _____  _____                 __  .__
+  _______/  |______ _/ ____\/ ____\ _____   __ ___/  |_|  |__
+ /  ___/\   __\__  \\   __\\   __\  \__  \ |  |  \   __\  |  \
+ \___ \  |  |  / __ \|  |   |  |     / __ \|  |  /|  | |   Y  \
+/____  > |__| (____  /__|   |__|    (____  /____/ |__| |___|  / /\
+     \/            \/                    \/                 \/  \/
+```
+
+# POLITICO staff auth
+
+This app stores a handful of useful utilities we use across our various Django apps at POLITICO to integrate our staff authorization and authentication, which is implemented with Slack via [`Python Social Auth`](https://python-social-auth.readthedocs.io/).
+
+
+## Requirements
+
+- Python 3.6 — `brew install python`
+
+- Pipenv — `brew install pipenv`
+
+- Django (tested on versions 2.1.x and 2.2.x)
+
+- A Slack workspace with users
+
+- A Slack app connected to that workspace, with a "Redirect URL" entry matching the following pattern:
+
+  `http://<your server name>/social/complete/slack/`
+
+  (**Note:** you can have multiple "Redirect URLs" for the same app. For local development, you'll be aliasing `localhost` to a subdomain of your choosing, as described in the ["Domain resolution"](#domain-resolution) section below.)
+
+- _Optional:_ PostgreSQL — `brew install postgresql`
+
+
+## What's inside
+
+#### `./staff_auth/`
+
+The app that handles staff Slack authorization and authentication.
+
+###### `./staff_auth/templates/admin/login.html` and `./staff_auth/static/staff_auth/css/custom-login.css`
+
+Custom HTML and CSS to add a "Staff login (with Slack)" button to the standard Django admin login form.
+
+###### `staff_auth.backend.WorkspaceSpecificSlackOAuth2`
+
+A subclass of Python Social Auth's Slack authentication backend. Unlike the original, this variant forces users to log in with credentials from the specified Slack workspace (rather than from any Slack workspace).
+
+###### `staff_auth.middleware.InvalidWorkspaceErrorMiddleware`
+
+A middleware that listens for Python Social Auth's `AuthForbidden` exceptions and maps them to rich output in a [`StaffAuthErrorView`](#staff_authviewsstaffautherrorview) page.
+
+###### `staff_auth.pipeline.associate_by_email`
+
+A function that finds any existing Django users with the same email address as the sign-er in-er, and ties this new sign-in to the same account — but only if that user has previously had a separate social-auth tie in.
+
+###### `staff_auth.pipeline.promote_staffer_to_staff`
+
+A function that promotes all Slack-authenticated users to "staff" status (meaning they can log into the Django admin) when they first sign in with their Slack credentials.
+
+###### `staff_auth.pipeline.promote_manager_to_superuser`
+
+A function that promotes all Slack-authenticated users to "superuser" status (meaning they can log into the Django admin) when they first sign in with their Slack credentials — if the email address on their Slack account matches an email address found in the `settings.MANAGERS` list.
+
+###### `staff_auth.views.StaffAuthErrorView`
+
+An error page shown to users if they try and log in via a different Slack workspace.
+
+(Note that the HTML and CSS for this view live at `./staff_auth/templates/staff_auth/auth-error.html` and `./staff_auth/static/staff_auth/css/page-styles.css`, respectively.)
+
+#### `./example/`
+
+An example Django project that shows how we implement staff Slack access.
+
+Inside this directory you'll find a standard (if threadbare) Django app, with an example `.env` file, a `Pipfile` and a `manage.py` script at the top level.
+
+Inside the `exampleapp` subdirectory is this example app's `settings.py` file (where you can see an example implementation of `politico-staff-auth`'s required configuration variables), along with a `urls.py` file to demonstrate how that piece of wiring should be performed. Standard helper files including `wsgi.py` can also be found in this subdirectory.
+
+
+## Launching the example app
+
+1.  Change into the `./example/` directory one level below this README and install dependencies.
+
+    ```sh
+    cd ./example/
+    pipenv install
+    ```
+
+2.  Create a `.env` file from the `.env.example` template, and insert appropriate values.
+
+    ```sh
+    cp .env.example .env
+    ```
+
+    See the ["Configuration"](#configuration) section below for more information about what goes in each setting.
+
+3.  Create a new blank database, then populate it with the necessary tables.
+
+    ```sh
+    make database
+    pipenv run python manage.py migrate
+    ```
+
+4.  Start the Django test server.
+
+    ```sh
+    pipenv run python manage.py runserver
+    ```
+
+5.  Navigate to [the admin site on your test server](http://local-dev.politicoapps.com:8000/admin/) and click the "Staff login" button.
+
+## Installation
+
+1.  Install from PyPI:
+
+    ```sh
+    pipenv install politico-staff-auth
+    ```
+
+2.  Add `staff_auth` and `social_django` to the list of apps installed into Django.
+
+    _In your project's `settings.py`:_
+
+    ```python
+    INSTALLED_APPS = [
+      "staff_auth",
+
+      # ...
+      # Existing installed apps
+      # ...
+
+      "social_django",
+    ]
+    ```
+
+    **NOTE:** The `staff_auth` app must be first in this list (or, at least, must appear before the pre-existing line `django.contrib.admin`). The `social_django` line should appear after all apps that are distributed with Django itself.
+
+3.  Add the credentials for your staff's Slack workspace.
+
+    _In your project's `settings.py`:_
+
+    ```python
+    STAFF_AUTH_SLACK_KEY = "auth-key"
+
+    STAFF_AUTH_SLACK_SECRET = "secret-key"
+
+    STAFF_AUTH_SLACK_TEAM = "my-value-here"
+    ```
+
+    For more on these values, see the ["Configuration"](#configuration) section below.
+
+    **NOTE:** We recommend reading these values from environment variables, but there's no accounting for taste.
+
+4.  Add the required middleware for rich login error messages.
+
+    _In your project's `settings.py`:_
+
+    ```python
+    MIDDLEWARE = [
+        # ...
+        # Existing middleware
+        # ...
+
+        "staff_auth.middleware.InvalidWorkspaceErrorMiddleware",
+    ]
+    ```
+
+    **NOTE:** The `staff_auth.middleware.InvalidWorkspaceErrorMiddleware` entry should go at the end of the existing `MIDDLEWARE` list.
+
+5.  With the previous steps complete, you can now implement the basic staff auth settings.
+
+    _In your project's `settings.py`:_
+
+    ```python
+    from staff_auth.configured_settings import configure_staff_auth
+
+    staff_auth_settings = configure_staff_auth(
+        key=STAFF_AUTH_SLACK_KEY,
+        secret=STAFF_AUTH_SLACK_SECRET,
+        team=STAFF_AUTH_SLACK_TEAM,
+    )
+
+    for setting_name, setting_value in staff_auth_settings.items():
+        globals()[setting_name] = setting_value
+    ```
+
+6.  Set Django to use the Slack auth backend whenever users are asked to log in.
+
+    _In your project's `settings.py`:_
+
+    ```python
+    LOGIN_URL = "staff_auth:slack-login"
+    ```
+
+7.  Wire up the `staff_auth` and `social_django` URLs.
+
+    _In your project's top-level URLconf (`urls.py` file):_
+
+    ```python
+    urlpatterns = [
+      # ...
+      # Existing URL patterns
+      # ...
+
+      path("social/", include("social_django.urls", namespace="social")),
+      path("staff-auth/", include("staff_auth.urls")),
+    ]
+    ```
+
+
+8.  _**Optional:**_ Add pipelines.
+
+    _In your project's `settings.py`:_
+
+    ```python
+    SOCIAL_AUTH_PIPELINE = (
+        "social_core.pipeline.social_auth.social_details",
+        "social_core.pipeline.social_auth.social_uid",
+        "social_core.pipeline.social_auth.auth_allowed",
+        "social_core.pipeline.social_auth.social_user",
+        "social_core.pipeline.user.get_username",
+        "social_core.pipeline.user.create_user",
+        "social_core.pipeline.social_auth.associate_user",
+        "social_core.pipeline.social_auth.load_extra_data",
+        "staff_auth.pipeline.promote_staffer_to_staff",
+        "staff_auth.pipeline.promote_manager_to_superuser",
+        "social_core.pipeline.user.user_details",
+    )
+    ```
+
+    You can disable either or both of the `staff_auth.pipeline` classes listed above, but please take care to preserve the order seen here — re-ordering these pipelines could produce unintended and hard-to-debug consequences.
+
+    **NOTE:** The behaviors of `staff_auth.pipeline.promote_staffer_to_staff` and `staff_auth.pipeline.promote_manager_to_superuser` are described in the ["What's inside"](#whats-inside) section above.
+
+    **NOTE 2:** If you're not using either `staff_auth.pipeline` class, skip this step and ensure your project's `settings.py` file has no `SOCIAL_AUTH_PIPELINE` value set.
+
+9.  _**Optional:**_ Modify the URLs where users are bounced to when they successfully log in or log out.
+
+    These are standard Django settings, and can take either URLs or named URL patterns (as you would pass to the `{% url %}` template tag).
+
+    _In your project's `settings.py`:_
+
+    ```python
+    LOGIN_REDIRECT_URL = "/my/url/pattern/"
+
+    LOGOUT_REDIRECT_URL = "namespace:view-name"
+    ```
+
+    **NOTE:** For more information, see the Django documentation entries [here](https://docs.djangoproject.com/en/2.2/ref/settings/#login-redirect-url) and [here](https://docs.djangoproject.com/en/2.2/ref/settings/#logout-redirect-url).
+
+
+## Configuration
+
+| Setting | What it does |
+|:--|:--|
+| `STAFF_AUTH_SLACK_KEY` | The **'Client ID'** from the Slack "app" you've connected to your workspace for authenticating users. Passed to Python Social Auth as `SOCIAL_AUTH_SLACK_KEY`. |
+| `STAFF_AUTH_SLACK_SECRET` | The `Client Secret` from this Slack "app". Passed to Python Social Auth as `SOCIAL_AUTH_SLACK_SECRET`. |
+| `STAFF_AUTH_SLACK_TEAM` | The name of the Slack workspace where your users have accounts. (A handy way of remembering this: it's also the subdomain of slack.com where users log in to use Slack itself.) Passed to Python Social Auth as `SOCIAL_AUTH_SLACK_TEAM`. |
+
+
+## Copyright
+
+&copy; 2019&ndash;present POLITICO LLC
```

### Comparing `politico-staff-auth-0.0.5/politico_staff_auth.egg-info/SOURCES.txt` & `politico-staff-auth-0.0.6/politico_staff_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `politico-staff-auth-0.0.5/staff_auth/backend.py` & `politico-staff-auth-0.0.6/staff_auth/backend.py`

 * *Files identical despite different names*

### Comparing `politico-staff-auth-0.0.5/staff_auth/static/staff_auth/css/page-styles.css` & `politico-staff-auth-0.0.6/staff_auth/static/staff_auth/css/page-styles.css`

 * *Files identical despite different names*

### Comparing `politico-staff-auth-0.0.5/staff_auth/static/staff_auth/css/custom-login.css` & `politico-staff-auth-0.0.6/staff_auth/static/staff_auth/css/custom-login.css`

 * *Files identical despite different names*

### Comparing `politico-staff-auth-0.0.5/staff_auth/templates/admin/login.html` & `politico-staff-auth-0.0.6/staff_auth/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `politico-staff-auth-0.0.5/staff_auth/templates/staff_auth/auth-error.html` & `politico-staff-auth-0.0.6/staff_auth/templates/staff_auth/auth-error.html`

 * *Files identical despite different names*

### Comparing `politico-staff-auth-0.0.5/staff_auth/configured_settings.py` & `politico-staff-auth-0.0.6/staff_auth/configured_settings.py`

 * *Files identical despite different names*

### Comparing `politico-staff-auth-0.0.5/staff_auth/middleware.py` & `politico-staff-auth-0.0.6/staff_auth/middleware.py`

 * *Files identical despite different names*

### Comparing `politico-staff-auth-0.0.5/staff_auth/views.py` & `politico-staff-auth-0.0.6/staff_auth/views.py`

 * *Files identical despite different names*

