# Comparing `tmp/visuallm-0.1.6.tar.gz` & `tmp/visuallm-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visuallm-0.1.6.tar", last modified: Thu Jun 15 16:34:04 2023, max compression
+gzip compressed data, was "visuallm-0.1.7.tar", last modified: Thu Jun 15 16:35:28 2023, max compression
```

## Comparing `visuallm-0.1.6.tar` & `visuallm-0.1.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:34:04.989772 visuallm-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-15 16:33:49.000000 visuallm-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 16:33:49.000000 visuallm-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20399 2023-06-15 16:34:04.989772 visuallm-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19805 2023-06-15 16:33:49.000000 visuallm-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-15 16:33:49.000000 visuallm-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 16:34:04.989772 visuallm-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:34:04.985772 visuallm-0.1.6/visuallm/
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-15 16:33:49.000000 visuallm-0.1.6/visuallm/component_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:34:04.989772 visuallm-0.1.6/visuallm/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-15 16:33:49.000000 visuallm-0.1.6/visuallm/components/DatasetVisualizationComponent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-06-15 16:33:49.000000 visuallm-0.1.6/visuallm/components/GenerationComponent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-15 16:33:49.000000 visuallm-0.1.6/visuallm/components/NextTokenPredictionComponent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:34:04.989772 visuallm-0.1.6/visuallm/components/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-06-15 16:33:49.000000 visuallm-0.1.6/visuallm/components/mixins/data_preparation_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-15 16:33:49.000000 visuallm-0.1.6/visuallm/components/mixins/generation_selectors_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-06-15 16:33:49.000000 visuallm-0.1.6/visuallm/components/mixins/metrics_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-15 16:33:49.000000 visuallm-0.1.6/visuallm/components/mixins/model_selection_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:34:04.989772 visuallm-0.1.6/visuallm/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:34:04.989772 visuallm-0.1.6/visuallm/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   201746 2023-06-15 16:33:49.000000 visuallm-0.1.6/visuallm/dist/assets/index-9006265c.js
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-06-15 16:33:49.000000 visuallm-0.1.6/visuallm/dist/assets/index-d8f16c2e.css
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-15 16:33:49.000000 visuallm-0.1.6/visuallm/dist/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-15 16:33:49.000000 visuallm-0.1.6/visuallm/dist/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:34:04.989772 visuallm-0.1.6/visuallm/elements/
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-06-15 16:33:49.000000 visuallm-0.1.6/visuallm/elements/barchart_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-15 16:33:49.000000 visuallm-0.1.6/visuallm/elements/element_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-15 16:33:49.000000 visuallm-0.1.6/visuallm/elements/plain_text_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-06-15 16:33:49.000000 visuallm-0.1.6/visuallm/elements/selector_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-06-15 16:33:49.000000 visuallm-0.1.6/visuallm/elements/table_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-15 16:33:49.000000 visuallm-0.1.6/visuallm/elements/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-15 16:33:49.000000 visuallm-0.1.6/visuallm/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:34:04.989772 visuallm-0.1.6/visuallm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20399 2023-06-15 16:34:04.000000 visuallm-0.1.6/visuallm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-15 16:34:04.000000 visuallm-0.1.6/visuallm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:34:04.000000 visuallm-0.1.6/visuallm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 16:34:04.000000 visuallm-0.1.6/visuallm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 16:34:04.000000 visuallm-0.1.6/visuallm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:35:28.180137 visuallm-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-15 16:35:16.000000 visuallm-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 16:35:16.000000 visuallm-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20371 2023-06-15 16:35:28.180137 visuallm-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-06-15 16:35:16.000000 visuallm-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-15 16:35:16.000000 visuallm-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 16:35:28.180137 visuallm-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:35:28.176137 visuallm-0.1.7/visuallm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/component_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:35:28.176137 visuallm-0.1.7/visuallm/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/components/DatasetVisualizationComponent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/components/GenerationComponent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/components/NextTokenPredictionComponent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:35:28.176137 visuallm-0.1.7/visuallm/components/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/components/mixins/data_preparation_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/components/mixins/generation_selectors_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/components/mixins/metrics_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/components/mixins/model_selection_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:35:28.176137 visuallm-0.1.7/visuallm/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:35:28.176137 visuallm-0.1.7/visuallm/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   201746 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/dist/assets/index-9006265c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/dist/assets/index-d8f16c2e.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/dist/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/dist/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:35:28.180137 visuallm-0.1.7/visuallm/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/elements/barchart_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/elements/element_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/elements/plain_text_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/elements/selector_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/elements/table_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/elements/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:35:28.176137 visuallm-0.1.7/visuallm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20371 2023-06-15 16:35:28.000000 visuallm-0.1.7/visuallm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-15 16:35:28.000000 visuallm-0.1.7/visuallm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:35:28.000000 visuallm-0.1.7/visuallm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 16:35:28.000000 visuallm-0.1.7/visuallm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 16:35:28.000000 visuallm-0.1.7/visuallm.egg-info/top_level.txt
```

### Comparing `visuallm-0.1.6/LICENSE` & `visuallm-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.6/PKG-INFO` & `visuallm-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: visuallm
-Version: 0.1.6
+Version: 0.1.7
 Summary: Visualization tool for various generation tasks on Language Models. 
 Author-email: "Frantisek Trebuna (gortibaldik)" <ferotre@gmail.com>
 Project-URL: Homepage, https://github.com/gortibaldik/visuallm
 Project-URL: Bug Tracker, https://github.com/gortibaldik/visuallm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: huggingface
 License-File: LICENSE
 
 # Conditional Language Model Generation Visualization
 
