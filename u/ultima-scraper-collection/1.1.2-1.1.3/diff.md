# Comparing `tmp/ultima_scraper_collection-1.1.2.tar.gz` & `tmp/ultima_scraper_collection-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_collection-1.1.2.tar", max compression
+gzip compressed data, was "ultima_scraper_collection-1.1.3.tar", max compression
```

## Comparing `ultima_scraper_collection-1.1.2.tar` & `ultima_scraper_collection-1.1.3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0      788 2023-05-31 21:42:12.599928 ultima_scraper_collection-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      293 2023-02-26 12:00:14.727199 ultima_scraper_collection-1.1.2/ultima_scraper_collection/__init__.py
--rw-r--r--   0        0        0        0 2023-02-26 11:42:41.007744 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/__init__.py
--rw-r--r--   0        0        0        0 2023-02-26 11:42:54.441267 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/__init__.py
--rw-r--r--   0        0        0        0 2023-03-06 01:27:30.462039 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/__init__.py
--rw-r--r--   0        0        0        0 2023-03-04 04:03:12.661102 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/__init__.py
--rw-r--r--   0        0        0        0 2023-02-26 11:42:54.461267 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/__init__.py
--rw-r--r--   0        0        0       38 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/README
--rw-r--r--   0        0        0     2150 2023-03-05 04:16:43.534861 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/script.py.mako
--rw-r--r--   0        0        0      662 2023-03-05 04:20:42.303797 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py
--rw-r--r--   0        0        0      941 2023-03-05 04:20:47.520466 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py
--rw-r--r--   0        0        0      861 2022-04-25 23:29:43.807242 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py
--rw-r--r--   0        0        0     3182 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py
--rw-r--r--   0        0        0     1651 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py
--rw-r--r--   0        0        0     1415 2023-03-05 04:20:57.727140 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py
--rw-r--r--   0        0        0     2201 2023-03-03 17:13:51.407142 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini
--rw-r--r--   0        0        0    77824 2023-02-14 03:46:10.695467 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db
--rw-r--r--   0        0        0        0 2023-03-10 12:28:15.033139 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 12:28:22.753355 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 12:27:11.408006 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/__init__.py
--rw-r--r--   0        0        0     2296 2023-03-10 12:28:05.882882 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/script.py.mako
--rw-r--r--   0        0        0     1769 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py
--rw-r--r--   0        0        0     1649 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py
--rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py
--rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py
--rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py
--rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini
--rw-r--r--   0        0        0      493 2023-03-10 12:30:45.700616 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/messages.py
--rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db
--rw-r--r--   0        0        0     2288 2023-03-10 12:32:59.654189 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/script.py.mako
--rw-r--r--   0        0        0     1762 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py
--rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py
--rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py
--rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py
--rw-r--r--   0        0        0     1643 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py
--rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini
--rw-r--r--   0        0        0      488 2023-03-10 12:32:58.467491 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/posts.py
--rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db
--rw-r--r--   0        0        0     2294 2023-03-10 12:32:46.997189 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/script.py.mako
--rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py
--rw-r--r--   0        0        0     1647 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py
--rw-r--r--   0        0        0     1766 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py
--rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py
--rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py
--rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini
--rw-r--r--   0        0        0      490 2023-03-10 12:32:57.520800 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/stories.py
--rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db
--rw-r--r--   0        0        0        0 2022-12-05 14:27:20.696663 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/__init__.py
--rw-r--r--   0        0        0     1611 2023-04-20 22:10:05.846209 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py
--rw-r--r--   0        0        0     2764 2023-05-08 21:50:28.707049 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py
--rw-r--r--   0        0        0     2073 2023-04-20 22:22:10.068827 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py
--rw-r--r--   0        0        0     9499 2023-05-14 03:29:16.005497 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py
--rw-r--r--   0        0        0      442 2023-03-12 15:01:42.766490 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/database_manager.py
--rw-r--r--   0        0        0        0 2023-02-26 16:06:18.482305 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/datascraper_manager/__init__.py
--rw-r--r--   0        0        0     1576 2023-05-22 07:47:32.668760 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py
--rw-r--r--   0        0        0        0 2023-02-26 16:04:46.426896 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/datascraper_manager/datascrapers/__init__.py
--rw-r--r--   0        0        0     5390 2023-05-14 03:41:06.309010 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py
--rw-r--r--   0        0        0     5641 2023-05-31 12:09:04.884552 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py
--rw-r--r--   0        0        0    10728 2023-05-31 18:34:23.965718 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/download_manager.py
--rw-r--r--   0        0        0    13669 2023-05-14 19:55:15.091076 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/filesystem_manager.py
--rw-r--r--   0        0        0     6102 2023-03-05 04:29:30.964171 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/legacy_code.py
--rw-r--r--   0        0        0        0 2023-01-26 08:21:03.864558 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/metadata_manager/__init__.py
--rw-r--r--   0        0        0    27937 2023-05-22 04:54:03.366424 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py
--rw-r--r--   0        0        0     7080 2023-05-22 08:09:26.097930 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/option_manager.py
--rw-r--r--   0        0        0        0 2023-03-14 06:55:35.872202 ultima_scraper_collection-1.1.2/ultima_scraper_collection/modules/__init__.py
--rw-r--r--   0        0        0    18213 2023-05-31 11:19:09.143046 ultima_scraper_collection-1.1.2/ultima_scraper_collection/modules/module_streamliner.py
--rw-r--r--   0        0        0        0 2023-02-26 16:07:35.717380 ultima_scraper_collection-1.1.2/ultima_scraper_collection/py.typed
--rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 ultima_scraper_collection-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      809 2023-06-15 09:42:46.743215 ultima_scraper_collection-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      293 2023-02-26 12:00:14.727199 ultima_scraper_collection-1.1.3/ultima_scraper_collection/__init__.py
+-rw-r--r--   0        0        0     3098 2023-06-15 09:44:14.174056 ultima_scraper_collection-1.1.3/ultima_scraper_collection/config.py
+-rw-r--r--   0        0        0        0 2023-02-26 11:42:41.007744 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-26 11:42:54.441267 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-06 01:27:30.462039 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-04 04:03:12.661102 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-26 11:42:54.461267 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/__init__.py
+-rw-r--r--   0        0        0       38 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/README
+-rw-r--r--   0        0        0     2150 2023-03-05 04:16:43.534861 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0      662 2023-03-05 04:20:42.303797 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py
+-rw-r--r--   0        0        0      941 2023-03-05 04:20:47.520466 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py
+-rw-r--r--   0        0        0      861 2022-04-25 23:29:43.807242 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py
+-rw-r--r--   0        0        0     3182 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py
+-rw-r--r--   0        0        0     1651 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py
+-rw-r--r--   0        0        0     1415 2023-03-05 04:20:57.727140 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py
+-rw-r--r--   0        0        0     2201 2023-03-03 17:13:51.407142 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini
+-rw-r--r--   0        0        0    77824 2023-02-14 03:46:10.695467 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db
+-rw-r--r--   0        0        0        0 2023-03-10 12:28:15.033139 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-10 12:28:22.753355 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-10 12:27:11.408006 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/__init__.py
+-rw-r--r--   0        0        0     2296 2023-03-10 12:28:05.882882 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0     1769 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py
+-rw-r--r--   0        0        0     1649 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py
+-rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py
+-rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py
+-rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py
+-rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini
+-rw-r--r--   0        0        0      493 2023-03-10 12:30:45.700616 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/messages.py
+-rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db
+-rw-r--r--   0        0        0     2288 2023-03-10 12:32:59.654189 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0     1762 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py
+-rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py
+-rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py
+-rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py
+-rw-r--r--   0        0        0     1643 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py
+-rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini
+-rw-r--r--   0        0        0      488 2023-03-10 12:32:58.467491 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/posts.py
+-rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db
+-rw-r--r--   0        0        0     2294 2023-03-10 12:32:46.997189 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py
+-rw-r--r--   0        0        0     1647 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py
+-rw-r--r--   0        0        0     1766 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py
+-rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py
+-rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py
+-rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini
+-rw-r--r--   0        0        0      490 2023-03-10 12:32:57.520800 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/stories.py
+-rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db
+-rw-r--r--   0        0        0        0 2022-12-05 14:27:20.696663 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/__init__.py
+-rw-r--r--   0        0        0     1611 2023-06-03 17:34:00.273754 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py
+-rw-r--r--   0        0        0     2764 2023-05-08 21:50:28.707049 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py
+-rw-r--r--   0        0        0     2073 2023-04-20 22:22:10.068827 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py
+-rw-r--r--   0        0        0     9956 2023-06-15 07:56:54.052868 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py
+-rw-r--r--   0        0        0      442 2023-03-12 15:01:42.766490 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/database_manager.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:06:18.482305 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/datascraper_manager/__init__.py
+-rw-r--r--   0        0        0     1576 2023-05-22 07:47:32.668760 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:04:46.426896 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/datascraper_manager/datascrapers/__init__.py
+-rw-r--r--   0        0        0     5344 2023-06-15 07:48:16.103922 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py
+-rw-r--r--   0        0        0     5608 2023-06-15 07:49:47.587365 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py
+-rw-r--r--   0        0        0    10668 2023-06-15 09:26:42.852114 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/download_manager.py
+-rw-r--r--   0        0        0    13669 2023-05-14 19:55:15.091076 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/filesystem_manager.py
+-rw-r--r--   0        0        0        0 2023-01-26 08:21:03.864558 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/metadata_manager/__init__.py
+-rw-r--r--   0        0        0    29119 2023-06-10 18:24:38.563431 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py
+-rw-r--r--   0        0        0     7134 2023-06-01 21:57:38.888076 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/option_manager.py
+-rw-r--r--   0        0        0        0 2023-03-14 06:55:35.872202 ultima_scraper_collection-1.1.3/ultima_scraper_collection/modules/__init__.py
+-rw-r--r--   0        0        0    18351 2023-06-15 09:30:35.138093 ultima_scraper_collection-1.1.3/ultima_scraper_collection/modules/module_streamliner.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:07:35.717380 ultima_scraper_collection-1.1.3/ultima_scraper_collection/py.typed
+-rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 ultima_scraper_collection-1.1.3/PKG-INFO
```

### Comparing `ultima_scraper_collection-1.1.2/pyproject.toml` & `ultima_scraper_collection-1.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ultima-scraper-collection"
-version = "1.1.2"
+version = "1.1.3"
 description = ""
 authors = [
     "DIGITALCRIMINALS <89371864+digitalcriminals@users.noreply.github.com>",
 ]
 packages = [{include = "ultima_scraper_collection"}]
 include = ["ultima_scraper_collection/py.typed"]
 
