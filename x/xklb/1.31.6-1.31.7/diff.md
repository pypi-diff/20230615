# Comparing `tmp/xklb-1.31.6.tar.gz` & `tmp/xklb-1.31.7.tar.gz`

## Comparing `xklb-1.31.6.tar` & `xklb-1.31.7.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.31.6/.gitattributes
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 xklb-1.31.6/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.31.6/Windows.md
--rw-r--r--   0        0        0   490396 2020-02-02 00:00:00.000000 xklb-1.31.6/pdm.lock
--rw-r--r--   0        0        0    19420 2020-02-02 00:00:00.000000 xklb-1.31.6/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.31.6/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.31.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.31.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-1.31.6/.github/workflows/green.yaml
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-1.31.6/.github/workflows/push.yaml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/__init__.py
--rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/av.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/books.py
--rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/consts.py
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/db.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/dl_config.py
--rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/dl_extract.py
--rw-r--r--   0        0        0    14103 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/fs_extract.py
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/gdl_backend.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/gdl_extract.py
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/gui.py
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/hn_extract.py
--rw-r--r--   0        0        0    11781 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/lb.py
--rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/media.py
--rw-r--r--   0        0        0    25252 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/play_actions.py
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/playback.py
--rw-r--r--   0        0        0    35233 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/player.py
--rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/playlists.py
--rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/praw_extract.py
--rw-r--r--   0        0        0     7949 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/search.py
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/subtitle.py
--rw-r--r--   0        0        0     6029 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/tabs_actions.py
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/tabs_extract.py
--rw-r--r--   0        0        0    15396 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/tube_backend.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/tube_extract.py
--rw-r--r--   0        0        0    76102 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/usage.py
--rw-r--r--   0        0        0    37338 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/block.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/christen.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/dedupe_db.py
--rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/history.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     6044 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/relmv.py
--rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.31.6/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.31.6/LICENSE
--rw-r--r--   0        0        0    98892 2020-02-02 00:00:00.000000 xklb-1.31.6/README.md
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 xklb-1.31.6/pyproject.toml
--rw-r--r--   0        0        0   102519 2020-02-02 00:00:00.000000 xklb-1.31.6/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.31.7/.gitattributes
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 xklb-1.31.7/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.31.7/Windows.md
+-rw-r--r--   0        0        0   490396 2020-02-02 00:00:00.000000 xklb-1.31.7/pdm.lock
+-rw-r--r--   0        0        0    19420 2020-02-02 00:00:00.000000 xklb-1.31.7/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.31.7/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.31.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.31.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-1.31.7/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-1.31.7/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/__init__.py
+-rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/av.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/books.py
+-rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/consts.py
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/db.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/dl_config.py
+-rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/dl_extract.py
+-rw-r--r--   0        0        0    14103 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/fs_extract.py
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/gdl_backend.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/gdl_extract.py
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/gui.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/hn_extract.py
+-rw-r--r--   0        0        0    11781 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/lb.py
+-rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/media.py
+-rw-r--r--   0        0        0    25448 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/play_actions.py
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/playback.py
+-rw-r--r--   0        0        0    35233 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/player.py
+-rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/playlists.py
+-rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/praw_extract.py
+-rw-r--r--   0        0        0     7949 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/search.py
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/subtitle.py
+-rw-r--r--   0        0        0     6029 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    15396 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/tube_backend.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/tube_extract.py
+-rw-r--r--   0        0        0    76102 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/usage.py
+-rw-r--r--   0        0        0    37347 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/block.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/dedupe_db.py
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/history.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     6044 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.31.7/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.31.7/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.31.7/LICENSE
+-rw-r--r--   0        0        0    98892 2020-02-02 00:00:00.000000 xklb-1.31.7/README.md
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 xklb-1.31.7/pyproject.toml
+-rw-r--r--   0        0        0   102519 2020-02-02 00:00:00.000000 xklb-1.31.7/PKG-INFO
```

### Comparing `xklb-1.31.6/TODO` & `xklb-1.31.7/TODO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 
 lb bigdirs ~/lb/video.db
 
 /mnt/d/75_MovieQueue/unsorted/NRMwalkthroughHD/ should be 200GB
 