-## VERSION: `0.1.6`
+## VERSION: `0.1.7`
 
 - when evaluating language models it is often pain to see what is generated and why
 - this little package is a `vue.js` frontend together with `flask` backend and it is designed to easily show some interesting visualizations on conditional generation models
 - it handles frontend-backend communication as well as frontend rendering
 - hence the developper can focus only on ML aspects of his work!
 
 ## Installation
@@ -39,15 +39,14 @@
 
 1. Create a class inheriting from `llm_generation_server.component_base.ComponentBase`. In `__init__` you should:
 
 - create all the elements from which the page should be composed
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/simple_component.py&lines=1-15&header=# ./examples_py/simple_component.py lines 1-15)-->
 <!-- The below code snippet is automatically added from ./examples_py/simple_component.py -->
-
 ```py
 # ./examples_py/simple_component.py lines 1-15
 from visuallm.component_base import ComponentBase
 from visuallm.elements.plain_text_element import PlainTextElement
 
 
 class SimpleComponent(ComponentBase):
@@ -58,48 +57,43 @@
         self.text_element = PlainTextElement(
             content="""
                 Some really interesting text that isn't formatted in any way, it is
                 just a plain simple text
             """
         )
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 - call `super().__init__`, where you specify name and title of the component as well as the created elements in the order that they should appear in the page
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/simple_component.py&lines=16-21&header=# ./examples_py/simple_component.py lines 16-21)-->
 <!-- The below code snippet is automatically added from ./examples_py/simple_component.py -->
-
 ```py
 # ./examples_py/simple_component.py lines 16-21
         super().__init__(
             name="simple_component",
             title="Simple Component",
             elements=[self.main_heading_element, self.text_element],
         )
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 2. Initialize `llm_generation_server.server.Server` and pass in the initialized components
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/simple_app.py&lines=1-7&header=# ./examples_py/simple_app.py)-->
 <!-- The below code snippet is automatically added from ./examples_py/simple_app.py -->
-
 ```py
 # ./examples_py/simple_app.py
 from visuallm.server import Server
 
 from .simple_component import SimpleComponent
 
 server = Server(__name__, [SimpleComponent()])
 app = server.app
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 3. Standard method to run the flask application, e.g. for the example provided above, it would be
 
 ```sh
 python3 -m flask --app examples_py.simple_app run
 ```
@@ -110,15 +104,14 @@
 
 I wrote this library to help me visualize the output distributions of various models I implemented during my master's thesis. Therefore I implemented only few basic elements for ML purposes.
 
 In the following paragraphs I'll explain how to create configuration selectors, tables and bar-charts, and I'll use the following server: (You'll see the implementation of each of yet unknown components)
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/app.py&header=# ./examples_py/app.py)-->
 <!-- The below code snippet is automatically added from ./examples_py/app.py -->
-
 ```py
 # ./examples_py/app.py
 from visuallm.server import Server
 
 from .bar_chart_component_advanced import BarChartComponentAdvanced
 from .bar_chart_component_simple import BarChartComponentSimple
 from .selector_component import SelectorComponent
@@ -134,102 +127,92 @@
         TableComponent(),
         TwoTablesComponent(),
         SelectorComponent(),
     ],
 )
 app = flask_app.app
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 You can see the generated page by running the following script after cloning the github repository and navigating into it:
 
 ```sh
 flask --app examples_py.app run
 ```
 
 #### Configuration Selection
 
 Several different kinds of configuration specifier, together with one button element. The button element allows backend communication and by itself it does nothing. However you can specify subelements, for which the button element will provide communication updates. For the example below, the following imports will be used:
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/selector_component.py&lines=1-10&header=# ./examples_py/selector_component.py lines 1-10)-->
 <!-- The below code snippet is automatically added from ./examples_py/selector_component.py -->
-
 ```py
 # ./examples_py/selector_component.py lines 1-10
 import time
 
 from visuallm.component_base import ComponentBase
 from visuallm.elements.plain_text_element import PlainTextElement
 from visuallm.elements.selector_elements import (
     ButtonElement,
     CheckBoxSubElement,
     ChoicesSubElement,
     MinMaxSubElement,
 )
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ##### MinMax SubElement
 
 Input element for setting integer in a range.
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/selector_component.py&lines=13-18&header=# ./examples_py/selector_component.py lines 13-18)-->
 <!-- The below code snippet is automatically added from ./examples_py/selector_component.py -->
-
 ```py
 # ./examples_py/selector_component.py lines 13-18
 class SelectorComponent(ComponentBase):
     def __init__(self):
         self.text_element = PlainTextElement(content="Nothing was selected")
         self.number_selector_element = MinMaxSubElement(
             sample_min=0, sample_max=10, text="Select Number:"
         )
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ##### Choices SubElement
 
 Input element for choosing between several choices.
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/selector_component.py&lines=19-21&header=# ./examples_py/selector_component.py lines 19-21)-->
 <!-- The below code snippet is automatically added from ./examples_py/selector_component.py -->
