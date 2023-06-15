# Comparing `tmp/tmlt_analytics-0.7.1.tar.gz` & `tmp/tmlt_analytics-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmlt_analytics-0.7.1.tar", max compression
+gzip compressed data, was "tmlt_analytics-0.7.2.tar", max compression
```

## Comparing `tmlt_analytics-0.7.1.tar` & `tmlt_analytics-0.7.2.tar`

### file list

```diff
@@ -1,167 +1,170 @@
--rw-r--r--   0        0        0    16001 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/CHANGELOG.rst
--rw-r--r--   0        0        0    11358 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/LICENSE
--rw-r--r--   0        0        0    20138 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/LICENSE.docs
--rw-r--r--   0        0        0      121 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/NOTICE
--rw-r--r--   0        0        0     2597 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/README.md
--rw-r--r--   0        0        0      951 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/_static/css/custom.css
--rw-r--r--   0        0        0    12470 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/_static/favicon.ico
--rw-r--r--   0        0        0     1001 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/_static/js/version-banner.js
--rw-r--r--   0        0        0    30903 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/_static/logo.png
--rw-r--r--   0        0        0       50 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/_templates/build-info.html
--rw-r--r--   0        0        0      408 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/_templates/layout.html
--rw-r--r--   0        0        0       23 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/_templates/package-name.html
--rw-r--r--   0        0        0     6786 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/conf.py
--rw-r--r--   0        0        0     1602 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/howto-guides/bigquery/bigquery-setup.rst
--rw-r--r--   0        0        0     3022 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/howto-guides/bigquery/docker-image.rst
--rw-r--r--   0        0        0     1237 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/howto-guides/bigquery/index.rst
--rw-r--r--   0        0        0     6303 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/howto-guides/bigquery/inputs-outputs.rst
--rw-r--r--   0        0        0     5770 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/howto-guides/bigquery/parameters.rst
--rw-r--r--   0        0        0     4763 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/howto-guides/bigquery/running-the-program.rst
--rw-r--r--   0        0        0     1716 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/howto-guides/bigquery/setup.rst
--rw-r--r--   0        0        0      314 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/howto-guides/index.rst
--rw-r--r--   0        0        0     4783 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/howto-guides/installation.rst
--rw-r--r--   0        0        0     2735 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/howto-guides/troubleshooting.rst
--rw-r--r--   0        0        0   118378 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/images/api_diagram.svg
--rw-r--r--   0        0        0    85925 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/images/chart_age_at_joining.png
--rw-r--r--   0        0        0    27267 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/images/chart_attacker_certainty.png
--rw-r--r--   0        0        0    41645 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/images/chart_average_age_by_edu.png
--rw-r--r--   0        0        0    34101 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/images/chart_books_by_unique_members.png
--rw-r--r--   0        0        0   104926 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/images/chart_counts_age_gender.png
--rw-r--r--   0        0        0    34006 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/images/chart_counts_different_eps.png
--rw-r--r--   0        0        0    25097 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/images/chart_counts_edu+sex.png
--rw-r--r--   0        0        0    13993 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/images/chart_counts_education.png
--rw-r--r--   0        0        0    41034 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/images/chart_error_vs_partition_age_edu.png
--rw-r--r--   0        0        0    59042 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/chart_favorite_genres.png
--rw-r--r--   0        0        0    14310 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/chart_filters_education.png
--rw-r--r--   0        0        0    30330 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/chart_genres_by_age.png
--rw-r--r--   0        0        0    14782 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/chart_quantiles_education.png
--rw-r--r--   0        0        0    20853 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/chart_senior_counts_1.png
--rw-r--r--   0        0        0    21067 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/chart_senior_counts_2.png
--rw-r--r--   0        0        0    29335 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/chart_teen_edu_counts.png
--rw-r--r--   0        0        0    20226 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/chart_younger_age_counts.png
--rw-r--r--   0        0        0    29155 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/clamping_bounds_averages.png
--rw-r--r--   0        0        0     9416 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/clamping_bounds_schema.png
--rw-r--r--   0        0        0    18639 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/flat_map_row_example.svg
--rw-r--r--   0        0        0    23590 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/flow_chart_truncation.svg
--rw-r--r--   0        0        0    14685 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/histogram_books_borrowed.png
--rw-r--r--   0        0        0     1844 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/index_api.svg
--rw-r--r--   0        0        0      609 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/index_howto_guides.svg
--rw-r--r--   0        0        0     1196 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/index_more.svg
--rw-r--r--   0        0        0      604 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/index_topic_guides.svg
--rw-r--r--   0        0        0     1371 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/index_tutorials.svg
--rw-r--r--   0        0        0    23369 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/intuitive_noise_visualization.png
--rw-r--r--   0        0        0    30903 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/logo.png
--rw-r--r--   0        0        0    59239 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/private_join_example.svg
--rw-r--r--   0        0        0    35838 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/private_join_tables.svg
--rw-r--r--   0        0        0    32227 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/public_join_example_zips.svg
--rw-r--r--   0        0        0     5748 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/index.rst
--rw-r--r--   0        0        0      662 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/intersphinx_mapping.json
--rw-r--r--   0        0        0     3169 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/privacy-policy.rst
--rw-r--r--   0        0        0     2024 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/templates/python/class.rst
--rw-r--r--   0        0        0     3440 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/templates/python/module.rst
--rw-r--r--   0        0        0      396 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/topic-guides/index.rst
--rw-r--r--   0        0        0    11697 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/topic-guides/nulls-nans-infinities.rst
--rw-r--r--   0        0        0     8608 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/topic-guides/privacy-budgets.rst
--rw-r--r--   0        0        0     6595 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/topic-guides/privacy-promise.rst
--rw-r--r--   0        0        0     7726 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/topic-guides/spark.rst
--rw-r--r--   0        0        0    12414 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/topic-guides/understanding-sensitivity.rst
--rw-r--r--   0        0        0     8462 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/topic-guides/working-with-sessions.rst
--rw-r--r--   0        0        0     9124 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/tutorials/clamping-bounds.rst
--rw-r--r--   0        0        0     7246 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/tutorials/first-steps.rst
--rw-r--r--   0        0        0    18802 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/tutorials/groupby-queries.rst
--rw-r--r--   0        0        0      430 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/tutorials/index.rst
--rw-r--r--   0        0        0    12394 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/tutorials/more-with-privacy-ids.rst
--rw-r--r--   0        0        0     8475 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/tutorials/privacy-budget-basics.rst
--rw-r--r--   0        0        0    14008 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/tutorials/privacy-id-basics.rst
--rw-r--r--   0        0        0    16252 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/tutorials/simple-transformations.rst
--rw-r--r--   0        0        0     4789 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/examples/interactive_evaluation.ipynb
--rw-r--r--   0        0        0     5459 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/examples/private_join.ipynb
--rw-r--r--   0        0        0     6570 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/examples/zcdp_puredp_switching.ipynb
--rw-r--r--   0        0        0     4645 2023-05-23 19:27:07.805302 tmlt_analytics-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      108 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/test/__init__.py
--rw-r--r--   0        0        0     6965 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/test/conftest.py
--rw-r--r--   0        0        0      115 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/test/system/__init__.py
--rw-r--r--   0        0        0      108 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/test/system/session/__init__.py
--rw-r--r--   0        0        0     4265 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/conftest.py
--rw-r--r--   0        0        0      151 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/ids/__init__.py
--rw-r--r--   0        0        0    15227 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/ids/test_constraint_propagation.py
--rw-r--r--   0        0        0     6531 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/ids/test_count_distinct_optimization.py
--rw-r--r--   0        0        0    21707 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/ids/test_l0_linf_truncation.py
--rw-r--r--   0        0        0    13996 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/ids/test_l1_truncation.py
--rw-r--r--   0        0        0     3965 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/ids/test_partition.py
--rw-r--r--   0        0        0      143 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/mixed/__init__.py
--rw-r--r--   0        0        0     5087 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/mixed/test_mixed_session.py
--rw-r--r--   0        0        0      152 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/rows/__init__.py
--rw-r--r--   0        0        0    26463 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/rows/conftest.py
--rw-r--r--   0        0        0    41576 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/rows/test_add_max_rows.py
--rw-r--r--   0        0        0     6122 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/rows/test_add_max_rows_in_max_groups.py
--rw-r--r--   0        0        0    13702 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/rows/test_add_max_rows_infs_nulls.py
--rw-r--r--   0        0        0     7708 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/rows/test_invalid.py
--rw-r--r--   0        0        0     4465 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/test_budgets.py
--rw-r--r--   0        0        0     2212 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/test_invalid_constraints.py
--rw-r--r--   0        0        0      108 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/__init__.py
--rw-r--r--   0        0        0      298 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/query_expr_compiler/__init__.py
--rw-r--r--   0        0        0    75173 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/query_expr_compiler/test_measurement_visitor.py
--rw-r--r--   0        0        0    54858 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/query_expr_compiler/test_output_schema_visitor.py
--rw-r--r--   0        0        0      107 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/query_expr_compiler/transformation_visitor/__init__.py
--rw-r--r--   0        0        0    17843 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/query_expr_compiler/transformation_visitor/conftest.py
--rw-r--r--   0        0        0    24152 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/query_expr_compiler/transformation_visitor/test_add_keys.py
--rw-r--r--   0        0        0    36750 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/query_expr_compiler/transformation_visitor/test_add_rows.py
--rw-r--r--   0        0        0     7610 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/query_expr_compiler/transformation_visitor/test_constraints.py
--rw-r--r--   0        0        0    14834 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/test_binning_spec.py
--rw-r--r--   0        0        0     2301 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/test_catalog.py
--rw-r--r--   0        0        0      657 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/test_cleanup.py
--rw-r--r--   0        0        0     5285 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/test_constraints.py
--rw-r--r--   0        0        0    21123 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/test_keyset.py
--rw-r--r--   0        0        0    14053 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/test_neighboring_relations.py
--rw-r--r--   0        0        0     3058 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/test_noise_info.py
--rw-r--r--   0        0        0     5865 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/test_privacy_budget.py
--rw-r--r--   0        0        0     5480 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test/unit/test_privacy_budget_rounding_helper.py
--rw-r--r--   0        0        0     3011 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test/unit/test_protected_change.py
--rw-r--r--   0        0        0    40754 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test/unit/test_query_builder.py
--rw-r--r--   0        0        0    64146 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test/unit/test_query_expr_compiler.py
--rw-r--r--   0        0        0    16787 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test/unit/test_query_expression.py
--rw-r--r--   0        0        0     4874 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test/unit/test_query_expression_visitor.py
--rw-r--r--   0        0        0     2172 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test/unit/test_schema.py
--rw-r--r--   0        0        0    13538 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test/unit/test_schema_conversion.py
--rw-r--r--   0        0        0    84283 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test/unit/test_session.py
--rw-r--r--   0        0        0     1604 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test/unit/test_table_identifiers.py
--rw-r--r--   0        0        0     5372 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test/unit/test_transformation_utils.py
--rw-r--r--   0        0        0      747 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test/unit/test_truncation_strategy.py
--rw-r--r--   0        0        0      518 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test/unit/test_utils.py
--rw-r--r--   0        0        0       37 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test_requirements.txt
--rw-r--r--   0        0        0      222 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/__init__.py
--rw-r--r--   0        0        0     3666 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_catalog.py
--rw-r--r--   0        0        0     3555 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_coerce_spark_schema.py
--rw-r--r--   0        0        0    16162 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_neighboring_relation.py
--rw-r--r--   0        0        0     6137 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_neighboring_relation_visitor.py
--rw-r--r--   0        0        0     5341 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_noise_info.py
--rw-r--r--   0        0        0     4021 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_privacy_budget_rounding_helper.py
--rw-r--r--   0        0        0      184 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_query_expr_compiler/__init__.py
--rw-r--r--   0        0        0     9810 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_query_expr_compiler/_compiler.py
--rw-r--r--   0        0        0     7694 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_query_expr_compiler/_constraint_propagation.py
--rw-r--r--   0        0        0    38980 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py
--rw-r--r--   0        0        0    46275 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py
--rw-r--r--   0        0        0    60186 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_query_expr_compiler/_transformation_visitor.py
--rw-r--r--   0        0        0    12795 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_schema.py
--rw-r--r--   0        0        0     1250 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_table_identifier.py
--rw-r--r--   0        0        0     3980 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_table_reference.py
--rw-r--r--   0        0        0    10148 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_transformation_utils.py
--rw-r--r--   0        0        0      420 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_type_checking.py
--rw-r--r--   0        0        0    11748 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/binning_spec.py
--rw-r--r--   0        0        0      306 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/cleanup.py
--rw-r--r--   0        0        0      458 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/constraints/__init__.py
--rw-r--r--   0        0        0     1101 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/constraints/_base.py
--rw-r--r--   0        0        0      735 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/constraints/_simplify.py
--rw-r--r--   0        0        0    12758 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/constraints/_truncation.py
--rw-r--r--   0        0        0    11850 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/keyset.py
--rw-r--r--   0        0        0    10390 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/privacy_budget.py
--rw-r--r--   0        0        0     5482 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/protected_change.py
--rw-r--r--   0        0        0        0 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/py.typed
--rw-r--r--   0        0        0   126828 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/query_builder.py
--rw-r--r--   0        0        0    41097 2023-05-23 19:26:33.548538 tmlt_analytics-0.7.1/tmlt/analytics/query_expr.py
--rw-r--r--   0        0        0    77763 2023-05-23 19:26:33.548538 tmlt_analytics-0.7.1/tmlt/analytics/session.py
--rw-r--r--   0        0        0     3965 2023-05-23 19:26:33.548538 tmlt_analytics-0.7.1/tmlt/analytics/truncation_strategy.py
--rw-r--r--   0        0        0     5397 2023-05-23 19:26:33.548538 tmlt_analytics-0.7.1/tmlt/analytics/utils.py
--rw-r--r--   0        0        0     3532 1970-01-01 00:00:00.000000 tmlt_analytics-0.7.1/setup.py
--rw-r--r--   0        0        0     3860 1970-01-01 00:00:00.000000 tmlt_analytics-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    18237 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/CHANGELOG.rst
+-rw-r--r--   0        0        0    11358 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/LICENSE
+-rw-r--r--   0        0        0    20138 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/LICENSE.docs
+-rw-r--r--   0        0        0      121 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/NOTICE
+-rw-r--r--   0        0        0     2593 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/README.md
+-rw-r--r--   0        0        0      951 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/_static/css/custom.css
+-rw-r--r--   0        0        0    12470 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/_static/favicon.ico
+-rw-r--r--   0        0        0     1001 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/_static/js/version-banner.js
+-rw-r--r--   0        0        0    30903 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/_static/logo.png
+-rw-r--r--   0        0        0       50 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/_templates/build-info.html
+-rw-r--r--   0        0        0      408 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/_templates/layout.html
+-rw-r--r--   0        0        0       23 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/_templates/package-name.html
+-rw-r--r--   0        0        0     6786 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/conf.py
+-rw-r--r--   0        0        0     1599 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/howto-guides/bigquery/bigquery-setup.rst
+-rw-r--r--   0        0        0     3005 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/howto-guides/bigquery/docker-image.rst
+-rw-r--r--   0        0        0     1225 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/howto-guides/bigquery/index.rst
+-rw-r--r--   0        0        0     6280 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/howto-guides/bigquery/inputs-outputs.rst
+-rw-r--r--   0        0        0     5760 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/howto-guides/bigquery/parameters.rst
+-rw-r--r--   0        0        0     4733 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/howto-guides/bigquery/running-the-program.rst
+-rw-r--r--   0        0        0     1706 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/howto-guides/bigquery/setup.rst
+-rw-r--r--   0        0        0     6911 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/howto-guides/databricks.rst
+-rw-r--r--   0        0        0      328 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/howto-guides/index.rst
+-rw-r--r--   0        0        0     4783 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/howto-guides/installation.rst
+-rw-r--r--   0        0        0     2735 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/howto-guides/troubleshooting.rst
+-rw-r--r--   0        0        0   118378 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/images/api_diagram.svg
+-rw-r--r--   0        0        0    85925 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/images/chart_age_at_joining.png
+-rw-r--r--   0        0        0    27267 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/images/chart_attacker_certainty.png
+-rw-r--r--   0        0        0    41645 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/images/chart_average_age_by_edu.png
+-rw-r--r--   0        0        0    34101 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/images/chart_books_by_unique_members.png
+-rw-r--r--   0        0        0   104926 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/chart_counts_age_gender.png
+-rw-r--r--   0        0        0    34006 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/chart_counts_different_eps.png
+-rw-r--r--   0        0        0    25097 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/chart_counts_edu+sex.png
+-rw-r--r--   0        0        0    13993 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/chart_counts_education.png
+-rw-r--r--   0        0        0    41034 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/chart_error_vs_partition_age_edu.png
+-rw-r--r--   0        0        0    59042 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/chart_favorite_genres.png
+-rw-r--r--   0        0        0    14310 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/chart_filters_education.png
+-rw-r--r--   0        0        0    30330 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/chart_genres_by_age.png
+-rw-r--r--   0        0        0    14782 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/chart_quantiles_education.png
+-rw-r--r--   0        0        0    20853 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/chart_senior_counts_1.png
+-rw-r--r--   0        0        0    21067 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/chart_senior_counts_2.png
+-rw-r--r--   0        0        0    29335 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/chart_teen_edu_counts.png
+-rw-r--r--   0        0        0    20226 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/chart_younger_age_counts.png
+-rw-r--r--   0        0        0    29155 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/clamping_bounds_averages.png
+-rw-r--r--   0        0        0     9416 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/clamping_bounds_schema.png
+-rw-r--r--   0        0        0    18639 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/flat_map_row_example.svg
+-rw-r--r--   0        0        0    23590 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/flow_chart_truncation.svg
+-rw-r--r--   0        0        0    14685 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/histogram_books_borrowed.png
+-rw-r--r--   0        0        0     1844 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/index_api.svg
+-rw-r--r--   0        0        0      609 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/index_howto_guides.svg
+-rw-r--r--   0        0        0     1196 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/index_more.svg
+-rw-r--r--   0        0        0      604 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/index_topic_guides.svg
+-rw-r--r--   0        0        0     1371 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/index_tutorials.svg
+-rw-r--r--   0        0        0    23369 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/intuitive_noise_visualization.png
+-rw-r--r--   0        0        0    30903 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/logo.png
+-rw-r--r--   0        0        0    85314 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/images/mock_checkout_logs.svg
+-rw-r--r--   0        0        0    59239 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/images/private_join_example.svg
+-rw-r--r--   0        0        0    35838 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/images/private_join_tables.svg
+-rw-r--r--   0        0        0    32227 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/images/public_join_example_zips.svg
+-rw-r--r--   0        0        0     5602 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/index.rst
+-rw-r--r--   0        0        0      662 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/intersphinx_mapping.json
+-rw-r--r--   0        0        0     3169 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/privacy-policy.rst
+-rw-r--r--   0        0        0     2024 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/templates/python/class.rst
+-rw-r--r--   0        0        0     3440 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/templates/python/module.rst
+-rw-r--r--   0        0        0      396 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/topic-guides/index.rst
+-rw-r--r--   0        0        0    11697 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/topic-guides/nulls-nans-infinities.rst
+-rw-r--r--   0        0        0     8608 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/topic-guides/privacy-budgets.rst
+-rw-r--r--   0        0        0     6595 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/topic-guides/privacy-promise.rst
+-rw-r--r--   0        0        0     7726 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/topic-guides/spark.rst
+-rw-r--r--   0        0        0    12513 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/topic-guides/understanding-sensitivity.rst
+-rw-r--r--   0        0        0     8462 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/topic-guides/working-with-sessions.rst
+-rw-r--r--   0        0        0     9124 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/tutorials/clamping-bounds.rst
+-rw-r--r--   0        0        0     7246 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/doc/tutorials/first-steps.rst
+-rw-r--r--   0        0        0    18802 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/doc/tutorials/groupby-queries.rst
+-rw-r--r--   0        0        0      430 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/doc/tutorials/index.rst
+-rw-r--r--   0        0        0    12394 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/doc/tutorials/more-with-privacy-ids.rst
+-rw-r--r--   0        0        0     8452 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/doc/tutorials/privacy-budget-basics.rst
+-rw-r--r--   0        0        0    15179 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/doc/tutorials/privacy-id-basics.rst
+-rw-r--r--   0        0        0    16252 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/doc/tutorials/simple-transformations.rst
+-rw-r--r--   0        0        0     4789 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/examples/interactive_evaluation.ipynb
+-rw-r--r--   0        0        0     5459 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/examples/private_join.ipynb
+-rw-r--r--   0        0        0     6570 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/examples/zcdp_puredp_switching.ipynb
+-rw-r--r--   0        0        0     4646 2023-06-15 12:46:22.353936 tmlt_analytics-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/__init__.py
+-rw-r--r--   0        0        0     6965 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/conftest.py
+-rw-r--r--   0        0        0      115 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/__init__.py
+-rw-r--r--   0        0        0      108 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/__init__.py
+-rw-r--r--   0        0        0     5642 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/conftest.py
+-rw-r--r--   0        0        0      151 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/ids/__init__.py
+-rw-r--r--   0        0        0    15227 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/ids/test_constraint_propagation.py
+-rw-r--r--   0        0        0     6531 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/ids/test_count_distinct_optimization.py
+-rw-r--r--   0        0        0     9106 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/ids/test_id_col_operations.py
+-rw-r--r--   0        0        0    22181 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/ids/test_l0_linf_truncation.py
+-rw-r--r--   0        0        0    14256 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/ids/test_l1_truncation.py
+-rw-r--r--   0        0        0     3965 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/ids/test_partition.py
+-rw-r--r--   0        0        0      143 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/mixed/__init__.py
+-rw-r--r--   0        0        0     5087 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/mixed/test_mixed_session.py
+-rw-r--r--   0        0        0      152 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/rows/__init__.py
+-rw-r--r--   0        0        0    26463 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/rows/conftest.py
+-rw-r--r--   0        0        0    42789 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/rows/test_add_max_rows.py
+-rw-r--r--   0        0        0     6122 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/rows/test_add_max_rows_in_max_groups.py
+-rw-r--r--   0        0        0    13702 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/rows/test_add_max_rows_infs_nulls.py
+-rw-r--r--   0        0        0    11017 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/system/session/rows/test_invalid.py
+-rw-r--r--   0        0        0     4465 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/system/session/test_budgets.py
+-rw-r--r--   0        0        0     2212 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/system/session/test_invalid_constraints.py
+-rw-r--r--   0        0        0      108 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/__init__.py
+-rw-r--r--   0        0        0      298 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/query_expr_compiler/__init__.py
+-rw-r--r--   0        0        0    76707 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/query_expr_compiler/test_measurement_visitor.py
+-rw-r--r--   0        0        0    54860 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/query_expr_compiler/test_output_schema_visitor.py
+-rw-r--r--   0        0        0      107 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/query_expr_compiler/transformation_visitor/__init__.py
+-rw-r--r--   0        0        0    17843 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/query_expr_compiler/transformation_visitor/conftest.py
+-rw-r--r--   0        0        0    24152 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/query_expr_compiler/transformation_visitor/test_add_keys.py
+-rw-r--r--   0        0        0    36839 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/query_expr_compiler/transformation_visitor/test_add_rows.py
+-rw-r--r--   0        0        0     7610 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/query_expr_compiler/transformation_visitor/test_constraints.py
+-rw-r--r--   0        0        0    15631 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_binning_spec.py
+-rw-r--r--   0        0        0     2301 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_catalog.py
+-rw-r--r--   0        0        0      657 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_cleanup.py
+-rw-r--r--   0        0        0     5285 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_constraints.py
+-rw-r--r--   0        0        0    21123 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_keyset.py
+-rw-r--r--   0        0        0    14053 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_neighboring_relations.py
+-rw-r--r--   0        0        0     3401 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_noise_info.py
+-rw-r--r--   0        0        0     5865 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_privacy_budget.py
+-rw-r--r--   0        0        0     5480 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_privacy_budget_rounding_helper.py
+-rw-r--r--   0        0        0     3011 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_protected_change.py
+-rw-r--r--   0        0        0    40576 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_query_builder.py
+-rw-r--r--   0        0        0    63726 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_query_expr_compiler.py
+-rw-r--r--   0        0        0    16787 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_query_expression.py
+-rw-r--r--   0        0        0     4874 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_query_expression_visitor.py
+-rw-r--r--   0        0        0     2172 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_schema.py
+-rw-r--r--   0        0        0    13538 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_schema_conversion.py
+-rw-r--r--   0        0        0    87562 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_session.py
+-rw-r--r--   0        0        0     1604 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_table_identifiers.py
+-rw-r--r--   0        0        0     5372 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_transformation_utils.py
+-rw-r--r--   0        0        0      747 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_truncation_strategy.py
+-rw-r--r--   0        0        0      518 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_utils.py
+-rw-r--r--   0        0        0       37 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test_requirements.txt
+-rw-r--r--   0        0        0      222 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/tmlt/analytics/__init__.py
+-rw-r--r--   0        0        0     3666 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/tmlt/analytics/_catalog.py
+-rw-r--r--   0        0        0     3555 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/tmlt/analytics/_coerce_spark_schema.py
+-rw-r--r--   0        0        0    16162 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/tmlt/analytics/_neighboring_relation.py
+-rw-r--r--   0        0        0     7164 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/tmlt/analytics/_neighboring_relation_visitor.py
+-rw-r--r--   0        0        0     5683 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/tmlt/analytics/_noise_info.py
+-rw-r--r--   0        0        0     4021 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/tmlt/analytics/_privacy_budget_rounding_helper.py
+-rw-r--r--   0        0        0      184 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/tmlt/analytics/_query_expr_compiler/__init__.py
+-rw-r--r--   0        0        0    10044 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/tmlt/analytics/_query_expr_compiler/_compiler.py
+-rw-r--r--   0        0        0     7694 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/tmlt/analytics/_query_expr_compiler/_constraint_propagation.py
+-rw-r--r--   0        0        0    42627 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py
+-rw-r--r--   0        0        0    46889 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py
+-rw-r--r--   0        0        0    60357 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/_query_expr_compiler/_transformation_visitor.py
+-rw-r--r--   0        0        0    12795 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/_schema.py
+-rw-r--r--   0        0        0     1250 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/_table_identifier.py
+-rw-r--r--   0        0        0     3980 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/_table_reference.py
+-rw-r--r--   0        0        0    10148 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/_transformation_utils.py
+-rw-r--r--   0        0        0      420 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/_type_checking.py
+-rw-r--r--   0        0        0    11871 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/binning_spec.py
+-rw-r--r--   0        0        0      306 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/cleanup.py
+-rw-r--r--   0        0        0      458 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/constraints/__init__.py
+-rw-r--r--   0        0        0     1101 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/constraints/_base.py
+-rw-r--r--   0        0        0      735 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/constraints/_simplify.py
+-rw-r--r--   0        0        0    12758 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/constraints/_truncation.py
+-rw-r--r--   0        0        0    11850 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/keyset.py
+-rw-r--r--   0        0        0    10546 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/privacy_budget.py
+-rw-r--r--   0        0        0     5482 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/protected_change.py
+-rw-r--r--   0        0        0        0 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/py.typed
+-rw-r--r--   0        0        0   129668 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/query_builder.py
+-rw-r--r--   0        0        0    41076 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/query_expr.py
+-rw-r--r--   0        0        0    80902 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/session.py
+-rw-r--r--   0        0        0     3965 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/truncation_strategy.py
+-rw-r--r--   0        0        0     5397 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/utils.py
+-rw-r--r--   0        0        0     3529 1970-01-01 00:00:00.000000 tmlt_analytics-0.7.2/setup.py
+-rw-r--r--   0        0        0     3908 1970-01-01 00:00:00.000000 tmlt_analytics-0.7.2/PKG-INFO
```

### Comparing `tmlt_analytics-0.7.1/CHANGELOG.rst` & `tmlt_analytics-0.7.2/CHANGELOG.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,39 @@
 .. _analytics-changelog:
 
 Changelog
 =========
 
