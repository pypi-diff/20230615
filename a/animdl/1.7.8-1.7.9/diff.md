# Comparing `tmp/animdl-1.7.8.tar.gz` & `tmp/animdl-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animdl-1.7.8.tar", max compression
+gzip compressed data, was "animdl-1.7.9.tar", max compression
```

## Comparing `animdl-1.7.8.tar` & `animdl-1.7.9.tar`

### file list

```diff
@@ -1,99 +1,100 @@
--rw-r--r--   0        0        0    35149 2023-03-08 04:07:01.079242 animdl-1.7.8/LICENSE
--rw-r--r--   0        0        0       20 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/__init__.py
--rw-r--r--   0        0        0     3140 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/__main__.py
--rw-r--r--   0        0        0       71 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/__init__.py
--rw-r--r--   0        0        0       18 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/__version__.py
--rw-r--r--   0        0        0        0 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/commands/__init__.py
--rw-r--r--   0        0        0     4282 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/commands/download.py
--rw-r--r--   0        0        0     1345 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/commands/grab.py
--rw-r--r--   0        0        0     3273 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/commands/schedule.py
--rw-r--r--   0        0        0     1645 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/commands/search.py
--rw-r--r--   0        0        0     8630 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/commands/stream.py
--rw-r--r--   0        0        0     3319 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/commands/update.py
--rw-r--r--   0        0        0      112 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/exit_codes.py
--rw-r--r--   0        0        0     4308 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/helpers/__init__.py
--rw-r--r--   0        0        0     1762 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/helpers/aniskip.py
--rw-r--r--   0        0        0     2314 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/helpers/banner.py
--rw-r--r--   0        0        0      262 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/helpers/constants.py
--rw-r--r--   0        0        0     4250 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/helpers/decorators.py
--rw-r--r--   0        0        0     1093 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/helpers/fuzzysearch.py
--rw-r--r--   0        0        0     6940 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/helpers/intelliq.py
--rw-r--r--   0        0        0     2589 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/helpers/logger.py
--rw-r--r--   0        0        0     1567 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/helpers/player.py
--rw-r--r--   0        0        0      343 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/helpers/players/__init__.py
--rw-r--r--   0        0        0      757 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/helpers/players/android.py
--rw-r--r--   0        0        0     2094 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/helpers/players/base_player.py
--rw-r--r--   0        0        0      725 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/helpers/players/ffplay.py
--rw-r--r--   0        0        0     2527 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/helpers/players/mpv.py
--rw-r--r--   0        0        0     1515 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/helpers/players/vlc.py
--rw-r--r--   0        0        0     1476 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/helpers/processors.py
--rw-r--r--   0        0        0     5095 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/helpers/prompts.py
--rw-r--r--   0        0        0     3032 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/helpers/rpc.py
--rw-r--r--   0        0        0     7687 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/helpers/searcher.py
--rw-r--r--   0        0        0     1009 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/helpers/special.py
--rw-r--r--   0        0        0     2004 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/helpers/stream_handlers.py
--rw-r--r--   0        0        0      566 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/cli/http_client.py
--rw-r--r--   0        0        0       26 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/__init__.py
--rw-r--r--   0        0        0       55 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/downloader/__init__.py
--rw-r--r--   0        0        0    52198 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/downloader/content_mt.py
--rw-r--r--   0        0        0     7053 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/downloader/ffmpeg.py
--rw-r--r--   0        0        0     9100 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/downloader/handle.py
--rw-r--r--   0        0        0     4844 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/downloader/hls.py
--rw-r--r--   0        0        0     1473 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/downloader/idmanlib.py
--rw-r--r--   0        0        0      434 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/extractors/__init__.py
--rw-r--r--   0        0        0     1371 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/extractors/dailymotion/__init__.py
--rw-r--r--   0        0        0      866 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/extractors/doodstream/__init__.py
--rw-r--r--   0        0        0     2148 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/extractors/gogoplay/__init__.py
--rw-r--r--   0        0        0     1087 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/extractors/mp4upload/__init__.py
--rw-r--r--   0        0        0       32 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/extractors/mycloud/__init__.py
--rw-r--r--   0        0        0      990 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/extractors/okru/__init__.py
--rw-r--r--   0        0        0     1211 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/extractors/rapidvideo/__init__.py
--rw-r--r--   0        0        0     2103 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/extractors/rapidvideo/polling.py
--rw-r--r--   0        0        0      812 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/extractors/rapidvideo/utils.py
--rw-r--r--   0        0        0      899 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/extractors/streamlare/__init__.py
--rw-r--r--   0        0        0     1103 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/extractors/streamsb/__init__.py
--rw-r--r--   0        0        0      910 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/extractors/streamtape/__init__.py
--rw-r--r--   0        0        0      373 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/extractors/videobin/__init__.py
--rw-r--r--   0        0        0     2349 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/extractors/vidstream/__init__.py
--rw-r--r--   0        0        0     1884 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/helpers/__init__.py
--rw-r--r--   0        0        0     2040 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/helpers/superscrapers.py
--rw-r--r--   0        0        0     2579 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/helpers/uwu.py
--rw-r--r--   0        0        0     1034 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/providers/__init__.py
--rw-r--r--   0        0        0     5250 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/providers/allanime/__init__.py
--rw-r--r--   0        0        0     2320 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/providers/animekaizoku/__init__.py
--rw-r--r--   0        0        0     2402 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/providers/animeonsen/__init__.py
--rw-r--r--   0        0        0     1742 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/providers/animeout/__init__.py
--rw-r--r--   0        0        0     2742 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/providers/animepahe/__init__.py
--rw-r--r--   0        0        0     1751 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/providers/animepahe/inner/__init__.py
--rw-r--r--   0        0        0     1009 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/providers/animepahe/inner/archive.py
--rw-r--r--   0        0        0     2823 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/providers/animexin/__init__.py
--rw-r--r--   0        0        0      394 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/providers/animixplay/__init__.py
--rw-r--r--   0        0        0     1187 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/providers/animixplay/hardstream.py
--rw-r--r--   0        0        0     2740 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/providers/animixplay/stream_url.py
--rw-r--r--   0        0        0     1846 2023-03-08 04:07:01.079242 animdl-1.7.8/animdl/core/codebase/providers/animtime/__init__.py
--rw-r--r--   0        0        0     2866 2023-03-08 04:07:01.083242 animdl-1.7.8/animdl/core/codebase/providers/crunchyroll/__init__.py
--rw-r--r--   0        0        0     2322 2023-03-08 04:07:01.083242 animdl-1.7.8/animdl/core/codebase/providers/gogoanime/__init__.py
--rw-r--r--   0        0        0     1511 2023-03-08 04:07:01.083242 animdl-1.7.8/animdl/core/codebase/providers/hahomoe/__init__.py
--rw-r--r--   0        0        0     1793 2023-03-08 04:07:01.083242 animdl-1.7.8/animdl/core/codebase/providers/hentaistream/__init__.py
--rw-r--r--   0        0        0     2814 2023-03-08 04:07:01.083242 animdl-1.7.8/animdl/core/codebase/providers/kamyroll/__init__.py
--rw-r--r--   0        0        0     2890 2023-03-08 04:07:01.083242 animdl-1.7.8/animdl/core/codebase/providers/kamyroll/api.py
--rw-r--r--   0        0        0     1819 2023-03-08 04:07:01.083242 animdl-1.7.8/animdl/core/codebase/providers/kawaiifu/__init__.py
--rw-r--r--   0        0        0     2311 2023-03-08 04:07:01.083242 animdl-1.7.8/animdl/core/codebase/providers/marinmoe/__init__.py
--rw-r--r--   0        0        0     2213 2023-03-08 04:07:01.083242 animdl-1.7.8/animdl/core/codebase/providers/nineanime/__init__.py
--rw-r--r--   0        0        0     1721 2023-03-08 04:07:01.083242 animdl-1.7.8/animdl/core/codebase/providers/nineanime/decipher.py
--rw-r--r--   0        0        0     1260 2023-03-08 04:07:01.083242 animdl-1.7.8/animdl/core/codebase/providers/twistmoe/__init__.py
--rw-r--r--   0        0        0     1611 2023-03-08 04:07:01.083242 animdl-1.7.8/animdl/core/codebase/providers/twistmoe/stream_url.py
--rw-r--r--   0        0        0     1901 2023-03-08 04:07:01.083242 animdl-1.7.8/animdl/core/codebase/providers/yugen/__init__.py
--rw-r--r--   0        0        0     2542 2023-03-08 04:07:01.083242 animdl-1.7.8/animdl/core/codebase/providers/zoro/__init__.py
--rw-r--r--   0        0        0     6046 2023-03-08 04:07:01.083242 animdl-1.7.8/animdl/core/config/__init__.py
--rw-r--r--   0        0        0     4306 2023-03-08 04:07:01.083242 animdl-1.7.8/animdl/core/package_resolver.py
--rw-r--r--   0        0        0      283 2023-03-08 04:07:01.083242 animdl-1.7.8/animdl/utils/__init__.py
--rw-r--r--   0        0        0     7278 2023-03-08 04:07:01.083242 animdl-1.7.8/animdl/utils/http_caching.py
--rw-r--r--   0        0        0     3934 2023-03-08 04:07:01.083242 animdl-1.7.8/animdl/utils/http_client.py
--rw-r--r--   0        0        0      388 2023-03-08 04:07:01.083242 animdl-1.7.8/animdl/utils/optopt.py
--rw-r--r--   0        0        0     1898 2023-03-08 04:07:01.083242 animdl-1.7.8/animdl/utils/powertools.py
--rw-r--r--   0        0        0     1777 2023-03-08 04:07:01.083242 animdl-1.7.8/animdl/utils/searching.py
--rw-r--r--   0        0        0      887 2023-03-08 04:07:01.099242 animdl-1.7.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-08 04:07:01.099242 animdl-1.7.8/readme.txt
--rw-r--r--   0        0        0     1293 1970-01-01 00:00:00.000000 animdl-1.7.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-03-08 04:47:18.962161 animdl-1.7.9/LICENSE
+-rw-r--r--   0        0        0       20 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/__init__.py
+-rw-r--r--   0        0        0     3140 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/__main__.py
+-rw-r--r--   0        0        0       71 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/__init__.py
+-rw-r--r--   0        0        0       18 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/__version__.py
+-rw-r--r--   0        0        0        0 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/commands/__init__.py
+-rw-r--r--   0        0        0     4282 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/commands/download.py
+-rw-r--r--   0        0        0     1345 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/commands/grab.py
+-rw-r--r--   0        0        0     3273 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/commands/schedule.py
+-rw-r--r--   0        0        0     1645 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/commands/search.py
+-rw-r--r--   0        0        0     8630 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/commands/stream.py
+-rw-r--r--   0        0        0     3319 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/commands/update.py
+-rw-r--r--   0        0        0      112 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/exit_codes.py
+-rw-r--r--   0        0        0     4308 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/helpers/__init__.py
+-rw-r--r--   0        0        0     1762 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/helpers/aniskip.py
+-rw-r--r--   0        0        0     2314 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/helpers/banner.py
+-rw-r--r--   0        0        0      262 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/helpers/constants.py
+-rw-r--r--   0        0        0     4250 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/helpers/decorators.py
+-rw-r--r--   0        0        0     1093 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/helpers/fuzzysearch.py
+-rw-r--r--   0        0        0     6940 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/helpers/intelliq.py
+-rw-r--r--   0        0        0     2589 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/helpers/logger.py
+-rw-r--r--   0        0        0     1567 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/helpers/player.py
+-rw-r--r--   0        0        0      343 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/helpers/players/__init__.py
+-rw-r--r--   0        0        0      757 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/helpers/players/android.py
+-rw-r--r--   0        0        0     2094 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/helpers/players/base_player.py
+-rw-r--r--   0        0        0      725 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/helpers/players/ffplay.py
+-rw-r--r--   0        0        0     2527 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/helpers/players/mpv.py
+-rw-r--r--   0        0        0     1515 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/helpers/players/vlc.py
+-rw-r--r--   0        0        0     1476 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/helpers/processors.py
+-rw-r--r--   0        0        0     5095 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/helpers/prompts.py
+-rw-r--r--   0        0        0     3032 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/helpers/rpc.py
+-rw-r--r--   0        0        0     6835 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/helpers/searcher.py
+-rw-r--r--   0        0        0     1009 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/helpers/special.py
+-rw-r--r--   0        0        0     2004 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/helpers/stream_handlers.py
+-rw-r--r--   0        0        0      566 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/cli/http_client.py
+-rw-r--r--   0        0        0       26 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/codebase/__init__.py
+-rw-r--r--   0        0        0       55 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/codebase/downloader/__init__.py
+-rw-r--r--   0        0        0    52198 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/codebase/downloader/content_mt.py
+-rw-r--r--   0        0        0     7053 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/codebase/downloader/ffmpeg.py
+-rw-r--r--   0        0        0     9100 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/codebase/downloader/handle.py
+-rw-r--r--   0        0        0     4844 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/codebase/downloader/hls.py
+-rw-r--r--   0        0        0     1473 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/codebase/downloader/idmanlib.py
+-rw-r--r--   0        0        0      434 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/codebase/extractors/__init__.py
+-rw-r--r--   0        0        0     1371 2023-03-08 04:47:18.962161 animdl-1.7.9/animdl/core/codebase/extractors/dailymotion/__init__.py
+-rw-r--r--   0        0        0      866 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/extractors/doodstream/__init__.py
+-rw-r--r--   0        0        0     2148 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/extractors/gogoplay/__init__.py
+-rw-r--r--   0        0        0     1087 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/extractors/mp4upload/__init__.py
+-rw-r--r--   0        0        0       32 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/extractors/mycloud/__init__.py
+-rw-r--r--   0        0        0      990 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/extractors/okru/__init__.py
+-rw-r--r--   0        0        0     1211 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/extractors/rapidvideo/__init__.py
+-rw-r--r--   0        0        0     2103 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/extractors/rapidvideo/polling.py
+-rw-r--r--   0        0        0      812 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/extractors/rapidvideo/utils.py
+-rw-r--r--   0        0        0      899 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/extractors/streamlare/__init__.py
+-rw-r--r--   0        0        0     1103 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/extractors/streamsb/__init__.py
+-rw-r--r--   0        0        0      910 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/extractors/streamtape/__init__.py
+-rw-r--r--   0        0        0      373 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/extractors/videobin/__init__.py
+-rw-r--r--   0        0        0     2349 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/extractors/vidstream/__init__.py
+-rw-r--r--   0        0        0     1884 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/helpers/__init__.py
+-rw-r--r--   0        0        0     2040 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/helpers/superscrapers.py
+-rw-r--r--   0        0        0     2579 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/helpers/uwu.py
+-rw-r--r--   0        0        0     1034 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/__init__.py
+-rw-r--r--   0        0        0     3829 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/allanime/__init__.py
+-rw-r--r--   0        0        0     4982 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/allanime/gql_api.py
+-rw-r--r--   0        0        0     2320 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/animekaizoku/__init__.py
+-rw-r--r--   0        0        0     2402 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/animeonsen/__init__.py
+-rw-r--r--   0        0        0     1742 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/animeout/__init__.py
+-rw-r--r--   0        0        0     2742 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/animepahe/__init__.py
+-rw-r--r--   0        0        0     1751 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/animepahe/inner/__init__.py
+-rw-r--r--   0        0        0     1009 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/animepahe/inner/archive.py
+-rw-r--r--   0        0        0     2823 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/animexin/__init__.py
+-rw-r--r--   0        0        0      394 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/animixplay/__init__.py
+-rw-r--r--   0        0        0     1187 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/animixplay/hardstream.py
+-rw-r--r--   0        0        0     2740 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/animixplay/stream_url.py
+-rw-r--r--   0        0        0     1846 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/animtime/__init__.py
+-rw-r--r--   0        0        0     2866 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/crunchyroll/__init__.py
+-rw-r--r--   0        0        0     2322 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/gogoanime/__init__.py
+-rw-r--r--   0        0        0     1511 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/hahomoe/__init__.py
+-rw-r--r--   0        0        0     1793 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/hentaistream/__init__.py
+-rw-r--r--   0        0        0     2814 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/kamyroll/__init__.py
+-rw-r--r--   0        0        0     2890 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/kamyroll/api.py
+-rw-r--r--   0        0        0     1819 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/kawaiifu/__init__.py
+-rw-r--r--   0        0        0     2311 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/marinmoe/__init__.py
+-rw-r--r--   0        0        0     2213 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/nineanime/__init__.py
+-rw-r--r--   0        0        0     1721 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/nineanime/decipher.py
+-rw-r--r--   0        0        0     1260 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/twistmoe/__init__.py
+-rw-r--r--   0        0        0     1611 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/twistmoe/stream_url.py
+-rw-r--r--   0        0        0     1901 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/yugen/__init__.py
+-rw-r--r--   0        0        0     2542 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/codebase/providers/zoro/__init__.py
+-rw-r--r--   0        0        0     6046 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/config/__init__.py
+-rw-r--r--   0        0        0     4306 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/core/package_resolver.py
+-rw-r--r--   0        0        0      283 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/utils/__init__.py
+-rw-r--r--   0        0        0     7278 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/utils/http_caching.py
+-rw-r--r--   0        0        0     3934 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/utils/http_client.py
+-rw-r--r--   0        0        0      388 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/utils/optopt.py
+-rw-r--r--   0        0        0     1898 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/utils/powertools.py
+-rw-r--r--   0        0        0     1777 2023-03-08 04:47:18.966161 animdl-1.7.9/animdl/utils/searching.py
+-rw-r--r--   0        0        0      887 2023-03-08 04:47:18.982161 animdl-1.7.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-08 04:47:18.982161 animdl-1.7.9/readme.txt
+-rw-r--r--   0        0        0     1293 1970-01-01 00:00:00.000000 animdl-1.7.9/PKG-INFO
```

### Comparing `animdl-1.7.8/LICENSE` & `animdl-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/__main__.py` & `animdl-1.7.9/animdl/__main__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/cli/commands/download.py` & `animdl-1.7.9/animdl/core/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/cli/commands/grab.py` & `animdl-1.7.9/animdl/core/cli/commands/grab.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/cli/commands/schedule.py` & `animdl-1.7.9/animdl/core/cli/commands/schedule.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/cli/commands/search.py` & `animdl-1.7.9/animdl/core/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/cli/commands/stream.py` & `animdl-1.7.9/animdl/core/cli/commands/stream.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/cli/commands/update.py` & `animdl-1.7.9/animdl/core/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/cli/helpers/__init__.py` & `animdl-1.7.9/animdl/core/cli/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/cli/helpers/aniskip.py` & `animdl-1.7.9/animdl/core/cli/helpers/aniskip.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/cli/helpers/banner.py` & `animdl-1.7.9/animdl/core/cli/helpers/banner.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/cli/helpers/decorators.py` & `animdl-1.7.9/animdl/core/cli/helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/cli/helpers/fuzzysearch.py` & `animdl-1.7.9/animdl/core/cli/helpers/fuzzysearch.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/cli/helpers/intelliq.py` & `animdl-1.7.9/animdl/core/cli/helpers/intelliq.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/cli/helpers/logger.py` & `animdl-1.7.9/animdl/core/cli/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/cli/helpers/player.py` & `animdl-1.7.9/animdl/core/cli/helpers/player.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/cli/helpers/players/android.py` & `animdl-1.7.9/animdl/core/cli/helpers/players/android.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/cli/helpers/players/base_player.py` & `animdl-1.7.9/animdl/core/cli/helpers/players/base_player.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/cli/helpers/players/ffplay.py` & `animdl-1.7.9/animdl/core/cli/helpers/players/ffplay.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/cli/helpers/players/mpv.py` & `animdl-1.7.9/animdl/core/cli/helpers/players/mpv.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/cli/helpers/players/vlc.py` & `animdl-1.7.9/animdl/core/cli/helpers/players/vlc.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/cli/helpers/processors.py` & `animdl-1.7.9/animdl/core/cli/helpers/processors.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/cli/helpers/prompts.py` & `animdl-1.7.9/animdl/core/cli/helpers/prompts.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/cli/helpers/rpc.py` & `animdl-1.7.9/animdl/core/cli/helpers/rpc.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/cli/helpers/searcher.py` & `animdl-1.7.9/animdl/core/cli/helpers/searcher.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 import json
 from urllib.parse import unquote
 
 import lxml.html as htmlparser
 
