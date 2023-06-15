# Comparing `tmp/configuraptor-1.3.1.tar.gz` & `tmp/configuraptor-1.3.2.tar.gz`

## Comparing `configuraptor-1.3.1.tar` & `configuraptor-1.3.2.tar`

### file list

```diff
@@ -1,83 +1,86 @@
--rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 configuraptor-1.3.1/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.3.1/coverage.svg
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 configuraptor-1.3.1/.github/workflows/su6.yml
--rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.3.1/_static/configuraptor_circle.png
--rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.3.1/_static/configuraptor_original.jpeg
--rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.3.1/_static/configuraptor_round.png
--rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.3.1/_static/configuraptor_transparent.png
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 configuraptor-1.3.1/examples/dataclass.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.3.1/examples/example_from_docs.json
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 configuraptor-1.3.1/examples/example_from_docs.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 configuraptor-1.3.1/examples/example_from_docs.toml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.3.1/examples/example_from_docs.yaml
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 configuraptor-1.3.1/examples/main.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 configuraptor-1.3.1/examples/singleton.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.3.1/examples/typedconfig_class.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_31a2a1dc9b603870___init___py.html
--rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_47560703719c1d9e___about___py.html
--rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_47560703719c1d9e___init___py.html
--rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_47560703719c1d9e_cls_py.html
--rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_47560703719c1d9e_core_py.html
--rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_47560703719c1d9e_errors_py.html
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_47560703719c1d9e_helpers_py.html
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_47560703719c1d9e_main_py.html
--rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_47560703719c1d9e_singleton_py.html
--rw-r--r--   0        0        0    13203 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_6c7dc8b73849fb97___init___py.html
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_6c7dc8b73849fb97__types_py.html
--rw-r--r--   0        0        0     9079 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html
--rw-r--r--   0        0        0     8566 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html
--rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40___about___py.html
--rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40___init___py.html
--rw-r--r--   0        0        0    10338 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40_cls_py.html
--rw-r--r--   0        0        0   124666 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40_core_py.html
--rw-r--r--   0        0        0    19533 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40_errors_py.html
--rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html
--rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     7414 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.3.1/pytest_examples/empty.toml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.3.1/pytest_examples/example.json
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configuraptor-1.3.1/pytest_examples/example.toml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.3.1/pytest_examples/example.yaml
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.3.1/pytest_examples/some.toml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.3.1/pytest_examples/with_dict_of_custom.toml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.3.1/pytest_examples/with_multiple_toplevel_keys.toml
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/__about__.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/__init__.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/cls.py
--rw-r--r--   0        0        0    15026 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/core.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/errors.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/py.typed
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/singleton.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/loaders/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/loaders/_types.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/loaders/loaders_310.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/loaders/loaders_311.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/loaders/loaders_shared.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/loaders/py.typed
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.3.1/tests/__init__.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.3.1/tests/constants.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.3.1/tests/test_about.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 configuraptor-1.3.1/tests/test_core.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.3.1/tests/test_json_yaml.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 configuraptor-1.3.1/tests/test_mypy.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.3.1/tests/test_singleton.py
--rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 configuraptor-1.3.1/tests/test_toml_basic.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 configuraptor-1.3.1/tests/test_toml_dataclass.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 configuraptor-1.3.1/tests/test_toml_existing.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 configuraptor-1.3.1/tests/test_toml_typedconfig_class.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.3.1/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.3.1/LICENSE.txt
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 configuraptor-1.3.1/README.md
--rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 configuraptor-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 configuraptor-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     4642 2020-02-02 00:00:00.000000 configuraptor-1.3.2/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.3.2/coverage.svg
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 configuraptor-1.3.2/.github/workflows/su6.yml
+-rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.3.2/_static/configuraptor_circle.png
+-rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.3.2/_static/configuraptor_original.jpeg
+-rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.3.2/_static/configuraptor_round.png
+-rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.3.2/_static/configuraptor_transparent.png
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 configuraptor-1.3.2/examples/ages.toml
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 configuraptor-1.3.2/examples/dataclass.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.3.2/examples/example_from_readme.json
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 configuraptor-1.3.2/examples/example_from_readme.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 configuraptor-1.3.2/examples/example_from_readme.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.3.2/examples/example_from_readme.yaml
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 configuraptor-1.3.2/examples/existing_instance.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 configuraptor-1.3.2/examples/main.py
+-rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 configuraptor-1.3.2/examples/readme.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 configuraptor-1.3.2/examples/singleton.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.3.2/examples/typedconfig_class.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_31a2a1dc9b603870___init___py.html
+-rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_47560703719c1d9e___about___py.html
+-rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_47560703719c1d9e___init___py.html
+-rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_47560703719c1d9e_cls_py.html
+-rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_47560703719c1d9e_core_py.html
+-rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_47560703719c1d9e_errors_py.html
+-rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_47560703719c1d9e_helpers_py.html
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_47560703719c1d9e_main_py.html
+-rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_47560703719c1d9e_singleton_py.html
+-rw-r--r--   0        0        0    13203 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_6c7dc8b73849fb97___init___py.html
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_6c7dc8b73849fb97__types_py.html
+-rw-r--r--   0        0        0     9079 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html
+-rw-r--r--   0        0        0     8566 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html
+-rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40___about___py.html
+-rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40___init___py.html
+-rw-r--r--   0        0        0    10338 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40_cls_py.html
+-rw-r--r--   0        0        0   124666 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40_core_py.html
+-rw-r--r--   0        0        0    19533 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40_errors_py.html
+-rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html
+-rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     7414 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.3.2/pytest_examples/empty.toml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.3.2/pytest_examples/example.json
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configuraptor-1.3.2/pytest_examples/example.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.3.2/pytest_examples/example.yaml
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.3.2/pytest_examples/some.toml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.3.2/pytest_examples/with_dict_of_custom.toml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.3.2/pytest_examples/with_multiple_toplevel_keys.toml
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/__about__.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/__init__.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/cls.py
+-rw-r--r--   0        0        0    15026 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/core.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/errors.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/py.typed
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/singleton.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/loaders/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/loaders/_types.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/loaders/loaders_310.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/loaders/loaders_311.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/loaders/loaders_shared.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/loaders/py.typed
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.3.2/tests/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.3.2/tests/constants.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.3.2/tests/test_about.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 configuraptor-1.3.2/tests/test_core.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.3.2/tests/test_json_yaml.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 configuraptor-1.3.2/tests/test_mypy.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.3.2/tests/test_singleton.py
+-rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 configuraptor-1.3.2/tests/test_toml_basic.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 configuraptor-1.3.2/tests/test_toml_dataclass.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 configuraptor-1.3.2/tests/test_toml_existing.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 configuraptor-1.3.2/tests/test_toml_typedconfig_class.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.3.2/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.3.2/LICENSE.txt
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 configuraptor-1.3.2/README.md
+-rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 configuraptor-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 configuraptor-1.3.2/PKG-INFO
```

