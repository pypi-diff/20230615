# Comparing `tmp/lolpop-0.1.0a7.tar.gz` & `tmp/lolpop-0.1.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lolpop-0.1.0a7.tar", max compression
+gzip compressed data, was "lolpop-0.1.0a8.tar", max compression
```

## Comparing `lolpop-0.1.0a7.tar` & `lolpop-0.1.0a8.tar`

### file list

```diff
@@ -1,167 +1,167 @@
--rw-r--r--   0        0        0    11357 2023-06-14 14:38:58.404935 lolpop-0.1.0a7/LICENSE
--rw-r--r--   0        0        0      373 2023-06-14 14:38:58.404935 lolpop-0.1.0a7/lolpop/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.404935 lolpop-0.1.0a7/lolpop/cli/__init__.py
--rw-r--r--   0        0        0     2552 2023-06-14 14:38:58.404935 lolpop-0.1.0a7/lolpop/cli/cli.py
--rw-r--r--   0        0        0    12841 2023-06-14 14:38:58.404935 lolpop-0.1.0a7/lolpop/cli/create.py
--rw-r--r--   0        0        0     3464 2023-06-14 14:38:58.404935 lolpop-0.1.0a7/lolpop/cli/datagen.py
--rw-r--r--   0        0        0      432 2023-06-14 14:38:58.404935 lolpop-0.1.0a7/lolpop/cli/package.py
--rw-r--r--   0        0        0     1928 2023-06-14 14:38:58.404935 lolpop-0.1.0a7/lolpop/cli/run.py
--rw-r--r--   0        0        0     2037 2023-06-14 14:38:58.404935 lolpop-0.1.0a7/lolpop/cli/seed.py
--rw-r--r--   0        0        0      451 2023-06-14 14:38:58.404935 lolpop-0.1.0a7/lolpop/cli/test.py
--rw-r--r--   0        0        0     1311 2023-06-14 14:38:58.404935 lolpop-0.1.0a7/lolpop/component/__init__.py
--rw-r--r--   0        0        0     3752 2023-06-14 14:38:58.404935 lolpop-0.1.0a7/lolpop/component/base_component.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.404935 lolpop-0.1.0a7/lolpop/component/data_checker/__init__.py
--rw-r--r--   0        0        0      164 2023-06-14 14:38:58.404935 lolpop-0.1.0a7/lolpop/component/data_checker/base_data_checker.py
--rw-r--r--   0        0        0     2356 2023-06-14 14:38:58.404935 lolpop-0.1.0a7/lolpop/component/data_checker/deepchecks_data_checker.py
--rw-r--r--   0        0        0     1813 2023-06-14 14:38:58.404935 lolpop-0.1.0a7/lolpop/component/data_checker/evidentlyai_data_checker.py
--rw-r--r--   0        0        0     2650 2023-06-14 14:38:58.404935 lolpop-0.1.0a7/lolpop/component/data_checker/stumpy_matrix_profiler.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.404935 lolpop-0.1.0a7/lolpop/component/data_connector/__init__.py
--rw-r--r--   0        0        0      233 2023-06-14 14:38:58.404935 lolpop-0.1.0a7/lolpop/component/data_connector/base_data_connector.py
--rw-r--r--   0        0        0     6265 2023-06-14 14:38:58.404935 lolpop-0.1.0a7/lolpop/component/data_connector/bigquery_data_connector.py
--rw-r--r--   0        0        0     5431 2023-06-14 14:38:58.404935 lolpop-0.1.0a7/lolpop/component/data_connector/databricks_sql_data_connector.py
--rw-r--r--   0        0        0     4188 2023-06-14 14:38:58.404935 lolpop-0.1.0a7/lolpop/component/data_connector/duckdb_data_connector.py
--rw-r--r--   0        0        0     4275 2023-06-14 14:38:58.404935 lolpop-0.1.0a7/lolpop/component/data_connector/gcs_data_connector.py
--rw-r--r--   0        0        0     1299 2023-06-14 14:38:58.404935 lolpop-0.1.0a7/lolpop/component/data_connector/local_data_connector.py
--rw-r--r--   0        0        0     5453 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_connector/postgres_data_connector.py
--rw-r--r--   0        0        0      637 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_connector/redshift_data_connector.py
--rw-r--r--   0        0        0     3352 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_connector/s3_data_connector.py
--rw-r--r--   0        0        0     6484 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_connector/snowflake_data_connector.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_profiler/__init__.py
--rw-r--r--   0        0        0      243 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_profiler/base_data_profiler.py
--rw-r--r--   0        0        0     1462 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_profiler/continual_data_profiler.py
--rw-r--r--   0        0        0     2314 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_profiler/evidentlyai_data_profiler.py
--rw-r--r--   0        0        0     2162 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_profiler/sweetviz_data_profiler.py
--rw-r--r--   0        0        0     1087 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_profiler/tslumen_data_profiler.py
--rw-r--r--   0        0        0     2164 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_profiler/ydata_profiling_data_profiler.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_splitter/__init__.py
--rw-r--r--   0        0        0      163 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_splitter/base_data_splitter.py
--rw-r--r--   0        0        0     9807 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_splitter/local_data_splitter.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_synthesizer/__init__.py
--rw-r--r--   0        0        0      396 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_synthesizer/base_data_synthesizer.py
--rw-r--r--   0        0        0     5878 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_synthesizer/svd_data_synthesizer.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_transformer/__init__.py
--rw-r--r--   0        0        0      301 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_transformer/base_data_transformer.py
--rw-r--r--   0        0        0      712 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_transformer/bigquery_data_transformer.py
--rw-r--r--   0        0        0      870 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_transformer/databricks_sql_data_transformer.py
--rw-r--r--   0        0        0     4525 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_transformer/dbt_data_transformer.py
--rw-r--r--   0        0        0      613 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_transformer/duckdb_data_transformer.py
--rw-r--r--   0        0        0     2484 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_transformer/local_data_transformer.py
--rw-r--r--   0        0        0      838 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_transformer/postrgres_data_transformer.py
--rw-r--r--   0        0        0      962 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_transformer/redshift_data_transformer.py
--rw-r--r--   0        0        0      855 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/data_transformer/snowflake_data_transformer.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/genai_chatbot/__init__.py
--rw-r--r--   0        0        0      228 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/genai_chatbot/base_genai_chatbot.py
--rw-r--r--   0        0        0      940 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/genai_chatbot/openai_chatbot.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/hyperparameter_tuner/__init__.py
--rw-r--r--   0        0        0     2705 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/hyperparameter_tuner/base_hyperparameter_tuner.py
--rw-r--r--   0        0        0     2755 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/hyperparameter_tuner/local_hyperparameter_tuner.py
--rw-r--r--   0        0        0     9416 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/hyperparameter_tuner/optuna_hyperparameter_tuner.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/logger/__init__.py
--rw-r--r--   0        0        0      139 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/logger/base_logger.py
--rw-r--r--   0        0        0     1699 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/logger/file_logger.py
--rw-r--r--   0        0        0     2017 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/logger/stdout_logger.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/metadata_tracker/__init__.py
--rw-r--r--   0        0        0     2073 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/metadata_tracker/base_metadata_tracker.py
--rw-r--r--   0        0        0    15598 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/metadata_tracker/continual_metadata_tracker.py
--rw-r--r--   0        0        0    12571 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/metadata_tracker/mlflow_metadata_tracker.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/metrics_tracker/__init__.py
--rw-r--r--   0        0        0      460 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/metrics_tracker/base_metrics_tracker.py
--rw-r--r--   0        0        0     5843 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/metrics_tracker/continual_metrics_tracker.py
--rw-r--r--   0        0        0     4804 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/metrics_tracker/mlflow_metrics_tracker.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/model_bias_checker/__init__.py
--rw-r--r--   0        0        0     4876 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/model_bias_checker/aifairness_model_bias_checker.py
--rw-r--r--   0        0        0      240 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/model_bias_checker/base_model_bias_checker.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/model_checker/__init__.py
--rw-r--r--   0        0        0    11210 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/model_checker/base_model_checker.py
--rw-r--r--   0        0        0     2846 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/model_checker/deepchecks_model_checker.py
--rw-r--r--   0        0        0     3601 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/model_checker/evidentlyai_model_checker.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/model_deployer/__init__.py
--rw-r--r--   0        0        0      371 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/model_deployer/base_model_deployer.py
--rw-r--r--   0        0        0      574 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/model_deployer/seldon_model_deployer.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/model_explainer/__init__.py
--rw-r--r--   0        0        0    10342 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/model_explainer/alibi_model_explainer.py
--rw-r--r--   0        0        0      244 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/model_explainer/base_model_explainer.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/model_repository/__init__.py
--rw-r--r--   0        0        0      309 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/model_repository/base_model_repository.py
--rw-r--r--   0        0        0     2993 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/model_repository/continual_model_repository.py
--rw-r--r--   0        0        0     4521 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/model_repository/mlflow_model_repository.py
--rw-r--r--   0        0        0     5064 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/model_trainer/ProphetModelTrainer.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/model_trainer/__init__.py
--rw-r--r--   0        0        0    12320 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/model_trainer/base_model_trainer.py
--rw-r--r--   0        0        0     2404 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/model_trainer/xgboost_model_trainer.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/model_visualizer/__init__.py
--rw-r--r--   0        0        0      169 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/model_visualizer/base_model_visualizer.py
--rw-r--r--   0        0        0     2504 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/model_visualizer/prophet_visualizer.py
--rw-r--r--   0        0        0     5102 2023-06-14 14:38:58.408935 lolpop-0.1.0a7/lolpop/component/model_visualizer/yellowbrick_model_visualizer.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/component/notifier/__init__.py
--rw-r--r--   0        0        0      156 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/component/notifier/base_notifier.py
--rw-r--r--   0        0        0     2904 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/component/notifier/gmail_notifier.py
--rw-r--r--   0        0        0      880 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/component/notifier/slack_notifier.py
--rw-r--r--   0        0        0     1272 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/component/notifier/smtp_notifier.py
--rw-r--r--   0        0        0      322 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/component/notifier/stdout_notifier.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/component/resource_version_control/__init__.py
--rw-r--r--   0        0        0      376 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/component/resource_version_control/base_resource_version_control.py
--rw-r--r--   0        0        0     3221 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/component/resource_version_control/continual_version_control.py
--rw-r--r--   0        0        0     5828 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/component/resource_version_control/dvc_version_control.py
--rw-r--r--   0        0        0     2661 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/extension/__init__.py
--rw-r--r--   0        0        0     1299 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/pipeline/__init__.py
--rw-r--r--   0        0        0     4971 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/pipeline/base_pipeline.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/pipeline/deploy/__init__.py
--rw-r--r--   0        0        0      454 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/pipeline/deploy/base_deploy.py
--rw-r--r--   0        0        0     3849 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/pipeline/deploy/metaflow_offline_deploy.py
--rw-r--r--   0        0        0     1660 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/pipeline/deploy/offline_deploy.py
--rw-r--r--   0        0        0       42 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/pipeline/predict/__init__.py
--rw-r--r--   0        0        0      227 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/pipeline/predict/base_predict.py
--rw-r--r--   0        0        0     7180 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/pipeline/predict/metaflow_offline_predict.py
--rw-r--r--   0        0        0     4172 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/pipeline/predict/offline_predict.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/pipeline/process/__init__.py
--rw-r--r--   0        0        0      452 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/pipeline/process/base_process.py
--rw-r--r--   0        0        0     5660 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/pipeline/process/metaflow_offline_process.py
--rw-r--r--   0        0        0     3267 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/pipeline/process/offline_process.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/pipeline/train/__init__.py
--rw-r--r--   0        0        0      645 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/pipeline/train/base_train.py
--rw-r--r--   0        0        0     7331 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/pipeline/train/metaflow_offline_train.py
--rw-r--r--   0        0        0     4499 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/pipeline/train/offline_train.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/pipeline/wrapper/__init__.py
--rw-r--r--   0        0        0      275 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/pipeline/wrapper/base_wrapper.py
--rw-r--r--   0        0        0      793 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/pipeline/wrapper/metaflow_pipeline_wrapper.py
--rw-r--r--   0        0        0     1285 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/runner/__init__.py
--rw-r--r--   0        0        0     7106 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/runner/base_runner.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/runner/classification_runner/__init__.py
--rw-r--r--   0        0        0     7732 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/runner/classification_runner/classification_runner.py
--rw-r--r--   0        0        0     6194 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/runner/classification_runner/metaflow_classification.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/runner/regression_runner/__init__.py
--rw-r--r--   0        0        0      397 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/runner/regression_runner/regression_runner.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/runner/timeseries_runner/__init__.py
--rw-r--r--   0        0        0     8862 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/runner/timeseries_runner/timeseries_runner.py
--rw-r--r--   0        0        0      175 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/templates/component_template/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/templates/component_template/{{cookiecutter.component_type}}/__init__.py
--rw-r--r--   0        0        0      802 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/templates/component_template/{{cookiecutter.component_type}}/base_{{cookiecutter.component_type}}.py
--rw-r--r--   0        0        0     1122 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/templates/component_template/{{cookiecutter.component_type}}/{{cookiecutter.component_class}}.py
--rw-r--r--   0        0        0      167 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/templates/pipeline_template/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/__init__.py
--rw-r--r--   0        0        0      803 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/base_{{cookiecutter.pipeline_type}}.py
--rw-r--r--   0        0        0     1096 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/{{cookiecutter.pipeline_class}}.py
--rw-r--r--   0        0        0       66 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/templates/project_template/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/templates/project_template/{{cookiecutter.project_name}}/Makefile
--rw-r--r--   0        0        0       32 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/templates/project_template/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/templates/project_template/{{cookiecutter.project_name}}/dvc.yaml
--rw-r--r--   0        0        0      152 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/__int__.py
--rw-r--r--   0        0        0      152 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/component/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/pipeline/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/runner/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop_project.yaml
--rw-r--r--   0        0        0      310 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/templates/project_template/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0      151 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/templates/runner_template/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/__init__.py
--rw-r--r--   0        0        0      795 2023-06-14 14:38:58.412935 lolpop-0.1.0a7/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/base_{{cookiecutter.runner_type}}.py
--rw-r--r--   0        0        0     1054 2023-06-14 14:38:58.416935 lolpop-0.1.0a7/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/{{cookiecutter.runner_class}}.py
--rw-r--r--   0        0        0        0 2023-06-14 14:38:58.416935 lolpop-0.1.0a7/lolpop/utils/__init__.py
--rw-r--r--   0        0        0    15753 2023-06-14 14:38:58.416935 lolpop-0.1.0a7/lolpop/utils/common_utils.py
--rw-r--r--   0        0        0     1566 2023-06-14 14:38:58.416935 lolpop-0.1.0a7/lolpop/utils/continual_utils.py
--rw-r--r--   0        0        0     2452 2023-06-14 14:38:58.416935 lolpop-0.1.0a7/lolpop/utils/metaflow_utils.py
--rw-r--r--   0        0        0     3298 2023-06-14 14:38:58.416935 lolpop-0.1.0a7/lolpop/utils/mlflow_utils.py
--rw-r--r--   0        0        0     2433 2023-06-14 14:39:15.992845 lolpop-0.1.0a7/pyproject.toml
--rw-r--r--   0        0        0     2914 1970-01-01 00:00:00.000000 lolpop-0.1.0a7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-15 03:53:18.075554 lolpop-0.1.0a8/LICENSE
+-rw-r--r--   0        0        0      373 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/cli/__init__.py
+-rw-r--r--   0        0        0     2552 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/cli/cli.py
+-rw-r--r--   0        0        0    12841 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/cli/create.py
+-rw-r--r--   0        0        0     3464 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/cli/datagen.py
+-rw-r--r--   0        0        0      432 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/cli/package.py
+-rw-r--r--   0        0        0     1928 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/cli/run.py
+-rw-r--r--   0        0        0     2037 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/cli/seed.py
+-rw-r--r--   0        0        0      451 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/cli/test.py
+-rw-r--r--   0        0        0     1454 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/__init__.py
+-rw-r--r--   0        0        0     3752 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/base_component.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_checker/__init__.py
+-rw-r--r--   0        0        0      164 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_checker/base_data_checker.py
+-rw-r--r--   0        0        0     2356 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_checker/deepchecks_data_checker.py
+-rw-r--r--   0        0        0     1813 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_checker/evidentlyai_data_checker.py
+-rw-r--r--   0        0        0     2650 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_checker/stumpy_matrix_profiler.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_connector/__init__.py
+-rw-r--r--   0        0        0      233 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_connector/base_data_connector.py
+-rw-r--r--   0        0        0     6265 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_connector/bigquery_data_connector.py
+-rw-r--r--   0        0        0     5431 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_connector/databricks_sql_data_connector.py
+-rw-r--r--   0        0        0     4188 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_connector/duckdb_data_connector.py
+-rw-r--r--   0        0        0     4275 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_connector/gcs_data_connector.py
+-rw-r--r--   0        0        0     1299 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_connector/local_data_connector.py
+-rw-r--r--   0        0        0     5453 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_connector/postgres_data_connector.py
+-rw-r--r--   0        0        0      637 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_connector/redshift_data_connector.py
+-rw-r--r--   0        0        0     3352 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_connector/s3_data_connector.py
+-rw-r--r--   0        0        0     6484 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_connector/snowflake_data_connector.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_profiler/__init__.py
+-rw-r--r--   0        0        0      243 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_profiler/base_data_profiler.py
+-rw-r--r--   0        0        0     1462 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_profiler/continual_data_profiler.py
+-rw-r--r--   0        0        0     2314 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_profiler/evidentlyai_data_profiler.py
+-rw-r--r--   0        0        0     2162 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_profiler/sweetviz_data_profiler.py
+-rw-r--r--   0        0        0     1087 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_profiler/tslumen_data_profiler.py
+-rw-r--r--   0        0        0     2164 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_profiler/ydata_profiling_data_profiler.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_splitter/__init__.py
+-rw-r--r--   0        0        0      163 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_splitter/base_data_splitter.py
+-rw-r--r--   0        0        0     9807 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_splitter/local_data_splitter.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_synthesizer/__init__.py
+-rw-r--r--   0        0        0      396 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_synthesizer/base_data_synthesizer.py
+-rw-r--r--   0        0        0     5878 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_synthesizer/svd_data_synthesizer.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_transformer/__init__.py
+-rw-r--r--   0        0        0      301 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_transformer/base_data_transformer.py
+-rw-r--r--   0        0        0      712 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_transformer/bigquery_data_transformer.py
+-rw-r--r--   0        0        0      870 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_transformer/databricks_sql_data_transformer.py
+-rw-r--r--   0        0        0     4525 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_transformer/dbt_data_transformer.py
+-rw-r--r--   0        0        0      613 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_transformer/duckdb_data_transformer.py
+-rw-r--r--   0        0        0     2484 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_transformer/local_data_transformer.py
+-rw-r--r--   0        0        0      838 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_transformer/postrgres_data_transformer.py
+-rw-r--r--   0        0        0      962 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_transformer/redshift_data_transformer.py
+-rw-r--r--   0        0        0      855 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_transformer/snowflake_data_transformer.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/genai_chatbot/__init__.py
+-rw-r--r--   0        0        0      228 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/genai_chatbot/base_genai_chatbot.py
+-rw-r--r--   0        0        0      940 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/genai_chatbot/openai_chatbot.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/hyperparameter_tuner/__init__.py
+-rw-r--r--   0        0        0     2705 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/hyperparameter_tuner/base_hyperparameter_tuner.py
+-rw-r--r--   0        0        0     2755 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/hyperparameter_tuner/local_hyperparameter_tuner.py
+-rw-r--r--   0        0        0     9416 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/hyperparameter_tuner/optuna_hyperparameter_tuner.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/logger/__init__.py
+-rw-r--r--   0        0        0      139 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/logger/base_logger.py
+-rw-r--r--   0        0        0     1699 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/logger/file_logger.py
+-rw-r--r--   0        0        0     2017 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/logger/stdout_logger.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/metadata_tracker/__init__.py
+-rw-r--r--   0        0        0     2073 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/metadata_tracker/base_metadata_tracker.py
+-rw-r--r--   0        0        0    15598 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/metadata_tracker/continual_metadata_tracker.py
+-rw-r--r--   0        0        0    12571 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/metadata_tracker/mlflow_metadata_tracker.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/metrics_tracker/__init__.py
+-rw-r--r--   0        0        0      460 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/metrics_tracker/base_metrics_tracker.py
+-rw-r--r--   0        0        0     5843 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/metrics_tracker/continual_metrics_tracker.py
+-rw-r--r--   0        0        0     4804 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/metrics_tracker/mlflow_metrics_tracker.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_bias_checker/__init__.py
+-rw-r--r--   0        0        0     4876 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_bias_checker/aifairness_model_bias_checker.py
+-rw-r--r--   0        0        0      240 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_bias_checker/base_model_bias_checker.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_checker/__init__.py
+-rw-r--r--   0        0        0    11210 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_checker/base_model_checker.py
+-rw-r--r--   0        0        0     2846 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_checker/deepchecks_model_checker.py
+-rw-r--r--   0        0        0     3601 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_checker/evidentlyai_model_checker.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_deployer/__init__.py
+-rw-r--r--   0        0        0      371 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_deployer/base_model_deployer.py
+-rw-r--r--   0        0        0      574 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_deployer/seldon_model_deployer.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_explainer/__init__.py
+-rw-r--r--   0        0        0    10342 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_explainer/alibi_model_explainer.py
+-rw-r--r--   0        0        0      244 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_explainer/base_model_explainer.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_repository/__init__.py
+-rw-r--r--   0        0        0      309 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_repository/base_model_repository.py
+-rw-r--r--   0        0        0     2993 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_repository/continual_model_repository.py
+-rw-r--r--   0        0        0     4521 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_repository/mlflow_model_repository.py
+-rw-r--r--   0        0        0     5064 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_trainer/ProphetModelTrainer.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_trainer/__init__.py
+-rw-r--r--   0        0        0    12320 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_trainer/base_model_trainer.py
+-rw-r--r--   0        0        0     2404 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_trainer/xgboost_model_trainer.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_visualizer/__init__.py
+-rw-r--r--   0        0        0      169 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_visualizer/base_model_visualizer.py
+-rw-r--r--   0        0        0     2504 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_visualizer/prophet_visualizer.py
+-rw-r--r--   0        0        0     5102 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_visualizer/yellowbrick_model_visualizer.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/notifier/__init__.py
+-rw-r--r--   0        0        0      156 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/notifier/base_notifier.py
+-rw-r--r--   0        0        0     2904 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/notifier/gmail_notifier.py
+-rw-r--r--   0        0        0      880 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/notifier/slack_notifier.py
+-rw-r--r--   0        0        0     1272 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/notifier/smtp_notifier.py
+-rw-r--r--   0        0        0      322 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/notifier/stdout_notifier.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/resource_version_control/__init__.py
+-rw-r--r--   0        0        0      376 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/resource_version_control/base_resource_version_control.py
+-rw-r--r--   0        0        0     3221 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/resource_version_control/continual_version_control.py
+-rw-r--r--   0        0        0     5828 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/resource_version_control/dvc_version_control.py
+-rw-r--r--   0        0        0     2802 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/extension/__init__.py
+-rw-r--r--   0        0        0     1376 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/__init__.py
+-rw-r--r--   0        0        0     4971 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/base_pipeline.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/deploy/__init__.py
+-rw-r--r--   0        0        0      454 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/deploy/base_deploy.py
+-rw-r--r--   0        0        0     3849 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/deploy/metaflow_offline_deploy.py
+-rw-r--r--   0        0        0     1660 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/deploy/offline_deploy.py
+-rw-r--r--   0        0        0       42 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/predict/__init__.py
+-rw-r--r--   0        0        0      227 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/predict/base_predict.py
+-rw-r--r--   0        0        0     7180 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/predict/metaflow_offline_predict.py
+-rw-r--r--   0        0        0     4172 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/predict/offline_predict.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/process/__init__.py
+-rw-r--r--   0        0        0      452 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/process/base_process.py
+-rw-r--r--   0        0        0     5660 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/process/metaflow_offline_process.py
+-rw-r--r--   0        0        0     3267 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/process/offline_process.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/train/__init__.py
+-rw-r--r--   0        0        0      645 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/train/base_train.py
+-rw-r--r--   0        0        0     7331 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/train/metaflow_offline_train.py
+-rw-r--r--   0        0        0     4499 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/train/offline_train.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/wrapper/__init__.py
+-rw-r--r--   0        0        0      275 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/wrapper/base_wrapper.py
+-rw-r--r--   0        0        0      793 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/wrapper/metaflow_pipeline_wrapper.py
+-rw-r--r--   0        0        0     1361 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/runner/__init__.py
+-rw-r--r--   0        0        0     7059 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/runner/base_runner.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/runner/classification_runner/__init__.py
+-rw-r--r--   0        0        0     7732 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/runner/classification_runner/classification_runner.py
+-rw-r--r--   0        0        0     6194 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/runner/classification_runner/metaflow_classification.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/runner/regression_runner/__init__.py
+-rw-r--r--   0        0        0      397 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/runner/regression_runner/regression_runner.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/runner/timeseries_runner/__init__.py
+-rw-r--r--   0        0        0     8862 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/runner/timeseries_runner/timeseries_runner.py
+-rw-r--r--   0        0        0      175 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/component_template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/component_template/{{cookiecutter.component_type}}/__init__.py
+-rw-r--r--   0        0        0      802 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/component_template/{{cookiecutter.component_type}}/base_{{cookiecutter.component_type}}.py
+-rw-r--r--   0        0        0     1122 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/component_template/{{cookiecutter.component_type}}/{{cookiecutter.component_class}}.py
+-rw-r--r--   0        0        0      167 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/pipeline_template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/__init__.py
+-rw-r--r--   0        0        0      803 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/base_{{cookiecutter.pipeline_type}}.py
+-rw-r--r--   0        0        0     1096 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/{{cookiecutter.pipeline_class}}.py
+-rw-r--r--   0        0        0       66 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/project_template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/project_template/{{cookiecutter.project_name}}/Makefile
+-rw-r--r--   0        0        0       32 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/project_template/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/project_template/{{cookiecutter.project_name}}/dvc.yaml
+-rw-r--r--   0        0        0      152 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/__int__.py
+-rw-r--r--   0        0        0      152 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/component/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/pipeline/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/runner/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop_project.yaml
+-rw-r--r--   0        0        0      310 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/project_template/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      151 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/runner_template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/__init__.py
+-rw-r--r--   0        0        0      795 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/base_{{cookiecutter.runner_type}}.py
+-rw-r--r--   0        0        0     1054 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/{{cookiecutter.runner_class}}.py
+-rw-r--r--   0        0        0        0 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/utils/__init__.py
+-rw-r--r--   0        0        0    15773 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/utils/common_utils.py
+-rw-r--r--   0        0        0     1566 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/utils/continual_utils.py
+-rw-r--r--   0        0        0     2452 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/utils/metaflow_utils.py
+-rw-r--r--   0        0        0     3298 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/utils/mlflow_utils.py
+-rw-r--r--   0        0        0     2433 2023-06-15 03:53:33.856530 lolpop-0.1.0a8/pyproject.toml
+-rw-r--r--   0        0        0     2914 1970-01-01 00:00:00.000000 lolpop-0.1.0a8/PKG-INFO
```

### Comparing `lolpop-0.1.0a7/LICENSE` & `lolpop-0.1.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/cli/cli.py` & `lolpop-0.1.0a8/lolpop/cli/cli.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/cli/create.py` & `lolpop-0.1.0a8/lolpop/cli/create.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/cli/datagen.py` & `lolpop-0.1.0a8/lolpop/cli/datagen.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/cli/run.py` & `lolpop-0.1.0a8/lolpop/cli/run.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/cli/seed.py` & `lolpop-0.1.0a8/lolpop/cli/seed.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/__init__.py` & `lolpop-0.1.0a8/lolpop/component/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,16 +15,19 @@
                if ((x[0] != "_") and (x[0] != ".") and (".py" not in x))]
     #for each resource type (i.e. subdir), get all resources implemented in that type (i.e. python files in the subdir)
     for subdir in subdirs: 
         files = [x for x in os.listdir(subdir) if (
             (".py" in x) and (x[0] != ".") and ("__" not in x))]
         #from each file, import all classes and register them in the global namespace. 
         for file in files:
-            module = import_module("lolpop.%s.%s.%s" %(subdir.split("/")[-2],subdir.split("/")[-1],file[:-3]))
-            classes = [x for x in dir(module) if isclass(getattr(module, x))]
-            components = [x for x in classes if issubclass(getattr(module, x), BaseComponent)]
-            globals().update({name: getattr(module,name) for name in components})
+            try: 
+                module = import_module("lolpop.%s.%s.%s" %(subdir.split("/")[-2],subdir.split("/")[-1],file[:-3]))
+                classes = [x for x in dir(module) if isclass(getattr(module, x))]
+                components = [x for x in classes if issubclass(getattr(module, x), BaseComponent)]
+                globals().update({name: getattr(module,name) for name in components})
+            except: #imports will fail for packages that are extras, we'll ignore them
+                pass 
 
     warnings.resetwarnings()
 
 
 __map_components__()
```

### Comparing `lolpop-0.1.0a7/lolpop/component/base_component.py` & `lolpop-0.1.0a8/lolpop/component/base_component.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_checker/deepchecks_data_checker.py` & `lolpop-0.1.0a8/lolpop/component/data_checker/deepchecks_data_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_checker/evidentlyai_data_checker.py` & `lolpop-0.1.0a8/lolpop/component/data_checker/evidentlyai_data_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_checker/stumpy_matrix_profiler.py` & `lolpop-0.1.0a8/lolpop/component/data_checker/stumpy_matrix_profiler.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_connector/bigquery_data_connector.py` & `lolpop-0.1.0a8/lolpop/component/data_connector/bigquery_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_connector/databricks_sql_data_connector.py` & `lolpop-0.1.0a8/lolpop/component/data_connector/databricks_sql_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_connector/duckdb_data_connector.py` & `lolpop-0.1.0a8/lolpop/component/data_connector/duckdb_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_connector/gcs_data_connector.py` & `lolpop-0.1.0a8/lolpop/component/data_connector/gcs_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_connector/local_data_connector.py` & `lolpop-0.1.0a8/lolpop/component/data_connector/local_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_connector/postgres_data_connector.py` & `lolpop-0.1.0a8/lolpop/component/data_connector/postgres_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_connector/redshift_data_connector.py` & `lolpop-0.1.0a8/lolpop/component/data_connector/redshift_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_connector/s3_data_connector.py` & `lolpop-0.1.0a8/lolpop/component/data_connector/s3_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_connector/snowflake_data_connector.py` & `lolpop-0.1.0a8/lolpop/component/data_connector/snowflake_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_profiler/continual_data_profiler.py` & `lolpop-0.1.0a8/lolpop/component/data_profiler/continual_data_profiler.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_profiler/evidentlyai_data_profiler.py` & `lolpop-0.1.0a8/lolpop/component/data_profiler/evidentlyai_data_profiler.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_profiler/sweetviz_data_profiler.py` & `lolpop-0.1.0a8/lolpop/component/data_profiler/sweetviz_data_profiler.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_profiler/tslumen_data_profiler.py` & `lolpop-0.1.0a8/lolpop/component/data_profiler/tslumen_data_profiler.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_profiler/ydata_profiling_data_profiler.py` & `lolpop-0.1.0a8/lolpop/component/data_profiler/ydata_profiling_data_profiler.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_splitter/local_data_splitter.py` & `lolpop-0.1.0a8/lolpop/component/data_splitter/local_data_splitter.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_synthesizer/svd_data_synthesizer.py` & `lolpop-0.1.0a8/lolpop/component/data_synthesizer/svd_data_synthesizer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_transformer/bigquery_data_transformer.py` & `lolpop-0.1.0a8/lolpop/component/data_transformer/bigquery_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_transformer/databricks_sql_data_transformer.py` & `lolpop-0.1.0a8/lolpop/component/data_transformer/databricks_sql_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_transformer/dbt_data_transformer.py` & `lolpop-0.1.0a8/lolpop/component/data_transformer/dbt_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_transformer/duckdb_data_transformer.py` & `lolpop-0.1.0a8/lolpop/component/data_transformer/duckdb_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_transformer/local_data_transformer.py` & `lolpop-0.1.0a8/lolpop/component/data_transformer/local_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_transformer/postrgres_data_transformer.py` & `lolpop-0.1.0a8/lolpop/component/data_transformer/postrgres_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_transformer/redshift_data_transformer.py` & `lolpop-0.1.0a8/lolpop/component/data_transformer/redshift_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/data_transformer/snowflake_data_transformer.py` & `lolpop-0.1.0a8/lolpop/component/data_transformer/snowflake_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/genai_chatbot/openai_chatbot.py` & `lolpop-0.1.0a8/lolpop/component/genai_chatbot/openai_chatbot.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/hyperparameter_tuner/base_hyperparameter_tuner.py` & `lolpop-0.1.0a8/lolpop/component/hyperparameter_tuner/base_hyperparameter_tuner.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/hyperparameter_tuner/local_hyperparameter_tuner.py` & `lolpop-0.1.0a8/lolpop/component/hyperparameter_tuner/local_hyperparameter_tuner.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/hyperparameter_tuner/optuna_hyperparameter_tuner.py` & `lolpop-0.1.0a8/lolpop/component/hyperparameter_tuner/optuna_hyperparameter_tuner.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/logger/file_logger.py` & `lolpop-0.1.0a8/lolpop/component/logger/file_logger.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/logger/stdout_logger.py` & `lolpop-0.1.0a8/lolpop/component/logger/stdout_logger.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/metadata_tracker/base_metadata_tracker.py` & `lolpop-0.1.0a8/lolpop/component/metadata_tracker/base_metadata_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/metadata_tracker/continual_metadata_tracker.py` & `lolpop-0.1.0a8/lolpop/component/metadata_tracker/continual_metadata_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/metadata_tracker/mlflow_metadata_tracker.py` & `lolpop-0.1.0a8/lolpop/component/metadata_tracker/mlflow_metadata_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/metrics_tracker/continual_metrics_tracker.py` & `lolpop-0.1.0a8/lolpop/component/metrics_tracker/continual_metrics_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/metrics_tracker/mlflow_metrics_tracker.py` & `lolpop-0.1.0a8/lolpop/component/metrics_tracker/mlflow_metrics_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/model_bias_checker/aifairness_model_bias_checker.py` & `lolpop-0.1.0a8/lolpop/component/model_bias_checker/aifairness_model_bias_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/model_checker/base_model_checker.py` & `lolpop-0.1.0a8/lolpop/component/model_checker/base_model_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/model_checker/deepchecks_model_checker.py` & `lolpop-0.1.0a8/lolpop/component/model_checker/deepchecks_model_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/model_checker/evidentlyai_model_checker.py` & `lolpop-0.1.0a8/lolpop/component/model_checker/evidentlyai_model_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/model_deployer/seldon_model_deployer.py` & `lolpop-0.1.0a8/lolpop/component/model_deployer/seldon_model_deployer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/model_explainer/alibi_model_explainer.py` & `lolpop-0.1.0a8/lolpop/component/model_explainer/alibi_model_explainer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/model_repository/continual_model_repository.py` & `lolpop-0.1.0a8/lolpop/component/model_repository/continual_model_repository.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/model_repository/mlflow_model_repository.py` & `lolpop-0.1.0a8/lolpop/component/model_repository/mlflow_model_repository.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/model_trainer/ProphetModelTrainer.py` & `lolpop-0.1.0a8/lolpop/component/model_trainer/ProphetModelTrainer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/model_trainer/base_model_trainer.py` & `lolpop-0.1.0a8/lolpop/component/model_trainer/base_model_trainer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/model_trainer/xgboost_model_trainer.py` & `lolpop-0.1.0a8/lolpop/component/model_trainer/xgboost_model_trainer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/model_visualizer/prophet_visualizer.py` & `lolpop-0.1.0a8/lolpop/component/model_visualizer/prophet_visualizer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/model_visualizer/yellowbrick_model_visualizer.py` & `lolpop-0.1.0a8/lolpop/component/model_visualizer/yellowbrick_model_visualizer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/notifier/gmail_notifier.py` & `lolpop-0.1.0a8/lolpop/component/notifier/gmail_notifier.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/notifier/slack_notifier.py` & `lolpop-0.1.0a8/lolpop/component/notifier/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/notifier/smtp_notifier.py` & `lolpop-0.1.0a8/lolpop/component/notifier/smtp_notifier.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/resource_version_control/continual_version_control.py` & `lolpop-0.1.0a8/lolpop/component/resource_version_control/continual_version_control.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/component/resource_version_control/dvc_version_control.py` & `lolpop-0.1.0a8/lolpop/component/resource_version_control/dvc_version_control.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/extension/__init__.py` & `lolpop-0.1.0a8/lolpop/extension/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,23 +29,26 @@
                         if ((x[0] != "_") and (x[0] != ".") and (".py" not in x))]
                 #for each resource type (i.e. subdir), get all resources implemented in that type (i.e. python files in the subdir)
                 for subdir in subdirs:
                     files = [x for x in os.listdir(subdir) if (
                         (".py" in x) and ("__" not in x) and (x[0] != "."))]
                     #from each file, import all classes and register them in the global namespace.
                     for file in files:
-                        subdir_arr = subdir.split("/")
-                        module = import_module("lolpop.extension.%s.%s.%s.%s" % (
-                            subdir_arr[-3], subdir_arr[-2], subdir_arr[-1], file[:-3]))
-                        classes = [x for x in dir(module) if isclass(getattr(module, x))]
-                        components = [x for x in classes if (
-                            issubclass(getattr(module, x), BaseComponent)
-                            or issubclass(getattr(module, x), BasePipeline)
-                            or issubclass(getattr(module, x), BaseRunner)
-                            )]
-                        globals().update({name: getattr(module, name)
-                                        for name in components})
+                        try: 
+                            subdir_arr = subdir.split("/")
+                            module = import_module("lolpop.extension.%s.%s.%s.%s" % (
+                                subdir_arr[-3], subdir_arr[-2], subdir_arr[-1], file[:-3]))
+                            classes = [x for x in dir(module) if isclass(getattr(module, x))]
+                            components = [x for x in classes if (
+                                issubclass(getattr(module, x), BaseComponent)
+                                or issubclass(getattr(module, x), BasePipeline)
+                                or issubclass(getattr(module, x), BaseRunner)
+                                )]
+                            globals().update({name: getattr(module, name)
+                                            for name in components})
+                        except: 
+                            pass 
 
     warnings.resetwarnings()
 
 
 __map_extensions__()