+
+- move mpv specific playhead code to a script subcommand
+
+option to delete mpv watch_later file if media file does not exist
+
 - dlstatus print errors also:
 
 sqlite lb/fs/blogspot.db 'select error, count(*) from media group by 1 order by 2'
 [{"error": "NoExtractorError", "count(*)": 21},
  {"error": null, "count(*)": 46},
  {"error": "HTTPError", "count(*)": 112},
  {"error": "HTTPNotFoundError", "count(*)": 118}]
@@ -23,18 +28,14 @@
 
 default 16000 files, flat subdirectory
 
 - POIs CLI -- save your trip plans and see places to go with automated day trip itineraries, geopandas buffer
 
 - wt/lt/search join and use fts on both tables, threading ?
 
-- move mpv specific playhead code to a script subcommand
-
-option to delete mpv watch_later file if media file does not exist
-
 - improve playlists subcommand
 
 - upscale command -- download higher quality videos; use webpath, PURL, comment to get URL
 
 - make generic printer. support --json or --csv for most subcommands
 
 - improve dlstatus subcommand tests
```

### Comparing `xklb-1.31.6/Windows.md` & `xklb-1.31.7/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/pdm.lock` & `xklb-1.31.7/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/readme.py` & `xklb-1.31.7/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.31.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.31.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/.github/workflows/push.yaml` & `xklb-1.31.7/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/av.py` & `xklb-1.31.7/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/books.py` & `xklb-1.31.7/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/consts.py` & `xklb-1.31.7/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/db.py` & `xklb-1.31.7/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/dl_config.py` & `xklb-1.31.7/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/dl_extract.py` & `xklb-1.31.7/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/fs_extract.py` & `xklb-1.31.7/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/gdl_backend.py` & `xklb-1.31.7/xklb/gdl_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/gdl_extract.py` & `xklb-1.31.7/xklb/gdl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/gui.py` & `xklb-1.31.7/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/hn_extract.py` & `xklb-1.31.7/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/lb.py` & `xklb-1.31.7/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/media.py` & `xklb-1.31.7/xklb/media.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/play_actions.py` & `xklb-1.31.7/xklb/play_actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse, shlex, shutil, sys, time
+import os
 from collections import deque
 from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
 from random import random
 from typing import Dict, Tuple
 
 from xklb import consts, db, player, subtitle, tube_backend, usage, utils
@@ -552,14 +553,15 @@
     if args.print and not any(
         [
             args.partial,
             args.lower,
             args.upper,
             args.safe,
             args.play_in_order >= consts.SIMILAR,
+            args.big_dirs,
             args.related >= consts.RELATED,
             args.cluster,
         ],
     ):
         player.printer(args, query, bindings)
         return
 
@@ -598,15 +600,20 @@
     if args.big_dirs:
         media_keyed = {d["path"]: d for d in media}
         dirs = process_bigdirs(args, media)
         dirs = list(reversed([d["path"] for d in dirs]))
         if "limit" in args.defaults:
             media = player.get_dir_media(args, dirs)
         else:
-            media = [media_keyed[key] for dir in dirs for key in media_keyed if key.startswith(dir)]
+            media = []
+            for dir in dirs:
+                for key in media_keyed:
+                    if os.sep not in key.replace(dir, '') and key.startswith(dir):
+                        media.append(media_keyed[key])
+                        break
         log.debug("big_dirs: %s", t.elapsed())
 
     if args.related >= consts.RELATED:
         media = player.get_related_media(args, media[0])
         log.debug("player.get_related_media: %s", t.elapsed())
 
     if args.cluster:
```

### Comparing `xklb-1.31.6/xklb/playback.py` & `xklb-1.31.7/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/player.py` & `xklb-1.31.7/xklb/player.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/playlists.py` & `xklb-1.31.7/xklb/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/praw_extract.py` & `xklb-1.31.7/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/search.py` & `xklb-1.31.7/xklb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/subtitle.py` & `xklb-1.31.7/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/tabs_actions.py` & `xklb-1.31.7/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/tabs_extract.py` & `xklb-1.31.7/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/tube_backend.py` & `xklb-1.31.7/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/tube_extract.py` & `xklb-1.31.7/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/usage.py` & `xklb-1.31.7/xklb/usage.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/utils.py` & `xklb-1.31.7/xklb/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1068,15 +1068,15 @@
 
     def elapsed(self):
         if not hasattr(self, "start_time"):
             raise RuntimeError("Timer has not been started.")
         end_time = default_timer()
         elapsed_time = end_time - self.start_time
         self.reset()
