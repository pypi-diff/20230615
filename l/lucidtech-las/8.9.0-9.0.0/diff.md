# Comparing `tmp/lucidtech-las-8.9.0.tar.gz` & `tmp/lucidtech-las-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lucidtech-las-8.9.0.tar", last modified: Wed Mar  1 15:24:39 2023, max compression
+gzip compressed data, was "lucidtech-las-9.0.0.tar", last modified: Thu Jun 15 08:08:49 2023, max compression
```

## Comparing `lucidtech-las-8.9.0.tar` & `lucidtech-las-9.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:24:39.788257 lucidtech-las-8.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-03-01 15:24:29.000000 lucidtech-las-8.9.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-01 15:24:29.000000 lucidtech-las-8.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-03-01 15:24:39.788257 lucidtech-las-8.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-03-01 15:24:29.000000 lucidtech-las-8.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:24:39.784257 lucidtech-las-8.9.0/las/
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-03-01 15:24:29.000000 lucidtech-las-8.9.0/las/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-01 15:24:29.000000 lucidtech-las-8.9.0/las/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    96232 2023-03-01 15:24:29.000000 lucidtech-las-8.9.0/las/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-03-01 15:24:29.000000 lucidtech-las-8.9.0/las/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:24:39.788257 lucidtech-las-8.9.0/lucidtech_las.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-03-01 15:24:39.000000 lucidtech-las-8.9.0/lucidtech_las.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-01 15:24:39.000000 lucidtech-las-8.9.0/lucidtech_las.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 15:24:39.000000 lucidtech-las-8.9.0/lucidtech_las.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-01 15:24:39.000000 lucidtech-las-8.9.0/lucidtech_las.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-01 15:24:39.000000 lucidtech-las-8.9.0/lucidtech_las.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-01 15:24:29.000000 lucidtech-las-8.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-01 15:24:39.788257 lucidtech-las-8.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-03-01 15:24:29.000000 lucidtech-las-8.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:08:49.455413 lucidtech-las-9.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-15 08:08:37.000000 lucidtech-las-9.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-15 08:08:37.000000 lucidtech-las-9.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-15 08:08:49.455413 lucidtech-las-9.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-15 08:08:37.000000 lucidtech-las-9.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:08:49.451413 lucidtech-las-9.0.0/las/
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-15 08:08:37.000000 lucidtech-las-9.0.0/las/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-15 08:08:37.000000 lucidtech-las-9.0.0/las/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101292 2023-06-15 08:08:37.000000 lucidtech-las-9.0.0/las/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-15 08:08:37.000000 lucidtech-las-9.0.0/las/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:08:49.455413 lucidtech-las-9.0.0/lucidtech_las.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-15 08:08:49.000000 lucidtech-las-9.0.0/lucidtech_las.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-15 08:08:49.000000 lucidtech-las-9.0.0/lucidtech_las.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 08:08:49.000000 lucidtech-las-9.0.0/lucidtech_las.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-15 08:08:49.000000 lucidtech-las-9.0.0/lucidtech_las.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-15 08:08:49.000000 lucidtech-las-9.0.0/lucidtech_las.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-15 08:08:37.000000 lucidtech-las-9.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-15 08:08:49.455413 lucidtech-las-9.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-15 08:08:37.000000 lucidtech-las-9.0.0/setup.py
```

### Comparing `lucidtech-las-8.9.0/LICENSE.md` & `lucidtech-las-9.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lucidtech-las-8.9.0/PKG-INFO` & `lucidtech-las-9.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lucidtech-las
-Version: 8.9.0
+Version: 9.0.0
 Summary: Python SDK for Lucidtech AI Services
 Home-page: https://github.com/LucidtechAI/las-sdk-python
 Author: Lucidtech
 Author-email: hello@lucidtech.ai
 Maintainer: Magnus Aarskaug Rud
 Maintainer-email: magnus@lucidtech.ai
 License: Apache 2.0