```

### Comparing `lolpop-0.1.0a7/lolpop/pipeline/__init__.py` & `lolpop-0.1.0a8/lolpop/pipeline/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,18 @@
                if ((x[0] != "_") and (x[0] != ".") and (".py" not in x))]
     #for each resource type (i.e. subdir), get all resources implemented in that type (i.e. python files in the subdir)
     for subdir in subdirs: 
         files = [x for x in os.listdir(subdir) if (
             (".py" in x) and (x[0] != ".") and ("__" not in x))]
         #from each file, import all classes and register them in the global namespace. 
         for file in files: 
-            module = import_module("lolpop.%s.%s.%s" %(subdir.split("/")[-2],subdir.split("/")[-1],file[:-3]))
-            classes = [x for x in dir(module) if isclass(getattr(module,x))]
-            pipelines = [x for x in classes if issubclass(getattr(module, x), BasePipeline)]
-            globals().update({name: getattr(module,name) for name in pipelines})
+            try: 
+                module = import_module("lolpop.%s.%s.%s" %(subdir.split("/")[-2],subdir.split("/")[-1],file[:-3]))
+                classes = [x for x in dir(module) if isclass(getattr(module,x))]
+                pipelines = [x for x in classes if issubclass(getattr(module, x), BasePipeline)]
+                globals().update({name: getattr(module,name) for name in pipelines})
+            except: 
+                pass 
 
     warnings.resetwarnings()
 
 __map_pipelines__()