+0.7.2 - 2023-06-15
+------------------
+
+This release adds support for running Tumult Analytics on Python 3.10.
+It also enables adding continuous Gaussian noise to query results, and addresses a number of bugs and API inconsistencies.
+
+Added
+~~~~~
+- Tumult Analytics now supports Python 3.10 in addition to the previously-supported versions.
+- Queries evaluated with zCDP budgets can now use continuous Gaussian noise, allowing the use of Gaussian noise for queries with non-integer results.
+
+Changed
+~~~~~~~
+- The :meth:`QueryBuilder.replace_null_and_nan()<tmlt.analytics.query_builder.QueryBuilder.replace_null_and_nan>` and :meth:`QueryBuilder.drop_null_and_nan()<tmlt.analytics.query_builder.QueryBuilder.drop_null_and_nan>` methods now accept empty column specifications on tables with an :class:`~tmlt.analytics.protected_change.AddRowsWithID` protected change.
+  Replacing/dropping nulls on ID columns is still not allowed, but the ID column will now automatically be excluded in this case rather than raising an exception.
+- :meth:`BinningSpec.bins()<tmlt.analytics.binning_spec.BinningSpec.bins>` used to only include the NaN bin if the provided bin edges were floats.
+  However, float-valued columns can be binned with integer bin edges, which resulted in a confusing situation where a :class:`~tmlt.analytics.binning_spec.BinningSpec` could indicate that it would not use a NaN bin but still place values in the NaN bin.
+  To avoid this, :meth:`BinningSpec.bins()<tmlt.analytics.binning_spec.BinningSpec.bins>` now always includes the NaN bin if one was specified, regardless of whether the bin edge type can represent NaN values.
+- The automatically-generated bin names in :class:`~tmlt.analytics.binning_spec.BinningSpec` now quote strings when they are used as bin edges.
+  For example, the bin generated by ``BinningSpec(["0", "1"])`` is now ``['0', '1']`` where it was previously ``[0, 1]``.
+  Bins with edges of other types are not affected.
+
+Fixed
+~~~~~
+- Creating a :class:`~tmlt.analytics.session.Session` with multiple tables in an ID space used to fail if some of those tables' ID columns allowed nulls and others did not.
+  This no longer occurs, and in such cases all of the tables' ID columns are made nullable.
+
 0.7.1 - 2023-05-23
 ------------------
 
 This is a maintenance release that mainly contains documentation updates.
 It also fixes a bug where installing Tumult Analytics using pip 23 and above could fail due to a dependency mismatch.
 
 0.7.0 - 2023-04-27
```

### Comparing `tmlt_analytics-0.7.1/LICENSE` & `tmlt_analytics-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/LICENSE.docs` & `tmlt_analytics-0.7.2/LICENSE.docs`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/README.md` & `tmlt_analytics-0.7.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,10 +54,10 @@
 }
 ```
 
 ## License
 
 Copyright Tumult Labs 2023
 
-The Tumult Platform source code is licensed under the Apache License, version 2.0 (Apache-2.0).
-The Tumult Platform documentation is licensed under
+Tumult Analytics' source code is licensed under the Apache License, version 2.0 (Apache-2.0).
+Tumult Analytics' documentation is licensed under
 Creative Commons Attribution-ShareAlike 4.0 International (CC-BY-SA-4.0).
```

### Comparing `tmlt_analytics-0.7.1/doc/_static/css/custom.css` & `tmlt_analytics-0.7.2/doc/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/_static/favicon.ico` & `tmlt_analytics-0.7.2/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/_static/js/version-banner.js` & `tmlt_analytics-0.7.2/doc/_static/js/version-banner.js`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/_static/logo.png` & `tmlt_analytics-0.7.2/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/conf.py` & `tmlt_analytics-0.7.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/howto-guides/bigquery/bigquery-setup.rst` & `tmlt_analytics-0.7.2/doc/howto-guides/bigquery/bigquery-setup.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _BigQuery setup:
 
 Introduction to BigQuery
 ========================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2022
+    Copyright Tumult Labs 2023
 
 BigQuery is a serverless, highly scalable, cost-effective, and fully managed
 cloud data warehouse for analytics.
 
 In this first section, we will upload a file to BigQuery to use as input for our DP query.
 We will use the same input data as for the Tumult Analytics :ref:`tutorial<first steps>`, which is provided
 as a CSV file.
@@ -23,14 +23,14 @@
 7. Select the file format as "CSV"
 8. Under Schema, select "Auto detect"
 9. Click on "Create table"
 
 .. _BigQuery interface: https://console.cloud.google.com/bigquery
 
 With our data in place, we can explore the data in BigQuery.
-We can expand the dataset we previously created, open up the table 
+We can expand the dataset we previously created, open up the table
 to see the schema, and query the data in the query editor
 using SQL.
 
-Now that we've set up our environment in BigQuery, let's move on to the :ref:`next part<bigquery inputs and outputs>` 
-of the topic guide and see how we would modify a simple Tumult Analtyics program to be able 
+Now that we've set up our environment in BigQuery, let's move on to the :ref:`next part<bigquery inputs and outputs>`
+of the topic guide and see how we would modify a simple Tumult Analtyics program to be able
 to run in BigQuery.
```

### Comparing `tmlt_analytics-0.7.1/doc/howto-guides/bigquery/docker-image.rst` & `tmlt_analytics-0.7.2/doc/howto-guides/bigquery/docker-image.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 .. _GCP Docker Image:
 
 Creating a Docker image for GCP
 ===============================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2022
+    Copyright Tumult Labs 2023
 
-In this final part of the topic guide, we will customize our own 
+In this final part of the topic guide, we will customize our own
 Docker image to contain additional libraries and dependencies.
-A working knowledge of Docker is useful to understand this section, 
-but if you have never used Docker before, you can still follow the 
+A working knowledge of Docker is useful to understand this section,
+but if you have never used Docker before, you can still follow the
 instructions below.
 
-The instructions below show how the public Tumult Analytics demo 
+The instructions below show how the public Tumult Analytics demo
 image was created, and can be used as a template for your own image.
 
 First, we will need to create a new Docker repository in the `Artifact Registry`_.
 
 .. _Cloud Build: https://console.cloud.google.com/cloud-build
 .. _Artifact Registry: https://console.cloud.google.com/artifacts
 
-Next, we will create the image that will be placed in the repository. We will need 
-to create two files for this locally. The first, ``Dockerfile``, contains Docker 
+Next, we will create the image that will be placed in the repository. We will need
+to create two files for this locally. The first, ``Dockerfile``, contains Docker
 instructions to build the image.
 
 .. code-block:: dockerfile
 
     FROM python:3.9-bullseye
-    
+
     # Install the dependencies needed for GCP
     RUN apt-get update && apt-get install -y procps tini
 
     # Install Tumult Analytics
     RUN pip install --upgrade pip && \
         pip install tmlt.analytics
 
     # Add additional dependancies here as needed
     # RUN pip install <package>
-    
+
     # Set up the Spark user for GCP integration
     RUN useradd -ms /bin/bash spark -u 1099
     USER 1099
     WORKDIR /home/spark
     ENV PYSPARK_PYTHON="/usr/local/bin/python"
 
-The second file, ``cloudbuild.yaml``, contains the instructions for the 
+The second file, ``cloudbuild.yaml``, contains the instructions for the
 Google command line tool to build the image and place it in the repository.
 In our example, we named our repository ``analytics``, and our image ``tutorial``.
-You will need to replace ``REPOSITORY NAME`` and ``IMAGE NAME`` with your 
-repository and image names you set earlier. We do not need to set the 
+You will need to replace ``REPOSITORY NAME`` and ``IMAGE NAME`` with your
+repository and image names you set earlier. We do not need to set the
 ``$PROJECT_ID`` variable as it is automatically set by the Google command line.
 
 .. code-block:: yaml
 
     steps:
     - name: 'gcr.io/cloud-builders/docker'
       args: ['build', '-t', 'us-docker.pkg.dev/$PROJECT_ID/[REPOSITORY NAME]/[IMAGE NAME]', '.']
```

### Comparing `tmlt_analytics-0.7.1/doc/howto-guides/bigquery/index.rst` & `tmlt_analytics-0.7.2/doc/howto-guides/bigquery/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Using Tumult Analytics on BigQuery
 ==================================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2022
+    Copyright Tumult Labs 2023
 
-This topic guide explains how to use Tumult Analytics on BigQuery.
-We will guide you to getting a minimal example of a Tumult 
+This guide explains how to use Tumult Analytics on BigQuery.
+We will guide you to getting a minimal example of a Tumult
 Analytics program running on BigQuery, then we will explain how to
 modify this program to work with custom parameters and custom
 libraries.
 
-Following this topic guide requires your project to have access to 
-the public preview of the stored procedures for Apache Spark. You 
+Following this topic guide requires your project to have access to
+the public preview of the stored procedures for Apache Spark. You
 can enroll in the preview by completing the `enrollment form`_.
 
-Throughout this topic guide, you must use the same region for all 
-the objects we will create and use in Google Cloud Platform (GCP): BigQuery tables, 
-Cloud Storage buckets, Artifact repositories, etc., must all 
+Throughout this topic guide, you must use the same region for all
+the objects we will create and use in Google Cloud Platform (GCP): BigQuery tables,
+Cloud Storage buckets, Artifact repositories, etc., must all
 reside in the same `GCP region`_.
 
 .. _GCP region: https://cloud.google.com/compute/docs/regions-zones
 .. _enrollment form: https://cloud.google.com/bigquery/docs/spark-procedures
 
-Let's get started by setting up the environment in Google Cloud 
+Let's get started by setting up the environment in Google Cloud
 Platform :ref:`here<gcp setup>`.
 
 .. toctree::
    :maxdepth: 1
 
    setup
    bigquery-setup
    inputs-outputs
    running-the-program
    parameters
-   docker-image
+   docker-image
```

### Comparing `tmlt_analytics-0.7.1/doc/howto-guides/bigquery/inputs-outputs.rst` & `tmlt_analytics-0.7.2/doc/howto-guides/bigquery/inputs-outputs.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 .. _BigQuery inputs and outputs:
 
 BigQuery inputs and outputs
 ===========================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2022
+    Copyright Tumult Labs 2023
 
-In this section, we will show how to adapt a Tumult Analytics 
-program to use BigQuery inputs and outputs, and provide a minimal 
+In this section, we will show how to adapt a Tumult Analytics
+program to use BigQuery inputs and outputs, and provide a minimal
 example of a BigQuery-compatible program.
 
-We will use the simple program from :ref:`the first tutorial<first steps>` 
-which constructs a differentially private count of the number of 
-members in a fake dataset containing members of a public library 
+We will use the simple program from :ref:`the first tutorial<first steps>`
+which constructs a differentially private count of the number of
+members in a fake dataset containing members of a public library
 ``library-members``.
 
 .. testcode::
 
     from pyspark import SparkFiles
     from pyspark.sql import SparkSession
     from tmlt.analytics.privacy_budget import PureDPBudget
@@ -52,52 +52,52 @@
 
     +-----+
     |count|
     +-----+
     |...|
     +-----+
 
-We will explain what needs to change to adapt this program to work on 
+We will explain what needs to change to adapt this program to work on
 BigQuery.
 
 Setup
 -----
 
-To be able to write to BigQuery, we need to create a Google Cloud 
+To be able to write to BigQuery, we need to create a Google Cloud
 Storage bucket to store the intermediate results and our programs.
 
 1. Go to the `Cloud Storage interface`_
 2. Create a new bucket by clicking on ``+ CREATE``
 
-In this topic guide, we will create two buckets. One to house our 
-programs, and the other for intermediate materialization. For this 
-topic guide, we will be calling ours ``tumult-shared-procedures`` 
-and ``tumult-warehouse`` respectively. Since buckets use a global 
+In this topic guide, we will create two buckets. One to house our
+programs, and the other for intermediate materialization. For this
+topic guide, we will be calling ours ``tumult-shared-procedures``
+and ``tumult-warehouse`` respectively. Since buckets use a global
 namespace, you will need to choose a unique name for your bucket.
 
 .. _BigQuery interface: https://console.cloud.google.com/bigquery
 .. _Cloud Storage interface: https://console.cloud.google.com/storage
 
 Creating the Spark Session
 --------------------------
 
-Our Spark session will use a `Google Cloud Storage`_ bucket to store 
-intermediate results that are generated and used by Tumult Analytics 
-to compute the differentially private results. This is done by setting 
+Our Spark session will use a `Google Cloud Storage`_ bucket to store
+intermediate results that are generated and used by Tumult Analytics
+to compute the differentially private results. This is done by setting
 the ``spark.sql.warehouse.dir`` configuration option.
 
 .. _Google Cloud Storage: https://cloud.google.com/storage
 
-Additionally, writing to BigQuery tables requires an intermediate 
-buffer to write to, which is also stored in a Google Cloud Storage 
+Additionally, writing to BigQuery tables requires an intermediate
+buffer to write to, which is also stored in a Google Cloud Storage
 bucket. In this case, we can use the same bucket for both purposes.
 You will need to replace ``BUCKET`` with your own bucket name.
 
-.. note:: Whenever working with sensitive data, make sure that these 
-    buckets are securely configured and that unauthorized users 
+.. note:: Whenever working with sensitive data, make sure that these
+    buckets are securely configured and that unauthorized users
     cannot access them.
 
 .. code-block:: diff
 
     -spark = SparkSession.builder.getOrCreate()
     +BUCKET = "my-gcs-bucket"
     +spark = (
@@ -107,21 +107,21 @@
     +    .config("temporaryGcsBucket", BUCKET)
     +    .getOrCreate()
     +)
 
 Specifying BigQuery inputs and outputs
 --------------------------------------
 
-Then, using BigQuery for inputs/outputs is straightforward. Instead of 
-reading from a CSV file, we specify that the format we're reading from is 
-``BigQuery``, with additional ``option`` properties that we set to indicate 
+Then, using BigQuery for inputs/outputs is straightforward. Instead of
+reading from a CSV file, we specify that the format we're reading from is
+``BigQuery``, with additional ``option`` properties that we set to indicate
 each table path.
 
 Here is a code snippet for reading a BigQuery input.
-You will need to replace ``PROJECT``, ``DATASET``, and ``TABLE`` with 
+You will need to replace ``PROJECT``, ``DATASET``, and ``TABLE`` with
 your own values.
 
 .. code-block:: diff
 
     -spark.sparkContext.addFile(
     -    "https://tumult-public.s3.amazonaws.com/library-members.csv"
     -)
@@ -133,15 +133,15 @@
     +TABLE   = "library_members"
     +members_df = (
     +  spark.read.format("bigquery")
     +  .option("table", f"{PROJECT}:{DATASET}.{TABLE}")
     +  .load()
     +)
 
-And here is a snippet to write to a BigQuery table. Here we write our 
+And here is a snippet to write to a BigQuery table. Here we write our
 counts to ``tumult-labs.analytics_tutorial.library_counts``.
 
 .. code-block:: python
 
     (
         total_count
         .write.format("bigquery")
```

### Comparing `tmlt_analytics-0.7.1/doc/howto-guides/bigquery/parameters.rst` & `tmlt_analytics-0.7.2/doc/howto-guides/bigquery/parameters.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 .. _Passing parameters to a stored procedure:
 
 Passing parameters to a stored procedure
 ========================================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2022
+    Copyright Tumult Labs 2023
 
-In this additional section of the topic guide, we will explain how 
-to pass parameters from BigQuery to the stored procedure containing 
-our Tumult Analytics program. This makes it possible to customize the 
-call, by specifying e.g. different inputs or outputs table, or privacy 
+In this additional section of the topic guide, we will explain how
+to pass parameters from BigQuery to the stored procedure containing
+our Tumult Analytics program. This makes it possible to customize the
+call, by specifying e.g. different inputs or outputs table, or privacy
 parameters, without modifying the underlying program.
 
 Recall that our remote procedure from :ref:`earlier<running the program>` had no parameters.
 
 .. code-block:: sql
 
     CREATE OR REPLACE PROCEDURE `tumult-labs.analytics_tutorial.count_members`()
@@ -53,15 +53,15 @@
 
     CALL `tumult-labs.analytics_tutorial.count_members`(
         "tumult-warehouse",
         "tumult-labs.analytics_tutorial.library_members",
         "tumult-labs.analytics_tutorial.member_counts"
     )
 
-.. note:: Replace the bucket, input, and output with the values 
+.. note:: Replace the bucket, input, and output with the values
     specific to your project.
 
 Now, recall our Tufts Analytics program defined :ref:`earlier<bigquery inputs and outputs>`.
 
 .. code-block:: python
 
     import json
@@ -109,17 +109,17 @@
         .mode("overwrite")
         .option("table", OUTPUT_TABLE)
         .save()
     )
 
 We need to modify this so that we can receive the parameters ``bucket``, ``input``, and ``output``.
 To read in our new parameters, we need to read the environment variables.
-Each parameter is stored in the environment variable in JSON format, and its 
-name has the following format: ``BIGQUERY_PROC_PARAM.[PARAMETER NAME]``. For example, 
-if we have a parameter named ``epsilon``, we can access it with 
+Each parameter is stored in the environment variable in JSON format, and its
+name has the following format: ``BIGQUERY_PROC_PARAM.[PARAMETER NAME]``. For example,
+if we have a parameter named ``epsilon``, we can access it with
 ``os.environ["BIGQUERY_PROC_PARAM.epsilon"]``.
 
 .. code-block:: diff
 
     +import json
     +import os
 
@@ -180,10 +180,10 @@
      total_count
      .write.format("bigquery")
      .mode("overwrite")
      .option("table", OUTPUT_TABLE)
      .save()
    )
 
-In the :ref:`final part of this topic guide<gcp docker image>`, 
-we will see how to create a customized GCP-compatible Docker image 
+In the :ref:`final part of this topic guide<gcp docker image>`,
+we will see how to create a customized GCP-compatible Docker image
 to run Tumult Analytics.
```

### Comparing `tmlt_analytics-0.7.1/doc/howto-guides/bigquery/running-the-program.rst` & `tmlt_analytics-0.7.2/doc/howto-guides/bigquery/running-the-program.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,112 +1,112 @@
 .. _Running the program:
 
 Calling Tumult Analytics from a BigQuery stored procedure
 =========================================================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2022
+    Copyright Tumult Labs 2023
 
-In this section, we will explain how to run a Tumult Analytics 
-program directly from BigQuery. We will do so using the sample 
-program from the :ref:`second part<bigquery inputs and outputs>` 
+In this section, we will explain how to run a Tumult Analytics
+program directly from BigQuery. We will do so using the sample
+program from the :ref:`second part<bigquery inputs and outputs>`
 of this topic guide.
 
-You should also have data in BigQuery, and a Google Cloud Storage bucket 
-to store intermediate results from the previous parts. Let's assume that 
-our table is as initialized in the :ref:`BigQuery setup section<bigquery setup>` 
-``tumult-labs.analytics_tutorial.library_members``. We'll use the public 
-Tumult Labs image being hosted at 
+You should also have data in BigQuery, and a Google Cloud Storage bucket
+to store intermediate results from the previous parts. Let's assume that
+our table is as initialized in the :ref:`BigQuery setup section<bigquery setup>`
+``tumult-labs.analytics_tutorial.library_members``. We'll use the public
+Tumult Labs image being hosted at
 ``us-docker.pkg.dev/tumult-labs/analytics/tutorial:demo``.
 
-.. note:: If you want to use your own image, you can find the instructions 
+.. note:: If you want to use your own image, you can find the instructions
    to do so in the :ref:`Docker section<gcp docker image>` of this topic guide.
 
 .. code-block:: python
 
     PROJECT          = "tumult-labs"
     BIGQUERY_DATASET = "analytics_tutorial"
     BIGQUERY_TABLE   = "library_members"
     IMAGE_REPOSITORY = "analytics"
     IMAGE_NAME       = "tutorial"
 
-In BigQuery, tables are used to store the data, and datasets are used 
+In BigQuery, tables are used to store the data, and datasets are used
 to group tables and procedures together.
-To call external Spark-based programs from BigQuery, we must create 
+To call external Spark-based programs from BigQuery, we must create
 a *stored procedure*, which is associated with a BigQuery dataset.
 
 First, we need to construct an external data source pointing to Apache Spark.
 
 1. Press the "+ Add Data" button in the top left corner of the `BigQuery console`_.
 2. Choose "Connections to external data sources".
 3. Select `Apache Spark` as the connection type.
 4. Choose a name for the connection, and remember it.
    In our running example, we will call it ``bigspark``.
 5. Create the connection.
 
 .. _BigQuery console: https://console.cloud.google.com/bigquery
 
-After creating the connection, in the explorer to the left above our dataset, 
-there is now an "External connections" section, in which we can see our 
-Apache Spark connection. Its name is the connection name appended 
-with the region. In our example, it is ``us.bigspark``, as our connection name is 
+After creating the connection, in the explorer to the left above our dataset,
+there is now an "External connections" section, in which we can see our
+Apache Spark connection. Its name is the connection name appended
+with the region. In our example, it is ``us.bigspark``, as our connection name is
 ``bigspark`` and it is situated in the ``us`` region.
 
 Another thing we need to to with the connection is to copy the service account ID
 that was generated for this connection. We will need to grant this service account
 the necessary permissions it needs to run our Tumult Analytics program.
 
-To do so, we have to go to the `IAM & Admin`_ page, click "Grant access", paste 
+To do so, we have to go to the `IAM & Admin`_ page, click "Grant access", paste
 our service account ID in "New Principals", and assign it the following roles.
 
 .. _IAM & Admin: https://console.cloud.google.com/iam-admin/iam
 
 * BigQuery Data Editor
 * BigQuery Read Session User
 * BigQuery Job User
 * Storage Admin
 * Artifact Registry Reader
 
-Now, we can navigate back to the BigQuery page to create the stored 
+Now, we can navigate back to the BigQuery page to create the stored
 procedure directly from the BigQuery editor.
 
-For this example, we can ignore the parameters, as our script does not 
-take any. With the sample values used throughout this topic guide, and 
-choosing ``count_members`` as the name of our stored procedure, we end 
+For this example, we can ignore the parameters, as our script does not
+take any. With the sample values used throughout this topic guide, and
+choosing ``count_members`` as the name of our stored procedure, we end
 up with the following query.
 
 .. code-block:: sql
 
     CREATE OR REPLACE PROCEDURE `tumult-labs.analytics_tutorial.count_members`()
     WITH CONNECTION `tumult-labs.us.bigspark`
     OPTIONS (
         engine='SPARK',
         container_image='us-docker.pkg.dev/tumult-labs/analytics/tutorial:demo',
         main_file_uri='gs://tumult-shared-procedures/library_members.py'
     )
     LANGUAGE python
 
-.. note:: When copy-pasting the procedure creation script, make sure you 
+.. note:: When copy-pasting the procedure creation script, make sure you
   replace the procedure name and external connection name,
   to point to your own project dataset and connection.
 
-This creates a stored procedure that exists in 
-``tumult-labs.analytics_tutorial.count_members``, akin to defining a function. 
+This creates a stored procedure that exists in
+``tumult-labs.analytics_tutorial.count_members``, akin to defining a function.
 Finally you can run the remote procedure by calling it with the appropriate parameters.
 
 .. code-block:: sql
 
     CALL `tumult-labs.analytics_tutorial.count_members`()
 
-If successful, our script should produce a BigQuery table, which we can 
-see after a few minutes once we refresh the page. Otherwise, you can 
-check `Cloud Logging`_ for the results. This does require you to enable 
+If successful, our script should produce a BigQuery table, which we can
+see after a few minutes once we refresh the page. Otherwise, you can
+check `Cloud Logging`_ for the results. This does require you to enable
 the Cloud Logging API as well.
 
 .. _Cloud Logging: https://console.cloud.google.com/logs
 
-Congratulations! You have successfully created a stored procedure 
-that runs a Tumult Analytics program in BigQuery. The next few parts 
-of the topic guide will cover how to set your :ref:`own parameters<Passing parameters to a stored procedure>` to the 
-program passing it from the remote procedure, and creating a custom 
+Congratulations! You have successfully created a stored procedure
+that runs a Tumult Analytics program in BigQuery. The next few parts
+of the topic guide will cover how to set your :ref:`own parameters<Passing parameters to a stored procedure>` to the
+program passing it from the remote procedure, and creating a custom
 image to include the libraries necessary for your programs.
```

### Comparing `tmlt_analytics-0.7.1/doc/howto-guides/bigquery/setup.rst` & `tmlt_analytics-0.7.2/doc/howto-guides/bigquery/setup.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 .. _GCP setup:
 
 GCP setup
 =========
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2022
+    Copyright Tumult Labs 2023
 
-When entering Google Cloud Platform (GCP) for the first time, 
+When entering Google Cloud Platform (GCP) for the first time,
 you will be greeted with your project dashboard.
 
-The search bar on top of the page can be used to search for, 
+The search bar on top of the page can be used to search for,
 and navigate to, any service in GCP.
 
-In the first part of this topic guide, we will enable the APIs 
+In the first part of this topic guide, we will enable the APIs
 and permissions that are necessary for Tumult Analytics to work.
 
-First, we will enable all the necessary APIs required for 
+First, we will enable all the necessary APIs required for
 the rest of the guide. Navigate to the `APIs & Services`_
-page, and click on `Enable APIs and Services`. Then, 
+page, and click on `Enable APIs and Services`. Then,
 search for and enable the following APIs.
 
 .. _APIs & Services: https://console.cloud.google.com/apis/dashboard
 
 * Artifact Registry API
 * BigQuery API
 * BigQuery Connection API
 * Cloud Build API
 * Cloud Logging API
 * Cloud Storage API
 
-Next, we will make sure that we have sufficient permissions to 
-perform the operations needed for this guide. We can check this 
-by going to `IAM & Admin`_ then under your account, press the edit 
+Next, we will make sure that we have sufficient permissions to
+perform the operations needed for this guide. We can check this
+by going to `IAM & Admin`_ then under your account, press the edit
 button, shaped as a pencil on the right, and add the following permissions.
