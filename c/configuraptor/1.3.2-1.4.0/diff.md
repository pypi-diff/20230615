# Comparing `tmp/configuraptor-1.3.2.tar.gz` & `tmp/configuraptor-1.4.0.tar.gz`

## Comparing `configuraptor-1.3.2.tar` & `configuraptor-1.4.0.tar`

### file list

```diff
@@ -1,86 +1,89 @@
--rw-r--r--   0        0        0     4642 2020-02-02 00:00:00.000000 configuraptor-1.3.2/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.3.2/coverage.svg
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 configuraptor-1.3.2/.github/workflows/su6.yml
--rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.3.2/_static/configuraptor_circle.png
--rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.3.2/_static/configuraptor_original.jpeg
--rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.3.2/_static/configuraptor_round.png
--rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.3.2/_static/configuraptor_transparent.png
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 configuraptor-1.3.2/examples/ages.toml
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 configuraptor-1.3.2/examples/dataclass.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.3.2/examples/example_from_readme.json
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 configuraptor-1.3.2/examples/example_from_readme.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 configuraptor-1.3.2/examples/example_from_readme.toml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.3.2/examples/example_from_readme.yaml
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 configuraptor-1.3.2/examples/existing_instance.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 configuraptor-1.3.2/examples/main.py
--rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 configuraptor-1.3.2/examples/readme.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 configuraptor-1.3.2/examples/singleton.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.3.2/examples/typedconfig_class.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_31a2a1dc9b603870___init___py.html
--rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_47560703719c1d9e___about___py.html
--rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_47560703719c1d9e___init___py.html
--rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_47560703719c1d9e_cls_py.html
--rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_47560703719c1d9e_core_py.html
--rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_47560703719c1d9e_errors_py.html
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_47560703719c1d9e_helpers_py.html
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_47560703719c1d9e_main_py.html
--rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_47560703719c1d9e_singleton_py.html
--rw-r--r--   0        0        0    13203 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_6c7dc8b73849fb97___init___py.html
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_6c7dc8b73849fb97__types_py.html
--rw-r--r--   0        0        0     9079 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html
--rw-r--r--   0        0        0     8566 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html
--rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40___about___py.html
--rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40___init___py.html
--rw-r--r--   0        0        0    10338 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40_cls_py.html
--rw-r--r--   0        0        0   124666 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40_core_py.html
--rw-r--r--   0        0        0    19533 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40_errors_py.html
--rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html
--rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     7414 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.3.2/htmlcov/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.3.2/pytest_examples/empty.toml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.3.2/pytest_examples/example.json
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configuraptor-1.3.2/pytest_examples/example.toml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.3.2/pytest_examples/example.yaml
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.3.2/pytest_examples/some.toml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.3.2/pytest_examples/with_dict_of_custom.toml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.3.2/pytest_examples/with_multiple_toplevel_keys.toml
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/__about__.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/__init__.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/cls.py
--rw-r--r--   0        0        0    15026 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/core.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/errors.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/py.typed
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/singleton.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/loaders/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/loaders/_types.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/loaders/loaders_310.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/loaders/loaders_311.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/loaders/loaders_shared.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.3.2/src/configuraptor/loaders/py.typed
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.3.2/tests/__init__.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.3.2/tests/constants.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.3.2/tests/test_about.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 configuraptor-1.3.2/tests/test_core.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.3.2/tests/test_json_yaml.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 configuraptor-1.3.2/tests/test_mypy.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.3.2/tests/test_singleton.py
--rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 configuraptor-1.3.2/tests/test_toml_basic.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 configuraptor-1.3.2/tests/test_toml_dataclass.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 configuraptor-1.3.2/tests/test_toml_existing.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 configuraptor-1.3.2/tests/test_toml_typedconfig_class.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.3.2/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.3.2/LICENSE.txt
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 configuraptor-1.3.2/README.md
--rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 configuraptor-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 configuraptor-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 configuraptor-1.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.4.0/coverage.svg
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 configuraptor-1.4.0/.github/workflows/su6.yml
+-rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.4.0/_static/configuraptor_circle.png
+-rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.4.0/_static/configuraptor_original.jpeg
+-rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.4.0/_static/configuraptor_round.png
+-rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.4.0/_static/configuraptor_transparent.png
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 configuraptor-1.4.0/examples/ages.toml
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 configuraptor-1.4.0/examples/dataclass.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.4.0/examples/example_from_readme.json
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 configuraptor-1.4.0/examples/example_from_readme.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 configuraptor-1.4.0/examples/example_from_readme.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.4.0/examples/example_from_readme.yaml
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 configuraptor-1.4.0/examples/existing_instance.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 configuraptor-1.4.0/examples/main.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 configuraptor-1.4.0/examples/postponed.py
+-rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 configuraptor-1.4.0/examples/readme.md
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 configuraptor-1.4.0/examples/singleton.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.4.0/examples/typedconfig_class.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/d_31a2a1dc9b603870___init___py.html
+-rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/d_47560703719c1d9e___about___py.html
+-rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/d_47560703719c1d9e___init___py.html
+-rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/d_47560703719c1d9e_cls_py.html
+-rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/d_47560703719c1d9e_core_py.html
+-rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/d_47560703719c1d9e_errors_py.html
+-rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/d_47560703719c1d9e_helpers_py.html
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/d_47560703719c1d9e_main_py.html
+-rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/d_47560703719c1d9e_singleton_py.html
+-rw-r--r--   0        0        0    13203 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/d_6c7dc8b73849fb97___init___py.html
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/d_6c7dc8b73849fb97__types_py.html
+-rw-r--r--   0        0        0     9079 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html
+-rw-r--r--   0        0        0     8566 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html
+-rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/d_eb75b6cf8f5eab40___about___py.html
+-rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/d_eb75b6cf8f5eab40___init___py.html
+-rw-r--r--   0        0        0    10338 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/d_eb75b6cf8f5eab40_cls_py.html
+-rw-r--r--   0        0        0   124666 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/d_eb75b6cf8f5eab40_core_py.html
+-rw-r--r--   0        0        0    19533 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/d_eb75b6cf8f5eab40_errors_py.html
+-rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html
+-rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     7414 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.4.0/htmlcov/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.4.0/pytest_examples/empty.toml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.4.0/pytest_examples/example.json
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configuraptor-1.4.0/pytest_examples/example.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.4.0/pytest_examples/example.yaml
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.4.0/pytest_examples/some.toml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.4.0/pytest_examples/with_dict_of_custom.toml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.4.0/pytest_examples/with_multiple_toplevel_keys.toml
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.4.0/src/configuraptor/__about__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 configuraptor-1.4.0/src/configuraptor/__init__.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 configuraptor-1.4.0/src/configuraptor/cls.py
+-rw-r--r--   0        0        0    15190 2020-02-02 00:00:00.000000 configuraptor-1.4.0/src/configuraptor/core.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 configuraptor-1.4.0/src/configuraptor/errors.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.4.0/src/configuraptor/helpers.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 configuraptor-1.4.0/src/configuraptor/postpone.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.4.0/src/configuraptor/py.typed
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 configuraptor-1.4.0/src/configuraptor/singleton.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 configuraptor-1.4.0/src/configuraptor/loaders/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 configuraptor-1.4.0/src/configuraptor/loaders/_types.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 configuraptor-1.4.0/src/configuraptor/loaders/loaders_310.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 configuraptor-1.4.0/src/configuraptor/loaders/loaders_311.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 configuraptor-1.4.0/src/configuraptor/loaders/loaders_shared.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.4.0/src/configuraptor/loaders/py.typed
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.4.0/tests/constants.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.4.0/tests/test_about.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 configuraptor-1.4.0/tests/test_core.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.4.0/tests/test_json_yaml.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 configuraptor-1.4.0/tests/test_mypy.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 configuraptor-1.4.0/tests/test_postponed.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.4.0/tests/test_singleton.py
+-rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 configuraptor-1.4.0/tests/test_toml_basic.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 configuraptor-1.4.0/tests/test_toml_dataclass.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 configuraptor-1.4.0/tests/test_toml_existing.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 configuraptor-1.4.0/tests/test_toml_typedconfig_class.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.4.0/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 configuraptor-1.4.0/README.md
+-rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 configuraptor-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 configuraptor-1.4.0/PKG-INFO
```