```

### Comparing `lolpop-0.1.0a7/lolpop/pipeline/base_pipeline.py` & `lolpop-0.1.0a8/lolpop/pipeline/base_pipeline.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/pipeline/deploy/metaflow_offline_deploy.py` & `lolpop-0.1.0a8/lolpop/pipeline/deploy/metaflow_offline_deploy.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/pipeline/deploy/offline_deploy.py` & `lolpop-0.1.0a8/lolpop/pipeline/deploy/offline_deploy.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/pipeline/predict/metaflow_offline_predict.py` & `lolpop-0.1.0a8/lolpop/pipeline/predict/metaflow_offline_predict.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/pipeline/predict/offline_predict.py` & `lolpop-0.1.0a8/lolpop/pipeline/predict/offline_predict.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/pipeline/process/metaflow_offline_process.py` & `lolpop-0.1.0a8/lolpop/pipeline/process/metaflow_offline_process.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/pipeline/process/offline_process.py` & `lolpop-0.1.0a8/lolpop/pipeline/process/offline_process.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/pipeline/train/base_train.py` & `lolpop-0.1.0a8/lolpop/pipeline/train/base_train.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/pipeline/train/metaflow_offline_train.py` & `lolpop-0.1.0a8/lolpop/pipeline/train/metaflow_offline_train.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/pipeline/train/offline_train.py` & `lolpop-0.1.0a8/lolpop/pipeline/train/offline_train.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/pipeline/wrapper/metaflow_pipeline_wrapper.py` & `lolpop-0.1.0a8/lolpop/pipeline/wrapper/metaflow_pipeline_wrapper.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/runner/__init__.py` & `lolpop-0.1.0a8/lolpop/runner/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,18 @@
                if ((x[0] != "_") and (x[0] != ".") and (".py" not in x))]
     #for each resource type (i.e. subdir), get all resources implemented in that type (i.e. python files in the subdir)
     for subdir in subdirs: 
         files = [x for x in os.listdir(subdir) if (
             (".py" in x) and (x[0] != ".")  and ("__" not in x))]
         #from each file, import all classes and register them in the global namespace. 
         for file in files: 
