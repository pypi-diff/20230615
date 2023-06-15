# Comparing `tmp/tegracli-0.2.5.tar.gz` & `tmp/tegracli-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tegracli-0.2.5.tar", max compression
+gzip compressed data, was "tegracli-0.2.6.tar", max compression
```

## Comparing `tegracli-0.2.5.tar` & `tegracli-0.2.6.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1100 2022-10-24 15:55:29.200116 tegracli-0.2.5/LICENSE
--rw-r--r--   0        0        0     8456 2023-04-12 14:05:59.583449 tegracli-0.2.5/README.md
--rw-r--r--   0        0        0     1322 2023-04-21 16:51:09.726105 tegracli-0.2.5/pyproject.toml
--rw-r--r--   0        0        0       65 2023-04-11 13:51:38.330956 tegracli-0.2.5/tegracli/__init__.py
--rw-r--r--   0        0        0     5666 2023-04-21 16:50:59.142072 tegracli-0.2.5/tegracli/dispatch.py
--rw-r--r--   0        0        0     4578 2023-02-03 16:03:39.618393 tegracli-0.2.5/tegracli/group.py
--rw-r--r--   0        0        0    12773 2023-04-13 10:33:21.255171 tegracli-0.2.5/tegracli/main.py
--rw-r--r--   0        0        0      246 2023-02-03 16:03:39.618393 tegracli-0.2.5/tegracli/types.py
--rw-r--r--   0        0        0     1578 2023-03-01 08:59:14.495867 tegracli-0.2.5/tegracli/utilities.py
--rw-r--r--   0        0        0     9568 2023-04-21 16:52:27.122540 tegracli-0.2.5/setup.py
--rw-r--r--   0        0        0     9430 2023-04-21 16:52:27.123299 tegracli-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1100 2022-10-24 15:55:29.200116 tegracli-0.2.6/LICENSE
+-rw-r--r--   0        0        0    10186 2023-06-15 14:05:56.208264 tegracli-0.2.6/README.md
+-rw-r--r--   0        0        0     1344 2023-06-15 14:05:56.208264 tegracli-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0       88 2023-06-15 14:05:56.212264 tegracli-0.2.6/tegracli/__init__.py
+-rw-r--r--   0        0        0     5666 2023-04-21 16:50:59.142072 tegracli-0.2.6/tegracli/dispatch.py
+-rw-r--r--   0        0        0     4578 2023-02-03 16:03:39.618393 tegracli-0.2.6/tegracli/group.py
+-rw-r--r--   0        0        0    13930 2023-06-15 14:05:56.212264 tegracli-0.2.6/tegracli/main.py
+-rw-r--r--   0        0        0      246 2023-02-03 16:03:39.618393 tegracli-0.2.6/tegracli/types.py
+-rw-r--r--   0        0        0     1578 2023-03-01 08:59:14.495867 tegracli-0.2.6/tegracli/utilities.py
+-rw-r--r--   0        0        0    11211 1970-01-01 00:00:00.000000 tegracli-0.2.6/PKG-INFO
```

### Comparing `tegracli-0.2.5/LICENSE` & `tegracli-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tegracli-0.2.5/README.md` & `tegracli-0.2.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,108 @@
+Metadata-Version: 2.1
+Name: tegracli
+Version: 0.2.6
+Summary: A research-focused Telegram CLI application
+Home-page: https://pypi.org/project/tegracli/
+License: MIT
+Author: Philipp Kessling
+Author-email: p.kessling@leibniz-hbi.de
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: Telethon (>=1.24.0,<2.0.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: pandas (>=1.4.3,<2.0.0)
+Requires-Dist: ujson (>=5.4.0,<6.0.0)
+Project-URL: Repository, https://github.com/Leibniz-HBI/tegracli
+Description-Content-Type: text/markdown
+
 # tegracli
 
 ![The TEGRACLI logo](https://github.com/Leibniz-HBI/tegracli/blob/trunk/tegracli.png?raw=true)
 
 A convenience wrapper around Telethon and the Telegram Client API for research purposes.
 
-# Installation Instructions
+## Installation Instructions
 
 `tegracli` uses Poetry and python >= 3.9 and < 4.0 for building and installing.
 
 To install using pipx, run the following command `pipx install tegracli`.
 
-## How to get API keys
+### How to get API keys
 
 If you don't have API keys for Telegram, head over to [my.telegram.org](https://my.telegram.org).
 Click on [API development tools](https://my.telegram.org/apps), fill the form to create yourself an app and pluck the keys into `tegracli.conf.yml`. The session name can be arbitrary.
 
 ```yaml
 api_id: 1234567
 api_hash : some12321hashthatmustbehere123
 session_name: somesessionyo
 ```
 
 This template file is provided with the repository.
 
-# Usage
+## Usage
 
 `tegracli` is a terminal application to access the Telegram API for research purposes.
 In order to retrieve messages the configuration-file from the section before must be present in the directory you start `tegracli`.
 
+```text
+Usage: tegracli [OPTIONS] COMMAND [ARGS]...
+
+  Tegracli!! Retrieve messages from *Te*le*gra*m with a *CLI*!
+
+Options:
+  -d, --debug              Enable legacy debugging, is overwritten by the
+                           other options. Defaults to False.
+  -v, --verbose            Logging verbosity.
+  -l, --log-file FILENAME  File to log to. Defaults to STDOUT.
+  -s, --serialize          Serialize output to JSON.
+  --help                   Show this message and exit.
+
+Commands:
+  configure  Configure tegracli.
+  get        Get messages for the specified channels by either ID or...
+  group      Manage account groups.
+  hydrate    Hydrate a file with messages-ids.
+  search     Searches Telegram content that is available to your account.
+```
+
+## Logging
+
+`tegracli` allows for configuring what and how it is logged. Per default logging is **disabled** and can be enabled by passing `--verbose` or `-v`, logging level can be increased by more `-vvvv`s. By default logging target is `STDOUT` but this can be redirected to a file with `--log-file yourfile.log`. Setting `--serialize` allows to be to write the entire logging information in JSON-encoded form. `--debug` is the legacy option used by `tegracli` <= 0.2.5, this will set serialized logging into `tegracli.log.jsonl` at the `DEBUG` level; it is overwritten by setting the `--verbose` option.
+
+## Commands 
+
 The following commands are available:
 
-## CONFIGURE
+### configure
 
 Opens an interactive prompt for configuring API-access. Aks you to input your API id, API hash and session name and requests
 a 2FA code from Telegram.
 
 ```text
 Usage: tegracli configure [OPTIONS]
 
   Configure tegracli.
 
 Options:
   --help  Show this message and exit.
 ```
 
-## GET
+### get
 
 To _get_ messages from a number of channels, use this command.
 
 ```text
 Usage: tegracli get [OPTIONS] [CHANNELS]...
 
   Get messages for the specified channels by either ID or username.
@@ -78,15 +132,15 @@
 | **min_id**          | sets the minimum post number                                                                                                 |
 | **max_id**          | sets the maximum post number                                                                                                 |
 | **add_offset**      | add a offset to the post numbers to be retrieved                                                                             |
 | **from_user**       | limit messages to posts *from* a specific user                                                                               |
 | **reply_to**        | limit messages to replies *to* a specific user                                                                               |
 | **reverse/forward** | flag to indicate whether messages should be retrieved in chronological or reverse chronological order.                       |
 
-### Basic Examples
+#### Basic Examples
 
 To retrieve the last fifty messages from a Telegram channel:
 
 ```bash
 tegracli get --limit 50 corona_infokanal_bmg
 ```
 
@@ -102,28 +156,28 @@
 ```
 
 To retrieve message sent before January, 1st 2022:
 
 ```bash
 tegracli get --reverse --offset_date 2022-01-01 corona_infokanal_bmg
 ```
-## SEARCH
+### search
 
 To _search_ messages of your chats and groups and channels you are subscribed to, use this command.
 
 ```text
 Usage: tegracli search [OPTIONS] [QUERIES]...
 
   This function searches Telegram content that is available to your account for the specified search term(s).
 
 Options:
   --help  Show this message and exit.
 ```
 
-## HYDRATE
+### hydrate
 
 To rehydrate messages from the API this command accepts a file with message IDs in the format of `$channel_name/$post_number`.
 Both input and output file are optional, if not given, `stdin` and `stdout` are used.
 
 Output data is JSONL, one message per line.
 
 ```text
@@ -138,23 +192,21 @@
 For example, to rehydrate message IDs:
 
 ```bash
 echo test_channel/1234 | tegracli hydrate
 >> {"_":"Message","id": 1234, ... , "restriction_reason":[],"ttl_period":null}
 ```
 
-## GROUP INIT and GROUP RUN
+### groups
 
-In order to support updatable  and long-running collections `tegracli` sports an *account group* feature which retrieves
-the history of a given set of accounts and is able to retrieve updates on each of these accounts.
+In order to support updatable  and long-running collections `tegracli` sports an *account group* feature which retrieves the history of a given set of accounts and is able to retrieve updates on each of these accounts.
 
-Groups are initialized by calling `teracli group init`, where accounts to track are stated by either stating them as arguments
-or by reading in a file.
+Groups are initialized by calling `teracli group init`, where accounts to track are stated by either stating them as arguments or by reading in a file.
 
-### Account Group File Format
+#### Account Group File Format
 
 Account files are expected to follow these requirements:
 
 - UTF8 text document,
 - per line one account, given as either username, channel-URL or ID,
 - there shall be no header and  no additional columns
 
@@ -186,27 +238,32 @@
  |- mysession.session
  |- my_group/
     |- tegracli_group.conf.yml
     |- profiles.jsonl
     |- 10000001.jsonl
     |- 10000002.jsonl
 ```
-To run the project command your terminal to `tegracli group run my_group` to collect the latest post of the accounts you want to track.
+
+To run the project command your terminal to `tegracli group run my_group` to collect the latest post of the accounts you want to track. If you have multiple groups configured you can run all by running `tegracli group run all`. This interprets all subdirectories as valid groups. However, `tegracli` will fail if a subdirectory is not a valid group.
 
 ```text
 Usage: tegracli group run [OPTIONS] [GROUPS]...
 
-  load a group configuration and run the groups operations
+  Load a group configuration and run the groups operations.
+    
+  GROUPS are subdirectories with a valid group configuration.
+    If the special keyword all is given, all subdirectories are considered.
 ```
 
 ## Result File Format
 
 Messages are stored in `jsonl`-files per channel or query. For channels filename is the channel's or user's id, for searches the query.
 **BEWARE:** how directories and files are structured is subject to active development and prone to changes in the near future.
 
-# Developer Installation
+## Developer Installation
 
 1. Install [poetry](https://python-poetry.org/docs/#installation),
 2. Clone repository and unzip, if necessary,
 3. In the directory run `poetry install`,
 4. Run `poetry shell` to start the development virtualenv,
 5. Run `pytest` to run tests, run `pytest --run_api` to include tests against the Telegram API (**these do require a valid configuration**), coverage report can be found under `tests/coverage`.
+
```

### Comparing `tegracli-0.2.5/pyproject.toml` & `tegracli-0.2.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tegracli"
-version = "0.2.5"
+version = "0.2.6"
 description = "A research-focused Telegram CLI application"
 authors = ["Philipp Kessling <p.kessling@leibniz-hbi.de>", "Felix Münch <f.muench@lebniz-hbi.de>"]
 readme  = "README.md"
 license = "MIT"
 repository  = "https://github.com/Leibniz-HBI/tegracli"
 homepage = "https://pypi.org/project/tegracli/"
 classifiers = [
@@ -29,14 +29,15 @@
 pytest-asyncio = "^0.18.3"
 black = "^22.6.0"
 isort = "^5.10.1"
 pytest-cov = "^3.0.0"
 coverage = "^6.4.2"
 pydocstyle = "^6.1.1"
 pylint = "*"
+pre-commit = "^3.3.3"
 
 [tool.pytest.ini_options]
 addopts = "--disable-socket --cov-report html:tests/coverage --cov=tegracli --capture=sys"
 asyncio_mode = "strict"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `tegracli-0.2.5/tegracli/dispatch.py` & `tegracli-0.2.6/tegracli/dispatch.py`

 * *Files identical despite different names*

### Comparing `tegracli-0.2.5/tegracli/group.py` & `tegracli-0.2.6/tegracli/group.py`

 * *Files identical despite different names*

### Comparing `tegracli-0.2.5/tegracli/main.py` & `tegracli-0.2.6/tegracli/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,21 +36,55 @@
 
 async def _handle_auth(client: TelegramClient):
     phone_number = click.prompt("Enter your phone number")
     await client.send_code_request(phone_number)
     await client.sign_in(phone_number, click.prompt("Enter 2FA code"))
 
 
+log_levels = {
+    1: "CRITICAL",
+    2: "ERROR",
+    3: "WARNING",
+    4: "INFO",
+    5: "DEBUG",
+}
+
+
 @click.group()
-@click.option("--debug/--no-debug", default=False)
+@click.option(
+    "--debug",
+    "-d",
+    is_flag=True,
+    help="Enable legacy debugging, is overwritten by the other options. Defaults to False.",
+    default=False,
+)
+@click.option("--verbose", "-v", count=True, help="Logging verbosity.", default=0)
+@click.option(
+    "--log-file",
+    "-l",
+    help="File to log to. Defaults to STDOUT.",
+    type=click.File("w", encoding="UTF-8"),
+    default="-",
+)
+@click.option(
+    "--serialize", "-s", help="Serialize output to JSON.", is_flag=True, default=False
+)
 @click.pass_context
-def cli(ctx: click.Context, debug: bool):
+def cli(
+    ctx: click.Context, debug: bool, verbose: int, log_file: click.File, serialize: bool
+) -> None:
     """Tegracli!! Retrieve messages from *Te*le*gra*m with a *CLI*!"""
-    if debug is True:
-        log.add("tegracli.log.json", serialize=True)
+    log.remove()
+
+    serialize = debug or serialize
+    log_file = "tegracli.log.jsonl" if debug else log_file
+    log_level = log_levels[verbose] if verbose != 0 else "DEBUG"
+
+    if verbose != 0 or debug:
+        log.add(log_file, level=log_level, serialize=serialize)
 
     if ctx.obj is None:
         ctx.obj = {}
 
     if not CONFIGURATION_PATH.exists() and not ctx.invoked_subcommand == "configure":
         log.error("Configuration not found. Terminating!")
         sys.exit(127)
@@ -258,15 +292,19 @@
         conf.dump()
 
 
 @group.command()
 @click.argument("groups", nargs=-1)
 @click.pass_context
 def run(ctx: click.Context, groups: Tuple[str]):
-    """Load a group configuration and run the groups operations."""
+    """Load a group configuration and run the groups operations.
+
+    GROUPS are subdirectories with a valid group configuration.
+        If the special keyword all is given, all subdirectories are considered.
+    """
     client = ctx.obj["client"]
     with client:
         run_group(client, groups)
 
 
 def _handle_group_member(member: str, conf: Group, client: TelegramClient) -> None:
     # check whether member is known already and, thus, present in profiles.jsonl
@@ -348,14 +386,21 @@
         )
 
 
 def run_group(client: TelegramClient, groups: Tuple[str]):
     """Runs the required operations for the specified groups."""
     cwd = Path()
 
+    if groups == ("all",):
+        groups = [
+            path
+            for path in Path().iterdir()
+            if path.is_dir() and not path.name.startswith(".")
+        ]
+
     # iterate groups
     for group_name in groups:
         # load group configuration
         conf: Group = _guarded_group_load(cwd, group_name)
 
         # iterate over group members
         for index, member in enumerate(conf.members):
```

### Comparing `tegracli-0.2.5/tegracli/utilities.py` & `tegracli-0.2.6/tegracli/utilities.py`

 * *Files identical despite different names*

### Comparing `tegracli-0.2.5/setup.py` & `tegracli-0.2.6/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,241 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+# tegracli
 
-packages = \
-['tegracli']
+![The TEGRACLI logo](https://github.com/Leibniz-HBI/tegracli/blob/trunk/tegracli.png?raw=true)
 
-package_data = \
-{'': ['*']}
+A convenience wrapper around Telethon and the Telegram Client API for research purposes.
 
-install_requires = \
-['PyYAML>=6.0,<7.0',
- 'Telethon>=1.24.0,<2.0.0',
- 'click>=8.1.3,<9.0.0',
- 'loguru>=0.6.0,<0.7.0',
- 'pandas>=1.4.3,<2.0.0',
- 'ujson>=5.4.0,<6.0.0']
-
-entry_points = \
-{'console_scripts': ['tegracli = tegracli.main:cli']}
-
-setup_kwargs = {
-    'name': 'tegracli',
-    'version': '0.2.5',
-    'description': 'A research-focused Telegram CLI application',
-    'long_description': '# tegracli\n\n![The TEGRACLI logo](https://github.com/Leibniz-HBI/tegracli/blob/trunk/tegracli.png?raw=true)\n\nA convenience wrapper around Telethon and the Telegram Client API for research purposes.\n\n# Installation Instructions\n\n`tegracli` uses Poetry and python >= 3.9 and < 4.0 for building and installing.\n\nTo install using pipx, run the following command `pipx install tegracli`.\n\n## How to get API keys\n\nIf you don\'t have API keys for Telegram, head over to [my.telegram.org](https://my.telegram.org).\nClick on [API development tools](https://my.telegram.org/apps), fill the form to create yourself an app and pluck the keys into `tegracli.conf.yml`. The session name can be arbitrary.\n\n```yaml\napi_id: 1234567\napi_hash : some12321hashthatmustbehere123\nsession_name: somesessionyo\n```\n\nThis template file is provided with the repository.\n\n# Usage\n\n`tegracli` is a terminal application to access the Telegram API for research purposes.\nIn order to retrieve messages the configuration-file from the section before must be present in the directory you start `tegracli`.\n\nThe following commands are available:\n\n## CONFIGURE\n\nOpens an interactive prompt for configuring API-access. Aks you to input your API id, API hash and session name and requests\na 2FA code from Telegram.\n\n```text\nUsage: tegracli configure [OPTIONS]\n\n  Configure tegracli.\n\nOptions:\n  --help  Show this message and exit.\n```\n\n## GET\n\nTo _get_ messages from a number of channels, use this command.\n\n```text\nUsage: tegracli get [OPTIONS] [CHANNELS]...\n\n  Get messages for the specified channels by either ID or username.\n\nOptions:\n  -l, --limit INTEGER           Number of messages to retrieve.\n  -O, --offset_date [%Y-%m-%d]  Offset retrieval to specific date in YYYY-MM-\n                                DD format.\n  -o, --offset_id INTEGER       Offset retrieval to a specific post number.\n  -m, --min_id INTEGER          Minimal post number.\n  -M, --max_id INTEGER          Maximal post number\n  -a, --add_offset INTEGER      Add an offset to the post numbers to be\n                                retrieved.\n  -f, --from_user TEXT          Only messages from this user.\n  --reverse / --forward         Should post numbers count upward or downward.\n                                Defaults to forward.\n  -r, --reply_to TEXT           Only messages replied to specific post id.\n  --help                        Show this message and exit.\n```\n\n| **parameter**       | **description**                                                                                                              |\n|---------------------|------------------------------------------------------------------------------------------------------------------------------|\n| **channels**        | a list of of either telegram usernames, channel or group URLs or user IDs.                                                   |\n| **limit**           | number of messages to retrieve, positive integer. If set to `-1` , retrieves all messages in the channel. defaults to `-1`.  |\n| **offset_date**     | specify start point of retrieval by date, retrieval direction is controlled by `reverse/forward`. Format must be YYYY-MM-DD. |\n| **offset_id**       | specify start point of retrieval by post number, retrieval direction is controlled by `reverse/forward`.                     |\n| **min_id**          | sets the minimum post number                                                                                                 |\n| **max_id**          | sets the maximum post number                                                                                                 |\n| **add_offset**      | add a offset to the post numbers to be retrieved                                                                             |\n| **from_user**       | limit messages to posts *from* a specific user                                                                               |\n| **reply_to**        | limit messages to replies *to* a specific user                                                                               |\n| **reverse/forward** | flag to indicate whether messages should be retrieved in chronological or reverse chronological order.                       |\n\n### Basic Examples\n\nTo retrieve the last fifty messages from a Telegram channel:\n\n```bash\ntegracli get --limit 50 corona_infokanal_bmg\n```\n\nTo retrieve the entire history starting with post #1 of a channel, set `limit` to `-1`.\n\n```bash\ntegracli get --reverse --limit -1 corona_infokanal_bmg\n```\nTo retrieve messages sent after January, 1st 2022:\n\n```bash\ntegracli get --offset_date 2022-01-01 corona_infokanal_bmg\n```\n\nTo retrieve message sent before January, 1st 2022:\n\n```bash\ntegracli get --reverse --offset_date 2022-01-01 corona_infokanal_bmg\n```\n## SEARCH\n\nTo _search_ messages of your chats and groups and channels you are subscribed to, use this command.\n\n```text\nUsage: tegracli search [OPTIONS] [QUERIES]...\n\n  This function searches Telegram content that is available to your account for the specified search term(s).\n\nOptions:\n  --help  Show this message and exit.\n```\n\n## HYDRATE\n\nTo rehydrate messages from the API this command accepts a file with message IDs in the format of `$channel_name/$post_number`.\nBoth input and output file are optional, if not given, `stdin` and `stdout` are used.\n\nOutput data is JSONL, one message per line.\n\n```text\nUsage: tegracli hydrate [OPTIONS] [INPUT_FILE] [OUTPUT_FILE]\n\n  Hydrate a file with messages-ids.\n\nOptions:\n  --help  Show this message and exit.\n```\n\nFor example, to rehydrate message IDs:\n\n```bash\necho test_channel/1234 | tegracli hydrate\n>> {"_":"Message","id": 1234, ... , "restriction_reason":[],"ttl_period":null}\n```\n\n## GROUP INIT and GROUP RUN\n\nIn order to support updatable  and long-running collections `tegracli` sports an *account group* feature which retrieves\nthe history of a given set of accounts and is able to retrieve updates on each of these accounts.\n\nGroups are initialized by calling `teracli group init`, where accounts to track are stated by either stating them as arguments\nor by reading in a file.\n\n### Account Group File Format\n\nAccount files are expected to follow these requirements:\n\n- UTF8 text document,\n- per line one account, given as either username, channel-URL or ID,\n- there shall be no header and  no additional columns\n\n```text\nUsage: tegracli group init [OPTIONS] NAME [ACCOUNTS]...\n\n  initialize a new account group\n\nOptions:\n  -f, --read_file PATH         read an account list from a file, one\n                               handle/id/url per line.\n  -s, --start_date [%Y-%m-%d]  Start date for the collection. Must be in YYYY-\n                               MM-DD format.\n  -l, --limit INTEGER          number of posts fo retrieve in one run\n  --help                       Show this message and exit.\n```\n\nA group is essentially a directory in your tegracli project folder which holdes\na group configuration file, a `profiles.jsonl` file which will collect all user objects returned\nby Telegram (these will be recycled to save API requests), as well as the jsonl-files containing the messages.\nThe messages-files are structured in a way that one file holds the messages of one account and is named by the\naccount\'s ID.\n\nAn exemplary project could look this:\n\n```text\ntegracli-project/\n |- tegracli.conf.yml\n |- mysession.session\n |- my_group/\n    |- tegracli_group.conf.yml\n    |- profiles.jsonl\n    |- 10000001.jsonl\n    |- 10000002.jsonl\n```\nTo run the project command your terminal to `tegracli group run my_group` to collect the latest post of the accounts you want to track.\n\n```text\nUsage: tegracli group run [OPTIONS] [GROUPS]...\n\n  load a group configuration and run the groups operations\n```\n\n## Result File Format\n\nMessages are stored in `jsonl`-files per channel or query. For channels filename is the channel\'s or user\'s id, for searches the query.\n**BEWARE:** how directories and files are structured is subject to active development and prone to changes in the near future.\n\n# Developer Installation\n\n1. Install [poetry](https://python-poetry.org/docs/#installation),\n2. Clone repository and unzip, if necessary,\n3. In the directory run `poetry install`,\n4. Run `poetry shell` to start the development virtualenv,\n5. Run `pytest` to run tests, run `pytest --run_api` to include tests against the Telegram API (**these do require a valid configuration**), coverage report can be found under `tests/coverage`.\n',
-    'author': 'Philipp Kessling',
-    'author_email': 'p.kessling@leibniz-hbi.de',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://pypi.org/project/tegracli/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+## Installation Instructions
 
+`tegracli` uses Poetry and python >= 3.9 and < 4.0 for building and installing.
 
-setup(**setup_kwargs)
+To install using pipx, run the following command `pipx install tegracli`.
+
+### How to get API keys
+
+If you don't have API keys for Telegram, head over to [my.telegram.org](https://my.telegram.org).
+Click on [API development tools](https://my.telegram.org/apps), fill the form to create yourself an app and pluck the keys into `tegracli.conf.yml`. The session name can be arbitrary.
+
+```yaml
+api_id: 1234567
+api_hash : some12321hashthatmustbehere123
+session_name: somesessionyo
+```
+
+This template file is provided with the repository.
+
+## Usage
+
+`tegracli` is a terminal application to access the Telegram API for research purposes.
+In order to retrieve messages the configuration-file from the section before must be present in the directory you start `tegracli`.
+
+```text
+Usage: tegracli [OPTIONS] COMMAND [ARGS]...
+
+  Tegracli!! Retrieve messages from *Te*le*gra*m with a *CLI*!
+
+Options:
+  -d, --debug              Enable legacy debugging, is overwritten by the
+                           other options. Defaults to False.
+  -v, --verbose            Logging verbosity.
+  -l, --log-file FILENAME  File to log to. Defaults to STDOUT.
+  -s, --serialize          Serialize output to JSON.
+  --help                   Show this message and exit.
+
+Commands:
+  configure  Configure tegracli.
+  get        Get messages for the specified channels by either ID or...
+  group      Manage account groups.
+  hydrate    Hydrate a file with messages-ids.
+  search     Searches Telegram content that is available to your account.
+```
+
+## Logging
+
+`tegracli` allows for configuring what and how it is logged. Per default logging is **disabled** and can be enabled by passing `--verbose` or `-v`, logging level can be increased by more `-vvvv`s. By default logging target is `STDOUT` but this can be redirected to a file with `--log-file yourfile.log`. Setting `--serialize` allows to be to write the entire logging information in JSON-encoded form. `--debug` is the legacy option used by `tegracli` <= 0.2.5, this will set serialized logging into `tegracli.log.jsonl` at the `DEBUG` level; it is overwritten by setting the `--verbose` option.
+
+## Commands 
+
+The following commands are available:
+
+### configure
+
+Opens an interactive prompt for configuring API-access. Aks you to input your API id, API hash and session name and requests
+a 2FA code from Telegram.
+
+```text
+Usage: tegracli configure [OPTIONS]
+
+  Configure tegracli.
+
+Options:
+  --help  Show this message and exit.
+```
+
+### get
+
+To _get_ messages from a number of channels, use this command.
+
+```text
+Usage: tegracli get [OPTIONS] [CHANNELS]...
+
+  Get messages for the specified channels by either ID or username.
+
+Options:
+  -l, --limit INTEGER           Number of messages to retrieve.
+  -O, --offset_date [%Y-%m-%d]  Offset retrieval to specific date in YYYY-MM-
+                                DD format.
+  -o, --offset_id INTEGER       Offset retrieval to a specific post number.
+  -m, --min_id INTEGER          Minimal post number.
+  -M, --max_id INTEGER          Maximal post number
+  -a, --add_offset INTEGER      Add an offset to the post numbers to be
+                                retrieved.
+  -f, --from_user TEXT          Only messages from this user.
+  --reverse / --forward         Should post numbers count upward or downward.
+                                Defaults to forward.
+  -r, --reply_to TEXT           Only messages replied to specific post id.
+  --help                        Show this message and exit.
+```
+
+| **parameter**       | **description**                                                                                                              |
+|---------------------|------------------------------------------------------------------------------------------------------------------------------|
+| **channels**        | a list of of either telegram usernames, channel or group URLs or user IDs.                                                   |
+| **limit**           | number of messages to retrieve, positive integer. If set to `-1` , retrieves all messages in the channel. defaults to `-1`.  |
+| **offset_date**     | specify start point of retrieval by date, retrieval direction is controlled by `reverse/forward`. Format must be YYYY-MM-DD. |
+| **offset_id**       | specify start point of retrieval by post number, retrieval direction is controlled by `reverse/forward`.                     |
+| **min_id**          | sets the minimum post number                                                                                                 |
+| **max_id**          | sets the maximum post number                                                                                                 |
+| **add_offset**      | add a offset to the post numbers to be retrieved                                                                             |
+| **from_user**       | limit messages to posts *from* a specific user                                                                               |
+| **reply_to**        | limit messages to replies *to* a specific user                                                                               |
+| **reverse/forward** | flag to indicate whether messages should be retrieved in chronological or reverse chronological order.                       |
+
+#### Basic Examples
+
+To retrieve the last fifty messages from a Telegram channel:
+
+```bash
+tegracli get --limit 50 corona_infokanal_bmg
+```
+
+To retrieve the entire history starting with post #1 of a channel, set `limit` to `-1`.
+
+```bash
+tegracli get --reverse --limit -1 corona_infokanal_bmg
+```
+To retrieve messages sent after January, 1st 2022:
+
+```bash
+tegracli get --offset_date 2022-01-01 corona_infokanal_bmg
+```
+
+To retrieve message sent before January, 1st 2022:
+
+```bash
+tegracli get --reverse --offset_date 2022-01-01 corona_infokanal_bmg
+```
+### search
+
+To _search_ messages of your chats and groups and channels you are subscribed to, use this command.
+
+```text
+Usage: tegracli search [OPTIONS] [QUERIES]...
+
+  This function searches Telegram content that is available to your account for the specified search term(s).
+
+Options:
+  --help  Show this message and exit.
+```
+
+### hydrate
+
+To rehydrate messages from the API this command accepts a file with message IDs in the format of `$channel_name/$post_number`.
+Both input and output file are optional, if not given, `stdin` and `stdout` are used.
+
+Output data is JSONL, one message per line.
+
+```text
+Usage: tegracli hydrate [OPTIONS] [INPUT_FILE] [OUTPUT_FILE]
+
+  Hydrate a file with messages-ids.
+
+Options:
+  --help  Show this message and exit.
+```
+
+For example, to rehydrate message IDs:
+
+```bash
+echo test_channel/1234 | tegracli hydrate
+>> {"_":"Message","id": 1234, ... , "restriction_reason":[],"ttl_period":null}
+```
+
+### groups
+
+In order to support updatable  and long-running collections `tegracli` sports an *account group* feature which retrieves the history of a given set of accounts and is able to retrieve updates on each of these accounts.
+
+Groups are initialized by calling `teracli group init`, where accounts to track are stated by either stating them as arguments or by reading in a file.
+
+#### Account Group File Format
+
+Account files are expected to follow these requirements:
+
+- UTF8 text document,
+- per line one account, given as either username, channel-URL or ID,
+- there shall be no header and  no additional columns
+
+```text
+Usage: tegracli group init [OPTIONS] NAME [ACCOUNTS]...
+
+  initialize a new account group
+
+Options:
+  -f, --read_file PATH         read an account list from a file, one
+                               handle/id/url per line.
+  -s, --start_date [%Y-%m-%d]  Start date for the collection. Must be in YYYY-
+                               MM-DD format.
+  -l, --limit INTEGER          number of posts fo retrieve in one run
+  --help                       Show this message and exit.
+```
+
+A group is essentially a directory in your tegracli project folder which holdes
+a group configuration file, a `profiles.jsonl` file which will collect all user objects returned
+by Telegram (these will be recycled to save API requests), as well as the jsonl-files containing the messages.
+The messages-files are structured in a way that one file holds the messages of one account and is named by the
+account's ID.
+
+An exemplary project could look this:
+
+```text
+tegracli-project/
+ |- tegracli.conf.yml
+ |- mysession.session
+ |- my_group/
+    |- tegracli_group.conf.yml
+    |- profiles.jsonl
+    |- 10000001.jsonl
+    |- 10000002.jsonl
+```
+
+To run the project command your terminal to `tegracli group run my_group` to collect the latest post of the accounts you want to track. If you have multiple groups configured you can run all by running `tegracli group run all`. This interprets all subdirectories as valid groups. However, `tegracli` will fail if a subdirectory is not a valid group.
+
+```text
+Usage: tegracli group run [OPTIONS] [GROUPS]...
+
+  Load a group configuration and run the groups operations.
+    
+  GROUPS are subdirectories with a valid group configuration.
+    If the special keyword all is given, all subdirectories are considered.
+```
+
+## Result File Format
+
+Messages are stored in `jsonl`-files per channel or query. For channels filename is the channel's or user's id, for searches the query.
+**BEWARE:** how directories and files are structured is subject to active development and prone to changes in the near future.
+
+## Developer Installation
+
+1. Install [poetry](https://python-poetry.org/docs/#installation),
+2. Clone repository and unzip, if necessary,
+3. In the directory run `poetry install`,
+4. Run `poetry shell` to start the development virtualenv,
+5. Run `pytest` to run tests, run `pytest --run_api` to include tests against the Telegram API (**these do require a valid configuration**), coverage report can be found under `tests/coverage`.
```

