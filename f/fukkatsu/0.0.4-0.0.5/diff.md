# Comparing `tmp/fukkatsu-0.0.4.tar.gz` & `tmp/fukkatsu-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fukkatsu-0.0.4.tar", last modified: Tue Jun 13 00:18:39 2023, max compression
+gzip compressed data, was "fukkatsu-0.0.5.tar", last modified: Wed Jun 14 23:47:14 2023, max compression
```

## Comparing `fukkatsu-0.0.4.tar` & `fukkatsu-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 00:18:39.891733 fukkatsu-0.0.4/
--rw-rw-rw-   0        0        0      914 2023-06-12 23:03:57.000000 fukkatsu-0.0.4/CHANGELOG.md
--rw-rw-rw-   0        0        0     1089 2023-04-28 00:39:24.000000 fukkatsu-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       58 2022-10-31 01:25:26.000000 fukkatsu-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0    12611 2023-06-13 00:18:39.884718 fukkatsu-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    11970 2023-06-12 23:37:54.000000 fukkatsu-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 00:18:39.807747 fukkatsu-0.0.4/fukkatsu/
--rw-rw-rw-   0        0        0     8008 2023-06-13 00:03:15.000000 fukkatsu-0.0.4/fukkatsu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 00:18:39.851079 fukkatsu-0.0.4/fukkatsu/memory/
--rw-rw-rw-   0        0        0       75 2023-05-20 04:07:03.000000 fukkatsu-0.0.4/fukkatsu/memory/__init__.py
--rw-rw-rw-   0        0        0      663 2023-05-20 04:07:01.000000 fukkatsu-0.0.4/fukkatsu/memory/manage.py
--rw-rw-rw-   0        0        0       23 2023-05-20 04:07:01.000000 fukkatsu-0.0.4/fukkatsu/memory/short.py
-drwxrwxrwx   0        0        0        0 2023-06-13 00:18:39.870986 fukkatsu-0.0.4/fukkatsu/utils/
--rw-rw-rw-   0        0        0      110 2023-05-18 05:17:09.000000 fukkatsu-0.0.4/fukkatsu/utils/__init__.py
--rw-rw-rw-   0        0        0     4082 2023-06-12 22:53:43.000000 fukkatsu-0.0.4/fukkatsu/utils/helper.py
--rw-rw-rw-   0        0        0     2241 2023-06-13 00:03:15.000000 fukkatsu-0.0.4/fukkatsu/utils/medic.py
--rw-rw-rw-   0        0        0     1531 2023-06-07 22:47:31.000000 fukkatsu-0.0.4/fukkatsu/utils/prompt.py
-drwxrwxrwx   0        0        0        0 2023-06-13 00:18:39.837747 fukkatsu-0.0.4/fukkatsu.egg-info/
--rw-rw-rw-   0        0        0    12611 2023-06-13 00:18:39.000000 fukkatsu-0.0.4/fukkatsu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-06-13 00:18:39.000000 fukkatsu-0.0.4/fukkatsu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 00:18:39.000000 fukkatsu-0.0.4/fukkatsu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-13 00:18:39.000000 fukkatsu-0.0.4/fukkatsu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-13 00:18:39.000000 fukkatsu-0.0.4/fukkatsu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 00:18:39.892730 fukkatsu-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1086 2023-06-12 22:59:04.000000 fukkatsu-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:47:14.528207 fukkatsu-0.0.5/
+-rw-rw-rw-   0        0        0     1085 2023-06-14 23:28:09.000000 fukkatsu-0.0.5/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1089 2023-04-28 00:39:24.000000 fukkatsu-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0       58 2022-10-31 01:25:26.000000 fukkatsu-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    12171 2023-06-14 23:47:14.528207 fukkatsu-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    11530 2023-06-13 23:47:46.000000 fukkatsu-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 23:47:14.455854 fukkatsu-0.0.5/fukkatsu/
+-rw-rw-rw-   0        0        0    10304 2023-06-14 23:46:10.000000 fukkatsu-0.0.5/fukkatsu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:47:14.497509 fukkatsu-0.0.5/fukkatsu/memory/
+-rw-rw-rw-   0        0        0       75 2023-05-20 04:07:03.000000 fukkatsu-0.0.5/fukkatsu/memory/__init__.py
+-rw-rw-rw-   0        0        0      663 2023-05-20 04:07:01.000000 fukkatsu-0.0.5/fukkatsu/memory/manage.py
+-rw-rw-rw-   0        0        0       23 2023-05-20 04:07:01.000000 fukkatsu-0.0.5/fukkatsu/memory/short.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:47:14.512552 fukkatsu-0.0.5/fukkatsu/utils/
+-rw-rw-rw-   0        0        0      110 2023-05-18 05:17:09.000000 fukkatsu-0.0.5/fukkatsu/utils/__init__.py
+-rw-rw-rw-   0        0        0     4082 2023-06-12 22:53:43.000000 fukkatsu-0.0.5/fukkatsu/utils/helper.py
+-rw-rw-rw-   0        0        0     3061 2023-06-14 23:46:10.000000 fukkatsu-0.0.5/fukkatsu/utils/medic.py
+-rw-rw-rw-   0        0        0     2779 2023-06-14 23:23:55.000000 fukkatsu-0.0.5/fukkatsu/utils/prompt.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:47:14.486758 fukkatsu-0.0.5/fukkatsu.egg-info/
+-rw-rw-rw-   0        0        0    12171 2023-06-14 23:47:13.000000 fukkatsu-0.0.5/fukkatsu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-06-14 23:47:14.000000 fukkatsu-0.0.5/fukkatsu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 23:47:13.000000 fukkatsu-0.0.5/fukkatsu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-14 23:47:13.000000 fukkatsu-0.0.5/fukkatsu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-14 23:47:13.000000 fukkatsu-0.0.5/fukkatsu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 23:47:14.528207 fukkatsu-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1086 2023-06-14 23:44:47.000000 fukkatsu-0.0.5/setup.py
```

### Comparing `fukkatsu-0.0.4/CHANGELOG.md` & `fukkatsu-0.0.5/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -18,8 +18,14 @@
 
 - added `allow_installs` argument to `mutate` and `resurrect` decorator. Allows LLM to install non installed python libraries
 
 ### 0.0.4
 
 - fixed a bug that caused input variables to be modified if a function performs in-place operations. I have added a deepcopy of the arguments
 - changed the name of `extract_text_between_backticks` to `extract_text_between_pipes`
