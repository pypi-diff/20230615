# Comparing `tmp/bulma_sphinx_theme-0.1.0rc1.tar.gz` & `tmp/bulma_sphinx_theme-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bulma_sphinx_theme-0.1.0rc1.tar", last modified: Wed Jun  7 05:08:57 2023, max compression
+gzip compressed data, was "bulma_sphinx_theme-0.2.0rc1.tar", last modified: Thu Jun 15 03:33:51 2023, max compression
```

## Comparing `bulma_sphinx_theme-0.1.0rc1.tar` & `bulma_sphinx_theme-0.2.0rc1.tar`

### file list

```diff
@@ -1,202 +1,224 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:57.788139 bulma_sphinx_theme-0.1.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-07 05:08:39.760347 bulma_sphinx_theme-0.1.0rc1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-07 05:08:39.760347 bulma_sphinx_theme-0.1.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-07 05:08:39.760347 bulma_sphinx_theme-0.1.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-07 05:08:39.760347 bulma_sphinx_theme-0.1.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.760347 bulma_sphinx_theme-0.1.0rc1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-06-07 05:08:39.760347 bulma_sphinx_theme-0.1.0rc1/docs/_static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-07 05:08:39.760347 bulma_sphinx_theme-0.1.0rc1/docs/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-07 05:08:39.760347 bulma_sphinx_theme-0.1.0rc1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-07 05:08:39.760347 bulma_sphinx_theme-0.1.0rc1/docs/examples/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-07 05:08:39.760347 bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/admonitions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/blocks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/generic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/images.rst
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/lists.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/really-long.md
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/sphinx-design.md
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/tables.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/typography.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/mult_headers.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/admonitions.md
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/api.md
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/code-blocks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/hyperlinks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/images.md
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/lists.md
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/tables.md
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/tabs.md
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/text-formatting.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subpage1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subpage2.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subsubpages/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subsubpages/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subsubpages/subsubpage1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subsubpages/subsubpage2.rst
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subsubpages/subsubpage3.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subsubpages/subsubsubpages/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subsubpages/subsubsubpages/subsubsubpage1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/user_guide/develop.md
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/user_guide/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/user_guide/navbar.md
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/user_guide/search.md
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/user_guide/sidenav.md
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/user_guide/source.md
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/user_guide/theme-elements.md
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/user_guide/web-components.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)   130410 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/postcss.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js
--rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/base/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/base/_icons.scss
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/base/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/base/_typography.scss
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/bulma-sphinx-theme.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_article-bottom.scss
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_article-top.scss
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_brand-logo.scss
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_breadcrumbs.scss
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_edit-page.scss
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_info-panel.scss
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_last-updated.scss
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_search-field.sass
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_search-icon.scss
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_search-results.scss
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_search-wrapper.scss
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_search.sass
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_sidenav-brand.scss
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_api.scss
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_blocks.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_code.scss
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_gui-labels.scss
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_images.sass
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_indexes.sass
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_lists.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_math.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_misc.sass
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_rubrics.sass
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_tables.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_target.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_ablog.scss
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_bulma.scss
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_leaflet.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_notebooks.scss
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_sphinx-design.scss
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_togglebutton.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_bulma-content.scss
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_bulma-main.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/variables/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_color.scss
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_layout.scss
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_spacing.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/translations/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/translations/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/translations/jsons/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/translations/jsons/Back to top.json
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/translations/jsons/last update.json
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/translations/jsons/with.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/demo/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/demo/sphinxext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/pygment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/back-to-top.html
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/brand-logo.html
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/copyright.html
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/icon-links.html
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/info-panel.html
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/navbar-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-icon.html
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-wrapper.html
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/searchbox.html
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sphinx-version.html
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/toggle-sidenav.html
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_css_variables_define.html
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/icons.html
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/sidenav.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf
--rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/toctree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/translations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/webpack.config.js
--rw-r--r--   0        0        0     4453 1970-01-01 00:00:00.000000 bulma_sphinx_theme-0.1.0rc1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:51.686626 bulma_sphinx_theme-0.2.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/_static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/_static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/_templates/megamenu.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/blog/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/blog/post1.md
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/blog/post2.md
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/blog/post3.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/blog/post4.md
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/kitchen-sink/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/kitchen-sink/admonitions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/kitchen-sink/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/kitchen-sink/blocks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/kitchen-sink/generic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/kitchen-sink/images.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/kitchen-sink/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/kitchen-sink/lists.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/kitchen-sink/really-long.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/kitchen-sink/sphinx-design.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/kitchen-sink/structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/kitchen-sink/tables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/kitchen-sink/typography.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/mult_headers.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/reference/admonitions.md
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/reference/code-blocks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/reference/hyperlinks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/reference/images.md
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/reference/lists.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/reference/tables.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/reference/tabs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/reference/text-formatting.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/subpages/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/subpages/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/subpages/subpage1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/subpages/subpage2.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/subpages/subsubpages/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/subpages/subsubpages/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/subpages/subsubpages/subsubpage1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/subpages/subsubpages/subsubpage2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/subpages/subsubpages/subsubpage3.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/subpages/subsubpages/subsubsubpages/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/subpages/subsubpages/subsubsubpages/subsubsubpage1.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/test_page/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/test_page/fullwidth.md
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/test_page/hidesidenav.md
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/test_page/hidetoc.md
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/test_page/hidetocnav.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/examples/test_page/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/user_guide/ablog.md
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/user_guide/bulma-extensions.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/user_guide/develop.md
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/user_guide/fonts.md
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/user_guide/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/user_guide/landing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/user_guide/navbar.md
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/user_guide/search.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/user_guide/sidenav.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/user_guide/source.md
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/user_guide/styling.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/user_guide/theme-elements.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/docs/user_guide/web-components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-15 03:33:29.826020 bulma_sphinx_theme-0.2.0rc1/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130410 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/postcss.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    12202 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/base/_icons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/base/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/base/_typography.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/bulma-sphinx-theme.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/components/_article-bottom.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/components/_article-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/components/_brand.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/components/_breadcrumbs.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/components/_edit-page.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/components/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/components/_last-updated.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/components/_search-field.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/components/_search-icon.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/components/_search-results.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/components/_search-wrapper.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/components/_search.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/components/_sidenav-brand.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/components/_sidenav-panel.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/_api.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/_blocks.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/_code.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/_gui-labels.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/_images.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/_indexes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/_lists.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/_math.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/_misc.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/_rubrics.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/_tables.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/_target.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_ablog.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_bulma-megamenu.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_bulma.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_leaflet.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_notebooks.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_sphinx-design.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_togglebutton.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_bulma-content.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_bulma-main.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_color.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_layout.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_spacing.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/translations/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/translations/jsons/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/translations/jsons/Back to top.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/translations/jsons/last update.json
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/translations/jsons/with.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/demo/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/demo/sphinxext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/pygment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/back-to-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/brand.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/copyright.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/icon-links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/navbar-nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/page-toc.html
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-15 03:33:29.830021 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-icon.html
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-wrapper.html
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sphinx-version.html
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/toggle-sidenav.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_css_variables_define.html
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/icons.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/sidenav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/tocnav.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/toctree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-15 03:33:29.834020 bulma_sphinx_theme-0.2.0rc1/webpack.config.js
+-rw-r--r--   0        0        0     4449 1970-01-01 00:00:00.000000 bulma_sphinx_theme-0.2.0rc1/PKG-INFO
```

### Comparing `bulma_sphinx_theme-0.1.0rc1/LICENSE` & `bulma_sphinx_theme-0.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/README.md` & `bulma_sphinx_theme-0.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/_static/favicon.png` & `bulma_sphinx_theme-0.2.0rc1/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/_static/logo.svg` & `bulma_sphinx_theme-0.2.0rc1/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/conf.py` & `bulma_sphinx_theme-0.2.0rc1/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "sphinx_inline_tabs",
     "sphinx_design",
     "sphinx_copybutton",
     "sphinx_togglebutton",
     "sphinx_subfigure",
     "bulma_sphinx_theme.demo.sphinxext",
     "myst_parser",