-
 ```py
 # ./examples_py/selector_component.py lines 19-21
         self.choices_element = ChoicesSubElement(
             choices=["super", "magnificent", "incredible"], text="This library is:"
         )
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ##### Checkbox SubElement
 
 Simple checkbox input element.
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/selector_component.py&lines=22-22&header=# ./examples_py/selector_component.py lines 22)-->
 <!-- The below code snippet is automatically added from ./examples_py/selector_component.py -->
-
 ```py
 # ./examples_py/selector_component.py lines 22
         self.checkbox_element = CheckBoxSubElement(text="Have you slept?:")
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ##### Button Element
 
 This is an element that should encapsulate all the other configuration selection elements. It needs a callback method that will be called when the button is pressed and we provide `ButtonElement.default_select_callback()` which handles processing all the changes sent from the frontend and attributing them to `subelement.selected` properties of subelements.
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/selector_component.py&lines=23-61&header=# ./examples_py/selector_component.py lines 23-61)-->
 <!-- The below code snippet is automatically added from ./examples_py/selector_component.py -->
-
 ```py
 # ./examples_py/selector_component.py lines 23-61
         self.button_element = ButtonElement(
             processing_callback=self.button_clicked,
             subelements=[
                 self.number_selector_element,
                 self.choices_element,
@@ -264,27 +247,25 @@
         self.text_element.content = (
             f"This library is {c} and I would give "
             + f"it {n} stars out of {n} if I could. ({b})"
             + f" This {'has' if any_updated else 'has not'} changed!"
         )
         time.sleep(n)
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ![selector_image](./readme_images/selector.png)
 
 #### Table Element
 
 This element can show several tables on the frontend together with a special feature, links between rows of the tables. They may connect different rows of different tables and display some value above links.
 The below example displays, how to generate one table on the frontend with the links pointing from each row to all the upwards rows as displayed on the image.
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/table_component.py&header=# ./examples_py/table_component.py)-->
 <!-- The below code snippet is automatically added from ./examples_py/table_component.py -->
-
 ```py
 # ./examples_py/table_component.py
 from visuallm.component_base import ComponentBase
 from visuallm.elements.plain_text_element import PlainTextElement
 from visuallm.elements.table_element import LinkBetweenRows, TableElement
 
 
@@ -327,46 +308,42 @@
         # add links pointing to all the rows upwards
         for j in range(len(rows) - 1, 0, -1):
             for i in range(j):
                 self.table_element.add_link_between_rows(
                     LinkBetweenRows(TABLE_NAME, j, TABLE_NAME, i, Label="some value")
                 )
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ![table_page](./readme_images/table.png)
 
 #### Table Element (Advanced)
 
 Let's look at an advanced example of table element, where we create two tables and add links which connect multiple tables. I will only show the important snippets of code.
 
 Firstly, we will import `Colors` enumeration to color links to different tables with different colors.
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/two_tables_component.py&header=# ./examples_py/two_tables_component.py lines 1-7&lines=1-7)-->
 <!-- The below code snippet is automatically added from ./examples_py/two_tables_component.py -->
-
 ```py
 # ./examples_py/two_tables_component.py lines 1-7
 from visuallm.component_base import ComponentBase
 from visuallm.elements.plain_text_element import PlainTextElement
 from visuallm.elements.table_element import Colors, LinkBetweenRows, TableElement
 
 
 class TwoTablesComponent(ComponentBase):
     def __init__(self):
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 Secondly, we will create the links in such a way, that links going within the same table will be colored orange (the default color), while the links going to the other table will be colored light blue. Also links within one table will be thin, while links to the other table will be thick (`Importance` parameter).
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/two_tables_component.py&header=# ./examples_py/two_tables_component.py lines 69-99&lines=69-99)-->
 <!-- The below code snippet is automatically added from ./examples_py/two_tables_component.py -->
-
 ```py
 # ./examples_py/two_tables_component.py lines 69-99
             # links going from the row j of the second table to all the upper
             # rows in the second table
             for i in range(j):
                 self.table_element.add_link_between_rows(
                     LinkBetweenRows(
@@ -389,28 +366,26 @@
                         i,
                         Label="to_first_table",
                         Importance=4,
                         Color=Colors.LIGHT_BLUE,
                     )
                 )
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ![table_advanced](./readme_images/table_advanced.png)
 
 #### BarChart Element
 
 This element displays a modular horizontal barchart. It has several configuration options, so I'll try to show-case several of them.
 
 The default bar-chart displays a horizontal selectable bar-chart. It is useful for displaying softmax distributions for the next token prediction. I implemented it in such a way that it is selectable, hence you can navigate the whole process of sequence generation in the same way as the automatic generation would do. Hence this component also implements frontend-backend communication and you can supply an `endpoint_callback` to it.
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/bar_chart_component_simple.py&lines=1-47&header=# ./examples_py/bar_chart_component_simple.py lines 1-47)-->
 <!-- The below code snippet is automatically added from ./examples_py/bar_chart_component_simple.py -->
-
 ```py
 # ./examples_py/bar_chart_component_simple.py lines 1-47
 import heapq
 import math
 import random
 
 import requests
@@ -453,15 +428,14 @@
         )
 
     def barchart_callback(self):
         s = self.barchart_element.selected
         self.text_element.content = f"Last selected: {s}"
         self.update_barchart_component()
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ![barchart_simple](./readme_images/barchart_simple.png)
 
 When you set `long_contexts` option to true, the bar charts will be below the bar titles.
 
 ![barchart_long_contexts](./readme_images/barchart_long_contexts.png)
@@ -470,15 +444,14 @@
 
 This example will display the advanced possibilities I use when e.g. comparing different generation candidates provided by the model.
 
 When I want to compare several candidates, I can display multi-bar-chart, e.g. add multiple bars with different heights, different annotations, each describing one particular quality of the generated sample.
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/bar_chart_component_advanced.py&lines=1-46&header=# ./examples_py/bar_chart_component_advanced.py lines 1-46)-->
 <!-- The below code snippet is automatically added from ./examples_py/bar_chart_component_advanced.py -->
-
 ```py
 # ./examples_py/bar_chart_component_advanced.py lines 1-46
 import math
 import random
 from typing import List
 
 from visuallm.component_base import ComponentBase
