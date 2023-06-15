# Comparing `tmp/IMDBTraktSyncer-1.3.9.tar.gz` & `tmp/IMDBTraktSyncer-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.3.9.tar", last modified: Mon Jun  5 07:56:20 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.4.0.tar", last modified: Thu Jun 15 16:35:22 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.3.9.tar` & `IMDBTraktSyncer-1.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 07:56:20.648797 IMDBTraktSyncer-1.3.9/
-drwxrwxrwx   0        0        0        0 2023-06-05 07:56:20.627798 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    23158 2023-06-05 07:55:19.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     4440 2023-05-28 13:20:16.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4209 2023-06-05 07:44:01.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     3858 2023-06-02 06:09:12.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     7844 2023-05-29 23:40:21.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0     5841 2023-05-23 23:18:31.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0     6982 2023-05-28 12:08:00.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-06-05 07:56:20.646798 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0    12090 2023-06-05 07:56:20.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2023-06-05 07:56:20.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 07:56:20.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-06-05 07:56:20.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-06-05 07:56:20.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-05 07:56:20.000000 IMDBTraktSyncer-1.3.9/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.3.9/LICENSE
--rw-rw-rw-   0        0        0    12090 2023-06-05 07:56:20.647797 IMDBTraktSyncer-1.3.9/PKG-INFO
--rw-rw-rw-   0        0        0    11346 2023-06-05 07:47:27.000000 IMDBTraktSyncer-1.3.9/README.md
--rw-rw-rw-   0        0        0       42 2023-06-05 07:56:20.648797 IMDBTraktSyncer-1.3.9/setup.cfg
--rw-rw-rw-   0        0        0     1370 2023-06-05 07:56:14.000000 IMDBTraktSyncer-1.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 16:35:22.982344 IMDBTraktSyncer-1.4.0/
+drwxrwxrwx   0        0        0        0 2023-06-15 16:35:22.949346 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    30500 2023-06-15 15:31:26.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     4440 2023-05-28 13:20:16.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4209 2023-06-05 07:44:01.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     3858 2023-06-02 06:09:12.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     8169 2023-06-15 15:55:40.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0    10272 2023-06-15 14:00:20.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0    11171 2023-06-15 16:19:15.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-06-15 16:35:22.979354 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    12090 2023-06-15 16:35:22.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      518 2023-06-15 16:35:22.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 16:35:22.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-06-15 16:35:22.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-06-15 16:35:22.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-15 16:35:22.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0    12090 2023-06-15 16:35:22.981345 IMDBTraktSyncer-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11344 2023-06-15 16:29:38.000000 IMDBTraktSyncer-1.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-15 16:35:22.982344 IMDBTraktSyncer-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1377 2023-06-15 15:51:23.000000 IMDBTraktSyncer-1.4.0/setup.py
```

### Comparing `IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/IMDBTraktSyncer.py` & `IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files 21% similar despite different names*

