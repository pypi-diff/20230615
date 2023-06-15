# Comparing `tmp/ultima_scraper_api-1.1.3.tar.gz` & `tmp/ultima_scraper_api-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_api-1.1.3.tar", max compression
+gzip compressed data, was "ultima_scraper_api-1.1.4.tar", max compression
```

## Comparing `ultima_scraper_api-1.1.3.tar` & `ultima_scraper_api-1.1.4.tar`

### file list

```diff
@@ -1,59 +1,61 @@
--rw-r--r--   0        0        0     1193 2023-05-31 21:40:39.725354 ultima_scraper_api-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      175 2022-12-03 17:24:36.799421 ultima_scraper_api-1.1.3/ultima_scraper_api/.readthedocs.yaml
--rw-r--r--   0        0        0     2286 2023-05-13 21:02:27.542962 ultima_scraper_api-1.1.3/ultima_scraper_api/__init__.py
--rw-r--r--   0        0        0        0 2022-12-04 09:00:20.736402 ultima_scraper_api-1.1.3/ultima_scraper_api/__main__.py
--rw-r--r--   0        0        0        0 2022-12-04 15:38:35.491230 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/__init__.py
--rw-r--r--   0        0        0     6875 2023-05-10 16:14:24.886974 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/api_helper.py
--rw-r--r--   0        0        0     3348 2023-05-22 07:12:01.748229 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/api_streamliner.py
--rw-r--r--   0        0        0      696 2022-12-02 16:36:46.812390 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/background_tasks.py
--rw-r--r--   0        0        0     2895 2023-05-09 15:10:07.346536 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/__init__.py
--rw-r--r--   0        0        0      189 2023-05-13 20:33:08.152436 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/__init__.py
--rw-r--r--   0        0        0    19575 2023-05-28 15:42:17.825968 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/auth_model.py
--rw-r--r--   0        0        0     6511 2023-04-10 15:12:02.910813 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/collection_model.py
--rw-r--r--   0        0        0    11479 2023-05-28 15:33:55.688326 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/extras.py
--rw-r--r--   0        0        0      472 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/hightlight_model.py
--rw-r--r--   0        0        0     6463 2023-05-31 08:46:59.121721 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/message_model.py
--rw-r--r--   0        0        0     6918 2023-04-09 17:42:13.567826 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/post_model.py
--rw-r--r--   0        0        0     3210 2023-05-14 02:55:01.328937 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/story_model.py
--rw-r--r--   0        0        0      862 2023-05-14 01:36:53.261674 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/subscription_model.py
--rw-r--r--   0        0        0    27593 2023-05-22 08:33:43.650098 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/user_model.py
--rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/decorators/decorators.py
--rw-r--r--   0        0        0     2961 2023-05-22 10:30:47.276706 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/fansly.py
--rw-r--r--   0        0        0     2784 2023-05-10 22:02:50.317100 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/__init__.py
--rw-r--r--   0        0        0      191 2023-05-11 21:59:14.648026 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/__init__.py
--rw-r--r--   0        0        0    19223 2023-05-31 11:24:17.146008 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/auth_model.py
--rw-r--r--   0        0        0    11391 2023-05-31 18:58:22.644908 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/extras.py
--rw-r--r--   0        0        0      686 2023-03-25 19:37:35.462288 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py
--rw-r--r--   0        0        0     2970 2023-05-31 09:00:33.734398 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/message_model.py
--rw-r--r--   0        0        0     5863 2023-05-22 05:00:15.206814 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/only_drm.py
--rw-r--r--   0        0        0     3375 2023-03-27 00:23:55.042753 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/post_model.py
--rw-r--r--   0        0        0     1318 2023-04-09 10:09:44.773447 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/story_model.py
--rw-r--r--   0        0        0     1623 2023-05-13 21:04:18.608237 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py
--rw-r--r--   0        0        0    28464 2023-05-31 11:29:25.511752 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/user_model.py
--rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/decorators/decorators.py
--rw-r--r--   0        0        0     3242 2023-05-31 11:23:04.368930 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/onlyfans.py
--rw-r--r--   0        0        0     2763 2023-05-05 07:56:21.734680 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/user_streamliner.py
--rw-r--r--   0        0        0        0 2022-12-04 09:59:08.749358 ultima_scraper_api-1.1.3/ultima_scraper_api/classes/__init__.py
--rw-r--r--   0        0        0    13187 2023-03-24 22:26:49.870986 ultima_scraper_api-1.1.3/ultima_scraper_api/classes/make_settings.py
--rw-r--r--   0        0        0     3977 2023-03-12 11:46:35.721289 ultima_scraper_api-1.1.3/ultima_scraper_api/classes/prepare_directories.py
--rw-r--r--   0        0        0      340 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.3/ultima_scraper_api/classes/prepare_download.py
--rw-r--r--   0        0        0    13410 2023-05-07 21:56:21.760084 ultima_scraper_api-1.1.3/ultima_scraper_api/classes/prepare_metadata.py
--rw-r--r--   0        0        0      630 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.3/ultima_scraper_api/classes/prepare_webhooks.py
--rw-r--r--   0        0        0      638 2022-12-03 12:11:12.443198 ultima_scraper_api-1.1.3/ultima_scraper_api/docs/Makefile
--rw-r--r--   0        0        0      804 2022-12-03 12:11:12.443198 ultima_scraper_api-1.1.3/ultima_scraper_api/docs/make.bat
--rw-r--r--   0        0        0       21 2022-12-03 17:06:06.309429 ultima_scraper_api-1.1.3/ultima_scraper_api/docs/requirements.txt
--rw-r--r--   0        0        0     1318 2022-12-03 18:16:52.399681 ultima_scraper_api-1.1.3/ultima_scraper_api/docs/source/conf.py
--rw-r--r--   0        0        0      464 2022-12-03 17:00:27.610084 ultima_scraper_api-1.1.3/ultima_scraper_api/docs/source/index.rst
--rw-r--r--   0        0        0        0 2022-12-04 09:51:18.483387 ultima_scraper_api-1.1.3/ultima_scraper_api/helpers/__init__.py
--rw-r--r--   0        0        0    11343 2023-05-28 15:06:20.263463 ultima_scraper_api-1.1.3/ultima_scraper_api/helpers/main_helper.py
--rw-r--r--   0        0        0        0 2023-01-26 05:39:16.747803 ultima_scraper_api-1.1.3/ultima_scraper_api/managers/__init__.py
--rw-r--r--   0        0        0        0 2023-01-22 17:41:52.794214 ultima_scraper_api-1.1.3/ultima_scraper_api/managers/job_manager/__init__.py
--rw-r--r--   0        0        0     1911 2023-05-31 10:43:31.029509 ultima_scraper_api-1.1.3/ultima_scraper_api/managers/job_manager/job_manager.py
--rw-r--r--   0        0        0        0 2023-01-22 17:42:18.641239 ultima_scraper_api-1.1.3/ultima_scraper_api/managers/job_manager/jobs/__init__.py
--rw-r--r--   0        0        0      767 2023-05-12 15:00:15.819155 ultima_scraper_api-1.1.3/ultima_scraper_api/managers/job_manager/jobs/custom_job.py
--rw-r--r--   0        0        0     2181 2023-05-31 11:25:12.717213 ultima_scraper_api-1.1.3/ultima_scraper_api/managers/scrape_manager.py
--rw-r--r--   0        0        0    18054 2023-05-31 16:21:52.459421 ultima_scraper_api-1.1.3/ultima_scraper_api/managers/session_manager.py
--rw-r--r--   0        0        0        0 2023-05-09 14:42:23.613712 ultima_scraper_api-1.1.3/ultima_scraper_api/models/__init__.py
--rw-r--r--   0        0        0      677 2023-05-11 21:44:11.005112 ultima_scraper_api-1.1.3/ultima_scraper_api/models/subscription_model.py
--rw-r--r--   0        0        0        0 2022-12-04 16:42:28.821209 ultima_scraper_api-1.1.3/ultima_scraper_api/py.typed
--rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 ultima_scraper_api-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1214 2023-06-14 18:29:27.848708 ultima_scraper_api-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0      175 2022-12-03 17:24:36.799421 ultima_scraper_api-1.1.4/ultima_scraper_api/.readthedocs.yaml
+-rw-r--r--   0        0        0     2499 2023-06-15 03:55:06.849210 ultima_scraper_api-1.1.4/ultima_scraper_api/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-04 09:00:20.736402 ultima_scraper_api-1.1.4/ultima_scraper_api/__main__.py
+-rw-r--r--   0        0        0        0 2022-12-04 15:38:35.491230 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/__init__.py
+-rw-r--r--   0        0        0     6913 2023-06-01 15:05:27.454325 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/api_helper.py
+-rw-r--r--   0        0        0     2983 2023-06-01 21:49:26.036612 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/api_streamliner.py
+-rw-r--r--   0        0        0     1306 2023-06-15 08:27:10.520823 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/auth_streamliner.py
+-rw-r--r--   0        0        0      696 2022-12-02 16:36:46.812390 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/background_tasks.py
+-rw-r--r--   0        0        0     2891 2023-06-01 20:52:37.751350 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/__init__.py
+-rw-r--r--   0        0        0      189 2023-05-13 20:33:08.152436 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/__init__.py
+-rw-r--r--   0        0        0    12932 2023-06-15 08:56:58.240672 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/auth_model.py
+-rw-r--r--   0        0        0     6511 2023-04-10 15:12:02.910813 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/collection_model.py
+-rw-r--r--   0        0        0    15106 2023-06-15 08:12:06.529813 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/extras.py
+-rw-r--r--   0        0        0      472 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/hightlight_model.py
+-rw-r--r--   0        0        0     6433 2023-06-07 23:41:16.462833 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/message_model.py
+-rw-r--r--   0        0        0     6914 2023-06-01 20:52:37.758016 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/post_model.py
+-rw-r--r--   0        0        0     3210 2023-05-14 02:55:01.328937 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/story_model.py
+-rw-r--r--   0        0        0      862 2023-05-14 01:36:53.261674 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/subscription_model.py
+-rw-r--r--   0        0        0    27732 2023-06-15 05:16:50.559836 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/user_model.py
+-rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/decorators/decorators.py
+-rw-r--r--   0        0        0     6306 2023-06-15 08:12:42.082002 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/fansly.py
+-rw-r--r--   0        0        0     2810 2023-06-07 23:39:07.287094 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/__init__.py
+-rw-r--r--   0        0        0      191 2023-06-01 22:07:45.846163 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/__init__.py
+-rw-r--r--   0        0        0    13837 2023-06-15 08:57:37.093501 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/auth_model.py
+-rw-r--r--   0        0        0    17105 2023-06-15 08:51:10.952788 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/extras.py
+-rw-r--r--   0        0        0      686 2023-03-25 19:37:35.462288 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py
+-rw-r--r--   0        0        0     2940 2023-06-07 23:41:09.279737 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/message_model.py
+-rw-r--r--   0        0        0     5863 2023-05-22 05:00:15.206814 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/only_drm.py
+-rw-r--r--   0        0        0     3341 2023-06-15 08:39:06.344592 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/post_model.py
+-rw-r--r--   0        0        0     1318 2023-06-15 08:39:00.921432 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/story_model.py
+-rw-r--r--   0        0        0     1623 2023-05-13 21:04:18.608237 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py
+-rw-r--r--   0        0        0    28895 2023-06-15 06:10:58.787578 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/user_model.py
+-rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/decorators/decorators.py
+-rw-r--r--   0        0        0     6689 2023-06-14 15:08:49.308972 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/onlyfans.py
+-rw-r--r--   0        0        0     2759 2023-06-01 20:52:37.711351 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/user_streamliner.py
+-rw-r--r--   0        0        0        0 2022-12-04 09:59:08.749358 ultima_scraper_api-1.1.4/ultima_scraper_api/classes/__init__.py
+-rw-r--r--   0        0        0    13187 2023-03-24 22:26:49.870986 ultima_scraper_api-1.1.4/ultima_scraper_api/classes/make_settings.py
+-rw-r--r--   0        0        0     3977 2023-03-12 11:46:35.721289 ultima_scraper_api-1.1.4/ultima_scraper_api/classes/prepare_directories.py
+-rw-r--r--   0        0        0      340 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.4/ultima_scraper_api/classes/prepare_download.py
+-rw-r--r--   0        0        0    13410 2023-05-07 21:56:21.760084 ultima_scraper_api-1.1.4/ultima_scraper_api/classes/prepare_metadata.py
+-rw-r--r--   0        0        0      630 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.4/ultima_scraper_api/classes/prepare_webhooks.py
+-rw-r--r--   0        0        0     1204 2023-06-15 09:03:54.583570 ultima_scraper_api-1.1.4/ultima_scraper_api/config.py
+-rw-r--r--   0        0        0      638 2022-12-03 12:11:12.443198 ultima_scraper_api-1.1.4/ultima_scraper_api/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-12-03 12:11:12.443198 ultima_scraper_api-1.1.4/ultima_scraper_api/docs/make.bat
+-rw-r--r--   0        0        0       21 2022-12-03 17:06:06.309429 ultima_scraper_api-1.1.4/ultima_scraper_api/docs/requirements.txt
+-rw-r--r--   0        0        0     1318 2022-12-03 18:16:52.399681 ultima_scraper_api-1.1.4/ultima_scraper_api/docs/source/conf.py
+-rw-r--r--   0        0        0      464 2022-12-03 17:00:27.610084 ultima_scraper_api-1.1.4/ultima_scraper_api/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2022-12-04 09:51:18.483387 ultima_scraper_api-1.1.4/ultima_scraper_api/helpers/__init__.py
+-rw-r--r--   0        0        0    12020 2023-06-15 08:33:26.165471 ultima_scraper_api-1.1.4/ultima_scraper_api/helpers/main_helper.py
+-rw-r--r--   0        0        0        0 2023-01-26 05:39:16.747803 ultima_scraper_api-1.1.4/ultima_scraper_api/managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:41:52.794214 ultima_scraper_api-1.1.4/ultima_scraper_api/managers/job_manager/__init__.py
+-rw-r--r--   0        0        0     1911 2023-05-31 10:43:31.029509 ultima_scraper_api-1.1.4/ultima_scraper_api/managers/job_manager/job_manager.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:42:18.641239 ultima_scraper_api-1.1.4/ultima_scraper_api/managers/job_manager/jobs/__init__.py
+-rw-r--r--   0        0        0      767 2023-05-12 15:00:15.819155 ultima_scraper_api-1.1.4/ultima_scraper_api/managers/job_manager/jobs/custom_job.py
+-rw-r--r--   0        0        0     2179 2023-06-01 22:11:24.179495 ultima_scraper_api-1.1.4/ultima_scraper_api/managers/scrape_manager.py
+-rw-r--r--   0        0        0    18429 2023-06-15 03:54:30.180364 ultima_scraper_api-1.1.4/ultima_scraper_api/managers/session_manager.py
+-rw-r--r--   0        0        0        0 2023-05-09 14:42:23.613712 ultima_scraper_api-1.1.4/ultima_scraper_api/models/__init__.py
+-rw-r--r--   0        0        0      677 2023-05-11 21:44:11.005112 ultima_scraper_api-1.1.4/ultima_scraper_api/models/subscription_model.py
+-rw-r--r--   0        0        0        0 2022-12-04 16:42:28.821209 ultima_scraper_api-1.1.4/ultima_scraper_api/py.typed
+-rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 ultima_scraper_api-1.1.4/PKG-INFO
```

### Comparing `ultima_scraper_api-1.1.3/pyproject.toml` & `ultima_scraper_api-1.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ultima-scraper-api"
-version = "1.1.3"
+version = "1.1.4"
 description = ""
 authors = [
     "DIGITALCRIMINALS <89371864+digitalcriminals@users.noreply.github.com>",
 ]
 packages = [{include = "ultima_scraper_api"}]
 include = ["ultima_scraper_api/py.typed"]
 