@@ -520,11 +493,10 @@
             "This will indicate the state of the repository that should be "
             + "evaluated.",
         ]
         self.barchart_element.set_possibilities(
             bar_heights, bar_annotations, annotations
         )
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ![barchart_advanced](./readme_images/barchart_advanced.png)
```

### Comparing `visuallm-0.1.6/README.md` & `visuallm-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Conditional Language Model Generation Visualization
 
-## VERSION: `0.1.6`
+## VERSION: `0.1.7`
 
 - when evaluating language models it is often pain to see what is generated and why
 - this little package is a `vue.js` frontend together with `flask` backend and it is designed to easily show some interesting visualizations on conditional generation models
 - it handles frontend-backend communication as well as frontend rendering
 - hence the developper can focus only on ML aspects of his work!
 
 ## Installation
@@ -24,15 +24,14 @@
 
 1. Create a class inheriting from `llm_generation_server.component_base.ComponentBase`. In `__init__` you should:
 
 - create all the elements from which the page should be composed
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/simple_component.py&lines=1-15&header=# ./examples_py/simple_component.py lines 1-15)-->
 <!-- The below code snippet is automatically added from ./examples_py/simple_component.py -->
-
 ```py
 # ./examples_py/simple_component.py lines 1-15
 from visuallm.component_base import ComponentBase
 from visuallm.elements.plain_text_element import PlainTextElement
 
 
 class SimpleComponent(ComponentBase):
@@ -43,48 +42,43 @@
         self.text_element = PlainTextElement(
             content="""
                 Some really interesting text that isn't formatted in any way, it is
                 just a plain simple text
             """
         )
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 - call `super().__init__`, where you specify name and title of the component as well as the created elements in the order that they should appear in the page
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/simple_component.py&lines=16-21&header=# ./examples_py/simple_component.py lines 16-21)-->
 <!-- The below code snippet is automatically added from ./examples_py/simple_component.py -->
-
 ```py
 # ./examples_py/simple_component.py lines 16-21
         super().__init__(
             name="simple_component",
             title="Simple Component",
             elements=[self.main_heading_element, self.text_element],
         )
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 2. Initialize `llm_generation_server.server.Server` and pass in the initialized components
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/simple_app.py&lines=1-7&header=# ./examples_py/simple_app.py)-->
 <!-- The below code snippet is automatically added from ./examples_py/simple_app.py -->
-
 ```py
 # ./examples_py/simple_app.py
 from visuallm.server import Server
 
 from .simple_component import SimpleComponent
 
 server = Server(__name__, [SimpleComponent()])
 app = server.app
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 3. Standard method to run the flask application, e.g. for the example provided above, it would be
 
 ```sh
 python3 -m flask --app examples_py.simple_app run
 ```
@@ -95,15 +89,14 @@
 
 I wrote this library to help me visualize the output distributions of various models I implemented during my master's thesis. Therefore I implemented only few basic elements for ML purposes.
 
 In the following paragraphs I'll explain how to create configuration selectors, tables and bar-charts, and I'll use the following server: (You'll see the implementation of each of yet unknown components)
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/app.py&header=# ./examples_py/app.py)-->
 <!-- The below code snippet is automatically added from ./examples_py/app.py -->
-
 ```py
 # ./examples_py/app.py
 from visuallm.server import Server
 
 from .bar_chart_component_advanced import BarChartComponentAdvanced
 from .bar_chart_component_simple import BarChartComponentSimple
 from .selector_component import SelectorComponent
@@ -119,102 +112,92 @@
         TableComponent(),
         TwoTablesComponent(),
         SelectorComponent(),
     ],
 )
 app = flask_app.app
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 You can see the generated page by running the following script after cloning the github repository and navigating into it:
 
 ```sh
 flask --app examples_py.app run
 ```
 
 #### Configuration Selection
 
 Several different kinds of configuration specifier, together with one button element. The button element allows backend communication and by itself it does nothing. However you can specify subelements, for which the button element will provide communication updates. For the example below, the following imports will be used:
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/selector_component.py&lines=1-10&header=# ./examples_py/selector_component.py lines 1-10)-->
 <!-- The below code snippet is automatically added from ./examples_py/selector_component.py -->
-
 ```py
 # ./examples_py/selector_component.py lines 1-10
 import time
 
 from visuallm.component_base import ComponentBase
 from visuallm.elements.plain_text_element import PlainTextElement
 from visuallm.elements.selector_elements import (
     ButtonElement,
     CheckBoxSubElement,
     ChoicesSubElement,
     MinMaxSubElement,
 )
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ##### MinMax SubElement
 
 Input element for setting integer in a range.
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/selector_component.py&lines=13-18&header=# ./examples_py/selector_component.py lines 13-18)-->
 <!-- The below code snippet is automatically added from ./examples_py/selector_component.py -->
-
 ```py
 # ./examples_py/selector_component.py lines 13-18
 class SelectorComponent(ComponentBase):
     def __init__(self):
         self.text_element = PlainTextElement(content="Nothing was selected")
         self.number_selector_element = MinMaxSubElement(
             sample_min=0, sample_max=10, text="Select Number:"
         )
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ##### Choices SubElement
 
 Input element for choosing between several choices.
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/selector_component.py&lines=19-21&header=# ./examples_py/selector_component.py lines 19-21)-->
 <!-- The below code snippet is automatically added from ./examples_py/selector_component.py -->
