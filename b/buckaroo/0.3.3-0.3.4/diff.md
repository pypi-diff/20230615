# Comparing `tmp/buckaroo-0.3.3.tar.gz` & `tmp/buckaroo-0.3.4.tar.gz`

## Comparing `buckaroo-0.3.3.tar` & `buckaroo-0.3.4.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 buckaroo-0.3.3/.coveragerc
--rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 buckaroo-0.3.3/RELEASE.md
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 buckaroo-0.3.3/Untitled.ipynb
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 buckaroo-0.3.3/babel.config.js
--rw-r--r--   0        0        0    24393 2020-02-02 00:00:00.000000 buckaroo-0.3.3/bike-share-data-explore.ipynb
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo.json
--rw-r--r--   0        0        0    24936 2020-02-02 00:00:00.000000 buckaroo-0.3.3/col-ordering.ipynb
--rwxr-xr-x   0        0        0      237 2020-02-02 00:00:00.000000 buckaroo-0.3.3/full_build.sh
--rw-r--r--   0        0        0   129498 2020-02-02 00:00:00.000000 buckaroo-0.3.3/gbfs-play.ipynb
--rw-r--r--   0        0        0    97653 2020-02-02 00:00:00.000000 buckaroo-0.3.3/gbfs-play2.ipynb
--rw-r--r--   0        0        0     7542 2020-02-02 00:00:00.000000 buckaroo-0.3.3/introduction.ipynb
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 buckaroo-0.3.3/notes.txt
--rw-r--r--   0        0        0   693792 2020-02-02 00:00:00.000000 buckaroo-0.3.3/package-lock.json
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 buckaroo-0.3.3/package.json
--rw-r--r--   0        0        0     6380 2020-02-02 00:00:00.000000 buckaroo-0.3.3/package.json.old
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 buckaroo-0.3.3/setup.py
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 buckaroo-0.3.3/tryit.ipynb
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 buckaroo-0.3.3/tsconfig.json
--rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 buckaroo-0.3.3/webpack.config.js
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 buckaroo-0.3.3/webpack.lab.config.js
--rw-r--r--   0        0        0   365701 2020-02-02 00:00:00.000000 buckaroo-0.3.3/yarn.lock
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 buckaroo-0.3.3/.yarn/cache/.gitignore
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/_frontend.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/_version.py
--rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/all_transforms.py
--rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/buckaroo_widget.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/channeldata.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/configure_utils.py
--rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/dcf_transform.py
--rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/df_methods.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/index.html
--rw-r--r--   0        0        0    17284 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/lispy.py
--rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/summary_stats.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/views.py
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/package.json
--rw-r--r--   0        0        0   145367 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js.LICENSE.txt
--rw-r--r--   0        0        0    35455 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/399.252405500e4886745cf0.js
--rw-r--r--   0        0        0   231664 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/41.dea207301743f71053c5.js
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/480.c541de2b54a15c8f7330.js
--rw-r--r--   0        0        0    70484 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js.LICENSE.txt
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/568.50d29d049ddb62602cc0.js
--rw-r--r--   0        0        0  1067038 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/731.d4bf968c7a94633ef5a3.js
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/731.d4bf968c7a94633ef5a3.js.LICENSE.txt
--rw-r--r--   0        0        0   139612 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js.LICENSE.txt
--rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/remoteEntry.25db2035d9cfb129895d.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/style.js
--rw-r--r--   0        0        0    11965 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0  1691110 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/nbextension/index.js
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/nbextension/index.js.LICENSE.txt
--rw-r--r--   0        0        0  5896429 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/nbextension/index.js.map
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/noarch/current_repodata.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/noarch/current_repodata.json.bz2
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/noarch/index.html
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/noarch/repodata.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/noarch/repodata.json.bz2
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/noarch/repodata_from_packages.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/noarch/repodata_from_packages.json.bz2
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 buckaroo-0.3.3/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 buckaroo-0.3.3/docs/make.bat
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 buckaroo-0.3.3/docs/source/.#nodejs-download.html -> paddy@Paddys-MacBook-Air.local.405
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 buckaroo-0.3.3/docs/source/.#vs-code-download.html -> paddy@Paddys-MacBook-Air.local.405
--rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 buckaroo-0.3.3/docs/source/FAQ.rst
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 buckaroo-0.3.3/docs/source/conf.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 buckaroo-0.3.3/docs/source/contributing.rst
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 buckaroo-0.3.3/docs/source/index.rst
--rwxr-xr-x   0        0        0      295 2020-02-02 00:00:00.000000 buckaroo-0.3.3/docs/source/install.rst
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 buckaroo-0.3.3/docs/source/using.rst
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 buckaroo-0.3.3/docs/source/_static/embed-bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     7144 2020-02-02 00:00:00.000000 buckaroo-0.3.3/example-notebooks/testcases-fast.ipynb
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/comp1.tsx
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/dcefwidget.ts
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/extension.ts
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/index.ts
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/plugin.ts
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/version.ts
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/components/ColumnsEditor.tsx
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/components/CommandUtils.ts
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/components/DCFCell.tsx
--rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/components/DFViewer.tsx
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/components/DependentTabs.tsx
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/components/OperationDetail.tsx
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/components/OperationUtils.ts
--rw-r--r--   0        0        0     6989 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/components/Operations.tsx
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/components/StatusBar.tsx
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/components/bakedOperationDefaults.ts
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/components/gridUtils.ts
--rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/components/staticData.ts
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/components/utils.ts
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/style/dcf-npm.css
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/style/icons/arrow-down-short-dark.svg
--rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/style/icons/arrow-down-short.svg
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/style/icons/arrow-up-short-dark.svg
--rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/style/icons/arrow-up-short.svg
--rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/style/icons/filter-dark.svg
--rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/style/icons/filter.svg
--rw-r--r--   0        0        0  1420117 2020-02-02 00:00:00.000000 buckaroo-0.3.3/static/images/Buckaroo-screenshot.png
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 buckaroo-0.3.3/.gitignore
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 buckaroo-0.3.3/LICENSE.txt
--rw-r--r--   0        0        0    10241 2020-02-02 00:00:00.000000 buckaroo-0.3.3/README.md
--rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 buckaroo-0.3.3/pyproject.toml
--rw-r--r--   0        0        0    13091 2020-02-02 00:00:00.000000 buckaroo-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 buckaroo-0.3.4/.coveragerc
+-rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 buckaroo-0.3.4/RELEASE.md
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 buckaroo-0.3.4/Untitled.ipynb
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 buckaroo-0.3.4/babel.config.js
+-rw-r--r--   0        0        0    24393 2020-02-02 00:00:00.000000 buckaroo-0.3.4/bike-share-data-explore.ipynb
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo.json
+-rw-r--r--   0        0        0    24936 2020-02-02 00:00:00.000000 buckaroo-0.3.4/col-ordering.ipynb
+-rwxr-xr-x   0        0        0      237 2020-02-02 00:00:00.000000 buckaroo-0.3.4/full_build.sh
+-rw-r--r--   0        0        0   129498 2020-02-02 00:00:00.000000 buckaroo-0.3.4/gbfs-play.ipynb
+-rw-r--r--   0        0        0    97653 2020-02-02 00:00:00.000000 buckaroo-0.3.4/gbfs-play2.ipynb
+-rw-r--r--   0        0        0     7542 2020-02-02 00:00:00.000000 buckaroo-0.3.4/introduction.ipynb
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 buckaroo-0.3.4/notes.txt
+-rw-r--r--   0        0        0   693792 2020-02-02 00:00:00.000000 buckaroo-0.3.4/package-lock.json
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 buckaroo-0.3.4/package.json
+-rw-r--r--   0        0        0     6380 2020-02-02 00:00:00.000000 buckaroo-0.3.4/package.json.old
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 buckaroo-0.3.4/setup.py
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 buckaroo-0.3.4/tryit.ipynb
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 buckaroo-0.3.4/tsconfig.json
+-rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 buckaroo-0.3.4/webpack.config.js
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 buckaroo-0.3.4/webpack.lab.config.js
+-rw-r--r--   0        0        0   365701 2020-02-02 00:00:00.000000 buckaroo-0.3.4/yarn.lock
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 buckaroo-0.3.4/.yarn/cache/.gitignore
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/_frontend.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/_version.py
+-rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/all_transforms.py
+-rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/buckaroo_widget.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/channeldata.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/configure_utils.py
+-rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/dcf_transform.py
+-rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/df_methods.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/index.html
+-rw-r--r--   0        0        0    17284 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/lispy.py
+-rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/summary_stats.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/views.py
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/labextension/package.json
+-rw-r--r--   0        0        0   145367 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js.LICENSE.txt
+-rw-r--r--   0        0        0    35955 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/labextension/static/399.50690b06cf528166a430.js
+-rw-r--r--   0        0        0   231664 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/labextension/static/41.dea207301743f71053c5.js
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/labextension/static/480.c541de2b54a15c8f7330.js
+-rw-r--r--   0        0        0    70484 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js.LICENSE.txt
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/labextension/static/568.50d29d049ddb62602cc0.js
+-rw-r--r--   0        0        0  1067038 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/labextension/static/731.d4bf968c7a94633ef5a3.js
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/labextension/static/731.d4bf968c7a94633ef5a3.js.LICENSE.txt
+-rw-r--r--   0        0        0   139612 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js.LICENSE.txt
+-rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/labextension/static/remoteEntry.e0e4ad417ed29f6a520a.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/labextension/static/style.js
+-rw-r--r--   0        0        0    11965 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0  1691110 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/nbextension/index.js
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/nbextension/index.js.LICENSE.txt
+-rw-r--r--   0        0        0  5896429 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/nbextension/index.js.map
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/noarch/current_repodata.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/noarch/current_repodata.json.bz2
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/noarch/index.html
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/noarch/repodata.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/noarch/repodata.json.bz2
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/noarch/repodata_from_packages.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.3.4/buckaroo/noarch/repodata_from_packages.json.bz2
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 buckaroo-0.3.4/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 buckaroo-0.3.4/docs/make.bat
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 buckaroo-0.3.4/docs/source/.#nodejs-download.html -> paddy@Paddys-MacBook-Air.local.405
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 buckaroo-0.3.4/docs/source/.#vs-code-download.html -> paddy@Paddys-MacBook-Air.local.405
+-rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 buckaroo-0.3.4/docs/source/FAQ.rst
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 buckaroo-0.3.4/docs/source/conf.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 buckaroo-0.3.4/docs/source/contributing.rst
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 buckaroo-0.3.4/docs/source/index.rst
+-rwxr-xr-x   0        0        0      295 2020-02-02 00:00:00.000000 buckaroo-0.3.4/docs/source/install.rst
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 buckaroo-0.3.4/docs/source/using.rst
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 buckaroo-0.3.4/docs/source/_static/embed-bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     7144 2020-02-02 00:00:00.000000 buckaroo-0.3.4/example-notebooks/testcases-fast.ipynb
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 buckaroo-0.3.4/js/comp1.tsx
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 buckaroo-0.3.4/js/dcefwidget.ts
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 buckaroo-0.3.4/js/extension.ts
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 buckaroo-0.3.4/js/index.ts
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 buckaroo-0.3.4/js/plugin.ts
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 buckaroo-0.3.4/js/version.ts
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 buckaroo-0.3.4/js/components/ColumnsEditor.tsx
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 buckaroo-0.3.4/js/components/CommandUtils.ts
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 buckaroo-0.3.4/js/components/DCFCell.tsx
+-rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 buckaroo-0.3.4/js/components/DFViewer.tsx
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 buckaroo-0.3.4/js/components/DependentTabs.tsx
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 buckaroo-0.3.4/js/components/OperationDetail.tsx
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 buckaroo-0.3.4/js/components/OperationUtils.ts
+-rw-r--r--   0        0        0     6989 2020-02-02 00:00:00.000000 buckaroo-0.3.4/js/components/Operations.tsx
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 buckaroo-0.3.4/js/components/StatusBar.tsx
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 buckaroo-0.3.4/js/components/bakedOperationDefaults.ts
+-rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 buckaroo-0.3.4/js/components/gridUtils.ts
+-rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 buckaroo-0.3.4/js/components/staticData.ts
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 buckaroo-0.3.4/js/components/utils.ts
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 buckaroo-0.3.4/js/style/dcf-npm.css
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.3.4/js/style/icons/arrow-down-short-dark.svg
+-rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.3.4/js/style/icons/arrow-down-short.svg
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.3.4/js/style/icons/arrow-up-short-dark.svg
+-rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.3.4/js/style/icons/arrow-up-short.svg
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.3.4/js/style/icons/filter-dark.svg
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.3.4/js/style/icons/filter.svg
+-rw-r--r--   0        0        0  1420117 2020-02-02 00:00:00.000000 buckaroo-0.3.4/static/images/Buckaroo-screenshot.png
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 buckaroo-0.3.4/.gitignore
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 buckaroo-0.3.4/LICENSE.txt
+-rw-r--r--   0        0        0    10241 2020-02-02 00:00:00.000000 buckaroo-0.3.4/README.md
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 buckaroo-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0    13091 2020-02-02 00:00:00.000000 buckaroo-0.3.4/PKG-INFO
```

### Comparing `buckaroo-0.3.3/RELEASE.md` & `buckaroo-0.3.4/RELEASE.md`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/bike-share-data-explore.ipynb` & `buckaroo-0.3.4/bike-share-data-explore.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/col-ordering.ipynb` & `buckaroo-0.3.4/col-ordering.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/gbfs-play.ipynb` & `buckaroo-0.3.4/gbfs-play.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/gbfs-play2.ipynb` & `buckaroo-0.3.4/gbfs-play2.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/introduction.ipynb` & `buckaroo-0.3.4/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/package-lock.json` & `buckaroo-0.3.4/package-lock.json`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/package.json` & `buckaroo-0.3.4/package.json`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/package.json.old` & `buckaroo-0.3.4/package.json.old`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/tryit.ipynb` & `buckaroo-0.3.4/tryit.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/tsconfig.json` & `buckaroo-0.3.4/tsconfig.json`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/webpack.config.js` & `buckaroo-0.3.4/webpack.config.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/yarn.lock` & `buckaroo-0.3.4/yarn.lock`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/buckaroo/__init__.py` & `buckaroo-0.3.4/buckaroo/__init__.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/buckaroo/all_transforms.py` & `buckaroo-0.3.4/buckaroo/all_transforms.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/buckaroo/buckaroo_widget.py` & `buckaroo-0.3.4/buckaroo/buckaroo_widget.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/buckaroo/configure_utils.py` & `buckaroo-0.3.4/buckaroo/configure_utils.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/buckaroo/dcf_transform.py` & `buckaroo-0.3.4/buckaroo/dcf_transform.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/buckaroo/df_methods.py` & `buckaroo-0.3.4/buckaroo/df_methods.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/buckaroo/index.html` & `buckaroo-0.3.4/buckaroo/index.html`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/buckaroo/lispy.py` & `buckaroo-0.3.4/buckaroo/lispy.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/buckaroo/summary_stats.py` & `buckaroo-0.3.4/buckaroo/summary_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,17 @@
 def table_sumarize_ser(ser):
     if pd.api.types.is_numeric_dtype(ser.dtype):
         return table_sumarize_num_ser(ser.dropna())
     else:
         return table_sumarize_obj_ser(ser)
     
 def table_sumarize(df):
-    return {col:table_sumarize_ser(df[col]) for col in df}
+    table_hints = {col:table_sumarize_ser(df[col]) for col in df}
+    table_hints['index'] = table_sumarize_ser(df.index)
+    return table_hints
 
 
 def summarize_string(ser):
     l = len(ser)
     val_counts = ser.value_counts()
     distinct_count= len(val_counts)
     nan_count = l - len(ser.dropna())
```

