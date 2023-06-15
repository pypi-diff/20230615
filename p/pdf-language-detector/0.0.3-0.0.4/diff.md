# Comparing `tmp/pdf_language_detector-0.0.3.tar.gz` & `tmp/pdf_language_detector-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_language_detector-0.0.3.tar", max compression
+gzip compressed data, was "pdf_language_detector-0.0.4.tar", max compression
```

## Comparing `pdf_language_detector-0.0.3.tar` & `pdf_language_detector-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     2327 2023-06-15 10:32:33.053853 pdf_language_detector-0.0.3/README.md
--rw-r--r--   0        0        0      744 2023-06-15 10:32:57.470057 pdf_language_detector-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       24 2023-06-14 22:13:51.629533 pdf_language_detector-0.0.3/src/__init__.py
--rw-r--r--   0        0        0     1031 2023-06-15 10:22:30.384584 pdf_language_detector-0.0.3/src/cli.py
--rw-r--r--   0        0        0     8688 2023-06-15 10:28:42.755903 pdf_language_detector-0.0.3/src/pld.py
--rw-r--r--   0        0        0     3444 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.3/setup.py
--rw-r--r--   0        0        0     3104 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2707 2023-06-15 13:51:48.211566 pdf_language_detector-0.0.4/README.md
+-rw-r--r--   0        0        0      744 2023-06-15 13:58:09.402339 pdf_language_detector-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-06-14 22:13:51.629533 pdf_language_detector-0.0.4/src/__init__.py
+-rw-r--r--   0        0        0     1350 2023-06-15 13:51:45.811549 pdf_language_detector-0.0.4/src/cli.py
+-rw-r--r--   0        0        0     9711 2023-06-15 13:56:12.913500 pdf_language_detector-0.0.4/src/pld.py
+-rw-r--r--   0        0        0     3734 2023-06-15 13:44:40.224290 pdf_language_detector-0.0.4/src/report.py
+-rw-r--r--   0        0        0     3839 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.4/setup.py
+-rw-r--r--   0        0        0     3484 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.4/PKG-INFO
```

### Comparing `pdf_language_detector-0.0.3/README.md` & `pdf_language_detector-0.0.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -63,25 +63,40 @@
 ```bash
 docker run -it icij/pld pld --help
 ```
 
 
 ## Usage
 
+### Detect
+
+This command process PDF files and detect the dominant language.
+
 ```
-pld --help
+pld detect --help
 
     --language A list of ISO3 language codes to detect.
     --input-dir: Path to the input directory containing PDF files. Default is the current directory.
     --output-dir (optional): Path to the output directory. Default is 'out' directory in the current directory.
     --max-pages (optional): Maximum number of pages to process per PDF file. Default is 5.
+    --resume (optional): Skip PDF files already analyzed.
     --skip-images (optional): Skip the extraction of PDF files a images.
     --skip-ocr (optional): Skip the OCR of images from PDF files.
 ```
 
+### Report
+
+This command print a report from the previously detected language (using the same output dir).
+
+```
+pld report --help
+
+    --output-dir: Path to the output directory. Default is 'out' directory in the current directory.
+```
+
 ## Examples
 
 Process PDF files in the current directory, detect English and Spanish languages, and save the results in the 'results' directory:
 
 ```bash
 pld --language eng --language spa --input-dir documents --output-dir results
 ```
```

### Comparing `pdf_language_detector-0.0.3/pyproject.toml` & `pdf_language_detector-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdf-language-detector"
-version = "0.0.3"
+version = "0.0.4"
 description = "A python script to iterate over a list of PDF in a directory and try to guess their language with Tesseract OCR."
 authors = ["ICIJ <engineering@icij.org>"]
 readme = "README.md"
 packages = [{include = "src"}]
 
 [tool.poetry.dependencies]
 python = '^3.8.1'
```

### Comparing `pdf_language_detector-0.0.3/src/cli.py` & `pdf_language_detector-0.0.4/src/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 import typer
 
 from pathlib import Path
 from typing import Optional, List
 from src.pld import PdfLanguageDetector
+from src.report import Report
 
 app = typer.Typer()
 
 @app.command()