-
 ```py
 # ./examples_py/selector_component.py lines 19-21
         self.choices_element = ChoicesSubElement(
             choices=["super", "magnificent", "incredible"], text="This library is:"
         )
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ##### Checkbox SubElement
 
 Simple checkbox input element.
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/selector_component.py&lines=22-22&header=# ./examples_py/selector_component.py lines 22)-->
 <!-- The below code snippet is automatically added from ./examples_py/selector_component.py -->
-
 ```py
 # ./examples_py/selector_component.py lines 22
         self.checkbox_element = CheckBoxSubElement(text="Have you slept?:")
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ##### Button Element
 
 This is an element that should encapsulate all the other configuration selection elements. It needs a callback method that will be called when the button is pressed and we provide `ButtonElement.default_select_callback()` which handles processing all the changes sent from the frontend and attributing them to `subelement.selected` properties of subelements.
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/selector_component.py&lines=23-61&header=# ./examples_py/selector_component.py lines 23-61)-->
 <!-- The below code snippet is automatically added from ./examples_py/selector_component.py -->
-
 ```py
 # ./examples_py/selector_component.py lines 23-61
         self.button_element = ButtonElement(
             processing_callback=self.button_clicked,
             subelements=[
                 self.number_selector_element,
                 self.choices_element,
@@ -249,27 +232,25 @@
         self.text_element.content = (
             f"This library is {c} and I would give "
             + f"it {n} stars out of {n} if I could. ({b})"
             + f" This {'has' if any_updated else 'has not'} changed!"
         )
         time.sleep(n)
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ![selector_image](./readme_images/selector.png)
 
 #### Table Element
 
 This element can show several tables on the frontend together with a special feature, links between rows of the tables. They may connect different rows of different tables and display some value above links.
 The below example displays, how to generate one table on the frontend with the links pointing from each row to all the upwards rows as displayed on the image.
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/table_component.py&header=# ./examples_py/table_component.py)-->
 <!-- The below code snippet is automatically added from ./examples_py/table_component.py -->
-
 ```py
 # ./examples_py/table_component.py
 from visuallm.component_base import ComponentBase
 from visuallm.elements.plain_text_element import PlainTextElement
 from visuallm.elements.table_element import LinkBetweenRows, TableElement
 
 
@@ -312,46 +293,42 @@
         # add links pointing to all the rows upwards
         for j in range(len(rows) - 1, 0, -1):
             for i in range(j):
                 self.table_element.add_link_between_rows(
                     LinkBetweenRows(TABLE_NAME, j, TABLE_NAME, i, Label="some value")
                 )
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ![table_page](./readme_images/table.png)
 
 #### Table Element (Advanced)
 
 Let's look at an advanced example of table element, where we create two tables and add links which connect multiple tables. I will only show the important snippets of code.
 
 Firstly, we will import `Colors` enumeration to color links to different tables with different colors.
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/two_tables_component.py&header=# ./examples_py/two_tables_component.py lines 1-7&lines=1-7)-->
 <!-- The below code snippet is automatically added from ./examples_py/two_tables_component.py -->
-
 ```py
 # ./examples_py/two_tables_component.py lines 1-7
 from visuallm.component_base import ComponentBase
 from visuallm.elements.plain_text_element import PlainTextElement
 from visuallm.elements.table_element import Colors, LinkBetweenRows, TableElement
 
 
 class TwoTablesComponent(ComponentBase):
     def __init__(self):
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 Secondly, we will create the links in such a way, that links going within the same table will be colored orange (the default color), while the links going to the other table will be colored light blue. Also links within one table will be thin, while links to the other table will be thick (`Importance` parameter).
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/two_tables_component.py&header=# ./examples_py/two_tables_component.py lines 69-99&lines=69-99)-->
 <!-- The below code snippet is automatically added from ./examples_py/two_tables_component.py -->
-
 ```py
 # ./examples_py/two_tables_component.py lines 69-99
             # links going from the row j of the second table to all the upper
             # rows in the second table
             for i in range(j):
                 self.table_element.add_link_between_rows(
                     LinkBetweenRows(
@@ -374,28 +351,26 @@
                         i,
                         Label="to_first_table",
                         Importance=4,
                         Color=Colors.LIGHT_BLUE,
                     )
                 )
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ![table_advanced](./readme_images/table_advanced.png)
 
 #### BarChart Element
 
 This element displays a modular horizontal barchart. It has several configuration options, so I'll try to show-case several of them.
 
 The default bar-chart displays a horizontal selectable bar-chart. It is useful for displaying softmax distributions for the next token prediction. I implemented it in such a way that it is selectable, hence you can navigate the whole process of sequence generation in the same way as the automatic generation would do. Hence this component also implements frontend-backend communication and you can supply an `endpoint_callback` to it.
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/bar_chart_component_simple.py&lines=1-47&header=# ./examples_py/bar_chart_component_simple.py lines 1-47)-->
 <!-- The below code snippet is automatically added from ./examples_py/bar_chart_component_simple.py -->
