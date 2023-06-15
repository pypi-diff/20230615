# Comparing `tmp/secureli-0.3.9.tar.gz` & `tmp/secureli-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secureli-0.3.9.tar", max compression
+gzip compressed data, was "secureli-0.4.0.tar", max compression
```

## Comparing `secureli-0.3.9.tar` & `secureli-0.4.0.tar`

### file list

```diff
@@ -1,48 +1,50 @@
--rw-r--r--   0        0        0    11343 2023-06-07 19:55:25.814880 secureli-0.3.9/LICENSE
--rw-r--r--   0        0        0    10572 2023-06-07 19:55:25.814880 secureli-0.3.9/README.md
--rw-r--r--   0        0        0     1911 2023-06-07 19:55:25.814880 secureli-0.3.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/abstractions/__init__.py
--rw-r--r--   0        0        0     3919 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/abstractions/echo.py
--rw-r--r--   0        0        0      550 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/abstractions/lexer_guesser.py
--rw-r--r--   0        0        0    30306 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/abstractions/pre_commit.py
--rw-r--r--   0        0        0        0 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/actions/__init__.py
--rw-r--r--   0        0        0    10730 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/actions/action.py
--rw-r--r--   0        0        0      761 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/actions/build.py
--rw-r--r--   0        0        0     1160 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/actions/initializer.py
--rw-r--r--   0        0        0    10484 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/actions/scan.py
--rw-r--r--   0        0        0      791 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/actions/setup.py
--rw-r--r--   0        0        0     2087 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/actions/update.py
--rw-r--r--   0        0        0     6165 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/container.py
--rw-r--r--   0        0        0     2807 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/main.py
--rw-r--r--   0        0        0        0 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/repositories/__init__.py
--rw-r--r--   0        0        0     3685 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/repositories/repo_files.py
--rw-r--r--   0        0        0     1752 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/repositories/secureli_config.py
--rw-r--r--   0        0        0     3926 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/repositories/settings.py
--rw-r--r--   0        0        0       59 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/resources/__init__.py
--rw-r--r--   0        0        0     4883 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/resources/files/build.txt
--rw-r--r--   0        0        0     1271 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/resources/files/csharp-pre-commit.yaml
--rw-r--r--   0        0        0      461 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/resources/files/epilog.md
--rw-r--r--   0        0        0      619 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/resources/files/java-pre-commit.yaml
--rw-r--r--   0        0        0     1151 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/resources/files/python-pre-commit.yaml
--rw-r--r--   0        0        0      356 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/resources/files/secrets_detecting_repos.yaml
--rw-r--r--   0        0        0      409 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/resources/files/swift-pre-commit.yaml
--rw-r--r--   0        0        0      433 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/resources/files/terraform-pre-commit.yaml
--rw-r--r--   0        0        0      642 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/resources/files/typescript-pre-commit.yaml
--rw-r--r--   0        0        0      817 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/resources/read_resource.py
--rw-r--r--   0        0        0     1325 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/resources/slugify.py
--rw-r--r--   0        0        0        0 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/services/__init__.py
--rw-r--r--   0        0        0     3646 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/services/git_ignore.py
--rw-r--r--   0        0        0     3505 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/services/language_analyzer.py
--rw-r--r--   0        0        0     2211 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/services/language_support.py
--rw-r--r--   0        0        0     4413 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/services/logging.py
--rw-r--r--   0        0        0     6374 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/services/scanner.py
--rw-r--r--   0        0        0     1180 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/services/secureli_ignore.py
--rw-r--r--   0        0        0     3074 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/services/updater.py
--rw-r--r--   0        0        0     1482 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/settings.py
--rw-r--r--   0        0        0        0 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/utilities/__init__.py
--rw-r--r--   0        0        0     1080 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/utilities/git_meta.py
--rw-r--r--   0        0        0     1372 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/utilities/patterns.py
--rw-r--r--   0        0        0      198 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/utilities/secureli_meta.py
--rw-r--r--   0        0        0      587 2023-06-07 19:55:25.814880 secureli-0.3.9/secureli/utilities/usage_stats.py
--rw-r--r--   0        0        0    11409 1970-01-01 00:00:00.000000 secureli-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-06-15 19:40:09.872930 secureli-0.4.0/LICENSE
+-rw-r--r--   0        0        0    11614 2023-06-15 19:40:09.872930 secureli-0.4.0/README.md
+-rw-r--r--   0        0        0     2043 2023-06-15 19:40:09.876930 secureli-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/abstractions/__init__.py
+-rw-r--r--   0        0        0     3919 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/abstractions/echo.py
+-rw-r--r--   0        0        0      550 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/abstractions/lexer_guesser.py
+-rw-r--r--   0        0        0    34250 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/abstractions/pre_commit.py
+-rw-r--r--   0        0        0        0 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/actions/__init__.py
+-rw-r--r--   0        0        0    10730 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/actions/action.py
+-rw-r--r--   0        0        0      761 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/actions/build.py
+-rw-r--r--   0        0        0     1160 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/actions/initializer.py
+-rw-r--r--   0        0        0    10628 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/actions/scan.py
+-rw-r--r--   0        0        0      791 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/actions/setup.py
+-rw-r--r--   0        0        0     2087 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/actions/update.py
+-rw-r--r--   0        0        0     6165 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/container.py
+-rw-r--r--   0        0        0     2807 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/main.py
+-rw-r--r--   0        0        0        0 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/repositories/__init__.py
+-rw-r--r--   0        0        0     3685 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/repositories/repo_files.py
+-rw-r--r--   0        0        0     1752 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/repositories/secureli_config.py
+-rw-r--r--   0        0        0     3926 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/repositories/settings.py
+-rw-r--r--   0        0        0       59 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/resources/__init__.py
+-rw-r--r--   0        0        0     4883 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/resources/files/build.txt
+-rw-r--r--   0        0        0       93 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/resources/files/configs/javascript.config.yaml
+-rw-r--r--   0        0        0     1271 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/resources/files/csharp-pre-commit.yaml
+-rw-r--r--   0        0        0      461 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/resources/files/epilog.md
+-rw-r--r--   0        0        0      619 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/resources/files/java-pre-commit.yaml
+-rw-r--r--   0        0        0     1361 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/resources/files/javascript-pre-commit.yaml
+-rw-r--r--   0        0        0     1151 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/resources/files/python-pre-commit.yaml
+-rw-r--r--   0        0        0      356 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/resources/files/secrets_detecting_repos.yaml
+-rw-r--r--   0        0        0      409 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/resources/files/swift-pre-commit.yaml
+-rw-r--r--   0        0        0      433 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/resources/files/terraform-pre-commit.yaml
+-rw-r--r--   0        0        0      642 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/resources/files/typescript-pre-commit.yaml
+-rw-r--r--   0        0        0      817 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/resources/read_resource.py
+-rw-r--r--   0        0        0     1325 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/resources/slugify.py
+-rw-r--r--   0        0        0        0 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/services/__init__.py
+-rw-r--r--   0        0        0     3646 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/services/git_ignore.py
+-rw-r--r--   0        0        0     3505 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/services/language_analyzer.py
+-rw-r--r--   0        0        0     2225 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/services/language_support.py
+-rw-r--r--   0        0        0     4413 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/services/logging.py
+-rw-r--r--   0        0        0     6374 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/services/scanner.py
+-rw-r--r--   0        0        0     1180 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/services/secureli_ignore.py
+-rw-r--r--   0        0        0     3074 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/services/updater.py
+-rw-r--r--   0        0        0     1482 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/settings.py
+-rw-r--r--   0        0        0        0 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/utilities/__init__.py
+-rw-r--r--   0        0        0     1080 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/utilities/git_meta.py
+-rw-r--r--   0        0        0     1372 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/utilities/patterns.py
+-rw-r--r--   0        0        0      198 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/utilities/secureli_meta.py
+-rw-r--r--   0        0        0     1028 2023-06-15 19:40:09.876930 secureli-0.4.0/secureli/utilities/usage_stats.py
+-rw-r--r--   0        0        0    12494 1970-01-01 00:00:00.000000 secureli-0.4.0/PKG-INFO
```

### Comparing `secureli-0.3.9/LICENSE` & `secureli-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/README.md` & `secureli-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -61,14 +61,31 @@
 When invoking these commands, you can combine the short versions into a single flag. For example, the following commands are equivalent:
 
 ```python
 % secureli init --reset --yes
 % secureli init -ry
 ```
 
