# Comparing `tmp/TMDBTraktSyncer-1.2.0.tar.gz` & `tmp/TMDBTraktSyncer-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMDBTraktSyncer-1.2.0.tar", last modified: Mon Jun  5 08:05:09 2023, max compression
+gzip compressed data, was "TMDBTraktSyncer-1.3.0.tar", last modified: Thu Jun 15 16:56:06 2023, max compression
```

## Comparing `TMDBTraktSyncer-1.2.0.tar` & `TMDBTraktSyncer-1.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 08:05:09.555062 TMDBTraktSyncer-1.2.0/
--rw-rw-rw-   0        0        0     1079 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.2.0/LICENSE
--rw-rw-rw-   0        0        0    10794 2023-06-05 08:05:09.554074 TMDBTraktSyncer-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    10048 2023-06-05 08:01:07.000000 TMDBTraktSyncer-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 08:05:09.523999 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer/
--rw-rw-rw-   0        0        0    10142 2023-06-02 06:29:12.000000 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer/TMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     4440 2023-05-28 13:31:50.000000 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     8916 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     3952 2023-05-24 00:42:48.000000 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer/tmdbData.py
--rw-rw-rw-   0        0        0     3046 2023-05-31 11:17:57.000000 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0     3325 2023-05-24 00:34:12.000000 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-06-05 08:05:09.552073 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0    10794 2023-06-05 08:05:09.000000 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      481 2023-06-05 08:05:09.000000 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 08:05:09.000000 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-06-05 08:05:09.000000 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-06-05 08:05:09.000000 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-05 08:05:09.000000 TMDBTraktSyncer-1.2.0/TMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 08:05:09.555062 TMDBTraktSyncer-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1334 2023-06-05 08:04:41.000000 TMDBTraktSyncer-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 16:56:06.226338 TMDBTraktSyncer-1.3.0/
+-rw-rw-rw-   0        0        0     1079 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0    10774 2023-06-15 16:56:06.225338 TMDBTraktSyncer-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10026 2023-06-15 16:29:12.000000 TMDBTraktSyncer-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 16:56:06.194354 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    16789 2023-06-15 16:10:43.000000 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer/TMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     4440 2023-05-28 13:31:50.000000 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     9033 2023-06-15 14:40:44.000000 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     3977 2023-06-15 14:30:16.000000 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer/tmdbData.py
+-rw-rw-rw-   0        0        0     7039 2023-06-15 15:19:15.000000 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     7315 2023-06-15 16:15:40.000000 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-06-15 16:56:06.223338 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    10774 2023-06-15 16:56:06.000000 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      481 2023-06-15 16:56:06.000000 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 16:56:06.000000 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-06-15 16:56:06.000000 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-06-15 16:56:06.000000 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-15 16:56:06.000000 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 16:56:06.226338 TMDBTraktSyncer-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1341 2023-06-15 16:55:45.000000 TMDBTraktSyncer-1.3.0/setup.py
```

### Comparing `TMDBTraktSyncer-1.2.0/LICENSE` & `TMDBTraktSyncer-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.2.0/PKG-INFO` & `TMDBTraktSyncer-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.2.0
-Summary: This python script syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.
+Version: 1.3.0
+Summary: A python script that syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # TMDB-Trakt-Syncer
 
