# Comparing `tmp/thipstercli-0.1.3.tar.gz` & `tmp/thipstercli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipstercli-0.1.3.tar", last modified: Tue Jun 13 10:34:32 2023, max compression
+gzip compressed data, was "thipstercli-0.2.0.tar", last modified: Thu Jun 15 08:38:45 2023, max compression
```

## Comparing `thipstercli-0.1.3.tar` & `thipstercli-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:34:32.495290 thipstercli-0.1.3/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-13 10:34:29.000000 thipstercli-0.1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3486 2023-06-13 10:34:32.495290 thipstercli-0.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2798 2023-06-13 10:34:29.000000 thipstercli-0.1.3/README.md
--rw-r--r--   0 root         (0) root         (0)      919 2023-06-13 10:34:29.000000 thipstercli-0.1.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 10:34:32.495290 thipstercli-0.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1642 2023-06-13 10:34:30.000000 thipstercli-0.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:34:32.491290 thipstercli-0.1.3/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 10:34:29.000000 thipstercli-0.1.3/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2673 2023-06-13 10:34:29.000000 thipstercli-0.1.3/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     1273 2023-06-13 10:34:29.000000 thipstercli-0.1.3/tests/test_providers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:34:32.495290 thipstercli-0.1.3/thipstercli/
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-13 10:34:29.000000 thipstercli-0.1.3/thipstercli/__init__.py
--rw-r--r--   0 root         (0) root         (0)       58 2023-06-13 10:34:29.000000 thipstercli-0.1.3/thipstercli/__main__.py
--rw-r--r--   0 root         (0) root         (0)     3662 2023-06-13 10:34:29.000000 thipstercli-0.1.3/thipstercli/cli.py
--rw-r--r--   0 root         (0) root         (0)      321 2023-06-13 10:34:29.000000 thipstercli-0.1.3/thipstercli/helpers.py
--rw-r--r--   0 root         (0) root         (0)     2772 2023-06-13 10:34:29.000000 thipstercli-0.1.3/thipstercli/providers.py
--rw-r--r--   0 root         (0) root         (0)      520 2023-06-13 10:34:29.000000 thipstercli-0.1.3/thipstercli/state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:34:32.495290 thipstercli-0.1.3/thipstercli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3486 2023-06-13 10:34:32.000000 thipstercli-0.1.3/thipstercli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      449 2023-06-13 10:34:32.000000 thipstercli-0.1.3/thipstercli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 10:34:32.000000 thipstercli-0.1.3/thipstercli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-06-13 10:34:32.000000 thipstercli-0.1.3/thipstercli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      189 2023-06-13 10:34:32.000000 thipstercli-0.1.3/thipstercli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-13 10:34:32.000000 thipstercli-0.1.3/thipstercli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:38:45.799937 thipstercli-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-15 08:38:42.000000 thipstercli-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4040 2023-06-15 08:38:45.799937 thipstercli-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3352 2023-06-15 08:38:42.000000 thipstercli-0.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      919 2023-06-15 08:38:42.000000 thipstercli-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 08:38:45.799937 thipstercli-0.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1642 2023-06-15 08:38:43.000000 thipstercli-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:38:45.795937 thipstercli-0.2.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 08:38:42.000000 thipstercli-0.2.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2023-06-15 08:38:42.000000 thipstercli-0.2.0/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     3195 2023-06-15 08:38:42.000000 thipstercli-0.2.0/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     2156 2023-06-15 08:38:42.000000 thipstercli-0.2.0/tests/test_providers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:38:45.799937 thipstercli-0.2.0/thipstercli/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-15 08:38:42.000000 thipstercli-0.2.0/thipstercli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       58 2023-06-15 08:38:42.000000 thipstercli-0.2.0/thipstercli/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     4848 2023-06-15 08:38:42.000000 thipstercli-0.2.0/thipstercli/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-06-15 08:38:42.000000 thipstercli-0.2.0/thipstercli/config.py
+-rw-r--r--   0 root         (0) root         (0)      256 2023-06-15 08:38:42.000000 thipstercli-0.2.0/thipstercli/constants.py
+-rw-r--r--   0 root         (0) root         (0)      696 2023-06-15 08:38:42.000000 thipstercli-0.2.0/thipstercli/display.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-06-15 08:38:42.000000 thipstercli-0.2.0/thipstercli/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2023-06-15 08:38:42.000000 thipstercli-0.2.0/thipstercli/providers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:38:45.799937 thipstercli-0.2.0/thipstercli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4040 2023-06-15 08:38:45.000000 thipstercli-0.2.0/thipstercli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      516 2023-06-15 08:38:45.000000 thipstercli-0.2.0/thipstercli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 08:38:45.000000 thipstercli-0.2.0/thipstercli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-06-15 08:38:45.000000 thipstercli-0.2.0/thipstercli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2023-06-15 08:38:45.000000 thipstercli-0.2.0/thipstercli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-15 08:38:45.000000 thipstercli-0.2.0/thipstercli.egg-info/top_level.txt
```

### Comparing `thipstercli-0.1.3/LICENSE` & `thipstercli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thipstercli-0.1.3/PKG-INFO` & `thipstercli-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: thipstercli
-Version: 0.1.3
-Summary: CLI interface build with typer, designed to use the thipster package
-Home-page: https://github.com/THipster/THipster-cli
-Download-URL: https://github.com/THipster/THipster-cli.git
-License: MIT
-Keywords: thipster,cli,generator,infrastructure as code,iac,terraform,typer
-Classifier: Development Status :: 1 - Planning
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: dev
-Provides-Extra: doc
-License-File: LICENSE
-
 # THipster CLI
 
 CLI tool to interact and use [THipster](https://github.com/THipster/THipster), build with [Typer](https://typer.tiangolo.com/).
 
 THipster is a tool dedicated to simplifying the ordeal associated with writing Terraform files.
 It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 
@@ -43,14 +24,33 @@
 
 ```bash
 pip install thipstercli
 ```
 
 The list of available versions can be found on [PyPI](https://pypi.org/project/thipstercli/).
 
+### Configuration
+
+The CLI can be configured using a configuration file. A default `config.json` file will be created in the `/home/<user>/.config/thipstercli` directory the first time the CLI is used.
+
+Example of a configuration file:
+```json
+{
+    "app_name": "thipstercli",
+    "auth_provider": "google",
+    "input_dir": ".",
+    "local_models_repository_path": "models",
+    "models_repository": "THipster/models",
+    "models_repository_branch": "main",
+    "models_repository_provider": "local",
+    "output_dir": ".",
+    "verbose": false
+}
+```
+
 ## Usage
 
 The cli is composed of 3 main commands:
 - `version`: display the current version of the package
 ```bash
 thipster version -t
 ```
```

### Comparing `thipstercli-0.1.3/README.md` & `thipstercli-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: thipstercli
+Version: 0.2.0
+Summary: CLI interface build with typer, designed to use the thipster package
+Home-page: https://github.com/THipster/THipster-cli
+Download-URL: https://github.com/THipster/THipster-cli.git
+License: MIT
+Keywords: thipster,cli,generator,infrastructure as code,iac,terraform,typer
+Classifier: Development Status :: 1 - Planning
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: dev
+Provides-Extra: doc
+License-File: LICENSE
+
 # THipster CLI
 
 CLI tool to interact and use [THipster](https://github.com/THipster/THipster), build with [Typer](https://typer.tiangolo.com/).
 
 THipster is a tool dedicated to simplifying the ordeal associated with writing Terraform files.
 It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 
@@ -24,14 +43,33 @@
 
 ```bash
 pip install thipstercli
 ```
 
 The list of available versions can be found on [PyPI](https://pypi.org/project/thipstercli/).
 
+### Configuration
+
+The CLI can be configured using a configuration file. A default `config.json` file will be created in the `/home/<user>/.config/thipstercli` directory the first time the CLI is used.
+
+Example of a configuration file:
+```json
+{
+    "app_name": "thipstercli",
+    "auth_provider": "google",
+    "input_dir": ".",
+    "local_models_repository_path": "models",
+    "models_repository": "THipster/models",
+    "models_repository_branch": "main",
+    "models_repository_provider": "local",
+    "output_dir": ".",
+    "verbose": false
+}
+```
+
 ## Usage
 
 The cli is composed of 3 main commands:
 - `version`: display the current version of the package
 ```bash
 thipster version -t
 ```
```

### Comparing `thipstercli-0.1.3/pyproject.toml` & `thipstercli-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipstercli-0.1.3/setup.py` & `thipstercli-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = '0.1.3'
+__version__ = '0.2.0'
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 with open('README.md') as f:
     long_description = f.read()
```

### Comparing `thipstercli-0.1.3/tests/test_cli.py` & `thipstercli-0.2.0/tests/test_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from importlib.metadata import version as get_version
 
 from typer.testing import CliRunner
-
+from thipstercli.config import state
 from thipstercli.cli import app
 
 AUTH_FILE_PATH = 'tests/credentials.json'
 
 runner = CliRunner(mix_stderr=False)
 
 
@@ -87,7 +87,25 @@
             '-l', 'tests/resources/models',
         ],
     )
 
     assert result.exit_code == 0
     assert 'thipster_cli_test_bucket' in result.output
     assert 'Terraform will perform the following actions' in result.output
+
+
+def test_config_file_verbose(config_file):
+    _ = config_file
+    runner.invoke(app, ['--help'])
+    assert state.get('verbose', False) is True
+
+
+def test_config_file_input_dir(config_file):
+    _ = config_file
+    runner.invoke(app, ['--help'])
+    assert state.get('input_dir', None) == 'test/input_directory'
+
+
+def test_config_file_output_dir(config_file):
+    _ = config_file
+    runner.invoke(app, ['--help'])
+    assert state.get('output_dir', None) == 'test/output_directory'
```

### Comparing `thipstercli-0.1.3/tests/test_providers.py` & `thipstercli-0.2.0/tests/test_providers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from .conftest import get_config_file
 from typer.testing import CliRunner
-from thipstercli.state import state
-from thipstercli.providers import app, get_provider_class, check_provider_exists
+from thipstercli.config import state
+from thipstercli.helpers import get_auth_provider_class
+from thipstercli.providers import app, check_provider_exists
 
 runner = CliRunner(mix_stderr=False)
 
 providers = [
     'google',
 ]
 
@@ -19,28 +21,54 @@
 def test_info_provider():
     result = runner.invoke(app, ['info', 'google'])
     assert result.exit_code == 0
     assert 'google' in result.stdout.lower()
     assert 'gcloud' in result.stdout.lower()
 
 
+def test_info_provider_not_found():
+    result = runner.invoke(app, ['info', 'notfound'])
+    assert result.exit_code == 1
+    assert 'provider notfound not found.' in result.stdout.lower()
+
+
 def test_set_provider():
     result = runner.invoke(app, ['set', 'google'])
     assert result.exit_code == 0
     assert 'google' in result.stdout.lower()
     assert 'provider set to' in result.stdout.lower()
 
+
+def test_set_provider_not_found():
+    result = runner.invoke(app, ['set', 'notfound'])
+    assert result.exit_code == 1
+    assert 'provider notfound not found.' in result.stdout.lower()
+
+
+def test_display_provider(config_file):
+    _ = config_file
     result = runner.invoke(app, ['display'])
     assert result.exit_code == 0
-    assert 'google' in result.stdout.lower()
     assert 'provider set to' in result.stdout.lower()
+    assert 'google' in result.stdout.lower()
 
 
 def test_get_provider_class():
-    provider = get_provider_class('Google')
+    provider = get_auth_provider_class('Google')
     assert provider.__name__ == 'GoogleAuth'
 
 
 def test_check_provider_exists():
-    state['providers'] = ['Google.py']
     provider = check_provider_exists('google')
-    assert provider == 'Google'
+    assert provider == 'google'
+
+
+def test_set_provider_config_file(config_file_wrong_provider):
+    _ = config_file_wrong_provider
+    runner.invoke(app, ['set', 'google'])
+    assert get_config_file().get('auth_provider', None) == 'google'
+
+
+def test_wrong_provider_config_file(config_file_wrong_provider):
+    _ = config_file_wrong_provider
+    runner.invoke(app, ['--help'])
+    assert state.get('auth_provider', None) is None
```

### Comparing `thipstercli-0.1.3/thipstercli/cli.py` & `thipstercli-0.2.0/thipstercli/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 import typer
+import thipstercli.constants as constants
 from rich import print
 from thipster import Engine as ThipsterEngine
 from thipster.auth import Google
 from thipster.parser import ParserFactory
 from thipster.repository import GithubRepo, LocalRepo
 from thipster.terraform import Terraform
 from thipster.engine.exceptions import THipsterException
 
 from thipstercli import providers
-from thipstercli.helpers import (
+from thipstercli.display import (
     error,
     print_if_verbose,
+    print_package_version,
+    print_start_if_verbose,
+    print_success_if_verbose,
 )
-from thipstercli.state import init_state, state
+from thipstercli.config import init_parameters, state
 
-init_state()
-app = typer.Typer(name=state['app_name'], no_args_is_help=True)
+init_parameters()
+
+app = typer.Typer(
+    name=state.get(
+        'app_name', constants.APP_NAME,
+    ), no_args_is_help=True,
+)
 app.add_typer(providers.app, name='providers')
 
 
 @app.callback()
 def _callback(
     verbose: bool = typer.Option(
-        False,
+        state.get('verbose', constants.VERBOSE),
         '--verbose', '-v',
         help='Prints more information about the execution of the THipster CLI',
     ),
 ):
     """THipster CLI
 
     THipster is a tool that allows you to generate Terraform code
@@ -41,33 +50,52 @@
         False,
         '--thipster', '-t',
         help='Prints the version of the THipster tool',
     ),
 ):
     """Prints the version of the THipster CLI
     """
-    print(f"{state['app_name']}")
+    print_package_version('thipstercli')
 
     if thipster:
-        print(
-            f":bookmark: THipster [green]v{state['thipster_version']}[/green]",
-        )
+        print_package_version('thipster')
 
 
 @app.command('run')
 def _run(
     path: str = typer.Argument(
-        '.',
+        state.get('input_dir', constants.INPUT_DIR),
         help='Path to the file or directory to run',
     ),
     local: str = typer.Option(
         None,
         '--local', '-l',
         help='Runs the THipster Tool locally, importing models from the given path',
     ),
+    repository_provider: str = typer.Option(
+        state.get(
+            'models_repository_provider',
+            constants.MODELS_REPOSITORY_PROVIDER,
+        ),
+        '--repository-provider', '-rp',
+        help='Runs the THipster Tool using the given model repository provider',
+    ),
+    repository: str = typer.Option(
+        state.get('models_repository', constants.MODELS_REPOSITORY),
+        '--repository-name', '-rn',
+        help='Runs the THipster Tool using the given model repository',
+    ),
+    repository_branch: str = typer.Option(
+        state.get(
+            'models_repository_branch',
+            constants.MODELS_REPOSITORY_BRANCH,
+        ),
+        '--repository-branch', '-rb',
+        help='Runs the THipster Tool using the given model repository branch',
+    ),
     provider: str = typer.Option(
         None,
         '--provider', '-p',
         help='Runs the THipster Tool using the given provider',
     ),
     apply: bool = typer.Option(
         False,
@@ -75,50 +103,54 @@
         help='Applies the generated Terraform code',
     ),
 ):
     """Runs the THipster Tool on the given path
     """
     print_if_verbose(f'Running THipster on {path}')
 
-    authentification_provider = providers.get_provider_class(
+    authentification_provider = providers.get_auth_provider_class(
         providers.check_provider_exists(provider),
     ) if provider else Google
 
     print_if_verbose(
         f'Provider Auth set to [green]{authentification_provider.__name__}[/green]',
     )
 
     repo = LocalRepo(local) if local else GithubRepo(
-        state['github_repo'], state['github_repo_branch'],
+        repository,
+        repository_branch,
     )
     print_if_verbose('Repo set-up successful! :memo:')
 
     engine = ThipsterEngine(
         ParserFactory(),
         repo,
         authentification_provider,
         Terraform(),
     )
     print_if_verbose('Engine start-up successful! :rocket:')
 
-    print_if_verbose('Parsing files...')
-
     try:
+        print_start_if_verbose('Parsing files')
         parsed_file = engine._parse_files(path)
-        print_if_verbose('Parsing successful! :white_check_mark:')
+        print_success_if_verbose('Parsing successful!')
 
+        print_start_if_verbose('Retrieving models')
         models = engine._get_models(parsed_file)
-        print_if_verbose('Models retrieved! :white_check_mark:')
+        print_success_if_verbose('Models retrieved!')
 
+        print_start_if_verbose('Generating Terraform files')
         engine._generate_tf_files(parsed_file, models)
-        print_if_verbose('Terraform files generated! :white_check_mark:')
+        print_success_if_verbose('Terraform files generated!')
 
+        print_start_if_verbose('Initializing Terraform')
         engine._init_terraform()
-        print_if_verbose('Terraform initialized! :white_check_mark:')
+        print_success_if_verbose('Terraform initialized!')
 
+        print_start_if_verbose('Creating Terraform plan')
         print(engine._plan_terraform())
 
         if apply:
             print("Type 'yes' to apply the changes : ")
             print(engine._apply_terraform())
 
         print_if_verbose('Done! :tada:')
```

### Comparing `thipstercli-0.1.3/thipstercli.egg-info/PKG-INFO` & `thipstercli-0.2.0/thipstercli.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipstercli
-Version: 0.1.3
+Version: 0.2.0
 Summary: CLI interface build with typer, designed to use the thipster package
 Home-page: https://github.com/THipster/THipster-cli
 Download-URL: https://github.com/THipster/THipster-cli.git
 License: MIT
 Keywords: thipster,cli,generator,infrastructure as code,iac,terraform,typer
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
@@ -43,14 +43,33 @@
 
 ```bash
 pip install thipstercli
 ```
 
 The list of available versions can be found on [PyPI](https://pypi.org/project/thipstercli/).
 
+### Configuration
+
+The CLI can be configured using a configuration file. A default `config.json` file will be created in the `/home/<user>/.config/thipstercli` directory the first time the CLI is used.
+
+Example of a configuration file:
+```json
+{
+    "app_name": "thipstercli",
+    "auth_provider": "google",
+    "input_dir": ".",
+    "local_models_repository_path": "models",
+    "models_repository": "THipster/models",
+    "models_repository_branch": "main",
+    "models_repository_provider": "local",
+    "output_dir": ".",
+    "verbose": false
+}
+```
+
 ## Usage
 
 The cli is composed of 3 main commands:
 - `version`: display the current version of the package
 ```bash
 thipster version -t
 ```
```