-    # "ablog",
+    "ablog",
     # "jupyter_sphinx",
     # "myst_nb",
     # "matplotlib.sphinxext.plot_directive",
 ]
 
 
 myst_enable_extensions = ["colon_fence", "deflist"]
@@ -105,37 +105,31 @@
     ],
     "source_repository": "https://github.com/zclab/bulma-sphinx-theme",
     "source_branch": "main",
     "source_directory": "docs/",
     "use_edit_page_button": True,
     "fix_navbar": True,
     "have_top_navbar": True,
+    "navbar_start": ["navbar-nav.html", "megamenu.html"],
 }
 
 html_context = {"default_mode": "auto"}
 
-# blog_path = "blog"
+blog_path = "examples/blog/index"
+blog_authors = {
+    "zclab": ("子川", "https://github.com/zclab"),
+}
 # blog_post_pattern = "posts/*/*"
-# blog_authors = {
-#     "zclab": ("子川", "https://github.com/zclab"),
-# }
-
-# html_sidebars = {
-#     "posts/**": [
-#         "ablog/postcard.html",
-#         "ablog/categories.html",
-#         "ablog/tagcloud.html",
-#         "ablog/recentposts.html",
-#     ],
-#     "blog": [
-#         "ablog/categories.html",
-#         "ablog/tagcloud.html",
-#         "ablog/archives.html",
-#         "ablog/recentposts.html",
-#     ],
-#     "blog/**": [
-#         "ablog/categories.html",
-#         "ablog/tagcloud.html",
-#         "ablog/archives.html",
-#         "ablog/recentposts.html",
-#     ],
-# }
+
+html_sidebars = {
+    "examples/blog/*": [
+        "sidenav-panel.html",
+        "ablog/postcard.html",
+        "ablog/recentposts.html",
+        "ablog/tagcloud.html",
+        "ablog/categories.html",
+        "ablog/authors.html",
+        "ablog/languages.html",
+        "ablog/locations.html",
+        "ablog/archives.html",
+    ],
+}
```

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/index.md` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/index.md`

 * *Files 19% similar despite different names*

```diff
@@ -17,11 +17,12 @@
 ```
 
 ```{toctree}
 :caption: Reference and test section
 :maxdepth: 2
 :numbered:
 
