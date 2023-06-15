# Comparing `tmp/shaku_database-0.0.1.tar.gz` & `tmp/shaku_database-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaku_database-0.0.1.tar", last modified: Thu Jun 15 07:58:15 2023, max compression
+gzip compressed data, was "shaku_database-1.0.0.tar", last modified: Thu Jun 15 08:25:29 2023, max compression
```

## Comparing `shaku_database-0.0.1.tar` & `shaku_database-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 07:58:15.989316 shaku_database-0.0.1/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     6618 2023-06-15 07:58:15.989206 shaku_database-0.0.1/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)     6177 2023-06-15 07:54:10.000000 shaku_database-0.0.1/README.md
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 07:58:15.988603 shaku_database-0.0.1/database/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku_database-0.0.1/database/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-06-15 07:58:15.989355 shaku_database-0.0.1/setup.cfg
--rw-r--r--   0 tongyuhao   (501) staff       (20)      715 2023-06-15 07:57:50.000000 shaku_database-0.0.1/setup.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 07:58:15.989049 shaku_database-0.0.1/shaku_database.egg-info/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     6618 2023-06-15 07:58:15.000000 shaku_database-0.0.1/shaku_database.egg-info/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)      191 2023-06-15 07:58:15.000000 shaku_database-0.0.1/shaku_database.egg-info/SOURCES.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-06-15 07:58:15.000000 shaku_database-0.0.1/shaku_database.egg-info/dependency_links.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)        9 2023-06-15 07:58:15.000000 shaku_database-0.0.1/shaku_database.egg-info/top_level.txt
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 08:25:29.575956 shaku_database-1.0.0/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku_database-1.0.0/LICENSE
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7197 2023-06-15 08:25:29.575837 shaku_database-1.0.0/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku_database-1.0.0/README.md
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 08:25:29.575102 shaku_database-1.0.0/database/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku_database-1.0.0/database/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-06-15 08:25:29.575996 shaku_database-1.0.0/setup.cfg
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1015 2023-06-15 08:25:25.000000 shaku_database-1.0.0/setup.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 08:25:29.575656 shaku_database-1.0.0/shaku_database.egg-info/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7197 2023-06-15 08:25:29.000000 shaku_database-1.0.0/shaku_database.egg-info/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)      236 2023-06-15 08:25:29.000000 shaku_database-1.0.0/shaku_database.egg-info/SOURCES.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-06-15 08:25:29.000000 shaku_database-1.0.0/shaku_database.egg-info/dependency_links.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)      417 2023-06-15 08:25:29.000000 shaku_database-1.0.0/shaku_database.egg-info/requires.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        9 2023-06-15 08:25:29.000000 shaku_database-1.0.0/shaku_database.egg-info/top_level.txt
```

### Comparing `shaku_database-0.0.1/PKG-INFO` & `shaku_database-1.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,8 @@
-Metadata-Version: 2.1
-Name: shaku_database
-Version: 0.0.1
-Summary: Shaku Database util
-Home-page: https://gitlab.com/hawktorng1/test_shaku
-Author: hawktorng
-Author-email: hawktorng@shaku.com.tw
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# test_shaku
+# shaku_data_util
 
 
 
 ## Getting started
 
 To make it easy for you to get started with GitLab, here's a list of recommended next steps.
 
