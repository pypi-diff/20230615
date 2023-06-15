# Comparing `tmp/biobear-0.5.0.tar.gz` & `tmp/biobear-0.6.0.tar.gz`

## Comparing `biobear-0.5.0.tar` & `biobear-0.6.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
--rw-r--r--   0        0        0      307 1970-01-01 00:00:00.000000 biobear-0.5.0/Cargo.toml
--rw-r--r--   0     1001      123     2566 2023-06-14 21:27:24.000000 biobear-0.5.0/.github/workflows/release.yml
--rw-r--r--   0     1001      123      865 2023-06-14 21:27:24.000000 biobear-0.5.0/.github/workflows/smoke-test.yml
--rw-r--r--   0     1001      123      107 2023-06-14 21:27:24.000000 biobear-0.5.0/.github/workflows/smoketest.py
--rw-r--r--   0     1001      123      999 2023-06-14 21:27:24.000000 biobear-0.5.0/.github/workflows/test.yml
--rw-r--r--   0     1001      123     4135 2023-06-14 21:27:24.000000 biobear-0.5.0/.gitignore
--rw-r--r--   0     1001      123     1055 2023-06-14 21:27:24.000000 biobear-0.5.0/LICENSE
--rw-r--r--   0     1001      123       71 2023-06-14 21:27:24.000000 biobear-0.5.0/Makefile
--rw-r--r--   0     1001      123    16222 2023-06-14 21:27:24.000000 biobear-0.5.0/README.md
--rw-r--r--   0     1001      123      186 2023-06-14 21:27:24.000000 biobear-0.5.0/cz.json
--rw-r--r--   0     1001      123      238 2023-06-14 21:27:24.000000 biobear-0.5.0/docs.bash
--rw-r--r--   0     1001      123      565 2023-06-14 21:27:24.000000 biobear-0.5.0/pyproject.toml
--rw-r--r--   0     1001      123      552 2023-06-14 21:27:24.000000 biobear-0.5.0/python/biobear/__init__.py
--rw-r--r--   0     1001      123     1343 2023-06-14 21:27:24.000000 biobear-0.5.0/python/biobear/bam_reader.py
--rw-r--r--   0     1001      123      720 2023-06-14 21:27:24.000000 biobear-0.5.0/python/biobear/compression.py
--rw-r--r--   0     1001      123      931 2023-06-14 21:27:24.000000 biobear-0.5.0/python/biobear/fasta_reader.py
--rw-r--r--   0     1001      123      927 2023-06-14 21:27:24.000000 biobear-0.5.0/python/biobear/fastq_reader.py
--rw-r--r--   0     1001      123      787 2023-06-14 21:27:24.000000 biobear-0.5.0/python/biobear/genbank_reader.py
--rw-r--r--   0     1001      123     1390 2023-06-14 21:27:24.000000 biobear-0.5.0/python/biobear/gff_reader.py
--rw-r--r--   0     1001      123      941 2023-06-14 21:27:24.000000 biobear-0.5.0/python/biobear/reader.py
--rw-r--r--   0     1001      123     1400 2023-06-14 21:27:24.000000 biobear-0.5.0/python/biobear/vcf_reader.py
--rw-r--r--   0     1001      123   124562 2023-06-14 21:27:24.000000 biobear-0.5.0/python/tests/data/BGC0000404.gbk
--rw-r--r--   0     1001      123     6152 2023-06-14 21:27:24.000000 biobear-0.5.0/python/tests/data/bedcov.bam
--rw-r--r--   0     1001      123     7608 2023-06-14 21:27:24.000000 biobear-0.5.0/python/tests/data/bedcov.bam.bai
--rw-r--r--   0     1001      123     1749 2023-06-14 21:27:24.000000 biobear-0.5.0/python/tests/data/file.vcf
--rw-r--r--   0     1001      123     8638 2023-06-14 21:27:24.000000 biobear-0.5.0/python/tests/data/index.vcf.gz
--rw-r--r--   0     1001      123      213 2023-06-14 21:27:24.000000 biobear-0.5.0/python/tests/data/index.vcf.gz.tbi
--rw-r--r--   0     1001      123       41 2023-06-14 21:27:24.000000 biobear-0.5.0/python/tests/data/test.fasta
--rw-r--r--   0     1001      123       58 2023-06-14 21:27:24.000000 biobear-0.5.0/python/tests/data/test.fasta.gz
--rw-r--r--   0     1001      123      286 2023-06-14 21:27:24.000000 biobear-0.5.0/python/tests/data/test.fastq
--rw-r--r--   0     1001      123      134 2023-06-14 21:27:24.000000 biobear-0.5.0/python/tests/data/test.fastq.gz
--rw-r--r--   0     1001      123      112 2023-06-14 21:27:24.000000 biobear-0.5.0/python/tests/data/test.gff
--rw-r--r--   0     1001      123       91 2023-06-14 21:27:24.000000 biobear-0.5.0/python/tests/data/test.gff.gz
--rw-r--r--   0     1001      123     4302 2023-06-14 21:27:24.000000 biobear-0.5.0/python/tests/data/vcf_file.vcf
--rw-r--r--   0     1001      123     1669 2023-06-14 21:27:24.000000 biobear-0.5.0/python/tests/data/vcf_file.vcf.gz
--rw-r--r--   0     1001      123      254 2023-06-14 21:27:24.000000 biobear-0.5.0/python/tests/data/vcf_file.vcf.gz.tbi
--rw-r--r--   0     1001      123      674 2023-06-14 21:27:24.000000 biobear-0.5.0/python/tests/test_bam_reader.py
--rw-r--r--   0     1001      123     1218 2023-06-14 21:27:24.000000 biobear-0.5.0/python/tests/test_fasta_reader.py
--rw-r--r--   0     1001      123     1154 2023-06-14 21:27:24.000000 biobear-0.5.0/python/tests/test_fastq_reader.py
--rw-r--r--   0     1001      123      421 2023-06-14 21:27:24.000000 biobear-0.5.0/python/tests/test_genbank_reader.py
--rw-r--r--   0     1001      123     1241 2023-06-14 21:27:24.000000 biobear-0.5.0/python/tests/test_gff_reader.py
--rw-r--r--   0     1001      123      755 2023-06-14 21:27:24.000000 biobear-0.5.0/python/tests/test_vcf_reader.py
--rw-r--r--   0     1001      123       20 2023-06-14 21:27:24.000000 biobear-0.5.0/requirements-dev.txt
--rw-r--r--   0     1001      123     4822 2023-06-14 21:27:24.000000 biobear-0.5.0/src/bam_reader.rs
--rw-r--r--   0     1001      123     3474 2023-06-14 21:27:24.000000 biobear-0.5.0/src/exon_reader.rs
--rw-r--r--   0     1001      123      398 2023-06-14 21:27:24.000000 biobear-0.5.0/src/lib.rs
--rw-r--r--   0     1001      123     5329 2023-06-14 21:27:24.000000 biobear-0.5.0/src/vcf_reader.rs
--rw-r--r--   0     1001      123    69725 2023-06-14 21:29:24.000000 biobear-0.5.0/Cargo.lock
--rw-r--r--   0        0        0    16670 1970-01-01 00:00:00.000000 biobear-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      407 1970-01-01 00:00:00.000000 biobear-0.6.0/Cargo.toml
+-rw-r--r--   0     1001      123     2428 2023-06-15 15:55:52.000000 biobear-0.6.0/.github/workflows/release.yml
+-rw-r--r--   0     1001      123      704 2023-06-15 15:55:52.000000 biobear-0.6.0/.github/workflows/smoke-test.yml
+-rw-r--r--   0     1001      123      138 2023-06-15 15:55:52.000000 biobear-0.6.0/.github/workflows/smoketest.py
+-rw-r--r--   0     1001      123      771 2023-06-15 15:55:52.000000 biobear-0.6.0/.github/workflows/test.yml
+-rw-r--r--   0     1001      123     4135 2023-06-15 15:55:52.000000 biobear-0.6.0/.gitignore
+-rw-r--r--   0     1001      123     1290 2023-06-15 15:55:52.000000 biobear-0.6.0/CHANGELOG.md
+-rw-r--r--   0     1001      123     1055 2023-06-15 15:55:52.000000 biobear-0.6.0/LICENSE
+-rw-r--r--   0     1001      123       71 2023-06-15 15:55:52.000000 biobear-0.6.0/Makefile
+-rw-r--r--   0     1001      123    16633 2023-06-15 15:55:52.000000 biobear-0.6.0/README.md
+-rw-r--r--   0     1001      123      224 2023-06-15 15:55:52.000000 biobear-0.6.0/cz.json
+-rw-r--r--   0     1001      123      238 2023-06-15 15:55:52.000000 biobear-0.6.0/docs.bash
+-rw-r--r--   0     1001      123      565 2023-06-15 15:55:52.000000 biobear-0.6.0/pyproject.toml
+-rw-r--r--   0     1001      123      552 2023-06-15 15:55:52.000000 biobear-0.6.0/python/biobear/__init__.py
+-rw-r--r--   0     1001      123     1358 2023-06-15 15:55:52.000000 biobear-0.6.0/python/biobear/bam_reader.py
+-rw-r--r--   0     1001      123      720 2023-06-15 15:55:52.000000 biobear-0.6.0/python/biobear/compression.py
+-rw-r--r--   0     1001      123      931 2023-06-15 15:55:52.000000 biobear-0.6.0/python/biobear/fasta_reader.py
+-rw-r--r--   0     1001      123      927 2023-06-15 15:55:52.000000 biobear-0.6.0/python/biobear/fastq_reader.py
+-rw-r--r--   0     1001      123      787 2023-06-15 15:55:52.000000 biobear-0.6.0/python/biobear/genbank_reader.py
+-rw-r--r--   0     1001      123     1390 2023-06-15 15:55:52.000000 biobear-0.6.0/python/biobear/gff_reader.py
+-rw-r--r--   0     1001      123      941 2023-06-15 15:55:52.000000 biobear-0.6.0/python/biobear/reader.py
+-rw-r--r--   0     1001      123     1415 2023-06-15 15:55:52.000000 biobear-0.6.0/python/biobear/vcf_reader.py
+-rw-r--r--   0     1001      123   124562 2023-06-15 15:55:52.000000 biobear-0.6.0/python/tests/data/BGC0000404.gbk
+-rw-r--r--   0     1001      123     6152 2023-06-15 15:55:52.000000 biobear-0.6.0/python/tests/data/bedcov.bam
+-rw-r--r--   0     1001      123     7608 2023-06-15 15:55:52.000000 biobear-0.6.0/python/tests/data/bedcov.bam.bai
+-rw-r--r--   0     1001      123     1749 2023-06-15 15:55:52.000000 biobear-0.6.0/python/tests/data/file.vcf
+-rw-r--r--   0     1001      123     8638 2023-06-15 15:55:52.000000 biobear-0.6.0/python/tests/data/index.vcf.gz
+-rw-r--r--   0     1001      123      213 2023-06-15 15:55:52.000000 biobear-0.6.0/python/tests/data/index.vcf.gz.tbi
+-rw-r--r--   0     1001      123       41 2023-06-15 15:55:52.000000 biobear-0.6.0/python/tests/data/test.fasta
+-rw-r--r--   0     1001      123       58 2023-06-15 15:55:52.000000 biobear-0.6.0/python/tests/data/test.fasta.gz
+-rw-r--r--   0     1001      123      286 2023-06-15 15:55:52.000000 biobear-0.6.0/python/tests/data/test.fastq
+-rw-r--r--   0     1001      123      134 2023-06-15 15:55:52.000000 biobear-0.6.0/python/tests/data/test.fastq.gz
+-rw-r--r--   0     1001      123      112 2023-06-15 15:55:52.000000 biobear-0.6.0/python/tests/data/test.gff
+-rw-r--r--   0     1001      123       91 2023-06-15 15:55:52.000000 biobear-0.6.0/python/tests/data/test.gff.gz
+-rw-r--r--   0     1001      123     4302 2023-06-15 15:55:52.000000 biobear-0.6.0/python/tests/data/vcf_file.vcf
+-rw-r--r--   0     1001      123     1669 2023-06-15 15:55:52.000000 biobear-0.6.0/python/tests/data/vcf_file.vcf.gz
+-rw-r--r--   0     1001      123      254 2023-06-15 15:55:52.000000 biobear-0.6.0/python/tests/data/vcf_file.vcf.gz.tbi
+-rw-r--r--   0     1001      123      674 2023-06-15 15:55:52.000000 biobear-0.6.0/python/tests/test_bam_reader.py
+-rw-r--r--   0     1001      123     1218 2023-06-15 15:55:52.000000 biobear-0.6.0/python/tests/test_fasta_reader.py
+-rw-r--r--   0     1001      123     1154 2023-06-15 15:55:52.000000 biobear-0.6.0/python/tests/test_fastq_reader.py
+-rw-r--r--   0     1001      123      421 2023-06-15 15:55:52.000000 biobear-0.6.0/python/tests/test_genbank_reader.py
+-rw-r--r--   0     1001      123     1241 2023-06-15 15:55:52.000000 biobear-0.6.0/python/tests/test_gff_reader.py
+-rw-r--r--   0     1001      123      755 2023-06-15 15:55:52.000000 biobear-0.6.0/python/tests/test_vcf_reader.py
+-rw-r--r--   0     1001      123       20 2023-06-15 15:55:52.000000 biobear-0.6.0/requirements-dev.txt
+-rw-r--r--   0     1001      123     2766 2023-06-15 15:55:52.000000 biobear-0.6.0/src/bam_reader.rs
+-rw-r--r--   0     1001      123     5217 2023-06-15 15:55:52.000000 biobear-0.6.0/src/exon_reader.rs
+-rw-r--r--   0     1001      123      307 2023-06-15 15:55:52.000000 biobear-0.6.0/src/lib.rs
+-rw-r--r--   0     1001      123     2605 2023-06-15 15:55:52.000000 biobear-0.6.0/src/vcf_reader.rs
+-rw-r--r--   0     1001      123    91472 2023-06-15 15:56:01.000000 biobear-0.6.0/Cargo.lock
+-rw-r--r--   0        0        0    17081 1970-01-01 00:00:00.000000 biobear-0.6.0/PKG-INFO
```

### Comparing `biobear-0.5.0/.github/workflows/release.yml` & `biobear-0.6.0/.github/workflows/release.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,109 +1,109 @@
 name: Release
 
 on:
   push:
     tags:
-      - 'v*'
+    - 'v*'
 
 permissions:
   contents: read
 
 jobs:
   linux:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         target: [x86_64, aarch64, armv7]
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
-        with:
-          python-version: '3.10'
-      - name: Build wheels
-        uses: PyO3/maturin-action@v1
-        with:
-          target: ${{ matrix.target }}
-          args: --release --out dist --find-interpreter
-          sccache: 'true'
-          manylinux: auto
-      - name: Upload wheels
-        uses: actions/upload-artifact@v3
-        with:
-          name: wheels
-          path: dist
+    - uses: actions/checkout@v3
+    - uses: actions/setup-python@v4
+      with:
+        python-version: '3.10'
+    - name: Build wheels
+      uses: PyO3/maturin-action@v1
+      with:
+        target: ${{ matrix.target }}
+        args: --release --out dist --find-interpreter
+        sccache: 'true'
+        manylinux: auto
+    - name: Upload wheels
+      uses: actions/upload-artifact@v3
+      with:
+        name: wheels
+        path: dist
 
   windows:
     runs-on: windows-latest
     strategy:
       matrix:
         target: [x64, x86]
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
-        with:
-          python-version: '3.10'
-          architecture: ${{ matrix.target }}
-      - name: Build wheels
-        uses: PyO3/maturin-action@v1
-        with:
-          target: ${{ matrix.target }}
-          args: --release --out dist --find-interpreter
-          sccache: 'true'
-      - name: Upload wheels
-        uses: actions/upload-artifact@v3
-        with:
-          name: wheels
-          path: dist
+    - uses: actions/checkout@v3
+    - uses: actions/setup-python@v4
+      with:
+        python-version: '3.10'
+        architecture: ${{ matrix.target }}
+    - name: Build wheels
+      uses: PyO3/maturin-action@v1
+      with:
+        target: ${{ matrix.target }}
+        args: --release --out dist --find-interpreter
+        sccache: 'true'
+    - name: Upload wheels
+      uses: actions/upload-artifact@v3
+      with:
+        name: wheels
+        path: dist
 
   macos:
     runs-on: macos-latest
     strategy:
       matrix:
         target: [x86_64, aarch64]
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
-        with:
-          python-version: '3.10'
-      - name: Build wheels
-        uses: PyO3/maturin-action@v1
-        with:
-          target: ${{ matrix.target }}
-          args: --release --out dist --find-interpreter
-          sccache: 'true'
-      - name: Upload wheels
-        uses: actions/upload-artifact@v3
-        with:
-          name: wheels
-          path: dist
+    - uses: actions/checkout@v3
+    - uses: actions/setup-python@v4
+      with:
+        python-version: '3.10'
+    - name: Build wheels
+      uses: PyO3/maturin-action@v1
+      with:
+        target: ${{ matrix.target }}
+        args: --release --out dist --find-interpreter
+        sccache: 'true'
+    - name: Upload wheels
+      uses: actions/upload-artifact@v3
+      with:
+        name: wheels
+        path: dist
 
   sdist:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
