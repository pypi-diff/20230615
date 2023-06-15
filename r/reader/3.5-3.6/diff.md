# Comparing `tmp/reader-3.5.tar.gz` & `tmp/reader-3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reader-3.5.tar", last modified: Sat Mar 18 22:57:52 2023, max compression
+gzip compressed data, was "reader-3.6.tar", last modified: Thu Jun 15 21:41:04 2023, max compression
```

## Comparing `reader-3.5.tar` & `reader-3.6.tar`

### file list

```diff
@@ -1,241 +1,241 @@
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-03-18 22:57:52.700754 reader-3.5/
--rw-r--r--   0 lemon      (501) staff       (20)    54205 2023-03-18 22:55:52.000000 reader-3.5/CHANGES.rst
--rw-r--r--   0 lemon      (501) staff       (20)     1475 2021-04-07 12:51:45.000000 reader-3.5/LICENSE
--rw-r--r--   0 lemon      (501) staff       (20)      406 2022-06-28 21:13:50.000000 reader-3.5/MANIFEST.in
--rw-r--r--   0 lemon      (501) staff       (20)     5412 2023-03-18 22:57:52.701096 reader-3.5/PKG-INFO
--rw-r--r--   0 lemon      (501) staff       (20)     3503 2022-07-08 20:16:13.000000 reader-3.5/README.rst
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-03-18 22:57:52.206670 reader-3.5/docs/
--rw-r--r--   0 lemon      (501) staff       (20)      604 2020-10-28 07:20:55.000000 reader-3.5/docs/Makefile
--rw-r--r--   0 lemon      (501) staff       (20)     2956 2023-03-13 22:26:16.000000 reader-3.5/docs/api.rst
--rw-r--r--   0 lemon      (501) staff       (20)     2984 2021-06-02 17:57:04.000000 reader-3.5/docs/app.rst
--rw-r--r--   0 lemon      (501) staff       (20)       29 2020-10-28 07:20:55.000000 reader-3.5/docs/changelog.rst
--rw-r--r--   0 lemon      (501) staff       (20)     2125 2020-10-28 07:22:28.000000 reader-3.5/docs/cli.rst
--rw-r--r--   0 lemon      (501) staff       (20)     2303 2020-11-06 16:00:45.000000 reader-3.5/docs/compat.rst
--rw-r--r--   0 lemon      (501) staff       (20)     3368 2023-01-17 21:57:57.000000 reader-3.5/docs/conf.py
--rw-r--r--   0 lemon      (501) staff       (20)     1147 2020-10-28 07:23:47.000000 reader-3.5/docs/config.rst
--rw-r--r--   0 lemon      (501) staff       (20)     2817 2022-03-11 21:58:00.000000 reader-3.5/docs/dev-app.rst
--rw-r--r--   0 lemon      (501) staff       (20)    12080 2023-01-17 21:16:38.000000 reader-3.5/docs/dev.rst
--rw-r--r--   0 lemon      (501) staff       (20)    28324 2023-03-18 22:12:54.000000 reader-3.5/docs/guide.rst
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-03-18 22:57:52.207316 reader-3.5/docs/images/
--rw-r--r--   0 lemon      (501) staff       (20)    36483 2020-10-28 07:20:31.000000 reader-3.5/docs/images/redesign-01.png
--rw-r--r--   0 lemon      (501) staff       (20)     1589 2023-01-01 14:20:52.000000 reader-3.5/docs/index.rst
--rw-r--r--   0 lemon      (501) staff       (20)     2920 2022-12-29 21:45:24.000000 reader-3.5/docs/install.rst
--rw-r--r--   0 lemon      (501) staff       (20)     2053 2023-01-17 21:53:16.000000 reader-3.5/docs/internal.rst
--rw-r--r--   0 lemon      (501) staff       (20)      810 2020-10-28 07:19:52.000000 reader-3.5/docs/make.bat
--rw-r--r--   0 lemon      (501) staff       (20)     2092 2022-07-08 20:32:37.000000 reader-3.5/docs/plugins.rst
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-03-18 22:57:52.222383 reader-3.5/docs/screenshots/
--rw-r--r--   0 lemon      (501) staff       (20)    68106 2020-10-28 07:20:31.000000 reader-3.5/docs/screenshots/dillo.png
--rw-r--r--   0 lemon      (501) staff       (20)   109426 2020-10-28 07:22:31.000000 reader-3.5/docs/screenshots/entries-feed.png
--rw-r--r--   0 lemon      (501) staff       (20)    96393 2020-10-28 07:22:31.000000 reader-3.5/docs/screenshots/entries.png
--rw-r--r--   0 lemon      (501) staff       (20)   277564 2022-07-09 07:30:35.000000 reader-3.5/docs/screenshots/entry-one.png
--rw-r--r--   0 lemon      (501) staff       (20)   128002 2020-10-28 07:22:31.000000 reader-3.5/docs/screenshots/entry-two.png
--rw-r--r--   0 lemon      (501) staff       (20)    48411 2020-10-28 07:22:31.000000 reader-3.5/docs/screenshots/feeds.png
--rw-r--r--   0 lemon      (501) staff       (20)   364336 2020-10-28 07:22:31.000000 reader-3.5/docs/screenshots/lynx.png
--rw-r--r--   0 lemon      (501) staff       (20)   111458 2020-10-28 07:22:31.000000 reader-3.5/docs/screenshots/search.png
--rw-r--r--   0 lemon      (501) staff       (20)   135812 2022-06-27 22:00:00.000000 reader-3.5/docs/screenshots/twitter-one.png
--rw-r--r--   0 lemon      (501) staff       (20)   385070 2022-07-01 13:21:27.000000 reader-3.5/docs/screenshots/twitter-two.png
--rw-r--r--   0 lemon      (501) staff       (20)     9271 2023-01-16 22:55:01.000000 reader-3.5/docs/tutorial.rst
--rw-r--r--   0 lemon      (501) staff       (20)     1940 2022-07-08 20:24:57.000000 reader-3.5/docs/why.rst
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-03-18 22:57:52.227240 reader-3.5/examples/
--rw-r--r--   0 lemon      (501) staff       (20)     2713 2021-05-05 18:41:19.000000 reader-3.5/examples/config.yaml
--rw-r--r--   0 lemon      (501) staff       (20)     1639 2023-01-16 23:03:30.000000 reader-3.5/examples/parser_only.py
--rw-r--r--   0 lemon      (501) staff       (20)     1596 2022-01-20 22:05:30.000000 reader-3.5/examples/podcast.py
--rw-r--r--   0 lemon      (501) staff       (20)     1819 2020-12-23 13:16:52.000000 reader-3.5/examples/terminal.py
--rw-r--r--   0 lemon      (501) staff       (20)       90 2021-06-08 13:32:02.000000 reader-3.5/pyproject.toml
--rwxr-xr-x   0 lemon      (501) staff       (20)     3687 2022-09-11 14:58:00.000000 reader-3.5/run.sh
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-03-18 22:57:52.244145 reader-3.5/scripts/
--rw-r--r--   0 lemon      (501) staff       (20)    53248 2020-06-23 14:22:09.000000 reader-3.5/scripts/.coverage
--rwxr-xr-x   0 lemon      (501) staff       (20)      559 2023-01-28 10:01:54.000000 reader-3.5/scripts/backup.sh
--rw-r--r--   0 lemon      (501) staff       (20)    13837 2022-12-31 08:17:16.000000 reader-3.5/scripts/bench.py
--rw-r--r--   0 lemon      (501) staff       (20)     4340 2022-12-31 08:17:15.000000 reader-3.5/scripts/debug_storage_stats.py
--rw-r--r--   0 lemon      (501) staff       (20)      356 2022-06-28 20:55:42.000000 reader-3.5/scripts/generate_import_all.py
--rw-r--r--   0 lemon      (501) staff       (20)     5021 2020-10-28 07:24:20.000000 reader-3.5/scripts/jscontrols.html
--rw-r--r--   0 lemon      (501) staff       (20)     1211 2020-10-28 07:24:20.000000 reader-3.5/scripts/jscontrols.py
--rwxr-xr-x   0 lemon      (501) staff       (20)      764 2020-10-28 07:21:42.000000 reader-3.5/scripts/lines.sh
--rw-r--r--   0 lemon      (501) staff       (20)     4600 2022-12-31 08:17:15.000000 reader-3.5/scripts/release.py
--rw-r--r--   0 lemon      (501) staff       (20)     3403 2023-03-18 22:57:52.706096 reader-3.5/setup.cfg
--rw-r--r--   0 lemon      (501) staff       (20)       38 2021-04-26 16:52:55.000000 reader-3.5/setup.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-03-18 22:57:52.185048 reader-3.5/src/
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-03-18 22:57:52.270761 reader-3.5/src/reader/
--rw-r--r--   0 lemon      (501) staff       (20)     2532 2023-03-18 22:55:52.000000 reader-3.5/src/reader/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)      381 2020-10-28 07:22:22.000000 reader-3.5/src/reader/__main__.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-03-18 22:57:52.281646 reader-3.5/src/reader/_app/
--rw-r--r--   0 lemon      (501) staff       (20)    22629 2023-03-05 14:28:08.000000 reader-3.5/src/reader/_app/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)     4329 2022-12-31 08:17:16.000000 reader-3.5/src/reader/_app/api_thing.py
--rw-r--r--   0 lemon      (501) staff       (20)     1457 2021-10-30 11:02:39.000000 reader-3.5/src/reader/_app/cli.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-03-18 22:57:52.285099 reader-3.5/src/reader/_app/static/
--rw-r--r--   0 lemon      (501) staff       (20)    14735 2022-06-23 20:50:42.000000 reader-3.5/src/reader/_app/static/controls.js
--rw-r--r--   0 lemon      (501) staff       (20)     4194 2022-06-22 19:10:26.000000 reader-3.5/src/reader/_app/static/style.css
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-03-18 22:57:52.300469 reader-3.5/src/reader/_app/templates/
--rw-r--r--   0 lemon      (501) staff       (20)      980 2021-10-27 17:55:28.000000 reader-3.5/src/reader/_app/templates/add_entry.html
--rw-r--r--   0 lemon      (501) staff       (20)    12029 2023-03-05 14:26:36.000000 reader-3.5/src/reader/_app/templates/entries.html
--rw-r--r--   0 lemon      (501) staff       (20)     3200 2023-02-14 22:28:37.000000 reader-3.5/src/reader/_app/templates/entry.html
--rw-r--r--   0 lemon      (501) staff       (20)     5083 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_app/templates/feeds.html
--rw-r--r--   0 lemon      (501) staff       (20)     1631 2022-03-11 23:07:17.000000 reader-3.5/src/reader/_app/templates/layout.html
--rw-r--r--   0 lemon      (501) staff       (20)     9375 2023-03-05 14:18:18.000000 reader-3.5/src/reader/_app/templates/macros.html
--rw-r--r--   0 lemon      (501) staff       (20)     2569 2022-07-30 08:02:27.000000 reader-3.5/src/reader/_app/templates/metadata.html
--rw-r--r--   0 lemon      (501) staff       (20)     1515 2021-08-17 08:51:46.000000 reader-3.5/src/reader/_app/templates/tags.html
--rw-r--r--   0 lemon      (501) staff       (20)     1150 2020-10-28 07:23:44.000000 reader-3.5/src/reader/_app/wsgi.py
--rw-r--r--   0 lemon      (501) staff       (20)    13132 2022-12-31 08:17:16.000000 reader-3.5/src/reader/_cli.py
--rw-r--r--   0 lemon      (501) staff       (20)     4587 2022-07-16 20:45:27.000000 reader-3.5/src/reader/_config.py
--rw-r--r--   0 lemon      (501) staff       (20)     1531 2023-01-17 22:12:52.000000 reader-3.5/src/reader/_feedparser.py
--rw-r--r--   0 lemon      (501) staff       (20)     4074 2022-12-18 08:53:24.000000 reader-3.5/src/reader/_feedparser_lazy.py
--rw-r--r--   0 lemon      (501) staff       (20)     2980 2023-03-14 06:52:53.000000 reader-3.5/src/reader/_hash_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)     2220 2022-12-31 08:18:29.000000 reader-3.5/src/reader/_html_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)     2158 2022-12-31 08:19:05.000000 reader-3.5/src/reader/_http_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)     5677 2023-01-17 22:12:52.000000 reader-3.5/src/reader/_jsonfeed.py
--rw-r--r--   0 lemon      (501) staff       (20)    24586 2023-01-19 20:52:11.000000 reader-3.5/src/reader/_parser.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-03-18 22:57:52.307497 reader-3.5/src/reader/_plugins/
--rw-r--r--   0 lemon      (501) staff       (20)     1617 2022-12-29 21:54:33.000000 reader-3.5/src/reader/_plugins/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)     3201 2021-11-05 08:41:21.000000 reader-3.5/src/reader/_plugins/cli_status.py
--rw-r--r--   0 lemon      (501) staff       (20)     3065 2022-12-29 22:18:56.000000 reader-3.5/src/reader/_plugins/enclosure_tags.py
--rw-r--r--   0 lemon      (501) staff       (20)     4561 2023-01-01 10:20:44.000000 reader-3.5/src/reader/_plugins/preview_feed_list.py
--rw-r--r--   0 lemon      (501) staff       (20)     2931 2022-06-27 21:01:33.000000 reader-3.5/src/reader/_plugins/sqlite_releases.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-03-18 22:57:52.309346 reader-3.5/src/reader/_plugins/templates/
--rw-r--r--   0 lemon      (501) staff       (20)      815 2022-12-27 22:01:52.000000 reader-3.5/src/reader/_plugins/templates/preview_feed_list.html
--rw-r--r--   0 lemon      (501) staff       (20)     2094 2022-11-21 20:16:44.000000 reader-3.5/src/reader/_plugins/tumblr_gdpr.py
--rw-r--r--   0 lemon      (501) staff       (20)    26325 2023-01-17 22:12:52.000000 reader-3.5/src/reader/_plugins/twitter.py
--rw-r--r--   0 lemon      (501) staff       (20)     7785 2023-01-17 21:52:55.000000 reader-3.5/src/reader/_requests_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)      726 2023-01-01 10:22:19.000000 reader-3.5/src/reader/_requests_utils_lazy.py
--rw-r--r--   0 lemon      (501) staff       (20)     5623 2023-01-01 10:41:25.000000 reader-3.5/src/reader/_retrievers.py
--rw-r--r--   0 lemon      (501) staff       (20)    34166 2023-03-03 21:46:20.000000 reader-3.5/src/reader/_search.py
--rw-r--r--   0 lemon      (501) staff       (20)     8256 2022-12-31 09:50:28.000000 reader-3.5/src/reader/_sql_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)    24243 2022-12-31 08:26:13.000000 reader-3.5/src/reader/_sqlite_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)    53091 2023-03-03 21:46:46.000000 reader-3.5/src/reader/_storage.py
--rw-r--r--   0 lemon      (501) staff       (20)    16419 2023-03-14 06:54:33.000000 reader-3.5/src/reader/_types.py
--rw-r--r--   0 lemon      (501) staff       (20)    16725 2022-12-31 08:26:13.000000 reader-3.5/src/reader/_update.py
--rw-r--r--   0 lemon      (501) staff       (20)     4224 2022-12-31 08:10:27.000000 reader-3.5/src/reader/_url_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)     9052 2022-12-31 08:26:29.000000 reader-3.5/src/reader/_utils.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-03-18 22:57:52.310797 reader-3.5/src/reader/_vendor/
--rw-r--r--   0 lemon      (501) staff       (20)        0 2020-10-28 07:24:12.000000 reader-3.5/src/reader/_vendor/__init__.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-03-18 22:57:52.332810 reader-3.5/src/reader/_vendor/feedparser/
--rw-r--r--   0 lemon      (501) staff       (20)     2715 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)    16169 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/api.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-03-18 22:57:52.342645 reader-3.5/src/reader/_vendor/feedparser/datetimes/
--rw-r--r--   0 lemon      (501) staff       (20)     2905 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/datetimes/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)     2380 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/datetimes/asctime.py
--rw-r--r--   0 lemon      (501) staff       (20)     4022 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/datetimes/greek.py
--rw-r--r--   0 lemon      (501) staff       (20)     2945 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/datetimes/hungarian.py
--rw-r--r--   0 lemon      (501) staff       (20)     5459 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/datetimes/iso8601.py
--rw-r--r--   0 lemon      (501) staff       (20)     3354 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/datetimes/korean.py
--rw-r--r--   0 lemon      (501) staff       (20)     2198 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/datetimes/perforce.py
--rw-r--r--   0 lemon      (501) staff       (20)     5423 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/datetimes/rfc822.py
--rw-r--r--   0 lemon      (501) staff       (20)     4506 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/datetimes/w3dtf.py
--rw-r--r--   0 lemon      (501) staff       (20)    21181 2022-02-12 10:04:56.000000 reader-3.5/src/reader/_vendor/feedparser/encodings.py
--rw-r--r--   0 lemon      (501) staff       (20)     1897 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/exceptions.py
--rw-r--r--   0 lemon      (501) staff       (20)    10791 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/html.py
--rw-r--r--   0 lemon      (501) staff       (20)     9834 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/http.py
--rw-r--r--   0 lemon      (501) staff       (20)    32296 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/mixin.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-03-18 22:57:52.356204 reader-3.5/src/reader/_vendor/feedparser/namespaces/
--rw-r--r--   0 lemon      (501) staff       (20)        0 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/namespaces/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)    16998 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/namespaces/_base.py
--rw-r--r--   0 lemon      (501) staff       (20)     2317 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/namespaces/admin.py
--rw-r--r--   0 lemon      (501) staff       (20)     2866 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/namespaces/cc.py
--rw-r--r--   0 lemon      (501) staff       (20)     4446 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/namespaces/dc.py
--rw-r--r--   0 lemon      (501) staff       (20)    11399 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/namespaces/georss.py
--rw-r--r--   0 lemon      (501) staff       (20)     4115 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/namespaces/itunes.py
--rw-r--r--   0 lemon      (501) staff       (20)     5336 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/namespaces/mediarss.py
--rw-r--r--   0 lemon      (501) staff       (20)     2839 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/namespaces/psc.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-03-18 22:57:52.362507 reader-3.5/src/reader/_vendor/feedparser/parsers/
--rw-r--r--   0 lemon      (501) staff       (20)        0 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/parsers/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)     4729 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/parsers/json.py
--rw-r--r--   0 lemon      (501) staff       (20)     3420 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/parsers/loose.py
--rw-r--r--   0 lemon      (501) staff       (20)     5805 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/parsers/strict.py
--rw-r--r--   0 lemon      (501) staff       (20)        0 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/py.typed
--rw-r--r--   0 lemon      (501) staff       (20)    23731 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/sanitizer.py
--rw-r--r--   0 lemon      (501) staff       (20)     3517 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/sgml.py
--rw-r--r--   0 lemon      (501) staff       (20)     5487 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/urls.py
--rw-r--r--   0 lemon      (501) staff       (20)     6448 2022-02-11 15:50:56.000000 reader-3.5/src/reader/_vendor/feedparser/util.py
--rw-r--r--   0 lemon      (501) staff       (20)    71228 2023-03-13 22:26:15.000000 reader-3.5/src/reader/core.py
--rw-r--r--   0 lemon      (501) staff       (20)     6149 2022-12-31 08:26:06.000000 reader-3.5/src/reader/exceptions.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-03-18 22:57:52.368661 reader-3.5/src/reader/plugins/
--rw-r--r--   0 lemon      (501) staff       (20)     1503 2022-12-31 08:26:13.000000 reader-3.5/src/reader/plugins/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)      798 2021-03-26 12:03:04.000000 reader-3.5/src/reader/plugins/enclosure_dedupe.py
--rw-r--r--   0 lemon      (501) staff       (20)    16705 2023-01-29 20:48:33.000000 reader-3.5/src/reader/plugins/entry_dedupe.py
--rw-r--r--   0 lemon      (501) staff       (20)     2734 2023-03-18 22:45:04.000000 reader-3.5/src/reader/plugins/mark_as_read.py
--rw-r--r--   0 lemon      (501) staff       (20)     4678 2022-09-14 19:27:33.000000 reader-3.5/src/reader/plugins/readtime.py
--rw-r--r--   0 lemon      (501) staff       (20)     1626 2022-12-18 09:01:52.000000 reader-3.5/src/reader/plugins/ua_fallback.py
--rw-r--r--   0 lemon      (501) staff       (20)        0 2022-06-28 20:04:35.000000 reader-3.5/src/reader/py.typed
--rw-r--r--   0 lemon      (501) staff       (20)    28282 2023-03-18 22:18:25.000000 reader-3.5/src/reader/types.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-03-18 22:57:52.277645 reader-3.5/src/reader.egg-info/
--rw-r--r--   0 lemon      (501) staff       (20)     5412 2023-03-18 22:57:52.000000 reader-3.5/src/reader.egg-info/PKG-INFO
--rw-r--r--   0 lemon      (501) staff       (20)     6273 2023-03-18 22:57:52.000000 reader-3.5/src/reader.egg-info/SOURCES.txt
--rw-r--r--   0 lemon      (501) staff       (20)        1 2023-03-18 22:57:52.000000 reader-3.5/src/reader.egg-info/dependency_links.txt
--rw-r--r--   0 lemon      (501) staff       (20)      658 2023-03-18 22:57:52.000000 reader-3.5/src/reader.egg-info/requires.txt
--rw-r--r--   0 lemon      (501) staff       (20)        7 2023-03-18 22:57:52.000000 reader-3.5/src/reader.egg-info/top_level.txt
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-03-18 22:57:52.448157 reader-3.5/tests/
--rw-r--r--   0 lemon      (501) staff       (20)     4829 2023-03-05 10:19:51.000000 reader-3.5/tests/conftest.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-03-18 22:57:52.694044 reader-3.5/tests/data/
--rw-r--r--   0 lemon      (501) staff       (20)       69 2021-10-18 18:44:15.000000 reader-3.5/tests/data/10.json
--rw-r--r--   0 lemon      (501) staff       (20)      231 2022-12-31 08:17:15.000000 reader-3.5/tests/data/10.json.py
--rw-r--r--   0 lemon      (501) staff       (20)       12 2021-01-28 12:46:50.000000 reader-3.5/tests/data/custom
--rw-r--r--   0 lemon      (501) staff       (20)      180 2020-10-28 07:20:07.000000 reader-3.5/tests/data/empty.atom
--rw-r--r--   0 lemon      (501) staff       (20)      446 2022-12-31 08:17:17.000000 reader-3.5/tests/data/empty.atom.py
--rw-r--r--   0 lemon      (501) staff       (20)      157 2021-01-28 10:55:34.000000 reader-3.5/tests/data/empty.json
--rw-r--r--   0 lemon      (501) staff       (20)      455 2022-12-31 08:17:15.000000 reader-3.5/tests/data/empty.json.py
--rw-r--r--   0 lemon      (501) staff       (20)      191 2020-10-28 07:20:07.000000 reader-3.5/tests/data/empty.rss
--rw-r--r--   0 lemon      (501) staff       (20)      326 2022-12-31 08:17:16.000000 reader-3.5/tests/data/empty.rss.py
--rw-r--r--   0 lemon      (501) staff       (20)     1551 2022-03-26 15:46:54.000000 reader-3.5/tests/data/full.atom
--rw-r--r--   0 lemon      (501) staff       (20)     2327 2022-12-31 08:17:15.000000 reader-3.5/tests/data/full.atom.py
--rw-r--r--   0 lemon      (501) staff       (20)     1743 2021-10-18 18:27:51.000000 reader-3.5/tests/data/full.json
--rw-r--r--   0 lemon      (501) staff       (20)     1760 2022-12-31 08:17:16.000000 reader-3.5/tests/data/full.json.py
--rw-r--r--   0 lemon      (501) staff       (20)     1401 2021-06-08 19:16:41.000000 reader-3.5/tests/data/full.rss
--rw-r--r--   0 lemon      (501) staff       (20)     1523 2022-12-31 08:17:15.000000 reader-3.5/tests/data/full.rss.py
--rw-r--r--   0 lemon      (501) staff       (20)     2024 2021-01-28 13:31:45.000000 reader-3.5/tests/data/invalid.json
--rw-r--r--   0 lemon      (501) staff       (20)     1290 2022-12-31 08:17:16.000000 reader-3.5/tests/data/invalid.json.py
--rw-r--r--   0 lemon      (501) staff       (20)      577 2020-10-28 07:22:29.000000 reader-3.5/tests/data/relative.atom
--rw-r--r--   0 lemon      (501) staff       (20)      906 2022-12-31 08:17:20.000000 reader-3.5/tests/data/relative.atom.py
--rw-r--r--   0 lemon      (501) staff       (20)      560 2020-10-28 07:22:29.000000 reader-3.5/tests/data/relative.rss
--rw-r--r--   0 lemon      (501) staff       (20)      907 2022-12-31 08:17:15.000000 reader-3.5/tests/data/relative.rss.py
--rw-r--r--   0 lemon      (501) staff       (20)      629 2021-01-28 18:18:08.000000 reader-3.5/tests/data/sqlite_releases.html
--rw-r--r--   0 lemon      (501) staff       (20)       72 2021-10-18 18:48:17.000000 reader-3.5/tests/data/unknown.json
--rw-r--r--   0 lemon      (501) staff       (20)      234 2022-12-31 08:17:17.000000 reader-3.5/tests/data/unknown.json.py
--rw-r--r--   0 lemon      (501) staff       (20)     4468 2023-01-17 22:12:52.000000 reader-3.5/tests/fakeparser.py
--rw-r--r--   0 lemon      (501) staff       (20)     2440 2023-03-05 10:19:51.000000 reader-3.5/tests/reader_methods.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-03-18 22:57:52.700057 reader-3.5/tests/reader_test_plugins/
--rw-r--r--   0 lemon      (501) staff       (20)        0 2022-03-27 11:01:36.000000 reader-3.5/tests/reader_test_plugins/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)       34 2022-03-27 11:03:08.000000 reader-3.5/tests/reader_test_plugins/good.py
--rw-r--r--   0 lemon      (501) staff       (20)       59 2022-07-25 20:59:03.000000 reader-3.5/tests/reader_test_plugins/init_error.py
--rw-r--r--   0 lemon      (501) staff       (20)       73 2022-03-27 11:08:08.000000 reader-3.5/tests/reader_test_plugins/missing_dependency.py
--rw-r--r--   0 lemon      (501) staff       (20)       24 2022-03-27 11:08:24.000000 reader-3.5/tests/reader_test_plugins/missing_entry_point.py
--rw-r--r--   0 lemon      (501) staff       (20)     5534 2023-03-05 10:19:52.000000 reader-3.5/tests/test__types.py
--rw-r--r--   0 lemon      (501) staff       (20)     8655 2022-12-27 22:17:34.000000 reader-3.5/tests/test_app.py
--rw-r--r--   0 lemon      (501) staff       (20)      654 2020-10-28 07:22:21.000000 reader-3.5/tests/test_app_wsgi.py
--rw-r--r--   0 lemon      (501) staff       (20)     1028 2021-01-28 18:37:51.000000 reader-3.5/tests/test_bench.py
--rw-r--r--   0 lemon      (501) staff       (20)    11712 2023-01-23 15:26:55.000000 reader-3.5/tests/test_cli.py
--rw-r--r--   0 lemon      (501) staff       (20)     3055 2021-03-26 16:15:01.000000 reader-3.5/tests/test_config.py
--rw-r--r--   0 lemon      (501) staff       (20)     1815 2022-07-25 20:59:03.000000 reader-3.5/tests/test_exceptions.py
--rw-r--r--   0 lemon      (501) staff       (20)     2477 2021-03-19 09:00:44.000000 reader-3.5/tests/test_hash_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)     2246 2022-08-21 15:09:18.000000 reader-3.5/tests/test_html_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)     1338 2022-11-21 13:33:45.000000 reader-3.5/tests/test_http_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)     3156 2022-12-18 23:10:11.000000 reader-3.5/tests/test_lazy_imports.py
--rw-r--r--   0 lemon      (501) staff       (20)    33547 2023-01-23 15:11:14.000000 reader-3.5/tests/test_parser.py
--rw-r--r--   0 lemon      (501) staff       (20)      702 2021-11-04 22:22:57.000000 reader-3.5/tests/test_plugins_cli_status.py
--rw-r--r--   0 lemon      (501) staff       (20)      915 2022-12-31 08:17:15.000000 reader-3.5/tests/test_plugins_enclosure_dedupe.py
--rw-r--r--   0 lemon      (501) staff       (20)    22348 2023-01-29 21:01:09.000000 reader-3.5/tests/test_plugins_entry_dedupe.py
--rw-r--r--   0 lemon      (501) staff       (20)     3393 2023-01-29 20:48:19.000000 reader-3.5/tests/test_plugins_mark_as_read.py
--rw-r--r--   0 lemon      (501) staff       (20)     3159 2022-12-27 22:17:35.000000 reader-3.5/tests/test_plugins_preview_feed_list.py
--rw-r--r--   0 lemon      (501) staff       (20)     6610 2022-09-14 19:27:33.000000 reader-3.5/tests/test_plugins_readtime.py
--rw-r--r--   0 lemon      (501) staff       (20)     2467 2023-01-23 15:09:42.000000 reader-3.5/tests/test_plugins_sqlite_releases.py
--rw-r--r--   0 lemon      (501) staff       (20)      118 2020-10-28 07:22:21.000000 reader-3.5/tests/test_plugins_tumblr_gdpr.py
--rw-r--r--   0 lemon      (501) staff       (20)    34750 2022-11-06 15:48:05.000000 reader-3.5/tests/test_plugins_twitter.py
--rw-r--r--   0 lemon      (501) staff       (20)     1070 2022-12-31 08:17:15.000000 reader-3.5/tests/test_plugins_ua_fallback.py
--rw-r--r--   0 lemon      (501) staff       (20)    94505 2023-03-05 10:19:56.000000 reader-3.5/tests/test_reader.py
--rw-r--r--   0 lemon      (501) staff       (20)     8018 2022-07-30 08:23:00.000000 reader-3.5/tests/test_reader_context.py
--rw-r--r--   0 lemon      (501) staff       (20)       99 2021-07-17 15:02:59.000000 reader-3.5/tests/test_reader_deprecations.py
--rw-r--r--   0 lemon      (501) staff       (20)     8028 2022-12-31 08:17:16.000000 reader-3.5/tests/test_reader_hooks.py
--rw-r--r--   0 lemon      (501) staff       (20)     5885 2023-01-23 15:26:18.000000 reader-3.5/tests/test_reader_integration.py
--rw-r--r--   0 lemon      (501) staff       (20)     2617 2022-07-25 20:59:03.000000 reader-3.5/tests/test_reader_plugins.py
--rw-r--r--   0 lemon      (501) staff       (20)     7248 2022-12-31 08:17:15.000000 reader-3.5/tests/test_reader_private.py
--rw-r--r--   0 lemon      (501) staff       (20)    33613 2022-08-21 15:09:18.000000 reader-3.5/tests/test_reader_search.py
--rw-r--r--   0 lemon      (501) staff       (20)     7103 2022-08-29 19:45:44.000000 reader-3.5/tests/test_reader_sort.py
--rw-r--r--   0 lemon      (501) staff       (20)     5683 2022-08-21 15:09:18.000000 reader-3.5/tests/test_search.py
--rw-r--r--   0 lemon      (501) staff       (20)     4724 2021-05-21 12:10:53.000000 reader-3.5/tests/test_sql_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)    11991 2022-03-16 22:01:23.000000 reader-3.5/tests/test_sqlite_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)    17626 2023-03-03 21:47:06.000000 reader-3.5/tests/test_storage.py
--rw-r--r--   0 lemon      (501) staff       (20)    12402 2022-08-21 15:09:18.000000 reader-3.5/tests/test_tags.py
--rw-r--r--   0 lemon      (501) staff       (20)     1129 2020-10-28 07:23:39.000000 reader-3.5/tests/test_test_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)    11006 2022-09-09 21:29:27.000000 reader-3.5/tests/test_types.py
--rw-r--r--   0 lemon      (501) staff       (20)     2516 2022-07-19 22:03:54.000000 reader-3.5/tests/test_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)     3077 2023-01-23 14:51:43.000000 reader-3.5/tests/utils.py
--rw-r--r--   0 lemon      (501) staff       (20)      698 2022-12-29 21:11:03.000000 reader-3.5/tox.ini
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.479325 reader-3.6/
+-rw-r--r--   0 lemon      (501) staff       (20)    54796 2023-06-15 21:40:39.000000 reader-3.6/CHANGES.rst
+-rw-r--r--   0 lemon      (501) staff       (20)     1475 2021-04-07 12:51:45.000000 reader-3.6/LICENSE
+-rw-r--r--   0 lemon      (501) staff       (20)      406 2022-06-28 21:13:50.000000 reader-3.6/MANIFEST.in
+-rw-r--r--   0 lemon      (501) staff       (20)     5410 2023-06-15 21:41:04.479606 reader-3.6/PKG-INFO
+-rw-r--r--   0 lemon      (501) staff       (20)     3501 2023-04-30 15:42:17.000000 reader-3.6/README.rst
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.290879 reader-3.6/docs/
+-rw-r--r--   0 lemon      (501) staff       (20)      604 2020-10-28 07:20:55.000000 reader-3.6/docs/Makefile
+-rw-r--r--   0 lemon      (501) staff       (20)     2956 2023-05-04 19:18:28.000000 reader-3.6/docs/api.rst
+-rw-r--r--   0 lemon      (501) staff       (20)     3007 2023-06-08 16:51:43.000000 reader-3.6/docs/app.rst
+-rw-r--r--   0 lemon      (501) staff       (20)       29 2020-10-28 07:20:55.000000 reader-3.6/docs/changelog.rst
+-rw-r--r--   0 lemon      (501) staff       (20)     2164 2023-06-08 16:56:19.000000 reader-3.6/docs/cli.rst
+-rw-r--r--   0 lemon      (501) staff       (20)     3368 2023-06-05 20:23:53.000000 reader-3.6/docs/conf.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1147 2020-10-28 07:23:47.000000 reader-3.6/docs/config.rst
+-rw-r--r--   0 lemon      (501) staff       (20)       33 2023-05-04 06:00:46.000000 reader-3.6/docs/contributing.rst
+-rw-r--r--   0 lemon      (501) staff       (20)     3062 2023-04-29 12:30:57.000000 reader-3.6/docs/dev-app.rst
+-rw-r--r--   0 lemon      (501) staff       (20)    15936 2023-06-08 17:00:43.000000 reader-3.6/docs/dev.rst
+-rw-r--r--   0 lemon      (501) staff       (20)    29113 2023-05-12 22:28:36.000000 reader-3.6/docs/guide.rst
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.291727 reader-3.6/docs/images/
+-rw-r--r--   0 lemon      (501) staff       (20)    36483 2020-10-28 07:20:31.000000 reader-3.6/docs/images/redesign-01.png
+-rw-r--r--   0 lemon      (501) staff       (20)     1595 2023-05-04 19:59:30.000000 reader-3.6/docs/index.rst
+-rw-r--r--   0 lemon      (501) staff       (20)     2920 2022-12-29 21:45:24.000000 reader-3.6/docs/install.rst
+-rw-r--r--   0 lemon      (501) staff       (20)     2227 2023-03-19 14:35:51.000000 reader-3.6/docs/internal.rst
+-rw-r--r--   0 lemon      (501) staff       (20)      810 2020-10-28 07:19:52.000000 reader-3.6/docs/make.bat
+-rw-r--r--   0 lemon      (501) staff       (20)     2092 2022-07-08 20:32:37.000000 reader-3.6/docs/plugins.rst
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.315450 reader-3.6/docs/screenshots/
+-rw-r--r--   0 lemon      (501) staff       (20)    68106 2020-10-28 07:20:31.000000 reader-3.6/docs/screenshots/dillo.png
+-rw-r--r--   0 lemon      (501) staff       (20)   109426 2020-10-28 07:22:31.000000 reader-3.6/docs/screenshots/entries-feed.png
+-rw-r--r--   0 lemon      (501) staff       (20)    96393 2020-10-28 07:22:31.000000 reader-3.6/docs/screenshots/entries.png
+-rw-r--r--   0 lemon      (501) staff       (20)   277564 2022-07-09 07:30:35.000000 reader-3.6/docs/screenshots/entry-one.png
+-rw-r--r--   0 lemon      (501) staff       (20)   128002 2020-10-28 07:22:31.000000 reader-3.6/docs/screenshots/entry-two.png
+-rw-r--r--   0 lemon      (501) staff       (20)    48411 2020-10-28 07:22:31.000000 reader-3.6/docs/screenshots/feeds.png
+-rw-r--r--   0 lemon      (501) staff       (20)   364336 2020-10-28 07:22:31.000000 reader-3.6/docs/screenshots/lynx.png
+-rw-r--r--   0 lemon      (501) staff       (20)   111458 2020-10-28 07:22:31.000000 reader-3.6/docs/screenshots/search.png
+-rw-r--r--   0 lemon      (501) staff       (20)   135812 2022-06-27 22:00:00.000000 reader-3.6/docs/screenshots/twitter-one.png
+-rw-r--r--   0 lemon      (501) staff       (20)   385070 2022-07-01 13:21:27.000000 reader-3.6/docs/screenshots/twitter-two.png
+-rw-r--r--   0 lemon      (501) staff       (20)     9271 2023-01-16 22:55:01.000000 reader-3.6/docs/tutorial.rst
+-rw-r--r--   0 lemon      (501) staff       (20)     2290 2023-05-04 20:38:52.000000 reader-3.6/docs/why.rst
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.322555 reader-3.6/examples/
+-rw-r--r--   0 lemon      (501) staff       (20)     2713 2021-05-05 18:41:19.000000 reader-3.6/examples/config.yaml
+-rw-r--r--   0 lemon      (501) staff       (20)     1639 2023-01-16 23:03:30.000000 reader-3.6/examples/parser_only.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1596 2022-01-20 22:05:30.000000 reader-3.6/examples/podcast.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1819 2020-12-23 13:16:52.000000 reader-3.6/examples/terminal.py
+-rw-r--r--   0 lemon      (501) staff       (20)       90 2021-06-08 13:32:02.000000 reader-3.6/pyproject.toml
+-rwxr-xr-x   0 lemon      (501) staff       (20)     3831 2023-05-04 14:35:44.000000 reader-3.6/run.sh
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.330830 reader-3.6/scripts/
+-rw-r--r--   0 lemon      (501) staff       (20)    53248 2020-06-23 14:22:09.000000 reader-3.6/scripts/.coverage
+-rwxr-xr-x   0 lemon      (501) staff       (20)      559 2023-01-28 10:01:54.000000 reader-3.6/scripts/backup.sh
+-rw-r--r--   0 lemon      (501) staff       (20)    13837 2022-12-31 08:17:16.000000 reader-3.6/scripts/bench.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4340 2022-12-31 08:17:15.000000 reader-3.6/scripts/debug_storage_stats.py
+-rw-r--r--   0 lemon      (501) staff       (20)      356 2022-06-28 20:55:42.000000 reader-3.6/scripts/generate_import_all.py
+-rw-r--r--   0 lemon      (501) staff       (20)     5021 2020-10-28 07:24:20.000000 reader-3.6/scripts/jscontrols.html
+-rw-r--r--   0 lemon      (501) staff       (20)     1211 2020-10-28 07:24:20.000000 reader-3.6/scripts/jscontrols.py
+-rwxr-xr-x   0 lemon      (501) staff       (20)      764 2020-10-28 07:21:42.000000 reader-3.6/scripts/lines.sh
+-rw-r--r--   0 lemon      (501) staff       (20)     4600 2022-12-31 08:17:15.000000 reader-3.6/scripts/release.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3398 2023-06-15 21:41:04.482902 reader-3.6/setup.cfg
+-rw-r--r--   0 lemon      (501) staff       (20)       38 2021-04-26 16:52:55.000000 reader-3.6/setup.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.265334 reader-3.6/src/
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.355346 reader-3.6/src/reader/
+-rw-r--r--   0 lemon      (501) staff       (20)     2532 2023-06-15 21:40:39.000000 reader-3.6/src/reader/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)      381 2020-10-28 07:22:22.000000 reader-3.6/src/reader/__main__.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.362072 reader-3.6/src/reader/_app/
+-rw-r--r--   0 lemon      (501) staff       (20)    22629 2023-03-05 14:28:08.000000 reader-3.6/src/reader/_app/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4329 2022-12-31 08:17:16.000000 reader-3.6/src/reader/_app/api_thing.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1457 2021-10-30 11:02:39.000000 reader-3.6/src/reader/_app/cli.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.363642 reader-3.6/src/reader/_app/static/
+-rw-r--r--   0 lemon      (501) staff       (20)    14735 2022-06-23 20:50:42.000000 reader-3.6/src/reader/_app/static/controls.js
+-rw-r--r--   0 lemon      (501) staff       (20)     4194 2022-06-22 19:10:26.000000 reader-3.6/src/reader/_app/static/style.css
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.370852 reader-3.6/src/reader/_app/templates/
+-rw-r--r--   0 lemon      (501) staff       (20)      980 2021-10-27 17:55:28.000000 reader-3.6/src/reader/_app/templates/add_entry.html
+-rw-r--r--   0 lemon      (501) staff       (20)    12029 2023-03-05 14:26:36.000000 reader-3.6/src/reader/_app/templates/entries.html
+-rw-r--r--   0 lemon      (501) staff       (20)     3200 2023-02-14 22:28:37.000000 reader-3.6/src/reader/_app/templates/entry.html
+-rw-r--r--   0 lemon      (501) staff       (20)     5083 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_app/templates/feeds.html
+-rw-r--r--   0 lemon      (501) staff       (20)     1631 2022-03-11 23:07:17.000000 reader-3.6/src/reader/_app/templates/layout.html
+-rw-r--r--   0 lemon      (501) staff       (20)     9375 2023-03-05 14:18:18.000000 reader-3.6/src/reader/_app/templates/macros.html
+-rw-r--r--   0 lemon      (501) staff       (20)     2569 2022-07-30 08:02:27.000000 reader-3.6/src/reader/_app/templates/metadata.html
+-rw-r--r--   0 lemon      (501) staff       (20)     1515 2021-08-17 08:51:46.000000 reader-3.6/src/reader/_app/templates/tags.html
+-rw-r--r--   0 lemon      (501) staff       (20)     1150 2020-10-28 07:23:44.000000 reader-3.6/src/reader/_app/wsgi.py
+-rw-r--r--   0 lemon      (501) staff       (20)    13132 2022-12-31 08:17:16.000000 reader-3.6/src/reader/_cli.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4587 2022-07-16 20:45:27.000000 reader-3.6/src/reader/_config.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1531 2023-01-17 22:12:52.000000 reader-3.6/src/reader/_feedparser.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4074 2022-12-18 08:53:24.000000 reader-3.6/src/reader/_feedparser_lazy.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2980 2023-03-14 06:52:53.000000 reader-3.6/src/reader/_hash_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2220 2022-12-31 08:18:29.000000 reader-3.6/src/reader/_html_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)     7493 2023-06-08 21:12:49.000000 reader-3.6/src/reader/_http_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)     5677 2023-01-17 22:12:52.000000 reader-3.6/src/reader/_jsonfeed.py
+-rw-r--r--   0 lemon      (501) staff       (20)    24586 2023-03-19 13:56:03.000000 reader-3.6/src/reader/_parser.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.376954 reader-3.6/src/reader/_plugins/
+-rw-r--r--   0 lemon      (501) staff       (20)     1617 2022-12-29 21:54:33.000000 reader-3.6/src/reader/_plugins/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3201 2021-11-05 08:41:21.000000 reader-3.6/src/reader/_plugins/cli_status.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3065 2022-12-29 22:18:56.000000 reader-3.6/src/reader/_plugins/enclosure_tags.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4561 2023-01-01 10:20:44.000000 reader-3.6/src/reader/_plugins/preview_feed_list.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2931 2022-06-27 21:01:33.000000 reader-3.6/src/reader/_plugins/sqlite_releases.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.378209 reader-3.6/src/reader/_plugins/templates/
+-rw-r--r--   0 lemon      (501) staff       (20)      815 2022-12-27 22:01:52.000000 reader-3.6/src/reader/_plugins/templates/preview_feed_list.html
+-rw-r--r--   0 lemon      (501) staff       (20)     2094 2022-11-21 20:16:44.000000 reader-3.6/src/reader/_plugins/tumblr_gdpr.py
+-rw-r--r--   0 lemon      (501) staff       (20)    26547 2023-06-15 21:32:39.000000 reader-3.6/src/reader/_plugins/twitter.py
+-rw-r--r--   0 lemon      (501) staff       (20)     7785 2023-01-17 21:52:55.000000 reader-3.6/src/reader/_requests_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)      726 2023-01-01 10:22:19.000000 reader-3.6/src/reader/_requests_utils_lazy.py
+-rw-r--r--   0 lemon      (501) staff       (20)     5623 2023-01-01 10:41:25.000000 reader-3.6/src/reader/_retrievers.py
+-rw-r--r--   0 lemon      (501) staff       (20)    34166 2023-03-03 21:46:20.000000 reader-3.6/src/reader/_search.py
+-rw-r--r--   0 lemon      (501) staff       (20)     8256 2022-12-31 09:50:28.000000 reader-3.6/src/reader/_sql_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)    24243 2022-12-31 08:26:13.000000 reader-3.6/src/reader/_sqlite_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)    53646 2023-03-19 14:35:50.000000 reader-3.6/src/reader/_storage.py
+-rw-r--r--   0 lemon      (501) staff       (20)    16419 2023-03-14 06:54:33.000000 reader-3.6/src/reader/_types.py
+-rw-r--r--   0 lemon      (501) staff       (20)    16725 2022-12-31 08:26:13.000000 reader-3.6/src/reader/_update.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4224 2022-12-31 08:10:27.000000 reader-3.6/src/reader/_url_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)     9052 2022-12-31 08:26:29.000000 reader-3.6/src/reader/_utils.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.378839 reader-3.6/src/reader/_vendor/
+-rw-r--r--   0 lemon      (501) staff       (20)        0 2020-10-28 07:24:12.000000 reader-3.6/src/reader/_vendor/__init__.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.388612 reader-3.6/src/reader/_vendor/feedparser/
+-rw-r--r--   0 lemon      (501) staff       (20)     2715 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)    16169 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/api.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.395132 reader-3.6/src/reader/_vendor/feedparser/datetimes/
+-rw-r--r--   0 lemon      (501) staff       (20)     2905 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/datetimes/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2380 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/datetimes/asctime.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4022 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/datetimes/greek.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2945 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/datetimes/hungarian.py
+-rw-r--r--   0 lemon      (501) staff       (20)     5459 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/datetimes/iso8601.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3354 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/datetimes/korean.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2198 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/datetimes/perforce.py
+-rw-r--r--   0 lemon      (501) staff       (20)     5423 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/datetimes/rfc822.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4506 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/datetimes/w3dtf.py
+-rw-r--r--   0 lemon      (501) staff       (20)    21181 2022-02-12 10:04:56.000000 reader-3.6/src/reader/_vendor/feedparser/encodings.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1897 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/exceptions.py
+-rw-r--r--   0 lemon      (501) staff       (20)    10791 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/html.py
+-rw-r--r--   0 lemon      (501) staff       (20)     9834 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/http.py
+-rw-r--r--   0 lemon      (501) staff       (20)    32296 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/mixin.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.403217 reader-3.6/src/reader/_vendor/feedparser/namespaces/
+-rw-r--r--   0 lemon      (501) staff       (20)        0 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/namespaces/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)    16998 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/namespaces/_base.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2317 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/namespaces/admin.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2866 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/namespaces/cc.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4446 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/namespaces/dc.py
+-rw-r--r--   0 lemon      (501) staff       (20)    11399 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/namespaces/georss.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4115 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/namespaces/itunes.py
+-rw-r--r--   0 lemon      (501) staff       (20)     5336 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/namespaces/mediarss.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2839 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/namespaces/psc.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.405841 reader-3.6/src/reader/_vendor/feedparser/parsers/
+-rw-r--r--   0 lemon      (501) staff       (20)        0 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/parsers/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4729 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/parsers/json.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3420 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/parsers/loose.py
+-rw-r--r--   0 lemon      (501) staff       (20)     5805 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/parsers/strict.py
+-rw-r--r--   0 lemon      (501) staff       (20)        0 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/py.typed
+-rw-r--r--   0 lemon      (501) staff       (20)    23731 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/sanitizer.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3517 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/sgml.py
+-rw-r--r--   0 lemon      (501) staff       (20)     5487 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/urls.py
+-rw-r--r--   0 lemon      (501) staff       (20)     6448 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/util.py
+-rw-r--r--   0 lemon      (501) staff       (20)    71461 2023-03-19 13:58:22.000000 reader-3.6/src/reader/core.py
+-rw-r--r--   0 lemon      (501) staff       (20)     6149 2022-12-31 08:26:06.000000 reader-3.6/src/reader/exceptions.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.411224 reader-3.6/src/reader/plugins/
+-rw-r--r--   0 lemon      (501) staff       (20)     1503 2022-12-31 08:26:13.000000 reader-3.6/src/reader/plugins/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)      798 2021-03-26 12:03:04.000000 reader-3.6/src/reader/plugins/enclosure_dedupe.py
+-rw-r--r--   0 lemon      (501) staff       (20)    16705 2023-01-29 20:48:33.000000 reader-3.6/src/reader/plugins/entry_dedupe.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2734 2023-03-18 22:45:04.000000 reader-3.6/src/reader/plugins/mark_as_read.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4678 2022-09-14 19:27:33.000000 reader-3.6/src/reader/plugins/readtime.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1626 2022-12-18 09:01:52.000000 reader-3.6/src/reader/plugins/ua_fallback.py
+-rw-r--r--   0 lemon      (501) staff       (20)        0 2022-06-28 20:04:35.000000 reader-3.6/src/reader/py.typed
+-rw-r--r--   0 lemon      (501) staff       (20)    28282 2023-03-18 22:18:25.000000 reader-3.6/src/reader/types.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.358296 reader-3.6/src/reader.egg-info/
+-rw-r--r--   0 lemon      (501) staff       (20)     5410 2023-06-15 21:41:04.000000 reader-3.6/src/reader.egg-info/PKG-INFO
+-rw-r--r--   0 lemon      (501) staff       (20)     6279 2023-06-15 21:41:04.000000 reader-3.6/src/reader.egg-info/SOURCES.txt
+-rw-r--r--   0 lemon      (501) staff       (20)        1 2023-06-15 21:41:04.000000 reader-3.6/src/reader.egg-info/dependency_links.txt
+-rw-r--r--   0 lemon      (501) staff       (20)      653 2023-06-15 21:41:04.000000 reader-3.6/src/reader.egg-info/requires.txt
+-rw-r--r--   0 lemon      (501) staff       (20)        7 2023-06-15 21:41:04.000000 reader-3.6/src/reader.egg-info/top_level.txt
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.455378 reader-3.6/tests/
+-rw-r--r--   0 lemon      (501) staff       (20)     4829 2023-03-05 10:19:51.000000 reader-3.6/tests/conftest.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.475654 reader-3.6/tests/data/
+-rw-r--r--   0 lemon      (501) staff       (20)       69 2021-10-18 18:44:15.000000 reader-3.6/tests/data/10.json
+-rw-r--r--   0 lemon      (501) staff       (20)      231 2022-12-31 08:17:15.000000 reader-3.6/tests/data/10.json.py
+-rw-r--r--   0 lemon      (501) staff       (20)       12 2021-01-28 12:46:50.000000 reader-3.6/tests/data/custom
+-rw-r--r--   0 lemon      (501) staff       (20)      180 2020-10-28 07:20:07.000000 reader-3.6/tests/data/empty.atom
+-rw-r--r--   0 lemon      (501) staff       (20)      446 2022-12-31 08:17:17.000000 reader-3.6/tests/data/empty.atom.py
+-rw-r--r--   0 lemon      (501) staff       (20)      157 2021-01-28 10:55:34.000000 reader-3.6/tests/data/empty.json
+-rw-r--r--   0 lemon      (501) staff       (20)      455 2022-12-31 08:17:15.000000 reader-3.6/tests/data/empty.json.py
+-rw-r--r--   0 lemon      (501) staff       (20)      191 2020-10-28 07:20:07.000000 reader-3.6/tests/data/empty.rss
+-rw-r--r--   0 lemon      (501) staff       (20)      326 2022-12-31 08:17:16.000000 reader-3.6/tests/data/empty.rss.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1551 2022-03-26 15:46:54.000000 reader-3.6/tests/data/full.atom
+-rw-r--r--   0 lemon      (501) staff       (20)     2327 2022-12-31 08:17:15.000000 reader-3.6/tests/data/full.atom.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1743 2021-10-18 18:27:51.000000 reader-3.6/tests/data/full.json
+-rw-r--r--   0 lemon      (501) staff       (20)     1760 2022-12-31 08:17:16.000000 reader-3.6/tests/data/full.json.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1401 2021-06-08 19:16:41.000000 reader-3.6/tests/data/full.rss
+-rw-r--r--   0 lemon      (501) staff       (20)     1523 2022-12-31 08:17:15.000000 reader-3.6/tests/data/full.rss.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2024 2021-01-28 13:31:45.000000 reader-3.6/tests/data/invalid.json
+-rw-r--r--   0 lemon      (501) staff       (20)     1290 2022-12-31 08:17:16.000000 reader-3.6/tests/data/invalid.json.py
+-rw-r--r--   0 lemon      (501) staff       (20)      577 2020-10-28 07:22:29.000000 reader-3.6/tests/data/relative.atom
+-rw-r--r--   0 lemon      (501) staff       (20)      906 2022-12-31 08:17:20.000000 reader-3.6/tests/data/relative.atom.py
+-rw-r--r--   0 lemon      (501) staff       (20)      560 2020-10-28 07:22:29.000000 reader-3.6/tests/data/relative.rss
+-rw-r--r--   0 lemon      (501) staff       (20)      907 2022-12-31 08:17:15.000000 reader-3.6/tests/data/relative.rss.py
+-rw-r--r--   0 lemon      (501) staff       (20)      629 2021-01-28 18:18:08.000000 reader-3.6/tests/data/sqlite_releases.html
+-rw-r--r--   0 lemon      (501) staff       (20)       72 2021-10-18 18:48:17.000000 reader-3.6/tests/data/unknown.json
+-rw-r--r--   0 lemon      (501) staff       (20)      234 2022-12-31 08:17:17.000000 reader-3.6/tests/data/unknown.json.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4468 2023-01-17 22:12:52.000000 reader-3.6/tests/fakeparser.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2440 2023-03-05 10:19:51.000000 reader-3.6/tests/reader_methods.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.478810 reader-3.6/tests/reader_test_plugins/
+-rw-r--r--   0 lemon      (501) staff       (20)        0 2022-03-27 11:01:36.000000 reader-3.6/tests/reader_test_plugins/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)       34 2022-03-27 11:03:08.000000 reader-3.6/tests/reader_test_plugins/good.py
+-rw-r--r--   0 lemon      (501) staff       (20)       59 2022-07-25 20:59:03.000000 reader-3.6/tests/reader_test_plugins/init_error.py
+-rw-r--r--   0 lemon      (501) staff       (20)       73 2022-03-27 11:08:08.000000 reader-3.6/tests/reader_test_plugins/missing_dependency.py
+-rw-r--r--   0 lemon      (501) staff       (20)       24 2022-03-27 11:08:24.000000 reader-3.6/tests/reader_test_plugins/missing_entry_point.py
+-rw-r--r--   0 lemon      (501) staff       (20)     5534 2023-03-05 10:19:52.000000 reader-3.6/tests/test__types.py
+-rw-r--r--   0 lemon      (501) staff       (20)     9097 2023-06-08 21:15:29.000000 reader-3.6/tests/test_app.py
+-rw-r--r--   0 lemon      (501) staff       (20)      654 2020-10-28 07:22:21.000000 reader-3.6/tests/test_app_wsgi.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1028 2021-01-28 18:37:51.000000 reader-3.6/tests/test_bench.py
+-rw-r--r--   0 lemon      (501) staff       (20)    11712 2023-01-23 15:26:55.000000 reader-3.6/tests/test_cli.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3055 2021-03-26 16:15:01.000000 reader-3.6/tests/test_config.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1815 2022-07-25 20:59:03.000000 reader-3.6/tests/test_exceptions.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2477 2021-03-19 09:00:44.000000 reader-3.6/tests/test_hash_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2246 2022-08-21 15:09:18.000000 reader-3.6/tests/test_html_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1319 2023-04-30 09:15:21.000000 reader-3.6/tests/test_http_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3229 2023-04-30 09:15:21.000000 reader-3.6/tests/test_lazy_imports.py
+-rw-r--r--   0 lemon      (501) staff       (20)    33547 2023-01-23 15:11:14.000000 reader-3.6/tests/test_parser.py
+-rw-r--r--   0 lemon      (501) staff       (20)      702 2021-11-04 22:22:57.000000 reader-3.6/tests/test_plugins_cli_status.py
+-rw-r--r--   0 lemon      (501) staff       (20)      915 2022-12-31 08:17:15.000000 reader-3.6/tests/test_plugins_enclosure_dedupe.py
+-rw-r--r--   0 lemon      (501) staff       (20)    22348 2023-01-29 21:01:09.000000 reader-3.6/tests/test_plugins_entry_dedupe.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3393 2023-01-29 20:48:19.000000 reader-3.6/tests/test_plugins_mark_as_read.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3159 2022-12-27 22:17:35.000000 reader-3.6/tests/test_plugins_preview_feed_list.py
+-rw-r--r--   0 lemon      (501) staff       (20)     6610 2022-09-14 19:27:33.000000 reader-3.6/tests/test_plugins_readtime.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2467 2023-01-23 15:09:42.000000 reader-3.6/tests/test_plugins_sqlite_releases.py
+-rw-r--r--   0 lemon      (501) staff       (20)      118 2020-10-28 07:22:21.000000 reader-3.6/tests/test_plugins_tumblr_gdpr.py
+-rw-r--r--   0 lemon      (501) staff       (20)    34750 2022-11-06 15:48:05.000000 reader-3.6/tests/test_plugins_twitter.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1070 2022-12-31 08:17:15.000000 reader-3.6/tests/test_plugins_ua_fallback.py
+-rw-r--r--   0 lemon      (501) staff       (20)    94505 2023-03-05 10:19:56.000000 reader-3.6/tests/test_reader.py
+-rw-r--r--   0 lemon      (501) staff       (20)     8018 2022-07-30 08:23:00.000000 reader-3.6/tests/test_reader_context.py
+-rw-r--r--   0 lemon      (501) staff       (20)       99 2021-07-17 15:02:59.000000 reader-3.6/tests/test_reader_deprecations.py
+-rw-r--r--   0 lemon      (501) staff       (20)     8028 2022-12-31 08:17:16.000000 reader-3.6/tests/test_reader_hooks.py
+-rw-r--r--   0 lemon      (501) staff       (20)     5885 2023-01-23 15:26:18.000000 reader-3.6/tests/test_reader_integration.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2617 2022-07-25 20:59:03.000000 reader-3.6/tests/test_reader_plugins.py
+-rw-r--r--   0 lemon      (501) staff       (20)     7248 2022-12-31 08:17:15.000000 reader-3.6/tests/test_reader_private.py
+-rw-r--r--   0 lemon      (501) staff       (20)    33613 2022-08-21 15:09:18.000000 reader-3.6/tests/test_reader_search.py
+-rw-r--r--   0 lemon      (501) staff       (20)     7103 2022-08-29 19:45:44.000000 reader-3.6/tests/test_reader_sort.py
+-rw-r--r--   0 lemon      (501) staff       (20)     5683 2022-08-21 15:09:18.000000 reader-3.6/tests/test_search.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4724 2021-05-21 12:10:53.000000 reader-3.6/tests/test_sql_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)    11991 2022-03-16 22:01:23.000000 reader-3.6/tests/test_sqlite_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)    17626 2023-03-03 21:47:06.000000 reader-3.6/tests/test_storage.py
+-rw-r--r--   0 lemon      (501) staff       (20)    12402 2022-08-21 15:09:18.000000 reader-3.6/tests/test_tags.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1129 2020-10-28 07:23:39.000000 reader-3.6/tests/test_test_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)    11006 2022-09-09 21:29:27.000000 reader-3.6/tests/test_types.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2516 2022-07-19 22:03:54.000000 reader-3.6/tests/test_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3077 2023-01-23 14:51:43.000000 reader-3.6/tests/utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)      698 2022-12-29 21:11:03.000000 reader-3.6/tox.ini
```

### Comparing `reader-3.5/CHANGES.rst` & `reader-3.6/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,36 @@
 Changelog
 =========
 
 .. module:: reader
   :noindex:
 
 
