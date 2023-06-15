# Comparing `tmp/openapi_spec_validator-0.5.7.tar.gz` & `tmp/openapi_spec_validator-0.6.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi_spec_validator-0.5.7.tar", max compression
+gzip compressed data, was "openapi_spec_validator-0.6.0a1.tar", max compression
```

## Comparing `openapi_spec_validator-0.5.7.tar` & `openapi_spec_validator-0.6.0a1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    11357 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/LICENSE
--rw-r--r--   0        0        0     3936 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/README.rst
--rw-r--r--   0        0        0      845 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/openapi_spec_validator/__init__.py
--rw-r--r--   0        0        0     3041 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/openapi_spec_validator/__main__.py
--rw-r--r--   0        0        0       53 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/openapi_spec_validator/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/openapi_spec_validator/py.typed
--rw-r--r--   0        0        0      670 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/openapi_spec_validator/readers.py
--rw-r--r--   0        0        0    40203 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/openapi_spec_validator/resources/schemas/v2.0/schema.json
--rw-r--r--   0        0        0    35816 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/openapi_spec_validator/resources/schemas/v3.0/schema.json
--rw-r--r--   0        0        0    37211 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/openapi_spec_validator/resources/schemas/v3.0.0/schema.json
--rw-r--r--   0        0        0    34260 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/openapi_spec_validator/resources/schemas/v3.1/schema.json
--rw-r--r--   0        0        0      612 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/openapi_spec_validator/schemas/__init__.py
--rw-r--r--   0        0        0      924 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/openapi_spec_validator/schemas/utils.py
--rw-r--r--   0        0        0      756 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/openapi_spec_validator/shortcuts.py
--rw-r--r--   0        0        0     2523 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/openapi_spec_validator/validation/__init__.py
--rw-r--r--   0        0        0      922 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/openapi_spec_validator/validation/decorators.py
--rw-r--r--   0        0        0      529 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/openapi_spec_validator/validation/exceptions.py
--rw-r--r--   0        0        0      796 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/openapi_spec_validator/validation/protocols.py
--rw-r--r--   0        0        0     1537 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/openapi_spec_validator/validation/proxies.py
--rw-r--r--   0        0        0    11732 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/openapi_spec_validator/validation/validators.py
--rw-r--r--   0        0        0     2577 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     1401 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/conftest.py
--rw-r--r--   0        0        0        2 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/empty.yaml
--rw-r--r--   0        0        0       14 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v2.0/empty.yaml
--rw-r--r--   0        0        0     2137 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v2.0/missing-reference.yaml
--rw-r--r--   0        0        0     2145 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v2.0/petstore.yaml
--rw-r--r--   0        0        0       16 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/empty.yaml
--rw-r--r--   0        0        0      267 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/missing-description.yaml
--rw-r--r--   0        0        0      306 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/parent-reference/common.yaml
--rw-r--r--   0        0        0      938 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/parent-reference/openapi.yaml
--rw-r--r--   0        0        0       94 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/parent-reference/recursive.yaml
--rw-r--r--   0        0        0      159 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/parent-reference/recursive2.yaml
--rw-r--r--   0        0        0      198 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/parent-reference/spec/components.yaml
--rw-r--r--   0        0        0      127 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/petstore-separate/common/schemas/Error.yaml
--rw-r--r--   0        0        0     2037 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/petstore-separate/spec/openapi.yaml
--rw-r--r--   0        0        0      128 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/petstore-separate/spec/schemas/Pet.yaml
--rw-r--r--   0        0        0       37 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/petstore-separate/spec/schemas/Pets.yaml
--rw-r--r--   0        0        0     2571 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/petstore.yaml
--rw-r--r--   0        0        0      279 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/property-missing-reference.yaml
--rw-r--r--   0        0        0      295 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/property-recursive.yaml
--rw-r--r--   0        0        0     2718 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.1/petstore.yaml
--rw-r--r--   0        0        0     3576 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/test_main.py
--rw-r--r--   0        0        0     4647 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/test_shortcuts.py
--rw-r--r--   0        0        0    16360 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/validation/test_exceptions.py
--rw-r--r--   0        0        0     5867 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/validation/test_validators.py
--rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 openapi_spec_validator-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/LICENSE
+-rw-r--r--   0        0        0     3936 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/README.rst
+-rw-r--r--   0        0        0      847 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/__init__.py
+-rw-r--r--   0        0        0     3041 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/__main__.py
+-rw-r--r--   0        0        0       53 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/py.typed
+-rw-r--r--   0        0        0      670 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/readers.py
+-rw-r--r--   0        0        0    40203 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/resources/schemas/v2.0/schema.json
+-rw-r--r--   0        0        0    35816 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/resources/schemas/v3.0/schema.json
+-rw-r--r--   0        0        0    37211 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/resources/schemas/v3.0.0/schema.json
+-rw-r--r--   0        0        0    34260 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/resources/schemas/v3.1/schema.json
+-rw-r--r--   0        0        0      612 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/schemas/__init__.py
+-rw-r--r--   0        0        0      924 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/schemas/utils.py
+-rw-r--r--   0        0        0      756 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/shortcuts.py
+-rw-r--r--   0        0        0     2523 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/validation/__init__.py
+-rw-r--r--   0        0        0      922 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/validation/decorators.py
+-rw-r--r--   0        0        0      529 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/validation/exceptions.py
+-rw-r--r--   0        0        0      644 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/validation/protocols.py
+-rw-r--r--   0        0        0     1537 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/validation/proxies.py
+-rw-r--r--   0        0        0    11887 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/validation/validators.py
+-rw-r--r--   0        0        0     2533 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/pyproject.toml
+-rw-r--r--   0        0        0     1401 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/tests/integration/conftest.py
+-rw-r--r--   0        0        0        2 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/tests/integration/data/empty.yaml
+-rw-r--r--   0        0        0       14 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/tests/integration/data/v2.0/empty.yaml
+-rw-r--r--   0        0        0     2137 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/tests/integration/data/v2.0/missing-reference.yaml
+-rw-r--r--   0        0        0     2145 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/tests/integration/data/v2.0/petstore.yaml
+-rw-r--r--   0        0        0       16 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/empty.yaml
+-rw-r--r--   0        0        0      267 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/missing-description.yaml
+-rw-r--r--   0        0        0      306 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/parent-reference/common.yaml
+-rw-r--r--   0        0        0      938 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/parent-reference/openapi.yaml
+-rw-r--r--   0        0        0       94 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/parent-reference/recursive.yaml
+-rw-r--r--   0        0        0      159 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/parent-reference/recursive2.yaml
+-rw-r--r--   0        0        0      198 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/parent-reference/spec/components.yaml
+-rw-r--r--   0        0        0      127 2023-06-15 11:39:35.584022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/petstore-separate/common/schemas/Error.yaml
+-rw-r--r--   0        0        0     2037 2023-06-15 11:39:35.584022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/petstore-separate/spec/openapi.yaml
+-rw-r--r--   0        0        0      128 2023-06-15 11:39:35.584022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/petstore-separate/spec/schemas/Pet.yaml
+-rw-r--r--   0        0        0       37 2023-06-15 11:39:35.584022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/petstore-separate/spec/schemas/Pets.yaml
+-rw-r--r--   0        0        0     2571 2023-06-15 11:39:35.584022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/petstore.yaml
+-rw-r--r--   0        0        0      279 2023-06-15 11:39:35.584022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/property-missing-reference.yaml
+-rw-r--r--   0        0        0      295 2023-06-15 11:39:35.584022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/property-recursive.yaml
+-rw-r--r--   0        0        0     2718 2023-06-15 11:39:35.584022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.1/petstore.yaml
+-rw-r--r--   0        0        0     3576 2023-06-15 11:39:35.584022 openapi_spec_validator-0.6.0a1/tests/integration/test_main.py
+-rw-r--r--   0        0        0     4643 2023-06-15 11:39:35.584022 openapi_spec_validator-0.6.0a1/tests/integration/test_shortcuts.py
+-rw-r--r--   0        0        0    16360 2023-06-15 11:39:35.584022 openapi_spec_validator-0.6.0a1/tests/integration/validation/test_exceptions.py
+-rw-r--r--   0        0        0     5846 2023-06-15 11:39:35.584022 openapi_spec_validator-0.6.0a1/tests/integration/validation/test_validators.py
+-rw-r--r--   0        0        0     5276 1970-01-01 00:00:00.000000 openapi_spec_validator-0.6.0a1/PKG-INFO
```

### Comparing `openapi_spec_validator-0.5.7/LICENSE` & `openapi_spec_validator-0.6.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.7/README.rst` & `openapi_spec_validator-0.6.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.7/openapi_spec_validator/__init__.py` & `openapi_spec_validator-0.6.0a1/openapi_spec_validator/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from openapi_spec_validator.validation import openapi_v2_spec_validator
 from openapi_spec_validator.validation import openapi_v3_spec_validator
 from openapi_spec_validator.validation import openapi_v30_spec_validator
 from openapi_spec_validator.validation import openapi_v31_spec_validator
 
 __author__ = "Artur Maciag"
 __email__ = "maciag.artur@gmail.com"
