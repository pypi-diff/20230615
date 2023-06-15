# Comparing `tmp/bl_hector-0.1.0a8.tar.gz` & `tmp/bl_hector-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bl_hector-0.1.0a8.tar", max compression
+gzip compressed data, was "bl_hector-0.1.1.tar", max compression
```

## Comparing `bl_hector-0.1.0a8.tar` & `bl_hector-0.1.1.tar`

### file list

```diff
@@ -1,92 +1,90 @@
--rw-r--r--   0        0        0    34523 2023-05-31 09:45:12.827540 bl_hector-0.1.0a8/LICENSE
--rw-r--r--   0        0        0     1854 2023-06-14 06:53:49.525288 bl_hector-0.1.0a8/README.md
--rw-r--r--   0        0        0      807 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/__init__.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/application/__init__.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/application/use_cases/__init__.py
--rw-r--r--   0        0        0     3803 2023-06-14 08:52:32.636997 bl_hector-0.1.0a8/bl_hector/application/use_cases/add_book.py
--rw-r--r--   0        0        0     1977 2023-06-14 08:52:32.588998 bl_hector-0.1.0a8/bl_hector/application/use_cases/display_book.py
--rw-r--r--   0        0        0     1975 2023-06-14 08:52:32.616998 bl_hector-0.1.0a8/bl_hector/application/use_cases/look_up_book.py
--rw-r--r--   0        0        0     3751 2023-06-14 08:52:32.600998 bl_hector-0.1.0a8/bl_hector/application/use_cases/search_books.py
--rw-r--r--   0        0        0     3801 2023-06-14 08:52:32.580998 bl_hector-0.1.0a8/bl_hector/application/use_cases/update_book.py
--rw-r--r--   0        0        0      944 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/configuration/__init__.py
--rw-r--r--   0        0        0      981 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/configuration/cli.py
--rw-r--r--   0        0        0      986 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/configuration/wsgi.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/domain/__init__.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/domain/administration/__init__.py
--rw-r--r--   0        0        0     1272 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/domain/administration/entities.py
--rw-r--r--   0        0        0      808 2023-06-09 13:18:08.922894 bl_hector-0.1.0a8/bl_hector/domain/administration/enumerations.py
--rw-r--r--   0        0        0     1659 2023-06-09 13:18:04.750942 bl_hector-0.1.0a8/bl_hector/domain/administration/repositories.py
--rw-r--r--   0        0        0     1196 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/domain/administration/services.py
--rw-r--r--   0        0        0      931 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/domain/administration/value_objects.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/domain/collection_management/__init__.py
--rw-r--r--   0        0        0     1563 2023-06-14 08:54:37.759525 bl_hector-0.1.0a8/bl_hector/domain/collection_management/entities.py
--rw-r--r--   0        0        0      996 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/domain/collection_management/errors.py
--rw-r--r--   0        0        0     1509 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/domain/collection_management/repositories.py
--rw-r--r--   0        0        0     1173 2023-06-13 16:46:31.847726 bl_hector-0.1.0a8/bl_hector/domain/collection_management/services.py
--rw-r--r--   0        0        0     1800 2023-06-14 08:53:33.276286 bl_hector-0.1.0a8/bl_hector/domain/collection_management/validators.py
--rw-r--r--   0        0        0     3325 2023-06-14 08:52:32.560998 bl_hector-0.1.0a8/bl_hector/domain/collection_management/value_objects.py
--rw-r--r--   0        0        0     1453 2023-06-13 16:46:31.579729 bl_hector-0.1.0a8/bl_hector/infrastructure/__init__.py
--rw-r--r--   0        0        0     3738 2023-06-14 08:44:03.058810 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/__init__.py
--rw-r--r--   0        0        0     1064 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/aliases/__init__.py
--rw-r--r--   0        0        0     1693 2023-06-09 08:04:31.521092 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/auth/__init__.py
--rw-r--r--   0        0        0     4116 2023-06-13 17:14:54.950836 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/books/__init__.py
--rw-r--r--   0        0        0     3466 2023-06-13 16:45:43.904308 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/services.py
--rw-r--r--   0        0        0   207302 2023-06-07 16:14:27.662555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css
--rw-r--r--   0        0        0    73117 2023-06-07 16:14:27.662555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css
--rw-r--r--   0        0        0      664 2023-06-13 07:15:23.075945 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/css/hector.css
--rw-r--r--   0        0        0      655 2023-06-07 16:14:27.662555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/favicon.svg
--rw-r--r--   0        0        0    35880 2023-06-07 16:14:27.662555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/img/placeholders/1280x960.png
--rw-r--r--   0        0        0      928 2023-06-07 16:14:27.662555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png
--rw-r--r--   0        0        0     3602 2023-06-07 16:14:27.662555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/img/placeholders/96x96.png
--rw-r--r--   0        0        0    42819 2023-06-07 16:14:27.670555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js
--rw-r--r--   0        0        0    97249 2023-06-07 16:14:27.670555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js
--rw-r--r--   0        0        0     6828 2023-06-07 16:14:27.670555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js
--rw-r--r--   0        0        0   186112 2023-06-07 16:14:27.670555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   107460 2023-06-07 16:14:27.674555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    62048 2023-06-07 16:14:27.674555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    25096 2023-06-07 16:14:27.674555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   397728 2023-06-07 16:14:27.674555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   150472 2023-06-07 16:14:27.674555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0     2363 2023-06-14 06:38:35.772624 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/totp/__init__.py
--rw-r--r--   0        0        0     1265 2023-06-09 13:18:08.926894 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/utils.py
--rw-r--r--   0        0        0     4544 2023-06-13 08:24:56.879217 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/webauthn/__init__.py
--rw-r--r--   0        0        0     3282 2023-06-13 05:56:18.671790 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/webauthn/security.py
--rw-r--r--   0        0        0     1789 2023-06-13 17:15:23.130490 bl_hector-0.1.0a8/bl_hector/infrastructure/isbnlib/__init__.py
--rw-r--r--   0        0        0     1568 2023-06-13 07:05:37.235116 bl_hector-0.1.0a8/bl_hector/infrastructure/requests/__init__.py
--rw-r--r--   0        0        0     2615 2023-06-14 06:22:16.919024 bl_hector-0.1.0a8/bl_hector/infrastructure/settings.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.674555 bl_hector-0.1.0a8/bl_hector/infrastructure/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     8336 2023-06-14 08:52:32.540998 bl_hector-0.1.0a8/bl_hector/infrastructure/sqlalchemy/repositories.py
--rw-r--r--   0        0        0     2058 2023-06-07 16:14:27.674555 bl_hector-0.1.0a8/bl_hector/infrastructure/typer/__init__.py
--rw-r--r--   0        0        0     2419 2023-06-14 08:58:30.132757 bl_hector-0.1.0a8/bl_hector/infrastructure/typer/books.py
--rw-r--r--   0        0        0     2099 2023-06-14 08:40:08.593384 bl_hector-0.1.0a8/bl_hector/infrastructure/typer/services.py
--rw-r--r--   0        0        0     1845 2023-06-14 08:54:22.907701 bl_hector-0.1.0a8/bl_hector/interfaces/__init__.py
--rw-r--r--   0        0        0      761 2023-06-10 16:50:21.825376 bl_hector-0.1.0a8/bl_hector/interfaces/exceptions.py
--rw-r--r--   0        0        0     3371 2023-06-11 08:23:57.603430 bl_hector-0.1.0a8/bl_hector/interfaces/from_dict.py
--rw-r--r--   0        0        0     1659 2023-06-13 07:05:37.239116 bl_hector-0.1.0a8/bl_hector/interfaces/from_json.py
--rw-r--r--   0        0        0     1435 2023-06-07 17:00:49.589157 bl_hector-0.1.0a8/bl_hector/interfaces/l10n/__init__.py
--rw-r--r--   0        0        0     4568 2023-06-13 17:14:28.243164 bl_hector-0.1.0a8/bl_hector/interfaces/l10n/en-GB/main.ftl
--rw-r--r--   0        0        0     5167 2023-06-13 17:14:41.846997 bl_hector-0.1.0a8/bl_hector/interfaces/l10n/fr-FR/main.ftl
--rw-r--r--   0        0        0     1407 2023-06-07 16:14:27.682555 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/__init__.py
--rw-r--r--   0        0        0    14753 2023-06-14 08:55:58.762565 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/__init__.py
--rw-r--r--   0        0        0     1331 2023-06-14 09:08:21.253609 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug
--rw-r--r--   0        0        0     4296 2023-06-13 14:17:08.848203 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/books/add.pug
--rw-r--r--   0        0        0     2100 2023-06-13 17:14:13.355347 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/books/display.pug
--rw-r--r--   0        0        0     2043 2023-06-14 08:24:15.964273 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug
--rw-r--r--   0        0        0     5646 2023-06-14 09:05:35.607596 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/books/search.pug
--rw-r--r--   0        0        0     3589 2023-06-13 08:34:41.343554 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/books/update.pug
--rw-r--r--   0        0        0      982 2023-06-09 13:18:08.934894 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/error.pug
--rw-r--r--   0        0        0     2045 2023-06-14 09:04:09.936643 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/layout.pug
--rw-r--r--   0        0        0     1127 2023-06-13 07:11:41.542636 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug
--rw-r--r--   0        0        0     4129 2023-06-14 08:23:59.692482 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug
--rw-r--r--   0        0        0     1992 2023-06-13 14:17:08.848203 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug
--rw-r--r--   0        0        0     1400 2023-06-13 09:27:19.501527 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug
--rw-r--r--   0        0        0     2010 2023-06-07 16:14:27.682555 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug
--rw-r--r--   0        0        0     2045 2023-06-07 16:14:27.682555 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug
--rw-r--r--   0        0        0     1310 2023-06-07 16:14:27.682555 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_json/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-07 16:14:27.682555 bl_hector-0.1.0a8/bl_hector/interfaces/to_terminal/__init__.py
--rw-r--r--   0        0        0     1885 2023-06-13 07:05:37.239116 bl_hector-0.1.0a8/bl_hector/interfaces/to_terminal/as_json.py
--rw-r--r--   0        0        0     3888 2023-06-14 08:58:01.757097 bl_hector-0.1.0a8/bl_hector/interfaces/to_terminal/as_text.py
--rw-r--r--   0        0        0     1519 2023-06-07 16:14:27.682555 bl_hector-0.1.0a8/bl_hector/interfaces/utils.py
--rw-r--r--   0        0        0     1516 2023-06-14 09:09:41.284665 bl_hector-0.1.0a8/pyproject.toml
--rw-r--r--   0        0        0     4603 2023-06-14 09:10:49.897226 bl_hector-0.1.0a8/setup.py
--rw-r--r--   0        0        0     2907 2023-06-14 09:10:49.898937 bl_hector-0.1.0a8/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-15 06:52:14.608155 bl_hector-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1854 2023-06-15 06:52:14.608155 bl_hector-0.1.1/README.md
+-rw-r--r--   0        0        0      807 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/application/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/application/use_cases/__init__.py
+-rw-r--r--   0        0        0     3803 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/application/use_cases/add_book.py
+-rw-r--r--   0        0        0     2048 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/application/use_cases/display_book.py
+-rw-r--r--   0        0        0     1975 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/application/use_cases/look_up_book.py
+-rw-r--r--   0        0        0     3751 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/application/use_cases/search_books.py
+-rw-r--r--   0        0        0     3801 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/application/use_cases/update_book.py
+-rw-r--r--   0        0        0      944 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/configuration/__init__.py
+-rw-r--r--   0        0        0      981 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/configuration/cli.py
+-rw-r--r--   0        0        0      986 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/configuration/wsgi.py
+-rw-r--r--   0        0        0      721 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/administration/__init__.py
+-rw-r--r--   0        0        0     1272 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/administration/entities.py
+-rw-r--r--   0        0        0      808 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/administration/enumerations.py
+-rw-r--r--   0        0        0     1659 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/administration/repositories.py
+-rw-r--r--   0        0        0     1196 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/administration/services.py
+-rw-r--r--   0        0        0      931 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/administration/value_objects.py
+-rw-r--r--   0        0        0      721 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/collection_management/__init__.py
+-rw-r--r--   0        0        0     1563 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/collection_management/entities.py
+-rw-r--r--   0        0        0      996 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/collection_management/errors.py
+-rw-r--r--   0        0        0     1509 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/collection_management/repositories.py
+-rw-r--r--   0        0        0     1173 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/collection_management/services.py
+-rw-r--r--   0        0        0     1800 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/collection_management/validators.py
+-rw-r--r--   0        0        0     3325 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/collection_management/value_objects.py
+-rw-r--r--   0        0        0     1453 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/infrastructure/__init__.py
+-rw-r--r--   0        0        0     3738 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/infrastructure/flask/__init__.py
+-rw-r--r--   0        0        0     1064 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/infrastructure/flask/aliases/__init__.py
+-rw-r--r--   0        0        0     1693 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/infrastructure/flask/auth/__init__.py
+-rw-r--r--   0        0        0     4116 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/infrastructure/flask/books/__init__.py
+-rw-r--r--   0        0        0     3466 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/infrastructure/flask/services.py
+-rw-r--r--   0        0        0   207302 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css
+-rw-r--r--   0        0        0    73117 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css
+-rw-r--r--   0        0        0      664 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/css/hector.css
+-rw-r--r--   0        0        0      655 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/favicon.svg
+-rw-r--r--   0        0        0     1502 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png
+-rw-r--r--   0        0        0    42819 2023-06-15 06:52:14.612155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js
+-rw-r--r--   0        0        0    97249 2023-06-15 06:52:14.612155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js
+-rw-r--r--   0        0        0     6828 2023-06-15 06:52:14.612155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js
+-rw-r--r--   0        0        0   186112 2023-06-15 06:52:14.612155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   107460 2023-06-15 06:52:14.612155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    62048 2023-06-15 06:52:14.612155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    25096 2023-06-15 06:52:14.612155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   397728 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   150472 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0     2363 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/flask/totp/__init__.py
+-rw-r--r--   0        0        0     1265 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/flask/utils.py
+-rw-r--r--   0        0        0     4544 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/flask/webauthn/__init__.py
+-rw-r--r--   0        0        0     3282 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/flask/webauthn/security.py
+-rw-r--r--   0        0        0     1789 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/isbnlib/__init__.py
+-rw-r--r--   0        0        0     1729 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/requests/__init__.py
+-rw-r--r--   0        0        0     2615 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/settings.py
+-rw-r--r--   0        0        0      721 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     8336 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/sqlalchemy/repositories.py
+-rw-r--r--   0        0        0     2058 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/typer/__init__.py
+-rw-r--r--   0        0        0     2886 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/typer/books.py
+-rw-r--r--   0        0        0     2099 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/typer/services.py
+-rw-r--r--   0        0        0     1845 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/interfaces/__init__.py
+-rw-r--r--   0        0        0      761 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/interfaces/exceptions.py
+-rw-r--r--   0        0        0     3371 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/interfaces/from_dict.py
+-rw-r--r--   0        0        0     1659 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/interfaces/from_json.py
+-rw-r--r--   0        0        0     1435 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/interfaces/l10n/__init__.py
+-rw-r--r--   0        0        0     4792 2023-06-15 13:06:54.302159 bl_hector-0.1.1/bl_hector/interfaces/l10n/en-GB/main.ftl
+-rw-r--r--   0        0        0     5330 2023-06-15 13:06:54.302159 bl_hector-0.1.1/bl_hector/interfaces/l10n/fr-FR/main.ftl
+-rw-r--r--   0        0        0     1407 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/interfaces/to_http/__init__.py
+-rw-r--r--   0        0        0    14758 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/__init__.py
+-rw-r--r--   0        0        0     1247 2023-06-15 13:06:54.302159 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug
+-rw-r--r--   0        0        0     4296 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/books/add.pug
+-rw-r--r--   0        0        0     2100 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/books/display.pug
+-rw-r--r--   0        0        0     2043 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug
+-rw-r--r--   0        0        0     5727 2023-06-15 13:06:54.302159 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/books/search.pug
+-rw-r--r--   0        0        0     3589 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/books/update.pug
+-rw-r--r--   0        0        0      982 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/error.pug
+-rw-r--r--   0        0        0     2028 2023-06-15 13:06:54.302159 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/layout.pug
+-rw-r--r--   0        0        0     1127 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug
+-rw-r--r--   0        0        0     4129 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug
+-rw-r--r--   0        0        0     1992 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug
+-rw-r--r--   0        0        0     1678 2023-06-15 13:06:54.302159 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug
+-rw-r--r--   0        0        0     2010 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug
+-rw-r--r--   0        0        0     2045 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug
+-rw-r--r--   0        0        0     1310 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_json/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_terminal/__init__.py
+-rw-r--r--   0        0        0     1885 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_terminal/as_json.py
+-rw-r--r--   0        0        0     5280 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_terminal/as_text.py
+-rw-r--r--   0        0        0     1519 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/utils.py
+-rw-r--r--   0        0        0     1570 2023-06-15 13:06:54.302159 bl_hector-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4676 2023-06-15 13:07:06.618553 bl_hector-0.1.1/setup.py
+-rw-r--r--   0        0        0     3048 2023-06-15 13:07:06.618820 bl_hector-0.1.1/PKG-INFO
```

### Comparing `bl_hector-0.1.0a8/LICENSE` & `bl_hector-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/README.md` & `bl_hector-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/__init__.py` & `bl_hector-0.1.1/bl_hector/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/application/__init__.py` & `bl_hector-0.1.1/bl_hector/application/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/application/use_cases/__init__.py` & `bl_hector-0.1.1/bl_hector/application/use_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/application/use_cases/add_book.py` & `bl_hector-0.1.1/bl_hector/application/use_cases/add_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/application/use_cases/display_book.py` & `bl_hector-0.1.1/bl_hector/application/use_cases/display_book.py`

 * *Files 16% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 
     def execute(self, request: Request) -> None:
         try:
             isbn = Isbn.instanciate(request.isbn)
         except IncorrectValue:
             return self.presenter.not_an_isbn(request.isbn)
 
-        if str(isbn) != request.isbn:
-            return self.presenter.see_other(isbn)
+        if not (book := self.books.by_isbn(isbn)):
+            return self.presenter.book_not_found(isbn)
 
-        if book := self.books.by_isbn(isbn):
-            return self.presenter.book(book)
+        self.presenter.book(book)
 
-        self.presenter.book_not_found(isbn)
+        if str(isbn) != request.isbn:
+            # It's just a notification. Some presenters might redirect.
+            self.presenter.see_other(isbn)
```

