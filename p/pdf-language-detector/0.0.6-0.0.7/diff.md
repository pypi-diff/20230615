# Comparing `tmp/pdf_language_detector-0.0.6.tar.gz` & `tmp/pdf_language_detector-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_language_detector-0.0.6.tar", max compression
+gzip compressed data, was "pdf_language_detector-0.0.7.tar", max compression
```

## Comparing `pdf_language_detector-0.0.6.tar` & `pdf_language_detector-0.0.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2707 2023-06-15 13:51:48.211566 pdf_language_detector-0.0.6/README.md
--rw-r--r--   0        0        0      744 2023-06-15 14:30:22.585957 pdf_language_detector-0.0.6/pyproject.toml
--rw-r--r--   0        0        0       24 2023-06-14 22:13:51.629533 pdf_language_detector-0.0.6/src/__init__.py
--rw-r--r--   0        0        0     1350 2023-06-15 13:51:45.811549 pdf_language_detector-0.0.6/src/cli.py
--rw-r--r--   0        0        0     9683 2023-06-15 14:19:31.817070 pdf_language_detector-0.0.6/src/pld.py
--rw-r--r--   0        0        0     3735 2023-06-15 14:29:56.113761 pdf_language_detector-0.0.6/src/report.py
--rw-r--r--   0        0        0     3839 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.6/setup.py
--rw-r--r--   0        0        0     3484 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     2772 2023-06-15 18:42:42.158079 pdf_language_detector-0.0.7/README.md
+-rw-r--r--   0        0        0      744 2023-06-15 18:44:06.610843 pdf_language_detector-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-06-14 22:13:51.629533 pdf_language_detector-0.0.7/src/__init__.py
+-rw-r--r--   0        0        0     1466 2023-06-15 15:36:48.029796 pdf_language_detector-0.0.7/src/cli.py
+-rw-r--r--   0        0        0    10085 2023-06-15 18:38:19.863717 pdf_language_detector-0.0.7/src/pld.py
+-rw-r--r--   0        0        0     3735 2023-06-15 14:29:56.113761 pdf_language_detector-0.0.7/src/report.py
+-rw-r--r--   0        0        0     3905 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.7/setup.py
+-rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.7/PKG-INFO
```

### Comparing `pdf_language_detector-0.0.6/README.md` & `pdf_language_detector-0.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     --language A list of ISO3 language codes to detect.
     --input-dir: Path to the input directory containing PDF files. Default is the current directory.
     --output-dir (optional): Path to the output directory. Default is 'out' directory in the current directory.
     --max-pages (optional): Maximum number of pages to process per PDF file. Default is 5.
     --resume (optional): Skip PDF files already analyzed.
     --skip-images (optional): Skip the extraction of PDF files a images.
     --skip-ocr (optional): Skip the OCR of images from PDF files.
+    --parallel (optional): Number of threads to run in parallel.
 ```
 
 ### Report
 
 This command print a report from the previously detected language (using the same output dir).
 
 ```
```

### Comparing `pdf_language_detector-0.0.6/pyproject.toml` & `pdf_language_detector-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdf-language-detector"
-version = "0.0.6"
+version = "0.0.7"
 description = "A python script to iterate over a list of PDF in a directory and try to guess their language with Tesseract OCR."
 authors = ["ICIJ <engineering@icij.org>"]
 readme = "README.md"
 packages = [{include = "src"}]
 
 [tool.poetry.dependencies]
 python = '^3.8.1'
```

### Comparing `pdf_language_detector-0.0.6/src/cli.py` & `pdf_language_detector-0.0.7/src/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 @app.command()
 def detect(languages: List[str] = typer.Option(..., '--language', help="An ISO3 language code."), 
          input_dir: Path  = typer.Option(..., '--input-dir', help="Path to the input directory."),
          output_dir: Optional[Path] = typer.Option('out', help="Path to the output directory."),
          max_pages: Optional[int] = typer.Option(5, help="Maximum number of pages to process per PDF file."),
          resume: Optional[bool] = typer.Option(False, help="Skip PDF files already analyzed."),
          skip_images:  Optional[bool] = typer.Option(False, help="Skip the extraction of PDF files as images."),
-         skip_ocr:  Optional[bool] = typer.Option(False, help="Skip the OCR of images from PDF files.")):
+         skip_ocr:  Optional[bool] = typer.Option(False, help="Skip the OCR of images from PDF files."),
+         parallel: Optional[int] = typer.Option(1, help="Number of paralell PDF to process in threads.")):
     """
     Process PDF files and detect the dominant language.
     """
