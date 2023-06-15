# Comparing `tmp/p3do-0.6.1.tar.gz` & `tmp/p3do-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p3do-0.6.1.tar", max compression
+gzip compressed data, was "p3do-0.7.0.tar", max compression
```

## Comparing `p3do-0.6.1.tar` & `p3do-0.7.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-03-20 12:59:28.801176 p3do-0.6.1/LICENSE
--rw-r--r--   0        0        0    14949 2023-03-20 12:59:28.801176 p3do-0.6.1/README.md
--rw-r--r--   0        0        0       22 2023-03-20 12:59:28.801176 p3do-0.6.1/p3do/__init__.py
--rw-r--r--   0        0        0    12075 2023-03-20 12:59:28.801176 p3do-0.6.1/p3do/cli.py
--rw-r--r--   0        0        0     1798 2023-03-20 12:59:28.801176 p3do-0.6.1/p3do/jenkins.py
--rw-r--r--   0        0        0     1161 2023-03-20 12:59:28.801176 p3do-0.6.1/p3do/keycloak.py
--rw-r--r--   0        0        0     4626 2023-03-20 12:59:28.801176 p3do-0.6.1/p3do/poolparty.py
--rw-r--r--   0        0        0      915 2023-03-20 12:59:28.801176 p3do-0.6.1/pyproject.toml
--rw-r--r--   0        0        0    16313 2023-03-20 12:59:44.626616 p3do-0.6.1/setup.py
--rw-r--r--   0        0        0    15836 2023-03-20 12:59:44.627668 p3do-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-15 11:14:09.440278 p3do-0.7.0/LICENSE
+-rw-r--r--   0        0        0    15444 2023-06-15 11:14:09.440278 p3do-0.7.0/README.md
+-rw-r--r--   0        0        0       22 2023-06-15 11:14:09.440278 p3do-0.7.0/p3do/__init__.py
+-rw-r--r--   0        0        0    13964 2023-06-15 11:14:09.440278 p3do-0.7.0/p3do/cli.py
+-rw-r--r--   0        0        0      274 2023-06-15 11:14:09.440278 p3do-0.7.0/p3do/github.py
+-rw-r--r--   0        0        0     1832 2023-06-15 11:14:09.440278 p3do-0.7.0/p3do/jenkins.py
+-rw-r--r--   0        0        0     1161 2023-06-15 11:14:09.440278 p3do-0.7.0/p3do/keycloak.py
+-rw-r--r--   0        0        0     4626 2023-06-15 11:14:09.440278 p3do-0.7.0/p3do/poolparty.py
+-rw-r--r--   0        0        0      936 2023-06-15 11:14:09.444278 p3do-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    16424 1970-01-01 00:00:00.000000 p3do-0.7.0/PKG-INFO
```

### Comparing `p3do-0.6.1/LICENSE` & `p3do-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `p3do-0.6.1/README.md` & `p3do-0.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -103,14 +103,17 @@
     - [`install-snapshot`](#install-snapshot): Download and run latest snapshot installer. Linux only.
     - [`mock-server`](#mock-server): Run a mock server for debugging external
       services integration (Semantic Middleware Configurator).
 
 * [`kc`](#kc): Keycloak commands
     - [KC Configuration](#kc-configuration): Not a command but read this first!
     - [`add-mappers`](#add-mappers): Add mappers to IdPs from realm export
+    
+* [`gh`](#gh): GitHub commands
+    - [`deploy-key`](#deploy-key): Add a deployment key to a GitHub repository
 
 ### jk
 
 Commands in this group allow to perform common operations on Jenkins.
 
 #### build
 
@@ -364,14 +367,28 @@
 does not import mapper configuration by itself (yet?).
 
 ```bash
 # `realm-export.json` is the path the the export file
 p3do kc add-mappers --auth_config config.ini --auth test realm-export.json
 ```
 
+### gh
+
+Commands in this group allow to perform operations on GitHub
+`poolparty-semantic-suite` organization. Most operations need an access token.
+This can be generated in GitHub user settings
+https://github.com/settings/tokens.
+
+Commands:
+* [`deploy-key`](#deploy-key): Add a deployment key to a GitHub repository
+
+#### deploy-key
+
+Add a deployment key to a GitHub repository.
+
 ## Contribute
 
 ***`p3do` is licensed under MIT and published to PyPI (including source). Do not
 add sensitive company data. Any sensitive data has to be read from external
 configuration files.***
 
 ### Contributors
```

### Comparing `p3do-0.6.1/p3do/cli.py` & `p3do-0.7.0/p3do/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from .keycloak import Keycloak
 from . import poolparty
 from . import jenkins
+from . import github
 
 from functools import update_wrapper, partial
 from configparser import ConfigParser
 from sys import platform
 import subprocess
 import os
 import sys
 import appdirs
 import click
 import tempfile
+import time
+import math
 
 from pathlib import Path
 
 from loguru import logger
 
 
 @click.group()
@@ -33,14 +36,19 @@
     ...
 
 @cli.group()
 def kc():
     """Keycloak commands"""
     ...
 
+@cli.group()
+def gh():
+    """GitHub commands"""
+    ...
+
 def kc_adm_command(func):
     """Decorator to encapsulate common logic for kc admin commands that need authentication"""
     @click.option("--server", help="The server url")
     @click.option("--username", help="The username for import must have rights to modify the realm")
     @click.option("--password", help="The password")
     @click.option("--user_realm_name", help="The realm the user is in")
     @click.option("--realm_name", help="The realm the mappers should be added to")