### Comparing `bl_hector-0.1.0a8/bl_hector/application/use_cases/look_up_book.py` & `bl_hector-0.1.1/bl_hector/application/use_cases/look_up_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/application/use_cases/search_books.py` & `bl_hector-0.1.1/bl_hector/application/use_cases/search_books.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/application/use_cases/update_book.py` & `bl_hector-0.1.1/bl_hector/application/use_cases/update_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/configuration/__init__.py` & `bl_hector-0.1.1/bl_hector/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/configuration/cli.py` & `bl_hector-0.1.1/bl_hector/configuration/cli.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/configuration/wsgi.py` & `bl_hector-0.1.1/bl_hector/configuration/wsgi.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/domain/__init__.py` & `bl_hector-0.1.1/bl_hector/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/domain/administration/__init__.py` & `bl_hector-0.1.1/bl_hector/domain/administration/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/domain/administration/entities.py` & `bl_hector-0.1.1/bl_hector/domain/administration/entities.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/domain/administration/enumerations.py` & `bl_hector-0.1.1/bl_hector/domain/administration/enumerations.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/domain/administration/repositories.py` & `bl_hector-0.1.1/bl_hector/domain/administration/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/domain/administration/services.py` & `bl_hector-0.1.1/bl_hector/domain/administration/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/domain/administration/value_objects.py` & `bl_hector-0.1.1/bl_hector/domain/administration/value_objects.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/domain/collection_management/__init__.py` & `bl_hector-0.1.1/bl_hector/domain/collection_management/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/domain/collection_management/entities.py` & `bl_hector-0.1.1/bl_hector/domain/collection_management/entities.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/domain/collection_management/errors.py` & `bl_hector-0.1.1/bl_hector/domain/collection_management/errors.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/domain/collection_management/repositories.py` & `bl_hector-0.1.1/bl_hector/domain/collection_management/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/domain/collection_management/services.py` & `bl_hector-0.1.1/bl_hector/domain/collection_management/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/domain/collection_management/validators.py` & `bl_hector-0.1.1/bl_hector/domain/collection_management/validators.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/domain/collection_management/value_objects.py` & `bl_hector-0.1.1/bl_hector/domain/collection_management/value_objects.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/__init__.py` & `bl_hector-0.1.1/bl_hector/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/__init__.py` & `bl_hector-0.1.1/bl_hector/infrastructure/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/aliases/__init__.py` & `bl_hector-0.1.1/bl_hector/infrastructure/flask/aliases/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/auth/__init__.py` & `bl_hector-0.1.1/bl_hector/infrastructure/flask/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/books/__init__.py` & `bl_hector-0.1.1/bl_hector/infrastructure/flask/books/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/services.py` & `bl_hector-0.1.1/bl_hector/infrastructure/flask/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css` & `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css` & `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/css/hector.css` & `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/css/hector.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/favicon.svg` & `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js` & `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js` & `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js` & `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf` & `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2` & `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf` & `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2` & `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf` & `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2` & `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/totp/__init__.py` & `bl_hector-0.1.1/bl_hector/infrastructure/flask/totp/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/utils.py` & `bl_hector-0.1.1/bl_hector/infrastructure/flask/utils.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/webauthn/__init__.py` & `bl_hector-0.1.1/bl_hector/infrastructure/flask/webauthn/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/webauthn/security.py` & `bl_hector-0.1.1/bl_hector/infrastructure/flask/webauthn/security.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/isbnlib/__init__.py` & `bl_hector-0.1.1/bl_hector/infrastructure/isbnlib/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/requests/__init__.py` & `bl_hector-0.1.1/bl_hector/infrastructure/requests/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,19 +25,22 @@
 )
 from bl_hector.domain.collection_management.value_objects import Cover, Isbn
 
 
 class CoverProvider(CoverProviderABC):
     def by_isbn(self, isbn: Isbn) -> Optional[Cover]:
         try:
-            return Cover.instanciate(
-                self.__to_data_url(requests.get(self.__get_url(isbn)))
-            )
+            if data_url := self.__to_data_url(requests.get(self.__get_url(isbn))):
+                return Cover.instanciate(data_url)
+            return None
         except Exception as exc:
             logging.error(str(exc))
             return None
 
     def __get_url(self, isbn: Isbn) -> str:
         return f"https://covers.openlibrary.org/b/isbn/{isbn}-L.jpg"
 
     def __to_data_url(self, response: requests.Response) -> str:
-        return "data:image/jpeg;base64," + base64.b64encode(response.content).decode()
+        if response.headers.get("Content-Type", "").startswith("image/"):
+            content = base64.b64encode(response.content).decode()
+            return f"data:image/jpeg;base64,{content}"
+        return ""
```

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/settings.py` & `bl_hector-0.1.1/bl_hector/infrastructure/settings.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/sqlalchemy/__init__.py` & `bl_hector-0.1.1/bl_hector/infrastructure/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/sqlalchemy/repositories.py` & `bl_hector-0.1.1/bl_hector/infrastructure/sqlalchemy/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/typer/__init__.py` & `bl_hector-0.1.1/bl_hector/infrastructure/typer/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/typer/books.py` & `bl_hector-0.1.1/bl_hector/infrastructure/typer/books.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,24 +15,36 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import sys
 
 import typer
 from typing_extensions import Annotated
 
-from bl_hector.application.use_cases import add_book, look_up_book
+from bl_hector.application.use_cases import add_book, display_book, look_up_book
 from bl_hector.infrastructure import ONLY_USER, DummyPermissions, SystemCalendar
 from bl_hector.infrastructure.typer import services
 from bl_hector.interfaces import from_json as controllers
 from bl_hector.interfaces.to_terminal import LookUpBookInterface, as_json, as_text
 
 cmd = typer.Typer()
 
 
 @cmd.command()
+def display(ctx: typer.Context, isbn: str) -> None:
+    """Display a book from the collection."""
+    with services.get_books(ctx.obj) as books:
+        presenter = as_text.DisplayBook(
+            lambda m: typer.echo(m), translator=services.get_translator()
+        )
+        interactor = display_book.Interactor(presenter, books)
+        interactor.execute(display_book.Request(isbn))
+        raise typer.Exit(presenter.exit_code())
+
+
+@cmd.command()
 def look_up(
     ctx: typer.Context,
     isbn: str,
     json: Annotated[bool, typer.Option(help="Format output in JSON.")] = False,
 ) -> None:
     """Look up for book information based on its ISBN number."""
     presenter: LookUpBookInterface
```

