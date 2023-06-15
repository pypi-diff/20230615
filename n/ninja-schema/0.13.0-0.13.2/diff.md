# Comparing `tmp/ninja-schema-0.13.0.tar.gz` & `tmp/ninja_schema-0.13.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ninja-schema-0.13.0.tar", last modified: Tue Sep  6 15:18:36 2022, max compression
+gzip compressed data, was "ninja_schema-0.13.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ninja-schema-0.13.0.tar` & `ninja_schema-0.13.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rwxr-xr-x   0        0        0       65 2022-09-06 15:18:15.231530 ninja-schema-0.13.0/.dockerignore
--rwxr-xr-x   0        0        0      104 2022-09-06 15:18:15.231530 ninja-schema-0.13.0/.flake8
--rw-r--r--   0        0        0      594 2022-09-06 15:18:15.231530 ninja-schema-0.13.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      531 2022-09-06 15:18:15.231530 ninja-schema-0.13.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1269 2022-09-06 15:18:15.231530 ninja-schema-0.13.0/.github/workflows/test_full.yml
--rwxr-xr-x   0        0        0      108 2022-09-06 15:18:15.231530 ninja-schema-0.13.0/.gitignore
--rw-r--r--   0        0        0       52 2022-09-06 15:18:15.231530 ninja-schema-0.13.0/.isort.cfg
--rwxr-xr-x   0        0        0     1082 2022-09-06 15:18:15.231530 ninja-schema-0.13.0/LICENSE
--rw-r--r--   0        0        0      862 2022-09-06 15:18:15.231530 ninja-schema-0.13.0/Makefile
--rwxr-xr-x   0        0        0     9121 2022-09-06 15:18:15.231530 ninja-schema-0.13.0/README.md
--rw-r--r--   0        0        0      419 2022-09-06 15:18:15.231530 ninja-schema-0.13.0/mypy.ini
--rwxr-xr-x   0        0        0      361 2022-09-06 15:18:15.231530 ninja-schema-0.13.0/ninja_schema/__init__.py
--rwxr-xr-x   0        0        0      403 2022-09-06 15:18:15.231530 ninja-schema-0.13.0/ninja_schema/compat.py
--rw-r--r--   0        0        0       41 2022-09-06 15:18:15.231530 ninja-schema-0.13.0/ninja_schema/errors.py
--rwxr-xr-x   0        0        0        1 2022-09-06 15:18:15.231530 ninja-schema-0.13.0/ninja_schema/orm/__init__.py
--rwxr-xr-x   0        0        0     1864 2022-09-06 15:18:15.231530 ninja-schema-0.13.0/ninja_schema/orm/factory.py
--rw-r--r--   0        0        0      846 2022-09-06 15:18:15.231530 ninja-schema-0.13.0/ninja_schema/orm/getters.py
--rw-r--r--   0        0        0      432 2022-09-06 15:18:15.231530 ninja-schema-0.13.0/ninja_schema/orm/mixins.py
--rwxr-xr-x   0        0        0    13898 2022-09-06 15:18:15.231530 ninja-schema-0.13.0/ninja_schema/orm/model_schema.py
--rwxr-xr-x   0        0        0     2849 2022-09-06 15:18:15.231530 ninja-schema-0.13.0/ninja_schema/orm/model_validators.py
--rwxr-xr-x   0        0        0      217 2022-09-06 15:18:15.231530 ninja-schema-0.13.0/ninja_schema/orm/schema.py
--rwxr-xr-x   0        0        0     1691 2022-09-06 15:18:15.231530 ninja-schema-0.13.0/ninja_schema/orm/schema_registry.py
--rwxr-xr-x   0        0        0        0 2022-09-06 15:18:15.235530 ninja-schema-0.13.0/ninja_schema/orm/utils/__init__.py
--rwxr-xr-x   0        0        0    13732 2022-09-06 15:18:15.235530 ninja-schema-0.13.0/ninja_schema/orm/utils/converter.py
--rwxr-xr-x   0        0        0      307 2022-09-06 15:18:15.235530 ninja-schema-0.13.0/ninja_schema/orm/utils/utils.py
--rwxr-xr-x   0        0        0     1322 2022-09-06 15:18:15.235530 ninja-schema-0.13.0/ninja_schema/pydanticutils/__init__.py
--rw-r--r--   0        0        0       61 2022-09-06 15:18:15.235530 ninja-schema-0.13.0/ninja_schema/types.py
--rwxr-xr-x   0        0        0     1896 2022-09-06 15:18:15.235530 ninja-schema-0.13.0/pyproject.toml
--rw-r--r--   0        0        0       61 2022-09-06 15:18:15.235530 ninja-schema-0.13.0/pytest.ini
--rw-r--r--   0        0        0        0 2022-09-06 15:18:15.235530 ninja-schema-0.13.0/tests/__init__.py
--rw-r--r--   0        0        0     2085 2022-09-06 15:18:15.235530 ninja-schema-0.13.0/tests/conftest.py
--rw-r--r--   0        0        0      800 2022-09-06 15:18:15.235530 ninja-schema-0.13.0/tests/models.py
--rw-r--r--   0        0        0    11600 2022-09-06 15:18:15.235530 ninja-schema-0.13.0/tests/test_converters.py
--rw-r--r--   0        0        0     2547 2022-09-06 15:18:15.235530 ninja-schema-0.13.0/tests/test_custom_fields.py
--rw-r--r--   0        0        0    12213 2022-09-06 15:18:15.235530 ninja-schema-0.13.0/tests/test_model_schema.py
--rw-r--r--   0        0        0     1817 2022-09-06 15:18:15.235530 ninja-schema-0.13.0/tests/test_schema.py
--rw-r--r--   0        0        0       18 2022-09-06 15:18:15.235530 ninja-schema-0.13.0/tests/urls.py
--rw-r--r--   0        0        0    11351 1970-01-01 00:00:00.000000 ninja-schema-0.13.0/PKG-INFO
+-rwxr-xr-x   0        0        0       65 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/.dockerignore
+-rwxr-xr-x   0        0        0      104 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/.flake8
+-rw-r--r--   0        0        0      594 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      531 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1271 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/.github/workflows/test_full.yml
+-rwxr-xr-x   0        0        0      108 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/.gitignore
+-rw-r--r--   0        0        0       52 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/.isort.cfg
+-rwxr-xr-x   0        0        0     1082 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/LICENSE
+-rw-r--r--   0        0        0      862 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/Makefile
+-rwxr-xr-x   0        0        0     9120 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/README.md
+-rw-r--r--   0        0        0      419 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/mypy.ini
+-rwxr-xr-x   0        0        0      361 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/ninja_schema/__init__.py
+-rwxr-xr-x   0        0        0      403 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/ninja_schema/compat.py
+-rw-r--r--   0        0        0       41 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/ninja_schema/errors.py
+-rwxr-xr-x   0        0        0        1 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/ninja_schema/orm/__init__.py
+-rwxr-xr-x   0        0        0     1864 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/ninja_schema/orm/factory.py
+-rw-r--r--   0        0        0      846 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/ninja_schema/orm/getters.py
+-rw-r--r--   0        0        0      432 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/ninja_schema/orm/mixins.py
+-rwxr-xr-x   0        0        0    14161 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/ninja_schema/orm/model_schema.py
+-rwxr-xr-x   0        0        0     2849 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/ninja_schema/orm/model_validators.py
+-rwxr-xr-x   0        0        0      217 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/ninja_schema/orm/schema.py
+-rwxr-xr-x   0        0        0     1691 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/ninja_schema/orm/schema_registry.py
+-rwxr-xr-x   0        0        0        0 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/ninja_schema/orm/utils/__init__.py
+-rwxr-xr-x   0        0        0    13732 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/ninja_schema/orm/utils/converter.py
+-rwxr-xr-x   0        0        0      307 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/ninja_schema/orm/utils/utils.py
+-rwxr-xr-x   0        0        0     1322 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/ninja_schema/pydanticutils/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/ninja_schema/types.py
+-rwxr-xr-x   0        0        0     1912 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/pytest.ini
+-rw-r--r--   0        0        0        0 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/tests/__init__.py
+-rw-r--r--   0        0        0     2085 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/tests/conftest.py
+-rw-r--r--   0        0        0      800 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/tests/models.py
+-rw-r--r--   0        0        0    11600 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/tests/test_converters.py
+-rw-r--r--   0        0        0     2547 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/tests/test_custom_fields.py
+-rw-r--r--   0        0        0    12690 2023-06-15 20:03:37.200468 ninja_schema-0.13.2/tests/test_model_schema.py
+-rw-r--r--   0        0        0     1817 2023-06-15 20:03:37.204468 ninja_schema-0.13.2/tests/test_schema.py
+-rw-r--r--   0        0        0       18 2023-06-15 20:03:37.204468 ninja_schema-0.13.2/tests/urls.py
+-rw-r--r--   0        0        0    11361 1970-01-01 00:00:00.000000 ninja_schema-0.13.2/PKG-INFO
```

### Comparing `ninja-schema-0.13.0/.github/workflows/publish.yml` & `ninja_schema-0.13.2/.github/workflows/publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   publish:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python
         uses: actions/setup-python@v1
         with:
