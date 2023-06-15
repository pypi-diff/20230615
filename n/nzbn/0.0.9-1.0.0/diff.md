# Comparing `tmp/nzbn-0.0.9.tar.gz` & `tmp/nzbn-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nzbn-0.0.9.tar", last modified: Fri Dec 10 05:33:55 2021, max compression
+gzip compressed data, was "nzbn-1.0.0.tar", last modified: Thu Jun 15 03:36:42 2023, max compression
```

## Comparing `nzbn-0.0.9.tar` & `nzbn-1.0.0.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-12-10 05:33:55.185880 nzbn-0.0.9/
--rw-r--r--   0 hugh       (501) staff       (20)     1066 2021-12-08 01:13:11.000000 nzbn-0.0.9/LICENSE
--rw-r--r--   0 hugh       (501) staff       (20)     1240 2021-12-10 05:33:55.185774 nzbn-0.0.9/PKG-INFO
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-12-10 05:33:55.184419 nzbn-0.0.9/nzbn/
--rw-r--r--   0 hugh       (501) staff       (20)      507 2021-12-09 22:53:24.000000 nzbn-0.0.9/nzbn/__init__.py
--rw-r--r--   0 hugh       (501) staff       (20)     7154 2021-12-10 04:25:04.000000 nzbn-0.0.9/nzbn/abbreviated_entity.py
--rw-r--r--   0 hugh       (501) staff       (20)     3249 2021-12-09 23:52:02.000000 nzbn-0.0.9/nzbn/address.py
--rw-r--r--   0 hugh       (501) staff       (20)        0 2021-12-09 19:03:41.000000 nzbn-0.0.9/nzbn/address_type.py
--rw-r--r--   0 hugh       (501) staff       (20)     1318 2021-12-10 05:32:47.000000 nzbn-0.0.9/nzbn/classification.py
--rw-r--r--   0 hugh       (501) staff       (20)      400 2021-12-08 08:56:06.000000 nzbn-0.0.9/nzbn/disposition.py
--rw-r--r--   0 hugh       (501) staff       (20)     4482 2021-12-10 00:07:38.000000 nzbn-0.0.9/nzbn/entity.py
--rw-r--r--   0 hugh       (501) staff       (20)      884 2021-12-09 09:55:22.000000 nzbn-0.0.9/nzbn/entity_status.py
--rw-r--r--   0 hugh       (501) staff       (20)     1181 2021-12-08 08:56:06.000000 nzbn-0.0.9/nzbn/entity_type.py
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-12-10 05:33:55.185176 nzbn-0.0.9/nzbn/errors/
--rw-r--r--   0 hugh       (501) staff       (20)        0 2021-12-08 08:54:35.000000 nzbn-0.0.9/nzbn/errors/__init__.py
--rw-r--r--   0 hugh       (501) staff       (20)      749 2021-12-10 04:28:33.000000 nzbn-0.0.9/nzbn/errors/api.py
--rw-r--r--   0 hugh       (501) staff       (20)      144 2021-12-08 08:56:06.000000 nzbn-0.0.9/nzbn/errors/error.py
--rw-r--r--   0 hugh       (501) staff       (20)      576 2021-12-08 08:56:06.000000 nzbn-0.0.9/nzbn/errors/type_error.py
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-12-10 05:33:55.185634 nzbn-0.0.9/nzbn/http/
--rw-r--r--   0 hugh       (501) staff       (20)        0 2021-12-08 01:01:49.000000 nzbn-0.0.9/nzbn/http/__init__.py
--rw-r--r--   0 hugh       (501) staff       (20)     2624 2021-12-10 00:07:26.000000 nzbn-0.0.9/nzbn/http/api_request.py
--rw-r--r--   0 hugh       (501) staff       (20)      251 2021-12-08 08:56:06.000000 nzbn-0.0.9/nzbn/http/method.py
--rw-r--r--   0 hugh       (501) staff       (20)     1387 2021-12-09 10:31:31.000000 nzbn-0.0.9/nzbn/http/query_parameter.py
--rw-r--r--   0 hugh       (501) staff       (20)     1002 2021-12-08 08:56:06.000000 nzbn-0.0.9/nzbn/http/query_parameters.py
--rw-r--r--   0 hugh       (501) staff       (20)      340 2021-12-08 08:56:06.000000 nzbn-0.0.9/nzbn/order.py
--rw-r--r--   0 hugh       (501) staff       (20)     1223 2021-12-09 19:12:06.000000 nzbn-0.0.9/nzbn/time.py
--rw-r--r--   0 hugh       (501) staff       (20)     1066 2021-12-09 06:25:06.000000 nzbn-0.0.9/nzbn/trading_name.py
--rw-r--r--   0 hugh       (501) staff       (20)       18 2021-12-10 04:27:28.000000 nzbn-0.0.9/nzbn/version.py
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2021-12-10 05:33:55.184816 nzbn-0.0.9/nzbn.egg-info/
--rw-r--r--   0 hugh       (501) staff       (20)     1240 2021-12-10 05:33:55.000000 nzbn-0.0.9/nzbn.egg-info/PKG-INFO
--rw-r--r--   0 hugh       (501) staff       (20)      589 2021-12-10 05:33:55.000000 nzbn-0.0.9/nzbn.egg-info/SOURCES.txt
--rw-r--r--   0 hugh       (501) staff       (20)        1 2021-12-10 05:33:55.000000 nzbn-0.0.9/nzbn.egg-info/dependency_links.txt
--rw-r--r--   0 hugh       (501) staff       (20)        5 2021-12-10 05:33:55.000000 nzbn-0.0.9/nzbn.egg-info/top_level.txt
--rw-r--r--   0 hugh       (501) staff       (20)       38 2021-12-10 05:33:55.185928 nzbn-0.0.9/setup.cfg
--rw-r--r--   0 hugh       (501) staff       (20)     1666 2021-12-08 08:56:09.000000 nzbn-0.0.9/setup.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2023-06-15 03:36:42.597294 nzbn-1.0.0/
+-rw-r--r--   0 hugh       (501) staff       (20)     1066 2021-12-08 01:13:11.000000 nzbn-1.0.0/LICENSE
+-rw-r--r--   0 hugh       (501) staff       (20)     2612 2023-06-15 03:36:42.597184 nzbn-1.0.0/PKG-INFO
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2023-06-15 03:36:42.595630 nzbn-1.0.0/nzbn/
+-rw-r--r--   0 hugh       (501) staff       (20)      533 2023-06-15 03:25:52.000000 nzbn-1.0.0/nzbn/__init__.py
+-rw-r--r--   0 hugh       (501) staff       (20)     7248 2023-06-15 03:33:26.000000 nzbn-1.0.0/nzbn/abbreviated_entity.py
+-rw-r--r--   0 hugh       (501) staff       (20)     3401 2023-02-07 04:39:24.000000 nzbn-1.0.0/nzbn/address.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1366 2022-02-24 23:47:16.000000 nzbn-1.0.0/nzbn/classification.py
+-rw-r--r--   0 hugh       (501) staff       (20)      400 2021-12-08 08:56:06.000000 nzbn-1.0.0/nzbn/disposition.py
+-rw-r--r--   0 hugh       (501) staff       (20)     4613 2023-06-15 03:33:26.000000 nzbn-1.0.0/nzbn/entity.py
+-rw-r--r--   0 hugh       (501) staff       (20)      884 2021-12-09 09:55:22.000000 nzbn-1.0.0/nzbn/entity_status.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1181 2021-12-08 08:56:06.000000 nzbn-1.0.0/nzbn/entity_type.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2023-06-15 03:36:42.596566 nzbn-1.0.0/nzbn/errors/
+-rw-r--r--   0 hugh       (501) staff       (20)        0 2021-12-08 08:54:35.000000 nzbn-1.0.0/nzbn/errors/__init__.py
+-rw-r--r--   0 hugh       (501) staff       (20)      749 2021-12-10 04:28:33.000000 nzbn-1.0.0/nzbn/errors/api.py
+-rw-r--r--   0 hugh       (501) staff       (20)      144 2021-12-08 08:56:06.000000 nzbn-1.0.0/nzbn/errors/error.py
+-rw-r--r--   0 hugh       (501) staff       (20)      576 2021-12-08 08:56:06.000000 nzbn-1.0.0/nzbn/errors/type_error.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2023-06-15 03:36:42.597046 nzbn-1.0.0/nzbn/http/
+-rw-r--r--   0 hugh       (501) staff       (20)        0 2021-12-08 01:01:49.000000 nzbn-1.0.0/nzbn/http/__init__.py
+-rw-r--r--   0 hugh       (501) staff       (20)     2649 2023-06-15 03:33:26.000000 nzbn-1.0.0/nzbn/http/api_request.py
+-rw-r--r--   0 hugh       (501) staff       (20)      251 2021-12-08 08:56:06.000000 nzbn-1.0.0/nzbn/http/method.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1387 2021-12-09 10:31:31.000000 nzbn-1.0.0/nzbn/http/query_parameter.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1002 2021-12-08 08:56:06.000000 nzbn-1.0.0/nzbn/http/query_parameters.py
+-rw-r--r--   0 hugh       (501) staff       (20)      340 2021-12-08 08:56:06.000000 nzbn-1.0.0/nzbn/order.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1706 2022-09-15 23:10:18.000000 nzbn-1.0.0/nzbn/time.py
+-rw-r--r--   0 hugh       (501) staff       (20)     1115 2021-12-10 06:03:11.000000 nzbn-1.0.0/nzbn/trading_name.py
+-rw-r--r--   0 hugh       (501) staff       (20)       18 2023-06-15 03:32:32.000000 nzbn-1.0.0/nzbn/version.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2023-06-15 03:36:42.596139 nzbn-1.0.0/nzbn.egg-info/
+-rw-r--r--   0 hugh       (501) staff       (20)     2612 2023-06-15 03:36:42.000000 nzbn-1.0.0/nzbn.egg-info/PKG-INFO
+-rw-r--r--   0 hugh       (501) staff       (20)      568 2023-06-15 03:36:42.000000 nzbn-1.0.0/nzbn.egg-info/SOURCES.txt
+-rw-r--r--   0 hugh       (501) staff       (20)        1 2023-06-15 03:36:42.000000 nzbn-1.0.0/nzbn.egg-info/dependency_links.txt
+-rw-r--r--   0 hugh       (501) staff       (20)        5 2023-06-15 03:36:42.000000 nzbn-1.0.0/nzbn.egg-info/top_level.txt
+-rw-r--r--   0 hugh       (501) staff       (20)       38 2023-06-15 03:36:42.597333 nzbn-1.0.0/setup.cfg
+-rw-r--r--   0 hugh       (501) staff       (20)     1666 2021-12-08 08:56:09.000000 nzbn-1.0.0/setup.py
```

### Comparing `nzbn-0.0.9/LICENSE` & `nzbn-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nzbn-0.0.9/nzbn/abbreviated_entity.py` & `nzbn-1.0.0/nzbn/abbreviated_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         self,
         entity_name: str,
         status: EntityStatus,
         nzbn: str,
         entity_type: EntityType,
         trading_names: List[TradingName],
         classifications: List[Classification],