+# Tutorial to Use Observability Platform to Show Usage Statistics
+
+This tutorial uses New Relic as the sample observability platform. Other platforms may also work, but have not been tested.
+Should you need seCureLI to work with other platforms, please create a new issue in github, or contribute to the open source project.
+
+## Steps
+
+- Assuming, seCureLI has been setup and installed, sign up to New Relic Log Platform https://docs.newrelic.com/docs/logs/log-api/introduction-log-api/
+- Retrieve API_KEY and API_ENDPOINT from New Relic. API_ENDPOINT for New Relic should be https://log-api.newrelic.com/log/v1
+- On your development machine, setup environment variable with variable name API_KEY and API_ENDPOINT
+- Once the above setup is complete, everytime seCureLI triggered, it should send a usage log to New Relic
+- In New Relic, you can create a dashboard of metric to see the number of times secret was caught using query such as
+
+```commandline
+FROM Log Select sum(failure_count_details.detect_secrets) as 'Caught Secret Count'
+```
+
 # Configuration
 
 SeCureLI is configurable via a .secureli.yaml file present in the consuming repository.
 
 ## .secureli.yaml - top level
 
 | Key                | Description                                                                                                                      |
```

### Comparing `secureli-0.3.9/pyproject.toml` & `secureli-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 [tool.poetry]
 name = "secureli"