-This Python script syncs user watchlist and ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Data already set will not be overwritten. Ratings are synced by default and watchlist sync is optional. The user will be prompted to enter their preferences and api keys on first run. 
+This Python script syncs user watchlist and ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Data already set will not be overwritten. Ratings and watchlist sync are both optional. The user will be prompted to enter their settings and api keys on first run.
 
 The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/TMDB-Trakt-Syncer#other-recommended-projects).
 
 ## Installation Instructions:
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
 2. Install the script by running `python -m pip install TMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDbTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
    - Type of use: `Personal`
    - Application name: `TMDB-Trakt-Sync`
    - Application URL: `https://github.com/RileyXX/TMDB-Trakt-Syncer`
    - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms.`
    - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
 5. Run the script by running `TMDBTraktSyncer` in the command line.
-6. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
+6. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
 7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
 
 ## Installing the Script:
 ```
 python -m pip install TMDBTraktSyncer
 ```
 _Run in your operating system's native command line._
@@ -64,19 +64,19 @@
 ## Alternative Manual Installation Method (without pip install):
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
 2. Download the latest .zip from the [releases page](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) and extract it to the desired directory.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
    - Type of use: `Personal`
    - Application name: `TMDB-Trakt-Sync`
-   - Application URL: `localhost`
-   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`
+   - Application URL: `https://github.com/RileyXX/TMDB-Trakt-Syncer`
+   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms.`
    - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
 5. Run `TMDBTraktSyncer.py` or open the terminal and navigate to the folder where `TMDBTraktSyncer.py` is located, then run `TMDBTraktSyncer.py` in the terminal.
-6. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
+6. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
 7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
 
 ## For Setting Up Automation See the Following Wiki Pages:
 - Setup Automation for:
    - [Windows](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
    - [Linux](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
    - [macOS](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
```

### Comparing `TMDBTraktSyncer-1.2.0/README.md` & `TMDBTraktSyncer-1.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # TMDB-Trakt-Syncer
 
-This Python script syncs user watchlist and ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Data already set will not be overwritten. Ratings are synced by default and watchlist sync is optional. The user will be prompted to enter their preferences and api keys on first run. 
+This Python script syncs user watchlist and ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Data already set will not be overwritten. Ratings and watchlist sync are both optional. The user will be prompted to enter their settings and api keys on first run.
 
 The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/TMDB-Trakt-Syncer#other-recommended-projects).
 
 ## Installation Instructions:
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
 2. Install the script by running `python -m pip install TMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDbTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
    - Type of use: `Personal`
    - Application name: `TMDB-Trakt-Sync`
    - Application URL: `https://github.com/RileyXX/TMDB-Trakt-Syncer`
    - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms.`
    - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
 5. Run the script by running `TMDBTraktSyncer` in the command line.
-6. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
+6. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
 7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
 
 ## Installing the Script:
 ```
 python -m pip install TMDBTraktSyncer
 ```
 _Run in your operating system's native command line._
@@ -48,19 +48,19 @@
 ## Alternative Manual Installation Method (without pip install):
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
 2. Download the latest .zip from the [releases page](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) and extract it to the desired directory.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
    - Type of use: `Personal`
    - Application name: `TMDB-Trakt-Sync`
-   - Application URL: `localhost`
-   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`
+   - Application URL: `https://github.com/RileyXX/TMDB-Trakt-Syncer`
+   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms.`
    - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
 5. Run `TMDBTraktSyncer.py` or open the terminal and navigate to the folder where `TMDBTraktSyncer.py` is located, then run `TMDBTraktSyncer.py` in the terminal.
-6. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
+6. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
 7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
 
 ## For Setting Up Automation See the Following Wiki Pages:
 - Setup Automation for:
    - [Windows](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
    - [Linux](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
    - [macOS](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
```

### Comparing `TMDBTraktSyncer-1.2.0/TMDBTraktSyncer/TMDBTraktSyncer.py` & `TMDBTraktSyncer-1.3.0/TMDBTraktSyncer/TMDBTraktSyncer.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,27 +12,42 @@
     import tmdbData
     import errorHandling as EH
 
 
 def main():
     try:
             
-        trakt_watchlist, trakt_ratings = traktData.getTraktData()
+        trakt_watchlist, trakt_ratings, watched_content = traktData.getTraktData()
         tmdb_watchlist, tmdb_ratings = tmdbData.getTMDBRatings()
 
         #Get trakt and tmdb ratings and filter out trakt ratings with missing tmdb id
-        trakt_ratings = [rating for rating in trakt_ratings if rating['ID'] is not None]
-        tmdb_ratings = [rating for rating in tmdb_ratings if rating['ID'] is not None]
-        trakt_watchlist = [item for item in trakt_watchlist if item['ID'] is not None]
-        tmdb_watchlist = [item for item in tmdb_watchlist if item['ID'] is not None]
+        trakt_ratings = [rating for rating in trakt_ratings if rating['TMDB_ID'] is not None]
+        tmdb_ratings = [rating for rating in tmdb_ratings if rating['TMDB_ID'] is not None]
+        trakt_watchlist = [item for item in trakt_watchlist if item['TMDB_ID'] is not None]
+        tmdb_watchlist = [item for item in tmdb_watchlist if item['TMDB_ID'] is not None]
         #Filter out ratings already set
