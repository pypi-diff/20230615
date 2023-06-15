# Comparing `tmp/otel_tracer-0.0.4-py3-none-any.whl.zip` & `tmp/otel_tracer-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,12 @@
-Zip file size: 2199 bytes, number of entries: 7
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-12 04:21 otel_tracer/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-12 04:35 otel_tracer/tracing/__init__.py
--rw-r--r--  2.0 unx     1558 b- defN 23-Jun-13 06:09 otel_tracer/tracing/tracer.py
--rw-r--r--  2.0 unx      854 b- defN 23-Jun-13 06:10 otel_tracer-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 06:10 otel_tracer-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-13 06:10 otel_tracer-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      561 b- defN 23-Jun-13 06:10 otel_tracer-0.0.4.dist-info/RECORD
-7 files, 3077 bytes uncompressed, 1191 bytes compressed:  61.3%
+Zip file size: 3624 bytes, number of entries: 10
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-15 03:17 otel_tracer/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-15 03:17 otel_tracer/tracing/__init__.py
+-rw-r--r--  2.0 unx     1639 b- defN 23-Jun-15 03:17 otel_tracer/tracing/tracer.py
+-rw-r--r--  2.0 unx     2311 b- defN 23-Jun-15 03:17 otel_tracer/tracing/threading_instrumentor/__init__.py
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-15 03:17 otel_tracer/tracing/threading_instrumentor/package.py
+-rw-r--r--  2.0 unx       26 b- defN 23-Jun-15 03:17 otel_tracer/tracing/threading_instrumentor/version.py
+-rw-r--r--  2.0 unx      670 b- defN 23-Jun-15 03:17 otel_tracer-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 03:17 otel_tracer-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-15 03:17 otel_tracer-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      888 b- defN 23-Jun-15 03:17 otel_tracer-0.0.5.dist-info/RECORD
+10 files, 5683 bytes uncompressed, 2068 bytes compressed:  63.6%
```

## zipnote {}

```diff
@@ -3,20 +3,29 @@
 
 Filename: otel_tracer/tracing/__init__.py
 Comment: 
 
 Filename: otel_tracer/tracing/tracer.py
 Comment: 
 
-Filename: otel_tracer-0.0.4.dist-info/METADATA
+Filename: otel_tracer/tracing/threading_instrumentor/__init__.py
 Comment: 
 
-Filename: otel_tracer-0.0.4.dist-info/WHEEL
+Filename: otel_tracer/tracing/threading_instrumentor/package.py
 Comment: 
 
-Filename: otel_tracer-0.0.4.dist-info/top_level.txt
+Filename: otel_tracer/tracing/threading_instrumentor/version.py
 Comment: 
 
-Filename: otel_tracer-0.0.4.dist-info/RECORD
+Filename: otel_tracer-0.0.5.dist-info/METADATA
+Comment: 
+
+Filename: otel_tracer-0.0.5.dist-info/WHEEL
+Comment: 
+
+Filename: otel_tracer-0.0.5.dist-info/top_level.txt
+Comment: 
+
+Filename: otel_tracer-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## otel_tracer/tracing/tracer.py

```diff
@@ -1,49 +1,56 @@
+from flask import request
 from opentelemetry import trace
-from opentelemetry.exporter.otlp.proto.grpc.trace_exporter import OTLPSpanExporter
-from opentelemetry.sdk.resources import Resource
-from opentelemetry.sdk.trace import TracerProvider
-from opentelemetry.sdk.trace.export import BatchSpanProcessor
+from opentelemetry.exporter.otlp.proto.grpc.trace_exporter import \
+    OTLPSpanExporter
 from opentelemetry.instrumentation.flask import FlaskInstrumentor
-from opentelemetry.instrumentation.requests import RequestsInstrumentor
 from opentelemetry.instrumentation.pika import PikaInstrumentor
 from opentelemetry.instrumentation.redis import RedisInstrumentor
+from opentelemetry.instrumentation.requests import RequestsInstrumentor
+from opentelemetry.sdk.resources import Resource
+from opentelemetry.sdk.trace import TracerProvider
+from opentelemetry.sdk.trace.export import BatchSpanProcessor
+
+from .threading_instrumentor import ThreadingInstrumentor
 
 
-def flask_tracer(app, servicename, endpoint):
+def init_flask(app, servicename, endpoint):
     FlaskInstrumentor().instrument_app(app)
 
     trace.set_tracer_provider(
         TracerProvider(
             resource=Resource.create({"service.name": servicename})
         )
     )
 
     otlp_exporter = OTLPSpanExporter(
         endpoint=endpoint  # Use the address and port of your OpenTelemetry Collector
     )
     span_processor = BatchSpanProcessor(otlp_exporter)
 
     trace.get_tracer_provider().add_span_processor(span_processor)
+
+    @app.before_request
+    def start_span():
+        span_name = request.path or "root"
+        request.span = trace.get_tracer(__name__).start_span(span_name)
+
+    @app.after_request
+    def end_span(response):
+        request.span.end()
+        return response
     return app
 
 
-def requests_tracer():
+def init_requests():
     RequestsInstrumentor().instrument()
 
 
-def redis_tracer():
+def init_redis():
     RedisInstrumentor().instrument()
 
 
-def pika_tracer():
+def init_pika():
     PikaInstrumentor().instrument()
 
-
-def celery_tracer():
-    from opentelemetry.instrumentation.celery import CeleryInstrumentor
-    CeleryInstrumentor().instrument()
-
-
-def flask_sqlalchemy_tracer():
-    from opentelemetry.instrumentation.sqlalchemy import SQLAlchemyInstrumentor
-    SQLAlchemyInstrumentor().instrument(enable_commenter=True, commenter_options={})
+def init_threading():
+    ThreadingInstrumentor().instrument()
```

## Comparing `otel_tracer-0.0.4.dist-info/METADATA` & `otel_tracer-0.0.5.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 Metadata-Version: 2.1
 Name: otel-tracer
-Version: 0.0.4
-Summary: common python utilities for otel
+Version: 0.0.5
+Summary: common python utilities for VxRail
 Home-page: UNKNOWN
 Author: VxRail
 Author-email: UNKNOWN
 License: ToBeDone
 Platform: python3
 Requires-Dist: flask
 Requires-Dist: opentelemetry-api
-Requires-Dist: opentelemetry-exporter-jaeger-thrift
 Requires-Dist: opentelemetry-exporter-otlp-proto-grpc
-Requires-Dist: opentelemetry-instrumentation-celery
 Requires-Dist: opentelemetry-instrumentation-flask
 Requires-Dist: opentelemetry-instrumentation-pika
 Requires-Dist: opentelemetry-instrumentation-redis
 Requires-Dist: opentelemetry-instrumentation-requests
-Requires-Dist: opentelemetry-instrumentation-sqlalchemy
 Requires-Dist: opentelemetry-sdk
 Requires-Dist: opentelemetry-semantic-conventions
 Requires-Dist: pika
 Requires-Dist: redis
 Requires-Dist: requests
-Requires-Dist: sqlalchemy
 
 
 otel tracing
```

