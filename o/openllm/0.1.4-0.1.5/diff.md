# Comparing `tmp/openllm-0.1.4.tar.gz` & `tmp/openllm-0.1.5.tar.gz`

## Comparing `openllm-0.1.4.tar` & `openllm-0.1.5.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 openllm-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.1.4/ADDING_NEW_MODEL.md
--rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 openllm-0.1.4/DEVELOPMENT.md
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.1.4/package.json
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.1.4/taplo.toml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 openllm-0.1.4/.github/CODEOWNERS
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 openllm-0.1.4/.github/dependabot.yml
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 openllm-0.1.4/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 openllm-0.1.4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 openllm-0.1.4/.github/ISSUE_TEMPLATE/feature_request.yml
--rwxr-xr-x   0        0        0     1306 2020-02-02 00:00:00.000000 openllm-0.1.4/.github/actions/create_release_and_archive.sh
--rwxr-xr-x   0        0        0     1764 2020-02-02 00:00:00.000000 openllm-0.1.4/.github/actions/release.sh
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm-0.1.4/.github/actions/setup-repo/action.yml
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 openllm-0.1.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 openllm-0.1.4/.github/workflows/create-releases.yml
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 openllm-0.1.4/.github/workflows/release-notes.yml
--rw-r--r--   0        0        0  1549838 2020-02-02 00:00:00.000000 openllm-0.1.4/assets/output.gif
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 openllm-0.1.4/examples/play.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/__about__.py
--rw-r--r--   0        0        0     8157 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/__init__.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/__main__.py
--rw-r--r--   0        0        0    50213 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/_configuration.py
--rw-r--r--   0        0        0    34895 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/_llm.py
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/_package.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/_prompt.py
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/_schema.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/_service.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/_types.py
--rw-r--r--   0        0        0    40654 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/cli.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/client.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/py.typed
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/__init__.py
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/auto/__init__.py
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/auto/configuration_auto.py
--rw-r--r--   0        0        0     9874 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/auto/factory.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/auto/modeling_auto.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/auto/modeling_flax_auto.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/auto/modeling_tf_auto.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/chatglm/__init__.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/chatglm/configuration_chatglm.py
--rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/chatglm/modeling_chatglm.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/dolly_v2/__init__.py
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/dolly_v2/configuration_dolly_v2.py
--rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/dolly_v2/modeling_dolly_v2.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/falcon/__init__.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/falcon/configuration_falcon.py
--rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/falcon/modeling_falcon.py
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/flan_t5/__init__.py
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/flan_t5/configuration_flan_t5.py
--rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/flan_t5/modeling_flan_t5.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/gpt_neox/__init__.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/gptj/__init__.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/llama/__init__.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/roberta/__init__.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/stablelm/__init__.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/stablelm/configuration_stablelm.py
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/stablelm/modeling_stablelm.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/starcoder/__init__.py
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/starcoder/configuration_starcoder.py
--rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/models/starcoder/modeling_starcoder.py
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/utils/__init__.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/utils/analytics.py
--rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/utils/codegen.py
--rw-r--r--   0        0        0    15304 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/utils/dantic.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/utils/dummy_flax_objects.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/utils/dummy_pt_and_einops_objects.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/utils/dummy_pt_objects.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/utils/dummy_tf_objects.py
--rw-r--r--   0        0        0    10442 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/utils/import_utils.py
--rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm/utils/lazy.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm_client/__init__.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm_client/_prompt.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm_client/cache/__init__.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm_client/cache/inmemory.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm_client/runtimes/__init__.py
--rw-r--r--   0        0        0     6777 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm_client/runtimes/base.py
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm_client/runtimes/grpc.py
--rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm_client/runtimes/http.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm_js/package.json
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm_js/tsconfig.cjs.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.1.4/src/openllm_js/tsconfig.json
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 openllm-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 openllm-0.1.4/tests/test_configuration.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.4/tests/_strategies/__init__.py
--rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 openllm-0.1.4/tests/_strategies/_configuration.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.4/tests/models/flan_t5/__init__.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 openllm-0.1.4/tests/models/flan_t5/test_modeling_flan_t5.py
--rwxr-xr-x   0        0        0      489 2020-02-02 00:00:00.000000 openllm-0.1.4/tools/add-license-headers
--rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 openllm-0.1.4/tools/assert-license-headers
--rwxr-xr-x   0        0        0      718 2020-02-02 00:00:00.000000 openllm-0.1.4/tools/assert-model-table-latest
--rwxr-xr-x   0        0        0     1901 2020-02-02 00:00:00.000000 openllm-0.1.4/tools/run-release-action
--rwxr-xr-x   0        0        0     1844 2020-02-02 00:00:00.000000 openllm-0.1.4/tools/update-optional-dependencies.py
--rwxr-xr-x   0        0        0     3559 2020-02-02 00:00:00.000000 openllm-0.1.4/tools/update-readme.py
--rw-r--r--   0        0        0    15605 2020-02-02 00:00:00.000000 openllm-0.1.4/typings/attr/__init__.pyi
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 openllm-0.1.4/typings/attr/_cmp.pyi
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 openllm-0.1.4/typings/attr/_compat.pyi
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 openllm-0.1.4/typings/attr/_typing_compat.pyi
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 openllm-0.1.4/typings/attr/_version_info.pyi
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 openllm-0.1.4/typings/attr/converters.pyi
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 openllm-0.1.4/typings/attr/exceptions.pyi
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 openllm-0.1.4/typings/attr/filters.pyi
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 openllm-0.1.4/typings/attr/setters.pyi
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 openllm-0.1.4/typings/attr/validators.pyi
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 openllm-0.1.4/typings/click_option_group/__init__.pyi
--rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 openllm-0.1.4/typings/click_option_group/_core.pyi
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 openllm-0.1.4/typings/click_option_group/_decorators.pyi
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 openllm-0.1.4/typings/click_option_group/_helpers.pyi
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 openllm-0.1.4/typings/click_option_group/_version.pyi
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 openllm-0.1.4/typings/deepmerge/__init__.pyi
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 openllm-0.1.4/typings/deepmerge/merger.pyi
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 openllm-0.1.4/typings/deepmerge/strategy/core.pyi
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 openllm-0.1.4/typings/deepmerge/strategy/dict.pyi
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 openllm-0.1.4/typings/deepmerge/strategy/list.pyi
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 openllm-0.1.4/typings/deepmerge/strategy/set.pyi
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 openllm-0.1.4/.gitignore
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.1.4/LICENSE.md
--rw-r--r--   0        0        0    13116 2020-02-02 00:00:00.000000 openllm-0.1.4/README.md
--rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 openllm-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    15968 2020-02-02 00:00:00.000000 openllm-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 openllm-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.1.5/ADDING_NEW_MODEL.md
+-rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 openllm-0.1.5/DEVELOPMENT.md
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.1.5/package.json
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.1.5/taplo.toml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 openllm-0.1.5/.github/CODEOWNERS
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 openllm-0.1.5/.github/dependabot.yml
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 openllm-0.1.5/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 openllm-0.1.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 openllm-0.1.5/.github/ISSUE_TEMPLATE/feature_request.yml
+-rwxr-xr-x   0        0        0     1306 2020-02-02 00:00:00.000000 openllm-0.1.5/.github/actions/create_release_and_archive.sh
+-rwxr-xr-x   0        0        0     1764 2020-02-02 00:00:00.000000 openllm-0.1.5/.github/actions/release.sh
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm-0.1.5/.github/actions/setup-repo/action.yml
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 openllm-0.1.5/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 openllm-0.1.5/.github/workflows/create-releases.yml
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 openllm-0.1.5/.github/workflows/release-notes.yml
+-rw-r--r--   0        0        0  1549838 2020-02-02 00:00:00.000000 openllm-0.1.5/assets/output.gif
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 openllm-0.1.5/examples/play.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/__about__.py
+-rw-r--r--   0        0        0     8157 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/__init__.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/__main__.py
+-rw-r--r--   0        0        0    50213 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/_configuration.py
+-rw-r--r--   0        0        0    34895 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/_llm.py
+-rw-r--r--   0        0        0    10649 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/_package.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/_prompt.py
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/_schema.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/_service.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/_types.py
+-rw-r--r--   0        0        0    41496 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/cli.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/client.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/py.typed
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/__init__.py
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/auto/__init__.py
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/auto/configuration_auto.py
+-rw-r--r--   0        0        0     9874 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/auto/factory.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/auto/modeling_auto.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/auto/modeling_flax_auto.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/auto/modeling_tf_auto.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/chatglm/__init__.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/chatglm/configuration_chatglm.py
+-rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/chatglm/modeling_chatglm.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/dolly_v2/__init__.py
+-rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/dolly_v2/configuration_dolly_v2.py
+-rw-r--r--   0        0        0     4025 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/dolly_v2/modeling_dolly_v2.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/falcon/__init__.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/falcon/configuration_falcon.py
+-rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/falcon/modeling_falcon.py
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/flan_t5/__init__.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/flan_t5/configuration_flan_t5.py
+-rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/flan_t5/modeling_flan_t5.py
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/gpt_neox/__init__.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/gptj/__init__.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/llama/__init__.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/roberta/__init__.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/stablelm/__init__.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/stablelm/configuration_stablelm.py
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/stablelm/modeling_stablelm.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/starcoder/__init__.py
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/starcoder/configuration_starcoder.py
+-rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/starcoder/modeling_starcoder.py
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/utils/__init__.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/utils/analytics.py
+-rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/utils/codegen.py
+-rw-r--r--   0        0        0    15309 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/utils/dantic.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/utils/dummy_flax_objects.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/utils/dummy_pt_and_einops_objects.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/utils/dummy_pt_objects.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/utils/dummy_tf_objects.py
+-rw-r--r--   0        0        0    10442 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/utils/import_utils.py
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/utils/lazy.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm_client/__init__.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm_client/_prompt.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm_client/cache/__init__.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm_client/cache/inmemory.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm_client/runtimes/__init__.py
+-rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm_client/runtimes/base.py
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm_client/runtimes/grpc.py
+-rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm_client/runtimes/http.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm_js/package.json
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm_js/tsconfig.cjs.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm_js/tsconfig.json
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 openllm-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 openllm-0.1.5/tests/test_configuration.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.5/tests/_strategies/__init__.py
+-rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 openllm-0.1.5/tests/_strategies/_configuration.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.5/tests/models/flan_t5/__init__.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 openllm-0.1.5/tests/models/flan_t5/test_modeling_flan_t5.py
+-rwxr-xr-x   0        0        0      489 2020-02-02 00:00:00.000000 openllm-0.1.5/tools/add-license-headers
+-rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 openllm-0.1.5/tools/assert-license-headers
+-rwxr-xr-x   0        0        0      718 2020-02-02 00:00:00.000000 openllm-0.1.5/tools/assert-model-table-latest
+-rwxr-xr-x   0        0        0     1901 2020-02-02 00:00:00.000000 openllm-0.1.5/tools/run-release-action
+-rwxr-xr-x   0        0        0     1844 2020-02-02 00:00:00.000000 openllm-0.1.5/tools/update-optional-dependencies.py
+-rwxr-xr-x   0        0        0     3559 2020-02-02 00:00:00.000000 openllm-0.1.5/tools/update-readme.py
+-rw-r--r--   0        0        0    15605 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/attr/__init__.pyi
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/attr/_cmp.pyi
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/attr/_compat.pyi
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/attr/_typing_compat.pyi
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/attr/_version_info.pyi
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/attr/converters.pyi
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/attr/exceptions.pyi
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/attr/filters.pyi
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/attr/setters.pyi
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/attr/validators.pyi
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/click_option_group/__init__.pyi
+-rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/click_option_group/_core.pyi
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/click_option_group/_decorators.pyi
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/click_option_group/_helpers.pyi
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/click_option_group/_version.pyi
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/deepmerge/__init__.pyi
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/deepmerge/merger.pyi
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/deepmerge/strategy/core.pyi
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/deepmerge/strategy/dict.pyi
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/deepmerge/strategy/list.pyi
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/deepmerge/strategy/set.pyi
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 openllm-0.1.5/.gitignore
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.1.5/LICENSE.md
+-rw-r--r--   0        0        0    13116 2020-02-02 00:00:00.000000 openllm-0.1.5/README.md
+-rw-r--r--   0        0        0     6467 2020-02-02 00:00:00.000000 openllm-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    15989 2020-02-02 00:00:00.000000 openllm-0.1.5/PKG-INFO
```

### Comparing `openllm-0.1.4/.pre-commit-config.yaml` & `openllm-0.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/ADDING_NEW_MODEL.md` & `openllm-0.1.5/ADDING_NEW_MODEL.md`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/DEVELOPMENT.md` & `openllm-0.1.5/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/package.json` & `openllm-0.1.5/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'0.1.5'"}*

```diff
@@ -11,12 +11,12 @@
     "engines": {
         "node": ">=16"
     },
     "license": "Apache 2.0",
     "name": "openllm",
     "private": true,
     "repository": "git@github.com:llmsys/OpenLLM.git",