```diff
@@ -102,57 +102,68 @@
             print("\nPossible IMDB captcha check or IMDB login incorrect.")
             print("\nIf your login is correct then an IMDB captcha check likely the cause of this error. To fix this, simply login to the IMDB website in your browser, preferably Chrome, and from the same computer. If logged in, log out and log back in. It may ask you to fill in a captcha; complete it and finish logging in. After logging in successfully on your browser, run the script again and it should work. You may need to repeat this step once or twice if it still gives you issues.")
             print("\nIf your IMDB login is incorrect, simply edit the credentials.txt file with the correct login or delete the credentials file and run the script again.")
             print("\nSee this GitHub link for more details: https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/2")
             print("\nStopping script...")
             raise SystemExit
         
-        trakt_watchlist, trakt_ratings, trakt_reviews = traktData.getTraktData()
+        trakt_watchlist, trakt_ratings, trakt_reviews, watched_content = traktData.getTraktData()
         imdb_watchlist, imdb_ratings, imdb_reviews, errors_found_getting_imdb_reviews = imdbData.getImdbData(imdb_username, imdb_password, driver, directory, wait)
 
-        #Get trakt and imdb data and filter out items with missing imdb id
-        trakt_ratings = [rating for rating in trakt_ratings if rating.get('ID') is not None]
-        imdb_ratings = [rating for rating in imdb_ratings if rating.get('ID') is not None]
-        trakt_reviews = [review for review in trakt_reviews if review.get('ID') is not None]
-        imdb_reviews = [review for review in imdb_reviews if review.get('ID') is not None]
-        trakt_watchlist = [item for item in trakt_watchlist if item.get('ID') is not None]
-        imdb_watchlist = [item for item in imdb_watchlist if item.get('ID') is not None]
-        #Filter out items already set
-        imdb_ratings_to_set = [rating for rating in trakt_ratings if rating['ID'] not in [imdb_rating['ID'] for imdb_rating in imdb_ratings]]
-        trakt_ratings_to_set = [rating for rating in imdb_ratings if rating['ID'] not in [trakt_rating['ID'] for trakt_rating in trakt_ratings]]
-        imdb_reviews_to_set = [review for review in trakt_reviews if review['ID'] not in [imdb_review['ID'] for imdb_review in imdb_reviews]]
-        trakt_reviews_to_set = [review for review in imdb_reviews if review['ID'] not in [trakt_review['ID'] for trakt_review in trakt_reviews]]
-        imdb_watchlist_to_set = [item for item in trakt_watchlist if item['ID'] not in [imdb_item['ID'] for imdb_item in imdb_watchlist]]
-        trakt_watchlist_to_set = [item for item in imdb_watchlist if item['ID'] not in [trakt_item['ID'] for trakt_item in trakt_watchlist]]
-        # Remove duplicate reviews and filter by out any items for imdb_reviews_to_set where comment length is less than 600 characters
-        def remove_duplicates_and_filter(lst, key, min_comment_length=None):
-            seen = set()
+        # Get trakt and imdb data and filter out items with missing imdb id
+        trakt_ratings = [rating for rating in trakt_ratings if rating.get('IMDB_ID') is not None]
+        imdb_ratings = [rating for rating in imdb_ratings if rating.get('IMDB_ID') is not None]
+        trakt_reviews = [review for review in trakt_reviews if review.get('IMDB_ID') is not None]
+        imdb_reviews = [review for review in imdb_reviews if review.get('IMDB_ID') is not None]
+        trakt_watchlist = [item for item in trakt_watchlist if item.get('IMDB_ID') is not None]
+        imdb_watchlist = [item for item in imdb_watchlist if item.get('IMDB_ID') is not None]
+        # Filter out items already set
+        imdb_ratings_to_set = [rating for rating in trakt_ratings if rating['IMDB_ID'] not in [imdb_rating['IMDB_ID'] for imdb_rating in imdb_ratings]]
+        trakt_ratings_to_set = [rating for rating in imdb_ratings if rating['IMDB_ID'] not in [trakt_rating['IMDB_ID'] for trakt_rating in trakt_ratings]]
+        imdb_reviews_to_set = [review for review in trakt_reviews if review['IMDB_ID'] not in [imdb_review['IMDB_ID'] for imdb_review in imdb_reviews]]
+        trakt_reviews_to_set = [review for review in imdb_reviews if review['IMDB_ID'] not in [trakt_review['IMDB_ID'] for trakt_review in trakt_reviews]]
+        imdb_watchlist_to_set = [item for item in trakt_watchlist if item['IMDB_ID'] not in [imdb_item['IMDB_ID'] for imdb_item in imdb_watchlist]]
+        trakt_watchlist_to_set = [item for item in imdb_watchlist if item['IMDB_ID'] not in [trakt_item['IMDB_ID'] for trakt_item in trakt_watchlist]]
+        # Filter out items where the comment length is less than 600 characters
+        def filter_by_comment_length(lst, min_comment_length=None):
             result = []
             for item in lst:
-                if item[key] not in seen and (min_comment_length is None or ('Comment' in item and len(item['Comment']) >= min_comment_length)):
-                    seen.add(item[key])
+                if min_comment_length is None or ('Comment' in item and len(item['Comment']) >= min_comment_length):
                     result.append(item)
             return result
-
-        imdb_reviews_to_set = remove_duplicates_and_filter(imdb_reviews_to_set, 'ID', 600)
-        trakt_reviews_to_set = remove_duplicates_and_filter(trakt_reviews_to_set, 'ID')
+        imdb_reviews_to_set = filter_by_comment_length(imdb_reviews_to_set, 600)
+        
+        # If remove_watched_from_watchlists_value is true
+        if VC.remove_watched_from_watchlists_value:        
+            # Get the IDs from watched_content
+            watched_content_ids = set(item['IMDB_ID'] for item in watched_content if item['IMDB_ID'])
+                    
+            # Filter out watched content from trakt_watchlist_to_set
+            trakt_watchlist_to_set = [item for item in trakt_watchlist_to_set if item['IMDB_ID'] not in watched_content_ids]
+            # Filter out watched content from trakt_watchlist_to_set
+            imdb_watchlist_to_set = [item for item in imdb_watchlist_to_set if item['IMDB_ID'] not in watched_content_ids]
+            
+            # Find items to remove from trakt_watchlist
+            trakt_watchlist_items_to_remove = [item for item in trakt_watchlist if item['IMDB_ID'] in watched_content_ids]
+            # Find items to remove from imdb_watchlist
+            imdb_watchlist_items_to_remove = [item for item in imdb_watchlist if item['IMDB_ID'] in watched_content_ids]
         
         # If sync_watchlist_value is true
         if VC.sync_watchlist_value:
             # Set Trakt Watchlist Items
             if trakt_watchlist_to_set:
                 print('Setting Trakt Watchlist Items')
 
                 # Count the total number of items
                 num_items = len(trakt_watchlist_to_set)
                 item_count = 0
 
                 for item in trakt_watchlist_to_set:
                     item_count += 1
-                    imdb_id = item['ID']
+                    imdb_id = item['IMDB_ID']
                     media_type = item['Type']  # 'movie', 'show', or 'episode'
 
                     url = f"https://api.trakt.tv/sync/watchlist"
 
                     data = {
                         "movies": [],
                         "shows": [],
@@ -199,29 +210,39 @@
                                 
                 for item in imdb_watchlist_to_set:
                     try:
                         item_count += 1
                         year_str = f' ({item["Year"]})' if item["Year"] is not None else '' # sometimes year is None for episodes from trakt so remove it from the print string
                         print(f"Adding item ({item_count} of {num_items}): {item['Title']}{year_str} to IMDB Watchlist")
                         
-                        driver.get(f'https://www.imdb.com/title/{item["ID"]}/')
+                        driver.get(f'https://www.imdb.com/title/{item["IMDB_ID"]}/')
                         
                         # Scroll the page to bring the element into view
                         watchlist_button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"]')))
                         driver.execute_script("arguments[0].scrollIntoView(true);", watchlist_button)
                         
                         # Wait for the element to be clickable
                         watchlist_button = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"]')))
                         
                         # Check if item is already in watchlist otherwise skip it
                         if 'ipc-icon--done' not in watchlist_button.get_attribute('innerHTML'):
-                            driver.execute_script("arguments[0].click();", watchlist_button)
-                            time.sleep(1)
+                            retry_count = 0
+                            while retry_count < 2:
+                                driver.execute_script("arguments[0].click();", watchlist_button)
+                                try:
+                                    WebDriverWait(driver, 3).until(EC.presence_of_element_located((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"] .ipc-icon--done')))
+                                    break  # Break the loop if successful
+                                except TimeoutException:
+                                    retry_count += 1
+
+                            if retry_count == 2:
+                                print(f"Failed to add item ({item_count} of {num_items}): {item['Title']}{year_str} to IMDB Watchlist ({item['IMDB_ID']})")
+                        
                     except (NoSuchElementException, TimeoutException):
-                        print(f"Failed to add item ({item_count} of {num_items}): {item['Title']}{year_str} to IMDB Watchlist ({item['ID']})")
+                        print(f"Failed to add item ({item_count} of {num_items}): {item['Title']}{year_str} to IMDB Watchlist ({item['IMDB_ID']})")
                         pass
 
                 
                 print('Setting IMDB Watchlist Items Complete')
             else:
                 print('No IMDB Watchlist Items To Set')
 
@@ -240,37 +261,37 @@
             for item in trakt_ratings_to_set:
                 item_count += 1
                 if item["Type"] == "show":
                     # This is a TV show
                     data = {
                         "shows": [{
                             "ids": {
-                                "imdb": item["ID"]
+                                "imdb": item["IMDB_ID"]
                             },
                             "rating": item["Rating"]
                         }]
                     }
                     print(f"Rating TV show ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
                 elif item["Type"] == "movie":
                     # This is a movie
                     data = {
                         "movies": [{
                             "ids": {
-                                "imdb": item["ID"]
+                                "imdb": item["IMDB_ID"]
                             },
                             "rating": item["Rating"]
                         }]
                     }
                     print(f"Rating movie ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
                 elif item["Type"] == "episode":
                     # This is an episode
                     data = {
                         "episodes": [{
                             "ids": {
-                                "imdb": item["ID"]
+                                "imdb": item["IMDB_ID"]
                             },
                             "rating": item["Rating"]
                         }]
                     }
                     print(f"Rating episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
 
                 # Make the API call to rate the item
@@ -287,15 +308,15 @@
         if imdb_ratings_to_set:
             print('Setting IMDB Ratings')
 
             # loop through each movie and TV show rating and submit rating on IMDB website
             for i, item in enumerate(imdb_ratings_to_set, 1):
                 year_str = f' ({item["Year"]})' if item["Year"] is not None else '' # sometimes year is None for episodes from trakt so remove it from the print string
                 print(f'Rating {item["Type"]}: ({i} of {len(imdb_ratings_to_set)}) {item["Title"]}{year_str}: {item["Rating"]}/10 on IMDB')
-                driver.get(f'https://www.imdb.com/title/{item["ID"]}/')
+                driver.get(f'https://www.imdb.com/title/{item["IMDB_ID"]}/')
                 
                 # Wait until rate button is located and scroll to it
                 button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, '[data-testid="hero-rating-bar__user-rating"] button.ipc-btn')))
                 driver.execute_script("arguments[0].scrollIntoView(true);", button)
 
                 # click on "Rate" button and select rating option, then submit rating
                 button = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, '[data-testid="hero-rating-bar__user-rating"] button.ipc-btn')))
@@ -305,15 +326,15 @@
                         driver.execute_script("arguments[0].click();", button)
                         rating_option_element = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, f'button[aria-label="Rate {item["Rating"]}"]')))
                         driver.execute_script("arguments[0].click();", rating_option_element)
                         submit_element = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, 'button.ipc-rating-prompt__rate-button')))
                         submit_element.click()
                         time.sleep(1)
                 except (NoSuchElementException, TimeoutException):
-                    print(f'Failed to rate {item["Type"]}: ({i} of {len(imdb_ratings_to_set)}) {item["Title"]}{year_str}: {item["Rating"]}/10 on IMDB ({item["ID"]})')
+                    print(f'Failed to rate {item["Type"]}: ({i} of {len(imdb_ratings_to_set)}) {item["Title"]}{year_str}: {item["Rating"]}/10 on IMDB ({item["IMDB_ID"]})')
                     pass
 
             print('Setting IMDB Ratings Complete')
         else:
             print('No IMDB Ratings To Set')
 
         # If sync_reviews_value is true
@@ -326,15 +347,15 @@
 
                     # Count the total number of items
                     num_items = len(trakt_reviews_to_set)
                     item_count = 0
 
                     for review in trakt_reviews_to_set:
                         item_count += 1
-                        imdb_id = review['ID']
+                        imdb_id = review['IMDB_ID']
                         comment = review['Comment']
                         media_type = review['Type']  # 'movie', 'show', or 'episode'
 
                         url = f"https://api.trakt.tv/comments"
 
                         data = {
                             "comment": comment
@@ -380,15 +401,15 @@
                         num_items = len(imdb_reviews_to_set)
                         item_count = 0
                         
                         for review in imdb_reviews_to_set:
                             item_count += 1
                             try:
                                 print(f"Submitting review ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on IMDB")
-                                driver.get(f'https://contribute.imdb.com/review/{review["ID"]}/add?bus=imdb')
+                                driver.get(f'https://contribute.imdb.com/review/{review["IMDB_ID"]}/add?bus=imdb')
                                 
                                 review_title_input = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "input.klondike-input")))
                                 review_input = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "textarea.klondike-textarea")))
                                 
                                 review_title_input.send_keys("My Review")
                                 review_input.send_keys(review["Comment"])
                                 
@@ -402,25 +423,129 @@
                                                         
                                 submit_button = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, "input.a-button-input[type='submit']")))
 
                                 submit_button.click()
                                 
                                 time.sleep(3) # wait for rating to submit
                             except (NoSuchElementException, TimeoutException):
-                                print(f"Failed to submit review ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on IMDB ({item['ID']})")
+                                print(f"Failed to submit review ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on IMDB ({item['IMDB_ID']})")
                                 pass
                         
                         print('Setting IMDB Reviews Complete')
                     else:
                         print('IMDB reviews were submitted within the last 10 days. Skipping IMDB review submission.')
                 else:
                     print('No IMDB Reviews To Set')
             else:
                 print('There was an error getting IMDB reviews. See exception. Skipping reviews submissions.')
 
+        # If remove_watched_from_watchlists_value is true
+        if VC.remove_watched_from_watchlists_value:
+            
+            # Remove Watched Items Trakt Watchlist
+            if trakt_watchlist_items_to_remove:
+                print('Removing Watched Items From Trakt Watchlist')
+
+                # Set the API endpoint
+                remove_url = "https://api.trakt.tv/sync/watchlist/remove"
+
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
+            # Remove Watched Items IMDB Watchlist
+            if imdb_watchlist_items_to_remove:
+                print('Removing Watched Items From IMDB Watchlist')
+                
+                # Count the total number of items
+                num_items = len(imdb_watchlist_items_to_remove)
+                item_count = 0
+                                
+                for item in imdb_watchlist_items_to_remove:
+                    try:
+                        item_count += 1
+                        year_str = f' ({item["Year"]})' if item["Year"] is not None else '' # sometimes year is None for episodes from trakt so remove it from the print string
+                        print(f"Removing item ({item_count} of {num_items}): {item['Title']}{year_str} from IMDB Watchlist")
+                        
+                        driver.get(f'https://www.imdb.com/title/{item["IMDB_ID"]}/')
+                        
+                        # Scroll the page to bring the element into view
+                        watchlist_button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"]')))
+                        driver.execute_script("arguments[0].scrollIntoView(true);", watchlist_button)
+                        
+                        # Wait for the element to be clickable
+                        watchlist_button = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"]')))
+                        
+                        # Check if item is not in watchlist otherwise skip it
+                        if 'ipc-icon--add' not in watchlist_button.get_attribute('innerHTML'):
+                            retry_count = 0
+                            while retry_count < 2:
+                                driver.execute_script("arguments[0].click();", watchlist_button)
+                                try:
+                                    WebDriverWait(driver, 3).until(EC.presence_of_element_located((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"] .ipc-icon--add')))
+                                    break  # Break the loop if successful
+                                except TimeoutException:
+                                    retry_count += 1
+
+                            if retry_count == 2:
+                                print(f"Failed to remove item ({item_count} of {num_items}): {item['Title']}{year_str} from IMDB Watchlist ({item['IMDB_ID']})")
+
+                    except (NoSuchElementException, TimeoutException):
+                        print(f"Failed to remove item ({item_count} of {num_items}): {item['Title']}{year_str} from IMDB Watchlist ({item['IMDB_ID']})")
+                        pass
+
+                
+                print('Removing Watched Items From IMDB Watchlist Complete')
+            else:
+                print('No Watched Items To Remove From IMDB Watchlist')
+        
         #Close web driver
         print("Closing webdriver...")
         driver.quit()
         service.stop()
     
     except Exception as e:
         error_message = "An error occurred while running the script."
```