-- added additional functions for response sanitation in LLM: `standardize_delimiters` and `add_delimiters`, which handle edge case answers from LLM
+- added additional functions for response sanitation in LLM: `standardize_delimiters` and `add_delimiters`, which handle edge case answers from LLM
+
+### 0.0.5
+
+- added control arguments for OpenAi model and temperature
+- added `twin` for review capabilities
+- improved prompt clarity on code indicator tags `|||`
```

### Comparing `fukkatsu-0.0.4/LICENSE` & `fukkatsu-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.4/PKG-INFO` & `fukkatsu-0.0.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fukkatsu
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python library for runtime LLM supported code corrections.
 Home-page: https://github.com/maxmekiska/fukkatsu
 Author: Maximilian Mekiska
 Author-email: maxmekiska@gmail.com
 Keywords: machinelearning,llm,runtime,codecorrection
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -254,57 +254,49 @@
 ### `mutate`
 ```python
 def mutate(request: str = "", allow_installs: bool = False):
   ...
 ```
 </details>
 
-## Testing Capabilities
 
-This section will conduct a series of simulations to better understand fukkatsu's potential capabilities. To achieve this, multiple error types will be tested. Each error type and scenario will consist of a total of 25 runs under the same conditions. We will test the following hypotheses:
+## fukkatsu 0.0.5 - `Not so Evil Twin`
 
-### Hypotheses testing
+<details>
+  <summary>Expand</summary>
+  <br>
 
-- H<sub>0</sub>: "The proportion of errors solved is not significantly greater than 0.5."
-- H<sub>1</sub>: "The proportion of errors solved is significantly greater than 0.5."
+The `mutate` and `resurrect` decorators now support new arguments `active_twin`, `llm`, and `temperature`. By default, `active_twin` is set to `False`, `llm` is set to `{"primary": "gpt-3.5-turbo", "secondary": "gpt-3.5-turbo"}`, and `temperature` is set to `{"primary": 0.1, "secondary": 0.1}`. This allows the user to configure the two decorators in a more granular way.
 