-version = "0.3.9"
+version = "0.4.0"
 description = "Secure Project Manager"
 authors = ["Caleb Tonn <caleb.tonn@slalom.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 secureli = "secureli.main:app"
 
 [tool.poe.tasks]
 coverage = ["test", "coverage_report"]
 coverage_report = "coverage report"
 coverage_run = "coverage run -m pytest"
+coverage_html = "coverage html"
 docker-build-app = "docker build -t secureli . -f Dockerfile_secureli --progress=plain --no-cache"
 docker-build-homebrew = "docker build -t homebrew . -f Dockerfile_homebrew --no-cache --progress=plain"
 docker-build-pypi = "docker build -t pypi . -f Dockerfile_pypi --no-cache --progress=plain"
 init = ["install", "secureli_init"]
 secureli_init = "secureli init -y"
 install = "poetry install"
 lint = "black --check ."
 precommit = "pre-commit run -a"
-test = ["init", "lint", "coverage_run"]
+test = ["init", "lint", "coverage_run", "coverage_html"]
+e2e = "bats tests/end-to-end/test.bats"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-typer = {version = "^0.6.1", extras = ["all"]}
+typer = {version = ">=0.6.1,<0.10.0", extras = ["all"]}
 pygments = "^2.13.0"
 dependency-injector = {version = "^4.40.0", extras = ["yaml"]}
 pydantic = "^1.10.2"
 jinja2 = "^3.1.2"
-pathspec = "^0.10.1"
+pathspec = ">=0.10.1,<0.12.0"
 cfgv = "^3.3.1"
 pre-commit = ">=2.20,<4.0"
+requests = "^2.31.0"
 
 [tool.pytest.ini_options]
 addopts = "-p no:cacheprovider"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 pytest-mock = "^3.10.0"
-coverage = "^6.5.0"
+coverage = ">=6.5,<8.0"
 black = ">=22.10,<24.0"
 identify = "^2.5.7"
 poethepoet = ">=0.16.4,<0.21.0"
 python-semantic-release = "^7.33.1"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `secureli-0.3.9/secureli/abstractions/echo.py` & `secureli-0.4.0/secureli/abstractions/echo.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/abstractions/lexer_guesser.py` & `secureli-0.4.0/secureli/abstractions/lexer_guesser.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/abstractions/pre_commit.py` & `secureli-0.4.0/secureli/abstractions/pre_commit.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,24 +27,45 @@
 
 class LanguageNotSupportedError(Exception):
     """The given language was not supported by the PreCommitHooks abstraction"""
 
     pass
 
 
-class LanguagePreCommitConfig(pydantic.BaseModel):
+class InstallLanguageConfigError(Exception):
+    """Attempting to install language specific config to .secureli was not successful"""
+
+    pass
+
+
+class LanguagePreCommitInstallResult(pydantic.BaseModel):
     """
     A configuration model for a supported pre-commit-configurable language.
     """
 
     language: str
     config_data: str
     version: str
 
 
+class LanguagePreCommitConfigInstallResult(pydantic.BaseModel):
+    """Results from installing langauge specific configs for pre-commit hooks"""
+
+    num_successful: int
+    num_non_success: int
+    non_success_messages: list[str]
+
+
+class LoadLanguageConfigsResult(pydantic.BaseModel):
+    """Results from finding and loading any pre-commit configs for the language"""
+
+    success: bool
+    config_data: list[Any]
+
+
 class UnexpectedReposResult(pydantic.BaseModel):
     """
     The result of checking for unexpected repos in config
     """
 
     missing_repos: Optional[list[str]] = []
     unexpected_repos: Optional[list[str]] = []
@@ -62,14 +83,15 @@
 class InstallResult(pydantic.BaseModel):
     """
     The results of calling install
     """
 
     successful: bool
     version_installed: str
+    configs_result: LanguagePreCommitConfigInstallResult
 
 
 class ValidateConfigResult(pydantic.BaseModel):
     """
     The results of calling validate_config
     """
 
@@ -185,15 +207,21 @@
 
         completed_process = subprocess.run(["pre-commit", "install"])
         if completed_process.returncode != 0:
             raise InstallFailedError(
                 f"Installing the pre-commit script for {language} failed"
             )
 
-        return InstallResult(successful=True, version_installed=language_config.version)
+        install_configs_result = self._install_pre_commit_configs(language)
+
+        return InstallResult(
+            successful=True,
+            version_installed=language_config.version,
+            configs_result=install_configs_result,
+        )
 
     def get_configuration(self, language: str) -> HookConfiguration:
         """
         Creates a basic, serializable configuration out of the combined specified language config
         :param language: The language to load the configuration for
         :return: A serializable Configuration model
         """
@@ -378,28 +406,28 @@
             completed_process.stdout.decode("utf8") if completed_process.stdout else ""
         )
         if completed_process.returncode != 0:
             return ExecuteResult(successful=False, output=output)
         else:
             return ExecuteResult(successful=True, output=output)
 
-    def _get_language_config(self, language: str) -> LanguagePreCommitConfig:
+    def _get_language_config(self, language: str) -> LanguagePreCommitInstallResult:
         """
         Calculates a hash of the pre-commit file for the given language to be used as part
         of the overall installed configuration.
         :param language: The language specified
         :raises LanguageNotSupportedError if the associated pre-commit file for the language is not found
         :return: LanguagePreCommitConfig - A configuration model containing the language,
         config file data, and a versioning hash of the file contents.
         """
         try:
             config_data = self._calculate_combined_configuration_data(language)
 
             version = self._hash_config(config_data)
-            return LanguagePreCommitConfig(
+            return LanguagePreCommitInstallResult(
                 language=language, config_data=config_data, version=version
             )
         except ValueError:
             raise LanguageNotSupportedError(
                 f"Language '{language}' is currently unsupported"
             )
 
@@ -758,7 +786,83 @@
 
         output += self._process_mismatched_repo_versions(
             current_repos=current_config_repos,
             expected_repos=expected_config_repos,
         )
 
         return output
+
+    def _load_language_config_file(self, language: str) -> LoadLanguageConfigsResult:
+        """
+        Load any config files for given language if they exist.
+        :param language: repo language
+        :return:
+        """
+
+        # respective name for config file
+        language_config_name = Path(f"configs/{slugify(language)}.config.yaml")
+
+        # build absolute path to config file if one exists
+        absolute_secureli_path = f'{Path(f"{__file__}").parent.resolve()}'.rsplit(
+            "/", 1
+        )[0]
+        absolut_configs_path = Path(
+            f"{absolute_secureli_path}/resources/files/{language_config_name}"
+        )
+
+        #  check if config file exists for current language
+        if Path.exists(absolut_configs_path):
+            language_configs_data = self.data_loader(language_config_name)
+            language_configs = yaml.safe_load_all(language_configs_data)
+
+            return LoadLanguageConfigsResult(success=True, config_data=language_configs)
+
+        return LoadLanguageConfigsResult(success=False, config_data=list())
+
+    def _install_pre_commit_configs(
+        self, language: str
+    ) -> LanguagePreCommitConfigInstallResult:
+        """
+        Install any config files for given language to support any pre-commit commands.
+        i.e. Javascript ESLint requires a .eslintrc file to sufficiently use plugins and allow
+        for further customization for repo's flavor of Javascript
+        :param language: repo language
+        :return: LanguagePreCommitConfigInstallResult
+        """
+
+        language_configs_result = self._load_language_config_file(language)
+
+        num_configs_wrote = 0
+        num_configs_non_success = 0
+        non_success_warnings = list[str]()
+
+        # if successfully loaded any language specific configs
+        if language_configs_result.success:
+            for config in language_configs_result.config_data:
+                try:
+                    for key in config:
+                        config_name = f"{slugify(language)}.{key}.yaml"
+                        path_to_config_file = Path(f".secureli/{config_name}")
+
+                        with open(path_to_config_file, "w") as f:
+                            f.write(yaml.dump(config[key]))
+
+                        completed_process = subprocess.run(
+                            ["pre-commit", "install-language-config"]
+                        )
+
+                        if completed_process.returncode != 0:
+                            raise InstallLanguageConfigError(
+                                f"Installing config: {key}, was not successful"
+                            )
+                        num_configs_wrote += 1
+                except Exception as e:
+                    num_configs_non_success += 1
+                    non_success_warnings.append(
+                        f"Unable to install config: {config_name}. {e}"
+                    )
+
+        return LanguagePreCommitConfigInstallResult(
+            num_successful=num_configs_wrote,
+            num_non_success=num_configs_non_success,
+            non_success_messages=non_success_warnings,
+        )
```

### Comparing `secureli-0.3.9/secureli/actions/action.py` & `secureli-0.4.0/secureli/actions/action.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/actions/build.py` & `secureli-0.4.0/secureli/actions/build.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/actions/initializer.py` & `secureli-0.4.0/secureli/actions/initializer.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/actions/scan.py` & `secureli-0.4.0/secureli/actions/scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from typing import Optional
 
-from secureli.utilities.usage_stats import convert_failures_to_failure_count
+from secureli.utilities.usage_stats import post_log, convert_failures_to_failure_count
 from secureli.abstractions.echo import EchoAbstraction
 from secureli.services.logging import LoggingService, LogAction
 from secureli.services.scanner import (
     ScanMode,
     ScannerService,
     Failure,
     OutputParseErrors,
@@ -80,23 +80,27 @@
             scan_result.failures
         )
 
         if failure_count > 0:
             self._process_failures(scan_result.failures, always_yes=always_yes)
 
         if not scan_result.successful:
-            self.logging.failure(
+            log_data = self.logging.failure(
                 LogAction.scan,
                 scan_result_failures_json_string,
                 failure_count,
                 individual_failure_count,
             )
+
+            post_log(log_data.json(exclude_none=True))
         else:
             self.echo.print("Scan executed successfully and detected no issues!")
-            self.logging.success(LogAction.scan)
+            log_data = self.logging.success(LogAction.scan)
+
+            post_log(log_data.json(exclude_none=True))
 
     def _process_failures(
         self,
         failures: list[Failure],
         always_yes: bool,
     ):
         """
```

### Comparing `secureli-0.3.9/secureli/actions/setup.py` & `secureli-0.4.0/secureli/actions/setup.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/actions/update.py` & `secureli-0.4.0/secureli/actions/update.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/container.py` & `secureli-0.4.0/secureli/container.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/main.py` & `secureli-0.4.0/secureli/main.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/repositories/repo_files.py` & `secureli-0.4.0/secureli/repositories/repo_files.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/repositories/secureli_config.py` & `secureli-0.4.0/secureli/repositories/secureli_config.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/repositories/settings.py` & `secureli-0.4.0/secureli/repositories/settings.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/resources/files/build.txt` & `secureli-0.4.0/secureli/resources/files/build.txt`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/resources/files/csharp-pre-commit.yaml` & `secureli-0.4.0/secureli/resources/files/csharp-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/resources/files/java-pre-commit.yaml` & `secureli-0.4.0/secureli/resources/files/java-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/resources/files/python-pre-commit.yaml` & `secureli-0.4.0/secureli/resources/files/python-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/resources/files/typescript-pre-commit.yaml` & `secureli-0.4.0/secureli/resources/files/typescript-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/resources/read_resource.py` & `secureli-0.4.0/secureli/resources/read_resource.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/resources/slugify.py` & `secureli-0.4.0/secureli/resources/slugify.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/services/git_ignore.py` & `secureli-0.4.0/secureli/services/git_ignore.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/services/language_analyzer.py` & `secureli-0.4.0/secureli/services/language_analyzer.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/services/language_support.py` & `secureli-0.4.0/secureli/services/language_support.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional
 
 import pydantic
 
 from secureli.abstractions.pre_commit import PreCommitAbstraction
 from secureli.services.git_ignore import GitIgnoreService
 
-supported_languages = ["C#", "Python", "Java", "Terraform", "TypeScript"]
+supported_languages = ["C#", "Python", "Java", "Terraform", "TypeScript", "JavaScript"]
 
 
 class LanguageMetadata(pydantic.BaseModel):
     version: str
     security_hook_id: Optional[str]
```

### Comparing `secureli-0.3.9/secureli/services/logging.py` & `secureli-0.4.0/secureli/services/logging.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/services/scanner.py` & `secureli-0.4.0/secureli/services/scanner.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/services/secureli_ignore.py` & `secureli-0.4.0/secureli/services/secureli_ignore.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/services/updater.py` & `secureli-0.4.0/secureli/services/updater.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/settings.py` & `secureli-0.4.0/secureli/settings.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/utilities/git_meta.py` & `secureli-0.4.0/secureli/utilities/git_meta.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/secureli/utilities/patterns.py` & `secureli-0.4.0/secureli/utilities/patterns.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.9/PKG-INFO` & `secureli-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: secureli
-Version: 0.3.9
+Version: 0.4.0
 Summary: Secure Project Manager
 License: Apache-2.0
 Author: Caleb Tonn
 Author-email: caleb.tonn@slalom.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cfgv (>=3.3.1,<4.0.0)
 Requires-Dist: dependency-injector[yaml] (>=4.40.0,<5.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: pathspec (>=0.10.1,<0.11.0)
+Requires-Dist: pathspec (>=0.10.1,<0.12.0)
 Requires-Dist: pre-commit (>=2.20,<4.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pygments (>=2.13.0,<3.0.0)
-Requires-Dist: typer[all] (>=0.6.1,<0.7.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: typer[all] (>=0.6.1,<0.10.0)
 Description-Content-Type: text/markdown
 
 [![SeCureLI Logo](https://repository-images.githubusercontent.com/606206029/aa43fa10-689b-4f8a-a6dc-2e9ed06d9e2d)](https://github.com/slalombuild/secureli)
 
 <h1 align="center">SeCureLI</h1>
 <strong>The Builder's Security CLI</strong>
 
@@ -84,14 +85,31 @@
 When invoking these commands, you can combine the short versions into a single flag. For example, the following commands are equivalent:
 
 ```python
 % secureli init --reset --yes
 % secureli init -ry
 ```
 
+# Tutorial to Use Observability Platform to Show Usage Statistics
+
+This tutorial uses New Relic as the sample observability platform. Other platforms may also work, but have not been tested.
+Should you need seCureLI to work with other platforms, please create a new issue in github, or contribute to the open source project.
+
+## Steps
+
+- Assuming, seCureLI has been setup and installed, sign up to New Relic Log Platform https://docs.newrelic.com/docs/logs/log-api/introduction-log-api/
+- Retrieve API_KEY and API_ENDPOINT from New Relic. API_ENDPOINT for New Relic should be https://log-api.newrelic.com/log/v1
+- On your development machine, setup environment variable with variable name API_KEY and API_ENDPOINT
+- Once the above setup is complete, everytime seCureLI triggered, it should send a usage log to New Relic
+- In New Relic, you can create a dashboard of metric to see the number of times secret was caught using query such as
+
+```commandline
+FROM Log Select sum(failure_count_details.detect_secrets) as 'Caught Secret Count'
+```
+
 # Configuration
 
 SeCureLI is configurable via a .secureli.yaml file present in the consuming repository.
 
 ## .secureli.yaml - top level
 
 | Key                | Description                                                                                                                      |
```