-        registration_date: NzbnTime,
+        registration_date: Optional[NzbnTime],
         disposition: Disposition
     ) -> None:
 
         self._entity_name = entity_name
         self._status = status
         self._nzbn = nzbn
         self._entity_type = entity_type
@@ -53,15 +53,17 @@
     status: EntityStatus = property(lambda s: s._status)
     nzbn: str = property(lambda s: s._nzbn)
     entity_type: EntityType = property(lambda s: s._entity_type)
     trading_names: List[str] = property(lambda s: s._trading_names)
     classifications: List[Classification] = property(
         lambda s: s._classifications
     )
-    registration_date: NzbnTime = property(lambda s: s._registration_date)
+    registration_date: Optional[NzbnTime] = property(
+        lambda s: s._registration_date
+    )
     disposition: Disposition = property(
         lambda s: s._disposition
     )
 
     @classmethod
     def decode_encapsulated_list(
         Self: Type[Self],
@@ -106,27 +108,29 @@
             status=EntityStatus(data['entityStatusCode']),
             nzbn=data['nzbn'],
             entity_type=EntityType(data['entityTypeCode']),
             trading_names=TradingName.decode_many(data['tradingNames']),
             classifications=Classification.decode_many(
                 data['classifications']
             ) if 'classifications' in data else [],
-            registration_date=NzbnTime.decode(data['registrationDate']),
+            registration_date=NzbnTime.optionally_decode(
+                data['registrationDate']
+            ),
             disposition=disposition or Disposition(
                 1,
                 1,
                 1,
                 1
             )
         )
 
     @classmethod
     def retrieve_many(
         Self: Type[Self],
-        access_token: str,
+        api_key: str,
         page: int = 0,
         limit: int = 20,
         search_text: Optional[str] = None,
         entity_status: Optional[Union[
             EntityStatus,
             List[EntityStatus]
         ]] = None,
@@ -228,12 +232,14 @@
 
             pass
 
         result = ApiRequest.make(
             path=Self.path,
             method=HTTPMethod.GET,
             query_parameters=QueryParameters(parameters),
-            access_token=access_token,
+            api_key=api_key,
             sandbox=sandbox
         )
 
         return Self.decode_encapsulated_list(result)
+
+SearchEntity = AbbreviatedEntity
```

### Comparing `nzbn-0.0.9/nzbn/address.py` & `nzbn-1.0.0/nzbn/address.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,23 +13,27 @@
 
 
 class AddressType(Enum):
 
     POSTAL = 'POSTAL'
     REGISTERED = 'REGISTERED'
     SERVICE = 'SERVICE'
-
+    RECORDS = 'RECORDS'
+    SHAREREGISTER = 'SHAREREGISTER'
+    OFFICE = 'OFFICE'
+    DELIVERY = 'DELIVERY'
+    INVOICE = 'INVOICE'
 
 
 class Address:
 
     def __init__(
         self,
         unique_identifier: str,
-        start_date: NzbnTime,
+        start_date: Optional[NzbnTime],
         end_date: Optional[NzbnTime],
         care_of: Optional[str],
         address_1: str,
         address_2: Optional[str],
         address_3: Optional[str],
         address_4: Optional[str],
         post_code: Optional[str],
@@ -69,28 +73,28 @@
     address_type: Optional[AddressType] = property(
         lambda s: s._address_type
     )
     paf_id: Optional[str] = property(lambda s: s._paf_id)
 
     expired: bool = property(
         lambda s: (
-            s._end_date is not None and s._end_date <= datetime.utcnow()
+            s._end_date is not None and s._end_date <= NzbnTime.utcnow()
         )
     )
     not_expired: bool = property(lambda s: not s.expired)
 
     @classmethod
     def decode(
         Self: Type[Self],
         data: Dict[str, Optional[str]]
     ) -> Self:
 
         return Address(
             unique_identifier=data['uniqueIdentifier'],
-            start_date=NzbnTime.decode(data['startDate']),
+            start_date=NzbnTime.optionally_decode(data['startDate']),
             end_date=NzbnTime.optionally_decode(data['endDate']),
             care_of=data['careOf'],
             address_1=data['address1'],
             address_2=data['address2'],
             address_3=data['address3'],
             address_4=data['address4'],
             post_code=data['postCode'],
```

### Comparing `nzbn-0.0.9/nzbn/classification.py` & `nzbn-1.0.0/nzbn/classification.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 """
 New Zealand Business Number
 Classification Module
 author: hugh@procuret.com
 © Procuret Operating Pty Ltd
 """
-from typing import List, Dict, TypeVar, Type
+from typing import List, Dict, TypeVar, Type, Optional
 
 Self = TypeVar('Self', bound='Classification')
 
 
 class Classification:
 
     def __init__(
         self,
-        unique_identifier: str,
+        unique_identifier: Optional[str],
         classification_code: str,
         classification_description: str
     ) -> None:
 
         self._unique_identifier = unique_identifier
         self._classification_code = classification_code
         self._classification_description = classification_description
 
         return
 
-    unique_identifier = property(lambda s: s._unique_identifier)
+    unique_identifier: Optional[str] = property(
+        lambda s: s._unique_identifier
+    )
     classification_code = property(lambda s: s._classification_code)
     classification_description = property(
         lambda s: s._classification_description
     )
 
     @classmethod
     def decode(
         Self: Type[Self],
         data: Dict[str, str]
     ) -> Self:
 
         return Classification(
-            unique_identifier=data['unique_identifier'],
-            classification_code=data['classification_code'],
-            classification_description=data['classification_description']
+            unique_identifier=(data['uniqueIdentifier']),
+            classification_code=data['classificationCode'],
+            classification_description=data['classificationDescription']
         )
 
     @classmethod
     def decode_many(
         Self: Type[Self],
         data: List[Dict[str, str]]
     ) -> List[Self]:
```

### Comparing `nzbn-0.0.9/nzbn/entity.py` & `nzbn-1.0.0/nzbn/entity.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 from nzbn.address import Address
 
 Self = TypeVar('Self', bound='Entity')
 
 
 class Entity:
 
+    # A "FullEntity" response from the NZBN API
+    # https://portal.api.business.govt.nz/api-details#api=nzbn&operation=EntitiesByNzbnGet
+
     path = '/entities'
 
     def __init__(
         self,
         entity_name: str,
         status: EntityStatus,
         nzbn: str,
@@ -109,21 +112,21 @@
             ),
             addresses=Address.decode_many(data['addresses']['addressList'])
         )
 
     @classmethod
     def retrieve(
         Self: Type[Self],
-        access_token: str,
+        api_key: str,
         nzbn: str,
         sandbox: bool = False
     ) -> Optional[Self]:
 
-        if not isinstance(access_token, str):
-            raise NzbnTypeError('access_token', access_token, 'str')
+        if not isinstance(api_key, str):
+            raise NzbnTypeError('api_key', api_key, 'str')
         
         if not isinstance(nzbn, str):
             raise NzbnTypeError('nzbn', nzbn, 'str')
         
         if len(nzbn) != 13:
             raise NzbnError('nzbn must be 13 characters')
         
@@ -131,15 +134,17 @@
             if character not in '0123456789':
                 raise NzbnError('nzbn must be only numeric characters')
             continue
 
         result = ApiRequest.make(
             path=Self.path + '/' + nzbn,
             method=HTTPMethod.GET,
-            access_token=access_token,
+            api_key=api_key,
             sandbox=sandbox
         )
         
         if result is None:
             return None
         
         return Self.decode(result)
+
+FullEntity = Entity
```

### Comparing `nzbn-0.0.9/nzbn/entity_status.py` & `nzbn-1.0.0/nzbn/entity_status.py`

 * *Files identical despite different names*

### Comparing `nzbn-0.0.9/nzbn/entity_type.py` & `nzbn-1.0.0/nzbn/entity_type.py`

 * *Files identical despite different names*

### Comparing `nzbn-0.0.9/nzbn/errors/api.py` & `nzbn-1.0.0/nzbn/errors/api.py`

 * *Files identical despite different names*

### Comparing `nzbn-0.0.9/nzbn/errors/type_error.py` & `nzbn-1.0.0/nzbn/errors/type_error.py`

 * *Files identical despite different names*

### Comparing `nzbn-0.0.9/nzbn/http/api_request.py` & `nzbn-1.0.0/nzbn/http/api_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,46 +10,47 @@
 from nzbn.http.query_parameters import QueryParameters
 from nzbn.errors.api import NzbnApiError
 from urllib.request import HTTPError
 from urllib.request import Request
 from urllib.request import urlopen
 from nzbn.version import VERSION as AGENT_VERSION
 
-SANDBOX_ENDPOINT = 'https://sandbox.api.business.govt.nz/services/v4/nzbn'
-API_ENDPOINT = 'https://api.business.govt.nz/services/v4/nzbn'
+SANDBOX_ENDPOINT = 'https://api.business.govt.nz/sandbox/nzbn/v5'
+API_ENDPOINT = 'https://api.business.govt.nz/gateway/nzbn/v5/'
 USER_AGENT = 'NZBN Python ' + AGENT_VERSION
 
 
 class ApiRequest:
 
     @staticmethod
     def make(
         path: str,
         method: HTTPMethod,
-        access_token: Optional[str] = None,
+        api_key: Optional[str] = None,
         data: Optional[Union[Dict, List[Dict]]] = None,
         query_parameters: Optional[QueryParameters] = None,
         api_endpoint: Optional[str] = None,
         throw_on_404: bool = False,
-        sandbox: bool = False
+        sandbox: bool = False,
+        timeout: int = 10
     ) -> Optional[Union[Dict, List[Dict]]]:
         """Return the decoded json body of a response from the Procuret API"""
 
         api_endpoint = api_endpoint or (
             SANDBOX_ENDPOINT if sandbox is True
             else API_ENDPOINT
         )
 
         url = api_endpoint + path
         if query_parameters is not None:
             url = query_parameters.add_to(url)
 
         headers = {
             'User-Agent': USER_AGENT,
-            'Authorization': 'Bearer ' + access_token
+            'Ocp-Apim-Subscription-Key': api_key
         }
 
         encoded_data: Optional[bytes] = None
         if data is not None:
             encoded_data = json.dumps(data).encode('utf-8')
             headers['Content-Type'] = 'application/json'
 
@@ -57,15 +58,15 @@
             url=url,
             method=method.value,
             data=encoded_data,
             headers=headers
         )
 
         try:
-            response = urlopen(request).read()
+            response = urlopen(request, timeout=timeout).read()
         except HTTPError as error:
             if error.code == 404 and throw_on_404 is False:
                 return None
             body: Optional[str] = None
             try:
                 body = error.read()
                 try:
```

### Comparing `nzbn-0.0.9/nzbn/http/query_parameter.py` & `nzbn-1.0.0/nzbn/http/query_parameter.py`

 * *Files identical despite different names*

### Comparing `nzbn-0.0.9/nzbn/http/query_parameters.py` & `nzbn-1.0.0/nzbn/http/query_parameters.py`

 * *Files identical despite different names*

### Comparing `nzbn-0.0.9/nzbn/time.py` & `nzbn-1.0.0/nzbn/time.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """
 New Zealand Business Number
 Time Module
 author: hugh@procuret.com
 © Procuret Operating Pty Ltd
 """
-from datetime import datetime, tzinfo
+from datetime import datetime, tzinfo, timedelta
 from typing import Optional, TypeVar, Type
 
 Self = TypeVar('Self', bound='NzbnTime')
 
 
 class TimeZoneUTC(tzinfo):
     """
     UTC timezone.
     """
     def utcoffset(self, dt):
-        return datetime.timedelta(0)
+        return timedelta(0)
 
     def tzname(self, dt):
         return 'UTC'
 
     def dst(self, dt):
-        return datetime.timedelta(0)
+        return timedelta(0)
 
 
 UTC = TimeZoneUTC()
 
 
 class NzbnTime(datetime):
 
@@ -54,7 +54,25 @@
         data: Optional[str]
     ) -> Optional[Self]:
 
         if data is None:
             return None
         
         return Self.decode(data)
