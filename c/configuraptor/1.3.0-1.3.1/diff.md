# Comparing `tmp/configuraptor-1.3.0.tar.gz` & `tmp/configuraptor-1.3.1.tar.gz`

## Comparing `configuraptor-1.3.0.tar` & `configuraptor-1.3.1.tar`

### file list

```diff
@@ -1,81 +1,83 @@
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 configuraptor-1.3.0/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.3.0/coverage.svg
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 configuraptor-1.3.0/.github/workflows/su6.yml
--rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.3.0/_static/configuraptor_circle.png
--rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.3.0/_static/configuraptor_original.jpeg
--rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.3.0/_static/configuraptor_round.png
--rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.3.0/_static/configuraptor_transparent.png
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 configuraptor-1.3.0/examples/dataclass.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.3.0/examples/example_from_docs.json
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 configuraptor-1.3.0/examples/example_from_docs.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 configuraptor-1.3.0/examples/example_from_docs.toml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.3.0/examples/example_from_docs.yaml
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 configuraptor-1.3.0/examples/main.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 configuraptor-1.3.0/examples/singleton.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.3.0/examples/typedconfig_class.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_31a2a1dc9b603870___init___py.html
--rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_47560703719c1d9e___about___py.html
--rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_47560703719c1d9e___init___py.html
--rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_47560703719c1d9e_cls_py.html
--rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_47560703719c1d9e_core_py.html
--rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_47560703719c1d9e_errors_py.html
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_47560703719c1d9e_helpers_py.html
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_47560703719c1d9e_main_py.html
--rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_47560703719c1d9e_singleton_py.html
--rw-r--r--   0        0        0    13203 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_6c7dc8b73849fb97___init___py.html
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_6c7dc8b73849fb97__types_py.html
--rw-r--r--   0        0        0     9079 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html
--rw-r--r--   0        0        0     8566 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html
--rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40___about___py.html
--rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40___init___py.html
--rw-r--r--   0        0        0    10338 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40_cls_py.html
--rw-r--r--   0        0        0   124666 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40_core_py.html
--rw-r--r--   0        0        0    19533 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40_errors_py.html
--rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html
--rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     7414 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.3.0/htmlcov/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.3.0/pytest_examples/empty.toml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.3.0/pytest_examples/example.json
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configuraptor-1.3.0/pytest_examples/example.toml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.3.0/pytest_examples/example.yaml
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.3.0/pytest_examples/some.toml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.3.0/pytest_examples/with_dict_of_custom.toml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.3.0/pytest_examples/with_multiple_toplevel_keys.toml
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.3.0/src/configuraptor/__about__.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 configuraptor-1.3.0/src/configuraptor/__init__.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 configuraptor-1.3.0/src/configuraptor/cls.py
--rw-r--r--   0        0        0    14707 2020-02-02 00:00:00.000000 configuraptor-1.3.0/src/configuraptor/core.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 configuraptor-1.3.0/src/configuraptor/errors.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.3.0/src/configuraptor/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.3.0/src/configuraptor/py.typed
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 configuraptor-1.3.0/src/configuraptor/singleton.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 configuraptor-1.3.0/src/configuraptor/loaders/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 configuraptor-1.3.0/src/configuraptor/loaders/_types.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 configuraptor-1.3.0/src/configuraptor/loaders/loaders_310.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 configuraptor-1.3.0/src/configuraptor/loaders/loaders_311.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 configuraptor-1.3.0/src/configuraptor/loaders/loaders_shared.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.3.0/tests/__init__.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.3.0/tests/constants.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.3.0/tests/test_about.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 configuraptor-1.3.0/tests/test_core.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.3.0/tests/test_json_yaml.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.3.0/tests/test_singleton.py
--rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 configuraptor-1.3.0/tests/test_toml_basic.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 configuraptor-1.3.0/tests/test_toml_dataclass.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 configuraptor-1.3.0/tests/test_toml_existing.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 configuraptor-1.3.0/tests/test_toml_typedconfig_class.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.3.0/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.3.0/LICENSE.txt
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 configuraptor-1.3.0/README.md
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 configuraptor-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 configuraptor-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 configuraptor-1.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.3.1/coverage.svg
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 configuraptor-1.3.1/.github/workflows/su6.yml
+-rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.3.1/_static/configuraptor_circle.png
+-rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.3.1/_static/configuraptor_original.jpeg
+-rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.3.1/_static/configuraptor_round.png
+-rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.3.1/_static/configuraptor_transparent.png
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 configuraptor-1.3.1/examples/dataclass.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.3.1/examples/example_from_docs.json
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 configuraptor-1.3.1/examples/example_from_docs.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 configuraptor-1.3.1/examples/example_from_docs.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.3.1/examples/example_from_docs.yaml
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 configuraptor-1.3.1/examples/main.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 configuraptor-1.3.1/examples/singleton.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.3.1/examples/typedconfig_class.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_31a2a1dc9b603870___init___py.html
+-rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_47560703719c1d9e___about___py.html
+-rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_47560703719c1d9e___init___py.html
+-rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_47560703719c1d9e_cls_py.html
+-rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_47560703719c1d9e_core_py.html
+-rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_47560703719c1d9e_errors_py.html
+-rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_47560703719c1d9e_helpers_py.html
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_47560703719c1d9e_main_py.html
+-rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_47560703719c1d9e_singleton_py.html
+-rw-r--r--   0        0        0    13203 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_6c7dc8b73849fb97___init___py.html
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_6c7dc8b73849fb97__types_py.html
+-rw-r--r--   0        0        0     9079 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html
+-rw-r--r--   0        0        0     8566 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html
+-rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40___about___py.html
+-rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40___init___py.html
+-rw-r--r--   0        0        0    10338 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40_cls_py.html
+-rw-r--r--   0        0        0   124666 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40_core_py.html
+-rw-r--r--   0        0        0    19533 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40_errors_py.html
+-rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html
+-rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     7414 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.3.1/htmlcov/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.3.1/pytest_examples/empty.toml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.3.1/pytest_examples/example.json
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configuraptor-1.3.1/pytest_examples/example.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.3.1/pytest_examples/example.yaml
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.3.1/pytest_examples/some.toml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.3.1/pytest_examples/with_dict_of_custom.toml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.3.1/pytest_examples/with_multiple_toplevel_keys.toml
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/__about__.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/__init__.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/cls.py
+-rw-r--r--   0        0        0    15026 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/core.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/errors.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/py.typed
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/singleton.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/loaders/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/loaders/_types.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/loaders/loaders_310.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/loaders/loaders_311.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/loaders/loaders_shared.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.3.1/src/configuraptor/loaders/py.typed
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.3.1/tests/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.3.1/tests/constants.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.3.1/tests/test_about.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 configuraptor-1.3.1/tests/test_core.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.3.1/tests/test_json_yaml.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 configuraptor-1.3.1/tests/test_mypy.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.3.1/tests/test_singleton.py
+-rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 configuraptor-1.3.1/tests/test_toml_basic.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 configuraptor-1.3.1/tests/test_toml_dataclass.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 configuraptor-1.3.1/tests/test_toml_existing.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 configuraptor-1.3.1/tests/test_toml_typedconfig_class.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.3.1/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 configuraptor-1.3.1/README.md
+-rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 configuraptor-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 configuraptor-1.3.1/PKG-INFO
```

