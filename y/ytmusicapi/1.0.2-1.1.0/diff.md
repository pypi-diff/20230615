# Comparing `tmp/ytmusicapi-1.0.2.tar.gz` & `tmp/ytmusicapi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytmusicapi-1.0.2.tar", last modified: Sat Apr 22 06:56:01 2023, max compression
+gzip compressed data, was "ytmusicapi-1.1.0.tar", last modified: Thu Jun 15 18:28:45 2023, max compression
```

## Comparing `ytmusicapi-1.0.2.tar` & `ytmusicapi-1.1.0.tar`

### file list

```diff
@@ -1,146 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.310473 ytmusicapi-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.290473 ytmusicapi-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.290473 ytmusicapi-1.0.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.290473 ytmusicapi-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/.github/workflows/docsbuild.yml
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-04-22 06:56:01.310473 ytmusicapi-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.290473 ytmusicapi-1.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.294473 ytmusicapi-1.0.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/docs/source/reference.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.294473 ytmusicapi-1.0.2/docs/source/setup/
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/docs/source/setup/browser.rst
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/docs/source/setup/headers_auth.json.example
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/docs/source/setup/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/docs/source/setup/oauth.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 06:56:01.310473 ytmusicapi-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.294473 ytmusicapi-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/tests/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/tests/test.cfg.example
--rw-r--r--   0 runner    (1001) docker     (123)    22775 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.294473 ytmusicapi-1.0.2/ytmusicapi/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.298473 ytmusicapi-1.0.2/ytmusicapi/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/auth/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/auth/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/auth/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/continuations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.298473 ytmusicapi-1.0.2/ytmusicapi/locales/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.286473 ytmusicapi-1.0.2/ytmusicapi/locales/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.298473 ytmusicapi-1.0.2/ytmusicapi/locales/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/ar/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/ar/LC_MESSAGES/base.po
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/base.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.286473 ytmusicapi-1.0.2/ytmusicapi/locales/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.298473 ytmusicapi-1.0.2/ytmusicapi/locales/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/de/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/de/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.286473 ytmusicapi-1.0.2/ytmusicapi/locales/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.298473 ytmusicapi-1.0.2/ytmusicapi/locales/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/en/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/en/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.286473 ytmusicapi-1.0.2/ytmusicapi/locales/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.298473 ytmusicapi-1.0.2/ytmusicapi/locales/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/es/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/es/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.286473 ytmusicapi-1.0.2/ytmusicapi/locales/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.302473 ytmusicapi-1.0.2/ytmusicapi/locales/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/fr/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/fr/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.286473 ytmusicapi-1.0.2/ytmusicapi/locales/hi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.302473 ytmusicapi-1.0.2/ytmusicapi/locales/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/hi/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/hi/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.286473 ytmusicapi-1.0.2/ytmusicapi/locales/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.302473 ytmusicapi-1.0.2/ytmusicapi/locales/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/it/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/it/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.286473 ytmusicapi-1.0.2/ytmusicapi/locales/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.302473 ytmusicapi-1.0.2/ytmusicapi/locales/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/ja/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/ja/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.286473 ytmusicapi-1.0.2/ytmusicapi/locales/ko/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.302473 ytmusicapi-1.0.2/ytmusicapi/locales/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/ko/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/ko/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.286473 ytmusicapi-1.0.2/ytmusicapi/locales/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.302473 ytmusicapi-1.0.2/ytmusicapi/locales/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/pt/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/pt/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.286473 ytmusicapi-1.0.2/ytmusicapi/locales/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.302473 ytmusicapi-1.0.2/ytmusicapi/locales/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/ru/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/ru/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.286473 ytmusicapi-1.0.2/ytmusicapi/locales/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.302473 ytmusicapi-1.0.2/ytmusicapi/locales/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/tr/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/tr/LC_MESSAGES/base.po
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/update_mo.sh
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/update_po.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.286473 ytmusicapi-1.0.2/ytmusicapi/locales/ur/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.302473 ytmusicapi-1.0.2/ytmusicapi/locales/ur/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/ur/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/ur/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.286473 ytmusicapi-1.0.2/ytmusicapi/locales/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.306473 ytmusicapi-1.0.2/ytmusicapi/locales/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.286473 ytmusicapi-1.0.2/ytmusicapi/locales/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.306473 ytmusicapi-1.0.2/ytmusicapi/locales/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.306473 ytmusicapi-1.0.2/ytmusicapi/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/mixins/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35118 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/mixins/browsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/mixins/explore.py
--rw-r--r--   0 runner    (1001) docker     (123)    13053 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/mixins/library.py
--rw-r--r--   0 runner    (1001) docker     (123)    15802 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/mixins/playlists.py
--rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/mixins/search.py
--rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/mixins/uploads.py
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/mixins/watch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.310473 ytmusicapi-1.0.2/ytmusicapi/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/parsers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/parsers/albums.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/parsers/browsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/parsers/explore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/parsers/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/parsers/library.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/parsers/playlists.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/parsers/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/parsers/songs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/parsers/uploads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/parsers/watch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-04-22 06:55:42.000000 ytmusicapi-1.0.2/ytmusicapi/ytmusic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:56:01.298473 ytmusicapi-1.0.2/ytmusicapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-04-22 06:56:01.000000 ytmusicapi-1.0.2/ytmusicapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-22 06:56:01.000000 ytmusicapi-1.0.2/ytmusicapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 06:56:01.000000 ytmusicapi-1.0.2/ytmusicapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-22 06:56:01.000000 ytmusicapi-1.0.2/ytmusicapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-22 06:56:01.000000 ytmusicapi-1.0.2/ytmusicapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-22 06:56:01.000000 ytmusicapi-1.0.2/ytmusicapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.861526 ytmusicapi-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.845525 ytmusicapi-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.845525 ytmusicapi-1.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.845525 ytmusicapi-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/.github/workflows/docsbuild.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-06-15 18:28:45.857526 ytmusicapi-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.845525 ytmusicapi-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.845525 ytmusicapi-1.1.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/docs/source/reference.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.845525 ytmusicapi-1.1.0/docs/source/setup/
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/docs/source/setup/browser.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/docs/source/setup/headers_auth.json.example
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/docs/source/setup/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/docs/source/setup/oauth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 18:28:45.861526 ytmusicapi-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.849526 ytmusicapi-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/tests/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/tests/test.cfg.example
+-rw-r--r--   0 runner    (1001) docker     (123)    22845 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.849526 ytmusicapi-1.1.0/ytmusicapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.849526 ytmusicapi-1.1.0/ytmusicapi/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/auth/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/auth/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/auth/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/continuations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.849526 ytmusicapi-1.1.0/ytmusicapi/locales/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.849526 ytmusicapi-1.1.0/ytmusicapi/locales/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/ar/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/ar/LC_MESSAGES/base.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/base.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/de/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/de/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/en/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/en/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/es/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/es/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/fr/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/fr/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/hi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/hi/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/hi/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/it/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/it/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/ja/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/ja/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/ko/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/ko/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/ko/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/nl/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/nl/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/pt/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/pt/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/ru/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/ru/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/tr/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/tr/LC_MESSAGES/base.po
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/update_mo.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/update_po.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/ur/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/ur/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/ur/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/ur/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.853526 ytmusicapi-1.1.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.841525 ytmusicapi-1.1.0/ytmusicapi/locales/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.857526 ytmusicapi-1.1.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.857526 ytmusicapi-1.1.0/ytmusicapi/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/mixins/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35118 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/mixins/browsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/mixins/explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13053 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/mixins/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15818 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/mixins/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/mixins/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/mixins/uploads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/mixins/watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.857526 ytmusicapi-1.1.0/ytmusicapi/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/parsers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/parsers/albums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/parsers/browsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/parsers/explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/parsers/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/parsers/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/parsers/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/parsers/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/parsers/songs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/parsers/uploads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/parsers/watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-06-15 18:28:32.000000 ytmusicapi-1.1.0/ytmusicapi/ytmusic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:28:45.849526 ytmusicapi-1.1.0/ytmusicapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-06-15 18:28:45.000000 ytmusicapi-1.1.0/ytmusicapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-15 18:28:45.000000 ytmusicapi-1.1.0/ytmusicapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 18:28:45.000000 ytmusicapi-1.1.0/ytmusicapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 18:28:45.000000 ytmusicapi-1.1.0/ytmusicapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-15 18:28:45.000000 ytmusicapi-1.1.0/ytmusicapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 18:28:45.000000 ytmusicapi-1.1.0/ytmusicapi.egg-info/top_level.txt
```

### Comparing `ytmusicapi-1.0.2/.github/ISSUE_TEMPLATE/bug_report.md` & `ytmusicapi-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/.github/ISSUE_TEMPLATE/feature_request.md` & `ytmusicapi-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/.github/workflows/coverage.yml` & `ytmusicapi-1.1.0/.github/workflows/coverage.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 name: Code coverage
 
 on:
   push:
     branches:
       - '**'
