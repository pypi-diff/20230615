# Comparing `tmp/reddit_user_to_sqlite-0.3.1.tar.gz` & `tmp/reddit_user_to_sqlite-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit_user_to_sqlite-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "reddit_user_to_sqlite-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `reddit_user_to_sqlite-0.3.1.tar` & `reddit_user_to_sqlite-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-05-01 03:22:25.344837 reddit_user_to_sqlite-0.3.1/LICENSE
--rw-r--r--   0        0        0     6057 2023-05-24 04:19:17.358399 reddit_user_to_sqlite-0.3.1/README.md
--rw-r--r--   0        0        0     1298 2023-06-09 17:16:17.064762 reddit_user_to_sqlite-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-01 03:19:48.457234 reddit_user_to_sqlite-0.3.1/reddit_user_to_sqlite/__init__.py
--rw-r--r--   0        0        0     4503 2023-05-24 04:15:46.246173 reddit_user_to_sqlite-0.3.1/reddit_user_to_sqlite/cli.py
--rw-r--r--   0        0        0     1365 2023-05-23 19:13:25.850919 reddit_user_to_sqlite-0.3.1/reddit_user_to_sqlite/csv_helpers.py
--rw-r--r--   0        0        0     1097 2023-05-24 04:09:07.506319 reddit_user_to_sqlite-0.3.1/reddit_user_to_sqlite/helpers.py
--rw-r--r--   0        0        0     4621 2023-06-09 17:15:42.160717 reddit_user_to_sqlite-0.3.1/reddit_user_to_sqlite/reddit_api.py
--rw-r--r--   0        0        0     5566 2023-05-24 04:16:03.274343 reddit_user_to_sqlite-0.3.1/reddit_user_to_sqlite/sqlite_helpers.py
--rw-r--r--   0        0        0     7369 1970-01-01 00:00:00.000000 reddit_user_to_sqlite-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-01 03:22:25.344837 reddit_user_to_sqlite-0.4.0/LICENSE
+-rw-r--r--   0        0        0     7209 2023-06-15 05:47:17.749668 reddit_user_to_sqlite-0.4.0/README.md
+-rw-r--r--   0        0        0     1365 2023-06-15 05:47:08.122458 reddit_user_to_sqlite-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-01 03:19:48.457234 reddit_user_to_sqlite-0.4.0/reddit_user_to_sqlite/__init__.py
+-rw-r--r--   0        0        0     5914 2023-06-15 05:43:06.259931 reddit_user_to_sqlite-0.4.0/reddit_user_to_sqlite/cli.py
+-rw-r--r--   0        0        0     1727 2023-06-15 05:44:28.477049 reddit_user_to_sqlite-0.4.0/reddit_user_to_sqlite/csv_helpers.py
+-rw-r--r--   0        0        0     1110 2023-06-15 05:44:28.477262 reddit_user_to_sqlite-0.4.0/reddit_user_to_sqlite/helpers.py
+-rw-r--r--   0        0        0     4760 2023-06-15 05:44:28.477491 reddit_user_to_sqlite-0.4.0/reddit_user_to_sqlite/reddit_api.py
+-rw-r--r--   0        0        0     6222 2023-06-15 05:44:28.477747 reddit_user_to_sqlite-0.4.0/reddit_user_to_sqlite/sqlite_helpers.py
+-rw-r--r--   0        0        0     8587 1970-01-01 00:00:00.000000 reddit_user_to_sqlite-0.4.0/PKG-INFO
```

### Comparing `reddit_user_to_sqlite-0.3.1/LICENSE` & `reddit_user_to_sqlite-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reddit_user_to_sqlite-0.3.1/README.md` & `reddit_user_to_sqlite-0.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
 #### Params
 
 > Note: the argument order is reversed from most dogsheep packages (which take db_path first). This method allows for use of a default db name, so I prefer it.
 
 1. `archive_path`: the path to the (unzipped) archive directory on your machine. Don't rename/move the files that Reddit gives you.
 2. (optional) `--db`: the path to a sqlite file, which will be created or updated as needed. Defaults to `reddit.db`.