-    "version": "0.1.4",
+    "version": "0.1.5",
     "workspaces": [
         "src/openllm_js"
     ]
 }
```

### Comparing `openllm-0.1.4/.github/dependabot.yml` & `openllm-0.1.5/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/.github/ISSUE_TEMPLATE/bug_report.yml` & `openllm-0.1.5/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/.github/ISSUE_TEMPLATE/config.yml` & `openllm-0.1.5/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/.github/ISSUE_TEMPLATE/feature_request.yml` & `openllm-0.1.5/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/.github/actions/create_release_and_archive.sh` & `openllm-0.1.5/.github/actions/create_release_and_archive.sh`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/.github/actions/release.sh` & `openllm-0.1.5/.github/actions/release.sh`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/.github/actions/setup-repo/action.yml` & `openllm-0.1.5/.github/actions/setup-repo/action.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/.github/workflows/ci.yml` & `openllm-0.1.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/.github/workflows/create-releases.yml` & `openllm-0.1.5/.github/workflows/create-releases.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/.github/workflows/release-notes.yml` & `openllm-0.1.5/.github/workflows/release-notes.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/assets/output.gif` & `openllm-0.1.5/assets/output.gif`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/examples/play.py` & `openllm-0.1.5/examples/play.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/__about__.py` & `openllm-0.1.5/src/openllm/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.1.4"
+__version__ = "0.1.5"
```