+Version 3.6
+-----------
+
+Released 2023-06-16
+
+* Add documentation on :doc:`contributing`. (:issue:`60`)
+* Add a detailed :ref:`roadmap`. (:issue:`60`)
+* Document the low-level
+  :meth:`~reader._storage.Storage.delete_entries`
+  storage method.
+  (:issue:`301`, :issue:`96`)
+* Update vendored ``reader._http_utils`` to werkzeug 2.3.5.
+
+* Deprecate the (experimental) :mod:`~reader._plugins.twitter` plugin,
+  since the Twitter API does not have a (useful) free tier anymore.
+  (:issue:`310`)
+
+  .. attention::
+
+    The :mod:`~reader._plugins.twitter` plugin will be removed in version 3.7.
+
+
 Version 3.5
 -----------
 
 Released 2023-03-19
 
 * Make :attr:`Entry.important` an *optional* boolean
   defaulting to :const:`None`,
@@ -653,15 +675,15 @@
 
   This is allows supplying a user-defined ``json_array_length`` function
   on platforms where SQLite doesn't come with the JSON1 extension
   (e.g. on Windows with stock Python earlier than 3.9;
   `details <https://github.com/lemon24/reader/issues/163#issuecomment-895041943>`_).
 
   Note these globals are private, and thus *not* covered by the
