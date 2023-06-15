# Comparing `tmp/pdf_language_detector-0.0.7.tar.gz` & `tmp/pdf_language_detector-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_language_detector-0.0.7.tar", max compression
+gzip compressed data, was "pdf_language_detector-0.0.8.tar", max compression
```

## Comparing `pdf_language_detector-0.0.7.tar` & `pdf_language_detector-0.0.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2772 2023-06-15 18:42:42.158079 pdf_language_detector-0.0.7/README.md
--rw-r--r--   0        0        0      744 2023-06-15 18:44:06.610843 pdf_language_detector-0.0.7/pyproject.toml
--rw-r--r--   0        0        0       24 2023-06-14 22:13:51.629533 pdf_language_detector-0.0.7/src/__init__.py
--rw-r--r--   0        0        0     1466 2023-06-15 15:36:48.029796 pdf_language_detector-0.0.7/src/cli.py
--rw-r--r--   0        0        0    10085 2023-06-15 18:38:19.863717 pdf_language_detector-0.0.7/src/pld.py
--rw-r--r--   0        0        0     3735 2023-06-15 14:29:56.113761 pdf_language_detector-0.0.7/src/report.py
--rw-r--r--   0        0        0     3905 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.7/setup.py
--rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     2772 2023-06-15 18:42:42.158079 pdf_language_detector-0.0.8/README.md
+-rw-r--r--   0        0        0      744 2023-06-15 20:12:55.815424 pdf_language_detector-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-06-14 22:13:51.629533 pdf_language_detector-0.0.8/src/__init__.py
+-rw-r--r--   0        0        0     1466 2023-06-15 15:36:48.029796 pdf_language_detector-0.0.8/src/cli.py
+-rw-r--r--   0        0        0    12932 2023-06-15 20:12:03.762975 pdf_language_detector-0.0.8/src/pld.py
+-rw-r--r--   0        0        0     3735 2023-06-15 14:29:56.113761 pdf_language_detector-0.0.8/src/report.py
+-rw-r--r--   0        0        0     3905 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.8/setup.py
+-rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.8/PKG-INFO
```

### Comparing `pdf_language_detector-0.0.7/README.md` & `pdf_language_detector-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pdf_language_detector-0.0.7/pyproject.toml` & `pdf_language_detector-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdf-language-detector"
-version = "0.0.7"
+version = "0.0.8"
 description = "A python script to iterate over a list of PDF in a directory and try to guess their language with Tesseract OCR."
 authors = ["ICIJ <engineering@icij.org>"]
 readme = "README.md"
 packages = [{include = "src"}]
 
 [tool.poetry.dependencies]
 python = '^3.8.1'
```

### Comparing `pdf_language_detector-0.0.7/src/cli.py` & `pdf_language_detector-0.0.8/src/cli.py`

 * *Files identical despite different names*

### Comparing `pdf_language_detector-0.0.7/src/pld.py` & `pdf_language_detector-0.0.8/src/pld.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 import json
 import os
 import pytesseract
 
-from multiprocessing import Pool, JoinableQueue
+from multiprocessing import Pool, JoinableQueue, Manager
 from lingua import IsoCode639_3, LanguageDetectorBuilder
 from langcodes import Language, find as find_language
 from pathlib import Path
 from PIL import Image
 from rich import print
+from rich.progress import Progress, SpinnerColumn
 from sh import pdftoppm
 from typing import Optional, List
 
 class PdfLanguageDetector:
+    STATUS_SKIPPED = 'SKIPPED'
+    STATUS_DONE = 'DONE'
+    STATUS_FAILED = 'FAILED'
+    
     def __init__(self, 
                 languages: List[str], 
                 input_dir: Path = Path(),
                 output_dir: Optional[Path] = 'out',
                 max_pages: Optional[int] = 5,
                 resume:  Optional[bool] = False,
                 skip_images:  Optional[bool] = False,
@@ -196,39 +201,95 @@
         coeff_avgs_file = output_file_dir.resolve() / 'avgs.json'
         with coeff_avgs_file.open("w") as f:
             f.write(json.dumps(coeff_avgs, indent=2))
         return max(coeff_avgs, key=coeff_avgs.get)
 
     def worker(self, queue: JoinableQueue):
         while True:
-            input_file, output_file_dir = queue.get()
+            input_file, output_file_dir, tasks_statuses = queue.get()
             try:
                 if self.resume and self.is_already_analyzed(output_file_dir):
-                    print(f"→ {input_file.resolve()} [blue]SKIPPED[/blue]")
+                    tasks_statuses[input_file] = dict(status=PdfLanguageDetector.STATUS_SKIPPED)
                 else:
-                    print(f"┅ {input_file.resolve()}")
                     lang = self.analyse_file(input_file, output_file_dir)
-                    print(f"✓ {input_file.resolve()} [green]{lang}[/green]")
+                    tasks_statuses[input_file] = dict(status=PdfLanguageDetector.STATUS_DONE, lang=lang)
             except Exception:
-                print(f"✕ {input_file.resolve()} [red]ERROR[/red]")
+                tasks_statuses[input_file] = dict(status=PdfLanguageDetector.STATUS_FAILED)
             finally:
                 queue.task_done()
 
     def process_input_files(self):
         """
         Process all the PDF files in the input directory.
         """
         # Create a queue that each worker will join
         queue = JoinableQueue(self.parallel)
         # Start a pool of worker processes
         with Pool(self.parallel, self.worker, (queue,)):
-            for input_file in self.input_dir.glob('**/*.pdf'):
-                output_file_dir = self.get_output_dir(input_file)
-                queue.put((input_file, output_file_dir))
+            # Create progress bar
+            with Progress(SpinnerColumn(), "[progress.description]{task.description}", transient=True) as progress:
+                # Shared dictionary for task statuses
+                tasks_statuses = Manager().dict()
+                # Dictionary for tracking tasks' progress
+                tasks_progresses = dict()
+                for input_file in self.input_dir.glob('**/*.pdf'):
+                    # Add task to the progress bar
+                    if len(tasks_progresses) < self.parallel:
+                        tasks_progresses[input_file] = progress.add_task(input_file.resolve(), total=None)
+                    self.process_file(input_file, queue, progress, tasks_statuses, tasks_progresses)
+                self.print_tasks_statuses(tasks_statuses)
             queue.join()
+
+    def process_file(self, input_file, queue, progress, tasks_statuses, tasks_progresses):
+        """
+        Process a single PDF file.
+
+        Args:
+            input_file: Path to the input PDF file.
+            queue: JoinableQueue for worker processes.
+            progress: Progress bar for displaying task progress.
+            tasks_statuses: Shared dictionary for task statuses.
+            tasks_progresses: Dictionary for tracking tasks' progress.
+        """
+        output_file_dir = self.get_output_dir(input_file)
+        queue.put((input_file, output_file_dir, tasks_statuses))
+        self.update_progress(progress, tasks_statuses, tasks_progresses)
+
+    def update_progress(self, progress, tasks_statuses, tasks_progresses):
+        """
+        Update the progress bar and print task statuses.
+
+        Args:
+            progress: Progress bar for displaying task progress.
+            tasks_statuses: Shared dictionary for task statuses.
+            tasks_progresses: Dictionary for tracking tasks' progress.
+        """
+        for key in tasks_statuses.copy():
+            if key in tasks_progresses:
+                task = tasks_progresses.pop(key)
+                progress.remove_task(task)
+        self.print_tasks_statuses(tasks_statuses)
+
+    def print_tasks_statuses(self, tasks_statuses):
+        """
+        Print the statuses of completed tasks.
+
+        Args:
+            tasks_statuses: Shared dictionary for task statuses.
+        """
+        for key in tasks_statuses.copy():
+            task = tasks_statuses.pop(key)
+            if task['status'] ==  PdfLanguageDetector.STATUS_DONE:
+                print(f"✓ {key.resolve()} [green]{task['lang']}[/green]")
+            elif task['status'] == PdfLanguageDetector.STATUS_SKIPPED:
+                print(f"→ {key.resolve()} [blue]SKIPPED[/blue]")
+            elif task['status'] == PdfLanguageDetector.STATUS_FAILED:
+                print(f"✕ {key.resolve()} [red]FAILED[/red]")
+            else:
+                print(f"? {key.resolve()} [orange]UNKNOWN[/orange]")
                 
     def get_output_dir(self, input_file: Path) -> Path:
         """
         Get the output directory path for a given input file.
 
         Args:
             input_file: Path to the input file.
```

### Comparing `pdf_language_detector-0.0.7/src/report.py` & `pdf_language_detector-0.0.8/src/report.py`

 * *Files identical despite different names*

### Comparing `pdf_language_detector-0.0.7/setup.py` & `pdf_language_detector-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 entry_points = \
 {'console_scripts': ['pdf-language-detector = src.cli:app',
                      'pld = src.cli:app']}
 
 setup_kwargs = {
     'name': 'pdf-language-detector',
-    'version': '0.0.7',
+    'version': '0.0.8',
     'description': 'A python script to iterate over a list of PDF in a directory and try to guess their language with Tesseract OCR.',
     'long_description': "# PLD (PDF Language Detector)\n\nPLD is a Python program that analyzes PDF files, extracts images, processes them using Optical Character Recognition (OCR), and detects the dominant language of the text. It provides language detection information in JSON format and calculates the average confidence coefficient for each language.\n\n## Requirements\n\n- [Python 3.8](https://www.python.org/downloads/) or above\n- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)\n- [pdftoppm](https://poppler.freedesktop.org/)\n\n## Installation\n\nInstall Tesseract OCR and pdftoppm using your package manager. For example, on Ubuntu:\n\n```bash\nsudo apt install tesseract-ocr tesseract-ocr-all poppler-utils\n```\n\n### From PyPi\n\nInstall with pip:\n\n```bash\npython3 -m pip install --user pdf-language-detector\n```\n\nThen run directly from your terminal:\n\n```bash\npld --help\n````\n\n### From the sources\n\nClone the PLD repository:\n\n```bash\ngit clone git@github.com:github.com/icij/pld.git\n```\n\nInstall the required Python packages with poetry:\n\n```bash\npoetry install\n````\n\nThen run inside a virtual env managed by poetry:\n\n```bash\npoetry run pld --help\n````\n\n### From Docker\n\nInstall with Docker:\n\n```bash\ndocker pull icij/pld\n```\n\nThen run inside a container:\n\n```bash\ndocker run -it icij/pld pld --help\n```\n\n\n## Usage\n\n### Detect\n\nThis command process PDF files and detect the dominant language.\n\n```\npld detect --help\n\n    --language A list of ISO3 language codes to detect.\n    --input-dir: Path to the input directory containing PDF files. Default is the current directory.\n    --output-dir (optional): Path to the output directory. Default is 'out' directory in the current directory.\n    --max-pages (optional): Maximum number of pages to process per PDF file. Default is 5.\n    --resume (optional): Skip PDF files already analyzed.\n    --skip-images (optional): Skip the extraction of PDF files a images.\n    --skip-ocr (optional): Skip the OCR of images from PDF files.\n    --parallel (optional): Number of threads to run in parallel.\n```\n\n### Report\n\nThis command print a report from the previously detected language (using the same output dir).\n\n```\npld report --help\n\n    --output-dir: Path to the output directory. Default is 'out' directory in the current directory.\n```\n\n## Examples\n\nProcess PDF files in the current directory, detect English and Spanish languages, and save the results in the 'results' directory:\n\n```bash\npld --language eng --language spa --input-dir documents --output-dir results\n```\n\nProcess PDF files in the 'documents' directory, detect French and Greek languages, and limit the processing to 3 pages per file:\n\n```bash\npld --language fra --language ell --input-dir documents --max-pages 3\n```\n\n## License\n\nThis project is licensed under the MIT License.\n",
     'author': 'ICIJ',
     'author_email': 'engineering@icij.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pdf_language_detector-0.0.7/PKG-INFO` & `pdf_language_detector-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf-language-detector
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python script to iterate over a list of PDF in a directory and try to guess their language with Tesseract OCR.
 Author: ICIJ
 Author-email: engineering@icij.org
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