@@ -14,14 +14,15 @@
 sqlalchemy = "^2.0.1"
 psycopg2 = "^2.9.5"
 alembic = "^1.9.2"
 tqdm = "^4.65.0"
 ultima-scraper-api = "^1.1.1"
 ultima-scraper-renamer = "^1.1.0"
 ffmpeg-python = "^0.2.0"
+pydantic = "^1.10.9"
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.2"
 black = {version = "^23.3.0", allow-prereleases = true}
 
 [tool.semantic_release]
 version_toml = "pyproject.toml:tool.poetry.version"
```

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,19 @@
 
 import ultima_scraper_api
 from alembic import command
 from alembic.config import Config
 from alembic.migration import MigrationContext
 from sqlalchemy import create_engine, func
 from sqlalchemy.orm import DeclarativeBase, scoped_session, sessionmaker
-
 from ultima_scraper_collection.managers.database_manager.connections.sqlite.models import (
     user_database,
 )
 
 if TYPE_CHECKING:
-
     from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
         ContentMetadata,
     )
 
 user_types = ultima_scraper_api.user_types
 
 
@@ -68,15 +66,14 @@
         return scoped_session(self.session_factory)
 
     def execute(self, statement: Any):
         result = self.session.execute(statement)
         return result
 
     def generate_migration(self):
-
         if not self.session.bind:
             return
         conn = self.session.bind.engine.connect()
         context = MigrationContext.configure(conn)
         current_rev = context.get_current_revision()
         alembic_cfg = Config(self.migration_directory.joinpath("alembic.ini"))
         alembic_cfg.set_main_option(
@@ -90,15 +87,14 @@
             _ggg = command.revision(alembic_cfg, autogenerate=True, head=current_rev)
         self.run_migrations()
         return True
 
     def run_migrations(self, legacy: bool = False) -> None:
         while True:
             try:
-
                 migration_directory = (
                     self.alembic_directory.parent.joinpath("migration")
                     if legacy
                     else self.migration_directory
                 )
 
                 alembic_cfg = Config(migration_directory.joinpath("alembic.ini"))
@@ -140,18 +136,25 @@
         for post in datas:
             if post.api_type:
                 api_type = post.api_type
             api_table = database.table_picker(api_type)
             if not api_table:
                 return
             post_id = post.content_id
-            created_at_string = post.created_at_string
+            post_created_at_string = post.created_at_string
             date_object = None
-            if created_at_string:
-                date_object = datetime.strptime(created_at_string, "%d-%m-%Y %H:%M:%S")
+            if post_created_at_string:
+                try:
+                    date_object = datetime.fromisoformat(post_created_at_string)
+                    pass
+                except Exception as _e:
+                    date_object = datetime.strptime(
+                        post_created_at_string, "%d-%m-%Y %H:%M:%S"
+                    )
+                    pass
             result = database_session.query(api_table)
             post_db = result.filter_by(post_id=post_id).first()
             if not post_db:
                 post_db = api_table()
             else:
                 pass
             if api_type == "Messages":
@@ -163,17 +166,20 @@
             post_db.archived = post.archived
             if date_object:
                 post_db.created_at = date_object
             database_session.add(post_db)
             for media in post.medias:
                 if media.media_type == "Texts":
                     continue
-                created_at = media.created_at
-                if not isinstance(created_at, datetime):
-                    date_object = datetime.strptime(created_at, "%d-%m-%Y %H:%M:%S")
+                media_created_at_string = media.created_at
+                if not isinstance(media_created_at_string, datetime):
+                    if isinstance(media_created_at_string, int):
+                        date_object = datetime.fromtimestamp(media_created_at_string)
+                    else:
+                        date_object = datetime.fromisoformat(media_created_at_string)
                 media_id = media.id
                 result = database_session.query(database.media_table)
                 media_db = result.filter_by(post_id=post_id, media_id=media_id).first()
                 if not media_db:
                     media_db = result.filter_by(
                         filename=media.filename, created_at=date_object
                     ).first()
```

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 from pathlib import Path
 from typing import Any, Union
 