-If you cannot set the following permissions for yourself, 
+If you cannot set the following permissions for yourself,
 contact your organization administrator.
 
 .. _IAM & Admin: https://console.cloud.google.com/iam-admin/iam
 
 * Create a connection (BigQuery Connection Admin)
 * Read / Write GCS Buckets (Google Storage Admin)
 * Read Images (Artifact Registry Reader)
 * Run BigQuery jobs (BigQuery Job User)
 * Use BigQuery Datasets (BigQuery Data Editor)
 * View remote procedures (BigQuery Metadata Viewer)
 
-In the :ref:`next part of this topic guide<bigquery setup>`, 
+In the :ref:`next part of this topic guide<bigquery setup>`,
 we will see how to use BigQuery and how to upload our dataset to it.
```

### Comparing `tmlt_analytics-0.7.1/doc/howto-guides/installation.rst` & `tmlt_analytics-0.7.2/doc/howto-guides/installation.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/howto-guides/troubleshooting.rst` & `tmlt_analytics-0.7.2/doc/howto-guides/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/api_diagram.svg` & `tmlt_analytics-0.7.2/doc/images/api_diagram.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/chart_age_at_joining.png` & `tmlt_analytics-0.7.2/doc/images/chart_age_at_joining.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/chart_attacker_certainty.png` & `tmlt_analytics-0.7.2/doc/images/chart_attacker_certainty.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/chart_average_age_by_edu.png` & `tmlt_analytics-0.7.2/doc/images/chart_average_age_by_edu.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/chart_books_by_unique_members.png` & `tmlt_analytics-0.7.2/doc/images/chart_books_by_unique_members.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/chart_counts_age_gender.png` & `tmlt_analytics-0.7.2/doc/images/chart_counts_age_gender.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/chart_counts_different_eps.png` & `tmlt_analytics-0.7.2/doc/images/chart_counts_different_eps.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/chart_counts_edu+sex.png` & `tmlt_analytics-0.7.2/doc/images/chart_counts_edu+sex.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/chart_counts_education.png` & `tmlt_analytics-0.7.2/doc/images/chart_counts_education.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/chart_error_vs_partition_age_edu.png` & `tmlt_analytics-0.7.2/doc/images/chart_error_vs_partition_age_edu.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/chart_favorite_genres.png` & `tmlt_analytics-0.7.2/doc/images/chart_favorite_genres.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/chart_filters_education.png` & `tmlt_analytics-0.7.2/doc/images/chart_filters_education.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/chart_genres_by_age.png` & `tmlt_analytics-0.7.2/doc/images/chart_genres_by_age.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/chart_quantiles_education.png` & `tmlt_analytics-0.7.2/doc/images/chart_quantiles_education.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/chart_senior_counts_1.png` & `tmlt_analytics-0.7.2/doc/images/chart_senior_counts_1.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/chart_senior_counts_2.png` & `tmlt_analytics-0.7.2/doc/images/chart_senior_counts_2.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/chart_teen_edu_counts.png` & `tmlt_analytics-0.7.2/doc/images/chart_teen_edu_counts.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/chart_younger_age_counts.png` & `tmlt_analytics-0.7.2/doc/images/chart_younger_age_counts.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/clamping_bounds_averages.png` & `tmlt_analytics-0.7.2/doc/images/clamping_bounds_averages.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/clamping_bounds_schema.png` & `tmlt_analytics-0.7.2/doc/images/clamping_bounds_schema.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/flat_map_row_example.svg` & `tmlt_analytics-0.7.2/doc/images/flat_map_row_example.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/flow_chart_truncation.svg` & `tmlt_analytics-0.7.2/doc/images/flow_chart_truncation.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/histogram_books_borrowed.png` & `tmlt_analytics-0.7.2/doc/images/histogram_books_borrowed.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/index_api.svg` & `tmlt_analytics-0.7.2/doc/images/index_api.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/index_howto_guides.svg` & `tmlt_analytics-0.7.2/doc/images/index_howto_guides.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/index_more.svg` & `tmlt_analytics-0.7.2/doc/images/index_more.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/index_topic_guides.svg` & `tmlt_analytics-0.7.2/doc/images/index_topic_guides.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/index_tutorials.svg` & `tmlt_analytics-0.7.2/doc/images/index_tutorials.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/intuitive_noise_visualization.png` & `tmlt_analytics-0.7.2/doc/images/intuitive_noise_visualization.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/logo.png` & `tmlt_analytics-0.7.2/doc/images/logo.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/private_join_example.svg` & `tmlt_analytics-0.7.2/doc/images/private_join_example.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/private_join_tables.svg` & `tmlt_analytics-0.7.2/doc/images/private_join_tables.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/images/public_join_example_zips.svg` & `tmlt_analytics-0.7.2/doc/images/public_join_example_zips.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/index.rst` & `tmlt_analytics-0.7.2/doc/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -23,19 +23,16 @@
 - … *feature-rich*: it supports a large and ever-growing list of aggregation
   functions, data transformation operators, and privacy definitions.
 - … *robust*: it is built and maintained by a team of differential privacy
   experts, and runs in production at institutions like the U.S. Census Bureau.
 - … *scalable*: it runs on `Spark <http://spark.apache.org>`__, so it can scale
   to very large datasets.
 
-..
-    TODO(#2650): Add this back to the docs, removing the placeholder text.
-
-    For new users, `this Colab notebook <https://colab.research.google.com/drive/18J_UrHAKJf52RMRxi4OOpk59dV9tvKxO#offline=true&sandboxMode=true>`__ demonstrates basic features of the library without requiring a local installation.
-    To explore further or work on larger datasets, a good starting point is the :ref:`installation instructions <installation instructions>`.
+For new users, `this Colab notebook <https://colab.research.google.com/drive/18J_UrHAKJf52RMRxi4OOpk59dV9tvKxO#offline=true&sandboxMode=true>`__ demonstrates basic features of the library without requiring a local installation.
+To explore further or work on larger datasets, a good starting point is the :ref:`installation instructions <installation instructions>`.
 
 A good starting point is the :ref:`installation instructions <installation instructions>`.
 
 The Tumult Analytics documentation introduces all of the concepts necessary to get started producing differentially private results.
 Users who wish to learn more about the fundamentals of differential privacy can consult
 `this blog post series <https://desfontain.es/privacy/friendly-intro-to-differential-privacy.html>`__
 or `this longer introduction <https://privacytools.seas.harvard.edu/files/privacytools/files/pedagogical-document-dp_0.pdf>`__.
@@ -107,16 +104,15 @@
    which have huge text.
 
 Additional resources
 --------------------
 
 Contact us
 ^^^^^^^^^^
-The best place to ask questions, file feature requests, or give feedback about Tumult Analytics
-is our `Slack server <https://tmltdev.slack.com/join/shared_invite/zt-1bky0mh9v-vOB8azKAVoxmzJDUdWd5Wg#>`__.
+The best place to ask questions, file feature requests, or give feedback about Tumult Analytics is our `Slack server <https://tmlt.dev/slack>`__.
 We also use it for announcements of new releases and feature additions.
 
 Cite us
 ^^^^^^^
 
 If you use Tumult Analytics for a scientific publication, we would appreciate citations to the published software and/or its whitepaper.
 Both citations can be found below; for the software citation, please replace the version with the version you are using.
```

### Comparing `tmlt_analytics-0.7.1/doc/intersphinx_mapping.json` & `tmlt_analytics-0.7.2/doc/intersphinx_mapping.json`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/privacy-policy.rst` & `tmlt_analytics-0.7.2/doc/privacy-policy.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/templates/python/class.rst` & `tmlt_analytics-0.7.2/doc/templates/python/class.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/templates/python/module.rst` & `tmlt_analytics-0.7.2/doc/templates/python/module.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/topic-guides/nulls-nans-infinities.rst` & `tmlt_analytics-0.7.2/doc/topic-guides/nulls-nans-infinities.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/topic-guides/privacy-budgets.rst` & `tmlt_analytics-0.7.2/doc/topic-guides/privacy-budgets.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/topic-guides/privacy-promise.rst` & `tmlt_analytics-0.7.2/doc/topic-guides/privacy-promise.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/topic-guides/spark.rst` & `tmlt_analytics-0.7.2/doc/topic-guides/spark.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/topic-guides/understanding-sensitivity.rst` & `tmlt_analytics-0.7.2/doc/topic-guides/understanding-sensitivity.rst`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 each. The sensitivity computation is more complicated than before:
 
 :math:`\text{sensitivity} = (T_{left}  *  S_{right}  *  M_{right}) + (T_{right}  *  S_{left}  *  M_{left})`
 
 where:
 
   - :math:`T_{left}` and :math:`T_{right}` are the truncation thresholds, i.e. ``max_records``, for the left and right tables, respectively. When using :class:`DropNonUnique<tmlt.analytics.truncation_strategy.TruncationStrategy.DropNonUnique>`, these values are always 1.
-  - :math:`S_{left}` and :math:`S_{right}` are factors called the *stability* of each ``TruncationStrategy``. This value is always 2 for :class:`DropExcess<tmlt.analytics.truncation_strategy.TruncationStrategy.DropExcess>`, and 1 for :class:`DropNonUnique<tmlt.analytics.truncation_strategy.TruncationStrategy.DropNonUnique>`.
+  - :math:`S_{left}` and :math:`S_{right}` are factors called the *stability* of each ``TruncationStrategy``. These values are always 2 for :class:`DropExcess<tmlt.analytics.truncation_strategy.TruncationStrategy.DropExcess>` and 1 for :class:`DropNonUnique<tmlt.analytics.truncation_strategy.TruncationStrategy.DropNonUnique>`.
   - :math:`M_{left}` and :math:`M_{right}` are the ``max_rows`` parameters of the protected change on the left and right tables, respectively.
 
 
 In this example, if we choose a truncation strategy of ``DropExcess(max_records=2)`` for
 both tables, they will be truncated to include no more than two rows for each value of
 our join key, ``user_id``. The private join might look something like:
 
@@ -152,17 +152,21 @@
     When we know that a table always contains only one row per join key, it's preferable
     to use ``DropNonUnique``, due to the smaller truncation stability. In this case,
     using ``DropNonUnique`` for the Users table and ``DropExcess(max_records=2)`` for the
     Purchases table would have led to a join sensitivity of :math:`1 * 2 * 1 + 2 * 1 * 1 = 4`.
     Using ``DropExcess(max_records=1)`` for the users table would have led to a sensitivity of
     :math:`1 * 2 * 1 + 2 * 2 * 1 = 6` instead.
 
-As you can see, tracking stability can be complicated. When in doubt, you can use the
-:meth:`describe<tmlt.analytics.session.Session.describe>` method to see how stability evolves
-with transformations.
+As you can see, tracking stability can be complicated!
+
+..
+    TODO(#2696): Add this back in when describe() actually shows stability info.
+    When in doubt, you can use the
+    :meth:`describe<tmlt.analytics.session.Session.describe>` method to see how stability evolves
+    with transformations.
 
 Queries on tables using ``AddRowsWithID``
 -----------------------------------------
 
 Queries on tables using the
 :class:`AddRowsWithID<tmlt.analytics.protected_change.AddRowsWithID>` protected change
 protect the presence of arbitrarily many rows associated with the same privacy ID. In this case,
```

### Comparing `tmlt_analytics-0.7.1/doc/topic-guides/working-with-sessions.rst` & `tmlt_analytics-0.7.2/doc/topic-guides/working-with-sessions.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/tutorials/clamping-bounds.rst` & `tmlt_analytics-0.7.2/doc/tutorials/clamping-bounds.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/tutorials/first-steps.rst` & `tmlt_analytics-0.7.2/doc/tutorials/first-steps.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/tutorials/groupby-queries.rst` & `tmlt_analytics-0.7.2/doc/tutorials/groupby-queries.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/tutorials/more-with-privacy-ids.rst` & `tmlt_analytics-0.7.2/doc/tutorials/more-with-privacy-ids.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/doc/tutorials/privacy-budget-basics.rst` & `tmlt_analytics-0.7.2/doc/tutorials/privacy-budget-basics.rst`

 * *Files 2% similar despite different names*

```diff
@@ -226,16 +226,18 @@
        privacy_budget=PureDPBudget(epsilon=1),
    )
 
 .. testoutput::
    :options: +NORMALIZE_WHITESPACE
 
    Traceback (most recent call last):
-   RuntimeError: Cannot answer query without exceeding privacy budget: it needs
-   approximately 1.000, but the remaining budget is approximately 0.500 (difference: 5.000e-01)
+   RuntimeError: Cannot answer query without exceeding the Session privacy budget.
+   Requested: ε=1.000
+   Remaining: ε=0.500
+   Difference: ε=0.500
 
 The ``evaluate`` call returns an error. This is how the Session enforces its
 privacy promise: it makes sure that the queries cannot consume more than the
 initial privacy budget.
 
 Note that since the call to ``evaluate`` was rejected by the Session, it did not
 consume any privacy budget.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tmlt_analytics-0.7.1/doc/tutorials/privacy-id-basics.rst` & `tmlt_analytics-0.7.2/doc/tutorials/privacy-id-basics.rst`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,21 @@
     from tmlt.analytics.keyset import KeySet
     from tmlt.analytics.privacy_budget import PureDPBudget
     from tmlt.analytics.protected_change import AddRowsWithID
     from tmlt.analytics.query_builder import QueryBuilder
     from tmlt.analytics.session import Session
 
 ... and download two datasets: one containing books checked out from
-the library, and one that contains a list of the books that the library has.
+the library, and one that contains a list of the books that the library has. The checkout logs might look like:
+
+.. image:: ../images/mock_checkout_logs.svg
+   :alt: An 8x6 table demonstrating the checkout logs data structure. The columns of the table are checkout_date, member_id, title, author, isbn, publication_date, publisher, and genres. The rows of the table are the individual checkouts. The checkout_date column contains dates, the member_id column contains integers, the title, author, isbn, publication_date, publisher, and genres columns contain strings.
+   :align: center
+
+Notice that the *same member* may have checked out *many books*, as illustrated by the highlighted rows. This is a defining characteristic of data fit for use with privacy IDs, as we will see in a moment.
 
 .. testcode::
 
     spark = SparkSession.builder.getOrCreate()
     spark.sparkContext.addFile(
         "https://tumult-public.s3.amazonaws.com/checkout-logs.csv"
     )
@@ -352,11 +358,20 @@
 or using :class:`~tmlt.analytics.constraints.MaxGroupsPerID` and
 :class:`~tmlt.analytics.constraints.MaxRowsPerGroupPerID`.
 
 .. image:: ../images/flow_chart_truncation.svg
    :alt: A flow chart showing three paths from "data with privacy IDs" to "compute statistic". The first path is "data with privacy IDs" to "truncate using MaxRowsPerID" to "compute statistic". The second and third paths are paired together. The second path is "data with privacy IDs" to "truncate using MaxGroupsPerID" to "truncate using MaxRowsPerGroupPerID" to "compute statistic". The third path is "data with privacy IDs" to "truncate using MaxRowsPerGroupPerID" to "truncate using MaxGroupsPerID" to "compute statistic".
    :align: center
 
-To understand more the impact of choosing one kind of constraint vs. another,
+As a reminder:
+
+* :class:`~tmlt.analytics.constraints.MaxRowsPerID` limits the number of rows
+  associated with each privacy ID in a table.
+* :class:`~tmlt.analytics.constraints.MaxGroupsPerID` limits the number of distinct
+  values of the grouping column that may appear for each privacy ID in a table.
+* :class:`~tmlt.analytics.constraints.MaxRowsPerGroupPerID` limits the number of rows
+  associated with each (privacy ID, grouping column value) pair in a table.
+
+To understand the impact of the various constraints in more detail,
 you can consult our :ref:`topic guide about sensitivity<Understanding sensitivity>`.
 To learn more about how to perform more complex queries on tables initialized with
 privacy IDs, you can proceed to the :ref:`next tutorial<Advanced IDs features>`.
```

### Comparing `tmlt_analytics-0.7.1/doc/tutorials/simple-transformations.rst` & `tmlt_analytics-0.7.2/doc/tutorials/simple-transformations.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/examples/interactive_evaluation.ipynb` & `tmlt_analytics-0.7.2/examples/interactive_evaluation.ipynb`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/examples/private_join.ipynb` & `tmlt_analytics-0.7.2/examples/private_join.ipynb`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/examples/zcdp_puredp_switching.ipynb` & `tmlt_analytics-0.7.2/examples/zcdp_puredp_switching.ipynb`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/pyproject.toml` & `tmlt_analytics-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 readme = "README.md"
 authors = []
 license = "Apache-2.0"
 homepage = "https://www.tmlt.dev/"
 repository = "https://gitlab.com/tumult-labs/analytics"
 documentation = "https://docs.tmlt.dev/analytics/latest"
 # The version field is required in this file format, even though it's ignored because of poetry-dynamic-versioning.
-version = "0.7.1"
+version = "0.7.2"
 
 classifiers = [
    "Development Status :: 4 - Beta",
    "Intended Audience :: Developers",
    "Intended Audience :: Education",
    "Intended Audience :: Science/Research",
    "Natural Language :: English",
@@ -32,20 +32,20 @@
 ]
 packages = [
   { include = "tmlt" },
 ]
 
 
 [tool.poetry.dependencies]
-python = "^3.7.1, <3.10.0"
+python = "^3.7.1, <3.11.0"
 
 # When updating Core, PySpark, Pandas or SymPy, remember to update
 # test_multi_deps in the Noxfile.
 
-"tmlt.core" = "^0.9.0"
+"tmlt.core" = "^0.10.1"
 
 pandas = "^1.2.0"
 pyspark = { version = "^3.0.0,<=3.3.1", extras = ["sql"] }
 sympy = "^1.8,<1.10"
 typeguard = "^2.12.1,<2.13.0"
 typing-extensions = "^3.10.0"
```

### Comparing `tmlt_analytics-0.7.1/test/conftest.py` & `tmlt_analytics-0.7.2/test/conftest.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/system/session/conftest.py` & `tmlt_analytics-0.7.2/test/system/session/conftest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Common fixtures for Session integration tests."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
 
 import pandas as pd
 import pytest
-from pyspark.sql.types import LongType, StringType, StructField, StructType
+from pyspark.sql.types import IntegerType, LongType, StringType, StructField, StructType
 
 from tmlt.analytics.privacy_budget import PrivacyBudget, PureDPBudget, RhoZCDPBudget
 from tmlt.analytics.protected_change import AddMaxRows, AddRowsWithID
 from tmlt.analytics.session import Session
 
 INF_BUDGET = PureDPBudget(float("inf"))
 INF_BUDGET_ZCDP = RhoZCDPBudget(float("inf"))
@@ -62,25 +62,67 @@
                 [2, "B", 21],
                 [3, "A", 24],
                 [3, "B", 27],
             ],
             columns=["id", "group", "x"],
         )
     )
+    df_id3 = spark.createDataFrame(
+        [
+            [1, "A", 12],
+            [None, "B", 15],
+            [1, "A", 18],
+            [2, "B", None],
+            [3, "A", 24],
+            [3, "B", 27],
+            [None, "A", 30],
+        ],
+        schema=StructType(
+            [
+                StructField("id", IntegerType(), nullable=True),
+                StructField("group", StringType(), nullable=False),
+                StructField("x", LongType(), nullable=True),
+            ]
+        ),
+    )
+    # df with non-nullable id column
+    df_id4 = spark.createDataFrame(
+        [
+            [1, "A", 12],
+            [1, "B", 15],
+            [1, "A", 18],
+            [2, "B", 21],
+            [3, "A", 24],
+            [3, "B", 27],
+        ],
+        schema=StructType(
+            [
+                StructField("id", IntegerType(), nullable=False),
+                StructField("group", StringType(), nullable=False),
+                StructField("x", LongType(), nullable=False),
+            ]
+        ),
+    )
     df_rows1 = spark.createDataFrame(
         [["0", 0, 0], ["0", 0, 1], ["0", 1, 2], ["1", 0, 3]],
         schema=StructType(
             [
                 StructField("A", StringType(), nullable=False),
                 StructField("B", LongType(), nullable=False),
                 StructField("X", LongType(), nullable=False),
             ]
         ),
     )