### Comparing `bl_hector-0.1.0a8/bl_hector/infrastructure/typer/services.py` & `bl_hector-0.1.1/bl_hector/infrastructure/typer/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/__init__.py` & `bl_hector-0.1.1/bl_hector/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/exceptions.py` & `bl_hector-0.1.1/bl_hector/interfaces/exceptions.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/from_dict.py` & `bl_hector-0.1.1/bl_hector/interfaces/from_dict.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/from_json.py` & `bl_hector-0.1.1/bl_hector/interfaces/from_json.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/l10n/__init__.py` & `bl_hector-0.1.1/bl_hector/interfaces/l10n/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/l10n/en-GB/main.ftl` & `bl_hector-0.1.1/bl_hector/interfaces/l10n/en-GB/main.ftl`

 * *Files 4% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 webauthn-login-title = Log in
 webauthn-login-description = Your browser should be asking you to tap your security device…
 webauthn-login-failure = You couldn't be logged in!?
 
 totp-login-title = Log in
 totp-login-description = Please enter your one-time password.
 totp-login-password = Password
+totp-login-pattern = An TOTP code is made up of 6 digits.
 totp-login-action = Log in
 
 add-book-requires-authentification = You must be authenticated before adding a book!
 add-book-title = Add a new book to the collection
 add-book-action = Add a book
 add-book-cancel = Cancel
 add-book-add = Add