@@ -22,14 +22,15 @@
 aiofiles = "^22.1.0"
 beautifulsoup4 = "^4.11.1"
 mypy = "^0.991"
 lxml =  "^4.9.1"
 win32-setctime = {version="^1.1.0", platform = 'win32'}
 pywidevine = "^1.6.0"
 xmltodict = "^0.13.0"
+pydantic = "^1.10.9"
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.2"
 black = {version = "^23.3.0", allow-prereleases = true}
 Sphinx = "^5.3.0"
 sphinx-autoapi = "^2.0.0"
 sphinx-rtd-theme = "^1.1.1"
```

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/__init__.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Any
 
 import ultima_scraper_api.apis.fansly.classes as fansly_classes
 import ultima_scraper_api.apis.onlyfans.classes as onlyfans_classes
+from ultima_scraper_api.apis.fansly.classes.extras import FanslyAuthenticator
 from ultima_scraper_api.apis.fansly.fansly import FanslyAPI
+from ultima_scraper_api.apis.onlyfans.classes.extras import OnlyFansAuthenticator
 from ultima_scraper_api.apis.onlyfans.onlyfans import OnlyFansAPI
 from ultima_scraper_api.classes.make_settings import Config
 
 api_types = OnlyFansAPI | FanslyAPI
-
-auth_types = (
-    onlyfans_classes.auth_model.create_auth | fansly_classes.auth_model.create_auth
-)
+authenticator_types = OnlyFansAuthenticator | FanslyAuthenticator
+auth_types = onlyfans_classes.auth_model.AuthModel | fansly_classes.auth_model.AuthModel
 user_types = (
     onlyfans_classes.user_model.create_user | fansly_classes.user_model.create_user
 )
 story_types = (
     onlyfans_classes.story_model.create_story | fansly_classes.story_model.create_story
 )
 post_types = (
```

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/api_helper.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/api_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,21 +133,21 @@
         match function_that_called:
             case function_that_called if function_that_called in [
                 "get_paid_content",
                 "get_chats",
                 "get_lists_users",
                 "get_subscriptions",
             ]:
-                if not auth.active or not refresh:
+                if not auth.get_auth_details().active or not refresh:
                     result = await handle_refresh(
                         auth, api_type, refresh, function_that_called
                     )
                     status = True
             case "get_mass_messages":