-        tmdb_ratings_to_set = [rating for rating in trakt_ratings if rating['ID'] not in [tmdb_rating['ID'] for tmdb_rating in tmdb_ratings]]
-        trakt_ratings_to_set = [rating for rating in tmdb_ratings if rating['ID'] not in [trakt_rating['ID'] for trakt_rating in trakt_ratings]]
-        tmdb_watchlist_to_set = [item for item in trakt_watchlist if item['ID'] not in [tmdb_item['ID'] for tmdb_item in tmdb_watchlist]]
-        trakt_watchlist_to_set = [item for item in tmdb_watchlist if item['ID'] not in [trakt_item['ID'] for trakt_item in trakt_watchlist]]
+        tmdb_ratings_to_set = [rating for rating in trakt_ratings if rating['TMDB_ID'] not in [tmdb_rating['TMDB_ID'] for tmdb_rating in tmdb_ratings]]
+        trakt_ratings_to_set = [rating for rating in tmdb_ratings if rating['TMDB_ID'] not in [trakt_rating['TMDB_ID'] for trakt_rating in trakt_ratings]]
+        tmdb_watchlist_to_set = [item for item in trakt_watchlist if item['TMDB_ID'] not in [tmdb_item['TMDB_ID'] for tmdb_item in tmdb_watchlist]]
+        trakt_watchlist_to_set = [item for item in tmdb_watchlist if item['TMDB_ID'] not in [trakt_item['TMDB_ID'] for trakt_item in trakt_watchlist]]
+        
+        # If remove_watched_from_watchlists_value is true
+        if VC.remove_watched_from_watchlists_value:        
+            # Get the IDs from watched_content
+            watched_content_ids = set(item['TMDB_ID'] for item in watched_content if item['TMDB_ID'])
+                    
+            # Filter out watched content from trakt_watchlist_to_set
+            trakt_watchlist_to_set = [item for item in trakt_watchlist_to_set if item['TMDB_ID'] not in watched_content_ids]
+            # Filter out watched content from trakt_watchlist_to_set
+            tmdb_watchlist_to_set = [item for item in tmdb_watchlist_to_set if item['TMDB_ID'] not in watched_content_ids]
+            
+            # Find items to remove from trakt_watchlist
+            trakt_watchlist_items_to_remove = [item for item in trakt_watchlist if item['TMDB_ID'] in watched_content_ids]
+            # Find items to remove from tmdb_watchlist
+            tmdb_watchlist_items_to_remove = [item for item in tmdb_watchlist if item['TMDB_ID'] in watched_content_ids]
         
         # If sync_watchlist_value is true
         if VC.sync_watchlist_value:
 
             # Set TMDB Watchlist Items
             if tmdb_watchlist_to_set:
                 print('Setting TMDB Watchlist Items')
@@ -48,28 +63,28 @@
                 
                 for item in tmdb_watchlist_to_set:
                     item_count += 1
                     payload = {}  # Add any additional payload parameters if required
                     if item['Type'] == 'movie':
                         url = f"https://api.themoviedb.org/3/account/{account_id}/watchlist"
                         payload['media_type'] = "movie"
-                        payload['media_id'] = item['ID']
+                        payload['media_id'] = item['TMDB_ID']
                         payload['watchlist'] = True
                         response = EH.make_tmdb_request(url, payload=payload)
 
                     elif item['Type'] == 'show':
                         url = f"https://api.themoviedb.org/3/account/{account_id}/watchlist"
                         payload['media_type'] = "tv"
-                        payload['media_id'] = item['ID']
+                        payload['media_id'] = item['TMDB_ID']
                         payload['watchlist'] = True
                         response = EH.make_tmdb_request(url, payload=payload)
                     if response:
                         print(f"Adding item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to TMDB Watchlist")
                     else:
-                        print(f"Failed to add item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to TMDB Watchlist (TMDB ID: {item['ID']})")
+                        print(f"Failed to add item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to TMDB Watchlist (TMDB ID: {item['TMDB_ID']})")
                 
                 print('Setting TMDB Watchlist Items Complete')
             else:
                 print('No TMDB Watchlist Items To Set')
 
             # Set Trakt Watchlist Items
             if trakt_watchlist_to_set:
@@ -77,15 +92,15 @@
 
                 # Count the total number of items
                 num_items = len(trakt_watchlist_to_set)
                 item_count = 0
 
                 for item in trakt_watchlist_to_set:
                     item_count += 1
-                    tmdb_id = item['ID']
+                    tmdb_id = item['TMDB_ID']
                     media_type = item['Type']  # 'movie', 'show', or 'episode'
 
                     url = f"https://api.trakt.tv/sync/watchlist"
 
                     data = {
                         "movies": [],
                         "shows": [],
@@ -111,112 +126,215 @@
                             }
                         })
 
                     response = EH.make_trakt_request(url, payload=data)
                     if response:
                         print(f"Adding item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to Trakt Watchlist")
                     else:
-                        print(f"Failed to add item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to Trakt Watchlist (TMDB ID: {item['ID']})")
+                        print(f"Failed to add item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to Trakt Watchlist (TMDB ID: {item['TMDB_ID']})")
                         print("Error Response:", response.content, response.status_code)
 
                 print('Setting Trakt Watchlist Items Complete')
             else:
                 print('No Trakt Watchlist Items To Set')
 
-        if tmdb_ratings_to_set:
-            print('Setting TMDB Ratings')
+        # If sync_ratings_value is true
+        if VC.sync_ratings_value:
             
-            # Count the total number of items to rate
-            num_items = len(tmdb_ratings_to_set)
-            item_count = 0
-            
-            # Set TMDB Rating
-            for item in tmdb_ratings_to_set:
-                item_count += 1
-
-                if item['Type'] == 'movie':
-                    payload = {
-                        'value': item['Rating']
-                    }
-                    url = f"https://api.themoviedb.org/3/movie/{item['ID']}/rating"
-                    print(f"Rating movie ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on TMDB")
+            # Set TMDB Ratings
+            if tmdb_ratings_to_set:
+                print('Setting TMDB Ratings')
+                
+                # Count the total number of items to rate
+                num_items = len(tmdb_ratings_to_set)
+                item_count = 0
+                
+                # Set TMDB Rating
+                for item in tmdb_ratings_to_set:
+                    item_count += 1
 
-                elif item['Type'] == 'show':
-                    payload = {
-                        'value': item['Rating']
-                    }
-                    url = f"https://api.themoviedb.org/3/tv/{item['ID']}/rating"
-                    print(f"Rating TV show ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on TMDB")
+                    if item['Type'] == 'movie':
+                        payload = {
+                            'value': item['Rating']
+                        }
+                        url = f"https://api.themoviedb.org/3/movie/{item['TMDB_ID']}/rating"
+                        print(f"Rating movie ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on TMDB")
 
-                elif item['Type'] == 'episode':
-                    payload = {
-                        'value': item['Rating']
-                    }
-                    url = f"https://api.themoviedb.org/3/tv/{item['ShowID']}/season/{item['Season']}/episode/{item['Episode']}/rating"
-                    print(f"Rating episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}) [S{item['Season']:02d}E{item['Episode']:02d}]: {item['Rating']}/10 on TMDB")
+                    elif item['Type'] == 'show':
+                        payload = {
+                            'value': item['Rating']
+                        }
+                        url = f"https://api.themoviedb.org/3/tv/{item['TMDB_ID']}/rating"
+                        print(f"Rating TV show ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on TMDB")
+
+                    elif item['Type'] == 'episode':
+                        payload = {
+                            'value': item['Rating']
+                        }
+                        url = f"https://api.themoviedb.org/3/tv/{item['TMDB_ShowID']}/season/{item['Season']}/episode/{item['Episode']}/rating"
+                        print(f"Rating episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}) [S{item['Season']:02d}E{item['Episode']:02d}]: {item['Rating']}/10 on TMDB")
 