+  pull_request:
+    branches:
+      - master
 
 jobs:
   build:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@master
     - name: Setup Python
```

### Comparing `ytmusicapi-1.0.2/.github/workflows/pythonpublish.yml` & `ytmusicapi-1.1.0/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/CONTRIBUTING.rst` & `ytmusicapi-1.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/LICENSE` & `ytmusicapi-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/PKG-INFO` & `ytmusicapi-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytmusicapi
-Version: 1.0.2
+Version: 1.1.0
 Summary: Unofficial API for YouTube Music
 Author-email: sigma67 <ytmusicapi@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 sigma67
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -62,16 +62,14 @@
 ytmusicapi is a Python 3 library to send requests to the YouTube Music API.
 It emulates YouTube Music web client requests using the user's cookie data for authentication.
 
 .. features
 
 Features
 --------
-At this point ytmusicapi supports nearly all content interactions in the YouTube Music web app.
-If you find something missing or broken, feel free to create an `issue <https://github.com/sigma67/ytmusicapi/issues/new>`_
 
 | **Browsing**:
 
 * search (including all filters) and suggestions
 * get artist information and releases (songs, videos, albums, singles, related artists)
 * get user information (videos, playlists)
 * get albums
@@ -98,14 +96,17 @@
 * get playlist suggestions
 
 | **Uploads**:
 
 * upload songs and remove them again
 * list uploaded songs, artists and albums
 