### Comparing `IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/authTrakt.py` & `IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/errorHandling.py` & `IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.9/IMDBTraktSyncer/imdbData.py` & `IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/imdbData.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,30 +32,30 @@
 
         imdb_watchlist = []
 
         # Read the watchlist items from the CSV file
         here = os.path.abspath(os.path.dirname(__file__))
         watchlist_path = os.path.join(here, 'WATCHLIST.csv')
         try:
-            with open(watchlist_path, 'r') as file:
+            with open(watchlist_path, 'r', encoding='utf-8') as file:
                 reader = csv.reader(file)
                 header = next(reader)  # skip the header row
                 for row in reader:
                     title = row[5]
                     year = row[10]
                     imdb_id = row[1]
                     if "tvSeries" in row[7] or "tvMiniSeries" in row[7]:
                         media_type = "show"
                     elif "tvEpisode" in row[7]:
                         media_type = "episode"
                     elif "movie" in row[7]:
                         media_type = "movie"
                     else:
                         media_type = "unknown"
-                    imdb_watchlist.append({'Title': title, 'Year': year, 'ID': imdb_id, 'Type': media_type})
+                    imdb_watchlist.append({'Title': title, 'Year': year, 'IMDB_ID': imdb_id, 'Type': media_type})
         except FileNotFoundError:
             print('Ratings file not found')
             
         # Delete csv files
         for file in os.listdir(directory):
             if file.endswith('.csv') and 'WATCHLIST' in file:
                 os.remove(os.path.join(directory, file))