-We will consider a confidence interval of 0.05 and utilize a binomial distribution.
+If `active_twin` is set to `True`, another LLM, the `TWIN`, will crosscheck the answer of the first LLM and make corrections if deemed necessary. This is highly experimental but might become very powerful as soon as more diverse LLMs become available.
 
+### `resurrect`
 ```python
-import scipy.stats as stats
-
-successes = # number of successful repairs
-
-alpha = 0.05
-
-p_value = stats.binom_test(successes, n=25, p=0.5, alternative='greater')
-
-print(f"p_value: {p_value}")
-
-if p_value < alpha:
-    print("Reject the null hypothesis")
-    print("The proportion of errors solved is significantly greater than 0.5.")
-else:
-    print("Fail to reject the null hypothesis")
-    print("The proportion of errors solved is not significantly greater than 0.5.")
+def resurrect(
+    lives: int = 1,
+    additional_req: str = "",
+    allow_installs: bool = False,
+    active_twin: bool = False,
+    llm: dict = {"primary": "gpt-3.5-turbo", "secondary": "gpt-3.5-turbo"},
+    temperature: dict = {"primary": 0.1, "secondary": 0.1},
+):
+  ...
 ```
 
-
-fukkatsu will utilize the `gpt-3.5-turbo` model in all simulations. For each simulation, 3 lives will be allocated. The functions will also be provided with sufficient context. 
-
-After conducting all the tests, we will finally apply a `chi-square test`. This test will help determine whether there is a statistically significant difference in the fukkatsu's performance across the error types. If the test results indicate a significant association, it suggests that the effectiveness of fukkatsu varies depending on the error type.
-
+### `mutate`
 ```python
-import numpy as np
-from scipy.stats import chi2_contingency
-
-observed_counts = np.array([[10, 20], [15, 25], [5, 30]])
+def mutate(
+    request: str = "",
+    allow_installs: bool = False,
+    active_twin: bool = False,
+    llm: dict = {"primary": "gpt-3.5-turbo", "secondary": "gpt-3.5-turbo"},
+    temperature: dict = {"primary": 0.1, "secondary": 0.1},
+):
+  ...
+```
+</details>
 
-chi2, p_value, dof, expected = chi2_contingency(observed_counts)
+## Testing and measuring fukkatsu's Capabilities
 
-print("Chi-square statistic:", chi2)
-print("P-value:", p_value)
-print("Degrees of freedom:", dof)
-print("Expected counts:", expected)
-```
+The following section delves into a series of simulations aimed at gaining a deeper understanding of fukkatsu's potential capabilities.
 
-You can see each simulation recored in the different jupyter notebooks contained within the `research` directory.
+Please follow this [Link](https://github.com/maxmekiska/fukkatsu/blob/main/research/SIMULATIONS.md) for more information on fukkatsu's performance.
```