-  :doc:`backwards compatibility policy <compat>`.
+  :ref:`backwards compatibility policy <compat>`.
 
 
 Version 2.0
 -----------
 
 Released 2021-07-17
```

### Comparing `reader-3.5/LICENSE` & `reader-3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `reader-3.5/PKG-INFO` & `reader-3.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reader
-Version: 3.5
+Version: 3.6
 Summary: A Python feed reader library.
 Home-page: https://github.com/lemon24/reader
 Author: lemon24
 License: BSD-3-Clause
 Project-URL: Changes, https://reader.readthedocs.io/en/latest/changelog.html
 Project-URL: Documentation, https://reader.readthedocs.io/
 Project-URL: Issue tracker, https://github.com/lemon24/reader/issues
@@ -58,16 +58,16 @@
 |build-status-github| |code-coverage| |documentation-status| |pypi-status| |type-checking| |code-style|
 
 
 .. |build-status-github| image:: https://github.com/lemon24/reader/workflows/build/badge.svg
   :target: https://github.com/lemon24/reader/actions?query=workflow%3Abuild
   :alt: build status (GitHub Actions)
 
-.. |code-coverage| image:: https://codecov.io/github/lemon24/reader/coverage.svg?branch=master
-  :target: https://codecov.io/github/lemon24/reader?branch=master
+.. |code-coverage| image:: https://codecov.io/gh/lemon24/reader/branch/master/graph/badge.svg?token=lcLZaSFysf
+  :target: https://codecov.io/gh/lemon24/reader
   :alt: code coverage
 
 .. |documentation-status| image:: https://readthedocs.org/projects/reader/badge/?version=latest&style=flat
   :target: https://reader.readthedocs.io/en/latest/?badge=latest
   :alt: documentation status
 
 .. |pypi-status| image:: https://img.shields.io/pypi/v/reader.svg
```