@@ -80,15 +80,15 @@
 
         imdb_ratings = []
 
         # Read the ratings from the CSV file
         here = os.path.abspath(os.path.dirname(__file__))
         ratings_path = os.path.join(here, 'ratings.csv')
         try:
-            with open(ratings_path, 'r') as file:
+            with open(ratings_path, 'r', encoding='utf-8') as file:
                 reader = csv.reader(file)
                 header = next(reader)  # skip the header row
                 for row in reader:
                     title = row[3]
                     year = row[8]
                     rating = row[1]
                     imdb_id = row[0]
@@ -96,15 +96,15 @@
                         media_type = "show"
                     elif "tvEpisode" in row[5]:
                         media_type = "episode"
                     elif "movie" in row[5]:
                         media_type = "movie"
                     else:
                         media_type = "unknown"
-                    imdb_ratings.append({'Title': title, 'Year': year, 'Rating': rating, 'ID': imdb_id, 'Type': media_type})
+                    imdb_ratings.append({'Title': title, 'Year': year, 'Rating': rating, 'IMDB_ID': imdb_id, 'Type': media_type})
         except FileNotFoundError:
             print('Ratings file not found')
             
         # Delete csv files
         for file in os.listdir(directory):
             if file.endswith('.csv') and 'ratings' in file:
                 os.remove(os.path.join(directory, file))
