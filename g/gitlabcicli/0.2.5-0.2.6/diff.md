# Comparing `tmp/gitlabcicli-0.2.5.tar.gz` & `tmp/gitlabcicli-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlabcicli-0.2.5.tar", max compression
+gzip compressed data, was "gitlabcicli-0.2.6.tar", max compression
```

## Comparing `gitlabcicli-0.2.5.tar` & `gitlabcicli-0.2.6.tar`

### file list

```diff
@@ -1,22 +1,11 @@
--rw-r--r--   0        0        0    35069 2018-09-09 00:49:12.046406 gitlabcicli-0.2.5/LICENSE
--rw-r--r--   0        0        0      293 2020-05-01 18:06:58.428742 gitlabcicli-0.2.5/gitlabcicli/__init__.py
--rwxr-xr-x   0        0        0      210 2018-07-13 18:47:25.212540 gitlabcicli-0.2.5/gitlabcicli/__main__.py
--rw-r--r--   0        0        0        0 2020-05-04 21:16:19.337317 gitlabcicli-0.2.5/gitlabcicli/api/__init__.py
--rw-r--r--   0        0        0     2134 2023-04-27 09:33:10.249630 gitlabcicli-0.2.5/gitlabcicli/api/gitlab_api_driver.py
--rw-r--r--   0        0        0       98 2020-05-01 22:50:56.147701 gitlabcicli-0.2.5/gitlabcicli/api/models/__init__.py
--rw-r--r--   0        0        0     1485 2023-04-27 09:28:50.094831 gitlabcicli-0.2.5/gitlabcicli/api/models/pipeline.py
--rw-r--r--   0        0        0     3936 2023-04-27 09:30:07.811935 gitlabcicli-0.2.5/gitlabcicli/api/models/project.py
--rw-r--r--   0        0        0     6929 2021-03-31 17:20:49.085504 gitlabcicli-0.2.5/gitlabcicli/gitlabapiwrapper.py
--rwxr-xr-x   0        0        0    19464 2023-06-05 17:35:36.446759 gitlabcicli-0.2.5/gitlabcicli/gitlabcicli.py
--rw-r--r--   0        0        0     2442 2021-03-31 17:43:41.430511 gitlabcicli-0.2.5/gitlabcicli/gitwrapper.py
--rw-r--r--   0        0        0     1105 2023-06-05 18:04:59.411829 gitlabcicli-0.2.5/gitlabcicli/keyring_wrapper.py
--rw-r--r--   0        0        0      423 2020-12-08 14:07:42.199276 gitlabcicli-0.2.5/gitlabcicli/managerlib/__init__.py
--rw-r--r--   0        0        0     4531 2023-04-27 09:31:07.458938 gitlabcicli-0.2.5/gitlabcicli/managerlib/api_driver.py
--rw-r--r--   0        0        0      469 2020-05-04 22:08:08.496965 gitlabcicli-0.2.5/gitlabcicli/managerlib/errors.py
--rw-r--r--   0        0        0     7246 2023-05-28 20:20:46.579857 gitlabcicli-0.2.5/gitlabcicli/managerlib/fields.py
--rw-r--r--   0        0        0     3880 2023-04-27 09:29:47.421820 gitlabcicli-0.2.5/gitlabcicli/managerlib/model.py
--rw-r--r--   0        0        0      691 2023-04-27 09:31:41.092461 gitlabcicli-0.2.5/gitlabcicli/managerlib/utils.py
--rw-r--r--   0        0        0     1032 2023-06-05 17:40:00.708015 gitlabcicli-0.2.5/gitlabcicli/script_helpers.py
--rw-r--r--   0        0        0      268 2020-12-08 14:07:42.239276 gitlabcicli-0.2.5/gitlabcicli/utils.py
--rw-r--r--   0        0        0      752 2023-06-05 18:06:22.845517 gitlabcicli-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 gitlabcicli-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    35069 2023-06-15 06:00:37.027574 gitlabcicli-0.2.6/LICENSE
+-rw-r--r--   0        0        0      293 2023-06-15 06:00:37.027574 gitlabcicli-0.2.6/gitlabcicli/__init__.py
+-rwxr-xr-x   0        0        0      210 2023-06-15 06:00:37.027574 gitlabcicli-0.2.6/gitlabcicli/__main__.py
+-rw-r--r--   0        0        0     7184 2023-06-15 06:55:11.859126 gitlabcicli-0.2.6/gitlabcicli/gitlabapiwrapper.py
+-rwxr-xr-x   0        0        0    19978 2023-06-15 06:55:11.859126 gitlabcicli-0.2.6/gitlabcicli/gitlabcicli.py
+-rw-r--r--   0        0        0     2442 2023-06-15 06:00:37.027574 gitlabcicli-0.2.6/gitlabcicli/gitwrapper.py
+-rw-r--r--   0        0        0     1105 2023-06-15 06:00:37.027574 gitlabcicli-0.2.6/gitlabcicli/keyring_wrapper.py
+-rw-r--r--   0        0        0     1066 2023-06-15 06:55:11.862459 gitlabcicli-0.2.6/gitlabcicli/script_helpers.py
+-rw-r--r--   0        0        0      283 2023-06-15 06:55:11.865792 gitlabcicli-0.2.6/gitlabcicli/utils.py
+-rw-r--r--   0        0        0      827 2023-06-15 06:55:58.544185 gitlabcicli-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 gitlabcicli-0.2.6/PKG-INFO
```

### Comparing `gitlabcicli-0.2.5/LICENSE` & `gitlabcicli-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlabcicli-0.2.5/gitlabcicli/gitlabapiwrapper.py` & `gitlabcicli-0.2.6/gitlabcicli/gitlabapiwrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """A small and simple GitLab API wrapper."""
 
