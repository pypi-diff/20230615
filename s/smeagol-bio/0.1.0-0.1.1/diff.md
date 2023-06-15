# Comparing `tmp/smeagol-bio-0.1.0.tar.gz` & `tmp/smeagol-bio-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/smeagol-bio-0.1.0.tar", last modified: Thu Dec 22 23:26:06 2022, max compression
+gzip compressed data, was "smeagol-bio-0.1.1.tar", last modified: Thu Jun 15 17:33:03 2023, max compression
```

## Comparing `smeagol-bio-0.1.0.tar` & `smeagol-bio-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 avantika   (502) staff       (20)        0 2022-12-22 23:26:06.000000 smeagol-bio-0.1.0/
--rw-r--r--   0 avantika   (502) staff       (20)     1075 2022-02-03 22:20:29.000000 smeagol-bio-0.1.0/LICENSE
--rw-r--r--   0 avantika   (502) staff       (20)      121 2022-12-22 23:26:06.000000 smeagol-bio-0.1.0/PKG-INFO
--rw-r--r--   0 avantika   (502) staff       (20)     2867 2022-11-23 22:38:55.000000 smeagol-bio-0.1.0/README.md
--rw-r--r--   0 avantika   (502) staff       (20)       90 2022-12-22 22:59:45.000000 smeagol-bio-0.1.0/pyproject.toml
--rw-r--r--   0 avantika   (502) staff       (20)       38 2022-12-22 23:26:06.000000 smeagol-bio-0.1.0/setup.cfg
--rw-r--r--   0 avantika   (502) staff       (20)      693 2022-12-22 23:24:04.000000 smeagol-bio-0.1.0/setup.py
-drwxr-xr-x   0 avantika   (502) staff       (20)        0 2022-12-22 23:26:06.000000 smeagol-bio-0.1.0/smeagol/
--rw-r--r--   0 avantika   (502) staff       (20)        0 2022-05-30 04:36:45.000000 smeagol-bio-0.1.0/smeagol/__init__.py
--rw-r--r--   0 avantika   (502) staff       (20)     1365 2022-12-05 02:53:02.000000 smeagol-bio-0.1.0/smeagol/aggregate.py
--rw-r--r--   0 avantika   (502) staff       (20)     7457 2022-12-05 02:53:02.000000 smeagol-bio-0.1.0/smeagol/encode.py
--rw-r--r--   0 avantika   (502) staff       (20)    14037 2022-12-05 02:53:02.000000 smeagol-bio-0.1.0/smeagol/enrich.py
--rw-r--r--   0 avantika   (502) staff       (20)    13022 2022-12-22 19:59:40.000000 smeagol-bio-0.1.0/smeagol/io.py
--rw-r--r--   0 avantika   (502) staff       (20)    16546 2022-12-05 02:53:02.000000 smeagol-bio-0.1.0/smeagol/matrices.py
--rw-r--r--   0 avantika   (502) staff       (20)     6856 2022-12-05 02:53:02.000000 smeagol-bio-0.1.0/smeagol/models.py
--rw-r--r--   0 avantika   (502) staff       (20)    15577 2022-12-05 02:53:02.000000 smeagol-bio-0.1.0/smeagol/scan.py
--rw-r--r--   0 avantika   (502) staff       (20)     5113 2022-12-05 02:53:02.000000 smeagol-bio-0.1.0/smeagol/utils.py
--rw-r--r--   0 avantika   (502) staff       (20)     3993 2022-12-05 02:53:02.000000 smeagol-bio-0.1.0/smeagol/variant.py
--rw-r--r--   0 avantika   (502) staff       (20)    17371 2022-12-05 02:53:02.000000 smeagol-bio-0.1.0/smeagol/visualize.py
-drwxr-xr-x   0 avantika   (502) staff       (20)        0 2022-12-22 23:26:06.000000 smeagol-bio-0.1.0/smeagol_bio.egg-info/
--rw-r--r--   0 avantika   (502) staff       (20)      121 2022-12-22 23:26:06.000000 smeagol-bio-0.1.0/smeagol_bio.egg-info/PKG-INFO
--rw-r--r--   0 avantika   (502) staff       (20)      417 2022-12-22 23:26:06.000000 smeagol-bio-0.1.0/smeagol_bio.egg-info/SOURCES.txt
--rw-r--r--   0 avantika   (502) staff       (20)        1 2022-12-22 23:26:06.000000 smeagol-bio-0.1.0/smeagol_bio.egg-info/dependency_links.txt
--rw-r--r--   0 avantika   (502) staff       (20)      270 2022-12-22 23:26:06.000000 smeagol-bio-0.1.0/smeagol_bio.egg-info/requires.txt
--rw-r--r--   0 avantika   (502) staff       (20)        8 2022-12-22 23:26:06.000000 smeagol-bio-0.1.0/smeagol_bio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 17:33:02.990856 smeagol-bio-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-06-15 17:32:48.000000 smeagol-bio-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-06-15 17:33:02.990856 smeagol-bio-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-06-15 17:32:48.000000 smeagol-bio-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-06-15 17:32:48.000000 smeagol-bio-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-15 17:33:02.990856 smeagol-bio-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-06-15 17:32:48.000000 smeagol-bio-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 17:33:02.990856 smeagol-bio-0.1.1/smeagol/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 17:32:48.000000 smeagol-bio-0.1.1/smeagol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-06-15 17:32:48.000000 smeagol-bio-0.1.1/smeagol/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7457 2023-06-15 17:32:48.000000 smeagol-bio-0.1.1/smeagol/encode.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14037 2023-06-15 17:32:48.000000 smeagol-bio-0.1.1/smeagol/enrich.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13025 2023-06-15 17:32:48.000000 smeagol-bio-0.1.1/smeagol/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16546 2023-06-15 17:32:48.000000 smeagol-bio-0.1.1/smeagol/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6856 2023-06-15 17:32:48.000000 smeagol-bio-0.1.1/smeagol/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15581 2023-06-15 17:32:48.000000 smeagol-bio-0.1.1/smeagol/scan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5667 2023-06-15 17:32:48.000000 smeagol-bio-0.1.1/smeagol/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3993 2023-06-15 17:32:48.000000 smeagol-bio-0.1.1/smeagol/variant.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17726 2023-06-15 17:32:48.000000 smeagol-bio-0.1.1/smeagol/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 17:33:02.990856 smeagol-bio-0.1.1/smeagol_bio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-06-15 17:33:02.000000 smeagol-bio-0.1.1/smeagol_bio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-06-15 17:33:02.000000 smeagol-bio-0.1.1/smeagol_bio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 17:33:02.000000 smeagol-bio-0.1.1/smeagol_bio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-06-15 17:33:02.000000 smeagol-bio-0.1.1/smeagol_bio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-15 17:33:02.000000 smeagol-bio-0.1.1/smeagol_bio.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `smeagol-bio-0.1.0/LICENSE` & `smeagol-bio-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smeagol-bio-0.1.0/README.md` & `smeagol-bio-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -20,34 +20,30 @@
 ```
 
 ### 1. Clone this git repository
 ```
 git clone https://github.com/gruber-sciencelab/SMEAGOL && cd SMEAGOL
 ```
 
