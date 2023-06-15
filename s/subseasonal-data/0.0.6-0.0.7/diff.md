# Comparing `tmp/subseasonal_data-0.0.6.tar.gz` & `tmp/subseasonal_data-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subseasonal_data-0.0.6.tar", last modified: Wed Feb 15 19:35:26 2023, max compression
+gzip compressed data, was "subseasonal_data-0.0.7.tar", last modified: Thu Jun 15 21:01:18 2023, max compression
```

## Comparing `subseasonal_data-0.0.6.tar` & `subseasonal_data-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lmackey    (501) staff       (20)        0 2023-02-15 19:35:26.598713 subseasonal_data-0.0.6/
--rw-r--r--   0 lmackey    (501) staff       (20)     1141 2023-02-15 19:25:46.000000 subseasonal_data-0.0.6/LICENSE
--rw-r--r--   0 lmackey    (501) staff       (20)     6113 2023-02-15 19:35:26.598927 subseasonal_data-0.0.6/PKG-INFO
--rw-r--r--   0 lmackey    (501) staff       (20)     5950 2023-02-15 19:25:46.000000 subseasonal_data-0.0.6/README.md
--rw-r--r--   0 lmackey    (501) staff       (20)      418 2023-02-15 19:35:26.600422 subseasonal_data-0.0.6/setup.cfg
--rw-r--r--   0 lmackey    (501) staff       (20)       98 2023-02-15 19:25:46.000000 subseasonal_data-0.0.6/setup.py
-drwxr-xr-x   0 lmackey    (501) staff       (20)        0 2023-02-15 19:35:26.583344 subseasonal_data-0.0.6/subseasonal_data/
--rw-r--r--   0 lmackey    (501) staff       (20)        0 2023-02-15 19:25:46.000000 subseasonal_data-0.0.6/subseasonal_data/__init__.py
--rw-r--r--   0 lmackey    (501) staff       (20)    31422 2023-02-15 19:25:46.000000 subseasonal_data-0.0.6/subseasonal_data/data_loaders.py
--rw-r--r--   0 lmackey    (501) staff       (20)     7311 2023-02-15 19:25:46.000000 subseasonal_data-0.0.6/subseasonal_data/downloader.py
--rw-r--r--   0 lmackey    (501) staff       (20)    11017 2023-02-15 19:25:46.000000 subseasonal_data-0.0.6/subseasonal_data/utils.py
-drwxr-xr-x   0 lmackey    (501) staff       (20)        0 2023-02-15 19:35:26.598126 subseasonal_data-0.0.6/subseasonal_data.egg-info/
--rw-r--r--   0 lmackey    (501) staff       (20)     6113 2023-02-15 19:35:26.000000 subseasonal_data-0.0.6/subseasonal_data.egg-info/PKG-INFO
--rw-r--r--   0 lmackey    (501) staff       (20)      354 2023-02-15 19:35:26.000000 subseasonal_data-0.0.6/subseasonal_data.egg-info/SOURCES.txt
--rw-r--r--   0 lmackey    (501) staff       (20)        1 2023-02-15 19:35:26.000000 subseasonal_data-0.0.6/subseasonal_data.egg-info/dependency_links.txt
--rw-r--r--   0 lmackey    (501) staff       (20)       34 2023-02-15 19:35:26.000000 subseasonal_data-0.0.6/subseasonal_data.egg-info/requires.txt
--rw-r--r--   0 lmackey    (501) staff       (20)       17 2023-02-15 19:35:26.000000 subseasonal_data-0.0.6/subseasonal_data.egg-info/top_level.txt
+drwxr-xr-x   0 lmackey    (501) staff       (20)        0 2023-06-15 21:01:18.817960 subseasonal_data-0.0.7/
+-rw-r--r--   0 lmackey    (501) staff       (20)     1141 2023-06-15 20:59:54.000000 subseasonal_data-0.0.7/LICENSE
+-rw-r--r--   0 lmackey    (501) staff       (20)     6454 2023-06-15 21:01:18.818089 subseasonal_data-0.0.7/PKG-INFO
+-rw-r--r--   0 lmackey    (501) staff       (20)     6169 2023-06-15 20:59:54.000000 subseasonal_data-0.0.7/README.md
+-rw-r--r--   0 lmackey    (501) staff       (20)      418 2023-06-15 21:01:18.819099 subseasonal_data-0.0.7/setup.cfg
+-rw-r--r--   0 lmackey    (501) staff       (20)       98 2023-06-15 20:59:54.000000 subseasonal_data-0.0.7/setup.py
+drwxr-xr-x   0 lmackey    (501) staff       (20)        0 2023-06-15 21:01:18.804639 subseasonal_data-0.0.7/subseasonal_data/
+-rw-r--r--   0 lmackey    (501) staff       (20)        0 2023-06-15 20:59:54.000000 subseasonal_data-0.0.7/subseasonal_data/__init__.py
+-rw-r--r--   0 lmackey    (501) staff       (20)    31422 2023-06-15 20:59:54.000000 subseasonal_data-0.0.7/subseasonal_data/data_loaders.py
+-rw-r--r--   0 lmackey    (501) staff       (20)     7311 2023-06-15 20:59:54.000000 subseasonal_data-0.0.7/subseasonal_data/downloader.py
+-rw-r--r--   0 lmackey    (501) staff       (20)    11017 2023-06-15 20:59:54.000000 subseasonal_data-0.0.7/subseasonal_data/utils.py
+drwxr-xr-x   0 lmackey    (501) staff       (20)        0 2023-06-15 21:01:18.817427 subseasonal_data-0.0.7/subseasonal_data.egg-info/
+-rw-r--r--   0 lmackey    (501) staff       (20)     6454 2023-06-15 21:01:18.000000 subseasonal_data-0.0.7/subseasonal_data.egg-info/PKG-INFO
+-rw-r--r--   0 lmackey    (501) staff       (20)      354 2023-06-15 21:01:18.000000 subseasonal_data-0.0.7/subseasonal_data.egg-info/SOURCES.txt
+-rw-r--r--   0 lmackey    (501) staff       (20)        1 2023-06-15 21:01:18.000000 subseasonal_data-0.0.7/subseasonal_data.egg-info/dependency_links.txt
+-rw-r--r--   0 lmackey    (501) staff       (20)       34 2023-06-15 21:01:18.000000 subseasonal_data-0.0.7/subseasonal_data.egg-info/requires.txt
+-rw-r--r--   0 lmackey    (501) staff       (20)       17 2023-06-15 21:01:18.000000 subseasonal_data-0.0.7/subseasonal_data.egg-info/top_level.txt
```

### Comparing `subseasonal_data-0.0.6/LICENSE` & `subseasonal_data-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `subseasonal_data-0.0.6/PKG-INFO` & `subseasonal_data-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subseasonal_data
-Version: 0.0.6
+Version: 0.0.7
 Summary: Data access package for the SubseasonalClimateUSA dataset.
 Home-page: https://github.com/microsoft/subseasonal_data
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -91,23 +91,25 @@
 
 To generate a local copy of the documentation from a clone of this repository, run `python setup.py build_sphinx -W -E -a`, which will build the documentation and place it under the `build/sphinx/html` path. 
 
 The reStructuredText files that make up the documentation are stored in the `docs` directory; module documentation is automatically generated by the Sphinx build process.
 
 ## Data Usage and Citation
 
+The **SubseasonalClimateUSA** dataset is released under a [CC BY 4.0 license](https://creativecommons.org/licenses/by/4.0/), and the `subseasonal_data` repository code is released under an [MIT license](https://github.com/microsoft/subseasonal_data/blob/main/LICENSE).
+
 If you make use of the `subseasonal_data` package or the **SubseasonalClimateUSA** dataset, please acknowledge the Python package, the individual data sources described in [DATA.md](https://github.com/microsoft/subseasonal_data/blob/main/DATA.md), and the associated **SubseasonalClimateUSA** preprint:
 
-[Learned Benchmarks for Subseasonal Forecasting](https://arxiv.org/pdf/2109.10399.pdf)  
+[**SubseasonalClimateUSA**: A Dataset for Subseasonal Forecasting and Benchmarking](https://arxiv.org/pdf/2109.10399.pdf)  
 Soukayna Mouatadid, Paulo Orenstein, Genevieve Flaspohler, Miruna Oprescu, Judah Cohen, Franklyn Wang, Sean Knight, Maria Geogdzhayeva, Sam Levang, Ernest Fraenkel, and Lester Mackey.  Sep. 2021.
 
 ```
 @article{
-  mouatadid2021toolkit,
-  title={Learned Benchmarks for Subseasonal Forecasting},
+  mouatadid2021subseasonal,
+  title={SubseasonalClimateUSA: A Dataset for Subseasonal Forecasting and Benchmarking},
   author={Soukayna Mouatadid, Paulo Orenstein, Genevieve Flaspohler, Miruna Oprescu, Judah Cohen, Franklyn Wang, Sean Knight, Maria Geogdzhayeva, Sam Levang, Ernest Fraenkel, and Lester Mackey},
   journal={arXiv preprint arXiv:2109.10399},
   year={2021}
 }
 ```
 
 ## Contributing
@@ -128,7 +130,8 @@
 
 This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft 
 trademarks or logos is subject to and must follow 
 [Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
 Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
 Any use of third-party trademarks or logos are subject to those third-party's policies.
 
+
```

