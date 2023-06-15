# Comparing `tmp/wand-ai-client-0.0.8.tar.gz` & `tmp/wand-ai-client-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wand-ai-client-0.0.8.tar", last modified: Wed Jun 14 14:58:25 2023, max compression
+gzip compressed data, was "wand-ai-client-0.0.9.tar", last modified: Thu Jun 15 15:28:04 2023, max compression
```

## Comparing `wand-ai-client-0.0.8.tar` & `wand-ai-client-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-06-14 14:58:25.515448 wand-ai-client-0.0.8/
--rw-r--r--   0 romasku   (1000) romasku   (1000)      821 2023-06-14 14:58:25.515448 wand-ai-client-0.0.8/PKG-INFO
--rw-r--r--   0 romasku   (1000) romasku   (1000)      344 2023-06-12 15:17:19.000000 wand-ai-client-0.0.8/README.md
--rw-r--r--   0 romasku   (1000) romasku   (1000)      176 2023-05-27 16:26:52.000000 wand-ai-client-0.0.8/pyproject.toml
--rw-r--r--   0 romasku   (1000) romasku   (1000)     1859 2023-06-14 14:58:25.515448 wand-ai-client-0.0.8/setup.cfg
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-06-14 14:58:25.515448 wand-ai-client-0.0.8/wand_ai_client.egg-info/
--rw-r--r--   0 romasku   (1000) romasku   (1000)      821 2023-06-14 14:58:25.000000 wand-ai-client-0.0.8/wand_ai_client.egg-info/PKG-INFO
--rw-r--r--   0 romasku   (1000) romasku   (1000)      508 2023-06-14 14:58:25.000000 wand-ai-client-0.0.8/wand_ai_client.egg-info/SOURCES.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-06-14 14:58:25.000000 wand-ai-client-0.0.8/wand_ai_client.egg-info/dependency_links.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)       54 2023-06-14 14:58:25.000000 wand-ai-client-0.0.8/wand_ai_client.egg-info/entry_points.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-05-27 19:56:31.000000 wand-ai-client-0.0.8/wand_ai_client.egg-info/not-zip-safe
--rw-r--r--   0 romasku   (1000) romasku   (1000)      227 2023-06-14 14:58:25.000000 wand-ai-client-0.0.8/wand_ai_client.egg-info/requires.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)       12 2023-06-14 14:58:25.000000 wand-ai-client-0.0.8/wand_ai_client.egg-info/top_level.txt
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-06-14 14:58:25.515448 wand-ai-client-0.0.8/wand_client/
--rw-r--r--   0 romasku   (1000) romasku   (1000)       21 2023-06-14 14:03:00.000000 wand-ai-client-0.0.8/wand_client/__init__.py
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-06-14 14:58:25.515448 wand-ai-client-0.0.8/wand_client/cli/
--rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:55:30.000000 wand-ai-client-0.0.8/wand_client/cli/__init__.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     1161 2023-06-01 09:24:47.000000 wand-ai-client-0.0.8/wand_client/cli/config.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     3043 2023-05-29 13:18:26.000000 wand-ai-client-0.0.8/wand_client/cli/formatters.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     5512 2023-06-14 14:04:35.000000 wand-ai-client-0.0.8/wand_client/cli/main.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     2773 2023-05-29 14:03:37.000000 wand-ai-client-0.0.8/wand_client/jupyter.py
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-06-14 14:58:25.515448 wand-ai-client-0.0.8/wand_client/sdk/
--rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:04:20.000000 wand-ai-client-0.0.8/wand_client/sdk/__init__.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     5795 2023-06-13 13:52:34.000000 wand-ai-client-0.0.8/wand_client/sdk/core.py
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-06-15 15:28:04.251881 wand-ai-client-0.0.9/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      821 2023-06-15 15:28:04.251881 wand-ai-client-0.0.9/PKG-INFO
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      344 2023-06-12 15:17:19.000000 wand-ai-client-0.0.9/README.md
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      176 2023-05-27 16:26:52.000000 wand-ai-client-0.0.9/pyproject.toml
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     1859 2023-06-15 15:28:04.255215 wand-ai-client-0.0.9/setup.cfg
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-06-15 15:28:04.251881 wand-ai-client-0.0.9/wand_ai_client.egg-info/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      821 2023-06-15 15:28:04.000000 wand-ai-client-0.0.9/wand_ai_client.egg-info/PKG-INFO
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      508 2023-06-15 15:28:04.000000 wand-ai-client-0.0.9/wand_ai_client.egg-info/SOURCES.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-06-15 15:28:04.000000 wand-ai-client-0.0.9/wand_ai_client.egg-info/dependency_links.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)       54 2023-06-15 15:28:04.000000 wand-ai-client-0.0.9/wand_ai_client.egg-info/entry_points.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-05-27 19:56:31.000000 wand-ai-client-0.0.9/wand_ai_client.egg-info/not-zip-safe
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      227 2023-06-15 15:28:04.000000 wand-ai-client-0.0.9/wand_ai_client.egg-info/requires.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)       12 2023-06-15 15:28:04.000000 wand-ai-client-0.0.9/wand_ai_client.egg-info/top_level.txt
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-06-15 15:28:04.251881 wand-ai-client-0.0.9/wand_client/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)       22 2023-06-15 15:27:40.000000 wand-ai-client-0.0.9/wand_client/__init__.py
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-06-15 15:28:04.251881 wand-ai-client-0.0.9/wand_client/cli/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:55:30.000000 wand-ai-client-0.0.9/wand_client/cli/__init__.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     1161 2023-06-01 09:24:47.000000 wand-ai-client-0.0.9/wand_client/cli/config.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     4992 2023-06-15 15:25:29.000000 wand-ai-client-0.0.9/wand_client/cli/formatters.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     6793 2023-06-15 14:59:45.000000 wand-ai-client-0.0.9/wand_client/cli/main.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     2773 2023-05-29 14:03:37.000000 wand-ai-client-0.0.9/wand_client/jupyter.py
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-06-15 15:28:04.251881 wand-ai-client-0.0.9/wand_client/sdk/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:04:20.000000 wand-ai-client-0.0.9/wand_client/sdk/__init__.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     7637 2023-06-15 15:17:12.000000 wand-ai-client-0.0.9/wand_client/sdk/core.py
```

### Comparing `wand-ai-client-0.0.8/PKG-INFO` & `wand-ai-client-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wand-ai-client
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wand AI API client
 Author: Wand.AI Team
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `wand-ai-client-0.0.8/setup.cfg` & `wand-ai-client-0.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wand-ai-client
-version = 0.0.8
+version = 0.0.9
 description = Wand AI API client
 author = Wand.AI Team
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
```