-
 ```py
 # ./examples_py/bar_chart_component_simple.py lines 1-47
 import heapq
 import math
 import random
 
 import requests
@@ -438,15 +413,14 @@
         )
 
     def barchart_callback(self):
         s = self.barchart_element.selected
         self.text_element.content = f"Last selected: {s}"
         self.update_barchart_component()
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ![barchart_simple](./readme_images/barchart_simple.png)
 
 When you set `long_contexts` option to true, the bar charts will be below the bar titles.
 
 ![barchart_long_contexts](./readme_images/barchart_long_contexts.png)
@@ -455,15 +429,14 @@
 
 This example will display the advanced possibilities I use when e.g. comparing different generation candidates provided by the model.
 
 When I want to compare several candidates, I can display multi-bar-chart, e.g. add multiple bars with different heights, different annotations, each describing one particular quality of the generated sample.
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/bar_chart_component_advanced.py&lines=1-46&header=# ./examples_py/bar_chart_component_advanced.py lines 1-46)-->
 <!-- The below code snippet is automatically added from ./examples_py/bar_chart_component_advanced.py -->
-
 ```py
 # ./examples_py/bar_chart_component_advanced.py lines 1-46
 import math
 import random
 from typing import List
 
 from visuallm.component_base import ComponentBase
@@ -505,11 +478,10 @@
             "This will indicate the state of the repository that should be "
             + "evaluated.",
         ]
         self.barchart_element.set_possibilities(
             bar_heights, bar_annotations, annotations
         )
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ![barchart_advanced](./readme_images/barchart_advanced.png)
```

### Comparing `visuallm-0.1.6/pyproject.toml` & `visuallm-0.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "visuallm"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Frantisek Trebuna (gortibaldik)", email="ferotre@gmail.com" },
 ]
 description = "Visualization tool for various generation tasks on Language Models. "
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -34,15 +34,15 @@
 [tool.setuptools.package-dir]
 visuallm = "visuallm"
 
 [tool.isort]
 profile = "black"
 
 [tool.bumpver]
-current_version = "0.1.6"
+current_version = "0.1.7"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `visuallm-0.1.6/visuallm/component_base.py` & `visuallm-0.1.7/visuallm/component_base.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.6/visuallm/components/DatasetVisualizationComponent.py` & `visuallm-0.1.7/visuallm/components/DatasetVisualizationComponent.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.6/visuallm/components/GenerationComponent.py` & `visuallm-0.1.7/visuallm/components/GenerationComponent.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.6/visuallm/components/NextTokenPredictionComponent.py` & `visuallm-0.1.7/visuallm/components/NextTokenPredictionComponent.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.6/visuallm/components/mixins/data_preparation_mixin.py` & `visuallm-0.1.7/visuallm/components/mixins/data_preparation_mixin.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.6/visuallm/components/mixins/generation_selectors_mixin.py` & `visuallm-0.1.7/visuallm/components/mixins/generation_selectors_mixin.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.6/visuallm/components/mixins/metrics_mixin.py` & `visuallm-0.1.7/visuallm/components/mixins/metrics_mixin.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.6/visuallm/components/mixins/model_selection_mixin.py` & `visuallm-0.1.7/visuallm/components/mixins/model_selection_mixin.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.6/visuallm/dist/assets/index-9006265c.js` & `visuallm-0.1.7/visuallm/dist/assets/index-9006265c.js`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.6/visuallm/dist/assets/index-d8f16c2e.css` & `visuallm-0.1.7/visuallm/dist/assets/index-d8f16c2e.css`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.6/visuallm/dist/favicon.ico` & `visuallm-0.1.7/visuallm/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.6/visuallm/elements/barchart_element.py` & `visuallm-0.1.7/visuallm/elements/barchart_element.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.6/visuallm/elements/element_base.py` & `visuallm-0.1.7/visuallm/elements/element_base.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.6/visuallm/elements/plain_text_element.py` & `visuallm-0.1.7/visuallm/elements/plain_text_element.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.6/visuallm/elements/selector_elements.py` & `visuallm-0.1.7/visuallm/elements/selector_elements.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.6/visuallm/elements/table_element.py` & `visuallm-0.1.7/visuallm/elements/table_element.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.6/visuallm/elements/utils.py` & `visuallm-0.1.7/visuallm/elements/utils.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.6/visuallm/server.py` & `visuallm-0.1.7/visuallm/server.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.6/visuallm.egg-info/PKG-INFO` & `visuallm-0.1.7/visuallm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: visuallm
-Version: 0.1.6
+Version: 0.1.7
 Summary: Visualization tool for various generation tasks on Language Models. 
 Author-email: "Frantisek Trebuna (gortibaldik)" <ferotre@gmail.com>
 Project-URL: Homepage, https://github.com/gortibaldik/visuallm
 Project-URL: Bug Tracker, https://github.com/gortibaldik/visuallm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: huggingface
 License-File: LICENSE
 
 # Conditional Language Model Generation Visualization
 
-## VERSION: `0.1.6`
+## VERSION: `0.1.7`
 
 - when evaluating language models it is often pain to see what is generated and why
 - this little package is a `vue.js` frontend together with `flask` backend and it is designed to easily show some interesting visualizations on conditional generation models
 - it handles frontend-backend communication as well as frontend rendering
 - hence the developper can focus only on ML aspects of his work!
 
 ## Installation
@@ -39,15 +39,14 @@
 
 1. Create a class inheriting from `llm_generation_server.component_base.ComponentBase`. In `__init__` you should:
 
 - create all the elements from which the page should be composed
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/simple_component.py&lines=1-15&header=# ./examples_py/simple_component.py lines 1-15)-->
 <!-- The below code snippet is automatically added from ./examples_py/simple_component.py -->
-
 ```py
 # ./examples_py/simple_component.py lines 1-15
 from visuallm.component_base import ComponentBase
 from visuallm.elements.plain_text_element import PlainTextElement
 
 
 class SimpleComponent(ComponentBase):