-                if not auth.active or not auth.isPerformer:
+                if not auth.get_auth_details().active or not auth.isPerformer:
                     result = await handle_refresh(
                         auth, api_type, refresh, function_that_called
                     )
                     status = True
             case _:
                 result = await handle_refresh(
                     auth, api_type, refresh, function_that_called
```

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/api_streamliner.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/api_streamliner.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING
 
 import ultima_scraper_api
 from ultima_scraper_api.apis import api_helper
 from ultima_scraper_api.classes.make_settings import Config
 
+
 if TYPE_CHECKING:
     api_types = ultima_scraper_api.api_types
     auth_types = ultima_scraper_api.auth_types
 
 
 class Packages:
     def __init__(self, site_name: str) -> None:
         match site_name.lower():
             case "onlyfans":
                 from ultima_scraper_api.apis.onlyfans.classes.extras import AuthDetails
 
                 self.AuthDetails = AuthDetails
                 from ultima_scraper_api.apis.onlyfans.classes.auth_model import (
-                    create_auth,
+                    AuthModel,
                 )
 
-                self.CreateAuth = create_auth
+                self.CreateAuth = AuthModel
             case "fansly":
                 from ultima_scraper_api.apis.fansly.classes.extras import AuthDetails
 
                 self.AuthDetails = AuthDetails
                 from ultima_scraper_api.apis.fansly.classes.auth_model import (
-                    create_auth,
+                    AuthModel,
                 )
 
-                self.CreateAuth = create_auth
+                self.CreateAuth = AuthModel
             case _:
                 raise ValueError("Site Doesn't Exist")
 
 
 class StreamlinedAPI:
     def __init__(
         self,
@@ -49,45 +50,40 @@
         self.config = config
         self.lists = None
         self.pool = api_helper.CustomPool()
 
         self.job_manager = JobManager()
         self.packages = Packages(self.api.site_name)
 
-    async def login(self, auth_json: dict[str, Any] = {}, guest: bool = False):
-        auth = self.add_auth(auth_json)
-        authed = await auth.login(guest=guest)
-        return authed
+
 
     def add_auth(
-        self, auth_json: dict[str, Any] = {}, only_active: bool = False
+        self, authenticator:ultima_scraper_api.authenticator_types, only_active: bool = False
     ) -> auth_types:
         """Creates and appends an auth object to auths property
 
         Args:
             auth_json (dict[str, str], optional): []. Defaults to {}.
             only_active (bool, optional): [description]. Defaults to False.
 
         Returns:
             create_auth: [Auth object]
         """
         packages = self.packages
-        temp_auth_details = packages.AuthDetails(**auth_json).upgrade_legacy(auth_json)
         auth = packages.CreateAuth(
-            self.api, max_threads=self.max_threads, auth_details=temp_auth_details  # type: ignore
+            authenticator   # type: ignore
         )
-        if only_active and not auth.auth_details.active:
+        if only_active and not auth.authenticator.auth_details.active:
             return auth
-        auth.auth_details = temp_auth_details  # type: ignore
         auth.extras["settings"] = self.config
         self.api.auths.append(auth)  # type: ignore
         return auth
 
     def has_active_auths(self):
-        return bool([x for x in self.api.auths if x.active])
+        return bool([x for x in self.api.auths if x.is_authed()])
 
     def get_auths_via_subscription_identifier(self, identifier: str):
         for auth in self.api.auths:
             if auth.username == identifier:
                 pass
 
     def get_site_settings(self):
```

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/background_tasks.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/background_tasks.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/__init__.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Literal
 from urllib.parse import urlparse
 
 if TYPE_CHECKING:
     from ultima_scraper_api.apis.fansly.classes.user_model import (
-        create_auth,
+        AuthModel,
         create_user,
     )
 
 SubscriptionType = Literal["all", "active", "expired"]
 
 
 class SiteContent:
-    def __init__(self, option: dict[str, Any], user: create_auth | create_user) -> None:
+    def __init__(self, option: dict[str, Any], user: AuthModel | create_user) -> None:
         self.id: int = int(option["id"])
         self.author = user
         self.media: list[dict[str, Any]] = option.get("media", [])
         self.preview_ids: list[int] = []
 
     def url_picker(self, media_item: dict[str, Any], video_quality: str = ""):
         # There are two media results at play here.
```

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/auth_model.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/auth_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,217 +1,95 @@
 from __future__ import annotations
 
 import asyncio
 from datetime import datetime
 from itertools import product
-from typing import TYPE_CHECKING, Any, Dict, Optional
+from typing import TYPE_CHECKING, Any, Dict
 
 from dateutil.relativedelta import relativedelta
-from user_agent import generate_user_agent
 
 from ultima_scraper_api.apis import api_helper
+from ultima_scraper_api.apis.auth_streamliner import StreamlinedAuth
 from ultima_scraper_api.apis.fansly import SubscriptionType
-from ultima_scraper_api.apis.fansly.classes.extras import (
-    AuthDetails,
-    ErrorDetails,
-    create_headers,
-    endpoint_links,
-)
+from ultima_scraper_api.apis.fansly.classes.extras import endpoint_links
 from ultima_scraper_api.apis.fansly.classes.message_model import create_message
 from ultima_scraper_api.apis.fansly.classes.post_model import create_post
 from ultima_scraper_api.apis.fansly.classes.subscription_model import SubscriptionModel
 from ultima_scraper_api.apis.fansly.classes.user_model import create_user
-from ultima_scraper_api.managers.session_manager import SessionManager
 
 if TYPE_CHECKING:
-    from ultima_scraper_api.apis.fansly.fansly import FanslyAPI
+    from ultima_scraper_api.apis.fansly.classes.extras import FanslyAuthenticator
     from ultima_scraper_api.apis.onlyfans.classes.only_drm import OnlyDRM
 
 
-class create_auth(create_user):
+class AuthModel(StreamlinedAuth):
     def __init__(
         self,
-        api: FanslyAPI,
-        option: dict[str, Any] = {},
-        max_threads: int = -1,
-        auth_details: AuthDetails = AuthDetails(),
+        authenticator: FanslyAuthenticator,
     ) -> None:
-        self.api = api
+        self.api = authenticator.api
         self.users: set[create_user] = set()
-        self.auth_details = auth_details
-        self.session_manager = self._SessionManager(self, max_threads=max_threads)
-        create_user.__init__(self, option, self)
-        if not self.username:
-            self.username = f"u{self.id}"
+        self.authenticator = authenticator
+        self.session_manager = authenticator.session_manager
+        assert authenticator.__raw__ is not None
+        self.user: create_user = create_user(
+            authenticator.__raw__["response"]["account"], self
+        )
+        self.id = self.user.id
+        self.username = self.user.username
         self.lists = []
-        self.links = api.ContentTypes()
+        self.links = self.api.ContentTypes()
         self.subscriptions: list[SubscriptionModel] = []
         self.followed_users: list[create_user] = []
         self.chats = None
         self.archived_stories = {}
         self.mass_messages = []
         self.paid_content: list[create_message | create_post] = []
-        self.auth_attempt = 0
-        self.max_attempts = 10
-        self.guest = False
-        self.errors: list[ErrorDetails] = []
         self.extras: dict[str, Any] = {}
         self.blacklist: list[str] = []
+        self.guest = self.authenticator.guest
         self.drm: OnlyDRM | None = None
+        self.update()
 
-    class _SessionManager(SessionManager):
-        def __init__(
-            self,
-            auth: create_auth,
-            headers: dict[str, Any] = {},
-            proxies: list[str] = [],
-            max_threads: int = -1,
-            use_cookies: bool = True,
-        ) -> None:
-            SessionManager.__init__(
-                self, auth, headers, proxies, max_threads, use_cookies
-            )
+        StreamlinedAuth.__init__(self, self.authenticator)
 
     def get_pool(self):
         return self.api.pool
 
-    async def convert_to_user(self):
-        user = await self.get_user(self.username)
-        for k, _v in user.__dict__.items():
-            setattr(user, k, getattr(self, k))
-        return user
-
-    def update(self, data: Dict[str, Any]):
-        data = data["response"][0]
-        if not data["username"]:
-            data["username"] = f"u{data['id']}"
-        for key, value in data.items():
-            found_attr = hasattr(self, key)
-            if found_attr:
-                setattr(self, key, value)
-
-    async def login(self, guest: bool = False):
-        auth_items = self.auth_details
-        if not auth_items:
-            return self
-        if guest and auth_items:
-            auth_items.user_agent = generate_user_agent()
-        link = endpoint_links().customer
-        user_agent = auth_items.user_agent
-        dynamic_rules = self.session_manager.dynamic_rules
-        a: list[Any] = [dynamic_rules, user_agent, link]
-        self.session_manager.headers = create_headers(*a)
-        if guest:
-            self.guest = True
-            return self
-
-        while self.auth_attempt < self.max_attempts:
-            await self.process_auth()
-            self.auth_attempt += 1
-
-            async def resolve_auth(auth: create_auth):
-                if self.errors:
-                    error = self.errors[-1]
-                    print(error.message)
-                    if error.code == 101:
-                        if auth_items.support_2fa:
-                            link = f"https://onlyfans.com/api2/v2/users/otp/check"
-                            count = 1
-                            max_count = 3
-                            while count < max_count + 1:
-                                print(
-                                    "2FA Attempt " + str(count) + "/" + str(max_count)
-                                )
-                                code = input("Enter 2FA Code\n")
-                                data = {"code": code, "rememberMe": True}
-                                response = await self.session_manager.json_request(
-                                    link, method="POST", payload=data
-                                )
-                                if isinstance(response, ErrorDetails):
-                                    error.message = response.message
-                                    count += 1
-                                else:
-                                    print("Success")
-                                    auth.active = False
-                                    auth.errors.remove(error)
-                                    await self.process_auth()
-                                    break
-
-            await resolve_auth(self)
-            if not self.check_authed():
-                if self.errors:
-                    error = self.errors[-1]
-                    error_message = error.message
-                    if "token" in error_message:
-                        break
-                    if "Code wrong" in error_message:
-                        break
-                    if "Please refresh" in error_message:
-                        break
-                else:
-                    print("Auth 404'ed")
-                continue
-            else:
-                break
-        if not self.check_authed():
-            user = await self.get_user(self.id)
-            if isinstance(user, create_user):
-                self.update(user.__dict__)
-        return self
-
-    async def process_auth(self):
-        if not self.maxed_out_auth_attempts():
-            link = endpoint_links().settings
-            response = await self.session_manager.json_request(link)
-            if isinstance(response, dict):
-                final_response: dict[str, Any] = response
-                link = endpoint_links(final_response["response"]["accountId"]).customer
-                final_response = await self.session_manager.json_request(link)
-                await self.resolve_auth_errors(final_response)
-                if not self.errors:
-                    self.auth_details.active = True
-                    self.update(final_response)
-                else:
-                    self.auth_details.active = False
-            else:
-                # 404'ed
-                self.auth_details.active = False
-        return self
-
-    async def resolve_auth_errors(self, response: ErrorDetails | dict[str, Any]):
-        # Adds an error object to self.auth.errors
-        if isinstance(response, ErrorDetails):
-            error = response
-        elif "error" in response:
-            error = response["error"]
-            error = ErrorDetails(error)
-        else:
-            self.errors.clear()
-            return
-        error_message = error.message
-        error_code = error.code
-        if error_code == 0:
-            pass
-        elif error_code == 101:
-            error_message = "Blocked by 2FA."
-        elif error_code == 401:
-            # Session/Refresh
-            pass
-        error.code = error_code
-        error.message = error_message
-        self.errors.append(error)
+    def update(self):
+        if self.user:
+            identifier = self.user.id
+            username = self.user.username
+            self.id = identifier
+            self.username = username
+            # # This affects scripts that use the username to select profiles
+            auth_details = self.get_auth_details()
+            auth_details.id = identifier
+            # auth_details.username = username
+
+    async def get_authed_user(self):
+        assert self.user
+        return self.user
+
+    async def get_id(self):
+        assert self.user
+        return self.user.id
+
+    async def get_username(self):
+        assert self.user
+        return self.user.get_username()
 
     async def get_lists(self, refresh: bool = True, limit: int = 100, offset: int = 0):
         result, status = await api_helper.default_data(self, refresh)
         if status:
             return result
         link = endpoint_links(global_limit=limit, global_offset=offset).lists
-        results = await self.session_manager.json_request(link)
-        self.lists = results
-        return results
+        json_resp = await self.session_manager.json_request(link)
+        self.lists = json_resp
+        return json_resp
 
     async def get_blacklist(self, blacklists: list[str]):
         bl_ids: list[str] = []
         return bl_ids
         remote_blacklists = await self.get_lists()
         if remote_blacklists:
             for remote_blacklist in remote_blacklists:
@@ -239,39 +117,45 @@
             return user
 
     async def get_user(self, identifier: int | str):
         valid_user = self.find_user_by_identifier(identifier)
         if valid_user:
             return valid_user
         else:
-            link = endpoint_links(identifier).users
-            response = await self.session_manager.json_request(link)
+            identifier = str(identifier)
+            if identifier.isdigit():
+                url = endpoint_links(identifier).users_by_id
+            else:
+                url = endpoint_links(identifier).users_by_username
+                pass
+            response = await self.session_manager.json_request(url)
             if "error" not in response:
                 response["session_manager"] = self.session_manager
                 response = create_user(response["response"][0], self)
             return response
 
     async def get_lists_users(
         self,
         identifier: int | str,
         check: bool = False,
         limit: int = 100,
         offset: int = 0,
     ):
-        if not self.active:
-            return
+        result, status = await api_helper.default_data(self, refresh=True)
+        if status:
+            return result
         link = endpoint_links(
             identifier, global_limit=limit, global_offset=offset
         ).lists_users
         results = await self.session_manager.json_request(link)
         if len(results) >= limit and not check:
             results2 = await self.get_lists_users(
                 identifier, limit=limit, offset=limit + offset
             )
-            results.extend(results2)
+            results.extend(results2)  # type: ignore
         return results
 
     async def get_followings(self, identifiers: list[int | str]) -> list[create_user]:
         offset_count = 0
         followings: list[dict[str, Any]] = []
         while True:
             followings_link = endpoint_links().list_followings(self.id, offset_count)
@@ -371,16 +255,14 @@
                 subscriptions = [
                     x for x in subscriptions if x.ends_at > datetime.utcnow()
                 ]
             case "expired":
                 subscriptions = [
                     x for x in subscriptions if x.ends_at < datetime.utcnow()
                 ]
-            case _:
-                raise ValueError(f"Invalid subscription type: {sub_type}")
         return subscriptions
 
     async def get_chats(
         self,
         links: list[str] = [],
         limit: int = 25,
         offset: int = 0,
@@ -430,74 +312,12 @@
                             last_message, result["withUser"]
                         )
             final_results = final_results["data"]
             final_results.sort(key=lambda x: x["withUser"].id, reverse=True)
         self.chats = final_results
         return final_results
 
-    async def get_mass_messages(
-        self,
-        resume: Optional[list[dict[str, Any]]] = None,
-        refresh: bool = True,
-        limit: int = 10,
-        offset: int = 0,
-    ) -> list[dict[str, Any]]:
-        result, status = await api_helper.default_data(self, refresh)
-        if status:
-            return result
-        link = endpoint_links(
-            global_limit=limit, global_offset=offset
-        ).mass_messages_api
-        results = await self.session_manager.json_request(link)
-        items = results.get("list", [])
-        if not items:
-            return items
-        if resume:
-            for item in items:
-                if any(x["id"] == item["id"] for x in resume):
-                    resume.sort(key=lambda x: x["id"], reverse=True)
-                    self.mass_messages = resume
-                    return resume
-                else:
-                    resume.append(item)
-
-        if results["hasMore"]:
-            results2 = self.get_mass_messages(
-                resume=resume, limit=limit, offset=limit + offset
-            )
-            items.extend(results2)
-        if resume:
-            items = resume
-
-        items.sort(key=lambda x: x["id"], reverse=True)
-        self.mass_messages = items
-        return items
-
-    async def get_paid_content(
-        self,
-        check: bool = False,
-        refresh: bool = True,
-        limit: int = 99,
-        offset: int = 0,
-        inside_loop: bool = False,
-    ) -> list[create_message | create_post]:
-        return []
-
-    async def resolve_user(self, post_id: int | None = None):
-        user = None
-        if post_id:
-            post = await self.get_post(post_id)
-            if not isinstance(post, ErrorDetails):
-                user = post.author
-        return user
-
     async def get_scrapable_users(self):
         followed_users = self.followed_users
         subscription_users = [x.user for x in self.subscriptions]
         unique_users = list(set(followed_users) | set(subscription_users))
         return unique_users
-
-    def maxed_out_auth_attempts(self):
-        return True if self.auth_attempt >= self.max_attempts else False
-
-    def check_authed(self):
-        return self.auth_details.active
```

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/collection_model.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/collection_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/extras.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/extras.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,86 @@
 import copy
 import math
 from itertools import chain
 from pathlib import Path
-from typing import Any, Literal, Optional, Union
+from typing import TYPE_CHECKING, Any, Literal, Optional, Union
+
+from user_agent import generate_user_agent
+
+from ultima_scraper_api.managers.session_manager import SessionManager
+
+if TYPE_CHECKING:
+    from ultima_scraper_api.apis.fansly.fansly import FanslyAPI
+
+from ultima_scraper_api.apis import api_helper
+
+
+class ErrorDetails:
+    def __init__(self, result: dict[str, Any]) -> None:
+        error = result["error"] if "error" in result else result
+        self.code = error["code"]
+        self.message = error["message"]
+
+    async def format(self, extras: dict[str, Any]):
+        match self.code:
+            case 0:
+                match self.message:
+                    case "User not found":
+                        link = Path(extras["link"])
+                        self.message = f"{link.name} not found"
+                    case _:
+                        pass
+            case _:
+                pass
+        return self
+
+
+class CookieParser:
+    def __init__(self, options: str) -> None:
+        new_dict: dict[str, Any] = {}
+        for crumble in options.strip().split(";"):
+            if crumble:
+                key, value = crumble.strip().split("=")
+                new_dict[key] = value
+        self.auth_id = new_dict.get("auth_id", "")
+        self.sess = new_dict.get("sess", "")
+        self.auth_hash = new_dict.get("auth_hash", "")
+        self.auth_uniq_ = new_dict.get("auth_uniq_", "")
+        self.auth_uid_ = new_dict.get("auth_uid_", "")
+
+    def format(self):
+        """
+        Typically used for adding cookies to requests
+        """
+        return self.__dict__
+
+    def convert(self):
+        new_dict = ""
+        for key, value in self.__dict__.items():
+            key = key.replace("auth_uniq_", f"auth_uniq_{self.auth_id}")
+            key = key.replace("auth_uid_", f"auth_uid_{self.auth_id}")
+            new_dict += f"{key}={value}; "
+        new_dict = new_dict.strip()
+        return new_dict
 
 
 class AuthDetails:
     def __init__(
         self,
+        id: int | None = None,
         username: str = "",
         authorization: str = "",
         user_agent: str = "",
         email: str = "",
         password: str = "",
         hashed: bool = False,
         support_2fa: bool = True,
         active: bool | None = None,
     ) -> None:
+        self.id = id
         self.username = username
         self.authorization = authorization
         self.user_agent = user_agent
         self.email = email
         self.password = password
         self.hashed = hashed
         self.support_2fa = support_2fa
@@ -30,14 +90,118 @@
         return self
 
     def export(self):
         new_dict = copy.copy(self.__dict__)
         return new_dict
 
 
+class FanslyAuthenticator:
+    def __init__(
+        self,
+        api: "FanslyAPI",
+        auth_details: AuthDetails = AuthDetails(),
+        max_threads: int = -1,
+    ) -> None:
+        self.api = api
+        self.auth_details = auth_details
+        self.session_manager = SessionManager(self, max_threads=max_threads)
+        self.auth_attempt = 0
+        self.max_attempts = 10
+        self.errors: list[ErrorDetails] = []
+        self.active = False
+        self.guest = False
+        self.__raw__: dict[str, Any] | None = None
+
+    async def login(self, guest: bool = False):
+        auth_items = self.auth_details
+        if not auth_items:
+            return self
+        if guest and auth_items:
+            auth_items.user_agent = generate_user_agent()
+        link = endpoint_links().customer
+        user_agent = auth_items.user_agent
+        dynamic_rules = self.session_manager.dynamic_rules
+        a: list[Any] = [dynamic_rules, user_agent, link]
+        self.session_manager.headers = create_headers(*a)
+        if guest:
+            self.guest = True
+            self.__raw__ = {}
+            return self
+
+        while self.auth_attempt < self.max_attempts:
+            await self.process_auth()
+            self.auth_attempt += 1
+
+            if not self.is_authed():
+                if self.errors:
+                    error = self.errors[-1]
+                    error_message = error.message
+                    if "token" in error_message:
+                        break
+                    if "Code wrong" in error_message:
+                        break
+                    if "Please refresh" in error_message:
+                        break
+                continue
+            else:
+                break
+        return self
+
+    async def process_auth(self):
+        if not self.maxed_out_auth_attempts():
+            link = endpoint_links().me
+            json_resp = await self.session_manager.json_request(link)
+            await self.resolve_auth_errors(json_resp)
+            if not self.errors:
+                self.auth_details.active = True
+                self.__raw__ = json_resp
+            else:
+                if self.auth_details.id:
+                    link = endpoint_links(self.auth_details.id).users_by_id
+                    json_resp = await self.session_manager.json_request(link)
+                    await self.resolve_auth_errors(json_resp)
+                    self.__raw__ = json_resp
+                self.auth_details.active = False
+        return self
+
+    def maxed_out_auth_attempts(self):
+        return True if self.auth_attempt >= self.max_attempts else False
+
+    def is_authed(self):
+        return self.auth_details.active
+
+    async def resolve_auth_errors(self, response: ErrorDetails | dict[str, Any]):
+        # Adds an error object to self.auth.errors
+        if isinstance(response, ErrorDetails):
+            error = response
+        elif "error" in response:
+            error = response["error"]
+            error = ErrorDetails(error)
+        else:
+            self.errors.clear()
+            return
+        error_message = error.message
+        error_code = error.code
+        if error_code == 0:
+            pass
+        elif error_code == 101:
+            error_message = "Blocked by 2FA."
+        elif error_code == 401:
+            # Session/Refresh
+            error_message = "Invalid Auth Info"
+        error.code = error_code
+        error.message = error_message
+        match error_code:
+            case 0:
+                pass
+            case _:
+                await api_helper.handle_error_details(error)
+        self.errors.append(error)
+
+
 class legacy_auth_details:
     def __init__(self, option: dict[str, Any] = {}):
         self.username = option.get("username", "")
         self.auth_id = option.get("auth_id", "")
         self.sess = option.get("sess", "")
         self.user_agent = option.get("user_agent", "")
         self.auth_hash = option.get("auth_hash", "")
@@ -56,62 +220,14 @@
             skippable = ["username", "user_agent"]
             if key not in skippable:
                 new_dict += f"{key}={value}; "
         new_dict = new_dict.strip()
         return new_auth_details
 
 
-class cookie_parser:
-    def __init__(self, options: str) -> None:
-        new_dict = {}
-        for crumble in options.strip().split(";"):
-            if crumble:
-                key, value = crumble.strip().split("=")
-                new_dict[key] = value
-        self.auth_id = new_dict.get("auth_id", "")
-        self.sess = new_dict.get("sess", "")
-        self.auth_hash = new_dict.get("auth_hash", "")
-        self.auth_uniq_ = new_dict.get("auth_uniq_", "")
-        self.auth_uid_ = new_dict.get("auth_uid_", "")
-
-    def format(self):
-        """
-        Typically used for adding cookies to requests
-        """
-        return self.__dict__
-
-    def convert(self):
-        new_dict = ""
-        for key, value in self.__dict__.items():
-            key = key.replace("auth_uniq_", f"auth_uniq_{self.auth_id}")
-            key = key.replace("auth_uid_", f"auth_uid_{self.auth_id}")
-            new_dict += f"{key}={value}; "
-        new_dict = new_dict.strip()
-        return new_dict
-
-
-class content_types:
-    def __init__(self, option={}) -> None:
-        class archived_types(content_types):
-            def __init__(self) -> None:
-                self.Posts = []
-
-        self.Stories = []
-        self.Posts = []
-        self.Archived = archived_types()
-        self.Chats = []
-        self.Messages = []
-        self.Highlights = []
-        self.MassMessages = []
-
-    def __iter__(self):
-        for attr, value in self.__dict__.items():
-            yield attr, value
-
-
 class endpoint_links(object):
     def __init__(
         self,
         identifier: Optional[str | int] = None,
         identifier2: Optional[str | int] = None,
         identifier3: Optional[str | int] = None,
         text: str = "",
@@ -120,17 +236,19 @@
         sort_order: Literal["asc", "desc"] = "desc",
         before_id: str = "",
     ):
         domain = "https://apiv3.fansly.com"
         api = "/api/v1"
         full_url_path = f"{domain}{api}"
         self.full_url_path = full_url_path
+        self.me = f"{full_url_path}/account/me"
         self.customer = f"{full_url_path}/account?ids={identifier}"
         self.settings = f"{full_url_path}/account/settings"
-        self.users = f"{self.full_url_path}/account?ids={identifier}"
+        self.users_by_id = f"{self.full_url_path}/account?ids={identifier}"
+        self.users_by_username = f"{self.full_url_path}/account?usernames={identifier}"
         self.followings = f"{full_url_path}/account/{identifier}/following?before={global_offset}&after=0&limit=100&offset=0"
         self.subscriptions = f"{full_url_path}/subscriptions"
         self.lists = f"https://onlyfans.com/api2/v2/lists?limit={global_limit}&offset={global_offset}"
         self.lists_users = f"https://onlyfans.com/api2/v2/lists/{identifier}/users?limit={global_limit}&offset={global_offset}&query="
         self.list_chats = f"{full_url_path}/messaging/groups?sortOrder=1&flags=0&subscriptionTierId=&search=&limit={global_limit}&offset={global_offset}"
         self.post_by_id = f"https://onlyfans.com/api2/v2/posts/{identifier}"
         self.message_by_id = f"https://onlyfans.com/api2/v2/chats/{identifier}/messages?limit=10&offset=0&firstId={identifier2}&order=desc&skip_users=all&skip_users_dups=1"
@@ -208,32 +326,14 @@
                 num = num * limit
                 link = link.replace(f"limit={limit}", f"limit={limit}")
                 new_link = link.replace(f"offset={offset}", f"offset={num}")
                 final_links.append(new_link)
         return final_links
 
 
-class ErrorDetails:
-    def __init__(self, result: dict[str, Any]) -> None:
-        error = result["error"] if "error" in result else result
-        self.code = error["code"]
-        self.message = error.get("details", "")
-        if not self.message:
-            self.message = error["message"]
-
-    async def format(self, extras: dict[str, Any]):
-        match self.code:
-            case 0:
-                match self.message:
-                    case "User not found":
-                        link = Path(extras["link"])
-                        self.message = f"{link.name} not found"
-        return self
-
-
 def create_headers(
     dynamic_rules: dict[str, Any],
     auth_id: Union[str, int],
     user_agent: str = "",
     link: str = "https://onlyfans.com/",
 ):
     headers: dict[str, Any] = {}
```

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/message_model.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/message_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
         self.changedAt: Optional[str] = option.get("changedAt")
         self.cancelSeconds: Optional[int] = option.get("cancelSeconds")
         self.isLiked: Optional[bool] = option.get("isLiked")
         self.canPurchase: Optional[bool] = option.get("canPurchase")
         self.canPurchaseReason: Optional[str] = option.get("canPurchaseReason")
         self.canReport: Optional[bool] = option.get("canReport")
         self.attachments: list[dict[str, Any]] = option.get("attachments", {})
-        self.__raw__ = option
         # Custom
         final_media_ids: list[Any] = []
         for attachment in self.attachments:
             attachment_content_id = attachment["contentId"]
             match attachment["contentType"]:
                 case 1:
                     final_media_ids.append(attachment_content_id)
```

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/post_model.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/post_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 from typing import TYPE_CHECKING, Any
 
 from ultima_scraper_api.apis.fansly import SiteContent
 from ultima_scraper_api.apis.fansly.classes.extras import endpoint_links
 
 if TYPE_CHECKING:
     from ultima_scraper_api.apis.fansly.classes.user_model import (
-        create_auth,
+        AuthModel,
         create_user,
     )
 
 
 class create_post(SiteContent):
     def __init__(
         self,
         option: dict[str, Any],
-        user: create_auth | create_user,
+        user: AuthModel | create_user,
         extra: dict[str, Any],
     ) -> None:
         SiteContent.__init__(self, option, user)
         self.responseType: str = option.get("responseType")
         self.createdAt: str = option.get("createdAt")
         self.postedAtPrecise: str = option.get("postedAtPrecise")
         self.expiredAt: Any = option.get("expiredAt")
```

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/story_model.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/story_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/subscription_model.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/subscription_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/user_model.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/user_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 )
 from ultima_scraper_api.apis.fansly.classes.hightlight_model import create_highlight
 from ultima_scraper_api.apis.fansly.classes.story_model import create_story
 from ultima_scraper_api.apis.user_streamliner import StreamlinedUser
 from ultima_scraper_api.managers.scrape_manager import ScrapeManager
 
 if TYPE_CHECKING:
-    from ultima_scraper_api.apis.fansly.classes.auth_model import create_auth
+    from ultima_scraper_api.apis.fansly.classes.auth_model import AuthModel
     from ultima_scraper_api.apis.fansly.classes.post_model import create_post
 
 
 class create_user(StreamlinedUser):
     def __init__(
         self,
         option: dict[str, Any],
-        authed: create_auth,
+        authed: AuthModel,
     ) -> None:
         self.avatar: Any = option.get("avatar")
         self.avatarThumbs: Any = option.get("avatarThumbs")
         self.header: Any = option.get("banner")
         self.headerSize: Any = option.get("headerSize")
         self.headerThumbs: Any = option.get("headerThumbs")
         self.id: int = option.get("id")
@@ -225,24 +225,33 @@
         authed.users.add(self)
         self.download_info: dict[str, Any] = {}
         self.duplicate_media = []
         self.scrape_manager = ScrapeManager(authed.session_manager)
         self.__raw__ = option
         StreamlinedUser.__init__(self, authed)
 
+    def get_username(self):
+        return self.username
+
     def get_link(self):
         link = f"https://fansly.com/{self.username}"
         return link
 
     def is_me(self) -> bool:
         status = False
         if self.email:
             status = True
         return status
 
+    def is_authed_user(self):
+        if self.id == self.get_authed().id:
+            return True
+        else:
+            return False
+
     async def get_stories(
         self, refresh: bool = True, limit: int = 100, offset: int = 0
     ) -> list[create_story]:
         result, status = await api_helper.default_data(self, refresh)
         if status:
             return result
         link = [
@@ -340,29 +349,27 @@
     async def get_messages(
         self,
         links: Optional[list[str]] = None,
         limit: int = 100000,
         before: str = "",
         refresh: bool = True,
         inside_loop: bool = False,
-    ) -> list[Any]:
+    ):
         result, status = await api_helper.default_data(self, refresh)
         if status:
             return result
         groups = await self.get_groups()
         if isinstance(groups, ErrorDetails):
             return []
         found_id: Optional[int] = None
         for group in groups["groups"]:
             for user in group["users"]:
                 if self.id == user["userId"]:
                     found_id = user["groupId"]
                     break
-                print
-            print
         final_results: list[message_model.create_message] = []
         if found_id:
             if links is None:
                 links = []
 
             link = endpoint_links(
                 identifier=found_id, global_limit=limit, before_id=before
```

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/fansly.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/user_streamliner.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,98 @@
-from typing import Any, Literal, Optional, Union
+from __future__ import annotations
 
-from ultima_scraper_api.apis.api_streamliner import StreamlinedAPI
-from ultima_scraper_api.apis.fansly.classes.auth_model import create_auth
-from ultima_scraper_api.apis.fansly.classes.extras import AuthDetails, endpoint_links
-from ultima_scraper_api.apis.fansly.classes.user_model import create_user
-from ultima_scraper_api.classes.make_settings import Config
-
-
-class FanslyAPI(StreamlinedAPI):
-    def __init__(self, config: Config) -> None:
-        self.site_name: Literal["Fansly"] = "Fansly"
-        StreamlinedAPI.__init__(self, self, config)
-        self.auths: list[create_auth] = []
-        self.users: dict[int, create_user] = {}
-        self.endpoint_links = endpoint_links
-
-    def get_auth(self, identifier: Union[str, int]) -> Optional[create_auth]:
-        final_auth = None
-        for auth in self.auths:
-            if auth.id == identifier:
-                final_auth = auth
-            elif auth.username == identifier:
-                final_auth = auth
-            if final_auth:
-                break
-        return final_auth
-
-    async def remove_invalid_auths(self):
-        for auth in self.auths.copy():
-            if not auth.check_authed():
-                await self.remove_auth(auth)
-
-    async def remove_auth(self, auth: create_auth):
-        await auth.session_manager.active_session.close()
-        self.auths.remove(auth)
-
-    def create_auth_details(self, auth_json: dict[str, Any] = {}) -> AuthDetails:
-        """If you've got a auth.json file, you can load it into python and pass it through here.
-
-        Args:
-            auth_json (dict[str, Any], optional): [description]. Defaults to {}.
-
-        Returns:
-            auth_details: [auth_details object]
-        """
-        return AuthDetails(**auth_json).upgrade_legacy(auth_json)
-
-    class ContentTypes:
-        def __init__(self) -> None:
-            self.Stories = []
-            self.Posts = []
-            self.Chats = []
-            self.Messages = []
-            self.Highlights = []
-            self.MassMessages = []
-
-        def __iter__(self):
-            for attr, value in self.__dict__.items():
-                yield attr, value
-
-        def get_keys(self):
-            return [item[0] for item in self]
-
-    class MediaTypes:
-        def __init__(self) -> None:
-            self.Images = ["photo", "image"]
-            self.Videos = ["video", "stream", "gif"]
-            self.Audios = ["audio"]
-            self.Texts = ["text"]
-
-        def get_keys(self):
-            return [item[0] for item in self.__dict__.items()]
-
-        def find_by_value(self, value: str):
-            final_media_type = None
-            for media_type, alt_media_types in self.__dict__.items():
-                if value in alt_media_types:
-                    final_media_type = media_type
-            if not final_media_type:
-                raise Exception("No media type found")
-            return final_media_type
+import copy
+from typing import TYPE_CHECKING
+
+import dill
+from ultima_scraper_api.managers.job_manager.jobs.custom_job import CustomJob
+
+if TYPE_CHECKING:
+    import ultima_scraper_api.apis.fansly.classes as fansly_classes
+    import ultima_scraper_api.apis.onlyfans.classes as onlyfans_classes
+
+    auth_types = (
+        onlyfans_classes.auth_model.AuthModel | fansly_classes.auth_model.AuthModel
+    )
+
+
+class JobTask:
+    def __init__(self, title: str) -> None:
+        self.title = title
+        self.child_tasks: list[JobTask] = []
+        self.min = 0
+        self.max = 0
+        self.done = False
+
+    def advance(self, length: int):
+        self.min += length
+
+
+class Job:
+    def __init__(self, title: str) -> None:
+        self.title = title
+        self.done = False
+        self.added = False
+        self.tasks: list[JobTask] = []
+
+    def create_task(self, title: str):
+        task = JobTask(title)
+        self.tasks.append(task)
+        return task
+
+    def create_tasks(self, data: list[str]):
+        for key in data:
+            self.create_task(key)
+
+    def get_current_task(self):
+        tasks = [x for x in self.tasks if not x.done]
+        return None if not tasks else tasks[0]
+
+
+class StreamlinedUser:
+    def __init__(self, authed: auth_types) -> None:
+        self.__authed = authed
+        self.jobs: list[CustomJob] = []
+        self.job_whitelist: list[int | str] = []
+        self.scrape_whitelist: list[int | str] = []
+        self.active: bool = True
+
+    def get_authed(self):
+        return self.__authed
+
+    def get_job(self, value: str):
+        found_jobs = [x for x in self.jobs if x.title == value]
+        found_job = None
+        if found_jobs:
+            found_job = found_jobs[0]
+        return found_job
+
+    def get_complete_jobs(self):
+        return [x for x in self.jobs if x.done == True]
+
+    def get_incomplete_jobs(self):
+        return [x for x in self.jobs if x.done == False]
+
+    def get_current_job(self):
+        incomplete_jobs = self.get_incomplete_jobs()
+        return None if not incomplete_jobs else incomplete_jobs[0]
+
+    def convert_to_dill(self):
+        old = copy.copy(self)
+        delattr(old, "_StreamlinedUser__authed")
+        delattr(old, "__raw__")
+        delattr(old, "directory_manager")
+        delattr(old, "file_manager")
+        delattr(old, "temp_scraped")
+        delattr(old, "scraped")
+        old.jobs = [x.convert_to_dill()[1] for x in old.jobs]
+        data_string: bytes = dill.dumps(old)  # type: ignore
+        return data_string
+
+    def get_session_manager(self):
+        return self.__authed.session_manager
+
+    def get_api(self):
+        return self.__authed.api
+
+    def is_active(self):
+        return self.active
```

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/__init__.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 from typing import TYPE_CHECKING, Any, Literal
 from urllib.parse import urlparse
 
 SubscriptionType = Literal["all", "active", "expired", "attention"]
 
 if TYPE_CHECKING:
     from ultima_scraper_api.apis.onlyfans.classes.user_model import (
-        create_auth,
+        AuthModel,
         create_user,
     )
 
 
 class SiteContent:
-    def __init__(self, option: dict[str, Any], user: create_auth | create_user) -> None:
+    def __init__(self, option: dict[str, Any], user: AuthModel | create_user) -> None:
         self.id: int = option["id"]
         self.author = user
         self.media: list[dict[str, Any]] = option.get("media", [])
         self.preview_ids: list[int] = []
+        self.__raw__ = option
 
     def url_picker(self, media_item: dict[str, Any], video_quality: str = ""):
         authed = self.get_author().get_authed()
         video_quality = (
             video_quality or self.author.get_api().get_site_settings().video_quality
         )
         if not media_item["canView"]:
```

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/auth_model.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/auth_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,210 +2,82 @@
 
 import asyncio
 import math
 from itertools import chain, product
 from typing import TYPE_CHECKING, Any, Dict, Optional
 
 from ultima_scraper_api.apis import api_helper
+from ultima_scraper_api.apis.auth_streamliner import StreamlinedAuth
 from ultima_scraper_api.apis.onlyfans import SubscriptionType
-from ultima_scraper_api.apis.onlyfans.classes.extras import (
-    AuthDetails,
-    ErrorDetails,
-    create_headers,
-    endpoint_links,
-)
+from ultima_scraper_api.apis.onlyfans.classes.extras import endpoint_links
 from ultima_scraper_api.apis.onlyfans.classes.message_model import create_message
 from ultima_scraper_api.apis.onlyfans.classes.post_model import create_post
 from ultima_scraper_api.apis.onlyfans.classes.subscription_model import (
     SubscriptionModel,
 )
 from ultima_scraper_api.apis.onlyfans.classes.user_model import create_user
-from ultima_scraper_api.managers.session_manager import SessionManager
-from user_agent import generate_user_agent
 
 if TYPE_CHECKING:
+    from ultima_scraper_api.apis.onlyfans.classes.extras import OnlyFansAuthenticator
     from ultima_scraper_api.apis.onlyfans.classes.only_drm import OnlyDRM
-    from ultima_scraper_api.apis.onlyfans.onlyfans import OnlyFansAPI
-
-# auth_model.py handles functions that only relate to the authenticated user
-# We can create a auth_streamliner that has a parent class of create_user instead
 
 
-class create_auth(create_user):
+class AuthModel(StreamlinedAuth):
     def __init__(
         self,
-        api: OnlyFansAPI,
-        option: dict[str, Any] = {},
-        max_threads: int = -1,
-        auth_details: AuthDetails = AuthDetails(),
+        authenticator: OnlyFansAuthenticator,
     ) -> None:
-        self.api = api
+        self.api = authenticator.api
         self.users: set[create_user] = set()
-        self.auth_details = auth_details
-        self.session_manager = self._SessionManager(self, max_threads=max_threads)
-        create_user.__init__(self, option, self)
-        if not self.username:
-            self.username = f"u{self.id}"
+        self.authenticator = authenticator
+        self.session_manager = authenticator.session_manager
+        assert authenticator.__raw__ is not None
+        self.user: create_user = create_user(authenticator.__raw__, self)
+        self.id = self.user.id
+        self.username = self.user.username
         self.lists = []
-        self.links = api.ContentTypes()
+        self.links = self.api.ContentTypes()
         self.subscriptions: list[SubscriptionModel] = []
         self.chats = None
         self.archived_stories = {}
         self.mass_messages = []
         self.paid_content: list[create_message | create_post] = []
-        self.auth_attempt = 0
-        self.max_attempts = 10
-        self.guest = False
-        self.errors: list[ErrorDetails] = []
         self.extras: dict[str, Any] = {}
         self.blacklist: list[str] = []
+        self.guest = self.authenticator.guest
         self.drm: OnlyDRM | None = None
+        self.update()
 
-    class _SessionManager(SessionManager):
-        def __init__(
-            self,
-            auth: create_auth,
-            headers: dict[str, Any] = {},
-            proxies: list[str] = [],
-            max_threads: int = -1,
-            use_cookies: bool = True,
-        ) -> None:
-            SessionManager.__init__(
-                self, auth, headers, proxies, max_threads, use_cookies
-            )
+        StreamlinedAuth.__init__(self, self.authenticator)
 
     def get_pool(self):
         return self.api.pool
 
-    async def convert_to_user(self):
-        user = await self.get_user(self.username)
-        for k, _v in user.__dict__.items():
-            setattr(user, k, getattr(self, k))
-        return user
-
-    def update(self, data: Dict[str, Any]):
-        if not data["username"]:
-            data["username"] = f"u{data['id']}"
-        for key, value in data.items():
-            found_attr = hasattr(self, key)
-            if found_attr:
-                setattr(self, key, value)
-
-    async def login(self, guest: bool = False):
-        auth_items = self.auth_details
-        if not auth_items:
-            return self
-        if guest and auth_items:
-            auth_items.cookie.auth_id = "0"
-            auth_items.user_agent = generate_user_agent()
-        link = endpoint_links().customer
-        user_agent = auth_items.user_agent
-        auth_id = str(auth_items.cookie.auth_id)
-        # expected string error is fixed by auth_id
-        dynamic_rules = self.session_manager.dynamic_rules
-        a: list[Any] = [dynamic_rules, auth_id, auth_items.x_bc, user_agent, link]
-        self.session_manager.headers = create_headers(*a)
-        if guest:
-            self.guest = True
-            return self
-
-        while self.auth_attempt < self.max_attempts:
-            await self.process_auth()
-            self.auth_attempt += 1
-
-            async def resolve_auth(auth: create_auth):
-                if self.errors:
-                    error = self.errors[-1]
-                    if error.code == 101:
-                        if auth_items.support_2fa:
-                            link = f"https://onlyfans.com/api2/v2/users/otp/check"
-                            count = 1
-                            max_count = 3
-                            while count < max_count + 1:
-                                print(
-                                    "2FA Attempt " + str(count) + "/" + str(max_count)
-                                )
-                                code = input("Enter 2FA Code\n")
-                                data = {"code": code, "rememberMe": True}
-                                response = await self.session_manager.json_request(
-                                    link, method="POST", payload=data
-                                )
-                                if isinstance(response, ErrorDetails):
-                                    error.message = response.message
-                                    count += 1
-                                else:
-                                    print("Success")
-                                    auth.active = False
-                                    auth.errors.remove(error)
-                                    await self.process_auth()
-                                    break
-
-            await resolve_auth(self)
-            if not self.check_authed():
-                if self.errors:
-                    error = self.errors[-1]
-                    error_message = error.message
-                    if "token" in error_message:
-                        break
-                    if "Code wrong" in error_message:
-                        break
-                    if "Please refresh" in error_message:
-                        break
-                continue
-            else:
-                break
-        if not self.check_authed():
-            user = await self.get_user(auth_id)
-            if isinstance(user, create_user):
-                self.update(user.__dict__)
-        return self
-
-    async def process_auth(self):
-        if not self.maxed_out_auth_attempts():
-            link = endpoint_links().customer
-            json_resp = await self.session_manager.json_request(link)
-            if json_resp:
-                await self.resolve_auth_errors(json_resp)
-                if not self.errors:
-                    self.auth_details.active = True
-                    self.update(json_resp)
-                else:
-                    self.auth_details.active = False
-            else:
-                # 404'ed
-                self.auth_details.active = False
-        return self
-
-    async def resolve_auth_errors(self, response: ErrorDetails | dict[str, Any]):
-        # Adds an error object to self.auth.errors
-        if isinstance(response, ErrorDetails):
-            error = response
-        elif "error" in response:
-            error = response["error"]
-            error = ErrorDetails(error)
-        else:
-            self.errors.clear()
-            return
-        error_message = error.message
-        error_code = error.code
-        if error_code == 0:
-            pass
-        elif error_code == 101:
-            error_message = "Blocked by 2FA."
-        elif error_code == 401:
-            # Session/Refresh
-            error_message = "Invalid Auth Info"
-        error.code = error_code
-        error.message = error_message
-        match error_code:
-            case 0:
-                pass
-            case _:
-                await api_helper.handle_error_details(error)
-        self.errors.append(error)
+    def update(self):
+        if self.user:
+            identifier = self.user.id
+            username = self.user.username
+            self.id = identifier
+            self.username = username
+            # # This affects scripts that use the username to select profiles
+            auth_details = self.get_auth_details()
+            auth_details.id = identifier
+            # auth_details.username = username
+
+    async def get_authed_user(self):
+        assert self.user
+        return self.user
+
+    async def get_id(self):
+        assert self.user
+        return self.user.id
+
+    async def get_username(self):
+        assert self.user
+        return self.user.get_username()
 
     async def get_lists(self, refresh: bool = True, limit: int = 100, offset: int = 0):
         result, status = await api_helper.default_data(self, refresh)
         if status:
             return result
         link = endpoint_links(global_limit=limit, global_offset=offset).lists
         json_resp = await self.session_manager.json_request(link)
@@ -250,15 +122,15 @@
             if "error" not in response:
                 response["session_manager"] = self.session_manager
                 response = create_user(response, self)
             return response
 
     async def get_lists_users(
         self,
-        identifier: int | str,
+        identifier: int,
         check: bool = False,
         limit: int = 100,
         offset: int = 0,
     ):
         result, status = await api_helper.default_data(self, refresh=True)
         if status:
             return result
@@ -266,15 +138,15 @@
             identifier, global_limit=limit, global_offset=offset
         ).lists_users
         results = await self.session_manager.json_request(link)
         if len(results) >= limit and not check:
             results2 = await self.get_lists_users(
                 identifier, limit=limit, offset=limit + offset
             )
