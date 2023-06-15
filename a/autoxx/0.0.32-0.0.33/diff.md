# Comparing `tmp/autoxx-0.0.32.tar.gz` & `tmp/autoxx-0.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.32.tar", max compression
+gzip compressed data, was "autoxx-0.0.33.tar", max compression
```

## Comparing `autoxx-0.0.32.tar` & `autoxx-0.0.33.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.32/README.md
--rw-r--r--   0        0        0     7808 2023-06-14 07:11:34.884437 autoxx-0.0.32/autoxx/agent/babyagi/agi.py
--rw-r--r--   0        0        0     3623 2023-06-14 04:47:16.286995 autoxx-0.0.32/autoxx/agent/babyagi/task_manager.py
--rw-r--r--   0        0        0    10487 2023-05-27 10:37:00.472121 autoxx-0.0.32/autoxx/agent/react/agent.py
--rw-r--r--   0        0        0     6070 2023-06-14 03:10:17.811860 autoxx-0.0.32/autoxx/config/config.py
--rw-r--r--   0        0        0      244 2023-06-14 02:27:24.680814 autoxx-0.0.32/autoxx/setup.py
--rw-r--r--   0        0        0     7659 2023-06-14 01:42:51.264483 autoxx-0.0.32/autoxx/tools/knowledge_base/base.py
--rw-r--r--   0        0        0      409 2023-06-14 01:47:30.199685 autoxx-0.0.32/autoxx/tools/llm/base.py
--rw-r--r--   0        0        0      788 2023-05-26 05:35:16.597623 autoxx-0.0.32/autoxx/tools/web_search/js/overlay.js
--rw-r--r--   0        0        0    13243 2023-06-14 02:32:00.475100 autoxx-0.0.32/autoxx/tools/web_search/search.py
--rw-r--r--   0        0        0     1060 2023-05-27 00:53:33.776643 autoxx-0.0.32/autoxx/utils/base.py
--rw-r--r--   0        0        0     3197 2023-06-14 06:49:37.535797 autoxx-0.0.32/autoxx/utils/llm.py
--rw-r--r--   0        0        0     2271 2023-06-14 03:11:09.896898 autoxx-0.0.32/autoxx/utils/openai_models.py
--rw-r--r--   0        0        0      928 2023-05-26 07:29:31.512652 autoxx-0.0.32/autoxx/utils/processing_html.py
--rw-r--r--   0        0        0     5553 2023-06-14 02:32:02.094489 autoxx-0.0.32/autoxx/utils/processing_text.py
--rw-r--r--   0        0        0     2676 2023-06-14 03:38:54.107786 autoxx-0.0.32/autoxx/utils/token_counter.py
--rw-r--r--   0        0        0      660 2023-06-14 06:57:57.644730 autoxx-0.0.32/pyproject.toml
--rw-r--r--   0        0        0     1047 1970-01-01 00:00:00.000000 autoxx-0.0.32/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.33/README.md
+-rw-r--r--   0        0        0     7808 2023-06-14 07:11:34.884437 autoxx-0.0.33/autoxx/agent/babyagi/agi.py
+-rw-r--r--   0        0        0     3623 2023-06-14 04:47:16.286995 autoxx-0.0.33/autoxx/agent/babyagi/task_manager.py
+-rw-r--r--   0        0        0    10487 2023-05-27 10:37:00.472121 autoxx-0.0.33/autoxx/agent/react/agent.py
+-rw-r--r--   0        0        0     6070 2023-06-14 03:10:17.811860 autoxx-0.0.33/autoxx/config/config.py
+-rw-r--r--   0        0        0      244 2023-06-14 02:27:24.680814 autoxx-0.0.33/autoxx/setup.py
+-rw-r--r--   0        0        0     7895 2023-06-15 10:14:04.414108 autoxx-0.0.33/autoxx/tools/knowledge_base/base.py
+-rw-r--r--   0        0        0      409 2023-06-14 01:47:30.199685 autoxx-0.0.33/autoxx/tools/llm/base.py
+-rw-r--r--   0        0        0      788 2023-05-26 05:35:16.597623 autoxx-0.0.33/autoxx/tools/web_search/js/overlay.js
+-rw-r--r--   0        0        0    13277 2023-06-15 02:57:54.299087 autoxx-0.0.33/autoxx/tools/web_search/search.py
+-rw-r--r--   0        0        0     1060 2023-06-15 03:38:02.463809 autoxx-0.0.33/autoxx/utils/base.py
+-rw-r--r--   0        0        0     3197 2023-06-15 10:05:15.563247 autoxx-0.0.33/autoxx/utils/llm.py
+-rw-r--r--   0        0        0     2271 2023-06-14 03:11:09.896898 autoxx-0.0.33/autoxx/utils/openai_models.py
+-rw-r--r--   0        0        0      928 2023-05-26 07:29:31.512652 autoxx-0.0.33/autoxx/utils/processing_html.py
+-rw-r--r--   0        0        0     5553 2023-06-14 02:32:02.094489 autoxx-0.0.33/autoxx/utils/processing_text.py
+-rw-r--r--   0        0        0     2631 2023-06-15 01:51:01.679558 autoxx-0.0.33/autoxx/utils/token_counter.py
+-rw-r--r--   0        0        0      684 2023-06-15 10:15:09.470687 autoxx-0.0.33/pyproject.toml
+-rw-r--r--   0        0        0     1101 1970-01-01 00:00:00.000000 autoxx-0.0.33/PKG-INFO
```

### Comparing `autoxx-0.0.32/autoxx/agent/babyagi/agi.py` & `autoxx-0.0.33/autoxx/agent/babyagi/agi.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.32/autoxx/agent/babyagi/task_manager.py` & `autoxx-0.0.33/autoxx/agent/babyagi/task_manager.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.32/autoxx/agent/react/agent.py` & `autoxx-0.0.33/autoxx/agent/react/agent.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.32/autoxx/config/config.py` & `autoxx-0.0.33/autoxx/config/config.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.32/autoxx/tools/knowledge_base/base.py` & `autoxx-0.0.33/autoxx/tools/knowledge_base/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,19 +137,24 @@
             print("Error:", e)
             raise Exception(f"failed to retrieve nodes: {str(e)}")
 
     def upsert_document(self, documents: List[Document]) -> None:
         self.index.docstore.add_documents(documents, allow_update=True)
         for document in documents:
             nodes = self.index.service_context.node_parser.get_nodes_from_documents([document])