-__version__ = "0.5.7"
+__version__ = "0.6.0a1"
 __url__ = "https://github.com/python-openapi/openapi-spec-validator"
 __license__ = "Apache License, Version 2.0"
 
 __all__ = [
     "openapi_v2_spec_validator",
     "openapi_v3_spec_validator",
     "openapi_v30_spec_validator",
```

### Comparing `openapi_spec_validator-0.5.7/openapi_spec_validator/__main__.py` & `openapi_spec_validator-0.6.0a1/openapi_spec_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.7/openapi_spec_validator/readers.py` & `openapi_spec_validator-0.6.0a1/openapi_spec_validator/readers.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.7/openapi_spec_validator/resources/schemas/v2.0/schema.json` & `openapi_spec_validator-0.6.0a1/openapi_spec_validator/resources/schemas/v2.0/schema.json`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.7/openapi_spec_validator/resources/schemas/v3.0/schema.json` & `openapi_spec_validator-0.6.0a1/openapi_spec_validator/resources/schemas/v3.0/schema.json`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.7/openapi_spec_validator/resources/schemas/v3.0.0/schema.json` & `openapi_spec_validator-0.6.0a1/openapi_spec_validator/resources/schemas/v3.0.0/schema.json`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.7/openapi_spec_validator/resources/schemas/v3.1/schema.json` & `openapi_spec_validator-0.6.0a1/openapi_spec_validator/resources/schemas/v3.1/schema.json`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.7/openapi_spec_validator/schemas/__init__.py` & `openapi_spec_validator-0.6.0a1/openapi_spec_validator/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.7/openapi_spec_validator/schemas/utils.py` & `openapi_spec_validator-0.6.0a1/openapi_spec_validator/schemas/utils.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.7/openapi_spec_validator/shortcuts.py` & `openapi_spec_validator-0.6.0a1/openapi_spec_validator/shortcuts.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.7/openapi_spec_validator/validation/__init__.py` & `openapi_spec_validator-0.6.0a1/openapi_spec_validator/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.7/openapi_spec_validator/validation/decorators.py` & `openapi_spec_validator-0.6.0a1/openapi_spec_validator/validation/decorators.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.7/openapi_spec_validator/validation/exceptions.py` & `openapi_spec_validator-0.6.0a1/openapi_spec_validator/validation/exceptions.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.7/openapi_spec_validator/validation/protocols.py` & `openapi_spec_validator-0.6.0a1/openapi_spec_validator/validation/protocols.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,13 @@
-import sys
 from typing import Any
 from typing import Hashable
 from typing import Iterator
 from typing import Mapping
-
-if sys.version_info >= (3, 8):
-    from typing import Protocol
-    from typing import runtime_checkable
-else:
-    from typing_extensions import Protocol
-    from typing_extensions import runtime_checkable
+from typing import Protocol
+from typing import runtime_checkable
 
 from openapi_spec_validator.validation.exceptions import OpenAPIValidationError
 
 
 @runtime_checkable
 class SupportsValidation(Protocol):
     def is_valid(self, instance: Mapping[Hashable, Any]) -> bool:
```

### Comparing `openapi_spec_validator-0.5.7/openapi_spec_validator/validation/proxies.py` & `openapi_spec_validator-0.6.0a1/openapi_spec_validator/validation/proxies.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.7/openapi_spec_validator/validation/validators.py` & `openapi_spec_validator-0.6.0a1/openapi_spec_validator/validation/validators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """OpenAPI spec validator validation validators module."""
 import logging
 import string
+import warnings
 from typing import Any
-from typing import Callable
-from typing import Hashable
 from typing import Iterator
 from typing import List
-from typing import Mapping
 from typing import Optional
 from typing import Type
 
 from jsonschema._format import FormatChecker
 from jsonschema.exceptions import ValidationError
 from jsonschema.protocols import Validator
-from jsonschema.validators import RefResolver
-from jsonschema_spec.accessors import SpecAccessor
-from jsonschema_spec.paths import Spec
+from jsonschema_spec.handlers import default_handlers
+from jsonschema_spec.paths import SchemaPath
+from jsonschema_spec.typing import ResolverHandlers
+from jsonschema_spec.typing import Schema
 
 from openapi_spec_validator.validation.decorators import ValidationErrorWrapper
 from openapi_spec_validator.validation.exceptions import (
     DuplicateOperationIDError,
 )
 from openapi_spec_validator.validation.exceptions import ExtraParametersError
 from openapi_spec_validator.validation.exceptions import OpenAPIValidationError
@@ -31,20 +30,15 @@
 )
 
 log = logging.getLogger(__name__)
 
 wraps_errors = ValidationErrorWrapper(OpenAPIValidationError)
 
 