-            results.extend(results2)
+            results.extend(results2)  # type: ignore
         return results
 
     async def get_subscription(
         self, identifier: int | str = "", custom_list: list[SubscriptionModel] = []
     ) -> SubscriptionModel | None:
         subscriptions = (
             await self.get_subscriptions(refresh=False)
@@ -445,54 +317,45 @@
     async def get_paid_content(
         self,
         check: bool = False,
         refresh: bool = True,
         limit: int = 10,
         offset: int = 0,
         inside_loop: bool = False,
-    ) -> list[create_message | create_post] | ErrorDetails:
+    ):
+        if not self.cache.paid_content.is_released():
+            return self.paid_content
         result, status = await api_helper.default_data(self, refresh)
         if status:
             return result
         link = endpoint_links(global_limit=limit, global_offset=offset).paid_api
         final_results = await self.session_manager.json_request(link)
-        if not isinstance(final_results, ErrorDetails):
-            if len(final_results) > 0 and not check:
-                results2 = await self.get_paid_content(
-                    limit=limit, offset=limit + offset, inside_loop=True
-                )
-                final_results.extend(results2)
-            if not inside_loop:
-                temp: list[create_message | create_post] = []
-                for final_result in final_results:
-                    content = None
-                    if final_result["responseType"] == "message":
-                        user = await self.get_user(final_result["fromUser"]["id"])
-                        if isinstance(user, dict):
-                            user = create_user(final_result["fromUser"], self)
-                        content = create_message(final_result, user)
-                    elif final_result["responseType"] == "post":
-                        user = create_user(final_result["author"], self)
-                        content = create_post(final_result, user)
-                    if content:
-                        temp.append(content)
-                final_results = temp
-            self.paid_content = final_results
+        if len(final_results) > 0 and not check:
+            results2 = await self.get_paid_content(
+                limit=limit, offset=limit + offset, inside_loop=True
+            )
+            final_results.extend(results2)  # type:ignore
+        if not inside_loop:
+            for final_result in final_results:
+                content = None
+                if final_result["responseType"] == "message":
+                    user = await self.get_user(final_result["fromUser"]["id"])
+                    if isinstance(user, dict):
+                        user = create_user(final_result["fromUser"], self)
+                    content = create_message(final_result, user)
+                elif final_result["responseType"] == "post":
+                    user = create_user(final_result["author"], self)
+                    content = create_post(final_result, user)
+                if content:
+                    self.paid_content.append(content)
+                    self.cache.paid_content.activate()
+            return self.paid_content
         return final_results
 