+from urllib.parse import urljoin
 import requests
 
 from gitlabcicli.script_helpers import debug, error
 
 try:
     from hyper.contrib import HTTP20Adapter
 except ImportError:
@@ -48,15 +49,15 @@
 
             return default
 
         return api
 
     def _request(self, url, method="GET", **kwargs):
         """Make a requests."""
-        apiurl = f"{self.server_url}{url}"
+        apiurl = urljoin(self.server_url, url.replace("//", "/"))
         debug(f"{method} {apiurl}", 5)
 
         if method == "GET":
             return self.session.get(apiurl, **kwargs)
         elif method == "POST":
             return self.session.post(apiurl, **kwargs)
         else:
@@ -127,15 +128,16 @@
         if not response.ok:
             if response.status_code == 404:
                 error(f"No log for job {job_id} found.")
 
                 return ""
             else:
                 error(
-                    f"Could not get raw job log. Received status code {response.status_code}"
+                    "Could not get raw job log."
+                    f" Received status code {response.status_code}"
                 )
 
         return response.text
 
     def get_project_path(self, project_id):
         """Return the full path with namespace for the project with id `project_id`."""
 
@@ -155,15 +157,15 @@
         """Return the id for the project on server"""
 
         if project.isnumeric():
             debug("interpreting project argument as id.", 3)
 
             return int(project)
 
-        query = project.split("/", 2)[-1]
+        query = project.rsplit("/", 2)[-1]
         api = self._get_api(
             apiurl=f"projects/?search={query}",
             default_return_value=[],
             params={"order_by": "last_activity_at", "sort": "desc"},
         )
 
         for apiproj in api:
@@ -189,33 +191,38 @@
         """Run action (cancel, retry, erase) on job"""
 
         return self._post_api(
             apiurl=f"projects/{project_id}/jobs/{job_id}/{action}",
             default_return_value={},
         )
 
