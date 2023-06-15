# Comparing `tmp/django_cqrs-2.6.0.tar.gz` & `tmp/django_cqrs-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_cqrs-2.6.0.tar", max compression
+gzip compressed data, was "django_cqrs-2.7.0.tar", max compression
```

## Comparing `django_cqrs-2.6.0.tar` & `django_cqrs-2.7.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    11369 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/LICENSE
--rw-r--r--   0        0        0     9066 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/README.md
--rw-r--r--   0        0        0      196 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/__init__.py
--rw-r--r--   0        0        0     7567 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/_validation.py
--rw-r--r--   0        0        0     1842 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/admin.py
--rw-r--r--   0        0        0      289 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/apps.py
--rw-r--r--   0        0        0      728 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/constants.py
--rw-r--r--   0        0        0       60 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/controller/__init__.py
--rw-r--r--   0        0        0     3086 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/controller/consumer.py
--rw-r--r--   0        0        0      285 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/controller/producer.py
--rw-r--r--   0        0        0      698 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/correlation.py
--rw-r--r--   0        0        0     4758 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/dataclasses.py
--rw-r--r--   0        0        0     2229 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/delay.py
--rw-r--r--   0        0        0       60 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/management/__init__.py
--rw-r--r--   0        0        0       60 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/management/commands/__init__.py
--rw-r--r--   0        0        0     4084 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_bulk_dump.py
--rw-r--r--   0        0        0     3564 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_bulk_load.py
--rw-r--r--   0        0        0     5915 2023-06-01 06:50:42.188210 django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_consume.py
--rw-r--r--   0        0        0     5149 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_dead_letters.py
--rw-r--r--   0        0        0     1545 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_deleted_diff_master.py
--rw-r--r--   0        0        0     2397 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_deleted_diff_replica.py
--rw-r--r--   0        0        0     1178 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_deleted_sync_replica.py
--rw-r--r--   0        0        0     2502 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_diff_master.py
--rw-r--r--   0        0        0     1776 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_diff_replica.py
--rw-r--r--   0        0        0     2132 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_diff_sync.py
--rw-r--r--   0        0        0     4319 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_sync.py
--rw-r--r--   0        0        0      484 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/management/utils.py
--rw-r--r--   0        0        0    12661 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/managers.py
--rw-r--r--   0        0        0     5321 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/metas.py
--rw-r--r--   0        0        0    17101 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/mixins.py
--rw-r--r--   0        0        0     1392 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/registries.py
--rw-r--r--   0        0        0     5197 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/signals.py
--rw-r--r--   0        0        0     1855 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/tracker.py
--rw-r--r--   0        0        0      545 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/transport/__init__.py
--rw-r--r--   0        0        0     1003 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/transport/base.py
--rw-r--r--   0        0        0     6561 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/transport/kombu.py
--rw-r--r--   0        0        0     3250 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/transport/mixins.py
--rw-r--r--   0        0        0      316 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/transport/mock.py
--rw-r--r--   0        0        0    15323 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/transport/rabbit_mq.py
--rw-r--r--   0        0        0     1501 2023-06-01 06:50:42.192210 django_cqrs-2.6.0/dj_cqrs/utils.py
--rw-r--r--   0        0        0     3214 2023-06-01 06:52:48.383820 django_cqrs-2.6.0/pyproject.toml
--rw-r--r--   0        0        0    10343 1970-01-01 00:00:00.000000 django_cqrs-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11369 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/LICENSE
+-rw-r--r--   0        0        0     9131 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/README.md
+-rw-r--r--   0        0        0      196 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/__init__.py
+-rw-r--r--   0        0        0     7634 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/_validation.py
+-rw-r--r--   0        0        0     1842 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/admin.py
+-rw-r--r--   0        0        0      289 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/apps.py
+-rw-r--r--   0        0        0      728 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/constants.py
+-rw-r--r--   0        0        0       60 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/controller/__init__.py
+-rw-r--r--   0        0        0     3168 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/controller/consumer.py
+-rw-r--r--   0        0        0      284 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/controller/producer.py
+-rw-r--r--   0        0        0      698 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/correlation.py
+-rw-r--r--   0        0        0     4722 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/dataclasses.py
+-rw-r--r--   0        0        0     2232 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/delay.py
+-rw-r--r--   0        0        0       60 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/__init__.py
+-rw-r--r--   0        0        0       60 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/commands/__init__.py
+-rw-r--r--   0        0        0     4512 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_bulk_dump.py
+-rw-r--r--   0        0        0     3612 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_bulk_load.py
+-rw-r--r--   0        0        0     5805 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_consume.py
+-rw-r--r--   0        0        0     5196 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_dead_letters.py
+-rw-r--r--   0        0        0     1569 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_deleted_diff_master.py
+-rw-r--r--   0        0        0     2433 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_deleted_diff_replica.py
+-rw-r--r--   0        0        0     1178 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_deleted_sync_replica.py
+-rw-r--r--   0        0        0     2538 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_diff_master.py
+-rw-r--r--   0        0        0     1866 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_diff_replica.py
+-rw-r--r--   0        0        0     2156 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_diff_sync.py
+-rw-r--r--   0        0        0     4675 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_sync.py
+-rw-r--r--   0        0        0      484 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/utils.py
+-rw-r--r--   0        0        0    13276 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/managers.py
+-rw-r--r--   0        0        0     5316 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/metas.py
+-rw-r--r--   0        0        0    17146 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/mixins.py
+-rw-r--r--   0        0        0     1390 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/registries.py
+-rw-r--r--   0        0        0     5196 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/signals.py
+-rw-r--r--   0        0        0     1807 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/tracker.py
+-rw-r--r--   0        0        0      545 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/transport/__init__.py
+-rw-r--r--   0        0        0     1003 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/transport/base.py
+-rw-r--r--   0        0        0     6620 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/transport/kombu.py
+-rw-r--r--   0        0        0     3292 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/transport/mixins.py
+-rw-r--r--   0        0        0      316 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/transport/mock.py
+-rw-r--r--   0        0        0    15631 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/transport/rabbit_mq.py
+-rw-r--r--   0        0        0     1501 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/utils.py
+-rw-r--r--   0        0        0     3332 2023-06-15 08:09:10.606085 django_cqrs-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0    10408 1970-01-01 00:00:00.000000 django_cqrs-2.7.0/PKG-INFO
```

### Comparing `django_cqrs-2.6.0/LICENSE` & `django_cqrs-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.6.0/README.md` & `django_cqrs-2.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -208,16 +208,17 @@
 ```
 
 Development
 ===========
 
 1. Python >= 3.8
 2. Install dependencies `requirements/dev.txt`
-3. We use `isort` library to order and format our imports, and we check it using `flake8-isort` library (automatically on `flake8` run).  
-For convenience you may run `isort .` to order imports.
+3. We use `isort` library to order and format our imports, and `black` - to format the code. 
+We check it using `flake8-isort` and `flake8-black` libraries (automatically on `flake8` run).  
+For convenience you may run `isort . && black .` to format the code.
 
 
 Testing
 =======
 
 Unit testing
 ------
```

### Comparing `django_cqrs-2.6.0/dj_cqrs/_validation.py` & `django_cqrs-2.7.0/dj_cqrs/_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,17 +72,18 @@
     _validate_master_message_ttl(master_settings)
     _validate_master_correlation_func(master_settings)
     _validate_master_meta_func(master_settings)
 
 
 def _validate_master_auto_update_fields(master_settings):
     if 'CQRS_AUTO_UPDATE_FIELDS' in master_settings:
-        assert isinstance(master_settings['CQRS_AUTO_UPDATE_FIELDS'], bool), (
-            'CQRS master CQRS_AUTO_UPDATE_FIELDS must be bool.'
-        )
+        assert isinstance(
+            master_settings['CQRS_AUTO_UPDATE_FIELDS'],
+            bool,
+        ), 'CQRS master CQRS_AUTO_UPDATE_FIELDS must be bool.'
     else:
         master_settings['CQRS_AUTO_UPDATE_FIELDS'] = DEFAULT_MASTER_AUTO_UPDATE_FIELDS
 
 
 def _validate_master_message_ttl(master_settings):
     if 'CQRS_MESSAGE_TTL' in master_settings:
         min_message_ttl = 1
@@ -90,15 +91,16 @@
         if (message_ttl is not None) and (
             not isinstance(message_ttl, int) or message_ttl < min_message_ttl
         ):
             # No error is raised for backward compatibility
             # TODO: raise error in 2.0.0
             logger.warning(
                 'Settings CQRS_MESSAGE_TTL=%s is invalid, using default %s.',
-                message_ttl, DEFAULT_MASTER_MESSAGE_TTL,
+                message_ttl,
+                DEFAULT_MASTER_MESSAGE_TTL,
             )
             master_settings['CQRS_MESSAGE_TTL'] = DEFAULT_MASTER_MESSAGE_TTL
     else:
         master_settings['CQRS_MESSAGE_TTL'] = DEFAULT_MASTER_MESSAGE_TTL
 
 
 def _validate_master_correlation_func(master_settings):