-    async def resolve_user(self, post_id: int | None = None):
-        user = None
-        if post_id:
-            post = await self.get_post(post_id)
-            if not isinstance(post, ErrorDetails):
-                user = post.author
-        return user
-
     async def get_scrapable_users(self):
         subscription_users = [x.user for x in self.subscriptions]
         return subscription_users
 
-    def maxed_out_auth_attempts(self):
-        return True if self.auth_attempt >= self.max_attempts else False
-
-    def check_authed(self):
-        return self.auth_details.active
+    async def get_login_issues(self):
+        url = endpoint_links().login_issues
+        response = await self.session_manager.json_request(url, method="POST")
+        return response
```

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/extras.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/extras.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,97 @@
 import copy
 import math
 from itertools import chain
 from pathlib import Path
-from typing import Any, Literal, Optional, Union
+from typing import TYPE_CHECKING, Any, Literal, Optional, Union
 from urllib.parse import parse_qs, urlparse
 
+from user_agent import generate_user_agent
+
+from ultima_scraper_api.managers.session_manager import SessionManager
+
+if TYPE_CHECKING:
+    from ultima_scraper_api.apis.onlyfans.onlyfans import OnlyFansAPI
+
+from ultima_scraper_api.apis import api_helper
+
+
+class ErrorDetails:
+    def __init__(self, result: dict[str, Any]) -> None:
+        error = result["error"] if "error" in result else result
+        self.code = error["code"]
+        self.message = error["message"]
+
+    async def format(self, extras: dict[str, Any]):
+        match self.code:
+            case 0:
+                match self.message:
+                    case "User not found":
+                        link = Path(extras["link"])
+                        self.message = f"{link.name} not found"
+                    case _:
+                        pass
+            case _:
+                pass
+        return self
+
+
+class CookieParser:
+    def __init__(self, options: str) -> None:
+        new_dict: dict[str, Any] = {}
+        for crumble in options.strip().split(";"):
+            if crumble:
+                split_value = crumble.strip().split("=", 1)
+                if len(split_value) >= 2:
+                    key, value = split_value
+                    new_dict[key] = value
+        self.auth_id = new_dict.get("auth_id", "")
+        self.sess = new_dict.get("sess", "")
+        self.auth_hash = new_dict.get("auth_hash", "")
+        self.auth_uniq_ = new_dict.get("auth_uniq_", "")
+        self.auth_uid_ = new_dict.get("auth_uid_", "")
+        self.aws_waf_token = new_dict.get("aws-waf-token", "")
+
+    def format(self):
+        """
+        Typically used for adding cookies to requests
+        """
+        final_dict = self.__dict__.copy()
+        final_dict["aws-waf-token"] = final_dict["aws_waf_token"]
+        final_dict.pop("aws_waf_token")
+        return final_dict
+
+    def convert(self):
+        new_dict = ""
+        for key, value in self.__dict__.items():
+            key = key.replace("auth_uniq_", f"auth_uniq_{self.auth_id}")
+            key = key.replace("auth_uid_", f"auth_uid_{self.auth_id}")
+            key = key.replace("aws_waf_token", f"aws-waf-token")
+            new_dict += f"{key}={value}; "
+        new_dict = new_dict.strip()
+        return new_dict
+
 
 class AuthDetails:
     def __init__(
         self,
+        id: int | None = None,
         username: str = "",
         cookie: str = "",
         x_bc: str = "",
         user_agent: str = "",
         email: str = "",
         password: str = "",
         hashed: bool = False,
         support_2fa: bool = True,
         active: bool | None = None,
     ) -> None:
+        self.id = id
         self.username = username
-        self.cookie = cookie_parser(cookie)
+        self.cookie = CookieParser(cookie)
         self.x_bc = x_bc
         self.user_agent = user_agent
         self.email = email
         self.password = password
         self.hashed = hashed
         self.support_2fa = support_2fa
         self.active = active
@@ -44,14 +111,148 @@
         if model:
             for att in new_dict.copy():
                 if att not in model.__annotations__:
                     del new_dict[att]
         return new_dict
 
 
+class OnlyFansAuthenticator:
+    def __init__(
+        self,
+        api: "OnlyFansAPI",
+        auth_details: AuthDetails = AuthDetails(),
+        max_threads: int = -1,
+    ) -> None:
+        self.api = api
+        self.auth_details = auth_details
+        self.session_manager = SessionManager(self, max_threads=max_threads)
+        self.auth_attempt = 0
+        self.max_attempts = 10
+        self.errors: list[ErrorDetails] = []
+        self.active = False
+        self.guest = False
+        self.__raw__: dict[str, Any] | None = None
+
+    async def login(self, guest: bool = False):
+        auth_items = self.auth_details
+        if not auth_items:
+            return self
+        if guest and auth_items:
+            auth_items.cookie.auth_id = "0"
+            auth_items.user_agent = generate_user_agent()
+        link = endpoint_links().customer
+        user_agent = auth_items.user_agent
+        auth_id = str(auth_items.cookie.auth_id)
+        # expected string error is fixed by auth_id
+        dynamic_rules = self.session_manager.dynamic_rules
+        a: list[Any] = [dynamic_rules, auth_id, auth_items.x_bc, user_agent, link]
+        self.session_manager.headers = create_headers(*a)
+        if guest:
+            self.guest = True
+            self.__raw__ = {}
+            return self
+
+        while self.auth_attempt < self.max_attempts:
+            await self.process_auth()
+            self.auth_attempt += 1
+
+            async def resolve_auth(auth: OnlyFansAuthenticator):
+                if self.errors:
+                    error = self.errors[-1]
+                    if error.code == 101:
+                        if auth_items.support_2fa:
+                            link = f"https://onlyfans.com/api2/v2/users/otp/check"
+                            count = 1
+                            max_count = 3
+                            while count < max_count + 1:
+                                print(
+                                    "2FA Attempt " + str(count) + "/" + str(max_count)
+                                )
+                                code = input("Enter 2FA Code\n")
+                                data = {"code": code, "rememberMe": True}
+                                response = await self.session_manager.json_request(
+                                    link, method="POST", payload=data
+                                )
+                                if isinstance(response, ErrorDetails):
+                                    error.message = response.message
+                                    count += 1
+                                else:
+                                    print("Success")
+                                    auth.active = False
+                                    auth.errors.remove(error)
+                                    await self.process_auth()
+                                    break
+
+            await resolve_auth(self)
+            if not self.is_authed():
+                if self.errors:
+                    error = self.errors[-1]
+                    error_message = error.message
+                    if "token" in error_message:
+                        break
+                    if "Code wrong" in error_message:
+                        break
+                    if "Please refresh" in error_message:
+                        break
+                continue
+            else:
+                break
+        return self
+
+    async def process_auth(self):
+        if not self.maxed_out_auth_attempts():
+            link = endpoint_links().customer
+            json_resp = await self.session_manager.json_request(link)
+            await self.resolve_auth_errors(json_resp)
+            if not self.errors:
+                self.auth_details.active = True
+                self.__raw__ = json_resp
+            else:
+                link = endpoint_links(self.auth_details.cookie.auth_id).users
+                json_resp = await self.session_manager.json_request(link)
+                await self.resolve_auth_errors(json_resp)
+                self.auth_details.active = False
+                self.__raw__ = json_resp
+        return self
+
+    def maxed_out_auth_attempts(self):
+        return True if self.auth_attempt >= self.max_attempts else False
+
+    def is_authed(self):
+        return self.auth_details.active
+
+    async def resolve_auth_errors(self, response: ErrorDetails | dict[str, Any]):
+        # Adds an error object to self.auth.errors
+        if isinstance(response, ErrorDetails):
+            error = response
+        elif "error" in response:
+            error = response["error"]
+            error = ErrorDetails(error)
+        else:
+            self.errors.clear()
+            return
+        error_message = error.message
+        error_code = error.code
+        if error_code == 0:
+            pass
+        elif error_code == 101:
+            error_message = "Blocked by 2FA."
+        elif error_code == 401:
+            # Session/Refresh
+            error_message = "Invalid Auth Info"
+        error.code = error_code
+        error.message = error_message
+        match error_code:
+            case 0:
+                pass
+            case _:
+                await api_helper.handle_error_details(error)
+        self.errors.append(error)
+
+
 class legacy_auth_details:
     def __init__(self, option: dict[str, Any] = {}):
         self.username = option.get("username", "")
         self.auth_id = option.get("auth_id", "")
         self.sess = option.get("sess", "")
         self.user_agent = option.get("user_agent", "")
         self.auth_hash = option.get("auth_hash", "")
@@ -67,54 +268,18 @@
         new_dict = ""
         for key, value in self.__dict__.items():
             value = value if value != None else ""
             skippable = ["username", "user_agent"]
             if key not in skippable:
                 new_dict += f"{key}={value}; "
         new_dict = new_dict.strip()
-        new_auth_details.cookie = cookie_parser(new_dict)
+        new_auth_details.cookie = CookieParser(new_dict)
         return new_auth_details
 
 
-class cookie_parser:
-    def __init__(self, options: str) -> None:
-        new_dict: dict[str, Any] = {}
-        for crumble in options.strip().split(";"):
-            if crumble:
-                split_value = crumble.strip().split("=", 1)
-                if len(split_value) >= 2:
-                    key, value = split_value
-                    new_dict[key] = value
-        self.auth_id = new_dict.get("auth_id", "")
-        self.sess = new_dict.get("sess", "")
-        self.auth_hash = new_dict.get("auth_hash", "")
-        self.auth_uniq_ = new_dict.get("auth_uniq_", "")
-        self.auth_uid_ = new_dict.get("auth_uid_", "")
-        self.aws_waf_token = new_dict.get("aws-waf-token", "")
-
-    def format(self):
-        """
-        Typically used for adding cookies to requests
-        """
-        final_dict = self.__dict__.copy()
-        final_dict["aws-waf-token"] = final_dict["aws_waf_token"]
-        final_dict.pop("aws_waf_token")
-        return final_dict
-
-    def convert(self):
-        new_dict = ""
-        for key, value in self.__dict__.items():
-            key = key.replace("auth_uniq_", f"auth_uniq_{self.auth_id}")
-            key = key.replace("auth_uid_", f"auth_uid_{self.auth_id}")
-            key = key.replace("aws_waf_token", f"aws-waf-token")
-            new_dict += f"{key}={value}; "
-        new_dict = new_dict.strip()
-        return new_dict
-
-
 class endpoint_links(object):
     def __init__(
         self,
         identifier: Optional[int | str] = None,
         identifier2: Optional[int | str] = None,
         identifier3: Optional[int | str] = None,
         text: str = "",
@@ -122,14 +287,15 @@
         global_offset: int = 0,
         sort_order: Literal["asc", "desc"] = "desc",
     ):
         domain = "https://onlyfans.com"
         api = "/api2/v2"
         full_url_path = f"{domain}{api}"
         self.full_url_path = full_url_path
+        self.login_issues = f"{full_url_path}/issues/login"
         self.customer = f"https://onlyfans.com/api2/v2/users/me"
         self.users = f"https://onlyfans.com/api2/v2/users/{identifier}"
         self.subscriptions = f"{full_url_path}/subscriptions/subscribes?limit={global_limit}&offset={global_offset}&type={identifier}"
         self.lists = f"https://onlyfans.com/api2/v2/lists?limit=100&offset=0"
         self.lists_users = f"https://onlyfans.com/api2/v2/lists/{identifier}/users?limit={global_limit}&offset={global_offset}&query="
         self.list_chats = f"https://onlyfans.com/api2/v2/chats?limit={global_limit}&offset={global_offset}&order=desc"
         self.post_by_id = f"https://onlyfans.com/api2/v2/posts/{identifier}"
@@ -196,30 +362,14 @@
                 limit_value = query_params["limit"][0]
                 url = url.replace(f"limit={limit_value}", f"limit={limit}")
                 new_link = url.replace(f"offset={offset}", f"offset={num}")
                 final_links.append(new_link)
         return final_links
 
 
-class ErrorDetails:
-    def __init__(self, result: dict[str, Any]) -> None:
-        error = result["error"] if "error" in result else result
-        self.code = error["code"]
-        self.message = error["message"]
-
-    async def format(self, extras: dict[str, Any]):
-        match self.code:
-            case 0:
-                match self.message:
-                    case "User not found":
-                        link = Path(extras["link"])
-                        self.message = f"{link.name} not found"
-        return self
-
-
 def create_headers(
     dynamic_rules: dict[str, Any],
     auth_id: Union[str, int],
     x_bc: str,
     user_agent: str = "",
     link: str = "https://onlyfans.com/",
 ):
```

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/message_model.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/message_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
         self.createdAt: Optional[str] = option.get("createdAt")
         self.changedAt: Optional[str] = option.get("changedAt")
         self.cancelSeconds: Optional[int] = option.get("cancelSeconds")
         self.isLiked: Optional[bool] = option.get("isLiked")
         self.canPurchase: Optional[bool] = option.get("canPurchase")
         self.canPurchaseReason: Optional[str] = option.get("canPurchaseReason")
         self.canReport: Optional[bool] = option.get("canReport")
