# Comparing `tmp/getdaft-0.1.5.tar.gz` & `tmp/getdaft-0.1.6.tar.gz`

## Comparing `getdaft-0.1.5.tar` & `getdaft-0.1.6.tar`

### file list

```diff
@@ -1,469 +1,489 @@
--rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 getdaft-0.1.5/Cargo.toml
--rw-r--r--   0      501       20      834 2023-06-06 06:00:19.000000 getdaft-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0      501       20      595 2023-06-06 06:00:19.000000 getdaft-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0      501       20      428 2023-06-06 06:00:19.000000 getdaft-0.1.5/.github/dependabot.yml
--rw-r--r--   0      501       20     1333 2023-06-06 06:00:19.000000 getdaft-0.1.5/.github/workflows/broken-link-checker.yml
--rw-r--r--   0      501       20     3378 2023-06-06 06:00:19.000000 getdaft-0.1.5/.github/workflows/daft-profiling.yml
--rw-r--r--   0      501       20     1627 2023-06-06 06:00:19.000000 getdaft-0.1.5/.github/workflows/notebook-checker.yml
--rw-r--r--   0      501       20     2194 2023-06-06 06:00:19.000000 getdaft-0.1.5/.github/workflows/property-based-tests.yml
--rw-r--r--   0      501       20    12886 2023-06-06 06:00:19.000000 getdaft-0.1.5/.github/workflows/python-package.yml
--rw-r--r--   0      501       20     6182 2023-06-06 06:00:19.000000 getdaft-0.1.5/.github/workflows/python-publish.yml
--rw-r--r--   0      501       20     2638 2023-06-06 06:00:19.000000 getdaft-0.1.5/.github/workflows/ray-compatibility.yml
--rw-r--r--   0      501       20      300 2023-06-06 06:00:19.000000 getdaft-0.1.5/.gitignore
--rw-r--r--   0      501       20     2126 2023-06-06 06:00:19.000000 getdaft-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0      501       20      205 2023-06-06 06:00:19.000000 getdaft-0.1.5/.readthedocs.yaml
--rw-r--r--   0      501       20     1550 2023-06-06 06:00:19.000000 getdaft-0.1.5/CONTRIBUTING.md
--rw-r--r--   0      501       20    11357 2023-06-06 06:00:19.000000 getdaft-0.1.5/LICENSE
--rw-r--r--   0      501       20     1295 2023-06-06 06:00:19.000000 getdaft-0.1.5/Makefile
--rw-r--r--   0      501       20     9185 2023-06-06 06:00:19.000000 getdaft-0.1.5/README.rst
--rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/benchmarking/__init__.py
--rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/benchmarking/tpch/__init__.py
--rw-r--r--   0      501       20     9495 2023-06-06 06:00:19.000000 getdaft-0.1.5/benchmarking/tpch/__main__.py
--rw-r--r--   0      501       20    12428 2023-06-06 06:00:19.000000 getdaft-0.1.5/benchmarking/tpch/answers.py
--rw-r--r--   0      501       20    12140 2023-06-06 06:00:19.000000 getdaft-0.1.5/benchmarking/tpch/data_generation.py
--rw-r--r--   0      501       20     4573 2023-06-06 06:00:19.000000 getdaft-0.1.5/benchmarking/tpch/pipelined_data_generation.py
--rw-r--r--   0      501       20     2654 2023-06-06 06:00:19.000000 getdaft-0.1.5/benchmarking/tpch/subprefix_s3_files.py
--rw-r--r--   0      501       20     1436 2023-06-06 06:00:19.000000 getdaft-0.1.5/ci/upload_wheels.sh
--rw-r--r--   0      501       20      440 2023-06-06 06:00:19.000000 getdaft-0.1.5/codecov.yml
--rw-r--r--   0      501       20     2092 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/__init__.py
--rw-r--r--   0      501       20     6724 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/analytics.py
--rw-r--r--   0      501       20     3935 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/api_annotations.py
--rw-r--r--   0      501       20    10591 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/arrow_utils.py
--rw-r--r--   0      501       20     5395 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/context.py
--rw-r--r--   0      501       20     3403 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/convert.py
--rw-r--r--   0      501       20      724 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/daft.pyi
--rw-r--r--   0      501       20       94 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/dataframe/__init__.py
--rw-r--r--   0      501       20    49646 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/dataframe/dataframe.py
--rw-r--r--   0      501       20      306 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/dataframe/preview.py
--rw-r--r--   0      501       20      850 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/datasources.py
--rw-r--r--   0      501       20    13221 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/datatype.py
--rw-r--r--   0      501       20       84 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/errors.py
--rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/execution/__init__.py
--rw-r--r--   0      501       20    24774 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/execution/execution_step.py
--rw-r--r--   0      501       20     4231 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/execution/logical_op_runners.py
--rw-r--r--   0      501       20    28173 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/execution/physical_plan.py
--rw-r--r--   0      501       20     6110 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/execution/physical_plan_factory.py
--rw-r--r--   0      501       20      170 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/expressions/__init__.py
--rw-r--r--   0      501       20    25203 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/expressions/expressions.py
--rw-r--r--   0      501       20      572 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/expressions/testing.py
--rw-r--r--   0      501       20    12728 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/filesystem.py
--rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/internal/__init__.py
--rw-r--r--   0      501       20      509 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/internal/gpu.py
--rw-r--r--   0      501       20     1804 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/internal/rule.py
--rw-r--r--   0      501       20     2030 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/internal/rule_runner.py
--rw-r--r--   0      501       20     3490 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/internal/treenode.py
--rw-r--r--   0      501       20      263 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/io/__init__.py
--rw-r--r--   0      501       20     1682 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/io/_csv.py
--rw-r--r--   0      501       20     1223 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/io/_json.py
--rw-r--r--   0      501       20     2032 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/io/common.py
--rw-r--r--   0      501       20     2034 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/io/file_path.py
--rw-r--r--   0      501       20     1243 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/io/parquet.py
--rw-r--r--   0      501       20      264 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/logging.py
--rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/logical/__init__.py
--rw-r--r--   0      501       20     8601 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/logical/aggregation_plan_builder.py
--rw-r--r--   0      501       20    37496 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/logical/logical_plan.py
--rw-r--r--   0      501       20     1492 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/logical/map_partition_ops.py
--rw-r--r--   0      501       20    19183 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/logical/optimizer.py
--rw-r--r--   0      501       20     3625 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/logical/schema.py
--rw-r--r--   0      501       20       99 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/pickle/__init__.py
--rw-r--r--   0      501       20    34760 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/pickle/cloudpickle.py
--rw-r--r--   0      501       20    34262 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/pickle/cloudpickle_fast.py
--rw-r--r--   0      501       20      639 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/pickle/compat.py
--rw-r--r--   0      501       20      312 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/pickle/pickle.py
--rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/py.typed
--rw-r--r--   0      501       20     2036 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/resource_request.py
--rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/runners/__init__.py
--rw-r--r--   0      501       20     5708 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/runners/partitioning.py
--rw-r--r--   0      501       20     1488 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/runners/profiler.py
--rw-r--r--   0      501       20    13059 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/runners/pyrunner.py
--rw-r--r--   0      501       20    25296 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/runners/ray_runner.py
--rw-r--r--   0      501       20      918 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/runners/runner.py
--rw-r--r--   0      501       20     4324 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/runners/runner_io.py
--rw-r--r--   0      501       20    19568 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/series.py
--rw-r--r--   0      501       20       82 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/table/__init__.py
--rw-r--r--   0      501       20    13765 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/table/table.py
--rw-r--r--   0      501       20     9457 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/table/table_io.py
--rw-r--r--   0      501       20     7263 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/udf.py
--rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/udf_library/__init__.py
--rw-r--r--   0      501       20     3486 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/udf_library/url_udfs.py
--rw-r--r--   0      501       20     2796 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/utils.py
--rw-r--r--   0      501       20      183 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/viz/__init__.py
--rw-r--r--   0      501       20     1699 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/viz/dataframe_display.py
--rw-r--r--   0      501       20     1517 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/viz/html_viz_hooks.py
--rw-r--r--   0      501       20     6592 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/viz/repr.py
--rw-r--r--   0      501       20      148 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/CONTRIBUTING.md
--rw-r--r--   0      501       20      638 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/Makefile
--rw-r--r--   0      501       20    71692 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/10-min.ipynb
--rw-r--r--   0      501       20      389 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/custom-function-signatures.css
--rw-r--r--   0      501       20      565 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/daft-favicon.png
--rw-r--r--   0      501       20     7804 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/daft-logo.png
--rw-r--r--   0      501       20    42148 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/daft_illustration.png
--rw-r--r--   0      501       20      583 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/dataframe-comp-table.csv
--rw-r--r--   0      501       20    25200 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/execution_model.png
--rw-r--r--   0      501       20     1901 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/header.css
--rw-r--r--   0      501       20    32864 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/high_level_architecture.png
--rw-r--r--   0      501       20      343 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/icon-menu-close.svg
--rw-r--r--   0      501       20      333 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/icon-menu-dots.svg
--rw-r--r--   0      501       20    18177 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/in_memory_data_representation.png
--rw-r--r--   0      501       20      786 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/mobile-menu.js
--rw-r--r--   0      501       20     9142 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/tpch-1000sf.html
--rw-r--r--   0      501       20     9647 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/tpch-100sf.html
--rw-r--r--   0      501       20     8757 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/tpch-nodes-count-daft-1000-sf.html
--rw-r--r--   0      501       20      856 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_templates/layout.html
--rw-r--r--   0      501       20     1179 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_templates/sections/header.html
--rw-r--r--   0      501       20     1129 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_templates/sections/mobile-menu.html
--rw-r--r--   0      501       20      325 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/api_docs/context.rst
--rw-r--r--   0      501       20     2564 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/api_docs/dataframe.rst
--rw-r--r--   0      501       20     1997 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/api_docs/datatype.rst
--rw-r--r--   0      501       20     3898 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/api_docs/expressions.rst
--rw-r--r--   0      501       20      784 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/api_docs/groupby.rst
--rw-r--r--   0      501       20      136 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/api_docs/index.rst
--rw-r--r--   0      501       20     1457 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/api_docs/input_output.rst
--rw-r--r--   0      501       20       88 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/api_docs/udf.rst
--rw-r--r--   0      501       20    14528 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/benchmarks/index.rst
--rw-r--r--   0      501       20     3868 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/conf.py
--rw-r--r--   0      501       20     5078 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/dataframe_comparison.rst
--rw-r--r--   0      501       20     1665 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/index.rst
--rw-r--r--   0      501       20     1089 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/install.rst
--rw-r--r--   0      501       20      743 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/learn/index.rst
--rw-r--r--   0      501       20     7586 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/learn/key_concepts.rst
--rw-r--r--   0      501       20     1783 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/learn/tutorials.rst
--rw-r--r--   0      501       20     1388 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/learn/user_guides/aggregations.rst
--rw-r--r--   0      501       20     6686 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/learn/user_guides/dataframe-operations.rst
--rw-r--r--   0      501       20     4801 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/learn/user_guides/datatypes.rst
--rw-r--r--   0      501       20     9131 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/learn/user_guides/expressions.rst
--rw-r--r--   0      501       20     7829 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/learn/user_guides/intro-dataframes.rst
--rw-r--r--   0      501       20      206 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/learn/user_guides/partitioning.rst
--rw-r--r--   0      501       20     3190 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/learn/user_guides/read-write.rst
--rw-r--r--   0      501       20     1257 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/learn/user_guides/scaling-up.rst
--rw-r--r--   0      501       20     8691 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/learn/user_guides/udf.rst
--rw-r--r--   0      501       20     1577 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/learn/user_guides.rst
--rw-r--r--   0      501       20     3575 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.0.13.rst
--rw-r--r--   0      501       20     2241 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.0.14.rst
--rw-r--r--   0      501       20     1913 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.0.16.rst
--rw-r--r--   0      501       20     1750 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.0.17.rst
--rw-r--r--   0      501       20     2100 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.0.18.rst
--rw-r--r--   0      501       20     3647 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.0.19.rst
--rw-r--r--   0      501       20     4240 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.0.20.rst
--rw-r--r--   0      501       20     4633 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.0.21.rst
--rw-r--r--   0      501       20     8016 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.0.22.rst
--rw-r--r--   0      501       20     5385 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.0.23.rst
--rw-r--r--   0      501       20    11759 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.0.24.rst
--rw-r--r--   0      501       20     4750 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.1.0.rst
--rw-r--r--   0      501       20     2411 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.1.1.rst
--rw-r--r--   0      501       20     2557 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.1.2.rst
--rw-r--r--   0      501       20      839 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.1.3.rst
--rw-r--r--   0      501       20     3065 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.1.4.rst
--rw-r--r--   0      501       20      935 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/_template.rst
--rw-r--r--   0      501       20      369 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/index.rst
--rw-r--r--   0      501       20     6574 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/technical_architecture.rst
--rw-r--r--   0      501       20     1316 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/telemetry.rst
--rw-r--r--   0      501       20     1873 2023-06-06 06:00:19.000000 getdaft-0.1.5/pyproject.toml
--rw-r--r--   0      501       20      843 2023-06-06 06:00:19.000000 getdaft-0.1.5/requirements-dev.txt
--rw-r--r--   0      501       20       98 2023-06-06 06:00:19.000000 getdaft-0.1.5/rust-toolchain.toml
--rw-r--r--   0      501       20     4732 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/from.rs
--rw-r--r--   0      501       20      734 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/iterator.rs
--rw-r--r--   0      501       20     2945 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/mod.rs
--rw-r--r--   0      501       20      257 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/abs.rs
--rw-r--r--   0      501       20      726 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/apply.rs
--rw-r--r--   0      501       20      841 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/arange.rs
--rw-r--r--   0      501       20     6964 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/arithmetic.rs
--rw-r--r--   0      501       20     3048 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/arrow2/comparison.rs
--rw-r--r--   0      501       20       34 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/arrow2/mod.rs
--rw-r--r--   0      501       20       19 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/arrow2/sort/mod.rs
--rw-r--r--   0      501       20     3482 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/arrow2/sort/primitive/common.rs
--rw-r--r--   0      501       20      723 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/arrow2/sort/primitive/indices.rs
--rw-r--r--   0      501       20       47 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/arrow2/sort/primitive/mod.rs
--rw-r--r--   0      501       20     8075 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/arrow2/sort/primitive/sort.rs
--rw-r--r--   0      501       20     3501 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/as_arrow.rs
--rw-r--r--   0      501       20    11387 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/broadcast.rs
--rw-r--r--   0      501       20    30767 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/cast.rs
--rw-r--r--   0      501       20    11017 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/compare_agg.rs
--rw-r--r--   0      501       20    47218 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/comparison.rs
--rw-r--r--   0      501       20     1634 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/concat.rs
--rw-r--r--   0      501       20     5982 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/concat_agg.rs
--rw-r--r--   0      501       20     1433 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/count.rs
--rw-r--r--   0      501       20     1550 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/date.rs
--rw-r--r--   0      501       20     3335 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/filter.rs
--rw-r--r--   0      501       20     1264 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/float.rs
--rw-r--r--   0      501       20     1936 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/full.rs
--rw-r--r--   0      501       20     4112 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/groups.rs
--rw-r--r--   0      501       20     1515 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/hash.rs
--rw-r--r--   0      501       20    12551 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/if_else.rs
--rw-r--r--   0      501       20    16433 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/image.rs
--rw-r--r--   0      501       20     1058 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/len.rs
--rw-r--r--   0      501       20     3446 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/list.rs
--rw-r--r--   0      501       20     3360 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/list_agg.rs
--rw-r--r--   0      501       20     1622 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/mean.rs
--rw-r--r--   0      501       20     2617 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/mod.rs
--rw-r--r--   0      501       20     1314 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/null.rs
--rw-r--r--   0      501       20     3819 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/pairwise.rs
--rw-r--r--   0      501       20      484 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/search_sorted.rs
--rw-r--r--   0      501       20    19387 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/sort.rs
--rw-r--r--   0      501       20     2383 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/sum.rs
--rw-r--r--   0      501       20    17241 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/take.rs
--rw-r--r--   0      501       20     5279 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/utf8.rs
--rw-r--r--   0      501       20      995 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/pseudo_arrow/compute.rs
--rw-r--r--   0      501       20    13611 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/pseudo_arrow/mod.rs
--rw-r--r--   0      501       20     2502 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/pseudo_arrow/python.rs
--rw-r--r--   0      501       20    14860 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/datatypes/dtype.rs
--rw-r--r--   0      501       20     2012 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/datatypes/field.rs
--rw-r--r--   0      501       20     4549 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/datatypes/image_mode.rs
--rw-r--r--   0      501       20     2889 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/datatypes/logical.rs
--rw-r--r--   0      501       20     9088 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/datatypes/matching.rs
--rw-r--r--   0      501       20     6836 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/datatypes/mod.rs
--rw-r--r--   0      501       20     1083 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/datatypes/time_unit.rs
--rw-r--r--   0      501       20      273 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/README.md
--rw-r--r--   0      501       20     1474 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/arithmetic.rs
--rw-r--r--   0      501       20    21828 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/expr.rs
--rw-r--r--   0      501       20     1431 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/float/is_nan.rs
--rw-r--r--   0      501       20      587 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/float/mod.rs
--rw-r--r--   0      501       20     1414 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/image/decode.rs
--rw-r--r--   0      501       20      914 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/image/mod.rs
--rw-r--r--   0      501       20     1663 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/image/resize.rs
--rw-r--r--   0      501       20     1122 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/list/explode.rs
--rw-r--r--   0      501       20      597 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/list/mod.rs
--rw-r--r--   0      501       20     1944 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/mod.rs
--rw-r--r--   0      501       20     1188 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/numeric/abs.rs
--rw-r--r--   0      501       20      580 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/numeric/mod.rs
--rw-r--r--   0      501       20      676 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/python/mod.rs
--rw-r--r--   0      501       20     2050 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/python/partial_udf.rs
--rw-r--r--   0      501       20     2779 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/python/udf.rs
--rw-r--r--   0      501       20     1320 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/temporal/day.rs
--rw-r--r--   0      501       20     1348 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/temporal/day_of_week.rs
--rw-r--r--   0      501       20     1425 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/temporal/mod.rs
--rw-r--r--   0      501       20     1330 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/temporal/month.rs
--rw-r--r--   0      501       20     1324 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/temporal/year.rs
--rw-r--r--   0      501       20     1627 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/utf8/contains.rs
--rw-r--r--   0      501       20     1627 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/utf8/endswith.rs
--rw-r--r--   0      501       20     1346 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/utf8/length.rs
--rw-r--r--   0      501       20     1524 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/utf8/mod.rs
--rw-r--r--   0      501       20     1637 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/utf8/startswith.rs
--rw-r--r--   0      501       20     4961 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/lit.rs
--rw-r--r--   0      501       20      233 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/mod.rs
--rw-r--r--   0      501       20     5298 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/optimization.rs
--rw-r--r--   0      501       20     1982 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/pyobject.rs
--rw-r--r--   0      501       20     1681 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/error.rs
--rw-r--r--   0      501       20     7867 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/ffi.rs
--rw-r--r--   0      501       20     6022 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/kernels/hashing.rs
--rw-r--r--   0      501       20       54 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/kernels/mod.rs
--rw-r--r--   0      501       20    12159 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/kernels/search_sorted.rs
--rw-r--r--   0      501       20     3917 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/kernels/utf8.rs
--rw-r--r--   0      501       20     1117 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/lib.rs
--rw-r--r--   0      501       20     6900 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/python/datatype.rs
--rw-r--r--   0      501       20      307 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/python/error.rs
--rw-r--r--   0      501       20    10801 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/python/expr.rs
--rw-r--r--   0      501       20     1644 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/python/field.rs
--rw-r--r--   0      501       20      802 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/python/mod.rs
--rw-r--r--   0      501       20     2425 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/python/schema.rs
--rw-r--r--   0      501       20     9789 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/python/series.rs
--rw-r--r--   0      501       20    10760 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/python/table.rs
--rw-r--r--   0      501       20     3016 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/schema.rs
--rw-r--r--   0      501       20    10158 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/array_impl/data_array.rs
--rw-r--r--   0      501       20     5459 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/array_impl/logical_array.rs
--rw-r--r--   0      501       20      161 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/array_impl/mod.rs
--rw-r--r--   0      501       20     2099 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/from.rs
--rw-r--r--   0      501       20     2190 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/mod.rs
--rw-r--r--   0      501       20      902 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/abs.rs
--rw-r--r--   0      501       20     5207 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/agg.rs
--rw-r--r--   0      501       20     6298 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/arithmetic.rs
--rw-r--r--   0      501       20     1925 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/broadcast.rs
--rw-r--r--   0      501       20      194 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/cast.rs
--rw-r--r--   0      501       20     2609 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/comparison.rs
--rw-r--r--   0      501       20     1558 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/concat.rs
--rw-r--r--   0      501       20     1822 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/date.rs
--rw-r--r--   0      501       20     3612 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/downcast.rs
--rw-r--r--   0      501       20      697 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/filter.rs
--rw-r--r--   0      501       20      399 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/float.rs
--rw-r--r--   0      501       20      432 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/groups.rs
--rw-r--r--   0      501       20      412 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/hash.rs
--rw-r--r--   0      501       20      314 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/if_else.rs
--rw-r--r--   0      501       20     1024 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/image.rs
--rw-r--r--   0      501       20      229 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/len.rs
--rw-r--r--   0      501       20     1925 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/list.rs
--rw-r--r--   0      501       20     2367 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/mod.rs
--rw-r--r--   0      501       20      475 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/not.rs
--rw-r--r--   0      501       20      150 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/null.rs
--rw-r--r--   0      501       20      638 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/search_sorted.rs
--rw-r--r--   0      501       20     1492 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/sort.rs
--rw-r--r--   0      501       20      557 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/take.rs
--rw-r--r--   0      501       20     1528 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/utf8.rs
--rw-r--r--   0      501       20     1351 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/series_like.rs
--rw-r--r--   0      501       20    16798 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/table/mod.rs
--rw-r--r--   0      501       20     2165 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/table/ops/agg.rs
--rw-r--r--   0      501       20     3729 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/table/ops/explode.rs
--rw-r--r--   0      501       20     4403 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/table/ops/groups.rs
--rw-r--r--   0      501       20     2886 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/table/ops/hash.rs
--rw-r--r--   0      501       20     2483 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/table/ops/joins/hash_join.rs
--rw-r--r--   0      501       20     3712 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/table/ops/joins/mod.rs
--rw-r--r--   0      501       20       99 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/table/ops/mod.rs
--rw-r--r--   0      501       20     3468 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/table/ops/partition.rs
--rw-r--r--   0      501       20     1804 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/table/ops/search_sorted.rs
--rw-r--r--   0      501       20      999 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/table/ops/sort.rs
--rw-r--r--   0      501       20     5371 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/utils/arrow.rs
--rw-r--r--   0      501       20       34 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/utils/mod.rs
--rw-r--r--   0      501       20    10065 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/utils/supertype.rs
--rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/__init__.py
--rw-r--r--   0      501       20      299 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/assets/__init__.py
--rw-r--r--   0      501       20      544 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/assets/tpch-sqlite-queries/1.sql
--rw-r--r--   0      501       20      542 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/assets/tpch-sqlite-queries/10.sql
--rw-r--r--   0      501       20      703 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/assets/tpch-sqlite-queries/2.sql
--rw-r--r--   0      501       20      444 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/assets/tpch-sqlite-queries/3.sql
--rw-r--r--   0      501       20      371 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/assets/tpch-sqlite-queries/4.sql
--rw-r--r--   0      501       20      504 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/assets/tpch-sqlite-queries/5.sql
--rw-r--r--   0      501       20      259 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/assets/tpch-sqlite-queries/6.sql
--rw-r--r--   0      501       20      834 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/assets/tpch-sqlite-queries/7.sql
--rw-r--r--   0      501       20      815 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/assets/tpch-sqlite-queries/8.sql
--rw-r--r--   0      501       20      627 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/assets/tpch-sqlite-queries/9.sql
--rw-r--r--   0      501       20       48 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/assets/tpch-sqlite-queries/README.md
--rw-r--r--   0      501       20      604 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/benchmarks/conftest.py
--rw-r--r--   0      501       20     1227 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/benchmarks/test_df_arithmetic.py
--rw-r--r--   0      501       20     2706 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/benchmarks/test_file_read.py
--rw-r--r--   0      501       20     5604 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/benchmarks/test_groups_and_aggs.py
--rw-r--r--   0      501       20     7292 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/benchmarks/test_join.py
--rw-r--r--   0      501       20     2603 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/benchmarks/test_repartition.py
--rw-r--r--   0      501       20     4005 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/benchmarks/test_sort.py
--rw-r--r--   0      501       20     2911 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/conftest.py
--rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/__init__.py
--rw-r--r--   0      501       20    13229 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/assets/311-service-requests.24.csv
--rw-r--r--   0      501       20      255 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/assets/__init__.py
--rw-r--r--   0      501       20      924 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/assets/images/0000.jpg
--rw-r--r--   0      501       20      941 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/assets/images/0007.jpg
--rw-r--r--   0      501       20     2740 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/assets/images/0018.png
--rw-r--r--   0      501       20     7462 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/assets/images/0025.tiff
--rw-r--r--   0      501       20      882 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/conftest.py
--rw-r--r--   0      501       20     9268 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/test_aggregations.py
--rw-r--r--   0      501       20     2979 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/test_computations.py
--rw-r--r--   0      501       20     1798 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/test_count_rows.py
--rw-r--r--   0      501       20     7099 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/test_dataloading.py
--rw-r--r--   0      501       20      800 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/test_distinct.py
--rw-r--r--   0      501       20     6049 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/test_filter.py
--rw-r--r--   0      501       20     2301 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/test_image.py
--rw-r--r--   0      501       20     3810 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/test_joins.py
--rw-r--r--   0      501       20     2878 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/test_literals.py
--rw-r--r--   0      501       20    10311 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/test_pandas_cookbook.py
--rw-r--r--   0      501       20     4148 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/test_sorting.py
--rw-r--r--   0      501       20     1497 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/test_write.py
--rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/__init__.py
--rw-r--r--   0      501       20      751 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/conftest.py
--rw-r--r--   0      501       20      805 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_accessors.py
--rw-r--r--   0      501       20    10308 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_aggregations.py
--rw-r--r--   0      501       20    21893 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_creation.py
--rw-r--r--   0      501       20     1824 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_distinct.py
--rw-r--r--   0      501       20     1428 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_explode.py
--rw-r--r--   0      501       20     1097 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_filter.py
--rw-r--r--   0      501       20     2435 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_getitem.py
--rw-r--r--   0      501       20     4091 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_joins.py
--rw-r--r--   0      501       20     1940 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_logical_type.py
--rw-r--r--   0      501       20      223 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_repartition.py
--rw-r--r--   0      501       20     4858 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_repr.py
--rw-r--r--   0      501       20      815 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_select.py
--rw-r--r--   0      501       20      656 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_show.py
--rw-r--r--   0      501       20     6364 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_sort.py
--rw-r--r--   0      501       20     3596 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_temporals.py
--rw-r--r--   0      501       20     2385 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_to_integrations.py
--rw-r--r--   0      501       20      850 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_with_column.py
--rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/__init__.py
--rw-r--r--   0      501       20     1417 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/test_apply.py
--rw-r--r--   0      501       20     3533 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/test_expressions.py
--rw-r--r--   0      501       20     4259 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/test_expressions_projection.py
--rw-r--r--   0      501       20     5019 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/test_udf.py
--rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/typing/__init__.py
--rw-r--r--   0      501       20     6290 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/typing/conftest.py
--rw-r--r--   0      501       20     1363 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/typing/test_aggs.py
--rw-r--r--   0      501       20     2335 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/typing/test_arithmetic.py
--rw-r--r--   0      501       20      853 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/typing/test_compare.py
--rw-r--r--   0      501       20      792 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/typing/test_dt.py
--rw-r--r--   0      501       20      531 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/typing/test_float.py
--rw-r--r--   0      501       20      684 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/typing/test_if_else.py
--rw-r--r--   0      501       20      422 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/typing/test_is_null.py
--rw-r--r--   0      501       20     1176 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/typing/test_logical.py
--rw-r--r--   0      501       20     1544 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/typing/test_str.py
--rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/integration/__init__.py
--rw-r--r--   0      501       20     4193 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/integration/test_tpch.py
--rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/optimizer/__init__.py
--rw-r--r--   0      501       20     1116 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/optimizer/conftest.py
--rw-r--r--   0      501       20     1666 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/optimizer/test_drop_projections.py
--rw-r--r--   0      501       20     1847 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/optimizer/test_drop_repartition.py
--rw-r--r--   0      501       20     2463 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/optimizer/test_fold_projections.py
--rw-r--r--   0      501       20     7624 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/optimizer/test_prune_columns.py
--rw-r--r--   0      501       20     3597 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/optimizer/test_pushdown_clauses_into_scan.py
--rw-r--r--   0      501       20     1170 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/optimizer/test_pushdown_limit.py
--rw-r--r--   0      501       20     8453 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/optimizer/test_pushdown_predicates.py
--rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/property_based_testing/__init__.py
--rw-r--r--   0      501       20     4575 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/property_based_testing/strategies.py
--rw-r--r--   0      501       20     8895 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/property_based_testing/test_sort.py
--rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/ray/__init__.py
--rw-r--r--   0      501       20     5375 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/ray/test_dask.py
--rw-r--r--   0      501       20     8461 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/ray/test_datasets.py
--rw-r--r--   0      501       20      278 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/__init__.py
--rw-r--r--   0      501       20     9299 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_arithmetic.py
--rw-r--r--   0      501       20     8932 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_cast.py
--rw-r--r--   0      501       20    17207 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_comparisons.py
--rw-r--r--   0      501       20     7188 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_concat.py
--rw-r--r--   0      501       20      864 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_embedding.py
--rw-r--r--   0      501       20     6151 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_filter.py
--rw-r--r--   0      501       20      874 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_float.py
--rw-r--r--   0      501       20     3344 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_hash.py
--rw-r--r--   0      501       20    21522 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_if_else.py
--rw-r--r--   0      501       20     8674 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_image.py
--rw-r--r--   0      501       20      889 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_numeric_ops.py
--rw-r--r--   0      501       20     3418 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_series.py
--rw-r--r--   0      501       20     9173 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_size_bytes.py
--rw-r--r--   0      501       20     2188 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_slice.py
--rw-r--r--   0      501       20     5495 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_sort.py
--rw-r--r--   0      501       20     6111 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_take.py
--rw-r--r--   0      501       20     1934 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_temporal_ops.py
--rw-r--r--   0      501       20     4413 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_utf8_ops.py
--rw-r--r--   0      501       20      694 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/__init__.py
--rw-r--r--   0      501       20     1070 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_blackbox_kernels.py
--rw-r--r--   0      501       20      426 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_broadcasts.py
--rw-r--r--   0      501       20     2123 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_concat.py
--rw-r--r--   0      501       20     4900 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_eval.py
--rw-r--r--   0      501       20     3930 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_explodes.py
--rw-r--r--   0      501       20     7413 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_filter.py
--rw-r--r--   0      501       20    23374 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_from_py.py
--rw-r--r--   0      501       20      842 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_head.py
--rw-r--r--   0      501       20    10974 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_joins.py
--rw-r--r--   0      501       20     7811 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_partitioning.py
--rw-r--r--   0      501       20      654 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_size_bytes.py
--rw-r--r--   0      501       20    10955 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_sorting.py
--rw-r--r--   0      501       20    20923 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_table_aggs.py
--rw-r--r--   0      501       20    10064 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_table_io.py
--rw-r--r--   0      501       20     5061 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_take.py
--rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/utf8/__init__.py
--rw-r--r--   0      501       20     1165 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/utf8/test_compares.py
--rw-r--r--   0      501       20      321 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/utf8/test_length.py
--rw-r--r--   0      501       20     3533 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/test_analytics.py
--rw-r--r--   0      501       20      703 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/test_datatypes.py
--rw-r--r--   0      501       20     3542 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/test_schema.py
--rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/udf_library/__init__.py
--rw-r--r--   0      501       20     3777 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/udf_library/test_url_udfs.py
--rw-r--r--   0      501       20      338 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/utils.py
--rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests_legacy/__init__.py
--rw-r--r--   0      501       20     6988 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests_legacy/test_resource_requests.py
--rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/__init__.py
--rw-r--r--   0      501       20     1633 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/patch_package_version.py
--rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/__init__.py
--rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/_vendor/__init__.py
--rw-r--r--   0      501       20     1125 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/_vendor/wheel/LICENSE.txt
--rw-r--r--   0      501       20       59 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/_vendor/wheel/__init__.py
--rw-r--r--   0      501       20     2499 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/_vendor/wheel/cli/__init__.py
--rw-r--r--   0      501       20     9514 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/_vendor/wheel/cli/convert.py
--rw-r--r--   0      501       20     3113 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/_vendor/wheel/cli/pack.py
--rw-r--r--   0      501       20      662 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/_vendor/wheel/cli/unpack.py
--rw-r--r--   0      501       20     1246 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/_vendor/wheel/pkginfo.py
--rw-r--r--   0      501       20      974 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/_vendor/wheel/util.py
--rw-r--r--   0      501       20     7125 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/_vendor/wheel/wheelfile.py
--rw-r--r--   0      501       20      878 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/fix-and-copy-wheel.py
--rw-r--r--   0      501       20     2981 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/tmpdirs.py
--rw-r--r--   0      501       20     4469 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/tools.py
--rw-r--r--   0      501       20     9484 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/wheeltools.py
--rw-r--r--   0      501       20       19 2023-06-06 06:00:19.000000 getdaft-0.1.5/tutorials/.gitignore
--rw-r--r--   0      501       20    19576 2023-06-06 06:00:19.000000 getdaft-0.1.5/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb
--rw-r--r--   0      501       20    12068 2023-06-06 06:00:19.000000 getdaft-0.1.5/tutorials/image_querying/top_n_red_color.ipynb
--rw-r--r--   0      501       20    98730 2023-06-06 06:00:19.000000 getdaft-0.1.5/tutorials/mnist.ipynb
--rw-r--r--   0      501       20    11847 2023-06-06 06:00:19.000000 getdaft-0.1.5/tutorials/text_to_image/text_to_image_generation.ipynb
--rw-r--r--   0      501       20     9134 2023-06-06 06:00:19.000000 getdaft-0.1.5/tutorials/text_to_image/using_cloud_with_ray.ipynb
--rw-r--r--   0      501       20    34807 2023-06-06 06:00:59.000000 getdaft-0.1.5/Cargo.lock
--rw-r--r--   0        0        0    10384 1970-01-01 00:00:00.000000 getdaft-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1765 1970-01-01 00:00:00.000000 getdaft-0.1.6/Cargo.toml
+-rw-r--r--   0      501       20      834 2023-06-14 22:12:42.000000 getdaft-0.1.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0      501       20      595 2023-06-14 22:12:42.000000 getdaft-0.1.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0      501       20      428 2023-06-14 22:12:42.000000 getdaft-0.1.6/.github/dependabot.yml
+-rw-r--r--   0      501       20     1063 2023-06-14 22:12:42.000000 getdaft-0.1.6/.github/release-drafter.yml
+-rw-r--r--   0      501       20     1333 2023-06-14 22:12:42.000000 getdaft-0.1.6/.github/workflows/broken-link-checker.yml
+-rw-r--r--   0      501       20     3378 2023-06-14 22:12:42.000000 getdaft-0.1.6/.github/workflows/daft-profiling.yml
+-rw-r--r--   0      501       20     1052 2023-06-14 22:12:42.000000 getdaft-0.1.6/.github/workflows/enforce-pr-labels.yml
+-rw-r--r--   0      501       20     1627 2023-06-14 22:12:42.000000 getdaft-0.1.6/.github/workflows/notebook-checker.yml
+-rw-r--r--   0      501       20     2194 2023-06-14 22:12:42.000000 getdaft-0.1.6/.github/workflows/property-based-tests.yml
+-rw-r--r--   0      501       20    12886 2023-06-14 22:12:42.000000 getdaft-0.1.6/.github/workflows/python-package.yml
+-rw-r--r--   0      501       20     6182 2023-06-14 22:12:42.000000 getdaft-0.1.6/.github/workflows/python-publish.yml
+-rw-r--r--   0      501       20     2638 2023-06-14 22:12:42.000000 getdaft-0.1.6/.github/workflows/ray-compatibility.yml
+-rw-r--r--   0      501       20     1477 2023-06-14 22:12:42.000000 getdaft-0.1.6/.github/workflows/release-drafter.yml
+-rw-r--r--   0      501       20      306 2023-06-14 22:12:42.000000 getdaft-0.1.6/.gitignore
+-rw-r--r--   0      501       20     2126 2023-06-14 22:12:42.000000 getdaft-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0      501       20      205 2023-06-14 22:12:42.000000 getdaft-0.1.6/.readthedocs.yaml
+-rw-r--r--   0      501       20     1550 2023-06-14 22:12:42.000000 getdaft-0.1.6/CONTRIBUTING.md
+-rw-r--r--   0      501       20    11357 2023-06-14 22:12:42.000000 getdaft-0.1.6/LICENSE
+-rw-r--r--   0      501       20     1295 2023-06-14 22:12:42.000000 getdaft-0.1.6/Makefile
+-rw-r--r--   0      501       20     9185 2023-06-14 22:12:42.000000 getdaft-0.1.6/README.rst
+-rw-r--r--   0      501       20        0 2023-06-14 22:12:42.000000 getdaft-0.1.6/benchmarking/__init__.py
+-rw-r--r--   0      501       20        0 2023-06-14 22:12:42.000000 getdaft-0.1.6/benchmarking/tpch/__init__.py
+-rw-r--r--   0      501       20     9495 2023-06-14 22:12:42.000000 getdaft-0.1.6/benchmarking/tpch/__main__.py
+-rw-r--r--   0      501       20    12428 2023-06-14 22:12:42.000000 getdaft-0.1.6/benchmarking/tpch/answers.py
+-rw-r--r--   0      501       20    12336 2023-06-14 22:12:42.000000 getdaft-0.1.6/benchmarking/tpch/data_generation.py
+-rw-r--r--   0      501       20     4573 2023-06-14 22:12:42.000000 getdaft-0.1.6/benchmarking/tpch/pipelined_data_generation.py
+-rw-r--r--   0      501       20     2654 2023-06-14 22:12:42.000000 getdaft-0.1.6/benchmarking/tpch/subprefix_s3_files.py
+-rw-r--r--   0      501       20     1436 2023-06-14 22:12:42.000000 getdaft-0.1.6/ci/upload_wheels.sh
+-rw-r--r--   0      501       20      440 2023-06-14 22:12:42.000000 getdaft-0.1.6/codecov.yml
+-rw-r--r--   0      501       20     2199 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/__init__.py
+-rw-r--r--   0      501       20     6724 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/analytics.py
+-rw-r--r--   0      501       20     3935 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/api_annotations.py
+-rw-r--r--   0      501       20    10591 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/arrow_utils.py
+-rw-r--r--   0      501       20     5395 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/context.py
+-rw-r--r--   0      501       20     3412 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/convert.py
+-rw-r--r--   0      501       20     1298 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/daft.pyi
+-rw-r--r--   0      501       20       94 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/dataframe/__init__.py
+-rw-r--r--   0      501       20    50737 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/dataframe/dataframe.py
+-rw-r--r--   0      501       20      306 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/dataframe/preview.py
+-rw-r--r--   0      501       20      850 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/datasources.py
+-rw-r--r--   0      501       20    17086 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/datatype.py
+-rw-r--r--   0      501       20       84 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/errors.py
+-rw-r--r--   0      501       20        0 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/execution/__init__.py
+-rw-r--r--   0      501       20    24774 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/execution/execution_step.py
+-rw-r--r--   0      501       20     4487 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/execution/logical_op_runners.py
+-rw-r--r--   0      501       20    28513 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/execution/physical_plan.py
+-rw-r--r--   0      501       20     6350 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/execution/physical_plan_factory.py
+-rw-r--r--   0      501       20      170 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/expressions/__init__.py
+-rw-r--r--   0      501       20    27772 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/expressions/expressions.py
+-rw-r--r--   0      501       20      572 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/expressions/testing.py
+-rw-r--r--   0      501       20    12728 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/filesystem.py
+-rw-r--r--   0      501       20        0 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/internal/__init__.py
+-rw-r--r--   0      501       20      509 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/internal/gpu.py
+-rw-r--r--   0      501       20     1804 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/internal/rule.py
+-rw-r--r--   0      501       20     2030 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/internal/rule_runner.py
+-rw-r--r--   0      501       20     3490 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/internal/treenode.py
+-rw-r--r--   0      501       20      263 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/io/__init__.py
+-rw-r--r--   0      501       20     2292 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/io/_csv.py
+-rw-r--r--   0      501       20     1470 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/io/_json.py
+-rw-r--r--   0      501       20     2243 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/io/common.py
+-rw-r--r--   0      501       20     2034 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/io/file_path.py
+-rw-r--r--   0      501       20     1490 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/io/parquet.py
+-rw-r--r--   0      501       20      264 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/logging.py
+-rw-r--r--   0      501       20        0 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/logical/__init__.py
+-rw-r--r--   0      501       20     8601 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/logical/aggregation_plan_builder.py
+-rw-r--r--   0      501       20    38976 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/logical/logical_plan.py
+-rw-r--r--   0      501       20     1492 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/logical/map_partition_ops.py
+-rw-r--r--   0      501       20    19757 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/logical/optimizer.py
+-rw-r--r--   0      501       20     3868 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/logical/schema.py
+-rw-r--r--   0      501       20       99 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/pickle/__init__.py
+-rw-r--r--   0      501       20    34760 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/pickle/cloudpickle.py
+-rw-r--r--   0      501       20    34262 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/pickle/cloudpickle_fast.py
+-rw-r--r--   0      501       20      639 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/pickle/compat.py
+-rw-r--r--   0      501       20      312 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/pickle/pickle.py
+-rw-r--r--   0      501       20        0 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/py.typed
+-rw-r--r--   0      501       20     2036 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/resource_request.py
+-rw-r--r--   0      501       20        0 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/runners/__init__.py
+-rw-r--r--   0      501       20     4676 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/runners/partitioning.py
+-rw-r--r--   0      501       20     1488 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/runners/profiler.py
+-rw-r--r--   0      501       20    12927 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/runners/pyrunner.py
+-rw-r--r--   0      501       20    25058 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/runners/ray_runner.py
+-rw-r--r--   0      501       20      918 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/runners/runner.py
+-rw-r--r--   0      501       20     3338 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/runners/runner_io.py
+-rw-r--r--   0      501       20    22096 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/series.py
+-rw-r--r--   0      501       20       82 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/table/__init__.py
+-rw-r--r--   0      501       20     2960 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/table/schema_inference.py
+-rw-r--r--   0      501       20    14029 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/table/table.py
+-rw-r--r--   0      501       20     9916 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/table/table_io.py
+-rw-r--r--   0      501       20     7370 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/udf.py
+-rw-r--r--   0      501       20        0 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/udf_library/__init__.py
+-rw-r--r--   0      501       20     3486 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/udf_library/url_udfs.py
+-rw-r--r--   0      501       20     2796 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/utils.py
+-rw-r--r--   0      501       20      183 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/viz/__init__.py
+-rw-r--r--   0      501       20     1929 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/viz/dataframe_display.py
+-rw-r--r--   0      501       20     1517 2023-06-14 22:12:42.000000 getdaft-0.1.6/daft/viz/html_viz_hooks.py
+-rw-r--r--   0      501       20      148 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/CONTRIBUTING.md
+-rw-r--r--   0      501       20      638 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/Makefile
+-rw-r--r--   0      501       20    73229 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/10-min.ipynb
+-rw-r--r--   0      501       20      389 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/_static/custom-function-signatures.css
+-rw-r--r--   0      501       20      565 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/_static/daft-favicon.png
+-rw-r--r--   0      501       20     7804 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/_static/daft-logo.png
+-rw-r--r--   0      501       20    42148 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/_static/daft_illustration.png
+-rw-r--r--   0      501       20      583 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/_static/dataframe-comp-table.csv
+-rw-r--r--   0      501       20    25200 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/_static/execution_model.png
+-rw-r--r--   0      501       20     1901 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/_static/header.css
+-rw-r--r--   0      501       20    32864 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/_static/high_level_architecture.png
+-rw-r--r--   0      501       20      343 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/_static/icon-menu-close.svg
+-rw-r--r--   0      501       20      333 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/_static/icon-menu-dots.svg
+-rw-r--r--   0      501       20    18177 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/_static/in_memory_data_representation.png
+-rw-r--r--   0      501       20      786 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/_static/mobile-menu.js
+-rw-r--r--   0      501       20     9142 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/_static/tpch-1000sf.html
+-rw-r--r--   0      501       20     9647 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/_static/tpch-100sf.html
+-rw-r--r--   0      501       20     8757 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/_static/tpch-nodes-count-daft-1000-sf.html
+-rw-r--r--   0      501       20      856 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/_templates/layout.html
+-rw-r--r--   0      501       20     1179 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/_templates/sections/header.html
+-rw-r--r--   0      501       20     1129 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/_templates/sections/mobile-menu.html
+-rw-r--r--   0      501       20      333 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/api_docs/context.rst
+-rw-r--r--   0      501       20     2678 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/api_docs/dataframe.rst
+-rw-r--r--   0      501       20     2293 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/api_docs/datatype.rst
+-rw-r--r--   0      501       20      139 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/api_docs/datatype_image_mode/daft.ImageMode.from_mode_string.rst
+-rw-r--r--   0      501       20      430 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/api_docs/datatype_image_mode/daft.ImageMode.rst
+-rw-r--r--   0      501       20      151 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/api_docs/datetype_image_format/daft.ImageFormat.from_format_string.rst
+-rw-r--r--   0      501       20      333 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/api_docs/datetype_image_format/daft.ImageFormat.rst
+-rw-r--r--   0      501       20     4719 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/api_docs/expressions.rst
+-rw-r--r--   0      501       20      816 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/api_docs/groupby.rst
+-rw-r--r--   0      501       20      146 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/api_docs/index.rst
+-rw-r--r--   0      501       20     1537 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/api_docs/input_output.rst
+-rw-r--r--   0      501       20      273 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/api_docs/series/daft.Series.rst
+-rw-r--r--   0      501       20      492 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/api_docs/series.rst
+-rw-r--r--   0      501       20       88 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/api_docs/udf.rst
+-rw-r--r--   0      501       20    14528 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/benchmarks/index.rst
+-rw-r--r--   0      501       20     4251 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/conf.py
+-rw-r--r--   0      501       20     5114 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/dataframe_comparison.rst
+-rw-r--r--   0      501       20     1655 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/index.rst
+-rw-r--r--   0      501       20     1356 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/install.rst
+-rw-r--r--   0      501       20      743 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/learn/index.rst
+-rw-r--r--   0      501       20     7830 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/learn/key_concepts.rst
+-rw-r--r--   0      501       20     1783 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/learn/tutorials.rst
+-rw-r--r--   0      501       20     1388 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/learn/user_guides/aggregations.rst
+-rw-r--r--   0      501       20     7009 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/learn/user_guides/dataframe-operations.rst
+-rw-r--r--   0      501       20     5166 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/learn/user_guides/datatypes.rst
+-rw-r--r--   0      501       20     9481 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/learn/user_guides/expressions.rst
+-rw-r--r--   0      501       20     8241 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/learn/user_guides/intro-dataframes.rst
+-rw-r--r--   0      501       20      206 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/learn/user_guides/partitioning.rst
+-rw-r--r--   0      501       20     3251 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/learn/user_guides/read-write.rst
+-rw-r--r--   0      501       20     1257 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/learn/user_guides/scaling-up.rst
+-rw-r--r--   0      501       20     8853 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/learn/user_guides/udf.rst
+-rw-r--r--   0      501       20     1577 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/learn/user_guides.rst
+-rw-r--r--   0      501       20     3575 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/release_notes/0.0.13.rst
+-rw-r--r--   0      501       20     2241 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/release_notes/0.0.14.rst
+-rw-r--r--   0      501       20     1913 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/release_notes/0.0.16.rst
+-rw-r--r--   0      501       20     1750 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/release_notes/0.0.17.rst
+-rw-r--r--   0      501       20     2094 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/release_notes/0.0.18.rst
+-rw-r--r--   0      501       20     3647 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/release_notes/0.0.19.rst
+-rw-r--r--   0      501       20     4240 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/release_notes/0.0.20.rst
+-rw-r--r--   0      501       20     4633 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/release_notes/0.0.21.rst
+-rw-r--r--   0      501       20     8016 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/release_notes/0.0.22.rst
+-rw-r--r--   0      501       20     5385 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/release_notes/0.0.23.rst
+-rw-r--r--   0      501       20    11759 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/release_notes/0.0.24.rst
+-rw-r--r--   0      501       20     4750 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/release_notes/0.1.0.rst
+-rw-r--r--   0      501       20     2411 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/release_notes/0.1.1.rst
+-rw-r--r--   0      501       20     2557 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/release_notes/0.1.2.rst
+-rw-r--r--   0      501       20      839 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/release_notes/0.1.3.rst
+-rw-r--r--   0      501       20     3065 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/release_notes/0.1.4.rst
+-rw-r--r--   0      501       20     1285 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/release_notes/0.1.5.rst
+-rw-r--r--   0      501       20      935 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/release_notes/_template.rst
+-rw-r--r--   0      501       20      387 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/release_notes/index.rst
+-rw-r--r--   0      501       20     6628 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/technical_architecture.rst
+-rw-r--r--   0      501       20     1316 2023-06-14 22:12:42.000000 getdaft-0.1.6/docs/source/telemetry.rst
+-rw-r--r--   0      501       20     1850 2023-06-14 22:12:42.000000 getdaft-0.1.6/pyproject.toml
+-rw-r--r--   0      501       20      868 2023-06-14 22:12:42.000000 getdaft-0.1.6/requirements-dev.txt
+-rw-r--r--   0      501       20       98 2023-06-14 22:12:42.000000 getdaft-0.1.6/rust-toolchain.toml
+-rw-r--r--   0      501       20     4732 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/from.rs
+-rw-r--r--   0      501       20      734 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/iterator.rs
+-rw-r--r--   0      501       20     2945 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/mod.rs
+-rw-r--r--   0      501       20      257 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/abs.rs
+-rw-r--r--   0      501       20      726 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/apply.rs
+-rw-r--r--   0      501       20      841 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/arange.rs
+-rw-r--r--   0      501       20     6964 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/arithmetic.rs
+-rw-r--r--   0      501       20     3048 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/arrow2/comparison.rs
+-rw-r--r--   0      501       20       34 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/arrow2/mod.rs
+-rw-r--r--   0      501       20       19 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/arrow2/sort/mod.rs
+-rw-r--r--   0      501       20     3482 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/arrow2/sort/primitive/common.rs
+-rw-r--r--   0      501       20      723 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/arrow2/sort/primitive/indices.rs
+-rw-r--r--   0      501       20       47 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/arrow2/sort/primitive/mod.rs
+-rw-r--r--   0      501       20     8075 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/arrow2/sort/primitive/sort.rs
+-rw-r--r--   0      501       20     4102 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/as_arrow.rs
+-rw-r--r--   0      501       20    11387 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/broadcast.rs
+-rw-r--r--   0      501       20    35045 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/cast.rs
+-rw-r--r--   0      501       20    11017 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/compare_agg.rs
+-rw-r--r--   0      501       20    47218 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/comparison.rs
+-rw-r--r--   0      501       20     1634 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/concat.rs
+-rw-r--r--   0      501       20     5982 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/concat_agg.rs
+-rw-r--r--   0      501       20     1433 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/count.rs
+-rw-r--r--   0      501       20     1550 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/date.rs
+-rw-r--r--   0      501       20     3556 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/filter.rs
+-rw-r--r--   0      501       20     1264 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/float.rs
+-rw-r--r--   0      501       20     1936 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/full.rs
+-rw-r--r--   0      501       20     4112 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/groups.rs
+-rw-r--r--   0      501       20     1515 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/hash.rs
+-rw-r--r--   0      501       20    12822 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/if_else.rs
+-rw-r--r--   0      501       20    18520 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/image.rs
+-rw-r--r--   0      501       20     1058 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/len.rs
+-rw-r--r--   0      501       20     6625 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/list.rs
+-rw-r--r--   0      501       20     3360 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/list_agg.rs
+-rw-r--r--   0      501       20     1622 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/mean.rs
+-rw-r--r--   0      501       20     2617 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/mod.rs
+-rw-r--r--   0      501       20     1314 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/null.rs
+-rw-r--r--   0      501       20     3819 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/pairwise.rs
+-rw-r--r--   0      501       20      484 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/search_sorted.rs
+-rw-r--r--   0      501       20    19607 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/sort.rs
+-rw-r--r--   0      501       20     2383 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/sum.rs
+-rw-r--r--   0      501       20    23415 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/take.rs
+-rw-r--r--   0      501       20     5279 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/ops/utf8.rs
+-rw-r--r--   0      501       20      995 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/pseudo_arrow/compute.rs
+-rw-r--r--   0      501       20    13611 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/pseudo_arrow/mod.rs
+-rw-r--r--   0      501       20     2502 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/array/pseudo_arrow/python.rs
+-rw-r--r--   0      501       20    14928 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/datatypes/dtype.rs
+-rw-r--r--   0      501       20     2012 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/datatypes/field.rs
+-rw-r--r--   0      501       20     3187 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/datatypes/image_format.rs
+-rw-r--r--   0      501       20     4796 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/datatypes/image_mode.rs
+-rw-r--r--   0      501       20     2959 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/datatypes/logical.rs
+-rw-r--r--   0      501       20     9145 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/datatypes/matching.rs
+-rw-r--r--   0      501       20     6889 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/datatypes/mod.rs
+-rw-r--r--   0      501       20     1083 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/datatypes/time_unit.rs
+-rw-r--r--   0      501       20      273 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/README.md
+-rw-r--r--   0      501       20     1474 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/arithmetic.rs
+-rw-r--r--   0      501       20    21828 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/expr.rs
+-rw-r--r--   0      501       20     1431 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/functions/float/is_nan.rs
+-rw-r--r--   0      501       20      587 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/functions/float/mod.rs
+-rw-r--r--   0      501       20     1414 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/functions/image/decode.rs
+-rw-r--r--   0      501       20     1661 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/functions/image/encode.rs
+-rw-r--r--   0      501       20     1283 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/functions/image/mod.rs
+-rw-r--r--   0      501       20     1663 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/functions/image/resize.rs
+-rw-r--r--   0      501       20     1122 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/functions/list/explode.rs
+-rw-r--r--   0      501       20     2305 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/functions/list/join.rs
+-rw-r--r--   0      501       20      878 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/functions/list/mod.rs
+-rw-r--r--   0      501       20     1944 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/functions/mod.rs
+-rw-r--r--   0      501       20     1188 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/functions/numeric/abs.rs
+-rw-r--r--   0      501       20      580 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/functions/numeric/mod.rs
+-rw-r--r--   0      501       20      676 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/functions/python/mod.rs
+-rw-r--r--   0      501       20     2050 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/functions/python/partial_udf.rs
+-rw-r--r--   0      501       20     2779 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/functions/python/udf.rs
+-rw-r--r--   0      501       20     1320 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/functions/temporal/day.rs
+-rw-r--r--   0      501       20     1348 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/functions/temporal/day_of_week.rs
+-rw-r--r--   0      501       20     1425 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/functions/temporal/mod.rs
+-rw-r--r--   0      501       20     1330 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/functions/temporal/month.rs
+-rw-r--r--   0      501       20     1324 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/functions/temporal/year.rs
+-rw-r--r--   0      501       20     1627 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/functions/utf8/contains.rs
+-rw-r--r--   0      501       20     1627 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/functions/utf8/endswith.rs
+-rw-r--r--   0      501       20     1346 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/functions/utf8/length.rs
+-rw-r--r--   0      501       20     1524 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/functions/utf8/mod.rs
+-rw-r--r--   0      501       20     1637 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/functions/utf8/startswith.rs
+-rw-r--r--   0      501       20     4961 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/lit.rs
+-rw-r--r--   0      501       20      233 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/mod.rs
+-rw-r--r--   0      501       20     5298 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/optimization.rs
+-rw-r--r--   0      501       20     1982 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/dsl/pyobject.rs
+-rw-r--r--   0      501       20     1681 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/error.rs
+-rw-r--r--   0      501       20     7867 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/ffi.rs
+-rw-r--r--   0      501       20     6022 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/kernels/hashing.rs
+-rw-r--r--   0      501       20       54 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/kernels/mod.rs
+-rw-r--r--   0      501       20    12159 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/kernels/search_sorted.rs
+-rw-r--r--   0      501       20     3917 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/kernels/utf8.rs
+-rw-r--r--   0      501       20     1117 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/lib.rs
+-rw-r--r--   0      501       20     8657 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/python/datatype.rs
+-rw-r--r--   0      501       20      307 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/python/error.rs
+-rw-r--r--   0      501       20    11184 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/python/expr.rs
+-rw-r--r--   0      501       20     1661 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/python/field.rs
+-rw-r--r--   0      501       20      926 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/python/mod.rs
+-rw-r--r--   0      501       20     2843 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/python/schema.rs
+-rw-r--r--   0      501       20     9947 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/python/series.rs
+-rw-r--r--   0      501       20    10995 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/python/table.rs
+-rw-r--r--   0      501       20     3660 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/schema.rs
+-rw-r--r--   0      501       20    10733 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/array_impl/data_array.rs
+-rw-r--r--   0      501       20     5637 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/array_impl/logical_array.rs
+-rw-r--r--   0      501       20      161 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/array_impl/mod.rs
+-rw-r--r--   0      501       20     2099 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/from.rs
+-rw-r--r--   0      501       20     2311 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/mod.rs
+-rw-r--r--   0      501       20      902 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/ops/abs.rs
+-rw-r--r--   0      501       20     5207 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/ops/agg.rs
+-rw-r--r--   0      501       20     6298 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/ops/arithmetic.rs
+-rw-r--r--   0      501       20     1925 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/ops/broadcast.rs
+-rw-r--r--   0      501       20      194 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/ops/cast.rs
+-rw-r--r--   0      501       20     2609 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/ops/comparison.rs
+-rw-r--r--   0      501       20     1558 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/ops/concat.rs
+-rw-r--r--   0      501       20     1822 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/ops/date.rs
+-rw-r--r--   0      501       20     3612 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/ops/downcast.rs
+-rw-r--r--   0      501       20      697 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/ops/filter.rs
+-rw-r--r--   0      501       20      399 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/ops/float.rs
+-rw-r--r--   0      501       20      432 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/ops/groups.rs
+-rw-r--r--   0      501       20      412 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/ops/hash.rs
+-rw-r--r--   0      501       20      314 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/ops/if_else.rs
+-rw-r--r--   0      501       20     1522 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/ops/image.rs
+-rw-r--r--   0      501       20      229 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/ops/len.rs
+-rw-r--r--   0      501       20     2341 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/ops/list.rs
+-rw-r--r--   0      501       20     2367 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/ops/mod.rs
+-rw-r--r--   0      501       20      475 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/ops/not.rs
+-rw-r--r--   0      501       20      150 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/ops/null.rs
+-rw-r--r--   0      501       20      638 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/ops/search_sorted.rs
+-rw-r--r--   0      501       20     1492 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/ops/sort.rs
+-rw-r--r--   0      501       20      652 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/ops/take.rs
+-rw-r--r--   0      501       20     1528 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/ops/utf8.rs
+-rw-r--r--   0      501       20     1399 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/series/series_like.rs
+-rw-r--r--   0      501       20    20263 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/table/mod.rs
+-rw-r--r--   0      501       20     2165 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/table/ops/agg.rs
+-rw-r--r--   0      501       20     3729 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/table/ops/explode.rs
+-rw-r--r--   0      501       20     4403 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/table/ops/groups.rs
+-rw-r--r--   0      501       20     2886 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/table/ops/hash.rs
+-rw-r--r--   0      501       20     2483 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/table/ops/joins/hash_join.rs
+-rw-r--r--   0      501       20     3712 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/table/ops/joins/mod.rs
+-rw-r--r--   0      501       20       99 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/table/ops/mod.rs
+-rw-r--r--   0      501       20     3468 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/table/ops/partition.rs
+-rw-r--r--   0      501       20     1804 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/table/ops/search_sorted.rs
+-rw-r--r--   0      501       20      999 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/table/ops/sort.rs
+-rw-r--r--   0      501       20     5371 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/utils/arrow.rs
+-rw-r--r--   0      501       20       34 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/utils/mod.rs
+-rw-r--r--   0      501       20    10065 2023-06-14 22:12:42.000000 getdaft-0.1.6/src/utils/supertype.rs
+-rw-r--r--   0      501       20        0 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/__init__.py
+-rw-r--r--   0      501       20      299 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/assets/__init__.py
+-rw-r--r--   0      501       20      544 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/assets/tpch-sqlite-queries/1.sql
+-rw-r--r--   0      501       20      542 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/assets/tpch-sqlite-queries/10.sql
+-rw-r--r--   0      501       20      703 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/assets/tpch-sqlite-queries/2.sql
+-rw-r--r--   0      501       20      444 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/assets/tpch-sqlite-queries/3.sql
+-rw-r--r--   0      501       20      371 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/assets/tpch-sqlite-queries/4.sql
+-rw-r--r--   0      501       20      504 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/assets/tpch-sqlite-queries/5.sql
+-rw-r--r--   0      501       20      259 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/assets/tpch-sqlite-queries/6.sql
+-rw-r--r--   0      501       20      834 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/assets/tpch-sqlite-queries/7.sql
+-rw-r--r--   0      501       20      815 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/assets/tpch-sqlite-queries/8.sql
+-rw-r--r--   0      501       20      627 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/assets/tpch-sqlite-queries/9.sql
+-rw-r--r--   0      501       20       48 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/assets/tpch-sqlite-queries/README.md
+-rw-r--r--   0      501       20      604 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/benchmarks/conftest.py
+-rw-r--r--   0      501       20     1227 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/benchmarks/test_df_arithmetic.py
+-rw-r--r--   0      501       20     2706 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/benchmarks/test_file_read.py
+-rw-r--r--   0      501       20     5604 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/benchmarks/test_groups_and_aggs.py
+-rw-r--r--   0      501       20     7292 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/benchmarks/test_join.py
+-rw-r--r--   0      501       20     2603 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/benchmarks/test_repartition.py
+-rw-r--r--   0      501       20     4005 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/benchmarks/test_sort.py
+-rw-r--r--   0      501       20     2911 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/conftest.py
+-rw-r--r--   0      501       20        0 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/cookbook/__init__.py
+-rw-r--r--   0      501       20    13229 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/cookbook/assets/311-service-requests.24.csv
+-rw-r--r--   0      501       20      255 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/cookbook/assets/__init__.py
+-rw-r--r--   0      501       20      924 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/cookbook/assets/images/0000.jpg
+-rw-r--r--   0      501       20      941 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/cookbook/assets/images/0007.jpg
+-rw-r--r--   0      501       20     2740 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/cookbook/assets/images/0018.png
+-rw-r--r--   0      501       20     7462 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/cookbook/assets/images/0025.tiff
+-rw-r--r--   0      501       20      882 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/cookbook/conftest.py
+-rw-r--r--   0      501       20     9268 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/cookbook/test_aggregations.py
+-rw-r--r--   0      501       20     2979 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/cookbook/test_computations.py
+-rw-r--r--   0      501       20     1798 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/cookbook/test_count_rows.py
+-rw-r--r--   0      501       20     7099 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/cookbook/test_dataloading.py
+-rw-r--r--   0      501       20      800 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/cookbook/test_distinct.py
+-rw-r--r--   0      501       20     6049 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/cookbook/test_filter.py
+-rw-r--r--   0      501       20     3072 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/cookbook/test_image.py
+-rw-r--r--   0      501       20     3810 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/cookbook/test_joins.py
+-rw-r--r--   0      501       20     2878 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/cookbook/test_literals.py
+-rw-r--r--   0      501       20    10311 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/cookbook/test_pandas_cookbook.py
+-rw-r--r--   0      501       20     4148 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/cookbook/test_sorting.py
+-rw-r--r--   0      501       20     1497 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/cookbook/test_write.py
+-rw-r--r--   0      501       20        0 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/dataframe/__init__.py
+-rw-r--r--   0      501       20      751 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/dataframe/conftest.py
+-rw-r--r--   0      501       20      805 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/dataframe/test_accessors.py
+-rw-r--r--   0      501       20    10308 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/dataframe/test_aggregations.py
+-rw-r--r--   0      501       20      472 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/dataframe/test_concat.py
+-rw-r--r--   0      501       20    24591 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/dataframe/test_creation.py
+-rw-r--r--   0      501       20     1824 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/dataframe/test_distinct.py
+-rw-r--r--   0      501       20     1428 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/dataframe/test_explode.py
+-rw-r--r--   0      501       20     1097 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/dataframe/test_filter.py
+-rw-r--r--   0      501       20     2435 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/dataframe/test_getitem.py
+-rw-r--r--   0      501       20     4091 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/dataframe/test_joins.py
+-rw-r--r--   0      501       20     1940 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/dataframe/test_logical_type.py
+-rw-r--r--   0      501       20      223 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/dataframe/test_repartition.py
+-rw-r--r--   0      501       20     5527 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/dataframe/test_repr.py
+-rw-r--r--   0      501       20      815 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/dataframe/test_select.py
+-rw-r--r--   0      501       20      656 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/dataframe/test_show.py
+-rw-r--r--   0      501       20     6364 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/dataframe/test_sort.py
+-rw-r--r--   0      501       20     4576 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/dataframe/test_temporals.py
+-rw-r--r--   0      501       20     2385 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/dataframe/test_to_integrations.py
+-rw-r--r--   0      501       20      850 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/dataframe/test_with_column.py
+-rw-r--r--   0      501       20        0 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/expressions/__init__.py
+-rw-r--r--   0      501       20     1417 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/expressions/test_apply.py
+-rw-r--r--   0      501       20     3533 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/expressions/test_expressions.py
+-rw-r--r--   0      501       20     4259 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/expressions/test_expressions_projection.py
+-rw-r--r--   0      501       20     5019 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/expressions/test_udf.py
+-rw-r--r--   0      501       20        0 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/expressions/typing/__init__.py
+-rw-r--r--   0      501       20     6290 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/expressions/typing/conftest.py
+-rw-r--r--   0      501       20     1363 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/expressions/typing/test_aggs.py
+-rw-r--r--   0      501       20     2335 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/expressions/typing/test_arithmetic.py
+-rw-r--r--   0      501       20      853 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/expressions/typing/test_compare.py
+-rw-r--r--   0      501       20      792 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/expressions/typing/test_dt.py
+-rw-r--r--   0      501       20      531 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/expressions/typing/test_float.py
+-rw-r--r--   0      501       20      684 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/expressions/typing/test_if_else.py
+-rw-r--r--   0      501       20      422 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/expressions/typing/test_is_null.py
+-rw-r--r--   0      501       20     1176 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/expressions/typing/test_logical.py
+-rw-r--r--   0      501       20     1544 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/expressions/typing/test_str.py
+-rw-r--r--   0      501       20        0 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/integration/__init__.py
+-rw-r--r--   0      501       20     4343 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/integration/test_tpch.py
+-rw-r--r--   0      501       20        0 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/optimizer/__init__.py
+-rw-r--r--   0      501       20     1116 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/optimizer/conftest.py
+-rw-r--r--   0      501       20     1666 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/optimizer/test_drop_projections.py
+-rw-r--r--   0      501       20     1847 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/optimizer/test_drop_repartition.py
+-rw-r--r--   0      501       20     2463 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/optimizer/test_fold_projections.py
+-rw-r--r--   0      501       20     8050 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/optimizer/test_prune_columns.py
+-rw-r--r--   0      501       20     3597 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/optimizer/test_pushdown_clauses_into_scan.py
+-rw-r--r--   0      501       20     1170 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/optimizer/test_pushdown_limit.py
+-rw-r--r--   0      501       20     8981 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/optimizer/test_pushdown_predicates.py
+-rw-r--r--   0      501       20        0 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/property_based_testing/__init__.py
+-rw-r--r--   0      501       20     4575 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/property_based_testing/strategies.py
+-rw-r--r--   0      501       20     8895 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/property_based_testing/test_sort.py
+-rw-r--r--   0      501       20        0 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/ray/__init__.py
+-rw-r--r--   0      501       20     5375 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/ray/test_dask.py
+-rw-r--r--   0      501       20     8755 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/ray/test_datasets.py
+-rw-r--r--   0      501       20      278 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/series/__init__.py
+-rw-r--r--   0      501       20     9299 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/series/test_arithmetic.py
+-rw-r--r--   0      501       20    11662 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/series/test_cast.py
+-rw-r--r--   0      501       20    17207 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/series/test_comparisons.py
+-rw-r--r--   0      501       20     7188 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/series/test_concat.py
+-rw-r--r--   0      501       20      864 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/series/test_embedding.py
+-rw-r--r--   0      501       20     6151 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/series/test_filter.py
+-rw-r--r--   0      501       20      874 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/series/test_float.py
+-rw-r--r--   0      501       20     3344 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/series/test_hash.py
+-rw-r--r--   0      501       20    21522 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/series/test_if_else.py
+-rw-r--r--   0      501       20    16414 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/series/test_image.py
+-rw-r--r--   0      501       20      889 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/series/test_numeric_ops.py
+-rw-r--r--   0      501       20     3418 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/series/test_series.py
+-rw-r--r--   0      501       20     9173 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/series/test_size_bytes.py
+-rw-r--r--   0      501       20     2188 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/series/test_slice.py
+-rw-r--r--   0      501       20     5495 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/series/test_sort.py
+-rw-r--r--   0      501       20     6111 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/series/test_take.py
+-rw-r--r--   0      501       20     1934 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/series/test_temporal_ops.py
+-rw-r--r--   0      501       20     4413 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/series/test_utf8_ops.py
+-rw-r--r--   0      501       20      694 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/table/__init__.py
+-rw-r--r--   0      501       20        0 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/table/list/__init__.py
+-rw-r--r--   0      501       20     1156 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/table/list/test_list_join.py
+-rw-r--r--   0      501       20        0 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/table/table_io/__init__.py
+-rw-r--r--   0      501       20     6289 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/table/table_io/test_csv.py
+-rw-r--r--   0      501       20     4355 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/table/table_io/test_json.py
+-rw-r--r--   0      501       20     4778 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/table/table_io/test_parquet.py
+-rw-r--r--   0      501       20     2100 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/table/table_io/test_read_time_cast.py
+-rw-r--r--   0      501       20     1070 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/table/test_blackbox_kernels.py
+-rw-r--r--   0      501       20      426 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/table/test_broadcasts.py
+-rw-r--r--   0      501       20     2123 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/table/test_concat.py
+-rw-r--r--   0      501       20     4900 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/table/test_eval.py
+-rw-r--r--   0      501       20     3930 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/table/test_explodes.py
+-rw-r--r--   0      501       20     7413 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/table/test_filter.py
+-rw-r--r--   0      501       20    23530 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/table/test_from_py.py
+-rw-r--r--   0      501       20      842 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/table/test_head.py
+-rw-r--r--   0      501       20    10974 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/table/test_joins.py
+-rw-r--r--   0      501       20     7811 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/table/test_partitioning.py
+-rw-r--r--   0      501       20      654 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/table/test_size_bytes.py
+-rw-r--r--   0      501       20    10955 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/table/test_sorting.py
+-rw-r--r--   0      501       20    20923 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/table/test_table_aggs.py
+-rw-r--r--   0      501       20     5061 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/table/test_take.py
+-rw-r--r--   0      501       20        0 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/table/utf8/__init__.py
+-rw-r--r--   0      501       20     1165 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/table/utf8/test_compares.py
+-rw-r--r--   0      501       20      321 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/table/utf8/test_length.py
+-rw-r--r--   0      501       20     3533 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/test_analytics.py
+-rw-r--r--   0      501       20      703 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/test_datatypes.py
+-rw-r--r--   0      501       20     3653 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/test_schema.py
+-rw-r--r--   0      501       20        0 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/udf_library/__init__.py
+-rw-r--r--   0      501       20     3777 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/udf_library/test_url_udfs.py
+-rw-r--r--   0      501       20      338 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests/utils.py
+-rw-r--r--   0      501       20        0 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests_legacy/__init__.py
+-rw-r--r--   0      501       20     6988 2023-06-14 22:12:42.000000 getdaft-0.1.6/tests_legacy/test_resource_requests.py
+-rw-r--r--   0      501       20        0 2023-06-14 22:12:42.000000 getdaft-0.1.6/tools/__init__.py
+-rw-r--r--   0      501       20     1633 2023-06-14 22:12:42.000000 getdaft-0.1.6/tools/patch_package_version.py
+-rw-r--r--   0      501       20        0 2023-06-14 22:12:42.000000 getdaft-0.1.6/tools/wheels/__init__.py
+-rw-r--r--   0      501       20        0 2023-06-14 22:12:42.000000 getdaft-0.1.6/tools/wheels/_vendor/__init__.py
+-rw-r--r--   0      501       20     1125 2023-06-14 22:12:42.000000 getdaft-0.1.6/tools/wheels/_vendor/wheel/LICENSE.txt
+-rw-r--r--   0      501       20       59 2023-06-14 22:12:42.000000 getdaft-0.1.6/tools/wheels/_vendor/wheel/__init__.py
+-rw-r--r--   0      501       20     2499 2023-06-14 22:12:42.000000 getdaft-0.1.6/tools/wheels/_vendor/wheel/cli/__init__.py
+-rw-r--r--   0      501       20     9514 2023-06-14 22:12:42.000000 getdaft-0.1.6/tools/wheels/_vendor/wheel/cli/convert.py
+-rw-r--r--   0      501       20     3113 2023-06-14 22:12:42.000000 getdaft-0.1.6/tools/wheels/_vendor/wheel/cli/pack.py
+-rw-r--r--   0      501       20      662 2023-06-14 22:12:42.000000 getdaft-0.1.6/tools/wheels/_vendor/wheel/cli/unpack.py
+-rw-r--r--   0      501       20     1246 2023-06-14 22:12:42.000000 getdaft-0.1.6/tools/wheels/_vendor/wheel/pkginfo.py
+-rw-r--r--   0      501       20      974 2023-06-14 22:12:42.000000 getdaft-0.1.6/tools/wheels/_vendor/wheel/util.py
+-rw-r--r--   0      501       20     7125 2023-06-14 22:12:42.000000 getdaft-0.1.6/tools/wheels/_vendor/wheel/wheelfile.py
+-rw-r--r--   0      501       20      878 2023-06-14 22:12:42.000000 getdaft-0.1.6/tools/wheels/fix-and-copy-wheel.py
+-rw-r--r--   0      501       20     2981 2023-06-14 22:12:42.000000 getdaft-0.1.6/tools/wheels/tmpdirs.py
+-rw-r--r--   0      501       20     4469 2023-06-14 22:12:42.000000 getdaft-0.1.6/tools/wheels/tools.py
+-rw-r--r--   0      501       20     9484 2023-06-14 22:12:42.000000 getdaft-0.1.6/tools/wheels/wheeltools.py
+-rw-r--r--   0      501       20       19 2023-06-14 22:12:42.000000 getdaft-0.1.6/tutorials/.gitignore
+-rw-r--r--   0      501       20    19576 2023-06-14 22:12:42.000000 getdaft-0.1.6/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb
+-rw-r--r--   0      501       20    12068 2023-06-14 22:12:42.000000 getdaft-0.1.6/tutorials/image_querying/top_n_red_color.ipynb
+-rw-r--r--   0      501       20    98730 2023-06-14 22:12:42.000000 getdaft-0.1.6/tutorials/mnist.ipynb
+-rw-r--r--   0      501       20    11847 2023-06-14 22:12:42.000000 getdaft-0.1.6/tutorials/text_to_image/text_to_image_generation.ipynb
+-rw-r--r--   0      501       20     9134 2023-06-14 22:12:42.000000 getdaft-0.1.6/tutorials/text_to_image/using_cloud_with_ray.ipynb
+-rw-r--r--   0      501       20    39602 2023-06-14 22:12:42.000000 getdaft-0.1.6/Cargo.lock
+-rw-r--r--   0        0        0    10351 1970-01-01 00:00:00.000000 getdaft-0.1.6/PKG-INFO
```

### Comparing `getdaft-0.1.5/Cargo.toml` & `getdaft-0.1.6/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 [dependencies]
+base64 = "0.21.2"
+chrono = "0.4.26"
+chrono-tz = "0.8.2"
 dyn-clone = "1.0.11"
 fnv = "1.0.7"
+html-escape = "0.2.13"
 ndarray = "0.15.6"
 num-derive = "0.3.3"
 prettytable-rs = "^0.10"
 pyo3-log = "0.8.2"
 rand = "^0.8"
 serde_json = "1.0.96"
 
@@ -18,19 +22,19 @@
 
 [net]
 git-fetch-with-cli = true
 
 [package]
 edition = "2021"
 name = "daft"
-version = "0.1.5"
+version = "0.1.6"
 
 [dependencies.arrow2]
 branch = "clark/expand-casting-support"
-features = [ "compute_take", "compute_cast", "compute_aggregate", "compute_if_then_else", "compute_sort", "compute_filter", "compute_temporal", "compute_comparison", "compute_arithmetics", "compute_concatenate", "io_ipc",]
+features = [ "chrono-tz", "compute_take", "compute_cast", "compute_aggregate", "compute_if_then_else", "compute_sort", "compute_filter", "compute_temporal", "compute_comparison", "compute_arithmetics", "compute_concatenate", "io_ipc",]
 git = "https://github.com/Eventual-Inc/arrow2"
 package = "arrow2"
 version = "0.17.1"
 
 [dependencies.bincode]
 version = "1.3.3"
 
@@ -44,15 +48,15 @@
 version = "1.9.2"
 
 [dependencies.lazy_static]
 version = "1.4.0"
 
 [dependencies.log]
 features = [ "std",]
-version = "0.4.18"
+version = "0.4.19"
 
 [dependencies.num-traits]
 version = "0.2"
 
 [dependencies.numpy]
 optional = true
 version = "0.18"
@@ -60,15 +64,15 @@
 [dependencies.pyo3]
 features = [ "extension-module", "abi3-py37",]
 optional = true
 version = "0.18.3"
 
 [dependencies.serde]
 features = [ "derive", "rc",]
-version = "1.0.163"
+version = "1.0.164"
 
 [dependencies.xxhash-rust]
 features = [ "xxh3", "const_xxh3",]
 version = "0.8.5"
 
 [profile.dev]
 overflow-checks = false
```

### Comparing `getdaft-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md` & `getdaft-0.1.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md` & `getdaft-0.1.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/.github/workflows/broken-link-checker.yml` & `getdaft-0.1.6/.github/workflows/broken-link-checker.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/.github/workflows/daft-profiling.yml` & `getdaft-0.1.6/.github/workflows/daft-profiling.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/.github/workflows/notebook-checker.yml` & `getdaft-0.1.6/.github/workflows/notebook-checker.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/.github/workflows/property-based-tests.yml` & `getdaft-0.1.6/.github/workflows/property-based-tests.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/.github/workflows/python-package.yml` & `getdaft-0.1.6/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/.github/workflows/python-publish.yml` & `getdaft-0.1.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/.github/workflows/ray-compatibility.yml` & `getdaft-0.1.6/.github/workflows/ray-compatibility.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/.pre-commit-config.yaml` & `getdaft-0.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/CONTRIBUTING.md` & `getdaft-0.1.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/LICENSE` & `getdaft-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/Makefile` & `getdaft-0.1.6/Makefile`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/README.rst` & `getdaft-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/benchmarking/tpch/__main__.py` & `getdaft-0.1.6/benchmarking/tpch/__main__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/benchmarking/tpch/answers.py` & `getdaft-0.1.6/benchmarking/tpch/answers.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/benchmarking/tpch/data_generation.py` & `getdaft-0.1.6/benchmarking/tpch/data_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,17 +310,22 @@
     for tab_name in SCHEMA.keys():
         table_parquet_path = os.path.join(PARQUET_FILE_PATH, tab_name)
         if not os.path.exists(table_parquet_path):
             logger.info(f"Generating Parquet Files for {tab_name}")
             df = daft.read_csv(
                 os.path.join(csv_files_location, f"{tab_name}.tbl*"),
                 has_headers=False,
-                column_names=SCHEMA[tab_name],
                 delimiter="|",
             ).exclude("")
+            df = df.select(
+                *[
+                    df[autogen_col_name].alias(actual_col_name)
+                    for actual_col_name, autogen_col_name in zip(SCHEMA[tab_name], df.column_names)
+                ]
+            )
             df = df.write_parquet(table_parquet_path)
             df.collect()
             assert os.path.exists(table_parquet_path), f"Parquet files not generated by Daft at {table_parquet_path}"
         else:
             logger.info(
                 f"Cached Parquet files for table {tab_name} already exists at {table_parquet_path}, skipping Parquet file generation"
             )
```

### Comparing `getdaft-0.1.5/benchmarking/tpch/pipelined_data_generation.py` & `getdaft-0.1.6/benchmarking/tpch/pipelined_data_generation.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/benchmarking/tpch/subprefix_s3_files.py` & `getdaft-0.1.6/benchmarking/tpch/subprefix_s3_files.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/ci/upload_wheels.sh` & `getdaft-0.1.6/ci/upload_wheels.sh`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/daft/__init__.py` & `getdaft-0.1.6/daft/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -72,16 +72,17 @@
     from_arrow,
     from_dask_dataframe,
     from_pandas,
     from_pydict,
     from_pylist,
     from_ray_dataset,
 )
+from daft.daft import ImageFormat
 from daft.dataframe import DataFrame
-from daft.datatype import DataType
+from daft.datatype import DataType, ImageMode, TimeUnit
 from daft.expressions import col, lit
 from daft.io import from_glob_path, read_csv, read_json, read_parquet
 from daft.series import Series
 from daft.udf import udf
 from daft.viz import register_viz_hook
 
 __all__ = [
@@ -94,12 +95,15 @@
     "from_glob_path",
     "read_csv",
     "read_json",
     "read_parquet",
     "DataFrame",
     "col",
     "DataType",
+    "ImageMode",
+    "ImageFormat",
     "lit",
     "Series",
+    "TimeUnit",
     "register_viz_hook",
     "udf",
 ]
```

### Comparing `getdaft-0.1.5/daft/analytics.py` & `getdaft-0.1.6/daft/analytics.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/daft/api_annotations.py` & `getdaft-0.1.6/daft/api_annotations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/daft/arrow_utils.py` & `getdaft-0.1.6/daft/arrow_utils.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/daft/context.py` & `getdaft-0.1.6/daft/context.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/daft/convert.py` & `getdaft-0.1.6/daft/convert.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
 
 @PublicAPI
 def from_dask_dataframe(ddf: "dask.DataFrame") -> "DataFrame":
     """Creates a Daft DataFrame from a Dask DataFrame.
 
     The provided Dask DataFrame must have been created using
-    `Dask-on-Ray <https://docs.ray.io/en/latest/data/dask-on-ray.html>`__.
+    `Dask-on-Ray <https://docs.ray.io/en/latest/ray-more-libs/dask-on-ray.html>`__.
 
     .. NOTE::
         This function can only work if Daft is running using the RayRunner
 
     Args:
         ddf: The Dask DataFrame to create a Daft DataFrame from.
     """
```

### Comparing `getdaft-0.1.5/daft/dataframe/dataframe.py` & `getdaft-0.1.6/daft/dataframe/dataframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -679,14 +679,36 @@
         right_exprs = self.__column_input_to_expression(tuple(right_on) if isinstance(right_on, list) else (right_on,))
         join_op = logical_plan.Join(
             self._plan, other._plan, left_on=left_exprs, right_on=right_exprs, how=logical_plan.JoinType.INNER
         )
         return DataFrame(join_op)
 
     @DataframePublicAPI
+    def concat(self, other: "DataFrame") -> "DataFrame":
+        """Concatenates two DataFrames together in a "vertical" concatenation. The resulting DataFrame
+        has number of rows equal to the sum of the number of rows of the input DataFrames.
+
+        .. NOTE::
+            DataFrames being concatenated **must have exactly the same schema**. You may wish to use the
+            :meth:`df.select() <daft.DataFrame.select>` and :meth:`expr.cast() <daft.Expression.cast>` methods
+            to ensure schema compatibility before concatenation.
+
+        Args:
+            other (DataFrame): other DataFrame to concatenate
+
+        Returns:
+            DataFrame: DataFrame with rows from `self` on top and rows from `other` at the bottom.
+        """
+        if self.schema() != other.schema():
+            raise ValueError(
+                f"DataFrames must have exactly the same schema for concatenation! Expected:\n{self.schema()}\n\nReceived:\n{other.schema()}"
+            )
+        return DataFrame(logical_plan.Concat(self._plan, other._plan))
+
+    @DataframePublicAPI
     def drop_nan(self, *cols: ColumnInputType):
         """drops rows that contains NaNs. If cols is None it will drop rows with any NaN value.
         If column names are supplied, it will drop only those rows that contains NaNs in one of these columns.
         Example:
             >>> df = daft.from_pydict({"a": [1.0, 2.2, 3.5, float("nan")]})
             >>> df.drop_na()  # drops rows where any column contains NaN values
             >>> df = daft.from_pydict({"a": [1.6, 2.5, 3.3, float("nan")]})
@@ -1097,15 +1119,15 @@
             Iterable[Any],
             Tuple[Any],
             None,
         ] = None,
     ) -> "dask.DataFrame":
         """Converts the current Daft DataFrame to a Dask DataFrame.
 
-        The returned Dask DataFrame will use `Dask-on-Ray <https://docs.ray.io/en/latest/data/dask-on-ray.html>`__
+        The returned Dask DataFrame will use `Dask-on-Ray <https://docs.ray.io/en/latest/ray-more-libs/dask-on-ray.html>`__
         to execute operations on a Ray cluster.
 
         .. NOTE::
             This function can only work if Daft is running using the RayRunner.
 
         Args:
             meta: An empty pandas DataFrame or Series that matches the dtypes and column
```

### Comparing `getdaft-0.1.5/daft/datasources.py` & `getdaft-0.1.6/daft/datasources.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/daft/datatype.py` & `getdaft-0.1.6/daft/datatype.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import builtins
 
 import pyarrow as pa
 
 from daft.context import get_context
-from daft.daft import ImageMode, PyDataType
+from daft.daft import ImageMode, PyDataType, PyTimeUnit
 
 _RAY_DATA_EXTENSIONS_AVAILABLE = True
 _TENSOR_EXTENSION_TYPES = []
 try:
     import ray
 except ImportError:
     _RAY_DATA_EXTENSIONS_AVAILABLE = False
@@ -28,14 +28,74 @@
             from ray.data.extensions import ArrowTensorType
 
             _TENSOR_EXTENSION_TYPES = [ArrowTensorType]
     except ImportError:
         _RAY_DATA_EXTENSIONS_AVAILABLE = False
 
 
+class TimeUnit:
+    _timeunit: PyTimeUnit
+
+    def __init__(self) -> None:
+        raise NotImplementedError("Please use TimeUnit.from_str(), .s(), .ms(), .us(), or .ns() instead.")
+
+    @staticmethod
+    def _from_pytimeunit(o3: PyTimeUnit) -> TimeUnit:
+        timeunit = TimeUnit.__new__(TimeUnit)
+        timeunit._timeunit = o3
+        return timeunit
+
+    @classmethod
+    def s(cls) -> TimeUnit:
+        """Represents seconds."""
+        return cls._from_pytimeunit(PyTimeUnit.seconds())
+
+    @classmethod
+    def ms(cls) -> TimeUnit:
+        """Represents milliseconds."""
+        return cls._from_pytimeunit(PyTimeUnit.milliseconds())
+
+    @classmethod
+    def us(cls) -> TimeUnit:
+        """Represents microseconds."""
+        return cls._from_pytimeunit(PyTimeUnit.microseconds())
+
+    @classmethod
+    def ns(cls) -> TimeUnit:
+        """Represents nanoseconds."""
+        return cls._from_pytimeunit(PyTimeUnit.nanoseconds())
+
+    @classmethod
+    def from_str(cls, unit: str) -> TimeUnit:
+        unit = unit.lower()
+        if unit == "s":
+            return cls.s()
+        elif unit == "ms":
+            return cls.ms()
+        elif unit == "us":
+            return cls.us()
+        elif unit == "ns":
+            return cls.ns()
+        else:
+            raise ValueError("Unsupported unit: {unit}")
+
+    def __str__(self) -> str:
+        # These are the strings PyArrow uses.
+        if self._timeunit == PyTimeUnit.seconds():
+            return "s"
+        elif self._timeunit == PyTimeUnit.milliseconds():
+            return "ms"
+        elif self._timeunit == PyTimeUnit.microseconds():
+            return "us"
+        elif self._timeunit == PyTimeUnit.nanoseconds():
+            return "ns"
+        else:
+            assert False
+
+
 class DataType:
     """A Daft DataType defines the type of all the values in an Expression or DataFrame column"""
 
     _dtype: PyDataType
 
     def __init__(self) -> None:
         raise NotImplementedError(
@@ -121,14 +181,19 @@
 
     @classmethod
     def date(cls) -> DataType:
         """Create a Date DataType: A date with a year, month and day"""
         return cls._from_pydatatype(PyDataType.date())
 
     @classmethod
+    def timestamp(cls, timeunit: TimeUnit, timezone: str | None = None) -> DataType:
+        """Timestamp DataType."""
+        return cls._from_pydatatype(PyDataType.timestamp(timeunit._timeunit, timezone))
+
+    @classmethod
     def list(cls, name: str, dtype: DataType) -> DataType:
         """Create a List DataType: Variable-length list, where each element in the list has type ``dtype``
 
         Args:
             dtype: DataType of each element in the list
         """
         return cls._from_pydatatype(PyDataType.list(name, dtype._dtype))
@@ -172,16 +237,40 @@
             raise ValueError("The size for a embedding must be a positive integer, but got: ", size)
         return cls._from_pydatatype(PyDataType.embedding(name, dtype._dtype, size))
 
     @classmethod
     def image(
         cls, mode: str | ImageMode | None = None, height: int | None = None, width: int | None = None
     ) -> DataType:
+        """Create an Image DataType: image arrays contain (height, width, channel) ndarrays of pixel values.
+
+        Each image in the array has an :class:`~daft.ImageMode`, which describes the pixel dtype (e.g. uint8) and
+        the number of image channels/bands and their logical interpretation (e.g. RGB).
+
+        If the height, width, and mode are the same for all images in the array, specifying them when constructing
+        this type is advised, since that will allow Daft to create a more optimized physical representation
+        of the image array.
+
+        If the height, width, or mode may vary across images in the array, leaving these fields unspecified when
+        creating this type will cause Daft to respresent this image array as a heterogeneous collection of images,
+        where each image can have a different mode, height, and width. This is much more flexible, but will result
+        in a less compact representation and may be make some operations less efficient.
+
+        Args:
+            mode: The mode of the image. By default, this is inferred from the underlying data.
+                If height and width are specified, the mode must also be specified.
+            height: The height of the image. By default, this is inferred from the underlying data.
+                Must be specified if the width is specified.
+            width: The width of the image. By default, this is inferred from the underlying data.
+                Must be specified if the width is specified.
+        """
         if isinstance(mode, str):
-            mode = ImageMode.from_mode_string(mode)
+            mode = ImageMode.from_mode_string(mode.upper())
+        if mode is not None and not isinstance(mode, ImageMode):
+            raise ValueError(f"mode must be a string or ImageMode variant, but got: {mode}")
         if height is not None and width is not None:
             if not isinstance(height, int) or height <= 0:
                 raise ValueError("Image height must be a positive integer, but got: ", height)
             if not isinstance(width, int) or width <= 0:
                 raise ValueError("Image width must be a positive integer, but got: ", width)
         elif height is not None or width is not None:
             raise ValueError(
@@ -218,14 +307,17 @@
             return cls.binary()
         elif pa.types.is_boolean(arrow_type):
             return cls.bool()
         elif pa.types.is_null(arrow_type):
             return cls.null()
         elif pa.types.is_date32(arrow_type):
             return cls.date()
+        elif pa.types.is_timestamp(arrow_type):
+            timeunit = TimeUnit.from_str(arrow_type.unit)
+            return cls.timestamp(timeunit=timeunit, timezone=arrow_type.tz)
         elif pa.types.is_list(arrow_type) or pa.types.is_large_list(arrow_type):
             assert isinstance(arrow_type, (pa.ListType, pa.LargeListType))
             field = arrow_type.value_field
             return cls.list(field.name, cls.from_arrow_type(field.type))
         elif pa.types.is_fixed_size_list(arrow_type):
             assert isinstance(arrow_type, pa.FixedSizeListType)
             field = arrow_type.value_field
```

### Comparing `getdaft-0.1.5/daft/execution/execution_step.py` & `getdaft-0.1.6/daft/execution/execution_step.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/daft/execution/logical_op_runners.py` & `getdaft-0.1.6/daft/execution/logical_op_runners.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,19 +3,16 @@
 from daft.datasources import (
     CSVSourceInfo,
     JSONSourceInfo,
     ParquetSourceInfo,
     StorageType,
 )
 from daft.logical.logical_plan import FileWrite, TabularFilesScan
-from daft.runners.partitioning import (
-    vPartitionParseCSVOptions,
-    vPartitionReadOptions,
-    vPartitionSchemaInferenceOptions,
-)
+from daft.logical.schema import Schema
+from daft.runners.partitioning import TableParseCSVOptions, TableReadOptions
 from daft.table import Table, table_io
 
 
 class LogicalPartitionOpRunner:
     # TODO(charles): move to ExecutionStep
 
     def _handle_tabular_files_scan(
@@ -31,66 +28,75 @@
 
         if index is not None:
             filepaths = [filepaths[index]]
 
         # Common options for reading vPartition
         fs = scan._fs
         schema = scan._schema
-        schema_options = vPartitionSchemaInferenceOptions(schema=schema)
-        read_options = vPartitionReadOptions(
+        read_options = TableReadOptions(
             num_rows=scan._limit_rows,
             column_names=scan._column_names,  # read only specified columns
         )
 
         if scan._source_info.scan_type() == StorageType.CSV:
             assert isinstance(scan._source_info, CSVSourceInfo)
-            return Table.concat(
+            table = Table.concat(
                 [
                     table_io.read_csv(
                         file=fp,
+                        schema=schema,
                         fs=fs,
-                        csv_options=vPartitionParseCSVOptions(
+                        csv_options=TableParseCSVOptions(
                             delimiter=scan._source_info.delimiter,
-                            has_headers=scan._source_info.has_headers,
-                            skip_rows_before_header=0,
-                            skip_rows_after_header=0,
+                            header_index=0 if scan._source_info.has_headers else None,
                         ),
-                        schema_options=schema_options,
                         read_options=read_options,
                     )
                     for fp in filepaths
                 ]
             )
         elif scan._source_info.scan_type() == StorageType.JSON:
             assert isinstance(scan._source_info, JSONSourceInfo)
-            return Table.concat(
+            table = Table.concat(
                 [
                     table_io.read_json(
                         file=fp,
+                        schema=schema,
                         fs=fs,
                         read_options=read_options,
                     )
                     for fp in filepaths
                 ]
             )
         elif scan._source_info.scan_type() == StorageType.PARQUET:
             assert isinstance(scan._source_info, ParquetSourceInfo)
-            return Table.concat(
+            table = Table.concat(
                 [
                     table_io.read_parquet(
                         file=fp,
+                        schema=schema,
                         fs=fs,
                         read_options=read_options,
                     )
                     for fp in filepaths
                 ]
             )
         else:
             raise NotImplementedError(f"PyRunner has not implemented scan: {scan._source_info.scan_type()}")
 
+        expected_schema = (
+            Schema._from_fields([schema[name] for name in read_options.column_names])
+            if read_options.column_names is not None
+            else schema
+        )
+        assert (
+            table.schema() == expected_schema
+        ), f"Expected table to have schema:\n{expected_schema}\n\nReceived instead:\n{table.schema()}"
+        return table
+
     def _handle_file_write(self, inputs: dict[int, Table], file_write: FileWrite) -> Table:
         child_id = file_write._children()[0].id()
         assert file_write._storage_type == StorageType.PARQUET or file_write._storage_type == StorageType.CSV
         if file_write._storage_type == StorageType.PARQUET:
             file_names = table_io.write_parquet(
                 inputs[child_id],
                 path=file_write._root_dir,
```

### Comparing `getdaft-0.1.5/daft/execution/physical_plan.py` & `getdaft-0.1.6/daft/execution/physical_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,23 @@
                 yield None
 
             # Otherwise, we are entirely done.
             else:
                 return
 
 
+def concat(
+    top_plan: InProgressPhysicalPlan[PartitionT], bottom_plan: InProgressPhysicalPlan[PartitionT]
+) -> InProgressPhysicalPlan[PartitionT]:
+    """Vertical concat of the partitions in `top_plan` and `bottom_plan`"""
+    # Yield steps in order from the top_plan to bottom_plan
+    yield from top_plan
+    yield from bottom_plan
+
+
 def local_limit(
     child_plan: InProgressPhysicalPlan[PartitionT],
     limit: int,
 ) -> Generator[None | PartitionTask[PartitionT] | PartitionTaskBuilder[PartitionT], int, None]:
     """Apply a limit instruction to each partition in the child_plan.
 
     limit:
```

### Comparing `getdaft-0.1.5/daft/execution/physical_plan_factory.py` & `getdaft-0.1.6/daft/execution/physical_plan_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,12 +141,18 @@
         if isinstance(node, logical_plan.Join):
             return physical_plan.join(
                 left_plan=_get_physical_plan(left_child, psets),
                 right_plan=_get_physical_plan(right_child, psets),
                 join=node,
             )
 
+        elif isinstance(node, logical_plan.Concat):
+            return physical_plan.concat(
+                top_plan=_get_physical_plan(left_child, psets),
+                bottom_plan=_get_physical_plan(right_child, psets),
+            )
+
         else:
             raise NotImplementedError(f"Unsupported plan type {node}")
 
     else:
         raise NotImplementedError(f"Unsupported plan type {node}")
```

### Comparing `getdaft-0.1.5/daft/expressions/expressions.py` & `getdaft-0.1.6/daft/expressions/expressions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from __future__ import annotations
 
 import builtins
 import sys
-from datetime import date
+from datetime import date, datetime
 from typing import Callable, Iterable, Iterator, TypeVar, overload
 
 import fsspec
+import pyarrow as pa
 
+from daft.daft import ImageFormat
 from daft.daft import PyExpr as _PyExpr
 from daft.daft import col as _col
 from daft.daft import lit as _lit
 from daft.daft import udf as _udf
-from daft.datatype import DataType
+from daft.datatype import DataType, TimeUnit
 from daft.expressions.testing import expr_structurally_equal
 from daft.logical.schema import Field, Schema
 
 if sys.version_info < (3, 8):
     from typing_extensions import Literal
 else:
     from typing import Literal
@@ -29,15 +31,24 @@
 
     Args:
         val: value of column
 
     Returns:
         Expression: Expression representing the value provided
     """
-    if isinstance(value, date):
+    if isinstance(value, datetime):
+        pa_timestamp = pa.scalar(value)
+        return lit(pa_timestamp.cast(pa.int64()).as_py()).cast(
+            DataType.timestamp(
+                TimeUnit.from_str(pa_timestamp.type.unit),
+                pa_timestamp.type.tz,
+            )
+        )
+
+    elif isinstance(value, date):
         epoch_time = value - date(1970, 1, 1)
         return lit(epoch_time.days).cast(DataType.date())
     else:
         lit_value = _lit(value)
     return Expression._from_pyexpr(lit_value)
 
 
@@ -79,14 +90,19 @@
 
     @property
     def url(self) -> ExpressionUrlNamespace:
         """Access methods that work on columns of URLs"""
         return ExpressionUrlNamespace.from_expression(self)
 
     @property
+    def list(self) -> ExpressionListNamespace:
+        """Access methods that work on columns of lists"""
+        return ExpressionListNamespace.from_expression(self)
+
+    @property
     def image(self) -> ExpressionImageNamespace:
         """Access methods that work on columns of images"""
         return ExpressionImageNamespace.from_expression(self)
 
     @staticmethod
     def _from_pyexpr(pyexpr: _PyExpr) -> Expression:
         expr = Expression.__new__(Expression)
@@ -97,15 +113,15 @@
     def _to_expression(obj: object) -> Expression:
         if isinstance(obj, Expression):
             return obj
         else:
             return lit(obj)
 
     @staticmethod
-    def udf(func: Callable, expressions: list[Expression], return_dtype: DataType) -> Expression:
+    def udf(func: Callable, expressions: builtins.list[Expression], return_dtype: DataType) -> Expression:
         return Expression._from_pyexpr(_udf(func, [e._expr for e in expressions], return_dtype._dtype))
 
     def __bool__(self) -> bool:
         raise ValueError(
             "Expressions don't have a truth value. "
             "If you used Python keywords `and` `not` `or` on an expression, use `&` `~` `|` instead."
         )
@@ -557,14 +573,28 @@
 
         Returns:
             Expression: an UInt64 expression with the length of each string
         """
         return Expression._from_pyexpr(self._expr.utf8_length())
 
 
+class ExpressionListNamespace(ExpressionNamespace):
+    def join(self, delimiter: str | Expression) -> Expression:
+        """Joins every element of a list using the specified string delimiter
+
+        Args:
+            delimiter (str | Expression): the delimiter to use to join lists with
+
+        Returns:
+            Expression: a String expression which is every element of the list joined on the delimiter
+        """
+        delimiter_expr = Expression._to_expression(delimiter)
+        return Expression._from_pyexpr(self._expr.list_join(delimiter_expr._expr))
+
+
 class ExpressionsProjection(Iterable[Expression]):
     """A collection of Expressions that can be projected onto a Table to produce another Table
 
     Invariants:
         1. All Expressions have names
         2. All Expressions have unique names
     """
@@ -664,16 +694,53 @@
 
     def resolve_schema(self, schema: Schema) -> Schema:
         fields = [e._to_field(schema) for e in self]
         return Schema._from_field_name_and_types([(f.name, f.dtype) for f in fields])
 
 
 class ExpressionImageNamespace(ExpressionNamespace):
+    """Expression operations for image columns."""
+
     def decode(self) -> Expression:
+        """
+        Decodes the binary data in this column into images.
+
+        This can only be applied to binary columns that contain encoded images (e.g. PNG, JPEG, etc.)
+
+        Returns:
+            Expression: An Image expression represnting an image column.
+        """
         return Expression._from_pyexpr(self._expr.image_decode())
 
+    def encode(self, image_format: str | ImageFormat) -> Expression:
+        """
+        Encode an image column as the provided image file format, returning a binary column
+        of encoded bytes.
+
+        Args:
+            image_format: The image file format into which the images will be encoded.
+
+        Returns:
+            Expression: A Binary expression representing a binary column of encoded image bytes.
+        """
+        if isinstance(image_format, str):
+            image_format = ImageFormat.from_format_string(image_format.upper())
+        if not isinstance(image_format, ImageFormat):
+            raise ValueError(f"image_format must be a string or ImageFormat variant, but got: {image_format}")
+        return Expression._from_pyexpr(self._expr.image_encode(image_format))
+
     def resize(self, w: int, h: int) -> Expression:
+        """
+        Resize image into the provided width and height.
+
+        Args:
+            w: Desired width of the resized image.
+            h: Desired height of the resized image.
+
+        Returns:
+            Expression: An Image expression representing an image column of the resized images.
+        """
         if not isinstance(w, int):
             raise TypeError(f"expected int for w but got {type(w)}")
         if not isinstance(h, int):
             raise TypeError(f"expected int for h but got {type(h)}")
         return Expression._from_pyexpr(self._expr.image_resize(w, h))
```

### Comparing `getdaft-0.1.5/daft/expressions/testing.py` & `getdaft-0.1.6/daft/expressions/testing.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/daft/filesystem.py` & `getdaft-0.1.6/daft/filesystem.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/daft/internal/rule.py` & `getdaft-0.1.6/daft/internal/rule.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/daft/internal/rule_runner.py` & `getdaft-0.1.6/daft/internal/rule_runner.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/daft/internal/treenode.py` & `getdaft-0.1.6/daft/internal/treenode.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/daft/io/_csv.py` & `getdaft-0.1.6/daft/io/_csv.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # isort: dont-add-import: from __future__ import annotations
 
-from typing import List, Optional
+from typing import Dict, List, Optional
 
 import fsspec
 
 from daft.api_annotations import PublicAPI
 from daft.dataframe import DataFrame
 from daft.datasources import CSVSourceInfo
+from daft.datatype import DataType
 from daft.io.common import _get_tabular_files_scan
-from daft.runners.partitioning import vPartitionSchemaInferenceOptions
 
 
 @PublicAPI
 def read_csv(
     path: str,
+    schema_hints: Optional[Dict[str, DataType]] = None,
     fs: Optional[fsspec.AbstractFileSystem] = None,
     has_headers: bool = True,
     column_names: Optional[List[str]] = None,
     delimiter: str = ",",
 ) -> DataFrame:
     """Creates a DataFrame from CSV file(s)
 
@@ -25,26 +26,35 @@
         >>> df = daft.read_csv("/path/to/file.csv")
         >>> df = daft.read_csv("/path/to/directory")
         >>> df = daft.read_csv("/path/to/files-*.csv")
         >>> df = daft.read_csv("s3://path/to/files-*.csv")
 
     Args:
         path (str): Path to CSV (allows for wildcards)
+        schema_hints (dict[str, DataType]): A mapping between column names and datatypes - passing this option will
+            disable all schema inference on data being read, and throw an error if data being read is incompatible.
         fs (fsspec.AbstractFileSystem): fsspec FileSystem to use for reading data.
             By default, Daft will automatically construct a FileSystem instance internally.
         has_headers (bool): Whether the CSV has a header or not, defaults to True
-        column_names (Optional[List[str]]): Custom column names to assign to the DataFrame, defaults to None
         delimiter (Str): Delimiter used in the CSV, defaults to ","
 
     returns:
         DataFrame: parsed DataFrame
     """
+    if column_names is not None:
+        raise NotImplementedError(
+            "The `column_names` option has been deprecated. As an alternative, you may specify `has_headers=False` which will have Daft "
+            "autogenerate your column names. Then, you can use `df.select` to alias each of the autogenerated columns: "
+            "`df.select(*[col(old).alias(new) for old, new in zip(df.column_names, MY_COL_NAMES)])`. Please submit an issue if this is a "
+            "blocker for your workflow!"
+        )
+
     plan = _get_tabular_files_scan(
         path,
+        schema_hints,
         CSVSourceInfo(
             delimiter=delimiter,
             has_headers=has_headers,
         ),
         fs,
-        vPartitionSchemaInferenceOptions(inference_column_names=column_names),
     )
     return DataFrame(plan)
```

### Comparing `getdaft-0.1.5/daft/io/common.py` & `getdaft-0.1.6/daft/io/common.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 from __future__ import annotations
 
 import fsspec
 
 from daft.context import get_context
 from daft.datasources import SourceInfo
+from daft.datatype import DataType
 from daft.logical import logical_plan
-from daft.runners.partitioning import vPartitionSchemaInferenceOptions
+from daft.logical.schema import Schema
+
+
+def _get_schema_from_hints(hints: dict[str, DataType]) -> Schema:
+    if isinstance(hints, dict):
+        return Schema._from_field_name_and_types([(fname, dtype) for fname, dtype in hints.items()])
+    else:
+        raise NotImplementedError(f"Unsupported schema hints: {type(hints)}")
 
 
 def _get_tabular_files_scan(
     path: str,
+    schema_hints: dict[str, DataType] | None,
     source_info: SourceInfo,
     fs: fsspec.AbstractFileSystem | None,
-    schema_inference_options: vPartitionSchemaInferenceOptions,
 ) -> logical_plan.TabularFilesScan:
     """Returns a TabularFilesScan LogicalPlan for a given glob filepath."""
     # Glob the path using the Runner
     runner_io = get_context().runner().runner_io()
     listing_details_partition_set = runner_io.glob_paths_details(path, source_info, fs)
 
-    # TODO: We should have a more sophisticated schema inference mechanism (sample >1 file and resolve schemas across files)
-    # Infer schema from the first filepath in the listings PartitionSet
-    data_schema = runner_io.get_schema_from_first_filepath(
-        listing_details_partition_set, source_info, fs, schema_inference_options
+    # Infer schema if no hints provided
+    inferred_or_provided_schema = (
+        _get_schema_from_hints(schema_hints)
+        if schema_hints is not None
+        else runner_io.get_schema_from_first_filepath(listing_details_partition_set, source_info, fs)
     )
 
     # Construct plan
     cache_entry = get_context().runner().put_partition_set_into_cache(listing_details_partition_set)
     filepath_plan = logical_plan.InMemoryScan(
         cache_entry=cache_entry,
         schema=runner_io.FS_LISTING_SCHEMA,
         partition_spec=logical_plan.PartitionSpec(
             logical_plan.PartitionScheme.UNKNOWN, listing_details_partition_set.num_partitions()
         ),
     )
     return logical_plan.TabularFilesScan(
-        schema=data_schema,
+        schema=inferred_or_provided_schema,
         predicate=None,
         columns=None,
         source_info=source_info,
         fs=fs,
         filepaths_child=filepath_plan,
         filepaths_column_name=runner_io.FS_LISTING_PATH_COLUMN_NAME,
         # WARNING: This is currently hardcoded to be the same number of partitions as rows!! This is because we emit
```

### Comparing `getdaft-0.1.5/daft/io/file_path.py` & `getdaft-0.1.6/daft/io/file_path.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/daft/io/parquet.py` & `getdaft-0.1.6/daft/io/parquet.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 # isort: dont-add-import: from __future__ import annotations
 
-from typing import Optional
+from typing import Dict, Optional
 
 import fsspec
 
 from daft.api_annotations import PublicAPI
 from daft.dataframe import DataFrame
 from daft.datasources import ParquetSourceInfo
+from daft.datatype import DataType
 from daft.io.common import _get_tabular_files_scan
-from daft.runners.partitioning import vPartitionSchemaInferenceOptions
 
 
 @PublicAPI
-def read_parquet(path: str, fs: Optional[fsspec.AbstractFileSystem] = None) -> DataFrame:
+def read_parquet(
+    path: str,
+    schema_hints: Optional[Dict[str, DataType]] = None,
+    fs: Optional[fsspec.AbstractFileSystem] = None,
+) -> DataFrame:
     """Creates a DataFrame from Parquet file(s)
 
     Example:
         >>> df = daft.read_parquet("/path/to/file.parquet")
         >>> df = daft.read_parquet("/path/to/directory")
         >>> df = daft.read_parquet("/path/to/files-*.parquet")
         >>> df = daft.read_parquet("s3://path/to/files-*.parquet")
 
     Args:
         path (str): Path to Parquet file (allows for wildcards)
+        schema_hints (dict[str, DataType]): A mapping between column names and datatypes - passing this option will
+            disable all schema inference on data being read, and throw an error if data being read is incompatible.
         fs (fsspec.AbstractFileSystem): fsspec FileSystem to use for reading data.
             By default, Daft will automatically construct a FileSystem instance internally.
 
     returns:
         DataFrame: parsed DataFrame
     """
     plan = _get_tabular_files_scan(
         path,
+        schema_hints,
         ParquetSourceInfo(),
         fs,
-        vPartitionSchemaInferenceOptions(),
     )
     return DataFrame(plan)
```

### Comparing `getdaft-0.1.5/daft/logical/aggregation_plan_builder.py` & `getdaft-0.1.6/daft/logical/aggregation_plan_builder.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/daft/logical/logical_plan.py` & `getdaft-0.1.6/daft/logical/logical_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1025,7 +1025,49 @@
         return Join(
             left=self._children()[0].rebuild(),
             right=self._children()[1].rebuild(),
             left_on=self._left_on,
             right_on=self._right_on,
             how=self._how,
         )
+
+
+class Concat(BinaryNode):
+    def __init__(self, top: LogicalPlan, bottom: LogicalPlan):
+        assert top.schema() == bottom.schema()
+        self._top = top
+        self._bottom = bottom
+
+        new_partition_spec = PartitionSpec(
+            PartitionScheme.UNKNOWN,
+            num_partitions=(top.partition_spec().num_partitions + bottom.partition_spec().num_partitions),
+            by=None,
+        )
+
+        super().__init__(top.schema(), partition_spec=new_partition_spec, op_level=OpLevel.GLOBAL)
+        self._register_child(self._top)
+        self._register_child(self._bottom)
+
+    def __repr__(self) -> str:
+        return self._repr_helper(num_partitions=self.num_partitions())
+
+    def copy_with_new_children(self, new_children: list[LogicalPlan]) -> LogicalPlan:
+        assert len(new_children) == 2
+        return Concat(new_children[0], new_children[1])
+
+    def required_columns(self) -> list[set[str]]:
+        return [set(), set()]
+
+    def input_mapping(self) -> list[dict[str, str]]:
+        return [
+            {name: name for name in self._top.schema().column_names()},
+            {name: name for name in self._bottom.schema().column_names()},
+        ]
+
+    def _local_eq(self, other: Any) -> bool:
+        return isinstance(other, Concat) and self.schema() == other.schema()
+
+    def rebuild(self) -> LogicalPlan:
+        return Concat(
+            top=self._children()[0].rebuild(),
+            bottom=self._children()[1].rebuild(),
+        )
```

### Comparing `getdaft-0.1.5/daft/logical/map_partition_ops.py` & `getdaft-0.1.6/daft/logical/map_partition_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/daft/logical/optimizer.py` & `getdaft-0.1.6/daft/logical/optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from loguru import logger
 
 from daft import resource_request
 from daft.expressions import ExpressionsProjection, col
 from daft.internal.rule import Rule
 from daft.logical.logical_plan import (
     Coalesce,
+    Concat,
     Filter,
     GlobalLimit,
     Join,
     LocalAggregate,
     LocalLimit,
     LogicalPlan,
     PartitionScheme,
@@ -29,14 +30,15 @@
         super().__init__()
         self._combine_filters_rule = CombineFilters()
         self.register_fn(Filter, Filter, self._combine_filters_rule._combine_filters)
         self.register_fn(Filter, Projection, self._filter_through_projection)
         for op in self._supported_unary_nodes:
             self.register_fn(Filter, op, self._filter_through_unary_node)
         self.register_fn(Filter, Join, self._filter_through_join)
+        self.register_fn(Filter, Concat, self._filter_through_concat)
 
     def _filter_through_projection(self, parent: Filter, child: Projection) -> LogicalPlan | None:
         """Pushes Filter through Projections, only if filter does not rely on any projected columns
 
         Filter-Projection-* -> Projection-Filter-*
         """
         filter_predicate = parent._predicate
@@ -73,14 +75,27 @@
         Filter-Unary-* -> Unary-Filter-*
         """
         assert type(child) in self._supported_unary_nodes
         grandchild = child._children()[0]
         logger.debug(f"Pushing Filter {parent} through {child}")
         return child.copy_with_new_children([Filter(grandchild, parent._predicate)])
 
+    def _filter_through_concat(self, parent: Filter, child: Concat) -> LogicalPlan | None:
+        """Pushes a Filter through a Concat to its left/right children
+
+        Filter-Concat-Bottom-* -> Concat-Filter-Bottom-*
+        Filter-Concat-Top-* -> Concat-Filter-Top-*
+        """
+        top = child._children()[0]
+        bottom = child._children()[1]
+        return Concat(
+            top=Filter(top, parent._predicate),
+            bottom=Filter(bottom, parent._predicate),
+        )
+
     def _filter_through_join(self, parent: Filter, child: Join) -> LogicalPlan | None:
         """Pushes Filter through a Join to its left/right children
 
         Filter-Join-Left-* -> Join-Filter-Left-*
         Filter-Join-Right-* -> Join-Filter-Right-*
         """
         left = child._children()[0]
```

### Comparing `getdaft-0.1.5/daft/logical/schema.py` & `getdaft-0.1.6/daft/logical/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,20 @@
             assert isinstance(name, str), f"Expected a string name, received: {name}"
             assert isinstance(dtype, DataType), f"Expected a DataType dtype, received: {dtype}"
 
         s = Schema.__new__(Schema)
         s._schema = _PySchema.from_field_name_and_types([(name, dtype._dtype) for name, dtype in fields])
         return s
 
+    @classmethod
+    def _from_fields(self, fields: list[Field]) -> Schema:
+        s = Schema.__new__(Schema)
+        s._schema = _PySchema.from_fields([f._field for f in fields])
+        return s
+
     def __getitem__(self, key: str) -> Field:
         assert isinstance(key, str), f"Expected str for key, but received: {type(key)}"
         if key not in self._schema.names():
             raise ValueError(f"{key} was not found in Schema of fields {[f.name for f in self]}")
         pyfield = self._schema[key]
         return Field._from_pyfield(pyfield)
 
@@ -82,15 +88,18 @@
     def __eq__(self, other: object) -> bool:
         return isinstance(other, Schema) and self._schema.eq(other._schema)
 
     def to_name_set(self) -> set[str]:
         return set(self.column_names())
 
     def __repr__(self) -> str:
-        return repr([(field.name, field.dtype) for field in self])
+        return repr(self._schema)
+
+    def _repr_html_(self) -> str:
+        return self._schema._repr_html_()
 
     def union(self, other: Schema) -> Schema:
         if not isinstance(other, Schema):
             raise ValueError(f"Expected Schema, got other: {type(other)}")
 
         intersecting_names = self.to_name_set().intersection(other.to_name_set())
         if intersecting_names:
```

### Comparing `getdaft-0.1.5/daft/pickle/cloudpickle.py` & `getdaft-0.1.6/daft/pickle/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/daft/pickle/cloudpickle_fast.py` & `getdaft-0.1.6/daft/pickle/cloudpickle_fast.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/daft/pickle/compat.py` & `getdaft-0.1.6/daft/pickle/compat.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/daft/resource_request.py` & `getdaft-0.1.6/daft/resource_request.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/daft/runners/profiler.py` & `getdaft-0.1.6/daft/runners/profiler.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/daft/runners/pyrunner.py` & `getdaft-0.1.6/daft/runners/pyrunner.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 from daft.resource_request import ResourceRequest
 from daft.runners import runner_io
 from daft.runners.partitioning import (
     PartID,
     PartitionCacheEntry,
     PartitionMetadata,
     PartitionSet,
-    vPartitionSchemaInferenceOptions,
 )
 from daft.runners.profiler import profiler
 from daft.runners.runner import Runner
 from daft.table import Table
 
 
 @dataclass
@@ -119,27 +118,26 @@
         return pset
 
     def get_schema_from_first_filepath(
         self,
         listing_details_partitions: PartitionSet[Table],
         source_info: SourceInfo,
         fs: fsspec.AbstractFileSystem | None,
-        schema_inference_options: vPartitionSchemaInferenceOptions,
     ) -> Schema:
         # Naively retrieve the first filepath in the PartitionSet
         nonempty_partitions = [
             p
             for p, p_len in zip(listing_details_partitions.values(), listing_details_partitions.len_of_partitions())
             if p_len > 0
         ]
         if len(nonempty_partitions) == 0:
             raise ValueError("No files to get schema from")
         first_filepath = nonempty_partitions[0].to_pydict()[PyRunnerIO.FS_LISTING_PATH_COLUMN_NAME][0]
 
-        return runner_io.sample_schema(first_filepath, source_info, fs, schema_inference_options)
+        return runner_io.sample_schema(first_filepath, source_info, fs)
 
 
 class LocalLogicalPartitionOpRunner(LogicalPartitionOpRunner):
     ...
 
 
 class PyRunner(Runner):
```

### Comparing `getdaft-0.1.5/daft/runners/ray_runner.py` & `getdaft-0.1.6/daft/runners/ray_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 from daft.resource_request import ResourceRequest
 from daft.runners import runner_io
 from daft.runners.partitioning import (
     PartID,
     PartitionCacheEntry,
     PartitionMetadata,
     PartitionSet,
-    vPartitionSchemaInferenceOptions,
 )
 from daft.runners.profiler import profiler
 from daft.runners.pyrunner import LocalPartitionSet
 from daft.runners.runner import Runner
 from daft.table import Table
 
 if TYPE_CHECKING:
@@ -140,22 +139,21 @@
 
 @ray.remote
 def sample_schema_from_filepath_vpartition(
     p: Table,
     filepath_column: str,
     source_info: SourceInfo,
     fs: fsspec.AbstractFileSystem | None,
-    schema_inference_options: vPartitionSchemaInferenceOptions,
 ) -> Schema:
     """Ray remote function to run schema sampling on top of a Table containing filepaths"""
     assert len(p) > 0
 
     # Currently just samples the Schema from the first file
     first_filepath = p.to_pydict()[filepath_column][0]
-    return runner_io.sample_schema(first_filepath, source_info, fs, schema_inference_options)
+    return runner_io.sample_schema(first_filepath, source_info, fs)
 
 
 @dataclass
 class RayPartitionSet(PartitionSet[ray.ObjectRef]):
     _partitions: dict[PartID, ray.ObjectRef]
 
     def items(self) -> list[tuple[PartID, ray.ObjectRef]]:
@@ -239,15 +237,14 @@
         return RayPartitionSet({part_id: part for part_id, part in partition_refs})
 
     def get_schema_from_first_filepath(
         self,
         listing_details_partitions: PartitionSet[ray.ObjectRef],
         source_info: SourceInfo,
         fs: fsspec.AbstractFileSystem | None,
-        schema_inference_options: vPartitionSchemaInferenceOptions,
     ) -> Schema:
         nonempty_partitions: list[ray.ObjectRef] = [
             p
             for p, p_len in zip(listing_details_partitions.values(), listing_details_partitions.len_of_partitions())
             if p_len > 0
         ]
         if len(nonempty_partitions) == 0:
@@ -255,15 +252,14 @@
         partition: ray.ObjectRef = nonempty_partitions[0]
         return ray.get(
             sample_schema_from_filepath_vpartition.remote(
                 partition,
                 RayRunnerIO.FS_LISTING_PATH_COLUMN_NAME,
                 source_info,
                 fs,
-                schema_inference_options,
             )
         )
 
     def partition_set_from_ray_dataset(
         self,
         ds: RayDataset,
     ) -> tuple[RayPartitionSet, Schema]:
```

### Comparing `getdaft-0.1.5/daft/runners/runner.py` & `getdaft-0.1.6/daft/runners/runner.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/daft/series.py` & `getdaft-0.1.6/daft/series.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import TypeVar
 
 import pyarrow as pa
 
 from daft.arrow_utils import ensure_array, ensure_chunked_array
-from daft.daft import PySeries
+from daft.daft import ImageFormat, PySeries
 from daft.datatype import DataType
 
 _NUMPY_AVAILABLE = True
 try:
     import numpy as np
 except ImportError:
     _NUMPY_AVAILABLE = False
@@ -18,27 +18,38 @@
 try:
     import pandas as pd
 except ImportError:
     _PANDAS_AVAILABLE = False
 
 
 class Series:
+    """
+    A Daft Series is an array of data of a single type, and is usually a column in a DataFrame.
+    """
+
     _series: PySeries
 
     def __init__(self) -> None:
         raise NotImplementedError("We do not support creating a Series via __init__ ")
 
     @staticmethod
     def _from_pyseries(pyseries: PySeries) -> Series:
         s = Series.__new__(Series)
         s._series = pyseries
         return s
 
     @staticmethod
     def from_arrow(array: pa.Array | pa.ChunkedArray, name: str = "arrow_series") -> Series:
+        """
+        Construct a Series from an pyarrow array or chunked array.
+
+        Args:
+            array: The pyarrow (chunked) array whose data we wish to put in the Series.
+            name: The name associated with the Series; this is usually the column name.
+        """
         if DataType.from_arrow_type(array.type) == DataType.python():
             # If the Arrow type is not natively supported, go through the Python list path.
             return Series.from_pylist(array.to_pylist(), name=name, pyobj="force")
         elif isinstance(array, pa.Array):
             array = ensure_array(array)
             pys = PySeries.from_arrow(name, array)
             return Series._from_pyseries(pys)
@@ -54,20 +65,27 @@
             pys = PySeries.from_arrow(name, combined_array)
             return Series._from_pyseries(pys)
         else:
             raise TypeError(f"expected either PyArrow Array or Chunked Array, got {type(array)}")
 
     @staticmethod
     def from_pylist(data: list, name: str = "list_series", pyobj: str = "allow") -> Series:
-        """Make a series from the given data.
+        """Construct a Series from a Python list.
 
         The resulting type depends on the setting of pyobjects:
-            - "allow": Arrow-backed types if possible, else PyObject;
-            - "disallow": Arrow-backed types only, raising error if not convertible;
-            - "force": Store as PyObject types.
+            - ``"allow"``: Arrow-backed types if possible, else PyObject;
+            - ``"disallow"``: Arrow-backed types only, raising error if not convertible;
+            - ``"force"``: Store as PyObject types.
+
+        Args:
+            data: The Python list whose data we wish to put in the Series.
+            name: The name associated with the Series; this is usually the column name.
+            pyobj: Whether we want to ``"allow"`` coercion to Arrow types, ``"disallow"``
+                falling back to Python type representation, or ``"force"`` the data to only
+                have a Python type representation. Default is ``"allow"``.
         """
 
         if not isinstance(data, list):
             raise TypeError(f"expected a python list, got {type(data)}")
 
         if pyobj not in {"allow", "disallow", "force"}:
             raise ValueError(f"pyobj: expected either 'allow', 'disallow', or 'force', but got {pyobj})")
@@ -83,14 +101,25 @@
             if pyobj == "disallow":
                 raise
             pys = PySeries.from_pylist(name, data)
             return Series._from_pyseries(pys)
 
     @classmethod
     def from_numpy(cls, data: np.ndarray, name: str = "numpy_series") -> Series:
+        """
+        Construct a Series from a NumPy ndarray.
+
+        If the provided NumPy ndarray is 1-dimensional, Daft will attempt to store the ndarray
+        in a pyarrow Array. If the ndarray has more than 1 dimension OR storing the 1D array in Arrow failed,
+        Daft will store the ndarray data as a Python list of NumPy ndarrays.
+
+        Args:
+            data: The NumPy ndarray whose data we wish to put in the Series.
+            name: The name associated with the Series; this is usually the column name.
+        """
         if not isinstance(data, np.ndarray):
             raise TypeError(f"Expected a NumPy ndarray, got {type(data)}")
         if data.ndim <= 1:
             try:
                 arrow_array = pa.array(data)
             except pa.ArrowInvalid:
                 pass
@@ -99,14 +128,26 @@
         # TODO(Clark): Represent the tensor series with an Arrow extension type in order
         # to keep the series data contiguous.
         list_ndarray = [np.asarray(item) for item in data]
         return cls.from_pylist(list_ndarray, name=name, pyobj="force")
 
     @classmethod
     def from_pandas(cls, data: pd.Series, name: str = "pd_series") -> Series:
+        """
+        Construct a Series from a pandas Series.
+
+        This will first try to convert the series into a pyarrow array, then will fall
+        back to converting the series to a NumPy ndarray and going through that construction path,
+        and will finally fall back to converting the series to a Python list and going through that
+        path.
+
+        Args:
+            data: The pandas Series whose data we wish to put in the Daft Series.
+            name: The name associated with the Series; this is usually the column name.
+        """
         if not isinstance(data, pd.Series):
             raise TypeError(f"expected a pandas Series, got {type(data)}")
         # First, try Arrow path.
         try:
             arrow_arr = pa.Array.from_pandas(data)
         except pa.ArrowInvalid:
             pass
@@ -172,17 +213,23 @@
     def rename(self, name: str) -> Series:
         return Series._from_pyseries(self._series.rename(name))
 
     def datatype(self) -> DataType:
         return DataType._from_pydatatype(self._series.data_type())
 
     def to_arrow(self) -> pa.Array:
+        """
+        Convert this Series to an pyarrow array.
+        """
         return self._series.to_arrow()
 
     def to_pylist(self) -> list:
+        """
+        Convert this Series to a Python list.
+        """
         if self.datatype()._is_python_type():
             return self._series.to_pylist()
         else:
             return self._series.to_arrow().to_pylist()
 
     def filter(self, mask: Series) -> Series:
         if not isinstance(mask, Series):
@@ -464,14 +511,21 @@
         return Series._from_pyseries(self._series.arr_lengths())
 
 
 class SeriesImageNamespace(SeriesNamespace):
     def decode(self) -> Series:
         return Series._from_pyseries(self._series.image_decode())
 
+    def encode(self, image_format: str | ImageFormat) -> Series:
+        if isinstance(image_format, str):
+            image_format = ImageFormat.from_format_string(image_format.upper())
+        if not isinstance(image_format, ImageFormat):
+            raise ValueError(f"image_format must be a string or ImageFormat variant, but got: {image_format}")
+        return Series._from_pyseries(self._series.image_encode(image_format))
+
     def resize(self, w: int, h: int) -> Series:
         if not isinstance(w, int):
             raise TypeError(f"expected int for w but got {type(w)}")
         if not isinstance(h, int):
             raise TypeError(f"expected int for h but got {type(h)}")
 
         return Series._from_pyseries(self._series.image_resize(w, h))
```

### Comparing `getdaft-0.1.5/daft/table/table.py` & `getdaft-0.1.6/daft/table/table.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,14 +56,17 @@
 
     def __len__(self) -> int:
         return len(self._table)
 
     def __repr__(self) -> str:
         return repr(self._table)
 
+    def _repr_html_(self) -> str:
+        return self._table._repr_html_()
+
     ###
     # Creation methods
     ###
 
     @staticmethod
     def empty(schema: Schema | None = None) -> Table:
         pyt = _PyTable.empty(None) if schema is None else _PyTable.empty(schema._schema)
@@ -204,14 +207,18 @@
         else:
             return self.to_arrow().to_pandas()
 
     ###
     # Compute methods (Table -> Table)
     ###
 
+    def cast_to_schema(self, schema: Schema) -> Table:
+        """Casts a Table into the provided schema"""
+        return Table._from_pytable(self._table.cast_to_schema(schema._schema))
+
     def eval_expression_list(self, exprs: ExpressionsProjection) -> Table:
         assert all(isinstance(e, Expression) for e in exprs)
         pyexprs = [e._expr for e in exprs]
         return Table._from_pytable(self._table.eval_expression_list(pyexprs))
 
     def head(self, num: int) -> Table:
         return Table._from_pytable(self._table.head(num))
```

### Comparing `getdaft-0.1.5/daft/table/table_io.py` & `getdaft-0.1.6/daft/table/table_io.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,19 +12,16 @@
 from pyarrow import dataset as pads
 from pyarrow import json as pajson
 from pyarrow import parquet as papq
 from pyarrow.fs import FileSystem
 
 from daft.expressions import ExpressionsProjection
 from daft.filesystem import _resolve_paths_and_filesystem
-from daft.runners.partitioning import (
-    vPartitionParseCSVOptions,
-    vPartitionReadOptions,
-    vPartitionSchemaInferenceOptions,
-)
+from daft.logical.schema import Schema
+from daft.runners.partitioning import TableParseCSVOptions, TableReadOptions
 from daft.table import Table
 
 FileInput = Union[pathlib.Path, str, IO[bytes]]
 
 
 @contextlib.contextmanager
 def _open_stream(
@@ -38,73 +35,97 @@
         path = paths[0]
         with fs.open_input_stream(path) as f:
             yield f
     else:
         yield file
 
 
+def _cast_table_to_schema(table: Table, read_options: TableReadOptions, schema: Schema) -> pa.Table:
+    """Performs a cast of a Daft Table to the requested Schema/Data. This is required because:
+
+    1. Data read from the datasource may have types that do not match the inferred global schema
+    2. Data read from the datasource may have columns that are out-of-order with the inferred schema
+    3. We may need only a subset of columns, or differently-ordered columns, in `read_options`
+
+    This helper function takes care of all that, ensuring that the resulting Table has all column types matching
+    their corresponding dtype in `schema`, and column ordering/inclusion matches `read_options.column_names` (if provided).
+    """
+    pruned_schema = schema
+
+    # If reading only a subset of fields, prune the schema
+    if read_options.column_names is not None:
+        pruned_schema = Schema._from_fields([schema[name] for name in read_options.column_names])
+
+    table = table.cast_to_schema(pruned_schema)
+    return table
+
+
 def read_json(
     file: FileInput,
+    schema: Schema,
     fs: fsspec.AbstractFileSystem | None = None,
-    read_options: vPartitionReadOptions = vPartitionReadOptions(),
+    read_options: TableReadOptions = TableReadOptions(),
 ) -> Table:
     """Reads a Table from a JSON file
 
     Args:
         file (str | IO): either a file-like object or a string file path (potentially prefixed with a protocol such as "s3://")
         fs (fsspec.AbstractFileSystem): fsspec FileSystem to use for reading data.
             By default, Daft will automatically construct a FileSystem instance internally.
-        read_options (vPartitionReadOptions, optional): Options for reading the file
+        read_options (TableReadOptions, optional): Options for reading the file
 
     Returns:
         Table: Parsed Table from JSON
     """
     with _open_stream(file, fs) as f:
         table = pajson.read_json(f)
 
     if read_options.column_names is not None:
         table = table.select(read_options.column_names)
 
     # TODO(jay): Can't limit number of rows with current PyArrow filesystem so we have to shave it off after the read
     if read_options.num_rows is not None:
         table = table[: read_options.num_rows]
 
-    return Table.from_arrow(table)
+    return _cast_table_to_schema(Table.from_arrow(table), read_options=read_options, schema=schema)
 
 
 def read_parquet(
     file: FileInput,
+    schema: Schema,
     fs: fsspec.AbstractFileSystem | None = None,
-    read_options: vPartitionReadOptions = vPartitionReadOptions(),
+    read_options: TableReadOptions = TableReadOptions(),
 ) -> Table:
     """Reads a Table from a Parquet file
 
     Args:
         file (str | IO): either a file-like object or a string file path (potentially prefixed with a protocol such as "s3://")
         fs (fsspec.AbstractFileSystem): fsspec FileSystem to use for reading data.
             By default, Daft will automatically construct a FileSystem instance internally.
-        read_options (vPartitionReadOptions, optional): Options for reading the file
+        read_options (TableReadOptions, optional): Options for reading the file
 
     Returns:
         Table: Parsed Table from Parquet
     """
+    f: IO
     if not isinstance(file, (str, pathlib.Path)):
-        # BytesIO path.
-        return Table.from_arrow(papq.read_table(file, columns=read_options.column_names))
+        f = file
+    else:
+        paths, fs = _resolve_paths_and_filesystem(file, fs)
+        assert len(paths) == 1
+        path = paths[0]
+        f = fs.open_input_file(path)
 
-    paths, fs = _resolve_paths_and_filesystem(file, fs)
-    assert len(paths) == 1
-    path = paths[0]
-    f = fs.open_input_file(path)
-    pqf = papq.ParquetFile(f)
     # If no rows required, we manually construct an empty table with the right schema
     if read_options.num_rows == 0:
+        pqf = papq.ParquetFile(f)
         arrow_schema = pqf.metadata.schema.to_arrow_schema()
         table = pa.Table.from_arrays([pa.array([], type=field.type) for field in arrow_schema], schema=arrow_schema)
     elif read_options.num_rows is not None:
+        pqf = papq.ParquetFile(f)
         # Only read the required row groups.
         rows_needed = read_options.num_rows
         for i in range(pqf.metadata.num_row_groups):
             row_group_meta = pqf.metadata.row_group(i)
             rows_needed -= row_group_meta.num_rows
             if rows_needed <= 0:
                 break
@@ -114,68 +135,63 @@
             table = table.slice(length=read_options.num_rows)
     else:
         table = papq.read_table(
             f,
             columns=read_options.column_names,
         )
 
-    return Table.from_arrow(table)
+    return _cast_table_to_schema(Table.from_arrow(table), read_options=read_options, schema=schema)
 
 
 def read_csv(
     file: FileInput,
+    schema: Schema,
     fs: fsspec.AbstractFileSystem | None = None,
-    csv_options: vPartitionParseCSVOptions = vPartitionParseCSVOptions(),
-    schema_options: vPartitionSchemaInferenceOptions = vPartitionSchemaInferenceOptions(),
-    read_options: vPartitionReadOptions = vPartitionReadOptions(),
+    csv_options: TableParseCSVOptions = TableParseCSVOptions(),
+    read_options: TableReadOptions = TableReadOptions(),
 ) -> Table:
     """Reads a Table from a CSV file
 
     Args:
         file (str | IO): either a file-like object or a string file path (potentially prefixed with a protocol such as "s3://")
+        schema (Schema): Daft schema to read the CSV file into
         fs (fsspec.AbstractFileSystem): fsspec FileSystem to use for reading data.
             By default, Daft will automatically construct a FileSystem instance internally.
-        csv_options (vPartitionParseCSVOptions, optional): CSV-specific configs to apply when reading the file
-        schema_options (vPartitionSchemaInferenceOptions, optional): configs to apply when inferring schema from the file
-        read_options (vPartitionReadOptions, optional): Options for reading the file
+        csv_options (TableParseCSVOptions, optional): CSV-specific configs to apply when reading the file
+        read_options (TableReadOptions, optional): Options for reading the file
 
     Returns:
         Table: Parsed Table from CSV
     """
-    # Use provided CSV column names, or None if nothing provided
-    full_column_names = schema_options.full_schema_column_names()
-
-    # Have PyArrow generate the column names if the CSV has no header and no column names were provided
-    pyarrow_autogenerate_column_names = (not csv_options.has_headers) and (full_column_names is None)
-
-    # Have Pyarrow skip the header row if column names were provided, and a header exists in the CSV
-    skip_header_row = full_column_names is not None and csv_options.has_headers
-    pyarrow_skip_rows_after_names = (1 if skip_header_row else 0) + csv_options.skip_rows_after_header
 
     with _open_stream(file, fs) as f:
         table = pacsv.read_csv(
             f,
             parse_options=pacsv.ParseOptions(
                 delimiter=csv_options.delimiter,
             ),
-            # skip_rows applied, header row is read if column_names is not None, skip_rows_after_names is applied
             read_options=pacsv.ReadOptions(
-                autogenerate_column_names=pyarrow_autogenerate_column_names,
-                column_names=full_column_names,
-                skip_rows_after_names=pyarrow_skip_rows_after_names,
-                skip_rows=csv_options.skip_rows_before_header,
+                # If no header, we use the schema's column names. Otherwise we use the headers in the CSV file.
+                column_names=schema.column_names()
+                if csv_options.header_index is None
+                else None,
+            ),
+            convert_options=pacsv.ConvertOptions(
+                # Column pruning
+                include_columns=read_options.column_names,
+                # If any columns are missing, parse as null array
+                include_missing_columns=True,
             ),
-            convert_options=pacsv.ConvertOptions(include_columns=read_options.column_names),
         )
 
     # TODO(jay): Can't limit number of rows with current PyArrow filesystem so we have to shave it off after the read
     if read_options.num_rows is not None:
         table = table[: read_options.num_rows]
 
-    return Table.from_arrow(table)
+    return _cast_table_to_schema(Table.from_arrow(table), read_options=read_options, schema=schema)
 
 
 def write_csv(
     table: Table,
     path: str | pathlib.Path,
     compression: str | None = None,
     partition_cols: ExpressionsProjection | None = None,
```

### Comparing `getdaft-0.1.5/daft/udf.py` & `getdaft-0.1.6/daft/udf.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,14 @@
         assert len(evaluated_expressions) == len(
             expressions
         ), "Computed series must map 1:1 to the expressions that were evaluated"
         function_parameter_name_to_index = {name: i for i, name in enumerate(expressions)}
 
         args = []
         for name in arg_keys:
-
             # special-case to skip `self` since that would be a redundant argument in a method call to a class-UDF
             if name == "self":
                 continue
 
             assert name in pyvalues or name in function_parameter_name_to_index
             if name in pyvalues:
                 args.append(pyvalues[name])
@@ -147,18 +146,19 @@
         your computation can be expressed using Daft expressions, you should do so instead of writing a UDF. If your UDF expresses a
         common use-case that isn't already covered by Daft, you should file a ticket or contribute this functionality back to Daft
         as a kernel!
 
     In the example below, we create a UDF that:
 
     1. Receives data under the argument name ``x``
-    2. Converts the ``x`` Daft Series into a Python list using ``x.to_pylist()``
+    2. Converts the ``x`` Daft Series into a Python list using :meth:`x.to_pylist() <daft.Series.to_pylist>`
     3. Adds a Python constant value ``c`` to every element in ``x``
     4. Returns a new list of Python values which will be coerced to the specified return type: ``return_dtype=DataType.int64()``.
-    5. We can call our UDF on a dataframe using any of the dataframe projection operations (``with_column``, ``select`` etc)
+    5. We can call our UDF on a dataframe using any of the dataframe projection operations (:meth:`df.with_column() <daft.DataFrame.with_column>`,
+       :meth:`df.select() <daft.DataFrame.select>`, etc.)
 
     Example:
         >>> @udf(return_dtype=DataType.int64())
         >>> def add_constant(x: Series, c=10):
         >>>     return [v + c for v in x.to_pylist()]
         >>>
         >>> df = df.with_column("new_x", add_constant(df["x"], c=20))
```

### Comparing `getdaft-0.1.5/daft/udf_library/url_udfs.py` & `getdaft-0.1.6/daft/udf_library/url_udfs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/daft/utils.py` & `getdaft-0.1.6/daft/utils.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/daft/viz/dataframe_display.py` & `getdaft-0.1.6/daft/viz/dataframe_display.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 
 from daft.dataframe.preview import DataFramePreview
 from daft.logical.schema import Schema
-from daft.viz.repr import vpartition_repr, vpartition_repr_html
 
 HAS_PILLOW = False
 try:
     pass
 
     HAS_PILLOW = True
 except ImportError:
@@ -18,39 +17,48 @@
 
 
 @dataclass(frozen=True)
 class DataFrameDisplay:
 
     preview: DataFramePreview
     schema: Schema
+    # These formatting options are deprecated for now and not guaranteed to be supported.
     column_char_width: int = 20
     max_col_rows: int = 3
     num_rows: int = 10
 
     def _get_user_message(self) -> str:
         if self.preview.preview_partition is None:
             return "(No data to display: Dataframe not materialized)"
         if self.preview.dataframe_num_rows == 0:
             return "(No data to display: Materialized dataframe has no rows)"
         if self.preview.dataframe_num_rows is None:
             return f"(Showing first {min(self.num_rows, len(self.preview.preview_partition))} rows)"
         return f"(Showing first {min(self.num_rows, len(self.preview.preview_partition))} of {self.preview.dataframe_num_rows} rows)"
 
     def _repr_html_(self) -> str:
-        return vpartition_repr_html(
-            self.preview.preview_partition,
-            self.schema,
-            self.num_rows,
-            self._get_user_message(),
-            max_col_width=self.column_char_width,
-            max_lines=self.max_col_rows,
-        )
+        if len(self.schema) == 0:
+            return "<small>(No data to display: Dataframe has no columns)</small>"
+
+        res = "<div>\n"
+
+        if self.preview.preview_partition is not None:
+            res += self.preview.preview_partition._repr_html_()
+        else:
+            res += self.schema._repr_html_()
+
+        res += f"\n<small>{self._get_user_message()}</small>\n</div>"
+
+        return res
 
     def __repr__(self) -> str:
-        return vpartition_repr(
-            self.preview.preview_partition,
-            self.schema,
-            self.num_rows,
-            self._get_user_message(),
-            max_col_width=self.column_char_width,
-            max_lines=self.max_col_rows,
-        )
+        if len(self.schema) == 0:
+            return "(No data to display: Dataframe has no columns)"
+
+        if self.preview.preview_partition is not None:
+            res = repr(self.preview.preview_partition)
+        else:
+            res = repr(self.schema)
+
+        res += f"\n{self._get_user_message()}"
+
+        return res
```

### Comparing `getdaft-0.1.5/daft/viz/html_viz_hooks.py` & `getdaft-0.1.6/daft/viz/html_viz_hooks.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/Makefile` & `getdaft-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/10-min.ipynb` & `getdaft-0.1.6/docs/source/10-min.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9846538064799784%*

 * *Differences: {"'cells'": "{2: {'attachments': OrderedDict()}, 6: {'source': {insert: [(2, '1. CSV files: "*

 * *            '{func}`daft.read_csv("s3://bucket/*.csv") <daft.read_csv>`\\n\'), (3, \'2. Parquet '*

 * *            'files: {func}`daft.read_parquet("/path/*.parquet") <daft.read_parquet>`\\n\'), (4, '*

 * *            '\'3. JSON line-delimited files: {func}`daft.read_json("/path/*.parquet") '*

 * *            "<daft.read_json>`\\n'), (5, '4. Files on disk: "*

 * *            '{func}`daft.from_glob_path("/path/*.jpeg") <daft.from_glob_ […]*

```diff
@@ -18,14 +18,15 @@
                 "\u2728\u2728\u2728 **Run this notebook on Google Colab** \u2728\u2728\u2728\n",
                 "\n",
                 "You can [run this notebook yourself with Google Colab](https://colab.research.google.com/github/Eventual-Inc/Daft/blob/main/docs/source/10-min.ipynb)!\n",
                 "```"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# 10 minutes Quickstart\n",
                 "\n",
                 "This is a short introduction to all the main functionality in Daft, geared towards new users.\n",
                 "\n",
@@ -88,23 +89,24 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "You can also load DataFrames from other sources, such as:\n",
                 "\n",
-                "1. CSV files: `daft.read_csv(\"s3://bucket/*.csv\")`\n",
-                "2. Parquet files: `daft.read_parquet(\"/path/*.parquet\")`\n",
-                "3. JSON line-delimited files: `daft.read_json(\"/path/*.parquet\")`\n",
-                "4. Files on disk: `daft.from_glob_path(\"/path/*.jpeg\")`\n",
+                "1. CSV files: {func}`daft.read_csv(\"s3://bucket/*.csv\") <daft.read_csv>`\n",
+                "2. Parquet files: {func}`daft.read_parquet(\"/path/*.parquet\") <daft.read_parquet>`\n",
+                "3. JSON line-delimited files: {func}`daft.read_json(\"/path/*.parquet\") <daft.read_json>`\n",
+                "4. Files on disk: {func}`daft.from_glob_path(\"/path/*.jpeg\") <daft.from_glob_path>`\n",
                 "\n",
                 "Daft automatically supports local paths as well as paths to object storage such as AWS S3."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Inspect your dataframe by printing the `df` variable"
             ]
         },
         {
@@ -141,22 +143,23 @@
                 }
             ],
             "source": [
                 "df"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Executing your DataFrame and Displaying Data\n",
                 "\n",
                 "Notice that instead of the contents of the dataframe, the message `(no data to display: Dataframe not materialized)` is displayed when we printed our dataframe in the previous section.\n",
                 "\n",
-                "This is because Daft is **lazy** and only executes computations when explicitly told to do so. When you call methods on DataFrames such as `.select`, `.where` and `.read_csv`, Daft actually only enqueues these operations in a *Logical Plan*. You can examine this logical plan using `DataFrame.explain()`:"
+                "This is because Daft is **lazy** and only executes computations when explicitly told to do so. When you call methods on DataFrames such as {meth}`df.select() <daft.DataFrame.select>`, {meth}`df.where() <daft.DataFrame.where>` and {func}`daft.read_csv`, Daft actually only enqueues these operations in a *Logical Plan*. You can examine this logical plan using {meth}`df.explain() <daft.DataFrame.explain>`:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {
                 "tags": []
@@ -177,20 +180,21 @@
                 }
             ],
             "source": [
                 "df.explain()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Our currently plan says that there is only one operation to be executed, which is an `InMemoryScan` operation that reads from a set of in-memory data.\n",
                 "\n",
-                "To execute all operations on all data in the current DataFrame's plan, you can use the `DataFrame.collect()` method."
+                "To execute all operations on all data in the current DataFrame's plan, you can use the {meth}`df.collect() <daft.DataFrame.collect>` method."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {
                 "tags": []
@@ -236,20 +240,21 @@
                 }
             ],
             "source": [
                 "df.collect()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "`DataFrame.collect()` is useful because it executes computations on **all** your data, and shows you a little preview of the materialized results. These results are then kept in memory so that subsequent operations will avoid recomputations.\n",
+                "{meth}`df.collect() <daft.DataFrame.collect>` is useful because it executes computations on **all** your data, and shows you a little preview of the materialized results. These results are then kept in memory so that subsequent operations will avoid recomputations.\n",
                 "\n",
-                "However, if you only wish to \"peek\" at your data instead of materializing the entire dataframe (e.g. your dataframe has a million rows, and you only want to view the first 10 without materializing the entire result set in memory), you can use `DataFrame.show(N)` instead to view the first `N` rows of your dataframe. This is especially useful when developing interactively on small samples of data."
+                "However, if you only wish to \"peek\" at your data instead of materializing the entire dataframe (e.g. your dataframe has a million rows, and you only want to view the first 10 without materializing the entire result set in memory), you can use {meth}`df.show(N) <daft.DataFrame.show>` instead to view the first `N` rows of your dataframe. This is especially useful when developing interactively on small samples of data."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {
                 "tags": []
@@ -289,25 +294,27 @@
                 }
             ],
             "source": [
                 "df.show(2)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Sorting Data"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "You can sort a dataframe with `DataFrame.sort`, which we do so here in descending order:"
+                "You can sort a dataframe with {meth}`df.sort() <daft.DataFrame.sort>`, which we do so here in descending order:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {
                 "tags": []
@@ -353,20 +360,21 @@
                 }
             ],
             "source": [
                 "df.sort(df[\"integers\"], desc=True).collect()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Data Selection\n",
                 "\n",
-                "You can limit the number of rows in a dataframe by calling `DataFrame.limit`."
+                "You can limit the number of rows in a dataframe by calling {meth}`df.limit() <daft.DataFrame.limit>`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {
                 "tags": []
@@ -404,18 +412,19 @@
             ],
             "source": [
                 "df_limited = df.limit(1)\n",
                 "df_limited.collect()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "To select just a few columns, you can use `DataFrame.select`:"
+                "To select just a few columns, you can use {meth}`df.select() <daft.DataFrame.select>`:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {
                 "tags": []
@@ -462,18 +471,19 @@
             ],
             "source": [
                 "df_selected = df.select(df[\"integers\"], df[\"floats\"])\n",
                 "df_selected.collect()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Column selection also allows you to rename columns using `Expression.alias`:"
+                "Column selection also allows you to rename columns using {meth}`.alias() <daft.expressions.Expression.alias>`:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "metadata": {
                 "tags": []
@@ -520,18 +530,19 @@
             ],
             "source": [
                 "df_renamed = df.select(df[\"integers\"].alias(\"ints\"), df[\"floats\"])\n",
                 "df_renamed.collect()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "To drop columns from the dataframe, call `DataFrame.exclude`:"
+                "To drop columns from the dataframe, call {meth}`df.exclude() <daft.DataFrame.exclude>`:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
             "metadata": {
                 "tags": []
@@ -649,17 +660,17 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Method Accessors\n",
                 "\n",
-                "Some Expression methods are only allowed on certain types and are accessible through \"method accessors\" such as the `Expression.str` accessor (see: [Expression Accessor Properties](expression-accessor-properties)).\n",
+                "Some Expression methods are only allowed on certain types and are accessible through \"method accessors\" such as the {meth}`.str <daft.expressions.Expression.str>` accessor (see: [Expression Accessor Properties](expression-accessor-properties)).\n",
                 "\n",
-                "For example, the `.str.length()` expression is only valid when run on a String column:"
+                "For example, the {meth}`.str.length() <daft.expressions.expressions.ExpressionStringNamespace.length>` expression is only valid when run on a String column:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
             "metadata": {
                 "tags": []
@@ -706,18 +717,19 @@
             ],
             "source": [
                 "df_E_length = df.with_column(\"strings_length\", df[\"strings\"].str.length())\n",
                 "df_E_length.collect()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Another example of a useful method accessor is the `.url` accessor. You can use `.url.download()` to download data from a column of URLs like so:"
+                "Another example of a useful method accessor is the {meth}`.url <daft.expressions.Expression.url>` accessor. You can use {meth}`.url.download() <daft.expressions.expressions.ExpressionUrlNamespace.download>` to download data from a column of URLs like so:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 14,
             "metadata": {
                 "tags": []
@@ -774,14 +786,15 @@
                 "    ],\n",
                 "})\n",
                 "image_downloaded_df = image_url_df.with_column(\"image_bytes\", image_url_df[\"urls\"].url.download())\n",
                 "image_downloaded_df.collect()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "For a full list of all Expression methods and operators, see: [Expressions API Docs](../api_docs/expressions.rst)"
             ]
         },
         {
@@ -789,14 +802,15 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Python object columns"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Daft Dataframes can also contain Python objects. Here is an example of how to create a dataframe with Python objects."
             ]
         },
         {
@@ -818,18 +832,19 @@
                 "py_df = daft.from_pydict({\n",
                 "    \"dogs\": [Dog(\"ruffles\"), Dog(\"waffles\"), Dog(\"doofus\")],\n",
                 "    \"owner\": [\"russell\", \"william\", \"david\"],\n",
                 "})"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Now, when we print our dataframe we can see that it contains our `Dog` Python objects! Also note that the type of the column is `Python`."
+                "Now, when we print our dataframe we can see that it contains our `Dog` Python objects! Also note that the type of the column is {meth}`Python <daft.DataType.python>`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 16,
             "metadata": {
                 "tags": []
@@ -875,20 +890,21 @@
                 }
             ],
             "source": [
                 "py_df.collect()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "To work with `Python` type columns, Daft provides a few useful Expression methods.\n",
+                "To work with {meth}`Python <daft.DataType.python>` type columns, Daft provides a few useful Expression methods.\n",
                 "\n",
-                "`Expression.apply` is useful to work on each Dog individually and apply a function.\n",
+                "{meth}`.apply <daft.expressions.Expression.apply>` is useful to work on each Dog individually and apply a function.\n",
                 "\n",
                 "Here's an example where we extract a string from each `Dog` by calling `.bark` on each `Dog` object and returning a new `Utf8` column."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 17,
@@ -945,15 +961,15 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### User-Defined Functions\n",
                 "\n",
-                "`.apply` makes it really easy to map a function on a single column, but is limited in 2 main ways:\n",
+                "{meth}`.apply <daft.expressions.Expression.apply>` makes it really easy to map a function on a single column, but is limited in 2 main ways:\n",
                 "\n",
                 "1. Only runs on a single column: some algorithms require multiple columns as inputs\n",
                 "2. Only runs on a single row: some algorithms run much more efficiently when run on a batch of rows instead\n",
                 "\n",
                 "To overcome these limitations, you can use User-Defined Functions (UDFs).\n",
                 "\n",
                 "See Also: [UDF User Guide](learn/user_guides/udf)"
@@ -1022,15 +1038,15 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Filtering Data\n",
                 "\n",
-                "You can filter rows in dataframe using `DataFrame.where`, which accepts a Boolean type Expression as an argument:"
+                "You can filter rows in dataframe using {meth}`df.where() <daft.DataFrame.where>`, which accepts a Boolean type Expression as an argument:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 19,
             "metadata": {
                 "tags": []
@@ -1072,14 +1088,15 @@
             "source": [
                 "# Keep only rows where values in column \"A\" are less than 3\n",
                 "df_filtered = df.where(df[\"integers\"] < 3)\n",
                 "df_filtered.collect()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Missing Data\n",
                 "\n",
                 "All columns in Daft are \"nullable\" by default. Unlike other frameworks such as Pandas, Daft differentiates between \"null\" (missing) and \"nan\" (stands for not a number - a special value indicating an invalid float)."
             ]
@@ -1135,18 +1152,19 @@
                 "    .with_column(\"floats_is_null\", missing_data_df[\"floats\"].is_null()) \\\n",
                 "    .with_column(\"floats_is_nan\", missing_data_df[\"floats\"].float.is_nan())\n",
                 "\n",
                 "missing_data_df.collect()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "To fill in missing values, a useful Expression is the `.if_else` expression which can be used to fill in values if the value is null:"
+                "To fill in missing values, a useful Expression is the {meth}`.if_else <daft.expressions.Expression.if_else>` expression which can be used to fill in values if the value is null:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 21,
             "metadata": {
                 "tags": []
@@ -1190,20 +1208,21 @@
             ],
             "source": [
                 "missing_data_df = missing_data_df.with_column(\"filled_in_floats\", (missing_data_df[\"floats\"].is_null()).if_else(0.0, missing_data_df[\"floats\"]))\n",
                 "missing_data_df.collect()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Merging Dataframes\n",
                 "\n",
-                "DataFrames can be joined with `.join`. Here is a naive example of a self-join where we join `df` on itself with column \"A\" as the join key."
+                "DataFrames can be joined with {meth}`df.join() <daft.DataFrame.join>`. Here is a naive example of a self-join where we join `df` on itself with column \"A\" as the join key."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 22,
             "metadata": {
                 "tags": []
@@ -1260,23 +1279,24 @@
                 }
             ],
             "source": [
                 "joined_df.collect()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Grouping and Aggregations\n",
                 "\n",
                 "Groupby aggregation operations over a dataset happens in 2 phases:\n",
                 "\n",
-                "1. Splitting the data into groups based on some criteria using `DataFrame.groupby`\n",
-                "2. Specifying how to aggregate the data for each group using `GroupedDataFrame.agg`\n",
+                "1. Splitting the data into groups based on some criteria using {meth}`df.groupby() <daft.DataFrame.groupby>`\n",
+                "2. Specifying how to aggregate the data for each group using {meth}`GroupedDataFrame.agg() <daft.dataframe.dataframe.GroupedDataFrame.agg>`\n",
                 "\n",
                 "Let's take a look at an example:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 24,
@@ -1344,14 +1364,15 @@
                 "        \"D\": [i for i in range(8)],\n",
                 "    }\n",
                 ")\n",
                 "grouping_df.collect()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "First we group by \"A\", so that we will evaluate rows with `A=foo` and `A=bar` separately in their respective groups."
             ]
         },
         {
@@ -1394,14 +1415,15 @@
             ],
             "source": [
                 "grouped_df = grouping_df.groupby(grouping_df[\"A\"])\n",
                 "grouped_df"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Now we can specify the aggregations we want to compute over columns C and D. Here we compute the sum over column C, and the mean over column D for each group:"
             ]
         },
         {
@@ -1449,14 +1471,15 @@
                 "    (grouped_df[\"C\"].alias(\"C_sum\"), \"sum\"),\n",
                 "    (grouped_df[\"D\"].alias(\"D_mean\"), \"mean\"),\n",
                 "])\n",
                 "aggregated_df.collect()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "These operations work as well when run over multiple groupby columns, which will produce one row for each combination of columns that occur in the DataFrame:"
             ]
         },
         {
@@ -1518,36 +1541,38 @@
                 "        (grouping_df[\"C\"].alias(\"C_sum\"), \"sum\"),\n",
                 "        (grouping_df[\"D\"].alias(\"D_mean\"), \"mean\"),\n",
                 "    ]) \\\n",
                 "    .collect()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Writing Data\n",
                 "\n",
                 "See: [Writing Data](df-writing-data)\n",
                 "\n",
-                "Writing data will execute your DataFrame and write the results out to the specified backend. For example, to write data out to Parquet:\n"
+                "Writing data will execute your DataFrame and write the results out to the specified backend. For example, to write data out to Parquet with {meth}`df.write_parquet() <daft.DataFrame.write_parquet>`:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 28,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "written_df = df.write_parquet(\"my-dataframe.parquet\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Note that writing your dataframe is a **blocking** operation that executes your DataFrame. It will return a new `DataFrame` that contains the filepaths to the written data:"
             ]
         },
         {
```

### Comparing `getdaft-0.1.5/docs/source/_static/daft-favicon.png` & `getdaft-0.1.6/docs/source/_static/daft-favicon.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/_static/daft-logo.png` & `getdaft-0.1.6/docs/source/_static/daft-logo.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/_static/daft_illustration.png` & `getdaft-0.1.6/docs/source/_static/daft_illustration.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/_static/dataframe-comp-table.csv` & `getdaft-0.1.6/docs/source/_static/dataframe-comp-table.csv`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/_static/execution_model.png` & `getdaft-0.1.6/docs/source/_static/execution_model.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/_static/header.css` & `getdaft-0.1.6/docs/source/_static/header.css`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/_static/high_level_architecture.png` & `getdaft-0.1.6/docs/source/_static/high_level_architecture.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/_static/in_memory_data_representation.png` & `getdaft-0.1.6/docs/source/_static/in_memory_data_representation.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/_static/mobile-menu.js` & `getdaft-0.1.6/docs/source/_static/mobile-menu.js`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/_static/tpch-1000sf.html` & `getdaft-0.1.6/docs/source/_static/tpch-1000sf.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/_static/tpch-100sf.html` & `getdaft-0.1.6/docs/source/_static/tpch-100sf.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/_static/tpch-nodes-count-daft-1000-sf.html` & `getdaft-0.1.6/docs/source/_static/tpch-nodes-count-daft-1000-sf.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/_templates/layout.html` & `getdaft-0.1.6/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/_templates/sections/header.html` & `getdaft-0.1.6/docs/source/_templates/sections/header.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/_templates/sections/mobile-menu.html` & `getdaft-0.1.6/docs/source/_templates/sections/mobile-menu.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/api_docs/dataframe.rst` & `getdaft-0.1.6/docs/source/api_docs/dataframe.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 DataFrame
 =========
 
 .. currentmodule:: daft
 
 .. autosummary::
     :nosignatures:
-    :toctree: dataframe_methods
+    :toctree: doc_gen/dataframe_methods
 
     DataFrame
 
 .. NOTE::
     Most DataFrame methods are **lazy**, meaning that they do not execute computation immediately when invoked. Instead, these operations are enqueued in
     the DataFrame's internal query plan, and are only executed when `Execution`_ DataFrame methods are called.
 
@@ -22,70 +22,71 @@
 ********************
 
 .. _df-select:
 .. _df-with-column:
 
 .. autosummary::
     :nosignatures:
-    :toctree: dataframe_methods
+    :toctree: doc_gen/dataframe_methods
 
     daft.DataFrame.select
     daft.DataFrame.with_column
     daft.DataFrame.exclude
     daft.DataFrame.explode
 
 Filtering Rows
 **************
 
 .. _df-where:
 .. _df-limit:
 
 .. autosummary::
     :nosignatures:
-    :toctree: dataframe_methods
+    :toctree: doc_gen/dataframe_methods
 
     daft.DataFrame.distinct
     daft.DataFrame.where
     daft.DataFrame.limit
 
 Reordering
 **********
 
 .. _df-sort:
 
 .. autosummary::
     :nosignatures:
-    :toctree: dataframe_methods
+    :toctree: doc_gen/dataframe_methods
 
     daft.DataFrame.sort
     daft.DataFrame.repartition
 
 Combining
 *********
 
 .. _df-join:
 
 .. autosummary::
     :nosignatures:
-    :toctree: dataframe_methods
+    :toctree: doc_gen/dataframe_methods
 
     daft.DataFrame.join
+    daft.DataFrane.concat
 
 .. _df-aggregations:
 
 Aggregations
 ************
 
 .. _df-groupby:
 .. _df-sum:
 .. _df-mean:
 
 .. autosummary::
     :nosignatures:
-    :toctree: dataframe_methods
+    :toctree: doc_gen/dataframe_methods
 
     daft.DataFrame.groupby
     daft.DataFrame.sum
     daft.DataFrame.mean
     daft.DataFrame.count
     daft.DataFrame.min
     daft.DataFrame.max
@@ -98,60 +99,60 @@
     These methods will execute the operations in your DataFrame and **are blocking**.
 
 Materialization
 ***************
 
 .. autosummary::
     :nosignatures:
-    :toctree: dataframe_methods
+    :toctree: doc_gen/dataframe_methods
 
     daft.DataFrame.collect
 
 Visualization
 *************
 
 .. _df-show:
 
 .. autosummary::
     :nosignatures:
-    :toctree: dataframe_methods
+    :toctree: doc_gen/dataframe_methods
 
     daft.DataFrame.show
 
 
 .. _df-write-data:
 
 Writing Data
 ************
 
 .. _df-writing-data:
 
 .. autosummary::
     :nosignatures:
-    :toctree: dataframe_methods
+    :toctree: doc_gen/dataframe_methods
 
     daft.DataFrame.write_parquet
     daft.DataFrame.write_csv
 
 Integrations
 ************
 
 .. _df-to-integrations:
 
 .. autosummary::
     :nosignatures:
-    :toctree: dataframe_methods
+    :toctree: doc_gen/dataframe_methods
 
     daft.DataFrame.to_pandas
     daft.DataFrame.to_ray_dataset
     daft.DataFrame.to_dask_dataframe
 
 Schema and Lineage
 ##################
 
 .. autosummary::
     :nosignatures:
-    :toctree: dataframe_methods
+    :toctree: doc_gen/dataframe_methods
 
     daft.DataFrame.explain
     daft.DataFrame.schema
     daft.DataFrame.column_names
```

### Comparing `getdaft-0.1.5/docs/source/api_docs/datatype.rst` & `getdaft-0.1.6/docs/source/api_docs/datatype.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 DataTypes
 =========
 
 .. currentmodule:: daft
 
 .. autosummary::
     :nosignatures:
-    :toctree: datatype_methods
+    :toctree: doc_gen/datatype_methods
 
     daft.DataType
 
 DataType Constructors
 #####################
 
 Construct Daft DataTypes using these constructor APIs.
@@ -26,15 +26,15 @@
 .. _api-datatypes-numeric:
 
 Numeric
 -------
 
 .. autosummary::
     :nosignatures:
-    :toctree: datatype_methods
+    :toctree: doc_gen/datatype_methods
 
     daft.DataType.int8
     daft.DataType.int16
     daft.DataType.int32
     daft.DataType.int64
     daft.DataType.uint8
     daft.DataType.uint16
@@ -47,92 +47,108 @@
 .. _api-datatypes-logical:
 
 Logical
 -------
 
 .. autosummary::
     :nosignatures:
-    :toctree: datatype_methods
+    :toctree: doc_gen/datatype_methods
 
     daft.DataType.bool
 
 
 .. _api-datatypes-string:
 
 Strings
 -------
 
 .. autosummary::
     :nosignatures:
-    :toctree: datatype_methods
+    :toctree: doc_gen/datatype_methods
 
     daft.DataType.binary
     daft.DataType.string
 
 
 .. _api-datatypes-temporal:
 
 Temporal
 --------
 
 .. autosummary::
     :nosignatures:
-    :toctree: datatype_methods
+    :toctree: doc_gen/datatype_methods
 
     daft.DataType.date
 
 
 .. _api-datatypes-nested:
 
 Nested
 ------
 
 .. autosummary::
     :nosignatures:
-    :toctree: datatype_methods
+    :toctree: doc_gen/datatype_methods
 
     daft.DataType.list
     daft.DataType.fixed_size_list
     daft.DataType.struct
 
 
 Python
 ------
 
 .. autosummary::
     :nosignatures:
-    :toctree: datatype_methods
+    :toctree: doc_gen/datatype_methods
 
     daft.DataType.python
 
 
 .. _api-datatypes-complex:
 
 Complex Types
 -------------
 
 Machine Learning
 ^^^^^^^^^^^^^^^^
 
 .. autosummary::
     :nosignatures:
-    :toctree: datatype_methods
+    :toctree: doc_gen/datatype_methods
 
     daft.DataType.embedding
 
 Computer Vision
 ^^^^^^^^^^^^^^^
 
 .. autosummary::
     :nosignatures:
-    :toctree: datatype_methods
+    :toctree: doc_gen/datatype_methods
 
     daft.DataType.image
 
+.. autosummary::
+    :nosignatures:
+
+    ImageMode
+
+.. autosummary::
+    :nosignatures:
+
+    ImageFormat
+
 
 Miscellaneous
 ^^^^^^^^^^^^^
 .. autosummary::
     :nosignatures:
-    :toctree: datatype_methods
+    :toctree: doc_gen/datatype_methods
 
     daft.DataType.null
+
+.. toctree::
+    :hidden:
+
+    datetype_image_format/daft.ImageFormat
+    datatype_image_mode/daft.ImageMode
```

### Comparing `getdaft-0.1.5/docs/source/api_docs/expressions.rst` & `getdaft-0.1.6/docs/source/api_docs/expressions.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Expressions
 ===========
 
 .. currentmodule:: daft
 
 .. autosummary::
     :nosignatures:
-    :toctree: expression_methods
+    :toctree: doc_gen/expression_methods
 
     daft.expressions.Expression
 
 Expression Constructors
 #######################
 
 .. autosummary::
     :nosignatures:
-    :toctree: expression_methods
+    :toctree: doc_gen/expression_methods
 
     daft.DataFrame.__getitem__
     daft.expressions.col
     daft.expressions.lit
 
 Operators
 #########
@@ -27,45 +27,45 @@
 
 Numeric
 *******
 
 Operations on numbers (floats and integers)
 
 .. autosummary::
-    :toctree: expression_methods
+    :toctree: doc_gen/expression_methods
 
     daft.expressions.Expression.__abs__
     daft.expressions.Expression.__add__
     daft.expressions.Expression.__sub__
     daft.expressions.Expression.__mul__
     daft.expressions.Expression.__truediv__
     daft.expressions.Expression.__mod__
 
 Logical
 *******
 
 Operations on logical expressions (True/False booleans)
 
 .. autosummary::
-    :toctree: expression_methods
+    :toctree: doc_gen/expression_methods
 
     daft.expressions.Expression.__invert__
     daft.expressions.Expression.__and__
     daft.expressions.Expression.__or__
     daft.expressions.Expression.if_else
 
 .. _api-comparison-expression:
 
 Comparisons
 ***********
 
 Comparing expressions and values, returning a logical expression
 
 .. autosummary::
-    :toctree: expression_methods
+    :toctree: doc_gen/expression_methods
 
     daft.expressions.Expression.__lt__
     daft.expressions.Expression.__le__
     daft.expressions.Expression.__eq__
     daft.expressions.Expression.__ne__
     daft.expressions.Expression.__gt__
     daft.expressions.Expression.__ge__
@@ -74,102 +74,121 @@
 .. _expression-accessor-properties:
 
 .. _api-float-expression-operations:
 
 Floats
 ******
 
-Operations on strings, accessible through the ``Expression.float`` method accessor.
+Operations on strings, accessible through the :meth:`Expression.float <daft.expressions.Expression.float>` method accessor.
 
 Example: ``e1.float.is_nan()``
 
 .. autosummary::
-    :toctree: expression_methods
+    :toctree: doc_gen/expression_methods
 
+    daft.expressions.Expression.float
     daft.expressions.expressions.ExpressionFloatNamespace.is_nan
 
 .. _api-string-expression-operations:
 
 Strings
 *******
 
-Operations on strings, accessible through the ``Expression.str`` method accessor.
+Operations on strings, accessible through the :meth:`Expression.str <daft.expressions.Expression.str>` method accessor.
 
 Example: ``e1.str.concat(e2)``
 
 .. autosummary::
-    :toctree: expression_methods
+    :toctree: doc_gen/expression_methods
 
+    daft.expressions.Expression.str
     daft.expressions.expressions.ExpressionStringNamespace.concat
     daft.expressions.expressions.ExpressionStringNamespace.contains
     daft.expressions.expressions.ExpressionStringNamespace.endswith
     daft.expressions.expressions.ExpressionStringNamespace.startswith
     daft.expressions.expressions.ExpressionStringNamespace.length
 
 .. _api-expressions-temporal:
 
 Dates
 *****
 
-Operations on datetimes, accessible through the ``Expression.dt`` method accessor:
+Operations on datetimes, accessible through the :meth:`Expression.dt <daft.expressions.Expression.dt>` method accessor:
 
 Example: ``e.dt.day()``
 
 .. autosummary::
     :nosignatures:
-    :toctree: expression_methods
+    :toctree: doc_gen/expression_methods
 
+    daft.expressions.Expression.dt
     daft.expressions.expressions.ExpressionDatetimeNamespace.day
     daft.expressions.expressions.ExpressionDatetimeNamespace.month
     daft.expressions.expressions.ExpressionDatetimeNamespace.year
     daft.expressions.expressions.ExpressionDatetimeNamespace.day_of_week
 
 .. _api-expressions-urls:
 
 URLs
 ****
 
-Operations on URLs, accessible through the ``Expression.url`` method accessor:
+Operations on URLs, accessible through the :meth:`Expression.url <daft.expressions.Expression.url>` method accessor:
 
 Example: ``e.url.download()``
 
 .. autosummary::
     :nosignatures:
-    :toctree: expression_methods
+    :toctree: doc_gen/expression_methods
 
+    daft.expressions.Expression.url
     daft.expressions.expressions.ExpressionUrlNamespace.download
 
 .. _api-expressions-images:
 
 Images
 ******
 
-Operations on images, accessible through the ``Expression.image`` method accessor:
+Operations on images, accessible through the :meth:`Expression.image <daft.expressions.Expression.image>` method accessor:
 
 Example: ``e.image.resize()``
 
 .. autosummary::
     :nosignatures:
-    :toctree: expression_methods
+    :toctree: doc_gen/expression_methods
 
+    daft.expressions.Expression.image
     daft.expressions.expressions.ExpressionImageNamespace.resize
     daft.expressions.expressions.ExpressionImageNamespace.decode
+    daft.expressions.expressions.ExpressionImageNamespace.encode
+
+
+Nested
+******
+
+Operations on nested types (such as List and FixedSizeList), accessible through the ``Expression.list`` method accessor.
+
+Example: ``e1.str.concat(e2)``
+
+.. autosummary::
+    :toctree: expression_methods
+
+    daft.expressions.expressions.ExpressionListNamespace.join
 
 
 Changing Column Names/Types
 ###########################
 
 .. autosummary::
     :nosignatures:
-    :toctree: expression_methods
+    :toctree: doc_gen/expression_methods
 
     daft.expressions.Expression.alias
     daft.expressions.Expression.cast
 
 Running Python Functions
 ########################
 
 .. autosummary::
     :nosignatures:
-    :toctree: expression_methods
+    :toctree: doc_gen/expression_methods
 
     daft.expressions.Expression.apply
```

### Comparing `getdaft-0.1.5/docs/source/api_docs/groupby.rst` & `getdaft-0.1.6/docs/source/api_docs/groupby.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 GroupBy
 =======
 
 When performing aggregations such as sum, mean and count, you may often want to group data by certain keys and aggregate within those keys.
 
-Calling ``DataFrame.groupby`` returns a ``GroupedDataFrame`` object which is a view of the original DataFrame but with additional context on which keys to group on. You can then call various aggregation methods to run the aggregation within each group, returning a new DataFrame.
+Calling :meth:`df.groupby() <daft.DataFrame.groupby>` returns a ``GroupedDataFrame`` object which is a view of the original DataFrame but with additional context on which keys to group on. You can then call various aggregation methods to run the aggregation within each group, returning a new DataFrame.
 
 .. currentmodule:: daft
 
 .. autosummary::
     :nosignatures:
-    :toctree: dataframe_methods
+    :toctree: doc_gen/dataframe_methods
 
     daft.dataframe.dataframe.GroupedDataFrame.sum
     daft.dataframe.dataframe.GroupedDataFrame.mean
     daft.dataframe.dataframe.GroupedDataFrame.min
     daft.dataframe.dataframe.GroupedDataFrame.max
     daft.dataframe.dataframe.GroupedDataFrame.agg
```

### Comparing `getdaft-0.1.5/docs/source/api_docs/input_output.rst` & `getdaft-0.1.6/docs/source/api_docs/input_output.rst`

 * *Files 12% similar despite different names*

```diff
@@ -11,106 +11,106 @@
 .. _df-io-in-memory:
 
 Python Objects
 ~~~~~~~~~~~~~~
 
 .. autosummary::
     :nosignatures:
-    :toctree: io_functions
+    :toctree: doc_gen/io_functions
 
     daft.from_pylist
     daft.from_pydict
     daft.DataFrame.to_pydict
 
 Arrow
 ~~~~~
 
 .. autosummary::
     :nosignatures:
-    :toctree: io_functions
+    :toctree: doc_gen/io_functions
 
 
 .. autosummary::
     :nosignatures:
-    :toctree: io_functions
+    :toctree: doc_gen/io_functions
 
     daft.from_arrow
     daft.DataFrame.to_arrow
 
 Pandas
 ~~~~~~
 
 .. autosummary::
     :nosignatures:
-    :toctree: io_functions
+    :toctree: doc_gen/io_functions
 
     daft.from_pandas
     daft.DataFrame.to_pandas
 
 File Paths
 ~~~~~~~~~~
 
 .. autosummary::
     :nosignatures:
-    :toctree: io_functions
+    :toctree: doc_gen/io_functions
 
     daft.from_glob_path
 
 Files
 -----
 
 .. _df-io-files:
 
 Parquet
 ~~~~~~~
 
 .. autosummary::
     :nosignatures:
-    :toctree: io_functions
+    :toctree: doc_gen/io_functions
 
     daft.read_parquet
     daft.DataFrame.write_parquet
 
 CSV
 ~~~
 
 .. autosummary::
     :nosignatures:
-    :toctree: io_functions
+    :toctree: doc_gen/io_functions
 
     daft.read_csv
     daft.DataFrame.write_csv
 
 JSON
 ~~~~
 
 .. autosummary::
     :nosignatures:
-    :toctree: io_functions
+    :toctree: doc_gen/io_functions
 
     daft.read_json
 
 Integrations
 ------------
 
 .. _df-io-integrations:
 
 Ray Datasets
 ~~~~~~~~~~~~
 
 .. autosummary::
     :nosignatures:
-    :toctree: io_functions
+    :toctree: doc_gen/io_functions
 
     daft.from_ray_dataset
     daft.DataFrame.to_ray_dataset
 
 Dask
 ~~~~
 
 .. autosummary::
     :nosignatures:
-    :toctree: io_functions
+    :toctree: doc_gen/io_functions
 
     daft.from_dask_dataframe
     daft.DataFrame.to_dask_dataframe
```

### Comparing `getdaft-0.1.5/docs/source/benchmarks/index.rst` & `getdaft-0.1.6/docs/source/benchmarks/index.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/conf.py` & `getdaft-0.1.6/docs/source/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     "sphinx_reredirects",
     "sphinx.ext.autodoc",
     "sphinx.ext.napoleon",
     "sphinx.ext.autosummary",
     "sphinx.ext.linkcode",
     "IPython.sphinxext.ipython_console_highlighting",
     "myst_nb",
+    "sphinx_copybutton",
 ]
 
 templates_path = ["_templates"]
 exclude_patterns = ["release_notes/_template.rst"]
 
 
 # -- Options for Notebook rendering
@@ -58,14 +59,24 @@
     "extra_navbar": "",
     # This is how many levels are shown on the secondary sidebar
     "show_toc_level": 2,
     # Remove title under the logo on the left sidebar
     "logo_only": True,
 }
 
+# -- Copy button configuration
+
+# This pattern matches:
+# - Python Repl prompts (">>> ") and it's continuation ("... ")
+# - Bash prompts ("$ ")
+# - IPython prompts ("In []: ", "In [999]: ") and it's continuations
+#   ("  ...: ", "     : ")
+copybutton_prompt_text = r">>> |\.\.\. |\$ |In \[\d*\]: | {2,5}\.\.\.: | {5,8}: "
+copybutton_prompt_is_regexp = True
+
 # -- Options for redirecting URLs
 redirects = {
     "learn/install": "../install.html",
     "learn/user_guides/dataframes": "intro-dataframes.html",
     "learn/user_guides/types_and_ops": "intro-dataframes.html",
     "learn/user_guides/remote_cluster_execution": "scaling-up.html",
     "learn/quickstart": "learn/10-min.html",
```

### Comparing `getdaft-0.1.5/docs/source/dataframe_comparison.rst` & `getdaft-0.1.6/docs/source/dataframe_comparison.rst`

 * *Files 3% similar despite different names*

```diff
@@ -48,8 +48,8 @@
 Ray Datasets
 ------------
 
 Ray Datasets make it easy to feed data really efficiently into Ray's model training and inference ecosystem. Datasets also provide basic functionality for data preprocessing such as mapping a function over each data item, filtering data etc.
 
 However, Ray Datasets are not a fully-fledged Dataframe abstraction (and `it is explicit in not being an ETL framework for data science <https://docs.ray.io/en/latest/data/faq.html#what-should-i-not-use-ray-datasets-for>`_) which means that it lacks key features in data querying, visualization and aggregations.
 
-Instead, Ray Data is a perfect destination for processed data from DaFt Dataframes to be sent to with a simple ``df.to_ray_dataset()`` call. This is useful as an entrypoint into your model training and inference ecosystem!
+Instead, Ray Data is a perfect destination for processed data from DaFt Dataframes to be sent to with a simple :meth:`df.to_ray_dataset() <daft.DataFrame.to_ray_dataset>` call. This is useful as an entrypoint into your model training and inference ecosystem!
```

### Comparing `getdaft-0.1.5/docs/source/index.rst` & `getdaft-0.1.6/docs/source/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Daft Documentation
 ==================
 
-Daft is a **fast and scalable Python dataframe** for Complex Data and Machine Learning workloads.
+Daft is a **fast and scalable Python dataframe** for complex data and machine learning workloads.
 
 .. NOTE::
 
    *Daft is currently in its Beta release phase - please expect bugs and rapid improvements to the project. We welcome user feedback/feature requests in our* `Discussions forums <https://github.com/Eventual-Inc/Daft/discussions>`_.
 
 Installing Daft
 ---------------
@@ -25,15 +25,15 @@
 1. Read a CSV into a Daft dataframe
 2. Work with images using the Pillow library in Daft
 3. Downloading data from URLs
 
 Use Daft
 --------
 
-Reference the :doc:`Daft API Documentation <api_docs/index>` for Daft.
+Refer to the :doc:`Daft API Documentation <api_docs/index>`.
 
 Keep up to date
 ---------------
 
 Keep up to date with the latest features and fixes in Daft with our :doc:`Release Notes <release_notes/index>`.
 
 Compare Daft to alternatives
```

### Comparing `getdaft-0.1.5/docs/source/install.rst` & `getdaft-0.1.6/docs/source/install.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,52 @@
 Installation
 ============
 
 To install Daft, run this from your terminal:
 
-``pip install getdaft``
+.. code-block:: shell
+
+    pip install -U getdaft
 
 Extra Dependencies
 ------------------
 
 Some Daft functionality may also require other dependencies, which are specified as "extras":
 
-1. Installing ``getdaft[aws]`` will install the extra dependencies required to use Daft with AWS services such as AWS S3
-2. Installing ``getdaft[ray]`` will install the extra dependencies required to use Daft with Ray
+To install Daft with the extra dependencies required for interacting with AWS services, such as AWS S3, run:
+
+.. code-block:: shell
+
+    pip install -U getdaft[aws]
+
+To install Daft with the extra dependencies required for running distributed Daft on top of a `Ray cluster <https://docs.ray.io/en/latest/index.html>`__, run:
+
+.. code-block:: shell
+
+    pip install -U getdaft[ray]
 
 To install Daft with all extras, run:
 
-``pip install getdaft[all]``
+.. code-block:: shell
+
+    pip install -U getdaft[all]
 
 Advanced Installation
 ---------------------
 
 Installing Nightlies
 ^^^^^^^^^^^^^^^^^^^^
 
 If you wish to use Daft at the bleeding edge of development, you may also install the nightly build of Daft which is built every night against the ``main`` branch:
 
-``pip install getdaft --pre --extra-index-url https://pypi.anaconda.org/daft-nightly/simple``
+.. code-block:: shell
+
+    pip install -U getdaft --pre --extra-index-url https://pypi.anaconda.org/daft-nightly/simple
 
 Installing Daft from source
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-``pip install https://github.com/Eventual-Inc/Daft/archive/refs/heads/main.zip``
+.. code-block:: shell
+
+    pip install -U https://github.com/Eventual-Inc/Daft/archive/refs/heads/main.zip
 
 Please note that Daft requires the Rust toolchain in order to build from source.
```

### Comparing `getdaft-0.1.5/docs/source/learn/index.rst` & `getdaft-0.1.6/docs/source/learn/index.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/learn/key_concepts.rst` & `getdaft-0.1.6/docs/source/learn/key_concepts.rst`

 * *Files 5% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 .. image:: /_static/daft_illustration.png
    :alt: Daft python dataframes make it easy to load any data such as PDF documents, images, protobufs, csv, parquet and audio files into a table dataframe structure for easy querying
    :width: 500
    :align: center
 
 Using this abstraction of a DataFrame, you can run common tabular operations such as:
 
-1. Filters: ``df.where(...)``
-2. Creating new columns as a computation of existing columns: ``df.with_column(...)``
-3. Joining two tables together: ``df.join(...)``
-4. Sorting a table by the values in specified column(s): ``df.sort(...)``
-5. Grouping and aggregations: ``df.groupby(...).agg(...)``
+1. Filters: :meth:`df.where(...) <daft.DataFrame.where>`
+2. Creating new columns as a computation of existing columns: :meth:`df.with_column(...) <daft.DataFrame.with_column>`
+3. Joining two tables together: :meth:`df.join(...) <daft.DataFrame.join>`
+4. Sorting a table by the values in specified column(s): :meth:`df.sort(...) <daft.DataFrame.sort>`
+5. Grouping and aggregations: :meth:`df.groupby(...).agg(...) <daft.DataFrame.groupby>`
 
 Daft DataFrames are:
 
 1. **Distributed:** your data is split into *Partitions* and can be processed in parallel
 2. **Lazy:** computations are enqueued in a query plan, and only executed when requested
 3. **Complex:** columns can contain complex datatypes such as tensors, images and Python objects
 
@@ -67,15 +67,15 @@
     | Int64   | Int64   |
     +=========+=========+
     +---------+---------+
     (No data to display: Dataframe not materialized)
 
 Notice that when printing the DataFrame, Daft will say that there is "No data to display". This is because Daft enqueues all your operations into a "query plan" instead of executing it immediately when you define your operations.
 
-To actually execute your DataFrame, you can call a method such as ``df.show()``. This method will run just the necessary computation required to show the first few rows of your DataFrame:
+To actually execute your DataFrame, you can call a method such as :meth:`df.show() <daft.DataFrame.show>`. This method will run just the necessary computation required to show the first few rows of your DataFrame:
 
 .. code:: python
 
     df.show()
 
 .. code:: none
 
@@ -139,23 +139,23 @@
     (Showing first 3 rows)
 
 Similarly, working with complex types such as images, tensors, Python objects and more are greatly simplified when using Daft!
 
 Expressions
 -----------
 
-The other important concept to understand when working with Daft are ``Expressions``.
+The other important concept to understand when working with Daft are **expressions**.
 
-Because Daft is "lazy", it needs a way to represent computations that need to be performed on its data so that it can execute these computations at some later time. The answer to this is an ``Expression``!
+Because Daft is "lazy", it needs a way to represent computations that need to be performed on its data so that it can execute these computations at some later time. The answer to this is an :class:`~daft.expressions.Expression`!
 
 The simplest Expressions are:
 
-1. The column expression: ``col("a")`` which is used to refer to "some column named 'a'"
+1. The column expression: :func:`col("a") <daft.expressions.col>` which is used to refer to "some column named 'a'"
 2. Or, if you already have an existing DataFrame ``df`` with a column named "a", you can refer to its column like we did before with square brackets: ``df["a"]``
-3. The literal expression: ``lit(100)`` which represents a column that always takes on the provided value
+3. The literal expression: :func:`lit(100) <daft.expressions.lit>` which represents a column that always takes on the provided value
 
 Daft then provides an extremely rich Expressions library to allow you to compose different computations that need to happen. For example:
 
 .. code:: python
 
     from daft import col, DataType
```

### Comparing `getdaft-0.1.5/docs/source/learn/tutorials.rst` & `getdaft-0.1.6/docs/source/learn/tutorials.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/learn/user_guides/aggregations.rst` & `getdaft-0.1.6/docs/source/learn/user_guides/aggregations.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/learn/user_guides/dataframe-operations.rst` & `getdaft-0.1.6/docs/source/learn/user_guides/dataframe-operations.rst`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 However, the Daft DataFrame is table containing equal-length columns. Many operations affect the entire table at once, affecting the ordering or sizes of all columns.
 
 This section of the user guide covers these operations, and how to use them.
 
 Selecting Columns
 -----------------
 
-Select specific columns in a DataFrame using ``.select``, which also takes Expressions as an input.
+Select specific columns in a DataFrame using :meth:`df.select() <daft.DataFrame.select>`, which also takes Expressions as an input.
 
 .. code-block:: python
 
     import daft
 
     df = daft.from_pydict({"A": [1, 2, 3], "B": [4, 5, 6]})
 
@@ -30,15 +30,15 @@
     +---------+
     |       2 |
     +---------+
     |       3 |
     +---------+
     (Showing first 3 rows)
 
-A useful alias for ``.select`` is indexing a DataFrame with a list of column names or Expressions:
+A useful alias for :meth:`df.select() <daft.DataFrame.select>` is indexing a DataFrame with a list of column names or Expressions:
 
 .. code-block:: python
 
     df[["A", "B"]].show()
 
 .. code-block:: none
 
@@ -50,15 +50,15 @@
     +---------+---------+
     |       2 |       5 |
     +---------+---------+
     |       3 |       6 |
     +---------+---------+
     (Showing first 3 rows)
 
-Sometimes, it may be useful to exclude certain columns from a DataFrame. This can be done with ``.exclude``:
+Sometimes, it may be useful to exclude certain columns from a DataFrame. This can be done with :meth:`df.exclude() <daft.DataFrame.exclude>`:
 
 .. code-block:: python
 
     df.exclude("A").show()
 
 .. code-block:: none
 
@@ -70,15 +70,15 @@
     +---------+
     |       5 |
     +---------+
     |       6 |
     +---------+
     (Showing first 3 rows)
 
-As we have already seen in previous guides, adding a new column can be achieved with ``.with_column``:
+As we have already seen in previous guides, adding a new column can be achieved with :meth:`df.with_column() <daft.DataFrame.with_column>`:
 
 .. code-block:: python
 
     df.with_column("C", df["A"] + df["B"]).show()
 
 .. code-block:: none
 
@@ -93,15 +93,15 @@
     |       3 |       6 |       9 |
     +---------+---------+---------+
     (Showing first 3 rows)
 
 Selecting Rows
 --------------
 
-We can limit the rows to the first ``N`` rows using ``.limit``:
+We can limit the rows to the first ``N`` rows using :meth:`df.limit(N) <daft.DataFrame.limit>`:
 
 .. code-block:: python
 
     df = daft.from_pydict({
         "A": [1, 2, 3, 4, 5],
         "B": [6, 7, 8, 9, 10],
     })
@@ -119,15 +119,15 @@
     |       2 |       7 |
     +---------+---------+
     |       3 |       8 |
     +---------+---------+
     (Showing first 3 rows)
 
 
-We can also filter rows using ``.where``, which takes an input a Logical Expression predicate:
+We can also filter rows using :meth:`df.where() <daft.DataFrame.where>`, which takes an input a Logical Expression predicate:
 
 .. code-block:: python
 
     df.where(df["A"] > 3).show()
 
 .. code-block:: none
 
@@ -140,15 +140,15 @@
     |       5 |      10 |
     +---------+---------+
     (Showing first 2 rows)
 
 Combining DataFrames
 --------------------
 
-Two DataFrames can be column-wise joined using ``.join``.
+Two DataFrames can be column-wise joined using :meth:`df.join() <daft.DataFrame.join>`.
 
 This requires a "join key", which can be supplied as the ``on`` argument if both DataFrames have the same name for their key columns, or the ``left_on`` and ``right_on`` argument if the key column has different names in each dataframe.
 
 Daft also supports multi-column joins key you have a join key comprising of multiple columns!
 
 .. code-block:: python
 
@@ -170,15 +170,15 @@
     |       3 |       6 |       9 |
     +---------+---------+---------+
     (Showing first 3 rows)
 
 Reordering Rows
 ---------------
 
-Rows in a DataFrame can be reordered based on some column using ``.sort``. Daft also supports multi-column sorts for sorting on multiple columns at once.
+Rows in a DataFrame can be reordered based on some column using :meth:`df.sort() <daft.DataFrame.sort>`. Daft also supports multi-column sorts for sorting on multiple columns at once.
 
 .. code-block:: python
 
     df = daft.from_pydict({
         "A": [1, 2, 3],
         "B": [6, 7, 8],
     })
@@ -198,15 +198,15 @@
     |       1 |       6 |
     +---------+---------+
     (Showing first 3 rows)
 
 Exploding Columns
 -----------------
 
-The ``df.explode`` method can be used to explode a column containing a list of values into multiple rows. All other rows will be **duplicated**.
+The :meth:`df.explode() <daft.DataFrame.explode>` method can be used to explode a column containing a list of values into multiple rows. All other rows will be **duplicated**.
 
 .. code:: python
 
     df = daft.from_pydict({
         "A": [1, 2, 3],
         "B": [[1, 2, 3], [4, 5, 6], [7, 8, 9]],
     })
@@ -238,14 +238,14 @@
     (Showing first 8 rows)
 
 Repartitioning
 --------------
 
 Daft is a distributed DataFrame, and the dataframe is broken in multiple "partitions" which are distributed across the cluster.
 
-You may choose to increase or decrease the number of partitions with ``.repartition``.
+You may choose to increase or decrease the number of partitions with :meth:`df.repartition() <daft.DataFrame.partition>`.
 
 1. Increasing the number of partitions to 2x the total number of CPUs could help with resource utilization
 2. If each partition is potentially overly large (e.g. containing large images), causing memory issues, you may increase the number of partitions to reduce the size of each individual partition
 3. If you have too many partitions, global operations such as a sort or a join may take longer to execute
 
 A good rule of thumb is to keep the number of partitions as twice the number of CPUs available on your backend, increasing the number of partitions as necessary if they cannot be processed in memory.
```

### Comparing `getdaft-0.1.5/docs/source/learn/user_guides/datatypes.rst` & `getdaft-0.1.6/docs/source/learn/user_guides/datatypes.rst`

 * *Files 18% similar despite different names*

```diff
@@ -15,60 +15,60 @@
 -----------------
 
 Numeric DataTypes allows Daft to represent numbers. These numbers can differ in terms of the number of bits used to represent them (8, 16, 32 or 64 bits) and the semantic meaning of those bits
 (float vs integer vs unsigned integers).
 
 Examples:
 
-1. ``DataType.int8()``: represents an 8-bit signed integer (-128 to 127)
-2. ``DataType.float32()``: represents a 32-bit float (a float number with about 7 decimal digits of precision)
+1. :meth:`DataType.int8() <daft.DataType.int8>`: represents an 8-bit signed integer (-128 to 127)
+2. :meth:`DataType.float32() <daft.DataType.float32>`: represents a 32-bit float (a float number with about 7 decimal digits of precision)
 
 Columns/expressions with these datatypes can be operated on with many numeric expressions such as ``+`` and ``*``.
 
 See also:
 
 * :ref:`Numeric DataTypes <api-datatypes-numeric>`
 * :ref:`Numeric Expressions <userguide-numeric-expressions>`
 
 Logical DataTypes
 -----------------
 
-The ``DataType.bool()`` DataType represents values which are boolean values: ``True``, ``False`` or ``Null``.
+The :meth:`DataType.bool() <daft.DataType.bool>` DataType represents values which are boolean values: ``True``, ``False`` or ``Null``.
 
-Columns/expressions with this dtype can be operated on using logical expressions such as ``&`` and ``if_else``.
+Columns/expressions with this dtype can be operated on using logical expressions such as ``&`` and :meth:`.if_else() <daft.expressions.Expression.if_else>`.
 
 See also:
 
 * :ref:`Logical DataTypes <api-datatypes-logical>`
 * :ref:`Logical Expressions <userguide-logical-expressions>`
 
 String Types
 ------------
 
 Daft has string types, which represent a variable-length string of characters.
 
-As a convenience method, string types also support the ``+`` Expression, which has been overloaded to support concatenation of elements between two ``DataType.string()`` columns.
+As a convenience method, string types also support the ``+`` Expression, which has been overloaded to support concatenation of elements between two :meth:`DataType.string() <daft.DataType.string>` columns.
 
-1. ``DataType.string()``: represents a string of UTF-8 characters
-2. ``DataType.binary()``: represents a string of bytes
+1. :meth:`DataType.string() <daft.DataType.string>`: represents a string of UTF-8 characters
+2. :meth:`DataType.binary() <daft.DataType.binary>`: represents a string of bytes
 
 See also:
 
 * :ref:`String DataTypes <api-datatypes-string>`
 * :ref:`String Expressions <userguide-string-expressions>`
 
 Temporal
 --------
 
 Temporal dtypes represent data that have to do with time.
 
 Examples:
 
-1. ``DataType.date()``: represents a Date (year, month and day)
-2. ``DataType.duration()``: [COMING SOON] represents the duration between two instances in time
+1. :meth:`DataType.date() <daft.DataType.date>`: represents a Date (year, month and day)
+2. :meth:`DataType.duration() <daft.DataType.duration>`: [COMING SOON] represents the duration between two instances in time
 
 NOTE: Many temporal types are still a work-in-progress!
 
 See also:
 
 * :ref:`Temporal DataTypes <api-datatypes-temporal>`
 * :ref:`Temporal Expressions <api-expressions-temporal>`
@@ -76,47 +76,47 @@
 Nested
 ------
 
 Nested DataTypes wrap other DataTypes, allowing you to compose types into complex datastructures.
 
 Examples:
 
-1. ``DataType.list(child_dtype)``: represents a list where each element is of the child dtype
-2. ``DataType.struct({"field_name": child_dtype})``: represents a structure that has children dtypes, each mapped to a field name
+1. :meth:`DataType.list(child_dtype) <daft.DataType.list>`: represents a list where each element is of the child dtype
+2. :meth:`DataType.struct({"field_name": child_dtype}) <daft.DataType.struct>`: represents a structure that has children dtypes, each mapped to a field name
 
 See also:
 
 * :ref:`Nested DataTypes <api-datatypes-nested>`
 
 Python
 ------
 
-The ``DataType.python()`` dtype represent items that are Python objects.
+The :meth:`DataType.python() <daft.DataType.python>` dtype represent items that are Python objects.
 
 .. WARNING::
 
     Daft does not impose any invariants about what *Python types* these objects are. To Daft, these are just generic Python objects!
 
 Python is AWESOME because it's so flexible, but it's also slow and memory inefficient! Thus we recommend:
 
 1. **Cast early!**: Casting your Python data into native Daft DataTypes if possible - this results in much more efficient downstream data serialization and computation.
 2. **Use Python UDFs**: If there is no suitable Daft representation for your Python objects, use Python UDFs to process your Python data and extract the relevant data to be returned as native Daft DataTypes!
 
 .. NOTE::
 
-    If you work with Python classes for a generalizable use-case (e.g. images, documents, protobufs), it may be that these types are good candidates for "promotion" into a native Daft type!
+    If you work with Python classes for a generalizable use-case (e.g. documents, protobufs), it may be that these types are good candidates for "promotion" into a native Daft type!
     Please get in touch with the Daft team and we would love to work together on building your type into canonical Daft types.
 
 Complex Types
 -------------
 
 Daft supports many more interesting complex DataTypes, for example:
 
-* :meth:`~daft.DataType.embedding()`: Lower-dimensional vector representation of data (e.g. words)
-* :meth:`~daft.DataType.image()`: NHWC images
+* :meth:`DataType.embedding() <daft.DataType.embedding>`: Lower-dimensional vector representation of data (e.g. words)
+* :meth:`DataType.image() <daft.DataType.image>`: NHWC images
 
 Daft abstracts away the in-memory representation of your data and provides kernels for many common operations on top of these data types. For supported image operations see the :ref:`image expressions API reference <api-expressions-images>`.
 
 For more complex algorithms, you can also drop into a Python UDF to process this data using your custom Python libraries.
 
 Please add suggestions for new DataTypes to our Github Discussions page!
```

### Comparing `getdaft-0.1.5/docs/source/learn/user_guides/expressions.rst` & `getdaft-0.1.6/docs/source/learn/user_guides/expressions.rst`

 * *Files 3% similar despite different names*

```diff
@@ -27,38 +27,38 @@
     col(A)
 
 When we evaluate this ``df["A"]`` Expression, it will evaluate to the column from the ``df`` DataFrame with name "A"!
 
 Refer to a column with a certain name
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-You may also find it necessary in certain situations to create an Expression with just the name of a column, without having an existing DataFrame to refer to. You can do this with the ``col`` helper:
+You may also find it necessary in certain situations to create an Expression with just the name of a column, without having an existing DataFrame to refer to. You can do this with the :func:`~daft.expressions.col` helper:
 
 .. code:: python
 
     from daft import col
 
     # Refers to a column named "A"
     col("A")
 
 When this Expression is evaluated, it will resolve to "the column named A" in whatever evaluation context it is used within!
 
 Literals
 ^^^^^^^^
 
-You may find yourself needing to hardcode a "single value" oftentimes as an expression. Daft provides a ``lit`` helper to do so:
+You may find yourself needing to hardcode a "single value" oftentimes as an expression. Daft provides a :func:`~daft.expressions.lit` helper to do so:
 
 .. code:: python
 
     from daft import lit
 
     # Refers to an expression which always evaluates to 42
     lit(42)
 
-This special ``lit`` expression we just created evaluates always to the value ``42``.
+This special :func:`~daft.expressions.lit` expression we just created evaluates always to the value ``42``.
 
 .. _userguide-numeric-expressions:
 
 Numeric Expressions
 -------------------
 
 Since column "A" is an integer, we can run numeric computation such as addition, division and checking its value. Here are some examples where we create new columns using the results of such computations:
@@ -86,17 +86,17 @@
     +---------+-------------+----------------+-----------+
     |       2 |           3 |            1   | true      |
     +---------+-------------+----------------+-----------+
     |       3 |           4 |            1.5 | true      |
     +---------+-------------+----------------+-----------+
     (Showing first 3 of 3 rows)
 
-Notice that the returned types of these operations are also well-typed according to their input types. For example, calling ``df["A"] > 1`` returns a column of type ``Boolean``.
+Notice that the returned types of these operations are also well-typed according to their input types. For example, calling ``df["A"] > 1`` returns a column of type :meth:`Boolean <daft.DataType.boolean>`.
 
-Both The Float and Int types are numeric types, and inherit many of the same arithmetic Expression operations. You may find the full list of numeric operations in the :ref:`Expressions API reference <api-numeric-expression-operations>`.
+Both the :meth:`Float <daft.DataType.float>` and :meth:`Int <daft.DataType.int>` types are numeric types, and inherit many of the same arithmetic Expression operations. You may find the full list of numeric operations in the :ref:`Expressions API reference <api-numeric-expression-operations>`.
 
 .. _userguide-string-expressions:
 
 String Expressions
 ------------------
 
 Daft also lets you have columns of strings in a DataFrame. Let's take a look!
@@ -137,17 +137,17 @@
     +--------+--------+
     | bar    | barfoo |
     +--------+--------+
     | baz    | bazfoo |
     +--------+--------+
     (Showing first 3 rows)
 
-There are also many string operators that are accessed through a separate ``Expression.str.*`` "method namespace".
+There are also many string operators that are accessed through a separate :meth:`.str.* <daft.expressions.Expresison.str>` "method namespace".
 
-For example, to check if each element in column "B" contains the substring "a", we can use the ``.str.contains`` method:
+For example, to check if each element in column "B" contains the substring "a", we can use the :meth:`.str.contains <daft.expressions.expressions.ExpressionStringNamespace.contains>` method:
 
 .. code:: python
 
     df = df.with_column("B2_contains_B", df["B2"].str.contains(df["B"]))
     df.show()
 
 .. code:: none
@@ -167,15 +167,15 @@
 You may find a full list of string operations in the :ref:`Expressions API reference <api-string-expression-operations>`.
 
 URL Expressions
 ^^^^^^^^^^^^^^^
 
 One special case of a String column you may find yourself working with is a column of URL strings.
 
-Daft provides the ``Expression.url.*`` method namespace with functionality for working with URL strings. For example, to download data from URLs:
+Daft provides the :meth:`.url.* <daft.expressions.Expression.url>` method namespace with functionality for working with URL strings. For example, to download data from URLs:
 
 .. code:: python
 
     df = daft.from_pydict({
         "urls": [
             "https://www.google.com",
             "s3://daft-public-data/open-images/validation-images/0001eeaf4aed83f9.jpg",
@@ -205,15 +205,15 @@
 This works well for URLs which are HTTP paths to non-HTML files (e.g. jpeg), local filepaths or even paths to a file in an object store such as AWS S3 as well!
 
 .. _userguide-logical-expressions:
 
 Logical Expressions
 -------------------
 
-Logical Expressions are an expression that refers to a column of type ``Boolean``, and can only take on the values True or False.
+Logical Expressions are an expression that refers to a column of type :meth:`Boolean <daft.DataType.boolean>`, and can only take on the values True or False.
 
 .. code:: python
 
     df = daft.from_pydict({"C": [True, False, True]})
     df["C"]
 
 Daft supports logical operations such as ``&`` (and) and ``|`` (or) between logical expressions.
@@ -248,15 +248,15 @@
     (Showing first 3 of 3 rows)
 
 Other useful comparisons can be found in the :ref:`Expressions API reference <api-comparison-expression>`.
 
 If Else Pattern
 ^^^^^^^^^^^^^^^
 
-The ``.if_else`` method is a useful expression to have up your sleeve for choosing values between two other expressions based on a logical expression:
+The :meth:`.if_else() <daft.expressions.Expression.if_else>` method is a useful expression to have up your sleeve for choosing values between two other expressions based on a logical expression:
 
 .. code:: python
 
     df = daft.from_pydict({"A": [1, 2, 3], "B": [0, 2, 4]})
 
     # Pick values from column A if the value in column A is bigger
     # than the value in column B. Otherwise, pick values from column B.
```

### Comparing `getdaft-0.1.5/docs/source/learn/user_guides/intro-dataframes.rst` & `getdaft-0.1.6/docs/source/learn/user_guides/intro-dataframes.rst`

 * *Files 8% similar despite different names*

```diff
@@ -54,19 +54,19 @@
 
 The reason that our DataFrame currently does not display its rows is that Daft DataFrames are **lazy**. This just means that Daft DataFrames will defer all its work until you tell it to execute.
 
 In this case, Daft is just deferring the work required to read data from the Python dictionary, however in practice this laziness can be very useful for helping Daft optimize your queries before execution!
 
 .. NOTE::
 
-    When you call methods on a Daft Dataframe, it defers the work by adding to an internal "plan". You can examine the current plan of a DataFrame by calling ``DataFrame.explain()``!
+    When you call methods on a Daft Dataframe, it defers the work by adding to an internal "plan". You can examine the current plan of a DataFrame by calling :meth:`df.explain() <daft.DataFrame.explain>`!
 
     Passing the ``show_optimized=True`` argument will show you the plan after Daft applies its query optimizations.
 
-We can tell Daft to execute our DataFrame and cache the results using ``df.collect()``:
+We can tell Daft to execute our DataFrame and cache the results using :meth:`df.collect() <daft.DataFrame.collect>`:
 
 .. code:: python
 
     df.collect()
     df
 
 .. code:: none
@@ -88,39 +88,39 @@
 Now your DataFrame object ``df`` is **materialized** - Daft has executed all the steps required to compute the results, and has cached the results in memory so that it can display this preview.
 
 Any subsequent operations on ``df`` will avoid recomputations, and just use this materialized result!
 
 When should I materialize my DataFrame?
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-If you "eagerly" call ``.collect()`` immediately on every DataFrame, you may run into issues:
+If you "eagerly" call :meth:`df.collect() <daft.DataFrame.collect>` immediately on every DataFrame, you may run into issues:
 
 1. If data is too large at any step, materializing all of it may cause memory issues
 2. Optimizations are not possible since we cannot "predict future operations"
 
 However, data science is all about experimentation and trying different things on the same data. This means that materialization crucial when working interactively with DataFrames, since it speeds up all subsequent experimentation on that DataFrame.
 
-We suggest materializing DataFrames using ``.collect()`` when they contain expensive operations (e.g. sorts or expensive function calls) and have to be called multiple times by downstream code:
+We suggest materializing DataFrames using :meth:`df.collect() <daft.DataFrame.collect>` when they contain expensive operations (e.g. sorts or expensive function calls) and have to be called multiple times by downstream code:
 
 .. code:: python
 
     df = df.with_column("A", df["A"].apply(expensive_function))  # expensive function
     df = df.sort("A")  # expensive sort
     df.collect()  # materialize the DataFrame
 
     # All subsequent work on df avoids recomputing previous steps
     df.sum().show()
     df.mean().show()
     df.with_column("try_this", df["A"] + 1).show(5)
 
-In many other cases however, there are better options than materializing your entire DataFrame with ``.collect()``:
+In many other cases however, there are better options than materializing your entire DataFrame with :meth:`df.collect() <daft.DataFrame.collect>`:
 
-1. **Peeking with df.show(N)**: If you only want to "peek" at the first few rows of your data for visualization purposes, you can use ``df.show(N)``, which processes and shows only the first ``N`` rows.
+1. **Peeking with df.show(N)**: If you only want to "peek" at the first few rows of your data for visualization purposes, you can use :meth:`df.show(N) <daft.DataFrame.show>`, which processes and shows only the first ``N`` rows.
 2. **Writing to disk**: The ``df.write_*`` methods will process and write your data to disk per-partition, avoiding materializing it all in memory at once.
-3. **Pruning data**: You can materialize your DataFrame after performing a ``.limit``, ``.where`` or ``.select`` operation which processes your data or prune it down to a smaller size.
+3. **Pruning data**: You can materialize your DataFrame after performing a :meth:`df.limit() <daft.DataFrame.limit>`, :meth:`df.where() <daft.DataFrame.where>` or :meth:`df.select() <daft.DataFrame.select>` operation which processes your data or prune it down to a smaller size.
 
 Schemas and Types
 -----------------
 
 Notice also that when we printed our DataFrame, Daft displayed its **schema**. Each column of your DataFrame has a **name** and a **type**, and that all data in that column will adhere to that type!
 
 Daft can display your DataFrame's schema without materializing it. Under the hood, it performs intelligent sampling of your data to determine the appropriate schema, and if you make any modifications to your DataFrame it can infer the resulting types based on the operation.
@@ -131,15 +131,15 @@
 
 
 Running Computations
 --------------------
 
 To run computations on data in our DataFrame, we use Expressions.
 
-The following statement will ``.show()`` a DataFrame that has only one column - the column ``A`` from our original DataFrame but with every row incremented by 1.
+The following statement will :meth:`df.show() <daft.DataFrame.show>` a DataFrame that has only one column - the column ``A`` from our original DataFrame but with every row incremented by 1.
 
 .. code:: python
 
     df.select(df["A"] + 1).show()
 
 .. code:: none
 
@@ -172,17 +172,17 @@
 Expressions
 ^^^^^^^^^^^
 
 Expressions are how you define computations on your columns in Daft.
 
 The world of Daft contains much more than just numbers, and you can do much more than just add numbers together. Daft's rich Expressions API allows you to do things such as:
 
-1. Convert between different types with ``df["numbers"].cast(float)``
-2. Download Bytes from a column containing String URLs using ``df["urls"].url.download()``
-3. Run arbitrary Python functions on your data using ``df["objects"].apply(my_python_function)``
+1. Convert between different types with :meth:`df["numbers"].cast(float) <daft.DataFrame.cast>`
+2. Download Bytes from a column containing String URLs using :meth:`df["urls"].url.download() <daft.expressions.expressions.ExpressionUrlNamespace.download>`
+3. Run arbitrary Python functions on your data using :meth:`df["objects"].apply(my_python_function) <daft.DataFrame.apply>`
 
 We are also constantly looking to improve Daft and add more Expression functionality. Please contribute to the project with your ideas and code if you have an Expression in mind!
 
 The next section on :doc:`expressions` will provide a much deeper look at the Expressions that Daft provides.
 
 What now?
 ---------
```

### Comparing `getdaft-0.1.5/docs/source/learn/user_guides/read-write.rst` & `getdaft-0.1.6/docs/source/learn/user_guides/read-write.rst`

 * *Files 6% similar despite different names*

```diff
@@ -33,27 +33,27 @@
     df = daft.read_csv("s3://mybucket/path/to/*.csv")
 
 To learn more about each of these constructors, as well as the options that they support, consult the API documentation on :ref:`creating DataFrames from files <df-io-files>`.
 
 From File Paths
 ^^^^^^^^^^^^^^^
 
-However, if instead you are reading a set of files that are not container file formats, you can use the ``daft.from_glob_path`` method which will read a DataFrame of globbed filepaths.
+However, if instead you are reading a set of files that are not container file formats, you can use the :func:`daft.from_glob_path` method which will read a DataFrame of globbed filepaths.
 
 .. code:: python
 
     df = daft.from_glob_path("s3://mybucket/path/to/images/*.jpeg")
 
     # +----------+------+-----+
     # | name     | size | ... |
     # +----------+------+-----+
     #   ...
 
 
-This is especially useful for reading things such as a folder of images or documents into Daft. A common pattern is to then download data from these files into your DataFrame as bytes, using the ``Expression.url.download()`` method.
+This is especially useful for reading things such as a folder of images or documents into Daft. A common pattern is to then download data from these files into your DataFrame as bytes, using the :meth:`.url.download() <daft.expressions.expressions.ExpressionUrlNamespace.download>` method.
 
 
 From Memory
 ^^^^^^^^^^^
 
 For testing, or small datasets that fit in memory, you may also create DataFrames using Python lists and dictionaries.
```

### Comparing `getdaft-0.1.5/docs/source/learn/user_guides/scaling-up.rst` & `getdaft-0.1.6/docs/source/learn/user_guides/scaling-up.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/learn/user_guides/udf.rst` & `getdaft-0.1.6/docs/source/learn/user_guides/udf.rst`

 * *Files 4% similar despite different names*

```diff
@@ -23,18 +23,18 @@
     +----------+---------------+
     | image    | crop          |
     | Python   | List[Int64]   |
     +==========+===============+
     +----------+---------------+
     (No data to display: Dataframe not materialized)
 
-Per-column per-row functions using ``Expression.apply``
--------------------------------------------------------
+Per-column per-row functions using :meth:`.apply <daft.expressions.Expression.apply>`
+-------------------------------------------------------------------------------------
 
-You can use ``Expression.apply`` to run a Python function on every row in a column.
+You can use :meth:`.apply <daft.expressions.Expression.apply>` to run a Python function on every row in a column.
 
 For example, the following example creates a new ``"flattened_image"`` column by calling ``.flatten()`` on every object in the ``"image"`` column.
 
 .. code:: python
 
     df.with_column(
         "flattened_image",
@@ -58,15 +58,15 @@
     (Showing first 2 rows)
 
 Note here that we use the ``return_dtype`` keyword argument to specify that our returned column type is a Python column!
 
 Multi-column per-partition functions using ``@udf``
 ---------------------------------------------------
 
-``Expression.apply`` is great for convenience, but has two main limitations:
+:meth:`.apply <daft.expressions.Expression.apply>` is great for convenience, but has two main limitations:
 
 1. It can only run on single columns
 2. It can only run on single items at a time
 
 Daft provides the ``@udf`` decorator for defining your own UDFs that process multiple columns or multiple rows at a time.
 
 For example, let's try writing a function that will crop all our images in the ``"image"`` column by its corresponding value in the ``"crop"`` column:
@@ -108,46 +108,45 @@
 
 1. ``crop_images`` is a normal Python function. It takes as input:
     a. A list of images: ``images``
     b. A list of cropping boxes: ``crops``
     c. An integer indicating how much padding to apply to the right and bottom of the cropping: ``padding``
 2. To allow Daft to pass column data into the ``images`` and ``crops`` arguments, we decorate the function with ``@udf``
     a. ``return_dtype`` defines the returned data type. In this case, we return a column containing Python objects of numpy arrays
-    b. At runtime, because we call the UDF on the ``"image"`` and ``"crop"`` columns, the UDF will receive a ``daft.series.Series`` object for each argument.
-3. We can create a new column in our DataFrame by applying our UDF on the ``"image"`` and ``"crop"`` columns inside of a ``df.with_column`` call.
+    b. At runtime, because we call the UDF on the ``"image"`` and ``"crop"`` columns, the UDF will receive a :class:`daft.series.Series` object for each argument.
+3. We can create a new column in our DataFrame by applying our UDF on the ``"image"`` and ``"crop"`` columns inside of a :meth:`df.with_column() <daft.DataFrame.with_column>` call.
 
 UDF Inputs
 ^^^^^^^^^^
 
-When you specify an Expression as an input to a UDF, Daft will calculate the result of that Expression and pass it into your function as a ``daft.series.Series`` object.
+When you specify an Expression as an input to a UDF, Daft will calculate the result of that Expression and pass it into your function as a :class:`daft.Series` object.
 
-The Daft ``Series`` is just an abstraction on a "column" of data! You can obtain several different data representations from a ``Series``:
+The Daft :class:`~daft.series.Series` is just an abstraction on a "column" of data! You can obtain several different data representations from a :class:`~daft.Series`:
 
-1. Numpy Arrays (``np.ndarray``): ``Series.to_numpy()``
-2. Pandas Series (``pd.Series``): ``Series.to_pandas()``
-3. PyArrow Arrays (``pa.Array``): ``Series.to_arrow()``
-4. Python lists (``list``): ``Series.to_pylist()``
+1. PyArrow Arrays (``pa.Array``): :meth:`s.to_arrow() <daft.Series.to_arrow>`
+2. Python lists (``list``): :meth:`s.to_pylist() <daft.Series.to_pylist>`
 
 Depending on your application, you may choose a different data representation that is more performant or more convenient!
 
 .. NOTE::
     Certain array formats have some restrictions around the type of data that they can handle:
 
     1. **Null Handling**: In Pandas and Numpy, nulls are represented as NaNs for numeric types, and Nones for non-numeric types.
     Additionally, the existence of nulls will trigger a type casting from integer to float arrays. If null handling is important to
     your use-case, we recommend using one of the other available options.
+
     2. **Python Objects**: PyArrow array formats cannot support Python columns.
 
     We recommend using Python lists if performance is not a major consideration, and using the arrow-native formats such as
     PyArrow arrays and numpy arrays if performance is important.
 
 Return Types
 ^^^^^^^^^^^^
 
-The ``return_dtype`` argument specifies what type of column your UDF will return. Types can be specified using the ``daft.DataType`` class.
+The ``return_dtype`` argument specifies what type of column your UDF will return. Types can be specified using the :class:`daft.DataType` class.
 
 Your UDF function itself needs to return a batch of columnar data, and can do so as any one of the following array types:
 
 1. Numpy Arrays (``np.ndarray``)
 2. PyArrow Arrays (``pa.Array``)
 3. Python lists (``list``)
 
@@ -179,15 +178,15 @@
 
 
 Resource Requests
 -----------------
 
 Sometimes, you may want to request for specific resources for your UDF. For example, some UDFs need one GPU to run as they will load a model onto the GPU.
 
-Custom resources can be requested when you call ``.with_column``:
+Custom resources can be requested when you call :meth:`df.with_column() <daft.DataFrame.with_column>`:
 
 .. code:: python
 
     from daft.resource_request import ResourceRequest
 
     # Runs the UDF `func` with the specified resource requests
     df = df.with_column(
```

### Comparing `getdaft-0.1.5/docs/source/learn/user_guides.rst` & `getdaft-0.1.6/docs/source/learn/user_guides.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/release_notes/0.0.13.rst` & `getdaft-0.1.6/docs/source/release_notes/0.0.13.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/release_notes/0.0.14.rst` & `getdaft-0.1.6/docs/source/release_notes/0.0.14.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/release_notes/0.0.16.rst` & `getdaft-0.1.6/docs/source/release_notes/0.0.16.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/release_notes/0.0.17.rst` & `getdaft-0.1.6/docs/source/release_notes/0.0.17.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/release_notes/0.0.18.rst` & `getdaft-0.1.6/docs/source/release_notes/0.0.18.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Daft 0.0.18 Release Notes
 =========================
 
 
 The Daft 0.0.18 adds bugfixes and new functionality - highlights:
 
-* `Ray Datasets <https://docs.ray.io/en/latest/data/dataset.html>`_ integration - Daft Dataframes can now feed into ML training on Ray easily using the ``.to_ray_dataset()`` method
+* `Ray Datasets <https://docs.ray.io/en/latest/data/data.html>`_ integration - Daft Dataframes can now feed into ML training on Ray easily using the ``.to_ray_dataset()`` method
 * Big performance improvements from fixes in join algorithm
 * ``.apply`` now infers the return type from the function's type annotation if available
 
 
 New Features
 ------------
 
 Ray Datasets Integration
 ^^^^^^^^^^^^^^^^^^^^^^^^
 
-Daft Dataframes can now be converted easily into a `Ray Datasets <https://docs.ray.io/en/latest/data/dataset.html>`_, which makes it really easy to go from preprocessing/analyzing your data in Daft to ML training using the Ray ecosystem of tools, all on the same Ray cluster.
+Daft Dataframes can now be converted easily into a `Ray Datasets <https://docs.ray.io/en/latest/data/data.html>`_, which makes it really easy to go from preprocessing/analyzing your data in Daft to ML training using the Ray ecosystem of tools, all on the same Ray cluster.
 
 See: `#316 <https://github.com/Eventual-Inc/Daft/pull/316>`_
 
 String Concatenation
 ^^^^^^^^^^^^^^^^^^^^
 
 ``Expression.str.concat`` now allows for concatenation of strings in a Daft Dataframe.
```

### Comparing `getdaft-0.1.5/docs/source/release_notes/0.0.19.rst` & `getdaft-0.1.6/docs/source/release_notes/0.0.19.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/release_notes/0.0.20.rst` & `getdaft-0.1.6/docs/source/release_notes/0.0.20.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/release_notes/0.0.21.rst` & `getdaft-0.1.6/docs/source/release_notes/0.0.21.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/release_notes/0.0.22.rst` & `getdaft-0.1.6/docs/source/release_notes/0.0.22.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/release_notes/0.0.23.rst` & `getdaft-0.1.6/docs/source/release_notes/0.0.23.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/release_notes/0.0.24.rst` & `getdaft-0.1.6/docs/source/release_notes/0.0.24.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/release_notes/0.1.0.rst` & `getdaft-0.1.6/docs/source/release_notes/0.1.0.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/release_notes/0.1.1.rst` & `getdaft-0.1.6/docs/source/release_notes/0.1.1.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/release_notes/0.1.2.rst` & `getdaft-0.1.6/docs/source/release_notes/0.1.2.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/release_notes/0.1.3.rst` & `getdaft-0.1.6/docs/source/release_notes/0.1.3.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/release_notes/0.1.4.rst` & `getdaft-0.1.6/docs/source/release_notes/0.1.4.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/release_notes/_template.rst` & `getdaft-0.1.6/docs/source/release_notes/_template.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/docs/source/technical_architecture.rst` & `getdaft-0.1.6/docs/source/technical_architecture.rst`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 2. **Distributed Computing**: each partition can reside in a different machine, unlocking DataFrames that can span terabytes of data
 3. **Pipelining:** different operations may require different resources (some operations can be I/O-bound, while others may be compute-bound). By chunking up the data into Partitions, Daft can effectively pipeline these operations during scheduling to maximize resource utilization.
 4. **Memory pressure:** by processing one partition at a time, Daft can limit the amount of memory it needs to execute and possibly spill result partitions to disk if necessary, freeing up memory that it needs for execution.
 5. **Optimizations:** by understanding the PartitionSpec (invariants around the data inside each partition), Daft can make intelligent decisions to avoid unnecessary data movement for certain operations that may otherwise require a global shuffle of data.
 
 Partitioning is most often inherited from the data source that Daft is reading from. For example, if read from a directory of files, each file naturally is read as a single partition. If reading from a data catalog service such as Apache Iceberg or Delta Lake, Daft will inherit the partitioning scheme as informed by these services.
 
-When querying a DataFrame, global operations will also require a repartitioning of the data, depending on the operation. For instance, sorting a DataFrame on ``col(x)`` will require repartitioning by range on ``col(x)``, so that a local sort on each partition will provide a globally sorted DataFrame.
+When querying a DataFrame, global operations will also require a repartitioning of the data, depending on the operation. For instance, sorting a DataFrame on :func:`col(x) <daft.expressions.col>` will require repartitioning by range on :func:`col(x) <daft.expressions.col>`, so that a local sort on each partition will provide a globally sorted DataFrame.
 
 In-Memory Data Representation
 -----------------------------
 
 .. image:: /_static/in_memory_data_representation.png
    :alt: Diagram for the hierarchy of datastructures that make up Daft's in-memory representation: DataFrame, Table and Series
    :width: 800
```

### Comparing `getdaft-0.1.5/docs/source/telemetry.rst` & `getdaft-0.1.6/docs/source/telemetry.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/pyproject.toml` & `getdaft-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 [project]
 authors = [{name = "Eventual Inc", email = "daft@eventualcomputing.com"}]
 dependencies = [
   "pyarrow >= 6.0.1",
   "fsspec[http]",
   "loguru",
-  "tabulate >= 0.9.0",
   "psutil",
   "typing-extensions >= 4.0.0; python_version < '3.8'",
   "pickle5 >= 0.0.12; python_version < '3.8'"
 ]
 description = "A Distributed DataFrame library for large scale complex data processing."
 dynamic = ["version"]
 license = {file = "LICENSE"}
```

### Comparing `getdaft-0.1.5/requirements-dev.txt` & `getdaft-0.1.6/requirements-dev.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 # Development/Build utilities (allow to be unpinned)
 ipdb
 maturin
 pre-commit
 
 # Tracing
-orjson==3.9.0  # orjson recommended for viztracer
+orjson==3.9.1  # orjson recommended for viztracer
 py-spy==0.3.14
 viztracer==0.15.6
 
 # Testing frameworks
-hypothesis==6.76.0
-pytest==7.3.1
+hypothesis==6.78.2
+pytest==7.3.2
 pytest-benchmark==4.0.0
 pytest-cov==4.1.0
 
 # Testing dependencies
 lxml==4.9.2
 dask==2022.2.0; python_version < '3.8'
 dask==2023.5.0; python_version == '3.8'
-dask==2023.5.1; python_version >= '3.9'
+dask==2023.6.0; python_version >= '3.9'
 numpy; python_version < '3.8'
 numpy==1.24.3; python_version >= '3.8'
 pandas==1.3.5; python_version < '3.8'
 pandas==2.0.2; python_version >= '3.8'
 xxhash>=3.0.0
 Pillow==9.5.0
 opencv-python==4.7.0.72
 
 # Ray
 ray[data, default]==2.4.0
 
 # AWS
 s3fs==2023.1.0; python_version < '3.8'
-s3fs==2023.5.0; python_version >= '3.8'
+s3fs==2023.6.0; python_version >= '3.8'
 
 # Documentation
 myst-nb>=0.16.0
 Sphinx <= 5
 sphinx-book-theme>=0.3.3,<1.0.0
 sphinx-reredirects>=0.1.1
+sphinx-copybutton>=0.5.2
```

### Comparing `getdaft-0.1.5/src/array/from.rs` & `getdaft-0.1.6/src/array/from.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/iterator.rs` & `getdaft-0.1.6/src/array/iterator.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/mod.rs` & `getdaft-0.1.6/src/array/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/ops/apply.rs` & `getdaft-0.1.6/src/array/ops/apply.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/ops/arange.rs` & `getdaft-0.1.6/src/array/ops/arange.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/ops/arithmetic.rs` & `getdaft-0.1.6/src/array/ops/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/ops/arrow2/comparison.rs` & `getdaft-0.1.6/src/array/ops/arrow2/comparison.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/ops/arrow2/sort/primitive/common.rs` & `getdaft-0.1.6/src/array/ops/arrow2/sort/primitive/common.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/ops/arrow2/sort/primitive/indices.rs` & `getdaft-0.1.6/src/array/ops/arrow2/sort/primitive/indices.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/ops/arrow2/sort/primitive/sort.rs` & `getdaft-0.1.6/src/array/ops/arrow2/sort/primitive/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/ops/broadcast.rs` & `getdaft-0.1.6/src/array/ops/broadcast.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/ops/cast.rs` & `getdaft-0.1.6/src/array/ops/cast.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 use arrow2::compute::{
     self,
     cast::{can_cast_types, cast, CastOptions},
 };
 
-use crate::series::IntoSeries;
 use crate::{
     array::DataArray,
     datatypes::logical::{
-        DateArray, EmbeddingArray, FixedShapeImageArray, ImageArray, LogicalArray,
+        DateArray, EmbeddingArray, FixedShapeImageArray, ImageArray, LogicalArray, TimestampArray,
     },
     datatypes::{DaftArrowBackedType, DataType, Field, Utf8Array},
     error::{DaftError, DaftResult},
     series::Series,
     with_match_arrow_daft_types, with_match_daft_logical_types,
 };
+use crate::{datatypes::TimeUnit, series::IntoSeries};
 
 #[cfg(feature = "python")]
 use crate::array::{ops::image::ImageArrayVecs, pseudo_arrow::PseudoArrowArray};
 #[cfg(feature = "python")]
 use crate::datatypes::{FixedSizeListArray, ImageMode, ListArray, PythonArray};
 #[cfg(feature = "python")]
 use crate::ffi;
@@ -51,31 +51,54 @@
             "Can not cast {:?} to type: {:?}: not convertible to Arrow",
             to_cast.data_type(),
             dtype
         )));
     }
     let physical_type = dtype.to_physical();
     let self_arrow_type = to_cast.data_type().to_arrow()?;
-    let target_arrow_type = physical_type.to_arrow()?;
+    let target_arrow_type = dtype.to_arrow()?;
     if !can_cast_types(&self_arrow_type, &target_arrow_type) {
         return Err(DaftError::TypeError(format!(
             "can not cast {:?} to type: {:?}: Arrow types not castable",
             to_cast.data_type(),
             dtype
         )));
     }
 
-    let result_array = cast(
-        to_cast.data(),
-        &target_arrow_type,
-        CastOptions {
-            wrapped: true,
-            partial: false,
-        },
-    )?;
+    let result_array = {
+        let target_arrow_physical = physical_type.to_arrow()?;
+        if target_arrow_physical == target_arrow_type {
+            cast(
+                to_cast.data(),
+                &target_arrow_type,
+                CastOptions {
+                    wrapped: true,
+                    partial: false,
+                },
+            )?
+        } else {
+            let arrow_logical = cast(
+                to_cast.data(),
+                &target_arrow_type,
+                CastOptions {
+                    wrapped: true,
+                    partial: false,
+                },
+            )?;
+            cast(
+                arrow_logical.as_ref(),
+                &target_arrow_physical,
+                CastOptions {
+                    wrapped: true,
+                    partial: false,
+                },
+            )?
+        }
+    };
+
     let new_field = Arc::new(Field::new(to_cast.name(), dtype.clone()));
 
     if dtype.is_logical() {
         with_match_daft_logical_types!(dtype, |$T| {
             let physical = DataArray::try_from((Field::new(to_cast.name(), physical_type), result_array))?;
             return Ok(LogicalArray::<$T>::new(new_field.clone(), physical).into_series());
         })
@@ -150,14 +173,96 @@
             DataType::Float32 => self.cast(&DataType::Int32)?.cast(&DataType::Float32),
             DataType::Float64 => self.cast(&DataType::Int32)?.cast(&DataType::Float64),
             _ => arrow_cast(&self.physical, dtype),
         }
     }
 }
 
+pub(super) fn timestamp_to_str_naive(val: i64, unit: &TimeUnit) -> String {
+    let chrono_ts = {
+        arrow2::temporal_conversions::timestamp_to_naive_datetime(val, unit.to_arrow().unwrap())
+    };
+    let format_str = match unit {
+        TimeUnit::Seconds => "%Y-%m-%dT%H:%M:%S",
+        TimeUnit::Milliseconds => "%Y-%m-%dT%H:%M:%S%.3f",
+        TimeUnit::Microseconds => "%Y-%m-%dT%H:%M:%S%.6f",
+        TimeUnit::Nanoseconds => "%Y-%m-%dT%H:%M:%S%.9f",
+    };
+    chrono_ts.format(format_str).to_string()
+}
+
+pub(super) fn timestamp_to_str_offset(
+    val: i64,
+    unit: &TimeUnit,
+    offset: &chrono::FixedOffset,
+) -> String {
+    let seconds_format = match unit {
+        TimeUnit::Seconds => chrono::SecondsFormat::Secs,
+        TimeUnit::Milliseconds => chrono::SecondsFormat::Millis,
+        TimeUnit::Microseconds => chrono::SecondsFormat::Micros,
+        TimeUnit::Nanoseconds => chrono::SecondsFormat::Nanos,
+    };
+    arrow2::temporal_conversions::timestamp_to_datetime(val, unit.to_arrow().unwrap(), offset)
+        .to_rfc3339_opts(seconds_format, false)
+}
+
+pub(super) fn timestamp_to_str_tz(val: i64, unit: &TimeUnit, tz: &chrono_tz::Tz) -> String {
+    let seconds_format = match unit {
+        TimeUnit::Seconds => chrono::SecondsFormat::Secs,
+        TimeUnit::Milliseconds => chrono::SecondsFormat::Millis,
+        TimeUnit::Microseconds => chrono::SecondsFormat::Micros,
+        TimeUnit::Nanoseconds => chrono::SecondsFormat::Nanos,
+    };
+    arrow2::temporal_conversions::timestamp_to_datetime(val, unit.to_arrow().unwrap(), tz)
+        .to_rfc3339_opts(seconds_format, false)
+}
+
+impl TimestampArray {
+    pub fn cast(&self, dtype: &DataType) -> DaftResult<Series> {
+        match dtype {
+            DataType::Utf8 => {
+                let DataType::Timestamp(unit, timezone) = &self.field.dtype else { panic!("Wrong dtype for TimestampArray: {}", self.field.dtype) };
+
+                let str_array: arrow2::array::Utf8Array<i64> = timezone.as_ref().map_or_else(
+                    || {
+                        self.as_arrow()
+                            .iter()
+                            .map(|val| val.map(|val| timestamp_to_str_naive(*val, unit)))
+                            .collect()
+                    },
+                    |timezone| {
+                        if let Ok(offset) = arrow2::temporal_conversions::parse_offset(timezone) {
+                            self.as_arrow()
+                                .iter()
+                                .map(|val| {
+                                    val.map(|val| timestamp_to_str_offset(*val, unit, &offset))
+                                })
+                                .collect()
+                        } else if let Ok(tz) =
+                            arrow2::temporal_conversions::parse_offset_tz(timezone)
+                        {
+                            self.as_arrow()
+                                .iter()
+                                .map(|val| val.map(|val| timestamp_to_str_tz(*val, unit, &tz)))
+                                .collect()
+                        } else {
+                            panic!("Unable to parse timezone string {}", timezone)
+                        }
+                    },
+                );
+
+                Ok(Utf8Array::from((self.name(), Box::new(str_array))).into_series())
+            }
+            DataType::Float32 => self.cast(&DataType::Int64)?.cast(&DataType::Float32),
+            DataType::Float64 => self.cast(&DataType::Int64)?.cast(&DataType::Float64),
+            _ => arrow_cast(&self.physical, dtype),
+        }
+    }
+}
+
 #[cfg(feature = "python")]
 macro_rules! pycast_then_arrowcast {
     ($self:expr, $daft_type:expr, $pytype_str:expr) => {
         {
             let old_pyseries = PySeries::from($self.clone().into_series());
 
             let new_pyseries = Python::with_gil(|py| -> PyResult<PySeries> {
@@ -627,15 +732,14 @@
             | dt @ DataType::Int16
             | dt @ DataType::Int32
             | dt @ DataType::Int64 => pycast_then_arrowcast!(self, dt, "int"),
             // DataType::Float16 => todo!(),
             dt @ DataType::Float32 | dt @ DataType::Float64 => {
                 pycast_then_arrowcast!(self, dt, "float")
             }
-            DataType::Date => unimplemented!(),
             DataType::List(field) => {
                 if !field.dtype.is_numeric() {
                     return Err(DaftError::ValueError(format!(
                         "We can only convert numeric python types to List, got {}",
                         field.dtype
                     )));
                 }
```

### Comparing `getdaft-0.1.5/src/array/ops/compare_agg.rs` & `getdaft-0.1.6/src/array/ops/compare_agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/ops/comparison.rs` & `getdaft-0.1.6/src/array/ops/comparison.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/ops/concat.rs` & `getdaft-0.1.6/src/array/ops/concat.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/ops/concat_agg.rs` & `getdaft-0.1.6/src/array/ops/concat_agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/ops/count.rs` & `getdaft-0.1.6/src/array/ops/count.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/ops/date.rs` & `getdaft-0.1.6/src/array/ops/date.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/ops/filter.rs` & `getdaft-0.1.6/src/array/ops/filter.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use crate::{
     array::DataArray,
     datatypes::{
-        logical::{DateArray, EmbeddingArray, FixedShapeImageArray, ImageArray},
+        logical::{DateArray, EmbeddingArray, FixedShapeImageArray, ImageArray, TimestampArray},
         BooleanArray, DaftArrowBackedType,
     },
     error::DaftResult,
 };
 
 use super::as_arrow::AsArrow;
 
@@ -76,14 +76,21 @@
 impl DateArray {
     pub fn filter(&self, mask: &BooleanArray) -> DaftResult<Self> {
         let new_array = self.physical.filter(mask)?;
         Ok(Self::new(self.field.clone(), new_array))
     }
 }
 
+impl TimestampArray {
+    pub fn filter(&self, mask: &BooleanArray) -> DaftResult<Self> {
+        let new_array = self.physical.filter(mask)?;
+        Ok(Self::new(self.field.clone(), new_array))
+    }
+}
+
 impl EmbeddingArray {
     pub fn filter(&self, mask: &BooleanArray) -> DaftResult<Self> {
         let new_array = self.physical.filter(mask)?;
         Ok(Self::new(self.field.clone(), new_array))
     }
 }
```

### Comparing `getdaft-0.1.5/src/array/ops/float.rs` & `getdaft-0.1.6/src/array/ops/float.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/ops/full.rs` & `getdaft-0.1.6/src/array/ops/full.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/ops/groups.rs` & `getdaft-0.1.6/src/array/ops/groups.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/ops/hash.rs` & `getdaft-0.1.6/src/array/ops/hash.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/ops/if_else.rs` & `getdaft-0.1.6/src/array/ops/if_else.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 use crate::array::DataArray;
-use crate::datatypes::logical::{DateArray, EmbeddingArray, FixedShapeImageArray, ImageArray};
+use crate::datatypes::logical::{
+    DateArray, EmbeddingArray, FixedShapeImageArray, ImageArray, TimestampArray,
+};
 use crate::datatypes::{
     BinaryArray, BooleanArray, DaftArrowBackedType, DaftNumericType, ExtensionArray, Field,
     FixedSizeListArray, ListArray, NullArray, StructArray, Utf8Array,
 };
 use crate::error::{DaftError, DaftResult};
 use crate::utils::arrow::arrow_bitmap_and_helper;
 use std::convert::identity;
@@ -324,14 +326,21 @@
 impl DateArray {
     pub fn if_else(&self, other: &Self, predicate: &BooleanArray) -> DaftResult<Self> {
         let new_array = self.physical.if_else(&other.physical, predicate)?;
         Ok(Self::new(self.field.clone(), new_array))
     }
 }
 
+impl TimestampArray {
+    pub fn if_else(&self, other: &Self, predicate: &BooleanArray) -> DaftResult<Self> {
+        let new_array = self.physical.if_else(&other.physical, predicate)?;
+        Ok(Self::new(self.field.clone(), new_array))
+    }
+}
+
 impl EmbeddingArray {
     pub fn if_else(&self, other: &Self, predicate: &BooleanArray) -> DaftResult<Self> {
         let new_array = self.physical.if_else(&other.physical, predicate)?;
         Ok(Self::new(self.field.clone(), new_array))
     }
 }
```

### Comparing `getdaft-0.1.5/src/array/ops/image.rs` & `getdaft-0.1.6/src/array/ops/image.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 use std::borrow::Cow;
+use std::io::Write;
 use std::vec;
 
 use image::{ColorType, DynamicImage, ImageBuffer};
 
-use crate::datatypes::{logical::ImageArray, BinaryArray, DataType, Field, ImageMode, StructArray};
+use crate::datatypes::{
+    logical::ImageArray, BinaryArray, DataType, Field, ImageFormat, ImageMode, StructArray,
+};
 use crate::error::{DaftError, DaftResult};
 use image::{Luma, LumaA, Rgb, Rgba};
 
 use super::as_arrow::AsArrow;
 use num_traits::FromPrimitive;
 
 use std::ops::Deref;
@@ -90,14 +93,51 @@
 
     pub fn decode(bytes: &[u8]) -> DaftResult<Self> {
         image::load_from_memory(bytes)
             .map(|v| v.into())
             .map_err(|e| DaftError::ValueError(format!("Decoding image from bytes failed: {}", e)))
     }
 
+    pub fn encode(&self, image_format: ImageFormat, out: &mut Vec<u8>) -> DaftResult<()> {
+        let mut writer = std::io::BufWriter::new(std::io::Cursor::new(out));
+        image::write_buffer_with_format(
+            &mut writer,
+            self.as_u8_slice(),
+            self.width(),
+            self.height(),
+            self.color(),
+            image::ImageFormat::from(image_format),
+        )
+        .map_err(|e| {
+            DaftError::ValueError(format!(
+                "Encoding image into file format {} failed: {}",
+                image_format, e
+            ))
+        })?;
+        writer.flush().map_err(|e| {
+            DaftError::ValueError(format!(
+                "Encoding image into file format {} failed: {}",
+                image_format, e
+            ))
+        })
+    }
+
+    pub fn fit_to(&self, w: u32, h: u32) -> Self {
+        // Preserving aspect ratio, resize an image to fit within the specified dimensions.
+        let scale_factor = {
+            let width_scale = w as f64 / self.width() as f64;
+            let height_scale = h as f64 / self.height() as f64;
+            width_scale.min(height_scale)
+        };
+        let new_w = self.width() as f64 * scale_factor;
+        let new_h = self.height() as f64 * scale_factor;
+
+        self.resize(new_w.floor() as u32, new_h.floor() as u32)
+    }
+
     pub fn resize(&self, w: u32, h: u32) -> Self {
         use DaftImageBuffer::*;
         match self {
             L(imgbuf) => {
                 let result =
                     image::imageops::resize(imgbuf, w, h, image::imageops::FilterType::Triangle);
                 DaftImageBuffer::L(image_buffer_vec_to_cow(result))
@@ -344,14 +384,33 @@
         };
 
         assert_eq!(result.height(), h);
         assert_eq!(result.width(), w);
         Some(result)
     }
 
+    pub fn encode(&self, image_format: ImageFormat) -> DaftResult<BinaryArray> {
+        let result = (0..self.len())
+            .map(|i| self.as_image_obj(i))
+            .map(|img| {
+                img.map(|img| {
+                    let mut buf = Vec::new();
+                    img.encode(image_format, &mut buf)?;
+                    Ok(buf)
+                })
+                .transpose()
+            })
+            .collect::<DaftResult<Vec<_>>>()?;
+        let arrow_array = arrow2::array::BinaryArray::<i64>::from_iter(result.into_iter());
+        BinaryArray::new(
+            Field::new(self.name(), arrow_array.data_type().into()).into(),
+            arrow_array.boxed(),
+        )
+    }
+
     pub fn resize(&self, w: u32, h: u32) -> DaftResult<Self> {
         let result = (0..self.len())
             .map(|i| self.as_image_obj(i))
             .map(|img| img.map(|img| img.resize(w, h)))
             .collect::<Vec<_>>();
         Self::from_daft_image_buffers(self.name(), result.as_slice(), self.image_mode())
     }
```

### Comparing `getdaft-0.1.5/src/array/ops/len.rs` & `getdaft-0.1.6/src/array/ops/len.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/ops/list_agg.rs` & `getdaft-0.1.6/src/array/ops/list_agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/ops/mean.rs` & `getdaft-0.1.6/src/array/ops/mean.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/ops/mod.rs` & `getdaft-0.1.6/src/array/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/ops/null.rs` & `getdaft-0.1.6/src/array/ops/null.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/ops/pairwise.rs` & `getdaft-0.1.6/src/array/ops/pairwise.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/ops/sort.rs` & `getdaft-0.1.6/src/array/ops/sort.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use crate::{
     array::DataArray,
     datatypes::{
-        logical::{DateArray, EmbeddingArray, FixedShapeImageArray, ImageArray},
+        logical::{DateArray, EmbeddingArray, FixedShapeImageArray, ImageArray, TimestampArray},
         BinaryArray, BooleanArray, DaftIntegerType, DaftNumericType, ExtensionArray,
         FixedSizeListArray, Float32Array, Float64Array, ListArray, NullArray, StructArray,
         Utf8Array,
     },
     error::DaftResult,
     kernels::search_sorted::{build_compare_with_nulls, cmp_float},
     series::Series,
@@ -594,14 +594,21 @@
 impl DateArray {
     pub fn sort(&self, descending: bool) -> DaftResult<Self> {
         let new_array = self.physical.sort(descending)?;
         Ok(Self::new(self.field.clone(), new_array))
     }
 }
 
+impl TimestampArray {
+    pub fn sort(&self, descending: bool) -> DaftResult<Self> {
+        let new_array = self.physical.sort(descending)?;
+        Ok(Self::new(self.field.clone(), new_array))
+    }
+}
+
 impl EmbeddingArray {
     pub fn sort(&self, _descending: bool) -> DaftResult<Self> {
         todo!("impl sort for EmbeddingArray")
     }
 }
 
 impl ImageArray {
```

### Comparing `getdaft-0.1.5/src/array/ops/sum.rs` & `getdaft-0.1.6/src/array/ops/sum.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/ops/take.rs` & `getdaft-0.1.6/src/array/ops/take.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+use base64::Engine;
+
 use crate::{
     array::DataArray,
     datatypes::{
-        logical::{DateArray, EmbeddingArray, FixedShapeImageArray, ImageArray},
+        logical::{DateArray, EmbeddingArray, FixedShapeImageArray, ImageArray, TimestampArray},
         BinaryArray, BooleanArray, DaftIntegerType, DaftNumericType, ExtensionArray,
-        FixedSizeListArray, ListArray, NullArray, StructArray, Utf8Array,
+        FixedSizeListArray, ImageFormat, ListArray, NullArray, StructArray, Utf8Array,
     },
     error::DaftResult,
 };
 
 use super::as_arrow::AsArrow;
 
 impl<T> DataArray<T>
@@ -42,14 +44,21 @@
     pub fn str_value(&self, idx: usize) -> DaftResult<String> {
         let val = self.get(idx);
         match val {
             None => Ok("None".to_string()),
             Some(v) => Ok(format!("{v}")),
         }
     }
+
+    pub fn html_value(&self, idx: usize) -> String {
+        let str_value = self.str_value(idx).unwrap();
+        html_escape::encode_text(&str_value)
+            .into_owned()
+            .replace('\n', "<br />")
+    }
 }
 
 impl Utf8Array {
     #[inline]
     pub fn get(&self, idx: usize) -> Option<&str> {
         if idx >= self.len() {
             panic!("Out of bounds: {} vs len: {}", idx, self.len())
@@ -74,17 +83,24 @@
         Self::try_from((self.field.clone(), result))
     }
 
     pub fn str_value(&self, idx: usize) -> DaftResult<String> {
         let val = self.get(idx);
         match val {
             None => Ok("None".to_string()),
-            Some(v) => Ok(format!("\"{v}\"")),
+            Some(v) => Ok(v.to_string()),
         }
     }
+
+    pub fn html_value(&self, idx: usize) -> String {
+        let str_value = self.str_value(idx).unwrap();
+        html_escape::encode_text(&str_value)
+            .into_owned()
+            .replace('\n', "<br />")
+    }
 }
 
 impl BooleanArray {
     #[inline]
     pub fn get(&self, idx: usize) -> Option<bool> {
         if idx >= self.len() {
             panic!("Out of bounds: {} vs len: {}", idx, self.len())
@@ -112,14 +128,20 @@
     pub fn str_value(&self, idx: usize) -> DaftResult<String> {
         let val = self.get(idx);
         match val {
             None => Ok("None".to_string()),
             Some(v) => Ok(format!("{v}")),
         }
     }
+    pub fn html_value(&self, idx: usize) -> String {
+        let str_value = self.str_value(idx).unwrap();
+        html_escape::encode_text(&str_value)
+            .into_owned()
+            .replace('\n', "<br />")
+    }
 }
 
 impl NullArray {
     #[inline]
     pub fn get(&self, idx: usize) -> Option<()> {
         if idx >= self.len() {
             panic!("Out of bounds: {} vs len: {}", idx, self.len())
@@ -138,14 +160,20 @@
 
     pub fn str_value(&self, idx: usize) -> DaftResult<String> {
         if idx >= self.len() {
             panic!("Out of bounds: {} vs len: {}", idx, self.len())
         }
         Ok("None".to_string())
     }
+    pub fn html_value(&self, idx: usize) -> String {
+        let str_value = self.str_value(idx).unwrap();
+        html_escape::encode_text(&str_value)
+            .into_owned()
+            .replace('\n', "<br />")
+    }
 }
 
 impl BinaryArray {
     #[inline]
     pub fn get(&self, idx: usize) -> Option<&[u8]> {
         if idx >= self.len() {
             panic!("Out of bounds: {} vs len: {}", idx, self.len())
@@ -175,14 +203,20 @@
         match val {
             None => Ok("None".to_string()),
             // TODO: [RUST-INT] proper display of bytes as string here, preferably similar to how Python displays it
             // See discussion: https://stackoverflow.com/questions/54358833/how-does-bytes-repr-representation-work
             Some(v) => Ok(format!("b\"{:?}\"", v)),
         }
     }
+    pub fn html_value(&self, idx: usize) -> String {
+        let str_value = self.str_value(idx).unwrap();
+        html_escape::encode_text(&str_value)
+            .into_owned()
+            .replace('\n', "<br />")
+    }
 }
 
 impl ListArray {
     #[inline]
     pub fn get(&self, idx: usize) -> Option<Box<dyn arrow2::array::Array>> {
         if idx >= self.len() {
             panic!("Out of bounds: {} vs len: {}", idx, self.len())
@@ -210,14 +244,20 @@
     pub fn str_value(&self, idx: usize) -> DaftResult<String> {
         let val = self.get(idx);
         match val {
             None => Ok("None".to_string()),
             Some(v) => Ok(format!("{v:?}")),
         }
     }
+    pub fn html_value(&self, idx: usize) -> String {
+        let str_value = self.str_value(idx).unwrap();
+        html_escape::encode_text(&str_value)
+            .into_owned()
+            .replace('\n', "<br />")
+    }
 }
 
 impl FixedSizeListArray {
     #[inline]
     pub fn get(&self, idx: usize) -> Option<Box<dyn arrow2::array::Array>> {
         if idx >= self.len() {
             panic!("Out of bounds: {} vs len: {}", idx, self.len())
@@ -245,14 +285,20 @@
     pub fn str_value(&self, idx: usize) -> DaftResult<String> {
         let val = self.get(idx);
         match val {
             None => Ok("None".to_string()),
             Some(v) => Ok(format!("{v:?}")),
         }
     }
+    pub fn html_value(&self, idx: usize) -> String {
+        let str_value = self.str_value(idx).unwrap();
+        html_escape::encode_text(&str_value)
+            .into_owned()
+            .replace('\n', "<br />")
+    }
 }
 
 impl StructArray {
     #[inline]
     pub fn get(&self, idx: usize) -> Option<Vec<Box<dyn arrow2::array::Array>>> {
         if idx >= self.len() {
             panic!("Out of bounds: {} vs len: {}", idx, self.len())
@@ -286,14 +332,20 @@
     pub fn str_value(&self, idx: usize) -> DaftResult<String> {
         let val = self.get(idx);
         match val {
             None => Ok("None".to_string()),
             Some(v) => Ok(format!("{v:?}")),
         }
     }
+    pub fn html_value(&self, idx: usize) -> String {
+        let str_value = self.str_value(idx).unwrap();
+        html_escape::encode_text(&str_value)
+            .into_owned()
+            .replace('\n', "<br />")
+    }
 }
 
 impl ExtensionArray {
     #[inline]
     pub fn get(&self, idx: usize) -> Option<Box<dyn arrow2::scalar::Scalar>> {
         if idx >= self.len() {
             panic!("Out of bounds: {} vs len: {}", idx, self.len())
@@ -321,14 +373,20 @@
     pub fn str_value(&self, idx: usize) -> DaftResult<String> {
         let val = self.get(idx);
         match val {
             None => Ok("None".to_string()),
             Some(v) => Ok(format!("{v:?}")),
         }
     }
+    pub fn html_value(&self, idx: usize) -> String {
+        let str_value = self.str_value(idx).unwrap();
+        html_escape::encode_text(&str_value)
+            .into_owned()
+            .replace('\n', "<br />")
+    }
 }
 
 #[cfg(feature = "python")]
 impl crate::datatypes::PythonArray {
     #[inline]
     pub fn get(&self, idx: usize) -> pyo3::PyObject {
         use arrow2::array::Array;
@@ -419,14 +477,20 @@
         let call_result =
             Python::with_gil(|py| val.call_method0(py, pyo3::intern!(py, "__str__")))?;
 
         let extracted = Python::with_gil(|py| call_result.extract(py))?;
 
         Ok(extracted)
     }
+    pub fn html_value(&self, idx: usize) -> String {
+        let str_value = self.str_value(idx).unwrap();
+        html_escape::encode_text(&str_value)
+            .into_owned()
+            .replace('\n', "<br />")
+    }
 }
 
 impl DateArray {
     #[inline]
     pub fn get(&self, idx: usize) -> Option<i32> {
         if idx >= self.len() {
             panic!("Out of bounds: {} vs len: {}", idx, self.len())
@@ -454,14 +518,87 @@
     pub fn str_value(&self, idx: usize) -> DaftResult<String> {
         let val = self.get(idx);
         match val {
             None => Ok("None".to_string()),
             Some(v) => Ok(format!("{v}")),
         }
     }
+    pub fn html_value(&self, idx: usize) -> String {
+        let str_value = self.str_value(idx).unwrap();
+        html_escape::encode_text(&str_value)
+            .into_owned()
+            .replace('\n', "<br />")
+    }
+}
+
+impl TimestampArray {
+    #[inline]
+    pub fn get(&self, idx: usize) -> Option<i64> {
+        if idx >= self.len() {
+            panic!("Out of bounds: {} vs len: {}", idx, self.len())
+        }
+        let arrow_array = self.as_arrow();
+        let is_valid = arrow_array
+            .validity()
+            .map_or(true, |validity| validity.get_bit(idx));
+        if is_valid {
+            Some(unsafe { arrow_array.value_unchecked(idx) })
+        } else {
+            None
+        }
+    }
+
+    pub fn take<I>(&self, idx: &DataArray<I>) -> DaftResult<Self>
+    where
+        I: DaftIntegerType,
+        <I as DaftNumericType>::Native: arrow2::types::Index,
+    {
+        let new_array = self.physical.take(idx)?;
+        Ok(Self::new(self.field.clone(), new_array))
+    }
+
+    pub fn str_value(&self, idx: usize) -> DaftResult<String> {
+        let res = self.get(idx).map_or_else(
+            || "None".to_string(),
+            |val| -> String {
+                use crate::datatypes::DataType::Timestamp;
+                use crate::array::ops::cast::{
+                    timestamp_to_str_naive,
+                    timestamp_to_str_offset,
+                    timestamp_to_str_tz,
+                };
+
+                let Timestamp(unit, timezone) = &self.field.dtype else { panic!("Wrong dtype for TimestampArray: {}", self.field.dtype) };
+
+                timezone.as_ref().map_or_else(
+                    || timestamp_to_str_naive(val, unit),
+                    |timezone| {
+                        // In arrow, timezone string can be either:
+                        // 1. a fixed offset "-07:00", parsed using parse_offset, or
+                        // 2. a timezone name e.g. "America/Los_Angeles", parsed using parse_offset_tz.
+                        if let Ok(offset) = arrow2::temporal_conversions::parse_offset(timezone) {
+                            timestamp_to_str_offset(val, unit, &offset)
+                        } else if let Ok(tz) = arrow2::temporal_conversions::parse_offset_tz(timezone) {
+                            timestamp_to_str_tz(val, unit, &tz)
+                        } else {
+                            panic!("Unable to parse timezone string {}", timezone)
+                        }
+                    },
+                )
+            }
+        );
+        Ok(res)
+    }
+
+    pub fn html_value(&self, idx: usize) -> String {
+        let str_value = self.str_value(idx).unwrap();
+        html_escape::encode_text(&str_value)
+            .into_owned()
+            .replace('\n', "<br />")
+    }
 }
 
 impl EmbeddingArray {
     #[inline]
     pub fn get(&self, idx: usize) -> Option<Box<dyn arrow2::array::Array>> {
         if idx >= self.len() {
             panic!("Out of bounds: {} vs len: {}", idx, self.len())
@@ -489,14 +626,20 @@
     pub fn str_value(&self, idx: usize) -> DaftResult<String> {
         let val = self.get(idx);
         match val {
             None => Ok("None".to_string()),
             Some(v) => Ok(format!("{v:?}")),
         }
     }
+    pub fn html_value(&self, idx: usize) -> String {
+        let str_value = self.str_value(idx).unwrap();
+        html_escape::encode_text(&str_value)
+            .into_owned()
+            .replace('\n', "<br />")
+    }
 }
 
 impl ImageArray {
     #[inline]
     pub fn get(&self, idx: usize) -> Option<Box<dyn arrow2::array::Array>> {
         if idx >= self.len() {
             panic!("Out of bounds: {} vs len: {}", idx, self.len())
@@ -527,14 +670,32 @@
     pub fn str_value(&self, idx: usize) -> DaftResult<String> {
         let val = self.get(idx);
         match val {
             None => Ok("None".to_string()),
             Some(v) => Ok(format!("{v:?}")),
         }
     }
+    pub fn html_value(&self, idx: usize) -> String {
+        let maybe_image = self.as_image_obj(idx);
+        let str_val = self.str_value(idx).unwrap();
+
+        match maybe_image {
+            None => "None".to_string(),
+            Some(image) => {
+                let thumb = image.fit_to(128, 128);
+                let mut bytes: Vec<u8> = vec![];
+                thumb.encode(ImageFormat::JPEG, &mut bytes).unwrap();
+                format!(
+                    "<img style=\"max-height:128px;width:auto\" src=\"data:image/png;base64, {}\" alt=\"{}\" />",
+                    base64::engine::general_purpose::STANDARD.encode(&bytes),
+                    str_val,
+                )
+            }
+        }
+    }
 }
 
 impl FixedShapeImageArray {
     #[inline]
     pub fn get(&self, idx: usize) -> Option<Box<dyn arrow2::array::Array>> {
         if idx >= self.len() {
             panic!("Out of bounds: {} vs len: {}", idx, self.len())
@@ -562,8 +723,14 @@
     pub fn str_value(&self, idx: usize) -> DaftResult<String> {
         let val = self.get(idx);
         match val {
             None => Ok("None".to_string()),
             Some(v) => Ok(format!("{v:?}")),
         }
     }
+    pub fn html_value(&self, idx: usize) -> String {
+        let str_value = self.str_value(idx).unwrap();
+        html_escape::encode_text(&str_value)
+            .into_owned()
+            .replace('\n', "<br />")
+    }
 }
```

### Comparing `getdaft-0.1.5/src/array/ops/utf8.rs` & `getdaft-0.1.6/src/array/ops/utf8.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/pseudo_arrow/compute.rs` & `getdaft-0.1.6/src/array/pseudo_arrow/compute.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/pseudo_arrow/mod.rs` & `getdaft-0.1.6/src/array/pseudo_arrow/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/array/pseudo_arrow/python.rs` & `getdaft-0.1.6/src/array/pseudo_arrow/python.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/datatypes/dtype.rs` & `getdaft-0.1.6/src/datatypes/dtype.rs`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,15 @@
             DataType::Float16 | DataType::Float32 | DataType::Float64
         )
     }
 
     #[inline]
     pub fn is_temporal(&self) -> bool {
         match self {
-            DataType::Date => true,
+            DataType::Date | DataType::Timestamp(..) => true,
             DataType::Extension(_, inner, _) => inner.is_temporal(),
             _ => false,
         }
     }
 
     #[inline]
     pub fn is_null(&self) -> bool {
@@ -280,14 +280,15 @@
     }
 
     #[inline]
     pub fn is_logical(&self) -> bool {
         matches!(
             self,
             DataType::Date
+                | DataType::Timestamp(..)
                 | DataType::Embedding(..)
                 | DataType::Image(..)
                 | DataType::FixedShapeImage(..)
         )
     }
 
     #[inline]
```

### Comparing `getdaft-0.1.5/src/datatypes/field.rs` & `getdaft-0.1.6/src/datatypes/field.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/datatypes/image_mode.rs` & `getdaft-0.1.6/src/datatypes/image_mode.rs`

 * *Files 23% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 use crate::{
     datatypes::DataType,
     error::{DaftError, DaftResult},
 };
 
 /// Supported image modes for Daft's image type.
 ///
-/// L       - 8-bit grayscale
-/// LA      - 8-bit grayscale + alpha
-/// RGB     - 8-bit RGB
-/// RGBA    - 8-bit RGB + alpha
-/// L16     - 16-bit grayscale
-/// LA16    - 16-bit grayscale + alpha
-/// RGB16   - 16-bit RGB
-/// RGBA16  - 16-bit RGB + alpha
-/// RGB32F  - 32-bit floating RGB
-/// RGBA32F - 32-bit floating RGB + alpha
+/// | L       - 8-bit grayscale
+/// | LA      - 8-bit grayscale + alpha
+/// | RGB     - 8-bit RGB
+/// | RGBA    - 8-bit RGB + alpha
+/// | L16     - 16-bit grayscale
+/// | LA16    - 16-bit grayscale + alpha
+/// | RGB16   - 16-bit RGB
+/// | RGBA16  - 16-bit RGB + alpha
+/// | RGB32F  - 32-bit floating RGB
+/// | RGBA32F - 32-bit floating RGB + alpha
 #[allow(clippy::upper_case_acronyms)]
 #[derive(Clone, Copy, Debug, PartialEq, Eq, Serialize, Deserialize, Hash, FromPrimitive)]
 #[cfg_attr(feature = "python", pyclass)]
 pub enum ImageMode {
     L = 1,
     LA = 2,
     RGB = 3,
@@ -39,14 +39,19 @@
     RGBA32F = 10,
 }
 
 #[cfg(feature = "python")]
 #[pymethods]
 impl ImageMode {
     /// Create an ImageMode from its string representation.
+    ///
+    /// Args:
+    ///     mode: String representation of the mode. This is the same as the enum
+    ///         attribute name, e.g. ``ImageMode.from_mode_string("RGB")`` would
+    ///         return ``ImageMode.RGB``.
     #[staticmethod]
     pub fn from_mode_string(mode: &str) -> PyResult<Self> {
         Self::from_str(mode).map_err(|e| PyValueError::new_err(e.to_string()))
     }
 
     pub fn __str__(&self) -> PyResult<String> {
         Ok(self.to_string())
```

### Comparing `getdaft-0.1.5/src/datatypes/logical.rs` & `getdaft-0.1.6/src/datatypes/logical.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 use std::{marker::PhantomData, sync::Arc};
 
 use crate::{
     datatypes::{DaftLogicalType, DateType, Field},
     error::DaftResult,
 };
 
-use super::{DataArray, DataType, EmbeddingType, FixedShapeImageType, ImageType};
+use super::{DataArray, DataType, EmbeddingType, FixedShapeImageType, ImageType, TimestampType};
 pub struct LogicalArray<L: DaftLogicalType> {
     pub field: Arc<Field>,
     pub physical: DataArray<L::PhysicalType>,
     marker_: PhantomData<L>,
 }
 
 impl<L: DaftLogicalType + 'static> LogicalArray<L> {
@@ -91,7 +91,8 @@
     }
 }
 
 pub type DateArray = LogicalArray<DateType>;
 pub type EmbeddingArray = LogicalArray<EmbeddingType>;
 pub type ImageArray = LogicalArray<ImageType>;
 pub type FixedShapeImageArray = LogicalArray<FixedShapeImageType>;
+pub type TimestampArray = LogicalArray<TimestampType>;
```

### Comparing `getdaft-0.1.5/src/datatypes/matching.rs` & `getdaft-0.1.6/src/datatypes/matching.rs`

 * *Files 0% similar despite different names*

```diff
@@ -227,13 +227,14 @@
     macro_rules! __with_ty__ {( $_ $T:ident ) => ( $($body)* )}
     use $crate::datatypes::DataType::*;
     #[allow(unused_imports)]
     use $crate::datatypes::*;
 
     match $key_type {
         Date => __with_ty__! { DateType },
+        Timestamp(..) => __with_ty__! { TimestampType },
         Embedding(..) => __with_ty__! { EmbeddingType },
         Image(..) => __with_ty__! { ImageType },
         FixedShapeImage(..) => __with_ty__! { FixedShapeImageType },
         _ => panic!("{:?} not implemented for with_match_daft_logical_types", $key_type)
     }
 })}
```

### Comparing `getdaft-0.1.5/src/datatypes/mod.rs` & `getdaft-0.1.6/src/datatypes/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 mod dtype;
 mod field;
+mod image_format;
 mod image_mode;
 mod matching;
 mod time_unit;
 
 use std::ops::{Add, Div, Mul, Rem, Sub};
 
 pub use crate::array::DataArray;
 use arrow2::{
     compute::{arithmetics::basic::NativeArithmetics, comparison::Simd8},
     types::{simd::Simd, NativeType},
 };
 pub use dtype::DataType;
 pub use field::Field;
+pub use image_format::ImageFormat;
 pub use image_mode::ImageMode;
 use num_traits::{Bounded, Float, FromPrimitive, Num, NumCast, ToPrimitive, Zero};
 pub use time_unit::TimeUnit;
 pub mod logical;
 
 /// Trait to wrap DataType Enum
 pub trait DaftDataType: Sync + Send {
```

### Comparing `getdaft-0.1.5/src/datatypes/time_unit.rs` & `getdaft-0.1.6/src/datatypes/time_unit.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/dsl/arithmetic.rs` & `getdaft-0.1.6/src/dsl/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/dsl/expr.rs` & `getdaft-0.1.6/src/dsl/expr.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/dsl/functions/float/is_nan.rs` & `getdaft-0.1.6/src/dsl/functions/float/is_nan.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/dsl/functions/float/mod.rs` & `getdaft-0.1.6/src/dsl/functions/float/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/dsl/functions/image/decode.rs` & `getdaft-0.1.6/src/dsl/functions/image/decode.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/dsl/functions/image/resize.rs` & `getdaft-0.1.6/src/dsl/functions/image/resize.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/dsl/functions/list/explode.rs` & `getdaft-0.1.6/src/dsl/functions/list/explode.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/dsl/functions/list/mod.rs` & `getdaft-0.1.6/src/dsl/functions/list/mod.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 mod explode;
+mod join;
 
 use explode::ExplodeEvaluator;
+use join::JoinEvaluator;
 use serde::{Deserialize, Serialize};
 
 use crate::dsl::Expr;
 
 use super::FunctionEvaluator;
 
 #[derive(Debug, Clone, Serialize, Deserialize, PartialEq)]
 pub enum ListExpr {
     Explode,
+    Join,
 }
 
 impl ListExpr {
     #[inline]
     pub fn get_evaluator(&self) -> &dyn FunctionEvaluator {
         use ListExpr::*;
         match self {
             Explode => &ExplodeEvaluator {},
+            Join => &JoinEvaluator {},
         }
     }
 }
 
 pub fn explode(input: &Expr) -> Expr {
     Expr::Function {
         func: super::FunctionExpr::List(ListExpr::Explode),
         inputs: vec![input.clone()],
     }
 }
+
+pub fn join(input: &Expr, delimiter: &Expr) -> Expr {
+    Expr::Function {
+        func: super::FunctionExpr::List(ListExpr::Join),
+        inputs: vec![input.clone(), delimiter.clone()],
+    }
+}
```

### Comparing `getdaft-0.1.5/src/dsl/functions/mod.rs` & `getdaft-0.1.6/src/dsl/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/dsl/functions/numeric/abs.rs` & `getdaft-0.1.6/src/dsl/functions/numeric/abs.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/dsl/functions/numeric/mod.rs` & `getdaft-0.1.6/src/dsl/functions/numeric/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/dsl/functions/python/mod.rs` & `getdaft-0.1.6/src/dsl/functions/python/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/dsl/functions/python/partial_udf.rs` & `getdaft-0.1.6/src/dsl/functions/python/partial_udf.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/dsl/functions/python/udf.rs` & `getdaft-0.1.6/src/dsl/functions/python/udf.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/dsl/functions/temporal/day.rs` & `getdaft-0.1.6/src/dsl/functions/temporal/day.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/dsl/functions/temporal/day_of_week.rs` & `getdaft-0.1.6/src/dsl/functions/temporal/day_of_week.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/dsl/functions/temporal/mod.rs` & `getdaft-0.1.6/src/dsl/functions/temporal/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/dsl/functions/temporal/month.rs` & `getdaft-0.1.6/src/dsl/functions/temporal/month.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/dsl/functions/temporal/year.rs` & `getdaft-0.1.6/src/dsl/functions/temporal/year.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/dsl/functions/utf8/contains.rs` & `getdaft-0.1.6/src/dsl/functions/utf8/contains.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/dsl/functions/utf8/endswith.rs` & `getdaft-0.1.6/src/dsl/functions/utf8/endswith.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/dsl/functions/utf8/length.rs` & `getdaft-0.1.6/src/dsl/functions/utf8/length.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/dsl/functions/utf8/mod.rs` & `getdaft-0.1.6/src/dsl/functions/utf8/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/dsl/functions/utf8/startswith.rs` & `getdaft-0.1.6/src/dsl/functions/utf8/startswith.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/dsl/lit.rs` & `getdaft-0.1.6/src/dsl/lit.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/dsl/optimization.rs` & `getdaft-0.1.6/src/dsl/optimization.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/dsl/pyobject.rs` & `getdaft-0.1.6/src/dsl/pyobject.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/error.rs` & `getdaft-0.1.6/src/error.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/ffi.rs` & `getdaft-0.1.6/src/ffi.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/kernels/hashing.rs` & `getdaft-0.1.6/src/kernels/hashing.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/kernels/search_sorted.rs` & `getdaft-0.1.6/src/kernels/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/kernels/utf8.rs` & `getdaft-0.1.6/src/kernels/utf8.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/lib.rs` & `getdaft-0.1.6/src/lib.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/python/expr.rs` & `getdaft-0.1.6/src/python/expr.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 use std::collections::HashSet;
 
 use super::field::PyField;
 use super::{datatype::PyDataType, schema::PySchema};
-use crate::dsl::{self, functions, optimization, Expr};
+use crate::{
+    datatypes::ImageFormat,
+    dsl::{self, functions, optimization, Expr},
+};
 use pyo3::{
     exceptions::PyValueError,
     prelude::*,
     pyclass::CompareOp,
     types::{PyBool, PyBytes, PyFloat, PyInt, PyString, PyTuple},
 };
 
@@ -310,28 +313,38 @@
     }
 
     pub fn image_decode(&self) -> PyResult<Self> {
         use dsl::functions::image::decode;
         Ok(decode(&self.expr).into())
     }
 
+    pub fn image_encode(&self, image_format: ImageFormat) -> PyResult<Self> {
+        use dsl::functions::image::encode;
+        Ok(encode(&self.expr, image_format).into())
+    }
+
     pub fn image_resize(&self, w: i64, h: i64) -> PyResult<Self> {
         if w < 0 {
             return Err(PyValueError::new_err(format!(
                 "width can not be negative: {w}"
             )));
         }
         if h < 0 {
             return Err(PyValueError::new_err(format!(
                 "height can not be negative: {h}"
             )));
         }
         use dsl::functions::image::resize;
         Ok(resize(&self.expr, w as u32, h as u32).into())
     }
+
+    pub fn list_join(&self, delimiter: &Self) -> PyResult<Self> {
+        use dsl::functions::list::join;
+        Ok(join(&self.expr, &delimiter.expr).into())
+    }
 }
 
 impl From<dsl::Expr> for PyExpr {
     fn from(value: dsl::Expr) -> Self {
         PyExpr { expr: value }
     }
 }
```

### Comparing `getdaft-0.1.5/src/python/field.rs` & `getdaft-0.1.6/src/python/field.rs`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     types::{PyBytes, PyTuple},
 };
 
 use super::datatype::PyDataType;
 use crate::datatypes::{self, DataType, Field};
 
 #[pyclass]
+#[derive(Clone)]
 pub struct PyField {
     pub field: datatypes::Field,
 }
 
 #[pymethods]
 impl PyField {
     #[new]
```

### Comparing `getdaft-0.1.5/src/python/mod.rs` & `getdaft-0.1.6/src/python/mod.rs`

 * *Files 16% similar despite different names*

```diff
@@ -3,26 +3,29 @@
 mod error;
 mod expr;
 mod field;
 mod schema;
 mod series;
 mod table;
 
+use crate::datatypes::ImageFormat;
 use crate::datatypes::ImageMode;
 pub use datatype::PyDataType;
 pub use series::PySeries;
 
 pub fn register_modules(_py: Python, parent: &PyModule) -> PyResult<()> {
     parent.add_class::<expr::PyExpr>()?;
     parent.add_class::<table::PyTable>()?;
     parent.add_class::<series::PySeries>()?;
     parent.add_class::<datatype::PyDataType>()?;
+    parent.add_class::<datatype::PyTimeUnit>()?;
     parent.add_class::<schema::PySchema>()?;
     parent.add_class::<field::PyField>()?;
     parent.add_class::<ImageMode>()?;
+    parent.add_class::<ImageFormat>()?;
 
     parent.add_wrapped(wrap_pyfunction!(expr::col))?;
     parent.add_wrapped(wrap_pyfunction!(expr::lit))?;
     parent.add_wrapped(wrap_pyfunction!(expr::udf))?;
     parent.add_wrapped(wrap_pyfunction!(expr::eq))?;
 
     Ok(())
```

### Comparing `getdaft-0.1.5/src/python/schema.rs` & `getdaft-0.1.6/src/python/schema.rs`

 * *Files 11% similar despite different names*

```diff
@@ -60,27 +60,42 @@
             .collect();
         let schema = schema::Schema::new(fields)?;
         Ok(PySchema {
             schema: schema.into(),
         })
     }
 
+    #[staticmethod]
+    pub fn from_fields(fields: Vec<PyField>) -> PyResult<PySchema> {
+        Ok(PySchema {
+            schema: schema::Schema::new(fields.iter().map(|f| f.field.clone()).collect())?.into(),
+        })
+    }
+
     pub fn __setstate__(&mut self, py: Python, state: PyObject) -> PyResult<()> {
         match state.extract::<&PyBytes>(py) {
             Ok(s) => {
                 self.schema = bincode::deserialize(s.as_bytes()).unwrap();
                 Ok(())
             }
             Err(e) => Err(e),
         }
     }
 
     pub fn __getstate__(&self, py: Python) -> PyResult<PyObject> {
         Ok(PyBytes::new(py, &bincode::serialize(&self.schema).unwrap()).to_object(py))
     }
+
+    pub fn __repr__(&self) -> PyResult<String> {
+        Ok(format!("{}", self.schema))
+    }
+
+    pub fn _repr_html_(&self) -> PyResult<String> {
+        Ok(self.schema.repr_html())
+    }
 }
 
 impl From<schema::SchemaRef> for PySchema {
     fn from(schema: schema::SchemaRef) -> Self {
         PySchema { schema }
     }
 }
```

### Comparing `getdaft-0.1.5/src/python/series.rs` & `getdaft-0.1.6/src/python/series.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use std::ops::{Add, Div, Mul, Rem, Sub};
 
 use pyo3::{exceptions::PyValueError, prelude::*, pyclass::CompareOp, types::PyList};
 
 use crate::{
     array::{ops::DaftLogical, pseudo_arrow::PseudoArrowArray, DataArray},
-    datatypes::{DataType, Field, PythonType, UInt64Type},
+    datatypes::{DataType, Field, ImageFormat, PythonType, UInt64Type},
     ffi,
     series::{self, IntoSeries, Series},
     utils::arrow::{cast_array_for_daft_if_needed, cast_array_from_daft_if_needed},
 };
 
 use super::datatype::PyDataType;
 use crate::array::ops::as_arrow::AsArrow;
@@ -265,14 +265,19 @@
     pub fn arr_lengths(&self) -> PyResult<Self> {
         Ok(self.series.arr_lengths()?.into_series().into())
     }
 
     pub fn image_decode(&self) -> PyResult<Self> {
         Ok(self.series.image_decode()?.into())
     }
+
+    pub fn image_encode(&self, image_format: ImageFormat) -> PyResult<Self> {
+        Ok(self.series.image_encode(image_format)?.into())
+    }
+
     pub fn image_resize(&self, w: i64, h: i64) -> PyResult<Self> {
         if w < 0 {
             return Err(PyValueError::new_err(format!(
                 "width can not be negative: {w}"
             )));
         }
         if h < 0 {
```

### Comparing `getdaft-0.1.5/src/python/table.rs` & `getdaft-0.1.6/src/python/table.rs`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,18 @@
 impl PyTable {
     pub fn schema(&self) -> PyResult<PySchema> {
         Ok(PySchema {
             schema: self.table.schema.clone(),
         })
     }
 
+    pub fn cast_to_schema(&self, schema: &PySchema) -> PyResult<Self> {
+        Ok(self.table.cast_to_schema(&schema.schema)?.into())
+    }
+
     pub fn eval_expression_list(&self, py: Python, exprs: Vec<PyExpr>) -> PyResult<Self> {
         let converted_exprs: Vec<dsl::Expr> = exprs.into_iter().map(|e| e.into()).collect();
         py.allow_threads(|| {
             Ok(self
                 .table
                 .eval_expression_list(converted_exprs.as_slice())?
                 .into())
@@ -113,14 +117,18 @@
         py.allow_threads(|| Ok(self.table.explode(converted_to_explode.as_slice())?.into()))
     }
 
     pub fn __repr__(&self) -> PyResult<String> {
         Ok(format!("{}", self.table))
     }
 
+    pub fn _repr_html_(&self) -> PyResult<String> {
+        Ok(self.table.repr_html())
+    }
+
     pub fn head(&self, py: Python, num: i64) -> PyResult<Self> {
         if num < 0 {
             return Err(PyValueError::new_err(format!(
                 "Can not head table with negative number: {num}"
             )));
         }
         let num = num as usize;
```

### Comparing `getdaft-0.1.5/src/schema.rs` & `getdaft-0.1.6/src/schema.rs`

 * *Files 23% similar despite different names*

```diff
@@ -154,36 +154,76 @@
 00000990: 726f 723a 3a56 616c 7565 4572 726f 7228  ror::ValueError(
 000009a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000009b0: 2022 4361 6e6e 6f74 2075 6e69 6f6e 2074   "Cannot union t
 000009c0: 776f 2073 6368 656d 6173 2077 6974 6820  wo schemas with 
 000009d0: 6f76 6572 6c61 7070 696e 6720 6b65 7973  overlapping keys
 000009e0: 222e 746f 5f73 7472 696e 6728 292c 0a20  ".to_string(),. 
 000009f0: 2020 2020 2020 2020 2020 2029 292c 0a20             )),. 
-00000a00: 2020 2020 2020 207d 0a20 2020 207d 0a7d         }.    }.}
-00000a10: 0a0a 696d 706c 2044 6973 706c 6179 2066  ..impl Display f
-00000a20: 6f72 2053 6368 656d 6120 7b0a 2020 2020  or Schema {.    
-00000a30: 2f2f 2060 6660 2069 7320 6120 6275 6666  // `f` is a buff
-00000a40: 6572 2c20 616e 6420 7468 6973 206d 6574  er, and this met
-00000a50: 686f 6420 6d75 7374 2077 7269 7465 2074  hod must write t
-00000a60: 6865 2066 6f72 6d61 7474 6564 2073 7472  he formatted str
-00000a70: 696e 6720 696e 746f 2069 740a 2020 2020  ing into it.    
-00000a80: 666e 2066 6d74 2826 7365 6c66 2c20 663a  fn fmt(&self, f:
-00000a90: 2026 6d75 7420 466f 726d 6174 7465 7229   &mut Formatter)
-00000aa0: 202d 3e20 5265 7375 6c74 207b 0a20 2020   -> Result {.   
-00000ab0: 2020 2020 206c 6574 206d 7574 2074 6162       let mut tab
-00000ac0: 6c65 203d 2070 7265 7474 7974 6162 6c65  le = prettytable
-00000ad0: 3a3a 5461 626c 653a 3a6e 6577 2829 3b0a  ::Table::new();.
-00000ae0: 0a20 2020 2020 2020 206c 6574 2068 6561  .        let hea
-00000af0: 6465 7220 3d20 7365 6c66 0a20 2020 2020  der = self.     
-00000b00: 2020 2020 2020 202e 6669 656c 6473 0a20         .fields. 
-00000b10: 2020 2020 2020 2020 2020 202e 6974 6572             .iter
-00000b20: 2829 0a20 2020 2020 2020 2020 2020 202e  ().            .
-00000b30: 6d61 7028 7c28 6e61 6d65 2c20 6669 656c  map(|(name, fiel
-00000b40: 6429 7c20 666f 726d 6174 2128 227b 7d5c  d)| format!("{}\
-00000b50: 6e7b 3a3f 7d22 2c20 6e61 6d65 2c20 6669  n{:?}", name, fi
-00000b60: 656c 642e 6474 7970 6529 290a 2020 2020  eld.dtype)).    
-00000b70: 2020 2020 2020 2020 2e63 6f6c 6c65 6374          .collect
-00000b80: 2829 3b0a 2020 2020 2020 2020 7461 626c  ();.        tabl
-00000b90: 652e 6164 645f 726f 7728 6865 6164 6572  e.add_row(header
-00000ba0: 293b 0a20 2020 2020 2020 2077 7269 7465  );.        write
-00000bb0: 2128 662c 2022 7b74 6162 6c65 7d22 290a  !(f, "{table}").
-00000bc0: 2020 2020 7d0a 7d0a                          }.}.
+00000a00: 2020 2020 2020 207d 0a20 2020 207d 0a0a         }.    }..
+00000a10: 2020 2020 7075 6220 666e 2072 6570 725f      pub fn repr_
+00000a20: 6874 6d6c 2826 7365 6c66 2920 2d3e 2053  html(&self) -> S
+00000a30: 7472 696e 6720 7b0a 2020 2020 2020 2020  tring {.        
+00000a40: 2f2f 2050 726f 6475 6365 7320 6120 3c74  // Produces a <t
+00000a50: 6162 6c65 3e20 4854 4d4c 2065 6c65 6d65  able> HTML eleme
+00000a60: 6e74 2e0a 0a20 2020 2020 2020 206c 6574  nt...        let
+00000a70: 206d 7574 2072 6573 203d 2022 3c74 6162   mut res = "<tab
+00000a80: 6c65 2063 6c61 7373 3d5c 2264 6174 6166  le class=\"dataf
+00000a90: 7261 6d65 5c22 3e5c 6e22 2e74 6f5f 7374  rame\">\n".to_st
+00000aa0: 7269 6e67 2829 3b0a 0a20 2020 2020 2020  ring();..       
+00000ab0: 202f 2f20 4265 6769 6e20 7468 6520 6865   // Begin the he
+00000ac0: 6164 6572 2e0a 2020 2020 2020 2020 7265  ader..        re
+00000ad0: 732e 7075 7368 5f73 7472 2822 3c74 6865  s.push_str("<the
+00000ae0: 6164 3e3c 7472 3e22 293b 0a0a 2020 2020  ad><tr>");..    
+00000af0: 2020 2020 666f 7220 286e 616d 652c 2066      for (name, f
+00000b00: 6965 6c64 2920 696e 2026 7365 6c66 2e66  ield) in &self.f
+00000b10: 6965 6c64 7320 7b0a 2020 2020 2020 2020  ields {.        
+00000b20: 2020 2020 7265 732e 7075 7368 5f73 7472      res.push_str
+00000b30: 2822 3c74 683e 2229 3b0a 2020 2020 2020  ("<th>");.      
+00000b40: 2020 2020 2020 7265 732e 7075 7368 5f73        res.push_s
+00000b50: 7472 2826 6874 6d6c 5f65 7363 6170 653a  tr(&html_escape:
+00000b60: 3a65 6e63 6f64 655f 7465 7874 286e 616d  :encode_text(nam
+00000b70: 6529 293b 0a20 2020 2020 2020 2020 2020  e));.           
+00000b80: 2072 6573 2e70 7573 685f 7374 7228 223c   res.push_str("<
+00000b90: 6272 202f 3e22 293b 0a20 2020 2020 2020  br />");.       
+00000ba0: 2020 2020 2072 6573 2e70 7573 685f 7374       res.push_st
+00000bb0: 7228 2668 746d 6c5f 6573 6361 7065 3a3a  r(&html_escape::
+00000bc0: 656e 636f 6465 5f74 6578 7428 2666 6f72  encode_text(&for
+00000bd0: 6d61 7421 2822 7b7d 222c 2066 6965 6c64  mat!("{}", field
+00000be0: 2e64 7479 7065 2929 293b 0a20 2020 2020  .dtype)));.     
+00000bf0: 2020 2020 2020 2072 6573 2e70 7573 685f         res.push_
+00000c00: 7374 7228 223c 2f74 683e 2229 3b0a 2020  str("</th>");.  
+00000c10: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
+00000c20: 202f 2f20 456e 6420 7468 6520 6865 6164   // End the head
+00000c30: 6572 2e0a 2020 2020 2020 2020 7265 732e  er..        res.
+00000c40: 7075 7368 5f73 7472 2822 3c2f 7472 3e3c  push_str("</tr><
+00000c50: 2f74 6865 6164 3e5c 6e22 293b 0a0a 2020  /thead>\n");..  
+00000c60: 2020 2020 2020 7265 732e 7075 7368 5f73        res.push_s
+00000c70: 7472 2822 3c2f 7461 626c 653e 2229 3b0a  tr("</table>");.
+00000c80: 0a20 2020 2020 2020 2072 6573 0a20 2020  .        res.   
+00000c90: 207d 0a7d 0a0a 696d 706c 2044 6973 706c   }.}..impl Displ
+00000ca0: 6179 2066 6f72 2053 6368 656d 6120 7b0a  ay for Schema {.
+00000cb0: 2020 2020 2f2f 2060 6660 2069 7320 6120      // `f` is a 
+00000cc0: 6275 6666 6572 2c20 616e 6420 7468 6973  buffer, and this
+00000cd0: 206d 6574 686f 6420 6d75 7374 2077 7269   method must wri
+00000ce0: 7465 2074 6865 2066 6f72 6d61 7474 6564  te the formatted
+00000cf0: 2073 7472 696e 6720 696e 746f 2069 740a   string into it.
+00000d00: 2020 2020 666e 2066 6d74 2826 7365 6c66      fn fmt(&self
+00000d10: 2c20 663a 2026 6d75 7420 466f 726d 6174  , f: &mut Format
+00000d20: 7465 7229 202d 3e20 5265 7375 6c74 207b  ter) -> Result {
+00000d30: 0a20 2020 2020 2020 206c 6574 206d 7574  .        let mut
+00000d40: 2074 6162 6c65 203d 2070 7265 7474 7974   table = prettyt
+00000d50: 6162 6c65 3a3a 5461 626c 653a 3a6e 6577  able::Table::new
+00000d60: 2829 3b0a 0a20 2020 2020 2020 206c 6574  ();..        let
+00000d70: 2068 6561 6465 7220 3d20 7365 6c66 0a20   header = self. 
+00000d80: 2020 2020 2020 2020 2020 202e 6669 656c             .fiel
+00000d90: 6473 0a20 2020 2020 2020 2020 2020 202e  ds.            .
+00000da0: 6974 6572 2829 0a20 2020 2020 2020 2020  iter().         
+00000db0: 2020 202e 6d61 7028 7c28 6e61 6d65 2c20     .map(|(name, 
+00000dc0: 6669 656c 6429 7c20 666f 726d 6174 2128  field)| format!(
+00000dd0: 227b 7d5c 6e7b 3a3f 7d22 2c20 6e61 6d65  "{}\n{:?}", name
+00000de0: 2c20 6669 656c 642e 6474 7970 6529 290a  , field.dtype)).
+00000df0: 2020 2020 2020 2020 2020 2020 2e63 6f6c              .col
+00000e00: 6c65 6374 2829 3b0a 2020 2020 2020 2020  lect();.        
+00000e10: 7461 626c 652e 6164 645f 726f 7728 6865  table.add_row(he
+00000e20: 6164 6572 293b 0a20 2020 2020 2020 2077  ader);.        w
+00000e30: 7269 7465 2128 662c 2022 7b74 6162 6c65  rite!(f, "{table
+00000e40: 7d22 290a 2020 2020 7d0a 7d0a            }").    }.}.
```

### Comparing `getdaft-0.1.5/src/series/array_impl/data_array.rs` & `getdaft-0.1.6/src/series/array_impl/data_array.rs`

 * *Files 3% similar despite different names*

```diff
@@ -126,14 +126,26 @@
                 .downcast_ref::<arrow2::array::PrimitiveArray<i32>>()
                 .unwrap();
             let casted: Box<dyn arrow2::array::Array> =
                 Box::new(downcasted.clone().to(arrow2::datatypes::DataType::Date32));
             Cow::Owned(casted)
         }
 
+        DataType::Timestamp(unit, tz) => {
+            let downcasted = arr
+                .as_ref()
+                .as_any()
+                .downcast_ref::<arrow2::array::PrimitiveArray<i64>>()
+                .unwrap();
+            let casted: Box<dyn arrow2::array::Array> = Box::new(downcasted.clone().to(
+                arrow2::datatypes::DataType::Timestamp(unit.to_arrow().unwrap(), tz.clone()),
+            ));
+            Cow::Owned(casted)
+        }
+
         _ => arr,
     }
 }
 
 impl<T: DaftArrowBackedType> IntoSeries for DataArray<T>
 where
     ArrayWrapper<DataArray<T>>: SeriesLike,
@@ -217,14 +229,17 @@
             }
             fn sort(&self, descending: bool) -> DaftResult<Series> {
                 Ok(self.0.sort(descending)?.into_series())
             }
             fn str_value(&self, idx: usize) -> DaftResult<String> {
                 self.0.str_value(idx)
             }
+            fn html_value(&self, idx: usize) -> String {
+                self.0.html_value(idx)
+            }
             fn take(&self, idx: &Series) -> DaftResult<Series> {
                 with_match_integer_daft_types!(idx.data_type(), |$S| {
                     Ok(self.0.take(idx.downcast::<$S>()?)?.into_series())
                 })
             }
 
             fn min(&self, groups: Option<&GroupIndices>) -> DaftResult<Series> {
```

### Comparing `getdaft-0.1.5/src/series/array_impl/logical_array.rs` & `getdaft-0.1.6/src/series/array_impl/logical_array.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-use crate::datatypes::logical::{DateArray, EmbeddingArray, FixedShapeImageArray, ImageArray};
+use crate::datatypes::logical::{
+    DateArray, EmbeddingArray, FixedShapeImageArray, ImageArray, TimestampArray,
+};
 
 use super::{ArrayWrapper, IntoSeries, Series};
 use crate::array::ops::GroupIndices;
 use crate::series::DaftResult;
 use crate::series::SeriesLike;
 use crate::with_match_integer_daft_types;
 use std::sync::Arc;
@@ -96,15 +98,19 @@
             }
 
             fn sort(&self, descending: bool) -> DaftResult<Series> {
                 Ok(self.0.sort(descending)?.into_series())
             }
 
             fn str_value(&self, idx: usize) -> DaftResult<String> {
-                self.0.physical.str_value(idx)
+                self.0.str_value(idx)
+            }
+
+            fn html_value(&self, idx: usize) -> String {
+                self.0.html_value(idx)
             }
 
             fn take(&self, idx: &Series) -> DaftResult<Series> {
                 with_match_integer_daft_types!(idx.data_type(), |$S| {
                     Ok(self.0.take(idx.downcast::<$S>()?)?.into_series())
                 })
             }
@@ -139,7 +145,8 @@
     };
 }
 
 impl_series_like_for_logical_array!(DateArray);
 impl_series_like_for_logical_array!(EmbeddingArray);
 impl_series_like_for_logical_array!(ImageArray);
 impl_series_like_for_logical_array!(FixedShapeImageArray);
+impl_series_like_for_logical_array!(TimestampArray);
```

### Comparing `getdaft-0.1.5/src/series/from.rs` & `getdaft-0.1.6/src/series/from.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/series/mod.rs` & `getdaft-0.1.6/src/series/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -46,19 +46,16 @@
         let physical_dtype = self.data_type().to_physical();
         if &physical_dtype == self.data_type() {
             Ok(self.clone())
         } else {
             self.inner.cast(&physical_dtype)
         }
     }
-}
 
-impl Display for Series {
-    // `f` is a buffer, and this method must write the formatted string into it
-    fn fmt(&self, f: &mut Formatter) -> Result {
+    pub fn to_prettytable(&self) -> prettytable::Table {
         let mut table = prettytable::Table::new();
 
         let header =
             prettytable::Cell::new(format!("{}\n{}", self.name(), self.data_type()).as_str())
                 .with_style(prettytable::Attr::Bold);
         table.add_row(prettytable::Row::new(vec![header]));
 
@@ -83,13 +80,21 @@
         }
 
         for i in 0..tail_rows {
             let row = vec![self.str_value(self.len() - tail_rows - 1 + i).unwrap()];
             table.add_row(row.into());
         }
 
+        table
+    }
+}
+
+impl Display for Series {
+    // `f` is a buffer, and this method must write the formatted string into it
+    fn fmt(&self, f: &mut Formatter) -> Result {
+        let table = self.to_prettytable();
         write!(f, "{table}")
     }
 }
 
 #[cfg(test)]
 mod tests {}
```

### Comparing `getdaft-0.1.5/src/series/ops/abs.rs` & `getdaft-0.1.6/src/series/ops/abs.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/series/ops/agg.rs` & `getdaft-0.1.6/src/series/ops/agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/series/ops/arithmetic.rs` & `getdaft-0.1.6/src/series/ops/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/series/ops/broadcast.rs` & `getdaft-0.1.6/src/series/ops/broadcast.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/series/ops/comparison.rs` & `getdaft-0.1.6/src/series/ops/comparison.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/series/ops/concat.rs` & `getdaft-0.1.6/src/series/ops/concat.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/series/ops/date.rs` & `getdaft-0.1.6/src/series/ops/date.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/series/ops/downcast.rs` & `getdaft-0.1.6/src/series/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/series/ops/filter.rs` & `getdaft-0.1.6/src/series/ops/filter.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/series/ops/list.rs` & `getdaft-0.1.6/src/series/ops/list.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 use crate::array::ops::as_arrow::AsArrow;
-use crate::datatypes::{DataType, UInt64Array};
+use crate::datatypes::{DataType, UInt64Array, Utf8Array};
 use crate::error::DaftError;
 use crate::{error::DaftResult, series::Series};
 
 impl Series {
     pub fn explode(&self) -> DaftResult<Series> {
         use DataType::*;
         match self.data_type() {
@@ -45,8 +45,19 @@
             }
             dt => Err(DaftError::TypeError(format!(
                 "lengths not implemented for {}",
                 dt
             ))),
         }
     }
+
+    pub fn join(&self, delimiter: &Utf8Array) -> DaftResult<Utf8Array> {
+        match self.data_type() {
+            DataType::List(_) => self.list()?.join(delimiter),
+            DataType::FixedSizeList(..) => self.fixed_size_list()?.join(delimiter),
+            dt => Err(DaftError::TypeError(format!(
+                "Join not implemented for {}",
+                dt
+            ))),
+        }
+    }
 }
```

### Comparing `getdaft-0.1.5/src/series/ops/mod.rs` & `getdaft-0.1.6/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/series/ops/search_sorted.rs` & `getdaft-0.1.6/src/series/ops/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/series/ops/sort.rs` & `getdaft-0.1.6/src/series/ops/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/series/ops/take.rs` & `getdaft-0.1.6/src/series/ops/take.rs`

 * *Files 16% similar despite different names*

```diff
@@ -15,8 +15,12 @@
     pub fn take(&self, idx: &Series) -> DaftResult<Series> {
         self.inner.take(idx)
     }
 
     pub fn str_value(&self, idx: usize) -> DaftResult<String> {
         self.inner.str_value(idx)
     }
+
+    pub fn html_value(&self, idx: usize) -> String {
+        self.inner.html_value(idx)
+    }
 }
```

### Comparing `getdaft-0.1.5/src/series/ops/utf8.rs` & `getdaft-0.1.6/src/series/ops/utf8.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/series/series_like.rs` & `getdaft-0.1.6/src/series/series_like.rs`

 * *Files 11% similar despite different names*

```diff
@@ -26,8 +26,9 @@
     fn size_bytes(&self) -> DaftResult<usize>;
     fn is_null(&self) -> DaftResult<Series>;
     fn sort(&self, descending: bool) -> DaftResult<Series>;
     fn head(&self, num: usize) -> DaftResult<Series>;
     fn slice(&self, start: usize, end: usize) -> DaftResult<Series>;
     fn take(&self, idx: &Series) -> DaftResult<Series>;
     fn str_value(&self, idx: usize) -> DaftResult<String>;
+    fn html_value(&self, idx: usize) -> String;
 }
```

### Comparing `getdaft-0.1.5/src/table/mod.rs` & `getdaft-0.1.6/src/table/mod.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+use std::collections::HashSet;
 use std::fmt::{Display, Formatter, Result};
 
 use num_traits::ToPrimitive;
 
 use crate::array::ops::GroupIndices;
 
 use crate::datatypes::logical::LogicalArray;
 use crate::datatypes::{BooleanType, DataType, Field, UInt64Array};
 use crate::dsl::functions::FunctionEvaluator;
-use crate::dsl::{AggExpr, Expr};
+use crate::dsl::{col, null_lit, AggExpr, Expr};
 use crate::error::{DaftError, DaftResult};
 use crate::schema::{Schema, SchemaRef};
 use crate::series::{IntoSeries, Series};
 use crate::{with_match_daft_logical_types, with_match_physical_daft_types};
 mod ops;
 #[derive(Clone)]
 pub struct Table {
@@ -341,15 +342,14 @@
             .map(|e| self.eval_expression(e))
             .collect::<DaftResult<Vec<Series>>>()?;
 
         let fields = result_series
             .iter()
             .map(|s| s.field().clone())
             .collect::<Vec<Field>>();
-        use std::collections::HashSet;
         let mut seen: HashSet<String> = HashSet::new();
         for field in fields.iter() {
             let name = &field.name;
             if seen.contains(name) {
                 return Err(DaftError::ValueError(format!(
                     "Duplicate name found when evaluating expressions: {name}"
                 )));
@@ -359,19 +359,109 @@
         let schema = Schema::new(fields)?;
         Table::new(schema, result_series)
     }
     pub fn as_physical(&self) -> DaftResult<Self> {
         let new_series: DaftResult<Vec<_>> = self.columns.iter().map(|s| s.as_physical()).collect();
         Table::from_columns(new_series?)
     }
-}
 
-impl Display for Table {
-    // `f` is a buffer, and this method must write the formatted string into it
-    fn fmt(&self, f: &mut Formatter) -> Result {
+    pub fn cast_to_schema(&self, schema: &Schema) -> DaftResult<Self> {
+        let current_col_names = HashSet::<_>::from_iter(self.column_names());
+        let exprs: Vec<_> = schema
+            .fields
+            .iter()
+            .map(|(name, field)| {
+                if current_col_names.contains(name) {
+                    // For any fields already in the table, perform a cast
+                    col(name.clone()).cast(&field.dtype)
+                } else {
+                    // For any fields in schema that are not in self.schema, create all-null arrays
+                    null_lit().alias(name.clone()).cast(&field.dtype)
+                }
+            })
+            .collect();
+        self.eval_expression_list(&exprs)
+    }
+
+    pub fn repr_html(&self) -> String {
+        // Produces a <table> HTML element.
+
+        let mut res = "<table class=\"dataframe\">\n".to_string();
+
+        // Begin the header.
+        res.push_str("<thead><tr>");
+
+        for (name, field) in &self.schema.fields {
+            res.push_str("<th>");
+            res.push_str(&html_escape::encode_text(name));
+            res.push_str("<br />");
+            res.push_str(&html_escape::encode_text(&format!("{}", field.dtype)));
+            res.push_str("</th>");
+        }
+
+        // End the header.
+        res.push_str("</tr></thead>\n");
+
+        // Begin the body.
+        res.push_str("<tbody>\n");
+
+        let head_rows;
+        let tail_rows;
+
+        if self.len() > 10 {
+            head_rows = 5;
+            tail_rows = 5;
+        } else {
+            head_rows = self.len();
+            tail_rows = 0;
+        }
+
+        for i in 0..head_rows {
+            // Begin row.
+            res.push_str("<tr>");
+
+            for col in self.columns.iter() {
+                res.push_str("<td>");
+                res.push_str(&col.html_value(i));
+                res.push_str("</td>");
+            }
+
+            // End row.
+            res.push_str("</tr>\n");
+        }
+
+        if tail_rows != 0 {
+            res.push_str("<tr>");
+            for _ in self.columns.iter() {
+                res.push_str("<td>...</td>");
+            }
+            res.push_str("</tr>\n");
+        }
+
+        for i in (self.len() - tail_rows)..(self.len()) {
+            // Begin row.
+            res.push_str("<tr>");
+
+            for col in self.columns.iter() {
+                res.push_str("<td>");
+                res.push_str(&col.html_value(i));
+                res.push_str("</td>");
+            }
+
+            // End row.
+            res.push_str("</tr>\n");
+        }
+
+        // End the body and the table.
+        res.push_str("</tbody>\n</table>");
+
+        res
+    }
+
+    pub fn to_prettytable(&self, max_col_width: Option<usize>) -> prettytable::Table {
         let mut table = prettytable::Table::new();
         let header = self
             .schema
             .fields
             .iter()
             .map(|(name, field)| {
                 prettytable::Cell::new(format!("{}\n{}", name, field.dtype).as_str())
@@ -391,34 +481,56 @@
             tail_rows = 0;
         }
 
         for i in 0..head_rows {
             let row = self
                 .columns
                 .iter()
-                .map(|s| s.str_value(i))
-                .collect::<DaftResult<Vec<String>>>()
-                .unwrap();
+                .map(|s| {
+                    let mut str_val = s.str_value(i).unwrap();
+                    if let Some(max_col_width) = max_col_width {
+                        if str_val.len() > max_col_width {
+                            str_val = format!("{}...", &str_val[..max_col_width - 3]);
+                        }
+                    }
+                    str_val
+                })
+                .collect::<Vec<String>>();
             table.add_row(row.into());
         }
         if tail_rows != 0 {
             let row: prettytable::Row = (0..self.num_columns()).map(|_| "...").collect();
             table.add_row(row);
         }
 
-        for i in 0..tail_rows {
+        for i in (self.len() - tail_rows)..(self.len()) {
             let row = self
                 .columns
                 .iter()
-                .map(|s| s.str_value(self.len() - tail_rows - 1 + i))
-                .collect::<DaftResult<Vec<String>>>()
-                .unwrap();
+                .map(|s| {
+                    let mut str_val = s.str_value(i).unwrap();
+                    if let Some(max_col_width) = max_col_width {
+                        if s.len() > max_col_width {
+                            str_val = format!("{}...", &str_val[..max_col_width - 3]);
+                        }
+                    }
+                    str_val
+                })
+                .collect::<Vec<String>>();
             table.add_row(row.into());
         }
 
+        table
+    }
+}
+
+impl Display for Table {
+    // `f` is a buffer, and this method must write the formatted string into it
+    fn fmt(&self, f: &mut Formatter) -> Result {
+        let table = self.to_prettytable(Some(32));
         write!(f, "{table}")
     }
 }
 
 #[cfg(test)]
 mod test {
```

### Comparing `getdaft-0.1.5/src/table/ops/agg.rs` & `getdaft-0.1.6/src/table/ops/agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/table/ops/explode.rs` & `getdaft-0.1.6/src/table/ops/explode.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/table/ops/groups.rs` & `getdaft-0.1.6/src/table/ops/groups.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/table/ops/hash.rs` & `getdaft-0.1.6/src/table/ops/hash.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/table/ops/joins/hash_join.rs` & `getdaft-0.1.6/src/table/ops/joins/hash_join.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/table/ops/joins/mod.rs` & `getdaft-0.1.6/src/table/ops/joins/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/table/ops/partition.rs` & `getdaft-0.1.6/src/table/ops/partition.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/table/ops/search_sorted.rs` & `getdaft-0.1.6/src/table/ops/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/table/ops/sort.rs` & `getdaft-0.1.6/src/table/ops/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/utils/arrow.rs` & `getdaft-0.1.6/src/utils/arrow.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/src/utils/supertype.rs` & `getdaft-0.1.6/src/utils/supertype.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/assets/tpch-sqlite-queries/1.sql` & `getdaft-0.1.6/tests/assets/tpch-sqlite-queries/1.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/assets/tpch-sqlite-queries/10.sql` & `getdaft-0.1.6/tests/assets/tpch-sqlite-queries/10.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/assets/tpch-sqlite-queries/2.sql` & `getdaft-0.1.6/tests/assets/tpch-sqlite-queries/2.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/assets/tpch-sqlite-queries/7.sql` & `getdaft-0.1.6/tests/assets/tpch-sqlite-queries/7.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/assets/tpch-sqlite-queries/8.sql` & `getdaft-0.1.6/tests/assets/tpch-sqlite-queries/8.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/assets/tpch-sqlite-queries/9.sql` & `getdaft-0.1.6/tests/assets/tpch-sqlite-queries/9.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/benchmarks/conftest.py` & `getdaft-0.1.6/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/benchmarks/test_df_arithmetic.py` & `getdaft-0.1.6/tests/benchmarks/test_df_arithmetic.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/benchmarks/test_file_read.py` & `getdaft-0.1.6/tests/benchmarks/test_file_read.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/benchmarks/test_groups_and_aggs.py` & `getdaft-0.1.6/tests/benchmarks/test_groups_and_aggs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/benchmarks/test_join.py` & `getdaft-0.1.6/tests/benchmarks/test_join.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/benchmarks/test_repartition.py` & `getdaft-0.1.6/tests/benchmarks/test_repartition.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/benchmarks/test_sort.py` & `getdaft-0.1.6/tests/benchmarks/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/conftest.py` & `getdaft-0.1.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/cookbook/assets/311-service-requests.24.csv` & `getdaft-0.1.6/tests/cookbook/assets/311-service-requests.24.csv`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/cookbook/assets/images/0000.jpg` & `getdaft-0.1.6/tests/cookbook/assets/images/0000.jpg`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/cookbook/assets/images/0007.jpg` & `getdaft-0.1.6/tests/cookbook/assets/images/0007.jpg`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/cookbook/assets/images/0018.png` & `getdaft-0.1.6/tests/cookbook/assets/images/0018.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/cookbook/assets/images/0025.tiff` & `getdaft-0.1.6/tests/cookbook/assets/images/0025.tiff`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/cookbook/conftest.py` & `getdaft-0.1.6/tests/cookbook/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/cookbook/test_aggregations.py` & `getdaft-0.1.6/tests/cookbook/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/cookbook/test_computations.py` & `getdaft-0.1.6/tests/cookbook/test_computations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/cookbook/test_count_rows.py` & `getdaft-0.1.6/tests/cookbook/test_count_rows.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/cookbook/test_dataloading.py` & `getdaft-0.1.6/tests/cookbook/test_dataloading.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/cookbook/test_distinct.py` & `getdaft-0.1.6/tests/cookbook/test_distinct.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/cookbook/test_filter.py` & `getdaft-0.1.6/tests/cookbook/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/cookbook/test_image.py` & `getdaft-0.1.6/tests/cookbook/test_image.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+import io
+
 import numpy as np
 from PIL import Image
 
 import daft
 from daft import col
 from daft.datatype import DataType
 from daft.series import Series
@@ -67,7 +69,29 @@
         daft.from_glob_path(f"{ASSET_FOLDER}/images/**")
         .into_partitions(2)
         .with_column("image", col("path").url.download().image.decode().image.resize(10, 10))
     )
     target_dtype = DataType.image()
     assert df.schema()["image"].dtype == target_dtype
     df.collect()
+
+
+def test_image_encode() -> None:
+    file_format = "png"
+    mode = "RGB"
+    np_dtype = np.uint8
+    shape = (4, 4, 3)
+    arr = np.arange(np.prod(shape)).reshape(shape).astype(np_dtype)
+    arrs = [arr, arr, arr]
+
+    s = Series.from_pylist(arrs, pyobj="force")
+
+    df = daft.from_pydict({"img": s}).into_partitions(2)
+    target_dtype = DataType.image(mode)
+    df = df.select(df["img"].cast(target_dtype))
+    assert df.schema()["img"].dtype == target_dtype
+
+    df = df.with_column("encoded", df["img"].image.encode(file_format))
+    assert df.schema()["encoded"].dtype == DataType.binary()
+
+    pil_decoded_imgs = [np.asarray(Image.open(io.BytesIO(bytes_))) for bytes_ in df.to_pydict()["encoded"]]
+    np.testing.assert_equal(pil_decoded_imgs, arrs)
```

### Comparing `getdaft-0.1.5/tests/cookbook/test_joins.py` & `getdaft-0.1.6/tests/cookbook/test_joins.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/cookbook/test_literals.py` & `getdaft-0.1.6/tests/cookbook/test_literals.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/cookbook/test_pandas_cookbook.py` & `getdaft-0.1.6/tests/cookbook/test_pandas_cookbook.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/cookbook/test_sorting.py` & `getdaft-0.1.6/tests/cookbook/test_sorting.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/cookbook/test_write.py` & `getdaft-0.1.6/tests/cookbook/test_write.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/dataframe/conftest.py` & `getdaft-0.1.6/tests/dataframe/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/dataframe/test_accessors.py` & `getdaft-0.1.6/tests/dataframe/test_accessors.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/dataframe/test_aggregations.py` & `getdaft-0.1.6/tests/dataframe/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/dataframe/test_creation.py` & `getdaft-0.1.6/tests/dataframe/test_creation.py`

 * *Files 4% similar despite different names*

```diff
@@ -231,15 +231,15 @@
     t = pa.Table.from_pydict(pydict)
     with pytest.raises(ValueError):
         daft.from_arrow(t)
 
 
 def test_create_dataframe_arrow_unsupported_dtype(valid_data: list[dict[str, float]]) -> None:
     pydict = {k: [item[k] for item in valid_data] for k in valid_data[0].keys()}
-    pydict["obj"] = [datetime.datetime.now() for _ in range(len(valid_data))]
+    pydict["obj"] = [datetime.timedelta(hours=1) for _ in range(len(valid_data))]
     t = pa.Table.from_pydict(pydict)
     df = daft.from_arrow(t)
     assert set(df.column_names) == set(t.column_names)
     # Type not natively supported, so should have Python object dtype.
     assert df.schema()["obj"].dtype == DataType.python()
     casted_field = t.schema.field("variety").with_type(pa.large_string())
     expected = t.cast(t.schema.set(t.schema.get_field_index("variety"), casted_field))
@@ -381,33 +381,14 @@
             # Check that open() is called on the passed filesystem.
             mock_open.assert_called()
 
         assert list(pd_df.columns) == COL_NAMES
         assert len(pd_df) == len(valid_data)
 
 
-@pytest.mark.parametrize("has_headers", [True, False])
-def test_create_dataframe_csv_provide_headers(valid_data: list[dict[str, float]], has_headers: bool) -> None:
-    with tempfile.NamedTemporaryFile("w") as f:
-        header = list(valid_data[0].keys())
-        writer = csv.writer(f)
-        if has_headers:
-            writer.writerow(header)
-        writer.writerows([[item[col] for col in header] for item in valid_data])
-        f.flush()
-
-        cnames = [f"foo{i}" for i in range(5)]
-        df = daft.read_csv(f.name, has_headers=has_headers, column_names=cnames)
-        assert df.column_names == cnames
-
-        pd_df = df.to_pandas()
-        assert list(pd_df.columns) == cnames
-        assert len(pd_df) == len(valid_data)
-
-
 def test_create_dataframe_csv_generate_headers(valid_data: list[dict[str, float]]) -> None:
     with tempfile.NamedTemporaryFile("w") as f:
         header = list(valid_data[0].keys())
         writer = csv.writer(f)
         writer.writerows([[item[col] for col in header] for item in valid_data])
         f.flush()
 
@@ -451,14 +432,66 @@
         assert df.column_names == COL_NAMES
 
         pd_df = df.to_pandas()
         assert list(pd_df.columns) == COL_NAMES
         assert len(pd_df) == len(valid_data)
 
 
+def test_create_dataframe_csv_specify_schema(valid_data: list[dict[str, float]]) -> None:
+    with tempfile.NamedTemporaryFile("w") as f:
+        header = list(valid_data[0].keys())
+        writer = csv.writer(f, delimiter="\t")
+        writer.writerow(header)
+        writer.writerows([[item[col] for col in header] for item in valid_data])
+        f.flush()
+
+        df = daft.read_csv(
+            f.name,
+            delimiter="\t",
+            schema_hints={
+                "sepal_length": DataType.float32(),
+                "sepal_width": DataType.float32(),
+                "petal_length": DataType.float32(),
+                "petal_width": DataType.float32(),
+                "variety": DataType.string(),
+            },
+        )
+        assert df.column_names == COL_NAMES
+
+        pd_df = df.to_pandas()
+        assert list(pd_df.columns) == COL_NAMES
+        assert len(pd_df) == len(valid_data)
+
+
+def test_create_dataframe_csv_specify_schema_no_headers(valid_data: list[dict[str, float]]) -> None:
+    with tempfile.NamedTemporaryFile("w") as f:
+        header = list(valid_data[0].keys())
+        writer = csv.writer(f, delimiter="\t")
+        writer.writerows([[item[col] for col in header] for item in valid_data])
+        f.flush()
+
+        df = daft.read_csv(
+            f.name,
+            delimiter="\t",
+            schema_hints={
+                "sepal_length": DataType.float64(),
+                "sepal_width": DataType.float64(),
+                "petal_length": DataType.float64(),
+                "petal_width": DataType.float64(),
+                "variety": DataType.string(),
+            },
+            has_headers=False,
+        )
+        assert df.column_names == COL_NAMES
+
+        pd_df = df.to_pandas()
+        assert list(pd_df.columns) == COL_NAMES
+        assert len(pd_df) == len(valid_data)
+
+
 ###
 # JSON tests
 ###
 
 
 def test_create_dataframe_json(valid_data: list[dict[str, float]]) -> None:
     with tempfile.NamedTemporaryFile("w") as f:
@@ -527,14 +560,38 @@
 def test_create_dataframe_json_https() -> None:
     df = daft.read_json("https://github.com/Eventual-Inc/mnist-json/raw/master/mnist_handwritten_test.json.gz")
     df.collect()
     assert set(df.column_names) == {"label", "image"}
     assert len(df) == 10000
 
 
+def test_create_dataframe_json_specify_schema(valid_data: list[dict[str, float]]) -> None:
+    with tempfile.NamedTemporaryFile("w") as f:
+        for data in valid_data:
+            f.write(json.dumps(data))
+            f.write("\n")
+        f.flush()
+
+        df = daft.read_json(
+            f.name,
+            schema_hints={
+                "sepal_length": DataType.float32(),
+                "sepal_width": DataType.float32(),
+                "petal_length": DataType.float32(),
+                "petal_width": DataType.float32(),
+                "variety": DataType.string(),
+            },
+        )
+        assert df.column_names == COL_NAMES
+
+        pd_df = df.to_pandas()
+        assert list(pd_df.columns) == COL_NAMES
+        assert len(pd_df) == len(valid_data)
+
+
 ###
 # Parquet tests
 ###
 
 
 def test_create_dataframe_parquet(valid_data: list[dict[str, float]]) -> None:
     with tempfile.NamedTemporaryFile("w") as f:
@@ -591,7 +648,30 @@
         df = daft.read_parquet(f.name)
         df = df.select(*col_subset)
         assert df.column_names == col_subset
 
         pd_df = df.to_pandas()
         assert list(pd_df.columns) == col_subset
         assert len(pd_df) == len(valid_data)
+
+
+def test_create_dataframe_parquet_specify_schema(valid_data: list[dict[str, float]]) -> None:
+    with tempfile.NamedTemporaryFile("w") as f:
+        table = pa.Table.from_pydict({col: [d[col] for d in valid_data] for col in COL_NAMES})
+        papq.write_table(table, f.name)
+        f.flush()
+
+        df = daft.read_parquet(
+            f.name,
+            schema_hints={
+                "sepal_length": DataType.float32(),
+                "sepal_width": DataType.float32(),
+                "petal_length": DataType.float32(),
+                "petal_width": DataType.float32(),
+                "variety": DataType.string(),
+            },
+        )
+        assert df.column_names == COL_NAMES
+
+        pd_df = df.to_pandas()
+        assert list(pd_df.columns) == COL_NAMES
+        assert len(pd_df) == len(valid_data)
```

### Comparing `getdaft-0.1.5/tests/dataframe/test_distinct.py` & `getdaft-0.1.6/tests/dataframe/test_distinct.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/dataframe/test_explode.py` & `getdaft-0.1.6/tests/dataframe/test_explode.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/dataframe/test_filter.py` & `getdaft-0.1.6/tests/dataframe/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/dataframe/test_getitem.py` & `getdaft-0.1.6/tests/dataframe/test_getitem.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/dataframe/test_joins.py` & `getdaft-0.1.6/tests/dataframe/test_joins.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/dataframe/test_logical_type.py` & `getdaft-0.1.6/tests/dataframe/test_logical_type.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/dataframe/test_select.py` & `getdaft-0.1.6/tests/dataframe/test_select.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/dataframe/test_show.py` & `getdaft-0.1.6/tests/dataframe/test_show.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/dataframe/test_sort.py` & `getdaft-0.1.6/tests/dataframe/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/dataframe/test_to_integrations.py` & `getdaft-0.1.6/tests/dataframe/test_to_integrations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/dataframe/test_with_column.py` & `getdaft-0.1.6/tests/dataframe/test_with_column.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/expressions/test_apply.py` & `getdaft-0.1.6/tests/expressions/test_apply.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/expressions/test_expressions.py` & `getdaft-0.1.6/tests/expressions/test_expressions.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/expressions/test_expressions_projection.py` & `getdaft-0.1.6/tests/expressions/test_expressions_projection.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/expressions/test_udf.py` & `getdaft-0.1.6/tests/expressions/test_udf.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/expressions/typing/conftest.py` & `getdaft-0.1.6/tests/expressions/typing/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/expressions/typing/test_aggs.py` & `getdaft-0.1.6/tests/expressions/typing/test_aggs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/expressions/typing/test_arithmetic.py` & `getdaft-0.1.6/tests/expressions/typing/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/expressions/typing/test_compare.py` & `getdaft-0.1.6/tests/expressions/typing/test_compare.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/expressions/typing/test_dt.py` & `getdaft-0.1.6/tests/expressions/typing/test_dt.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/expressions/typing/test_float.py` & `getdaft-0.1.6/tests/expressions/typing/test_float.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/expressions/typing/test_if_else.py` & `getdaft-0.1.6/tests/expressions/typing/test_if_else.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/expressions/typing/test_logical.py` & `getdaft-0.1.6/tests/expressions/typing/test_logical.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/expressions/typing/test_str.py` & `getdaft-0.1.6/tests/expressions/typing/test_str.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/integration/test_tpch.py` & `getdaft-0.1.6/tests/integration/test_tpch.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,17 +46,22 @@
             fp = chunked_filepath
         except FileNotFoundError:
             fp = nonchunked_filepath
 
         df = daft.read_csv(
             fp,
             has_headers=False,
-            column_names=data_generation.SCHEMA[tbl_name],
             delimiter="|",
         )
+        df = df.select(
+            *[
+                daft.col(autoname).alias(colname)
+                for autoname, colname in zip(df.column_names, data_generation.SCHEMA[tbl_name])
+            ]
+        )
         return df
 
     return _get_df
 
 
 @pytest.fixture(scope="module")
 def check_answer(gen_tpch):
```

### Comparing `getdaft-0.1.5/tests/optimizer/conftest.py` & `getdaft-0.1.6/tests/optimizer/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/optimizer/test_drop_projections.py` & `getdaft-0.1.6/tests/optimizer/test_drop_projections.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/optimizer/test_drop_repartition.py` & `getdaft-0.1.6/tests/optimizer/test_drop_repartition.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/optimizer/test_fold_projections.py` & `getdaft-0.1.6/tests/optimizer/test_fold_projections.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/optimizer/test_prune_columns.py` & `getdaft-0.1.6/tests/optimizer/test_prune_columns.py`

 * *Files 6% similar despite different names*

```diff
@@ -131,14 +131,26 @@
         df.select(*left_selection, "variety")
         .join(df.select(*[s.replace("right.", "") for s in right_selection], "variety"), on="variety")
         .select(*left_selection_final, *right_selection_final, *key_selection_final)
     )
     assert_plan_eq(optimizer(df_unoptimized.plan()), df_optimized.plan())
 
 
+def test_projection_concat_pruning(valid_data, optimizer):
+    df1 = daft.from_pylist(valid_data)
+    df2 = daft.from_pylist(valid_data)
+    concatted = df1.concat(df2)
+
+    selected = concatted.select("sepal_length")
+    optimized = optimizer(selected.plan())
+
+    expected = df1.select(col("sepal_length")).concat(df2.select(col("sepal_length"))).select(col("sepal_length"))
+    assert_plan_eq(optimized, expected.plan())
+
+
 @pytest.mark.parametrize(
     "key_aggregation",
     [pytest.param([], id="KeyAgg:0"), pytest.param([(col("variety").alias("count(variety)"), "count")], id="KeyAgg:1")],
 )
 @pytest.mark.parametrize(
     "left_aggregation",
     [
```

### Comparing `getdaft-0.1.5/tests/optimizer/test_pushdown_clauses_into_scan.py` & `getdaft-0.1.6/tests/optimizer/test_pushdown_clauses_into_scan.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/optimizer/test_pushdown_limit.py` & `getdaft-0.1.6/tests/optimizer/test_pushdown_limit.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/optimizer/test_pushdown_predicates.py` & `getdaft-0.1.6/tests/optimizer/test_pushdown_predicates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import pytest
 
 import daft
 from daft.expressions import ExpressionsProjection, col
 from daft.internal.rule_runner import Once, RuleBatch, RuleRunner
-from daft.logical.logical_plan import Filter, Join, LogicalPlan
+from daft.logical.logical_plan import Concat, Filter, Join, LogicalPlan
 from daft.logical.optimizer import PushDownPredicates
 from tests.optimizer.conftest import assert_plan_eq
 
 
 @pytest.fixture(scope="function")
 def optimizer() -> RuleRunner[LogicalPlan]:
     return RuleRunner(
@@ -194,7 +194,20 @@
         df1.where(col("sepal_length") > 4.8)
         .join(df2.where(col("sepal_width") > 4.8), on="variety")
         .where(((col("sepal_length") > 4.8) | (col("right.sepal_length") > 4.8)).alias("foo"))
     )
     assert isinstance(optimized, Filter)
     assert isinstance(expected.plan(), Filter)
     assert_plan_eq(optimized, expected.plan())
+
+
+def test_filter_concat_predicate_pushdown(valid_data, optimizer) -> None:
+    df1 = daft.from_pylist(valid_data)
+    df2 = daft.from_pylist(valid_data)
+    concatted = df1.concat(df2)
+    filtered = concatted.where(col("sepal_length") > 4.8)
+    optimized = optimizer(filtered.plan())
+
+    expected = df1.where(col("sepal_length") > 4.8).concat(df2.where(col("sepal_length") > 4.8))
+    assert isinstance(optimized, Concat)
+    assert isinstance(expected.plan(), Concat)
+    assert_plan_eq(optimized, expected.plan())
```

### Comparing `getdaft-0.1.5/tests/property_based_testing/strategies.py` & `getdaft-0.1.6/tests/property_based_testing/strategies.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/property_based_testing/test_sort.py` & `getdaft-0.1.6/tests/property_based_testing/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/ray/test_dask.py` & `getdaft-0.1.6/tests/ray/test_dask.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/ray/test_datasets.py` & `getdaft-0.1.6/tests/ray/test_datasets.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import pyarrow as pa
 import pytest
 import ray
 
 import daft
 from daft import DataType
 from daft.context import get_context
-from daft.utils import freeze
 
 RAY_VERSION = tuple(int(s) for s in ray.__version__.split("."))
 
 
 class MyObj:
     def __init__(self, x: int):
         self._x = x
@@ -153,15 +152,16 @@
     if RAY_VERSION < (2, 4, 0):
         if RAY_VERSION >= (2, 2, 0):
             assert ds.dataset_format() == "arrow", "Ray Dataset format should be arrow"
         elif RAY_VERSION >= (2, 0, 0):
             assert ds._dataset_format() == "arrow", "Ray Dataset format should be arrow"
 
     df = daft.from_ray_dataset(ds)
-    out_table = df.to_arrow()
+    # Sort data since partition ordering in Datasets is not deterministic.
+    out_table = df.to_arrow().sort_by("intcol")
     expected_table = add_float(table).cast(
         pa.schema(
             [
                 ("intcol", pa.int64()),
                 ("strcol", pa.large_string()),
                 ("floatcol", pa.float64()),
             ]
@@ -173,32 +173,37 @@
 @pytest.mark.skipif(get_context().runner_config.name != "ray", reason="Needs to run on Ray runner")
 @pytest.mark.parametrize("n_partitions", [1, 2])
 def test_from_ray_dataset_simple(n_partitions: int):
     ds = ray.data.range(8, parallelism=n_partitions)
 
     df = daft.from_ray_dataset(ds)
     # Sort data since partition ordering in Datasets is not deterministic.
-    assert freeze(df.to_pydict()) == freeze({"value": list(range(8))})
+    out = df.to_pydict()
+    assert list(out.keys()) == ["value"]
+    assert sorted(out["value"]) == list(range(8))
 
 
 @pytest.mark.skipif(get_context().runner_config.name != "ray", reason="Needs to run on Ray runner")
 @pytest.mark.parametrize("n_partitions", [1, 2])
 def test_from_ray_dataset_tensor(n_partitions: int):
     ds = ray.data.range(8)
     ds = ds.map(lambda i: {"int": i, "np": np.ones((3, 3))}).repartition(n_partitions)
 
     df = daft.from_ray_dataset(ds)
     out = df.to_pydict()
-    out["np"] = [arr.tolist() for arr in out["np"]]
+    assert out.keys() == {"int", "np"}
+    # Sort data since partition ordering in Datasets is not deterministic.
+    out_sorted_rows = sorted(list(zip(out["int"], out["np"])), key=lambda row: row[0])
+    int_col, np_col = zip(*out_sorted_rows)
+    out_sorted = {"int": int_col, "np": np_col}
     expected = {
         "int": list(range(8)),
         "np": [np.ones((3, 3)) for i in range(8)],
     }
-    expected["np"] = [arr.tolist() for arr in expected["np"]]
-    assert freeze(out) == freeze(expected)
+    np.testing.assert_equal(out_sorted, expected)
 
 
 @pytest.mark.skipif(get_context().runner_config.name != "ray", reason="Needs to run on Ray runner")
 @pytest.mark.parametrize("n_partitions", [1, 2])
 def test_from_ray_dataset_pandas(n_partitions: int):
     def add_float(df: pd.DataFrame) -> pd.DataFrame:
         df["floatcol"] = df["intcol"].astype(float)
```

### Comparing `getdaft-0.1.5/tests/series/test_arithmetic.py` & `getdaft-0.1.6/tests/series/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/series/test_comparisons.py` & `getdaft-0.1.6/tests/series/test_comparisons.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/series/test_concat.py` & `getdaft-0.1.6/tests/series/test_concat.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/series/test_embedding.py` & `getdaft-0.1.6/tests/series/test_embedding.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/series/test_filter.py` & `getdaft-0.1.6/tests/series/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/series/test_float.py` & `getdaft-0.1.6/tests/series/test_float.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/series/test_hash.py` & `getdaft-0.1.6/tests/series/test_hash.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/series/test_if_else.py` & `getdaft-0.1.6/tests/series/test_if_else.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/series/test_numeric_ops.py` & `getdaft-0.1.6/tests/series/test_numeric_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/series/test_series.py` & `getdaft-0.1.6/tests/series/test_series.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/series/test_size_bytes.py` & `getdaft-0.1.6/tests/series/test_size_bytes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/series/test_slice.py` & `getdaft-0.1.6/tests/series/test_slice.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/series/test_sort.py` & `getdaft-0.1.6/tests/series/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/series/test_take.py` & `getdaft-0.1.6/tests/series/test_take.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/series/test_temporal_ops.py` & `getdaft-0.1.6/tests/series/test_temporal_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/series/test_utf8_ops.py` & `getdaft-0.1.6/tests/series/test_utf8_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/table/__init__.py` & `getdaft-0.1.6/tests/table/__init__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/table/test_blackbox_kernels.py` & `getdaft-0.1.6/tests/table/test_blackbox_kernels.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/table/test_concat.py` & `getdaft-0.1.6/tests/table/test_concat.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/table/test_eval.py` & `getdaft-0.1.6/tests/table/test_eval.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/table/test_explodes.py` & `getdaft-0.1.6/tests/table/test_explodes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/table/test_filter.py` & `getdaft-0.1.6/tests/table/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/table/test_from_py.py` & `getdaft-0.1.6/tests/table/test_from_py.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 import pyarrow.compute as pac
 import pytest
 from ray.data.extensions import ArrowTensorArray, ArrowTensorType
 
-from daft import DataType
+from daft import DataType, TimeUnit
 from daft.context import get_context
 from daft.series import Series
 from daft.table import Table
 
 ARROW_VERSION = tuple(int(s) for s in pa.__version__.split(".") if s.isnumeric())
 
 PYTHON_TYPE_ARRAYS = {
@@ -30,31 +30,35 @@
     "null": [None, None],
     # The following types are not natively supported and will be cast to Python object types.
     "tensor": list(np.arange(8).reshape(2, 2, 2)),
     "timestamp": [datetime.datetime.now(), datetime.datetime.now()],
 }
 
 
-INFERRED_TYPES = {
+PYTHON_INFERRED_TYPES = {
     "int": DataType.int64(),
     "float": DataType.float64(),
     "bool": DataType.bool(),
     "str": DataType.string(),
     "binary": DataType.binary(),
     "date": DataType.date(),
     "list": DataType.list("item", DataType.int64()),
     "struct": DataType.struct({"a": DataType.int64(), "b": DataType.float64()}),
     "empty_struct": DataType.struct({"": DataType.null()}),
     "null": DataType.null(),
     # The following types are not natively supported and will be cast to Python object types.
     # TODO(Clark): Change the tensor inferred type to be the canonical fixed-shape tensor extension type.
     "tensor": DataType.python(),
-    "timestamp": DataType.python(),
+    "timestamp": DataType.timestamp(TimeUnit.us()),
 }
 
+PANDAS_INFERRED_TYPES = {
+    **PYTHON_INFERRED_TYPES,
+    "timestamp": DataType.timestamp(TimeUnit.ns()),
+}
 
 ROUNDTRIP_TYPES = {
     "int": pa.int64(),
     "float": pa.float64(),
     "bool": pa.bool_(),
     "str": pa.large_string(),
     "binary": pa.large_binary(),
@@ -140,15 +144,15 @@
 
 
 def test_from_pydict_roundtrip() -> None:
     table = Table.from_pydict(PYTHON_TYPE_ARRAYS)
     assert len(table) == 2
     assert set(table.column_names()) == set(PYTHON_TYPE_ARRAYS.keys())
     for field in table.schema():
-        assert field.dtype == INFERRED_TYPES[field.name]
+        assert field.dtype == PYTHON_INFERRED_TYPES[field.name]
     schema = pa.schema(ROUNDTRIP_TYPES)
     arrs = {}
     for col_name, col in PYTHON_TYPE_ARRAYS.items():
         if col_name == "tensor":
             arrs[col_name] = ArrowTensorArray.from_numpy(col)
         else:
             arrs[col_name] = pa.array(col, type=schema.field(col_name).type)
@@ -181,15 +185,15 @@
 
 def test_from_pandas_roundtrip() -> None:
     df = pd.DataFrame(PYTHON_TYPE_ARRAYS)
     table = Table.from_pandas(df)
     assert len(table) == 2
     assert set(table.column_names()) == set(PYTHON_TYPE_ARRAYS.keys())
     for field in table.schema():
-        assert field.dtype == INFERRED_TYPES[field.name]
+        assert field.dtype == PANDAS_INFERRED_TYPES[field.name]
     # pyarrow --> pandas doesn't preserve the datetime type for the "date" column, so we need to
     # convert it before the comparison.
     df["date"] = pd.to_datetime(df["date"]).astype("datetime64[s]")
     # pyarrow --> pandas will insert explicit Nones within the struct fields.
     df["struct"][1]["a"] = None
     df["empty_struct"][0][""] = None
     df["empty_struct"][1][""] = None
```

### Comparing `getdaft-0.1.5/tests/table/test_head.py` & `getdaft-0.1.6/tests/table/test_head.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/table/test_joins.py` & `getdaft-0.1.6/tests/table/test_joins.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/table/test_partitioning.py` & `getdaft-0.1.6/tests/table/test_partitioning.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/table/test_size_bytes.py` & `getdaft-0.1.6/tests/table/test_size_bytes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/table/test_sorting.py` & `getdaft-0.1.6/tests/table/test_sorting.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/table/test_table_aggs.py` & `getdaft-0.1.6/tests/table/test_table_aggs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/table/test_take.py` & `getdaft-0.1.6/tests/table/test_take.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/table/utf8/test_compares.py` & `getdaft-0.1.6/tests/table/utf8/test_compares.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/test_analytics.py` & `getdaft-0.1.6/tests/test_analytics.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/test_datatypes.py` & `getdaft-0.1.6/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests/test_schema.py` & `getdaft-0.1.6/tests/test_schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,15 +58,22 @@
 def test_schema_to_name_set():
     schema = TABLE.schema()
     assert schema.to_name_set() == set(DATA.keys())
 
 
 def test_repr():
     schema = TABLE.schema()
-    assert repr(schema) == "[('int', Int64), ('float', Float64), ('string', Utf8), ('bool', Boolean)]"
+    assert (
+        repr(schema)
+        == """+-------+---------+--------+---------+
+| int   | float   | string | bool    |
+| Int64 | Float64 | Utf8   | Boolean |
++-------+---------+--------+---------+
+"""
+    )
 
 
 def test_to_col_expr():
     schema = TABLE.schema()
     schema_col_exprs = ExpressionsProjection.from_schema(schema)
     expected_col_exprs = [col(n) for n in schema.column_names()]
```

### Comparing `getdaft-0.1.5/tests/udf_library/test_url_udfs.py` & `getdaft-0.1.6/tests/udf_library/test_url_udfs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tests_legacy/test_resource_requests.py` & `getdaft-0.1.6/tests_legacy/test_resource_requests.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tools/patch_package_version.py` & `getdaft-0.1.6/tools/patch_package_version.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tools/wheels/_vendor/wheel/LICENSE.txt` & `getdaft-0.1.6/tools/wheels/_vendor/wheel/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tools/wheels/_vendor/wheel/cli/__init__.py` & `getdaft-0.1.6/tools/wheels/_vendor/wheel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tools/wheels/_vendor/wheel/cli/convert.py` & `getdaft-0.1.6/tools/wheels/_vendor/wheel/cli/convert.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tools/wheels/_vendor/wheel/cli/pack.py` & `getdaft-0.1.6/tools/wheels/_vendor/wheel/cli/pack.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tools/wheels/_vendor/wheel/cli/unpack.py` & `getdaft-0.1.6/tools/wheels/_vendor/wheel/cli/unpack.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tools/wheels/_vendor/wheel/pkginfo.py` & `getdaft-0.1.6/tools/wheels/_vendor/wheel/pkginfo.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tools/wheels/_vendor/wheel/util.py` & `getdaft-0.1.6/tools/wheels/_vendor/wheel/util.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tools/wheels/_vendor/wheel/wheelfile.py` & `getdaft-0.1.6/tools/wheels/_vendor/wheel/wheelfile.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tools/wheels/fix-and-copy-wheel.py` & `getdaft-0.1.6/tools/wheels/fix-and-copy-wheel.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tools/wheels/tmpdirs.py` & `getdaft-0.1.6/tools/wheels/tmpdirs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tools/wheels/tools.py` & `getdaft-0.1.6/tools/wheels/tools.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tools/wheels/wheeltools.py` & `getdaft-0.1.6/tools/wheels/wheeltools.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb` & `getdaft-0.1.6/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tutorials/image_querying/top_n_red_color.ipynb` & `getdaft-0.1.6/tutorials/image_querying/top_n_red_color.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tutorials/mnist.ipynb` & `getdaft-0.1.6/tutorials/mnist.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tutorials/text_to_image/text_to_image_generation.ipynb` & `getdaft-0.1.6/tutorials/text_to_image/text_to_image_generation.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/tutorials/text_to_image/using_cloud_with_ray.ipynb` & `getdaft-0.1.6/tutorials/text_to_image/using_cloud_with_ray.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.5/Cargo.lock` & `getdaft-0.1.6/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,23 @@
 [[package]]
 name = "android-tzdata"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
 
 [[package]]
+name = "android_system_properties"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "arc-swap"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
 
 [[package]]
 name = "array-init-cursor"
@@ -53,14 +62,15 @@
 version = "0.17.1"
 source = "git+https://github.com/Eventual-Inc/arrow2?branch=clark/expand-casting-support#2ace8097342d5634746915b094c5a3cdf53f75b9"
 dependencies = [
  "ahash",
  "arrow-format",
  "bytemuck",
  "chrono",
+ "chrono-tz",
  "dyn-clone",
  "either",
  "ethnum",
  "foreign_vec",
  "getrandom",
  "hash_hasher",
  "hashbrown 0.13.2",
@@ -75,14 +85,20 @@
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
+name = "base64"
+version = "0.21.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
+
+[[package]]
 name = "bincode"
 version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
 dependencies = [
  "serde",
 ]
@@ -140,24 +156,57 @@
 [[package]]
 name = "chrono"
 version = "0.4.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
 dependencies = [
  "android-tzdata",
+ "iana-time-zone",
+ "js-sys",
  "num-traits",
+ "time",
+ "wasm-bindgen",
+ "winapi",
+]
+
+[[package]]
+name = "chrono-tz"
+version = "0.8.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cf9cc2b23599e6d7479755f3594285efb3f74a1bdca7a7374948bc831e23a552"
+dependencies = [
+ "chrono",
+ "chrono-tz-build",
+ "phf",
+]
+
+[[package]]
+name = "chrono-tz-build"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d9998fb9f7e9b2111641485bf8beb32f92945f97f92a3d061f744cfef335f751"
+dependencies = [
+ "parse-zoneinfo",
+ "phf",
+ "phf_codegen",
 ]
 
 [[package]]
 name = "color_quant"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3d7b894f5411737b7867f4827955924d7c254fc9f4d91a6aad6b097804b1018b"
 
 [[package]]
+name = "core-foundation-sys"
+version = "0.8.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
+
+[[package]]
 name = "crc32fast"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
 dependencies = [
  "cfg-if",
 ]
@@ -181,20 +230,24 @@
 checksum = "2b2466559f260f48ad25fe6317b3c8dac77b5bdb5763ac7d9d6103530663bc90"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "daft"
-version = "0.1.5"
+version = "0.1.6"
 dependencies = [
  "arrow2",
+ "base64",
  "bincode",
+ "chrono",
+ "chrono-tz",
  "dyn-clone",
  "fnv",
+ "html-escape",
  "image",
  "indexmap",
  "lazy_static",
  "log",
  "ndarray",
  "num-derive",
  "num-traits",
@@ -310,15 +363,15 @@
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
- "wasi",
+ "wasi 0.11.0+wasi-snapshot-preview1",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "gif"
 version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -349,14 +402,46 @@
 [[package]]
 name = "hermit-abi"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
 
 [[package]]
+name = "html-escape"
+version = "0.2.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6d1ad449764d627e22bfd7cd5e8868264fc9236e07c752972b4080cd351cb476"
+dependencies = [
+ "utf8-width",
+]
+
+[[package]]
+name = "iana-time-zone"
+version = "0.1.57"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2fad5b825842d2b38bd206f3e81d6957625fd7f0a361e345c30e01a0ae2dd613"
+dependencies = [
+ "android_system_properties",
+ "core-foundation-sys",
+ "iana-time-zone-haiku",
+ "js-sys",
+ "wasm-bindgen",
+ "windows",
+]
+
+[[package]]
+name = "iana-time-zone-haiku"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
+dependencies = [
+ "cc",
+]
+
+[[package]]
 name = "image"
 version = "0.24.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "527909aa81e20ac3a44803521443a765550f09b5130c2c2fa1ea59c2f8f50a3a"
 dependencies = [
  "bytemuck",
  "byteorder",
@@ -520,17 +605,17 @@
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.18"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
 name = "matrixmultiply"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "090126dc04f95dc0d1c1c91f61bdd474b3930ca064c1edc8a849da2c6cbe1e77"
 dependencies = [
@@ -689,14 +774,61 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
+name = "parse-zoneinfo"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c705f256449c60da65e11ff6626e0c16a0a0b96aaa348de61376b249bc340f41"
+dependencies = [
+ "regex",
+]
+
+[[package]]
+name = "phf"
+version = "0.11.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "928c6535de93548188ef63bb7c4036bd415cd8f36ad25af44b9789b2ee72a48c"
+dependencies = [
+ "phf_shared",
+]
+
+[[package]]
+name = "phf_codegen"
+version = "0.11.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a56ac890c5e3ca598bbdeaa99964edb5b0258a583a9eb6ef4e89fc85d9224770"
+dependencies = [
+ "phf_generator",
+ "phf_shared",
+]
+
+[[package]]
+name = "phf_generator"
+version = "0.11.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b1181c94580fa345f50f19d738aaa39c0ed30a600d95cb2d3e23f94266f14fbf"
+dependencies = [
+ "phf_shared",
+ "rand",
+]
+
+[[package]]
+name = "phf_shared"
+version = "0.11.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e1fb5f6f826b772a8d4c0394209441e7d37cbbb967ae9c7e0e8134365c9ee676"
+dependencies = [
+ "siphasher",
+]
+
+[[package]]
 name = "planus"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fc1691dd09e82f428ce8d6310bd6d5da2557c82ff17694d2a32cad7242aea89f"
 dependencies = [
  "array-init-cursor",
 ]
@@ -876,14 +1008,29 @@
 dependencies = [
  "getrandom",
  "redox_syscall",
  "thiserror",
 ]
 
 [[package]]
+name = "regex"
+version = "1.8.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
+dependencies = [
+ "regex-syntax",
+]
+
+[[package]]
+name = "regex-syntax"
+version = "0.7.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
+
+[[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustc_version"
@@ -930,26 +1077,26 @@
 name = "semver"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 
 [[package]]
 name = "serde"
-version = "1.0.163"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
+checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.163"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
+checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.18",
 ]
 
 [[package]]
@@ -972,14 +1119,20 @@
 [[package]]
 name = "simdutf8"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
 
 [[package]]
+name = "siphasher"
+version = "0.3.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7bd3e3206899af3f8b12af284fafc038cc1dc2b41d1b89dd17297221c5d225de"
+
+[[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "static_assertions"
@@ -1066,14 +1219,25 @@
 dependencies = [
  "flate2",
  "jpeg-decoder",
  "weezl",
 ]
 
 [[package]]
+name = "time"
+version = "0.1.45"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1b797afad3f312d1c66a56d11d0316f916356d11bd158fbc6ca6389ff6bf805a"
+dependencies = [
+ "libc",
+ "wasi 0.10.0+wasi-snapshot-preview1",
+ "winapi",
+]
+
+[[package]]
 name = "unicode-ident"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unicode-width"
@@ -1084,21 +1248,33 @@
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
+name = "utf8-width"
+version = "0.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5190c9442dcdaf0ddd50f37420417d219ae5261bbf5db120d0f9bab996c9cba1"
+
+[[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "wasi"
+version = "0.10.0+wasi-snapshot-preview1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a143597ca7c7793eff794def352d41792a93c481eb1042423ff7ff72ba2c31f"
+
+[[package]]
+name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
 version = "0.2.86"
@@ -1178,14 +1354,23 @@
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
+name = "windows"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
+dependencies = [
+ "windows-targets 0.48.0",
+]
+
+[[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
  "windows-targets 0.42.2",
 ]
```

### Comparing `getdaft-0.1.5/PKG-INFO` & `getdaft-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: getdaft
-Version: 0.1.5
+Version: 0.1.6
 Requires-Dist: pyarrow >= 6.0.1
 Requires-Dist: fsspec[http]
 Requires-Dist: loguru
-Requires-Dist: tabulate >= 0.9.0
 Requires-Dist: psutil
 Requires-Dist: typing-extensions >= 4.0.0; python_version < '3.8'
 Requires-Dist: pickle5 >= 0.0.12; python_version < '3.8'
-Requires-Dist: numpy; extra == 'numpy'
 Requires-Dist: s3fs; extra == 'aws'
-Requires-Dist: getdaft[aws, ray, pandas, numpy, viz]; extra == 'all'
-Requires-Dist: pydot; extra == 'viz'
+Requires-Dist: numpy; extra == 'numpy'
 Requires-Dist: pandas; extra == 'pandas'
 Requires-Dist: ray[data, default]>=2.0.0; extra == 'ray'
 Requires-Dist: packaging; extra == 'ray'
-Provides-Extra: numpy
+Requires-Dist: pydot; extra == 'viz'
+Requires-Dist: getdaft[aws, ray, pandas, numpy, viz]; extra == 'all'
 Provides-Extra: aws
-Provides-Extra: all
-Provides-Extra: viz
+Provides-Extra: numpy
 Provides-Extra: pandas
 Provides-Extra: ray
+Provides-Extra: viz
+Provides-Extra: all
 License-File: LICENSE
 Summary: A Distributed DataFrame library for large scale complex data processing.
 Author-email: Eventual Inc <daft@eventualcomputing.com>
 Maintainer-email: Sammy Sidhu <sammy@eventualcomputing.com>, Jay Chia <jay@eventualcomputing.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
 Project-URL: repository, https://github.com/Eventual-Inc/Daft
```