@@ -163,15 +165,16 @@
         if (max_retries is not None) and (
             not isinstance(max_retries, int) or max_retries < min_retries
         ):
             # No error is raised for backward compatibility
             # TODO: raise error in 2.0.0
             logger.warning(
                 'Replica setting CQRS_MAX_RETRIES=%s is invalid, using default %s.',
-                max_retries, DEFAULT_REPLICA_MAX_RETRIES,
+                max_retries,
+                DEFAULT_REPLICA_MAX_RETRIES,
             )
             replica_settings['CQRS_MAX_RETRIES'] = DEFAULT_REPLICA_MAX_RETRIES
     else:
         replica_settings['CQRS_MAX_RETRIES'] = DEFAULT_REPLICA_MAX_RETRIES
 
 
 def _validate_replica_retry_delay(replica_settings):
@@ -180,27 +183,29 @@
     if 'CQRS_RETRY_DELAY' not in replica_settings:
         replica_settings['CQRS_RETRY_DELAY'] = DEFAULT_REPLICA_RETRY_DELAY
     elif not isinstance(retry_delay, int) or retry_delay < min_retry_delay:
         # No error is raised for backward compatibility
         # TODO: raise error in 2.0.0
         logger.warning(
             'Replica setting CQRS_RETRY_DELAY=%s is invalid, using default %s.',
-            retry_delay, DEFAULT_REPLICA_RETRY_DELAY,
+            retry_delay,
+            DEFAULT_REPLICA_RETRY_DELAY,
         )
         replica_settings['CQRS_RETRY_DELAY'] = DEFAULT_REPLICA_RETRY_DELAY
 
 
 def _validate_replica_delay_queue_max_size(replica_settings):
     min_qsize = 0
     max_qsize = replica_settings.get('delay_queue_max_size')
     if 'delay_queue_max_size' not in replica_settings:
         max_qsize = DEFAULT_REPLICA_DELAY_QUEUE_MAX_SIZE
     elif (max_qsize is not None) and (not isinstance(max_qsize, int) or max_qsize <= min_qsize):
         # No error is raised for backward compatibility
         # TODO: raise error in 2.0.0
         logger.warning(
             'Settings delay_queue_max_size=%s is invalid, using default %s.',
-            max_qsize, DEFAULT_REPLICA_DELAY_QUEUE_MAX_SIZE,
+            max_qsize,
+            DEFAULT_REPLICA_DELAY_QUEUE_MAX_SIZE,
         )
         max_qsize = DEFAULT_REPLICA_DELAY_QUEUE_MAX_SIZE
 
     replica_settings['delay_queue_max_size'] = max_qsize
```

### Comparing `django_cqrs-2.6.0/dj_cqrs/admin.py` & `django_cqrs-2.7.0/dj_cqrs/admin.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.6.0/dj_cqrs/constants.py` & `django_cqrs-2.7.0/dj_cqrs/constants.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.6.0/dj_cqrs/controller/consumer.py` & `django_cqrs-2.7.0/dj_cqrs/controller/consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from dj_cqrs.registries import ReplicaRegistry
 
 
 logger = logging.getLogger('django-cqrs')
 
 
 def consume(payload):
-    """ Consumer controller.
+    """Consumer controller.
 
     :param dj_cqrs.dataclasses.TransportPayload payload: Consumed payload from master service.
     """
     payload = copy.deepcopy(payload)
     return route_signal_to_replica_model(
         payload.signal_type,
         payload.cqrs_id,
@@ -27,17 +27,22 @@
         previous_data=payload.previous_data,
         meta=payload.meta,
         queue=payload.queue,
     )
 
 
 def route_signal_to_replica_model(
-    signal_type, cqrs_id, instance_data, previous_data=None, meta=None, queue=None,
+    signal_type,
+    cqrs_id,
+    instance_data,
+    previous_data=None,
+    meta=None,
+    queue=None,
 ):
-    """ Routes signal to model method to create/update/delete replica instance.
+    """Routes signal to model method to create/update/delete replica instance.
 
     :param dj_cqrs.constants.SignalType signal_type: Consumed signal type.
     :param str cqrs_id: Replica model CQRS unique identifier.
     :param dict instance_data: Master model data.
     :param dict or None previous_data: Previous model data for changed tracked fields, if exists.
     :param dict or None meta: Payload metadata, if exists.
     :param str or None queue: Synced queue.
@@ -81,10 +86,14 @@
     except Error as e:
         pk_name = getattr(model_cls._meta.pk, 'name', 'id')
         pk_value = instance_data.get(pk_name)
         cqrs_revision = instance_data.get('cqrs_revision')
 
         logger.error(
             '{0}\nCQRS {1} error: pk = {2}, cqrs_revision = {3} ({4}).'.format(
-                str(e), signal_type, pk_value, cqrs_revision, model_cls.CQRS_ID,
+                str(e),
+                signal_type,
+                pk_value,
+                cqrs_revision,
+                model_cls.CQRS_ID,
             ),
         )
```

### Comparing `django_cqrs-2.6.0/dj_cqrs/correlation.py` & `django_cqrs-2.7.0/dj_cqrs/correlation.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.6.0/dj_cqrs/dataclasses.py` & `django_cqrs-2.7.0/dj_cqrs/dataclasses.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 
     @property
     def retries(self):
         return self.__retries
 
     @retries.setter
     def retries(self, value):
-        assert value >= 0, "Payload retries field should be 0 or positive integer."
+        assert value >= 0, 'Payload retries field should be 0 or positive integer.'
         self.__retries = value
 
     def to_dict(self) -> dict:
         """Return the payload as a dictionary.
 
         Returns:
             (dict): This payload.
@@ -153,11 +153,8 @@
 
     def is_expired(self):
         """Checks if this payload is expired.
 
         Returns:
             (bool): True if payload is expired, False otherwise.
         """
-        return (
-            self.__expires is not None
-            and self.__expires <= timezone.now()
-        )
+        return self.__expires is not None and self.__expires <= timezone.now()
```

### Comparing `django_cqrs-2.6.0/dj_cqrs/delay.py` & `django_cqrs-2.7.0/dj_cqrs/delay.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 class DelayQueue:
     """Queue for delay messages."""
 
     def __init__(self, max_size=None):
         if max_size is not None:
-            assert max_size > 0, "Delay queue max_size should be positive integer."
+            assert max_size > 0, 'Delay queue max_size should be positive integer.'
 
         self._max_size = max_size
         self._queue = PriorityQueue()
 
     def get(self):
         """
         :rtype: DelayMessage
@@ -59,23 +59,22 @@
         """Adds message to queue.
 
         :param delay_message: DelayMessage instance.
         :type delay_message: DelayMessage
         """
         assert isinstance(delay_message, DelayMessage)
         if self.full():
-            raise Full("Delay queue is full")
+            raise Full('Delay queue is full')
 
-        self._queue.put((
-            delay_message.eta.timestamp(),
-            delay_message.delivery_tag,
-            delay_message,
-        ))
+        self._queue.put(
+            (
+                delay_message.eta.timestamp(),
+                delay_message.delivery_tag,
+                delay_message,
+            ),
+        )
 
     def qsize(self):
         return self._queue.qsize()
 
     def full(self):
-        return (
-            self._max_size is not None
-            and self.qsize() >= self._max_size
-        )
+        return self._max_size is not None and self.qsize() >= self._max_size
```

### Comparing `django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_bulk_dump.py` & `django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_bulk_dump.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,38 +13,43 @@
 
 
 class Command(BaseCommand):
     help = 'Bulk dump of a CQRS model from master service.'
 
     def add_arguments(self, parser):
         parser.add_argument(
-            '--cqrs-id', '-c',
+            '--cqrs-id',
+            '-c',
             help='CQRS_ID of the master model',
             type=str,
             required=True,
         )
         parser.add_argument(
-            '--output', '-o',
+            '--output',
+            '-o',
             help='Output file for dumping (- for writing to stdout)',
             type=str,
             default=None,
         )
         parser.add_argument(
-            '--batch', '-b',
+            '--batch',
+            '-b',
             help='Batch size',
             type=int,
             default=10000,
         )
         parser.add_argument(
-            '--progress', '-p',
+            '--progress',
+            '-p',
             help='Display progress',
             action='store_true',
         )
         parser.add_argument(
-            '--force', '-f',
+            '--force',
+            '-f',
             help='Override output file',
             action='store_true',
         )
 
     def handle(self, *args, **options):
         model = self._get_model(options)
         out_fname = self._get_output_filename(options)
@@ -59,44 +64,59 @@
 
             if progress:
                 print(
                     'Processing {0} records with batch size {1}'.format(db_count, batch_size),
                     file=sys.stderr,
                 )
             for qs in batch_qs(
-                    model.relate_cqrs_serialization(model._default_manager.order_by().all()),
-                    batch_size=batch_size,
+                model.relate_cqrs_serialization(model._default_manager.order_by().all()),
+                batch_size=batch_size,
             ):
                 ts = time.time()
                 cs = counter
                 for instance in qs:
                     counter += 1
                     try:
                         f.write(
                             '\n' + ujson.dumps(instance.to_cqrs_dict()),
                         )
                         success_counter += 1
                     except Exception as e:
-                        print('\nDump record failed for pk={0}: {1}: {2}'.format(
-                            instance.pk, type(e).__name__, str(e),
-                        ), file=sys.stderr)
+                        print(
+                            '\nDump record failed for pk={0}: {1}: {2}'.format(
+                                instance.pk,
+                                type(e).__name__,
+                                str(e),
+                            ),
+                            file=sys.stderr,
+                        )
                 if progress:
                     rate = (counter - cs) / (time.time() - ts)
                     percent = 100 * counter / db_count
                     eta = datetime.timedelta(seconds=int((db_count - counter) / rate))
                     sys.stderr.write(
                         '\r{0} of {1} processed - {2}% with '
                         'rate {3:.1f} rps, to go {4} ...{5:20}'.format(
-                            counter, db_count, int(percent), rate, str(eta), ' ',
-                        ))
+                            counter,
+                            db_count,
+                            int(percent),
+                            rate,
+                            str(eta),
+                            ' ',
+                        ),
+                    )
                     sys.stderr.flush()
 
-        print('Done!\n{0} instance(s) saved.\n{1} instance(s) processed.'.format(
-            success_counter, counter,
-        ), file=sys.stderr)
+        print(
+            'Done!\n{0} instance(s) saved.\n{1} instance(s) processed.'.format(
+                success_counter,
+                counter,
+            ),
+            file=sys.stderr,
+        )
 
     @staticmethod
     def _get_model(options):
         cqrs_id = options['cqrs_id']
         model = MasterRegistry.get_model_by_cqrs_id(cqrs_id)
 
         if not model:
```

### Comparing `django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_bulk_load.py` & `django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_bulk_load.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,27 +11,31 @@
 
 
 class Command(BaseCommand):
     help = 'Bulk load of a CQRS model to a replica service.'
 
     def add_arguments(self, parser):
         parser.add_argument(
-            '--input', '-i',
+            '--input',
+            '-i',
             help='Input file for loading (- for reading from stdin)',
-            type=str, required=True,
+            type=str,
+            required=True,
         )
         parser.add_argument(
-            '--clear', '-c',
+            '--clear',
+            '-c',
             help='Delete existing models',
             type=bool,
             required=False,
             default=False,
         )
         parser.add_argument(
-            '--batch', '-b',
+            '--batch',
+            '-b',
             help='Batch size',
             type=int,
             default=10000,
         )
 
     def handle(self, *args, **options):
         batch_size = self._get_batch_size(options)
@@ -54,15 +58,15 @@
                 raise CommandError('Wrong CQRS ID: {0}!'.format(cqrs_id))
 
             with transaction.atomic():
                 if options['clear']:
                     try:
                         model._default_manager.all().delete()
                     except DatabaseError:
-                        raise CommandError("Delete operation fails!")
+                        raise CommandError('Delete operation fails!')
 
             self._process(f, model, batch_size)
 
     @classmethod
     def _process(cls, stream, model, batch_size):
         success_counter = 0
         line_number = 2
```

### Comparing `django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_consume.py` & `django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_consume.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,40 +13,41 @@
 
 
 logger = logging.getLogger('django-cqrs')
 
 
 def consume(**kwargs):
     import django
+
     django.setup()
 
     from dj_cqrs.transport import current_transport
+
     try:
         current_transport.consume(**kwargs)
     except KeyboardInterrupt:
         pass
 
 
 def _display_path(path):
     try:
         return f'"{path.relative_to(Path.cwd())}"'
     except ValueError:  # pragma: no cover
         return f'"{path}"'
 
 
 class WorkersManager:
-
     def __init__(
-            self,
-            consume_kwargs,
-            workers=1,
-            reload=False,
-            ignore_paths=None,
-            sigint_timeout=5,
-            sigkill_timeout=1,
+        self,
+        consume_kwargs,
+        workers=1,
+        reload=False,
+        ignore_paths=None,
+        sigint_timeout=5,
+        sigkill_timeout=1,
     ):
         self.pool = []
         self.workers = workers
         self.reload = reload
         self.consume_kwargs = consume_kwargs
         self.stop_event = threading.Event()
         self.sigint_timeout = sigint_timeout
@@ -133,18 +134,15 @@
             nargs='*',
             type=str,
             help='Choose model(s) by CQRS_ID for consuming',
         )
         parser.add_argument(
             '--reload',
             '-r',
-            help=(
-                'Enable reload signal SIGHUP and autoreload '
-                'on file changes'
-            ),
+            help=('Enable reload signal SIGHUP and autoreload ' 'on file changes'),
             action='store_true',
             default=False,
         )
         parser.add_argument(
             '--ignore-paths',
             nargs='?',
             type=str,
@@ -166,25 +164,24 @@
             nargs='?',
             type=int,
             default=1,
             help='How long to wait for the sigkill timeout before issuing a timeout exception.',
         )
 
     def handle(
-            self,
-            *args,
-            workers=1,
-            cqrs_id=None,
-            reload=False,
-            ignore_paths=None,
-            sigint_timeout=5,
-            sigkill_timeout=1,
-            **options,
+        self,
+        *args,
+        workers=1,
+        cqrs_id=None,
+        reload=False,
+        ignore_paths=None,
+        sigint_timeout=5,
+        sigkill_timeout=1,
+        **options,
     ):
-
         paths_to_ignore = None
         if ignore_paths:
             paths_to_ignore = [Path(p).resolve() for p in ignore_paths.split(',')]
 
         workers_manager = WorkersManager(
             workers=workers,
             consume_kwargs=self.get_consume_kwargs(cqrs_id),
```

### Comparing `django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_dead_letters.py` & `django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_dead_letters.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from dj_cqrs.registries import ReplicaRegistry
 from dj_cqrs.transport import current_transport
 from dj_cqrs.transport.rabbit_mq import RabbitMQTransport
 from dj_cqrs.utils import get_message_expiration_dt
 
 
 class RabbitMQTransportService(RabbitMQTransport):
-
     @classmethod
     def get_consumer_settings(cls):
         return cls._get_consumer_settings()
 
     @classmethod
     def get_common_settings(cls):
         return cls._get_common_settings()
@@ -46,15 +45,16 @@
 
     def handle(self, *args, **options):
         self.check_transport()
         channel, connection = self.init_broker()
 
         queue_name, dead_letter_queue_name, *_ = RabbitMQTransportService.get_consumer_settings()
         dead_letters_queue = RabbitMQTransportService.declare_queue(
-            channel, dead_letter_queue_name,
+            channel,
+            dead_letter_queue_name,
         )
         dead_letters_count = dead_letters_queue.method.message_count
         consumer_generator = channel.consume(
             queue=dead_letter_queue_name,
             auto_ack=False,
             exclusive=False,
         )
@@ -68,20 +68,23 @@
             self.handle_purge(channel, dead_letter_queue_name, dead_letters_count)
 
         if not connection.is_closed:
             connection.close()
 
     def check_transport(self):
         if not issubclass(current_transport, RabbitMQTransport):
-            raise CommandError("Dead letters commands available only for RabbitMQTransport.")
+            raise CommandError('Dead letters commands available only for RabbitMQTransport.')
 
     def init_broker(self):
         host, port, creds, exchange = RabbitMQTransportService.get_common_settings()
         connection, channel = RabbitMQTransportService.create_connection(
-            host, port, creds, exchange,
+            host,
+            port,
+            creds,
+            exchange,
         )
 
         queue_name, dead_letter_queue_name, *_ = RabbitMQTransportService.get_consumer_settings()
         RabbitMQTransportService.declare_queue(channel, queue_name)
         RabbitMQTransportService.declare_queue(channel, dead_letter_queue_name)
         for cqrs_id, _ in ReplicaRegistry.models.items():
             channel.queue_bind(exchange=exchange, queue=queue_name, routing_key=cqrs_id)
@@ -92,17 +95,17 @@
                 queue=queue_name,
                 routing_key='cqrs.{0}.{1}'.format(queue_name, cqrs_id),
             )
 
         return channel, connection
 
     def handle_retry(self, channel, consumer_generator, dead_letters_count):
-        self.stdout.write("Total dead letters: {0}".format(dead_letters_count))
+        self.stdout.write('Total dead letters: {0}'.format(dead_letters_count))
         for i in range(1, dead_letters_count + 1):
-            self.stdout.write("Retrying: {0}/{1}".format(i, dead_letters_count))
+            self.stdout.write('Retrying: {0}/{1}'.format(i, dead_letters_count))
             method_frame, properties, body = next(consumer_generator)
 
             dct = ujson.loads(body)
             dct['retries'] = 0
             if dct.get('expires'):
                 # Message could expire already
                 expires = get_message_expiration_dt(DEFAULT_MASTER_MESSAGE_TTL)
@@ -118,11 +121,11 @@
 
     def handle_dump(self, consumer_generator, dead_letters_count):
         for _ in range(1, dead_letters_count + 1):
             *_, body = next(consumer_generator)
             self.stdout.write(body.decode('utf-8'))
 
     def handle_purge(self, channel, dead_letter_queue_name, dead_letter_count):
-        self.stdout.write("Total dead letters: {0}".format(dead_letter_count))
+        self.stdout.write('Total dead letters: {0}'.format(dead_letter_count))
         if dead_letter_count > 0:
             channel.queue_purge(dead_letter_queue_name)
-            self.stdout.write("Purged")
+            self.stdout.write('Purged')
```

### Comparing `django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_deleted_diff_master.py` & `django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_deleted_diff_master.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,16 @@
             for package_line in f:
                 master_data = self.deserialize_in(package_line)
 
                 exist_pks = set(
                     model.objects.filter(
                         pk__in=master_data,
                     ).values_list(
-                        'pk', flat=True,
+                        'pk',
+                        flat=True,
                     ),
                 )
                 diff_ids = list(master_data - exist_pks)
                 if diff_ids:
                     self.stdout.write(self.serialize_out(diff_ids))
                     self.stderr.write('PK to delete: {0}'.format(str(diff_ids)))
```

### Comparing `django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_deleted_diff_replica.py` & `django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_deleted_diff_replica.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,27 +14,30 @@
 
     @classmethod
     def serialize_package(cls, package):
         return ujson.dumps(package)
 
     def add_arguments(self, parser):
         parser.add_argument(
-            '--cqrs-id', '-cid',
+            '--cqrs-id',
+            '-cid',
             help='CQRS_ID of the replica model',
             type=str,
             required=True,
         )
         parser.add_argument(
-            '--filter', '-f',
+            '--filter',
+            '-f',
             help='Filter kwargs',
             type=str,
             default=None,
         )
         parser.add_argument(
-            '--batch', '-b',
+            '--batch',
+            '-b',
             help='Batch size',
             type=int,
             default=10000,
         )
 
     def handle(self, *args, **options):
         model = self._get_model(options)
```

### Comparing `django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_deleted_sync_replica.py` & `django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_deleted_sync_replica.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_diff_master.py` & `django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_diff_master.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,27 +14,30 @@
 
     @classmethod
     def serialize_package(cls, package):
         return ujson.dumps(package)
 
     def add_arguments(self, parser):
         parser.add_argument(
-            '--cqrs-id', '-cid',
+            '--cqrs-id',
+            '-cid',
             help='CQRS_ID of the master model',
             type=str,
             required=True,
         )
         parser.add_argument(
-            '--filter', '-f',
+            '--filter',
+            '-f',
             help='Filter kwargs',
             type=str,
             default=None,
         )
         parser.add_argument(
-            '--batch', '-b',
+            '--batch',
+            '-b',
             help='Batch size',
             type=int,
             default=10000,
         )
 
     def handle(self, *args, **options):
         model = self._get_model(options)
```

### Comparing `django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_diff_replica.py` & `django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_diff_replica.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,21 @@
             first_line = f.readline()
             model = self._get_model(first_line)
             self.stdout.write('{0},{1}'.format(first_line.strip(), settings.CQRS.get('queue')))
 
             for package_line in f:
                 master_data = self.deserialize_in(package_line)
 
-                qs = model._default_manager.filter(
-                    pk__in=master_data.keys(),
-                ).order_by().only('pk', 'cqrs_revision')
+                qs = (
+                    model._default_manager.filter(
+                        pk__in=master_data.keys(),
+                    )
+                    .order_by()
+                    .only('pk', 'cqrs_revision')
+                )
                 replica_data = {instance.pk: instance.cqrs_revision for instance in qs}
 
                 diff_ids = set()
                 for pk, cqrs_revision in master_data.items():
                     if replica_data.get(pk, -1) != cqrs_revision:
                         diff_ids.add(pk)
```

### Comparing `django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_diff_sync.py` & `django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_diff_sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,21 +14,23 @@
 
 
 class Command(BaseCommand):
     help = 'Diff synchronizer from CQRS replica stream.'
 
     def add_arguments(self, parser):
         parser.add_argument(
-            '--batch', '-b',
+            '--batch',
+            '-b',
             help='Batch size',
             type=int,
             default=DEFAULT_BATCH,
         )
         parser.add_argument(
-            '--progress', '-p',
+            '--progress',
+            '-p',
             help='Display progress',
             action='store_true',
         )
 
     def handle(self, *args, **options):
         progress = self._get_progress(options)
         batch_size = self._get_batch_size(options)
```

### Comparing `django_cqrs-2.6.0/dj_cqrs/management/commands/cqrs_sync.py` & `django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,39 +18,44 @@
 
 
 class Command(BaseCommand):
     help = 'Filter synchronization of certain CQRS model rows over transport to replicas.'
 
     def add_arguments(self, parser):
         parser.add_argument(
-            '--cqrs-id', '-cid',
+            '--cqrs-id',
+            '-cid',
             help='CQRS_ID of the master model',
             type=str,
             required=True,
         )
         parser.add_argument(
-            '--filter', '-f',
+            '--filter',
+            '-f',
             help='Filter kwargs',
             type=str,
             default=None,
         )
         parser.add_argument(
-            '--queue', '-q',
+            '--queue',
+            '-q',
             help='Name of the specific replica queue',
             type=str,
             default=None,
         )
         parser.add_argument(
-            '--batch', '-b',
+            '--batch',
+            '-b',
             help='Batch size',
             type=int,
             default=DEFAULT_BATCH,
         )
         parser.add_argument(
-            '--progress', '-p',
+            '--progress',
+            '-p',
             help='Display progress',
             action='store_true',
         )
 
     def handle(self, *args, **options):
         model = self._get_model(options)
         progress = self._get_progress(options)
@@ -76,33 +81,46 @@
 
             for instance in qs_:
                 counter += 1
                 try:
                     instance.cqrs_sync(queue=options['queue'])
                     success_counter += 1
                 except Exception as e:
-                    print('\nSync record failed for pk={0}: {1}: {2}'.format(
-                        instance.pk, type(e).__name__, str(e),
-                    ))
+                    print(
+                        '\nSync record failed for pk={0}: {1}: {2}'.format(
+                            instance.pk,
+                            type(e).__name__,
+                            str(e),
+                        ),
+                    )
                     close_old_connections()
 
             if progress:
                 rate = (counter - cs) / (time.time() - ts)
                 percent = 100 * counter / db_count
                 eta = datetime.timedelta(seconds=int((db_count - counter) / rate))
                 sys.stdout.write(
                     '\r{0} of {1} processed - {2}% with '
                     'rate {3:.1f} rps, to go {4} ...{5:20}'.format(
-                        counter, db_count, int(percent), rate, str(eta), ' ',
-                    ))
+                        counter,
+                        db_count,
+                        int(percent),
+                        rate,
+                        str(eta),
+                        ' ',
+                    ),
+                )
                 sys.stdout.flush()
 
-        print('Done!\n{0} instance(s) synced.\n{1} instance(s) processed.'.format(
-            success_counter, counter,
-        ))
+        print(
+            'Done!\n{0} instance(s) synced.\n{1} instance(s) processed.'.format(
+                success_counter,
+                counter,
+            ),
+        )
 
     @staticmethod
     def _prepare_qs(model, options):
         qs = model._default_manager.none()
         if options['filter']:
             try:
                 kwargs = ujson.loads(options['filter'])
```

### Comparing `django_cqrs-2.6.0/dj_cqrs/managers.py` & `django_cqrs-2.7.0/dj_cqrs/managers.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
         if objs:
             self.model.call_post_bulk_create(objs, using=self.db)
 
         return objs
 
     def bulk_update(self, queryset, **kwargs):
-        """ Custom update method to support sending of update signals.
+        """Custom update method to support sending of update signals.
 
         Args:
             queryset (django.db.models.QuerySet): Django Queryset (f.e. filter).
             kwargs (dict): Update kwargs.
         """
         prev_data_mapper = {}
         collect_prev_data = hasattr(self.model, FIELDS_TRACKER_FIELD_NAME)