+If you find something missing or broken,
+check the `FAQ <https://ytmusicapi.readthedocs.io/en/stable/faq.html>`__ or
+feel free to create an `issue <https://github.com/sigma67/ytmusicapi/issues/new/choose>`__.
 
 Usage
 ------
 .. code-block:: python
 
     from ytmusicapi import YTMusic
```

### Comparing `ytmusicapi-1.0.2/README.rst` & `ytmusicapi-1.1.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -25,16 +25,14 @@
 ytmusicapi is a Python 3 library to send requests to the YouTube Music API.
 It emulates YouTube Music web client requests using the user's cookie data for authentication.
 
 .. features
 
 Features
 --------
-At this point ytmusicapi supports nearly all content interactions in the YouTube Music web app.
-If you find something missing or broken, feel free to create an `issue <https://github.com/sigma67/ytmusicapi/issues/new>`_
 
 | **Browsing**:
 
 * search (including all filters) and suggestions
 * get artist information and releases (songs, videos, albums, singles, related artists)
 * get user information (videos, playlists)
 * get albums
@@ -61,14 +59,17 @@
 * get playlist suggestions
 
 | **Uploads**:
 
 * upload songs and remove them again
 * list uploaded songs, artists and albums
 
+If you find something missing or broken,
+check the `FAQ <https://ytmusicapi.readthedocs.io/en/stable/faq.html>`__ or
+feel free to create an `issue <https://github.com/sigma67/ytmusicapi/issues/new/choose>`__.
 
 Usage
 ------
 .. code-block:: python
 
     from ytmusicapi import YTMusic
```

### Comparing `ytmusicapi-1.0.2/docs/Makefile` & `ytmusicapi-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/docs/make.bat` & `ytmusicapi-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/docs/source/conf.py` & `ytmusicapi-1.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/docs/source/index.rst` & `ytmusicapi-1.1.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/docs/source/reference.rst` & `ytmusicapi-1.1.0/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/docs/source/setup/browser.rst` & `ytmusicapi-1.1.0/docs/source/setup/browser.rst`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,16 @@
 
    <details>
    <summary><a>MacOS special pasting instructions</a></summary>
 
 .. container::
 
     - MacOS terminal application can only accept 1024 characters pasted to std input. To paste in terminal, a small utility called pbpaste must be used.
-    - In terminal just prefix the command used to run the script you created above with :kbd:`pbpaste | `
+    - In terminal just prefix the command used to run the script you created above with
+        ``pbpaste |``
     - This will pipe the contents of the clipboard into the script just as if you had pasted it from the edit menu.
 
 .. raw:: html
 
    </details><br>
 
 Manual file creation
```

### Comparing `ytmusicapi-1.0.2/docs/source/usage.rst` & `ytmusicapi-1.1.0/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/pyproject.toml` & `ytmusicapi-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/tests/README.rst` & `ytmusicapi-1.1.0/tests/README.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/tests/test.cfg.example` & `ytmusicapi-1.1.0/tests/test.cfg.example`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/tests/test.py` & `ytmusicapi-1.1.0/tests/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     @classmethod
     def setUpClass(cls):
         warnings.filterwarnings(action="ignore", message="unclosed", category=ResourceWarning)
         with YTMusic(requests_session=False) as yt:
             assert isinstance(yt, YTMusic)
         cls.yt = YTMusic()
         cls.yt_oauth = YTMusic(headers_oauth)
