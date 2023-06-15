# Comparing `tmp/alphawave-0.2.3.tar.gz` & `tmp/alphawave-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphawave-0.2.3.tar", last modified: Wed Jun 14 16:02:16 2023, max compression
+gzip compressed data, was "alphawave-0.2.4.tar", last modified: Thu Jun 15 20:03:28 2023, max compression
```

## Comparing `alphawave-0.2.3.tar` & `alphawave-0.2.4.tar`

### file list

```diff
@@ -1,66 +1,50 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-14 16:02:16.252409 alphawave-0.2.3/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.2.3/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7742 2023-06-14 16:02:16.252409 alphawave-0.2.3/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7129 2023-06-10 04:04:27.000000 alphawave-0.2.3/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      849 2023-06-14 15:58:56.000000 alphawave-0.2.3/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-14 16:02:16.252409 alphawave-0.2.3/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-14 16:02:16.244409 alphawave-0.2.3/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-14 16:02:16.248409 alphawave-0.2.3/src/alphawave/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8822 2023-06-11 19:08:17.000000 alphawave-0.2.3/src/alphawave/AlphaWave.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.2.3/src/alphawave/Colorize.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      711 2023-06-11 16:07:13.000000 alphawave-0.2.3/src/alphawave/DefaultResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4975 2023-06-11 19:09:29.000000 alphawave-0.2.3/src/alphawave/JSONResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7236 2023-06-11 19:10:18.000000 alphawave-0.2.3/src/alphawave/LLMClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      545 2023-06-03 22:27:04.000000 alphawave-0.2.3/src/alphawave/MemoryFork.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7966 2023-06-11 19:12:11.000000 alphawave-0.2.3/src/alphawave/OSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8572 2023-06-11 18:41:22.000000 alphawave-0.2.3/src/alphawave/OpenAIClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3007 2023-06-11 03:54:19.000000 alphawave-0.2.3/src/alphawave/Response.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      788 2023-06-10 03:00:13.000000 alphawave-0.2.3/src/alphawave/TestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1503 2023-06-09 18:41:13.000000 alphawave-0.2.3/src/alphawave/TestClientTest.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.2.3/src/alphawave/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1347 2023-06-13 18:50:06.000000 alphawave-0.2.3/src/alphawave/alphawaveTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.2.3/src/alphawave/internalTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.2.3/src/alphawave/jsonParser.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2745 2023-06-07 18:39:44.000000 alphawave-0.2.3/src/alphawave/utilityV2.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-14 16:02:16.248409 alphawave-0.2.3/src/alphawave.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7742 2023-06-14 16:02:16.000000 alphawave-0.2.3/src/alphawave.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1775 2023-06-14 16:02:16.000000 alphawave-0.2.3/src/alphawave.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-14 16:02:16.000000 alphawave-0.2.3/src/alphawave.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       86 2023-06-14 16:02:16.000000 alphawave-0.2.3/src/alphawave.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       36 2023-06-14 16:02:16.000000 alphawave-0.2.3/src/alphawave.egg-info/top_level.txt
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-14 16:02:16.248409 alphawave-0.2.3/src/alphawave_agents/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    17857 2023-06-11 20:59:20.000000 alphawave-0.2.3/src/alphawave_agents/Agent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1332 2023-06-11 16:22:40.000000 alphawave-0.2.3/src/alphawave_agents/AgentCommandSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2464 2023-06-11 20:48:55.000000 alphawave-0.2.3/src/alphawave_agents/AgentCommandValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1428 2023-06-11 19:07:37.000000 alphawave-0.2.3/src/alphawave_agents/AskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.2.3/src/alphawave_agents/CompleteTaskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.2.3/src/alphawave_agents/ConfirmAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1386 2023-06-07 02:55:09.000000 alphawave-0.2.3/src/alphawave_agents/FinalAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1509 2023-06-07 03:15:08.000000 alphawave-0.2.3/src/alphawave_agents/MathCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3142 2023-06-11 20:47:19.000000 alphawave-0.2.3/src/alphawave_agents/PromptCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3553 2023-06-11 03:56:28.000000 alphawave-0.2.3/src/alphawave_agents/SchemaBasedCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.2.3/src/alphawave_agents/SentimentAnalysis.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.2.3/src/alphawave_agents/SetPropertyCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.2.3/src/alphawave_agents/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1686 2023-06-10 21:45:49.000000 alphawave-0.2.3/src/alphawave_agents/agentTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-14 16:02:16.248409 alphawave-0.2.3/src/aphawave/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8822 2023-06-11 19:08:17.000000 alphawave-0.2.3/src/aphawave/AlphaWave.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.2.3/src/aphawave/Colorize.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      711 2023-06-11 16:07:13.000000 alphawave-0.2.3/src/aphawave/DefaultResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4975 2023-06-11 19:09:29.000000 alphawave-0.2.3/src/aphawave/JSONResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7236 2023-06-11 19:10:18.000000 alphawave-0.2.3/src/aphawave/LLMClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      545 2023-06-03 22:27:04.000000 alphawave-0.2.3/src/aphawave/MemoryFork.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7966 2023-06-11 19:12:11.000000 alphawave-0.2.3/src/aphawave/OSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8572 2023-06-11 18:41:22.000000 alphawave-0.2.3/src/aphawave/OpenAIClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3007 2023-06-11 03:54:19.000000 alphawave-0.2.3/src/aphawave/Response.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      788 2023-06-10 03:00:13.000000 alphawave-0.2.3/src/aphawave/TestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1503 2023-06-09 18:41:13.000000 alphawave-0.2.3/src/aphawave/TestClientTest.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.2.3/src/aphawave/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1347 2023-06-13 18:50:06.000000 alphawave-0.2.3/src/aphawave/alphawaveTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.2.3/src/aphawave/internalTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.2.3/src/aphawave/jsonParser.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2745 2023-06-07 18:39:44.000000 alphawave-0.2.3/src/aphawave/utilityV2.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-14 16:02:16.252409 alphawave-0.2.3/tests/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.2.3/tests/testOSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14653 2023-06-07 04:29:45.000000 alphawave-0.2.3/tests/testOpenAiClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      948 2023-06-06 20:59:59.000000 alphawave-0.2.3/tests/testSchema.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-15 20:03:28.144310 alphawave-0.2.4/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.2.4/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7742 2023-06-15 20:03:28.144310 alphawave-0.2.4/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7129 2023-06-10 04:04:27.000000 alphawave-0.2.4/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      849 2023-06-15 20:03:13.000000 alphawave-0.2.4/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-15 20:03:28.144310 alphawave-0.2.4/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-15 20:03:28.140310 alphawave-0.2.4/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-15 20:03:28.144310 alphawave-0.2.4/src/alphawave/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9229 2023-06-15 03:36:54.000000 alphawave-0.2.4/src/alphawave/AlphaWave.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.2.4/src/alphawave/Colorize.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      723 2023-06-15 04:11:00.000000 alphawave-0.2.4/src/alphawave/DefaultResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5982 2023-06-15 20:01:04.000000 alphawave-0.2.4/src/alphawave/JSONResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7236 2023-06-11 19:10:18.000000 alphawave-0.2.4/src/alphawave/LLMClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      545 2023-06-03 22:27:04.000000 alphawave-0.2.4/src/alphawave/MemoryFork.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7966 2023-06-11 19:12:11.000000 alphawave-0.2.4/src/alphawave/OSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8572 2023-06-11 18:41:22.000000 alphawave-0.2.4/src/alphawave/OpenAIClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-06-15 04:11:41.000000 alphawave-0.2.4/src/alphawave/RepairTestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 04:11:51.000000 alphawave-0.2.4/src/alphawave/Response.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.2.4/src/alphawave/TestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.2.4/src/alphawave/TestClientTest.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.2.4/src/alphawave/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1359 2023-06-15 04:10:27.000000 alphawave-0.2.4/src/alphawave/alphawaveTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.2.4/src/alphawave/internalTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.2.4/src/alphawave/jsonParser.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2745 2023-06-07 18:39:44.000000 alphawave-0.2.4/src/alphawave/utilityV2.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-15 20:03:28.144310 alphawave-0.2.4/src/alphawave.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7742 2023-06-15 20:03:28.000000 alphawave-0.2.4/src/alphawave.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1350 2023-06-15 20:03:28.000000 alphawave-0.2.4/src/alphawave.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-15 20:03:28.000000 alphawave-0.2.4/src/alphawave.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       86 2023-06-15 20:03:28.000000 alphawave-0.2.4/src/alphawave.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       27 2023-06-15 20:03:28.000000 alphawave-0.2.4/src/alphawave.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-15 20:03:28.144310 alphawave-0.2.4/src/alphawave_agents/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    16240 2023-06-15 18:47:04.000000 alphawave-0.2.4/src/alphawave_agents/Agent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1332 2023-06-11 16:22:40.000000 alphawave-0.2.4/src/alphawave_agents/AgentCommandSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2637 2023-06-15 18:44:50.000000 alphawave-0.2.4/src/alphawave_agents/AgentCommandValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1428 2023-06-11 19:07:37.000000 alphawave-0.2.4/src/alphawave_agents/AskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.2.4/src/alphawave_agents/CompleteTaskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.2.4/src/alphawave_agents/ConfirmAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1386 2023-06-07 02:55:09.000000 alphawave-0.2.4/src/alphawave_agents/FinalAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1509 2023-06-07 03:15:08.000000 alphawave-0.2.4/src/alphawave_agents/MathCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3130 2023-06-15 19:13:49.000000 alphawave-0.2.4/src/alphawave_agents/PromptCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3553 2023-06-11 03:56:28.000000 alphawave-0.2.4/src/alphawave_agents/SchemaBasedCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.2.4/src/alphawave_agents/SentimentAnalysis.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.2.4/src/alphawave_agents/SetPropertyCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.2.4/src/alphawave_agents/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1686 2023-06-10 21:45:49.000000 alphawave-0.2.4/src/alphawave_agents/agentTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-15 20:03:28.144310 alphawave-0.2.4/tests/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.2.4/tests/testOSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14653 2023-06-07 04:29:45.000000 alphawave-0.2.4/tests/testOpenAiClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      948 2023-06-06 20:59:59.000000 alphawave-0.2.4/tests/testSchema.py
```

### Comparing `alphawave-0.2.3/LICENSE` & `alphawave-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.3/PKG-INFO` & `alphawave-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.2.3
+Version: 0.2.4
 Summary: AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://github.com/Stevenic/alphawave-py
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.2.3/README.md` & `alphawave-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.3/pyproject.toml` & `alphawave-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alphawave"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)"
```

### Comparing `alphawave-0.2.3/src/alphawave/AlphaWave.py` & `alphawave-0.2.4/src/alphawave/AlphaWave.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,21 @@
     logRepairs: bool = False
 
 def update_dataclass(instance, **kwargs):
     for key, value in kwargs.items():
         if hasattr(instance, key):
             setattr(instance, key, value)
 