@@ -58,15 +58,17 @@
                     return
 
                 for obj in objs:
                     prev_data_mapper[obj.pk] = getattr(obj, FIELDS_TRACKER_FIELD_NAME).current()
 
             current_dt = timezone.now()
             result = queryset.update(
-                cqrs_revision=F('cqrs_revision') + 1, cqrs_updated=current_dt, **kwargs,
+                cqrs_revision=F('cqrs_revision') + 1,
+                cqrs_updated=current_dt,
+                **kwargs,
             )
 
             objs = list_all()
             if collect_prev_data:
                 for obj in objs:
                     setattr(obj, TRACKED_FIELDS_ATTR_NAME, prev_data_mapper.get(obj.pk))
 
@@ -79,15 +81,15 @@
     def save_instance(
         self,
         master_data: dict,
         previous_data: dict = None,
         sync: bool = False,
         meta: dict = None,
     ):
-        """ This method saves (creates or updates) model instance from CQRS master instance data.
+        """This method saves (creates or updates) model instance from CQRS master instance data.
 
         Args:
             master_data (dict): CQRS master instance data.
             previous_data (dict): Previous values for tracked fields.
             sync (bool): Sync package flag.
             meta (dict): Payload metadata, if exists.
 
@@ -126,15 +128,15 @@
     def create_instance(
         self,
         mapped_data: dict,
         previous_data: dict = None,
         sync: bool = False,
         meta: dict = None,
     ):