### Comparing `fukkatsu-0.0.4/README.md` & `fukkatsu-0.0.5/fukkatsu.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: fukkatsu
+Version: 0.0.5
+Summary: A python library for runtime LLM supported code corrections.
+Home-page: https://github.com/maxmekiska/fukkatsu
+Author: Maximilian Mekiska
+Author-email: maxmekiska@gmail.com
+Keywords: machinelearning,llm,runtime,codecorrection
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # fukkatsu 復活 [![Downloads](https://pepy.tech/badge/fukkatsu)](https://pepy.tech/project/fukkatsu) [![PyPi](https://img.shields.io/pypi/v/fukkatsu.svg?color=blue)](https://pypi.org/project/fukkatsu/) [![GitHub license](https://img.shields.io/github/license/maxmekiska/fukkatsu?color=black)](https://github.com/maxmekiska/fukkatsu/blob/main/LICENSE) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/fukkatsu.svg)](https://pypi.python.org/project/fukkatsu/)
 
 <br>
 
 | Build | Status|
 |---|---|
 | `MAIN BUILD`  |  ![master](https://github.com/maxmekiska/fukkatsu/actions/workflows/main.yml/badge.svg?branch=main) |
@@ -238,57 +254,49 @@
 ### `mutate`
 ```python
 def mutate(request: str = "", allow_installs: bool = False):
   ...
 ```
 </details>
 
-## Testing Capabilities
 
-This section will conduct a series of simulations to better understand fukkatsu's potential capabilities. To achieve this, multiple error types will be tested. Each error type and scenario will consist of a total of 25 runs under the same conditions. We will test the following hypotheses:
+## fukkatsu 0.0.5 - `Not so Evil Twin`
 
-### Hypotheses testing
+<details>
+  <summary>Expand</summary>
+  <br>
 
-- H<sub>0</sub>: "The proportion of errors solved is not significantly greater than 0.5."
-- H<sub>1</sub>: "The proportion of errors solved is significantly greater than 0.5."
+The `mutate` and `resurrect` decorators now support new arguments `active_twin`, `llm`, and `temperature`. By default, `active_twin` is set to `False`, `llm` is set to `{"primary": "gpt-3.5-turbo", "secondary": "gpt-3.5-turbo"}`, and `temperature` is set to `{"primary": 0.1, "secondary": 0.1}`. This allows the user to configure the two decorators in a more granular way.
 
-We will consider a confidence interval of 0.05 and utilize a binomial distribution.
+If `active_twin` is set to `True`, another LLM, the `TWIN`, will crosscheck the answer of the first LLM and make corrections if deemed necessary. This is highly experimental but might become very powerful as soon as more diverse LLMs become available.
 
+### `resurrect`
 ```python
-import scipy.stats as stats
-
-successes = # number of successful repairs
-
-alpha = 0.05
-
-p_value = stats.binom_test(successes, n=25, p=0.5, alternative='greater')
-
-print(f"p_value: {p_value}")
-
-if p_value < alpha:
-    print("Reject the null hypothesis")
-    print("The proportion of errors solved is significantly greater than 0.5.")
-else:
-    print("Fail to reject the null hypothesis")
-    print("The proportion of errors solved is not significantly greater than 0.5.")
+def resurrect(
+    lives: int = 1,
+    additional_req: str = "",
+    allow_installs: bool = False,
+    active_twin: bool = False,
+    llm: dict = {"primary": "gpt-3.5-turbo", "secondary": "gpt-3.5-turbo"},
+    temperature: dict = {"primary": 0.1, "secondary": 0.1},
+):
+  ...
 ```
 
-
-fukkatsu will utilize the `gpt-3.5-turbo` model in all simulations. For each simulation, 3 lives will be allocated. The functions will also be provided with sufficient context. 
-
-After conducting all the tests, we will finally apply a `chi-square test`. This test will help determine whether there is a statistically significant difference in the fukkatsu's performance across the error types. If the test results indicate a significant association, it suggests that the effectiveness of fukkatsu varies depending on the error type.
-
+### `mutate`
 ```python
-import numpy as np
-from scipy.stats import chi2_contingency
-
-observed_counts = np.array([[10, 20], [15, 25], [5, 30]])
+def mutate(
+    request: str = "",
+    allow_installs: bool = False,
+    active_twin: bool = False,
+    llm: dict = {"primary": "gpt-3.5-turbo", "secondary": "gpt-3.5-turbo"},
+    temperature: dict = {"primary": 0.1, "secondary": 0.1},
+):
+  ...
+```
+</details>
 
-chi2, p_value, dof, expected = chi2_contingency(observed_counts)
+## Testing and measuring fukkatsu's Capabilities
 
-print("Chi-square statistic:", chi2)
-print("P-value:", p_value)
-print("Degrees of freedom:", dof)
-print("Expected counts:", expected)
-```
+The following section delves into a series of simulations aimed at gaining a deeper understanding of fukkatsu's potential capabilities.
 
-You can see each simulation recored in the different jupyter notebooks contained within the `research` directory.
+Please follow this [Link](https://github.com/maxmekiska/fukkatsu/blob/main/research/SIMULATIONS.md) for more information on fukkatsu's performance.
```

### Comparing `fukkatsu-0.0.4/fukkatsu/__init__.py` & `fukkatsu-0.0.5/fukkatsu/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,31 @@
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 import copy
 import functools
 import logging
 import traceback
 
 from fukkatsu.memory import SHORT_TERM_MEMORY
 from fukkatsu.utils import (check_and_install_libraries, extract_imports,
                             extract_text_between_pipes,
                             insert_string_after_colon, remove_trace_lines,
                             remove_wrapper_name, return_input_arguments,
                             return_source_code)
-from fukkatsu.utils.medic import defibrillate, enhance
+from fukkatsu.utils.medic import defibrillate, enhance, twin
 
 
-def resurrect(lives: int = 1, additional_req: str = "", allow_installs: bool = False):
+def resurrect(
+    lives: int = 1,
+    additional_req: str = "",
+    allow_installs: bool = False,
+    active_twin: bool = False,
+    llm: dict = {"primary": "gpt-3.5-turbo", "secondary": "gpt-3.5-turbo"},
+    temperature: dict = {"primary": 0.1, "secondary": 0.1},
+):
     def _resurrect(func):
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             input_args = return_input_arguments(func, *args, **kwargs)
 
             try:
                 args_copy = copy.deepcopy(args)
@@ -47,22 +54,33 @@
 
                 else:
                     logging.warning("Requesting INITIAL correction\n")
                     suggested_code = defibrillate(
                         inputs=input_args,
                         faulty_function=source,
                         error_trace=trace,
+                        model=llm["primary"],
+                        temperature=temperature["primary"],
                         additional_req=additional_req,
                     )
                     logging.warning(
-                        f"Received INITIAL RAW suggestion: {suggested_code}\n"
+                        f"Received INITIAL RAW suggestion:\n{suggested_code}\n"
                     )
+                    if active_twin == True:
+                        logging.warning("Requesting TWIN review\n")
+                        suggested_code = twin(
+                            inputs=input_args,
+                            target_function=suggested_code,
+                            model=llm["secondary"],
+                            temperature=temperature["secondary"],
+                        )
+                        logging.warning(f"TWIN review complete:\n{suggested_code}")
                     suggested_code = extract_text_between_pipes(suggested_code)
                     logging.warning(
-                        f"Received INITIAL CLEANED suggestion: {suggested_code}\n"
+                        f"Received INITIAL CLEANED suggestion:\n{suggested_code}\n"
                     )
 
                     import_block = extract_imports(suggested_code)
                     if allow_installs == True:
                         check_and_install_libraries(import_statements=import_block)
 
                     suggested_code = insert_string_after_colon(
@@ -82,15 +100,15 @@
                         compiled_code = compile(suggested_code, "<string>", "exec")
 
                         exec(compiled_code, global_dict, local_dict)
                         new_function = local_dict[func.__name__]
 
                         SHORT_TERM_MEMORY[trace] = suggested_code
                         logging.warning(
-                            f"Reanimation successful, using {suggested_code}\n"
+                            f"Reanimation successful, using:\n{suggested_code}\n"
                         )
                         locals()[func.__name__] = new_function
 
                         args_copy = copy.deepcopy(args)
                         kwargs_copy = copy.deepcopy(kwargs)
 
                         return new_function(*args_copy, **kwargs_copy)
@@ -111,22 +129,36 @@
                             )
 
                         else:
                             suggested_code = defibrillate(
                                 inputs=input_args,
                                 faulty_function=suggested_code,
                                 error_trace=trace,
+                                model=llm["primary"],
+                                temperature=temperature["primary"],
                                 additional_req=additional_req,
                             )
                             logging.warning(
-                                f"Received attempt RAW suggestion: {suggested_code}\n"
+                                f"Received attempt RAW suggestion:\n{suggested_code}\n"
                             )
+
+                            if active_twin == True:
+                                logging.warning("Requesting TWIN review\n")
+                                suggested_code = twin(
+                                    inputs=input_args,
+                                    target_function=suggested_code,
+                                    model=llm["secondary"],
+                                    temperature=temperature["secondary"],
+                                )
+                                logging.warning(
+                                    f"TWIN review complete:\n{suggested_code}"
+                                )
                             suggested_code = extract_text_between_pipes(suggested_code)
                             logging.warning(
-                                f"Received attempt CLEANED suggestion: {suggested_code}\n"
+                                f"Received attempt CLEANED suggestion:\n{suggested_code}\n"
                             )
 
                             import_block = extract_imports(suggested_code)
                             if allow_installs == True:
                                 check_and_install_libraries(
                                     import_statements=import_block
                                 )
@@ -141,15 +173,21 @@
                 raise Exception(f"|__|__|______ {func.__name__} flatlined")
 
         return wrapper
 
     return _resurrect
 
 
-def mutate(request: str = "", allow_installs: bool = False):
+def mutate(
+    request: str = "",
+    allow_installs: bool = False,
+    active_twin: bool = False,
+    llm: dict = {"primary": "gpt-3.5-turbo", "secondary": "gpt-3.5-turbo"},
+    temperature: dict = {"primary": 0.1, "secondary": 0.1},
+):
     def _mutate(func):
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
 
             input_args = return_input_arguments(func, *args, **kwargs)
             source = return_source_code(func)
             source = remove_wrapper_name(source)
@@ -157,17 +195,29 @@
             logging.warning(f"Input arguments: {input_args}\n")
             logging.warning(f"\nSource Code: \n {source}\n")
 
             logging.warning("Requesting mutation\n")
             suggested_code = enhance(
                 inputs=input_args,
                 target_function=source,
+                model=llm["primary"],
+                temperature=temperature["primary"],
                 request=request,
             )
-            logging.warning(f"Received RAW suggestion mutation: {suggested_code}\n")
+            logging.warning(f"Received RAW suggestion mutation:\n{suggested_code}\n")
+
+            if active_twin == True:
+                logging.warning("Requesting TWIN review:\n")
+                suggested_code = twin(
+                    inputs=input_args,
+                    target_function=suggested_code,
+                    model=llm["secondary"],
+                    temperature=temperature["secondary"],
+                )
+                logging.warning(f"TWIN review complete:\n{suggested_code}")
             suggested_code = extract_text_between_pipes(suggested_code)
             logging.warning(f"Received CLEANED suggestion mutation: {suggested_code}\n")
 
             global_dict = globals()
             local_dict = locals()
 
             import_block = extract_imports(suggested_code)
```

### Comparing `fukkatsu-0.0.4/fukkatsu/memory/manage.py` & `fukkatsu-0.0.5/fukkatsu/memory/manage.py`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.4/fukkatsu/utils/helper.py` & `fukkatsu-0.0.5/fukkatsu/utils/helper.py`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.4/fukkatsu/utils/medic.py` & `fukkatsu-0.0.5/fukkatsu/utils/medic.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,102 @@
 import os
 
 import openai
 
 from fukkatsu.utils.prompt import (ADDITIONAL, CONTEXT, CONTEXT_MUTATE,
-                                   OUTPUT_CONSTRAINTS,
-                                   OUTPUT_CONSTRAINTS_MUTATE)
+                                   CONTEXT_TWIN, OUTPUT_CONSTRAINTS,
+                                   OUTPUT_CONSTRAINTS_MUTATE,
+                                   OUTPUT_CONSTRAINTS_TWIN)
 
 try:
     openai.api_key = os.environ.get("OPENAI_API_KEY")
     print("OPENAI_API_KEY found in environment variables.")
 except:
     print("OPENAI_API_KEY not found in environment variables.")
     raise Exception("OPENAI_API_KEY not found in environment variables.")
 