-### 2. Install ghostscript if needed
-
-Some of SMEAGOL's visualization functions require [ghostscript](https://www.ghostscript.com/). If you do not have ghostscript installed, please see the link for installation instructions or use `conda install -c conda-forge ghostscript`. (Installing ghostscript via pip leads to an error).
-
-### 3. Install SMEAGOL along with pip dependencies
+### 2. Install SMEAGOL
 ```
 pip install .
 ```
 Or, if you want to edit the code:
 ```
 pip install -e .
 ```
 
-### 4. Run tests locally (optional)
+### 3. Run tests locally (optional)
 ```
 cd tests
 pytest
 ```
 
-### 5. Install jupyter lab and add SMEAGOL kernel to Ipython (if running SMEAGOL in Jupyter notebooks)
+### 4. Install jupyter lab and add SMEAGOL kernel to Ipython (if running SMEAGOL in Jupyter notebooks)
 ```
 pip install jupyterlab 
 python -m ipykernel install --user --name=SMEAGOL --display-name='Python 3.7 (SMEAGOL)'
 ```
 
 ## Usage
```

### Comparing `smeagol-bio-0.1.0/setup.py` & `smeagol-bio-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,14 @@
     for line in open(requirements_path, "r")
     if line.strip() and not line.lstrip().startswith("#")
 ]
 
 # Set up SMEAGOL
 setup(
     name="smeagol-bio",
-    version="0.1.0",
+    version="0.1.1",
     install_requires=required_packages,
     include_package_data=True,
     packages=["smeagol"],
     python_requires=">=3.7, !=3.9",
     platforms=["any"],
 )
```

### Comparing `smeagol-bio-0.1.0/smeagol/aggregate.py` & `smeagol-bio-0.1.1/smeagol/aggregate.py`

 * *Files identical despite different names*

### Comparing `smeagol-bio-0.1.0/smeagol/encode.py` & `smeagol-bio-0.1.1/smeagol/encode.py`

 * *Files identical despite different names*

### Comparing `smeagol-bio-0.1.0/smeagol/enrich.py` & `smeagol-bio-0.1.1/smeagol/enrich.py`

 * *Files identical despite different names*

### Comparing `smeagol-bio-0.1.0/smeagol/io.py` & `smeagol-bio-0.1.1/smeagol/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     # Get matrix start and end positions
     starts = np.where([x[0].startswith(">") for x in pms])[0]
     # Check that the first line of the file starts with >
     assert starts[0] == 0
     ends = np.append(starts[1:], len(pms))
 
     # Get matrix IDs and values