@@ -111,11 +112,14 @@
 update-book-update = Save
 update-book-cover-help = Click to upload a new cover
 update-book-cover-format-not-supported = The format of this cover is not supported!
 
 book-already-exists = Book already in the collection!
 # isbn (string) The ISBN of the book
 # url (string) The URL of the book
+book-added-html = Book <a href="{ $url }">{ $isbn }</a> successfully added!
+# isbn (string) The ISBN of the book
+book-added-text = Book { $isbn } successfully added!
 book-added = Book <a href="{ $url }">{ $isbn }</a> successfully added!
 book-not-found = Book not found!
 book-cannot-be-added = The book cannot be added!
 books-cannot-be-found = The search cannot be performed!
```

#### html2text {}

```diff
@@ -33,27 +33,30 @@
 registration webauthn-register-description = Your browser should be asking you
 to tap your security deviceâ¦ webauthn-register-success = Your security device
 has been succesfully registered! webauthn-register-failure = Your security
 device could not be registered!? webauthn-login-title = Log in webauthn-login-
 description = Your browser should be asking you to tap your security deviceâ¦
 webauthn-login-failure = You couldn't be logged in!? totp-login-title = Log in
 totp-login-description = Please enter your one-time password. totp-login-
-password = Password totp-login-action = Log in add-book-requires-
-authentification = You must be authenticated before adding a book! add-book-
-title = Add a new book to the collection add-book-action = Add a book add-book-
-cancel = Cancel add-book-add = Add add-book-cover-help = Click to upload a
-cover add-book-cover-format-not-supported = The format of this cover is not
-supported! search-books-title = Search for a book search-books-action = Look up
-book search-books-clear = Clear search-books-search = Search search-books-no-
-result = No matching book! search-books-previous-page = Previous search-books-
-next-page = Next # title (string) The title of the book display-book-title =
-Details for "{ $title }" update-book-requires-authentification = You must be
-authenticated before editing a book! # isbn (string) The ISBN of the book
-update-book-title = Edit information for `{ $isbn }` update-book-action = Edit
-update-book-failure = Book cannot be updated! update-book-success = Book has
-been updated! update-book-cancel = Cancel update-book-update = Save update-
-book-cover-help = Click to upload a new cover update-book-cover-format-not-
-supported = The format of this cover is not supported! book-already-exists =
-Book already in the collection! # isbn (string) The ISBN of the book # url
-(string) The URL of the book book-added = Book {_$isbn_} successfully added!
-book-not-found = Book not found! book-cannot-be-added = The book cannot be
-added! books-cannot-be-found = The search cannot be performed!
+password = Password totp-login-pattern = An TOTP code is made up of 6 digits.
+totp-login-action = Log in add-book-requires-authentification = You must be
+authenticated before adding a book! add-book-title = Add a new book to the
+collection add-book-action = Add a book add-book-cancel = Cancel add-book-add =
+Add add-book-cover-help = Click to upload a cover add-book-cover-format-not-
+supported = The format of this cover is not supported! search-books-title =
+Search for a book search-books-action = Look up book search-books-clear = Clear
+search-books-search = Search search-books-no-result = No matching book! search-
+books-previous-page = Previous search-books-next-page = Next # title (string)
+The title of the book display-book-title = Details for "{ $title }" update-
+book-requires-authentification = You must be authenticated before editing a
+book! # isbn (string) The ISBN of the book update-book-title = Edit information
+for `{ $isbn }` update-book-action = Edit update-book-failure = Book cannot be
+updated! update-book-success = Book has been updated! update-book-cancel =
+Cancel update-book-update = Save update-book-cover-help = Click to upload a new
+cover update-book-cover-format-not-supported = The format of this cover is not
+supported! book-already-exists = Book already in the collection! # isbn
+(string) The ISBN of the book # url (string) The URL of the book book-added-
+html = Book {_$isbn_} successfully added! # isbn (string) The ISBN of the book
+book-added-text = Book { $isbn } successfully added! book-added = Book {_$isbn
+} successfully added! book-not-found = Book not found! book-cannot-be-added =
+The book cannot be added! books-cannot-be-found = The search cannot be
+performed!
```

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/l10n/fr-FR/main.ftl` & `bl_hector-0.1.1/bl_hector/interfaces/l10n/fr-FR/main.ftl`

 * *Files 4% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 webauthn-login-title = Connexion
 webauthn-login-description = Votre navigateur devrait être en train de vous demander de toucher votre dispositif de sécurité…
 webauthn-login-failure = Vous n'avez pas pu être connecté·e !?
 
 totp-login-title = Connexion
 totp-login-description = Merci de saisir votre mot de passe à usage unique.
 totp-login-password = Mot de passe
