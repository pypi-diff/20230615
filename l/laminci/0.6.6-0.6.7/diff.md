# Comparing `tmp/laminci-0.6.6.tar.gz` & `tmp/laminci-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laminci-0.6.6.tar", last modified: Thu Jun  1 09:34:58 2023, max compression
+gzip compressed data, was "laminci-0.6.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `laminci-0.6.6.tar` & `laminci-0.6.7.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     1371 2023-02-23 21:08:15.192204 laminci-0.6.6/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-02-23 20:36:15.651723 laminci-0.6.6/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-02-23 20:36:15.652253 laminci-0.6.6/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1194 2023-02-23 20:36:15.627521 laminci-0.6.6/.gitignore
--rw-r--r--   0        0        0     1770 2023-02-23 20:36:15.623232 laminci-0.6.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0       29 2023-02-23 21:02:08.741159 laminci-0.6.6/README.md
--rw-r--r--   0        0        0     3052 2023-05-30 09:01:05.110946 laminci-0.6.6/docs/changelog.md
--rw-r--r--   0        0        0      339 2023-02-23 20:36:15.640096 laminci-0.6.6/docs/guide/index.md
--rw-r--r--   0        0        0     1415 2023-05-26 15:57:31.631988 laminci-0.6.6/docs/guide/quickstart.ipynb
--rw-r--r--   0        0        0        0 2023-02-23 21:02:08.741423 laminci-0.6.6/docs/index.md
--rw-r--r--   0        0        0      805 2023-02-23 20:36:15.648759 laminci-0.6.6/docs/notes/YYYY-MM-DD-my-design-choice.ipynb
--rw-r--r--   0        0        0      223 2023-02-23 20:36:15.647572 laminci-0.6.6/docs/notes/index.md
--rw-r--r--   0        0        0      122 2023-02-23 20:36:15.618482 laminci-0.6.6/lamin-project.yaml
--rw-r--r--   0        0        0      378 2023-06-01 09:34:38.124922 laminci-0.6.6/laminci/__init__.py
--rw-r--r--   0        0        0     2122 2023-05-26 16:17:30.304228 laminci-0.6.6/laminci/_artifacts.py
--rw-r--r--   0        0        0     1358 2023-05-26 16:17:30.304517 laminci-0.6.6/laminci/_db.py
--rw-r--r--   0        0        0      380 2023-02-23 22:56:58.478640 laminci-0.6.6/laminci/_docs.py
--rw-r--r--   0        0        0      737 2023-02-23 22:56:58.478807 laminci-0.6.6/laminci/_env.py
--rw-r--r--   0        0        0     2727 2023-06-01 09:34:04.219058 laminci-0.6.6/laminci/_nox.py
--rw-r--r--   0        0        0      148 2023-05-26 16:33:21.362381 laminci-0.6.6/laminci/db.py
--rw-r--r--   0        0        0      167 2023-02-23 21:55:02.625861 laminci-0.6.6/laminci/nox.py
--rw-r--r--   0        0        0      497 2023-02-23 21:02:08.742361 laminci-0.6.6/noxfile.py
--rw-r--r--   0        0        0      708 2023-05-28 21:50:19.140197 laminci-0.6.6/pyproject.toml
--rw-r--r--   0        0        0      126 2023-05-26 16:17:30.304991 laminci-0.6.6/tests/test_artifacts.py
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 laminci-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0     1371 2023-02-23 21:08:15.192204 laminci-0.6.7/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-02-23 20:36:15.651723 laminci-0.6.7/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-02-23 20:36:15.652253 laminci-0.6.7/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1194 2023-02-23 20:36:15.627521 laminci-0.6.7/.gitignore
+-rw-r--r--   0        0        0     1770 2023-02-23 20:36:15.623232 laminci-0.6.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       29 2023-02-23 21:02:08.741159 laminci-0.6.7/README.md
+-rw-r--r--   0        0        0     3211 2023-06-14 22:05:32.502528 laminci-0.6.7/docs/changelog.md
+-rw-r--r--   0        0        0      339 2023-02-23 20:36:15.640096 laminci-0.6.7/docs/guide/index.md
+-rw-r--r--   0        0        0     1415 2023-05-26 15:57:31.631988 laminci-0.6.7/docs/guide/quickstart.ipynb
+-rw-r--r--   0        0        0        0 2023-02-23 21:02:08.741423 laminci-0.6.7/docs/index.md
+-rw-r--r--   0        0        0      805 2023-02-23 20:36:15.648759 laminci-0.6.7/docs/notes/YYYY-MM-DD-my-design-choice.ipynb
+-rw-r--r--   0        0        0      223 2023-02-23 20:36:15.647572 laminci-0.6.7/docs/notes/index.md
+-rw-r--r--   0        0        0      122 2023-02-23 20:36:15.618482 laminci-0.6.7/lamin-project.yaml
+-rw-r--r--   0        0        0      378 2023-06-14 22:05:25.872250 laminci-0.6.7/laminci/__init__.py
+-rw-r--r--   0        0        0     2122 2023-05-26 16:17:30.304228 laminci-0.6.7/laminci/_artifacts.py
+-rw-r--r--   0        0        0     1358 2023-05-26 16:17:30.304517 laminci-0.6.7/laminci/_db.py
+-rw-r--r--   0        0        0      380 2023-02-23 22:56:58.478640 laminci-0.6.7/laminci/_docs.py
+-rw-r--r--   0        0        0      948 2023-06-14 22:05:00.624145 laminci-0.6.7/laminci/_env.py
+-rw-r--r--   0        0        0     2727 2023-06-01 09:34:04.219058 laminci-0.6.7/laminci/_nox.py
+-rw-r--r--   0        0        0      148 2023-05-26 16:33:21.362381 laminci-0.6.7/laminci/db.py
+-rw-r--r--   0        0        0      167 2023-02-23 21:55:02.625861 laminci-0.6.7/laminci/nox.py
+-rw-r--r--   0        0        0      497 2023-02-23 21:02:08.742361 laminci-0.6.7/noxfile.py
+-rw-r--r--   0        0        0      720 2023-06-14 22:05:00.624279 laminci-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0      126 2023-05-26 16:17:30.304991 laminci-0.6.7/tests/test_artifacts.py
+-rw-r--r--   0        0        0      104 2023-06-14 22:05:00.624370 laminci-0.6.7/tests/test_package_name.py
+-rw-r--r--   0        0        0      515 1970-01-01 00:00:00.000000 laminci-0.6.7/PKG-INFO
```

### Comparing `laminci-0.6.6/.github/workflows/build.yml` & `laminci-0.6.7/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `laminci-0.6.6/.github/workflows/latest-changes.yml` & `laminci-0.6.7/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `laminci-0.6.6/.gitignore` & `laminci-0.6.7/.gitignore`

 * *Files identical despite different names*

### Comparing `laminci-0.6.6/.pre-commit-config.yaml` & `laminci-0.6.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `laminci-0.6.6/docs/changelog.md` & `laminci-0.6.7/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🚸 Add fallback for `get_package_name` | [21](https://github.com/laminlabs/laminci/pull/21) | [falexwolf](https://github.com/falexwolf) | 2023-06-14 | 0.6.7
 ✨ Add aws cli based way of pushing a docs artifact | [20](https://github.com/laminlabs/laminci/pull/20) | [falexwolf](https://github.com/falexwolf) | 2023-05-26 | 0.6.4
 🚸 Allow passing version to `setup_local_test_postgres` | [19](https://github.com/laminlabs/laminci/pull/19) | [falexwolf](https://github.com/falexwolf) | 2023-04-20 |
 🚸 Close current instance before uploading docs artifacts | [17](https://github.com/laminlabs/laminci/pull/17) | [falexwolf](https://github.com/falexwolf) | 2023-04-10 | 0.5.3
 🚸 Add support for environments | [16](https://github.com/laminlabs/laminci/pull/16) | [falexwolf](https://github.com/falexwolf) | 2023-04-10 | 0.5.1
 ⬆️ Upgrade to new replace API | [15](https://github.com/laminlabs/laminci/pull/15) | [falexwolf](https://github.com/falexwolf) | 2023-04-10 | 0.5.0
 ♻️ Replace `lndb` with `lamin` | [14](https://github.com/laminlabs/laminci/pull/14) | [falexwolf](https://github.com/falexwolf) | 2023-03-29 | 0.4.2
 🚸 Replace git checkout with git switch | [13](https://github.com/laminlabs/laminci/pull/13) | [falexwolf](https://github.com/falexwolf) | 2023-03-27 | 0.4.1
```