-    def validate_ciyml(self, gitlabciyml_text):
+    def validate_ciyml(self, gitlabciyml_text: str, project_id: int) -> dict:
         """Return:
         valid:
-            {"status": "valid", "errors": []}
+            {"valid": True, "warnings": [], "errors": []}
         invalid:
-            {"status": "invalid", "errors": ["description 1", "description 2"]}
+            {
+                "valid": "False",
+                "warnings": [],
+                "errors": ["description 1", "description 2"]
+            }
         error:
             {"error": "description"}
         """
         api = self._post_api(
-            apiurl="/ci/lint",
+            apiurl=f"/projects/{project_id}/ci/lint",
             default_return_value={"error": "request failed"},
             data={"content": gitlabciyml_text},
         )
 
         if "error" in api.keys():
             error(api["error"])
         elif (
-            "status" not in api.keys()
+            "valid" not in api.keys()
             or "errors" not in api.keys()
-            or api["status"] not in ["valid", "invalid"]
+            or "warnings" not in api.keys()
+            or api["valid"] not in (True, False)
         ):
             debug(api, 4)
             error("Invalid response from api")
         else:
             return api
```

### Comparing `gitlabcicli-0.2.5/gitlabcicli/gitlabcicli.py` & `gitlabcicli-0.2.6/gitlabcicli/gitlabcicli.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
 COMMANDS = dict[str, Command]()
 
 
 def register_command(
     *,
     name: str | None = None,
-    aliases: set[str] = frozenset[str](),
+    aliases=frozenset[str](),
     doc: str | None = None,
 ) -> typing.Callable:
     """Decorator to register a command"""
 
     def inner(func: typing.Callable) -> typing.Callable:
         cmd_name = name or func.__name__.replace("_", "-")
         COMMANDS[cmd_name] = Command(
@@ -101,15 +101,15 @@
         )
 
         return func
 
     return inner
 
 
-def sha_completer(prefix, **kwargs):
+def sha_completer(prefix, **_):
     """tab completion shas in current git"""
 
     return (s[:8] for s in get_shas() if s.startswith(prefix))
 
 
 def gitlabciyml_completer(prefix, **_):
     """tab completion for .gitlab-ci.yml"""
@@ -230,15 +230,15 @@
         table_jobs.append(table_job)
     print(tabulate(table_jobs, headers=table_headers, disable_numparse=True))
 
 
 class GitLabCiCli(object):
     """A Cli class."""
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs) -> None:
         self._api_client: GitLabApiClient | None = None
         self._server_url: str | None = kwargs.get("server_url", None)
         self._project_id: int | None = kwargs.get("project_id", None)
         self._project_path: str | None = kwargs.get("project_path", None)
         self._project: str | None = kwargs.get("project", None)
         self._token: str | None = kwargs.get("token", None)
         self._commit_hash: str | None = kwargs.get("commit_hash", None)
@@ -337,22 +337,21 @@
                         f"Please enter the GitLab API Token for {self.server_url}: ",
                         attrs=["bold"],
                     )
                 )
             except (EOFError, KeyboardInterrupt):
                 print()
                 error("Interrupted")
-                exit(1)
         elif not self._token:
             debug("Try to get token for server from config...", 2)
             self._token = self._keyring_wrapper.get_token(self.server_url)
 
         if not self._token:
             error(
-                "No token found in wallet or given."
+                f"No token for {self.server_url} found in wallet or given."
                 " Please use --ask-for-token to specify your token."
             )
             sys.exit(501)
 
         debug(f"Using token {self._token}", 5)
 
         return self._token
@@ -384,26 +383,26 @@
                 project_id=self.project_id,
                 pipeline_id=pipeline_id,
             )
             jobs = sorted(jobs, key=lambda v: v["id"])
 
         return jobs
 
-    @register_command(aliases={"status"})
+    @register_command(aliases=frozenset({"status"}))
     def show(self):
         """Run gitlabcicli show."""
         jobs = self.get_jobs()
 
         if not jobs:
             error("No jobs found.")
 
             return
         print_job_table(jobs)
 
