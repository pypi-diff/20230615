# Comparing `tmp/pdf_language_detector-0.0.1.tar.gz` & `tmp/pdf_language_detector-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_language_detector-0.0.1.tar", max compression
+gzip compressed data, was "pdf_language_detector-0.0.2.tar", max compression
```

## Comparing `pdf_language_detector-0.0.1.tar` & `pdf_language_detector-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1787 2023-06-14 22:48:49.605840 pdf_language_detector-0.0.1/README.md
--rw-r--r--   0        0        0      744 2023-06-14 22:49:18.693924 pdf_language_detector-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       24 2023-06-14 22:13:51.629533 pdf_language_detector-0.0.1/src/__init__.py
--rw-r--r--   0        0        0      790 2023-06-14 22:36:14.330867 pdf_language_detector-0.0.1/src/cli.py
--rw-r--r--   0        0        0     8310 2023-06-14 22:12:41.467946 pdf_language_detector-0.0.1/src/pld.py
--rw-r--r--   0        0        0     2875 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.1/setup.py
--rw-r--r--   0        0        0     2564 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2192 2023-06-15 08:03:51.498582 pdf_language_detector-0.0.2/README.md
+-rw-r--r--   0        0        0      744 2023-06-15 08:04:18.858784 pdf_language_detector-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-06-14 22:13:51.629533 pdf_language_detector-0.0.2/src/__init__.py
+-rw-r--r--   0        0        0      790 2023-06-14 22:36:14.330867 pdf_language_detector-0.0.2/src/cli.py
+-rw-r--r--   0        0        0     8310 2023-06-14 22:12:41.467946 pdf_language_detector-0.0.2/src/pld.py
+-rw-r--r--   0        0        0     3307 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.2/setup.py
+-rw-r--r--   0        0        0     2969 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.2/PKG-INFO
```

### Comparing `pdf_language_detector-0.0.1/README.md` & `pdf_language_detector-0.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # PLD (PDF Language Detector)
 
 PLD is a Python program that analyzes PDF files, extracts images, processes them using Optical Character Recognition (OCR), and detects the dominant language of the text. It provides language detection information in JSON format and calculates the average confidence coefficient for each language.
 
 ## Requirements
 