+            print(nodes)
             self.index.insert_nodes(nodes)
 
     def delete_document(self, document_id: str) -> None:
-        self.index.delete(document_id)
+        self.index.delete_ref_doc(document_id)
         self.index.docstore.delete_document(document_id)
+        try:
+            self.vector_store.delete(document_id, namespace=self.namespace)
+        except Exception as e:
+            print(f"failed to delete vector for document {document_id}: {str(e)}")
 
     def retrieve_document(self, document_ids: List[str]) ->  List[Document]:
         if document_ids is None or len(document_ids) == 0:
             return [doc for _, doc in self.index.docstore.docs.items()]
 
         documents = []
         for document_id in document_ids:
```

### Comparing `autoxx-0.0.32/autoxx/tools/web_search/js/overlay.js` & `autoxx-0.0.33/autoxx/tools/web_search/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.32/autoxx/tools/web_search/search.py` & `autoxx-0.0.33/autoxx/tools/web_search/search.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,22 @@
 from autoxx.utils.llm import get_chat_completion
 from autoxx.utils.processing_text import split_text
 from autoxx.utils.token_counter import count_message_tokens
 from autoxx.utils.processing_html import extract_hyperlinks, format_hyperlinks
 from autoxx.utils.base import Message
 
 BrowserOptions = ChromeOptions | EdgeOptions | FirefoxOptions | SafariOptions
+BrowserSummaryModel = "gpt-3.5-turbo-16k"
 MaxSummaryTokenSize = 2048