@@ -299,18 +307,60 @@
         logger.info("No branch specified and autodetect disabled. Using branch {}", branch)
     elif not branch and not no_autodetect:
         res = subprocess.run(["git", "rev-parse", "--abbrev-ref", "HEAD"], capture_output=True)
         if res.returncode == 0:
             branch = res.stdout.decode('utf-8').strip(" \n")
             logger.info("No branch specified and autodetect enabled. Using current branch {} of git directory", branch)
         else:
-            branch = "develop"
+
             logger.info("No branch specified and autodetect enabled. Not in a git directory. Using branch {}", branch)
     else: # branch given
         logger.info("Using branch {}", branch)
 
     url = jenkins.run_deploy("P3D-Build-Deploy-PoolParty-(parent-pom)", server, branch, api_user, api_key)
     print(f"{url}")
 
 
+@gh.command()
+@click.argument("repository")
+@click.argument("ssh-key")
+@click.option("--token", help="GitHub access token (generate in GitHub)")
+@click.option("--title", help="Title for the deploy key")
+@click.option("--write_access", type=click.BOOL, is_flag=True, default=False, help="Allow deploy key write access to the repository")
+def deploy_key(repository: str, ssh_key: str, token: str, title: str, write_access: bool):
+    """Add a deployment key to a GitHub repository"""
+
+    if not token:
+        cache_dir = appdirs.user_cache_dir("p3do")
+        os.makedirs(cache_dir, exist_ok=True)
+        gh_key = os.path.join(cache_dir, "gh_key")
+
+        try:
+            with open(gh_key, 'r') as f:
+                token = f.read()
+        except:
+            token = click.prompt("GitHub Access Token")
+            with open(gh_key, 'w') as f:
+                f.write(token)
+
+    if not title:
+        logger.debug("No title given, inferring title")
+        key_sections = ssh_key.split(" ")
+        if len(key_sections) >= 3:
+            logger.debug("Inferring title from ssh comment section")
+            title=key_sections[2]
+        else:
+            logger.debug("No comment section in ssh key. Using generated title.")
+            title = "deploy-key"+str(math.floor(time.time()))
+
+    logger.debug("Cleaning up repository name")
+    repository = repository.strip()
+    repository = repository.strip('/')
+    if not repository.startswith("poolparty-semantic-suite"):
+        logger.debug("Repository does not contain `poolparty-semantic-suite` organization. Trying to add organization.")
+        repository = "poolparty-semantic-suite/"+repository
+
+    logger.info(f"Creating deploy key {ssh_key} for repository {repository}")
+    github.deploy_key(repository, ssh_key, token, title, not write_access)
+
 if __name__ == "__main__":
     cli()
```

### Comparing `p3do-0.6.1/p3do/jenkins.py` & `p3do-0.7.0/p3do/jenkins.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     # This will start the job and will return a QueueItem object which
     # can be used to get build results
     jk_job = server[job]
     logger.debug("Got job {}", jk_job)
     qi = jk_job.invoke(build_params=params)
     logger.debug("Got job invocation {}", qi)
 
+    breakpoint()
     logger.info("Block until building")
     qi.block_until_building()
     logger.info("Started build {}", qi.get_build())
     return qi.get_build().get_build_url()
 
 
 @logger.catch
@@ -45,11 +46,12 @@
     # This will start the job and will return a QueueItem object which
     # can be used to get build results
     jk_job = server[job]
     logger.debug("Got job {}", jk_job)
     qi = jk_job.invoke(build_params=params)
     logger.debug("Got job invocation {}", qi)
 
+    breakpoint()
     logger.info("Block until building")
     qi.block_until_building()
     logger.info("Started build {}", qi.get_build())
     return qi.get_build().get_build_url()