+3. (optional) `--skip-saved`: a flag for skipping the inclusion of loading saved comments/posts from the archive.
 
 ## Viewing Data
 
 The resulting SQLite database pairs well with [Datasette](https://datasette.io/), a tool for viewing SQLite in the web. Below is my recommended configuration.
 
 First, install `datasette`:
 
@@ -111,20 +112,39 @@
 
 ## Motivation
 
 I got nervous when I saw Reddit's [notification of upcoming API changes](https://old.reddit.com/r/reddit/comments/12qwagm/an_update_regarding_reddits_api/). To ensure I could always access data I created, I wanted to make sure I had a backup in place before anything changed in a big way.
 
 ## FAQs
 
-### Why do some of my posts say `[removed]` even though I can see them?
+### Why does this post only show 1k recent comments / posts?
+
+Reddit's paging API only shows 1000 items (page 11 is an empty list). If you have more comments (or posts) than than that, you can use the [GDPR archive import feature](#archive) feature to backfill your older data.
+
+### Why are my longer posts truncated in Datasette?
+
+Datasette truncates long text fields by default. You can disable this behavior by using the `truncate_cells_html` flag when running `datasette` ([see the docs](https://docs.datasette.io/en/stable/settings.html#truncate-cells-html)):
+
+```shell
+datasette reddit.db --setting truncate_cells_html 0
+```
+
+### How do I store a username that starts with `-`?
+
+By default, [click](https://click.palletsprojects.com/en/8.1.x/) (the argument parser this uses) interprets leading dashes on argument as a flag. If you're fetching data for user `-asdf`, you'll get an error saying `Error: No such option: -a`. To ensure the last argument is interpreted positionally, put it after a `--`:
+
+```shell
+reddit-user-to-sqlite user -- -asdf
+```
+
+### Why do some of my posts say `[removed]` even though I can see them on the web?
 
 If a post is removed, only the mods and the user who posted it can see its text. Since this tool currently runs without any authentication, those removed posts can't be fetched via the API.
 
-To fetch data about your own removed posts, use the GDPR archive import
-This will be fixed in a future release, either by:
+To load data about your own removed posts, use the [GDPR archive import feature](#archive).
 
 ### Why is the database missing data returned by the Reddit API?
 
 While most [Dogsheep](https://github.com/dogsheep) projects grab the raw JSON output of their source APIs, Reddit's API has a lot of junk in it. So, I opted for a slimmed down approach.
 
 If there's a field missing that you think would be useful, feel free to open an issue!
 
@@ -152,14 +172,14 @@
 
 In your virtual environment, a simple `pytest` should run the unit test suite. You can also run `pyright` for type checking.
 
 ### Releasing New Versions
 
 > these notes are mostly for myself (or other contributors)
 
-0. ensure tests pass (`pytest`)
+0. ensure tests pass (`tox -p`)
 1. install release tooling (`pip install -e '.[release]'`)
 2. build the package (`python -m build`)
 3. upload the release (`python -m twine upload dist/*`)
    1. give your username as `__token__`
    2. give your password as your stored API key
    3. If you're getting invalid password, verify that `~/.pypirc` is empty
```

### Comparing `reddit_user_to_sqlite-0.3.1/pyproject.toml` & `reddit_user_to_sqlite-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "reddit-user-to-sqlite"
-version = "0.3.1"
+version = "0.4.0"
 
 authors = [{ name = "David Brownman", email = "beamneocube@gmail.com" }]
 description = "Create a SQLite database containing data pulled from Reddit about a single user."
 readme = "README.md"
 license = { file = "LICENSE" }
 
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 classifiers = [
   "Programming Language :: Python :: 3",
   "Development Status :: 3 - Alpha",
   "Environment :: Console",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Natural Language :: English",
@@ -19,26 +19,29 @@
 keywords = ["sqlite", "reddit", "dogsheep"]
 
 dependencies = [
   "sqlite-utils==3.32.1",
   "click==8.1.3",
   "requests==2.29.0",
   "tqdm==4.65.0",
-  "typing_extensions==4.6.3",
 ]
 
 [project.optional-dependencies]
-test = ["pytest==7.3.1", "responses==0.23.1", "pyright==1.1.309"]
+test = ["pytest==7.3.1", "responses==0.23.1"]
 release = ["twine==4.0.2", "build==0.10.0"]
+ci = ["black==23.3.0", "isort==5.12.0", "pyright==1.1.309"]
 
 [project.urls]
 "Homepage" = "https://github.com/xavdid/reddit-user-to-sqlite"
 "Bug Tracker" = "https://github.com/xavdid/reddit-user-to-sqlite/issues"
 "Author" = "https://xavd.id"
 "Changelog" = "https://github.com/xavdid/reddit-user-to-sqlite/blob/main/CHANGELOG.md"
 
 [project.scripts]
 reddit-user-to-sqlite = "reddit_user_to_sqlite.cli:cli"
 
 [build-system]
 requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
+
+# needed so the LSP performs typechecking
+[tool.pyright]
```

### Comparing `reddit_user_to_sqlite-0.3.1/reddit_user_to_sqlite/csv_helpers.py` & `reddit_user_to_sqlite-0.4.0/reddit_user_to_sqlite/csv_helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,56 @@
 from csv import DictReader
 from pathlib import Path
-from typing import Literal
+from typing import Literal, Optional
 
 from sqlite_utils import Database
 
 ItemType = Literal["comments", "posts"]
-PREFIX: dict[ItemType, str] = {"comments": "t1", "posts": "t3"}
+PrefixType = Literal["saved_"]
+
+FULLNAME_PREFIX: dict[ItemType, str] = {
+    "comments": "t1",
+    "posts": "t3",
+}
+
+
+def build_table_name(
+    table_name: ItemType, table_prefix: Optional[PrefixType] = None
+) -> str:
+    return f"{table_prefix or ''}{table_name}"
 
 
 def validate_and_build_path(archive_path: Path, item_type: str) -> Path:
     filename = f"{item_type}.csv"
     if not (file := archive_path / filename).exists():
         raise ValueError(
-            f'Ensure path "{archive_path}" points to an unzipped Reddit GDPR archive folder; {filename} not found in the expected spot.'
+            f'Ensure path "{archive_path}" points to an unzipped Reddit GDPR archive folder; "{filename}" not found in the expected spot.'
         )
     return file
 
 
-def load_ids_from_file(
-    db: Database, archive_path: Path, item_type: ItemType
+def load_unsaved_ids_from_file(
+    db: Database,
+    archive_path: Path,
+    item_type: ItemType,
+    prefix: Optional[PrefixType] = None,
 ) -> list[str]:
-    saved_ids = {row["id"] for row in db[item_type].rows}
+    filename = build_table_name(item_type, prefix)
+    # we save each file into a matching table
+    saved_ids = {row["id"] for row in db[filename].rows}
 
-    with open(validate_and_build_path(archive_path, item_type)) as comment_archive_rows:
+    with open(validate_and_build_path(archive_path, filename)) as archive_rows:
         return [
-            f'{PREFIX[item_type]}_{c["id"]}'
-            for c in DictReader(comment_archive_rows)
+            f'{FULLNAME_PREFIX[item_type]}_{c["id"]}'
+            for c in DictReader(archive_rows)
             if c["id"] not in saved_ids
         ]
 
 
-def get_username_from_archive(archive_path: Path) -> str | None:
+def get_username_from_archive(archive_path: Path) -> Optional[str]:
     with open(validate_and_build_path(archive_path, "statistics")) as stat_rows:
         try:
             return next(
                 row["value"]
                 for row in DictReader(stat_rows)
                 if row["statistic"] == "account name"
             )
```

### Comparing `reddit_user_to_sqlite-0.3.1/reddit_user_to_sqlite/helpers.py` & `reddit_user_to_sqlite-0.4.0/reddit_user_to_sqlite/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 from itertools import islice
-from typing import Iterable, TypeVar
+from typing import Iterable, Optional, TypeVar
 
 T = TypeVar("T")
 
 
 # https://docs.python.org/3.11/library/itertools.html#itertools-recipes
 # available natively in 3.12
 def batched(iterable: Iterable[T], n: int) -> Iterable[tuple[T]]:
@@ -22,15 +22,15 @@
     strips the leading `/u/` off the front of a username, if present
     """
     if re.match(r"/?u/", username):
         return username.strip().strip("/u")
     return username
 
 
-def find_user_details_from_items(items) -> tuple[str, str] | None:
+def find_user_details_from_items(items) -> Optional[tuple[str, str]]:
     """
     Returns a 2-tuple of prefixed user_id and username if found, otherwise None
     """
     try:
         return next(
             (c["author"], c["author_fullname"]) for c in items if "author_fullname" in c
         )
```

### Comparing `reddit_user_to_sqlite-0.3.1/reddit_user_to_sqlite/reddit_api.py` & `reddit_user_to_sqlite-0.4.0/reddit_user_to_sqlite/reddit_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,24 @@
-from typing_extensions import NotRequired
+import os
 from typing import (
+    TYPE_CHECKING,
     Any,
     Literal,
     Optional,
     Sequence,
     TypedDict,
     TypeVar,
+    Union,
     cast,
     final,
 )
 
+if TYPE_CHECKING:
+    from typing import NotRequired
+
 import requests
 from tqdm import tqdm, trange
 
 from reddit_user_to_sqlite.helpers import batched
 
 USER_AGENT = "reddit-to-sqlite"
 
@@ -28,15 +33,15 @@
     subreddit_type: str
 
 
 class UserFragment(TypedDict):
     # comment author username
     author: str
     # comment author prefixed id
-    author_fullname: NotRequired[str]
+    author_fullname: "NotRequired[str]"
 
 
 class Comment(SubredditFragment, UserFragment):
     # this is only the relevant fields from the response
 
     ## COMMENT
     # short ID
@@ -101,15 +106,15 @@
 # class Subreddit(TypedDict):
 #     should_archive_posts: bool
 
 
 @final
 class ResourceWrapper(TypedDict):
     kind: str
-    data: Comment | Post
+    data: Union[Comment, Post]
 
 
 @final
 class ResponseBody(TypedDict):
     before: Optional[str]
     after: Optional[str]
     modhash: str
@@ -137,15 +142,17 @@
 def _raise_reddit_error(response):
     if "error" in response:
         raise ValueError(
             f'Received API error from Reddit (code {response["error"]}): {response["message"]}'
         )
 
 
-def _call_reddit_api(url: str, params: dict[str, Any] | None = None) -> SuccessResponse:
+def _call_reddit_api(
+    url: str, params: Optional[dict[str, Any]] = None
+) -> SuccessResponse:
     response = requests.get(
         url,
         {"limit": PAGE_SIZE, "raw_json": 1, **(params or {})},
         headers={"user-agent": USER_AGENT},
     ).json()
 
     _raise_reddit_error(response)
@@ -175,18 +182,20 @@
     return _load_paged_resource("comments", username)
 
 
 def load_posts_for_user(username: str) -> list[Post]:
     return _load_paged_resource("submitted", username)
 
 
-def load_info(resources: Sequence[str]) -> list[Comment | Post]:
+def load_info(resources: Sequence[str]) -> list[Union[Comment, Post]]:
     result = []
 
-    for batch in batched(tqdm(resources), PAGE_SIZE):
+    for batch in batched(
+        tqdm(resources, disable=bool(os.environ.get("DISABLE_PROGRESS"))), PAGE_SIZE
+    ):
         response = _call_reddit_api(
             "https://www.reddit.com/api/info.json", params={"id": ",".join(batch)}
         )
         result += [c["data"] for c in response["data"]["children"]]
 
     return result
```

### Comparing `reddit_user_to_sqlite-0.3.1/PKG-INFO` & `reddit_user_to_sqlite-0.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: reddit-user-to-sqlite
-Version: 0.3.1
+Version: 0.4.0
 Summary: Create a SQLite database containing data pulled from Reddit about a single user.
 Keywords: sqlite,reddit,dogsheep
 Author-email: David Brownman <beamneocube@gmail.com>
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Requires-Dist: sqlite-utils==3.32.1
 Requires-Dist: click==8.1.3
 Requires-Dist: requests==2.29.0
 Requires-Dist: tqdm==4.65.0
-Requires-Dist: typing_extensions==4.6.3
+Requires-Dist: black==23.3.0 ; extra == "ci"
+Requires-Dist: isort==5.12.0 ; extra == "ci"
+Requires-Dist: pyright==1.1.309 ; extra == "ci"
 Requires-Dist: twine==4.0.2 ; extra == "release"
 Requires-Dist: build==0.10.0 ; extra == "release"
 Requires-Dist: pytest==7.3.1 ; extra == "test"
 Requires-Dist: responses==0.23.1 ; extra == "test"
-Requires-Dist: pyright==1.1.309 ; extra == "test"
 Project-URL: Author, https://xavd.id
 Project-URL: Bug Tracker, https://github.com/xavdid/reddit-user-to-sqlite/issues
 Project-URL: Changelog, https://github.com/xavdid/reddit-user-to-sqlite/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://github.com/xavdid/reddit-user-to-sqlite
+Provides-Extra: ci
 Provides-Extra: release
 Provides-Extra: test
 
 # reddit-user-to-sqlite
 
 Stores all the content from a specific user in a SQLite database. This includes their comments and their posts.
 
@@ -69,14 +71,15 @@
 
 #### Params
 
 > Note: the argument order is reversed from most dogsheep packages (which take db_path first). This method allows for use of a default db name, so I prefer it.
 
 1. `archive_path`: the path to the (unzipped) archive directory on your machine. Don't rename/move the files that Reddit gives you.
 2. (optional) `--db`: the path to a sqlite file, which will be created or updated as needed. Defaults to `reddit.db`.
+3. (optional) `--skip-saved`: a flag for skipping the inclusion of loading saved comments/posts from the archive.
 
 ## Viewing Data
 
 The resulting SQLite database pairs well with [Datasette](https://datasette.io/), a tool for viewing SQLite in the web. Below is my recommended configuration.
 
 First, install `datasette`:
 
@@ -142,20 +145,39 @@
 
 ## Motivation
 
 I got nervous when I saw Reddit's [notification of upcoming API changes](https://old.reddit.com/r/reddit/comments/12qwagm/an_update_regarding_reddits_api/). To ensure I could always access data I created, I wanted to make sure I had a backup in place before anything changed in a big way.
 
 ## FAQs
 
-### Why do some of my posts say `[removed]` even though I can see them?
+### Why does this post only show 1k recent comments / posts?
+
+Reddit's paging API only shows 1000 items (page 11 is an empty list). If you have more comments (or posts) than than that, you can use the [GDPR archive import feature](#archive) feature to backfill your older data.
+
+### Why are my longer posts truncated in Datasette?
+
+Datasette truncates long text fields by default. You can disable this behavior by using the `truncate_cells_html` flag when running `datasette` ([see the docs](https://docs.datasette.io/en/stable/settings.html#truncate-cells-html)):
+
+```shell
+datasette reddit.db --setting truncate_cells_html 0
+```
+
+### How do I store a username that starts with `-`?
+
+By default, [click](https://click.palletsprojects.com/en/8.1.x/) (the argument parser this uses) interprets leading dashes on argument as a flag. If you're fetching data for user `-asdf`, you'll get an error saying `Error: No such option: -a`. To ensure the last argument is interpreted positionally, put it after a `--`:
+
+```shell
+reddit-user-to-sqlite user -- -asdf
+```
+
+### Why do some of my posts say `[removed]` even though I can see them on the web?
 
 If a post is removed, only the mods and the user who posted it can see its text. Since this tool currently runs without any authentication, those removed posts can't be fetched via the API.
 
-To fetch data about your own removed posts, use the GDPR archive import
-This will be fixed in a future release, either by:
+To load data about your own removed posts, use the [GDPR archive import feature](#archive).
 
 ### Why is the database missing data returned by the Reddit API?
 
 While most [Dogsheep](https://github.com/dogsheep) projects grab the raw JSON output of their source APIs, Reddit's API has a lot of junk in it. So, I opted for a slimmed down approach.
 
 If there's a field missing that you think would be useful, feel free to open an issue!
 
@@ -183,15 +205,15 @@
 
 In your virtual environment, a simple `pytest` should run the unit test suite. You can also run `pyright` for type checking.
 
 ### Releasing New Versions
 
 > these notes are mostly for myself (or other contributors)
 
-0. ensure tests pass (`pytest`)
+0. ensure tests pass (`tox -p`)
 1. install release tooling (`pip install -e '.[release]'`)
 2. build the package (`python -m build`)
 3. upload the release (`python -m twine upload dist/*`)
    1. give your username as `__token__`
    2. give your password as your stored API key
    3. If you're getting invalid password, verify that `~/.pypirc` is empty
```