-        cls.yt_auth = YTMusic(headers_browser)
+        cls.yt_auth = YTMusic(headers_browser, location="GB")
         cls.yt_brand = YTMusic(config["auth"]["headers"], config["auth"]["brand_account"])
         cls.yt_empty = YTMusic(config["auth"]["headers_empty"],
                                config["auth"]["brand_account_empty"])
 
     @mock.patch("sys.argv", ["ytmusicapi", "browser", "--file", headers_browser])
     def test_setup_browser(self):
         headers = setup(headers_browser, config["auth"]["headers_raw"])
@@ -158,16 +158,16 @@
     def test_get_artist_albums(self):
         artist = self.yt.get_artist("UCj5ZiBBqpe0Tg4zfKGHEFuQ")
         results = self.yt.get_artist_albums(artist["albums"]["browseId"],
                                             artist["albums"]["params"])
         self.assertGreater(len(results), 0)
 
     def test_get_artist_singles(self):
-        artist = self.yt_auth.get_artist("UCAeLFBCQS7FvI8PvBrWvSBg")
-        results = self.yt_auth.get_artist_albums(artist["singles"]["browseId"],
+        artist = self.yt.get_artist("UCAeLFBCQS7FvI8PvBrWvSBg")
+        results = self.yt.get_artist_albums(artist["singles"]["browseId"],
                                                  artist["singles"]["params"])
         self.assertGreater(len(results), 0)
 
     def test_get_user(self):
         results = self.yt.get_user("UC44hbeRoCZVVMVg5z0FfIww")
         self.assertEqual(len(results), 3)
 
@@ -387,22 +387,23 @@
     ###############
     # PLAYLISTS
     ###############
 
     def test_get_foreign_playlist(self):
         self.assertRaises(Exception, self.yt.get_playlist, "PLABC")
         playlist = self.yt.get_playlist(sample_playlist, limit=300, suggestions_limit=7)
+        self.assertGreater(len(playlist['duration']), 5)
         self.assertGreater(len(playlist["tracks"]), 200)
         self.assertNotIn("suggestions", playlist)
 
-        playlist = self.yt.get_playlist("RDCLAK5uy_kpxnNxJpPZjLKbL9WgvrPuErWkUxMP6x4",
-                                        limit=None,
-                                        related=True)
-        self.assertGreater(len(playlist["tracks"]), 100)
-        self.assertEqual(len(playlist["related"]), 10)
+        playlist = self.yt_oauth.get_playlist("PLj4BSJLnVpNyIjbCWXWNAmybc97FXLlTk",
+                                              limit=None,
+                                              related=True)
+        self.assertGreater(len(playlist["tracks"]), 200)
+        self.assertEqual(len(playlist["related"]), 0)
 
     def test_get_owned_playlist(self):
         playlist = self.yt_brand.get_playlist(config["playlists"]["own"],
                                               related=True,
                                               suggestions_limit=21)
         self.assertLess(len(playlist["tracks"]), 100)
         self.assertEqual(len(playlist["suggestions"]), 21)
```

### Comparing `ytmusicapi-1.0.2/ytmusicapi/auth/browser.py` & `ytmusicapi-1.1.0/ytmusicapi/auth/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ytmusicapi.helpers import *
 
 path = os.path.dirname(os.path.realpath(__file__)) + os.sep
 
 
 def is_browser(headers: CaseInsensitiveDict) -> bool:
     browser_structure = {"authorization", "cookie"}
-    return browser_structure.issubset(headers.keys())
+    return all(key in headers for key in browser_structure)
 
 
 def setup_browser(filepath=None, headers_raw=None):
     contents = []
     if not headers_raw:
         eof = "Ctrl-D" if platform.system() != "Windows" else "'Enter, Ctrl-Z, Enter'"
         print(f"Please paste the request headers from Firefox and press {eof} to continue:")
```

### Comparing `ytmusicapi-1.0.2/ytmusicapi/auth/headers.py` & `ytmusicapi-1.1.0/ytmusicapi/auth/headers.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 from typing import Dict, Optional
 
 import requests
 from requests.structures import CaseInsensitiveDict
 
 from ytmusicapi.auth.browser import is_browser
-from ytmusicapi.auth.oauth import YTMusicOAuth, is_oauth
+from ytmusicapi.auth.oauth import YTMusicOAuth, is_oauth, is_custom_oauth
 from ytmusicapi.helpers import initialize_headers
 
 
 def load_headers_file(auth: str) -> Dict:
     if os.path.isfile(auth):
         with open(auth) as json_file:
             input_json = json.load(json_file)
@@ -32,14 +32,17 @@
         if is_oauth(input_dict):
             oauth = YTMusicOAuth(session, proxies)
             headers = oauth.load_headers(dict(input_dict), auth)
 
         elif is_browser(input_dict):
             headers = input_dict
 
+        elif is_custom_oauth(input_dict):
+            headers = input_dict
+
         else:
             raise Exception(
                 "Could not detect credential type. "
                 "Please ensure your oauth or browser credentials are set up correctly.")
 
     else:  # no authentication
         headers = initialize_headers()
```

### Comparing `ytmusicapi-1.0.2/ytmusicapi/auth/oauth.py` & `ytmusicapi-1.1.0/ytmusicapi/auth/oauth.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import time
+import webbrowser
 from typing import Dict, Optional
 
 import requests
 from requests.structures import CaseInsensitiveDict
 
 from ytmusicapi.constants import (OAUTH_CLIENT_ID, OAUTH_CLIENT_SECRET, OAUTH_CODE_URL,
                                   OAUTH_SCOPE, OAUTH_TOKEN_URL, OAUTH_USER_AGENT)
@@ -14,15 +15,20 @@
     oauth_structure = {
         "access_token",
         "expires_at",
         "expires_in",
         "token_type",
         "refresh_token",
     }
-    return oauth_structure.issubset(headers.keys())
+    return all(key in headers for key in oauth_structure)
+
+
+def is_custom_oauth(headers: CaseInsensitiveDict) -> bool:
+    """Checks whether the headers contain a Bearer token, indicating a custom OAuth implementation."""
+    return "authorization" in headers and headers["authorization"].startswith("Bearer ")
 
 
 class YTMusicOAuth:
     """OAuth implementation for YouTube Music based on YouTube TV"""
 
     def __init__(self, session: requests.Session, proxies: Dict = None):
         self._session = session
@@ -70,17 +76,19 @@
     @staticmethod
     def dump_token(token: Dict, filepath: Optional[str]):
         if not filepath or len(filepath) > 255:
             return
         with open(filepath, encoding="utf8", mode="w") as file:
             json.dump(token, file, indent=True)
 
-    def setup(self, filepath: Optional[str] = None) -> Dict:
+    def setup(self, filepath: Optional[str] = None, open_browser: bool = False) -> Dict:
         code = self.get_code()
         url = f"{code['verification_url']}?user_code={code['user_code']}"
+        if open_browser:
+            webbrowser.open(url)
         input(f"Go to {url}, finish the login flow and press Enter when done, Ctrl-C to abort")
         token = self.get_token_from_code(code["device_code"])
         self.dump_token(token, filepath)
 
         return token
 
     def load_headers(self, token: Dict, filepath: Optional[str] = None):
```

### Comparing `ytmusicapi-1.0.2/ytmusicapi/continuations.py` & `ytmusicapi-1.1.0/ytmusicapi/continuations.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/helpers.py` & `ytmusicapi-1.1.0/ytmusicapi/helpers.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/README.rst` & `ytmusicapi-1.1.0/ytmusicapi/locales/README.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/ar/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.0/ytmusicapi/locales/ar/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/ar/LC_MESSAGES/base.po` & `ytmusicapi-1.1.0/ytmusicapi/locales/ar/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/base.pot` & `ytmusicapi-1.1.0/ytmusicapi/locales/base.pot`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/de/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.0/ytmusicapi/locales/de/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/de/LC_MESSAGES/base.po` & `ytmusicapi-1.1.0/ytmusicapi/locales/de/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/en/LC_MESSAGES/base.po` & `ytmusicapi-1.1.0/ytmusicapi/locales/en/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/es/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.0/ytmusicapi/locales/es/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/es/LC_MESSAGES/base.po` & `ytmusicapi-1.1.0/ytmusicapi/locales/es/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/fr/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.0/ytmusicapi/locales/fr/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/fr/LC_MESSAGES/base.po` & `ytmusicapi-1.1.0/ytmusicapi/locales/fr/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/hi/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.0/ytmusicapi/locales/hi/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/hi/LC_MESSAGES/base.po` & `ytmusicapi-1.1.0/ytmusicapi/locales/hi/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/it/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.0/ytmusicapi/locales/it/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/it/LC_MESSAGES/base.po` & `ytmusicapi-1.1.0/ytmusicapi/locales/it/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/ja/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.0/ytmusicapi/locales/ja/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/ja/LC_MESSAGES/base.po` & `ytmusicapi-1.1.0/ytmusicapi/locales/ja/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/ko/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.0/ytmusicapi/locales/ko/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/ko/LC_MESSAGES/base.po` & `ytmusicapi-1.1.0/ytmusicapi/locales/ko/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/pt/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.0/ytmusicapi/locales/pt/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/pt/LC_MESSAGES/base.po` & `ytmusicapi-1.1.0/ytmusicapi/locales/pt/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/ru/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.0/ytmusicapi/locales/ru/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/ru/LC_MESSAGES/base.po` & `ytmusicapi-1.1.0/ytmusicapi/locales/ru/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/tr/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.0/ytmusicapi/locales/tr/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/tr/LC_MESSAGES/base.po` & `ytmusicapi-1.1.0/ytmusicapi/locales/tr/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/ur/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.0/ytmusicapi/locales/ur/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/ur/LC_MESSAGES/base.po` & `ytmusicapi-1.1.0/ytmusicapi/locales/ur/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.pot` & `ytmusicapi-1.1.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.pot`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo` & `ytmusicapi-1.1.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po` & `ytmusicapi-1.1.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/mixins/_utils.py` & `ytmusicapi-1.1.0/ytmusicapi/mixins/_utils.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/mixins/browsing.py` & `ytmusicapi-1.1.0/ytmusicapi/mixins/browsing.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/mixins/explore.py` & `ytmusicapi-1.1.0/ytmusicapi/mixins/explore.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/mixins/library.py` & `ytmusicapi-1.1.0/ytmusicapi/mixins/library.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/mixins/playlists.py` & `ytmusicapi-1.1.0/ytmusicapi/mixins/playlists.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,28 +129,28 @@
                 'name': nav(header, SUBTITLE2),
                 'id': nav(header, SUBTITLE_RUNS + [2] + NAVIGATION_BROWSE_ID, True)
             }
             if run_count == 5:
                 playlist['year'] = nav(header, SUBTITLE3)
 
         second_subtitle_runs = header['secondSubtitle']['runs']