```

### Comparing `lucidtech-las-8.9.0/README.md` & `lucidtech-las-9.0.0/README.md`

 * *Files identical despite different names*

### Comparing `lucidtech-las-8.9.0/las/__init__.py` & `lucidtech-las-9.0.0/las/__init__.py`

 * *Files identical despite different names*

### Comparing `lucidtech-las-8.9.0/las/client.py` & `lucidtech-las-9.0.0/las/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             d = d.astimezone()
         return d.isoformat()
     return d
 
 
 def dictstrip(d):
     """Given a dict, return the dict with keys mapping to falsey values removed."""
-    return {k: v for k, v in d.items() if v}
+    return {k: v for k, v in d.items() if v is not None}
 
 
 def _fatal_code(e):
     return 400 <= e.response.status_code < 500
 
 
 def _json_decode(response):
@@ -906,18 +906,40 @@
 
         :param field_config: Specification of the fields that the model is going to predict
         :type field_config: dict
         :param width: The number of pixels to be used for the input image width of your model
         :type width: int, optional
         :param height: The number of pixels to be used for the input image height of your model
         :type height: int, optional
-        :param preprocess_config: Specification of the processing steps prior to the prediction of an image
-        :type preprocess_config: dict
-        :param postprocess_config: Specification of the processing steps after the prediction of an image
-        :type postprocess_config: dict
+        :param preprocess_config: Preprocessing configuration for predictions.
+            {
+                'autoRotate': True | False                          (optional)
+                'maxPages': 1 - 3                                   (optional)
+                'imageQuality': 'LOW' | 'HIGH'                      (optional)
+                'pages': List with up to 3 page-indices to process  (optional)
+                'rotation': 0, 90, 180 or 270                       (optional)
+            }
+            Examples:
+            {'pages': [0, 1, 5], 'autoRotate': True}
+            {'pages': [0, 1, -1], 'rotation': 90, 'imageQuality': 'HIGH'}
+            {'maxPages': 3, 'imageQuality': 'LOW'}
+        :type preprocess_config: dict, optional
+        :param postprocess_config: Post processing configuration for predictions.
+            {
+                'strategy': 'BEST_FIRST' | 'BEST_N_PAGES',  (required)
+                'parameters': {                             (required if strategy=BEST_N_PAGES, omit otherwise)
+                    'n': int,                               (required if strategy=BEST_N_PAGES, omit otherwise)
+                    'collapse': True | False                (optional if strategy=BEST_N_PAGES, omit otherwise)
+                }
+            }
+            Examples:
+            {'strategy': 'BEST_FIRST'}
+            {'strategy': 'BEST_N_PAGES', 'parameters': {'n': 3}}
+            {'strategy': 'BEST_N_PAGES', 'parameters': {'n': 3, 'collapse': False}}
+        :type postprocess_config: dict, optional
         :param name: Name of the model
         :type name: str, optional
         :param description: Description of the model
         :type description: str, optional
         :param metadata: Dictionary that can be used to store additional information
         :type metadata: dict, optional
         :param base_model: Specify which model to use as base model. Example: \
@@ -1011,21 +1033,43 @@
         :type model_id: str, optional
         :param width: The number of pixels to be used for the input image width of your model
         :type width: int, optional
         :param height: The number of pixels to be used for the input image height of your model
         :type height: int, optional
         :param field_config: Specification of the fields that the model is going to predict
         :type field_config: dict