-        return elapsed_time
+        return f"{elapsed_time:.4f}"
 
 
 def cover_scan(media_duration, scan_percentage):
     num_scans = max(2, int(math.log(media_duration) * (scan_percentage / 10)))
     scan_duration_total = max(1, media_duration * (scan_percentage / 100))
     scan_duration = max(1, int(scan_duration_total / num_scans))
     scan_interval = media_duration / num_scans
```

### Comparing `xklb-1.31.6/xklb/scripts/bigdirs.py` & `xklb-1.31.7/xklb/scripts/bigdirs.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,16 +43,14 @@
 
     args.include += args.search
     if args.include == ["."]:
         args.include = [str(Path().cwd().resolve())]
 
     if args.size:
         args.size = utils.parse_human_to_sql(utils.human_to_bytes, "size", args.size)
-    if args.folder_size:
-        args.folder_size = utils.parse_human_to_lambda(utils.human_to_bytes, args.folder_size)
 
     log.info(utils.dict_filter_bool(args.__dict__))
     return args
 
 
 def group_files_by_folder(args, media) -> List[Dict]:
     d = {}
@@ -156,14 +154,15 @@
 
 
 def process_bigdirs(args, media) -> List[Dict]:
     folders = group_files_by_folder(args, media)
     if args.depth:
         folders = folder_depth(args, folders)
     if args.folder_size:
+        args.folder_size = utils.parse_human_to_lambda(utils.human_to_bytes, args.folder_size)
         folders = [d for d in folders if args.folder_size(d["size"])]
     return sorted(folders, key=sort_by(args))
 
 
 def bigdirs() -> None:
     args = parse_args()
     tbl = get_table(args)
```

### Comparing `xklb-1.31.6/xklb/scripts/block.py` & `xklb-1.31.7/xklb/scripts/block.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/scripts/christen.py` & `xklb-1.31.7/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/scripts/cluster_sort.py` & `xklb-1.31.7/xklb/scripts/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/scripts/copy_play_counts.py` & `xklb-1.31.7/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/scripts/dedupe.py` & `xklb-1.31.7/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/scripts/dedupe_db.py` & `xklb-1.31.7/xklb/scripts/dedupe_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/scripts/download_status.py` & `xklb-1.31.7/xklb/scripts/download_status.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/scripts/history.py` & `xklb-1.31.7/xklb/scripts/history.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/scripts/merge_dbs.py` & `xklb-1.31.7/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/scripts/merge_online_local.py` & `xklb-1.31.7/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/scripts/move_list.py` & `xklb-1.31.7/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/scripts/optimize_db.py` & `xklb-1.31.7/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/scripts/playlists.py` & `xklb-1.31.7/xklb/scripts/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/scripts/redownload.py` & `xklb-1.31.7/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/scripts/relmv.py` & `xklb-1.31.7/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/scripts/scatter.py` & `xklb-1.31.7/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/scripts/streaming_tab_loader.py` & `xklb-1.31.7/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/scripts/mining/data.py` & `xklb-1.31.7/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/scripts/mining/extract_links.py` & `xklb-1.31.7/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/scripts/mining/nouns.py` & `xklb-1.31.7/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/scripts/mining/pushshift.py` & `xklb-1.31.7/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.31.7/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/xklb/assets/kotobago.png` & `xklb-1.31.7/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/.gitignore` & `xklb-1.31.7/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/LICENSE` & `xklb-1.31.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/README.md` & `xklb-1.31.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.31.006)
+    xk media library subcommands (v1.31.007)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-1.31.6/pyproject.toml` & `xklb-1.31.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.31.6/PKG-INFO` & `xklb-1.31.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.31.6
+Version: 1.31.7
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -224,15 +224,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.31.006)
+    xk media library subcommands (v1.31.007)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