-        own_offset = (own_playlist and len(second_subtitle_runs) > 3) * 2
-        song_count = to_int(second_subtitle_runs[own_offset]['text'])
-        if len(second_subtitle_runs) > 1:
-            playlist['duration'] = second_subtitle_runs[own_offset + 2]['text']
 
+        has_views = (len(second_subtitle_runs) > 3) * 2
+        playlist['views'] = None if not has_views else to_int(second_subtitle_runs[0]['text'])
+        has_duration = (len(second_subtitle_runs) > 1) * 2
+        playlist['duration'] = None if not has_duration else second_subtitle_runs[has_views + has_duration]['text']
+        song_count = second_subtitle_runs[has_views + 0]['text'].split(" ")
+        song_count = to_int(song_count[0]) if len(song_count) > 1 else 0
         playlist['trackCount'] = song_count
-        playlist['views'] = None
-        if own_playlist:
-            playlist['views'] = to_int(second_subtitle_runs[0]['text'])
 
         request_func = lambda additionalParams: self._send_request(endpoint, body, additionalParams)
 
         # suggestions and related are missing e.g. on liked songs
         section_list = nav(response, SINGLE_COLUMN_TAB + ['sectionListRenderer'])
+        playlist['related'] = []
         if 'continuations' in section_list:
             additionalParams = get_continuation_params(section_list)
             if own_playlist and (suggestions_limit > 0 or related):
                 parse_func = lambda results: parse_playlist_items(results)
                 suggested = request_func(additionalParams)
                 continuation = nav(suggested, SECTION_LIST_CONTINUATION)
                 additionalParams = get_continuation_params(continuation)