@@ -58,48 +57,43 @@
         self.text_element = PlainTextElement(
             content="""
                 Some really interesting text that isn't formatted in any way, it is
                 just a plain simple text
             """
         )
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 - call `super().__init__`, where you specify name and title of the component as well as the created elements in the order that they should appear in the page
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/simple_component.py&lines=16-21&header=# ./examples_py/simple_component.py lines 16-21)-->
 <!-- The below code snippet is automatically added from ./examples_py/simple_component.py -->
-
 ```py
 # ./examples_py/simple_component.py lines 16-21
         super().__init__(
             name="simple_component",
             title="Simple Component",
             elements=[self.main_heading_element, self.text_element],
         )
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 2. Initialize `llm_generation_server.server.Server` and pass in the initialized components
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/simple_app.py&lines=1-7&header=# ./examples_py/simple_app.py)-->
 <!-- The below code snippet is automatically added from ./examples_py/simple_app.py -->
-
 ```py
 # ./examples_py/simple_app.py
 from visuallm.server import Server
 
 from .simple_component import SimpleComponent
 
 server = Server(__name__, [SimpleComponent()])
 app = server.app
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 3. Standard method to run the flask application, e.g. for the example provided above, it would be
 
 ```sh
 python3 -m flask --app examples_py.simple_app run
 ```