```

### Comparing `p3do-0.6.1/p3do/keycloak.py` & `p3do-0.7.0/p3do/keycloak.py`

 * *Files identical despite different names*

### Comparing `p3do-0.6.1/p3do/poolparty.py` & `p3do-0.7.0/p3do/poolparty.py`

 * *Files identical despite different names*

### Comparing `p3do-0.6.1/pyproject.toml` & `p3do-0.7.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "p3do"
-version = "0.6.1"
+version = "0.7.0"
 description = "CLI utilities for p3d"
 authors = ["Armin Friedl <armin.friedl@semantic-web.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -16,14 +16,15 @@
                      # are incompatible with python-keycloak
 cryptography = ">=37.0.3,<40.0.0"
 appdirs = "^1.4.4"
 jenkinsapi = "^0.3.11"
 loguru = "^0.6.0"
 rich = "^12.4.4"
 Flask = "^2.1.3"
+pygithub = "^1.58.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 black = "^22.3.0"
 pyflakes = "^2.4.0"
 isort = "^5.10.1"
```

### Comparing `p3do-0.6.1/setup.py` & `p3do-0.7.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,456 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: p3do
+Version: 0.7.0
+Summary: CLI utilities for p3d
+License: MIT
+Author: Armin Friedl
+Author-email: armin.friedl@semantic-web.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Flask (>=2.1.3,<3.0.0)
+Requires-Dist: appdirs (>=1.4.4,<2.0.0)
+Requires-Dist: click (>=8.1,<9.0)
+Requires-Dist: cryptography (>=37.0.3,<40.0.0)
+Requires-Dist: jenkinsapi (>=0.3.11,<0.4.0)
+Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: pygithub (>=1.58.2,<2.0.0)
+Requires-Dist: python-keycloak (>=0.27,<0.28)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: rich (>=12.4.4,<13.0.0)
+Requires-Dist: urllib3 (>=1.26.9,<2.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['p3do']
+<div align="center">
 
-package_data = \
-{'': ['*']}
+# p3do - let 'em minions do it
 
-install_requires = \
-['Flask>=2.1.3,<3.0.0',
- 'appdirs>=1.4.4,<2.0.0',
- 'click>=8.1,<9.0',
- 'cryptography>=37.0.3,<40.0.0',
- 'jenkinsapi>=0.3.11,<0.4.0',
- 'loguru>=0.6.0,<0.7.0',
- 'python-keycloak>=0.27,<0.28',
- 'requests>=2.27.1,<3.0.0',
- 'rich>=12.4.4,<13.0.0',
- 'urllib3>=1.26.9,<2.0.0']
-
-entry_points = \
-{'console_scripts': ['p3do = p3do.cli:cli']}
-
-setup_kwargs = {
-    'name': 'p3do',
-    'version': '0.6.1',
-    'description': 'CLI utilities for p3d',
-    'long_description': '<div align="center">\n\n# p3do - let \'em minions do it\n\n[![PyPI - License](https://img.shields.io/pypi/l/p3do)](https://github.com/poolparty-semantic-suite/p3do/blob/main/LICENSE)\n[![PyPI](https://img.shields.io/pypi/v/p3do)](https://pypi.org/project/p3do/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/p3do)](https://www.python.org/)\n[![Publish](https://github.com/poolparty-semantic-suite/p3do/actions/workflows/publish.yml/badge.svg)](https://github.com/poolparty-semantic-suite/p3do/actions)\n\n\np3do (pronounced _pee-three-duh_) is a collection of command-line utilities for\np3d. It allows you to conjure some tedious operations right from your magic little\nfingertips.\n\n<img src="res/p3do-animation.gif?raw=true" alt="p3do in action" width="75%"/>\n\n<p />\n\n[Installation](#installation) •\n[Getting started](#getting-started) •\n[Commands](#commands) •\n[Contribute](#contribute)\n\n</div>\n\n## Installation\n<img src="res/p3do-logo.png?raw=true" alt="p3do logo" align="right" width="180px"/>\n\n`p3do` is built with Python 3.8 or later. You can get Python from your package\nmanager du jour or download and install it from\nhttps://www.python.org/downloads/ (looking at you Windows. Mac.\nWhyihavetobother. Veryannoyingyouare.)\n\n`p3do` is published to the [CheeseShop](https://pypi.org/project/p3do/) and\nhence can be installed with pip:\n\n```bash\npip install p3do\n```\n\n`p3do` installs itself as a command. If your `$PATH` is set up correctly you\nwill be able to just invoke `p3do` like so\n\n```bash\np3do --help\n```\n\n### Shell Completion\n\n`p3do` supports shell completion (tab completion). Shell completion is supported\nfor bash, zsh and fish shells. For each of these, the autocompletion script is\ndifferent.\n\nBash 4.4 and later:\n``` bash\n# add to your ~/.bashrc\neval "$(_P3DO_COMPLETE=bash_source p3do)"\n```\n\nZsh:\n``` bash\n# add to your ~/.zshrc:\neval "$(_P3DO_COMPLETE=zsh_source p3do)"\n```\n\nFish:\n``` bash\n#  ~/.config/fish/completions/p3do.fish\neval (env _P3DO_COMPLETE=fish_source p3do)\n```\n\n## Getting Started\n\n<img src="res/p3do-logo2.png?raw=true" alt="p3do logo" align="left" width="180px"/>\n\nLight a bonfire and whisper _p3do_ in the most conspirative voice available to\nyou. Then start a terminal.\n\n`p3do` is hierarchical, self-documenting and discoverable. The best way to start\nis to just type `p3do`. This will show you the available commands and some\ndescription. From there you can drill down the hierarchy for useful sub-command.\n\nEach sub-command/command group has special flags and configuration. How to use\nthem is explained in [Commands](#commands) for each of them separately. You can\nalso use `p3d <group> <command> --help` in your terminal for concise on-line\nhelp.\n\n## Commands\n\n`p3do` is hierarchical. Commands are batched into groups which can be further\nnested into parent groups. We follow the same principle in the documentation\nhere.\n\n* [`jk`](#jk): Jenkins commands\n    - [`build`](#build): Run the `P3D-BUILD` jenkins job with smart branch\n      detection\n    - [`deploy`](#deploy): Run the `P3D-Build-Deploy-PoolParty-(parent-pom)`\n      jenkins job with smart branch detection\n\n* [`pp`](#pp): PoolParty commands\n    - [`encrypt`](#encrypt): Encrypt a clear text with poolparty encryption\n    - [`decrypt`](#decrypt): Decrypt a secret text with poolparty encryption\n    - [`install-snapshot`](#install-snapshot): Download and run latest snapshot installer. Linux only.\n    - [`mock-server`](#mock-server): Run a mock server for debugging external\n      services integration (Semantic Middleware Configurator).\n\n* [`kc`](#kc): Keycloak commands\n    - [KC Configuration](#kc-configuration): Not a command but read this first!\n    - [`add-mappers`](#add-mappers): Add mappers to IdPs from realm export\n\n### jk\n\nCommands in this group allow to perform common operations on Jenkins.\n\n#### build\n\nStart the `P3D-BUILD` job from the command line with smart branch detection.\nFor this command `git` has to be installed.\n\nPer default (and outside a git repository) builds the `develop` branch of\nPoolParty.\n\nWhen inside a git repository p3do will automatically detect the current\nbranch and build it. This behavior can be disabled with `--no-autodetect`.\n\nThe branch to build can be specified via `--branch` (note that this implies\n`--no-autodetect` inside a git repository).\n\nWith `--api-user` and `--api-key` you can specify the credentials accessing the\nJenkins API. These credentials are cached and only need to be specified once. If\nnot specified and no cached credentials are found, p3do will ask for them\ninteractively. You can generate a token for `--api-key` in your [Jenkins Account\nSettings](https://ci2.semantic-web.at/user/<username>/configure). `--api-user`\nis the username you use to log in to Jenkins.\n\n``` bash\n# Build branch PoolParty develop without branch detection\np3do jk build --branch develop\n```\n\n#### deploy\n\nStart the `P3D-Build-Deploy-PoolParty-(parent-pom)` job from the command line\nwith smart branch detection. For this command `git` has to be installed.\n\nPer default (and outside a git repository) deploys the `develop` branch of\nPoolParty.\n\nWhen inside a git repository `p3do` will automatically detect the current branch\nand deploy it. This behavior can be disabled with --no-autodetect.\n\nThe branch to deploy can be specified via --branch (note that this implies\n--no-autodetect inside a git repository).\n\nWith `--api-user` and `--api-key` you can specify the credentials accessing the\nJenkins API. These credentials are cached and only need to be specified once. If\nnot specified and no cached credentials are found, p3do will ask for them\ninteractively. You can generate a token for `--api-key` in your [Jenkins Account\nSettings](https://ci2.semantic-web.at/user/<username>/configure). `--api-user`\nis the username you use to log in to Jenkins.\n\nThe `SERVER` argument is mandatory and must be a valid ssh server name.\nPoolParty will be deployed to this server.\n\n``` bash\n# Deploy PoolParty develop branch to pp-lazer-kittens-dev without branch detection\np3do jk deploy --branch develop pp-lazer-kittens-dev\n```\n\n### pp\n\nCommands in this group allow to perform operations useful for or related to\nour dear PoolParty.\n\n#### encrypt\n\nEncrypt a clear text with PoolParty encryption. The parameters for encryption\nused by PoolParty can usually be found in the `poolparty.properties` file.\n\nThis command can be used by specifying the encryption parameters directly as\noptions to p3do (`--password`, `--salt`, `--strength`) or with an interactive\nprompt (just specify the clear text and leave out the options).\n\nTo make sure that your command line processor does not mingle the input, always\nwrap the clear text, password, and salt it in quotes if you are passing them as\noptions to p3do.\n\nFor interactive prompt do _not_ wrap them in quotes.\n\nInteractive prompt:\n``` bash\n# encrypt mysecret with \n# password H7dwBFDh3gEVDH1YecgikmOBpx9kKZ9nj1wJ5ZuhEeg=\n# salt Y+Fw/4dHBajqEGxOsEyfNSGsYYXE7JUyLmc3nRFrB84=\n# and 256 rounds\np3do pp encrypt "mysecret"\nPassword: H7dwBFDh3gEVDH1YecgikmOBpx9kKZ9nj1wJ5ZuhEeg= # interactive prompt\nSalt: Y+Fw/4dHBajqEGxOsEyfNSGsYYXE7JUyLmc3nRFrB84= # interactive prompt\nStrength: 256 # interactive prompt\neYRLg0SUzGNSlfmS6MYrt8pnu5MTYU3EWVmNp1q/JFQ=\n```\n\nWith options:\n``` bash\n# encrypt mysecret with \n# password H7dwBFDh3gEVDH1YecgikmOBpx9kKZ9nj1wJ5ZuhEeg=\n# salt Y+Fw/4dHBajqEGxOsEyfNSGsYYXE7JUyLmc3nRFrB84=\n# and 256 rounds\np3do pp encrypt --password "H7dwBFDh3gEVDH1YecgikmOBpx9kKZ9nj1wJ5ZuhEeg=" --salt "Y+Fw/4dHBajqEGxOsEyfNSGsYYXE7JUyLmc3nRFrB84=" --strength 256 "mysecret"\n```\n\n#### decrypt\nDecrypt a secret text encrypted by PoolParty. The parameters for encryption/decryption used\nby PoolParty can usually be found in the `poolparty.properties` file.\n\nThis command can be used by specifying the encryption parameters directly as\noptions to p3do (`--password`, `--salt`, `--strength`) or with an interactive\nprompt (just specify the clear text and leave out the options).\n\nTo make sure that your command line processor does not mingle the input, always\nwrap the clear text, password, and salt it in quotes if you are passing them as\noptions to p3do.\n\nFor interactive prompt do _not_ wrap them in quotes.\n\nInteractive prompt:\n``` bash\n# decrypt 6NjzLmQp7kGM7bbezhQX1G2hrqCoqLrC32ayBTjQVjU= with \n# password H7dwBFDh3gEVDH1YecgikmOBpx9kKZ9nj1wJ5ZuhEeg=\n# salt Y+Fw/4dHBajqEGxOsEyfNSGsYYXE7JUyLmc3nRFrB84=\n# and 256 rounds\np3do pp decrypt "6NjzLmQp7kGM7bbezhQX1G2hrqCoqLrC32ayBTjQVjU="\nPassword: H7dwBFDh3gEVDH1YecgikmOBpx9kKZ9nj1wJ5ZuhEeg= # interactive prompt\nSalt: Y+Fw/4dHBajqEGxOsEyfNSGsYYXE7JUyLmc3nRFrB84= # interactive prompt\nStrength: 256 # interactive prompt\neYRLg0SUzGNSlfmS6MYrt8pnu5MTYU3EWVmNp1q/JFQ=\n```\n\nWith options:\n``` bash\n# decrypt 6NjzLmQp7kGM7bbezhQX1G2hrqCoqLrC32ayBTjQVjU= with \n# password H7dwBFDh3gEVDH1YecgikmOBpx9kKZ9nj1wJ5ZuhEeg=\n# salt Y+Fw/4dHBajqEGxOsEyfNSGsYYXE7JUyLmc3nRFrB84=\n# and 256 rounds\np3do pp decrypt --password "H7dwBFDh3gEVDH1YecgikmOBpx9kKZ9nj1wJ5ZuhEeg=" --salt "Y+Fw/4dHBajqEGxOsEyfNSGsYYXE7JUyLmc3nRFrB84=" --strength 256 "6NjzLmQp7kGM7bbezhQX1G2hrqCoqLrC32ayBTjQVjU=" \n```\n\n#### install-snapshot\n\nDownload and invoke the latest snapshot installer. Specify `--path` to download\nthe installer to a specific folder. Otherwise, the installer will be installed\nto a temporary directory. \n\nThis command is restricted to Linux for now.\n\n``` bash\np3do pp install-snapshot\n```\n\n#### mock-server\n\nRuns a mock server for testing and debugging external integrations\n\nPoolParty provides several integrations with external APIs/services (cf.\nSemantic Middleware Configurator). This command starts a mock server for\ndebugging/testing such integrations.\n\nThe port on which to run the server can be specified via --port. It defaults\nto 5000.\n\n##### Webhook consumer\nStarts a server and echoes any request (+ auxiliary information) coming in.\nIn addition starts a healthcheck endpoint that just always returns `200 OK`.\n\nThe webhook consumer url (to configure in Semantic Middleware Configurator)\nis `http://localhost:5000/hook`.\n\n``` bash\np3do pp mock-server\n```\n\n### kc\n\nCommands in this group allow to perform operations for Keycloak. Most of them\nneed authentication and server information. Please read [KC\nConfiguration](#kc-configuration) first on how to add your configuration.\n\nCommands:\n* [KC Configuration](#kc-configuration): Not a command but read this first!\n* [`add-mappers`](#add-mappers): Add mappers to IdPs from realm export\n\n#### KC Configuration\n\nkc commands usually need some information about the server, realm and\nauthentication. This information can be read from a configuration file, given\nvia CLI parameters or interactively if information is missing. CLI parameters\ntake precendence and override any configuration read from a configuration file.\n\n***Note:*** you don\'t need a configuration file at all. All (partial) parameters\ncan be specified via CLI arguments. Just leave out the `--auth_config` and\n`--auth` flags.\n\nA full configuration file which specifies all available options looks like this:\n\n```ini\n[test]\nserver=https://keycloak.example.com/auth/\nusername=admin\nuser_realm_name=master\npassword=password\nrealm_name=my-app\n```\n\n`[test]` is the name of the configuration. You can have multiple configurations\nfor different servers in your config file. `server`, `username`, `password` are\nrather self-explanatory. `user_realm_name` is the realm the _user_ is in. This\nis not necessarily the same realm as the one you want to modify. `realm_name` is\nthe realm name you want to modify (it usually does not make sense to put this\ninto the config file).\n\nTo specify the config file and config name you want to use, invoke a `p3do` command like this:\n\n```bash\n# `config.ini` is the config file, `test` is the config section you want to use\np3do kc add-mappers --auth_config config.ini --auth test <...other arguments...>\n```\n\nNote that you can override any configuration via CLI arguments:\n\n```bash\n# Override `admin` from `config.ini` with `admin2`\np3do kc add-mappers --auth_config config.ini --auth test --username admin2 <...other arguments...>\n```\n\nThe configuration can also be partial:\n```ini\n[partial-test]\nserver=https://keycloak.example.com/auth/\nusername=admin\nuser_realm_name=master\n```\n\nNote that we don\'t specify a `password` or `realm_name` here. You can now invoke `p3do` with\n\n```bash\n# Complete `partial-test` via arguments\np3do kc add-mappers --auth_config config.ini --auth partial-test --password password --realm_name my-other-app <...other arguments...>\n```\n\nYou can also just invoke `p3do` as before and will be asked interactively to fill out the missing pieces:\n\n```bash\n# No `password` or `realm_name` from `config.ini` or cli arguments\np3do kc add-mappers --auth_config config.ini --auth partial-test <...other arguments...>\n# `p3do` will ask you to complete them interactively\nPassword: password\nRealm_name: my-other-app\n```\n\n#### add-mappers\n\nAdd IdP mappers from a realm export `.json` to a realm. The IdP must already\nexist and correspond to the IdP name specified in the mapper config. Keycloak\ndoes not import mapper configuration by itself (yet?).\n\n```bash\n# `realm-export.json` is the path the the export file\np3do kc add-mappers --auth_config config.ini --auth test realm-export.json\n```\n\n## Contribute\n\n***`p3do` is licensed under MIT and published to PyPI (including source). Do not\nadd sensitive company data. Any sensitive data has to be read from external\nconfiguration files.***\n\n### Contributors\n\nAll contributions are welcome. This can be new commands, improvements to the\non-line help, documentation or spelling mistakes. Just open a PR with your\nchanges. If your changes are larger, you find a bug but don\'t know how to fix\nit, or you are just unsure if your idea fits, open an issue on GitHub first.\n\n### Maintainers\n\nThe `p3do` main branch is protected and PRs have to be approved by by\n[maintainers](CODEOWNERS) (code owners in GitHub lingo). Tooling like this can\neasily grow out of control. Maintainers ensure that this is not happening to\n`p3do`. Here are some guidelines.\n\n- Every command in `p3do` must have a well known and feasible (manual)\n  alternative\n- `p3do` must not smear over too complicated process. If a process is too\n  complicated fix the process.\n- `p3do` must not obfuscate processes. If knowledge about how things work isn\'t\n  spread enough, spread it.\n- `p3do` must not gatekeep processes. It is not a mechanism for access\n  management.\n- `p3do` believes in the competency of its users\n\n### Release Maintainers\n\nReleases are pushed to [PyPI](https://pypi.org/project/p3do/). This requires\na token with Maintainer or Owner status on PyPI.\n\nReleases are automatically created and pushed by a [GitHub\nAction](https://github.com/swc-friedla/p3do/actions/workflows/publish.yml) when\na tagged release is created in GitHub.\n\nRepository and release maintainers is probably but not necessarily the same set\nof people.\n',
-    'author': 'Armin Friedl',
-    'author_email': 'armin.friedl@semantic-web.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+[![PyPI - License](https://img.shields.io/pypi/l/p3do)](https://github.com/poolparty-semantic-suite/p3do/blob/main/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/p3do)](https://pypi.org/project/p3do/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/p3do)](https://www.python.org/)
+[![Publish](https://github.com/poolparty-semantic-suite/p3do/actions/workflows/publish.yml/badge.svg)](https://github.com/poolparty-semantic-suite/p3do/actions)
 
 
-setup(**setup_kwargs)
+p3do (pronounced _pee-three-duh_) is a collection of command-line utilities for
+p3d. It allows you to conjure some tedious operations right from your magic little
+fingertips.
+
+<img src="res/p3do-animation.gif?raw=true" alt="p3do in action" width="75%"/>
+
+<p />
+
+[Installation](#installation) •
+[Getting started](#getting-started) •
+[Commands](#commands) •
+[Contribute](#contribute)
+
+</div>
+
+## Installation
+<img src="res/p3do-logo.png?raw=true" alt="p3do logo" align="right" width="180px"/>
+
+`p3do` is built with Python 3.8 or later. You can get Python from your package
+manager du jour or download and install it from
+https://www.python.org/downloads/ (looking at you Windows. Mac.
+Whyihavetobother. Veryannoyingyouare.)
+
+`p3do` is published to the [CheeseShop](https://pypi.org/project/p3do/) and
+hence can be installed with pip:
+
+```bash
+pip install p3do
+```
+
+`p3do` installs itself as a command. If your `$PATH` is set up correctly you
+will be able to just invoke `p3do` like so
+
+```bash
+p3do --help
+```
+
+### Shell Completion
+
+`p3do` supports shell completion (tab completion). Shell completion is supported
+for bash, zsh and fish shells. For each of these, the autocompletion script is
+different.
+
+Bash 4.4 and later:
+``` bash
+# add to your ~/.bashrc
+eval "$(_P3DO_COMPLETE=bash_source p3do)"
+```
+
+Zsh:
+``` bash
+# add to your ~/.zshrc:
+eval "$(_P3DO_COMPLETE=zsh_source p3do)"
+```
+
+Fish:
+``` bash
+#  ~/.config/fish/completions/p3do.fish
+eval (env _P3DO_COMPLETE=fish_source p3do)
+```
+
+## Getting Started
+
+<img src="res/p3do-logo2.png?raw=true" alt="p3do logo" align="left" width="180px"/>
+
+Light a bonfire and whisper _p3do_ in the most conspirative voice available to
+you. Then start a terminal.
+
+`p3do` is hierarchical, self-documenting and discoverable. The best way to start
+is to just type `p3do`. This will show you the available commands and some
+description. From there you can drill down the hierarchy for useful sub-command.
+
+Each sub-command/command group has special flags and configuration. How to use
+them is explained in [Commands](#commands) for each of them separately. You can
+also use `p3d <group> <command> --help` in your terminal for concise on-line
+help.
+
+## Commands
+
+`p3do` is hierarchical. Commands are batched into groups which can be further
+nested into parent groups. We follow the same principle in the documentation
+here.
+
+* [`jk`](#jk): Jenkins commands
+    - [`build`](#build): Run the `P3D-BUILD` jenkins job with smart branch
+      detection
+    - [`deploy`](#deploy): Run the `P3D-Build-Deploy-PoolParty-(parent-pom)`
+      jenkins job with smart branch detection
+
+* [`pp`](#pp): PoolParty commands
+    - [`encrypt`](#encrypt): Encrypt a clear text with poolparty encryption
+    - [`decrypt`](#decrypt): Decrypt a secret text with poolparty encryption
+    - [`install-snapshot`](#install-snapshot): Download and run latest snapshot installer. Linux only.
+    - [`mock-server`](#mock-server): Run a mock server for debugging external
+      services integration (Semantic Middleware Configurator).
+
+* [`kc`](#kc): Keycloak commands
+    - [KC Configuration](#kc-configuration): Not a command but read this first!
+    - [`add-mappers`](#add-mappers): Add mappers to IdPs from realm export
+    
+* [`gh`](#gh): GitHub commands
+    - [`deploy-key`](#deploy-key): Add a deployment key to a GitHub repository
+
+### jk
+
+Commands in this group allow to perform common operations on Jenkins.
+
+#### build
+
+Start the `P3D-BUILD` job from the command line with smart branch detection.
+For this command `git` has to be installed.
+
+Per default (and outside a git repository) builds the `develop` branch of
+PoolParty.
+
+When inside a git repository p3do will automatically detect the current
+branch and build it. This behavior can be disabled with `--no-autodetect`.
+
+The branch to build can be specified via `--branch` (note that this implies
+`--no-autodetect` inside a git repository).
+
+With `--api-user` and `--api-key` you can specify the credentials accessing the
+Jenkins API. These credentials are cached and only need to be specified once. If
+not specified and no cached credentials are found, p3do will ask for them
+interactively. You can generate a token for `--api-key` in your [Jenkins Account
+Settings](https://ci2.semantic-web.at/user/<username>/configure). `--api-user`
+is the username you use to log in to Jenkins.
+
+``` bash
+# Build branch PoolParty develop without branch detection
+p3do jk build --branch develop
+```
+
+#### deploy
+
+Start the `P3D-Build-Deploy-PoolParty-(parent-pom)` job from the command line
+with smart branch detection. For this command `git` has to be installed.
+
+Per default (and outside a git repository) deploys the `develop` branch of
+PoolParty.
+
+When inside a git repository `p3do` will automatically detect the current branch
+and deploy it. This behavior can be disabled with --no-autodetect.
+
+The branch to deploy can be specified via --branch (note that this implies
+--no-autodetect inside a git repository).
+
+With `--api-user` and `--api-key` you can specify the credentials accessing the
+Jenkins API. These credentials are cached and only need to be specified once. If
+not specified and no cached credentials are found, p3do will ask for them
+interactively. You can generate a token for `--api-key` in your [Jenkins Account
+Settings](https://ci2.semantic-web.at/user/<username>/configure). `--api-user`
+is the username you use to log in to Jenkins.
+
+The `SERVER` argument is mandatory and must be a valid ssh server name.
+PoolParty will be deployed to this server.
+
+``` bash
+# Deploy PoolParty develop branch to pp-lazer-kittens-dev without branch detection
+p3do jk deploy --branch develop pp-lazer-kittens-dev
+```
+
+### pp
+
+Commands in this group allow to perform operations useful for or related to
+our dear PoolParty.
+
+#### encrypt
+
+Encrypt a clear text with PoolParty encryption. The parameters for encryption
+used by PoolParty can usually be found in the `poolparty.properties` file.
+
+This command can be used by specifying the encryption parameters directly as
+options to p3do (`--password`, `--salt`, `--strength`) or with an interactive
+prompt (just specify the clear text and leave out the options).
+
+To make sure that your command line processor does not mingle the input, always
+wrap the clear text, password, and salt it in quotes if you are passing them as
+options to p3do.
+
+For interactive prompt do _not_ wrap them in quotes.
+
+Interactive prompt:
+``` bash
+# encrypt mysecret with 
+# password H7dwBFDh3gEVDH1YecgikmOBpx9kKZ9nj1wJ5ZuhEeg=
+# salt Y+Fw/4dHBajqEGxOsEyfNSGsYYXE7JUyLmc3nRFrB84=
+# and 256 rounds
+p3do pp encrypt "mysecret"
+Password: H7dwBFDh3gEVDH1YecgikmOBpx9kKZ9nj1wJ5ZuhEeg= # interactive prompt
+Salt: Y+Fw/4dHBajqEGxOsEyfNSGsYYXE7JUyLmc3nRFrB84= # interactive prompt
+Strength: 256 # interactive prompt
+eYRLg0SUzGNSlfmS6MYrt8pnu5MTYU3EWVmNp1q/JFQ=
+```
+
+With options:
+``` bash
+# encrypt mysecret with 
+# password H7dwBFDh3gEVDH1YecgikmOBpx9kKZ9nj1wJ5ZuhEeg=
+# salt Y+Fw/4dHBajqEGxOsEyfNSGsYYXE7JUyLmc3nRFrB84=
+# and 256 rounds
+p3do pp encrypt --password "H7dwBFDh3gEVDH1YecgikmOBpx9kKZ9nj1wJ5ZuhEeg=" --salt "Y+Fw/4dHBajqEGxOsEyfNSGsYYXE7JUyLmc3nRFrB84=" --strength 256 "mysecret"
+```
+
+#### decrypt
+Decrypt a secret text encrypted by PoolParty. The parameters for encryption/decryption used
+by PoolParty can usually be found in the `poolparty.properties` file.
+
+This command can be used by specifying the encryption parameters directly as
+options to p3do (`--password`, `--salt`, `--strength`) or with an interactive
+prompt (just specify the clear text and leave out the options).
+
+To make sure that your command line processor does not mingle the input, always
+wrap the clear text, password, and salt it in quotes if you are passing them as
+options to p3do.
+
+For interactive prompt do _not_ wrap them in quotes.
+
+Interactive prompt:
+``` bash
+# decrypt 6NjzLmQp7kGM7bbezhQX1G2hrqCoqLrC32ayBTjQVjU= with 
+# password H7dwBFDh3gEVDH1YecgikmOBpx9kKZ9nj1wJ5ZuhEeg=
+# salt Y+Fw/4dHBajqEGxOsEyfNSGsYYXE7JUyLmc3nRFrB84=
+# and 256 rounds
+p3do pp decrypt "6NjzLmQp7kGM7bbezhQX1G2hrqCoqLrC32ayBTjQVjU="
+Password: H7dwBFDh3gEVDH1YecgikmOBpx9kKZ9nj1wJ5ZuhEeg= # interactive prompt
+Salt: Y+Fw/4dHBajqEGxOsEyfNSGsYYXE7JUyLmc3nRFrB84= # interactive prompt
+Strength: 256 # interactive prompt
+eYRLg0SUzGNSlfmS6MYrt8pnu5MTYU3EWVmNp1q/JFQ=
+```
+
+With options:
+``` bash
+# decrypt 6NjzLmQp7kGM7bbezhQX1G2hrqCoqLrC32ayBTjQVjU= with 
+# password H7dwBFDh3gEVDH1YecgikmOBpx9kKZ9nj1wJ5ZuhEeg=
+# salt Y+Fw/4dHBajqEGxOsEyfNSGsYYXE7JUyLmc3nRFrB84=
+# and 256 rounds
+p3do pp decrypt --password "H7dwBFDh3gEVDH1YecgikmOBpx9kKZ9nj1wJ5ZuhEeg=" --salt "Y+Fw/4dHBajqEGxOsEyfNSGsYYXE7JUyLmc3nRFrB84=" --strength 256 "6NjzLmQp7kGM7bbezhQX1G2hrqCoqLrC32ayBTjQVjU=" 
+```
+
+#### install-snapshot
+
+Download and invoke the latest snapshot installer. Specify `--path` to download
+the installer to a specific folder. Otherwise, the installer will be installed
+to a temporary directory. 
+
+This command is restricted to Linux for now.
+
+``` bash
+p3do pp install-snapshot
+```
+
+#### mock-server
+
+Runs a mock server for testing and debugging external integrations
+
+PoolParty provides several integrations with external APIs/services (cf.
+Semantic Middleware Configurator). This command starts a mock server for
+debugging/testing such integrations.
+
+The port on which to run the server can be specified via --port. It defaults
+to 5000.
+
+##### Webhook consumer
+Starts a server and echoes any request (+ auxiliary information) coming in.
+In addition starts a healthcheck endpoint that just always returns `200 OK`.
+
+The webhook consumer url (to configure in Semantic Middleware Configurator)
+is `http://localhost:5000/hook`.
+
+``` bash
+p3do pp mock-server
+```
+
+### kc
+
+Commands in this group allow to perform operations for Keycloak. Most of them
+need authentication and server information. Please read [KC
+Configuration](#kc-configuration) first on how to add your configuration.
+
+Commands:
+* [KC Configuration](#kc-configuration): Not a command but read this first!
+* [`add-mappers`](#add-mappers): Add mappers to IdPs from realm export
+
+#### KC Configuration
+
+kc commands usually need some information about the server, realm and
+authentication. This information can be read from a configuration file, given
+via CLI parameters or interactively if information is missing. CLI parameters
+take precendence and override any configuration read from a configuration file.
+
+***Note:*** you don't need a configuration file at all. All (partial) parameters
+can be specified via CLI arguments. Just leave out the `--auth_config` and
+`--auth` flags.
+
+A full configuration file which specifies all available options looks like this:
+
+```ini
+[test]
+server=https://keycloak.example.com/auth/
+username=admin
+user_realm_name=master
+password=password
+realm_name=my-app
+```
+
+`[test]` is the name of the configuration. You can have multiple configurations
+for different servers in your config file. `server`, `username`, `password` are
+rather self-explanatory. `user_realm_name` is the realm the _user_ is in. This
+is not necessarily the same realm as the one you want to modify. `realm_name` is
+the realm name you want to modify (it usually does not make sense to put this
+into the config file).
+
+To specify the config file and config name you want to use, invoke a `p3do` command like this:
+
+```bash
+# `config.ini` is the config file, `test` is the config section you want to use
+p3do kc add-mappers --auth_config config.ini --auth test <...other arguments...>
+```
+
+Note that you can override any configuration via CLI arguments:
+
+```bash
+# Override `admin` from `config.ini` with `admin2`
+p3do kc add-mappers --auth_config config.ini --auth test --username admin2 <...other arguments...>
+```
+
+The configuration can also be partial:
+```ini
+[partial-test]
+server=https://keycloak.example.com/auth/
+username=admin
+user_realm_name=master
+```
+
+Note that we don't specify a `password` or `realm_name` here. You can now invoke `p3do` with
+
+```bash
+# Complete `partial-test` via arguments
+p3do kc add-mappers --auth_config config.ini --auth partial-test --password password --realm_name my-other-app <...other arguments...>
+```
+
+You can also just invoke `p3do` as before and will be asked interactively to fill out the missing pieces:
+
+```bash
+# No `password` or `realm_name` from `config.ini` or cli arguments
+p3do kc add-mappers --auth_config config.ini --auth partial-test <...other arguments...>
+# `p3do` will ask you to complete them interactively
+Password: password
+Realm_name: my-other-app
+```
+
+#### add-mappers
+
+Add IdP mappers from a realm export `.json` to a realm. The IdP must already
+exist and correspond to the IdP name specified in the mapper config. Keycloak
+does not import mapper configuration by itself (yet?).
+
+```bash
+# `realm-export.json` is the path the the export file
+p3do kc add-mappers --auth_config config.ini --auth test realm-export.json
+```
+
+### gh
+
+Commands in this group allow to perform operations on GitHub
+`poolparty-semantic-suite` organization. Most operations need an access token.
+This can be generated in GitHub user settings
+https://github.com/settings/tokens.
+
+Commands:
+* [`deploy-key`](#deploy-key): Add a deployment key to a GitHub repository
+
+#### deploy-key
+
+Add a deployment key to a GitHub repository.
+
+## Contribute
+
+***`p3do` is licensed under MIT and published to PyPI (including source). Do not
+add sensitive company data. Any sensitive data has to be read from external
+configuration files.***
+
+### Contributors
+
+All contributions are welcome. This can be new commands, improvements to the
+on-line help, documentation or spelling mistakes. Just open a PR with your
+changes. If your changes are larger, you find a bug but don't know how to fix
+it, or you are just unsure if your idea fits, open an issue on GitHub first.
+
+### Maintainers
+
+The `p3do` main branch is protected and PRs have to be approved by by
+[maintainers](CODEOWNERS) (code owners in GitHub lingo). Tooling like this can
+easily grow out of control. Maintainers ensure that this is not happening to
+`p3do`. Here are some guidelines.
+
+- Every command in `p3do` must have a well known and feasible (manual)
+  alternative
+- `p3do` must not smear over too complicated process. If a process is too
+  complicated fix the process.
+- `p3do` must not obfuscate processes. If knowledge about how things work isn't
+  spread enough, spread it.
+- `p3do` must not gatekeep processes. It is not a mechanism for access
+  management.
+- `p3do` believes in the competency of its users
+
+### Release Maintainers
+
+Releases are pushed to [PyPI](https://pypi.org/project/p3do/). This requires
+a token with Maintainer or Owner status on PyPI.
+
+Releases are automatically created and pushed by a [GitHub
+Action](https://github.com/swc-friedla/p3do/actions/workflows/publish.yml) when
+a tagged release is created in GitHub.
+
+Repository and release maintainers is probably but not necessarily the same set
+of people.
+
```