-      - name: Build sdist
-        uses: PyO3/maturin-action@v1
-        with:
-          command: sdist
-          args: --out dist
-      - name: Upload sdist
-        uses: actions/upload-artifact@v3
-        with:
-          name: wheels
-          path: dist
+    - uses: actions/checkout@v3
+    - name: Build sdist
+      uses: PyO3/maturin-action@v1
+      with:
+        command: sdist
+        args: --out dist
+    - name: Upload sdist
+      uses: actions/upload-artifact@v3
+      with:
+        name: wheels
+        path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     needs: [linux, windows, macos, sdist]
     steps:
-      - uses: actions/download-artifact@v3
-        with:
-          name: wheels
-      - name: Publish to PyPI
-        uses: PyO3/maturin-action@v1
-        env:
-          MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
-        with:
-          command: upload
-          args: --skip-existing *
+    - uses: actions/download-artifact@v3
+      with:
+        name: wheels
+    - name: Publish to PyPI
+      uses: PyO3/maturin-action@v1
+      env:
+        MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
+      with:
+        command: upload
+        args: --skip-existing *
```

### Comparing `biobear-0.5.0/.github/workflows/smoke-test.yml` & `biobear-0.6.0/.github/workflows/smoke-test.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # Create a smoketest that just installs the biobear python package and reads an example file
 
 name: Smoke Test
 
 on:
-    workflow_dispatch:
+  workflow_dispatch:
 
 
 jobs:
-    test-package:
-        runs-on: ${{ matrix.os }}
-        strategy:
-            matrix:
-                os: [ubuntu-latest, macos-latest, windows-latest]
-                python-version: [3.9, "3.10", 3.11]
-        steps:
-            - name: Checkout
-              uses: actions/checkout@v2
-
-            - uses: actions/setup-python@v2
-              with:
-                  python-version: ${{ matrix.python-version }}
-
-            - name: Install biobear
-              run: |
-                  python -m pip install --upgrade pip
-                  pip install biobear
-
-            - name: Read example fasta file
-              shell: bash
-              run: |
-                python ./.github/workflows/smoketest.py
+  test-package:
+    runs-on: ${{ matrix.os }}
+    strategy:
+      matrix:
+        os: [ubuntu-latest, macos-latest, windows-latest]
+        python-version: [3.11]
+    steps:
+    - name: Checkout
+      uses: actions/checkout@v2
+
+    - uses: actions/setup-python@v2
+      with:
+        python-version: ${{ matrix.python-version }}
+
+    - name: Install biobear
+      run: |
+        python -m pip install --upgrade pip
+        pip install biobear
+
+    - name: Read example fasta file
+      shell: bash
+      run: |
+        python ./.github/workflows/smoketest.py
```

### Comparing `biobear-0.5.0/.github/workflows/test.yml` & `biobear-0.6.0/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 name: Test
 
 on:
-    push:
-        branches:
-            - main
-    pull_request:
-        branches:
-            - main
+  push:
+    branches:
+    - main
+  pull_request:
+    branches:
+    - main
 
 jobs:
-    test:
-        runs-on: ubuntu-latest
-        steps:
-            - uses: actions/checkout@v2
-
-            - uses: actions-rs/toolchain@v1
-              with:
-                  toolchain: stable
-
-            - uses: actions/setup-python@v2
-              with:
-                  python-version: '3.9'
-
-            - name: Run clippy
-              run: cargo clippy --all-targets --all-features -- -D warnings
-
-            # setup a virtual environment
-            - name: Setup Python and Run Tests
-              run: |
-                  python -m pip install --upgrade pip
-                  pip install virtualenv
-                  virtualenv venv
-                  source venv/bin/activate
-                  pip install -r requirements-dev.txt
-                  cargo build
-                  maturin develop
+  test:
+    runs-on: ubuntu-latest
+    steps:
+    - uses: actions/checkout@v2
+
+    - uses: actions-rs/toolchain@v1
+      with:
+        toolchain: stable
+
+    - uses: actions/setup-python@v2
+      with:
+        python-version: '3.9'
+
+    - name: Run clippy
+      run: cargo clippy --all-targets --all-features -- -D warnings
+
+    # setup a virtual environment
+    - name: Setup Python and Run Tests
+      run: |
+        python -m pip install --upgrade pip
+        pip install virtualenv
+        virtualenv venv
+        source venv/bin/activate
+        pip install -r requirements-dev.txt
+        cargo build
+        maturin develop
 
-                  ruff check python/
-                  pytest
+        ruff check python/
+        pytest
```

### Comparing `biobear-0.5.0/.gitignore` & `biobear-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `biobear-0.5.0/LICENSE` & `biobear-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobear-0.5.0/README.md` & `biobear-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-# biobear (v0.5.0)
+# biobear (v0.6.0)
 
 biobear is a Python library designed for reading and searching bioinformatic file formats, using Rust as its backend and producing Arrow or Polars DataFrames as its output.
 
 The python package has minimal dependencies and only requires Polars. Biobear can be used to read various bioinformatic file formats, including FASTA, FASTQ, VCF, BAM, and GFF. It can also query some indexed file formats, including VCF and BAM.
 
 - [Installation](#installation)
 - [Usage](#usage)
+- [S3 and GCS](#s3-and-gcs)
 - [Similar Packages](#similar-packages)
 - [API Documentation](#api-documentation)
   - [vcf\_reader](#vcf_reader)
     - [VCFReader](#vcfreader)
     - [VCFIndexedReader](#vcfindexedreader)
   - [genbank\_reader](#genbank_reader)
     - [GenbankReader](#genbankreader)
@@ -104,14 +105,25 @@
 # │ 1          ┆ 3000151  ┆       ┆ C         ┆ … ┆ 59.200001     ┆ PASS   ┆ AN=4;AC=2                         ┆ GT:DP:GQ       │
 # │ 1          ┆ 3062915  ┆ id3D  ┆ GTTT      ┆ … ┆ 12.9          ┆ q10    ┆ DP4=1,2,3,4;AN=4;AC=2;INDEL;STR=… ┆ GT:GQ:DP:GL    │
 # │ 1          ┆ 3062915  ┆ idSNP ┆ G         ┆ … ┆ 12.6          ┆ test   ┆ TEST=5;DP4=1,2,3,4;AN=3;AC=1,1    ┆ GT:TT:GQ:DP:GL │
 # │ 1          ┆ 3106154  ┆       ┆ CAAA      ┆ … ┆ 342.0         ┆ PASS   ┆ AN=4;AC=2                         ┆ GT:GQ:DP       │
 # └────────────┴──────────┴───────┴───────────┴───┴───────────────┴────────┴───────────────────────────────────┴────────────────┘
 ```
 
+## S3 and GCS
+
+If you pass a `path` that is a URL to an object store, BioBear will attempt to infer your credentials from the environment, and use them to read the file. For example, if you have your `AWS_PROFILE` and `AWS_REGION` env vars set, then you can read from S3 like so:
+
+```python
+import biobear as bb
+
+# Read from S3
+df = bb.FastaReader("s3://bucket/test.fa").read()
+```
+
 ## Similar Packages
 
 Similar packages and/or inspiration for this package:
 
 - https://github.com/abdenlab/saimin/
 - https://github.com/tshauck/brrrr/
 - https://github.com/natir/vcf2parquet/
```

### Comparing `biobear-0.5.0/pyproject.toml` & `biobear-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `biobear-0.5.0/python/biobear/__init__.py` & `biobear-0.6.0/python/biobear/__init__.py`

 * *Files identical despite different names*

### Comparing `biobear-0.5.0/python/biobear/bam_reader.py` & `biobear-0.6.0/python/biobear/bam_reader.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 import os
 
 import polars as pl
 import pyarrow.dataset as ds
 
 from biobear.reader import Reader
-from .biobear import _BamIndexedReader, _BamReader
+from .biobear import _BamIndexedReader, _ExonReader
 
 
 class BamReader(Reader):
     """A BAM File Reader."""
 
     def __init__(self, path: os.PathLike):
         """Initialize the BamReader.
 
         Args:
             path (Path): Path to the BAM file.
 
         """
-        self._bam_reader = _BamReader(str(path))
+        self._bam_reader = _ExonReader(str(path), "BAM", None)
 
     @property
     def inner(self):
         """Return the inner reader."""
         return self._bam_reader