### Comparing `openllm-0.1.4/src/openllm/__init__.py` & `openllm-0.1.5/src/openllm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/__main__.py` & `openllm-0.1.5/src/openllm/__main__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/_configuration.py` & `openllm-0.1.5/src/openllm/_configuration.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1022,19 +1022,19 @@
             elif k.startswith(f"{self.__openllm_model_name__}_"):
                 llm_config_attrs[k[len(self.__openllm_model_name__ + "_") :]] = v
                 key_to_remove.append(k)
 
         return self.model_construct_env(**llm_config_attrs), {k: v for k, v in attrs.items() if k not in key_to_remove}
 
     @t.overload
-    def to_generation_config(self, return_as_dict: t.Literal[True] = ...) -> DictStrAny:
+    def to_generation_config(self, return_as_dict: t.Literal[False] = ...) -> transformers.GenerationConfig:
         ...
 
     @t.overload
-    def to_generation_config(self, return_as_dict: t.Literal[False] = ...) -> transformers.GenerationConfig:
+    def to_generation_config(self, return_as_dict: t.Literal[True] = ...) -> DictStrAny:
         ...
 
     def to_generation_config(self, return_as_dict: bool = False) -> transformers.GenerationConfig | DictStrAny:
         config = transformers.GenerationConfig(**bentoml_cattr.unstructure(self.generation_config))
         return config.to_dict() if return_as_dict else config
 
     @classmethod
```

### Comparing `openllm-0.1.4/src/openllm/_llm.py` & `openllm-0.1.5/src/openllm/_llm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/_package.py` & `openllm-0.1.5/src/openllm/_package.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,15 @@
 def build(model_name: str, *, __cli__: bool = False, **attrs: t.Any) -> tuple[bentoml.Bento, bool] | bentoml.Bento:
     """Package a LLM into a Bento."""
 
     overwrite_existing_bento = attrs.pop("_overwrite_existing_bento", False)
     current_model_envvar = os.environ.pop("OPENLLM_MODEL", None)
     current_model_id_envvar = os.environ.pop("OPENLLM_MODEL_ID", None)
     _previously_built = False
-    workers = attrs.pop("_workers", None)
+    workers_per_resource = attrs.pop("_workers_per_resource", None)
     model_id: str = attrs.pop("model_id", None)
 
     llm_config = openllm.AutoConfig.for_model(model_name)
 
     logger.info("Packing '%s' into a Bento with kwargs=%s...", model_name, attrs)
 
     # NOTE: We set this environment variable so that our service.py logic won't raise RuntimeError
@@ -189,15 +189,17 @@
             llm = openllm.AutoLLM.for_model(model_name, model_id=model_id, llm_config=llm_config, **attrs)
 
         os.environ["OPENLLM_MODEL_ID"] = llm.model_id
 
         labels = dict(llm.identifying_params)
         labels.update({"_type": llm.llm_type, "_framework": to_use_framework})
         service_name = f"generated_{llm.config.__openllm_model_name__}_service.py"
-        workers_per_resource = utils.first_not_none(workers, default=llm.config.__openllm_workers_per_resource__)
+        workers_per_resource = utils.first_not_none(
+            workers_per_resource, default=llm.config.__openllm_workers_per_resource__
+        )
 
         with fs.open_fs(f"temp://llm_{llm.config.__openllm_model_name__}") as llm_fs:
             # add service.py definition to this temporary folder
             utils.codegen.write_service(model_name, llm.model_id, service_name, llm_fs)
 
             bento_tag = bentoml.Tag.from_taglike(f"{llm.llm_type}-service:{llm.tag.version}")
             try:
```

### Comparing `openllm-0.1.4/src/openllm/_prompt.py` & `openllm-0.1.5/src/openllm/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/_schema.py` & `openllm-0.1.5/src/openllm/_schema.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/_service.py` & `openllm-0.1.5/src/openllm/_service.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/_types.py` & `openllm-0.1.5/src/openllm/_types.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/cli.py` & `openllm-0.1.5/src/openllm/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from __future__ import annotations
 
 import functools
 import inspect
 import logging
 import os
 import re
-import subprocess
+import contextlib
 import sys
 import time
 import traceback
 import typing as t
 
 import bentoml
 import click
@@ -158,19 +158,21 @@
         cls=NargsOptions,
         nargs=-1,
         envvar="CUDA_VISIBLE_DEVICES",
         callback=parse_device_callback,
         help=f"Assign GPU devices (if available) for {model_name}.",
         show_envvar=True,
     )
-    @workers_option(cog.optgroup)
+    @workers_per_resource_option(cog.optgroup)
+    @click.pass_context
     def model_start(
+        ctx: click.Context,
         server_timeout: int | None,
         model_id: str | None,
-        workers: float | None,
+        workers_per_resource: float | None,
         device: tuple[str, ...] | None,
         **attrs: t.Any,
     ) -> openllm.LLMConfig:
         config, server_attrs = llm_config.model_validate_click(**attrs)
 
         if llm_config.__openllm_env__.get_framework_env() == "flax":
             llm = openllm.AutoFlaxLLM.for_model(model_name, model_id=model_id, llm_config=config)