-    return {"id1": df_id1, "id2": df_id2, "rows1": df_rows1}
+    return {
+        "id1": df_id1,
+        "id2": df_id2,
+        "id3": df_id3,
+        "id4": df_id4,
+        "rows1": df_rows1,
+    }
 
 
 @pytest.fixture
 def session(_session_data, request):
     """A Session with some sample data.
 
     This fixture requires a parameter (typically passed by setting the
@@ -107,14 +149,20 @@
         .with_private_dataframe(
             "id_a1", _session_data["id1"], protected_change=AddRowsWithID("id", "a")
         )
         .with_private_dataframe(
             "id_a2", _session_data["id2"], protected_change=AddRowsWithID("id", "a")
         )
         .with_private_dataframe(
+            "id_a3", _session_data["id3"], protected_change=AddRowsWithID("id", "a")
+        )
+        .with_private_dataframe(
+            "id_a4", _session_data["id4"], protected_change=AddRowsWithID("id", "a")
+        )
+        .with_private_dataframe(
             "id_b1", _session_data["id1"], protected_change=AddRowsWithID("id", "b")
         )
         .with_private_dataframe(
             "id_b2", _session_data["id1"], protected_change=AddRowsWithID("id", "b")
         )
         .with_private_dataframe(
             "rows_1", _session_data["rows1"], protected_change=AddMaxRows(2)
```

### Comparing `tmlt_analytics-0.7.1/test/system/session/ids/test_constraint_propagation.py` & `tmlt_analytics-0.7.2/test/system/session/ids/test_constraint_propagation.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/system/session/ids/test_count_distinct_optimization.py` & `tmlt_analytics-0.7.2/test/system/session/ids/test_count_distinct_optimization.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/system/session/ids/test_l0_linf_truncation.py` & `tmlt_analytics-0.7.2/test/system/session/ids/test_l0_linf_truncation.py`

 * *Files 2% similar despite different names*

```diff
@@ -463,14 +463,29 @@
             QueryBuilder("id_a1")
             .enforce(MaxGroupsPerID("group", 2))
             .enforce(MaxRowsPerGroupPerID("group", 3))
             .groupby(_KEYSET)
             .average("n", 0, 10),
             [450, 18],
         ),
+        (
+            QueryBuilder("id_a1")
+            .enforce(MaxGroupsPerID("group", 2))
+            .enforce(MaxRowsPerGroupPerID("group", 3))
+            .average("float_n", 0, 10),
+            [900, 36],
+        ),
+        (
+            QueryBuilder("id_a1")
+            .enforce(MaxGroupsPerID("group", 2))
+            .enforce(MaxRowsPerGroupPerID("group", 3))
+            .groupby(_KEYSET)
+            .average("float_n", 0, 10),
+            [450, 18],
+        ),
     ],
 )
 def test_noise_scale_zcdp(query: QueryExpr, expected_noise: List[float], session):
     """Noise scales are adjusted correctly for different truncations with zCDP."""
     # pylint: disable=protected-access
     noise_info = session._noise_info(query, RhoZCDPBudget(1))
     # pylint: enable=protected-access
```

### Comparing `tmlt_analytics-0.7.1/test/system/session/ids/test_l1_truncation.py` & `tmlt_analytics-0.7.2/test/system/session/ids/test_l1_truncation.py`

 * *Files 2% similar despite different names*

```diff
@@ -321,14 +321,22 @@
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(1)).average("n", 0, 10), [25, 1]),
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(5)).average("n", 0, 10), [625, 25]),
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(1)).average("n", 0, 20), [100, 1]),
         (
             QueryBuilder("id_a1").enforce(MaxRowsPerID(5)).average("n", 0, 20),
             [2500, 25],
         ),
+        (
+            QueryBuilder("id_a1").enforce(MaxRowsPerID(1)).average("float_n", 0, 20),
+            [100, 1],
+        ),
+        (
+            QueryBuilder("id_a1").enforce(MaxRowsPerID(5)).average("float_n", 0, 20),
+            [2500, 25],
+        ),
     ],
 )
 def test_noise_scale_zcdp(query: QueryExpr, expected_noise: List[float], session):
     """Noise scales are adjusted correctly for different truncations with zCDP."""
     # pylint: disable=protected-access
     noise_info = session._noise_info(query, RhoZCDPBudget(1))
     # pylint: enable=protected-access
```

### Comparing `tmlt_analytics-0.7.1/test/system/session/ids/test_partition.py` & `tmlt_analytics-0.7.2/test/system/session/ids/test_partition.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/system/session/mixed/test_mixed_session.py` & `tmlt_analytics-0.7.2/test/system/session/mixed/test_mixed_session.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/system/session/rows/conftest.py` & `tmlt_analytics-0.7.2/test/system/session/rows/conftest.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/system/session/rows/test_add_max_rows.py` & `tmlt_analytics-0.7.2/test/system/session/rows/test_add_max_rows.py`

 * *Files 2% similar despite different names*

```diff
@@ -425,15 +425,15 @@
         actual = session.evaluate(sum_query, privacy_budget)
         assert_frame_equal_with_sort(actual.toPandas(), expected, rtol=1)
 
     @pytest.mark.parametrize(
         "starting_budget,partition_budget",
         [
             (PureDPBudget(20), PureDPBudget(10)),
-            (ApproxDPBudget(20, 0.5), ApproxDPBudget(10, 0)),
+            (ApproxDPBudget(20, 1 / 2), ApproxDPBudget(10, 1 / 4)),
             (RhoZCDPBudget(20), RhoZCDPBudget(10)),
         ],
     )
     def test_partition_and_create(
         self, starting_budget: PrivacyBudget, partition_budget: PrivacyBudget
     ):
         """Tests using :func:`partition_and_create` to create a new session."""
@@ -460,24 +460,45 @@
         )
         assert session3.remaining_privacy_budget == partition_budget
         assert session3.private_sources == ["private1"]
         assert session3.get_schema("private1") == Schema(
             {"A": ColumnType.VARCHAR, "B": ColumnType.INTEGER, "X": ColumnType.INTEGER}
         )
 
+    def test_partition_nonexistent_table(self):
+        """Partitioning on a nonexistent table works correctly."""
+        sess = Session.from_dataframe(
+            PureDPBudget(1), "private", self.sdf, protected_change=AddOneRow()
+        )
+        sess.add_public_dataframe("public", self.sdf)
+
+        with pytest.raises(KeyError, match="Private table '.*' does not exist"):
+            sess.partition_and_create(
+                "nonexistent", PureDPBudget(1), "A", {"private0": "0"}
+            )
+        with pytest.raises(ValueError, match="Table '.*' is a public table"):
+            sess.partition_and_create("public", PureDPBudget(1), "A", {"private0": "0"})
+
     @pytest.mark.parametrize(
-        "starting_budget,partition_budget",
+        "starting_budget,partition_budget,remaining_budget",
         [
-            (PureDPBudget(20), PureDPBudget(10)),
-            (ApproxDPBudget(20, 0.5), ApproxDPBudget(10, 0)),
-            (RhoZCDPBudget(20), RhoZCDPBudget(10)),
+            (PureDPBudget(20), PureDPBudget(12), PureDPBudget(8)),
+            (
+                ApproxDPBudget(20, 1 / 4),
+                ApproxDPBudget(12, 3 / 16),
+                ApproxDPBudget(8, 1 / 16),
+            ),
+            (RhoZCDPBudget(20), RhoZCDPBudget(12), RhoZCDPBudget(8)),
         ],
     )
     def test_partition_and_create_query(
-        self, starting_budget: PrivacyBudget, partition_budget: PrivacyBudget
+        self,
+        starting_budget: PrivacyBudget,
+        partition_budget: PrivacyBudget,
+        remaining_budget: PrivacyBudget,
     ):
         """Querying on a partitioned session with stability>1 works."""
         session1 = Session.from_dataframe(
             privacy_budget=starting_budget,
             source_id="private",
             dataframe=self.sdf,
             protected_change=AddOneRow(),
@@ -496,15 +517,15 @@
         session1.create_view(transformation_query, "flatmap", True)
 
         sessions = session1.partition_and_create(
             "flatmap", partition_budget, "A", splits={"private0": "0", "private1": "1"}
         )
         session2 = sessions["private0"]
         session3 = sessions["private1"]
-        assert session1.remaining_privacy_budget == partition_budget
+        assert session1.remaining_privacy_budget == remaining_budget
         assert session2.remaining_privacy_budget == partition_budget
         assert session2.private_sources == ["private0"]
         assert session2.get_schema("private0") == Schema(
             {"A": ColumnType.VARCHAR, "B": ColumnType.INTEGER, "X": ColumnType.INTEGER}
         )
         assert session3.remaining_privacy_budget == partition_budget
         assert session3.private_sources == ["private1"]
@@ -513,28 +534,33 @@
         )
         query = GroupByCount(
             child=PrivateSource("private0"), groupby_keys=KeySet.from_dict({})
         )
         session2.evaluate(query, partition_budget)
 
     @pytest.mark.parametrize(
-        "starting_budget,partition_budget",
-        [(ApproxDPBudget(20, 0.5), PureDPBudget(10))],
+        "starting_budget,partition_budget,remaining_budget",
+        [(ApproxDPBudget(20, 0.5), PureDPBudget(10), ApproxDPBudget(10, 0.5))],
     )
     def test_partition_and_create_approxDP_session_pureDP_partition(
-        self, starting_budget: PrivacyBudget, partition_budget: PrivacyBudget
+        self,
+        starting_budget: PrivacyBudget,
+        partition_budget: PrivacyBudget,
+        remaining_budget: PrivacyBudget,
     ):
         """Tests using :func:`partition_and_create` to create a new ApproxDP session
         that supports PureDP partitions."""
 
         is_approxDP_starting_budget = isinstance(starting_budget, ApproxDPBudget)
         if is_approxDP_starting_budget and isinstance(partition_budget, PureDPBudget):
-            partition_budget = ApproxDPBudget(partition_budget.epsilon, 0)
+            partition_budget = ApproxDPBudget(partition_budget.value, 0)
 
-        self.test_partition_and_create_query(starting_budget, partition_budget)
+        self.test_partition_and_create_query(
+            starting_budget, partition_budget, remaining_budget
+        )
 
     @pytest.mark.parametrize(
         "inf_budget,mechanism",
         [
             (PureDPBudget(float("inf")), CountMechanism.LAPLACE),
             (ApproxDPBudget(float("inf"), 0.5), CountMechanism.LAPLACE),
             (RhoZCDPBudget(float("inf")), CountMechanism.LAPLACE),
@@ -580,40 +606,45 @@
         )
 
     @pytest.mark.parametrize("output_measure", [(PureDP()), (ApproxDP()), (RhoZCDP())])
     def test_partitions_composed(
         self, output_measure: Union[PureDP, ApproxDP, RhoZCDP]
     ):
         """Smoke test for composing :func:`partition_and_create`."""
-        starting_budget: Union[PureDPBudget, ApproxDPBudget, RhoZCDPBudget]
-        partition_budget: Union[PureDPBudget, ApproxDPBudget, RhoZCDPBudget]
-        second_partition_budget: Union[PureDPBudget, ApproxDPBudget, RhoZCDPBudget]
-        final_evaluate_budget: Union[PureDPBudget, ApproxDPBudget, RhoZCDPBudget]
+        root_session_budget: PrivacyBudget
+        root_session_remaining_budget: PrivacyBudget
+        column_A_partition_budget: PrivacyBudget
+        column_A_remaining_budget: PrivacyBudget
+        column_B_partition_budget: PrivacyBudget
+
         if output_measure == PureDP():
-            starting_budget = PureDPBudget(20)
-            partition_budget = PureDPBudget(10)
-            second_partition_budget = PureDPBudget(5)
-            final_evaluate_budget = PureDPBudget(2)
+            root_session_budget = PureDPBudget(20)
+            root_session_remaining_budget = PureDPBudget(8)
+            column_A_partition_budget = PureDPBudget(12)
+            column_A_remaining_budget = PureDPBudget(7)
+            column_B_partition_budget = PureDPBudget(5)
         elif output_measure == ApproxDP():
-            starting_budget = ApproxDPBudget(20, 0)
-            partition_budget = ApproxDPBudget(10, 0)
-            second_partition_budget = ApproxDPBudget(5, 0)
-            final_evaluate_budget = ApproxDPBudget(2, 0)
+            root_session_budget = ApproxDPBudget(20, 1 / 4)
+            root_session_remaining_budget = ApproxDPBudget(8, 3 / 16)
+            column_A_partition_budget = ApproxDPBudget(12, 1 / 16)
+            column_A_remaining_budget = ApproxDPBudget(7, 3 / 64)
+            column_B_partition_budget = ApproxDPBudget(5, 1 / 64)
         elif output_measure == RhoZCDP():
-            starting_budget = RhoZCDPBudget(20)
-            partition_budget = RhoZCDPBudget(10)
-            second_partition_budget = RhoZCDPBudget(5)
-            final_evaluate_budget = RhoZCDPBudget(2)
+            root_session_budget = RhoZCDPBudget(20)
+            root_session_remaining_budget = RhoZCDPBudget(8)
+            column_A_partition_budget = RhoZCDPBudget(12)
+            column_A_remaining_budget = RhoZCDPBudget(7)
+            column_B_partition_budget = RhoZCDPBudget(5)
         else:
             pytest.fail(
                 f"must use PureDP, ApproxDP, or RhoZCDP, found {output_measure}"
             )
 
-        session1 = Session.from_dataframe(
-            privacy_budget=starting_budget,
+        root_session = Session.from_dataframe(
+            privacy_budget=root_session_budget,
             source_id="private",
             dataframe=self.sdf,
             protected_change=AddOneRow(),
         )
 
         transformation_query1 = ReplaceNullAndNan(
             replace_with={},
@@ -621,78 +652,73 @@
                 child=PrivateSource("private"),
                 f=lambda row: [{}, {}],
                 schema_new_columns=Schema({}),
                 augment=True,
                 max_num_rows=2,
             ),
         )
-        session1.create_view(transformation_query1, "transform1", cache=False)
+        root_session.create_view(transformation_query1, "transform1", cache=False)
 
-        sessions = session1.partition_and_create(
+        first_partition_sessions = root_session.partition_and_create(
             "transform1",
-            partition_budget,
+            column_A_partition_budget,
             "A",
             splits={"private0": "0", "private1": "1"},
         )
-        session2 = sessions["private0"]
-        session3 = sessions["private1"]
-        assert session1.remaining_privacy_budget == partition_budget
-        assert session2.remaining_privacy_budget == partition_budget
-        assert session2.private_sources == ["private0"]
-        assert session2.get_schema("private0") == Schema(
+        sessionA0 = first_partition_sessions["private0"]
+        sessionA1 = first_partition_sessions["private1"]
+        assert root_session.remaining_privacy_budget == root_session_remaining_budget
+        assert sessionA0.remaining_privacy_budget == column_A_partition_budget
+        assert sessionA0.private_sources == ["private0"]
+        assert sessionA0.get_schema("private0") == Schema(
             {"A": ColumnType.VARCHAR, "B": ColumnType.INTEGER, "X": ColumnType.INTEGER}
         )
-        assert session3.remaining_privacy_budget == partition_budget
-        assert session3.private_sources == ["private1"]
-        assert session3.get_schema("private1") == Schema(
+        assert sessionA1.remaining_privacy_budget == column_A_partition_budget
+        assert sessionA1.private_sources == ["private1"]
+        assert sessionA1.get_schema("private1") == Schema(
             {"A": ColumnType.VARCHAR, "B": ColumnType.INTEGER, "X": ColumnType.INTEGER}
         )
 
         transformation_query2 = ReplaceNullAndNan(
             replace_with={},
             child=FlatMap(
                 child=PrivateSource("private0"),
                 f=lambda row: [{}, {}, {}],
                 schema_new_columns=Schema({}),
                 augment=True,
                 max_num_rows=2,
             ),
         )
-        session2.create_view(transformation_query2, "transform2", cache=False)
+        sessionA0.create_view(transformation_query2, "transform2", cache=False)
 
-        sessions = session2.partition_and_create(
+        second_parition_sessions = sessionA0.partition_and_create(
             "transform2",
-            second_partition_budget,
-            "A",
-            splits={"private0": "0", "private1": "1"},
-        )
-        session4 = sessions["private0"]
-        session5 = sessions["private1"]
-        assert session2.remaining_privacy_budget == second_partition_budget
-        assert session4.remaining_privacy_budget == second_partition_budget
-        assert session4.private_sources == ["private0"]
-        assert session4.get_schema("private0") == Schema(
+            column_B_partition_budget,
+            "B",
+            splits={"private0": 0, "private1": 1},
+        )
+        sessionA0B0 = second_parition_sessions["private0"]
+        sessionA0B1 = second_parition_sessions["private1"]
+        assert sessionA0.remaining_privacy_budget == column_A_remaining_budget
+        assert sessionA0B0.remaining_privacy_budget == column_B_partition_budget
+        assert sessionA0B0.private_sources == ["private0"]
+        assert sessionA0B0.get_schema("private0") == Schema(
             {"A": ColumnType.VARCHAR, "B": ColumnType.INTEGER, "X": ColumnType.INTEGER}
         )
-        assert session5.remaining_privacy_budget == second_partition_budget
-        assert session5.private_sources == ["private1"]
-        assert session5.get_schema("private1") == Schema(
+        assert sessionA0B1.remaining_privacy_budget == column_B_partition_budget
+        assert sessionA0B1.private_sources == ["private1"]
+        assert sessionA0B1.get_schema("private1") == Schema(
             {"A": ColumnType.VARCHAR, "B": ColumnType.INTEGER, "X": ColumnType.INTEGER}
         )
 
-        query = GroupByCount(
-            child=PrivateSource("private0"), groupby_keys=KeySet.from_dict({})
-        )
-        session4.evaluate(query_expr=query, privacy_budget=final_evaluate_budget)
-
     @pytest.mark.parametrize(
         "starting_budget,partition_budget",
         [
             (PureDPBudget(20), PureDPBudget(10)),
-            (ApproxDPBudget(20, 0.5), ApproxDPBudget(10, 0)),
+            (ApproxDPBudget(20, 1 / 2), ApproxDPBudget(10, 1 / 4)),
             (RhoZCDPBudget(20), RhoZCDPBudget(10)),
         ],
     )
     def test_partition_execution_order(
         self, starting_budget: PrivacyBudget, partition_budget: PrivacyBudget
     ):
         """Tests behavior using :func:`partition_and_create` sessions out of order."""
```

### Comparing `tmlt_analytics-0.7.1/test/system/session/rows/test_add_max_rows_in_max_groups.py` & `tmlt_analytics-0.7.2/test/system/session/rows/test_add_max_rows_in_max_groups.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/system/session/rows/test_add_max_rows_infs_nulls.py` & `tmlt_analytics-0.7.2/test/system/session/rows/test_add_max_rows_infs_nulls.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/system/session/test_budgets.py` & `tmlt_analytics-0.7.2/test/system/session/test_budgets.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/system/session/test_invalid_constraints.py` & `tmlt_analytics-0.7.2/test/system/session/test_invalid_constraints.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/unit/query_expr_compiler/test_measurement_visitor.py` & `tmlt_analytics-0.7.2/test/unit/query_expr_compiler/test_measurement_visitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,20 @@
             ),
             (
                 AverageMechanism.DEFAULT,
                 RhoZCDP(),
                 SparkIntegerColumnDescriptor(),
                 NoiseMechanism.DISCRETE_GAUSSIAN,
             ),
-            (AverageMechanism.DEFAULT, RhoZCDP(), SparkFloatColumnDescriptor(), None),
+            (
+                AverageMechanism.DEFAULT,
+                RhoZCDP(),
+                SparkFloatColumnDescriptor(),
+                NoiseMechanism.GAUSSIAN,
+            ),
             (
                 AverageMechanism.LAPLACE,
                 PureDP(),
                 SparkIntegerColumnDescriptor(),
                 NoiseMechanism.GEOMETRIC,
             ),
             (
@@ -430,28 +435,28 @@
             ),
             (
                 AverageMechanism.LAPLACE,
                 RhoZCDP(),
                 SparkFloatColumnDescriptor(),
                 NoiseMechanism.LAPLACE,
             ),
+            (AverageMechanism.GAUSSIAN, PureDP(), SparkIntegerColumnDescriptor(), None),
+            (AverageMechanism.GAUSSIAN, PureDP(), SparkFloatColumnDescriptor(), None),
             (
                 AverageMechanism.GAUSSIAN,
-                PureDP(),
+                RhoZCDP(),
                 SparkIntegerColumnDescriptor(),
                 NoiseMechanism.DISCRETE_GAUSSIAN,
             ),
-            (AverageMechanism.GAUSSIAN, PureDP(), SparkFloatColumnDescriptor(), None),
             (
                 AverageMechanism.GAUSSIAN,
                 RhoZCDP(),
-                SparkIntegerColumnDescriptor(),
-                NoiseMechanism.DISCRETE_GAUSSIAN,
+                SparkFloatColumnDescriptor(),
+                NoiseMechanism.GAUSSIAN,
             ),
-            (AverageMechanism.GAUSSIAN, RhoZCDP(), SparkFloatColumnDescriptor(), None),
         ],
     )
     def test_pick_noise_for_average(
         self,
         query_mechanism: AverageMechanism,
         output_measure: Union[PureDP, RhoZCDP],
         measure_column_type: SparkColumnDescriptor,
@@ -471,15 +476,21 @@
         # pylint: disable=protected-access
         if expected_mechanism is not None:
             got_mechanism = self.pick_noise_visitor._pick_noise_for_non_count(
                 query, measure_column_type
             )
             assert got_mechanism == expected_mechanism
         else:
-            with pytest.raises(NotImplementedError):
+            with pytest.raises(
+                ValueError,
+                match=(
+                    "Gaussian noise is not supported under PureDP. "
+                    "Please use RhoZCDP or another measure."
+                ),
+            ):
                 self.pick_noise_visitor._pick_noise_for_non_count(
                     query, measure_column_type
                 )
         # pylint: enable=protected-access
 
     @pytest.mark.parametrize(
         "query_mechanism,output_measure,measure_column_type,expected_mechanism",
@@ -498,15 +509,20 @@
             ),
             (
                 SumMechanism.DEFAULT,
                 RhoZCDP(),
                 SparkIntegerColumnDescriptor(),
                 NoiseMechanism.DISCRETE_GAUSSIAN,
             ),
-            (SumMechanism.DEFAULT, RhoZCDP(), SparkFloatColumnDescriptor(), None),
+            (
+                SumMechanism.DEFAULT,
+                RhoZCDP(),
+                SparkFloatColumnDescriptor(),
+                NoiseMechanism.GAUSSIAN,
+            ),
             (
                 SumMechanism.LAPLACE,
                 PureDP(),
                 SparkIntegerColumnDescriptor(),
                 NoiseMechanism.GEOMETRIC,
             ),
             (
@@ -523,28 +539,28 @@
             ),
             (
                 SumMechanism.LAPLACE,
                 RhoZCDP(),
                 SparkFloatColumnDescriptor(),
                 NoiseMechanism.LAPLACE,
             ),
+            (SumMechanism.GAUSSIAN, PureDP(), SparkIntegerColumnDescriptor(), None),
+            (SumMechanism.GAUSSIAN, PureDP(), SparkFloatColumnDescriptor(), None),
             (
                 SumMechanism.GAUSSIAN,
-                PureDP(),
+                RhoZCDP(),
                 SparkIntegerColumnDescriptor(),
                 NoiseMechanism.DISCRETE_GAUSSIAN,
             ),
-            (SumMechanism.GAUSSIAN, PureDP(), SparkFloatColumnDescriptor(), None),
             (
                 SumMechanism.GAUSSIAN,
                 RhoZCDP(),
-                SparkIntegerColumnDescriptor(),
-                NoiseMechanism.DISCRETE_GAUSSIAN,
+                SparkFloatColumnDescriptor(),
+                NoiseMechanism.GAUSSIAN,
             ),
-            (SumMechanism.GAUSSIAN, RhoZCDP(), SparkFloatColumnDescriptor(), None),
         ],
     )
     def test_pick_noise_for_sum(
         self,
         query_mechanism: SumMechanism,
         output_measure: Union[PureDP, RhoZCDP],
         measure_column_type: SparkColumnDescriptor,
@@ -564,15 +580,21 @@
         # pylint: disable=protected-access
         if expected_mechanism is not None:
             got_mechanism = self.pick_noise_visitor._pick_noise_for_non_count(
                 query, measure_column_type
             )
             assert got_mechanism == expected_mechanism
         else:
-            with pytest.raises(NotImplementedError):
+            with pytest.raises(
+                ValueError,
+                match=(
+                    "Gaussian noise is not supported under PureDP. "
+                    "Please use RhoZCDP or another measure."
+                ),
+            ):
                 self.pick_noise_visitor._pick_noise_for_non_count(
                     query, measure_column_type
                 )
         # pylint: enable=protected-access
 
     @pytest.mark.parametrize(
         "query_mechanism,output_measure,measure_column_type,expected_mechanism",
@@ -591,15 +613,20 @@
             ),
             (
                 VarianceMechanism.DEFAULT,
                 RhoZCDP(),
                 SparkIntegerColumnDescriptor(),
                 NoiseMechanism.DISCRETE_GAUSSIAN,
             ),
-            (VarianceMechanism.DEFAULT, RhoZCDP(), SparkFloatColumnDescriptor(), None),
+            (
+                VarianceMechanism.DEFAULT,
+                RhoZCDP(),
+                SparkFloatColumnDescriptor(),
+                NoiseMechanism.GAUSSIAN,
+            ),
             (
                 VarianceMechanism.LAPLACE,
                 PureDP(),
                 SparkIntegerColumnDescriptor(),
                 NoiseMechanism.GEOMETRIC,
             ),
             (
@@ -620,24 +647,29 @@
                 SparkFloatColumnDescriptor(),
                 NoiseMechanism.LAPLACE,
             ),
             (
                 VarianceMechanism.GAUSSIAN,
                 PureDP(),
                 SparkIntegerColumnDescriptor(),
-                NoiseMechanism.DISCRETE_GAUSSIAN,
+                None,
             ),
             (VarianceMechanism.GAUSSIAN, PureDP(), SparkFloatColumnDescriptor(), None),
             (
                 VarianceMechanism.GAUSSIAN,
                 RhoZCDP(),
                 SparkIntegerColumnDescriptor(),
                 NoiseMechanism.DISCRETE_GAUSSIAN,
             ),
-            (VarianceMechanism.GAUSSIAN, RhoZCDP(), SparkFloatColumnDescriptor(), None),
+            (
+                VarianceMechanism.GAUSSIAN,
+                RhoZCDP(),
+                SparkFloatColumnDescriptor(),
+                NoiseMechanism.GAUSSIAN,
+            ),
         ],
     )
     def test_pick_noise_for_variance(
         self,
         query_mechanism: VarianceMechanism,
         output_measure: Union[PureDP, RhoZCDP],
         measure_column_type: SparkColumnDescriptor,
@@ -657,15 +689,21 @@
         # pylint: disable=protected-access
         if expected_mechanism is not None:
             got_mechanism = self.pick_noise_visitor._pick_noise_for_non_count(
                 query, measure_column_type
             )
             assert got_mechanism == expected_mechanism
         else:
-            with pytest.raises(NotImplementedError):
+            with pytest.raises(
+                ValueError,
+                match=(
+                    "Gaussian noise is not supported under PureDP. "
+                    "Please use RhoZCDP or another measure."
+                ),
+            ):
                 self.pick_noise_visitor._pick_noise_for_non_count(
                     query, measure_column_type
                 )
         # pylint: enable=protected-access
 
     @pytest.mark.parametrize(
         "query_mechanism,output_measure,measure_column_type,expected_mechanism",
@@ -684,15 +722,20 @@
             ),
             (
                 StdevMechanism.DEFAULT,
                 RhoZCDP(),
                 SparkIntegerColumnDescriptor(),
                 NoiseMechanism.DISCRETE_GAUSSIAN,
             ),
-            (StdevMechanism.DEFAULT, RhoZCDP(), SparkFloatColumnDescriptor(), None),
+            (
+                StdevMechanism.DEFAULT,
+                RhoZCDP(),
+                SparkFloatColumnDescriptor(),
+                NoiseMechanism.GAUSSIAN,
+            ),
             (
                 StdevMechanism.LAPLACE,
                 PureDP(),
                 SparkIntegerColumnDescriptor(),
                 NoiseMechanism.GEOMETRIC,
             ),
             (
@@ -709,28 +752,28 @@
             ),
             (
                 StdevMechanism.LAPLACE,
                 RhoZCDP(),
                 SparkFloatColumnDescriptor(),
                 NoiseMechanism.LAPLACE,
             ),
+            (StdevMechanism.GAUSSIAN, PureDP(), SparkIntegerColumnDescriptor(), None),
+            (StdevMechanism.GAUSSIAN, PureDP(), SparkFloatColumnDescriptor(), None),
             (
                 StdevMechanism.GAUSSIAN,
-                PureDP(),
+                RhoZCDP(),
                 SparkIntegerColumnDescriptor(),
                 NoiseMechanism.DISCRETE_GAUSSIAN,
             ),
-            (StdevMechanism.GAUSSIAN, PureDP(), SparkFloatColumnDescriptor(), None),
             (
                 StdevMechanism.GAUSSIAN,
                 RhoZCDP(),
-                SparkIntegerColumnDescriptor(),
-                NoiseMechanism.DISCRETE_GAUSSIAN,
+                SparkFloatColumnDescriptor(),
+                NoiseMechanism.GAUSSIAN,
             ),
-            (StdevMechanism.GAUSSIAN, RhoZCDP(), SparkFloatColumnDescriptor(), None),
         ],
     )
     def test_pick_noise_for_stdev(
         self,
         query_mechanism: StdevMechanism,
         output_measure: Union[PureDP, RhoZCDP],
         measure_column_type: SparkColumnDescriptor,
@@ -750,15 +793,21 @@
         # pylint: disable=protected-access
         if expected_mechanism is not None:
             got_mechanism = self.pick_noise_visitor._pick_noise_for_non_count(
                 query, measure_column_type
             )
             assert got_mechanism == expected_mechanism
         else:
-            with pytest.raises(NotImplementedError):
+            with pytest.raises(
+                ValueError,
+                match=(
+                    "Gaussian noise is not supported under PureDP. "
+                    "Please use RhoZCDP or another measure."
+                ),
+            ):
                 self.pick_noise_visitor._pick_noise_for_non_count(
                     query, measure_column_type
                 )
         # pylint: enable=protected-access
 
     @pytest.mark.parametrize(
         "mechanism",
@@ -837,14 +886,19 @@
             (HammingDistance(), NoiseMechanism.GEOMETRIC, SumOf(SymmetricDifference())),
             (
                 HammingDistance(),
                 NoiseMechanism.DISCRETE_GAUSSIAN,
                 RootSumOfSquared(SymmetricDifference()),
             ),
             (
+                HammingDistance(),
+                NoiseMechanism.GAUSSIAN,
+                RootSumOfSquared(SymmetricDifference()),
+            ),
+            (
                 SymmetricDifference(),
                 NoiseMechanism.LAPLACE,
                 SumOf(SymmetricDifference()),
             ),
             (
                 SymmetricDifference(),
                 NoiseMechanism.GEOMETRIC,
@@ -852,14 +906,19 @@
             ),
             (
                 SymmetricDifference(),
                 NoiseMechanism.DISCRETE_GAUSSIAN,
                 RootSumOfSquared(SymmetricDifference()),
             ),
             (
+                SymmetricDifference(),
+                NoiseMechanism.GAUSSIAN,
+                RootSumOfSquared(SymmetricDifference()),
+            ),
+            (
                 IfGroupedBy(column="A", inner_metric=SumOf(SymmetricDifference())),
                 NoiseMechanism.LAPLACE,
                 SumOf(SymmetricDifference()),
             ),
             (
                 IfGroupedBy(column="A", inner_metric=SumOf(SymmetricDifference())),
                 NoiseMechanism.GEOMETRIC,
@@ -966,18 +1025,18 @@
             (
                 GroupByBoundedVariance(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["zero", "one"]}),
                     measure_column="B",
                     low=-100,
                     high=100,
-                    mechanism=VarianceMechanism.GAUSSIAN,
+                    mechanism=VarianceMechanism.DEFAULT,
                 ),
                 ExactNumber(3).expr,
-                NoiseMechanism.DISCRETE_GAUSSIAN,
+                NoiseMechanism.GEOMETRIC,
             ),
             (
                 GroupByBoundedVariance(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["zero", "one"]}),
                     measure_column="inf",
                     low=-100,
```

### Comparing `tmlt_analytics-0.7.1/test/unit/query_expr_compiler/test_output_schema_visitor.py` & `tmlt_analytics-0.7.2/test/unit/query_expr_compiler/test_output_schema_visitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,23 +139,23 @@
     ),
     (  # Filter on invalid column
         Filter(child=PrivateSource("private"), condition="NONEXISTENT>1"),
         "Invalid filter condition 'NONEXISTENT>1'.*",
     ),
     (  # Rename on non-existent column
         Rename(child=PrivateSource("private"), column_mapper={"NONEXISTENT": "Z"}),
-        "Nonexistent columns {'NONEXISTENT'} in rename query",
+        "Nonexistent columns in rename query: {'NONEXISTENT'}",
     ),
     (  # Rename when column exists
         Rename(child=PrivateSource("private"), column_mapper={"A": "B"}),
         "Cannot rename 'A' to 'B': column 'B' already exists",
     ),
     (  # Select non-existent column
         Select(child=PrivateSource("private"), columns=["NONEXISTENT"]),
-        "Nonexistent columns {'NONEXISTENT'} in select query",
+        "Nonexistent columns in select query: {'NONEXISTENT'}",
     ),
     (  # Nested grouping FlatMap
         FlatMap(
             child=FlatMap(
                 child=PrivateSource("private"),
                 f=lambda row: [{"i": row["X"]} for i in range(row["Repeat"])],
                 schema_new_columns=Schema({"i": "INTEGER"}, grouping_column="i"),
```

### Comparing `tmlt_analytics-0.7.1/test/unit/query_expr_compiler/transformation_visitor/conftest.py` & `tmlt_analytics-0.7.2/test/unit/query_expr_compiler/transformation_visitor/conftest.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/unit/query_expr_compiler/transformation_visitor/test_add_keys.py` & `tmlt_analytics-0.7.2/test/unit/query_expr_compiler/transformation_visitor/test_add_keys.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/unit/query_expr_compiler/transformation_visitor/test_add_rows.py` & `tmlt_analytics-0.7.2/test/unit/query_expr_compiler/transformation_visitor/test_add_rows.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,18 +152,18 @@
         # check dataframe renamed as expected
         self._validate_result(transformation, reference, expected_df)
         assert constraints == []
 
     def test_visit_invalid_rename(self) -> None:
         """Test visit_rename with an invalid query."""
         query = Rename(
-            column_mapper={"column_that_does_not_exit": "asdf"},
+            column_mapper={"column_that_does_not_exist": "asdf"},
             child=PrivateSource(source_id="rows1"),
         )
-        with pytest.raises(ValueError):
+        with pytest.raises(ValueError, match="Nonexistent columns in rename query"):
             query.accept(self.visitor)
 
     @pytest.mark.parametrize(
         "filter_expr,expected_df",
         [
             (
                 "F > I",
@@ -212,15 +212,15 @@
 
     def test_visit_invalid_select(self) -> None:
         """Test visit_select with invalid query."""
         query = Select(
             columns=["column_that_does_not_exist"],
             child=PrivateSource(source_id="rows1"),
         )
-        with pytest.raises(ValueError):
+        with pytest.raises(ValueError, match="Nonexistent columns in select query"):
             query.accept(self.visitor)
 
     @pytest.mark.parametrize(
         "query,expected_df",
         [
             (
                 Map(
@@ -725,16 +725,16 @@
             ),
             augment=True,
             max_num_rows=2,
         )
         with pytest.raises(
             ValueError,
             match=(
-                "Cannot drop infinite values in column group, because it is being used"
-                " as a grouping column"
+                "Cannot drop infinite values from column group, because that column's "
+                "type is not DECIMAL"
             ),
         ):
             invalid_drop_query = DropInfExpr(child=flatmap_query, columns=["group"])
             invalid_drop_query.accept(self.visitor)
         valid_drop_query = DropInfExpr(child=flatmap_query, columns=[])
         transformation, reference, constraints = valid_drop_query.accept(self.visitor)
         self._validate_transform_basics(transformation, reference, valid_drop_query)
```

### Comparing `tmlt_analytics-0.7.1/test/unit/query_expr_compiler/transformation_visitor/test_constraints.py` & `tmlt_analytics-0.7.2/test/unit/query_expr_compiler/transformation_visitor/test_constraints.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/unit/test_binning_spec.py` & `tmlt_analytics-0.7.2/test/unit/test_binning_spec.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 """Unit tests for BinningSpec."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
-# pylint: disable=pointless-string-statement
 
 import datetime
 from typing import Any, List
 
 import pytest
 
 from tmlt.analytics._schema import ColumnDescriptor
 from tmlt.analytics.binning_spec import BinningSpec, _default_bin_names, _edges_as_str
 from tmlt.analytics.query_builder import ColumnType
 