-        """ This method creates model instance from mapped CQRS master instance data.
+        """This method creates model instance from mapped CQRS master instance data.
 
         Args:
             mapped_data (dict): Mapped CQRS master instance data.
             previous_data (dict): Previous values for tracked fields.
             sync (bool): Sync package flag.
             meta (dict): Payload metadata, if exists.
 
@@ -148,27 +150,29 @@
         try:
             return self.model.cqrs_create(sync, mapped_data, **f_kw)
         except (Error, ValidationError) as e:
             pk_value = mapped_data[self._get_model_pk_name()]
 
             logger.error(
                 '{0}\nCQRS create error: pk = {1} ({2}).'.format(
-                    str(e), pk_value, self.model.CQRS_ID,
+                    str(e),
+                    pk_value,
+                    self.model.CQRS_ID,
                 ),
             )
 
     def update_instance(
         self,
         instance,
         mapped_data: dict,
         previous_data: dict = None,
         sync: bool = False,
         meta: dict = None,
     ):
-        """ This method updates model instance from mapped CQRS master instance data.
+        """This method updates model instance from mapped CQRS master instance data.
 
         Args:
             instance (django.db.models.Model): ReplicaMixin model instance.
             mapped_data (dict): Mapped CQRS master instance data.
             previous_data (dict): Previous values for tracked fields.
             sync (bool): Sync package flag.
             meta (dict): Payload metadata, if exists.
@@ -182,68 +186,88 @@
 
         if sync:
             if existing_cqrs_revision > current_cqrs_revision:
                 w_tpl = (
                     'CQRS revision downgrade on sync: pk = {0}, '
                     'cqrs_revision = new {1} / existing {2} ({3}).'
                 )
-                logger.warning(w_tpl.format(
-                    pk_value, current_cqrs_revision, existing_cqrs_revision, self.model.CQRS_ID,
-                ))
+                logger.warning(
+                    w_tpl.format(
+                        pk_value,
+                        current_cqrs_revision,
+                        existing_cqrs_revision,
+                        self.model.CQRS_ID,
+                    ),
+                )
 
         else:
             if existing_cqrs_revision > current_cqrs_revision:
                 e_tpl = (
                     'Wrong CQRS sync order: pk = {0}, '
                     'cqrs_revision = new {1} / existing {2} ({3}).'
                 )
-                logger.error(e_tpl.format(
-                    pk_value, current_cqrs_revision, existing_cqrs_revision, self.model.CQRS_ID,
-                ))
+                logger.error(
+                    e_tpl.format(
+                        pk_value,
+                        current_cqrs_revision,
+                        existing_cqrs_revision,
+                        self.model.CQRS_ID,
+                    ),
+                )
                 return instance
 
             if existing_cqrs_revision == current_cqrs_revision:
                 logger.error(
                     'Received duplicate CQRS data: pk = {0}, cqrs_revision = {1} ({2}).'.format(
-                        pk_value, current_cqrs_revision, self.model.CQRS_ID,
+                        pk_value,
+                        current_cqrs_revision,
+                        self.model.CQRS_ID,
                     ),
                 )
                 if current_cqrs_revision == 0:
                     logger.warning(
                         'CQRS potential creation race condition: pk = {0} ({1}).'.format(
-                            pk_value, self.model.CQRS_ID,
+                            pk_value,
+                            self.model.CQRS_ID,
                         ),
                     )
 
                 return instance
 
             if current_cqrs_revision != instance.cqrs_revision + 1:
                 w_tpl = (
                     'Lost or filtered out {0} CQRS packages: pk = {1}, cqrs_revision = {2} ({3})'
                 )
-                logger.warning(w_tpl.format(
-                    current_cqrs_revision - instance.cqrs_revision - 1,
-                    pk_value, current_cqrs_revision, self.model.CQRS_ID,
-                ))
+                logger.warning(
+                    w_tpl.format(
+                        current_cqrs_revision - instance.cqrs_revision - 1,
+                        pk_value,
+                        current_cqrs_revision,
+                        self.model.CQRS_ID,
+                    ),
+                )
 
         f_kw = {'previous_data': previous_data}
         if self.model.CQRS_META:
             f_kw['meta'] = meta
 
         try:
             return instance.cqrs_update(sync, mapped_data, **f_kw)
         except (Error, ValidationError) as e:
             logger.error(
                 '{0}\nCQRS update error: pk = {1}, cqrs_revision = {2} ({3}).'.format(
-                    str(e), pk_value, current_cqrs_revision, self.model.CQRS_ID,
+                    str(e),
+                    pk_value,
+                    current_cqrs_revision,
+                    self.model.CQRS_ID,
                 ),
             )
 
     def delete_instance(self, master_data: dict) -> bool:
-        """ This method deletes model instance from mapped CQRS master instance data.
+        """This method deletes model instance from mapped CQRS master instance data.
 
         Args:
             master_data (dict): CQRS master instance data.
 
         Returns:
             Flag, if delete operation is successful (even if nothing was deleted).
         """
@@ -254,15 +278,17 @@
             pk_value = mapped_data[pk_name]
             try:
                 self.model._default_manager.filter(**{pk_name: pk_value}).delete()
                 return True
             except Error as e:
                 logger.error(
                     '{0}\nCQRS delete error: pk = {1} ({2}).'.format(
-                        str(e), pk_value, self.model.CQRS_ID,
+                        str(e),
+                        pk_value,
+                        self.model.CQRS_ID,
                     ),
                 )
 
         return False
 
     def _map_previous_data(self, previous_data):
         if self.model.CQRS_MAPPING is None:
@@ -304,35 +330,34 @@
 
         mapped_data = {
             'cqrs_revision': master_data['cqrs_revision'],
             'cqrs_updated': master_data['cqrs_updated'],
         }
         for master_name, replica_name in self.model.CQRS_MAPPING.items():
             if master_name not in master_data:
-                logger.error('Bad master-replica mapping for {0} ({1}).'.format(
-                    master_name, self.model.CQRS_ID,
-                ))
+                logger.error(
+                    'Bad master-replica mapping for {0} ({1}).'.format(
+                        master_name,
+                        self.model.CQRS_ID,
+                    ),
+                )
                 return
 
             mapped_data[replica_name] = master_data[master_name]
         return mapped_data
 
     def _remove_excessive_data(self, data):
         opts = self.model._meta
-        possible_field_names = {
-            f.name for f in opts.fields
-        }
+        possible_field_names = {f.name for f in opts.fields}
         return {k: v for k, v in data.items() if k in possible_field_names}
 
     def _all_required_fields_are_filled(self, mapped_data):
         opts = self.model._meta
 
-        required_field_names = {
-            f.name for f in opts.fields if not f.null
-        }
+        required_field_names = {f.name for f in opts.fields if not f.null}
         if not (required_field_names - set(mapped_data.keys())):
             return True
 
         logger.error(
             'Not all required CQRS fields are provided in data ({0}).'.format(self.model.CQRS_ID),
         )
         return False
```

### Comparing `django_cqrs-2.6.0/dj_cqrs/metas.py` & `django_cqrs-2.7.0/dj_cqrs/metas.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,33 +46,33 @@
                 model_cls,
                 tracked_fields,
                 'CQRS_TRACKED_FIELDS',
             )
             _MetaUtils._check_unexisting_names(model_cls, tracked_fields, 'CQRS_TRACKED_FIELDS')
             return
 
-        e = "Model {0}: Invalid configuration for CQRS_TRACKED_FIELDS".format(model_cls.__name__)
+        e = 'Model {0}: Invalid configuration for CQRS_TRACKED_FIELDS'.format(model_cls.__name__)
         assert isinstance(tracked_fields, str) and tracked_fields == ALL_BASIC_FIELDS, e
 
     @staticmethod
     def _check_correct_configuration(model_cls):
-        """ Check that model has correct CQRS configuration.
+        """Check that model has correct CQRS configuration.
 
         :param dj_cqrs.mixins.MasterMixin model_cls: CQRS Master Model.
         :raises: AssertionError
         """
         if model_cls.CQRS_FIELDS != ALL_BASIC_FIELDS:
             e = "Model {0}: CQRS_FIELDS can't be set together with CQRS_SERIALIZER.".format(
                 model_cls.__name__,
             )
             assert model_cls.CQRS_SERIALIZER is None, e
 
     @staticmethod
     def _check_cqrs_fields(model_cls):