-    @register_command(aliases={"log"})
+    @register_command(aliases=frozenset({"log"}))
     def raw(self):
         """run gitlabcicli raw"""
         jobs = self.get_jobs()
 
         for job in jobs:
             artifacts = job.get("artifacts", [])
             traces = [
@@ -411,21 +410,23 @@
                 for artifact in artifacts
                 if artifact.get("file_type") == "trace"
             ]
             job_id = job.get("id")
 
             if not traces:
                 error(
-                    f"There is no job log yet for job #{job_id} for project '{self.project}'."
+                    f"There is no job log yet for job #{job_id}"
+                    f" in project '{self.project}'."
                 )
 
                 continue
             elif len(traces) > 1:
                 error(
-                    f"There are too many job logs for job #{job_id} for project '{self.project}'."
+                    f"There are too many job logs for job #{job_id}"
+                    f" in project '{self.project}'."
                 )
 
                 continue
 
             trace_file_name = traces.pop().get("filename")
             print()
             cprint(f" === Job output of job #{job['id']} === ", attrs=["bold"])
@@ -435,82 +436,96 @@
                 job_id=job["id"],
                 file_path=trace_file_name,
             )
             print(raw_output)
 
             print()
 
-    @register_command(aliases={"action"})
+    @register_command(aliases=frozenset({"action"}))
     def do(self):
         """Run gitlabcicli do."""
 
         for job_id in self.args["job_ids"]:
             response = self.api_client.run_action_on_job(
                 action=self.args["job_action"],
                 job_id=job_id,
                 project_id=self.project_id,
             )
             debug(response, 5)
 
             if not response:
                 error(
-                    f"Could not {self.args['job_action']} job #{job_id} for project '{self.project}'."
+                    f"Could not {self.args['job_action']} job #{job_id}"
+                    f" in project '{self.project}'."
                 )
             else:
                 cprint(
-                    f"Successfully {self.args['job_action']} job #{job_id} for project '{self.project}'",
+                    f"Successfully {self.args['job_action']} job #{job_id}"
+                    f" in project '{self.project}'",
                     color="green",
                     attrs=["bold"],
                 )
 
                 if self.args["job_action"] == "retry":
                     cprint(
                         f"New job id is #{response['id']}",
                         color="green",
                         attrs=["bold"],
                     )
 
-    @register_command(aliases={"validate"})
+    @register_command(aliases=frozenset({"validate"}))
     def lint(self):
         """Run gitlabcicli lint."""
         gitlabciyml_text = self.args["file"].read()
+        self.args["file"].close()
         debug(f"gitlabci.yml content:\n{gitlabciyml_text}", 5)
-        api = self.api_client.validate_ciyml(gitlabciyml_text=gitlabciyml_text)
+        api = self.api_client.validate_ciyml(
+            gitlabciyml_text=gitlabciyml_text,
+            project_id=self.project_id,
+        )
 
-        if api["status"] == "valid":
+        if api["valid"] is True:
             cprint(
                 ".gitlab-ci.yml is valid",
                 color="green",
                 attrs=["bold"],
             )
         else:
             cprint(
                 ".gitlab-ci.yml is invalid",
                 color="red",
                 attrs=["bold"],
             )
-            print("List of errors:")
 
-            for error_description in api["errors"]:
-                print(f" - {error_description}")
+            if api["warnings"]:
+                print("List of warnings:")
+
+                for error_description in api["warnings"]:
+                    cprint(f" - {error_description}", color="orange")
+
+            if api["errors"]:
+                print("List of errors:")
+
+                for error_description in api["errors"]:
+                    cprint(f" - {error_description}", color="red")
 
-    @register_command(aliases={"web"})
+    @register_command(aliases=frozenset({"web"}))
     def open(self):
         """Open the current project in browser."""
         url = self.api_client.get_project_url(self.project_id)
         webbrowser.open(url)
 
