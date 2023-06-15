# Comparing `tmp/cz_github_jira_conventional-1.1.1.tar.gz` & `tmp/cz_github_jira_conventional-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cz_github_jira_conventional-1.1.1.tar", last modified: Wed Jul 27 08:13:50 2022, max compression
+gzip compressed data, was "cz_github_jira_conventional-2.0.0.tar", last modified: Thu Jun 15 08:13:57 2023, max compression
```

## Comparing `cz_github_jira_conventional-1.1.1.tar` & `cz_github_jira_conventional-2.0.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxr-x   0 falkokrause  (1000) falkokrause  (1000)        0 2022-07-27 08:13:50.332831 cz_github_jira_conventional-1.1.1/
--rw-rw-r--   0 falkokrause  (1000) falkokrause  (1000)     4469 2022-07-27 08:13:50.332831 cz_github_jira_conventional-1.1.1/PKG-INFO
--rw-rw-r--   0 falkokrause  (1000) falkokrause  (1000)     3377 2022-07-26 07:55:51.000000 cz_github_jira_conventional-1.1.1/README.md
-drwxrwxr-x   0 falkokrause  (1000) falkokrause  (1000)        0 2022-07-27 08:13:50.332831 cz_github_jira_conventional-1.1.1/cz_github_jira_conventional.egg-info/
--rw-rw-r--   0 falkokrause  (1000) falkokrause  (1000)     4469 2022-07-27 08:13:50.000000 cz_github_jira_conventional-1.1.1/cz_github_jira_conventional.egg-info/PKG-INFO
--rw-rw-r--   0 falkokrause  (1000) falkokrause  (1000)      303 2022-07-27 08:13:50.000000 cz_github_jira_conventional-1.1.1/cz_github_jira_conventional.egg-info/SOURCES.txt
--rw-rw-r--   0 falkokrause  (1000) falkokrause  (1000)        1 2022-07-27 08:13:50.000000 cz_github_jira_conventional-1.1.1/cz_github_jira_conventional.egg-info/dependency_links.txt
--rw-rw-r--   0 falkokrause  (1000) falkokrause  (1000)       11 2022-07-27 08:13:50.000000 cz_github_jira_conventional-1.1.1/cz_github_jira_conventional.egg-info/requires.txt
--rw-rw-r--   0 falkokrause  (1000) falkokrause  (1000)       28 2022-07-27 08:13:50.000000 cz_github_jira_conventional-1.1.1/cz_github_jira_conventional.egg-info/top_level.txt
--rw-rw-r--   0 falkokrause  (1000) falkokrause  (1000)     9483 2022-07-26 07:56:02.000000 cz_github_jira_conventional-1.1.1/cz_github_jira_conventional.py
--rw-rw-r--   0 falkokrause  (1000) falkokrause  (1000)       38 2022-07-27 08:13:50.332831 cz_github_jira_conventional-1.1.1/setup.cfg
--rw-rw-r--   0 falkokrause  (1000) falkokrause  (1000)      786 2022-07-27 08:12:56.000000 cz_github_jira_conventional-1.1.1/setup.py
+drwxrwxr-x   0 falkokrause  (1000) falkokrause  (1000)        0 2023-06-15 08:13:57.833859 cz_github_jira_conventional-2.0.0/
+-rw-rw-r--   0 falkokrause  (1000) falkokrause  (1000)     1072 2022-07-26 07:55:51.000000 cz_github_jira_conventional-2.0.0/LICENSE
+-rw-rw-r--   0 falkokrause  (1000) falkokrause  (1000)     3772 2023-06-15 08:13:57.833859 cz_github_jira_conventional-2.0.0/PKG-INFO
+-rw-rw-r--   0 falkokrause  (1000) falkokrause  (1000)     3377 2022-07-26 07:55:51.000000 cz_github_jira_conventional-2.0.0/README.md
+drwxrwxr-x   0 falkokrause  (1000) falkokrause  (1000)        0 2023-06-15 08:13:57.833859 cz_github_jira_conventional-2.0.0/cz_github_jira_conventional.egg-info/
+-rw-rw-r--   0 falkokrause  (1000) falkokrause  (1000)     3772 2023-06-15 08:13:57.000000 cz_github_jira_conventional-2.0.0/cz_github_jira_conventional.egg-info/PKG-INFO
+-rw-rw-r--   0 falkokrause  (1000) falkokrause  (1000)      365 2023-06-15 08:13:57.000000 cz_github_jira_conventional-2.0.0/cz_github_jira_conventional.egg-info/SOURCES.txt
+-rw-rw-r--   0 falkokrause  (1000) falkokrause  (1000)        1 2023-06-15 08:13:57.000000 cz_github_jira_conventional-2.0.0/cz_github_jira_conventional.egg-info/dependency_links.txt
+-rw-rw-r--   0 falkokrause  (1000) falkokrause  (1000)      103 2023-06-15 08:13:57.000000 cz_github_jira_conventional-2.0.0/cz_github_jira_conventional.egg-info/entry_points.txt
+-rw-rw-r--   0 falkokrause  (1000) falkokrause  (1000)       11 2023-06-15 08:13:57.000000 cz_github_jira_conventional-2.0.0/cz_github_jira_conventional.egg-info/requires.txt
+-rw-rw-r--   0 falkokrause  (1000) falkokrause  (1000)       28 2023-06-15 08:13:57.000000 cz_github_jira_conventional-2.0.0/cz_github_jira_conventional.egg-info/top_level.txt
+-rw-rw-r--   0 falkokrause  (1000) falkokrause  (1000)     9869 2023-06-15 07:55:54.000000 cz_github_jira_conventional-2.0.0/cz_github_jira_conventional.py
+-rw-rw-r--   0 falkokrause  (1000) falkokrause  (1000)       38 2023-06-15 08:13:57.833859 cz_github_jira_conventional-2.0.0/setup.cfg
+-rw-rw-r--   0 falkokrause  (1000) falkokrause  (1000)      950 2023-06-15 08:11:40.000000 cz_github_jira_conventional-2.0.0/setup.py
```

### Comparing `cz_github_jira_conventional-1.1.1/PKG-INFO` & `cz_github_jira_conventional-2.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,97 +1,97 @@
 Metadata-Version: 2.1
 Name: cz_github_jira_conventional
