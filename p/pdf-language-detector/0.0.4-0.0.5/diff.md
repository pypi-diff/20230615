# Comparing `tmp/pdf_language_detector-0.0.4.tar.gz` & `tmp/pdf_language_detector-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_language_detector-0.0.4.tar", max compression
+gzip compressed data, was "pdf_language_detector-0.0.5.tar", max compression
```

## Comparing `pdf_language_detector-0.0.4.tar` & `pdf_language_detector-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2707 2023-06-15 13:51:48.211566 pdf_language_detector-0.0.4/README.md
--rw-r--r--   0        0        0      744 2023-06-15 13:58:09.402339 pdf_language_detector-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       24 2023-06-14 22:13:51.629533 pdf_language_detector-0.0.4/src/__init__.py
--rw-r--r--   0        0        0     1350 2023-06-15 13:51:45.811549 pdf_language_detector-0.0.4/src/cli.py
--rw-r--r--   0        0        0     9711 2023-06-15 13:56:12.913500 pdf_language_detector-0.0.4/src/pld.py
--rw-r--r--   0        0        0     3734 2023-06-15 13:44:40.224290 pdf_language_detector-0.0.4/src/report.py
--rw-r--r--   0        0        0     3839 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.4/setup.py
--rw-r--r--   0        0        0     3484 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2707 2023-06-15 13:51:48.211566 pdf_language_detector-0.0.5/README.md
+-rw-r--r--   0        0        0      744 2023-06-15 14:20:02.493305 pdf_language_detector-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-06-14 22:13:51.629533 pdf_language_detector-0.0.5/src/__init__.py
+-rw-r--r--   0        0        0     1350 2023-06-15 13:51:45.811549 pdf_language_detector-0.0.5/src/cli.py
+-rw-r--r--   0        0        0     9683 2023-06-15 14:19:31.817070 pdf_language_detector-0.0.5/src/pld.py
+-rw-r--r--   0        0        0     3734 2023-06-15 13:44:40.224290 pdf_language_detector-0.0.5/src/report.py
+-rw-r--r--   0        0        0     3839 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.5/setup.py
+-rw-r--r--   0        0        0     3484 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.5/PKG-INFO
```

### Comparing `pdf_language_detector-0.0.4/README.md` & `pdf_language_detector-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pdf_language_detector-0.0.4/pyproject.toml` & `pdf_language_detector-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdf-language-detector"
-version = "0.0.4"
+version = "0.0.5"
 description = "A python script to iterate over a list of PDF in a directory and try to guess their language with Tesseract OCR."
 authors = ["ICIJ <engineering@icij.org>"]
 readme = "README.md"
 packages = [{include = "src"}]
 
 [tool.poetry.dependencies]
 python = '^3.8.1'
```

### Comparing `pdf_language_detector-0.0.4/src/cli.py` & `pdf_language_detector-0.0.5/src/cli.py`

 * *Files identical despite different names*

### Comparing `pdf_language_detector-0.0.4/src/pld.py` & `pdf_language_detector-0.0.5/src/pld.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
             f.write(json.dumps(coeff_avgs, indent=2))
         return max(coeff_avgs, key=coeff_avgs.get)
 
     def process_input_files(self):
         """
         Process all the PDF files in the input directory.
         """
-        for input_file in sorted(self.input_dir.glob('**/*.pdf')):                    
+        for input_file in self.input_dir.glob('**/*.pdf'):
             with Progress(SpinnerColumn(), "[progress.description]{task.description}", transient=True) as progress:
                 progress.add_task(input_file.resolve(), total=None)
                 output_file_dir = self.get_output_dir(input_file)
                 try:
                     if self.resume and self.is_already_analyzed(output_file_dir):
                         print(f"→ {input_file.resolve()} [blue]SKIPPED[/blue]")
                     else:
```

### Comparing `pdf_language_detector-0.0.4/src/report.py` & `pdf_language_detector-0.0.5/src/report.py`

 * *Files identical despite different names*

### Comparing `pdf_language_detector-0.0.4/setup.py` & `pdf_language_detector-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 entry_points = \
 {'console_scripts': ['pdf-language-detector = src.cli:app',
                      'pld = src.cli:app']}
 
 setup_kwargs = {
     'name': 'pdf-language-detector',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'A python script to iterate over a list of PDF in a directory and try to guess their language with Tesseract OCR.',
     'long_description': "# PLD (PDF Language Detector)\n\nPLD is a Python program that analyzes PDF files, extracts images, processes them using Optical Character Recognition (OCR), and detects the dominant language of the text. It provides language detection information in JSON format and calculates the average confidence coefficient for each language.\n\n## Requirements\n\n- [Python 3.8](https://www.python.org/downloads/) or above\n- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)\n- [pdftoppm](https://poppler.freedesktop.org/)\n\n## Installation\n\nInstall Tesseract OCR and pdftoppm using your package manager. For example, on Ubuntu:\n\n```bash\nsudo apt install tesseract-ocr tesseract-ocr-all poppler-utils\n```\n\n### From PyPi\n\nInstall with pip:\n\n```bash\npython3 -m pip install --user pdf-language-detector\n```\n\nThen run directly from your terminal:\n\n```bash\npld --help\n````\n\n### From the sources\n\nClone the PLD repository:\n\n```bash\ngit clone git@github.com:github.com/icij/pld.git\n```\n\nInstall the required Python packages with poetry:\n\n```bash\npoetry install\n````\n\nThen run inside a virtual env managed by poetry:\n\n```bash\npoetry run pld --help\n````\n\n### From Docker\n\nInstall with Docker:\n\n```bash\ndocker pull icij/pld\n```\n\nThen run inside a container:\n\n```bash\ndocker run -it icij/pld pld --help\n```\n\n\n## Usage\n\n### Detect\n\nThis command process PDF files and detect the dominant language.\n\n```\npld detect --help\n\n    --language A list of ISO3 language codes to detect.\n    --input-dir: Path to the input directory containing PDF files. Default is the current directory.\n    --output-dir (optional): Path to the output directory. Default is 'out' directory in the current directory.\n    --max-pages (optional): Maximum number of pages to process per PDF file. Default is 5.\n    --resume (optional): Skip PDF files already analyzed.\n    --skip-images (optional): Skip the extraction of PDF files a images.\n    --skip-ocr (optional): Skip the OCR of images from PDF files.\n```\n\n### Report\n\nThis command print a report from the previously detected language (using the same output dir).\n\n```\npld report --help\n\n    --output-dir: Path to the output directory. Default is 'out' directory in the current directory.\n```\n\n## Examples\n\nProcess PDF files in the current directory, detect English and Spanish languages, and save the results in the 'results' directory:\n\n```bash\npld --language eng --language spa --input-dir documents --output-dir results\n```\n\nProcess PDF files in the 'documents' directory, detect French and Greek languages, and limit the processing to 3 pages per file:\n\n```bash\npld --language fra --language ell --input-dir documents --max-pages 3\n```\n\n## License\n\nThis project is licensed under the MIT License.\n",
     'author': 'ICIJ',
     'author_email': 'engineering@icij.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pdf_language_detector-0.0.4/PKG-INFO` & `pdf_language_detector-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf-language-detector
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python script to iterate over a list of PDF in a directory and try to guess their language with Tesseract OCR.
 Author: ICIJ
 Author-email: engineering@icij.org
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