-          python-version: 3.6
+          python-version: 3.8
       - name: Install Flit
         run: pip install flit
       - name: Install Dependencies
         run: flit install --symlink
       - name: Publish
         env:
           FLIT_USERNAME: ${{ secrets.FLIT_USERNAME }}
```

### Comparing `ninja-schema-0.13.0/.github/workflows/test.yml` & `ninja_schema-0.13.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ninja-schema-0.13.0/.github/workflows/test_full.yml` & `ninja_schema-0.13.2/.github/workflows/test_full.yml`

 * *Files 10% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.6', '3.7', '3.8', '3.9']
-        django-version: ['<2.1', '<2.2', '<3.0', '<3.1', '<3.2', '<3.3']
+        python-version: ['3.8', '3.9', '3.10', '3.11']
+        django-version: ['<3.0', '<3.1', '<3.2', '<3.3', '<4.1', '<4.2']
 
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python
         uses: actions/setup-python@v1
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `ninja-schema-0.13.0/LICENSE` & `ninja_schema-0.13.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ninja-schema-0.13.0/Makefile` & `ninja_schema-0.13.2/Makefile`

 * *Files identical despite different names*

### Comparing `ninja-schema-0.13.0/README.md` & `ninja_schema-0.13.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ![Test](https://github.com/eadwinCode/ninja-schema/workflows/Test/badge.svg)
 [![PyPI version](https://badge.fury.io/py/ninja-schema.svg)](https://badge.fury.io/py/ninja-schema)
 [![PyPI version](https://img.shields.io/pypi/pyversions/ninja-schema.svg)](https://pypi.python.org/pypi/ninja-schema)
 [![PyPI version](https://img.shields.io/pypi/djversions/ninja-schema.svg)](https://pypi.python.org/pypi/ninja-schema)
 [![Codecov](https://img.shields.io/codecov/c/gh/eadwinCode/ninja-schema)](https://codecov.io/gh/eadwinCode/ninja-schema)
-[![Downloads](https://pepy.tech/badge/ninja-schema/month)](https://pepy.tech/project/ninja-schema)
+[![Downloads](https://static.pepy.tech/badge/ninja-schema)](https://pepy.tech/project/ninja-schema)
 
 # Ninja Schema
 Ninja Schema converts your Django ORM models to Pydantic schemas with more Pydantic features supported.
 
 **Inspired by**: [django-ninja](https://django-ninja.rest-framework.com/) and [djantic](https://jordaneremieff.github.io/djantic/)
 
 ### Requirements
-Python >= 3.6
-django >= 2.1
+Python >= 3.8
+django >= 3
 pydantic >= 1.6
 
 **Key features:**
 - **Custom Field Support**: Ninja Schema converts django model to native pydantic types which gives you quick field validation out of the box. eg Enums, email, IPAddress, URLs, JSON, etc
 - **Field Validator**: Fields can be validated with **model_validator** just like pydantic **[validator](https://pydantic-docs.helpmanual.io/usage/validators/)** or **[root_validator](https://pydantic-docs.helpmanual.io/usage/validators/)**. 
   
 ## Installation
```

### Comparing `ninja-schema-0.13.0/ninja_schema/orm/factory.py` & `ninja_schema-0.13.2/ninja_schema/orm/factory.py`

 * *Files identical despite different names*

### Comparing `ninja-schema-0.13.0/ninja_schema/orm/getters.py` & `ninja_schema-0.13.2/ninja_schema/orm/getters.py`

 * *Files identical despite different names*

### Comparing `ninja-schema-0.13.0/ninja_schema/orm/model_schema.py` & `ninja_schema-0.13.2/ninja_schema/orm/model_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,22 +212,24 @@
         super(ModelSchemaConfig, self).__init__()
         self.model = getattr(options, "model", None)
         _include = getattr(options, "include", None) or ALL_FIELDS
         self.include = set() if _include == ALL_FIELDS else set(_include or ())
         self.exclude = set(getattr(options, "exclude", None) or ())
         self.skip_registry = getattr(options, "skip_registry", False)
         self.registry = getattr(options, "registry", global_registry)
+        self.abstract = getattr(options, "ninja_schema_abstract", False)
         _optional = getattr(options, "optional", None)
         self.optional = (
             {ALL_FIELDS} if _optional == ALL_FIELDS else set(_optional or ())
         )
         self.depth = int(getattr(options, "depth", 0))
         self.schema_class_name = schema_class_name
-        self.validate_configuration()
-        self.process_build_schema_parameters()
+        if not self.abstract:
+            self.validate_configuration()
+            self.process_build_schema_parameters()
 
     @classmethod
     def clone_field(cls, field: FieldInfo, **kwargs: Any) -> FieldInfo:
         field_dict = dict(field.__repr_args__())
         field_dict.update(**kwargs)
         new_field = FieldInfo(**field_dict)  # type: ignore
         return new_field
@@ -301,19 +303,26 @@
         bases: tuple,
         namespace: dict,
     ):
         cls = super().__new__(mcs, name, bases, namespace)
         if bases == (SchemaBaseModel,) or not namespace.get("Config"):
             return cls
 
-        if issubclass(cls, ModelSchema):
-            config = namespace["Config"]
+        config = namespace.get("Config")
+        config_instance = None
+
+        if config:
             config_instance = ModelSchemaConfig(name, config)
-            annotations = namespace.get("__annotations__", {})
 
+        if (
+            issubclass(cls, ModelSchema)
+            and config_instance
+            and not config_instance.abstract
+        ):
+            annotations = namespace.get("__annotations__", {})
             try:
                 fields = list(config_instance.model_fields())
             except AttributeError as exc:
                 raise ConfigError(
                     f"{exc} (Is `Config.model` a valid Django model class?)"
                 )
```

### Comparing `ninja-schema-0.13.0/ninja_schema/orm/model_validators.py` & `ninja_schema-0.13.2/ninja_schema/orm/model_validators.py`

 * *Files identical despite different names*

### Comparing `ninja-schema-0.13.0/ninja_schema/orm/schema_registry.py` & `ninja_schema-0.13.2/ninja_schema/orm/schema_registry.py`

 * *Files identical despite different names*

### Comparing `ninja-schema-0.13.0/ninja_schema/orm/utils/converter.py` & `ninja_schema-0.13.2/ninja_schema/orm/utils/converter.py`

 * *Files identical despite different names*

### Comparing `ninja-schema-0.13.0/ninja_schema/pydanticutils/__init__.py` & `ninja_schema-0.13.2/ninja_schema/pydanticutils/__init__.py`

 * *Files identical despite different names*

### Comparing `ninja-schema-0.13.0/pyproject.toml` & `ninja_schema-0.13.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -18,49 +18,48 @@
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development",
     "Typing :: Typed",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Framework :: Django",
-    "Framework :: Django :: 2.0",
-    "Framework :: Django :: 2.1",
-    "Framework :: Django :: 2.2",
     "Framework :: Django :: 3.0",
     "Framework :: Django :: 3.1",
     "Framework :: Django :: 3.2",
+    "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
     "Framework :: AsyncIO",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 
 requires = [
     "Django >=2.0",
     "pydantic",
     "pydantic[email]"
 ]
 description-file = "README.md"
-requires-python = ">=3.6"
+requires-python = ">=3.8"
 
 
 [tool.flit.metadata.urls]
 Documentation = "https://github.com/eadwinCode/ninja-schema"
 
 [tool.flit.metadata.requires-extra]
 test = [
     "pytest",
     "pytest-cov",
     "pytest-django",
     "pytest-asyncio",
-    "black",
-    "isort",
-    "flake8",
-    "mypy",
+    "mypy ==0.971",
+    "flake8 >=3.8.3,<4.0.0",
+    "black ==22.12.0",
+    "isort >=5.0.6,<6.0.0",
     "django-stubs",
 ]
 doc = []
```

### Comparing `ninja-schema-0.13.0/tests/conftest.py` & `ninja_schema-0.13.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ninja-schema-0.13.0/tests/models.py` & `ninja_schema-0.13.2/tests/models.py`

 * *Files identical despite different names*

### Comparing `ninja-schema-0.13.0/tests/test_converters.py` & `ninja_schema-0.13.2/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `ninja-schema-0.13.0/tests/test_custom_fields.py` & `ninja_schema-0.13.2/tests/test_custom_fields.py`

 * *Files identical despite different names*

### Comparing `ninja-schema-0.13.0/tests/test_model_schema.py` & `ninja_schema-0.13.2/tests/test_model_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -341,7 +341,22 @@
         json_event = EventSchema.from_orm(event)
 
         assert json_event.dict() == {"id": 1, "title": "PyConf", "category": None}
         json_event.title = "PyConf Updated"
 
         json_event.apply_to_model(event)
         assert event.title == "PyConf Updated"
+
+    def test_abstract_model_schema_does_not_raise_exception_for_incomplete_configuration(
+        self,
+    ):
+        with pytest.raises(
+            Exception, match="Invalid Configuration. 'model' is required"
+        ):
+
+            class AbstractModel(ModelSchema):
+                class Config:
+                    orm_mode = True
+
+        class AbstractBaseModelSchema(ModelSchema):
+            class Config:
+                ninja_schema_abstract = True
```

### Comparing `ninja-schema-0.13.0/tests/test_schema.py` & `ninja_schema-0.13.2/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `ninja-schema-0.13.0/PKG-INFO` & `ninja_schema-0.13.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,75 +1,74 @@
 Metadata-Version: 2.1
 Name: ninja-schema
-Version: 0.13.0
+Version: 0.13.2
 Summary: Django Schema - Builds Pydantic Schemas from Django Models with default field type validations
 Home-page: https://github.com/eadwinCode/ninja-schema
 Author: Ezeudoh Tochukwu
 Author-email: tochukwu.ezeudoh@gmail.com
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.0
-Classifier: Framework :: Django :: 2.1
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: AsyncIO
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Dist: Django >=2.0
 Requires-Dist: pydantic
 Requires-Dist: pydantic[email]
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-django ; extra == "test"
 Requires-Dist: pytest-asyncio ; extra == "test"
-Requires-Dist: black ; extra == "test"
-Requires-Dist: isort ; extra == "test"
-Requires-Dist: flake8 ; extra == "test"
-Requires-Dist: mypy ; extra == "test"
+Requires-Dist: mypy ==0.971 ; extra == "test"
+Requires-Dist: flake8 >=3.8.3,<4.0.0 ; extra == "test"
+Requires-Dist: black ==22.12.0 ; extra == "test"
+Requires-Dist: isort >=5.0.6,<6.0.0 ; extra == "test"
 Requires-Dist: django-stubs ; extra == "test"
 Project-URL: Documentation, https://github.com/eadwinCode/ninja-schema
 Provides-Extra: doc
 Provides-Extra: test
 
 ![Test](https://github.com/eadwinCode/ninja-schema/workflows/Test/badge.svg)
 [![PyPI version](https://badge.fury.io/py/ninja-schema.svg)](https://badge.fury.io/py/ninja-schema)
 [![PyPI version](https://img.shields.io/pypi/pyversions/ninja-schema.svg)](https://pypi.python.org/pypi/ninja-schema)
 [![PyPI version](https://img.shields.io/pypi/djversions/ninja-schema.svg)](https://pypi.python.org/pypi/ninja-schema)
 [![Codecov](https://img.shields.io/codecov/c/gh/eadwinCode/ninja-schema)](https://codecov.io/gh/eadwinCode/ninja-schema)
-[![Downloads](https://pepy.tech/badge/ninja-schema/month)](https://pepy.tech/project/ninja-schema)
+[![Downloads](https://static.pepy.tech/badge/ninja-schema)](https://pepy.tech/project/ninja-schema)
 
 # Ninja Schema
 Ninja Schema converts your Django ORM models to Pydantic schemas with more Pydantic features supported.
 
 **Inspired by**: [django-ninja](https://django-ninja.rest-framework.com/) and [djantic](https://jordaneremieff.github.io/djantic/)
 
 ### Requirements
-Python >= 3.6
-django >= 2.1
+Python >= 3.8
+django >= 3
 pydantic >= 1.6
 
 **Key features:**
 - **Custom Field Support**: Ninja Schema converts django model to native pydantic types which gives you quick field validation out of the box. eg Enums, email, IPAddress, URLs, JSON, etc
 - **Field Validator**: Fields can be validated with **model_validator** just like pydantic **[validator](https://pydantic-docs.helpmanual.io/usage/validators/)** or **[root_validator](https://pydantic-docs.helpmanual.io/usage/validators/)**. 
   
 ## Installation
```

