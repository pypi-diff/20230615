# Comparing `tmp/django-business-metrics-0.1.0a5.tar.gz` & `tmp/django-business-metrics-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-business-metrics-0.1.0a5.tar", max compression
+gzip compressed data, was "django-business-metrics-1.0.0.tar", max compression
```

## Comparing `django-business-metrics-0.1.0a5.tar` & `django-business-metrics-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1004 2022-08-22 06:48:38.843283 django-business-metrics-0.1.0a5/README.md
--rw-r--r--   0        0        0        0 2022-08-14 18:04:19.544999 django-business-metrics-0.1.0a5/django_business_metrics/__init__.py
--rw-r--r--   0        0        0      298 2022-08-21 19:37:54.330958 django-business-metrics-0.1.0a5/django_business_metrics/metrics.py
--rw-r--r--   0        0        0     3321 2022-08-22 06:47:38.193706 django-business-metrics-0.1.0a5/django_business_metrics/metrics_manager.py
--rw-r--r--   0        0        0      139 2022-08-21 19:23:15.836007 django-business-metrics-0.1.0a5/django_business_metrics/v0/__init__.py
--rw-r--r--   0        0        0      565 2022-08-22 06:52:39.265589 django-business-metrics-0.1.0a5/pyproject.toml
--rw-r--r--   0        0        0     1767 2022-08-22 06:52:58.405919 django-business-metrics-0.1.0a5/setup.py
--rw-r--r--   0        0        0     1602 2022-08-22 06:52:58.406126 django-business-metrics-0.1.0a5/PKG-INFO
+-rw-r--r--   0        0        0     1287 2023-06-15 12:06:22.909135 django-business-metrics-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2022-08-14 18:04:19.544999 django-business-metrics-1.0.0/django_business_metrics/__init__.py
+-rw-r--r--   0        0        0      148 2023-06-15 12:06:22.909135 django-business-metrics-1.0.0/django_business_metrics/_internal/__init__.py
+-rw-r--r--   0        0        0      298 2023-06-15 12:06:22.909135 django-business-metrics-1.0.0/django_business_metrics/_internal/metrics.py
+-rw-r--r--   0        0        0     3365 2023-06-15 12:06:22.909135 django-business-metrics-1.0.0/django_business_metrics/_internal/metrics_manager.py
+-rw-r--r--   0        0        0       62 2022-08-25 10:16:06.678805 django-business-metrics-1.0.0/django_business_metrics/models.py
+-rw-r--r--   0        0        0      159 2023-06-15 12:06:22.909135 django-business-metrics-1.0.0/django_business_metrics/v0/__init__.py
+-rw-r--r--   0        0        0     1448 2023-06-15 12:06:22.910135 django-business-metrics-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2327 2023-06-15 12:07:03.562394 django-business-metrics-1.0.0/setup.py
+-rw-r--r--   0        0        0     2168 2023-06-15 12:07:03.562567 django-business-metrics-1.0.0/PKG-INFO
```

### Comparing `django-business-metrics-0.1.0a5/django_business_metrics/metrics_manager.py` & `django-business-metrics-1.0.0/django_business_metrics/_internal/metrics_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+from __future__ import annotations
+
+from collections.abc import Iterable
 from concurrent.futures import ThreadPoolExecutor
 from dataclasses import dataclass
-from typing import Callable, Dict, Iterable, Optional
+from typing import Callable
 
 import prometheus_client
 from django.http import HttpRequest, HttpResponse
 from prometheus_client.metrics_core import GaugeMetricFamily
 from prometheus_client.registry import CollectorRegistry
 
 
@@ -12,15 +15,15 @@
 class _BusinessMetric:
     name: str
     documentation: str
     callable: Callable[[], float]
 
 
 class _BusinessMetricsCollector(CollectorRegistry):
-    _metrics: Dict[str, _BusinessMetric]
+    _metrics: dict[str, _BusinessMetric]
     _concurrent_collections: int
     _timeout: float
 
     def __init__(self, concurrent_collections: int, timeout: float):
         self._metrics = {}
         self._concurrent_collections = concurrent_collections
         self._timeout = timeout
@@ -64,15 +67,15 @@
             name=name or callable.__name__,
             documentation=documentation,
             callable=callable,
         )
         self._collector.add(metric)
         return self
 