### Comparing `wand-ai-client-0.0.8/wand_ai_client.egg-info/PKG-INFO` & `wand-ai-client-0.0.9/wand_ai_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wand-ai-client
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wand AI API client
 Author: Wand.AI Team
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `wand-ai-client-0.0.8/wand_client/cli/config.py` & `wand-ai-client-0.0.9/wand_client/cli/config.py`

 * *Files identical despite different names*

### Comparing `wand-ai-client-0.0.8/wand_client/cli/formatters.py` & `wand-ai-client-0.0.9/wand_client/cli/formatters.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,21 @@
 
 from rich import box
 from rich.console import RenderableType
 from rich.progress import Progress
 from rich.table import Table
 
 from wand_client.cli.config import WandCliSettings
-from wand_client.sdk.core import Model, Source, TrainingListener
+from wand_client.sdk.core import (
+    Model,
+    ReTrainingListener,
+    Source,
+    Training,
+    TrainingListener,
+)
 
 
 class SettingsFormatter:
     def __call__(self, settings: WandCliSettings) -> RenderableType:
         table = Table(
             box=None,
             show_header=False,
@@ -81,14 +87,68 @@
 
 
 class RichProgressListener(TrainingListener):
     def __init__(self, progress: Progress) -> None:
         self._progress = progress
         self._task = progress.add_task("Training model")
 
-    def on_model_progress(self, model: Model) -> None:
+    def on_progress(self, model: Model) -> None:
         self._progress.update(
             self._task,
             completed=model.status.progress,
             description=f"Training model {model.id}",
         )
         self._progress.refresh()
+
+
+class RichRetrainProgressListener(ReTrainingListener):
+    def __init__(self, progress: Progress) -> None:
+        self._progress = progress
+        self._task = progress.add_task("Re-training model")
+
+    def on_progress(self, training: Training) -> None:
+        self._progress.update(
+            self._task,
+            completed=training.status.progress,
+            description=f"Re-training model {training.model_id}",
+        )
+        self._progress.refresh()
+
+
+class TrainingFormatter:
+    def __call__(self, training: Training) -> RenderableType:
+        table = Table(
+            box=None,
+            show_header=False,
+            show_edge=False,
+        )
+        table.add_column()
+        table.add_column(style="bold")
+        table.add_row("Id", training.id)
+        table.add_row("Model Id", training.model_id)
+        table.add_row("Progress", str(training.status.progress))
+        table.add_row("Training completed", str(training.status.training_completed))
+        return table
+
+
+class TrainingsFormatter:
+    def _training_to_table_row(self, training: Training) -> Sequence[str]:
+        line = [
+            training.id,
+            training.model_id,
+            str(training.status.progress),
+            str(training.status.training_completed),
+        ]
+        return line
+
+    def __call__(self, trainings: Sequence[Training]) -> RenderableType:
+        trainings = sorted(trainings, key=operator.attrgetter("id"))
+        table = Table(box=box.SIMPLE_HEAVY)
+        # make sure that the first column is fully expanded
+        width = len("1ce961e5172a688b842d")
+        table.add_column("Id", style="bold", width=width)
+        table.add_column("Model Id")
+        table.add_column("Progress")
+        table.add_column("Training Completed")
+        for training in trainings:
+            table.add_row(*self._training_to_table_row(training))
+        return table
```

### Comparing `wand-ai-client-0.0.8/wand_client/cli/main.py` & `wand-ai-client-0.0.9/wand_client/cli/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,16 +9,19 @@
 from rich.progress import Progress
 
 from wand_client import __version__
 from wand_client.cli.config import CONFIG_PATH, WandCliSettings
 from wand_client.cli.formatters import (
     ModelFormatter,
     ModelsFormatter,
+    RichRetrainProgressListener,
     SettingsFormatter,
     SourceFormatter,
+    TrainingFormatter,
+    TrainingsFormatter,
 )
 from wand_client.sdk.core import Model, TrainingListener, WandClient
 
 
 class Root:
     def __init__(self, option_settings: Dict[str, Any]) -> None:
         self._option_settings = option_settings
@@ -129,15 +132,15 @@
     """Upload a file as a source"""
     client: WandClient = ctx.obj.get_client()
 
     with Progress() as progress:
         task = progress.add_task("Training model")
 
         class _Listener(TrainingListener):
-            def on_model_progress(self, model: Model) -> None:
+            def on_progress(self, model: Model) -> None:
                 progress.update(
                     task,
                     completed=model.status.progress,
                     description=f"Training model {model.id}",
                 )
                 progress.refresh()
 
@@ -161,14 +164,31 @@
 def delete(ctx: Context, model_id: str) -> None:
     """Get info about model by ID"""
     client: WandClient = ctx.obj.get_client()
     client.models.delete(model_id=model_id)
     rich.print("Model deleted")
 
 
+@model.command()
+@click.argument("model_id", type=click.STRING)
+@click.pass_context
+def retrain(ctx: Context, model_id: str) -> None:
+    """Upload a file as a source"""
+    client: WandClient = ctx.obj.get_client()
+
+    with Progress() as progress:
+        training = client.models.retrain(
+            model_id, listener=RichRetrainProgressListener(progress)
+        )
+        rich.print(
+            f"Training of model {training.model_id} with "
+            f"training id {training.id} finished"
+        )
+
+
 @model.command(name="list")
 @click.pass_context
 def list_(ctx: Context) -> None:
     """List all models"""
     client: WandClient = ctx.obj.get_client()
     models = client.models.list_all()
     rich.print(ModelsFormatter()(models))
@@ -191,9 +211,35 @@
         if prompt_text == "exit":
             return
         with console.status("Generating answer...", spinner="bouncingBall"):
             resp = chat.ask(prompt_text)
         console.print(resp, style="bold")
 
 
+@cli.group()
+def training() -> None:
+    """
+    Operations with ml trainings
+    """
+
+
+@training.command(name="get")
+@click.argument("training_id", type=click.STRING)
+@click.pass_context
+def get_training(ctx: Context, training_id: str) -> None:
+    """Get info about training by ID"""
+    client: WandClient = ctx.obj.get_client()
+    training = client.trainings.get(training_id=training_id)
+    rich.print(TrainingFormatter()(training))
+
+
+@training.command(name="list")
+@click.pass_context
+def list_training(ctx: Context) -> None:
+    """List all training"""
+    client: WandClient = ctx.obj.get_client()
+    models = client.trainings.list_all()
+    rich.print(TrainingsFormatter()(models))
+
+
 if __name__ == "__main__":
     cli()
```

### Comparing `wand-ai-client-0.0.8/wand_client/jupyter.py` & `wand-ai-client-0.0.9/wand_client/jupyter.py`

 * *Files identical despite different names*

### Comparing `wand-ai-client-0.0.8/wand_client/sdk/core.py` & `wand-ai-client-0.0.9/wand_client/sdk/core.py`

 * *Files 17% similar despite different names*

```diff
@@ -87,34 +87,77 @@
 
 class Model(BaseModel):
     id: str
     source_ids: List[str]
     status: ModelStatus
 
 
+class Training(BaseModel):
+    id: str
+    model_id: str
+    status: ModelStatus
+
+
 class ChatMessageAuthor(str, enum.Enum):
     AI = "ai"
     HUMAN = "human"
 
 
 class ChatMessage(BaseModel):
     author: ChatMessageAuthor
     message: str
 
 
 class TrainingListener(abc.ABC):
     @abc.abstractmethod
-    def on_model_progress(self, model: Model) -> None:
+    def on_progress(self, model: Model) -> None:
         pass
 
 
-class Models:
+class ReTrainingListener(abc.ABC):
+    @abc.abstractmethod
+    def on_progress(self, training: Training) -> None:
+        pass
+
+
+def _parse_training_payload(payload: Mapping[str, Any]) -> Training:
+    return Training(
+        id=payload["train_id"],
+        model_id=payload["model_id"],
+        status=ModelStatus(
+            progress=payload["status"]["progress"],
+            training_completed=payload["status"]["training_completed"],
+        ),
+    )
+
+
+class Trainings:
     def __init__(self, core: WandCoreClient) -> None:
         self._core = core
 
+    def get(self, training_id: str) -> Training:
+        res = self._core.request(
+            method="GET",
+            path=f"/trainings/{training_id}",
+        ).json()
+        return _parse_training_payload(res)
+
+    def list_all(self) -> List[Training]:
+        res = self._core.request(
+            method="GET",
+            path=f"/trainings",
+        ).json()
+        return [_parse_training_payload(it) for it in res]
+
+
+class Models:
+    def __init__(self, core: WandCoreClient, trainings: Trainings) -> None:
+        self._core = core
+        self._trainings = trainings
+
     def _parse_model_payload(self, payload: Mapping[str, Any]) -> Model:
         return Model(
             id=payload["model_id"],
             source_ids=payload["source_ids"],
             status=ModelStatus(
                 progress=payload["status"]["progress"],
                 training_completed=payload["status"]["training_completed"],
@@ -127,14 +170,22 @@
             path="/models",
             json={
                 "source_ids": source_ids,
             },
         ).json()
         return self._parse_model_payload(res)
 
+    def start_retraining(self, model_id: str) -> Training:
+        res = self._core.request(
+            method="POST",
+            path=f"/models/{model_id}/train",
+            json={},
+        ).json()
+        return _parse_training_payload(res)
+
     def get(self, model_id: str) -> Model:
         res = self._core.request(
             method="GET",
             path=f"/models/{model_id}",
         ).json()
         return self._parse_model_payload(res)
 
@@ -173,19 +224,31 @@
     def train(
         self, source_ids: List[str], listener: Optional[TrainingListener] = None
     ) -> Model:
         model = self.start_training(source_ids)
         while True:
             model = self.get(model.id)
             if listener:
-                listener.on_model_progress(model)
+                listener.on_progress(model)
             if model.status.training_completed:
                 return model
             time.sleep(1)
 
+    def retrain(
+        self, model_id: str, listener: Optional[ReTrainingListener] = None
+    ) -> Training:
+        training = self.start_retraining(model_id)
+        while True:
+            training = self._trainings.get(training.id)
+            if listener:
+                listener.on_progress(training)
+            if training.status.training_completed:
+                return training
+            time.sleep(1)
+
     def start_chat(self, model_id: str) -> "ChatSession":
         return ChatSession(model_id, self)
 
 
 class ChatSession:
     def __init__(self, model_id: str, client: Models) -> None:
         self._model_id = model_id
@@ -207,8 +270,9 @@
     def __init__(
         self,
         token: str,
         base_url: str,
     ):
         core = WandCoreClient(token=token, base_url=base_url)
         self.source = Sources(core)
-        self.models = Models(core)
+        self.trainings = Trainings(core)
+        self.models = Models(core, self.trainings)
```