-"""Tests for helper functions releated to default bin names."""
-
 
 @pytest.mark.parametrize(
     "bin_edges,expected_strs",
     [
         ([0, 1, 2], ["0", "1", "2"]),
-        (["0", "1", "2"], ["0", "1", "2"]),
+        (["0", "1", "2"], ["'0'", "'1'", "'2'"]),
         (
             [datetime.date(2022, 1, 1), datetime.date(2022, 2, 1)],
             ["2022-01-01", "2022-02-01"],
         ),
         ([0.0, 0.1, 0.2], ["0.00", "0.10", "0.20"]),
         ([0.0, 0.111111, 0.222222], ["0.00", "0.11", "0.22"]),
         ([0.0, 0.000001, 0.000002], ["0.000000", "0.000001", "0.000002"]),
@@ -70,65 +67,14 @@
     ],
 )
 def test_default_bin_names(args: List[Any], expected_strs: List[str]):
     """Generation of bin names from bin edges works as expected."""
     assert _default_bin_names(*args) == expected_strs
 
 
-"""Tests for :cls:`tmlt.analytics.binning_spec.BinningSpec`."""
-
-
-def test_binning() -> None:
-    """Basic BinningSpec works as expected."""
-    spec = BinningSpec([0, 5, 10, 15, 20])
-    assert spec.bins() == ["[0, 5]", "(5, 10]", "(10, 15]", "(15, 20]"]
-    assert spec.bins(include_null=True) == [
-        "[0, 5]",
-        "(5, 10]",
-        "(10, 15]",
-        "(15, 20]",
-        None,
-    ]
-    assert spec.column_descriptor == ColumnDescriptor(
-        ColumnType.VARCHAR, allow_null=True, allow_nan=False, allow_inf=False
-    )
-    bin_tests = {
-        2: "[0, 5]",
-        7: "(5, 10]",
-        12: "(10, 15]",
-        17: "(15, 20]",
-        -1: None,
-        0: "[0, 5]",
-        20: "(15, 20]",
-        21: None,
-        None: None,
-    }
-    for val, expected_bin in bin_tests.items():
-        assert spec(val) == expected_bin
-
-
-def test_binning_left() -> None:
-    """BinningSpec with right=False works as expected."""
-    spec = BinningSpec([0, 5, 10, 15, 20], right=False)
-    assert spec.bins() == ["[0, 5)", "[5, 10)", "[10, 15)", "[15, 20]"]
-    bin_tests = {
-        2: "[0, 5)",
-        7: "[5, 10)",
-        12: "[10, 15)",
-        17: "[15, 20]",
-        -1: None,
-        0: "[0, 5)",
-        20: "[15, 20]",
-        21: None,
-        None: None,
-    }
-    for val, expected_bin in bin_tests.items():
-        assert spec(val) == expected_bin
-
-
 @pytest.mark.parametrize(
     "edges,ty",
     [
         ([0, 1], ColumnType.INTEGER),
         ([0.0, 1.0], ColumnType.DECIMAL),
         (["0", "1"], ColumnType.VARCHAR),
         ([datetime.date(2022, 1, 1), datetime.date(2022, 1, 2)], ColumnType.DATE),
@@ -159,72 +105,149 @@
 )
 def test_column_type(names: List[Any], ty: ColumnType):
     """BinningSpec.column_descriptor.column_type works as expected."""
     spec = BinningSpec([0, 1, 2], names=names)
     assert spec.column_descriptor.column_type == ty
 
 
-def test_binning_allow_nan() -> None:
+def test_descriptor_allow_nan() -> None:
     """BinningSpec sets allow_nan as expected."""
     edges = [0, 5, 10]
     spec = BinningSpec(edges, names=[float("NaN"), float("0")])
     assert spec.column_descriptor.allow_nan
     spec = BinningSpec(edges, names=[float("-NaN"), float("0")])
     assert spec.column_descriptor.allow_nan
     spec = BinningSpec(edges, names=[float("0"), float("5")])
     assert not spec.column_descriptor.allow_nan
     spec = BinningSpec(edges, names=[float("0"), float(5)], nan_bin=float("nan"))
     assert spec.column_descriptor.allow_nan
     spec = BinningSpec(edges, names=[float("0"), float(5)], nan_bin=3.3)
     assert not spec.column_descriptor.allow_nan
 
 
-def test_binning_allow_null() -> None:
+def test_descriptor_allow_null() -> None:
     """BinningSpec sets allow_null as expected."""
     edges = [0, 5, 10]
     spec = BinningSpec(edges, names=["null", "5"])
     assert spec.column_descriptor.allow_null
     spec = BinningSpec(edges, names=["NULL", "5"])
     assert spec.column_descriptor.allow_null
     spec = BinningSpec(edges, names=["Null", "5"])
     assert spec.column_descriptor.allow_null
     spec = BinningSpec(edges, names=["0", "5"])
     assert spec.column_descriptor.allow_null
 
 
-def test_binning_allow_inf() -> None:
+def test_descriptor_allow_inf() -> None:
     """BinningSpec sets allow_inf as expected."""
     edges = [float("0"), float("5"), float("10")]
-    spec = BinningSpec(edges, names=[float("0"), float("inf")])
+    spec = BinningSpec(edges, names=[float(0), float("inf")])
     assert spec.column_descriptor.allow_inf
-    spec = BinningSpec(edges, names=[float("0"), float("-inf")])
+    spec = BinningSpec(edges, names=[float(0), float("-inf")])
     assert spec.column_descriptor.allow_inf
-    spec = BinningSpec(edges, names=[float("0"), float("5")])
+    spec = BinningSpec(edges, names=[float(0), float(5)])
     assert not spec.column_descriptor.allow_inf
-    spec = BinningSpec(edges, names=[float("0"), float("nan")], nan_bin=float("inf"))
+    spec = BinningSpec(edges, names=[float(0), float("nan")], nan_bin=float("inf"))
     assert spec.column_descriptor.allow_inf
-    spec = BinningSpec(edges, names=[float("0"), float("nan")], nan_bin=float("-inf"))
+    spec = BinningSpec(edges, names=[float(0), float("nan")], nan_bin=float("-inf"))
     assert spec.column_descriptor.allow_inf
-    spec = BinningSpec(edges, names=[float("0"), float(5)], nan_bin=3.3)
+    spec = BinningSpec(edges, names=[float(0), float(5)], nan_bin=3.3)
     assert not spec.column_descriptor.allow_inf
 
 
+@pytest.mark.parametrize(
+    "spec,bins",
+    [
+        (BinningSpec([0, 1, 2]), ["[0, 1]", "(1, 2]"]),
+        (BinningSpec([0.0, 1.0, 2.0]), ["[0.00, 1.00]", "(1.00, 2.00]"]),
+        (BinningSpec(["0", "1", "2"]), ["['0', '1']", "('1', '2']"]),
+        (BinningSpec([0, 1, 2], nan_bin="NaN"), ["[0, 1]", "(1, 2]", "NaN"]),
+        (
+            BinningSpec([0.0, 1.0, 2.0], nan_bin="NaN"),
+            ["[0.00, 1.00]", "(1.00, 2.00]", "NaN"],
+        ),
+        (
+            BinningSpec(["0", "1", "2"], nan_bin="NaN"),
+            ["['0', '1']", "('1', '2']", "NaN"],
+        ),
+        (
+            BinningSpec(["0", "1", "2"], nan_bin="['0', '1']"),
+            ["['0', '1']", "('1', '2']"],
+        ),
+    ],
+)
+def test_bins(spec: BinningSpec, bins: List) -> None:
+    """BinningSpec.bins() returns the expected value."""
+    assert spec.bins() == bins
+    assert spec.bins(include_null=True) == bins + [None]
+
+
+def test_binning() -> None:
+    """Basic BinningSpec works as expected."""
+    spec = BinningSpec([0, 5, 10, 15, 20])
+    assert spec.bins() == ["[0, 5]", "(5, 10]", "(10, 15]", "(15, 20]"]
+    assert spec.bins(include_null=True) == [
+        "[0, 5]",
+        "(5, 10]",
+        "(10, 15]",
+        "(15, 20]",
+        None,
+    ]
+    assert spec.column_descriptor == ColumnDescriptor(
+        ColumnType.VARCHAR, allow_null=True, allow_nan=False, allow_inf=False
+    )
+    bin_tests = {
+        2: "[0, 5]",
+        7: "(5, 10]",
+        12: "(10, 15]",
+        17: "(15, 20]",
+        -1: None,
+        0: "[0, 5]",
+        20: "(15, 20]",
+        21: None,
+        3.0: "[0, 5]",
+        20.1: None,
+        None: None,
+    }
+    for val, expected_bin in bin_tests.items():
+        assert spec(val) == expected_bin
+
+
+def test_binning_left() -> None:
+    """BinningSpec with right=False works as expected."""
+    spec = BinningSpec([0, 5, 10, 15, 20], right=False)
+    assert spec.bins() == ["[0, 5)", "[5, 10)", "[10, 15)", "[15, 20]"]
+    bin_tests = {
+        2: "[0, 5)",
+        7: "[5, 10)",
+        12: "[10, 15)",
+        17: "[15, 20]",
+        -1: None,
+        0: "[0, 5)",
+        20: "[15, 20]",
+        21: None,
+        None: None,
+    }
+    for val, expected_bin in bin_tests.items():
+        assert spec(val) == expected_bin
+
+
 def test_binning_noninclusive() -> None:
     """BinningSpec with include_both_endpoints=False works as expected."""
     spec = BinningSpec([0, 5, 10, 15, 20], include_both_endpoints=False)
     assert spec.bins() == ["(0, 5]", "(5, 10]", "(10, 15]", "(15, 20]"]
     assert spec(0) is None
     assert spec(20) == "(15, 20]"
     spec = BinningSpec([0, 5, 10, 15, 20], right=False, include_both_endpoints=False)
     assert spec.bins() == ["[0, 5)", "[5, 10)", "[10, 15)", "[15, 20)"]
     assert spec(0) == "[0, 5)"
     assert spec(20) is None
 
 
-def test_binning_names() -> None:
+def test_binning_custom_names() -> None:
     """BinningSpec with custom bin names works as expected."""
     spec = BinningSpec([0, 64, 69, 79, 89, 100], names=["F", "D", "C", "B", "A"])
     assert spec.bins() == ["F", "D", "C", "B", "A"]
     assert spec.column_descriptor.column_type == ColumnType.VARCHAR
     bin_tests = {0: "F", 10: "F", 75: "C", 100: "A", None: None}
     for val, expected_bin in bin_tests.items():
         assert spec(val) == expected_bin
```

### Comparing `tmlt_analytics-0.7.1/test/unit/test_catalog.py` & `tmlt_analytics-0.7.2/test/unit/test_catalog.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/unit/test_cleanup.py` & `tmlt_analytics-0.7.2/test/unit/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/unit/test_constraints.py` & `tmlt_analytics-0.7.2/test/unit/test_constraints.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/unit/test_keyset.py` & `tmlt_analytics-0.7.2/test/unit/test_keyset.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/unit/test_neighboring_relations.py` & `tmlt_analytics-0.7.2/test/unit/test_neighboring_relations.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/unit/test_noise_info.py` & `tmlt_analytics-0.7.2/test/unit/test_noise_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
 
 from typing import Dict
 
 import pytest
 import sympy as sp
-from tmlt.core.domains.numpy_domains import NumpyIntegerDomain
+from tmlt.core.domains.numpy_domains import NumpyFloatDomain, NumpyIntegerDomain
 from tmlt.core.domains.pandas_domains import PandasSeriesDomain
 from tmlt.core.measurements.base import Measurement
 from tmlt.core.measurements.noise_mechanisms import (
     AddDiscreteGaussianNoise,
+    AddGaussianNoise,
     AddGeometricNoise,
     AddLaplaceNoise,
 )
 from tmlt.core.measurements.pandas_measurements.series import NoisyQuantile
 from tmlt.core.measures import PureDP
 
 from tmlt.analytics._noise_info import (
@@ -42,14 +43,20 @@
                 {
                     "noise_mechanism": _NoiseMechanism.DISCRETE_GAUSSIAN,
                     "noise_parameter": 4.5,
                 }
             ],
         ),
         (
+            AddGaussianNoise(
+                input_domain=NumpyFloatDomain(), sigma_squared=sp.Rational(5.5)
+            ),
+            [{"noise_mechanism": _NoiseMechanism.GAUSSIAN, "noise_parameter": 5.5}],
+        ),
+        (
             NoisyQuantile(
                 PandasSeriesDomain(element_domain=NumpyIntegerDomain()),
                 PureDP(),
                 quantile=0.5,
                 lower=0,
                 upper=10,
                 epsilon=sp.Rational(5.5),
@@ -60,14 +67,15 @@
 )
 def test_noise_from_measurement(measurement: Measurement, expected: Dict):
     """Get noise from measurement."""
     noise_info = _noise_from_measurement(measurement)
     assert noise_info == expected
 
 
+# TODO(#2730): Add test for continuous gaussian once it's added to core
 @pytest.mark.parametrize(
     "noise_info,p,expected",
     [
         ({"noise_mechanism": _NoiseMechanism.LAPLACE, "noise_parameter": 1}, 0.5, 0.0),
         (
             {"noise_mechanism": _NoiseMechanism.LAPLACE, "noise_parameter": 1},
             0.75,
```

### Comparing `tmlt_analytics-0.7.1/test/unit/test_privacy_budget.py` & `tmlt_analytics-0.7.2/test/unit/test_privacy_budget.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/unit/test_privacy_budget_rounding_helper.py` & `tmlt_analytics-0.7.2/test/unit/test_privacy_budget_rounding_helper.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/unit/test_protected_change.py` & `tmlt_analytics-0.7.2/test/unit/test_protected_change.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/unit/test_query_builder.py` & `tmlt_analytics-0.7.2/test/unit/test_query_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -610,17 +610,14 @@
 def test_replace_null_and_nan(
     replace_with: Optional[
         Mapping[str, Union[int, float, str, datetime.date, datetime.datetime]]
     ]
 ) -> None:
     """QueryBuilder.replace_null_and_nan works as expected."""
     query = root_builder().replace_null_and_nan(replace_with).count()
-    # You want to use both of these assert statements:
-    # - `self.assertIsInstance` will print a helpful error message if it isn't true
-    # - `assert isinstance` helps mypy
     assert isinstance(query, GroupByCount)
     replace_expr = query.child
     assert isinstance(replace_expr, ReplaceNullAndNan)
 
     root_expr = replace_expr.child
     assert isinstance(root_expr, PrivateSource)
     assert root_expr.source_id == PRIVATE_ID
```

### Comparing `tmlt_analytics-0.7.1/test/unit/test_query_expr_compiler.py` & `tmlt_analytics-0.7.2/test/unit/test_query_expr_compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -943,95 +943,70 @@
                     low=0.0,
                     high=3.0,
                     mechanism=SumMechanism.LAPLACE,
                 ),
                 PureDP(),
                 [pd.DataFrame({"Repeat": [1, 2], "sum": [3.0, 6.0]})],
             ),
-        ],
-    )
-    def test_noise_param_combinations(
-        self,
-        query: QueryExpr,
-        output_measure: Union[PureDP, RhoZCDP],
-        expected: List[pd.DataFrame],
-    ):
-        """Tests aggregation with various privacy definition and mechanism."""
-        compiler = QueryExprCompiler(output_measure=output_measure)
-        privacy_budget = (
-            PureDPBudget(float("inf"))
-            if isinstance(output_measure, PureDP)
-            else RhoZCDPBudget(float("inf"))
-        )
-        measurement = compiler(
-            [query],
-            privacy_budget=privacy_budget,
-            stability=self.stability,
-            input_domain=self.input_domain,
-            input_metric=self.input_metric,
-            public_sources={"public": self.join_df},
-            catalog=self.catalog,
-            table_constraints={t: [] for t in self.stability.keys()},
-        )
-        actual = measurement({NamedTable("private"): self.sdf})
-        assert len(actual) == len(expected)
-        for actual_sdf, expected_df in zip(actual, expected):
-            assert_frame_equal_with_sort(actual_sdf.toPandas(), expected_df)
-
-    @pytest.mark.parametrize(
-        "query_exprs",
-        [
             (  # BoundedAverage with floating-point valued measure column with GAUSSIAN
                 [
                     GroupByBoundedAverage(
                         child=PrivateSource("private"),
                         groupby_keys=KeySet.from_dict({"A": ["0", "1"]}),
                         measure_column="X",
                         low=0.0,
                         high=1.0,
                         mechanism=AverageMechanism.GAUSSIAN,
-                    )
+                    ),
+                    RhoZCDP(),
+                    [pd.DataFrame({"A": ["0", "1"], "average": [2 / 3, 1.0]})],
                 ]
             ),
             (  # BoundedSTDEV on floating-point valued measure column with GAUSSIAN
                 [
                     GroupByBoundedSTDEV(
                         child=PrivateSource("private"),
                         groupby_keys=KeySet.from_dict({"A": ["0", "1"]}),
                         measure_column="X",
                         low=0.0,
                         high=1.0,
                         mechanism=StdevMechanism.GAUSSIAN,
-                    )
+                    ),
+                    RhoZCDP(),
+                    [pd.DataFrame({"A": ["0", "1"], "stdev": [0.471404, 0.5]})],
                 ]
             ),
             (  # BoundedVariance on floating-point valued measure column with GAUSSIAN
                 [
                     GroupByBoundedVariance(
                         child=PrivateSource("private"),
                         groupby_keys=KeySet.from_dict({"A": ["0", "1"]}),
                         measure_column="X",
                         low=0.0,
                         high=1.0,
                         output_column="var",
                         mechanism=VarianceMechanism.GAUSSIAN,
-                    )
+                    ),
+                    RhoZCDP(),
+                    [pd.DataFrame({"A": ["0", "1"], "var": [0.22222, 0.25]})],
                 ]
             ),
             (  # BoundedSum on floating-point valued measure column with GAUSSIAN
                 [
                     GroupByBoundedSum(
                         child=PrivateSource("private"),
                         groupby_keys=KeySet.from_dict({"A": ["0", "1"]}),
                         measure_column="X",
                         low=0.0,
                         high=1.0,
                         output_column="sum",
                         mechanism=SumMechanism.GAUSSIAN,
-                    )
+                    ),
+                    RhoZCDP(),
+                    [pd.DataFrame({"A": ["0", "1"], "sum": [2.0, 1.0]})],
                 ]
             ),
             (  # Grouping flat map with GAUSSIAN
                 [
                     GroupByBoundedSum(
                         child=ReplaceNullAndNan(
                             replace_with={},
@@ -1056,39 +1031,48 @@
                             ),
                         ),
                         groupby_keys=KeySet.from_dict({"Repeat": [1, 2]}),
                         measure_column="i",
                         low=0.0,
                         high=3.0,
                         mechanism=SumMechanism.GAUSSIAN,
-                    )
+                    ),
+                    RhoZCDP(),
+                    [pd.DataFrame({"Repeat": [1, 2], "sum": [3.0, 6.0]})],
                 ]
             ),
         ],
     )
-    def test_gaussian_noise_param_on_float_errors(self, query_exprs: List[QueryExpr]):
-        """Tests that Gaussian noise with floating-point values errors."""
-        compiler = QueryExprCompiler(output_measure=RhoZCDP())
-        with pytest.raises(
-            NotImplementedError,
-            match=(
-                "(GAUSSIAN)|(Discrete gaussian) noise is not yet compatible with"
-                " floating-point values."
-            ),
-        ):
-            compiler(
-                query_exprs,
-                privacy_budget=RhoZCDPBudget(float("inf")),
-                stability=self.stability,
-                input_domain=self.input_domain,
-                input_metric=self.input_metric,
-                public_sources={"public": self.join_df},
-                catalog=self.catalog,
-                table_constraints={t: [] for t in self.stability.keys()},
-            )
+    def test_noise_param_combinations(
+        self,
+        query: QueryExpr,
+        output_measure: Union[PureDP, RhoZCDP],
+        expected: List[pd.DataFrame],
+    ):
+        """Tests aggregation with various privacy definition and mechanism."""
+        compiler = QueryExprCompiler(output_measure=output_measure)
+        privacy_budget = (
+            PureDPBudget(float("inf"))
+            if isinstance(output_measure, PureDP)
+            else RhoZCDPBudget(float("inf"))
+        )
+        measurement = compiler(
+            [query],
+            privacy_budget=privacy_budget,
+            stability=self.stability,
+            input_domain=self.input_domain,
+            input_metric=self.input_metric,
+            public_sources={"public": self.join_df},
+            catalog=self.catalog,
+            table_constraints={t: [] for t in self.stability.keys()},
+        )
+        actual = measurement({NamedTable("private"): self.sdf})
+        assert len(actual) == len(expected)
+        for actual_sdf, expected_df in zip(actual, expected):
+            assert_frame_equal_with_sort(actual_sdf.toPandas(), expected_df)
 
     def test_join_public_dataframe(self, spark):
         """Public join works with public tables given as Spark dataframes."""
         # This sets up a DF with a column that Spark thinks could contain NaNs,
         # but which doesn't actually contain any. This is allowed by Analytics,
         # but it has caused some bugs in the past which this test should
         # detect.
```

### Comparing `tmlt_analytics-0.7.1/test/unit/test_query_expression.py` & `tmlt_analytics-0.7.2/test/unit/test_query_expression.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/unit/test_query_expression_visitor.py` & `tmlt_analytics-0.7.2/test/unit/test_query_expression_visitor.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/unit/test_schema.py` & `tmlt_analytics-0.7.2/test/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/unit/test_schema_conversion.py` & `tmlt_analytics-0.7.2/test/unit/test_schema_conversion.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/unit/test_session.py` & `tmlt_analytics-0.7.2/test/unit/test_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,20 @@
     ColumnType,
     Schema,
     analytics_to_spark_columns_descriptor,
     spark_schema_to_analytics_columns,
 )
 from tmlt.analytics._table_identifier import NamedTable, TableCollection
 from tmlt.analytics._table_reference import TableReference
-from tmlt.analytics.constraints import MaxRowsPerID
+from tmlt.analytics.constraints import (
+    Constraint,
+    MaxGroupsPerID,
+    MaxRowsPerGroupPerID,
+    MaxRowsPerID,
+)
 from tmlt.analytics.privacy_budget import (
     ApproxDPBudget,
     PrivacyBudget,
     PureDPBudget,
     RhoZCDPBudget,
 )
 from tmlt.analytics.protected_change import (
@@ -1164,14 +1169,19 @@
                 QueryBuilder("private").drop_null_and_nan(["A", "B", "X"]),
                 """Columns:
 \t- 'A'  VARCHAR, not null
 \t- 'B'  INTEGER, not null
 \t- 'X'  INTEGER, not null""",
                 id="query_builder_drop_null",
             ),
+            pytest.param(
+                QueryBuilder("private").count(),
+                """Columns:
+\t- 'count'  INTEGER, not null""",
+            ),
         ],
     )
     def test_describe_query(
         self, spark, query: Union[str, QueryBuilder, QueryExpr], expected_output: str
     ):
         """Test :func:`_describe` with a QueryExpr, QueryBuilder, or table name."""
         with patch("builtins.print") as mock_print, patch(
@@ -1188,14 +1198,92 @@
                 accountant=mock_accountant,
                 public_sources={"public1": public_df_1, "public2": public_df_2},
             )
 
             session.describe(query)
             mock_print.assert_called_with(expected_output)
 