-def is_ref(spec: Any) -> bool:
-    return isinstance(spec, dict) and "$ref" in spec
-
-
 class SpecValidator:
-
     OPERATIONS = [
         "get",
         "put",
         "post",
         "delete",
         "options",
         "head",
@@ -53,66 +47,81 @@
     ]
 
     def __init__(
         self,
         schema_validator: Validator,
         value_validator_class: Type[Validator],
         value_validator_format_checker: FormatChecker,
-        resolver_handlers: Optional[Mapping[str, Callable[[str], Any]]] = None,
+        resolver_handlers: ResolverHandlers = default_handlers,
     ):
         self.schema_validator = schema_validator
         self.value_validator_class = value_validator_class
         self.value_validator_format_checker = value_validator_format_checker
         self.resolver_handlers = resolver_handlers
 
         self.operation_ids_registry: Optional[List[str]] = None
         self.schema_ids_registry: Optional[List[int]] = None
-        self.resolver = None
 
     def validate(
-        self, instance: Mapping[Hashable, Any], spec_url: str = ""
+        self,
+        schema: Schema,
+        base_uri: str = "",
+        spec_url: Optional[str] = None,
     ) -> None:
-        for err in self.iter_errors(instance, spec_url=spec_url):
+        for err in self.iter_errors(
+            schema,
+            base_uri=base_uri,
+            spec_url=spec_url,
+        ):
             raise err
 