-                response = EH.make_tmdb_request(url, payload=payload)
+                    response = EH.make_tmdb_request(url, payload=payload)
 
-            print('Setting TMDB Ratings Complete')
-        else:
-            print('No TMDB Ratings To Set')
+                print('Setting TMDB Ratings Complete')
+            else:
+                print('No TMDB Ratings To Set')
 
-        if trakt_ratings_to_set:
-            print('Setting Trakt Ratings')
+            # Set Trakt Ratings
+            if trakt_ratings_to_set:
+                print('Setting Trakt Ratings')
 
-            # Set the API endpoints
-            rate_url = "https://api.trakt.tv/sync/ratings"
-            
-            # Count the total number of items to rate
-            num_items = len(trakt_ratings_to_set)
-            item_count = 0
-                    
-            # Loop through your data table and rate each item on Trakt
-            for item in trakt_ratings_to_set:
-                item_count += 1
-                if item["Type"] == "show":
-                    # This is a TV show
-                    data = {
-                        "shows": [{
-                            "ids": {
-                                "tmdb": item["ID"]
-                            },
-                            "rating": item["Rating"]
-                        }]
-                    }
-                    print(f"Rating TV show ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
-                elif item["Type"] == "movie":
-                    # This is a movie
-                    data = {
-                        "movies": [{
-                            "ids": {
-                                "tmdb": item["ID"]
-                            },
-                            "rating": item["Rating"]
-                        }]
-                    }
-                    print(f"Rating movie ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
-                elif item["Type"] == "episode":
-                    # This is an episode
-                    data = {
-                        "episodes": [{
-                            "ids": {
-                                "tmdb": item["ID"]
-                            },
-                            "rating": item["Rating"]
-                        }]
-                    }
-                    print(f"Rating episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}) [S{item['Season']:02d}E{item['Episode']:02d}]: {item['Rating']}/10 on Trakt")
+                # Set the API endpoints
+                rate_url = "https://api.trakt.tv/sync/ratings"
+                
+                # Count the total number of items to rate
+                num_items = len(trakt_ratings_to_set)
+                item_count = 0
+                        
+                # Loop through your data table and rate each item on Trakt
+                for item in trakt_ratings_to_set:
+                    item_count += 1
+                    if item["Type"] == "show":
+                        # This is a TV show
+                        data = {
+                            "shows": [{
+                                "ids": {
+                                    "tmdb": item["TMDB_ID"]
+                                },
+                                "rating": item["Rating"]
+                            }]
+                        }
+                        print(f"Rating TV show ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
+                    elif item["Type"] == "movie":
+                        # This is a movie
+                        data = {
+                            "movies": [{
+                                "ids": {
+                                    "tmdb": item["TMDB_ID"]
+                                },
+                                "rating": item["Rating"]
+                            }]
+                        }
+                        print(f"Rating movie ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
+                    elif item["Type"] == "episode":
+                        # This is an episode
+                        data = {
+                            "episodes": [{
+                                "ids": {
+                                    "tmdb": item["TMDB_ID"]
+                                },
+                                "rating": item["Rating"]
+                            }]
+                        }
+                        print(f"Rating episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}) [S{item['Season']:02d}E{item['Episode']:02d}]: {item['Rating']}/10 on Trakt")
+
+                    # Make the API call to rate the item
+                    response = EH.make_trakt_request(rate_url, payload=data)
+
+                print('Setting Trakt Ratings Complete')
+            else:
+                print('No Trakt Ratings To Set')
+        
+        # If remove_watched_from_watchlists_value is true
+        if VC.remove_watched_from_watchlists_value:
+        
+            # Remove Watched Items Trakt Watchlist
+            if trakt_watchlist_items_to_remove:
+                print('Removing Watched Items From Trakt Watchlist')
+
+                # Set the API endpoint
+                remove_url = "https://api.trakt.tv/sync/watchlist/remove"
 
-                # Make the API call to rate the item
-                response = EH.make_trakt_request(rate_url, payload=data)
+                # Count the total number of items
+                num_items = len(trakt_watchlist_items_to_remove)
+                item_count = 0
+
+                # Loop through the items to remove from the watchlist
+                for item in trakt_watchlist_items_to_remove:
+                    item_count += 1
+                    if item["Type"] == "show":
+                        # This is a TV show
+                        data = {
+                            "shows": [{
+                                "ids": {
+                                    "trakt": item["TraktID"]
+                                }
+                            }]
+                        }
+                        print(f"Removing TV show ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from Trakt Watchlist")
+                    elif item["Type"] == "movie":
+                        # This is a movie
+                        data = {
+                            "movies": [{
+                                "ids": {
+                                    "trakt": item["TraktID"]
+                                }
+                            }]
+                        }
+                        print(f"Removing movie ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from Trakt Watchlist")
+                    elif item["Type"] == "episode":
+                        # This is an episode
+                        data = {
+                            "episodes": [{
+                                "ids": {
+                                    "trakt": item["TraktID"]
+                                }
+                            }]
+                        }
+                        print(f"Removing episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from Trakt Watchlist")
+
+                    # Make the API call to remove the item from the watchlist
+                    response = EH.make_trakt_request(remove_url, payload=data)
+
+                    if response is None:
+                        print(f"Error removing {item}: {response.content}")
+
+                print('Removing Watched Items From Trakt Watchlist Complete')
+            else:
+                print('No Watched Items To Remove From Trakt Watchlist')
+
+            # Remove Watched Items TMDB Watchlist
+            if tmdb_watchlist_items_to_remove:
+                print('Removing Watched Items From TMDB Watchlist')
+                
+                # Fetch Account ID
+                response = EH.make_tmdb_request('https://api.themoviedb.org/3/account')
+                json_data = json.loads(response.text)
+                account_id = json_data['id']
+                
+                # Count the total number of items
+                num_items = len(tmdb_watchlist_items_to_remove)
+                item_count = 0
+                
+                for item in tmdb_watchlist_items_to_remove:
+                    item_count += 1
+                    payload = {}  # Add any additional payload parameters if required
+                    if item['Type'] == 'movie':
+                        url = f"https://api.themoviedb.org/3/account/{account_id}/watchlist"
+                        payload['media_type'] = "movie"
+                        payload['media_id'] = item['TMDB_ID']
+                        payload['watchlist'] = False  # Set watchlist to False to remove the item
+                        response = EH.make_tmdb_request(url, payload=payload)
 
-            print('Setting Trakt Ratings Complete')
-        else:
-            print('No Trakt Ratings To Set')
+                    elif item['Type'] == 'show':
+                        url = f"https://api.themoviedb.org/3/account/{account_id}/watchlist"
+                        payload['media_type'] = "tv"
+                        payload['media_id'] = item['TMDB_ID']
+                        payload['watchlist'] = False  # Set watchlist to False to remove the item
+                        response = EH.make_tmdb_request(url, payload=payload)
+                    
+                    if response:
+                        print(f"Removing item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from TMDB Watchlist")
+                    else:
+                        print(f"Failed to remove item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from TMDB Watchlist (TMDB ID: {item['TMDB_ID']})")
 
+                
+                print('Removing Watched Items From TMDB Watchlist Complete')
+            else:
+                print('No Watched Items To Remove From TMDB Watchlist')
+        
     except Exception as e:
         error_message = "An error occurred while running the script."
         EH.report_error(error_message)
 
 if __name__ == '__main__':
     main()
```

### Comparing `TMDBTraktSyncer-1.2.0/TMDBTraktSyncer/authTrakt.py` & `TMDBTraktSyncer-1.3.0/TMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.2.0/TMDBTraktSyncer/errorHandling.py` & `TMDBTraktSyncer-1.3.0/TMDBTraktSyncer/errorHandling.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 import traceback
 import requests
 import time
 try:
-    from TMDBTraktSyncer import verifyCredentials
+    from TMDBTraktSyncer import verifyCredentials as VC
 except ImportError:
-    import verifyCredentials
+    import verifyCredentials as VC
 
 def report_error(error_message):
     github_issue_url = "https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/new?template=bug_report.yml"
     traceback_info = traceback.format_exc()
 
     print("\n--- ERROR ---")
     print(error_message)
     print("Please submit the error to GitHub with the following information:")
     print("-" * 50)
     print(traceback_info)
     print("-" * 50)
     print(f"Submit the error here: {github_issue_url}")
     print("-" * 50)
 
-def make_trakt_request(url, headers=None, payload=None, max_retries=3):
+def make_trakt_request(url, headers=None, params=None, payload=None, max_retries=3):
     if headers is None:
         headers = {
             'Content-Type': 'application/json',
             'trakt-api-version': '2',
-            'trakt-api-key': verifyCredentials.trakt_client_id,
-            'Authorization': f'Bearer {verifyCredentials.trakt_access_token}'
+            'trakt-api-key': VC.trakt_client_id,
+            'Authorization': f'Bearer {VC.trakt_access_token}'
         }
 
     retry_delay = 5  # seconds between retries
     retry_attempts = 0
 
     while retry_attempts < max_retries:
         response = None
         try:
             if payload is None:
-                response = requests.get(url, headers=headers)
+                if params:
+                    response = requests.get(url, headers=headers, params=params)
+                else:
+                    response = requests.get(url, headers=headers)
             else:
                 response = requests.post(url, headers=headers, json=payload)
 
             if response.status_code in [200, 201, 204]:
                 return response  # Request succeeded, return response
             elif response.status_code in [429, 500, 502, 503, 504, 520, 521, 522]:
                 # Server overloaded or rate limit exceeded, retry after delay
@@ -87,15 +90,15 @@
 
     return error_messages.get(status_code, "Unknown error")
 
 def make_tmdb_request(url, headers=None, payload=None, max_retries=3):
     if headers is None:
         headers = {
             'Content-Type': 'application/json',
-            'Authorization': f'Bearer {verifyCredentials.tmdb_v4_token}'
+            'Authorization': f'Bearer {VC.tmdb_v4_token}'
         }
 
     retry_delay = 5  # seconds between retries
     retry_attempts = 0
 
     while retry_attempts < max_retries:
         response = None
```

### Comparing `TMDBTraktSyncer-1.2.0/TMDBTraktSyncer/tmdbData.py` & `TMDBTraktSyncer-1.3.0/TMDBTraktSyncer/tmdbData.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,29 +28,29 @@
     total_pages = 1
 
     while page <= total_pages:
         url = f'https://api.themoviedb.org/3/account/{account_id}/watchlist/movies?page={page}'
         results, total_pages, _ = fetch_data(url)
         
         for movie in results:
-            movie_watchlist.append({'Title': movie['title'], 'Year': movie['release_date'][:4], 'ID': movie['id'], 'Type': 'movie'})
+            movie_watchlist.append({'Title': movie['title'], 'Year': movie['release_date'][:4], 'TMDB_ID': movie['id'], 'Type': 'movie'})
         
         page += 1
 
     # Fetch TV Show Watchlist
     show_watchlist = []
     page = 1
     total_pages = 1
 
     while page <= total_pages:
         url = f'https://api.themoviedb.org/3/account/{account_id}/watchlist/tv?page={page}'
         results, total_pages, _ = fetch_data(url)
         
         for show in results:
-            show_watchlist.append({'Title': show['name'], 'Year': show['first_air_date'][:4], 'ID': show['id'], 'Type': 'show'})
+            show_watchlist.append({'Title': show['name'], 'Year': show['first_air_date'][:4], 'TMDB_ID': show['id'], 'Type': 'show'})
         
         page += 1
 
     tmdb_watchlist = movie_watchlist + show_watchlist
 
     # Fetch Movie Ratings
     movie_ratings = []
@@ -58,29 +58,29 @@
     total_pages = 1
 
     while page <= total_pages:
         url = f'https://api.themoviedb.org/3/account/{account_id}/rated/movies?page={page}'
         results, total_pages, _ = fetch_data(url)
         
         for movie in results:
-            movie_ratings.append({'Title': movie['title'], 'Year': movie['release_date'][:4], 'Rating': movie['rating'], 'ID': movie['id'], 'Type': 'movie'})
+            movie_ratings.append({'Title': movie['title'], 'Year': movie['release_date'][:4], 'Rating': movie['rating'], 'TMDB_ID': movie['id'], 'Type': 'movie'})
         
         page += 1
 
     # Fetch TV Show Ratings
     show_ratings = []
     page = 1
     total_pages = 1
 
     while page <= total_pages:
         url = f'https://api.themoviedb.org/3/account/{account_id}/rated/tv?page={page}'
         results, total_pages, _ = fetch_data(url)
         
         for show in results:
-            show_ratings.append({'Title': show['name'], 'Year': show['first_air_date'][:4], 'Rating': show['rating'], 'ID': show['id'], 'Type': 'show'})
+            show_ratings.append({'Title': show['name'], 'Year': show['first_air_date'][:4], 'Rating': show['rating'], 'TMDB_ID': show['id'], 'Type': 'show'})
         
         page += 1
 
     # Fetch Episode Ratings
     episode_ratings = []
     page = 1
     total_pages = 1
@@ -95,15 +95,15 @@
             show_info = json.loads(response.text)
             show_name = show_info.get('name', 'Show Name Not Found')
             episode_title = f"{show_name}: {episode.get('name', 'Episode Name Not Found')}"
             episode_ratings.append({
                 'Title': episode_title,
                 'Year': episode.get('air_date', '')[:4],
                 'Rating': episode.get('rating'),
-                'ID': episode.get('id'),
+                'TMDB_ID': episode.get('id'),
                 'Season': episode.get('season_number'),
                 'Episode': episode.get('episode_number'),
                 'ShowID': show_id,
                 'Type': 'episode'
             })
             
             page += 1
```

### Comparing `TMDBTraktSyncer-1.2.0/TMDBTraktSyncer.egg-info/PKG-INFO` & `TMDBTraktSyncer-1.3.0/TMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.2.0
-Summary: This python script syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.
+Version: 1.3.0
+Summary: A python script that syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # TMDB-Trakt-Syncer
 
-This Python script syncs user watchlist and ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Data already set will not be overwritten. Ratings are synced by default and watchlist sync is optional. The user will be prompted to enter their preferences and api keys on first run. 
+This Python script syncs user watchlist and ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Data already set will not be overwritten. Ratings and watchlist sync are both optional. The user will be prompted to enter their settings and api keys on first run.
 
 The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/TMDB-Trakt-Syncer#other-recommended-projects).
 
 ## Installation Instructions:
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
 2. Install the script by running `python -m pip install TMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDbTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
    - Type of use: `Personal`
    - Application name: `TMDB-Trakt-Sync`
    - Application URL: `https://github.com/RileyXX/TMDB-Trakt-Syncer`
    - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms.`
    - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
 5. Run the script by running `TMDBTraktSyncer` in the command line.
-6. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
+6. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
 7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
 
 ## Installing the Script:
 ```
 python -m pip install TMDBTraktSyncer
 ```
 _Run in your operating system's native command line._
@@ -64,19 +64,19 @@
 ## Alternative Manual Installation Method (without pip install):
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
 2. Download the latest .zip from the [releases page](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) and extract it to the desired directory.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
    - Type of use: `Personal`
    - Application name: `TMDB-Trakt-Sync`
-   - Application URL: `localhost`
-   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms. https://github.com/RileyXX/TMDB-Trakt-Syncer`
+   - Application URL: `https://github.com/RileyXX/TMDB-Trakt-Syncer`
+   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms.`
    - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
 5. Run `TMDBTraktSyncer.py` or open the terminal and navigate to the folder where `TMDBTraktSyncer.py` is located, then run `TMDBTraktSyncer.py` in the terminal.
-6. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
+6. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
 7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
 
 ## For Setting Up Automation See the Following Wiki Pages:
 - Setup Automation for:
    - [Windows](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
    - [Linux](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
    - [macOS](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
```

### Comparing `TMDBTraktSyncer-1.2.0/setup.py` & `TMDBTraktSyncer-1.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import os
 
 #To create package: python setup.py sdist bdist_wheel
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
+with codecs.open(os.path.join(here, "README.md"), 'r', encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.2.0'
-DESCRIPTION = 'This python script syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.'
+VERSION = '1.3.0'
+DESCRIPTION = 'A python script that syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.'
 
 # Setting up
 setup(
     name="TMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
     description=DESCRIPTION,
```

