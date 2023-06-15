# Comparing `tmp/pandasai-0.5.2.tar.gz` & `tmp/pandasai-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.5.2.tar", max compression
+gzip compressed data, was "pandasai-0.5.3.tar", max compression
```

## Comparing `pandasai-0.5.2.tar` & `pandasai-0.5.3.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     1055 2023-06-12 22:28:47.671282 pandasai-0.5.2/LICENSE
--rw-r--r--   0        0        0     9138 2023-06-12 22:28:47.671282 pandasai-0.5.2/README.md
--rw-r--r--   0        0        0    20547 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/__init__.py
--rw-r--r--   0        0        0     1423 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/constants.py
--rw-r--r--   0        0        0     1509 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3787 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5434 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1825 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      566 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1493 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3252 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0        0 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4354 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    10683 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/llm/base.py
--rw-r--r--   0        0        0      542 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1213 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/llm/falcon.py
--rw-r--r--   0        0        0     1828 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0     1482 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     2869 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1220 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/middlewares/__init__.py
--rw-r--r--   0        0        0      663 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/middlewares/base.py
--rw-r--r--   0        0        0      558 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/middlewares/charts.py
--rw-r--r--   0        0        0      595 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/middlewares/streamlit.py
--rw-r--r--   0        0        0        0 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      647 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1737 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1262 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1554 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      460 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1343 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1557 2023-06-12 22:28:47.679282 pandasai-0.5.2/pyproject.toml
--rw-r--r--   0        0        0    10060 1970-01-01 00:00:00.000000 pandasai-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-06-15 10:45:52.718959 pandasai-0.5.3/LICENSE
+-rw-r--r--   0        0        0     7123 2023-06-15 10:45:52.718959 pandasai-0.5.3/README.md
+-rw-r--r--   0        0        0    20746 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/__init__.py
+-rw-r--r--   0        0        0     1423 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/constants.py
+-rw-r--r--   0        0        0     1509 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3787 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5434 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1825 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      566 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1493 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3252 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4354 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    10885 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/llm/base.py
+-rw-r--r--   0        0        0      542 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1213 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     1828 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0      841 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     1482 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     2932 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1220 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/middlewares/__init__.py
+-rw-r--r--   0        0        0      663 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/middlewares/base.py
+-rw-r--r--   0        0        0      558 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/middlewares/charts.py
+-rw-r--r--   0        0        0      595 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/middlewares/streamlit.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      647 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1697 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1262 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1514 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      460 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1343 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1636 2023-06-15 10:45:52.730959 pandasai-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     8140 1970-01-01 00:00:00.000000 pandasai-0.5.3/PKG-INFO
```

### Comparing `pandasai-0.5.2/LICENSE` & `pandasai-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.2/README.md` & `pandasai-0.5.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,69 @@
+Metadata-Version: 2.1
+Name: pandasai
+Version: 0.5.3
+Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
+License: MIT
+Author: Gabriele Venturi
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: google
+Provides-Extra: langchain
+Provides-Extra: tests
+Requires-Dist: astor (>=0.8.1,<0.9.0)
+Requires-Dist: google-generativeai (>=0.1.0rc2,<0.2.0) ; extra == "google"
+Requires-Dist: ipython (>=8.13.1,<9.0.0)
+Requires-Dist: langchain (>=0.0.199,<0.0.200) ; extra == "langchain"
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: openai (>=0.27.5,<0.28.0)
+Requires-Dist: pandas (==1.5.3)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Description-Content-Type: text/markdown
+
 # PandasAI 🐼
 
 [![Release](https://img.shields.io/pypi/v/pandasai?label=Release&style=flat-square)](https://pypi.org/project/pandasai/)
 [![CI](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)
 [![CD](https://github.com/gventuri/pandas-ai/actions/workflows/cd.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/cd.yml/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/pandas-ai/badge/?version=latest)](https://pandas-ai.readthedocs.io/en/latest/?badge=latest)
 [![](https://dcbadge.vercel.app/api/server/kF7FqH2FwS?style=flat&compact=true)](https://discord.gg/kF7FqH2FwS)
-[![Downloads](https://static.pepy.tech/badge/pandasai/month)](https://pepy.tech/project/pandasai) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![Downloads](https://static.pepy.tech/badge/pandasai)](https://pepy.tech/project/pandasai) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/1rKz7TudOeCeKGHekw7JFNL4sagN9hon-?usp=sharing)
 
-Pandas AI is a Python library that adds generative artificial intelligence capabilities to Pandas, the popular data analysis and manipulation tool. It is designed to be used in conjunction with Pandas, and is not a replacement for it.
+PandasAI is a Python library that adds Generative AI capabilities to [pandas](https://github.com/pandas-dev/pandas), the popular data analysis and manipulation tool. It is designed to be used in conjunction with pandas, and is not a replacement for it.
 
 <!-- Add images/pandas-ai.png -->
 
 ![PandasAI](images/pandas-ai.png?raw=true)
 
-## Demo
+## 🔧 Quick install
+
+```bash
+pip install pandasai
+```
+
+## 🔍 Demo
 
 Try out PandasAI in your browser:
 
 [![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/1rKz7TudOeCeKGHekw7JFNL4sagN9hon-?usp=sharing)
 
-## Documentation
+## 📖 Documentation
 
 The documentation for PandasAI can be found [here](https://pandas-ai.readthedocs.io/en/latest/).
 
-## Installation
-
-```bash
-pip install pandasai
-```
-
-## Usage
+## 💻 Usage
 
 > Disclaimer: GDP data was collected from [this source](https://ourworldindata.org/grapher/gross-domestic-product?tab=table), published by World Development Indicators - World Bank (2022.05.26) and collected at National accounts data - World Bank / OECD. It relates to the year of 2020. Happiness indexes were extracted from [the World Happiness Report](https://ftnnews.com/images/stories/documents/2020/WHR20.pdf). Another useful [link](https://data.world/makeovermonday/2020w19-world-happiness-report-2020).
 
-PandasAI is designed to be used in conjunction with [pandas](https://github.com/pandas-dev/pandas). It makes Pandas conversational, allowing you to ask questions about your data and get answers back, in the form of pandas DataFrames.
+PandasAI is designed to be used in conjunction with pandas. It makes pandas conversational, allowing you to ask questions to your data in natural language.
 
 ### Queries
 
 For example, you can ask PandasAI to find all the rows in a DataFrame where the value of a column is greater than 5, and it will return a DataFrame containing only those rows:
 
 ```python
 import pandas as pd
@@ -129,115 +154,39 @@
 
 ```
 Oh, Olivia gets paid the most.
 ```
 
 You can find more examples in the [examples](examples) directory.
 
-## Command-Line Tool
-
-Pai is the command line tool designed to provide a convenient way to interact with PandasAI through a command line interface (CLI). In order to access the CLI tool, make sure to create a virtualenv for testing purpose and to install project dependencies in your local virtual environment using `pip` by running the following command:
-
-```
-pip install -e .
-```
-
-Alternatively, you can use `poetry` to create and activate the virtual environment by running the following command:
-
-```
-poetry shell
-```
-
-Inside the activated virtual environment, install the project dependencies by running the following command:
-
-```
-poetry install
-```
-
-By following these steps, you will now have the necessary environment to access the CLI tool.
-
-```
-pai [OPTIONS]
-```
-
-Options:
-
-- **-d, --dataset**: The file path to the dataset.
-- **-t, --token**: Your HuggingFace or OpenAI API token, if no token provided pai will pull from the `.env` file.
-- **-m, --model**: Choice of LLM, either `openai`, `open-assistant`, `starcoder`, `falcon`, `azure-openai` or `google-palm`.
-- **-p, --prompt**: Prompt that PandasAI will run.
-
-To view a full list of available options and their descriptions, run the following command:
-
-```
-pai --help
-
-```
-
-> For example,
->
-> ```
-> pai -d "~/pandasai/example/data/Loan payments data.csv" -m "openai" -p "How many loans are from men and have been paid off?"
-> ```
->
-> Should result in the same output as the `from_csv.py` example.
-
-## Privacy & Security
+## 🔒 Privacy & Security
 
 In order to generate the Python code to run, we take the dataframe head, we randomize it (using random generation for sensitive data and shuffling for non-sensitive data) and send just the head.
 
 Also, if you want to enforce further your privacy you can instantiate PandasAI with `enforce_privacy = True` which will not send the head (but just column names) to the LLM.
 
-## Environment Variables
-
-In order to set the API key for the LLM (Hugging Face Hub, OpenAI), you need to set the appropriate environment variables. You can do this by copying the `.env.example` file to `.env`:
-
-```bash
-cp .env.example .env
-```
-
-Then, edit the `.env` file and set the appropriate values.
+## ⚙️ Command-Line Tool
 
-As an alternative, you can also pass the environment variables directly to the constructor of the LLM:
-
-```python
-# OpenAI
-llm = OpenAI(api_token="YOUR_API_KEY")
-
-# Starcoder
-llm = Starcoder(api_token="YOUR_HF_API_KEY")
-
-# Falcon
-llm = Falcon(api_token="YOUR_HF_API_KEY")
-```
-
-Please note that at the moment OpenAI provides the best results, as the prompts are specifically designed for OpenAI and might hallucinate with other LLMs.
-
-## License
+Pai is the command line tool designed to provide a convenient way to interact with PandasAI through a command line interface (CLI). In order to access the CLI tool, make sure to create a virtualenv for testing purpose and to install project dependencies in your local virtual environment using `pip` by running the following command:
 
-PandasAI is licensed under the MIT License. See the LICENSE file for more details.
+Read more about how to use the CLI [here](https://pandas-ai.readthedocs.io/en/latest/pai_cli/).
 
-## Contributing
+## 🤝 Contributing
 
 Contributions are welcome! Please check out the todos below, and feel free to open a pull request.
 For more information, please see the [contributing guidelines](CONTRIBUTING.md).
 
 After installing the virtual environment, please remember to install `pre-commit` to be compliant with our standards:
 
 ```bash
 pre-commit install
 ```
 
+## 📜 License
+
+PandasAI is licensed under the MIT License. See the LICENSE file for more details.
+
 ## Acknowledgements
 
 - This project is based on the [pandas](https://github.com/pandas-dev/pandas) library by independent contributors, but it's in no way affiliated with the pandas project.
 - This project is meant to be used as a tool for data exploration and analysis, and it's not meant to be used for production purposes. Please use it responsibly.
 
-### Todo
-
-- [x] Add support for more LLMs
-- [x] Make PandasAI available from a CLI
-- [ ] Create a web interface for PandasAI
-- [x] Add unit tests
-- [x] Add contributing guidelines
-- [x] Add CI
-- [x] Add support for conversational responses
```

### Comparing `pandasai-0.5.2/pandasai/__init__.py` & `pandasai-0.5.3/pandasai/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 from .exceptions import BadImportError, LLMNotFoundError
 from .helpers._optional import import_dependency
 from .helpers.anonymizer import anonymize_dataframe_head
 from .helpers.cache import Cache
 from .helpers.notebook import Notebook
 from .helpers.save_chart import add_save_chart
 from .llm.base import LLM
+from .llm.langchain import LangchainLLM
 from .middlewares.base import Middleware
 from .middlewares.charts import ChartsMiddleware
 from .prompts.correct_error_prompt import CorrectErrorPrompt
 from .prompts.correct_multiples_prompt import CorrectMultipleDataframesErrorPrompt
 from .prompts.generate_python_code import GeneratePythonCodePrompt
 from .prompts.generate_response import GenerateResponsePrompt
 from .prompts.multiple_dataframes import MultipleDataframesPrompt
@@ -109,15 +110,14 @@
     _max_retries: int = 3
     _is_notebook: bool = False
     _original_instructions: dict = {
         "question": None,
         "df_head": None,
         "num_rows": None,
         "num_columns": None,
-        "rows_to_display": None,
     }
     _cache: Cache = Cache()
     _enable_cache: bool = True
     _prompt_id: Optional[str] = None
     _middlewares: List[Middleware] = [ChartsMiddleware()]
     _additional_dependencies: List[dict] = []
     _custom_whitelisted_dependencies: List[str] = []
@@ -172,15 +172,15 @@
         )
         self._logger = logging.getLogger(__name__)
 
         if llm is None:
             raise LLMNotFoundError(
                 "An LLM should be provided to instantiate a PandasAI instance"
             )
-        self._llm = llm
+        self._load_llm(llm)
         self._is_conversational_answer = conversational
         self._verbose = verbose
         self._enforce_privacy = enforce_privacy
         self._save_charts = save_charts
         self._enable_cache = enable_cache
         self._process_id = str(uuid.uuid4())
 
@@ -189,14 +189,34 @@
 
         if middlewares is not None:
             self.add_middlewares(*middlewares)
 
         if custom_whitelisted_dependencies is not None:
             self._custom_whitelisted_dependencies = custom_whitelisted_dependencies
 
+    def _load_llm(self, llm):
+        """
+        Check if it is a PandasAI LLM or a Langchain LLM.
+        If it is a Langchain LLM, wrap it in a PandasAI LLM.
+
+        Args:
+            llm (object): LLMs option to be used for API access
+
+        Raises:
+            BadImportError: If the LLM is a Langchain LLM but the langchain package
+            is not installed
+        """
+
+        try:
+            llm.is_pandasai_llm()
+        except AttributeError:
+            llm = LangchainLLM(llm)
+
+        self._llm = llm
+
     def conversational_answer(self, question: str, answer: str) -> str:
         """
         Returns the answer in conversational form about the resultant data.
 
         Args:
             question (str): A question in Conversational form
             answer (str): A summary / resultant Data
@@ -266,39 +286,36 @@
                         MultipleDataframesPrompt(dataframes=heads),
                         prompt,
                     )
 
                     self._original_instructions = {
                         "question": prompt,
                         "df_head": heads,
-                        "rows_to_display": rows_to_display,
                     }
 
                 else:
                     df_head = data_frame.head(rows_to_display)
                     if anonymize_df:
                         df_head = anonymize_dataframe_head(df_head)
 
                     code = self._llm.generate_code(
                         GeneratePythonCodePrompt(
                             prompt=prompt,
                             df_head=df_head,
                             num_rows=data_frame.shape[0],
                             num_columns=data_frame.shape[1],
-                            rows_to_display=rows_to_display,
                         ),
                         prompt,
                     )
 
                     self._original_instructions = {
                         "question": prompt,
                         "df_head": df_head,
                         "num_rows": data_frame.shape[0],
                         "num_columns": data_frame.shape[1],
-                        "rows_to_display": rows_to_display,
                     }
 
                 self.last_code_generated = code
                 self.log(
                     f"""
                         Code generated:
                         ```
@@ -556,17 +573,14 @@
                         error_correcting_instruction = CorrectErrorPrompt(
                             code=code,
                             error_returned=e,
                             question=self._original_instructions["question"],
                             df_head=self._original_instructions["df_head"],
                             num_rows=self._original_instructions["num_rows"],
                             num_columns=self._original_instructions["num_columns"],
-                            rows_to_display=self._original_instructions[
-                                "rows_to_display"
-                            ],
                         )
 
                     code_to_run = self._llm.generate_code(
                         error_correcting_instruction, ""
                     )
 
         captured_output = output.getvalue()
```

### Comparing `pandasai-0.5.2/pandasai/constants.py` & `pandasai-0.5.3/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.2/pandasai/exceptions.py` & `pandasai-0.5.3/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.2/pandasai/helpers/_optional.py` & `pandasai-0.5.3/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.2/pandasai/helpers/anonymizer.py` & `pandasai-0.5.3/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.2/pandasai/helpers/cache.py` & `pandasai-0.5.3/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.2/pandasai/helpers/from_excel.py` & `pandasai-0.5.3/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.2/pandasai/helpers/notebook.py` & `pandasai-0.5.3/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.2/pandasai/helpers/save_chart.py` & `pandasai-0.5.3/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.2/pandasai/llm/azure_openai.py` & `pandasai-0.5.3/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.2/pandasai/llm/base.py` & `pandasai-0.5.3/pandasai/llm/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,23 @@
 
 
 class LLM:
     """Base class to implement a new LLM."""
 
     last_prompt: Optional[str] = None
 
+    def is_pandasai_llm(self) -> bool:
+        """
+        Return True if the LLM is from pandasAI.
+
+        Returns:
+            bool: True if the LLM is from pandasAI
+        """
+        return True
+
     @property
     def type(self) -> str:
         """
         Return type of LLM.
 
         Raises:
             APIKeyNotFoundError: Type has not been implemented
```

### Comparing `pandasai-0.5.2/pandasai/llm/fake.py` & `pandasai-0.5.3/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.2/pandasai/llm/falcon.py` & `pandasai-0.5.3/pandasai/llm/falcon.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.2/pandasai/llm/google_palm.py` & `pandasai-0.5.3/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.2/pandasai/llm/open_assistant.py` & `pandasai-0.5.3/pandasai/llm/open_assistant.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         "https://api-inference.huggingface.co/models/"
         "OpenAssistant/oasst-sft-1-pythia-12b"
     )
     _max_retries: int = 10
 
     def __init__(self, api_token: Optional[str] = None):
         """
-        __init__ method of OpenAssistant Calss
+        __init__ method of OpenAssistant Class
 
         Raises:
             APIKeyNotFoundError: HuggingFace Hub API key is required
 
         Args:
             api_token (str): API token from Huggingface platform
         """
```

### Comparing `pandasai-0.5.2/pandasai/llm/openai.py` & `pandasai-0.5.3/pandasai/llm/openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,19 +30,21 @@
     The list of supported Chat models includes ["gpt-4", "gpt-4-0314", "gpt-4-32k",
      "gpt-4-32k-0314","gpt-3.5-turbo", "gpt-3.5-turbo-0301"].
 
     """
 
     _supported_chat_models = [
         "gpt-4",
-        "gpt-4-0314",
+        "gpt-4-0613",
         "gpt-4-32k",
-        "gpt-4-32k-0314",
+        "gpt-4-32k-0613",
         "gpt-3.5-turbo",
-        "gpt-3.5-turbo-0301",
+        "gpt-3.5-turbo-16k",
+        "gpt-3.5-turbo-0613",
+        "gpt-3.5-turbo-16k-0613",
     ]
     _supported_completion_models = ["text-davinci-003"]
 
     model: str = "gpt-3.5-turbo"
 
     def __init__(
         self,
```

### Comparing `pandasai-0.5.2/pandasai/llm/starcoder.py` & `pandasai-0.5.3/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.2/pandasai/middlewares/base.py` & `pandasai-0.5.3/pandasai/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.2/pandasai/middlewares/charts.py` & `pandasai-0.5.3/pandasai/middlewares/charts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.2/pandasai/middlewares/streamlit.py` & `pandasai-0.5.3/pandasai/middlewares/streamlit.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.2/pandasai/prompts/base.py` & `pandasai-0.5.3/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.2/pandasai/prompts/correct_error_prompt.py` & `pandasai-0.5.3/pandasai/prompts/correct_error_prompt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Prompt to correct Python Code on Error
 ```
 Today is {today_date}.
 You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
-This is the result of `print(df.head({rows_to_display}))`:
+This is the metadata of the dataframe:
 {df_head}.
 
 The user asked the following question:
 {question}
 
 You generated this python code:
 {code}
@@ -28,15 +28,15 @@
 
 class CorrectErrorPrompt(Prompt):
     """Prompt to Correct Python code on Error"""
 
     text: str = """
 Today is {today_date}.
 You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
-This is the result of `print(df.head({rows_to_display}))`:
+This is the metadata of the dataframe:
 {df_head}.
 
 The user asked the following question:
 {question}
 
 You generated this python code:
 {code}
```

### Comparing `pandasai-0.5.2/pandasai/prompts/correct_multiples_prompt.py` & `pandasai-0.5.3/pandasai/prompts/correct_multiples_prompt.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         question: str,
         df_head: list[pd.DataFrame],
     ):
         for i, dataframe in enumerate(df_head, start=1):
             row, col = dataframe.shape
             self.text += f"""
 Dataframe df{i}, with {row} rows and {col} columns.
-This is the result of `print(df{i}.head())`:
+This is the metadata of the dataframe df{i}:
 {dataframe}"""
 
         instruction: str = f"""
 The user asked the following question:
 {question}
 
 You generated this python code:
```

### Comparing `pandasai-0.5.2/pandasai/prompts/generate_python_code.py` & `pandasai-0.5.3/pandasai/prompts/generate_python_code.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Prompt to generate Python code
 ```
 Today is {today_date}.
 You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
-This is the result of `print(df.head({rows_to_display}))`:
+This is the metadata of the dataframe:
 {df_head}.
 
 When asked about the data, your response should include a python code that describes the
 dataframe `df`. Using the provided dataframe, df, return the python code and make sure to prefix
 the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG}
 exactly to get the answer to the following question:
 ```
@@ -21,15 +21,15 @@
 
 class GeneratePythonCodePrompt(Prompt):
     """Prompt to generate Python code"""
 
     text: str = """
 Today is {today_date}.
 You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
-This is the result of `print(df.head({rows_to_display}))`:
+This is the metadata of the dataframe:
 {df_head}.
 
 When asked about the data, your response should include a python code that describes the dataframe `df`.
 Using the provided dataframe, df, return the python code and make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly to get the answer to the following question:
 """  # noqa: E501
 
     def __init__(self, **kwargs):
```

### Comparing `pandasai-0.5.2/pandasai/prompts/multiple_dataframes.py` & `pandasai-0.5.3/pandasai/prompts/multiple_dataframes.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     def __init__(self, dataframes: list[pd.DataFrame]):
         for i, dataframe in enumerate(dataframes, start=1):
             row, col = dataframe.shape
 
             self.text += f"""
 Dataframe df{i}, with {row} rows and {col} columns.
-This is the result of `print(df{i}.head())`:
+This is the metadata of the dataframe df{i}:
 {dataframe}"""
 
         self.text += self.instruction
         self.text = self.text.format(
             today_date=date.today(),
             START_CODE_TAG=START_CODE_TAG,
             END_CODE_TAG=END_CODE_TAG,
```

### Comparing `pandasai-0.5.2/pyproject.toml` & `pandasai-0.5.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.5.2"
+version = "0.5.3"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
@@ -12,27 +12,29 @@
 python-dotenv = "^1.0.0"
 pandas = "1.5.3"
 astor = "^0.8.1"
 openai = "^0.27.5"
 ipython = "^8.13.1"
 matplotlib = "^3.7.1"
 google-generativeai = { version = "^0.1.0rc2", optional = true }
+langchain = { version = "^0.0.199", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pre-commit = "^3.2.2"
 ruff = "^0.0.220"
 pytest = "^7.3.1"
 pytest-mock = "^3.10.0"
 pytest-env = "^0.8.1"
 click = "^8.1.3"
 
 [tool.poetry.extras]
 google = ["google-generativeai"]
 tests = ["numpy", "seaborn"]
+langchain = ["langchain"]
 
 [tool.poetry.group.whitelist.dependencies]
 statsmodels = {version = "^0.14.0", optional = true}
 scikit-learn = {version = "^1.2.2", optional = true}
 seaborn = {version = "^0.12.2", optional = true}
 plotly = {version = "^5.14.1", optional = true}
 ggplot = {version = "^0.11.5", optional = true}
```

### Comparing `pandasai-0.5.2/PKG-INFO` & `pandasai-0.5.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,44 @@
-Metadata-Version: 2.1
-Name: pandasai
-Version: 0.5.2
-Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
-License: MIT
-Author: Gabriele Venturi
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: google
-Provides-Extra: tests
-Requires-Dist: astor (>=0.8.1,<0.9.0)
-Requires-Dist: google-generativeai (>=0.1.0rc2,<0.2.0) ; extra == "google"
-Requires-Dist: ipython (>=8.13.1,<9.0.0)
-Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: openai (>=0.27.5,<0.28.0)
-Requires-Dist: pandas (==1.5.3)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Description-Content-Type: text/markdown
-
 # PandasAI 🐼
 
 [![Release](https://img.shields.io/pypi/v/pandasai?label=Release&style=flat-square)](https://pypi.org/project/pandasai/)
 [![CI](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)
 [![CD](https://github.com/gventuri/pandas-ai/actions/workflows/cd.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/cd.yml/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/pandas-ai/badge/?version=latest)](https://pandas-ai.readthedocs.io/en/latest/?badge=latest)
 [![](https://dcbadge.vercel.app/api/server/kF7FqH2FwS?style=flat&compact=true)](https://discord.gg/kF7FqH2FwS)
-[![Downloads](https://static.pepy.tech/badge/pandasai/month)](https://pepy.tech/project/pandasai) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![Downloads](https://static.pepy.tech/badge/pandasai)](https://pepy.tech/project/pandasai) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/1rKz7TudOeCeKGHekw7JFNL4sagN9hon-?usp=sharing)
 
-Pandas AI is a Python library that adds generative artificial intelligence capabilities to Pandas, the popular data analysis and manipulation tool. It is designed to be used in conjunction with Pandas, and is not a replacement for it.
+PandasAI is a Python library that adds Generative AI capabilities to [pandas](https://github.com/pandas-dev/pandas), the popular data analysis and manipulation tool. It is designed to be used in conjunction with pandas, and is not a replacement for it.
 
 <!-- Add images/pandas-ai.png -->
 
 ![PandasAI](images/pandas-ai.png?raw=true)
 
-## Demo
+## 🔧 Quick install
+
+```bash
+pip install pandasai
+```
+
+## 🔍 Demo
 
 Try out PandasAI in your browser:
 
 [![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/1rKz7TudOeCeKGHekw7JFNL4sagN9hon-?usp=sharing)
 
-## Documentation
+## 📖 Documentation
 
 The documentation for PandasAI can be found [here](https://pandas-ai.readthedocs.io/en/latest/).
 
-## Installation
-
-```bash
-pip install pandasai
-```
-
-## Usage
+## 💻 Usage
 
 > Disclaimer: GDP data was collected from [this source](https://ourworldindata.org/grapher/gross-domestic-product?tab=table), published by World Development Indicators - World Bank (2022.05.26) and collected at National accounts data - World Bank / OECD. It relates to the year of 2020. Happiness indexes were extracted from [the World Happiness Report](https://ftnnews.com/images/stories/documents/2020/WHR20.pdf). Another useful [link](https://data.world/makeovermonday/2020w19-world-happiness-report-2020).
 
-PandasAI is designed to be used in conjunction with [pandas](https://github.com/pandas-dev/pandas). It makes Pandas conversational, allowing you to ask questions about your data and get answers back, in the form of pandas DataFrames.
+PandasAI is designed to be used in conjunction with pandas. It makes pandas conversational, allowing you to ask questions to your data in natural language.
 
 ### Queries
 
 For example, you can ask PandasAI to find all the rows in a DataFrame where the value of a column is greater than 5, and it will return a DataFrame containing only those rows:
 
 ```python
 import pandas as pd
@@ -152,116 +129,38 @@
 
 ```
 Oh, Olivia gets paid the most.
 ```
 
 You can find more examples in the [examples](examples) directory.
 
-## Command-Line Tool
-
-Pai is the command line tool designed to provide a convenient way to interact with PandasAI through a command line interface (CLI). In order to access the CLI tool, make sure to create a virtualenv for testing purpose and to install project dependencies in your local virtual environment using `pip` by running the following command:
-
-```
-pip install -e .
-```
-
-Alternatively, you can use `poetry` to create and activate the virtual environment by running the following command:
-
-```
-poetry shell
-```
-
-Inside the activated virtual environment, install the project dependencies by running the following command:
-
-```
-poetry install
-```
-
-By following these steps, you will now have the necessary environment to access the CLI tool.
-
-```
-pai [OPTIONS]
-```
-
-Options:
-
-- **-d, --dataset**: The file path to the dataset.
-- **-t, --token**: Your HuggingFace or OpenAI API token, if no token provided pai will pull from the `.env` file.
-- **-m, --model**: Choice of LLM, either `openai`, `open-assistant`, `starcoder`, `falcon`, `azure-openai` or `google-palm`.
-- **-p, --prompt**: Prompt that PandasAI will run.
-
-To view a full list of available options and their descriptions, run the following command:
-
-```
-pai --help
-
-```
-
-> For example,
->
-> ```
-> pai -d "~/pandasai/example/data/Loan payments data.csv" -m "openai" -p "How many loans are from men and have been paid off?"
-> ```
->
-> Should result in the same output as the `from_csv.py` example.
-
-## Privacy & Security
+## 🔒 Privacy & Security
 
 In order to generate the Python code to run, we take the dataframe head, we randomize it (using random generation for sensitive data and shuffling for non-sensitive data) and send just the head.
 
 Also, if you want to enforce further your privacy you can instantiate PandasAI with `enforce_privacy = True` which will not send the head (but just column names) to the LLM.
 
-## Environment Variables
-
-In order to set the API key for the LLM (Hugging Face Hub, OpenAI), you need to set the appropriate environment variables. You can do this by copying the `.env.example` file to `.env`:
-
-```bash
-cp .env.example .env
-```
-
-Then, edit the `.env` file and set the appropriate values.
-
-As an alternative, you can also pass the environment variables directly to the constructor of the LLM:
+## ⚙️ Command-Line Tool
 
-```python
-# OpenAI
-llm = OpenAI(api_token="YOUR_API_KEY")
-
-# Starcoder
-llm = Starcoder(api_token="YOUR_HF_API_KEY")
-
-# Falcon
-llm = Falcon(api_token="YOUR_HF_API_KEY")
-```
-
-Please note that at the moment OpenAI provides the best results, as the prompts are specifically designed for OpenAI and might hallucinate with other LLMs.
-
-## License
+Pai is the command line tool designed to provide a convenient way to interact with PandasAI through a command line interface (CLI). In order to access the CLI tool, make sure to create a virtualenv for testing purpose and to install project dependencies in your local virtual environment using `pip` by running the following command:
 
-PandasAI is licensed under the MIT License. See the LICENSE file for more details.
+Read more about how to use the CLI [here](https://pandas-ai.readthedocs.io/en/latest/pai_cli/).
 
-## Contributing
+## 🤝 Contributing
 
 Contributions are welcome! Please check out the todos below, and feel free to open a pull request.
 For more information, please see the [contributing guidelines](CONTRIBUTING.md).
 
 After installing the virtual environment, please remember to install `pre-commit` to be compliant with our standards:
 
 ```bash
 pre-commit install
 ```
 
+## 📜 License
+
+PandasAI is licensed under the MIT License. See the LICENSE file for more details.
+
 ## Acknowledgements
 
 - This project is based on the [pandas](https://github.com/pandas-dev/pandas) library by independent contributors, but it's in no way affiliated with the pandas project.
 - This project is meant to be used as a tool for data exploration and analysis, and it's not meant to be used for production purposes. Please use it responsibly.
-
-### Todo
-
-- [x] Add support for more LLMs
-- [x] Make PandasAI available from a CLI
-- [ ] Create a web interface for PandasAI
-- [x] Add unit tests
-- [x] Add contributing guidelines
-- [x] Add CI
-- [x] Add support for conversational responses
-
```