-    @register_command(aliases={"exec"})
+    @register_command(aliases=frozenset({"exec"}))
     def run_local(self):
         """Run pipeline on local machine."""
         raise NotImplementedError(
             "run_local is not yet implemented. Contribution is welcome."
         )
 
-    @register_command(aliases={"start"})
+    @register_command(aliases=frozenset({"start"}))
     def init(self):
         """Create a .gitlab-ci.yml."""
         # TODO ensure this is in git root
         file_path = Path(".gitlab-ci.yml")
 
         if file_path.is_file():
             error(f"{file_path} already exists")
```

### Comparing `gitlabcicli-0.2.5/gitlabcicli/gitwrapper.py` & `gitlabcicli-0.2.6/gitlabcicli/gitwrapper.py`

 * *Files identical despite different names*

### Comparing `gitlabcicli-0.2.5/gitlabcicli/keyring_wrapper.py` & `gitlabcicli-0.2.6/gitlabcicli/keyring_wrapper.py`

 * *Files identical despite different names*

### Comparing `gitlabcicli-0.2.5/gitlabcicli/script_helpers.py` & `gitlabcicli-0.2.6/gitlabcicli/script_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 
 """Some helperfunctions for clis."""
 
 import sys
+import typing
 
 from termcolor import cprint
 
 VERBOSITY = 5
 DEBUG_PRINT_LEVELS = [
     {"color": "blue", "attrs": ["bold"]},
     {"color": "blue", "attrs": []},
@@ -19,21 +20,22 @@
 
 def set_verbosity(verbosity):
     """sets the verbosity level of this script"""
     global VERBOSITY
     VERBOSITY = verbosity
 
 
-def error(message, exit_code: int = 1):
+def error(message, exit_code: int = 1) -> typing.NoReturn:
     """prints the message to stderr and exits"""
     cprint(f"[!] {message}", attrs=["bold"], color="red", file=sys.stderr)
     sys.exit(exit_code)
 
 
 def debug(message, min_debug_level):
     """prints the message to stdout if debug level >= min_debug_level"""
+
     if min_debug_level <= VERBOSITY:
         cprint(
             f"[i] {message}",
             color=DEBUG_PRINT_LEVELS[min_debug_level]["color"],
             attrs=DEBUG_PRINT_LEVELS[min_debug_level]["attrs"],
         )
```

### Comparing `gitlabcicli-0.2.5/pyproject.toml` & `gitlabcicli-0.2.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "GitLabCICli"
-version = "0.2.5"
+version = "0.2.6"
 description = "Command line interface for GitLab CI"
 authors = ["sedrubal <dev@sedrubal.de>"]
 repository = "https://gitlab.com/sedrubal/gitlabcicli.git"
 license = "GPL-3.0-or-later"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -15,18 +15,21 @@
 termcolor = "^1.1.0"
 GitPython = "^3.1.31"
 dbus-python = "^1.3.2"
 secretstorage = "^3.3.3"
 
 [tool.poetry.group.dev.dependencies]
 types-requests = "^2.28.11.17"
+types-tabulate = "^0.9.0.2"
+types-termcolor = "^1.1.6.2"
 pylint = "^2.17.3"
 mypy = "^1.2.0"
 black = "^22.12.0"
 pre-commit = "^2.21.0"
+ruff = "^0.0.272"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry.scripts]
 gitlabcicli = 'gitlabcicli.gitlabcicli:main'
```

### Comparing `gitlabcicli-0.2.5/PKG-INFO` & `gitlabcicli-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabcicli
-Version: 0.2.5
+Version: 0.2.6
 Summary: Command line interface for GitLab CI
 Home-page: https://gitlab.com/sedrubal/gitlabcicli.git
 License: GPL-3.0-or-later
 Author: sedrubal
 Author-email: dev@sedrubal.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