-def main(languages: List[str] = typer.Option(..., '--language', help="An ISO3 language code."), 
+def detect(languages: List[str] = typer.Option(..., '--language', help="An ISO3 language code."), 
          input_dir: Path  = typer.Option(..., '--input-dir', help="Path to the input directory."),
          output_dir: Optional[Path] = typer.Option('out', help="Path to the output directory."),
          max_pages: Optional[int] = typer.Option(5, help="Maximum number of pages to process per PDF file."),
+         resume: Optional[bool] = typer.Option(False, help="Skip PDF files already analyzed."),
          skip_images:  Optional[bool] = typer.Option(False, help="Skip the extraction of PDF files as images."),
          skip_ocr:  Optional[bool] = typer.Option(False, help="Skip the OCR of images from PDF files.")):
     """
     Process PDF files and detect the dominant language.
     """
-    detector = PdfLanguageDetector(languages, input_dir, output_dir, max_pages, skip_images, skip_ocr)
+    detector = PdfLanguageDetector(languages, input_dir, output_dir, max_pages, resume, skip_images, skip_ocr)
     detector.process_input_files()
 
-
-if __name__ == "__main__":
-    typer.run(main)
+@app.command()
+def report(output_dir: Optional[Path] = typer.Option('out', help="Path to the output directory.")):
+    """
+    Process generated files to output a report
+    """
+    report = Report(output_dir)
+    report.generate()
```

### Comparing `pdf_language_detector-0.0.3/src/pld.py` & `pdf_language_detector-0.0.4/src/pld.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,53 +3,64 @@
 import pytesseract
 
 from lingua import IsoCode639_3, LanguageDetectorBuilder
 from langcodes import Language, find as find_language
 from pathlib import Path
 from PIL import Image
 from rich.progress import Progress, SpinnerColumn
+from rich import print
 from sh import pdftoppm
 from typing import Optional, List
 
 class PdfLanguageDetector:
     def __init__(self, 
                 languages: List[str], 
                 input_dir: Path = Path(),
                 output_dir: Optional[Path] = 'out',
                 max_pages: Optional[int] = 5,
+                resume:  Optional[bool] = False,
                 skip_images:  Optional[bool] = False,
                 skip_ocr:  Optional[bool] = False):
         """
         Initialize the PdfLanguageDetector class.
 
         Args:
             languages: List of ISO3 language codes.
             input_dir: Path to the input directory.
             output_dir: Path to the output directory.
             max_pages: Maximum number of pages to process per PDF file.
+            resume: Skip PDF files already analyzed.
             skip_images: Skip the extraction of PDF files as images.
             skip_ocr: Skip the OCR of images from PDF files.
         """
         self.languages = [Language.get(language) for language in languages]
         self.lang_detector = LanguageDetectorBuilder.from_iso_codes_639_3(*self.lingua_langs).build()
         self.input_dir = input_dir
         self.output_dir = output_dir
         self.max_pages = max_pages
+        self.resume = resume
         self.skip_images = skip_images
         self.skip_ocr = skip_ocr
 
     def create_output_directories(self, *dirs: Path):
         """
         Create output directories if they don't exist.
 
         Args:
             *dirs: Variable number of directory paths to create.
         """
         for dir_path in dirs:
             os.makedirs(dir_path.resolve(), exist_ok=True)
+    
+    def extract_meta(self, input_file: Path):
+        output_dir = self.get_output_dir(input_file)
+        meta_file = output_dir / 'meta.json'
+        meta = dict(input_file=str(input_file.resolve()), output_dir=str(output_dir.resolve()))
+        with meta_file.open("w") as f:
+            f.write(json.dumps(meta, indent=2))
 
     def extract_images(self, input_file: Path, images_dir: Path):
         """
         Extract images from a PDF file using pdftoppm.
 
         Args:
             input_file: Path to the input PDF file.
@@ -169,14 +180,15 @@
         Returns:
             The language with the highest average coefficient.
         """
         images_dir = output_file_dir / 'images'
         texts_dir = output_file_dir / 'texts'
         langs_dir = output_file_dir / 'langs'
         self.create_output_directories(images_dir, texts_dir, langs_dir)
+        self.extract_meta(input_file)
         if not self.skip_images:
             self.extract_images(input_file, images_dir)
         if not self.skip_ocr:
             self.process_images(images_dir, texts_dir, langs_dir)
         coeff_avgs = self.calculate_coeff_avgs(langs_dir)
         coeff_avgs_file = output_file_dir.resolve() / 'avgs.json'
         with coeff_avgs_file.open("w") as f:
@@ -185,18 +197,24 @@
 
     def process_input_files(self):
         """
         Process all the PDF files in the input directory.
         """
         for input_file in sorted(self.input_dir.glob('**/*.pdf')):                    
             with Progress(SpinnerColumn(), "[progress.description]{task.description}", transient=True) as progress:
-                output_file_dir = self.get_output_dir(input_file)
                 progress.add_task(input_file.resolve(), total=None)
-                lang = self.analyse_file(input_file, output_file_dir)
-                print(f"✓ {input_file.resolve()} {lang}")
+                output_file_dir = self.get_output_dir(input_file)
+                try:
+                    if self.resume and self.is_already_analyzed(output_file_dir):
+                        print(f"→ {input_file.resolve()} [blue]SKIPPED[/blue]")
+                    else:
+                        lang = self.analyse_file(input_file, output_file_dir)
+                        print(f"✓ {input_file.resolve()} [green]{lang}[/green]")            
+                except Exception as e:
+                        print(f"✕ {input_file.resolve()} [red]ERROR[/red]")
                     
 
     def get_output_dir(self, input_file: Path) -> Path:
         """
         Get the output directory path for a given input file.
 
         Args:
@@ -207,14 +225,18 @@
         """
         output_file_dir = input_file.relative_to(self.input_dir)
         output_file_dir = output_file_dir.parent / output_file_dir.stem
         output_file_dir = self.output_dir / output_file_dir
         return output_file_dir
     
 
+    def is_already_analyzed(self, output_file_dir: Path) -> bool:
+        return (output_file_dir / 'avgs.json').exists()
+    
+
     @property
     def tesseract_langs(self):
         """
         Get the list of languages for Tesseract. As opposed to Lingua,
         Tesseract uses ISO 639-2/B (derived from English)e.
 
         Returns:
```

### Comparing `pdf_language_detector-0.0.3/setup.py` & `pdf_language_detector-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 
 entry_points = \
 {'console_scripts': ['pdf-language-detector = src.cli:app',
                      'pld = src.cli:app']}
 
 setup_kwargs = {
     'name': 'pdf-language-detector',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'A python script to iterate over a list of PDF in a directory and try to guess their language with Tesseract OCR.',
-    'long_description': "# PLD (PDF Language Detector)\n\nPLD is a Python program that analyzes PDF files, extracts images, processes them using Optical Character Recognition (OCR), and detects the dominant language of the text. It provides language detection information in JSON format and calculates the average confidence coefficient for each language.\n\n## Requirements\n\n- [Python 3.8](https://www.python.org/downloads/) or above\n- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)\n- [pdftoppm](https://poppler.freedesktop.org/)\n\n## Installation\n\nInstall Tesseract OCR and pdftoppm using your package manager. For example, on Ubuntu:\n\n```bash\nsudo apt install tesseract-ocr tesseract-ocr-all poppler-utils\n```\n\n### From PyPi\n\nInstall with pip:\n\n```bash\npython3 -m pip install --user pdf-language-detector\n```\n\nThen run directly from your terminal:\n\n```bash\npld --help\n````\n\n### From the sources\n\nClone the PLD repository:\n\n```bash\ngit clone git@github.com:github.com/icij/pld.git\n```\n\nInstall the required Python packages with poetry:\n\n```bash\npoetry install\n````\n\nThen run inside a virtual env managed by poetry:\n\n```bash\npoetry run pld --help\n````\n\n### From Docker\n\nInstall with Docker:\n\n```bash\ndocker pull icij/pld\n```\n\nThen run inside a container:\n\n```bash\ndocker run -it icij/pld pld --help\n```\n\n\n## Usage\n\n```\npld --help\n\n    --language A list of ISO3 language codes to detect.\n    --input-dir: Path to the input directory containing PDF files. Default is the current directory.\n    --output-dir (optional): Path to the output directory. Default is 'out' directory in the current directory.\n    --max-pages (optional): Maximum number of pages to process per PDF file. Default is 5.\n    --skip-images (optional): Skip the extraction of PDF files a images.\n    --skip-ocr (optional): Skip the OCR of images from PDF files.\n```\n\n## Examples\n\nProcess PDF files in the current directory, detect English and Spanish languages, and save the results in the 'results' directory:\n\n```bash\npld --language eng --language spa --input-dir documents --output-dir results\n```\n\nProcess PDF files in the 'documents' directory, detect French and Greek languages, and limit the processing to 3 pages per file:\n\n```bash\npld --language fra --language ell --input-dir documents --max-pages 3\n```\n\n## License\n\nThis project is licensed under the MIT License.\n",
+    'long_description': "# PLD (PDF Language Detector)\n\nPLD is a Python program that analyzes PDF files, extracts images, processes them using Optical Character Recognition (OCR), and detects the dominant language of the text. It provides language detection information in JSON format and calculates the average confidence coefficient for each language.\n\n## Requirements\n\n- [Python 3.8](https://www.python.org/downloads/) or above\n- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)\n- [pdftoppm](https://poppler.freedesktop.org/)\n\n## Installation\n\nInstall Tesseract OCR and pdftoppm using your package manager. For example, on Ubuntu:\n\n```bash\nsudo apt install tesseract-ocr tesseract-ocr-all poppler-utils\n```\n\n### From PyPi\n\nInstall with pip:\n\n```bash\npython3 -m pip install --user pdf-language-detector\n```\n\nThen run directly from your terminal:\n\n```bash\npld --help\n````\n\n### From the sources\n\nClone the PLD repository:\n\n```bash\ngit clone git@github.com:github.com/icij/pld.git\n```\n\nInstall the required Python packages with poetry:\n\n```bash\npoetry install\n````\n\nThen run inside a virtual env managed by poetry:\n\n```bash\npoetry run pld --help\n````\n\n### From Docker\n\nInstall with Docker:\n\n```bash\ndocker pull icij/pld\n```\n\nThen run inside a container:\n\n```bash\ndocker run -it icij/pld pld --help\n```\n\n\n## Usage\n\n### Detect\n\nThis command process PDF files and detect the dominant language.\n\n```\npld detect --help\n\n    --language A list of ISO3 language codes to detect.\n    --input-dir: Path to the input directory containing PDF files. Default is the current directory.\n    --output-dir (optional): Path to the output directory. Default is 'out' directory in the current directory.\n    --max-pages (optional): Maximum number of pages to process per PDF file. Default is 5.\n    --resume (optional): Skip PDF files already analyzed.\n    --skip-images (optional): Skip the extraction of PDF files a images.\n    --skip-ocr (optional): Skip the OCR of images from PDF files.\n```\n\n### Report\n\nThis command print a report from the previously detected language (using the same output dir).\n\n```\npld report --help\n\n    --output-dir: Path to the output directory. Default is 'out' directory in the current directory.\n```\n\n## Examples\n\nProcess PDF files in the current directory, detect English and Spanish languages, and save the results in the 'results' directory:\n\n```bash\npld --language eng --language spa --input-dir documents --output-dir results\n```\n\nProcess PDF files in the 'documents' directory, detect French and Greek languages, and limit the processing to 3 pages per file:\n\n```bash\npld --language fra --language ell --input-dir documents --max-pages 3\n```\n\n## License\n\nThis project is licensed under the MIT License.\n",
     'author': 'ICIJ',
     'author_email': 'engineering@icij.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pdf_language_detector-0.0.3/PKG-INFO` & `pdf_language_detector-0.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf-language-detector
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python script to iterate over a list of PDF in a directory and try to guess their language with Tesseract OCR.
 Author: ICIJ
 Author-email: engineering@icij.org
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -82,25 +82,40 @@
 ```bash
 docker run -it icij/pld pld --help
 ```
 
 
 ## Usage
 
+### Detect
+
+This command process PDF files and detect the dominant language.
+
 ```
-pld --help
+pld detect --help
 
     --language A list of ISO3 language codes to detect.
     --input-dir: Path to the input directory containing PDF files. Default is the current directory.
     --output-dir (optional): Path to the output directory. Default is 'out' directory in the current directory.
     --max-pages (optional): Maximum number of pages to process per PDF file. Default is 5.
+    --resume (optional): Skip PDF files already analyzed.
     --skip-images (optional): Skip the extraction of PDF files a images.
     --skip-ocr (optional): Skip the OCR of images from PDF files.
 ```
 
+### Report
+
+This command print a report from the previously detected language (using the same output dir).
+
+```
+pld report --help
+
+    --output-dir: Path to the output directory. Default is 'out' directory in the current directory.
+```
+
 ## Examples
 
 Process PDF files in the current directory, detect English and Spanish languages, and save the results in the 'results' directory:
 
 ```bash
 pld --language eng --language spa --input-dir documents --output-dir results
 ```
```