+from animdl.core.codebase.providers.allanime import gql_api as allanime_gql_api
 from animdl.utils.powertools import ctx
 
 from ...codebase.helpers import uwu
 from ...codebase.providers.kamyroll.api import get_api
 from ...config import (
     ALLANIME,
     ANIMEKAIZOKU,
@@ -48,58 +49,17 @@
     for results in animekaizoku_results.cssselect(".post-title"):
         yield {
             "anime_url": ANIMEKAIZOKU + results.cssselect("a")[0].get("href"),
             "name": results.text_content(),
         }
 
 
-ALLANIME_GQL = """
-query(
-        $search: SearchInput
-        $translationType: VaildTranslationTypeEnumType
-        $countryOrigin: VaildCountryOriginEnumType
-    ) {
-        shows(
-            search: $search
-            limit: 40
-            page: 1
-            translationType: $translationType
-            countryOrigin: $countryOrigin
-        ) {
-            pageInfo {
-                total
-            }
-            edges {
-                _id
-                name
-            }
-        }
-    }
-"""
-
-
 def search_allanime(session, query):
 
-    gql_response = session.get(
-        ALLANIME + "allanimeapi",
-        params={
-            "variables": json.dumps(
-                {
-                    "search": {
-                        "allowAdult": True,
-                        "allowUnknown": True,
-                        "query": query,
-                    },
-                }
-            ),
-            "query": ALLANIME_GQL,
-        },
-    ).json()
-
-    for result in gql_response.get("data", {}).get("shows", {}).get("edges", []):
+    for result in allanime_gql_api.api.iter_search_results(session, query):
         yield {
             "anime_url": ALLANIME + f"anime/{result['_id']}",
             "name": result["name"],
         }
 
 
 def search_animepahe(session, query):
```

### Comparing `animdl-1.7.8/animdl/core/cli/helpers/special.py` & `animdl-1.7.9/animdl/core/cli/helpers/special.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/cli/helpers/stream_handlers.py` & `animdl-1.7.9/animdl/core/cli/helpers/stream_handlers.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/cli/http_client.py` & `animdl-1.7.9/animdl/core/cli/http_client.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/downloader/content_mt.py` & `animdl-1.7.9/animdl/core/codebase/downloader/content_mt.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/downloader/ffmpeg.py` & `animdl-1.7.9/animdl/core/codebase/downloader/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/downloader/handle.py` & `animdl-1.7.9/animdl/core/codebase/downloader/handle.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/downloader/hls.py` & `animdl-1.7.9/animdl/core/codebase/downloader/hls.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/downloader/idmanlib.py` & `animdl-1.7.9/animdl/core/codebase/downloader/idmanlib.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/extractors/dailymotion/__init__.py` & `animdl-1.7.9/animdl/core/codebase/extractors/dailymotion/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/extractors/doodstream/__init__.py` & `animdl-1.7.9/animdl/core/codebase/extractors/doodstream/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/extractors/gogoplay/__init__.py` & `animdl-1.7.9/animdl/core/codebase/extractors/gogoplay/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/extractors/mp4upload/__init__.py` & `animdl-1.7.9/animdl/core/codebase/extractors/mp4upload/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/extractors/okru/__init__.py` & `animdl-1.7.9/animdl/core/codebase/extractors/okru/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/extractors/rapidvideo/__init__.py` & `animdl-1.7.9/animdl/core/codebase/extractors/rapidvideo/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/extractors/rapidvideo/polling.py` & `animdl-1.7.9/animdl/core/codebase/extractors/rapidvideo/polling.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/extractors/rapidvideo/utils.py` & `animdl-1.7.9/animdl/core/codebase/extractors/rapidvideo/utils.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/extractors/streamlare/__init__.py` & `animdl-1.7.9/animdl/core/codebase/extractors/streamlare/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/extractors/streamsb/__init__.py` & `animdl-1.7.9/animdl/core/codebase/extractors/streamsb/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/extractors/streamtape/__init__.py` & `animdl-1.7.9/animdl/core/codebase/extractors/streamtape/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/extractors/vidstream/__init__.py` & `animdl-1.7.9/animdl/core/codebase/extractors/vidstream/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/helpers/__init__.py` & `animdl-1.7.9/animdl/core/codebase/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/helpers/superscrapers.py` & `animdl-1.7.9/animdl/core/codebase/helpers/superscrapers.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/helpers/uwu.py` & `animdl-1.7.9/animdl/core/codebase/helpers/uwu.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/providers/__init__.py` & `animdl-1.7.9/animdl/core/codebase/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/providers/allanime/__init__.py` & `animdl-1.7.9/animdl/core/codebase/providers/allanime/gql_api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,202 +1,210 @@
-from collections import defaultdict
-from functools import partial
+from animdl.utils import optopt
 
-import yarl
-
-from ....config import ALLANIME, SUPERANIME_RETURN_ALL, SUPERANIME_TYPE_OF
-from ...helpers import construct_site_based_regex, optopt, superscrapers
-
-REGEX = construct_site_based_regex(ALLANIME, extra_regex=r"/anime/([^?&/]+)")
-
-
-def iter_episodes(
-    episode_dictionary: dict,
-    *,
-    selected_type_of: str = SUPERANIME_TYPE_OF,
-):
-    episodes = defaultdict(list)
-
-    for type_of, episode_numbers in episode_dictionary.items():
-        if type_of != selected_type_of:
-            continue
-
-        for episode in episode_numbers:
-            episodes[int(episode) if episode.isdigit() else 0].append(
-                (type_of, episode)
-            )
-
-    yield from sorted(episodes.items(), key=lambda x: x[0])
-
-
-def to_clock_json(url: str):
-    return optopt.regexlib.sub(r"(?<=/clock)(?=[?&#])", ".json", url, count=1)
+ENDPOINT = "https://api.allanime.co/allanimeapi"
 
+ALLANIME_SEARCH_GQL = """\
+query(
+        $search: SearchInput
+        $limit: Int
+        $page: Int
+        $translationType: VaildTranslationTypeEnumType
+        $countryOrigin: VaildCountryOriginEnumType
+    ) {
+    shows(
+        search: $search
+        limit: $limit
+        page: $page
+        translationType: $translationType
+        countryOrigin: $countryOrigin
+    ) {
+        pageInfo {
+            total
+        }
+        edges {
+            %s
+        }
+    }
+}"""
 
-ALLANIME_GQL_API = "https://api.allanime.co/allanimeapi"
 
-ALLANIME_EPISODES_GQL = """
+ALLANIME_EPISODES_GQL = """\
 query ($showId: String!, $translationType: VaildTranslationTypeEnumType!, $episodeString: String!) {
     episode(
         showId: $showId
         translationType: $translationType
         episodeString: $episodeString
     ) {
-        episodeString
-        sourceUrls
-        notes
+        %s
     }
-}
-"""
-
-ALLANIME_EPISODE_LIST_GQL = """
-query ($showId: String!) {
-    show(
-        _id: $showId
-    ) {
-        availableEpisodesDetail
-    }
-}
-"""
+}"""
 
-ALLANIME_TITLE_GQL = """
+ALLANIME_SHOW_GQL = """
 query ($showId: String!) {
     show(
         _id: $showId
     ) {
-        name
+        %s
     }
 }
 """
 
 
-def extract_content(
-    session,
-    content: "iter_episodes",
-    show_id: str,
-    *,
-    api_endpoint: str,
-    return_all: bool = SUPERANIME_RETURN_ALL,
-):
+class AllAnimeGQLAPI:
+    """
+    Fast and effective GQL API wrapper for AllAnime.
+    """
+
+    info_table = {}
+
+    def __init__(self, *, endpoint: str = ENDPOINT):
+        self.api_endpoint = endpoint
+
+    def iter_search_results(
+        self,
+        session,
+        query: str,
+        translation_type=None,
+        country_origin=None,
+        show_nsfw=True,
+        show_unknown=True,
+        limit=None,
+        *,
+        keys: tuple = (
+            "_id",
+            "name",
+            "availableEpisodesDetail",
+        ),
+    ):
+        search = {
+            "allowAdult": show_nsfw,
+            "allowUnknown": show_unknown,
+            "query": query,
+        }
+
+        variables = {
+            "search": search,
+        }
+
+        if translation_type is not None:
+            variables["translationType"] = translation_type
+
+        if country_origin is not None:
+            variables["countryOrigin"] = country_origin
+
+        current_count = 0
+        total = None
+        page = 1
+
+        gql = ALLANIME_SEARCH_GQL % " ".join(keys)
+
+        while limit is None or current_count < limit:
+            variables["page"] = page
+            variables["limit"] = limit or 40
+
+            response = session.get(
+                self.api_endpoint,
+                params={
+                    "variables": optopt.jsonlib.dumps(variables),
+                    "query": gql,
+                },
+            ).json()
+
+            edges = response.get("data", {}).get("shows", {}).get("edges", [])
+
+            if not edges:
+                return
+
+            for data in edges:
+
+                self.info_table.setdefault(data["_id"], {}).update(data)
+
+                yield data
+
+            current_count += len(edges)
+            page += 1
+
+            total = total or (
+                response.get("data", {})
+                .get("shows", {})
+                .get("pageInfo", {})
+                .get("total", limit)
+            )
+            if limit is None:
+                limit = total
 
-    for type_of, episode in content:
+    def fetch_show_info(
+        self,
+        session,
+        show_id: str,
+        keys: tuple = (
+            "_id",
+            "name",
+            "availableEpisodesDetail",
+        ),
+    ):
+        if show_id in self.info_table and (
+            keys is None or all(key in self.info_table[show_id] for key in keys)
+        ):
+            return self.info_table[show_id]
+
+        variables = {
+            "showId": show_id,
+        }
 
-        api_response = session.get(
-            ALLANIME_GQL_API,
+        response = session.get(
+            self.api_endpoint,
             params={
-                "variables": optopt.jsonlib.dumps(
-                    {
-                        "showId": show_id,
-                        "translationType": type_of,
-                        "episodeString": episode,
-                    }
-                ),
-                "query": ALLANIME_EPISODES_GQL,
+                "variables": optopt.jsonlib.dumps(variables),
+                "query": ALLANIME_SHOW_GQL % " ".join(keys),
             },
         ).json()
 
-        episode_info = api_response["data"]["episode"]
-
-        attrs = {}
-
-        if "notes" in episode_info and episode_info["notes"]:
-            attrs.update(title=episode_info["notes"].replace("<note-split>", " // "))
-
-        sources = sorted(
-            api_response["data"]["episode"]["sourceUrls"],
-            key=lambda value: value.get("priority", 0),
-            reverse=True,
+        self.info_table.setdefault(show_id, {}).update(
+            response.get("data", {}).get("show", {})
         )
 
-        if not sources:
-            continue
-
-        for source in sources:
-            if source["type"] == "iframe":
-
-                streams = (
-                    session.get(to_clock_json(api_endpoint + source["sourceUrl"]))
-                    .json()
-                    .get("links")
-                )
-
-                if not streams:
-                    continue
-
-                for stream_data in streams:
-                    if "link" in stream_data and stream_data["link"]:
-                        url = stream_data["link"]
-                    else:
-                        if not stream_data["portData"]["streams"]:
-                            continue
-
-                        stream = stream_data["portData"]["streams"][0]
-
-                        url = stream["url"]
-
-                    yield from superscrapers.iter_unpacked_from_packed_hls(
-                        session, yarl.URL(url), stream_attribs=attrs
-                    )
+        return response.get("data", {}).get("show", {})
 
-                    if not return_all:
-                        return
-
-            else:
-                yield from superscrapers.iter_unpacked_from_packed_hls(
-                    session, yarl.URL(source["sourceUrl"]), stream_attribs=attrs
-                )
-                if not return_all:
-                    return
+    def fetch_episode(
+        self,
+        session,
+        show_id: str,
+        episode_string: str,
+        *,
+        translation_type: str = "sub",
+        keys: tuple = ("episodeString", "sourceUrls", "notes"),
+    ):
+        variables = {
+            "showId": show_id,
+            "translationType": translation_type,
+            "episodeString": episode_string,
+        }
 
+        response = session.get(
+            self.api_endpoint,
+            params={
+                "variables": optopt.jsonlib.dumps(variables),
+                "query": ALLANIME_EPISODES_GQL % " ".join(keys),
+            },
+        ).json()
 
-def fetcher(session, url: "str", check, match):
+        return response.get("data", {})
 
-    api_endpoint = (
-        session.get(ALLANIME + "getVersion").json().get("episodeIframeHead", "")
-    )
+    def iter_episodes(
+        self,
+        session,
+        show_id: str,
+        *,
+        translation_type: str = "sub",
+    ):
+        show_info = self.fetch_show_info(session, show_id)
+
+        for episode_string in show_info.get("availableEpisodesDetail", {}).get(
+            translation_type, []
+        ):
+            yield self.fetch_episode(
+                session, show_id, episode_string, translation_type=translation_type
+            )
 
-    available_episodes = (
-        session.get(
-            ALLANIME_GQL_API,
-            params={
-                "variables": optopt.jsonlib.dumps({"showId": match.group(1)}),
-                "query": ALLANIME_EPISODE_LIST_GQL,
-            },
-        )
-        .json()
-        .get("data", {})
-        .get("show", {})
-        .get("availableEpisodesDetail", {})
-    )
-
-    for episode, content in iter_episodes(available_episodes):
-
-        if check(episode):
-            yield partial(
-                lambda session, content, show_id: list(
-                    extract_content(
-                        session, content, show_id, api_endpoint=api_endpoint
-                    )
-                ),
-                session,
-                content,
-                match.group(1),
-            ), episode
-
-
-def metadata_fetcher(session, url: "str", match):
-
-    anime_name = (
-        session.get(
-            ALLANIME_GQL_API,
-            params={
-                "variables": optopt.jsonlib.dumps({"showId": match.group(1)}),
-                "query": ALLANIME_TITLE_GQL,
-            },
-        )
-        .json()
-        .get("data", {})
-        .get("show", {})
-        .get("name", "")
-    )
 
-    return {"titles": [anime_name]}
+api = AllAnimeGQLAPI()
```

### Comparing `animdl-1.7.8/animdl/core/codebase/providers/animekaizoku/__init__.py` & `animdl-1.7.9/animdl/core/codebase/providers/animekaizoku/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/providers/animeonsen/__init__.py` & `animdl-1.7.9/animdl/core/codebase/providers/animeonsen/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/providers/animeout/__init__.py` & `animdl-1.7.9/animdl/core/codebase/providers/animeout/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/providers/animepahe/__init__.py` & `animdl-1.7.9/animdl/core/codebase/providers/animepahe/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/providers/animepahe/inner/__init__.py` & `animdl-1.7.9/animdl/core/codebase/providers/animepahe/inner/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/providers/animepahe/inner/archive.py` & `animdl-1.7.9/animdl/core/codebase/providers/animepahe/inner/archive.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/providers/animexin/__init__.py` & `animdl-1.7.9/animdl/core/codebase/providers/animexin/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/providers/animixplay/hardstream.py` & `animdl-1.7.9/animdl/core/codebase/providers/animixplay/hardstream.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/providers/animixplay/stream_url.py` & `animdl-1.7.9/animdl/core/codebase/providers/animixplay/stream_url.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/providers/animtime/__init__.py` & `animdl-1.7.9/animdl/core/codebase/providers/animtime/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/providers/crunchyroll/__init__.py` & `animdl-1.7.9/animdl/core/codebase/providers/crunchyroll/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/providers/gogoanime/__init__.py` & `animdl-1.7.9/animdl/core/codebase/providers/gogoanime/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/providers/hahomoe/__init__.py` & `animdl-1.7.9/animdl/core/codebase/providers/hahomoe/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/providers/hentaistream/__init__.py` & `animdl-1.7.9/animdl/core/codebase/providers/hentaistream/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/providers/kamyroll/__init__.py` & `animdl-1.7.9/animdl/core/codebase/providers/kamyroll/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/providers/kamyroll/api.py` & `animdl-1.7.9/animdl/core/codebase/providers/kamyroll/api.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/providers/kawaiifu/__init__.py` & `animdl-1.7.9/animdl/core/codebase/providers/kawaiifu/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/providers/marinmoe/__init__.py` & `animdl-1.7.9/animdl/core/codebase/providers/marinmoe/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/providers/nineanime/__init__.py` & `animdl-1.7.9/animdl/core/codebase/providers/nineanime/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/providers/nineanime/decipher.py` & `animdl-1.7.9/animdl/core/codebase/providers/nineanime/decipher.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/providers/twistmoe/__init__.py` & `animdl-1.7.9/animdl/core/codebase/providers/twistmoe/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/providers/twistmoe/stream_url.py` & `animdl-1.7.9/animdl/core/codebase/providers/twistmoe/stream_url.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/providers/yugen/__init__.py` & `animdl-1.7.9/animdl/core/codebase/providers/yugen/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/codebase/providers/zoro/__init__.py` & `animdl-1.7.9/animdl/core/codebase/providers/zoro/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/config/__init__.py` & `animdl-1.7.9/animdl/core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/core/package_resolver.py` & `animdl-1.7.9/animdl/core/package_resolver.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/utils/http_caching.py` & `animdl-1.7.9/animdl/utils/http_caching.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/utils/http_client.py` & `animdl-1.7.9/animdl/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/utils/powertools.py` & `animdl-1.7.9/animdl/utils/powertools.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/animdl/utils/searching.py` & `animdl-1.7.9/animdl/utils/searching.py`

 * *Files identical despite different names*

### Comparing `animdl-1.7.8/pyproject.toml` & `animdl-1.7.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "animdl"
-version = "1.7.8"
+version = "1.7.9"
 description = "A highly efficient, fast, powerful and light-weight anime downloader and streamer for your favorite anime."
 readme = "readme.txt"
 authors = [ "justfoolingaround <kr.justfoolingaround@gmail.com>",]
 license = "GPT-3"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
```

### Comparing `animdl-1.7.8/PKG-INFO` & `animdl-1.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animdl
-Version: 1.7.8
+Version: 1.7.9
 Summary: A highly efficient, fast, powerful and light-weight anime downloader and streamer for your favorite anime.
 License: GPT-3
 Author: justfoolingaround
 Author-email: kr.justfoolingaround@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