+    @pytest.mark.parametrize(
+        "constraints,expected_output",
+        [
+            ([MaxRowsPerID(5)], "\t\t- MaxRowsPerID(max=5)"),
+            (
+                [MaxRowsPerGroupPerID("B", 1), MaxGroupsPerID("X", 5)],
+                "\t\t- MaxRowsPerGroupPerID(grouping_column='B', max=1)\n\t\t"
+                "- MaxGroupsPerID(grouping_column='X', max=5)",
+            ),
+        ],
+    )
+    def test_describe_table_with_constraints(
+        self, constraints: List[Constraint], expected_output: str
+    ):
+        """Test :func:`_describe` with a table with constraints."""
+        with patch("builtins.print") as mock_print, patch(
+            "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
+        ) as mock_accountant:
+            self._setup_accountant_with_id(
+                mock_accountant, privacy_budget=ExactNumber(10)
+            )
+            mock_accountant.state = PrivacyAccountantState.ACTIVE
+            session = Session(accountant=mock_accountant, public_sources={})
+            # pylint: disable=protected-access
+            session._table_constraints[NamedTable("private")] = constraints
+            # pylint: enable=protected-access
+            expected = (
+                """Columns:
+\t- 'A'  VARCHAR, ID column (in ID space identifier_A)
+\t- 'B'  INTEGER
+\t- 'X'  INTEGER
+\tConstraints:\n"""
+                + expected_output
+            )
+            session.describe("private")
+            # pylint: enable=line-too-long
+            mock_print.assert_called_with(expected)
+
+    @pytest.mark.parametrize(
+        "query,expected_output",
+        [
+            (
+                QueryBuilder("private").enforce(MaxRowsPerID(5)),
+                "\t\t- MaxRowsPerID(max=5)",
+            ),
+            (
+                QueryBuilder("private")
+                .enforce(MaxGroupsPerID("X", 5))
+                .enforce(MaxRowsPerGroupPerID("B", 1)),
+                "\t\t- MaxGroupsPerID(grouping_column='X', max=5)\n\t\t"
+                "- MaxRowsPerGroupPerID(grouping_column='B', max=1)",
+            ),
+        ],
+    )
+    def test_describe_query_with_constraints(
+        self, query: QueryBuilder, expected_output: str
+    ):
+        """Test :func:`_describe` with a query with constraints."""
+        with patch("builtins.print") as mock_print, patch(
+            "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
+        ) as mock_accountant:
+            self._setup_accountant_with_id(
+                mock_accountant, privacy_budget=ExactNumber(10)
+            )
+            mock_accountant.state = PrivacyAccountantState.ACTIVE
+            session = Session(accountant=mock_accountant, public_sources={})
+            expected = (
+                """Columns:
+\t- 'A'  VARCHAR, ID column (in ID space identifier_A)
+\t- 'B'  INTEGER
+\t- 'X'  INTEGER
+\tConstraints:\n"""
+                + expected_output
+            )
+            session.describe(query)
+            # pylint: enable=line-too-long
+            mock_print.assert_called_with(expected)
+
     def test_supported_spark_types(self, spark):
         """Session works with supported Spark data types."""
         alltypes_sdf = spark.createDataFrame(
             pd.DataFrame(
                 [[1.2, 3.4, 17, 42, "blah"]], columns=["A", "B", "C", "D", "E"]
             ),
             schema=StructType(
@@ -2036,15 +2124,15 @@
                 sp.Integer(10),
                 PureDP(),
                 [("df1", 1)],
                 [],
             ),
             (
                 Session.Builder().with_privacy_budget(ApproxDPBudget(10, 0.5)),
-                (sp.Integer(10), 0),
+                (sp.Integer(10), sp.Rational("0.5")),
                 ApproxDP(),
                 [("df1", 1)],
                 [],
             ),
             (
                 Session.Builder().with_privacy_budget(PureDPBudget(1.5)),
                 sp.Rational("1.5"),
```

### Comparing `tmlt_analytics-0.7.1/test/unit/test_table_identifiers.py` & `tmlt_analytics-0.7.2/test/unit/test_table_identifiers.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/unit/test_transformation_utils.py` & `tmlt_analytics-0.7.2/test/unit/test_transformation_utils.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/unit/test_truncation_strategy.py` & `tmlt_analytics-0.7.2/test/unit/test_truncation_strategy.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/test/unit/test_utils.py` & `tmlt_analytics-0.7.2/test/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/_catalog.py` & `tmlt_analytics-0.7.2/tmlt/analytics/_catalog.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/_coerce_spark_schema.py` & `tmlt_analytics-0.7.2/tmlt/analytics/_coerce_spark_schema.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/_neighboring_relation.py` & `tmlt_analytics-0.7.2/tmlt/analytics/_neighboring_relation.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/_neighboring_relation_visitor.py` & `tmlt_analytics-0.7.2/tmlt/analytics/_neighboring_relation_visitor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Module to define NeighboringRelationVisitors."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 
+import dataclasses
 from typing import Any, Dict, NamedTuple, Union
 
 import sympy as sp
 from pyspark.sql import DataFrame
 from tmlt.core.domains.base import Domain
 from tmlt.core.domains.collections import DictDomain
 from tmlt.core.domains.spark_domains import SparkDataFrameDomain
@@ -28,14 +29,38 @@
     AddRemoveRowsAcrossGroups,
     Conjunction,
     NeighboringRelationVisitor,
 )
 from tmlt.analytics._table_identifier import Identifier, NamedTable, TableCollection
 
 
+def _ensure_valid_schema_ark(
+    metric_dict: Dict[Identifier, str], domain_dict: Dict[Identifier, Any]
+) -> Dict[Identifier, Any]:
+    """Ensure valid schema for an ``AddRemoveKeys`` neighboring relation.
+
+    Ensures that the schema for the table(s) in the ``AddRemoveKeys`` neighboring
+    relation have consistent nullability in the key column(s), which is required for
+    the metric to support the domain.
+    """
+    nullable_id_col = any(
+        domain_dict[table_id].schema[key_column].allow_null
+        for table_id, key_column in metric_dict.items()
+    )
+    if nullable_id_col:
+        for table_id, key_column in metric_dict.items():
+            table_schema = domain_dict[table_id].schema
+            table_schema[key_column] = dataclasses.replace(
+                table_schema[key_column], allow_null=True
+            )
+            domain_dict[table_id] = SparkDataFrameDomain(table_schema)
+
+    return domain_dict
+
+
 class _RelationIDVisitor(NeighboringRelationVisitor):
     """Generate identifiers for neighboring relations."""
 
     def visit_add_remove_rows(self, relation: AddRemoveRows) -> Identifier:
         return NamedTable(relation.table)
 
     def visit_add_remove_rows_across_groups(
@@ -130,15 +155,15 @@
         domain_dict: Dict[Identifier, Any] = {}
         for table_name, key_column in relation.table_to_key_column.items():
             table_id = _RelationIDVisitor().visit_str(table_name)
             data = self.tables[table_name]
             domain_dict[table_id] = SparkDataFrameDomain.from_spark_schema(data.schema)
             metric_dict[table_id] = key_column
             data_dict[table_id] = data
-
+        domain_dict = _ensure_valid_schema_ark(metric_dict, domain_dict)
         return self.Output(
             DictDomain(domain_dict), CoreAddRemoveKeys(metric_dict), distance, data_dict
         )
 
     def visit_conjunction(self, relation: Conjunction) -> Output:
         """Build Core state from ``Conjunction`` neighboring relation."""
         domain_dict: Dict[Identifier, Any] = {}
```

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/_noise_info.py` & `tmlt_analytics-0.7.2/tmlt/analytics/_noise_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,38 +5,42 @@
 from functools import singledispatch
 from typing import Any, Dict, List, Set, Tuple, Union
 
 from pyspark.sql import DataFrame
 from tmlt.core.measurements.base import Measurement
 from tmlt.core.measurements.noise_mechanisms import (
     AddDiscreteGaussianNoise,
+    AddGaussianNoise,
     AddGeometricNoise,
     AddLaplaceNoise,
 )
 from tmlt.core.measurements.pandas_measurements.series import NoisyQuantile
 from tmlt.core.transformations.base import Transformation
 from tmlt.core.utils.exact_number import ExactNumber
 
 
 class _NoiseMechanism(Enum):
     LAPLACE = 1
     GEOMETRIC = 2
     DISCRETE_GAUSSIAN = 3
     EXPONENTIAL = 4
+    GAUSSIAN = 5
 
     def to_cls(self):
         """Returns the appropriate measurement class for this enum value."""
         if self.value == _NoiseMechanism.LAPLACE.value:
             return AddLaplaceNoise
         if self.value == _NoiseMechanism.GEOMETRIC.value:
             return AddGeometricNoise
         if self.value == _NoiseMechanism.DISCRETE_GAUSSIAN.value:
             return AddDiscreteGaussianNoise
         if self.value == _NoiseMechanism.EXPONENTIAL.value:
             return NoisyQuantile
+        if self.value == _NoiseMechanism.GAUSSIAN.value:
+            return AddGaussianNoise
         raise KeyError("Unknown measurement type.")
 
 
 @singledispatch
 def _get_info(a: Any) -> Any:
     """Get information from a measurement or transformation.
 
@@ -141,14 +145,21 @@
     if name == "AddDiscreteGaussianNoise":
         return [
             {
                 "noise_mechanism": _NoiseMechanism.DISCRETE_GAUSSIAN,
                 "noise_parameter": info["_sigma_squared"],
             }
         ]
+    if name == "AddGaussianNoise":
+        return [
+            {
+                "noise_mechanism": _NoiseMechanism.GAUSSIAN,
+                "noise_parameter": info["_sigma_squared"],
+            }
+        ]
     if name == "AddGeometricNoise":
         return [
             {
                 "noise_mechanism": _NoiseMechanism.GEOMETRIC,
                 "noise_parameter": info["_alpha"],
             }
         ]
```

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/_privacy_budget_rounding_helper.py` & `tmlt_analytics-0.7.2/tmlt/analytics/_privacy_budget_rounding_helper.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/_query_expr_compiler/_compiler.py` & `tmlt_analytics-0.7.2/tmlt/analytics/_query_expr_compiler/_compiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -151,32 +151,38 @@
             input_metric=input_metric,
             output_measure=self._output_measure,
             default_mechanism=self._mechanism,
             public_sources=public_sources,
             catalog=catalog,
             table_constraints=table_constraints,
         )
+
         measurements: List[Measurement] = []
+        # Note: Each query is re-using the adjusted_budget from the same visitor, which
+        # could become a problem if we go back to supporting multiple queries.
         for query in queries:
             query_measurement = query.accept(visitor)
             if not isinstance(query_measurement, Measurement):
                 raise AssertionError(
                     "This query did not create a measurement. "
                     "This is probably a bug; please let us know so we can fix it!"
                 )
-            if query_measurement.privacy_function(stability) != privacy_budget.value:
+            if (
+                query_measurement.privacy_function(stability)
+                != visitor.adjusted_budget.value
+            ):
                 raise AssertionError(
                     "Query measurement privacy function does not match "
                     "privacy budget value. This is probably a bug; "
                     "please let us know so we can fix it!"
                 )
             measurements.append(query_measurement)
 
         measurement = Composition(measurements)
-        if measurement.privacy_function(stability) != privacy_budget.value:
+        if measurement.privacy_function(stability) != visitor.adjusted_budget.value:
             raise AssertionError(
                 "Measurement privacy function does not match "
                 "privacy budget. This is probably a bug; "
                 "please let us know so we can fix it!"
             )
         return measurement
```

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/_query_expr_compiler/_constraint_propagation.py` & `tmlt_analytics-0.7.2/tmlt/analytics/_query_expr_compiler/_constraint_propagation.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py` & `tmlt_analytics-0.7.2/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Defines a visitor for creating noisy measurements from query expressions."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
 
 import dataclasses
 import math
+import warnings
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import sympy as sp
 from pyspark.sql import DataFrame
 from tmlt.core.domains.collections import DictDomain
 from tmlt.core.domains.spark_domains import (
     SparkColumnDescriptor,
@@ -59,15 +60,15 @@
 from tmlt.analytics.constraints import (
     Constraint,
     MaxGroupsPerID,
     MaxRowsPerGroupPerID,
     MaxRowsPerID,
 )
 from tmlt.analytics.keyset import KeySet
-from tmlt.analytics.privacy_budget import PrivacyBudget
+from tmlt.analytics.privacy_budget import ApproxDPBudget, PrivacyBudget
 from tmlt.analytics.query_expr import (
     AverageMechanism,
     CountDistinctMechanism,
     CountMechanism,
     DropNullAndNan,
     EnforceConstraint,
     GroupByBoundedAverage,
@@ -266,14 +267,15 @@
         default_mechanism: NoiseMechanism,
         public_sources: Dict[str, DataFrame],
         catalog: Catalog,
         table_constraints: Dict[Identifier, List[Constraint]],
     ):
         """Constructor for MeasurementVisitor."""
         self.budget = privacy_budget
+        self.adjusted_budget = privacy_budget
         self.stability = stability
         self.input_domain = input_domain
         self.input_metric = input_metric
         self.default_mechanism = default_mechanism
         self.public_sources = public_sources
         self.output_measure = output_measure
         self.catalog = catalog
@@ -384,55 +386,119 @@
         else:
             # This should never happen
             raise AssertionError(
                 f"Did not recognize the requested mechanism {requested_mechanism}."
                 " This is probably a bug; please let us know about it so we can fix it!"
             )
 
+    def _validate_approxDP_and_adjust_budget(
+        self,
+        expr: Union[
+            GroupByBoundedAverage,
+            GroupByBoundedSTDEV,
+            GroupByBoundedSum,
+            GroupByBoundedVariance,
+            GroupByCount,
+            GroupByCountDistinct,
+        ],
+    ) -> None:
+        """Validate and set adjusted_budget for ApproxDP queries.
+
+        First, validate that the user is not using a Gaussian noise mechanism with
+        ApproxDP. Then, for queries that use noise addition mechanisms replace non-zero
+        deltas with zero in self.adjusted_budget. If the user chose this mechanism
+        (i.e. didn't use the DEFAULT mechanism) we warn them of this replacement.
+        """
+        if not isinstance(self.budget, ApproxDPBudget):
+            return
+
+        if expr.mechanism in (
+            AverageMechanism.GAUSSIAN,
+            CountDistinctMechanism.GAUSSIAN,
+            CountMechanism.GAUSSIAN,
+            StdevMechanism.GAUSSIAN,
+            SumMechanism.GAUSSIAN,
+            VarianceMechanism.GAUSSIAN,
+        ):
+            raise NotImplementedError(
+                "Gaussian noise is only supported with RhoZCDP. Please use "
+                "CountMechanism.LAPLACE instead."
+            )
+
+        epsilon, delta = self.budget.value
+        if delta != 0:
+            if expr.mechanism in (
+                AverageMechanism.LAPLACE,
+                CountDistinctMechanism.LAPLACE,
+                CountMechanism.LAPLACE,
+                StdevMechanism.LAPLACE,
+                SumMechanism.LAPLACE,
+                VarianceMechanism.LAPLACE,
+            ):
+                warnings.warn(
+                    "When using LAPLACE with an ApproxDPBudget, the delta value of "
+                    "the budget will be replaced with zero."
+                )
+                self.adjusted_budget = ApproxDPBudget(epsilon, 0)
+            elif expr.mechanism in (
+                AverageMechanism.DEFAULT,
+                CountDistinctMechanism.DEFAULT,
+                CountMechanism.DEFAULT,
+                StdevMechanism.DEFAULT,
+                SumMechanism.DEFAULT,
+                VarianceMechanism.DEFAULT,
+            ):
+                self.adjusted_budget = ApproxDPBudget(epsilon, 0)
+            else:
+                raise AssertionError(
+                    f"Unknown mechanism {expr.mechanism}. This is probably a bug; "
+                    "please let us know so we can fix it!"
+                )
+
     def _pick_noise_for_non_count(
         self,
         query: Union[
             GroupByBoundedAverage,
             GroupByBoundedSTDEV,
             GroupByBoundedSum,
             GroupByBoundedVariance,
         ],
         measure_column_type: SparkColumnDescriptor,
     ) -> NoiseMechanism:
-        """Pick the noise mechnaism for non-count queries.
+        """Pick the noise mechanism for non-count queries.
 
         GroupByQuantile only supports one noise mechanism, so it is not
         included here.
         """
         requested_mechanism: NoiseMechanism
         if query.mechanism in (
             SumMechanism.DEFAULT,
             AverageMechanism.DEFAULT,
             VarianceMechanism.DEFAULT,
             StdevMechanism.DEFAULT,
         ):
             requested_mechanism = (
                 NoiseMechanism.LAPLACE
                 if isinstance(self.output_measure, (PureDP, ApproxDP))
-                else NoiseMechanism.DISCRETE_GAUSSIAN
+                else NoiseMechanism.GAUSSIAN
             )
         elif query.mechanism in (
             SumMechanism.LAPLACE,
             AverageMechanism.LAPLACE,
             VarianceMechanism.LAPLACE,
             StdevMechanism.LAPLACE,
         ):
             requested_mechanism = NoiseMechanism.LAPLACE
         elif query.mechanism in (
             SumMechanism.GAUSSIAN,
             AverageMechanism.GAUSSIAN,
             VarianceMechanism.GAUSSIAN,
             StdevMechanism.GAUSSIAN,
         ):
-            requested_mechanism = NoiseMechanism.DISCRETE_GAUSSIAN
+            requested_mechanism = NoiseMechanism.GAUSSIAN
         else:
             raise ValueError(
                 f"Did not recognize requested mechanism {query.mechanism}."
                 " Supported mechanisms are DEFAULT, LAPLACE,  and GAUSSIAN."
             )
 
         # If the query requested a Laplace measure ...
@@ -445,25 +511,33 @@
                 raise AssertionError(
                     "Query's measure column should be numeric. This should"
                     " not happen and is probably a bug;  please let us know"
                     " so we can fix it!"
                 )
 
         # If the query requested a Gaussian measure...
-        elif requested_mechanism == NoiseMechanism.DISCRETE_GAUSSIAN:
-            if isinstance(measure_column_type, SparkIntegerColumnDescriptor):
+        elif requested_mechanism == NoiseMechanism.GAUSSIAN:
+            if isinstance(self.output_measure, PureDP):
+                raise ValueError(
+                    "Gaussian noise is not supported under PureDP. "
+                    "Please use RhoZCDP or another measure."
+                )
+            if isinstance(measure_column_type, SparkFloatColumnDescriptor):
+                return NoiseMechanism.GAUSSIAN
+            elif isinstance(measure_column_type, SparkIntegerColumnDescriptor):
                 return NoiseMechanism.DISCRETE_GAUSSIAN
             else:
-                raise NotImplementedError(
-                    f"{NoiseMechanism.DISCRETE_GAUSSIAN} noise is not yet"
-                    " compatible with floating-point values."
+                raise AssertionError(
+                    "Query's measure column should be numeric. This should"
+                    " not happen and is probably a bug;  please let us know"
+                    " so we can fix it!"
                 )
 
         # The requested_mechanism should be either LAPLACE or
-        # DISCRETE_GAUSSIAN, so something has gone awry
+        # GAUSSIAN, so something has gone awry
         else:
             raise AssertionError(
                 f"Did not recognize requested mechanism {requested_mechanism}."
                 " This is probably a bug; please let us know about it so we can fix it!"
             )
 
     @staticmethod
@@ -475,15 +549,18 @@
     ) -> GroupBy:
         """Build a groupby query from the parameters provided.
 
         This groupby query will run after the provided Transformation.
         """
         # TODO(#1044 and #1547): Update condition to when issue is resolved.
         # isinstance(self._output_measure, RhoZCDP)
-        use_l2 = mechanism == NoiseMechanism.DISCRETE_GAUSSIAN
+        use_l2 = mechanism in (
+            NoiseMechanism.DISCRETE_GAUSSIAN,
+            NoiseMechanism.GAUSSIAN,
+        )
 
         groupby_df: DataFrame = groupby_keys.dataframe()
 
         return GroupBy(
             input_domain=input_domain,
             input_metric=input_metric,
             use_l2=use_l2,
@@ -591,23 +668,25 @@
             groupby=groupby,
             lower_bound=lower_bound,
             upper_bound=upper_bound,
         )
 
     def _validate_measurement(self, measurement: Measurement, mid_stability: sp.Expr):
         """Validate a measurement."""
-        if measurement.privacy_function(mid_stability) != self.budget.value:
+        if measurement.privacy_function(mid_stability) != self.adjusted_budget.value:
             raise AssertionError(
                 "Privacy function does not match per-query privacy budget. "
                 "This is probably a bug; please let us know so we can "
                 "fix it!"
             )
 
     def visit_groupby_count(self, expr: GroupByCount) -> Measurement:
         """Create a measurement from a GroupByCount query expression."""
+        self._validate_approxDP_and_adjust_budget(expr)
+
         # Peek at the schema, to see if there are errors there
         OutputSchemaVisitor(self.catalog).visit_groupby_count(expr)
         mechanism = self._pick_noise_for_count(expr)
         child_transformation, child_ref = self._truncate_table(
             *self._visit_child_transformation(expr.child, mechanism),
             grouping_columns=expr.groupby_keys.dataframe().columns,
         )
@@ -629,24 +708,25 @@
         )
 
         agg = create_count_measurement(
             input_domain=transformation.output_domain,
             input_metric=transformation.output_metric,
             noise_mechanism=mechanism,
             d_in=mid_stability,
-            d_out=self.budget.value,
+            d_out=self.adjusted_budget.value,
             output_measure=self.output_measure,
             groupby_transformation=groupby,
             count_column=expr.output_column,
         )
         self._validate_measurement(agg, mid_stability)
         return transformation | agg
 
     def visit_groupby_count_distinct(self, expr: GroupByCountDistinct) -> Measurement:
         """Create a measurement from a GroupByCountDistinct query expression."""
+        self._validate_approxDP_and_adjust_budget(expr)
         mechanism = self._pick_noise_for_count(expr)
         (
             child_transformation,
             child_ref,
             child_constraints,
         ) = self._visit_child_transformation(expr.child, mechanism)
         constrained_query = _generate_constrained_count_distinct(
@@ -699,15 +779,15 @@
         )
 
         agg = create_count_distinct_measurement(
             input_domain=transformation.output_domain,
             input_metric=transformation.output_metric,
             noise_mechanism=mechanism,
             d_in=mid_stability,
-            d_out=self.budget.value,
+            d_out=self.adjusted_budget.value,
             output_measure=self.output_measure,
             groupby_transformation=groupby,
             count_column=expr.output_column,
         )
         self._validate_measurement(agg, mid_stability)
         return transformation | agg
 
@@ -767,32 +847,41 @@
         groupby = self._build_groupby(
             transformation.output_domain,
             transformation.output_metric,
             expr.groupby_keys,
             self.default_mechanism,
         )
 
+        # For ApproxDP keep epsilon value, but always pass 0 for delta
+        self.adjusted_budget = (
+            ApproxDPBudget(self.budget.value[0], 0)
+            if isinstance(self.budget, ApproxDPBudget)
+            else self.budget
+        )
+
         agg = create_quantile_measurement(
             input_domain=transformation.output_domain,
             input_metric=transformation.output_metric,
             measure_column=expr.measure_column,
             quantile=expr.quantile,
             lower=expr.low,
             upper=expr.high,
             d_in=mid_stability,
-            d_out=self.budget.value,
+            d_out=self.adjusted_budget.value,
             output_measure=self.output_measure,
             groupby_transformation=groupby,
             quantile_column=expr.output_column,
         )
         self._validate_measurement(agg, mid_stability)
         return transformation | agg
 
     def visit_groupby_bounded_sum(self, expr: GroupByBoundedSum) -> Measurement:
         """Create a measurement from a GroupByBoundedSum query expression."""
+        self._validate_approxDP_and_adjust_budget(expr)
+
         # Peek at the schema, to see if there are errors there
         OutputSchemaVisitor(self.catalog).visit_groupby_bounded_sum(expr)
 
         info = self._build_common(expr)
         # _build_common already checks these;
         # these asserts are just for mypy's benefit
         assert isinstance(info.transformation.output_domain, SparkDataFrameDomain)
@@ -805,24 +894,26 @@
             input_domain=info.transformation.output_domain,
             input_metric=info.transformation.output_metric,
             measure_column=expr.measure_column,
             lower=info.lower_bound,
             upper=info.upper_bound,
             noise_mechanism=info.mechanism,
             d_in=info.mid_stability,
-            d_out=self.budget.value,
+            d_out=self.adjusted_budget.value,
             output_measure=self.output_measure,
             groupby_transformation=info.groupby,
             sum_column=expr.output_column,
         )
         self._validate_measurement(agg, info.mid_stability)
         return info.transformation | agg
 
     def visit_groupby_bounded_average(self, expr: GroupByBoundedAverage) -> Measurement:
         """Create a measurement from a GroupByBoundedAverage query expression."""
+        self._validate_approxDP_and_adjust_budget(expr)
+
         # Peek at the schema, to see if there are errors there
         OutputSchemaVisitor(self.catalog).visit_groupby_bounded_average(expr)
         info = self._build_common(expr)
         # _visit_child_transformation already raises an error if these aren't true
         # these are just here for MyPy's benefit
         assert isinstance(info.transformation.output_domain, SparkDataFrameDomain)
         assert isinstance(
@@ -834,26 +925,28 @@
             input_domain=info.transformation.output_domain,
             input_metric=info.transformation.output_metric,
             measure_column=expr.measure_column,
             lower=info.lower_bound,
             upper=info.upper_bound,
             noise_mechanism=info.mechanism,
             d_in=info.mid_stability,
-            d_out=self.budget.value,
+            d_out=self.adjusted_budget.value,
             output_measure=self.output_measure,
             groupby_transformation=info.groupby,
             average_column=expr.output_column,
         )
         self._validate_measurement(agg, info.mid_stability)
         return info.transformation | agg
 
     def visit_groupby_bounded_variance(
         self, expr: GroupByBoundedVariance
     ) -> Measurement:
         """Create a measurement from a GroupByBoundedVariance query expression."""
+        self._validate_approxDP_and_adjust_budget(expr)
+
         # Peek at the schema, to see if there are errors there
         OutputSchemaVisitor(self.catalog).visit_groupby_bounded_variance(expr)
         info = self._build_common(expr)
         # _visit_child_transformation already raises an error if these aren't true
         # these are just here for MyPy's benefit
         assert isinstance(info.transformation.output_domain, SparkDataFrameDomain)
         assert isinstance(
@@ -865,24 +958,26 @@
             input_domain=info.transformation.output_domain,
             input_metric=info.transformation.output_metric,
             measure_column=expr.measure_column,
             lower=info.lower_bound,
             upper=info.upper_bound,
             noise_mechanism=info.mechanism,
             d_in=info.mid_stability,
-            d_out=self.budget.value,
+            d_out=self.adjusted_budget.value,
             output_measure=self.output_measure,
             groupby_transformation=info.groupby,
             variance_column=expr.output_column,
         )
         self._validate_measurement(agg, info.mid_stability)
         return info.transformation | agg
 
     def visit_groupby_bounded_stdev(self, expr: GroupByBoundedSTDEV) -> Measurement:
         """Create a measurement from a GroupByBoundedStdev query expression."""
+        self._validate_approxDP_and_adjust_budget(expr)
+
         # Peek at the schema, to see if there are errors there
         OutputSchemaVisitor(self.catalog).visit_groupby_bounded_stdev(expr)
         info = self._build_common(expr)
         # _visit_child_transformation already raises an error if these aren't true
         # these are just here for MyPy's benefit
         assert isinstance(info.transformation.output_domain, SparkDataFrameDomain)
         assert isinstance(
@@ -894,15 +989,15 @@
             input_domain=info.transformation.output_domain,
             input_metric=info.transformation.output_metric,
             measure_column=expr.measure_column,
             lower=info.lower_bound,
             upper=info.upper_bound,
             noise_mechanism=info.mechanism,
             d_in=info.mid_stability,
-            d_out=self.budget.value,
+            d_out=self.adjusted_budget.value,
             output_measure=self.output_measure,
             groupby_transformation=info.groupby,
             standard_deviation_column=expr.output_column,
         )
 
         self._validate_measurement(agg, info.mid_stability)
         return info.transformation | agg
```

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py` & `tmlt_analytics-0.7.2/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,15 +298,15 @@
         input_schema = expr.child.accept(self)
         grouping_column = input_schema.grouping_column
         id_column = input_schema.id_column
         id_space = input_schema.id_space
         nonexistent_columns = set(expr.column_mapper) - set(input_schema)
         if nonexistent_columns:
             raise ValueError(
-                f"Nonexistent columns {nonexistent_columns} in rename query"
+                f"Nonexistent columns in rename query: {nonexistent_columns}"
             )
         for old, new in expr.column_mapper.items():
             if new in input_schema and new != old:
                 raise ValueError(
                     f"Cannot rename '{old}' to '{new}': column '{new}' already exists"
                 )
             if old == grouping_column:
@@ -384,15 +384,15 @@
             raise ValueError(
                 f"ID column '{id_column}' may not be dropped by select query"
             )
 
         nonexistent_columns = set(expr.columns) - set(input_schema)
         if nonexistent_columns:
             raise ValueError(
-                f"Nonexistent columns {nonexistent_columns} in select query."
+                f"Nonexistent columns in select query: {nonexistent_columns}"
             )
 
         return Schema(
             {column: input_schema[column] for column in expr.columns},
             grouping_column=grouping_column,
             id_column=id_column,
             id_space=input_schema.id_space,
@@ -684,27 +684,31 @@
             join_columns=expr.join_columns,
             join_id_space=input_schema.id_space,
         )
 
     def visit_replace_null_and_nan(self, expr: ReplaceNullAndNan) -> Schema:
         """Returns the resulting schema from evaluating a ReplaceNullAndNan."""
         input_schema = expr.child.accept(self)
-
         if (
             input_schema.grouping_column
             and input_schema.grouping_column in expr.replace_with
         ):
             raise ValueError(
                 "Cannot replace null values in column "
-                f"'{input_schema.grouping_column}', as it is a grouping column"
+                f"'{input_schema.grouping_column}', as it is a grouping column."
             )
         if input_schema.id_column and input_schema.id_column in expr.replace_with:
             raise ValueError(
                 f"Cannot replace null values in column '{input_schema.id_column}', "
-                "as it is an ID column"
+                "as it is an ID column."
+            )
+        if input_schema.id_column and (len(expr.replace_with) == 0):
+            raise RuntimeWarning(
+                f"Replacing null values in the ID column '{input_schema.id_column}' "
+                "is not allowed, so the ID column may still contain null values."
             )
 
         if len(expr.replace_with) != 0:
             pytypes = analytics_to_py_types(input_schema)
             for col, val in expr.replace_with.items():
                 if col not in input_schema.keys():
                     raise ValueError(
@@ -723,17 +727,16 @@
 
         columns_to_change = list(dict(expr.replace_with).keys())
         if len(columns_to_change) == 0:
             columns_to_change = [
                 col
                 for col in input_schema.column_descs.keys()
                 if (input_schema[col].allow_null or input_schema[col].allow_nan)
-                and not (col == input_schema.grouping_column)
+                and not (col in [input_schema.grouping_column, input_schema.id_column])
             ]
-
         return Schema(
             {
                 name: ColumnDescriptor(
                     column_type=cd.column_type,
                     allow_null=(cd.allow_null and not name in columns_to_change),
                     allow_nan=(cd.allow_nan and not name in columns_to_change),
                     allow_inf=cd.allow_inf,
@@ -799,45 +802,47 @@
             id_column=input_schema.id_column,
             id_space=input_schema.id_space,
         )
 
     def visit_drop_null_and_nan(self, expr: DropNullAndNan) -> Schema:
         """Returns the resulting schema from evaluating a DropNullAndNan."""
         input_schema = expr.child.accept(self)
-
         if (
             input_schema.grouping_column
             and input_schema.grouping_column in expr.columns
         ):
             raise ValueError(
                 f"Cannot drop null values in column '{input_schema.grouping_column}', "
                 "as it is a grouping column"
             )
         if input_schema.id_column and input_schema.id_column in expr.columns:
             raise ValueError(
                 f"Cannot drop null values in column '{input_schema.id_column}', "
-                "as it is an ID column"
+                "as it is an ID column."
+            )
+        if input_schema.id_column and len(expr.columns) == 0:
+            raise RuntimeWarning(
+                f"Replacing null values in the ID column '{input_schema.id_column}' "
+                "is not allowed, so the ID column may still contain null values."
             )
-
         columns = expr.columns.copy()
         if len(columns) == 0:
             columns = [
                 name
                 for name, cd in input_schema.column_descs.items()
                 if (cd.allow_null or cd.allow_nan)
-                and not name == input_schema.grouping_column
+                and not name in [input_schema.grouping_column, input_schema.id_column]
             ]
         else:
             for name in columns:
                 if name not in input_schema.keys():
                     raise ValueError(
                         f"Column '{name}' does not exist in this table, "
                         f"available columns are {list(input_schema.keys())}"
                     )
-
         return Schema(
             {
                 name: ColumnDescriptor(
                     column_type=cd.column_type,
                     allow_null=(cd.allow_null and not name in columns),
                     allow_nan=(cd.allow_nan and not name in columns),
                     allow_inf=(cd.allow_inf),
```

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/_query_expr_compiler/_transformation_visitor.py` & `tmlt_analytics-0.7.2/tmlt/analytics/_query_expr_compiler/_transformation_visitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,24 +257,28 @@
                 "please let us know about it so we can fix it!"
             )
 
     def inner_metric(self) -> Union[SumOf, RootSumOfSquared]:
         """Get the inner metric used by this TransformationVisitor."""
         if self.mechanism in (NoiseMechanism.LAPLACE, NoiseMechanism.GEOMETRIC):
             return SumOf(SymmetricDifference())
-        else:
-            if self.mechanism != NoiseMechanism.DISCRETE_GAUSSIAN:
-                raise RuntimeError(
-                    f"Unsupported mechanism {self.mechanism}. "
-                    "Supported mechanisms are "
-                    f"{NoiseMechanism.DISCRETE_GAUSSIAN}, "
-                    f"{NoiseMechanism.LAPLACE}, and"
-                    f"{NoiseMechanism.GEOMETRIC}."
-                )
+        elif self.mechanism in (
+            NoiseMechanism.DISCRETE_GAUSSIAN,
+            NoiseMechanism.GAUSSIAN,
+        ):
             return RootSumOfSquared(SymmetricDifference())
+        else:
+            raise RuntimeError(
+                f"Unsupported mechanism {self.mechanism}. "
+                "Supported mechanisms are "
+                f"{NoiseMechanism.GAUSSIAN},"
+                f"{NoiseMechanism.DISCRETE_GAUSSIAN}, "
+                f"{NoiseMechanism.LAPLACE}, and"
+                f"{NoiseMechanism.GEOMETRIC}."
+            )
 
     def _visit_child(self, child: QueryExpr) -> Output:
         """Visit a child query and raise assertion errors if needed."""
         transformation, reference, constraints = child.accept(self)
         if not isinstance(transformation, Transformation):
             raise AssertionError(
                 "Child query did not create a transformation. "
@@ -371,14 +375,19 @@
                     "please let us know about it so we can fix it!"
                 )
             if not isinstance(input_metric, (SymmetricDifference, IfGroupedBy)):
                 raise AssertionError(
                     "Unrecognized input metric. This is probably a bug; "
                     "please let us know about it so we can fix it!"
                 )
+            nonexistent_columns = set(expr.column_mapper) - set(input_domain.schema)
+            if nonexistent_columns:
+                raise ValueError(
+                    f"Nonexistent columns in rename query: {nonexistent_columns}"
+                )
             return create_copy_and_transform_value(
                 parent_domain,
                 parent_metric,
                 child_ref.identifier,
                 target,
                 RenameTransformation(input_domain, input_metric, expr.column_mapper),
                 lambda *args: None,
@@ -468,14 +477,19 @@
             if not isinstance(
                 input_metric, (IfGroupedBy, SymmetricDifference, HammingDistance)
             ):
                 raise AssertionError(
                     "Unrecognized input metric. This is probably a bug; "
                     "please let us know about it so we can fix it!"
                 )
+            nonexistent_columns = set(expr.columns) - set(input_domain.schema)
+            if nonexistent_columns:
+                raise ValueError(
+                    f"Nonexistent columns in select query: {nonexistent_columns}"
+                )
             return create_copy_and_transform_value(
                 parent_domain,
                 parent_metric,
                 child_ref.identifier,
                 target,
                 SelectTransformation(input_domain, input_metric, expr.columns),
                 lambda *args: None,
@@ -1184,31 +1198,20 @@
         )
         input_domain = lookup_domain(child_transformation.output_domain, child_ref)
         input_metric = lookup_metric(child_transformation.output_metric, child_ref)
         analytics_schema = Schema(
             spark_dataframe_domain_to_analytics_columns(input_domain)
         )
 
-        grouping_column: Optional[str] = None
-        if isinstance(input_metric, IfGroupedBy):
-            grouping_column = input_metric.column
-            if grouping_column in expr.columns:
-                raise ValueError(
-                    "Cannot drop infinite values in column"
-                    f" {input_metric.column}, because it is being used as a"
-                    " grouping column"
-                )
-
         columns = expr.columns.copy()
         if len(columns) == 0:
             columns = [
                 col
                 for col, cd in analytics_schema.column_descs.items()
                 if (cd.column_type == ColumnType.DECIMAL and cd.allow_inf)
-                and not (col == grouping_column)
             ]
         else:
             for col in columns:
                 if analytics_schema.column_descs[col].column_type != ColumnType.DECIMAL:
                     raise ValueError(
                         f"Cannot drop infinite values from column {col}, because that"
                         " column's type is not DECIMAL"
@@ -1260,19 +1263,19 @@
     def visit_drop_null_and_nan(self, expr: DropNullAndNan) -> Output:
         """Create a transformation from a DropNullAndNan query expression."""
         child_transformation, child_ref, child_constraints = self._ensure_not_hamming(
             *self._visit_child(expr.child)
         )
         input_domain = lookup_domain(child_transformation.output_domain, child_ref)
         input_metric = lookup_metric(child_transformation.output_metric, child_ref)
-
         analytics_schema = Schema(
             spark_dataframe_domain_to_analytics_columns(input_domain)
         )
 
+        # TODO(2702): This should be supported for IDs tables
         grouping_column: Optional[str] = None
         if isinstance(input_metric, IfGroupedBy):
             grouping_column = input_metric.column
             if grouping_column in expr.columns:
                 raise ValueError(
                     "Cannot drop null values in column"
                     f" {input_metric.column}, because it is being used as a"
```

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/_schema.py` & `tmlt_analytics-0.7.2/tmlt/analytics/_schema.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/_table_identifier.py` & `tmlt_analytics-0.7.2/tmlt/analytics/_table_identifier.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/_table_reference.py` & `tmlt_analytics-0.7.2/tmlt/analytics/_table_reference.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/_transformation_utils.py` & `tmlt_analytics-0.7.2/tmlt/analytics/_transformation_utils.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/binning_spec.py` & `tmlt_analytics-0.7.2/tmlt/analytics/binning_spec.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
 
 import bisect
 import datetime
 import math
-from typing import Any, Generic, List, Optional, Sequence, TypeVar, cast
+from typing import Any, Generic, List, Optional, Sequence, TypeVar, Union, cast
 
 from tmlt.core.utils.type_utils import get_element_type
 
 from tmlt.analytics._schema import ColumnDescriptor, ColumnType, column_type_to_py_type
 
-BinT = TypeVar("BinT", str, int, float, datetime.date, datetime.datetime)
+BinT = TypeVar("BinT", str, Union[int, float], datetime.date, datetime.datetime)
 BinNameT = TypeVar("BinNameT", str, int, float, datetime.date, datetime.datetime)
 
 
 def _get_column_descriptor(
     bin_names: Sequence[Any], nan_bin: Optional[BinNameT]
 ) -> ColumnDescriptor:
     """Return the ColumnDescriptor for the non-``None`` elements of a list.
@@ -74,14 +74,17 @@
         elif any(e.second for e in bin_edges):  # type: ignore
             timespec = "seconds"
         else:
             timespec = "minutes"
         return [
             e.isoformat(sep=" ", timespec=timespec) for e in bin_edges  # type: ignore
         ]
+    elif isinstance(bin_edges[0], str):
+        # Use repr for strings so that they get quoted.
+        return [repr(e) for e in bin_edges]
     else:
         return [str(e) for e in bin_edges]
 
 
 def _default_bin_names(
     bin_edges: List[BinT], right: bool, include_edges: bool
 ) -> List[str]:
@@ -111,23 +114,21 @@
             ]
 
 
 class BinningSpec(Generic[BinT, BinNameT]):
     """A spec object defining an operation where values are assigned to bins.
 
     A BinningSpec divides values into bins based on a list of bin edges, for use
-    with the :meth:`~tmlt.analytics.query_builder.QueryBuilder.bin_column`
-    method. All :data:`supported data types
-    <tmlt.analytics.session.SUPPORTED_SPARK_TYPES>` can be binned using a
-    BinningSpec.
-
-    Values outside the range of the provided bins, ``None`` types,
-    and NaN values are all mapped to ``None`` (``null`` in Spark).
-    Bin names are generated based on the bin edges, but custom names can be provided.
-
+    with the :meth:`~tmlt.analytics.query_builder.QueryBuilder.bin_column` method.
+    All :data:`supported data types <tmlt.analytics.session.SUPPORTED_SPARK_TYPES>`
+    can be binned using a BinningSpec.
+
+    Values outside the range of the provided bins and ``None`` types are all
+    mapped to ``None`` (``null`` in Spark), as are NaN values by default. Bin
+    names are generated based on the bin edges, but custom names can be provided.
 
     Examples:
         >>> spec = BinningSpec([0,5,10])
         >>> spec.bins()
         ['[0, 5]', '(5, 10]']
         >>> spec(0)
         '[0, 5]'
@@ -233,15 +234,15 @@
 
         The returned list is guaranteed to contain unique elements, even if
         multiple bins were mapped to the same name. The NaN bin, if one was
         specified, is included. If ``include_null`` is true, the null bin is
         included as well; by default, it is not included.
         """
         names = cast(List[Optional[BinNameT]], list(self._bin_names))
-        if self._input_type == ColumnType.DECIMAL and self._nan_bin is not None:
+        if self._nan_bin is not None:
             names.append(self._nan_bin)
         if include_null:
             names.append(None)
         # This conversion is a trick to deduplicate values in `names` while
         # preserving the order in which they first appeared.
         return list(dict.fromkeys(names))
```

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/constraints/_base.py` & `tmlt_analytics-0.7.2/tmlt/analytics/constraints/_base.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/constraints/_simplify.py` & `tmlt_analytics-0.7.2/tmlt/analytics/constraints/_simplify.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/constraints/_truncation.py` & `tmlt_analytics-0.7.2/tmlt/analytics/constraints/_truncation.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/keyset.py` & `tmlt_analytics-0.7.2/tmlt/analytics/keyset.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/privacy_budget.py` & `tmlt_analytics-0.7.2/tmlt/analytics/privacy_budget.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,20 +110,21 @@
         return _to_int_or_float(self._epsilon)
 
     def __repr__(self) -> str:
         """Returns string representation of this PureDPBudget."""
         return f"PureDPBudget(epsilon={self.epsilon})"
 
     def __eq__(self, other) -> bool:
-        """Returns whether or not a PureDPBudget are equivalent to another PrivacyBudget.
+        """Returns whether or not a PureDPBudget is equivalent to another PrivacyBudget.
 
-        PureDPBudgets are considered equal to ApproxDPBudgets that have delta of 0, and the same epsilon.
+        PureDPBudgets are considered equal to ApproxDPBudgets that have delta of 0 and
+        the same epsilon.
         """
         if isinstance(other, PureDPBudget):
-            return self.value == other.value
+            return self._epsilon == other._epsilon
         if isinstance(other, ApproxDPBudget):
             if self._epsilon == other._epsilon and other._delta == 0:
                 return True
         return False
 
 
 class ApproxDPBudget(PrivacyBudget):
@@ -191,15 +192,15 @@
         a computation, you should use self.value[1] instead.
         """
         return _to_int_or_float(self._delta)
 
     @property
     def is_infinite(self) -> bool:
         """Returns true if epsilon is float('inf') or delta is 1."""
-        return self.epsilon == float("inf") or self.delta == 1
+        return self._epsilon == float("inf") or self._delta == 1
 
     def __repr__(self) -> str:
         """Returns the string representation of this ApproxDPBudget."""
         return f"ApproxDPBudget(epsilon={self.epsilon}, delta={self.delta})"
 
     def __eq__(self, other) -> bool:
         """Returns whether an ApproxDPBudget is equivalent to another privacy budget.
@@ -256,14 +257,19 @@
         """Returns the value of rho as an int or float.
 
         This is helpful for human readability. If you need to use the rho value in
         a computation, you should use self.value instead.
         """
         return _to_int_or_float(self._rho)
 
+    @property
+    def is_infinite(self) -> bool:
+        """Returns true if rho is float('inf')."""
+        return self._rho == float("inf")
+
     def __repr__(self) -> str:
         """Returns string representation of this RhoZCDPBudget."""
         return f"RhoZCDPBudget(rho={self.rho})"
 
     def __eq__(self, other) -> bool:
         """Returns whether or not two RhoZCDPBudgets are equivalent."""
         if isinstance(other, RhoZCDPBudget):
```

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/protected_change.py` & `tmlt_analytics-0.7.2/tmlt/analytics/protected_change.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/query_builder.py` & `tmlt_analytics-0.7.2/tmlt/analytics/query_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,14 +403,21 @@
         self,
         replace_with: Optional[
             Mapping[str, Union[int, float, str, datetime.date, datetime.datetime]]
         ] = None,
     ) -> "QueryBuilder":
         """Updates the current query to replace null and NaN values in some columns.
 
+        .. note::
+            Null values *cannot* be replaced in the ID column of a table initialized
+            with a :class:`~tmlt.analytics.protected_change.AddRowsWithID`
+            :class:`~tmlt.analytics.protected_change.ProtectedChange`, nor on a column
+            generated by a :meth:`~tmlt.analytics.query_builder.QueryBuilder.flat_map`
+            with the grouping parameter set to True.
+
         .. warning::
             If null values are replaced in a column, then Analytics will raise
             an error if you use a KeySet with a null value for that column.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
             >>> import tmlt.analytics.session
@@ -558,14 +565,21 @@
             child=self.query_expr, replace_with=replace_with
         )
         return self
 
     def drop_null_and_nan(self, columns: Optional[List[str]]) -> "QueryBuilder":
         """Updates the current query to drop rows containing null or NaN values.
 
+        .. note::
+            Null values *cannot* be dropped in the ID column of a table initialized
+            with a :class:`~tmlt.analytics.protected_change.AddRowsWithID`
+            :class:`~tmlt.analytics.protected_change.ProtectedChange`, nor on a column
+            generated by a :meth:`~tmlt.analytics.query_builder.QueryBuilder.flat_map`
+            with the grouping parameter set to True.
+
         .. warning::
             If null and NaN values are dropped from a column, then Analytics will
             raise an error if you use a :class:`~tmlt.analytics.keyset.KeySet`
             that contains a null value for that column.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
@@ -1322,14 +1336,60 @@
     def enforce(self, constraint: Constraint) -> "QueryBuilder":
         """Enforce a :mod:`~tmlt.analytics.constraints.Constraint` on the current table.
 
         This method can be used to enforce constraints on the current table. See
         the :mod:`~tmlt.analytics.constraints` module for information about the
         available constraints and what they are used for.
 
+        ..
+            >>> from tmlt.analytics.query_builder import QueryBuilder
+            >>> from tmlt.analytics.privacy_budget import PureDPBudget
+            >>> from tmlt.analytics.session import Session
+            >>> from tmlt.analytics.protected_change import AddRowsWithID
+            >>> from tmlt.analytics.constraints import MaxRowsPerID
+            >>> import pandas as pd
+            >>> from pyspark.sql import SparkSession
+            >>> spark = SparkSession.builder.getOrCreate()
+            >>> my_private_data = spark.createDataFrame(
+            ...     pd.DataFrame(
+            ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]],
+            ...         columns=["id", "B", "X"]
+            ...     )
+            ... )
+
+        Example:
+            >>> my_private_data.toPandas()
+              id  B  X
+            0  0  1  0
+            1  1  0  1
+            2  1  2  1
+            >>> sess = (
+            ...     Session.Builder()
+            ...     .with_privacy_budget(PureDPBudget(float("inf")))
+            ...     .with_id_space("a")
+            ...     .with_private_dataframe(
+            ...         "my_private_data",
+            ...         my_private_data,
+            ...         protected_change=AddRowsWithID("id", "a"),
+            ...     )
+            ...     .build()
+            ... )
+            >>> # No ID contributes more than 2 rows, so no rows are dropped when
+            >>> # enforcing the constraint
+            >>> query = QueryBuilder("my_private_data").enforce(MaxRowsPerID(2)).count()
+            >>> sess.evaluate(query, sess.remaining_privacy_budget).toPandas()
+               count
+            0      3
+            >>> # ID 1 contributes more than one row, so one of the rows with ID 1 will
+            >>> # be dropped when enforcing the constraint
+            >>> query = QueryBuilder("my_private_data").enforce(MaxRowsPerID(1)).count()
+            >>> sess.evaluate(query, sess.remaining_privacy_budget).toPandas()
+               count
+            0      2
+
         Args:
             constraint: The constraint to enforce.
         """
         self._query_expr = EnforceConstraint(self._query_expr, constraint, options={})
         return self
 
     def groupby(self, keys: KeySet) -> "GroupedQueryBuilder":
```

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/query_expr.py` & `tmlt_analytics-0.7.2/tmlt/analytics/query_expr.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,16 +80,16 @@
     might change over time as additional optimizations are added to the library.
     """
     LAPLACE = auto()
     """Laplace and/or double-sided geometric noise is used, depending on the
     column type.
     """
     GAUSSIAN = auto()
-    """The discrete Gaussian mechanism is used for integer sums. Not compatible
-    with floating-point sums or pure DP.
+    """Discrete and/or continuous Gaussian noise is used, depending on the column type.
+    Not compatible with pure DP.
     """
 
 
 class AverageMechanism(Enum):
     """Possible mechanisms for the average() aggregation.
 
     Currently, the
@@ -102,16 +102,16 @@
     might change over time as additional optimizations are added to the library.
     """
     LAPLACE = auto()
     """Laplace and/or double-sided geometric noise is used, depending on the
     column type.
     """
     GAUSSIAN = auto()
-    """The discrete Gaussian mechanism is used for integer averages. Not
-    compatible with floating-point averages or pure DP.
+    """Discrete and/or continuous Gaussian noise is used, depending on the column type.
+    Not compatible with pure DP.
     """
 
 
 class VarianceMechanism(Enum):
     """Possible mechanisms for the variance() aggregation.
 
     Currently, the
@@ -124,16 +124,16 @@
     might change over time as additional optimizations are added to the library.
     """
     LAPLACE = auto()
     """Laplace and/or double-sided geometric noise is used, depending on the
     column type.
     """
     GAUSSIAN = auto()
-    """The discrete Gaussian mechanism is used for integer variance. Not
-    compatible with floating-point averages or pure DP.
+    """Discrete and/or continuous Gaussian noise is used, depending on the column type.
+    Not compatible with pure DP.
     """
 
 
 class StdevMechanism(Enum):
     """Possible mechanisms for the stdev() aggregation.
 
     Currently, the
@@ -146,16 +146,16 @@
     might change over time as additional optimizations are added to the library.
     """
     LAPLACE = auto()
     """Laplace and/or double-sided geometric noise is used, depending on the
     column type.
     """
     GAUSSIAN = auto()
-    """The discrete Gaussian mechanism is used for integer stdev. Not compatible
-    with floating-point averages or pure DP.
+    """Discrete and/or continuous Gaussian noise is used, depending on the column type.
+    Not compatible with pure DP.
     """
 
 
 class QueryExpr(ABC):
     """A query expression, base class for relational operators.
 
     In most cases, QueryExpr should not be manipulated directly, but rather
```

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/session.py` & `tmlt_analytics-0.7.2/tmlt/analytics/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 More details on the exact privacy promise provided by :class:`Session` can be
 found in the :ref:`Privacy promise topic guide <Privacy promise>`.
 """
 
 # Copyright Tumult Labs 2023
 # SPDX-License-Identifier: Apache-2.0
+
 from operator import xor
 from typing import Any, Dict, List, NamedTuple, Optional, Tuple, Union, cast
 from warnings import warn
 
 import pandas as pd  # pylint: disable=unused-import
 import sympy as sp
 from pyspark.sql import SparkSession  # pylint: disable=unused-import
@@ -159,14 +160,107 @@
                 f"Unsupported ProtectedChange type: {type(protected_change)}"
             )
     for identifier, table_to_key_column in protected_ids_dict.items():
         relations.append(AddRemoveKeys(identifier, table_to_key_column))
     return Conjunction(relations)
 
 
+# TODO(2476): Uncomment this once we allow consuming delta, and remove the part
+# that only reports epsilon (immediately after the commented section).
+def _format_insufficient_budget_msg(
+    requested_budget: Union[ExactNumber, Tuple[ExactNumber, ExactNumber]],
+    remaining_budget: Union[ExactNumber, Tuple[ExactNumber, ExactNumber]],
+    privacy_budget: PrivacyBudget,
+) -> str:
+    """Format message for InsufficientBudgetError."""
+    output = ""
+
+    if isinstance(privacy_budget, ApproxDPBudget):
+        if is_exact_number_tuple(requested_budget) and is_exact_number_tuple(
+            remaining_budget
+        ):
+            assert isinstance(requested_budget, tuple)
+            assert isinstance(remaining_budget, tuple)
+            remaining_epsilon = remaining_budget[0].to_float(round_up=True)
+            requested_epsilon = requested_budget[0].to_float(round_up=True)
+            #   requested_delta = requested_budget[1].to_float(round_up=True)
+            #   remaining_delta = remaining_budget[1].to_float(round_up=True)
+            #   output += f"\nRequested: ε={requested_epsilon:.3f},"
+            #   output += f" δ={requested_delta:.3f}"
+            #   output += f"\nRemaining: ε={remaining_epsilon:.3f},"
+            #   output += f" δ={remaining_delta:.3f}"
+            #   output += "\nDifference: "
+            #   lacks_epsilon = remaining_epsilon < requested_epsilon
+            #   lacks_delta = remaining_delta < requested_delta
+            #   if lacks_epsilon and lacks_delta:
+            #       eps_diff = abs(remaining_epsilon - requested_epsilon)
+            #       delta_diff = abs(remaining_delta - requested_delta)
+            #       if eps_diff >= 0.1 and delta_diff >= 0.1:
+            #           output += f"ε={eps_diff:.3f}, δ={delta_diff:.3f}"
+            #       elif eps_diff < 0.1:
+            #           output += f"ε={eps_diff:.3e}, δ={delta_diff:.3f}"
+            #       elif delta_diff < 0.1:
+            #           output += f"ε={eps_diff:.3f}, δ={delta_diff:.3e}"
+            #   elif lacks_epsilon:
+            #       eps_diff = abs(remaining_epsilon - requested_epsilon)
+            #       if eps_diff >= 0.1:
+            #           output += f"ε={eps_diff:.3f}"
+            #       else:
+            #           output += f"ε={eps_diff:.3e}"
+            #   elif lacks_delta:
+            #       delta_diff = abs(remaining_delta - requested_delta)
+            #       if delta_diff >= 0.1:
+            #           output += f"δ={delta_diff:.3f}"
+            #       else:
+            #           output += f"δ={delta_diff:.3e}"
+            approx_diff = abs(remaining_epsilon - requested_epsilon)
+            output += f"\nRequested: ε={requested_epsilon:.3f}"
+            output += f"\nRemaining: ε={remaining_epsilon:.3f}"
+            if approx_diff >= 0.1:
+                output += f"\nDifference: ε={approx_diff:.3f}"
+            else:
+                output += f"\nDifference: ε={approx_diff:.3e}"
+        else:
+            raise AssertionError(
+                "Unable to convert privacy budget of type"
+                f" {type(privacy_budget)} to float or floats. This is"
+                " probably a bug; please let us know about it so we can fix it!"
+            )
+    elif isinstance(privacy_budget, (PureDPBudget, RhoZCDPBudget)):
+        assert isinstance(requested_budget, ExactNumber)
+        assert isinstance(remaining_budget, ExactNumber)
+        if isinstance(privacy_budget, PureDPBudget):
+            remaining_epsilon = remaining_budget.to_float(round_up=True)
+            requested_epsilon = requested_budget.to_float(round_up=True)
+            approx_diff = abs(remaining_epsilon - requested_epsilon)
+            output += f"\nRequested: ε={requested_epsilon:.3f}"
+            output += f"\nRemaining: ε={remaining_epsilon:.3f}"
+            if approx_diff >= 0.1:
+                output += f"\nDifference: ε={approx_diff:.3f}"
+            else:
+                output += f"\nDifference: ε={approx_diff:.3e}"
+        elif isinstance(privacy_budget, RhoZCDPBudget):
+            remaining_rho = remaining_budget.to_float(round_up=True)
+            requested_rho = requested_budget.to_float(round_up=True)
+            approx_diff = abs(remaining_rho - requested_rho)
+            output += f"\nRequested: 𝝆={requested_rho:.3f}"
+            output += f"\nRemaining: 𝝆={remaining_rho:.3f}"
+            if approx_diff >= 0.1:
+                output += f"\nDifference: 𝝆={approx_diff:.3f}"
+            else:
+                output += f"\nDifference: 𝝆={approx_diff:.3e}"
+    else:
+        raise AssertionError(
+            f"Unsupported budget types: {type(requested_budget)},"
+            f" {type(remaining_budget)}. This is probably a bug, please let us know"
+            " about it so we can fix it!"
+        )
+    return output
+
+
 class Session:
     """Allows differentially private query evaluation on sensitive data.
 
     Sessions should not be directly constructed. Instead, they should be created
     using :meth:`from_dataframe` or with a :class:`Builder`.
     """
 
@@ -550,15 +644,18 @@
                 )
             else:
                 warn(
                     "The use of ApproxDP is not yet fully supported. Your session"
                     " will be initialized with PureDP using the epsilon provided.",
                     UserWarning,
                 )
-                sympy_budget = (privacy_budget._epsilon.expr, 0)
+                sympy_budget = (
+                    privacy_budget._epsilon.expr,
+                    privacy_budget._delta.expr,
+                )
         elif isinstance(privacy_budget, RhoZCDPBudget):
             output_measure = RhoZCDP()
             sympy_budget = privacy_budget._rho.expr
         # pylint: enable=protected-access
         else:
             raise ValueError(
                 f"Unsupported PrivacyBudget variant: {type(privacy_budget)}"
@@ -662,14 +759,54 @@
         will describe the table that would result from that query if it were
         applied to the Session.
 
         If ``obj`` is a string, ``session.describe(obj)`` will describe the table
         with that name. This is a shorthand for
         ``session.describe(QueryBuilder(obj))``.
 
+        ..
+            >>> # Set up data
+            >>> spark = SparkSession.builder.getOrCreate()
+            >>> spark_data = spark.createDataFrame(
+            ...     pd.DataFrame(
+            ...         [["0", 1, 0], ["1", 0, 1], ["1", 2, 1]], columns=["A", "B", "X"]
+            ...     )
+            ... )
+            >>> # construct session
+            >>> sess = Session.from_dataframe(
+            ...     PureDPBudget(1),
+            ...     "my_private_data",
+            ...     spark_data,
+            ...     protected_change=AddOneRow(),
+            ... )
+
+        Examples:
+            >>> # describe a session, "sess"
+            >>> sess.describe() # doctest: +NORMALIZE_WHITESPACE
+            The session has a remaining privacy budget of PureDPBudget(epsilon=1).
+            The following private tables are available:
+            Table 'my_private_data' (no constraints):
+                Columns:
+                    - 'A'  VARCHAR
+                    - 'B'  INTEGER
+                    - 'X'  INTEGER
+            >>> # describe a query object
+            >>> query = QueryBuilder("my_private_data").drop_null_and_nan(["B", "X"])
+            >>> sess.describe(query) # doctest: +NORMALIZE_WHITESPACE
+            Columns:
+                - 'A'  VARCHAR
+                - 'B'  INTEGER, not null
+                - 'X'  INTEGER, not null
+            >>> # describe a table by name
+            >>> sess.describe("my_private_data") # doctest: +NORMALIZE_WHITESPACE
+            Columns:
+                - 'A'  VARCHAR
+                - 'B'  INTEGER
+                - 'X'  INTEGER
+
         Args:
             obj: The table or query to be described, or None to describe the
                 whole Session.
         """
         if obj is None:
             self._describe_self()
         elif isinstance(obj, QueryExpr):
@@ -751,19 +888,41 @@
             if len(public_table_descs) != 0:
                 out.append(
                     "The following public tables are available:\n"
                     + "\n".join(public_table_descs)
                 )
         print("\n".join(out))
 
-    def _describe_query(self, query: QueryExpr):
+    def _describe_query(self, query_expr: QueryExpr):
         """Describe the output schema of a query and the constraints on it."""
-        schema = self._compiler.query_schema(query, self._catalog)
-        out = _describe_schema(schema)
-        print("\n".join(out))
+        schema = self._compiler.query_schema(query_expr, self._catalog)
+        schema_desc = _describe_schema(schema)
+        constraints: Optional[List[Constraint]] = None
+        try:
+            constraints = self._compiler.build_transformation(
+                query=query_expr,
+                input_domain=self._input_domain,
+                input_metric=self._input_metric,
+                public_sources=self._public_sources,
+                catalog=self._catalog,
+                table_constraints=self._table_constraints,
+            )[2]
+        except NotImplementedError:
+            # If the query results in a measurement, this will happen.
+            # There are no constraints on measurements, so we can just
+            # pass the schema description through.
+            pass
+        description = "\n".join(schema_desc)
+        if not constraints:
+            print(description)
+        else:
+            description += "\n\tConstraints:\n"
+            constraints_strs = [f"\t\t- {e}" for e in constraints]
+            description += "\n".join(constraints_strs)
+            print(description)
 
     @typechecked
     def get_schema(self, source_id: str) -> Schema:
         """Returns the schema for any data source.
 
         This includes information on whether the columns are nullable.
 
@@ -975,15 +1134,15 @@
         check_type("query_expr", query_expr, QueryExpr)
         check_type("privacy_budget", privacy_budget, PrivacyBudget)
 
         is_approxDP_session = self._accountant.output_measure == ApproxDP()
 
         # If pureDP session, and approxDP budget, let Core handle the error.
         if is_approxDP_session and isinstance(privacy_budget, PureDPBudget):
-            privacy_budget = ApproxDPBudget(privacy_budget.epsilon, 0)
+            privacy_budget = ApproxDPBudget(privacy_budget.value, 0)
 
         self._validate_budget_type_matches_session(privacy_budget)
         if privacy_budget in [PureDPBudget(0), ApproxDPBudget(0, 0), RhoZCDPBudget(0)]:
             raise ValueError("You need a non-zero privacy budget to evaluate a query.")
 
         adjusted_budget = self._process_requested_budget(privacy_budget)
 
@@ -1121,63 +1280,23 @@
                     " *not* produce similar outputs. This is probably a bug; please let"
                     " us know about it so we can fix it!"
                 )
             try:
                 answers = self._accountant.measure(
                     measurement, d_out=adjusted_budget.value
                 )
-            # TODO #2476: Parse InsufficientBudgetError based on budget type
-            except InsufficientBudgetError as e:
-                # pylint: disable=protected-access
-                if isinstance(adjusted_budget, (PureDPBudget)):
-                    approximate_budget_needed = adjusted_budget._epsilon
-                elif isinstance(adjusted_budget, (ApproxDPBudget)):
-                    approximate_budget_needed = adjusted_budget._epsilon
-                elif isinstance(adjusted_budget, RhoZCDPBudget):
-                    approximate_budget_needed = adjusted_budget._rho
-                # pylint: enable=protected-access
-                else:
-                    raise AssertionError(
-                        "Unable to convert privacy budget of"
-                        f" {adjusted_budget} to float or floats. This"
-                        " is probably a bug; please let us know about it so we can"
-                        " fix it!"
-                    ) from e
-
-                # mypy doesn't know we just checked for Tuple[ExactNumber, ExactNumber]
-                if is_exact_number_tuple(self._accountant.privacy_budget):
-                    # pylint: disable=line-too-long
-                    approximate_budget_left = self._accountant.privacy_budget[0]  # type: ignore
-                elif isinstance(self._accountant.privacy_budget, ExactNumber):
-                    approximate_budget_left = self._accountant.privacy_budget
-                else:
-                    raise AssertionError(
-                        "Unable to convert privacy budget of"
-                        f" {self._accountant.privacy_budget} to float or floats. This"
-                        " is probably a bug; please let us know about it so we can"
-                        " fix it!"
-                    ) from e
-
-                approximate_diff = abs(
-                    approximate_budget_left - approximate_budget_needed
-                ).to_float(round_up=False)
-                readable_approximate_budget_needed = approximate_budget_needed.to_float(
-                    round_up=False
+            except InsufficientBudgetError as err:
+                msg = _format_insufficient_budget_msg(
+                    err.requested_budget, err.remaining_budget, privacy_budget
                 )
-                readable_approximate_budget_left = approximate_budget_left.to_float(
-                    round_up=False
-                )
-
                 raise RuntimeError(
-                    "Cannot answer query without exceeding privacy budget: it needs"
-                    f" approximately {readable_approximate_budget_needed:.3f}, but the"
-                    " remaining budget is approximately"
-                    f" {readable_approximate_budget_left:.3f} (difference:"
-                    f" {approximate_diff:.3e})"
-                ) from e
+                    "Cannot answer query without exceeding the Session privacy budget."
+                    + msg
+                ) from err
+
             if len(answers) != 1:
                 raise AssertionError(
                     "Expected exactly one answer, but got "
                     f"{len(answers)} answers instead. This is "
                     "probably a bug; please let us know about it so "
                     "we can fix it!"
                 )
@@ -1438,24 +1557,33 @@
                 "Unable to convert privacy budget of type"
                 f" {type(self._accountant.privacy_budget)} to float or floats. This is"
                 " probably a bug; please let us know about it so we can fix it!"
             )
 
         is_approxDP_session = isinstance(self._accountant.output_measure, ApproxDP)
         if is_approxDP_session and isinstance(privacy_budget, PureDPBudget):
-            privacy_budget = ApproxDPBudget(privacy_budget.epsilon, 0)
+            privacy_budget = ApproxDPBudget(privacy_budget.value, 0)
 
         self._validate_budget_type_matches_session(privacy_budget)
         self._activate_accountant()
 
         transformation: Transformation = Identity(
             domain=self._input_domain, metric=self._input_metric
         )
         table_ref = find_reference(source_id, self._input_domain)
-        assert isinstance(table_ref, TableReference)
+        if table_ref is None:
+            if source_id in self.public_sources:
+                raise ValueError(
+                    f"Table '{source_id}' is a public table, which cannot have an "
+                    "ID space."
+                )
+            raise KeyError(
+                f"Private table '{source_id}' does not exist. "
+                f"Available private tables are: {', '.join(self.private_sources)}"
+            )
 
         # Either DictMetric or AddRemoveKeys
         parent_metric = lookup_metric(self._input_metric, table_ref.parent)
         table_has_ids: bool = isinstance(parent_metric, AddRemoveKeysMetric)
         if table_has_ids:
             parent_last_element = table_ref.parent.identifier
             constraints = self._table_constraints.get(NamedTable(source_id))
@@ -1573,62 +1701,22 @@
         except InactiveAccountantError as e:
             raise RuntimeError(
                 "This session is no longer active. Either it was manually stopped"
                 "with session.stop(), or it was stopped indirectly by the "
                 "activity of other sessions. See partition_and_create "
                 "for more information."
             ) from e
-        # TODO #2476: Parse InsufficientBudgetError based on budget type
-        except InsufficientBudgetError as e:
-            # pylint: disable=protected-access
-            if isinstance(adjusted_budget, (PureDPBudget)):
-                approximate_budget_needed = adjusted_budget._epsilon
-            elif isinstance(adjusted_budget, (ApproxDPBudget)):
-                approximate_budget_needed = adjusted_budget._epsilon
-            elif isinstance(adjusted_budget, RhoZCDPBudget):
-                approximate_budget_needed = adjusted_budget._rho
-            # pylint: enable=protected-access
-            else:
-                raise AssertionError(
-                    "Unable to convert privacy budget of"
-                    f" {adjusted_budget} to float or floats. This"
-                    " is probably a bug; please let us know about it so we can"
-                    " fix it!"
-                ) from e
-            # mypy doesn't know we just checked for Tuple[ExactNumber, ExactNumber]
-            if is_exact_number_tuple(self._accountant.privacy_budget):
-                # pylint: disable-next=line-too-long
-                approximate_budget_left = self._accountant.privacy_budget[0]  # type: ignore
-            elif isinstance(self._accountant.privacy_budget, ExactNumber):
-                approximate_budget_left = self._accountant.privacy_budget
-            else:
-                raise AssertionError(
-                    "Unable to convert privacy budget of"
-                    f" {self._accountant.privacy_budget} to float or floats. This"
-                    " is probably a bug; please let us know about it so we can"
-                    " fix it!"
-                ) from e
-
-            approximate_diff = abs(
-                approximate_budget_left - approximate_budget_needed
-            ).to_float(round_up=False)
-            readable_approximate_budget_needed = approximate_budget_needed.to_float(
-                round_up=False
+        except InsufficientBudgetError as err:
+            msg = _format_insufficient_budget_msg(
+                err.requested_budget, err.remaining_budget, privacy_budget
             )
-            readable_approximate_budget_left = approximate_budget_left.to_float(
-                round_up=False
-            )
-
             raise RuntimeError(
-                "Cannot perform this partition without exceeding privacy budget: it"
-                f" needs approximately {readable_approximate_budget_needed:.3f}, but"
-                " the remaining budget is approximately"
-                f" {readable_approximate_budget_left:.3f} (difference:"
-                f" {approximate_diff:.3e})"
-            ) from e
+                "Cannot perform this partition without exceeding "
+                "the Session privacy budget." + msg
+            ) from err
 
         for i, source in enumerate(new_sources):
             if table_has_ids:
                 create_dict = CreateDictFromValue(
                     input_domain=transformation_domain,
                     input_metric=element_metric,
                     key=NamedTable(source),
@@ -1673,35 +1761,28 @@
                     " fix it!"
                 )
             return get_adjusted_budget(
                 privacy_budget,
                 PureDPBudget(remaining_budget_value.to_float(round_up=False)),
             )
         elif isinstance(privacy_budget, ApproxDPBudget):
-            # TODO #2476: Reverse this when we support consuming delta
             if privacy_budget.is_infinite:
                 return ApproxDPBudget(float("inf"), 0)
             else:
-                warn(
-                    "The use of ApproxDP is not yet fully supported. your budget"
-                    " request will be processed as PureDP using the epsilon"
-                    " provided.",
-                    UserWarning,
-                )
                 if not is_exact_number_tuple(remaining_budget_value):
                     raise AssertionError(
                         "Remaining budget type for ApproxDP must be Tuple[ExactNumber,"
                         " ExactNumber], but instead received"
                         f" {type(remaining_budget_value)}. This is probably a bug;"
                         " please let us know about it so we can fix it!"
                     )
                 # mypy doesn't understand that we've already checked that this is a tuple
                 remaining_epsilon, remaining_delta = remaining_budget_value  # type: ignore
                 return get_adjusted_budget(
-                    ApproxDPBudget(privacy_budget.epsilon, 0),
+                    ApproxDPBudget(*privacy_budget.value),
                     ApproxDPBudget(
                         remaining_epsilon.to_float(round_up=False),
                         remaining_delta.to_float(round_up=False),
                     ),
                 )
         elif isinstance(privacy_budget, RhoZCDPBudget):
             if not isinstance(remaining_budget_value, ExactNumber):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/truncation_strategy.py` & `tmlt_analytics-0.7.2/tmlt/analytics/truncation_strategy.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/tmlt/analytics/utils.py` & `tmlt_analytics-0.7.2/tmlt/analytics/utils.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.1/setup.py` & `tmlt_analytics-0.7.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['pandas>=1.2.0,<2.0.0',
  'pyspark[sql]>=3.0.0,<=3.3.1',
  'sympy>=1.8,<1.10',
- 'tmlt.core>=0.9.0,<0.10.0',
+ 'tmlt.core>=0.10.1,<0.11.0',
  'typeguard>=2.12.1,<2.13.0',
  'typing-extensions>=3.10.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'tmlt-analytics',
-    'version': '0.7.1',
+    'version': '0.7.2',
     'description': "Tumult's differential privacy analytics API",
-    'long_description': '# Tumult Analytics\n\nTumult Analytics is a library that allows users to execute differentially private operations on\ndata without having to worry about the privacy implementation, which is handled\nautomatically by the API. It is built atop the [Tumult Core library](https://gitlab.com/tumult-labs/core).\n\n## Installation\n\nSee the [installation instructions in the documentation](https://docs.tmlt.dev/analytics/latest/installation.html#prerequisites)\nfor information about setting up prerequisites such as Spark.\n\nOnce the prerequisites are installed, you can install Tumult Analytics using [pip](https://pypi.org/project/pip).\n\n```bash\npip install tmlt.analytics\n```\n\n## Documentation\n\nThe full documentation is located at https://docs.tmlt.dev/analytics/latest/.\n\n## Support\n\nIf you have any questions/concerns, please [create an issue](https://gitlab.com/tumult-labs/analytics/-/issues) or reach out to us on [Slack](https://tmltdev.slack.com/join/shared_invite/zt-1bky0mh9v-vOB8azKAVoxmzJDUdWd5Wg#).\n\n## Contributing\n\nWe are not yet accepting external contributions, but please let us know if you are interested in contributing [via Slack](https://tmltdev.slack.com/join/shared_invite/zt-1bky0mh9v-vOB8azKAVoxmzJDUdWd5Wg#).\n\nSee [CONTRIBUTING.md](CONTRIBUTING.md) for information about installing our development dependencies and running tests.\n\n## Citing Tumult Analytics\n\nIf you use Tumult Analytics for a scientific publication, we would appreciate citations to the published software or/and its whitepaper. Both citations can be found below; for the software citation, please replace the version with the version you are using.\n\n```\n@software{tumultanalyticssoftware,\n    author = {Tumult Labs},\n    title = {Tumult {{Analytics}}},\n    month = dec,\n    year = 2022,\n    version = {latest},\n    url = {https://tmlt.dev}\n}\n```\n\n```\n@article{tumultanalyticswhitepaper,\n  title={Tumult {{Analytics}}: a robust, easy-to-use, scalable, and expressive framework for differential privacy},\n  author={Berghel, Skye and Bohannon, Philip and Desfontaines, Damien and Estes, Charles and Haney, Sam and Hartman, Luke and Hay, Michael and Machanavajjhala, Ashwin and Magerlein, Tom and Miklau, Gerome and Pai, Amritha and Sexton, William and Shrestha, Ruchit},\n  journal={arXiv preprint arXiv:2212.04133},\n  month = dec,\n  year={2022}\n}\n```\n\n## License\n\nCopyright Tumult Labs 2023\n\nThe Tumult Platform source code is licensed under the Apache License, version 2.0 (Apache-2.0).\nThe Tumult Platform documentation is licensed under\nCreative Commons Attribution-ShareAlike 4.0 International (CC-BY-SA-4.0).\n',
+    'long_description': "# Tumult Analytics\n\nTumult Analytics is a library that allows users to execute differentially private operations on\ndata without having to worry about the privacy implementation, which is handled\nautomatically by the API. It is built atop the [Tumult Core library](https://gitlab.com/tumult-labs/core).\n\n## Installation\n\nSee the [installation instructions in the documentation](https://docs.tmlt.dev/analytics/latest/installation.html#prerequisites)\nfor information about setting up prerequisites such as Spark.\n\nOnce the prerequisites are installed, you can install Tumult Analytics using [pip](https://pypi.org/project/pip).\n\n```bash\npip install tmlt.analytics\n```\n\n## Documentation\n\nThe full documentation is located at https://docs.tmlt.dev/analytics/latest/.\n\n## Support\n\nIf you have any questions/concerns, please [create an issue](https://gitlab.com/tumult-labs/analytics/-/issues) or reach out to us on [Slack](https://tmltdev.slack.com/join/shared_invite/zt-1bky0mh9v-vOB8azKAVoxmzJDUdWd5Wg#).\n\n## Contributing\n\nWe are not yet accepting external contributions, but please let us know if you are interested in contributing [via Slack](https://tmltdev.slack.com/join/shared_invite/zt-1bky0mh9v-vOB8azKAVoxmzJDUdWd5Wg#).\n\nSee [CONTRIBUTING.md](CONTRIBUTING.md) for information about installing our development dependencies and running tests.\n\n## Citing Tumult Analytics\n\nIf you use Tumult Analytics for a scientific publication, we would appreciate citations to the published software or/and its whitepaper. Both citations can be found below; for the software citation, please replace the version with the version you are using.\n\n```\n@software{tumultanalyticssoftware,\n    author = {Tumult Labs},\n    title = {Tumult {{Analytics}}},\n    month = dec,\n    year = 2022,\n    version = {latest},\n    url = {https://tmlt.dev}\n}\n```\n\n```\n@article{tumultanalyticswhitepaper,\n  title={Tumult {{Analytics}}: a robust, easy-to-use, scalable, and expressive framework for differential privacy},\n  author={Berghel, Skye and Bohannon, Philip and Desfontaines, Damien and Estes, Charles and Haney, Sam and Hartman, Luke and Hay, Michael and Machanavajjhala, Ashwin and Magerlein, Tom and Miklau, Gerome and Pai, Amritha and Sexton, William and Shrestha, Ruchit},\n  journal={arXiv preprint arXiv:2212.04133},\n  month = dec,\n  year={2022}\n}\n```\n\n## License\n\nCopyright Tumult Labs 2023\n\nTumult Analytics' source code is licensed under the Apache License, version 2.0 (Apache-2.0).\nTumult Analytics' documentation is licensed under\nCreative Commons Attribution-ShareAlike 4.0 International (CC-BY-SA-4.0).\n",
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://www.tmlt.dev/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7.1,<3.10.0',
+    'python_requires': '>=3.7.1,<3.11.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `tmlt_analytics-0.7.1/PKG-INFO` & `tmlt_analytics-0.7.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: tmlt-analytics
-Version: 0.7.1
+Version: 0.7.2
 Summary: Tumult's differential privacy analytics API
 Home-page: https://www.tmlt.dev/
 License: Apache-2.0
-Requires-Python: >=3.7.1,<3.10.0
+Requires-Python: >=3.7.1,<3.11.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: pandas (>=1.2.0,<2.0.0)
 Requires-Dist: pyspark[sql] (>=3.0.0,<=3.3.1)
 Requires-Dist: sympy (>=1.8,<1.10)
-Requires-Dist: tmlt.core (>=0.9.0,<0.10.0)
+Requires-Dist: tmlt.core (>=0.10.1,<0.11.0)
 Requires-Dist: typeguard (>=2.12.1,<2.13.0)
 Requires-Dist: typing-extensions (>=3.10.0,<4.0.0)
 Project-URL: Documentation, https://docs.tmlt.dev/analytics/latest
 Project-URL: Repository, https://gitlab.com/tumult-labs/analytics
 Description-Content-Type: text/markdown
 
 # Tumult Analytics
@@ -84,11 +85,11 @@
 }
 ```
 
 ## License
 
 Copyright Tumult Labs 2023
 
-The Tumult Platform source code is licensed under the Apache License, version 2.0 (Apache-2.0).
-The Tumult Platform documentation is licensed under
+Tumult Analytics' source code is licensed under the Apache License, version 2.0 (Apache-2.0).
+Tumult Analytics' documentation is licensed under
 Creative Commons Attribution-ShareAlike 4.0 International (CC-BY-SA-4.0).
```