-        :param preprocess_config: Specification of the processing steps prior to the prediction of an image
-        :type preprocess_config: dict
-        :param postprocess_config: Specification of the processing steps after the prediction of an image
-        :type postprocess_config: dict
+        :param preprocess_config: Preprocessing configuration for predictions.
+            {
+                'autoRotate': True | False                          (optional)
+                'maxPages': 1 - 3                                   (optional)
+                'imageQuality': 'LOW' | 'HIGH'                      (optional)
+                'pages': List with up to 3 page-indices to process  (optional)
+                'rotation': 0, 90, 180 or 270                       (optional)
+            }
+            Examples:
+            {'pages': [0, 1, 5], 'autoRotate': True}
+            {'pages': [0, 1, -1], 'rotation': 90, 'imageQuality': 'HIGH'}
+            {'maxPages': 3, 'imageQuality': 'LOW'}
+        :type preprocess_config: dict, optional
+        :param postprocess_config: Post processing configuration for predictions.
+            {
+                'strategy': 'BEST_FIRST' | 'BEST_N_PAGES',  (required)
+                'parameters': {                             (required if strategy=BEST_N_PAGES, omit otherwise)
+                    'n': int,                               (required if strategy=BEST_N_PAGES, omit otherwise)
+                    'collapse': True | False                (optional if strategy=BEST_N_PAGES, omit otherwise)
+                }
+            }
+            Examples:
+            {'strategy': 'BEST_FIRST'}
+            {'strategy': 'BEST_N_PAGES', 'parameters': {'n': 3}}
+            {'strategy': 'BEST_N_PAGES', 'parameters': {'n': 3, 'collapse': False}}
+        :type postprocess_config: dict, optional
         :param metadata: Dictionary that can be used to store additional information
         :type metadata: dict, optional
-        :param training_id: Use training_id for model inference in POST /predictions
+        :param training_id: Use this training for model inference in POST /predictions
         :type training_id: str, optional
         :param name: Name of the model
         :type name: str, optional
         :param description: Description of the model
         :type description: str, optional
         :return: Model response from REST API
         :rtype: dict
@@ -1084,42 +1128,42 @@
         return self._make_request(requests.post, f'/models/{model_id}/dataBundles', body=body)
 
     def create_training(
         self,
         model_id,
         data_bundle_ids,
         *,
-        instance_type: Optional[str] = None,
         metadata: Optional[dict] = None,
+        data_scientist_assistance: Optional[bool] = None,
         **optional_args,
     ) -> Dict:
         """Requests a training, calls the POST /models/{modelId}/trainings endpoint.
 
         :param model_id: Id of the model
         :type model_id: str
         :param data_bundle_ids: Data bundle ids that will be used for training
         :type data_bundle_ids: List[str]
-        :param instance_type: The type of instance that will be used for training
-        :type instance_type: List[str]
         :param name: Name of the data bundle
         :type name: str, optional
         :param description: Description of the training
         :type description: str, optional
         :param metadata: Dictionary that can be used to store additional information
         :type metadata: dict, optional
+        :param data_scientist_assistance: Request that one of Cradl's data scientists reviews and optimizes your training
+        :type data_scientist_assistance: bool, optional
         :return: Training response from REST API
         :rtype: dict
 
         :raises: :py:class:`~las.InvalidCredentialsException`, :py:class:`~las.TooManyRequestsException`,\
  :py:class:`~las.LimitExceededException`, :py:class:`requests.exception.RequestException`
         """
 
         body = dictstrip({
             'dataBundleIds': data_bundle_ids,
-            'instanceType': instance_type,
+            'dataScientistAssistance': data_scientist_assistance,
             'metadata': metadata,
         })
         body.update(**optional_args)
         return self._make_request(requests.post, f'/models/{model_id}/trainings', body=body)
 
     def list_trainings(self, model_id, *, max_results: Optional[int] = None, next_token: Optional[str] = None) -> Dict:
         """List trainings available, calls the GET /models/{modelId}/trainings endpoint.
@@ -1150,27 +1194,34 @@
     ) -> Dict:
         """Updates a training, calls the PATCH /models/{modelId}/trainings/{trainingId} endpoint.
 
         :param model_id: Id of the model
         :type model_id: str
         :param training_id: Id of the training
         :type training_id: str