@@ -110,15 +104,14 @@
 
 I wrote this library to help me visualize the output distributions of various models I implemented during my master's thesis. Therefore I implemented only few basic elements for ML purposes.
 
 In the following paragraphs I'll explain how to create configuration selectors, tables and bar-charts, and I'll use the following server: (You'll see the implementation of each of yet unknown components)
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/app.py&header=# ./examples_py/app.py)-->
 <!-- The below code snippet is automatically added from ./examples_py/app.py -->
-
 ```py
 # ./examples_py/app.py
 from visuallm.server import Server
 
 from .bar_chart_component_advanced import BarChartComponentAdvanced
 from .bar_chart_component_simple import BarChartComponentSimple
 from .selector_component import SelectorComponent
@@ -134,102 +127,92 @@
         TableComponent(),
         TwoTablesComponent(),
         SelectorComponent(),
     ],
 )
 app = flask_app.app
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 You can see the generated page by running the following script after cloning the github repository and navigating into it:
 
 ```sh
 flask --app examples_py.app run
 ```
 
 #### Configuration Selection
 
 Several different kinds of configuration specifier, together with one button element. The button element allows backend communication and by itself it does nothing. However you can specify subelements, for which the button element will provide communication updates. For the example below, the following imports will be used:
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/selector_component.py&lines=1-10&header=# ./examples_py/selector_component.py lines 1-10)-->
 <!-- The below code snippet is automatically added from ./examples_py/selector_component.py -->
-
 ```py
 # ./examples_py/selector_component.py lines 1-10
 import time
 
 from visuallm.component_base import ComponentBase
 from visuallm.elements.plain_text_element import PlainTextElement
 from visuallm.elements.selector_elements import (
     ButtonElement,
     CheckBoxSubElement,
     ChoicesSubElement,
     MinMaxSubElement,
 )
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ##### MinMax SubElement
 
 Input element for setting integer in a range.
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/selector_component.py&lines=13-18&header=# ./examples_py/selector_component.py lines 13-18)-->
 <!-- The below code snippet is automatically added from ./examples_py/selector_component.py -->
-
 ```py
 # ./examples_py/selector_component.py lines 13-18
 class SelectorComponent(ComponentBase):
     def __init__(self):
         self.text_element = PlainTextElement(content="Nothing was selected")
         self.number_selector_element = MinMaxSubElement(
             sample_min=0, sample_max=10, text="Select Number:"
         )
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ##### Choices SubElement
 
 Input element for choosing between several choices.
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/selector_component.py&lines=19-21&header=# ./examples_py/selector_component.py lines 19-21)-->
 <!-- The below code snippet is automatically added from ./examples_py/selector_component.py -->
-
 ```py
 # ./examples_py/selector_component.py lines 19-21
         self.choices_element = ChoicesSubElement(
             choices=["super", "magnificent", "incredible"], text="This library is:"
         )
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ##### Checkbox SubElement
 
 Simple checkbox input element.
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/selector_component.py&lines=22-22&header=# ./examples_py/selector_component.py lines 22)-->
 <!-- The below code snippet is automatically added from ./examples_py/selector_component.py -->
-
 ```py
 # ./examples_py/selector_component.py lines 22
         self.checkbox_element = CheckBoxSubElement(text="Have you slept?:")
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ##### Button Element
 
 This is an element that should encapsulate all the other configuration selection elements. It needs a callback method that will be called when the button is pressed and we provide `ButtonElement.default_select_callback()` which handles processing all the changes sent from the frontend and attributing them to `subelement.selected` properties of subelements.
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/selector_component.py&lines=23-61&header=# ./examples_py/selector_component.py lines 23-61)-->
 <!-- The below code snippet is automatically added from ./examples_py/selector_component.py -->
-
 ```py
 # ./examples_py/selector_component.py lines 23-61
         self.button_element = ButtonElement(
             processing_callback=self.button_clicked,
             subelements=[
                 self.number_selector_element,
                 self.choices_element,
@@ -264,27 +247,25 @@
         self.text_element.content = (
             f"This library is {c} and I would give "
             + f"it {n} stars out of {n} if I could. ({b})"
             + f" This {'has' if any_updated else 'has not'} changed!"
         )
         time.sleep(n)
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ![selector_image](./readme_images/selector.png)
 
 #### Table Element
 
 This element can show several tables on the frontend together with a special feature, links between rows of the tables. They may connect different rows of different tables and display some value above links.
 The below example displays, how to generate one table on the frontend with the links pointing from each row to all the upwards rows as displayed on the image.
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/table_component.py&header=# ./examples_py/table_component.py)-->
 <!-- The below code snippet is automatically added from ./examples_py/table_component.py -->
-
 ```py
 # ./examples_py/table_component.py
 from visuallm.component_base import ComponentBase
 from visuallm.elements.plain_text_element import PlainTextElement
 from visuallm.elements.table_element import LinkBetweenRows, TableElement
 
 
@@ -327,46 +308,42 @@
         # add links pointing to all the rows upwards
         for j in range(len(rows) - 1, 0, -1):
             for i in range(j):
                 self.table_element.add_link_between_rows(
                     LinkBetweenRows(TABLE_NAME, j, TABLE_NAME, i, Label="some value")
                 )
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ![table_page](./readme_images/table.png)
 
 #### Table Element (Advanced)
 
 Let's look at an advanced example of table element, where we create two tables and add links which connect multiple tables. I will only show the important snippets of code.
 
 Firstly, we will import `Colors` enumeration to color links to different tables with different colors.
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/two_tables_component.py&header=# ./examples_py/two_tables_component.py lines 1-7&lines=1-7)-->
 <!-- The below code snippet is automatically added from ./examples_py/two_tables_component.py -->
-
 ```py
 # ./examples_py/two_tables_component.py lines 1-7
 from visuallm.component_base import ComponentBase
 from visuallm.elements.plain_text_element import PlainTextElement
 from visuallm.elements.table_element import Colors, LinkBetweenRows, TableElement
 
 
 class TwoTablesComponent(ComponentBase):
     def __init__(self):
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 Secondly, we will create the links in such a way, that links going within the same table will be colored orange (the default color), while the links going to the other table will be colored light blue. Also links within one table will be thin, while links to the other table will be thick (`Importance` parameter).
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/two_tables_component.py&header=# ./examples_py/two_tables_component.py lines 69-99&lines=69-99)-->
 <!-- The below code snippet is automatically added from ./examples_py/two_tables_component.py -->
-
 ```py
 # ./examples_py/two_tables_component.py lines 69-99
             # links going from the row j of the second table to all the upper
             # rows in the second table
             for i in range(j):
                 self.table_element.add_link_between_rows(
                     LinkBetweenRows(
@@ -389,28 +366,26 @@
                         i,
                         Label="to_first_table",
                         Importance=4,
                         Color=Colors.LIGHT_BLUE,
                     )
                 )
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ![table_advanced](./readme_images/table_advanced.png)
 
 #### BarChart Element
 
 This element displays a modular horizontal barchart. It has several configuration options, so I'll try to show-case several of them.
 
 The default bar-chart displays a horizontal selectable bar-chart. It is useful for displaying softmax distributions for the next token prediction. I implemented it in such a way that it is selectable, hence you can navigate the whole process of sequence generation in the same way as the automatic generation would do. Hence this component also implements frontend-backend communication and you can supply an `endpoint_callback` to it.
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/bar_chart_component_simple.py&lines=1-47&header=# ./examples_py/bar_chart_component_simple.py lines 1-47)-->
 <!-- The below code snippet is automatically added from ./examples_py/bar_chart_component_simple.py -->
-
 ```py
 # ./examples_py/bar_chart_component_simple.py lines 1-47
 import heapq
 import math
 import random
 
 import requests
@@ -453,15 +428,14 @@
         )
 
     def barchart_callback(self):
         s = self.barchart_element.selected
         self.text_element.content = f"Last selected: {s}"
         self.update_barchart_component()
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ![barchart_simple](./readme_images/barchart_simple.png)
 
 When you set `long_contexts` option to true, the bar charts will be below the bar titles.
 
 ![barchart_long_contexts](./readme_images/barchart_long_contexts.png)
@@ -470,15 +444,14 @@
 
 This example will display the advanced possibilities I use when e.g. comparing different generation candidates provided by the model.
 
 When I want to compare several candidates, I can display multi-bar-chart, e.g. add multiple bars with different heights, different annotations, each describing one particular quality of the generated sample.
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/bar_chart_component_advanced.py&lines=1-46&header=# ./examples_py/bar_chart_component_advanced.py lines 1-46)-->
 <!-- The below code snippet is automatically added from ./examples_py/bar_chart_component_advanced.py -->
-
 ```py
 # ./examples_py/bar_chart_component_advanced.py lines 1-46
 import math
 import random
 from typing import List
 
 from visuallm.component_base import ComponentBase
@@ -520,11 +493,10 @@
             "This will indicate the state of the repository that should be "
             + "evaluated.",
         ]
         self.barchart_element.set_possibilities(
             bar_heights, bar_annotations, annotations
         )
 ```
-
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ![barchart_advanced](./readme_images/barchart_advanced.png)
```

### Comparing `visuallm-0.1.6/visuallm.egg-info/SOURCES.txt` & `visuallm-0.1.7/visuallm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