### Comparing `reader-3.5/README.rst` & `reader-3.6/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 |build-status-github| |code-coverage| |documentation-status| |pypi-status| |type-checking| |code-style|
 
 
 .. |build-status-github| image:: https://github.com/lemon24/reader/workflows/build/badge.svg
   :target: https://github.com/lemon24/reader/actions?query=workflow%3Abuild
   :alt: build status (GitHub Actions)
 
-.. |code-coverage| image:: https://codecov.io/github/lemon24/reader/coverage.svg?branch=master
-  :target: https://codecov.io/github/lemon24/reader?branch=master
+.. |code-coverage| image:: https://codecov.io/gh/lemon24/reader/branch/master/graph/badge.svg?token=lcLZaSFysf
+  :target: https://codecov.io/gh/lemon24/reader
   :alt: code coverage
 
 .. |documentation-status| image:: https://readthedocs.org/projects/reader/badge/?version=latest&style=flat
   :target: https://reader.readthedocs.io/en/latest/?badge=latest
   :alt: documentation status
 
 .. |pypi-status| image:: https://img.shields.io/pypi/v/reader.svg
```

### Comparing `reader-3.5/docs/Makefile` & `reader-3.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reader-3.5/docs/api.rst` & `reader-3.6/docs/api.rst`

 * *Files identical despite different names*

### Comparing `reader-3.5/docs/app.rst` & `reader-3.6/docs/app.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 *reader* comes with a minimal web application, intended to work across
 all browsers, including light-weight / text-only ones.
 
 
 .. warning::
 
