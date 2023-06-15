# Comparing `tmp/configuraptor-1.5.0.tar.gz` & `tmp/configuraptor-1.5.1.tar.gz`

## Comparing `configuraptor-1.5.0.tar` & `configuraptor-1.5.1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 configuraptor-1.5.0/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.5.0/coverage.svg
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 configuraptor-1.5.0/.github/workflows/su6.yml
--rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.5.0/_static/configuraptor_circle.png
--rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.5.0/_static/configuraptor_original.jpeg
--rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.5.0/_static/configuraptor_round.png
--rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.5.0/_static/configuraptor_transparent.png
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 configuraptor-1.5.0/examples/ages.toml
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 configuraptor-1.5.0/examples/dataclass.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 configuraptor-1.5.0/examples/dumping.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 configuraptor-1.5.0/examples/dumping.yml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.5.0/examples/example_from_readme.json
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 configuraptor-1.5.0/examples/example_from_readme.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 configuraptor-1.5.0/examples/example_from_readme.toml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.5.0/examples/example_from_readme.yaml
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 configuraptor-1.5.0/examples/existing_instance.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 configuraptor-1.5.0/examples/main.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 configuraptor-1.5.0/examples/postponed.py
--rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 configuraptor-1.5.0/examples/readme.md
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 configuraptor-1.5.0/examples/singleton.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.5.0/examples/typedconfig_class.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/d_31a2a1dc9b603870___init___py.html
--rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/d_47560703719c1d9e___about___py.html
--rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/d_47560703719c1d9e___init___py.html
--rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/d_47560703719c1d9e_cls_py.html
--rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/d_47560703719c1d9e_core_py.html
--rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/d_47560703719c1d9e_errors_py.html
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/d_47560703719c1d9e_helpers_py.html
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/d_47560703719c1d9e_main_py.html
--rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/d_47560703719c1d9e_singleton_py.html
--rw-r--r--   0        0        0    13222 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/d_6c7dc8b73849fb97___init___py.html
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/d_6c7dc8b73849fb97__types_py.html
--rw-r--r--   0        0        0     9079 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html
--rw-r--r--   0        0        0     8566 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html
--rw-r--r--   0        0        0    12229 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/d_eb75b6cf8f5eab40___about___py.html
--rw-r--r--   0        0        0    11779 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/d_eb75b6cf8f5eab40___init___py.html
--rw-r--r--   0        0        0    10889 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/d_eb75b6cf8f5eab40_cls_py.html
--rw-r--r--   0        0        0   128799 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/d_eb75b6cf8f5eab40_core_py.html
--rw-r--r--   0        0        0     8854 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/d_eb75b6cf8f5eab40_dump_py.html
--rw-r--r--   0        0        0    21312 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/d_eb75b6cf8f5eab40_errors_py.html
--rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html
--rw-r--r--   0        0        0    12046 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/d_eb75b6cf8f5eab40_postpone_py.html
--rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     8028 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.5.0/htmlcov/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.5.0/pytest_examples/empty.toml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.5.0/pytest_examples/example.json
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configuraptor-1.5.0/pytest_examples/example.toml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.5.0/pytest_examples/example.yaml
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.5.0/pytest_examples/some.toml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.5.0/pytest_examples/with_dict_of_custom.toml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.5.0/pytest_examples/with_multiple_toplevel_keys.toml
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.5.0/src/configuraptor/__about__.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 configuraptor-1.5.0/src/configuraptor/__init__.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 configuraptor-1.5.0/src/configuraptor/cls.py
--rw-r--r--   0        0        0    15378 2020-02-02 00:00:00.000000 configuraptor-1.5.0/src/configuraptor/core.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 configuraptor-1.5.0/src/configuraptor/dump.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 configuraptor-1.5.0/src/configuraptor/errors.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.5.0/src/configuraptor/helpers.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 configuraptor-1.5.0/src/configuraptor/postpone.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.5.0/src/configuraptor/py.typed
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 configuraptor-1.5.0/src/configuraptor/singleton.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 configuraptor-1.5.0/src/configuraptor/loaders/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 configuraptor-1.5.0/src/configuraptor/loaders/_types.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 configuraptor-1.5.0/src/configuraptor/loaders/loaders_310.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 configuraptor-1.5.0/src/configuraptor/loaders/loaders_311.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 configuraptor-1.5.0/src/configuraptor/loaders/loaders_shared.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.5.0/src/configuraptor/loaders/py.typed
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.5.0/tests/__init__.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.5.0/tests/constants.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.5.0/tests/test_about.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 configuraptor-1.5.0/tests/test_core.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 configuraptor-1.5.0/tests/test_dumps.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.5.0/tests/test_json_yaml.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 configuraptor-1.5.0/tests/test_mypy.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 configuraptor-1.5.0/tests/test_postponed.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.5.0/tests/test_singleton.py
--rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 configuraptor-1.5.0/tests/test_toml_basic.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 configuraptor-1.5.0/tests/test_toml_dataclass.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 configuraptor-1.5.0/tests/test_toml_existing.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 configuraptor-1.5.0/tests/test_toml_typedconfig_class.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.5.0/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.5.0/LICENSE.txt
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 configuraptor-1.5.0/README.md
--rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 configuraptor-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 configuraptor-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     5339 2020-02-02 00:00:00.000000 configuraptor-1.5.1/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.5.1/coverage.svg
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 configuraptor-1.5.1/.github/workflows/su6.yml
+-rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.5.1/_static/configuraptor_circle.png
+-rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.5.1/_static/configuraptor_original.jpeg
+-rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.5.1/_static/configuraptor_round.png
+-rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.5.1/_static/configuraptor_transparent.png
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 configuraptor-1.5.1/examples/ages.toml
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 configuraptor-1.5.1/examples/dataclass.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 configuraptor-1.5.1/examples/dumping.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 configuraptor-1.5.1/examples/dumping.yml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.5.1/examples/example_from_readme.json
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 configuraptor-1.5.1/examples/example_from_readme.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 configuraptor-1.5.1/examples/example_from_readme.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.5.1/examples/example_from_readme.yaml
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 configuraptor-1.5.1/examples/existing_instance.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 configuraptor-1.5.1/examples/main.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 configuraptor-1.5.1/examples/postponed.py
+-rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 configuraptor-1.5.1/examples/readme.md
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 configuraptor-1.5.1/examples/singleton.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.5.1/examples/typedconfig_class.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/d_31a2a1dc9b603870___init___py.html
+-rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/d_47560703719c1d9e___about___py.html
+-rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/d_47560703719c1d9e___init___py.html
+-rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/d_47560703719c1d9e_cls_py.html
+-rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/d_47560703719c1d9e_core_py.html
+-rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/d_47560703719c1d9e_errors_py.html
+-rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/d_47560703719c1d9e_helpers_py.html
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/d_47560703719c1d9e_main_py.html
+-rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/d_47560703719c1d9e_singleton_py.html
+-rw-r--r--   0        0        0    13033 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/d_6c7dc8b73849fb97___init___py.html
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/d_6c7dc8b73849fb97__types_py.html
+-rw-r--r--   0        0        0     9079 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html
+-rw-r--r--   0        0        0     8566 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html
+-rw-r--r--   0        0        0    12229 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/d_eb75b6cf8f5eab40___about___py.html
+-rw-r--r--   0        0        0    13155 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/d_eb75b6cf8f5eab40___init___py.html
+-rw-r--r--   0        0        0    10889 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/d_eb75b6cf8f5eab40_cls_py.html
+-rw-r--r--   0        0        0   131223 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/d_eb75b6cf8f5eab40_core_py.html
+-rw-r--r--   0        0        0    22352 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/d_eb75b6cf8f5eab40_dump_py.html
+-rw-r--r--   0        0        0    24080 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/d_eb75b6cf8f5eab40_errors_py.html
+-rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html
+-rw-r--r--   0        0        0    12046 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/d_eb75b6cf8f5eab40_postpone_py.html
+-rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     8035 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     5554 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.5.1/htmlcov/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.5.1/pytest_examples/empty.toml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.5.1/pytest_examples/example.json
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configuraptor-1.5.1/pytest_examples/example.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.5.1/pytest_examples/example.yaml
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.5.1/pytest_examples/some.toml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.5.1/pytest_examples/with_dict_of_custom.toml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.5.1/pytest_examples/with_multiple_toplevel_keys.toml
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.5.1/src/configuraptor/__about__.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 configuraptor-1.5.1/src/configuraptor/__init__.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 configuraptor-1.5.1/src/configuraptor/cls.py
+-rw-r--r--   0        0        0    15538 2020-02-02 00:00:00.000000 configuraptor-1.5.1/src/configuraptor/core.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 configuraptor-1.5.1/src/configuraptor/dump.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 configuraptor-1.5.1/src/configuraptor/errors.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.5.1/src/configuraptor/helpers.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 configuraptor-1.5.1/src/configuraptor/postpone.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.5.1/src/configuraptor/py.typed
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 configuraptor-1.5.1/src/configuraptor/singleton.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 configuraptor-1.5.1/src/configuraptor/loaders/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 configuraptor-1.5.1/src/configuraptor/loaders/_types.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 configuraptor-1.5.1/src/configuraptor/loaders/loaders_310.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 configuraptor-1.5.1/src/configuraptor/loaders/loaders_311.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 configuraptor-1.5.1/src/configuraptor/loaders/loaders_shared.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.5.1/src/configuraptor/loaders/py.typed
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.5.1/tests/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.5.1/tests/constants.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.5.1/tests/test_about.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 configuraptor-1.5.1/tests/test_core.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 configuraptor-1.5.1/tests/test_dumps.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.5.1/tests/test_json_yaml.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 configuraptor-1.5.1/tests/test_mypy.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 configuraptor-1.5.1/tests/test_postponed.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.5.1/tests/test_singleton.py
+-rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 configuraptor-1.5.1/tests/test_toml_basic.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 configuraptor-1.5.1/tests/test_toml_dataclass.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 configuraptor-1.5.1/tests/test_toml_existing.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 configuraptor-1.5.1/tests/test_toml_typedconfig_class.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.5.1/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.5.1/LICENSE.txt
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 configuraptor-1.5.1/README.md
+-rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 configuraptor-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 configuraptor-1.5.1/PKG-INFO
```

### Comparing `configuraptor-1.5.0/CHANGELOG.md` & `configuraptor-1.5.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.5.1 (2023-06-15)
+### Fix
+* **core:** Patch issue with `is_optional` ([`fd4a897`](https://github.com/trialandsuccess/configuraptor/commit/fd4a8972b847ac69eb012041188420a02880e696))
+
 ## v1.5.0 (2023-06-15)
 ### Feature
 * **dumping:** Add methods to dump class instances to dict/toml/yaml/json ([`ea8232b`](https://github.com/trialandsuccess/configuraptor/commit/ea8232b6cf0d152520cbf11278851646eb1e96a9))
 
 ## v1.4.0 (2023-06-15)
 ### Feature
 * **postpone:** Allow marking a field as `postponed` if you can't fill it in right away or from config (useful for cli tools with cli args) ([`1494000`](https://github.com/trialandsuccess/configuraptor/commit/1494000a0f373b83188f892c83e6c1bb5a7ae755))
```

### Comparing `configuraptor-1.5.0/coverage.svg` & `configuraptor-1.5.1/coverage.svg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/_static/configuraptor_circle.png` & `configuraptor-1.5.1/_static/configuraptor_circle.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/_static/configuraptor_original.jpeg` & `configuraptor-1.5.1/_static/configuraptor_original.jpeg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/_static/configuraptor_round.png` & `configuraptor-1.5.1/_static/configuraptor_round.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/_static/configuraptor_transparent.png` & `configuraptor-1.5.1/_static/configuraptor_transparent.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/examples/dataclass.py` & `configuraptor-1.5.1/examples/dataclass.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/examples/dumping.py` & `configuraptor-1.5.1/examples/dumping.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/examples/example_from_readme.py` & `configuraptor-1.5.1/examples/example_from_readme.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/examples/main.py` & `configuraptor-1.5.1/examples/main.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/examples/postponed.py` & `configuraptor-1.5.1/examples/postponed.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/examples/readme.md` & `configuraptor-1.5.1/examples/readme.md`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/examples/singleton.py` & `configuraptor-1.5.1/examples/singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/examples/typedconfig_class.py` & `configuraptor-1.5.1/examples/typedconfig_class.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/htmlcov/coverage_html.js` & `configuraptor-1.5.1/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/htmlcov/d_31a2a1dc9b603870___init___py.html` & `configuraptor-1.5.1/htmlcov/d_31a2a1dc9b603870___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html` & `configuraptor-1.5.1/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html` & `configuraptor-1.5.1/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/htmlcov/d_47560703719c1d9e___about___py.html` & `configuraptor-1.5.1/htmlcov/d_47560703719c1d9e___about___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/htmlcov/d_47560703719c1d9e___init___py.html` & `configuraptor-1.5.1/htmlcov/d_47560703719c1d9e___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/htmlcov/d_47560703719c1d9e_cls_py.html` & `configuraptor-1.5.1/htmlcov/d_47560703719c1d9e_cls_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/htmlcov/d_47560703719c1d9e_core_py.html` & `configuraptor-1.5.1/htmlcov/d_47560703719c1d9e_core_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/htmlcov/d_47560703719c1d9e_errors_py.html` & `configuraptor-1.5.1/htmlcov/d_47560703719c1d9e_errors_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/htmlcov/d_47560703719c1d9e_helpers_py.html` & `configuraptor-1.5.1/htmlcov/d_47560703719c1d9e_helpers_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/htmlcov/d_47560703719c1d9e_main_py.html` & `configuraptor-1.5.1/htmlcov/d_47560703719c1d9e_main_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/htmlcov/d_47560703719c1d9e_singleton_py.html` & `configuraptor-1.5.1/htmlcov/d_47560703719c1d9e_singleton_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/htmlcov/d_6c7dc8b73849fb97___init___py.html` & `configuraptor-1.5.1/htmlcov/d_6c7dc8b73849fb97___init___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">12 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">12<span class="text"> run</span></button>
+            <span class="text">11 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">11<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">1<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_helpers_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97__types_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 14:30 +0200
+            created at 2023-06-15 16:40 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -80,57 +80,56 @@
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Loads loaders based on Python version.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">sys</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">_types</span> <span class="key">import</span> <span class="nam">T_config</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="com"># tomlkit used for every Python version now.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">loaders_shared</span> <span class="key">import</span> <span class="nam">json</span><span class="op">,</span> <span class="nam">yaml</span><span class="op">,</span> <span class="nam">toml</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="com"># if sys.version_info > (3, 11):</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="com">#     from .loaders_311 import toml</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="com"># else:  # pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="com">#     from .loaders_310 import toml</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">_types</span> <span class="key">import</span> <span class="nam">T_config</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="com"># tomlkit used for every Python version now.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">loaders_shared</span> <span class="key">import</span> <span class="nam">json</span><span class="op">,</span> <span class="nam">toml</span><span class="op">,</span> <span class="nam">yaml</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="com"># if sys.version_info > (3, 11):</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="com">#     from .loaders_311 import toml</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="com"># else:  # pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="com">#     from .loaders_310 import toml</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="nam">__all__</span> <span class="op">=</span> <span class="op">[</span><span class="str">"get"</span><span class="op">,</span> <span class="str">"toml"</span><span class="op">,</span> <span class="str">"json"</span><span class="op">,</span> <span class="str">"yaml"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="nam">T_loader</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Callable</span><span class="op">[</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">BinaryIO</span><span class="op">]</span><span class="op">,</span> <span class="nam">T_config</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="nam">LOADERS</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T_loader</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="str">"toml"</span><span class="op">:</span> <span class="nam">toml</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="str">"json"</span><span class="op">:</span> <span class="nam">json</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="str">"yml"</span><span class="op">:</span> <span class="nam">yaml</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="str">"yaml"</span><span class="op">:</span> <span class="nam">yaml</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t"><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="nam">__all__</span> <span class="op">=</span> <span class="op">[</span><span class="str">"get"</span><span class="op">,</span> <span class="str">"toml"</span><span class="op">,</span> <span class="str">"json"</span><span class="op">,</span> <span class="str">"yaml"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="nam">T_loader</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Callable</span><span class="op">[</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">BinaryIO</span><span class="op">]</span><span class="op">,</span> <span class="nam">T_config</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="nam">LOADERS</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T_loader</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="str">"toml"</span><span class="op">:</span> <span class="nam">toml</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="str">"json"</span><span class="op">:</span> <span class="nam">json</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="str">"yml"</span><span class="op">:</span> <span class="nam">yaml</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="str">"yaml"</span><span class="op">:</span> <span class="nam">yaml</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t"><span class="key">def</span> <span class="nam">get</span><span class="op">(</span><span class="nam">extension</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">T_loader</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t"><span class="str">    Get the right loader for a specific extension.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="nam">extension</span> <span class="op">=</span> <span class="nam">extension</span><span class="op">.</span><span class="nam">removeprefix</span><span class="op">(</span><span class="str">"."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="key">if</span> <span class="nam">loader</span> <span class="op">:=</span> <span class="nam">LOADERS</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">extension</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">        <span class="key">return</span> <span class="nam">loader</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">f"Invalid extension {extension}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t"><span class="key">def</span> <span class="nam">get</span><span class="op">(</span><span class="nam">extension</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">T_loader</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="str">    Get the right loader for a specific extension.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="nam">extension</span> <span class="op">=</span> <span class="nam">extension</span><span class="op">.</span><span class="nam">removeprefix</span><span class="op">(</span><span class="str">"."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="key">if</span> <span class="nam">loader</span> <span class="op">:=</span> <span class="nam">LOADERS</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">extension</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">        <span class="key">return</span> <span class="nam">loader</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">f"Invalid extension {extension}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_helpers_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97__types_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 14:30 +0200
+            created at 2023-06-15 16:40 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,54 +5,53 @@
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 12 statements   12 run 0 missing 1 excluded *****
+***** 11 statements   11 run 0 missing 1 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-15 14:30 +0200
+at 2023-06-15 16:40 +0200
 
 
 1""" 
 2Loads loaders based on Python version. 
 3""" 
 4 
-5import sys 
-6import typing 
-7 
-8from ._types import T_config 
-9 
-10# tomlkit used for every Python version now. 
-11from .loaders_shared import json, yaml, toml 
-12 
-13# if sys.version_info > (3, 11): 
-14# from .loaders_311 import toml 
-15# else: # pragma: no cover 
-16# from .loaders_310 import toml 
+5import typing 
+6 
+7from ._types import T_config 
+8 
+9# tomlkit used for every Python version now. 
+10from .loaders_shared import json, toml, yaml 
+11 
+12# if sys.version_info > (3, 11): 
+13# from .loaders_311 import toml 
+14# else: # pragma: no cover 
+15# from .loaders_310 import toml 
+16 
 17 
-18 
-19__all__ = ["get", "toml", "json", "yaml"] 
-20 
-21T_loader = typing.Callable[[typing.BinaryIO], T_config] 
-22 
-23LOADERS: dict[str, T_loader] = { 
-24 "toml": toml, 
-25 "json": json, 
-26 "yml": yaml, 
-27 "yaml": yaml, 
-28} 
+18__all__ = ["get", "toml", "json", "yaml"] 
+19 
+20T_loader = typing.Callable[[typing.BinaryIO], T_config] 
+21 
+22LOADERS: dict[str, T_loader] = { 
+23 "toml": toml, 
+24 "json": json, 
+25 "yml": yaml, 
+26 "yaml": yaml, 
+27} 
+28 
 29 
-30 
-31def get(extension: str) -> T_loader: 
-32 """ 
-33 Get the right loader for a specific extension. 
-34 """ 
-35 extension = extension.removeprefix(".") 
-36 if loader := LOADERS.get(extension): 
-37 return loader 
-38 else: 
-39 raise ValueError(f"Invalid extension {extension}") 
+30def get(extension: str) -> T_loader: 
+31 """ 
+32 Get the right loader for a specific extension. 
+33 """ 
+34 extension = extension.removeprefix(".") 
+35 if loader := LOADERS.get(extension): 
+36 return loader 
+37 else: 
+38 raise ValueError(f"Invalid extension {extension}") 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-15 14:30 +0200
+at 2023-06-15 16:40 +0200
```

### Comparing `configuraptor-1.5.0/htmlcov/d_6c7dc8b73849fb97__types_py.html` & `configuraptor-1.5.1/htmlcov/d_6c7dc8b73849fb97__types_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html` & `configuraptor-1.5.1/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html` & `configuraptor-1.5.1/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html` & `configuraptor-1.5.1/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_311_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_postpone_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 14:30 +0200
+            created at 2023-06-15 16:40 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -83,16 +83,16 @@
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">File loaders that work regardless of Python version.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">json</span> <span class="key">as</span> <span class="nam">json_lib</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">BinaryIO</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">yaml</span> <span class="key">as</span> <span class="nam">yaml_lib</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">tomlkit</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">tomlkit</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">yaml</span> <span class="key">as</span> <span class="nam">yaml_lib</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">_types</span> <span class="key">import</span> <span class="nam">T_config</span><span class="op">,</span> <span class="nam">as_tconfig</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="key">def</span> <span class="nam">json</span><span class="op">(</span><span class="nam">f</span><span class="op">:</span> <span class="nam">BinaryIO</span><span class="op">)</span> <span class="op">-></span> <span class="nam">T_config</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="str">    Load a JSON file.</span>&nbsp;</span><span class="r"></span></p>
@@ -120,13 +120,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_311_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_postpone_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 14:30 +0200
+            created at 2023-06-15 16:40 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,26 +7,26 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 14 statements   14 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-15 14:30 +0200
+at 2023-06-15 16:40 +0200
 
 
 1""" 
 2File loaders that work regardless of Python version. 
 3""" 
 4 
 5import json as json_lib 
 6from typing import BinaryIO 
 7 
-8import yaml as yaml_lib 
-9import tomlkit 
+8import tomlkit 
+9import yaml as yaml_lib 
 10 
 11from ._types import T_config, as_tconfig 
 12 
 13 
 14def json(f: BinaryIO) -> T_config: 
 15 """ 
 16 Load a JSON file. 
@@ -47,8 +47,8 @@
 31 """ 
 32 Load a toml file. 
 33 """ 
 34 data = tomlkit.load(f) 
 35 return as_tconfig(data) 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-15 14:30 +0200
+at 2023-06-15 16:40 +0200
```

### Comparing `configuraptor-1.5.0/htmlcov/d_eb75b6cf8f5eab40___about___py.html` & `configuraptor-1.5.1/htmlcov/d_eb75b6cf8f5eab40___about___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 14:30 +0200
+            created at 2023-06-15 16:40 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -83,23 +83,23 @@
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">This file contains the module version.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="com"># SPDX-FileCopyrightText: 2023-present Robin van der Noord &lt;robinvandernoord@gmail.com></span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="com"># SPDX-License-Identifier: MIT</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"1.4.0"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"1.5.0"</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 14:30 +0200
+            created at 2023-06-15 16:40 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,22 +7,22 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 1 statements   1 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-15 14:30 +0200
+at 2023-06-15 16:40 +0200
 
 
 1""" 
 2This file contains the module version. 
 3""" 
 4 
 5# SPDX-FileCopyrightText: 2023-present Robin van der Noord
 <robinvandernoord@gmail.com> 
 6# 
 7# SPDX-License-Identifier: MIT 
-8__version__ = "1.4.0" 
+8__version__ = "1.5.0" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-15 14:30 +0200
+at 2023-06-15 16:40 +0200
```

### Comparing `configuraptor-1.5.0/htmlcov/d_eb75b6cf8f5eab40___init___py.html` & `configuraptor-1.5.1/htmlcov/d_eb75b6cf8f5eab40___init___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">5 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">5<span class="text"> run</span></button>
+            <span class="text">6 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">6<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40___about___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_cls_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 14:30 +0200
+            created at 2023-06-15 16:40 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -93,42 +93,48 @@
     <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="nam">check_and_convert_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="nam">convert_config</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">    <span class="nam">ensure_types</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">    <span class="nam">load_into</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">    <span class="nam">load_into_class</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">    <span class="nam">load_into_instance</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">postpone</span> <span class="key">import</span> <span class="nam">postpone</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">singleton</span> <span class="key">import</span> <span class="nam">Singleton</span><span class="op">,</span> <span class="nam">SingletonMeta</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="nam">__all__</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">    <span class="com"># cls</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="str">"TypedConfig"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="com"># singleton</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="str">"Singleton"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="str">"SingletonMeta"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="com"># core</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="str">"all_annotations"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="str">"check_and_convert_data"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">    <span class="str">"convert_config"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="str">"ensure_types"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="str">"load_into"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="str">"load_into_class"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="str">"load_into_instance"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="com"># postpone</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="str">"postpone"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t"><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">dump</span> <span class="key">import</span> <span class="nam">asdict</span><span class="op">,</span> <span class="nam">asjson</span><span class="op">,</span> <span class="nam">astoml</span><span class="op">,</span> <span class="nam">asyaml</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">postpone</span> <span class="key">import</span> <span class="nam">postpone</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">singleton</span> <span class="key">import</span> <span class="nam">Singleton</span><span class="op">,</span> <span class="nam">SingletonMeta</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="nam">__all__</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="com"># cls</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="str">"TypedConfig"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="com"># singleton</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="str">"Singleton"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="str">"SingletonMeta"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="com"># core</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="str">"all_annotations"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">    <span class="str">"check_and_convert_data"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="str">"convert_config"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="str">"ensure_types"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="str">"load_into"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="str">"load_into_class"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="str">"load_into_instance"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="com"># postpone</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="str">"postpone"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="com"># dump</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">    <span class="str">"asdict"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">    <span class="str">"astoml"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="str">"asyaml"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="str">"asjson"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t"><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40___about___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_cls_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 14:30 +0200
+            created at 2023-06-15 16:40 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,17 +5,17 @@
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 5 statements   5 run 0 missing 0 excluded *****
+***** 6 statements   6 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-15 14:30 +0200
+at 2023-06-15 16:40 +0200
 
 
 1""" 
 2Exposes TypedConfig and load_into for this library. 
 3""" 
 4 
 5# SPDX-FileCopyrightText: 2023-present Robin van der Noord
@@ -28,30 +28,36 @@
 11 check_and_convert_data, 
 12 convert_config, 
 13 ensure_types, 
 14 load_into, 
 15 load_into_class, 
 16 load_into_instance, 
 17) 
-18from .postpone import postpone 
-19from .singleton import Singleton, SingletonMeta 
-20 
-21__all__ = [ 
-22 # cls 
-23 "TypedConfig", 
-24 # singleton 
-25 "Singleton", 
-26 "SingletonMeta", 
-27 # core 
-28 "all_annotations", 
-29 "check_and_convert_data", 
-30 "convert_config", 
-31 "ensure_types", 
-32 "load_into", 
-33 "load_into_class", 
-34 "load_into_instance", 
-35 # postpone 
-36 "postpone", 
-37] 
+18from .dump import asdict, asjson, astoml, asyaml 
+19from .postpone import postpone 
+20from .singleton import Singleton, SingletonMeta 
+21 
+22__all__ = [ 
+23 # cls 
+24 "TypedConfig", 
+25 # singleton 
+26 "Singleton", 
+27 "SingletonMeta", 
+28 # core 
+29 "all_annotations", 
+30 "check_and_convert_data", 
+31 "convert_config", 
+32 "ensure_types", 
+33 "load_into", 
+34 "load_into_class", 
+35 "load_into_instance", 
+36 # postpone 
+37 "postpone", 
+38 # dump 
+39 "asdict", 
+40 "astoml", 
+41 "asyaml", 
+42 "asjson", 
+43] 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-15 14:30 +0200
+at 2023-06-15 16:40 +0200
```

### Comparing `configuraptor-1.5.0/htmlcov/d_eb75b6cf8f5eab40_cls_py.html` & `configuraptor-1.5.1/htmlcov/d_eb75b6cf8f5eab40_cls_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/htmlcov/d_eb75b6cf8f5eab40_core_py.html` & `configuraptor-1.5.1/htmlcov/d_eb75b6cf8f5eab40_core_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">153 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">153<span class="text"> run</span></button>
+            <span class="text">158 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">158<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">3<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_cls_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_dump_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 14:30 +0200
+            created at 2023-06-15 16:44 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -81,493 +81,504 @@
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Contains most of the loading logic.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">dataclasses</span> <span class="key">as</span> <span class="nam">dc</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">types</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">warnings</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="nam">collections</span> <span class="key">import</span> <span class="nam">ChainMap</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="nam">typeguard</span> <span class="key">import</span> <span class="nam">TypeCheckError</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">from</span> <span class="nam">typeguard</span> <span class="key">import</span> <span class="nam">check_type</span> <span class="key">as</span> <span class="nam">_check_type</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="key">from</span> <span class="op">.</span> <span class="key">import</span> <span class="nam">loaders</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">errors</span> <span class="key">import</span> <span class="nam">ConfigErrorInvalidType</span><span class="op">,</span> <span class="nam">ConfigErrorMissingKey</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">helpers</span> <span class="key">import</span> <span class="nam">camel_to_snake</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">postpone</span> <span class="key">import</span> <span class="nam">Postponed</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="com"># T is a reusable typevar</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="nam">T</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"T"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="com"># t_typelike is anything that can be type hinted</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="nam">T_typelike</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeAlias</span> <span class="op">=</span> <span class="nam">type</span> <span class="op">|</span> <span class="nam">types</span><span class="op">.</span><span class="nam">UnionType</span>  <span class="com"># | typing.Union</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="com"># t_data is anything that can be fed to _load_data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="nam">T_data</span> <span class="op">=</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span> <span class="op">|</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="com"># c = a config class instance, can be any (user-defined) class</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="nam">C</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"C"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t"><span class="com"># type c is a config class</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t"><span class="nam">Type_C</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">math</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">import</span> <span class="nam">types</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">warnings</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="nam">collections</span> <span class="key">import</span> <span class="nam">ChainMap</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">from</span> <span class="nam">typeguard</span> <span class="key">import</span> <span class="nam">TypeCheckError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="key">from</span> <span class="nam">typeguard</span> <span class="key">import</span> <span class="nam">check_type</span> <span class="key">as</span> <span class="nam">_check_type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="key">from</span> <span class="op">.</span> <span class="key">import</span> <span class="nam">loaders</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">errors</span> <span class="key">import</span> <span class="nam">ConfigErrorInvalidType</span><span class="op">,</span> <span class="nam">ConfigErrorMissingKey</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">helpers</span> <span class="key">import</span> <span class="nam">camel_to_snake</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">postpone</span> <span class="key">import</span> <span class="nam">Postponed</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="com"># T is a reusable typevar</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="nam">T</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"T"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="com"># t_typelike is anything that can be type hinted</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="nam">T_typelike</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeAlias</span> <span class="op">=</span> <span class="nam">type</span> <span class="op">|</span> <span class="nam">types</span><span class="op">.</span><span class="nam">UnionType</span>  <span class="com"># | typing.Union</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="com"># t_data is anything that can be fed to _load_data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="nam">T_data</span> <span class="op">=</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">Path</span> <span class="op">|</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="com"># c = a config class instance, can be any (user-defined) class</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t"><span class="nam">C</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"C"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t"><span class="com"># type c is a config class</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t"><span class="nam">Type_C</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="key">def</span> <span class="nam">_data_for_nested_key</span><span class="op">(</span><span class="nam">key</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">raw</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t"><span class="str">    If a key contains a dot, traverse the raw dict until the right key was found.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t"><span class="str">    Example:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t"><span class="str">        key = some.nested.key</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t"><span class="str">        raw = {"some": {"nested": {"key": {"with": "data"}}}}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t"><span class="str">        -> {"with": "data"}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="nam">parts</span> <span class="op">=</span> <span class="nam">key</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="key">while</span> <span class="nam">parts</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">        <span class="nam">raw</span> <span class="op">=</span> <span class="nam">raw</span><span class="op">[</span><span class="nam">parts</span><span class="op">.</span><span class="nam">pop</span><span class="op">(</span><span class="num">0</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="key">return</span> <span class="nam">raw</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t"><span class="key">def</span> <span class="nam">_data_for_nested_key</span><span class="op">(</span><span class="nam">key</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">raw</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t"><span class="str">    If a key contains a dot, traverse the raw dict until the right key was found.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t"><span class="str">    Example:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t"><span class="str">        key = some.nested.key</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t"><span class="str">        raw = {"some": {"nested": {"key": {"with": "data"}}}}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="str">        -> {"with": "data"}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="nam">parts</span> <span class="op">=</span> <span class="nam">key</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="key">while</span> <span class="nam">parts</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">        <span class="nam">raw</span> <span class="op">=</span> <span class="nam">raw</span><span class="op">[</span><span class="nam">parts</span><span class="op">.</span><span class="nam">pop</span><span class="op">(</span><span class="num">0</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">    <span class="key">return</span> <span class="nam">raw</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t"><span class="key">def</span> <span class="nam">_guess_key</span><span class="op">(</span><span class="nam">clsname</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t"><span class="str">    If no key is manually defined for `load_into`, \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t"><span class="str">    the class' name is converted to snake_case to use as the default key.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="key">return</span> <span class="nam">camel_to_snake</span><span class="op">(</span><span class="nam">clsname</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t"><span class="key">def</span> <span class="nam">_guess_key</span><span class="op">(</span><span class="nam">clsname</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t"><span class="str">    If no key is manually defined for `load_into`, \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t"><span class="str">    the class' name is converted to snake_case to use as the default key.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="key">return</span> <span class="nam">camel_to_snake</span><span class="op">(</span><span class="nam">clsname</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t"><span class="key">def</span> <span class="nam">_load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">classname</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t"><span class="str">    Tries to load the right data from a filename/path or dict, based on a manual key or a classname.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t"><span class="str">    E.g. class Tool will be mapped to key tool.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t"><span class="str">    It also deals with nested keys (tool.extra -> {"tool": {"extra": ...}}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">    <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">        <span class="nam">data</span> <span class="op">=</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">    <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">Path</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">        <span class="key">with</span> <span class="nam">data</span><span class="op">.</span><span class="nam">open</span><span class="op">(</span><span class="str">"rb"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">f</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">            <span class="nam">loader</span> <span class="op">=</span> <span class="nam">loaders</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">data</span><span class="op">.</span><span class="nam">suffix</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">            <span class="nam">data</span> <span class="op">=</span> <span class="nam">loader</span><span class="op">(</span><span class="nam">f</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="key">return</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">    <span class="key">if</span> <span class="nam">key</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">        <span class="com"># try to guess key by grabbing the first one or using the class name</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">        <span class="key">if</span> <span class="nam">len</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span> <span class="op">==</span> <span class="num">1</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">            <span class="nam">key</span> <span class="op">=</span> <span class="nam">list</span><span class="op">(</span><span class="nam">data</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">        <span class="key">elif</span> <span class="nam">classname</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">            <span class="nam">key</span> <span class="op">=</span> <span class="nam">_guess_key</span><span class="op">(</span><span class="nam">classname</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">    <span class="key">if</span> <span class="nam">key</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">        <span class="key">return</span> <span class="nam">_data_for_nested_key</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">        <span class="com"># no key found, just return all data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">        <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t"><span class="key">def</span> <span class="nam">_load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">classname</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t"><span class="str">    Tries to load the right data from a filename/path or dict, based on a manual key or a classname.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t"><span class="str">    E.g. class Tool will be mapped to key tool.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t"><span class="str">    It also deals with nested keys (tool.extra -> {"tool": {"extra": ...}}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">    <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">        <span class="nam">data</span> <span class="op">=</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">    <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">Path</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">        <span class="key">with</span> <span class="nam">data</span><span class="op">.</span><span class="nam">open</span><span class="op">(</span><span class="str">"rb"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">f</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">            <span class="nam">loader</span> <span class="op">=</span> <span class="nam">loaders</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">data</span><span class="op">.</span><span class="nam">suffix</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">            <span class="nam">data</span> <span class="op">=</span> <span class="nam">loader</span><span class="op">(</span><span class="nam">f</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">        <span class="key">return</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">    <span class="key">if</span> <span class="nam">key</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">        <span class="com"># try to guess key by grabbing the first one or using the class name</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">        <span class="key">if</span> <span class="nam">len</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span> <span class="op">==</span> <span class="num">1</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">            <span class="nam">key</span> <span class="op">=</span> <span class="nam">list</span><span class="op">(</span><span class="nam">data</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">        <span class="key">elif</span> <span class="nam">classname</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">            <span class="nam">key</span> <span class="op">=</span> <span class="nam">_guess_key</span><span class="op">(</span><span class="nam">classname</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">    <span class="key">if</span> <span class="nam">key</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">        <span class="key">return</span> <span class="nam">_data_for_nested_key</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">        <span class="com"># no key found, just return all data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">        <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t"><span class="key">def</span> <span class="nam">check_type</span><span class="op">(</span><span class="nam">value</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">expected_type</span><span class="op">:</span> <span class="nam">T_typelike</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t"><span class="str">    Given a variable, check if it matches 'expected_type' (which can be a Union, parameterized generic etc.).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t"><span class="str">    Based on typeguard but this returns a boolean instead of returning the value or throwing a TypeCheckError</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">        <span class="nam">_check_type</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">expected_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="key">return</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">    <span class="key">except</span> <span class="nam">TypeCheckError</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">        <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t"><span class="key">def</span> <span class="nam">check_type</span><span class="op">(</span><span class="nam">value</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">expected_type</span><span class="op">:</span> <span class="nam">T_typelike</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t"><span class="str">    Given a variable, check if it matches 'expected_type' (which can be a Union, parameterized generic etc.).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t"><span class="str">    Based on typeguard but this returns a boolean instead of returning the value or throwing a TypeCheckError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="nam">_check_type</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">expected_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">        <span class="key">return</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">    <span class="key">except</span> <span class="nam">TypeCheckError</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">        <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t"><span class="key">def</span> <span class="nam">ensure_types</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">type</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span> <span class="op">|</span> <span class="key">None</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t"><span class="str">    Make sure all values in 'data' are in line with the ones stored in 'annotations'.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t"><span class="str">    If an annotated key in missing from data, it will be filled with None for convenience.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">    <span class="com"># custom object to use instead of None, since typing.Optional can be None!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">    <span class="com"># cast to T to make mypy happy</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">    <span class="nam">notfound</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">T</span><span class="op">,</span> <span class="nam">object</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">    <span class="nam">postponed</span> <span class="op">=</span> <span class="nam">Postponed</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">    <span class="nam">final</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span> <span class="op">|</span> <span class="key">None</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">    <span class="key">for</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">_type</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">        <span class="nam">compare</span> <span class="op">=</span> <span class="nam">data</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">notfound</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">        <span class="key">if</span> <span class="nam">compare</span> <span class="key">is</span> <span class="nam">notfound</span><span class="op">:</span>  <span class="com"># pragma: nocover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">            <span class="nam">warnings</span><span class="op">.</span><span class="nam">warn</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">                <span class="str">"This should not happen since "</span> <span class="str">"`load_recursive` already fills `data` "</span> <span class="str">"based on `annotations`"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">            <span class="com"># skip!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">            <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">        <span class="key">if</span> <span class="nam">compare</span> <span class="key">is</span> <span class="nam">postponed</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">            <span class="com"># don't do anything with this item!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">            <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">check_type</span><span class="op">(</span><span class="nam">compare</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ConfigErrorInvalidType</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">value</span><span class="op">=</span><span class="nam">compare</span><span class="op">,</span> <span class="nam">expected_type</span><span class="op">=</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">        <span class="nam">final</span><span class="op">[</span><span class="nam">key</span><span class="op">]</span> <span class="op">=</span> <span class="nam">compare</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">    <span class="key">return</span> <span class="nam">final</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t"><span class="key">def</span> <span class="nam">ensure_types</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">type</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span> <span class="op">|</span> <span class="key">None</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t"><span class="str">    Make sure all values in 'data' are in line with the ones stored in 'annotations'.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t"><span class="str">    If an annotated key in missing from data, it will be filled with None for convenience.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">    <span class="com"># custom object to use instead of None, since typing.Optional can be None!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">    <span class="com"># cast to T to make mypy happy</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">    <span class="nam">notfound</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">T</span><span class="op">,</span> <span class="nam">object</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">    <span class="nam">postponed</span> <span class="op">=</span> <span class="nam">Postponed</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">    <span class="nam">final</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span> <span class="op">|</span> <span class="key">None</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">    <span class="key">for</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">_type</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">        <span class="nam">compare</span> <span class="op">=</span> <span class="nam">data</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">notfound</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">        <span class="key">if</span> <span class="nam">compare</span> <span class="key">is</span> <span class="nam">notfound</span><span class="op">:</span>  <span class="com"># pragma: nocover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">            <span class="nam">warnings</span><span class="op">.</span><span class="nam">warn</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">                <span class="str">"This should not happen since "</span> <span class="str">"`load_recursive` already fills `data` "</span> <span class="str">"based on `annotations`"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">            <span class="com"># skip!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">            <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">        <span class="key">if</span> <span class="nam">compare</span> <span class="key">is</span> <span class="nam">postponed</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">            <span class="com"># don't do anything with this item!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">            <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">check_type</span><span class="op">(</span><span class="nam">compare</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ConfigErrorInvalidType</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">value</span><span class="op">=</span><span class="nam">compare</span><span class="op">,</span> <span class="nam">expected_type</span><span class="op">=</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">        <span class="nam">final</span><span class="op">[</span><span class="nam">key</span><span class="op">]</span> <span class="op">=</span> <span class="nam">compare</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t"><span class="key">def</span> <span class="nam">convert_config</span><span class="op">(</span><span class="nam">items</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t"><span class="str">    Converts the config dict (from toml) or 'overwrites' dict in two ways.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t"><span class="str">    1. removes any items where the value is None, since in that case the default should be used;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t"><span class="str">    2. replaces '-' and '.' in keys with '_' so it can be mapped to the Config properties.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span><span class="nam">k</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="str">"-"</span><span class="op">,</span> <span class="str">"_"</span><span class="op">)</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="str">"."</span><span class="op">,</span> <span class="str">"_"</span><span class="op">)</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">items</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">v</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t"><span class="nam">Type</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t"><span class="nam">T_Type</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"T_Type"</span><span class="op">,</span> <span class="nam">bound</span><span class="op">=</span><span class="nam">Type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t"><span class="key">def</span> <span class="nam">is_builtin_type</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t"><span class="str">    Returns whether _type is one of the builtin types.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">    <span class="key">return</span> <span class="nam">_type</span><span class="op">.</span><span class="nam">__module__</span> <span class="key">in</span> <span class="op">(</span><span class="str">"__builtin__"</span><span class="op">,</span> <span class="str">"builtins"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t"><span class="com"># def is_builtin_class_instance(obj: typing.Any) -> bool:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t"><span class="com">#     return is_builtin_type(obj.__class__)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t"><span class="key">def</span> <span class="nam">is_from_types_or_typing</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t"><span class="str">    Returns whether _type is one of the stlib typing/types types.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t"><span class="str">    e.g. types.UnionType or typing.Union</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">    <span class="key">return</span> <span class="nam">_type</span><span class="op">.</span><span class="nam">__module__</span> <span class="key">in</span> <span class="op">(</span><span class="str">"types"</span><span class="op">,</span> <span class="str">"typing"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t"><span class="key">def</span> <span class="nam">is_from_other_toml_supported_module</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t"><span class="str">    Besides builtins, toml also supports 'datetime' and 'math' types, \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t"><span class="str">    so this returns whether _type is a type from these stdlib modules.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">    <span class="key">return</span> <span class="nam">_type</span><span class="op">.</span><span class="nam">__module__</span> <span class="key">in</span> <span class="op">(</span><span class="str">"datetime"</span><span class="op">,</span> <span class="str">"math"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t"><span class="key">def</span> <span class="nam">is_parameterized</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t"><span class="str">    Returns whether _type is a parameterized type.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t"><span class="str">    Examples:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t"><span class="str">        list[str] -> True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t"><span class="str">        str -> False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">    <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t"><span class="key">def</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t"><span class="str">    Tries to guess if _type is a builtin or a custom (user-defined) class.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t"><span class="str">    Other logic in this module depends on knowing that.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">    <span class="key">return</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">        <span class="nam">type</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span> <span class="key">is</span> <span class="nam">type</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">        <span class="key">and</span> <span class="key">not</span> <span class="nam">is_builtin_type</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">        <span class="key">and</span> <span class="key">not</span> <span class="nam">is_from_other_toml_supported_module</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">        <span class="key">and</span> <span class="key">not</span> <span class="nam">is_from_types_or_typing</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t"><span class="key">def</span> <span class="nam">is_optional</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span> <span class="op">|</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t"><span class="str">    Tries to guess if _type could be optional.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t"><span class="str">    Examples:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t"><span class="str">        None -> True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t"><span class="str">        NoneType -> True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t"><span class="str">        typing.Union[str, None] -> True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t"><span class="str">        str | None -> True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t"><span class="str">        list[str | None] -> False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t"><span class="str">        list[str] -> False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">    <span class="key">if</span> <span class="nam">_type</span> <span class="key">and</span> <span class="nam">is_parameterized</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span> <span class="key">and</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span> <span class="key">in</span> <span class="op">(</span><span class="nam">dict</span><span class="op">,</span> <span class="nam">list</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">        <span class="com"># e.g. list[str]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">        <span class="com"># will crash issubclass to test it first here</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">        <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">    <span class="key">return</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">        <span class="nam">_type</span> <span class="key">is</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">        <span class="key">or</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">types</span><span class="op">.</span><span class="nam">NoneType</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">        <span class="key">or</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">types</span><span class="op">.</span><span class="nam">NoneType</span><span class="op">,</span> <span class="nam">type</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">)</span>  <span class="com"># no type  # Nonetype</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">        <span class="key">or</span> <span class="nam">type</span><span class="op">(</span><span class="key">None</span><span class="op">)</span> <span class="key">in</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>  <span class="com"># union with Nonetype</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t"><span class="key">def</span> <span class="nam">dataclass_field</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">dc</span><span class="op">.</span><span class="nam">Field</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t"><span class="str">    Get Field info for a dataclass cls.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">    <span class="nam">fields</span> <span class="op">=</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="str">"__dataclass_fields__"</span><span class="op">,</span> <span class="op">{</span><span class="op">}</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">    <span class="key">return</span> <span class="nam">fields</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t"><span class="key">def</span> <span class="nam">load_recursive</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t"><span class="str">    For all annotations (recursively gathered from parents with `all_annotations`), \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t"><span class="str">    try to resolve the tree of annotations.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t"><span class="str">    Uses `load_into_recurse`, not itself directly.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t"><span class="str">    Example:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t"><span class="str">        class First:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t"><span class="str">            key: str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">    <span class="key">return</span> <span class="nam">final</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t"><span class="key">def</span> <span class="nam">convert_config</span><span class="op">(</span><span class="nam">items</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t"><span class="str">    Converts the config dict (from toml) or 'overwrites' dict in two ways.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t"><span class="str">    1. removes any items where the value is None, since in that case the default should be used;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t"><span class="str">    2. replaces '-' and '.' in keys with '_' so it can be mapped to the Config properties.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span><span class="nam">k</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="str">"-"</span><span class="op">,</span> <span class="str">"_"</span><span class="op">)</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="str">"."</span><span class="op">,</span> <span class="str">"_"</span><span class="op">)</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">items</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">v</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t"><span class="nam">Type</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t"><span class="nam">T_Type</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"T_Type"</span><span class="op">,</span> <span class="nam">bound</span><span class="op">=</span><span class="nam">Type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t"><span class="key">def</span> <span class="nam">is_builtin_type</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t"><span class="str">    Returns whether _type is one of the builtin types.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">    <span class="key">return</span> <span class="nam">_type</span><span class="op">.</span><span class="nam">__module__</span> <span class="key">in</span> <span class="op">(</span><span class="str">"__builtin__"</span><span class="op">,</span> <span class="str">"builtins"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t"><span class="com"># def is_builtin_class_instance(obj: typing.Any) -> bool:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t"><span class="com">#     return is_builtin_type(obj.__class__)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t"><span class="key">def</span> <span class="nam">is_from_types_or_typing</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t"><span class="str">    Returns whether _type is one of the stlib typing/types types.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t"><span class="str">    e.g. types.UnionType or typing.Union</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">    <span class="key">return</span> <span class="nam">_type</span><span class="op">.</span><span class="nam">__module__</span> <span class="key">in</span> <span class="op">(</span><span class="str">"types"</span><span class="op">,</span> <span class="str">"typing"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t"><span class="key">def</span> <span class="nam">is_from_other_toml_supported_module</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t"><span class="str">    Besides builtins, toml also supports 'datetime' and 'math' types, \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t"><span class="str">    so this returns whether _type is a type from these stdlib modules.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">    <span class="key">return</span> <span class="nam">_type</span><span class="op">.</span><span class="nam">__module__</span> <span class="key">in</span> <span class="op">(</span><span class="str">"datetime"</span><span class="op">,</span> <span class="str">"math"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t"><span class="key">def</span> <span class="nam">is_parameterized</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t"><span class="str">    Returns whether _type is a parameterized type.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t"><span class="str">    Examples:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t"><span class="str">        list[str] -> True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t"><span class="str">        str -> False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">    <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t"><span class="key">def</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t"><span class="str">    Tries to guess if _type is a builtin or a custom (user-defined) class.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t"><span class="str">    Other logic in this module depends on knowing that.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">    <span class="key">return</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">        <span class="nam">type</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span> <span class="key">is</span> <span class="nam">type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">        <span class="key">and</span> <span class="key">not</span> <span class="nam">is_builtin_type</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">        <span class="key">and</span> <span class="key">not</span> <span class="nam">is_from_other_toml_supported_module</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">        <span class="key">and</span> <span class="key">not</span> <span class="nam">is_from_types_or_typing</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t"><span class="key">def</span> <span class="nam">instance_of_custom_class</span><span class="op">(</span><span class="nam">var</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t"><span class="str">    Calls `is_custom_class` on an instance of a (possibly custom) class.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">    <span class="key">return</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">var</span><span class="op">.</span><span class="nam">__class__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t"><span class="key">def</span> <span class="nam">is_optional</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span> <span class="op">|</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t"><span class="str">    Tries to guess if _type could be optional.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t"><span class="str">    Examples:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t"><span class="str">        None -> True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t"><span class="str">        NoneType -> True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t"><span class="str">        typing.Union[str, None] -> True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t"><span class="str">        str | None -> True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t"><span class="str">        list[str | None] -> False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t"><span class="str">        list[str] -> False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">    <span class="key">if</span> <span class="nam">_type</span> <span class="key">and</span> <span class="nam">is_parameterized</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span> <span class="key">and</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span> <span class="key">in</span> <span class="op">(</span><span class="nam">dict</span><span class="op">,</span> <span class="nam">list</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">        <span class="com"># e.g. list[str]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">        <span class="com"># will crash issubclass to test it first here</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">        <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">    <span class="key">elif</span> <span class="nam">_type</span> <span class="key">is</span> <span class="nam">math</span><span class="op">.</span><span class="nam">nan</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">        <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">    <span class="key">return</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">        <span class="nam">_type</span> <span class="key">is</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">        <span class="key">or</span> <span class="nam">types</span><span class="op">.</span><span class="nam">NoneType</span> <span class="key">in</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>  <span class="com"># union with Nonetype</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">        <span class="key">or</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">types</span><span class="op">.</span><span class="nam">NoneType</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">        <span class="key">or</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">types</span><span class="op">.</span><span class="nam">NoneType</span><span class="op">,</span> <span class="nam">type</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">)</span>  <span class="com"># no type  # Nonetype</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t"><span class="key">def</span> <span class="nam">dataclass_field</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">dc</span><span class="op">.</span><span class="nam">Field</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t"><span class="str">    Get Field info for a dataclass cls.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">    <span class="nam">fields</span> <span class="op">=</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="str">"__dataclass_fields__"</span><span class="op">,</span> <span class="op">{</span><span class="op">}</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">    <span class="key">return</span> <span class="nam">fields</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t"><span class="str">        class Second:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t"><span class="str">            other: First</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t"><span class="str">        # step 1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t"><span class="str">        cls = Second</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t"><span class="str">        data = {"second": {"other": {"key": "anything"}}}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t"><span class="str">        annotations: {"other": First}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t"><span class="str">        # step 1.5</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t"><span class="str">        data = {"other": {"key": "anything"}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t"><span class="str">        annotations: {"other": First}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t"><span class="str">        # step 2</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t"><span class="str">        cls = First</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t"><span class="str">        data = {"key": "anything"}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t"><span class="str">        annotations: {"key": str}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">    <span class="nam">updated</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">    <span class="key">for</span> <span class="nam">_key</span><span class="op">,</span> <span class="nam">_type</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">        <span class="key">if</span> <span class="nam">_key</span> <span class="key">in</span> <span class="nam">data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">            <span class="nam">value</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span> <span class="op">=</span> <span class="nam">data</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span>  <span class="com"># value can change so define it as any instead of T</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">            <span class="key">if</span> <span class="nam">is_parameterized</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">                <span class="nam">origin</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">                <span class="nam">arguments</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">                <span class="key">if</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">list</span> <span class="key">and</span> <span class="nam">arguments</span> <span class="key">and</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arguments</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">                    <span class="nam">subtype</span> <span class="op">=</span> <span class="nam">arguments</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">                    <span class="nam">value</span> <span class="op">=</span> <span class="op">[</span><span class="nam">_load_into_recurse</span><span class="op">(</span><span class="nam">subtype</span><span class="op">,</span> <span class="nam">subvalue</span><span class="op">)</span> <span class="key">for</span> <span class="nam">subvalue</span> <span class="key">in</span> <span class="nam">value</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">                <span class="key">elif</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">dict</span> <span class="key">and</span> <span class="nam">arguments</span> <span class="key">and</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arguments</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">                    <span class="com"># e.g. dict[str, Point]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">                    <span class="nam">subkeytype</span><span class="op">,</span> <span class="nam">subvaluetype</span> <span class="op">=</span> <span class="nam">arguments</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">                    <span class="com"># subkey(type) is not a custom class, so don't try to convert it:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">                    <span class="nam">value</span> <span class="op">=</span> <span class="op">{</span><span class="nam">subkey</span><span class="op">:</span> <span class="nam">_load_into_recurse</span><span class="op">(</span><span class="nam">subvaluetype</span><span class="op">,</span> <span class="nam">subvalue</span><span class="op">)</span> <span class="key">for</span> <span class="nam">subkey</span><span class="op">,</span> <span class="nam">subvalue</span> <span class="key">in</span> <span class="nam">value</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">                <span class="com"># elif origin is dict:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">                <span class="com"># keep data the same</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">                <span class="key">elif</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Union</span> <span class="key">and</span> <span class="nam">arguments</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">                    <span class="key">for</span> <span class="nam">arg</span> <span class="key">in</span> <span class="nam">arguments</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">                        <span class="key">if</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arg</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">                            <span class="nam">value</span> <span class="op">=</span> <span class="nam">_load_into_recurse</span><span class="op">(</span><span class="nam">arg</span><span class="op">,</span> <span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">                        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">                            <span class="com"># print(_type, arg, value)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">                            <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">                <span class="com"># todo: other parameterized/unions/typing.Optional</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">            <span class="key">elif</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">                <span class="com"># type must be C (custom class) at this point</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">                <span class="nam">value</span> <span class="op">=</span> <span class="nam">_load_into_recurse</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">                    <span class="com"># make mypy and pycharm happy by telling it _type is of type C...</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t">                    <span class="com"># actually just passing _type as first arg!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">                    <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">Type_C</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">                    <span class="nam">value</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">        <span class="key">elif</span> <span class="nam">_key</span> <span class="key">in</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">            <span class="com"># property has default, use that instead.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">        <span class="key">elif</span> <span class="nam">is_optional</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">            <span class="com"># type is optional and not found in __dict__ -> default is None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">        <span class="key">elif</span> <span class="nam">dc</span><span class="op">.</span><span class="nam">is_dataclass</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span> <span class="key">and</span> <span class="op">(</span><span class="nam">field</span> <span class="op">:=</span> <span class="nam">dataclass_field</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">_key</span><span class="op">)</span><span class="op">)</span> <span class="key">and</span> <span class="nam">field</span><span class="op">.</span><span class="nam">default_factory</span> <span class="key">is</span> <span class="key">not</span> <span class="nam">dc</span><span class="op">.</span><span class="nam">MISSING</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">            <span class="com"># could have a default factory</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">            <span class="com"># todo: do something with field.default?</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">field</span><span class="op">.</span><span class="nam">default_factory</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">            <span class="com"># todo: exception group?</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ConfigErrorMissingKey</span><span class="op">(</span><span class="nam">_key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">        <span class="nam">updated</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span> <span class="op">=</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">    <span class="key">return</span> <span class="nam">updated</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t"><span class="key">def</span> <span class="nam">_all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">ChainMap</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t"><span class="str">    Returns a dictionary-like ChainMap that includes annotations for all \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t"><span class="str">    attributes defined in cls or inherited from superclasses.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t">    <span class="key">return</span> <span class="nam">ChainMap</span><span class="op">(</span><span class="op">*</span><span class="op">(</span><span class="nam">c</span><span class="op">.</span><span class="nam">__annotations__</span> <span class="key">for</span> <span class="nam">c</span> <span class="key">in</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="str">"__mro__"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span> <span class="key">if</span> <span class="str">"__annotations__"</span> <span class="key">in</span> <span class="nam">c</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t"><span class="key">def</span> <span class="nam">load_recursive</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t"><span class="str">    For all annotations (recursively gathered from parents with `all_annotations`), \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t"><span class="str">    try to resolve the tree of annotations.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t"><span class="str">    Uses `load_into_recurse`, not itself directly.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t"><span class="str">    Example:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t"><span class="str">        class First:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t"><span class="str">            key: str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t"><span class="str">        class Second:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t"><span class="str">            other: First</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t"><span class="str">        # step 1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t"><span class="str">        cls = Second</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t"><span class="str">        data = {"second": {"other": {"key": "anything"}}}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t"><span class="str">        annotations: {"other": First}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t"><span class="str">        # step 1.5</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t"><span class="str">        data = {"other": {"key": "anything"}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t"><span class="str">        annotations: {"other": First}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t"><span class="str">        # step 2</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t"><span class="str">        cls = First</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t"><span class="str">        data = {"key": "anything"}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t"><span class="str">        annotations: {"key": str}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">    <span class="nam">updated</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">    <span class="key">for</span> <span class="nam">_key</span><span class="op">,</span> <span class="nam">_type</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">        <span class="key">if</span> <span class="nam">_key</span> <span class="key">in</span> <span class="nam">data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">            <span class="nam">value</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span> <span class="op">=</span> <span class="nam">data</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span>  <span class="com"># value can change so define it as any instead of T</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">            <span class="key">if</span> <span class="nam">is_parameterized</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">                <span class="nam">origin</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">                <span class="nam">arguments</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">                <span class="key">if</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">list</span> <span class="key">and</span> <span class="nam">arguments</span> <span class="key">and</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arguments</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">                    <span class="nam">subtype</span> <span class="op">=</span> <span class="nam">arguments</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">                    <span class="nam">value</span> <span class="op">=</span> <span class="op">[</span><span class="nam">_load_into_recurse</span><span class="op">(</span><span class="nam">subtype</span><span class="op">,</span> <span class="nam">subvalue</span><span class="op">)</span> <span class="key">for</span> <span class="nam">subvalue</span> <span class="key">in</span> <span class="nam">value</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">                <span class="key">elif</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">dict</span> <span class="key">and</span> <span class="nam">arguments</span> <span class="key">and</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arguments</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">                    <span class="com"># e.g. dict[str, Point]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">                    <span class="nam">subkeytype</span><span class="op">,</span> <span class="nam">subvaluetype</span> <span class="op">=</span> <span class="nam">arguments</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">                    <span class="com"># subkey(type) is not a custom class, so don't try to convert it:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">                    <span class="nam">value</span> <span class="op">=</span> <span class="op">{</span><span class="nam">subkey</span><span class="op">:</span> <span class="nam">_load_into_recurse</span><span class="op">(</span><span class="nam">subvaluetype</span><span class="op">,</span> <span class="nam">subvalue</span><span class="op">)</span> <span class="key">for</span> <span class="nam">subkey</span><span class="op">,</span> <span class="nam">subvalue</span> <span class="key">in</span> <span class="nam">value</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">                <span class="com"># elif origin is dict:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">                <span class="com"># keep data the same</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">                <span class="key">elif</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Union</span> <span class="key">and</span> <span class="nam">arguments</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">                    <span class="key">for</span> <span class="nam">arg</span> <span class="key">in</span> <span class="nam">arguments</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t">                        <span class="key">if</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arg</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">                            <span class="nam">value</span> <span class="op">=</span> <span class="nam">_load_into_recurse</span><span class="op">(</span><span class="nam">arg</span><span class="op">,</span> <span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">                        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">                            <span class="com"># print(_type, arg, value)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">                            <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">                <span class="com"># todo: other parameterized/unions/typing.Optional</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">            <span class="key">elif</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">                <span class="com"># type must be C (custom class) at this point</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">                <span class="nam">value</span> <span class="op">=</span> <span class="nam">_load_into_recurse</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">                    <span class="com"># make mypy and pycharm happy by telling it _type is of type C...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">                    <span class="com"># actually just passing _type as first arg!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">                    <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">Type_C</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">                    <span class="nam">value</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t">        <span class="key">elif</span> <span class="nam">_key</span> <span class="key">in</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">            <span class="com"># property has default, use that instead.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">        <span class="key">elif</span> <span class="nam">is_optional</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">            <span class="com"># type is optional and not found in __dict__ -> default is None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t">        <span class="key">elif</span> <span class="nam">dc</span><span class="op">.</span><span class="nam">is_dataclass</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span> <span class="key">and</span> <span class="op">(</span><span class="nam">field</span> <span class="op">:=</span> <span class="nam">dataclass_field</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">_key</span><span class="op">)</span><span class="op">)</span> <span class="key">and</span> <span class="nam">field</span><span class="op">.</span><span class="nam">default_factory</span> <span class="key">is</span> <span class="key">not</span> <span class="nam">dc</span><span class="op">.</span><span class="nam">MISSING</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t">            <span class="com"># could have a default factory</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t">            <span class="com"># todo: do something with field.default?</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">field</span><span class="op">.</span><span class="nam">default_factory</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ConfigErrorMissingKey</span><span class="op">(</span><span class="nam">_key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t">        <span class="nam">updated</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span> <span class="op">=</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t"><span class="key">def</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">_except</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Iterable</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t"><span class="str">    Wrapper around `_all_annotations` that filters away any keys in _except.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t"><span class="str">    It also flattens the ChainMap to a regular dict.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t">    <span class="key">if</span> <span class="nam">_except</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t">        <span class="nam">_except</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t">    <span class="nam">_all</span> <span class="op">=</span> <span class="nam">_all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">_all</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">k</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">_except</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t"><span class="key">def</span> <span class="nam">check_and_convert_data</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t">    <span class="nam">_except</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Iterable</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t"><span class="str">    Based on class annotations, this prepares the data for `load_into_recurse`.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t"><span class="str">    1. convert config-keys to python compatible config_keys</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t"><span class="str">    2. loads custom class type annotations with the same logic (see also `load_recursive`)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t349" href="#t349">349</a></span><span class="t"><span class="str">    3. ensures the annotated types match the actual types after loading the config file.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t">    <span class="nam">annotations</span> <span class="op">=</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">_except</span><span class="op">=</span><span class="nam">_except</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">convert_config</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">load_recursive</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t">    <span class="key">if</span> <span class="nam">strict</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">ensure_types</span><span class="op">(</span><span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t">    <span class="key">return</span> <span class="nam">updated</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t"><span class="key">def</span> <span class="nam">_all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">ChainMap</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t"><span class="str">    Returns a dictionary-like ChainMap that includes annotations for all \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t"><span class="str">    attributes defined in cls or inherited from superclasses.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t">    <span class="key">return</span> <span class="nam">ChainMap</span><span class="op">(</span><span class="op">*</span><span class="op">(</span><span class="nam">c</span><span class="op">.</span><span class="nam">__annotations__</span> <span class="key">for</span> <span class="nam">c</span> <span class="key">in</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="str">"__mro__"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span> <span class="key">if</span> <span class="str">"__annotations__"</span> <span class="key">in</span> <span class="nam">c</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t"><span class="key">def</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">_except</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Iterable</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t"><span class="str">    Wrapper around `_all_annotations` that filters away any keys in _except.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t"><span class="str">    It also flattens the ChainMap to a regular dict.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t">    <span class="key">if</span> <span class="nam">_except</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t">        <span class="nam">_except</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t">    <span class="nam">_all</span> <span class="op">=</span> <span class="nam">_all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">_all</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">k</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">_except</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t349" href="#t349">349</a></span><span class="t"><span class="key">def</span> <span class="nam">check_and_convert_data</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t">    <span class="nam">_except</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Iterable</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t"><span class="str">    Based on class annotations, this prepares the data for `load_into_recurse`.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t">    <span class="key">return</span> <span class="nam">to_load</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t"><span class="key">def</span> <span class="nam">_load_into_recurse</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t363" href="#t363">363</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t364" href="#t364">364</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t366" href="#t366">366</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t368" href="#t368">368</a></span><span class="t"><span class="str">    Loads an instance of `cls` filled with `data`.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t369" href="#t369">369</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t370" href="#t370">370</a></span><span class="t"><span class="str">    Uses `load_recursive` to load any fillable annotated properties (see that method for an example).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t371" href="#t371">371</a></span><span class="t"><span class="str">    `init` can be used to optionally pass extra __init__ arguments. \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t372" href="#t372">372</a></span><span class="t"><span class="str">        NOTE: This will overwrite a config key with the same name!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t373" href="#t373">373</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t">    <span class="key">if</span> <span class="nam">init</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t">        <span class="nam">init</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t">    <span class="com"># fixme: cls.__init__ can set other keys than the name is in kwargs!!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t">    <span class="key">if</span> <span class="nam">dc</span><span class="op">.</span><span class="nam">is_dataclass</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">check_and_convert_data</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">init</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">|=</span> <span class="nam">init</span>  <span class="com"># add extra init variables (should not happen for a dataclass but whatev)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t383" href="#t383">383</a></span><span class="t">        <span class="com"># ensure mypy inst is an instance of the cls type (and not a fictuous `DataclassInstance`)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t">        <span class="nam">inst</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">C</span><span class="op">,</span> <span class="nam">cls</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t386" href="#t386">386</a></span><span class="t">        <span class="nam">inst</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">(</span><span class="op">**</span><span class="nam">init</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t387" href="#t387">387</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">check_and_convert_data</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t388" href="#t388">388</a></span><span class="t">        <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t"><span class="str">    1. convert config-keys to python compatible config_keys</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t"><span class="str">    2. loads custom class type annotations with the same logic (see also `load_recursive`)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t"><span class="str">    3. ensures the annotated types match the actual types after loading the config file.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t">    <span class="nam">annotations</span> <span class="op">=</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">_except</span><span class="op">=</span><span class="nam">_except</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t363" href="#t363">363</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t364" href="#t364">364</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">convert_config</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">load_recursive</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t366" href="#t366">366</a></span><span class="t">    <span class="key">if</span> <span class="nam">strict</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">ensure_types</span><span class="op">(</span><span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t368" href="#t368">368</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t369" href="#t369">369</a></span><span class="t">    <span class="key">return</span> <span class="nam">to_load</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t370" href="#t370">370</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t371" href="#t371">371</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t372" href="#t372">372</a></span><span class="t"><span class="key">def</span> <span class="nam">_load_into_recurse</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t373" href="#t373">373</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t"><span class="str">    Loads an instance of `cls` filled with `data`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t"><span class="str">    Uses `load_recursive` to load any fillable annotated properties (see that method for an example).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t"><span class="str">    `init` can be used to optionally pass extra __init__ arguments. \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t383" href="#t383">383</a></span><span class="t"><span class="str">        NOTE: This will overwrite a config key with the same name!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t">    <span class="key">if</span> <span class="nam">init</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t386" href="#t386">386</a></span><span class="t">        <span class="nam">init</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t387" href="#t387">387</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t388" href="#t388">388</a></span><span class="t">    <span class="com"># fixme: cls.__init__ can set other keys than the name is in kwargs!!</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t389" href="#t389">389</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t390" href="#t390">390</a></span><span class="t">    <span class="key">return</span> <span class="nam">inst</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t391" href="#t391">391</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t392" href="#t392">392</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t393" href="#t393">393</a></span><span class="t"><span class="key">def</span> <span class="nam">_load_into_instance</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t394" href="#t394">394</a></span><span class="t">    <span class="nam">inst</span><span class="op">:</span> <span class="nam">C</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t395" href="#t395">395</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t396" href="#t396">396</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t397" href="#t397">397</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t398" href="#t398">398</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t399" href="#t399">399</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t400" href="#t400">400</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t401" href="#t401">401</a></span><span class="t"><span class="str">    Similar to `load_into_recurse` but uses an existing instance of a class (so after __init__) \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t402" href="#t402">402</a></span><span class="t"><span class="str">    and thus does not support init.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t390" href="#t390">390</a></span><span class="t">    <span class="key">if</span> <span class="nam">dc</span><span class="op">.</span><span class="nam">is_dataclass</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t391" href="#t391">391</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">check_and_convert_data</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">init</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t392" href="#t392">392</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">|=</span> <span class="nam">init</span>  <span class="com"># add extra init variables (should not happen for a dataclass but whatev)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t393" href="#t393">393</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t394" href="#t394">394</a></span><span class="t">        <span class="com"># ensure mypy inst is an instance of the cls type (and not a fictuous `DataclassInstance`)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t395" href="#t395">395</a></span><span class="t">        <span class="nam">inst</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">C</span><span class="op">,</span> <span class="nam">cls</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t396" href="#t396">396</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t397" href="#t397">397</a></span><span class="t">        <span class="nam">inst</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">(</span><span class="op">**</span><span class="nam">init</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t398" href="#t398">398</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">check_and_convert_data</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t399" href="#t399">399</a></span><span class="t">        <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t400" href="#t400">400</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t401" href="#t401">401</a></span><span class="t">    <span class="key">return</span> <span class="nam">inst</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t402" href="#t402">402</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t403" href="#t403">403</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t404" href="#t404">404</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t405" href="#t405">405</a></span><span class="t">    <span class="key">if</span> <span class="nam">init</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t406" href="#t406">406</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Can not init an existing instance!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t407" href="#t407">407</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t408" href="#t408">408</a></span><span class="t">    <span class="nam">existing_data</span> <span class="op">=</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t409" href="#t409">409</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t410" href="#t410">410</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">check_and_convert_data</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">_except</span><span class="op">=</span><span class="nam">existing_data</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t411" href="#t411">411</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t412" href="#t412">412</a></span><span class="t">    <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t413" href="#t413">413</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t414" href="#t414">414</a></span><span class="t">    <span class="key">return</span> <span class="nam">inst</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t415" href="#t415">415</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t416" href="#t416">416</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t417" href="#t417">417</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_class</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t418" href="#t418">418</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t419" href="#t419">419</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t420" href="#t420">420</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t421" href="#t421">421</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t422" href="#t422">422</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t423" href="#t423">423</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t424" href="#t424">424</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t425" href="#t425">425</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t426" href="#t426">426</a></span><span class="t"><span class="str">    Shortcut for _load_data + load_into_recurse.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t427" href="#t427">427</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t428" href="#t428">428</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t429" href="#t429">429</a></span><span class="t">    <span class="key">return</span> <span class="nam">_load_into_recurse</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t430" href="#t430">430</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t431" href="#t431">431</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t432" href="#t432">432</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_instance</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t433" href="#t433">433</a></span><span class="t">    <span class="nam">inst</span><span class="op">:</span> <span class="nam">C</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t434" href="#t434">434</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t435" href="#t435">435</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t436" href="#t436">436</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t437" href="#t437">437</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t438" href="#t438">438</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t439" href="#t439">439</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t440" href="#t440">440</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t441" href="#t441">441</a></span><span class="t"><span class="str">    Shortcut for _load_data + load_into_existing.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t442" href="#t442">442</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t443" href="#t443">443</a></span><span class="t">    <span class="nam">cls</span> <span class="op">=</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__class__</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t444" href="#t444">444</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t445" href="#t445">445</a></span><span class="t">    <span class="key">return</span> <span class="nam">_load_into_instance</span><span class="op">(</span><span class="nam">inst</span><span class="op">,</span> <span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t446" href="#t446">446</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t447" href="#t447">447</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t448" href="#t448">448</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t449" href="#t449">449</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t450" href="#t450">450</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t451" href="#t451">451</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t452" href="#t452">452</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t453" href="#t453">453</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t454" href="#t454">454</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t455" href="#t455">455</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t456" href="#t456">456</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t457" href="#t457">457</a></span><span class="t"><span class="str">    Load your config into a class (instance).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t404" href="#t404">404</a></span><span class="t"><span class="key">def</span> <span class="nam">_load_into_instance</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t405" href="#t405">405</a></span><span class="t">    <span class="nam">inst</span><span class="op">:</span> <span class="nam">C</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t406" href="#t406">406</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t407" href="#t407">407</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t408" href="#t408">408</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t409" href="#t409">409</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t410" href="#t410">410</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t411" href="#t411">411</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t412" href="#t412">412</a></span><span class="t"><span class="str">    Similar to `load_into_recurse` but uses an existing instance of a class (so after __init__) \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t413" href="#t413">413</a></span><span class="t"><span class="str">    and thus does not support init.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t414" href="#t414">414</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t415" href="#t415">415</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t416" href="#t416">416</a></span><span class="t">    <span class="key">if</span> <span class="nam">init</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t417" href="#t417">417</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Can not init an existing instance!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t418" href="#t418">418</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t419" href="#t419">419</a></span><span class="t">    <span class="nam">existing_data</span> <span class="op">=</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t420" href="#t420">420</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t421" href="#t421">421</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">check_and_convert_data</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">_except</span><span class="op">=</span><span class="nam">existing_data</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t422" href="#t422">422</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t423" href="#t423">423</a></span><span class="t">    <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t424" href="#t424">424</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t425" href="#t425">425</a></span><span class="t">    <span class="key">return</span> <span class="nam">inst</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t426" href="#t426">426</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t427" href="#t427">427</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t428" href="#t428">428</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_class</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t429" href="#t429">429</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t430" href="#t430">430</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t431" href="#t431">431</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t432" href="#t432">432</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t433" href="#t433">433</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t434" href="#t434">434</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t435" href="#t435">435</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t436" href="#t436">436</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t437" href="#t437">437</a></span><span class="t"><span class="str">    Shortcut for _load_data + load_into_recurse.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t438" href="#t438">438</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t439" href="#t439">439</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t440" href="#t440">440</a></span><span class="t">    <span class="key">return</span> <span class="nam">_load_into_recurse</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t441" href="#t441">441</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t442" href="#t442">442</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t443" href="#t443">443</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_instance</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t444" href="#t444">444</a></span><span class="t">    <span class="nam">inst</span><span class="op">:</span> <span class="nam">C</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t445" href="#t445">445</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t446" href="#t446">446</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t447" href="#t447">447</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t448" href="#t448">448</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t449" href="#t449">449</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t450" href="#t450">450</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t451" href="#t451">451</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t452" href="#t452">452</a></span><span class="t"><span class="str">    Shortcut for _load_data + load_into_existing.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t453" href="#t453">453</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t454" href="#t454">454</a></span><span class="t">    <span class="nam">cls</span> <span class="op">=</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__class__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t455" href="#t455">455</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t456" href="#t456">456</a></span><span class="t">    <span class="key">return</span> <span class="nam">_load_into_instance</span><span class="op">(</span><span class="nam">inst</span><span class="op">,</span> <span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t457" href="#t457">457</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t458" href="#t458">458</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t459" href="#t459">459</a></span><span class="t"><span class="str">    Supports both a class or an instance as first argument, but that's hard to explain to mypy, so officially only</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t460" href="#t460">460</a></span><span class="t"><span class="str">    classes are supported, and if you want to `load_into` an instance, you should use `load_into_instance`.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t461" href="#t461">461</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t462" href="#t462">462</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t463" href="#t463">463</a></span><span class="t"><span class="str">        cls: either a class or an existing instance of that class.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t464" href="#t464">464</a></span><span class="t"><span class="str">        data: can be a dictionary or a path to a file to load (as pathlib.Path or str)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t465" href="#t465">465</a></span><span class="t"><span class="str">        key: optional (nested) dictionary key to load data from (e.g. 'tool.su6.specific')</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t466" href="#t466">466</a></span><span class="t"><span class="str">        init: optional data to pass to your cls' __init__ method (only if cls is not an instance already)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t467" href="#t467">467</a></span><span class="t"><span class="str">        strict: enable type checks or allow anything?</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t468" href="#t468">468</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t469" href="#t469">469</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t470" href="#t470">470</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t471" href="#t471">471</a></span><span class="t">        <span class="com"># would not be supported according to mypy, but you can still load_into(instance)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t472" href="#t472">472</a></span><span class="t">        <span class="key">return</span> <span class="nam">load_into_instance</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t473" href="#t473">473</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t474" href="#t474">474</a></span><span class="t">    <span class="com"># make mypy and pycharm happy by telling it cls is of type C and not just 'type'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t475" href="#t475">475</a></span><span class="t">    <span class="com"># _cls = typing.cast(typing.Type[C], cls)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t476" href="#t476">476</a></span><span class="t">    <span class="key">return</span> <span class="nam">load_into_class</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t459" href="#t459">459</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t460" href="#t460">460</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t461" href="#t461">461</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t462" href="#t462">462</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t463" href="#t463">463</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t464" href="#t464">464</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t465" href="#t465">465</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t466" href="#t466">466</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t467" href="#t467">467</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t468" href="#t468">468</a></span><span class="t"><span class="str">    Load your config into a class (instance).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t469" href="#t469">469</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t470" href="#t470">470</a></span><span class="t"><span class="str">    Supports both a class or an instance as first argument, but that's hard to explain to mypy, so officially only</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t471" href="#t471">471</a></span><span class="t"><span class="str">    classes are supported, and if you want to `load_into` an instance, you should use `load_into_instance`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t472" href="#t472">472</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t473" href="#t473">473</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t474" href="#t474">474</a></span><span class="t"><span class="str">        cls: either a class or an existing instance of that class.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t475" href="#t475">475</a></span><span class="t"><span class="str">        data: can be a dictionary or a path to a file to load (as pathlib.Path or str)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t476" href="#t476">476</a></span><span class="t"><span class="str">        key: optional (nested) dictionary key to load data from (e.g. 'tool.su6.specific')</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t477" href="#t477">477</a></span><span class="t"><span class="str">        init: optional data to pass to your cls' __init__ method (only if cls is not an instance already)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t478" href="#t478">478</a></span><span class="t"><span class="str">        strict: enable type checks or allow anything?</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t479" href="#t479">479</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t480" href="#t480">480</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t481" href="#t481">481</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t482" href="#t482">482</a></span><span class="t">        <span class="com"># would not be supported according to mypy, but you can still load_into(instance)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t483" href="#t483">483</a></span><span class="t">        <span class="key">return</span> <span class="nam">load_into_instance</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t484" href="#t484">484</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t485" href="#t485">485</a></span><span class="t">    <span class="com"># make mypy and pycharm happy by telling it cls is of type C and not just 'type'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t486" href="#t486">486</a></span><span class="t">    <span class="com"># _cls = typing.cast(typing.Type[C], cls)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t487" href="#t487">487</a></span><span class="t">    <span class="key">return</span> <span class="nam">load_into_class</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_cls_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_dump_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 14:30 +0200
+            created at 2023-06-15 16:44 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,529 +5,540 @@
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 153 statements   153 run 0 missing 3 excluded *****
+***** 158 statements   158 run 0 missing 3 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-15 14:30 +0200
+at 2023-06-15 16:44 +0200
 
 
 1""" 
 2Contains most of the loading logic. 
 3""" 
 4 
 5import dataclasses as dc 
-6import types 
-7import typing 
-8import warnings 
-9from collections import ChainMap 
-10from pathlib import Path 
-11 
-12from typeguard import TypeCheckError 
-13from typeguard import check_type as _check_type 
-14 
-15from . import loaders 
-16from .errors import ConfigErrorInvalidType, ConfigErrorMissingKey 
-17from .helpers import camel_to_snake 
-18from .postpone import Postponed 
-19 
-20# T is a reusable typevar 
-21T = typing.TypeVar("T") 
-22# t_typelike is anything that can be type hinted 
-23T_typelike: typing.TypeAlias = type | types.UnionType # | typing.Union 
-24# t_data is anything that can be fed to _load_data 
-25T_data = str | Path | dict[str, typing.Any] 
-26# c = a config class instance, can be any (user-defined) class 
-27C = typing.TypeVar("C") 
-28# type c is a config class 
-29Type_C = typing.Type[C] 
-30 
+6import math 
+7import types 
+8import typing 
+9import warnings 
+10from collections import ChainMap 
+11from pathlib import Path 
+12 
+13from typeguard import TypeCheckError 
+14from typeguard import check_type as _check_type 
+15 
+16from . import loaders 
+17from .errors import ConfigErrorInvalidType, ConfigErrorMissingKey 
+18from .helpers import camel_to_snake 
+19from .postpone import Postponed 
+20 
+21# T is a reusable typevar 
+22T = typing.TypeVar("T") 
+23# t_typelike is anything that can be type hinted 
+24T_typelike: typing.TypeAlias = type | types.UnionType # | typing.Union 
+25# t_data is anything that can be fed to _load_data 
+26T_data = str | Path | dict[str, typing.Any] 
+27# c = a config class instance, can be any (user-defined) class 
+28C = typing.TypeVar("C") 
+29# type c is a config class 
+30Type_C = typing.Type[C] 
 31 
-32def _data_for_nested_key(key: str, raw: dict[str, typing.Any]) -> dict[str,
+32 
+33def _data_for_nested_key(key: str, raw: dict[str, typing.Any]) -> dict[str,
 typing.Any]: 
-33 """ 
-34 If a key contains a dot, traverse the raw dict until the right key was
+34 """ 
+35 If a key contains a dot, traverse the raw dict until the right key was
 found. 
-35 
-36 Example: 
-37 key = some.nested.key 
-38 raw = {"some": {"nested": {"key": {"with": "data"}}}} 
-39 -> {"with": "data"} 
-40 """ 
-41 parts = key.split(".") 
-42 while parts: 
-43 raw = raw[parts.pop(0)] 
-44 
-45 return raw 
-46 
+36 
+37 Example: 
+38 key = some.nested.key 
+39 raw = {"some": {"nested": {"key": {"with": "data"}}}} 
+40 -> {"with": "data"} 
+41 """ 
+42 parts = key.split(".") 
+43 while parts: 
+44 raw = raw[parts.pop(0)] 
+45 
+46 return raw 
 47 
-48def _guess_key(clsname: str) -> str: 
-49 """ 
-50 If no key is manually defined for `load_into`, \ 
-51 the class' name is converted to snake_case to use as the default key. 
-52 """ 
-53 return camel_to_snake(clsname) 
-54 
+48 
+49def _guess_key(clsname: str) -> str: 
+50 """ 
+51 If no key is manually defined for `load_into`, \ 
+52 the class' name is converted to snake_case to use as the default key. 
+53 """ 
+54 return camel_to_snake(clsname) 
 55 
-56def _load_data(data: T_data, key: str = None, classname: str = None) -> dict
+56 
+57def _load_data(data: T_data, key: str = None, classname: str = None) -> dict
 [str, typing.Any]: 
-57 """ 
-58 Tries to load the right data from a filename/path or dict, based on a manual
+58 """ 
+59 Tries to load the right data from a filename/path or dict, based on a manual
 key or a classname. 
-59 
-60 E.g. class Tool will be mapped to key tool. 
-61 It also deals with nested keys (tool.extra -> {"tool": {"extra": ...}} 
-62 """ 
-63 if isinstance(data, str): 
-64 data = Path(data) 
-65 if isinstance(data, Path): 
-66 with data.open("rb") as f: 
-67 loader = loaders.get(data.suffix) 
-68 data = loader(f) 
-69 
-70 if not data: 
-71 return {} 
-72 
-73 if key is None: 
-74 # try to guess key by grabbing the first one or using the class name 
-75 if len(data) == 1: 
-76 key = list(data.keys())[0] 
-77 elif classname is not None: 
-78 key = _guess_key(classname) 
-79 
-80 if key: 
-81 return _data_for_nested_key(key, data) 
-82 else: 
-83 # no key found, just return all data 
-84 return data 
-85 
+60 
+61 E.g. class Tool will be mapped to key tool. 
+62 It also deals with nested keys (tool.extra -> {"tool": {"extra": ...}} 
+63 """ 
+64 if isinstance(data, str): 
+65 data = Path(data) 
+66 if isinstance(data, Path): 
+67 with data.open("rb") as f: 
+68 loader = loaders.get(data.suffix) 
+69 data = loader(f) 
+70 
+71 if not data: 
+72 return {} 
+73 
+74 if key is None: 
+75 # try to guess key by grabbing the first one or using the class name 
+76 if len(data) == 1: 
+77 key = list(data.keys())[0] 
+78 elif classname is not None: 
+79 key = _guess_key(classname) 
+80 
+81 if key: 
+82 return _data_for_nested_key(key, data) 
+83 else: 
+84 # no key found, just return all data 
+85 return data 
 86 
-87def check_type(value: typing.Any, expected_type: T_typelike) -> bool: 
-88 """ 
-89 Given a variable, check if it matches 'expected_type' (which can be a Union,
+87 
+88def check_type(value: typing.Any, expected_type: T_typelike) -> bool: 
+89 """ 
+90 Given a variable, check if it matches 'expected_type' (which can be a Union,
 parameterized generic etc.). 
-90 
-91 Based on typeguard but this returns a boolean instead of returning the value
+91 
+92 Based on typeguard but this returns a boolean instead of returning the value
 or throwing a TypeCheckError 
-92 """ 
-93 try: 
-94 _check_type(value, expected_type) 
-95 return True 
-96 except TypeCheckError: 
-97 return False 
-98 
+93 """ 
+94 try: 
+95 _check_type(value, expected_type) 
+96 return True 
+97 except TypeCheckError: 
+98 return False 
 99 
-100def ensure_types(data: dict[str, T], annotations: dict[str, type]) -> dict
+100 
+101def ensure_types(data: dict[str, T], annotations: dict[str, type]) -> dict
 [str, T | None]: 
-101 """ 
-102 Make sure all values in 'data' are in line with the ones stored in
+102 """ 
+103 Make sure all values in 'data' are in line with the ones stored in
 'annotations'. 
-103 
-104 If an annotated key in missing from data, it will be filled with None for
+104 
+105 If an annotated key in missing from data, it will be filled with None for
 convenience. 
-105 """ 
-106 # custom object to use instead of None, since typing.Optional can be None! 
-107 # cast to T to make mypy happy 
-108 notfound = typing.cast(T, object()) 
-109 postponed = Postponed() 
-110 
-111 final: dict[str, T | None] = {} 
-112 for key, _type in annotations.items(): 
-113 compare = data.get(key, notfound) 
-114 if compare is notfound: # pragma: nocover 
-115 warnings.warn( 
-116 "This should not happen since " "`load_recursive` already fills `data` "
+106 """ 
+107 # custom object to use instead of None, since typing.Optional can be None! 
+108 # cast to T to make mypy happy 
+109 notfound = typing.cast(T, object()) 
+110 postponed = Postponed() 
+111 
+112 final: dict[str, T | None] = {} 
+113 for key, _type in annotations.items(): 
+114 compare = data.get(key, notfound) 
+115 if compare is notfound: # pragma: nocover 
+116 warnings.warn( 
+117 "This should not happen since " "`load_recursive` already fills `data` "
 "based on `annotations`" 
-117 ) 
-118 # skip! 
-119 continue 
-120 
-121 if compare is postponed: 
-122 # don't do anything with this item! 
-123 continue 
-124 
-125 if not check_type(compare, _type): 
-126 raise ConfigErrorInvalidType(key, value=compare, expected_type=_type) 
-127 
-128 final[key] = compare 
-129 return final 
+118 ) 
+119 # skip! 
+120 continue 
+121 
+122 if compare is postponed: 
+123 # don't do anything with this item! 
+124 continue 
+125 
+126 if not check_type(compare, _type): 
+127 raise ConfigErrorInvalidType(key, value=compare, expected_type=_type) 
+128 
+129 final[key] = compare 
 130 
-131 
-132def convert_config(items: dict[str, T]) -> dict[str, T]: 
-133 """ 
-134 Converts the config dict (from toml) or 'overwrites' dict in two ways. 
-135 
-136 1. removes any items where the value is None, since in that case the
+131 return final 
+132 
+133 
+134def convert_config(items: dict[str, T]) -> dict[str, T]: 
+135 """ 
+136 Converts the config dict (from toml) or 'overwrites' dict in two ways. 
+137 
+138 1. removes any items where the value is None, since in that case the
 default should be used; 
-137 2. replaces '-' and '.' in keys with '_' so it can be mapped to the Config
+139 2. replaces '-' and '.' in keys with '_' so it can be mapped to the Config
 properties. 
-138 """ 
-139 return {k.replace("-", "_").replace(".", "_"): v for k, v in items.items()
+140 """ 
+141 return {k.replace("-", "_").replace(".", "_"): v for k, v in items.items()
 if v is not None} 
-140 
-141 
-142Type = typing.Type[typing.Any] 
-143T_Type = typing.TypeVar("T_Type", bound=Type) 
-144 
-145 
-146def is_builtin_type(_type: Type) -> bool: 
-147 """ 
-148 Returns whether _type is one of the builtin types. 
+142 
+143 
+144Type = typing.Type[typing.Any] 
+145T_Type = typing.TypeVar("T_Type", bound=Type) 
+146 
+147 
+148def is_builtin_type(_type: Type) -> bool: 
 149 """ 
-150 return _type.__module__ in ("__builtin__", "builtins") 
-151 
-152 
-153# def is_builtin_class_instance(obj: typing.Any) -> bool: 
-154# return is_builtin_type(obj.__class__) 
-155 
-156 
-157def is_from_types_or_typing(_type: Type) -> bool: 
-158 """ 
-159 Returns whether _type is one of the stlib typing/types types. 
-160 
-161 e.g. types.UnionType or typing.Union 
-162 """ 
-163 return _type.__module__ in ("types", "typing") 
-164 
-165 
-166def is_from_other_toml_supported_module(_type: Type) -> bool: 
-167 """ 
-168 Besides builtins, toml also supports 'datetime' and 'math' types, \ 
-169 so this returns whether _type is a type from these stdlib modules. 
-170 """ 
-171 return _type.__module__ in ("datetime", "math") 
-172 
-173 
-174def is_parameterized(_type: Type) -> bool: 
-175 """ 
-176 Returns whether _type is a parameterized type. 
-177 
-178 Examples: 
-179 list[str] -> True 
-180 str -> False 
-181 """ 
-182 return typing.get_origin(_type) is not None 
-183 
-184 
-185def is_custom_class(_type: Type) -> bool: 
-186 """ 
-187 Tries to guess if _type is a builtin or a custom (user-defined) class. 
-188 
-189 Other logic in this module depends on knowing that. 
-190 """ 
-191 return ( 
-192 type(_type) is type 
-193 and not is_builtin_type(_type) 
-194 and not is_from_other_toml_supported_module(_type) 
-195 and not is_from_types_or_typing(_type) 
-196 ) 
-197 
-198 
-199def is_optional(_type: Type | None) -> bool: 
-200 """ 
-201 Tries to guess if _type could be optional. 
-202 
-203 Examples: 
-204 None -> True 
-205 NoneType -> True 
-206 typing.Union[str, None] -> True 
-207 str | None -> True 
-208 list[str | None] -> False 
-209 list[str] -> False 
-210 """ 
-211 if _type and is_parameterized(_type) and typing.get_origin(_type) in (dict,
+150 Returns whether _type is one of the builtin types. 
+151 """ 
+152 return _type.__module__ in ("__builtin__", "builtins") 
+153 
+154 
+155# def is_builtin_class_instance(obj: typing.Any) -> bool: 
+156# return is_builtin_type(obj.__class__) 
+157 
+158 
+159def is_from_types_or_typing(_type: Type) -> bool: 
+160 """ 
+161 Returns whether _type is one of the stlib typing/types types. 
+162 
+163 e.g. types.UnionType or typing.Union 
+164 """ 
+165 return _type.__module__ in ("types", "typing") 
+166 
+167 
+168def is_from_other_toml_supported_module(_type: Type) -> bool: 
+169 """ 
+170 Besides builtins, toml also supports 'datetime' and 'math' types, \ 
+171 so this returns whether _type is a type from these stdlib modules. 
+172 """ 
+173 return _type.__module__ in ("datetime", "math") 
+174 
+175 
+176def is_parameterized(_type: Type) -> bool: 
+177 """ 
+178 Returns whether _type is a parameterized type. 
+179 
+180 Examples: 
+181 list[str] -> True 
+182 str -> False 
+183 """ 
+184 return typing.get_origin(_type) is not None 
+185 
+186 
+187def is_custom_class(_type: Type) -> bool: 
+188 """ 
+189 Tries to guess if _type is a builtin or a custom (user-defined) class. 
+190 
+191 Other logic in this module depends on knowing that. 
+192 """ 
+193 return ( 
+194 type(_type) is type 
+195 and not is_builtin_type(_type) 
+196 and not is_from_other_toml_supported_module(_type) 
+197 and not is_from_types_or_typing(_type) 
+198 ) 
+199 
+200 
+201def instance_of_custom_class(var: typing.Any) -> bool: 
+202 """ 
+203 Calls `is_custom_class` on an instance of a (possibly custom) class. 
+204 """ 
+205 return is_custom_class(var.__class__) 
+206 
+207 
+208def is_optional(_type: Type | None) -> bool: 
+209 """ 
+210 Tries to guess if _type could be optional. 
+211 
+212 Examples: 
+213 None -> True 
+214 NoneType -> True 
+215 typing.Union[str, None] -> True 
+216 str | None -> True 
+217 list[str | None] -> False 
+218 list[str] -> False 
+219 """ 
+220 if _type and is_parameterized(_type) and typing.get_origin(_type) in (dict,
 list): 
-212 # e.g. list[str] 
-213 # will crash issubclass to test it first here 
-214 return False 
-215 
-216 return ( 
-217 _type is None 
-218 or issubclass(types.NoneType, _type) 
-219 or issubclass(types.NoneType, type(_type)) # no type # Nonetype 
-220 or type(None) in typing.get_args(_type) # union with Nonetype 
-221 ) 
-222 
-223 
-224def dataclass_field(cls: Type, key: str) -> typing.Optional[dc.Field
+221 # e.g. list[str] 
+222 # will crash issubclass to test it first here 
+223 return False 
+224 elif _type is math.nan: 
+225 return False 
+226 
+227 return ( 
+228 _type is None 
+229 or types.NoneType in typing.get_args(_type) # union with Nonetype 
+230 or issubclass(types.NoneType, _type) 
+231 or issubclass(types.NoneType, type(_type)) # no type # Nonetype 
+232 ) 
+233 
+234 
+235def dataclass_field(cls: Type, key: str) -> typing.Optional[dc.Field
 [typing.Any]]: 
-225 """ 
-226 Get Field info for a dataclass cls. 
-227 """ 
-228 fields = getattr(cls, "__dataclass_fields__", {}) 
-229 return fields.get(key) 
-230 
-231 
-232def load_recursive(cls: Type, data: dict[str, T], annotations: dict[str,
+236 """ 
+237 Get Field info for a dataclass cls. 
+238 """ 
+239 fields = getattr(cls, "__dataclass_fields__", {}) 
+240 return fields.get(key) 
+241 
+242 
+243def load_recursive(cls: Type, data: dict[str, T], annotations: dict[str,
 Type]) -> dict[str, T]: 
-233 """ 
-234 For all annotations (recursively gathered from parents with
+244 """ 
+245 For all annotations (recursively gathered from parents with
 `all_annotations`), \ 
-235 try to resolve the tree of annotations. 
-236 
-237 Uses `load_into_recurse`, not itself directly. 
-238 
-239 Example: 
-240 class First: 
-241 key: str 
-242 
-243 class Second: 
-244 other: First 
-245 
-246 # step 1 
-247 cls = Second 
-248 data = {"second": {"other": {"key": "anything"}}} 
-249 annotations: {"other": First} 
-250 
-251 # step 1.5 
-252 data = {"other": {"key": "anything"} 
-253 annotations: {"other": First} 
-254 
-255 # step 2 
-256 cls = First 
-257 data = {"key": "anything"} 
-258 annotations: {"key": str} 
-259 
-260 """ 
-261 updated = {} 
-262 for _key, _type in annotations.items(): 
-263 if _key in data: 
-264 value: typing.Any = data[_key] # value can change so define it as any
+246 try to resolve the tree of annotations. 
+247 
+248 Uses `load_into_recurse`, not itself directly. 
+249 
+250 Example: 
+251 class First: 
+252 key: str 
+253 
+254 class Second: 
+255 other: First 
+256 
+257 # step 1 
+258 cls = Second 
+259 data = {"second": {"other": {"key": "anything"}}} 
+260 annotations: {"other": First} 
+261 
+262 # step 1.5 
+263 data = {"other": {"key": "anything"} 
+264 annotations: {"other": First} 
+265 
+266 # step 2 
+267 cls = First 
+268 data = {"key": "anything"} 
+269 annotations: {"key": str} 
+270 
+271 """ 
+272 updated = {} 
+273 
+274 for _key, _type in annotations.items(): 
+275 if _key in data: 
+276 value: typing.Any = data[_key] # value can change so define it as any
 instead of T 
-265 if is_parameterized(_type): 
-266 origin = typing.get_origin(_type) 
-267 arguments = typing.get_args(_type) 
-268 if origin is list and arguments and is_custom_class(arguments[0]): 
-269 subtype = arguments[0] 
-270 value = [_load_into_recurse(subtype, subvalue) for subvalue in value] 
-271 
-272 elif origin is dict and arguments and is_custom_class(arguments[1]): 
-273 # e.g. dict[str, Point] 
-274 subkeytype, subvaluetype = arguments 
-275 # subkey(type) is not a custom class, so don't try to convert it: 
-276 value = {subkey: _load_into_recurse(subvaluetype, subvalue) for subkey,
+277 if is_parameterized(_type): 
+278 origin = typing.get_origin(_type) 
+279 arguments = typing.get_args(_type) 
+280 if origin is list and arguments and is_custom_class(arguments[0]): 
+281 subtype = arguments[0] 
+282 value = [_load_into_recurse(subtype, subvalue) for subvalue in value] 
+283 
+284 elif origin is dict and arguments and is_custom_class(arguments[1]): 
+285 # e.g. dict[str, Point] 
+286 subkeytype, subvaluetype = arguments 
+287 # subkey(type) is not a custom class, so don't try to convert it: 
+288 value = {subkey: _load_into_recurse(subvaluetype, subvalue) for subkey,
 subvalue in value.items()} 
-277 # elif origin is dict: 
-278 # keep data the same 
-279 elif origin is typing.Union and arguments: 
-280 for arg in arguments: 
-281 if is_custom_class(arg): 
-282 value = _load_into_recurse(arg, value) 
-283 else: 
-284 # print(_type, arg, value) 
-285 ... 
-286 
-287 # todo: other parameterized/unions/typing.Optional 
-288 
-289 elif is_custom_class(_type): 
-290 # type must be C (custom class) at this point 
-291 value = _load_into_recurse( 
-292 # make mypy and pycharm happy by telling it _type is of type C... 
-293 # actually just passing _type as first arg! 
-294 typing.cast(Type_C[typing.Any], _type), 
-295 value, 
-296 ) 
-297 
-298 elif _key in cls.__dict__: 
-299 # property has default, use that instead. 
-300 value = cls.__dict__[_key] 
-301 elif is_optional(_type): 
-302 # type is optional and not found in __dict__ -> default is None 
-303 value = None 
-304 elif dc.is_dataclass(cls) and (field := dataclass_field(cls, _key)) and
+289 # elif origin is dict: 
+290 # keep data the same 
+291 elif origin is typing.Union and arguments: 
+292 for arg in arguments: 
+293 if is_custom_class(arg): 
+294 value = _load_into_recurse(arg, value) 
+295 else: 
+296 # print(_type, arg, value) 
+297 ... 
+298 
+299 # todo: other parameterized/unions/typing.Optional 
+300 
+301 elif is_custom_class(_type): 
+302 # type must be C (custom class) at this point 
+303 value = _load_into_recurse( 
+304 # make mypy and pycharm happy by telling it _type is of type C... 
+305 # actually just passing _type as first arg! 
+306 typing.cast(Type_C[typing.Any], _type), 
+307 value, 
+308 ) 
+309 
+310 elif _key in cls.__dict__: 
+311 # property has default, use that instead. 
+312 value = cls.__dict__[_key] 
+313 elif is_optional(_type): 
+314 # type is optional and not found in __dict__ -> default is None 
+315 value = None 
+316 elif dc.is_dataclass(cls) and (field := dataclass_field(cls, _key)) and
 field.default_factory is not dc.MISSING: 
-305 # could have a default factory 
-306 # todo: do something with field.default? 
-307 value = field.default_factory() 
-308 else: 
-309 # todo: exception group? 
-310 raise ConfigErrorMissingKey(_key, cls, _type) 
-311 
-312 updated[_key] = value 
-313 
-314 return updated 
-315 
-316 
-317def _all_annotations(cls: Type) -> ChainMap[str, Type]: 
-318 """ 
-319 Returns a dictionary-like ChainMap that includes annotations for all \ 
-320 attributes defined in cls or inherited from superclasses. 
-321 """ 
-322 return ChainMap(*(c.__annotations__ for c in getattr(cls, "__mro__", []) if
-"__annotations__" in c.__dict__)) 
-323 
+317 # could have a default factory 
+318 # todo: do something with field.default? 
+319 value = field.default_factory() 
+320 else: 
+321 raise ConfigErrorMissingKey(_key, cls, _type) 
+322 
+323 updated[_key] = value 
 324 
-325def all_annotations(cls: Type, _except: typing.Iterable[str] = None) -> dict
+325 return updated 
+326 
+327 
+328def _all_annotations(cls: Type) -> ChainMap[str, Type]: 
+329 """ 
+330 Returns a dictionary-like ChainMap that includes annotations for all \ 
+331 attributes defined in cls or inherited from superclasses. 
+332 """ 
+333 return ChainMap(*(c.__annotations__ for c in getattr(cls, "__mro__", []) if
+"__annotations__" in c.__dict__)) 
+334 
+335 
+336def all_annotations(cls: Type, _except: typing.Iterable[str] = None) -> dict
 [str, Type]: 
-326 """ 
-327 Wrapper around `_all_annotations` that filters away any keys in _except. 
-328 
-329 It also flattens the ChainMap to a regular dict. 
-330 """ 
-331 if _except is None: 
-332 _except = set() 
-333 
-334 _all = _all_annotations(cls) 
-335 return {k: v for k, v in _all.items() if k not in _except} 
-336 
-337 
-338def check_and_convert_data( 
-339 cls: typing.Type[C], 
-340 data: dict[str, typing.Any], 
-341 _except: typing.Iterable[str], 
-342 strict: bool = True, 
-343) -> dict[str, typing.Any]: 
-344 """ 
-345 Based on class annotations, this prepares the data for
+337 """ 
+338 Wrapper around `_all_annotations` that filters away any keys in _except. 
+339 
+340 It also flattens the ChainMap to a regular dict. 
+341 """ 
+342 if _except is None: 
+343 _except = set() 
+344 
+345 _all = _all_annotations(cls) 
+346 return {k: v for k, v in _all.items() if k not in _except} 
+347 
+348 
+349def check_and_convert_data( 
+350 cls: typing.Type[C], 
+351 data: dict[str, typing.Any], 
+352 _except: typing.Iterable[str], 
+353 strict: bool = True, 
+354) -> dict[str, typing.Any]: 
+355 """ 
+356 Based on class annotations, this prepares the data for
 `load_into_recurse`. 
-346 
-347 1. convert config-keys to python compatible config_keys 
-348 2. loads custom class type annotations with the same logic (see also
+357 
+358 1. convert config-keys to python compatible config_keys 
+359 2. loads custom class type annotations with the same logic (see also
 `load_recursive`) 
-349 3. ensures the annotated types match the actual types after loading the
+360 3. ensures the annotated types match the actual types after loading the
 config file. 
-350 """ 
-351 annotations = all_annotations(cls, _except=_except) 
-352 
-353 to_load = convert_config(data) 
-354 to_load = load_recursive(cls, to_load, annotations) 
-355 if strict: 
-356 to_load = ensure_types(to_load, annotations) 
-357 
-358 return to_load 
-359 
-360 
-361def _load_into_recurse( 
-362 cls: typing.Type[C], 
-363 data: dict[str, typing.Any], 
-364 init: dict[str, typing.Any] = None, 
-365 strict: bool = True, 
-366) -> C: 
-367 """ 
-368 Loads an instance of `cls` filled with `data`. 
-369 
-370 Uses `load_recursive` to load any fillable annotated properties (see that
+361 """ 
+362 annotations = all_annotations(cls, _except=_except) 
+363 
+364 to_load = convert_config(data) 
+365 to_load = load_recursive(cls, to_load, annotations) 
+366 if strict: 
+367 to_load = ensure_types(to_load, annotations) 
+368 
+369 return to_load 
+370 
+371 
+372def _load_into_recurse( 
+373 cls: typing.Type[C], 
+374 data: dict[str, typing.Any], 
+375 init: dict[str, typing.Any] = None, 
+376 strict: bool = True, 
+377) -> C: 
+378 """ 
+379 Loads an instance of `cls` filled with `data`. 
+380 
+381 Uses `load_recursive` to load any fillable annotated properties (see that
 method for an example). 
-371 `init` can be used to optionally pass extra __init__ arguments. \ 
-372 NOTE: This will overwrite a config key with the same name! 
-373 """ 
-374 if init is None: 
-375 init = {} 
-376 
-377 # fixme: cls.__init__ can set other keys than the name is in kwargs!! 
-378 
-379 if dc.is_dataclass(cls): 
-380 to_load = check_and_convert_data(cls, data, init.keys(), strict=strict) 
-381 to_load |= init # add extra init variables (should not happen for a
+382 `init` can be used to optionally pass extra __init__ arguments. \ 
+383 NOTE: This will overwrite a config key with the same name! 
+384 """ 
+385 if init is None: 
+386 init = {} 
+387 
+388 # fixme: cls.__init__ can set other keys than the name is in kwargs!! 
+389 
+390 if dc.is_dataclass(cls): 
+391 to_load = check_and_convert_data(cls, data, init.keys(), strict=strict) 
+392 to_load |= init # add extra init variables (should not happen for a
 dataclass but whatev) 
-382 
-383 # ensure mypy inst is an instance of the cls type (and not a fictuous
+393 
+394 # ensure mypy inst is an instance of the cls type (and not a fictuous
 `DataclassInstance`) 
-384 inst = typing.cast(C, cls(**to_load)) 
-385 else: 
-386 inst = cls(**init) 
-387 to_load = check_and_convert_data(cls, data, inst.__dict__.keys(),
+395 inst = typing.cast(C, cls(**to_load)) 
+396 else: 
+397 inst = cls(**init) 
+398 to_load = check_and_convert_data(cls, data, inst.__dict__.keys(),
 strict=strict) 
-388 inst.__dict__.update(**to_load) 
-389 
-390 return inst 
-391 
-392 
-393def _load_into_instance( 
-394 inst: C, 
-395 cls: typing.Type[C], 
-396 data: dict[str, typing.Any], 
-397 init: dict[str, typing.Any] = None, 
-398 strict: bool = True, 
-399) -> C: 
-400 """ 
-401 Similar to `load_into_recurse` but uses an existing instance of a class (so
-after __init__) \ 
-402 and thus does not support init. 
+399 inst.__dict__.update(**to_load) 
+400 
+401 return inst 
+402 
 403 
-404 """ 
-405 if init is not None: 
-406 raise ValueError("Can not init an existing instance!") 
-407 
-408 existing_data = inst.__dict__ 
-409 
-410 to_load = check_and_convert_data(cls, data, _except=existing_data.keys(),
+404def _load_into_instance( 
+405 inst: C, 
+406 cls: typing.Type[C], 
+407 data: dict[str, typing.Any], 
+408 init: dict[str, typing.Any] = None, 
+409 strict: bool = True, 
+410) -> C: 
+411 """ 
+412 Similar to `load_into_recurse` but uses an existing instance of a class (so
+after __init__) \ 
+413 and thus does not support init. 
+414 
+415 """ 
+416 if init is not None: 
+417 raise ValueError("Can not init an existing instance!") 
+418 
+419 existing_data = inst.__dict__ 
+420 
+421 to_load = check_and_convert_data(cls, data, _except=existing_data.keys(),
 strict=strict) 
-411 
-412 inst.__dict__.update(**to_load) 
-413 
-414 return inst 
-415 
-416 
-417def load_into_class( 
-418 cls: typing.Type[C], 
-419 data: T_data, 
-420 /, 
-421 key: str = None, 
-422 init: dict[str, typing.Any] = None, 
-423 strict: bool = True, 
-424) -> C: 
-425 """ 
-426 Shortcut for _load_data + load_into_recurse. 
-427 """ 
-428 to_load = _load_data(data, key, cls.__name__) 
-429 return _load_into_recurse(cls, to_load, init=init, strict=strict) 
-430 
-431 
-432def load_into_instance( 
-433 inst: C, 
-434 data: T_data, 
-435 /, 
-436 key: str = None, 
-437 init: dict[str, typing.Any] = None, 
-438 strict: bool = True, 
-439) -> C: 
-440 """ 
-441 Shortcut for _load_data + load_into_existing. 
-442 """ 
-443 cls = inst.__class__ 
-444 to_load = _load_data(data, key, cls.__name__) 
-445 return _load_into_instance(inst, cls, to_load, init=init, strict=strict) 
-446 
-447 
-448def load_into( 
-449 cls: typing.Type[C], 
-450 data: T_data, 
-451 /, 
-452 key: str = None, 
-453 init: dict[str, typing.Any] = None, 
-454 strict: bool = True, 
-455) -> C: 
-456 """ 
-457 Load your config into a class (instance). 
+422 
+423 inst.__dict__.update(**to_load) 
+424 
+425 return inst 
+426 
+427 
+428def load_into_class( 
+429 cls: typing.Type[C], 
+430 data: T_data, 
+431 /, 
+432 key: str = None, 
+433 init: dict[str, typing.Any] = None, 
+434 strict: bool = True, 
+435) -> C: 
+436 """ 
+437 Shortcut for _load_data + load_into_recurse. 
+438 """ 
+439 to_load = _load_data(data, key, cls.__name__) 
+440 return _load_into_recurse(cls, to_load, init=init, strict=strict) 
+441 
+442 
+443def load_into_instance( 
+444 inst: C, 
+445 data: T_data, 
+446 /, 
+447 key: str = None, 
+448 init: dict[str, typing.Any] = None, 
+449 strict: bool = True, 
+450) -> C: 
+451 """ 
+452 Shortcut for _load_data + load_into_existing. 
+453 """ 
+454 cls = inst.__class__ 
+455 to_load = _load_data(data, key, cls.__name__) 
+456 return _load_into_instance(inst, cls, to_load, init=init, strict=strict) 
+457 
 458 
-459 Supports both a class or an instance as first argument, but that's hard to
+459def load_into( 
+460 cls: typing.Type[C], 
+461 data: T_data, 
+462 /, 
+463 key: str = None, 
+464 init: dict[str, typing.Any] = None, 
+465 strict: bool = True, 
+466) -> C: 
+467 """ 
+468 Load your config into a class (instance). 
+469 
+470 Supports both a class or an instance as first argument, but that's hard to
 explain to mypy, so officially only 
-460 classes are supported, and if you want to `load_into` an instance, you
+471 classes are supported, and if you want to `load_into` an instance, you
 should use `load_into_instance`. 
-461 
-462 Args: 
-463 cls: either a class or an existing instance of that class. 
-464 data: can be a dictionary or a path to a file to load (as pathlib.Path or
+472 
+473 Args: 
+474 cls: either a class or an existing instance of that class. 
+475 data: can be a dictionary or a path to a file to load (as pathlib.Path or
 str) 
-465 key: optional (nested) dictionary key to load data from (e.g.
+476 key: optional (nested) dictionary key to load data from (e.g.
 'tool.su6.specific') 
-466 init: optional data to pass to your cls' __init__ method (only if cls is
+477 init: optional data to pass to your cls' __init__ method (only if cls is
 not an instance already) 
-467 strict: enable type checks or allow anything? 
-468 
-469 """ 
-470 if not isinstance(cls, type): 
-471 # would not be supported according to mypy, but you can still load_into
+478 strict: enable type checks or allow anything? 
+479 
+480 """ 
+481 if not isinstance(cls, type): 
+482 # would not be supported according to mypy, but you can still load_into
 (instance) 
-472 return load_into_instance(cls, data, key=key, init=init, strict=strict) 
-473 
-474 # make mypy and pycharm happy by telling it cls is of type C and not just
+483 return load_into_instance(cls, data, key=key, init=init, strict=strict) 
+484 
+485 # make mypy and pycharm happy by telling it cls is of type C and not just
 'type' 
-475 # _cls = typing.cast(typing.Type[C], cls) 
-476 return load_into_class(cls, data, key=key, init=init, strict=strict) 
+486 # _cls = typing.cast(typing.Type[C], cls) 
+487 return load_into_class(cls, data, key=key, init=init, strict=strict) 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-15 14:30 +0200
+at 2023-06-15 16:44 +0200
```

### Comparing `configuraptor-1.5.0/htmlcov/d_eb75b6cf8f5eab40_dump_py.html` & `configuraptor-1.5.1/htmlcov/d_eb75b6cf8f5eab40_postpone_py.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/configuraptor/dump.py: 0%</title>
+    <title>Coverage for src/configuraptor/postpone.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>src/configuraptor/dump.py</b>:
-            <span class="pc_cov">0%</span>
+            <span class="text">Coverage for </span><b>src/configuraptor/postpone.py</b>:
+            <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -50,23 +50,23 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">9 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">9<span class="text"> missing</span></button>
+            <span class="text">8 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">8<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_core_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_shared_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_singleton_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
             created at 2023-06-15 14:30 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
@@ -76,38 +76,57 @@
             <button type="button" class="button_next_file" data-shortcut="]"/>
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
-    <p class="mis show_mis"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">def</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">    <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">File contains logic to do with the 'postpone' feature.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">def</span> <span class="nam">astoml</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">errors</span> <span class="key">import</span> <span class="nam">IsPostponedError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">singleton</span> <span class="key">import</span> <span class="nam">Singleton</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">def</span> <span class="nam">asjson</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">class</span> <span class="nam">Postponed</span><span class="op">(</span><span class="nam">Singleton</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="str">    Class returned by `postpone` below.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="key">def</span> <span class="nam">asyaml</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">    <span class="key">def</span> <span class="nam">__get__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">instance</span><span class="op">:</span> <span class="nam">type</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">owner</span><span class="op">:</span> <span class="nam">type</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Never</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="str">        This magic method is called when a property is accessed.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="str">        Example:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="str">             someclass.someprop will trigger the __get__ of `someprop`</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="str">        Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="str">            instance: the class on which the postponed property is defined,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="str">            owner: `SingletonMeta`</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="key">raise</span> <span class="nam">IsPostponedError</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t"><span class="key">def</span> <span class="nam">postpone</span><span class="op">(</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="str">    Can be used to mark a property as postponed, meaning the user will fill it in later (they promose).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t"><span class="str">    If they don't fill it in and still try to use it, they will be met with a IsPostponedError.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="key">return</span> <span class="nam">Postponed</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_core_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_shared_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_singleton_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
             created at 2023-06-15 14:30 +0200
         </p>
     </div>
 </footer>
 </body>
```

#### html2text {}

```diff
@@ -1,36 +1,58 @@
 
-****** Coverage for src/configuraptor/dump.py: 0% ******
+****** Coverage for src/configuraptor/postpone.py: 100% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 9 statements   0 run 9 missing 0 excluded *****
+***** 8 statements   8 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
 at 2023-06-15 14:30 +0200
 
 
-1import typing 
-2 
-3 
-4def asdict(inst: typing.Any) -> dict[str, typing.Any]: 
-5 ... 
+1""" 
+2File contains logic to do with the 'postpone' feature. 
+3""" 
+4 
+5import typing 
 6 
-7 
-8def astoml(inst: typing.Any) -> str: 
-9 data = asdict(inst) 
+7from .errors import IsPostponedError 
+8from .singleton import Singleton 
+9 
 10 
-11 
-12def asjson(inst: typing.Any) -> str: 
-13 data = asdict(inst) 
-14 
+11class Postponed(Singleton): 
+12 """ 
+13 Class returned by `postpone` below. 
+14 """ 
 15 
-16def asyaml(inst: typing.Any) -> str: 
-17 data = asdict(inst) 
+16 def __get__(self, instance: type[typing.Any], owner: type[typing.Any]) -
+> typing.Never: 
+17 """ 
+18 This magic method is called when a property is accessed. 
+19 
+20 Example: 
+21 someclass.someprop will trigger the __get__ of `someprop` 
+22 
+23 Args: 
+24 instance: the class on which the postponed property is defined, 
+25 owner: `SingletonMeta` 
+26 """ 
+27 raise IsPostponedError() 
+28 
+29 
+30def postpone() -> typing.Any: 
+31 """ 
+32 Can be used to mark a property as postponed, meaning the user will fill it
+in later (they promose). 
+33 
+34 If they don't fill it in and still try to use it, they will be met with a
+IsPostponedError. 
+35 """ 
+36 return Postponed() 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
 at 2023-06-15 14:30 +0200
```

### Comparing `configuraptor-1.5.0/htmlcov/d_eb75b6cf8f5eab40_errors_py.html` & `configuraptor-1.5.1/htmlcov/d_eb75b6cf8f5eab40_errors_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_dump_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_helpers_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 14:30 +0200
+            created at 2023-06-15 16:40 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -89,88 +89,101 @@
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">class</span> <span class="nam">ConfigError</span><span class="op">(</span><span class="nam">Exception</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="str">    Base exception class for this module.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="op">@</span><span class="nam">dataclass</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="key">class</span> <span class="nam">ConfigErrorMissingKey</span><span class="op">(</span><span class="nam">ConfigError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="str">    Exception for when the config file is missing a required key.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">type</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">    <span class="nam">annotated_type</span><span class="op">:</span> <span class="nam">type</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="key">def</span> <span class="nam">__post_init__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="str">        Automatically filles in the names of annotated type and cls for printing from __str__.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_annotated_type</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">annotated_type</span><span class="op">.</span><span class="nam">__name__</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_cls</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t"><span class="str">        Custom error message based on dataclass values and calculated actual type.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="key">return</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">            <span class="str">f"Config key '{self.key}' (type `{self._annotated_type}`) "</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">            <span class="str">f"of class `{self._cls}` was not found in the config, "</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">            <span class="str">f"but is required as a default value is not specified."</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t"><span class="op">@</span><span class="nam">dataclass</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t"><span class="key">class</span> <span class="nam">ConfigErrorInvalidType</span><span class="op">(</span><span class="nam">ConfigError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t"><span class="str">    Exception for when the config file contains a key with an unexpected type.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="nam">value</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">    <span class="nam">expected_type</span><span class="op">:</span> <span class="nam">type</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">    <span class="key">def</span> <span class="nam">__post_init__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t"><span class="str">        Store the actual type of the config variable.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">actual_type</span> <span class="op">=</span> <span class="nam">type</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">        <span class="nam">max_len</span> <span class="op">=</span> <span class="num">50</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_value</span> <span class="op">=</span> <span class="nam">str</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">        <span class="key">if</span> <span class="nam">len</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_value</span><span class="op">)</span> <span class="op">></span> <span class="nam">max_len</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">_value</span> <span class="op">=</span> <span class="str">f"{self._value[:max_len]}..."</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t"><span class="str">        Custom error message based on dataclass values and calculated actual type.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">        <span class="key">return</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">            <span class="str">f"Config key '{self.key}' had a value (`{self._value}`) with a type (`{self.actual_type}`) "</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">            <span class="str">f"that was not expected: `{self.expected_type}` is the required type."</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t"><span class="op">@</span><span class="nam">dataclass</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t"><span class="key">class</span> <span class="nam">IsPostponedError</span><span class="op">(</span><span class="nam">ConfigError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t"><span class="str">    Error thrown when you try to access a 'postponed' property without filling its value first.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">    <span class="nam">message</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">"This postponed property has not been filled yet!"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="com"># class ConfigErrorGroup(ConfigError, ExceptionGroup):</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="com">#     """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="com">#     Base Exception class for this module, but for exception groups (3.11+)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="com">#     """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="com">#     def __init__(self, _type: str, errors: list[Exception]):</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="com">#         more = len(errors) > 1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="com">#         cnt = "Multiple" if more else "One"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="com">#         s = "s" if more else ""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="com">#         message = f"{cnt} {_type}{s} in config!"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="com">#         super().__init__(message, errors)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="com">#         if not errors:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="com">#             raise ValueError("Error group raised without any errors?")</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="op">@</span><span class="nam">dataclass</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t"><span class="key">class</span> <span class="nam">ConfigErrorMissingKey</span><span class="op">(</span><span class="nam">ConfigError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t"><span class="str">    Exception for when the config file is missing a required key.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="nam">annotated_type</span><span class="op">:</span> <span class="nam">type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="key">def</span> <span class="nam">__post_init__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t"><span class="str">        Automatically filles in the names of annotated type and cls for printing from __str__.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_annotated_type</span> <span class="op">=</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">annotated_type</span><span class="op">,</span> <span class="str">"__name__"</span><span class="op">,</span> <span class="nam">str</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">annotated_type</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_cls</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t"><span class="str">        Custom error message based on dataclass values and calculated actual type.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">        <span class="key">return</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">            <span class="str">f"Config key '{self.key}' (type `{self._annotated_type}`) "</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">            <span class="str">f"of class `{self._cls}` was not found in the config, "</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">            <span class="str">f"but is required as a default value is not specified."</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t"><span class="op">@</span><span class="nam">dataclass</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t"><span class="key">class</span> <span class="nam">ConfigErrorInvalidType</span><span class="op">(</span><span class="nam">ConfigError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t"><span class="str">    Exception for when the config file contains a key with an unexpected type.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="nam">value</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">    <span class="nam">expected_type</span><span class="op">:</span> <span class="nam">type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">    <span class="key">def</span> <span class="nam">__post_init__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t"><span class="str">        Store the actual type of the config variable.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">actual_type</span> <span class="op">=</span> <span class="nam">type</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="nam">max_len</span> <span class="op">=</span> <span class="num">50</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_value</span> <span class="op">=</span> <span class="nam">str</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">        <span class="key">if</span> <span class="nam">len</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_value</span><span class="op">)</span> <span class="op">></span> <span class="nam">max_len</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">_value</span> <span class="op">=</span> <span class="str">f"{self._value[:max_len]}..."</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t"><span class="str">        Custom error message based on dataclass values and calculated actual type.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">        <span class="key">return</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">            <span class="str">f"Config key '{self.key}' had a value (`{self._value}`) with a type (`{self.actual_type}`) "</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">            <span class="str">f"that was not expected: `{self.expected_type}` is the required type."</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t"><span class="op">@</span><span class="nam">dataclass</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t"><span class="key">class</span> <span class="nam">IsPostponedError</span><span class="op">(</span><span class="nam">ConfigError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t"><span class="str">    Error thrown when you try to access a 'postponed' property without filling its value first.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">    <span class="nam">message</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">"This postponed property has not been filled yet!"</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_dump_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_helpers_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 14:30 +0200
+            created at 2023-06-15 16:40 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 29 statements   29 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-15 14:30 +0200
+at 2023-06-15 16:40 +0200
 
 
 1""" 
 2Contains module-specific custom errors. 
 3""" 
 4import typing 
 5from dataclasses import dataclass 
@@ -23,79 +23,93 @@
 7 
 8class ConfigError(Exception): 
 9 """ 
 10 Base exception class for this module. 
 11 """ 
 12 
 13 
-14@dataclass 
-15class ConfigErrorMissingKey(ConfigError): 
-16 """ 
-17 Exception for when the config file is missing a required key. 
-18 """ 
-19 
-20 key: str 
-21 cls: type 
-22 annotated_type: type 
-23 
-24 def __post_init__(self) -> None: 
-25 """ 
-26 Automatically filles in the names of annotated type and cls for printing
+14# class ConfigErrorGroup(ConfigError, ExceptionGroup): 
+15# """ 
+16# Base Exception class for this module, but for exception groups (3.11+) 
+17# """ 
+18# def __init__(self, _type: str, errors: list[Exception]): 
+19# more = len(errors) > 1 
+20# cnt = "Multiple" if more else "One" 
+21# s = "s" if more else "" 
+22# message = f"{cnt} {_type}{s} in config!" 
+23# super().__init__(message, errors) 
+24# if not errors: 
+25# raise ValueError("Error group raised without any errors?") 
+26 
+27@dataclass 
+28class ConfigErrorMissingKey(ConfigError): 
+29 """ 
+30 Exception for when the config file is missing a required key. 
+31 """ 
+32 
+33 key: str 
+34 cls: type 
+35 annotated_type: type 
+36 
+37 def __post_init__(self) -> None: 
+38 """ 
+39 Automatically filles in the names of annotated type and cls for printing
 from __str__. 
-27 """ 
-28 self._annotated_type = self.annotated_type.__name__ 
-29 self._cls = self.cls.__name__ 
-30 
-31 def __str__(self) -> str: 
-32 """ 
-33 Custom error message based on dataclass values and calculated actual type. 
-34 """ 
-35 return ( 
-36 f"Config key '{self.key}' (type `{self._annotated_type}`) " 
-37 f"of class `{self._cls}` was not found in the config, " 
-38 f"but is required as a default value is not specified." 
-39 ) 
-40 
-41 
-42@dataclass 
-43class ConfigErrorInvalidType(ConfigError): 
-44 """ 
-45 Exception for when the config file contains a key with an unexpected type. 
-46 """ 
-47 
-48 key: str 
-49 value: typing.Any 
-50 expected_type: type 
-51 
-52 def __post_init__(self) -> None: 
-53 """ 
-54 Store the actual type of the config variable. 
-55 """ 
-56 self.actual_type = type(self.value) 
-57 
-58 max_len = 50 
-59 self._value = str(self.value) 
-60 if len(self._value) > max_len: 
-61 self._value = f"{self._value[:max_len]}..." 
-62 
-63 def __str__(self) -> str: 
-64 """ 
-65 Custom error message based on dataclass values and calculated actual type. 
+40 """ 
+41 self._annotated_type = getattr(self.annotated_type, "__name__", str
+(self.annotated_type)) 
+42 self._cls = self.cls.__name__ 
+43 
+44 def __str__(self) -> str: 
+45 """ 
+46 Custom error message based on dataclass values and calculated actual type. 
+47 """ 
+48 return ( 
+49 f"Config key '{self.key}' (type `{self._annotated_type}`) " 
+50 f"of class `{self._cls}` was not found in the config, " 
+51 f"but is required as a default value is not specified." 
+52 ) 
+53 
+54 
+55@dataclass 
+56class ConfigErrorInvalidType(ConfigError): 
+57 """ 
+58 Exception for when the config file contains a key with an unexpected type. 
+59 """ 
+60 
+61 key: str 
+62 value: typing.Any 
+63 expected_type: type 
+64 
+65 def __post_init__(self) -> None: 
 66 """ 
-67 return ( 
-68 f"Config key '{self.key}' had a value (`{self._value}`) with a type (`
+67 Store the actual type of the config variable. 
+68 """ 
+69 self.actual_type = type(self.value) 
+70 
+71 max_len = 50 
+72 self._value = str(self.value) 
+73 if len(self._value) > max_len: 
+74 self._value = f"{self._value[:max_len]}..." 
+75 
+76 def __str__(self) -> str: 
+77 """ 
+78 Custom error message based on dataclass values and calculated actual type. 
+79 """ 
+80 return ( 
+81 f"Config key '{self.key}' had a value (`{self._value}`) with a type (`
 {self.actual_type}`) " 
-69 f"that was not expected: `{self.expected_type}` is the required type." 
-70 ) 
-71 
-72 
-73@dataclass 
-74class IsPostponedError(ConfigError): 
-75 """ 
-76 Error thrown when you try to access a 'postponed' property without filling
+82 f"that was not expected: `{self.expected_type}` is the required type." 
+83 ) 
+84 
+85 
+86@dataclass 
+87class IsPostponedError(ConfigError): 
+88 """ 
+89 Error thrown when you try to access a 'postponed' property without filling
 its value first. 
-77 """ 
-78 
-79 message: str = "This postponed property has not been filled yet!" 
+90 """ 
+91 
+92 message: str = "This postponed property has not been filled yet!" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-15 14:30 +0200
+at 2023-06-15 16:40 +0200
```

### Comparing `configuraptor-1.5.0/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html` & `configuraptor-1.5.1/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html` & `configuraptor-1.5.1/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/htmlcov/favicon_32.png` & `configuraptor-1.5.1/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/htmlcov/index.html` & `configuraptor-1.5.1/htmlcov/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">97%</span>
+            <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -41,15 +41,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 14:32 +0200
+            created at 2023-06-15 16:44 +0200
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -66,39 +66,39 @@
                 <td>1</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="1 1">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_eb75b6cf8f5eab40___init___py.html">src/configuraptor/__init__.py</a></td>
-                <td>5</td>
+                <td>6</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="5 5">100%</td>
+                <td class="right" data-ratio="6 6">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_eb75b6cf8f5eab40_cls_py.html">src/configuraptor/cls.py</a></td>
                 <td>7</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="7 7">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_eb75b6cf8f5eab40_core_py.html">src/configuraptor/core.py</a></td>
-                <td>153</td>
+                <td>158</td>
                 <td>0</td>
                 <td>3</td>
-                <td class="right" data-ratio="153 153">100%</td>
+                <td class="right" data-ratio="158 158">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_eb75b6cf8f5eab40_dump_py.html">src/configuraptor/dump.py</a></td>
-                <td>9</td>
-                <td>9</td>
+                <td>31</td>
                 <td>0</td>
-                <td class="right" data-ratio="0 9">0%</td>
+                <td>0</td>
+                <td class="right" data-ratio="31 31">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_eb75b6cf8f5eab40_errors_py.html">src/configuraptor/errors.py</a></td>
                 <td>29</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="29 29">100%</td>
@@ -108,18 +108,18 @@
                 <td>2</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="2 2">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_6c7dc8b73849fb97___init___py.html">src/configuraptor/loaders/__init__.py</a></td>
-                <td>12</td>
+                <td>11</td>
                 <td>0</td>
                 <td>1</td>
-                <td class="right" data-ratio="12 12">100%</td>
+                <td class="right" data-ratio="11 11">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_6c7dc8b73849fb97__types_py.html">src/configuraptor/loaders/_types.py</a></td>
                 <td>4</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="4 4">100%</td>
@@ -159,30 +159,30 @@
                 <td>0</td>
                 <td class="right" data-ratio="13 13">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>268</td>
-                <td>9</td>
+                <td>295</td>
+                <td>0</td>
                 <td>12</td>
-                <td class="right" data-ratio="259 268">97%</td>
+                <td class="right" data-ratio="295 295">100%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 14:32 +0200
+            created at 2023-06-15 16:44 +0200
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_singleton_py.html"/>
         <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40___about___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
```

#### html2text {}

```diff
@@ -1,31 +1,31 @@
 
-****** Coverage report: 97% ******
+****** Coverage report: 100% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-coverage.py_v7.2.7, created at 2023-06-15 14:32 +0200
+coverage.py_v7.2.7, created at 2023-06-15 16:44 +0200
 
 Module                                   statements missing excluded coverage
 src/configuraptor/__about__.py           1          0       0        100%
-src/configuraptor/__init__.py            5          0       0        100%
+src/configuraptor/__init__.py            6          0       0        100%
 src/configuraptor/cls.py                 7          0       0        100%
-src/configuraptor/core.py                153        0       3        100%
-src/configuraptor/dump.py                9          9       0        0%
+src/configuraptor/core.py                158        0       3        100%
+src/configuraptor/dump.py                31         0       0        100%
 src/configuraptor/errors.py              29         0       0        100%
 src/configuraptor/helpers.py             2          0       0        100%
-src/configuraptor/loaders/__init__.py    12         0       1        100%
+src/configuraptor/loaders/__init__.py    11         0       1        100%
 src/configuraptor/loaders/_types.py      4          0       0        100%
 src/configuraptor/loaders/loaders_310.py 5          0       6        100%
 src/configuraptor/loaders/loaders_311.py 6          0       2        100%
 src/configuraptor/loaders/               14         0       0        100%
 loaders_shared.py
 src/configuraptor/postpone.py            8          0       0        100%
 src/configuraptor/singleton.py           13         0       0        100%
-Total                                    268        9       12       97%
+Total                                    295        0       12       100%
 No items found using the specified filter.
 
-coverage.py_v7.2.7, created at 2023-06-15 14:32 +0200
+coverage.py_v7.2.7, created at 2023-06-15 16:44 +0200
  ____
```

### Comparing `configuraptor-1.5.0/htmlcov/keybd_closed.png` & `configuraptor-1.5.1/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/htmlcov/keybd_open.png` & `configuraptor-1.5.1/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/htmlcov/status.json` & `configuraptor-1.5.1/htmlcov/status.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9955138888888889%*

 * *Differences: {"'files'": "{'d_eb75b6cf8f5eab40___about___py': {'hash': 'c751a6ade0f2b1e3c963979cd459801f'}, "*

 * *            "'d_eb75b6cf8f5eab40___init___py': {'hash': '06dbb9f67d79162cdd2611932d9db344', "*

 * *            "'index': {'nums': {insert: [(2, 6)], delete: [2]}}}, 'd_eb75b6cf8f5eab40_core_py': "*

 * *            "{'hash': '081a1def5c22a0813fc9b4f6d534cf5f', 'index': {'nums': {insert: [(2, 158)], "*

 * *            "delete: [2]}}}, 'd_eb75b6cf8f5eab40_errors_py': {'hash': "*

 * *            "'7dd27517b14a07012ed62bb746e3aa16'}, 'd […]*

```diff
@@ -184,21 +184,21 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/typedconfig/singleton.py"
             }
         },
         "d_6c7dc8b73849fb97___init___py": {
-            "hash": "dcd295f1034f16584936a371969a6beb",
+            "hash": "2ef72ea4377e2966b657f2d94ba1a8c2",
             "index": {
                 "html_filename": "d_6c7dc8b73849fb97___init___py.html",
                 "nums": [
                     0,
                     1,
-                    12,
+                    11,
                     1,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/loaders/__init__.py"
@@ -252,15 +252,15 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/loaders/loaders_311.py"
             }
         },
         "d_6c7dc8b73849fb97_loaders_shared_py": {
-            "hash": "7b50961f6d1e766a1ec9852c1a986615",
+            "hash": "3c629c3aee227f260f4f55d7d252b644",
             "index": {
                 "html_filename": "d_6c7dc8b73849fb97_loaders_shared_py.html",
                 "nums": [
                     0,
                     1,
                     14,
                     0,
@@ -269,15 +269,15 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/loaders/loaders_shared.py"
             }
         },
         "d_eb75b6cf8f5eab40___about___py": {
-            "hash": "ddcab299fefdbca7ab5149887c79e342",
+            "hash": "c751a6ade0f2b1e3c963979cd459801f",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40___about___py.html",
                 "nums": [
                     0,
                     1,
                     1,
                     0,
@@ -286,21 +286,21 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/__about__.py"
             }
         },
         "d_eb75b6cf8f5eab40___init___py": {
-            "hash": "cc5369f83418bca1e9459dfbe12b4bdb",
+            "hash": "06dbb9f67d79162cdd2611932d9db344",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40___init___py.html",
                 "nums": [
                     0,
                     1,
-                    5,
+                    6,
                     0,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/__init__.py"
@@ -320,49 +320,49 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/cls.py"
             }
         },
         "d_eb75b6cf8f5eab40_core_py": {
-            "hash": "a6dc681a32d43c07cb0d3466d02099a6",
+            "hash": "081a1def5c22a0813fc9b4f6d534cf5f",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40_core_py.html",
                 "nums": [
                     0,
                     1,
-                    153,
+                    158,
                     3,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/core.py"
             }
         },
         "d_eb75b6cf8f5eab40_dump_py": {
-            "hash": "9c634b2f736ce78469468f75131fae41",
+            "hash": "d64f111484683805138ede1d7542d62d",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40_dump_py.html",
                 "nums": [
                     0,
                     1,
-                    9,
+                    31,
+                    0,
                     0,
-                    9,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/dump.py"
             }
         },
         "d_eb75b6cf8f5eab40_errors_py": {
-            "hash": "a203963c1ed7ace1238ca6ace8ba1fb5",
+            "hash": "7dd27517b14a07012ed62bb746e3aa16",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40_errors_py.html",
                 "nums": [
                     0,
                     1,
                     29,
                     0,
```

### Comparing `configuraptor-1.5.0/htmlcov/style.css` & `configuraptor-1.5.1/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/pytest_examples/some.toml` & `configuraptor-1.5.1/pytest_examples/some.toml`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/src/configuraptor/__init__.py` & `configuraptor-1.5.1/src/configuraptor/__init__.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/src/configuraptor/cls.py` & `configuraptor-1.5.1/src/configuraptor/cls.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/src/configuraptor/core.py` & `configuraptor-1.5.1/src/configuraptor/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Contains most of the loading logic.
 """
 
 import dataclasses as dc
+import math
 import types
 import typing
 import warnings
 from collections import ChainMap
 from pathlib import Path
 
 from typeguard import TypeCheckError
@@ -98,14 +99,16 @@
 
 
 def ensure_types(data: dict[str, T], annotations: dict[str, type]) -> dict[str, T | None]:
     """
     Make sure all values in 'data' are in line with the ones stored in 'annotations'.
 
     If an annotated key in missing from data, it will be filled with None for convenience.
+
+    TODO: python 3.11 exception groups to throw multiple errors at once!
     """
     # custom object to use instead of None, since typing.Optional can be None!
     # cast to T to make mypy happy
     notfound = typing.cast(T, object())
     postponed = Postponed()
 
     final: dict[str, T | None] = {}
@@ -122,14 +125,15 @@
             # don't do anything with this item!
             continue
 
         if not check_type(compare, _type):
             raise ConfigErrorInvalidType(key, value=compare, expected_type=_type)
 
         final[key] = compare
+
     return final
 
 
 def convert_config(items: dict[str, T]) -> dict[str, T]:
     """
     Converts the config dict (from toml) or 'overwrites' dict in two ways.
 
@@ -199,36 +203,36 @@
 def instance_of_custom_class(var: typing.Any) -> bool:
     """
     Calls `is_custom_class` on an instance of a (possibly custom) class.
     """
     return is_custom_class(var.__class__)
 
 
-def is_optional(_type: Type | None) -> bool:
+def is_optional(_type: Type | typing.Any) -> bool:
     """
     Tries to guess if _type could be optional.
 
     Examples:
         None -> True
         NoneType -> True
         typing.Union[str, None] -> True
         str | None -> True
         list[str | None] -> False
         list[str] -> False
     """
-    if _type and is_parameterized(_type) and typing.get_origin(_type) in (dict, list):
+    if _type and (is_parameterized(_type) and typing.get_origin(_type) in (dict, list)) or (_type is math.nan):
         # e.g. list[str]
         # will crash issubclass to test it first here
         return False
 
     return (
         _type is None
+        or types.NoneType in typing.get_args(_type)  # union with Nonetype
         or issubclass(types.NoneType, _type)
         or issubclass(types.NoneType, type(_type))  # no type  # Nonetype
-        or type(None) in typing.get_args(_type)  # union with Nonetype
     )
 
 
 def dataclass_field(cls: Type, key: str) -> typing.Optional[dc.Field[typing.Any]]:
     """
     Get Field info for a dataclass cls.
     """
@@ -260,16 +264,19 @@
         annotations: {"other": First}
 
         # step 2
         cls = First
         data = {"key": "anything"}
         annotations: {"key": str}
 
+
+    TODO: python 3.11 exception groups to throw multiple errors at once!
     """
     updated = {}
+
     for _key, _type in annotations.items():
         if _key in data:
             value: typing.Any = data[_key]  # value can change so define it as any instead of T
             if is_parameterized(_type):
                 origin = typing.get_origin(_type)
                 arguments = typing.get_args(_type)
                 if origin is list and arguments and is_custom_class(arguments[0]):
@@ -309,15 +316,14 @@
             # type is optional and not found in __dict__ -> default is None
             value = None
         elif dc.is_dataclass(cls) and (field := dataclass_field(cls, _key)) and field.default_factory is not dc.MISSING:
             # could have a default factory
             # todo: do something with field.default?
             value = field.default_factory()
         else:
-            # todo: exception group?
             raise ConfigErrorMissingKey(_key, cls, _type)
 
         updated[_key] = value
 
     return updated
```

### Comparing `configuraptor-1.5.0/src/configuraptor/dump.py` & `configuraptor-1.5.1/src/configuraptor/dump.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/src/configuraptor/postpone.py` & `configuraptor-1.5.1/src/configuraptor/postpone.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/src/configuraptor/singleton.py` & `configuraptor-1.5.1/src/configuraptor/singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/src/configuraptor/loaders/__init__.py` & `configuraptor-1.5.1/src/configuraptor/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/src/configuraptor/loaders/loaders_shared.py` & `configuraptor-1.5.1/src/configuraptor/loaders/loaders_shared.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/tests/test_core.py` & `configuraptor-1.5.1/tests/test_core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # not directly testable
+import math
 import sys
+import typing
 
 import pytest
 
 from src.configuraptor import all_annotations
+from src.configuraptor.core import is_optional
 from tests.constants import EXAMPLE_FILE
 
 if sys.version_info > (3, 11):
 
     def test_loader_310_fails():
         with pytest.raises(EnvironmentError):
             from src.configuraptor.loaders.loaders_310 import toml
@@ -32,14 +35,18 @@
 def test_invalid_extension():
     from src.configuraptor.loaders import get
 
     with pytest.raises(ValueError):
         get(".doesntexist")
 
 
+def test_is_optional_with_weird_inputs():
+    assert is_optional(math.nan) is False
+    assert is_optional(typing.Optional[dict[str, typing.Optional[str]]]) is True
+
 class Base:
     has: int
 
 
 class Sub(Base):
     has_also: int
```

### Comparing `configuraptor-1.5.0/tests/test_dumps.py` & `configuraptor-1.5.1/tests/test_dumps.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/tests/test_json_yaml.py` & `configuraptor-1.5.1/tests/test_json_yaml.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/tests/test_postponed.py` & `configuraptor-1.5.1/tests/test_postponed.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/tests/test_singleton.py` & `configuraptor-1.5.1/tests/test_singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/tests/test_toml_basic.py` & `configuraptor-1.5.1/tests/test_toml_basic.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/tests/test_toml_dataclass.py` & `configuraptor-1.5.1/tests/test_toml_dataclass.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/tests/test_toml_existing.py` & `configuraptor-1.5.1/tests/test_toml_existing.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 def test_existing_instances():
     data = _load_toml()
 
     inst1 = ToolWithInit("some setup")
 
     normal_tool = configuraptor.load_into(Tool, data)
     inst1_extended = configuraptor.load_into(inst1, data)
+    assert inst1_extended is inst1
 
     assert inst1.fruits
 
     assert inst1_extended.first.extra["name"]["first"] == normal_tool.first.extra["name"]["first"]
 
     with pytest.raises(ValueError):
         configuraptor.load_into(inst1, data, init=dict(more_properties="Should not be allowed!"))
```

### Comparing `configuraptor-1.5.0/tests/test_toml_typedconfig_class.py` & `configuraptor-1.5.1/tests/test_toml_typedconfig_class.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/LICENSE.txt` & `configuraptor-1.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/README.md` & `configuraptor-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/pyproject.toml` & `configuraptor-1.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `configuraptor-1.5.0/PKG-INFO` & `configuraptor-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configuraptor
-Version: 1.5.0
+Version: 1.5.1
 Summary: Load toml/yaml/json config files into classes for a typed config (type hinting etc.)
 Project-URL: Documentation, https://github.com/trialandsuccess/configuraptor#readme
 Project-URL: Issues, https://github.com/trialandsuccess/configuraptor/issues
 Project-URL: Source, https://github.com/trialandsuccess/configuraptor
 Author-email: Robin van der Noord <robin@trialandsuccess.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