+totp-login-pattern = Un code TOTP se compose de 6 chiffres.
 totp-login-action = Se connecter
 
 add-book-requires-authentification = Vous devez être authentifié·e pour pouvoir ajouter un livre !
 add-book-title = Ajouter un nouveau livre à la collection
 add-book-action = Ajouter un livre
 add-book-cancel = Annuler
 add-book-add = Ajouter
@@ -111,11 +112,13 @@
 update-book-update = Enregistrer
 update-book-cover-help = Cliquez pour téléverser une nouvelle couverture
 update-book-cover-format-not-supported = Le format de cette couverture n'est pas supporté !
 
 book-already-exists = Ce livre est déjà dans la collection !
 # isbn (string) The ISBN of the book
 # url (string) The URL of the book
-book-added = Le livre <a href="{ $url }">{ $isbn }</a> a bien été ajouté !
+book-added-html = Le livre <a href="{ $url }">{ $isbn }</a> a bien été ajouté !
+# isbn (string) The ISBN of the book
+book-added-text = Le livre { $isbn } a bien été ajouté !
 book-not-found = Le livre n'a pas été trouvé !
 book-cannot-be-added = Le livre n'a pas pu être ajouté !
 books-cannot-be-found = La recherche n'a pas pu être effectuée !
```

#### html2text {}

```diff
@@ -37,31 +37,33 @@
 de sÃ©curitÃ©â¦ webauthn-register-success = Votre dispositif de sÃ©curitÃ© a
 Ã©tÃ© correctement associÃ©Â ! webauthn-register-failure = Votre dispositif de
 sÃ©curitÃ© n'a pas pu Ãªtre associÃ©Â !? webauthn-login-title = Connexion
 webauthn-login-description = Votre navigateur devrait Ãªtre en train de vous
 demander de toucher votre dispositif de sÃ©curitÃ©â¦ webauthn-login-failure =
 Vous n'avez pas pu Ãªtre connectÃ©Â·eÂ !? totp-login-title = Connexion totp-
 login-description = Merci de saisir votre mot de passe Ã  usage unique. totp-
-login-password = Mot de passe totp-login-action = Se connecter add-book-
+login-password = Mot de passe totp-login-pattern = Un code TOTP se compose de 6
+chiffres. totp-login-action = Se connecter add-book-requires-authentification =
+Vous devez Ãªtre authentifiÃ©Â·e pour pouvoir ajouter un livreÂ ! add-book-
+title = Ajouter un nouveau livre Ã  la collection add-book-action = Ajouter un
+livre add-book-cancel = Annuler add-book-add = Ajouter add-book-cover-help =
+Cliquez pour tÃ©lÃ©verser une couverture add-book-cover-format-not-supported =
+Le format de cette couverture n'est pas supportÃ©Â ! search-books-title =
+Chercher un livre dans la collection search-books-action = Chercher un livre
+search-books-clear = RÃ©initialiser search-books-search = Chercher search-
+books-no-result = Aucun livre ne correspondÂ ! search-books-previous-page =
+PrÃ©cÃ©dent search-books-next-page = Suivant # title (string) The title of the
+book display-book-title = DÃ©tails pour Â«Â { $title }Â Â» update-book-
 requires-authentification = Vous devez Ãªtre authentifiÃ©Â·e pour pouvoir
-ajouter un livreÂ ! add-book-title = Ajouter un nouveau livre Ã  la collection
-add-book-action = Ajouter un livre add-book-cancel = Annuler add-book-add =
-Ajouter add-book-cover-help = Cliquez pour tÃ©lÃ©verser une couverture add-
-book-cover-format-not-supported = Le format de cette couverture n'est pas
-supportÃ©Â ! search-books-title = Chercher un livre dans la collection search-
-books-action = Chercher un livre search-books-clear = RÃ©initialiser search-
-books-search = Chercher search-books-no-result = Aucun livre ne correspondÂ !
-search-books-previous-page = PrÃ©cÃ©dent search-books-next-page = Suivant #
-title (string) The title of the book display-book-title = DÃ©tails pour Â«Â 
-{ $title }Â Â» update-book-requires-authentification = Vous devez Ãªtre
-authentifiÃ©Â·e pour pouvoir Ã©diter un livreÂ ! # isbn (string) The ISBN of
-the book update-book-title = Ãditer les informations de `{ $isbn }` update-
-book-action = Ãditer update-book-failure = Le livre n'a pas pu Ãªtre mis Ã 
-jourÂ ! update-book-success = Le livre a bien Ã©tÃ© mis Ã  jourÂ ! update-book-
-cancel = Annuler update-book-update = Enregistrer update-book-cover-help =
-Cliquez pour tÃ©lÃ©verser une nouvelle couverture update-book-cover-format-not-
-supported = Le format de cette couverture n'est pas supportÃ©Â ! book-already-
-exists = Ce livre est dÃ©jÃ  dans la collectionÂ ! # isbn (string) The ISBN of
-the book # url (string) The URL of the book book-added = Le livre {_$isbn_} a
-bien Ã©tÃ© ajoutÃ©Â ! book-not-found = Le livre n'a pas Ã©tÃ© trouvÃ©Â ! book-
+Ã©diter un livreÂ ! # isbn (string) The ISBN of the book update-book-title =
+Ãditer les informations de `{ $isbn }` update-book-action = Ãditer update-
+book-failure = Le livre n'a pas pu Ãªtre mis Ã  jourÂ ! update-book-success =
+Le livre a bien Ã©tÃ© mis Ã  jourÂ ! update-book-cancel = Annuler update-book-
+update = Enregistrer update-book-cover-help = Cliquez pour tÃ©lÃ©verser une
+nouvelle couverture update-book-cover-format-not-supported = Le format de cette
+couverture n'est pas supportÃ©Â ! book-already-exists = Ce livre est dÃ©jÃ 
+dans la collectionÂ ! # isbn (string) The ISBN of the book # url (string) The
+URL of the book book-added-html = Le livre {_$isbn_} a bien Ã©tÃ© ajoutÃ©Â ! #
+isbn (string) The ISBN of the book book-added-text = Le livre { $isbn } a bien
+Ã©tÃ© ajoutÃ©Â ! book-not-found = Le livre n'a pas Ã©tÃ© trouvÃ©Â ! book-
 cannot-be-added = Le livre n'a pas pu Ãªtre ajoutÃ©Â ! books-cannot-be-found =
 La recherche n'a pas pu Ãªtre effectuÃ©eÂ !