-    def is_valid(self, instance: Mapping[Hashable, Any]) -> bool:
-        error = next(self.iter_errors(instance), None)
+    def is_valid(self, schema: Schema) -> bool:
+        error = next(self.iter_errors(schema), None)
         return error is None
 
     @wraps_errors
     def iter_errors(
-        self, instance: Mapping[Hashable, Any], spec_url: str = ""
-    ) -> Iterator[ValidationError]:
+        self,
+        schema: Schema,
+        base_uri: str = "",
+        spec_url: Optional[str] = None,
+    ) -> Iterator[ValidationError]:
+        if spec_url is not None:
+            warnings.warn(
+                "spec_url parameter is deprecated. " "Use base_uri instead.",
+                DeprecationWarning,
+            )
+            base_uri = spec_url
+
         self.operation_ids_registry = []
         self.schema_ids_registry = []
-        self.resolver = self._get_resolver(spec_url, instance)
 
-        yield from self.schema_validator.iter_errors(instance)
+        yield from self.schema_validator.iter_errors(schema)
 
-        accessor = SpecAccessor(instance, self.resolver)
-        spec = Spec(accessor)
+        spec = SchemaPath.from_dict(
+            schema,
+            base_uri=base_uri,
+            handlers=self.resolver_handlers,
+        )
         if "paths" in spec:
             paths = spec / "paths"
             yield from self._iter_paths_errors(paths)
 
         if "components" in spec:
             components = spec / "components"
             yield from self._iter_components_errors(components)
 