+test_page/index
 subpages/index
 mult_headers
 Link to an external site <https://github.com>
 ```
```

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/admonitions.rst` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/kitchen-sink/admonitions.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/api.rst` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/kitchen-sink/api.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/blocks.rst` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/kitchen-sink/blocks.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/generic.rst` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/kitchen-sink/generic.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/images.rst` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/kitchen-sink/images.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/index.md` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/kitchen-sink/index.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/lists.rst` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/kitchen-sink/lists.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/really-long.md` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/kitchen-sink/really-long.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/sphinx-design.md` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/kitchen-sink/sphinx-design.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/structure.rst` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/kitchen-sink/structure.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/tables.rst` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/kitchen-sink/tables.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/typography.rst` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/kitchen-sink/typography.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/mult_headers.rst` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/mult_headers.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/admonitions.md` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/reference/admonitions.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/api.md` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/reference/api.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/code-blocks.md` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/reference/code-blocks.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/hyperlinks.md` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/reference/hyperlinks.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/images.md` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/reference/images.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/index.md` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/reference/index.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/lists.md` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/reference/lists.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/tables.md` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/reference/tables.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/tabs.md` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/reference/tabs.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/text-formatting.md` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/reference/text-formatting.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subpage1.rst` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/subpages/subpage1.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subpage2.rst` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/subpages/subpage2.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subsubpages/subsubpage1.rst` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/subpages/subsubpages/subsubpage1.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subsubpages/subsubpage2.rst` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/subpages/subsubpages/subsubpage2.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subsubpages/subsubpage3.rst` & `bulma_sphinx_theme-0.2.0rc1/docs/examples/subpages/subsubpages/subsubpage3.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/user_guide/navbar.md` & `bulma_sphinx_theme-0.2.0rc1/docs/user_guide/navbar.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/user_guide/sidenav.md` & `bulma_sphinx_theme-0.2.0rc1/docs/user_guide/sidenav.md`

 * *Files 22% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ## Changing sidenav width
 
 Bulma sphinx theme allows specifying the width of sidenav, the sidenav width is `20%` by default. To change the width, you need to provide the `sidenav-width` css variable configuration value to Bulma sphinx theme, for example,
 
 ```python
 html_theme_options = {
     "css_variables": {
-        "sidenav-width": "20%",
+        "sidenav-width": "320px",
     }
 }
 ```
 
 ## Changing sidenav background
 
 We can also specify the sidenav background (light color or dark color). To change the background, you need to provide the `bst-color-background-sidenav` color variable value to Bulma sphinx theme, for example,