-MODEL = "gpt-3.5-turbo"
-
 
 def defibrillate(
-    inputs: str, faulty_function: str, error_trace: str, additional_req: str = ""
+    inputs: str,
+    faulty_function: str,
+    error_trace: str,
+    model: str,
+    temperature: float,
+    additional_req: str = "",
 ) -> str:
     if additional_req == "":
         set_prompt = (
             f"{CONTEXT}\n\n{faulty_function}\n\nThe function received the following inputs:\n\n"
             f"{inputs}\n\nAnd returned the following error trace:\n\n{error_trace}\n\n{OUTPUT_CONSTRAINTS}"
         )
     else:
         set_prompt = (
             f"{CONTEXT}\n\n{faulty_function}\n\nThe function received the following inputs:\n\n"
             f"{inputs}\n\nAnd returned the following error trace:\n\n{error_trace}\n\n{OUTPUT_CONSTRAINTS}\n"
             f"{ADDITIONAL}{additional_req}"
         )
 
     response = openai.ChatCompletion.create(
-        model=MODEL,
+        model=model,
         messages=[
             {"role": "system", "content": set_prompt},
         ],
         max_tokens=1024,
         n=1,
         stop=None,
-        temperature=0.1,
+        temperature=temperature,
     )
 
     corrected_function = response["choices"][0]["message"]["content"].strip()
 
     return corrected_function
 
 