-            module = import_module("lolpop.%s.%s.%s" %(subdir.split("/")[-2],subdir.split("/")[-1],file[:-3]))
-            classes = [x for x in dir(module) if isclass(getattr(module,x))]
-            runners = [x for x in classes if issubclass(getattr(module, x), BaseRunner)]
-            globals().update({name: getattr(module,name) for name in runners})
+            try: 
+                module = import_module("lolpop.%s.%s.%s" %(subdir.split("/")[-2],subdir.split("/")[-1],file[:-3]))
+                classes = [x for x in dir(module) if isclass(getattr(module,x))]
+                runners = [x for x in classes if issubclass(getattr(module, x), BaseRunner)]
+                globals().update({name: getattr(module,name) for name in runners})
+            except: 
+                pass
 
     warnings.resetwarnings()
 
 __map_runners__()
```

### Comparing `lolpop-0.1.0a7/lolpop/runner/base_runner.py` & `lolpop-0.1.0a8/lolpop/runner/base_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-from omegaconf import OmegaConf
 from lolpop.utils import common_utils as utils
-import os 
-from pathlib import Path
 from inspect import currentframe
+
 class BaseRunner: 
 
     __REQUIRED_CONF__ = {
         "pipelines": [], 
         "components": ["metadata_tracker"], 
         "config": []
     }
