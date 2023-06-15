# Comparing `tmp/agixt-1.2.7.tar.gz` & `tmp/agixt-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.2.7.tar", last modified: Tue Jun 13 02:04:55 2023, max compression
+gzip compressed data, was "agixt-1.2.8.tar", last modified: Thu Jun 15 16:17:05 2023, max compression
```

## Comparing `agixt-1.2.7.tar` & `agixt-1.2.8.tar`

### file list

```diff
@@ -1,207 +1,210 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.137424 agixt-1.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-13 02:04:45.000000 agixt-1.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-13 02:04:45.000000 agixt-1.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-13 02:04:55.137424 agixt-1.2.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.117424 agixt-1.2.7/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    15882 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/Extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    24534 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/Interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/Prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.117424 agixt-1.2.7/agixt/WORKSPACE/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/WORKSPACE/example.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.113424 agixt-1.2.7/agixt/agents/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.117424 agixt-1.2.7/agixt/agents/gpt4free/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/agents/gpt4free/config.json
--rw-r--r--   0 runner    (1001) docker     (123)    16614 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.117424 agixt-1.2.7/agixt/chains/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/chains/Generate Smart Task Chain.json
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/chains/Generate Task Chain.json
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/chains/Generate and Run Smart Task Chain.json
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/chains/Generate and Run Task Chain.json
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/chains/Smart Chat.json
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/chains/Smart Instruct.json
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/chains/Test_Commands.json
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/chains/Write a Poem.json
--rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/example.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.121424 agixt-1.2.7/agixt/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/agixt_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/agixt_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/briantts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/dalle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/elevenlabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/google.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/gtts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/macostts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/microsoft_365.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/searxng.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/sendgrid_email.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/times.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/twitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/web_playwright.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.121424 agixt-1.2.7/agixt/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Chat.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Check-Instruction.txt
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Create New Command.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Custom Input.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Get Task Description.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Get Task List.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Instruction.txt
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/JSONFormatter.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Pick a Poem Subject.txt
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Pick-a-Link.txt
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Prioritize.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Pseudo Code.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Score Response.txt
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/SmartChat-CleanResponse.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/SmartChat-Researcher.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/SmartChat-Resolver.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/SmartChat-StepByStep.txt
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/SmartInstruct-CleanResponse.txt
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/SmartInstruct-Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/SmartInstruct-Researcher.txt
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/SmartInstruct-Resolver.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/SmartInstruct-StepByStep.txt
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/SmartTask-CleanResponse.txt
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/SmartTask-Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/SmartTask-StepByStep.txt
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Task Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Tell Me How.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Title a Poem.txt
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Validation.txt
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/ValidationFailed.txt
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/WebSearch.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Write a Haiku.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Write a Poem.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.121424 agixt-1.2.7/agixt/prompts/gpt-3.5-turbo/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/gpt-3.5-turbo/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.125424 agixt-1.2.7/agixt/prompts/gpt-4/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/gpt-4/instruct.txt
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.125424 agixt-1.2.7/agixt/prompts/starchat/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/starchat/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.125424 agixt-1.2.7/agixt/prompts/vicuna/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/vicuna/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.125424 agixt-1.2.7/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/claude.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/llamacppapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/poe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/runpod.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.117424 agixt-1.2.7/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-13 02:04:55.000000 agixt-1.2.7/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-06-13 02:04:55.000000 agixt-1.2.7/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 02:04:55.000000 agixt-1.2.7/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-13 02:04:55.000000 agixt-1.2.7/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 02:04:55.000000 agixt-1.2.7/agixt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.125424 agixt-1.2.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.125424 agixt-1.2.7/docs/1-Getting started/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/1-Getting started/Quick Start.md
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/1-Getting started/Screenshots.md
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/1-Getting started/Support.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.129424 agixt-1.2.7/docs/2-Concepts/
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/2-Concepts/0-Core Concepts.md
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/2-Concepts/Agents.md
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/2-Concepts/Chains.md
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/2-Concepts/Chat.md
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/2-Concepts/Commands.md
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/2-Concepts/Instructions.md
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/2-Concepts/Prompts.md
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/2-Concepts/Providers.md
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/2-Concepts/Smart Chat.md
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/2-Concepts/Smart Instruct.md
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/2-Concepts/Smart Task.md
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/2-Concepts/Tasks.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.129424 agixt-1.2.7/docs/3-Providers/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/Anthropic Claude.md
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/Azure OpenAI.md
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/ChatGPT.md
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/FastChat.md
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/GPT4ALL-GPU.md
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/GPT4ALL.md
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/GPT4Free.md
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/Google Bard.md
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/Google Palm.md
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/Hugging Face Transformers.md
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/HuggingChat.md
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/Kobold.md
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/Microsoft Bing.md
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/Oobabooga Text Generation Web UI.md
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/OpenAI.md
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/Poe.md
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/llamacpp API.md
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/llamacpp.md
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.133424 agixt-1.2.7/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/images/AGiXT-gradient-flat.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/images/AGiXT-gradient-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/images/AGiXT.png
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/images/AGiXT.svg
--rw-r--r--   0 runner    (1001) docker     (123)  1707562 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/images/AGiXT_Original_PSD.psd
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/images/AGiXTwhiteborder.svg
--rw-r--r--   0 runner    (1001) docker     (123)    22316 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/images/Docker-desktop-win-setting-streamlit.png
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/images/Smart Instruct.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    20691 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/images/Smart Instruct.drawio.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/images/Smart Tasks.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    22011 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/images/Smart Tasks.drawio.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/images/Untitled Diagram.drawio
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 02:04:45.000000 agixt-1.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-13 02:04:45.000000 agixt-1.2.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 02:04:55.137424 agixt-1.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-13 02:04:45.000000 agixt-1.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.133424 agixt-1.2.7/streamlit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.133424 agixt-1.2.7/streamlit/.streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/.streamlit/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/ApiClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/Main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.133424 agixt-1.2.7/streamlit/auth_libs/
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/auth_libs/Cfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/auth_libs/Redirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/auth_libs/Users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.133424 agixt-1.2.7/streamlit/auth_libs/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/auth_libs/pages/Login.py
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/auth_libs/pages/Profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/auth_libs/pages/Register.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.133424 agixt-1.2.7/streamlit/components/
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/components/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/components/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/components/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/components/learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/components/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/components/verify_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.133424 agixt-1.2.7/streamlit/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/pages/0-Agent_Settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/pages/1-Prompt_Templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/pages/2-Chain_Management.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/pages/3-Interact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.133424 agixt-1.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-06-13 02:04:45.000000 agixt-1.2.7/tests/ApiClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-06-13 02:04:45.000000 agixt-1.2.7/tests/test-commands.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    56800 2023-06-13 02:04:45.000000 agixt-1.2.7/tests/tests.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.882562 agixt-1.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-15 16:16:56.000000 agixt-1.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-15 16:16:56.000000 agixt-1.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-15 16:17:05.882562 agixt-1.2.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.862562 agixt-1.2.8/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    16013 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/Extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27135 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/Interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/Prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.862562 agixt-1.2.8/agixt/WORKSPACE/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/WORKSPACE/example.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.858561 agixt-1.2.8/agixt/agents/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.862562 agixt-1.2.8/agixt/agents/gpt4free/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/agents/gpt4free/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16777 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.862562 agixt-1.2.8/agixt/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/chains/Generate Smart Task Chain without Research.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/chains/Generate Smart Task Chain.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/chains/Generate Task Chain without Research.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/chains/Generate Task Chain.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/chains/Generate and Run Smart Task Chain.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/chains/Generate and Run Task Chain.json
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/chains/Smart Chat.json
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/chains/Smart Instruct.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/chains/Test_Commands.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/chains/Write a Poem.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.866562 agixt-1.2.8/agixt/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/agixt_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/agixt_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/briantts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/dalle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/elevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/gtts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/macostts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/microsoft_365.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/searxng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/sendgrid_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/twitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/web_playwright.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.870561 agixt-1.2.8/agixt/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Chat.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Check-Instruction.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Create New Command.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Custom Input.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Get Task Description.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Get Task List.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Instruction.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/JSONFormatter.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Pick a Poem Subject.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Pick-a-Link.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Prioritize.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Pseudo Code.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Score Response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/SmartChat-CleanResponse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/SmartChat-Researcher.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/SmartChat-Resolver.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/SmartChat-StepByStep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/SmartInstruct-CleanResponse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/SmartInstruct-Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/SmartInstruct-Researcher.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/SmartInstruct-Resolver.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/SmartInstruct-StepByStep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/SmartTask-CleanResponse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/SmartTask-Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/SmartTask-StepByStep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Task Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Tell Me How.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Title a Chain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Title a Poem.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Validation.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/ValidationFailed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/WebSearch.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Write a Haiku.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Write a Poem.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.870561 agixt-1.2.8/agixt/prompts/gpt-3.5-turbo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/gpt-3.5-turbo/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.870561 agixt-1.2.8/agixt/prompts/gpt-4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/gpt-4/instruct.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.870561 agixt-1.2.8/agixt/prompts/starchat/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/starchat/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.870561 agixt-1.2.8/agixt/prompts/vicuna/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/vicuna/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.874561 agixt-1.2.8/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/claude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/llamacppapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/poe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.862562 agixt-1.2.8/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-15 16:17:05.000000 agixt-1.2.8/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-06-15 16:17:05.000000 agixt-1.2.8/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:17:05.000000 agixt-1.2.8/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-15 16:17:05.000000 agixt-1.2.8/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 16:17:05.000000 agixt-1.2.8/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.874561 agixt-1.2.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.874561 agixt-1.2.8/docs/1-Getting started/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/1-Getting started/Quick Start.md
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/1-Getting started/Screenshots.md
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/1-Getting started/Support.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.874561 agixt-1.2.8/docs/2-Concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/2-Concepts/0-Core Concepts.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/2-Concepts/Agents.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/2-Concepts/Chains.md
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/2-Concepts/Chat.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/2-Concepts/Commands.md
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/2-Concepts/Instructions.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/2-Concepts/Prompts.md
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/2-Concepts/Providers.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/2-Concepts/Smart Chat.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/2-Concepts/Smart Instruct.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/2-Concepts/Smart Task.md
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/2-Concepts/Tasks.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.874561 agixt-1.2.8/docs/3-Providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/Anthropic Claude.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/Azure OpenAI.md
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/ChatGPT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/FastChat.md
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/GPT4ALL-GPU.md
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/GPT4ALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/GPT4Free.md
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/Google Bard.md
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/Google Palm.md
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/Hugging Face Transformers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/HuggingChat.md
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/Kobold.md
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/Microsoft Bing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/Oobabooga Text Generation Web UI.md
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/OpenAI.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/Poe.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/llamacpp API.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/llamacpp.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.878561 agixt-1.2.8/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/images/AGiXT-gradient-flat.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/images/AGiXT-gradient-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/images/AGiXT.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/images/AGiXT.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  1707562 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/images/AGiXT_Original_PSD.psd
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/images/AGiXTwhiteborder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22316 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/images/Docker-desktop-win-setting-streamlit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/images/Smart Instruct.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    20691 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/images/Smart Instruct.drawio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/images/Smart Tasks.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    22011 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/images/Smart Tasks.drawio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/images/Untitled Diagram.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 16:16:56.000000 agixt-1.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-15 16:16:56.000000 agixt-1.2.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 16:17:05.882562 agixt-1.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-15 16:16:56.000000 agixt-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.878561 agixt-1.2.8/streamlit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.878561 agixt-1.2.8/streamlit/.streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/.streamlit/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/ApiClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/Main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.878561 agixt-1.2.8/streamlit/auth_libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/auth_libs/Cfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/auth_libs/Redirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/auth_libs/Users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.882562 agixt-1.2.8/streamlit/auth_libs/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/auth_libs/pages/Login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/auth_libs/pages/Profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/auth_libs/pages/Register.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.882562 agixt-1.2.8/streamlit/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/components/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/components/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/components/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/components/learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/components/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/components/verify_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.882562 agixt-1.2.8/streamlit/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/pages/0-Agent_Settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/pages/1-Prompt_Templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/pages/2-Chain_Management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/pages/3-Interact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.882562 agixt-1.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-06-15 16:16:56.000000 agixt-1.2.8/tests/ApiClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-06-15 16:16:56.000000 agixt-1.2.8/tests/test-commands.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    57091 2023-06-15 16:16:56.000000 agixt-1.2.8/tests/tests.ipynb
```

### Comparing `agixt-1.2.7/LICENSE` & `agixt-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/PKG-INFO` & `agixt-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.2.7
+Version: 1.2.8
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.2.7/agixt/Agent.py` & `agixt-1.2.8/agixt/Agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     return output
 
 
 class Agent:
     def __init__(self, agent_name=None):
         self.agent_name = agent_name if agent_name is not None else "AGiXT"
         self.config_path, self.history_file, self.folder_path = get_agent_file_paths(
-            agent_name=agent_name
+            agent_name=self.agent_name
         )
         self.AGENT_CONFIG = self.get_agent_config()
         if "settings" in self.AGENT_CONFIG:
             self.PROVIDER_SETTINGS = self.AGENT_CONFIG["settings"]
             if "provider" in self.PROVIDER_SETTINGS:
                 self.AI_PROVIDER = self.PROVIDER_SETTINGS["provider"]
                 self.PROVIDER = Provider(self.AI_PROVIDER, **self.PROVIDER_SETTINGS)