+def display_dataclass(obj):
+    print ('\n ', obj)
+    for attr_name in dir(obj):
+        if not attr_name.startswith('__'):  # Exclude dunder (double underscore) attributes
+            attr_value = getattr(obj, attr_name)
+            print(f"    {attr_name}: {attr_value}")
+
 def get_values(instance, keys):
     values = []
     for key in keys:
         if hasattr(instance, key):
             values.append(getattr(instance, key))
         else:
             values.append(None)
@@ -119,22 +126,24 @@
         except Exception as err:
             return {
                 'status': 'error',
                 'message': str(err)
             }
 
     def addInputToHistory(self, memory, variable, input):
+        #print(f'***** Alphawave addInputToHistory {variable}')
         if variable and input is not None and len(input) > 0:
             history = memory.get(variable) or []
             history.append({'role': 'user', 'content': input})
             if len(history) > self.options.max_history_messages:
                 history = history[self.options.max_history_messages:]
             memory.set(variable, history)
 
     def addResponseToHistory(self, memory, variable, message):
+        #print(f'***** Alphawave addResponseToHistory {variable}')
         if variable:
             history = memory.get(variable) or []
             history.append(message)
             if len(history) > self.options.max_history_messages:
                 history = history[self.options.max_history_messages:]
             memory.set(variable, history)