-    detector = PdfLanguageDetector(languages, input_dir, output_dir, max_pages, resume, skip_images, skip_ocr)
+    detector = PdfLanguageDetector(languages, input_dir, output_dir, max_pages, resume, skip_images, skip_ocr, parallel)
     detector.process_input_files()
 
 @app.command()
 def report(output_dir: Optional[Path] = typer.Option('out', help="Path to the output directory.")):
     """
     Process generated files to output a report
     """
```

### Comparing `pdf_language_detector-0.0.6/src/pld.py` & `pdf_language_detector-0.0.7/src/pld.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 import json
 import os
 import pytesseract
 
+from multiprocessing import Pool, JoinableQueue
 from lingua import IsoCode639_3, LanguageDetectorBuilder
 from langcodes import Language, find as find_language
 from pathlib import Path
 from PIL import Image
-from rich.progress import Progress, SpinnerColumn
 from rich import print
 from sh import pdftoppm
 from typing import Optional, List
 
 class PdfLanguageDetector:
     def __init__(self, 
                 languages: List[str], 
                 input_dir: Path = Path(),
                 output_dir: Optional[Path] = 'out',
                 max_pages: Optional[int] = 5,
                 resume:  Optional[bool] = False,
                 skip_images:  Optional[bool] = False,
-                skip_ocr:  Optional[bool] = False):
+                skip_ocr:  Optional[bool] = False,
+                parallel: Optional[int] = 1):
         """
         Initialize the PdfLanguageDetector class.
 
         Args:
             languages: List of ISO3 language codes.
             input_dir: Path to the input directory.
             output_dir: Path to the output directory.
             max_pages: Maximum number of pages to process per PDF file.
             resume: Skip PDF files already analyzed.
             skip_images: Skip the extraction of PDF files as images.
             skip_ocr: Skip the OCR of images from PDF files.
+            parallel: Number of threads to run in parallel.
         """
         self.languages = [Language.get(language) for language in languages]
         self.lang_detector = LanguageDetectorBuilder.from_iso_codes_639_3(*self.lingua_langs).build()
         self.input_dir = input_dir
         self.output_dir = output_dir
         self.max_pages = max_pages
         self.resume = resume
         self.skip_images = skip_images
         self.skip_ocr = skip_ocr
+        self.parallel = parallel
 
     def create_output_directories(self, *dirs: Path):
         """
         Create output directories if they don't exist.
 
         Args:
             *dirs: Variable number of directory paths to create.
@@ -191,32 +194,42 @@
             self.process_images(images_dir, texts_dir, langs_dir)
         coeff_avgs = self.calculate_coeff_avgs(langs_dir)
         coeff_avgs_file = output_file_dir.resolve() / 'avgs.json'
         with coeff_avgs_file.open("w") as f:
             f.write(json.dumps(coeff_avgs, indent=2))
         return max(coeff_avgs, key=coeff_avgs.get)
 
+    def worker(self, queue: JoinableQueue):
+        while True:
+            input_file, output_file_dir = queue.get()
+            try:
+                if self.resume and self.is_already_analyzed(output_file_dir):
+                    print(f"→ {input_file.resolve()} [blue]SKIPPED[/blue]")
+                else:
+                    print(f"┅ {input_file.resolve()}")
+                    lang = self.analyse_file(input_file, output_file_dir)
+                    print(f"✓ {input_file.resolve()} [green]{lang}[/green]")
+            except Exception:
+                print(f"✕ {input_file.resolve()} [red]ERROR[/red]")
+            finally:
+                queue.task_done()
+
     def process_input_files(self):
         """
         Process all the PDF files in the input directory.
         """
-        for input_file in self.input_dir.glob('**/*.pdf'):
-            with Progress(SpinnerColumn(), "[progress.description]{task.description}", transient=True) as progress:
-                progress.add_task(input_file.resolve(), total=None)
+        # Create a queue that each worker will join
+        queue = JoinableQueue(self.parallel)
+        # Start a pool of worker processes
+        with Pool(self.parallel, self.worker, (queue,)):
+            for input_file in self.input_dir.glob('**/*.pdf'):
                 output_file_dir = self.get_output_dir(input_file)
-                try:
-                    if self.resume and self.is_already_analyzed(output_file_dir):
-                        print(f"→ {input_file.resolve()} [blue]SKIPPED[/blue]")
-                    else:
-                        lang = self.analyse_file(input_file, output_file_dir)
-                        print(f"✓ {input_file.resolve()} [green]{lang}[/green]")            
-                except Exception as e:
-                        print(f"✕ {input_file.resolve()} [red]ERROR[/red]")
-                    
-
+                queue.put((input_file, output_file_dir))
+            queue.join()
+                
     def get_output_dir(self, input_file: Path) -> Path:
         """
         Get the output directory path for a given input file.
 
         Args:
             input_file: Path to the input file.
 
