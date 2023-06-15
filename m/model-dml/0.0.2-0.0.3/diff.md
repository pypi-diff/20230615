# Comparing `tmp/model_dml-0.0.2.tar.gz` & `tmp/model_dml-0.0.3.tar.gz`

## Comparing `model_dml-0.0.2.tar` & `model_dml-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 model_dml-0.0.2/.flake8
--rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 model_dml-0.0.2/.gitlab-ci.yml
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 model_dml-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 model_dml-0.0.2/CONTRIBUTING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 model_dml-0.0.2/build_requirements.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 model_dml-0.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 model_dml-0.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 model_dml-0.0.2/.idea/modml.iml
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 model_dml-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 model_dml-0.0.2/.idea/vcs.xml
--rw-r--r--   0        0        0    13128 2020-02-02 00:00:00.000000 model_dml-0.0.2/.idea/workspace.xml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 model_dml-0.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 model_dml-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 model_dml-0.0.2/src/model_dml/__init__.py
--rw-r--r--   0        0        0     6626 2020-02-02 00:00:00.000000 model_dml-0.0.2/src/model_dml/dml.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 model_dml-0.0.2/src/model_dml/py.typed
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 model_dml-0.0.2/tests/conftest.py
--rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 model_dml-0.0.2/tests/test_main.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 model_dml-0.0.2/.gitignore
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 model_dml-0.0.2/AUTHORS.rst
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 model_dml-0.0.2/LICENCE
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 model_dml-0.0.2/README.md
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 model_dml-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 model_dml-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 model_dml-0.0.3/.flake8
+-rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 model_dml-0.0.3/.gitlab-ci.yml
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 model_dml-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 model_dml-0.0.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 model_dml-0.0.3/build_requirements.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 model_dml-0.0.3/.idea/.gitignore
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 model_dml-0.0.3/.idea/misc.xml
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 model_dml-0.0.3/.idea/modml.iml
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 model_dml-0.0.3/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 model_dml-0.0.3/.idea/vcs.xml
+-rw-r--r--   0        0        0    13128 2020-02-02 00:00:00.000000 model_dml-0.0.3/.idea/workspace.xml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 model_dml-0.0.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 model_dml-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 model_dml-0.0.3/src/model_dml/__init__.py
+-rw-r--r--   0        0        0     6590 2020-02-02 00:00:00.000000 model_dml-0.0.3/src/model_dml/dml.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 model_dml-0.0.3/src/model_dml/py.typed
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 model_dml-0.0.3/tests/conftest.py
+-rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 model_dml-0.0.3/tests/test_main.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 model_dml-0.0.3/.gitignore
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 model_dml-0.0.3/AUTHORS.rst
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 model_dml-0.0.3/LICENCE
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 model_dml-0.0.3/README.md
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 model_dml-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 model_dml-0.0.3/PKG-INFO
```

### Comparing `model_dml-0.0.2/.gitlab-ci.yml` & `model_dml-0.0.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `model_dml-0.0.2/CONTRIBUTING.md` & `model_dml-0.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `model_dml-0.0.2/.idea/workspace.xml` & `model_dml-0.0.3/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `model_dml-0.0.2/.idea/inspectionProfiles/Project_Default.xml` & `model_dml-0.0.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `model_dml-0.0.2/src/model_dml/dml.py` & `model_dml-0.0.3/src/model_dml/dml.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 
 import sqlalchemy.orm
 
 SingleExecuteParams = typing.Mapping[str, typing.Any]
 MultiExecuteParams = typing.Sequence[SingleExecuteParams]
 AnyExecuteParams = typing.Union[MultiExecuteParams, SingleExecuteParams]
 
-COLUMNS_CLAUSE_ARGUMENT = typing.TypeVar(
-    "COLUMNS_CLAUSE_ARGUMENT",
-    bound=sqlalchemy.sql._typing._ColumnsClauseArgument[typing.Any],
-)
+COLUMNS_CLAUSE_ARGUMENT: typing.TypeAlias = sqlalchemy.sql._typing._ColumnsClauseArgument[
+    typing.Any
+]
 
 
 class SessionMakerMixin:
     @classmethod
     def session_maker(cls) -> sqlalchemy.orm.sessionmaker:
         raise NotImplementedError(
             """
```

### Comparing `model_dml-0.0.2/tests/conftest.py` & `model_dml-0.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `model_dml-0.0.2/tests/test_main.py` & `model_dml-0.0.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `model_dml-0.0.2/.gitignore` & `model_dml-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `model_dml-0.0.2/LICENCE` & `model_dml-0.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `model_dml-0.0.2/README.md` & `model_dml-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `model_dml-0.0.2/pyproject.toml` & `model_dml-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "model_dml"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "Dorian Turba", email = "contact.5oldw@8shield.net" },
 ]
 description = "A package for SQLAlchemy models DML mixins."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `model_dml-0.0.2/PKG-INFO` & `model_dml-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model_dml
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for SQLAlchemy models DML mixins.
 Project-URL: Homepage, https://lab.frogg.it/dorianturba/model_dml
 Project-URL: Bug Tracker, https://lab.frogg.it/dorianturba/model_dml
 Author-email: Dorian Turba <contact.5oldw@8shield.net>
 License-File: AUTHORS.rst
 License-File: LICENCE
 Classifier: Development Status :: 3 - Alpha
```