### Comparing `configuraptor-1.3.1/CHANGELOG.md` & `configuraptor-1.3.2/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.3.2 (2023-06-15)
+### Documentation
+* **examples:** Added more examples ([`884d11a`](https://github.com/trialandsuccess/configuraptor/commit/884d11a3f77836de907772237f58e723e5b7995b))
+* **examples:** Added more example code for the `basic` category ([`9782442`](https://github.com/trialandsuccess/configuraptor/commit/97824420e187d2ad01f597b4d458a55c535bb512))
+* **examples:** Started on providing more examples ([`ca84ecb`](https://github.com/trialandsuccess/configuraptor/commit/ca84ecbbc755108a35dabb9f9395d78f68b13b11))
+
 ## v1.3.1 (2023-06-15)
 ### Fix
 * **mypy:** `Type[C] | C` confused mypy so `load_into` (officially) only supports classes (not instances) now. ([`cd1c45e`](https://github.com/trialandsuccess/configuraptor/commit/cd1c45eae4c1fea0d7b9fa127a21655ae1c065b2))
 
 ## v1.3.0 (2023-06-14)
 ### Feature
 * **strict:** Allow strict=False for load_into to ignore types (not recommended) ([`16853bb`](https://github.com/trialandsuccess/configuraptor/commit/16853bb62b88c229ca0d9487692f9688b504bcf2))
```

### Comparing `configuraptor-1.3.1/coverage.svg` & `configuraptor-1.3.2/coverage.svg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/_static/configuraptor_circle.png` & `configuraptor-1.3.2/_static/configuraptor_circle.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/_static/configuraptor_original.jpeg` & `configuraptor-1.3.2/_static/configuraptor_original.jpeg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/_static/configuraptor_round.png` & `configuraptor-1.3.2/_static/configuraptor_round.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/_static/configuraptor_transparent.png` & `configuraptor-1.3.2/_static/configuraptor_transparent.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/examples/dataclass.py` & `configuraptor-1.3.2/examples/typedconfig_class.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 """
-Example with dataclasses
+Example with basic classes
 """
-from dataclasses import dataclass, field
 
-from configuraptor import load_into
+from configuraptor import TypedConfig
 
 
-@dataclass
-class Two:
+class AbsHasName(TypedConfig):
     name: str
+
+
+class Two(AbsHasName):
     some_str: str
     some_int: int
-    include: list[str] = field(default_factory=list) # <- not required in config file since it has a default value
 
     def __repr__(self) -> str:
         return f"{self.name=} {self.some_str=} {self.some_int=}"
 
 
-@dataclass
-class Simple:
-    name: str
+class Simple(AbsHasName):
     two: Two
 
     def __repr__(self) -> str:
         return f"{self.name=} {self.two=}"
 
 
 def main() -> None:
     data = {"simple": {"name": "Steve", "two": {"name": "Alex", "some_str": "string", "some_int": 30}}}
 
-    simple = load_into(Simple, data)
+    simple = Simple.load(data)
     two = simple.two
     print(simple, two)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `configuraptor-1.3.1/examples/example_from_docs.py` & `configuraptor-1.3.2/examples/example_from_readme.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 class Config:
     name: str
     reference: SomeRegularClass
 
 
 if __name__ == '__main__':
-    my_config = load_into(Config, "example_from_docs.json")
+    my_config = load_into(Config, "example_from_readme.json")
 
     print(my_config.name)
     # Hello World!
     print(my_config.reference.numbers)
     # [41, 43]
 
 
@@ -36,13 +36,13 @@
 
 class OtherConfig(TypedConfig):
     name: str
     reference: SomeRegularClass
 
 
 if __name__ == '__main__':
-    my_config = OtherConfig.load("example_from_docs.json")
+    my_config = OtherConfig.load("example_from_readme.json")
 
     print(my_config.name)
     # Hello World!
     print(my_config.reference.numbers)
     # [41, 43]
```

### Comparing `configuraptor-1.3.1/examples/main.py` & `configuraptor-1.3.2/examples/main.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/coverage_html.js` & `configuraptor-1.3.2/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/d_31a2a1dc9b603870___init___py.html` & `configuraptor-1.3.2/htmlcov/d_31a2a1dc9b603870___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html` & `configuraptor-1.3.2/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html` & `configuraptor-1.3.2/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/d_47560703719c1d9e___about___py.html` & `configuraptor-1.3.2/htmlcov/d_47560703719c1d9e___about___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/d_47560703719c1d9e___init___py.html` & `configuraptor-1.3.2/htmlcov/d_47560703719c1d9e___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/d_47560703719c1d9e_cls_py.html` & `configuraptor-1.3.2/htmlcov/d_47560703719c1d9e_cls_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/d_47560703719c1d9e_core_py.html` & `configuraptor-1.3.2/htmlcov/d_47560703719c1d9e_core_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/d_47560703719c1d9e_errors_py.html` & `configuraptor-1.3.2/htmlcov/d_47560703719c1d9e_errors_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/d_47560703719c1d9e_helpers_py.html` & `configuraptor-1.3.2/htmlcov/d_47560703719c1d9e_helpers_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/d_47560703719c1d9e_main_py.html` & `configuraptor-1.3.2/htmlcov/d_47560703719c1d9e_main_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/d_47560703719c1d9e_singleton_py.html` & `configuraptor-1.3.2/htmlcov/d_47560703719c1d9e_singleton_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/d_6c7dc8b73849fb97___init___py.html` & `configuraptor-1.3.2/htmlcov/d_6c7dc8b73849fb97___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/d_6c7dc8b73849fb97__types_py.html` & `configuraptor-1.3.2/htmlcov/d_6c7dc8b73849fb97__types_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html` & `configuraptor-1.3.2/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html` & `configuraptor-1.3.2/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html` & `configuraptor-1.3.2/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40___about___py.html` & `configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40___about___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40___init___py.html` & `configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40_cls_py.html` & `configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40_cls_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40_core_py.html` & `configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40_core_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40_errors_py.html` & `configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40_errors_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html` & `configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html` & `configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/favicon_32.png` & `configuraptor-1.3.2/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/index.html` & `configuraptor-1.3.2/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/keybd_closed.png` & `configuraptor-1.3.2/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/keybd_open.png` & `configuraptor-1.3.2/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/status.json` & `configuraptor-1.3.2/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/htmlcov/style.css` & `configuraptor-1.3.2/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/pytest_examples/some.toml` & `configuraptor-1.3.2/pytest_examples/some.toml`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/src/configuraptor/__init__.py` & `configuraptor-1.3.2/src/configuraptor/__init__.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/src/configuraptor/cls.py` & `configuraptor-1.3.2/src/configuraptor/cls.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 class TypedConfig:
     """
     Can be used instead of load_into.
     """
 
     @classmethod
-    def load(cls: typing.Type[C], data: T_data, key: str = None, init: dict[str, typing.Any] = None) -> C:
+    def load(
+        cls: typing.Type[C], data: T_data, key: str = None, init: dict[str, typing.Any] = None, strict: bool = True
+    ) -> C:
         """
         Load a class' config values from the config file.
 
         SomeClass.load(data, ...) = load_into(SomeClass, data, ...).
         """
-        return load_into(cls, data, key=key, init=init)
+        return load_into(cls, data, key=key, init=init, strict=strict)
```

### Comparing `configuraptor-1.3.1/src/configuraptor/core.py` & `configuraptor-1.3.2/src/configuraptor/core.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/src/configuraptor/errors.py` & `configuraptor-1.3.2/src/configuraptor/errors.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/src/configuraptor/singleton.py` & `configuraptor-1.3.2/src/configuraptor/singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/src/configuraptor/loaders/__init__.py` & `configuraptor-1.3.2/src/configuraptor/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/tests/test_core.py` & `configuraptor-1.3.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/tests/test_json_yaml.py` & `configuraptor-1.3.2/tests/test_json_yaml.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/tests/test_singleton.py` & `configuraptor-1.3.2/tests/test_singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/tests/test_toml_basic.py` & `configuraptor-1.3.2/tests/test_toml_basic.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/tests/test_toml_dataclass.py` & `configuraptor-1.3.2/tests/test_toml_dataclass.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/tests/test_toml_existing.py` & `configuraptor-1.3.2/tests/test_toml_existing.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/tests/test_toml_typedconfig_class.py` & `configuraptor-1.3.2/tests/test_toml_typedconfig_class.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/LICENSE.txt` & `configuraptor-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/README.md` & `configuraptor-1.3.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -41,29 +41,31 @@
 ```
 
 ## Usage
 
 Configuraptor can be used to load your config files into structured Python classes.
 
 ```toml
-# example_from_docs.toml
+# examples/example_from_readme.toml
 [config]
 name = "Hello World!"
 
 [config.reference]
 number = 42
 numbers = [41, 43]
 string = "42"
 ```
 
 Could be loaded into Python classes using the following code:
+
 ```python
-# example_from_docs.py
+# examples/example_from_readme.py
 from configuraptor import load_into, TypedConfig
 
+
 ######################
 # with basic classes #
 ######################
 
 class SomeRegularClass:
     number: int
     numbers: list[int]
@@ -72,15 +74,15 @@
 
 class Config:
     name: str
     reference: SomeRegularClass
 
 
 if __name__ == '__main__':
-    my_config = load_into(Config, "example_from_docs.toml")  # or .json, .yaml
+    my_config = load_into(Config, "example_from_readme.toml")  # or .json, .yaml
 
     print(my_config.name)
     # Hello World!
     print(my_config.reference.numbers)
     # [41, 43]
 
 
@@ -96,23 +98,23 @@
 
 class OtherConfig(TypedConfig):
     name: str
     reference: SomeRegularClass
 
 
 if __name__ == '__main__':
-    my_config = OtherConfig.load("example_from_docs.toml")  # or .json, .yaml
+    my_config = OtherConfig.load("example_from_readme.toml")  # or .json, .yaml
 
     print(my_config.name)
     # Hello World!
     print(my_config.reference.numbers)
     # [41, 43]
 ```
 
-More examples will be available soon.
+More examples can be round in [examples](https://github.com/trialandsuccess/configuraptor/blob/master/examples).
 
 ## License
 
 `configuraptor` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
 
 ## Changelog
```

### Comparing `configuraptor-1.3.1/pyproject.toml` & `configuraptor-1.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.1/PKG-INFO` & `configuraptor-1.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configuraptor
-Version: 1.3.1
+Version: 1.3.2
 Summary: Load toml/yaml/json config files into classes for a typed config (type hinting etc.)
 Project-URL: Documentation, https://github.com/trialandsuccess/configuraptor#readme
 Project-URL: Issues, https://github.com/trialandsuccess/configuraptor/issues
 Project-URL: Source, https://github.com/trialandsuccess/configuraptor
 Author-email: Robin van der Noord <robin@trialandsuccess.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -69,29 +69,31 @@
 ```
 
 ## Usage
 
 Configuraptor can be used to load your config files into structured Python classes.
 
 ```toml
-# example_from_docs.toml
+# examples/example_from_readme.toml
 [config]
 name = "Hello World!"
 
 [config.reference]
 number = 42
 numbers = [41, 43]
 string = "42"
 ```
 
 Could be loaded into Python classes using the following code:
+
 ```python
-# example_from_docs.py
+# examples/example_from_readme.py
 from configuraptor import load_into, TypedConfig
 
+
 ######################
 # with basic classes #
 ######################
 
 class SomeRegularClass:
     number: int
     numbers: list[int]
@@ -100,15 +102,15 @@
 
 class Config:
     name: str
     reference: SomeRegularClass
 
 
 if __name__ == '__main__':
-    my_config = load_into(Config, "example_from_docs.toml")  # or .json, .yaml
+    my_config = load_into(Config, "example_from_readme.toml")  # or .json, .yaml
 
     print(my_config.name)
     # Hello World!
     print(my_config.reference.numbers)
     # [41, 43]
 
 
@@ -124,23 +126,23 @@
 
 class OtherConfig(TypedConfig):
     name: str
     reference: SomeRegularClass
 
 
 if __name__ == '__main__':
-    my_config = OtherConfig.load("example_from_docs.toml")  # or .json, .yaml
+    my_config = OtherConfig.load("example_from_readme.toml")  # or .json, .yaml
 
     print(my_config.name)
     # Hello World!
     print(my_config.reference.numbers)
     # [41, 43]
 ```
 
-More examples will be available soon.
+More examples can be round in [examples](https://github.com/trialandsuccess/configuraptor/blob/master/examples).
 
 ## License
 
 `configuraptor` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
 
 ## Changelog
```