### Comparing `buckaroo-0.3.3/buckaroo/views.py` & `buckaroo-0.3.4/buckaroo/views.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/buckaroo/labextension/package.json` & `buckaroo-0.3.4/buckaroo/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99921875%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.e0e4ad417ed29f6a520a.js'}}"}*

```diff
@@ -81,15 +81,15 @@
         "dist/*.png",
         "style/**/*.*"
     ],
     "homepage": "https://github.com/paddymul/buckaroo",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.25db2035d9cfb129895d.js"
+            "load": "static/remoteEntry.e0e4ad417ed29f6a520a.js"
         },
         "extension": "lib/plugin",
         "outputDir": "./buckaroo/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
```

### Comparing `buckaroo-0.3.3/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js` & `buckaroo-0.3.4/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js.LICENSE.txt` & `buckaroo-0.3.4/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/buckaroo/labextension/static/399.252405500e4886745cf0.js` & `buckaroo-0.3.4/buckaroo/labextension/static/399.50690b06cf528166a430.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -149,29 +149,31 @@
                 dfConfig: o,
                 on_dfConfig: i,
                 summaryDf: d
             }) {
                 const [m, f] = (0, l.useState)("stoptime"), p = {
                     showCommands: o.showCommands,
                     showTransformed: o.showTransformed
-                };
+                }, b = Object.assign(Object.assign({}, o), {
+                    rowsShown: e.data.length || 0
+                });
                 return l.default.createElement("div", {
                     className: "dcf-root flex flex-col",
                     style: {
                         width: "100%",
                         height: "100%"
                     }
                 }, l.default.createElement("div", {
                     className: "orig-df flex flex-row",
                     style: {
                         height: "450px",
                         overflow: "hidden"
                     }
                 }, l.default.createElement(c.StatusBar, {
-                    config: o,
+                    config: b,
                     setConfig: i
                 }), l.default.createElement(u.DFViewer, {
                     df: o.summaryStats ? d : e,
                     activeCol: m,
                     setActiveCol: f
                 })), p.showCommands || p.showTransformed ? l.default.createElement(s.ColumnsEditor, {
                     df: e,
@@ -837,15 +839,16 @@
                     return r(t, e), t
                 };
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.StatusBarEx = t.StatusBar = void 0;
             const l = o(n(7294)),
                 i = n(1048),
-                s = [{
+                s = n(214),
+                d = [{
                     field: "summaryStats",
                     headerName: "Σ",
                     headerTooltip: "Summary Stats",
                     width: 30
                 }, {
                     field: "reorderdColumns",
                     headerName: "Θ",
@@ -876,48 +879,48 @@
                     field: "rowsShown",
                     width: 120
                 }, {
                     field: "sampleSize",
                     width: 120
                 }];
 
-            function d({
+            function u({
                 config: e,
                 setConfig: t
             }) {
                 const {
                     totalRows: n,
                     columns: a,
                     rowsShown: r,
                     sampleSize: o,
-                    sampled: d,
-                    summaryStats: u,
-                    reorderdColumns: c,
-                    showTransformed: m,
-                    showCommands: f
-                } = e, p = [{
-                    totalRows: n,
+                    sampled: u,
+                    summaryStats: c,
+                    reorderdColumns: m,
+                    showTransformed: f,
+                    showCommands: p
+                } = e, b = [{
+                    totalRows: s.intFormatter.format(n),
                     columns: a,
-                    rowsShown: r,
-                    sampleSize: o,
-                    sampled: d ? "Ϋ" : "ό",
-                    summaryStats: u ? "Ϋ" : "ό",
-                    reorderdColumns: c ? "Ϋ" : "ό",
-                    showTransformed: m ? "Ϋ" : "ό",
-                    showCommands: f ? "Ϋ" : "ό"
-                }], b = (0, l.useRef)(null);
+                    rowsShown: s.intFormatter.format(r),
+                    sampleSize: s.intFormatter.format(o),
+                    sampled: u ? "Ϋ" : "ό",
+                    summaryStats: c ? "Ϋ" : "ό",
+                    reorderdColumns: m ? "Ϋ" : "ό",
+                    showTransformed: f ? "Ϋ" : "ό",
+                    showCommands: p ? "Ϋ" : "ό"
+                }], g = (0, l.useRef)(null);
                 return l.default.createElement("div", {
                     className: "statusBar"
                 }, l.default.createElement("div", {
                     style: {
                         height: 50
                     },
                     className: "theme-hanger ag-theme-alpine-dark"
                 }, l.default.createElement(i.AgGridReact, {
-                    ref: b,
+                    ref: g,
                     onCellClicked: n => {
                         const a = n.column.getColId();
                         "summaryStats" === a ? t(Object.assign(Object.assign({}, e), {
                             summaryStats: !e.summaryStats
                         })) : "sampled" === a ? t(Object.assign(Object.assign({}, e), {
                             sampled: !e.sampled
                         })) : "reorderdColumns" === a ? t(Object.assign(Object.assign({}, e), {
@@ -933,31 +936,31 @@
                     },
                     defaultColDef: {
                         type: "left-aligned",
                         cellStyle: {
                             textAlign: "left"
                         }
                     },
-                    rowData: p,
-                    columnDefs: s
+                    rowData: b,
+                    columnDefs: d
                 })))
             }
-            t.StatusBar = d, t.StatusBarEx = function() {
+            t.StatusBar = u, t.StatusBarEx = function() {
                 const [e, t] = (0, l.useState)({
                     totalRows: 1309,
                     columns: 30,
                     rowsShown: 500,
                     sampleSize: 1e4,
                     sampled: !0,
                     summaryStats: !1,
                     reorderdColumns: !0,
                     showTransformed: !0,
                     showCommands: !0
                 });
-                return l.default.createElement(d, {
+                return l.default.createElement(u, {
                     config: e,
                     setConfig: t
                 })
             }
         },
         4619: (e, t, n) => {
             Object.defineProperty(t, "__esModule", {
@@ -978,35 +981,49 @@
             var a = this && this.__importDefault || function(e) {
                 return e && e.__esModule ? e : {
                     default: e
                 }
             };
             Object.defineProperty(t, "__esModule", {
                 value: !0
-            }), t.dfToAgrid = t.updateAtMatch = void 0;
+            }), t.dfToAgrid = t.anyFormatter = t.intFormatter = t.updateAtMatch = void 0;
             const r = a(n(4439));
+            t.updateAtMatch = (e, t, n, a) => e.map((e => e.field === t ? Object.assign(Object.assign({}, e), n) : Object.assign(Object.assign({}, e), a))), t.intFormatter = new Intl.NumberFormat("en-US", {
+                minimumFractionDigits: 0,
+                maximumFractionDigits: 3
+            });
+            const o = new Intl.NumberFormat("en-US", {
+                minimumFractionDigits: 3,
+                maximumFractionDigits: 3
+            });
 
-            function o(e) {
-                if (void 0 === e || !1 === e.is_numeric) return e => e.value; {
+            function l(e) {
+                if (void 0 === e || !1 === e.is_numeric) return t.anyFormatter; {
                     const t = Math.floor(e.max_digits / 3);
                     if (e.is_integer) {
                         const n = t + e.max_digits;
                         return e => (console.log("params", e), new Intl.NumberFormat("en-US").format(e.value).padStart(n, " "))
                     }
-                    return e => new Intl.NumberFormat("en-US", {
-                        minimumFractionDigits: 3,
-                        maximumFractionDigits: 3
-                    }).format(e.value)
+                    return e => o.format(e.value)
                 }
             }
-            t.updateAtMatch = (e, t, n, a) => e.map((e => e.field === t ? Object.assign(Object.assign({}, e), n) : Object.assign(Object.assign({}, e), a))), t.dfToAgrid = function(e) {
+            t.anyFormatter = e => {
+                const n = e.value;
+                try {
+                    const e = Number(n);
+                    if (null === n) return "";
+                    if (void 0 === n) return "";
+                    if (Number.isFinite(e)) return Number.isInteger(e) ? `${t.intFormatter.format(e)}    ` : o.format(e)
+                } catch (e) {}
+                return n
+            }, t.dfToAgrid = function(e) {
                 return [e.schema.fields.map((t => {
                     const n = {
                         field: t.name,
-                        valueFormatter: o(r.default.get(e.table_hints, t.name, {
+                        valueFormatter: l(r.default.get(e.table_hints, t.name, {
                             is_numeric: !1
                         }))
                     };
                     return "index" === t.name && (n.pinned = "left"), n
                 })), e.data]
             }
         },
```

### Comparing `buckaroo-0.3.3/buckaroo/labextension/static/41.dea207301743f71053c5.js` & `buckaroo-0.3.4/buckaroo/labextension/static/41.dea207301743f71053c5.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/buckaroo/labextension/static/480.c541de2b54a15c8f7330.js` & `buckaroo-0.3.4/buckaroo/labextension/static/480.c541de2b54a15c8f7330.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js` & `buckaroo-0.3.4/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/buckaroo/labextension/static/568.50d29d049ddb62602cc0.js` & `buckaroo-0.3.4/buckaroo/labextension/static/568.50d29d049ddb62602cc0.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/buckaroo/labextension/static/731.d4bf968c7a94633ef5a3.js` & `buckaroo-0.3.4/buckaroo/labextension/static/731.d4bf968c7a94633ef5a3.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js` & `buckaroo-0.3.4/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js.LICENSE.txt` & `buckaroo-0.3.4/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/buckaroo/labextension/static/remoteEntry.25db2035d9cfb129895d.js` & `buckaroo-0.3.4/buckaroo/labextension/static/remoteEntry.e0e4ad417ed29f6a520a.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -45,25 +45,25 @@
         for (var t in r) P.o(r, t) && !P.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, P.f = {}, P.e = e => Promise.all(Object.keys(P.f).reduce(((r, t) => (P.f[t](e, r), r)), [])), P.u = e => e + "." + {
         0: "c008020c7e2133e6c7db",
         41: "dea207301743f71053c5",
-        399: "252405500e4886745cf0",
+        399: "50690b06cf528166a430",
         480: "c541de2b54a15c8f7330",
         486: "f08778dfb765d893ceaf",
         497: "a76de7c665cc86a1c49a",
         568: "50d29d049ddb62602cc0",
         731: "d4bf968c7a94633ef5a3",
         935: "2832d17fef97c1ec6694"
     } [e] + ".js?v=" + {
         0: "c008020c7e2133e6c7db",
         41: "dea207301743f71053c5",
-        399: "252405500e4886745cf0",
+        399: "50690b06cf528166a430",
         480: "c541de2b54a15c8f7330",
         486: "f08778dfb765d893ceaf",
         497: "a76de7c665cc86a1c49a",
         568: "50d29d049ddb62602cc0",
         731: "d4bf968c7a94633ef5a3",
         935: "2832d17fef97c1ec6694"
     } [e], P.g = function() {
```

### Comparing `buckaroo-0.3.3/buckaroo/labextension/static/third-party-licenses.json` & `buckaroo-0.3.4/buckaroo/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/buckaroo/nbextension/index.js` & `buckaroo-0.3.4/buckaroo/nbextension/index.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/buckaroo/nbextension/index.js.LICENSE.txt` & `buckaroo-0.3.4/buckaroo/nbextension/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/buckaroo/nbextension/index.js.map` & `buckaroo-0.3.4/buckaroo/nbextension/index.js.map`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/buckaroo/noarch/index.html` & `buckaroo-0.3.4/buckaroo/noarch/index.html`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/docs/Makefile` & `buckaroo-0.3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/docs/make.bat` & `buckaroo-0.3.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/docs/source/FAQ.rst` & `buckaroo-0.3.4/docs/source/FAQ.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/docs/source/conf.py` & `buckaroo-0.3.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/docs/source/contributing.rst` & `buckaroo-0.3.4/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/docs/source/index.rst` & `buckaroo-0.3.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/docs/source/using.rst` & `buckaroo-0.3.4/docs/source/using.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/docs/source/_static/embed-bundle.js.LICENSE.txt` & `buckaroo-0.3.4/docs/source/_static/embed-bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/example-notebooks/testcases-fast.ipynb` & `buckaroo-0.3.4/example-notebooks/testcases-fast.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/js/dcefwidget.ts` & `buckaroo-0.3.4/js/dcefwidget.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/js/extension.ts` & `buckaroo-0.3.4/js/extension.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/js/plugin.ts` & `buckaroo-0.3.4/js/plugin.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/js/components/ColumnsEditor.tsx` & `buckaroo-0.3.4/js/components/ColumnsEditor.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/js/components/CommandUtils.ts` & `buckaroo-0.3.4/js/components/CommandUtils.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/js/components/DCFCell.tsx` & `buckaroo-0.3.4/js/components/DCFCell.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -34,24 +34,25 @@
   commandConfig: CommandConfigT;
   dfConfig: DfConfig;
   on_dfConfig: unknown;
   summaryDf: DFWhole
 }) {
   const [activeCol, setActiveCol] = useState('stoptime');
   const widgetConfig: WidgetConfig = {showCommands:dfConfig.showCommands, showTransformed:dfConfig.showTransformed}
+  const localDfConfig = {...dfConfig, 'rowsShown': origDf.data.length || 0}
   return (
     <div
       className="dcf-root flex flex-col"
       style={{ width: '100%', height: '100%' }}
     >
       <div
         className="orig-df flex flex-row"
         style={{ height: '450px', overflow: 'hidden' }}
       >
-        <StatusBar config={dfConfig} setConfig={on_dfConfig} />
+        <StatusBar config={localDfConfig} setConfig={on_dfConfig} />
         <DFViewer
           df={(dfConfig.summaryStats ? summaryDf : origDf) }
           activeCol={activeCol}
           setActiveCol={setActiveCol}
         />
       </div>
     {(widgetConfig.showCommands || widgetConfig.showTransformed) ? (
```

### Comparing `buckaroo-0.3.3/js/components/DFViewer.tsx` & `buckaroo-0.3.4/js/components/DFViewer.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/js/components/DependentTabs.tsx` & `buckaroo-0.3.4/js/components/DependentTabs.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/js/components/OperationDetail.tsx` & `buckaroo-0.3.4/js/components/OperationDetail.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/js/components/OperationUtils.ts` & `buckaroo-0.3.4/js/components/OperationUtils.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/js/components/Operations.tsx` & `buckaroo-0.3.4/js/components/Operations.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/js/components/StatusBar.tsx` & `buckaroo-0.3.4/js/components/StatusBar.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 } from 'react';
 import _ from 'lodash';
 import { AgGridReact } from 'ag-grid-react'; // the AG Grid React Component
 import {
   ColDef,
   GridOptions,
 } from 'ag-grid-community';
-
+import { intFormatter } from './gridUtils';
 export type setColumFunc = (newCol: string) => void;
 
 export interface DfConfig {
   totalRows: number;
   columns: number;
   rowsShown: number;
   sampleSize: number;
@@ -67,18 +67,18 @@
     reorderdColumns,
     showTransformed,
     showCommands
   } = config;
 
   const rowData = [
     {
-      totalRows,
+      totalRows: intFormatter.format(totalRows),
       columns,
-      rowsShown,
-      sampleSize,
+      rowsShown : intFormatter.format(rowsShown),
+      sampleSize : intFormatter.format(sampleSize),
       sampled: sampled  ? "Ϋ" : "ό",
       summaryStats: summaryStats ? "Ϋ" : "ό",
       reorderdColumns: reorderdColumns ? "Ϋ" : "ό",
       showTransformed: showTransformed ? "Ϋ" : "ό",
       showCommands: showCommands ? "Ϋ" : "ό",
     },
   ];
```

### Comparing `buckaroo-0.3.3/js/components/gridUtils.ts` & `buckaroo-0.3.4/js/components/gridUtils.ts`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,41 @@
     } else {
       return { ...x, ...negative };
     }
   });
   return retColumns;
 };
 
+export const intFormatter = new Intl.NumberFormat(
+  'en-US', { minimumFractionDigits:0, maximumFractionDigits: 3 });
+
+const floatFormatter = new Intl.NumberFormat('en-US', { minimumFractionDigits:3, maximumFractionDigits: 3 });
+
+export const anyFormatter = (params: ValueFormatterParams):string => {
+  const val = params.value;
+  try {
+    const num = Number(val)
+    if (val === null) {
+      return "";
+    } else if (val === undefined) {
+      return "";
+    }
+    else if (Number.isFinite(num)) {
+      if (Number.isInteger(num)) {
+	const formatted = intFormatter.format(num)
+	return `${formatted}    `
+      } else {
+	return floatFormatter.format(num)
+      }
+    }
+  } catch (e:any) {
+    //console.log("formatting error", val, e);
+  }
+  return val
+}
 /*
   console.log((new Intl.NumberFormat('en-US')).format(amount))
   console.log((new Intl.NumberFormat('en-US', {  maximumFractionDigits: 1})).format(number))
 
   console.log(`|${last4Digits.padStart(7, ' ')}|`)
   
  valueFormatter: currencyFormatter}
@@ -28,25 +55,24 @@
     
     function currencyFormatter(params) {
         return '£' + formatNumber(params.value);
     }
 */
 function getFormatter(hint: ColumnHint):  ValueFormatterFunc<unknown> {
   if (hint === undefined || hint.is_numeric === false) {
-    return (params: ValueFormatterParams):string => params.value;
+    return anyFormatter;
   } else {
     const commas = Math.floor(hint.max_digits / 3);
 
     if (hint.is_integer) {
       const totalWidth = commas + hint.max_digits;
       return (params: ValueFormatterParams):string => {
         console.log("params", params)
 
         const formatter = new Intl.NumberFormat('en-US');
-        //console.log(`|${last4Digits.padStart(7, ' ')}|`)
         return formatter.format(params.value).padStart(totalWidth, ' ');
       };
     } else {
       /*
 
       const intWidth = commas + hint.max_digits;
       const fracWidth = 4;
@@ -60,16 +86,16 @@
           return [intPart.padStart(intWidth, " "), fracPart.padEnd(3, " ")].join(".") }
         else {
           return numFormatted.padStart(intWidth, " ").padEnd(intWidth + fracWidth, " ")
         }
       };*/
       return (params: ValueFormatterParams):string => {
         //console.log("params", params)
-        const formatter = new Intl.NumberFormat('en-US', { minimumFractionDigits:3, maximumFractionDigits: 3 });
-        return formatter.format(params.value);
+
+        return floatFormatter.format(params.value);
       };
 
     }
   }
 }
 
 export function dfToAgrid(tdf: DFWhole): [ColDef[], unknown[]] {
```

### Comparing `buckaroo-0.3.3/js/components/staticData.ts` & `buckaroo-0.3.4/js/components/staticData.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/js/components/utils.ts` & `buckaroo-0.3.4/js/components/utils.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/js/style/dcf-npm.css` & `buckaroo-0.3.4/js/style/dcf-npm.css`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/static/images/Buckaroo-screenshot.png` & `buckaroo-0.3.4/static/images/Buckaroo-screenshot.png`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/.gitignore` & `buckaroo-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/LICENSE.txt` & `buckaroo-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/README.md` & `buckaroo-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.3/pyproject.toml` & `buckaroo-0.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "ipywidgets>=7.6.0,<9"
 ]
-version = "0.3.3"
+version = "0.3.4"
 
 [project.license]
 file = "LICENSE.txt"
 
 [project.optional-dependencies]
 test = [
     "nbval>=0.9",
```

### Comparing `buckaroo-0.3.3/PKG-INFO` & `buckaroo-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buckaroo
-Version: 0.3.3
+Version: 0.3.4
 Summary: Buckaroo - GUI Data wrangling for pandas
 Project-URL: Homepage, https://github.com/paddymul/buckaroo
 Author: Paddy Mullen
 License: Copyright (c) 2019 Bloomberg
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