-from ultima_scraper_renamer.reformat import ReformatManager
-from ultima_scraper_api.apis.fansly.classes.auth_model import create_auth
+from ultima_scraper_api.apis.fansly.classes.auth_model import AuthModel
 from ultima_scraper_api.apis.fansly.classes.message_model import create_message
 from ultima_scraper_api.apis.fansly.classes.post_model import create_post
 from ultima_scraper_api.apis.fansly.classes.story_model import create_story
 from ultima_scraper_api.apis.fansly.classes.user_model import create_user
 from ultima_scraper_api.apis.fansly.fansly import FanslyAPI
-
 from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
     ContentMetadata,
 )
 from ultima_scraper_collection.managers.option_manager import OptionManager
 from ultima_scraper_collection.modules.module_streamliner import StreamlinedDatascraper
+from ultima_scraper_renamer.reformat import ReformatManager
 
 
 class FanslyDataScraper(StreamlinedDatascraper):
     def __init__(self, api: FanslyAPI, option_manager: OptionManager) -> None:
         self.api = api
         self.option_manager = option_manager
         StreamlinedDatascraper.__init__(self, self)
 
     # Scrapes the API for content
     async def media_scraper(
         self,
         post_result: Union[create_story, create_post, create_message],
         subscription: create_user,
-        formatted_directory: Path,
         api_type: str,
     ) -> dict[str, Any]:
         authed = subscription.get_authed()
         api = authed.api
         site_settings = api.get_site_settings()
         if not site_settings:
             return {}