-        """ Check that model has correct CQRS fields configuration.
+        """Check that model has correct CQRS fields configuration.
 
         :param dj_cqrs.mixins.MasterMixin model_cls: CQRS Master Model.
         :raises: AssertionError
         """
         if model_cls.CQRS_FIELDS != ALL_BASIC_FIELDS:
             cqrs_field_names = list(model_cls.CQRS_FIELDS)
             _MetaUtils.check_cqrs_field_setting(model_cls, cqrs_field_names, 'CQRS_FIELDS')
@@ -91,15 +91,15 @@
     def register(model_cls):
         _MetaUtils.check_cqrs_id(model_cls)
         ReplicaMeta._check_cqrs_mapping(model_cls)
         ReplicaRegistry.register_model(model_cls)
 
     @staticmethod
     def _check_cqrs_mapping(model_cls):
-        """ Check that model has correct CQRS mapping configuration.
+        """Check that model has correct CQRS mapping configuration.
 
         :param dj_cqrs.mixins.ReplicaMixin model_cls: CQRS Replica Model.
         :raises: AssertionError
         """
         cqrs_mapping = getattr(model_cls, 'CQRS_MAPPING', None)
         if cqrs_mapping is not None:
             cqrs_field_names = list(cqrs_mapping.values())
@@ -111,15 +111,15 @@
     def check_cqrs_field_setting(cls, model_cls, cqrs_field_names, cqrs_attr):
         cls._check_no_duplicate_names(model_cls, cqrs_field_names, cqrs_attr)
         cls._check_id_in_names(model_cls, cqrs_field_names, cqrs_attr)
         cls._check_unexisting_names(model_cls, cqrs_field_names, cqrs_attr)
 
     @staticmethod
     def check_cqrs_id(model_cls):
-        """ Check that CQRS Model has CQRS_ID set up. """
+        """Check that CQRS Model has CQRS_ID set up."""
         assert model_cls.CQRS_ID, 'CQRS_ID must be set for every model, that uses CQRS.'
 
     @staticmethod
     def _check_no_duplicate_names(model_cls, cqrs_field_names, cqrs_attr):
         model_name = model_cls.__name__
 
         e = 'Duplicate names in {0} field for model {1}.'.format(cqrs_attr, model_name)
```

### Comparing `django_cqrs-2.6.0/dj_cqrs/mixins.py` & `django_cqrs-2.7.0/dj_cqrs/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,20 +60,22 @@
 
     objects = Manager()
 
     cqrs = MasterManager()
     """Manager that adds needed CQRS queryset methods."""
 
     cqrs_revision = IntegerField(
-        default=0, help_text="This field must be incremented on any model update. "
-                             "It's used to for CQRS sync.",
+        default=0,
+        help_text='This field must be incremented on any model update. '
+        "It's used to for CQRS sync.",
     )
     cqrs_updated = DateTimeField(
-        auto_now=True, help_text="This field must be incremented on every model update. "
-                                 "It's used to for CQRS sync.",
+        auto_now=True,
+        help_text='This field must be incremented on every model update. '
+        "It's used to for CQRS sync.",
     )
 
     class Meta:
         abstract = True
 
     @property
     def cqrs_saves_count(self):
@@ -178,15 +180,19 @@
         if not self.CQRS_SERIALIZER:
             try:
                 self.refresh_from_db()
             except self._meta.model.DoesNotExist:
                 return False
 
         MasterSignals.post_save(
-            self._meta.model, instance=self, using=using, queue=queue, sync=True,
+            self._meta.model,
+            instance=self,
+            using=using,
+            queue=queue,
+            sync=True,
         )
         return True
 
     def is_sync_instance(self) -> bool:
         """
         This method can be overridden to apply syncing only to instances by some rules.
         For example, only objects with special status or after some creation date, etc.
@@ -226,32 +232,32 @@
         Returns:
             (django.db.models.QuerySet): The optimized queryset.
 
         """
         return queryset
 
     def get_custom_cqrs_delete_data(self):
-        """ This method should be overridden when additional data is needed in DELETE payload. """
+        """This method should be overridden when additional data is needed in DELETE payload."""
         pass
 
     @classmethod
     def call_post_bulk_create(cls, instances: list, using=None):
