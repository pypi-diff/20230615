# Comparing `tmp/nonebot_plugin_pixivbot-1.9.0.tar.gz` & `tmp/nonebot_plugin_pixivbot-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pixivbot-1.9.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_pixivbot-2.0.0a1.tar", max compression
```

## Comparing `nonebot_plugin_pixivbot-1.9.0.tar` & `nonebot_plugin_pixivbot-2.0.0a1.tar`

### file list

```diff
@@ -1,171 +1,131 @@
--rw-r--r--   0        0        0     1085 2023-02-13 05:42:01.812872 nonebot_plugin_pixivbot-1.9.0/LICENSE
--rw-r--r--   0        0        0     1840 2023-06-14 11:53:13.246031 nonebot_plugin_pixivbot-1.9.0/pyproject.toml
--rw-r--r--   0        0        0    17595 2023-04-27 10:16:31.843054 nonebot_plugin_pixivbot-1.9.0/README.md
--rw-r--r--   0        0        0     1252 2023-06-14 11:53:13.242032 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/__init__.py
--rw-r--r--   0        0        0     7793 2023-04-27 09:37:04.739003 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/config.py
--rw-r--r--   0        0        0     4411 2023-04-27 10:16:31.872054 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/context.py
--rw-r--r--   0        0        0      443 2023-02-13 05:42:01.817870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/__init__.py
--rw-r--r--   0        0        0       56 2023-02-13 05:42:01.817870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/errors.py
--rw-r--r--   0        0        0     1515 2023-02-13 05:42:01.817870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/interval_task_repo.py
--rw-r--r--   0        0        0      488 2023-04-26 10:41:42.735891 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/local_tag/__init__.py
--rw-r--r--   0        0        0      535 2023-04-26 10:41:42.735891 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/local_tag/base.py
--rw-r--r--   0        0        0     2643 2023-04-26 10:41:42.736891 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/local_tag/mongo.py
--rw-r--r--   0        0        0     2702 2023-04-26 10:41:42.736891 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/local_tag/sql.py
--rw-r--r--   0        0        0      541 2023-04-26 10:41:42.737892 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_binding/__init__.py
--rw-r--r--   0        0        0      387 2023-04-26 10:41:42.737892 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_binding/base.py
--rw-r--r--   0        0        0     2087 2023-04-26 10:41:42.738890 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_binding/mongo.py
--rw-r--r--   0        0        0     2715 2023-04-26 10:41:42.739891 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_binding/sql.py
--rw-r--r--   0        0        0      262 2023-02-13 05:42:01.821870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/__init__.py
--rw-r--r--   0        0        0     1524 2023-02-13 05:42:01.822870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/base.py
--rw-r--r--   0        0        0     1829 2023-04-26 10:41:42.739891 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/compressor.py
--rw-r--r--   0        0        0      355 2023-02-13 05:42:01.822870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/enums.py
--rw-r--r--   0        0        0      334 2023-02-13 05:42:01.823870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/errors.py
--rw-r--r--   0        0        0     1036 2023-02-13 05:42:01.823870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/lazy_illust.py
--rw-r--r--   0        0        0      826 2023-03-15 03:52:01.493698 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/__init__.py
--rw-r--r--   0        0        0     2823 2023-03-15 03:26:56.195873 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/base.py
--rw-r--r--   0        0        0     3419 2023-04-26 10:41:42.740890 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/dummy.py
--rw-r--r--   0        0        0    31650 2023-04-26 10:41:42.820890 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo.py
--rw-r--r--   0        0        0     4802 2023-04-26 08:33:36.389185 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo_models.py
--rw-r--r--   0        0        0    33317 2023-04-26 10:41:42.821890 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql.py
--rw-r--r--   0        0        0     3536 2023-04-26 08:33:36.390185 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql_models.py
--rw-r--r--   0        0        0     9990 2023-04-26 10:41:42.822892 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator.py
--rw-r--r--   0        0        0    22139 2023-04-26 10:41:42.822892 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator_repo.py
--rw-r--r--   0        0        0      332 2023-04-26 10:41:42.823892 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/models.py
--rw-r--r--   0        0        0    18821 2023-04-27 13:33:43.566359 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/remote_repo.py
--rw-r--r--   0        0        0     1079 2023-02-13 05:42:01.829870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/source/__init__.py
--rw-r--r--   0        0        0     1820 2023-02-13 05:42:01.830870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/source/lifecycle_mixin.py
--rw-r--r--   0        0        0     3211 2023-02-13 05:42:01.830870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/source/migration_manager.py
--rw-r--r--   0        0        0     5774 2023-04-26 10:41:42.787891 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/source/mongo/__init__.py
--rw-r--r--   0        0        0      290 2023-04-26 10:41:42.743890 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/source/mongo/meta_info.py
--rw-r--r--   0        0        0      693 2023-02-13 05:42:01.833870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/source/mongo/migration/__init__.py
--rw-r--r--   0        0        0     1424 2023-02-13 05:42:01.833870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v1_to_v2.py
--rw-r--r--   0        0        0      674 2023-02-13 05:42:01.833870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v2_to_v3.py
--rw-r--r--   0        0        0     2729 2023-02-13 05:42:01.834869 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v3_to_v4.py
--rw-r--r--   0        0        0     1039 2023-02-13 05:42:01.834869 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v4_to_v5.py
--rw-r--r--   0        0        0     3306 2023-02-13 05:42:01.834869 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v5_to_v6.py
--rw-r--r--   0        0        0      416 2023-02-13 05:42:01.835870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/source/mongo/migration/mongo_v6_to_v7.py
--rw-r--r--   0        0        0     5781 2023-04-26 10:41:42.788890 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/source/sql/__init__.py
--rw-r--r--   0        0        0      306 2023-03-13 13:51:04.755048 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/source/sql/meta_info.py
--rw-r--r--   0        0        0      457 2023-02-13 05:42:01.837870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/source/sql/migration/__init__.py
--rw-r--r--   0        0        0     3824 2023-02-13 05:42:01.838869 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v1_to_v2.py
--rw-r--r--   0        0        0     1842 2023-02-13 05:42:01.839869 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v2_to_v3.py
--rw-r--r--   0        0        0      360 2023-02-13 05:42:01.839869 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v3_to_v4.py
--rw-r--r--   0        0        0      520 2023-04-26 10:41:42.744892 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/subscription/__init__.py
--rw-r--r--   0        0        0      177 2023-04-26 10:41:42.745891 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/subscription/base.py
--rw-r--r--   0        0        0     4446 2023-04-26 10:41:42.745891 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/subscription/mongo.py
--rw-r--r--   0        0        0     5698 2023-04-26 10:41:42.746890 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/subscription/sql.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.842870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/utils/__init__.py
--rw-r--r--   0        0        0      164 2023-02-13 05:42:01.842870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/utils/shortuuid.py
--rw-r--r--   0        0        0      814 2023-02-13 05:42:01.843869 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/utils/sql/__init__.py
--rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843869 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/utils/sql/utc_datetime.py
--rw-r--r--   0        0        0      720 2023-02-13 05:42:01.842870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/utils/sql.pyi
--rw-r--r--   0        0        0      517 2023-04-26 10:41:42.747890 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/watch_task/__init__.py
--rw-r--r--   0        0        0      226 2023-04-26 10:41:42.747890 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/watch_task/base.py
--rw-r--r--   0        0        0     5155 2023-04-26 10:41:42.748890 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/watch_task/mongo.py
--rw-r--r--   0        0        0     6613 2023-04-26 10:41:42.748890 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/watch_task/sql.py
--rw-r--r--   0        0        0      964 2023-03-15 03:24:39.857013 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/enums.py
--rw-r--r--   0        0        0      102 2023-02-14 03:27:31.463009 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/global_context.py
--rw-r--r--   0        0        0       92 2023-02-13 05:42:01.847870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/__init__.py
--rw-r--r--   0        0        0     9597 2023-04-26 11:20:41.866640 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/base.py
--rw-r--r--   0        0        0      308 2023-02-13 05:42:01.847870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/command/__init__.py
--rw-r--r--   0        0        0     2489 2023-04-26 11:20:41.835065 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/command/bind.py
--rw-r--r--   0        0        0     2481 2023-03-29 02:34:22.114209 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/command/command.py
--rw-r--r--   0        0        0     1207 2023-04-26 11:20:41.815065 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/command/help.py
--rw-r--r--   0        0        0      804 2023-04-26 11:20:41.870642 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/command/invalidate_cache.py
--rw-r--r--   0        0        0     4291 2023-04-26 11:28:38.961827 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/command/schedule.py
--rw-r--r--   0        0        0     1363 2023-03-29 02:34:22.116335 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/command/subcommand.py
--rw-r--r--   0        0        0     6050 2023-04-26 11:28:38.966828 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/command/watch.py
--rw-r--r--   0        0        0      633 2023-02-13 05:42:01.851870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/common/__init__.py
--rw-r--r--   0        0        0      688 2023-03-29 02:34:22.117934 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/common/base.py
--rw-r--r--   0        0        0     1635 2023-06-14 11:49:20.424779 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/common/illust.py
--rw-r--r--   0        0        0     1465 2023-06-14 11:49:20.376253 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/common/more.py
--rw-r--r--   0        0        0     2842 2023-06-14 11:49:20.420780 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/common/random_bookmark.py
--rw-r--r--   0        0        0     1767 2023-06-14 11:49:20.400777 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/common/random_illust.py
--rw-r--r--   0        0        0     1624 2023-06-14 11:49:20.357703 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/common/random_recommended_illust.py
--rw-r--r--   0        0        0     2006 2023-04-26 11:20:41.839065 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/common/random_related_illust.py
--rw-r--r--   0        0        0     2104 2023-06-14 11:49:20.386252 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/common/random_user_illust.py
--rw-r--r--   0        0        0     4224 2023-06-14 11:49:20.410778 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/common/ranking.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.857869 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/interceptor/__init__.py
--rw-r--r--   0        0        0      524 2023-03-29 02:34:22.124122 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/interceptor/base.py
--rw-r--r--   0        0        0     2012 2023-03-29 02:34:22.125123 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/interceptor/combined_interceptor.py
--rw-r--r--   0        0        0     1601 2023-04-27 13:28:45.858775 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/interceptor/default_error_interceptor.py
--rw-r--r--   0        0        0     1134 2023-03-29 02:34:22.126120 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/interceptor/loading_prompt_interceptor.py
--rw-r--r--   0        0        0     1947 2023-03-29 02:34:54.094101 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/interceptor/permission_interceptor.py
--rw-r--r--   0        0        0      654 2023-03-29 02:34:22.127120 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/interceptor/record_req_interceptor.py
--rw-r--r--   0        0        0      938 2023-04-27 15:02:23.301078 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/interceptor/retry_interceptor.py
--rw-r--r--   0        0        0     1526 2023-03-29 02:34:22.128120 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/interceptor/service_interceptor.py
--rw-r--r--   0        0        0      673 2023-03-29 02:34:22.129121 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/interceptor/timeout_interceptor.py
--rw-r--r--   0        0        0      201 2023-02-13 05:42:01.861870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/pkg_context.py
--rw-r--r--   0        0        0     3378 2023-04-26 10:41:42.749891 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/recorder.py
--rw-r--r--   0        0        0      325 2023-02-14 11:56:02.041347 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/schedule/__init__.py
--rw-r--r--   0        0        0      349 2023-04-26 11:20:41.850065 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/schedule/base.py
--rw-r--r--   0        0        0      461 2023-03-29 02:34:22.131121 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/schedule/random_bookmark.py
--rw-r--r--   0        0        0      453 2023-03-29 02:34:22.131121 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/schedule/random_illust.py
--rw-r--r--   0        0        0      498 2023-03-29 02:34:22.132122 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/schedule/random_recommended_illust.py
--rw-r--r--   0        0        0      470 2023-03-29 02:34:22.132122 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/schedule/random_user_illust.py
--rw-r--r--   0        0        0      432 2023-03-29 02:34:22.133120 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/schedule/ranking.py
--rw-r--r--   0        0        0       27 2023-02-13 05:42:01.862870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/sniffer/__init__.py
--rw-r--r--   0        0        0     1017 2023-06-14 11:49:20.366702 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/sniffer/illust_link.py
--rw-r--r--   0        0        0     1324 2023-06-14 11:49:20.390967 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/utils.py
--rw-r--r--   0        0        0      112 2023-02-14 12:15:47.490983 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/watch/__init__.py
--rw-r--r--   0        0        0      865 2023-04-26 11:20:41.827066 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/watch/base.py
--rw-r--r--   0        0        0     2498 2023-04-26 10:41:42.749891 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/watch/following_illusts.py
--rw-r--r--   0        0        0     1864 2023-04-26 10:41:42.750890 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/watch/user_illusts.py
--rw-r--r--   0        0        0      530 2023-02-13 05:42:01.865869 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/model/__init__.py
--rw-r--r--   0        0        0     1366 2023-02-13 05:42:01.865869 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/model/identifier.py
--rw-r--r--   0        0        0     1858 2023-04-27 09:18:54.765186 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/model/illust.py
--rw-r--r--   0        0        0      352 2023-02-13 05:42:01.866870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/model/interval_task.py
--rw-r--r--   0        0        0      157 2023-02-13 05:42:01.867870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/model/message/__init__.py
--rw-r--r--   0        0        0     2623 2023-02-13 05:42:01.867870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/model/message/illust_message.py
--rw-r--r--   0        0        0     2443 2023-02-13 05:42:01.867870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/model/message/illust_messages.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.868870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/model/old/__init__.py
--rw-r--r--   0        0        0      120 2023-02-13 05:42:01.868870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/model/old/pixiv_binding.py
--rw-r--r--   0        0        0      950 2023-02-13 05:42:01.868870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/model/old/subscription.py
--rw-r--r--   0        0        0      242 2023-02-13 05:42:01.869870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/model/pixiv_binding.py
--rw-r--r--   0        0        0     1450 2023-04-26 10:52:37.464803 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/model/subscription.py
--rw-r--r--   0        0        0      203 2023-02-13 05:42:01.870869 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/model/tag.py
--rw-r--r--   0        0        0      131 2023-02-13 05:42:01.870869 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/model/user.py
--rw-r--r--   0        0        0      242 2023-02-13 05:42:01.871622 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/model/user_preview.py
--rw-r--r--   0        0        0     1004 2023-04-26 10:52:37.460801 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/model/watch_task.py
--rw-r--r--   0        0        0     1680 2023-02-14 03:39:10.628376 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/plugin_service.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.872870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/protocol_dep/__init__.py
--rw-r--r--   0        0        0      914 2023-03-14 09:12:27.158624 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/protocol_dep/authenticator.py
--rw-r--r--   0        0        0     2757 2023-03-29 02:34:22.136711 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/protocol_dep/post_dest.py
--rw-r--r--   0        0        0     1445 2023-02-14 03:32:29.851104 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/protocol_dep/postman.py
--rw-r--r--   0        0        0     1452 2023-02-14 03:32:29.852102 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/protocol_dep/protocol_dep.py
--rw-r--r--   0        0        0       49 2023-02-13 05:42:01.874870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/service/__init__.py
--rw-r--r--   0        0        0     5470 2023-04-27 13:38:00.669631 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/service/interval_task_worker.py
--rw-r--r--   0        0        0      958 2023-04-26 10:41:42.751891 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/service/pixiv_account_binder.py
--rw-r--r--   0        0        0     6023 2023-04-26 10:41:42.751891 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/service/pixiv_service.py
--rw-r--r--   0        0        0     2244 2023-02-13 05:42:01.877869 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/service/roulette.py
--rw-r--r--   0        0        0     5640 2023-04-26 10:41:42.752891 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/service/scheduler.py
--rw-r--r--   0        0        0     3821 2023-04-26 10:41:42.752891 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/service/watchman.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.878870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/utils/__init__.py
--rw-r--r--   0        0        0      230 2023-03-29 02:34:22.138709 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/utils/algorithm.py
--rw-r--r--   0        0        0      265 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/utils/coros.py
--rw-r--r--   0        0        0     1148 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/utils/decode_integer.py
--rw-r--r--   0        0        0      515 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/utils/errors.py
--rw-r--r--   0        0        0     3604 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/utils/expires_lru_dict.py
--rw-r--r--   0        0        0       95 2023-04-26 10:41:42.825893 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/utils/format.py
--rw-r--r--   0        0        0      494 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/utils/lazy_delegation.py
--rw-r--r--   0        0        0     4188 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/utils/lifecycler.py
--rw-r--r--   0        0        0      776 2023-03-01 13:53:49.845581 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/utils/nonebot.py
--rw-r--r--   0        0        0     8653 2023-04-27 14:59:21.481094 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/utils/shared_agen.py
--rw-r--r--   0        0        0      384 2023-02-13 05:42:01.882870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot_kook/__init__.py
--rw-r--r--   0        0        0      866 2023-03-14 09:12:27.159625 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot_kook/config.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.883870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot_kook/protocol_dep/__init__.py
--rw-r--r--   0        0        0     5195 2023-03-23 15:08:25.496164 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot_kook/protocol_dep/authenticator.py
--rw-r--r--   0        0        0     5346 2023-03-23 15:08:25.498161 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot_kook/protocol_dep/post_dest.py
--rw-r--r--   0        0        0     2046 2023-02-14 03:32:29.855103 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot_kook/protocol_dep/postman.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.885870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot_kook/utils/__init__.py
--rw-r--r--   0        0        0     1083 2023-02-13 05:42:01.885870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot_kook/utils/card_builder.py
--rw-r--r--   0        0        0     1008 2023-02-13 05:42:01.886870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot_kook/utils/illust_card.py
--rw-r--r--   0        0        0      479 2023-04-26 08:29:16.962322 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot_onebot_v11/__init__.py
--rw-r--r--   0        0        0      896 2023-02-13 05:42:01.887870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot_onebot_v11/config.py
--rw-r--r--   0        0        0       20 2023-03-29 02:34:22.139710 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot_onebot_v11/handler/__init__.py
--rw-r--r--   0        0        0     1468 2023-03-29 02:34:22.140709 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot_onebot_v11/handler/poke.py
--rw-r--r--   0        0        0        0 2023-02-13 05:42:01.888870 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/__init__.py
--rw-r--r--   0        0        0     1512 2023-02-14 03:32:29.856103 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/authenticator.py
--rw-r--r--   0        0        0     4845 2023-04-27 09:44:58.747904 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/post_dest.py
--rw-r--r--   0        0        0     4028 2023-04-27 13:34:24.653172 nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/postman.py
--rw-r--r--   0        0        0    19118 1970-01-01 00:00:00.000000 nonebot_plugin_pixivbot-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-02-13 05:42:01.812872 nonebot_plugin_pixivbot-2.0.0a1/LICENSE
+-rw-r--r--   0        0        0     1179 2023-06-15 02:11:03.871897 nonebot_plugin_pixivbot-2.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0    17595 2023-04-27 10:16:31.843054 nonebot_plugin_pixivbot-2.0.0a1/README.md
+-rw-r--r--   0        0        0      915 2023-06-15 01:44:24.090734 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/__init__.py
+-rw-r--r--   0        0        0     7217 2023-06-15 01:44:24.091241 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/config.py
+-rw-r--r--   0        0        0     4411 2023-04-27 10:16:31.872054 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/context.py
+-rw-r--r--   0        0        0        0 2023-06-15 01:44:24.091241 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/__init__.py
+-rw-r--r--   0        0        0       56 2023-02-13 05:42:01.817000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/errors.py
+-rw-r--r--   0        0        0      924 2023-06-15 01:44:24.092249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/interval_task_repo.py
+-rw-r--r--   0        0        0     2541 2023-06-15 01:44:24.092249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/local_tag.py
+-rw-r--r--   0        0        0      858 2023-06-15 01:44:24.092249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/nb_session.py
+-rw-r--r--   0        0        0     2513 2023-06-15 01:44:24.093248 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_binding.py
+-rw-r--r--   0        0        0      262 2023-02-13 05:42:01.821000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/__init__.py
+-rw-r--r--   0        0        0     1524 2023-02-13 05:42:01.822000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/base.py
+-rw-r--r--   0        0        0     1829 2023-04-26 10:41:42.739000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/compressor.py
+-rw-r--r--   0        0        0      355 2023-02-13 05:42:01.822000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/enums.py
+-rw-r--r--   0        0        0      334 2023-02-13 05:42:01.823000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/errors.py
+-rw-r--r--   0        0        0     1036 2023-02-13 05:42:01.823000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/lazy_illust.py
+-rw-r--r--   0        0        0      532 2023-06-15 01:44:24.093248 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/__init__.py
+-rw-r--r--   0        0        0     2823 2023-03-15 03:26:56.195000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/base.py
+-rw-r--r--   0        0        0     3419 2023-04-26 10:41:42.740000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/dummy.py
+-rw-r--r--   0        0        0    33227 2023-06-15 01:44:24.094251 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql.py
+-rw-r--r--   0        0        0     3460 2023-06-15 01:44:24.094251 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql_models.py
+-rw-r--r--   0        0        0     9990 2023-04-26 10:41:42.822000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator.py
+-rw-r--r--   0        0        0    22139 2023-04-26 10:41:42.822000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator_repo.py
+-rw-r--r--   0        0        0      332 2023-04-26 10:41:42.823000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/models.py
+-rw-r--r--   0        0        0    18821 2023-04-27 13:33:43.566000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/remote_repo.py
+-rw-r--r--   0        0        0        0 2023-06-15 01:44:24.095249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/__init__.py
+-rw-r--r--   0        0        0     1815 2023-06-15 01:44:24.095249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/lifecycle_mixin.py
+-rw-r--r--   0        0        0     3211 2023-02-13 05:42:01.830000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/migration_manager.py
+-rw-r--r--   0        0        0     5411 2023-06-15 01:44:24.096249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/sql/__init__.py
+-rw-r--r--   0        0        0      270 2023-06-15 01:44:24.096249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/sql/meta_info.py
+-rw-r--r--   0        0        0      523 2023-06-15 01:44:24.097249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/sql/migration/__init__.py
+-rw-r--r--   0        0        0     3824 2023-02-13 05:42:01.838000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v1_to_v2.py
+-rw-r--r--   0        0        0     1783 2023-06-15 01:44:24.097249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v2_to_v3.py
+-rw-r--r--   0        0        0      327 2023-06-15 01:44:24.098250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v3_to_v4.py
+-rw-r--r--   0        0        0     8662 2023-06-15 01:44:24.098250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v4_to_v5.py
+-rw-r--r--   0        0        0     5554 2023-06-15 01:44:24.099249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/subscription.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.842000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/utils/__init__.py
+-rw-r--r--   0        0        0      164 2023-02-13 05:42:01.842000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/utils/shortuuid.py
+-rw-r--r--   0        0        0      814 2023-02-13 05:42:01.843000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/utils/sql/__init__.py
+-rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/utils/sql/utc_datetime.py
+-rw-r--r--   0        0        0      720 2023-02-13 05:42:01.842000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/utils/sql.pyi
+-rw-r--r--   0        0        0     6474 2023-06-15 01:44:24.099249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/watch_task.py
+-rw-r--r--   0        0        0      870 2023-06-15 01:44:24.100250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/enums.py
+-rw-r--r--   0        0        0      102 2023-02-14 03:27:31.463009 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/global_context.py
+-rw-r--r--   0        0        0       92 2023-02-13 05:42:01.847870 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/__init__.py
+-rw-r--r--   0        0        0     9360 2023-06-15 01:44:24.100250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/base.py
+-rw-r--r--   0        0        0      308 2023-02-13 05:42:01.847870 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/command/__init__.py
+-rw-r--r--   0        0        0     2318 2023-06-15 01:44:24.101249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/command/bind.py
+-rw-r--r--   0        0        0     2500 2023-06-15 01:44:24.101249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/command/command.py
+-rw-r--r--   0        0        0      369 2023-06-15 01:44:24.102249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/command/help.py
+-rw-r--r--   0        0        0      696 2023-06-15 01:44:24.102249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/command/invalidate_cache.py
+-rw-r--r--   0        0        0     4064 2023-06-15 01:44:24.103249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/command/schedule.py
+-rw-r--r--   0        0        0     1342 2023-06-15 01:44:24.103249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/command/subcommand.py
+-rw-r--r--   0        0        0     5664 2023-06-15 01:44:24.104250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/command/watch.py
+-rw-r--r--   0        0        0      633 2023-02-13 05:42:01.851870 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/__init__.py
+-rw-r--r--   0        0        0      688 2023-03-29 02:34:22.117934 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/base.py
+-rw-r--r--   0        0        0     1560 2023-06-15 01:44:24.104250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/illust.py
+-rw-r--r--   0        0        0     1369 2023-06-15 01:44:24.105250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/more.py
+-rw-r--r--   0        0        0     2558 2023-06-15 01:44:24.105250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/random_bookmark.py
+-rw-r--r--   0        0        0     1790 2023-06-15 01:44:24.106249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/random_illust.py
+-rw-r--r--   0        0        0     1566 2023-06-15 01:44:24.106249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/random_recommended_illust.py
+-rw-r--r--   0        0        0     1992 2023-06-15 01:44:24.107248 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/random_related_illust.py
+-rw-r--r--   0        0        0     2148 2023-06-15 01:44:24.107248 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/random_user_illust.py
+-rw-r--r--   0        0        0     4180 2023-06-15 01:44:24.108251 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/ranking.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.857869 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/__init__.py
+-rw-r--r--   0        0        0      494 2023-06-15 01:44:24.108251 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/base.py
+-rw-r--r--   0        0        0     1982 2023-06-15 01:44:24.109250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/combined_interceptor.py
+-rw-r--r--   0        0        0     1571 2023-06-15 01:44:24.109250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/default_error_interceptor.py
+-rw-r--r--   0        0        0     1218 2023-06-15 01:44:24.110248 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/loading_prompt_interceptor.py
+-rw-r--r--   0        0        0     1855 2023-06-15 01:44:24.110248 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/permission_interceptor.py
+-rw-r--r--   0        0        0      538 2023-06-15 01:44:24.111251 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/record_req_interceptor.py
+-rw-r--r--   0        0        0      887 2023-06-15 01:44:24.111251 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/retry_interceptor.py
+-rw-r--r--   0        0        0     1654 2023-06-15 01:44:24.112250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/service_interceptor.py
+-rw-r--r--   0        0        0      609 2023-06-15 01:44:24.112250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/timeout_interceptor.py
+-rw-r--r--   0        0        0      157 2023-06-15 01:44:24.113251 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/pkg_context.py
+-rw-r--r--   0        0        0     2620 2023-06-15 01:44:24.113251 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/recorder.py
+-rw-r--r--   0        0        0      325 2023-02-14 11:56:02.041347 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/schedule/__init__.py
+-rw-r--r--   0        0        0      349 2023-04-26 11:20:41.850065 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/schedule/base.py
+-rw-r--r--   0        0        0      461 2023-03-29 02:34:22.131121 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/schedule/random_bookmark.py
+-rw-r--r--   0        0        0      453 2023-03-29 02:34:22.131121 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/schedule/random_illust.py
+-rw-r--r--   0        0        0      498 2023-03-29 02:34:22.132122 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/schedule/random_recommended_illust.py
+-rw-r--r--   0        0        0      470 2023-03-29 02:34:22.132122 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/schedule/random_user_illust.py
+-rw-r--r--   0        0        0      432 2023-03-29 02:34:22.133120 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/schedule/ranking.py
+-rw-r--r--   0        0        0       27 2023-02-13 05:42:01.862870 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/sniffer/__init__.py
+-rw-r--r--   0        0        0     1051 2023-06-15 01:44:24.114250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/sniffer/illust_link.py
+-rw-r--r--   0        0        0     1219 2023-06-15 01:44:24.114250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/utils.py
+-rw-r--r--   0        0        0      112 2023-02-14 12:15:47.490983 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/watch/__init__.py
+-rw-r--r--   0        0        0      865 2023-04-26 11:20:41.827066 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/watch/base.py
+-rw-r--r--   0        0        0     2363 2023-06-15 01:44:24.115250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/watch/following_illusts.py
+-rw-r--r--   0        0        0     1759 2023-06-15 01:44:24.116249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/watch/user_illusts.py
+-rw-r--r--   0        0        0      394 2023-06-15 01:44:24.116249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/__init__.py
+-rw-r--r--   0        0        0     1858 2023-04-27 09:18:54.765186 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/illust.py
+-rw-r--r--   0        0        0      157 2023-06-15 01:44:24.117251 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/interval_task.py
+-rw-r--r--   0        0        0      157 2023-02-13 05:42:01.867870 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/message/__init__.py
+-rw-r--r--   0        0        0     2512 2023-06-15 01:44:24.117251 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/message/illust_message.py
+-rw-r--r--   0        0        0     2379 2023-06-15 01:44:24.118248 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/message/illust_messages.py
+-rw-r--r--   0        0        0      129 2023-06-15 01:44:24.118248 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/pixiv_binding.py
+-rw-r--r--   0        0        0     1376 2023-06-15 01:44:24.118248 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/subscription.py
+-rw-r--r--   0        0        0      203 2023-02-13 05:42:01.870869 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/tag.py
+-rw-r--r--   0        0        0      131 2023-02-13 05:42:01.870869 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/user.py
+-rw-r--r--   0        0        0      242 2023-02-13 05:42:01.871622 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/user_preview.py
+-rw-r--r--   0        0        0      930 2023-06-15 01:44:24.119250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/watch_task.py
+-rw-r--r--   0        0        0      208 2023-06-15 01:44:24.119250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/platform/__init__.py
+-rw-r--r--   0        0        0      531 2023-06-15 01:44:24.120252 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/platform/available/__init__.py
+-rw-r--r--   0        0        0     4368 2023-06-15 01:44:24.120252 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/platform/available/kaiheila.py
+-rw-r--r--   0        0        0      826 2023-06-15 01:44:24.121250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/platform/available/onebot_v11.py
+-rw-r--r--   0        0        0      878 2023-06-15 01:44:24.121250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/platform/func_manager.py
+-rw-r--r--   0        0        0     1680 2023-06-14 12:11:02.914517 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/plugin_service.py
+-rw-r--r--   0        0        0       49 2023-02-13 05:42:01.874870 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/service/__init__.py
+-rw-r--r--   0        0        0     4494 2023-06-15 01:44:24.122249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/service/interval_task_worker.py
+-rw-r--r--   0        0        0      844 2023-06-15 01:44:24.122249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/service/pixiv_account_binder.py
+-rw-r--r--   0        0        0     6023 2023-04-26 10:41:42.751891 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/service/pixiv_service.py
+-rw-r--r--   0        0        0     4506 2023-06-15 02:08:21.682591 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/service/postman.py
+-rw-r--r--   0        0        0     2244 2023-02-13 05:42:01.877869 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/service/roulette.py
+-rw-r--r--   0        0        0     5082 2023-06-15 01:44:24.123250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/service/scheduler.py
+-rw-r--r--   0        0        0     3170 2023-06-15 01:44:24.124250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/service/watchman.py
+-rw-r--r--   0        0        0      790 2023-06-15 01:44:24.124250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/usage.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.878870 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/__init__.py
+-rw-r--r--   0        0        0      230 2023-03-29 02:34:22.138709 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/algorithm.py
+-rw-r--r--   0        0        0      265 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/coros.py
+-rw-r--r--   0        0        0     1148 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/decode_integer.py
+-rw-r--r--   0        0        0      515 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/errors.py
+-rw-r--r--   0        0        0     3604 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/expires_lru_dict.py
+-rw-r--r--   0        0        0       95 2023-04-26 10:41:42.825893 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/format.py
+-rw-r--r--   0        0        0      494 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/lazy_delegation.py
+-rw-r--r--   0        0        0     4188 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/lifecycler.py
+-rw-r--r--   0        0        0      324 2023-06-15 01:44:24.125249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/nonebot.py
+-rw-r--r--   0        0        0     8653 2023-04-27 14:59:21.481094 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/shared_agen.py
+-rw-r--r--   0        0        0    18550 1970-01-01 00:00:00.000000 nonebot_plugin_pixivbot-2.0.0a1/PKG-INFO
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/LICENSE` & `nonebot_plugin_pixivbot-2.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/pyproject.toml` & `nonebot_plugin_pixivbot-2.0.0a1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,42 @@
 [tool.poetry]
 name = "nonebot-plugin-pixivbot"
