# Comparing `tmp/pdf_language_detector-0.0.2.tar.gz` & `tmp/pdf_language_detector-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_language_detector-0.0.2.tar", max compression
+gzip compressed data, was "pdf_language_detector-0.0.3.tar", max compression
```

## Comparing `pdf_language_detector-0.0.2.tar` & `pdf_language_detector-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2192 2023-06-15 08:03:51.498582 pdf_language_detector-0.0.2/README.md
--rw-r--r--   0        0        0      744 2023-06-15 08:04:18.858784 pdf_language_detector-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       24 2023-06-14 22:13:51.629533 pdf_language_detector-0.0.2/src/__init__.py
--rw-r--r--   0        0        0      790 2023-06-14 22:36:14.330867 pdf_language_detector-0.0.2/src/cli.py
--rw-r--r--   0        0        0     8310 2023-06-14 22:12:41.467946 pdf_language_detector-0.0.2/src/pld.py
--rw-r--r--   0        0        0     3307 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.2/setup.py
--rw-r--r--   0        0        0     2969 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2327 2023-06-15 10:32:33.053853 pdf_language_detector-0.0.3/README.md
+-rw-r--r--   0        0        0      744 2023-06-15 10:32:57.470057 pdf_language_detector-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-06-14 22:13:51.629533 pdf_language_detector-0.0.3/src/__init__.py
+-rw-r--r--   0        0        0     1031 2023-06-15 10:22:30.384584 pdf_language_detector-0.0.3/src/cli.py
+-rw-r--r--   0        0        0     8688 2023-06-15 10:28:42.755903 pdf_language_detector-0.0.3/src/pld.py
+-rw-r--r--   0        0        0     3444 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.3/setup.py
+-rw-r--r--   0        0        0     3104 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.3/PKG-INFO
```

### Comparing `pdf_language_detector-0.0.2/README.md` & `pdf_language_detector-0.0.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -63,21 +63,23 @@
 ```bash
 docker run -it icij/pld pld --help
 ```
 
 
 ## Usage
 
-```bash
+```
 pld --help
 
     --language A list of ISO3 language codes to detect.
     --input-dir: Path to the input directory containing PDF files. Default is the current directory.
     --output-dir (optional): Path to the output directory. Default is 'out' directory in the current directory.
     --max-pages (optional): Maximum number of pages to process per PDF file. Default is 5.
+    --skip-images (optional): Skip the extraction of PDF files a images.
+    --skip-ocr (optional): Skip the OCR of images from PDF files.
 ```
 
 ## Examples
 
 Process PDF files in the current directory, detect English and Spanish languages, and save the results in the 'results' directory:
 
 ```bash
```

### Comparing `pdf_language_detector-0.0.2/pyproject.toml` & `pdf_language_detector-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdf-language-detector"
-version = "0.0.2"
+version = "0.0.3"
 description = "A python script to iterate over a list of PDF in a directory and try to guess their language with Tesseract OCR."
 authors = ["ICIJ <engineering@icij.org>"]
 readme = "README.md"
 packages = [{include = "src"}]
 
 [tool.poetry.dependencies]
 python = '^3.8.1'
```

### Comparing `pdf_language_detector-0.0.2/src/pld.py` & `pdf_language_detector-0.0.3/src/pld.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,29 +11,35 @@
 from typing import Optional, List
 
 class PdfLanguageDetector:
     def __init__(self, 
                 languages: List[str], 
                 input_dir: Path = Path(),
                 output_dir: Optional[Path] = 'out',
-                max_pages: Optional[int] = 5):
+                max_pages: Optional[int] = 5,
+                skip_images:  Optional[bool] = False,
+                skip_ocr:  Optional[bool] = False):
         """
         Initialize the PdfLanguageDetector class.
 
         Args:
             languages: List of ISO3 language codes.
             input_dir: Path to the input directory.
             output_dir: Path to the output directory.
             max_pages: Maximum number of pages to process per PDF file.
+            skip_images: Skip the extraction of PDF files as images.
+            skip_ocr: Skip the OCR of images from PDF files.
         """
         self.languages = [Language.get(language) for language in languages]
         self.lang_detector = LanguageDetectorBuilder.from_iso_codes_639_3(*self.lingua_langs).build()
         self.input_dir = input_dir
         self.output_dir = output_dir
         self.max_pages = max_pages
