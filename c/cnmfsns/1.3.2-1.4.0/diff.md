# Comparing `tmp/cnmfsns-1.3.2.tar.gz` & `tmp/cnmfsns-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnmfsns-1.3.2.tar", last modified: Mon May 29 18:21:07 2023, max compression
+gzip compressed data, was "cnmfsns-1.4.0.tar", last modified: Thu Jun 15 03:50:41 2023, max compression
```

## Comparing `cnmfsns-1.3.2.tar` & `cnmfsns-1.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 18:21:07.235811 cnmfsns-1.3.2/
--rw-rw-rw-   0        0        0     1090 2023-04-24 20:31:27.000000 cnmfsns-1.3.2/LICENSE
--rw-rw-rw-   0        0        0     3982 2023-05-29 18:21:07.235811 cnmfsns-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     3467 2023-05-29 18:20:04.000000 cnmfsns-1.3.2/README.md
--rw-rw-rw-   0        0        0       86 2023-04-24 20:31:27.000000 cnmfsns-1.3.2/pyproject.toml
--rw-rw-rw-   0        0        0      964 2023-05-29 18:21:07.235811 cnmfsns-1.3.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-29 18:21:07.204917 cnmfsns-1.3.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-29 18:21:07.221291 cnmfsns-1.3.2/src/cnmfsns/
--rw-rw-rw-   0        0        0      513 2023-05-12 18:06:16.000000 cnmfsns-1.3.2/src/cnmfsns/__init__.py
--rw-rw-rw-   0        0        0    56223 2023-05-16 20:25:56.000000 cnmfsns-1.3.2/src/cnmfsns/cli.py
--rw-rw-rw-   0        0        0    39682 2023-05-12 20:51:27.000000 cnmfsns-1.3.2/src/cnmfsns/cnmf.py
--rw-rw-rw-   0        0        0    16061 2023-04-24 20:31:27.000000 cnmfsns-1.3.2/src/cnmfsns/colors.py
--rw-rw-rw-   0        0        0     3257 2023-04-24 20:31:27.000000 cnmfsns-1.3.2/src/cnmfsns/config.py
--rw-rw-rw-   0        0        0    35130 2023-05-29 17:09:43.000000 cnmfsns-1.3.2/src/cnmfsns/dataset.py
--rw-rw-rw-   0        0        0    21163 2023-05-15 22:09:27.000000 cnmfsns-1.3.2/src/cnmfsns/integration.py
--rw-rw-rw-   0        0        0    57617 2023-05-16 18:55:37.000000 cnmfsns-1.3.2/src/cnmfsns/plots.py
--rw-rw-rw-   0        0        0    35301 2023-05-16 19:23:15.000000 cnmfsns-1.3.2/src/cnmfsns/sns.py
--rw-rw-rw-   0        0        0     2767 2023-04-24 20:31:27.000000 cnmfsns-1.3.2/src/cnmfsns/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-29 18:21:07.235811 cnmfsns-1.3.2/src/cnmfsns.egg-info/
--rw-rw-rw-   0        0        0     3982 2023-05-29 18:21:07.000000 cnmfsns-1.3.2/src/cnmfsns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      472 2023-05-29 18:21:07.000000 cnmfsns-1.3.2/src/cnmfsns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 18:21:07.000000 cnmfsns-1.3.2/src/cnmfsns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-29 18:21:07.000000 cnmfsns-1.3.2/src/cnmfsns.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      177 2023-05-29 18:21:07.000000 cnmfsns-1.3.2/src/cnmfsns.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-29 18:21:07.000000 cnmfsns-1.3.2/src/cnmfsns.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 03:50:41.945923 cnmfsns-1.4.0/
+-rw-rw-rw-   0        0        0     1090 2023-04-24 20:31:27.000000 cnmfsns-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0     3982 2023-06-15 03:50:41.945923 cnmfsns-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3467 2023-06-15 03:49:18.000000 cnmfsns-1.4.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-24 20:31:27.000000 cnmfsns-1.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0      964 2023-06-15 03:50:41.945923 cnmfsns-1.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-15 03:50:41.917259 cnmfsns-1.4.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-15 03:50:41.930265 cnmfsns-1.4.0/src/cnmfsns/
+-rw-rw-rw-   0        0        0      513 2023-05-12 18:06:16.000000 cnmfsns-1.4.0/src/cnmfsns/__init__.py
+-rw-rw-rw-   0        0        0    51783 2023-06-15 03:32:43.000000 cnmfsns-1.4.0/src/cnmfsns/cli.py
+-rw-rw-rw-   0        0        0    39682 2023-05-12 20:51:27.000000 cnmfsns-1.4.0/src/cnmfsns/cnmf.py
+-rw-rw-rw-   0        0        0    16061 2023-04-24 20:31:27.000000 cnmfsns-1.4.0/src/cnmfsns/colors.py
+-rw-rw-rw-   0        0        0     3257 2023-04-24 20:31:27.000000 cnmfsns-1.4.0/src/cnmfsns/config.py
+-rw-rw-rw-   0        0        0    35838 2023-06-14 22:17:36.000000 cnmfsns-1.4.0/src/cnmfsns/dataset.py
+-rw-rw-rw-   0        0        0    21163 2023-06-15 03:50:05.000000 cnmfsns-1.4.0/src/cnmfsns/integration.py
+-rw-rw-rw-   0        0        0    59336 2023-06-15 03:48:57.000000 cnmfsns-1.4.0/src/cnmfsns/plots.py
+-rw-rw-rw-   0        0        0    35301 2023-05-16 19:23:15.000000 cnmfsns-1.4.0/src/cnmfsns/sns.py
+-rw-rw-rw-   0        0        0     2767 2023-04-24 20:31:27.000000 cnmfsns-1.4.0/src/cnmfsns/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 03:50:41.945923 cnmfsns-1.4.0/src/cnmfsns.egg-info/
+-rw-rw-rw-   0        0        0     3982 2023-06-15 03:50:41.000000 cnmfsns-1.4.0/src/cnmfsns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2023-06-15 03:50:41.000000 cnmfsns-1.4.0/src/cnmfsns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 03:50:41.000000 cnmfsns-1.4.0/src/cnmfsns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-15 03:50:41.000000 cnmfsns-1.4.0/src/cnmfsns.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      177 2023-06-15 03:50:41.000000 cnmfsns-1.4.0/src/cnmfsns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-15 03:50:41.000000 cnmfsns-1.4.0/src/cnmfsns.egg-info/top_level.txt
```

### Comparing `cnmfsns-1.3.2/LICENSE` & `cnmfsns-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.2/PKG-INFO` & `cnmfsns-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnmfsns
-Version: 1.3.2
+Version: 1.4.0
 Summary: cNMF Solution Network Space
 Home-page: https://github.com/MorrissyLab/cNMF-SNS
 Author: Ted Verhey
 Author-email: tbverhey@ucalgary.ca
 Project-URL: Bug Tracker, https://github.com/MorrissyLab/cNMF-SNS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 
 ![cNMF-SNS logo](logo.png)
 
 -----------------
 
 # cNMF-SNS: powerful factorization-based multi-omics integration toolkit
 
-![version badge](https://img.shields.io/badge/version-1.3.2-blue)
+![version badge](https://img.shields.io/badge/version-1.4.0-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
 [![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/cnmfsns)](https://anaconda.org/conda-forge/cnmfsns/)
 [![Documentation status](https://readthedocs.org/projects/cnmf-sns/badge/?version=latest&style=flat)]()
 [![Downloads](https://static.pepy.tech/badge/cnmfsns)](https://pepy.tech/project/cnmfsns)
 [![License](https://img.shields.io/pypi/l/cnmfsns.svg)](https://github.com/MorrissyLab/cNMF-SNS/blob/main/LICENSE)
 
 Authors: [Ted Verhey](https://github.com/verheytb), [Heewon Seo](https://github.com/lootpiz), [Sorana Morrissy](https://github.com/ancasorana)
```

### Comparing `cnmfsns-1.3.2/README.md` & `cnmfsns-1.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 2070 6f77 6572 6675 6c20 6661 6374 6f72   powerful factor
 00000050: 697a 6174 696f 6e2d 6261 7365 6420 6d75  ization-based mu
 00000060: 6c74 692d 6f6d 6963 7320 696e 7465 6772  lti-omics integr
 00000070: 6174 696f 6e20 746f 6f6c 6b69 740d 0a0d  ation toolkit...
 00000080: 0a21 5b76 6572 7369 6f6e 2062 6164 6765  .![version badge
 00000090: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
 000000a0: 6965 6c64 732e 696f 2f62 6164 6765 2f76  ields.io/badge/v
-000000b0: 6572 7369 6f6e 2d31 2e33 2e32 2d62 6c75  ersion-1.3.2-blu
+000000b0: 6572 7369 6f6e 2d31 2e34 2e30 2d62 6c75  ersion-1.4.0-blu
 000000c0: 6529 0d0a 5b21 5b50 7950 4920 4c61 7465  e)..[![PyPI Late
 000000d0: 7374 2052 656c 6561 7365 5d28 6874 7470  st Release](http
 000000e0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
 000000f0: 696f 2f70 7970 692f 762f 636e 6d66 736e  io/pypi/v/cnmfsn
 00000100: 732e 7376 6729 5d28 6874 7470 733a 2f2f  s.svg)](https://
 00000110: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
 00000120: 2f63 6e6d 6673 6e73 2f29 0d0a 5b21 5b43  /cnmfsns/)..[![C
```

### Comparing `cnmfsns-1.3.2/setup.cfg` & `cnmfsns-1.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6e6d 6673 6e73 0d0a 7665 7273   = cnmfsns..vers
-00000020: 696f 6e20 3d20 312e 332e 320d 0a61 7574  ion = 1.3.2..aut
+00000020: 696f 6e20 3d20 312e 342e 300d 0a61 7574  ion = 1.4.0..aut
 00000030: 686f 7220 3d20 5465 6420 5665 7268 6579  hor = Ted Verhey
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 2074 6276 6572 6865 7940 7563 616c 6761   tbverhey@ucalga
 00000060: 7279 2e63 610d 0a64 6573 6372 6970 7469  ry.ca..descripti
 00000070: 6f6e 203d 2063 4e4d 4620 536f 6c75 7469  on = cNMF Soluti
 00000080: 6f6e 204e 6574 776f 726b 2053 7061 6365  on Network Space
 00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
```

### Comparing `cnmfsns-1.3.2/src/cnmfsns/__init__.py` & `cnmfsns-1.4.0/src/cnmfsns/__init__.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.2/src/cnmfsns/cli.py` & `cnmfsns-1.4.0/src/cnmfsns/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -460,26 +460,24 @@
     # create config
     if config_toml is not None:
         config = Config.from_toml(config_toml)
     elif input_h5ad:
         config = Config.from_h5ad_files(input_h5ad)
 
     # Create dataset objects from config parameters
-    datasets = []
+    datasets = {}
     for dsname, dsparams in config.datasets.items():
         
         dataset = Dataset.from_h5ad(
             dsparams["filename"],
-            name=dsname,
-            color=(dsparams["color"] if "color" in dsparams else None),
             backed=False,
             patient_id_col = (dsparams["patient_id_col"] if "patient_id_col" in dsparams else None),
             force_migrate = False
         )
-        datasets.append(dataset)
+        datasets[dsname] = dataset
         
     # creates integration object from config parameters
     integration = Integration(
         datasets=datasets,
         corr_method = config.integrate["corr_method"],
         max_median_corr = config.integrate["max_median_corr"],
         negative_corr_quantile = config.integrate["negative_corr_quantile"]
@@ -554,27 +552,23 @@
         config = Config.from_toml(config_toml)
 
     # Create directory structures
     sns_output_dir = os.path.join(output_dir, "sns_networks", name)
     os.makedirs(sns_output_dir, exist_ok=True)
 
     # Create dataset objects from config parameters
-    datasets = []
+    datasets = {}
     for dsname, dsparams in config.datasets.items():
-        
         ds_obj = Dataset.from_h5ad(
             dsparams["filename"],
-            name=dsname,
-            color=(dsparams["color"] if "color" in dsparams else None),
             backed="r",
             patient_id_col = (dsparams["patient_id_col"] if "patient_id_col" in dsparams else None),
             force_migrate = False
         )
-        datasets.append(ds_obj)
-        
+        datasets[dsname] = ds_obj
         
     # selected_k from config.toml file overrides defaults
     selected_k = {dsname: ("selected_k" in dsparams) for dsname, dsparams in config.datasets.items()}
     if all(list(selected_k.values())):
         selected_k = {dsname: dsparams["selected_k"] for dsname, dsparams in config.datasets.items()}
     elif any(list(selected_k.values())):
         no_selected_k = ", ".join([dsname for dsname, hasselected in selected_k.items() if not hasselected])
@@ -606,14 +600,15 @@
     nx.write_graphml(snsmap.gep_graph, os.path.join(sns_output_dir, "gep_graph.graphml"))
 
     snsmap.compute_layout(
         algorithm=config.sns["layout_algorithm"],
         shared_community_weight = config.sns["layouts"]["community_weighted_spring"]["within_community"],
         shared_dataset_weight = config.sns["layouts"]["community_weighted_spring"]["within_dataset"]
     )
+    snsmap.compute_community_network_layout()
     
     # make figure legends for metadata
     colors = Colors.from_config(config)
     colors.add_missing_dataset_colors(datasets=integration)
     colors.add_missing_metadata_colors(datasets=integration)
     colors.add_missing_community_colors(snsmap=snsmap)
     colors.to_toml(os.path.join(sns_output_dir, "colors.toml"))
@@ -626,24 +621,31 @@
     fig.savefig(os.path.join(sns_output_dir, "dataset_colors_legend.pdf"))
     plt.close(fig)
     
     snsmap.write_communities_toml( os.path.join(sns_output_dir, "communities.toml"))
     pd.DataFrame.from_dict(data=snsmap.gep_communities, orient='index').to_csv(os.path.join(sns_output_dir, 'gep_communities.txt'), sep="\t", header=False)
         
     representative_geps = snsmap.get_representative_geps()
-    representative_geps.to_csv(os.path.join(sns_output_dir, "representative_geps.txt"), sep="\t") # outputs the GEP identities
+    representative_geps.to_csv(os.path.join(sns_output_dir, "representative_geps.txt"), sep="\t") # outputs the GEPs to text file
 
     logging.info("Creating SNS plots...")
 
     # plot membership of datasets and ranks for each community
     fig = plot_community_by_dataset_rank(snsmap, colors)
     fig.savefig(os.path.join(sns_output_dir, "communities_by_dataset_rank.pdf"))
     fig.savefig(os.path.join(sns_output_dir, "communities_by_dataset_rank.png"), dpi=600)
     plt.close(fig)
     
+    # summary community network
+    fig = plot_summary_community_network(snsmap, colors)
+    fig.savefig(os.path.join(sns_output_dir, "community_summary_network.pdf"))
+    fig.savefig(os.path.join(sns_output_dir, "community_summary_network.png"), dpi=600)
+    plt.close(fig)
+
+
     # Plot network colored by dataset
     fig = plot_gep_network_datasets(snsmap, colors)
     fig.savefig(os.path.join(sns_output_dir, "gep_network_datasets.pdf"))
     fig.savefig(os.path.join(sns_output_dir, "gep_network_datasets.png"), dpi=600)
     plt.close(fig)
     
     # Plot network colored by dataset and size by rank
@@ -658,231 +660,144 @@
     fig.savefig(os.path.join(sns_output_dir, "gep_network_communities.png"), dpi=600)
     plt.close(fig)
     
     # Cumulative proportion of samples contributing to each GEP
     fig = plot_gep_network_nsamples(snsmap, colors)
     fig.savefig(os.path.join(sns_output_dir, "gep_network_n_samples.pdf"))
     fig.savefig(os.path.join(sns_output_dir, "gep_network_n_samples.png"), dpi=600)
+    plt.close(fig)
     
     # Cumulative proportion of patients contributing to each GEP
     if snsmap.integration.sample_to_patient is not None:
         fig = plot_gep_network_npatients(snsmap, colors)
         fig.savefig(os.path.join(sns_output_dir, "gep_network_n_patients.pdf"))
         fig.savefig(os.path.join(sns_output_dir, "gep_network_n_patients.png"), dpi=600)
+        plt.close(fig)
     
+    
+    logging.info("Creating community usage heatmap...")
+
     # integrated community usage
     ic_usage = snsmap.get_community_usage()
     ic_usage.to_csv(os.path.join(sns_output_dir, "integrated_community_usage.txt"), sep="\t")
     fig = plot_community_usage_heatmap(snsmap, colors)
     fig.savefig(os.path.join(sns_output_dir, "integrated_community_usage.pdf"))
+    plt.close(fig)
    
-    # GEP-level, categorical data, overrepresentation data
+
+    logging.info("Creating community-level associations")
+
+    # Community-level, categorical metadata, overrepresentation
+    for dataset_name, dataset in integration.datasets.items():
+        os.makedirs(os.path.join(sns_output_dir, "annotated_communities", "overrepresentation", dataset_name), exist_ok=True)
+        for layer in dataset.get_metadata_df(include_numerical=False):
+            df = snsmap.get_community_category_overrepresentation(layer=layer, subset_datasets=dataset_name, truncate_negative=False)
+            df.to_csv(os.path.join(sns_output_dir, "annotated_communities", "overrepresentation", dataset_name, layer + ".txt"), sep='\t')
+            
+    # Community-level, numerical metadata, correlation
+    for dataset_name, dataset in integration.datasets.items():
+        os.makedirs(os.path.join(sns_output_dir, "annotated_communities", "correlation", dataset_name), exist_ok=True)
+        for layer in dataset.get_metadata_df(include_categorical=False):
+            df = snsmap.get_community_metadata_correlation(layer=layer, subset_datasets=dataset_name, method="pearson")
+            df.to_csv(os.path.join(sns_output_dir, "annotated_communities", "correlation", dataset_name, layer + ".txt"), sep='\t')
+
+    logging.info("Creating community-level bar plots")
+
+    # Community-level, categorical data, overrepresentation bar plots
+    for dataset_name in integration.datasets:
+        os.makedirs(os.path.join(sns_output_dir, "annotated_communities", "overrepresentation_bar", dataset_name), exist_ok=True)
+        for layer in dataset.get_metadata_df(include_numerical=False):
+            fig = plot_overrepresentation_community_bar(snsmap, colors, layer=layer, subset_datasets=dataset_name)
+            os.makedirs(os.path.join(sns_output_dir, "annotated_communities", "overrepresentation_bar"), exist_ok=True)
+            fig.savefig(os.path.join(sns_output_dir, "annotated_communities", "overrepresentation_bar", dataset_name, layer + ".pdf"))
+            plt.close(fig)
+        
+    # Community-level, numerical metadata, correlation bar plots
+    for dataset_name in integration.datasets:
+        os.makedirs(os.path.join(sns_output_dir, "annotated_communities", "correlation_bar", dataset_name), exist_ok=True)
+        for layer in dataset.get_metadata_df(include_categorical=False):
+            fig = plot_metadata_correlation_community_bar(snsmap, colors, layer=layer, subset_datasets=dataset_name)
+            os.makedirs(os.path.join(sns_output_dir, "annotated_communities", "correlation_bar"), exist_ok=True)
+            fig.savefig(os.path.join(sns_output_dir, "annotated_communities", "correlation_bar", dataset_name, layer + ".pdf"))
+            plt.close(fig)
+
+
+    logging.info("Creating community-level network plots")
+
+    # Community-level, categorical data, overrepresentation network
+    for dataset_name in integration.datasets:
+        os.makedirs(os.path.join(sns_output_dir, "annotated_communities", "overrepresentation_network", dataset_name), exist_ok=True)
+        for layer in dataset.get_metadata_df(include_numerical=False):
+            fig = plot_overrepresentation_community_network(snsmap, colors, layer=layer, subset_datasets=dataset_name)   
+            fig.savefig(os.path.join(sns_output_dir, "annotated_communities", "overrepresentation_network", dataset_name, layer + ".pdf"))
+            fig.savefig(os.path.join(sns_output_dir, "annotated_communities", "overrepresentation_network", dataset_name, layer + ".png"), dpi=600)
+            plt.close(fig)
+ 
+    # Community-level, numerical data, correlation network
+    for dataset_name in integration.datasets:
+        os.makedirs(os.path.join(sns_output_dir, "annotated_communities", "correlation_network", dataset_name), exist_ok=True)
+        for layer in dataset.get_metadata_df(include_categorical=False):
+            fig = plot_metadata_correlation_community_network(snsmap, colors, layer=layer, subset_datasets=dataset_name)   
+            fig.savefig(os.path.join(sns_output_dir, "annotated_communities", "correlation_network", dataset_name, layer + ".pdf"))
+            fig.savefig(os.path.join(sns_output_dir, "annotated_communities", "correlation_network", dataset_name, layer + ".png"), dpi=600)
+            plt.close(fig)    
+
+    logging.info("Creating GEP-level associations")
+
+    # GEP-level, categorical metadata, overrepresentation
     for dataset_name, dataset in integration.datasets.items():
         os.makedirs(os.path.join(sns_output_dir, "annotated_geps", "overrepresentation", dataset_name), exist_ok=True)
         for layer in dataset.get_metadata_df(include_numerical=False):
             df = dataset.get_category_overrepresentation(layer)
             df.to_csv(os.path.join(sns_output_dir, "annotated_geps", "overrepresentation", dataset_name, layer + ".txt"), sep='\t')
             
+    # GEP-level, numerical metadata, correlation
+    for dataset_name, dataset in integration.datasets.items():
+        os.makedirs(os.path.join(sns_output_dir, "annotated_geps", "correlation", dataset_name), exist_ok=True)
+        for layer in dataset.get_metadata_df(include_categorical=False):
+            df = dataset.get_metadata_correlation(layer, method="pearson")
+            df.to_csv(os.path.join(sns_output_dir, "annotated_geps", "correlation", dataset_name, layer + ".txt"), sep='\t')
+
+    logging.info("Creating GEP-level bar plots")
+
     # GEP-level, categorical data, overrepresentation bar plots
     for dataset_name in integration.datasets:
         fig = plot_overrepresentation_gep_bar(snsmap, colors, dataset_name=dataset_name)
         os.makedirs(os.path.join(sns_output_dir, "annotated_geps", "overrepresentation_bar"), exist_ok=True)
         fig.savefig(os.path.join(sns_output_dir, "annotated_geps", "overrepresentation_bar", dataset_name + ".pdf"))
+        plt.close(fig)
         
+    # GEP-level, numerical metadata, correlation bar plots
+    for dataset_name in integration.datasets:
+        fig = plot_metadata_correlation_gep_bar(snsmap, colors, dataset_name=dataset_name)
+        os.makedirs(os.path.join(sns_output_dir, "annotated_geps", "correlation_bar"), exist_ok=True)
+        fig.savefig(os.path.join(sns_output_dir, "annotated_geps", "correlation_bar", dataset_name + ".pdf"))
+        plt.close(fig)
+
+    logging.info("Creating GEP-level network plots")
 
     # GEP-level, categorical data, overrepresentation network
     for dataset_name in integration.datasets:
         os.makedirs(os.path.join(sns_output_dir, "annotated_geps", "overrepresentation_network", dataset_name), exist_ok=True)
         for layer in dataset.get_metadata_df(include_numerical=False):
             fig = plot_overrepresentation_gep_network(snsmap, colors, layer=layer, subset_datasets=dataset_name)   
             fig.savefig(os.path.join(sns_output_dir, "annotated_geps", "overrepresentation_network", dataset_name, layer + ".pdf"))
             fig.savefig(os.path.join(sns_output_dir, "annotated_geps", "overrepresentation_network", dataset_name, layer + ".png"), dpi=600)
             plt.close(fig)
-        
-
-
-
+ 
+    # GEP-level, numerical data, correlation network
+    for dataset_name in integration.datasets:
+        os.makedirs(os.path.join(sns_output_dir, "annotated_geps", "overrepresentation_network", dataset_name), exist_ok=True)
+        for layer in dataset.get_metadata_df(include_categorical=False):
+            fig = plot_metadata_correlation_gep_network(snsmap, colors, layer=layer, subset_datasets=dataset_name)   
+            fig.savefig(os.path.join(sns_output_dir, "annotated_geps", "correlation_network", dataset_name, layer + ".pdf"))
+            fig.savefig(os.path.join(sns_output_dir, "annotated_geps", "correlation_network", dataset_name, layer + ".png"), dpi=600)
+            plt.close(fig)       
 
 
-    # # GEP level, numerical data, correlation plots
-    # logging.info("Creating GEP network plots for numerical metadata")
-    # for dataset_name, dataset in config.datasets.items():
-    #     metadata = read_h5ad(dataset["filename"], backed="r").obs.select_dtypes(exclude="category").dropna(axis=1, how="all")  # exclude categorical data
-    #     if metadata.shape[1] == 0:
-    #         continue
-        
-    #     dataset_is_in_nodes = any([node.split("|")[0] == dataset_name for community in communities.values() for node in community])
-    #     if not dataset_is_in_nodes:
-    #         continue
-        
-    #     # bar charts
-    #     fig = plot_metadata_correlation_geps_bar(usage, metadata, communities, dataset_name, config)
-    #     os.makedirs(os.path.join(sns_output_dir, "annotated_geps", "correlation_bar_by_community"), exist_ok=True)
-    #     fig.savefig(os.path.join(sns_output_dir, "annotated_geps", "correlation_bar_by_community", dataset_name + ".pdf"))
-    #     plt.close(fig)
-
-    #     for annotation_layer, sample_to_numeric in metadata.items():
-    #         ds_usage = usage.loc[:, (dataset_name, slice(None), slice(None))].dropna(how="all").droplevel(axis=0, level=0)
-    #         correlation = ds_usage.corrwith(sample_to_numeric, method="spearman")
-    #         os.makedirs(os.path.join(sns_output_dir, "annotated_geps", "correlation", dataset_name), exist_ok=True)
-    #         correlation.to_csv(os.path.join(sns_output_dir, "annotated_geps", "correlation", dataset_name, annotation_layer + ".txt"), sep='\t')
-    #         correlation.index = pd.Index([f"{c[0]}|{c[1]}|{c[2]}" for c in correlation.index])
-    #         fig = plot_metadata_correlation_network(
-    #             graph=G,
-    #             layout=layout,
-    #             title=f"Dataset: {dataset_name}\nMetadata Layer: {annotation_layer}",
-    #             correlation=correlation,
-    #             plot_size=config.sns["plot_size_gep"],
-    #             node_size=config.sns["node_size"],
-    #             config=config
-    #         )
-    #         os.makedirs(os.path.join(sns_output_dir, "annotated_geps", "correlation_network", dataset_name), exist_ok=True)
-    #         fig.savefig(os.path.join(sns_output_dir, "annotated_geps", "correlation_network", dataset_name, annotation_layer + ".pdf"))
-    #         fig.savefig(os.path.join(sns_output_dir, "annotated_geps", "correlation_network", dataset_name, annotation_layer + ".png"), dpi=600)
-    #         plt.close(fig)
-
-    # # Community-level Network
-    # logging.info("Creating community network")
-    # edge_list = []
-    # for c1, n1 in communities.items():
-    #     for c2, n2 in communities.items():
-    #         if c1 != c2:  # no self-loops
-    #             n_edges = len(list(nx.edge_boundary(G, n1, n2)))
-    #             edge_list.append((c1, c2, n_edges))
-
-    # edge_list = pd.DataFrame(edge_list, columns = ("comm1", "comm2", "n_edges"))
-    # Gcomm = nx.from_pandas_edgelist(pd.DataFrame(edge_list, columns = ("comm1", "comm2", "n_edges")), "comm1", "comm2", "n_edges")
-    # Gcomm.add_nodes_from(communities.keys())
-    # # Centroid method for community layout
-    # community_layout = {}
-    # for community_name, nodes in communities.items():
-    #     points = np.array([layout[node] for node in nodes])
-    #     centroid = (np.median(points[:, 0]), np.median(points[:, 1]))
-    #     community_layout[community_name] = centroid
-
-    # ### Plot network layout ###
-    # fig, ax = plt.subplots(figsize=config.sns["plot_size_gep"])
-    # ax.set_aspect(1)
-    # if Gcomm.edges:
-    #     width = np.array(list(nx.get_edge_attributes(Gcomm, "n_edges").values()))
-    #     width = 20 * width / np.max(width)
-    # else:
-    #     width = None
-    # sizes = np.array([len(communities[node]) for node in Gcomm.nodes])
-    # sizes = 20 * config.sns["node_size"] * sizes / np.max(sizes)
-    # node_colors = [community_colors[node] for node in Gcomm]
-    # nx.draw(Gcomm, pos=community_layout, node_color=node_colors, node_size=sizes, linewidths=0, width=width, edge_color=config.sns["edge_color"], with_labels=True, font_size=20)
-    # plt.tight_layout()
-    # fig.savefig(os.path.join(sns_output_dir, "community_network.pdf"))
-    # fig.savefig(os.path.join(sns_output_dir, "community_network.png"), dpi=600)
-    # plt.close(fig)
-            
-    # # Community-level overrepresentation plots
-    # logging.info("Creating community network plots for categorical metadata")
-    # plot_data = {}
-    # for dataset_name, dataset in config.datasets.items():
-    #     metadata = read_h5ad(dataset["filename"], backed="r").obs.select_dtypes(include="category").dropna(axis=1, how="all")  # only use categorical data
-    #     for row, (annotation_layer, sample_to_class) in enumerate(metadata.items()):
-    #         # usage subset to dataset
-    #         ds_usage = usage.loc[:, (dataset_name, slice(None), slice(None))].dropna(how="all").droplevel(axis=0, level=0)
-    #         overrepresentation = get_category_overrepresentation(ds_usage, sample_to_class)
-    #         result_df = []
-    #         for col, community in enumerate(sorted(list(communities))):
-    #             geps = []
-    #             for node in communities[community]:
-    #                 dataset_str, k_str, gep_str = node.split("|")
-    #                 if dataset_str == dataset_name:
-    #                     geps.append((dataset_str, int(k_str), int(gep_str)))
-    #             geps = sorted(geps)
-    #             if geps:
-    #                 com_es = overrepresentation[geps].mean(axis=1)
-    #                 com_es[com_es < 0] = 0
-    #             else:
-    #                 com_es = pd.Series(0, index=overrepresentation.index)
-    #             result_df.append(com_es.rename(community))
-    #         result_df = pd.concat(result_df, axis=1)
-    #         plot_data[(dataset_name, annotation_layer)] = result_df
-
-    # for (dataset_name, annotation_layer), community_es in plot_data.items():
-    #     # bar plots
-    #     fig, ax = plt.subplots()
-    #     community_es.T.plot.bar(stacked=True, width=0.9, ax=ax, legend=None, rot=0, color=config.get_metadata_colors(annotation_layer))
-    #     os.makedirs(os.path.join(sns_output_dir, "annotated_communities", "overrepresentation_bar", dataset_name), exist_ok=True)
-    #     fig.savefig(os.path.join(sns_output_dir, "annotated_communities", "overrepresentation_bar", dataset_name, annotation_layer + ".pdf"))
-    #     fig.savefig(os.path.join(sns_output_dir, "annotated_communities", "overrepresentation_bar", dataset_name, annotation_layer + ".png"), dpi=600)
-    #     plt.close(fig)
-
-    #     # network plots
-    #     fig, ax = plt.subplots(figsize=config.sns["plot_size_community"])
-    #     plot_overrepresentation_network(
-    #         graph=Gcomm,
-    #         layout=community_layout,
-    #         title=f"Dataset: {dataset_name}\nAnnotations: {annotation_layer}",
-    #         overrepresentation=community_es,
-    #         colordict=config.get_metadata_colors(annotation_layer),
-    #         pie_size=np.array(config.sns["pie_size_community"]),
-    #         edge_weights="n_edges",
-    #         ax=ax
-    #     )
-    #     os.makedirs(os.path.join(sns_output_dir, "annotated_communities", "overrepresentation_network", dataset_name), exist_ok=True)
-    #     fig.savefig(os.path.join(sns_output_dir, "annotated_communities", "overrepresentation_network", dataset_name, annotation_layer + ".pdf"))
-    #     fig.savefig(os.path.join(sns_output_dir, "annotated_communities", "overrepresentation_network", dataset_name, annotation_layer + ".png"), dpi=600)
-    #     plt.close(fig)
-
-
-    # # Community-level correlation plots
-    # logging.info("Creating community network plots for numerical metadata")
-    # plot_data = {}
-    # for dataset_name, dataset in config.datasets.items():
-    #     metadata = read_h5ad(dataset["filename"], backed="r").obs.select_dtypes(exclude="category").dropna(axis=1, how="all")  # only use categorical data
-    #     for row, (annotation_layer, sample_to_numeric) in enumerate(metadata.items()):
-    #         # usage subset to dataset
-    #         ds_usage = usage.loc[:, (dataset_name, slice(None), slice(None))].dropna(how="all").droplevel(axis=0, level=0)
-    #         correlation = ds_usage.corrwith(sample_to_numeric)
-    #         result = {}
-    #         for col, community in enumerate(sorted(list(communities))):
-    #             geps = []
-    #             for node in communities[community]:
-    #                 dataset_str, k_str, gep_str = node.split("|")
-    #                 if dataset_str == dataset_name:
-    #                     geps.append((dataset_str, int(k_str), int(gep_str)))
-    #             geps = sorted(geps)
-    #             if geps:
-    #                 com_meancorr = correlation[geps].mean()
-    #             else:
-    #                 com_meancorr = 0
-    #             result[community] = com_meancorr
-    #         plot_data[(dataset_name, annotation_layer)] = pd.Series(result).sort_index()
-
-    # for (dataset_name, annotation_layer), community_corr in plot_data.items():
-    #     # bar plots
-    #     fig, ax = plt.subplots()
-    #     community_corr.plot.bar(width=0.9, ax=ax, legend=None, rot=0, ylim=[-1, 1])
-    #     ax.set_ylabel("Pearson correlation")
-    #     os.makedirs(os.path.join(sns_output_dir, "annotated_communities", "correlation_bar", dataset_name), exist_ok=True)
-    #     fig.savefig(os.path.join(sns_output_dir, "annotated_communities", "correlation_bar", dataset_name, annotation_layer + ".pdf"))
-    #     fig.savefig(os.path.join(sns_output_dir, "annotated_communities", "correlation_bar", dataset_name, annotation_layer + ".png"), dpi=600)
-    #     plt.close(fig)
-
-    #     # network plots
-    #     fig = plot_metadata_correlation_network(
-    #         graph=Gcomm,
-    #         layout=community_layout,
-    #         title=f"Dataset: {dataset_name}\nMetadata Layer: {annotation_layer}",
-    #         correlation=community_corr,
-    #         plot_size=config.sns["plot_size_community"],
-    #         node_size=np.array(config.sns["node_size"]),
-    #         edge_weights="n_edges",
-    #         config=config
-    #     )
-    #     os.makedirs(os.path.join(sns_output_dir, "annotated_communities", "correlation_network", dataset_name), exist_ok=True)
-    #     fig.savefig(os.path.join(sns_output_dir, "annotated_communities", "correlation_network", dataset_name, annotation_layer + ".pdf"))
-    #     fig.savefig(os.path.join(sns_output_dir, "annotated_communities", "correlation_network", dataset_name, annotation_layer + ".png"), dpi=600)
-    #     plt.close(fig)
-        
     # for dataset_name, geps in selected_geps.droplevel(axis=1, level=[2,3]).groupby(axis=1, level=1):
     #     geps = geps.droplevel(axis=1, level=1)
     #     geps.columns = geps.columns.astype("int")
     #     for feature in config.features["features_of_interest"]:
     #         if feature in geps.index:
     #             positive_scores = geps.loc[feature].groupby(axis=0, level=0).mean().reindex(communities.keys()).fillna(0).clip(lower=0)
     #             if positive_scores.sum() == 0:
```

### Comparing `cnmfsns-1.3.2/src/cnmfsns/cnmf.py` & `cnmfsns-1.4.0/src/cnmfsns/cnmf.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.2/src/cnmfsns/colors.py` & `cnmfsns-1.4.0/src/cnmfsns/colors.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.2/src/cnmfsns/config.py` & `cnmfsns-1.4.0/src/cnmfsns/config.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.2/src/cnmfsns/dataset.py` & `cnmfsns-1.4.0/src/cnmfsns/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,2104 +93,2148 @@
 000005c0: 2020 2020 2020 2020 206c 6f67 6769 6e67           logging
 000005d0: 2e65 7272 6f72 2866 2261 6461 7461 2063  .error(f"adata c
 000005e0: 6f6e 7461 696e 7320 6e6f 2065 7870 7265  ontains no expre
 000005f0: 7373 696f 6e20 6461 7461 2028 6164 6174  ssion data (adat
 00000600: 612e 5829 2229 0d0a 2020 2020 2020 2020  a.X)")..        
 00000610: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
 00000620: 7272 6f72 2829 0d0a 2020 2020 2020 2020  rror()..        
-00000630: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
-00000640: 6174 6965 6e74 5f69 645f 636f 6c20 3d20  atient_id_col = 
-00000650: 7061 7469 656e 745f 6964 5f63 6f6c 0d0a  patient_id_col..
-00000660: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00000670: 2020 6966 2022 636e 6d66 736e 735f 7665    if "cnmfsns_ve
-00000680: 7273 696f 6e22 2069 6e20 6164 6174 612e  rsion" in adata.
-00000690: 756e 7320 616e 6420 6164 6174 612e 756e  uns and adata.un
-000006a0: 735b 2263 6e6d 6673 6e73 5f76 6572 7369  s["cnmfsns_versi
-000006b0: 6f6e 225d 2069 7320 6e6f 7420 4e6f 6e65  on"] is not None
-000006c0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-000006d0: 656c 662e 6164 6174 6120 3d20 6164 6174  elf.adata = adat
-000006e0: 610d 0a20 2020 2020 2020 2065 6c73 653a  a..        else:
-000006f0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00000700: 6368 6563 6b20 616e 6420 7570 6461 7465  check and update
-00000710: 206f 6c64 206f 7220 6578 7465 726e 616c   old or external
-00000720: 2068 3561 6420 6669 6c65 7320 666f 7220   h5ad files for 
-00000730: 634e 4d46 2d53 4e53 2063 6f6d 706c 6961  cNMF-SNS complia
-00000740: 6e63 650d 0a20 2020 200d 0a20 2020 2020  nce..    ..     
-00000750: 2020 2020 2020 2058 203d 2061 6461 7461         X = adata
-00000760: 2e74 6f5f 6466 2829 0d0a 2020 2020 2020  .to_df()..      
-00000770: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00000780: 2020 2020 6966 2061 6461 7461 2e69 7362      if adata.isb
-00000790: 6163 6b65 643a 0d0a 2020 2020 2020 2020  acked:..        
-000007a0: 2020 2020 2020 2020 7261 6973 6520 5275          raise Ru
-000007b0: 6e74 696d 6545 7272 6f72 2822 6164 6174  ntimeError("adat
-000007c0: 6120 6973 2061 2062 6163 6b65 6420 416e  a is a backed An
-000007d0: 6e44 6174 6120 6f62 6a65 6374 2e20 416e  nData object. An
-000007e0: 6e44 6174 6120 6f62 6a65 6374 7320 6f70  nData objects op
-000007f0: 656e 6564 2069 6e20 6261 636b 6564 206d  ened in backed m
-00000800: 6f64 6520 6361 6e6e 6f74 2062 6520 6d69  ode cannot be mi
-00000810: 6772 6174 6564 2e22 290d 0a0d 0a20 2020  grated.")....   
-00000820: 2020 2020 2020 2020 2069 6620 6164 6174           if adat
-00000830: 612e 7261 7720 6973 204e 6f6e 653a 0d0a  a.raw is None:..
-00000840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000850: 6973 5f6e 6f72 6d61 6c69 7a65 643d 4661  is_normalized=Fa
-00000860: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
-00000870: 2020 2020 2072 6177 203d 2061 6461 7461       raw = adata
-00000880: 2e74 6f5f 6466 2829 0d0a 2020 2020 2020  .to_df()..      
-00000890: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-000008a0: 2020 2020 2020 2020 2020 2020 2072 6177               raw
-000008b0: 203d 2070 642e 4461 7461 4672 616d 6528   = pd.DataFrame(
-000008c0: 6164 6174 612e 7261 772e 582c 2069 6e64  adata.raw.X, ind
-000008d0: 6578 3d58 2e69 6e64 6578 2c20 636f 6c75  ex=X.index, colu
-000008e0: 6d6e 733d 582e 636f 6c75 6d6e 7329 0d0a  mns=X.columns)..
-000008f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000900: 636f 7272 6469 7374 203d 2058 2e63 6f72  corrdist = X.cor
-00000910: 7277 6974 6828 7261 772c 2061 7869 733d  rwith(raw, axis=
-00000920: 3129 0d0a 2020 2020 2020 2020 2020 2020  1)..            
-00000930: 2020 2020 2320 6368 6563 6b73 2074 6861      # checks tha
-00000940: 7420 616c 6c20 7361 6d70 6c65 7320 6172  t all samples ar
-00000950: 6520 7065 7266 6563 746c 7920 636f 7272  e perfectly corr
-00000960: 656c 6174 6564 2062 6574 7765 656e 2063  elated between c
-00000970: 6f75 6e74 7320 616e 6420 6e6f 726d 616c  ounts and normal
-00000980: 697a 6564 2064 6174 610d 0a20 2020 2020  ized data..     
-00000990: 2020 2020 2020 2020 2020 2069 6620 2828             if ((
-000009a0: 636f 7272 6469 7374 202d 2031 292e 6162  corrdist - 1).ab
-000009b0: 7328 2920 3e20 3165 2d36 292e 616e 7928  s() > 1e-6).any(
-000009c0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000009d0: 2020 2020 2020 2020 6c6f 6767 696e 672e          logging.
-000009e0: 7761 726e 696e 6728 2243 6f75 6e74 7320  warning("Counts 
-000009f0: 616e 6420 6e6f 726d 616c 697a 6564 2065  and normalized e
-00000a00: 7870 7265 7373 696f 6e20 6d61 7472 6963  xpression matric
-00000a10: 6573 2061 7265 206e 6f74 2070 6572 6665  es are not perfe
-00000a20: 6374 6c79 2063 6f72 7265 6c61 7465 642e  ctly correlated.
-00000a30: 2043 6f75 6e74 7320 6461 7461 2077 696c   Counts data wil
-00000a40: 6c20 6265 2072 6574 6169 6e65 6420 696e  l be retained in
-00000a50: 206d 6967 7261 7465 6420 6f62 6a65 6374   migrated object
-00000a60: 2e22 290d 0a20 2020 2020 2020 2020 2020  .")..           
-00000a70: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00000a80: 666f 7263 655f 6d69 6772 6174 653a 0d0a  force_migrate:..
-00000a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000aa0: 2020 2020 2020 2020 6572 726f 726d 7367          errormsg
-00000ab0: 203d 2022 436f 756c 6420 6e6f 7420 6d69   = "Could not mi
-00000ac0: 6772 6174 6520 416e 6e44 6174 6120 6f62  grate AnnData ob
-00000ad0: 6a65 6374 2e22 0d0a 2020 2020 2020 2020  ject."..        
+00000630: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00000640: 2020 2020 6966 2022 636e 6d66 736e 735f      if "cnmfsns_
+00000650: 7665 7273 696f 6e22 2069 6e20 6164 6174  version" in adat
+00000660: 612e 756e 7320 616e 6420 6164 6174 612e  a.uns and adata.
+00000670: 756e 735b 2263 6e6d 6673 6e73 5f76 6572  uns["cnmfsns_ver
+00000680: 7369 6f6e 225d 2069 7320 6e6f 7420 4e6f  sion"] is not No
+00000690: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+000006a0: 2073 656c 662e 6164 6174 6120 3d20 6164   self.adata = ad
+000006b0: 6174 610d 0a20 2020 2020 2020 2065 6c73  ata..        els
+000006c0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000006d0: 2320 6368 6563 6b20 616e 6420 7570 6461  # check and upda
+000006e0: 7465 206f 6c64 206f 7220 6578 7465 726e  te old or extern
+000006f0: 616c 2068 3561 6420 6669 6c65 7320 666f  al h5ad files fo
+00000700: 7220 634e 4d46 2d53 4e53 2063 6f6d 706c  r cNMF-SNS compl
+00000710: 6961 6e63 650d 0a20 2020 200d 0a20 2020  iance..    ..   
+00000720: 2020 2020 2020 2020 2058 203d 2061 6461           X = ada
+00000730: 7461 2e74 6f5f 6466 2829 0d0a 2020 2020  ta.to_df()..    
+00000740: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00000750: 2020 2020 2020 6966 2061 6461 7461 2e69        if adata.i
+00000760: 7362 6163 6b65 643a 0d0a 2020 2020 2020  sbacked:..      
+00000770: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00000780: 5275 6e74 696d 6545 7272 6f72 2822 6164  RuntimeError("ad
+00000790: 6174 6120 6973 2061 2062 6163 6b65 6420  ata is a backed 
+000007a0: 416e 6e44 6174 6120 6f62 6a65 6374 2e20  AnnData object. 
+000007b0: 416e 6e44 6174 6120 6f62 6a65 6374 7320  AnnData objects 
+000007c0: 6f70 656e 6564 2069 6e20 6261 636b 6564  opened in backed
+000007d0: 206d 6f64 6520 6361 6e6e 6f74 2062 6520   mode cannot be 
+000007e0: 6d69 6772 6174 6564 2e22 290d 0a0d 0a20  migrated.").... 
+000007f0: 2020 2020 2020 2020 2020 2069 6620 6164             if ad
+00000800: 6174 612e 7261 7720 6973 204e 6f6e 653a  ata.raw is None:
+00000810: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000820: 2020 6973 5f6e 6f72 6d61 6c69 7a65 643d    is_normalized=
+00000830: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
+00000840: 2020 2020 2020 2072 6177 203d 2061 6461         raw = ada
+00000850: 7461 2e74 6f5f 6466 2829 0d0a 2020 2020  ta.to_df()..    
+00000860: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00000870: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00000880: 6177 203d 2070 642e 4461 7461 4672 616d  aw = pd.DataFram
+00000890: 6528 6164 6174 612e 7261 772e 582c 2069  e(adata.raw.X, i
+000008a0: 6e64 6578 3d58 2e69 6e64 6578 2c20 636f  ndex=X.index, co
+000008b0: 6c75 6d6e 733d 582e 636f 6c75 6d6e 7329  lumns=X.columns)
+000008c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000008d0: 2020 636f 7272 6469 7374 203d 2058 2e63    corrdist = X.c
+000008e0: 6f72 7277 6974 6828 7261 772c 2061 7869  orrwith(raw, axi
+000008f0: 733d 3129 0d0a 2020 2020 2020 2020 2020  s=1)..          
+00000900: 2020 2020 2020 2320 6368 6563 6b73 2074        # checks t
+00000910: 6861 7420 616c 6c20 7361 6d70 6c65 7320  hat all samples 
+00000920: 6172 6520 7065 7266 6563 746c 7920 636f  are perfectly co
+00000930: 7272 656c 6174 6564 2062 6574 7765 656e  rrelated between
+00000940: 2063 6f75 6e74 7320 616e 6420 6e6f 726d   counts and norm
+00000950: 616c 697a 6564 2064 6174 610d 0a20 2020  alized data..   
+00000960: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00000970: 2828 636f 7272 6469 7374 202d 2031 292e  ((corrdist - 1).
+00000980: 6162 7328 2920 3e20 3165 2d36 292e 616e  abs() > 1e-6).an
+00000990: 7928 293a 0d0a 2020 2020 2020 2020 2020  y():..          
+000009a0: 2020 2020 2020 2020 2020 6c6f 6767 696e            loggin
+000009b0: 672e 7761 726e 696e 6728 2243 6f75 6e74  g.warning("Count
+000009c0: 7320 616e 6420 6e6f 726d 616c 697a 6564  s and normalized
+000009d0: 2065 7870 7265 7373 696f 6e20 6d61 7472   expression matr
+000009e0: 6963 6573 2061 7265 206e 6f74 2070 6572  ices are not per
+000009f0: 6665 6374 6c79 2063 6f72 7265 6c61 7465  fectly correlate
+00000a00: 642e 2043 6f75 6e74 7320 6461 7461 2077  d. Counts data w
+00000a10: 696c 6c20 6265 2072 6574 6169 6e65 6420  ill be retained 
+00000a20: 696e 206d 6967 7261 7465 6420 6f62 6a65  in migrated obje
+00000a30: 6374 2e22 290d 0a20 2020 2020 2020 2020  ct.")..         
+00000a40: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00000a50: 7420 666f 7263 655f 6d69 6772 6174 653a  t force_migrate:
+00000a60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000a70: 2020 2020 2020 2020 2020 6572 726f 726d            errorm
+00000a80: 7367 203d 2022 436f 756c 6420 6e6f 7420  sg = "Could not 
+00000a90: 6d69 6772 6174 6520 416e 6e44 6174 6120  migrate AnnData 
+00000aa0: 6f62 6a65 6374 2e22 0d0a 2020 2020 2020  object."..      
+00000ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ac0: 2020 6c6f 6767 696e 672e 6572 726f 7228    logging.error(
+00000ad0: 6572 726f 726d 7367 290d 0a20 2020 2020  errormsg)..     
 00000ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000af0: 6c6f 6767 696e 672e 6572 726f 7228 6572  logging.error(er
-00000b00: 726f 726d 7367 290d 0a20 2020 2020 2020  rormsg)..       
-00000b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b20: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00000b30: 7228 6572 726f 726d 7367 290d 0a20 2020  r(errormsg)..   
-00000b40: 2020 2020 2020 2020 2020 2020 2023 2063               # c
-00000b50: 6865 636b 2066 6f72 2077 6865 7468 6572  heck for whether
-00000b60: 2075 7365 7220 6f72 6967 696e 616c 6c79   user originally
-00000b70: 2069 6e70 7574 206e 6f72 6d61 6c69 7a65   input normalize
-00000b80: 6420 6f72 2063 6f75 6e74 7320 6461 7461  d or counts data
-00000b90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000ba0: 2020 6973 5f6e 6f72 6d61 6c69 7a65 6420    is_normalized 
-00000bb0: 3d20 2828 5820 2d20 7261 7729 2e61 6273  = ((X - raw).abs
-00000bc0: 2829 203c 2031 652d 3629 2e61 6c6c 2829  () < 1e-6).all()
-00000bd0: 2e61 6c6c 2829 0d0a 2020 2020 2020 2020  .all()..        
-00000be0: 2020 2020 2020 2020 585f 6973 5f74 706d          X_is_tpm
-00000bf0: 203d 2028 2858 2e73 756d 2861 7869 733d   = ((X.sum(axis=
-00000c00: 3129 202d 2031 6536 292e 6162 7328 2920  1) - 1e6).abs() 
-00000c10: 3e20 3165 3229 2e61 6e79 2829 0d0a 2020  > 1e2).any()..  
-00000c20: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00000c30: 2069 735f 6e6f 726d 616c 697a 6564 2061   is_normalized a
-00000c40: 6e64 206e 6f74 2058 5f69 735f 7470 6d3a  nd not X_is_tpm:
-00000c50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000c60: 2020 2020 2020 6c6f 6767 696e 672e 7761        logging.wa
-00000c70: 726e 696e 6728 2241 6e6e 4461 7461 206f  rning("AnnData o
-00000c80: 626a 6563 7420 636f 6e74 6169 6e73 206e  bject contains n
-00000c90: 6f6e 2d54 504d 206e 6f72 6d61 6c69 7a65  on-TPM normalize
-00000ca0: 6420 6461 7461 2e20 4e65 7720 416e 6e44  d data. New AnnD
-00000cb0: 6174 6120 6f62 6a65 6374 2077 696c 6c20  ata object will 
-00000cc0: 7265 7461 696e 2074 6865 2063 6f75 6e74  retain the count
-00000cd0: 2028 756e 6e6f 726d 616c 697a 6564 2920   (unnormalized) 
-00000ce0: 6461 7461 206f 6e6c 792e 2229 0d0a 2020  data only.")..  
-00000cf0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00000d00: 2020 2020 2020 2020 2020 2020 6966 2022              if "
-00000d10: 6f64 6722 2069 6e20 6164 6174 612e 756e  odg" in adata.un
-00000d20: 7320 616e 6420 2267 656e 655f 7374 6174  s and "gene_stat
-00000d30: 7322 2069 6e20 6164 6174 612e 756e 735b  s" in adata.uns[
-00000d40: 226f 6467 225d 3a0d 0a20 2020 2020 2020  "odg"]:..       
-00000d50: 2020 2020 2020 2020 2067 656e 655f 7374           gene_st
-00000d60: 6174 5f63 6f6c 756d 6e73 203d 2061 6461  at_columns = ada
-00000d70: 7461 2e75 6e73 5b22 6f64 6722 5d5b 2267  ta.uns["odg"]["g
-00000d80: 656e 655f 7374 6174 7322 5d2e 636f 6c75  ene_stats"].colu
-00000d90: 6d6e 730d 0a20 2020 2020 2020 2020 2020  mns..           
-00000da0: 2020 2020 2069 6620 6164 6174 612e 7661       if adata.va
-00000db0: 722e 636f 6c75 6d6e 732e 6973 696e 2867  r.columns.isin(g
-00000dc0: 656e 655f 7374 6174 5f63 6f6c 756d 6e73  ene_stat_columns
-00000dd0: 292e 616e 7928 293a 0d0a 2020 2020 2020  ).any():..      
-00000de0: 2020 2020 2020 2020 2020 2020 2020 6f76                ov
-00000df0: 6572 6c61 7070 696e 675f 636f 6c73 203d  erlapping_cols =
-00000e00: 2061 6461 7461 2e76 6172 2e63 6f6c 756d   adata.var.colum
-00000e10: 6e73 2e69 7369 6e28 6765 6e65 5f73 7461  ns.isin(gene_sta
-00000e20: 745f 636f 6c75 6d6e 7329 0d0a 2020 2020  t_columns)..    
-00000e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e40: 6f76 6572 6c61 7070 696e 675f 636f 6c73  overlapping_cols
-00000e50: 7472 203d 2022 2c20 222e 6a6f 696e 286f  tr = ", ".join(o
-00000e60: 7665 726c 6170 7069 6e67 5f63 6f6c 735b  verlapping_cols[
-00000e70: 6f76 6572 6c61 7070 696e 675f 636f 6c73  overlapping_cols
-00000e80: 5d2e 696e 6465 782e 746f 5f6c 6973 7428  ].index.to_list(
-00000e90: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00000ea0: 2020 2020 2020 2020 6c6f 6767 696e 672e          logging.
-00000eb0: 7761 726e 696e 6728 6622 416e 6e44 6174  warning(f"AnnDat
-00000ec0: 6120 6f62 6a65 6374 2063 6f6e 7461 696e  a object contain
-00000ed0: 7320 634e 4d46 2067 656e 6520 7374 6174  s cNMF gene stat
-00000ee0: 7320 7768 6963 6820 7769 6c6c 206f 7665  s which will ove
-00000ef0: 7272 6964 6520 636f 6c75 6d6e 7320 696e  rride columns in
-00000f00: 2061 6461 7461 2e76 6172 3a20 7b6f 7665   adata.var: {ove
-00000f10: 726c 6170 7069 6e67 5f63 6f6c 7374 727d  rlapping_colstr}
-00000f20: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-00000f30: 2020 2020 6164 6174 612e 7661 7220 3d20      adata.var = 
-00000f40: 7064 2e6d 6572 6765 286c 6566 743d 6164  pd.merge(left=ad
-00000f50: 6174 612e 7661 722c 2072 6967 6874 3d61  ata.var, right=a
-00000f60: 6461 7461 2e75 6e73 5b22 6f64 6722 5d5b  data.uns["odg"][
-00000f70: 2267 656e 655f 7374 6174 7322 5d2c 2068  "gene_stats"], h
-00000f80: 6f77 3d22 6c65 6674 222c 206c 6566 745f  ow="left", left_
-00000f90: 696e 6465 783d 5472 7565 2c20 7269 6768  index=True, righ
-00000fa0: 745f 696e 6465 783d 5472 7565 290d 0a20  t_index=True).. 
-00000fb0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00000fc0: 656c 2061 6461 7461 2e75 6e73 5b22 6f64  el adata.uns["od
-00000fd0: 6722 5d5b 2267 656e 655f 7374 6174 7322  g"]["gene_stats"
-00000fe0: 5d0d 0a20 2020 2020 2020 2020 2020 200d  ]..            .
-00000ff0: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
-00001000: 7265 6174 6520 6e65 7720 416e 6e44 6174  reate new AnnDat
-00001010: 6120 6f62 6a65 6374 0d0a 2020 2020 2020  a object..      
-00001020: 2020 2020 2020 6e65 775f 6164 6174 6120        new_adata 
-00001030: 3d20 6164 2e41 6e6e 4461 7461 2858 3d72  = ad.AnnData(X=r
-00001040: 6177 2c20 6f62 733d 6164 6174 612e 6f62  aw, obs=adata.ob
-00001050: 732c 2076 6172 3d61 6461 7461 2e76 6172  s, var=adata.var
-00001060: 2c20 7661 726d 3d61 6461 7461 2e76 6172  , varm=adata.var
-00001070: 6d2c 206f 6273 6d3d 6164 6174 612e 6f62  m, obsm=adata.ob
-00001080: 736d 2c20 756e 733d 6164 6174 612e 756e  sm, uns=adata.un
-00001090: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
-000010a0: 6966 2022 6869 7374 6f72 7922 206e 6f74  if "history" not
-000010b0: 2069 6e20 6e65 775f 6164 6174 612e 756e   in new_adata.un
-000010c0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-000010d0: 2020 2020 6e65 775f 6164 6174 612e 756e      new_adata.un
-000010e0: 735b 2268 6973 746f 7279 225d 203d 207b  s["history"] = {
-000010f0: 7d0d 0a0d 0a20 2020 2020 2020 2020 2020  }....           
-00001100: 2023 2075 7064 6174 6520 6461 7461 7365   # update datase
-00001110: 7420 6f62 6a65 6374 0d0a 2020 2020 2020  t object..      
-00001120: 2020 2020 2020 7365 6c66 2e61 6461 7461        self.adata
-00001130: 203d 206e 6577 5f61 6461 7461 0d0a 2020   = new_adata..  
-00001140: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
-00001150: 735f 6e6f 726d 616c 697a 6564 203d 2069  s_normalized = i
-00001160: 735f 6e6f 726d 616c 697a 6564 0d0a 2020  s_normalized..  
-00001170: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00001180: 6e6d 6673 6e73 5f76 6572 7369 6f6e 203d  nmfsns_version =
-00001190: 205f 5f76 6572 7369 6f6e 5f5f 0d0a 2020   __version__..  
-000011a0: 2020 0d0a 2020 2020 4063 6c61 7373 6d65    ..    @classme
-000011b0: 7468 6f64 0d0a 2020 2020 6465 6620 6672  thod..    def fr
-000011c0: 6f6d 5f64 6628 636c 732c 0d0a 2020 2020  om_df(cls,..    
-000011d0: 2020 2020 2020 2020 2020 2020 2020 6461                da
-000011e0: 7461 3a20 7064 2e44 6174 6146 7261 6d65  ta: pd.DataFrame
-000011f0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00001200: 2020 2020 2069 735f 6e6f 726d 616c 697a       is_normaliz
-00001210: 6564 3a20 626f 6f6c 2c0d 0a20 2020 2020  ed: bool,..     
-00001220: 2020 2020 2020 2020 2020 2020 2073 7061               spa
-00001230: 7273 6966 793a 2062 6f6f 6c20 3d20 4661  rsify: bool = Fa
-00001240: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
-00001250: 2020 2020 2020 2020 6f62 733a 204f 7074          obs: Opt
-00001260: 696f 6e61 6c5b 7064 2e44 6174 6146 7261  ional[pd.DataFra
-00001270: 6d65 5d20 3d20 4e6f 6e65 2c0d 0a20 2020  me] = None,..   
-00001280: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-00001290: 6172 3a20 4f70 7469 6f6e 616c 5b70 642e  ar: Optional[pd.
-000012a0: 4461 7461 4672 616d 655d 203d 204e 6f6e  DataFrame] = Non
-000012b0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-000012c0: 2020 2020 2020 7061 7469 656e 745f 6964        patient_id
-000012d0: 5f63 6f6c 3a20 4f70 7469 6f6e 616c 5b73  _col: Optional[s
-000012e0: 7472 5d20 3d20 4e6f 6e65 0d0a 2020 2020  tr] = None..    
-000012f0: 2020 2020 2020 2020 2020 2020 2020 293a                ):
-00001300: 0d0a 2020 2020 2020 2020 2222 2243 7265  ..        """Cre
-00001310: 6174 6573 2061 203a 636c 6173 733a 607e  ates a :class:`~
-00001320: 636e 6d66 736e 732e 6461 7461 7365 742e  cnmfsns.dataset.
-00001330: 4461 7461 7365 7460 206f 626a 6563 7420  Dataset` object 
-00001340: 6672 6f6d 2061 2070 616e 6461 7320 4461  from a pandas Da
-00001350: 7461 4672 616d 652e 0d0a 0d0a 2020 2020  taFrame.....    
-00001360: 2020 2020 3a70 6172 616d 2064 6174 613a      :param data:
-00001370: 2041 6e20 6f62 7365 7276 6174 696f 6e73   An observations
-00001380: 20c3 9720 7661 7269 6162 6c65 7320 6461   .. variables da
-00001390: 7461 0d0a 2020 2020 2020 2020 3a74 7970  ta..        :typ
-000013a0: 6520 6461 7461 3a20 7064 2e44 6174 6146  e data: pd.DataF
-000013b0: 7261 6d65 0d0a 2020 2020 2020 2020 3a70  rame..        :p
-000013c0: 6172 616d 2069 735f 6e6f 726d 616c 697a  aram is_normaliz
-000013d0: 6564 3a20 5370 6563 6966 7920 6966 2064  ed: Specify if d
-000013e0: 6174 6120 6973 2061 6c72 6561 6479 206e  ata is already n
-000013f0: 6f72 6d61 6c69 7a65 6420 6f72 2077 6865  ormalized or whe
-00001400: 7468 6572 206e 6f74 2e20 5261 7720 6461  ther not. Raw da
-00001410: 7461 2077 696c 6c20 6265 2054 504d 206e  ta will be TPM n
-00001420: 6f72 6d61 6c69 7a65 6420 7072 696f 7220  ormalized prior 
-00001430: 746f 206f 7665 7264 6973 7065 7273 6564  to overdispersed
-00001440: 2067 656e 6520 7365 6c65 6374 696f 6e2c   gene selection,
-00001450: 2077 6865 7265 6173 2061 6c72 6561 6479   whereas already
-00001460: 206e 6f72 6d61 6c69 7a65 6420 6461 7461   normalized data
-00001470: 2077 696c 6c20 6e6f 742e 0d0a 2020 2020   will not...    
-00001480: 2020 2020 3a74 7970 6520 6973 5f6e 6f72      :type is_nor
-00001490: 6d61 6c69 7a65 643a 2062 6f6f 6c0d 0a20  malized: bool.. 
-000014a0: 2020 2020 2020 203a 7061 7261 6d20 7370         :param sp
-000014b0: 6172 7369 6679 3a20 5374 6f72 6520 6461  arsify: Store da
-000014c0: 7461 2061 7320 6120 7370 6172 7365 206d  ta as a sparse m
-000014d0: 6174 7269 782e 205b 4e6f 7465 2074 6861  atrix. [Note tha
-000014e0: 7420 7468 6973 2066 6561 7475 7265 2069  t this feature i
-000014f0: 7320 6578 7065 7269 6d65 6e74 616c 5d2c  s experimental],
-00001500: 2064 6566 6175 6c74 7320 746f 2046 616c   defaults to Fal
-00001510: 7365 0d0a 2020 2020 2020 2020 3a74 7970  se..        :typ
-00001520: 6520 7370 6172 7369 6679 3a20 626f 6f6c  e sparsify: bool
-00001530: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
-00001540: 2020 2020 3a70 6172 616d 206f 6273 3a20      :param obs: 
-00001550: 416e 206f 6273 6572 7661 7469 6f6e 7320  An observations 
-00001560: c397 206d 6574 6164 6174 6120 6d61 7472  .. metadata matr
-00001570: 6978 2c20 6465 6661 756c 7473 2074 6f20  ix, defaults to 
-00001580: 4e6f 6e65 0d0a 2020 2020 2020 2020 3a74  None..        :t
-00001590: 7970 6520 6f62 733a 2060 7064 2e44 6174  ype obs: `pd.Dat
-000015a0: 6146 7261 6d65 602c 206f 7074 696f 6e61  aFrame`, optiona
-000015b0: 6c0d 0a20 2020 2020 2020 203a 7061 7261  l..        :para
-000015c0: 6d20 7661 723a 2041 2076 6172 6961 626c  m var: A variabl
-000015d0: 6573 20c3 9720 6d65 7461 6461 7461 206d  es .. metadata m
-000015e0: 6174 7269 782c 2064 6566 6175 6c74 7320  atrix, defaults 
-000015f0: 746f 204e 6f6e 650d 0a20 2020 2020 2020  to None..       
-00001600: 203a 7479 7065 2076 6172 3a20 6070 642e   :type var: `pd.
-00001610: 4461 7461 4672 616d 6560 2c20 6f70 7469  DataFrame`, opti
-00001620: 6f6e 616c 0d0a 2020 2020 2020 2020 3a70  onal..        :p
-00001630: 6172 616d 2070 6174 6965 6e74 5f69 645f  aram patient_id_
-00001640: 636f 6c3a 204e 616d 6520 6f66 206d 6574  col: Name of met
-00001650: 6164 6174 6120 6c61 7965 7220 7769 7468  adata layer with
-00001660: 2070 6174 6965 6e74 2049 4420 696e 666f   patient ID info
-00001670: 726d 6174 696f 6e2c 2064 6566 6175 6c74  rmation, default
-00001680: 7320 746f 204e 6f6e 650d 0a20 2020 2020  s to None..     
-00001690: 2020 203a 7479 7065 2070 6174 6965 6e74     :type patient
-000016a0: 5f69 645f 636f 6c3a 2073 7472 2c20 6f70  _id_col: str, op
-000016b0: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
-000016c0: 3a72 6574 7572 6e3a 204f 626a 6563 7420  :return: Object 
-000016d0: 7769 7468 2065 7870 7265 7373 696f 6e20  with expression 
-000016e0: 616e 6420 6d65 7461 6461 7461 0d0a 2020  and metadata..  
-000016f0: 2020 2020 2020 3a72 7479 7065 3a20 3a63        :rtype: :c
-00001700: 6c61 7373 3a60 7e63 6e6d 6673 6e73 2e64  lass:`~cnmfsns.d
-00001710: 6174 6173 6574 2e44 6174 6173 6574 600d  ataset.Dataset`.
-00001720: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00001730: 2020 2020 2020 6966 2076 6172 2069 7320        if var is 
-00001740: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-00001750: 2020 2020 2020 2076 6172 203d 2076 6172         var = var
-00001760: 2e72 6569 6e64 6578 2864 6174 612e 636f  .reindex(data.co
-00001770: 6c75 6d6e 7329 0d0a 2020 2020 2020 2020  lumns)..        
-00001780: 6966 2073 7061 7273 6966 793a 0d0a 2020  if sparsify:..  
-00001790: 2020 2020 2020 2020 2020 6461 7461 203d            data =
-000017a0: 2073 702e 6373 725f 6d61 7472 6978 2864   sp.csr_matrix(d
-000017b0: 6174 612e 7661 6c75 6573 290d 0a20 2020  ata.values)..   
-000017c0: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
-000017d0: 2e61 7374 7970 6528 2266 6c6f 6174 3332  .astype("float32
-000017e0: 2229 0d0a 2020 2020 2020 2020 756e 7320  ")..        uns 
-000017f0: 3d20 7b22 6869 7374 6f72 7922 3a20 7b7d  = {"history": {}
-00001800: 2c20 226f 6467 223a 7b7d 7d0d 0a20 2020  , "odg":{}}..   
-00001810: 2020 2020 2061 6461 7461 203d 2061 642e       adata = ad.
-00001820: 416e 6e44 6174 6128 583d 6461 7461 2c20  AnnData(X=data, 
-00001830: 7661 723d 7661 722c 2075 6e73 3d75 6e73  var=var, uns=uns
-00001840: 290d 0a20 2020 2020 2020 2064 6174 6173  )..        datas
-00001850: 6574 203d 2063 6c73 2861 6461 7461 3d61  et = cls(adata=a
-00001860: 6461 7461 2c20 7061 7469 656e 745f 6964  data, patient_id
-00001870: 5f63 6f6c 3d70 6174 6965 6e74 5f69 645f  _col=patient_id_
-00001880: 636f 6c29 0d0a 2020 2020 2020 2020 6966  col)..        if
-00001890: 206f 6273 2069 7320 6e6f 7420 4e6f 6e65   obs is not None
-000018a0: 3a0d 0a20 2020 2020 2020 2020 2020 2064  :..            d
-000018b0: 6174 6173 6574 2e75 7064 6174 655f 6f62  ataset.update_ob
-000018c0: 7328 6f62 733d 6f62 7329 200d 0a20 2020  s(obs=obs) ..   
-000018d0: 2020 2020 2072 6574 7572 6e20 6461 7461       return data
-000018e0: 7365 740d 0a20 2020 200d 0a20 2020 2040  set..    ..    @
-000018f0: 636c 6173 736d 6574 686f 640d 0a20 2020  classmethod..   
-00001900: 2064 6566 2066 726f 6d5f 6835 6164 2863   def from_h5ad(c
-00001910: 6c73 2c0d 0a20 2020 2020 2020 2020 2020  ls,..           
-00001920: 2020 2020 2020 2068 3561 645f 6669 6c65         h5ad_file
-00001930: 3a20 7374 722c 0d0a 2020 2020 2020 2020  : str,..        
-00001940: 2020 2020 2020 2020 2020 6e61 6d65 3a20            name: 
-00001950: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00001960: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2020  None,..         
-00001970: 2020 2020 2020 2020 2070 6174 6965 6e74           patient
-00001980: 5f69 645f 636f 6c3a 204f 7074 696f 6e61  _id_col: Optiona
-00001990: 6c5b 7374 725d 203d 204e 6f6e 652c 0d0a  l[str] = None,..
-000019a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019b0: 2020 666f 7263 655f 6d69 6772 6174 653d    force_migrate=
-000019c0: 4661 6c73 652c 2062 6163 6b65 643d 4661  False, backed=Fa
-000019d0: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
-000019e0: 2020 2020 2020 2029 3a0d 0a20 2020 2020         ):..     
-000019f0: 2020 2022 2222 4372 6561 7465 7320 6120     """Creates a 
-00001a00: 3a63 6c61 7373 3a60 7e63 6e6d 6673 6e73  :class:`~cnmfsns
-00001a10: 2e64 6174 6173 6574 2e44 6174 6173 6574  .dataset.Dataset
-00001a20: 6020 6f62 6a65 6374 2066 726f 6d20 616e  ` object from an
-00001a30: 2041 6e6e 4461 7461 2d63 6f6d 7061 7469   AnnData-compati
-00001a40: 626c 6520 2e68 3561 6420 6669 6c65 2e0d  ble .h5ad file..
-00001a50: 0a0d 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-00001a60: 6d20 6835 6164 5f66 696c 653a 2050 6174  m h5ad_file: Pat
-00001a70: 6820 746f 202e 6835 6164 2066 696c 6520  h to .h5ad file 
-00001a80: 7072 6f64 7563 6564 2062 7920 7363 616e  produced by scan
-00001a90: 7079 2c20 416e 6e44 6174 612c 206f 7220  py, AnnData, or 
-00001aa0: 634e 4d46 2d53 4e53 0d0a 2020 2020 2020  cNMF-SNS..      
-00001ab0: 2020 3a74 7970 6520 6835 6164 5f66 696c    :type h5ad_fil
-00001ac0: 653a 2073 7472 0d0a 2020 2020 2020 2020  e: str..        
-00001ad0: 3a70 6172 616d 2070 6174 6965 6e74 5f69  :param patient_i
-00001ae0: 645f 636f 6c3a 204e 616d 6520 6f66 206d  d_col: Name of m
-00001af0: 6574 6164 6174 6120 6c61 7965 7220 7769  etadata layer wi
-00001b00: 7468 2070 6174 6965 6e74 2049 4420 696e  th patient ID in
-00001b10: 666f 726d 6174 696f 6e2c 2064 6566 6175  formation, defau
-00001b20: 6c74 7320 746f 204e 6f6e 650d 0a20 2020  lts to None..   
-00001b30: 2020 2020 203a 7479 7065 2070 6174 6965       :type patie
-00001b40: 6e74 5f69 645f 636f 6c3a 2073 7472 2c20  nt_id_col: str, 
-00001b50: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
-00001b60: 2020 3a70 6172 616d 2066 6f72 6365 5f6d    :param force_m
-00001b70: 6967 7261 7465 3a20 666f 7263 6573 2063  igrate: forces c
-00001b80: 6f6e 7665 7273 696f 6e20 6f66 2041 6e6e  onversion of Ann
-00001b90: 4461 7461 206f 626a 6563 7473 2065 7665  Data objects eve
-00001ba0: 6e20 7768 656e 2061 6461 7461 2e58 2061  n when adata.X a
-00001bb0: 6e64 2061 6461 7461 2e72 6177 2e58 2061  nd adata.raw.X a
-00001bc0: 7265 206e 6f74 206c 696e 6561 726c 7920  re not linearly 
-00001bd0: 7363 616c 6564 2072 656c 6174 6976 6520  scaled relative 
-00001be0: 746f 2065 6163 6820 6f74 6865 722c 2064  to each other, d
-00001bf0: 6566 6175 6c74 7320 746f 2046 616c 7365  efaults to False
-00001c00: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00001c10: 666f 7263 655f 6d69 6772 6174 653a 2062  force_migrate: b
-00001c20: 6f6f 6c2c 206f 7074 696f 6e61 6c0d 0a20  ool, optional.. 
-00001c30: 2020 2020 2020 203a 7061 7261 6d20 6261         :param ba
-00001c40: 636b 6564 3a20 5573 6520 6261 636b 6564  cked: Use backed
-00001c50: 206d 6f64 6520 746f 206f 7065 6e20 6835   mode to open h5
-00001c60: 6164 2066 696c 652e 2054 6869 7320 6361  ad file. This ca
-00001c70: 6e20 7361 7665 206d 656d 6f72 7920 7768  n save memory wh
-00001c80: 656e 2074 6865 2064 6174 6173 6574 2069  en the dataset i
-00001c90: 7320 7665 7279 206c 6172 6765 2c20 6275  s very large, bu
-00001ca0: 7420 6973 206e 6f74 2063 6f6d 7061 7469  t is not compati
-00001cb0: 626c 6520 7769 7468 2068 3561 6420 6669  ble with h5ad fi
-00001cc0: 6c65 7320 7072 6f64 7563 6564 206f 7574  les produced out
-00001cd0: 7369 6465 206f 6620 634e 4d46 2d53 4e53  side of cNMF-SNS
-00001ce0: 2c20 6465 6661 756c 7473 2074 6f20 4661  , defaults to Fa
-00001cf0: 6c73 650d 0a20 2020 2020 2020 203a 7479  lse..        :ty
-00001d00: 7065 2062 6163 6b65 643a 2062 6f6f 6c2c  pe backed: bool,
-00001d10: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
-00001d20: 2020 203a 7265 7475 726e 3a20 4f62 6a65     :return: Obje
-00001d30: 6374 2077 6974 6820 6578 7072 6573 7369  ct with expressi
-00001d40: 6f6e 2061 6e64 206d 6574 6164 6174 610d  on and metadata.
-00001d50: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00001d60: 203a 636c 6173 733a 607e 636e 6d66 736e   :class:`~cnmfsn
-00001d70: 732e 6461 7461 7365 742e 4461 7461 7365  s.dataset.Datase
-00001d80: 7460 0d0a 2020 2020 2020 2020 2222 220d  t`..        """.
-00001d90: 0a20 2020 2020 2020 2061 6461 7461 203d  .        adata =
-00001da0: 2061 642e 7265 6164 5f68 3561 6428 6835   ad.read_h5ad(h5
-00001db0: 6164 5f66 696c 652c 2062 6163 6b65 643d  ad_file, backed=
-00001dc0: 6261 636b 6564 290d 0a20 2020 2020 2020  backed)..       
-00001dd0: 2064 6174 6173 6574 203d 2044 6174 6173   dataset = Datas
-00001de0: 6574 2861 6461 7461 3d61 6461 7461 2c20  et(adata=adata, 
-00001df0: 7061 7469 656e 745f 6964 5f63 6f6c 3d70  patient_id_col=p
-00001e00: 6174 6965 6e74 5f69 645f 636f 6c2c 2066  atient_id_col, f
-00001e10: 6f72 6365 5f6d 6967 7261 7465 3d66 6f72  orce_migrate=for
-00001e20: 6365 5f6d 6967 7261 7465 290d 0a20 2020  ce_migrate)..   
-00001e30: 2020 2020 2072 6574 7572 6e20 6461 7461       return data
-00001e40: 7365 740d 0a20 2020 200d 0a20 2020 2040  set..    ..    @
-00001e50: 7072 6f70 6572 7479 0d0a 2020 2020 6465  property..    de
-00001e60: 6620 6973 5f6e 6f72 6d61 6c69 7a65 6428  f is_normalized(
-00001e70: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00001e80: 2222 224f 7574 7075 7473 2074 6865 206e  """Outputs the n
-00001e90: 6f72 6d61 6c69 7a61 7469 6f6e 2073 7461  ormalization sta
-00001ea0: 7475 7320 6f66 2074 6865 2064 6174 6173  tus of the datas
-00001eb0: 6574 2e0d 0a0d 0a20 2020 2020 2020 203a  et.....        :
-00001ec0: 7265 7475 726e 3a20 5472 7565 2069 6620  return: True if 
-00001ed0: 6461 7461 7365 7420 636f 6e74 6169 6e73  dataset contains
-00001ee0: 206e 6f72 6d61 6c69 7a65 6420 6461 7461   normalized data
-00001ef0: 2c20 4661 6c73 6520 6966 2069 7420 6973  , False if it is
-00001f00: 2072 6177 2064 6174 612e 0d0a 2020 2020   raw data...    
-00001f10: 2020 2020 3a72 7479 7065 3a20 626f 6f6c      :rtype: bool
-00001f20: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00001f30: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00001f40: 6c66 2e61 6461 7461 2e75 6e73 5b22 6973  lf.adata.uns["is
-00001f50: 5f6e 6f72 6d61 6c69 7a65 6422 5d0d 0a20  _normalized"].. 
-00001f60: 2020 200d 0a20 2020 2040 6973 5f6e 6f72     ..    @is_nor
-00001f70: 6d61 6c69 7a65 642e 7365 7474 6572 0d0a  malized.setter..
-00001f80: 2020 2020 6465 6620 6973 5f6e 6f72 6d61      def is_norma
-00001f90: 6c69 7a65 6428 7365 6c66 2c20 7661 6c75  lized(self, valu
-00001fa0: 653a 2062 6f6f 6c29 3a0d 0a20 2020 2020  e: bool):..     
-00001fb0: 2020 2073 656c 662e 6164 6174 612e 756e     self.adata.un
-00001fc0: 735b 2269 735f 6e6f 726d 616c 697a 6564  s["is_normalized
-00001fd0: 225d 203d 2076 616c 7565 0d0a 2020 2020  "] = value..    
-00001fe0: 2020 2020 0d0a 2020 2020 4070 726f 7065      ..    @prope
-00001ff0: 7274 790d 0a20 2020 2064 6566 2063 6e6d  rty..    def cnm
-00002000: 6673 6e73 5f76 6572 7369 6f6e 2873 656c  fsns_version(sel
-00002010: 6629 3a0d 0a20 2020 2020 2020 2022 2222  f):..        """
-00002020: 634e 4d46 2d53 4e53 2076 6572 7369 6f6e  cNMF-SNS version
-00002030: 2075 7365 6420 746f 2063 7265 6174 6520   used to create 
-00002040: 7468 6520 6461 7461 7365 740d 0a0d 0a20  the dataset.... 
-00002050: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-00002060: 7665 7273 696f 6e0d 0a20 2020 2020 2020  version..       
-00002070: 203a 7274 7970 653a 2073 7472 0d0a 2020   :rtype: str..  
-00002080: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00002090: 2020 2069 6620 2263 6e6d 6673 6e73 5f76     if "cnmfsns_v
-000020a0: 6572 7369 6f6e 2220 696e 2073 656c 662e  ersion" in self.
-000020b0: 6164 6174 612e 756e 733a 0d0a 2020 2020  adata.uns:..    
-000020c0: 2020 2020 2020 2020 7665 7273 696f 6e20          version 
-000020d0: 3d20 7365 6c66 2e61 6461 7461 2e75 6e73  = self.adata.uns
-000020e0: 5b22 636e 6d66 736e 735f 7665 7273 696f  ["cnmfsns_versio
-000020f0: 6e22 5d0d 0a20 2020 2020 2020 2065 6c73  n"]..        els
-00002100: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00002110: 7665 7273 696f 6e20 3d20 4e6f 6e65 0d0a  version = None..
-00002120: 2020 2020 2020 2020 7265 7475 726e 2076          return v
-00002130: 6572 7369 6f6e 0d0a 2020 2020 2020 2020  ersion..        
-00002140: 0d0a 2020 2020 4070 726f 7065 7274 790d  ..    @property.
-00002150: 0a20 2020 2064 6566 2068 6173 5f63 6e6d  .    def has_cnm
-00002160: 665f 7265 7375 6c74 7328 7365 6c66 293a  f_results(self):
-00002170: 0d0a 2020 2020 2020 2020 2222 2254 6573  ..        """Tes
-00002180: 7420 666f 7220 7765 6874 6865 7220 4461  t for wehther Da
-00002190: 7461 7365 7420 636f 6e74 6169 6e73 2063  taset contains c
-000021a0: 4e4d 4620 7265 7375 6c74 7320 666f 7220  NMF results for 
-000021b0: 7468 6520 6461 7461 7365 740d 0a0d 0a20  the dataset.... 
-000021c0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-000021d0: 5768 6574 6865 7220 636f 6d70 6c65 7465  Whether complete
-000021e0: 2063 4e4d 4620 7265 7375 6c74 7320 6172   cNMF results ar
-000021f0: 6520 636f 6e74 6169 6e65 6420 666f 7220  e contained for 
-00002200: 6174 206c 6561 7374 2031 2072 616e 6b20  at least 1 rank 
-00002210: 286b 290d 0a20 2020 2020 2020 203a 7274  (k)..        :rt
-00002220: 7970 653a 2062 6f6f 6c0d 0a20 2020 2020  ype: bool..     
-00002230: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00002240: 6d61 7472 6978 5f63 6865 636b 7320 3d20  matrix_checks = 
-00002250: 5b0d 0a20 2020 2020 2020 2020 2020 2022  [..            "
-00002260: 636e 6d66 5f75 7361 6765 2220 696e 2073  cnmf_usage" in s
-00002270: 656c 662e 6164 6174 612e 6f62 736d 2c0d  elf.adata.obsm,.
-00002280: 0a20 2020 2020 2020 2020 2020 2022 636e  .            "cn
-00002290: 6d66 5f67 6570 5f73 636f 7265 2220 696e  mf_gep_score" in
-000022a0: 2073 656c 662e 6164 6174 612e 7661 726d   self.adata.varm
-000022b0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-000022c0: 636e 6d66 5f67 6570 5f74 706d 2220 696e  cnmf_gep_tpm" in
-000022d0: 2073 656c 662e 6164 6174 612e 7661 726d   self.adata.varm
-000022e0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-000022f0: 636e 6d66 5f67 6570 5f72 6177 2220 696e  cnmf_gep_raw" in
-00002300: 2073 656c 662e 6164 6174 612e 7661 726d   self.adata.varm
-00002310: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00002320: 6b76 616c 7322 2069 6e20 7365 6c66 2e61  kvals" in self.a
-00002330: 6461 7461 2e75 6e73 0d0a 2020 2020 2020  data.uns..      
-00002340: 2020 5d0d 0a20 2020 2020 2020 2072 6574    ]..        ret
-00002350: 7572 6e20 616c 6c28 6d61 7472 6978 5f63  urn all(matrix_c
-00002360: 6865 636b 7329 0d0a 2020 2020 2020 2020  hecks)..        
-00002370: 0d0a 2020 2020 4070 726f 7065 7274 790d  ..    @property.
-00002380: 0a20 2020 2064 6566 206f 7665 7264 6973  .    def overdis
-00002390: 7065 7273 6564 5f67 656e 6573 2873 656c  persed_genes(sel
-000023a0: 6629 3a0d 0a20 2020 2020 2020 2022 2222  f):..        """
-000023b0: 4f76 6572 6469 7370 6572 7365 6420 6765  Overdispersed ge
-000023c0: 6e65 206c 6973 7420 7573 6564 2066 6f72  ne list used for
-000023d0: 2063 4e4d 460d 0a0d 0a20 2020 2020 2020   cNMF....       
-000023e0: 203a 7265 7475 726e 3a20 6765 6e65 206c   :return: gene l
-000023f0: 6973 740d 0a20 2020 2020 2020 203a 7274  ist..        :rt
-00002400: 7970 653a 206c 6973 740d 0a20 2020 2020  ype: list..     
-00002410: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00002420: 7265 7475 726e 2073 656c 662e 6164 6174  return self.adat
-00002430: 612e 756e 735b 2267 656e 655f 6c69 7374  a.uns["gene_list
-00002440: 225d 0d0a 0d0a 0d0a 2020 2020 4063 6e6d  "]......    @cnm
-00002450: 6673 6e73 5f76 6572 7369 6f6e 2e73 6574  fsns_version.set
-00002460: 7465 720d 0a20 2020 2064 6566 2063 6e6d  ter..    def cnm
-00002470: 6673 6e73 5f76 6572 7369 6f6e 2873 656c  fsns_version(sel
-00002480: 662c 2076 616c 7565 3a20 626f 6f6c 293a  f, value: bool):
-00002490: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-000024a0: 6461 7461 2e75 6e73 5b22 636e 6d66 736e  data.uns["cnmfsn
-000024b0: 735f 7665 7273 696f 6e22 5d20 3d20 7661  s_version"] = va
-000024c0: 6c75 650d 0a0d 0a20 2020 2020 2020 200d  lue....        .
-000024d0: 0a20 2020 2064 6566 2075 7064 6174 655f  .    def update_
-000024e0: 6f62 7328 7365 6c66 2c20 6f62 7329 3a0d  obs(self, obs):.
-000024f0: 0a20 2020 2020 2020 2022 2222 5570 6461  .        """Upda
-00002500: 7465 2074 6865 206f 6273 6572 7661 7469  te the observati
-00002510: 6f6e 206d 6574 6164 6174 6120 7769 7468  on metadata with
-00002520: 2061 206e 6577 206d 6574 6164 6174 6120   a new metadata 
-00002530: 6d61 7472 6978 0d0a 0d0a 2020 2020 2020  matrix....      
-00002540: 2020 3a70 6172 616d 206f 6273 3a20 416e    :param obs: An
-00002550: 206f 6273 6572 7661 7469 6f6e 7320 c397   observations ..
-00002560: 206d 6574 6164 6174 6120 6d61 7472 6978   metadata matrix
-00002570: 2c20 6465 6661 756c 7473 2074 6f20 4e6f  , defaults to No
-00002580: 6e65 0d0a 2020 2020 2020 2020 3a74 7970  ne..        :typ
-00002590: 6520 6f62 733a 2060 7064 2e44 6174 6146  e obs: `pd.DataF
-000025a0: 7261 6d65 602c 206f 7074 696f 6e61 6c0d  rame`, optional.
-000025b0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-000025c0: 2020 2020 2020 2320 636f 6e76 6572 7420        # convert 
-000025d0: 276f 626a 6563 7427 2064 7479 7065 2074  'object' dtype t
-000025e0: 6f20 6361 7465 676f 7269 6361 6c2c 2063  o categorical, c
-000025f0: 6f6e 7665 7274 696e 6720 626f 6f6c 2076  onverting bool v
-00002600: 616c 7565 7320 746f 2073 7472 696e 6773  alues to strings
-00002610: 2061 7320 7468 6573 6520 6172 6520 6e6f   as these are no
-00002620: 7420 7375 7070 6f72 7465 6420 6279 2041  t supported by A
-00002630: 6e6e 4461 7461 206f 6e2d 6469 736b 2066  nnData on-disk f
-00002640: 6f72 6d61 740d 0a20 2020 2020 2020 2066  ormat..        f
-00002650: 6f72 2063 6f6c 2069 6e20 6f62 732e 7365  or col in obs.se
-00002660: 6c65 6374 5f64 7479 7065 7328 696e 636c  lect_dtypes(incl
-00002670: 7564 653d 226f 626a 6563 7422 292e 636f  ude="object").co
-00002680: 6c75 6d6e 733a 0d0a 2020 2020 2020 2020  lumns:..        
-00002690: 2020 2020 6f62 735b 636f 6c5d 203d 206f      obs[col] = o
-000026a0: 6273 5b63 6f6c 5d2e 7265 706c 6163 6528  bs[col].replace(
-000026b0: 7b54 7275 653a 2022 5472 7565 222c 2046  {True: "True", F
-000026c0: 616c 7365 3a20 2246 616c 7365 227d 292e  alse: "False"}).
-000026d0: 6173 7479 7065 2822 6361 7465 676f 7279  astype("category
-000026e0: 2229 0d0a 2020 2020 2020 2020 6d69 7373  ")..        miss
-000026f0: 696e 675f 7361 6d70 6c65 735f 696e 5f58  ing_samples_in_X
-00002700: 203d 206f 6273 2e69 6e64 6578 2e64 6966   = obs.index.dif
-00002710: 6665 7265 6e63 6528 7365 6c66 2e61 6461  ference(self.ada
-00002720: 7461 2e6f 6273 2e69 6e64 6578 292e 6173  ta.obs.index).as
-00002730: 7479 7065 2873 7472 292e 746f 5f6c 6973  type(str).to_lis
-00002740: 7428 290d 0a20 2020 2020 2020 2069 6620  t()..        if 
-00002750: 6d69 7373 696e 675f 7361 6d70 6c65 735f  missing_samples_
-00002760: 696e 5f58 3a0d 0a20 2020 2020 2020 2020  in_X:..         
-00002770: 2020 206c 6f67 6769 6e67 2e77 6172 6e69     logging.warni
-00002780: 6e67 2822 5468 6520 666f 6c6c 6f77 696e  ng("The followin
-00002790: 6720 7361 6d70 6c65 7320 696e 2074 6865  g samples in the
-000027a0: 206d 6574 6164 6174 6120 7765 7265 206e   metadata were n
-000027b0: 6f74 2070 7265 7365 6e74 2069 6e20 7468  ot present in th
-000027c0: 6520 6461 7461 2028 6061 6461 7461 2e58  e data (`adata.X
-000027d0: 6029 3a5c 6e20 202d 2022 202b 2022 5c6e  `):\n  - " + "\n
-000027e0: 2020 2d20 222e 6a6f 696e 286d 6973 7369    - ".join(missi
-000027f0: 6e67 5f73 616d 706c 6573 5f69 6e5f 5829  ng_samples_in_X)
-00002800: 290d 0a20 2020 2020 2020 206d 6973 7369  )..        missi
-00002810: 6e67 5f73 616d 706c 6573 5f69 6e5f 6d64  ng_samples_in_md
-00002820: 203d 2073 656c 662e 6164 6174 612e 6f62   = self.adata.ob
-00002830: 732e 696e 6465 782e 6469 6666 6572 656e  s.index.differen
-00002840: 6365 286f 6273 2e69 6e64 6578 292e 6173  ce(obs.index).as
-00002850: 7479 7065 2873 7472 292e 746f 5f6c 6973  type(str).to_lis
-00002860: 7428 290d 0a20 2020 2020 2020 2069 6620  t()..        if 
-00002870: 6d69 7373 696e 675f 7361 6d70 6c65 735f  missing_samples_
-00002880: 696e 5f6d 643a 0d0a 2020 2020 2020 2020  in_md:..        
-00002890: 2020 2020 6c6f 6767 696e 672e 7761 726e      logging.warn
-000028a0: 696e 6728 2254 6865 2066 6f6c 6c6f 7769  ing("The followi
-000028b0: 6e67 2073 616d 706c 6573 2069 6e20 7468  ng samples in th
-000028c0: 6520 6461 7461 2028 6061 6461 7461 2e58  e data (`adata.X
-000028d0: 6029 2077 6572 6520 6162 7365 6e74 2069  `) were absent i
-000028e0: 6e20 7468 6520 6d65 7461 6461 7461 3a5c  n the metadata:\
-000028f0: 6e20 202d 2022 202b 2022 5c6e 2020 2d20  n  - " + "\n  - 
-00002900: 222e 6a6f 696e 286d 6973 7369 6e67 5f73  ".join(missing_s
-00002910: 616d 706c 6573 5f69 6e5f 6d64 2929 0d0a  amples_in_md))..
-00002920: 2020 2020 2020 2020 7365 6c66 2e61 6461          self.ada
-00002930: 7461 2e6f 6273 203d 206f 6273 2e72 6569  ta.obs = obs.rei
-00002940: 6e64 6578 2873 656c 662e 6164 6174 612e  ndex(self.adata.
-00002950: 6f62 732e 696e 6465 7829 0d0a 2020 2020  obs.index)..    
-00002960: 0d0a 2020 2020 6465 6620 6765 745f 6d65  ..    def get_me
-00002970: 7461 6461 7461 5f74 7970 655f 7375 6d6d  tadata_type_summ
-00002980: 6172 7928 7365 6c66 293a 0d0a 2020 2020  ary(self):..    
-00002990: 2020 2020 2222 2252 6574 7572 6e20 6120      """Return a 
-000029a0: 7072 696e 7461 626c 6520 7375 6d6d 6172  printable summar
-000029b0: 7920 6f66 206d 6574 6164 6174 6120 616e  y of metadata an
-000029c0: 6420 7661 6c75 6520 7479 7065 7320 666f  d value types fo
-000029d0: 7220 6561 6368 206d 6574 6164 6174 6120  r each metadata 
-000029e0: 6c61 7965 722e 0d0a 0d0a 2020 2020 2020  layer.....      
-000029f0: 2020 3a72 6574 7572 6e3a 2053 756d 6d61    :return: Summa
-00002a00: 7279 206f 6620 6d65 7461 6461 7461 0d0a  ry of metadata..
-00002a10: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00002a20: 7374 720d 0a20 2020 2020 2020 2022 2222  str..        """
-00002a30: 0d0a 2020 2020 2020 2020 6d73 6720 3d20  ..        msg = 
-00002a40: 2222 0d0a 2020 2020 2020 2020 666f 7220  ""..        for 
-00002a50: 636f 6c20 696e 2073 656c 662e 6164 6174  col in self.adat
-00002a60: 612e 6f62 732e 636f 6c75 6d6e 733a 0d0a  a.obs.columns:..
-00002a70: 2020 2020 2020 2020 2020 2020 6d73 6720              msg 
-00002a80: 2b3d 2022 2020 2020 436f 6c75 6d6e 3a20  += "    Column: 
-00002a90: 2220 2b20 636f 6c20 2b20 225c 6e22 0d0a  " + col + "\n"..
-00002aa0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00002ab0: 7661 6c75 655f 7479 7065 2c20 636f 756e  value_type, coun
-00002ac0: 7420 696e 2073 656c 662e 6164 6174 612e  t in self.adata.
-00002ad0: 6f62 735b 636f 6c5d 2e64 726f 706e 6128  obs[col].dropna(
-00002ae0: 292e 6d61 7028 7479 7065 292e 7661 6c75  ).map(type).valu
-00002af0: 655f 636f 756e 7473 2829 2e69 7465 6d73  e_counts().items
-00002b00: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-00002b10: 2020 2020 206d 7367 202b 3d20 6622 2020       msg += f"  
-00002b20: 2020 2020 2020 7b76 616c 7565 5f74 7970        {value_typ
-00002b30: 657d 3a20 7b63 6f75 6e74 7d5c 6e22 0d0a  e}: {count}\n"..
-00002b40: 2020 2020 2020 2020 7265 7475 726e 206d          return m
-00002b50: 7367 0d0a 2020 2020 0d0a 2020 2020 6465  sg..    ..    de
-00002b60: 6620 7772 6974 655f 6835 6164 2873 656c  f write_h5ad(sel
-00002b70: 662c 2066 696c 656e 616d 6529 3a0d 0a20  f, filename):.. 
-00002b80: 2020 2020 2020 2022 2222 5772 6974 6520         """Write 
-00002b90: 6461 7461 7365 7420 746f 202e 6835 6164  dataset to .h5ad
-00002ba0: 2066 696c 652e 0d0a 0d0a 2020 2020 2020   file.....      
-00002bb0: 2020 3a70 6172 616d 2066 696c 656e 616d    :param filenam
-00002bc0: 653a 2066 696c 6570 6174 680d 0a20 2020  e: filepath..   
-00002bd0: 2020 2020 203a 7479 7065 2066 696c 656e       :type filen
-00002be0: 616d 653a 2073 7472 0d0a 2020 2020 2020  ame: str..      
-00002bf0: 2020 2222 220d 0a20 2020 2020 2020 2066    """..        f
-00002c00: 696c 656e 616d 6520 3d20 6f73 2e70 6174  ilename = os.pat
-00002c10: 682e 6162 7370 6174 6828 6669 6c65 6e61  h.abspath(filena
-00002c20: 6d65 290d 0a20 2020 2020 2020 206c 6f67  me)..        log
-00002c30: 6769 6e67 2e69 6e66 6f28 6622 5772 6974  ging.info(f"Writ
-00002c40: 696e 6720 746f 207b 6669 6c65 6e61 6d65  ing to {filename
-00002c50: 7d22 290d 0a20 2020 2020 2020 2073 656c  }")..        sel
-00002c60: 662e 6164 6174 612e 7772 6974 655f 6835  f.adata.write_h5
-00002c70: 6164 2866 696c 656e 616d 6529 0d0a 2020  ad(filename)..  
-00002c80: 2020 2020 2020 6c6f 6767 696e 672e 696e        logging.in
-00002c90: 666f 2866 2244 6f6e 6522 290d 0a20 2020  fo(f"Done")..   
-00002ca0: 200d 0a20 2020 2064 6566 2074 6f5f 6466   ..    def to_df
-00002cb0: 2873 656c 662c 206e 6f72 6d61 6c69 7a65  (self, normalize
-00002cc0: 643d 4661 6c73 6529 3a0d 0a20 2020 2020  d=False):..     
-00002cd0: 2020 2022 2222 4765 7420 6461 7461 206d     """Get data m
-00002ce0: 6174 7269 7820 6173 2061 2060 7064 2e44  atrix as a `pd.D
-00002cf0: 6174 6146 7261 6d65 600d 0a0d 0a20 2020  ataFrame`....   
-00002d00: 2020 2020 203a 7061 7261 6d20 6e6f 726d       :param norm
-00002d10: 616c 697a 6564 3a20 5365 7420 7472 7565  alized: Set true
-00002d20: 2066 6f72 2054 504d 206e 6f72 6d61 6c69   for TPM normali
-00002d30: 7a65 6420 6f75 7470 7574 2c20 6465 6661  zed output, defa
-00002d40: 756c 7473 2074 6f20 4661 6c73 650d 0a20  ults to False.. 
-00002d50: 2020 2020 2020 203a 7479 7065 206e 6f72         :type nor
-00002d60: 6d61 6c69 7a65 643a 2062 6f6f 6c2c 206f  malized: bool, o
-00002d70: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
-00002d80: 203a 7265 7475 726e 3a20 6f62 7365 7276   :return: observ
-00002d90: 6174 696f 6e73 20c3 9720 7661 7269 6162  ations .. variab
-00002da0: 6c65 7320 6461 7461 206d 6174 7269 780d  les data matrix.
-00002db0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00002dc0: 2070 642e 4461 7461 4672 616d 650d 0a20   pd.DataFrame.. 
-00002dd0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00002de0: 2020 2020 6466 203d 2073 656c 662e 6164      df = self.ad
-00002df0: 6174 612e 746f 5f64 6628 290d 0a20 2020  ata.to_df()..   
-00002e00: 2020 2020 2069 6620 6e6f 726d 616c 697a       if normaliz
-00002e10: 6564 2061 6e64 206e 6f74 2073 656c 662e  ed and not self.
-00002e20: 6973 5f6e 6f72 6d61 6c69 7a65 643a 0d0a  is_normalized:..
-00002e30: 2020 2020 2020 2020 2020 2020 6466 203d              df =
-00002e40: 2064 662e 6469 7628 6466 2e73 756d 2861   df.div(df.sum(a
-00002e50: 7869 733d 3129 2c20 6178 6973 3d30 2920  xis=1), axis=0) 
-00002e60: 2a20 3165 3620 2023 2054 504d 206e 6f72  * 1e6  # TPM nor
-00002e70: 6d61 6c69 7a61 7469 6f6e 0d0a 2020 2020  malization..    
-00002e80: 2020 2020 7265 7475 726e 2064 660d 0a20      return df.. 
-00002e90: 2020 2020 2020 200d 0a20 2020 2064 6566         ..    def
-00002ea0: 2072 656d 6f76 655f 756e 6661 6374 6f72   remove_unfactor
-00002eb0: 697a 6162 6c65 5f67 656e 6573 2873 656c  izable_genes(sel
-00002ec0: 6629 3a0d 0a20 2020 2020 2020 2022 2222  f):..        """
-00002ed0: 5265 6d6f 7665 7320 6765 6e65 7320 7769  Removes genes wi
-00002ee0: 7468 206d 6973 7369 6e67 2076 616c 7565  th missing value
-00002ef0: 7320 6f72 207a 6572 6f20 7661 7269 616e  s or zero varian
-00002f00: 6365 2066 726f 6d20 7468 6520 6461 7461  ce from the data
-00002f10: 206d 6174 7269 782e 0d0a 2020 2020 2020   matrix...      
-00002f20: 2020 2222 220d 0a20 2020 2020 2020 2064    """..        d
-00002f30: 6620 3d20 7365 6c66 2e74 6f5f 6466 286e  f = self.to_df(n
-00002f40: 6f72 6d61 6c69 7a65 643d 4661 6c73 6529  ormalized=False)
-00002f50: 0d0a 2020 2020 2020 2020 2320 4368 6563  ..        # Chec
-00002f60: 6b20 666f 7220 7661 7269 6162 6c65 7320  k for variables 
-00002f70: 7769 7468 206d 6973 7369 6e67 2076 616c  with missing val
-00002f80: 7565 730d 0a20 2020 2020 2020 2067 656e  ues..        gen
-00002f90: 6573 5f77 6974 685f 6d69 7373 696e 6776  es_with_missingv
-00002fa0: 616c 7565 7320 3d20 6466 2e69 736e 756c  alues = df.isnul
-00002fb0: 6c28 292e 616e 7928 290d 0a20 2020 2020  l().any()..     
-00002fc0: 2020 200d 0a20 2020 2020 2020 2069 6620     ..        if 
-00002fd0: 6765 6e65 735f 7769 7468 5f6d 6973 7369  genes_with_missi
-00002fe0: 6e67 7661 6c75 6573 2e61 6e79 2829 3a0d  ngvalues.any():.
-00002ff0: 0a20 2020 2020 2020 2020 2020 206e 5f6d  .            n_m
-00003000: 6973 7369 6e67 203d 2067 656e 6573 5f77  issing = genes_w
-00003010: 6974 685f 6d69 7373 696e 6776 616c 7565  ith_missingvalue
-00003020: 732e 7375 6d28 290d 0a20 2020 2020 2020  s.sum()..       
-00003030: 2020 2020 206c 6f67 6769 6e67 2e77 6172       logging.war
-00003040: 6e69 6e67 2866 227b 6e5f 6d69 7373 696e  ning(f"{n_missin
-00003050: 677d 206f 6620 7b73 656c 662e 6164 6174  g} of {self.adat
-00003060: 612e 6e5f 7661 7273 7d20 7661 7269 6162  a.n_vars} variab
-00003070: 6c65 7320 6172 6520 6d69 7373 696e 6720  les are missing 
-00003080: 7661 6c75 6573 2028 6061 6461 7461 2e58  values (`adata.X
-00003090: 6029 2e22 290d 0a20 2020 2020 2020 2020  `).")..         
-000030a0: 2020 206c 6f67 6769 6e67 2e77 6172 6e69     logging.warni
-000030b0: 6e67 2866 2253 7562 7365 7474 696e 6720  ng(f"Subsetting 
-000030c0: 7661 7269 6162 6c65 7320 746f 2074 686f  variables to tho
-000030d0: 7365 2077 6974 6820 6e6f 206d 6973 7369  se with no missi
-000030e0: 6e67 2076 616c 7565 732e 2229 0d0a 2020  ng values.")..  
-000030f0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00003100: 2020 2020 2020 2020 2320 4368 6563 6b20          # Check 
-00003110: 666f 7220 6765 6e65 7320 7769 7468 207a  for genes with z
-00003120: 6572 6f20 7661 7269 616e 6365 0d0a 2020  ero variance..  
-00003130: 2020 2020 2020 7a65 726f 7661 7267 656e        zerovargen
-00003140: 6573 203d 2028 6466 2e76 6172 2829 203d  es = (df.var() =
-00003150: 3d20 3029 0d0a 2020 2020 2020 2020 6966  = 0)..        if
-00003160: 207a 6572 6f76 6172 6765 6e65 732e 616e   zerovargenes.an
-00003170: 7928 293a 0d0a 2020 2020 2020 2020 2020  y():..          
-00003180: 2020 6e5f 7a65 726f 7661 7220 3d20 7a65    n_zerovar = ze
-00003190: 726f 7661 7267 656e 6573 2e73 756d 2829  rovargenes.sum()
-000031a0: 0d0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
-000031b0: 6767 696e 672e 7761 726e 696e 6728 6622  gging.warning(f"
-000031c0: 7b6e 5f7a 6572 6f76 6172 7d20 6f66 207b  {n_zerovar} of {
-000031d0: 7365 6c66 2e61 6461 7461 2e6e 5f76 6172  self.adata.n_var
-000031e0: 737d 2076 6172 6961 626c 6573 2068 6176  s} variables hav
-000031f0: 6520 6120 7661 7269 616e 6365 206f 6620  e a variance of 
-00003200: 7a65 726f 2069 6e20 636f 756e 7473 2064  zero in counts d
-00003210: 6174 6120 2860 6164 6174 612e 7261 772e  ata (`adata.raw.
-00003220: 5860 292e 2229 0d0a 2020 2020 2020 2020  X`).")..        
-00003230: 2020 2020 6c6f 6767 696e 672e 7761 726e      logging.warn
-00003240: 696e 6728 6622 5375 6273 6574 7469 6e67  ing(f"Subsetting
-00003250: 2076 6172 6961 626c 6573 2074 6f20 7468   variables to th
-00003260: 6f73 6520 7769 7468 206e 6f6e 7a65 726f  ose with nonzero
-00003270: 2076 6172 6961 6e63 652e 2229 0d0a 2020   variance.")..  
-00003280: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00003290: 6765 6e65 735f 746f 5f6b 6565 7020 3d20  genes_to_keep = 
-000032a0: 287e 6765 6e65 735f 7769 7468 5f6d 6973  (~genes_with_mis
-000032b0: 7369 6e67 7661 6c75 6573 2920 2620 287e  singvalues) & (~
-000032c0: 7a65 726f 7661 7267 656e 6573 290d 0a20  zerovargenes).. 
-000032d0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000032e0: 2073 656c 662e 6164 6174 6120 3d20 7365   self.adata = se
-000032f0: 6c66 2e61 6461 7461 5b3a 2c67 656e 6573  lf.adata[:,genes
-00003300: 5f74 6f5f 6b65 6570 5d0d 0a0d 0a20 2020  _to_keep]....   
-00003310: 2064 6566 2063 6f6d 7075 7465 5f67 656e   def compute_gen
-00003320: 655f 7374 6174 7328 7365 6c66 2c20 6f64  e_stats(self, od
-00003330: 675f 6465 6661 756c 745f 7370 6c69 6e65  g_default_spline
-00003340: 5f64 6567 7265 653a 2069 6e74 203d 2033  _degree: int = 3
-00003350: 2c20 6f64 675f 6465 6661 756c 745f 646f  , odg_default_do
-00003360: 663a 2069 6e74 203d 2038 293a 0d0a 2020  f: int = 8):..  
-00003370: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00003380: 2020 2043 6f6d 7075 7465 7320 6765 6e65     Computes gene
-00003390: 2073 7461 7469 7374 6963 7320 616e 6420   statistics and 
-000033a0: 6669 7473 2074 776f 206d 6f64 656c 7320  fits two models 
-000033b0: 6f66 206d 6561 6e20 616e 6420 7661 7269  of mean and vari
-000033c0: 616e 6365 206f 6620 6765 6e65 7320 696e  ance of genes in
-000033d0: 2074 6865 2064 6174 6173 6574 2e20 5468   the dataset. Th
-000033e0: 6520 6669 7273 7420 6d65 7468 6f64 2069  e first method i
-000033f0: 7320 7468 650d 0a20 2020 2020 2020 2067  s the..        g
-00003400: 656e 6572 616c 697a 6564 2061 6464 6974  eneralized addit
-00003410: 6976 6520 6d6f 6465 6c20 7769 7468 2073  ive model with s
-00003420: 6d6f 6f74 6820 636f 6d70 6f6e 656e 7473  mooth components
-00003430: 2028 422d 7370 6c69 6e65 7329 2074 6f20   (B-splines) to 
-00003440: 6d6f 6465 6c20 7468 6520 7265 6c61 7469  model the relati
-00003450: 6f6e 7368 6970 206f 6620 6d65 616e 2061  onship of mean a
-00003460: 6e64 2076 6172 6961 6e63 650d 0a20 2020  nd variance..   
-00003470: 2020 2020 2062 6574 7765 656e 2067 656e       between gen
-00003480: 6573 2069 6e20 7468 6520 6461 7461 7365  es in the datase
-00003490: 742e 2049 7420 7072 6f64 7563 6573 2061  t. It produces a
-000034a0: 6e20 6f64 7363 6f72 6520 6d65 7472 6963  n odscore metric
-000034b0: 2066 6f72 206f 7665 7264 6973 7065 7273   for overdispers
-000034c0: 696f 6e2e 2054 6865 2073 6563 6f6e 6420  ion. The second 
-000034d0: 6973 2074 6865 2063 6f75 6e74 2d73 7461  is the count-sta
-000034e0: 7469 7374 6963 730d 0a20 2020 2020 2020  tistics..       
-000034f0: 206d 6574 686f 6420 666f 756e 6420 696e   method found in
-00003500: 2074 6865 2063 4e4d 4620 7061 636b 6167   the cNMF packag
-00003510: 652c 2077 6869 6368 2070 726f 6475 6365  e, which produce
-00003520: 7320 6120 6d6f 6469 6669 6564 2076 2d73  s a modified v-s
-00003530: 636f 7265 206d 6574 7269 632e 2041 6c6c  core metric. All
-00003540: 2067 656e 6520 7374 6174 6973 7469 6373   gene statistics
-00003550: 2061 7265 2073 746f 7265 6420 7769 7468   are stored with
-00003560: 696e 2074 6865 0d0a 2020 2020 2020 2020  in the..        
-00003570: 6461 7461 7365 7420 6f62 6a65 6374 2061  dataset object a
-00003580: 6e64 2061 7265 2061 6363 6573 7369 626c  nd are accessibl
-00003590: 6520 7573 696e 6720 6064 6174 6173 6574  e using `dataset
-000035a0: 2e61 6e6e 6461 7461 2e76 6172 602e 0d0a  .anndata.var`...
-000035b0: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-000035c0: 206f 6467 5f64 6566 6175 6c74 5f73 706c   odg_default_spl
-000035d0: 696e 655f 6465 6772 6565 3a20 422d 5370  ine_degree: B-Sp
-000035e0: 6c69 6e65 2064 6567 7265 6520 666f 7220  line degree for 
-000035f0: 474c 4d2d 4741 4d20 6d6f 6465 6c6c 696e  GLM-GAM modellin
-00003600: 6720 6f66 206d 6561 6e2d 7661 7269 616e  g of mean-varian
-00003610: 6365 2072 656c 6174 696f 6e73 6869 702c  ce relationship,
-00003620: 2064 6566 6175 6c74 7320 746f 2033 0d0a   defaults to 3..
-00003630: 2020 2020 2020 2020 3a74 7970 6520 6f64          :type od
-00003640: 675f 6465 6661 756c 745f 7370 6c69 6e65  g_default_spline
-00003650: 5f64 6567 7265 653a 2069 6e74 2c20 6f70  _degree: int, op
-00003660: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
-00003670: 3a70 6172 616d 206f 6467 5f64 6566 6175  :param odg_defau
-00003680: 6c74 5f64 6f66 3a20 4465 6772 6565 7320  lt_dof: Degrees 
-00003690: 6f66 2066 7265 6564 6f6d 2066 6f72 2047  of freedom for G
-000036a0: 4c4d 2d47 414d 206d 6f64 656c 6c69 6e67  LM-GAM modelling
-000036b0: 206f 6620 6d65 616e 2d76 6172 616e 6365   of mean-varance
-000036c0: 2c20 6465 6661 756c 7473 2074 6f20 380d  , defaults to 8.
-000036d0: 0a20 2020 2020 2020 203a 7479 7065 206f  .        :type o
-000036e0: 6467 5f64 6566 6175 6c74 5f64 6f66 3a20  dg_default_dof: 
-000036f0: 696e 742c 206f 7074 696f 6e61 6c0d 0a20  int, optional.. 
-00003700: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00003710: 2020 2020 6461 7461 5f72 6177 203d 2073      data_raw = s
-00003720: 656c 662e 746f 5f64 6628 290d 0a20 2020  elf.to_df()..   
-00003730: 2020 2020 2064 6174 615f 6e6f 726d 616c       data_normal
-00003740: 697a 6564 203d 2073 656c 662e 746f 5f64  ized = self.to_d
-00003750: 6628 6e6f 726d 616c 697a 6564 3d54 7275  f(normalized=Tru
-00003760: 6529 0d0a 2020 2020 2020 2020 0d0a 2020  e)..        ..  
-00003770: 2020 2020 2020 2320 6372 6561 7465 2064        # create d
-00003780: 6174 6166 7261 6d65 206f 6620 7065 722d  ataframe of per-
-00003790: 6765 6e65 2073 7461 7469 7374 6963 730d  gene statistics.
-000037a0: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
-000037b0: 6174 612e 7661 725b 226d 6561 6e22 5d20  ata.var["mean"] 
-000037c0: 3d20 6461 7461 5f6e 6f72 6d61 6c69 7a65  = data_normalize
-000037d0: 642e 6d65 616e 2829 0d0a 2020 2020 2020  d.mean()..      
-000037e0: 2020 7365 6c66 2e61 6461 7461 2e76 6172    self.adata.var
-000037f0: 5b22 7261 6e6b 5f6d 6561 6e22 5d20 3d20  ["rank_mean"] = 
-00003800: 7365 6c66 2e61 6461 7461 2e76 6172 5b22  self.adata.var["
-00003810: 6d65 616e 225d 2e72 616e 6b28 290d 0a20  mean"].rank().. 
-00003820: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
-00003830: 612e 7661 725b 2276 6172 6961 6e63 6522  a.var["variance"
-00003840: 5d20 3d20 6461 7461 5f6e 6f72 6d61 6c69  ] = data_normali
-00003850: 7a65 642e 7661 7228 290d 0a20 2020 2020  zed.var()..     
-00003860: 2020 2073 656c 662e 6164 6174 612e 7661     self.adata.va
-00003870: 725b 2273 6422 5d20 3d20 6461 7461 5f6e  r["sd"] = data_n
-00003880: 6f72 6d61 6c69 7a65 642e 7374 6428 290d  ormalized.std().
-00003890: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
-000038a0: 6174 612e 7661 725b 226d 6973 7369 6e67  ata.var["missing
-000038b0: 6e65 7373 225d 203d 2064 6174 615f 6e6f  ness"] = data_no
-000038c0: 726d 616c 697a 6564 2e69 736e 756c 6c28  rmalized.isnull(
-000038d0: 292e 7375 6d28 2920 2f20 6461 7461 5f6e  ).sum() / data_n
-000038e0: 6f72 6d61 6c69 7a65 642e 7368 6170 655b  ormalized.shape[
-000038f0: 305d 0d0a 2020 2020 2020 2020 7365 6c66  0]..        self
-00003900: 2e61 6461 7461 2e76 6172 5b5b 226c 6f67  .adata.var[["log
-00003910: 5f6d 6561 6e22 2c20 226c 6f67 5f76 6172  _mean", "log_var
-00003920: 6961 6e63 6522 5d5d 203d 206e 702e 6c6f  iance"]] = np.lo
-00003930: 6731 3028 7365 6c66 2e61 6461 7461 2e76  g10(self.adata.v
-00003940: 6172 5b5b 226d 6561 6e22 2c20 2276 6172  ar[["mean", "var
-00003950: 6961 6e63 6522 5d5d 290d 0a20 2020 2020  iance"]])..     
-00003960: 2020 2073 656c 662e 6164 6174 612e 7661     self.adata.va
-00003970: 725b 226d 6561 6e5f 636f 756e 7473 225d  r["mean_counts"]
-00003980: 203d 2064 6174 615f 7261 772e 6d65 616e   = data_raw.mean
-00003990: 2829 0d0a 2020 2020 2020 2020 7365 6c66  ()..        self
-000039a0: 2e61 6461 7461 2e76 6172 5b22 6f64 7363  .adata.var["odsc
-000039b0: 6f72 655f 6578 636c 7564 6564 225d 203d  ore_excluded"] =
-000039c0: 2028 2873 656c 662e 6164 6174 612e 7661   ((self.adata.va
-000039d0: 725b 226d 6973 7369 6e67 6e65 7373 225d  r["missingness"]
-000039e0: 203e 2030 2920 7c0d 0a20 2020 2020 2020   > 0) |..       
-000039f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a10: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
-00003a20: 612e 7661 725b 226c 6f67 5f6d 6561 6e22  a.var["log_mean"
-00003a30: 5d2e 6973 6e75 6c6c 2829 207c 0d0a 2020  ].isnull() |..  
-00003a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a60: 2020 2020 2020 2020 2020 2020 2873 656c              (sel
-00003a70: 662e 6164 6174 612e 7661 725b 226d 6561  f.adata.var["mea
-00003a80: 6e22 5d20 3d3d 2030 2920 7c0d 0a20 2020  n"] == 0) |..   
-00003a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ab0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003ac0: 6164 6174 612e 7661 725b 226c 6f67 5f76  adata.var["log_v
-00003ad0: 6172 6961 6e63 6522 5d2e 6973 6e75 6c6c  ariance"].isnull
-00003ae0: 2829 290d 0a0d 0a20 2020 2020 2020 2023  ())....        #
-00003af0: 206d 6f64 656c 206d 6561 6e2d 7661 7269   model mean-vari
-00003b00: 616e 6365 2072 656c 6174 696f 6e73 6869  ance relationshi
-00003b10: 7020 7573 696e 6720 6765 6e65 7261 6c69  p using generali
-00003b20: 7a65 6420 6164 6469 7469 7665 206d 6f64  zed additive mod
-00003b30: 656c 2077 6974 6820 736d 6f6f 7468 2063  el with smooth c
-00003b40: 6f6d 706f 6e65 6e74 730d 0a20 2020 2020  omponents..     
-00003b50: 2020 2064 665f 6d6f 6465 6c20 3d20 7365     df_model = se
-00003b60: 6c66 2e61 6461 7461 2e76 6172 5b7e 7365  lf.adata.var[~se
-00003b70: 6c66 2e61 6461 7461 2e76 6172 5b22 6f64  lf.adata.var["od
-00003b80: 7363 6f72 655f 6578 636c 7564 6564 225d  score_excluded"]
-00003b90: 5d0d 0a20 2020 2020 2020 2062 7320 3d20  ]..        bs = 
-00003ba0: 4253 706c 696e 6573 2864 665f 6d6f 6465  BSplines(df_mode
-00003bb0: 6c5b 226d 6561 6e22 5d2c 2064 663d 6f64  l["mean"], df=od
-00003bc0: 675f 6465 6661 756c 745f 646f 662c 2064  g_default_dof, d
-00003bd0: 6567 7265 653d 6f64 675f 6465 6661 756c  egree=odg_defaul
-00003be0: 745f 7370 6c69 6e65 5f64 6567 7265 6529  t_spline_degree)
-00003bf0: 0d0a 2020 2020 2020 2020 6761 6d20 3d20  ..        gam = 
-00003c00: 474c 4d47 616d 2e66 726f 6d5f 666f 726d  GLMGam.from_form
-00003c10: 756c 6128 226c 6f67 5f76 6172 6961 6e63  ula("log_varianc
-00003c20: 6520 7e20 6c6f 675f 6d65 616e 222c 2064  e ~ log_mean", d
-00003c30: 6174 613d 6466 5f6d 6f64 656c 2c20 736d  ata=df_model, sm
-00003c40: 6f6f 7468 6572 3d62 7329 2e66 6974 2829  oother=bs).fit()
-00003c50: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-00003c60: 6461 7461 2e76 6172 5b22 7265 7369 645f  data.var["resid_
-00003c70: 6c6f 675f 7661 7269 616e 6365 225d 203d  log_variance"] =
-00003c80: 2067 616d 2e72 6573 6964 5f72 6573 706f   gam.resid_respo
-00003c90: 6e73 650d 0a20 2020 2020 2020 2073 656c  nse..        sel
-00003ca0: 662e 6164 6174 612e 7661 725b 226f 6473  f.adata.var["ods
-00003cb0: 636f 7265 225d 203d 206e 702e 7371 7274  core"] = np.sqrt
-00003cc0: 2831 3020 2a2a 2073 656c 662e 6164 6174  (10 ** self.adat
-00003cd0: 612e 7661 725b 2272 6573 6964 5f6c 6f67  a.var["resid_log
-00003ce0: 5f76 6172 6961 6e63 6522 5d29 0d0a 2020  _variance"])..  
-00003cf0: 2020 2020 2020 7365 6c66 2e61 6461 7461        self.adata
-00003d00: 2e76 6172 5b22 6761 6d5f 6669 7474 6564  .var["gam_fitted
-00003d10: 7661 6c75 6573 225d 203d 2067 616d 2e66  values"] = gam.f
-00003d20: 6974 7465 6476 616c 7565 730d 0a0d 0a0d  ittedvalues.....
-00003d30: 0a20 2020 2020 2020 2023 206d 6f64 656c  .        # model
-00003d40: 206d 6561 6e2d 7661 7269 616e 6365 2072   mean-variance r
-00003d50: 656c 6174 696f 6e73 6869 7020 7573 696e  elationship usin
-00003d60: 6720 634e 4d46 2773 206d 6574 686f 6420  g cNMF's method 
-00003d70: 6261 7365 6420 6f6e 2076 2d73 636f 7265  based on v-score
-00003d80: 2061 6e64 206d 696e 696d 756d 2065 7870   and minimum exp
-00003d90: 7265 7373 696f 6e20 7468 7265 7368 6f6c  ression threshol
-00003da0: 640d 0a20 2020 2020 2020 2076 7363 6f72  d..        vscor
-00003db0: 655f 7374 6174 7320 3d20 7064 2e44 6174  e_stats = pd.Dat
-00003dc0: 6146 7261 6d65 2863 6e6d 662e 6765 745f  aFrame(cnmf.get_
-00003dd0: 6869 6768 7661 725f 6765 6e65 7328 696e  highvar_genes(in
-00003de0: 7075 745f 636f 756e 7473 3d64 6174 615f  put_counts=data_
-00003df0: 6e6f 726d 616c 697a 6564 2e76 616c 7565  normalized.value
-00003e00: 732c 206d 696e 696d 616c 5f6d 6561 6e3d  s, minimal_mean=
-00003e10: 3029 5b30 5d29 0d0a 2020 2020 2020 2020  0)[0])..        
-00003e20: 7673 636f 7265 5f73 7461 7473 2e69 6e64  vscore_stats.ind
-00003e30: 6578 203d 2064 6174 615f 6e6f 726d 616c  ex = data_normal
-00003e40: 697a 6564 2e63 6f6c 756d 6e73 0d0a 2020  ized.columns..  
-00003e50: 2020 2020 2020 7365 6c66 2e61 6461 7461        self.adata
-00003e60: 2e76 6172 5b22 7673 636f 7265 225d 203d  .var["vscore"] =
-00003e70: 2076 7363 6f72 655f 7374 6174 735b 2266   vscore_stats["f
-00003e80: 616e 6f5f 7261 7469 6f22 5d0d 0a20 2020  ano_ratio"]..   
-00003e90: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
-00003ea0: 756e 735b 226f 6467 225d 5b22 6f64 675f  uns["odg"]["odg_
-00003eb0: 6465 6661 756c 745f 7370 6c69 6e65 5f64  default_spline_d
-00003ec0: 6567 7265 6522 5d20 3d20 6f64 675f 6465  egree"] = odg_de
-00003ed0: 6661 756c 745f 7370 6c69 6e65 5f64 6567  fault_spline_deg
-00003ee0: 7265 650d 0a20 2020 2020 2020 2073 656c  ree..        sel
-00003ef0: 662e 6164 6174 612e 756e 735b 226f 6467  f.adata.uns["odg
-00003f00: 225d 5b22 6f64 675f 6465 6661 756c 745f  "]["odg_default_
-00003f10: 646f 6622 5d20 3d20 6f64 675f 6465 6661  dof"] = odg_defa
-00003f20: 756c 745f 646f 660d 0a20 2020 2020 2020  ult_dof..       
-00003f30: 2073 656c 662e 6170 7065 6e64 5f74 6f5f   self.append_to_
-00003f40: 6869 7374 6f72 7928 2247 656e 652d 6c65  history("Gene-le
-00003f50: 7665 6c20 7374 6174 6973 7469 6373 2061  vel statistics a
-00003f60: 6e64 206f 7665 7264 6973 7065 7273 696f  nd overdispersio
-00003f70: 6e20 6d6f 6465 6c6c 696e 6720 636f 6d70  n modelling comp
-00003f80: 6c65 7465 642e 2229 0d0a 2020 2020 2020  leted.")..      
-00003f90: 2020 0d0a 2020 2020 6465 6620 7365 6c65    ..    def sele
-00003fa0: 6374 5f6f 7665 7264 6973 7065 7273 6564  ct_overdispersed
-00003fb0: 5f67 656e 6573 5f66 726f 6d5f 6765 6e65  _genes_from_gene
-00003fc0: 6c69 7374 2873 656c 662c 2067 656e 6573  list(self, genes
-00003fd0: 3a20 436f 6c6c 6563 7469 6f6e 2c20 6d69  : Collection, mi
-00003fe0: 6e5f 6d65 616e 3d30 293a 0d0a 2020 2020  n_mean=0):..    
-00003ff0: 2020 2020 2222 2253 656c 6563 7420 6f76      """Select ov
-00004000: 6572 6469 7370 6572 7365 6420 6765 6e65  erdispersed gene
-00004010: 732f 6665 6174 7572 6573 2075 7369 6e67  s/features using
-00004020: 2061 2063 7573 746f 6d20 6c69 7374 2e20   a custom list. 
-00004030: 4765 6e65 732f 6665 6174 7572 6573 206e  Genes/features n
-00004040: 6f74 2070 7265 7365 6e74 2069 6e20 7468  ot present in th
-00004050: 6520 6461 7461 7365 7420 6172 6520 6175  e dataset are au
-00004060: 746f 6d61 7469 6361 6c6c 7920 6669 6c74  tomatically filt
-00004070: 6572 6564 206f 7574 2e0d 0a0d 0a20 2020  ered out.....   
-00004080: 2020 2020 203a 7061 7261 6d20 6765 6e65       :param gene
-00004090: 733a 2067 656e 6520 6c69 7374 0d0a 2020  s: gene list..  
-000040a0: 2020 2020 2020 3a74 7970 6520 6765 6e65        :type gene
-000040b0: 733a 2043 6f6c 6c65 6374 696f 6e0d 0a20  s: Collection.. 
-000040c0: 2020 2020 2020 203a 7061 7261 6d20 6d69         :param mi
-000040d0: 6e5f 6d65 616e 3a20 6d69 6e69 6d75 6d20  n_mean: minimum 
-000040e0: 6765 6e65 2065 7870 7265 7373 696f 6e20  gene expression 
-000040f0: 666f 7220 6765 6e65 7320 746f 2062 6520  for genes to be 
-00004100: 636f 756e 7465 6420 6173 206f 7665 7264  counted as overd
-00004110: 6973 7065 7273 6564 2c20 6465 6661 756c  ispersed, defaul
-00004120: 7473 2074 6f20 300d 0a20 2020 2020 2020  ts to 0..       
-00004130: 203a 7479 7065 206d 696e 5f6d 6561 6e3a   :type min_mean:
-00004140: 2069 6e74 2c20 6f70 7469 6f6e 616c 0d0a   int, optional..
-00004150: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00004160: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
-00004170: 7661 725b 2273 656c 6563 7465 6422 5d20  var["selected"] 
-00004180: 3d20 7365 6c66 2e61 6461 7461 2e76 6172  = self.adata.var
-00004190: 2e69 6e64 6578 2e69 7369 6e28 6765 6e65  .index.isin(gene
-000041a0: 7329 2026 2073 656c 662e 6164 6174 612e  s) & self.adata.
-000041b0: 7661 725b 226d 6561 6e5f 636f 756e 7473  var["mean_counts
-000041c0: 225d 203e 3d20 6d69 6e5f 6d65 616e 0d0a  "] >= min_mean..
-000041d0: 2020 2020 2020 2020 7365 6c66 2e61 6461          self.ada
-000041e0: 7461 2e75 6e73 5b22 6f64 6722 5d5b 226f  ta.uns["odg"]["o
-000041f0: 7665 7264 6973 7065 7273 696f 6e5f 6d65  verdispersion_me
-00004200: 7472 6963 225d 203d 2022 220d 0a20 2020  tric"] = ""..   
-00004210: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
-00004220: 756e 735b 226f 6467 225d 5b22 6d69 6e5f  uns["odg"]["min_
-00004230: 6d65 616e 225d 203d 206d 696e 5f6d 6561  mean"] = min_mea
-00004240: 6e0d 0a20 2020 2020 2020 2073 656c 662e  n..        self.
-00004250: 6164 6174 612e 756e 735b 226f 6467 225d  adata.uns["odg"]
-00004260: 5b22 6d69 6e5f 7363 6f72 6522 5d20 3d20  ["min_score"] = 
-00004270: 2222 0d0a 2020 2020 2020 2020 7365 6c66  ""..        self
-00004280: 2e61 6461 7461 2e75 6e73 5b22 6f64 6722  .adata.uns["odg"
-00004290: 5d5b 2274 6f70 5f6e 225d 203d 2022 220d  ]["top_n"] = "".
-000042a0: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
-000042b0: 6174 612e 756e 735b 226f 6467 225d 5b22  ata.uns["odg"]["
-000042c0: 7175 616e 7469 6c65 225d 203d 2022 220d  quantile"] = "".
-000042d0: 0a20 2020 2020 2020 2073 656c 662e 6170  .        self.ap
-000042e0: 7065 6e64 5f74 6f5f 6869 7374 6f72 7928  pend_to_history(
-000042f0: 224f 7665 7264 6973 7065 7273 6564 2067  "Overdispersed g
-00004300: 656e 6573 2073 656c 6563 7465 6420 6672  enes selected fr
-00004310: 6f6d 2063 7573 746f 6d20 6765 6e65 206c  om custom gene l
-00004320: 6973 7422 290d 0a20 2020 2020 2020 200d  ist")..        .
-00004330: 0a20 2020 2064 6566 2073 656c 6563 745f  .    def select_
-00004340: 6f76 6572 6469 7370 6572 7365 645f 6765  overdispersed_ge
-00004350: 6e65 7328 7365 6c66 2c0d 0a20 2020 2020  nes(self,..     
-00004360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004370: 2020 2020 2020 2020 2020 2020 2020 6f76                ov
-00004380: 6572 6469 7370 6572 7369 6f6e 5f6d 6574  erdispersion_met
-00004390: 7269 633a 2073 7472 203d 2022 6f64 7363  ric: str = "odsc
-000043a0: 6f72 6522 2c0d 0a20 2020 2020 2020 2020  ore",..         
-000043b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043c0: 2020 2020 2020 2020 2020 6d69 6e5f 6d65            min_me
-000043d0: 616e 3a20 666c 6f61 7420 3d20 302c 0d0a  an: float = 0,..
-000043e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004400: 2020 206d 696e 5f73 636f 7265 3a20 666c     min_score: fl
-00004410: 6f61 7420 3d20 312e 302c 0d0a 2020 2020  oat = 1.0,..    
-00004420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004430: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00004440: 6f70 5f6e 3a20 696e 7420 3d20 4e6f 6e65  op_n: int = None
-00004450: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00004460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004470: 2020 2020 2020 7175 616e 7469 6c65 3a20        quantile: 
-00004480: 666c 6f61 7420 3d20 4e6f 6e65 293a 0d0a  float = None):..
-00004490: 2020 2020 2020 2020 2222 2253 656c 6563          """Selec
-000044a0: 7420 6f76 6572 6469 7370 6572 7365 6420  t overdispersed 
-000044b0: 6765 6e65 732f 6665 6174 7572 6573 2075  genes/features u
-000044c0: 7369 6e67 2061 6e20 6f76 6572 6469 7370  sing an overdisp
-000044d0: 6572 7369 6f6e 206d 6574 7269 632e 204f  ersion metric. O
-000044e0: 7074 696f 6e61 6c6c 7920 7365 7420 6120  ptionally set a 
-000044f0: 6d69 6e69 6d75 6d20 6765 6e65 2065 7870  minimum gene exp
-00004500: 7265 7373 696f 6e20 6c65 7665 6c2e 0d0a  ression level...
-00004510: 2020 2020 2020 2020 5365 7420 6120 7468          Set a th
-00004520: 7265 7368 6f6c 6420 7573 696e 6720 7468  reshold using th
-00004530: 6520 746f 7020 4e20 2827 746f 705f 6e27  e top N ('top_n'
-00004540: 292c 206d 696e 696d 756d 2073 636f 7265  ), minimum score
-00004550: 2028 276d 696e 5f73 636f 7265 2729 2c20   ('min_score'), 
-00004560: 6f72 2070 726f 706f 7274 696f 6e20 6f66  or proportion of
-00004570: 2066 6561 7475 7265 7320 2827 7175 616e   features ('quan
-00004580: 7469 6c65 2729 206d 6574 686f 6473 2e0d  tile') methods..
-00004590: 0a20 2020 2020 2020 204f 7665 7264 6973  .        Overdis
-000045a0: 7065 7273 6564 2067 656e 6520 6c69 7374  persed gene list
-000045b0: 2069 7320 7361 7665 6420 696e 2074 6865   is saved in the
-000045c0: 2044 6174 6173 6574 206f 626a 6563 742e   Dataset object.
-000045d0: 0d0a 0d0a 2020 2020 2020 2020 3a70 6172  ....        :par
-000045e0: 616d 206f 7665 7264 6973 7065 7273 696f  am overdispersio
-000045f0: 6e5f 6d65 7472 6963 3a20 226f 6473 636f  n_metric: "odsco
-00004600: 7265 2220 6f72 2022 7673 636f 7265 222c  re" or "vscore",
-00004610: 2064 6566 6175 6c74 7320 746f 2022 6f64   defaults to "od
-00004620: 7363 6f72 6522 0d0a 2020 2020 2020 2020  score"..        
-00004630: 3a74 7970 6520 6f76 6572 6469 7370 6572  :type overdisper
-00004640: 7369 6f6e 5f6d 6574 7269 633a 2073 7472  sion_metric: str
-00004650: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
-00004660: 2020 2020 3a70 6172 616d 206d 696e 5f6d      :param min_m
-00004670: 6561 6e3a 206d 696e 696d 756d 2067 656e  ean: minimum gen
-00004680: 6520 6578 7072 6573 7369 6f6e 2066 6f72  e expression for
-00004690: 2067 656e 6573 2074 6f20 6265 2063 6f75   genes to be cou
-000046a0: 6e74 6564 2061 7320 6f76 6572 6469 7370  nted as overdisp
-000046b0: 6572 7365 642c 2064 6566 6175 6c74 7320  ersed, defaults 
-000046c0: 746f 2030 0d0a 2020 2020 2020 2020 3a74  to 0..        :t
-000046d0: 7970 6520 6d69 6e5f 6d65 616e 3a20 696e  ype min_mean: in
-000046e0: 742c 206f 7074 696f 6e61 6c0d 0a20 2020  t, optional..   
-000046f0: 2020 2020 203a 7061 7261 6d20 6d69 6e5f       :param min_
-00004700: 7363 6f72 653a 206d 696e 696d 756d 2073  score: minimum s
-00004710: 636f 7265 2066 6f72 206f 7665 7264 6973  core for overdis
-00004720: 7065 7273 696f 6e2c 2064 6566 6175 6c74  persion, default
-00004730: 7320 746f 2031 2e30 0d0a 2020 2020 2020  s to 1.0..      
-00004740: 2020 3a74 7970 6520 6d69 6e5f 7363 6f72    :type min_scor
-00004750: 653a 2066 6c6f 6174 2c20 6f70 7469 6f6e  e: float, option
-00004760: 616c 0d0a 2020 2020 2020 2020 3a70 6172  al..        :par
-00004770: 616d 2074 6f70 5f6e 3a20 4368 6f6f 7365  am top_n: Choose
-00004780: 2074 6865 2074 6f70 204e 206d 6f73 7420   the top N most 
-00004790: 6f76 6572 6469 7370 6572 7365 6420 6765  overdispersed ge
-000047a0: 6e65 732c 2064 6566 6175 6c74 7320 746f  nes, defaults to
-000047b0: 204e 6f6e 650d 0a20 2020 2020 2020 203a   None..        :
-000047c0: 7479 7065 2074 6f70 5f6e 3a20 696e 742c  type top_n: int,
-000047d0: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
-000047e0: 2020 203a 7061 7261 6d20 7175 616e 7469     :param quanti
-000047f0: 6c65 3a20 4368 6f6f 7365 2061 2071 7561  le: Choose a qua
-00004800: 6e74 696c 6520 6f66 206f 7665 7264 6973  ntile of overdis
-00004810: 7065 7273 696f 6e2e 2046 6f72 2065 7861  persion. For exa
-00004820: 6d70 6c65 2c20 7468 6520 746f 7020 3130  mple, the top 10
-00004830: 2520 6f66 206f 7665 7264 6973 7065 7273  % of overdispers
-00004840: 6564 2067 656e 6573 2077 6f75 6c64 2062  ed genes would b
-00004850: 6520 302e 3130 2e20 4465 6661 756c 7473  e 0.10. Defaults
-00004860: 2074 6f20 4e6f 6e65 0d0a 2020 2020 2020   to None..      
-00004870: 2020 3a74 7970 6520 7175 616e 7469 6c65    :type quantile
-00004880: 3a20 666c 6f61 742c 206f 7074 696f 6e61  : float, optiona
-00004890: 6c0d 0a20 2020 2020 2020 203a 7261 6973  l..        :rais
-000048a0: 6573 2056 616c 7565 4572 726f 723a 2045  es ValueError: E
-000048b0: 7272 6f72 2069 6620 696e 7661 6c69 6420  rror if invalid 
-000048c0: 6f76 6572 6469 7370 6572 7369 6f6e 206d  overdispersion m
-000048d0: 6574 7269 6320 6973 2063 686f 7365 6e2e  etric is chosen.
-000048e0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-000048f0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00004900: 2069 6620 6f76 6572 6469 7370 6572 7369   if overdispersi
-00004910: 6f6e 5f6d 6574 7269 6320 6e6f 7420 696e  on_metric not in
-00004920: 2073 656c 662e 6164 6174 612e 7661 722e   self.adata.var.
-00004930: 636f 6c75 6d6e 733a 0d0a 2020 2020 2020  columns:..      
-00004940: 2020 2020 2020 6966 206f 7665 7264 6973        if overdis
-00004950: 7065 7273 696f 6e5f 6d65 7472 6963 2069  persion_metric i
-00004960: 6e20 2822 6f64 7363 6f72 6522 2c20 2276  n ("odscore", "v
-00004970: 7363 6f72 6522 293a 0d0a 2020 2020 2020  score"):..      
-00004980: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00004990: 5661 6c75 6545 7272 6f72 280d 0a20 2020  ValueError(..   
-000049a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049b0: 2066 227b 6f76 6572 6469 7370 6572 7369   f"{overdispersi
-000049c0: 6f6e 5f6d 6574 7269 637d 2068 6173 206e  on_metric} has n
-000049d0: 6f74 2062 6565 6e20 6361 6c63 756c 6174  ot been calculat
-000049e0: 6564 2066 6f72 2074 6869 7320 6461 7461  ed for this data
-000049f0: 7365 742e 2022 0d0a 2020 2020 2020 2020  set. "..        
-00004a00: 2020 2020 2020 2020 2020 2020 2245 6e73              "Ens
-00004a10: 7572 6520 7468 6174 2079 6f75 2063 616c  ure that you cal
-00004a20: 6c20 7468 6520 6044 6174 6173 6574 2e63  l the `Dataset.c
-00004a30: 6f6d 7075 7465 5f67 656e 655f 7374 6174  ompute_gene_stat
-00004a40: 7328 2960 2066 6972 7374 2e22 0d0a 2020  s()` first."..  
-00004a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a60: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-00004a70: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00004a80: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00004a90: 6c75 6545 7272 6f72 280d 0a20 2020 2020  lueError(..     
-00004aa0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00004ab0: 227b 6f76 6572 6469 7370 6572 7369 6f6e  "{overdispersion
-00004ac0: 5f6d 6574 7269 637d 2069 7320 6e6f 7420  _metric} is not 
-00004ad0: 6120 7661 6c69 6420 6f76 6572 6469 7370  a valid overdisp
-00004ae0: 6572 7369 6f6e 206d 6574 7269 632e 220d  ersion metric.".
-00004af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004b00: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-00004b10: 0d0a 2020 2020 2020 2020 2320 7761 726e  ..        # warn
-00004b20: 2069 6620 6d75 6c74 6970 6c65 206d 6574   if multiple met
-00004b30: 686f 6473 2061 7265 2073 656c 6563 7465  hods are selecte
-00004b40: 640d 0a20 2020 2020 2020 2073 656c 6563  d..        selec
-00004b50: 7465 645f 6d65 7468 6f64 7320 3d20 5b5d  ted_methods = []
-00004b60: 0d0a 2020 2020 2020 2020 6966 206d 696e  ..        if min
-00004b70: 5f73 636f 7265 2069 7320 6e6f 7420 4e6f  _score is not No
-00004b80: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00004b90: 2073 656c 6563 7465 645f 6d65 7468 6f64   selected_method
-00004ba0: 732e 6170 7065 6e64 2822 6d69 6e5f 7363  s.append("min_sc
-00004bb0: 6f72 6522 290d 0a20 2020 2020 2020 2069  ore")..        i
-00004bc0: 6620 746f 705f 6e20 6973 206e 6f74 204e  f top_n is not N
-00004bd0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00004be0: 2020 7365 6c65 6374 6564 5f6d 6574 686f    selected_metho
-00004bf0: 6473 2e61 7070 656e 6428 2274 6f70 5f6e  ds.append("top_n
-00004c00: 2229 0d0a 2020 2020 2020 2020 6966 2071  ")..        if q
-00004c10: 7561 6e74 696c 6520 6973 206e 6f74 204e  uantile is not N
-00004c20: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00004c30: 2020 7365 6c65 6374 6564 5f6d 6574 686f    selected_metho
-00004c40: 6473 2e61 7070 656e 6428 2271 7561 6e74  ds.append("quant
-00004c50: 696c 6522 290d 0a20 2020 2020 2020 2069  ile")..        i
-00004c60: 6620 6c65 6e28 7365 6c65 6374 6564 5f6d  f len(selected_m
-00004c70: 6574 686f 6473 2920 3e20 313a 0d0a 2020  ethods) > 1:..  
-00004c80: 2020 2020 2020 2020 2020 6d65 7468 6f64            method
-00004c90: 7761 726e 7374 7220 3d20 222c 2022 2e6a  warnstr = ", ".j
-00004ca0: 6f69 6e28 7365 6c65 6374 6564 5f6d 6574  oin(selected_met
-00004cb0: 686f 6473 290d 0a20 2020 2020 2020 2020  hods)..         
-00004cc0: 2020 206c 6f67 6769 6e67 2e77 6172 6e69     logging.warni
-00004cd0: 6e67 2866 224d 756c 7469 706c 6520 636f  ng(f"Multiple co
-00004ce0: 6e66 6c69 6374 696e 6720 6f76 6572 6469  nflicting overdi
-00004cf0: 7370 6572 7365 6420 6765 6e65 2073 656c  spersed gene sel
-00004d00: 6563 7469 6f6e 2063 7269 7465 7269 6120  ection criteria 
-00004d10: 6861 7665 2062 6565 6e20 7365 6c65 6374  have been select
-00004d20: 6564 3a20 7b6d 6574 686f 6477 6172 6e73  ed: {methodwarns
-00004d30: 7472 7d2e 2022 0d0a 2020 2020 2020 2020  tr}. "..        
-00004d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d50: 2020 2020 224f 6e6c 7920 7468 6520 696e      "Only the in
-00004d60: 7465 7273 6563 7469 6f6e 206f 6620 7468  tersection of th
-00004d70: 6573 6520 6d65 7468 6f64 7320 7769 6c6c  ese methods will
-00004d80: 2062 6520 7365 6c65 6374 6564 2e22 290d   be selected.").
-00004d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004da0: 200d 0a20 2020 2020 2020 2023 206d 696e   ..        # min
-00004db0: 5f6d 6561 6e20 6669 6c74 6572 0d0a 2020  _mean filter..  
-00004dc0: 2020 2020 2020 7365 6c65 6374 6564 5f67        selected_g
-00004dd0: 656e 6573 203d 2073 656c 662e 6164 6174  enes = self.adat
-00004de0: 612e 7661 725b 226d 6561 6e5f 636f 756e  a.var["mean_coun
-00004df0: 7473 225d 203e 3d20 6d69 6e5f 6d65 616e  ts"] >= min_mean
-00004e00: 0d0a 2020 2020 2020 2020 2320 6d69 6e5f  ..        # min_
-00004e10: 7363 6f72 6520 6669 6c74 6572 0d0a 2020  score filter..  
-00004e20: 2020 2020 2020 6966 206d 696e 5f73 636f        if min_sco
-00004e30: 7265 2069 7320 6e6f 7420 4e6f 6e65 3a0d  re is not None:.
-00004e40: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00004e50: 6563 7465 645f 6765 6e65 7320 3d20 7365  ected_genes = se
-00004e60: 6c65 6374 6564 5f67 656e 6573 2026 2028  lected_genes & (
-00004e70: 7365 6c66 2e61 6461 7461 2e76 6172 5b6f  self.adata.var[o
-00004e80: 7665 7264 6973 7065 7273 696f 6e5f 6d65  verdispersion_me
-00004e90: 7472 6963 5d20 3e3d 206d 696e 5f73 636f  tric] >= min_sco
-00004ea0: 7265 290d 0a20 2020 2020 2020 2023 2074  re)..        # t
-00004eb0: 6f70 5f6e 2066 696c 7465 720d 0a20 2020  op_n filter..   
-00004ec0: 2020 2020 2069 6620 746f 705f 6e20 6973       if top_n is
+00000af0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00000b00: 726f 7228 6572 726f 726d 7367 290d 0a20  ror(errormsg).. 
+00000b10: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00000b20: 2063 6865 636b 2066 6f72 2077 6865 7468   check for wheth
+00000b30: 6572 2075 7365 7220 6f72 6967 696e 616c  er user original
+00000b40: 6c79 2069 6e70 7574 206e 6f72 6d61 6c69  ly input normali
+00000b50: 7a65 6420 6f72 2063 6f75 6e74 7320 6461  zed or counts da
+00000b60: 7461 0d0a 2020 2020 2020 2020 2020 2020  ta..            
+00000b70: 2020 2020 6973 5f6e 6f72 6d61 6c69 7a65      is_normalize
+00000b80: 6420 3d20 2828 5820 2d20 7261 7729 2e61  d = ((X - raw).a
+00000b90: 6273 2829 203c 2031 652d 3629 2e61 6c6c  bs() < 1e-6).all
+00000ba0: 2829 2e61 6c6c 2829 0d0a 2020 2020 2020  ().all()..      
+00000bb0: 2020 2020 2020 2020 2020 585f 6973 5f74            X_is_t
+00000bc0: 706d 203d 2028 2858 2e73 756d 2861 7869  pm = ((X.sum(axi
+00000bd0: 733d 3129 202d 2031 6536 292e 6162 7328  s=1) - 1e6).abs(
+00000be0: 2920 3e20 3165 3229 2e61 6e79 2829 0d0a  ) > 1e2).any()..
+00000bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c00: 6966 2069 735f 6e6f 726d 616c 697a 6564  if is_normalized
+00000c10: 2061 6e64 206e 6f74 2058 5f69 735f 7470   and not X_is_tp
+00000c20: 6d3a 0d0a 2020 2020 2020 2020 2020 2020  m:..            
+00000c30: 2020 2020 2020 2020 6c6f 6767 696e 672e          logging.
+00000c40: 7761 726e 696e 6728 2241 6e6e 4461 7461  warning("AnnData
+00000c50: 206f 626a 6563 7420 636f 6e74 6169 6e73   object contains
+00000c60: 206e 6f6e 2d54 504d 206e 6f72 6d61 6c69   non-TPM normali
+00000c70: 7a65 6420 6461 7461 2e20 4e65 7720 416e  zed data. New An
+00000c80: 6e44 6174 6120 6f62 6a65 6374 2077 696c  nData object wil
+00000c90: 6c20 7265 7461 696e 2074 6865 2063 6f75  l retain the cou
+00000ca0: 6e74 2028 756e 6e6f 726d 616c 697a 6564  nt (unnormalized
+00000cb0: 2920 6461 7461 206f 6e6c 792e 2229 0d0a  ) data only.")..
+00000cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000cd0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00000ce0: 2022 6f64 6722 2069 6e20 6164 6174 612e   "odg" in adata.
+00000cf0: 756e 7320 616e 6420 2267 656e 655f 7374  uns and "gene_st
+00000d00: 6174 7322 2069 6e20 6164 6174 612e 756e  ats" in adata.un
+00000d10: 735b 226f 6467 225d 3a0d 0a20 2020 2020  s["odg"]:..     
+00000d20: 2020 2020 2020 2020 2020 2067 656e 655f             gene_
+00000d30: 7374 6174 5f63 6f6c 756d 6e73 203d 2061  stat_columns = a
+00000d40: 6461 7461 2e75 6e73 5b22 6f64 6722 5d5b  data.uns["odg"][
+00000d50: 2267 656e 655f 7374 6174 7322 5d2e 636f  "gene_stats"].co
+00000d60: 6c75 6d6e 730d 0a20 2020 2020 2020 2020  lumns..         
+00000d70: 2020 2020 2020 2069 6620 6164 6174 612e         if adata.
+00000d80: 7661 722e 636f 6c75 6d6e 732e 6973 696e  var.columns.isin
+00000d90: 2867 656e 655f 7374 6174 5f63 6f6c 756d  (gene_stat_colum
+00000da0: 6e73 292e 616e 7928 293a 0d0a 2020 2020  ns).any():..    
+00000db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000dc0: 6f76 6572 6c61 7070 696e 675f 636f 6c73  overlapping_cols
+00000dd0: 203d 2061 6461 7461 2e76 6172 2e63 6f6c   = adata.var.col
+00000de0: 756d 6e73 2e69 7369 6e28 6765 6e65 5f73  umns.isin(gene_s
+00000df0: 7461 745f 636f 6c75 6d6e 7329 0d0a 2020  tat_columns)..  
+00000e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e10: 2020 6f76 6572 6c61 7070 696e 675f 636f    overlapping_co
+00000e20: 6c73 7472 203d 2022 2c20 222e 6a6f 696e  lstr = ", ".join
+00000e30: 286f 7665 726c 6170 7069 6e67 5f63 6f6c  (overlapping_col
+00000e40: 735b 6f76 6572 6c61 7070 696e 675f 636f  s[overlapping_co
+00000e50: 6c73 5d2e 696e 6465 782e 746f 5f6c 6973  ls].index.to_lis
+00000e60: 7428 2929 0d0a 2020 2020 2020 2020 2020  t())..          
+00000e70: 2020 2020 2020 2020 2020 6c6f 6767 696e            loggin
+00000e80: 672e 7761 726e 696e 6728 6622 416e 6e44  g.warning(f"AnnD
+00000e90: 6174 6120 6f62 6a65 6374 2063 6f6e 7461  ata object conta
+00000ea0: 696e 7320 634e 4d46 2067 656e 6520 7374  ins cNMF gene st
+00000eb0: 6174 7320 7768 6963 6820 7769 6c6c 206f  ats which will o
+00000ec0: 7665 7272 6964 6520 636f 6c75 6d6e 7320  verride columns 
+00000ed0: 696e 2061 6461 7461 2e76 6172 3a20 7b6f  in adata.var: {o
+00000ee0: 7665 726c 6170 7069 6e67 5f63 6f6c 7374  verlapping_colst
+00000ef0: 727d 2229 0d0a 2020 2020 2020 2020 2020  r}")..          
+00000f00: 2020 2020 2020 6164 6174 612e 7661 7220        adata.var 
+00000f10: 3d20 7064 2e6d 6572 6765 286c 6566 743d  = pd.merge(left=
+00000f20: 6164 6174 612e 7661 722c 2072 6967 6874  adata.var, right
+00000f30: 3d61 6461 7461 2e75 6e73 5b22 6f64 6722  =adata.uns["odg"
+00000f40: 5d5b 2267 656e 655f 7374 6174 7322 5d2c  ]["gene_stats"],
+00000f50: 2068 6f77 3d22 6c65 6674 222c 206c 6566   how="left", lef
+00000f60: 745f 696e 6465 783d 5472 7565 2c20 7269  t_index=True, ri
+00000f70: 6768 745f 696e 6465 783d 5472 7565 290d  ght_index=True).
+00000f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000f90: 2064 656c 2061 6461 7461 2e75 6e73 5b22   del adata.uns["
+00000fa0: 6f64 6722 5d5b 2267 656e 655f 7374 6174  odg"]["gene_stat
+00000fb0: 7322 5d0d 0a20 2020 2020 2020 2020 2020  s"]..           
+00000fc0: 200d 0a20 2020 2020 2020 2020 2020 2023   ..            #
+00000fd0: 2063 7265 6174 6520 6e65 7720 416e 6e44   create new AnnD
+00000fe0: 6174 6120 6f62 6a65 6374 0d0a 2020 2020  ata object..    
+00000ff0: 2020 2020 2020 2020 6e65 775f 6164 6174          new_adat
+00001000: 6120 3d20 6164 2e41 6e6e 4461 7461 2858  a = ad.AnnData(X
+00001010: 3d72 6177 2c20 6f62 733d 6164 6174 612e  =raw, obs=adata.
+00001020: 6f62 732c 2076 6172 3d61 6461 7461 2e76  obs, var=adata.v
+00001030: 6172 2c20 7661 726d 3d61 6461 7461 2e76  ar, varm=adata.v
+00001040: 6172 6d2c 206f 6273 6d3d 6164 6174 612e  arm, obsm=adata.
+00001050: 6f62 736d 2c20 756e 733d 6164 6174 612e  obsm, uns=adata.
+00001060: 756e 7329 0d0a 2020 2020 2020 2020 2020  uns)..          
+00001070: 2020 6966 2022 6869 7374 6f72 7922 206e    if "history" n
+00001080: 6f74 2069 6e20 6e65 775f 6164 6174 612e  ot in new_adata.
+00001090: 756e 733a 0d0a 2020 2020 2020 2020 2020  uns:..          
+000010a0: 2020 2020 2020 6e65 775f 6164 6174 612e        new_adata.
+000010b0: 756e 735b 2268 6973 746f 7279 225d 203d  uns["history"] =
+000010c0: 207b 7d0d 0a0d 0a20 2020 2020 2020 2020   {}....         
+000010d0: 2020 2023 2075 7064 6174 6520 6461 7461     # update data
+000010e0: 7365 7420 6f62 6a65 6374 0d0a 2020 2020  set object..    
+000010f0: 2020 2020 2020 2020 7365 6c66 2e61 6461          self.ada
+00001100: 7461 203d 206e 6577 5f61 6461 7461 0d0a  ta = new_adata..
+00001110: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00001120: 2e69 735f 6e6f 726d 616c 697a 6564 203d  .is_normalized =
+00001130: 2069 735f 6e6f 726d 616c 697a 6564 0d0a   is_normalized..
+00001140: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00001150: 2e63 6e6d 6673 6e73 5f76 6572 7369 6f6e  .cnmfsns_version
+00001160: 203d 205f 5f76 6572 7369 6f6e 5f5f 0d0a   = __version__..
+00001170: 2020 2020 0d0a 2020 2020 2020 2020 6966      ..        if
+00001180: 2070 6174 6965 6e74 5f69 645f 636f 6c20   patient_id_col 
+00001190: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+000011a0: 7061 7469 656e 745f 6964 5f63 6f6c 206e  patient_id_col n
+000011b0: 6f74 2069 6e20 7365 6c66 2e61 6461 7461  ot in self.adata
+000011c0: 2e6f 6273 2e63 6f6c 756d 6e73 3a0d 0a20  .obs.columns:.. 
+000011d0: 2020 2020 2020 2020 2020 2061 7661 696c             avail
+000011e0: 5f63 6f6c 756d 6e73 203d 2022 2c20 222e  _columns = ", ".
+000011f0: 6a6f 696e 2873 656c 662e 6164 6174 612e  join(self.adata.
+00001200: 6f62 732e 636f 6c75 6d6e 7329 0d0a 2020  obs.columns)..  
+00001210: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00001220: 5661 6c75 6545 7272 6f72 2866 227b 7061  ValueError(f"{pa
+00001230: 7469 656e 745f 6964 5f63 6f6c 7d20 6973  tient_id_col} is
+00001240: 206e 6f74 2061 2076 616c 6964 2063 6f6c   not a valid col
+00001250: 756d 6e20 696e 2074 6865 206d 6574 6164  umn in the metad
+00001260: 6174 6120 6d61 7472 6978 2e20 4176 6169  ata matrix. Avai
+00001270: 6c61 626c 6520 636f 6c75 6d6e 7320 6172  lable columns ar
+00001280: 653a 207b 6176 6169 6c5f 636f 6c75 6d6e  e: {avail_column
+00001290: 737d 2229 0d0a 2020 2020 2020 2020 7365  s}")..        se
+000012a0: 6c66 2e70 6174 6965 6e74 5f69 645f 636f  lf.patient_id_co
+000012b0: 6c20 3d20 7061 7469 656e 745f 6964 5f63  l = patient_id_c
+000012c0: 6f6c 0d0a 2020 2020 0d0a 2020 2020 4063  ol..    ..    @c
+000012d0: 6c61 7373 6d65 7468 6f64 0d0a 2020 2020  lassmethod..    
+000012e0: 6465 6620 6672 6f6d 5f64 6628 636c 732c  def from_df(cls,
+000012f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001300: 2020 2020 6461 7461 3a20 7064 2e44 6174      data: pd.Dat
+00001310: 6146 7261 6d65 2c0d 0a20 2020 2020 2020  aFrame,..       
+00001320: 2020 2020 2020 2020 2020 2069 735f 6e6f             is_no
+00001330: 726d 616c 697a 6564 3a20 626f 6f6c 2c0d  rmalized: bool,.
+00001340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001350: 2020 2073 7061 7273 6966 793a 2062 6f6f     sparsify: boo
+00001360: 6c20 3d20 4661 6c73 652c 0d0a 2020 2020  l = False,..    
+00001370: 2020 2020 2020 2020 2020 2020 2020 6f62                ob
+00001380: 733a 204f 7074 696f 6e61 6c5b 7064 2e44  s: Optional[pd.D
+00001390: 6174 6146 7261 6d65 5d20 3d20 4e6f 6e65  ataFrame] = None
+000013a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000013b0: 2020 2020 2076 6172 3a20 4f70 7469 6f6e       var: Option
+000013c0: 616c 5b70 642e 4461 7461 4672 616d 655d  al[pd.DataFrame]
+000013d0: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
+000013e0: 2020 2020 2020 2020 2020 2020 7061 7469              pati
+000013f0: 656e 745f 6964 5f63 6f6c 3a20 4f70 7469  ent_id_col: Opti
+00001400: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00001410: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001420: 2020 2020 293a 0d0a 2020 2020 2020 2020      ):..        
+00001430: 2222 2243 7265 6174 6573 2061 203a 636c  """Creates a :cl
+00001440: 6173 733a 607e 636e 6d66 736e 732e 6461  ass:`~cnmfsns.da
+00001450: 7461 7365 742e 4461 7461 7365 7460 206f  taset.Dataset` o
+00001460: 626a 6563 7420 6672 6f6d 2061 2070 616e  bject from a pan
+00001470: 6461 7320 4461 7461 4672 616d 652e 0d0a  das DataFrame...
+00001480: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+00001490: 2064 6174 613a 2041 6e20 6f62 7365 7276   data: An observ
+000014a0: 6174 696f 6e73 20c3 9720 7661 7269 6162  ations .. variab
+000014b0: 6c65 7320 6461 7461 0d0a 2020 2020 2020  les data..      
+000014c0: 2020 3a74 7970 6520 6461 7461 3a20 7064    :type data: pd
+000014d0: 2e44 6174 6146 7261 6d65 0d0a 2020 2020  .DataFrame..    
+000014e0: 2020 2020 3a70 6172 616d 2069 735f 6e6f      :param is_no
+000014f0: 726d 616c 697a 6564 3a20 5370 6563 6966  rmalized: Specif
+00001500: 7920 6966 2064 6174 6120 6973 2061 6c72  y if data is alr
+00001510: 6561 6479 206e 6f72 6d61 6c69 7a65 6420  eady normalized 
+00001520: 6f72 2077 6865 7468 6572 206e 6f74 2e20  or whether not. 
+00001530: 5261 7720 6461 7461 2077 696c 6c20 6265  Raw data will be
+00001540: 2054 504d 206e 6f72 6d61 6c69 7a65 6420   TPM normalized 
+00001550: 7072 696f 7220 746f 206f 7665 7264 6973  prior to overdis
+00001560: 7065 7273 6564 2067 656e 6520 7365 6c65  persed gene sele
+00001570: 6374 696f 6e2c 2077 6865 7265 6173 2061  ction, whereas a
+00001580: 6c72 6561 6479 206e 6f72 6d61 6c69 7a65  lready normalize
+00001590: 6420 6461 7461 2077 696c 6c20 6e6f 742e  d data will not.
+000015a0: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+000015b0: 6973 5f6e 6f72 6d61 6c69 7a65 643a 2062  is_normalized: b
+000015c0: 6f6f 6c0d 0a20 2020 2020 2020 203a 7061  ool..        :pa
+000015d0: 7261 6d20 7370 6172 7369 6679 3a20 5374  ram sparsify: St
+000015e0: 6f72 6520 6461 7461 2061 7320 6120 7370  ore data as a sp
+000015f0: 6172 7365 206d 6174 7269 782e 205b 4e6f  arse matrix. [No
+00001600: 7465 2074 6861 7420 7468 6973 2066 6561  te that this fea
+00001610: 7475 7265 2069 7320 6578 7065 7269 6d65  ture is experime
+00001620: 6e74 616c 5d2c 2064 6566 6175 6c74 7320  ntal], defaults 
+00001630: 746f 2046 616c 7365 0d0a 2020 2020 2020  to False..      
+00001640: 2020 3a74 7970 6520 7370 6172 7369 6679    :type sparsify
+00001650: 3a20 626f 6f6c 2c20 6f70 7469 6f6e 616c  : bool, optional
+00001660: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+00001670: 206f 6273 3a20 416e 206f 6273 6572 7661   obs: An observa
+00001680: 7469 6f6e 7320 c397 206d 6574 6164 6174  tions .. metadat
+00001690: 6120 6d61 7472 6978 2c20 6465 6661 756c  a matrix, defaul
+000016a0: 7473 2074 6f20 4e6f 6e65 0d0a 2020 2020  ts to None..    
+000016b0: 2020 2020 3a74 7970 6520 6f62 733a 2060      :type obs: `
+000016c0: 7064 2e44 6174 6146 7261 6d65 602c 206f  pd.DataFrame`, o
+000016d0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
+000016e0: 203a 7061 7261 6d20 7661 723a 2041 2076   :param var: A v
+000016f0: 6172 6961 626c 6573 20c3 9720 6d65 7461  ariables .. meta
+00001700: 6461 7461 206d 6174 7269 782c 2064 6566  data matrix, def
+00001710: 6175 6c74 7320 746f 204e 6f6e 650d 0a20  aults to None.. 
+00001720: 2020 2020 2020 203a 7479 7065 2076 6172         :type var
+00001730: 3a20 6070 642e 4461 7461 4672 616d 6560  : `pd.DataFrame`
+00001740: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
+00001750: 2020 2020 3a70 6172 616d 2070 6174 6965      :param patie
+00001760: 6e74 5f69 645f 636f 6c3a 204e 616d 6520  nt_id_col: Name 
+00001770: 6f66 206d 6574 6164 6174 6120 6c61 7965  of metadata laye
+00001780: 7220 7769 7468 2070 6174 6965 6e74 2049  r with patient I
+00001790: 4420 696e 666f 726d 6174 696f 6e2c 2064  D information, d
+000017a0: 6566 6175 6c74 7320 746f 204e 6f6e 650d  efaults to None.
+000017b0: 0a20 2020 2020 2020 203a 7479 7065 2070  .        :type p
+000017c0: 6174 6965 6e74 5f69 645f 636f 6c3a 2073  atient_id_col: s
+000017d0: 7472 2c20 6f70 7469 6f6e 616c 0d0a 2020  tr, optional..  
+000017e0: 2020 2020 2020 3a72 6574 7572 6e3a 204f        :return: O
+000017f0: 626a 6563 7420 7769 7468 2065 7870 7265  bject with expre
+00001800: 7373 696f 6e20 616e 6420 6d65 7461 6461  ssion and metada
+00001810: 7461 0d0a 2020 2020 2020 2020 3a72 7479  ta..        :rty
+00001820: 7065 3a20 3a63 6c61 7373 3a60 7e63 6e6d  pe: :class:`~cnm
+00001830: 6673 6e73 2e64 6174 6173 6574 2e44 6174  fsns.dataset.Dat
+00001840: 6173 6574 600d 0a20 2020 2020 2020 2022  aset`..        "
+00001850: 2222 0d0a 2020 2020 2020 2020 6966 2076  ""..        if v
+00001860: 6172 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ar is not None:.
+00001870: 0a20 2020 2020 2020 2020 2020 2076 6172  .            var
+00001880: 203d 2076 6172 2e72 6569 6e64 6578 2864   = var.reindex(d
+00001890: 6174 612e 636f 6c75 6d6e 7329 0d0a 2020  ata.columns)..  
+000018a0: 2020 2020 2020 6966 2073 7061 7273 6966        if sparsif
+000018b0: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+000018c0: 6461 7461 203d 2073 702e 6373 725f 6d61  data = sp.csr_ma
+000018d0: 7472 6978 2864 6174 612e 7661 6c75 6573  trix(data.values
+000018e0: 290d 0a20 2020 2020 2020 2064 6174 6120  )..        data 
+000018f0: 3d20 6461 7461 2e61 7374 7970 6528 2266  = data.astype("f
+00001900: 6c6f 6174 3332 2229 0d0a 2020 2020 2020  loat32")..      
+00001910: 2020 756e 7320 3d20 7b22 6869 7374 6f72    uns = {"histor
+00001920: 7922 3a20 7b7d 2c20 226f 6467 223a 7b7d  y": {}, "odg":{}
+00001930: 7d0d 0a20 2020 2020 2020 2061 6461 7461  }..        adata
+00001940: 203d 2061 642e 416e 6e44 6174 6128 583d   = ad.AnnData(X=
+00001950: 6461 7461 2c20 7661 723d 7661 722c 2075  data, var=var, u
+00001960: 6e73 3d75 6e73 290d 0a20 2020 2020 2020  ns=uns)..       
+00001970: 2064 6174 6173 6574 203d 2063 6c73 2861   dataset = cls(a
+00001980: 6461 7461 3d61 6461 7461 2c20 7061 7469  data=adata, pati
+00001990: 656e 745f 6964 5f63 6f6c 3d70 6174 6965  ent_id_col=patie
+000019a0: 6e74 5f69 645f 636f 6c29 0d0a 2020 2020  nt_id_col)..    
+000019b0: 2020 2020 6966 206f 6273 2069 7320 6e6f      if obs is no
+000019c0: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+000019d0: 2020 2020 2064 6174 6173 6574 2e75 7064       dataset.upd
+000019e0: 6174 655f 6f62 7328 6f62 733d 6f62 7329  ate_obs(obs=obs)
+000019f0: 200d 0a20 2020 2020 2020 2072 6574 7572   ..        retur
+00001a00: 6e20 6461 7461 7365 740d 0a20 2020 200d  n dataset..    .
+00001a10: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
+00001a20: 640d 0a20 2020 2064 6566 2066 726f 6d5f  d..    def from_
+00001a30: 6835 6164 2863 6c73 2c0d 0a20 2020 2020  h5ad(cls,..     
+00001a40: 2020 2020 2020 2020 2020 2020 2068 3561               h5a
+00001a50: 645f 6669 6c65 3a20 7374 722c 0d0a 2020  d_file: str,..  
+00001a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a70: 7061 7469 656e 745f 6964 5f63 6f6c 3a20  patient_id_col: 
+00001a80: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00001a90: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2020  None,..         
+00001aa0: 2020 2020 2020 2020 2066 6f72 6365 5f6d           force_m
+00001ab0: 6967 7261 7465 3d46 616c 7365 2c20 6261  igrate=False, ba
+00001ac0: 636b 6564 3d46 616c 7365 0d0a 2020 2020  cked=False..    
+00001ad0: 2020 2020 2020 2020 2020 2020 2020 293a                ):
+00001ae0: 0d0a 2020 2020 2020 2020 2222 2243 7265  ..        """Cre
+00001af0: 6174 6573 2061 203a 636c 6173 733a 607e  ates a :class:`~
+00001b00: 636e 6d66 736e 732e 6461 7461 7365 742e  cnmfsns.dataset.
+00001b10: 4461 7461 7365 7460 206f 626a 6563 7420  Dataset` object 
+00001b20: 6672 6f6d 2061 6e20 416e 6e44 6174 612d  from an AnnData-
+00001b30: 636f 6d70 6174 6962 6c65 202e 6835 6164  compatible .h5ad
+00001b40: 2066 696c 652e 0d0a 0d0a 2020 2020 2020   file.....      
+00001b50: 2020 3a70 6172 616d 2068 3561 645f 6669    :param h5ad_fi
+00001b60: 6c65 3a20 5061 7468 2074 6f20 2e68 3561  le: Path to .h5a
+00001b70: 6420 6669 6c65 2070 726f 6475 6365 6420  d file produced 
+00001b80: 6279 2073 6361 6e70 792c 2041 6e6e 4461  by scanpy, AnnDa
+00001b90: 7461 2c20 6f72 2063 4e4d 462d 534e 530d  ta, or cNMF-SNS.
+00001ba0: 0a20 2020 2020 2020 203a 7479 7065 2068  .        :type h
+00001bb0: 3561 645f 6669 6c65 3a20 7374 720d 0a20  5ad_file: str.. 
+00001bc0: 2020 2020 2020 203a 7061 7261 6d20 7061         :param pa
+00001bd0: 7469 656e 745f 6964 5f63 6f6c 3a20 4e61  tient_id_col: Na
+00001be0: 6d65 206f 6620 6d65 7461 6461 7461 206c  me of metadata l
+00001bf0: 6179 6572 2077 6974 6820 7061 7469 656e  ayer with patien
+00001c00: 7420 4944 2069 6e66 6f72 6d61 7469 6f6e  t ID information
+00001c10: 2c20 6465 6661 756c 7473 2074 6f20 4e6f  , defaults to No
+00001c20: 6e65 0d0a 2020 2020 2020 2020 3a74 7970  ne..        :typ
+00001c30: 6520 7061 7469 656e 745f 6964 5f63 6f6c  e patient_id_col
+00001c40: 3a20 7374 722c 206f 7074 696f 6e61 6c0d  : str, optional.
+00001c50: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00001c60: 666f 7263 655f 6d69 6772 6174 653a 2066  force_migrate: f
+00001c70: 6f72 6365 7320 636f 6e76 6572 7369 6f6e  orces conversion
+00001c80: 206f 6620 416e 6e44 6174 6120 6f62 6a65   of AnnData obje
+00001c90: 6374 7320 6576 656e 2077 6865 6e20 6164  cts even when ad
+00001ca0: 6174 612e 5820 616e 6420 6164 6174 612e  ata.X and adata.
+00001cb0: 7261 772e 5820 6172 6520 6e6f 7420 6c69  raw.X are not li
+00001cc0: 6e65 6172 6c79 2073 6361 6c65 6420 7265  nearly scaled re
+00001cd0: 6c61 7469 7665 2074 6f20 6561 6368 206f  lative to each o
+00001ce0: 7468 6572 2c20 6465 6661 756c 7473 2074  ther, defaults t
+00001cf0: 6f20 4661 6c73 650d 0a20 2020 2020 2020  o False..       
+00001d00: 203a 7479 7065 2066 6f72 6365 5f6d 6967   :type force_mig
+00001d10: 7261 7465 3a20 626f 6f6c 2c20 6f70 7469  rate: bool, opti
+00001d20: 6f6e 616c 0d0a 2020 2020 2020 2020 3a70  onal..        :p
+00001d30: 6172 616d 2062 6163 6b65 643a 2055 7365  aram backed: Use
+00001d40: 2062 6163 6b65 6420 6d6f 6465 2074 6f20   backed mode to 
+00001d50: 6f70 656e 2068 3561 6420 6669 6c65 2e20  open h5ad file. 
+00001d60: 5468 6973 2063 616e 2073 6176 6520 6d65  This can save me
+00001d70: 6d6f 7279 2077 6865 6e20 7468 6520 6461  mory when the da
+00001d80: 7461 7365 7420 6973 2076 6572 7920 6c61  taset is very la
+00001d90: 7267 652c 2062 7574 2069 7320 6e6f 7420  rge, but is not 
+00001da0: 636f 6d70 6174 6962 6c65 2077 6974 6820  compatible with 
+00001db0: 6835 6164 2066 696c 6573 2070 726f 6475  h5ad files produ
+00001dc0: 6365 6420 6f75 7473 6964 6520 6f66 2063  ced outside of c
+00001dd0: 4e4d 462d 534e 532c 2064 6566 6175 6c74  NMF-SNS, default
+00001de0: 7320 746f 2046 616c 7365 0d0a 2020 2020  s to False..    
+00001df0: 2020 2020 3a74 7970 6520 6261 636b 6564      :type backed
+00001e00: 3a20 626f 6f6c 2c20 6f70 7469 6f6e 616c  : bool, optional
+00001e10: 0d0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
+00001e20: 6e3a 204f 626a 6563 7420 7769 7468 2065  n: Object with e
+00001e30: 7870 7265 7373 696f 6e20 616e 6420 6d65  xpression and me
+00001e40: 7461 6461 7461 0d0a 2020 2020 2020 2020  tadata..        
+00001e50: 3a72 7479 7065 3a20 3a63 6c61 7373 3a60  :rtype: :class:`
+00001e60: 7e63 6e6d 6673 6e73 2e64 6174 6173 6574  ~cnmfsns.dataset
+00001e70: 2e44 6174 6173 6574 600d 0a20 2020 2020  .Dataset`..     
+00001e80: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00001e90: 6164 6174 6120 3d20 6164 2e72 6561 645f  adata = ad.read_
+00001ea0: 6835 6164 2868 3561 645f 6669 6c65 2c20  h5ad(h5ad_file, 
+00001eb0: 6261 636b 6564 3d62 6163 6b65 6429 0d0a  backed=backed)..
+00001ec0: 2020 2020 2020 2020 6461 7461 7365 7420          dataset 
+00001ed0: 3d20 636c 7328 6164 6174 613d 6164 6174  = cls(adata=adat
+00001ee0: 612c 2070 6174 6965 6e74 5f69 645f 636f  a, patient_id_co
+00001ef0: 6c3d 7061 7469 656e 745f 6964 5f63 6f6c  l=patient_id_col
+00001f00: 2c20 666f 7263 655f 6d69 6772 6174 653d  , force_migrate=
+00001f10: 666f 7263 655f 6d69 6772 6174 6529 0d0a  force_migrate)..
+00001f20: 2020 2020 2020 2020 7265 7475 726e 2064          return d
+00001f30: 6174 6173 6574 0d0a 2020 2020 0d0a 2020  ataset..    ..  
+00001f40: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
+00001f50: 2064 6566 2069 735f 6e6f 726d 616c 697a   def is_normaliz
+00001f60: 6564 2873 656c 6629 3a0d 0a20 2020 2020  ed(self):..     
+00001f70: 2020 2022 2222 4f75 7470 7574 7320 7468     """Outputs th
+00001f80: 6520 6e6f 726d 616c 697a 6174 696f 6e20  e normalization 
+00001f90: 7374 6174 7573 206f 6620 7468 6520 6461  status of the da
+00001fa0: 7461 7365 742e 0d0a 0d0a 2020 2020 2020  taset.....      
+00001fb0: 2020 3a72 6574 7572 6e3a 2054 7275 6520    :return: True 
+00001fc0: 6966 2064 6174 6173 6574 2063 6f6e 7461  if dataset conta
+00001fd0: 696e 7320 6e6f 726d 616c 697a 6564 2064  ins normalized d
+00001fe0: 6174 612c 2046 616c 7365 2069 6620 6974  ata, False if it
+00001ff0: 2069 7320 7261 7720 6461 7461 2e0d 0a20   is raw data... 
+00002000: 2020 2020 2020 203a 7274 7970 653a 2062         :rtype: b
+00002010: 6f6f 6c0d 0a20 2020 2020 2020 2022 2222  ool..        """
+00002020: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00002030: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
+00002040: 2269 735f 6e6f 726d 616c 697a 6564 225d  "is_normalized"]
+00002050: 0d0a 2020 2020 0d0a 2020 2020 4069 735f  ..    ..    @is_
+00002060: 6e6f 726d 616c 697a 6564 2e73 6574 7465  normalized.sette
+00002070: 720d 0a20 2020 2064 6566 2069 735f 6e6f  r..    def is_no
+00002080: 726d 616c 697a 6564 2873 656c 662c 2076  rmalized(self, v
+00002090: 616c 7565 3a20 626f 6f6c 293a 0d0a 2020  alue: bool):..  
+000020a0: 2020 2020 2020 7365 6c66 2e61 6461 7461        self.adata
+000020b0: 2e75 6e73 5b22 6973 5f6e 6f72 6d61 6c69  .uns["is_normali
+000020c0: 7a65 6422 5d20 3d20 7661 6c75 650d 0a20  zed"] = value.. 
+000020d0: 2020 200d 0a20 2020 2040 7072 6f70 6572     ..    @proper
+000020e0: 7479 0d0a 2020 2020 6465 6620 7061 7469  ty..    def pati
+000020f0: 656e 745f 6964 5f63 6f6c 2873 656c 6629  ent_id_col(self)
+00002100: 3a0d 0a20 2020 2020 2020 2022 2222 4f75  :..        """Ou
+00002110: 7470 7574 7320 7468 6520 6e6f 726d 616c  tputs the normal
+00002120: 697a 6174 696f 6e20 7374 6174 7573 206f  ization status o
+00002130: 6620 7468 6520 6461 7461 7365 742e 0d0a  f the dataset...
+00002140: 0d0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
+00002150: 6e3a 2054 7275 6520 6966 2064 6174 6173  n: True if datas
+00002160: 6574 2063 6f6e 7461 696e 7320 6e6f 726d  et contains norm
+00002170: 616c 697a 6564 2064 6174 612c 2046 616c  alized data, Fal
+00002180: 7365 2069 6620 6974 2069 7320 7261 7720  se if it is raw 
+00002190: 6461 7461 2e0d 0a20 2020 2020 2020 203a  data...        :
+000021a0: 7274 7970 653a 2062 6f6f 6c0d 0a20 2020  rtype: bool..   
+000021b0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+000021c0: 2020 7265 7475 726e 2073 656c 662e 6164    return self.ad
+000021d0: 6174 612e 756e 735b 2270 6174 6965 6e74  ata.uns["patient
+000021e0: 5f69 645f 636f 6c22 5d0d 0a20 2020 200d  _id_col"]..    .
+000021f0: 0a20 2020 2040 7061 7469 656e 745f 6964  .    @patient_id
+00002200: 5f63 6f6c 2e73 6574 7465 720d 0a20 2020  _col.setter..   
+00002210: 2064 6566 2070 6174 6965 6e74 5f69 645f   def patient_id_
+00002220: 636f 6c28 7365 6c66 2c20 7661 6c75 653a  col(self, value:
+00002230: 2073 7472 293a 0d0a 2020 2020 2020 2020   str):..        
+00002240: 7365 6c66 2e61 6461 7461 2e75 6e73 5b22  self.adata.uns["
+00002250: 7061 7469 656e 745f 6964 5f63 6f6c 225d  patient_id_col"]
+00002260: 203d 2076 616c 7565 0d0a 0d0a 2020 2020   = value....    
+00002270: 4070 726f 7065 7274 790d 0a20 2020 2064  @property..    d
+00002280: 6566 2063 6e6d 6673 6e73 5f76 6572 7369  ef cnmfsns_versi
+00002290: 6f6e 2873 656c 6629 3a0d 0a20 2020 2020  on(self):..     
+000022a0: 2020 2022 2222 634e 4d46 2d53 4e53 2076     """cNMF-SNS v
+000022b0: 6572 7369 6f6e 2075 7365 6420 746f 2063  ersion used to c
+000022c0: 7265 6174 6520 7468 6520 6461 7461 7365  reate the datase
+000022d0: 740d 0a0d 0a20 2020 2020 2020 203a 7265  t....        :re
+000022e0: 7475 726e 3a20 7665 7273 696f 6e0d 0a20  turn: version.. 
+000022f0: 2020 2020 2020 203a 7274 7970 653a 2073         :rtype: s
+00002300: 7472 0d0a 2020 2020 2020 2020 2222 220d  tr..        """.
+00002310: 0a20 2020 2020 2020 2069 6620 2263 6e6d  .        if "cnm
+00002320: 6673 6e73 5f76 6572 7369 6f6e 2220 696e  fsns_version" in
+00002330: 2073 656c 662e 6164 6174 612e 756e 733a   self.adata.uns:
+00002340: 0d0a 2020 2020 2020 2020 2020 2020 7665  ..            ve
+00002350: 7273 696f 6e20 3d20 7365 6c66 2e61 6461  rsion = self.ada
+00002360: 7461 2e75 6e73 5b22 636e 6d66 736e 735f  ta.uns["cnmfsns_
+00002370: 7665 7273 696f 6e22 5d0d 0a20 2020 2020  version"]..     
+00002380: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00002390: 2020 2020 2020 7665 7273 696f 6e20 3d20        version = 
+000023a0: 4e6f 6e65 0d0a 2020 2020 2020 2020 7265  None..        re
+000023b0: 7475 726e 2076 6572 7369 6f6e 0d0a 2020  turn version..  
+000023c0: 2020 2020 2020 0d0a 2020 2020 4070 726f        ..    @pro
+000023d0: 7065 7274 790d 0a20 2020 2064 6566 2068  perty..    def h
+000023e0: 6173 5f63 6e6d 665f 7265 7375 6c74 7328  as_cnmf_results(
+000023f0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00002400: 2222 2254 6573 7420 666f 7220 7765 6874  """Test for weht
+00002410: 6865 7220 4461 7461 7365 7420 636f 6e74  her Dataset cont
+00002420: 6169 6e73 2063 4e4d 4620 7265 7375 6c74  ains cNMF result
+00002430: 7320 666f 7220 7468 6520 6461 7461 7365  s for the datase
+00002440: 740d 0a0d 0a20 2020 2020 2020 203a 7265  t....        :re
+00002450: 7475 726e 3a20 5768 6574 6865 7220 636f  turn: Whether co
+00002460: 6d70 6c65 7465 2063 4e4d 4620 7265 7375  mplete cNMF resu
+00002470: 6c74 7320 6172 6520 636f 6e74 6169 6e65  lts are containe
+00002480: 6420 666f 7220 6174 206c 6561 7374 2031  d for at least 1
+00002490: 2072 616e 6b20 286b 290d 0a20 2020 2020   rank (k)..     
+000024a0: 2020 203a 7274 7970 653a 2062 6f6f 6c0d     :rtype: bool.
+000024b0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+000024c0: 2020 2020 2020 6d61 7472 6978 5f63 6865        matrix_che
+000024d0: 636b 7320 3d20 5b0d 0a20 2020 2020 2020  cks = [..       
+000024e0: 2020 2020 2022 636e 6d66 5f75 7361 6765       "cnmf_usage
+000024f0: 2220 696e 2073 656c 662e 6164 6174 612e  " in self.adata.
+00002500: 6f62 736d 2c0d 0a20 2020 2020 2020 2020  obsm,..         
+00002510: 2020 2022 636e 6d66 5f67 6570 5f73 636f     "cnmf_gep_sco
+00002520: 7265 2220 696e 2073 656c 662e 6164 6174  re" in self.adat
+00002530: 612e 7661 726d 2c0d 0a20 2020 2020 2020  a.varm,..       
+00002540: 2020 2020 2022 636e 6d66 5f67 6570 5f74       "cnmf_gep_t
+00002550: 706d 2220 696e 2073 656c 662e 6164 6174  pm" in self.adat
+00002560: 612e 7661 726d 2c0d 0a20 2020 2020 2020  a.varm,..       
+00002570: 2020 2020 2022 636e 6d66 5f67 6570 5f72       "cnmf_gep_r
+00002580: 6177 2220 696e 2073 656c 662e 6164 6174  aw" in self.adat
+00002590: 612e 7661 726d 2c0d 0a20 2020 2020 2020  a.varm,..       
+000025a0: 2020 2020 2022 6b76 616c 7322 2069 6e20       "kvals" in 
+000025b0: 7365 6c66 2e61 6461 7461 2e75 6e73 0d0a  self.adata.uns..
+000025c0: 2020 2020 2020 2020 5d0d 0a20 2020 2020          ]..     
+000025d0: 2020 2072 6574 7572 6e20 616c 6c28 6d61     return all(ma
+000025e0: 7472 6978 5f63 6865 636b 7329 0d0a 2020  trix_checks)..  
+000025f0: 2020 2020 2020 0d0a 2020 2020 4070 726f        ..    @pro
+00002600: 7065 7274 790d 0a20 2020 2064 6566 206f  perty..    def o
+00002610: 7665 7264 6973 7065 7273 6564 5f67 656e  verdispersed_gen
+00002620: 6573 2873 656c 6629 3a0d 0a20 2020 2020  es(self):..     
+00002630: 2020 2022 2222 4f76 6572 6469 7370 6572     """Overdisper
+00002640: 7365 6420 6765 6e65 206c 6973 7420 7573  sed gene list us
+00002650: 6564 2066 6f72 2063 4e4d 460d 0a0d 0a20  ed for cNMF.... 
+00002660: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00002670: 6765 6e65 206c 6973 740d 0a20 2020 2020  gene list..     
+00002680: 2020 203a 7274 7970 653a 206c 6973 740d     :rtype: list.
+00002690: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+000026a0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000026b0: 662e 6164 6174 612e 756e 735b 2267 656e  f.adata.uns["gen
+000026c0: 655f 6c69 7374 225d 0d0a 0d0a 0d0a 2020  e_list"]......  
+000026d0: 2020 4063 6e6d 6673 6e73 5f76 6572 7369    @cnmfsns_versi
+000026e0: 6f6e 2e73 6574 7465 720d 0a20 2020 2064  on.setter..    d
+000026f0: 6566 2063 6e6d 6673 6e73 5f76 6572 7369  ef cnmfsns_versi
+00002700: 6f6e 2873 656c 662c 2076 616c 7565 3a20  on(self, value: 
+00002710: 626f 6f6c 293a 0d0a 2020 2020 2020 2020  bool):..        
+00002720: 7365 6c66 2e61 6461 7461 2e75 6e73 5b22  self.adata.uns["
+00002730: 636e 6d66 736e 735f 7665 7273 696f 6e22  cnmfsns_version"
+00002740: 5d20 3d20 7661 6c75 650d 0a0d 0a20 2020  ] = value....   
+00002750: 2020 2020 200d 0a20 2020 2064 6566 2075       ..    def u
+00002760: 7064 6174 655f 6f62 7328 7365 6c66 2c20  pdate_obs(self, 
+00002770: 6f62 7329 3a0d 0a20 2020 2020 2020 2022  obs):..        "
+00002780: 2222 5570 6461 7465 2074 6865 206f 6273  ""Update the obs
+00002790: 6572 7661 7469 6f6e 206d 6574 6164 6174  ervation metadat
+000027a0: 6120 7769 7468 2061 206e 6577 206d 6574  a with a new met
+000027b0: 6164 6174 6120 6d61 7472 6978 0d0a 0d0a  adata matrix....
+000027c0: 2020 2020 2020 2020 3a70 6172 616d 206f          :param o
+000027d0: 6273 3a20 416e 206f 6273 6572 7661 7469  bs: An observati
+000027e0: 6f6e 7320 c397 206d 6574 6164 6174 6120  ons .. metadata 
+000027f0: 6d61 7472 6978 2c20 6465 6661 756c 7473  matrix, defaults
+00002800: 2074 6f20 4e6f 6e65 0d0a 2020 2020 2020   to None..      
+00002810: 2020 3a74 7970 6520 6f62 733a 2060 7064    :type obs: `pd
+00002820: 2e44 6174 6146 7261 6d65 602c 206f 7074  .DataFrame`, opt
+00002830: 696f 6e61 6c0d 0a20 2020 2020 2020 2022  ional..        "
+00002840: 2222 0d0a 2020 2020 2020 2020 2320 636f  ""..        # co
+00002850: 6e76 6572 7420 276f 626a 6563 7427 2064  nvert 'object' d
+00002860: 7479 7065 2074 6f20 6361 7465 676f 7269  type to categori
+00002870: 6361 6c2c 2063 6f6e 7665 7274 696e 6720  cal, converting 
+00002880: 626f 6f6c 2076 616c 7565 7320 746f 2073  bool values to s
+00002890: 7472 696e 6773 2061 7320 7468 6573 6520  trings as these 
+000028a0: 6172 6520 6e6f 7420 7375 7070 6f72 7465  are not supporte
+000028b0: 6420 6279 2041 6e6e 4461 7461 206f 6e2d  d by AnnData on-
+000028c0: 6469 736b 2066 6f72 6d61 740d 0a20 2020  disk format..   
+000028d0: 2020 2020 2066 6f72 2063 6f6c 2069 6e20       for col in 
+000028e0: 6f62 732e 7365 6c65 6374 5f64 7479 7065  obs.select_dtype
+000028f0: 7328 696e 636c 7564 653d 226f 626a 6563  s(include="objec
+00002900: 7422 292e 636f 6c75 6d6e 733a 0d0a 2020  t").columns:..  
+00002910: 2020 2020 2020 2020 2020 6f62 735b 636f            obs[co
+00002920: 6c5d 203d 206f 6273 5b63 6f6c 5d2e 7265  l] = obs[col].re
+00002930: 706c 6163 6528 7b54 7275 653a 2022 5472  place({True: "Tr
+00002940: 7565 222c 2046 616c 7365 3a20 2246 616c  ue", False: "Fal
+00002950: 7365 227d 292e 6173 7479 7065 2822 6361  se"}).astype("ca
+00002960: 7465 676f 7279 2229 0d0a 2020 2020 2020  tegory")..      
+00002970: 2020 6d69 7373 696e 675f 7361 6d70 6c65    missing_sample
+00002980: 735f 696e 5f58 203d 206f 6273 2e69 6e64  s_in_X = obs.ind
+00002990: 6578 2e64 6966 6665 7265 6e63 6528 7365  ex.difference(se
+000029a0: 6c66 2e61 6461 7461 2e6f 6273 2e69 6e64  lf.adata.obs.ind
+000029b0: 6578 292e 6173 7479 7065 2873 7472 292e  ex).astype(str).
+000029c0: 746f 5f6c 6973 7428 290d 0a20 2020 2020  to_list()..     
+000029d0: 2020 2069 6620 6d69 7373 696e 675f 7361     if missing_sa
+000029e0: 6d70 6c65 735f 696e 5f58 3a0d 0a20 2020  mples_in_X:..   
+000029f0: 2020 2020 2020 2020 206c 6f67 6769 6e67           logging
+00002a00: 2e77 6172 6e69 6e67 2822 5468 6520 666f  .warning("The fo
+00002a10: 6c6c 6f77 696e 6720 7361 6d70 6c65 7320  llowing samples 
+00002a20: 696e 2074 6865 206d 6574 6164 6174 6120  in the metadata 
+00002a30: 7765 7265 206e 6f74 2070 7265 7365 6e74  were not present
+00002a40: 2069 6e20 7468 6520 6461 7461 2028 6061   in the data (`a
+00002a50: 6461 7461 2e58 6029 3a5c 6e20 202d 2022  data.X`):\n  - "
+00002a60: 202b 2022 5c6e 2020 2d20 222e 6a6f 696e   + "\n  - ".join
+00002a70: 286d 6973 7369 6e67 5f73 616d 706c 6573  (missing_samples
+00002a80: 5f69 6e5f 5829 290d 0a20 2020 2020 2020  _in_X))..       
+00002a90: 206d 6973 7369 6e67 5f73 616d 706c 6573   missing_samples
+00002aa0: 5f69 6e5f 6d64 203d 2073 656c 662e 6164  _in_md = self.ad
+00002ab0: 6174 612e 6f62 732e 696e 6465 782e 6469  ata.obs.index.di
+00002ac0: 6666 6572 656e 6365 286f 6273 2e69 6e64  fference(obs.ind
+00002ad0: 6578 292e 6173 7479 7065 2873 7472 292e  ex).astype(str).
+00002ae0: 746f 5f6c 6973 7428 290d 0a20 2020 2020  to_list()..     
+00002af0: 2020 2069 6620 6d69 7373 696e 675f 7361     if missing_sa
+00002b00: 6d70 6c65 735f 696e 5f6d 643a 0d0a 2020  mples_in_md:..  
+00002b10: 2020 2020 2020 2020 2020 6c6f 6767 696e            loggin
+00002b20: 672e 7761 726e 696e 6728 2254 6865 2066  g.warning("The f
+00002b30: 6f6c 6c6f 7769 6e67 2073 616d 706c 6573  ollowing samples
+00002b40: 2069 6e20 7468 6520 6461 7461 2028 6061   in the data (`a
+00002b50: 6461 7461 2e58 6029 2077 6572 6520 6162  data.X`) were ab
+00002b60: 7365 6e74 2069 6e20 7468 6520 6d65 7461  sent in the meta
+00002b70: 6461 7461 3a5c 6e20 202d 2022 202b 2022  data:\n  - " + "
+00002b80: 5c6e 2020 2d20 222e 6a6f 696e 286d 6973  \n  - ".join(mis
+00002b90: 7369 6e67 5f73 616d 706c 6573 5f69 6e5f  sing_samples_in_
+00002ba0: 6d64 2929 0d0a 2020 2020 2020 2020 7365  md))..        se
+00002bb0: 6c66 2e61 6461 7461 2e6f 6273 203d 206f  lf.adata.obs = o
+00002bc0: 6273 2e72 6569 6e64 6578 2873 656c 662e  bs.reindex(self.
+00002bd0: 6164 6174 612e 6f62 732e 696e 6465 7829  adata.obs.index)
+00002be0: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
+00002bf0: 6765 745f 6d65 7461 6461 7461 5f74 7970  get_metadata_typ
+00002c00: 655f 7375 6d6d 6172 7928 7365 6c66 293a  e_summary(self):
+00002c10: 0d0a 2020 2020 2020 2020 2222 2252 6574  ..        """Ret
+00002c20: 7572 6e20 6120 7072 696e 7461 626c 6520  urn a printable 
+00002c30: 7375 6d6d 6172 7920 6f66 206d 6574 6164  summary of metad
+00002c40: 6174 6120 616e 6420 7661 6c75 6520 7479  ata and value ty
+00002c50: 7065 7320 666f 7220 6561 6368 206d 6574  pes for each met
+00002c60: 6164 6174 6120 6c61 7965 722e 0d0a 0d0a  adata layer.....
+00002c70: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00002c80: 2053 756d 6d61 7279 206f 6620 6d65 7461   Summary of meta
+00002c90: 6461 7461 0d0a 2020 2020 2020 2020 3a72  data..        :r
+00002ca0: 7479 7065 3a20 7374 720d 0a20 2020 2020  type: str..     
+00002cb0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00002cc0: 6d73 6720 3d20 2222 0d0a 2020 2020 2020  msg = ""..      
+00002cd0: 2020 666f 7220 636f 6c20 696e 2073 656c    for col in sel
+00002ce0: 662e 6164 6174 612e 6f62 732e 636f 6c75  f.adata.obs.colu
+00002cf0: 6d6e 733a 0d0a 2020 2020 2020 2020 2020  mns:..          
+00002d00: 2020 6d73 6720 2b3d 2022 2020 2020 436f    msg += "    Co
+00002d10: 6c75 6d6e 3a20 2220 2b20 636f 6c20 2b20  lumn: " + col + 
+00002d20: 225c 6e22 0d0a 2020 2020 2020 2020 2020  "\n"..          
+00002d30: 2020 666f 7220 7661 6c75 655f 7479 7065    for value_type
+00002d40: 2c20 636f 756e 7420 696e 2073 656c 662e  , count in self.
+00002d50: 6164 6174 612e 6f62 735b 636f 6c5d 2e64  adata.obs[col].d
+00002d60: 726f 706e 6128 292e 6d61 7028 7479 7065  ropna().map(type
+00002d70: 292e 7661 6c75 655f 636f 756e 7473 2829  ).value_counts()
+00002d80: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
+00002d90: 2020 2020 2020 2020 2020 206d 7367 202b             msg +
+00002da0: 3d20 6622 2020 2020 2020 2020 7b76 616c  = f"        {val
+00002db0: 7565 5f74 7970 657d 3a20 7b63 6f75 6e74  ue_type}: {count
+00002dc0: 7d5c 6e22 0d0a 2020 2020 2020 2020 7265  }\n"..        re
+00002dd0: 7475 726e 206d 7367 0d0a 2020 2020 0d0a  turn msg..    ..
+00002de0: 2020 2020 6465 6620 7772 6974 655f 6835      def write_h5
+00002df0: 6164 2873 656c 662c 0d0a 2020 2020 2020  ad(self,..      
+00002e00: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+00002e10: 656e 616d 653a 2073 7472 293a 0d0a 2020  ename: str):..  
+00002e20: 2020 2020 2020 2222 2257 7269 7465 2064        """Write d
+00002e30: 6174 6173 6574 2074 6f20 2e68 3561 6420  ataset to .h5ad 
+00002e40: 6669 6c65 2e0d 0a0d 0a20 2020 2020 2020  file.....       
+00002e50: 203a 7061 7261 6d20 6669 6c65 6e61 6d65   :param filename
+00002e60: 3a20 6669 6c65 7061 7468 0d0a 2020 2020  : filepath..    
+00002e70: 2020 2020 3a74 7970 6520 6669 6c65 6e61      :type filena
+00002e80: 6d65 3a20 7374 720d 0a20 2020 2020 2020  me: str..       
+00002e90: 2022 2222 0d0a 2020 2020 2020 2020 6669   """..        fi
+00002ea0: 6c65 6e61 6d65 203d 206f 732e 7061 7468  lename = os.path
+00002eb0: 2e61 6273 7061 7468 2866 696c 656e 616d  .abspath(filenam
+00002ec0: 6529 0d0a 2020 2020 2020 2020 6c6f 6767  e)..        logg
+00002ed0: 696e 672e 696e 666f 2866 2257 7269 7469  ing.info(f"Writi
+00002ee0: 6e67 2074 6f20 7b66 696c 656e 616d 657d  ng to {filename}
+00002ef0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00002f00: 2e61 6461 7461 2e77 7269 7465 5f68 3561  .adata.write_h5a
+00002f10: 6428 6669 6c65 6e61 6d65 290d 0a20 2020  d(filename)..   
+00002f20: 2020 2020 206c 6f67 6769 6e67 2e69 6e66       logging.inf
+00002f30: 6f28 6622 446f 6e65 2229 0d0a 2020 2020  o(f"Done")..    
+00002f40: 0d0a 2020 2020 6465 6620 746f 5f64 6628  ..    def to_df(
+00002f50: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
+00002f60: 2020 2020 206e 6f72 6d61 6c69 7a65 643a       normalized:
+00002f70: 2062 6f6f 6c20 3d20 4661 6c73 6529 3a0d   bool = False):.
+00002f80: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
+00002f90: 6461 7461 206d 6174 7269 7820 6173 2061  data matrix as a
+00002fa0: 2060 7064 2e44 6174 6146 7261 6d65 600d   `pd.DataFrame`.
+00002fb0: 0a0d 0a20 2020 2020 2020 203a 7061 7261  ...        :para
+00002fc0: 6d20 6e6f 726d 616c 697a 6564 3a20 5365  m normalized: Se
+00002fd0: 7420 7472 7565 2066 6f72 2054 504d 206e  t true for TPM n
+00002fe0: 6f72 6d61 6c69 7a65 6420 6f75 7470 7574  ormalized output
+00002ff0: 2c20 6465 6661 756c 7473 2074 6f20 4661  , defaults to Fa
+00003000: 6c73 650d 0a20 2020 2020 2020 203a 7479  lse..        :ty
+00003010: 7065 206e 6f72 6d61 6c69 7a65 643a 2062  pe normalized: b
+00003020: 6f6f 6c2c 206f 7074 696f 6e61 6c0d 0a20  ool, optional.. 
+00003030: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00003040: 6f62 7365 7276 6174 696f 6e73 20c3 9720  observations .. 
+00003050: 7661 7269 6162 6c65 7320 6461 7461 206d  variables data m
+00003060: 6174 7269 780d 0a20 2020 2020 2020 203a  atrix..        :
+00003070: 7274 7970 653a 2070 642e 4461 7461 4672  rtype: pd.DataFr
+00003080: 616d 650d 0a20 2020 2020 2020 2022 2222  ame..        """
+00003090: 0d0a 2020 2020 2020 2020 6466 203d 2073  ..        df = s
+000030a0: 656c 662e 6164 6174 612e 746f 5f64 6628  elf.adata.to_df(
+000030b0: 290d 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
+000030c0: 726d 616c 697a 6564 2061 6e64 206e 6f74  rmalized and not
+000030d0: 2073 656c 662e 6973 5f6e 6f72 6d61 6c69   self.is_normali
+000030e0: 7a65 643a 0d0a 2020 2020 2020 2020 2020  zed:..          
+000030f0: 2020 6466 203d 2064 662e 6469 7628 6466    df = df.div(df
+00003100: 2e73 756d 2861 7869 733d 3129 2c20 6178  .sum(axis=1), ax
+00003110: 6973 3d30 2920 2a20 3165 3620 2023 2054  is=0) * 1e6  # T
+00003120: 504d 206e 6f72 6d61 6c69 7a61 7469 6f6e  PM normalization
+00003130: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00003140: 2064 660d 0a20 2020 2020 2020 200d 0a20   df..        .. 
+00003150: 2020 2064 6566 2072 656d 6f76 655f 756e     def remove_un
+00003160: 6661 6374 6f72 697a 6162 6c65 5f67 656e  factorizable_gen
+00003170: 6573 2873 656c 6629 3a0d 0a20 2020 2020  es(self):..     
+00003180: 2020 2022 2222 5265 6d6f 7665 7320 6765     """Removes ge
+00003190: 6e65 7320 7769 7468 206d 6973 7369 6e67  nes with missing
+000031a0: 2076 616c 7565 7320 6f72 207a 6572 6f20   values or zero 
+000031b0: 7661 7269 616e 6365 2066 726f 6d20 7468  variance from th
+000031c0: 6520 6461 7461 206d 6174 7269 782e 0d0a  e data matrix...
+000031d0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+000031e0: 2020 2020 2064 6620 3d20 7365 6c66 2e74       df = self.t
+000031f0: 6f5f 6466 286e 6f72 6d61 6c69 7a65 643d  o_df(normalized=
+00003200: 4661 6c73 6529 0d0a 2020 2020 2020 2020  False)..        
+00003210: 2320 4368 6563 6b20 666f 7220 7661 7269  # Check for vari
+00003220: 6162 6c65 7320 7769 7468 206d 6973 7369  ables with missi
+00003230: 6e67 2076 616c 7565 730d 0a20 2020 2020  ng values..     
+00003240: 2020 2067 656e 6573 5f77 6974 685f 6d69     genes_with_mi
+00003250: 7373 696e 6776 616c 7565 7320 3d20 6466  ssingvalues = df
+00003260: 2e69 736e 756c 6c28 292e 616e 7928 290d  .isnull().any().
+00003270: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00003280: 2020 2069 6620 6765 6e65 735f 7769 7468     if genes_with
+00003290: 5f6d 6973 7369 6e67 7661 6c75 6573 2e61  _missingvalues.a
+000032a0: 6e79 2829 3a0d 0a20 2020 2020 2020 2020  ny():..         
+000032b0: 2020 206e 5f6d 6973 7369 6e67 203d 2067     n_missing = g
+000032c0: 656e 6573 5f77 6974 685f 6d69 7373 696e  enes_with_missin
+000032d0: 6776 616c 7565 732e 7375 6d28 290d 0a20  gvalues.sum().. 
+000032e0: 2020 2020 2020 2020 2020 206c 6f67 6769             loggi
+000032f0: 6e67 2e77 6172 6e69 6e67 2866 227b 6e5f  ng.warning(f"{n_
+00003300: 6d69 7373 696e 677d 206f 6620 7b73 656c  missing} of {sel
+00003310: 662e 6164 6174 612e 6e5f 7661 7273 7d20  f.adata.n_vars} 
+00003320: 7661 7269 6162 6c65 7320 6172 6520 6d69  variables are mi
+00003330: 7373 696e 6720 7661 6c75 6573 2028 6061  ssing values (`a
+00003340: 6461 7461 2e58 6029 2e22 290d 0a20 2020  data.X`).")..   
+00003350: 2020 2020 2020 2020 206c 6f67 6769 6e67           logging
+00003360: 2e77 6172 6e69 6e67 2866 2253 7562 7365  .warning(f"Subse
+00003370: 7474 696e 6720 7661 7269 6162 6c65 7320  tting variables 
+00003380: 746f 2074 686f 7365 2077 6974 6820 6e6f  to those with no
+00003390: 206d 6973 7369 6e67 2076 616c 7565 732e   missing values.
+000033a0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+000033b0: 2020 2020 0d0a 2020 2020 2020 2020 2320      ..        # 
+000033c0: 4368 6563 6b20 666f 7220 6765 6e65 7320  Check for genes 
+000033d0: 7769 7468 207a 6572 6f20 7661 7269 616e  with zero varian
+000033e0: 6365 0d0a 2020 2020 2020 2020 7a65 726f  ce..        zero
+000033f0: 7661 7267 656e 6573 203d 2028 6466 2e76  vargenes = (df.v
+00003400: 6172 2829 203d 3d20 3029 0d0a 2020 2020  ar() == 0)..    
+00003410: 2020 2020 6966 207a 6572 6f76 6172 6765      if zerovarge
+00003420: 6e65 732e 616e 7928 293a 0d0a 2020 2020  nes.any():..    
+00003430: 2020 2020 2020 2020 6e5f 7a65 726f 7661          n_zerova
+00003440: 7220 3d20 7a65 726f 7661 7267 656e 6573  r = zerovargenes
+00003450: 2e73 756d 2829 0d0a 2020 2020 2020 2020  .sum()..        
+00003460: 2020 2020 6c6f 6767 696e 672e 7761 726e      logging.warn
+00003470: 696e 6728 6622 7b6e 5f7a 6572 6f76 6172  ing(f"{n_zerovar
+00003480: 7d20 6f66 207b 7365 6c66 2e61 6461 7461  } of {self.adata
+00003490: 2e6e 5f76 6172 737d 2076 6172 6961 626c  .n_vars} variabl
+000034a0: 6573 2068 6176 6520 6120 7661 7269 616e  es have a varian
+000034b0: 6365 206f 6620 7a65 726f 2069 6e20 636f  ce of zero in co
+000034c0: 756e 7473 2064 6174 6120 2860 6164 6174  unts data (`adat
+000034d0: 612e 7261 772e 5860 292e 2229 0d0a 2020  a.raw.X`).")..  
+000034e0: 2020 2020 2020 2020 2020 6c6f 6767 696e            loggin
+000034f0: 672e 7761 726e 696e 6728 6622 5375 6273  g.warning(f"Subs
+00003500: 6574 7469 6e67 2076 6172 6961 626c 6573  etting variables
+00003510: 2074 6f20 7468 6f73 6520 7769 7468 206e   to those with n
+00003520: 6f6e 7a65 726f 2076 6172 6961 6e63 652e  onzero variance.
+00003530: 2229 0d0a 2020 2020 2020 2020 0d0a 2020  ")..        ..  
+00003540: 2020 2020 2020 6765 6e65 735f 746f 5f6b        genes_to_k
+00003550: 6565 7020 3d20 287e 6765 6e65 735f 7769  eep = (~genes_wi
+00003560: 7468 5f6d 6973 7369 6e67 7661 6c75 6573  th_missingvalues
+00003570: 2920 2620 287e 7a65 726f 7661 7267 656e  ) & (~zerovargen
+00003580: 6573 290d 0a20 2020 2020 2020 200d 0a20  es)..        .. 
+00003590: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
+000035a0: 6120 3d20 7365 6c66 2e61 6461 7461 5b3a  a = self.adata[:
+000035b0: 2c67 656e 6573 5f74 6f5f 6b65 6570 5d0d  ,genes_to_keep].
+000035c0: 0a0d 0a20 2020 2064 6566 2063 6f6d 7075  ...    def compu
+000035d0: 7465 5f67 656e 655f 7374 6174 7328 7365  te_gene_stats(se
+000035e0: 6c66 2c20 6f64 675f 6465 6661 756c 745f  lf, odg_default_
+000035f0: 7370 6c69 6e65 5f64 6567 7265 653a 2069  spline_degree: i
+00003600: 6e74 203d 2033 2c20 6f64 675f 6465 6661  nt = 3, odg_defa
+00003610: 756c 745f 646f 663a 2069 6e74 203d 2038  ult_dof: int = 8
+00003620: 293a 0d0a 2020 2020 2020 2020 2222 220d  ):..        """.
+00003630: 0a20 2020 2020 2020 2043 6f6d 7075 7465  .        Compute
+00003640: 7320 6765 6e65 2073 7461 7469 7374 6963  s gene statistic
+00003650: 7320 616e 6420 6669 7473 2074 776f 206d  s and fits two m
+00003660: 6f64 656c 7320 6f66 206d 6561 6e20 616e  odels of mean an
+00003670: 6420 7661 7269 616e 6365 206f 6620 6765  d variance of ge
+00003680: 6e65 7320 696e 2074 6865 2064 6174 6173  nes in the datas
+00003690: 6574 2e20 5468 6520 6669 7273 7420 6d65  et. The first me
+000036a0: 7468 6f64 2069 7320 7468 650d 0a20 2020  thod is the..   
+000036b0: 2020 2020 2067 656e 6572 616c 697a 6564       generalized
+000036c0: 2061 6464 6974 6976 6520 6d6f 6465 6c20   additive model 
+000036d0: 7769 7468 2073 6d6f 6f74 6820 636f 6d70  with smooth comp
+000036e0: 6f6e 656e 7473 2028 422d 7370 6c69 6e65  onents (B-spline
+000036f0: 7329 2074 6f20 6d6f 6465 6c20 7468 6520  s) to model the 
+00003700: 7265 6c61 7469 6f6e 7368 6970 206f 6620  relationship of 
+00003710: 6d65 616e 2061 6e64 2076 6172 6961 6e63  mean and varianc
+00003720: 650d 0a20 2020 2020 2020 2062 6574 7765  e..        betwe
+00003730: 656e 2067 656e 6573 2069 6e20 7468 6520  en genes in the 
+00003740: 6461 7461 7365 742e 2049 7420 7072 6f64  dataset. It prod
+00003750: 7563 6573 2061 6e20 6f64 7363 6f72 6520  uces an odscore 
+00003760: 6d65 7472 6963 2066 6f72 206f 7665 7264  metric for overd
+00003770: 6973 7065 7273 696f 6e2e 2054 6865 2073  ispersion. The s
+00003780: 6563 6f6e 6420 6973 2074 6865 2063 6f75  econd is the cou
+00003790: 6e74 2d73 7461 7469 7374 6963 730d 0a20  nt-statistics.. 
+000037a0: 2020 2020 2020 206d 6574 686f 6420 666f         method fo
+000037b0: 756e 6420 696e 2074 6865 2063 4e4d 4620  und in the cNMF 
+000037c0: 7061 636b 6167 652c 2077 6869 6368 2070  package, which p
+000037d0: 726f 6475 6365 7320 6120 6d6f 6469 6669  roduces a modifi
+000037e0: 6564 2076 2d73 636f 7265 206d 6574 7269  ed v-score metri
+000037f0: 632e 2041 6c6c 2067 656e 6520 7374 6174  c. All gene stat
+00003800: 6973 7469 6373 2061 7265 2073 746f 7265  istics are store
+00003810: 6420 7769 7468 696e 2074 6865 0d0a 2020  d within the..  
+00003820: 2020 2020 2020 6461 7461 7365 7420 6f62        dataset ob
+00003830: 6a65 6374 2061 6e64 2061 7265 2061 6363  ject and are acc
+00003840: 6573 7369 626c 6520 7573 696e 6720 6064  essible using `d
+00003850: 6174 6173 6574 2e61 6e6e 6461 7461 2e76  ataset.anndata.v
+00003860: 6172 602e 0d0a 0d0a 2020 2020 2020 2020  ar`.....        
+00003870: 3a70 6172 616d 206f 6467 5f64 6566 6175  :param odg_defau
+00003880: 6c74 5f73 706c 696e 655f 6465 6772 6565  lt_spline_degree
+00003890: 3a20 422d 5370 6c69 6e65 2064 6567 7265  : B-Spline degre
+000038a0: 6520 666f 7220 474c 4d2d 4741 4d20 6d6f  e for GLM-GAM mo
+000038b0: 6465 6c6c 696e 6720 6f66 206d 6561 6e2d  delling of mean-
+000038c0: 7661 7269 616e 6365 2072 656c 6174 696f  variance relatio
+000038d0: 6e73 6869 702c 2064 6566 6175 6c74 7320  nship, defaults 
+000038e0: 746f 2033 0d0a 2020 2020 2020 2020 3a74  to 3..        :t
+000038f0: 7970 6520 6f64 675f 6465 6661 756c 745f  ype odg_default_
+00003900: 7370 6c69 6e65 5f64 6567 7265 653a 2069  spline_degree: i
+00003910: 6e74 2c20 6f70 7469 6f6e 616c 0d0a 2020  nt, optional..  
+00003920: 2020 2020 2020 3a70 6172 616d 206f 6467        :param odg
+00003930: 5f64 6566 6175 6c74 5f64 6f66 3a20 4465  _default_dof: De
+00003940: 6772 6565 7320 6f66 2066 7265 6564 6f6d  grees of freedom
+00003950: 2066 6f72 2047 4c4d 2d47 414d 206d 6f64   for GLM-GAM mod
+00003960: 656c 6c69 6e67 206f 6620 6d65 616e 2d76  elling of mean-v
+00003970: 6172 616e 6365 2c20 6465 6661 756c 7473  arance, defaults
+00003980: 2074 6f20 380d 0a20 2020 2020 2020 203a   to 8..        :
+00003990: 7479 7065 206f 6467 5f64 6566 6175 6c74  type odg_default
+000039a0: 5f64 6f66 3a20 696e 742c 206f 7074 696f  _dof: int, optio
+000039b0: 6e61 6c0d 0a20 2020 2020 2020 2022 2222  nal..        """
+000039c0: 0d0a 2020 2020 2020 2020 6461 7461 5f72  ..        data_r
+000039d0: 6177 203d 2073 656c 662e 746f 5f64 6628  aw = self.to_df(
+000039e0: 290d 0a20 2020 2020 2020 2064 6174 615f  )..        data_
+000039f0: 6e6f 726d 616c 697a 6564 203d 2073 656c  normalized = sel
+00003a00: 662e 746f 5f64 6628 6e6f 726d 616c 697a  f.to_df(normaliz
+00003a10: 6564 3d54 7275 6529 0d0a 2020 2020 2020  ed=True)..      
+00003a20: 2020 0d0a 2020 2020 2020 2020 2320 6372    ..        # cr
+00003a30: 6561 7465 2064 6174 6166 7261 6d65 206f  eate dataframe o
+00003a40: 6620 7065 722d 6765 6e65 2073 7461 7469  f per-gene stati
+00003a50: 7374 6963 730d 0a20 2020 2020 2020 2073  stics..        s
+00003a60: 656c 662e 6164 6174 612e 7661 725b 226d  elf.adata.var["m
+00003a70: 6561 6e22 5d20 3d20 6461 7461 5f6e 6f72  ean"] = data_nor
+00003a80: 6d61 6c69 7a65 642e 6d65 616e 2829 0d0a  malized.mean()..
+00003a90: 2020 2020 2020 2020 7365 6c66 2e61 6461          self.ada
+00003aa0: 7461 2e76 6172 5b22 7261 6e6b 5f6d 6561  ta.var["rank_mea
+00003ab0: 6e22 5d20 3d20 7365 6c66 2e61 6461 7461  n"] = self.adata
+00003ac0: 2e76 6172 5b22 6d65 616e 225d 2e72 616e  .var["mean"].ran
+00003ad0: 6b28 290d 0a20 2020 2020 2020 2073 656c  k()..        sel
+00003ae0: 662e 6164 6174 612e 7661 725b 2276 6172  f.adata.var["var
+00003af0: 6961 6e63 6522 5d20 3d20 6461 7461 5f6e  iance"] = data_n
+00003b00: 6f72 6d61 6c69 7a65 642e 7661 7228 290d  ormalized.var().
+00003b10: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
+00003b20: 6174 612e 7661 725b 2273 6422 5d20 3d20  ata.var["sd"] = 
+00003b30: 6461 7461 5f6e 6f72 6d61 6c69 7a65 642e  data_normalized.
+00003b40: 7374 6428 290d 0a20 2020 2020 2020 2073  std()..        s
+00003b50: 656c 662e 6164 6174 612e 7661 725b 226d  elf.adata.var["m
+00003b60: 6973 7369 6e67 6e65 7373 225d 203d 2064  issingness"] = d
+00003b70: 6174 615f 6e6f 726d 616c 697a 6564 2e69  ata_normalized.i
+00003b80: 736e 756c 6c28 292e 7375 6d28 2920 2f20  snull().sum() / 
+00003b90: 6461 7461 5f6e 6f72 6d61 6c69 7a65 642e  data_normalized.
+00003ba0: 7368 6170 655b 305d 0d0a 2020 2020 2020  shape[0]..      
+00003bb0: 2020 7365 6c66 2e61 6461 7461 2e76 6172    self.adata.var
+00003bc0: 5b5b 226c 6f67 5f6d 6561 6e22 2c20 226c  [["log_mean", "l
+00003bd0: 6f67 5f76 6172 6961 6e63 6522 5d5d 203d  og_variance"]] =
+00003be0: 206e 702e 6c6f 6731 3028 7365 6c66 2e61   np.log10(self.a
+00003bf0: 6461 7461 2e76 6172 5b5b 226d 6561 6e22  data.var[["mean"
+00003c00: 2c20 2276 6172 6961 6e63 6522 5d5d 290d  , "variance"]]).
+00003c10: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
+00003c20: 6174 612e 7661 725b 226d 6561 6e5f 636f  ata.var["mean_co
+00003c30: 756e 7473 225d 203d 2064 6174 615f 7261  unts"] = data_ra
+00003c40: 772e 6d65 616e 2829 0d0a 2020 2020 2020  w.mean()..      
+00003c50: 2020 7365 6c66 2e61 6461 7461 2e76 6172    self.adata.var
+00003c60: 5b22 6f64 7363 6f72 655f 6578 636c 7564  ["odscore_exclud
+00003c70: 6564 225d 203d 2028 2873 656c 662e 6164  ed"] = ((self.ad
+00003c80: 6174 612e 7661 725b 226d 6973 7369 6e67  ata.var["missing
+00003c90: 6e65 7373 225d 203e 2030 2920 7c0d 0a20  ness"] > 0) |.. 
+00003ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003cc0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00003cd0: 662e 6164 6174 612e 7661 725b 226c 6f67  f.adata.var["log
+00003ce0: 5f6d 6561 6e22 5d2e 6973 6e75 6c6c 2829  _mean"].isnull()
+00003cf0: 207c 0d0a 2020 2020 2020 2020 2020 2020   |..            
+00003d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d20: 2020 2873 656c 662e 6164 6174 612e 7661    (self.adata.va
+00003d30: 725b 226d 6561 6e22 5d20 3d3d 2030 2920  r["mean"] == 0) 
+00003d40: 7c0d 0a20 2020 2020 2020 2020 2020 2020  |..             
+00003d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d70: 2073 656c 662e 6164 6174 612e 7661 725b   self.adata.var[
+00003d80: 226c 6f67 5f76 6172 6961 6e63 6522 5d2e  "log_variance"].
+00003d90: 6973 6e75 6c6c 2829 290d 0a0d 0a20 2020  isnull())....   
+00003da0: 2020 2020 2023 206d 6f64 656c 206d 6561       # model mea
+00003db0: 6e2d 7661 7269 616e 6365 2072 656c 6174  n-variance relat
+00003dc0: 696f 6e73 6869 7020 7573 696e 6720 6765  ionship using ge
+00003dd0: 6e65 7261 6c69 7a65 6420 6164 6469 7469  neralized additi
+00003de0: 7665 206d 6f64 656c 2077 6974 6820 736d  ve model with sm
+00003df0: 6f6f 7468 2063 6f6d 706f 6e65 6e74 730d  ooth components.
+00003e00: 0a20 2020 2020 2020 2064 665f 6d6f 6465  .        df_mode
+00003e10: 6c20 3d20 7365 6c66 2e61 6461 7461 2e76  l = self.adata.v
+00003e20: 6172 5b7e 7365 6c66 2e61 6461 7461 2e76  ar[~self.adata.v
+00003e30: 6172 5b22 6f64 7363 6f72 655f 6578 636c  ar["odscore_excl
+00003e40: 7564 6564 225d 5d0d 0a20 2020 2020 2020  uded"]]..       
+00003e50: 2062 7320 3d20 4253 706c 696e 6573 2864   bs = BSplines(d
+00003e60: 665f 6d6f 6465 6c5b 226d 6561 6e22 5d2c  f_model["mean"],
+00003e70: 2064 663d 6f64 675f 6465 6661 756c 745f   df=odg_default_
+00003e80: 646f 662c 2064 6567 7265 653d 6f64 675f  dof, degree=odg_
+00003e90: 6465 6661 756c 745f 7370 6c69 6e65 5f64  default_spline_d
+00003ea0: 6567 7265 6529 0d0a 2020 2020 2020 2020  egree)..        
+00003eb0: 6761 6d20 3d20 474c 4d47 616d 2e66 726f  gam = GLMGam.fro
+00003ec0: 6d5f 666f 726d 756c 6128 226c 6f67 5f76  m_formula("log_v
+00003ed0: 6172 6961 6e63 6520 7e20 6c6f 675f 6d65  ariance ~ log_me
+00003ee0: 616e 222c 2064 6174 613d 6466 5f6d 6f64  an", data=df_mod
+00003ef0: 656c 2c20 736d 6f6f 7468 6572 3d62 7329  el, smoother=bs)
+00003f00: 2e66 6974 2829 0d0a 2020 2020 2020 2020  .fit()..        
+00003f10: 7365 6c66 2e61 6461 7461 2e76 6172 5b22  self.adata.var["
+00003f20: 7265 7369 645f 6c6f 675f 7661 7269 616e  resid_log_varian
+00003f30: 6365 225d 203d 2067 616d 2e72 6573 6964  ce"] = gam.resid
+00003f40: 5f72 6573 706f 6e73 650d 0a20 2020 2020  _response..     
+00003f50: 2020 2073 656c 662e 6164 6174 612e 7661     self.adata.va
+00003f60: 725b 226f 6473 636f 7265 225d 203d 206e  r["odscore"] = n
+00003f70: 702e 7371 7274 2831 3020 2a2a 2073 656c  p.sqrt(10 ** sel
+00003f80: 662e 6164 6174 612e 7661 725b 2272 6573  f.adata.var["res
+00003f90: 6964 5f6c 6f67 5f76 6172 6961 6e63 6522  id_log_variance"
+00003fa0: 5d29 0d0a 2020 2020 2020 2020 7365 6c66  ])..        self
+00003fb0: 2e61 6461 7461 2e76 6172 5b22 6761 6d5f  .adata.var["gam_
+00003fc0: 6669 7474 6564 7661 6c75 6573 225d 203d  fittedvalues"] =
+00003fd0: 2067 616d 2e66 6974 7465 6476 616c 7565   gam.fittedvalue
+00003fe0: 730d 0a0d 0a0d 0a20 2020 2020 2020 2023  s......        #
+00003ff0: 206d 6f64 656c 206d 6561 6e2d 7661 7269   model mean-vari
+00004000: 616e 6365 2072 656c 6174 696f 6e73 6869  ance relationshi
+00004010: 7020 7573 696e 6720 634e 4d46 2773 206d  p using cNMF's m
+00004020: 6574 686f 6420 6261 7365 6420 6f6e 2076  ethod based on v
+00004030: 2d73 636f 7265 2061 6e64 206d 696e 696d  -score and minim
+00004040: 756d 2065 7870 7265 7373 696f 6e20 7468  um expression th
+00004050: 7265 7368 6f6c 640d 0a20 2020 2020 2020  reshold..       
+00004060: 2076 7363 6f72 655f 7374 6174 7320 3d20   vscore_stats = 
+00004070: 7064 2e44 6174 6146 7261 6d65 2863 6e6d  pd.DataFrame(cnm
+00004080: 662e 6765 745f 6869 6768 7661 725f 6765  f.get_highvar_ge
+00004090: 6e65 7328 696e 7075 745f 636f 756e 7473  nes(input_counts
+000040a0: 3d64 6174 615f 6e6f 726d 616c 697a 6564  =data_normalized
+000040b0: 2e76 616c 7565 732c 206d 696e 696d 616c  .values, minimal
+000040c0: 5f6d 6561 6e3d 3029 5b30 5d29 0d0a 2020  _mean=0)[0])..  
+000040d0: 2020 2020 2020 7673 636f 7265 5f73 7461        vscore_sta
+000040e0: 7473 2e69 6e64 6578 203d 2064 6174 615f  ts.index = data_
+000040f0: 6e6f 726d 616c 697a 6564 2e63 6f6c 756d  normalized.colum
+00004100: 6e73 0d0a 2020 2020 2020 2020 7365 6c66  ns..        self
+00004110: 2e61 6461 7461 2e76 6172 5b22 7673 636f  .adata.var["vsco
+00004120: 7265 225d 203d 2076 7363 6f72 655f 7374  re"] = vscore_st
+00004130: 6174 735b 2266 616e 6f5f 7261 7469 6f22  ats["fano_ratio"
+00004140: 5d0d 0a20 2020 2020 2020 2073 656c 662e  ]..        self.
+00004150: 6164 6174 612e 756e 735b 226f 6467 225d  adata.uns["odg"]
+00004160: 5b22 6f64 675f 6465 6661 756c 745f 7370  ["odg_default_sp
+00004170: 6c69 6e65 5f64 6567 7265 6522 5d20 3d20  line_degree"] = 
+00004180: 6f64 675f 6465 6661 756c 745f 7370 6c69  odg_default_spli
+00004190: 6e65 5f64 6567 7265 650d 0a20 2020 2020  ne_degree..     
+000041a0: 2020 2073 656c 662e 6164 6174 612e 756e     self.adata.un
+000041b0: 735b 226f 6467 225d 5b22 6f64 675f 6465  s["odg"]["odg_de
+000041c0: 6661 756c 745f 646f 6622 5d20 3d20 6f64  fault_dof"] = od
+000041d0: 675f 6465 6661 756c 745f 646f 660d 0a20  g_default_dof.. 
+000041e0: 2020 2020 2020 2073 656c 662e 6170 7065         self.appe
+000041f0: 6e64 5f74 6f5f 6869 7374 6f72 7928 2247  nd_to_history("G
+00004200: 656e 652d 6c65 7665 6c20 7374 6174 6973  ene-level statis
+00004210: 7469 6373 2061 6e64 206f 7665 7264 6973  tics and overdis
+00004220: 7065 7273 696f 6e20 6d6f 6465 6c6c 696e  persion modellin
+00004230: 6720 636f 6d70 6c65 7465 642e 2229 0d0a  g completed.")..
+00004240: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
+00004250: 6620 7365 6c65 6374 5f6f 7665 7264 6973  f select_overdis
+00004260: 7065 7273 6564 5f67 656e 6573 5f66 726f  persed_genes_fro
+00004270: 6d5f 6765 6e65 6c69 7374 2873 656c 662c  m_genelist(self,
+00004280: 2067 656e 6573 3a20 436f 6c6c 6563 7469   genes: Collecti
+00004290: 6f6e 2c20 6d69 6e5f 6d65 616e 3d30 293a  on, min_mean=0):
+000042a0: 0d0a 2020 2020 2020 2020 2222 2253 656c  ..        """Sel
+000042b0: 6563 7420 6f76 6572 6469 7370 6572 7365  ect overdisperse
+000042c0: 6420 6765 6e65 732f 6665 6174 7572 6573  d genes/features
+000042d0: 2075 7369 6e67 2061 2063 7573 746f 6d20   using a custom 
+000042e0: 6c69 7374 2e20 4765 6e65 732f 6665 6174  list. Genes/feat
+000042f0: 7572 6573 206e 6f74 2070 7265 7365 6e74  ures not present
+00004300: 2069 6e20 7468 6520 6461 7461 7365 7420   in the dataset 
+00004310: 6172 6520 6175 746f 6d61 7469 6361 6c6c  are automaticall
+00004320: 7920 6669 6c74 6572 6564 206f 7574 2e0d  y filtered out..
+00004330: 0a0d 0a20 2020 2020 2020 203a 7061 7261  ...        :para
+00004340: 6d20 6765 6e65 733a 2067 656e 6520 6c69  m genes: gene li
+00004350: 7374 0d0a 2020 2020 2020 2020 3a74 7970  st..        :typ
+00004360: 6520 6765 6e65 733a 2043 6f6c 6c65 6374  e genes: Collect
+00004370: 696f 6e0d 0a20 2020 2020 2020 203a 7061  ion..        :pa
+00004380: 7261 6d20 6d69 6e5f 6d65 616e 3a20 6d69  ram min_mean: mi
+00004390: 6e69 6d75 6d20 6765 6e65 2065 7870 7265  nimum gene expre
+000043a0: 7373 696f 6e20 666f 7220 6765 6e65 7320  ssion for genes 
+000043b0: 746f 2062 6520 636f 756e 7465 6420 6173  to be counted as
+000043c0: 206f 7665 7264 6973 7065 7273 6564 2c20   overdispersed, 
+000043d0: 6465 6661 756c 7473 2074 6f20 300d 0a20  defaults to 0.. 
+000043e0: 2020 2020 2020 203a 7479 7065 206d 696e         :type min
+000043f0: 5f6d 6561 6e3a 2069 6e74 2c20 6f70 7469  _mean: int, opti
+00004400: 6f6e 616c 0d0a 2020 2020 2020 2020 2222  onal..        ""
+00004410: 220d 0a20 2020 2020 2020 2073 656c 662e  "..        self.
+00004420: 6164 6174 612e 7661 725b 2273 656c 6563  adata.var["selec
+00004430: 7465 6422 5d20 3d20 7365 6c66 2e61 6461  ted"] = self.ada
+00004440: 7461 2e76 6172 2e69 6e64 6578 2e69 7369  ta.var.index.isi
+00004450: 6e28 6765 6e65 7329 2026 2073 656c 662e  n(genes) & self.
+00004460: 6164 6174 612e 7661 725b 226d 6561 6e5f  adata.var["mean_
+00004470: 636f 756e 7473 225d 203e 3d20 6d69 6e5f  counts"] >= min_
+00004480: 6d65 616e 0d0a 2020 2020 2020 2020 7365  mean..        se
+00004490: 6c66 2e61 6461 7461 2e75 6e73 5b22 6f64  lf.adata.uns["od
+000044a0: 6722 5d5b 226f 7665 7264 6973 7065 7273  g"]["overdispers
+000044b0: 696f 6e5f 6d65 7472 6963 225d 203d 2022  ion_metric"] = "
+000044c0: 220d 0a20 2020 2020 2020 2073 656c 662e  "..        self.
+000044d0: 6164 6174 612e 756e 735b 226f 6467 225d  adata.uns["odg"]
+000044e0: 5b22 6d69 6e5f 6d65 616e 225d 203d 206d  ["min_mean"] = m
+000044f0: 696e 5f6d 6561 6e0d 0a20 2020 2020 2020  in_mean..       
+00004500: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
+00004510: 226f 6467 225d 5b22 6d69 6e5f 7363 6f72  "odg"]["min_scor
+00004520: 6522 5d20 3d20 2222 0d0a 2020 2020 2020  e"] = ""..      
+00004530: 2020 7365 6c66 2e61 6461 7461 2e75 6e73    self.adata.uns
+00004540: 5b22 6f64 6722 5d5b 2274 6f70 5f6e 225d  ["odg"]["top_n"]
+00004550: 203d 2022 220d 0a20 2020 2020 2020 2073   = ""..        s
+00004560: 656c 662e 6164 6174 612e 756e 735b 226f  elf.adata.uns["o
+00004570: 6467 225d 5b22 7175 616e 7469 6c65 225d  dg"]["quantile"]
+00004580: 203d 2022 220d 0a20 2020 2020 2020 2073   = ""..        s
+00004590: 656c 662e 6170 7065 6e64 5f74 6f5f 6869  elf.append_to_hi
+000045a0: 7374 6f72 7928 224f 7665 7264 6973 7065  story("Overdispe
+000045b0: 7273 6564 2067 656e 6573 2073 656c 6563  rsed genes selec
+000045c0: 7465 6420 6672 6f6d 2063 7573 746f 6d20  ted from custom 
+000045d0: 6765 6e65 206c 6973 7422 290d 0a20 2020  gene list")..   
+000045e0: 2020 2020 200d 0a20 2020 2064 6566 2073       ..    def s
+000045f0: 656c 6563 745f 6f76 6572 6469 7370 6572  elect_overdisper
+00004600: 7365 645f 6765 6e65 7328 7365 6c66 2c0d  sed_genes(self,.
+00004610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004630: 2020 2020 6f76 6572 6469 7370 6572 7369      overdispersi
+00004640: 6f6e 5f6d 6574 7269 633a 2073 7472 203d  on_metric: str =
+00004650: 2022 6f64 7363 6f72 6522 2c0d 0a20 2020   "odscore",..   
+00004660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004680: 6d69 6e5f 6d65 616e 3a20 666c 6f61 7420  min_mean: float 
+00004690: 3d20 302c 0d0a 2020 2020 2020 2020 2020  = 0,..          
+000046a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046b0: 2020 2020 2020 2020 206d 696e 5f73 636f           min_sco
+000046c0: 7265 3a20 666c 6f61 7420 3d20 312e 302c  re: float = 1.0,
+000046d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000046e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046f0: 2020 2020 2074 6f70 5f6e 3a20 696e 7420       top_n: int 
+00004700: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
+00004710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004720: 2020 2020 2020 2020 2020 2020 7175 616e              quan
+00004730: 7469 6c65 3a20 666c 6f61 7420 3d20 4e6f  tile: float = No
+00004740: 6e65 293a 0d0a 2020 2020 2020 2020 2222  ne):..        ""
+00004750: 2253 656c 6563 7420 6f76 6572 6469 7370  "Select overdisp
+00004760: 6572 7365 6420 6765 6e65 732f 6665 6174  ersed genes/feat
+00004770: 7572 6573 2075 7369 6e67 2061 6e20 6f76  ures using an ov
+00004780: 6572 6469 7370 6572 7369 6f6e 206d 6574  erdispersion met
+00004790: 7269 632e 204f 7074 696f 6e61 6c6c 7920  ric. Optionally 
+000047a0: 7365 7420 6120 6d69 6e69 6d75 6d20 6765  set a minimum ge
+000047b0: 6e65 2065 7870 7265 7373 696f 6e20 6c65  ne expression le
+000047c0: 7665 6c2e 0d0a 2020 2020 2020 2020 5365  vel...        Se
+000047d0: 7420 6120 7468 7265 7368 6f6c 6420 7573  t a threshold us
+000047e0: 696e 6720 7468 6520 746f 7020 4e20 2827  ing the top N ('
+000047f0: 746f 705f 6e27 292c 206d 696e 696d 756d  top_n'), minimum
+00004800: 2073 636f 7265 2028 276d 696e 5f73 636f   score ('min_sco
+00004810: 7265 2729 2c20 6f72 2070 726f 706f 7274  re'), or proport
+00004820: 696f 6e20 6f66 2066 6561 7475 7265 7320  ion of features 
+00004830: 2827 7175 616e 7469 6c65 2729 206d 6574  ('quantile') met
+00004840: 686f 6473 2e0d 0a20 2020 2020 2020 204f  hods...        O
+00004850: 7665 7264 6973 7065 7273 6564 2067 656e  verdispersed gen
+00004860: 6520 6c69 7374 2069 7320 7361 7665 6420  e list is saved 
+00004870: 696e 2074 6865 2044 6174 6173 6574 206f  in the Dataset o
+00004880: 626a 6563 742e 0d0a 0d0a 2020 2020 2020  bject.....      
+00004890: 2020 3a70 6172 616d 206f 7665 7264 6973    :param overdis
+000048a0: 7065 7273 696f 6e5f 6d65 7472 6963 3a20  persion_metric: 
+000048b0: 226f 6473 636f 7265 2220 6f72 2022 7673  "odscore" or "vs
+000048c0: 636f 7265 222c 2064 6566 6175 6c74 7320  core", defaults 
+000048d0: 746f 2022 6f64 7363 6f72 6522 0d0a 2020  to "odscore"..  
+000048e0: 2020 2020 2020 3a74 7970 6520 6f76 6572        :type over
+000048f0: 6469 7370 6572 7369 6f6e 5f6d 6574 7269  dispersion_metri
+00004900: 633a 2073 7472 2c20 6f70 7469 6f6e 616c  c: str, optional
+00004910: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+00004920: 206d 696e 5f6d 6561 6e3a 206d 696e 696d   min_mean: minim
+00004930: 756d 2067 656e 6520 6578 7072 6573 7369  um gene expressi
+00004940: 6f6e 2066 6f72 2067 656e 6573 2074 6f20  on for genes to 
+00004950: 6265 2063 6f75 6e74 6564 2061 7320 6f76  be counted as ov
+00004960: 6572 6469 7370 6572 7365 642c 2064 6566  erdispersed, def
+00004970: 6175 6c74 7320 746f 2030 0d0a 2020 2020  aults to 0..    
+00004980: 2020 2020 3a74 7970 6520 6d69 6e5f 6d65      :type min_me
+00004990: 616e 3a20 696e 742c 206f 7074 696f 6e61  an: int, optiona
+000049a0: 6c0d 0a20 2020 2020 2020 203a 7061 7261  l..        :para
+000049b0: 6d20 6d69 6e5f 7363 6f72 653a 206d 696e  m min_score: min
+000049c0: 696d 756d 2073 636f 7265 2066 6f72 206f  imum score for o
+000049d0: 7665 7264 6973 7065 7273 696f 6e2c 2064  verdispersion, d
+000049e0: 6566 6175 6c74 7320 746f 2031 2e30 0d0a  efaults to 1.0..
+000049f0: 2020 2020 2020 2020 3a74 7970 6520 6d69          :type mi
+00004a00: 6e5f 7363 6f72 653a 2066 6c6f 6174 2c20  n_score: float, 
+00004a10: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
+00004a20: 2020 3a70 6172 616d 2074 6f70 5f6e 3a20    :param top_n: 
+00004a30: 4368 6f6f 7365 2074 6865 2074 6f70 204e  Choose the top N
+00004a40: 206d 6f73 7420 6f76 6572 6469 7370 6572   most overdisper
+00004a50: 7365 6420 6765 6e65 732c 2064 6566 6175  sed genes, defau
+00004a60: 6c74 7320 746f 204e 6f6e 650d 0a20 2020  lts to None..   
+00004a70: 2020 2020 203a 7479 7065 2074 6f70 5f6e       :type top_n
+00004a80: 3a20 696e 742c 206f 7074 696f 6e61 6c0d  : int, optional.
+00004a90: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00004aa0: 7175 616e 7469 6c65 3a20 4368 6f6f 7365  quantile: Choose
+00004ab0: 2061 2071 7561 6e74 696c 6520 6f66 206f   a quantile of o
+00004ac0: 7665 7264 6973 7065 7273 696f 6e2e 2046  verdispersion. F
+00004ad0: 6f72 2065 7861 6d70 6c65 2c20 7468 6520  or example, the 
+00004ae0: 746f 7020 3130 2520 6f66 206f 7665 7264  top 10% of overd
+00004af0: 6973 7065 7273 6564 2067 656e 6573 2077  ispersed genes w
+00004b00: 6f75 6c64 2062 6520 302e 3130 2e20 4465  ould be 0.10. De
+00004b10: 6661 756c 7473 2074 6f20 4e6f 6e65 0d0a  faults to None..
+00004b20: 2020 2020 2020 2020 3a74 7970 6520 7175          :type qu
+00004b30: 616e 7469 6c65 3a20 666c 6f61 742c 206f  antile: float, o
+00004b40: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
+00004b50: 203a 7261 6973 6573 2056 616c 7565 4572   :raises ValueEr
+00004b60: 726f 723a 2045 7272 6f72 2069 6620 696e  ror: Error if in
+00004b70: 7661 6c69 6420 6f76 6572 6469 7370 6572  valid overdisper
+00004b80: 7369 6f6e 206d 6574 7269 6320 6973 2063  sion metric is c
+00004b90: 686f 7365 6e2e 0d0a 2020 2020 2020 2020  hosen...        
+00004ba0: 2222 220d 0a20 2020 2020 2020 200d 0a20  """..        .. 
+00004bb0: 2020 2020 2020 2069 6620 6f76 6572 6469         if overdi
+00004bc0: 7370 6572 7369 6f6e 5f6d 6574 7269 6320  spersion_metric 
+00004bd0: 6e6f 7420 696e 2073 656c 662e 6164 6174  not in self.adat
+00004be0: 612e 7661 722e 636f 6c75 6d6e 733a 0d0a  a.var.columns:..
+00004bf0: 2020 2020 2020 2020 2020 2020 6966 206f              if o
+00004c00: 7665 7264 6973 7065 7273 696f 6e5f 6d65  verdispersion_me
+00004c10: 7472 6963 2069 6e20 2822 6f64 7363 6f72  tric in ("odscor
+00004c20: 6522 2c20 2276 7363 6f72 6522 293a 0d0a  e", "vscore"):..
+00004c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c40: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00004c50: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00004c60: 2020 2020 2020 2066 227b 6f76 6572 6469         f"{overdi
+00004c70: 7370 6572 7369 6f6e 5f6d 6574 7269 637d  spersion_metric}
+00004c80: 2068 6173 206e 6f74 2062 6565 6e20 6361   has not been ca
+00004c90: 6c63 756c 6174 6564 2066 6f72 2074 6869  lculated for thi
+00004ca0: 7320 6461 7461 7365 742e 2022 0d0a 2020  s dataset. "..  
+00004cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cc0: 2020 2245 6e73 7572 6520 7468 6174 2079    "Ensure that y
+00004cd0: 6f75 2063 616c 6c20 7468 6520 6044 6174  ou call the `Dat
+00004ce0: 6173 6574 2e63 6f6d 7075 7465 5f67 656e  aset.compute_gen
+00004cf0: 655f 7374 6174 7328 2960 2066 6972 7374  e_stats()` first
+00004d00: 2e22 0d0a 2020 2020 2020 2020 2020 2020  ."..            
+00004d10: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+00004d20: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00004d30: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00004d40: 6973 6520 5661 6c75 6545 7272 6f72 280d  ise ValueError(.
+00004d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004d60: 2020 2020 2066 227b 6f76 6572 6469 7370       f"{overdisp
+00004d70: 6572 7369 6f6e 5f6d 6574 7269 637d 2069  ersion_metric} i
+00004d80: 7320 6e6f 7420 6120 7661 6c69 6420 6f76  s not a valid ov
+00004d90: 6572 6469 7370 6572 7369 6f6e 206d 6574  erdispersion met
+00004da0: 7269 632e 220d 0a20 2020 2020 2020 2020  ric."..         
+00004db0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+00004dc0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00004dd0: 2320 7761 726e 2069 6620 6d75 6c74 6970  # warn if multip
+00004de0: 6c65 206d 6574 686f 6473 2061 7265 2073  le methods are s
+00004df0: 656c 6563 7465 640d 0a20 2020 2020 2020  elected..       
+00004e00: 2073 656c 6563 7465 645f 6d65 7468 6f64   selected_method
+00004e10: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+00004e20: 6966 206d 696e 5f73 636f 7265 2069 7320  if min_score is 
+00004e30: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+00004e40: 2020 2020 2020 2073 656c 6563 7465 645f         selected_
+00004e50: 6d65 7468 6f64 732e 6170 7065 6e64 2822  methods.append("
+00004e60: 6d69 6e5f 7363 6f72 6522 290d 0a20 2020  min_score")..   
+00004e70: 2020 2020 2069 6620 746f 705f 6e20 6973       if top_n is
+00004e80: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+00004e90: 2020 2020 2020 2020 7365 6c65 6374 6564          selected
+00004ea0: 5f6d 6574 686f 6473 2e61 7070 656e 6428  _methods.append(
+00004eb0: 2274 6f70 5f6e 2229 0d0a 2020 2020 2020  "top_n")..      
+00004ec0: 2020 6966 2071 7561 6e74 696c 6520 6973    if quantile is
 00004ed0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-00004ee0: 2020 2020 2020 2020 6765 6e65 7320 3d20          genes = 
-00004ef0: 7365 6c66 2e61 6461 7461 2e76 6172 5b6f  self.adata.var[o
-00004f00: 7665 7264 6973 7065 7273 696f 6e5f 6d65  verdispersion_me
-00004f10: 7472 6963 5d2e 736f 7274 5f76 616c 7565  tric].sort_value
-00004f20: 7328 6173 6365 6e64 696e 673d 4661 6c73  s(ascending=Fals
-00004f30: 6529 2e68 6561 6428 696e 7428 746f 705f  e).head(int(top_
-00004f40: 6e29 292e 696e 6465 780d 0a20 2020 2020  n)).index..     
-00004f50: 2020 2020 2020 2073 656c 6563 7465 645f         selected_
-00004f60: 6765 6e65 7320 3d20 7365 6c65 6374 6564  genes = selected
-00004f70: 5f67 656e 6573 2026 2073 656c 662e 6164  _genes & self.ad
-00004f80: 6174 612e 7661 722e 696e 6465 782e 6973  ata.var.index.is
-00004f90: 696e 2867 656e 6573 290d 0a20 2020 2020  in(genes)..     
-00004fa0: 2020 2023 2071 7561 6e74 696c 6520 6669     # quantile fi
-00004fb0: 6c74 6572 0d0a 2020 2020 2020 2020 6966  lter..        if
-00004fc0: 2071 7561 6e74 696c 6520 6973 206e 6f74   quantile is not
-00004fd0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00004fe0: 2020 2020 6e5f 746f 7461 6c5f 6765 6e65      n_total_gene
-00004ff0: 7320 3d20 7365 6c66 2e61 6461 7461 2e76  s = self.adata.v
-00005000: 6172 5b6f 7665 7264 6973 7065 7273 696f  ar[overdispersio
-00005010: 6e5f 6d65 7472 6963 5d2e 6e6f 746e 756c  n_metric].notnul
-00005020: 6c28 292e 7375 6d28 290d 0a20 2020 2020  l().sum()..     
-00005030: 2020 2020 2020 2067 656e 6573 203d 2073         genes = s
-00005040: 656c 662e 6164 6174 612e 7661 725b 6f76  elf.adata.var[ov
-00005050: 6572 6469 7370 6572 7369 6f6e 5f6d 6574  erdispersion_met
-00005060: 7269 635d 2e73 6f72 745f 7661 6c75 6573  ric].sort_values
-00005070: 2861 7363 656e 6469 6e67 3d46 616c 7365  (ascending=False
-00005080: 292e 6865 6164 2869 6e74 2871 7561 6e74  ).head(int(quant
-00005090: 696c 6520 2a20 6e5f 746f 7461 6c5f 6765  ile * n_total_ge
-000050a0: 6e65 7329 292e 696e 6465 780d 0a20 2020  nes)).index..   
-000050b0: 2020 2020 2020 2020 2073 656c 6563 7465           selecte
-000050c0: 645f 6765 6e65 7320 3d20 7365 6c65 6374  d_genes = select
-000050d0: 6564 5f67 656e 6573 2026 2073 656c 662e  ed_genes & self.
-000050e0: 6164 6174 612e 7661 722e 696e 6465 782e  adata.var.index.
-000050f0: 6973 696e 2867 656e 6573 290d 0a0d 0a20  isin(genes).... 
-00005100: 2020 2020 2020 206e 5f73 656c 6563 7465         n_selecte
-00005110: 645f 6765 6e65 7320 3d20 7365 6c65 6374  d_genes = select
-00005120: 6564 5f67 656e 6573 2e73 756d 2829 0d0a  ed_genes.sum()..
-00005130: 2020 2020 2020 2020 6c6f 6767 696e 672e          logging.
-00005140: 696e 666f 2866 227b 6e5f 7365 6c65 6374  info(f"{n_select
-00005150: 6564 5f67 656e 6573 7d20 6765 6e65 7320  ed_genes} genes 
-00005160: 7365 6c65 6374 6564 2066 6f72 2066 6163  selected for fac
-00005170: 746f 7269 7a61 7469 6f6e 2229 0d0a 2020  torization")..  
-00005180: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00005190: 2320 6d61 6b65 2063 6861 6e67 6573 2074  # make changes t
-000051a0: 6f20 4461 7461 7365 7420 6f62 6a65 6374  o Dataset object
-000051b0: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-000051c0: 6461 7461 2e76 6172 5b22 7365 6c65 6374  data.var["select
-000051d0: 6564 225d 203d 2073 656c 6563 7465 645f  ed"] = selected_
-000051e0: 6765 6e65 730d 0a20 2020 2020 2020 2073  genes..        s
-000051f0: 656c 662e 6164 6174 612e 756e 735b 226f  elf.adata.uns["o
-00005200: 6467 225d 5b22 6f76 6572 6469 7370 6572  dg"]["overdisper
-00005210: 7369 6f6e 5f6d 6574 7269 6322 5d20 3d20  sion_metric"] = 
-00005220: 6f76 6572 6469 7370 6572 7369 6f6e 5f6d  overdispersion_m
-00005230: 6574 7269 630d 0a20 2020 2020 2020 2073  etric..        s
-00005240: 656c 662e 6164 6174 612e 756e 735b 226f  elf.adata.uns["o
-00005250: 6467 225d 5b22 6d69 6e5f 6d65 616e 225d  dg"]["min_mean"]
-00005260: 203d 206d 696e 5f6d 6561 6e0d 0a20 2020   = min_mean..   
-00005270: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
-00005280: 756e 735b 226f 6467 225d 5b22 6d69 6e5f  uns["odg"]["min_
-00005290: 7363 6f72 6522 5d20 3d20 6d69 6e5f 7363  score"] = min_sc
-000052a0: 6f72 6520 6966 206d 696e 5f73 636f 7265  ore if min_score
-000052b0: 2069 7320 6e6f 7420 4e6f 6e65 2065 6c73   is not None els
-000052c0: 6520 2222 0d0a 2020 2020 2020 2020 7365  e ""..        se
-000052d0: 6c66 2e61 6461 7461 2e75 6e73 5b22 6f64  lf.adata.uns["od
-000052e0: 6722 5d5b 2274 6f70 5f6e 225d 203d 2074  g"]["top_n"] = t
-000052f0: 6f70 5f6e 2069 6620 746f 705f 6e20 6973  op_n if top_n is
-00005300: 206e 6f74 204e 6f6e 6520 656c 7365 2022   not None else "
-00005310: 220d 0a20 2020 2020 2020 2073 656c 662e  "..        self.
-00005320: 6164 6174 612e 756e 735b 226f 6467 225d  adata.uns["odg"]
-00005330: 5b22 7175 616e 7469 6c65 225d 203d 2071  ["quantile"] = q
-00005340: 7561 6e74 696c 6520 6966 2071 7561 6e74  uantile if quant
-00005350: 696c 6520 6973 206e 6f74 204e 6f6e 6520  ile is not None 
-00005360: 656c 7365 2022 220d 0a20 2020 2020 2020  else ""..       
-00005370: 2073 656c 662e 6170 7065 6e64 5f74 6f5f   self.append_to_
-00005380: 6869 7374 6f72 7928 224f 7665 7264 6973  history("Overdis
-00005390: 7065 7273 6564 2067 656e 6573 2073 656c  persed genes sel
-000053a0: 6563 7465 6422 290d 0a20 2020 200d 0a20  ected")..    .. 
-000053b0: 2020 2064 6566 2069 6e69 7469 616c 697a     def initializ
-000053c0: 655f 636e 6d66 2873 656c 662c 2063 6e6d  e_cnmf(self, cnm
-000053d0: 665f 6f75 7470 7574 5f64 6972 3a20 7374  f_output_dir: st
-000053e0: 722c 0d0a 2020 2020 2020 2020 2020 2020  r,..            
-000053f0: 2020 2020 2020 2020 2020 2020 636e 6d66              cnmf
-00005400: 5f6e 616d 653a 2073 7472 2c0d 0a20 2020  _name: str,..   
-00005410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005420: 2020 2020 206b 7661 6c73 3a20 436f 6c6c       kvals: Coll
-00005430: 6563 7469 6f6e 203d 2072 616e 6765 2832  ection = range(2
-00005440: 2c20 3631 292c 0d0a 2020 2020 2020 2020  , 61),..        
-00005450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005460: 6e5f 6974 6572 3a20 696e 7420 3d20 3230  n_iter: int = 20
-00005470: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
-00005480: 2020 2020 2020 2020 2020 2020 6265 7461              beta
-00005490: 5f6c 6f73 733a 2073 7472 203d 2022 6b75  _loss: str = "ku
-000054a0: 6c6c 6261 636b 2d6c 6569 626c 6572 222c  llback-leibler",
-000054b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000054c0: 2020 2020 2020 2020 2020 7365 6564 3a20            seed: 
-000054d0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-000054e0: 4e6f 6e65 2920 2d3e 2063 6e6d 662e 634e  None) -> cnmf.cN
-000054f0: 4d46 3a0d 0a20 2020 2020 2020 2022 2222  MF:..        """
-00005500: 496e 6974 6961 6c69 7a65 2061 2063 4e4d  Initialize a cNM
-00005510: 4620 7275 6e20 666f 7220 7375 6273 6571  F run for subseq
-00005520: 7565 6e74 2066 6163 746f 7269 7a61 7469  uent factorizati
-00005530: 6f6e 2e0d 0a0d 0a20 2020 2020 2020 203a  on.....        :
-00005540: 7061 7261 6d20 636e 6d66 5f6f 7574 7075  param cnmf_outpu
-00005550: 745f 6469 723a 204f 7574 7075 7420 6469  t_dir: Output di
-00005560: 7265 6374 6f72 7920 666f 7220 634e 4d46  rectory for cNMF
-00005570: 2072 6573 756c 7473 0d0a 2020 2020 2020   results..      
-00005580: 2020 3a74 7970 6520 636e 6d66 5f6f 7574    :type cnmf_out
-00005590: 7075 745f 6469 723a 2073 7472 0d0a 2020  put_dir: str..  
-000055a0: 2020 2020 2020 3a70 6172 616d 2063 6e6d        :param cnm
-000055b0: 665f 6e61 6d65 3a20 4e61 6d65 206f 6620  f_name: Name of 
-000055c0: 7468 6520 634e 4d46 2072 6573 756c 7473  the cNMF results
-000055d0: 2e20 4669 6c65 7320 7769 6c6c 2062 6520  . Files will be 
-000055e0: 6f75 7470 7574 2074 6f20 5b63 6e6d 665f  output to [cnmf_
-000055f0: 6f75 7470 7574 5f64 6972 5d2f 5b63 6e6d  output_dir]/[cnm
-00005600: 665f 6e61 6d65 5d2f 0d0a 2020 2020 2020  f_name]/..      
-00005610: 2020 3a74 7970 6520 636e 6d66 5f6e 616d    :type cnmf_nam
-00005620: 653a 2073 7472 0d0a 2020 2020 2020 2020  e: str..        
-00005630: 3a70 6172 616d 206b 7661 6c73 3a20 5261  :param kvals: Ra
-00005640: 6e6b 7320 666f 7220 634e 4d46 2066 6163  nks for cNMF fac
-00005650: 746f 7269 7a61 7469 6f6e 2c20 6465 6661  torization, defa
-00005660: 756c 7473 2074 6f20 7261 6e67 6528 322c  ults to range(2,
-00005670: 2036 3129 0d0a 2020 2020 2020 2020 3a74   61)..        :t
-00005680: 7970 6520 6b76 616c 733a 2043 6f6c 6c65  ype kvals: Colle
-00005690: 6374 696f 6e2c 206f 7074 696f 6e61 6c0d  ction, optional.
-000056a0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000056b0: 6e5f 6974 6572 3a20 4e75 6d62 6572 206f  n_iter: Number o
-000056c0: 6620 6974 6572 6174 696f 6e73 2066 726f  f iterations fro
-000056d0: 6d20 7768 6963 6820 746f 2062 7569 6c64  m which to build
-000056e0: 2061 2063 6f6e 7365 6e73 7573 2073 6f6c   a consensus sol
-000056f0: 7574 696f 6e2c 2064 6566 6175 6c74 7320  ution, defaults 
-00005700: 746f 2032 3030 0d0a 2020 2020 2020 2020  to 200..        
-00005710: 3a74 7970 6520 6e5f 6974 6572 3a20 696e  :type n_iter: in
-00005720: 742c 206f 7074 696f 6e61 6c0d 0a20 2020  t, optional..   
-00005730: 2020 2020 203a 7061 7261 6d20 6265 7461       :param beta
-00005740: 5f6c 6f73 733a 2062 6574 612d 6c6f 7373  _loss: beta-loss
-00005750: 2066 756e 6374 696f 6e2c 2065 6974 6865   function, eithe
-00005760: 7220 226b 756c 6c62 6163 6b2d 6c65 6962  r "kullback-leib
-00005770: 6c65 7222 206f 7220 2266 726f 6265 6e69  ler" or "frobeni
-00005780: 7573 222e 2044 6566 6175 6c74 7320 746f  us". Defaults to
-00005790: 2022 6b75 6c6c 6261 636b 2d6c 6569 626c   "kullback-leibl
-000057a0: 6572 220d 0a20 2020 2020 2020 203a 7479  er"..        :ty
-000057b0: 7065 2062 6574 615f 6c6f 7373 3a20 7374  pe beta_loss: st
-000057c0: 722c 206f 7074 696f 6e61 6c0d 0a20 2020  r, optional..   
-000057d0: 2020 2020 203a 7061 7261 6d20 7365 6564       :param seed
-000057e0: 3a20 5261 6e64 6f6d 2073 6565 6420 666f  : Random seed fo
-000057f0: 7220 7265 7072 6f64 7563 6962 696c 6974  r reproducibilit
-00005800: 792c 2064 6566 6175 6c74 7320 746f 204e  y, defaults to N
-00005810: 6f6e 650d 0a20 2020 2020 2020 203a 7479  one..        :ty
-00005820: 7065 2073 6565 643a 204f 7074 696f 6e61  pe seed: Optiona
-00005830: 6c5b 696e 745d 2c20 6f70 7469 6f6e 616c  l[int], optional
-00005840: 0d0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
-00005850: 6e3a 2063 4e4d 4620 6f62 6a65 6374 0d0a  n: cNMF object..
-00005860: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00005870: 3a63 6c61 7373 3a60 636e 6d66 736e 732e  :class:`cnmfsns.
-00005880: 636e 6d66 2e63 4e4d 4660 0d0a 2020 2020  cnmf.cNMF`..    
-00005890: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-000058a0: 2063 6e6d 665f 6f62 6a20 3d20 636e 6d66   cnmf_obj = cnmf
-000058b0: 2e63 4e4d 4628 6f75 7470 7574 5f64 6972  .cNMF(output_dir
-000058c0: 3d63 6e6d 665f 6f75 7470 7574 5f64 6972  =cnmf_output_dir
-000058d0: 2c20 6e61 6d65 3d63 6e6d 665f 6e61 6d65  , name=cnmf_name
-000058e0: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
-000058f0: 2020 2020 2023 2077 7269 7465 2054 504d       # write TPM
-00005900: 2028 6e6f 726d 616c 697a 6564 2920 6461   (normalized) da
-00005910: 7461 0d0a 2020 2020 2020 2020 7470 6d20  ta..        tpm 
-00005920: 3d20 6164 2e41 6e6e 4461 7461 2873 656c  = ad.AnnData(sel
-00005930: 662e 746f 5f64 6628 6e6f 726d 616c 697a  f.to_df(normaliz
-00005940: 6564 3d54 7275 6529 290d 0a20 2020 2020  ed=True))..     
-00005950: 2020 2074 706d 2e77 7269 7465 5f68 3561     tpm.write_h5a
-00005960: 6428 636e 6d66 5f6f 626a 2e70 6174 6873  d(cnmf_obj.paths
-00005970: 5b22 7470 6d22 5d29 0d0a 0d0a 2020 2020  ["tpm"])....    
-00005980: 2020 2020 6765 6e65 5f74 706d 5f6d 6561      gene_tpm_mea
-00005990: 6e20 3d20 6e70 2e61 7272 6179 2874 706d  n = np.array(tpm
-000059a0: 2e58 2e6d 6561 6e28 6178 6973 3d30 2929  .X.mean(axis=0))
-000059b0: 2e72 6573 6861 7065 282d 3129 0d0a 2020  .reshape(-1)..  
-000059c0: 2020 2020 2020 6765 6e65 5f74 706d 5f73        gene_tpm_s
-000059d0: 7464 6465 7620 3d20 6e70 2e61 7272 6179  tddev = np.array
-000059e0: 2874 706d 2e58 2e73 7464 2861 7869 733d  (tpm.X.std(axis=
-000059f0: 302c 2064 646f 663d 3029 292e 7265 7368  0, ddof=0)).resh
-00005a00: 6170 6528 2d31 290d 0a20 2020 2020 2020  ape(-1)..       
-00005a10: 2069 6e70 7574 5f74 706d 5f73 7461 7473   input_tpm_stats
-00005a20: 203d 2070 642e 4461 7461 4672 616d 6528   = pd.DataFrame(
-00005a30: 5b67 656e 655f 7470 6d5f 6d65 616e 2c20  [gene_tpm_mean, 
-00005a40: 6765 6e65 5f74 706d 5f73 7464 6465 765d  gene_tpm_stddev]
-00005a50: 2c20 696e 6465 7820 3d20 5b27 5f5f 6d65  , index = ['__me
-00005a60: 616e 272c 2027 5f5f 7374 6427 5d29 2e54  an', '__std']).T
-00005a70: 0d0a 2020 2020 2020 2020 7574 696c 732e  ..        utils.
-00005a80: 7361 7665 5f64 665f 746f 5f6e 707a 2869  save_df_to_npz(i
-00005a90: 6e70 7574 5f74 706d 5f73 7461 7473 2c20  nput_tpm_stats, 
-00005aa0: 636e 6d66 5f6f 626a 2e70 6174 6873 5b27  cnmf_obj.paths['
-00005ab0: 7470 6d5f 7374 6174 7327 5d29 0d0a 2020  tpm_stats'])..  
-00005ac0: 2020 2020 2020 6f76 6572 6469 7370 6572        overdisper
-00005ad0: 7365 645f 6765 6e65 7320 3d20 7365 6c66  sed_genes = self
-00005ae0: 2e61 6461 7461 2e76 6172 5b22 7365 6c65  .adata.var["sele
-00005af0: 6374 6564 225d 5b73 656c 662e 6164 6174  cted"][self.adat
-00005b00: 612e 7661 725b 2273 656c 6563 7465 6422  a.var["selected"
-00005b10: 5d5d 2e69 6e64 6578 0d0a 2020 2020 2020  ]].index..      
-00005b20: 2020 6e6f 726d 5f63 6f75 6e74 7320 3d20    norm_counts = 
-00005b30: 636e 6d66 5f6f 626a 2e67 6574 5f6e 6f72  cnmf_obj.get_nor
-00005b40: 6d5f 636f 756e 7473 2873 656c 662e 6164  m_counts(self.ad
-00005b50: 6174 612c 2074 706d 2c20 6869 6768 5f76  ata, tpm, high_v
-00005b60: 6172 6961 6e63 655f 6765 6e65 735f 6669  ariance_genes_fi
-00005b70: 6c74 6572 3d6f 7665 7264 6973 7065 7273  lter=overdispers
-00005b80: 6564 5f67 656e 6573 290d 0a20 2020 2020  ed_genes)..     
-00005b90: 2020 2069 6620 6e6f 726d 5f63 6f75 6e74     if norm_count
-00005ba0: 732e 582e 6474 7970 6520 213d 206e 702e  s.X.dtype != np.
-00005bb0: 666c 6f61 7436 343a 0d0a 2020 2020 2020  float64:..      
-00005bc0: 2020 2020 2020 6e6f 726d 5f63 6f75 6e74        norm_count
-00005bd0: 732e 5820 3d20 6e6f 726d 5f63 6f75 6e74  s.X = norm_count
-00005be0: 732e 582e 6173 7479 7065 286e 702e 666c  s.X.astype(np.fl
-00005bf0: 6f61 7436 3429 0d0a 2020 2020 2020 2020  oat64)..        
-00005c00: 636e 6d66 5f6f 626a 2e73 6176 655f 6e6f  cnmf_obj.save_no
-00005c10: 726d 5f63 6f75 6e74 7328 6e6f 726d 5f63  rm_counts(norm_c
-00005c20: 6f75 6e74 7329 0d0a 0d0a 2020 2020 2020  ounts)....      
-00005c30: 2020 2320 7361 7665 2070 6172 616d 6574    # save paramet
-00005c40: 6572 7320 666f 7220 6661 6374 6f72 697a  ers for factoriz
-00005c50: 6174 696f 6e20 7374 6570 0d0a 2020 2020  ation step..    
-00005c60: 2020 2020 636e 6d66 5f6f 626a 2e73 6176      cnmf_obj.sav
-00005c70: 655f 6e6d 665f 6974 6572 5f70 6172 616d  e_nmf_iter_param
-00005c80: 7328 2a63 6e6d 665f 6f62 6a2e 6765 745f  s(*cnmf_obj.get_
-00005c90: 6e6d 665f 6974 6572 5f70 6172 616d 7328  nmf_iter_params(
-00005ca0: 6b73 3d6b 7661 6c73 2c20 6e5f 6974 6572  ks=kvals, n_iter
-00005cb0: 3d6e 5f69 7465 722c 2072 616e 646f 6d5f  =n_iter, random_
-00005cc0: 7374 6174 655f 7365 6564 3d73 6565 642c  state_seed=seed,
-00005cd0: 2062 6574 615f 6c6f 7373 3d62 6574 615f   beta_loss=beta_
-00005ce0: 6c6f 7373 2929 0d0a 0d0a 2020 2020 2020  loss))....      
-00005cf0: 2020 2320 7361 7665 2070 6172 616d 6574    # save paramet
-00005d00: 6572 7320 696e 2041 6e6e 4461 7461 206f  ers in AnnData o
-00005d10: 626a 6563 740d 0a20 2020 2020 2020 2073  bject..        s
-00005d20: 656c 662e 6164 6174 612e 756e 735b 2263  elf.adata.uns["c
-00005d30: 6e6d 6622 5d20 3d20 636e 6d66 5f6f 626a  nmf"] = cnmf_obj
-00005d40: 2e67 6574 5f6e 6d66 5f69 7465 725f 7061  .get_nmf_iter_pa
-00005d50: 7261 6d73 286b 733d 6b76 616c 732c 206e  rams(ks=kvals, n
-00005d60: 5f69 7465 723d 6e5f 6974 6572 2c20 7261  _iter=n_iter, ra
-00005d70: 6e64 6f6d 5f73 7461 7465 5f73 6565 643d  ndom_state_seed=
-00005d80: 7365 6564 2c20 6265 7461 5f6c 6f73 733d  seed, beta_loss=
-00005d90: 6265 7461 5f6c 6f73 7329 5b31 5d20 2023  beta_loss)[1]  #
-00005da0: 2064 6963 7420 6f66 2063 6e6d 6620 7061   dict of cnmf pa
-00005db0: 7261 6d65 7465 7273 0d0a 2020 2020 2020  rameters..      
-00005dc0: 2020 0d0a 2020 2020 2020 2020 7365 6c66    ..        self
-00005dd0: 2e61 7070 656e 645f 746f 5f68 6973 746f  .append_to_histo
-00005de0: 7279 2866 2263 4e4d 4620 7061 7261 6d65  ry(f"cNMF parame
-00005df0: 7465 7273 2061 6464 6564 2e20 634e 4d46  ters added. cNMF
-00005e00: 2069 6e70 7574 7320 696e 6974 6961 6c69   inputs initiali
-00005e10: 7a65 6420 696e 207b 636e 6d66 5f6f 7574  zed in {cnmf_out
-00005e20: 7075 745f 6469 727d 2f7b 636e 6d66 5f6e  put_dir}/{cnmf_n
-00005e30: 616d 657d 2229 0d0a 2020 2020 2020 2020  ame}")..        
-00005e40: 7265 7475 726e 2063 6e6d 665f 6f62 6a0d  return cnmf_obj.
-00005e50: 0a20 2020 200d 0a20 2020 2064 6566 2061  .    ..    def a
-00005e60: 6464 5f63 6e6d 665f 7265 7375 6c74 7328  dd_cnmf_results(
-00005e70: 7365 6c66 2c20 636e 6d66 5f6f 7574 7075  self, cnmf_outpu
-00005e80: 745f 6469 722c 2063 6e6d 665f 6e61 6d65  t_dir, cnmf_name
-00005e90: 2c20 6c6f 6361 6c5f 6465 6e73 6974 795f  , local_density_
-00005ea0: 7468 7265 7368 6f6c 643a 2066 6c6f 6174  threshold: float
-00005eb0: 203d 204e 6f6e 652c 206c 6f63 616c 5f6e   = None, local_n
-00005ec0: 6569 6768 626f 7268 6f6f 645f 7369 7a65  eighborhood_size
-00005ed0: 3a20 666c 6f61 7420 3d20 4e6f 6e65 293a  : float = None):
-00005ee0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00005ef0: 2020 2020 2020 2041 6674 6572 2066 6163         After fac
-00005f00: 746f 7269 7a61 7469 6f6e 2c20 6164 6420  torization, add 
-00005f10: 636f 6d70 6c65 7465 6420 634e 4d46 2072  completed cNMF r
-00005f20: 6573 756c 7473 2069 6e20 5b63 6e6d 665f  esults in [cnmf_
-00005f30: 6f75 7470 7574 5f64 6972 5d2f 5b63 6e6d  output_dir]/[cnm
-00005f40: 665f 6e61 6d65 5d20 746f 2074 6865 2064  f_name] to the d
-00005f50: 6174 6173 6574 206f 626a 6563 742e 0d0a  ataset object...
-00005f60: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00005f70: 2063 6e6d 665f 6f75 7470 7574 5f64 6972   cnmf_output_dir
-00005f80: 3a20 4f75 7470 7574 2064 6972 6563 746f  : Output directo
-00005f90: 7279 2066 6f72 2063 4e4d 4620 7265 7375  ry for cNMF resu
-00005fa0: 6c74 730d 0a20 2020 2020 2020 203a 7479  lts..        :ty
-00005fb0: 7065 2063 6e6d 665f 6f75 7470 7574 5f64  pe cnmf_output_d
-00005fc0: 6972 3a20 7374 720d 0a20 2020 2020 2020  ir: str..       
-00005fd0: 203a 7061 7261 6d20 636e 6d66 5f6e 616d   :param cnmf_nam
-00005fe0: 653a 204e 616d 6520 6f66 2074 6865 2063  e: Name of the c
-00005ff0: 4e4d 4620 7265 7375 6c74 732e 2046 696c  NMF results. Fil
-00006000: 6573 2077 696c 6c20 6265 206f 7574 7075  es will be outpu
-00006010: 7420 746f 205b 636e 6d66 5f6f 7574 7075  t to [cnmf_outpu
-00006020: 745f 6469 725d 2f5b 636e 6d66 5f6e 616d  t_dir]/[cnmf_nam
-00006030: 655d 2f0d 0a20 2020 2020 2020 203a 7479  e]/..        :ty
-00006040: 7065 2063 6e6d 665f 6e61 6d65 3a20 7374  pe cnmf_name: st
-00006050: 720d 0a20 2020 2020 2020 203a 7061 7261  r..        :para
-00006060: 6d20 6c6f 6361 6c5f 6465 6e73 6974 795f  m local_density_
-00006070: 7468 7265 7368 6f6c 643a 2054 6872 6573  threshold: Thres
-00006080: 686f 6c64 2066 6f72 2074 6865 206c 6f63  hold for the loc
-00006090: 616c 2064 656e 7369 7479 2066 696c 7465  al density filte
-000060a0: 7269 6e67 2070 7269 6f72 2074 6f20 4745  ring prior to GE
-000060b0: 5020 636f 6e73 656e 7375 732e 2041 6363  P consensus. Acc
-000060c0: 6570 7461 626c 6520 7468 7265 7368 6f6c  eptable threshol
-000060d0: 6473 2061 7265 203e 2030 2061 6e64 203c  ds are > 0 and <
-000060e0: 3d20 3220 2832 2e30 2069 7320 6e6f 2066  = 2 (2.0 is no f
-000060f0: 696c 7465 7269 6e67 292e 2044 6566 6175  iltering). Defau
-00006100: 6c74 7320 746f 204e 6f6e 652e 0d0a 2020  lts to None...  
-00006110: 2020 2020 2020 3a74 7970 6520 6c6f 6361        :type loca
-00006120: 6c5f 6465 6e73 6974 795f 7468 7265 7368  l_density_thresh
-00006130: 6f6c 643a 2066 6c6f 6174 2c20 6f70 7469  old: float, opti
-00006140: 6f6e 616c 0d0a 2020 2020 2020 2020 3a70  onal..        :p
-00006150: 6172 616d 206c 6f63 616c 5f6e 6569 6768  aram local_neigh
-00006160: 626f 7268 6f6f 645f 7369 7a65 3a20 4672  borhood_size: Fr
-00006170: 6163 7469 6f6e 206f 6620 7468 6520 6e75  action of the nu
-00006180: 6d62 6572 206f 6620 7265 706c 6963 6174  mber of replicat
-00006190: 6573 2074 6f20 7573 6520 6173 206e 6561  es to use as nea
-000061a0: 7265 7374 206e 6569 6768 626f 7273 2066  rest neighbors f
-000061b0: 6f72 206c 6f63 616c 2064 656e 7369 7479  or local density
-000061c0: 2066 696c 7465 7269 6e67 2e20 4465 6661   filtering. Defa
-000061d0: 756c 7473 2074 6f20 4e6f 6e65 0d0a 2020  ults to None..  
-000061e0: 2020 2020 2020 3a74 7970 6520 6c6f 6361        :type loca
-000061f0: 6c5f 6e65 6967 6862 6f72 686f 6f64 5f73  l_neighborhood_s
-00006200: 697a 653a 2066 6c6f 6174 2c20 6f70 7469  ize: float, opti
-00006210: 6f6e 616c 0d0a 2020 2020 2020 2020 2222  onal..        ""
-00006220: 220d 0a20 2020 2020 2020 2073 656c 662e  "..        self.
-00006230: 6164 6174 612e 756e 735b 2263 6e6d 665f  adata.uns["cnmf_
-00006240: 6e61 6d65 225d 203d 2063 6e6d 665f 6e61  name"] = cnmf_na
-00006250: 6d65 0d0a 0d0a 2020 2020 2020 2020 2320  me....        # 
-00006260: 696e 6665 7220 6672 6f6d 2066 696c 656e  infer from filen
-00006270: 616d 6573 2077 6869 6368 206c 6f63 616c  ames which local
-00006280: 2064 656e 7369 7479 2074 6872 6573 686f   density thresho
-00006290: 6c64 2077 6173 2075 7365 640d 0a20 2020  ld was used..   
-000062a0: 2020 2020 2073 656e 7365 645f 6c64 7473       sensed_ldts
-000062b0: 203d 2073 6574 2829 0d0a 2020 2020 2020   = set()..      
-000062c0: 2020 666f 7220 666e 2069 6e20 676c 6f62    for fn in glob
-000062d0: 286f 732e 7061 7468 2e6a 6f69 6e28 636e  (os.path.join(cn
-000062e0: 6d66 5f6f 7574 7075 745f 6469 722c 2063  mf_output_dir, c
-000062f0: 6e6d 665f 6e61 6d65 2c20 6622 7b63 6e6d  nmf_name, f"{cnm
-00006300: 665f 6e61 6d65 7d2a 2e2a 7370 6563 7472  f_name}*.*spectr
-00006310: 612a 2e6b 5f2a 2229 293a 0d0a 2020 2020  a*.k_*")):..    
-00006320: 2020 2020 2020 2020 6c64 745f 7374 7220          ldt_str 
-00006330: 3d20 6f73 2e70 6174 682e 6261 7365 6e61  = os.path.basena
-00006340: 6d65 2866 6e29 2e73 706c 6974 2822 2e22  me(fn).split("."
-00006350: 295b 2d33 5d0d 0a20 2020 2020 2020 2020  )[-3]..         
-00006360: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-00006370: 2020 2020 2020 2020 206c 6474 203d 2066           ldt = f
-00006380: 6c6f 6174 286c 6474 5f73 7472 2e72 6570  loat(ldt_str.rep
-00006390: 6c61 6365 2822 6474 5f22 2c20 2222 292e  lace("dt_", "").
-000063a0: 7265 706c 6163 6528 225f 222c 2022 2e22  replace("_", "."
-000063b0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-000063c0: 6578 6365 7074 2056 616c 7565 4572 726f  except ValueErro
-000063d0: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
-000063e0: 2020 2020 7061 7373 0d0a 2020 2020 2020      pass..      
-000063f0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00006400: 2020 2020 2020 2020 2020 2020 2073 656e               sen
-00006410: 7365 645f 6c64 7473 2e61 6464 2828 6c64  sed_ldts.add((ld
-00006420: 745f 7374 722c 206c 6474 2929 0d0a 2020  t_str, ldt))..  
-00006430: 2020 2020 2020 6966 206c 6f63 616c 5f64        if local_d
-00006440: 656e 7369 7479 5f74 6872 6573 686f 6c64  ensity_threshold
-00006450: 2069 7320 4e6f 6e65 2061 6e64 206c 656e   is None and len
-00006460: 2873 656e 7365 645f 6c64 7473 2920 3d3d  (sensed_ldts) ==
-00006470: 2031 3a0d 0a20 2020 2020 2020 2020 2020   1:..           
-00006480: 206c 6474 5f73 7472 2c20 6c64 7420 3d20   ldt_str, ldt = 
-00006490: 7365 6e73 6564 5f6c 6474 732e 706f 7028  sensed_ldts.pop(
-000064a0: 290d 0a20 2020 2020 2020 2065 6c69 6620  )..        elif 
-000064b0: 6c6f 6361 6c5f 6465 6e73 6974 795f 7468  local_density_th
-000064c0: 7265 7368 6f6c 6420 696e 2028 6c64 745b  reshold in (ldt[
-000064d0: 315d 2066 6f72 206c 6474 2069 6e20 7365  1] for ldt in se
-000064e0: 6e73 6564 5f6c 6474 7329 3a0d 0a20 2020  nsed_ldts):..   
-000064f0: 2020 2020 2020 2020 206c 6474 5f73 7472           ldt_str
-00006500: 2c20 6c64 7420 3d20 5b28 6c64 745f 7374  , ldt = [(ldt_st
-00006510: 722c 206c 6474 2920 666f 7220 6c64 745f  r, ldt) for ldt_
-00006520: 7374 722c 206c 6474 2069 6e20 7365 6e73  str, ldt in sens
-00006530: 6564 5f6c 6474 7320 6966 206c 6474 203d  ed_ldts if ldt =
-00006540: 3d20 6c6f 6361 6c5f 6465 6e73 6974 795f  = local_density_
-00006550: 7468 7265 7368 6f6c 645d 2e70 6f70 2829  threshold].pop()
-00006560: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-00006570: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-00006580: 6769 6e67 2e65 7272 6f72 2866 226c 6f63  ging.error(f"loc
-00006590: 616c 5f64 656e 7369 7479 5f74 6872 6573  al_density_thres
-000065a0: 686f 6c64 206f 6620 7b6c 6f63 616c 5f64  hold of {local_d
-000065b0: 656e 7369 7479 5f74 6872 6573 686f 6c64  ensity_threshold
-000065c0: 7d20 646f 6573 206e 6f74 206d 6174 6368  } does not match
-000065d0: 2077 6861 7420 6973 2069 6e20 7468 6520   what is in the 
-000065e0: 634e 4d46 2072 6573 756c 7420 6469 7265  cNMF result dire
-000065f0: 6374 6f72 793a 207b 7365 6e73 6564 5f6c  ctory: {sensed_l
-00006600: 6474 737d 2229 0d0a 2020 2020 2020 2020  dts}")..        
-00006610: 2020 2020 7379 732e 6578 6974 2831 290d      sys.exit(1).
-00006620: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
-00006630: 6174 612e 756e 735b 226c 6474 225d 203d  ata.uns["ldt"] =
-00006640: 206c 6474 0d0a 2020 2020 2020 2020 7365   ldt..        se
-00006650: 6c66 2e61 6461 7461 2e75 6e73 5b22 6c6e  lf.adata.uns["ln
-00006660: 7322 5d20 3d20 6c6f 6361 6c5f 6e65 6967  s"] = local_neig
-00006670: 6862 6f72 686f 6f64 5f73 697a 650d 0a20  hborhood_size.. 
-00006680: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00006690: 2020 2020 2023 2049 6d70 6f72 7420 4745       # Import GE
-000066a0: 5073 0d0a 2020 2020 2020 2020 7265 7375  Ps..        resu
-000066b0: 6c74 5f74 7970 6573 203d 207b 0d0a 2020  lt_types = {..  
-000066c0: 2020 2020 2020 2020 2020 2267 656e 655f            "gene_
-000066d0: 7370 6563 7472 615f 7363 6f72 6522 3a20  spectra_score": 
-000066e0: 2263 6e6d 665f 6765 705f 7363 6f72 6522  "cnmf_gep_score"
-000066f0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00006700: 6765 6e65 5f73 7065 6374 7261 5f74 706d  gene_spectra_tpm
-00006710: 223a 2022 636e 6d66 5f67 6570 5f74 706d  ": "cnmf_gep_tpm
-00006720: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00006730: 2273 7065 6374 7261 223a 2022 636e 6d66  "spectra": "cnmf
-00006740: 5f67 6570 5f72 6177 220d 0a20 2020 2020  _gep_raw"..     
-00006750: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
-00006760: 2020 666f 7220 6d61 7463 6873 7472 2c20    for matchstr, 
-00006770: 7265 7375 6c74 5f74 7970 6520 696e 2072  result_type in r
-00006780: 6573 756c 745f 7479 7065 732e 6974 656d  esult_types.item
-00006790: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
-000067a0: 2020 6c6f 6767 696e 672e 696e 666f 2866    logging.info(f
-000067b0: 2249 6d70 6f72 7469 6e67 2047 4550 733a  "Importing GEPs:
-000067c0: 207b 6d61 7463 6873 7472 7d22 2920 200d   {matchstr}")  .
-000067d0: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
-000067e0: 615f 7720 3d20 5b5d 0d0a 2020 2020 2020  a_w = []..      
-000067f0: 2020 2020 2020 666f 7220 666e 2069 6e20        for fn in 
-00006800: 676c 6f62 286f 732e 7061 7468 2e6a 6f69  glob(os.path.joi
-00006810: 6e28 636e 6d66 5f6f 7574 7075 745f 6469  n(cnmf_output_di
-00006820: 722c 2063 6e6d 665f 6e61 6d65 2c20 6622  r, cnmf_name, f"
-00006830: 7b63 6e6d 665f 6e61 6d65 7d2a 2e7b 6d61  {cnmf_name}*.{ma
-00006840: 7463 6873 7472 7d2e 6b5f 2a2e 7b6c 6474  tchstr}.k_*.{ldt
-00006850: 5f73 7472 7d2e 2a74 7874 2229 293a 0d0a  _str}.*txt")):..
-00006860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006870: 6b20 3d20 696e 7428 6f73 2e70 6174 682e  k = int(os.path.
-00006880: 6261 7365 6e61 6d65 2866 6e29 2e72 656d  basename(fn).rem
-00006890: 6f76 6570 7265 6669 7828 6622 7b63 6e6d  oveprefix(f"{cnm
-000068a0: 665f 6e61 6d65 7d2e 7b6d 6174 6368 7374  f_name}.{matchst
-000068b0: 727d 2e22 292e 7370 6c69 7428 222e 2229  r}.").split(".")
-000068c0: 5b30 5d2e 7265 706c 6163 6528 226b 5f22  [0].replace("k_"
-000068d0: 2c20 2222 2929 0d0a 2020 2020 2020 2020  , ""))..        
-000068e0: 2020 2020 2020 2020 7720 3d20 7064 2e72          w = pd.r
-000068f0: 6561 645f 7461 626c 6528 666e 2c20 696e  ead_table(fn, in
-00006900: 6465 785f 636f 6c3d 3029 0d0a 2020 2020  dex_col=0)..    
-00006910: 2020 2020 2020 2020 2020 2020 772e 696e              w.in
-00006920: 6465 7820 3d20 7374 7228 6b29 202b 2022  dex = str(k) + "
-00006930: 2e22 202b 2077 2e69 6e64 6578 2e61 7374  ." + w.index.ast
-00006940: 7970 6528 7374 7229 0d0a 2020 2020 2020  ype(str)..      
-00006950: 2020 2020 2020 2020 2020 6d65 7461 5f77            meta_w
-00006960: 2e61 7070 656e 6428 7729 0d0a 2020 2020  .append(w)..    
-00006970: 2020 2020 2020 2020 6d65 7461 5f77 203d          meta_w =
-00006980: 2070 642e 636f 6e63 6174 286d 6574 615f   pd.concat(meta_
-00006990: 772c 2061 7869 733d 3029 2e54 2e72 6569  w, axis=0).T.rei
-000069a0: 6e64 6578 2873 656c 662e 6164 6174 612e  ndex(self.adata.
-000069b0: 7661 722e 696e 6465 7829 2e72 656e 616d  var.index).renam
-000069c0: 655f 6178 6973 285b 226b 2e67 6570 225d  e_axis(["k.gep"]
-000069d0: 2c20 6178 6973 3d31 290d 0a20 2020 2020  , axis=1)..     
-000069e0: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
-000069f0: 612e 7661 726d 5b72 6573 756c 745f 7479  a.varm[result_ty
-00006a00: 7065 5d20 3d20 6d65 7461 5f77 0d0a 0d0a  pe] = meta_w....
-00006a10: 2020 2020 2020 2020 2320 496d 706f 7274          # Import
-00006a20: 2055 7361 6765 730d 0a20 2020 2020 2020   Usages..       
-00006a30: 206c 6f67 6769 6e67 2e69 6e66 6f28 6622   logging.info(f"
-00006a40: 496d 706f 7274 696e 6720 5573 6167 6573  Importing Usages
-00006a50: 2229 2020 0d0a 2020 2020 2020 2020 7573  ")  ..        us
-00006a60: 6167 6520 3d20 5b5d 0d0a 2020 2020 2020  age = []..      
-00006a70: 2020 666f 7220 666e 2069 6e20 676c 6f62    for fn in glob
-00006a80: 286f 732e 7061 7468 2e6a 6f69 6e28 636e  (os.path.join(cn
-00006a90: 6d66 5f6f 7574 7075 745f 6469 722c 2063  mf_output_dir, c
-00006aa0: 6e6d 665f 6e61 6d65 2c20 6622 7b63 6e6d  nmf_name, f"{cnm
-00006ab0: 665f 6e61 6d65 7d2a 2e75 7361 6765 732e  f_name}*.usages.
-00006ac0: 6b5f 2a2e 7b6c 6474 5f73 7472 7d2e 2a74  k_*.{ldt_str}.*t
-00006ad0: 7874 2229 293a 0d0a 2020 2020 2020 2020  xt")):..        
-00006ae0: 2020 2020 6b20 3d20 696e 7428 6f73 2e70      k = int(os.p
-00006af0: 6174 682e 6261 7365 6e61 6d65 2866 6e29  ath.basename(fn)
-00006b00: 2e72 656d 6f76 6570 7265 6669 7828 6622  .removeprefix(f"
-00006b10: 7b63 6e6d 665f 6e61 6d65 7d2e 7573 6167  {cnmf_name}.usag
-00006b20: 6573 2e22 292e 7370 6c69 7428 222e 2229  es.").split(".")
-00006b30: 5b30 5d2e 7265 706c 6163 6528 226b 5f22  [0].replace("k_"
-00006b40: 2c20 2222 2929 0d0a 2020 2020 2020 2020  , ""))..        
-00006b50: 2020 2020 6820 3d20 7064 2e72 6561 645f      h = pd.read_
-00006b60: 7461 626c 6528 666e 2c20 696e 6465 785f  table(fn, index_
-00006b70: 636f 6c3d 3029 0d0a 2020 2020 2020 2020  col=0)..        
-00006b80: 2020 2020 682e 636f 6c75 6d6e 7320 3d20      h.columns = 
-00006b90: 7374 7228 6b29 202b 2022 2e22 202b 2068  str(k) + "." + h
-00006ba0: 2e63 6f6c 756d 6e73 2e61 7374 7970 6528  .columns.astype(
-00006bb0: 7374 7229 0d0a 2020 2020 2020 2020 2020  str)..          
-00006bc0: 2020 7573 6167 652e 6170 7065 6e64 2868    usage.append(h
-00006bd0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00006be0: 6164 6174 612e 6f62 736d 5b22 636e 6d66  adata.obsm["cnmf
-00006bf0: 5f75 7361 6765 225d 203d 2070 642e 636f  _usage"] = pd.co
-00006c00: 6e63 6174 2875 7361 6765 2c20 6178 6973  ncat(usage, axis
-00006c10: 3d31 292e 736f 7274 5f69 6e64 6578 2861  =1).sort_index(a
-00006c20: 7869 733d 3129 2e72 656e 616d 655f 6178  xis=1).rename_ax
-00006c30: 6973 285b 226b 2e67 6570 225d 2c20 6178  is(["k.gep"], ax
-00006c40: 6973 3d31 290d 0a20 2020 2020 2020 200d  is=1)..        .
-00006c50: 0a20 2020 2020 2020 2023 2049 6d70 6f72  .        # Impor
-00006c60: 7420 6765 6e65 206c 6973 7420 7573 6564  t gene list used
-00006c70: 2066 6f72 2066 6163 746f 7269 7a61 7469   for factorizati
-00006c80: 6f6e 0d0a 2020 2020 2020 2020 7769 7468  on..        with
-00006c90: 206f 7065 6e28 6f73 2e70 6174 682e 6a6f   open(os.path.jo
-00006ca0: 696e 2863 6e6d 665f 6f75 7470 7574 5f64  in(cnmf_output_d
-00006cb0: 6972 2c20 636e 6d66 5f6e 616d 652c 2066  ir, cnmf_name, f
-00006cc0: 227b 636e 6d66 5f6e 616d 657d 2e6f 7665  "{cnmf_name}.ove
-00006cd0: 7264 6973 7065 7273 6564 5f67 656e 6573  rdispersed_genes
-00006ce0: 2e74 7874 2229 2920 6173 2066 3a0d 0a20  .txt")) as f:.. 
-00006cf0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00006d00: 6164 6174 612e 756e 735b 2267 656e 655f  adata.uns["gene_
-00006d10: 6c69 7374 225d 203d 205b 6c69 6e65 2e73  list"] = [line.s
-00006d20: 7472 6970 2829 2066 6f72 206c 696e 6520  trip() for line 
-00006d30: 696e 2066 2e72 6561 646c 696e 6573 2829  in f.readlines()
-00006d40: 5d0d 0a0d 0a20 2020 2020 2020 2023 2049  ]....        # I
-00006d50: 6d70 6f72 7420 4b2d 7365 6c65 6374 696f  mport K-selectio
-00006d60: 6e20 7374 6174 730d 0a20 2020 2020 2020  n stats..       
-00006d70: 206b 7661 6c73 203d 2070 642e 4461 7461   kvals = pd.Data
-00006d80: 4672 616d 6528 2a2a 6e70 2e6c 6f61 6428  Frame(**np.load(
-00006d90: 6f73 2e70 6174 682e 6a6f 696e 2863 6e6d  os.path.join(cnm
-00006da0: 665f 6f75 7470 7574 5f64 6972 2c20 636e  f_output_dir, cn
-00006db0: 6d66 5f6e 616d 652c 2066 227b 636e 6d66  mf_name, f"{cnmf
-00006dc0: 5f6e 616d 657d 2e6b 5f73 656c 6563 7469  _name}.k_selecti
-00006dd0: 6f6e 5f73 7461 7473 2e64 662e 6e70 7a22  on_stats.df.npz"
-00006de0: 292c 2061 6c6c 6f77 5f70 6963 6b6c 653d  ), allow_pickle=
-00006df0: 5472 7565 2929 2e73 6574 5f69 6e64 6578  True)).set_index
-00006e00: 2822 6b22 295b 5b22 7374 6162 696c 6974  ("k")[["stabilit
-00006e10: 7922 2c20 2270 7265 6469 6374 696f 6e5f  y", "prediction_
-00006e20: 6572 726f 7222 5d5d 0d0a 2020 2020 2020  error"]]..      
-00006e30: 2020 6b76 616c 732e 696e 6465 7820 3d20    kvals.index = 
-00006e40: 6b76 616c 732e 696e 6465 782e 6173 7479  kvals.index.asty
-00006e50: 7065 2869 6e74 290d 0a20 2020 2020 2020  pe(int)..       
-00006e60: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
-00006e70: 226b 7661 6c73 225d 203d 206b 7661 6c73  "kvals"] = kvals
-00006e80: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-00006e90: 7070 656e 645f 746f 5f68 6973 746f 7279  ppend_to_history
-00006ea0: 2822 634e 4d46 2072 6573 756c 7473 2061  ("cNMF results a
-00006eb0: 6464 6564 2066 726f 6d20 6f75 7470 7574  dded from output
-00006ec0: 2064 6972 6563 746f 7279 207b 636e 6d66   directory {cnmf
-00006ed0: 5f6f 7574 7075 745f 6469 727d 2f7b 636e  _output_dir}/{cn
-00006ee0: 6d66 5f6e 616d 657d 2229 0d0a 0d0a 2020  mf_name}")....  
-00006ef0: 2020 6465 6620 6765 745f 7573 6167 6573    def get_usages
-00006f00: 2873 656c 662c 0d0a 2020 2020 2020 2020  (self,..        
-00006f10: 2020 2020 2020 2020 2020 206b 3a20 556e             k: Un
-00006f20: 696f 6e5b 696e 742c 2049 7465 7261 626c  ion[int, Iterabl
-00006f30: 655d 203d 204e 6f6e 652c 0d0a 2020 2020  e] = None,..    
-00006f40: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00006f50: 6973 6372 6574 697a 653a 2062 6f6f 6c20  iscretize: bool 
-00006f60: 3d20 4661 6c73 652c 0d0a 2020 2020 2020  = False,..      
-00006f70: 2020 2020 2020 2020 2020 2020 206e 6f72               nor
-00006f80: 6d61 6c69 7a65 3a20 626f 6f6c 203d 2046  malize: bool = F
-00006f90: 616c 7365 0d0a 2020 2020 2020 2020 2020  alse..          
-00006fa0: 2020 2020 2020 2020 2029 202d 3e20 7064           ) -> pd
-00006fb0: 2e44 6174 6146 7261 6d65 3a0d 0a20 2020  .DataFrame:..   
-00006fc0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00006fd0: 2020 4361 6c63 756c 6174 6520 7573 6167    Calculate usag
-00006fe0: 6520 6f66 2065 6163 6820 4745 5020 696e  e of each GEP in
-00006ff0: 2065 6163 6820 7361 6d70 6c65 2f6f 6273   each sample/obs
-00007000: 6572 7661 7469 6f6e 2e0d 0a0d 0a20 2020  ervation.....   
-00007010: 2020 2020 203a 7061 7261 6d20 6b3a 2049       :param k: I
-00007020: 6620 616e 2069 6e74 6567 6572 206f 7220  f an integer or 
-00007030: 6c69 7374 206f 6620 696e 7465 6765 7273  list of integers
-00007040: 2c20 7265 7475 726e 7320 7573 6167 6573  , returns usages
-00007050: 206f 6e6c 7920 666f 7220 7370 6563 6966   only for specif
-00007060: 6965 6420 7261 6e6b 732e 204f 7468 6572  ied ranks. Other
-00007070: 7769 7365 2c20 7265 7475 726e 7320 7573  wise, returns us
-00007080: 6167 6520 6f66 2061 6c6c 2047 4550 7320  age of all GEPs 
-00007090: 6163 726f 7373 2072 616e 6b73 2e20 4465  across ranks. De
-000070a0: 6661 756c 7473 2074 6f20 4e6f 6e65 0d0a  faults to None..
-000070b0: 2020 2020 2020 2020 3a74 7970 6520 6b3a          :type k:
-000070c0: 2069 6e74 2c20 6f70 7469 6f6e 616c 0d0a   int, optional..
-000070d0: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
-000070e0: 6973 6372 6574 697a 653a 2044 6973 6372  iscretize: Discr
-000070f0: 6574 697a 6573 2074 6865 2075 7361 6765  etizes the usage
-00007100: 206d 6174 7269 7820 7375 6368 2074 6861   matrix such tha
-00007110: 7420 666f 7220 6561 6368 2076 616c 7565  t for each value
-00007120: 206f 6620 6b2c 2065 6163 6820 7361 6d70   of k, each samp
-00007130: 6c65 2068 6173 2075 7361 6765 206f 6620  le has usage of 
-00007140: 6f6e 6c79 2031 2047 4550 2028 7468 6520  only 1 GEP (the 
-00007150: 6f6e 6520 7769 7468 2074 6865 206d 6178  one with the max
-00007160: 696d 756d 2075 7361 6765 292e 2044 6566  imum usage). Def
-00007170: 6175 6c74 7320 746f 2046 616c 7365 0d0a  aults to False..
-00007180: 2020 2020 2020 2020 3a74 7970 6520 6469          :type di
-00007190: 7363 7265 7469 7a65 3a20 626f 6f6c 2c20  scretize: bool, 
-000071a0: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
-000071b0: 2020 3a70 6172 616d 206e 6f72 6d61 6c69    :param normali
-000071c0: 7a65 3a20 4e6f 726d 616c 697a 6520 7468  ze: Normalize th
-000071d0: 6520 4745 5020 7573 6167 6520 6d61 7472  e GEP usage matr
-000071e0: 6978 2073 7563 6820 7468 6174 2066 6f72  ix such that for
-000071f0: 2065 6163 6820 7661 6c75 6520 6f66 206b   each value of k
-00007200: 2c20 7573 6167 6520 6f66 2061 6c6c 2047  , usage of all G
-00007210: 4550 7320 7375 6d73 2074 6f20 312e 2044  EPs sums to 1. D
-00007220: 6566 6175 6c74 7320 746f 2046 616c 7365  efaults to False
-00007230: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00007240: 6e6f 726d 616c 697a 653a 2062 6f6f 6c2c  normalize: bool,
-00007250: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
-00007260: 2020 203a 7265 7475 726e 3a20 6f62 7365     :return: obse
-00007270: 7276 6174 696f 6e20 c397 2047 4550 206d  rvation .. GEP m
-00007280: 6174 7269 780d 0a20 2020 2020 2020 203a  atrix..        :
-00007290: 7274 7970 653a 2070 642e 4461 7461 4672  rtype: pd.DataFr
-000072a0: 616d 650d 0a20 2020 2020 2020 2022 2222  ame..        """
-000072b0: 0d0a 2020 2020 2020 2020 6466 203d 2073  ..        df = s
-000072c0: 656c 662e 6164 6174 612e 6f62 736d 5b22  elf.adata.obsm["
-000072d0: 636e 6d66 5f75 7361 6765 225d 2e63 6f70  cnmf_usage"].cop
-000072e0: 7928 290d 0a20 2020 2020 2020 2064 662e  y()..        df.
-000072f0: 636f 6c75 6d6e 7320 3d20 7064 2e4d 756c  columns = pd.Mul
-00007300: 7469 496e 6465 782e 6672 6f6d 5f74 7570  tiIndex.from_tup
-00007310: 6c65 7328 6466 2e63 6f6c 756d 6e73 2e73  les(df.columns.s
-00007320: 7472 2e73 706c 6974 2822 2e22 292e 746f  tr.split(".").to
-00007330: 5f6c 6973 7428 2929 0d0a 2020 2020 2020  _list())..      
-00007340: 2020 6466 2e63 6f6c 756d 6e73 203d 2064    df.columns = d
-00007350: 662e 636f 6c75 6d6e 732e 7365 745f 6c65  f.columns.set_le
-00007360: 7665 6c73 285b 6c2e 6173 7479 7065 2822  vels([l.astype("
-00007370: 696e 7422 2920 666f 7220 6c20 696e 2064  int") for l in d
-00007380: 662e 636f 6c75 6d6e 732e 6c65 7665 6c73  f.columns.levels
-00007390: 5d29 0d0a 2020 2020 2020 2020 6966 206e  ])..        if n
-000073a0: 6f72 6d61 6c69 7a65 3a0d 0a20 2020 2020  ormalize:..     
-000073b0: 2020 2020 2020 206e 6f72 6d61 6c69 7a65         normalize
-000073c0: 6420 3d20 5b5d 0d0a 2020 2020 2020 2020  d = []..        
-000073d0: 2020 2020 666f 7220 5f2c 2073 7562 6466      for _, subdf
-000073e0: 2069 6e20 6466 2e67 726f 7570 6279 2861   in df.groupby(a
-000073f0: 7869 733d 312c 206c 6576 656c 3d30 293a  xis=1, level=0):
-00007400: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007410: 2020 6e6f 726d 616c 697a 6564 2e61 7070    normalized.app
-00007420: 656e 6428 7375 6264 662e 6469 7628 7375  end(subdf.div(su
-00007430: 6264 662e 7375 6d28 6178 6973 3d31 292c  bdf.sum(axis=1),
-00007440: 2061 7869 733d 3029 290d 0a20 2020 2020   axis=0))..     
-00007450: 2020 2020 2020 2064 6620 3d20 7064 2e63         df = pd.c
-00007460: 6f6e 6361 7428 6e6f 726d 616c 697a 6564  oncat(normalized
-00007470: 2c20 6178 6973 3d31 290d 0a20 2020 2020  , axis=1)..     
-00007480: 2020 2069 6620 6469 7363 7265 7469 7a65     if discretize
-00007490: 3a0d 0a20 2020 2020 2020 2020 2020 2064  :..            d
-000074a0: 6973 6372 6574 697a 6564 203d 205b 5d0d  iscretized = [].
-000074b0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-000074c0: 205f 2c20 7375 6264 6620 696e 2064 662e   _, subdf in df.
-000074d0: 6772 6f75 7062 7928 6178 6973 3d31 2c20  groupby(axis=1, 
-000074e0: 6c65 7665 6c3d 3029 3a0d 0a20 2020 2020  level=0):..     
-000074f0: 2020 2020 2020 2020 2020 2064 6973 6372             discr
-00007500: 6574 697a 6564 2e61 7070 656e 6428 7375  etized.append(su
-00007510: 6264 662e 6571 2873 7562 6466 2e6d 6178  bdf.eq(subdf.max
-00007520: 2861 7869 733d 3129 2c20 6178 6973 3d30  (axis=1), axis=0
-00007530: 292e 6173 7479 7065 2869 6e74 2929 0d0a  ).astype(int))..
-00007540: 2020 2020 2020 2020 2020 2020 6466 203d              df =
-00007550: 2070 642e 636f 6e63 6174 2864 6973 6372   pd.concat(discr
-00007560: 6574 697a 6564 2c20 6178 6973 3d31 2920  etized, axis=1) 
-00007570: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00007580: 2069 6620 6b20 6973 206e 6f74 204e 6f6e   if k is not Non
-00007590: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000075a0: 6466 203d 2064 662e 6c6f 635b 3a2c 206b  df = df.loc[:, k
-000075b0: 5d0d 0a20 2020 2020 2020 2064 6620 3d20  ]..        df = 
-000075c0: 6466 2e73 6f72 745f 696e 6465 7828 6178  df.sort_index(ax
-000075d0: 6973 3d30 292e 736f 7274 5f69 6e64 6578  is=0).sort_index
-000075e0: 2861 7869 733d 3129 2020 200d 0a20 2020  (axis=1)   ..   
-000075f0: 2020 2020 2072 6574 7572 6e20 6466 0d0a       return df..
-00007600: 2020 2020 0d0a 2020 2020 6465 6620 6765      ..    def ge
-00007610: 745f 6765 7073 2873 656c 662c 0d0a 2020  t_geps(self,..  
-00007620: 2020 2020 2020 2020 2020 2020 2020 206b                 k
-00007630: 3a20 556e 696f 6e5b 696e 742c 2049 7465  : Union[int, Ite
-00007640: 7261 626c 655d 203d 204e 6f6e 652c 0d0a  rable] = None,..
-00007650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007660: 2074 7970 653d 2263 6e6d 665f 6765 705f   type="cnmf_gep_
-00007670: 7363 6f72 6522 0d0a 2020 2020 2020 2020  score"..        
-00007680: 2020 2020 2020 2020 2029 202d 3e20 7064           ) -> pd
-00007690: 2e44 6174 6146 7261 6d65 3a0d 0a20 2020  .DataFrame:..   
-000076a0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-000076b0: 2020 4765 7420 4745 5073 2e0d 0a0d 0a20    Get GEPs..... 
-000076c0: 2020 2020 2020 203a 7061 7261 6d20 6b3a         :param k:
-000076d0: 2049 6620 616e 2069 6e74 6567 6572 206f   If an integer o
-000076e0: 7220 6c69 7374 206f 6620 696e 7465 6765  r list of intege
-000076f0: 7273 2c20 7265 7475 726e 7320 4745 5073  rs, returns GEPs
-00007700: 206f 6e6c 7920 666f 7220 7370 6563 6966   only for specif
-00007710: 6965 6420 7261 6e6b 732e 204f 7468 6572  ied ranks. Other
-00007720: 7769 7365 2c20 7265 7475 726e 7320 4745  wise, returns GE
-00007730: 5073 2066 726f 6d20 616c 6c20 7261 6e6b  Ps from all rank
-00007740: 732e 2044 6566 6175 6c74 7320 746f 204e  s. Defaults to N
-00007750: 6f6e 650d 0a20 2020 2020 2020 203a 7479  one..        :ty
-00007760: 7065 206b 3a20 556e 696f 6e5b 696e 742c  pe k: Union[int,
-00007770: 2049 7465 7261 626c 655d 2c20 6f70 7469   Iterable], opti
-00007780: 6f6e 616c 0d0a 2020 2020 2020 2020 3a70  onal..        :p
-00007790: 6172 616d 2074 7970 653a 2022 636e 6d66  aram type: "cnmf
-000077a0: 5f67 6570 5f73 636f 7265 2220 6f72 2022  _gep_score" or "
-000077b0: 636e 6d66 5f67 6570 5f74 706d 222c 2064  cnmf_gep_tpm", d
-000077c0: 6566 6175 6c74 7320 746f 2022 636e 6d66  efaults to "cnmf
-000077d0: 5f67 6570 5f73 636f 7265 220d 0a20 2020  _gep_score"..   
-000077e0: 2020 2020 203a 7479 7065 2074 7970 653a       :type type:
-000077f0: 2073 7472 2c20 6f70 7469 6f6e 616c 0d0a   str, optional..
-00007800: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00007810: 2066 6561 7475 7265 7320 c397 2047 4550   features .. GEP
-00007820: 206d 6174 7269 780d 0a20 2020 2020 2020   matrix..       
-00007830: 203a 7274 7970 653a 2070 642e 4461 7461   :rtype: pd.Data
-00007840: 4672 616d 650d 0a20 2020 2020 2020 2022  Frame..        "
-00007850: 2222 0d0a 2020 2020 2020 2020 6466 203d  ""..        df =
-00007860: 2073 656c 662e 6164 6174 612e 7661 726d   self.adata.varm
-00007870: 5b74 7970 655d 2e63 6f70 7928 290d 0a20  [type].copy().. 
-00007880: 2020 2020 2020 2064 662e 636f 6c75 6d6e         df.column
-00007890: 7320 3d20 7064 2e4d 756c 7469 496e 6465  s = pd.MultiInde
-000078a0: 782e 6672 6f6d 5f74 7570 6c65 7328 6466  x.from_tuples(df
-000078b0: 2e63 6f6c 756d 6e73 2e73 7472 2e73 706c  .columns.str.spl
-000078c0: 6974 2822 2e22 292e 746f 5f6c 6973 7428  it(".").to_list(
-000078d0: 2929 0d0a 2020 2020 2020 2020 6466 2e63  ))..        df.c
-000078e0: 6f6c 756d 6e73 203d 2064 662e 636f 6c75  olumns = df.colu
-000078f0: 6d6e 732e 7365 745f 6c65 7665 6c73 285b  mns.set_levels([
-00007900: 6c2e 6173 7479 7065 2822 696e 7422 2920  l.astype("int") 
-00007910: 666f 7220 6c20 696e 2064 662e 636f 6c75  for l in df.colu
-00007920: 6d6e 732e 6c65 7665 6c73 5d29 0d0a 2020  mns.levels])..  
-00007930: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00007940: 6e63 6528 6b2c 2028 696e 742c 2049 7465  nce(k, (int, Ite
-00007950: 7261 626c 6529 293a 0d0a 2020 2020 2020  rable)):..      
-00007960: 2020 2020 2020 6466 203d 2064 662e 6c6f        df = df.lo
-00007970: 635b 3a2c 206b 5d0d 0a20 2020 2020 2020  c[:, k]..       
-00007980: 2064 6620 3d20 6466 2e73 6f72 745f 696e   df = df.sort_in
-00007990: 6465 7828 6178 6973 3d31 290d 0a20 2020  dex(axis=1)..   
-000079a0: 2020 2020 2072 6574 7572 6e20 6466 0d0a       return df..
-000079b0: 2020 2020 0d0a 2020 2020 6465 6620 6765      ..    def ge
-000079c0: 745f 6d65 7461 6461 7461 5f64 6628 7365  t_metadata_df(se
-000079d0: 6c66 2c0d 0a20 2020 2020 2020 2020 2020  lf,..           
-000079e0: 2020 2020 2020 2020 2020 2020 2069 6e63               inc
-000079f0: 6c75 6465 5f63 6174 6567 6f72 6963 616c  lude_categorical
-00007a00: 3a20 626f 6f6c 203d 2054 7275 652c 0d0a  : bool = True,..
-00007a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a20: 2020 2020 2020 2020 696e 636c 7564 655f          include_
-00007a30: 6e75 6d65 7269 6361 6c3a 2062 6f6f 6c20  numerical: bool 
-00007a40: 3d20 5472 7565 0d0a 2020 2020 2020 2020  = True..        
-00007a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a60: 2920 2d3e 2070 642e 4461 7461 4672 616d  ) -> pd.DataFram
-00007a70: 653a 0d0a 2020 2020 2020 2020 2222 2247  e:..        """G
-00007a80: 6574 2073 616d 706c 652f 6f62 7365 7276  et sample/observ
-00007a90: 6174 696f 6e20 6d65 7461 6461 7461 2e0d  ation metadata..
-00007aa0: 0a0d 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-00007ab0: 6d20 696e 636c 7564 655f 6361 7465 676f  m include_catego
-00007ac0: 7269 6361 6c3a 2049 6e63 6c75 6465 2063  rical: Include c
-00007ad0: 6174 6567 6f72 6963 616c 206d 6574 6164  ategorical metad
-00007ae0: 6174 6120 6c61 7965 7273 2c20 6465 6661  ata layers, defa
-00007af0: 756c 7473 2074 6f20 5472 7565 0d0a 2020  ults to True..  
-00007b00: 2020 2020 2020 3a74 7970 6520 696e 636c        :type incl
-00007b10: 7564 655f 6361 7465 676f 7269 6361 6c3a  ude_categorical:
-00007b20: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0d   bool, optional.
-00007b30: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00007b40: 696e 636c 7564 655f 6e75 6d65 7269 6361  include_numerica
-00007b50: 6c3a 2049 6e63 6c75 6465 206e 756d 6572  l: Include numer
-00007b60: 6963 616c 206d 6574 6164 6174 6120 6c61  ical metadata la
-00007b70: 7965 7273 2c20 6465 6661 756c 7473 2074  yers, defaults t
-00007b80: 6f20 5472 7565 0d0a 2020 2020 2020 2020  o True..        
-00007b90: 3a74 7970 6520 696e 636c 7564 655f 6e75  :type include_nu
-00007ba0: 6d65 7269 6361 6c3a 2062 6f6f 6c2c 206f  merical: bool, o
-00007bb0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
-00007bc0: 203a 7261 6973 6573 2056 616c 7565 4572   :raises ValueEr
-00007bd0: 726f 723a 2045 7272 6f72 2069 6620 6d65  ror: Error if me
-00007be0: 7461 6461 7461 2074 7970 6573 2061 7265  tadata types are
-00007bf0: 206e 6f74 2072 6563 6f67 6e69 7a65 640d   not recognized.
-00007c00: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-00007c10: 3a20 6f62 7365 7276 6174 696f 6e73 20c3  : observations .
-00007c20: 9720 6d65 7461 6461 7461 206d 6174 7269  . metadata matri
-00007c30: 780d 0a20 2020 2020 2020 203a 7274 7970  x..        :rtyp
-00007c40: 653a 2070 642e 4461 7461 4672 616d 650d  e: pd.DataFrame.
-00007c50: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00007c60: 2020 2020 2020 6474 7970 6573 203d 205b        dtypes = [
-00007c70: 5d0d 0a20 2020 2020 2020 2069 6620 696e  ]..        if in
-00007c80: 636c 7564 655f 6361 7465 676f 7269 6361  clude_categorica
-00007c90: 6c3a 0d0a 2020 2020 2020 2020 2020 2020  l:..            
-00007ca0: 6474 7970 6573 2e61 7070 656e 6428 2263  dtypes.append("c
-00007cb0: 6174 6567 6f72 7922 290d 0a20 2020 2020  ategory")..     
-00007cc0: 2020 2069 6620 696e 636c 7564 655f 6e75     if include_nu
-00007cd0: 6d65 7269 6361 6c3a 0d0a 2020 2020 2020  merical:..      
-00007ce0: 2020 2020 2020 6474 7970 6573 202b 3d20        dtypes += 
-00007cf0: 5b22 666c 6f61 7422 2c20 2269 6e74 225d  ["float", "int"]
-00007d00: 0d0a 2020 2020 2020 2020 756e 6578 706c  ..        unexpl
-00007d10: 6169 6e65 645f 636f 6c73 203d 2073 656c  ained_cols = sel
-00007d20: 662e 6164 6174 612e 6f62 732e 7365 6c65  f.adata.obs.sele
-00007d30: 6374 5f64 7479 7065 7328 6578 636c 7564  ct_dtypes(exclud
-00007d40: 653d 2822 6361 7465 676f 7279 222c 2022  e=("category", "
-00007d50: 666c 6f61 7422 2c20 2269 6e74 2229 292e  float", "int")).
-00007d60: 636f 6c75 6d6e 730d 0a20 2020 2020 2020  columns..       
-00007d70: 2069 6620 6c65 6e28 756e 6578 706c 6169   if len(unexplai
-00007d80: 6e65 645f 636f 6c73 2920 3e20 303a 0d0a  ned_cols) > 0:..
-00007d90: 2020 2020 2020 2020 2020 2020 756e 6578              unex
-00007da0: 706c 6169 6e65 645f 636f 6c5f 7374 7220  plained_col_str 
-00007db0: 3d20 222c 2022 2e6a 6f69 6e28 756e 6578  = ", ".join(unex
-00007dc0: 706c 6169 6e65 645f 636f 6c73 290d 0a20  plained_cols).. 
-00007dd0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00007de0: 2056 616c 7565 4572 726f 7228 6622 7b75   ValueError(f"{u
-00007df0: 6e65 7870 6c61 696e 6564 5f63 6f6c 5f73  nexplained_col_s
-00007e00: 7472 7d20 6d65 7461 6461 7461 2063 6f6c  tr} metadata col
-00007e10: 756d 6e73 2068 6176 6520 756e 7265 636f  umns have unreco
-00007e20: 676e 697a 6564 2064 7479 7065 732e 2229  gnized dtypes.")
-00007e30: 0d0a 2020 2020 2020 2020 6466 203d 2073  ..        df = s
-00007e40: 656c 662e 6164 6174 612e 6f62 732e 7365  elf.adata.obs.se
-00007e50: 6c65 6374 5f64 7479 7065 7328 696e 636c  lect_dtypes(incl
-00007e60: 7564 653d 6474 7970 6573 290d 0a20 2020  ude=dtypes)..   
-00007e70: 2020 2020 2072 6574 7572 6e20 6466 0d0a       return df..
-00007e80: 2020 2020 0d0a 2020 2020 6465 6620 6765      ..    def ge
-00007e90: 745f 6361 7465 676f 7279 5f6f 7665 7272  t_category_overr
-00007ea0: 6570 7265 7365 6e74 6174 696f 6e28 7365  epresentation(se
-00007eb0: 6c66 2c0d 0a20 2020 2020 2020 2020 2020  lf,..           
-00007ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ed0: 2020 2020 2020 2020 2020 2020 206c 6179               lay
-00007ee0: 6572 3a20 7374 722c 0d0a 2020 2020 2020  er: str,..      
-00007ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f10: 2020 7472 756e 6361 7465 5f6e 6567 6174    truncate_negat
-00007f20: 6976 653a 2062 6f6f 6c20 3d20 5472 7565  ive: bool = True
-00007f30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f50: 2020 2020 2020 2020 2020 2920 2d3e 2070            ) -> p
-00007f60: 642e 4461 7461 4672 616d 653a 0d0a 2020  d.DataFrame:..  
-00007f70: 2020 2020 2020 2222 2243 616c 6375 6c61        """Calcula
-00007f80: 7465 2050 6561 7273 6f6e 2072 6573 6964  te Pearson resid
-00007f90: 7561 6c20 6f66 2063 6869 2d73 7175 6172  ual of chi-squar
-00007fa0: 6564 2074 6573 742c 2061 7373 6f63 6961  ed test, associa
-00007fb0: 7469 6e67 2047 4550 7320 666f 7220 6561  ting GEPs for ea
-00007fc0: 6368 2072 616e 6b20 286b 2920 746f 2063  ch rank (k) to c
-00007fd0: 6174 6567 6f72 6965 7320 6f66 2073 616d  ategories of sam
-00007fe0: 706c 6573 2f6f 6273 6572 7661 7469 6f6e  ples/observation
-00007ff0: 732e 2042 7920 6465 6661 756c 742c 2074  s. By default, t
-00008000: 7275 6e63 6174 6573 206e 6567 6174 6976  runcates negativ
-00008010: 6520 7661 6c75 6573 2e0d 0a0d 0a20 2020  e values.....   
-00008020: 2020 2020 203a 7061 7261 6d20 6c61 7965       :param laye
-00008030: 723a 206e 616d 6520 6f66 2063 6174 6567  r: name of categ
-00008040: 6f72 6963 616c 2064 6174 6120 6c61 7965  orical data laye
-00008050: 720d 0a20 2020 2020 2020 203a 7479 7065  r..        :type
-00008060: 206c 6179 6572 3a20 7374 720d 0a20 2020   layer: str..   
-00008070: 2020 2020 203a 7061 7261 6d20 7472 756e       :param trun
-00008080: 6361 7465 5f6e 6567 6174 6976 653a 2054  cate_negative: T
-00008090: 7275 6e63 6174 6520 6e65 6761 7469 7665  runcate negative
-000080a0: 2072 6573 6964 7561 6c73 2074 6f20 302c   residuals to 0,
-000080b0: 2064 6566 6175 6c74 7320 746f 2054 7275   defaults to Tru
-000080c0: 650d 0a20 2020 2020 2020 203a 7479 7065  e..        :type
-000080d0: 2074 7275 6e63 6174 655f 6e65 6761 7469   truncate_negati
-000080e0: 7665 3a20 626f 6f6c 2c20 6f70 7469 6f6e  ve: bool, option
-000080f0: 616c 0d0a 2020 2020 2020 2020 3a72 6574  al..        :ret
-00008100: 7572 6e3a 2063 6174 6567 6f72 7920 c397  urn: category ..
-00008110: 2047 4550 206d 6174 7269 7820 6f66 206f   GEP matrix of o
-00008120: 7665 7272 6570 7265 7365 6e74 6174 696f  verrepresentatio
-00008130: 6e20 7661 6c75 6573 0d0a 2020 2020 2020  n values..      
-00008140: 2020 3a72 7479 7065 3a20 7064 2e44 6174    :rtype: pd.Dat
-00008150: 6146 7261 6d65 0d0a 2020 2020 2020 2020  aFrame..        
-00008160: 2222 220d 0a20 2020 2020 2020 2075 7361  """..        usa
-00008170: 6765 203d 2073 656c 662e 6765 745f 7573  ge = self.get_us
-00008180: 6167 6573 2829 2e63 6f70 7928 290d 0a20  ages().copy().. 
-00008190: 2020 2020 2020 2073 616d 706c 655f 746f         sample_to
-000081a0: 5f63 6c61 7373 203d 2073 656c 662e 6765  _class = self.ge
-000081b0: 745f 6d65 7461 6461 7461 5f64 6628 295b  t_metadata_df()[
-000081c0: 6c61 7965 725d 0d0a 2020 2020 2020 2020  layer]..        
-000081d0: 7573 6167 652e 696e 6465 7820 3d20 7573  usage.index = us
-000081e0: 6167 652e 696e 6465 782e 6d61 7028 7361  age.index.map(sa
-000081f0: 6d70 6c65 5f74 6f5f 636c 6173 7329 0d0a  mple_to_class)..
-00008200: 2020 2020 2020 2020 6f62 7365 7276 6564          observed
-00008210: 203d 2075 7361 6765 2e67 726f 7570 6279   = usage.groupby
-00008220: 2861 7869 733d 302c 206c 6576 656c 3d30  (axis=0, level=0
-00008230: 292e 7375 6d28 290d 0a20 2020 2020 2020  ).sum()..       
-00008240: 2065 7870 6563 7465 6420 3d20 5b5d 0d0a   expected = []..
-00008250: 2020 2020 2020 2020 666f 7220 6b2c 206f          for k, o
-00008260: 6273 5f6b 2069 6e20 6f62 7365 7276 6564  bs_k in observed
-00008270: 2e67 726f 7570 6279 2861 7869 733d 312c  .groupby(axis=1,
-00008280: 206c 6576 656c 3d31 293a 0d0a 2020 2020   level=1):..    
-00008290: 2020 2020 2020 2020 6578 705f 6b20 3d20          exp_k = 
-000082a0: 7064 2e44 6174 6146 7261 6d65 286f 6273  pd.DataFrame(obs
-000082b0: 5f6b 2e73 756d 2861 7869 733d 3129 2920  _k.sum(axis=1)) 
-000082c0: 4020 7064 2e44 6174 6146 7261 6d65 286f  @ pd.DataFrame(o
-000082d0: 6273 5f6b 2e73 756d 2861 7869 733d 3029  bs_k.sum(axis=0)
-000082e0: 292e 5420 2f20 6f62 735f 6b2e 7375 6d28  ).T / obs_k.sum(
-000082f0: 292e 7375 6d28 290d 0a20 2020 2020 2020  ).sum()..       
-00008300: 2020 2020 2065 7870 6563 7465 642e 6170       expected.ap
-00008310: 7065 6e64 2865 7870 5f6b 290d 0a20 2020  pend(exp_k)..   
-00008320: 2020 2020 2065 7870 6563 7465 6420 3d20       expected = 
-00008330: 7064 2e63 6f6e 6361 7428 6578 7065 6374  pd.concat(expect
-00008340: 6564 2c20 6178 6973 3d31 290d 0a20 2020  ed, axis=1)..   
-00008350: 2020 2020 2063 6869 7371 5f72 6573 6964       chisq_resid
-00008360: 203d 2028 6f62 7365 7276 6564 202d 2065   = (observed - e
-00008370: 7870 6563 7465 6429 202f 206e 702e 7371  xpected) / np.sq
-00008380: 7274 2865 7870 6563 7465 6429 2020 2320  rt(expected)  # 
-00008390: 7065 6172 736f 6e20 7265 7369 6475 616c  pearson residual
-000083a0: 206f 6620 6368 692d 7371 7561 7265 6420   of chi-squared 
-000083b0: 7465 7374 206f 6620 636f 6e74 696e 6765  test of continge
-000083c0: 6e63 7920 7461 626c 650d 0a20 2020 2020  ncy table..     
-000083d0: 2020 2069 6620 7472 756e 6361 7465 5f6e     if truncate_n
-000083e0: 6567 6174 6976 653a 0d0a 2020 2020 2020  egative:..      
-000083f0: 2020 2020 2020 6368 6973 715f 7265 7369        chisq_resi
-00008400: 6420 3d20 6368 6973 715f 7265 7369 642e  d = chisq_resid.
-00008410: 636c 6970 286c 6f77 6572 3d30 290d 0a20  clip(lower=0).. 
-00008420: 2020 2020 2020 2072 6574 7572 6e20 6368         return ch
-00008430: 6973 715f 7265 7369 640d 0a20 2020 200d  isq_resid..    .
-00008440: 0a20 2020 2020 2020 200d 0a20 2020 2064  .        ..    d
-00008450: 6566 2067 6574 5f6d 6574 6164 6174 615f  ef get_metadata_
-00008460: 636f 7272 656c 6174 696f 6e28 7365 6c66  correlation(self
-00008470: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
-00008480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008490: 2020 2020 206c 6179 6572 3a20 7374 722c       layer: str,
-000084a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000084b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084c0: 2020 206d 6574 686f 643a 2073 7472 203d     method: str =
-000084d0: 2022 7065 6172 736f 6e22 0d0a 2020 2020   "pearson"..    
-000084e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084f0: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
-00008500: 3e20 7064 2e53 6572 6965 733a 0d0a 2020  > pd.Series:..  
-00008510: 2020 2020 2020 2222 2243 616c 6375 6c61        """Calcula
-00008520: 7465 2050 6561 7273 6f6e 2063 6f72 7265  te Pearson corre
-00008530: 6c61 7469 6f6e 206f 6620 4745 5020 7573  lation of GEP us
-00008540: 6167 6520 746f 206e 756d 6572 6963 616c  age to numerical
-00008550: 206d 6574 6164 6174 6120 6163 726f 7373   metadata across
-00008560: 2073 616d 706c 6573 2f6f 6273 6572 7661   samples/observa
-00008570: 7469 6f6e 732e 0d0a 0d0a 2020 2020 2020  tions.....      
-00008580: 2020 3a70 6172 616d 206c 6179 6572 3a20    :param layer: 
-00008590: 6e61 6d65 206f 6620 6e75 6d65 7269 6361  name of numerica
-000085a0: 6c20 6461 7461 206c 6179 6572 0d0a 2020  l data layer..  
-000085b0: 2020 2020 2020 3a74 7970 6520 6c61 7965        :type laye
-000085c0: 723a 2073 7472 0d0a 2020 2020 2020 2020  r: str..        
-000085d0: 3a70 6172 616d 206d 6574 686f 643a 2043  :param method: C
-000085e0: 6f72 7265 6c61 7469 6f6e 206d 6574 686f  orrelation metho
-000085f0: 643a 2022 7065 6172 736f 6e22 2c20 2273  d: "pearson", "s
-00008600: 7065 6172 6d61 6e22 2c20 6f72 2022 6b65  pearman", or "ke
-00008610: 6e64 616c 6c22 2e20 4465 6661 756c 7473  ndall". Defaults
-00008620: 2074 6f20 2270 6561 7273 6f6e 220d 0a20   to "pearson".. 
-00008630: 2020 2020 2020 203a 7479 7065 206d 6574         :type met
-00008640: 686f 643a 2073 7472 2c20 6f70 7469 6f6e  hod: str, option
-00008650: 616c 0d0a 2020 2020 2020 2020 3a72 6574  al..        :ret
-00008660: 7572 6e3a 2063 6f72 7265 6c61 7469 6f6e  urn: correlation
-00008670: 206f 6620 4745 5020 746f 206d 6574 6164   of GEP to metad
-00008680: 6174 610d 0a20 2020 2020 2020 203a 7274  ata..        :rt
-00008690: 7970 653a 2070 642e 5365 7269 6573 0d0a  ype: pd.Series..
-000086a0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-000086b0: 2020 2020 2075 7361 6765 203d 2073 656c       usage = sel
-000086c0: 662e 6765 745f 7573 6167 6573 2829 2e63  f.get_usages().c
-000086d0: 6f70 7928 290d 0a20 2020 2020 2020 206d  opy()..        m
-000086e0: 6574 6164 6174 6120 3d20 7365 6c66 2e67  etadata = self.g
-000086f0: 6574 5f6d 6574 6164 6174 615f 6466 2829  et_metadata_df()
-00008700: 5b6c 6179 6572 5d0d 0a20 2020 2020 2020  [layer]..       
-00008710: 206d 645f 636f 7272 203d 2075 7361 6765   md_corr = usage
-00008720: 2e63 6f72 7277 6974 6828 6d65 7461 6461  .corrwith(metada
-00008730: 7461 2c20 6d65 7468 6f64 3d6d 6574 686f  ta, method=metho
-00008740: 6429 0d0a 2020 2020 2020 2020 7265 7475  d)..        retu
-00008750: 726e 206d 645f 636f 7272 0d0a 2020 2020  rn md_corr..    
-00008760: 2020 2020 0d0a 2020 2020 6465 6620 6170      ..    def ap
-00008770: 7065 6e64 5f74 6f5f 6869 7374 6f72 7928  pend_to_history(
-00008780: 7365 6c66 2c20 656e 7472 7929 3a0d 0a20  self, entry):.. 
-00008790: 2020 2020 2020 2022 2222 4164 6420 656e         """Add en
-000087a0: 7472 7920 746f 2044 6174 6173 6574 2068  try to Dataset h
-000087b0: 6973 746f 7279 2e0d 0a0d 0a20 2020 2020  istory.....     
-000087c0: 2020 203a 7061 7261 6d20 656e 7472 793a     :param entry:
-000087d0: 2044 6573 6372 6970 7469 6f6e 206f 6620   Description of 
-000087e0: 6576 656e 7420 746f 2072 6563 6f72 6420  event to record 
-000087f0: 696e 2074 6865 2068 6973 746f 7279 2e0d  in the history..
-00008800: 0a20 2020 2020 2020 203a 7479 7065 2065  .        :type e
-00008810: 6e74 7279 3a20 7374 720d 0a20 2020 2020  ntry: str..     
-00008820: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00008830: 7365 6c66 2e61 6461 7461 2e75 6e73 5b22  self.adata.uns["
-00008840: 6869 7374 6f72 7922 5d5b 6461 7465 7469  history"][dateti
-00008850: 6d65 2e75 7463 6e6f 7728 292e 6973 6f66  me.utcnow().isof
-00008860: 6f72 6d61 7428 295d 203d 2065 6e74 7279  ormat()] = entry
-00008870: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00008880: 6465 6620 6765 745f 6869 7374 6f72 7928  def get_history(
-00008890: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-000088a0: 2222 2252 6574 7572 6e73 2074 696d 6573  """Returns times
-000088b0: 7461 6d70 6564 2068 6973 746f 7279 206f  tamped history o
-000088c0: 6620 4461 7461 7365 7420 6f62 6a65 6374  f Dataset object
-000088d0: 2e0d 0a0d 0a20 2020 2020 2020 203a 7265  .....        :re
-000088e0: 7475 726e 3a20 6869 7374 6f72 790d 0a20  turn: history.. 
-000088f0: 2020 2020 2020 203a 7274 7970 653a 2064         :rtype: d
-00008900: 6963 740d 0a20 2020 2020 2020 2022 2222  ict..        """
-00008910: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00008920: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
-00008930: 2268 6973 746f 7279 225d                 "history"]
+00004ee0: 2020 2020 2020 2020 7365 6c65 6374 6564          selected
+00004ef0: 5f6d 6574 686f 6473 2e61 7070 656e 6428  _methods.append(
+00004f00: 2271 7561 6e74 696c 6522 290d 0a20 2020  "quantile")..   
+00004f10: 2020 2020 2069 6620 6c65 6e28 7365 6c65       if len(sele
+00004f20: 6374 6564 5f6d 6574 686f 6473 2920 3e20  cted_methods) > 
+00004f30: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
+00004f40: 6d65 7468 6f64 7761 726e 7374 7220 3d20  methodwarnstr = 
+00004f50: 222c 2022 2e6a 6f69 6e28 7365 6c65 6374  ", ".join(select
+00004f60: 6564 5f6d 6574 686f 6473 290d 0a20 2020  ed_methods)..   
+00004f70: 2020 2020 2020 2020 206c 6f67 6769 6e67           logging
+00004f80: 2e77 6172 6e69 6e67 2866 224d 756c 7469  .warning(f"Multi
+00004f90: 706c 6520 636f 6e66 6c69 6374 696e 6720  ple conflicting 
+00004fa0: 6f76 6572 6469 7370 6572 7365 6420 6765  overdispersed ge
+00004fb0: 6e65 2073 656c 6563 7469 6f6e 2063 7269  ne selection cri
+00004fc0: 7465 7269 6120 6861 7665 2062 6565 6e20  teria have been 
+00004fd0: 7365 6c65 6374 6564 3a20 7b6d 6574 686f  selected: {metho
+00004fe0: 6477 6172 6e73 7472 7d2e 2022 0d0a 2020  dwarnstr}. "..  
+00004ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005000: 2020 2020 2020 2020 2020 224f 6e6c 7920            "Only 
+00005010: 7468 6520 696e 7465 7273 6563 7469 6f6e  the intersection
+00005020: 206f 6620 7468 6573 6520 6d65 7468 6f64   of these method
+00005030: 7320 7769 6c6c 2062 6520 7365 6c65 6374  s will be select
+00005040: 6564 2e22 290d 0a20 2020 2020 2020 2020  ed.")..         
+00005050: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00005060: 2023 206d 696e 5f6d 6561 6e20 6669 6c74   # min_mean filt
+00005070: 6572 0d0a 2020 2020 2020 2020 7365 6c65  er..        sele
+00005080: 6374 6564 5f67 656e 6573 203d 2073 656c  cted_genes = sel
+00005090: 662e 6164 6174 612e 7661 725b 226d 6561  f.adata.var["mea
+000050a0: 6e5f 636f 756e 7473 225d 203e 3d20 6d69  n_counts"] >= mi
+000050b0: 6e5f 6d65 616e 0d0a 2020 2020 2020 2020  n_mean..        
+000050c0: 2320 6d69 6e5f 7363 6f72 6520 6669 6c74  # min_score filt
+000050d0: 6572 0d0a 2020 2020 2020 2020 6966 206d  er..        if m
+000050e0: 696e 5f73 636f 7265 2069 7320 6e6f 7420  in_score is not 
+000050f0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00005100: 2020 2073 656c 6563 7465 645f 6765 6e65     selected_gene
+00005110: 7320 3d20 7365 6c65 6374 6564 5f67 656e  s = selected_gen
+00005120: 6573 2026 2028 7365 6c66 2e61 6461 7461  es & (self.adata
+00005130: 2e76 6172 5b6f 7665 7264 6973 7065 7273  .var[overdispers
+00005140: 696f 6e5f 6d65 7472 6963 5d20 3e3d 206d  ion_metric] >= m
+00005150: 696e 5f73 636f 7265 290d 0a20 2020 2020  in_score)..     
+00005160: 2020 2023 2074 6f70 5f6e 2066 696c 7465     # top_n filte
+00005170: 720d 0a20 2020 2020 2020 2069 6620 746f  r..        if to
+00005180: 705f 6e20 6973 206e 6f74 204e 6f6e 653a  p_n is not None:
+00005190: 0d0a 2020 2020 2020 2020 2020 2020 6765  ..            ge
+000051a0: 6e65 7320 3d20 7365 6c66 2e61 6461 7461  nes = self.adata
+000051b0: 2e76 6172 5b6f 7665 7264 6973 7065 7273  .var[overdispers
+000051c0: 696f 6e5f 6d65 7472 6963 5d2e 736f 7274  ion_metric].sort
+000051d0: 5f76 616c 7565 7328 6173 6365 6e64 696e  _values(ascendin
+000051e0: 673d 4661 6c73 6529 2e68 6561 6428 696e  g=False).head(in
+000051f0: 7428 746f 705f 6e29 292e 696e 6465 780d  t(top_n)).index.
+00005200: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00005210: 6563 7465 645f 6765 6e65 7320 3d20 7365  ected_genes = se
+00005220: 6c65 6374 6564 5f67 656e 6573 2026 2073  lected_genes & s
+00005230: 656c 662e 6164 6174 612e 7661 722e 696e  elf.adata.var.in
+00005240: 6465 782e 6973 696e 2867 656e 6573 290d  dex.isin(genes).
+00005250: 0a20 2020 2020 2020 2023 2071 7561 6e74  .        # quant
+00005260: 696c 6520 6669 6c74 6572 0d0a 2020 2020  ile filter..    
+00005270: 2020 2020 6966 2071 7561 6e74 696c 6520      if quantile 
+00005280: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+00005290: 2020 2020 2020 2020 2020 6e5f 746f 7461            n_tota
+000052a0: 6c5f 6765 6e65 7320 3d20 7365 6c66 2e61  l_genes = self.a
+000052b0: 6461 7461 2e76 6172 5b6f 7665 7264 6973  data.var[overdis
+000052c0: 7065 7273 696f 6e5f 6d65 7472 6963 5d2e  persion_metric].
+000052d0: 6e6f 746e 756c 6c28 292e 7375 6d28 290d  notnull().sum().
+000052e0: 0a20 2020 2020 2020 2020 2020 2067 656e  .            gen
+000052f0: 6573 203d 2073 656c 662e 6164 6174 612e  es = self.adata.
+00005300: 7661 725b 6f76 6572 6469 7370 6572 7369  var[overdispersi
+00005310: 6f6e 5f6d 6574 7269 635d 2e73 6f72 745f  on_metric].sort_
+00005320: 7661 6c75 6573 2861 7363 656e 6469 6e67  values(ascending
+00005330: 3d46 616c 7365 292e 6865 6164 2869 6e74  =False).head(int
+00005340: 2871 7561 6e74 696c 6520 2a20 6e5f 746f  (quantile * n_to
+00005350: 7461 6c5f 6765 6e65 7329 292e 696e 6465  tal_genes)).inde
+00005360: 780d 0a20 2020 2020 2020 2020 2020 2073  x..            s
+00005370: 656c 6563 7465 645f 6765 6e65 7320 3d20  elected_genes = 
+00005380: 7365 6c65 6374 6564 5f67 656e 6573 2026  selected_genes &
+00005390: 2073 656c 662e 6164 6174 612e 7661 722e   self.adata.var.
+000053a0: 696e 6465 782e 6973 696e 2867 656e 6573  index.isin(genes
+000053b0: 290d 0a0d 0a20 2020 2020 2020 206e 5f73  )....        n_s
+000053c0: 656c 6563 7465 645f 6765 6e65 7320 3d20  elected_genes = 
+000053d0: 7365 6c65 6374 6564 5f67 656e 6573 2e73  selected_genes.s
+000053e0: 756d 2829 0d0a 2020 2020 2020 2020 6c6f  um()..        lo
+000053f0: 6767 696e 672e 696e 666f 2866 227b 6e5f  gging.info(f"{n_
+00005400: 7365 6c65 6374 6564 5f67 656e 6573 7d20  selected_genes} 
+00005410: 6765 6e65 7320 7365 6c65 6374 6564 2066  genes selected f
+00005420: 6f72 2066 6163 746f 7269 7a61 7469 6f6e  or factorization
+00005430: 2229 0d0a 2020 2020 2020 2020 0d0a 2020  ")..        ..  
+00005440: 2020 2020 2020 2320 6d61 6b65 2063 6861        # make cha
+00005450: 6e67 6573 2074 6f20 4461 7461 7365 7420  nges to Dataset 
+00005460: 6f62 6a65 6374 0d0a 2020 2020 2020 2020  object..        
+00005470: 7365 6c66 2e61 6461 7461 2e76 6172 5b22  self.adata.var["
+00005480: 7365 6c65 6374 6564 225d 203d 2073 656c  selected"] = sel
+00005490: 6563 7465 645f 6765 6e65 730d 0a20 2020  ected_genes..   
+000054a0: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
+000054b0: 756e 735b 226f 6467 225d 5b22 6f76 6572  uns["odg"]["over
+000054c0: 6469 7370 6572 7369 6f6e 5f6d 6574 7269  dispersion_metri
+000054d0: 6322 5d20 3d20 6f76 6572 6469 7370 6572  c"] = overdisper
+000054e0: 7369 6f6e 5f6d 6574 7269 630d 0a20 2020  sion_metric..   
+000054f0: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
+00005500: 756e 735b 226f 6467 225d 5b22 6d69 6e5f  uns["odg"]["min_
+00005510: 6d65 616e 225d 203d 206d 696e 5f6d 6561  mean"] = min_mea
+00005520: 6e0d 0a20 2020 2020 2020 2073 656c 662e  n..        self.
+00005530: 6164 6174 612e 756e 735b 226f 6467 225d  adata.uns["odg"]
+00005540: 5b22 6d69 6e5f 7363 6f72 6522 5d20 3d20  ["min_score"] = 
+00005550: 6d69 6e5f 7363 6f72 6520 6966 206d 696e  min_score if min
+00005560: 5f73 636f 7265 2069 7320 6e6f 7420 4e6f  _score is not No
+00005570: 6e65 2065 6c73 6520 2222 0d0a 2020 2020  ne else ""..    
+00005580: 2020 2020 7365 6c66 2e61 6461 7461 2e75      self.adata.u
+00005590: 6e73 5b22 6f64 6722 5d5b 2274 6f70 5f6e  ns["odg"]["top_n
+000055a0: 225d 203d 2074 6f70 5f6e 2069 6620 746f  "] = top_n if to
+000055b0: 705f 6e20 6973 206e 6f74 204e 6f6e 6520  p_n is not None 
+000055c0: 656c 7365 2022 220d 0a20 2020 2020 2020  else ""..       
+000055d0: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
+000055e0: 226f 6467 225d 5b22 7175 616e 7469 6c65  "odg"]["quantile
+000055f0: 225d 203d 2071 7561 6e74 696c 6520 6966  "] = quantile if
+00005600: 2071 7561 6e74 696c 6520 6973 206e 6f74   quantile is not
+00005610: 204e 6f6e 6520 656c 7365 2022 220d 0a20   None else "".. 
+00005620: 2020 2020 2020 2073 656c 662e 6170 7065         self.appe
+00005630: 6e64 5f74 6f5f 6869 7374 6f72 7928 224f  nd_to_history("O
+00005640: 7665 7264 6973 7065 7273 6564 2067 656e  verdispersed gen
+00005650: 6573 2073 656c 6563 7465 6422 290d 0a20  es selected").. 
+00005660: 2020 200d 0a20 2020 2064 6566 2069 6e69     ..    def ini
+00005670: 7469 616c 697a 655f 636e 6d66 2873 656c  tialize_cnmf(sel
+00005680: 662c 2063 6e6d 665f 6f75 7470 7574 5f64  f, cnmf_output_d
+00005690: 6972 3a20 7374 722c 0d0a 2020 2020 2020  ir: str,..      
+000056a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056b0: 2020 636e 6d66 5f6e 616d 653a 2073 7472    cnmf_name: str
+000056c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000056d0: 2020 2020 2020 2020 2020 206b 7661 6c73             kvals
+000056e0: 3a20 436f 6c6c 6563 7469 6f6e 203d 2072  : Collection = r
+000056f0: 616e 6765 2832 2c20 3631 292c 0d0a 2020  ange(2, 61),..  
+00005700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005710: 2020 2020 2020 6e5f 6974 6572 3a20 696e        n_iter: in
+00005720: 7420 3d20 3230 302c 0d0a 2020 2020 2020  t = 200,..      
+00005730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005740: 2020 6265 7461 5f6c 6f73 733a 2073 7472    beta_loss: str
+00005750: 203d 2022 6b75 6c6c 6261 636b 2d6c 6569   = "kullback-lei
+00005760: 626c 6572 222c 0d0a 2020 2020 2020 2020  bler",..        
+00005770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005780: 7365 6564 3a20 4f70 7469 6f6e 616c 5b69  seed: Optional[i
+00005790: 6e74 5d20 3d20 4e6f 6e65 2920 2d3e 2063  nt] = None) -> c
+000057a0: 6e6d 662e 634e 4d46 3a0d 0a20 2020 2020  nmf.cNMF:..     
+000057b0: 2020 2022 2222 496e 6974 6961 6c69 7a65     """Initialize
+000057c0: 2061 2063 4e4d 4620 7275 6e20 666f 7220   a cNMF run for 
+000057d0: 7375 6273 6571 7565 6e74 2066 6163 746f  subsequent facto
+000057e0: 7269 7a61 7469 6f6e 2e0d 0a0d 0a20 2020  rization.....   
+000057f0: 2020 2020 203a 7061 7261 6d20 636e 6d66       :param cnmf
+00005800: 5f6f 7574 7075 745f 6469 723a 204f 7574  _output_dir: Out
+00005810: 7075 7420 6469 7265 6374 6f72 7920 666f  put directory fo
+00005820: 7220 634e 4d46 2072 6573 756c 7473 0d0a  r cNMF results..
+00005830: 2020 2020 2020 2020 3a74 7970 6520 636e          :type cn
+00005840: 6d66 5f6f 7574 7075 745f 6469 723a 2073  mf_output_dir: s
+00005850: 7472 0d0a 2020 2020 2020 2020 3a70 6172  tr..        :par
+00005860: 616d 2063 6e6d 665f 6e61 6d65 3a20 4e61  am cnmf_name: Na
+00005870: 6d65 206f 6620 7468 6520 634e 4d46 2072  me of the cNMF r
+00005880: 6573 756c 7473 2e20 4669 6c65 7320 7769  esults. Files wi
+00005890: 6c6c 2062 6520 6f75 7470 7574 2074 6f20  ll be output to 
+000058a0: 5b63 6e6d 665f 6f75 7470 7574 5f64 6972  [cnmf_output_dir
+000058b0: 5d2f 5b63 6e6d 665f 6e61 6d65 5d2f 0d0a  ]/[cnmf_name]/..
+000058c0: 2020 2020 2020 2020 3a74 7970 6520 636e          :type cn
+000058d0: 6d66 5f6e 616d 653a 2073 7472 0d0a 2020  mf_name: str..  
+000058e0: 2020 2020 2020 3a70 6172 616d 206b 7661        :param kva
+000058f0: 6c73 3a20 5261 6e6b 7320 666f 7220 634e  ls: Ranks for cN
+00005900: 4d46 2066 6163 746f 7269 7a61 7469 6f6e  MF factorization
+00005910: 2c20 6465 6661 756c 7473 2074 6f20 7261  , defaults to ra
+00005920: 6e67 6528 322c 2036 3129 0d0a 2020 2020  nge(2, 61)..    
+00005930: 2020 2020 3a74 7970 6520 6b76 616c 733a      :type kvals:
+00005940: 2043 6f6c 6c65 6374 696f 6e2c 206f 7074   Collection, opt
+00005950: 696f 6e61 6c0d 0a20 2020 2020 2020 203a  ional..        :
+00005960: 7061 7261 6d20 6e5f 6974 6572 3a20 4e75  param n_iter: Nu
+00005970: 6d62 6572 206f 6620 6974 6572 6174 696f  mber of iteratio
+00005980: 6e73 2066 726f 6d20 7768 6963 6820 746f  ns from which to
+00005990: 2062 7569 6c64 2061 2063 6f6e 7365 6e73   build a consens
+000059a0: 7573 2073 6f6c 7574 696f 6e2c 2064 6566  us solution, def
+000059b0: 6175 6c74 7320 746f 2032 3030 0d0a 2020  aults to 200..  
+000059c0: 2020 2020 2020 3a74 7970 6520 6e5f 6974        :type n_it
+000059d0: 6572 3a20 696e 742c 206f 7074 696f 6e61  er: int, optiona
+000059e0: 6c0d 0a20 2020 2020 2020 203a 7061 7261  l..        :para
+000059f0: 6d20 6265 7461 5f6c 6f73 733a 2062 6574  m beta_loss: bet
+00005a00: 612d 6c6f 7373 2066 756e 6374 696f 6e2c  a-loss function,
+00005a10: 2065 6974 6865 7220 226b 756c 6c62 6163   either "kullbac
+00005a20: 6b2d 6c65 6962 6c65 7222 206f 7220 2266  k-leibler" or "f
+00005a30: 726f 6265 6e69 7573 222e 2044 6566 6175  robenius". Defau
+00005a40: 6c74 7320 746f 2022 6b75 6c6c 6261 636b  lts to "kullback
+00005a50: 2d6c 6569 626c 6572 220d 0a20 2020 2020  -leibler"..     
+00005a60: 2020 203a 7479 7065 2062 6574 615f 6c6f     :type beta_lo
+00005a70: 7373 3a20 7374 722c 206f 7074 696f 6e61  ss: str, optiona
+00005a80: 6c0d 0a20 2020 2020 2020 203a 7061 7261  l..        :para
+00005a90: 6d20 7365 6564 3a20 5261 6e64 6f6d 2073  m seed: Random s
+00005aa0: 6565 6420 666f 7220 7265 7072 6f64 7563  eed for reproduc
+00005ab0: 6962 696c 6974 792c 2064 6566 6175 6c74  ibility, default
+00005ac0: 7320 746f 204e 6f6e 650d 0a20 2020 2020  s to None..     
+00005ad0: 2020 203a 7479 7065 2073 6565 643a 204f     :type seed: O
+00005ae0: 7074 696f 6e61 6c5b 696e 745d 2c20 6f70  ptional[int], op
+00005af0: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
+00005b00: 3a72 6574 7572 6e3a 2063 4e4d 4620 6f62  :return: cNMF ob
+00005b10: 6a65 6374 0d0a 2020 2020 2020 2020 3a72  ject..        :r
+00005b20: 7479 7065 3a20 3a63 6c61 7373 3a60 636e  type: :class:`cn
+00005b30: 6d66 736e 732e 636e 6d66 2e63 4e4d 4660  mfsns.cnmf.cNMF`
+00005b40: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00005b50: 2020 2020 2020 2063 6e6d 665f 6f62 6a20         cnmf_obj 
+00005b60: 3d20 636e 6d66 2e63 4e4d 4628 6f75 7470  = cnmf.cNMF(outp
+00005b70: 7574 5f64 6972 3d63 6e6d 665f 6f75 7470  ut_dir=cnmf_outp
+00005b80: 7574 5f64 6972 2c20 6e61 6d65 3d63 6e6d  ut_dir, name=cnm
+00005b90: 665f 6e61 6d65 290d 0a20 2020 2020 2020  f_name)..       
+00005ba0: 200d 0a20 2020 2020 2020 2023 2077 7269   ..        # wri
+00005bb0: 7465 2054 504d 2028 6e6f 726d 616c 697a  te TPM (normaliz
+00005bc0: 6564 2920 6461 7461 0d0a 2020 2020 2020  ed) data..      
+00005bd0: 2020 7470 6d20 3d20 6164 2e41 6e6e 4461    tpm = ad.AnnDa
+00005be0: 7461 2873 656c 662e 746f 5f64 6628 6e6f  ta(self.to_df(no
+00005bf0: 726d 616c 697a 6564 3d54 7275 6529 290d  rmalized=True)).
+00005c00: 0a20 2020 2020 2020 2074 706d 2e77 7269  .        tpm.wri
+00005c10: 7465 5f68 3561 6428 636e 6d66 5f6f 626a  te_h5ad(cnmf_obj
+00005c20: 2e70 6174 6873 5b22 7470 6d22 5d29 0d0a  .paths["tpm"])..
+00005c30: 0d0a 2020 2020 2020 2020 6765 6e65 5f74  ..        gene_t
+00005c40: 706d 5f6d 6561 6e20 3d20 6e70 2e61 7272  pm_mean = np.arr
+00005c50: 6179 2874 706d 2e58 2e6d 6561 6e28 6178  ay(tpm.X.mean(ax
+00005c60: 6973 3d30 2929 2e72 6573 6861 7065 282d  is=0)).reshape(-
+00005c70: 3129 0d0a 2020 2020 2020 2020 6765 6e65  1)..        gene
+00005c80: 5f74 706d 5f73 7464 6465 7620 3d20 6e70  _tpm_stddev = np
+00005c90: 2e61 7272 6179 2874 706d 2e58 2e73 7464  .array(tpm.X.std
+00005ca0: 2861 7869 733d 302c 2064 646f 663d 3029  (axis=0, ddof=0)
+00005cb0: 292e 7265 7368 6170 6528 2d31 290d 0a20  ).reshape(-1).. 
+00005cc0: 2020 2020 2020 2069 6e70 7574 5f74 706d         input_tpm
+00005cd0: 5f73 7461 7473 203d 2070 642e 4461 7461  _stats = pd.Data
+00005ce0: 4672 616d 6528 5b67 656e 655f 7470 6d5f  Frame([gene_tpm_
+00005cf0: 6d65 616e 2c20 6765 6e65 5f74 706d 5f73  mean, gene_tpm_s
+00005d00: 7464 6465 765d 2c20 696e 6465 7820 3d20  tddev], index = 
+00005d10: 5b27 5f5f 6d65 616e 272c 2027 5f5f 7374  ['__mean', '__st
+00005d20: 6427 5d29 2e54 0d0a 2020 2020 2020 2020  d']).T..        
+00005d30: 7574 696c 732e 7361 7665 5f64 665f 746f  utils.save_df_to
+00005d40: 5f6e 707a 2869 6e70 7574 5f74 706d 5f73  _npz(input_tpm_s
+00005d50: 7461 7473 2c20 636e 6d66 5f6f 626a 2e70  tats, cnmf_obj.p
+00005d60: 6174 6873 5b27 7470 6d5f 7374 6174 7327  aths['tpm_stats'
+00005d70: 5d29 0d0a 2020 2020 2020 2020 6f76 6572  ])..        over
+00005d80: 6469 7370 6572 7365 645f 6765 6e65 7320  dispersed_genes 
+00005d90: 3d20 7365 6c66 2e61 6461 7461 2e76 6172  = self.adata.var
+00005da0: 5b22 7365 6c65 6374 6564 225d 5b73 656c  ["selected"][sel
+00005db0: 662e 6164 6174 612e 7661 725b 2273 656c  f.adata.var["sel
+00005dc0: 6563 7465 6422 5d5d 2e69 6e64 6578 0d0a  ected"]].index..
+00005dd0: 2020 2020 2020 2020 6e6f 726d 5f63 6f75          norm_cou
+00005de0: 6e74 7320 3d20 636e 6d66 5f6f 626a 2e67  nts = cnmf_obj.g
+00005df0: 6574 5f6e 6f72 6d5f 636f 756e 7473 2873  et_norm_counts(s
+00005e00: 656c 662e 6164 6174 612c 2074 706d 2c20  elf.adata, tpm, 
+00005e10: 6869 6768 5f76 6172 6961 6e63 655f 6765  high_variance_ge
+00005e20: 6e65 735f 6669 6c74 6572 3d6f 7665 7264  nes_filter=overd
+00005e30: 6973 7065 7273 6564 5f67 656e 6573 290d  ispersed_genes).
+00005e40: 0a20 2020 2020 2020 2069 6620 6e6f 726d  .        if norm
+00005e50: 5f63 6f75 6e74 732e 582e 6474 7970 6520  _counts.X.dtype 
+00005e60: 213d 206e 702e 666c 6f61 7436 343a 0d0a  != np.float64:..
+00005e70: 2020 2020 2020 2020 2020 2020 6e6f 726d              norm
+00005e80: 5f63 6f75 6e74 732e 5820 3d20 6e6f 726d  _counts.X = norm
+00005e90: 5f63 6f75 6e74 732e 582e 6173 7479 7065  _counts.X.astype
+00005ea0: 286e 702e 666c 6f61 7436 3429 0d0a 2020  (np.float64)..  
+00005eb0: 2020 2020 2020 636e 6d66 5f6f 626a 2e73        cnmf_obj.s
+00005ec0: 6176 655f 6e6f 726d 5f63 6f75 6e74 7328  ave_norm_counts(
+00005ed0: 6e6f 726d 5f63 6f75 6e74 7329 0d0a 0d0a  norm_counts)....
+00005ee0: 2020 2020 2020 2020 2320 7361 7665 2070          # save p
+00005ef0: 6172 616d 6574 6572 7320 666f 7220 6661  arameters for fa
+00005f00: 6374 6f72 697a 6174 696f 6e20 7374 6570  ctorization step
+00005f10: 0d0a 2020 2020 2020 2020 636e 6d66 5f6f  ..        cnmf_o
+00005f20: 626a 2e73 6176 655f 6e6d 665f 6974 6572  bj.save_nmf_iter
+00005f30: 5f70 6172 616d 7328 2a63 6e6d 665f 6f62  _params(*cnmf_ob
+00005f40: 6a2e 6765 745f 6e6d 665f 6974 6572 5f70  j.get_nmf_iter_p
+00005f50: 6172 616d 7328 6b73 3d6b 7661 6c73 2c20  arams(ks=kvals, 
+00005f60: 6e5f 6974 6572 3d6e 5f69 7465 722c 2072  n_iter=n_iter, r
+00005f70: 616e 646f 6d5f 7374 6174 655f 7365 6564  andom_state_seed
+00005f80: 3d73 6565 642c 2062 6574 615f 6c6f 7373  =seed, beta_loss
+00005f90: 3d62 6574 615f 6c6f 7373 2929 0d0a 0d0a  =beta_loss))....
+00005fa0: 2020 2020 2020 2020 2320 7361 7665 2070          # save p
+00005fb0: 6172 616d 6574 6572 7320 696e 2041 6e6e  arameters in Ann
+00005fc0: 4461 7461 206f 626a 6563 740d 0a20 2020  Data object..   
+00005fd0: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
+00005fe0: 756e 735b 2263 6e6d 6622 5d20 3d20 636e  uns["cnmf"] = cn
+00005ff0: 6d66 5f6f 626a 2e67 6574 5f6e 6d66 5f69  mf_obj.get_nmf_i
+00006000: 7465 725f 7061 7261 6d73 286b 733d 6b76  ter_params(ks=kv
+00006010: 616c 732c 206e 5f69 7465 723d 6e5f 6974  als, n_iter=n_it
+00006020: 6572 2c20 7261 6e64 6f6d 5f73 7461 7465  er, random_state
+00006030: 5f73 6565 643d 7365 6564 2c20 6265 7461  _seed=seed, beta
+00006040: 5f6c 6f73 733d 6265 7461 5f6c 6f73 7329  _loss=beta_loss)
+00006050: 5b31 5d20 2023 2064 6963 7420 6f66 2063  [1]  # dict of c
+00006060: 6e6d 6620 7061 7261 6d65 7465 7273 0d0a  nmf parameters..
+00006070: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00006080: 2020 7365 6c66 2e61 7070 656e 645f 746f    self.append_to
+00006090: 5f68 6973 746f 7279 2866 2263 4e4d 4620  _history(f"cNMF 
+000060a0: 7061 7261 6d65 7465 7273 2061 6464 6564  parameters added
+000060b0: 2e20 634e 4d46 2069 6e70 7574 7320 696e  . cNMF inputs in
+000060c0: 6974 6961 6c69 7a65 6420 696e 207b 636e  itialized in {cn
+000060d0: 6d66 5f6f 7574 7075 745f 6469 727d 2f7b  mf_output_dir}/{
+000060e0: 636e 6d66 5f6e 616d 657d 2229 0d0a 2020  cnmf_name}")..  
+000060f0: 2020 2020 2020 7265 7475 726e 2063 6e6d        return cnm
+00006100: 665f 6f62 6a0d 0a20 2020 200d 0a20 2020  f_obj..    ..   
+00006110: 2064 6566 2061 6464 5f63 6e6d 665f 7265   def add_cnmf_re
+00006120: 7375 6c74 7328 7365 6c66 2c20 636e 6d66  sults(self, cnmf
+00006130: 5f6f 7574 7075 745f 6469 722c 2063 6e6d  _output_dir, cnm
+00006140: 665f 6e61 6d65 2c20 6c6f 6361 6c5f 6465  f_name, local_de
+00006150: 6e73 6974 795f 7468 7265 7368 6f6c 643a  nsity_threshold:
+00006160: 2066 6c6f 6174 203d 204e 6f6e 652c 206c   float = None, l
+00006170: 6f63 616c 5f6e 6569 6768 626f 7268 6f6f  ocal_neighborhoo
+00006180: 645f 7369 7a65 3a20 666c 6f61 7420 3d20  d_size: float = 
+00006190: 4e6f 6e65 293a 0d0a 2020 2020 2020 2020  None):..        
+000061a0: 2222 220d 0a20 2020 2020 2020 2041 6674  """..        Aft
+000061b0: 6572 2066 6163 746f 7269 7a61 7469 6f6e  er factorization
+000061c0: 2c20 6164 6420 636f 6d70 6c65 7465 6420  , add completed 
+000061d0: 634e 4d46 2072 6573 756c 7473 2069 6e20  cNMF results in 
+000061e0: 5b63 6e6d 665f 6f75 7470 7574 5f64 6972  [cnmf_output_dir
+000061f0: 5d2f 5b63 6e6d 665f 6e61 6d65 5d20 746f  ]/[cnmf_name] to
+00006200: 2074 6865 2064 6174 6173 6574 206f 626a   the dataset obj
+00006210: 6563 742e 0d0a 0d0a 2020 2020 2020 2020  ect.....        
+00006220: 3a70 6172 616d 2063 6e6d 665f 6f75 7470  :param cnmf_outp
+00006230: 7574 5f64 6972 3a20 4f75 7470 7574 2064  ut_dir: Output d
+00006240: 6972 6563 746f 7279 2066 6f72 2063 4e4d  irectory for cNM
+00006250: 4620 7265 7375 6c74 730d 0a20 2020 2020  F results..     
+00006260: 2020 203a 7479 7065 2063 6e6d 665f 6f75     :type cnmf_ou
+00006270: 7470 7574 5f64 6972 3a20 7374 720d 0a20  tput_dir: str.. 
+00006280: 2020 2020 2020 203a 7061 7261 6d20 636e         :param cn
+00006290: 6d66 5f6e 616d 653a 204e 616d 6520 6f66  mf_name: Name of
+000062a0: 2074 6865 2063 4e4d 4620 7265 7375 6c74   the cNMF result
+000062b0: 732e 2046 696c 6573 2077 696c 6c20 6265  s. Files will be
+000062c0: 206f 7574 7075 7420 746f 205b 636e 6d66   output to [cnmf
+000062d0: 5f6f 7574 7075 745f 6469 725d 2f5b 636e  _output_dir]/[cn
+000062e0: 6d66 5f6e 616d 655d 2f0d 0a20 2020 2020  mf_name]/..     
+000062f0: 2020 203a 7479 7065 2063 6e6d 665f 6e61     :type cnmf_na
+00006300: 6d65 3a20 7374 720d 0a20 2020 2020 2020  me: str..       
+00006310: 203a 7061 7261 6d20 6c6f 6361 6c5f 6465   :param local_de
+00006320: 6e73 6974 795f 7468 7265 7368 6f6c 643a  nsity_threshold:
+00006330: 2054 6872 6573 686f 6c64 2066 6f72 2074   Threshold for t
+00006340: 6865 206c 6f63 616c 2064 656e 7369 7479  he local density
+00006350: 2066 696c 7465 7269 6e67 2070 7269 6f72   filtering prior
+00006360: 2074 6f20 4745 5020 636f 6e73 656e 7375   to GEP consensu
+00006370: 732e 2041 6363 6570 7461 626c 6520 7468  s. Acceptable th
+00006380: 7265 7368 6f6c 6473 2061 7265 203e 2030  resholds are > 0
+00006390: 2061 6e64 203c 3d20 3220 2832 2e30 2069   and <= 2 (2.0 i
+000063a0: 7320 6e6f 2066 696c 7465 7269 6e67 292e  s no filtering).
+000063b0: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
+000063c0: 652e 0d0a 2020 2020 2020 2020 3a74 7970  e...        :typ
+000063d0: 6520 6c6f 6361 6c5f 6465 6e73 6974 795f  e local_density_
+000063e0: 7468 7265 7368 6f6c 643a 2066 6c6f 6174  threshold: float
+000063f0: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
+00006400: 2020 2020 3a70 6172 616d 206c 6f63 616c      :param local
+00006410: 5f6e 6569 6768 626f 7268 6f6f 645f 7369  _neighborhood_si
+00006420: 7a65 3a20 4672 6163 7469 6f6e 206f 6620  ze: Fraction of 
+00006430: 7468 6520 6e75 6d62 6572 206f 6620 7265  the number of re
+00006440: 706c 6963 6174 6573 2074 6f20 7573 6520  plicates to use 
+00006450: 6173 206e 6561 7265 7374 206e 6569 6768  as nearest neigh
+00006460: 626f 7273 2066 6f72 206c 6f63 616c 2064  bors for local d
+00006470: 656e 7369 7479 2066 696c 7465 7269 6e67  ensity filtering
+00006480: 2e20 4465 6661 756c 7473 2074 6f20 4e6f  . Defaults to No
+00006490: 6e65 0d0a 2020 2020 2020 2020 3a74 7970  ne..        :typ
+000064a0: 6520 6c6f 6361 6c5f 6e65 6967 6862 6f72  e local_neighbor
+000064b0: 686f 6f64 5f73 697a 653a 2066 6c6f 6174  hood_size: float
+000064c0: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
+000064d0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+000064e0: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
+000064f0: 2263 6e6d 665f 6e61 6d65 225d 203d 2063  "cnmf_name"] = c
+00006500: 6e6d 665f 6e61 6d65 0d0a 0d0a 2020 2020  nmf_name....    
+00006510: 2020 2020 2320 696e 6665 7220 6672 6f6d      # infer from
+00006520: 2066 696c 656e 616d 6573 2077 6869 6368   filenames which
+00006530: 206c 6f63 616c 2064 656e 7369 7479 2074   local density t
+00006540: 6872 6573 686f 6c64 2077 6173 2075 7365  hreshold was use
+00006550: 640d 0a20 2020 2020 2020 2073 656e 7365  d..        sense
+00006560: 645f 6c64 7473 203d 2073 6574 2829 0d0a  d_ldts = set()..
+00006570: 2020 2020 2020 2020 666f 7220 666e 2069          for fn i
+00006580: 6e20 676c 6f62 286f 732e 7061 7468 2e6a  n glob(os.path.j
+00006590: 6f69 6e28 636e 6d66 5f6f 7574 7075 745f  oin(cnmf_output_
+000065a0: 6469 722c 2063 6e6d 665f 6e61 6d65 2c20  dir, cnmf_name, 
+000065b0: 6622 7b63 6e6d 665f 6e61 6d65 7d2a 2e2a  f"{cnmf_name}*.*
+000065c0: 7370 6563 7472 612a 2e6b 5f2a 2229 293a  spectra*.k_*")):
+000065d0: 0d0a 2020 2020 2020 2020 2020 2020 6c64  ..            ld
+000065e0: 745f 7374 7220 3d20 6f73 2e70 6174 682e  t_str = os.path.
+000065f0: 6261 7365 6e61 6d65 2866 6e29 2e73 706c  basename(fn).spl
+00006600: 6974 2822 2e22 295b 2d33 5d0d 0a20 2020  it(".")[-3]..   
+00006610: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
+00006620: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00006630: 6474 203d 2066 6c6f 6174 286c 6474 5f73  dt = float(ldt_s
+00006640: 7472 2e72 6570 6c61 6365 2822 6474 5f22  tr.replace("dt_"
+00006650: 2c20 2222 292e 7265 706c 6163 6528 225f  , "").replace("_
+00006660: 222c 2022 2e22 2929 0d0a 2020 2020 2020  ", "."))..      
+00006670: 2020 2020 2020 6578 6365 7074 2056 616c        except Val
+00006680: 7565 4572 726f 723a 0d0a 2020 2020 2020  ueError:..      
+00006690: 2020 2020 2020 2020 2020 7061 7373 0d0a            pass..
+000066a0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000066b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000066c0: 2020 2073 656e 7365 645f 6c64 7473 2e61     sensed_ldts.a
+000066d0: 6464 2828 6c64 745f 7374 722c 206c 6474  dd((ldt_str, ldt
+000066e0: 2929 0d0a 2020 2020 2020 2020 6966 206c  ))..        if l
+000066f0: 6f63 616c 5f64 656e 7369 7479 5f74 6872  ocal_density_thr
+00006700: 6573 686f 6c64 2069 7320 4e6f 6e65 2061  eshold is None a
+00006710: 6e64 206c 656e 2873 656e 7365 645f 6c64  nd len(sensed_ld
+00006720: 7473 2920 3d3d 2031 3a0d 0a20 2020 2020  ts) == 1:..     
+00006730: 2020 2020 2020 206c 6474 5f73 7472 2c20         ldt_str, 
+00006740: 6c64 7420 3d20 7365 6e73 6564 5f6c 6474  ldt = sensed_ldt
+00006750: 732e 706f 7028 290d 0a20 2020 2020 2020  s.pop()..       
+00006760: 2065 6c69 6620 6c6f 6361 6c5f 6465 6e73   elif local_dens
+00006770: 6974 795f 7468 7265 7368 6f6c 6420 696e  ity_threshold in
+00006780: 2028 6c64 745b 315d 2066 6f72 206c 6474   (ldt[1] for ldt
+00006790: 2069 6e20 7365 6e73 6564 5f6c 6474 7329   in sensed_ldts)
+000067a0: 3a0d 0a20 2020 2020 2020 2020 2020 206c  :..            l
+000067b0: 6474 5f73 7472 2c20 6c64 7420 3d20 5b28  dt_str, ldt = [(
+000067c0: 6c64 745f 7374 722c 206c 6474 2920 666f  ldt_str, ldt) fo
+000067d0: 7220 6c64 745f 7374 722c 206c 6474 2069  r ldt_str, ldt i
+000067e0: 6e20 7365 6e73 6564 5f6c 6474 7320 6966  n sensed_ldts if
+000067f0: 206c 6474 203d 3d20 6c6f 6361 6c5f 6465   ldt == local_de
+00006800: 6e73 6974 795f 7468 7265 7368 6f6c 645d  nsity_threshold]
+00006810: 2e70 6f70 2829 0d0a 2020 2020 2020 2020  .pop()..        
+00006820: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00006830: 2020 206c 6f67 6769 6e67 2e65 7272 6f72     logging.error
+00006840: 2866 226c 6f63 616c 5f64 656e 7369 7479  (f"local_density
+00006850: 5f74 6872 6573 686f 6c64 206f 6620 7b6c  _threshold of {l
+00006860: 6f63 616c 5f64 656e 7369 7479 5f74 6872  ocal_density_thr
+00006870: 6573 686f 6c64 7d20 646f 6573 206e 6f74  eshold} does not
+00006880: 206d 6174 6368 2077 6861 7420 6973 2069   match what is i
+00006890: 6e20 7468 6520 634e 4d46 2072 6573 756c  n the cNMF resul
+000068a0: 7420 6469 7265 6374 6f72 793a 207b 7365  t directory: {se
+000068b0: 6e73 6564 5f6c 6474 737d 2229 0d0a 2020  nsed_ldts}")..  
+000068c0: 2020 2020 2020 2020 2020 7379 732e 6578            sys.ex
+000068d0: 6974 2831 290d 0a20 2020 2020 2020 2073  it(1)..        s
+000068e0: 656c 662e 6164 6174 612e 756e 735b 226c  elf.adata.uns["l
+000068f0: 6474 225d 203d 206c 6474 0d0a 2020 2020  dt"] = ldt..    
+00006900: 2020 2020 7365 6c66 2e61 6461 7461 2e75      self.adata.u
+00006910: 6e73 5b22 6c6e 7322 5d20 3d20 6c6f 6361  ns["lns"] = loca
+00006920: 6c5f 6e65 6967 6862 6f72 686f 6f64 5f73  l_neighborhood_s
+00006930: 697a 650d 0a20 2020 2020 2020 2020 2020  ize..           
+00006940: 200d 0a20 2020 2020 2020 2023 2049 6d70   ..        # Imp
+00006950: 6f72 7420 4745 5073 0d0a 2020 2020 2020  ort GEPs..      
+00006960: 2020 7265 7375 6c74 5f74 7970 6573 203d    result_types =
+00006970: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00006980: 2267 656e 655f 7370 6563 7472 615f 7363  "gene_spectra_sc
+00006990: 6f72 6522 3a20 2263 6e6d 665f 6765 705f  ore": "cnmf_gep_
+000069a0: 7363 6f72 6522 2c0d 0a20 2020 2020 2020  score",..       
+000069b0: 2020 2020 2022 6765 6e65 5f73 7065 6374       "gene_spect
+000069c0: 7261 5f74 706d 223a 2022 636e 6d66 5f67  ra_tpm": "cnmf_g
+000069d0: 6570 5f74 706d 222c 0d0a 2020 2020 2020  ep_tpm",..      
+000069e0: 2020 2020 2020 2273 7065 6374 7261 223a        "spectra":
+000069f0: 2022 636e 6d66 5f67 6570 5f72 6177 220d   "cnmf_gep_raw".
+00006a00: 0a20 2020 2020 2020 2020 2020 207d 0d0a  .            }..
+00006a10: 2020 2020 2020 2020 666f 7220 6d61 7463          for matc
+00006a20: 6873 7472 2c20 7265 7375 6c74 5f74 7970  hstr, result_typ
+00006a30: 6520 696e 2072 6573 756c 745f 7479 7065  e in result_type
+00006a40: 732e 6974 656d 7328 293a 0d0a 2020 2020  s.items():..    
+00006a50: 2020 2020 2020 2020 6c6f 6767 696e 672e          logging.
+00006a60: 696e 666f 2866 2249 6d70 6f72 7469 6e67  info(f"Importing
+00006a70: 2047 4550 733a 207b 6d61 7463 6873 7472   GEPs: {matchstr
+00006a80: 7d22 2920 200d 0a20 2020 2020 2020 2020  }")  ..         
+00006a90: 2020 206d 6574 615f 7720 3d20 5b5d 0d0a     meta_w = []..
+00006aa0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00006ab0: 666e 2069 6e20 676c 6f62 286f 732e 7061  fn in glob(os.pa
+00006ac0: 7468 2e6a 6f69 6e28 636e 6d66 5f6f 7574  th.join(cnmf_out
+00006ad0: 7075 745f 6469 722c 2063 6e6d 665f 6e61  put_dir, cnmf_na
+00006ae0: 6d65 2c20 6622 7b63 6e6d 665f 6e61 6d65  me, f"{cnmf_name
+00006af0: 7d2a 2e7b 6d61 7463 6873 7472 7d2e 6b5f  }*.{matchstr}.k_
+00006b00: 2a2e 7b6c 6474 5f73 7472 7d2e 2a74 7874  *.{ldt_str}.*txt
+00006b10: 2229 293a 0d0a 2020 2020 2020 2020 2020  ")):..          
+00006b20: 2020 2020 2020 6b20 3d20 696e 7428 6f73        k = int(os
+00006b30: 2e70 6174 682e 6261 7365 6e61 6d65 2866  .path.basename(f
+00006b40: 6e29 2e72 656d 6f76 6570 7265 6669 7828  n).removeprefix(
+00006b50: 6622 7b63 6e6d 665f 6e61 6d65 7d2e 7b6d  f"{cnmf_name}.{m
+00006b60: 6174 6368 7374 727d 2e22 292e 7370 6c69  atchstr}.").spli
+00006b70: 7428 222e 2229 5b30 5d2e 7265 706c 6163  t(".")[0].replac
+00006b80: 6528 226b 5f22 2c20 2222 2929 0d0a 2020  e("k_", ""))..  
+00006b90: 2020 2020 2020 2020 2020 2020 2020 7720                w 
+00006ba0: 3d20 7064 2e72 6561 645f 7461 626c 6528  = pd.read_table(
+00006bb0: 666e 2c20 696e 6465 785f 636f 6c3d 3029  fn, index_col=0)
+00006bc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006bd0: 2020 772e 696e 6465 7820 3d20 7374 7228    w.index = str(
+00006be0: 6b29 202b 2022 2e22 202b 2077 2e69 6e64  k) + "." + w.ind
+00006bf0: 6578 2e61 7374 7970 6528 7374 7229 0d0a  ex.astype(str)..
+00006c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c10: 6d65 7461 5f77 2e61 7070 656e 6428 7729  meta_w.append(w)
+00006c20: 0d0a 2020 2020 2020 2020 2020 2020 6d65  ..            me
+00006c30: 7461 5f77 203d 2070 642e 636f 6e63 6174  ta_w = pd.concat
+00006c40: 286d 6574 615f 772c 2061 7869 733d 3029  (meta_w, axis=0)
+00006c50: 2e54 2e72 6569 6e64 6578 2873 656c 662e  .T.reindex(self.
+00006c60: 6164 6174 612e 7661 722e 696e 6465 7829  adata.var.index)
+00006c70: 2e72 656e 616d 655f 6178 6973 285b 226b  .rename_axis(["k
+00006c80: 2e67 6570 225d 2c20 6178 6973 3d31 290d  .gep"], axis=1).
+00006c90: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00006ca0: 662e 6164 6174 612e 7661 726d 5b72 6573  f.adata.varm[res
+00006cb0: 756c 745f 7479 7065 5d20 3d20 6d65 7461  ult_type] = meta
+00006cc0: 5f77 0d0a 0d0a 2020 2020 2020 2020 2320  _w....        # 
+00006cd0: 496d 706f 7274 2055 7361 6765 730d 0a20  Import Usages.. 
+00006ce0: 2020 2020 2020 206c 6f67 6769 6e67 2e69         logging.i
+00006cf0: 6e66 6f28 6622 496d 706f 7274 696e 6720  nfo(f"Importing 
+00006d00: 5573 6167 6573 2229 2020 0d0a 2020 2020  Usages")  ..    
+00006d10: 2020 2020 7573 6167 6520 3d20 5b5d 0d0a      usage = []..
+00006d20: 2020 2020 2020 2020 666f 7220 666e 2069          for fn i
+00006d30: 6e20 676c 6f62 286f 732e 7061 7468 2e6a  n glob(os.path.j
+00006d40: 6f69 6e28 636e 6d66 5f6f 7574 7075 745f  oin(cnmf_output_
+00006d50: 6469 722c 2063 6e6d 665f 6e61 6d65 2c20  dir, cnmf_name, 
+00006d60: 6622 7b63 6e6d 665f 6e61 6d65 7d2a 2e75  f"{cnmf_name}*.u
+00006d70: 7361 6765 732e 6b5f 2a2e 7b6c 6474 5f73  sages.k_*.{ldt_s
+00006d80: 7472 7d2e 2a74 7874 2229 293a 0d0a 2020  tr}.*txt")):..  
+00006d90: 2020 2020 2020 2020 2020 6b20 3d20 696e            k = in
+00006da0: 7428 6f73 2e70 6174 682e 6261 7365 6e61  t(os.path.basena
+00006db0: 6d65 2866 6e29 2e72 656d 6f76 6570 7265  me(fn).removepre
+00006dc0: 6669 7828 6622 7b63 6e6d 665f 6e61 6d65  fix(f"{cnmf_name
+00006dd0: 7d2e 7573 6167 6573 2e22 292e 7370 6c69  }.usages.").spli
+00006de0: 7428 222e 2229 5b30 5d2e 7265 706c 6163  t(".")[0].replac
+00006df0: 6528 226b 5f22 2c20 2222 2929 0d0a 2020  e("k_", ""))..  
+00006e00: 2020 2020 2020 2020 2020 6820 3d20 7064            h = pd
+00006e10: 2e72 6561 645f 7461 626c 6528 666e 2c20  .read_table(fn, 
+00006e20: 696e 6465 785f 636f 6c3d 3029 0d0a 2020  index_col=0)..  
+00006e30: 2020 2020 2020 2020 2020 682e 636f 6c75            h.colu
+00006e40: 6d6e 7320 3d20 7374 7228 6b29 202b 2022  mns = str(k) + "
+00006e50: 2e22 202b 2068 2e63 6f6c 756d 6e73 2e61  ." + h.columns.a
+00006e60: 7374 7970 6528 7374 7229 0d0a 2020 2020  stype(str)..    
+00006e70: 2020 2020 2020 2020 7573 6167 652e 6170          usage.ap
+00006e80: 7065 6e64 2868 290d 0a20 2020 2020 2020  pend(h)..       
+00006e90: 2073 656c 662e 6164 6174 612e 6f62 736d   self.adata.obsm
+00006ea0: 5b22 636e 6d66 5f75 7361 6765 225d 203d  ["cnmf_usage"] =
+00006eb0: 2070 642e 636f 6e63 6174 2875 7361 6765   pd.concat(usage
+00006ec0: 2c20 6178 6973 3d31 292e 736f 7274 5f69  , axis=1).sort_i
+00006ed0: 6e64 6578 2861 7869 733d 3129 2e72 656e  ndex(axis=1).ren
+00006ee0: 616d 655f 6178 6973 285b 226b 2e67 6570  ame_axis(["k.gep
+00006ef0: 225d 2c20 6178 6973 3d31 290d 0a20 2020  "], axis=1)..   
+00006f00: 2020 2020 200d 0a20 2020 2020 2020 2023       ..        #
+00006f10: 2049 6d70 6f72 7420 6765 6e65 206c 6973   Import gene lis
+00006f20: 7420 7573 6564 2066 6f72 2066 6163 746f  t used for facto
+00006f30: 7269 7a61 7469 6f6e 0d0a 2020 2020 2020  rization..      
+00006f40: 2020 7769 7468 206f 7065 6e28 6f73 2e70    with open(os.p
+00006f50: 6174 682e 6a6f 696e 2863 6e6d 665f 6f75  ath.join(cnmf_ou
+00006f60: 7470 7574 5f64 6972 2c20 636e 6d66 5f6e  tput_dir, cnmf_n
+00006f70: 616d 652c 2066 227b 636e 6d66 5f6e 616d  ame, f"{cnmf_nam
+00006f80: 657d 2e6f 7665 7264 6973 7065 7273 6564  e}.overdispersed
+00006f90: 5f67 656e 6573 2e74 7874 2229 2920 6173  _genes.txt")) as
+00006fa0: 2066 3a0d 0a20 2020 2020 2020 2020 2020   f:..           
+00006fb0: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
+00006fc0: 2267 656e 655f 6c69 7374 225d 203d 205b  "gene_list"] = [
+00006fd0: 6c69 6e65 2e73 7472 6970 2829 2066 6f72  line.strip() for
+00006fe0: 206c 696e 6520 696e 2066 2e72 6561 646c   line in f.readl
+00006ff0: 696e 6573 2829 5d0d 0a0d 0a20 2020 2020  ines()]....     
+00007000: 2020 2023 2049 6d70 6f72 7420 4b2d 7365     # Import K-se
+00007010: 6c65 6374 696f 6e20 7374 6174 730d 0a20  lection stats.. 
+00007020: 2020 2020 2020 206b 7661 6c73 203d 2070         kvals = p
+00007030: 642e 4461 7461 4672 616d 6528 2a2a 6e70  d.DataFrame(**np
+00007040: 2e6c 6f61 6428 6f73 2e70 6174 682e 6a6f  .load(os.path.jo
+00007050: 696e 2863 6e6d 665f 6f75 7470 7574 5f64  in(cnmf_output_d
+00007060: 6972 2c20 636e 6d66 5f6e 616d 652c 2066  ir, cnmf_name, f
+00007070: 227b 636e 6d66 5f6e 616d 657d 2e6b 5f73  "{cnmf_name}.k_s
+00007080: 656c 6563 7469 6f6e 5f73 7461 7473 2e64  election_stats.d
+00007090: 662e 6e70 7a22 292c 2061 6c6c 6f77 5f70  f.npz"), allow_p
+000070a0: 6963 6b6c 653d 5472 7565 2929 2e73 6574  ickle=True)).set
+000070b0: 5f69 6e64 6578 2822 6b22 295b 5b22 7374  _index("k")[["st
+000070c0: 6162 696c 6974 7922 2c20 2270 7265 6469  ability", "predi
+000070d0: 6374 696f 6e5f 6572 726f 7222 5d5d 0d0a  ction_error"]]..
+000070e0: 2020 2020 2020 2020 6b76 616c 732e 696e          kvals.in
+000070f0: 6465 7820 3d20 6b76 616c 732e 696e 6465  dex = kvals.inde
+00007100: 782e 6173 7479 7065 2869 6e74 290d 0a20  x.astype(int).. 
+00007110: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
+00007120: 612e 756e 735b 226b 7661 6c73 225d 203d  a.uns["kvals"] =
+00007130: 206b 7661 6c73 0d0a 2020 2020 2020 2020   kvals..        
+00007140: 7365 6c66 2e61 7070 656e 645f 746f 5f68  self.append_to_h
+00007150: 6973 746f 7279 2822 634e 4d46 2072 6573  istory("cNMF res
+00007160: 756c 7473 2061 6464 6564 2066 726f 6d20  ults added from 
+00007170: 6f75 7470 7574 2064 6972 6563 746f 7279  output directory
+00007180: 207b 636e 6d66 5f6f 7574 7075 745f 6469   {cnmf_output_di
+00007190: 727d 2f7b 636e 6d66 5f6e 616d 657d 2229  r}/{cnmf_name}")
+000071a0: 0d0a 0d0a 2020 2020 6465 6620 6765 745f  ....    def get_
+000071b0: 7573 6167 6573 2873 656c 662c 0d0a 2020  usages(self,..  
+000071c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071d0: 206b 3a20 556e 696f 6e5b 696e 742c 2049   k: Union[int, I
+000071e0: 7465 7261 626c 655d 203d 204e 6f6e 652c  terable] = None,
+000071f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007200: 2020 2020 2064 6973 6372 6574 697a 653a       discretize:
+00007210: 2062 6f6f 6c20 3d20 4661 6c73 652c 0d0a   bool = False,..
+00007220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007230: 2020 206e 6f72 6d61 6c69 7a65 3a20 626f     normalize: bo
+00007240: 6f6c 203d 2046 616c 7365 0d0a 2020 2020  ol = False..    
+00007250: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00007260: 202d 3e20 7064 2e44 6174 6146 7261 6d65   -> pd.DataFrame
+00007270: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+00007280: 2020 2020 2020 2020 4361 6c63 756c 6174          Calculat
+00007290: 6520 7573 6167 6520 6f66 2065 6163 6820  e usage of each 
+000072a0: 4745 5020 696e 2065 6163 6820 7361 6d70  GEP in each samp
+000072b0: 6c65 2f6f 6273 6572 7661 7469 6f6e 2e0d  le/observation..
+000072c0: 0a0d 0a20 2020 2020 2020 203a 7061 7261  ...        :para
+000072d0: 6d20 6b3a 2049 6620 616e 2069 6e74 6567  m k: If an integ
+000072e0: 6572 206f 7220 6c69 7374 206f 6620 696e  er or list of in
+000072f0: 7465 6765 7273 2c20 7265 7475 726e 7320  tegers, returns 
+00007300: 7573 6167 6573 206f 6e6c 7920 666f 7220  usages only for 
+00007310: 7370 6563 6966 6965 6420 7261 6e6b 732e  specified ranks.
+00007320: 204f 7468 6572 7769 7365 2c20 7265 7475   Otherwise, retu
+00007330: 726e 7320 7573 6167 6520 6f66 2061 6c6c  rns usage of all
+00007340: 2047 4550 7320 6163 726f 7373 2072 616e   GEPs across ran
+00007350: 6b73 2e20 4465 6661 756c 7473 2074 6f20  ks. Defaults to 
+00007360: 4e6f 6e65 0d0a 2020 2020 2020 2020 3a74  None..        :t
+00007370: 7970 6520 6b3a 2069 6e74 2c20 6f70 7469  ype k: int, opti
+00007380: 6f6e 616c 0d0a 2020 2020 2020 2020 3a70  onal..        :p
+00007390: 6172 616d 2064 6973 6372 6574 697a 653a  aram discretize:
+000073a0: 2044 6973 6372 6574 697a 6573 2074 6865   Discretizes the
+000073b0: 2075 7361 6765 206d 6174 7269 7820 7375   usage matrix su
+000073c0: 6368 2074 6861 7420 666f 7220 6561 6368  ch that for each
+000073d0: 2076 616c 7565 206f 6620 6b2c 2065 6163   value of k, eac
+000073e0: 6820 7361 6d70 6c65 2068 6173 2075 7361  h sample has usa
+000073f0: 6765 206f 6620 6f6e 6c79 2031 2047 4550  ge of only 1 GEP
+00007400: 2028 7468 6520 6f6e 6520 7769 7468 2074   (the one with t
+00007410: 6865 206d 6178 696d 756d 2075 7361 6765  he maximum usage
+00007420: 292e 2044 6566 6175 6c74 7320 746f 2046  ). Defaults to F
+00007430: 616c 7365 0d0a 2020 2020 2020 2020 3a74  alse..        :t
+00007440: 7970 6520 6469 7363 7265 7469 7a65 3a20  ype discretize: 
+00007450: 626f 6f6c 2c20 6f70 7469 6f6e 616c 0d0a  bool, optional..
+00007460: 2020 2020 2020 2020 3a70 6172 616d 206e          :param n
+00007470: 6f72 6d61 6c69 7a65 3a20 4e6f 726d 616c  ormalize: Normal
+00007480: 697a 6520 7468 6520 4745 5020 7573 6167  ize the GEP usag
+00007490: 6520 6d61 7472 6978 2073 7563 6820 7468  e matrix such th
+000074a0: 6174 2066 6f72 2065 6163 6820 7661 6c75  at for each valu
+000074b0: 6520 6f66 206b 2c20 7573 6167 6520 6f66  e of k, usage of
+000074c0: 2061 6c6c 2047 4550 7320 7375 6d73 2074   all GEPs sums t
+000074d0: 6f20 312e 2044 6566 6175 6c74 7320 746f  o 1. Defaults to
+000074e0: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+000074f0: 3a74 7970 6520 6e6f 726d 616c 697a 653a  :type normalize:
+00007500: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0d   bool, optional.
+00007510: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00007520: 3a20 6f62 7365 7276 6174 696f 6e20 c397  : observation ..
+00007530: 2047 4550 206d 6174 7269 780d 0a20 2020   GEP matrix..   
+00007540: 2020 2020 203a 7274 7970 653a 2070 642e       :rtype: pd.
+00007550: 4461 7461 4672 616d 650d 0a20 2020 2020  DataFrame..     
+00007560: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00007570: 6466 203d 2073 656c 662e 6164 6174 612e  df = self.adata.
+00007580: 6f62 736d 5b22 636e 6d66 5f75 7361 6765  obsm["cnmf_usage
+00007590: 225d 2e63 6f70 7928 290d 0a20 2020 2020  "].copy()..     
+000075a0: 2020 2064 662e 636f 6c75 6d6e 7320 3d20     df.columns = 
+000075b0: 7064 2e4d 756c 7469 496e 6465 782e 6672  pd.MultiIndex.fr
+000075c0: 6f6d 5f74 7570 6c65 7328 6466 2e63 6f6c  om_tuples(df.col
+000075d0: 756d 6e73 2e73 7472 2e73 706c 6974 2822  umns.str.split("
+000075e0: 2e22 292e 746f 5f6c 6973 7428 2929 0d0a  .").to_list())..
+000075f0: 2020 2020 2020 2020 6466 2e63 6f6c 756d          df.colum
+00007600: 6e73 203d 2064 662e 636f 6c75 6d6e 732e  ns = df.columns.
+00007610: 7365 745f 6c65 7665 6c73 285b 6c2e 6173  set_levels([l.as
+00007620: 7479 7065 2822 696e 7422 2920 666f 7220  type("int") for 
+00007630: 6c20 696e 2064 662e 636f 6c75 6d6e 732e  l in df.columns.
+00007640: 6c65 7665 6c73 5d29 0d0a 2020 2020 2020  levels])..      
+00007650: 2020 6966 206e 6f72 6d61 6c69 7a65 3a0d    if normalize:.
+00007660: 0a20 2020 2020 2020 2020 2020 206e 6f72  .            nor
+00007670: 6d61 6c69 7a65 6420 3d20 5b5d 0d0a 2020  malized = []..  
+00007680: 2020 2020 2020 2020 2020 666f 7220 5f2c            for _,
+00007690: 2073 7562 6466 2069 6e20 6466 2e67 726f   subdf in df.gro
+000076a0: 7570 6279 2861 7869 733d 312c 206c 6576  upby(axis=1, lev
+000076b0: 656c 3d30 293a 0d0a 2020 2020 2020 2020  el=0):..        
+000076c0: 2020 2020 2020 2020 6e6f 726d 616c 697a          normaliz
+000076d0: 6564 2e61 7070 656e 6428 7375 6264 662e  ed.append(subdf.
+000076e0: 6469 7628 7375 6264 662e 7375 6d28 6178  div(subdf.sum(ax
+000076f0: 6973 3d31 292c 2061 7869 733d 3029 290d  is=1), axis=0)).
+00007700: 0a20 2020 2020 2020 2020 2020 2064 6620  .            df 
+00007710: 3d20 7064 2e63 6f6e 6361 7428 6e6f 726d  = pd.concat(norm
+00007720: 616c 697a 6564 2c20 6178 6973 3d31 290d  alized, axis=1).
+00007730: 0a20 2020 2020 2020 2069 6620 6469 7363  .        if disc
+00007740: 7265 7469 7a65 3a0d 0a20 2020 2020 2020  retize:..       
+00007750: 2020 2020 2064 6973 6372 6574 697a 6564       discretized
+00007760: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00007770: 2020 2066 6f72 205f 2c20 7375 6264 6620     for _, subdf 
+00007780: 696e 2064 662e 6772 6f75 7062 7928 6178  in df.groupby(ax
+00007790: 6973 3d31 2c20 6c65 7665 6c3d 3029 3a0d  is=1, level=0):.
+000077a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000077b0: 2064 6973 6372 6574 697a 6564 2e61 7070   discretized.app
+000077c0: 656e 6428 7375 6264 662e 6571 2873 7562  end(subdf.eq(sub
+000077d0: 6466 2e6d 6178 2861 7869 733d 3129 2c20  df.max(axis=1), 
+000077e0: 6178 6973 3d30 292e 6173 7479 7065 2869  axis=0).astype(i
+000077f0: 6e74 2929 0d0a 2020 2020 2020 2020 2020  nt))..          
+00007800: 2020 6466 203d 2070 642e 636f 6e63 6174    df = pd.concat
+00007810: 2864 6973 6372 6574 697a 6564 2c20 6178  (discretized, ax
+00007820: 6973 3d31 2920 2020 2020 2020 200d 0a20  is=1)        .. 
+00007830: 2020 2020 2020 2069 6620 6b20 6973 206e         if k is n
+00007840: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+00007850: 2020 2020 2020 6466 203d 2064 662e 6c6f        df = df.lo
+00007860: 635b 3a2c 206b 5d0d 0a20 2020 2020 2020  c[:, k]..       
+00007870: 2064 6620 3d20 6466 2e73 6f72 745f 696e   df = df.sort_in
+00007880: 6465 7828 6178 6973 3d30 292e 736f 7274  dex(axis=0).sort
+00007890: 5f69 6e64 6578 2861 7869 733d 3129 2020  _index(axis=1)  
+000078a0: 200d 0a20 2020 2020 2020 2072 6574 7572   ..        retur
+000078b0: 6e20 6466 0d0a 2020 2020 0d0a 2020 2020  n df..    ..    
+000078c0: 6465 6620 6765 745f 6765 7073 2873 656c  def get_geps(sel
+000078d0: 662c 0d0a 2020 2020 2020 2020 2020 2020  f,..            
+000078e0: 2020 2020 206b 3a20 556e 696f 6e5b 696e       k: Union[in
+000078f0: 742c 2049 7465 7261 626c 655d 203d 204e  t, Iterable] = N
+00007900: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
+00007910: 2020 2020 2020 2074 7970 653d 2263 6e6d         type="cnm
+00007920: 665f 6765 705f 7363 6f72 6522 0d0a 2020  f_gep_score"..  
+00007930: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00007940: 202d 3e20 7064 2e44 6174 6146 7261 6d65   -> pd.DataFrame
+00007950: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+00007960: 2020 2020 2020 2020 4765 7420 4745 5073          Get GEPs
+00007970: 2e0d 0a0d 0a20 2020 2020 2020 203a 7061  .....        :pa
+00007980: 7261 6d20 6b3a 2049 6620 616e 2069 6e74  ram k: If an int
+00007990: 6567 6572 206f 7220 6c69 7374 206f 6620  eger or list of 
+000079a0: 696e 7465 6765 7273 2c20 7265 7475 726e  integers, return
+000079b0: 7320 4745 5073 206f 6e6c 7920 666f 7220  s GEPs only for 
+000079c0: 7370 6563 6966 6965 6420 7261 6e6b 732e  specified ranks.
+000079d0: 204f 7468 6572 7769 7365 2c20 7265 7475   Otherwise, retu
+000079e0: 726e 7320 4745 5073 2066 726f 6d20 616c  rns GEPs from al
+000079f0: 6c20 7261 6e6b 732e 2044 6566 6175 6c74  l ranks. Default
+00007a00: 7320 746f 204e 6f6e 650d 0a20 2020 2020  s to None..     
+00007a10: 2020 203a 7479 7065 206b 3a20 556e 696f     :type k: Unio
+00007a20: 6e5b 696e 742c 2049 7465 7261 626c 655d  n[int, Iterable]
+00007a30: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
+00007a40: 2020 2020 3a70 6172 616d 2074 7970 653a      :param type:
+00007a50: 2022 636e 6d66 5f67 6570 5f73 636f 7265   "cnmf_gep_score
+00007a60: 2220 6f72 2022 636e 6d66 5f67 6570 5f74  " or "cnmf_gep_t
+00007a70: 706d 222c 2064 6566 6175 6c74 7320 746f  pm", defaults to
+00007a80: 2022 636e 6d66 5f67 6570 5f73 636f 7265   "cnmf_gep_score
+00007a90: 220d 0a20 2020 2020 2020 203a 7479 7065  "..        :type
+00007aa0: 2074 7970 653a 2073 7472 2c20 6f70 7469   type: str, opti
+00007ab0: 6f6e 616c 0d0a 2020 2020 2020 2020 3a72  onal..        :r
+00007ac0: 6574 7572 6e3a 2066 6561 7475 7265 7320  eturn: features 
+00007ad0: c397 2047 4550 206d 6174 7269 780d 0a20  .. GEP matrix.. 
+00007ae0: 2020 2020 2020 203a 7274 7970 653a 2070         :rtype: p
+00007af0: 642e 4461 7461 4672 616d 650d 0a20 2020  d.DataFrame..   
+00007b00: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00007b10: 2020 6466 203d 2073 656c 662e 6164 6174    df = self.adat
+00007b20: 612e 7661 726d 5b74 7970 655d 2e63 6f70  a.varm[type].cop
+00007b30: 7928 290d 0a20 2020 2020 2020 2064 662e  y()..        df.
+00007b40: 636f 6c75 6d6e 7320 3d20 7064 2e4d 756c  columns = pd.Mul
+00007b50: 7469 496e 6465 782e 6672 6f6d 5f74 7570  tiIndex.from_tup
+00007b60: 6c65 7328 6466 2e63 6f6c 756d 6e73 2e73  les(df.columns.s
+00007b70: 7472 2e73 706c 6974 2822 2e22 292e 746f  tr.split(".").to
+00007b80: 5f6c 6973 7428 2929 0d0a 2020 2020 2020  _list())..      
+00007b90: 2020 6466 2e63 6f6c 756d 6e73 203d 2064    df.columns = d
+00007ba0: 662e 636f 6c75 6d6e 732e 7365 745f 6c65  f.columns.set_le
+00007bb0: 7665 6c73 285b 6c2e 6173 7479 7065 2822  vels([l.astype("
+00007bc0: 696e 7422 2920 666f 7220 6c20 696e 2064  int") for l in d
+00007bd0: 662e 636f 6c75 6d6e 732e 6c65 7665 6c73  f.columns.levels
+00007be0: 5d29 0d0a 2020 2020 2020 2020 6966 2069  ])..        if i
+00007bf0: 7369 6e73 7461 6e63 6528 6b2c 2028 696e  sinstance(k, (in
+00007c00: 742c 2049 7465 7261 626c 6529 293a 0d0a  t, Iterable)):..
+00007c10: 2020 2020 2020 2020 2020 2020 6466 203d              df =
+00007c20: 2064 662e 6c6f 635b 3a2c 206b 5d0d 0a20   df.loc[:, k].. 
+00007c30: 2020 2020 2020 2064 6620 3d20 6466 2e73         df = df.s
+00007c40: 6f72 745f 696e 6465 7828 6178 6973 3d31  ort_index(axis=1
+00007c50: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00007c60: 6e20 6466 0d0a 2020 2020 0d0a 2020 2020  n df..    ..    
+00007c70: 6465 6620 6765 745f 6d65 7461 6461 7461  def get_metadata
+00007c80: 5f64 6628 7365 6c66 2c0d 0a20 2020 2020  _df(self,..     
+00007c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ca0: 2020 2069 6e63 6c75 6465 5f63 6174 6567     include_categ
+00007cb0: 6f72 6963 616c 3a20 626f 6f6c 203d 2054  orical: bool = T
+00007cc0: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
+00007cd0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00007ce0: 636c 7564 655f 6e75 6d65 7269 6361 6c3a  clude_numerical:
+00007cf0: 2062 6f6f 6c20 3d20 5472 7565 0d0a 2020   bool = True..  
+00007d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d10: 2020 2020 2020 2920 2d3e 2070 642e 4461        ) -> pd.Da
+00007d20: 7461 4672 616d 653a 0d0a 2020 2020 2020  taFrame:..      
+00007d30: 2020 2222 2247 6574 2073 616d 706c 652f    """Get sample/
+00007d40: 6f62 7365 7276 6174 696f 6e20 6d65 7461  observation meta
+00007d50: 6461 7461 2e0d 0a0d 0a20 2020 2020 2020  data.....       
+00007d60: 203a 7061 7261 6d20 696e 636c 7564 655f   :param include_
+00007d70: 6361 7465 676f 7269 6361 6c3a 2049 6e63  categorical: Inc
+00007d80: 6c75 6465 2063 6174 6567 6f72 6963 616c  lude categorical
+00007d90: 206d 6574 6164 6174 6120 6c61 7965 7273   metadata layers
+00007da0: 2c20 6465 6661 756c 7473 2074 6f20 5472  , defaults to Tr
+00007db0: 7565 0d0a 2020 2020 2020 2020 3a74 7970  ue..        :typ
+00007dc0: 6520 696e 636c 7564 655f 6361 7465 676f  e include_catego
+00007dd0: 7269 6361 6c3a 2062 6f6f 6c2c 206f 7074  rical: bool, opt
+00007de0: 696f 6e61 6c0d 0a20 2020 2020 2020 203a  ional..        :
+00007df0: 7061 7261 6d20 696e 636c 7564 655f 6e75  param include_nu
+00007e00: 6d65 7269 6361 6c3a 2049 6e63 6c75 6465  merical: Include
+00007e10: 206e 756d 6572 6963 616c 206d 6574 6164   numerical metad
+00007e20: 6174 6120 6c61 7965 7273 2c20 6465 6661  ata layers, defa
+00007e30: 756c 7473 2074 6f20 5472 7565 0d0a 2020  ults to True..  
+00007e40: 2020 2020 2020 3a74 7970 6520 696e 636c        :type incl
+00007e50: 7564 655f 6e75 6d65 7269 6361 6c3a 2062  ude_numerical: b
+00007e60: 6f6f 6c2c 206f 7074 696f 6e61 6c0d 0a20  ool, optional.. 
+00007e70: 2020 2020 2020 203a 7261 6973 6573 2056         :raises V
+00007e80: 616c 7565 4572 726f 723a 2045 7272 6f72  alueError: Error
+00007e90: 2069 6620 6d65 7461 6461 7461 2074 7970   if metadata typ
+00007ea0: 6573 2061 7265 206e 6f74 2072 6563 6f67  es are not recog
+00007eb0: 6e69 7a65 640d 0a20 2020 2020 2020 203a  nized..        :
+00007ec0: 7265 7475 726e 3a20 6f62 7365 7276 6174  return: observat
+00007ed0: 696f 6e73 20c3 9720 6d65 7461 6461 7461  ions .. metadata
+00007ee0: 206d 6174 7269 780d 0a20 2020 2020 2020   matrix..       
+00007ef0: 203a 7274 7970 653a 2070 642e 4461 7461   :rtype: pd.Data
+00007f00: 4672 616d 650d 0a20 2020 2020 2020 2022  Frame..        "
+00007f10: 2222 0d0a 2020 2020 2020 2020 6474 7970  ""..        dtyp
+00007f20: 6573 203d 205b 5d0d 0a20 2020 2020 2020  es = []..       
+00007f30: 2069 6620 696e 636c 7564 655f 6361 7465   if include_cate
+00007f40: 676f 7269 6361 6c3a 0d0a 2020 2020 2020  gorical:..      
+00007f50: 2020 2020 2020 6474 7970 6573 2e61 7070        dtypes.app
+00007f60: 656e 6428 2263 6174 6567 6f72 7922 290d  end("category").
+00007f70: 0a20 2020 2020 2020 2069 6620 696e 636c  .        if incl
+00007f80: 7564 655f 6e75 6d65 7269 6361 6c3a 0d0a  ude_numerical:..
+00007f90: 2020 2020 2020 2020 2020 2020 6474 7970              dtyp
+00007fa0: 6573 202b 3d20 5b22 666c 6f61 7422 2c20  es += ["float", 
+00007fb0: 2269 6e74 225d 0d0a 2020 2020 2020 2020  "int"]..        
+00007fc0: 756e 6578 706c 6169 6e65 645f 636f 6c73  unexplained_cols
+00007fd0: 203d 2073 656c 662e 6164 6174 612e 6f62   = self.adata.ob
+00007fe0: 732e 7365 6c65 6374 5f64 7479 7065 7328  s.select_dtypes(
+00007ff0: 6578 636c 7564 653d 2822 6361 7465 676f  exclude=("catego
+00008000: 7279 222c 2022 666c 6f61 7422 2c20 2269  ry", "float", "i
+00008010: 6e74 2229 292e 636f 6c75 6d6e 730d 0a20  nt")).columns.. 
+00008020: 2020 2020 2020 2069 6620 6c65 6e28 756e         if len(un
+00008030: 6578 706c 6169 6e65 645f 636f 6c73 2920  explained_cols) 
+00008040: 3e20 303a 0d0a 2020 2020 2020 2020 2020  > 0:..          
+00008050: 2020 756e 6578 706c 6169 6e65 645f 636f    unexplained_co
+00008060: 6c5f 7374 7220 3d20 222c 2022 2e6a 6f69  l_str = ", ".joi
+00008070: 6e28 756e 6578 706c 6169 6e65 645f 636f  n(unexplained_co
+00008080: 6c73 290d 0a20 2020 2020 2020 2020 2020  ls)..           
+00008090: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+000080a0: 7228 6622 7b75 6e65 7870 6c61 696e 6564  r(f"{unexplained
+000080b0: 5f63 6f6c 5f73 7472 7d20 6d65 7461 6461  _col_str} metada
+000080c0: 7461 2063 6f6c 756d 6e73 2068 6176 6520  ta columns have 
+000080d0: 756e 7265 636f 676e 697a 6564 2064 7479  unrecognized dty
+000080e0: 7065 732e 2229 0d0a 2020 2020 2020 2020  pes.")..        
+000080f0: 6466 203d 2073 656c 662e 6164 6174 612e  df = self.adata.
+00008100: 6f62 732e 7365 6c65 6374 5f64 7479 7065  obs.select_dtype
+00008110: 7328 696e 636c 7564 653d 6474 7970 6573  s(include=dtypes
+00008120: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00008130: 6e20 6466 0d0a 2020 2020 0d0a 2020 2020  n df..    ..    
+00008140: 6465 6620 6765 745f 6361 7465 676f 7279  def get_category
+00008150: 5f6f 7665 7272 6570 7265 7365 6e74 6174  _overrepresentat
+00008160: 696f 6e28 7365 6c66 2c0d 0a20 2020 2020  ion(self,..     
+00008170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008190: 2020 206c 6179 6572 3a20 7374 722c 0d0a     layer: str,..
+000081a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081c0: 2020 2020 2020 2020 7472 756e 6361 7465          truncate
+000081d0: 5f6e 6567 6174 6976 653a 2062 6f6f 6c20  _negative: bool 
+000081e0: 3d20 5472 7565 0d0a 2020 2020 2020 2020  = True..        
+000081f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008210: 2920 2d3e 2070 642e 4461 7461 4672 616d  ) -> pd.DataFram
+00008220: 653a 0d0a 2020 2020 2020 2020 2222 2243  e:..        """C
+00008230: 616c 6375 6c61 7465 2050 6561 7273 6f6e  alculate Pearson
+00008240: 2072 6573 6964 7561 6c20 6f66 2063 6869   residual of chi
+00008250: 2d73 7175 6172 6564 2074 6573 742c 2061  -squared test, a
+00008260: 7373 6f63 6961 7469 6e67 2047 4550 7320  ssociating GEPs 
+00008270: 666f 7220 6561 6368 2072 616e 6b20 286b  for each rank (k
+00008280: 2920 746f 2063 6174 6567 6f72 6965 7320  ) to categories 
+00008290: 6f66 2073 616d 706c 6573 2f6f 6273 6572  of samples/obser
+000082a0: 7661 7469 6f6e 732e 2042 7920 6465 6661  vations. By defa
+000082b0: 756c 742c 2074 7275 6e63 6174 6573 206e  ult, truncates n
+000082c0: 6567 6174 6976 6520 7661 6c75 6573 2e0d  egative values..
+000082d0: 0a0d 0a20 2020 2020 2020 203a 7061 7261  ...        :para
+000082e0: 6d20 6c61 7965 723a 206e 616d 6520 6f66  m layer: name of
+000082f0: 2063 6174 6567 6f72 6963 616c 2064 6174   categorical dat
+00008300: 6120 6c61 7965 720d 0a20 2020 2020 2020  a layer..       
+00008310: 203a 7479 7065 206c 6179 6572 3a20 7374   :type layer: st
+00008320: 720d 0a20 2020 2020 2020 203a 7061 7261  r..        :para
+00008330: 6d20 7472 756e 6361 7465 5f6e 6567 6174  m truncate_negat
+00008340: 6976 653a 2054 7275 6e63 6174 6520 6e65  ive: Truncate ne
+00008350: 6761 7469 7665 2072 6573 6964 7561 6c73  gative residuals
+00008360: 2074 6f20 302c 2064 6566 6175 6c74 7320   to 0, defaults 
+00008370: 746f 2054 7275 650d 0a20 2020 2020 2020  to True..       
+00008380: 203a 7479 7065 2074 7275 6e63 6174 655f   :type truncate_
+00008390: 6e65 6761 7469 7665 3a20 626f 6f6c 2c20  negative: bool, 
+000083a0: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
+000083b0: 2020 3a72 6574 7572 6e3a 2063 6174 6567    :return: categ
+000083c0: 6f72 7920 c397 2047 4550 206d 6174 7269  ory .. GEP matri
+000083d0: 7820 6f66 206f 7665 7272 6570 7265 7365  x of overreprese
+000083e0: 6e74 6174 696f 6e20 7661 6c75 6573 0d0a  ntation values..
+000083f0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+00008400: 7064 2e44 6174 6146 7261 6d65 0d0a 2020  pd.DataFrame..  
+00008410: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00008420: 2020 2075 7361 6765 203d 2073 656c 662e     usage = self.
+00008430: 6765 745f 7573 6167 6573 286e 6f72 6d61  get_usages(norma
+00008440: 6c69 7a65 3d54 7275 6529 2e63 6f70 7928  lize=True).copy(
+00008450: 290d 0a20 2020 2020 2020 2073 616d 706c  )..        sampl
+00008460: 655f 746f 5f63 6c61 7373 203d 2073 656c  e_to_class = sel
+00008470: 662e 6765 745f 6d65 7461 6461 7461 5f64  f.get_metadata_d
+00008480: 6628 295b 6c61 7965 725d 0d0a 2020 2020  f()[layer]..    
+00008490: 2020 2020 7573 6167 652e 696e 6465 7820      usage.index 
+000084a0: 3d20 7573 6167 652e 696e 6465 782e 6d61  = usage.index.ma
+000084b0: 7028 7361 6d70 6c65 5f74 6f5f 636c 6173  p(sample_to_clas
+000084c0: 7329 0d0a 2020 2020 2020 2020 6f62 7365  s)..        obse
+000084d0: 7276 6564 203d 2075 7361 6765 2e67 726f  rved = usage.gro
+000084e0: 7570 6279 2861 7869 733d 302c 206c 6576  upby(axis=0, lev
+000084f0: 656c 3d30 292e 7375 6d28 290d 0a20 2020  el=0).sum()..   
+00008500: 2020 2020 2065 7870 6563 7465 6420 3d20       expected = 
+00008510: 5b5d 0d0a 2020 2020 2020 2020 666f 7220  []..        for 
+00008520: 6b2c 206f 6273 5f6b 2069 6e20 6f62 7365  k, obs_k in obse
+00008530: 7276 6564 2e67 726f 7570 6279 2861 7869  rved.groupby(axi
+00008540: 733d 312c 206c 6576 656c 3d31 293a 0d0a  s=1, level=1):..
+00008550: 2020 2020 2020 2020 2020 2020 6578 705f              exp_
+00008560: 6b20 3d20 7064 2e44 6174 6146 7261 6d65  k = pd.DataFrame
+00008570: 286f 6273 5f6b 2e73 756d 2861 7869 733d  (obs_k.sum(axis=
+00008580: 3129 2920 4020 7064 2e44 6174 6146 7261  1)) @ pd.DataFra
+00008590: 6d65 286f 6273 5f6b 2e73 756d 2861 7869  me(obs_k.sum(axi
+000085a0: 733d 3029 292e 5420 2f20 6f62 735f 6b2e  s=0)).T / obs_k.
+000085b0: 7375 6d28 292e 7375 6d28 290d 0a20 2020  sum().sum()..   
+000085c0: 2020 2020 2020 2020 2065 7870 6563 7465           expecte
+000085d0: 642e 6170 7065 6e64 2865 7870 5f6b 290d  d.append(exp_k).
+000085e0: 0a20 2020 2020 2020 2065 7870 6563 7465  .        expecte
+000085f0: 6420 3d20 7064 2e63 6f6e 6361 7428 6578  d = pd.concat(ex
+00008600: 7065 6374 6564 2c20 6178 6973 3d31 290d  pected, axis=1).
+00008610: 0a20 2020 2020 2020 2063 6869 7371 5f72  .        chisq_r
+00008620: 6573 6964 203d 2028 6f62 7365 7276 6564  esid = (observed
+00008630: 202d 2065 7870 6563 7465 6429 202f 206e   - expected) / n
+00008640: 702e 7371 7274 2865 7870 6563 7465 6429  p.sqrt(expected)
+00008650: 2020 2320 7065 6172 736f 6e20 7265 7369    # pearson resi
+00008660: 6475 616c 206f 6620 6368 692d 7371 7561  dual of chi-squa
+00008670: 7265 6420 7465 7374 206f 6620 636f 6e74  red test of cont
+00008680: 696e 6765 6e63 7920 7461 626c 650d 0a20  ingency table.. 
+00008690: 2020 2020 2020 2069 6620 7472 756e 6361         if trunca
+000086a0: 7465 5f6e 6567 6174 6976 653a 0d0a 2020  te_negative:..  
+000086b0: 2020 2020 2020 2020 2020 6368 6973 715f            chisq_
+000086c0: 7265 7369 6420 3d20 6368 6973 715f 7265  resid = chisq_re
+000086d0: 7369 642e 636c 6970 286c 6f77 6572 3d30  sid.clip(lower=0
+000086e0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+000086f0: 6e20 6368 6973 715f 7265 7369 640d 0a20  n chisq_resid.. 
+00008700: 2020 200d 0a20 2020 2020 2020 200d 0a20     ..        .. 
+00008710: 2020 2064 6566 2067 6574 5f6d 6574 6164     def get_metad
+00008720: 6174 615f 636f 7272 656c 6174 696f 6e28  ata_correlation(
+00008730: 7365 6c66 2c20 0d0a 2020 2020 2020 2020  self, ..        
+00008740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008750: 2020 2020 2020 2020 206c 6179 6572 3a20           layer: 
+00008760: 7374 722c 0d0a 2020 2020 2020 2020 2020  str,..          
+00008770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008780: 2020 2020 2020 206d 6574 686f 643a 2073         method: s
+00008790: 7472 203d 2022 7065 6172 736f 6e22 0d0a  tr = "pearson"..
+000087a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087c0: 2029 202d 3e20 7064 2e53 6572 6965 733a   ) -> pd.Series:
+000087d0: 0d0a 2020 2020 2020 2020 2222 2243 616c  ..        """Cal
+000087e0: 6375 6c61 7465 2050 6561 7273 6f6e 2063  culate Pearson c
+000087f0: 6f72 7265 6c61 7469 6f6e 206f 6620 4745  orrelation of GE
+00008800: 5020 7573 6167 6520 746f 206e 756d 6572  P usage to numer
+00008810: 6963 616c 206d 6574 6164 6174 6120 6163  ical metadata ac
+00008820: 726f 7373 2073 616d 706c 6573 2f6f 6273  ross samples/obs
+00008830: 6572 7661 7469 6f6e 732e 0d0a 0d0a 2020  ervations.....  
+00008840: 2020 2020 2020 3a70 6172 616d 206c 6179        :param lay
+00008850: 6572 3a20 6e61 6d65 206f 6620 6e75 6d65  er: name of nume
+00008860: 7269 6361 6c20 6461 7461 206c 6179 6572  rical data layer
+00008870: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+00008880: 6c61 7965 723a 2073 7472 0d0a 2020 2020  layer: str..    
+00008890: 2020 2020 3a70 6172 616d 206d 6574 686f      :param metho
+000088a0: 643a 2043 6f72 7265 6c61 7469 6f6e 206d  d: Correlation m
+000088b0: 6574 686f 643a 2022 7065 6172 736f 6e22  ethod: "pearson"
+000088c0: 2c20 2273 7065 6172 6d61 6e22 2c20 6f72  , "spearman", or
+000088d0: 2022 6b65 6e64 616c 6c22 2e20 4465 6661   "kendall". Defa
+000088e0: 756c 7473 2074 6f20 2270 6561 7273 6f6e  ults to "pearson
+000088f0: 220d 0a20 2020 2020 2020 203a 7479 7065  "..        :type
+00008900: 206d 6574 686f 643a 2073 7472 2c20 6f70   method: str, op
+00008910: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
+00008920: 3a72 6574 7572 6e3a 2063 6f72 7265 6c61  :return: correla
+00008930: 7469 6f6e 206f 6620 4745 5020 746f 206d  tion of GEP to m
+00008940: 6574 6164 6174 610d 0a20 2020 2020 2020  etadata..       
+00008950: 203a 7274 7970 653a 2070 642e 5365 7269   :rtype: pd.Seri
+00008960: 6573 0d0a 2020 2020 2020 2020 2222 220d  es..        """.
+00008970: 0a20 2020 2020 2020 2075 7361 6765 203d  .        usage =
+00008980: 2073 656c 662e 6765 745f 7573 6167 6573   self.get_usages
+00008990: 2829 2e63 6f70 7928 290d 0a20 2020 2020  ().copy()..     
+000089a0: 2020 206d 6574 6164 6174 6120 3d20 7365     metadata = se
+000089b0: 6c66 2e67 6574 5f6d 6574 6164 6174 615f  lf.get_metadata_
+000089c0: 6466 2829 5b6c 6179 6572 5d0d 0a20 2020  df()[layer]..   
+000089d0: 2020 2020 206d 645f 636f 7272 203d 2075       md_corr = u
+000089e0: 7361 6765 2e63 6f72 7277 6974 6828 6d65  sage.corrwith(me
+000089f0: 7461 6461 7461 2c20 6d65 7468 6f64 3d6d  tadata, method=m
+00008a00: 6574 686f 6429 0d0a 2020 2020 2020 2020  ethod)..        
+00008a10: 7265 7475 726e 206d 645f 636f 7272 0d0a  return md_corr..
+00008a20: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
+00008a30: 6620 6170 7065 6e64 5f74 6f5f 6869 7374  f append_to_hist
+00008a40: 6f72 7928 7365 6c66 2c20 656e 7472 7929  ory(self, entry)
+00008a50: 3a0d 0a20 2020 2020 2020 2022 2222 4164  :..        """Ad
+00008a60: 6420 656e 7472 7920 746f 2044 6174 6173  d entry to Datas
+00008a70: 6574 2068 6973 746f 7279 2e0d 0a0d 0a20  et history..... 
+00008a80: 2020 2020 2020 203a 7061 7261 6d20 656e         :param en
+00008a90: 7472 793a 2044 6573 6372 6970 7469 6f6e  try: Description
+00008aa0: 206f 6620 6576 656e 7420 746f 2072 6563   of event to rec
+00008ab0: 6f72 6420 696e 2074 6865 2068 6973 746f  ord in the histo
+00008ac0: 7279 2e0d 0a20 2020 2020 2020 203a 7479  ry...        :ty
+00008ad0: 7065 2065 6e74 7279 3a20 7374 720d 0a20  pe entry: str.. 
+00008ae0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00008af0: 2020 2020 7365 6c66 2e61 6461 7461 2e75      self.adata.u
+00008b00: 6e73 5b22 6869 7374 6f72 7922 5d5b 6461  ns["history"][da
+00008b10: 7465 7469 6d65 2e75 7463 6e6f 7728 292e  tetime.utcnow().
+00008b20: 6973 6f66 6f72 6d61 7428 295d 203d 2065  isoformat()] = e
+00008b30: 6e74 7279 0d0a 2020 2020 2020 2020 0d0a  ntry..        ..
+00008b40: 2020 2020 6465 6620 6765 745f 6869 7374      def get_hist
+00008b50: 6f72 7928 7365 6c66 293a 0d0a 2020 2020  ory(self):..    
+00008b60: 2020 2020 2222 2252 6574 7572 6e73 2074      """Returns t
+00008b70: 696d 6573 7461 6d70 6564 2068 6973 746f  imestamped histo
+00008b80: 7279 206f 6620 4461 7461 7365 7420 6f62  ry of Dataset ob
+00008b90: 6a65 6374 2e0d 0a0d 0a20 2020 2020 2020  ject.....       
+00008ba0: 203a 7265 7475 726e 3a20 6869 7374 6f72   :return: histor
+00008bb0: 790d 0a20 2020 2020 2020 203a 7274 7970  y..        :rtyp
+00008bc0: 653a 2064 6963 740d 0a20 2020 2020 2020  e: dict..       
+00008bd0: 2022 2222 0d0a 2020 2020 2020 2020 7265   """..        re
+00008be0: 7475 726e 2073 656c 662e 6164 6174 612e  turn self.adata.
+00008bf0: 756e 735b 2268 6973 746f 7279 225d       uns["history"]
```

### Comparing `cnmfsns-1.3.2/src/cnmfsns/integration.py` & `cnmfsns-1.4.0/src/cnmfsns/integration.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.2/src/cnmfsns/plots.py` & `cnmfsns-1.4.0/src/cnmfsns/plots.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .integration import Integration
 from .colors import Colors
 from .sns import SNS
 from . import utils
 
 
 from collections.abc import Iterable, Collection, Mapping
-from typing import Union, Optional
+from typing import Union, Optional, Literal
 
 import pandas as pd
 import numpy as np
 import seaborn as sns
 import matplotlib as mpl
 from matplotlib.figure import Figure
 from matplotlib.axes import Axes
@@ -23,109 +23,140 @@
 import networkx as nx
 
 
 #########################
 # Dataset-related plots #
 #########################
 
-
-def plot_feature_dispersion(dataset: Dataset, show_selected:bool = False, all_plots: bool = False):
-    """
-    Create diagnostic plots for data from model_overdispersion()
-    """
+def plot_feature_dispersion(dataset: Dataset,
+                            show_selected: bool = False,
+                            show_model_curve: bool = True,
+                            y_unit: Literal["log_variance", "odscore", "log_odscore", "vscore", "log_vscore"] = "log_variance",
+                            ax: Optional[Axes] = None):
+    
     df = dataset.adata.var.sort_values("mean")
-    figs = {}
-
-    # Figure: Default model mean and variance
-    fig, axes = plt.subplots(1, 3, figsize=[12, 4], layout="tight")
+    if "log_odscore" not in df.columns:  # required for compatibility with older h5ad files which do not have this column
+        df["log_odscore"] = np.log10(df["odscore"])
+        df["log_vscore"] = np.log10(df["vscore"])
     
-    ax = axes[0]  # untransformed
-    if show_selected:
-        sns.histplot(df, x="log_mean", y="log_variance", hue="selected", bins=[100,100], ax=ax, alpha=0.5, palette={True: "red", False: "blue"})
-        ax.legend(handles=[
-            Patch(color="blue", alpha=0.5, label="False"),
-            Patch(color="red", alpha=0.5, label="True"),
-            Line2D([0], [0], color='green', label="model")
-        ], title="selected")
+    if ax is None:
+        fig, ax_plot = plt.subplots(figsize=[4, 4], layout="tight")
     else:
-        sns.histplot(df, x="log_mean", y="log_variance", bins=[100,100], ax=ax, color="blue")
-    ax.plot(df["log_mean"], df["gam_fittedvalues"], color="green")
-    ax.set_title("Mean-Variance")
-    ax.set_xlabel("log10(mean)")
-    ax.set_ylabel("log10(variance)")
+        ax_plot = ax
 
-    ax = axes[1]  # transformed
+    
     if show_selected:
-        sns.histplot(df, x="log_mean", y="odscore", hue="selected", bins=[100,100], ax=ax, palette={True: "red", False: "blue"})
-        ax.legend(handles=[
+        sns.histplot(df, x="log_mean", y=y_unit, hue="selected", bins=[100,100], ax=ax_plot, alpha=0.5, palette={True: "red", False: "blue"})
+        ax_plot.legend(handles=[
             Patch(color="blue", alpha=0.5, label="False"),
             Patch(color="red", alpha=0.5, label="True"),
             Line2D([0], [0], color='green', label="model")
         ], title="selected")
     else:
-        sns.histplot(df, x="log_mean", y="odscore", bins=[100,100], ax=ax, color="blue")
-    ax.hlines(1, xmin=df["log_mean"].min(), xmax=df["log_mean"].max(), color="green")
-    ax.set_title("Mean-Overdispersion (Default)")
-    ax.set_xlabel("log10(mean)")
-    ax.set_ylabel("od-score")
+        sns.histplot(df, x="log_mean", y=y_unit, bins=[100,100], ax=ax_plot, color="blue")
+    
+    # Show the model curve from the GAM
+    if show_model_curve:
+        if y_unit == "log_variance":
+            ax_plot.plot(df["log_mean"], df["gam_fittedvalues"], color="green")
+        elif y_unit == "odscore":
+            ax_plot.axhline(1)
+        elif y_unit == "log_odscore":
+            ax_plot.axhline(0)
+        else:
+            raise ValueError('show_model_curve must be False if the y-unit is "vscore" or "log_vscore".')
+    
+    ax_plot.set_xlabel("log10(mean)")
+    if y_unit == "log_variance":
+        ax_plot.set_ylabel("log10(variance)")
+    elif y_unit == "odscore":
+        ax_plot.set_ylabel("odscore")
+    elif y_unit == "log_odscore":
+        ax_plot.set_ylabel("log10(odscore)")
+    elif y_unit == "vscore":
+        ax_plot.set_ylabel("vscore")
+    elif y_unit == "log_vscore":
+        ax_plot.set_ylabel("log10(vscore)")
+
+
+    if ax is None:
+        return fig
+
+
+   
+
+def plot_feature_overdispersion_histogram(dataset: Dataset,
+                                          show_selected: bool = False,
+                                          y_unit: Literal["odscore", "log_odscore"] = "log_variance",
+                                          ax: Optional[Axes] = None):
+    df = dataset.adata.var.sort_values("mean")
+    if "log_odscore" not in df.columns:  # required for compatibility with older h5ad files which do not have this column
+        df["log_odscore"] = np.log10(df["odscore"])
     
-    ax=axes[2]  # thresholds
-    ax.set_title("od-score Distribution")
+    if ax is None:
+        fig, ax_plot = plt.subplots(figsize=[4, 4], layout="tight")
+    else:
+        ax_plot = ax
+
+
+    ax_plot.set_title("od-score Distribution")
     if df["odscore"].notnull().any():
         if show_selected:
-            sns.histplot(df, x="odscore", hue="selected", bins=100, linewidth=0, ax=ax, palette={True: "red", False: "blue"})
-            ax.legend(handles=[
+            sns.histplot(df, x="odscore", hue="selected", bins=100, linewidth=0, ax=ax_plot, palette={True: "red", False: "blue"})
+            ax_plot.legend(handles=[
                 Patch(color="blue", alpha=0.5, label="False"),
                 Patch(color="red", alpha=0.5, label="True")
             ], title="selected")
         else:
-            sns.histplot(df, x="odscore", bins=100, linewidth=0, ax=ax, color="blue")
-    ax.set_xlabel("od-score")
-    figs["default"] = fig
-
-    if all_plots:
-        # Figure: cnmf model mean and variance
-        fig, axes = plt.subplots(1, 3, figsize=[12, 4], layout="tight")
-        ax = axes[0]
-        if show_selected:
-            sns.histplot(df, x="log_mean", y="log_variance", hue="selected", bins=[100,100], ax=ax, alpha=0.5, palette={True: "red", False: "blue"})
-        else:
-            sns.histplot(df, x="log_mean", y="log_variance", bins=[100,100], ax=ax, color="blue")
-        ax.set_title("Mean-Variance")
-        ax.set_xlabel("log10(mean)")
-        ax.set_ylabel("log10(variance)")
-        ax = axes[1]
-        if show_selected:
-            sns.histplot(df, x="log_mean", y="vscore", hue="selected", bins=[100,100], ax=ax, palette={True: "red", False: "blue"})
-        else:
-            sns.histplot(df, x="log_mean", y="vscore", bins=[100,100], ax=ax, color="blue")
-        ax.set_title("Mean-Overdispersion (cnmf)")
-        ax.set_xlabel("log10(mean)")
-        ax.set_ylabel("v-score")
-        ax=axes[2]  # thresholds
-        ax.set_title("v-score Distribution")
-        if df["vscore"].notnull().any():
-            if show_selected:
-                sns.histplot(df, x="vscore", hue="selected", bins=100, linewidth=0, ax=ax, palette={True: "red", False: "blue"})
-                ax.legend(handles=[
-                    Patch(color="blue", alpha=0.5, label="False"),
-                    Patch(color="red", alpha=0.5, label="True")
-                ], title="selected")
-            else:
-                sns.histplot(df, x="vscore", bins=100, linewidth=0, ax=ax, color="blue")
-        ax.set_xlabel("v-score")
-        figs["cnmf"] = fig
-
-        fig, ax = plt.subplots(figsize=[12,12], layout="tight")
-        sns.histplot(data=df.fillna(0), x="odscore", y="vscore", bins=[100, 100], ax=ax)
-        ax.set_xlabel("od-score")
-        ax.set_ylabel("v-score")
-        figs["score_comparison"] = fig
+            sns.histplot(df, x=y_unit, bins=100, linewidth=0, ax=ax_plot, color="blue")
+    
+    if ax is None:
+        return fig
+
+
+    # if all_plots:
+    #     # Figure: cnmf model mean and variance
+    #     fig, axes = plt.subplots(1, 3, figsize=[12, 4], layout="tight")
+    #     ax = axes[0]
+    #     if show_selected:
+    #         sns.histplot(df, x="log_mean", y="log_variance", hue="selected", bins=[100,100], ax=ax, alpha=0.5, palette={True: "red", False: "blue"})
+    #     else:
+    #         sns.histplot(df, x="log_mean", y="log_variance", bins=[100,100], ax=ax, color="blue")
+    #     ax.set_title("Mean-Variance")
+    #     ax.set_xlabel("log10(mean)")
+    #     ax.set_ylabel("log10(variance)")
+    #     ax = axes[1]
+    #     if show_selected:
+    #         sns.histplot(df, x="log_mean", y="vscore", hue="selected", bins=[100,100], ax=ax, palette={True: "red", False: "blue"})
+    #     else:
+    #         sns.histplot(df, x="log_mean", y="vscore", bins=[100,100], ax=ax, color="blue")
+    #     ax.set_title("Mean-Overdispersion (cnmf)")
+    #     ax.set_xlabel("log10(mean)")
+    #     ax.set_ylabel("v-score")
+    #     ax=axes[2]  # thresholds
+    #     ax.set_title("v-score Distribution")
+    #     if df["vscore"].notnull().any():e
+    #         if show_selected:
+    #             sns.histplot(df, x="vscore", hue="selected", bins=100, linewidth=0, ax=ax, palette={True: "red", False: "blue"})
+    #             ax.legend(handles=[
+    #                 Patch(color="blue", alpha=0.5, label="False"),
+    #                 Patch(color="red", alpha=0.5, label="True")
+    #             ], title="selected")
+    #         else:
+    #             sns.histplot(df, x="vscore", bins=100, linewidth=0, ax=ax, color="blue")
+    #     ax.set_xlabel("v-score")
+    #     figs["cnmf"] = fig
+
+    #     fig, ax = plt.subplots(figsize=[12,12], layout="tight")
+    #     sns.histplot(data=df.fillna(0), x="odscore", y="vscore", bins=[100, 100], ax=ax)
+    #     ax.set_xlabel("od-score")
+    #     ax.set_ylabel("v-score")
+    #     figs["score_comparison"] = fig
         
-    return figs
+    # return figs
 
 
 def plot_stability_error(dataset: Dataset, figsize=(6, 4)):
     '''
     Borrowed from Alexandrov Et Al. 2013 Deciphering Mutational Signatures
     publication in Cell Reports
     '''
@@ -303,19 +334,20 @@
         ax.set_title(dataset_name)
         ax.set_xticks(df["max_k"])
         sns.lineplot(data=df, x="max_k", y="max_k_median_corr", hue="max_k_filter_pass", ax=ax, marker="o")
         ax.get_legend().remove()
         plt.tight_layout()
     return fig
 
-def plot_pairwise_corr(integration: Integration, subplot_size = [3, 3.5], overlaid=False):
+def plot_pairwise_corr(integration: Integration, subplot_size = [3, 3.5], overlaid=False, bins=50):
     tril = integration.get_corr_matrix_lowertriangle()
-    n_datasets = len(tril.index.levels[0])
     sps_width, sps_height = subplot_size
-    fig, axes = plt.subplots(n_datasets, n_datasets, figsize=[sps_width * n_datasets, sps_height * n_datasets], sharex=True, sharey=True, squeeze=False, layout="tight")
+    n_datasets = integration.n_datasets
+    fig, axes = plt.subplots(n_datasets, n_datasets,
+                             figsize=[sps_width * n_datasets, sps_height * n_datasets], sharex=True, sharey=True, squeeze=False, layout="tight")
     fig.suptitle(f"Correlation distribution between datasets")
     fig.supxlabel("Correlation coefficient")
     for row, dataset_row in enumerate(tril.index.levels[0]):
         for col, dataset_col in enumerate(tril.columns.levels[0]):
             ax = axes[row,col]
             if row < col:
                 ax.set_axis_off()
@@ -328,39 +360,40 @@
                         "palette": {"Included": "red", "Excluded": "gray"},
                         "hue_order": ["Excluded", "Included"]
                     }
                     included_fraction = (corr > min_corr).sum() / corr.shape[0]
                     ax.text(x=0.01, y=1.01, s=f"quantile={included_fraction:.3f}\nmin_corr={min_corr:.3f}", size=8, ha='left', va='bottom', transform=ax.transAxes, color="black")
                 else:
                     hist_kwargs = {"color": "gray"}
-                sns.histplot(x=corr, ax=ax,legend=(row == 0)&(col == 0), bins=50, linewidth=0, **hist_kwargs)
+                sns.histplot(x=corr, ax=ax,legend=(row == 0)&(col == 0), bins=bins, linewidth=0, **hist_kwargs)
 
                 ax.set_ylabel(dataset_row)
                 ax.set_xlabel(dataset_col)
                 ax.set_xlim(-1,1)
     return fig
 
-def plot_pairwise_corr_overlaid(integration: Integration, subplot_size = [3, 3.5]):
-    tril = tril = integration.get_corr_matrix_lowertriangle(max_k_filter=True)
+def plot_pairwise_corr_overlaid(integration: Integration, subplot_size = [3, 3.5], bins=50):
+    tril = integration.get_corr_matrix_lowertriangle(max_k_filter=True)
+    n_datasets = integration.n_datasets
     sps_width, sps_height = subplot_size
-    fig, axes = plt.subplots(integration.n_datasets, integration.n_datasets,
-                             figsize=[sps_width * integration.n_datasets, sps_height * integration.n_datasets],
+    fig, axes = plt.subplots(n_datasets, n_datasets,
+                             figsize=[sps_width * n_datasets, sps_height * n_datasets],
                              sharex=True, sharey=True, squeeze=False, layout="tight")
     fig.suptitle(f"Correlation distribution between datasets")
     fig.supxlabel("Correlation coefficient")
     for row, dataset_row in enumerate(tril.index.levels[0]):
         for col, dataset_col in enumerate(tril.columns.levels[0]):
             ax = axes[row,col]
             if row < col:
                 ax.set_axis_off()
             else:
                 corr = pd.DataFrame({"corr": tril.loc[dataset_row, dataset_col].values.flatten()}).dropna()
                 corr["sign"] = (corr["corr"] >= 0).map({True: "Positive", False: "Negative"})
                 corr["abscorr"] = corr["corr"].abs()
-                sns.histplot(data=corr, x="abscorr", hue="sign", palette= {"Positive": "red", "Negative": "blue"}, bins=50, alpha=0.5, linewidth=0,
+                sns.histplot(data=corr, x="abscorr", hue="sign", palette= {"Positive": "red", "Negative": "blue"}, bins=bins, alpha=0.5, linewidth=0,
                              hue_order= ["Negative", "Positive"], ax=ax,legend=(row == 0)&(col == 0))
 
                 # show min_corr as text in top left of plot and vertical line
                 min_corr = integration.pairwise_thresholds.loc[(dataset_row, dataset_col)]
                 included_fraction = (corr["corr"] > min_corr).sum() / corr.shape[0]  # could also show the quantile of the min_corr threshold
                 ax.text(x=0.01, y=1.01, s=f"quantile={included_fraction:.3f}\nmin_corr={min_corr:.3f}", size=8, ha='left', va='bottom', transform=ax.transAxes, color="black")
                 ax.axvline(min_corr, color="black")
@@ -1054,26 +1087,35 @@
 #################
 
 
 # overrepresentation bar plots
 def plot_overrepresentation_gep_bar(snsmap: SNS,
                                      colors: Colors,
                                      dataset_name: str,
+                                     layers: Optional[Union[str, Collection[str]]] = None,
                                      figsize: Optional[Collection] = None):
     dataset = snsmap.integration.datasets[dataset_name]
-    metadata = dataset.get_metadata_df(include_numerical=False).dropna(how="all", axis=1)
+
+    # layers to plot
+    if layers is None:
+        metadata_layers = dataset.get_metadata_df(include_numerical=False).dropna(how="all", axis=1).columns.to_list()
+    elif isinstance(layers, str):
+        metadata_layers = [layers]
+    else:
+        metadata_layers = layers
+
     # number of bars in each community for this dataset
     community_gep_counts = [len([node for node in snsmap.communities[c] if node.split("|")[0] == dataset_name]) for c in snsmap.ordered_community_names]
     
     if figsize is None:
         figsize = (snsmap.n_communities + 0.05 * sum(community_gep_counts),
-                   (metadata.shape[1] + 1)* 2)
+                   (len(metadata_layers) + 1)* 2)
     
     fig, axes = plt.subplots(
-        metadata.shape[1] + 1, snsmap.n_communities,
+        len(metadata_layers) + 1, snsmap.n_communities,
         figsize = figsize,
         sharey='row', squeeze=False,
         gridspec_kw={"width_ratios": community_gep_counts},
         layout="tight")
     fig.supxlabel("GEP")
     fig.supylabel("Overrepresentation")
     fig.suptitle("Community")
@@ -1093,15 +1135,15 @@
             kvals = pd.Series([k for k, gep in geps], index=geps)
             kvals.plot.bar(width=0.9, ax=ax, legend=None, color="#666666")
         ax.set_xlabel("")
         ax.set_xticks([])
         ax.yaxis.set_major_locator(mpl.ticker.MaxNLocator(nbins="auto", integer=True))  # y-ticks are integers!
     
     # subsequent subplot rows have metadata overrepresentation
-    for row, layer in enumerate(metadata.columns, 1):
+    for row, layer in enumerate(metadata_layers, 1):
         overrepresentation = dataset.get_category_overrepresentation(layer=layer)
         for col, community in enumerate(snsmap.ordered_community_names):
             ax = axes[row, col]
             geps = []
             for node in snsmap.communities[community]:
                 dataset_str, k_str, gep_str = node.split("|")
                 if dataset_str == dataset_name:
@@ -1118,30 +1160,38 @@
 
     return fig
 
 
 def plot_metadata_correlation_gep_bar(snsmap: SNS,
                                       colors: Colors,
                                       dataset_name: str,
+                                      layers: Optional[Union[str, Collection[str]]] = None,
                                       method: str = "pearson",
                                       figsize: Optional[Collection] = None
                                       ) -> Optional[Figure]:
     
     dataset = snsmap.integration.datasets[dataset_name]
-    metadata = dataset.get_metadata_df(include_categorical=False).dropna(how="all", axis=1)
-    
+
+    # layers to plot
+    if layers is None:
+        metadata_layers = dataset.get_metadata_df(include_categorical=False).dropna(how="all", axis=1).columns.to_list()
+    elif isinstance(layers, str):
+        metadata_layers = [layers]
+    else:
+        metadata_layers = layers
+
     # number of bars in each community for this dataset
     community_gep_counts = [len([node for node in snsmap.communities[c] if node.split("|")[0] == dataset_name]) for c in snsmap.ordered_community_names]
     
     if figsize is None:
         figsize = (snsmap.n_communities + 0.05 * sum(community_gep_counts),
-                   (metadata.shape[1] + 1)* 2)
+                   (len(metadata_layers) + 1)* 2)
     
     fig, axes = plt.subplots(
-        metadata.shape[1] + 1, snsmap.n_communities,
+        len(metadata_layers) + 1, snsmap.n_communities,
         figsize = figsize,
         sharey='row', squeeze=False,
         gridspec_kw={"width_ratios": community_gep_counts},
         layout="tight")
     fig.supxlabel("GEP")
     fig.supylabel(method.capitalize() + " Correlation")
     fig.suptitle("Community")
@@ -1160,15 +1210,15 @@
             kvals = pd.Series([k for k, gep in geps], index=geps)
             kvals.plot.bar(width=0.9, ax=ax, legend=None, color="#666666")
         ax.set_xlabel("")
         ax.set_xticks([])
         ax.yaxis.set_major_locator(mpl.ticker.MaxNLocator(nbins="auto", integer=True))  # y-ticks are integers!
     
     # subsequent subplot rows have metadata overrepresentation
-    for row, layer in enumerate(metadata.columns, 1):
+    for row, layer in enumerate(metadata_layers, 1):
         md_corr = dataset.get_metadata_correlation(layer=layer, method=method)
         for col, community in enumerate(snsmap.ordered_community_names):
             ax = axes[row, col]
             geps = []
             for node in snsmap.communities[community]:
                 dataset_str, k_str, gep_str = node.split("|")
                 if dataset_str == dataset_name:
```

### Comparing `cnmfsns-1.3.2/src/cnmfsns/sns.py` & `cnmfsns-1.4.0/src/cnmfsns/sns.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.2/src/cnmfsns/utils.py` & `cnmfsns-1.4.0/src/cnmfsns/utils.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.2/src/cnmfsns.egg-info/PKG-INFO` & `cnmfsns-1.4.0/src/cnmfsns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnmfsns
-Version: 1.3.2
+Version: 1.4.0
 Summary: cNMF Solution Network Space
 Home-page: https://github.com/MorrissyLab/cNMF-SNS
 Author: Ted Verhey
 Author-email: tbverhey@ucalgary.ca
 Project-URL: Bug Tracker, https://github.com/MorrissyLab/cNMF-SNS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 
 ![cNMF-SNS logo](logo.png)
 
 -----------------
 
 # cNMF-SNS: powerful factorization-based multi-omics integration toolkit
 
-![version badge](https://img.shields.io/badge/version-1.3.2-blue)
+![version badge](https://img.shields.io/badge/version-1.4.0-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
 [![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/cnmfsns)](https://anaconda.org/conda-forge/cnmfsns/)
 [![Documentation status](https://readthedocs.org/projects/cnmf-sns/badge/?version=latest&style=flat)]()
 [![Downloads](https://static.pepy.tech/badge/cnmfsns)](https://pepy.tech/project/cnmfsns)
 [![License](https://img.shields.io/pypi/l/cnmfsns.svg)](https://github.com/MorrissyLab/cNMF-SNS/blob/main/LICENSE)
 
 Authors: [Ted Verhey](https://github.com/verheytb), [Heewon Seo](https://github.com/lootpiz), [Sorana Morrissy](https://github.com/ancasorana)
```