-        self.__raw__ = option
 
     def get_author(self):
         return self.author
 
     def get_receiver(self):
         receiver = (
             self.author.get_authed() if self.author.id == self.user.id else self.user
```

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/only_drm.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/only_drm.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/post_model.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/post_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from typing import TYPE_CHECKING, Any
 
 from ultima_scraper_api.apis.onlyfans import SiteContent
 from ultima_scraper_api.apis.onlyfans.classes.extras import endpoint_links
 
 if TYPE_CHECKING:
     from ultima_scraper_api.apis.onlyfans.classes.user_model import (
-        create_auth,
+        AuthModel,
         create_user,
     )
 
 
 class create_post(SiteContent):
-    def __init__(self, option: dict[str, Any], user: create_auth | create_user) -> None:
+    def __init__(self, option: dict[str, Any], user: AuthModel | create_user) -> None:
         SiteContent.__init__(self, option, user)
         self.responseType: str = option.get("responseType")
         self.createdAt: str = option.get("postedAt")
         self.postedAtPrecise: str = option.get("postedAtPrecise")
         self.expiredAt: Any = option.get("expiredAt")
         text: str = option.get("text", "")
         self.text = str(text or "")
@@ -48,15 +48,14 @@
         self.mentionedUsers: list = option.get("mentionedUsers")
         self.linkedUsers: list = option.get("linkedUsers")
         self.linkedPosts: list = option.get("linkedPosts")
         self.canViewMedia: bool = option.get("canViewMedia")
         self.preview: list[int] = option.get("preview", [])
         self.canPurchase: bool = option.get("canPurchase")
         self.comments: list[Any] = []
-        self.__raw__ = option
 
     def get_author(self):
         return self.author
 
     async def get_comments(self):
         epl = endpoint_links()
         link = epl.list_comments(self.responseType, self.id)
```

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/story_model.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/story_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/user_model.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/user_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 from ultima_scraper_api.apis.onlyfans.classes.extras import ErrorDetails, endpoint_links
 from ultima_scraper_api.apis.onlyfans.classes.hightlight_model import create_highlight
 from ultima_scraper_api.apis.onlyfans.classes.story_model import create_story
 from ultima_scraper_api.apis.user_streamliner import StreamlinedUser
 from ultima_scraper_api.managers.scrape_manager import ScrapeManager
 
 if TYPE_CHECKING:
-    from ultima_scraper_api.apis.onlyfans.classes.auth_model import create_auth
+    from ultima_scraper_api.apis.onlyfans.classes.auth_model import AuthModel
     from ultima_scraper_api.apis.onlyfans.classes.post_model import create_post
 
 
 class create_user(StreamlinedUser):
-    def __init__(self, option: dict[str, Any], authed: create_auth) -> None:
+    def __init__(self, option: dict[str, Any], authed: AuthModel) -> None:
         self.avatar: Optional[str] = option.get("avatar")
         self.avatarThumbs: Optional[list[str]] = option.get("avatarThumbs")
         self.header: Optional[str] = option.get("header")
         self.headerSize: Optional[dict[str, int]] = option.get("headerSize")
         self.headerThumbs: Optional[list[str]] = option.get("headerThumbs")
         self.id: int = option.get("id")
         self.name: str = option.get("name")
@@ -40,14 +40,15 @@
         self.tipsEnabled: bool = option.get("tipsEnabled")
         self.tipsTextEnabled: bool = option.get("tipsTextEnabled")
         self.tipsMin: int = option.get("tipsMin")
         self.tipsMax: int = option.get("tipsMax")
         self.canEarn: bool = option.get("canEarn")
         self.canAddSubscriber: bool = option.get("canAddSubscriber")
         self.subscribePrice: int = option.get("subscribePrice")
+        self.is_deleted: bool | None = option.get("isDeleted", None)
         self.hasStripe: bool = option.get("hasStripe")
         self.isStripeExist: bool = option.get("isStripeExist")
         self.subscriptionBundles: list = option.get("subscriptionBundles")
         self.canSendChatToAll: bool = option.get("canSendChatToAll")
         self.creditsMin: int = option.get("creditsMin")
         self.creditsMax: int = option.get("creditsMax")
         self.isPaywallRestriction: bool = option.get("isPaywallRestriction")
@@ -208,30 +209,42 @@
         self.connectedOfAccounts: list = option.get("connectedOfAccounts")
         self.hasPassword: bool = option.get("hasPassword")
         self.canConnectOfAccount: bool = option.get("canConnectOfAccount")
         self.pinnedPostsCount: int = option.get("pinnedPostsCount")
         self.maxPinnedPostsCount: int = option.get("maxPinnedPostsCount")
         # Custom
         authed.users.add(self)
+        self.username = self.get_username()
         self.download_info: dict[str, Any] = {}
         self.duplicate_media = []
         self.scrape_manager = ScrapeManager(authed.session_manager)
         self.__raw__ = option
         StreamlinedUser.__init__(self, authed)
 
+    def get_username(self):
+        if not self.username:
+            self.username = f"u{self.id}"
+        return self.username
+
     def get_link(self):
         link = f"https://onlyfans.com/{self.username}"
         return link
 
     def is_me(self) -> bool:
         status = False
         if self.email:
             status = True
         return status
 
+    def is_authed_user(self):
+        if self.id == self.get_authed().id:
+            return True
+        else:
+            return False
+
     async def get_stories(
         self, refresh: bool = True, limit: int = 100, offset: int = 0
     ) -> list[create_story]:
         result, status = await api_helper.default_data(self, refresh)
         if status:
             return result
         links = [
@@ -322,14 +335,16 @@
         offset: int = 0,
         depth: int = 1,
         refresh: bool = True,
     ):
         result, status = await api_helper.default_data(self, refresh)
         if status:
             return result
+        if self.is_deleted:
+            return result
         multiplier = self.get_session_manager().max_threads
         temp_limit = limit
         temp_offset = offset
         link = endpoint_links(
             identifier=self.id, global_limit=temp_limit, global_offset=temp_offset
         ).message_api
         unpredictable_links, new_offset = api_helper.calculate_the_unpredictable(
```

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/classes/make_settings.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/classes/make_settings.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/classes/prepare_directories.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/classes/prepare_directories.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/classes/prepare_metadata.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/classes/prepare_metadata.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/classes/prepare_webhooks.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/classes/prepare_webhooks.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/docs/Makefile` & `ultima_scraper_api-1.1.4/ultima_scraper_api/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/docs/make.bat` & `ultima_scraper_api-1.1.4/ultima_scraper_api/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/docs/source/conf.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/helpers/main_helper.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/helpers/main_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 import json
 import os
 import platform
 import re
 import secrets
 import shutil
 import subprocess
+from datetime import datetime
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, BinaryIO, Literal
 
 import orjson
 import requests
-from aiofiles import os as async_os
-from bs4 import BeautifulSoup
-from mergedeep import Strategy, merge  # type: ignore
-
 import ultima_scraper_api
 import ultima_scraper_api.classes.make_settings as make_settings
 import ultima_scraper_api.classes.prepare_webhooks as prepare_webhooks
+from aiofiles import os as async_os
+from bs4 import BeautifulSoup
+from dateutil.relativedelta import relativedelta
+from mergedeep import Strategy, merge  # type: ignore
 
 if TYPE_CHECKING:
     pass
 
 api_types = ultima_scraper_api.api_types
 auth_types = ultima_scraper_api.auth_types
 
@@ -299,14 +300,20 @@
     if x:
         x = x.group(1)
     else:
         x = s
     return x
 
 
+def extract_string_between_characters(text:str, opening_char:str, closing_char:str):
+    pattern = re.escape(opening_char) + r"(.*?)" + re.escape(closing_char)
+    matches = re.findall(pattern, text)
+    return matches
+
+
 def module_chooser(domain: str, json_sites: dict[str, Any]):
     string = "Select Site: "
     separator = " | "
     site_names: list[str] = []
     wl = ["onlyfans", "fansly"]
     bl = []
     site_count = len(json_sites)
@@ -327,7 +334,21 @@
         string = f"{domain} not supported"
         site_names = []
     return string, site_names
 
 
 async def replace_path(old_string: str, new_string: str, path: Path):
     return Path(path.as_posix().replace(old_string, new_string))
+
+
+def date_between_cur_month(date_value: datetime):
+    current_date = datetime.today()
+    first_day = current_date.replace(day=1)
+    last_day = first_day + relativedelta(months=1, days=-1)
+    if first_day.date() < date_value.date() < last_day.date():
+        return True
+    else:
+        return False
+
+
+def split_string(identifiers: str):
+    return identifiers.split(",")
```

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/managers/job_manager/job_manager.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/managers/job_manager/job_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/managers/job_manager/jobs/custom_job.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/managers/job_manager/jobs/custom_job.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/managers/scrape_manager.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/managers/scrape_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
         session_manager = self.session_manager
         auth = session_manager.auth
         if "error" in json_res:
             extras: dict[str, Any] = {}
             extras["auth"] = session_manager.auth
             extras["link"] = url
-            if isinstance(auth, onlyfans_classes.auth_model.create_auth):
+            if isinstance(auth, onlyfans_classes.auth_model.AuthModel):
                 handle_error_ = onlyfans_classes.extras.ErrorDetails
             else:
                 handle_error_ = fansly_classes.extras.ErrorDetails
 
             result = await handle_error_(json_res).format(extras)
             if self.handle_errors:
                 return await handle_error_details(result)
```

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/managers/session_manager.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/managers/session_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,17 @@
         if proxy is None:
             proxy = self.proxies[0]
         return ProxyConnector(**proxy._asdict())  # type: ignore
 
     def get_current_proxy(self):
         return self.proxies[self.current_proxy_index]
 
+    def add_proxy(self, proxy: str):
+        self.proxies.append(ProxyInfo(*python_socks.parse_proxy_url(proxy)))  # type: ignore
+
     async def proxy_switcher(self):
         if self.proxies:
             self.current_proxy_index = (self.current_proxy_index + 1) % len(
                 self.proxies
             )
             await self.session_manager.active_session.close()
             self.session_manager.active_session = (
@@ -68,15 +71,15 @@
                 )
             )
 
 
 class SessionManager:
     def __init__(
         self,
-        auth: auth_types,
+        auth: ultima_scraper_api.authenticator_types,
         headers: dict[str, Any] = {},
         proxies: list[str] = [],
         max_threads: int = -1,
         use_cookies: bool = True,
     ) -> None:
         max_threads = api_helper.calculate_max_threads(max_threads)
         self.semaphore = asyncio.BoundedSemaphore(max_threads)
@@ -103,22 +106,26 @@
         # self.rate_limit_wait_minutes = 6
         self.rate_limit_check = False
         self.is_rate_limited = None
         self.time2sleep = 0
         asyncio.create_task(self.check_rate_limit())
 
     def get_cookies(self):
-        import ultima_scraper_api.apis.fansly.classes as fansly_classes
+        from ultima_scraper_api.apis.fansly.fansly import FanslyAuthenticator
 
-        if isinstance(self.auth, fansly_classes.auth_model.create_auth):
+        if isinstance(self.auth, FanslyAuthenticator):
             final_cookies: dict[str, Any] = {}
         else:
             final_cookies = self.auth.auth_details.cookie.format()
         return final_cookies
 
+    def add_proxies(self, proxies: list[str] = []):
+        for proxy in proxies:
+            self.proxy_manager.add_proxy(proxy)
+
     def test_proxies(self, proxies: list[str] = []):
         final_proxies: list[str] = []
 
         session = requests.Session()
         proxies = proxies if proxies else self.proxies
         for proxy in proxies:
             url = "https://checkip.amazonaws.com"
@@ -273,25 +280,25 @@
                         )
             except Exception as _e:
                 pass
 
     async def bulk_requests(self, urls: list[str]) -> list[ClientResponse | None]:
         return await asyncio.gather(*[self.request(url) for url in urls])
 
-    async def json_request(self, url: str):
+    async def json_request(self, url: str, method: str = "GET"):
         while True:
-            response = await self.request(url)
+            response = await self.request(url, method)
             json_resp: dict[Any, Any] = {}
             try:
                 if response.status == 200:
                     json_resp = await response.json()
                 else:
                     json_resp["error"] = {
                         "code": response.status,
-                        "message": response.reason,
+                        "message": getattr(response, "reason"),
                     }
                 return json_resp
             except EXCEPTION_TEMPLATE as _e:
                 continue
 
     async def bulk_json_requests(self, urls: list[str]) -> list[dict[Any, Any]]:
         return await asyncio.gather(*[self.json_request(url) for url in urls])
@@ -352,15 +359,15 @@
                             # qwsd = list(response.request_info.headers.items())
                             result = await response.json()
                             if "error" in result:
                                 extras: dict[str, Any] = {}
                                 extras["auth"] = self.auth
                                 extras["link"] = link
                                 if isinstance(
-                                    self.auth, onlyfans_classes.auth_model.create_auth
+                                    self.auth, onlyfans_classes.auth_model.AuthModel
                                 ):
                                     handle_error = onlyfans_classes.extras.ErrorDetails
                                 else:
                                     handle_error = fansly_classes.extras.ErrorDetails
 
                                 result = await handle_error(result).format(extras)
                                 if _handle_error_details:
@@ -434,15 +441,17 @@
     ):
         # Users: 300000 | Creators: 301000
         headers: dict[str, Any] = {}
         final_time = str(int(round(time.time()))) if not time_ else str(time_)
         path = urlparse(link).path
         query = urlparse(link).query
         if query:
-            auth_id = self.auth.id if self.auth.id else auth_id
+            auth_id = (
+                self.auth.auth_details.id if self.auth.auth_details.id else auth_id
+            )
             headers["user-id"] = str(auth_id)
         path = path if not query else f"{path}?{query}"
         dynamic_rules = self.dynamic_rules
         a = [dynamic_rules["static_param"], final_time, path, str(auth_id)]
         msg = "\n".join(a)
         message = msg.encode("utf-8")
         hash_object = hashlib.sha1(message)
```

### Comparing `ultima_scraper_api-1.1.3/ultima_scraper_api/models/subscription_model.py` & `ultima_scraper_api-1.1.4/ultima_scraper_api/models/subscription_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.3/PKG-INFO` & `ultima_scraper_api-1.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-api
-Version: 1.1.3
+Version: 1.1.4
 Summary: 
 Author: DIGITALCRIMINALS
 Author-email: 89371864+digitalcriminals@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -13,14 +13,15 @@
 Requires-Dist: aiohttp-socks (>=0.8.0,<0.9.0)
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: dill (>=0.3.6,<0.4.0)
 Requires-Dist: lxml (>=4.9.1,<5.0.0)
 Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
 Requires-Dist: mypy (>=0.991,<0.992)
 Requires-Dist: orjson (>=3.8.3,<4.0.0)
+Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-socks[asyncio] (==2.2.0)
 Requires-Dist: pywidevine (>=1.6.0,<2.0.0)
 Requires-Dist: requests[socks] (==2.28.2)
 Requires-Dist: user-agent (>=0.1.10,<0.2.0)
 Requires-Dist: win32-setctime (>=1.1.0,<2.0.0) ; sys_platform == "win32"
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
```

