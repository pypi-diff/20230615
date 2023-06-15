# Comparing `tmp/xklb-1.31.5.tar.gz` & `tmp/xklb-1.31.6.tar.gz`

## Comparing `xklb-1.31.5.tar` & `xklb-1.31.6.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.31.5/.gitattributes
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 xklb-1.31.5/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.31.5/Windows.md
--rw-r--r--   0        0        0   490396 2020-02-02 00:00:00.000000 xklb-1.31.5/pdm.lock
--rw-r--r--   0        0        0    19420 2020-02-02 00:00:00.000000 xklb-1.31.5/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.31.5/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.31.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.31.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-1.31.5/.github/workflows/green.yaml
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-1.31.5/.github/workflows/push.yaml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/__init__.py
--rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/av.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/books.py
--rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/consts.py
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/db.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/dl_config.py
--rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/dl_extract.py
--rw-r--r--   0        0        0    14103 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/fs_extract.py
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/gdl_backend.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/gdl_extract.py
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/gui.py
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/hn_extract.py
--rw-r--r--   0        0        0    11781 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/lb.py
--rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/media.py
--rw-r--r--   0        0        0    25148 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/play_actions.py
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/playback.py
--rw-r--r--   0        0        0    35233 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/player.py
--rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/playlists.py
--rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/praw_extract.py
--rw-r--r--   0        0        0     7949 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/search.py
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/subtitle.py
--rw-r--r--   0        0        0     6029 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/tabs_actions.py
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/tabs_extract.py
--rw-r--r--   0        0        0    15396 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/tube_backend.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/tube_extract.py
--rw-r--r--   0        0        0    76102 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/usage.py
--rw-r--r--   0        0        0    37338 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/scripts/block.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/scripts/christen.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/scripts/dedupe_db.py
--rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/scripts/history.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     6044 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/scripts/relmv.py
--rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.31.5/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.31.5/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.31.5/LICENSE
--rw-r--r--   0        0        0    98892 2020-02-02 00:00:00.000000 xklb-1.31.5/README.md
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 xklb-1.31.5/pyproject.toml
--rw-r--r--   0        0        0   102519 2020-02-02 00:00:00.000000 xklb-1.31.5/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.31.6/.gitattributes
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 xklb-1.31.6/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.31.6/Windows.md
+-rw-r--r--   0        0        0   490396 2020-02-02 00:00:00.000000 xklb-1.31.6/pdm.lock
+-rw-r--r--   0        0        0    19420 2020-02-02 00:00:00.000000 xklb-1.31.6/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.31.6/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.31.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.31.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-1.31.6/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-1.31.6/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/__init__.py
+-rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/av.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/books.py
+-rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/consts.py
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/db.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/dl_config.py
+-rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/dl_extract.py
+-rw-r--r--   0        0        0    14103 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/fs_extract.py
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/gdl_backend.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/gdl_extract.py
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/gui.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/hn_extract.py
+-rw-r--r--   0        0        0    11781 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/lb.py
+-rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/media.py
+-rw-r--r--   0        0        0    25252 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/play_actions.py
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/playback.py
+-rw-r--r--   0        0        0    35233 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/player.py
+-rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/playlists.py
+-rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/praw_extract.py
+-rw-r--r--   0        0        0     7949 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/search.py
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/subtitle.py
+-rw-r--r--   0        0        0     6029 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    15396 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/tube_backend.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/tube_extract.py
+-rw-r--r--   0        0        0    76102 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/usage.py
+-rw-r--r--   0        0        0    37338 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/block.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/dedupe_db.py
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/history.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     6044 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.31.6/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.31.6/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.31.6/LICENSE
+-rw-r--r--   0        0        0    98892 2020-02-02 00:00:00.000000 xklb-1.31.6/README.md
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 xklb-1.31.6/pyproject.toml
+-rw-r--r--   0        0        0   102519 2020-02-02 00:00:00.000000 xklb-1.31.6/PKG-INFO
```

### Comparing `xklb-1.31.5/TODO` & `xklb-1.31.6/TODO`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/Windows.md` & `xklb-1.31.6/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/pdm.lock` & `xklb-1.31.6/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/readme.py` & `xklb-1.31.6/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.31.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.31.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/.github/workflows/push.yaml` & `xklb-1.31.6/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/av.py` & `xklb-1.31.6/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/books.py` & `xklb-1.31.6/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/consts.py` & `xklb-1.31.6/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/db.py` & `xklb-1.31.6/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/dl_config.py` & `xklb-1.31.6/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/dl_extract.py` & `xklb-1.31.6/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/fs_extract.py` & `xklb-1.31.6/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/gdl_backend.py` & `xklb-1.31.6/xklb/gdl_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/gdl_extract.py` & `xklb-1.31.6/xklb/gdl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/gui.py` & `xklb-1.31.6/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/hn_extract.py` & `xklb-1.31.6/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/lb.py` & `xklb-1.31.6/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/media.py` & `xklb-1.31.6/xklb/media.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/play_actions.py` & `xklb-1.31.6/xklb/play_actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,14 +169,15 @@
     parser.add_argument("--sibling", "--episode", action="store_true")
     parser.add_argument("--solo", action="store_true")
 
     parser.add_argument("--sort-by")
     parser.add_argument("--depth", "-D", default=0, type=int, help="Depth of folders")
     parser.add_argument("--lower", type=int, help="Number of files per folder lower limit")
     parser.add_argument("--upper", type=int, help="Number of files per folder upper limit")
+    parser.add_argument("--folder-size", "--foldersize", "-Z", action="append", help=argparse.SUPPRESS)
 
     parser.add_argument("--prefetch", type=int, default=1)
     parser.add_argument("--prefix", default="", help=argparse.SUPPRESS)
     parser.add_argument(
         "--folder",
         action="store_true",
         help="Experimental escape hatch to open folder; breaks a lot of features like post-actions",
```