@@ -139,21 +139,21 @@
                 break
             
             for element in review_elements:
                 review = {}
                 # Extract review details
                 review['Title'] = element.find_element(By.CSS_SELECTOR, ".lister-item-header a").text
                 review['Year'] = element.find_element(By.CSS_SELECTOR, ".lister-item-header span").text.strip('()').split('–')[0].strip()
-                review['ID'] = element.find_element(By.CSS_SELECTOR, ".lister-item-header a").get_attribute("href").split('/')[4]
+                review['IMDB_ID'] = element.find_element(By.CSS_SELECTOR, ".lister-item-header a").get_attribute("href").split('/')[4]
                 review['IMDBReviewID'] = element.get_attribute("data-review-id")
                 review['Comment'] = element.find_element(By.CSS_SELECTOR, ".content > .text").text.strip()
                 spoiler_warning_elements = element.find_elements(By.CSS_SELECTOR, ".spoiler-warning")
                 review['Spoiler'] = len(spoiler_warning_elements) > 0
                 # Get the media type using Trakt API
-                media_type = get_media_type(review['ID'])
+                media_type = get_media_type(review['IMDB_ID'])
                 if media_type:
                     review['Type'] = media_type
                 else:
                     review['Type'] = 'unknown'
 
                 reviews.append(review)
 