```

### Comparing `alphawave-0.2.3/src/alphawave/Colorize.py` & `alphawave-0.2.4/src/alphawave/Colorize.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.3/src/alphawave/DefaultResponseValidator.py` & `alphawave-0.2.4/src/alphawave/DefaultResponseValidator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from promptrix.promptrixTypes import PromptFunctions, PromptMemory, Tokenizer
 from alphawave.alphawaveTypes import PromptResponse, Validation, PromptResponseValidator
+import json
 
 class DefaultResponseValidator(PromptResponseValidator):
     def validate_response(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, response: PromptResponse, remaining_attempts) -> Validation:
         self.feedback = response['message']['content'] if isinstance(response['message'], dict) else response.message
         return {
             'type': 'Validation',
             'valid': True,
```

### Comparing `alphawave-0.2.3/src/alphawave/LLMClient.py` & `alphawave-0.2.4/src/alphawave/LLMClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.3/src/alphawave/MemoryFork.py` & `alphawave-0.2.4/src/alphawave/MemoryFork.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.3/src/alphawave/OSClient.py` & `alphawave-0.2.4/src/alphawave/OSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.3/src/alphawave/OpenAIClient.py` & `alphawave-0.2.4/src/alphawave/OpenAIClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.3/src/alphawave/Response.py` & `alphawave-0.2.4/src/alphawave/Response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import re
+
 class Response:
     @staticmethod
     def parse_all_objects(text):
         objects = []
         if text is None:
             return objects
         lines = text.split('\n')
```

### Comparing `alphawave-0.2.3/src/alphawave/TestClient.py` & `alphawave-0.2.4/src/alphawave/TestClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Union
 from promptrix.promptrixTypes import PromptFunctions, PromptMemory, PromptSection, Tokenizer
 from  promptrix.promptrixTypes import Message
 from alphawave.alphawaveTypes import PromptCompletionClient, PromptCompletionOptions, PromptResponse, PromptResponseStatus
+import json
 
 class TestClient(PromptCompletionClient):
     def __init__(self, status: PromptResponseStatus = 'success', response: Union[str, Message] = {'role': 'assistant', 'content': "Hello World"}):
         self.status = status
         self.response = response
 
     async def completePrompt(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, prompt: PromptSection, options: PromptCompletionOptions) -> PromptResponse:
```

### Comparing `alphawave-0.2.3/src/alphawave/TestClientTest.py` & `alphawave-0.2.4/src/alphawave/TestClientTest.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from promptrix.FunctionRegistry import FunctionRegistry
 from promptrix.GPT3Tokenizer import  GPT3Tokenizer
 from promptrix.Prompt import Prompt
 
 from alphawave.alphawaveTypes import PromptCompletionOptions
 from alphawave.TestClient import TestClient
 import asyncio
+import json
 
 class TestClientTest(unittest.TestCase):
     def setUp(self):
         self.memory = VolatileMemory()
         self.functions = FunctionRegistry()
         self.tokenizer = GPT3Tokenizer()
         self.prompt = Prompt([])
```

### Comparing `alphawave-0.2.3/src/alphawave/alphawaveTypes.py` & `alphawave-0.2.4/src/alphawave/alphawaveTypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from dataclasses import dataclass
 from typing import Any, Optional, Union, List
+import json
 
 # Equivalent to TypeScript's import statement
 from promptrix.promptrixTypes import Message, PromptFunctions, PromptMemory, PromptSection, Tokenizer
 
 class PromptCompletionClient:
     def completePrompt(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, prompt: PromptSection, options: 'PromptCompletionOptions') -> 'Promise[PromptResponse]':
         pass
```

### Comparing `alphawave-0.2.3/src/alphawave/internalTypes.py` & `alphawave-0.2.4/src/alphawave/internalTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.3/src/alphawave/jsonParser.py` & `alphawave-0.2.4/src/alphawave/jsonParser.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.3/src/alphawave/utilityV2.py` & `alphawave-0.2.4/src/alphawave/utilityV2.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.3/src/alphawave.egg-info/PKG-INFO` & `alphawave-0.2.4/src/alphawave.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.2.3
+Version: 0.2.4
 Summary: AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://github.com/Stevenic/alphawave-py
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.2.3/src/alphawave.egg-info/SOURCES.txt` & `alphawave-0.2.4/src/alphawave.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/alphawave/Colorize.py
 src/alphawave/DefaultResponseValidator.py
 src/alphawave/JSONResponseValidator.py
 src/alphawave/LLMClient.py
 src/alphawave/MemoryFork.py
 src/alphawave/OSClient.py
 src/alphawave/OpenAIClient.py
+src/alphawave/RepairTestClient.py
 src/alphawave/Response.py
 src/alphawave/TestClient.py
 src/alphawave/TestClientTest.py
 src/alphawave/__init__.py
 src/alphawave/alphawaveTypes.py
 src/alphawave/internalTypes.py
 src/alphawave/jsonParser.py
@@ -32,26 +33,10 @@
 src/alphawave_agents/MathCommand.py
 src/alphawave_agents/PromptCommand.py
 src/alphawave_agents/SchemaBasedCommand.py
 src/alphawave_agents/SentimentAnalysis.py
 src/alphawave_agents/SetPropertyCommand.py
 src/alphawave_agents/__init__.py
 src/alphawave_agents/agentTypes.py
-src/aphawave/AlphaWave.py
-src/aphawave/Colorize.py
-src/aphawave/DefaultResponseValidator.py
-src/aphawave/JSONResponseValidator.py
-src/aphawave/LLMClient.py
-src/aphawave/MemoryFork.py
-src/aphawave/OSClient.py
-src/aphawave/OpenAIClient.py
-src/aphawave/Response.py
-src/aphawave/TestClient.py
-src/aphawave/TestClientTest.py
-src/aphawave/__init__.py
-src/aphawave/alphawaveTypes.py
-src/aphawave/internalTypes.py
-src/aphawave/jsonParser.py
-src/aphawave/utilityV2.py
 tests/testOSClient.py
 tests/testOpenAiClient.py
 tests/testSchema.py
```

### Comparing `alphawave-0.2.3/src/alphawave_agents/Agent.py` & `alphawave-0.2.4/src/alphawave_agents/Agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from alphawave_agents.AgentCommandValidator import AgentCommandValidator
 import promptrix.Utilities
 from alphawave_agents.agentTypes import Command, AgentThought, AgentThoughtSchema
 from alphawave_agents.AgentCommandSection import AgentCommandSection
 
 from typing import Dict, Any
 from pydantic import BaseModel, Field
+import traceback
 
 class AgentCommandSchema(BaseModel):
     type: str = Field("object", description="an agent that can perform a task")
     title: str = "Agent"
     properties: Dict[str, Any] = {
         "input": {
             "type": "string",
@@ -168,25 +169,25 @@
 
     def getCommand(self, title: str):
         return self._commands.get(title)
 
     def hasCommand(self, title: str):
         return title in self._commands
 
-    # Task execution
-
     async def completeTask(self, input: Optional[str] = None, agentId: Optional[str] = None, executeInitialThought: bool = False):
+      try:
         # Initialize the input to the next step
         stepInput = input if input is not None else self.memory.get(self.options['input_variable'])
         # Dispatch to child agent if needed
         step = 0
         state = self.get_agent_state(agentId)
-        if state.child:
-            childAgent = self.getCommand(state.child.title)
-            response = await childAgent.completeTask(input, state.child.agentId)
+        if 'child' in state and state['child'] is not None:
+            childAgent = self.getCommand(state['child'].title)
+            
+            response = await childAgent.completeTask(input, state['child'].agentId)
             if response.status != 'success':
                 return response
 
             # Delete child and save state
             del state.child
             self.setAgentState(state, agentId)
 
@@ -195,16 +196,18 @@
             stepInput = response.message
             step = 1
             executeInitialThought = False
 
         # Start main task loop
         while step < self.options['max_steps']:
             # Wait for step delay
+            
             if step > 0 and self.options['step_delay'] > 0:
-                await asyncio.sleep(self.options['step_delay'])
+                sys.stdout.flush()
+                await asyncio.sleep(self.options['step_delay']/1000)
 
             # Execute next step
             result = await self.execute_next_step(stepInput, agentId, executeInitialThought)
             if isinstance(result, str):
                 stepInput = result
             else:
                 return result
@@ -214,14 +217,17 @@
 
         # Return too many steps
         return {
             "type": "TaskResponse",
             "status": "too_many_steps",
             "message": "The current task has taken too many steps."
         }
+      except Exception as e:
+        traceback.print_exc()
+        pass
 
     # Agent as Commands
     async def execute(self, input: AgentCommandInput, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer):
         # Initialize the agents state
         agentId = input.agentId
         state = self.get_agent_state(agentId)
         state['context'] = input.input
@@ -262,25 +268,24 @@
                 self.memory.set(self.options['context_variable'], state['context'])
 
             # Create prompt
             history_variable = self.get_agent_history_variable(agent_id)
             sections = [agent_prompt]
             sections.append(AgentCommandSection(self._commands))
             sections.append(PromptInstructionSection)
-#            prompt = Prompt([
-#                GroupSection(sections, 'system'),
-#                ConversationHistory(history_variable, 1.0, True)
-#            ])
             prompt = Prompt([
-                agent_prompt, AgentCommandSection(self._commands), PromptInstructionSection,
+                GroupSection(sections, 'system'),
                 ConversationHistory(history_variable, 1.0, True)
             ])
+            #prompt = Prompt([
+            #    agent_prompt, AgentCommandSection(self._commands), PromptInstructionSection,
+            #    ConversationHistory(history_variable, 1.0, True)
+            #])
             if input:
-                prompt.sections.append(TextSection(input, 'user', -1, True, '\n', 'user: '))
-
+                prompt.sections.append(TextSection(input, 'user', -1, True, '\n', 'user'))
                 # Ensure input variable is set otherwise the history will be wrong.
                 self.memory.set(self.options['input_variable'], input)
 
 
             if execute_initial_thought and self._options['initial_thought']:
                 # Just use initial thought as response
                 # - This is used when agents are being called as commands.
@@ -288,15 +293,16 @@
                     'status': 'success',
                     'message': {'role': 'assistant', 'content': self._options['initial_thought']}
                 }
             else:
                 # Add initial thought to history
                 if state['totalSteps'] == 0 and self._options['initial_thought']:
                     history = self.memory.get(history_variable) or []
-                    history.append({'role': 'assistant', 'content': json.dumps(self._options['initial_thought'])})
+                    message = {'role': 'assistant', 'content': json.dumps(self._options['initial_thought'])}
+                    history.append(message)
                     self.memory.set(history_variable, history)
 
                 # Create command validator
                 validator = AgentCommandValidator(self._commands)
 
                 # Create a wave for the prompt
                 #wave = AlphaWave(client=self.client, prompt=self.prompt, prompt_options=self.options.prompt_options, memory=memory, functions=functions, tokenizer=tokenizer)
@@ -341,16 +347,17 @@
             if task_response:
                 if task_response['status'] in ['error', 'invalid_response', 'rate_limited', 'too_many_steps', 'too_long']:
                     return task_response
 
             # Update history
             history = self.memory.get(history_variable) or []
             if input:
-                history.append({'role': 'user', 'content': input})
-            history.append({'role': 'assistant', 'content': json.dumps(thought)})
+                #history.append({'role': 'user', 'content': input})
+                pass
+            #history.append({'role': 'assistant', 'content': json.dumps(thought)})
             self.memory.set(history_variable, history)
 
             # Save the agents state
             state['totalSteps'] += 1
             self.set_agent_state(state, agent_id)
 
             # Return result
@@ -388,54 +395,7 @@
         else:
             # Execute command and return result
             response = command.execute(input, self.memory, self.functions, self.tokenizer)
             if 'coroutine' in str(type(response)).lower():
                 return await response
             return response
 
-    async def completeTask(self, input: Optional[str] = None, agentId: Optional[str] = None, executeInitialThought: bool = False):
-        # Initialize the input to the next step
-        stepInput = input if input is not None else self.memory.get(self.options['input_variable'])
-
-        # Dispatch to child agent if needed
-        step = 0
-        state = self.get_agent_state(agentId)
-        if 'child' in state and state['child'] is not None:
-            childAgent = self.getCommand(state['child'].title)
-            response = await childAgent.completeTask(input, state['child'].agentId)
-            if response.status != 'success':
-                return response
-
-            # Delete child and save state
-            del state.child
-            self.setAgentState(state, agentId)
-
-            # Use agents response as input to the next step
-            # We don't know how many steps the child agent took, so we'll just assume it took one
-            stepInput = response.message
-            step = 1
-            executeInitialThought = False
-
-        # Start main task loop
-        while step < self.options['max_steps']:
-            # Wait for step delay
-            
-            if step > 0 and self.options['step_delay'] > 0:
-                sys.stdout.flush()
-                await asyncio.sleep(self.options['step_delay']/1000)
-
-            # Execute next step
-            result = await self.execute_next_step(stepInput, agentId, executeInitialThought)
-            if isinstance(result, str):
-                stepInput = result
-            else:
-                return result
-
-            step += 1
-            executeInitialThought = False
-
-        # Return too many steps
-        return {
-            "type": "TaskResponse",
-            "status": "too_many_steps",
-            "message": "The current task has taken too many steps."
-        }
```

### Comparing `alphawave-0.2.3/src/alphawave_agents/AgentCommandSection.py` & `alphawave-0.2.4/src/alphawave_agents/AgentCommandSection.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.3/src/alphawave_agents/AgentCommandValidator.py` & `alphawave-0.2.4/src/alphawave_agents/AgentCommandValidator.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,13 +37,17 @@
           command_validation_result = await command.validate(thought['command']['input'] or {}, memory, functions, tokenizer)
           if not command_validation_result['valid']:
               return command_validation_result
           
           # Return the validated thought
           return validation_result
         except Exception as e:
-            pass
+            return {
+                'type': 'Validation',
+                'valid': False,
+                'feedback': f'The command validation failed. try again {str(e)}'
+                }
         return {
             'type': 'Validation',
             'valid': False,
             'feedback': 'The command '+thought['command']['name']+' validation failed, try again'
         }
```

### Comparing `alphawave-0.2.3/src/alphawave_agents/AskCommand.py` & `alphawave-0.2.4/src/alphawave_agents/AskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.3/src/alphawave_agents/CompleteTaskCommand.py` & `alphawave-0.2.4/src/alphawave_agents/CompleteTaskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.3/src/alphawave_agents/ConfirmAnswerCommand.py` & `alphawave-0.2.4/src/alphawave_agents/ConfirmAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.3/src/alphawave_agents/FinalAnswerCommand.py` & `alphawave-0.2.4/src/alphawave_agents/FinalAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.3/src/alphawave_agents/MathCommand.py` & `alphawave-0.2.4/src/alphawave_agents/MathCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.3/src/alphawave_agents/PromptCommand.py` & `alphawave-0.2.4/src/alphawave_agents/PromptCommand.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,28 @@
 from alphawave.AlphaWave import AlphaWave
 from alphawave.AlphaWave import AlphaWaveOptions
 from alphawave.alphawaveTypes import PromptCompletionOptions
 from alphawave.MemoryFork import MemoryFork
 from alphawave_agents.SchemaBasedCommand import SchemaBasedCommand, CommandSchema as sbcCommandSchema
 from alphawave_agents.agentTypes import TaskResponse
 
+def update_dataclass(instance, **kwargs):
+    for key, value in kwargs.items():
+        if hasattr(instance, key):
+            setattr(instance, key, value)
+
 @dataclass
 class CommandSchema(sbcCommandSchema):
     schema_type: str
     title: str
     description: str
     properties: Dict[str,Dict[str,str]]
     required: list[str] = field(default_factory=list)
     returns: str = None
 
-def update_dataclass(instance, **kwargs):
-    for key, value in kwargs.items():
-        if hasattr(instance, key):
-            setattr(instance, key, value)
-
-    
 @dataclass
 class PromptCommandOptions(AlphaWaveOptions):
     def __init__(self, prompt_options: PromptCompletionOptions, schema: CommandSchema, parseResponse: Callable[[str, Dict[str, Any], PromptMemory, PromptFunctions, Tokenizer], Any] = None):
         super().__init__(prompt_options)
         self.prompt_options=prompt_options
         self.schema=schema
         self.parseResponse=parseResponse
@@ -44,24 +43,24 @@
     async def execute(self, input: Dict[str, Any], memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer) -> Union[TaskResponse, str]:
         # Fork memory and copy the input into the fork
         fork = MemoryFork(memory)
         for key, value in input.items():
             fork.set(key, value)
 
         # Create a wave and send it
-        #options = AlphaWaveOptions()
-        #update_dataclass(options, **self.options.__dict__)
-        #update_dataclass(options, memory=fork, functions= functions, tokenizer= tokenizer)
-        wave = AlphaWave(client=self.client, prompt=self.prompt, prompt_options=self.options.prompt_options, memory=memory, functions=functions, tokenizer=tokenizer)
+        options = AlphaWaveOptions()
+        update_dataclass(options, **self.options.__dict__)
+        update_dataclass(options, memory=fork, functions= functions, tokenizer= tokenizer)
+        wave = AlphaWave(client=self.client, prompt=self.prompt, prompt_options=self.options.prompt_options, memory=fork, functions=functions, tokenizer=tokenizer)
         response = await wave.completePrompt()
         # Process the response
         message = response['message']['content'] if isinstance(response['message'], dict) else response['message']
         if response['status'] == "success":
             # Return the response
-            parsed = await self.options.parseResponse(message, input, memory, functions, tokenizer) if self.options.parseResponse else message
+            parsed = await self.options.parseResponse(message, input, fork, functions, tokenizer) if self.options.parseResponse else message
             return Utilities.to_string(tokenizer, parsed)
         else:
             # Return the error
             return {
                 "type": "TaskResponse",
                 "status": response['status'],
                 "message": message
```

### Comparing `alphawave-0.2.3/src/alphawave_agents/SchemaBasedCommand.py` & `alphawave-0.2.4/src/alphawave_agents/SchemaBasedCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.3/src/alphawave_agents/SentimentAnalysis.py` & `alphawave-0.2.4/src/alphawave_agents/SentimentAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.3/src/alphawave_agents/SetPropertyCommand.py` & `alphawave-0.2.4/src/alphawave_agents/SetPropertyCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.3/src/alphawave_agents/agentTypes.py` & `alphawave-0.2.4/src/alphawave_agents/agentTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.3/tests/testOSClient.py` & `alphawave-0.2.4/tests/testOSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.3/tests/testOpenAiClient.py` & `alphawave-0.2.4/tests/testOpenAiClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.3/tests/testSchema.py` & `alphawave-0.2.4/tests/testSchema.py`

 * *Files identical despite different names*