-    The web application is not stable yet and might change without any notice.
+    The web application is not fully supported,
+    see the :ref:`roadmap <app roadmap>` for details.
 
 .. note::
 
     The web application is optional, use the ``app`` extra to install
     its :ref:`dependencies <Optional dependencies>`.
```

### Comparing `reader-3.5/docs/cli.rst` & `reader-3.6/docs/cli.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 
 Command-line interface
 ======================
 
-This part of the documentation covers the *reader* command-line interface.
+*reader* comes with a command-line interface
+that exposes basic management functionality.
+
 
 .. warning::
 
-    The CLI is not stable yet and might change without any notice.
+    The CLI is is not fully stable,
+    see the :ref:`roadmap <cli roadmap>` for details.
 
 .. note::
 
     The command-line interface is optional, use the ``cli`` extra to install
     its :ref:`dependencies <Optional dependencies>`.
 
 Most commands need a database to work. The following are equivalent:
```

### Comparing `reader-3.5/docs/conf.py` & `reader-3.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/docs/config.rst` & `reader-3.6/docs/config.rst`

 * *Files identical despite different names*

### Comparing `reader-3.5/docs/dev-app.rst` & `reader-3.6/docs/dev-app.rst`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,23 @@
 
 Fast and ugly is better than slow and pretty.
 
 It should be possible to build a decent web interface (at least for reader)
 using only HTML forms with a few JavaScript enhancements added on top.
 
 
+2023 update: `Hypermedia Systems`_ and `htmx`_ seem to embody these ideas
+in a much better way than I could;
+a potential web app re-design will likely use them.
+
+
+.. _Hypermedia Systems: https://hypermedia.systems/
+.. _htmx: https://htmx.org/
+
+
 User interactions
 ~~~~~~~~~~~~~~~~~
 
 .. note::
 
     This list might lag behind reality; anyway, it all started from here.
```

### Comparing `reader-3.5/docs/dev.rst` & `reader-3.6/docs/dev.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,127 +1,217 @@
 
 Development
 ===========
 
+.. module:: reader
+  :noindex:
 
-Goals
------
-
-Goals:
-
-* clearly documented API
-* minimal web interface
-* minimal CLI
 
 Development should follow a problem-solution_ approach.
 
+.. seealso:: :ref:`philosophy`
+
 .. _problem-solution: https://hintjens.gitbooks.io/scalable-c/content/chapter1.html#problem-what-do-we-do-next
 
 
+
+.. _roadmap:
+
 Roadmap
 -------
 
-In no particular order:
+The plan is to continue evolving the library
+to support as many "feed reader application" use cases as possible,
+while still following the :ref:`philosophy`.
+Even if a specific feature is not a good fit for the library itself,
+it should be possible to find a more generic solution
+that makes it possible to build the feature on top.
 
-* Internal API stabilization.
-* CLI stabilization.
-* Web application re-design.
-* Web application stabilization.
+Following is an unsorted, non-exhausive list of known areas for improvement.
+I am working on *reader* based on my current interests,
+in my spare time,
+but I will prioritize supporting :doc:`contributors <contributing>`
+(discussions, reviews and so on).
 
-Also see open issues: https://github.com/lemon24/reader/issues
+* OPML support, :issue:`165`
+* :ref:`deleting entries <deleting entries>`
+* more feed interaction statistics, :issue:`254`
 
+* security
 
-Supported Python versions
--------------------------
+  * XML safety, :issue:`212`
+  * sanitization unification, likely as a plugin, :issue:`125` and :issue:`227`
+  * relative link resolution unification, :issue:`125`
 
-The oldest Python version reader should support is:
+* sorting
 