### Comparing `laminci-0.6.6/docs/guide/quickstart.ipynb` & `laminci-0.6.7/docs/guide/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `laminci-0.6.6/docs/notes/YYYY-MM-DD-my-design-choice.ipynb` & `laminci-0.6.7/docs/notes/YYYY-MM-DD-my-design-choice.ipynb`

 * *Files identical despite different names*

### Comparing `laminci-0.6.6/laminci/_artifacts.py` & `laminci-0.6.7/laminci/_artifacts.py`

 * *Files identical despite different names*

### Comparing `laminci-0.6.6/laminci/_db.py` & `laminci-0.6.7/laminci/_db.py`

 * *Files identical despite different names*

### Comparing `laminci-0.6.6/laminci/_nox.py` & `laminci-0.6.7/laminci/_nox.py`

 * *Files identical despite different names*

### Comparing `laminci-0.6.6/pyproject.toml` & `laminci-0.6.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 dynamic = ["version", "description"]
 dependencies = [
     # this CANNOT depend on lamindb as long as we use it
     # as an upstream dependency within lndb!
     "nox",
     "lamin_logger",
     "pyyaml",
+    "toml",
 ]
 
 [project.urls]
 Home = "https://github.com/laminlabs/laminci"
 
 [project.optional-dependencies]
 dev = [
```