+summary_response_format = {
+    "relevant_content": "Extract all information in detail relevant to question. if there is no relevant information, summarize the text briefly.",
+    "relevance": "Yes/No # Whether there is a relevance",
+}
+formatted_summary_response_format = json.dumps(summary_response_format, indent=4)
+
 
 FILE_DIR = Path(__file__).parent
 
 def create_summary_message(chunk: str, question: str) -> Message:
     """Create a message for the chat completion
 
     Args:
@@ -46,41 +53,21 @@
     Returns:
         Dict[str, str]: The message to send to the chat completion
     """
     return Message(
         role="user", 
         content=(
             f'"""{chunk}""" Analyze the above text and extract all information in detail relevant to '
-            f'question: "{question}" -- if there is no relevant information, summarize the text in detail.'
+            f'question: "{question}" -- if there is no relevant information, summarize the text.'
+            f"\nResponse Format: \n{formatted_summary_response_format} "
+            f"\nEnsure the response can be parsed by Python json.loads"
         )
     )
 
-def no_relevance(chunk: str, question: str, model: str) -> bool:
-    """Create a message for the chat completion
-
-    Args:
-        chunk (str): The chunk of text to summarize
-        question (str): The question to answer
-
-    Returns:
-        Dict[str, str]: The message to send to the chat completion
-    """
-    messages = [Message(
-        role="user",
-        content=(
-            f'"""{chunk}""" Analyze the above text and determine if it is relevant to the '
-            f'question: "{question}"\nPlease answer only "Yes" or "No"'
-        )
-    )]
-
-    answer = get_chat_completion(
-        model=model,
-        messages=messages,
-    )
-
+def no_relevance(answer: str) -> bool:
     return answer.strip().replace(".", "").lower() == "no"
 
 def scroll_to_percentage(driver: WebDriver, ratio: float) -> None:
     """Scroll to a percentage of the page
 
     Args:
         driver (WebDriver): The webdriver to use
@@ -194,45 +181,46 @@
     Args:
         chunks (list[str]): The chunks to summarize
         question (str): The question to answer
 
     Returns:
         str: The summary of the chunks
     """
-    model = "gpt-3.5-turbo"
     logging.debug(f"Memorizing text:\n{'-'*32}\n{text}\n{'-'*32}\n")
     chunks = [
         chunk
         for chunk, _ in (
-            split_text(text, for_model=model)
+            split_text(text, for_model=BrowserSummaryModel)
         )
     ]
 
     summaries = []
     scroll_ratio = 1 / len(chunks)
     for i, chunk in enumerate(chunks):
         if driver:
             scroll_to_percentage(driver, scroll_ratio * i)
 
         messages = [create_summary_message(chunk, question)]
         tokens_for_chunk = count_message_tokens(messages)
 
-        if no_relevance(chunk, question, model):
-            logging.info(f"Skipping chunk {i + 1} / {len(chunks)} of length {len(chunk)} characters, or {tokens_for_chunk} tokens, not relevant.")
-            continue
-
         logging.info(
             f"Summarizing {url} chunk {i + 1} / {len(chunks)} of length {len(chunk)} characters, or {tokens_for_chunk} tokens"
         )
 