@@ -99,26 +97,26 @@
             temp_master_set.append(
                 await subscription.get_collection_content(collection)
             )
         return temp_master_set
 
     async def get_all_subscriptions(
         self,
-        authed: create_auth,
+        authed: AuthModel,
         identifiers: list[int | str] = [],
         refresh: bool = True,
     ):
         """
-        get_all_subscriptions(authed: create_auth, identifiers: list[int | str] = [], refresh: bool = True)
+        get_all_subscriptions(authed: AuthModel, identifiers: list[int | str] = [], refresh: bool = True)
 
         This function returns a list of all subscriptions, including both subscriptions and followings,
         from the given authenticated user.
 
         Arguments:
-        authed (create_auth): An instance of the create_auth class.
+        authed (AuthModel): An instance of the AuthModel class.
         identifiers (list[int | str], optional): A list of identifiers (username or id) for the subscriptions. Defaults to an empty list.
         refresh (bool, optional): A flag indicating whether to refresh the list of subscriptions. Defaults to True.
 
         Returns:
         list[create_subscription]: A list of all subscriptions, including both subscriptions and followings, from the authenticated user.
         """
         authed.followed_users = await authed.get_followings(identifiers=identifiers)
```

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,51 +1,48 @@
 from pathlib import Path
 from typing import Any, Union
 
-from ultima_scraper_api.apis.onlyfans.classes.auth_model import create_auth
+from ultima_scraper_api.apis.onlyfans.classes.auth_model import AuthModel
 from ultima_scraper_api.apis.onlyfans.classes.hightlight_model import create_highlight
 from ultima_scraper_api.apis.onlyfans.classes.message_model import create_message
 from ultima_scraper_api.apis.onlyfans.classes.post_model import create_post
 from ultima_scraper_api.apis.onlyfans.classes.story_model import create_story
 from ultima_scraper_api.apis.onlyfans.classes.user_model import create_user
 from ultima_scraper_api.apis.onlyfans.onlyfans import OnlyFansAPI
-from ultima_scraper_renamer.reformat import ReformatManager
-
 from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
     ContentMetadata,
 )
 from ultima_scraper_collection.managers.option_manager import OptionManager
 from ultima_scraper_collection.modules.module_streamliner import StreamlinedDatascraper
+from ultima_scraper_renamer.reformat import ReformatManager
 
 
 class OnlyFansDataScraper(StreamlinedDatascraper):
     def __init__(self, api: OnlyFansAPI, option_manager: OptionManager) -> None:
         self.api = api
         self.option_manager = option_manager
         StreamlinedDatascraper.__init__(self, self)
 
     # Scrapes the API for content
     async def media_scraper(
         self,
         post_result: Union[create_story, create_post, create_message],
         subscription: create_user,
-        formatted_directory: Path,
         api_type: str,
     ) -> dict[str, Any]:
+        api_type = self.api.convert_api_type_to_key(post_result)
         authed = subscription.get_authed()
         api = authed.api
         site_settings = api.get_site_settings()
         if not site_settings:
             return {}
         new_set: dict[str, Any] = {"content": []}
         directories: list[Path] = []
         if api_type == "Stories":
             pass
-        if api_type == "Archived":
-            pass
         if api_type == "Posts":
             pass
         if api_type == "Messages":
             pass
         from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
             Extractor,
         )
@@ -105,25 +102,25 @@
         temp_master_set = await subscription.get_posts()
         # get_archived_posts uses normal posts
         await subscription.get_archived_posts()
         return temp_master_set
 
     async def get_all_subscriptions(
         self,
-        authed: create_auth,
+        authed: AuthModel,
         identifiers: list[int | str] = [],
         refresh: bool = True,
     ):
         """
-        get_all_subscriptions(authed: create_auth, identifiers: list[int | str] = [], refresh: bool = True)
+        get_all_subscriptions(authed: AuthModel, identifiers: list[int | str] = [], refresh: bool = True)
 
         This function returns a list of all subscriptions from the given authenticated user.
 
         Arguments:
-        authed (create_auth): An instance of the create_auth class.
+        authed (AuthModel): An instance of the AuthModel class.
         identifiers (list[int | str], optional): A list of identifiers (username or id) for the subscriptions. Defaults to an empty list.
         refresh (bool, optional): A flag indicating whether to refresh the list of subscriptions. Defaults to True.
 
         Returns:
         list[create_subscription]: A list of all subscriptions, sorted by expiredAt, from the authenticated user.
         """
         subscriptions = await authed.get_subscriptions(
```

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/download_manager.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/download_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import asyncio
 import copy
 from pathlib import Path
 from urllib.parse import urlparse
 
 import ffmpeg
 from aiohttp import ClientResponse