@@ -183,29 +185,24 @@
             _echo(
                 f"Make sure to have the following dependencies available: {llm.config.__openllm_requirements__}",
                 fg="yellow",
             )
 
         # NOTE: We need to initialize llm here first to check if the model is already downloaded to
         # avoid deadlock before the subprocess forking.
-        subprocess.check_output(
-            [
-                sys.executable,
-                "-m",
-                "openllm",
-                "download-models",
-                model_name,
-                "--model-id",
-                llm.model_id,
-                "--output",
-                "porcelain",
-            ]
-        )
+        with open(os.devnull, "w") as devnull:
+            with contextlib.redirect_stderr(devnull), contextlib.redirect_stdout(devnull):
+                ctx.invoke(
+                    download_models,
+                    model_name=model_name,
+                    model_id=llm.model_id,
+                    output="porcelain",
+                )
 
-        workers_per_resource = first_not_none(workers, default=llm.config.__openllm_workers_per_resource__)
+        workers_per_resource = first_not_none(workers_per_resource, default=llm.config.__openllm_workers_per_resource__)
         server_timeout = first_not_none(server_timeout, default=llm.config.__openllm_timeout__)
 
         num_workers = int(1 / workers_per_resource)
         if num_workers > 1:
             _echo(
                 f"{model_name} requires at least {num_workers} GPUs/CPUs available per worker."
                 " Make sure that it has available resources to run inference.",
@@ -420,14 +417,17 @@
             attrs.setdefault("name", name)
 
             # Wrap implementation withc common parameters
             wrapped = self.common_params(f)
             # Wrap into OpenLLM tracking
             wrapped = self.usage_tracking(wrapped, self, **attrs)
             # Wrap into exception handling
+            if "do_not_track" in attrs:
+                # We hit this branch when ctx.invoke the function
+                attrs.pop("do_not_track")
             wrapped = self.exception_handling(wrapped, self, **attrs)
 
             # move common parameters to end of the parameters list
             wrapped.__click_params__ = (
                 wrapped.__click_params__[-self.NUMBER_OF_COMMON_PARAMS :]
                 + wrapped.__click_params__[: -self.NUMBER_OF_COMMON_PARAMS]
             )
@@ -539,20 +539,41 @@
                 self._nargs_parser = our_parser
                 self._prev_parser_process = our_parser.process
                 our_parser.process = _parser
                 break
         return retval
 
 
-def parse_device_callback(_: click.Context, params: click.Parameter, value: tuple[str, ...] | None) -> t.Any:
+def parse_device_callback(
+    _: click.Context, params: click.Parameter, value: tuple[str, ...] | tuple[t.Literal["all"]] | None
+) -> t.Any:
     if value is None:
         return value
 
     if not LazyType(TupleStrAny).isinstance(value):
         raise RuntimeError(f"{params} only accept multiple values.")
+
+    # NOTE: --device all is a special case
+    if len(value) == 1:
+        if value[0] != "all":
+            raise RuntimeError(f"{params} parameter only accept 'all' as a string value.")
+        import pynvml  # transitive dependencies of BentoML
+
+        try:
+            pynvml.nvmlInit()
+            return tuple(range(pynvml.nvmlDeviceGetCount()))
+        except (pynvml.nvml.NVMLError, OSError):
+            logger.debug("GPU not detected. Unable to initialize pynvml lib.")
+            return ()
+        finally:
+            try:
+                pynvml.nvmlShutdown()
+            except Exception:
+                pass
+
     parsed: tuple[str, ...] = tuple()
     for v in value:
         if v == ",":
             # NOTE: This hits when CUDA_VISIBLE_DEVICES is set
             continue
         if "," in v:
             parsed += tuple(v.split(","))
@@ -604,25 +625,25 @@
         default=None,
         help="Optional model_id name or path for (fine-tune) weight.",
         envvar=envvar,
         show_envvar=True if envvar is not None else False,
     )
 
 
-def workers_option(factory: t.Any, build: bool = False):
+def workers_per_resource_option(factory: t.Any, build: bool = False):
     help_str = """Number of workers per resource assigned.
     See https://docs.bentoml.org/en/latest/guides/scheduling.html#resource-scheduling-strategy
     for more information. By default, this is set to 1."""
     if build:
         help_str += """\n
     NOTE: The workers value passed into 'build' will determine how the LLM can
     be provisioned in Kubernetes as well as in standalone container. This will
     ensure it has the same effect with 'openllm start --workers ...'"""
     return factory.option(
-        "--workers",
+        "--workers-per-resource",
         default=None,
         type=click.FLOAT,
         help=help_str,
         required=False,
     )
 
 
@@ -669,16 +690,22 @@
     @cli.command()
     @click.argument(
         "model_name", type=click.Choice([inflection.dasherize(name) for name in openllm.CONFIG_MAPPING.keys()])
     )
     @model_id_option(click)
     @output_option
     @click.option("--overwrite", is_flag=True, help="Overwrite existing Bento for given LLM if it already exists.")