+
+    @classmethod
+    def utcnow(Self: Type[Self]) -> Self:
+        time = datetime.utcnow()
+        return Self._from_datetime(time)
+
+    @classmethod
+    def _from_datetime(Self: Type[Self], time: datetime) -> Self:
+        return Self(
+            year=time.year,
+            month=time.month,
+            day=time.day,
+            hour=time.hour,
+            minute=time.minute,
+            second=time.second,
+            microsecond=time.microsecond,
+            tzinfo=UTC
+        )
```

### Comparing `nzbn-0.0.9/nzbn/trading_name.py` & `nzbn-1.0.0/nzbn/trading_name.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """
 New Zealand Business Number
 Trading Name Module
 author: hugh@procuret.com
 © Procuret Operating Pty Ltd
 """
-from typing import Type,  TypeVar, Dict, List
+from typing import Type,  TypeVar, Dict, List, Optional
 from nzbn.time import NzbnTime
 
 Self = TypeVar('Self', bound='TradingName')
 
 
 class TradingName:
 
     def __init__(
         self,
         unique_identifier: str,
         name: str,
-        start_date: NzbnTime,
-        end_date: NzbnTime
+        start_date: Optional[NzbnTime],
+        end_date: Optional[NzbnTime]
     ) -> None:
 
         self._unique_identifier = unique_identifier
         self._name = name
         self._start_date = start_date
         self._end_date = end_date
 
         return
     
     @classmethod
     def decode(Self: Type[Self], data: Dict[str, str]) -> Self:
         return Self(
-            unique_identifier=data['unique_identifier'],
+            unique_identifier=data['uniqueIdentifier'],
             name=data['name'],
-            start_date=NzbnTime.decode(data['start_date']),
-            end_date=NzbnTime.decode(data['end_date'])
+            start_date=NzbnTime.optionally_decode(data['startDate']),
+            end_date=NzbnTime.optionally_decode(data['endDate'])
         )
 
     @classmethod
     def decode_many(
         Self: Type[Self],
         data: List[Dict[str, str]]
     ) -> List[Self]:
```

### Comparing `nzbn-0.0.9/setup.py` & `nzbn-1.0.0/setup.py`

 * *Files identical despite different names*