+from ultima_scraper_api import auth_types
 from ultima_scraper_api.helpers import main_helper
-from ultima_scraper_api.managers.session_manager import SessionManager
 from ultima_scraper_renamer.reformat import ReformatManager
 
 from ultima_scraper_collection.managers.database_manager.connections.sqlite.models.media_model import (
     TemplateMediaModel,
 )
 from ultima_scraper_collection.managers.filesystem_manager import FilesystemManager
 from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
@@ -18,39 +18,38 @@
     MediaMetadata,
 )
 
 
 class DownloadManager:
     def __init__(
         self,
+        authed: auth_types,
         filesystem_manager: FilesystemManager,
-        session_manager: SessionManager,
         content_list: set[ContentMetadata] = set(),
         reformat: bool = True,
     ) -> None:
+        self.authed = authed
         self.filesystem_manager = filesystem_manager
-        self.session_manager = session_manager
+        self.session_manager = self.authed.session_manager
         self.content_list: set[ContentMetadata] = content_list
         self.errors: list[TemplateMediaModel] = []
         self.reformat = reformat
-        self.reformat_manager = ReformatManager(
-            session_manager.auth, filesystem_manager
-        )
+        self.reformat_manager = ReformatManager(self.authed, filesystem_manager)
 
     async def bulk_download(self):