-Version: 1.1.1
+Version: 2.0.0
 Summary: Extend the commitizen tools to create conventional commits and README that link to Jira and GitHub.
 Home-page: https://github.com/apheris/cz-github-jira-conventional
 Author: Falko Krause, apheris AI GmbH
 Author-email: f.krause@apheris.com
 License: MIT
-Description: # cz-github-jira-conventional
-        
-        **cz-github-jira-conventional** is a plugin for the [**commitizen tools**](https://github.com/commitizen-tools/commitizen), a toolset that helps you to create [**conventional commit messages**](https://www.conventionalcommits.org/en/v1.0.0/). Since the structure of conventional commits messages is standardized they are machine readable and allow commitizen to automaticially calculate and tag [**semantic version numbers**](https://semver.org/) as well as create **CHANGELOG.md** files for your releases.
-        
-        This plugin extends the commitizen tools by:
-        - **require a Jira issue id** in the commit message
-        - **create links to GitHub** commits in the CHANGELOG.md
-        - **create links to Jira** issues in the CHANGELOG.md
-        
-        When you call commitizen `commit` you will be required you to enter the scope of your commit as a Jira issue id (or multiple issue ids, prefixed or without prefix, see config below).
-        ```
-        > cz commit
-        ? Select the type of change you are committing fix: A bug fix. Correlates with PATCH in SemVer
-        ? JIRA issue number (multiple "42, 123"). XX-
-        ...
-        ```
-        
-        The changelog created by cz (`cz bump --changelog`)will contain links to the commits in Github and the Jira issues.
-        ```markdown
-        ## v1.0.0 (2021-08-06)
-        
-        ### Features
-        
-        - **[XX-123](https://myproject.atlassian.net/browse/XX-123)**: create changelogs with links to issues and commits [a374b](https://github.com/apheris/cz-github-jira-conventional/commit/a374b93f39327964f5ab5290252b795647906008)
-        - **[XX-42](https://myproject.atlassian.net/browse/XX-42),[XX-13](https://myproject.atlassian.net/browse/XX-13)**: allow multiple issue to be referenced in the commit [07ab0](https://github.com/apheris/cz-github-jira-conventional/commit/07ab0e09de36712ab1db93fff0c821ecd80b5849)
-        ``` 
-        
-        
-        ## Installation
-        
-        Install with pip
-        `python -m pip install cz-github-jira-conventional` 
-        
-        You need to use a cz config file that has the **required** additional values `jira_base_url` and `github_repo` and may contain the **optional** value `jira_prefix`.
-        
-        Example `.cz.yaml` config for this repository
-        ```yaml
-        commitizen:
-          name: cz_github_jira_conventional
-          tag_format: v$version
-          version: 1.0.0
-          jira_prefix: XX-
-          jira_base_url: https://myproject.atlassian.net
-          github_repo: apheris/cz-github-jira-conventional
-        ```
-        
-        The `jira_prefix` can be either 
-        - empty (the user must write the prefix for each issue)
-        - a string (the prefix will be added automatically)
-        - a list (for multiple projects, the user will be asked to choose a prefix)
-        
-        ```yaml
-          jira_prefix: 
-            - XX-
-            - XY-
-            - YY-
-        ```
-        
-        ### pre-commit
-        Add this plugin to the dependencies of your commit message linting with `pre-commit`. 
-        
-        Example `.pre-commit-config.yaml` file.
-        ```yaml
-        repos:
-          - repo: https://github.com/commitizen-tools/commitizen
-            rev: v2.17.13
-            hooks:
-              - id: commitizen
-                stages: [commit-msg]
-                additional_dependencies: [cz-github-jira-conventional]
-        ```
-        Install the hook with 
-        ```bash
-        pre-commit install --hook-type commit-msg
-        ```
-        
-        <!-- LICENSE -->
-        ## License
-        
-        Distributed under the MIT License. See `LICENSE` for more information.
-        
-        <!-- ACKNOWLEDGEMENTS -->
-        ## Acknowledgements
-        This plugin would not have been possible without the fantastic work from:
-        * [commitizen tools](https://github.com/commitizen-tools/commitizen)
-        * [conventional_JIRA](https://github.com/Crystalix007/conventional_jira)
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# cz-github-jira-conventional
+
+**cz-github-jira-conventional** is a plugin for the [**commitizen tools**](https://github.com/commitizen-tools/commitizen), a toolset that helps you to create [**conventional commit messages**](https://www.conventionalcommits.org/en/v1.0.0/). Since the structure of conventional commits messages is standardized they are machine readable and allow commitizen to automaticially calculate and tag [**semantic version numbers**](https://semver.org/) as well as create **CHANGELOG.md** files for your releases.
+
+This plugin extends the commitizen tools by:
+- **require a Jira issue id** in the commit message
+- **create links to GitHub** commits in the CHANGELOG.md
+- **create links to Jira** issues in the CHANGELOG.md
+
+When you call commitizen `commit` you will be required you to enter the scope of your commit as a Jira issue id (or multiple issue ids, prefixed or without prefix, see config below).
+```
+> cz commit
+? Select the type of change you are committing fix: A bug fix. Correlates with PATCH in SemVer
+? JIRA issue number (multiple "42, 123"). XX-
+...
+```
+
+The changelog created by cz (`cz bump --changelog`)will contain links to the commits in Github and the Jira issues.
+```markdown
+## v1.0.0 (2021-08-06)
+
+### Features
+
+- **[XX-123](https://myproject.atlassian.net/browse/XX-123)**: create changelogs with links to issues and commits [a374b](https://github.com/apheris/cz-github-jira-conventional/commit/a374b93f39327964f5ab5290252b795647906008)
+- **[XX-42](https://myproject.atlassian.net/browse/XX-42),[XX-13](https://myproject.atlassian.net/browse/XX-13)**: allow multiple issue to be referenced in the commit [07ab0](https://github.com/apheris/cz-github-jira-conventional/commit/07ab0e09de36712ab1db93fff0c821ecd80b5849)
+``` 
+
+
+## Installation
+
+Install with pip
+`python -m pip install cz-github-jira-conventional` 
+
+You need to use a cz config file that has the **required** additional values `jira_base_url` and `github_repo` and may contain the **optional** value `jira_prefix`.
+
+Example `.cz.yaml` config for this repository
+```yaml
+commitizen:
+  name: cz_github_jira_conventional
+  tag_format: v$version
+  version: 1.0.0
+  jira_prefix: XX-
+  jira_base_url: https://myproject.atlassian.net
+  github_repo: apheris/cz-github-jira-conventional
+```
+
+The `jira_prefix` can be either 
+- empty (the user must write the prefix for each issue)
+- a string (the prefix will be added automatically)
+- a list (for multiple projects, the user will be asked to choose a prefix)
+
+```yaml
+  jira_prefix: 
+    - XX-
+    - XY-
+    - YY-
+```
+
+### pre-commit
+Add this plugin to the dependencies of your commit message linting with `pre-commit`. 
+
+Example `.pre-commit-config.yaml` file.
+```yaml
+repos:
+  - repo: https://github.com/commitizen-tools/commitizen
+    rev: v2.17.13
+    hooks:
+      - id: commitizen
+        stages: [commit-msg]
+        additional_dependencies: [cz-github-jira-conventional]
+```
+Install the hook with 
+```bash
+pre-commit install --hook-type commit-msg
+```
+
+<!-- LICENSE -->
+## License
+
+Distributed under the MIT License. See `LICENSE` for more information.
+
+<!-- ACKNOWLEDGEMENTS -->
+## Acknowledgements
+This plugin would not have been possible without the fantastic work from:
+* [commitizen tools](https://github.com/commitizen-tools/commitizen)
+* [conventional_JIRA](https://github.com/Crystalix007/conventional_jira)
```

### Comparing `cz_github_jira_conventional-1.1.1/README.md` & `cz_github_jira_conventional-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cz_github_jira_conventional-1.1.1/cz_github_jira_conventional.egg-info/PKG-INFO` & `cz_github_jira_conventional-2.0.0/cz_github_jira_conventional.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,97 +1,97 @@
 Metadata-Version: 2.1
 Name: cz-github-jira-conventional
-Version: 1.1.1
+Version: 2.0.0
 Summary: Extend the commitizen tools to create conventional commits and README that link to Jira and GitHub.
 Home-page: https://github.com/apheris/cz-github-jira-conventional
 Author: Falko Krause, apheris AI GmbH
 Author-email: f.krause@apheris.com
 License: MIT
-Description: # cz-github-jira-conventional
-        
-        **cz-github-jira-conventional** is a plugin for the [**commitizen tools**](https://github.com/commitizen-tools/commitizen), a toolset that helps you to create [**conventional commit messages**](https://www.conventionalcommits.org/en/v1.0.0/). Since the structure of conventional commits messages is standardized they are machine readable and allow commitizen to automaticially calculate and tag [**semantic version numbers**](https://semver.org/) as well as create **CHANGELOG.md** files for your releases.
-        
-        This plugin extends the commitizen tools by:
-        - **require a Jira issue id** in the commit message
-        - **create links to GitHub** commits in the CHANGELOG.md
-        - **create links to Jira** issues in the CHANGELOG.md
-        
-        When you call commitizen `commit` you will be required you to enter the scope of your commit as a Jira issue id (or multiple issue ids, prefixed or without prefix, see config below).
-        ```
-        > cz commit
-        ? Select the type of change you are committing fix: A bug fix. Correlates with PATCH in SemVer
-        ? JIRA issue number (multiple "42, 123"). XX-
-        ...
-        ```
-        
-        The changelog created by cz (`cz bump --changelog`)will contain links to the commits in Github and the Jira issues.
-        ```markdown
-        ## v1.0.0 (2021-08-06)
-        
-        ### Features
-        
-        - **[XX-123](https://myproject.atlassian.net/browse/XX-123)**: create changelogs with links to issues and commits [a374b](https://github.com/apheris/cz-github-jira-conventional/commit/a374b93f39327964f5ab5290252b795647906008)
-        - **[XX-42](https://myproject.atlassian.net/browse/XX-42),[XX-13](https://myproject.atlassian.net/browse/XX-13)**: allow multiple issue to be referenced in the commit [07ab0](https://github.com/apheris/cz-github-jira-conventional/commit/07ab0e09de36712ab1db93fff0c821ecd80b5849)
-        ``` 
-        
-        
-        ## Installation
-        
-        Install with pip
-        `python -m pip install cz-github-jira-conventional` 
-        
-        You need to use a cz config file that has the **required** additional values `jira_base_url` and `github_repo` and may contain the **optional** value `jira_prefix`.
-        
-        Example `.cz.yaml` config for this repository
-        ```yaml
-        commitizen:
-          name: cz_github_jira_conventional
-          tag_format: v$version
-          version: 1.0.0
-          jira_prefix: XX-
-          jira_base_url: https://myproject.atlassian.net
-          github_repo: apheris/cz-github-jira-conventional
-        ```
-        
-        The `jira_prefix` can be either 
-        - empty (the user must write the prefix for each issue)
-        - a string (the prefix will be added automatically)
-        - a list (for multiple projects, the user will be asked to choose a prefix)
-        
-        ```yaml
-          jira_prefix: 
-            - XX-
-            - XY-
-            - YY-
-        ```
-        
-        ### pre-commit
-        Add this plugin to the dependencies of your commit message linting with `pre-commit`. 
-        
-        Example `.pre-commit-config.yaml` file.
-        ```yaml
-        repos:
-          - repo: https://github.com/commitizen-tools/commitizen
-            rev: v2.17.13
-            hooks:
-              - id: commitizen
-                stages: [commit-msg]
-                additional_dependencies: [cz-github-jira-conventional]
-        ```
-        Install the hook with 
-        ```bash
-        pre-commit install --hook-type commit-msg
-        ```
-        
-        <!-- LICENSE -->
-        ## License
-        
-        Distributed under the MIT License. See `LICENSE` for more information.
-        
-        <!-- ACKNOWLEDGEMENTS -->
-        ## Acknowledgements
-        This plugin would not have been possible without the fantastic work from:
-        * [commitizen tools](https://github.com/commitizen-tools/commitizen)
-        * [conventional_JIRA](https://github.com/Crystalix007/conventional_jira)
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# cz-github-jira-conventional
+
+**cz-github-jira-conventional** is a plugin for the [**commitizen tools**](https://github.com/commitizen-tools/commitizen), a toolset that helps you to create [**conventional commit messages**](https://www.conventionalcommits.org/en/v1.0.0/). Since the structure of conventional commits messages is standardized they are machine readable and allow commitizen to automaticially calculate and tag [**semantic version numbers**](https://semver.org/) as well as create **CHANGELOG.md** files for your releases.
+
+This plugin extends the commitizen tools by:
+- **require a Jira issue id** in the commit message
+- **create links to GitHub** commits in the CHANGELOG.md
+- **create links to Jira** issues in the CHANGELOG.md
+
+When you call commitizen `commit` you will be required you to enter the scope of your commit as a Jira issue id (or multiple issue ids, prefixed or without prefix, see config below).
+```
+> cz commit
+? Select the type of change you are committing fix: A bug fix. Correlates with PATCH in SemVer
+? JIRA issue number (multiple "42, 123"). XX-
+...
+```
+
+The changelog created by cz (`cz bump --changelog`)will contain links to the commits in Github and the Jira issues.
+```markdown
+## v1.0.0 (2021-08-06)
+
+### Features
+
+- **[XX-123](https://myproject.atlassian.net/browse/XX-123)**: create changelogs with links to issues and commits [a374b](https://github.com/apheris/cz-github-jira-conventional/commit/a374b93f39327964f5ab5290252b795647906008)
+- **[XX-42](https://myproject.atlassian.net/browse/XX-42),[XX-13](https://myproject.atlassian.net/browse/XX-13)**: allow multiple issue to be referenced in the commit [07ab0](https://github.com/apheris/cz-github-jira-conventional/commit/07ab0e09de36712ab1db93fff0c821ecd80b5849)
+``` 
+
+
+## Installation
+
+Install with pip
+`python -m pip install cz-github-jira-conventional` 
+
+You need to use a cz config file that has the **required** additional values `jira_base_url` and `github_repo` and may contain the **optional** value `jira_prefix`.
+
+Example `.cz.yaml` config for this repository
+```yaml
+commitizen:
+  name: cz_github_jira_conventional
+  tag_format: v$version
+  version: 1.0.0
+  jira_prefix: XX-
+  jira_base_url: https://myproject.atlassian.net
+  github_repo: apheris/cz-github-jira-conventional
+```
+
+The `jira_prefix` can be either 
+- empty (the user must write the prefix for each issue)
+- a string (the prefix will be added automatically)
+- a list (for multiple projects, the user will be asked to choose a prefix)
+
+```yaml
+  jira_prefix: 
+    - XX-
+    - XY-
+    - YY-
+```
+
+### pre-commit
+Add this plugin to the dependencies of your commit message linting with `pre-commit`. 
+
+Example `.pre-commit-config.yaml` file.
+```yaml
+repos:
+  - repo: https://github.com/commitizen-tools/commitizen
+    rev: v2.17.13
+    hooks:
+      - id: commitizen
+        stages: [commit-msg]
+        additional_dependencies: [cz-github-jira-conventional]
+```
+Install the hook with 
+```bash
+pre-commit install --hook-type commit-msg
+```
+
+<!-- LICENSE -->
+## License
+
+Distributed under the MIT License. See `LICENSE` for more information.
+
+<!-- ACKNOWLEDGEMENTS -->
+## Acknowledgements
+This plugin would not have been possible without the fantastic work from:
+* [commitizen tools](https://github.com/commitizen-tools/commitizen)
+* [conventional_JIRA](https://github.com/Crystalix007/conventional_jira)
```

### Comparing `cz_github_jira_conventional-1.1.1/cz_github_jira_conventional.py` & `cz_github_jira_conventional-2.0.0/cz_github_jira_conventional.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 from commitizen import defaults, git, config
 from commitizen.cz.base import BaseCommitizen
 from commitizen.cz.utils import multiple_line_breaker, required_validator
 from commitizen.cz.exceptions import CzException
 
 __all__ = ["GithubJiraConventionalCz"]
 
+DEFAULT_GITHUB_BASE_URL = "https://github.com/"
+DEFAULT_CHANGE_TYPE_MAP = {
+    "feat": "Feat",
+    "fix": "Fix",
+    "refactor": "Refactor",
+    "perf": "Perf",
+}
 
 def parse_subject(text):
     if isinstance(text, str):
         text = text.strip(".").strip()
 
     return required_validator(text, msg="Subject is required.")
 
@@ -37,26 +44,33 @@
         issue_multiple_hint = "XZ-42, XY-123"
 
     if "jira_base_url" not in conf.settings:
         print(
             "Please add the key jira_base_url to your .cz.yaml|json|toml config file."
         )
         quit()
+    
     if "github_repo" not in conf.settings:
         print("Please add the key github_repo to your .cz.yaml|json|toml config file.")
         quit()
+    
     jira_base_url = conf.settings["jira_base_url"]
     github_repo = conf.settings["github_repo"]
-    # if "change_type_map" not in conf.settings:
-    change_type_map = {
-        "feat": "Feat",
-        "fix": "Fix",
-        "refactor": "Refactor",
-        "perf": "Perf",
-    }
+    
+    if "github_base_url" not in conf.settings:
+        github_base_url = DEFAULT_GITHUB_BASE_URL
+    else:
+        github_base_url = conf.settings["github_base_url"]
+    
+    if "change_type_map" not in conf.settings:
+        change_type_map = DEFAULT_CHANGE_TYPE_MAP
+    else:
+        #change_type_map = conf.settings["change_type_map"]
+        print("Only default change type map is supported at the moment.")
+        quit()
 
     def questions(self) -> List[Dict[str, Any]]:
         questions: List[Dict[str, Any]] = [
             {
                 "type": "list",
                 "name": "prefix",
                 "message": "Select the type of change you are committing",
@@ -262,16 +276,13 @@
                 [
                     f"[{issue_id}]({self.jira_base_url}/browse/{issue_id})"
                     for issue_id in parsed_message["scope"].split(",")
                 ]
             )
         parsed_message[
             "message"
-        ] = f"{m} [{rev[:5]}](https://github.com/{self.github_repo}/commit/{commit.rev})"
+        ] = f"{m} [{rev[:5]}]({self.github_base_url}/{self.github_repo}/commit/{commit.rev})"
         return parsed_message
 
 
 class InvalidAnswerError(CzException):
     ...
-
-
-discover_this = GithubJiraConventionalCz
```

### Comparing `cz_github_jira_conventional-1.1.1/setup.py` & `cz_github_jira_conventional-2.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,18 +5,23 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="cz_github_jira_conventional",
-    version="1.1.1",
+    version="2.0.0",
     py_modules=["cz_github_jira_conventional"],
     author="Falko Krause, apheris AI GmbH",
     author_email="f.krause@apheris.com",
     license="MIT",
     url="https://github.com/apheris/cz-github-jira-conventional",
     install_requires=["commitizen"],
     description="Extend the commitizen tools to create conventional commits and README that link to Jira and GitHub.",
     long_description=long_description,
     long_description_content_type="text/markdown",
+    entry_points={
+        "commitizen.plugin": [
+            "cz_github_jira_conventional = cz_github_jira_conventional:GithubJiraConventionalCz"
+        ]
+    },
 )
```