### Comparing `configuraptor-1.3.0/CHANGELOG.md` & `configuraptor-1.3.1/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.3.1 (2023-06-15)
+### Fix
+* **mypy:** `Type[C] | C` confused mypy so `load_into` (officially) only supports classes (not instances) now. ([`cd1c45e`](https://github.com/trialandsuccess/configuraptor/commit/cd1c45eae4c1fea0d7b9fa127a21655ae1c065b2))
+
 ## v1.3.0 (2023-06-14)
 ### Feature
 * **strict:** Allow strict=False for load_into to ignore types (not recommended) ([`16853bb`](https://github.com/trialandsuccess/configuraptor/commit/16853bb62b88c229ca0d9487692f9688b504bcf2))
 
 ## v1.2.1 (2023-06-14)
 ### Fix
 * **lib:** Exposed wrong method ([`d57b6df`](https://github.com/trialandsuccess/configuraptor/commit/d57b6df10e85693729ffb87f4ec36a7a932e1a3e))
```

### Comparing `configuraptor-1.3.0/coverage.svg` & `configuraptor-1.3.1/coverage.svg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/_static/configuraptor_circle.png` & `configuraptor-1.3.1/_static/configuraptor_circle.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/_static/configuraptor_original.jpeg` & `configuraptor-1.3.1/_static/configuraptor_original.jpeg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/_static/configuraptor_round.png` & `configuraptor-1.3.1/_static/configuraptor_round.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/_static/configuraptor_transparent.png` & `configuraptor-1.3.1/_static/configuraptor_transparent.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/examples/dataclass.py` & `configuraptor-1.3.1/examples/dataclass.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/examples/example_from_docs.py` & `configuraptor-1.3.1/examples/example_from_docs.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/examples/main.py` & `configuraptor-1.3.1/examples/main.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/examples/typedconfig_class.py` & `configuraptor-1.3.1/examples/typedconfig_class.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/coverage_html.js` & `configuraptor-1.3.1/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/d_31a2a1dc9b603870___init___py.html` & `configuraptor-1.3.1/htmlcov/d_31a2a1dc9b603870___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html` & `configuraptor-1.3.1/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html` & `configuraptor-1.3.1/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/d_47560703719c1d9e___about___py.html` & `configuraptor-1.3.1/htmlcov/d_47560703719c1d9e___about___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/d_47560703719c1d9e___init___py.html` & `configuraptor-1.3.1/htmlcov/d_47560703719c1d9e___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/d_47560703719c1d9e_cls_py.html` & `configuraptor-1.3.1/htmlcov/d_47560703719c1d9e_cls_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/d_47560703719c1d9e_core_py.html` & `configuraptor-1.3.1/htmlcov/d_47560703719c1d9e_core_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/d_47560703719c1d9e_errors_py.html` & `configuraptor-1.3.1/htmlcov/d_47560703719c1d9e_errors_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/d_47560703719c1d9e_helpers_py.html` & `configuraptor-1.3.1/htmlcov/d_47560703719c1d9e_helpers_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/d_47560703719c1d9e_main_py.html` & `configuraptor-1.3.1/htmlcov/d_47560703719c1d9e_main_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/d_47560703719c1d9e_singleton_py.html` & `configuraptor-1.3.1/htmlcov/d_47560703719c1d9e_singleton_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/d_6c7dc8b73849fb97___init___py.html` & `configuraptor-1.3.1/htmlcov/d_6c7dc8b73849fb97___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/d_6c7dc8b73849fb97__types_py.html` & `configuraptor-1.3.1/htmlcov/d_6c7dc8b73849fb97__types_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html` & `configuraptor-1.3.1/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html` & `configuraptor-1.3.1/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html` & `configuraptor-1.3.1/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40___about___py.html` & `configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40___about___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40___init___py.html` & `configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40_cls_py.html` & `configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40_cls_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40_core_py.html` & `configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40_core_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40_errors_py.html` & `configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40_errors_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html` & `configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html` & `configuraptor-1.3.1/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/favicon_32.png` & `configuraptor-1.3.1/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/index.html` & `configuraptor-1.3.1/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/keybd_closed.png` & `configuraptor-1.3.1/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/keybd_open.png` & `configuraptor-1.3.1/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/status.json` & `configuraptor-1.3.1/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/htmlcov/style.css` & `configuraptor-1.3.1/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/pytest_examples/some.toml` & `configuraptor-1.3.1/pytest_examples/some.toml`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/src/configuraptor/cls.py` & `configuraptor-1.3.1/src/configuraptor/cls.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/src/configuraptor/core.py` & `configuraptor-1.3.1/src/configuraptor/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,36 +256,36 @@
         if _key in data:
             value: typing.Any = data[_key]  # value can change so define it as any instead of T
             if is_parameterized(_type):
                 origin = typing.get_origin(_type)
                 arguments = typing.get_args(_type)
                 if origin is list and arguments and is_custom_class(arguments[0]):
                     subtype = arguments[0]
-                    value = [load_into_recurse(subtype, subvalue) for subvalue in value]
+                    value = [_load_into_recurse(subtype, subvalue) for subvalue in value]
 
                 elif origin is dict and arguments and is_custom_class(arguments[1]):
                     # e.g. dict[str, Point]
                     subkeytype, subvaluetype = arguments
                     # subkey(type) is not a custom class, so don't try to convert it:
-                    value = {subkey: load_into_recurse(subvaluetype, subvalue) for subkey, subvalue in value.items()}
+                    value = {subkey: _load_into_recurse(subvaluetype, subvalue) for subkey, subvalue in value.items()}
                 # elif origin is dict:
                 # keep data the same
                 elif origin is typing.Union and arguments:
                     for arg in arguments:
                         if is_custom_class(arg):
-                            value = load_into_recurse(arg, value)
+                            value = _load_into_recurse(arg, value)
                         else:
                             # print(_type, arg, value)
                             ...
 
                 # todo: other parameterized/unions/typing.Optional
 
             elif is_custom_class(_type):
                 # type must be C (custom class) at this point
-                value = load_into_recurse(
+                value = _load_into_recurse(
                     # make mypy and pycharm happy by telling it _type is of type C...
                     # actually just passing _type as first arg!
                     typing.cast(Type_C[typing.Any], _type),
                     value,
                 )
 
         elif _key in cls.__dict__:
@@ -347,15 +347,15 @@
     to_load = load_recursive(cls, to_load, annotations)
     if strict:
         to_load = ensure_types(to_load, annotations)
 
     return to_load
 
 
-def load_into_recurse(
+def _load_into_recurse(
     cls: typing.Type[C],
     data: dict[str, typing.Any],
     init: dict[str, typing.Any] = None,
     strict: bool = True,
 ) -> C:
     """
     Loads an instance of `cls` filled with `data`.
@@ -379,15 +379,15 @@
         inst = cls(**init)
         to_load = check_and_convert_data(cls, data, inst.__dict__.keys(), strict=strict)
         inst.__dict__.update(**to_load)
 
     return inst
 
 
-def load_into_existing(
+def _load_into_instance(
     inst: C,
     cls: typing.Type[C],
     data: dict[str, typing.Any],
     init: dict[str, typing.Any] = None,
     strict: bool = True,
 ) -> C:
     """
@@ -415,15 +415,15 @@
     init: dict[str, typing.Any] = None,
     strict: bool = True,
 ) -> C:
     """
     Shortcut for _load_data + load_into_recurse.
     """
     to_load = _load_data(data, key, cls.__name__)
-    return load_into_recurse(cls, to_load, init=init, strict=strict)
+    return _load_into_recurse(cls, to_load, init=init, strict=strict)
 
 
 def load_into_instance(
     inst: C,
     data: T_data,
     /,
     key: str = None,
@@ -431,35 +431,39 @@
     strict: bool = True,
 ) -> C:
     """
     Shortcut for _load_data + load_into_existing.
     """
     cls = inst.__class__
     to_load = _load_data(data, key, cls.__name__)
-    return load_into_existing(inst, cls, to_load, init=init, strict=strict)
+    return _load_into_instance(inst, cls, to_load, init=init, strict=strict)
 
 
 def load_into(
-    cls: typing.Type[C] | C,
+    cls: typing.Type[C],
     data: T_data,
     /,
     key: str = None,
     init: dict[str, typing.Any] = None,
     strict: bool = True,
 ) -> C:
     """
     Load your config into a class (instance).
 
+    Supports both a class or an instance as first argument, but that's hard to explain to mypy, so officially only
+    classes are supported, and if you want to `load_into` an instance, you should use `load_into_instance`.
+
     Args:
         cls: either a class or an existing instance of that class.
         data: can be a dictionary or a path to a file to load (as pathlib.Path or str)
         key: optional (nested) dictionary key to load data from (e.g. 'tool.su6.specific')
         init: optional data to pass to your cls' __init__ method (only if cls is not an instance already)
         strict: enable type checks or allow anything?
 
     """
     if not isinstance(cls, type):
+        # would not be supported according to mypy, but you can still load_into(instance)
         return load_into_instance(cls, data, key=key, init=init, strict=strict)
 
     # make mypy and pycharm happy by telling it cls is of type C and not just 'type'
-    _cls = typing.cast(typing.Type[C], cls)
-    return load_into_class(_cls, data, key=key, init=init, strict=strict)
+    # _cls = typing.cast(typing.Type[C], cls)
+    return load_into_class(cls, data, key=key, init=init, strict=strict)
```

### Comparing `configuraptor-1.3.0/src/configuraptor/errors.py` & `configuraptor-1.3.1/src/configuraptor/errors.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/src/configuraptor/singleton.py` & `configuraptor-1.3.1/src/configuraptor/singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/src/configuraptor/loaders/__init__.py` & `configuraptor-1.3.1/src/configuraptor/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/tests/test_core.py` & `configuraptor-1.3.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/tests/test_json_yaml.py` & `configuraptor-1.3.1/tests/test_json_yaml.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/tests/test_singleton.py` & `configuraptor-1.3.1/tests/test_singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/tests/test_toml_basic.py` & `configuraptor-1.3.1/tests/test_toml_basic.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/tests/test_toml_dataclass.py` & `configuraptor-1.3.1/tests/test_toml_dataclass.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/tests/test_toml_existing.py` & `configuraptor-1.3.1/tests/test_toml_existing.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/tests/test_toml_typedconfig_class.py` & `configuraptor-1.3.1/tests/test_toml_typedconfig_class.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/LICENSE.txt` & `configuraptor-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/README.md` & `configuraptor-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.0/pyproject.toml` & `configuraptor-1.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 "configuraptor" = ["py.typed"]
 
 [project.optional-dependencies]
 dev = [
     "su6[all]",
     "hatch",
     "types-PyYAML",
+    "pytest-mypy-testing",
 ]
 
 [project.urls]
 Documentation = "https://github.com/trialandsuccess/configuraptor#readme"
 Issues = "https://github.com/trialandsuccess/configuraptor/issues"
 Source = "https://github.com/trialandsuccess/configuraptor"
```

### Comparing `configuraptor-1.3.0/PKG-INFO` & `configuraptor-1.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configuraptor
-Version: 1.3.0
+Version: 1.3.1
 Summary: Load toml/yaml/json config files into classes for a typed config (type hinting etc.)
 Project-URL: Documentation, https://github.com/trialandsuccess/configuraptor#readme
 Project-URL: Issues, https://github.com/trialandsuccess/configuraptor/issues
 Project-URL: Source, https://github.com/trialandsuccess/configuraptor
 Author-email: Robin van der Noord <robin@trialandsuccess.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: pyyaml
 Requires-Dist: tomlkit; python_version < '3.11'
 Requires-Dist: typeguard
 Provides-Extra: dev
 Requires-Dist: hatch; extra == 'dev'
+Requires-Dist: pytest-mypy-testing; extra == 'dev'
 Requires-Dist: su6[all]; extra == 'dev'
 Requires-Dist: types-pyyaml; extra == 'dev'
 Description-Content-Type: text/markdown
 
 <div align="center">
     <img 
         align="center"
```