-        final_list: list[MediaMetadata] = [
+        final_list = [
             self.download(media_item)
             for download_item in self.content_list
             for media_item in download_item.medias
         ]
         _result = await asyncio.gather(*final_list, return_exceptions=True)
 
     async def drm_download(self, download_item: MediaMetadata):
         content_metadata = download_item.__content_metadata__
-        authed = self.session_manager.auth
+        authed = self.authed
         site_settings = authed.get_api().get_site_settings()
         reformat_manager = ReformatManager(authed, self.filesystem_manager)
         drm = authed.drm
         media_item = download_item.__raw__
         assert drm and media_item
         mpd = await drm.get_mpd(media_item)
         pssh = await drm.get_pssh(mpd)
@@ -103,15 +102,15 @@
         p_url = urlparse(download_item.urls[0])
 
         subdomain = p_url.hostname.split(".")[0]
         if any(subdomain in nm for nm in matches):
             return
         download_item.__db_item__ = db_media
 
-        authed = self.session_manager.auth
+        authed = self.authed
         authed_drm = authed.drm
 
         async with self.session_manager.semaphore:
             while attempt < self.session_manager.max_attempts + 1:
                 try:
                     if download_item.drm:
                         if not authed_drm:
@@ -169,15 +168,15 @@
                         if not formatted:
                             pass
                         final_size = download_path.stat().st_size
                     timestamp = db_media.created_at.timestamp()
                     await main_helper.format_file(
                         download_path, timestamp, self.reformat
                     )
-                    db_media.size = final_size
+                    db_media.size = download_item.size = final_size
                     db_media.downloaded = True
                     break
                 except asyncio.TimeoutError as _e:
                     continue
 
     async def writer(
         self,
```

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/filesystem_manager.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/filesystem_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 from datetime import datetime
 from pathlib import Path
 from typing import Any
 from urllib.parse import ParseResult, urlparse
 
 import ultima_scraper_api
 from sqlalchemy import inspect
-
 from ultima_scraper_collection.managers.database_manager.connections.sqlite.sqlite_database import (
     DBCollection,
     SqliteDatabase,
 )
 from ultima_scraper_collection.managers.database_manager.database_manager import (
     DatabaseManager,
 )
 from ultima_scraper_collection.managers.filesystem_manager import FilesystemManager
 
 api_types = ultima_scraper_api.api_types
 user_types = ultima_scraper_api.user_types
 content_types = ultima_scraper_api.content_types
 from ultima_scraper_api.classes.prepare_metadata import format_content
 from ultima_scraper_api.helpers import main_helper
-
 from ultima_scraper_collection.managers.database_manager.connections.sqlite.models.api_model import (
     ApiModel,
 )
 from ultima_scraper_collection.managers.database_manager.connections.sqlite.models.user_database import (
     messages_table,
 )
 
@@ -102,44 +100,53 @@
             final_preview_ids = self.item.previews
         else:
             final_preview_ids = []
         return final_preview_ids
 
     def get_date(self):
         temp_date = self.item.createdAt
-        default_date = datetime.strftime(datetime.utcnow(), "%d-%m-%Y %H:%M:%S")
+        assert temp_date
+        if isinstance(temp_date, str):
+            try:
+                temp_date = float(temp_date)
+            except:
+                pass
+        default_date = datetime.utcnow()
         if temp_date == "-001-11-30T00:00:00+00:00":
-            final_date_string = default_date
-            date_object = datetime.strptime(default_date, "%d-%m-%Y %H:%M:%S")
+            date_object = default_date
         else:
             if not temp_date:
                 temp_date = default_date
             if isinstance(temp_date, int):
                 timestamp = float(temp_date)
                 date_object = datetime.fromtimestamp(timestamp)
+            elif isinstance(temp_date, float):
+                date_object = datetime.fromtimestamp(temp_date)
             else:
                 date_object = datetime.fromisoformat(temp_date)
-            final_date_string = date_object.replace(tzinfo=None).strftime(
-                "%d-%m-%Y %H:%M:%S"
-            )
+        final_date_string = date_object.isoformat()
         return final_date_string
 
     def get_medias(self, content_metadata: "ContentMetadata"):
         final_assets: list[MediaMetadata] = []
         for asset_metadata in self.item.media:
             raw_media_type = asset_metadata["type"]
             if "mimetype" in asset_metadata:
                 raw_media_type: str = asset_metadata["mimetype"].split("/")[0]
             author = self.item.get_author()
             media_type = author.get_api().MediaTypes().find_by_value(raw_media_type)
+            if "createdAt" in asset_metadata:
+                media_created_at = asset_metadata["createdAt"]
+            else:
+                media_created_at = content_metadata.created_at_string
             new_asset = MediaMetadata(
                 asset_metadata["id"],
                 media_type,
                 content_metadata,
-                created_at=content_metadata.created_at_string,
+                created_at=media_created_at,
             )
             main_url = self.item.url_picker(asset_metadata)
             preview_url = self.item.preview_url_picker(asset_metadata)
             authed = author.get_authed()
             if authed.drm:
                 new_asset.drm = bool(authed.drm.has_drm(asset_metadata))
             new_asset.urls = []
@@ -387,15 +394,33 @@
                     pass
                 if not final_content_type:
                     # If we get an key error here, we need to move the json file to correct folder or we can resolve it by getting content_type by looking at the directory path
                     # directory_set = set()
                     # merged = merge_statuses(new_metadata_set)
                     # for item in merged:
                     #     directory_set.add(item["directory"])
-                    final_content_type = new_metadata_set["content_type"]
+                    if (
+                        "type" in new_metadata_set
+                        and "content_type" not in new_metadata_set
+                    ):
+                        item = new_metadata_set["valid"][0]
+                        directory = item["directory"]
+                        content_types = self.subscription.get_api().ContentTypes()
+                        temp_content_type = content_types.path_to_key(Path(directory))
+                        if all(
+                            temp_content_type
+                            == content_types.path_to_key(Path(item["directory"]))
+                            for item in new_metadata_set["valid"]
+                        ):
+                            final_content_type = temp_content_type
+                    else:
+                        final_content_type = new_metadata_set["content_type"]
+            assert (
+                final_content_type
+            ), "Content type (Posts,etc) not set before fixing JSON"
             final_metadata_set = {}
             content_json = {}
             if isinstance(new_metadata_set, list):
                 if len(new_metadata_set) > 1:
                     pass
                 for temp_set in new_metadata_set:
                     content_json[temp_set["type"]] = {
```

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/option_manager.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/option_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,29 +60,29 @@
                 self.final_choices = [
                     key
                     for choice in final_list
                     for key in self.items
                     if choice.lower() == key.lower()
                 ]
             case "profiles":
-                self.item_keys = [x.auth_details.username for x in self.items]
+                self.item_keys = [x.get_auth_details().username for x in self.items]
                 my_string = " | ".join(
                     map(
-                        lambda x: f"{self.items.index(x)+1} = {x.auth_details.username}",
+                        lambda x: f"{self.items.index(x)+1} = {x.get_auth_details().username}",
                         self.items,
                     )
                 )
                 final_string = f"{final_string} | {my_string}"
                 self.string = final_string
                 final_list = await self.choose_option()
                 self.final_choices = [
                     key
                     for choice in final_list
                     for key in self.items
-                    if choice.lower() == key.auth_details.username.lower()
+                    if choice.lower() == key.get_auth_details().username.lower()
                 ]
                 set1 = set(self.final_choices)
                 set2 = set(self.items)
                 difference = list(set2 - set1)
                 for auth in difference:
                     await auth.session_manager.active_session.close()
             case "subscriptions":
@@ -177,11 +177,11 @@
                 or self.auto_choice[0].lower() == "0"
             )
         ):
             status = True
         return status
 
     def return_auto_choice(self):