-def enhance(inputs: str, target_function: str, request: str = "") -> str:
+def enhance(
+    inputs: str, target_function: str, model: str, temperature: float, request: str = ""
+) -> str:
     set_prompt = (
         f"{CONTEXT_MUTATE}\n\n{target_function}\n\nThe function received the following inputs:\n\n"
         f"{inputs}\n\nThe user requests the following:\n{request}\n{OUTPUT_CONSTRAINTS_MUTATE}"
     )
 
     response = openai.ChatCompletion.create(
-        model=MODEL,
+        model=model,
+        messages=[
+            {"role": "system", "content": set_prompt},
+        ],
+        max_tokens=1024,
+        n=1,
+        stop=None,
+        temperature=temperature,
+    )
+
+    mutated_function = response["choices"][0]["message"]["content"].strip()
+
+    return mutated_function
+
+
+def twin(
+    inputs: str,
+    target_function: str,
+    model: str,
+    temperature: float,
+) -> str:
+    set_prompt = (
+        f"{CONTEXT_TWIN}\n\n{target_function}\n\nThe function received the following inputs:\n\n"
+        f"{inputs}\n\n{OUTPUT_CONSTRAINTS_TWIN}"
+    )
+
+    response = openai.ChatCompletion.create(
+        model=model,
         messages=[
             {"role": "system", "content": set_prompt},
         ],
         max_tokens=1024,
         n=1,
         stop=None,
-        temperature=0.1,
+        temperature=temperature,
     )
 
     mutated_function = response["choices"][0]["message"]["content"].strip()
 
     return mutated_function