@@ -351,15 +351,18 @@
             return []
         try:
             with open(self.history_file, "r") as f:
                 yaml_history = yaml.safe_load(f)
             history = []
             for interaction in yaml_history["interactions"]:
                 role = interaction["role"]
-                message = interaction["timestamp"] + "\n" + interaction["message"]
+                if "timestamp" in interaction:
+                    message = interaction["timestamp"] + "\n" + interaction["message"]
+                else:
+                    message = interaction["message"]
                 history.append({role: message})
             return history
         except:
             return []
 
     def wipe_agent_memories(self):
         memories_folder = os.path.normpath(
```

### Comparing `agixt-1.2.7/agixt/Embedding.py` & `agixt-1.2.8/agixt/Embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,25 +109,25 @@
         chunk_size = 500
         embed = HuggingFaceTextEmbedding(
             model_id="gtr-t5-large", log=logging
         ).generate_embeddings_async
         return embed, chunk_size
 
     async def azure(self):
-        chunk_size = 1000
+        chunk_size = 2048
         embed = AzureTextEmbedding(
             deployment_name=self.AGENT_CONFIG["settings"]["AZURE_DEPLOYMENT_NAME"],
             endpoint=self.AGENT_CONFIG["settings"]["AZURE_OPENAI_ENDPOINT"],
             api_key=self.AGENT_CONFIG["settings"]["AZURE_API_KEY"],
             logger=logging,
         ).generate_embeddings_async
         return embed, chunk_size
 
     async def openai(self):
-        chunk_size = 1000
+        chunk_size = 4096
         embed = OpenAITextEmbedding(
             model_id="text-embedding-ada-002",
             api_key=self.AGENT_CONFIG["settings"]["OPENAI_API_KEY"],
             log=logging,
         ).generate_embeddings_async
         return embed, chunk_size
```

### Comparing `agixt-1.2.7/agixt/Extensions.py` & `agixt-1.2.8/agixt/Extensions.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/Interactions.py` & `agixt-1.2.8/agixt/Interactions.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,25 +64,66 @@
         try:
             with open(file_path, "r") as f:
                 responses = json.load(f)
             return responses.get(str(step_number))
         except:
             return ""
 
-    def get_step_content(self, chain_name, step_number, prompt_content):
+    def get_step_content(self, chain_name, prompt_content, user_input, agent_name):
         new_prompt_content = {}
-        for arg, value in prompt_content.items():
-            if "{STEP" in value:
-                # get the response from the step number
-                step_response = self.get_step_response(
-                    chain_name=chain_name, step_number=step_number
+        if isinstance(prompt_content, dict):
+            for arg, value in prompt_content.items():
+                if isinstance(value, str):
+                    if "{user_input}" in value:
+                        value = value.replace("{user_input}", user_input)
+                    if "{agent_name}" in value:
+                        value = value.replace("{agent_name}", agent_name)
+                    if "{STEP" in value:
+                        # Count how many times {STEP is in the value
+                        step_count = value.count("{STEP")
+                        for i in range(step_count):
+                            # Get the step number from value between {STEP and }
+                            new_step_number = int(value.split("{STEP")[1].split("}")[0])
+                            # get the response from the step number
+                            step_response = self.get_step_response(
+                                chain_name=chain_name, step_number=new_step_number
+                            )
+                            # replace the {STEPx} with the response
+                            value = value.replace(
+                                f"{{STEP{new_step_number}}}",
+                                f"{step_response['response']}",
+                            )
+                new_prompt_content[arg] = value
+        elif isinstance(prompt_content, str):
+            new_prompt_content = prompt_content
+            if "{user_input}" in prompt_content:
+                new_prompt_content = new_prompt_content.replace(
+                    "{user_input}", user_input
+                )
+            if "{agent_name}" in new_prompt_content:
+                new_prompt_content = new_prompt_content.replace(
+                    "{agent_name}", agent_name
                 )
-                # replace the {STEPx} with the response
-                value = value.replace(f"{{STEP{step_number}}}", step_response)
-            new_prompt_content[arg] = value
+            if "{STEP" in prompt_content:
+                step_count = value.count("{STEP")
+                for i in range(step_count):
+                    # Get the step number from value between {STEP and }
+                    new_step_number = int(
+                        prompt_content.split("{STEP")[1].split("}")[0]
+                    )
+                    # get the response from the step number
+                    step_response = self.get_step_response(
+                        chain_name=chain_name, step_number=new_step_number
+                    )
+                    # replace the {STEPx} with the response
+                    new_prompt_content = prompt_content.replace(
+                        f"{{STEP{new_step_number}}}", f"{step_response['response']}"
+                    )
+            if new_prompt_content == {}:
+                new_prompt_content = prompt_content
         return new_prompt_content
 
     async def format_prompt(
         self,
         user_input: str = "",
         top_results: int = 5,
         prompt="",
@@ -246,15 +287,15 @@
             else:
                 self.agent.log_interaction(role="USER", message=formatted_prompt)
             self.agent.log_interaction(role=self.agent_name, message=self.response)
 
         if shots > 1:
             responses = [self.response]
             for shot in range(shots - 1):
-                shot_response = self.run(
+                shot_response = await self.run(
                     user_input=user_input,
                     prompt=prompt,
                     context_results=context_results,
                     shots=shots - 1,
                     chain_name=chain_name,
                     step_number=step_number,
                     **kwargs,
@@ -267,27 +308,26 @@
                     for shot, response in enumerate(responses)
                 ]
             )
         return self.response
 
     async def run_chain_step(self, step: dict = {}, chain_name="", user_input=""):
         logging.info(step)
-        chain = Chain()
         if step:
             if "prompt_type" in step:
                 self.agent_name = step["agent_name"]
                 self.agent = Agent(self.agent_name)
                 self.agent_commands = self.agent.get_commands_string()
                 prompt_type = step["prompt_type"]
                 step_number = step["step"]
                 if "prompt_name" in step["prompt"]:
                     prompt_name = step["prompt"]["prompt_name"]
                 else:
                     prompt_name = ""
-                args = chain.get_step_content(
+                args = self.get_step_content(
                     chain_name=chain_name,
                     prompt_content=step["prompt"],
                     user_input=user_input,
                     agent_name=self.agent_name,
                 )
                 if prompt_type == "Command":
                     return await self.agent.execute(
@@ -300,45 +340,55 @@
                         prompt=prompt_name,
                         chain_name=chain_name,
                         step_number=step_number,
                         **args,
                     )
                 elif prompt_type == "Chain":
                     result = await self.run_chain(
-                        chain_name=step["prompt"]["chain_name"], user_input=user_input
+                        chain_name=args["chain"],
+                        user_input=args["input"],
+                        all_responses=False,
                     )
         if result:
             return result
         else:
             return None
 
-    async def run_chain(self, chain_name, user_input=None):
+    async def run_chain(self, chain_name, user_input=None, all_responses=True):
         chain = Chain()
         file_path = get_chain_responses_file_path(chain_name=chain_name)
         chain_data = chain.get_chain(chain_name=chain_name)
+        if chain_data == {}:
+            return f"Chain `{chain_name}` not found."
         logging.info(f"Running chain '{chain_name}'")
         responses = {}  # Create a dictionary to hold responses.
+        last_response = ""
         for step_data in chain_data["steps"]:
             if "prompt" in step_data and "step" in step_data:
                 logging.info(f"Running step {step_data['step']}")
                 step = {}
                 step_response = await self.run_chain_step(
                     step=step_data, chain_name=chain_name, user_input=user_input
                 )  # Get the response of the current step.
                 step["response"] = step_response
                 step["agent_name"] = step_data["agent_name"]
                 step["prompt"] = step_data["prompt"]
                 step["prompt_type"] = step_data["prompt_type"]
+                last_response = step_response
                 responses[step_data["step"]] = step  # Store the response.
                 logging.info(f"Response: {step_response}")
                 # Write the responses to the json file.
                 dt = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
                 with open(file_path, "w") as f:
                     json.dump(responses, f)
-        return responses
+        if all_responses == True:
+            return responses
+        else:
+            # Return only the last response in the chain.
+            return last_response
 
     async def smart_instruct(
         self,
         user_input: str = "Write a tweet about AI.",
         shots: int = 3,
         learn_file: str = "",
         objective: str = None,
```

### Comparing `agixt-1.2.7/agixt/Memories.py` & `agixt-1.2.8/agixt/Memories.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/Prompts.py` & `agixt-1.2.8/agixt/Prompts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/app.py` & `agixt-1.2.8/agixt/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from Prompts import Prompts
 from typing import Optional, Dict, List, Any
 from provider import get_provider_options, get_providers
 from Embedding import get_embedding_providers
 from Extensions import Extensions
 import os
 import logging
+import base64
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "version"), encoding="utf-8") as f:
     version = f.read().strip()
 
 logging.basicConfig(
     level=os.environ.get("LOGLEVEL", "INFO"),
@@ -180,23 +181,26 @@
         new_config=settings.settings, config_key="settings"
     )
     return ResponseMessage(message=update_config)
 
 
 @app.post("/api/agent/{agent_name}/learn/file", tags=["Agent"])
 async def learn_file(agent_name: str, file: FileInput) -> ResponseMessage:
+    # Strip any path information from the file name
+    file.file_name = os.path.basename(file.file_name)
     base_path = os.path.join(os.getcwd(), "WORKSPACE")
     file_path = os.path.normpath(os.path.join(base_path, file.file_name))
     if not file_path.startswith(base_path):
         raise Exception("Path given not allowed")
-    with open(file_path, "w") as f:
-        f.write(file.file_content)
+    file_content = base64.b64decode(file.file_content)
+    with open(file_path, "wb") as f:
+        f.write(file_content)
     try:
         memories = Agent(agent_name=agent_name).get_memories()
-        await memories.mem_read_file(file_path=file.file_content)
+        await memories.mem_read_file(file_path=file_path)
         try:
             os.remove(file_path)
         except Exception:
             pass
         return ResponseMessage(message="Agent learned the content from the file.")
     except Exception as e:
         try:
```

### Comparing `agixt-1.2.7/agixt/chains/Generate Smart Task Chain.json` & `agixt-1.2.8/agixt/chains/Generate Task Chain.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.677734375%*

 * *Differences: {"'chain_name'": "'Generate Task Chain'",*

 * * "'steps'": "{3: {'step': 4, 'prompt': {'command_name': 'Create Task Chain', "*

 * *            "'short_chain_description': '{STEP3}'}}, insert: [(2, OrderedDict([('step', 3), "*

 * *            "('agent_name', 'gpt4free'), ('prompt_type', 'Prompt'), ('prompt', "*

 * *            "OrderedDict([('prompt_name', 'Title a Chain')]))]))]}"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "chain_name": "Generate Smart Task Chain",
+    "chain_name": "Generate Task Chain",
     "steps": [
         {
             "agent_name": "gpt4free",
             "prompt": {
                 "context_results": 5,
                 "prompt_name": "Get Task List",
                 "websearch": true,
@@ -19,18 +19,27 @@
             },
             "prompt_type": "Prompt",
             "step": 2
         },
         {
             "agent_name": "gpt4free",
             "prompt": {
+                "prompt_name": "Title a Chain"
+            },
+            "prompt_type": "Prompt",
+            "step": 3
+        },
+        {
+            "agent_name": "gpt4free",
+            "prompt": {
                 "agent": "gpt4free",
-                "command_name": "Create Smart Task Chain",
+                "command_name": "Create Task Chain",
                 "numbered_list_of_tasks": "{STEP1}",
                 "primary_objective": "{user_input}",
+                "short_chain_description": "{STEP3}",
                 "short_task_description": "{STEP2}"
             },
             "prompt_type": "Command",
-            "step": 3
+            "step": 4
         }
     ]
 }
```

### Comparing `agixt-1.2.7/agixt/chains/Generate Task Chain.json` & `agixt-1.2.8/agixt/chains/Generate and Run Task Chain.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6427083333333333%*

 * *Differences: {"'chain_name'": "'Generate and Run Task Chain'",*

 * * "'steps'": "{3: {'step': 4, 'prompt': {'short_chain_description': '{STEP3}'}}, insert: [(2, "*

 * *            "OrderedDict([('step', 3), ('agent_name', 'gpt4free'), ('prompt_type', 'Prompt'), "*

 * *            "('prompt', OrderedDict([('prompt_name', 'Title a Chain')]))])), (4, "*

 * *            "OrderedDict([('step', 5), ('agent_name', 'gpt4free'), ('prompt_type', 'Chain'), "*

 * *            "('prompt', OrderedDict([('chain', '{STEP4}'), ('input', '{user_input}')]))]))]}" […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "chain_name": "Generate Task Chain",
+    "chain_name": "Generate and Run Task Chain",
     "steps": [
         {
             "agent_name": "gpt4free",
             "prompt": {
                 "context_results": 5,
                 "prompt_name": "Get Task List",
                 "websearch": true,
@@ -19,18 +19,36 @@
             },
             "prompt_type": "Prompt",
             "step": 2
         },
         {
             "agent_name": "gpt4free",
             "prompt": {
+                "prompt_name": "Title a Chain"
+            },
+            "prompt_type": "Prompt",
+            "step": 3
+        },
+        {
+            "agent_name": "gpt4free",
+            "prompt": {
                 "agent": "gpt4free",
                 "command_name": "Create Task Chain",
                 "numbered_list_of_tasks": "{STEP1}",
                 "primary_objective": "{user_input}",
+                "short_chain_description": "{STEP3}",
                 "short_task_description": "{STEP2}"
             },
             "prompt_type": "Command",
-            "step": 3
+            "step": 4
+        },
+        {
+            "agent_name": "gpt4free",
+            "prompt": {
+                "chain": "{STEP4}",
+                "input": "{user_input}"
+            },
+            "prompt_type": "Chain",
+            "step": 5
         }
     ]
 }
```

### Comparing `agixt-1.2.7/agixt/chains/Generate and Run Smart Task Chain.json` & `agixt-1.2.8/agixt/chains/Generate Smart Task Chain.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.71875%*

 * *Differences: {"'chain_name'": "'Generate Smart Task Chain'",*

 * * "'steps'": "{2: {'prompt_type': 'Prompt', 'prompt': {replace: OrderedDict([('prompt_name', 'Title "*

 * *            "a Chain')])}}, 3: {'prompt_type': 'Command', 'prompt': {replace: "*

 * *            "OrderedDict([('command_name', 'Create Smart Task Chain'), ('agent', 'gpt4free'), "*

 * *            "('primary_objective', '{user_input}'), ('numbered_list_of_tasks', '{STEP1}'), "*

 * *            "('short_task_description', '{STEP2}'), ('short_chain_description', '{STEP3}')])}} […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "chain_name": "Generate and Run Smart Task Chain",
+    "chain_name": "Generate Smart Task Chain",
     "steps": [
         {
             "agent_name": "gpt4free",
             "prompt": {
                 "context_results": 5,
                 "prompt_name": "Get Task List",
                 "websearch": true,
@@ -19,26 +19,27 @@
             },
             "prompt_type": "Prompt",
             "step": 2
         },
         {
             "agent_name": "gpt4free",
             "prompt": {
-                "agent": "gpt4free",
-                "command_name": "Create Smart Task Chain",
-                "numbered_list_of_tasks": "{STEP1}",
-                "primary_objective": "{user_input}",
-                "short_task_description": "{STEP2}"
+                "prompt_name": "Title a Chain"
             },
-            "prompt_type": "Command",
+            "prompt_type": "Prompt",
             "step": 3
         },
         {
             "agent_name": "gpt4free",
             "prompt": {
-                "chain_name": "{STEP3}"
+                "agent": "gpt4free",
+                "command_name": "Create Smart Task Chain",
+                "numbered_list_of_tasks": "{STEP1}",
+                "primary_objective": "{user_input}",
+                "short_chain_description": "{STEP3}",
+                "short_task_description": "{STEP2}"
             },
-            "prompt_type": "Chain",
+            "prompt_type": "Command",
             "step": 4
         }
     ]
 }
```

### Comparing `agixt-1.2.7/agixt/chains/Generate and Run Task Chain.json` & `agixt-1.2.8/agixt/chains/Generate Task Chain without Research.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.71484375%*

 * *Differences: {"'chain_name'": "'Generate Task Chain without Research'",*

 * * "'steps'": "{0: {'prompt': {delete: ['websearch', 'websearch_depth']}}, 2: {'prompt_type': "*

 * *            "'Prompt', 'prompt': {replace: OrderedDict([('prompt_name', 'Title a Chain')])}}, 3: "*

 * *            "{'prompt_type': 'Command', 'prompt': {replace: OrderedDict([('command_name', 'Create "*

 * *            "Task Chain'), ('agent', 'gpt4free'), ('primary_objective', '{user_input}'), "*

 * *            "('numbered_list_of_tasks', '{STEP1}'), ('short_task_desc […]*

```diff
@@ -1,17 +1,15 @@
 {
-    "chain_name": "Generate and Run Task Chain",
+    "chain_name": "Generate Task Chain without Research",
     "steps": [
         {
             "agent_name": "gpt4free",
             "prompt": {
                 "context_results": 5,
-                "prompt_name": "Get Task List",
-                "websearch": true,
-                "websearch_depth": 3
+                "prompt_name": "Get Task List"
             },
             "prompt_type": "Prompt",
             "step": 1
         },
         {
             "agent_name": "gpt4free",
             "prompt": {
@@ -19,26 +17,27 @@
             },
             "prompt_type": "Prompt",
             "step": 2
         },
         {
             "agent_name": "gpt4free",
             "prompt": {
-                "agent": "gpt4free",
-                "command_name": "Create Task Chain",
-                "numbered_list_of_tasks": "{STEP1}",
-                "primary_objective": "{user_input}",
-                "short_task_description": "{STEP2}"
+                "prompt_name": "Title a Chain"
             },
-            "prompt_type": "Command",
+            "prompt_type": "Prompt",
             "step": 3
         },
         {
             "agent_name": "gpt4free",
             "prompt": {
-                "chain_name": "{STEP3}"
+                "agent": "gpt4free",
+                "command_name": "Create Task Chain",
+                "numbered_list_of_tasks": "{STEP1}",
+                "primary_objective": "{user_input}",
+                "short_chain_description": "{STEP3}",
+                "short_task_description": "{STEP2}"
             },
-            "prompt_type": "Chain",
+            "prompt_type": "Command",
             "step": 4
         }
     ]
 }
```

### Comparing `agixt-1.2.7/agixt/chains/Smart Chat.json` & `agixt-1.2.8/agixt/chains/Smart Chat.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/chains/Smart Instruct.json` & `agixt-1.2.8/agixt/chains/Smart Instruct.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/chains/Test_Commands.json` & `agixt-1.2.8/agixt/chains/Test_Commands.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/chains/Write a Poem.json` & `agixt-1.2.8/agixt/chains/Write a Poem.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/example.ipynb` & `agixt-1.2.8/agixt/example.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/extensions/agixt_agent.py` & `agixt-1.2.8/agixt/extensions/agixt_agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/extensions/agixt_chain.py` & `agixt-1.2.8/agixt/extensions/agixt_chain.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,70 +19,81 @@
 
     async def create_task_chain(
         self,
         agent: str,
         primary_objective: str,
         numbered_list_of_tasks: str,
         short_task_description: str,
+        short_chain_description: str,
     ):
+        import datetime
+        now = datetime.datetime.now()  
+        timestamp = now.strftime("%Y-%m-%d_%H-%M-%S")
         task_list = numbered_list_of_tasks.split("\n")
         task_list = [
-            task
+            task.lstrip("0123456789.")  # Strip leading digits and periods
             for task in task_list
-            if task and task[0] in [str(i) for i in range(len(task_list))]
+            if task
+            and task[0]
+            in [str(i) for i in range(10)]  # Check for task starting with a digit (0-9)
         ]
-        chain_name = f"AI Generated Task - {short_task_description}"
+        chain_name = f"AI Generated Task - {short_chain_description} - {timestamp}"
         chain = Chain()
         chain.add_chain(chain_name=chain_name)
+        i = 1
         for task in task_list:
-            if "task_name" in task:
-                chain.add_chain_step(
-                    chain_name=chain_name,
-                    agent_name=agent,
-                    step_number=1,
-                    prompt_type="Prompt",
-                    prompt={
-                        "prompt_name": "Task Execution",
-                        "user_input": primary_objective,
-                        "task": task["task_name"],
-                        "websearch": True,
-                        "websearch_depth": 3,
-                        "context_results": 5,
-                    },
-                )
+            chain.add_chain_step(
+                chain_name=chain_name,
+                agent_name=agent,
+                step_number=i,
+                prompt_type="Prompt",
+                prompt={
+                    "prompt_name": "Task Execution",
+                    "user_input": primary_objective,
+                    "task": task,
+                    "websearch": True,
+                    "websearch_depth": 3,
+                    "context_results": 5,
+                },
+            )
+            i += 1
         return chain_name
 
     async def create_smart_task_chain(
         self,
         agent: str,
         primary_objective: str,
         numbered_list_of_tasks: str,
         short_task_description: str,
     ):
+        import datetime
+        now = datetime.datetime.now()  
+        timestamp = now.strftime("%Y-%m-%d_%H-%M-%S")
         task_list = numbered_list_of_tasks.split("\n")
         task_list = [
-            task
+            task.lstrip("0123456789.")  # Strip leading digits and periods
             for task in task_list
-            if task and task[0] in [str(i) for i in range(len(task_list))]
+            if task
+            and task[0]
+            in [str(i) for i in range(10)]  # Check for task starting with a digit (0-9)
         ]
-        chain_name = f"AI Generated Smart Task - {short_task_description}"
+        chain_name = f"AI Generated Smart Task - {short_chain_description} - {timestamp}"
         chain = Chain()
         chain.add_chain(chain_name=chain_name)
+        i = 1
         for task in task_list:
-            if "task_name" in task:
-                chain.add_chain_step(
-                    chain_name=chain_name,
-                    agent_name=agent,
-                    step_number=1,
-                    prompt_type="Chain",
-                    prompt={
-                        "chain_name": "Smart Instruct",
-                        "user_input": f"Primary Objective: {primary_objective}\nYour Task: {task['task_name']}",
-                    },
-                )
+            chain.add_chain_step(
+                chain_name=chain_name,
+                agent_name=agent,
+                step_number=i,
+                prompt_type="Chain",
+                prompt={
+                    "chain": "Smart Instruct",
+                    "input": f"Primary Objective: {primary_objective}\nYour Task: {task}",
+                },
+            )
+            i += 1
         return chain_name
 
-    async def run_chain(self, chain_name: str = "", user_input: str = ""):
-        await Interactions(agent_name="").run_chain(
-            chain_name=chain_name, user_input=user_input
-        )
+    async def run_chain(self, chain: str = "", input: str = ""):
+        await Interactions(agent_name="").run_chain(chain_name=chain, user_input=input)
         return "Chain started successfully."
```

### Comparing `agixt-1.2.7/agixt/extensions/briantts.py` & `agixt-1.2.8/agixt/extensions/briantts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/extensions/dalle.py` & `agixt-1.2.8/agixt/extensions/dalle.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/extensions/discord.py` & `agixt-1.2.8/agixt/extensions/discord.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/extensions/elevenlabs.py` & `agixt-1.2.8/agixt/extensions/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/extensions/file_system.py` & `agixt-1.2.8/agixt/extensions/file_system.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/extensions/github.py` & `agixt-1.2.8/agixt/extensions/github.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/extensions/google.py` & `agixt-1.2.8/agixt/extensions/google.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/extensions/gtts.py` & `agixt-1.2.8/agixt/extensions/gtts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/extensions/huggingface.py` & `agixt-1.2.8/agixt/extensions/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/extensions/macostts.py` & `agixt-1.2.8/agixt/extensions/macostts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/extensions/microsoft_365.py` & `agixt-1.2.8/agixt/extensions/microsoft_365.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/extensions/searxng.py` & `agixt-1.2.8/agixt/extensions/searxng.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/extensions/sendgrid_email.py` & `agixt-1.2.8/agixt/extensions/sendgrid_email.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/extensions/twitter.py` & `agixt-1.2.8/agixt/extensions/twitter.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/extensions/web_playwright.py` & `agixt-1.2.8/agixt/extensions/web_playwright.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/prompts/Create New Command.txt` & `agixt-1.2.8/agixt/prompts/Create New Command.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/prompts/Execution.txt` & `agixt-1.2.8/agixt/prompts/Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/prompts/Instruction.txt` & `agixt-1.2.8/agixt/prompts/Instruction.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/prompts/SmartInstruct-Execution.txt` & `agixt-1.2.8/agixt/prompts/SmartInstruct-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/prompts/SmartTask-Execution.txt` & `agixt-1.2.8/agixt/prompts/SmartTask-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/prompts/Task Execution.txt` & `agixt-1.2.8/agixt/prompts/Task Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/prompts/ValidationFailed.txt` & `agixt-1.2.8/agixt/prompts/ValidationFailed.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/prompts/gpt-3.5-turbo/instruct.txt` & `agixt-1.2.8/agixt/prompts/gpt-3.5-turbo/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/prompts/gpt-4/instruct.txt` & `agixt-1.2.8/agixt/prompts/gpt-4/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/prompts/instruct.txt` & `agixt-1.2.8/agixt/prompts/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/prompts/starchat/instruct.txt` & `agixt-1.2.8/agixt/prompts/starchat/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/prompts/vicuna/instruct.txt` & `agixt-1.2.8/agixt/prompts/vicuna/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/provider/__init__.py` & `agixt-1.2.8/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/provider/azure.py` & `agixt-1.2.8/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/provider/bing.py` & `agixt-1.2.8/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/provider/chatgpt.py` & `agixt-1.2.8/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/provider/claude.py` & `agixt-1.2.8/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/provider/fastchat.py` & `agixt-1.2.8/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/provider/gpt4all.py` & `agixt-1.2.8/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/provider/gpt4free.py` & `agixt-1.2.8/agixt/provider/gpt4free.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
         self.FAILED_PROVIDERS = []
         self.providers = [
             "DeepAI",
             "You",
             "UseLess",
             "ForeFront",
             "Theb",
-            "Poe",
             "AiColors",
         ]
         self.account_tokens = {}
 
     def create_account(self, provider, module):
         try:
             # the following call will not terminate the program even if it calls quit()
```

### Comparing `agixt-1.2.7/agixt/provider/gpugpt4all.py` & `agixt-1.2.8/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/provider/huggingchat.py` & `agixt-1.2.8/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/provider/huggingface.py` & `agixt-1.2.8/agixt/provider/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/provider/kobold.py` & `agixt-1.2.8/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/provider/llamacpp.py` & `agixt-1.2.8/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/provider/llamacppapi.py` & `agixt-1.2.8/agixt/provider/llamacppapi.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/provider/oobabooga.py` & `agixt-1.2.8/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/provider/openai.py` & `agixt-1.2.8/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/provider/palm.py` & `agixt-1.2.8/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/provider/poe.py` & `agixt-1.2.8/agixt/provider/poe.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/provider/runpod.py` & `agixt-1.2.8/agixt/provider/runpod.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt/provider/transformer.py` & `agixt-1.2.8/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/agixt.egg-info/PKG-INFO` & `agixt-1.2.8/agixt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.2.7
+Version: 1.2.8
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.2.7/agixt.egg-info/SOURCES.txt` & `agixt-1.2.8/agixt.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 agixt.egg-info/PKG-INFO
 agixt.egg-info/SOURCES.txt
 agixt.egg-info/dependency_links.txt
 agixt.egg-info/requires.txt
 agixt.egg-info/top_level.txt
 agixt/WORKSPACE/example.txt
 agixt/agents/gpt4free/config.json
+agixt/chains/Generate Smart Task Chain without Research.json
 agixt/chains/Generate Smart Task Chain.json
+agixt/chains/Generate Task Chain without Research.json
 agixt/chains/Generate Task Chain.json
 agixt/chains/Generate and Run Smart Task Chain.json
 agixt/chains/Generate and Run Task Chain.json
 agixt/chains/Smart Chat.json
 agixt/chains/Smart Instruct.json
 agixt/chains/Test_Commands.json
 agixt/chains/Write a Poem.json
@@ -71,14 +73,15 @@
 agixt/prompts/SmartInstruct-Resolver.txt
 agixt/prompts/SmartInstruct-StepByStep.txt
 agixt/prompts/SmartTask-CleanResponse.txt
 agixt/prompts/SmartTask-Execution.txt
 agixt/prompts/SmartTask-StepByStep.txt
 agixt/prompts/Task Execution.txt
 agixt/prompts/Tell Me How.txt
+agixt/prompts/Title a Chain.txt
 agixt/prompts/Title a Poem.txt
 agixt/prompts/Validation.txt
 agixt/prompts/ValidationFailed.txt
 agixt/prompts/WebSearch.txt
 agixt/prompts/Write a Haiku.txt
 agixt/prompts/Write a Poem.txt
 agixt/prompts/instruct.txt
```

### Comparing `agixt-1.2.7/docs/1-Getting started/Quick Start.md` & `agixt-1.2.8/docs/1-Getting started/Quick Start.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/1-Getting started/Screenshots.md` & `agixt-1.2.8/docs/1-Getting started/Screenshots.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/1-Getting started/Support.md` & `agixt-1.2.8/docs/1-Getting started/Support.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/2-Concepts/0-Core Concepts.md` & `agixt-1.2.8/docs/2-Concepts/0-Core Concepts.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/2-Concepts/Agents.md` & `agixt-1.2.8/docs/2-Concepts/Agents.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/2-Concepts/Chains.md` & `agixt-1.2.8/docs/2-Concepts/Chains.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/2-Concepts/Chat.md` & `agixt-1.2.8/docs/2-Concepts/Chat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/2-Concepts/Commands.md` & `agixt-1.2.8/docs/2-Concepts/Commands.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/2-Concepts/Instructions.md` & `agixt-1.2.8/docs/2-Concepts/Instructions.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/2-Concepts/Prompts.md` & `agixt-1.2.8/docs/2-Concepts/Prompts.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/2-Concepts/Smart Chat.md` & `agixt-1.2.8/docs/2-Concepts/Smart Chat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/2-Concepts/Smart Instruct.md` & `agixt-1.2.8/docs/2-Concepts/Smart Instruct.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/2-Concepts/Smart Task.md` & `agixt-1.2.8/docs/2-Concepts/Smart Task.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/3-Providers/Anthropic Claude.md` & `agixt-1.2.8/docs/3-Providers/Anthropic Claude.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/3-Providers/Azure OpenAI.md` & `agixt-1.2.8/docs/3-Providers/Azure OpenAI.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/3-Providers/ChatGPT.md` & `agixt-1.2.8/docs/3-Providers/ChatGPT.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/3-Providers/FastChat.md` & `agixt-1.2.8/docs/3-Providers/FastChat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/3-Providers/GPT4ALL-GPU.md` & `agixt-1.2.8/docs/3-Providers/GPT4ALL-GPU.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/3-Providers/GPT4ALL.md` & `agixt-1.2.8/docs/3-Providers/GPT4ALL.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/3-Providers/GPT4Free.md` & `agixt-1.2.8/docs/3-Providers/GPT4Free.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/3-Providers/Google Bard.md` & `agixt-1.2.8/docs/3-Providers/Google Bard.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/3-Providers/Hugging Face Transformers.md` & `agixt-1.2.8/docs/3-Providers/Hugging Face Transformers.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/3-Providers/HuggingChat.md` & `agixt-1.2.8/docs/3-Providers/HuggingChat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/3-Providers/Microsoft Bing.md` & `agixt-1.2.8/docs/3-Providers/Microsoft Bing.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/3-Providers/Oobabooga Text Generation Web UI.md` & `agixt-1.2.8/docs/3-Providers/Oobabooga Text Generation Web UI.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/3-Providers/OpenAI.md` & `agixt-1.2.8/docs/3-Providers/OpenAI.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/3-Providers/Poe.md` & `agixt-1.2.8/docs/3-Providers/Poe.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/3-Providers/llamacpp API.md` & `agixt-1.2.8/docs/3-Providers/llamacpp API.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/3-Providers/llamacpp.md` & `agixt-1.2.8/docs/3-Providers/llamacpp.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/README.md` & `agixt-1.2.8/docs/README.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/images/AGiXT-gradient-flat.svg` & `agixt-1.2.8/docs/images/AGiXT-gradient-flat.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/images/AGiXT-gradient-light.svg` & `agixt-1.2.8/docs/images/AGiXT-gradient-light.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/images/AGiXT.png` & `agixt-1.2.8/docs/images/AGiXT.png`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/images/AGiXT.svg` & `agixt-1.2.8/docs/images/AGiXT.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/images/AGiXT_Original_PSD.psd` & `agixt-1.2.8/docs/images/AGiXT_Original_PSD.psd`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/images/AGiXTwhiteborder.svg` & `agixt-1.2.8/docs/images/AGiXTwhiteborder.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/images/Docker-desktop-win-setting-streamlit.png` & `agixt-1.2.8/docs/images/Docker-desktop-win-setting-streamlit.png`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/images/Smart Instruct.drawio` & `agixt-1.2.8/docs/images/Smart Instruct.drawio`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/images/Smart Instruct.drawio.svg` & `agixt-1.2.8/docs/images/Smart Instruct.drawio.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/images/Smart Tasks.drawio` & `agixt-1.2.8/docs/images/Smart Tasks.drawio`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/images/Smart Tasks.drawio.svg` & `agixt-1.2.8/docs/images/Smart Tasks.drawio.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/docs/images/Untitled Diagram.drawio` & `agixt-1.2.8/docs/images/Untitled Diagram.drawio`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/setup.py` & `agixt-1.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/streamlit/ApiClient.py` & `agixt-1.2.8/streamlit/ApiClient.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/streamlit/Main.py` & `agixt-1.2.8/streamlit/Main.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/streamlit/auth_libs/Cfig.py` & `agixt-1.2.8/streamlit/auth_libs/Cfig.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/streamlit/auth_libs/Redirect.py` & `agixt-1.2.8/streamlit/auth_libs/Redirect.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/streamlit/auth_libs/Users.py` & `agixt-1.2.8/streamlit/auth_libs/Users.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/streamlit/auth_libs/pages/Login.py` & `agixt-1.2.8/streamlit/auth_libs/pages/Login.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/streamlit/auth_libs/pages/Profile.py` & `agixt-1.2.8/streamlit/auth_libs/pages/Profile.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/streamlit/auth_libs/pages/Register.py` & `agixt-1.2.8/streamlit/auth_libs/pages/Register.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/streamlit/components/chain.py` & `agixt-1.2.8/streamlit/components/chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/streamlit/components/docs.py` & `agixt-1.2.8/streamlit/components/docs.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/streamlit/components/history.py` & `agixt-1.2.8/streamlit/components/history.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from ApiClient import ApiClient
 import streamlit as st
+import html
 
 
 def get_history(agent_name):
     st.markdown("### Agent History")
     st.markdown(
         "The history of the agent's interactions. The latest responses are at the top."
     )
@@ -54,10 +55,11 @@
         for item in history:
             if "USER" in item.keys():
                 message_container += f"<div class='message user-message'><b>You:</b><br>{item['USER']}</div>"
             else:
                 if item[agent_name].startswith(f"{agent_name}:"):
                     item[agent_name] = item[agent_name][len(agent_name) + 1 :]
                 item[agent_name] = item[agent_name].replace("\n", "<br>")
+                item[agent_name] = html.escape(item[agent_name])
                 message_container += f"<div class='message agent-message'><b>{agent_name}:</b><br>{item[agent_name]}</div>"
         message_container += "</div>"
         st.write(message_container, unsafe_allow_html=True)
```

### Comparing `agixt-1.2.7/streamlit/components/learning.py` & `agixt-1.2.8/streamlit/components/learning.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import streamlit as st
 from ApiClient import ApiClient
 import os
+import base64
 
 
 def learning_page(agent_name):
     st.markdown("### Choose a Method for Learning")
 
     if agent_name:
         st.markdown("### Learn from a file")
@@ -19,15 +20,17 @@
                 if not os.path.exists(os.path.dirname(learn_file_path)):
                     os.makedirs(os.path.dirname(learn_file_path))
                 with open(learn_file_path, "wb") as f:
                     f.write(learn_file_upload.getbuffer())
                 ApiClient.learn_file(
                     agent_name=agent_name,
                     file_name=learn_file_path,
-                    file_content=learn_file_upload.read(),
+                    file_content=base64.b64encode(learn_file_upload.read()).decode(
+                        "utf-8"
+                    ),
                 )
                 st.success(
                     "Agent '"
                     + agent_name
                     + "' has learned from file: "
                     + learn_file_upload.name
                 )
```

### Comparing `agixt-1.2.7/streamlit/components/selectors.py` & `agixt-1.2.8/streamlit/components/selectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,18 @@
     return ApiClient.get_extensions()
 
 
 def build_args(args: dict = {}, prompt: dict = {}, step_number: int = 0):
     return {
         arg: st.text_input(arg, value=prompt.get(arg, ""), key=f"{arg}_{step_number}")
         for arg in args
-        if arg != "context" and arg != "command_list" and arg != "COMMANDS"
+        if arg != "context"
+        and arg != "command_list"
+        and arg != "COMMANDS"
+        and arg != "user_input"
     }
 
 
 def prompt_selection(prompt: dict = {}, step_number: int = 0):
     available_prompts = ApiClient.get_prompts()
     prompt_name = st.selectbox(
         "Select Custom Prompt",
```

### Comparing `agixt-1.2.7/streamlit/components/verify_backend.py` & `agixt-1.2.8/streamlit/components/verify_backend.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/streamlit/pages/0-Agent_Settings.py` & `agixt-1.2.8/streamlit/pages/0-Agent_Settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from ApiClient import ApiClient
 from components.selectors import agent_selection
 from components.verify_backend import verify_backend
 from components.docs import agixt_docs
 
 verify_backend()
 
-
 st.set_page_config(
     page_title="Agent Settings",
     page_icon=":hammer_and_wrench:",
     layout="wide",
 )
 agixt_docs()
 
@@ -191,21 +190,26 @@
 
             # Save the existing command state to prevent duplication
             existing_command_states = {
                 command_name: command_status
                 for command_name, command_status in available_commands.items()
             }
 
+            all_commands_selected = st.checkbox("Select All Commands")
+
             for command_name, command_status in available_commands.items():
-                toggle_status = st.checkbox(
-                    command_name,
-                    value=command_status,
-                    key=command_name,
-                )
-                available_commands[command_name] = toggle_status
+                if all_commands_selected:
+                    available_commands[command_name] = True
+                else:
+                    toggle_status = st.checkbox(
+                        command_name,
+                        value=command_status,
+                        key=command_name,
+                    )
+                    available_commands[command_name] = toggle_status
             if st.form_submit_button("Update Agent Commands"):
                 ApiClient.update_agent_commands(
                     agent_name=agent_name, commands=available_commands
                 )
 
     except Exception as e:
         st.error(f"Error loading agent configuration: {str(e)}")
```

### Comparing `agixt-1.2.7/streamlit/pages/1-Prompt_Templates.py` & `agixt-1.2.8/streamlit/pages/1-Prompt_Templates.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/streamlit/pages/2-Chain_Management.py` & `agixt-1.2.8/streamlit/pages/2-Chain_Management.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,19 +15,18 @@
 agixt_docs()
 st.session_state = {}
 chain_names = ApiClient.get_chains()
 agents = ApiClient.get_agents()
 st.header("Chain Management")
 chain_action = st.selectbox("Action", ["Create Chain", "Modify Chain", "Delete Chain"])
 
-# Replace this line
-# chain_name = st.text_input("Chain Name")
-
-# With this line
-chain_name = st.text_area("Chain Name")
+if chain_action == "Create Chain":
+    chain_name = st.text_input("Chain Name")
+else:
+    chain_name = st.selectbox("Chains", options=chain_names)
 
 if chain_action == "Create Chain":
     action_button = st.button("Create New Chain")
     if action_button:
         if chain_name:
             ApiClient.add_chain(chain_name=chain_name)
             st.success(f"Chain '{chain_name}' created.")
```

### Comparing `agixt-1.2.7/streamlit/pages/3-Interact.py` & `agixt-1.2.8/streamlit/pages/3-Interact.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/tests/ApiClient.py` & `agixt-1.2.8/tests/ApiClient.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/tests/test-commands.ipynb` & `agixt-1.2.8/tests/test-commands.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.2.7/tests/tests.ipynb` & `agixt-1.2.8/tests/tests.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.993664031124498%*

 * *Differences: {"'cells'": '{3: {\'execution_count\': 152, \'outputs\': {0: {\'text\': {insert: [(0, "The history '*

 * *            "saving thread hit an unexpected error (OperationalError('attempt to write a readonly "*

 * *            'database\')).History will not be written to the database.\\n")]}}}}, 5: '*

 * *            "{'execution_count': 153}, 7: {'execution_count': 154}, 9: {'execution_count': 155}, "*

 * *            '11: {\'execution_count\': 156, \'outputs\': {0: {\'text\': ["Extensions response: '*

 * *            "[['Scrape Text  […]*

```diff
@@ -24,21 +24,22 @@
                 "## Get Providers\n",
                 "\n",
                 "This will get a list of AI providers available to use with AGiXT.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 111,
+            "execution_count": 152,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
+                        "The history saving thread hit an unexpected error (OperationalError('attempt to write a readonly database')).History will not be written to the database.\n",
                         "Providers: ['gpt4free', 'azure', 'chatgpt', 'runpod', 'poe', 'oobabooga', 'openai', 'huggingface', 'fastchat', 'transformer', 'bing', 'palm', 'claude', 'gpt4all', 'huggingchat', 'llamacppapi', 'kobold', 'llamacpp', 'gpugpt4all', 'bard']\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
@@ -55,15 +56,15 @@
                 "## Get Default Provider Settings\n",
                 "\n",
                 "Choose a provider from the list of AI providers and get the default settings for that provider.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 112,
+            "execution_count": 153,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Settings for gpt4free: {'AI_MODEL': 'gpt-3.5-turbo', 'AI_TEMPERATURE': 0.7, 'MAX_TOKENS': 4000, 'provider': 'gpt4free'}\n"
@@ -87,15 +88,15 @@
                 "## Get Embedding Providers\n",
                 "\n",
                 "Embedding providers are used to embed information to vectors to store in the vector database to be searched for context injection.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 113,
+            "execution_count": 154,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Embed Providers: ['azure', 'cohere', 'default', 'embed_text', 'get_embedder', 'google_palm', 'google_vertex', 'large_local', 'llamacpp', 'openai']\n"
@@ -118,15 +119,15 @@
                 "## Get Extension Settings\n",
                 "\n",
                 "This is where we get all third party extension settings for the agent with defaults to fill in when there is nothing entered on the front end.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 114,
+            "execution_count": 155,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Extension Settings response: {'macostts': {'USE_MAC_OS_TTS': False}, 'file_system': {'WORKING_DIRECTORY': './WORKSPACE', 'WORKING_DIRECTORY_RESTRICTED': True}, 'huggingface': {'HUGGINGFACE_API_KEY': '', 'HUGGINGFACE_AUDIO_TO_TEXT_MODEL': 'facebook/wav2vec2-large-960h-lv60-self', 'WORKING_DIRECTORY': './WORKSPACE'}, 'discord': {'DISCORD_API_KEY': '', 'DISCORD_COMMAND_PREFIX': '/AGiXT'}, 'dalle': {'HUGGINGFACE_API_KEY': '', 'OPENAI_API_KEY': '', 'WORKING_DIRECTORY': './WORKSPACE'}, 'briantts': {'USE_BRIAN_TTS': True}, 'google': {'GOOGLE_API_KEY': ''}, 'microsoft_365': {'MICROSOFT_365_CLIENT_ID': '', 'MICROSOFT_365_CLIENT_SECRET': '', 'MICROSOFT_365_REDIRECT_URI': ''}, 'github': {'GITHUB_USERNAME': '', 'GITHUB_API_KEY': '', 'WORKING_DIRECTORY': './WORKSPACE'}, 'gtts': {'USE_GTTS': False}, 'elevenlabs': {'ELEVENLABS_API_KEY': '', 'ELEVENLABS_VOICE': 'Josh'}, 'sendgrid_email': {'SENDGRID_API_KEY': '', 'SENDGRID_EMAIL': ''}, 'searxng': {'SEARXNG_INSTANCE_URL': ''}, 'twitter': {'TW_CONSUMER_KEY': '', 'TW_CONSUMER_SECRET': '', 'TW_ACCESS_TOKEN': '', 'TW_ACCESS_TOKEN_SECRET': ''}}\n"
@@ -147,22 +148,22 @@
             "metadata": {},
             "source": [
                 "## Get Extension Commands\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 115,
+            "execution_count": 156,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Extensions response: [['Scrape Text with Playwright', 'scrape_text_with_playwright', {'url': None}], ['Scrape Links with Playwright', 'scrape_links_with_playwright', {'url': None}], ['Speak with MacOS TTS', 'speak_with_macos_speech', {'text': None, 'voice_index': 0}], ['Evaluate Code', 'evaluate_code', {'code': None, 'agent': 'AGiXT'}], ['Analyze Pull Request', 'analyze_pull_request', {'pr_url': None, 'agent': 'AGiXT'}], ['Perform Automated Testing', 'perform_automated_testing', {'test_url': None, 'agent': 'AGiXT'}], ['Run CI-CD Pipeline', 'run_ci_cd_pipeline', {'repo_url': None, 'agent': 'AGiXT'}], ['Improve Code', 'improve_code', {'suggestions': None, 'code': None, 'agent': 'AGiXT'}], ['Write Tests', 'write_tests', {'code': None, 'focus': None, 'agent': 'AGiXT'}], ['Create a new command', 'create_command', {'function_description': None, 'agent': 'AGiXT'}], ['Describe Image', 'describe_image', {'image_url': None}], ['Ask AI Agent Bing', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent Bing', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent tester', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent tester', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent gpt4free', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent gpt4free', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent Bard', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent Bard', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent Vicuna', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent Vicuna', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent OpenAI', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent OpenAI', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent azure', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent azure', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent ChatGPT', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent ChatGPT', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent Guanaco', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent Guanaco', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Write to File', 'write_to_file', {'filename': None, 'text': None}], ['Read File', 'read_file', {'filename': None}], ['Search Files', 'search_files', {'directory': None}], ['Append to File', 'append_to_file', {'filename': None, 'text': None}], ['Execute Python File', 'execute_python_file', {'file': None}], ['Delete File', 'delete_file', {'filename': None}], ['Execute Shell', 'execute_shell', {'command_line': None}], ['Read Audio from File', 'read_audio_from_file', {'audio_path': None}], ['Read Audio', 'read_audio', {'audio': None}], ['Generate Image with Stable Diffusion', 'generate_image_with_hf', {'prompt': None, 'filename': None}], ['Speak with TTS with BrianTTS', 'speak_with_briantts', {'text': None}], ['Clone Github Repository', 'clone_repo', {'repo_url': None, 'clone_path': None}], ['Get Datetime', 'get_datetime', {}], ['Speak with TTS Using Elevenlabs', 'speak_with_elevenlabs', {'text': None, 'voice_index': 0}], ['Use The Search Engine', 'search', {'query': None}], ['Create Task Chain', 'create_task_chain', {'agent': None, 'primary_objective': None, 'numbered_list_of_tasks': None, 'short_task_description': None}], ['Create Smart Task Chain', 'create_smart_task_chain', {'agent': None, 'primary_objective': None, 'numbered_list_of_tasks': None, 'short_task_description': None}]]\n"
+                        "Extensions response: [['Scrape Text with Playwright', 'scrape_text_with_playwright', {'url': None}], ['Scrape Links with Playwright', 'scrape_links_with_playwright', {'url': None}], ['Speak with MacOS TTS', 'speak_with_macos_speech', {'text': None, 'voice_index': 0}], ['Evaluate Code', 'evaluate_code', {'code': None, 'agent': 'AGiXT'}], ['Analyze Pull Request', 'analyze_pull_request', {'pr_url': None, 'agent': 'AGiXT'}], ['Perform Automated Testing', 'perform_automated_testing', {'test_url': None, 'agent': 'AGiXT'}], ['Run CI-CD Pipeline', 'run_ci_cd_pipeline', {'repo_url': None, 'agent': 'AGiXT'}], ['Improve Code', 'improve_code', {'suggestions': None, 'code': None, 'agent': 'AGiXT'}], ['Write Tests', 'write_tests', {'code': None, 'focus': None, 'agent': 'AGiXT'}], ['Create a new command', 'create_command', {'function_description': None, 'agent': 'AGiXT'}], ['Describe Image', 'describe_image', {'image_url': None}], ['Ask AI Agent Bing', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent Bing', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent tester', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent tester', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent gpt4free', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent gpt4free', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent Bard', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent Bard', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent Vicuna', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent Vicuna', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent OpenAI', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent OpenAI', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent azure', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent azure', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent ChatGPT', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent ChatGPT', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent new_agent', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent new_agent', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent Guanaco', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent Guanaco', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Write to File', 'write_to_file', {'filename': None, 'text': None}], ['Read File', 'read_file', {'filename': None}], ['Search Files', 'search_files', {'directory': None}], ['Append to File', 'append_to_file', {'filename': None, 'text': None}], ['Execute Python File', 'execute_python_file', {'file': None}], ['Delete File', 'delete_file', {'filename': None}], ['Execute Shell', 'execute_shell', {'command_line': None}], ['Read Audio from File', 'read_audio_from_file', {'audio_path': None}], ['Read Audio', 'read_audio', {'audio': None}], ['Generate Image with Stable Diffusion', 'generate_image_with_hf', {'prompt': None, 'filename': None}], ['Speak with TTS with BrianTTS', 'speak_with_briantts', {'text': None}], ['Clone Github Repository', 'clone_repo', {'repo_url': None, 'clone_path': None}], ['Get Datetime', 'get_datetime', {}], ['Speak with TTS Using Elevenlabs', 'speak_with_elevenlabs', {'text': None, 'voice_index': 0}], ['Use The Search Engine', 'search', {'query': None}], ['Create Task Chain', 'create_task_chain', {'agent': None, 'primary_objective': None, 'numbered_list_of_tasks': None, 'short_task_description': None}], ['Create Smart Task Chain', 'create_smart_task_chain', {'agent': None, 'primary_objective': None, 'numbered_list_of_tasks': None, 'short_task_description': None}]]\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_extensions()\n",
@@ -178,22 +179,22 @@
                 "## Get a list of all current Agents\n",
                 "\n",
                 "Any agents that you have created will be listed here. The `status` field is to say if the agent is currently running a task or not.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 116,
+            "execution_count": 157,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Agents: [{'name': 'Bing', 'status': False}, {'name': 'tester', 'status': False}, {'name': 'gpt4free', 'status': False}, {'name': 'Bard', 'status': False}, {'name': 'Vicuna', 'status': False}, {'name': 'OpenAI', 'status': False}, {'name': 'azure', 'status': False}, {'name': 'ChatGPT', 'status': False}, {'name': 'Guanaco', 'status': False}]\n"
+                        "Agents: [{'name': 'Bing', 'status': False}, {'name': 'tester', 'status': False}, {'name': 'gpt4free', 'status': False}, {'name': 'Bard', 'status': False}, {'name': 'Vicuna', 'status': False}, {'name': 'OpenAI', 'status': False}, {'name': 'azure', 'status': False}, {'name': 'ChatGPT', 'status': False}, {'name': 'new_agent', 'status': False}, {'name': 'Guanaco', 'status': False}]\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_agents()\n",
@@ -209,15 +210,15 @@
                 "## Create a new Agent\n",
                 "\n",
                 "Creates a new agent with the `gpt4free` provider. We'll use `gpt4free` because it is the one that requires the least configuration.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 117,
+            "execution_count": 158,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Add agent response: {'message': 'Agent test_agent created.'}\n"
@@ -245,15 +246,15 @@
                 "## Rename the test agent\n",
                 "\n",
                 "We will just rename it to `new_agent`.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 118,
+            "execution_count": 159,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Rename agent response: {'message': 'Agent renamed.'}\n"
@@ -280,22 +281,22 @@
                 "## Get the agent's settings\n",
                 "\n",
                 "This will get the settings for the agent we just created, this will tell you all commands available to the agent as well as all of the provider settings for the agent.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 119,
+            "execution_count": 160,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Config for new_agent: {'commands': {'Scrape Text with Playwright': False, 'Scrape Links with Playwright': False, 'Speak with MacOS TTS': False, 'Evaluate Code': False, 'Analyze Pull Request': False, 'Perform Automated Testing': False, 'Run CI-CD Pipeline': False, 'Improve Code': False, 'Write Tests': False, 'Create a new command': False, 'Describe Image': False, 'Ask AI Agent Bing': False, 'Instruct AI Agent Bing': False, 'Ask AI Agent tester': False, 'Instruct AI Agent tester': False, 'Ask AI Agent gpt4free': False, 'Instruct AI Agent gpt4free': False, 'Ask AI Agent Bard': False, 'Instruct AI Agent Bard': False, 'Ask AI Agent Vicuna': False, 'Instruct AI Agent Vicuna': False, 'Ask AI Agent OpenAI': False, 'Instruct AI Agent OpenAI': False, 'Ask AI Agent azure': False, 'Instruct AI Agent azure': False, 'Ask AI Agent ChatGPT': False, 'Instruct AI Agent ChatGPT': False, 'Ask AI Agent new_agent': False, 'Instruct AI Agent new_agent': False, 'Ask AI Agent Guanaco': False, 'Instruct AI Agent Guanaco': False, 'Write to File': False, 'Read File': False, 'Search Files': False, 'Append to File': False, 'Execute Python File': False, 'Delete File': False, 'Execute Shell': False, 'Read Audio from File': False, 'Read Audio': False, 'Generate Image with Stable Diffusion': False, 'Speak with TTS with BrianTTS': False, 'Clone Github Repository': False, 'Get Datetime': False, 'Speak with TTS Using Elevenlabs': False, 'Use The Search Engine': False, 'Create Task Chain': False, 'Create Smart Task Chain': False}, 'settings': {'AI_MODEL': 'gpt-3.5-turbo', 'AI_TEMPERATURE': 0.7, 'MAX_TOKENS': 4000, 'provider': 'gpt4free'}}\n"
+                        "Config for new_agent: {'commands': {'Scrape Text with Playwright': False, 'Scrape Links with Playwright': False, 'Speak with MacOS TTS': False, 'Evaluate Code': False, 'Analyze Pull Request': False, 'Perform Automated Testing': False, 'Run CI-CD Pipeline': False, 'Improve Code': False, 'Write Tests': False, 'Create a new command': False, 'Describe Image': False, 'Ask AI Agent Bing': False, 'Instruct AI Agent Bing': False, 'Ask AI Agent tester': False, 'Instruct AI Agent tester': False, 'Ask AI Agent gpt4free': False, 'Instruct AI Agent gpt4free': False, 'Ask AI Agent Bard': False, 'Instruct AI Agent Bard': False, 'Ask AI Agent Vicuna': False, 'Instruct AI Agent Vicuna': False, 'Ask AI Agent OpenAI': False, 'Instruct AI Agent OpenAI': False, 'Ask AI Agent azure': False, 'Instruct AI Agent azure': False, 'Ask AI Agent ChatGPT': False, 'Instruct AI Agent ChatGPT': False, 'Ask AI Agent new_agent': False, 'Instruct AI Agent new_agent': False, 'Ask AI Agent Guanaco': False, 'Instruct AI Agent Guanaco': False, 'Write to File': False, 'Read File': False, 'Search Files': False, 'Append to File': False, 'Execute Python File': False, 'Delete File': False, 'Execute Shell': False, 'Read Audio from File': False, 'Read Audio': False, 'Generate Image with Stable Diffusion': False, 'Speak with TTS with BrianTTS': False, 'Clone Github Repository': False, 'Get Datetime': False, 'Speak with TTS Using Elevenlabs': False, 'Use The Search Engine': False, 'Create Task Chain': False, 'Create Smart Task Chain': False, 'Ask AI Agent new_agent_2': False, 'Instruct AI Agent new_agent_2': False}, 'settings': {'provider': 'gpt4free', 'AI_MODEL': 'gpt-3.5-turbo', 'AI_TEMPERATURE': '0.7', 'MAX_TOKENS': '4096', 'embedder': 'default', 'autonomous_execution': 'false'}}\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_agentconfig()\n",
@@ -312,23 +313,23 @@
                 "## Update the agent's settings\n",
                 "\n",
                 "We'll just update the temperature from the default `0.7` to `0.5` to confirm that we can modify a setting.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 120,
+            "execution_count": 161,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Update agent settings response: Agent new_agent configuration updated.\n",
-                        "New config for new_agent: {'commands': {'Scrape Text with Playwright': False, 'Scrape Links with Playwright': False, 'Speak with MacOS TTS': False, 'Evaluate Code': False, 'Analyze Pull Request': False, 'Perform Automated Testing': False, 'Run CI-CD Pipeline': False, 'Improve Code': False, 'Write Tests': False, 'Create a new command': False, 'Describe Image': False, 'Ask AI Agent Bing': False, 'Instruct AI Agent Bing': False, 'Ask AI Agent tester': False, 'Instruct AI Agent tester': False, 'Ask AI Agent gpt4free': False, 'Instruct AI Agent gpt4free': False, 'Ask AI Agent Bard': False, 'Instruct AI Agent Bard': False, 'Ask AI Agent Vicuna': False, 'Instruct AI Agent Vicuna': False, 'Ask AI Agent OpenAI': False, 'Instruct AI Agent OpenAI': False, 'Ask AI Agent azure': False, 'Instruct AI Agent azure': False, 'Ask AI Agent ChatGPT': False, 'Instruct AI Agent ChatGPT': False, 'Ask AI Agent new_agent': False, 'Instruct AI Agent new_agent': False, 'Ask AI Agent Guanaco': False, 'Instruct AI Agent Guanaco': False, 'Write to File': False, 'Read File': False, 'Search Files': False, 'Append to File': False, 'Execute Python File': False, 'Delete File': False, 'Execute Shell': False, 'Read Audio from File': False, 'Read Audio': False, 'Generate Image with Stable Diffusion': False, 'Speak with TTS with BrianTTS': False, 'Clone Github Repository': False, 'Get Datetime': False, 'Speak with TTS Using Elevenlabs': False, 'Use The Search Engine': False, 'Create Task Chain': False, 'Create Smart Task Chain': False}, 'settings': {'AI_MODEL': 'gpt-3.5-turbo', 'AI_TEMPERATURE': 0.5, 'MAX_TOKENS': 4000, 'provider': 'gpt4free'}}\n"
+                        "New config for new_agent: {'commands': {'Scrape Text with Playwright': False, 'Scrape Links with Playwright': False, 'Speak with MacOS TTS': False, 'Evaluate Code': False, 'Analyze Pull Request': False, 'Perform Automated Testing': False, 'Run CI-CD Pipeline': False, 'Improve Code': False, 'Write Tests': False, 'Create a new command': False, 'Describe Image': False, 'Ask AI Agent Bing': False, 'Instruct AI Agent Bing': False, 'Ask AI Agent tester': False, 'Instruct AI Agent tester': False, 'Ask AI Agent gpt4free': False, 'Instruct AI Agent gpt4free': False, 'Ask AI Agent Bard': False, 'Instruct AI Agent Bard': False, 'Ask AI Agent Vicuna': False, 'Instruct AI Agent Vicuna': False, 'Ask AI Agent OpenAI': False, 'Instruct AI Agent OpenAI': False, 'Ask AI Agent azure': False, 'Instruct AI Agent azure': False, 'Ask AI Agent ChatGPT': False, 'Instruct AI Agent ChatGPT': False, 'Ask AI Agent new_agent': False, 'Instruct AI Agent new_agent': False, 'Ask AI Agent Guanaco': False, 'Instruct AI Agent Guanaco': False, 'Write to File': False, 'Read File': False, 'Search Files': False, 'Append to File': False, 'Execute Python File': False, 'Delete File': False, 'Execute Shell': False, 'Read Audio from File': False, 'Read Audio': False, 'Generate Image with Stable Diffusion': False, 'Speak with TTS with BrianTTS': False, 'Clone Github Repository': False, 'Get Datetime': False, 'Speak with TTS Using Elevenlabs': False, 'Use The Search Engine': False, 'Create Task Chain': False, 'Create Smart Task Chain': False, 'Ask AI Agent new_agent_2': False, 'Instruct AI Agent new_agent_2': False}, 'settings': {'provider': 'gpt4free', 'AI_MODEL': 'gpt-3.5-turbo', 'AI_TEMPERATURE': 0.5, 'MAX_TOKENS': '4096', 'embedder': 'default', 'autonomous_execution': 'false'}}\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test update_agent_settings()\n",
@@ -353,22 +354,22 @@
                 "## Get a list of the agent's commands\n",
                 "\n",
                 "This will get a list of all commands available to the agent.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 121,
+            "execution_count": 162,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Commands: {'Scrape Text with Playwright': False, 'Scrape Links with Playwright': False, 'Speak with MacOS TTS': False, 'Evaluate Code': False, 'Analyze Pull Request': False, 'Perform Automated Testing': False, 'Run CI-CD Pipeline': False, 'Improve Code': False, 'Write Tests': False, 'Create a new command': False, 'Describe Image': False, 'Ask AI Agent Bing': False, 'Instruct AI Agent Bing': False, 'Ask AI Agent tester': False, 'Instruct AI Agent tester': False, 'Ask AI Agent gpt4free': False, 'Instruct AI Agent gpt4free': False, 'Ask AI Agent Bard': False, 'Instruct AI Agent Bard': False, 'Ask AI Agent Vicuna': False, 'Instruct AI Agent Vicuna': False, 'Ask AI Agent OpenAI': False, 'Instruct AI Agent OpenAI': False, 'Ask AI Agent azure': False, 'Instruct AI Agent azure': False, 'Ask AI Agent ChatGPT': False, 'Instruct AI Agent ChatGPT': False, 'Ask AI Agent new_agent': False, 'Instruct AI Agent new_agent': False, 'Ask AI Agent Guanaco': False, 'Instruct AI Agent Guanaco': False, 'Write to File': False, 'Read File': False, 'Search Files': False, 'Append to File': False, 'Execute Python File': False, 'Delete File': False, 'Execute Shell': False, 'Read Audio from File': False, 'Read Audio': False, 'Generate Image with Stable Diffusion': False, 'Speak with TTS with BrianTTS': False, 'Clone Github Repository': False, 'Get Datetime': False, 'Speak with TTS Using Elevenlabs': False, 'Use The Search Engine': False, 'Create Task Chain': False, 'Create Smart Task Chain': False}\n"
+                        "Commands: {'Scrape Text with Playwright': False, 'Scrape Links with Playwright': False, 'Speak with MacOS TTS': False, 'Evaluate Code': False, 'Analyze Pull Request': False, 'Perform Automated Testing': False, 'Run CI-CD Pipeline': False, 'Improve Code': False, 'Write Tests': False, 'Create a new command': False, 'Describe Image': False, 'Ask AI Agent Bing': False, 'Instruct AI Agent Bing': False, 'Ask AI Agent tester': False, 'Instruct AI Agent tester': False, 'Ask AI Agent gpt4free': False, 'Instruct AI Agent gpt4free': False, 'Ask AI Agent Bard': False, 'Instruct AI Agent Bard': False, 'Ask AI Agent Vicuna': False, 'Instruct AI Agent Vicuna': False, 'Ask AI Agent OpenAI': False, 'Instruct AI Agent OpenAI': False, 'Ask AI Agent azure': False, 'Instruct AI Agent azure': False, 'Ask AI Agent ChatGPT': False, 'Instruct AI Agent ChatGPT': False, 'Ask AI Agent new_agent': False, 'Instruct AI Agent new_agent': False, 'Ask AI Agent Guanaco': False, 'Instruct AI Agent Guanaco': False, 'Write to File': False, 'Read File': False, 'Search Files': False, 'Append to File': False, 'Execute Python File': False, 'Delete File': False, 'Execute Shell': False, 'Read Audio from File': False, 'Read Audio': False, 'Generate Image with Stable Diffusion': False, 'Speak with TTS with BrianTTS': False, 'Clone Github Repository': False, 'Get Datetime': False, 'Speak with TTS Using Elevenlabs': False, 'Use The Search Engine': False, 'Create Task Chain': False, 'Create Smart Task Chain': False, 'Ask AI Agent new_agent_2': False, 'Instruct AI Agent new_agent_2': False}\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_commands()\n",
@@ -385,15 +386,15 @@
                 "## Toggle a Command for the Agent\n",
                 "\n",
                 "We'll toggle the `Write to File` command to `true` to confirm that we can toggle a command.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 122,
+            "execution_count": 163,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Toggle command response: Command 'Write to File' toggled for agent 'new_agent'.\n"
@@ -418,15 +419,15 @@
                 "## Chat with the Agent\n",
                 "\n",
                 "We'll chat with the agent to confirm that it is working. We'll ask a simple question like `What is the capital of France?`\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 123,
+            "execution_count": 164,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Chat response: The capital of France is Paris.\n"
@@ -452,45 +453,40 @@
                 "## Prompt the Agent\n",
                 "\n",
                 "Use a custom Prompt Template to prompt the agent. For our example, we'll use our \"Write a Poem\" prompt template to have the agent write a poem for us about dragons.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 124,
+            "execution_count": 165,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Agent prompt response: In a land of fire and stone,\n",
-                        "Where dragons reign and wander alone,\n",
-                        "Their scales as hard as any stone,\n",
-                        "Their eyes as bright as the sun's own throne.\n",
+                        "Agent prompt response: Dragons, mighty beasts of fire\n",
+                        "With scales gleaming bright and higher\n",
+                        "Their breath scorching the earth and skies\n",
+                        "As they soar amidst the sunrise\n",
                         "\n",
-                        "They fly through skies of blue and red,\n",
-                        "And breathe out flames that can leave you dead,\n",
-                        "Horned beasts with sharp-toothed grins,\n",
-                        "That strike fear in the hearts of mortal men.\n",
+                        "Their wings spread wide, they glide with grace\n",
+                        "Through mountains and valleys they embrace\n",
+                        "Their eyes ablaze with ancient power\n",
+                        "As they guard their hoard with valour\n",
                         "\n",
-                        "Their wings move swift in the air,\n",
-                        "And their roars make kingdoms shake with care,\n",
-                        "Gold and jewels they hold in their keep,\n",
-                        "And woe to those who dare to steal or creep.\n",
+                        "Fierce and proud, they rule with might\n",
+                        "Their strength unmatched, their roar a fright\n",
+                        "Yet in their lair, a softer side\n",
+                        "As they tend to hatchlings, with gentle pride\n",
                         "\n",
-                        "Yet for all their strength and might,\n",
-                        "These creatures have a heart that's bright,\n",
-                        "They guard the sky with all their might,\n",
-                        "And in their lair they sleep at night.\n",
-                        "\n",
-                        "So let us honor these mighty beasts,\n",
-                        "For they are creatures we should please,\n",
-                        "With respect and homage we should treat,\n",
-                        "These dragons fierce and full of heat.\n"
+                        "From legend to myth, they captivate us still\n",
+                        "A symbol of power, and a tale to thrill\n",
+                        "Their existence a mystery, a fantasy so grand\n",
+                        "Dragons, creatures of wonder, guardians of the land.\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test prompt_agent()\n",
@@ -521,31 +517,27 @@
                 "## Instruct the Agent to do something\n",
                 "\n",
                 "We'll do something simple with it for the sake of the basic example, we'll just tell it to `Tell me the capital of France`.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 125,
+            "execution_count": 166,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Instruct response: The capital of France is Paris.\n",
-                        "\n",
-                        "Commands Executed:\n",
-                        "{'Write to File': {'filename': 'france_capital.txt', 'text': 'Paris'}}\n",
-                        "\n",
-                        "Command Execution Response:\n",
-                        "\n",
-                        "Executed Command:Write to File with args {'filename': 'france_capital.txt', 'text': 'Paris'}.\n",
-                        "Command Output: File written to successfully.\n",
-                        "\n"
+                        "Instruct response: ```JSON\n",
+                        "{\n",
+                        "    \"response\": \"The capital of France is Paris.\",\n",
+                        "    \"commands\": {}\n",
+                        "}\n",
+                        "```\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test instruct()\n",
@@ -564,22 +556,22 @@
                 "## Chat History of the Agent\n",
                 "\n",
                 "Get the chat history from the Agent.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 126,
+            "execution_count": 167,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Chat history: [{'USER': 'June 12, 2023 09:54 PM\\nWhat is the capital of France?'}, {'new_agent': 'June 12, 2023 09:54 PM\\nThe capital of France is Paris.'}, {'USER': 'June 12, 2023 09:54 PM\\nWrite a poem about dragons .\\n'}, {'new_agent': \"June 12, 2023 09:54 PM\\nIn a land of fire and stone,\\nWhere dragons reign and wander alone,\\nTheir scales as hard as any stone,\\nTheir eyes as bright as the sun's own throne.\\n\\nThey fly through skies of blue and red,\\nAnd breathe out flames that can leave you dead,\\nHorned beasts with sharp-toothed grins,\\nThat strike fear in the hearts of mortal men.\\n\\nTheir wings move swift in the air,\\nAnd their roars make kingdoms shake with care,\\nGold and jewels they hold in their keep,\\nAnd woe to those who dare to steal or creep.\\n\\nYet for all their strength and might,\\nThese creatures have a heart that's bright,\\nThey guard the sky with all their might,\\nAnd in their lair they sleep at night.\\n\\nSo let us honor these mighty beasts,\\nFor they are creatures we should please,\\nWith respect and homage we should treat,\\nThese dragons fierce and full of heat.\"}, {'USER': 'June 12, 2023 09:54 PM\\nCommands Available To Complete Task:\\n`Write to File` - Arguments: {\\'filename\\': None, \\'text\\': None}\\n\\n\\nYou are an AI language model. Your name is {AGENT_NAME}. Your role is to do anything asked of you with precision. You have the following constraints:\\n1. ~4000 word limit for short term memory. Your short term memory is short, so immediately save important information to files.\\n2. If you are unsure how you previously did something or want to recall past events, thinking about similar events will help you remember.\\n3. No user assistance.\\n4. Exclusively use the commands listed in double quotes e.g. \"command name\".\\n\\nYou have the following resources:\\n1. Internet access for searches and information gathering.\\n2. Long Term memory management.\\n3. GPT-3.5 powered Agents for delegation of simple tasks.\\n4. File output.\\n\\nRESPOND IN THE FOLLOWING JSON FORMAT ONLY! If there are no commands, simply make the commands section an empty object like {}.\\n```JSON\\n{\\n    \"response\": \"Your response to the task.\",\\n    \"commands\": {\\n        \"command_name\": {\\n            \"arg1\": \"val1\",\\n            \"arg2\": \"val2\"\\n        },\\n        \"command_name2\": {\\n            \"arg1\": \"val1\",\\n            \"arg2\": \"val2\",\\n            \"argN\": \"valN\"\\n        }\\n    }\\n}\\n```\\n\\nYour task: Tell me the capital of France.'}, {'new_agent': \"June 12, 2023 09:54 PM\\nThe capital of France is Paris.\\n\\nCommands Executed:\\n{'Write to File': {'filename': 'france_capital.txt', 'text': 'Paris'}}\\n\\nCommand Execution Response:\\n\\nExecuted Command:Write to File with args {'filename': 'france_capital.txt', 'text': 'Paris'}.\\nCommand Output: File written to successfully.\\n\"}]\n"
+                        "Chat history: [{'USER': 'June 13, 2023 02:26 PM\\nWhat is the capital of France?'}, {'new_agent': 'June 13, 2023 02:26 PM\\nThe capital of France is Paris.'}, {'USER': 'June 13, 2023 02:26 PM\\nWrite a poem about dragons .\\n'}, {'new_agent': 'June 13, 2023 02:26 PM\\nDragons, mighty beasts of fire\\nWith scales gleaming bright and higher\\nTheir breath scorching the earth and skies\\nAs they soar amidst the sunrise\\n\\nTheir wings spread wide, they glide with grace\\nThrough mountains and valleys they embrace\\nTheir eyes ablaze with ancient power\\nAs they guard their hoard with valour\\n\\nFierce and proud, they rule with might\\nTheir strength unmatched, their roar a fright\\nYet in their lair, a softer side\\nAs they tend to hatchlings, with gentle pride\\n\\nFrom legend to myth, they captivate us still\\nA symbol of power, and a tale to thrill\\nTheir existence a mystery, a fantasy so grand\\nDragons, creatures of wonder, guardians of the land.'}, {'USER': 'June 13, 2023 02:26 PM\\nCommands Available To Complete Task:\\n`Write to File` - Arguments: {\\'filename\\': None, \\'text\\': None}\\n\\n\\nYou are an AI language model. Your name is {AGENT_NAME}. Your role is to do anything asked of you with precision. You have the following constraints:\\n1. ~4000 word limit for short term memory. Your short term memory is short, so immediately save important information to files.\\n2. If you are unsure how you previously did something or want to recall past events, thinking about similar events will help you remember.\\n3. No user assistance.\\n4. Exclusively use the commands listed in double quotes e.g. \"command name\".\\n\\nYou have the following resources:\\n1. Internet access for searches and information gathering.\\n2. Long Term memory management.\\n3. GPT-3.5 powered Agents for delegation of simple tasks.\\n4. File output.\\n\\nRESPOND IN THE FOLLOWING JSON FORMAT ONLY! If there are no commands, simply make the commands section an empty object like {}.\\n```JSON\\n{\\n    \"response\": \"Your response to the task.\",\\n    \"commands\": {\\n        \"command_name\": {\\n            \"arg1\": \"val1\",\\n            \"arg2\": \"val2\"\\n        },\\n        \"command_name2\": {\\n            \"arg1\": \"val1\",\\n            \"arg2\": \"val2\",\\n            \"argN\": \"valN\"\\n        }\\n    }\\n}\\n```\\n\\nYour task: Tell me the capital of France.'}, {'new_agent': 'June 13, 2023 02:26 PM\\n```JSON\\n{\\n    \"response\": \"The capital of France is Paris.\",\\n    \"commands\": {}\\n}\\n```'}]\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_chat_history()\n",
@@ -596,23 +588,23 @@
                 "## Update Agent Commands\n",
                 "\n",
                 "In this example, we'll only change the `Write to File` command to `False`, but we could change any (or all) of the commands with this API call.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 127,
+            "execution_count": 168,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Update agent commands response: Agent new_agent configuration updated.\n",
-                        "New config for new_agent: {'commands': {'Scrape Text with Playwright': False, 'Scrape Links with Playwright': False, 'Speak with MacOS TTS': False, 'Evaluate Code': False, 'Analyze Pull Request': False, 'Perform Automated Testing': False, 'Run CI-CD Pipeline': False, 'Improve Code': False, 'Write Tests': False, 'Create a new command': False, 'Describe Image': False, 'Ask AI Agent Bing': False, 'Instruct AI Agent Bing': False, 'Ask AI Agent tester': False, 'Instruct AI Agent tester': False, 'Ask AI Agent gpt4free': False, 'Instruct AI Agent gpt4free': False, 'Ask AI Agent Bard': False, 'Instruct AI Agent Bard': False, 'Ask AI Agent Vicuna': False, 'Instruct AI Agent Vicuna': False, 'Ask AI Agent OpenAI': False, 'Instruct AI Agent OpenAI': False, 'Ask AI Agent azure': False, 'Instruct AI Agent azure': False, 'Ask AI Agent ChatGPT': False, 'Instruct AI Agent ChatGPT': False, 'Ask AI Agent new_agent': False, 'Instruct AI Agent new_agent': False, 'Ask AI Agent Guanaco': False, 'Instruct AI Agent Guanaco': False, 'Write to File': False, 'Read File': False, 'Search Files': False, 'Append to File': False, 'Execute Python File': False, 'Delete File': False, 'Execute Shell': False, 'Read Audio from File': False, 'Read Audio': False, 'Generate Image with Stable Diffusion': False, 'Speak with TTS with BrianTTS': False, 'Clone Github Repository': False, 'Get Datetime': False, 'Speak with TTS Using Elevenlabs': False, 'Use The Search Engine': False, 'Create Task Chain': False, 'Create Smart Task Chain': False}, 'settings': {'AI_MODEL': 'gpt-3.5-turbo', 'AI_TEMPERATURE': 0.5, 'MAX_TOKENS': 4000, 'provider': 'gpt4free'}}\n"
+                        "New config for new_agent: {'commands': {'Scrape Text with Playwright': False, 'Scrape Links with Playwright': False, 'Speak with MacOS TTS': False, 'Evaluate Code': False, 'Analyze Pull Request': False, 'Perform Automated Testing': False, 'Run CI-CD Pipeline': False, 'Improve Code': False, 'Write Tests': False, 'Create a new command': False, 'Describe Image': False, 'Ask AI Agent Bing': False, 'Instruct AI Agent Bing': False, 'Ask AI Agent tester': False, 'Instruct AI Agent tester': False, 'Ask AI Agent gpt4free': False, 'Instruct AI Agent gpt4free': False, 'Ask AI Agent Bard': False, 'Instruct AI Agent Bard': False, 'Ask AI Agent Vicuna': False, 'Instruct AI Agent Vicuna': False, 'Ask AI Agent OpenAI': False, 'Instruct AI Agent OpenAI': False, 'Ask AI Agent azure': False, 'Instruct AI Agent azure': False, 'Ask AI Agent ChatGPT': False, 'Instruct AI Agent ChatGPT': False, 'Ask AI Agent new_agent': False, 'Instruct AI Agent new_agent': False, 'Ask AI Agent Guanaco': False, 'Instruct AI Agent Guanaco': False, 'Write to File': False, 'Read File': False, 'Search Files': False, 'Append to File': False, 'Execute Python File': False, 'Delete File': False, 'Execute Shell': False, 'Read Audio from File': False, 'Read Audio': False, 'Generate Image with Stable Diffusion': False, 'Speak with TTS with BrianTTS': False, 'Clone Github Repository': False, 'Get Datetime': False, 'Speak with TTS Using Elevenlabs': False, 'Use The Search Engine': False, 'Create Task Chain': False, 'Create Smart Task Chain': False, 'Ask AI Agent new_agent_2': False, 'Instruct AI Agent new_agent_2': False}, 'settings': {'provider': 'gpt4free', 'AI_MODEL': 'gpt-3.5-turbo', 'AI_TEMPERATURE': 0.5, 'MAX_TOKENS': '4096', 'embedder': 'default', 'autonomous_execution': 'false'}}\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test update_agent_commands()\n",
@@ -634,47 +626,56 @@
             "metadata": {},
             "source": [
                 "## Have the Agent Learn from a File\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 128,
+            "execution_count": 172,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "File Learning response: Agent learned the content from the file.\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
+                "import base64\n",
+                "import os\n",
                 "\n",
                 "# Test learn_file()\n",
                 "agent_name = \"new_agent\"\n",
+                "learn_file_path = \"ApiClient.py\"\n",
+                "\n",
+                "with open(learn_file_path, \"rb\") as f:\n",
+                "    learn_file_content = base64.b64encode(f.read()).decode(\"utf-8\")\n",
+                "\n",
                 "file_learning = ApiClient.learn_file(\n",
-                "    agent_name=agent_name, file_name=\"test.txt\", file_content=\"This is a test file.\"\n",
+                "    agent_name=agent_name,\n",
+                "    file_name=learn_file_path,\n",
+                "    file_content=learn_file_content,\n",
                 ")\n",
                 "print(\"File Learning response:\", file_learning)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Have the Agent Learn from a URL\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 129,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "URL Learning response: Agent learned the content from the url.\n"
@@ -698,15 +699,15 @@
                 "## Wipe the agents memories\n",
                 "\n",
                 "This is necessary if you want the agent to serve a different purpose than its original intent after it has learned things. It may inject unnecessary context into the conversation if you don't wipe its memory and try to give it a different purpose, even temporarily.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 130,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Wipe agent memories response: Memories for agent new_agent deleted.\n"
@@ -737,15 +738,15 @@
             "metadata": {},
             "source": [
                 "## Get a list of Chains available to use\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 131,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Chains: ['Smart Instruct', 'Test_Commands', 'Generate and Run Smart Task Chain', 'Write a Poem', 'Generate and Run Task Chain', 'Generate Task Chain', 'Generate Smart Task Chain', 'Smart Chat']\n"
@@ -766,15 +767,15 @@
             "metadata": {},
             "source": [
                 "## Create a new chain\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 132,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Add chain response: Chain 'Write another Poem' created.\n"
@@ -796,15 +797,15 @@
             "metadata": {},
             "source": [
                 "## Rename the chain\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 133,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Rename chain response: Chain 'Write another Poem' renamed to 'Poem Writing Chain'.\n"
@@ -829,15 +830,15 @@
             "metadata": {},
             "source": [
                 "## Add Chain Steps\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 134,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Add step response: Step 1 added to chain 'Poem Writing Chain'.\n",
@@ -881,15 +882,15 @@
             "metadata": {},
             "source": [
                 "## Get the content of the chain\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 135,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Chain: {'chain_name': 'Poem Writing Chain', 'steps': [{'step': 1, 'agent_name': 'new_agent', 'prompt_type': 'Prompt', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Artificial Intelligence'}}, {'step': 2, 'agent_name': 'new_agent', 'prompt_type': 'Prompt', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Quantum Computers'}}]}\n"
@@ -913,15 +914,15 @@
                 "## Modify a chain step\n",
                 "\n",
                 "Instead of the subject of the poem just being Artificial Intelligence, we'll change it to be Artificial General Intelligence.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 136,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Update step response: Step 1 updated for chain 'Poem Writing Chain'.\n"
@@ -955,15 +956,15 @@
                 "## Move the chain step\n",
                 "\n",
                 "When you move a step, it will automatically reassign the order of the steps to match the new order. If there are only 2 steps like in our case, it will just swap them.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 137,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Move step response: Step 1 moved to 2 in chain 'Poem Writing Chain'.\n"
@@ -991,15 +992,15 @@
                 "## Add a Command to the Chain\n",
                 "\n",
                 "We'll write the result to a file for an example.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 138,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Add step response: Step 3 added to chain 'Poem Writing Chain'.\n"
@@ -1032,15 +1033,15 @@
             "metadata": {},
             "source": [
                 "## Run the chain\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 139,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Run chain response: {'1': {'response': \"Quantum computers, machines of wonder\\nWith qubits and gates to ponder\\nTheir power and speed beyond compare\\nA technological marvel, so rare.\\n\\nThey harness quantum physics' strange ways\\nTo solve problems in an astonishing craze\\nSimulating complex systems and more\\nTheir potential, endless, to explore.\\n\\nWith parallel universes to explore\\nQuantum computers will open new doors\\nTo knowledge and science, they'll lead the way\\nTo the discoveries of a brighter day.\\n\\nFrom cryptography to medicine and more\\nQuantum computers will help us explore\\nThe mysteries of our universe, vast and deep\\nWith great power, they'll help us reach.\\n\\nSo let us praise these machines of wonder\\nFor their potential, too great to ponder\\nQuantum computers, with their power and might\\nWill bring us closer to the light.\", 'agent_name': 'new_agent', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Quantum Computers'}, 'prompt_type': 'Prompt'}, '2': {'response': 'Artificial General Intelligence, a phrase so vast and deep\\nIt speaks of a world beyond our reach, where machines think and speak\\nWith their own kind of intelligence, separate from our own\\nA way of seeing, thinking, feeling, that\u2019s different, and yet somehow known\\n\\nAGI is a quest for man, to understand the mind\\nTo create intelligent machines that are of a similar kind\\nIt\u2019s a world beyond our reach, a place we\u2019ve never known\\nA world of pure intelligence, of metal, wires and chrome\\n\\nWe\u2019ve built machines to think before, but they\u2019re limited in their scope\\nAGI is different, it\u2019s a new kind of hope\\nA hope for a world where we can speak to our machines\\nAnd they will answer us with thoughts and hopes and dreams\\n\\nThe AI revolution is upon us, and AGI is the crown\\nIt will change the world forever, and turn it upside down\\nOur machines will be as smart as men, and much more efficient too\\nWe\u2019ll create a world of wonder, where anything we want to do, we\u2019ll do.\\n\\nSo let us claim this superpower, and build a new world with it\\nA world without limits, without boundaries or any limit\\nA world where our machines can think and speak, and where we\u2019ll all get along\\nA world where our machines can truly sing, and we\u2019ll all join in the song.', 'agent_name': 'new_agent', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Artificial General Intelligence'}, 'prompt_type': 'Prompt'}, '3': {'response': 'File written to successfully.', 'agent_name': 'new_agent', 'prompt': {'command_name': 'Write to File', 'filename': '{user_input}.txt', 'text': 'First Poem:\\n{STEP1}\\n\\nSecond Poem:\\n{STEP2}'}, 'prompt_type': 'Command'}}\n"
@@ -1064,15 +1065,15 @@
             "metadata": {},
             "source": [
                 "## Get the responses from the chain running\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 140,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Chain: {'1': {'response': \"Quantum computers, machines of wonder\\nWith qubits and gates to ponder\\nTheir power and speed beyond compare\\nA technological marvel, so rare.\\n\\nThey harness quantum physics' strange ways\\nTo solve problems in an astonishing craze\\nSimulating complex systems and more\\nTheir potential, endless, to explore.\\n\\nWith parallel universes to explore\\nQuantum computers will open new doors\\nTo knowledge and science, they'll lead the way\\nTo the discoveries of a brighter day.\\n\\nFrom cryptography to medicine and more\\nQuantum computers will help us explore\\nThe mysteries of our universe, vast and deep\\nWith great power, they'll help us reach.\\n\\nSo let us praise these machines of wonder\\nFor their potential, too great to ponder\\nQuantum computers, with their power and might\\nWill bring us closer to the light.\", 'agent_name': 'new_agent', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Quantum Computers'}, 'prompt_type': 'Prompt'}, '2': {'response': 'Artificial General Intelligence, a phrase so vast and deep\\nIt speaks of a world beyond our reach, where machines think and speak\\nWith their own kind of intelligence, separate from our own\\nA way of seeing, thinking, feeling, that\u2019s different, and yet somehow known\\n\\nAGI is a quest for man, to understand the mind\\nTo create intelligent machines that are of a similar kind\\nIt\u2019s a world beyond our reach, a place we\u2019ve never known\\nA world of pure intelligence, of metal, wires and chrome\\n\\nWe\u2019ve built machines to think before, but they\u2019re limited in their scope\\nAGI is different, it\u2019s a new kind of hope\\nA hope for a world where we can speak to our machines\\nAnd they will answer us with thoughts and hopes and dreams\\n\\nThe AI revolution is upon us, and AGI is the crown\\nIt will change the world forever, and turn it upside down\\nOur machines will be as smart as men, and much more efficient too\\nWe\u2019ll create a world of wonder, where anything we want to do, we\u2019ll do.\\n\\nSo let us claim this superpower, and build a new world with it\\nA world without limits, without boundaries or any limit\\nA world where our machines can think and speak, and where we\u2019ll all get along\\nA world where our machines can truly sing, and we\u2019ll all join in the song.', 'agent_name': 'new_agent', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Artificial General Intelligence'}, 'prompt_type': 'Prompt'}, '3': {'response': 'File written to successfully.', 'agent_name': 'new_agent', 'prompt': {'command_name': 'Write to File', 'filename': '{user_input}.txt', 'text': 'First Poem:\\n{STEP1}\\n\\nSecond Poem:\\n{STEP2}'}, 'prompt_type': 'Command'}}\n"
@@ -1095,15 +1096,15 @@
             "metadata": {},
             "source": [
                 "## Delete a step from the chain\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 141,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Delete step response: Step 2 deleted from chain 'Poem Writing Chain'.\n"
@@ -1125,15 +1126,15 @@
             "metadata": {},
             "source": [
                 "## Delete the chain\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 142,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Delete chain response: Chain 'Poem Writing Chain' deleted.\n"
@@ -1157,15 +1158,15 @@
                 "# Prompts\n",
                 "\n",
                 "## Get a list of prompts available to use\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 143,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Prompts: ['Pseudo Code', 'SmartInstruct-Researcher', 'Custom Input', 'Title a Poem', 'ValidationFailed', 'SmartTask-CleanResponse', 'SmartChat-Researcher', 'Tell Me How', 'Execution', 'Score Response', 'Get Task Description', 'Validation', 'Write a Haiku', 'SmartInstruct-Resolver', 'SmartInstruct-CleanResponse', 'SmartInstruct-StepByStep', 'instruct', 'Pick a Poem Subject', 'Task Execution', 'Check-Instruction', 'SmartTask-Execution', 'SmartChat-Resolver', 'Chat', 'Create New Command', 'SmartChat-CleanResponse', 'Prioritize', 'Pick-a-Link', 'SmartInstruct-Execution', 'Write a Poem', 'JSONFormatter', 'SmartTask-StepByStep', 'Instruction', 'WebSearch', 'SmartChat-StepByStep', 'Get Task List']\n"
@@ -1188,15 +1189,15 @@
                 "## Create a new prompt\n",
                 "\n",
                 "We'll make a basic prompt that asks the AI to tell us a short story about a subject. The subject is not yet defined, it would be defined in a chain. Using `{variable_name}` in a prompt will allow you to define the variable in a chain and have it be used in the prompt.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 144,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Add prompt response: Prompt 'Short Story' added.\n"
@@ -1219,15 +1220,15 @@
             "metadata": {},
             "source": [
                 "## Get the prompt content\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 145,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Get prompt response: Write a poem about {subject} .\n",
@@ -1249,15 +1250,15 @@
             "metadata": {},
             "source": [
                 "## Get the prompt variables\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 146,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Get prompt args response: ['subject']\n"
@@ -1281,15 +1282,15 @@
                 "## Update the prompt content\n",
                 "\n",
                 "We'll ask it to `Add a dragon to the story somehow` in the prompt to make the short story more interesting.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 147,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Update prompt response: Prompt 'Short Story' updated.\n"
@@ -1315,15 +1316,15 @@
                 "## Delete the prompt\n",
                 "\n",
                 "If you don't want the prompt anymore, delete it.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 148,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Delete prompt response: Prompt 'Short Story' deleted.\n"
@@ -1346,15 +1347,15 @@
                 "## Delete Agent History\n",
                 "\n",
                 "Delete the history for the agent.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 149,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Delete agent response: History for agent new_agent deleted.\n"
@@ -1378,15 +1379,15 @@
                 "## Delete the Agent\n",
                 "\n",
                 "If you are done with the agent and don't want or need it anymore, you can delete it along with everything associated with it, such as its memories, settings, and history. The Agent isn't just fired, it is dead.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 150,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Delete agent response: Agent new_agent deleted.\n"
```