### Comparing `xklb-1.31.5/xklb/playback.py` & `xklb-1.31.6/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/player.py` & `xklb-1.31.6/xklb/player.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/playlists.py` & `xklb-1.31.6/xklb/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/praw_extract.py` & `xklb-1.31.6/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/search.py` & `xklb-1.31.6/xklb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/subtitle.py` & `xklb-1.31.6/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/tabs_actions.py` & `xklb-1.31.6/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/tabs_extract.py` & `xklb-1.31.6/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/tube_backend.py` & `xklb-1.31.6/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/tube_extract.py` & `xklb-1.31.6/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/usage.py` & `xklb-1.31.6/xklb/usage.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/utils.py` & `xklb-1.31.6/xklb/utils.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/scripts/bigdirs.py` & `xklb-1.31.6/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/scripts/block.py` & `xklb-1.31.6/xklb/scripts/block.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/scripts/christen.py` & `xklb-1.31.6/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/scripts/cluster_sort.py` & `xklb-1.31.6/xklb/scripts/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/scripts/copy_play_counts.py` & `xklb-1.31.6/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/scripts/dedupe.py` & `xklb-1.31.6/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/scripts/dedupe_db.py` & `xklb-1.31.6/xklb/scripts/dedupe_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,16 +70,20 @@
                     ORDER BY {','.join(args.primary_keys)}
                     """
                 )
             )
             log.info("%s (%s rows)", col, len(data))
 
             with args.db.conn:
-                gen_where_sql = lambda row: ' AND '.join([f'{key} = {args.db.quote(row[key])}' for key in args.business_keys])
-                gen_update_sql = lambda row: f"UPDATE {args.table} SET {col} = {args.db.quote(row[col])} WHERE {gen_where_sql(row)};"
+                gen_where_sql = lambda row: " AND ".join(
+                    [f"{key} = {args.db.quote(row[key])}" for key in args.business_keys]
+                )
+                gen_update_sql = (
+                    lambda row: f"UPDATE {args.table} SET {col} = {args.db.quote(row[col])} WHERE {gen_where_sql(row)};"
+                )
                 args.db.conn.executescript("\n".join([gen_update_sql(row) for row in data]))
 
     with args.db.conn:
         args.db.conn.execute(
             f"""
             DELETE FROM {args.table}
             WHERE ({','.join(args.primary_keys)}) NOT IN (
```

### Comparing `xklb-1.31.5/xklb/scripts/download_status.py` & `xklb-1.31.6/xklb/scripts/download_status.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/scripts/history.py` & `xklb-1.31.6/xklb/scripts/history.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/scripts/merge_dbs.py` & `xklb-1.31.6/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/scripts/merge_online_local.py` & `xklb-1.31.6/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/scripts/move_list.py` & `xklb-1.31.6/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/scripts/optimize_db.py` & `xklb-1.31.6/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/scripts/playlists.py` & `xklb-1.31.6/xklb/scripts/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/scripts/redownload.py` & `xklb-1.31.6/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/scripts/relmv.py` & `xklb-1.31.6/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/scripts/scatter.py` & `xklb-1.31.6/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/scripts/streaming_tab_loader.py` & `xklb-1.31.6/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/scripts/mining/data.py` & `xklb-1.31.6/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/scripts/mining/extract_links.py` & `xklb-1.31.6/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/scripts/mining/nouns.py` & `xklb-1.31.6/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/scripts/mining/pushshift.py` & `xklb-1.31.6/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.31.6/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/xklb/assets/kotobago.png` & `xklb-1.31.6/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/.gitignore` & `xklb-1.31.6/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/LICENSE` & `xklb-1.31.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/README.md` & `xklb-1.31.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.31.005)
+    xk media library subcommands (v1.31.006)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-1.31.5/pyproject.toml` & `xklb-1.31.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.31.5/PKG-INFO` & `xklb-1.31.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.31.5
+Version: 1.31.6
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
-    xk media library subcommands (v1.31.005)
+    xk media library subcommands (v1.31.006)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