@@ -174,12 +174,19 @@
             except (NoSuchElementException, TimeoutException):
                 break  # "Next" link not found or timed out waiting for the 'Next' link, exit the loop without error.
         except Exception as e:
             errors_found_getting_imdb_reviews = True
             print(f"Exception occurred while getting IMDB reviews: {type(e)}")
             break
 
-    imdb_reviews = reviews
+    # Filter out duplicate reviews for the same item based on ID
+    filtered_reviews = []
+    seen = set()
+    for item in reviews:
+        if item['IMDB_ID'] not in seen:
+            seen.add(item['IMDB_ID'])
+            filtered_reviews.append(item)
+    imdb_reviews = filtered_reviews
 
     print('Processing IMDB Data Complete')
     
     return imdb_watchlist, imdb_ratings, imdb_reviews, errors_found_getting_imdb_reviews
```

### Comparing `IMDBTraktSyncer-1.3.9/IMDBTraktSyncer.egg-info/PKG-INFO` & `IMDBTraktSyncer-1.4.0/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.3.9
-Summary: This python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
+Version: 1.4.0
+Summary: A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # IMDB-Trakt-Syncer
-This Python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Existing items will not be overwritten. Ratings are synced by default, watchlist and comment/review sync are optional. The user will be prompted to enter their settings and credentials on first run.
+This Python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Existing items will not be overwritten. Ratings, watchlist and comment/review sync are all optional. The user will be prompted to enter their settings and credentials on first run.
 
 The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux and Mac). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/IMDB-Trakt-Syncer#other-recommended-projects).
 
 ## Installation Instructions
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Install the script by executing `python -m pip install IMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run the script by executing `IMDBTraktSyncer` in the command line.
-5. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your IMDB username and password. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
+5. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your IMDB `username` and `password`. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
 6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
 
 ## Installing the Script:
 ```
 python -m pip install IMDBTraktSyncer
 ```
 _Run in your operating system's native command line._
@@ -55,15 +55,15 @@
 _Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/IMDB-Trakt-Syncer/releases) (e.g. 1.1.6) and run in your operating system's native command line._
 
 ## Alternative Manual Installation Method (without pip install)
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/).  _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Download the latest .zip from the [releases page](https://github.com/RileyXX/IMDB-Trakt-Syncer/releases) and extract it to the desired directory.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run `IMDBTraktSyncer.py` or open the terminal and navigate to the folder where `IMDBTraktSyncer.py` is located. Run `IMDBTraktSyncer.py` in the terminal.
-5. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your IMDB username and password. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
+5. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your IMDB `username` and `password`. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
 6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
 
 ## For Setting Up Automation See the Following Wiki Pages:
 - Setup Automation for:
    - [Windows](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
    - [Linux](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
    - [macOS](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
```

