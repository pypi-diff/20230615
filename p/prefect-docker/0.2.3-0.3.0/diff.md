# Comparing `tmp/prefect-docker-0.2.3.tar.gz` & `tmp/prefect-docker-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-docker/prefect-docker/dist/.tmp-es7vqrnd/prefect-docker-0.2.3.tar", last modified: Mon May  8 17:53:45 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-docker/prefect-docker/dist/.tmp-q5zy82mj/prefect-docker-0.3.0.tar", last modified: Thu Jun 15 14:32:04 2023, max compression
```

## Comparing `prefect-docker-0.2.3.tar` & `prefect-docker-0.3.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/prefect_docker/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/prefect_docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/prefect_docker/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/prefect_docker/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/prefect_docker/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/prefect_docker/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/prefect_docker/images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/prefect_docker/projects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/prefect_docker/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/prefect_docker/projects/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    28174 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/prefect_docker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/prefect_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/prefect_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/prefect_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/prefect_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/prefect_docker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/prefect_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/prefect_docker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/tests/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/tests/test_host.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (123)    44087 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/prefect_docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/prefect_docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/prefect_docker/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/prefect_docker/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/prefect_docker/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/prefect_docker/deployments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/prefect_docker/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/prefect_docker/deployments/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/prefect_docker/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/prefect_docker/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29217 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/prefect_docker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/prefect_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/prefect_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/prefect_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/prefect_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/prefect_docker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/prefect_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/prefect_docker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/tests/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/tests/test_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45011 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/versioneer.py
```

### Comparing `prefect-docker-0.2.3/LICENSE` & `prefect-docker-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.3/PKG-INFO` & `prefect-docker-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-docker
-Version: 0.2.3
+Version: 0.3.0
 Summary: Prefect integrations for working with Docker
 Home-page: https://github.com/PrefectHQ/prefect-docker
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-docker-0.2.3/README.md` & `prefect-docker-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.3/prefect_docker/containers.py` & `prefect-docker-0.3.0/prefect_docker/containers.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.3/prefect_docker/credentials.py` & `prefect-docker-0.3.0/prefect_docker/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.3/prefect_docker/host.py` & `prefect-docker-0.3.0/prefect_docker/host.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.3/prefect_docker/images.py` & `prefect-docker-0.3.0/prefect_docker/images.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.3/prefect_docker/worker.py` & `prefect-docker-0.3.0/prefect_docker/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,25 +30,25 @@
 import docker.errors
 import packaging.version
 import prefect
 from docker import DockerClient
 from docker.models.containers import Container
 from prefect.client.orchestration import ServerType, get_client
 from prefect.client.schemas import FlowRun
-from prefect.docker import (
-    format_outlier_version_name,
-    get_prefect_image_name,
-    parse_image_tag,
-)
 from prefect.events import Event, RelatedResource, emit_event
 from prefect.exceptions import InfrastructureNotAvailable, InfrastructureNotFound
 from prefect.server.schemas.core import Flow
 from prefect.server.schemas.responses import DeploymentResponse
 from prefect.settings import PREFECT_API_URL
 from prefect.utilities.asyncutils import run_sync_in_worker_thread
+from prefect.utilities.dockerutils import (
+    format_outlier_version_name,
+    get_prefect_image_name,
+    parse_image_tag,
+)
 from prefect.workers.base import BaseJobConfiguration, BaseWorker, BaseWorkerResult
 from pydantic import Field, validator
 from slugify import slugify
 from typing_extensions import Literal
 
 CONTAINER_LABELS = {
     "io.prefect.version": prefect.__version__,
@@ -360,14 +360,23 @@
 
 
 class DockerWorker(BaseWorker):
     """Prefect worker that executes flow runs within Docker containers."""
 
     type = "docker"
     job_configuration = DockerWorkerJobConfiguration
+    _description = (
+        "Execute flow runs within Docker containers. Works well for managing flow "
+        "execution environments via Docker images. Requires access to a running "
+        "Docker daemon."
+    )
+    _display_name = "Docker"
+    _documentation_url = "https://prefecthq.github.io/prefect-docker/worker/"
+    _is_beta = True
+    _logo_url = "https://images.ctfassets.net/gm98wzqotmnx/2IfXXfMq66mrzJBDFFCHTp/6d8f320d9e4fc4393f045673d61ab612/Moby-logo.png?h=250"  # noqa
 
     def __init__(self, *args: Any, test_mode: bool = None, **kwargs: Any) -> None:
         if test_mode is None:
             self.test_mode = bool(os.getenv("PREFECT_DOCKER_TEST_MODE", False))
         else:
             self.test_mode = test_mode
         super().__init__(*args, **kwargs)
@@ -530,15 +539,19 @@
             docker_client, configuration
         )
 
         if self._should_pull_image(docker_client, configuration=configuration):
             self._logger.info(f"Pulling image {configuration.image!r}...")
             self._pull_image(docker_client, configuration)
 