+        :param deployment_environment_id: Id of deploymentEnvironment
+        :type deployment_environment_id: str, optional
         :param name: Name of the training
         :type name: str, optional
         :param description: Description of the training
         :type description: str, optional
         :param metadata: Dictionary that can be used to store additional information
         :type metadata: dict, optional
         :return: Training response from REST API
         :rtype: dict
 
         :raises: :py:class:`~las.InvalidCredentialsException`, :py:class:`~las.TooManyRequestsException`,\
  :py:class:`~las.LimitExceededException`, :py:class:`requests.exception.RequestException`
         """
-        return self._make_request(requests.patch, f'/models/{model_id}/trainings/{training_id}', body=optional_args)
+        body = {}
+        if 'deployment_environment_id' in optional_args:
+            body['deploymentEnvironmentId'] = optional_args.pop('deployment_environment_id')
+        body.update(optional_args)
+
+        return self._make_request(requests.patch, f'/models/{model_id}/trainings/{training_id}', body=body)
 
     def list_data_bundles(
         self,
         model_id,
         *,
         max_results: Optional[int] = None,
         next_token: Optional[str] = None,
@@ -1279,71 +1330,67 @@
 
     def create_prediction(
         self,
         document_id: str,
         model_id: str,
         *,
         training_id: Optional[str] = None,
-        max_pages: Optional[int] = None,
-        auto_rotate: Optional[bool] = None,
-        image_quality: Optional[str] = None,
+        preprocess_config: Optional[dict] = None,
         postprocess_config: Optional[dict] = None,
-        rotation: Optional[int] = None,
     ) -> Dict:
         """Create a prediction on a document using specified model, calls the POST /predictions endpoint.
 
         >>> from las.client import Client
         >>> client = Client()
         >>> client.create_prediction(document_id='<document id>', model_id='<model id>')
 
         :param document_id: Id of the document to run inference and create a prediction on
         :type document_id: str
         :param model_id: Id of the model to use for predictions
         :type model_id: str
         :param training_id: Id of training to use for predictions
         :type training_id: str
-        :param max_pages: Maximum number of pages to run predictions on
-        :type max_pages: int, optional
-        :param auto_rotate: Whether to let the API try different rotations on\
-            the document when running predictions
-        :type auto_rotate: bool, optional
-        :param image_quality: Image quality for prediction "LOW|HIGH". \
-            High quality could give better result but will also take longer time
-        :type image_quality: str, optional
+        :param preprocess_config: Preprocessing configuration for prediction.
+            {
+                'autoRotate': True | False                          (optional)
+                'maxPages': 1 - 3                                   (optional)
+                'imageQuality': 'LOW' | 'HIGH'                      (optional)
+                'pages': List with up to 3 page-indices to process  (optional)
+                'rotation': 0, 90, 180 or 270                       (optional)
+            }
+            Examples:
+            {'pages': [0, 1, 5], 'autoRotate': True}
+            {'pages': [0, 1, -1], 'rotation': 90, 'imageQuality': 'HIGH'}
+            {'maxPages': 3, 'imageQuality': 'LOW'}
+        :type preprocess_config: dict, optional
         :param postprocess_config: Post processing configuration for prediction.
             {
                 'strategy': 'BEST_FIRST' | 'BEST_N_PAGES',  (required)
                 'parameters': {                             (required if strategy=BEST_N_PAGES, omit otherwise)
                     'n': int,                               (required if strategy=BEST_N_PAGES, omit otherwise)
                     'collapse': True | False                (optional if strategy=BEST_N_PAGES, omit otherwise)
                 }
             }
             Examples:
             {'strategy': 'BEST_FIRST'}
             {'strategy': 'BEST_N_PAGES', 'parameters': {'n': 3}}
             {'strategy': 'BEST_N_PAGES', 'parameters': {'n': 3, 'collapse': False}}
         :type postprocess_config: dict, optional