-    pm_ids = [l[0].strip(">") for l in pms if l[0].startswith(">")]
+    pm_ids = [pm[0].strip(">") for pm in pms if pm[0].startswith(">")]
 
     # Check that matrix lengths match values supplied in the file
     if check_lens:
         lens = np.array([
             pm[1] for pm in pms if pm[0].startswith(">")]).astype("int")
         assert np.all(lens == ends - starts - 1)
```

### Comparing `smeagol-bio-0.1.0/smeagol/matrices.py` & `smeagol-bio-0.1.1/smeagol/matrices.py`

 * *Files identical despite different names*

### Comparing `smeagol-bio-0.1.0/smeagol/models.py` & `smeagol-bio-0.1.1/smeagol/models.py`

 * *Files identical despite different names*

### Comparing `smeagol-bio-0.1.0/smeagol/scan.py` & `smeagol-bio-0.1.1/smeagol/scan.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,15 @@
                     .reset_index()
                 )
         # Calculate stats
         if "stats" in outputs:
             stats = (
                 output["counts"]
                 .groupby(["Matrix_id", "width", "sense"])
-                .agg([len, np.mean, np.std])
+                .num.agg([len, np.mean, np.std])
                 .reset_index()
             )
             stats.columns = ["Matrix_id", "width", "sense", "len", "avg", "sd"]
             output["stats"] = stats
             if "counts" not in outputs:
                 del output["counts"]
```

### Comparing `smeagol-bio-0.1.0/smeagol/utils.py` & `smeagol-bio-0.1.1/smeagol/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import pandas as pd
-from ushuffle import shuffle, set_seed
+import random
+from deeplift.dinuc_shuffle import dinuc_shuffle
 
 # Biopython imports
 from Bio.Seq import Seq
 from Bio.SeqRecord import SeqRecord
 
 # Smeagol imports
 from smeagol.io import read_fasta, write_fasta
@@ -28,41 +29,50 @@
     elif type(x) == type(y) == list:
         assert len(x) == len(y)
         return np.all(abs(x - y) < (eps * len(x)))
     else:
         return abs(x - y) < eps
 
 
-def shuffle_records(records, simN, simK, out_file=None, seed=1):
+def shuffle_records(records, simN, simK=2, out_file=None, seed=1):
     """Function to shuffle sequences.
-
     Args:
         records (list): list of seqRecord objects
         simN (int): Number of times to shuffle
-        simK (int): k-mer frequency to conserve
+        simK (int): k-mer frequency to conserve, either 1 or 2
         out_file (str): Path to output file (optional)
-
+        seed (int): Random seed
     Returns:
         shuf_records (list): list of shuffled sequences
         Writes shuf_records to file if out_file provided.
-
     """
     shuf_records = []
-
-    if seed is not None:
-        set_seed(seed)
-
     # Shuffle each record
     for record in records:
-        for n in range(simN):
-            new_seq = shuffle(str.encode(record.seq.__str__()), simK).decode()
-            new_seq = SeqRecord(Seq(new_seq),
-                                id="background_seq_{0:d}".format(n))
-            new_seq.name = record.id
-            shuf_records.append(new_seq)
+        # Get sequence
+        seq = record.seq.__str__()
+        # Shuffle
+        if simK == 2:
+            new_seqs = dinuc_shuffle(seq, num_shufs=simN,
+                                     rng=np.random.RandomState(seed))
+        elif simK == 1:
+            random.seed(seed)
+            new_seqs = []
+            for i in range(simN):
+                shuffled = [base for base in seq].copy()
+                random.shuffle(shuffled)
+                new_seqs.append(''.join(shuffled))
+        else:
+            raise ValueError("simK must be 1 or 2.")
+
+        # Convert to seqrecord format
+        for i, new_seq in enumerate(new_seqs):
+            shuf_records.append(SeqRecord(Seq(new_seq),
+                                          id="background_seq_{0:d}".format(i),
+                                          name=record.id))
     print(
         "Shuffled {} sequence(s) {} times while conserving \
         k-mer frequency for k = {}.".format(
             len(records), simN, simK
         )
     )
```

### Comparing `smeagol-bio-0.1.0/smeagol/variant.py` & `smeagol-bio-0.1.1/smeagol/variant.py`

 * *Files identical despite different names*

### Comparing `smeagol-bio-0.1.0/smeagol/visualize.py` & `smeagol-bio-0.1.1/smeagol/visualize.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,88 +1,99 @@
 # General imports
 import numpy as np
 import pandas as pd