### Comparing `configuraptor-1.3.2/CHANGELOG.md` & `configuraptor-1.4.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.4.0 (2023-06-15)
+### Feature
+* **postpone:** Allow marking a field as `postponed` if you can't fill it in right away or from config (useful for cli tools with cli args) ([`1494000`](https://github.com/trialandsuccess/configuraptor/commit/1494000a0f373b83188f892c83e6c1bb5a7ae755))
+
 ## v1.3.2 (2023-06-15)
 ### Documentation
 * **examples:** Added more examples ([`884d11a`](https://github.com/trialandsuccess/configuraptor/commit/884d11a3f77836de907772237f58e723e5b7995b))
 * **examples:** Added more example code for the `basic` category ([`9782442`](https://github.com/trialandsuccess/configuraptor/commit/97824420e187d2ad01f597b4d458a55c535bb512))
 * **examples:** Started on providing more examples ([`ca84ecb`](https://github.com/trialandsuccess/configuraptor/commit/ca84ecbbc755108a35dabb9f9395d78f68b13b11))
 
 ## v1.3.1 (2023-06-15)
```

### Comparing `configuraptor-1.3.2/coverage.svg` & `configuraptor-1.4.0/coverage.svg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/_static/configuraptor_circle.png` & `configuraptor-1.4.0/_static/configuraptor_circle.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/_static/configuraptor_original.jpeg` & `configuraptor-1.4.0/_static/configuraptor_original.jpeg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/_static/configuraptor_round.png` & `configuraptor-1.4.0/_static/configuraptor_round.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/_static/configuraptor_transparent.png` & `configuraptor-1.4.0/_static/configuraptor_transparent.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/examples/dataclass.py` & `configuraptor-1.4.0/examples/dataclass.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/examples/example_from_readme.py` & `configuraptor-1.4.0/examples/example_from_readme.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,50 @@
-from configuraptor import load_into, TypedConfig
+from configuraptor import TypedConfig, load_into
 
 ######################
 # with basic classes #
 ######################
 
+
 class SomeRegularClass:
     number: int
     numbers: list[int]
     string: str
 
 
 class Config:
     name: str
     reference: SomeRegularClass
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     my_config = load_into(Config, "example_from_readme.json")
 
     print(my_config.name)
     # Hello World!
     print(my_config.reference.numbers)
     # [41, 43]
 
 
 ########################
 # alternative notation #
 ########################
 
+
 class SomeOtherRegularClass:
     number: int
     numbers: list[int]
     string: str
 
 
 class OtherConfig(TypedConfig):
     name: str
     reference: SomeRegularClass
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     my_config = OtherConfig.load("example_from_readme.json")
 
     print(my_config.name)
     # Hello World!
     print(my_config.reference.numbers)
     # [41, 43]
```

### Comparing `configuraptor-1.3.2/examples/main.py` & `configuraptor-1.4.0/examples/main.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/examples/readme.md` & `configuraptor-1.4.0/examples/readme.md`

 * *Files 14% similar despite different names*

```diff
@@ -202,8 +202,43 @@
 
 # only calling .update on `config` will also update `second_config`:
 config.update(string="second string", number=1)
 # config=self.string='second string', self.number=1
 # second_config=self.string='second string', self.number=1
 ```
 
-In this example, both `config` and `second_config` contain exactly the same data at any point in time.
+In this example, both `config` and `second_config` contain exactly the same data at any point in time.
+
+## Postponed Fields
+
+In some cases, a config key you want to define does not exist yet when calling `load_into`. When there is no default or
+matching value in the config file, which could be the case in cli tools where you NEED the value from the user,
+`postponed()` can be used.
+
+```python
+from configuraptor import Singleton, TypedConfig, load_into, postpone
+
+
+class Later(TypedConfig, Singleton):
+    field: str  # instant
+    other_field: str = postpone()
+
+    def update(self):
+        self.other_field = "usable"
+
+
+config = load_into(
+    Later,
+    {
+        "later": dict(field="instant")
+        # no other_field yet!
+    },
+)
+
+print(config.field)  # will work
+# config.other_field  # will give an error if you try to use it here!
+
+config.update()  # fill in other_field some way or another
+print(config.other_field)  # works now!
+
+```
+
```

### Comparing `configuraptor-1.3.2/examples/singleton.py` & `configuraptor-1.4.0/examples/singleton.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,22 +9,17 @@
         self.string = string
         self.number = number
 
     def __repr__(self):
         return f"{self.string=}, {self.number=}"
 
 
-config = load_into(MyConfig, {
-    "my_config": dict(
-        string="initial string",
-        number=0
-    )
-})
+config = load_into(MyConfig, {"my_config": dict(string="initial string", number=0)})
 
 second_config = MyConfig()  # note: no arguments required!
 print(f"{config=}\n{second_config=}")
 # config=self.string='initial string', self.number=0
 # second_config=self.string='initial string', self.number=0
 
 config.update(string="second string", number=1)
 # config=self.string='second string', self.number=1
-# second_config=self.string='second string', self.number=1
+# second_config=self.string='second string', self.number=1
```

### Comparing `configuraptor-1.3.2/examples/typedconfig_class.py` & `configuraptor-1.4.0/examples/typedconfig_class.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/coverage_html.js` & `configuraptor-1.4.0/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/d_31a2a1dc9b603870___init___py.html` & `configuraptor-1.4.0/htmlcov/d_31a2a1dc9b603870___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html` & `configuraptor-1.4.0/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html` & `configuraptor-1.4.0/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/d_47560703719c1d9e___about___py.html` & `configuraptor-1.4.0/htmlcov/d_47560703719c1d9e___about___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/d_47560703719c1d9e___init___py.html` & `configuraptor-1.4.0/htmlcov/d_47560703719c1d9e___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/d_47560703719c1d9e_cls_py.html` & `configuraptor-1.4.0/htmlcov/d_47560703719c1d9e_cls_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/d_47560703719c1d9e_core_py.html` & `configuraptor-1.4.0/htmlcov/d_47560703719c1d9e_core_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/d_47560703719c1d9e_errors_py.html` & `configuraptor-1.4.0/htmlcov/d_47560703719c1d9e_errors_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/d_47560703719c1d9e_helpers_py.html` & `configuraptor-1.4.0/htmlcov/d_47560703719c1d9e_helpers_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/d_47560703719c1d9e_main_py.html` & `configuraptor-1.4.0/htmlcov/d_47560703719c1d9e_main_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/d_47560703719c1d9e_singleton_py.html` & `configuraptor-1.4.0/htmlcov/d_47560703719c1d9e_singleton_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/d_6c7dc8b73849fb97___init___py.html` & `configuraptor-1.4.0/htmlcov/d_6c7dc8b73849fb97___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/d_6c7dc8b73849fb97__types_py.html` & `configuraptor-1.4.0/htmlcov/d_6c7dc8b73849fb97__types_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html` & `configuraptor-1.4.0/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html` & `configuraptor-1.4.0/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html` & `configuraptor-1.4.0/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40___about___py.html` & `configuraptor-1.4.0/htmlcov/d_eb75b6cf8f5eab40___about___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40___init___py.html` & `configuraptor-1.4.0/htmlcov/d_eb75b6cf8f5eab40___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40_cls_py.html` & `configuraptor-1.4.0/htmlcov/d_eb75b6cf8f5eab40_cls_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40_core_py.html` & `configuraptor-1.4.0/htmlcov/d_eb75b6cf8f5eab40_core_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40_errors_py.html` & `configuraptor-1.4.0/htmlcov/d_eb75b6cf8f5eab40_errors_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html` & `configuraptor-1.4.0/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html` & `configuraptor-1.4.0/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/favicon_32.png` & `configuraptor-1.4.0/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/index.html` & `configuraptor-1.4.0/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/keybd_closed.png` & `configuraptor-1.4.0/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/keybd_open.png` & `configuraptor-1.4.0/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/status.json` & `configuraptor-1.4.0/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/htmlcov/style.css` & `configuraptor-1.4.0/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/pytest_examples/some.toml` & `configuraptor-1.4.0/pytest_examples/some.toml`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/src/configuraptor/cls.py` & `configuraptor-1.4.0/src/configuraptor/cls.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/src/configuraptor/core.py` & `configuraptor-1.4.0/src/configuraptor/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 from typeguard import TypeCheckError
 from typeguard import check_type as _check_type
 
 from . import loaders
 from .errors import ConfigErrorInvalidType, ConfigErrorMissingKey
 from .helpers import camel_to_snake
+from .postpone import Postponed
 
 # T is a reusable typevar
 T = typing.TypeVar("T")
 # t_typelike is anything that can be type hinted
 T_typelike: typing.TypeAlias = type | types.UnionType  # | typing.Union
 # t_data is anything that can be fed to _load_data
 T_data = str | Path | dict[str, typing.Any]
@@ -101,24 +102,30 @@
     Make sure all values in 'data' are in line with the ones stored in 'annotations'.
 
     If an annotated key in missing from data, it will be filled with None for convenience.
     """
     # custom object to use instead of None, since typing.Optional can be None!
     # cast to T to make mypy happy
     notfound = typing.cast(T, object())
+    postponed = Postponed()
 
     final: dict[str, T | None] = {}
     for key, _type in annotations.items():
         compare = data.get(key, notfound)
         if compare is notfound:  # pragma: nocover
             warnings.warn(
                 "This should not happen since " "`load_recursive` already fills `data` " "based on `annotations`"
             )
             # skip!
             continue
+
+        if compare is postponed:
+            # don't do anything with this item!
+            continue
+
         if not check_type(compare, _type):
             raise ConfigErrorInvalidType(key, value=compare, expected_type=_type)
 
         final[key] = compare
     return final
```

### Comparing `configuraptor-1.3.2/src/configuraptor/errors.py` & `configuraptor-1.4.0/src/configuraptor/errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -64,7 +64,16 @@
         """
         Custom error message based on dataclass values and calculated actual type.
         """
         return (
             f"Config key '{self.key}' had a value (`{self._value}`) with a type (`{self.actual_type}`) "
             f"that was not expected: `{self.expected_type}` is the required type."
         )
+
+
+@dataclass
+class IsPostponedError(ConfigError):
+    """
+    Error thrown when you try to access a 'postponed' property without filling its value first.
+    """
+
+    message: str = "This postponed property has not been filled yet!"
```

### Comparing `configuraptor-1.3.2/src/configuraptor/singleton.py` & `configuraptor-1.4.0/src/configuraptor/singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/src/configuraptor/loaders/__init__.py` & `configuraptor-1.4.0/src/configuraptor/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/tests/test_core.py` & `configuraptor-1.4.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/tests/test_json_yaml.py` & `configuraptor-1.4.0/tests/test_json_yaml.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/tests/test_singleton.py` & `configuraptor-1.4.0/tests/test_singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/tests/test_toml_basic.py` & `configuraptor-1.4.0/tests/test_toml_basic.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/tests/test_toml_dataclass.py` & `configuraptor-1.4.0/tests/test_toml_dataclass.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/tests/test_toml_existing.py` & `configuraptor-1.4.0/tests/test_toml_existing.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/tests/test_toml_typedconfig_class.py` & `configuraptor-1.4.0/tests/test_toml_typedconfig_class.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/LICENSE.txt` & `configuraptor-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/README.md` & `configuraptor-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/pyproject.toml` & `configuraptor-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `configuraptor-1.3.2/PKG-INFO` & `configuraptor-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configuraptor
-Version: 1.3.2
+Version: 1.4.0
 Summary: Load toml/yaml/json config files into classes for a typed config (type hinting etc.)
 Project-URL: Documentation, https://github.com/trialandsuccess/configuraptor#readme
 Project-URL: Issues, https://github.com/trialandsuccess/configuraptor/issues
 Project-URL: Source, https://github.com/trialandsuccess/configuraptor
 Author-email: Robin van der Noord <robin@trialandsuccess.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