@@ -164,31 +164,29 @@
                                       suggestions_limit - len(playlist['suggestions']),
                                       request_func,
                                       parse_func,
                                       reloadable=True))
 
             if related:
                 response = request_func(additionalParams)
-                continuation = nav(response, SECTION_LIST_CONTINUATION)
-                parse_func = lambda results: parse_content_list(results, parse_playlist)
-                playlist['related'] = get_continuation_contents(
-                    nav(continuation, CONTENT + CAROUSEL), parse_func)
+                continuation = nav(response, SECTION_LIST_CONTINUATION, True)
+                if continuation:
+                    parse_func = lambda results: parse_content_list(results, parse_playlist)
+                    playlist['related'] = get_continuation_contents(
+                        nav(continuation, CONTENT + CAROUSEL), parse_func)
 
-        if song_count > 0:
+        playlist['tracks'] = []
+        if 'contents' in results:
             playlist['tracks'] = parse_playlist_items(results['contents'])
-            if limit is None:
-                limit = song_count
-            songs_to_get = min(limit, song_count)
 
             parse_func = lambda contents: parse_playlist_items(contents)
             if 'continuations' in results:
                 playlist['tracks'].extend(
-                    get_continuations(results, 'musicPlaylistShelfContinuation',
-                                      songs_to_get - len(playlist['tracks']), request_func,
-                                      parse_func))
+                    get_continuations(results, 'musicPlaylistShelfContinuation', limit,
+                                      request_func, parse_func))
 
         playlist['duration_seconds'] = sum_total_duration(playlist)
         return playlist
 
     def create_playlist(self,
                         title: str,
                         description: str,
```

### Comparing `ytmusicapi-1.0.2/ytmusicapi/mixins/search.py` & `ytmusicapi-1.1.0/ytmusicapi/mixins/search.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/mixins/uploads.py` & `ytmusicapi-1.1.0/ytmusicapi/mixins/uploads.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/mixins/watch.py` & `ytmusicapi-1.1.0/ytmusicapi/mixins/watch.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/navigation.py` & `ytmusicapi-1.1.0/ytmusicapi/navigation.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/parsers/_utils.py` & `ytmusicapi-1.1.0/ytmusicapi/parsers/_utils.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/parsers/albums.py` & `ytmusicapi-1.1.0/ytmusicapi/parsers/albums.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/parsers/browsing.py` & `ytmusicapi-1.1.0/ytmusicapi/parsers/browsing.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/parsers/explore.py` & `ytmusicapi-1.1.0/ytmusicapi/parsers/explore.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/parsers/i18n.py` & `ytmusicapi-1.1.0/ytmusicapi/parsers/i18n.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/parsers/library.py` & `ytmusicapi-1.1.0/ytmusicapi/parsers/library.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/parsers/playlists.py` & `ytmusicapi-1.1.0/ytmusicapi/parsers/playlists.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/parsers/search.py` & `ytmusicapi-1.1.0/ytmusicapi/parsers/search.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/parsers/songs.py` & `ytmusicapi-1.1.0/ytmusicapi/parsers/songs.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/parsers/uploads.py` & `ytmusicapi-1.1.0/ytmusicapi/parsers/uploads.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/parsers/watch.py` & `ytmusicapi-1.1.0/ytmusicapi/parsers/watch.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.2/ytmusicapi/setup.py` & `ytmusicapi-1.1.0/ytmusicapi/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,28 +20,30 @@
     :return: configuration headers string
     """
     return setup_browser(filepath, headers_raw)
 
 
 def setup_oauth(filepath: str = None,
                 session: requests.Session = None,
-                proxies: dict = None) -> Dict:
+                proxies: dict = None,
+                open_browser: bool = False) -> Dict:
     """
     Starts oauth flow from the terminal
     and returns a string that can be passed to YTMusic()
 
     :param session: Session to use for authentication
     :param proxies: Proxies to use for authentication
     :param filepath: Optional filepath to store headers to.
+    :param open_browser: If True, open the default browser with the setup link
     :return: configuration headers string
     """
     if not session:
         session = requests.Session()
 
-    return YTMusicOAuth(session, proxies).setup(filepath)
+    return YTMusicOAuth(session, proxies).setup(filepath, open_browser)
 
 
 def parse_args(args):
     parser = argparse.ArgumentParser(description='Setup ytmusicapi.')
     parser.add_argument("setup_type",
                         type=str,
                         choices=["oauth", "browser"],
@@ -50,9 +52,11 @@
     return parser.parse_args(args)
 
 
 def main():
     args = parse_args(sys.argv[1:])
     filename = args.file.as_posix() if args.file else f"{args.setup_type}.json"
     print(f"Creating {filename} with your authentication credentials...")
-    func = setup_oauth if args.setup_type == "oauth" else setup
-    return func(filename)
+    if args.setup_type == "oauth":
+        return setup_oauth(filename, open_browser=True)
+    else:
+        return setup(filename)
```

### Comparing `ytmusicapi-1.0.2/ytmusicapi/ytmusic.py` & `ytmusicapi-1.1.0/ytmusicapi/ytmusic.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,16 @@
     """
 
     def __init__(self,
                  auth: str = None,
                  user: str = None,
                  requests_session=True,
                  proxies: dict = None,
-                 language: str = 'en'):
+                 language: str = 'en',
+                 location: str = ''):
         """
         Create a new instance to interact with YouTube Music.
 
         :param auth: Optional. Provide a string or path to file.
           Authentication credentials are needed to manage your library.
           See :py:func:`setup` for how to fill in the correct credentials.
           Default: A default header is used without authentication.
@@ -58,14 +59,17 @@
 
             .. _requests: https://requests.readthedocs.io/
             .. _format: https://requests.readthedocs.io/en/master/user/advanced/#proxies
 
         :param language: Optional. Can be used to change the language of returned data.
             English will be used by default. Available languages can be checked in
             the ytmusicapi/locales directory.
+        :param location: Optional. Can be used to change the location of the user.
+            No location will be set by default. This means it is determined by the server.
+            Available languages can be checked in the FAQ.
         """
         self.auth = auth
 
         if isinstance(requests_session, requests.Session):
             self._session = requests_session
         else:
             if requests_session:  # Build a new session.
