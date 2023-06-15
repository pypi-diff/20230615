# Comparing `tmp/graphdatascience-1.7.tar.gz` & `tmp/graphdatascience-1.7a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphdatascience-1.7.tar", last modified: Thu Jun 15 10:51:05 2023, max compression
+gzip compressed data, was "graphdatascience-1.7a1.tar", last modified: Wed May 24 12:08:18 2023, max compression
```

## Comparing `graphdatascience-1.7.tar` & `graphdatascience-1.7a1.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:51:05.199283 graphdatascience-1.7/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-15 10:49:44.000000 graphdatascience-1.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      265 2023-06-15 10:49:44.000000 graphdatascience-1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7236 2023-06-15 10:51:05.199283 graphdatascience-1.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5841 2023-06-15 10:49:44.000000 graphdatascience-1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:51:05.091282 graphdatascience-1.7/graphdatascience/
--rw-r--r--   0 root         (0) root         (0)      195 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:51:05.091282 graphdatascience-1.7/graphdatascience/algo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/algo/__init__.py
--rw-r--r--   0 root         (0) root         (0)      959 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/algo/algo_endpoints.py
--rw-r--r--   0 root         (0) root         (0)     1742 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/algo/algo_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)      332 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/algo/single_mode_algo_endpoints.py
--rw-r--r--   0 root         (0) root         (0)     1015 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/call_builder.py
--rw-r--r--   0 root         (0) root         (0)      812 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/caller_base.py
--rw-r--r--   0 root         (0) root         (0)     2748 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/endpoints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:51:05.091282 graphdatascience-1.7/graphdatascience/error/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/error/__init__.py
--rw-r--r--   0 root         (0) root         (0)      766 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/error/client_only_endpoint.py
--rw-r--r--   0 root         (0) root         (0)      945 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/error/deprecation_warning.py
--rw-r--r--   0 root         (0) root         (0)     1242 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/error/endpoint_suggester.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/error/illegal_attr_checker.py
--rw-r--r--   0 root         (0) root         (0)       48 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/error/unable_to_connect.py
--rw-r--r--   0 root         (0) root         (0)      568 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/error/uncallable_namespace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:51:05.095282 graphdatascience-1.7/graphdatascience/graph/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3703 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/graph/graph_alpha_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)     1007 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/graph/graph_alpha_project_runner.py
--rw-r--r--   0 root         (0) root         (0)     1760 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/graph/graph_beta_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)      798 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/graph/graph_endpoints.py
--rw-r--r--   0 root         (0) root         (0)    13049 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/graph/graph_entity_ops_runner.py
--rw-r--r--   0 root         (0) root         (0)     1871 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/graph/graph_export_runner.py
--rw-r--r--   0 root         (0) root         (0)     6689 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/graph/graph_object.py
--rw-r--r--   0 root         (0) root         (0)    18104 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/graph/graph_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)     2377 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/graph/graph_project_runner.py
--rw-r--r--   0 root         (0) root         (0)     2853 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/graph/graph_sample_runner.py
--rw-r--r--   0 root         (0) root         (0)     1643 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/graph/graph_type_check.py
--rw-r--r--   0 root         (0) root         (0)     5526 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/graph/nx_loader.py
--rw-r--r--   0 root         (0) root         (0)    14488 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/graph/ogb_loader.py
--rw-r--r--   0 root         (0) root         (0)     8011 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/graph_data_science.py
--rw-r--r--   0 root         (0) root         (0)     3302 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/ignored_server_endpoints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:51:05.095282 graphdatascience-1.7/graphdatascience/model/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1634 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/model/graphsage_model.py
--rw-r--r--   0 root         (0) root         (0)     1325 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/model/link_prediction_model.py
--rw-r--r--   0 root         (0) root         (0)     7259 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/model/model.py
--rw-r--r--   0 root         (0) root         (0)     1788 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/model/model_alpha_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)     1216 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/model/model_beta_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)      798 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/model/model_endpoints.py
--rw-r--r--   0 root         (0) root         (0)      658 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/model/model_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)     1066 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/model/model_resolver.py
--rw-r--r--   0 root         (0) root         (0)     2314 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/model/node_classification_model.py
--rw-r--r--   0 root         (0) root         (0)      773 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/model/node_regression_model.py
--rw-r--r--   0 root         (0) root         (0)     3297 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/model/pipeline_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:51:05.099282 graphdatascience-1.7/graphdatascience/pipeline/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/pipeline/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2146 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/pipeline/classification_training_pipeline.py
--rw-r--r--   0 root         (0) root         (0)      663 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/pipeline/lp_pipeline_create_runner.py
--rw-r--r--   0 root         (0) root         (0)     1749 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/pipeline/lp_training_pipeline.py
--rw-r--r--   0 root         (0) root         (0)      663 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/pipeline/nc_pipeline_create_runner.py
--rw-r--r--   0 root         (0) root         (0)     1772 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/pipeline/nc_training_pipeline.py
--rw-r--r--   0 root         (0) root         (0)      663 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/pipeline/nr_pipeline_create_runner.py
--rw-r--r--   0 root         (0) root         (0)     2795 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/pipeline/nr_training_pipeline.py
--rw-r--r--   0 root         (0) root         (0)      444 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/pipeline/pipeline_alpha_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)     1890 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/pipeline/pipeline_beta_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)     2661 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/pipeline/pipeline_endpoints.py
--rw-r--r--   0 root         (0) root         (0)     1719 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/pipeline/pipeline_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)     8211 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/pipeline/training_pipeline.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:51:05.099282 graphdatascience-1.7/graphdatascience/query_runner/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/query_runner/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3976 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/query_runner/arrow_graph_constructor.py
--rw-r--r--   0 root         (0) root         (0)     9319 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/query_runner/arrow_query_runner.py
--rw-r--r--   0 root         (0) root         (0)     5883 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/query_runner/aura_db_arrow_query_runner.py
--rw-r--r--   0 root         (0) root         (0)    19215 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/query_runner/cypher_graph_constructor.py
--rw-r--r--   0 root         (0) root         (0)      243 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/query_runner/graph_constructor.py
--rw-r--r--   0 root         (0) root         (0)     7477 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/query_runner/neo4j_query_runner.py
--rw-r--r--   0 root         (0) root         (0)     1158 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/query_runner/query_runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:51:05.099282 graphdatascience-1.7/graphdatascience/resources/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:51:05.103282 graphdatascience-1.7/graphdatascience/resources/cora/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/resources/cora/__init__.py
--rw-r--r--   0 root         (0) root         (0)   109404 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/resources/cora/cora_nodes_gzip.pkl
--rw-r--r--   0 root         (0) root         (0)    18041 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/resources/cora/cora_rels_gzip.pkl
--rw-r--r--   0 root         (0) root         (0)     1231 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/resources/cora/serialize_cora.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:51:05.103282 graphdatascience-1.7/graphdatascience/resources/imdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/resources/imdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42197 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/resources/imdb/imdb_acted_in_rels_gzip.pkl
--rw-r--r--   0 root         (0) root         (0)   246714 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/resources/imdb/imdb_actors_gzip.pkl
--rw-r--r--   0 root         (0) root         (0)    15825 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/resources/imdb/imdb_directed_in_rels_gzip.pkl
--rw-r--r--   0 root         (0) root         (0)    94640 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/resources/imdb/imdb_directors_gzip.pkl
--rw-r--r--   0 root         (0) root         (0)   112462 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/resources/imdb/imdb_movies_with_genre_gzip.pkl
--rw-r--r--   0 root         (0) root         (0)    64260 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/resources/imdb/imdb_movies_without_genre_gzip.pkl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:51:05.107282 graphdatascience-1.7/graphdatascience/resources/imdb/raw/
--rw-r--r--   0 root         (0) root         (0)   652688 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/resources/imdb/raw/edges.pkl
--rw-r--r--   0 root         (0) root         (0)    37310 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/resources/imdb/raw/labels.pkl
--rw-r--r--   0 root         (0) root         (0) 64166690 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/resources/imdb/raw/node_features.pkl
--rw-r--r--   0 root         (0) root         (0)     3493 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/resources/imdb/serialize_imdb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:51:05.195282 graphdatascience-1.7/graphdatascience/resources/karate/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/resources/karate/__init__.py
--rw-r--r--   0 root         (0) root         (0)      727 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/resources/karate/karate_club_gzip.pkl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:51:05.195282 graphdatascience-1.7/graphdatascience/server_version/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/server_version/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/server_version/compatible_with.py
--rw-r--r--   0 root         (0) root         (0)     1244 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/server_version/server_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:51:05.195282 graphdatascience-1.7/graphdatascience/system/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/system/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1909 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/system/config_endpoints.py
--rw-r--r--   0 root         (0) root         (0)     2899 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/system/system_endpoints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:51:05.199283 graphdatascience-1.7/graphdatascience/topological_lp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/topological_lp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2109 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/topological_lp/topological_lp_alpha_runner.py
--rw-r--r--   0 root         (0) root         (0)      343 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/topological_lp/topological_lp_endpoints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:51:05.199283 graphdatascience-1.7/graphdatascience/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3796 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/utils/util_endpoints.py
--rw-r--r--   0 root         (0) root         (0)     2137 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/utils/util_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-15 10:49:44.000000 graphdatascience-1.7/graphdatascience/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:51:05.091282 graphdatascience-1.7/graphdatascience.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7236 2023-06-15 10:51:05.000000 graphdatascience-1.7/graphdatascience.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4842 2023-06-15 10:51:05.000000 graphdatascience-1.7/graphdatascience.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 10:51:05.000000 graphdatascience-1.7/graphdatascience.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 10:51:04.000000 graphdatascience-1.7/graphdatascience.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      194 2023-06-15 10:51:05.000000 graphdatascience-1.7/graphdatascience.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-15 10:51:05.000000 graphdatascience-1.7/graphdatascience.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      136 2023-06-15 10:49:44.000000 graphdatascience-1.7/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:51:05.087282 graphdatascience-1.7/requirements/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:51:05.199283 graphdatascience-1.7/requirements/base/
--rw-r--r--   0 root         (0) root         (0)      170 2023-06-15 10:49:44.000000 graphdatascience-1.7/requirements/base/base.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-15 10:49:44.000000 graphdatascience-1.7/requirements/base/networkx.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-15 10:49:44.000000 graphdatascience-1.7/requirements/base/ogb.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 10:51:05.199283 graphdatascience-1.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2176 2023-06-15 10:49:44.000000 graphdatascience-1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.969512 graphdatascience-1.7a1/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      265 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7238 2023-05-24 12:08:18.969512 graphdatascience-1.7a1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5841 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.877512 graphdatascience-1.7a1/graphdatascience/
+-rw-r--r--   0 root         (0) root         (0)      195 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.877512 graphdatascience-1.7a1/graphdatascience/algo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/algo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      959 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/algo/algo_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/algo/algo_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)      332 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/algo/single_mode_algo_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/call_builder.py
+-rw-r--r--   0 root         (0) root         (0)      812 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/caller_base.py
+-rw-r--r--   0 root         (0) root         (0)     2748 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/endpoints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.881512 graphdatascience-1.7a1/graphdatascience/error/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/error/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      766 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/error/client_only_endpoint.py
+-rw-r--r--   0 root         (0) root         (0)      835 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/error/deprecation_warning.py
+-rw-r--r--   0 root         (0) root         (0)     1242 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/error/endpoint_suggester.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/error/illegal_attr_checker.py
+-rw-r--r--   0 root         (0) root         (0)       48 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/error/unable_to_connect.py
+-rw-r--r--   0 root         (0) root         (0)      568 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/error/uncallable_namespace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.881512 graphdatascience-1.7a1/graphdatascience/graph/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3556 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/graph_alpha_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)      843 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/graph_alpha_project_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/graph_beta_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)      798 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/graph_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)    13049 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/graph_entity_ops_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1871 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/graph_export_runner.py
+-rw-r--r--   0 root         (0) root         (0)     6689 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/graph_object.py
+-rw-r--r--   0 root         (0) root         (0)    16626 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/graph_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)     2377 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/graph_project_runner.py
+-rw-r--r--   0 root         (0) root         (0)     2175 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/graph_sample_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/graph_type_check.py
+-rw-r--r--   0 root         (0) root         (0)     5526 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/nx_loader.py
+-rw-r--r--   0 root         (0) root         (0)    14488 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/ogb_loader.py
+-rw-r--r--   0 root         (0) root         (0)     8612 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph_data_science.py
+-rw-r--r--   0 root         (0) root         (0)     3302 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/ignored_server_endpoints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.885512 graphdatascience-1.7a1/graphdatascience/model/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/model/graphsage_model.py
+-rw-r--r--   0 root         (0) root         (0)     1325 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/model/link_prediction_model.py
+-rw-r--r--   0 root         (0) root         (0)     7259 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/model/model.py
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/model/model_alpha_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1216 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/model/model_beta_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)      798 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/model/model_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/model/model_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1066 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/model/model_resolver.py
+-rw-r--r--   0 root         (0) root         (0)     2314 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/model/node_classification_model.py
+-rw-r--r--   0 root         (0) root         (0)      773 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/model/node_regression_model.py
+-rw-r--r--   0 root         (0) root         (0)     3297 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/model/pipeline_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.885512 graphdatascience-1.7a1/graphdatascience/pipeline/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/pipeline/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/pipeline/classification_training_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      663 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/pipeline/lp_pipeline_create_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/pipeline/lp_training_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      663 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/pipeline/nc_pipeline_create_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/pipeline/nc_training_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      663 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/pipeline/nr_pipeline_create_runner.py
+-rw-r--r--   0 root         (0) root         (0)     2795 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/pipeline/nr_training_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      444 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/pipeline/pipeline_alpha_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1890 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/pipeline/pipeline_beta_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)     2661 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/pipeline/pipeline_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)     1719 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/pipeline/pipeline_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)     8211 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/pipeline/training_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.889512 graphdatascience-1.7a1/graphdatascience/query_runner/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/query_runner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3976 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/query_runner/arrow_graph_constructor.py
+-rw-r--r--   0 root         (0) root         (0)     9319 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/query_runner/arrow_query_runner.py
+-rw-r--r--   0 root         (0) root         (0)     5297 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/query_runner/aura_db_arrow_query_runner.py
+-rw-r--r--   0 root         (0) root         (0)    17897 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/query_runner/cypher_graph_constructor.py
+-rw-r--r--   0 root         (0) root         (0)      243 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/query_runner/graph_constructor.py
+-rw-r--r--   0 root         (0) root         (0)     7477 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/query_runner/neo4j_query_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1158 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/query_runner/query_runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.889512 graphdatascience-1.7a1/graphdatascience/resources/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.889512 graphdatascience-1.7a1/graphdatascience/resources/cora/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/cora/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   109404 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/cora/cora_nodes_gzip.pkl
+-rw-r--r--   0 root         (0) root         (0)    18041 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/cora/cora_rels_gzip.pkl
+-rw-r--r--   0 root         (0) root         (0)     1231 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/cora/serialize_cora.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.889512 graphdatascience-1.7a1/graphdatascience/resources/imdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/imdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42197 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/imdb/imdb_acted_in_rels_gzip.pkl
+-rw-r--r--   0 root         (0) root         (0)   246714 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/imdb/imdb_actors_gzip.pkl
+-rw-r--r--   0 root         (0) root         (0)    15825 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/imdb/imdb_directed_in_rels_gzip.pkl
+-rw-r--r--   0 root         (0) root         (0)    94640 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/imdb/imdb_directors_gzip.pkl
+-rw-r--r--   0 root         (0) root         (0)   112462 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/imdb/imdb_movies_with_genre_gzip.pkl
+-rw-r--r--   0 root         (0) root         (0)    64260 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/imdb/imdb_movies_without_genre_gzip.pkl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.893512 graphdatascience-1.7a1/graphdatascience/resources/imdb/raw/
+-rw-r--r--   0 root         (0) root         (0)   652688 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/imdb/raw/edges.pkl
+-rw-r--r--   0 root         (0) root         (0)    37310 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/imdb/raw/labels.pkl
+-rw-r--r--   0 root         (0) root         (0) 64166690 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/imdb/raw/node_features.pkl
+-rw-r--r--   0 root         (0) root         (0)     3493 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/imdb/serialize_imdb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.965512 graphdatascience-1.7a1/graphdatascience/resources/karate/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/karate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      727 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/karate/karate_club_gzip.pkl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.965512 graphdatascience-1.7a1/graphdatascience/server_version/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/server_version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/server_version/compatible_with.py
+-rw-r--r--   0 root         (0) root         (0)     1244 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/server_version/server_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.965512 graphdatascience-1.7a1/graphdatascience/system/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/system/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/system/config_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)     2702 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/system/system_endpoints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.965512 graphdatascience-1.7a1/graphdatascience/topological_lp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/topological_lp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/topological_lp/topological_lp_alpha_runner.py
+-rw-r--r--   0 root         (0) root         (0)      343 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/topological_lp/topological_lp_endpoints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.969512 graphdatascience-1.7a1/graphdatascience/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3796 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/utils/util_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)     2137 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/utils/util_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.877512 graphdatascience-1.7a1/graphdatascience.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7238 2023-05-24 12:08:18.000000 graphdatascience-1.7a1/graphdatascience.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4842 2023-05-24 12:08:18.000000 graphdatascience-1.7a1/graphdatascience.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 12:08:18.000000 graphdatascience-1.7a1/graphdatascience.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 12:08:18.000000 graphdatascience-1.7a1/graphdatascience.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      194 2023-05-24 12:08:18.000000 graphdatascience-1.7a1/graphdatascience.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-24 12:08:18.000000 graphdatascience-1.7a1/graphdatascience.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      136 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.873512 graphdatascience-1.7a1/requirements/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.969512 graphdatascience-1.7a1/requirements/base/
+-rw-r--r--   0 root         (0) root         (0)      170 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/requirements/base/base.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/requirements/base/networkx.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/requirements/base/ogb.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 12:08:18.969512 graphdatascience-1.7a1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2176 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/setup.py
```

### Comparing `graphdatascience-1.7/LICENSE` & `graphdatascience-1.7a1/LICENSE`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/PKG-INFO` & `graphdatascience-1.7a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphdatascience
-Version: 1.7
+Version: 1.7a1
 Summary: A Python client for the Neo4j Graph Data Science (GDS) library
 Home-page: https://neo4j.com/product/graph-data-science/
 Author: Neo4j
 Author-email: team-gds@neo4j.org
 License: Apache License 2.0
 Project-URL: Documentation, https://neo4j.com/docs/graph-data-science-client/current/
 Project-URL: Source, https://github.com/neo4j/graph-data-science-client
```