-        identifiers = []
+        identifiers: list[int | str] | int | str | bool = []
         if isinstance(self.auto_choice, list):
             identifiers = [x for x in self.auto_choice if not isinstance(x, bool)]
         return identifiers
```

### Comparing `ultima_scraper_collection-1.1.2/ultima_scraper_collection/modules/module_streamliner.py` & `ultima_scraper_collection-1.1.3/ultima_scraper_collection/modules/module_streamliner.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,30 +4,29 @@
 from itertools import product
 from typing import Any, Optional
 
 import ultima_scraper_api
 import ultima_scraper_api.classes.make_settings as make_settings
 from sqlalchemy.exc import OperationalError
 from tqdm.asyncio import tqdm_asyncio
-from ultima_scraper_renamer import renamer
-
 from ultima_scraper_collection.managers.database_manager.connections.sqlite.models.api_model import (
     ApiModel,
 )
 from ultima_scraper_collection.managers.database_manager.connections.sqlite.sqlite_database import (
     DBCollection,
 )
 from ultima_scraper_collection.managers.database_manager.database_manager import (
     DatabaseManager,
 )
 from ultima_scraper_collection.managers.download_manager import DownloadManager
 from ultima_scraper_collection.managers.filesystem_manager import FilesystemManager
 from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
     MetadataManager,
 )