-* the newest CPython available on the latest Ubuntu LTS (3 months after LTS release)
-* at least 1 stable PyPy version
+  * reverse order, :issue:`201`
+  * sort by unread entries, :issue:`245`
+  * sort by "recently interacted with", :issue:`294`
+  * better feed title sort, :issue:`250`
+  * sort feeds by entry counts, including :attr:`~EntryCounts.averages`
 
-This usually ends up being the last 3 stable CPython versions.
+* resource tags
 
+  * :ref:`searchable tag values <searchable tags>`, e.g. for comments
+  * :ref:`unification with entry.read/important <entry flag unification>`
+  * filter entries by entry tags
+  * optimistic locking, :issue:`308`
+  * filter tags by prefix, :issue:`309`
 
-Style guide
------------
 
-*reader* uses the `Black <https://black.readthedocs.io/en/stable/>`_ style.
+* HTTP compliance, likely as plugins
 
-You should enforce it by using `pre-commit <https://pre-commit.com/>`_.
-To install it into your git hooks, run::
+  * 301 Moved Permanently, :issue:`246`
+  * 410 Gone, :issue:`246`
+  * 429 Too Many Requests, :issue:`307`
 
-    pip install pre-commit  # ./run.sh install-dev already does both
-    pre-commit install
+* add more fields to data objects
 
-Every time you clone the repo, running ``pre-commit install`` should always be
-the first thing you do.
+  * entry source, :issue:`276`
+  * extra data, as an escape hatch, :issue:`277`
 
+* :ref:`multiple storage implementations <multiple storage implementations>`
+* :ref:`batch get methods <batch get methods>`
+* :doc:`internal` stabilization
+* arbitrary website scraping, :issue:`222`
+* :ref:`feed categories <categories>`, likely as a plugin
 
-Testing
--------
 
-First, install the testing dependencies::
+.. seealso::
 
-    ./run.sh install-dev    # or
-    pip install '.[dev]'
+    `Open issues`_ and :ref:`Design notes`.
 
-Run tests using the current Python interpreter::
+.. _open issues: https://github.com/lemon24/reader/issues
 
-    pytest --runslow
 
-Run tests using the current Python interpreter, but skip slow tests::
+.. _cli roadmap:
 
-    pytest
+Command-line interface
+~~~~~~~~~~~~~~~~~~~~~~
 
-Run tests for all supported Python versions::
+The :doc:`cli` is more or less stable,\ [*]_
+although both the output and config loading need more polish
+and additional tests.
 
-    tox
+A full-blown terminal feed reader is *not* in scope,
+since I don't need one,
+but I'm not opposed to the idea.
 
-Run tests with coverage and generate an HTML report (in ``./htmlcov``)::
+.. [*] With the exception of ``serve``, which is provided by the web app.
 
-    ./run.sh coverage-all
 
-Run the type checker::
+.. _app roadmap:
 
-    ./run.sh typing         # or
-    mypy --strict src
+Web application
+~~~~~~~~~~~~~~~
 
-Start a local development server for the web application::
+The :doc:`app` is "unsupported",
+in that it's not all that polished,
+and I don't have time to do major improvments.
+But, I am using it daily,
+and it will keep working until a better one exists.
 
-    ./run.sh serve-dev      # or
+Long term, I'd like to:
 
-    FLASK_DEBUG=1 FLASK_TRAP_BAD_REQUEST_ERRORS=1 \
-    FLASK_APP=src/reader/_app/wsgi.py \
-    READER_DB=db.sqlite flask run -h 0.0.0.0 -p 8000
+* re-design it from scratch to improve usability
+* switch to `htmx`_ instead of using a home-grown solution
+* spin it off into a separate package/project
 
+.. _htmx: https://htmx.org/
 
-Building the documentation
---------------------------
 
-First, install the dependencies::
 
-    pip install '.[docs]'   # ./run.sh install-dev already does it for you
+.. _compat:
 
-The documentation is built with Sphinx::
+Backwards compatibility
+-----------------------
 
-    ./run.sh docs           # or
-    make -C docs html       # using Sphinx's Makefile directly
+*reader* uses `semantic versioning`_.
 
-The built HTML docs should be in ``./docs/_build/html/``.
+Breaking compatibility is done by incrementing the major version,
+announcing it in the :doc:`changelog`,
+and raising deprecation warnings for at least one minor version
+before the new major version is released (if possible).
 
+There may be minor exceptions to this,
+e.g. bug fixes and gross violation of specifications;
+they will be announced in the :doc:`changelog`
+with a **This is a minor compatibility break** warning.
 
-Making a release
-----------------
+Schema migrations for the default storage must happen automatically.
+Migrations can be removed in new major versions,
+with at least 3 months provided since the last migration.
 
-Making a release (from ``x`` to ``y`` == ``x + 1``):
+.. _semantic versioning: https://semver.org/
+
+
+What is the public API
+~~~~~~~~~~~~~~~~~~~~~~
+
+*reader* follows the `PEP 8 definition`_ of public interface.
+
+The following are part of the public API:
+
+* Every interface documented in the :doc:`API reference <api>`.
+* Any (documented) module, function, object, method, and attribute,
+  defined in the *reader* package,
+  that is accessible without passing through a name
+  that starts with underscore.
+* The number and position of positional arguments.
+* The names of keyword arguments.
+* Argument types (argument types cannot become more strict).
+* Attribute types (attribute types cannot become less strict).
+
+Undocumented type aliases (even if not private)
+are **not** part of the public API.
+
+Other exceptions are possible; they will be marked aggresively as such.
+
+.. _PEP 8 definition: https://www.python.org/dev/peps/pep-0008/#public-and-internal-interfaces
+
+
+.. seealso::
+
+  The `Twisted Compatibility Policy <https://github.com/twisted/twisted/blob/twisted-16.2.0/docs/core/development/policy/compatibility-policy.rst>`_,
+  which served as inspiration for this.
+
+
+Supported Python versions
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The oldest Python version reader should support is:
+
+* the newest CPython available on the latest Ubuntu LTS (3 months after LTS release)
+* at least 1 stable PyPy version
+
+This usually ends up being the last 3 stable CPython versions.
+
+Dropping support for a Python version should be announced
+at least 1 release prior.
+
+
+
+Releases
+--------
+
+For convenience, *reader* only releases major and minor versions
+(bugfixes go in minor versions).
+Changes go only to the next release (no backports).
+
+
+Making a release
+~~~~~~~~~~~~~~~~
 
 .. note::
 
     :gh:`scripts/release.py <scripts/release.py>` already does most of these.
 
+Making a release (from ``x`` to ``y`` == ``x + 1``):
+
 * (release.py) bump version in ``src/reader/__init__.py`` to ``y``
 * (release.py) update changelog with release version and date
 * (release.py) make sure tests pass / docs build
 * (release.py) clean up dist/: ``rm -rf dist/``
 * (release.py) build tarball and wheel: ``python -m build``
 * (release.py) push to GitHub
 * (release.py prompts) wait for GitHub Actions / Codecov / Read the Docs builds to pass