### Comparing `graphdatascience-1.7/README.md` & `graphdatascience-1.7a1/README.md`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/algo/algo_endpoints.py` & `graphdatascience-1.7a1/graphdatascience/algo/algo_endpoints.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/algo/algo_proc_runner.py` & `graphdatascience-1.7a1/graphdatascience/algo/algo_proc_runner.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/call_builder.py` & `graphdatascience-1.7a1/graphdatascience/call_builder.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/caller_base.py` & `graphdatascience-1.7a1/graphdatascience/caller_base.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/endpoints.py` & `graphdatascience-1.7a1/graphdatascience/endpoints.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/error/client_only_endpoint.py` & `graphdatascience-1.7a1/graphdatascience/error/client_only_endpoint.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/error/deprecation_warning.py` & `graphdatascience-1.7a1/graphdatascience/error/deprecation_warning.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import warnings
 from functools import wraps
 from logging import warning
 from typing import Any, Callable, Optional, TypeVar, cast
 
 from ..server_version.server_version import ServerVersion
 
 F = TypeVar("F", bound=Callable[..., Any])
@@ -17,15 +16,14 @@
     deprecation_start_version: Optional[ServerVersion] = None,
 ) -> Callable[[F], F]:
     def decorator(func: F) -> F:
         wraps(func)
 
         @wraps(func)
         def wrapper(self: WithServerVersion, *args: Any, **kwargs: Any) -> Any:
-            if deprecation_start_version and self._server_version >= deprecation_start_version:
+            if deprecation_start_version and self._server_version > deprecation_start_version:
                 warning(f"Deprecated in favor of {new_procedure}")
-                warnings.warn(f"Deprecated in favor of {new_procedure}", DeprecationWarning)
             return func(self, *args, **kwargs)
 
         return cast(F, wrapper)
 
     return decorator
```

### Comparing `graphdatascience-1.7/graphdatascience/error/endpoint_suggester.py` & `graphdatascience-1.7a1/graphdatascience/error/endpoint_suggester.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/error/illegal_attr_checker.py` & `graphdatascience-1.7a1/graphdatascience/error/illegal_attr_checker.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/error/uncallable_namespace.py` & `graphdatascience-1.7a1/graphdatascience/error/uncallable_namespace.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/graph/graph_alpha_proc_runner.py` & `graphdatascience-1.7a1/graphdatascience/graph/graph_alpha_proc_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import os
 from typing import List, Optional, Union
 
 from pandas import DataFrame
 
 from ..error.client_only_endpoint import client_only_endpoint
-from ..error.deprecation_warning import deprecation_warning
 from ..error.illegal_attr_checker import IllegalAttrChecker
 from ..error.uncallable_namespace import UncallableNamespace
 from ..server_version.compatible_with import compatible_with
 from ..server_version.server_version import ServerVersion
 from .graph_alpha_project_runner import GraphAlphaProjectRunner
 from .graph_entity_ops_runner import GraphLabelRunner, GraphPropertyRunner
 from .graph_object import Graph
-from .graph_sample_runner import GraphAlphaSampleRunner
+from .graph_sample_runner import GraphSampleRunner
 
 
 class GraphAlphaProcRunner(UncallableNamespace, IllegalAttrChecker):
     @property
-    def sample(self) -> GraphAlphaSampleRunner:
+    def sample(self) -> GraphSampleRunner:
         self._namespace += ".sample"
-        return GraphAlphaSampleRunner(self._query_runner, self._namespace, self._server_version)
+        return GraphSampleRunner(self._query_runner, self._namespace, self._server_version)
 
     @property
     def graphProperty(self) -> GraphPropertyRunner:
         self._namespace += ".graphProperty"
         return GraphPropertyRunner(self._query_runner, self._namespace, self._server_version)
 
     @property
@@ -33,15 +32,14 @@
 
     @property
     def project(self) -> GraphAlphaProjectRunner:
         self._namespace += ".project"
         return GraphAlphaProjectRunner(self._query_runner, self._namespace, self._server_version)
 
     @client_only_endpoint("gds.alpha.graph")