@@ -77,15 +75,15 @@
             runner_components["metadata_tracker"] = meta_obj
             self.log("Loaded class %s into component %s" %(type(self.metadata_tracker).__name__, "metadata_tracker"))
         else: 
             #for local dev you may turn off metadata_tracker, so let's not strictly enforce that it exists for now
             self.log("Unable to load metadata_tracker component.")
 
         #build all other components
-        for component in conf.components.keys(): 
+        for component in conf.get("components",{}).keys(): 
             #ignore logger and metadata_tracker since we have already set those up
             if component != "logger" and component !="metadata_tracker": 
                 obj = utils.register_component_class(self, conf, component, runner_conf=self.config, parent_process=self.name,
                                                      problem_type=self.problem_type, dependent_components=runner_components, 
                                                      plugin_mods=plugin_mods, skip_config_validation=skip_config_validation)
                 if obj is not None: 
                     self.log("Loaded class %s into component %s" %(type(getattr(self, component)).__name__, component))
@@ -95,15 +93,15 @@
 
         #now that all component classes are built, we want to update all components so that they know about each other. 
         # there is probably a more elegant way to do this
         for obj in runner_components.values(): 
             obj._update_components(components = runner_components)
 
         #build all pipelines 
-        for pipeline in conf.pipelines.keys(): 
+        for pipeline in conf.get("pipelines",{}).keys(): 
             utils.register_pipeline_class(self, conf, pipeline, runner_conf=self.config, parent_process=self.name,
                                           problem_type=self.problem_type, dependent_components=runner_components, 
                                           plugin_mods=plugin_mods, skip_config_validation=skip_config_validation)
             self.log("Loaded class %s into pipeline %s" %(type(getattr(self, pipeline)).__name__, pipeline))
 
     def _validate_conf(self, conf):
         missing, total_missing = utils.validate_conf(conf, self.__REQUIRED_CONF__, conf.get("components"))