-    def metric(self, name: Optional[str] = None, documentation: str = ""):
+    def metric(self, name: str | None = None, documentation: str = ""):
         """A decorator that marks a function as a metric.
 
         Example use:
         ```
         @metric_manager.metric(name='my_metric_name', documentation='My documentation')
         def my_metric():
             return 1
```

### Comparing `django-business-metrics-0.1.0a5/setup.py` & `django-business-metrics-1.0.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,42 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['django_business_metrics', 'django_business_metrics.v0']
+['django_business_metrics',
+ 'django_business_metrics._internal',
+ 'django_business_metrics.v0']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['Django>=3,<4', 'prometheus-client>=0.13.0,<0.15']
+['Django>=3', 'prometheus-client>=0.13.0']
+
+extras_require = \
+{'dev': ['black>=22.6.0',
+         'django-stubs>=1.12.0',
+         'mypy>=0.971',
+         'nox>=2023',
+         'pytest>=6',
+         'pytest-django',
+         'ruff>=0.0.272']}
 
 setup_kwargs = {
     'name': 'django-business-metrics',
-    'version': '0.1.0a5',
+    'version': '1.0.0',
     'description': 'Django Prometheus business metrics',
-    'long_description': "# Django Prometheus business metrics\n\nThis Django app provides a Prometheus metrics endpoint serving so-called business metrics. These are metrics that are calculated when Prometheus hits the metrics endpoint.\n\n## Usage\n\n1. Create a `BusinessMetricsManager` object and register some metrics:\n\n    ```\n    # project/business_metrics.py\n\n    from django_business_metrics.v0 import BusinessMetricsManager, users\n\n    metrics_manager = BusinessMetricsManager()\n\n    # Add a pre-defined metric\n    metrics_manager.add(users)\n\n    # Add some custom metrics\n    @metrics_manager.metric(name='name', documentation='documentation')\n    def my_metric():\n        return 10\n    ```\n\n2. Register a Prometheus endpoint:\n\n\n    ```\n    # project/urls.py\n\n    ...\n    from .business_metrics import metrics_manager\n\n    ...\n    urlpatterns = [\n        ...\n        path('business-metrics', metrics_manager.view),\n        ...\n    ]\n    ```\n\n3. Setup your Prometheus agent to scrape metrics from `/business-metrics` endpoint.",
+    'long_description': "# Django Prometheus business metrics\n\nThis Django app provides a Prometheus metrics endpoint serving so-called business metrics. These are metrics that are calculated when Prometheus hits the metrics endpoint.\n\n## Usage\n\n> This project uses [ApiVer](https://www.youtube.com/watch?v=FgcoAKchPjk).\n> Always import from `django_business_metrics.v0` namespace and not from `django_business_metrics`.\n\n\n1. Create a `BusinessMetricsManager` object and register some metrics:\n\n    ```\n    # project/business_metrics.py\n\n    from django_business_metrics.v0 import BusinessMetricsManager, users\n\n    metrics_manager = BusinessMetricsManager()\n\n    # Add a pre-defined metric\n    metrics_manager.add(users)\n\n    # Add some custom metrics\n    @metrics_manager.metric(name='name', documentation='documentation')\n    def my_metric():\n        return 10\n    ```\n\n2. Register a Prometheus endpoint:\n\n\n    ```\n    # project/urls.py\n\n    ...\n    from .business_metrics import metrics_manager\n\n    ...\n    urlpatterns = [\n        ...\n        path('business-metrics', metrics_manager.view),\n        ...\n    ]\n    ```\n\n3. Setup your Prometheus agent to scrape metrics from `/business-metrics` endpoint.\n\n\n## Development\n\n```\npoetry install\n```\n\nBefore committing make sure to run:\n\n```\nnox -s format test\n```",
     'author': 'Reef Technologies',
     'author_email': 'vykintas.baltrusaitis@reef.pl',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
+    'extras_require': extras_require,
+    'python_requires': '>=3.9',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `django-business-metrics-0.1.0a5/PKG-INFO` & `django-business-metrics-1.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,17 @@
-Metadata-Version: 2.1
-Name: django-business-metrics
-Version: 0.1.0a5
-Summary: Django Prometheus business metrics
-License: MIT
-Author: Reef Technologies
-Author-email: vykintas.baltrusaitis@reef.pl
-Requires-Python: >=3.8,<3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: Django (>=3,<4)
-Requires-Dist: prometheus-client (>=0.13.0,<0.15)
-Description-Content-Type: text/markdown
-
 # Django Prometheus business metrics
 
 This Django app provides a Prometheus metrics endpoint serving so-called business metrics. These are metrics that are calculated when Prometheus hits the metrics endpoint.
 
 ## Usage
 
+> This project uses [ApiVer](https://www.youtube.com/watch?v=FgcoAKchPjk).
+> Always import from `django_business_metrics.v0` namespace and not from `django_business_metrics`.
+
+
 1. Create a `BusinessMetricsManager` object and register some metrics:
 
     ```
     # project/business_metrics.py
 
     from django_business_metrics.v0 import BusinessMetricsManager, users
 
@@ -53,7 +40,20 @@
         ...
         path('business-metrics', metrics_manager.view),
         ...
     ]
     ```
 
 3. Setup your Prometheus agent to scrape metrics from `/business-metrics` endpoint.
+
+
+## Development
+
+```
+poetry install
+```
+
+Before committing make sure to run:
+
+```
+nox -s format test
+```
```