@@ -26,22 +11,22 @@
 ## Add your files
 
 - [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
 - [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:
 
 ```
 cd existing_repo
-git remote add origin https://gitlab.com/hawktorng1/test_shaku.git
+git remote add origin https://gitlab.com/hawktorng1/shaku_data_util.git
 git branch -M main
 git push -uf origin main
 ```
 
 ## Integrate with your tools
 
-- [ ] [Set up project integrations](https://gitlab.com/hawktorng1/test_shaku/-/settings/integrations)
+- [ ] [Set up project integrations](https://gitlab.com/hawktorng1/shaku_data_util/-/settings/integrations)
 
 ## Collaborate with your team
 
 - [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
 - [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
 - [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
 - [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
@@ -101,9 +86,7 @@
 Show your appreciation to those who have contributed to the project.
 
 ## License
 For open source projects, say how it is licensed.
 
 ## Project status
 If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
-
-
```

### Comparing `shaku_database-0.0.1/README.md` & `shaku_database-1.0.0/shaku_database.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,43 @@
-# test_shaku
+Metadata-Version: 2.1
+Name: shaku-database
+Version: 1.0.0
+Summary: Shaku Database util
+Home-page: https://gitlab.com/hawktorng1/test_shaku
+Author: hawktorng
+Author-email: hawktorng@shaku.com.tw
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: db-dtypes
+Provides-Extra: google-api-core
+Provides-Extra: google-auth
+Provides-Extra: google-cloud-bigquery
+Provides-Extra: google-cloud-core
+Provides-Extra: google-cloud-storage
+Provides-Extra: google-crc32c
+Provides-Extra: google-resumable-media
+Provides-Extra: googleapis-common-protos
+Provides-Extra: numpy
+Provides-Extra: openpyxl
+Provides-Extra: pandas
+Provides-Extra: pyarrow
+Provides-Extra: PyMySQL
+Provides-Extra: requests
+Provides-Extra: rsa
+Provides-Extra: setuptools
+Provides-Extra: six
+Provides-Extra: sqlalchemy
+License-File: LICENSE
+
+# shaku_data_util
 
 
 
 ## Getting started
 
 To make it easy for you to get started with GitLab, here's a list of recommended next steps.
 
@@ -11,22 +46,22 @@
 ## Add your files
 
 - [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
 - [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:
 
 ```
 cd existing_repo
-git remote add origin https://gitlab.com/hawktorng1/test_shaku.git
+git remote add origin https://gitlab.com/hawktorng1/shaku_data_util.git
 git branch -M main
 git push -uf origin main
 ```
 
 ## Integrate with your tools
 
-- [ ] [Set up project integrations](https://gitlab.com/hawktorng1/test_shaku/-/settings/integrations)
+- [ ] [Set up project integrations](https://gitlab.com/hawktorng1/shaku_data_util/-/settings/integrations)
 
 ## Collaborate with your team
 
 - [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
 - [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
 - [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
 - [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
@@ -86,7 +121,9 @@
 Show your appreciation to those who have contributed to the project.
 
 ## License
 For open source projects, say how it is licensed.
 
 ## Project status
 If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
+
+
```

### Comparing `shaku_database-0.0.1/shaku_database.egg-info/PKG-INFO` & `shaku_database-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,43 @@
 Metadata-Version: 2.1
-Name: shaku-database
-Version: 0.0.1
+Name: shaku_database
+Version: 1.0.0
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: db-dtypes
+Provides-Extra: google-api-core
+Provides-Extra: google-auth
+Provides-Extra: google-cloud-bigquery
+Provides-Extra: google-cloud-core
+Provides-Extra: google-cloud-storage
+Provides-Extra: google-crc32c
+Provides-Extra: google-resumable-media
+Provides-Extra: googleapis-common-protos
+Provides-Extra: numpy
+Provides-Extra: openpyxl
+Provides-Extra: pandas
+Provides-Extra: pyarrow
+Provides-Extra: PyMySQL
+Provides-Extra: requests
+Provides-Extra: rsa
+Provides-Extra: setuptools
+Provides-Extra: six
+Provides-Extra: sqlalchemy
+License-File: LICENSE
 
-# test_shaku
+# shaku_data_util
 
 
 
 ## Getting started
 
 To make it easy for you to get started with GitLab, here's a list of recommended next steps.
 
@@ -26,22 +46,22 @@
 ## Add your files
 
 - [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
 - [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:
 
 ```
 cd existing_repo
-git remote add origin https://gitlab.com/hawktorng1/test_shaku.git
+git remote add origin https://gitlab.com/hawktorng1/shaku_data_util.git
 git branch -M main
 git push -uf origin main
 ```
 
 ## Integrate with your tools
 
-- [ ] [Set up project integrations](https://gitlab.com/hawktorng1/test_shaku/-/settings/integrations)
+- [ ] [Set up project integrations](https://gitlab.com/hawktorng1/shaku_data_util/-/settings/integrations)
 
 ## Collaborate with your team
 
 - [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
 - [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
 - [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
 - [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
```