### Comparing `IMDBTraktSyncer-1.3.9/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.4.0/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.9/LICENSE` & `IMDBTraktSyncer-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.9/PKG-INFO` & `IMDBTraktSyncer-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.3.9
-Summary: This python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
+Version: 1.4.0
+Summary: A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # IMDB-Trakt-Syncer
-This Python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Existing items will not be overwritten. Ratings are synced by default, watchlist and comment/review sync are optional. The user will be prompted to enter their settings and credentials on first run.
+This Python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Existing items will not be overwritten. Ratings, watchlist and comment/review sync are all optional. The user will be prompted to enter their settings and credentials on first run.
 
 The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux and Mac). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/IMDB-Trakt-Syncer#other-recommended-projects).
 
 ## Installation Instructions
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Install the script by executing `python -m pip install IMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run the script by executing `IMDBTraktSyncer` in the command line.
-5. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your IMDB username and password. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
+5. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your IMDB `username` and `password`. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
 6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
 
 ## Installing the Script:
 ```
 python -m pip install IMDBTraktSyncer
 ```
 _Run in your operating system's native command line._
@@ -55,15 +55,15 @@
 _Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/IMDB-Trakt-Syncer/releases) (e.g. 1.1.6) and run in your operating system's native command line._
 
 ## Alternative Manual Installation Method (without pip install)
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/).  _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Download the latest .zip from the [releases page](https://github.com/RileyXX/IMDB-Trakt-Syncer/releases) and extract it to the desired directory.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run `IMDBTraktSyncer.py` or open the terminal and navigate to the folder where `IMDBTraktSyncer.py` is located. Run `IMDBTraktSyncer.py` in the terminal.
-5. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your IMDB username and password. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
+5. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your IMDB `username` and `password`. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
 6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
 
 ## For Setting Up Automation See the Following Wiki Pages:
 - Setup Automation for:
    - [Windows](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
    - [Linux](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
    - [macOS](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
```