-        """ Post bulk create signal caller (django doesn't support it by default).
+        """Post bulk create signal caller (django doesn't support it by default).
 
         ``` py3
 
             # Used automatically by cqrs.bulk_create()
             instances = model.cqrs.bulk_create(instances)
         ```
         """
         post_bulk_create.send(cls, instances=instances, using=using)
 
     @classmethod
     def call_post_update(cls, instances, using=None):
-        """ Post bulk update signal caller (django doesn't support it by default).
+        """Post bulk update signal caller (django doesn't support it by default).
 
         ``` py3
 
             # Used automatically by cqrs.bulk_update()
             qs = model.objects.filter(k1=v1)
             model.cqrs.bulk_update(qs, k2=v2)
         ```
@@ -318,15 +324,15 @@
                 fields_to_refresh.append(f.name)
 
         if fields_to_refresh:
             self.refresh_from_db(fields=fields_to_refresh)
 
     @property
     def _cqrs_serializer_cls(self):
-        """ Serialization class loader. """
+        """Serialization class loader."""
         if hasattr(self.__class__, '_cqrs_serializer_class'):
             return self.__class__._cqrs_serializer_class
 
         try:
             serializer = import_string(self.CQRS_SERIALIZER)
             self.__class__._cqrs_serializer_class = serializer
             return serializer
@@ -336,22 +342,24 @@
             )
 
 
 class MasterMixin(RawMasterMixin, metaclass=MasterMeta):
     """
     Mixin for the master CQRS model, that will send data updates to it's replicas.
     """
+
     class Meta:
         abstract = True
 
 
 class RawReplicaMixin:
     CQRS_ID = None
     CQRS_NO_DB_OPERATIONS = True
     CQRS_META = False
+    CQRS_ONLY_DIRECT_SYNCS = False
 
     @classmethod
     def cqrs_save(cls, master_data, **kwargs):
         raise NotImplementedError
 
     @classmethod
     def cqrs_delete(cls, master_data, **kwargs):
@@ -389,14 +397,15 @@
 
 
 class ReplicaMixin(RawReplicaMixin, Model, metaclass=ReplicaMeta):
     """
     Mixin for the replica CQRS model, that will receive data updates from master. Models, using
     this mixin should be readonly, but this is not enforced (f.e. for admin).
     """
+
     CQRS_ID = None
     """Unique CQRS identifier for all microservices."""
 
     CQRS_MAPPING = None
     """Mapping of master data field name to replica model field name."""
 
     CQRS_CUSTOM_SERIALIZATION = False
@@ -428,15 +437,15 @@
     def cqrs_save(
         cls,
         master_data: dict,
         previous_data: dict = None,
         sync: bool = False,
         meta: dict = None,
     ):
-        """ This method saves (creates or updates) model instance from CQRS master instance data.
+        """This method saves (creates or updates) model instance from CQRS master instance data.
         This method must not be overridden. Otherwise, sync checks need to be implemented manually.
 
         Args:
             master_data (dict): CQRS master instance data.
             previous_data (dict): Previous values for tracked fields.
             sync (bool): Sync package flag.
             meta (dict): Payload metadata, if exists.
@@ -453,15 +462,15 @@
     def cqrs_create(
         cls,
         sync: bool,
         mapped_data: dict,
         previous_data: dict = None,
         meta: dict = None,
     ):
-        """ This method creates model instance from CQRS mapped instance data. It must be overridden
+        """This method creates model instance from CQRS mapped instance data. It must be overridden
         by replicas of master models with custom serialization.
 
         Args:
             sync (dict): Sync package flag.
             mapped_data (dict): CQRS mapped instance data.
             previous_data (dict): Previous mapped values for tracked fields.
             meta (dict): Payload metadata, if exists.
@@ -474,15 +483,15 @@
     def cqrs_update(
         self,
         sync: bool,
         mapped_data: dict,
         previous_data: dict = None,
         meta: dict = None,
     ):
-        """ This method updates model instance from CQRS mapped instance data. It must be overridden
+        """This method updates model instance from CQRS mapped instance data. It must be overridden
         by replicas of master models with custom serialization.
 
         Args:
             sync (dict): Sync package flag.
             mapped_data (dict): CQRS mapped instance data.
             previous_data (dict): Previous mapped values for tracked fields.
             meta (dict): Payload metadata, if exists.
@@ -494,15 +503,15 @@
         for key, value in mapped_data.items():
             setattr(self, key, value)
         self.save()
         return self
 
     @classmethod
     def cqrs_delete(cls, master_data: dict, meta: dict = None) -> bool:
-        """ This method deletes model instance from mapped CQRS master instance data.
+        """This method deletes model instance from mapped CQRS master instance data.
 
         Args:
             master_data (dict): CQRS master instance data.
             meta (dict): Payload metadata, if exists.
 
         Returns:
             (bool): Flag, if delete operation is successful (even if nothing was deleted).
```

### Comparing `django_cqrs-2.6.0/dj_cqrs/registries.py` & `django_cqrs-2.7.0/dj_cqrs/registries.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 logger = logging.getLogger('django-cqrs')
 
 
 class RegistryMixin:
     @classmethod
     def register_model(cls, model_cls):
-        """ Registration of CQRS model identifiers. """
+        """Registration of CQRS model identifiers."""
 
         e = "Two models can't have the same CQRS_ID: {0}.".format(model_cls.CQRS_ID)
         assert model_cls.CQRS_ID not in cls.models, e
 
         cls.models[model_cls.CQRS_ID] = model_cls
 
     @classmethod
```

### Comparing `django_cqrs-2.6.0/dj_cqrs/signals.py` & `django_cqrs-2.7.0/dj_cqrs/signals.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 """
 Signal sent after a bulk update.
 See dj_cqrs.mixins.RawMasterMixin.call_post_update.
 """
 
 
 class MasterSignals:
-    """ Signals registry and handlers for CQRS master models. """
+    """Signals registry and handlers for CQRS master models."""
+
     @classmethod
     def register_model(cls, model_cls):
         """
         Registers signals for a model.
 
         Args:
             model_cls (dj_cqrs.mixins.MasterMixin): Model class inherited from CQRS MasterMixin.
```

### Comparing `django_cqrs-2.6.0/dj_cqrs/tracker.py` & `django_cqrs-2.7.0/dj_cqrs/tracker.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,40 +4,34 @@
 from model_utils.tracker import FieldInstanceTracker
 
 from dj_cqrs.constants import ALL_BASIC_FIELDS, FIELDS_TRACKER_FIELD_NAME
 from dj_cqrs.utils import get_json_valid_value
 
 
 class _CQRSTrackerInstance(FieldInstanceTracker):
-
     def __init__(self, instance, fields, field_map):
         super().__init__(instance, fields, field_map)
         self._attr_to_field_map = {
-            f.attname: f.name
-            for f in instance._meta.concrete_fields if f.is_relation
+            f.attname: f.name for f in instance._meta.concrete_fields if f.is_relation
         }
 
     def changed(self):
         changed_fields = super().changed()
-        return {
-            self._attr_to_field_map.get(k, k): v
-            for k, v in changed_fields.items()
-        }
+        return {self._attr_to_field_map.get(k, k): v for k, v in changed_fields.items()}
 
     def changed_initial(self):
         return {field: None for field in self.fields if self.get_field_value(field) is not None}
 
     def get_field_value(self, field):
         value = super().get_field_value(field)
 
         return get_json_valid_value(value)
 
 
 class CQRSTracker(FieldTracker):
-
     tracker_class = _CQRSTrackerInstance
 
     @classmethod
     def add_to_model(cls, model_cls):
         """
         Add the CQRSTracker to a model.
```

### Comparing `django_cqrs-2.6.0/dj_cqrs/transport/__init__.py` & `django_cqrs-2.7.0/dj_cqrs/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.6.0/dj_cqrs/transport/base.py` & `django_cqrs-2.7.0/dj_cqrs/transport/base.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.6.0/dj_cqrs/transport/kombu.py` & `django_cqrs-2.7.0/dj_cqrs/transport/kombu.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from dj_cqrs.transport.mixins import LoggingMixin
 
 
 logger = logging.getLogger('django-cqrs')
 
 
 class _KombuConsumer(ConsumerMixin):
-
     def __init__(self, url, exchange_name, queue_name, prefetch_count, callback, cqrs_ids=None):
         self.connection = Connection(url)
         self.exchange = Exchange(
             exchange_name,
             type='topic',
             durable=True,
         )
@@ -72,14 +71,15 @@
                 auto_declare=True,
             ),
         ]
 
 
 class KombuTransport(LoggingMixin, BaseTransport):
     """Transport class for Kombu."""
+
     CONSUMER_RETRY_TIMEOUT = 5
 
     @classmethod
     def clean_connection(cls):
         """Nothing to do here"""
         pass
 
@@ -117,17 +117,20 @@
         try:
             # Decided not to create context-manager to stay within the class
             connection, channel = cls._get_producer_kombu_objects(url, exchange_name)
             exchange = cls._create_exchange(exchange_name)
             cls._produce_message(channel, exchange, payload)
             cls.log_produced(payload)
         except KombuError:
-            logger.error("CQRS couldn't be published: pk = {0} ({1}).".format(
-                payload.pk, payload.cqrs_id,
-            ))
+            logger.error(
+                "CQRS couldn't be published: pk = {0} ({1}).".format(
+                    payload.pk,
+                    payload.cqrs_id,
+                ),
+            )
         finally:
             if connection:
                 connection.close()
 
     @classmethod
     def _consume_message(cls, body, message):
         try:
```

### Comparing `django_cqrs-2.6.0/dj_cqrs/transport/mixins.py` & `django_cqrs-2.7.0/dj_cqrs/transport/mixins.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,92 +3,95 @@
 import logging
 
 
 logger = logging.getLogger('django-cqrs')
 
 
 class LoggingMixin:
-    _BASE_PAYLOAD_LOG_TEMPLATE = "CQRS is %s: pk = %s (%s), correlation_id = %s."
+    _BASE_PAYLOAD_LOG_TEMPLATE = 'CQRS is %s: pk = %s (%s), correlation_id = %s.'
 
     @staticmethod
     def log_consumed(payload):
         """
         Args:
             payload (dj_cqrs.dataclasses.TransportPayload): Transport payload from master model.
         """
-        msg = "CQRS is received: pk = %s (%s), correlation_id = %s."
+        msg = 'CQRS is received: pk = %s (%s), correlation_id = %s.'
         logger.info(msg, payload.pk, payload.cqrs_id, payload.correlation_id)
 
     @staticmethod
     def log_consumed_accepted(payload):
         """
         Args:
             payload (dj_cqrs.dataclasses.TransportPayload): Transport payload from master model.
         """
-        msg = "CQRS is applied: pk = %s (%s), correlation_id = %s."
+        msg = 'CQRS is applied: pk = %s (%s), correlation_id = %s.'
         logger.info(msg, payload.pk, payload.cqrs_id, payload.correlation_id)
 
     @staticmethod
     def log_consumed_denied(payload):
         """
         Args:
             payload (dj_cqrs.dataclasses.TransportPayload): Transport payload from master model.
         """
-        msg = "CQRS is denied: pk = %s (%s), correlation_id = %s."
+        msg = 'CQRS is denied: pk = %s (%s), correlation_id = %s.'
         logger.warning(msg, payload.pk, payload.cqrs_id, payload.correlation_id)
 
     @staticmethod
     def log_consumed_failed(payload):
         """
         Args:
             payload (dj_cqrs.dataclasses.TransportPayload): Transport payload from master model.
         """
-        msg = (
-            "CQRS is failed: pk = %s (%s), correlation_id = %s, retries = %s.",
-        )
+        msg = ('CQRS is failed: pk = %s (%s), correlation_id = %s, retries = %s.',)
         logger.warning(
-            msg, payload.pk, payload.cqrs_id, payload.correlation_id, payload.retries,
+            msg,
+            payload.pk,
+            payload.cqrs_id,
+            payload.correlation_id,
+            payload.retries,
         )
 
     @staticmethod
     def log_dead_letter(payload):
         """
         Args:
             payload (dj_cqrs.dataclasses.TransportPayload): Transport payload from master model.
         """
-        msg = "CQRS is added to dead letter queue: pk = %s (%s), correlation_id = %s."
+        msg = 'CQRS is added to dead letter queue: pk = %s (%s), correlation_id = %s.'
         logger.warning(msg, payload.pk, payload.cqrs_id, payload.correlation_id)
 
     @staticmethod
     def log_delayed(payload, delay, eta):
         """
         Args:
             payload (dj_cqrs.dataclasses.TransportPayload): Transport payload from master model.
             delay (int): Seconds to wait before requeuing message.
             eta (datetime): Requeuing datetime.
         """
-        msg = (
-            "CQRS is delayed: pk = %s (%s), correlation_id = %s, delay = %s sec, eta = %s.",
-        )
+        msg = ('CQRS is delayed: pk = %s (%s), correlation_id = %s, delay = %s sec, eta = %s.',)
         logger.warning(
-            msg, payload.pk, payload.cqrs_id, payload.correlation_id, delay, eta,
+            msg,
+            payload.pk,
+            payload.cqrs_id,
+            payload.correlation_id,
+            delay,
+            eta,
         )
 
     @staticmethod
     def log_requeued(payload):
         """
         Args:
             payload (dj_cqrs.dataclasses.TransportPayload): Transport payload from master model.
         """
-        msg = (
-            "CQRS is requeued: pk = %s (%s), correlation_id = %s.",
-        )
+        msg = ('CQRS is requeued: pk = %s (%s), correlation_id = %s.',)
         logger.warning(msg, payload.pk, payload.cqrs_id, payload.correlation_id)
 
     @staticmethod
     def log_produced(payload):
         """
         Args:
             payload (dj_cqrs.dataclasses.TransportPayload): Transport payload from master model.
         """
-        msg = "CQRS is published: pk = %s (%s), correlation_id = %s."
+        msg = 'CQRS is published: pk = %s (%s), correlation_id = %s.'
         logger.info(msg, payload.pk, payload.cqrs_id, payload.correlation_id)
```

### Comparing `django_cqrs-2.6.0/dj_cqrs/transport/rabbit_mq.py` & `django_cqrs-2.7.0/dj_cqrs/transport/rabbit_mq.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,29 +29,30 @@
 
 
 logger = logging.getLogger('django-cqrs')
 
 
 class RabbitMQTransport(LoggingMixin, BaseTransport):
     """Transport class for RabbitMQ."""
+
     CONSUMER_RETRY_TIMEOUT = 5
     PRODUCER_RETRIES = 1
 
     _producer_connection = None
     _producer_channel = None
 
     @classmethod
     def clean_connection(cls):
         """Clean the RabbitMQ connection."""
         connection = cls._producer_connection
         if connection and not connection.is_closed:
             try:
                 connection.close()
             except (exceptions.StreamLostError, exceptions.ConnectionClosed, ConnectionError):
-                logger.warning("Connection was closed or is closing. Skip it...")
+                logger.warning('Connection was closed or is closing. Skip it...')
 
         cls._producer_connection = None
         cls._producer_channel = None
 
     @classmethod
     def consume(cls, cqrs_ids=None):
         """Receive data from master model.
@@ -63,27 +64,34 @@
         common_rabbit_settings = cls._get_common_settings()
 
         while True:
             connection = None
             try:
                 delay_queue = DelayQueue(max_size=get_delay_queue_max_size())
                 connection, channel, consumer_generator = cls._get_consumer_rmq_objects(
-                    *(common_rabbit_settings + consumer_rabbit_settings), cqrs_ids=cqrs_ids,
+                    *(common_rabbit_settings + consumer_rabbit_settings),
+                    cqrs_ids=cqrs_ids,
                 )
 
                 for method_frame, properties, body in consumer_generator:
                     if method_frame is not None:
                         cls._consume_message(
-                            channel, method_frame, properties, body, delay_queue,
+                            channel,
+                            method_frame,
+                            properties,
+                            body,
+                            delay_queue,
                         )
                     cls._process_delay_messages(channel, delay_queue)
-            except (exceptions.AMQPError,
-                    exceptions.ChannelError,
-                    exceptions.ReentrancyError,
-                    gaierror):
+            except (
+                exceptions.AMQPError,
+                exceptions.ChannelError,
+                exceptions.ReentrancyError,
+                gaierror,
+            ):
                 logger.warning('AMQP connection error. Reconnecting...', exc_info=True)
                 time.sleep(cls.CONSUMER_RETRY_TIMEOUT)
             finally:
                 if connection and not connection.is_closed:
                     connection.close()
 
     @classmethod
@@ -99,15 +107,16 @@
     @classmethod
     def _produce_with_retries(cls, payload, retries):
         try:
             rmq_settings = cls._get_common_settings()
             exchange = rmq_settings[-1]
             # Decided not to create context-manager to stay within the class
             _, channel = cls._get_producer_rmq_objects(
-                *rmq_settings, signal_type=payload.signal_type,
+                *rmq_settings,
+                signal_type=payload.signal_type,
             )
 
             cls._produce_message(channel, exchange, payload)
             cls.log_produced(payload)
         except (
             exceptions.AMQPError,
             exceptions.ChannelError,
@@ -115,23 +124,27 @@
             AMQPConnectorException,
             AssertionError,
         ) as e:
             # in case of any error - close connection and try to reconnect
             cls.clean_connection()
 
             base_log_message = "CQRS couldn't be published: pk = {0} ({1}).".format(
-                payload.pk, payload.cqrs_id,
+                payload.pk,
+                payload.cqrs_id,
             )
             if not retries:
                 logger.exception(base_log_message)
                 return
 
-            logger.warning('{0} Error: {1}. Reconnect...'.format(
-                base_log_message, e.__class__.__name__,
-            ))
+            logger.warning(
+                '{0} Error: {1}. Reconnect...'.format(
+                    base_log_message,
+                    e.__class__.__name__,
+                ),
+            )
 
             cls._produce_with_retries(payload, retries - 1)
 
     @classmethod
     def _consume_message(cls, ch, method, properties, body, delay_queue):
         try:
             dct = ujson.loads(body)
@@ -158,29 +171,33 @@
             return
 
         instance, exception = None, None
         try:
             instance = consumer.consume(payload)
         except Exception as e:
             exception = e
-            logger.error("CQRS service exception", exc_info=True)
+            logger.error('CQRS service exception', exc_info=True)
 
         if instance and exception is None:
             cls._ack(ch, delivery_tag, payload)
         else:
             cls._fail_message(
-                ch, delivery_tag, payload, exception, delay_queue,
+                ch,
+                delivery_tag,
+                payload,
+                exception,
+                delay_queue,
             )
 
     @classmethod
     def _fail_message(cls, channel, delivery_tag, payload, exception, delay_queue):
         cls.log_consumed_failed(payload)
         model_cls = ReplicaRegistry.get_model_by_cqrs_id(payload.cqrs_id)
         if model_cls is None:
-            logger.error("Model for cqrs_id {0} is not found.".format(payload.cqrs_id))
+            logger.error('Model for cqrs_id {0} is not found.'.format(payload.cqrs_id))
             cls._nack(channel, delivery_tag)
             return
 
         if model_cls.should_retry_cqrs(payload.retries, exception):
             delay = model_cls.get_cqrs_retry_delay(payload.retries)
             cls._delay_message(channel, delivery_tag, payload, delay, delay_queue)
         else:
@@ -357,15 +374,15 @@
         )
 
     @staticmethod
     def _parse_url(url):
         scheme = urlparse(url).scheme
         assert scheme == 'amqp', 'Scheme must be "amqp" for RabbitMQTransport.'
 
-        schemeless = url[len(scheme) + 3:]
+        schemeless = url[len(scheme) + 3 :]
         parts = urlparse('http://' + schemeless)
 
         return (
             unquote(parts.hostname or '') or ConnectionParameters.DEFAULT_HOST,
             parts.port or ConnectionParameters.DEFAULT_PORT,
             unquote(parts.username or '') or ConnectionParameters.DEFAULT_USERNAME,
             unquote(parts.password or '') or ConnectionParameters.DEFAULT_PASSWORD,
```

### Comparing `django_cqrs-2.6.0/dj_cqrs/utils.py` & `django_cqrs-2.7.0/dj_cqrs/utils.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.6.0/pyproject.toml` & `django_cqrs-2.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-cqrs"
-version = "2.6.0"
+version = "2.7.0"
 description = "Django CQRS data synchronisation"
 authors = ["CloudBlue LLC"]
 license = "Apache-2.0"
 packages = [
     { include = "dj_cqrs" }
 ]
 readme = "./README.md"
@@ -41,22 +41,24 @@
 kombu = ">=4.6.*"
 ujson = ">=5.4.0"
 django-model-utils = ">=4.0.0"
 python-dateutil = ">=2.4"
 watchfiles = "^0.18.1"
 
 [tool.poetry.group.test.dependencies]
+black = ">=23.3"
 pytest = ">=7.2.0,<8"
 pytest-cov = ">=2.10.1,<5"
 pytest-mock = "^3.10"
 pytest-django = ">=4.4.0"
 pytest-randomly = ">=3.12"
 pytest-deadfixtures = "^2.2.1"
 coverage = {extras = ["toml"], version = ">=5.3,<7"}
 flake8 = ">=3.8,<6"
+flake8-black = ">=0.3"
 flake8-bugbear = ">=20,<23"
 flake8-cognitive-complexity = "^0.1"
 flake8-commas = "~2.1"
 flake8-future-import = "~0.4"
 flake8-isort = "^6.0"
 flake8-broken-line = ">=0.3,<0.7"
 flake8-comprehensions = "^3.10.1"
@@ -117,8 +119,13 @@
     "*.egg",
     "*.egg-info",
     "examples/*migrations/*",
 ]
 show-source = true
 max-line-length = 100
 max-cognitive-complexity = 20
+select = "B"
 ignore = ["FI1", "W503", "W605"]
+
+[tool.black]
+line_length = 100
+skip-string-normalization = true
```

### Comparing `django_cqrs-2.6.0/PKG-INFO` & `django_cqrs-2.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cqrs
-Version: 2.6.0
+Version: 2.7.0
 Summary: Django CQRS data synchronisation
 Home-page: https://django-cqrs.readthedocs.org
 License: Apache-2.0
 Keywords: django,cqrs,sql,mixin,amqp
 Author: CloudBlue LLC
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 5 - Production/Stable
@@ -242,16 +242,17 @@
 ```
 
 Development
 ===========
 
 1. Python >= 3.8
 2. Install dependencies `requirements/dev.txt`
-3. We use `isort` library to order and format our imports, and we check it using `flake8-isort` library (automatically on `flake8` run).  
-For convenience you may run `isort .` to order imports.
+3. We use `isort` library to order and format our imports, and `black` - to format the code. 
+We check it using `flake8-isort` and `flake8-black` libraries (automatically on `flake8` run).  
+For convenience you may run `isort . && black .` to format the code.
 
 
 Testing
 =======
 
 Unit testing
 ------
```