-    @deprecation_warning("gds.graph.construct", ServerVersion(2, 1, 0))
     @compatible_with("construct", min_inclusive=ServerVersion(2, 1, 0))
     def construct(
         self,
         graph_name: str,
         nodes: Union[DataFrame, List[DataFrame]],
         relationships: Union[DataFrame, List[DataFrame]],
         concurrency: int = 4,
```

### Comparing `graphdatascience-1.7/graphdatascience/graph/graph_alpha_project_runner.py` & `graphdatascience-1.7a1/graphdatascience/graph/graph_alpha_project_runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-from typing import Any, Tuple
+from typing import Any
 
 from pandas import Series
 
 from graphdatascience.error.illegal_attr_checker import IllegalAttrChecker
-from graphdatascience.graph.graph_object import Graph
 from graphdatascience.server_version.compatible_with import compatible_with
 from graphdatascience.server_version.server_version import ServerVersion
 
 
 class GraphAlphaProjectRunner(IllegalAttrChecker):
     @compatible_with("remote", min_inclusive=ServerVersion(2, 4, 0))
-    def remote(self, graph_name: str, query: str, remote_database: str, **config: Any) -> Tuple[Graph, "Series[Any]"]:
+    def remote(self, graph_name: str, query: str, remote_database: str, **config: Any) -> "Series[Any]":
         self._namespace += ".remote"
-        procedure_query = f"CALL {self._namespace}($graph_name, $query, $token, $host, $remote_database, $config)"
+        query = f"CALL {self._namespace}($graph_name, $query, $token, $host, $remote_database, $config)"
         params = {"graph_name": graph_name, "query": query, "remote_database": remote_database, "config": config}
-        result = self._query_runner.run_query(procedure_query, params).squeeze()
-        return Graph(graph_name, self._query_runner, self._server_version), result
+        return self._query_runner.run_query(query, params).squeeze()  # type: ignore
```

### Comparing `graphdatascience-1.7/graphdatascience/graph/graph_beta_proc_runner.py` & `graphdatascience-1.7a1/graphdatascience/graph/graph_beta_proc_runner.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/graph/graph_endpoints.py` & `graphdatascience-1.7a1/graphdatascience/graph/graph_endpoints.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/graph/graph_entity_ops_runner.py` & `graphdatascience-1.7a1/graphdatascience/graph/graph_entity_ops_runner.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/graph/graph_export_runner.py` & `graphdatascience-1.7a1/graphdatascience/graph/graph_export_runner.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/graph/graph_object.py` & `graphdatascience-1.7a1/graphdatascience/graph/graph_object.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/graph/graph_proc_runner.py` & `graphdatascience-1.7a1/graphdatascience/graph/graph_proc_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 import pathlib
 import sys
 from logging import warning
 from typing import Any, ContextManager, Dict, List, Optional, Union
 
 import pandas as pd
 from multimethod import multimethod
@@ -10,14 +9,15 @@
 
 from ..error.client_only_endpoint import client_only_endpoint
 from ..error.deprecation_warning import deprecation_warning
 from ..error.illegal_attr_checker import IllegalAttrChecker
 from ..error.uncallable_namespace import UncallableNamespace
 from ..server_version.compatible_with import compatible_with
 from ..server_version.server_version import ServerVersion
+from .graph_alpha_proc_runner import GraphAlphaProcRunner
 from .graph_entity_ops_runner import (
     GraphElementPropertyRunner,
     GraphNodePropertiesRunner,
     GraphRelationshipPropertiesRunner,
     GraphRelationshipRunner,
     GraphRelationshipsRunner,
 )
@@ -41,83 +41,46 @@
             return as_file(files(package) / os.path.normpath(resource))
         else:
             from importlib.resources import path
 
             return path(package, resource)
 
     @client_only_endpoint("gds.graph")
-    @compatible_with("construct", min_inclusive=ServerVersion(2, 1, 0))
-    def construct(
-        self,
-        graph_name: str,
-        nodes: Union[DataFrame, List[DataFrame]],
-        relationships: Union[DataFrame, List[DataFrame]],
-        concurrency: int = 4,
-        undirected_relationship_types: Optional[List[str]] = None,
-    ) -> Graph:
-        nodes = nodes if isinstance(nodes, List) else [nodes]
-        relationships = relationships if isinstance(relationships, List) else [relationships]
-
-        errors = []
-
-        exists = self._query_runner.run_query(
-            f"CALL gds.graph.exists('{graph_name}') YIELD exists", custom_error=False
-        ).squeeze()
-
-        # compare against True as (1) unit tests return None here and (2) numpys True does not work with `is True`.
-        if exists == True:  # noqa: E712
-            errors.append(
-                f"Graph '{graph_name}' already exists. Please drop the existing graph or use a different name."
-            )
-
-        for idx, node_df in enumerate(nodes):
-            if "nodeId" not in node_df.columns.values:
-                errors.append(f"Node dataframe at index {idx} needs to contain a 'nodeId' column.")
-
-        for idx, rel_df in enumerate(relationships):
-            for expected_col in ["sourceNodeId", "targetNodeId"]:
-                if expected_col not in rel_df.columns.values:
-                    errors.append(f"Relationship dataframe at index {idx} needs to contain a '{expected_col}' column.")
-
-        if self._server_version < ServerVersion(2, 3, 0) and undirected_relationship_types:
-            errors.append("The parameter 'undirected_relationship_types' is only supported since GDS 2.3.0.")
-
-        if len(errors) > 0:
-            raise ValueError(os.linesep.join(errors))
-
-        constructor = self._query_runner.create_graph_constructor(
-            graph_name, concurrency, undirected_relationship_types
-        )
-        constructor.run(nodes, relationships)
-
-        return Graph(graph_name, self._query_runner, self._server_version)
-
-    @client_only_endpoint("gds.graph")
     def load_cora(self, graph_name: str = "cora", undirected: bool = False) -> Graph:
         with self._path("graphdatascience.resources.cora", "cora_nodes_gzip.pkl") as nodes_resource:
             nodes = read_pickle(nodes_resource, compression="gzip")
 
         with self._path("graphdatascience.resources.cora", "cora_rels_gzip.pkl") as rels_resource:
             rels = read_pickle(rels_resource, compression="gzip")
 
+        self._namespace = "gds.alpha.graph"
+        alpha_proc_runner = GraphAlphaProcRunner(self._query_runner, self._namespace, self._server_version)
+
         undirected_relationship_types = ["*"] if undirected else []
 
-        return self.construct(graph_name, nodes, rels, undirected_relationship_types=undirected_relationship_types)
+        return alpha_proc_runner.construct(
+            graph_name, nodes, rels, undirected_relationship_types=undirected_relationship_types
+        )
 
     @client_only_endpoint("gds.graph")
     def load_karate_club(self, graph_name: str = "karate_club", undirected: bool = False) -> Graph:
         nodes = pd.DataFrame({"nodeId": range(1, 35)})
         nodes["labels"] = "Person"
 
         with self._path("graphdatascience.resources.karate", "karate_club_gzip.pkl") as rels_resource:
             rels = read_pickle(rels_resource, compression="gzip")
 
+        self._namespace = "gds.alpha.graph"
+        alpha_proc_runner = GraphAlphaProcRunner(self._query_runner, self._namespace, self._server_version)
+
         undirected_relationship_types = ["*"] if undirected else []
 
-        return self.construct(graph_name, nodes, rels, undirected_relationship_types=undirected_relationship_types)
+        return alpha_proc_runner.construct(
+            graph_name, nodes, rels, undirected_relationship_types=undirected_relationship_types
+        )
 
     @client_only_endpoint("gds.graph")
     def load_imdb(self, graph_name: str = "imdb", undirected: bool = True) -> Graph:
         if self._server_version < ServerVersion(2, 3, 0):
             raise ValueError("The IMDB dataset loading is only supported by GDS 2.3 or later.")
 
         with self._path("graphdatascience.resources.imdb", "imdb_movies_with_genre_gzip.pkl") as nodes_resource:
@@ -130,21 +93,26 @@
             directors = read_pickle(nodes_resource, compression="gzip")
 
         with self._path("graphdatascience.resources.imdb", "imdb_acted_in_rels_gzip.pkl") as rels_resource:
             acted_in_rels = read_pickle(rels_resource, compression="gzip")
         with self._path("graphdatascience.resources.imdb", "imdb_directed_in_rels_gzip.pkl") as rels_resource:
             directed_in_rels = read_pickle(rels_resource, compression="gzip")
 
+        self._namespace = "gds.alpha.graph"
+        alpha_proc_runner = GraphAlphaProcRunner(self._query_runner, self._namespace, self._server_version)
+
         nodes = [movies_with_genre, movies_without_genre, actors, directors]
         rels = [acted_in_rels, directed_in_rels]
 
         # Default undirected which matches raw data
         undirected_relationship_types = ["*"] if undirected else []
 
-        return self.construct(graph_name, nodes, rels, undirected_relationship_types=undirected_relationship_types)
+        return alpha_proc_runner.construct(
+            graph_name, nodes, rels, undirected_relationship_types=undirected_relationship_types
+        )
 
     @property
     def sample(self) -> GraphSampleRunner:
         self._namespace += ".sample"
         return GraphSampleRunner(self._query_runner, self._namespace, self._server_version)
 
     @property
```

### Comparing `graphdatascience-1.7/graphdatascience/graph/graph_project_runner.py` & `graphdatascience-1.7a1/graphdatascience/graph/graph_project_runner.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/graph/graph_sample_runner.py` & `graphdatascience-1.7a1/graphdatascience/graph/graph_sample_runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,39 @@
 from typing import Any, Tuple
 
 from pandas import Series
 
-from ..error.deprecation_warning import deprecation_warning
 from ..error.illegal_attr_checker import IllegalAttrChecker
 from ..server_version.compatible_with import compatible_with
 from ..server_version.server_version import ServerVersion
 from .graph_object import Graph
 from .graph_type_check import from_graph_type_check
 
 
-class GraphAlphaSampleRunner(IllegalAttrChecker):
+class GraphSampleRunner(IllegalAttrChecker):
     @compatible_with("construct", min_inclusive=ServerVersion(2, 2, 0))
-    @deprecation_warning("gds.graph.sample.rwr", ServerVersion(2, 4, 0))
     @from_graph_type_check
     def rwr(self, graph_name: str, from_G: Graph, **config: Any) -> Tuple[Graph, "Series[Any]"]:
-        runner = RWRRunner(self._query_runner, self._namespace + ".rwr", self._server_version)
-        return runner(graph_name, from_G, **config)
-
-
-class GraphSampleRunner(IllegalAttrChecker):
-    @property
-    def rwr(self) -> "RWRRunner":
-        return RWRRunner(self._query_runner, self._namespace + ".rwr", self._server_version)
-
-    @property
-    def cnarw(self) -> "CNARWRunner":
-        return CNARWRunner(self._query_runner, self._namespace + ".cnarw", self._server_version)
+        self._namespace += ".rwr"
 
-
-class RWRRunner(IllegalAttrChecker):
-    @compatible_with("construct", min_inclusive=ServerVersion(2, 2, 0))
-    @from_graph_type_check
-    def __call__(self, graph_name: str, from_G: Graph, **config: Any) -> Tuple[Graph, "Series[Any]"]:
         query = f"CALL {self._namespace}($graph_name, $from_graph_name, $config)"
         params = {
             "graph_name": graph_name,
             "from_graph_name": from_G.name(),
             "config": config,
         }
 
         result = self._query_runner.run_query_with_logging(query, params).squeeze()
 
         return Graph(graph_name, self._query_runner, self._server_version), result
 
+    @property
+    def cnarw(self) -> "CNARWRunner":
+        return CNARWRunner(self._query_runner, self._namespace + ".cnarw", self._server_version)
+
 
 class CNARWRunner(IllegalAttrChecker):
     @compatible_with("construct", min_inclusive=ServerVersion(2, 4, 0))
     @from_graph_type_check
     def __call__(self, graph_name: str, from_G: Graph, **config: Any) -> Tuple[Graph, "Series[Any]"]:
         query = f"CALL {self._namespace}($graph_name, $from_graph_name, $config)"
         params = {
```

### Comparing `graphdatascience-1.7/graphdatascience/graph/graph_type_check.py` & `graphdatascience-1.7a1/graphdatascience/graph/graph_type_check.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/graph/nx_loader.py` & `graphdatascience-1.7a1/graphdatascience/graph/nx_loader.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/graph/ogb_loader.py` & `graphdatascience-1.7a1/graphdatascience/graph/ogb_loader.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/graph_data_science.py` & `graphdatascience-1.7a1/graphdatascience/graph_data_science.py`

 * *Files 8% similar despite different names*

```diff
@@ -99,28 +99,40 @@
             if isinstance(endpoint, str):
                 driver.close()
 
         self._server_version = ServerVersion.from_string(server_version_string)
         self._query_runner.set_server_version(self._server_version)
 
         if arrow and self._server_version >= ServerVersion(2, 1, 0):
-            arrow_info: "Series[Any]" = self._query_runner.run_query(
-                "CALL gds.debug.arrow()", custom_error=False
-            ).squeeze()
-            listen_address: str = arrow_info.get("advertisedListenAddress", arrow_info["listenAddress"])  # type: ignore
-            if arrow_info["running"]:
-                self._query_runner = ArrowQueryRunner(
-                    listen_address,
-                    self._query_runner,
-                    self._server_version,
-                    auth,
-                    driver.encrypted,
-                    arrow_disable_server_verification,
-                    arrow_tls_root_certs,
-                )
+            try:
+                arrow_info: "Series[Any]" = self._query_runner.run_query(
+                    "CALL gds.debug.arrow()", custom_error=False
+                ).squeeze()
+                listen_address: str = arrow_info.get(
+                    "advertisedListenAddress", arrow_info["listenAddress"]
+                )  # type: ignore
+                if arrow_info["running"]:
+                    self._query_runner = ArrowQueryRunner(
+                        listen_address,
+                        self._query_runner,
+                        self._server_version,
+                        auth,
+                        driver.encrypted,
+                        arrow_disable_server_verification,
+                        arrow_tls_root_certs,
+                    )
+            except Exception as e:
+                # AuraDS does not have arrow support at this time, so we should not warn about it.
+                # TODO: Remove this check when AuraDS gets arrow support.
+                if (
+                    "There is no procedure with the name `gds.debug.arrow` "
+                    "registered for this database instance." not in str(e)
+                ):
+                    warnings.warn(f"Could not initialize GDS Flight Server client: {e}")
+
         if aura_db_connection_info:
             if self._server_version >= ServerVersion(2, 4, 0):
                 self._query_runner = AuraDbArrowQueryRunner(self._query_runner, aura_db_connection_info)
             else:
                 warnings.warn(
                     f"AuraDB connection info was provided but GDS version {self._server_version} \
                         does not support connecting to AuraDB"
```

### Comparing `graphdatascience-1.7/graphdatascience/ignored_server_endpoints.py` & `graphdatascience-1.7a1/graphdatascience/ignored_server_endpoints.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/model/graphsage_model.py` & `graphdatascience-1.7a1/graphdatascience/model/graphsage_model.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/model/link_prediction_model.py` & `graphdatascience-1.7a1/graphdatascience/model/link_prediction_model.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/model/model.py` & `graphdatascience-1.7a1/graphdatascience/model/model.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/model/model_alpha_proc_runner.py` & `graphdatascience-1.7a1/graphdatascience/model/model_alpha_proc_runner.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/model/model_beta_proc_runner.py` & `graphdatascience-1.7a1/graphdatascience/model/model_beta_proc_runner.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/model/model_endpoints.py` & `graphdatascience-1.7a1/graphdatascience/model/model_endpoints.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/model/model_proc_runner.py` & `graphdatascience-1.7a1/graphdatascience/model/model_proc_runner.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/model/model_resolver.py` & `graphdatascience-1.7a1/graphdatascience/model/model_resolver.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/model/node_classification_model.py` & `graphdatascience-1.7a1/graphdatascience/model/node_classification_model.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/model/node_regression_model.py` & `graphdatascience-1.7a1/graphdatascience/model/node_regression_model.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/model/pipeline_model.py` & `graphdatascience-1.7a1/graphdatascience/model/pipeline_model.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/pipeline/classification_training_pipeline.py` & `graphdatascience-1.7a1/graphdatascience/pipeline/classification_training_pipeline.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/pipeline/lp_pipeline_create_runner.py` & `graphdatascience-1.7a1/graphdatascience/pipeline/lp_pipeline_create_runner.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/pipeline/lp_training_pipeline.py` & `graphdatascience-1.7a1/graphdatascience/pipeline/lp_training_pipeline.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/pipeline/nc_pipeline_create_runner.py` & `graphdatascience-1.7a1/graphdatascience/pipeline/nc_pipeline_create_runner.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/pipeline/nc_training_pipeline.py` & `graphdatascience-1.7a1/graphdatascience/pipeline/nc_training_pipeline.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/pipeline/nr_pipeline_create_runner.py` & `graphdatascience-1.7a1/graphdatascience/pipeline/nr_pipeline_create_runner.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/pipeline/nr_training_pipeline.py` & `graphdatascience-1.7a1/graphdatascience/pipeline/nr_training_pipeline.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/pipeline/pipeline_beta_proc_runner.py` & `graphdatascience-1.7a1/graphdatascience/pipeline/pipeline_beta_proc_runner.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/pipeline/pipeline_endpoints.py` & `graphdatascience-1.7a1/graphdatascience/pipeline/pipeline_endpoints.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/pipeline/pipeline_proc_runner.py` & `graphdatascience-1.7a1/graphdatascience/pipeline/pipeline_proc_runner.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/pipeline/training_pipeline.py` & `graphdatascience-1.7a1/graphdatascience/pipeline/training_pipeline.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/query_runner/arrow_graph_constructor.py` & `graphdatascience-1.7a1/graphdatascience/query_runner/arrow_graph_constructor.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/query_runner/arrow_query_runner.py` & `graphdatascience-1.7a1/graphdatascience/query_runner/arrow_query_runner.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/query_runner/aura_db_arrow_query_runner.py` & `graphdatascience-1.7a1/graphdatascience/query_runner/aura_db_arrow_query_runner.py`

 * *Files 20% similar despite different names*

```diff
@@ -60,26 +60,14 @@
         if params is None:
             params = {}
 
         if "gds.alpha.graph.project.remote" in query:
             token, aura_db_arrow_endpoint = self._get_or_request_auth_pair()
             params["token"] = token
             params["host"] = aura_db_arrow_endpoint
-            params["config"] = {"useEncryption": False}
-
-        elif ".write" in query and "config" in params and "remote" in params["config"] and params["config"]["remote"]:
-            token, aura_db_arrow_endpoint = self._get_or_request_auth_pair()
-            host, port_string = aura_db_arrow_endpoint.split(":")
-            del params["config"]["remote"]
-            params["config"]["arrowConnectionInfo"] = {
-                "hostname": host,
-                "port": int(port_string),
-                "bearerToken": token,
-                "useEncryption": False,
-            }
 
         return self._fallback_query_runner.run_query(query, params, database, custom_error)
 
     def set_database(self, database: str) -> None:
         self._fallback_query_runner.set_database(database)
 
     def database(self) -> Optional[str]:
```

### Comparing `graphdatascience-1.7/graphdatascience/query_runner/cypher_graph_constructor.py` & `graphdatascience-1.7a1/graphdatascience/query_runner/cypher_graph_constructor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-import itertools
 import os
 import warnings
 from dataclasses import dataclass
+from functools import reduce
 from typing import Any, Dict, List, Optional, Set, Tuple
 from uuid import uuid4
 
 from pandas import DataFrame, concat
 
 from .graph_constructor import GraphConstructor
 from .query_runner import QueryRunner
 from graphdatascience.server_version.server_version import ServerVersion
 
 
-class CypherProjectionApi:
+class CypherAggregationApi:
     RELATIONSHIP_TYPE = "relationshipType"
     SOURCE_NODE_LABEL = "sourceNodeLabels"
-    TARGET_NODE_LABEL = "targetNodeLabels"
     SOURCE_NODE_PROPERTIES = "sourceNodeProperties"
-    TARGET_NODE_PROPERTIES = "targetNodeProperties"
     REL_PROPERTIES = "properties"
-    REL_PROPERTIES_NEW = "relationshipProperties"
 
 
 @dataclass
 class EntityColumnSchema:
     all: Set[str]
     properties: Set[str]
 
@@ -70,22 +67,18 @@
         if self._should_warn_about_arrow_missing():
             warnings.warn(
                 "GDS Enterprise users can use Apache Arrow for fast graph construction; please see the documentation "
                 "for instructions on how to enable it. Without Arrow enabled, this installation will use community "
                 "edition graph construction (slower)"
             )
 
-        # New Cypher propjection supports concurrency since 2.3.0
+        # Cypher aggregation supports concurrency since 2.3.0
         if self._server_version >= ServerVersion(2, 3, 0):
-            self.CypherProjectionRunner(
-                self._query_runner,
-                self._graph_name,
-                self._concurrency,
-                self._undirected_relationship_types,
-                self._server_version,
+            self.CypherAggregationRunner(
+                self._query_runner, self._graph_name, self._concurrency, self._undirected_relationship_types
             ).run(node_dfs, relationship_dfs)
         else:
             assert not self._undirected_relationship_types, "This should have been raised earlier."
 
             def graph_construct_error_multidf(element: str) -> str:
                 return f"Graph construction only supports a single {element} dataframe on GDS versions prior to GDS 2.3"
 
@@ -94,17 +87,15 @@
 
             if len(relationship_dfs) > 1:
                 raise ValueError(graph_construct_error_multidf("relationship"))
 
             node_df = node_dfs[0]
             rel_df = relationship_dfs[0]
 
-            self.LegacyCypherProjectionRunner(self._query_runner, self._graph_name, self._concurrency).run(
-                node_df, rel_df
-            )
+            self.CyperProjectionRunner(self._query_runner, self._graph_name, self._concurrency).run(node_df, rel_df)
 
     def _should_warn_about_arrow_missing(self) -> bool:
         try:
             license: str = self._query_runner.run_query(
                 "CALL gds.debug.sysInfo() YIELD key, value WHERE key = 'gdsEdition' RETURN value", custom_error=False
             ).squeeze()
             should_warn = license == "Licensed"
@@ -116,98 +107,81 @@
             ):
                 should_warn = False
             else:
                 raise e
 
         return should_warn
 
-    class CypherProjectionRunner:
+    class CypherAggregationRunner:
         _BIT_COL_SUFFIX = "_is_present" + str(uuid4())
 
         def __init__(
             self,
             query_runner: QueryRunner,
             graph_name: str,
             concurrency: int,
             undirected_relationship_types: Optional[List[str]],
-            server_version: ServerVersion,
         ):
             self._query_runner = query_runner
             self._concurrency = concurrency
             self._graph_name = graph_name
             self._undirected_relationship_types = undirected_relationship_types
-            self._server_version = server_version
 
         def run(self, node_dfs: List[DataFrame], relationship_dfs: List[DataFrame]) -> None:
             graph_schema = self.schema(node_dfs, relationship_dfs)
 
             same_cols = graph_schema.all_rels.all.intersection(graph_schema.all_nodes.all)
 
             if same_cols:
                 raise ValueError(
                     "Expected disjoint column names in node and relationship df "
                     f"but the columns {same_cols} exist in both dfs. Please rename the column in one df."
                 )
 
-            is_cypher_projection_v2 = self._server_version >= ServerVersion(2, 4, 0)
-
-            rel_properties_key = (
-                CypherProjectionApi.REL_PROPERTIES_NEW
-                if is_cypher_projection_v2
-                else CypherProjectionApi.REL_PROPERTIES
-            )
-
-            aligned_node_dfs = self.adjust_node_dfs(node_dfs, graph_schema, rel_properties_key)
-            aligned_rel_dfs = self.adjust_rel_dfs(relationship_dfs, graph_schema, rel_properties_key)
+            aligned_node_dfs = self.adjust_node_dfs(node_dfs, graph_schema)
+            aligned_rel_dfs = self.adjust_rel_dfs(relationship_dfs, graph_schema)
 
             # concat instead of join as we want to first have all nodes and then the rels
             # this way we don't duplicate the node property data and its cheaper
             combined_df: DataFrame = concat(aligned_node_dfs + aligned_rel_dfs, ignore_index=True, copy=False)
             # make column order deterministic
             combined_df = combined_df[sorted(combined_df)]
 
             # using a List and not a Set to preserve the order
             combined_cols: List[str] = combined_df.columns.tolist()
 
             property_clauses: List[str] = [
                 self.check_value_clause(combined_cols, prop_col)
-                for prop_col in [CypherProjectionApi.SOURCE_NODE_PROPERTIES, rel_properties_key]
+                for prop_col in [CypherAggregationApi.SOURCE_NODE_PROPERTIES, CypherAggregationApi.REL_PROPERTIES]
             ]
 
             source_node_labels_clause = (
-                self.check_value_clause(combined_cols, CypherProjectionApi.SOURCE_NODE_LABEL)
-                if CypherProjectionApi.SOURCE_NODE_LABEL in combined_cols
+                self.check_value_clause(combined_cols, CypherAggregationApi.SOURCE_NODE_LABEL)
+                if CypherAggregationApi.SOURCE_NODE_LABEL in combined_cols
                 else ""
             )
             rel_type_clause = (
                 self.check_value_clause(combined_cols, "relationshipType")
                 if "relationshipType" in combined_cols
                 else ""
             )
             target_id_clause = self.check_value_clause(combined_cols, "targetNodeId")
 
-            nodes_config_part = self.nodes_config_part(graph_schema.nodes_per_df, is_cypher_projection_v2)
-            rels_config_part = self.rels_config_part(graph_schema.rels_per_df, rel_properties_key)
-
-            if is_cypher_projection_v2:
-                data_config = f"{{{', '.join(itertools.chain(nodes_config_part, rels_config_part))}}}"
-            else:
-                data_config = f"{{{', '.join(nodes_config_part)}}}, {{{', '.join(rels_config_part)}}}"
+            nodes_config = self.nodes_config(graph_schema.nodes_per_df)
+            rels_config = self.rels_config(graph_schema.rels_per_df)
 
             property_clauses_str = f"{os.linesep}" if len(property_clauses) > 0 else ""
             property_clauses_str += f"{os.linesep}".join(property_clauses)[:-2]  # remove the final comma
 
-            tier = "" if is_cypher_projection_v2 else ".alpha"
-
             query = (
                 "UNWIND $data AS data"
                 f" WITH data, {source_node_labels_clause}{rel_type_clause}{target_id_clause}{property_clauses_str}"
-                f" RETURN gds{tier}.graph.project("
+                " RETURN gds.alpha.graph.project("
                 f"$graph_name, data[{combined_cols.index('sourceNodeId')}], targetNodeId, "
-                f"{data_config}, $configuration)"
+                f"{nodes_config}, {rels_config}, $configuration)"
             )
 
             configuration = {
                 "readConcurrency": self._concurrency,
                 "undirectedRelationshipTypes": self._undirected_relationship_types,
             }
 
@@ -241,125 +215,115 @@
                 rel_cols = set(df.columns.tolist())
                 rel_schema.append(
                     EntityColumnSchema(rel_cols, rel_cols - {"sourceNodeId", "targetNodeId", "relationshipType"})
                 )
 
             return GraphColumnSchema(node_schema, rel_schema)
 
-        def adjust_node_dfs(
-            self, node_dfs: List[DataFrame], schema: GraphColumnSchema, rel_properties_key: str
-        ) -> List[DataFrame]:
+        def adjust_node_dfs(self, node_dfs: List[DataFrame], schema: GraphColumnSchema) -> List[DataFrame]:
             adjusted_dfs = []
 
             for i, df in enumerate(node_dfs):
                 node_dict: Dict[str, Any] = {
                     "sourceNodeId": df["nodeId"],
                     "targetNodeId": -1,
                     f"targetNodeId{self._BIT_COL_SUFFIX}": False,
                 }
 
-                if CypherProjectionApi.RELATIONSHIP_TYPE in schema.all_rels.all:
-                    node_dict[CypherProjectionApi.RELATIONSHIP_TYPE] = None
-                    node_dict[CypherProjectionApi.RELATIONSHIP_TYPE + self._BIT_COL_SUFFIX] = False
+                if CypherAggregationApi.RELATIONSHIP_TYPE in schema.all_rels.all:
+                    node_dict[CypherAggregationApi.RELATIONSHIP_TYPE] = None
+                    node_dict[CypherAggregationApi.RELATIONSHIP_TYPE + self._BIT_COL_SUFFIX] = False
 
                 if "labels" in schema.nodes_per_df[i].all:
-                    node_dict[CypherProjectionApi.SOURCE_NODE_LABEL + self._BIT_COL_SUFFIX] = True
-                    node_dict[CypherProjectionApi.SOURCE_NODE_LABEL] = df["labels"]
+                    node_dict[CypherAggregationApi.SOURCE_NODE_LABEL + self._BIT_COL_SUFFIX] = True
+                    node_dict[CypherAggregationApi.SOURCE_NODE_LABEL] = df["labels"]
                 elif "labels" in schema.all_nodes.all:
-                    node_dict[CypherProjectionApi.SOURCE_NODE_LABEL + self._BIT_COL_SUFFIX] = False
-                    node_dict[CypherProjectionApi.SOURCE_NODE_LABEL] = ""
+                    node_dict[CypherAggregationApi.SOURCE_NODE_LABEL + self._BIT_COL_SUFFIX] = False
+                    node_dict[CypherAggregationApi.SOURCE_NODE_LABEL] = ""
 
                 def collect_to_dict(row: Dict[str, Any]) -> Dict[str, Any]:
                     return {column: row[column] for column in schema.nodes_per_df[i].properties}
 
                 node_dict_df = DataFrame(node_dict)
-                node_dict_df[CypherProjectionApi.SOURCE_NODE_PROPERTIES] = df.apply(collect_to_dict, axis=1)
-                node_dict_df[CypherProjectionApi.SOURCE_NODE_PROPERTIES + self._BIT_COL_SUFFIX] = True
-                node_dict_df[rel_properties_key] = None
-                node_dict_df[rel_properties_key + self._BIT_COL_SUFFIX] = False
+                node_dict_df[CypherAggregationApi.SOURCE_NODE_PROPERTIES] = df.apply(collect_to_dict, axis=1)
+                node_dict_df[CypherAggregationApi.SOURCE_NODE_PROPERTIES + self._BIT_COL_SUFFIX] = True
+                node_dict_df[CypherAggregationApi.REL_PROPERTIES] = None
+                node_dict_df[CypherAggregationApi.REL_PROPERTIES + self._BIT_COL_SUFFIX] = False
 
                 adjusted_dfs.append(node_dict_df)
 
             return adjusted_dfs
 
-        def adjust_rel_dfs(
-            self, rel_dfs: List[DataFrame], schema: GraphColumnSchema, rel_properties_key: str
-        ) -> List[DataFrame]:
+        def adjust_rel_dfs(self, rel_dfs: List[DataFrame], schema: GraphColumnSchema) -> List[DataFrame]:
             adjusted_dfs = []
 
             for i, df in enumerate(rel_dfs):
                 rel_dict: Dict[str, Any] = {
                     "sourceNodeId": df["sourceNodeId"],
                     "targetNodeId": df["targetNodeId"],
                     f"targetNodeId{self._BIT_COL_SUFFIX}": True,
                 }
 
-                if CypherProjectionApi.RELATIONSHIP_TYPE in schema.rels_per_df[i].all:
-                    rel_dict[CypherProjectionApi.RELATIONSHIP_TYPE + self._BIT_COL_SUFFIX] = True
-                    rel_dict[CypherProjectionApi.RELATIONSHIP_TYPE] = df[CypherProjectionApi.RELATIONSHIP_TYPE]
-                elif CypherProjectionApi.RELATIONSHIP_TYPE in schema.all_rels.all:
-                    rel_dict[CypherProjectionApi.RELATIONSHIP_TYPE + self._BIT_COL_SUFFIX] = False
-                    rel_dict[CypherProjectionApi.RELATIONSHIP_TYPE] = None
+                if CypherAggregationApi.RELATIONSHIP_TYPE in schema.rels_per_df[i].all:
+                    rel_dict[CypherAggregationApi.RELATIONSHIP_TYPE + self._BIT_COL_SUFFIX] = True
+                    rel_dict[CypherAggregationApi.RELATIONSHIP_TYPE] = df[CypherAggregationApi.RELATIONSHIP_TYPE]
+                elif CypherAggregationApi.RELATIONSHIP_TYPE in schema.all_rels.all:
+                    rel_dict[CypherAggregationApi.RELATIONSHIP_TYPE + self._BIT_COL_SUFFIX] = False
+                    rel_dict[CypherAggregationApi.RELATIONSHIP_TYPE] = None
 
                 if "labels" in schema.all_nodes.all:
-                    rel_dict[CypherProjectionApi.SOURCE_NODE_LABEL] = None
-                    rel_dict[CypherProjectionApi.SOURCE_NODE_LABEL + self._BIT_COL_SUFFIX] = False
+                    rel_dict[CypherAggregationApi.SOURCE_NODE_LABEL] = None
+                    rel_dict[CypherAggregationApi.SOURCE_NODE_LABEL + self._BIT_COL_SUFFIX] = False
 
                 def collect_to_dict(row: Dict[str, Any]) -> Dict[str, Any]:
                     return {column: row[column] for column in schema.rels_per_df[i].properties}
 
                 rel_dict_df = DataFrame(rel_dict)
-                rel_dict_df[rel_properties_key] = df.apply(collect_to_dict, axis=1)
-                rel_dict_df[rel_properties_key + self._BIT_COL_SUFFIX] = True
-                rel_dict_df[CypherProjectionApi.SOURCE_NODE_PROPERTIES] = None
-                rel_dict_df[CypherProjectionApi.SOURCE_NODE_PROPERTIES + self._BIT_COL_SUFFIX] = False
+                rel_dict_df[CypherAggregationApi.REL_PROPERTIES] = df.apply(collect_to_dict, axis=1)
+                rel_dict_df[CypherAggregationApi.REL_PROPERTIES + self._BIT_COL_SUFFIX] = True
+                rel_dict_df[CypherAggregationApi.SOURCE_NODE_PROPERTIES] = None
+                rel_dict_df[CypherAggregationApi.SOURCE_NODE_PROPERTIES + self._BIT_COL_SUFFIX] = False
 
                 adjusted_dfs.append(rel_dict_df)
 
             return adjusted_dfs
 
-        def nodes_config_part(self, node_cols: List[EntityColumnSchema], is_cypher_projection_v2: bool) -> List[str]:
+        def nodes_config(self, node_cols: List[EntityColumnSchema]) -> str:
             # Cannot use a dictionary as we need to refer to the `data` variable in the cypher query.
             # Otherwise we would just pass a string such as `data[0]`
             nodes_config_fields: List[str] = []
-            if any(x.has_labels() for x in node_cols):
+            if reduce(lambda x, y: x | y.has_labels(), node_cols, False):
                 nodes_config_fields.append(
-                    f"{CypherProjectionApi.SOURCE_NODE_LABEL}: {CypherProjectionApi.SOURCE_NODE_LABEL}"
+                    f"{CypherAggregationApi.SOURCE_NODE_LABEL}: {CypherAggregationApi.SOURCE_NODE_LABEL}"
                 )
-                if is_cypher_projection_v2:
-                    nodes_config_fields.append(
-                        f"{CypherProjectionApi.TARGET_NODE_LABEL}: NULL",
-                    )
 
             # as we first list all nodes at the top of the df, we don't need to lookup properties for the target node
-            if any(x.has_properties() for x in node_cols):
+            if reduce(lambda x, y: x | y.has_properties(), node_cols, False):
                 nodes_config_fields.append(
-                    f"{CypherProjectionApi.SOURCE_NODE_PROPERTIES}: {CypherProjectionApi.SOURCE_NODE_PROPERTIES}"
+                    f"{CypherAggregationApi.SOURCE_NODE_PROPERTIES}: {CypherAggregationApi.SOURCE_NODE_PROPERTIES}"
                 )
-                if is_cypher_projection_v2:
-                    nodes_config_fields.append(
-                        f"{CypherProjectionApi.TARGET_NODE_PROPERTIES}: NULL",
-                    )
 
-            return nodes_config_fields
+            return f"{{{', '.join(nodes_config_fields)}}}"
 
-        def rels_config_part(self, rel_cols: List[EntityColumnSchema], rel_properties_key: str) -> List[str]:
+        def rels_config(self, rel_cols: List[EntityColumnSchema]) -> str:
             rels_config_fields: List[str] = []
 
-            if any(x.has_rel_type() for x in rel_cols):
+            if reduce(lambda x, y: x | y.has_rel_type(), rel_cols, False):
                 rels_config_fields.append(
-                    f"{CypherProjectionApi.RELATIONSHIP_TYPE}: {CypherProjectionApi.RELATIONSHIP_TYPE}"
+                    f"{CypherAggregationApi.RELATIONSHIP_TYPE}: {CypherAggregationApi.RELATIONSHIP_TYPE}"
                 )
 
-            if any(x.has_properties() for x in rel_cols):
-                rels_config_fields.append(f"{rel_properties_key}: {rel_properties_key}")
+            if reduce(lambda x, y: x | y.has_properties(), rel_cols, False):
+                rels_config_fields.append(
+                    f"{CypherAggregationApi.REL_PROPERTIES}: {CypherAggregationApi.REL_PROPERTIES}"
+                )
 
-            return rels_config_fields
+            return f"{{{', '.join(rels_config_fields)}}}"
 
-    class LegacyCypherProjectionRunner:
+    class CyperProjectionRunner:
         def __init__(self, query_runner: QueryRunner, graph_name: str, concurrency: int):
             self._query_runner = query_runner
             self._concurrency = concurrency
             self._graph_name = graph_name
 
         def run(self, node_df: DataFrame, relationship_df: DataFrame) -> None:
             query = (
```

### Comparing `graphdatascience-1.7/graphdatascience/query_runner/neo4j_query_runner.py` & `graphdatascience-1.7a1/graphdatascience/query_runner/neo4j_query_runner.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/query_runner/query_runner.py` & `graphdatascience-1.7a1/graphdatascience/query_runner/query_runner.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/resources/cora/cora_nodes_gzip.pkl` & `graphdatascience-1.7a1/graphdatascience/resources/cora/cora_nodes_gzip.pkl`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/resources/cora/cora_rels_gzip.pkl` & `graphdatascience-1.7a1/graphdatascience/resources/cora/cora_rels_gzip.pkl`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/resources/cora/serialize_cora.py` & `graphdatascience-1.7a1/graphdatascience/resources/cora/serialize_cora.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/resources/imdb/imdb_acted_in_rels_gzip.pkl` & `graphdatascience-1.7a1/graphdatascience/resources/imdb/imdb_acted_in_rels_gzip.pkl`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/resources/imdb/imdb_actors_gzip.pkl` & `graphdatascience-1.7a1/graphdatascience/resources/imdb/imdb_actors_gzip.pkl`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/resources/imdb/imdb_directed_in_rels_gzip.pkl` & `graphdatascience-1.7a1/graphdatascience/resources/imdb/imdb_directed_in_rels_gzip.pkl`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/resources/imdb/imdb_directors_gzip.pkl` & `graphdatascience-1.7a1/graphdatascience/resources/imdb/imdb_directors_gzip.pkl`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/resources/imdb/imdb_movies_with_genre_gzip.pkl` & `graphdatascience-1.7a1/graphdatascience/resources/imdb/imdb_movies_with_genre_gzip.pkl`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/resources/imdb/imdb_movies_without_genre_gzip.pkl` & `graphdatascience-1.7a1/graphdatascience/resources/imdb/imdb_movies_without_genre_gzip.pkl`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/resources/imdb/raw/edges.pkl` & `graphdatascience-1.7a1/graphdatascience/resources/imdb/raw/edges.pkl`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/resources/imdb/raw/labels.pkl` & `graphdatascience-1.7a1/graphdatascience/resources/imdb/raw/labels.pkl`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/resources/imdb/raw/node_features.pkl` & `graphdatascience-1.7a1/graphdatascience/resources/imdb/raw/node_features.pkl`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/resources/imdb/serialize_imdb.py` & `graphdatascience-1.7a1/graphdatascience/resources/imdb/serialize_imdb.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/resources/karate/karate_club_gzip.pkl` & `graphdatascience-1.7a1/graphdatascience/resources/karate/karate_club_gzip.pkl`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/server_version/compatible_with.py` & `graphdatascience-1.7a1/graphdatascience/server_version/compatible_with.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/server_version/server_version.py` & `graphdatascience-1.7a1/graphdatascience/server_version/server_version.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/system/config_endpoints.py` & `graphdatascience-1.7a1/graphdatascience/system/config_endpoints.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/system/system_endpoints.py` & `graphdatascience-1.7a1/graphdatascience/system/system_endpoints.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,20 +11,14 @@
 class DebugProcRunner(UncallableNamespace, IllegalAttrChecker):
     def sysInfo(self) -> "Series[Any]":
         self._namespace += ".sysInfo"
         query = f"CALL {self._namespace}()"
 
         return self._query_runner.run_query(query).squeeze()  # type: ignore
 
-    def arrow(self) -> "Series[Any]":
-        self._namespace += ".arrow"
-        query = f"CALL {self._namespace}()"
-
-        return self._query_runner.run_query(query).squeeze()  # type: ignore
-
 
 class DirectSystemEndpoints(CallerBase):
     @client_only_endpoint("gds")
     def is_licensed(self) -> bool:
         try:
             license: str = self._query_runner.run_query(
                 "CALL gds.debug.sysInfo() YIELD key, value WHERE key = 'gdsEdition' RETURN value", custom_error=False
```

### Comparing `graphdatascience-1.7/graphdatascience/topological_lp/topological_lp_alpha_runner.py` & `graphdatascience-1.7a1/graphdatascience/topological_lp/topological_lp_alpha_runner.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/utils/util_endpoints.py` & `graphdatascience-1.7a1/graphdatascience/utils/util_endpoints.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience/utils/util_proc_runner.py` & `graphdatascience-1.7a1/graphdatascience/utils/util_proc_runner.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/graphdatascience.egg-info/PKG-INFO` & `graphdatascience-1.7a1/graphdatascience.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphdatascience
-Version: 1.7
+Version: 1.7a1
 Summary: A Python client for the Neo4j Graph Data Science (GDS) library
 Home-page: https://neo4j.com/product/graph-data-science/
 Author: Neo4j
 Author-email: team-gds@neo4j.org
 License: Apache License 2.0
 Project-URL: Documentation, https://neo4j.com/docs/graph-data-science-client/current/
 Project-URL: Source, https://github.com/neo4j/graph-data-science-client
```

### Comparing `graphdatascience-1.7/graphdatascience.egg-info/SOURCES.txt` & `graphdatascience-1.7a1/graphdatascience.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.7/setup.py` & `graphdatascience-1.7a1/setup.py`

 * *Files identical despite different names*