-    @workers_option(click, build=True)
-    def build(model_name: str, model_id: str | None, overwrite: bool, output: OutputLiteral, workers: float | None):
+    @workers_per_resource_option(click, build=True)
+    def build(
+        model_name: str,
+        model_id: str | None,
+        overwrite: bool,
+        output: OutputLiteral,
+        workers_per_resource: float | None,
+    ):
         """Package a given models into a Bento.
 
         $ openllm build flan-t5
 
         \b
         NOTE: To run a container built from this Bento with GPU support, make sure
         to have https://github.com/NVIDIA/nvidia-container-toolkit install locally.
@@ -691,15 +718,15 @@
             if overwrite:
                 _echo(f"Overwriting existing Bento for {model_name}.", fg="yellow")
 
         bento, _previously_built = openllm.build(
             model_name,
             __cli__=True,
             model_id=model_id,
-            _workers=workers,
+            _workers_per_resource=workers_per_resource,
             _overwrite_existing_bento=overwrite,
         )
 
         if output == "pretty":
             if not get_quiet_mode():
                 _echo("\n" + OPENLLM_FIGLET, fg="white")
                 if not _previously_built:
@@ -861,63 +888,14 @@
                     ).decode(),
                     fg="white",
                 )
 
         sys.exit(0)
 
     @cli.command()
-    @click.argument(
-        "model_name", type=click.Choice([inflection.dasherize(name) for name in openllm.CONFIG_MAPPING.keys()])
-    )
-    @model_id_option(click)
-    @output_option
-    def download_models(model_name: str, model_id: str | None, output: OutputLiteral):
-        """Setup LLM interactively.
-
-        Note: This is useful for development and setup for fine-tune.
-        """
-        config = openllm.AutoConfig.for_model(model_name)
-        env = config.__openllm_env__.get_framework_env()
-        if env == "flax":
-            model = openllm.AutoFlaxLLM.for_model(model_name, model_id=model_id, llm_config=config)
-        elif env == "tf":
-            model = openllm.AutoTFLLM.for_model(model_name, model_id=model_id, llm_config=config)
-        else:
-            model = openllm.AutoLLM.for_model(model_name, model_id=model_id, llm_config=config)
-
-        if len(bentoml.models.list(model.tag)) == 0:
-            if output == "pretty":
-                _echo(f"{model.tag} does not exists yet!. Downloading...", fg="yellow", nl=True)
-            m = model.ensure_model_id_exists()
-            if output == "pretty":
-                _echo(f"Saved model: {m.tag}")
-            elif output == "json":
-                _echo(
-                    orjson.dumps(
-                        {"previously_setup": False, "framework": env, "tag": str(m.tag)}, option=orjson.OPT_INDENT_2
-                    ).decode()
-                )
-            else:
-                _echo(model.tag)
-        else:
-            m = bentoml.transformers.get(model.tag)
-            if output == "pretty":
-                _echo(f"{model_name} is already setup for framework '{env}': {str(m.tag)}", nl=True, fg="yellow")
-            elif output == "json":
-                _echo(
-                    orjson.dumps(
-                        {"previously_setup": True, "framework": env, "model": str(m.tag)}, option=orjson.OPT_INDENT_2
-                    ).decode(),
-                    fg="white",
-                )
-            else:
-                _echo(m.tag, fg="white")
-        return m
-
-    @cli.command()
     @click.option(
         "-y",
         "--yes",
         "--assume-yes",
         is_flag=True,
         help="Skip confirmation when deleting a specific model",
     )
@@ -991,19 +969,71 @@
             _echo(formatted, fg="cyan")
         elif output == "json":
             _echo(orjson.dumps(res, option=orjson.OPT_INDENT_2).decode(), fg="white")
         else:
             _echo(res["responses"], fg="white")
 
     if t.TYPE_CHECKING:
-        assert download_models and build and models and start and start_grpc and query_ and prune
+        assert build and models and start and start_grpc and query_ and prune
 
     if psutil.WINDOWS:
         sys.stdout.reconfigure(encoding="utf-8")  # type: ignore
 
     return cli
 
 
 cli = cli_factory()
 
+
+@cli.command()
+@click.argument(
+    "model_name",
+    type=click.Choice([inflection.dasherize(name) for name in openllm.CONFIG_MAPPING.keys()]),
+)
+@model_id_option(click)
+@output_option
+def download_models(model_name: str, model_id: str | None, output: OutputLiteral):
+    """Setup LLM interactively.
+
+    Note: This is useful for development and setup for fine-tune.
+    """
+    config = openllm.AutoConfig.for_model(model_name)
+    env = config.__openllm_env__.get_framework_env()
+    if env == "flax":
+        model = openllm.AutoFlaxLLM.for_model(model_name, model_id=model_id, llm_config=config)
+    elif env == "tf":
+        model = openllm.AutoTFLLM.for_model(model_name, model_id=model_id, llm_config=config)
+    else:
+        model = openllm.AutoLLM.for_model(model_name, model_id=model_id, llm_config=config)
+
+    if len(bentoml.models.list(model.tag)) == 0:
+        if output == "pretty":
+            _echo(f"{model.tag} does not exists yet!. Downloading...", fg="yellow", nl=True)
+        m = model.ensure_model_id_exists()
+        if output == "pretty":
+            _echo(f"Saved model: {m.tag}")
+        elif output == "json":
+            _echo(
+                orjson.dumps(
+                    {"previously_setup": False, "framework": env, "tag": str(m.tag)}, option=orjson.OPT_INDENT_2
+                ).decode()
+            )
+        else:
+            _echo(model.tag)
+    else:
+        m = bentoml.transformers.get(model.tag)
+        if output == "pretty":
+            _echo(f"{model_name} is already setup for framework '{env}': {str(m.tag)}", nl=True, fg="yellow")
+        elif output == "json":
+            _echo(
+                orjson.dumps(
+                    {"previously_setup": True, "framework": env, "model": str(m.tag)}, option=orjson.OPT_INDENT_2
+                ).decode(),
+                fg="white",
+            )
+        else:
+            _echo(m.tag, fg="white")
+    return m
+
+
 if __name__ == "__main__":
     cli()
```

### Comparing `openllm-0.1.4/src/openllm/client.py` & `openllm-0.1.5/src/openllm/client.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/exceptions.py` & `openllm-0.1.5/src/openllm/exceptions.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/__init__.py` & `openllm-0.1.5/src/openllm/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/auto/__init__.py` & `openllm-0.1.5/src/openllm/models/auto/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/auto/configuration_auto.py` & `openllm-0.1.5/src/openllm/models/auto/configuration_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/auto/factory.py` & `openllm-0.1.5/src/openllm/models/auto/factory.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/auto/modeling_auto.py` & `openllm-0.1.5/src/openllm/models/auto/modeling_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/auto/modeling_flax_auto.py` & `openllm-0.1.5/src/openllm/models/auto/modeling_flax_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/auto/modeling_tf_auto.py` & `openllm-0.1.5/src/openllm/models/auto/modeling_tf_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/chatglm/__init__.py` & `openllm-0.1.5/src/openllm/models/chatglm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/chatglm/configuration_chatglm.py` & `openllm-0.1.5/src/openllm/models/chatglm/configuration_chatglm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/chatglm/modeling_chatglm.py` & `openllm-0.1.5/src/openllm/models/chatglm/modeling_chatglm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/dolly_v2/__init__.py` & `openllm-0.1.5/src/openllm/models/dolly_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/dolly_v2/configuration_dolly_v2.py` & `openllm-0.1.5/src/openllm/models/dolly_v2/configuration_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/dolly_v2/modeling_dolly_v2.py` & `openllm-0.1.5/src/openllm/models/dolly_v2/modeling_dolly_v2.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 class DollyV2(openllm.LLM["transformers.Pipeline", "transformers.PreTrainedTokenizer"]):
     __openllm_internal__ = True
 
     @property
     def import_kwargs(self):
         model_kwds = {
-            "device_map": "auto" if torch.cuda.is_available() and torch.cuda.device_count() > 1 else None,
+            "device_map": "auto" if torch.cuda.is_available() else None,
             "torch_dtype": torch.bfloat16,
         }
         tokenizer_kwds = {"padding_side": "left"}
         return model_kwds, tokenizer_kwds
 
     def llm_post_init(self):
         self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
```

### Comparing `openllm-0.1.4/src/openllm/models/falcon/__init__.py` & `openllm-0.1.5/src/openllm/models/falcon/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/falcon/configuration_falcon.py` & `openllm-0.1.5/src/openllm/models/falcon/configuration_falcon.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/falcon/modeling_falcon.py` & `openllm-0.1.5/src/openllm/models/falcon/modeling_falcon.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/flan_t5/__init__.py` & `openllm-0.1.5/src/openllm/models/flan_t5/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/flan_t5/configuration_flan_t5.py` & `openllm-0.1.5/src/openllm/models/flan_t5/configuration_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/flan_t5/modeling_flan_t5.py` & `openllm-0.1.5/src/openllm/models/flan_t5/modeling_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/flan_t5/modeling_flax_flan_t5.py` & `openllm-0.1.5/src/openllm/models/flan_t5/modeling_flax_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/flan_t5/modeling_tf_flan_t5.py` & `openllm-0.1.5/src/openllm/models/flan_t5/modeling_tf_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/gpt_neox/__init__.py` & `openllm-0.1.5/src/openllm/models/gpt_neox/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/gptj/__init__.py` & `openllm-0.1.5/src/openllm/models/gptj/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/llama/__init__.py` & `openllm-0.1.5/src/openllm/models/llama/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/roberta/__init__.py` & `openllm-0.1.5/src/openllm/models/roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/stablelm/__init__.py` & `openllm-0.1.5/src/openllm/models/stablelm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/stablelm/configuration_stablelm.py` & `openllm-0.1.5/src/openllm/models/stablelm/configuration_stablelm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/stablelm/modeling_stablelm.py` & `openllm-0.1.5/src/openllm/models/stablelm/modeling_stablelm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/starcoder/__init__.py` & `openllm-0.1.5/src/openllm/models/starcoder/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/starcoder/configuration_starcoder.py` & `openllm-0.1.5/src/openllm/models/starcoder/configuration_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/models/starcoder/modeling_starcoder.py` & `openllm-0.1.5/src/openllm/models/starcoder/modeling_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/utils/__init__.py` & `openllm-0.1.5/src/openllm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/utils/analytics.py` & `openllm-0.1.5/src/openllm/utils/analytics.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/utils/codegen.py` & `openllm-0.1.5/src/openllm/utils/codegen.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/utils/dantic.py` & `openllm-0.1.5/src/openllm/utils/dantic.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,27 +276,27 @@
     name = "enum"
 
     def __init__(self, enum: Enum, case_sensitive: bool = False):
         self.mapping = enum
         self.internal_type = enum
         super().__init__([e.name for e in self.mapping], case_sensitive)
 
-    def convert(self, value: t.Any, param: click.Parameter | None, ctx: click.Context | None) -> t.Any:
+    def convert(self, value: t.Any, param: click.Parameter | None, ctx: click.Context | None) -> Enum:
         if isinstance(value, self.internal_type):
             return value
         result = super().convert(value, param, ctx)
         if isinstance(result, str):
             result = self.mapping[result]
         return result
 
 
 class LiteralChoice(EnumChoice):
     name = "literal"
 
-    def __init__(self, enum: t.Literal, case_sensitive: bool = False):
+    def __init__(self, enum: t.LiteralString, case_sensitive: bool = False):
         # expect every literal value to belong to the same primitive type
         values = list(enum.__args__)
         item_type = type(values[0])
         assert all(isinstance(v, item_type) for v in values), f"Field {enum} contains items of different types"
         self.internal_type = item_type
         self.mapping = {str(v): v for v in values}
         super(EnumChoice, self).__init__(list(self.mapping.keys()), case_sensitive)
```

### Comparing `openllm-0.1.4/src/openllm/utils/dummy_flax_objects.py` & `openllm-0.1.5/src/openllm/utils/dummy_flax_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py` & `openllm-0.1.5/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/utils/dummy_pt_and_einops_objects.py` & `openllm-0.1.5/src/openllm/utils/dummy_pt_and_einops_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/utils/dummy_pt_objects.py` & `openllm-0.1.5/src/openllm/utils/dummy_pt_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/utils/dummy_tf_objects.py` & `openllm-0.1.5/src/openllm/utils/dummy_tf_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/utils/import_utils.py` & `openllm-0.1.5/src/openllm/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm/utils/lazy.py` & `openllm-0.1.5/src/openllm/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm_client/__init__.py` & `openllm-0.1.5/src/openllm_client/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm_client/_prompt.py` & `openllm-0.1.5/src/openllm_client/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm_client/cache/__init__.py` & `openllm-0.1.5/src/openllm_client/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm_client/cache/inmemory.py` & `openllm-0.1.5/src/openllm_client/cache/inmemory.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm_client/runtimes/__init__.py` & `openllm-0.1.5/src/openllm_client/runtimes/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/src/openllm_client/runtimes/base.py` & `openllm-0.1.5/src/openllm_client/runtimes/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+import asyncio
 import typing as t
 from abc import abstractmethod
+from urllib.parse import urljoin
 
 import bentoml
+import httpx
 
 import openllm
 
 if t.TYPE_CHECKING:
 
     class AnnotatedClient(bentoml.client.Client):
         def health(self, *args: t.Any, **attrs: t.Any) -> t.Any:
@@ -39,35 +42,48 @@
         def generate_v1(self, qa: openllm.GenerationInput) -> dict[str, t.Any]:
             ...
 
         def metadata_v1(self) -> dict[str, t.Any]:
             ...
 
 
+def in_async_context() -> bool:
+    try:
+        _ = asyncio.get_running_loop()
+        return True
+    except RuntimeError:
+        return False
+
+
 class ClientMixin:
     _api_version: str
     _client_class: type[bentoml.client.Client]
 
     _host: str
     _port: str
 
     __client__: AnnotatedClient | None = None
     __llm__: openllm.LLM[t.Any, t.Any] | None = None
 
     def __init__(self, address: str, timeout: int = 30):
         self._address = address
         self._timeout = timeout
         assert self._host and self._port, "Make sure to setup _host and _port based on your client implementation."
-        self._metadata = self.call("metadata")
 
     def __init_subclass__(cls, *, client_type: t.Literal["http", "grpc"] = "http", api_version: str = "v1"):
         cls._client_class = bentoml.client.HTTPClient if client_type == "http" else bentoml.client.GrpcClient
         cls._api_version = api_version
 
     @property
+    def _metadata(self) -> dict[str, t.Any]:
+        if in_async_context():
+            return httpx.post(urljoin(self._address, f"/{self._api_version}/metadata")).json()
+        return self.call("metadata")
+
+    @property
     @abstractmethod
     def model_name(self) -> str:
         raise NotImplementedError
 
     @property
     @abstractmethod
     def framework(self) -> t.Literal["pt", "flax", "tf"]:
@@ -136,15 +152,22 @@
     @t.overload
     def query(self, prompt: str, *, return_raw_response: t.Literal[True] = ..., **attrs: t.Any) -> dict[str, t.Any]:
         ...
 
     def query(self, prompt: str, **attrs: t.Any) -> dict[str, t.Any] | str:
         return_raw_response, prompt, generate_kwargs, postprocess_kwargs = self.prepare(prompt, **attrs)
         inputs = openllm.GenerationInput(prompt=prompt, llm_config=self.config.model_construct_env(**generate_kwargs))
-        result = self.call("generate", inputs)
+        if in_async_context():
+            result = httpx.post(
+                urljoin(self._address, f"/{self._api_version}/generate"),
+                json=openllm.utils.bentoml_cattr.unstructure(inputs),
+                timeout=self.timeout,
+            ).json()
+        else:
+            result = self.call("generate", inputs)
         r = self.postprocess(result)
 
         if return_raw_response:
             return openllm.utils.bentoml_cattr.unstructure(r)
 
         return self.llm.postprocess_generate(prompt, r.responses, **postprocess_kwargs)
```

### Comparing `openllm-0.1.4/src/openllm_client/runtimes/grpc.py` & `openllm-0.1.5/src/openllm_client/runtimes/grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,18 @@
     def configuration(self) -> dict[str, t.Any]:
         try:
             v = self._metadata.json.struct_value.fields["configuration"].string_value
             return orjson.loads(v)
         except KeyError:
             raise RuntimeError("Malformed service endpoint. (Possible malicious)")
 
-    def postprocess(self, result: Response) -> openllm.GenerationOutput:
+    def postprocess(self, result: Response | dict[str, t.Any]) -> openllm.GenerationOutput:
+        if isinstance(result, dict):
+            return openllm.GenerationOutput(**result)
+
         from google.protobuf.json_format import MessageToDict
 
         return openllm.GenerationOutput(**MessageToDict(result.json, preserving_proto_field_name=True))
 
 
 class GrpcClient(GrpcClientMixin, BaseClient, client_type="grpc"):
     def __init__(self, address: str, timeout: int = 30):
```

### Comparing `openllm-0.1.4/src/openllm_client/runtimes/http.py` & `openllm-0.1.5/src/openllm_client/runtimes/http.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/tests/__init__.py` & `openllm-0.1.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/tests/test_configuration.py` & `openllm-0.1.5/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/tests/_strategies/__init__.py` & `openllm-0.1.5/tests/_strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/tests/_strategies/_configuration.py` & `openllm-0.1.5/tests/_strategies/_configuration.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/tests/models/flan_t5/__init__.py` & `openllm-0.1.5/tests/models/flan_t5/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/tests/models/flan_t5/test_modeling_flan_t5.py` & `openllm-0.1.5/tests/models/flan_t5/test_modeling_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/tools/assert-model-table-latest` & `openllm-0.1.5/tools/assert-model-table-latest`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/tools/run-release-action` & `openllm-0.1.5/tools/run-release-action`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/tools/update-optional-dependencies.py` & `openllm-0.1.5/tools/update-optional-dependencies.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/tools/update-readme.py` & `openllm-0.1.5/tools/update-readme.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/typings/attr/__init__.pyi` & `openllm-0.1.5/typings/attr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/typings/attr/exceptions.pyi` & `openllm-0.1.5/typings/attr/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/typings/attr/validators.pyi` & `openllm-0.1.5/typings/attr/validators.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/typings/click_option_group/__init__.pyi` & `openllm-0.1.5/typings/click_option_group/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/typings/click_option_group/_core.pyi` & `openllm-0.1.5/typings/click_option_group/_core.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/typings/click_option_group/_decorators.pyi` & `openllm-0.1.5/typings/click_option_group/_decorators.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/typings/click_option_group/_helpers.pyi` & `openllm-0.1.5/typings/click_option_group/_helpers.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/typings/deepmerge/merger.pyi` & `openllm-0.1.5/typings/deepmerge/merger.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/typings/deepmerge/strategy/core.pyi` & `openllm-0.1.5/typings/deepmerge/strategy/core.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/typings/deepmerge/strategy/set.pyi` & `openllm-0.1.5/typings/deepmerge/strategy/set.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/.gitignore` & `openllm-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/LICENSE.md` & `openllm-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/README.md` & `openllm-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `openllm-0.1.4/pyproject.toml` & `openllm-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,17 @@
     "optimum",
     # Super fast JSON serialization
     "orjson",
     "inflection",
     # tabulate for CLI with CJK support
     # >=0.9.0 for some bug fixes
     "tabulate[widechars]>=0.9.0",
+    # httpx used within openllm.client
+    "httpx",
+    # for typing support
     "typing_extensions",
 ]
 description = 'OpenLLM: REST/gRPC API server for running any open Large-Language Model - StableLM, Llama, Alpaca, Dolly, Flan-T5, Custom'
 dynamic = ["version"]
 keywords = [
     "MLOps",
     "AI",
@@ -96,16 +99,14 @@
     "pytest",
     "pytest-asyncio>=0.21.0",
     "pytest-xdist[psutil]",
     "pytest-cov",
     "pytest-mock",
     "pytest-randomly",
     "pytest-rerunfailures",
-    # NOTE: black for generating service file.
-    "black[jupyter]==23.3.0",
     # NOTE: To run all hooks
     "pre-commit",
     # NOTE: Using under ./tools/update-optional-dependencies.py
     "tomlkit",
     # NOTE: Using under ./tools/update-readme.py
     "markdown-it-py",
     # NOTE: Tests strategies with Hypothesis
@@ -120,15 +121,21 @@
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11"]
 
 [tool.hatch.envs.dev]
-dependencies = ["ruff", "pyright", "hatch"]
+dependencies = [
+    "ruff",
+    "pyright",
+    "hatch",
+    # NOTE: black for generating service file.
+    "black[jupyter]==23.3.0",
+]
 detached = true
 
 [tool.hatch.envs.dev.scripts]
 all = ["fmt", "typing"]
 fmt = ["black {args:.}", "black --pyi {args:typings/}", "ruff --fix {args:.}", "style"]
 style = ["ruff {args:.}", "black --check --diff {args:.}"]
 typing = "pyright {args:src/openllm tests}"
```

### Comparing `openllm-0.1.4/PKG-INFO` & `openllm-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openllm
-Version: 0.1.4
+Version: 0.1.5
 Summary: OpenLLM: REST/gRPC API server for running any open Large-Language Model - StableLM, Llama, Alpaca, Dolly, Flan-T5, Custom
 Project-URL: Documentation, https://github.com/bentoml/openllm#readme
 Project-URL: Issues, https://github.com/bentoml/openllm/issues
 Project-URL: Source, https://github.com/bentoml/openllm
 Author-email: Aaron Pham <aarnphm@bentoml.com>, BentoML Team <contact@bentoml.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.md
@@ -23,14 +23,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Requires-Dist: attrs>=23.1.0
 Requires-Dist: bentoml[grpc,io]>=1.0.22
 Requires-Dist: cattrs>=23.1.0
+Requires-Dist: httpx
 Requires-Dist: inflection
 Requires-Dist: optimum
 Requires-Dist: orjson
 Requires-Dist: tabulate[widechars]>=0.9.0
 Requires-Dist: transformers[tokenizers,torch]>=4.29.0
 Requires-Dist: typing-extensions
 Provides-Extra: all
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openllm Version: 0.1.4 Summary: OpenLLM: REST/gRPC
+Metadata-Version: 2.1 Name: openllm Version: 0.1.5 Summary: OpenLLM: REST/gRPC
 API server for running any open Large-Language Model - StableLM, Llama, Alpaca,
 Dolly, Flan-T5, Custom Project-URL: Documentation, https://github.com/bentoml/
 openllm#readme Project-URL: Issues, https://github.com/bentoml/openllm/issues
 Project-URL: Source, https://github.com/bentoml/openllm Author-email: Aaron
 Pham
 bentoml.com>, BentoML Team
 bentoml.com> License-Expression: Apache-2.0 License-File: LICENSE.md Keywords:
@@ -15,32 +15,32 @@
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: Implementation :: CPython Classifier: Programming Language :: Python
 :: Implementation :: PyPy Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8 Requires-Dist: attrs>=23.1.0 Requires-Dist: bentoml
-[grpc,io]>=1.0.22 Requires-Dist: cattrs>=23.1.0 Requires-Dist: inflection
-Requires-Dist: optimum Requires-Dist: orjson Requires-Dist: tabulate
-[widechars]>=0.9.0 Requires-Dist: transformers[tokenizers,torch]>=4.29.0
-Requires-Dist: typing-extensions Provides-Extra: all Requires-Dist: openllm
-[chatglm]; extra == 'all' Requires-Dist: openllm[falcon]; extra == 'all'
-Requires-Dist: openllm[fine-tune]; extra == 'all' Requires-Dist: openllm[flan-
-t5]; extra == 'all' Requires-Dist: openllm[starcoder]; extra == 'all' Provides-
-Extra: chatglm Requires-Dist: cpm-kernels; extra == 'chatglm' Requires-Dist:
-sentencepiece; extra == 'chatglm' Provides-Extra: falcon Requires-Dist: einops;
-extra == 'falcon' Requires-Dist: safetensors; extra == 'falcon' Requires-Dist:
-xformers; extra == 'falcon' Provides-Extra: fine-tune Requires-Dist:
-accelerate; extra == 'fine-tune' Requires-Dist: bitsandbytes; extra == 'fine-
-tune' Requires-Dist: datasets; extra == 'fine-tune' Requires-Dist: peft; extra
-== 'fine-tune' Provides-Extra: flan-t5 Requires-Dist: flax; extra == 'flan-t5'
-Requires-Dist: jax; extra == 'flan-t5' Requires-Dist: jaxlib; extra == 'flan-
-t5' Requires-Dist: keras; extra == 'flan-t5' Requires-Dist: tensorflow; extra
-== 'flan-t5' Provides-Extra: starcoder Requires-Dist: bitsandbytes; extra ==
-'starcoder' Description-Content-Type: text/markdown
+[grpc,io]>=1.0.22 Requires-Dist: cattrs>=23.1.0 Requires-Dist: httpx Requires-
+Dist: inflection Requires-Dist: optimum Requires-Dist: orjson Requires-Dist:
+tabulate[widechars]>=0.9.0 Requires-Dist: transformers
+[tokenizers,torch]>=4.29.0 Requires-Dist: typing-extensions Provides-Extra: all
+Requires-Dist: openllm[chatglm]; extra == 'all' Requires-Dist: openllm[falcon];
+extra == 'all' Requires-Dist: openllm[fine-tune]; extra == 'all' Requires-Dist:
+openllm[flan-t5]; extra == 'all' Requires-Dist: openllm[starcoder]; extra ==
+'all' Provides-Extra: chatglm Requires-Dist: cpm-kernels; extra == 'chatglm'
+Requires-Dist: sentencepiece; extra == 'chatglm' Provides-Extra: falcon
+Requires-Dist: einops; extra == 'falcon' Requires-Dist: safetensors; extra ==
+'falcon' Requires-Dist: xformers; extra == 'falcon' Provides-Extra: fine-tune
+Requires-Dist: accelerate; extra == 'fine-tune' Requires-Dist: bitsandbytes;
+extra == 'fine-tune' Requires-Dist: datasets; extra == 'fine-tune' Requires-
+Dist: peft; extra == 'fine-tune' Provides-Extra: flan-t5 Requires-Dist: flax;
+extra == 'flan-t5' Requires-Dist: jax; extra == 'flan-t5' Requires-Dist:
+jaxlib; extra == 'flan-t5' Requires-Dist: keras; extra == 'flan-t5' Requires-
+Dist: tensorflow; extra == 'flan-t5' Provides-Extra: starcoder Requires-Dist:
+bitsandbytes; extra == 'starcoder' Description-Content-Type: text/markdown
                           ****** ð¦¾ OpenLLM ******
                       [pypi_status][ci][Twitter][Discord]
 An open platform for operating large language models(LLMs) in production. Fine-
              tune, serve, deploy, and monitor any LLMs with ease.
 ## ð Introduction With OpenLLM, you can run inference with any open-source
 large-language models(LLMs), deploy to the cloud or on-premises, and build
 powerful AI apps. ð **SOTA LLMs**: built-in supports a wide range of open-
```