+        self.skip_images = skip_images
+        self.skip_ocr = skip_ocr
 
     def create_output_directories(self, *dirs: Path):
         """
         Create output directories if they don't exist.
 
         Args:
             *dirs: Variable number of directory paths to create.
@@ -163,16 +169,18 @@
         Returns:
             The language with the highest average coefficient.
         """
         images_dir = output_file_dir / 'images'
         texts_dir = output_file_dir / 'texts'
         langs_dir = output_file_dir / 'langs'
         self.create_output_directories(images_dir, texts_dir, langs_dir)
-        self.extract_images(input_file, images_dir)
-        self.process_images(images_dir, texts_dir, langs_dir)
+        if not self.skip_images:
+            self.extract_images(input_file, images_dir)
+        if not self.skip_ocr:
+            self.process_images(images_dir, texts_dir, langs_dir)
         coeff_avgs = self.calculate_coeff_avgs(langs_dir)
         coeff_avgs_file = output_file_dir.resolve() / 'avgs.json'
         with coeff_avgs_file.open("w") as f:
             f.write(json.dumps(coeff_avgs, indent=2))
         return max(coeff_avgs, key=coeff_avgs.get)
 
     def process_input_files(self):
```

### Comparing `pdf_language_detector-0.0.2/setup.py` & `pdf_language_detector-0.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 
 entry_points = \
 {'console_scripts': ['pdf-language-detector = src.cli:app',
                      'pld = src.cli:app']}
 
 setup_kwargs = {
     'name': 'pdf-language-detector',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'A python script to iterate over a list of PDF in a directory and try to guess their language with Tesseract OCR.',
-    'long_description': "# PLD (PDF Language Detector)\n\nPLD is a Python program that analyzes PDF files, extracts images, processes them using Optical Character Recognition (OCR), and detects the dominant language of the text. It provides language detection information in JSON format and calculates the average confidence coefficient for each language.\n\n## Requirements\n\n- [Python 3.8](https://www.python.org/downloads/) or above\n- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)\n- [pdftoppm](https://poppler.freedesktop.org/)\n\n## Installation\n\nInstall Tesseract OCR and pdftoppm using your package manager. For example, on Ubuntu:\n\n```bash\nsudo apt install tesseract-ocr tesseract-ocr-all poppler-utils\n```\n\n### From PyPi\n\nInstall with pip:\n\n```bash\npython3 -m pip install --user pdf-language-detector\n```\n\nThen run directly from your terminal:\n\n```bash\npld --help\n````\n\n### From the sources\n\nClone the PLD repository:\n\n```bash\ngit clone git@github.com:github.com/icij/pld.git\n```\n\nInstall the required Python packages with poetry:\n\n```bash\npoetry install\n````\n\nThen run inside a virtual env managed by poetry:\n\n```bash\npoetry run pld --help\n````\n\n### From Docker\n\nInstall with Docker:\n\n```bash\ndocker pull icij/pld\n```\n\nThen run inside a container:\n\n```bash\ndocker run -it icij/pld pld --help\n```\n\n\n## Usage\n\n```bash\npld --help\n\n    --language A list of ISO3 language codes to detect.\n    --input-dir: Path to the input directory containing PDF files. Default is the current directory.\n    --output-dir (optional): Path to the output directory. Default is 'out' directory in the current directory.\n    --max-pages (optional): Maximum number of pages to process per PDF file. Default is 5.\n```\n\n## Examples\n\nProcess PDF files in the current directory, detect English and Spanish languages, and save the results in the 'results' directory:\n\n```bash\npld --language eng --language spa --input-dir documents --output-dir results\n```\n\nProcess PDF files in the 'documents' directory, detect French and Greek languages, and limit the processing to 3 pages per file:\n\n```bash\npld --language fra --language ell --input-dir documents --max-pages 3\n```\n\n## License\n\nThis project is licensed under the MIT License.\n",
+    'long_description': "# PLD (PDF Language Detector)\n\nPLD is a Python program that analyzes PDF files, extracts images, processes them using Optical Character Recognition (OCR), and detects the dominant language of the text. It provides language detection information in JSON format and calculates the average confidence coefficient for each language.\n\n## Requirements\n\n- [Python 3.8](https://www.python.org/downloads/) or above\n- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)\n- [pdftoppm](https://poppler.freedesktop.org/)\n\n## Installation\n\nInstall Tesseract OCR and pdftoppm using your package manager. For example, on Ubuntu:\n\n```bash\nsudo apt install tesseract-ocr tesseract-ocr-all poppler-utils\n```\n\n### From PyPi\n\nInstall with pip:\n\n```bash\npython3 -m pip install --user pdf-language-detector\n```\n\nThen run directly from your terminal:\n\n```bash\npld --help\n````\n\n### From the sources\n\nClone the PLD repository:\n\n```bash\ngit clone git@github.com:github.com/icij/pld.git\n```\n\nInstall the required Python packages with poetry:\n\n```bash\npoetry install\n````\n\nThen run inside a virtual env managed by poetry:\n\n```bash\npoetry run pld --help\n````\n\n### From Docker\n\nInstall with Docker:\n\n```bash\ndocker pull icij/pld\n```\n\nThen run inside a container:\n\n```bash\ndocker run -it icij/pld pld --help\n```\n\n\n## Usage\n\n```\npld --help\n\n    --language A list of ISO3 language codes to detect.\n    --input-dir: Path to the input directory containing PDF files. Default is the current directory.\n    --output-dir (optional): Path to the output directory. Default is 'out' directory in the current directory.\n    --max-pages (optional): Maximum number of pages to process per PDF file. Default is 5.\n    --skip-images (optional): Skip the extraction of PDF files a images.\n    --skip-ocr (optional): Skip the OCR of images from PDF files.\n```\n\n## Examples\n\nProcess PDF files in the current directory, detect English and Spanish languages, and save the results in the 'results' directory:\n\n```bash\npld --language eng --language spa --input-dir documents --output-dir results\n```\n\nProcess PDF files in the 'documents' directory, detect French and Greek languages, and limit the processing to 3 pages per file:\n\n```bash\npld --language fra --language ell --input-dir documents --max-pages 3\n```\n\n## License\n\nThis project is licensed under the MIT License.\n",
     'author': 'ICIJ',
     'author_email': 'engineering@icij.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pdf_language_detector-0.0.2/PKG-INFO` & `pdf_language_detector-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf-language-detector
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python script to iterate over a list of PDF in a directory and try to guess their language with Tesseract OCR.
 Author: ICIJ
 Author-email: engineering@icij.org
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -82,21 +82,23 @@
 ```bash
 docker run -it icij/pld pld --help
 ```
 
 
 ## Usage
 
-```bash
+```
 pld --help
 
     --language A list of ISO3 language codes to detect.
     --input-dir: Path to the input directory containing PDF files. Default is the current directory.
     --output-dir (optional): Path to the output directory. Default is 'out' directory in the current directory.
     --max-pages (optional): Maximum number of pages to process per PDF file. Default is 5.
+    --skip-images (optional): Skip the extraction of PDF files a images.
+    --skip-ocr (optional): Skip the OCR of images from PDF files.
 ```
 
 ## Examples
 
 Process PDF files in the current directory, detect English and Spanish languages, and save the results in the 'results' directory:
 
 ```bash
```