-        container = self._create_container(docker_client, **container_settings)
+        try:
+            container = self._create_container(docker_client, **container_settings)
+        except Exception as exc:
+            self._emit_container_creation_failed_event(configuration)
+            raise exc
 
         created_event = self._emit_container_status_change_event(
             container, configuration
         )
 
         # Add additional networks after the container is created; only one network can
         # be attached at creation time
@@ -710,28 +723,36 @@
     def _container_as_resource(self, container: "Container") -> Dict[str, str]:
         """Convert a container to a resource dictionary"""
         return {
             "prefect.resource.id": f"prefect.docker.container.{container.id}",
             "prefect.resource.name": container.name,
         }
 
+    def _emit_container_creation_failed_event(
+        self, configuration: DockerWorkerJobConfiguration
+    ) -> Event:
+        """Emit a Prefect event when a docker container fails to be created."""
+        return emit_event(
+            event="prefect.docker.container.creation-failed",
+            resource=self._event_resource(),
+            related=self._event_related_resources(configuration=configuration),
+        )
+
     def _emit_container_status_change_event(
         self,
         container: "Container",
         configuration: DockerWorkerJobConfiguration,
         last_event: Optional[Event] = None,
     ) -> Event:
         """Emit a Prefect event for a Docker container event."""
-        resource = self._container_as_resource(container)
-
         related = self._event_related_resources(configuration=configuration)
 
         worker_resource = self._event_resource()
         worker_resource["prefect.resource.role"] = "worker"
         worker_related_resource = RelatedResource(__root__=worker_resource)
 
         return emit_event(
             event=f"prefect.docker.container.{container.status.lower()}",
-            resource=resource,
+            resource=self._container_as_resource(container),
             related=related + [worker_related_resource],
             follows=last_event,
         )
```

### Comparing `prefect-docker-0.2.3/prefect_docker.egg-info/PKG-INFO` & `prefect-docker-0.3.0/prefect_docker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-docker
-Version: 0.2.3
+Version: 0.3.0
 Summary: Prefect integrations for working with Docker
 Home-page: https://github.com/PrefectHQ/prefect-docker
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-docker-0.2.3/prefect_docker.egg-info/SOURCES.txt` & `prefect-docker-0.3.0/prefect_docker.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 prefect_docker/worker.py
 prefect_docker.egg-info/PKG-INFO
 prefect_docker.egg-info/SOURCES.txt
 prefect_docker.egg-info/dependency_links.txt
 prefect_docker.egg-info/entry_points.txt
 prefect_docker.egg-info/requires.txt
 prefect_docker.egg-info/top_level.txt
-prefect_docker/projects/__init__.py
-prefect_docker/projects/steps.py
+prefect_docker/deployments/__init__.py
+prefect_docker/deployments/steps.py
 tests/test_containers.py
 tests/test_credentials.py
 tests/test_host.py
 tests/test_images.py
 tests/test_worker.py
```

### Comparing `prefect-docker-0.2.3/setup.cfg` & `prefect-docker-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.3/setup.py` & `prefect-docker-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.3/tests/test_containers.py` & `prefect-docker-0.3.0/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.3/tests/test_host.py` & `prefect-docker-0.3.0/tests/test_host.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.3/tests/test_images.py` & `prefect-docker-0.3.0/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.3/tests/test_worker.py` & `prefect-docker-0.3.0/tests/test_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 @pytest.fixture
 def default_docker_worker_job_configuration():
     return DockerWorkerJobConfiguration()
 
 
 @pytest.fixture
 def flow_run():
-    return FlowRun()
+    return FlowRun(flow_id=uuid.uuid4())
 
 
 @pytest.mark.parametrize(
     "requested_name,container_name",
     [
         ("_flow_run", "flow_run"),
         ("...flow_run", "flow_run"),
@@ -1152,7 +1152,33 @@
                     "prefect.resource.name": "fake-name",
                 },
                 related=[worker_related_resource],
                 follows=2,
             ),
         ]
     )
+
+
+async def test_emits_event_container_creation_failure(
+    mock_docker_client, flow_run, default_docker_worker_job_configuration
+):
+    import docker.errors
+
+    mock_docker_client.containers.create.side_effect = docker.errors.APIError(
+        "test error"
+    )
+
+    worker_resource = None
+    with patch("prefect_docker.worker.emit_event") as mock_emit:
+        with pytest.raises(docker.errors.APIError, match="test error"):
+            async with DockerWorker(work_pool_name="test") as worker:
+                worker_resource = worker._event_resource()
+                await worker.run(
+                    flow_run=flow_run,
+                    configuration=default_docker_worker_job_configuration,
+                )
+
+        mock_emit.assert_called_once_with(
+            event="prefect.docker.container.creation-failed",
+            resource=worker_resource,
+            related=[],
+        )
```

### Comparing `prefect-docker-0.2.3/versioneer.py` & `prefect-docker-0.3.0/versioneer.py`

 * *Files identical despite different names*