-        summary = get_chat_completion(
-            model=model,
+        summary_response_str = get_chat_completion(
+            model=BrowserSummaryModel,
             messages=messages,
         )
 
+        summary_response = json.loads(summary_response_str)
+        if no_relevance(summary_response.get("relevance", "")):
+            logging.info(f"Skipping chunk {i + 1} / {len(chunks)} of length {len(chunk)} characters, or {tokens_for_chunk} tokens, not relevant.")
+            continue
+        summary = summary_response.get("relevant_content", summary_response_str)
+
         logging.info(f"Chunk {i + 1} / {len(chunks)} summary.\n{summary}")
 
         summaries.append(summary)
 
     return summaries
 
 def add_header(driver: WebDriver) -> None:
@@ -283,15 +271,14 @@
     add_header(driver)
 
     summaries = summarize_chunks(text=text, question=question, url=url, driver=driver)
     text_gen = "\n".join(summaries)
     while count_message_tokens([create_summary_message(text_gen, question)]) > MaxSummaryTokenSize:
        summaries = summarize_chunks(text=text_gen, question=question, url=url, driver=driver)
        text_gen = "\n".join(summaries)
-       print(text_gen)
 
     if len(text_gen) == 0:
         close_browser(driver)
         return None
 
     links = scrape_links_with_selenium(driver, url)
     # Limit links to 5
```

### Comparing `autoxx-0.0.32/autoxx/utils/base.py` & `autoxx-0.0.33/autoxx/utils/base.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.32/autoxx/utils/llm.py` & `autoxx-0.0.33/autoxx/utils/llm.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.32/autoxx/utils/openai_models.py` & `autoxx-0.0.33/autoxx/utils/openai_models.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.32/autoxx/utils/processing_html.py` & `autoxx-0.0.33/autoxx/utils/processing_html.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.32/autoxx/utils/processing_text.py` & `autoxx-0.0.33/autoxx/utils/processing_text.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.32/autoxx/utils/token_counter.py` & `autoxx-0.0.33/autoxx/utils/token_counter.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,21 +19,21 @@
         int: The number of tokens used by the list of messages.
     """
     try:
         encoding = tiktoken.encoding_for_model(model)
     except KeyError:
         logging.warn("Warning: model not found. Using cl100k_base encoding.")
         encoding = tiktoken.get_encoding("cl100k_base")
-    if model in ("gpt-3.5-turbo-0301", "gpt-3.5-turbo-16k", "gpt-3.5-turbo-0613"):
+    if model.startswith("gpt-3.5-turbo-"):
         # !Note: gpt-3.5-turbo may change over time.
         # Returning num tokens assuming gpt-3.5-turbo-0301.")
-        return count_message_tokens(messages, model="gpt-3.5-turbo-0301")
-    elif model == "gpt-4-0314":
+        return count_message_tokens(messages, model="gpt-3.5-turbo")
+    elif model.startswith("gpt-4-"):
         # !Note: gpt-4 may change over time. Returning num tokens assuming gpt-4-0314.")
-        return count_message_tokens(messages, model="gpt-4-0314")
+        return count_message_tokens(messages, model="gpt-4")
     elif model == "gpt-3.5-turbo":
         tokens_per_message = (
             4  # every message follows <|start|>{role/name}\n{content}<|end|>\n
         )
         tokens_per_name = -1  # if there's a name, the role is omitted
     elif model == "gpt-4":
         tokens_per_message = 3
```

### Comparing `autoxx-0.0.32/pyproject.toml` & `autoxx-0.0.33/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.32"
+version = "0.0.33"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pinecone-client = "2.2.1"
 selenium = "4.9.0"
-openai = "0.27.6"
+openai = "^0.27.8"
 colorama = "^0.4.6"
 python-dotenv = "1.0.0"
 bs4 = "0.0.1"
 webdriver_manager = "3.8.6"
 tiktoken = "0.3.3"
 playsound = "1.2.2"
 gTTS = "2.3.1"
 orjson = "3.8.10"
 spacy = ">=3.0.0,<4.0.0"
 llama-index = "^0.6.23"
 google-api-python-client = "^2.86.0"
 pymongo = "^4.3.3"
 transformers = "^4.30.1"
+langchain = "^0.0.200"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `autoxx-0.0.32/PKG-INFO` & `autoxx-0.0.33/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.32
+Version: 0.0.33
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bs4 (==0.0.1)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: gTTS (==2.3.1)
 Requires-Dist: google-api-python-client (>=2.86.0,<3.0.0)
+Requires-Dist: langchain (>=0.0.200,<0.0.201)
 Requires-Dist: llama-index (>=0.6.23,<0.7.0)
-Requires-Dist: openai (==0.27.6)
+Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: orjson (==3.8.10)
 Requires-Dist: pinecone-client (==2.2.1)
 Requires-Dist: playsound (==1.2.2)
 Requires-Dist: pymongo (>=4.3.3,<5.0.0)
 Requires-Dist: python-dotenv (==1.0.0)
 Requires-Dist: selenium (==4.9.0)
 Requires-Dist: spacy (>=3.0.0,<4.0.0)
```