### Comparing `IMDBTraktSyncer-1.3.9/README.md` & `IMDBTraktSyncer-1.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # IMDB-Trakt-Syncer
-This Python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Existing items will not be overwritten. Ratings are synced by default, watchlist and comment/review sync are optional. The user will be prompted to enter their settings and credentials on first run.
+This Python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Existing items will not be overwritten. Ratings, watchlist and comment/review sync are all optional. The user will be prompted to enter their settings and credentials on first run.
 
 The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux and Mac). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/IMDB-Trakt-Syncer#other-recommended-projects).
 
 ## Installation Instructions
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Install the script by executing `python -m pip install IMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run the script by executing `IMDBTraktSyncer` in the command line.
-5. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your IMDB username and password. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
+5. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your IMDB `username` and `password`. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
 6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
 
 ## Installing the Script:
 ```
 python -m pip install IMDBTraktSyncer
 ```
 _Run in your operating system's native command line._
@@ -39,15 +39,15 @@
 _Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/IMDB-Trakt-Syncer/releases) (e.g. 1.1.6) and run in your operating system's native command line._
 
 ## Alternative Manual Installation Method (without pip install)
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/).  _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Download the latest .zip from the [releases page](https://github.com/RileyXX/IMDB-Trakt-Syncer/releases) and extract it to the desired directory.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run `IMDBTraktSyncer.py` or open the terminal and navigate to the folder where `IMDBTraktSyncer.py` is located. Run `IMDBTraktSyncer.py` in the terminal.
-5. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your IMDB username and password. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
+5. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your IMDB `username` and `password`. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
 6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
 
 ## For Setting Up Automation See the Following Wiki Pages:
 - Setup Automation for:
    - [Windows](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
    - [Linux](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
    - [macOS](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
```

### Comparing `IMDBTraktSyncer-1.3.9/setup.py` & `IMDBTraktSyncer-1.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import os
 
 #To create package: python setup.py sdist bdist_wheel
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
+with codecs.open(os.path.join(here, "README.md"), 'r', encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.3.9'
-DESCRIPTION = 'This python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.'
+VERSION = '1.4.0'
+DESCRIPTION = 'A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
     description=DESCRIPTION,
```