### Comparing `subseasonal_data-0.0.6/README.md` & `subseasonal_data-0.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,123 +1,125 @@
-# Subseasonal Data Python Package
-
-The `subseasonal_data` package provides an API for loading and manipulating the **SubseasonalClimateUSA** dataset developed for training and benchmarking subseasonal forecasting models.  Here, _subseasonal_ refers to climate and weather forecasts made 2-6 weeks in advance.  See [DATA.md](https://github.com/microsoft/subseasonal_data/blob/main/DATA.md) for a description of dataset contents, sources, and processing.
-
-## Getting Started
-
-- Install the subseasonal data package: `pip install subseasonal-data`
-- Define the environment variable `$SUBSEASONALDATA_PATH` to point to your desired data directory; any accessed data files will be read from, saved to, or synced with this directory
-
- This package is compatible with Python version 3.6+. 
- 
- The underlying data is made available through Azure and is updated periodically. To download the data through this package, you will need to have the Azure Storage CLI [`azcopy`](https://docs.microsoft.com/en-us/azure/storage/common/storage-use-azcopy) installed on your machine.
-
-## Usage Examples
-
-Detailed usage examples are provided in the `Getting Started` and `Examples` notebooks in the `examples` folder. It is recommended you start there.
-
-Quick examples:
-
-* Download all data
-
-**WARNING:** This requires an estimated 175GB disk space.
-
-```Python
-from subseasonal_data import downloader
-
-downloader.download()
-```
-
-* List files in a data directory
-
-```Python
-downloader.list_subdir_files(data_subdir="combined_dataframes")
-```
-
-* Download one data file
-
-```Python
-downloader.download_file(
-    data_subdir="combined_dataframes", 
-    filename="all_data-us_precip_34w.feather", 
-    verbose=True)
-```
-
-* Load ground truth data
-
-```Python
-from subseasonal_data import data_loaders
-
-# Loads into a Pandas dataframe
-df = data_loaders.get_ground_truth("us_precip")
-```
-
-* Load combined dataframes
-
-```Python
-data_loaders.load_combined_data("all_data", "us_tmp2m", "34w")
-```
-
-See the [Examples.ipynb](https://github.com/microsoft/subseasonal_data/blob/main/examples/Examples.ipynb) notebook for an example on how to retrieve historical temperature data using the `subseasonal_data` package. 
-
-![Usage Example](https://github.com/microsoft/subseasonal_data/blob/main/usage_example.gif)
-
-## For Developers
-
-### Installation
-
-Install from source in editable mode using `pip install -e .` in this directory or `pip install -e path/to/directory` from another directory. 
-
-### Running tests 
-
-To test your installation, run `python -m unittest [test_name].py` from the `subseasonal_data/tests` directory or `python -m unittest path/to/tests/folder/[test_name].py`. Example:
-
-```Python
-python -m unittest subseasonal_data/tests/test_data_loaders.py
-```
-
-### Generating Documentation
-
-This project's documentation is generated via [Sphinx](https://www.sphinx-doc.org/en/master/index.html). The HTML theme used is the [Read the Docs](https://github.com/readthedocs/sphinx_rtd_theme) sphinx theme which also needs to be installed.
-
-To generate a local copy of the documentation from a clone of this repository, run `python setup.py build_sphinx -W -E -a`, which will build the documentation and place it under the `build/sphinx/html` path. 
-
-The reStructuredText files that make up the documentation are stored in the `docs` directory; module documentation is automatically generated by the Sphinx build process.
-
-## Data Usage and Citation
-
-If you make use of the `subseasonal_data` package or the **SubseasonalClimateUSA** dataset, please acknowledge the Python package, the individual data sources described in [DATA.md](https://github.com/microsoft/subseasonal_data/blob/main/DATA.md), and the associated **SubseasonalClimateUSA** preprint:
-
-[Learned Benchmarks for Subseasonal Forecasting](https://arxiv.org/pdf/2109.10399.pdf)  
-Soukayna Mouatadid, Paulo Orenstein, Genevieve Flaspohler, Miruna Oprescu, Judah Cohen, Franklyn Wang, Sean Knight, Maria Geogdzhayeva, Sam Levang, Ernest Fraenkel, and Lester Mackey.  Sep. 2021.
-
-```
-@article{
-  mouatadid2021toolkit,
-  title={Learned Benchmarks for Subseasonal Forecasting},
-  author={Soukayna Mouatadid, Paulo Orenstein, Genevieve Flaspohler, Miruna Oprescu, Judah Cohen, Franklyn Wang, Sean Knight, Maria Geogdzhayeva, Sam Levang, Ernest Fraenkel, and Lester Mackey},
-  journal={arXiv preprint arXiv:2109.10399},
-  year={2021}
-}
-```
-
-## Contributing
-
-This project welcomes contributions and suggestions.  Most contributions require you to agree to a
-Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
-the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.
-
-When you submit a pull request, a CLA bot will automatically determine whether you need to provide
-a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
-provided by the bot. You will only need to do this once across all repos using our CLA.
-
-This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
-For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
-contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
-
-## Trademarks
-
-This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft 
-trademarks or logos is subject to and must follow 
-[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
-Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
-Any use of third-party trademarks or logos are subject to those third-party's policies.
+# Subseasonal Data Python Package
+
+The `subseasonal_data` package provides an API for loading and manipulating the **SubseasonalClimateUSA** dataset developed for training and benchmarking subseasonal forecasting models.  Here, _subseasonal_ refers to climate and weather forecasts made 2-6 weeks in advance.  See [DATA.md](https://github.com/microsoft/subseasonal_data/blob/main/DATA.md) for a description of dataset contents, sources, and processing.
+
+## Getting Started
+
+- Install the subseasonal data package: `pip install subseasonal-data`
+- Define the environment variable `$SUBSEASONALDATA_PATH` to point to your desired data directory; any accessed data files will be read from, saved to, or synced with this directory
+
+ This package is compatible with Python version 3.6+. 
+ 
+ The underlying data is made available through Azure and is updated periodically. To download the data through this package, you will need to have the Azure Storage CLI [`azcopy`](https://docs.microsoft.com/en-us/azure/storage/common/storage-use-azcopy) installed on your machine.
+
+## Usage Examples
+
+Detailed usage examples are provided in the `Getting Started` and `Examples` notebooks in the `examples` folder. It is recommended you start there.
+
+Quick examples:
+
+* Download all data
+
+**WARNING:** This requires an estimated 175GB disk space.
+
+```Python
+from subseasonal_data import downloader
+
+downloader.download()
+```
+
+* List files in a data directory
+
+```Python
+downloader.list_subdir_files(data_subdir="combined_dataframes")
+```
+
+* Download one data file
+
+```Python
+downloader.download_file(
+    data_subdir="combined_dataframes", 
+    filename="all_data-us_precip_34w.feather", 
+    verbose=True)
+```
+
+* Load ground truth data
+
+```Python
+from subseasonal_data import data_loaders
+
+# Loads into a Pandas dataframe
+df = data_loaders.get_ground_truth("us_precip")
+```
+
+* Load combined dataframes
+
+```Python
+data_loaders.load_combined_data("all_data", "us_tmp2m", "34w")
+```
+
+See the [Examples.ipynb](https://github.com/microsoft/subseasonal_data/blob/main/examples/Examples.ipynb) notebook for an example on how to retrieve historical temperature data using the `subseasonal_data` package. 
+
+![Usage Example](https://github.com/microsoft/subseasonal_data/blob/main/usage_example.gif)
+
+## For Developers
+
+### Installation
+
+Install from source in editable mode using `pip install -e .` in this directory or `pip install -e path/to/directory` from another directory. 
+
+### Running tests 
+
+To test your installation, run `python -m unittest [test_name].py` from the `subseasonal_data/tests` directory or `python -m unittest path/to/tests/folder/[test_name].py`. Example:
+
+```Python
+python -m unittest subseasonal_data/tests/test_data_loaders.py
+```
+
+### Generating Documentation
+
+This project's documentation is generated via [Sphinx](https://www.sphinx-doc.org/en/master/index.html). The HTML theme used is the [Read the Docs](https://github.com/readthedocs/sphinx_rtd_theme) sphinx theme which also needs to be installed.
+
+To generate a local copy of the documentation from a clone of this repository, run `python setup.py build_sphinx -W -E -a`, which will build the documentation and place it under the `build/sphinx/html` path. 
+
+The reStructuredText files that make up the documentation are stored in the `docs` directory; module documentation is automatically generated by the Sphinx build process.
+
+## Data Usage and Citation
+
+The **SubseasonalClimateUSA** dataset is released under a [CC BY 4.0 license](https://creativecommons.org/licenses/by/4.0/), and the `subseasonal_data` repository code is released under an [MIT license](https://github.com/microsoft/subseasonal_data/blob/main/LICENSE).
+
+If you make use of the `subseasonal_data` package or the **SubseasonalClimateUSA** dataset, please acknowledge the Python package, the individual data sources described in [DATA.md](https://github.com/microsoft/subseasonal_data/blob/main/DATA.md), and the associated **SubseasonalClimateUSA** preprint:
+
+[**SubseasonalClimateUSA**: A Dataset for Subseasonal Forecasting and Benchmarking](https://arxiv.org/pdf/2109.10399.pdf)  
+Soukayna Mouatadid, Paulo Orenstein, Genevieve Flaspohler, Miruna Oprescu, Judah Cohen, Franklyn Wang, Sean Knight, Maria Geogdzhayeva, Sam Levang, Ernest Fraenkel, and Lester Mackey.  Sep. 2021.
+
+```
+@article{
+  mouatadid2021subseasonal,
+  title={SubseasonalClimateUSA: A Dataset for Subseasonal Forecasting and Benchmarking},
+  author={Soukayna Mouatadid, Paulo Orenstein, Genevieve Flaspohler, Miruna Oprescu, Judah Cohen, Franklyn Wang, Sean Knight, Maria Geogdzhayeva, Sam Levang, Ernest Fraenkel, and Lester Mackey},
+  journal={arXiv preprint arXiv:2109.10399},
+  year={2021}
+}
+```
+
+## Contributing
+
+This project welcomes contributions and suggestions.  Most contributions require you to agree to a
+Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
+the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.
+
+When you submit a pull request, a CLA bot will automatically determine whether you need to provide
+a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
+provided by the bot. You will only need to do this once across all repos using our CLA.
+
+This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
+For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
+contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
+
+## Trademarks
+
+This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft 
+trademarks or logos is subject to and must follow 
+[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
+Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
+Any use of third-party trademarks or logos are subject to those third-party's policies.
```

### Comparing `subseasonal_data-0.0.6/subseasonal_data/data_loaders.py` & `subseasonal_data-0.0.7/subseasonal_data/data_loaders.py`

 * *Files identical despite different names*

### Comparing `subseasonal_data-0.0.6/subseasonal_data/downloader.py` & `subseasonal_data-0.0.7/subseasonal_data/downloader.py`

 * *Files identical despite different names*

### Comparing `subseasonal_data-0.0.6/subseasonal_data/utils.py` & `subseasonal_data-0.0.7/subseasonal_data/utils.py`

 * *Files identical despite different names*

### Comparing `subseasonal_data-0.0.6/subseasonal_data.egg-info/PKG-INFO` & `subseasonal_data-0.0.7/subseasonal_data.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subseasonal-data
-Version: 0.0.6
+Version: 0.0.7
 Summary: Data access package for the SubseasonalClimateUSA dataset.
 Home-page: https://github.com/microsoft/subseasonal_data
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -91,23 +91,25 @@
 
 To generate a local copy of the documentation from a clone of this repository, run `python setup.py build_sphinx -W -E -a`, which will build the documentation and place it under the `build/sphinx/html` path. 
 
 The reStructuredText files that make up the documentation are stored in the `docs` directory; module documentation is automatically generated by the Sphinx build process.
 
 ## Data Usage and Citation
 
+The **SubseasonalClimateUSA** dataset is released under a [CC BY 4.0 license](https://creativecommons.org/licenses/by/4.0/), and the `subseasonal_data` repository code is released under an [MIT license](https://github.com/microsoft/subseasonal_data/blob/main/LICENSE).
+
 If you make use of the `subseasonal_data` package or the **SubseasonalClimateUSA** dataset, please acknowledge the Python package, the individual data sources described in [DATA.md](https://github.com/microsoft/subseasonal_data/blob/main/DATA.md), and the associated **SubseasonalClimateUSA** preprint:
 
-[Learned Benchmarks for Subseasonal Forecasting](https://arxiv.org/pdf/2109.10399.pdf)  
+[**SubseasonalClimateUSA**: A Dataset for Subseasonal Forecasting and Benchmarking](https://arxiv.org/pdf/2109.10399.pdf)  
 Soukayna Mouatadid, Paulo Orenstein, Genevieve Flaspohler, Miruna Oprescu, Judah Cohen, Franklyn Wang, Sean Knight, Maria Geogdzhayeva, Sam Levang, Ernest Fraenkel, and Lester Mackey.  Sep. 2021.
 
 ```
 @article{
-  mouatadid2021toolkit,
-  title={Learned Benchmarks for Subseasonal Forecasting},
+  mouatadid2021subseasonal,
+  title={SubseasonalClimateUSA: A Dataset for Subseasonal Forecasting and Benchmarking},
   author={Soukayna Mouatadid, Paulo Orenstein, Genevieve Flaspohler, Miruna Oprescu, Judah Cohen, Franklyn Wang, Sean Knight, Maria Geogdzhayeva, Sam Levang, Ernest Fraenkel, and Lester Mackey},
   journal={arXiv preprint arXiv:2109.10399},
   year={2021}
 }
 ```
 
 ## Contributing
@@ -128,7 +130,8 @@
 
 This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft 
 trademarks or logos is subject to and must follow 
 [Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
 Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
 Any use of third-party trademarks or logos are subject to those third-party's policies.
 
+
```

