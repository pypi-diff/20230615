# Comparing `tmp/laminci-0.7.0.tar.gz` & `tmp/laminci-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laminci-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "laminci-0.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `laminci-0.7.0.tar` & `laminci-0.7.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1096 2023-06-14 23:30:30.962603 laminci-0.7.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-02-23 20:36:15.651723 laminci-0.7.0/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-02-23 20:36:15.652253 laminci-0.7.0/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1194 2023-02-23 20:36:15.627521 laminci-0.7.0/.gitignore
--rw-r--r--   0        0        0     1770 2023-02-23 20:36:15.623232 laminci-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       29 2023-02-23 21:02:08.741159 laminci-0.7.0/README.md
--rw-r--r--   0        0        0     3534 2023-06-14 23:34:54.108176 laminci-0.7.0/docs/changelog.md
--rw-r--r--   0        0        0      339 2023-02-23 20:36:15.640096 laminci-0.7.0/docs/guide/index.md
--rw-r--r--   0        0        0     1415 2023-05-26 15:57:31.631988 laminci-0.7.0/docs/guide/quickstart.ipynb
--rw-r--r--   0        0        0        0 2023-02-23 21:02:08.741423 laminci-0.7.0/docs/index.md
--rw-r--r--   0        0        0      805 2023-02-23 20:36:15.648759 laminci-0.7.0/docs/notes/YYYY-MM-DD-my-design-choice.ipynb
--rw-r--r--   0        0        0      223 2023-02-23 20:36:15.647572 laminci-0.7.0/docs/notes/index.md
--rw-r--r--   0        0        0      122 2023-02-23 20:36:15.618482 laminci-0.7.0/lamin-project.yaml
--rw-r--r--   0        0        0      378 2023-06-14 23:34:49.431050 laminci-0.7.0/laminci/__init__.py
--rw-r--r--   0        0        0     2275 2023-06-14 23:30:30.962727 laminci-0.7.0/laminci/__main__.py
--rw-r--r--   0        0        0     2130 2023-06-14 22:24:13.327779 laminci-0.7.0/laminci/_artifacts.py
--rw-r--r--   0        0        0     1358 2023-05-26 16:17:30.304517 laminci-0.7.0/laminci/_db.py
--rw-r--r--   0        0        0      380 2023-02-23 22:56:58.478640 laminci-0.7.0/laminci/_docs.py
--rw-r--r--   0        0        0      948 2023-06-14 22:05:00.624145 laminci-0.7.0/laminci/_env.py
--rw-r--r--   0        0        0     2727 2023-06-01 09:34:04.219058 laminci-0.7.0/laminci/_nox.py
--rw-r--r--   0        0        0      148 2023-05-26 16:33:21.362381 laminci-0.7.0/laminci/db.py
--rw-r--r--   0        0        0      167 2023-02-23 21:55:02.625861 laminci-0.7.0/laminci/nox.py
--rw-r--r--   0        0        0      476 2023-06-14 23:30:30.962848 laminci-0.7.0/noxfile.py
--rw-r--r--   0        0        0      762 2023-06-14 23:30:30.962964 laminci-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      126 2023-05-26 16:17:30.304991 laminci-0.7.0/tests/test_artifacts.py
--rw-r--r--   0        0        0      104 2023-06-14 22:05:00.624370 laminci-0.7.0/tests/test_package_name.py
--rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 laminci-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-06-14 23:30:30.962603 laminci-0.7.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-02-23 20:36:15.651723 laminci-0.7.1/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-02-23 20:36:15.652253 laminci-0.7.1/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1194 2023-02-23 20:36:15.627521 laminci-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1770 2023-02-23 20:36:15.623232 laminci-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       29 2023-02-23 21:02:08.741159 laminci-0.7.1/README.md
+-rw-r--r--   0        0        0     3534 2023-06-14 23:40:19.460950 laminci-0.7.1/docs/changelog.md
+-rw-r--r--   0        0        0      339 2023-02-23 20:36:15.640096 laminci-0.7.1/docs/guide/index.md
+-rw-r--r--   0        0        0     1415 2023-05-26 15:57:31.631988 laminci-0.7.1/docs/guide/quickstart.ipynb
+-rw-r--r--   0        0        0        0 2023-02-23 21:02:08.741423 laminci-0.7.1/docs/index.md
+-rw-r--r--   0        0        0      805 2023-02-23 20:36:15.648759 laminci-0.7.1/docs/notes/YYYY-MM-DD-my-design-choice.ipynb
+-rw-r--r--   0        0        0      223 2023-02-23 20:36:15.647572 laminci-0.7.1/docs/notes/index.md
+-rw-r--r--   0        0        0      122 2023-02-23 20:36:15.618482 laminci-0.7.1/lamin-project.yaml
+-rw-r--r--   0        0        0      378 2023-06-14 23:40:19.461060 laminci-0.7.1/laminci/__init__.py
+-rw-r--r--   0        0        0     2314 2023-06-14 23:39:51.079821 laminci-0.7.1/laminci/__main__.py
+-rw-r--r--   0        0        0     2130 2023-06-14 22:24:13.327779 laminci-0.7.1/laminci/_artifacts.py
+-rw-r--r--   0        0        0     1358 2023-05-26 16:17:30.304517 laminci-0.7.1/laminci/_db.py
+-rw-r--r--   0        0        0      380 2023-02-23 22:56:58.478640 laminci-0.7.1/laminci/_docs.py
+-rw-r--r--   0        0        0      948 2023-06-14 22:05:00.624145 laminci-0.7.1/laminci/_env.py
+-rw-r--r--   0        0        0     2727 2023-06-01 09:34:04.219058 laminci-0.7.1/laminci/_nox.py
+-rw-r--r--   0        0        0      148 2023-05-26 16:33:21.362381 laminci-0.7.1/laminci/db.py
+-rw-r--r--   0        0        0      167 2023-02-23 21:55:02.625861 laminci-0.7.1/laminci/nox.py
+-rw-r--r--   0        0        0      476 2023-06-14 23:30:30.962848 laminci-0.7.1/noxfile.py
+-rw-r--r--   0        0        0      762 2023-06-14 23:30:30.962964 laminci-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      126 2023-05-26 16:17:30.304991 laminci-0.7.1/tests/test_artifacts.py
+-rw-r--r--   0        0        0      104 2023-06-14 22:05:00.624370 laminci-0.7.1/tests/test_package_name.py
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 laminci-0.7.1/PKG-INFO
```

### Comparing `laminci-0.7.0/.github/workflows/build.yml` & `laminci-0.7.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `laminci-0.7.0/.github/workflows/latest-changes.yml` & `laminci-0.7.1/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `laminci-0.7.0/.gitignore` & `laminci-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `laminci-0.7.0/.pre-commit-config.yaml` & `laminci-0.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `laminci-0.7.0/docs/changelog.md` & `laminci-0.7.1/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
-🚸 Add light-weight release management | [23](https://github.com/laminlabs/laminci/pull/23) | [falexwolf](https://github.com/falexwolf) | 2023-06-14 | 0.7.0
+🚸 Add light-weight release management | [23](https://github.com/laminlabs/laminci/pull/23) | [falexwolf](https://github.com/falexwolf) | 2023-06-14 | 0.7.1
 ✨ Add `repository_dispatch` for docs upload | [22](https://github.com/laminlabs/laminci/pull/22) | [falexwolf](https://github.com/falexwolf) | 2023-06-14 | 0.6.8
 🚸 Add fallback for `get_package_name` | [21](https://github.com/laminlabs/laminci/pull/21) | [falexwolf](https://github.com/falexwolf) | 2023-06-14 | 0.6.7
 ✨ Add aws cli based way of pushing a docs artifact | [20](https://github.com/laminlabs/laminci/pull/20) | [falexwolf](https://github.com/falexwolf) | 2023-05-26 | 0.6.4
 🚸 Allow passing version to `setup_local_test_postgres` | [19](https://github.com/laminlabs/laminci/pull/19) | [falexwolf](https://github.com/falexwolf) | 2023-04-20 |
 🚸 Close current instance before uploading docs artifacts | [17](https://github.com/laminlabs/laminci/pull/17) | [falexwolf](https://github.com/falexwolf) | 2023-04-10 | 0.5.3
 🚸 Add support for environments | [16](https://github.com/laminlabs/laminci/pull/16) | [falexwolf](https://github.com/falexwolf) | 2023-04-10 | 0.5.1
 ⬆️ Upgrade to new replace API | [15](https://github.com/laminlabs/laminci/pull/15) | [falexwolf](https://github.com/falexwolf) | 2023-04-10 | 0.5.0
```

### Comparing `laminci-0.7.0/docs/guide/quickstart.ipynb` & `laminci-0.7.1/docs/guide/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `laminci-0.7.0/docs/notes/YYYY-MM-DD-my-design-choice.ipynb` & `laminci-0.7.1/docs/notes/YYYY-MM-DD-my-design-choice.ipynb`

 * *Files identical despite different names*

### Comparing `laminci-0.7.0/laminci/__main__.py` & `laminci-0.7.1/laminci/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,13 +57,14 @@
                 f"Your version ({version}) should increment the previous version"
                 f" ({previous_version})"
             )
         pypi = " & publish to PyPI" if args.pypi else ""
         response = input(f"Bump {previous_version} to {version}{pypi}? (y/n)")
         if response != "y":
             return None
-        run(f"git commit -m 'Release {version}", shell=True)
+        run("git add -u", shell=True)
+        run(f"git commit -m 'Release {version}'", shell=True)
         run("git push", shell=True)
         run(f"git tag {version}", shell=True)
         run(f"git tag push origin {version}", shell=True)
         if args.pypi:
             run("flit publish", shell=True)
```

### Comparing `laminci-0.7.0/laminci/_artifacts.py` & `laminci-0.7.1/laminci/_artifacts.py`

 * *Files identical despite different names*

### Comparing `laminci-0.7.0/laminci/_db.py` & `laminci-0.7.1/laminci/_db.py`

 * *Files identical despite different names*

### Comparing `laminci-0.7.0/laminci/_env.py` & `laminci-0.7.1/laminci/_env.py`

 * *Files identical despite different names*

### Comparing `laminci-0.7.0/laminci/_nox.py` & `laminci-0.7.1/laminci/_nox.py`

 * *Files identical despite different names*

### Comparing `laminci-0.7.0/pyproject.toml` & `laminci-0.7.1/pyproject.toml`

 * *Files identical despite different names*