@@ -80,26 +84,32 @@
         self.headers = prepare_headers(self._session, proxies, auth)
 
         if 'x-goog-visitor-id' not in self.headers:
             self.headers.update(get_visitor_id(self._send_get_request))
 
         # prepare context
         self.context = initialize_context()
-        self.context['context']['client']['hl'] = language
-        locale_dir = os.path.abspath(os.path.dirname(__file__)) + os.sep + 'locales'
-        supported_languages = [f for f in next(os.walk(locale_dir))[1]]
-        if language not in supported_languages:
+
+        if location:
+            if location not in SUPPORTED_LOCATIONS:
+                raise Exception("Location not supported. Check the FAQ for supported locations.")
+            self.context['context']['client']['gl'] = location
+
+        if language not in SUPPORTED_LANGUAGES:
             raise Exception("Language not supported. Supported languages are "
-                            + (', '.join(supported_languages)) + ".")
+                            + (', '.join(SUPPORTED_LANGUAGES)) + ".")
+        self.context['context']['client']['hl'] = language
         self.language = language
         try:
             locale.setlocale(locale.LC_ALL, self.language)
         except locale.Error:
             with suppress(locale.Error):
                 locale.setlocale(locale.LC_ALL, 'en_US.UTF-8')
+
+        locale_dir = os.path.abspath(os.path.dirname(__file__)) + os.sep + 'locales'
         self.lang = gettext.translation('base', localedir=locale_dir, languages=[language])
         self.parser = Parser(self.lang)
 
         if user:
             self.context['context']['user']['onBehalfOfUser'] = user
 
         auth_header = self.headers.get("authorization")