```

### Comparing `biobear-0.5.0/python/biobear/compression.py` & `biobear-0.6.0/python/biobear/compression.py`

 * *Files identical despite different names*

### Comparing `biobear-0.5.0/python/biobear/fasta_reader.py` & `biobear-0.6.0/python/biobear/fasta_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.5.0/python/biobear/fastq_reader.py` & `biobear-0.6.0/python/biobear/fastq_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.5.0/python/biobear/genbank_reader.py` & `biobear-0.6.0/python/biobear/genbank_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.5.0/python/biobear/gff_reader.py` & `biobear-0.6.0/python/biobear/gff_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.5.0/python/biobear/reader.py` & `biobear-0.6.0/python/biobear/reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.5.0/python/biobear/vcf_reader.py` & `biobear-0.6.0/python/biobear/vcf_reader.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 import polars as pl
 import pyarrow.dataset as ds
 
 from biobear.reader import Reader
 
-from .biobear import _VCFReader, _VCFIndexedReader
+from .biobear import _ExonReader, _VCFIndexedReader
 
 
 class VCFReader(Reader):
     """A VCF File Reader.
 
     This class is used to read a VCF file and convert it to a polars DataFrame.
     """
@@ -19,15 +19,15 @@
     def __init__(self, path: os.PathLike):
         """Initialize the VCFReader.
 
         Args:
             path (Path): Path to the VCF file.
 
         """
-        self._vcf_reader = _VCFReader(str(path))
+        self._vcf_reader = _ExonReader(str(path), "VCF", None)
 
     @property
     def inner(self):
         """Return the inner reader."""
         return self._vcf_reader
```

### Comparing `biobear-0.5.0/python/tests/data/BGC0000404.gbk` & `biobear-0.6.0/python/tests/data/BGC0000404.gbk`

 * *Files identical despite different names*

### Comparing `biobear-0.5.0/python/tests/data/bedcov.bam` & `biobear-0.6.0/python/tests/data/bedcov.bam`

 * *Files identical despite different names*

### Comparing `biobear-0.5.0/python/tests/data/bedcov.bam.bai` & `biobear-0.6.0/python/tests/data/bedcov.bam.bai`

 * *Files identical despite different names*

### Comparing `biobear-0.5.0/python/tests/data/file.vcf` & `biobear-0.6.0/python/tests/data/file.vcf`

 * *Files identical despite different names*

### Comparing `biobear-0.5.0/python/tests/data/index.vcf.gz` & `biobear-0.6.0/python/tests/data/index.vcf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.5.0/python/tests/data/vcf_file.vcf` & `biobear-0.6.0/python/tests/data/vcf_file.vcf`

 * *Files identical despite different names*

### Comparing `biobear-0.5.0/python/tests/data/vcf_file.vcf.gz` & `biobear-0.6.0/python/tests/data/vcf_file.vcf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.5.0/python/tests/test_bam_reader.py` & `biobear-0.6.0/python/tests/test_bam_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.5.0/python/tests/test_fasta_reader.py` & `biobear-0.6.0/python/tests/test_fasta_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.5.0/python/tests/test_fastq_reader.py` & `biobear-0.6.0/python/tests/test_fastq_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.5.0/python/tests/test_gff_reader.py` & `biobear-0.6.0/python/tests/test_gff_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.5.0/python/tests/test_vcf_reader.py` & `biobear-0.6.0/python/tests/test_vcf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.5.0/src/bam_reader.rs` & `biobear-0.6.0/src/bam_reader.rs`

 * *Files 24% similar despite different names*

```diff
@@ -8,83 +8,14 @@
 use pyo3::prelude::*;
 
 use tokio::runtime::Runtime;
 
 use std::io;
 use std::sync::Arc;
 
-#[pyclass(name = "_BamReader")]
-pub struct BamReader {
-    df: datafusion::dataframe::DataFrame,
-    _runtime: Arc<Runtime>,
-}
-
-impl BamReader {
-    fn open(path: &str, batch_size: Option<usize>) -> io::Result<Self> {
-        let rt = Arc::new(Runtime::new().unwrap());
-
-        let mut config = SessionConfig::new();
-        if let Some(batch_size) = batch_size {
-            config = config.with_batch_size(batch_size);
-        }
-
-        let ctx = SessionContext::with_config(config);
-
-        let df = rt.block_on(async {
-            match ctx.read_bam(path, None).await {
-                Ok(df) => Ok(df),
-                Err(e) => Err(io::Error::new(
-                    io::ErrorKind::Other,
-                    format!("Error reading BAM file: {e}"),
-                )),
-            }
-        });
-
-        match df {
-            Ok(df) => Ok(Self { df, _runtime: rt }),
-            Err(e) => Err(e),
-        }
-    }
-}
-
-#[pymethods]
-impl BamReader {
-    #[new]
-    fn py_new(path: &str, batch_size: Option<usize>) -> PyResult<Self> {
-        Self::open(path, batch_size).map_err(|e| {
-            PyErr::new::<pyo3::exceptions::PyIOError, _>(format!(
-                "Failed to open file: {path} with error: {e}",
-            ))
-        })
-    }
-
-    fn to_pyarrow(&self) -> PyResult<PyObject> {
-        let stream = Arc::new(FFI_ArrowArrayStream::empty());
-        let stream_ptr = Arc::into_raw(stream) as *mut FFI_ArrowArrayStream;
-
-        self._runtime.block_on(async {
-            create_dataset_stream_from_table_provider(
-                self.df.clone(),
-                self._runtime.clone(),
-                stream_ptr,
-            )
-            .await;
-        });
-
-        Python::with_gil(|py| unsafe {
-            match ArrowArrayStreamReader::from_raw(stream_ptr) {
-                Ok(stream_reader) => stream_reader.to_pyarrow(py),
-                Err(err) => Err(PyErr::new::<pyo3::exceptions::PyValueError, _>(format!(
-                    "Error converting to pyarrow: {err}"
-                ))),
-            }
-        })
-    }
-}
-
 #[pyclass(name = "_BamIndexedReader")]
 pub struct BamIndexedReader {
     path: String,
     batch_size: Option<usize>,
     _runtime: Arc<Runtime>,
 }
```

### Comparing `biobear-0.5.0/src/exon_reader.rs` & `biobear-0.6.0/src/vcf_reader.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,99 +1,78 @@
-use std::io::{self};
-use std::str::FromStr;
-use std::sync::Arc;
-
-use arrow::ffi_stream::{ArrowArrayStreamReader, FFI_ArrowArrayStream};
-use arrow::pyarrow::PyArrowConvert;
-use datafusion::datasource::file_format::file_type::FileCompressionType;
+use arrow::{
+    ffi_stream::{ArrowArrayStreamReader, FFI_ArrowArrayStream},
+    pyarrow::PyArrowConvert,
+};
 use datafusion::prelude::{SessionConfig, SessionContext};
-use exon::context::ExonSessionExt;
-use exon::datasources::ExonFileType;
-use exon::ffi::create_dataset_stream_from_table_provider;
 use pyo3::prelude::*;
 use tokio::runtime::Runtime;
 