```

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/user_guide/source.md` & `bulma_sphinx_theme-0.2.0rc1/docs/user_guide/source.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/user_guide/theme-elements.md` & `bulma_sphinx_theme-0.2.0rc1/docs/user_guide/theme-elements.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/docs/user_guide/web-components.rst` & `bulma_sphinx_theme-0.2.0rc1/docs/user_guide/web-components.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/noxfile.py` & `bulma_sphinx_theme-0.2.0rc1/noxfile.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,23 +22,14 @@
     session.install("-r", "docs/requirements.txt")
     session.install("-e", ".", "sphinx-theme-builder[cli]")
 
     # Generate documentation into `build/docs`
     session.run("stb", "serve", "docs/", *session.posargs)
 
 
-@nox.session(name="docs-deploy", reuse_venv=True)
-def docs_deploy(session):
-    session.install("-r", "docs/requirements.txt")
-    session.install(".")
-
-    # Generate documentation into `build/docs`
-    session.run("make", "build", external=True)
-
-
 @nox.session(reuse_venv=True)
 def lint(session):
     session.install("pre-commit")
 
     args = list(session.posargs)
     args.append("--all-files")
     if "CI" in os.environ:
```

### Comparing `bulma_sphinx_theme-0.1.0rc1/package-lock.json` & `bulma_sphinx_theme-0.2.0rc1/package-lock.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/package.json` & `bulma_sphinx_theme-0.2.0rc1/package.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/pyproject.toml` & `bulma_sphinx_theme-0.2.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   "sphinx-basic-ng",
   "pygments >= 2.7",
 ]
 
 license = { file = "LICENSE" }
 authors = [{ name = "zclab", email = "syfhub@hotmail.com" }]
 classifiers = [
-  "Development Status :: 2 - Pre-Alpha",
+  "Development Status :: 3 - Alpha",
   "Framework :: Sphinx",
   "Framework :: Sphinx :: Theme",
   "License :: OSI Approved :: MIT License",
   "Environment :: Web Environment",
   "Intended Audience :: Developers",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
@@ -65,8 +65,8 @@
 profile = "jinja"
 extension = "html"
 indent = 2
 max_line_length = 120
 use_gitignore = true
 format_js = true
 format_css = true
-ignore = "H006,J018,T003,H025"
+ignore = "H006,J018,T003,H025,H030"
```

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -342,42 +342,69 @@
 /*******************************************************************************
  * dropdown trigger ended
  */
 
 /*******************************************************************************
  * https://bulma.io/documentation/components/navbar/#navbar-menu
  */
-function navbarBurger() {
+function toggleBurger(selector, target_selector) {
     // Get all "navbar-burger" elements
-    const $navbarBurgers = Array.prototype.slice.call(
-        document.querySelectorAll(".navbar-burger"),
+    const $toggleBurgers = Array.prototype.slice.call(
+        document.querySelectorAll(selector),
         0,
     );
 
-    // Add a click event on each of them
-    $navbarBurgers.forEach((el) => {
-        el.addEventListener("click", () => {
-            // Get the target from the "data-target" attribute
-            const target = el.dataset.target;
+    if ($toggleBurgers.length > 0) {
+        // Add a click event on each of them
+        $toggleBurgers.forEach(function($el) {
+            $el.addEventListener("click", function(event) {
+                // Get the target from the "data-target" attribute
+                const target = $el.dataset.target;
+                const $target = document.getElementById(target);
+
+                // Toggle the "is-active" class on both the "navbar-burger" and the "navbar-menu"
+                event.stopPropagation();
+                $el.classList.toggle("is-active");
+                $target.classList.toggle("is-active");
+            });
+        });
+
+        // see https://segmentfault.com/q/1010000000452465 for close navburger when click empty place
+        // and https://g-dragon.gitbooks.io/-javascript/content/di-si-zhang-shi-li/83001-pan-duan-shi-jian-fa-sheng-zai-mou-ge-div-wai.html
+        document.addEventListener("click", function(event) {
+            var _con = document.querySelector(target_selector);
+            if (!_con.contains(event.target) && !(_con == event.target)) {
+                closetoggleBurgers();
+            }
+        });
+    }
+
+    function closetoggleBurgers() {
+        $toggleBurgers.forEach(function($el) {
+            const target = $el.dataset.target;
             const $target = document.getElementById(target);
 
-            // Toggle the "is-active" class on both the "navbar-burger" and the "navbar-menu"
-            el.classList.toggle("is-active");
-            $target.classList.toggle("is-active");
+            $el.classList.remove("is-active");
+            $target.classList.remove("is-active");
         });
-    });
+    }
+}
+
+function setupToggleButton() {
+    toggleBurger(".navbar .navbar-burger", "#navbarMenu");
+    toggleBurger(".bulma-content .navbar-burger", "#sidenavMenu");
 }
 ////////////////////////////////////////////////////////////////////////////////
 // Main entrypoint
 ////////////////////////////////////////////////////////////////////////////////
 function main() {
     document.body.parentNode.classList.remove("no-js");
     addModeListener();
     setupSearchButtons();
     setupDropdwon();
-    navbarBurger();
+    setupToggleButton();
     header = document.querySelector("header");
     tocScroll = document.querySelector(".toc-scroll");
     setup();
 }
 
 document.addEventListener("DOMContentLoaded", main);
```

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/base/_typography.scss` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/base/_typography.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .back-to-top {
   text-decoration: none;
-  top: calc(var(--navbar-height) + var(--top-content-to-navbar-gap));
+  top: calc(var(--navbar-height) + var(--gap-content-navbar));
 
   display: none;
   position: fixed;
   left: 0;
   // top: 1rem;
   padding: 0.5rem;
   padding-right: 0.75rem;
```

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_search-wrapper.scss` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/components/_search-wrapper.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_api.scss` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/_api.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_code.scss` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/_code.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_images.sass` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/_images.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_lists.scss` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/_lists.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_math.scss` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/_math.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_misc.sass` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/_misc.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_tables.sass` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/_tables.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_target.sass` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/content/_target.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_ablog.scss` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_ablog.scss`

 * *Files 2% similar despite different names*

```diff
@@ -154,7 +154,11 @@
 .ablog__blog_comments,
 .ablog__catalog_header,
 .ablog__catalog_post {
   &.section {
     padding: unset;
   }
 }
+
+article.article-container ul.postlist {
+  padding-left: 0;
+}
```

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_notebooks.scss` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_notebooks.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_sphinx-design.scss` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_sphinx-design.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     .sidenav-drawer {
       display: flex;
       flex-direction: column;
       height: 100%;
 
       nav.menu {
-        padding-left: 15px;
+        padding-left: var(--sidebar-item-spacing-horizontal);
         overflow: auto;
 
         .menu-list a {
           color: var(--bst-color-text-base);
 
           &.is-active {
             background-color: findLightColor(var(--bst-color-link));
```

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 .bulma-tocnav {
   padding: 0 1rem;
   word-break: break-word;
 
   .toc-wrapper {
     position: sticky;
-    top: calc(var(--navbar-height) + var(--top-content-to-navbar-gap));
+    top: calc(var(--navbar-height) + var(--gap-content-navbar));
     overflow-y: auto;
-    max-height: calc(
-      100vh - var(--navbar-height) - var(--top-content-to-navbar-gap)
-    );
+    max-height: calc(100vh - var(--navbar-height) - var(--gap-content-navbar));
   }
 
   ul.table-of-contents {
     font-size: var(--toc-font-size);
 
     li {
       border-left: 1px solid var(--bst-color-border);
```

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_color.scss` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_color.scss`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     ),
   // on_surface: object on top of surface object (without shadows)
   "on-surface":
     (
       "light": rgb(225, 225, 225),
       "dark": rgb(55, 55, 55),
     ),
-  "background-info-panel": (
+  "background-sidenav-panel": (
     "light": linear-gradient(0.25turn, #e3e5f7, #d9e1ef, #e8ebfb),
     "dark": linear-gradient(0.25turn, #5e605a, #51544e, #5a5c58),
   ),
   "canvas": (
     "light": rgb(246, 248, 250),
     "dark": rgb(22, 27, 34),
   ),
```

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/translations/README.md` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/translations/README.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/demo/module.py` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/demo/module.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/demo/sphinxext.py` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/demo/sphinxext.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/pygment.py` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/pygment.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 {%- import "static/webpack-macros.html" as _webpack with context %}
 {%- import "partials/_icon_links_declare.html" as _icon_declare with context %}
 
 <head>
     {%- block site_meta -%}
     <meta charset="utf-8" />
     <meta name="keywords" content="python, sphinx, sphinx-theme, sphinx-doc, documentation" />
-    <meta name="description" content="A sphinx theme based on bulma" />
     <meta name="viewport" content="width=device-width,initial-scale=1" />
     <meta http-equiv="X-UA-Compatible" content="IE=edge" />
     <meta name="msapplication-tap-highlight" content="no" />
 
     {%- if metatags %}{{ metatags }}{% endif -%}
 
     {%- block linktags %}
```

#### html2text {}

```diff
@@ -4,15 +4,14 @@
 webpack-macros.html" as _webpack with context %} {%- import "partials/
 _icon_links_declare.html" as _icon_declare with context %}
 {%- block site_meta -%}
 
 
 
 
-
  {%- if metatags %}{{ metatags }}{% endif -%} {%- block linktags %} {%- if
 hasdoc('about') %}
  {%- endif %} {%- if hasdoc('genindex') %}
  {%- endif %} {%- if hasdoc('search') %}
  {%- endif %} {%- if hasdoc('copyright') %}
  {%- endif %} {%- if next %}
  {%- endif %} {%- if prev %}
```

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html`

 * *Files 10% similar despite different names*

```diff
@@ -29,57 +29,53 @@
     <div class="main-wrapper">
         {% if theme_show_back_to_top %}
         {%- include "components/back-to-top.html" -%}
         {% endif %}
 
         {%- include "search-wrapper.html" -%}
 
+        {% if not hide_sidenav %}
         <div class="bulma-sidenav" id="sidenavMenu">
             <div class="sidenav-viewport">
                 {% block left_sidebar %}
                 {%- include "sections/sidenav.html" -%}
                 {% endblock left_sidebar %}
             </div>
         </div>
+        {% endif %}
 
         <main class="bulma-content">
             {%- include "components/toggle-sidenav.html" -%}
 
             <div class="columns">
-                <article role="main" class="column is-three-quarters article-container">
+                <article role="main"
+                    class="column {% if not hide_tocnav %} is-three-quarters {% endif %} article-container">
                     {% include "sections/article-top.html" %}
                     {% include "components/searchbox.html" %}
 
                     {% block body %}{{ body }}{% endblock body %}
 
                     {% include "sections/article-bottom.html" %}
                     {% if theme_show_prev_next %}
                     {% include "components/prev-next.html" %}
                     {% endif %}
                 </article>
-
-                {% set page_toc = generate_toc_html() %}
-                {%- if page_toc | length >= 1 %}
-                <aside class="column is-one-quarter bulma-tocnav is-hidden-mobile">
-                    <div class="toc-wrapper toc-scroll">
-                        {% if theme_toc_title %}
-                        <div class="toc-title">
-                            {{ theme_toc_title }}
-                        </div>
-                        {% endif %}
-                        {{ page_toc }}
-                    </div>
-                </aside>
-                {% endif %}
+                {% include "sections/tocnav.html" %}
             </div>
 
-            {% block footer %}
-            {% if theme_footer %}
-            {% include "sections/footer.html" %}
+            {% block article_footer %}
+            {% if theme_article_footer %}
+            {% include "sections/article-footer.html" %}
             {% endif %}
-            {% endblock footer %}
+            {% endblock article_footer %}
         </main>
     </div>
 </div>
 {%- endblock mainbody -%}
 
+{% block footer %}
+{% if theme_footer %}
+{% include "sections/footer.html" %}
+{% endif %}
+{% endblock footer %}
+
 {%- endblock htmlbody %}
```

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_css_variables_define.html` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_css_variables_define.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/icons.html` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/icons.html`

 * *Files 13% similar despite different names*

```diff
@@ -12,27 +12,18 @@
         <title>Home</title>
         <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16">
             <path
                 d="M6.906.664a1.749 1.749 0 0 1 2.187 0l5.25 4.2c.415.332.657.835.657 1.367v7.019A1.75 1.75 0 0 1 13.25 15h-3.5a.75.75 0 0 1-.75-.75V9H7v5.25a.75.75 0 0 1-.75.75h-3.5A1.75 1.75 0 0 1 1 13.25V6.23c0-.531.242-1.034.657-1.366l5.25-4.2Zm1.25 1.171a.25.25 0 0 0-.312 0l-5.25 4.2a.25.25 0 0 0-.094.196v7.019c0 .138.112.25.25.25H5.5V8.25a.75.75 0 0 1 .75-.75h3.5a.75.75 0 0 1 .75.75v5.25h2.75a.25.25 0 0 0 .25-.25V6.23a.25.25 0 0 0-.094-.195Z">
             </path>
         </svg>
     </symbol>
-    <symbol id="svg-github" viewBox="0 0 24 24">
-        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" fill="none"
-            stroke-linecap="round" stroke-linejoin="round">
-            <path stroke="none" d="M0 0h24v24H0z" fill="none" />
-            <path d="M4 18v-5.5c0 -.667 .167 -1.333 .5 -2" />
-            <path d="M12 7.5c0 -1 -.01 -4.07 -4 -3.5c-3.5 .5 -4 2.5 -4 3.5c0 1.5 0 4 3 4c4 0 5 -2.5 5 -4z" />
+    <symbol id="svg-github" viewBox="0 0 480 512">
+        <svg viewBox="0 0 480 512" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
             <path
-                d="M4 12c-1.333 .667 -2 1.333 -2 2c0 1 0 3 1.5 4c3 2 6.5 3 8.5 3s5.499 -1 8.5 -3c1.5 -1 1.5 -3 1.5 -4c0 -.667 -.667 -1.333 -2 -2" />
-            <path d="M20 18v-5.5c0 -.667 -.167 -1.333 -.5 -2" />
-            <path
-                d="M12 7.5l0 -.297l.01 -.269l.027 -.298l.013 -.105l.033 -.215c.014 -.073 .029 -.146 .046 -.22l.06 -.223c.336 -1.118 1.262 -2.237 3.808 -1.873c2.838 .405 3.703 1.797 3.93 2.842l.036 .204c0 .033 .01 .066 .013 .098l.016 .185l0 .171l0 .49l-.015 .394l-.02 .271c-.122 1.366 -.655 2.845 -2.962 2.845c-3.256 0 -4.524 -1.656 -4.883 -3.081l-.053 -.242a3.865 3.865 0 0 1 -.036 -.235l-.021 -.227a3.518 3.518 0 0 1 -.007 -.215z" />
-            <path d="M10 15v2" />
-            <path d="M14 15v2" />
+                d="M186.1 328.7c0 20.9-10.9 55.1-36.7 55.1s-36.7-34.2-36.7-55.1 10.9-55.1 36.7-55.1 36.7 34.2 36.7 55.1zM480 278.2c0 31.9-3.2 65.7-17.5 95-37.9 76.6-142.1 74.8-216.7 74.8-75.8 0-186.2 2.7-225.6-74.8-14.6-29-20.2-63.1-20.2-95 0-41.9 13.9-81.5 41.5-113.6-5.2-15.8-7.7-32.4-7.7-48.8 0-21.5 4.9-32.3 14.6-51.8 45.3 0 74.3 9 108.8 36 29-6.9 58.8-10 88.7-10 27 0 54.2 2.9 80.4 9.2 34-26.7 63-35.2 107.8-35.2 9.8 19.5 14.6 30.3 14.6 51.8 0 16.4-2.6 32.7-7.7 48.2 27.5 32.4 39 72.3 39 114.2zm-64.3 50.5c0-43.9-26.7-82.6-73.5-82.6-18.9 0-37 3.4-56 6-14.9 2.3-29.8 3.2-45.1 3.2-15.2 0-30.1-.9-45.1-3.2-18.7-2.6-37-6-56-6-46.8 0-73.5 38.7-73.5 82.6 0 87.8 80.4 101.3 150.4 101.3h48.2c70.3 0 150.6-13.4 150.6-101.3zm-82.6-55.1c-25.8 0-36.7 34.2-36.7 55.1s10.9 55.1 36.7 55.1 36.7-34.2 36.7-55.1-10.9-55.1-36.7-55.1z" />
         </svg>
     </symbol>
     <symbol id="svg-pencil" viewBox="0 0 16 16">
         <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16">
             <path
                 d="M11.013 1.427a1.75 1.75 0 0 1 2.474 0l1.086 1.086a1.75 1.75 0 0 1 0 2.474l-8.61 8.61c-.21.21-.47.364-.756.445l-3.251.93a.75.75 0 0 1-.927-.928l.929-3.25c.081-.286.235-.547.445-.758l8.61-8.61Zm.176 4.823L9.75 4.81l-6.286 6.287a.253.253 0 0 0-.064.108l-.558 1.953 1.953-.558a.253.253 0 0 0 .108-.064Zm1.238-3.763a.25.25 0 0 0-.354 0L10.811 3.75l1.439 1.44 1.263-1.263a.25.25 0 0 0 0-.354Z">
             </path>
```

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 {%- set icon_class = "navbar-item" -%}
 
 <div class="navbar-brand">
-    {% include "components/brand-logo.html" %}
+    {% include "components/brand.html" %}
 
     <a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false" data-target="navbarMenu">
         <span aria-hidden="true"></span>
         <span aria-hidden="true"></span>
         <span aria-hidden="true"></span>
     </a>
 </div>
 
 <div class="navbar-menu" id="navbarMenu">
     <div class="navbar-start">
         {% if theme_navbar_start %}
         {%- for ns_section in theme_navbar_start %}
-        {% if ns_section in theme_navbar_include_directly %}
-        {%- include ns_section %}
-        {% else %}
+        {% if ns_section in theme_navbar_wrapped_items %}
         <div class="navbar-item">
             {%- include ns_section %}
         </div>
+        {% else %}
+        {%- include ns_section %}
         {% endif %}
         {%- endfor %}
         {% endif %}
     </div>
 
     <div class="navbar-end">
         {% if theme_navbar_end %}
         {%- for ne_section in theme_navbar_end %}
-        {% if ne_section in theme_navbar_include_directly %}
-        {%- include ne_section %}
-        {% else %}
+        {% if ne_section in theme_navbar_wrapped_items %}
         <div class="navbar-item">
             {%- include ne_section %}
         </div>
+        {% else %}
+        {%- include ne_section %}
         {% endif %}
         {%- endfor %}
         {% endif %}
     </div>
 </div>
```

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [theme]
 inherit = basic-ng
 stylesheet = styles/bulma-sphinx-theme.css
 pygments_style = tango
 # sidebar-start
-sidebars = sidenav-nav.html
+sidebars = sidenav-panel.html, sidenav-nav.html
 # sidebar-end
 
 [options]
 have_top_navbar = True
 navigation_depth = 4
 show_nav_level = 1
 show_toc_level = 1
@@ -20,31 +20,33 @@
 pygment_light_style = manni
 pygment_dark_style = material
 
 # see https://bulma.io/documentation/components/navbar/#colors for more navbar color styles
 navbar_color_style = is-white
 navbar_start = navbar-nav.html
 navbar_end = theme-swither.html, icon-links.html
-navbar_include_directly =
+navbar_wrapped_items =
+article_top_left = breadcrumbs.html
+article_top_right =
+article_bottom_left = last-updated.html
+article_bottom_right = sourcelink.html, edit-this-page.html
+article_footer = copyright.html, sphinx-version.html
+footer =
 analytics =
-footer = copyright.html, sphinx-version.html
 toc_title = On this page
 dropdown_label_name = More
 dropdown_label_target_url =
 navigation_with_keys = True
 search_bar_text = Search the docs ...
 show_back_to_top = True
-article_top_left = breadcrumbs.html
-article_top_right =
-article_bottom_left = last-updated.html
-article_bottom_right = sourcelink.html, edit-this-page.html
 use_edit_page_button =
 source_repository =
 source_branch =
 source_directory =
 source_edit_link =
 show_prev_next = True
-information_panel =
+sidenav_panel =
+sidenav_panel_wrapped_items =
 # define css variables
 light_colors =
 dark_colors =
 css_variables =
```

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/toctree.py` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/toctree.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/transforms.py` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/transforms.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/translations.py` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/translations.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/utils.py` & `bulma_sphinx_theme-0.2.0rc1/src/bulma_sphinx_theme/utils.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/webpack.config.js` & `bulma_sphinx_theme-0.2.0rc1/webpack.config.js`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.1.0rc1/PKG-INFO` & `bulma_sphinx_theme-0.2.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulma-sphinx-theme
-Version: 0.1.0rc1
+Version: 0.2.0rc1
 Summary: A sphinx theme based on bulma.
 Author-Email: zclab <syfhub@hotmail.com>
 License: MIT License
         
         Copyright (c) 2023 zc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -20,15 +20,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bulma-sphinx-theme Version: 0.1.0rc1 Summary: A
+Metadata-Version: 2.1 Name: bulma-sphinx-theme Version: 0.2.0rc1 Summary: A
 sphinx theme based on bulma. Author-Email: zclab
 hotmail.com> License: MIT License Copyright (c) 2023 zc Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -10,15 +10,15 @@
 permission notice shall be included in all copies or substantial portions of
 the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE. Classifier: Development Status :: 2 - Pre-Alpha
+DEALINGS IN THE SOFTWARE. Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Sphinx Classifier: Framework :: Sphinx :: Theme
 Classifier: License :: OSI Approved :: MIT License Classifier: Environment ::
 Web Environment Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Operating System :: OS Independent Classifier: Topic
```