-- Python 3.8 or above
-- Tesseract OCR
-- pdftoppm
+- [Python 3.8](https://www.python.org/downloads/) or above
+- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)
+- [pdftoppm](https://poppler.freedesktop.org/)
 
 ## Installation
 
 Install Tesseract OCR and pdftoppm using your package manager. For example, on Ubuntu:
 
 ```bash
 sudo apt install tesseract-ocr tesseract-ocr-all poppler-utils
@@ -20,34 +20,61 @@
 
 Install with pip:
 
 ```bash
 python3 -m pip install --user pdf-language-detector
 ```
 
+Then run directly from your terminal:
+
+```bash
+pld --help
+````
+
 ### From the sources
 
 Clone the PLD repository:
 
 ```bash
 git clone git@github.com:github.com/icij/pld.git
 ```
 
 Install the required Python packages with poetry:
 
 ```bash
 poetry install
 ````
 
+Then run inside a virtual env managed by poetry:
+
+```bash
+poetry run pld --help
+````
+
+### From Docker
+
+Install with Docker:
+
+```bash
+docker pull icij/pld
+```
+
+Then run inside a container:
+
+```bash
+docker run -it icij/pld pld --help
+```
+
+
 ## Usage
 
 ```bash
 pld --help
 
-    --language A comma-separated list of ISO3 language codes to detect.
+    --language A list of ISO3 language codes to detect.
     --input-dir: Path to the input directory containing PDF files. Default is the current directory.
     --output-dir (optional): Path to the output directory. Default is 'out' directory in the current directory.
     --max-pages (optional): Maximum number of pages to process per PDF file. Default is 5.
 ```
 
 ## Examples
```

### Comparing `pdf_language_detector-0.0.1/pyproject.toml` & `pdf_language_detector-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdf-language-detector"
-version = "0.0.1"
+version = "0.0.2"
 description = "A python script to iterate over a list of PDF in a directory and try to guess their language with Tesseract OCR."
 authors = ["ICIJ <engineering@icij.org>"]
 readme = "README.md"
 packages = [{include = "src"}]
 
 [tool.poetry.dependencies]
 python = '^3.8.1'
```

### Comparing `pdf_language_detector-0.0.1/src/cli.py` & `pdf_language_detector-0.0.2/src/cli.py`

 * *Files identical despite different names*

### Comparing `pdf_language_detector-0.0.1/src/pld.py` & `pdf_language_detector-0.0.2/src/pld.py`

 * *Files identical despite different names*

### Comparing `pdf_language_detector-0.0.1/setup.py` & `pdf_language_detector-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 
 entry_points = \
 {'console_scripts': ['pdf-language-detector = src.cli:app',
                      'pld = src.cli:app']}
 
 setup_kwargs = {
     'name': 'pdf-language-detector',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'A python script to iterate over a list of PDF in a directory and try to guess their language with Tesseract OCR.',
-    'long_description': "# PLD (PDF Language Detector)\n\nPLD is a Python program that analyzes PDF files, extracts images, processes them using Optical Character Recognition (OCR), and detects the dominant language of the text. It provides language detection information in JSON format and calculates the average confidence coefficient for each language.\n\n## Requirements\n\n- Python 3.8 or above\n- Tesseract OCR\n- pdftoppm\n\n## Installation\n\nInstall Tesseract OCR and pdftoppm using your package manager. For example, on Ubuntu:\n\n```bash\nsudo apt install tesseract-ocr tesseract-ocr-all poppler-utils\n```\n\n### From PyPi\n\nInstall with pip:\n\n```bash\npython3 -m pip install --user pdf-language-detector\n```\n\n### From the sources\n\nClone the PLD repository:\n\n```bash\ngit clone git@github.com:github.com/icij/pld.git\n```\n\nInstall the required Python packages with poetry:\n\n```bash\npoetry install\n````\n\n## Usage\n\n```bash\npld --help\n\n    --language A comma-separated list of ISO3 language codes to detect.\n    --input-dir: Path to the input directory containing PDF files. Default is the current directory.\n    --output-dir (optional): Path to the output directory. Default is 'out' directory in the current directory.\n    --max-pages (optional): Maximum number of pages to process per PDF file. Default is 5.\n```\n\n## Examples\n\nProcess PDF files in the current directory, detect English and Spanish languages, and save the results in the 'results' directory:\n\n```bash\npld --language eng --language spa --input-dir documents --output-dir results\n```\n\nProcess PDF files in the 'documents' directory, detect French and Greek languages, and limit the processing to 3 pages per file:\n\n```bash\npld --language fra --language ell --input-dir documents --max-pages 3\n```\n\n## License\n\nThis project is licensed under the MIT License.\n",
+    'long_description': "# PLD (PDF Language Detector)\n\nPLD is a Python program that analyzes PDF files, extracts images, processes them using Optical Character Recognition (OCR), and detects the dominant language of the text. It provides language detection information in JSON format and calculates the average confidence coefficient for each language.\n\n## Requirements\n\n- [Python 3.8](https://www.python.org/downloads/) or above\n- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)\n- [pdftoppm](https://poppler.freedesktop.org/)\n\n## Installation\n\nInstall Tesseract OCR and pdftoppm using your package manager. For example, on Ubuntu:\n\n```bash\nsudo apt install tesseract-ocr tesseract-ocr-all poppler-utils\n```\n\n### From PyPi\n\nInstall with pip:\n\n```bash\npython3 -m pip install --user pdf-language-detector\n```\n\nThen run directly from your terminal:\n\n```bash\npld --help\n````\n\n### From the sources\n\nClone the PLD repository:\n\n```bash\ngit clone git@github.com:github.com/icij/pld.git\n```\n\nInstall the required Python packages with poetry:\n\n```bash\npoetry install\n````\n\nThen run inside a virtual env managed by poetry:\n\n```bash\npoetry run pld --help\n````\n\n### From Docker\n\nInstall with Docker:\n\n```bash\ndocker pull icij/pld\n```\n\nThen run inside a container:\n\n```bash\ndocker run -it icij/pld pld --help\n```\n\n\n## Usage\n\n```bash\npld --help\n\n    --language A list of ISO3 language codes to detect.\n    --input-dir: Path to the input directory containing PDF files. Default is the current directory.\n    --output-dir (optional): Path to the output directory. Default is 'out' directory in the current directory.\n    --max-pages (optional): Maximum number of pages to process per PDF file. Default is 5.\n```\n\n## Examples\n\nProcess PDF files in the current directory, detect English and Spanish languages, and save the results in the 'results' directory:\n\n```bash\npld --language eng --language spa --input-dir documents --output-dir results\n```\n\nProcess PDF files in the 'documents' directory, detect French and Greek languages, and limit the processing to 3 pages per file:\n\n```bash\npld --language fra --language ell --input-dir documents --max-pages 3\n```\n\n## License\n\nThis project is licensed under the MIT License.\n",
     'author': 'ICIJ',
     'author_email': 'engineering@icij.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pdf_language_detector-0.0.1/PKG-INFO` & `pdf_language_detector-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf-language-detector
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python script to iterate over a list of PDF in a directory and try to guess their language with Tesseract OCR.
 Author: ICIJ
 Author-email: engineering@icij.org
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -19,17 +19,17 @@
 
 # PLD (PDF Language Detector)
 
 PLD is a Python program that analyzes PDF files, extracts images, processes them using Optical Character Recognition (OCR), and detects the dominant language of the text. It provides language detection information in JSON format and calculates the average confidence coefficient for each language.
 
 ## Requirements
 
-- Python 3.8 or above
-- Tesseract OCR
-- pdftoppm
+- [Python 3.8](https://www.python.org/downloads/) or above
+- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)
+- [pdftoppm](https://poppler.freedesktop.org/)
 
 ## Installation
 
 Install Tesseract OCR and pdftoppm using your package manager. For example, on Ubuntu:
 
 ```bash
 sudo apt install tesseract-ocr tesseract-ocr-all poppler-utils
@@ -39,34 +39,61 @@
 
 Install with pip:
 
 ```bash
 python3 -m pip install --user pdf-language-detector
 ```
 
+Then run directly from your terminal:
+
+```bash
+pld --help
+````
+
 ### From the sources
 
 Clone the PLD repository:
 
 ```bash
 git clone git@github.com:github.com/icij/pld.git
 ```
 
 Install the required Python packages with poetry:
 
 ```bash
 poetry install
 ````
 
+Then run inside a virtual env managed by poetry:
+
+```bash
+poetry run pld --help
+````
+
+### From Docker
+
+Install with Docker:
+
+```bash
+docker pull icij/pld
+```
+
+Then run inside a container:
+
+```bash
+docker run -it icij/pld pld --help
+```
+
+
 ## Usage
 
 ```bash
 pld --help
 
-    --language A comma-separated list of ISO3 language codes to detect.
+    --language A list of ISO3 language codes to detect.
     --input-dir: Path to the input directory containing PDF files. Default is the current directory.
     --output-dir (optional): Path to the output directory. Default is 'out' directory in the current directory.
     --max-pages (optional): Maximum number of pages to process per PDF file. Default is 5.
 ```
 
 ## Examples
```