```

### Comparing `fukkatsu-0.0.4/fukkatsu.egg-info/PKG-INFO` & `fukkatsu-0.0.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: fukkatsu
-Version: 0.0.4
-Summary: A python library for runtime LLM supported code corrections.
-Home-page: https://github.com/maxmekiska/fukkatsu
-Author: Maximilian Mekiska
-Author-email: maxmekiska@gmail.com
-Keywords: machinelearning,llm,runtime,codecorrection
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # fukkatsu 復活 [![Downloads](https://pepy.tech/badge/fukkatsu)](https://pepy.tech/project/fukkatsu) [![PyPi](https://img.shields.io/pypi/v/fukkatsu.svg?color=blue)](https://pypi.org/project/fukkatsu/) [![GitHub license](https://img.shields.io/github/license/maxmekiska/fukkatsu?color=black)](https://github.com/maxmekiska/fukkatsu/blob/main/LICENSE) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/fukkatsu.svg)](https://pypi.python.org/project/fukkatsu/)
 
 <br>
 
 | Build | Status|
 |---|---|
 | `MAIN BUILD`  |  ![master](https://github.com/maxmekiska/fukkatsu/actions/workflows/main.yml/badge.svg?branch=main) |
@@ -254,57 +238,49 @@
 ### `mutate`
 ```python
 def mutate(request: str = "", allow_installs: bool = False):
   ...
 ```
 </details>
 
-## Testing Capabilities
 
-This section will conduct a series of simulations to better understand fukkatsu's potential capabilities. To achieve this, multiple error types will be tested. Each error type and scenario will consist of a total of 25 runs under the same conditions. We will test the following hypotheses:
+## fukkatsu 0.0.5 - `Not so Evil Twin`
 
-### Hypotheses testing
+<details>
+  <summary>Expand</summary>
+  <br>
 
-- H<sub>0</sub>: "The proportion of errors solved is not significantly greater than 0.5."
-- H<sub>1</sub>: "The proportion of errors solved is significantly greater than 0.5."
+The `mutate` and `resurrect` decorators now support new arguments `active_twin`, `llm`, and `temperature`. By default, `active_twin` is set to `False`, `llm` is set to `{"primary": "gpt-3.5-turbo", "secondary": "gpt-3.5-turbo"}`, and `temperature` is set to `{"primary": 0.1, "secondary": 0.1}`. This allows the user to configure the two decorators in a more granular way.
 
-We will consider a confidence interval of 0.05 and utilize a binomial distribution.
+If `active_twin` is set to `True`, another LLM, the `TWIN`, will crosscheck the answer of the first LLM and make corrections if deemed necessary. This is highly experimental but might become very powerful as soon as more diverse LLMs become available.
 
+### `resurrect`
 ```python
-import scipy.stats as stats
-
-successes = # number of successful repairs
-
-alpha = 0.05
-
-p_value = stats.binom_test(successes, n=25, p=0.5, alternative='greater')
-
-print(f"p_value: {p_value}")
-
-if p_value < alpha:
-    print("Reject the null hypothesis")
-    print("The proportion of errors solved is significantly greater than 0.5.")
-else:
-    print("Fail to reject the null hypothesis")
-    print("The proportion of errors solved is not significantly greater than 0.5.")
+def resurrect(
+    lives: int = 1,
+    additional_req: str = "",
+    allow_installs: bool = False,
+    active_twin: bool = False,
+    llm: dict = {"primary": "gpt-3.5-turbo", "secondary": "gpt-3.5-turbo"},
+    temperature: dict = {"primary": 0.1, "secondary": 0.1},
+):
+  ...
 ```
 
-
-fukkatsu will utilize the `gpt-3.5-turbo` model in all simulations. For each simulation, 3 lives will be allocated. The functions will also be provided with sufficient context. 
-
-After conducting all the tests, we will finally apply a `chi-square test`. This test will help determine whether there is a statistically significant difference in the fukkatsu's performance across the error types. If the test results indicate a significant association, it suggests that the effectiveness of fukkatsu varies depending on the error type.
-
+### `mutate`
 ```python
-import numpy as np
-from scipy.stats import chi2_contingency
-
-observed_counts = np.array([[10, 20], [15, 25], [5, 30]])
+def mutate(
+    request: str = "",
+    allow_installs: bool = False,
+    active_twin: bool = False,
+    llm: dict = {"primary": "gpt-3.5-turbo", "secondary": "gpt-3.5-turbo"},
+    temperature: dict = {"primary": 0.1, "secondary": 0.1},
+):
+  ...
+```
+</details>
 
-chi2, p_value, dof, expected = chi2_contingency(observed_counts)
+## Testing and measuring fukkatsu's Capabilities
 
-print("Chi-square statistic:", chi2)
-print("P-value:", p_value)
-print("Degrees of freedom:", dof)
-print("Expected counts:", expected)
-```
+The following section delves into a series of simulations aimed at gaining a deeper understanding of fukkatsu's potential capabilities.
 
-You can see each simulation recored in the different jupyter notebooks contained within the `research` directory.
+Please follow this [Link](https://github.com/maxmekiska/fukkatsu/blob/main/research/SIMULATIONS.md) for more information on fukkatsu's performance.
```

### Comparing `fukkatsu-0.0.4/setup.py` & `fukkatsu-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     author="Maximilian Mekiska",
     author_email="maxmekiska@gmail.com",
     url="https://github.com/maxmekiska/fukkatsu",
     description="A python library for runtime LLM supported code corrections.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     name="fukkatsu",
-    version="0.0.4",
+    version="0.0.5",
     packages=find_packages(include=["fukkatsu", "fukkatsu.*"]),
     install_requires=[
         "setuptools >= 41.0.0",
         "openai >= 0.27.5, <= 0.28",
     ],
     classifiers=[
         "Programming Language :: Python :: 3.8",
```

