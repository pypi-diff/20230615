# Comparing `tmp/kadaster_kikinzage_client-0.1.2.tar.gz` & `tmp/kadaster_kikinzage_client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kadaster_kikinzage_client-0.1.2.tar", max compression
+gzip compressed data, was "kadaster_kikinzage_client-0.1.3.tar", max compression
```

## Comparing `kadaster_kikinzage_client-0.1.2.tar` & `kadaster_kikinzage_client-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,23 @@
--rw-r--r--   0        0        0     1071 2023-06-14 09:39:27.090443 kadaster_kikinzage_client-0.1.2/LICENSE
--rw-r--r--   0        0        0     4027 2023-06-14 09:39:27.094443 kadaster_kikinzage_client-0.1.2/README.md
--rw-r--r--   0        0        0     2084 2023-06-14 09:39:45.890788 kadaster_kikinzage_client-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       45 2023-06-14 09:39:27.098443 kadaster_kikinzage_client-0.1.2/src/kikinzage/__init__.py
--rw-r--r--   0        0        0     2274 2023-06-14 09:39:27.098443 kadaster_kikinzage_client-0.1.2/src/kikinzage/__main__.py
--rw-r--r--   0        0        0      302 2023-06-14 09:39:27.098443 kadaster_kikinzage_client-0.1.2/src/kikinzage/client/__init__.py
--rw-r--r--   0        0        0     3442 2023-06-14 09:39:27.102443 kadaster_kikinzage_client-0.1.2/src/kikinzage/client/asyncio.py
--rw-r--r--   0        0        0     9087 2023-06-14 09:39:27.102443 kadaster_kikinzage_client-0.1.2/src/kikinzage/client/base.py
--rw-r--r--   0        0        0     6428 2023-06-14 09:39:27.102443 kadaster_kikinzage_client-0.1.2/src/kikinzage/client/default.py
--rw-r--r--   0        0        0      610 2023-06-14 09:39:27.102443 kadaster_kikinzage_client-0.1.2/src/kikinzage/client/errors.py
--rw-r--r--   0        0        0      182 2023-06-14 09:39:27.102443 kadaster_kikinzage_client-0.1.2/src/kikinzage/client/utils.py
--rw-r--r--   0        0        0      145 2023-06-14 09:39:27.102443 kadaster_kikinzage_client-0.1.2/src/kikinzage/models/__init__.py
--rw-r--r--   0        0        0    37698 2023-06-14 09:39:27.102443 kadaster_kikinzage_client-0.1.2/src/kikinzage/models/generated.py
--rw-r--r--   0        0        0        0 2023-06-14 09:39:27.102443 kadaster_kikinzage_client-0.1.2/src/kikinzage/py.typed
--rw-r--r--   0        0        0     5033 1970-01-01 00:00:00.000000 kadaster_kikinzage_client-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4027 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/README.md
+-rw-r--r--   0        0        0     2113 2023-06-15 15:43:00.989328 kadaster_kikinzage_client-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/__init__.py
+-rw-r--r--   0        0        0     2274 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/__main__.py
+-rw-r--r--   0        0        0      302 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/client/__init__.py
+-rw-r--r--   0        0        0     2379 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/client/asyncio.py
+-rw-r--r--   0        0        0     9405 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/client/base.py
+-rw-r--r--   0        0        0     5365 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/client/default.py
+-rw-r--r--   0        0        0      610 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/client/errors.py
+-rw-r--r--   0        0        0      182 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/client/utils.py
+-rw-r--r--   0        0        0      372 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/models/__init__.py
+-rw-r--r--   0        0        0    10276 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/models/collectie.py
+-rw-r--r--   0        0        0     5786 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/models/eigendomsinformatie.py
+-rw-r--r--   0        0        0     1400 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/models/enum.py
+-rw-r--r--   0        0        0    16298 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/models/generated.py
+-rw-r--r--   0        0        0      629 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/models/misc.py
+-rw-r--r--   0        0        0     3500 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/models/persoon.py
+-rw-r--r--   0        0        0     1129 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/models/product.py
+-rw-r--r--   0        0        0     1941 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/models/stukken.py
+-rw-r--r--   0        0        0     1243 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/models/zekerheid.py
+-rw-r--r--   0        0        0        0 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/py.typed
+-rw-r--r--   0        0        0     5083 1970-01-01 00:00:00.000000 kadaster_kikinzage_client-0.1.3/PKG-INFO
```

### Comparing `kadaster_kikinzage_client-0.1.2/LICENSE` & `kadaster_kikinzage_client-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.2/README.md` & `kadaster_kikinzage_client-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.2/pyproject.toml` & `kadaster_kikinzage_client-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kadaster-kikinzage-client"
-version = "0.1.2"
+version = "0.1.3"
 description = " Kadaster - KIK Inzage API Python client"
 authors = ["Jelmer Draaijer <info@jelmert.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/foarsitter/kadaster-kik-inzage-api-python-client"
 repository = "https://github.com/foarsitter/kadaster-kik-inzage-api-python-client"
 documentation = "https://kadaster-kik-inzage-api-python-client.readthedocs.io"
@@ -19,14 +19,15 @@
 Changelog = "https://github.com/foarsitter/kadaster-kik-inzage-api-python-client/releases"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1"
 click = ">=8.0.1"
 pydantic = ">=2.0a1"
 httpx = ">=0.24.1"
+typing-extensions = "^4.6.3"
 
 [tool.poetry.group.dev.dependencies]
 Pygments = ">=2.10.0"
 bandit = ">=1.7.4"
 black = ">=21.10b0"
 coverage = { extras = ["toml"], version = ">=6.2" }
 flake8 = ">=6.0.0"
```

### Comparing `kadaster_kikinzage_client-0.1.2/src/kikinzage/__main__.py` & `kadaster_kikinzage_client-0.1.3/src/kikinzage/__main__.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.2/src/kikinzage/client/asyncio.py` & `kadaster_kikinzage_client-0.1.3/src/kikinzage/client/asyncio.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,57 +5,49 @@
 from typing import Union
 
 import httpx
 from httpx import USE_CLIENT_DEFAULT
 from httpx._client import UseClientDefault
 
 from .. import models
-from ..models import Formaat
 from ..models import ResponseType
+from ..models.enum import Formaat
 from .base import KikinzageBaseClient
 
 
 class AsyncClient(KikinzageBaseClient):
     """Client for async requests"""
 
     client: httpx.AsyncClient
 
-    def __init__(
+    async def __aenter__(self) -> "AsyncClient":
+        await self.client.__aenter__()
+        return self
+
+    async def __aexit__(
         self,
-        username: str,
-        password: str,
-        base_url: str = "https://service10.kadaster.nl/kik-inzage-eto/v6/",
-        formaat: Formaat = Formaat.JSON,
-        klantreferentie: Optional[str] = None,
-        gebruikeridentificatie: Optional[str] = None,
-        hyperlinkopproduct: Optional[bool] = None,
-        inkoopnummer: Optional[str] = None,
-        referentienummer: Optional[str] = None,
-        **httpx_kwargs: Any,
+        exc_type: Optional[Type[BaseException]] = None,
+        exc_value: Optional[BaseException] = None,
+        traceback: Optional[TracebackType] = None,
     ) -> None:
-        super().__init__(
-            username=username,
-            password=password,
-            base_url=base_url,
-            formaat=formaat,
-            klantreferentie=klantreferentie,
-            gebruikeridentificatie=gebruikeridentificatie,
-            hyperlinkopproduct=hyperlinkopproduct,
-            inkoopnummer=inkoopnummer,
-            referentienummer=referentienummer,
-        )
-
-        httpx_kwargs.setdefault("base_url", base_url)
-        httpx_kwargs.setdefault("auth", (self.username, self.password))
-
-        self.client = self.create_client(**httpx_kwargs)
+        await self.client.__aexit__(exc_type, exc_value, traceback)
 
     def create_client(self, **httpx_kwargs: Any) -> httpx.AsyncClient:
         return httpx.AsyncClient(**httpx_kwargs)
 
+    async def send(
+        self,
+        request: httpx.Request,
+        model: Type[ResponseType],
+        status_code_success: int = 200,
+    ) -> ResponseType:
+        response = await self.client.send(request)
+
+        return self.process_response(response, model, status_code_success)
+
     async def eigendomsinformatie_kadastraalobjectidentificatie(
         self,
         kadastraalobjectidentificatie: str,
         formaat: Union[Formaat, UseClientDefault] = USE_CLIENT_DEFAULT,
         klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
         gebruikeridentificatie: Optional[str] = None,
         hyperlinkopproduct: Optional[bool] = None,
@@ -71,29 +63,7 @@
             gebruikeridentificatie=gebruikeridentificatie,
             hyperlinkopproduct=hyperlinkopproduct,
             inkoopnummer=inkoopnummer,
             referentienummer=referentienummer,
         )
 
         return await self.send(request, models.Eigendomsinformatie)
-
-    async def send(
-        self,
-        request: httpx.Request,
-        model: Type[ResponseType],
-        status_code_success: int = 200,
-    ) -> ResponseType:
-        response = await self.client.send(request)
-
-        return self.process_response(response, model, status_code_success)
-
-    async def __aenter__(self) -> "AsyncClient":
-        await self.client.__aenter__()
-        return self
-
-    async def __aexit__(
-        self,
-        exc_type: Optional[Type[BaseException]] = None,
-        exc_value: Optional[BaseException] = None,
-        traceback: Optional[TracebackType] = None,
-    ) -> None:
-        await self.client.__aexit__(exc_type, exc_value, traceback)
```

### Comparing `kadaster_kikinzage_client-0.1.2/src/kikinzage/client/base.py` & `kadaster_kikinzage_client-0.1.3/src/kikinzage/client/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 import httpx
 from httpx import USE_CLIENT_DEFAULT
 from httpx import Request
 from httpx._client import BaseClient
 from httpx._client import UseClientDefault
 
-from ..models import Formaat
 from ..models import ResponseType
+from ..models.enum import Formaat
 from . import errors
 from .utils import kwargs_as_params
 
 
 class KikinzageBaseClient(ABC):
     """Class with method shared between async and default client"""
 
@@ -39,25 +39,34 @@
         base_url: str = "https://service10.kadaster.nl/kik-inzage-eto/v6/",
         formaat: Formaat = Formaat.JSON,
         klantreferentie: Optional[str] = None,
         gebruikeridentificatie: Optional[str] = None,
         hyperlinkopproduct: Optional[bool] = None,
         inkoopnummer: Optional[str] = None,
         referentienummer: Optional[str] = None,
+        **httpx_kwargs: Any,
     ) -> None:
         self.klantreferentie = klantreferentie
         self.username = username
         self.password = password
         self.base_url = base_url
         self.formaat = formaat
         self.gebruikeridentificatie = gebruikeridentificatie
         self.hyperlinkopproduct = hyperlinkopproduct
         self.inkoopnummer = inkoopnummer
         self.referentienummer = referentienummer
 
+        httpx_kwargs.setdefault("base_url", base_url)
+        httpx_kwargs.setdefault("auth", (self.username, self.password))
+
+        self.client = self.create_client(**httpx_kwargs)
+
+    def create_client(self, **httpx_kwargs: Any) -> BaseClient:
+        raise NotImplementedError
+
     def process_response(
         self,
         response: httpx.Response,
         model: Type[ResponseType],
         status_code_success: int = 200,
     ) -> ResponseType:
         try:
@@ -88,14 +97,29 @@
 
     def map_exception(self, response: httpx.Response) -> Type[errors.KIKRequestError]:
         exception_type = self.ERROR_RESPONSE_MAPPING.get(
             response.status_code, errors.KIKRequestError
         )
         return exception_type
 
+    def _get_klantreferentie(
+        self, klantreferentie: Union[str, UseClientDefault]
+    ) -> str:
+        if isinstance(klantreferentie, str):
+            return klantreferentie
+        elif self.klantreferentie is not None:
+            return self.klantreferentie
+
+        raise errors.KIKError(
+            "`klantreferentie` is required, pass it as parameter or set `self.klantreferentie`"
+        )
+
+    def _get_formaat(self, formaat: Union[Formaat, UseClientDefault]) -> str:
+        return formaat.value if isinstance(formaat, Formaat) else self.formaat.value
+
     def request_eigendomsinformatie_kadastraleaanduiding(
         self,
         kadastralegemeente: str,
         sectie: str,
         perceelnummer: int,
         appartementsrecht_volgnummer: Optional[int] = None,
         *,
@@ -234,22 +258,7 @@
         request = self.client.build_request(
             method="GET",
             url=f"eigendomsinformatie/adres/{plaatsnaam}/{straatnaam}/{huisnummer}",
             params=params,
         )
 
         return request
-
-    def _get_klantreferentie(
-        self, klantreferentie: Union[str, UseClientDefault]
-    ) -> str:
-        if isinstance(klantreferentie, str):
-            return klantreferentie
-        elif self.klantreferentie is not None:
-            return self.klantreferentie
-
-        raise errors.KIKError(
-            "`klantreferentie` is required, pass it as parameter or set `self.klantreferentie`"
-        )
-
-    def _get_formaat(self, formaat: Union[Formaat, UseClientDefault]) -> str:
-        return formaat.value if isinstance(formaat, Formaat) else self.formaat.value
```

### Comparing `kadaster_kikinzage_client-0.1.2/src/kikinzage/client/default.py` & `kadaster_kikinzage_client-0.1.3/src/kikinzage/client/default.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,57 +4,37 @@
 from typing import Union
 
 import httpx
 from httpx._client import USE_CLIENT_DEFAULT
 from httpx._client import UseClientDefault
 
 from .. import models
-from ..models import Formaat
 from ..models import ResponseType
+from ..models.enum import Formaat
 from .base import KikinzageBaseClient
 
 
 class DefaultClient(KikinzageBaseClient):
     """Synchronous client"""
 
     client: httpx.Client
 
-    def __init__(
-        self,
-        username: str,
-        password: str,
-        base_url: str = "https://service10.kadaster.nl/kik-inzage-eto/v6/",
-        formaat: Formaat = Formaat.JSON,
-        klantreferentie: Optional[str] = None,
-        gebruikeridentificatie: Optional[str] = None,
-        hyperlinkopproduct: Optional[bool] = None,
-        inkoopnummer: Optional[str] = None,
-        referentienummer: Optional[str] = None,
-        **httpx_kwargs: Any,
-    ) -> None:
-        super().__init__(
-            username=username,
-            password=password,
-            base_url=base_url,
-            formaat=formaat,
-            klantreferentie=klantreferentie,
-            gebruikeridentificatie=gebruikeridentificatie,
-            hyperlinkopproduct=hyperlinkopproduct,
-            inkoopnummer=inkoopnummer,
-            referentienummer=referentienummer,
-        )
-
-        httpx_kwargs.setdefault("base_url", base_url)
-        httpx_kwargs.setdefault("auth", (self.username, self.password))
-
-        self.client = self.create_client(**httpx_kwargs)
-
     def create_client(self, **httpx_kwargs: Any) -> httpx.Client:
         return httpx.Client(**httpx_kwargs)
 
+    def send(
+        self,
+        request: httpx.Request,
+        model: Type[ResponseType],
+        status_code_success: int = 200,
+    ) -> ResponseType:
+        response = self.client.send(request)
+
+        return self.process_response(response, model, status_code_success)
+
     def eigendomsinformatie_kadastraalobjectidentificatie(
         self,
         kadastraalobjectidentificatie: str,
         formaat: Union[Formaat, UseClientDefault] = USE_CLIENT_DEFAULT,
         klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
         gebruikeridentificatie: Optional[str] = None,
         hyperlinkopproduct: Optional[bool] = None,
@@ -156,17 +136,7 @@
             gebruikeridentificatie=gebruikeridentificatie,
             hyperlinkopproduct=hyperlinkopproduct,
             inkoopnummer=inkoopnummer,
             referentienummer=referentienummer,
         )
 
         return self.send(request, models.Eigendomsinformatie)
-
-    def send(
-        self,
-        request: httpx.Request,
-        model: Type[ResponseType],
-        status_code_success: int = 200,
-    ) -> ResponseType:
-        response = self.client.send(request)
-
-        return self.process_response(response, model, status_code_success)
```

### Comparing `kadaster_kikinzage_client-0.1.2/src/kikinzage/client/errors.py` & `kadaster_kikinzage_client-0.1.3/src/kikinzage/client/errors.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.2/PKG-INFO` & `kadaster_kikinzage_client-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kadaster-kikinzage-client
-Version: 0.1.2
+Version: 0.1.3
 Summary:  Kadaster - KIK Inzage API Python client
 Home-page: https://github.com/foarsitter/kadaster-kik-inzage-api-python-client
 License: MIT
 Author: Jelmer Draaijer
 Author-email: info@jelmert.nl
 Requires-Python: >=3.8.1
 Classifier: Development Status :: 4 - Beta
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0.1)
 Requires-Dist: httpx (>=0.24.1)
 Requires-Dist: pydantic (>=2.0a1)
+Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
 Project-URL: Changelog, https://github.com/foarsitter/kadaster-kik-inzage-api-python-client/releases
 Project-URL: Documentation, https://kadaster-kik-inzage-api-python-client.readthedocs.io
 Project-URL: Repository, https://github.com/foarsitter/kadaster-kik-inzage-api-python-client
 Description-Content-Type: text/markdown
 
 # Kadaster - KIK Inzage API Python client
```