-        :param rotation: Number of degrees to rotate the document before making the prediction,
-            has to be 0, 90, 180 or 270
-        :type rotation: int, optional
         :return: Prediction response from REST API
         :rtype: dict
 
         :raises: :py:class:`~las.InvalidCredentialsException`, :py:class:`~las.TooManyRequestsException`,\
  :py:class:`~las.LimitExceededException`, :py:class:`requests.exception.RequestException`
         """
         body = {
             'documentId': document_id,
             'modelId': model_id,
             'trainingId': training_id,
-            'maxPages': max_pages,
-            'autoRotate': auto_rotate,
-            'imageQuality': image_quality,
+            'preprocessConfig': preprocess_config,
             'postprocessConfig': postprocess_config,
-            'rotation': rotation,
         }
         return self._make_request(requests.post, '/predictions', body=dictstrip(body))
 
     def list_predictions(
         self,
         *,
         max_results: Optional[int] = None,
@@ -1425,14 +1472,65 @@
         params = {
             'maxResults': max_results,
             'nextToken': next_token,
             'owner': owner,
         }
         return self._make_request(requests.get, '/plans', params=dictstrip(params))
 
+    def get_deployment_environment(self, deployment_environment_id: str) -> Dict:
+        """Get information about a specific DeploymentEnvironment, calls the
+        GET /deploymentEnvironments/{deploymentEnvironmentId} endpoint.
+
+        >>> from las.client import Client
+        >>> client = Client()
+        >>> client.get_deployment_environment('<deployment_environment_id>')
+
+        :param deployment_environment_id: Id of the DeploymentEnvironment
+        :type deployment_environment_id: str
+        :return: DeploymentEnvironment response from REST API
+        :rtype: dict
+
+        :raises: :py:class:`~las.InvalidCredentialsException`, :py:class:`~las.TooManyRequestsException`,\
+ :py:class:`~las.LimitExceededException`, :py:class:`requests.exception.RequestException`
+        """
+
+        return self._make_request(requests.get, f'/deploymentEnvironments/{quote(deployment_environment_id, safe="")}')
+
+    def list_deployment_environments(
+        self,
+        *,
+        owner: Optional[Queryparam] = None,
+        max_results: Optional[int] = None,
+        next_token: Optional[str] = None
+    ) -> Dict:
+        """List DeploymentEnvironments available, calls the GET /deploymentEnvironments endpoint.
+
+        >>> from las.client import Client
+        >>> client = Client()
+        >>> client.list_deployment_environments()
+
+        :param owner: Organizations to retrieve DeploymentEnvironments from
+        :type owner: Queryparam, optional
+        :param max_results: Maximum number of results to be returned
+        :type max_results: int, optional
+        :param next_token: A unique token for each page, use the returned token to retrieve the next page.
+        :type next_token: str, optional
+        :return: DeploymentEnvironments response from REST API
+        :rtype: dict
+
+        :raises: :py:class:`~las.InvalidCredentialsException`, :py:class:`~las.TooManyRequestsException`,\
+    :py:class:`~las.LimitExceededException`, :py:class:`requests.exception.RequestException`
+        """
+        params = {
+            'owner': owner,
+            'maxResults': max_results,
+            'nextToken': next_token,
+        }
+        return self._make_request(requests.get, '/deploymentEnvironments', params=dictstrip(params))
+
     def create_secret(self, data: dict, **optional_args) -> Dict:
         """Creates an secret, calls the POST /secrets endpoint.
 
         >>> from las.client import Client
         >>> client = Client()
         >>> data = {'username': '<username>', 'password': '<password>'}
         >>> client.create_secret(data, description='<description>')
```

### Comparing `lucidtech-las-8.9.0/las/credentials.py` & `lucidtech-las-9.0.0/las/credentials.py`

 * *Files identical despite different names*

### Comparing `lucidtech-las-8.9.0/lucidtech_las.egg-info/PKG-INFO` & `lucidtech-las-9.0.0/lucidtech_las.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lucidtech-las
-Version: 8.9.0
+Version: 9.0.0
 Summary: Python SDK for Lucidtech AI Services
 Home-page: https://github.com/LucidtechAI/las-sdk-python
 Author: Lucidtech
 Author-email: hello@lucidtech.ai
 Maintainer: Magnus Aarskaug Rud
 Maintainer-email: magnus@lucidtech.ai
 License: Apache 2.0
```

### Comparing `lucidtech-las-8.9.0/setup.py` & `lucidtech-las-9.0.0/setup.py`

 * *Files identical despite different names*