+from .matrices import pwm_to_ppm, position_wise_ic
 
 # Viz imports
 from matplotlib import pyplot as plt
 import seaborn as sns
-import weblogo as wl
-import IPython.display as ipd
-import seqlogo
+from deeplift.visualization.viz_sequence import plot_weights_given_ax
 
 # Stats imports
 import scipy.stats as stats
 
 
-def pwm_logo(weights, title="", height=15):
+def ppm_logo(probs, title="", figsize=(5, 2)):
+    """Function to visualize the sequence logo of a PPM.
+
+    Args:
+        probs (np.array): array containing probabilities
+        title (str): Title of the logo.
+        figsize (tuple): (width, height)
+
+    Returns:
+        PPM logo
+
+    """
+    # Calculate IC
+    ic = position_wise_ic(probs)
+    # Scale probabilities by IC
+    probs_scaled = probs*np.expand_dims(ic, 1)
+    # Create figure and axes
+    fig = plt.figure(figsize=figsize)
+    ax = fig.add_subplot(111)
+    # Set title
+    if title != "":
+        ax.set_title(title)
+    # Plot logo
+    plot_weights_given_ax(ax=ax, array=probs_scaled,
+                          height_padding_factor=0.1,
+                          length_padding=0.01,
+                          subticks_frequency=1,
+                          highlight={})
+    plt.show()
+
+
+def pwm_logo(weights, title="", figsize=(5, 2)):
     """Function to visualize the sequence logo of a PWM.
 
     Args:
         weights (np.array): array containing PWM weight values
         title (str): Title of the logo.
-        height (int): Height of the plot
+        figsize (tuple): (width, height)
 
     Returns:
         PWM logo
 
     """
-    pm = np.exp2(weights) / 4
-    pm = seqlogo.Ppm(pm / np.expand_dims(np.sum(pm, axis=1), 1))
-    options = wl.LogoOptions(
-        unit_name="bits",
-        color_scheme=wl.std_color_schemes["classic"],
-        show_fineprint=False,
-        stack_width=height,
-    )
-    options.logo_title = title
-    out = wl.formatters["png"](pm, wl.LogoFormat(pm, options))
-    return ipd.Image(out)
+    # Convert PWM to PPM
+    ppm = pwm_to_ppm(weights)
+    ppm_logo(ppm, title=title, figsize=figsize)
 
 
-def plot_pwm(pwm_df, Matrix_id, height=15):
+def plot_pwm(pwm_df, Matrix_id, figsize=(5, 2)):
     """Function to plot sequence logo from PWM
 
     Args:
         pwm_df (pd.DataFrame): Dataframe containing cols weight, Matrix_id
         Matrix_id: ID of PWM to plot (will be used as logo title)
-        height (int): Height of the plot
+        figsize (tuple): (width, height)
 
     Returns:
         Plots PWM
 
     """
-    weights = pwm_df.weights.values[pwm_df.Matrix_id == Matrix_id]
-    logo = pwm_logo(weights=weights[0], title=Matrix_id, height=height)
-
-    return logo
+    weights = pwm_df.weights.values[pwm_df.Matrix_id == Matrix_id][0]
+    pwm_logo(weights=weights, title=Matrix_id, figsize=figsize)
 
 
-def plot_ppm(ppm_df, Matrix_id, height=15):
+def plot_ppm(ppm_df, Matrix_id, figsize=(5, 2)):
     """
     Function to plot sequence logo from PPM
 
     Args:
         ppm_df (pd.DataFrame): Dataframe containing cols probs, Matrix_id
         Matrix_id: ID of PWM to plot
 
     Returns:
         Plots PPM
 
     """
-    probs = ppm_df.probs.values[ppm_df.Matrix_id == Matrix_id]
-    pm = seqlogo.Ppm(probs[0])
-    options = wl.LogoOptions(
-        unit_name="bits",
-        color_scheme=wl.std_color_schemes["classic"],
-        show_fineprint=False,
-        stack_width=height,
-    )
-    options.logo_title = Matrix_id
-    out = wl.formatters["png"](pm, wl.LogoFormat(pm, options))
-    return ipd.Image(out)
+    probs = ppm_df.probs.values[ppm_df.Matrix_id == Matrix_id][0]
+    ppm_logo(probs=probs, title=Matrix_id, figsize=figsize)
 
 
 def plot_binned_count_dist(
     real_preds, Matrix_id, sense, shuf_preds=None, rounding=3, file_path=None
 ):
     """Function to plot distribution of (fractional) binding site scores
     in real vs. shuffled genomes
```