```

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/__init__.py` & `bl_hector-0.1.1/bl_hector/interfaces/to_http/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/__init__.py` & `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,15 +238,15 @@
     def book_already_exists(self, book: Book) -> None:
         self.__notify(self._("book-already-exists"), "info")
         self.redirect(url_for("books.display", isbn=str(book.isbn)))
 
     def book_added(self, book: Book) -> None:
         self.__notify(
             self._(
-                "book-added",
+                "book-added-html",
                 isbn=str(book.isbn),
                 url=url_for("books.display", isbn=str(book.isbn)),
             ),
             "success",
         )
         self.redirect(url_for("books.add"))
```

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug` & `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,13 @@
   section.section
     .container
       h1.title.is-3.has-text-centered= _("auth-login-title")
 
       .columns
         .column
         .column
-          //- Webauthn requires the page to be "properly" loaded.
-          .buttons(hx-boost="false")
+          .buttons
             each link in links
               a.button.is-fullwidth(href="#{url_for(link.route)}")
                 span.icon: i.fas(class="fa-#{link.icon}")
                 span= _("auth-login-method", method=link.label)
         .column
```

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/books/add.pug` & `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/books/add.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/books/display.pug` & `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/books/display.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug` & `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/books/search.pug` & `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/books/search.pug`

 * *Files 7% similar despite different names*

```diff
@@ -62,46 +62,52 @@
                   span.icon: i.fas.fa-search
                   span= _("search-books-search")
 
           if books is defined
             if books|length > 0
               #books.books
                 block books
-                  each book in books
-                    article.book.card(
-                      hx-get="#{next_page_url if loop.last else ''}"
-                      hx-trigger="#{'revealed' if loop.last else ''}"
-                      hx-swap="#{'beforeend' if loop.last else ''}"
-                      hx-target="#books"
-                      hx-indicator="#indicator"
-                      hx-boost="false"
-                    )
-                      .card-content
-                        .media
-                          .media-left(style="width: 5em")
-                            figure.image.cover.is-2by3
-                              img(src="#{book.cover or url_for('static', filename='img/placeholders/320x480.png')}" alt="Book cover")
-                          .media-content
-                            h2.title.is-4(title="#{book.title}")= book.title|truncate(20)
-                            p.subtitle.is-6
-                              each author in book.authors
-                                if author == book.authors[-1]
-                                  | #[a(href="#{url_for('books.search', author=author)}") #{author}]
+                  mixin book_content(book)
+                    .card-content
+                      .media
+                        .media-left(style="width: 5em")
+                          figure.image.cover.is-2by3
+                            img(src="#{book.cover or url_for('static', filename='img/placeholders/320x480.png')}" alt="Book cover")
+                        .media-content
+                          h2.title.is-4(title="#{book.title}")= book.title|truncate(20)
+                          p.subtitle.is-6
+                            each author in book.authors
+                              if author == book.authors[-1]
+                                | #[a(href="#{url_for('books.search', author=author)}") #{author}]
+                              else
+                                | #[a(href="#{url_for('books.search', author=author)}") #{author}], 
+                          p
+                            small
+                              | #[time(datetime="#{book.year}-01-01") #{book.year}] / 
+                              a(href="#{url_for('books.display', isbn=book.isbn)}") #{book.isbn}
+                              br
+                              each genre in book.genres
+                                if genre == book.genres[-1]
+                                  | #[a(href="#{url_for('books.search', genre=genre)}") #{genre}]
                                 else
-                                  | #[a(href="#{url_for('books.search', author=author)}") #{author}], 
-                            p
-                              small
-                                | #[time(datetime="#{book.year}-01-01") #{book.year}] / 
-                                a(href="#{url_for('books.display', isbn=book.isbn)}") #{book.isbn}
-                                br
-                                each genre in book.genres
-                                  if genre == book.genres[-1]
-                                    | #[a(href="#{url_for('books.search', genre=genre)}") #{genre}]
-                                  else
-                                    | #[a(href="#{url_for('books.search', genre=genre)}") #{genre}], 
+                                  | #[a(href="#{url_for('books.search', genre=genre)}") #{genre}], 
+
+                  each book in books
+                    if loop.last
+                      article.book.card(
+                        hx-get=next_page_url
+                        hx-trigger="revealed"
+                        hx-swap="beforeend"
+                        hx-target="#books"
+                        hx-indicator="#indicator"
+                      )
+                        +book_content(book)
+                    else
+                      article.book.card
+                        +book_content(book)
 
               #indicator.buttons.is-centered.mt-3.htmx-indicator.is-hidden(_="on load remove .is-hidden")
                   button.button.is-white.is-loading Loading indicator
 
               if previous_page_url or next_page_url:
                 .buttons.is-centered.mt-3(_="on load remove me")
                   if previous_page_url:
```

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/books/update.pug` & `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/books/update.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/error.pug` & `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/error.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/layout.pug` & `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/layout.pug`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     link(rel="stylesheet" href="#{url_for('static', filename='css/bulma@0.9.4.min.css')}")
     link(rel="stylesheet" href="#{url_for('static', filename='css/font-awesome@5.14.0.css')}")
     link(rel="stylesheet" href="#{url_for('static', filename='css/hector.css')}")
     block links
 
     block head_scripts
 
-  body(hx-boost="true")
+  body
     +navbar()
 
     .page
       - var messages = get_flashed_messages(with_categories=true)
       +flash(messages)
 
       block content
```

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug` & `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug` & `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug` & `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug` & `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug`

 * *Files 22% similar despite different names*

```diff
@@ -30,12 +30,19 @@
       .columns
         .column
         .column.has-text-centered
           form.box(method="POST")
             .field
               label.label= _("totp-login-password")
               .control