+from ultima_scraper_renamer import renamer
 
 auth_types = ultima_scraper_api.auth_types
 user_types = ultima_scraper_api.user_types
 message_types = ultima_scraper_api.message_types
 error_types = ultima_scraper_api.error_types
 subscription_types = ultima_scraper_api.subscription_types
 
@@ -112,15 +111,21 @@
                 user.scrape_whitelist.append("Messages")
                 for user in chat_users
                 if not await user.is_subscribed() or not scraping_subscriptions
             ]
             [valid_user_list.add(x) for x in chat_users]
 
         if available_jobs.paid_contents:
+            from ultima_scraper_api.apis.onlyfans.classes.auth_model import (
+                AuthModel as OnlyFansAuthModel,
+            )
+
             for authed in self.datascraper.api.auths:
+                if not isinstance(authed, OnlyFansAuthModel):
+                    continue
                 paid_contents = await authed.get_paid_content()
                 if not isinstance(paid_contents, error_types):
                     for paid_content in paid_contents:
                         author = paid_content.get_author()
                         if identifiers:
                             found = await author.match_identifiers(identifiers)
                             if not found:
@@ -187,15 +192,17 @@
                     pass
                 case _:
                     raise Exception(f"{content_type} is an invalid choice")
         # Adding paid content and removing duplicates by id
         if isinstance(user, ultima_scraper_api.onlyfans_classes.user_model.create_user):
             for paid_content in await user.get_paid_contents(content_type):
                 temp_master_set.append(paid_content)
-            temp_master_set = list({getattr(obj,"id"): obj for obj in temp_master_set}.values())
+            temp_master_set = list(
+                {getattr(obj, "id"): obj for obj in temp_master_set}.values()
+            )
         await self.process_scraped_content(
             temp_master_set, content_type, user, metadata_manager
         )
         current_job.done = True
 
     async def process_scraped_content(
         self,
@@ -219,15 +226,14 @@
         with authed.get_pool() as pool:
             print(f"Processing Scraped {api_type}")
             tasks = pool.starmap(
                 self.datascraper.media_scraper,
                 product(
                     master_set,
                     [subscription],
-                    [subscription_directory_manager.root_download_directory],
                     [api_type],
                 ),
             )
             settings = {"colour": "MAGENTA"}
             unrefined_set: list[dict[str, Any]] = await tqdm_asyncio.gather(
                 *tasks, **settings
             )
@@ -317,16 +323,16 @@
                                 final_download_set.add(content_metadata)
                                 [
                                     final_media_set.add(x.id)
                                     for x in content_metadata.medias
                                 ]
                                 total_media_count += len(content_metadata.medias)
                 download_manager = DownloadManager(
+                    performer.get_authed(),
                     filesystem_manager,
-                    performer.get_session_manager(),
                     final_download_set,
                     global_settings.helpers.reformat_media,
                 )
                 download_count = len(final_media_set)
                 duplicate_count = total_media_count - download_count
                 string = "Processing Download:\n"
                 string += f"Name: {performer.username} | Type: {api_type} | Downloading: {download_count} | Total: {total_media_count} | Duplicates: {duplicate_count} | Directory: {directory}\n"
@@ -376,17 +382,16 @@
         auth: auth_types,
         datascraper: datascraper_types,
         site_settings: make_settings.SiteSettings,
         identifiers: list[int | str] | list[str] = [],
     ) -> tuple[bool, list[user_types]]:
         status = False
         subscriptions: list[subscription_types] = []
-        auth = await auth.login()
 
-        if auth.check_authed() and site_settings:
+        if auth.is_authed() and site_settings:
             authed = auth
             # metadata_filepath = (
             #     authed.directory_manager.profile.metadata_directory.joinpath(
             #         "Mass Messages.json"
             #     )
             # )
             # if authed.isPerformer:
```

### Comparing `ultima_scraper_collection-1.1.2/PKG-INFO` & `ultima_scraper_collection-1.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-collection
-Version: 1.1.2
+Version: 1.1.3
 Summary: 
 Author: DIGITALCRIMINALS
 Author-email: 89371864+digitalcriminals@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: alembic (>=1.9.2,<2.0.0)
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
 Requires-Dist: psycopg2 (>=2.9.5,<3.0.0)
+Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: sqlalchemy (>=2.0.1,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: ultima-scraper-api (>=1.1.1,<2.0.0)
 Requires-Dist: ultima-scraper-renamer (>=1.1.0,<2.0.0)
```