```

### Comparing `ytmusicapi-1.0.2/ytmusicapi.egg-info/PKG-INFO` & `ytmusicapi-1.1.0/ytmusicapi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytmusicapi
-Version: 1.0.2
+Version: 1.1.0
 Summary: Unofficial API for YouTube Music
 Author-email: sigma67 <ytmusicapi@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 sigma67
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -62,16 +62,14 @@
 ytmusicapi is a Python 3 library to send requests to the YouTube Music API.
 It emulates YouTube Music web client requests using the user's cookie data for authentication.
 
 .. features
 
 Features
 --------
-At this point ytmusicapi supports nearly all content interactions in the YouTube Music web app.
-If you find something missing or broken, feel free to create an `issue <https://github.com/sigma67/ytmusicapi/issues/new>`_
 
 | **Browsing**:
 
 * search (including all filters) and suggestions
 * get artist information and releases (songs, videos, albums, singles, related artists)
 * get user information (videos, playlists)
 * get albums
@@ -98,14 +96,17 @@
 * get playlist suggestions
 
 | **Uploads**:
 
 * upload songs and remove them again
 * list uploaded songs, artists and albums
 
+If you find something missing or broken,
+check the `FAQ <https://ytmusicapi.readthedocs.io/en/stable/faq.html>`__ or
+feel free to create an `issue <https://github.com/sigma67/ytmusicapi/issues/new/choose>`__.
 
 Usage
 ------
 .. code-block:: python
 
     from ytmusicapi import YTMusic
```

### Comparing `ytmusicapi-1.0.2/ytmusicapi.egg-info/SOURCES.txt` & `ytmusicapi-1.1.0/ytmusicapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,16 @@
 ytmusicapi/locales/hi/LC_MESSAGES/base.po
 ytmusicapi/locales/it/LC_MESSAGES/base.mo
 ytmusicapi/locales/it/LC_MESSAGES/base.po
 ytmusicapi/locales/ja/LC_MESSAGES/base.mo
 ytmusicapi/locales/ja/LC_MESSAGES/base.po
 ytmusicapi/locales/ko/LC_MESSAGES/base.mo
 ytmusicapi/locales/ko/LC_MESSAGES/base.po
+ytmusicapi/locales/nl/LC_MESSAGES/base.mo
+ytmusicapi/locales/nl/LC_MESSAGES/base.po
 ytmusicapi/locales/pt/LC_MESSAGES/base.mo
 ytmusicapi/locales/pt/LC_MESSAGES/base.po
 ytmusicapi/locales/ru/LC_MESSAGES/base.mo
 ytmusicapi/locales/ru/LC_MESSAGES/base.po
 ytmusicapi/locales/tr/LC_MESSAGES/base.mo
 ytmusicapi/locales/tr/LC_MESSAGES/base.po
 ytmusicapi/locales/ur/LC_MESSAGES/base.mo
```