-    def _get_resolver(
-        self, base_uri: str, referrer: Mapping[Hashable, Any]
-    ) -> RefResolver:
-        return RefResolver(base_uri, referrer, handlers=self.resolver_handlers)
-
-    def _iter_paths_errors(self, paths: Spec) -> Iterator[ValidationError]:
+    def _iter_paths_errors(
+        self, paths: SchemaPath
+    ) -> Iterator[ValidationError]:
         for url, path_item in paths.items():
             yield from self._iter_path_errors(url, path_item)
 
     def _iter_path_errors(
-        self, url: str, path_item: Spec
+        self, url: str, path_item: SchemaPath
     ) -> Iterator[ValidationError]:
         parameters = None
         if "parameters" in path_item:
             parameters = path_item / "parameters"
             yield from self._iter_parameters_errors(parameters)
 
         for field_name, operation in path_item.items():
@@ -123,16 +132,16 @@
                 url, field_name, operation, parameters
             )
 
     def _iter_operation_errors(
         self,
         url: str,
         name: str,
-        operation: Spec,
-        path_parameters: Optional[Spec],
+        operation: SchemaPath,
+        path_parameters: Optional[SchemaPath],
     ) -> Iterator[ValidationError]:
         assert self.operation_ids_registry is not None
 
         operation_id = operation.getkey("operationId")
         if (
             operation_id is not None
             and operation_id in self.operation_ids_registry
@@ -164,92 +173,94 @@
                 yield UnresolvableParameterError(
                     "Path parameter '{}' for '{}' operation in '{}' "
                     "was not resolved".format(path, name, url)
                 )
         return
 
     def _iter_responses_errors(
-        self, responses: Spec
+        self, responses: SchemaPath
     ) -> Iterator[ValidationError]:
         for response_code, response in responses.items():
             yield from self._iter_response_errors(response_code, response)
 
     def _iter_response_errors(
-        self, response_code: str, response: Spec
+        self, response_code: str, response: SchemaPath
     ) -> Iterator[ValidationError]:
         # openapi 2
         if "schema" in response:
             schema = response / "schema"
             yield from self._iter_schema_errors(schema)
         # openapi 3
         if "content" in response:
             content = response / "content"
             yield from self._iter_content_errors(content)
 
-    def _iter_content_errors(self, content: Spec) -> Iterator[ValidationError]:
+    def _iter_content_errors(
+        self, content: SchemaPath
+    ) -> Iterator[ValidationError]:
         for mimetype, media_type in content.items():
             yield from self._iter_media_type_errors(mimetype, media_type)
 
     def _iter_media_type_errors(
-        self, mimetype: str, media_type: Spec
+        self, mimetype: str, media_type: SchemaPath
     ) -> Iterator[ValidationError]:
         if "schema" in media_type:
             schema = media_type / "schema"
             yield from self._iter_schema_errors(schema)
 
-    def _get_path_param_names(self, params: Spec) -> Iterator[str]:
+    def _get_path_param_names(self, params: SchemaPath) -> Iterator[str]:
         for param in params:
             if param["in"] == "path":
                 yield param["name"]
 
     def _get_path_params_from_url(self, url: str) -> Iterator[str]:
         formatter = string.Formatter()
         path_params = [item[1] for item in formatter.parse(url)]
         return filter(None, path_params)
 
     def _iter_parameters_errors(
-        self, parameters: Spec
+        self, parameters: SchemaPath
     ) -> Iterator[ValidationError]:
         seen = set()
         for parameter in parameters:
             yield from self._iter_parameter_errors(parameter)
 
             key = (parameter["name"], parameter["in"])
             if key in seen:
                 yield ParameterDuplicateError(
                     f"Duplicate parameter `{parameter['name']}`"
                 )
             seen.add(key)
 
     def _iter_parameter_errors(
-        self, parameter: Spec
+        self, parameter: SchemaPath
     ) -> Iterator[ValidationError]:
         if "schema" in parameter:
             schema = parameter / "schema"
             yield from self._iter_schema_errors(schema)
 
         if "default" in parameter:
             # only possible in swagger 2.0
             default = parameter.getkey("default")
             if default is not None:
                 yield from self._iter_value_errors(parameter, default)
 
     def _iter_value_errors(
-        self, schema: Spec, value: Any
+        self, schema: SchemaPath, value: Any
     ) -> Iterator[ValidationError]:
-        with schema.open() as content:
+        with schema.resolve() as resolved:
             validator = self.value_validator_class(
-                content,
-                resolver=self.resolver,
+                resolved.contents,
+                _resolver=resolved.resolver,
                 format_checker=self.value_validator_format_checker,
             )
             yield from validator.iter_errors(value)
 
     def _iter_schema_errors(
-        self, schema: Spec, require_properties: bool = True
+        self, schema: SchemaPath, require_properties: bool = True
     ) -> Iterator[ValidationError]:
         if not hasattr(schema.content(), "__getitem__"):
             return
 
         assert self.schema_ids_registry is not None
         schema_id = id(schema.content())
         if schema_id in self.schema_ids_registry:
@@ -325,15 +336,17 @@
         if "default" in schema:
             default = schema["default"]
             nullable = schema.get("nullable", False)
             if default is not None or nullable is not True:
                 yield from self._iter_value_errors(schema, default)
 
     def _iter_components_errors(
-        self, components: Spec
+        self, components: SchemaPath
     ) -> Iterator[ValidationError]:
         schemas = components.get("schemas", {})
         yield from self._iter_schemas_errors(schemas)
 
-    def _iter_schemas_errors(self, schemas: Spec) -> Iterator[ValidationError]:
+    def _iter_schemas_errors(
+        self, schemas: SchemaPath
+    ) -> Iterator[ValidationError]:
         for _, schema in schemas.items():
             yield from self._iter_schema_errors(schema)
```

### Comparing `openapi_spec_validator-0.5.7/pyproject.toml` & `openapi_spec_validator-0.6.0a1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -14,68 +14,68 @@
 strict = true
 
 [[tool.mypy.overrides]]
 module = "jsonschema.*"
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
+module = "jsonschema_specifications"
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
 module = "lazy_object_proxy.*"
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "openapi-spec-validator"
-version = "0.5.7"
+version = "0.6.0a1"
 description = "OpenAPI 2.0 (aka Swagger) and OpenAPI 3 spec validator"
 authors = ["Artur Maciag <maciag.artur@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.rst"
 repository = "https://github.com/python-openapi/openapi-spec-validator"
 keywords = ["openapi", "swagger", "schema"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries"
 ]
 include = [
     {path = "tests", format = "sdist"},
 ]
 
 [tool.poetry.dependencies]
-jsonschema = ">=4.0.0,<4.18.0"
-openapi-schema-validator = "^0.4.2"
-python = "^3.7.0"
+jsonschema = {version = "^4.18.0a1", allow-prereleases = true}
+openapi-schema-validator = {version = "^0.6.0a1", allow-prereleases = true}
+python = "^3.8.0"
 importlib-resources = {version = "^5.8.0", python = "<3.9" }
-typing-extensions = {version = "^4.5.0", python = "<3.8" }
-jsonschema-spec = "^0.1.1"
+jsonschema-spec = "^0.2.2"
 lazy-object-proxy = "^1.7.1"
 
 [tool.poetry.extras]
-dev = ["pre-commit"]
 docs = ["sphinx", "sphinx-immaterial"]
-requests = ["requests"]
 
 [tool.poetry.dev-dependencies]
-pre-commit =  {version = "*", optional = true}
-pytest = "^6.2.5"
+pre-commit =  "*"
+pytest = "^7.3.2"
 pytest-flake8 = "=1.1.0"
 pytest-cov = "^4.1.0"
 tox = "*"
 mypy = "^1.3"
 isort = "^5.11.5"
 black = "^23.3.0"
 flynt = "^0.78"
-deptry = { version = "^0.11.0", python = ">=3.8" }
+deptry = "^0.11.0"
 
 [tool.poetry.scripts]
 openapi-spec-validator = "openapi_spec_validator.__main__:main"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^5.3.0"
 sphinx-immaterial = "^0.11.0"
```

### Comparing `openapi_spec_validator-0.5.7/tests/integration/conftest.py` & `openapi_spec_validator-0.6.0a1/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.7/tests/integration/data/v2.0/missing-reference.yaml` & `openapi_spec_validator-0.6.0a1/tests/integration/data/v2.0/missing-reference.yaml`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.7/tests/integration/data/v2.0/petstore.yaml` & `openapi_spec_validator-0.6.0a1/tests/integration/data/v2.0/petstore.yaml`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.7/tests/integration/data/v3.0/parent-reference/openapi.yaml` & `openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/parent-reference/openapi.yaml`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.7/tests/integration/data/v3.0/petstore-separate/spec/openapi.yaml` & `openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/petstore-separate/spec/openapi.yaml`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.7/tests/integration/data/v3.0/petstore.yaml` & `openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/petstore.yaml`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.7/tests/integration/data/v3.1/petstore.yaml` & `openapi_spec_validator-0.6.0a1/tests/integration/data/v3.1/petstore.yaml`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.7/tests/integration/test_main.py` & `openapi_spec_validator-0.6.0a1/tests/integration/test_main.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.7/tests/integration/test_shortcuts.py` & `openapi_spec_validator-0.6.0a1/tests/integration/test_shortcuts.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
         spec_url = factory.spec_file_url(spec_path)
 
         with pytest.raises(ValidatorDetectError):
             validate_spec_url(spec_url)
 
 
 class TestLiocalValidatev2Spec:
-
     LOCAL_SOURCE_DIRECTORY = "data/v2.0/"
 
     def local_test_suite_file_path(self, test_file):
         return f"{self.LOCAL_SOURCE_DIRECTORY}{test_file}"
 
     @pytest.mark.parametrize(
         "spec_file",
@@ -57,15 +56,14 @@
         spec = factory.spec_from_file(spec_path)
 
         with pytest.raises(OpenAPIValidationError):
             validate_spec(spec, validator=openapi_v2_spec_validator)
 
 
 class TestLocalValidatev30Spec:
-
     LOCAL_SOURCE_DIRECTORY = "data/v3.0/"
 
     def local_test_suite_file_path(self, test_file):
         return f"{self.LOCAL_SOURCE_DIRECTORY}{test_file}"
 
     @pytest.mark.parametrize(
         "spec_file",
@@ -94,15 +92,14 @@
 
         with pytest.raises(OpenAPIValidationError):
             validate_spec(spec, validator=openapi_v30_spec_validator)
 
 
 @pytest.mark.network
 class TestRemoteValidatev2SpecUrl:
-
     REMOTE_SOURCE_URL = (
         "https://raw.githubusercontent.com/OAI/OpenAPI-Specification/"
     )
 
     def remote_test_suite_file_path(self, test_file):
         return f"{self.REMOTE_SOURCE_URL}{test_file}"
 
@@ -122,15 +119,14 @@
 
         validate_spec_url(spec_url)
         validate_spec_url(spec_url, validator=openapi_v2_spec_validator)
 
 
 @pytest.mark.network
 class TestRemoteValidatev30SpecUrl:
-
     REMOTE_SOURCE_URL = (
         "https://raw.githubusercontent.com/OAI/OpenAPI-Specification/"
     )
 
     def remote_test_suite_file_path(self, test_file):
         return f"{self.REMOTE_SOURCE_URL}{test_file}"
```

### Comparing `openapi_spec_validator-0.5.7/tests/integration/validation/test_exceptions.py` & `openapi_spec_validator-0.6.0a1/tests/integration/validation/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.7/tests/integration/validation/test_validators.py` & `openapi_spec_validator-0.6.0a1/tests/integration/validation/test_validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import pytest
-from jsonschema.exceptions import RefResolutionError
+from referencing.exceptions import Unresolvable
 
 from openapi_spec_validator.validation.exceptions import OpenAPIValidationError
 
 
 class TestLocalOpenAPIv2Validator:
-
     LOCAL_SOURCE_DIRECTORY = "data/v2.0/"
 
     def local_test_suite_file_path(self, test_file):
         return f"{self.LOCAL_SOURCE_DIRECTORY}{test_file}"
 
     @pytest.mark.parametrize(
         "spec_file",
@@ -45,20 +44,19 @@
         ],
     )
     def test_ref_failed(self, factory, validator_v2, spec_file):
         spec_path = self.local_test_suite_file_path(spec_file)
         spec = factory.spec_from_file(spec_path)
         spec_url = factory.spec_file_url(spec_path)
 
-        with pytest.raises(RefResolutionError):
+        with pytest.raises(Unresolvable):
             validator_v2.validate(spec, spec_url=spec_url)
 
 
 class TestLocalOpenAPIv30Validator:
-
     LOCAL_SOURCE_DIRECTORY = "data/v3.0/"
 
     def local_test_suite_file_path(self, test_file):
         return f"{self.LOCAL_SOURCE_DIRECTORY}{test_file}"
 
     @pytest.mark.parametrize(
         "spec_file",
@@ -97,21 +95,20 @@
         ],
     )
     def test_ref_failed(self, factory, validator_v30, spec_file):
         spec_path = self.local_test_suite_file_path(spec_file)
         spec = factory.spec_from_file(spec_path)
         spec_url = factory.spec_file_url(spec_path)
 
-        with pytest.raises(RefResolutionError):
+        with pytest.raises(Unresolvable):
             validator_v30.validate(spec, spec_url=spec_url)
 
 
 @pytest.mark.network
 class TestRemoteOpenAPIv30Validator:
-
     REMOTE_SOURCE_URL = (
         "https://raw.githubusercontent.com/OAI/OpenAPI-Specification/"
     )
 
     def remote_test_suite_file_path(self, test_file):
         return f"{self.REMOTE_SOURCE_URL}{test_file}"
 
@@ -131,15 +128,14 @@
         spec = factory.spec_from_url(spec_url)
 
         return validator_v30.validate(spec, spec_url=spec_url)
 
 
 @pytest.mark.network
 class TestRemoteOpenAPIv31Validator:
-
     REMOTE_SOURCE_URL = (
         "https://raw.githubusercontent.com/"
         "OAI/OpenAPI-Specification/"
         "d9ac75b00c8bf405c2c90cfa9f20370564371dec/"
     )
 
     def remote_test_suite_file_path(self, test_file):
```

### Comparing `openapi_spec_validator-0.5.7/PKG-INFO` & `openapi_spec_validator-0.6.0a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 Metadata-Version: 2.1
 Name: openapi-spec-validator
-Version: 0.5.7
+Version: 0.6.0a1
 Summary: OpenAPI 2.0 (aka Swagger) and OpenAPI 3 spec validator
 Home-page: https://github.com/python-openapi/openapi-spec-validator
 License: Apache-2.0
 Keywords: openapi,swagger,schema
 Author: Artur Maciag
 Author-email: maciag.artur@gmail.com
-Requires-Python: >=3.7.0,<4.0.0
+Requires-Python: >=3.8.0,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Provides-Extra: dev
 Provides-Extra: docs
-Provides-Extra: requests
 Requires-Dist: importlib-resources (>=5.8.0,<6.0.0) ; python_version < "3.9"
-Requires-Dist: jsonschema (>=4.0.0,<4.18.0)
-Requires-Dist: jsonschema-spec (>=0.1.1,<0.2.0)
+Requires-Dist: jsonschema (>=4.18.0a1,<5.0.0)
+Requires-Dist: jsonschema-spec (>=0.2.2,<0.3.0)
 Requires-Dist: lazy-object-proxy (>=1.7.1,<2.0.0)
-Requires-Dist: openapi-schema-validator (>=0.4.2,<0.5.0)
-Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) ; python_version < "3.8"
+Requires-Dist: openapi-schema-validator (>=0.6.0a1,<0.7.0)
 Project-URL: Repository, https://github.com/python-openapi/openapi-spec-validator
 Description-Content-Type: text/x-rst
 
 **********************
 OpenAPI Spec validator
 **********************
```