@@ -131,14 +221,16 @@
   (e.g. when releasing `1.20`: `1.20` and `1.x`)
 * (release.py prompts) create release in GitHub
 * build docs from latest and enable ``y`` docs version (should happen automatically after the first time)
 * (release.py) bump versions from ``y`` to ``(y + 1).dev0``, add ``(y + 1)`` changelog section
 * (release.py prompts) trigger Read the Docs build for `<major>.x` (doesn't happen automatically)
 
 
+.. _design notes:
+
 Design notes
 ------------
 
 Folowing are various design notes that aren't captured somewhere else
 (either in the code, or in the issue where a feature was initially developed).
 
 
@@ -175,14 +267,16 @@
 and I think testing it with multiple databases would take quite some time.
 
 .. _the beginning: https://github.com/lemon24/reader/tree/afbc10335a45ec449205d5757d09cc4a3c6596da/reader
 .. _wanted: https://github.com/lemon24/reader/blame/99077c7e56db968cb892353075426bc5b0b141f1/README.md#L9
 .. _I had in mind: https://github.com/lemon24/reader/issues/168#issuecomment-642002049
 
 
+.. _multiple storage implementations:
+
 Multiple storage implementations
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Detailed requirements and API discussion: :issue:`168#issuecomment-642002049`.
 
 Minimal work needed to support alternate storages: :issue:`168#issuecomment-1383127564`.
 
@@ -268,45 +362,63 @@
 
 From the initial issue:
 
 * use cases: :issue:`149#issuecomment-700066794`
 * initial requirements: :issue:`149#issuecomment-700532183`
 
 
+Resource tags / metadata
+~~~~~~~~~~~~~~~~~~~~~~~~
+
 Feed tags
-~~~~~~~~~
+^^^^^^^^^
+
+.. _categories:
 
-Detailed requirements and API discussion: :issue:`184#issuecomment-689587006`.
+Detailed requirements and API discussion,
+and a case study of how to implement categories on top of tags:
+:issue:`184#issuecomment-689587006`.
 
 Merging tags and metadata, and the addition of a new,
 generic (global, feed, entry) tag API: :issue:`266#issuecomment-1013739526`.
 
+Entry tags
+^^^^^^^^^^
 
-Entry user data
-~~~~~~~~~~~~~~~
+.. _searchable tags:
 
-:issue:`228#issuecomment-810098748` discusses three different kinds,
+:issue:`228#issuecomment-810098748` discusses
+three different kinds of entry user data,
 how they would be implemented,
 and why I want more use-cases before implementing them (basically, YAGNI):
 
 * entry searchable text fields (for notes etc.)
 * entry tags (similar to feed tags, may be used as additional bool flags)
 * entry metadata (similar to feed metadata)
 
   * also discusses how to build an enclosure cache/preloader
     (doesn't need special *reader* features besides what's available in 1.16)
 
+.. _entry flag unification:
+
 :issue:`253` discusses using entry tags to implement the current entry flags
 (read, important); tl;dr: it's not worth adding entry tags just for this.
 
 After closing :issue:`228` with `wontfix` in late 2021,
 in early 2022 (following the :issue:`266` tag/metadata unification)
 I implemented entry and global tags in :issue:`272`;
 there's a list of known use cases in the issue description.
 
+Resource tags
+^^^^^^^^^^^^^
+
+Optimistic locking for tags: :issue:`308`.
+
+Filter tags by prefix: :issue:`309`.
+
 
 User-added entries
 ~~~~~~~~~~~~~~~~~~
 
 Discussion about API/typing, and things we didn't do: :issue:`239`.
 
 
@@ -335,14 +447,24 @@
   :issue:`179#issuecomment-796868555`, the :mod:`reader._hash_utils` module,
   `death and gravity article <https://death.andgravity.com/stable-hashing>`_
 * ideas for how to deal with spurious hash changes: :issue:`225`
 
 Decision to ignore feed.updated when updating feeds: :issue:`231`.
 
 
+.. _deleting entries:
+
+Deleting entries
+~~~~~~~~~~~~~~~~
+
+Requirements, open questions, and how it interacts with :mod:`~reader.plugins.entry_dedupe`: :issue:`96`.
+
+A summary of why it isn't easy to do: :issue:`301#issuecomment-1442423151`.
+
+
 Counts API
 ~~~~~~~~~~
 
 Detailed requirements and API discussion: :issue:`185#issuecomment-731743327`.
 
 
 Using None as a special argument value
@@ -350,14 +472,16 @@
 
 This comment: :issue:`177#issuecomment-674786498`.
 
 
 Batch methods
 ~~~~~~~~~~~~~
 
+.. _batch get methods:
+
 Some initial thoughts on batch get methods (including API/typing)
 in :issue:`191` (closed with `wontfix`, for now).
 
 Why I want to postpone batch update/set methods:
 :issue:`187#issuecomment-700740251`.
 
 tl:dr: Performance is likely a non-issue with SQLite,
```

### Comparing `reader-3.5/docs/guide.rst` & `reader-3.6/docs/guide.rst`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,19 @@
     Before starting, make sure that *reader* is :doc:`installed <install>`
     and up-to-date.
 
 
 The Reader object
 -----------------
 
-The :class:`Reader` object persists feed and entry state
-and provides operations on them.
+Most *reader* functionality is available through a :class:`Reader` instance,
+which persists feed and entry state
+and provides operations on them;
+in :abbr:`MVC (model–view–controller)` parlance,
+you would probably call it a fat model.
 
 
 To create a new Reader,
 call :func:`make_reader` with the path to a database file::
 
     >>> from reader import make_reader
     >>> reader = make_reader("db.sqlite")
@@ -84,15 +87,15 @@
 (but note that database connections will eventually be closed anyway
 when garbage-collected).
 
 
 Temporary databases
 ~~~~~~~~~~~~~~~~~~~
 
-In order to maximize the usefulness temporary databases,
+To maximize the usefulness of temporary databases,
 the database connection is closed (and the data discarded)
 only when calling :meth:`~Reader.close`,
 not when using the reader as a context manager.
 The reader cannot be reused after calling :meth:`~Reader.close`.
 
 ::
 
@@ -523,14 +526,15 @@
     The old, feed-only tags/metadata methods were deprecated,
     and **will be removed in version 3.0**.
 
 .. versionchanged:: 2.10
     Support entry and global tags.
 
 
+
 Counting things
 ---------------
 
 You can get aggregated feed and entry counts by using one of the
 :meth:`~Reader.get_feed_counts`,
 :meth:`~Reader.get_entry_counts`, or
 :meth:`~Reader.search_entry_counts` methods::
@@ -581,14 +585,34 @@
     ...
     1.0 entries/month (past month)
     2.0 entries/month (past 3 months)
     1.3 entries/month (past year)
 
 
 
+Deleting entries
+----------------
+
+As of version |version|, entries are **not** deleted automatically,
+and there is no high-level way of deleting entries;
+see :issue:`96` for details and updates.
+
+Deleting entries properly is non-trivial for two reasons:
+
+* Deleted entries should stay deleted;
+  right now, if you delete an entry that still appears in the feed,
+  it will be added again on the next update.
+* The :mod:`~reader.plugins.entry_dedupe` plugin needs the old entry in order to work.
+
+If you do not care about these issues,
+you can delete entries using the low-level
+:meth:`~reader._storage.Storage.delete_entries` storage method.
+
+
+
 .. _pagination:
 
 Pagination
 ----------
 
 :meth:`~Reader.get_feeds`, :meth:`~Reader.get_entries`,
 and :meth:`~Reader.search_entries`
```

### Comparing `reader-3.5/docs/images/redesign-01.png` & `reader-3.6/docs/images/redesign-01.png`

 * *Files identical despite different names*

### Comparing `reader-3.5/docs/index.rst` & `reader-3.6/docs/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 .. _GitHub: https://github.com/lemon24/reader
 .. _PyPI: https://pypi.org/project/reader/
 
 
 .. toctree::
     :maxdepth: 2
 
-    compat
+    contributing
     dev
     changelog
 
 
 Indices and tables
 ==================
```

### Comparing `reader-3.5/docs/install.rst` & `reader-3.6/docs/install.rst`

 * *Files identical despite different names*

### Comparing `reader-3.5/docs/internal.rst` & `reader-3.6/docs/internal.rst`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,17 @@
     the internal API is **not** part of the public API;
     it is not stable yet and might change without any notice.
 
 
 Parser
 ------
 
+.. autoattribute:: reader.Reader._parser
+
+
 .. module:: reader._parser
 
 .. autofunction:: default_parser
 
 .. autoclass:: Parser
     :members:
     :special-members: __call__
@@ -105,14 +108,26 @@
 .. autoclass:: FeedForUpdate
     :members:
 
 .. autoclass:: EntryForUpdate
     :members:
 
 
+Storage
+-------
+
+.. autoattribute:: reader.Reader._storage
+
+
+.. module:: reader._storage
+
+.. autoclass:: Storage()
+    :members:
+
+
 Recipes
 -------
 
 .. include:: ../examples/parser_only.py
     :start-after: """
     :end-before: """  # docstring-end
```

### Comparing `reader-3.5/docs/make.bat` & `reader-3.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reader-3.5/docs/plugins.rst` & `reader-3.6/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `reader-3.5/docs/screenshots/dillo.png` & `reader-3.6/docs/screenshots/dillo.png`

 * *Files identical despite different names*

### Comparing `reader-3.5/docs/screenshots/entries-feed.png` & `reader-3.6/docs/screenshots/entries-feed.png`

 * *Files identical despite different names*

### Comparing `reader-3.5/docs/screenshots/entries.png` & `reader-3.6/docs/screenshots/entries.png`

 * *Files identical despite different names*

### Comparing `reader-3.5/docs/screenshots/entry-one.png` & `reader-3.6/docs/screenshots/entry-one.png`

 * *Files identical despite different names*

### Comparing `reader-3.5/docs/screenshots/entry-two.png` & `reader-3.6/docs/screenshots/entry-two.png`

 * *Files identical despite different names*

### Comparing `reader-3.5/docs/screenshots/feeds.png` & `reader-3.6/docs/screenshots/feeds.png`

 * *Files identical despite different names*

### Comparing `reader-3.5/docs/screenshots/lynx.png` & `reader-3.6/docs/screenshots/lynx.png`

 * *Files identical despite different names*

### Comparing `reader-3.5/docs/screenshots/search.png` & `reader-3.6/docs/screenshots/search.png`

 * *Files identical despite different names*

### Comparing `reader-3.5/docs/screenshots/twitter-one.png` & `reader-3.6/docs/screenshots/twitter-one.png`

 * *Files identical despite different names*

### Comparing `reader-3.5/docs/screenshots/twitter-two.png` & `reader-3.6/docs/screenshots/twitter-two.png`

 * *Files identical despite different names*

### Comparing `reader-3.5/docs/tutorial.rst` & `reader-3.6/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `reader-3.5/docs/why.rst` & `reader-3.6/docs/why.rst`

 * *Files 15% similar despite different names*

```diff
@@ -29,14 +29,32 @@
 
 
 .. _feedparser: https://feedparser.readthedocs.io/en/latest/
 .. _requests: https://requests.readthedocs.io
 .. _JSON Feed: https://jsonfeed.org/
 
 
+
+.. _philosophy:
+
+The *reader* philosophy
+-----------------------
+
+* *reader* is a library
+* *reader* is for the long term
+* *reader* is extensible
+* *reader* is stable (within reason)
+* *reader* is simple to use; API matters
+* *reader* features work well together
+* *reader* is tested
+* *reader* is documented
+* *reader* has minimal dependencies
+
+
+
 Why make your own feed reader?
 ------------------------------
 
 So you can:
 
 * have full control over your data
 * control what features it has or doesn't have
```

### Comparing `reader-3.5/examples/config.yaml` & `reader-3.6/examples/config.yaml`

 * *Files identical despite different names*

### Comparing `reader-3.5/examples/parser_only.py` & `reader-3.6/examples/parser_only.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/examples/podcast.py` & `reader-3.6/examples/podcast.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/examples/terminal.py` & `reader-3.6/examples/terminal.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/run.sh` & `reader-3.6/run.sh`

 * *Files 10% similar despite different names*

```diff
@@ -28,31 +28,33 @@
 
 
 
 # Commands follow.
 
 
 function install-dev {
-    pip install -e '.[dev]'
-    pre-commit install
+    pip install -e '.[dev]' --upgrade --upgrade-strategy=eager
+    pre-commit install --install-hooks
 }
 
 
 function test {
     pytest --runslow "$@"
 }
 
 
 function coverage-all {
     clean-pyc
+    # TODO: do we need to --cov-context=test all the time?
     coverage-run --cov-context=test "$@"
     coverage-report --show-contexts
 }
 
 function coverage-run {
+    # TODO: is pytest-cov needed?
     pytest --runslow --cov "$@"
 }
 
 function coverage-report {
     coverage html "$@"
     coverage report \
         --include '*/reader/*' \
```

### Comparing `reader-3.5/scripts/.coverage` & `reader-3.6/scripts/.coverage`

 * *Files identical despite different names*

### Comparing `reader-3.5/scripts/backup.sh` & `reader-3.6/scripts/backup.sh`

 * *Files identical despite different names*

### Comparing `reader-3.5/scripts/bench.py` & `reader-3.6/scripts/bench.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/scripts/debug_storage_stats.py` & `reader-3.6/scripts/debug_storage_stats.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/scripts/jscontrols.html` & `reader-3.6/scripts/jscontrols.html`

 * *Files identical despite different names*

### Comparing `reader-3.5/scripts/jscontrols.py` & `reader-3.6/scripts/jscontrols.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/scripts/lines.sh` & `reader-3.6/scripts/lines.sh`

 * *Files identical despite different names*

### Comparing `reader-3.5/scripts/release.py` & `reader-3.6/scripts/release.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/setup.cfg` & `reader-3.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 	lxml
 	html5lib
 	werkzeug
 	mypy; implementation_name != "pypy"
 	types-requests
 docs = 
 	sphinx
-	sphinx-rtd-theme~=1.0
+	sphinx-rtd-theme
 	click>=7
 	sphinx-click
 	sphinx-issues
 	sphinx-hoverxref
 	sphinxcontrib-log-cabinet
 	setuptools
 dev =
```

### Comparing `reader-3.5/src/reader/__init__.py` & `reader-3.6/src/reader/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     for e in reader.get_entries(read=False):
         print(e.title)
 
 
 """
 
-__version__ = '3.5'
+__version__ = '3.6'
 
 from .core import (
     Reader as Reader,
     make_reader as make_reader,
 )
 
 from .types import (
```

### Comparing `reader-3.5/src/reader/_app/__init__.py` & `reader-3.6/src/reader/_app/__init__.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_app/api_thing.py` & `reader-3.6/src/reader/_app/api_thing.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_app/cli.py` & `reader-3.6/src/reader/_app/cli.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_app/static/controls.js` & `reader-3.6/src/reader/_app/static/controls.js`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_app/static/style.css` & `reader-3.6/src/reader/_app/static/style.css`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_app/templates/add_entry.html` & `reader-3.6/src/reader/_app/templates/add_entry.html`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_app/templates/entries.html` & `reader-3.6/src/reader/_app/templates/entries.html`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_app/templates/entry.html` & `reader-3.6/src/reader/_app/templates/entry.html`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_app/templates/feeds.html` & `reader-3.6/src/reader/_app/templates/feeds.html`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_app/templates/layout.html` & `reader-3.6/src/reader/_app/templates/layout.html`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_app/templates/macros.html` & `reader-3.6/src/reader/_app/templates/macros.html`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_app/templates/metadata.html` & `reader-3.6/src/reader/_app/templates/metadata.html`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_app/templates/tags.html` & `reader-3.6/src/reader/_app/templates/tags.html`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_app/wsgi.py` & `reader-3.6/src/reader/_app/wsgi.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_cli.py` & `reader-3.6/src/reader/_cli.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_config.py` & `reader-3.6/src/reader/_config.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_feedparser.py` & `reader-3.6/src/reader/_feedparser.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_feedparser_lazy.py` & `reader-3.6/src/reader/_feedparser_lazy.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_hash_utils.py` & `reader-3.6/src/reader/_hash_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_html_utils.py` & `reader-3.6/src/reader/_html_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_jsonfeed.py` & `reader-3.6/src/reader/_jsonfeed.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_parser.py` & `reader-3.6/src/reader/_parser.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_plugins/__init__.py` & `reader-3.6/src/reader/_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_plugins/cli_status.py` & `reader-3.6/src/reader/_plugins/cli_status.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_plugins/enclosure_tags.py` & `reader-3.6/src/reader/_plugins/enclosure_tags.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_plugins/preview_feed_list.py` & `reader-3.6/src/reader/_plugins/preview_feed_list.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_plugins/sqlite_releases.py` & `reader-3.6/src/reader/_plugins/sqlite_releases.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_plugins/templates/preview_feed_list.html` & `reader-3.6/src/reader/_plugins/templates/preview_feed_list.html`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_plugins/tumblr_gdpr.py` & `reader-3.6/src/reader/_plugins/tumblr_gdpr.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_plugins/twitter.py` & `reader-3.6/src/reader/_plugins/twitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 """
 twitter
 ~~~~~~~
 
+.. attention::
+
+  This plugin is deprecated and will be removed in version 3.7.
+
 .. module:: reader
   :noindex:
 
 Create a feed out of a Twitter account.
 
 Feed URLs must be of the of the form ``https://twitter.com/user`` (no query string).
 
@@ -94,14 +98,15 @@
 """
 from __future__ import annotations
 
 import json
 import logging
 import posixpath
 import re
+import warnings
 from contextlib import contextmanager
 from dataclasses import dataclass
 from dataclasses import field
 from datetime import timedelta
 from datetime import timezone
 from typing import NamedTuple
 from urllib.parse import parse_qs
@@ -116,14 +121,19 @@
 from reader import ParseError
 from reader import Reader
 from reader._parser import RetrieveResult
 from reader._types import EntryData
 from reader._types import FeedData
 
 
+warnings.warn(
+    "The twitter plugin is deprecated and will be removed in reader version 3.7.",
+    DeprecationWarning,
+)
+
 log = logging.getLogger('reader._plugins.twitter')
 
 
 MIME_TYPE = 'application/x.twitter'
 MIME_TYPE_JSON = MIME_TYPE + '+json'
 MIME_TYPE_HTML = 'text/html'
```

### Comparing `reader-3.5/src/reader/_requests_utils.py` & `reader-3.6/src/reader/_requests_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_requests_utils_lazy.py` & `reader-3.6/src/reader/_requests_utils_lazy.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_retrievers.py` & `reader-3.6/src/reader/_retrievers.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_search.py` & `reader-3.6/src/reader/_search.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_sql_utils.py` & `reader-3.6/src/reader/_sql_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_sqlite_utils.py` & `reader-3.6/src/reader/_sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_storage.py` & `reader-3.6/src/reader/_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,14 +381,15 @@
 MISSING_MIGRATION_DETAIL = (
     "; you may have skipped some required migrations, see "
     "https://reader.readthedocs.io/en/latest/changelog.html#removed-migrations-3-0"
 )
 
 
 class Storage:
+    """Data access object used for all storage except search."""
 
     # chunk_size and entry_counts_average_periods
     # are not part of the Storage interface,
     # but are part of the private API of this implementation.
     chunk_size = 2**8
     # 1, 3, 12 months rounded down to days,
     # assuming an average of 30.436875 days/month
@@ -1011,14 +1012,28 @@
         # TODO: unify with the or_update variants
         self._add_or_update_entries([intent], exclusive=True)
 
     @wrap_exceptions(StorageError)
     def delete_entries(
         self, entries: Iterable[tuple[str, str]], *, added_by: str | None = None
     ) -> None:
+        r"""Delete a list of entries.
+
+        Args:
+            entries (list(tuple(str, str))):
+                A list of :attr:`~reader.Entry.resource_id`\s.
+            added_by (str or None):
+                If given, only delete the entries if their
+                :attr:`~reader.Entry.added_by` is equal to this.
+
+        Raises:
+            EntryNotFoundError: An entry does not exist.
+            EntryError: An entry has a different ``added_by`` from the given one.
+
+        """
         # This must be atomic (unlike add_or_update_entries()); hence, no paging.
         # We'll deal with locking issues only if they start appearing
         # (hopefully, there are both fewer entries to be deleted and
         # this takes less time per entry).
 
         delete_query = "DELETE FROM entries WHERE feed = :feed AND id = :id"
         added_by_query = "SELECT added_by FROM entries WHERE feed = :feed AND id = :id"
```

### Comparing `reader-3.5/src/reader/_types.py` & `reader-3.6/src/reader/_types.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_update.py` & `reader-3.6/src/reader/_update.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_url_utils.py` & `reader-3.6/src/reader/_url_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_utils.py` & `reader-3.6/src/reader/_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/__init__.py` & `reader-3.6/src/reader/_vendor/feedparser/__init__.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/api.py` & `reader-3.6/src/reader/_vendor/feedparser/api.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/datetimes/__init__.py` & `reader-3.6/src/reader/_vendor/feedparser/datetimes/__init__.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/datetimes/asctime.py` & `reader-3.6/src/reader/_vendor/feedparser/datetimes/asctime.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/datetimes/greek.py` & `reader-3.6/src/reader/_vendor/feedparser/datetimes/greek.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/datetimes/hungarian.py` & `reader-3.6/src/reader/_vendor/feedparser/datetimes/hungarian.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/datetimes/iso8601.py` & `reader-3.6/src/reader/_vendor/feedparser/datetimes/iso8601.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/datetimes/korean.py` & `reader-3.6/src/reader/_vendor/feedparser/datetimes/korean.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/datetimes/perforce.py` & `reader-3.6/src/reader/_vendor/feedparser/datetimes/perforce.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/datetimes/rfc822.py` & `reader-3.6/src/reader/_vendor/feedparser/datetimes/rfc822.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/datetimes/w3dtf.py` & `reader-3.6/src/reader/_vendor/feedparser/datetimes/w3dtf.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/encodings.py` & `reader-3.6/src/reader/_vendor/feedparser/encodings.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/exceptions.py` & `reader-3.6/src/reader/_vendor/feedparser/exceptions.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/html.py` & `reader-3.6/src/reader/_vendor/feedparser/html.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/http.py` & `reader-3.6/src/reader/_vendor/feedparser/http.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/mixin.py` & `reader-3.6/src/reader/_vendor/feedparser/mixin.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/namespaces/_base.py` & `reader-3.6/src/reader/_vendor/feedparser/namespaces/_base.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/namespaces/admin.py` & `reader-3.6/src/reader/_vendor/feedparser/namespaces/admin.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/namespaces/cc.py` & `reader-3.6/src/reader/_vendor/feedparser/namespaces/cc.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/namespaces/dc.py` & `reader-3.6/src/reader/_vendor/feedparser/namespaces/dc.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/namespaces/georss.py` & `reader-3.6/src/reader/_vendor/feedparser/namespaces/georss.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/namespaces/itunes.py` & `reader-3.6/src/reader/_vendor/feedparser/namespaces/itunes.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/namespaces/mediarss.py` & `reader-3.6/src/reader/_vendor/feedparser/namespaces/mediarss.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/namespaces/psc.py` & `reader-3.6/src/reader/_vendor/feedparser/namespaces/psc.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/parsers/json.py` & `reader-3.6/src/reader/_vendor/feedparser/parsers/json.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/parsers/loose.py` & `reader-3.6/src/reader/_vendor/feedparser/parsers/loose.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/parsers/strict.py` & `reader-3.6/src/reader/_vendor/feedparser/parsers/strict.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/sanitizer.py` & `reader-3.6/src/reader/_vendor/feedparser/sanitizer.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/sgml.py` & `reader-3.6/src/reader/_vendor/feedparser/sgml.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/urls.py` & `reader-3.6/src/reader/_vendor/feedparser/urls.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/_vendor/feedparser/util.py` & `reader-3.6/src/reader/_vendor/feedparser/util.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/core.py` & `reader-3.6/src/reader/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -352,16 +352,19 @@
         _storage: Storage,
         _search: Search,
         _parser: Parser,
         _reserved_name_scheme: NameScheme,
         _enable_search: bool = False,
         _called_directly: bool = True,
     ):
+        #: The :class:`~reader._storage.Storage` instance used by this reader.
         self._storage = _storage
+        #: The :class:`~reader._search.Search` instance used by this reader.
         self._search = _search
+        #: The :class:`~reader._parser.Parser` instance used by this reader.
         self._parser = _parser
 
         self._reserved_name_scheme = _reserved_name_scheme
 
         self._enable_search = _enable_search
 
         #: List of functions called for each updated entry
```

### Comparing `reader-3.5/src/reader/exceptions.py` & `reader-3.6/src/reader/exceptions.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/plugins/__init__.py` & `reader-3.6/src/reader/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/plugins/enclosure_dedupe.py` & `reader-3.6/src/reader/plugins/enclosure_dedupe.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/plugins/entry_dedupe.py` & `reader-3.6/src/reader/plugins/entry_dedupe.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/plugins/mark_as_read.py` & `reader-3.6/src/reader/plugins/mark_as_read.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/plugins/readtime.py` & `reader-3.6/src/reader/plugins/readtime.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/plugins/ua_fallback.py` & `reader-3.6/src/reader/plugins/ua_fallback.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader/types.py` & `reader-3.6/src/reader/types.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/src/reader.egg-info/PKG-INFO` & `reader-3.6/src/reader.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reader
-Version: 3.5
+Version: 3.6
 Summary: A Python feed reader library.
 Home-page: https://github.com/lemon24/reader
 Author: lemon24
 License: BSD-3-Clause
 Project-URL: Changes, https://reader.readthedocs.io/en/latest/changelog.html
 Project-URL: Documentation, https://reader.readthedocs.io/
 Project-URL: Issue tracker, https://github.com/lemon24/reader/issues
@@ -58,16 +58,16 @@
 |build-status-github| |code-coverage| |documentation-status| |pypi-status| |type-checking| |code-style|
 
 
 .. |build-status-github| image:: https://github.com/lemon24/reader/workflows/build/badge.svg
   :target: https://github.com/lemon24/reader/actions?query=workflow%3Abuild
   :alt: build status (GitHub Actions)
 
-.. |code-coverage| image:: https://codecov.io/github/lemon24/reader/coverage.svg?branch=master
-  :target: https://codecov.io/github/lemon24/reader?branch=master
+.. |code-coverage| image:: https://codecov.io/gh/lemon24/reader/branch/master/graph/badge.svg?token=lcLZaSFysf
+  :target: https://codecov.io/gh/lemon24/reader
   :alt: code coverage
 
 .. |documentation-status| image:: https://readthedocs.org/projects/reader/badge/?version=latest&style=flat
   :target: https://reader.readthedocs.io/en/latest/?badge=latest
   :alt: documentation status
 
 .. |pypi-status| image:: https://img.shields.io/pypi/v/reader.svg
```

### Comparing `reader-3.5/src/reader.egg-info/SOURCES.txt` & `reader-3.6/src/reader.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 setup.py
 tox.ini
 docs/Makefile
 docs/api.rst
 docs/app.rst
 docs/changelog.rst
 docs/cli.rst
-docs/compat.rst
 docs/conf.py
 docs/config.rst
+docs/contributing.rst
 docs/dev-app.rst
 docs/dev.rst
 docs/guide.rst
 docs/index.rst
 docs/install.rst
 docs/internal.rst
 docs/make.bat
```

### Comparing `reader-3.5/src/reader.egg-info/requires.txt` & `reader-3.6/src/reader.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 tox
 pre-commit
 build
 twine
 
 [docs]
 sphinx
-sphinx-rtd-theme~=1.0
+sphinx-rtd-theme
 click>=7
 sphinx-click
 sphinx-issues
 sphinx-hoverxref
 sphinxcontrib-log-cabinet
 setuptools
```

### Comparing `reader-3.5/tests/conftest.py` & `reader-3.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/data/full.atom` & `reader-3.6/tests/data/full.atom`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/data/full.atom.py` & `reader-3.6/tests/data/full.atom.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/data/full.json` & `reader-3.6/tests/data/full.json`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/data/full.json.py` & `reader-3.6/tests/data/full.json.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/data/full.rss` & `reader-3.6/tests/data/full.rss`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/data/full.rss.py` & `reader-3.6/tests/data/full.rss.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/data/invalid.json` & `reader-3.6/tests/data/invalid.json`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/data/invalid.json.py` & `reader-3.6/tests/data/invalid.json.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/data/relative.atom` & `reader-3.6/tests/data/relative.atom`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/data/relative.atom.py` & `reader-3.6/tests/data/relative.atom.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/data/relative.rss` & `reader-3.6/tests/data/relative.rss`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/data/relative.rss.py` & `reader-3.6/tests/data/relative.rss.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/data/sqlite_releases.html` & `reader-3.6/tests/data/sqlite_releases.html`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/fakeparser.py` & `reader-3.6/tests/fakeparser.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/reader_methods.py` & `reader-3.6/tests/reader_methods.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test__types.py` & `reader-3.6/tests/test__types.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_app.py` & `reader-3.6/tests/test_app.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,19 +22,34 @@
 
 def make_app(config):
     return create_app(make_reader_config(config))
 
 
 def make_browser(app):
     session = requests.Session()
-    session.mount('http://app/', wsgiadapter.WSGIAdapter(app))
+    session.mount('http://app/', WSGIAdapter(app))
     browser = mechanicalsoup.StatefulBrowser(session)
     return browser
 
 
+class WSGIAdapter(wsgiadapter.WSGIAdapter):
+    """Workaround for https://github.com/seanbrant/requests-wsgi-adapter/issues/23."""
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        original_app = self.app
+
+        def new_app(environ, start_response):
+            environ['CONTENT_LENGTH'] = str(environ['CONTENT_LENGTH'])
+            return original_app(environ, start_response)
+
+        self.app = new_app
+
+
 @pytest.fixture
 def app(db_path):
     return make_app({'reader': {'url': db_path}})
 
 
 @pytest.fixture
 def browser(app):
@@ -56,14 +71,15 @@
     reader.update_feeds()
 
     browser.open('http://app/')
     assert len(browser.get_current_page().select('.entry')) == 1
 
     form = browser.select_form('.entry form.action-mark-as-read')
     response = browser.submit_selected(form.form.find('button', text='mark as read'))
+
     assert response.status_code == 200
     assert len(browser.get_current_page().select('.entry')) == 0
 
     response = browser.follow_link(browser.find_link(text='read'))
     assert response.status_code == 200
     assert len(browser.get_current_page().select('.entry')) == 1
```

### Comparing `reader-3.5/tests/test_app_wsgi.py` & `reader-3.6/tests/test_app_wsgi.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_bench.py` & `reader-3.6/tests/test_bench.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_cli.py` & `reader-3.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_config.py` & `reader-3.6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_exceptions.py` & `reader-3.6/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_hash_utils.py` & `reader-3.6/tests/test_hash_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_html_utils.py` & `reader-3.6/tests/test_html_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_http_utils.py` & `reader-3.6/tests/test_http_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         ';q=1',
         ';q=x',
         "type;q=10",
         "type;q=-10",
     ],
 )
 def test_parse_accept_header(value):