-                input.input(type="string" name="password")
+                input.input.has-text-centered.is-size-5(
+                  type="string"
+                  name="password"
+                  maxlength="6"
+                  pattern="[\d]{6}"
+                  oninvalid="#{'setCustomValidity(\'' + _('totp-login-pattern') + '\')'}"
+                  style="width: 7rem"
+                )
             .field
               .control
                 button.button.is-primary(type="submit")= _("totp-login-action")
         .column
```

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug` & `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug` & `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_json/__init__.py` & `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_json/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/to_terminal/__init__.py` & `bl_hector-0.1.1/bl_hector/interfaces/to_terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/to_terminal/as_json.py` & `bl_hector-0.1.1/bl_hector/interfaces/to_terminal/as_json.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/bl_hector/interfaces/utils.py` & `bl_hector-0.1.1/bl_hector/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a8/pyproject.toml` & `bl_hector-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "bl_hector"
-version = "0.1.0-alpha.8"
+version = "0.1.1"
 description = "A collection manager."
 authors = ["Tanguy Le Carrour <tanguy@bioneland.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
+repository = "https://git.easter-eggs.org/bioneland/hector"
 
 exclude = [
     "**/*_spec.py",
     "**/*_test.py",
     "**/*.feature",
     "**/use_cases/steps/*.py",
     "**/conftest.py",
@@ -47,15 +48,15 @@
 beautifulsoup4 = "^4.12.2"
 types-beautifulsoup4 = "^4.12.0"
 behave = "^1.2.6"
 types-requests = "^2.31.0"
 
 [tool.poetry.extras]
 webauthn = ["webauthn"]
-totp = ["otp"]
+totp = ["pyotp"]
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 
 [tool.black]
 line-length = 89
```

### Comparing `bl_hector-0.1.0a8/setup.py` & `bl_hector-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,29 +52,29 @@
  'isbnlib>=3.10.14,<4.0.0',
  'jinja2-fragments>=0.3.0,<0.4.0',
  'pypugjs>=5.9.12,<6.0.0',
  'requests>=2.31.0,<3.0.0',
  'typer>=0.9.0,<0.10.0']
 
 extras_require = \
-{'webauthn': ['webauthn>=1.8.1,<2.0.0']}
+{'totp': ['pyotp>=2.8.0,<3.0.0'], 'webauthn': ['webauthn>=1.8.1,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['hector = bl_hector.configuration.cli:cli']}
 
 setup_kwargs = {
     'name': 'bl-hector',
-    'version': '0.1.0a8',
+    'version': '0.1.1',
     'description': 'A collection manager.',
     'long_description': '# Hector — a collection manager\n\n## Install\n\nHector is available on PyPI under the name `bl_hector`.\nTo install, just run `python -m pip install bl_hector`.\n\n\n## Configure\n\nHector is configured using environment variables.\nSee [the `settings` module](bl_hector/infrastructure/settings.py) for\na comprehensive list of configuration variables.\n\nAll the variable names must be prefixed with `HECTOR_`. For instance\xa0:\n\n```console\n# The secret can be generated using the `secrets.token_hex()` function.\n$ export HECTOR_SECRET_KEY="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"\n\n# Additional Python database drivers might be required depending on the DSN.\n$ export HECTOR_DSN="sqlite:///data.sqlite"\n```\n\n\n## Authentication\n\nTo enable WebAuthn authentication, you must install extra dependencies (`bl-hector[webauthn]`)\nand enable it explicitly:\n\n```console\n$ export HECTOR_WEBAUTHN_ENABLED=1\n```\n\nTOTP authentication is provided to be able to login on servers that do not (yet) support\nthe `cryptography` module. You must install extra dependencies (`bl-hector[totp]`)\nand enable it explicitly by setting a base32 random secret:\n\n```console\n# The secret can be generated using the `pyotp.random_base32()` function.\n$ export HECTOR_TOTP_SECRET=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX\n```\n\nNote that it is a highly insecure way of authenticating, as anyone gaining access to your\nOTP generator would be able to login.\n\n\n## Initialise\n\nOnce configured, you must initialise Hector\'s database with the dedicated command:\n\n```console\n$ hector init-db\n```\n\n\n## Run\n\nHector being a Flask application, it can be run using any WSGI server,\nfor instance, with [Gunicorn](https://gunicorn.org):\n\n```console\n$ gunicorn --access-logfile="-" -w 4 -b 127.0.0.1:3000 "bl_hector.configuration.wsgi:app()"\n```\n\n\n## Contributing\n\nSee [CONTRIBUTING.md]() to set up a development environment.\n',
     'author': 'Tanguy Le Carrour',
     'author_email': 'tanguy@bioneland.org',
     'maintainer': None,
     'maintainer_email': None,
-    'url': None,
+    'url': 'https://git.easter-eggs.org/bioneland/hector',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
     'python_requires': '>=3.9,<4.0',
 }
```

### Comparing `bl_hector-0.1.0a8/PKG-INFO` & `bl_hector-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: bl-hector
-Version: 0.1.0a8
+Version: 0.1.1
 Summary: A collection manager.
+Home-page: https://git.easter-eggs.org/bioneland/hector
 License: AGPL-3.0-or-later
 Author: Tanguy Le Carrour
 Author-email: tanguy@bioneland.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -15,19 +16,20 @@
 Requires-Dist: Flask (>=2.3.2,<3.0.0)
 Requires-Dist: SQLAlchemy (>=2.0.15,<3.0.0)
 Requires-Dist: bl-seth (>=0.2.0,<0.3.0)
 Requires-Dist: bl3d (>=0.3.0,<0.4.0)
 Requires-Dist: fluent.runtime (>=0.4.0,<0.5.0)
 Requires-Dist: isbnlib (>=3.10.14,<4.0.0)
 Requires-Dist: jinja2-fragments (>=0.3.0,<0.4.0)
-Requires-Dist: pyotp (>=2.8.0,<3.0.0)
+Requires-Dist: pyotp (>=2.8.0,<3.0.0); extra == "totp"
 Requires-Dist: pypugjs (>=5.9.12,<6.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: webauthn (>=1.8.1,<2.0.0); extra == "webauthn"
+Project-URL: Repository, https://git.easter-eggs.org/bioneland/hector
 Description-Content-Type: text/markdown
 
 # Hector — a collection manager
 
 ## Install
 
 Hector is available on PyPI under the name `bl_hector`.
```