-version = "1.9.0"
+version = "2.0.0a1"
 description = "Nonebot Plugin PixivBot"
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/ssttkkl/nonebot-plugin-pixivbot"
 packages = [
-    { include = "nonebot_plugin_pixivbot", from = "src" },
-    { include = "nonebot_plugin_pixivbot_onebot_v11", from = "src" },
-    { include = "nonebot_plugin_pixivbot_kook", from = "src" },
+    { include = "nonebot_plugin_pixivbot", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 nonebot2 = "^2.0.0"
 nonebot_plugin_apscheduler = "^0.2.0"
-nonebot-plugin-access-control = "^0.4.0"
+nonebot-plugin-access-control = ">=0.5.5"
+nonebot-plugin-session = ">=0.0.4"
+nonebot-plugin-send-anything-anywhere = "^0.2.7"
 PixivPy-Async = "^1.2.14"
 Pillow = "^9.2.0"
 numpy = "^1.23.1"
 lazy = "^1.4"
 aiohttp-socks = "^0.8.0"
 frozendict = "^2.3.4"
-tzlocal = "^4.2"
+tzlocal = "^5.0.1"
 cachetools = "^5.2.0"
 asyncache = "^0.3.1"
 shortuuid = "^1.0.9"
 
-nonebot-adapter-onebot = { version = "^2.2.1", optional = true }
-nonebot-adapter-kaiheila = { version = "^0.2.0", optional = true }
-nonebot-adapter-telegram = { version = "^0.1.0b8", optional = true }
-
-motor = { version = "^3.0.0", optional = true }
-beanie = { version = "^1.17.0", optional = true }
-
-SQLAlchemy = { version = "^2.0.0", extras = ["asyncio"] }
-aiosqlite = "^0.18.0"
-asyncpg = { version = "^0.27.0", optional = true }
-nonebot-plugin-localstore = "^0.4.1"
-
 [tool.poetry.group.dev.dependencies]
 nb-cli = "^1.0.5"
 flake8 = "^6.0.0"
-nonebug = "^0.3.1"
-pytest-mock = "^3.10.0"
-pytest-cov = "^4.0.0"
+asyncpg = "^0.27.0"
 nonebot2 = { extras = ["fastapi", "websocket", "httpx"], version = "^2.0.0" }
-
-[tool.poetry.extras]
-onebot = ["nonebot-adapter-onebot"]
-kook = ["nonebot-adapter-kaiheila"]
-telegram = ["nonebot-adapter-telegram"]
-mongo = ["beanie", "motor"]
-postgresql = ["asyncpg"]
+nonebot-adapter-onebot = "^2.2.1"
+nonebot-adapter-kaiheila = "^0.2.0"
+nonebot-adapter-qqguild = "^0.2.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/README.md` & `nonebot_plugin_pixivbot-2.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/config.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,92 +1,70 @@
 from pathlib import Path
-from typing import Optional, List
+from typing import Optional, List, Literal
 from urllib.parse import urlparse
 
 from nonebot import get_driver, logger, require
 from pydantic import BaseSettings, validator, root_validator
 from pydantic.fields import ModelField
 
 require("nonebot_plugin_localstore")
 
 import nonebot_plugin_localstore as store
 
-from nonebot_plugin_pixivbot.enums import *
-from nonebot_plugin_pixivbot.enums import DataSourceType
-from nonebot_plugin_pixivbot.global_context import context
-
-
-def _deprecated_warn(name: str):
-    logger.warning(f"config \"{name}\" is deprecated, use nonebot-plugin-access-control instead "
-                   "(MORE INFO: https://github.com/ssttkkl/nonebot-plugin-pixivbot#%E6%9D%83%E9%99%90%E6%8E%A7%E5%88%B6)")
+from .enums import *
+from .global_context import context
 
 
 def _get_default_sql_conn_url():
     # 旧版本的sqlite数据库在working directory
     data_file = Path("pixiv_bot.db")
     if not data_file.exists():
         data_file = store.get_data_file("nonebot_plugin_pixivbot", "pixiv_bot.db")
 
     return "sqlite+aiosqlite:///" + str(data_file)
 
 
 @context.register_singleton(**get_driver().config.dict())
 class Config(BaseSettings):
     @root_validator(pre=True, allow_reuse=True)
-    def deprecated_config(cls, values):
+    def deprecated_access_control_config(cls, values):
         for name in {"blacklist", "pixiv_query_cooldown", "pixiv_no_query_cooldown_users"}:
             if name in values:
-                _deprecated_warn(name)
+                logger.warning(f"config \"{name}\" is deprecated, use nonebot-plugin-access-control instead "
+                               "(MORE INFO: https://github.com/ssttkkl/nonebot-plugin-pixivbot#%E6%9D%83%E9%99%90%E6%8E%A7%E5%88%B6)")
+        return values
+
+    @root_validator(pre=True, allow_reuse=True)
+    def deprecated_mongodb_config(cls, values):
+        if values.get("pixiv_data_source", "sql") == "mongo" or "pixiv_mongo_conn_url" in values:
+            logger.warning("mongo support was removed, use sql instead")
         return values
 
     pixiv_refresh_token: str
 
-    pixiv_data_source: DataSourceType = DataSourceType.sql
-    pixiv_mongo_conn_url: str
-    pixiv_mongo_database_name: str
     pixiv_sql_conn_url: str
     pixiv_sql_dialect: str
     pixiv_use_local_cache: bool = True
 
     @root_validator(pre=True, allow_reuse=True)
-    def detect_data_source(cls, values):
-        pixiv_data_source = values.get("pixiv_data_source", None)
-        pixiv_mongo_conn_url = values.get("pixiv_mongo_conn_url", None)
-
-        if pixiv_data_source is None:
-            if pixiv_mongo_conn_url is not None:
-                pixiv_data_source = DataSourceType.mongo
-            else:
-                pixiv_data_source = DataSourceType.sql
-
-        values["pixiv_data_source"] = pixiv_data_source
-        return values
-
-    @root_validator(pre=True, allow_reuse=True)
     def default_sql_conn_url(cls, values):
         if "pixiv_sql_conn_url" not in values:
             values["pixiv_sql_conn_url"] = _get_default_sql_conn_url()
         return values
 
     @root_validator(pre=True, allow_reuse=True)
     def detect_sql_dialect(cls, values):
-        pixiv_data_source = values["pixiv_data_source"]
+        values["pixiv_mongo_conn_url"] = ""
+        values["pixiv_mongo_database_name"] = ""
 
-        if pixiv_data_source == DataSourceType.sql:
-            values["pixiv_mongo_conn_url"] = ""
-            values["pixiv_mongo_database_name"] = ""
-
-            url = urlparse(values["pixiv_sql_conn_url"])
-            if '+' in url.scheme:
-                pixiv_sql_dialect = url.scheme.split('+')[0]
-            else:
-                pixiv_sql_dialect = url.scheme
+        url = urlparse(values["pixiv_sql_conn_url"])
+        if '+' in url.scheme:
+            pixiv_sql_dialect = url.scheme.split('+')[0]
         else:
-            pixiv_sql_dialect = ""
-
+            pixiv_sql_dialect = url.scheme
         values["pixiv_sql_dialect"] = pixiv_sql_dialect
 
         return values
 
     pixiv_proxy: Optional[str]
     pixiv_query_timeout: float = 60.0
     pixiv_loading_prompt_delayed_time: float = 5.0
@@ -125,14 +103,17 @@
             raise ValueError(
                 f'pixiv_compression_enabled is True but {field.name} got None.')
         return v
 
     pixiv_query_to_me_only = False
     pixiv_command_to_me_only = False
 
+    pixiv_send_illust_link: bool = False
+    pixiv_send_forward_message: Literal['always', 'auto', 'never'] = 'auto'
+
     pixiv_max_item_per_query = 10
 
     pixiv_tag_translation_enabled = True
 
     pixiv_more_enabled = True
     pixiv_query_expires_in = 10 * 60
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/context.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/context.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/local_tag/mongo.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/local_tag.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,74 +1,73 @@
 from typing import Optional, Collection
 
-from beanie.odm.operators.update.general import SetOnInsert
 from nonebot import logger
-from pymongo import *
+from sqlalchemy import select
+from sqlalchemy.orm import mapped_column, Mapped
 
-from nonebot_plugin_pixivbot.global_context import context
-from nonebot_plugin_pixivbot.model import Tag, Illust
-from .base import LocalTagRepo
-from ..source.mongo import MongoDataSource, MongoDocument
+from .source.sql import DataSource
+from .utils.sql import insert
+from ..global_context import context
+from ..model import Tag, Illust
 
 
-class LocalTag(Tag, MongoDocument):
-    class Settings:
-        name = "local_tags"
-        indexes = [
-            IndexModel([("name", 1)], unique=True),
-            IndexModel([("translated_name", 1)])
-        ]
+@DataSource.registry.mapped
+class LocalTag:
+    __tablename__ = "local_tag"
 
+    name: Mapped[str] = mapped_column(primary_key=True)
+    translated_name: Mapped[str] = mapped_column(index=True)
 
-data_source = context.require(MongoDataSource)
+
+data_source = context.require(DataSource)
 
 
 @context.register_singleton()
-class MongoLocalTagRepo(LocalTagRepo):
+class LocalTagRepo:
 
     async def find_by_name(self, name: str) -> Optional[Tag]:
         async with data_source.start_session() as session:
-            result = await LocalTag.find_one(LocalTag.name == name, session=session)
-            return result
+            stmt = select(LocalTag).where(LocalTag.name == name).limit(1)
+            local_tag = (await session.execute(stmt)).scalar_one_or_none()
+            if local_tag is not None:
+                return Tag.from_orm(local_tag)
+            else:
+                return None
 
     async def find_by_translated_name(self, translated_name: str) -> Optional[Tag]:
         async with data_source.start_session() as session:
-            result = await LocalTag.find_one(LocalTag.translated_name == translated_name, session=session)
-            return result
+            stmt = select(LocalTag).where(LocalTag.translated_name == translated_name).limit(1)
+            local_tag = (await session.execute(stmt)).scalar_one_or_none()
+            if local_tag is not None:
+                return Tag.from_orm(local_tag)
+            else:
+                return None
 
     async def update_one(self, tag: Tag):
-        async with data_source.start_session() as session:
-            await LocalTag.find_one(LocalTag.name == tag.name, session=session).upsert(
-                SetOnInsert({LocalTag.translated_name: tag.translated_name}),
-                on_insert=LocalTag(**tag.dict()),
-                session=session
-            )
+        await self.update_many([tag])
 
     async def update_many(self, tags: Collection[Tag]):
-        async with data_source.start_session() as session:
-            # BulkWriter存在bug，upsert不生效
-            # https://github.com/roman-right/beanie/issues/224
+        if len(tags) == 0:
+            return
 
-            opt = []
-
-            for tag in tags:
-                opt.append(UpdateOne(
-                    {"name": tag.name},
-                    {"$setOnInsert": {"translated_name": tag.translated_name}},
-                    upsert=True
-                ))
-
-            if len(opt) != 0:
-                await LocalTag.get_motor_collection().bulk_write(opt, ordered=False, session=session)
-                logger.debug(f"[local_tag_repo] added {len(tags)} local tags")
+        async with data_source.start_session() as session:
+            stmt = insert(LocalTag).values([t.dict() for t in tags])
+            stmt = stmt.on_conflict_do_update(index_elements=[LocalTag.name],
+                                              set_={
+                                                  LocalTag.translated_name: stmt.excluded.translated_name
+                                              })
+
+            await session.execute(stmt)
+            await session.commit()
+            logger.debug(f"[local_tag_repo] added {len(tags)} local tags")
 
     async def update_from_illusts(self, illusts: Collection[Illust]):
         tags = {}
         for x in illusts:
             for t in x.tags:
                 if t.translated_name:
                     tags[t.name] = t
 
         await self.update_many(tags.values())
 
 
-__all__ = ("MongoLocalTagRepo",)
+__all__ = ("LocalTagRepo",)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_binding/sql.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_binding.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,65 +1,64 @@
 from typing import Optional
 
 from sqlalchemy import select, delete
 from sqlalchemy.orm import Mapped, mapped_column
 
-from nonebot_plugin_pixivbot.data.source.sql import SqlDataSource
-from nonebot_plugin_pixivbot.data.utils.sql import insert
-from nonebot_plugin_pixivbot.global_context import context
-from nonebot_plugin_pixivbot.model import PixivBinding, T_UID
-from .base import PixivBindingRepo
+from .source.sql import DataSource
+from .utils.sql import insert
+from ..global_context import context
+from ..model import PixivBinding
 
 
-@SqlDataSource.registry.mapped
+@DataSource.registry.mapped
 class PixivBindingOrm:
     __tablename__ = "pixiv_binding"
 
-    adapter: Mapped[str] = mapped_column(primary_key=True)
+    platform: Mapped[str] = mapped_column(primary_key=True)
     user_id: Mapped[str] = mapped_column(primary_key=True)
     pixiv_user_id: Mapped[int]
 
 
-data_source = context.require(SqlDataSource)
+data_source = context.require(DataSource)
 
 
 @context.register_singleton()
-class SqlPixivBindingRepo(PixivBindingRepo):
+class PixivBindingRepo:
 
-    async def get(self, adapter: str, user_id: T_UID) -> Optional[PixivBinding]:
+    async def get(self, platform: str, user_id: str) -> Optional[PixivBinding]:
         async with data_source.start_session() as session:
             stmt = (select(PixivBindingOrm)
-                    .where(PixivBindingOrm.adapter == adapter,
-                           PixivBindingOrm.user_id == str(user_id))
+                    .where(PixivBindingOrm.platform == platform,
+                           PixivBindingOrm.user_id == user_id)
                     .limit(1))
             result = (await session.execute(stmt)).scalar_one_or_none()
             if result is not None:
-                return PixivBinding(adapter=result.adapter,
-                                    user_id=type(user_id)(result.user_id),
+                return PixivBinding(platform=result.platform,
+                                    user_id=result.user_id,
                                     pixiv_user_id=result.pixiv_user_id)
             else:
                 return None
 
-    async def update(self, binding: PixivBinding[T_UID]):
+    async def update(self, binding: PixivBinding):
         async with data_source.start_session() as session:
             stmt = (insert(PixivBindingOrm)
-                    .values(adapter=binding.adapter,
-                            user_id=str(binding.user_id),
+                    .values(platform=binding.platform,
+                            user_id=binding.user_id,
                             pixiv_user_id=binding.pixiv_user_id)
-                    .on_conflict_do_update(index_elements=[PixivBindingOrm.adapter, PixivBindingOrm.user_id],
+                    .on_conflict_do_update(index_elements=[PixivBindingOrm.platform, PixivBindingOrm.user_id],
                                            set_={
                                                PixivBindingOrm.pixiv_user_id: binding.pixiv_user_id
                                            }))
             await session.execute(stmt)
             await session.commit()
 
-    async def remove(self, adapter: str, user_id: T_UID) -> bool:
+    async def remove(self, platform: str, user_id: str) -> bool:
         async with data_source.start_session() as session:
-            stmt = (delete(PixivBinding)
-                    .where(PixivBindingOrm.adapter == adapter,
-                           PixivBindingOrm.user_id == str(user_id)))
+            stmt = (delete(PixivBindingOrm)
+                    .where(PixivBindingOrm.platform == platform,
+                           PixivBindingOrm.user_id == user_id))
             result = await session.execute(stmt)
             await session.commit()
             return result.rowcount == 1
 
 
-__all__ = ("SqlPixivBindingRepo",)
+__all__ = ("PixivBindingRepo",)
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/base.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/compressor.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/compressor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/lazy_illust.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/lazy_illust.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/base.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/dummy.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/dummy.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/mongo.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,673 +1,690 @@
-from datetime import datetime, timedelta, timezone
-from typing import List, Union, Sequence, Any, AsyncGenerator, Optional, Type, Mapping
+from datetime import datetime, timezone, timedelta
+from functools import partial
+from typing import AsyncGenerator, Union, Optional, List
 
-import bson
-from beanie.odm.operators.find.comparison import In
-from beanie.odm.operators.find.logical import And
-from beanie.odm.operators.update.array import AddToSet, Pull, Push
-from beanie.odm.operators.update.general import Set
+from apscheduler.triggers.interval import IntervalTrigger
 from nonebot import logger
-from pymongo import UpdateOne
-from pymongo.client_session import ClientSession
+from nonebot_plugin_apscheduler import scheduler as apscheduler
+from sqlalchemy import select, delete, func, text
+from sqlalchemy.ext.asyncio import AsyncSession
 
-from nonebot_plugin_pixivbot.config import Config
-from nonebot_plugin_pixivbot.enums import RankingMode
-from nonebot_plugin_pixivbot.global_context import context
-from nonebot_plugin_pixivbot.model import Illust, User
 from .base import LocalPixivRepo
-from .mongo_models import UserDetailCache, PixivRepoCache, IllustDetailCache, IllustSetCache, UserSetCache, \
-    SearchIllustCache, SearchUserCache, UserIllustsCache, UserBookmarksCache, OtherIllustCache, RelatedIllustsCache, \
-    IllustRankingCache, DownloadCache
+from .sql_models import IllustDetailCache, UserDetailCache, DownloadCache, IllustSetCache, IllustSetCacheIllust, \
+    UserSetCache, UserSetCacheUser
 from ..errors import CacheExpiredError, NoSuchItemError
 from ..lazy_illust import LazyIllust
 from ..models import PixivRepoMetadata
 from ...local_tag import LocalTagRepo
-from ...source.mongo import MongoDataSource
+from ...source.sql import DataSource
+from ...utils.sql import insert
+from ....config import Config
+from ....enums import RankingMode
+from ....global_context import context
+from ....model import Illust, User
+from ....utils.lifecycler import on_startup
 
 
 def _handle_expires_in(metadata: PixivRepoMetadata, expires_in: int):
     if datetime.now(timezone.utc) - metadata.update_time >= timedelta(seconds=expires_in):
         raise CacheExpiredError(metadata)
 
 
+def _extract_metadata(cache, is_set_cache):
+    update_time = cache.update_time.replace(tzinfo=timezone.utc)
+
+    if is_set_cache:
+        metadata = PixivRepoMetadata(update_time=update_time, pages=cache.pages, next_qs=cache.next_qs)
+    else:
+        metadata = PixivRepoMetadata(update_time=update_time)
+    return metadata
+
+
 conf = context.require(Config)
-data_source = context.require(MongoDataSource)
+data_source = context.require(DataSource)
 local_tags = context.require(LocalTagRepo)
 
 
 @context.register_singleton()
-class MongoPixivRepo(LocalPixivRepo):
+class SqlPixivRepo(LocalPixivRepo):
 
-    async def _add_to_local_tags(self, illusts: List[Union[LazyIllust, Illust]]):
-        li = []
-        for x in illusts:
-            if isinstance(x, LazyIllust):
-                if not x.loaded:
-                    continue
-                x = x.content
-            li.append(x)
+    def __init__(self):
+        on_startup(replay=True)(
+            partial(
+                apscheduler.add_job,
+                self.clean_expired,
+                id='pixivbot_sql_pixiv_repo_clean_expired',
+                trigger=IntervalTrigger(hours=2),
+                max_instances=1
+            )
+        )
 
-        await local_tags.update_from_illusts(li)
+    async def _get_illusts(self, session: AsyncSession,
+                           cache_type: str,
+                           key: dict,
+                           expired_in: int,
+                           offset: int = 0, ):
+        stmt = (select(IllustSetCache)
+                .where(IllustSetCache.cache_type == cache_type,
+                       IllustSetCache.key == key))
+        cache: Optional[IllustSetCache] = (await session.execute(stmt)).scalar_one_or_none()
+        if cache is None:
+            raise NoSuchItemError()
 
-    async def _illusts_agen(self, session: ClientSession,
-                            doc_type: Type[PixivRepoCache],
-                            *criteria: Union[Mapping[str, Any], bool],
-                            offset: int = 0) -> AsyncGenerator[LazyIllust, None]:
-        aggregation = [
-            {
-                "$match": And(*criteria).query
-            },
-            {
-                "$replaceWith": {"illust_id": "$illust_id"}
-            },
-            {
-                "$unwind": "$illust_id"
-            },
-        ]
-
-        if offset:
-            aggregation.append({"$offset": offset})
-
-        aggregation.extend([
-            {
-                "$lookup": {
-                    "from": IllustDetailCache.Settings.name,
-                    "localField": "illust_id",
-                    "foreignField": "illust.id",
-                    "as": "illusts"
-                }
-            },
-            {
-                "$replaceWith": {
-                    "$mergeObjects": [
-                        "$$ROOT",
-                        {"$arrayElemAt": ["$illusts", 0]}
-                    ]
-                }
-            },
-            {
-                "$project": {"_id": 0, "illust": 1, "illust_id": 1}
-            }
-        ])
+        metadata = _extract_metadata(cache, True)
+        _handle_expires_in(metadata, expired_in)
+
+        yield metadata.copy(update={"pages": 0})
+
+        stmt = (select(IllustSetCacheIllust, IllustDetailCache)
+                .where(IllustSetCacheIllust.cache_id == cache.id)
+                .outerjoin(IllustDetailCache, IllustSetCacheIllust.illust_id == IllustDetailCache.illust_id)
+                .order_by(IllustSetCacheIllust.rank, IllustDetailCache.update_time.desc())
+                .offset(offset))
 
         total = 0
         broken = 0
 
         try:
-            # noinspection PyTypeChecker
-            async for x in doc_type.aggregate(aggregation, session=session):
+            async for cache_illust, illust in await session.stream(stmt):
+                cache_illust: IllustSetCacheIllust
+                illust: Optional[IllustDetailCache]
+
                 total += 1
-                if "illust" in x and x["illust"] is not None:
-                    yield LazyIllust(x["illust_id"], Illust.parse_obj(x["illust"]))
+
+                if illust is not None:
+                    yield LazyIllust(illust.illust_id, Illust(**illust.illust))
                 else:
-                    yield LazyIllust(x["illust_id"])
+                    yield LazyIllust(cache_illust.illust_id)
                     broken += 1
         finally:
             logger.debug(f"[local] got {total} illusts, illust_detail of {broken} are missed")
 
-    async def _users_agen(self, session: ClientSession,
-                          doc_type: Type[PixivRepoCache],
-                          *criteria: Union[Mapping[str, Any], bool],
-                          offset: int = 0) -> AsyncGenerator[User, None]:
-        aggregation = [
-            {
-                "$match": And(*criteria).query
-            },
-            {
-                "$replaceWith": {"user_id": "$user_id"}
-            },
-            {
-                "$unwind": "$user_id"
-            },
-        ]
-
-        if offset:
-            aggregation.append({"$offset": offset})
-
-        aggregation.extend([
-            {
-                "$lookup": {
-                    "from": UserDetailCache.Settings.name,
-                    "localField": "user_id",
-                    "foreignField": "user.id",
-                    "as": "users"
-                }
-            },
-            {
-                "$replaceWith": {
-                    "$mergeObjects": [
-                        "$$ROOT",
-                        {"$arrayElemAt": ["$users", 0]}
-                    ]
+        yield metadata
+
+    async def _invalidate_illusts(self, session: AsyncSession,
+                                  cache_type: str,
+                                  key: dict):
+        if conf.pixiv_sql_dialect == 'sqlite':
+            await session.execute(text("PRAGMA foreign_keys = ON;"))
+
+        stmt = (delete(IllustSetCache)
+                .where(IllustSetCache.cache_type == cache_type,
+                       IllustSetCache.key == key))
+        await session.execute(stmt)
+        await session.commit()
+
+    async def _append_and_check_illusts(self, session: AsyncSession,
+                                        cache_type: str,
+                                        key: dict,
+                                        content: List[Union[Illust, LazyIllust]],
+                                        metadata: PixivRepoMetadata,
+                                        append_at_begin: bool = False):
+        async with session.begin_nested() as tx1:
+            async with session.begin_nested() as tx2:
+                stmt = (select(IllustSetCache)
+                        .where(IllustSetCache.cache_type == cache_type,
+                               IllustSetCache.key == key)
+                        .limit(1))
+                cache = (await session.execute(stmt)).scalar_one_or_none()
+                if cache is None:
+                    cache = IllustSetCache(cache_type=cache_type, key=key)
+                    session.add(cache)
+
+                cache.update_time = metadata.update_time
+                cache.next_qs = metadata.next_qs
+                cache.pages = metadata.pages
+
+                # commit to get cache id
+                await tx2.commit()
+
+            row_count = 0
+            if append_at_begin:
+                stmt = select(
+                    func.min(IllustSetCacheIllust.rank)
+                ).select_from(IllustSetCacheIllust).where(
+                    IllustSetCacheIllust.cache_id == cache.id
+                )
+
+                rnk = (await session.execute(stmt)).scalar_one_or_none()
+                if rnk is None:
+                    rnk = 0
+
+                for x in reversed(content):
+                    stmt = insert(IllustSetCacheIllust).values(
+                        cache_id=cache.id, illust_id=x.id, rank=rnk - 1
+                    ).on_conflict_do_nothing(index_elements=[
+                        IllustSetCacheIllust.cache_id, IllustSetCacheIllust.illust_id
+                    ])
+                    result = await session.execute(stmt)
+                    row_count += result.rowcount
+                    rnk -= result.rowcount
+            else:
+                stmt = select(
+                    func.max(IllustSetCacheIllust.rank)
+                ).select_from(IllustSetCacheIllust).where(
+                    IllustSetCacheIllust.cache_id == cache.id
+                )
+
+                rnk = (await session.execute(stmt)).scalar_one_or_none()
+                if rnk is None:
+                    rnk = 0
+
+                for x in content:
+                    stmt = insert(IllustSetCacheIllust).values(
+                        cache_id=cache.id, illust_id=x.id, rank=rnk + 1
+                    ).on_conflict_do_nothing(index_elements=[
+                        IllustSetCacheIllust.cache_id, IllustSetCacheIllust.illust_id
+                    ])
+                    result = await session.execute(stmt)
+                    row_count += result.rowcount
+                    rnk += result.rowcount
+
+            cache.size += row_count
+
+            await tx1.commit()
+
+        # insert illust detail
+        for x in content:
+            if isinstance(x, LazyIllust):
+                if not x.loaded:
+                    continue
+                x = x.content
+
+            stmt = insert(IllustDetailCache).values(
+                illust_id=x.id, illust=x.dict(), update_time=metadata.update_time
+            )
+            stmt = stmt.on_conflict_do_update(
+                index_elements=[IllustDetailCache.illust_id],
+                set_={
+                    IllustDetailCache.illust: stmt.excluded.illust,
+                    IllustDetailCache.update_time: stmt.excluded.update_time
                 }
-            },
-            {
-                "$project": {"_id": 0, "user": 1, "user_id": 1}
-            }
-        ])
+            )
+            await session.execute(stmt)
 
-        total = 0
-        try:
-            # noinspection PyTypeChecker
-            async for x in doc_type.aggregate(aggregation, session=session):
-                if "user" in x and x["user"] is not None:
-                    yield User.parse_obj(x["user"])
-                else:
-                    yield User(id=x["user_id"], name="", account="")
-                total += 1
-        finally:
-            logger.debug(f"[local] got {total} users")
+        await session.commit()
 
-    async def _get_illusts(self, session: ClientSession,
-                           doc_type: Type[PixivRepoCache],
-                           *criteria: Union[Mapping[str, Any], bool],
-                           expired_in: int,
-                           offset: int = 0) \
-            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], Any]:
-        doc: Optional[PixivRepoCache] = await doc_type.find_one(*criteria, session=session)
-        if not doc:
-            raise NoSuchItemError()
-        _handle_expires_in(doc.metadata, expired_in)
+        # insert local tags
+        li = []
+        for x in content:
+            if isinstance(x, LazyIllust):
+                if not x.loaded:
+                    continue
+                x = x.content
+            li.append(x)
+        await local_tags.update_from_illusts(li)
 
-        metadata = doc.metadata
-        yield metadata.copy(update={"pages": 0})
-        async for x in self._illusts_agen(session, doc_type, *criteria, offset=offset):
-            yield x
-        yield metadata
+        return row_count != len(content)
 
-    async def _get_users(self, session: ClientSession,
-                         doc_type: Type[PixivRepoCache],
-                         *criteria: Union[Mapping[str, Any], bool],
+    async def _get_users(self, session: AsyncSession,
+                         cache_type: str,
+                         key: dict,
                          expired_in: int,
-                         offset: int = 0) \
-            -> AsyncGenerator[Union[User, PixivRepoMetadata], Any]:
-        doc: Optional[PixivRepoCache] = await doc_type.find_one(*criteria, session=session)
-        if not doc:
+                         offset: int = 0):
+        stmt = (select(UserSetCache)
+                .where(UserSetCache.cache_type == cache_type,
+                       UserSetCache.key == key))
+        cache = (await session.execute(stmt)).scalar_one_or_none()
+        if cache is None:
             raise NoSuchItemError()
-        _handle_expires_in(doc.metadata, expired_in)
 
-        metadata = doc.metadata
+        metadata = _extract_metadata(cache, True)
+        _handle_expires_in(metadata, expired_in)
+
         yield metadata.copy(update={"pages": 0})
-        async for x in self._users_agen(session, doc_type, *criteria, offset=offset):
-            yield x
+
+        stmt = (select(UserSetCacheUser, UserDetailCache)
+                .where(UserSetCacheUser.cache_id == cache.id)
+                .outerjoin(UserDetailCache, UserSetCacheUser.user_id == UserDetailCache.user_id)
+                .offset(offset))
+
+        total = 0
+        try:
+            async for cache_user, user in await session.stream(stmt):
+                if user is not None:
+                    yield User(**user.user)
+                else:
+                    yield User(id=cache_user.user_id, name="", account="")
+                total += 1
+        finally:
+            logger.debug(f"[local] got {total} users")
+
         yield metadata
 
-    async def _check_illusts_exists(self, session: ClientSession,
-                                    doc_type: Type[IllustSetCache],
-                                    *criteria: Union[Mapping[str, Any], bool],
-                                    illust_id: Union[int, Sequence[int]]) -> bool:
-        if isinstance(illust_id, int):
-            return await doc_type.find(*criteria, In(doc_type.illust_id, illust_id),
-                                       session=session).count() != 0
-        else:
-            agg = [
-                {'$match': And(*criteria).query},
-                {'$unwind': {'path': '$illust_id'}},
-                {'$match': {'illust_id': {'$in': illust_id}}},
-                {'$count': 'count'}
-            ]
-
-            # noinspection PyTypeChecker
-            async for result in doc_type.aggregate(agg):
-                return result["count"] != 0
-
-    async def _check_users_exists(self, session: ClientSession,
-                                  doc_type: Type[UserSetCache],
-                                  *criteria: Union[Mapping[str, Any], bool],
-                                  user_id: Union[int, Sequence[int]]) -> bool:
-        if isinstance(user_id, int):
-            return await doc_type.find(*criteria, In(doc_type.user_id, user_id),
-                                       session=session).count() != 0
-        else:
-            agg = [
-                {'$match': And(*criteria).query},
-                {'$unwind': {'path': '$user_id'}},
-                {'$match': {'user_id': {'$in': user_id}}},
-                {'$count': 'count'}
-            ]
-
-            # noinspection PyTypeChecker
-            async for result in doc_type.aggregate(agg, session=session):
-                return result["count"] != 0
-
-    async def _update_illusts(self, session: ClientSession,
-                              doc_type: Type[IllustSetCache],
-                              *criteria: Union[Mapping[str, Any], bool],
-                              content: List[Union[Illust, LazyIllust]],
-                              metadata: PixivRepoMetadata,
-                              append_at_begin: bool = False):
-        if append_at_begin:
-            await doc_type.find_one(*criteria, session=session).update(
-                Set({
-                    doc_type.metadata: metadata
-                }),
-                Pull({
-                    doc_type.illust_id: {
-                        "$in": [illust.id for illust in content]
-                    }
-                }),
-                upsert=True,
-                session=session
-            )
-            await doc_type.find_one(*criteria, session=session).update(
-                Push({
-                    doc_type.illust_id: {
-                        "$each": [illust.id for illust in content],
-                        "$position": 0
-                    }
-                }),
-                session=session
-            )
-        else:
-            await doc_type.find_one(*criteria, session=session).update(
-                Set({
-                    doc_type.metadata: metadata
-                }),
-                AddToSet({
-                    doc_type.illust_id: {
-                        "$each": [illust.id for illust in content]
-                    }
-                }),
-                upsert=True,
-                session=session
-            )
-
-        # BulkWriter存在bug，upsert不生效
-        # https://github.com/roman-right/beanie/issues/224
-
-        opt = []
-        for illust in content:
-            if isinstance(illust, LazyIllust) and illust.content is not None:
-                illust = illust.content
-
-            if isinstance(illust, Illust):
-                opt.append(UpdateOne(
-                    {"illust.id": illust.id},
-                    {"$set": {
-                        "illust": illust.dict(exclude_none=True),
-                        "metadata": {"update_time": metadata.update_time}
-                    }},
-                    upsert=True
-                ))
-        if len(opt) != 0:
-            await IllustDetailCache.get_motor_collection().bulk_write(opt, ordered=False, session=session)
-
-        if conf.pixiv_tag_translation_enabled:
-            await self._add_to_local_tags(content)
-
-    async def _update_users(self, session: ClientSession,
-                            doc_type: Type[UserSetCache],
-                            *criteria: Union[Mapping[str, Any], bool],
-                            content: List[User],
-                            metadata: PixivRepoMetadata,
-                            append: bool = False):
-        if append:
-            await doc_type.find_one(*criteria, session=session).update(
-                Set({
-                    doc_type.metadata: metadata
-                }),
-                AddToSet({
-                    doc_type.user_id: {
-                        "$each": [user.id for user in content]
-                    }
-                }),
-                upsert=True,
-                session=session
-            )
-        else:
-            await doc_type.find_one(*criteria, session=session).update(
-                Set({
-                    doc_type.user_id: [user.id for user in content],
-                    doc_type.metadata: metadata
-                }),
-                upsert=True,
-                session=session
-            )
-        # BulkWriter存在bug，upsert不生效
-        # https://github.com/roman-right/beanie/issues/224
-        #
-        # async with BulkWriter() as bw:
-        #     user_metadata = PixivRepoMetadata(update_time=metadata.update_time)
-        #
-        #     for user in content:
-        #         await UserDetailCache.find_one(
-        #             UserDetailCache.user.id == user.id
-        #         ).upsert(
-        #             Set({
-        #                 UserDetailCache.user: user,
-        #                 UserDetailCache.metadata: user_metadata
-        #             }),
-        #             on_insert=UserDetailCache(user=user, metadata=user_metadata),
-        #             bulk_writer=bw
-        #         )
-
-        opt = []
-        for user in content:
-            opt.append(UpdateOne(
-                {"user.id": user.id},
-                {"$set": {
-                    "user": user.dict(exclude_none=True),
-                    "metadata": {"update_time": metadata.update_time}
-                }},
-                upsert=True
-            ))
-        if len(opt) != 0:
-            await data_source.db.user_detail_cache.bulk_write(opt, ordered=False, session=session)
-
-    async def _append_and_check_illusts(self, session: ClientSession,
-                                        doc_type: Type[IllustSetCache],
-                                        *criteria: Union[Mapping[str, Any], bool],
-                                        content: List[Union[Illust, LazyIllust]],
-                                        metadata: PixivRepoMetadata,
-                                        append_at_begin: bool = False):
-        exists = await self._check_illusts_exists(session, doc_type, *criteria, illust_id=[x.id for x in content])
-        await self._update_illusts(session, doc_type, *criteria, content=content, metadata=metadata,
-                                   append_at_begin=append_at_begin)
-        return exists
-
-    async def _append_and_check_users(self, session: ClientSession,
-                                      doc_type: Type[UserSetCache],
-                                      *criteria: Union[Mapping[str, Any], bool],
+    async def _invalidate_users(self, session: AsyncSession,
+                                cache_type: str,
+                                key: dict):
+        if conf.pixiv_sql_dialect == 'sqlite':
+            await session.execute(text("PRAGMA foreign_keys = ON;"))
+
+        stmt = (delete(UserSetCache)
+                .where(UserSetCache.cache_type == cache_type,
+                       UserSetCache.key == key))
+        await session.execute(stmt)
+        await session.commit()
+
+    async def _append_and_check_users(self, session: AsyncSession,
+                                      cache_type: str,
+                                      key: dict,
                                       content: List[User],
                                       metadata: PixivRepoMetadata):
-        exists = await self._check_users_exists(session, doc_type, *criteria, user_id=[x.id for x in content])
-        await self._update_users(session, doc_type, *criteria, content=content, metadata=metadata, append=True)
-        return exists
+
+        async with session.begin_nested() as tx1:
+            async with session.begin_nested() as tx2:
+                stmt = (select(UserSetCache)
+                        .where(UserSetCache.cache_type == cache_type,
+                               UserSetCache.key == key)
+                        .limit(1))
+                cache = (await session.execute(stmt)).scalar_one_or_none()
+                if cache is None:
+                    cache = UserSetCache(cache_type=cache_type, key=key)
+                    session.add(cache)
+
+                cache.update_time = metadata.update_time
+                cache.next_qs = metadata.next_qs
+                cache.pages = metadata.pages
+
+                # commit to get cache id
+                await tx2.commit()
+
+            row_count = 0
+            for x in content:
+                stmt = insert(UserSetCacheUser).values(
+                    cache_id=cache.id, user_id=x.id
+                ).on_conflict_do_nothing(index_elements=[
+                    UserSetCacheUser.cache_id, UserSetCacheUser.user_id
+                ])
+                row_count += (await session.execute(stmt)).rowcount
+
+            await tx1.commit()
+
+        # insert user detail
+        for x in content:
+            stmt = insert(UserDetailCache).values(
+                user_id=x.id, user=x.dict(), update_time=metadata.update_time
+            )
+            stmt = stmt.on_conflict_do_update(
+                index_elements=[UserDetailCache.user_id],
+                set_={
+                    UserDetailCache.user: stmt.excluded.user,
+                    UserDetailCache.update_time: stmt.excluded.update_time
+                }
+            )
+            await session.execute(stmt)
+            await session.commit()
+
+        return row_count != len(content)
 
     # ================ illust_detail ================
     async def illust_detail(self, illust_id: int) \
             -> AsyncGenerator[Union[Illust, PixivRepoMetadata], None]:
         logger.debug(f"[local] illust_detail {illust_id}")
+
         async with data_source.start_session() as session:
-            doc = await IllustDetailCache.find_one(IllustDetailCache.illust.id == illust_id, session=session)
-            if doc is not None:
-                _handle_expires_in(doc.metadata, conf.pixiv_illust_detail_cache_expires_in)
+            stmt = select(IllustDetailCache).where(IllustDetailCache.illust_id == illust_id).limit(1)
+            cache = (await session.execute(stmt)).scalar_one_or_none()
+
+            if cache is not None:
+                metadata = _extract_metadata(cache, False)
+                _handle_expires_in(metadata, conf.pixiv_illust_detail_cache_expires_in)
 
-                yield doc.metadata
-                yield doc.illust
+                yield metadata
+                yield Illust(**cache.illust)
             else:
                 raise NoSuchItemError()
 
     async def update_illust_detail(self, illust: Illust, metadata: PixivRepoMetadata):
         logger.debug(f"[local] update illust_detail {illust.id} {metadata}")
 
         async with data_source.start_session() as session:
-            await IllustDetailCache.find_one(
-                IllustDetailCache.illust.id == illust.id,
-                session=session
-            ).update(
-                Set({
-                    IllustDetailCache.illust: illust,
-                    IllustDetailCache.metadata: metadata
-                }),
-                upsert=True,
-                session=session
-            )
+            stmt = (insert(IllustDetailCache)
+                    .values(illust_id=illust.id, illust=illust.dict(), update_time=metadata.update_time))
+            stmt = stmt.on_conflict_do_update(index_elements=[IllustDetailCache.illust_id],
+                                              set_={
+                                                  IllustDetailCache.illust: stmt.excluded.illust,
+                                                  IllustDetailCache.update_time: stmt.excluded.update_time
+                                              })
+
+            await session.execute(stmt)
+            await session.commit()
 
             if conf.pixiv_tag_translation_enabled:
-                await self._add_to_local_tags([illust])
+                await local_tags.update_from_illusts([illust])
 
     # ================ user_detail ================
     async def user_detail(self, user_id: int) \
             -> AsyncGenerator[Union[User, PixivRepoMetadata], None]:
         logger.debug(f"[local] user_detail {user_id}")
+
         async with data_source.start_session() as session:
-            doc: Optional[UserDetailCache] = await UserDetailCache.find_one(UserDetailCache.user.id == user_id,
-                                                                            session=session)
-            if doc is not None:
-                _handle_expires_in(doc.metadata, conf.pixiv_user_detail_cache_expires_in)
+            stmt = select(UserDetailCache).where(UserDetailCache.user_id == user_id).limit(1)
+            cache = (await session.execute(stmt)).scalar_one_or_none()
+
+            if cache is not None:
+                metadata = _extract_metadata(cache, False)
+                _handle_expires_in(metadata, conf.pixiv_user_detail_cache_expires_in)
 
-                yield doc.metadata
-                yield doc.user
+                yield metadata
+                yield User(**cache.user)
             else:
                 raise NoSuchItemError()
 
     async def update_user_detail(self, user: User, metadata: PixivRepoMetadata):
         logger.debug(f"[local] update user_detail {user.id} {metadata}")
 
         async with data_source.start_session() as session:
-            if not metadata:
-                metadata = PixivRepoMetadata(update_time=datetime.now(timezone.utc))
+            stmt = (insert(UserDetailCache)
+                    .values(user_id=user.id, user=user.dict(), update_time=metadata.update_time))
+            stmt = stmt.on_conflict_do_update(index_elements=[UserDetailCache.user_id],
+                                              set_={
+                                                  UserDetailCache.user: stmt.excluded.user,
+                                                  UserDetailCache.update_time: stmt.excluded.update_time
+                                              })
 
-            await UserDetailCache.find_one(
-                UserDetailCache.user.id == user.id,
-                session=session
-            ).update(
-                Set({
-                    UserDetailCache.user: user,
-                    UserDetailCache.metadata: metadata
-                }),
-                upsert=True,
-                session=session
-            )
+            await session.execute(stmt)
+            await session.commit()
+
+    # ================ image ================
+    async def image(self, illust: Illust, page: int = 0) -> AsyncGenerator[Union[bytes, PixivRepoMetadata], None]:
+        logger.debug(f"[local] image {illust.id}")
+
+        async with data_source.start_session() as session:
+            stmt = select(DownloadCache).where(DownloadCache.illust_id == illust.id,
+                                               DownloadCache.page == page).limit(1)
+            cache = (await session.execute(stmt)).scalar_one_or_none()
+
+            if cache is not None:
+                metadata = _extract_metadata(cache, False)
+                _handle_expires_in(metadata, conf.pixiv_download_cache_expires_in)
+
+                yield metadata
+                yield cache.content
+            else:
+                raise NoSuchItemError()
+
+    async def update_image(self, illust_id: int, page: int,
+                           content: bytes, metadata: PixivRepoMetadata):
+        logger.debug(f"[local] update image {illust_id} {metadata}")
+
+        async with data_source.start_session() as session:
+            stmt = (insert(DownloadCache)
+                    .values(illust_id=illust_id, page=page, content=content, update_time=metadata.update_time))
+            stmt = stmt.on_conflict_do_update(index_elements=[DownloadCache.illust_id, DownloadCache.page],
+                                              set_={
+                                                  DownloadCache.content: stmt.excluded.content,
+                                                  DownloadCache.update_time: stmt.excluded.update_time
+                                              })
+
+            await session.execute(stmt)
+            await session.commit()
+
+    # ================ illust_ranking ================
+    async def illust_ranking(self, mode: Union[str, RankingMode], *, offset: int = 0) \
+            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
+        if isinstance(mode, str):
+            mode = RankingMode[mode]
+
+        logger.debug(f"[local] illust_ranking {mode}")
+
+        async with data_source.start_session() as session:
+            async for x in self._get_illusts(session, "illust_ranking", {"mode": mode},
+                                             expired_in=conf.pixiv_illust_ranking_cache_expires_in, offset=offset):
+                yield x
+
+    async def invalidate_illust_ranking(self, mode: RankingMode):
+        logger.debug(f"[local] invalidate illust_ranking")
+        async with data_source.start_session() as session:
+            await self._invalidate_illusts(session, "illust_ranking", {"mode": mode})
+
+    async def append_illust_ranking(self, mode: RankingMode, content: List[Union[Illust, LazyIllust]],
+                                    metadata: PixivRepoMetadata) -> bool:
+        logger.debug(f"[local] append illust_ranking {mode} "
+                     f"({len(content)} items) "
+                     f"{metadata}")
+        async with data_source.start_session() as session:
+            return await self._append_and_check_illusts(session, "illust_ranking", {"mode": mode},
+                                                        content=content, metadata=metadata)
 
     # ================ search_illust ================
     async def search_illust(self, word: str, *, offset: int = 0) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
         logger.debug(f"[local] search_illust {word}")
         async with data_source.start_session() as session:
-            async for x in self._get_illusts(session, SearchIllustCache, SearchIllustCache.word == word,
+            async for x in self._get_illusts(session, "search_illust", {"word": word},
                                              expired_in=conf.pixiv_search_illust_cache_expires_in, offset=offset):
                 yield x
 
     async def invalidate_search_illust(self, word: str):
         logger.debug(f"[local] invalidate search_illust {word}")
         async with data_source.start_session() as session:
-            await data_source.db.search_illust_cache.delete_one({"word": word}, session=session)
+            await self._invalidate_illusts(session, "search_illust", {"word": word})
 
     async def append_search_illust(self, word: str, content: List[Union[Illust, LazyIllust]],
                                    metadata: PixivRepoMetadata) -> bool:
         # 返回值表示content中是否有已经存在于集合的文档，下同
         logger.debug(f"[local] append search_illust {word} "
-                    f"({len(content)} items) "
-                    f"{metadata}")
+                     f"({len(content)} items) "
+                     f"{metadata}")
         async with data_source.start_session() as session:
-            return await self._append_and_check_illusts(session, SearchIllustCache, SearchIllustCache.word == word,
+            return await self._append_and_check_illusts(session, "search_illust", {"word": word},
                                                         content=content, metadata=metadata)
 
-    # ================ search_user ================
-    async def search_user(self, word: str, *, offset: int = 0) \
-            -> AsyncGenerator[Union[User, PixivRepoMetadata], None]:
-        logger.debug(f"[local] search_user {word}")
-        async with data_source.start_session() as session:
-            async for x in self._get_users(session, SearchUserCache, SearchUserCache.word == word,
-                                           expired_in=conf.pixiv_search_user_cache_expires_in, offset=offset):
-                yield x
-
-    async def invalidate_search_user(self, word: str):
-        logger.debug(f"[local] invalidate search_user {word}")
-        async with data_source.start_session() as session:
-            await SearchUserCache.find_one(SearchUserCache.word == word, session=session).delete()
-
-    async def append_search_user(self, word: str, content: List[User],
-                                 metadata: PixivRepoMetadata) -> bool:
-        logger.debug(f"[local] append search_user {word} "
-                    f"({len(content)} items) "
-                    f"{metadata}")
-        async with data_source.start_session() as session:
-            return await self._append_and_check_users(session, SearchUserCache, SearchUserCache.word == word,
-                                                      content=content, metadata=metadata)
-
     # ================ user_illusts ================
     async def user_illusts(self, user_id: int, *, offset: int = 0) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
         logger.debug(f"[local] user_illusts {user_id}")
         async with data_source.start_session() as session:
-            async for x in self._get_illusts(session, UserIllustsCache, UserIllustsCache.user_id == user_id,
+            async for x in self._get_illusts(session, "user_illusts", {"user_id": user_id},
                                              expired_in=conf.pixiv_user_illusts_cache_expires_in, offset=offset):
                 yield x
 
     async def invalidate_user_illusts(self, user_id: int):
         logger.debug(f"[local] invalidate user_illusts {user_id}")
         async with data_source.start_session() as session:
-            await UserIllustsCache.find_one(UserIllustsCache.user_id == user_id, session=session).delete()
+            await self._invalidate_illusts(session, "user_illusts", {"user_id": user_id})
 
     async def append_user_illusts(self, user_id: int,
                                   content: List[Union[Illust, LazyIllust]],
                                   metadata: PixivRepoMetadata,
                                   append_at_begin: bool = False) -> bool:
         logger.debug(f"[local] append user_illusts {user_id} "
-                    f"{'at begin ' if append_at_begin else ''}"
-                    f"({len(content)} items) "
-                    f"{metadata}")
+                     f"{'at begin ' if append_at_begin else ''}"
+                     f"({len(content)} items) "
+                     f"{metadata}")
         async with data_source.start_session() as session:
-            return await self._append_and_check_illusts(session, UserIllustsCache, UserIllustsCache.user_id == user_id,
+            return await self._append_and_check_illusts(session, "user_illusts", {"user_id": user_id},
                                                         content=content, metadata=metadata,
                                                         append_at_begin=append_at_begin)
 
     # ================ user_bookmarks ================
     async def user_bookmarks(self, user_id: int = 0, *, offset: int = 0) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
         logger.debug(f"[local] user_bookmarks {user_id}")
         async with data_source.start_session() as session:
-            async for x in self._get_illusts(session, UserBookmarksCache, UserBookmarksCache.user_id == user_id,
+            async for x in self._get_illusts(session, "user_bookmarks", {"user_id": user_id},
                                              expired_in=conf.pixiv_user_bookmarks_cache_expires_in, offset=offset):
                 yield x
 
     async def invalidate_user_bookmarks(self, user_id: int):
         logger.debug(f"[local] invalidate user_bookmarks {user_id}")
         async with data_source.start_session() as session:
-            await UserBookmarksCache.find_one(UserBookmarksCache.user_id == user_id, session=session).delete()
+            await self._invalidate_illusts(session, "user_bookmarks", {"user_id": user_id})
 
     async def append_user_bookmarks(self, user_id: int,
                                     content: List[Union[Illust, LazyIllust]],
                                     metadata: PixivRepoMetadata,
                                     append_at_begin: bool = False) -> bool:
         logger.debug(f"[local] append user_bookmarks {user_id} "
-                    f"{'at begin ' if append_at_begin else ''}"
-                    f"({len(content)} items) "
-                    f"{metadata}")
+                     f"{'at begin ' if append_at_begin else ''} "
+                     f"({len(content)} items) "
+                     f"{metadata}")
         async with data_source.start_session() as session:
-            return await self._append_and_check_illusts(session, UserBookmarksCache,
-                                                        UserBookmarksCache.user_id == user_id,
+            return await self._append_and_check_illusts(session, "user_bookmarks", {"user_id": user_id},
                                                         content=content, metadata=metadata,
                                                         append_at_begin=append_at_begin)
 
     # ================ recommended_illusts ================
     async def recommended_illusts(self, *, offset: int = 0) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
         logger.debug(f"[local] recommended_illusts")
         async with data_source.start_session() as session:
-            async for x in self._get_illusts(session, OtherIllustCache, OtherIllustCache.type == "recommended_illusts",
+            async for x in self._get_illusts(session, "other", {"type": "recommended_illusts"},
                                              expired_in=conf.pixiv_other_cache_expires_in, offset=offset):
                 yield x
 
     async def invalidate_recommended_illusts(self):
         logger.debug(f"[local] invalidate recommended_illusts")
         async with data_source.start_session() as session:
-            await OtherIllustCache.find_one(OtherIllustCache.type == "recommended_illusts",
-                                            session=session).delete()
+            await self._invalidate_illusts(session, "other", {"type": "recommended_illusts"})
 
     async def append_recommended_illusts(self, content: List[Union[Illust, LazyIllust]],
                                          metadata: PixivRepoMetadata) -> bool:
         logger.debug(f"[local] append recommended_illusts "
-                    f"({len(content)} items) "
-                    f"{metadata}")
+                     f"({len(content)} items) "
+                     f"{metadata}")
         async with data_source.start_session() as session:
-            return await self._append_and_check_illusts(session, OtherIllustCache,
-                                                        OtherIllustCache.type == "recommended_illusts",
+            return await self._append_and_check_illusts(session, "other", {"type": "recommended_illusts"},
                                                         content=content, metadata=metadata)
 
     # ================ related_illusts ================
     async def related_illusts(self, illust_id: int, *, offset: int = 0) \
             -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
         logger.debug(f"[local] related_illusts {illust_id}")
         async with data_source.start_session() as session:
-            async for x in self._get_illusts(session, RelatedIllustsCache,
-                                             RelatedIllustsCache.original_illust_id == illust_id,
+            async for x in self._get_illusts(session, "related_illusts", {"original_illust_id": illust_id},
                                              expired_in=conf.pixiv_related_illusts_cache_expires_in,
                                              offset=offset):
                 yield x
 
     async def invalidate_related_illusts(self, illust_id: int):
         logger.debug(f"[local] invalidate related_illusts")
         async with data_source.start_session() as session:
-            await RelatedIllustsCache.find_one(RelatedIllustsCache.original_illust_id == illust_id,
-                                               session=session).delete()
+            await self._invalidate_illusts(session, "related_illusts", {"original_illust_id": illust_id})
 
     async def append_related_illusts(self, illust_id: int, content: List[Union[Illust, LazyIllust]],
                                      metadata: PixivRepoMetadata) -> bool:
         logger.debug(f"[local] append related_illusts {illust_id} "
-                    f"({len(content)} items) "
-                    f"{metadata}")
+                     f"({len(content)} items) "
+                     f"{metadata}")
         async with data_source.start_session() as session:
-            return await self._append_and_check_illusts(session, RelatedIllustsCache,
-                                                        RelatedIllustsCache.original_illust_id == illust_id,
+            return await self._append_and_check_illusts(session, "related_illusts", {"original_illust_id": illust_id},
                                                         content=content, metadata=metadata)
 
-    # ================ illust_ranking ================
-    async def illust_ranking(self, mode: Union[str, RankingMode], *, offset: int = 0) \
-            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        if isinstance(mode, str):
-            mode = RankingMode[mode]
-
-        logger.debug(f"[local] illust_ranking {mode}")
-
+    # ================ search_user ================
+    async def search_user(self, word: str, *, offset: int = 0) \
+            -> AsyncGenerator[Union[User, PixivRepoMetadata], None]:
+        logger.debug(f"[local] search_user {word}")
         async with data_source.start_session() as session:
-            async for x in self._get_illusts(session, IllustRankingCache, IllustRankingCache.mode == mode,
-                                             expired_in=conf.pixiv_illust_ranking_cache_expires_in, offset=offset):
+            async for x in self._get_users(session, "search_user", {"word": word},
+                                           expired_in=conf.pixiv_search_user_cache_expires_in, offset=offset):
                 yield x
 
-    async def invalidate_illust_ranking(self, mode: RankingMode):
-        logger.debug(f"[local] invalidate illust_ranking")
+    async def invalidate_search_user(self, word: str):
+        logger.debug(f"[local] invalidate search_user {word}")
         async with data_source.start_session() as session:
-            await IllustRankingCache.find_one(IllustRankingCache.mode == mode,
-                                              session=session).delete()
+            await self._invalidate_users(session, "search_user", {"word": word})
 
-    async def append_illust_ranking(self, mode: RankingMode, content: List[Union[Illust, LazyIllust]],
-                                    metadata: PixivRepoMetadata) -> bool:
-        logger.debug(f"[local] append illust_ranking {mode} "
-                    f"({len(content)} items) "
-                    f"{metadata}")
+    async def append_search_user(self, word: str, content: List[User],
+                                 metadata: PixivRepoMetadata) -> bool:
+        logger.debug(f"[local] append search_user {word} "
+                     f"({len(content)} items) "
+                     f"{metadata}")
         async with data_source.start_session() as session:
-            return await self._append_and_check_illusts(session, IllustRankingCache, IllustRankingCache.mode == mode,
-                                                        content=content, metadata=metadata)
+            return await self._append_and_check_users(session, "search_user", {"word": word},
+                                                      content=content, metadata=metadata)
+
+    async def invalidate_all(self):
+        logger.debug(f"[local] invalidate_all")
 
-    # ================ image ================
-    async def image(self, illust: Illust, page: int = 0) -> AsyncGenerator[Union[bytes, PixivRepoMetadata], None]:
-        logger.debug(f"[local] image {illust.id}")
         async with data_source.start_session() as session:
-            doc = await DownloadCache.find_one(DownloadCache.illust_id == illust.id,
-                                               DownloadCache.page == page,
-                                               session=session)
-            if doc is not None:
-                _handle_expires_in(doc.metadata, conf.pixiv_download_cache_expires_in)
-                yield doc.metadata
-                yield doc.content
-            else:
-                raise NoSuchItemError()
+            if conf.pixiv_sql_dialect == 'sqlite':
+                await session.execute(text("PRAGMA foreign_keys = ON;"))
 
-    async def update_image(self, illust_id: int, page: int,
-                           content: bytes, metadata: PixivRepoMetadata):
-        logger.debug(f"[local] update image {illust_id} "
-                    f"{metadata}")
+            result = await session.execute(delete(IllustSetCache))
+            logger.success(f"[local] deleted {result.rowcount} illust_set cache")
+            result = await session.execute(delete(UserSetCache))
+            logger.success(f"[local] deleted {result.rowcount} user_set cache")
+            result = await session.execute(delete(IllustDetailCache))
+            logger.success(f"[local] deleted {result.rowcount} illust_detail cache")
+            result = await session.execute(delete(UserDetailCache))
+            logger.success(f"[local] deleted {result.rowcount} user_detail cache")
+            result = await session.execute(delete(DownloadCache))
+            logger.success(f"[local] deleted {result.rowcount} download cache")
+            await session.commit()
+
+    async def clean_expired(self):
+        logger.debug(f"[local] clean_expired")
+
+        async with data_source.start_session() as session:
+            if conf.pixiv_sql_dialect == 'sqlite':
+                await session.execute(text("PRAGMA foreign_keys = ON;"))
+
+            now = datetime.utcnow()
+            stmt = delete(IllustDetailCache).where(
+                IllustDetailCache.update_time <= now - timedelta(seconds=conf.pixiv_illust_detail_cache_expires_in)
+            )
+            result = await session.execute(stmt)
+            logger.success(f"[local] deleted {result.rowcount} illust_detail cache")
 
-        async with data_source.start_session() as session:
-            await DownloadCache.find_one(
-                DownloadCache.illust_id == illust_id,
-                DownloadCache.page == page,
-                session=session
-            ).update(
-                Set({
-                    DownloadCache.content: bson.Binary(content),
-                    DownloadCache.metadata: metadata
-                }),
-                upsert=True,
-                session=session
+            stmt = delete(UserDetailCache).where(
+                UserDetailCache.update_time <= now - timedelta(seconds=conf.pixiv_user_detail_cache_expires_in)
             )
+            result = await session.execute(stmt)
+            logger.success(f"[local] deleted {result.rowcount} user_detail cache")
 
-    async def invalidate_all(self):
-        logger.debug(f"[local] invalidate_all")
-        async with data_source.start_session() as session:
-            await DownloadCache.delete_all(session=session)
-            await IllustDetailCache.delete_all(session=session)
-            await UserDetailCache.delete_all(session=session)
-            await IllustRankingCache.delete_all(session=session)
-            await SearchIllustCache.delete_all(session=session)
-            await SearchUserCache.delete_all(session=session)
-            await UserIllustsCache.delete_all(session=session)
-            await UserBookmarksCache.delete_all(session=session)
-            await OtherIllustCache.delete_all(session=session)
+            stmt = delete(DownloadCache).where(
+                DownloadCache.update_time <= now - timedelta(seconds=conf.pixiv_download_cache_expires_in)
+            )
+            result = await session.execute(stmt)
+            logger.success(f"[local] deleted {result.rowcount} download cache")
+
+            stmt = delete(IllustSetCache).where(
+                IllustSetCache.cache_type == 'illust_ranking',
+                IllustSetCache.update_time <= now - timedelta(seconds=conf.pixiv_illust_ranking_cache_expires_in)
+            )
+            result = await session.execute(stmt)
+            logger.success(f"[local] deleted {result.rowcount} illust_ranking cache")
 
+            stmt = delete(IllustSetCache).where(
+                IllustSetCache.cache_type == 'search_illust',
+                IllustSetCache.update_time <= now - timedelta(seconds=conf.pixiv_search_illust_cache_delete_in)
+            )
+            result = await session.execute(stmt)
+            logger.success(f"[local] deleted {result.rowcount} search_illust cache")
+
+            stmt = delete(UserSetCache).where(
+                UserSetCache.cache_type == 'search_user',
+                UserSetCache.update_time <= now - timedelta(seconds=conf.pixiv_search_user_cache_delete_in)
+            )
+            result = await session.execute(stmt)
+            logger.success(f"[local] deleted {result.rowcount} search_user cache")
+
+            stmt = delete(IllustSetCache).where(
+                IllustSetCache.cache_type == 'user_illusts',
+                IllustSetCache.update_time <= now - timedelta(seconds=conf.pixiv_user_illusts_cache_delete_in)
+            )
+            result = await session.execute(stmt)
+            logger.success(f"[local] deleted {result.rowcount} user_illusts cache")
+
+            stmt = delete(IllustSetCache).where(
+                IllustSetCache.cache_type == 'user_bookmarks',
+                IllustSetCache.update_time <= now - timedelta(seconds=conf.pixiv_user_bookmarks_cache_delete_in)
+            )
+            result = await session.execute(stmt)
+            logger.success(f"[local] deleted {result.rowcount} user_bookmarks cache")
+
+            stmt = delete(IllustSetCache).where(
+                IllustSetCache.cache_type == 'related_illusts',
+                IllustSetCache.update_time <= now - timedelta(seconds=conf.pixiv_related_illusts_cache_expires_in)
+            )
+            result = await session.execute(stmt)
+            logger.success(f"[local] deleted {result.rowcount} related_illusts cache")
+
+            stmt = delete(IllustSetCache).where(
+                IllustSetCache.cache_type == 'other',
+                IllustSetCache.update_time <= now - timedelta(seconds=conf.pixiv_other_cache_expires_in)
+            )
+            result = await session.execute(stmt)
+            logger.success(f"[local] deleted {result.rowcount} other cache")
 
-__all__ = ("MongoPixivRepo",)
+            await session.commit()
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql_models.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql_models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 from datetime import datetime
 from typing import Optional, List
 
 from sqlalchemy import ForeignKey, UniqueConstraint
 from sqlalchemy.orm import mapped_column, relationship, Mapped
 
-from nonebot_plugin_pixivbot.data.source.sql import SqlDataSource
-from nonebot_plugin_pixivbot.data.utils.sql import BLOB, JSON, UTCDateTime
+from ...source.sql import DataSource
+from ...utils.sql import BLOB, JSON, UTCDateTime
 
 
-@SqlDataSource.registry.mapped
+@DataSource.registry.mapped
 class DownloadCache:
     __tablename__ = "download_cache"
 
     illust_id: Mapped[int] = mapped_column(primary_key=True)
     page: Mapped[int] = mapped_column(primary_key=True, default=0)
     content: Mapped[bytes] = mapped_column(BLOB)
 
     update_time: Mapped[datetime] = mapped_column(UTCDateTime, index=True)
 
 
-@SqlDataSource.registry.mapped
+@DataSource.registry.mapped
 class IllustDetailCache:
     __tablename__ = "illust_detail_cache"
 
     illust_id: Mapped[int] = mapped_column(primary_key=True)
     illust: Mapped[dict] = mapped_column(JSON)
 
     update_time: Mapped[datetime] = mapped_column(UTCDateTime, index=True)
 
 
-@SqlDataSource.registry.mapped
+@DataSource.registry.mapped
 class UserDetailCache:
     __tablename__ = "user_detail_cache"
 
     user_id: Mapped[int] = mapped_column(primary_key=True)
     user: Mapped[dict] = mapped_column(JSON)
 
     update_time: Mapped[datetime] = mapped_column(UTCDateTime, index=True)
 
 
-@SqlDataSource.registry.mapped
+@DataSource.registry.mapped
 class IllustSetCache:
     __tablename__ = "illust_set_cache"
 
     id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
     cache_type: Mapped[str]
     key: Mapped[dict] = mapped_column(JSON)
 
@@ -58,24 +58,24 @@
     size: Mapped[int] = mapped_column(default=0)
 
     __table_args__ = (
         UniqueConstraint('cache_type', 'key'),
     )
 
 
-@SqlDataSource.registry.mapped
+@DataSource.registry.mapped
 class IllustSetCacheIllust:
     __tablename__ = "illust_set_cache_illust"
 
     cache_id: Mapped[int] = mapped_column(ForeignKey("illust_set_cache.id", ondelete="cascade"), primary_key=True)
     illust_id: Mapped[int] = mapped_column(primary_key=True)
     rank: Mapped[int] = mapped_column(default=0)
 
 
-@SqlDataSource.registry.mapped
+@DataSource.registry.mapped
 class UserSetCache:
     __tablename__ = "user_set_cache"
 
     id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
     cache_type: Mapped[str]
     key: Mapped[dict] = mapped_column(JSON)
 
@@ -88,13 +88,13 @@
                                                                passive_deletes=True)
 
     __table_args__ = (
         UniqueConstraint('cache_type', 'key'),
     )
 
 
-@SqlDataSource.registry.mapped
+@DataSource.registry.mapped
 class UserSetCacheUser:
     __tablename__ = "user_set_cache_user"
 
     cache_id: Mapped[int] = mapped_column(ForeignKey("user_set_cache.id", ondelete="cascade"), primary_key=True)
     user_id: Mapped[int] = mapped_column(primary_key=True)
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator_repo.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator_repo.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/remote_repo.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/remote_repo.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/source/lifecycle_mixin.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/lifecycle_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 from inspect import isawaitable
 from typing import Callable, Union, Awaitable
 
 from nonebot import logger
 
 
-class DataSourceLifecycleMixin:
+class DataSourceLifecycle:
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._on_initializing_callbacks = []
         self._on_initialized_callbacks = []
         self._on_closing_callbacks = []
         self._on_closed_callbacks = []
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/source/migration_manager.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/migration_manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/source/sql/__init__.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/sql/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import json
 from contextlib import asynccontextmanager
 from datetime import datetime, date
 from typing import AsyncContextManager
 
 from nonebot import get_driver, logger
 from sqlalchemy import select, inspect
-from sqlalchemy.ext.asyncio import create_async_engine, AsyncSession, AsyncEngine
+from sqlalchemy.ext.asyncio import create_async_engine, AsyncSession, AsyncEngine, AsyncConnection
 from sqlalchemy.orm import registry, sessionmaker
 from sqlalchemy.pool import StaticPool
 
-from nonebot_plugin_pixivbot.config import Config
-from nonebot_plugin_pixivbot.enums import DataSourceType
-from nonebot_plugin_pixivbot.global_context import context
-from nonebot_plugin_pixivbot.utils.lifecycler import on_startup, on_shutdown
-from ..lifecycle_mixin import DataSourceLifecycleMixin
+from ..lifecycle_mixin import DataSourceLifecycle
 from ...errors import DataSourceNotReadyError
+from ....config import Config
+from ....global_context import context
+from ....utils.lifecycler import on_startup, on_shutdown
 
 conf = context.require(Config)
 
 
 def default_dumps(obj):
     if isinstance(obj, (datetime, date)):
         return obj.isoformat()
@@ -26,66 +25,61 @@
     return None
 
 
 def json_serializer(obj):
     return json.dumps(obj, default=default_dumps)
 
 
-class SqlDataSource(DataSourceLifecycleMixin):
-    app_db_version = 4
+@context.register_eager_singleton()
+class DataSource(DataSourceLifecycle):
+    app_db_version = 5
     registry = registry()
 
     def __init__(self):
         super().__init__()
 
         self._engine = None
         self._sessionmaker = None
 
         on_startup(replay=True)(self.initialize)
         on_shutdown()(self.close)
 
-    async def _raw_get_db_version(self) -> int:
-        async with self._engine.begin() as conn:
-            async with AsyncSession(conn, expire_on_commit=False) as session:
-                from .meta_info import MetaInfo
-
-                # 判断是否初次建库
-                blank_database = not await conn.run_sync(lambda conn: inspect(conn).has_table("subscription"))
-                if blank_database:
-                    result = MetaInfo(key="db_version", value=str(self.app_db_version))
-                    session.add(result)
-                    await session.commit()
-                    v = self.app_db_version
-                else:
-                    stmt = select(MetaInfo).where(MetaInfo.key == "db_version")
-                    result = (await session.execute(stmt)).scalar_one_or_none()
-                    if result is None:
-                        result = MetaInfo(key="db_version", value="1")
-                        session.add(result)
-                        await session.commit()
-
-                    v = int(result.value)
-
-            await conn.commit()
-            return v
+    async def _raw_get_db_version(self, conn: AsyncConnection) -> int:
+        async with AsyncSession(conn, expire_on_commit=False) as session:
+            from .meta_info import MetaInfo
 
-    async def _raw_set_db_version(self, db_version: int):
-        from .meta_info import MetaInfo
-        async with self._engine.begin() as conn:
-            async with AsyncSession(conn, expire_on_commit=False) as session:
+            # 判断是否初次建库
+            blank_database = not await conn.run_sync(lambda conn: inspect(conn).has_table("subscription"))
+            if blank_database:
+                result = MetaInfo(key="db_version", value=str(self.app_db_version))
+                session.add(result)
+                await session.commit()
+                v = self.app_db_version
+            else:
                 stmt = select(MetaInfo).where(MetaInfo.key == "db_version")
                 result = (await session.execute(stmt)).scalar_one_or_none()
                 if result is None:
                     result = MetaInfo(key="db_version", value="1")
                     session.add(result)
+                    await session.commit()
 
-                result.value = str(db_version)
-                await session.commit()
+                v = int(result.value)
+        return v
 
-            await conn.commit()
+    async def _raw_set_db_version(self, db_version: int, conn: AsyncConnection):
+        from .meta_info import MetaInfo
+        async with AsyncSession(conn, expire_on_commit=False) as session:
+            stmt = select(MetaInfo).where(MetaInfo.key == "db_version")
+            result = (await session.execute(stmt)).scalar_one_or_none()
+            if result is None:
+                result = MetaInfo(key="db_version", value="1")
+                session.add(result)
+
+            result.value = str(db_version)
+            await session.commit()
 
     async def initialize(self):
         await self._fire_initializing()
 
         driver = get_driver()
 
         params = {
@@ -107,20 +101,22 @@
         async with self._engine.begin() as conn:
             from .migration import SqlMigrationManager
             from .meta_info import MetaInfo
 
             await conn.run_sync(lambda conn: MetaInfo.__table__.create(conn, checkfirst=True))
 
             # migrate
-            mig_mgr = SqlMigrationManager(lambda prev, cur: self._raw_set_db_version(cur))
-            db_version = await self._raw_get_db_version()
+            mig_mgr = SqlMigrationManager(lambda prev, cur: self._raw_set_db_version(cur, conn))
+            db_version = await self._raw_get_db_version(conn)
             await mig_mgr.perform_migration(conn, db_version, self.app_db_version)
 
             await conn.run_sync(lambda conn: self.registry.metadata.create_all(conn))
 
+            await conn.commit()
+
         # expire_on_commit=False will prevent attributes from being expired
         # after commit.
         self._sessionmaker = sessionmaker(self._engine, expire_on_commit=False, class_=AsyncSession)
 
         logger.success(f"[data source] SqlDataSource Initialized (dialect: {conf.pixiv_sql_dialect})")
         await self._fire_initialized()
 
@@ -145,11 +141,8 @@
     @property
     def engine(self) -> AsyncEngine:
         if self._engine is None:
             raise DataSourceNotReadyError()
         return self._engine
 
 
-if conf.pixiv_data_source == DataSourceType.sql:
-    context.register_eager_singleton()(SqlDataSource)
-
-__all__ = ("SqlDataSource",)
+__all__ = ("DataSource",)
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v1_to_v2.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v1_to_v2.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v2_to_v3.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v2_to_v3.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Callable, Awaitable
 
 from nonebot import Bot
 from sqlalchemy import text
 from sqlalchemy.ext.asyncio import AsyncConnection
 
-from nonebot_plugin_pixivbot.global_context import context
-from nonebot_plugin_pixivbot.utils.lifecycler import on_bot_connect
-from nonebot_plugin_pixivbot.utils.nonebot import get_adapter_name
-from .. import SqlDataSource
 from ...migration_manager import DeferrableMigration
+from ...sql import DataSource
+from .....global_context import context
+from .....utils.lifecycler import on_bot_connect
+from .....utils.nonebot import get_adapter_name
 
 
 class SqlV2ToV3(DeferrableMigration):
     from_db_version = 2
     to_db_version = 3
     safe = True
 
     async def migrate(self, conn: AsyncConnection, on_migrated: Callable[[], Awaitable[None]]):
-        data_source = context.require(SqlDataSource)
+        data_source = context.require(DataSource)
 
         @on_bot_connect(replay=True, first=True)
         async def _(bot: Bot):
             async with AsyncConnection(data_source.engine) as conn:
                 adapter = get_adapter_name(bot)
                 await conn.execute(
                     text(f"update watch_task set bot=bot || '\:{bot.self_id}' where bot = '{adapter}'; ")
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/subscription/sql.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/watch_task.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,143 +1,155 @@
+from datetime import datetime
 from typing import Optional, AsyncIterable, Collection
 
-import tzlocal
-from sqlalchemy import select, UniqueConstraint
+from nonebot_plugin_session import Session
+from pytz import utc
+from sqlalchemy import select, UniqueConstraint, update
 from sqlalchemy.orm import mapped_column, Mapped
 
-from nonebot_plugin_pixivbot.global_context import context
-from nonebot_plugin_pixivbot.model import Subscription, PostIdentifier, ScheduleType, T_UID, T_GID, UserIdentifier
-from .base import SubscriptionRepo
-from ..interval_task_repo import process_subscriber
-from ..source.sql import SqlDataSource
-from ..utils.shortuuid import gen_code
-from ..utils.sql import insert, JSON
+from .interval_task_repo import IntervalTaskRepo, process_subscriber
+from .nb_session import NbSessionRepo
+from .source.sql import DataSource
+from .utils.shortuuid import gen_code
+from .utils.sql import insert, JSON, UTCDateTime
+from ..global_context import context
+from ..model import WatchType, WatchTask
 
 
-@SqlDataSource.registry.mapped
-class SubscriptionOrm:
-    __tablename__ = "subscription"
+@DataSource.registry.mapped
+class WatchTaskOrm:
+    __tablename__ = "watch_task"
 
     id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
-    subscriber: Mapped[dict] = mapped_column(JSON)
+    session_id: Mapped[int]
     code: Mapped[str]
-    type: Mapped[ScheduleType]
+    type: Mapped[WatchType]
     kwargs: Mapped[dict] = mapped_column(JSON, default=dict)
-    bot: Mapped[str]
-    schedule: Mapped[dict] = mapped_column(JSON)
-    tz: Mapped[str] = mapped_column(default=tzlocal.get_localzone_name)
+    bot_id: Mapped[str]
+    checkpoint: Mapped[datetime] = mapped_column(UTCDateTime)
 
     __table_args__ = (
-        UniqueConstraint("bot", "subscriber", "code"),
+        UniqueConstraint("bot_id", "session_id", "code"),
+        UniqueConstraint("bot_id", "session_id", "type", "kwargs"),
     )
 
 
-def _to_model(item: SubscriptionOrm) -> Subscription:
-    adapter, bot_id = item.bot.split(':')
-    return Subscription(subscriber=PostIdentifier(**item.subscriber),
-                        code=item.code,
-                        type=item.type,
-                        kwargs=item.kwargs,
-                        bot=UserIdentifier(adapter, bot_id),
-                        schedule=item.schedule,
-                        tz=item.tz)
+data_source = context.require(DataSource)
+nb_session_repo = context.require(NbSessionRepo)
 
 
-data_source = context.require(SqlDataSource)
+async def _to_model(item: WatchTaskOrm) -> WatchTask:
+    subscriber = await nb_session_repo.get_session(item.session_id)
+    return WatchTask(subscriber=subscriber,
+                     code=item.code,
+                     type=item.type,
+                     kwargs=item.kwargs,
+                     checkpoint=item.checkpoint)
 
 
 @context.register_singleton()
-class SqlSubscriptionRepo(SubscriptionRepo):
-
-    async def get_by_subscriber(self, bot: UserIdentifier[T_UID],
-                                subscriber: PostIdentifier[T_UID, T_GID]) -> AsyncIterable[Subscription]:
-        subscriber = process_subscriber(subscriber)
-
-        async with data_source.start_session() as session:
-            stmt = (
-                select(SubscriptionOrm)
-                .where(SubscriptionOrm.bot == str(bot),
-                       SubscriptionOrm.subscriber == subscriber.dict())
-            )
-            async for x in await session.stream_scalars(stmt):
-                yield _to_model(x)
-
-    async def get_by_bot(self, bot: UserIdentifier[T_UID]) -> AsyncIterable[Subscription]:
-        async with data_source.start_session() as session:
+class WatchTaskRepo(IntervalTaskRepo[WatchTask]):
+    async def get_by_session(self, session: Session) -> AsyncIterable[WatchTask]:
+        session = process_subscriber(session)
+        session_id = await nb_session_repo.get_id(session)
+        async with data_source.start_session() as db_sess:
             stmt = (
-                select(SubscriptionOrm)
-                .where(SubscriptionOrm.bot == str(bot))
+                select(WatchTaskOrm)
+                .where(WatchTaskOrm.bot_id == session.bot_id,
+                       WatchTaskOrm.session_id == session_id)
             )
-            async for x in await session.stream_scalars(stmt):
-                yield _to_model(x)
+            async for x in await db_sess.stream_scalars(stmt):
+                x.checkpoint = x.checkpoint.replace(tzinfo=utc)
+                yield await _to_model(x)
 
-    async def get_by_code(self, bot: UserIdentifier[T_UID],
-                          subscriber: PostIdentifier[T_UID, T_GID],
-                          code: str) -> Optional[Subscription]:
-        async with data_source.start_session() as session:
+    async def get_by_bot(self, bot_id: str) -> AsyncIterable[WatchTask]:
+        async with data_source.start_session() as db_sess:
             stmt = (
-                select(SubscriptionOrm)
-                .where(SubscriptionOrm.bot == str(bot),
-                       SubscriptionOrm.subscriber == subscriber.dict(),
-                       SubscriptionOrm.code == code)
+                select(WatchTaskOrm)
+                .where(WatchTaskOrm.bot_id == bot_id)
             )
-            x = (await session.execute(stmt)).scalar_one_or_none()
-            if x is not None:
-                return _to_model(x)
-            else:
-                return None
+            async for x in await db_sess.stream_scalars(stmt):
+                x.checkpoint = x.checkpoint.replace(tzinfo=utc)
+                yield await _to_model(x)
+
+    async def get_by_code(self, session: Session,
+                          code: str) -> Optional[WatchTask]:
+        session = process_subscriber(session)
+        session_id = await nb_session_repo.get_id(session)
+        async with data_source.start_session() as db_sess:
+            stmt = (select(WatchTaskOrm)
+                    .where(WatchTaskOrm.bot_id == session.bot_id,
+                           WatchTaskOrm.session_id == session_id,
+                           WatchTaskOrm.code == code))
+            result = (await db_sess.execute(stmt)).scalar_one_or_none()
+            result.checkpoint = result.checkpoint.replace(tzinfo=utc)
+            return await _to_model(result)
 
-    async def insert(self, item: Subscription[T_UID, T_GID]) -> bool:
-        item.subscriber = process_subscriber(item.subscriber)
+    async def insert(self, item: WatchTask) -> bool:
         item.code = gen_code()
+        item.subscriber = process_subscriber(item.subscriber)
+        session_id = await nb_session_repo.get_id(item.subscriber)
 
-        async with data_source.start_session() as session:
-            stmt = (insert(SubscriptionOrm)
-                    .values(subscriber=item.subscriber.dict(),
+        async with data_source.start_session() as db_session:
+            stmt = (insert(WatchTaskOrm)
+                    .values(session_id=session_id,
                             code=item.code,
                             type=item.type,
                             kwargs=item.kwargs,
-                            bot=str(item.bot),
-                            schedule=item.schedule,
-                            tz=item.tz))
-            await session.execute(stmt)
-            await session.commit()
-        return True
-
-    async def delete_one(self, bot: UserIdentifier[T_UID],
-                         subscriber: PostIdentifier[T_UID, T_GID],
-                         code: int) -> Optional[Subscription]:
-        subscriber = process_subscriber(subscriber)
-
-        async with data_source.start_session() as session:
-            stmt = (select(SubscriptionOrm)
-                    .where(SubscriptionOrm.bot == str(bot),
-                           SubscriptionOrm.subscriber == subscriber.dict(),
-                           SubscriptionOrm.code == code)
-                    .limit(1))
-            sub = (await session.execute(stmt)).scalar_one_or_none()
+                            bot_id=item.subscriber.bot_id,
+                            checkpoint=item.checkpoint))
+            stmt = stmt.on_conflict_do_nothing()
+            result = await db_session.execute(stmt)
+            await db_session.commit()
+
+            return result.rowcount == 1
 
-            if sub is None:
-                return sub
+    async def update(self, item: WatchTask) -> bool:
+        item.subscriber = process_subscriber(item.subscriber)
+        session_id = await nb_session_repo.get_id(item.subscriber)
+        async with data_source.start_session() as db_session:
+            stmt = (update(WatchTaskOrm)
+                    .values(type=item.type,
+                            kwargs=item.kwargs,
+                            bot_id=item.subscriber.bot_id,
+                            checkpoint=item.checkpoint)
+                    .where(WatchTaskOrm.session_id == session_id,
+                           WatchTaskOrm.code == item.code))
+            result = await db_session.execute(stmt)
+            await db_session.commit()
+            return result.rowcount == 1
+
+    async def delete_one(self, session: Session, code: str) -> Optional[WatchTask]:
+        session = process_subscriber(session)
+        session_id = await nb_session_repo.get_id(session)
+        async with data_source.start_session() as db_sess:
+            stmt = (select(WatchTaskOrm)
+                    .where(WatchTaskOrm.bot_id == session.bot_id,
+                           WatchTaskOrm.session_id == session_id,
+                           WatchTaskOrm.code == code)
+                    .limit(1))
+            task = (await db_sess.execute(stmt)).scalar_one_or_none()
 
-            await session.delete(sub)
-            await session.commit()
-            return _to_model(sub)
+            if task is None:
+                return task
 
-    async def delete_many_by_subscriber(self, bot: UserIdentifier[T_UID],
-                                        subscriber: PostIdentifier[T_UID, T_GID]) -> Collection[Subscription]:
-        subscriber = process_subscriber(subscriber)
+            await db_sess.delete(task)
+            await db_sess.commit()
+            return await _to_model(task)
 
-        async with data_source.start_session() as session:
-            stmt = (select(SubscriptionOrm)
-                    .where(SubscriptionOrm.bot == str(bot),
-                           SubscriptionOrm.subscriber == subscriber.dict()))
-            subs = (await session.execute(stmt)).scalars().all()
+    async def delete_many_by_session(self, session: Session) -> Collection[WatchTask]:
+        session = process_subscriber(session)
+        session_id = await nb_session_repo.get_id(session)
+        async with data_source.start_session() as db_sess:
+            stmt = (select(WatchTaskOrm)
+                    .where(WatchTaskOrm.bot_id == session.bot_id,
+                           WatchTaskOrm.session_id == session_id))
+            tasks = (await db_sess.execute(stmt)).scalars().all()
 
-            for t in subs:
-                await session.delete(t)
+            for t in tasks:
+                await db_sess.delete(t)
 
-            await session.commit()
-            return [_to_model(x) for x in subs]
+            await db_sess.commit()
+            return [await _to_model(x) for x in tasks]
 
 
-__all__ = ("SqlSubscriptionRepo",)
+__all__ = ("WatchTaskRepo",)
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/utils/sql/__init__.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/utils/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/utils/sql/utc_datetime.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/utils/sql/utc_datetime.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/data/utils/sql.pyi` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/utils/sql.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/enums.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/enums.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 from enum import Enum
 
-__all__ = ("DataSourceType", "BlockAction", "DownloadQuantity", "RandomIllustMethod", "RankingMode",)
-
-
-class DataSourceType(str, Enum):
-    mongo = 'mongo'
-    sql = 'sql'
+__all__ = ("BlockAction", "DownloadQuantity", "RandomIllustMethod", "RankingMode",)
 
 
 class BlockAction(str, Enum):
     no_image = 'no_image'
     completely_block = 'completely_block'
     no_reply = 'no_reply'
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/base.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from abc import ABC, abstractmethod, ABCMeta
+from asyncio import Event
 from typing import Sequence, Optional
 from typing import Type
 
 from nonebot import logger
+from nonebot_plugin_access_control.subject.extractor import extract_subjects_from_session
+from nonebot_plugin_session import Session
 
-from nonebot_plugin_pixivbot.config import Config
-from nonebot_plugin_pixivbot.model import Illust, T_UID, T_GID
-from nonebot_plugin_pixivbot.model.message import IllustMessagesModel
-from nonebot_plugin_pixivbot.protocol_dep.post_dest import PostDestination
-from nonebot_plugin_pixivbot.protocol_dep.postman import PostmanManager
 from .interceptor.base import Interceptor, DummyInterceptor
 from .interceptor.combined_interceptor import CombinedInterceptor
 from .interceptor.default_error_interceptor import DefaultErrorInterceptor
 from .interceptor.service_interceptor import ServiceInterceptor
 from .pkg_context import context
+from ..config import Config
+from ..model import Illust
+from ..model.message import IllustMessagesModel
 from ..plugin_service import r18_service, r18g_service
+from ..service.postman import Postman
 from ..utils.algorithm import as_unique
 
 conf = context.require(Config)
 
 
 def _log_interceptors(cls: Type["Handler"]):
     if isinstance(cls.interceptor, CombinedInterceptor):
@@ -75,18 +77,19 @@
 
         return cls
 
 
 class Handler(ABC, metaclass=HandlerMeta):
     interceptor: Interceptor
 
-    def __init__(self, post_dest: PostDestination[T_UID, T_GID],
+    def __init__(self, session: Session, event: Optional[Event] = None,
                  *, silently: bool = False,
                  disable_interceptors: bool = False):
-        self.post_dest = post_dest
+        self.session = session
+        self.event = event
         self.silently = silently
         self.disable_interceptors = disable_interceptors
 
     @classmethod
     @abstractmethod
     def type(cls) -> str:
         raise NotImplementedError()
@@ -100,26 +103,20 @@
         将位置参数转化为命名参数
         :param args: 位置参数sequence
         :return: 命名参数dict
         """
         return {}
 
     async def handle(self, *args, **kwargs):
-        if not self.enabled():
-            return
-
         if not self.disable_interceptors:
             await self.interceptor.intercept(self, self._parse_args_and_actual_handle, *args, **kwargs)
         else:
             await self._parse_args_and_actual_handle(*args, **kwargs)
 
     async def handle_with_parsed_args(self, **kwargs):
-        if not self.enabled():
-            return
-
         if not self.disable_interceptors:
             await self.interceptor.intercept(self, self.actual_handle, **kwargs)
         else:
             await self.actual_handle(**kwargs)
 
     async def _parse_args_and_actual_handle(self, *args, **kwargs):
         parsed_kwargs = await self.parse_args(args)
@@ -195,46 +192,42 @@
         if front:
             cls.interceptor = CombinedInterceptor(interceptor, cls.interceptor)
         else:
             cls.interceptor = CombinedInterceptor(cls.interceptor, interceptor)
         _log_interceptors(cls)
 
     async def is_r18_allowed(self) -> bool:
-        return await r18_service.check_by_subject(*self.post_dest.extract_subjects(),
+        return await r18_service.check_by_subject(*extract_subjects_from_session(self.session),
                                                   acquire_rate_limit_token=False)
 
     async def is_r18g_allowed(self) -> bool:
-        return await r18g_service.check_by_subject(*self.post_dest.extract_subjects(),
+        return await r18g_service.check_by_subject(*extract_subjects_from_session(self.session),
                                                    acquire_rate_limit_token=False)
 
     async def post_plain_text(self, message: str):
-
-        postman_manager = context.require(PostmanManager)
-        await postman_manager.send_plain_text(message, post_dest=self.post_dest)
+        await context.require(Postman).post_plain_text(message, self.session, self.event)
 
     async def post_illust(self, illust: Illust, *,
                           header: Optional[str] = None,
                           number: Optional[int] = None):
-        postman_manager = context.require(PostmanManager)
         model = await IllustMessagesModel.from_illust(illust, header=header, number=number,
                                                       max_page=conf.pixiv_max_item_per_query,
                                                       block_r18=(not await self.is_r18_allowed()),
                                                       block_r18g=(not await self.is_r18g_allowed()))
         if model:
-            await postman_manager.send_illusts(model, post_dest=self.post_dest)
+            await context.require(Postman).post_illusts(model, self.session, self.event)
 
     async def post_illusts(self, illusts: Sequence[Illust], *,
                            header: Optional[str] = None,
                            number: Optional[int] = None):
-        postman_manager = context.require(PostmanManager)
         if len(illusts) == 1:
             await self.post_illust(illusts[0], header=header, number=number)
         else:
             model = await IllustMessagesModel.from_illusts(illusts, header=header, number=number,
                                                            block_r18=(not await self.is_r18_allowed()),
                                                            block_r18g=(not await self.is_r18g_allowed()))
             if model:
-                await postman_manager.send_illusts(model, post_dest=self.post_dest)
+                await context.require(Postman).post_illusts(model, self.session, self.event)
 
 
 class EntryHandler(Handler, ABC, interceptors=[context.require(DefaultErrorInterceptor)]):
     pass
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/command/bind.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/command/bind.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import Sequence
 
-from nonebot_plugin_pixivbot.plugin_service import bind_service
-from nonebot_plugin_pixivbot.service.pixiv_account_binder import PixivAccountBinder
-from nonebot_plugin_pixivbot.utils.errors import BadRequestError
-from nonebot_plugin_pixivbot.utils.nonebot import default_command_start
 from .subcommand import SubCommandHandler
-from ..interceptor.service_interceptor import ServiceInterceptor
 from ..pkg_context import context
+from ...plugin_service import bind_service
+from ...service.pixiv_account_binder import PixivAccountBinder
+from ...utils.errors import BadRequestError
+from ...utils.nonebot import default_command_start
 
 binder = context.require(PixivAccountBinder)
 
 
 class BindHandler(SubCommandHandler, subcommand='bind', service=bind_service):
     @classmethod
     def type(cls) -> str:
@@ -25,23 +24,23 @@
             except ValueError as e:
                 raise BadRequestError("请输入正确格式的Pixiv账号") from e
 
             return {"pixiv_user_id": pixiv_user_id}
 
     # noinspection PyMethodOverriding
     async def actual_handle(self, *, pixiv_user_id: int):
-        await binder.bind(self.post_dest.adapter, self.post_dest.user_id, pixiv_user_id)
+        await binder.bind(self.session.platform, self.session.id1, pixiv_user_id)
         await self.post_plain_text(message="Pixiv账号绑定成功")
 
     async def actual_handle_bad_request(self, err: BadRequestError):
         if not self.silently:
             if err.message:
                 await self.post_plain_text(message=err.message)
             else:
-                pixiv_user_id = await binder.get_binding(self.post_dest.adapter, self.post_dest.user_id)
+                pixiv_user_id = await binder.get_binding(self.session.platform, self.session.id1)
                 if pixiv_user_id is not None:
                     msg = f"当前绑定账号：{pixiv_user_id}\n"
                 else:
                     msg = "当前未绑定Pixiv账号\n"
                 msg += f"命令格式：{default_command_start}pixivbot bind <pixiv_user_id>"
                 await self.post_plain_text(message=msg)
 
@@ -49,12 +48,12 @@
 class UnbindHandler(SubCommandHandler, subcommand='unbind', service=bind_service):
     @classmethod
     def type(cls) -> str:
         return "unbind"
 
     # noinspection PyMethodOverriding
     async def actual_handle(self):
-        result = await binder.unbind(self.post_dest.adapter, self.post_dest.user_id)
+        result = await binder.unbind(self.session.platform, self.session.id1)
         if result:
             await self.post_plain_text(message="Pixiv账号解绑成功")
         else:
             await self.post_plain_text(message="当前未绑定Pixiv账号")
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/command/command.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/command/command.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Type, Sequence, Dict, TYPE_CHECKING
 
 from nonebot import logger
 from nonebot import on_command
 from nonebot.internal.adapter import Event
 from nonebot.internal.params import Depends
+from nonebot_plugin_session import extract_session
 
-from nonebot_plugin_pixivbot.protocol_dep.post_dest import post_destination
 from ..base import EntryHandler
 from ..utils import get_command_rule
 
 if TYPE_CHECKING:
     from .subcommand import SubCommandHandler
 
 
@@ -40,21 +40,22 @@
         elif args[0] not in self.subcommand_handlers:
             if not self.silently:
                 await self.post_plain_text(f"不存在命令 '{args[0]}'")
             return
         else:
             handler_type = self.subcommand_handlers[args[0]]
 
-        handler = handler_type(self.post_dest, silently=self.silently, disable_interceptors=self.disable_interceptors)
+        handler = handler_type(self.session, self.event, silently=self.silently,
+                               disable_interceptors=self.disable_interceptors)
         await handler.handle(*args[1:])
 
 
 @on_command("pixivbot", rule=get_command_rule(), priority=5).handle()
 async def _(event: Event,
-            post_dest=Depends(post_destination)):
+            session=Depends(extract_session)):
     raw_args = str(event.get_message()).strip() + ' '  # 末尾加一个空格用于处理边界
 
     args = []
     slash = False
     pending_arg = ""
     for c in raw_args:
         if slash:
@@ -69,8 +70,8 @@
                 pending_arg = ""
         else:
             pending_arg += c
 
     logger.debug(f"command args: {args}")
     args = args[1:]
 
-    await CommandHandler(post_dest).handle(*args)
+    await CommandHandler(session, event).handle(*args)
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/command/invalidate_cache.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/command/invalidate_cache.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from nonebot_plugin_pixivbot.data.pixiv_repo import PixivRepo
-from nonebot_plugin_pixivbot.plugin_service import invalidate_cache_service
 from .subcommand import SubCommandHandler
 from ..interceptor.permission_interceptor import SuperuserInterceptor
-from ..interceptor.service_interceptor import ServiceInterceptor
 from ..pkg_context import context
+from ...data.pixiv_repo import PixivRepo
+from ...plugin_service import invalidate_cache_service
 
 repo = context.require(PixivRepo)
 
 
 class InvalidateCacheHandler(SubCommandHandler, subcommand='invalidate_cache', service=invalidate_cache_service,
                              interceptors=[context.require(SuperuserInterceptor)]):
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/command/schedule.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/service/scheduler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,106 +1,122 @@
-from io import StringIO
-from typing import Sequence
+from __future__ import annotations
 
-from nonebot_plugin_pixivbot.model import ScheduleType
-from nonebot_plugin_pixivbot.model import T_UID, T_GID
-from nonebot_plugin_pixivbot.plugin_service import manage_schedule_service
-from nonebot_plugin_pixivbot.protocol_dep.post_dest import PostDestination
-from nonebot_plugin_pixivbot.service.scheduler import Scheduler
-from nonebot_plugin_pixivbot.utils.errors import BadRequestError
-from nonebot_plugin_pixivbot.utils.nonebot import default_command_start
-from .subcommand import SubCommandHandler
-from ..pkg_context import context
-
-scheduler = context.require(Scheduler)
-
-
-async def build_subscriptions_msg(post_dest: PostDestination[T_UID, T_GID]):
-    scheduler = context.require(Scheduler)
-    subscription = [x async for x in scheduler.get_by_subscriber(post_dest)]
-    with StringIO() as sio:
-        sio.write("当前订阅：\n")
-        if len(subscription) > 0:
-            for sub in subscription:
-                sio.write(f'[{sub.code}] {sub.type.name} {sub.schedule_text}')
-                args_text = sub.args_text
-                if args_text:
-                    sio.write(f' ({args_text})')
-                sio.write('\n')
+import re
+from datetime import datetime, timedelta
+from inspect import isawaitable
+from typing import Sequence, Union, TYPE_CHECKING, overload, Type
+
+import pytz
+from apscheduler.triggers.interval import IntervalTrigger
+from nonebot_plugin_session import Session
+
+from .interval_task_worker import IntervalTaskWorker
+from ..data.subscription import SubscriptionRepo
+from ..global_context import context
+from ..model import Subscription
+from ..model.subscription import ScheduleType
+from ..utils.errors import BadRequestError
+
+if TYPE_CHECKING:
+    from nonebot_plugin_pixivbot.handler.base import Handler
+
+
+def parse_schedule(raw_schedule: str) -> Sequence[int]:
+    start_only_mat = re.fullmatch(r'(\d+):(\d+)', raw_schedule)
+    if start_only_mat is not None:
+        g = start_only_mat.groups()
+        start_hour, start_minute = int(g[0]), int(g[1])
+        interval_hour, interval_minute = 24, 0
+    else:
+        interval_only_mat = re.fullmatch(
+            r'(\d+):(\d+)\*x', raw_schedule)
+        if interval_only_mat is not None:
+            g = interval_only_mat.groups()
+            start_hour, start_minute = 0, 0
+            interval_hour, interval_minute = int(g[0]), int(g[1])
         else:
-            sio.write('无\n')
-        return sio.getvalue()
+            mat = re.fullmatch(
+                r'(\d+):(\d+)\+(\d+):(\d+)\*x', raw_schedule)
+            if mat is not None:
+                g = mat.groups()
+                start_hour, start_minute = int(g[0]), int(g[1])
+                interval_hour, interval_minute = int(g[2]), int(g[3])
+            else:
+                raise BadRequestError(f'{raw_schedule}不是合法的时间')
+
+    if start_hour < 0 or start_hour >= 24 or start_minute < 0 or start_minute >= 60 \
+            or interval_hour < 0 or interval_minute >= 60 \
+            or (interval_hour > 0 and interval_minute < 0) or (interval_hour == 0 and interval_minute <= 0):
+        raise BadRequestError(f'{raw_schedule}不是合法的时间')
+
+    return start_hour, start_minute, interval_hour, interval_minute
+
+
+@context.register_eager_singleton()
+class Scheduler(IntervalTaskWorker[Subscription]):
+    tag = "scheduler"
+
+    @property
+    def repo(self) -> SubscriptionRepo:
+        return context.require(SubscriptionRepo)
 
-
-class ScheduleHandler(SubCommandHandler, subcommand='schedule', service=manage_schedule_service):
     @classmethod
-    def type(cls) -> str:
-        return "schedule"
-
-    async def parse_args(self, args: Sequence[str]) -> dict:
-        if len(args) < 2:
-            raise BadRequestError()
-        try:
-            return {"type": ScheduleType(args[0]),
-                    "schedule": args[1],
-                    "args": args[2:]}
-        except ValueError as e:
-            raise BadRequestError(f"未知订阅类型：{args[0]}") from e
-
-    # noinspection PyMethodOverriding
-    async def actual_handle(self, *, type: ScheduleType,
-                            schedule: str,
-                            args: Sequence[str]):
-        await scheduler.add_task(type, schedule, args, self.post_dest)
-        await self.post_plain_text(message="订阅成功")
-
-    async def actual_handle_bad_request(self, err: BadRequestError):
-        msg = ""
-        if err.message:
-            msg += err.message
-            msg += '\n'
-
-        msg += await build_subscriptions_msg(self.post_dest)
-        msg += "\n" \
-               f"命令格式：{default_command_start}pixivbot schedule <type> <schedule> [..args]\n" \
-               "参数：\n" \
-               "  <type>：可选值有random_bookmark, random_recommended_illust, random_illust, " \
-               "random_user_illust, ranking\n" \
-               "  <schedule>：格式为HH:mm（每日固定时间点推送）或HH:mm*x（间隔时间推送）\n" \
-               "  [...args]：根据<type>不同需要提供不同的参数\n" \
-               f"示例：{default_command_start}pixivbot schedule ranking 06:00*x day 1-5"
-        await self.post_plain_text(message=msg)
+    def _get_handler_type(cls, type: ScheduleType) -> Type["Handler"]:
+        from ..handler.schedule import SubscriptionRandomBookmarkHandler, SubscriptionRandomRecommendedIllustHandler, \
+            SubscriptionRankingHandler, SubscriptionRandomIllustHandler, SubscriptionRandomUserIllustHandler
+
+        if type == ScheduleType.random_bookmark:
+            return SubscriptionRandomBookmarkHandler
+        elif type == ScheduleType.random_recommended_illust:
+            return SubscriptionRandomRecommendedIllustHandler
+        elif type == ScheduleType.ranking:
+            return SubscriptionRankingHandler
+        elif type == ScheduleType.random_illust:
+            return SubscriptionRandomIllustHandler
+        elif type == ScheduleType.random_user_illust:
+            return SubscriptionRandomUserIllustHandler
+
+    async def _handle_trigger(self, item: Subscription):
+        handler_type = self._get_handler_type(item.type)
+        await handler_type(item.subscriber, silently=True).handle_with_parsed_args(**item.kwargs)
+
+    def _make_job_trigger(self, item: Subscription) -> IntervalTrigger:
+        offset_hour, offset_minute, hours, minutes = item.schedule
+        tz = pytz.timezone(item.tz)
+        return IntervalTrigger(hours=hours, minutes=minutes,
+                               start_date=datetime.now(tz).replace(hour=offset_hour,
+                                                                   minute=offset_minute,
+                                                                   second=0,
+                                                                   microsecond=0) + timedelta(days=-1))
+
+    async def _build_task(self, type_: ScheduleType,
+                          schedule: Union[str, Sequence[int]],
+                          args: Sequence[str],
+                          session: Session) -> Subscription:
+        if args is None:
+            args = []
+
+        if isinstance(schedule, str):
+            schedule = parse_schedule(schedule)
+
+        handler_type = self._get_handler_type(type_)
+        kwargs = handler_type(session).parse_args(args)
+        if isawaitable(kwargs):
+            kwargs = await kwargs
+
+        sub = Subscription(type=type_, kwargs=kwargs,
+                           subscriber=session,
+                           schedule=schedule)
+        return sub
+
+    @overload
+    async def add_task(self, type_: ScheduleType,
+                       schedule: Union[str, Sequence[int]],
+                       args: Sequence[str],
+                       session: Session) -> bool:
+        ...
 
+    async def add_task(self, *args, **kwargs) -> bool:
+        return await super().add_task(*args, **kwargs)
 
-class UnscheduleHandler(SubCommandHandler, subcommand='unschedule', service=manage_schedule_service):
-    @classmethod
-    def type(cls) -> str:
-        return "unschedule"
-
-    async def parse_args(self, args: Sequence[str]) -> dict:
-        if len(args) == 0:
-            raise BadRequestError()
-        return {"code": args[0]}
-
-    # noinspection PyMethodOverriding
-    async def actual_handle(self, *, code: str):
-        if code != "all":
-            ok = await scheduler.remove_task(self.post_dest, code)
-        else:
-            await scheduler.remove_all_by_subscriber(self.post_dest)
-            ok = True
-
-        if ok:
-            await self.post_plain_text(message="取消订阅成功")
-        else:
-            raise BadRequestError("取消订阅失败，不存在该订阅")
 
-    async def actual_handle_bad_request(self, err: BadRequestError):
-        msg = ""
-        if err.message:
-            msg += err.message
-            msg += '\n'
-
-        msg += await build_subscriptions_msg(self.post_dest)
-        msg += "\n"
-        msg += f"命令格式：{default_command_start}pixivbot unschedule <id>"
-        await self.post_plain_text(message=msg)
+__all__ = ("Scheduler",)
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/command/subcommand.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/command/subcommand.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import inspect
 from abc import ABC
 
-from nonebot_plugin_pixivbot.utils.errors import BadRequestError
 from .command import CommandHandler
 from ..base import Handler, HandlerMeta
+from ...utils.errors import BadRequestError
 
 
 class SubCommandHandlerMeta(HandlerMeta):
     def __new__(mcs, *args, **kwargs):
         subcommand = None
         if 'subcommand' in kwargs:
             subcommand = kwargs['subcommand']
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/command/watch.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/command/watch.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 from io import StringIO
 from typing import Sequence
 
-from nonebot_plugin_pixivbot.model import WatchType, T_UID, T_GID
-from nonebot_plugin_pixivbot.plugin_service import manage_watch_service
-from nonebot_plugin_pixivbot.protocol_dep.post_dest import PostDestination
-from nonebot_plugin_pixivbot.service.pixiv_service import PixivService
-from nonebot_plugin_pixivbot.service.watchman import Watchman
-from nonebot_plugin_pixivbot.utils.errors import BadRequestError
-from nonebot_plugin_pixivbot.utils.nonebot import default_command_start
+from nonebot_plugin_session import Session
+
 from .subcommand import SubCommandHandler
 from ..pkg_context import context
+from ...model import WatchType
+from ...plugin_service import manage_watch_service
+from ...service.pixiv_service import PixivService
+from ...service.watchman import Watchman
+from ...utils.errors import BadRequestError
+from ...utils.nonebot import default_command_start
 
 watchman = context.require(Watchman)
 pixiv = context.require(PixivService)
 
 
 async def parse_and_get_user(raw_user: str):
     # try parse
     try:
         user = int(raw_user)
         return await pixiv.get_user(user)
     except ValueError:
         return await pixiv.get_user(raw_user)
 
 
-async def build_tasks_msg(post_dest: PostDestination[T_UID, T_GID]):
-    tasks = [x async for x in watchman.get_by_subscriber(post_dest)]
+async def build_tasks_msg(session: Session):
+    tasks = [x async for x in watchman.get_by_subscriber(session)]
     with StringIO() as sio:
         sio.write("当前订阅：\n")
         if len(tasks) > 0:
             for t in tasks:
                 sio.write(f'[{t.code}] {t.type.name}')
                 args_text = t.args_text
                 if args_text:
@@ -48,24 +49,22 @@
 
     watch_args = {"user_id": user.id}
     message = f"{user.name}({user.id})老师的插画更新"
 
     return watch_args, message
 
 
-async def parse_following_illusts_args(args: Sequence[str], post_dest: PostDestination[T_UID, T_GID]):
+async def parse_following_illusts_args(args: Sequence[str]):
     if len(args) > 1:
         user = await parse_and_get_user(args[1])
 
-        watch_args = {"pixiv_user_id": user.id,
-                      "sender_user_id": post_dest.user_id}
+        watch_args = {"pixiv_user_id": user.id}
         message = f"{user.name}({user.id})用户的关注者插画更新"
     else:
-        watch_args = {"pixiv_user_id": 0,
-                      "sender_user_id": post_dest.user_id}
+        watch_args = {"pixiv_user_id": 0}
         message = "关注者插画更新"
 
     return watch_args, message
 
 
 class WatchHandler(SubCommandHandler, subcommand='watch', service=manage_watch_service):
 
@@ -84,47 +83,47 @@
                     "code": args[1]}
 
         try:
             type = WatchType[args[0]]
             if type == WatchType.user_illusts:
                 watch_kwargs, message = await parse_user_illusts_args(args)
             elif type == WatchType.following_illusts:
-                watch_kwargs, message = await parse_following_illusts_args(args, self.post_dest)
+                watch_kwargs, message = await parse_following_illusts_args(args)
             else:
                 raise KeyError()
         except KeyError as e:
             raise BadRequestError(f"未知订阅类型：{args[0]}") from e
 
         return {"operation": "add",
                 "type": type,
                 "watch_kwargs": watch_kwargs,
                 "success_message": "成功订阅" + message}
 
     # noinspection PyMethodOverriding
     async def actual_handle(self, *, operation: str, **kwargs):
         if operation == 'fetch':
-            ok = await watchman.fetch(kwargs['code'], self.post_dest)
+            ok = await watchman.fetch(kwargs['code'], self.session)
             if ok:
                 await self.post_plain_text("拉取完毕")
             else:
                 raise BadRequestError("不存在该订阅")
         elif operation == 'add':
-            ok = await watchman.add_task(kwargs['type'], kwargs['watch_kwargs'], self.post_dest)
+            ok = await watchman.add_task(kwargs['type'], kwargs['watch_kwargs'], self.session)
             if ok:
                 await self.post_plain_text(kwargs['success_message'])
             else:
                 raise BadRequestError("该订阅已存在")
 
     async def actual_handle_bad_request(self, err: BadRequestError):
         msg = ""
         if err.message:
             msg += err.message
             msg += '\n\n'
 
-        msg += await build_tasks_msg(self.post_dest)
+        msg += await build_tasks_msg(self.session)
         msg += "\n" \
                f"命令格式：{default_command_start}pixivbot watch <type> [..args]\n" \
                "参数：\n" \
                "  <type>：可选值有user_illusts, following_illusts\n" \
                "  [...args]：根据<type>不同需要提供不同的参数\n" \
                f"示例：{default_command_start}pixivbot watch user_illusts <用户名>\n"
         await self.post_plain_text(message=msg)
@@ -139,27 +138,27 @@
         if len(args) == 0:
             raise BadRequestError()
         return {"code": args[0]}
 
     # noinspection PyMethodOverriding
     async def actual_handle(self, *, code: str):
         if code != "all":
-            ok = await watchman.remove_task(self.post_dest, code)
+            ok = await watchman.remove_task(self.session, code)
         else:
-            await watchman.remove_all_by_subscriber(self.post_dest)
+            await watchman.remove_all_by_subscriber(self.session)
             ok = True
 
         if ok:
             await self.post_plain_text(message="取消订阅成功")
         else:
             raise BadRequestError("取消订阅失败，不存在该订阅")
 
     async def actual_handle_bad_request(self, err: BadRequestError):
         msg = ""
         if err.message:
             msg += err.message
             msg += '\n'
 
-        msg += await build_tasks_msg(self.post_dest)
+        msg += await build_tasks_msg(self.session)
         msg += "\n"
         msg += f"命令格式：{default_command_start}pixivbot unwatch <id>"
         await self.post_plain_text(message=msg)
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/common/__init__.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/common/base.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/common/illust.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/illust.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from typing import Generic, Sequence
+from typing import Sequence
 
 from nonebot import on_regex
+from nonebot.internal.adapter import Event
 from nonebot.internal.params import Depends
 from nonebot.params import RegexGroup
+from nonebot_plugin_session import extract_session
 
-from nonebot_plugin_pixivbot.model import T_UID, T_GID
-from nonebot_plugin_pixivbot.plugin_service import illust_service
-from nonebot_plugin_pixivbot.utils.errors import BadRequestError
 from .base import CommonHandler
 from ..pkg_context import context
 from ..utils import get_common_query_rule
 from ...config import Config
-from ...protocol_dep.post_dest import post_destination
+from ...plugin_service import illust_service
 from ...service.pixiv_service import PixivService
+from ...utils.errors import BadRequestError
 
 conf = context.require(Config)
 service = context.require(PixivService)
 
 
-class IllustHandler(CommonHandler, Generic[T_UID, T_GID], service=illust_service):
+class IllustHandler(CommonHandler, service=illust_service):
     @classmethod
     def type(cls) -> str:
         return "illust"
 
     @classmethod
     def enabled(cls) -> bool:
         return conf.pixiv_illust_query_enabled
@@ -36,11 +36,12 @@
     # noinspection PyMethodOverriding
     async def actual_handle(self, illust_id: int):
         illust = await service.illust_detail(illust_id)
         await self.post_illust(illust)
 
 
 @on_regex(r"^看看图\s*([1-9][0-9]*)$", rule=get_common_query_rule(), priority=5).handle()
-async def on_match(matched_groups=RegexGroup(),
-                   post_dest=Depends(post_destination)):
+async def _(event: Event,
+            session=Depends(extract_session),
+            matched_groups=RegexGroup()):
     illust_id = matched_groups[0]
-    await IllustHandler(post_dest).handle(illust_id)
+    await IllustHandler(session, event).handle(illust_id)
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/common/more.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/random_recommended_illust.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from nonebot import on_regex
+from nonebot.internal.adapter import Event
 from nonebot.internal.params import Depends
-from nonebot.params import RegexGroup
+from nonebot_plugin_session import extract_session
 
-from nonebot_plugin_pixivbot.plugin_service import more_service
-from nonebot_plugin_pixivbot.protocol_dep.post_dest import post_destination
-from nonebot_plugin_pixivbot.utils.errors import BadRequestError
-from .base import CommonHandler
+from .base import RecordCommonHandler
 from ..pkg_context import context
-from ..recorder import Recorder
-from ..utils import get_common_query_rule, get_count
+from ..utils import get_common_query_rule, ArgCount
 from ...config import Config
+from ...plugin_service import random_recommended_illust_service
+from ...service.pixiv_service import PixivService
 
-recorder = context.require(Recorder)
 conf = context.require(Config)
+service = context.require(PixivService)
 
 
-class MoreHandler(CommonHandler, service=more_service):
+class RandomRecommendedIllustHandler(RecordCommonHandler, service=random_recommended_illust_service):
     @classmethod
     def type(cls) -> str:
-        return "more"
+        return "random_recommended_illust"
 
     @classmethod
     def enabled(cls) -> bool:
-        return conf.pixiv_more_enabled
+        return conf.pixiv_random_recommended_illust_query_enabled
 
-    async def actual_handle(self, count: int = 1):
-        req = recorder.get_req(self.post_dest.identifier)
-        if not req:
-            raise BadRequestError("你还没有发送过请求")
-
-        handler = req.handler_type(self.post_dest, silently=self.silently, disable_interceptors=True)
-        await handler.handle(*req.args, **{**req.kwargs, "count": count})
-
-
-@on_regex("^还要((.*)张)?$", rule=get_common_query_rule(), priority=1, block=True).handle()
-async def on_match(matched_groups=RegexGroup(),
-                   post_dest=Depends(post_destination)):
-    await MoreHandler(post_dest).handle(count=get_count(matched_groups, 1))
+    async def actual_handle(self, *, count: int = 1):
+        illusts = await service.random_recommended_illust(count=count,
+                                                          exclude_r18=(not await self.is_r18_allowed()),
+                                                          exclude_r18g=(not await self.is_r18g_allowed()))
+
+        await self.post_illusts(illusts,
+                                header="这是您点的图")
+
+
+@on_regex("^来(.*)?张图$", rule=get_common_query_rule(), priority=3, block=True).handle()
+async def _(event: Event,
+            session=Depends(extract_session),
+            count=ArgCount()):
+    await RandomRecommendedIllustHandler(session, event).handle(count=count)
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/common/random_bookmark.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/random_bookmark.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from typing import Sequence
 
 from nonebot import on_regex
+from nonebot.internal.adapter import Event
 from nonebot.internal.params import Depends
-from nonebot.params import RegexGroup
+from nonebot_plugin_session import extract_session
 
-from nonebot_plugin_pixivbot.model import T_UID
-from nonebot_plugin_pixivbot.plugin_service import random_bookmark_service
-from nonebot_plugin_pixivbot.service.pixiv_account_binder import PixivAccountBinder
-from nonebot_plugin_pixivbot.utils.errors import BadRequestError
 from .base import RecordCommonHandler
 from ..pkg_context import context
-from ..utils import get_common_query_rule, get_count
+from ..utils import get_common_query_rule, ArgCount
 from ...config import Config
-from ...protocol_dep.post_dest import post_destination
+from ...plugin_service import random_bookmark_service
+from ...service.pixiv_account_binder import PixivAccountBinder
 from ...service.pixiv_service import PixivService
+from ...utils.errors import BadRequestError
 
 conf = context.require(Config)
 binder = context.require(PixivAccountBinder)
 service = context.require(PixivService)
 
 
 class RandomBookmarkHandler(RecordCommonHandler, service=random_bookmark_service):
@@ -27,31 +26,29 @@
 
     @classmethod
     def enabled(cls) -> bool:
         return conf.pixiv_random_bookmark_query_enabled
 
     async def parse_args(self, args: Sequence[str]) -> dict:
         pixiv_user_id = 0
-        sender_user_id = self.post_dest.user_id
 
         if len(args) > 0:
             try:
                 pixiv_user_id = int(args[0])
             except ValueError:
                 raise BadRequestError(f"{args[0]}不是合法的ID")
 
-        # 因为群组的订阅会把PostIdentifier的user_id抹去，所以这里必须传递sender_user_id
-        return {"pixiv_user_id": pixiv_user_id, "sender_user_id": sender_user_id}
+        return {"pixiv_user_id": pixiv_user_id, "sender_user_id": self.session.id1}
 
     # noinspection PyMethodOverriding
-    async def actual_handle(self, *, sender_user_id: T_UID,
-                            pixiv_user_id: int = 0,
+    async def actual_handle(self, *, pixiv_user_id: int = 0,
+                            sender_user_id: int = 0,
                             count: int = 1):
         if not pixiv_user_id and sender_user_id:
-            pixiv_user_id = await binder.get_binding(self.post_dest.adapter, sender_user_id)
+            pixiv_user_id = await binder.get_binding(self.session.platform, sender_user_id)
 
         if not pixiv_user_id:
             pixiv_user_id = conf.pixiv_random_bookmark_user_id
 
         if not pixiv_user_id:
             raise BadRequestError("无效的Pixiv账号，或未绑定Pixiv账号")
 
@@ -60,10 +57,11 @@
                                                 exclude_r18g=(not await self.is_r18g_allowed()))
 
         await self.post_illusts(illusts,
                                 header="这是您点的私家车")
 
 
 @on_regex("^来(.*)?张私家车$", rule=get_common_query_rule(), priority=5).handle()
-async def on_match(matched_groups=RegexGroup(),
-                   post_dest=Depends(post_destination)):
-    await RandomBookmarkHandler(post_dest).handle(count=get_count(matched_groups))
+async def _(event: Event,
+            session=Depends(extract_session),
+            count=ArgCount()):
+    await RandomBookmarkHandler(session, event).handle(count=count)
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/common/random_illust.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/random_illust.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import Sequence
 
 from nonebot import on_regex
+from nonebot.internal.adapter import Event
 from nonebot.internal.params import Depends
 from nonebot.params import RegexGroup
+from nonebot_plugin_session import extract_session
 
-from nonebot_plugin_pixivbot.plugin_service import random_illust_service
-from nonebot_plugin_pixivbot.protocol_dep.post_dest import post_destination
 from .base import RecordCommonHandler
 from ..pkg_context import context
-from ..utils import get_common_query_rule, get_count
+from ..utils import get_common_query_rule, ArgCount
 from ...config import Config
+from ...plugin_service import random_illust_service
 from ...service.pixiv_service import PixivService
 
 conf = context.require(Config)
 service = context.require(PixivService)
 
 
 class RandomIllustHandler(RecordCommonHandler, service=random_illust_service):
@@ -36,11 +37,13 @@
                                               exclude_r18g=(not await self.is_r18g_allowed()))
 
         await self.post_illusts(illusts,
                                 header=f"这是您点的{word}图")
 
 
 @on_regex("^来(.*)?张(.+)图$", rule=get_common_query_rule(), priority=5).handle()
-async def on_match(matched_groups=RegexGroup(),
-                   post_dest=Depends(post_destination)):
+async def _(event: Event,
+            matched_groups=RegexGroup(),
+            session=Depends(extract_session),
+            count=ArgCount()):
     word = matched_groups[1]
-    await RandomIllustHandler(post_dest).handle(word, count=get_count(matched_groups))
+    await RandomIllustHandler(session, event).handle(word, count=count)
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/common/random_related_illust.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/random_related_illust.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import Sequence
 
 from nonebot import on_regex
+from nonebot.internal.adapter import Event
 from nonebot.internal.params import Depends
+from nonebot_plugin_session import extract_session
 
-from nonebot_plugin_pixivbot.plugin_service import random_related_illust_service
-from nonebot_plugin_pixivbot.protocol_dep.post_dest import post_destination
-from nonebot_plugin_pixivbot.utils.errors import BadRequestError
 from .base import RecordCommonHandler
 from ..pkg_context import context
 from ..recorder import Recorder
 from ..utils import get_common_query_rule
 from ...config import Config
+from ...plugin_service import random_related_illust_service
 from ...service.pixiv_service import PixivService
+from ...utils.errors import BadRequestError
 
 conf = context.require(Config)
 service = context.require(PixivService)
 recorder = context.require(Recorder)
 
 
 class RandomRelatedIllustHandler(RecordCommonHandler, service=random_related_illust_service):
@@ -24,15 +25,15 @@
         return "random_related_illust"
 
     @classmethod
     def enabled(cls) -> bool:
         return conf.pixiv_random_related_illust_query_enabled
 
     async def parse_args(self, args: Sequence[str]) -> dict:
-        illust_id = recorder.get_resp(self.post_dest.identifier)
+        illust_id = recorder.get_resp(self.session)
         if not illust_id:
             raise BadRequestError("你还没有发送过请求")
         return {"illust_id": illust_id}
 
     # noinspection PyMethodOverriding
     async def actual_handle(self, *, illust_id: int,
                             count: int = 1):
@@ -41,9 +42,10 @@
                                                       exclude_r18g=(not await self.is_r18g_allowed()))
 
         await self.post_illusts(illusts,
                                 header=f"这是您点的[{illust_id}]的相关图片")
 
 
 @on_regex("^不够色$", rule=get_common_query_rule(), priority=1, block=True).handle()
-async def on_match(post_dest=Depends(post_destination)):
-    await RandomRelatedIllustHandler(post_dest).handle()
+async def _(event: Event,
+            session=Depends(extract_session)):
+    await RandomRelatedIllustHandler(session, event).handle()
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/common/random_user_illust.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/random_user_illust.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import Sequence
 from typing import Union
 
 from nonebot import on_regex
+from nonebot.internal.adapter import Event
 from nonebot.internal.params import Depends
 from nonebot.params import RegexGroup
+from nonebot_plugin_session import extract_session
 
 from nonebot_plugin_pixivbot.plugin_service import random_user_illust_service
-from nonebot_plugin_pixivbot.protocol_dep.post_dest import post_destination
 from .base import RecordCommonHandler
 from ..pkg_context import context
-from ..utils import get_common_query_rule, get_count
+from ..utils import get_common_query_rule, ArgCount
 from ...config import Config
 from ...service.pixiv_service import PixivService
 
 conf = context.require(Config)
 service = context.require(PixivService)
 
 
@@ -42,11 +43,13 @@
                                                              exclude_r18g=(not await self.is_r18g_allowed()))
 
         await self.post_illusts(illusts,
                                 header=f"这是您点的{userinfo.name}({userinfo.id})老师的图")
 
 
 @on_regex("^来(.*)?张(.+)老师的图$", rule=get_common_query_rule(), priority=4, block=True).handle()
-async def on_match(matched_groups=RegexGroup(),
-                   post_dest=Depends(post_destination)):
+async def _(event: Event,
+            matched_groups=RegexGroup(),
+            session=Depends(extract_session),
+            count=ArgCount()):
     user = matched_groups[1]
-    await RandomUserIllustHandler(post_dest).handle(user, count=get_count(matched_groups))
+    await RandomUserIllustHandler(session, event).handle(user, count=count)
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/common/ranking.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/ranking.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 
 from nonebot import on_regex
+from nonebot.internal.adapter import Event
 from nonebot.internal.params import Depends
 from nonebot.params import RegexGroup
-from nonebot.typing import T_State
+from nonebot_plugin_session import extract_session
 
-from nonebot_plugin_pixivbot.enums import RankingMode
-from nonebot_plugin_pixivbot.plugin_service import ranking_service
-from nonebot_plugin_pixivbot.utils.decode_integer import decode_integer
-from nonebot_plugin_pixivbot.utils.errors import BadRequestError
 from .base import CommonHandler
 from ..pkg_context import context
 from ..utils import get_common_query_rule
 from ...config import Config
-from ...protocol_dep.post_dest import post_destination
+from ...enums import RankingMode
+from ...plugin_service import ranking_service
 from ...service.pixiv_service import PixivService
+from ...utils.decode_integer import decode_integer
+from ...utils.errors import BadRequestError
 
 conf = context.require(Config)
 service = context.require(PixivService)
 
 
 class RankingHandler(CommonHandler, service=ranking_service):
     @classmethod
@@ -95,16 +95,17 @@
         illusts = await service.illust_ranking(mode, range)
         await self.post_illusts(illusts,
                                 header=f"这是您点的{self.mode_mapping[mode]}榜",
                                 number=range[0])
 
 
 @on_regex(r"^看看(.*)?榜\s*(.*)?$", rule=get_common_query_rule(), priority=4, block=True).handle()
-async def on_match(matched_groups=RegexGroup(),
-                   post_dest=Depends(post_destination)):
+async def on_match(event: Event,
+                   matched_groups=RegexGroup(),
+                   session=Depends(extract_session)):
     if matched_groups:
         mode = matched_groups[0]
         num = matched_groups[1]
     else:
         mode = None
         num = None
-    await RankingHandler(post_dest).handle(mode, num)
+    await RankingHandler(session, event).handle(mode, num)
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/interceptor/combined_interceptor.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/combined_interceptor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from functools import partial
 from typing import Callable, Type, Optional, Iterable, TYPE_CHECKING
 
 from .base import Interceptor
 
 if TYPE_CHECKING:
-    from nonebot_plugin_pixivbot.handler.base import Handler
+    from ..base import Handler
 
 
 class CombinedInterceptor(Interceptor):
     def __init__(self, x: Interceptor, y: Interceptor):
         self.x = x
         self.y = y
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/interceptor/default_error_interceptor.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/default_error_interceptor.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pixivpy_async.error import NoTokenError
 
 from nonebot_plugin_pixivbot.utils.errors import BadRequestError, QueryError, RateLimitError
 from .base import Interceptor
 from ..pkg_context import context
 
 if TYPE_CHECKING:
-    from nonebot_plugin_pixivbot.handler.base import Handler
+    from ..base import Handler
 
 
 @context.register_singleton()
 class DefaultErrorInterceptor(Interceptor):
     async def intercept(self, handler: "Handler", wrapped_func: Callable, *args, **kwargs):
         try:
             await wrapped_func(*args, **kwargs)
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/interceptor/loading_prompt_interceptor.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/loading_prompt_interceptor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,35 @@
-from asyncio import create_task, sleep, shield, Task
+from asyncio import create_task, sleep, shield, Task, CancelledError
 from typing import Callable, Optional, TYPE_CHECKING
 
 from nonebot import logger
 
-from nonebot_plugin_pixivbot.config import Config
 from .base import Interceptor
 from ..pkg_context import context
+from ...config import Config
 
 if TYPE_CHECKING:
-    from nonebot_plugin_pixivbot.handler.base import Handler
+    from ..base import Handler
 
 conf = context.require(Config)
 
 
 @context.register_singleton()
 class LoadingPromptInterceptor(Interceptor):
 
     async def send_delayed_loading_prompt(self, handler: "Handler"):
-        await sleep(conf.pixiv_loading_prompt_delayed_time)
+        try:
+            await sleep(conf.pixiv_loading_prompt_delayed_time)
 
-        logger.debug(f"send delayed loading to {handler.post_dest.identifier}")
-        await shield(handler.post_plain_text("努力加载中"))
+            logger.debug(f"send delayed loading")
+            await shield(handler.post_plain_text("努力加载中"))
+        except CancelledError as e:
+            raise e
+        except BaseException as e:
+            logger.exception(e)
 
     async def intercept(self, handler: "Handler", wrapped_func: Callable, *args, **kwargs):
         task: Optional[Task] = None
         if not handler.silently:
             task = create_task(self.send_delayed_loading_prompt(handler))
 
         try:
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/interceptor/permission_interceptor.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/permission_interceptor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from abc import ABC, abstractmethod
 from typing import Callable, Optional, TYPE_CHECKING
 
-from nonebot import get_driver, logger
+from nonebot import logger
+from nonebot_plugin_access_control.subject import extract_subjects_from_session
 
 from .base import Interceptor
 from ..pkg_context import context
 
 if TYPE_CHECKING:
-    from nonebot_plugin_pixivbot.handler.base import Handler
+    from ..base import Handler
 
 
 class PermissionInterceptor(Interceptor, ABC):
     @abstractmethod
     async def has_permission(self, handler: "Handler") -> bool:
         raise NotImplementedError()
 
@@ -20,15 +21,15 @@
 
     async def intercept(self, handler: "Handler", wrapped_func: Callable, *args, **kwargs):
         p = await self.has_permission(handler)
 
         if p:
             await wrapped_func(*args, **kwargs)
         else:
-            logger.debug(f"permission denied {handler.post_dest}")
+            logger.debug(f"permission denied")
             if not handler.silently:
                 msg = await self.get_permission_denied_msg(handler)
                 if msg:
                     await handler.post_plain_text(msg)
 
 
 class AnyPermissionInterceptor(PermissionInterceptor):
@@ -47,10 +48,9 @@
 
         return False
 
 
 @context.register_singleton()
 class SuperuserInterceptor(PermissionInterceptor):
     async def has_permission(self, handler: "Handler") -> bool:
-        superusers = get_driver().config.superusers
-        return str(handler.post_dest.user_id) in superusers \
-               or f"{handler.post_dest.adapter}:{handler.post_dest.user_id}" in superusers
+        sbj = extract_subjects_from_session(handler.session)
+        return "superuser" in sbj
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/interceptor/record_req_interceptor.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/record_req_interceptor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Callable, TYPE_CHECKING
 
-from nonebot_plugin_pixivbot.handler.interceptor.base import Interceptor
-from nonebot_plugin_pixivbot.handler.recorder import Recorder, Req
+from .base import Interceptor
 from ..pkg_context import context
+from ..recorder import Recorder, Req
 
 if TYPE_CHECKING:
-    from nonebot_plugin_pixivbot.handler.base import Handler
+    from ..base import Handler
 
 recorder = context.require(Recorder)
 
 
 @context.register_singleton()
 class RecordReqInterceptor(Interceptor):
     async def intercept(self, handler: "Handler", wrapped_func: Callable, *args, **kwargs):
         await wrapped_func(*args, **kwargs)
-        recorder.record_req(Req(type(handler), args, kwargs), handler.post_dest.identifier)
+        recorder.record_req(Req(type(handler), args, kwargs), handler.session)
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/interceptor/timeout_interceptor.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/timeout_interceptor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from asyncio import wait_for
 from typing import Callable, TYPE_CHECKING
 
-from nonebot_plugin_pixivbot.config import Config
-from nonebot_plugin_pixivbot.handler.interceptor.base import Interceptor
+from .base import Interceptor
 from ..pkg_context import context
+from ...config import Config
 
 if TYPE_CHECKING:
     from nonebot_plugin_pixivbot.handler.base import Handler
 
 conf = context.require(Config)
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/recorder.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/recorder.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 from typing import Optional, TYPE_CHECKING, Mapping, Any, Type, NamedTuple, Sequence
 
 from cachetools import TTLCache
+from nonebot.internal.adapter import Event
+from nonebot_plugin_session import Session, SessionIdType
 
-from nonebot_plugin_pixivbot.config import Config
-from nonebot_plugin_pixivbot.model import PostIdentifier, T_UID, T_GID
-from nonebot_plugin_pixivbot.model.message import IllustMessagesModel
-from nonebot_plugin_pixivbot.protocol_dep.post_dest import PostDestination
-from nonebot_plugin_pixivbot.protocol_dep.postman import PostmanManager
 from .pkg_context import context
+from ..config import Config
+from ..model.message import IllustMessagesModel
+from ..service.postman import Postman
 
 if TYPE_CHECKING:
     from .base import Handler
 
 conf = context.require(Config)
 
 
@@ -27,68 +27,56 @@
     illust_id: int
 
 
 @context.root.register_singleton()
 class Recorder:
     def __init__(self, max_req_size: int = 65535,
                  max_resp_size: int = 65535):
-        self._reqs = TTLCache[PostIdentifier[T_UID, T_GID], Req](maxsize=max_req_size,
-                                                                 ttl=conf.pixiv_query_expires_in)
-        self._resps = TTLCache[PostIdentifier[T_UID, T_GID], Resp](maxsize=max_resp_size,
-                                                                   ttl=conf.pixiv_query_expires_in)
+        self._reqs = TTLCache[str, Req](maxsize=max_req_size,
+                                        ttl=conf.pixiv_query_expires_in)
+        self._resps = TTLCache[str, Resp](maxsize=max_resp_size,
+                                          ttl=conf.pixiv_query_expires_in)
 
         self.max_req_size = max_req_size
         self.max_resp_size = max_resp_size
 
-    @staticmethod
-    def _key_fallback(key: PostIdentifier[T_UID, T_GID]) -> Optional[PostIdentifier[T_UID, T_GID]]:
-        if key.user_id is not None and key.group_id is not None:
-            return PostIdentifier[T_UID, T_GID](key.adapter, None, key.group_id)
-        else:
-            return None
-
-    def record_req(self, record: Req, key: PostIdentifier[T_UID, T_GID]):
+    def record_req(self, record: Req, session: Session):
+        key = session.get_id(SessionIdType.GROUP)
         self._reqs[key] = record
 
-    def get_req(self, key: PostIdentifier[T_UID, T_GID]) -> Optional[Req]:
+    def get_req(self, session: Session) -> Optional[Req]:
+        key = session.get_id(SessionIdType.GROUP)
         if key in self._reqs:
             req = self._reqs[key]
             return req
         else:
-            key = self._key_fallback(key)
-            if key is not None:
-                return self.get_req(key)
-            else:
-                return None
+            return None
 
-    def record_resp(self, illust_id: int, key: PostIdentifier[T_UID, T_GID]):
+    def record_resp(self, illust_id: int, session: Session):
+        key = session.get_id(SessionIdType.GROUP)
         self._resps[key] = Resp(illust_id)
 
-    def get_resp(self, key: PostIdentifier[T_UID, T_GID]) -> Optional[int]:
+    def get_resp(self, session: Session) -> Optional[int]:
+        key = session.get_id(SessionIdType.GROUP)
         if key in self._resps:
             rec = self._resps[key]
             return rec.illust_id
         else:
-            key = self._key_fallback(key)
-            if key is not None:
-                return self.get_resp(key)
-            else:
-                return None
+            return None
 
 
-origin_postman_mgr = context.require(PostmanManager)
+origin_postman = context.require(Postman)
 
 
-@context.bind_singleton_to(PostmanManager, origin_postman_mgr)
-class RecordPostmanManager:
-    def __init__(self, delegation: PostmanManager):
+@context.bind_singleton_to(Postman, origin_postman)
+class RecordPostman:
+    def __init__(self, delegation: Postman):
         self.delegation = delegation
 
-    async def send_illusts(self, model: IllustMessagesModel,
-                           *, post_dest: PostDestination[T_UID, T_GID]):
+    async def post_illusts(self, model: IllustMessagesModel, session: Session, event: Optional[Event] = None):
         recorder = context.require(Recorder)
-        await self.delegation.send_illusts(model, post_dest=post_dest)
+        await self.delegation.post_illusts(model, session, event)
         if len(model.messages) == 1:
-            recorder.record_resp(model.messages[0].id, post_dest.identifier)
+            recorder.record_resp(model.messages[0].id, session)
 
     def __getattr__(self, name: str):
         return getattr(self.delegation, name)
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/sniffer/illust_link.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/sniffer/illust_link.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from nonebot import on_regex
+from nonebot.internal.adapter import Event
 from nonebot.internal.params import Depends
 from nonebot.params import RegexGroup
+from nonebot_plugin_session import extract_session
 
-from nonebot_plugin_pixivbot.protocol_dep.post_dest import post_destination
 from ..common import IllustHandler
 from ..pkg_context import context
 from ..utils import get_common_query_rule
 from ...config import Config
 from ...plugin_service import illust_link_service
 
 conf = context.require(Config)
@@ -20,11 +21,12 @@
     @classmethod
     def enabled(cls) -> bool:
         return conf.pixiv_illust_sniffer_enabled
 
 
 @on_regex(r"^(http://|https://)?(www.)?pixiv\.net/artworks/([1-9][0-9]*)/?$", rule=get_common_query_rule(),
           priority=5).handle()
-async def on_match(matched_groups=RegexGroup(),
-                   post_dest=Depends(post_destination)):
+async def _(event: Event,
+            matched_groups=RegexGroup(),
+            session=Depends(extract_session)):
     illust_id = matched_groups[2]
-    await IllustLinkHandler(post_dest).handle(illust_id)
+    await IllustLinkHandler(session, event).handle(illust_id)
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/utils.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-from nonebot import Bot
-from nonebot.internal.adapter import Event
+from nonebot.internal.params import Depends
+from nonebot.params import RegexGroup
 from nonebot.rule import to_me
 
 from nonebot_plugin_pixivbot.config import Config
 from nonebot_plugin_pixivbot.global_context import context
-from nonebot_plugin_pixivbot.protocol_dep.post_dest import PostDestinationFactoryManager
 from nonebot_plugin_pixivbot.utils.decode_integer import decode_integer
 from nonebot_plugin_pixivbot.utils.errors import BadRequestError
 
 
-def get_count(matched_groups, pos: int = 0):
-    count = 1
-    if matched_groups:
-        raw_count = matched_groups[pos]
-        if raw_count:
-            try:
-                count = decode_integer(raw_count)
-            except:
-                raise BadRequestError(f"{raw_count}不是合法的数字")
-    return count
+def ArgCount(pos: int = 0):
+    def dep(matched_groups=RegexGroup()):
+        count = 1
+        if matched_groups:
+            raw_count = matched_groups[pos]
+            if raw_count:
+                try:
+                    count = decode_integer(raw_count)
+                except ValueError:
+                    raise BadRequestError(f"{raw_count}不是合法的数字")
+        return count
+
+    return Depends(dep)
 
 
 def get_common_query_rule():
     if context.require(Config).pixiv_query_to_me_only:
         rule = to_me()
     else:
         rule = None
@@ -33,12 +35,8 @@
     if context.require(Config).pixiv_command_to_me_only:
         rule = to_me()
     else:
         rule = None
     return rule
 
 
-def get_post_dest(bot: Bot, event: Event):
-    return context.require(PostDestinationFactoryManager).from_event(bot, event)
-
-
 __all__ = ("get_count", "get_common_query_rule", "get_command_rule", "get_post_dest")
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/watch/base.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/watch/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/watch/following_illusts.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/watch/following_illusts.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import time
 
 from nonebot import logger
 
-from nonebot_plugin_pixivbot.data.pixiv_repo import PixivRepo
-from nonebot_plugin_pixivbot.data.pixiv_repo.enums import CacheStrategy
-from nonebot_plugin_pixivbot.handler.watch.base import WatchTaskHandler
-from nonebot_plugin_pixivbot.model import WatchTask, Illust
-from nonebot_plugin_pixivbot.service.pixiv_account_binder import PixivAccountBinder
-from nonebot_plugin_pixivbot.utils.shared_agen import SharedAsyncGeneratorManager
+from .base import WatchTaskHandler
 from ..pkg_context import context
 from ...config import Config
+from ...data.pixiv_repo import PixivRepo
+from ...data.pixiv_repo.enums import CacheStrategy
+from ...model import WatchTask, Illust
+from ...service.pixiv_account_binder import PixivAccountBinder
+from ...utils.shared_agen import SharedAsyncGeneratorManager
 
 conf = context.require(Config)
 binder = context.require(PixivAccountBinder)
 pixiv = context.require(PixivRepo)
 
 
 # 因为要强制从远端获取，所以用这个shared_agen_mgr来缓存
@@ -37,21 +37,21 @@
 
     # noinspection PyMethodOverriding
     async def actual_handle(self, *, task: WatchTask):
         pixiv_user_id = task.kwargs.get("pixiv_user_id", 0)
         sender_user_id = task.kwargs.get("sender_user_id", 0)
 
         if not pixiv_user_id and sender_user_id:
-            pixiv_user_id = await binder.get_binding(self.post_dest.adapter, sender_user_id)
+            pixiv_user_id = await binder.get_binding(task.subscriber.platform, sender_user_id)
 
         if not pixiv_user_id:
             pixiv_user_id = conf.pixiv_random_bookmark_user_id
 
         if not pixiv_user_id:
-            logger.warning(f"[watchman] no binding found for {self.post_dest}")
+            logger.warning(f"[watchman] no binding found for {task.subscriber.id1}")
             return
 
         async with shared_agen_mgr.get(pixiv_user_id) as illusts:
             async for illust in illusts:
                 if illust.create_date <= task.checkpoint:
                     break
                 logger.info(f"[watchman] send illust {illust.id} to {task.subscriber}")
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/handler/watch/user_illusts.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/watch/user_illusts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import time
 
 from nonebot import logger
 
-from nonebot_plugin_pixivbot.data.pixiv_repo import PixivRepo
-from nonebot_plugin_pixivbot.data.pixiv_repo.enums import CacheStrategy
-from nonebot_plugin_pixivbot.data.pixiv_repo.remote_repo import RemotePixivRepo
-from nonebot_plugin_pixivbot.model import WatchTask, Illust
-from nonebot_plugin_pixivbot.utils.shared_agen import SharedAsyncGeneratorManager
 from .base import WatchTaskHandler
 from ..pkg_context import context
+from ...data.pixiv_repo import PixivRepo
+from ...data.pixiv_repo.enums import CacheStrategy
+from ...data.pixiv_repo.remote_repo import RemotePixivRepo
+from ...model import WatchTask, Illust
+from ...utils.shared_agen import SharedAsyncGeneratorManager
 
 pixiv = context.require(PixivRepo)
 remote_pixiv = context.require(RemotePixivRepo)
 
 
 # 因为要强制从远端获取，所以用这个shared_agen_mgr来缓存
 class WatchUserIllustsSharedAsyncGeneratorManager(SharedAsyncGeneratorManager[int, Illust]):
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/model/illust.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/illust.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/model/message/illust_message.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/message/illust_message.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from io import BytesIO
 from typing import Optional
 
 from pydantic import BaseModel
 from tzlocal import get_localzone
 
-from nonebot_plugin_pixivbot.config import Config
-from nonebot_plugin_pixivbot.data.pixiv_repo import PixivRepo
-from nonebot_plugin_pixivbot.enums import BlockAction
-from nonebot_plugin_pixivbot.global_context import context
-from nonebot_plugin_pixivbot.model import Illust
+from .. import Illust
+from ...config import Config
+from ...data.pixiv_repo import PixivRepo
+from ...enums import BlockAction
+from ...global_context import context
 
 conf = context.require(Config)
 
 
 async def download_image(illust: Illust, page: int):
     with BytesIO() as bio:
         repo = context.require(PixivRepo)
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/model/message/illust_messages.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/message/illust_messages.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from asyncio import create_task, gather
 from typing import Optional, Sequence
 
 from pydantic import BaseModel
 
-from nonebot_plugin_pixivbot.model import Illust
-from nonebot_plugin_pixivbot.model.message.illust_message import IllustMessageModel
+from .illust_message import IllustMessageModel
+from .. import Illust
 
 
 class IllustMessagesModel(BaseModel):
     header: Optional[str] = None
     messages: Sequence[IllustMessageModel]
 
     @staticmethod
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/model/subscription.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/subscription.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from enum import Enum
-from typing import Sequence, Dict, Any, Generic
+from typing import Sequence, Dict, Any
 
 import tzlocal
 
-from . import T_UID, T_GID
 from .interval_task import IntervalTask
 from ..utils.format import format_kwargs
 
 
 class ScheduleType(str, Enum):
     random_bookmark = "random_bookmark"
     random_recommended_illust = "random_recommended_illust"
     random_illust = "random_illust"
     random_user_illust = "random_user_illust"
     ranking = "ranking"
 
 
-class Subscription(IntervalTask[T_UID, T_GID], Generic[T_UID, T_GID]):
+class Subscription(IntervalTask):
     type: ScheduleType
     kwargs: Dict[str, Any]
     schedule: Sequence[int]
     tz: str = tzlocal.get_localzone_name()
 
     @property
     def schedule_text(self) -> str:
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/plugin_service.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/plugin_service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/service/pixiv_account_binder.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/service/pixiv_account_binder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from typing import Optional
 
-from nonebot_plugin_pixivbot.data.pixiv_binding import PixivBindingRepo
-from nonebot_plugin_pixivbot.global_context import context
-from nonebot_plugin_pixivbot.model import T_UID
-from nonebot_plugin_pixivbot.model.pixiv_binding import PixivBinding
+from ..data.pixiv_binding import PixivBindingRepo
+from ..global_context import context
+from ..model.pixiv_binding import PixivBinding
 
 repo = context.require(PixivBindingRepo)
 
 
 @context.register_singleton()
 class PixivAccountBinder:
 
-    async def bind(self, adapter: str, user_id: T_UID, pixiv_user_id: int):
-        binding = PixivBinding(adapter=adapter, user_id=user_id, pixiv_user_id=pixiv_user_id)
+    async def bind(self, platform: str, user_id: str, pixiv_user_id: int):
+        binding = PixivBinding(platform=platform, user_id=user_id, pixiv_user_id=pixiv_user_id)
         await repo.update(binding)
 
-    async def unbind(self, adapter: str, user_id: T_UID) -> bool:
-        return await repo.remove(adapter, user_id)
+    async def unbind(self, platform: str, user_id: str) -> bool:
+        return await repo.remove(platform, user_id)
 
-    async def get_binding(self, adapter: str, user_id: T_UID) -> Optional[int]:
-        binding = await repo.get(adapter, user_id)
+    async def get_binding(self, platform: str, user_id: str) -> Optional[int]:
+        binding = await repo.get(platform, user_id)
         if binding:
             return binding.pixiv_user_id
         else:
             return None
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/service/pixiv_service.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/service/pixiv_service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/service/roulette.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/service/roulette.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/service/watchman.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/service/watchman.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,83 +1,81 @@
 from datetime import datetime, timedelta, timezone
-from typing import Dict, Any, overload, Type
+from typing import Dict, Any, overload, Type, TYPE_CHECKING
 
 from apscheduler.triggers.interval import IntervalTrigger
+from nonebot_plugin_session import Session
 
-from nonebot_plugin_pixivbot.config import Config
-from nonebot_plugin_pixivbot.data.watch_task import WatchTaskRepo
-from nonebot_plugin_pixivbot.global_context import context
-from nonebot_plugin_pixivbot.handler.base import Handler
-from nonebot_plugin_pixivbot.handler.watch import WatchUserIllustsHandler, WatchFollowingIllustsHandler
-from nonebot_plugin_pixivbot.model import T_UID, T_GID
-from nonebot_plugin_pixivbot.model import WatchTask, WatchType
-from nonebot_plugin_pixivbot.protocol_dep.post_dest import PostDestination
-from nonebot_plugin_pixivbot.service.interval_task_worker import IntervalTaskWorker
-from nonebot_plugin_pixivbot.utils.nonebot import get_bot_user_identifier
+from .interval_task_worker import IntervalTaskWorker
+from ..config import Config
+from ..data.watch_task import WatchTaskRepo
+from ..global_context import context
+from ..model import WatchTask, WatchType
+
+if TYPE_CHECKING:
+    from ..handler.base import Handler
 
 conf = context.require(Config)
 
 
 @context.root.register_eager_singleton()
-class Watchman(IntervalTaskWorker[WatchTask[T_UID, T_GID]]):
+class Watchman(IntervalTaskWorker[WatchTask]):
     tag = "watchman"
 
     _trigger_hasher_mapper = {
-        WatchType.user_illusts: lambda args: args["user_id"],
-        WatchType.following_illusts: lambda args: hash(args["sender_user_id"]),
+        WatchType.user_illusts: lambda item: item.kwargs["user_id"],
+        WatchType.following_illusts: lambda item: hash(item.subscriber.id1),
     }
 
     @property
     def repo(self) -> WatchTaskRepo:
         return context.require(WatchTaskRepo)
 
     @classmethod
     def _get_handler_type(cls, type: WatchType) -> Type["Handler"]:
+        from ..handler.watch import WatchUserIllustsHandler, WatchFollowingIllustsHandler
+
         if type == WatchType.user_illusts:
             return WatchUserIllustsHandler
         elif type == WatchType.following_illusts:
             return WatchFollowingIllustsHandler
 
-    async def _handle_trigger(self, task: WatchTask[T_UID, T_GID], post_dest: PostDestination[T_UID, T_GID],
-                              manually: bool = False):
+    async def _handle_trigger(self, item: WatchTask, manually: bool = False):
         try:
-            handler_type = self._get_handler_type(task.type)
-            handler = handler_type(post_dest, silently=not manually, disable_interceptors=manually)
-            await handler.handle_with_parsed_args(task=task)
+            handler_type = self._get_handler_type(item.type)
+            handler = handler_type(item.subscriber, silently=not manually, disable_interceptors=manually)
+            await handler.handle_with_parsed_args(task=item)
         finally:
             # 保存checkpoint，避免一次异常后下一次重复推送
             # 但是会存在丢失推送的问题
-            task.checkpoint = datetime.now(timezone.utc)
-            await self.repo.update(task)
+            item.checkpoint = datetime.now(timezone.utc)
+            await self.repo.update(item)
 
-    def _make_job_trigger(self, item: WatchTask[T_UID, T_GID]) -> IntervalTrigger:
+    def _make_job_trigger(self, item: WatchTask) -> IntervalTrigger:
         hasher = self._trigger_hasher_mapper[item.type]
-        hash_sec = hasher(item.kwargs) % conf.pixiv_watch_interval
+        hash_sec = hasher(item) % conf.pixiv_watch_interval
         yesterday = datetime.now(timezone.utc).replace(
             hour=0, minute=0, second=0, microsecond=0
         ) + timedelta(days=-1) + timedelta(seconds=hash_sec)
         trigger = IntervalTrigger(seconds=conf.pixiv_watch_interval, start_date=yesterday)
         return trigger
 
     async def _build_task(self, type_: WatchType,
                           kwargs: Dict[str, Any],
-                          post_dest: PostDestination[T_UID, T_GID]) -> WatchTask:
+                          session: Session) -> WatchTask:
         return WatchTask(type=type_, kwargs=kwargs,
-                         subscriber=post_dest.identifier,
-                         bot=get_bot_user_identifier(post_dest.bot))
+                         subscriber=session)
 
     @overload
     async def add_task(self, type_: WatchType,
                        kwargs: Dict[str, Any],
-                       post_dest: PostDestination[T_UID, T_GID]) -> bool:
+                       session: Session) -> bool:
         ...
 
     async def add_task(self, *args, **kwargs) -> bool:
         return await super().add_task(*args, **kwargs)
 
-    async def fetch(self, code: str, post_dest: PostDestination[T_UID, T_GID]) -> bool:
-        task = await self.repo.get_by_code(get_bot_user_identifier(post_dest.bot),
-                                           post_dest.identifier, code)
+    async def fetch(self, code: str, session: Session) -> bool:
+        task = await self.repo.get_by_code(session, code)
         if task is not None:
-            await self._handle_trigger(task, post_dest, manually=True)
+            await self._handle_trigger(task, manually=True)
             return True
         return False
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/utils/decode_integer.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/decode_integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/utils/errors.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/errors.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/utils/expires_lru_dict.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/expires_lru_dict.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/utils/lifecycler.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/lifecycler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot/utils/shared_agen.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/shared_agen.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot_onebot_v11/handler/poke.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/more.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,40 @@
-from typing import Dict, Type
-
-from nonebot import on_notice
-from nonebot.adapters import Event
-from nonebot.adapters.onebot.v11 import PokeNotifyEvent
+from nonebot import on_regex
+from nonebot.internal.adapter import Event
 from nonebot.internal.params import Depends
+from nonebot_plugin_session import extract_session
 
-from nonebot_plugin_pixivbot.global_context import context
-from nonebot_plugin_pixivbot.handler.base import Handler
-from nonebot_plugin_pixivbot.handler.common import RandomBookmarkHandler, RandomRecommendedIllustHandler, RankingHandler
-from nonebot_plugin_pixivbot.protocol_dep.post_dest import post_destination
-from nonebot_plugin_pixivbot_onebot_v11.config import OnebotV11Config
-
-adapter_conf = context.require(OnebotV11Config)
-
-handler_type_mapping: Dict[str, Type[Handler]] = {
-    "ranking": RankingHandler,
-    "random_recommended_illust": RandomRecommendedIllustHandler,
-    "random_bookmark": RandomBookmarkHandler
-}
-
-handler_type = handler_type_mapping.get(adapter_conf.pixiv_poke_action, None)
-
-if handler_type is not None:
-    class PokeHandler(handler_type):
-        @classmethod
-        def type(cls) -> str:
-            return "poke"
-
-        @classmethod
-        def enabled(cls) -> bool:
-            return handler_type is not None
-
-
-    async def _poke(event: Event) -> bool:
-        return isinstance(event, PokeNotifyEvent) and event.is_tome()
-
-
-    @on_notice(_poke, priority=10, block=True).handle()
-    async def on_match(post_dest=Depends(post_destination)):
-        await PokeHandler(post_dest).handle()
+from .base import CommonHandler
+from ..pkg_context import context
+from ..recorder import Recorder
+from ..utils import get_common_query_rule, ArgCount
+from ...config import Config
+from ...plugin_service import more_service
+from ...utils.errors import BadRequestError
+
+recorder = context.require(Recorder)
+conf = context.require(Config)
+
+
+class MoreHandler(CommonHandler, service=more_service):
+    @classmethod
+    def type(cls) -> str:
+        return "more"
+
+    @classmethod
+    def enabled(cls) -> bool:
+        return conf.pixiv_more_enabled
+
+    async def actual_handle(self, count: int = 1):
+        req = recorder.get_req(self.session)
+        if not req:
+            raise BadRequestError("你还没有发送过请求")
+
+        handler = req.handler_type(self.session, silently=self.silently, disable_interceptors=True)
+        await handler.handle(*req.args, **{**req.kwargs, "count": count})
+
+
+@on_regex("^还要((.*)张)?$", rule=get_common_query_rule(), priority=1, block=True).handle()
+async def _(event: Event,
+            session=Depends(extract_session),
+            count=ArgCount(1)):
+    await MoreHandler(session, event).handle(count=count)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/src/nonebot_plugin_pixivbot_onebot_v11/protocol_dep/post_dest.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/service/postman.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,137 +1,114 @@
-import dataclasses
-from typing import Optional, Sequence, Union, List
+from contextlib import asynccontextmanager
+from io import StringIO
+from typing import Optional, Union
+
+from nonebot import get_bot, logger
+from nonebot.exception import ActionFailed
+from nonebot.internal.adapter import Event
+from nonebot_plugin_saa import MessageFactory, Text, Image, AggregatedMessageFactory, extract_target
+from nonebot_plugin_session import Session
+from nonebot_plugin_session.saa import get_saa_target
+
+from ..config import Config
+from ..enums import BlockAction
+from ..global_context import context
+from ..model.message import IllustMessageModel, IllustMessagesModel
 
-from nonebot import logger
-from nonebot.adapters.onebot.v11 import Bot, Message, MessageSegment, MessageEvent
-from nonebot_plugin_access_control.subject import extract_subjects
-
-from nonebot_plugin_pixivbot.global_context import context
-from nonebot_plugin_pixivbot.model import PostIdentifier
-from nonebot_plugin_pixivbot.protocol_dep.post_dest import PostDestination as BasePostDestination, \
-    PostDestinationFactory as BasePostDestinationFactory, PostDestinationFactoryManager
-from nonebot_plugin_pixivbot.utils.nonebot import is_superuser
-
-
-class PostDestination(BasePostDestination[int, int]):
-    def __init__(self, bot: Bot,
-                 user_id: Optional[int] = None,
-                 group_id: Optional[int] = None,
-                 event: Optional[MessageEvent] = None):
-        self._bot = bot
-        self._identifier = PostIdentifier("onebot", user_id, group_id)
-        self._event = event
-
-    @property
-    def bot(self) -> Bot:
-        return self._bot
-
-    @property
-    def identifier(self):
-        return self._identifier
-
-    @property
-    def event(self) -> Optional[MessageEvent]:
-        return self._event
-
-    def normalized(self) -> "PostDestination":
-        return PostDestination(self.bot, self.user_id, self.group_id)
-
-    def extract_subjects(self) -> List[str]:
-        if self.event is not None:
-            return extract_subjects(self.bot, self.event)
-
-        li = []
-        if self.user_id is not None:
-            li.append(f"qq:{self.user_id}")
-            li.append(f"onebot:{self.user_id}")
-
-            if is_superuser(self.bot, self.user_id):
-                li.append("superuser")
-
-        if self.group_id is not None:
-            li.append(f"qq:{self.group_id}")
-            li.append(f"onebot:g{self.group_id}")
-            li.append("qq:group")
-            li.append("onebot:group")
-        else:
-            li.append("qq:private")
-            li.append("onebot:private")
+conf = context.require(Config)
 
-        li.append("qq")
-        li.append("onebot")
-        li.append("all")
-
-        return li
-
-    async def post(self, message: Union[Message, Sequence[Message]]):
-        if len(message) == 0:
-            logger.warning("message is empty")
-        else:
-            if isinstance(message[0], Message):
-                if len(message) > 1:
-                    await self.post_multiple(message)
-                else:
-                    await self.post_single(message[0])
-            else:
-                await self.post_single(message)
 
-    async def post_single(self, message: Message):
-        if self.event:
-            message.insert(0, MessageSegment.reply(self.event.message_id))
+@context.register_singleton()
+class Postman:
 
-        if self.group_id:
-            await self.bot.send_group_msg(group_id=self.group_id, message=message)
-        else:
-            await self.bot.send_msg(user_id=self.user_id, message=message)
+    @asynccontextmanager
+    async def _feedback_on_action_failed(self, session: Session):
+        try:
+            yield
+        except ActionFailed as e:
+            logger.opt(exception=e).error("图片发送失败")
+
+            await self.post_plain_text("图片发送失败", session)
+
+    def _make_illust_msg(self, model: IllustMessageModel) -> MessageFactory:
+        msg = MessageFactory([])
+
+        if model.block_action is not None:
+            if model.block_action == BlockAction.no_image:
+                msg.append(Text(model.block_message))
+            elif model.block_action == BlockAction.completely_block:
+                msg.append(Text(model.block_message))
+                return msg
+            elif model.block_action == BlockAction.no_reply:
+                return msg
+            else:
+                raise ValueError(f"invalid block_action: {model.block_action}")
 
-    async def post_multiple(self, messages: Sequence[Message]):
-        if not self.group_id:
-            self_info = await self.bot.get_login_info()
-            nickname = self_info["nickname"]
-        else:
-            # 获取bot的群昵称
-            self_info = await self.bot.get_group_member_info(group_id=self.group_id, user_id=int(self.bot.self_id))
-            nickname = self_info["card"] or self_info["nickname"]
-
-        # 创建转发消息
-        msg_dict = []
-
-        for msg in messages:
-            msg_dict.append([dataclasses.asdict(seg) for seg in msg])
-
-        messages = [{
-            "type": "node",
-            "data": {
-                "name": nickname,
-                "uin": self.bot.self_id,
-                "content": msg
-            }
-        } for msg in messages]
-
-        if not self.group_id:
-            await self.bot.send_private_forward_msg(
-                user_id=self.user_id,
-                messages=messages
-            )
-        else:
-            await self.bot.send_group_forward_msg(
-                group_id=self.group_id,
-                messages=messages
-            )
+        msg.append(Image(model.image))
 
+        with StringIO() as sio:
+            sio.write('\n')
+            if model.number is not None:
+                sio.write(f"#{model.number}")
+
+            sio.write(f"「{model.title}」")
+            if model.total != 1:
+                sio.write(f"（{model.page + 1}/{model.total}）")
+            sio.write("\n")
+
+            sio.write(f"作者：{model.author}\n"
+                      f"发布时间：{model.create_time}\n")
+            if conf.pixiv_send_illust_link:
+                sio.write(model.link)
+            else:
+                sio.write(f"P站ID：{model.id}")
 
-@context.register_singleton()
-class PostDestinationFactory(BasePostDestinationFactory[int, int, MessageEvent], manager=PostDestinationFactoryManager):
-    adapter = "onebot"
+            msg.append(Text(sio.getvalue()))
+        return msg
 
-    def build(self, bot: Bot, user_id: Optional[int], group_id: Optional[int]) -> PostDestination:
-        return PostDestination(bot, user_id, group_id)
+    async def _post(self, msg: Union[MessageFactory, AggregatedMessageFactory],
+                    session: Session, event: Optional[Event] = None):
+        bot = get_bot(session.bot_id)
+        if event is not None:
+            target = extract_target(event)
+        else:
+            target = get_saa_target(session)
 
-    def from_event(self, bot: Bot, event: MessageEvent) -> PostDestination:
-        user_id = getattr(event, "user_id", None)
-        group_id = getattr(event, "group_id", None)
+        if bot.type == "QQ Guild":  # QQ频道发消息要审核
+            from nonebot.adapters.qqguild.exception import AuditException
+            try:
+                await msg.send_to(target, bot)
+            except AuditException as e:
+                await e.get_audit_result()
+        else:
+            await msg.send_to(target, bot)
 
-        if not user_id and not group_id:
-            raise ValueError("user_id 和 group_id 不能同时为 None")
+    async def post_plain_text(self, message: str, session: Session, event: Optional[Event] = None):
+        msg = MessageFactory(Text(message))
+        await self._post(msg, session, event)
+
+    async def post_illust(self, model: IllustMessageModel, session: Session, event: Optional[Event] = None):
+        async with self._feedback_on_action_failed(session):
+            msg = MessageFactory([])
+            if model.header is not None:
+                msg.append(Text(model.header + '\n'))
+
+            msg.extend(self._make_illust_msg(model))
+
+            await self._post(msg, session, event)
+
+    async def post_illusts(self, model: IllustMessagesModel, session: Session, event: Optional[Event] = None):
+        async with self._feedback_on_action_failed(session):
+            if (session.bot_type != "OneBot V11" or
+                    conf.pixiv_send_forward_message == 'never' or
+                    conf.pixiv_send_forward_message == 'auto' and len(model.messages) == 1):
+                for x in model.flat():
+                    await self.post_illust(x, session, event)
+            else:
+                messages = []
+                if model.header:
+                    messages.append(MessageFactory([Text(model.header)]))
+                for sub_model in model.messages:
+                    messages.append(self._make_illust_msg(sub_model))
 
-        return PostDestination(bot, user_id, group_id, event)
+                msg = AggregatedMessageFactory(messages)
+                await self._post(msg, session, event)
```

### Comparing `nonebot_plugin_pixivbot-1.9.0/PKG-INFO` & `nonebot_plugin_pixivbot-2.0.0a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,36 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pixivbot
-Version: 1.9.0
+Version: 2.0.0a1
 Summary: Nonebot Plugin PixivBot
 Home-page: https://github.com/ssttkkl/nonebot-plugin-pixivbot
 License: MIT
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: kook
-Provides-Extra: mongo
-Provides-Extra: onebot
-Provides-Extra: postgresql
-Provides-Extra: telegram
 Requires-Dist: Pillow (>=9.2.0,<10.0.0)
 Requires-Dist: PixivPy-Async (>=1.2.14,<2.0.0)
-Requires-Dist: SQLAlchemy[asyncio] (>=2.0.0,<3.0.0)
 Requires-Dist: aiohttp-socks (>=0.8.0,<0.9.0)
-Requires-Dist: aiosqlite (>=0.18.0,<0.19.0)
 Requires-Dist: asyncache (>=0.3.1,<0.4.0)
-Requires-Dist: asyncpg (>=0.27.0,<0.28.0) ; extra == "postgresql"
-Requires-Dist: beanie (>=1.17.0,<2.0.0) ; extra == "mongo"
 Requires-Dist: cachetools (>=5.2.0,<6.0.0)
 Requires-Dist: frozendict (>=2.3.4,<3.0.0)
 Requires-Dist: lazy (>=1.4,<2.0)
-Requires-Dist: motor (>=3.0.0,<4.0.0) ; extra == "mongo"
-Requires-Dist: nonebot-adapter-kaiheila (>=0.2.0,<0.3.0) ; extra == "kook"
-Requires-Dist: nonebot-adapter-onebot (>=2.2.1,<3.0.0) ; extra == "onebot"
-Requires-Dist: nonebot-adapter-telegram (>=0.1.0b8,<0.2.0) ; extra == "telegram"
-Requires-Dist: nonebot-plugin-access-control (>=0.4.0,<0.5.0)
-Requires-Dist: nonebot-plugin-localstore (>=0.4.1,<0.5.0)
+Requires-Dist: nonebot-plugin-access-control (>=0.5.5)
+Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.7,<0.3.0)
+Requires-Dist: nonebot-plugin-session (>=0.0.4)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
 Requires-Dist: numpy (>=1.23.1,<2.0.0)
 Requires-Dist: shortuuid (>=1.0.9,<2.0.0)
-Requires-Dist: tzlocal (>=4.2,<5.0)
+Requires-Dist: tzlocal (>=5.0.1,<6.0.0)
 Project-URL: Repository, https://github.com/ssttkkl/nonebot-plugin-pixivbot
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
```

#### html2text {}

```diff
@@ -1,33 +1,25 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-pixivbot Version: 1.9.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-pixivbot Version: 2.0.0a1 Summary:
 Nonebot Plugin PixivBot Home-page: https://github.com/ssttkkl/nonebot-plugin-
 pixivbot License: MIT Author: ssttkkl Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Provides-Extra: kook
-Provides-Extra: mongo Provides-Extra: onebot Provides-Extra: postgresql
-Provides-Extra: telegram Requires-Dist: Pillow (>=9.2.0,<10.0.0) Requires-Dist:
-PixivPy-Async (>=1.2.14,<2.0.0) Requires-Dist: SQLAlchemy[asyncio]
-(>=2.0.0,<3.0.0) Requires-Dist: aiohttp-socks (>=0.8.0,<0.9.0) Requires-Dist:
-aiosqlite (>=0.18.0,<0.19.0) Requires-Dist: asyncache (>=0.3.1,<0.4.0)
-Requires-Dist: asyncpg (>=0.27.0,<0.28.0) ; extra == "postgresql" Requires-
-Dist: beanie (>=1.17.0,<2.0.0) ; extra == "mongo" Requires-Dist: cachetools
-(>=5.2.0,<6.0.0) Requires-Dist: frozendict (>=2.3.4,<3.0.0) Requires-Dist: lazy
-(>=1.4,<2.0) Requires-Dist: motor (>=3.0.0,<4.0.0) ; extra == "mongo" Requires-
-Dist: nonebot-adapter-kaiheila (>=0.2.0,<0.3.0) ; extra == "kook" Requires-
-Dist: nonebot-adapter-onebot (>=2.2.1,<3.0.0) ; extra == "onebot" Requires-
-Dist: nonebot-adapter-telegram (>=0.1.0b8,<0.2.0) ; extra == "telegram"
-Requires-Dist: nonebot-plugin-access-control (>=0.4.0,<0.5.0) Requires-Dist:
-nonebot-plugin-localstore (>=0.4.1,<0.5.0) Requires-Dist: nonebot2
-(>=2.0.0,<3.0.0) Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
-Requires-Dist: numpy (>=1.23.1,<2.0.0) Requires-Dist: shortuuid
-(>=1.0.9,<2.0.0) Requires-Dist: tzlocal (>=4.2,<5.0) Project-URL: Repository,
-https://github.com/ssttkkl/nonebot-plugin-pixivbot Description-Content-Type:
-text/markdown
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: Pillow
+(>=9.2.0,<10.0.0) Requires-Dist: PixivPy-Async (>=1.2.14,<2.0.0) Requires-Dist:
+aiohttp-socks (>=0.8.0,<0.9.0) Requires-Dist: asyncache (>=0.3.1,<0.4.0)
+Requires-Dist: cachetools (>=5.2.0,<6.0.0) Requires-Dist: frozendict
+(>=2.3.4,<3.0.0) Requires-Dist: lazy (>=1.4,<2.0) Requires-Dist: nonebot-
+plugin-access-control (>=0.5.5) Requires-Dist: nonebot-plugin-send-anything-
+anywhere (>=0.2.7,<0.3.0) Requires-Dist: nonebot-plugin-session (>=0.0.4)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Requires-Dist:
+nonebot_plugin_apscheduler (>=0.2.0,<0.3.0) Requires-Dist: numpy
+(>=1.23.1,<2.0.0) Requires-Dist: shortuuid (>=1.0.9,<2.0.0) Requires-Dist:
+tzlocal (>=5.0.1,<6.0.0) Project-URL: Repository, https://github.com/ssttkkl/
+nonebot-plugin-pixivbot Description-Content-Type: text/markdown
                                    [nonebot]
                nonebot_plugin_pixivbot ===== _â¨ PixivBot â¨_
                            [license] [pypi] [python]
 NoneBotæä»¶ï¼æ¯æåééæºPixivæç»ãç»å¸æ´æ°æ¨éãå®æ¶è®¢éæ¨éâ¦â¦
 ééåè®®ï¼ - [Onebot V11](https://onebot.adapters.nonebot.dev/) - [KOOK /
 å¼é»å¦](https://github.com/Tian-que/nonebot-adapter-kaiheila) - [Telegram]
 (https://github.com/nonebot/adapter-telegram) ## è§¦åè¯­å¥ ### æ®éè¯­å¥
```