@@ -224,18 +237,16 @@
             The output directory path.
         """
         output_file_dir = input_file.relative_to(self.input_dir)
         output_file_dir = output_file_dir.parent / output_file_dir.stem
         output_file_dir = self.output_dir / output_file_dir
         return output_file_dir
     
-
     def is_already_analyzed(self, output_file_dir: Path) -> bool:
         return (output_file_dir / 'avgs.json').exists()
-    
 
     @property
     def tesseract_langs(self):
         """
         Get the list of languages for Tesseract. As opposed to Lingua,
         Tesseract uses ISO 639-2/B (derived from English)e.
```

### Comparing `pdf_language_detector-0.0.6/src/report.py` & `pdf_language_detector-0.0.7/src/report.py`

 * *Files identical despite different names*

### Comparing `pdf_language_detector-0.0.6/setup.py` & `pdf_language_detector-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 
 entry_points = \
 {'console_scripts': ['pdf-language-detector = src.cli:app',
                      'pld = src.cli:app']}
 
 setup_kwargs = {
     'name': 'pdf-language-detector',
-    'version': '0.0.6',
+    'version': '0.0.7',
     'description': 'A python script to iterate over a list of PDF in a directory and try to guess their language with Tesseract OCR.',
-    'long_description': "# PLD (PDF Language Detector)\n\nPLD is a Python program that analyzes PDF files, extracts images, processes them using Optical Character Recognition (OCR), and detects the dominant language of the text. It provides language detection information in JSON format and calculates the average confidence coefficient for each language.\n\n## Requirements\n\n- [Python 3.8](https://www.python.org/downloads/) or above\n- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)\n- [pdftoppm](https://poppler.freedesktop.org/)\n\n## Installation\n\nInstall Tesseract OCR and pdftoppm using your package manager. For example, on Ubuntu:\n\n```bash\nsudo apt install tesseract-ocr tesseract-ocr-all poppler-utils\n```\n\n### From PyPi\n\nInstall with pip:\n\n```bash\npython3 -m pip install --user pdf-language-detector\n```\n\nThen run directly from your terminal:\n\n```bash\npld --help\n````\n\n### From the sources\n\nClone the PLD repository:\n\n```bash\ngit clone git@github.com:github.com/icij/pld.git\n```\n\nInstall the required Python packages with poetry:\n\n```bash\npoetry install\n````\n\nThen run inside a virtual env managed by poetry:\n\n```bash\npoetry run pld --help\n````\n\n### From Docker\n\nInstall with Docker:\n\n```bash\ndocker pull icij/pld\n```\n\nThen run inside a container:\n\n```bash\ndocker run -it icij/pld pld --help\n```\n\n\n## Usage\n\n### Detect\n\nThis command process PDF files and detect the dominant language.\n\n```\npld detect --help\n\n    --language A list of ISO3 language codes to detect.\n    --input-dir: Path to the input directory containing PDF files. Default is the current directory.\n    --output-dir (optional): Path to the output directory. Default is 'out' directory in the current directory.\n    --max-pages (optional): Maximum number of pages to process per PDF file. Default is 5.\n    --resume (optional): Skip PDF files already analyzed.\n    --skip-images (optional): Skip the extraction of PDF files a images.\n    --skip-ocr (optional): Skip the OCR of images from PDF files.\n```\n\n### Report\n\nThis command print a report from the previously detected language (using the same output dir).\n\n```\npld report --help\n\n    --output-dir: Path to the output directory. Default is 'out' directory in the current directory.\n```\n\n## Examples\n\nProcess PDF files in the current directory, detect English and Spanish languages, and save the results in the 'results' directory:\n\n```bash\npld --language eng --language spa --input-dir documents --output-dir results\n```\n\nProcess PDF files in the 'documents' directory, detect French and Greek languages, and limit the processing to 3 pages per file:\n\n```bash\npld --language fra --language ell --input-dir documents --max-pages 3\n```\n\n## License\n\nThis project is licensed under the MIT License.\n",
+    'long_description': "# PLD (PDF Language Detector)\n\nPLD is a Python program that analyzes PDF files, extracts images, processes them using Optical Character Recognition (OCR), and detects the dominant language of the text. It provides language detection information in JSON format and calculates the average confidence coefficient for each language.\n\n## Requirements\n\n- [Python 3.8](https://www.python.org/downloads/) or above\n- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)\n- [pdftoppm](https://poppler.freedesktop.org/)\n\n## Installation\n\nInstall Tesseract OCR and pdftoppm using your package manager. For example, on Ubuntu:\n\n```bash\nsudo apt install tesseract-ocr tesseract-ocr-all poppler-utils\n```\n\n### From PyPi\n\nInstall with pip:\n\n```bash\npython3 -m pip install --user pdf-language-detector\n```\n\nThen run directly from your terminal:\n\n```bash\npld --help\n````\n\n### From the sources\n\nClone the PLD repository:\n\n```bash\ngit clone git@github.com:github.com/icij/pld.git\n```\n\nInstall the required Python packages with poetry:\n\n```bash\npoetry install\n````\n\nThen run inside a virtual env managed by poetry:\n\n```bash\npoetry run pld --help\n````\n\n### From Docker\n\nInstall with Docker:\n\n```bash\ndocker pull icij/pld\n```\n\nThen run inside a container:\n\n```bash\ndocker run -it icij/pld pld --help\n```\n\n\n## Usage\n\n### Detect\n\nThis command process PDF files and detect the dominant language.\n\n```\npld detect --help\n\n    --language A list of ISO3 language codes to detect.\n    --input-dir: Path to the input directory containing PDF files. Default is the current directory.\n    --output-dir (optional): Path to the output directory. Default is 'out' directory in the current directory.\n    --max-pages (optional): Maximum number of pages to process per PDF file. Default is 5.\n    --resume (optional): Skip PDF files already analyzed.\n    --skip-images (optional): Skip the extraction of PDF files a images.\n    --skip-ocr (optional): Skip the OCR of images from PDF files.\n    --parallel (optional): Number of threads to run in parallel.\n```\n\n### Report\n\nThis command print a report from the previously detected language (using the same output dir).\n\n```\npld report --help\n\n    --output-dir: Path to the output directory. Default is 'out' directory in the current directory.\n```\n\n## Examples\n\nProcess PDF files in the current directory, detect English and Spanish languages, and save the results in the 'results' directory:\n\n```bash\npld --language eng --language spa --input-dir documents --output-dir results\n```\n\nProcess PDF files in the 'documents' directory, detect French and Greek languages, and limit the processing to 3 pages per file:\n\n```bash\npld --language fra --language ell --input-dir documents --max-pages 3\n```\n\n## License\n\nThis project is licensed under the MIT License.\n",
     'author': 'ICIJ',
     'author_email': 'engineering@icij.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pdf_language_detector-0.0.6/PKG-INFO` & `pdf_language_detector-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf-language-detector
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python script to iterate over a list of PDF in a directory and try to guess their language with Tesseract OCR.
 Author: ICIJ
 Author-email: engineering@icij.org
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -96,14 +96,15 @@
     --language A list of ISO3 language codes to detect.
     --input-dir: Path to the input directory containing PDF files. Default is the current directory.
     --output-dir (optional): Path to the output directory. Default is 'out' directory in the current directory.
     --max-pages (optional): Maximum number of pages to process per PDF file. Default is 5.
     --resume (optional): Skip PDF files already analyzed.
     --skip-images (optional): Skip the extraction of PDF files a images.
     --skip-ocr (optional): Skip the OCR of images from PDF files.
+    --parallel (optional): Number of threads to run in parallel.
 ```
 
 ### Report
 
 This command print a report from the previously detected language (using the same output dir).
 
 ```
```