```

### Comparing `lolpop-0.1.0a7/lolpop/runner/classification_runner/classification_runner.py` & `lolpop-0.1.0a8/lolpop/runner/classification_runner/classification_runner.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/runner/classification_runner/metaflow_classification.py` & `lolpop-0.1.0a8/lolpop/runner/classification_runner/metaflow_classification.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/runner/timeseries_runner/timeseries_runner.py` & `lolpop-0.1.0a8/lolpop/runner/timeseries_runner/timeseries_runner.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/templates/component_template/{{cookiecutter.component_type}}/base_{{cookiecutter.component_type}}.py` & `lolpop-0.1.0a8/lolpop/templates/component_template/{{cookiecutter.component_type}}/base_{{cookiecutter.component_type}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/templates/component_template/{{cookiecutter.component_type}}/{{cookiecutter.component_class}}.py` & `lolpop-0.1.0a8/lolpop/templates/component_template/{{cookiecutter.component_type}}/{{cookiecutter.component_class}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/base_{{cookiecutter.pipeline_type}}.py` & `lolpop-0.1.0a8/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/base_{{cookiecutter.pipeline_type}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/{{cookiecutter.pipeline_class}}.py` & `lolpop-0.1.0a8/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/{{cookiecutter.pipeline_class}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/base_{{cookiecutter.runner_type}}.py` & `lolpop-0.1.0a8/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/base_{{cookiecutter.runner_type}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/{{cookiecutter.runner_class}}.py` & `lolpop-0.1.0a8/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/{{cookiecutter.runner_class}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/utils/common_utils.py` & `lolpop-0.1.0a8/lolpop/utils/common_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,29 +127,29 @@
     return mod 
 
 #register component class as an attribute of the provided object
 def register_component_class(self_obj, conf, component_type, default_class_name=None, 
                              pipeline_conf = {}, runner_conf = {}, parent_process = "runner", 
                              problem_type = None, dependent_components = {}, plugin_mods=[], *args, **kwargs): 
     obj = None
-    component_class_name = conf.components.get(component_type, default_class_name)
+    component_class_name = conf.get("components",{}).get(component_type, default_class_name)
     if component_class_name is not None:
         cl = load_class(component_class_name) 
         if cl is not None: 
             obj = cl(conf=conf.get(component_type, {}), pipeline_conf=pipeline_conf, runner_conf=runner_conf,
                      parent_process=parent_process, problem_type=problem_type, components=dependent_components, *args, **kwargs)
             setattr(self_obj, component_type, obj)
     return obj 
 
 #registers pipeline as an attribute of the provided object
 def register_pipeline_class(self_obj, conf, pipeline_type, default_class_name=None, runner_conf = {}, 
                             parent_process = "runner", problem_type = None, dependent_components = {}, 
                             plugin_mods=[], *args, **kwargs): 
     obj = None 
-    pipeline_class_name = conf.pipelines.get(pipeline_type, default_class_name)
+    pipeline_class_name = conf.get("pipelines",{}).get(pipeline_type, default_class_name)
     if pipeline_class_name is not None: 
         cl = load_class(pipeline_class_name, class_type="pipeline")
         if cl is not None: 
             obj = cl(conf=conf.get(pipeline_type, {}), runner_conf=runner_conf, parent_process=parent_process,
                      problem_type=problem_type, components=dependent_components, plugin_mods=plugin_mods, *args, **kwargs)
             setattr(self_obj, pipeline_type, obj)
     return obj
```

### Comparing `lolpop-0.1.0a7/lolpop/utils/continual_utils.py` & `lolpop-0.1.0a8/lolpop/utils/continual_utils.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/utils/metaflow_utils.py` & `lolpop-0.1.0a8/lolpop/utils/metaflow_utils.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/lolpop/utils/mlflow_utils.py` & `lolpop-0.1.0a8/lolpop/utils/mlflow_utils.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a7/pyproject.toml` & `lolpop-0.1.0a8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lolpop"
-version = "v0.1.0-alpha.7"
+version = "v0.1.0-alpha.8"
 description = "A software engineering framework for machine learning workflows"
 authors = ["jordanvolz <jordan.volz@gmail.com>"]
 repository = "https://github.com/jordanvolz/lolpop"
 #hompage = 
 #documentation = 
 keywords = ["machine learning", "data science", "mlops"]
 license = "Apache-2.0"
```

### Comparing `lolpop-0.1.0a7/PKG-INFO` & `lolpop-0.1.0a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lolpop
-Version: 0.1.0a7
+Version: 0.1.0a8
 Summary: A software engineering framework for machine learning workflows
 Home-page: https://github.com/jordanvolz/lolpop
 License: Apache-2.0
 Keywords: machine learning,data science,mlops
 Author: jordanvolz
 Author-email: jordan.volz@gmail.com
 Requires-Python: >=3.9,<3.11
```