-#[pyclass(name = "_ExonReader")]
-pub struct ExonReader {
-    df: datafusion::dataframe::DataFrame,
+use exon::{context::ExonSessionExt, ffi::create_dataset_stream_from_table_provider};
+
+use std::io;
+use std::sync::Arc;
+
+#[pyclass(name = "_VCFIndexedReader")]
+pub struct VCFIndexedReader {
+    path: String,
+    batch_size: Option<usize>,
     _runtime: Arc<Runtime>,
 }
 
-impl ExonReader {
-    fn open(
-        path: &str,
-        file_type: ExonFileType,
-        compression: Option<FileCompressionType>,
-        batch_size: Option<usize>,
-    ) -> io::Result<Self> {
+impl VCFIndexedReader {
+    fn open(path: &str, batch_size: Option<usize>) -> io::Result<Self> {
+        // Check the path exists
+        if !std::path::Path::new(path).exists() {
+            return Err(io::Error::new(
+                io::ErrorKind::NotFound,
+                format!("File not found: {path}"),
+            ));
+        }
+
         let rt = Arc::new(Runtime::new().unwrap());
 
+        Ok(Self {
+            path: path.to_string(),
+            batch_size,
+            _runtime: rt,
+        })
+    }
+}
+
+#[pymethods]
+impl VCFIndexedReader {
+    #[new]
+    fn new(path: &str, batch_size: Option<usize>) -> PyResult<Self> {
+        Self::open(path, batch_size).map_err(PyErr::new::<pyo3::exceptions::PyValueError, _>)
+    }
+
+    fn query(&mut self, region: &str) -> PyResult<PyObject> {
         let mut config = SessionConfig::new();
-        if let Some(batch_size) = batch_size {
+        if let Some(batch_size) = self.batch_size {
             config = config.with_batch_size(batch_size);
         }
 
         let ctx = SessionContext::with_config(config);
 
-        let df = rt.block_on(async {
-            match ctx.read_exon_table(path, file_type, compression).await {
+        let df = self._runtime.block_on(async {
+            match ctx.query_vcf_file(self.path.as_str(), region).await {
                 Ok(df) => Ok(df),
                 Err(e) => Err(io::Error::new(
                     io::ErrorKind::Other,
-                    format!("Error reading GFF file: {e}"),
+                    format!("Error reading VCF file: {e}"),
                 )),
             }
-        });
-
-        match df {
-            Ok(df) => Ok(Self { df, _runtime: rt }),
-            Err(e) => Err(e),
-        }
-    }
-}
-
-#[pymethods]
-impl ExonReader {
-    #[new]
-    fn new(
-        path: &str,
-        file_type: &str,
-        compression: Option<&str>,
-        batch_size: Option<usize>,
-    ) -> PyResult<Self> {
-        let exon_file_type = ExonFileType::from_str(file_type).map_err(|e| {
-            PyErr::new::<pyo3::exceptions::PyValueError, _>(format!(
-                "Error reading file type: {e:?}"
-            ))
         })?;
 
-        let file_compression_type =
-            compression.map(
-                |compression| match FileCompressionType::from_str(compression) {
-                    Ok(compression_type) => Ok(compression_type),
-                    Err(e) => Err(PyErr::new::<pyo3::exceptions::PyValueError, _>(format!(
-                        "Error reading compression type: {e:?}"
-                    ))),
-                },
-            );
-
-        let file_compression_type = file_compression_type.transpose()?;
-
-        Self::open(path, exon_file_type, file_compression_type, batch_size).map_err(|e| {
-            PyErr::new::<pyo3::exceptions::PyIOError, _>(format!("Error opening file {path}: {e}"))
-        })
-    }
-
-    fn to_pyarrow(&self) -> PyResult<PyObject> {
         let stream = Arc::new(FFI_ArrowArrayStream::empty());
         let stream_ptr = Arc::into_raw(stream) as *mut FFI_ArrowArrayStream;
 
         self._runtime.block_on(async {
             create_dataset_stream_from_table_provider(
-                self.df.clone(),
+                df.clone(),
                 self._runtime.clone(),
                 stream_ptr,
             )
             .await;
         });
 
         Python::with_gil(|py| unsafe {
```

### Comparing `biobear-0.5.0/Cargo.lock` & `biobear-0.6.0/Cargo.lock`

 * *Files 11% similar despite different names*

```diff
@@ -318,28 +318,326 @@
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
+name = "aws-config"
+version = "0.54.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3c3d1e2a1f1ab3ac6c4b884e37413eaa03eb9d901e4fc68ee8f5c1d49721680e"
+dependencies = [
+ "aws-credential-types",
+ "aws-http",
+ "aws-sdk-sso",
+ "aws-sdk-sts",
+ "aws-smithy-async",
+ "aws-smithy-client",
+ "aws-smithy-http",
+ "aws-smithy-http-tower",
+ "aws-smithy-json",
+ "aws-smithy-types",
+ "aws-types",
+ "bytes",
+ "hex",
+ "http",
+ "hyper",
+ "ring",
+ "time",
+ "tokio",
+ "tower",
+ "tracing",
+ "zeroize",
+]
+
+[[package]]
+name = "aws-credential-types"
+version = "0.54.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bb0696a0523a39a19087747e4dafda0362dc867531e3d72a3f195564c84e5e08"
+dependencies = [
+ "aws-smithy-async",
+ "aws-smithy-types",
+ "tokio",
+ "tracing",
+ "zeroize",
+]
+
+[[package]]
+name = "aws-endpoint"
+version = "0.54.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "80a4f935ab6a1919fbfd6102a80c4fccd9ff5f47f94ba154074afe1051903261"
+dependencies = [
+ "aws-smithy-http",
+ "aws-smithy-types",
+ "aws-types",
+ "http",
+ "regex",
+ "tracing",
+]
+
+[[package]]
+name = "aws-http"
+version = "0.54.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "82976ca4e426ee9ca3ffcf919d9b2c8d14d0cd80d43cc02173737a8f07f28d4d"
+dependencies = [
+ "aws-credential-types",
+ "aws-smithy-http",
+ "aws-smithy-types",
+ "aws-types",
+ "bytes",
+ "http",
+ "http-body",
+ "lazy_static",
+ "percent-encoding",
+ "pin-project-lite",
+ "tracing",
+]
+
+[[package]]
+name = "aws-sdk-sso"
+version = "0.24.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca0119bacf0c42f587506769390983223ba834e605f049babe514b2bd646dbb2"
+dependencies = [
+ "aws-credential-types",
+ "aws-endpoint",
+ "aws-http",
+ "aws-sig-auth",
+ "aws-smithy-async",
+ "aws-smithy-client",
+ "aws-smithy-http",
+ "aws-smithy-http-tower",
+ "aws-smithy-json",
+ "aws-smithy-types",
+ "aws-types",
+ "bytes",
+ "http",
+ "regex",
+ "tokio-stream",
+ "tower",
+]
+
+[[package]]
+name = "aws-sdk-sts"
+version = "0.24.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "270b6a33969ebfcb193512fbd5e8ee5306888ad6c6d5d775cdbfb2d50d94de26"
+dependencies = [
+ "aws-credential-types",
+ "aws-endpoint",
+ "aws-http",
+ "aws-sig-auth",
+ "aws-smithy-async",
+ "aws-smithy-client",
+ "aws-smithy-http",
+ "aws-smithy-http-tower",
+ "aws-smithy-json",
+ "aws-smithy-query",
+ "aws-smithy-types",
+ "aws-smithy-xml",
+ "aws-types",
+ "bytes",
+ "http",
+ "regex",
+ "tower",
+ "tracing",
+]
+
+[[package]]
+name = "aws-sig-auth"
+version = "0.54.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "660a02a98ab1af83bd8d714afbab2d502ba9b18c49e7e4cddd6bf8837ff778cb"
+dependencies = [
+ "aws-credential-types",
+ "aws-sigv4",
+ "aws-smithy-http",
+ "aws-types",
+ "http",
+ "tracing",
+]
+
+[[package]]
+name = "aws-sigv4"
+version = "0.54.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "86529e7b64d902efea8fff52c1b2529368d04f90305cf632729e3713f6b57dc0"
+dependencies = [
+ "aws-smithy-http",
+ "form_urlencoded",
+ "hex",
+ "hmac",
+ "http",
+ "once_cell",
+ "percent-encoding",
+ "regex",
+ "sha2",
+ "time",
+ "tracing",
+]
+
+[[package]]
+name = "aws-smithy-async"
+version = "0.54.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "63c712a28a4f2f2139759235c08bf98aca99d4fdf1b13c78c5f95613df0a5db9"
+dependencies = [
+ "futures-util",
+ "pin-project-lite",
+ "tokio",
+ "tokio-stream",
+]
+
+[[package]]
+name = "aws-smithy-client"
+version = "0.54.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "104ca17f56cde00a10207169697dfe9c6810db339d52fb352707e64875b30a44"
+dependencies = [
+ "aws-smithy-async",
+ "aws-smithy-http",
+ "aws-smithy-http-tower",
+ "aws-smithy-types",
+ "bytes",
+ "fastrand",
+ "http",
+ "http-body",
+ "hyper",
+ "hyper-rustls 0.23.2",
+ "lazy_static",
+ "pin-project-lite",
+ "tokio",
+ "tower",
+ "tracing",
+]
+
+[[package]]
+name = "aws-smithy-http"
+version = "0.54.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "873f316f1833add0d3aa54ed1b0cd252ddd88c792a0cf839886400099971e844"
+dependencies = [
+ "aws-smithy-types",
+ "bytes",
+ "bytes-utils",
+ "futures-core",
+ "http",
+ "http-body",
+ "hyper",
+ "once_cell",
+ "percent-encoding",
+ "pin-project-lite",
+ "pin-utils",
+ "tracing",
+]
+
+[[package]]
+name = "aws-smithy-http-tower"
+version = "0.54.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4f38231d3f5dac9ac7976f44e12803add1385119ffca9e5f050d8e980733d164"
+dependencies = [
+ "aws-smithy-http",
+ "aws-smithy-types",
+ "bytes",
+ "http",
+ "http-body",
+ "pin-project-lite",
+ "tower",
+ "tracing",
+]
+
+[[package]]
+name = "aws-smithy-json"
+version = "0.54.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4bd83ff2b79e9f729746fcc8ad798676b68fe6ea72986571569a5306a277a182"
+dependencies = [
+ "aws-smithy-types",
+]
+
+[[package]]
+name = "aws-smithy-query"
+version = "0.54.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a2f0445dafe9d2cd50b44339ae3c3ed46549aad8ac696c52ad660b3e7ae8682b"
+dependencies = [
+ "aws-smithy-types",
+ "urlencoding",
+]
+
+[[package]]
+name = "aws-smithy-types"
+version = "0.54.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8161232eda10290f5136610a1eb9de56aceaccd70c963a26a260af20ac24794f"
+dependencies = [
+ "base64-simd",
+ "itoa",
+ "num-integer",
+ "ryu",
+ "time",
+]
+
+[[package]]
+name = "aws-smithy-xml"
+version = "0.54.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "343ffe9a9bb3f542675f4df0e0d5933513d6ad038ca3907ad1767ba690a99684"
+dependencies = [
+ "xmlparser",
+]
+
+[[package]]
+name = "aws-types"
+version = "0.54.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f8f15b34253b68cde08e39b0627cc6101bcca64351229484b4743392c035d057"
+dependencies = [
+ "aws-credential-types",
+ "aws-smithy-async",
+ "aws-smithy-client",
+ "aws-smithy-http",
+ "aws-smithy-types",
+ "http",
+ "rustc_version",
+ "tracing",
+]
+
+[[package]]
 name = "base64"
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
 
 [[package]]
+name = "base64-simd"
+version = "0.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "339abbe78e73178762e23bea9dfd08e697eb3f3301cd4be981c0f78ba5859195"
+dependencies = [
+ "outref",
+ "vsimd",
+]
+
+[[package]]
 name = "biobear"
-version = "0.5.0"
+version = "0.6.0"
 dependencies = [
  "arrow",
  "datafusion",
  "exon",
+ "object_store",
  "pyo3",
  "tokio",
+ "url",
 ]
 
 [[package]]
 name = "bit-vec"
 version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "349f9b6a179ed607305526ca489b34ad0a41aed5f7980fa90eb03160b69598fb"
@@ -424,14 +722,24 @@
 [[package]]
 name = "bytes"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89b2fd2a0dcf38d7971e2194b6b6eebab45ae01067456a7fd93d5547a61b70be"
 
 [[package]]
+name = "bytes-utils"
+version = "0.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e47d3a8076e283f3acd27400535992edb3ba4b5bb72f8891ad8fbe7932a7d4b9"
+dependencies = [
+ "bytes",
+ "either",
+]
+
+[[package]]
 name = "bzip2"
 version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bdb116a6ef3f6c3698828873ad02c3014b3c85cadb88496095628e3ef1e347f8"
 dependencies = [
  "bzip2-sys",
  "libc",
@@ -468,14 +776,15 @@
 version = "0.4.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "num-traits",
+ "serde",
  "winapi",
 ]
 
 [[package]]
 name = "chrono-tz"
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -539,14 +848,24 @@
 [[package]]
 name = "constant_time_eq"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "21a53c0a4d288377e7415b53dcfc3c04da5cdc2cc95c8d5ac178b58f0b861ad6"
 
 [[package]]
+name = "core-foundation"
+version = "0.9.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "194a7a9e6de53fa55116934067c844d9d749312f75c6f6d0980e8c252f8c2146"
+dependencies = [
+ "core-foundation-sys",
+ "libc",
+]
+
+[[package]]
 name = "core-foundation-sys"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpufeatures"
@@ -830,14 +1149,23 @@
 [[package]]
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
+name = "encoding_rs"
+version = "0.8.32"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "071a31f4ee85403370b58aca746f01041ede6f0da2730960ad001edc2b71b394"
+dependencies = [
+ "cfg-if",
+]
+
+[[package]]
 name = "err-derive"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c34a887c8df3ed90498c1c437ce21f211c8e27672921a8ffa293cb8d6d4caa9e"
 dependencies = [
  "proc-macro-error",
  "proc-macro2",
@@ -851,15 +1179,15 @@
 name = "errno"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "errno-dragonfly"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
@@ -924,14 +1252,20 @@
 checksum = "3b9429470923de8e8cbd4d2dc513535400b4b3fef0319fb5c4e1f520a7bef743"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
+name = "fnv"
+version = "1.0.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
+
+[[package]]
 name = "form_urlencoded"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
 dependencies = [
  "percent-encoding",
 ]
@@ -1066,14 +1400,33 @@
 [[package]]
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
+name = "h2"
+version = "0.3.19"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d357c7ae988e7d2182f7d7871d0b963962420b0678b0997ce7de72001aeab782"
+dependencies = [
+ "bytes",
+ "fnv",
+ "futures-core",
+ "futures-sink",
+ "futures-util",
+ "http",
+ "indexmap",
+ "slab",
+ "tokio",
+ "tokio-util",
+ "tracing",
+]
+
+[[package]]
 name = "half"
 version = "2.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "02b4af3693f1b705df946e9fe5631932443781d0aabb423b62fcd4d73f6d2fd0"
 dependencies = [
  "crunchy",
  "num-traits",
@@ -1112,14 +1465,115 @@
 [[package]]
 name = "hermit-abi"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
 
 [[package]]
+name = "hex"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
+
+[[package]]
+name = "hmac"
+version = "0.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6c49c37c09c17a53d937dfbb742eb3a961d65a994e6bcdcf37e7399d0cc8ab5e"
+dependencies = [
+ "digest",
+]
+
+[[package]]
+name = "http"
+version = "0.2.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bd6effc99afb63425aff9b05836f029929e345a6148a14b7ecd5ab67af944482"
+dependencies = [
+ "bytes",
+ "fnv",
+ "itoa",
+]
+
+[[package]]
+name = "http-body"
+version = "0.4.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d5f38f16d184e36f2408a55281cd658ecbd3ca05cce6d6510a176eca393e26d1"
+dependencies = [
+ "bytes",
+ "http",
+ "pin-project-lite",
+]
+
+[[package]]
+name = "httparse"
+version = "1.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d897f394bad6a705d5f4104762e116a75639e470d80901eed05a860a95cb1904"
+
+[[package]]
+name = "httpdate"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c4a1e36c821dbe04574f602848a19f742f4fb3c98d40449f11bcad18d6b17421"
+
+[[package]]
+name = "hyper"
+version = "0.14.26"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ab302d72a6f11a3b910431ff93aae7e773078c769f0a3ef15fb9ec692ed147d4"
+dependencies = [
+ "bytes",
+ "futures-channel",
+ "futures-core",
+ "futures-util",
+ "h2",
+ "http",
+ "http-body",
+ "httparse",
+ "httpdate",
+ "itoa",
+ "pin-project-lite",
+ "socket2",
+ "tokio",
+ "tower-service",
+ "tracing",
+ "want",
+]
+
+[[package]]
+name = "hyper-rustls"
+version = "0.23.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1788965e61b367cd03a62950836d5cd41560c3577d90e40e0819373194d1661c"
+dependencies = [
+ "http",
+ "hyper",
+ "log",
+ "rustls 0.20.8",
+ "rustls-native-certs",
+ "tokio",
+ "tokio-rustls 0.23.4",
+]
+
+[[package]]
+name = "hyper-rustls"
+version = "0.24.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0646026eb1b3eea4cd9ba47912ea5ce9cc07713d105b1a14698f4e6433d348b7"
+dependencies = [
+ "http",
+ "hyper",
+ "rustls 0.21.2",
+ "tokio",
+ "tokio-rustls 0.24.1",
+]
+
+[[package]]
 name = "iana-time-zone"
 version = "0.1.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2fad5b825842d2b38bd206f3e81d6957625fd7f0a361e345c30e01a0ae2dd613"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
@@ -1183,18 +1637,24 @@
 name = "io-lifetimes"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
 dependencies = [
  "hermit-abi 0.3.1",
  "libc",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "ipnet"
+version = "2.7.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "12b6ee2129af8d4fb011108c73d99a1b83a85977f23b82460c0ae2e25bb4b57f"
+
+[[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
@@ -1379,14 +1839,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "mime"
+version = "0.3.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
+
+[[package]]
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "miniz_oxide"
@@ -1394,14 +1860,25 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
+name = "mio"
+version = "0.8.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "927a765cd3fc26206e66b296465fa9d3e5ab003e651c1b3c060e7956d96b19d2"
+dependencies = [
+ "libc",
+ "wasi",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "new_debug_unreachable"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e4a24736216ec316047a1fc4252e27dabb04218aa4a3f37c6e7ddbf1f9782b54"
 
 [[package]]
 name = "nom"
@@ -1722,43 +2199,66 @@
 [[package]]
 name = "object_store"
 version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec9cd6ca25e796a49fa242876d1c4de36a24a6da5258e9f0bc062dbf5e81c53b"
 dependencies = [
  "async-trait",
+ "aws-config",
+ "aws-credential-types",
+ "aws-types",
+ "base64",
  "bytes",
  "chrono",
  "futures",
  "itertools",
  "parking_lot",
  "percent-encoding",
+ "quick-xml",
+ "rand",
+ "reqwest",
+ "ring",
+ "rustls-pemfile",
+ "serde",
+ "serde_json",
  "snafu",
  "tokio",
  "tracing",
  "url",
  "walkdir",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
+name = "openssl-probe"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
+
+[[package]]
 name = "ordered-float"
 version = "2.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7940cf2ca942593318d07fcf2596cdca60a85c9e7fab408a5e21a4f9dcd40d87"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
+name = "outref"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4030760ffd992bef45b0ae3f10ce1aba99e33464c90d14dd7c039884963ddc7a"
+
+[[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
@@ -2121,14 +2621,70 @@
 [[package]]
 name = "regex-syntax"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
+name = "reqwest"
+version = "0.11.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cde824a14b7c14f85caff81225f411faacc04a2013f41670f41443742b1c1c55"
+dependencies = [
+ "base64",
+ "bytes",
+ "encoding_rs",
+ "futures-core",
+ "futures-util",
+ "h2",
+ "http",
+ "http-body",
+ "hyper",
+ "hyper-rustls 0.24.0",
+ "ipnet",
+ "js-sys",
+ "log",
+ "mime",
+ "once_cell",
+ "percent-encoding",
+ "pin-project-lite",
+ "rustls 0.21.2",
+ "rustls-pemfile",
+ "serde",
+ "serde_json",
+ "serde_urlencoded",
+ "tokio",
+ "tokio-rustls 0.24.1",
+ "tokio-util",
+ "tower-service",
+ "url",
+ "wasm-bindgen",
+ "wasm-bindgen-futures",
+ "wasm-streams",
+ "web-sys",
+ "webpki-roots",
+ "winreg",
+]
+
+[[package]]
+name = "ring"
+version = "0.16.20"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3053cf52e236a3ed746dfc745aa9cacf1b791d846bdaf412f60a8d7d6e17c8fc"
+dependencies = [
+ "cc",
+ "libc",
+ "once_cell",
+ "spin",
+ "untrusted",
+ "web-sys",
+ "winapi",
+]
+
+[[package]]
 name = "rustc_version"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
@@ -2140,15 +2696,70 @@
 checksum = "b96e891d04aa506a6d1f318d2771bcb1c7dfda84e126660ace067c9b474bb2c0"
 dependencies = [
  "bitflags 1.3.2",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
- "windows-sys",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "rustls"
+version = "0.20.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fff78fc74d175294f4e83b28343315ffcfb114b156f0185e9741cb5570f50e2f"
+dependencies = [
+ "log",
+ "ring",
+ "sct",
+ "webpki",
+]
+
+[[package]]
+name = "rustls"
+version = "0.21.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e32ca28af694bc1bbf399c33a516dbdf1c90090b8ab23c2bc24f834aa2247f5f"
+dependencies = [
+ "log",
+ "ring",
+ "rustls-webpki",
+ "sct",
+]
+
+[[package]]
+name = "rustls-native-certs"
+version = "0.6.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a9aace74cb666635c918e9c12bc0d348266037aa8eb599b5cba565709a8dff00"
+dependencies = [
+ "openssl-probe",
+ "rustls-pemfile",
+ "schannel",
+ "security-framework",
+]
+
+[[package]]
+name = "rustls-pemfile"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d194b56d58803a43635bdc398cd17e383d6f71f9182b9a192c127ca42494a59b"
+dependencies = [
+ "base64",
+]
+
+[[package]]
+name = "rustls-webpki"
+version = "0.100.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d6207cd5ed3d8dca7816f8f3725513a34609c0c765bf652b8c3cb4cfd87db46b"
+dependencies = [
+ "ring",
+ "untrusted",
 ]
 
 [[package]]
 name = "rustversion"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
@@ -2165,20 +2776,62 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
+name = "schannel"
+version = "0.1.21"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "713cfb06c7059f3588fb8044c0fad1d09e3c01d225e25b9220dbfdcf16dbb1b3"
+dependencies = [
+ "windows-sys 0.42.0",
+]
+
+[[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
+name = "sct"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d53dcdb7c9f8158937a7981b48accfd39a43af418591a5d008c7b22b5e1b7ca4"
+dependencies = [
+ "ring",
+ "untrusted",
+]
+
+[[package]]
+name = "security-framework"
+version = "2.9.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1fc758eb7bffce5b308734e9b0c1468893cae9ff70ebf13e7090be8dcbcc83a8"
+dependencies = [
+ "bitflags 1.3.2",
+ "core-foundation",
+ "core-foundation-sys",
+ "libc",
+ "security-framework-sys",
+]
+
+[[package]]
+name = "security-framework-sys"
+version = "2.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f51d0c0d83bec45f16480d0ce0058397a69e48fcdc52d1dc8855fb68acbd31a7"
+dependencies = [
+ "core-foundation-sys",
+ "libc",
+]
+
+[[package]]
 name = "semver"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 
 [[package]]
 name = "seq-macro"
@@ -2223,14 +2876,26 @@
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
+name = "serde_urlencoded"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d3491c14715ca2294c4d6a88f15e84739788c1d030eed8c110436aafdaa2f3fd"
+dependencies = [
+ "form_urlencoded",
+ "itoa",
+ "ryu",
+ "serde",
+]
+
+[[package]]
 name = "sha2"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
 dependencies = [
  "cfg-if",
  "cpufeatures",
@@ -2283,14 +2948,30 @@
 [[package]]
 name = "snap"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5e9f0ab6ef7eb7353d9119c170a436d1bf248eea575ac42d19d12f4e34130831"
 
 [[package]]
+name = "socket2"
+version = "0.4.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "64a4a911eed85daf18834cfaa86a79b7d266ff93ff5ba14005426219480ed662"
+dependencies = [
+ "libc",
+ "winapi",
+]
+
+[[package]]
+name = "spin"
+version = "0.5.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6e63cff320ae2c57904679ba7cb63280a3dc4613885beafb148ee7bf9aa9042d"
+
+[[package]]
 name = "sqlparser"
 version = "0.34.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37d3706eefb17039056234df6b566b0014f303f867f2656108334a55b8096f59"
 dependencies = [
  "log",
  "sqlparser_derive",
@@ -2414,29 +3095,55 @@
 checksum = "31c0432476357e58790aaa47a8efb0c5138f137343f3b5f23bd36a27e3b0a6d6"
 dependencies = [
  "autocfg",
  "cfg-if",
  "fastrand",
  "redox_syscall",
  "rustix",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "thrift"
 version = "0.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7e54bc85fc7faa8bc175c4bab5b92ba8d9a3ce893d0e9f42cc455c8ab16a9e09"
 dependencies = [
  "byteorder",
  "integer-encoding",
  "ordered-float",
 ]
 
 [[package]]
+name = "time"
+version = "0.3.22"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ea9e1b3cf1243ae005d9e74085d4d542f3125458f3a81af210d901dcd7411efd"
+dependencies = [
+ "serde",
+ "time-core",
+ "time-macros",
+]
+
+[[package]]
+name = "time-core"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
+
+[[package]]
+name = "time-macros"
+version = "0.2.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
+dependencies = [
+ "time-core",
+]
+
+[[package]]
 name = "tiny-keccak"
 version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c9d3793400a45f954c52e73d068316d76b6f4e36977e3fcebb13a2721e80237"
 dependencies = [
  "crunchy",
 ]
@@ -2460,33 +3167,57 @@
 name = "tokio"
 version = "1.28.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94d7b1cfd2aa4011f2de74c2c4c63665e27a71006b0a192dcd2710272e73dfa2"
 dependencies = [
  "autocfg",
  "bytes",
+ "libc",
+ "mio",
  "num_cpus",
  "parking_lot",
  "pin-project-lite",
+ "socket2",
  "tokio-macros",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-macros"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.18",
 ]
 
 [[package]]
+name = "tokio-rustls"
+version = "0.23.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c43ee83903113e03984cb9e5cebe6c04a5116269e900e3ddba8f068a62adda59"
+dependencies = [
+ "rustls 0.20.8",
+ "tokio",
+ "webpki",
+]
+
+[[package]]
+name = "tokio-rustls"
+version = "0.24.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c28327cf380ac148141087fbfb9de9d7bd4e84ab5d2c28fbc911d753de8a7081"
+dependencies = [
+ "rustls 0.21.2",
+ "tokio",
+]
+
+[[package]]
 name = "tokio-stream"
 version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "397c988d37662c7dda6d2208364a706264bf3d6138b11d436cbac0ad38832842"
 dependencies = [
  "futures-core",
  "pin-project-lite",
@@ -2505,20 +3236,49 @@
  "futures-sink",
  "pin-project-lite",
  "tokio",
  "tracing",
 ]
 
 [[package]]
+name = "tower"
+version = "0.4.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b8fa9be0de6cf49e536ce1851f987bd21a43b771b09473c3549a6c853db37c1c"
+dependencies = [
+ "futures-core",
+ "futures-util",
+ "pin-project",
+ "pin-project-lite",
+ "tokio",
+ "tower-layer",
+ "tower-service",
+ "tracing",
+]
+
+[[package]]
+name = "tower-layer"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c20c8dbed6283a09604c3e69b4b7eeb54e298b8a600d4d5ecb5ad39de609f1d0"
+
+[[package]]
+name = "tower-service"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6bc1c9ce2b5135ac7f93c72918fc37feb872bdc6a5533a8b85eb4b86bfdae52"
+
+[[package]]
 name = "tracing"
 version = "0.1.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ce8c33a8d48bd45d624a6e523445fd21ec13d3653cd51f681abf67418f54eb8"
 dependencies = [
  "cfg-if",
+ "log",
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
@@ -2537,14 +3297,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
 dependencies = [
  "once_cell",
 ]
 
 [[package]]
+name = "try-lock"
+version = "0.2.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3528ecfd12c466c6f163363caf2d02a71161dd5e1cc6ae7b34207ea2d42d81ed"
+
+[[package]]
 name = "twox-hash"
 version = "1.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "97fee6b57c6a41524a810daee9286c02d7752c4253064d0b05472833a438f675"
 dependencies = [
  "cfg-if",
  "static_assertions",
@@ -2598,25 +3364,37 @@
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
+name = "untrusted"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a156c684c91ea7d62626509bce3cb4e1d9ed5c4d978f7b4352658f96a4c26b4a"
+
+[[package]]
 name = "url"
 version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50bff7831e19200a85b17131d085c25d7811bc4e186efdaf54bbd132994a88cb"
 dependencies = [
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
+name = "urlencoding"
+version = "2.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e8db7427f936968176eaa7cdf81b7f98b980b18495ec28f1b5791ac3bfe3eea9"
+
+[[package]]
 name = "uuid"
 version = "1.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fa2982af2eec27de306107c027578ff7f423d65f7250e40ce0fea8f45248b81"
 dependencies = [
  "getrandom",
 ]
@@ -2630,24 +3408,39 @@
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
+name = "vsimd"
+version = "0.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5c3082ca00d5a5ef149bb8b555a72ae84c9c59f7250f013ac822ac2e49b19c64"
+
+[[package]]
 name = "walkdir"
 version = "2.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "36df944cda56c7d8d8b7496af378e6b16de9284591917d307c9b4d313c44e698"
 dependencies = [
  "same-file",
  "winapi-util",
 ]
 
 [[package]]
+name = "want"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bfa7760aed19e106de2c7c0b581b509f2f25d3dacaf737cb82ac61bc6d760b0e"
+dependencies = [
+ "try-lock",
+]
+
+[[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
@@ -2671,14 +3464,26 @@
  "proc-macro2",
  "quote",
  "syn 2.0.18",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
+name = "wasm-bindgen-futures"
+version = "0.4.37"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c02dbc21516f9f1f04f187958890d7e6026df8d16540b7ad9492bc34a67cea03"
+dependencies = [
+ "cfg-if",
+ "js-sys",
+ "wasm-bindgen",
+ "web-sys",
+]
+
+[[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
@@ -2700,14 +3505,56 @@
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
 
 [[package]]
+name = "wasm-streams"
+version = "0.2.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6bbae3363c08332cadccd13b67db371814cd214c2524020932f0804b8cf7c078"
+dependencies = [
+ "futures-util",
+ "js-sys",
+ "wasm-bindgen",
+ "wasm-bindgen-futures",
+ "web-sys",
+]
+
+[[package]]
+name = "web-sys"
+version = "0.3.64"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9b85cbef8c220a6abc02aefd892dfc0fc23afb1c6a426316ec33253a3877249b"
+dependencies = [
+ "js-sys",
+ "wasm-bindgen",
+]
+
+[[package]]
+name = "webpki"
+version = "0.22.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f095d78192e208183081cc07bc5515ef55216397af48b873e5edcd72637fa1bd"
+dependencies = [
+ "ring",
+ "untrusted",
+]
+
+[[package]]
+name = "webpki-roots"
+version = "0.22.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6c71e40d7d2c34a5106301fb632274ca37242cd0c9d3e64dbece371a40a2d87"
+dependencies = [
+ "webpki",
+]
+
+[[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
  "winapi-i686-pc-windows-gnu",
  "winapi-x86_64-pc-windows-gnu",
@@ -2741,88 +3588,166 @@
 checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-sys"
+version = "0.42.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+dependencies = [
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
+]
+
+[[package]]
+name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+
+[[package]]
+name = "windows_aarch64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
+
+[[package]]
+name = "windows_aarch64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
+
+[[package]]
+name = "windows_i686_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
+
+[[package]]
+name = "windows_i686_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+
+[[package]]
+name = "windows_x86_64_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
+
+[[package]]
+name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
+name = "winreg"
+version = "0.10.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "80d0f4e272c85def139476380b12f9ac60926689dd2e01d4923222f40580869d"
+dependencies = [
+ "winapi",
+]
+
+[[package]]
+name = "xmlparser"
+version = "0.13.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4d25c75bf9ea12c4040a97f829154768bbbce366287e2dc044af160cd79a13fd"
+
+[[package]]
 name = "xz2"
 version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "388c44dc09d76f1536602ead6d325eb532f5c122f17782bd57fb47baeeb767e2"
 dependencies = [
  "lzma-sys",
 ]
 
 [[package]]
+name = "zeroize"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2a0956f1ba7c7909bfb66c2e9e4124ab6f6482560f6628b5aaeba39207c9aad9"
+
+[[package]]
 name = "zstd"
 version = "0.12.3+zstd.1.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "76eea132fb024e0e13fd9c2f5d5d595d8a967aa72382ac2f9d39fcc95afd0806"
 dependencies = [
  "zstd-safe",
 ]
```

### Comparing `biobear-0.5.0/PKG-INFO` & `biobear-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: biobear
-Version: 0.5.0
+Version: 0.6.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: polars[pyarrow]>=0.17.0
 License-File: LICENSE
 Author-email: WHERE TRUE devs <thauck+biobear@wheretrue.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
-# biobear (v0.5.0)
+# biobear (v0.6.0)
 
 biobear is a Python library designed for reading and searching bioinformatic file formats, using Rust as its backend and producing Arrow or Polars DataFrames as its output.
 
 The python package has minimal dependencies and only requires Polars. Biobear can be used to read various bioinformatic file formats, including FASTA, FASTQ, VCF, BAM, and GFF. It can also query some indexed file formats, including VCF and BAM.
 
 - [Installation](#installation)
 - [Usage](#usage)
+- [S3 and GCS](#s3-and-gcs)
 - [Similar Packages](#similar-packages)
 - [API Documentation](#api-documentation)
   - [vcf\_reader](#vcf_reader)
     - [VCFReader](#vcfreader)
     - [VCFIndexedReader](#vcfindexedreader)
   - [genbank\_reader](#genbank_reader)
     - [GenbankReader](#genbankreader)
@@ -116,14 +117,25 @@
 # │ 1          ┆ 3000151  ┆       ┆ C         ┆ … ┆ 59.200001     ┆ PASS   ┆ AN=4;AC=2                         ┆ GT:DP:GQ       │
 # │ 1          ┆ 3062915  ┆ id3D  ┆ GTTT      ┆ … ┆ 12.9          ┆ q10    ┆ DP4=1,2,3,4;AN=4;AC=2;INDEL;STR=… ┆ GT:GQ:DP:GL    │
 # │ 1          ┆ 3062915  ┆ idSNP ┆ G         ┆ … ┆ 12.6          ┆ test   ┆ TEST=5;DP4=1,2,3,4;AN=3;AC=1,1    ┆ GT:TT:GQ:DP:GL │
 # │ 1          ┆ 3106154  ┆       ┆ CAAA      ┆ … ┆ 342.0         ┆ PASS   ┆ AN=4;AC=2                         ┆ GT:GQ:DP       │
 # └────────────┴──────────┴───────┴───────────┴───┴───────────────┴────────┴───────────────────────────────────┴────────────────┘
 ```
 
+## S3 and GCS
+
+If you pass a `path` that is a URL to an object store, BioBear will attempt to infer your credentials from the environment, and use them to read the file. For example, if you have your `AWS_PROFILE` and `AWS_REGION` env vars set, then you can read from S3 like so:
+
+```python
+import biobear as bb
+
+# Read from S3
+df = bb.FastaReader("s3://bucket/test.fa").read()
+```
+
 ## Similar Packages
 
 Similar packages and/or inspiration for this package:
 
 - https://github.com/abdenlab/saimin/
 - https://github.com/tshauck/brrrr/
 - https://github.com/natir/vcf2parquet/
```