-    assert parse_accept_header(value) == werkzeug.http.parse_accept_header(value)
+    assert parse_accept_header(value) == list(werkzeug.http.parse_accept_header(value))
 
 
 @pytest.mark.parametrize(
     'values',
     [
         [('one', 1), ('one', 1), ('two', 0), ('three', 0.1), ('four', 0.1234)],
     ],
@@ -43,10 +43,10 @@
     [
         'one/two',
         'one/two;param=value',
         ' one/two ; param=value',
     ],
 )
 def test_parse_options_header(value):
-    content_type, options = parse_options_header(value)
-    assert content_type == werkzeug.http.parse_options_header(value)[0]
-    assert options == {}
+    actual = parse_options_header(value)
+    expected = werkzeug.http.parse_options_header(value)
+    assert actual == expected
```

### Comparing `reader-3.5/tests/test_lazy_imports.py` & `reader-3.6/tests/test_lazy_imports.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+See https://github.com/lemon24/reader/issues/297 for details.
+
+"""
 import os
 import pkgutil
 import subprocess
 import sys
 import textwrap
 
 import pytest
@@ -71,15 +75,15 @@
     multiprocessing
     """.split()
 )
 
 
 # all in a single script to save time
 
-NO_IMPORTS = """\
+S_NO_IMPORTS = """\
 reader.add_feed('file:feed.rss')  # but not http://
 list(reader.get_entries())
 list(reader.search_entries('entry'))
 reader._parser.session_factory.response_hooks.append('unused')
 """, set()  # fmt: skip
```

### Comparing `reader-3.5/tests/test_parser.py` & `reader-3.6/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_plugins_cli_status.py` & `reader-3.6/tests/test_plugins_cli_status.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_plugins_enclosure_dedupe.py` & `reader-3.6/tests/test_plugins_enclosure_dedupe.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_plugins_entry_dedupe.py` & `reader-3.6/tests/test_plugins_entry_dedupe.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_plugins_mark_as_read.py` & `reader-3.6/tests/test_plugins_mark_as_read.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_plugins_preview_feed_list.py` & `reader-3.6/tests/test_plugins_preview_feed_list.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_plugins_readtime.py` & `reader-3.6/tests/test_plugins_readtime.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_plugins_sqlite_releases.py` & `reader-3.6/tests/test_plugins_sqlite_releases.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_plugins_twitter.py` & `reader-3.6/tests/test_plugins_twitter.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_plugins_ua_fallback.py` & `reader-3.6/tests/test_plugins_ua_fallback.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_reader.py` & `reader-3.6/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_reader_context.py` & `reader-3.6/tests/test_reader_context.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_reader_hooks.py` & `reader-3.6/tests/test_reader_hooks.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_reader_integration.py` & `reader-3.6/tests/test_reader_integration.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_reader_plugins.py` & `reader-3.6/tests/test_reader_plugins.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_reader_private.py` & `reader-3.6/tests/test_reader_private.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_reader_search.py` & `reader-3.6/tests/test_reader_search.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_reader_sort.py` & `reader-3.6/tests/test_reader_sort.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_search.py` & `reader-3.6/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_sql_utils.py` & `reader-3.6/tests/test_sql_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_sqlite_utils.py` & `reader-3.6/tests/test_sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_storage.py` & `reader-3.6/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_tags.py` & `reader-3.6/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_test_utils.py` & `reader-3.6/tests/test_test_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_types.py` & `reader-3.6/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/test_utils.py` & `reader-3.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tests/utils.py` & `reader-3.6/tests/utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.5/tox.ini` & `reader-3.6/tox.ini`

 * *Files identical despite different names*

