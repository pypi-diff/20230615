# Comparing `tmp/cdpcli-0.9.89.tar.gz` & `tmp/cdpcli-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdpcli-0.9.89.tar", last modified: Wed Jun 14 22:47:31 2023, max compression
+gzip compressed data, was "dist/cdpcli-0.9.9.tar", last modified: Wed Apr  8 03:44:24 2020, max compression
```

## Comparing `cdpcli-0.9.89.tar` & `cdpcli-0.9.9.tar`

### file list

```diff
@@ -1,183 +1,227 @@
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.529270 cdpcli-0.9.89/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11358 2023-06-14 22:34:54.000000 cdpcli-0.9.89/LICENSE.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2309 2023-06-14 22:34:54.000000 cdpcli-0.9.89/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      301 2023-06-14 22:34:54.000000 cdpcli-0.9.89/MANIFEST.in
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7819 2023-06-14 22:47:31.529270 cdpcli-0.9.89/PKG-INFO
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5510 2023-06-14 22:34:54.000000 cdpcli-0.9.89/README.md
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.529270 cdpcli-0.9.89/cdpcli/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3972 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      497 2023-06-14 22:47:31.529270 cdpcli-0.9.89/cdpcli/_version.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8594 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/argparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    16126 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/argprocess.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    13419 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/arguments.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11535 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/auth.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    16324 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/cdprequest.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1207 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/clicommand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31143 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/clidriver.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    22668 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/client.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6574 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/compat.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6562 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/completer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4116 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/config.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8338 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/configloader.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    15597 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/credentials.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.509270 cdpcli-0.9.89/cdpcli/data/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1002 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/data/_retry.json
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      222 2023-06-14 22:47:30.000000 cdpcli-0.9.89/cdpcli/data/aliases.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.509270 cdpcli-0.9.89/cdpcli/data/audit/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    32709 2023-06-14 22:47:30.000000 cdpcli-0.9.89/cdpcli/data/audit/audit.yaml
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3965 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/data/cli.json
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.509270 cdpcli-0.9.89/cdpcli/data/compute/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    15591 2023-06-14 22:47:26.000000 cdpcli-0.9.89/cdpcli/data/compute/compute.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.509270 cdpcli-0.9.89/cdpcli/data/datacatalog/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4002 2023-06-14 22:47:30.000000 cdpcli-0.9.89/cdpcli/data/datacatalog/datacatalog.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.509270 cdpcli-0.9.89/cdpcli/data/datahub/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   142817 2023-06-14 22:47:28.000000 cdpcli-0.9.89/cdpcli/data/datahub/datahub.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.509270 cdpcli-0.9.89/cdpcli/data/datalake/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   101227 2023-06-14 22:47:26.000000 cdpcli-0.9.89/cdpcli/data/datalake/datalake.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.509270 cdpcli-0.9.89/cdpcli/data/de/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    32532 2023-06-14 22:47:29.000000 cdpcli-0.9.89/cdpcli/data/de/de.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.509270 cdpcli-0.9.89/cdpcli/data/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    91702 2023-06-14 22:47:27.000000 cdpcli-0.9.89/cdpcli/data/df/df.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.513270 cdpcli-0.9.89/cdpcli/data/dfworkload/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    81768 2023-06-14 22:47:29.000000 cdpcli-0.9.89/cdpcli/data/dfworkload/dfworkload.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.513270 cdpcli-0.9.89/cdpcli/data/drscp/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    21583 2023-06-14 22:47:26.000000 cdpcli-0.9.89/cdpcli/data/drscp/drscp.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.513270 cdpcli-0.9.89/cdpcli/data/dw/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   193260 2023-06-14 22:47:26.000000 cdpcli-0.9.89/cdpcli/data/dw/dw.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.513270 cdpcli-0.9.89/cdpcli/data/environments/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   163226 2023-06-14 22:47:25.000000 cdpcli-0.9.89/cdpcli/data/environments/environments.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.513270 cdpcli-0.9.89/cdpcli/data/iam/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   132904 2023-06-14 22:47:28.000000 cdpcli-0.9.89/cdpcli/data/iam/iam.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.513270 cdpcli-0.9.89/cdpcli/data/imagecatalog/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    19320 2023-06-14 22:47:26.000000 cdpcli-0.9.89/cdpcli/data/imagecatalog/imagecatalog.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.513270 cdpcli-0.9.89/cdpcli/data/ml/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    56809 2023-06-14 22:47:29.000000 cdpcli-0.9.89/cdpcli/data/ml/ml.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.513270 cdpcli-0.9.89/cdpcli/data/opdb/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    24469 2023-06-14 22:47:29.000000 cdpcli-0.9.89/cdpcli/data/opdb/opdb.yaml
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        6 2023-06-14 22:47:30.000000 cdpcli-0.9.89/cdpcli/data/release.txt
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.513270 cdpcli-0.9.89/cdpcli/data/replicationmanager/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    30963 2023-06-14 22:47:30.000000 cdpcli-0.9.89/cdpcli/data/replicationmanager/replicationmanager.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.513270 cdpcli-0.9.89/cdpcli/doc/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/doc/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1857 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/doc/docstringparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7269 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/doc/restdoc.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10873 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/doc/style.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    29420 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/docs.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17043 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/endpoint.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.497269 cdpcli-0.9.89/cdpcli/examples/
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.513270 cdpcli-0.9.89/cdpcli/examples/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1942 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/examples/configure/_description.rst
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.513270 cdpcli-0.9.89/cdpcli/examples/configure/get/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1940 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/examples/configure/get/_description.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      764 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/examples/configure/get/_examples.rst
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.517270 cdpcli-0.9.89/cdpcli/examples/configure/set/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      862 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/examples/configure/set/_description.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      560 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/examples/configure/set/_examples.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9213 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/exceptions.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.517270 cdpcli-0.9.89/cdpcli/extensions/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      971 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/extensions/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2650 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/extensions/arguments.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3908 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/extensions/cliinputjson.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17226 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/extensions/commands.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.517270 cdpcli-0.9.89/cdpcli/extensions/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1330 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/extensions/configure/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2047 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/extensions/configure/classify.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6210 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/extensions/configure/configure.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3749 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/extensions/configure/get.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6414 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/extensions/configure/list.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5108 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/extensions/configure/set.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.521270 cdpcli-0.9.89/cdpcli/extensions/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12046 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/extensions/df/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    29050 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/extensions/df/createdeployment.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1575 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/extensions/df/register.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3353 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/extensions/generatecliskeleton.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10396 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/extensions/interactivelogin.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2154 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/extensions/logout.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9335 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/extensions/paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2642 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/extensions/redirect.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6277 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/extensions/refdoc.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3771 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/extensions/workload.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11071 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/extensions/writer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9343 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/formatter.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8083 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/help.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9314 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/loader.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      771 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/main.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    18902 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/model.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7307 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5898 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/paramfile.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3218 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/paramformfactor.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4085 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/parser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11836 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/retryhandler.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5732 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/schema.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4322 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/serialize.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14202 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/shorthand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2258 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/signers.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14828 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/table.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4389 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/text.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    20981 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/textwriter.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.521270 cdpcli-0.9.89/cdpcli/thirdparty/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/thirdparty/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    27344 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/thirdparty/six.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1652 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/translate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10165 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/utils.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10637 2023-06-14 22:34:54.000000 cdpcli-0.9.89/cdpcli/validate.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.509270 cdpcli-0.9.89/cdpcli.egg-info/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7819 2023-06-14 22:47:31.000000 cdpcli-0.9.89/cdpcli.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4214 2023-06-14 22:47:31.000000 cdpcli-0.9.89/cdpcli.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        1 2023-06-14 22:47:31.000000 cdpcli-0.9.89/cdpcli.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)       85 2023-06-14 22:47:31.000000 cdpcli-0.9.89/cdpcli.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      190 2023-06-14 22:47:31.000000 cdpcli-0.9.89/cdpcli.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)       13 2023-06-14 22:47:31.000000 cdpcli-0.9.89/cdpcli.egg-info/top_level.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      271 2023-06-14 22:47:31.529270 cdpcli-0.9.89/setup.cfg
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1414 2023-06-14 22:34:54.000000 cdpcli-0.9.89/setup.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2655 2023-06-14 22:34:54.000000 cdpcli-0.9.89/setup_common.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.497269 cdpcli-0.9.89/tests/
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.525270 cdpcli-0.9.89/tests/unit/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4604 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.525270 cdpcli-0.9.89/tests/unit/cdp/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1815 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/cdp/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.525270 cdpcli-0.9.89/tests/unit/extensions/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      732 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/extensions/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.529270 cdpcli-0.9.89/tests/unit/extensions/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/extensions/configure/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2290 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/extensions/configure/test_classify.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12860 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/extensions/configure/test_configure.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5637 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/extensions/configure/test_get.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6675 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/extensions/configure/test_list.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6656 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/extensions/configure/test_set.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.529270 cdpcli-0.9.89/tests/unit/extensions/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/extensions/df/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    38131 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/extensions/df/test_createdeployment.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2253 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/extensions/df/test_upload_file.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5854 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/extensions/test_cliinputjson.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    18795 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/extensions/test_df.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3807 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/extensions/test_generatecliskeleton.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17115 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/extensions/test_interactivelogin.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2556 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/extensions/test_logout.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8305 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/extensions/test_operation_extension.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10918 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/extensions/test_paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4828 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/extensions/test_redirect.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9041 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/extensions/test_workload.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11649 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/extensions/test_writer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2709 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/test_argparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4768 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/test_argprocess.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11931 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/test_auth.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4421 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/test_cli_data.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12187 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/test_client.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14018 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/test_completer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    23039 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/test_credentials.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7271 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/test_docs.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31273 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/test_endpoint.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10750 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/test_help.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12035 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/test_loaders.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14102 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/test_model.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    15246 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/test_paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8243 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/test_paramfile.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14417 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/test_protocol.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    13714 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/test_retryhandler.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11240 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/test_shorthand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3227 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/test_signers.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    22467 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/test_table_formatter.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12971 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/test_utils.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12772 2023-06-14 22:34:54.000000 cdpcli-0.9.89/tests/unit/test_validate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    68612 2023-06-14 22:34:54.000000 cdpcli-0.9.89/versioneer.py
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    49425 2020-04-08 03:37:47.000000 cdpcli-0.9.9/NOTICES.txt
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     2309 2020-04-08 03:37:47.000000 cdpcli-0.9.9/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    68612 2020-04-08 03:37:47.000000 cdpcli-0.9.9/versioneer.py
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli.egg-info/
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)       85 2020-04-08 03:44:22.000000 cdpcli-0.9.9/cdpcli.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)        1 2020-04-08 03:44:22.000000 cdpcli-0.9.9/cdpcli.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     1343 2020-04-08 03:44:22.000000 cdpcli-0.9.9/cdpcli.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)       13 2020-04-08 03:44:22.000000 cdpcli-0.9.9/cdpcli.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)      144 2020-04-08 03:44:22.000000 cdpcli-0.9.9/cdpcli.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     7594 2020-04-08 03:44:22.000000 cdpcli-0.9.9/cdpcli.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    11358 2020-04-08 03:37:47.000000 cdpcli-0.9.9/LICENSE.txt
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     1343 2020-04-08 03:44:24.000000 cdpcli-0.9.9/PKG-INFO
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/thirdparty/
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     2517 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/exceptions.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    16810 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/adapters.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)   308434 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/cacert.pem
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)      820 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/hooks.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     5415 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/api.py
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     4374 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/exceptions.py
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/contrib/
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     4507 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/contrib/ntlmpool.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     9326 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/contrib/pyopenssl.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/contrib/__init__.py
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/packages/
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    11628 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/packages/six.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     8935 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/packages/ordered_dict.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)       74 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/packages/__init__.py
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/packages/ssl_match_hostname/
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     3778 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)      460 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/packages/ssl_match_hostname/__init__.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     2281 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/filepost.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     9011 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/connection.py
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/util/
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    10037 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/util/ssl_.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     9544 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/util/timeout.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     5836 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/util/url.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     9924 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/util/retry.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     3293 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/util/connection.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)      566 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/util/response.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     2089 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/util/request.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)      486 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/util/__init__.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     9406 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/poolmanager.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    16459 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/response.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     5833 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/fields.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     5751 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/request.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    30319 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/connectionpool.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     2055 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/__init__.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    10428 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/urllib3/_collections.py
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     3187 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/escprober.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    45972 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/euckrfreq.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     1902 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/charsetprober.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     1674 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/euctwprober.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     1967 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/mbcsgroupprober.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     2318 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/codingstatemachine.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    11318 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/langhebrewmodel.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    17725 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/langcyrillicmodel.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     6840 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/universaldetector.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     1684 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/big5prober.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     7839 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/escsm.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     2652 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/utf8prober.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     9226 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/chardistribution.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    82594 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/big5freq.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    19348 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/jpcntx.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    12784 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/langbulgarianmodel.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    47315 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/jisfreq.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     1675 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/euckrprober.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    19590 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/mbcssm.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    36011 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/gb2312freq.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    12536 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/langhungarianmodel.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    34872 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/euctwfreq.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     1782 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/cp949prober.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     1333 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/constants.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     2504 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/chardetect.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     3764 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/sjisprober.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     3291 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/sbcsgroupprober.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     3787 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/charsetgroupprober.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    11275 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/langthaimodel.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    13359 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/hebrewprober.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     3678 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/eucjpprober.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     1157 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/compat.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     1679 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/gb2312prober.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     1295 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/__init__.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     5232 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/latin1prober.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     4793 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/sbcharsetprober.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    12628 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/langgreekmodel.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     3268 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/chardet/mbcharsetprober.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)       62 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/packages/__init__.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    17191 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/cookies.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    24250 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/sessions.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     2977 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/structures.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)      613 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/certs.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     6794 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/auth.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    29176 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/models.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     3200 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/status_codes.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    21334 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/utils.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     1469 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/compat.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     1861 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/requests/__init__.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    27344 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/six.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/thirdparty/__init__.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     6261 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/exceptions.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    16363 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/cdprequest.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)      497 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/_version.py
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/extensions/
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     3837 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/extensions/cliinputjson.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     3344 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/extensions/generatecliskeleton.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    17092 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/extensions/commands.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     9335 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/extensions/paginate.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    11071 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/extensions/writer.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     2641 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/extensions/arguments.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)      971 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/extensions/__init__.py
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/extensions/configure/
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     3749 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/extensions/configure/get.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     4854 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/extensions/configure/set.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     6203 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/extensions/configure/configure.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     5432 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/extensions/configure/list.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     1357 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/extensions/configure/__init__.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    11436 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/credentials.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)      771 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/main.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     9950 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/validate.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    20401 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/client.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    20750 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/clidriver.py
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/doc/
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    10699 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/doc/style.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     7269 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/doc/restdoc.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     1857 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/doc/docstringparser.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/doc/__init__.py
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/examples/
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/examples/configure/
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/examples/configure/get/
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)      764 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/examples/configure/get/_examples.rst
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     1936 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/examples/configure/get/_description.rst
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     1193 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/examples/configure/_description.rst
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/examples/configure/set/
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)      560 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/examples/configure/set/_examples.rst
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)      862 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/examples/configure/set/_description.rst
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/examples/dataeng/
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     2137 2020-04-08 03:44:21.000000 cdpcli-0.9.9/cdpcli/examples/dataeng/submit-jobs.rst
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     3401 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/serialize.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    11896 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/retryhandler.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     6963 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/paginate.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    14764 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/table.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    16344 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/model.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    22915 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/docs.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    13740 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/shorthand.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    13421 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/arguments.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     9313 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/loader.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     8353 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/configloader.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    10239 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/endpoint.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     4389 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/text.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     1652 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/translate.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     7949 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/auth.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     7604 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/argparser.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    20851 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/textwriter.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     3437 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/parser.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     7334 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/help.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     9323 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/utils.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     6528 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/compat.py
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/data/
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/data/iam/
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    94175 2020-04-08 03:44:21.000000 cdpcli-0.9.9/cdpcli/data/iam/iam.yaml
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)       73 2020-04-08 03:44:21.000000 cdpcli-0.9.9/cdpcli/data/aliases.yaml
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     1002 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/data/_retry.json
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/data/datalake/
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    22237 2020-04-08 03:44:21.000000 cdpcli-0.9.9/cdpcli/data/datalake/datalake.yaml
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/data/ml/
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    29396 2020-04-08 03:44:20.000000 cdpcli-0.9.9/cdpcli/data/ml/ml.yaml
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     2070 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/data/cli.json
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/data/environments/
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    57881 2020-04-08 03:44:21.000000 cdpcli-0.9.9/cdpcli/data/environments/environments.yaml
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/cdpcli/data/datahub/
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    50828 2020-04-08 03:44:21.000000 cdpcli-0.9.9/cdpcli/data/datahub/datahub.yaml
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     9211 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/formatter.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     6456 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/completer.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     1207 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/clicommand.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     5732 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/schema.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     2241 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/signers.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     3377 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/__init__.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     4824 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/paramfile.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    16301 2020-04-08 03:37:47.000000 cdpcli-0.9.9/cdpcli/argprocess.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     2433 2020-04-08 03:37:47.000000 cdpcli-0.9.9/setup.py
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/tests/
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/tests/unit/
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/tests/unit/cdp/
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     1815 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/cdp/__init__.py
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/tests/unit/extensions/
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     5370 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/extensions/test_cliinputjson.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     3807 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/extensions/test_generatecliskeleton.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    10918 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/extensions/test_paginate.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    11649 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/extensions/test_writer.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)      732 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/extensions/__init__.py
+drwxrwxr-x   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:44:24.000000 cdpcli-0.9.9/tests/unit/extensions/configure/
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    13191 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/extensions/configure/test_configure.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     6143 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/extensions/configure/test_list.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     5696 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/extensions/configure/test_set.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)        0 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/extensions/configure/__init__.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     5637 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/extensions/configure/test_get.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     8304 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_auth.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     3412 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_argprocess.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     6671 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_help.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    12035 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_loaders.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    11015 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_protocol.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     6829 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_client.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     6354 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_paramfile.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    11859 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_utils.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     2663 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_cli_data.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    12543 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_model.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    14273 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_paginate.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    22467 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_table_formatter.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    18652 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_credentials.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    14551 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_endpoint.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     3116 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_signers.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     4603 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_docs.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    12725 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_completer.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     2642 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_argparser.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    11124 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_shorthand.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     8860 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_validate.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)    13775 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/test_retryhandler.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)     4162 2020-04-08 03:37:47.000000 cdpcli-0.9.9/tests/unit/__init__.py
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)      314 2020-04-08 03:44:24.000000 cdpcli-0.9.9/setup.cfg
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)      308 2020-04-08 03:37:47.000000 cdpcli-0.9.9/MANIFEST.in
+-rw-rw-r--   0 jenkins    (114) jenkins    (118)      451 2020-04-08 03:37:47.000000 cdpcli-0.9.9/README.rst
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `cdpcli-0.9.89/LICENSE.txt` & `cdpcli-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.89/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt` & `cdpcli-0.9.9/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.89/cdpcli/__init__.py` & `cdpcli-0.9.9/cdpcli/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,30 +16,21 @@
 
 import os
 import re
 
 from ._version import get_versions
 
 
-# Retrieve the version number from versioneer's code.
 __version__ = get_versions()['version']
 del get_versions
 
 VERSION = __version__
 
 CDPCLI_ROOT = os.path.dirname(os.path.abspath(__file__))
 
-# Read in the release file and update the advertised version with it if it's
-# not the default / PUBLIC release.
-_release_file_path = os.path.normpath("{0}/data/release.txt".format(CDPCLI_ROOT))
-with open(_release_file_path) as releaseFile:
-    RELEASE = releaseFile.readline()
-
-if RELEASE != 'PUBLIC':
-    VERSION += ' (%s)' % RELEASE
 
 # Used to specify anonymous (unsigned) request signature
 UNSIGNED = object()
 
 
 SCALAR_TYPES = set(['string',
                     'float',
@@ -61,19 +52,14 @@
 COMPLEX_TYPES = set([OBJECT_TYPE,
                      LIST_TYPE,
                      MAP_TYPE])
 
 DEFAULT_PROFILE_NAME = 'default'
 CDP_ACCESS_KEY_ID_KEY_NAME = 'cdp_access_key_id'
 CDP_PRIVATE_KEY_KEY_NAME = 'cdp_private_key'
-CDP_ACCESS_TOKEN_KEY_NAME = 'cdp_access_token'
-CDP_REGION_KEY_NAME = 'cdp_region'
-CDP_ENDPOINT_URL_KEY_NAME = 'cdp_endpoint_url'
-ENDPOINT_URL_KEY_NAME = 'endpoint_url'
-FORM_FACTOR_KEY_NAME = 'form_factor'
 # Python argparse has a bug in which '-' are not parsed correctly if they appear
 # as values for other arguments, see: http://bugs.python.org/issue9334 for more
 # details. This defines special encoding for dash that we will "decode" and
 # replace with a dash. The reason we are using \\ is that there is a non zero
 # chance that customers can discover this themselves.
 ARGPARSE_DASH_ENCODING = '\\-'
```

### Comparing `cdpcli-0.9.89/cdpcli/argparser.py` & `cdpcli-0.9.9/cdpcli/argparser.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,24 +13,36 @@
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 import argparse
 from difflib import get_close_matches
 import logging
-import os
 import sys
 
 from cdpcli import ARGPARSE_DASH_ENCODING
 from cdpcli.compat import six
 
 
 LOG = logging.getLogger('cdpcli.argparser')
 
 
+HELP_BLURB = (
+    "To see help text, you can run:\n"
+    "\n"
+    "  cdp help\n"
+    "  cdp <command> help\n"
+    "  cdp <command> <subcommand> help\n"
+)
+USAGE = (
+    "cdp [options] <command> <subcommand> [<subcommand> ...] [parameters]\n"
+    "%s" % HELP_BLURB
+)
+
+
 class CLIArgParser(argparse.ArgumentParser):
     Formatter = argparse.RawTextHelpFormatter
 
     # When displaying invalid choice error messages, this controls how many
     # options to show per line.
     ChoicesPerLine = 2
 
@@ -38,21 +50,19 @@
         """
         It's probably not a great idea to override a "hidden" method but the default
         behavior is pretty ugly and there doesn't seem to be any other way to change
         it.
         """
         # converted value must be one of the choices (if specified)
         if action.choices is not None and value not in action.choices:
-            choice_max_len = len(max(action.choices, key=len))
-            column_width = max(choice_max_len, 40)
             msg = ['Invalid choice, valid choices are:\n']
             for i in range(len(action.choices))[::self.ChoicesPerLine]:
                 current = []
                 for choice in action.choices[i:i + self.ChoicesPerLine]:
-                    current.append(('%-' + str(column_width) + 's') % choice)
+                    current.append('%-40s' % choice)
                 msg.append(' | '.join(current))
             possible = get_close_matches(value, action.choices, cutoff=0.8)
             if possible:
                 extra = ['\n\nInvalid choice: %r, maybe you meant:\n' % value]
                 for word in possible:
                     extra.append('  * %s' % word)
                 msg.extend(extra)
@@ -110,17 +120,16 @@
                  description,
                  argument_table):
         super(MainArgParser, self).__init__(
             formatter_class=self.Formatter,
             add_help=False,
             conflict_handler='resolve',
             description=description,
-            allow_abbrev=False)
+            usage=USAGE)
         self._build(command_table, version_string, argument_table)
-        self._command_table = command_table
 
     def _create_choice_help(self, choices):
         help_str = ''
         for choice in sorted(choices):
             help_str += '* %s\n' % choice
         return help_str
 
@@ -130,75 +139,54 @@
             argument.add_to_parser(self)
         self.add_argument('--version',
                           action="version",
                           version=version_string,
                           help='Display the version of this tool')
         self.add_argument('command', choices=list(command_table.keys()))
 
-    def parse_known_args(self, args, namespace=None):
-        """
-        Parses normally, but also adds the command_table to the parsed
-        arguments, so that commands like refdoc may access it. This is a hack.
-        """
-        parsed, remaining = super(MainArgParser, self).parse_known_args(args, namespace)
-        setattr(parsed, 'command_table', self._command_table)
-        return parsed, remaining
-
 
 class ArgTableArgParser(CLIArgParser):
 
-    def __init__(self, argument_table, service_name=None, operation_name=None,
-                 command_table=None):
+    def __init__(self, argument_table, command_table=None):
         # command_table is an optional subcommand_table.  If it's passed
         # in, then we'll update the argparse to parse a 'subcommand' argument
         # and populate the choices field with the command table keys.
-        if service_name and operation_name:
-            progString = "{} {} {}".format(os.path.basename(sys.argv[0]), service_name,
-                                           operation_name)
-        else:
-            progString = os.path.basename(sys.argv[0])
         super(ArgTableArgParser, self).__init__(
-            prog=progString,
             formatter_class=self.Formatter,
             add_help=False,
+            usage=USAGE,
             conflict_handler='resolve')
         if command_table is None:
             command_table = {}
         self._build(argument_table, command_table)
 
     def _build(self, argument_table, command_table):
         for arg_name in argument_table:
             argument = argument_table[arg_name]
             argument.add_to_parser(self)
         if command_table:
             self.add_argument('subcommand', choices=list(command_table.keys()),
                               nargs='?')
 
     def parse_known_args(self, args, namespace=None):
-        if len(args) == 1 and (args[0] == 'help' or args[0] == '--help'):
+        if len(args) == 1 and args[0] == 'help':
             namespace = argparse.Namespace()
             namespace.help = 'help'
             return namespace, []
         else:
             return super(ArgTableArgParser, self).parse_known_args(
                 args, namespace)
 
 
 class ServiceArgParser(CLIArgParser):
 
     def __init__(self, operations_table, service_name):
         super(ServiceArgParser, self).__init__(
-            prog="{} {}".format(os.path.basename(sys.argv[0]), service_name),
             formatter_class=argparse.RawTextHelpFormatter,
             add_help=False,
-            conflict_handler='resolve')
+            conflict_handler='resolve',
+            usage=USAGE)
         self._build(operations_table)
         self._service_name = service_name
 
     def _build(self, operations_table):
         self.add_argument('operation', choices=list(operations_table.keys()))
-
-    def parse_known_args(self, args, namespace=None):
-        if len(args) == 0 or (len(args) == 1 and args[0] == '--help'):
-            args = ['help']
-        return super(ServiceArgParser, self).parse_known_args(
-            args, namespace)
```

### Comparing `cdpcli-0.9.89/cdpcli/argprocess.py` & `cdpcli-0.9.9/cdpcli/argprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 #     http://aws.amazon.com/apache2.0/
 #
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
+import os
+
 from cdpcli import COMPLEX_TYPES
 from cdpcli import LIST_TYPE
 from cdpcli import MAP_TYPE
 from cdpcli import OBJECT_TYPE
 from cdpcli import SCALAR_TYPES
 from cdpcli import shorthand
 from cdpcli.compat import json
@@ -56,35 +58,33 @@
         super(ParamUnknownKeyError, self).__init__(full_message)
 
 
 class TooComplexError(Exception):
     pass
 
 
-def unpack_argument(cli_argument, value, parsed_globals):
-    override = uri_param(cli_argument, value, parsed_globals)
+def unpack_argument(cli_argument, value):
+    override = uri_param(cli_argument, value)
     if override is not None:
         value = override
     return value
 
 
-def uri_param(cli_argument, value, parsed_globals):
-    if not getattr(parsed_globals, 'expand_param', True):
-        return
-    elif getattr(cli_argument, 'no_paramfile', None):
+def uri_param(cli_argument, value):
+    if getattr(cli_argument, 'no_paramfile', None):
         return
     else:
-        return _check_for_uri_param(cli_argument, value, parsed_globals)
+        return _check_for_uri_param(cli_argument, value)
 
 
-def _check_for_uri_param(param, value, parsed_globals):
+def _check_for_uri_param(param, value):
     if isinstance(value, list) and len(value) == 1:
         value = value[0]
     try:
-        return get_paramfile(value, parsed_globals)
+        return get_paramfile(value)
     except ResourceLoadingError as e:
         raise ParamError(param.cli_name, six.text_type(e))
 
 
 def unpack_cli_arg(cli_argument, value):
     """
     Parses and unpacks the encoded string command line parameter
@@ -156,14 +156,22 @@
     # Note the cli_name is used strictly for error reporting.  It's
     # not required to use unpack_scalar_cli_arg
     if argument_model.type_name == 'integer' or argument_model.type_name == 'long':
         return int(value)
     elif argument_model.type_name == 'float' or argument_model.type_name == 'double':
         # TODO: losing precision on double types
         return float(value)
+    elif argument_model.type_name == 'blob' and \
+            argument_model.serialization.get('streaming'):
+        file_path = os.path.expandvars(value)
+        file_path = os.path.expanduser(file_path)
+        if not os.path.isfile(file_path):
+            msg = 'Blob values must be a path to a file.'
+            raise ParamError(cli_name, msg)
+        return open(file_path, 'rb')
     elif argument_model.type_name == 'boolean':
         if isinstance(value, six.string_types) and value.lower() == 'false':
             return False
         return bool(value)
     else:
         return value
 
@@ -327,16 +335,15 @@
 
         # Otherwise we fall back to the normal docgen for shorthand
         # syntax.
         stack = []
         try:
             if argument_model.type_name == LIST_TYPE:
                 argument_model = argument_model.member
-                return self._shorthand_docs(argument_model, stack) + \
-                    ' ... (separate items with spaces)'
+                return self._shorthand_docs(argument_model, stack) + ' ...'
             else:
                 return self._shorthand_docs(argument_model, stack)
         except TooComplexError:
             return ''
 
     def _handle_special_cases(self, cli_name, model):
         if model.type_name == LIST_TYPE and \
```

### Comparing `cdpcli-0.9.89/cdpcli/arguments.py` & `cdpcli-0.9.9/cdpcli/arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,15 +283,15 @@
         if serialized_name is None:
             serialized_name = name
         self._serialized_name = serialized_name
         self.argument_model = argument_model
         self._required = is_required
         self._operation_model = operation_model
         self.no_paramfile = no_paramfile
-        self._UNDOCUMENTED = self.argument_model.is_deprecated
+        self._UNDOCUMENTED = self.argument_model.is_undocumented
 
     @property
     def py_name(self):
         return self._name.replace('-', '_')
 
     @property
     def required(self):
```

### Comparing `cdpcli-0.9.89/cdpcli/auth.py` & `cdpcli-0.9.9/cdpcli/auth.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,24 +12,21 @@
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 from base64 import b64decode, urlsafe_b64encode
 from email.utils import formatdate
-import hashlib
 import logging
 
 from asn1crypto import keys, pem
 from cdpcli.compat import json
 from cdpcli.compat import OrderedDict
 from cdpcli.compat import urlsplit
 from cdpcli.exceptions import NoCredentialsError
-from ecdsa import SigningKey
-from ecdsa.util import sigencode_der
 from pure25519 import eddsa
 import rsa
 
 
 LOG = logging.getLogger('cdpcli.auth')
 
 
@@ -92,16 +89,15 @@
     def _get_signature(self, method, split, headers):
         string_to_sign = self._canonical_string(method, split, headers)
         LOG.debug('StringToSign:\n%s', string_to_sign)
         return self._sign_string(string_to_sign)
 
     def add_auth(self, request):
         if self.credentials is None:
-            raise NoCredentialsError(
-                err_msg='Credentials not available for request signing')
+            raise NoCredentialsError
         LOG.debug("Calculating signature using %s." % self.auth_method)
         LOG.debug('HTTP request method: %s', request.method)
         split = urlsplit(request.url)
         signature = self._get_signature(request.method,
                                         split,
                                         request.headers)
         self._inject_signature(request, signature)
@@ -198,100 +194,11 @@
             LOG.debug(message, exc_info=True)
             raise Exception(message)
         # We sign the hash.
         signature = rsa.sign(string_to_sign.encode('utf-8'), key, 'SHA-256')
         return signature
 
 
-class ECDSAv1Auth(V1Signer):
-    """
-    ECDSA signing with a SHA-512 hash returning a base64 encoded signature.
-    """
-    AUTH_METHOD_NAME = 'ecdsav1'
-
-    def __init__(self, credentials):
-        super(ECDSAv1Auth, self).__init__(credentials, self.AUTH_METHOD_NAME)
-
-    @staticmethod
-    def _parse_private_key(private_key, error_message="Failed to import private key."):
-        """
-        Parse the ECDSA private key.
-        :param private_key: The private key.
-        :return: The SigningKey.
-        :raise: Exception if the private key can not be parsed.
-        """
-        try:
-            # We expect the private key to be a PKCS8 pem formatted string.
-            pem_bytes = private_key.encode('utf-8')
-            if pem.detect(pem_bytes):
-                _, _, der_bytes = pem.unarmor(pem_bytes)
-                # In PKCS8 the key is wrapped in a container that describes it
-                info = keys.PrivateKeyInfo.load(der_bytes, strict=True)
-                # Directly unwrap the private key. The asn1crypto library stopped
-                # offering an API call for this in their 1.0.0 release but their
-                # official answer of using a separate native-code-dependent
-                # library to do one line of work is unreasonable. Of course, this
-                # line might break in the future...
-                unwrapped = info['private_key'].parsed
-                # The unwrapped key is equivalent to pkcs1 contents
-                return SigningKey.from_der(unwrapped.dump())
-            else:
-                raise Exception('Not a PEM file')
-        except Exception:
-            LOG.debug(error_message, exc_info=True)
-            raise Exception(error_message)
-
-    @staticmethod
-    def detect_private_key(private_key):
-        """
-        Try to see if the private key is an ECDSA key by parsing it.
-        :param private_key: The key to check.
-        :return: True if the key is an ECDSA key, False otherwise.
-        """
-        try:
-            ECDSAv1Auth._parse_private_key(private_key)
-            return True
-        except Exception:
-            return False
-
-    def _raw_sign_string(self, string_to_sign):
-        """
-        Sign the supplied string using the credentials and return the raw signature.
-        :param string_to_sign: String to sign
-        :return: Raw signature as string
-        """
-        sk = ECDSAv1Auth._parse_private_key(
-            self.credentials.private_key,
-            self.ERROR_MESSAGE % self.credentials.method)
-        # Sign the hash.
-        signature = sk.sign_deterministic(
-            string_to_sign.encode('utf-8'),
-            hashfunc=hashlib.sha512,
-            sigencode=sigencode_der)
-        return signature
-
-
-class AccessTokenAuth:
-    AUTH_METHOD_NAME = 'access_token'
-
-    def __init__(self, credentials):
-        self._credentials = credentials
-
-    def add_auth(self, request):
-        if self._credentials is None:
-            raise NoCredentialsError(
-                err_msg='Credentials not available for request signing')
-        if 'Authorization' in request.headers:
-            raise Exception("Authorization found in headers!")
-        request.headers['Authorization'] = self._credentials.access_token
-
-    @classmethod
-    def is_access_token(cls, access_token):
-        return bool(access_token)
-
-
 AUTH_TYPE_MAPS = {
-    ECDSAv1Auth.AUTH_METHOD_NAME: ECDSAv1Auth,
     Ed25519v1Auth.AUTH_METHOD_NAME: Ed25519v1Auth,
     RSAv1Auth.AUTH_METHOD_NAME: RSAv1Auth,
-    AccessTokenAuth.AUTH_METHOD_NAME: AccessTokenAuth
 }
```

### Comparing `cdpcli-0.9.89/cdpcli/cdprequest.py` & `cdpcli-0.9.9/cdpcli/cdprequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,21 +21,20 @@
 
 from cdpcli.compat import HTTPHeaders
 from cdpcli.compat import HTTPResponse
 from cdpcli.compat import six
 from cdpcli.compat import urlsplit
 from cdpcli.compat import urlunsplit
 from cdpcli.exceptions import UnseekableStreamError
-from cdpcli.utils import is_absolute_url
-from requests import models
-from requests.sessions import REDIRECT_STATI
-from urllib3.connection import HTTPConnection
-from urllib3.connection import VerifiedHTTPSConnection  # noqa
-from urllib3.connectionpool import HTTPConnectionPool   # noqa
-from urllib3.connectionpool import HTTPSConnectionPool  # noqa
+from cdpcli.thirdparty.requests import models
+from cdpcli.thirdparty.requests.packages.urllib3.connection import HTTPConnection
+from cdpcli.thirdparty.requests.packages.urllib3.connection import VerifiedHTTPSConnection  # noqa
+from cdpcli.thirdparty.requests.packages.urllib3.connectionpool import HTTPConnectionPool   # noqa
+from cdpcli.thirdparty.requests.packages.urllib3.connectionpool import HTTPSConnectionPool  # noqa
+from cdpcli.thirdparty.requests.sessions import REDIRECT_STATI
 
 
 def _urljoin(endpoint_url, url_path):
     p = urlsplit(endpoint_url)
     # <part>   - <index>
     # scheme   - p[0]
     # netloc   - p[1]
@@ -63,19 +62,15 @@
         additional_headers):
     r = request_dict
     headers = r['headers']
     for name, value in additional_headers.items():
         headers[name] = value
     if user_agent_header is not None:
         headers['User-Agent'] = user_agent_header
-    url_path = r['url_path']
-    if is_absolute_url(url_path):
-        r['url'] = url_path
-    else:
-        r['url'] = _urljoin(endpoint_url, url_path)
+    r['url'] = _urljoin(endpoint_url, r['url_path'])
 
 
 def create_request_object(request_dict):
     return CdpRequest(method=request_dict['method'],
                       url=request_dict['url'],
                       data=request_dict['body'],
                       headers=request_dict['headers'])
```

### Comparing `cdpcli-0.9.89/cdpcli/clicommand.py` & `cdpcli-0.9.9/cdpcli/clicommand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.89/cdpcli/client.py` & `cdpcli-0.9.9/cdpcli/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,31 +16,28 @@
 
 import copy
 import os
 import uuid
 
 from cdpcli import credentials, DEFAULT_PROFILE_NAME
 from cdpcli import xform_name
-from cdpcli.auth import AccessTokenAuth
-from cdpcli.auth import ECDSAv1Auth
 from cdpcli.auth import Ed25519v1Auth
 from cdpcli.auth import RSAv1Auth
 from cdpcli.cdprequest import prepare_request_dict
 from cdpcli.configloader import load_config, raw_config_parse
 from cdpcli.endpoint import DEFAULT_TIMEOUT
 from cdpcli.exceptions import ClientError, ConfigNotFound, ProfileNotFound
 from cdpcli.exceptions import OperationNotPageableError
 from cdpcli.model import ServiceModel
 from cdpcli.paginate import Paginator
 from cdpcli.serialize import create_serializer
 from cdpcli.signers import RequestSigner
 from cdpcli.utils import get_service_module_name
 
-ALTUS_REQUEST_ID_HEADER = 'x-altus-request-id'
-CDP_REQUEST_ID_HEADER = 'x-cdp-request-id'
+CDP_REQUEST_ID_HEADER = 'x-altus-request-id'
 
 
 class ClientCreator(object):
 
     def __init__(self,
                  loader,
                  context,
@@ -57,27 +54,23 @@
 
     @property
     def context(self):
         return self._context
 
     def create_client(self,
                       service_name,
-                      explicit_endpoint_url,
-                      region,
+                      endpoint_url,
                       tls_verification,
-                      credentials,
-                      client_config=None):
+                      credentials):
         service_model = self._load_service_model(service_name)
         cls = self._create_client_class(service_name, service_model)
         client_args = self._get_client_args(service_model,
-                                            explicit_endpoint_url,
-                                            region,
+                                            endpoint_url,
                                             tls_verification,
-                                            credentials,
-                                            client_config)
+                                            credentials)
         return cls(**client_args)
 
     def _load_service_model(self, service_name):
         service_data = self._loader.load_service_data(service_name)
         return ServiceModel(service_data, service_name=service_name)
 
     def _create_client_class(self, service_name, service_model):
@@ -87,47 +80,29 @@
         bases = [BaseClient]
         class_name = get_service_module_name(service_model)
         cls = type(str(class_name), tuple(bases), class_attributes)
         return cls
 
     def _get_client_args(self,
                          service_model,
-                         explicit_endpoint_url,
-                         region,
+                         endpoint_url,
                          tls_verification,
-                         credentials,
-                         client_config):
-        """Get keyword arguments for constructing a client object.
-        """
+                         credentials):
         serializer = create_serializer()
-        if client_config is not None:
-            connect_timeout = client_config.connect_timeout
-            if connect_timeout <= 0:
-                connect_timeout = None
-            read_timeout = client_config.read_timeout
-            if read_timeout <= 0:
-                read_timeout = None
-        else:
-            connect_timeout = DEFAULT_TIMEOUT
-            read_timeout = DEFAULT_TIMEOUT
+        timeout = (DEFAULT_TIMEOUT, DEFAULT_TIMEOUT)
         endpoint = self._endpoint_creator.create_endpoint(
             service_model,
-            explicit_endpoint_url,
+            endpoint_url,
             self._context.get_scoped_config(),
-            region,
             self._response_parser_factory,
             tls_verification,
-            (connect_timeout, read_timeout),
+            timeout,
             self._retryhandler)
-        if AccessTokenAuth.is_access_token(credentials.access_token):
-            auth_method = AccessTokenAuth.AUTH_METHOD_NAME
-        elif Ed25519v1Auth.detect_private_key(credentials.private_key):
+        if Ed25519v1Auth.detect_private_key(credentials.private_key):
             auth_method = Ed25519v1Auth.AUTH_METHOD_NAME
-        elif ECDSAv1Auth.detect_private_key(credentials.private_key):
-            auth_method = ECDSAv1Auth.AUTH_METHOD_NAME
         else:
             auth_method = RSAv1Auth.AUTH_METHOD_NAME
         additional_headers = dict()
         request_headers_string = self._context.get_scoped_config().get(
             'request_headers', '')
         for header_string in request_headers_string.split(','):
             header_string = header_string.strip()
@@ -164,16 +139,15 @@
         return mapping
 
     def _create_api_method(self, py_operation_name, operation_name, service_model):
         def _api_call(self, *args, **kwargs):
             if args:
                 raise TypeError(
                     "%s() only accepts keyword arguments." % py_operation_name)
-            http, parsed_response = self.make_api_call(operation_name, kwargs)
-            return parsed_response
+            return self._make_api_call(operation_name, kwargs)
 
         _api_call.__name__ = str(py_operation_name)
         return _api_call
 
 
 class BaseClient(object):
 
@@ -213,60 +187,38 @@
         method = getattr(self, operation_name)
         return Paginator(method, operation_model)
 
     @property
     def _service_model(self):
         return self.meta.service_model
 
-    def make_api_call(self, operation_name, api_params,
-                      allow_redirects=True):
+    def _make_api_call(self, operation_name, api_params):
         operation_model = self._service_model.operation_model(operation_name)
-        request_dict = self._serializer.serialize_to_request(api_params, operation_model)
-        return self._make_request(operation_name, operation_model, request_dict,
-                                  allow_redirects)
-
-    def make_request(self, operation_name,
-                     method, url_path, headers, body,
-                     allow_redirects=True):
-        operation_model = self._service_model.operation_model(operation_name)
-        request_dict = {
-            'url_path': url_path,
-            'method': method,
-            'headers': headers,
-            'body': body
-        }
-        return self._make_request(operation_name, operation_model, request_dict,
-                                  allow_redirects)
-
-    def raise_error(self, operation_name, http, parsed_response):
-        request_id = http.headers.get(ALTUS_REQUEST_ID_HEADER) \
-            if ALTUS_REQUEST_ID_HEADER in http.headers \
-            else http.headers.get(CDP_REQUEST_ID_HEADER, 'Unknown')
-        raise ClientError(
-            parsed_response,
-            operation_name,
-            self._service_model.service_name,
-            http.status_code,
-            request_id)
+        request_dict = self._convert_to_request_dict(
+            api_params, operation_model)
+        http, parsed_response = self._endpoint.make_request(
+            operation_model, request_dict, self._request_signer)
+        if http.status_code >= 300:
+            raise ClientError(
+                parsed_response,
+                operation_name,
+                self._service_model.service_name,
+                http.status_code,
+                http.headers.get(CDP_REQUEST_ID_HEADER, 'Unknown'))
+        else:
+            return parsed_response
 
-    def _make_request(self, operation_name, operation_model, request_dict,
-                      allow_redirects):
+    def _convert_to_request_dict(self, api_params, operation_model):
+        request_dict = self._serializer.serialize_to_request(
+            api_params, operation_model)
         prepare_request_dict(request_dict,
                              endpoint_url=self._endpoint.host,
                              user_agent_header=self._user_agent_header,
                              additional_headers=self._additional_headers)
-        http, parsed_response = self._endpoint.make_request(
-            operation_model, request_dict, self._request_signer,
-            allow_redirects=allow_redirects)
-        if allow_redirects and http.status_code >= 300:
-            self.raise_error(operation_name, http, parsed_response)
-        elif not allow_redirects and http.status_code >= 400:
-            self.raise_error(operation_name, http, parsed_response)
-        else:
-            return http, parsed_response
+        return request_dict
 
 
 class ClientMeta(object):
 
     def __init__(self, service_model, endpoint_url, method_to_api_mapping):
         self._service_model = service_model
         self._endpoint_url = endpoint_url
@@ -322,28 +274,25 @@
         'ca_bundle': ('ca_bundle', 'CDP_CA_BUNDLE', None, None),
         'api_versions': ('api_versions', None, {}, None),
         # This is the legacy json configuration file
         'auth_config': (None, None, None, None),
         # This is the shared credentials file.
         'credentials_file': (None, 'CDP_SHARED_CREDENTIALS_FILE',
                              '~/.cdp/credentials', None),
-        'cdp_region': ('cdp_region', None, None, None),
-        'cdp_endpoint_url': ('cdp_endpoint_url', None, None, None),
-        'endpoint_url': ('endpoint_url', None, None, None),
-        'form_factor': ('form_factor', None, None, None),
     }
 
     def __init__(self, profile=None):
         self.context_var_map = copy.copy(self.CONTEXT_VARIABLES)
         # The _profile attribute is just used to cache the value
         # of the current profile to avoid going through the normal
         # config lookup process each access time.
         self._profile = None
         self._config = None
         self._profile_map = None
+        self._credentials = None
         # This is a dict that stores per context specific config variable
         # overrides via set_config_variable().
         self._context_instance_vars = {}
         if profile is not None:
             self._context_instance_vars['profile'] = profile
         self._client_config = None
 
@@ -524,14 +473,19 @@
             'myvalue'
             >>> s.set_config_variable('foo', 'othervalue')
             >>> s.get_config_variable('foo')
             'othervalue'
         """
         self._context_instance_vars[logical_name] = value
 
-    def get_credentials(self, parsed_globals=None):
+    def get_credentials(self):
         """
         Return the :class:`botocore.credential.Credential` object
-        associated with this session.
+        associated with this session.  If the credentials have not
+        yet been loaded, this will attempt to load them.  If they
+        have already been loaded, this will return the cached
+        credentials.
+
         """
-        resolver = credentials.create_credential_resolver(self, parsed_globals)
-        return resolver.load_credentials()
+        if self._credentials is None:
+            resolver = credentials.create_credential_resolver(self)
+            return resolver.load_credentials()
```

### Comparing `cdpcli-0.9.89/cdpcli/compat.py` & `cdpcli-0.9.9/cdpcli/compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,16 +90,14 @@
         # That way consumers can just call get_stdout_text_writer() and write
         # unicode to the returned stream.  Note that get_stdout_text_writer
         # just returns sys.stdout in the PY3 section above because python3
         # handles this.
         return codecs.getwriter(locale.getpreferredencoding())(sys.stdout)
 
     def ensure_unicode(s, encoding='utf-8', errors='strict'):
-        if s is None:
-            return None
         if isinstance(s, six.text_type):
             return s
         return unicode(s, encoding, errors)  # noqa
 
     def compat_open(filename, mode='r', encoding=None):
         # See docstring for compat_open in the PY3 section above.
         if 'b' not in mode:
```

### Comparing `cdpcli-0.9.89/cdpcli/completer.py` & `cdpcli-0.9.9/cdpcli/completer.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,22 +72,21 @@
         if current_arg != subcmd_name and current_arg.startswith('-'):
             return self._find_possible_options(current_arg, opts, subcmd_help)
         return []
 
     def _complete_option(self, option_name):
         if option_name == '--endpoint-url':
             return []
-        if option_name == '--profile':
+        if option_name == '--cdp-endpoint-url':
             return []
-        cli_data_options = getattr(self.driver, '_cli_data', {}).get('options', {})
-        enum_option_names = ['--' + name
-                             for name, option in cli_data_options.items()
-                             if 'choices' in option]
-        if option_name in enum_option_names:
-            return cli_data_options[option_name.lstrip('-')]['choices']
+        if option_name == '--output':
+            cli_data = self.driver.session.get_data('cli')
+            return cli_data['options']['output']['choices']
+        if option_name == '--profile':
+            return self.driver.session.available_profiles
         return []
 
     def _complete_provider(self, current_arg, opts):
         if current_arg.startswith('-'):
             return self._find_possible_options(current_arg, opts)
         elif current_arg == 'cdp':
             return self._get_documented_completions(
```

### Comparing `cdpcli-0.9.89/cdpcli/configloader.py` & `cdpcli-0.9.9/cdpcli/configloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 # http://aws.amazon.com/apache2.0/
 #
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
-import configparser
 import copy
 import os
 import shlex
 
 from cdpcli.exceptions import ConfigNotFound, ConfigParseError
+from six.moves import configparser
 
 
 def multi_file_load_config(*filenames):
     """Load and combine multiple INI configs with profiles.
 
     This function will take a list of filesnames and return
     a single dictionary that represents the merging of the loaded
```

### Comparing `cdpcli-0.9.89/cdpcli/credentials.py` & `cdpcli-0.9.9/cdpcli/credentials.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,55 +14,45 @@
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 from collections import namedtuple
 import logging
 import os
 
-from cdpcli import CDP_ACCESS_KEY_ID_KEY_NAME, \
-                   CDP_ACCESS_TOKEN_KEY_NAME, \
-                   CDP_PRIVATE_KEY_KEY_NAME
-from cdpcli.auth import AccessTokenAuth
+from cdpcli import CDP_ACCESS_KEY_ID_KEY_NAME, CDP_PRIVATE_KEY_KEY_NAME
 from cdpcli.auth import Ed25519v1Auth
 import cdpcli.compat
 from cdpcli.compat import json
 from cdpcli.configloader import raw_config_parse
 from cdpcli.exceptions import ConfigNotFound
 from cdpcli.exceptions import MalformedCredentialsError
 from cdpcli.exceptions import NoCredentialsError
 from cdpcli.exceptions import PartialCredentialsError
 from cdpcli.exceptions import UnknownCredentialError
 
 LOG = logging.getLogger('cdpcli.credentials')
 ReadOnlyCredentials = namedtuple('ReadOnlyCredentials',
-                                 ['access_key_id',
-                                  'private_key',
-                                  'access_token',
-                                  'method'])
+                                 ['access_key_id', 'private_key', 'method'])
 ACCESS_KEY_ID = 'access_key_id'
 PRIVATE_KEY = 'private_key'
-ACCESS_TOKEN = 'access_token'
 
 
-def create_credential_resolver(context, parsed_globals=None):
+def create_credential_resolver(context):
     """Create a default credential resolver.
 
     This creates a pre-configured credential resolver
     that includes the default lookup chain for
     credentials.
-
-    :param parsed_globals: CLI input parameters which might contain an access-token.
     """
     profile_name = context.effective_profile
     auth_file = context.get_config_variable('auth_config')
     shared_credential_file = context.get_config_variable('credentials_file')
 
     env_provider = EnvProvider()
     providers = [
-        ParamsProvider(parsed_globals),
         env_provider,
         AuthConfigFile(auth_file),
         SharedCredentialProvider(
             creds_filename=shared_credential_file,
             profile_name=profile_name
         ),
     ]
@@ -89,44 +79,37 @@
         LOG.debug('Skipping environment variable credential check because '
                   'profile name was explicitly set.')
 
     resolver = CredentialResolver(providers=providers)
     return resolver
 
 
-def get_credentials(context, parsed_globals=None):
-    resolver = create_credential_resolver(context, parsed_globals)
+def get_credentials(context):
+    resolver = create_credential_resolver(context)
     return resolver.load_credentials()
 
 
 class Credentials(object):
     """
     Holds the credentials needed to authenticate requests.
     """
 
-    def __init__(self,
-                 access_key_id=None,
-                 private_key=None,
-                 access_token=None,
-                 method=None):
+    def __init__(self, access_key_id, private_key, method):
         self.access_key_id = access_key_id
         self.private_key = private_key
-        self.access_token = access_token
         self.method = method
         self._normalize()
 
     def _normalize(self):
         self.access_key_id = cdpcli.compat.ensure_unicode(self.access_key_id)
         self.private_key = cdpcli.compat.ensure_unicode(self.private_key)
-        self.access_token = cdpcli.compat.ensure_unicode(self.access_token)
 
     def get_frozen_credentials(self):
         return ReadOnlyCredentials(self.access_key_id,
                                    self.private_key,
-                                   self.access_token,
                                    self.method)
 
 
 class CredentialProvider(object):
 
     # Implementations must provide a method.
     METHOD = None
@@ -138,25 +121,21 @@
         found = []
         for key_name in key_names:
             try:
                 found.append(mapping[key_name])
             except KeyError:
                 raise PartialCredentialsError(provider=self.METHOD,
                                               cred_var=key_name)
-        if len(found) == 1:  # found access-token, returns a single-value string.
-            return found[0]
-        else:  # found access-key-id and private-key, returns a tuple.
-            return found
+        return found
 
 
 class EnvProvider(CredentialProvider):
     METHOD = 'env'
     ACCESS_KEY_ID_ENV_VAR = 'CDP_ACCESS_KEY_ID'
     PRIVATE_KEY_ENV_VAR = 'CDP_PRIVATE_KEY'
-    ACCESS_TOKEN_ENV_VAR = 'CDP_ACCESS_TOKEN'
 
     def __init__(self, environ=None, mapping=None):
         super(EnvProvider, self).__init__()
         if environ is None:
             environ = os.environ
         self.environ = environ
         self._mapping = self._build_mapping(mapping)
@@ -164,22 +143,19 @@
     def _build_mapping(self, mapping):
         # Mapping of variable name to env var name.
         var_mapping = {}
         if mapping is None:
             # Use the class var default.
             var_mapping[ACCESS_KEY_ID] = self.ACCESS_KEY_ID_ENV_VAR
             var_mapping[PRIVATE_KEY] = self.PRIVATE_KEY_ENV_VAR
-            var_mapping[ACCESS_TOKEN] = self.ACCESS_TOKEN_ENV_VAR
         else:
             var_mapping[ACCESS_KEY_ID] = mapping.get(
                 ACCESS_KEY_ID, self.ACCESS_KEY_ID_ENV_VAR)
             var_mapping[PRIVATE_KEY] = mapping.get(
                 PRIVATE_KEY, self.PRIVATE_KEY_ENV_VAR)
-            var_mapping[ACCESS_TOKEN] = mapping.get(
-                ACCESS_TOKEN, self.ACCESS_TOKEN_ENV_VAR)
         return var_mapping
 
     def load(self):
         """
         Search for credentials in explicit environment variables.
         """
         if self._mapping[ACCESS_KEY_ID] in self.environ:
@@ -191,30 +167,19 @@
             # For compatibility, assume the PRIVATE_KEY is a path to a file
             # containing the key. Only if there is no file, should the value
             # be checked to see if it's an actual key.
             if not os.path.isfile(private_key):
                 if Ed25519v1Auth.detect_private_key(private_key):
                     private_key_value = private_key
                 else:
-                    raise NoCredentialsError(
-                        err_msg='Private key file {} does not exist'.format(private_key))
+                    LOG.debug("Private key at %s does not exist!" % private_key)
+                    raise NoCredentialsError()
             else:
                 private_key_value = open(private_key).read()
-            return Credentials(access_key_id=access_key_id,
-                               private_key=private_key_value,
-                               method=self.METHOD)
-        elif self._mapping[ACCESS_TOKEN] in self.environ:
-            access_token = self._extract_creds_from_mapping(
-                self.environ, self._mapping[ACCESS_TOKEN])
-            LOG.info('Found access token in environment variables.')
-            if not AccessTokenAuth.is_access_token(access_token):
-                LOG.debug('Invalid access token {}'.format(access_token))
-                raise NoCredentialsError(
-                    err_msg='Invalid access token (see debug log for value)')
-            return Credentials(access_token=access_token,
+            return Credentials(access_key_id, private_key_value,
                                method=self.METHOD)
         else:
             return None
 
 
 class CredentialResolver(object):
 
@@ -265,33 +230,22 @@
             raise UnknownCredentialError(name=name)
 
     def load_credentials(self):
         """
         Goes through the credentials chain, returning the first ``Credentials``
         that could be loaded.
         """
-
-        # Grab this during the scan in case no credentials are available.
-        creds_expanded_path = None
-
         # First provider to return a non-None response wins.
         for provider in self.providers:
             LOG.debug("Looking for credentials via: %s", provider.METHOD)
-            if isinstance(provider, SharedCredentialProvider):
-                creds_expanded_path = provider.get_creds_expanded_path()
             creds = provider.load()
             if creds is not None:
                 return creds
 
-        err_msg = "No credentials found anywhere in chain"
-        if creds_expanded_path:
-            err_msg += ". The shared credentials file should be stored at {}"\
-                .format(creds_expanded_path)
-
-        raise NoCredentialsError(err_msg=err_msg)
+        raise NoCredentialsError()
 
 
 class AuthConfigFile(CredentialProvider):
     METHOD = 'auth_config_file'
 
     def __init__(self, conf):
         super(AuthConfigFile, self).__init__()
@@ -301,102 +255,56 @@
         """
         load the credential from the json configuration file.
         """
         if self._conf is None:
             return None
 
         if not os.path.isfile(self._conf):
-            raise NoCredentialsError(
-                err_msg="Config file {} not found".format(self._conf))
+            LOG.debug("Conf file at %s does not exist!" % self._conf)
+            raise NoCredentialsError()
         try:
             conf = json.loads(open(self._conf).read())
         except Exception:
             LOG.debug("Could not read conf: %s", exc_info=True)
             return None
 
-        if ACCESS_KEY_ID in conf or PRIVATE_KEY in conf:
-            LOG.debug('Found credentials for key: %s in configuration file.',
-                      conf[ACCESS_KEY_ID])
-            access_key_id, private_key = self._extract_creds_from_mapping(
-                conf,
-                ACCESS_KEY_ID,
-                PRIVATE_KEY)
-            return Credentials(access_key_id=access_key_id,
-                               private_key=private_key,
-                               method=self.METHOD)
-        elif ACCESS_TOKEN in conf:
-            LOG.debug('Found access-token in configuration file.')
-            access_token = self._extract_creds_from_mapping(conf, ACCESS_TOKEN)
-            return Credentials(access_token=access_token,
-                               method=self.METHOD)
-        else:
-            cred_vars = '%s or %s' % (ACCESS_KEY_ID, ACCESS_TOKEN)
+        if ACCESS_KEY_ID not in conf:
             LOG.debug('Auth config file is missing required key %s',
-                      cred_vars)
+                      ACCESS_KEY_ID)
             raise MalformedCredentialsError(provider=self.METHOD,
-                                            cred_var=cred_vars)
+                                            cred_var=ACCESS_KEY_ID)
+
+        LOG.debug('Found credentials for key: %s in configuration file.',
+                  conf[ACCESS_KEY_ID])
+        access_key_id, private_key = self._extract_creds_from_mapping(
+            conf,
+            ACCESS_KEY_ID,
+            PRIVATE_KEY)
+        return Credentials(access_key_id, private_key, self.METHOD)
 
 
 class SharedCredentialProvider(CredentialProvider):
     METHOD = 'shared-credentials-file'
 
     def __init__(self, creds_filename, profile_name):
         self._creds_filename = creds_filename
-        self._creds_expanded_path = os.path.expanduser(creds_filename)
         self._profile_name = profile_name
 
-    def get_creds_expanded_path(self):
-        return self._creds_expanded_path
-
     def load(self):
         try:
             available_creds = raw_config_parse(self._creds_filename)
         except ConfigNotFound:
-            LOG.debug("Shared credentials file {} not found".format(self._creds_filename))
+            LOG.debug("Credentials file at %s does not exist!" % self._creds_filename)
             return None
         if self._profile_name in available_creds:
             config = available_creds[self._profile_name]
-
-            if CDP_ACCESS_KEY_ID_KEY_NAME in config or \
-                    CDP_PRIVATE_KEY_KEY_NAME in config:
-                access_key_id, private_key = self._extract_creds_from_mapping(
-                    config, CDP_ACCESS_KEY_ID_KEY_NAME, CDP_PRIVATE_KEY_KEY_NAME)
-                # We store the private key in the credentials file as a one-line
-                # value in which the newlines in the PEM file are replaced with
-                # '\n'. We need to replace them back as the RawConfigParser we use
-                # does not do it for us. Note that if the value in the configuration
-                # IS a PEM formatted value this is a no-op.
-                private_key = private_key.replace('\\n', '\n')
-                LOG.info("Found credentials in shared credentials file: %s",
-                         self._creds_filename)
-                return Credentials(access_key_id=access_key_id,
-                                   private_key=private_key,
-                                   method=self.METHOD)
-            elif CDP_ACCESS_TOKEN_KEY_NAME in config:
-                access_token = self._extract_creds_from_mapping(
-                    config, CDP_ACCESS_TOKEN_KEY_NAME)
-                LOG.info("Found access-token in shared credentials file: %s",
-                         self._creds_filename)
-                return Credentials(access_token=access_token,
-                                   method=self.METHOD)
-            else:
-                return None
-
-
-class ParamsProvider(CredentialProvider):
-    """
-    Support for access-token parameter only.
-    """
-
-    METHOD = 'params'
-
-    def __init__(self, params):
-        if params is None:
-            self._access_token = None
-        else:
-            self._access_token = getattr(params, 'access_token', None)
-
-    def load(self):
-        if bool(self._access_token):
-            return Credentials(access_token=self._access_token,
-                               method=self.METHOD)
-        return None
+            access_key_id, private_key = self._extract_creds_from_mapping(
+                config, CDP_ACCESS_KEY_ID_KEY_NAME, CDP_PRIVATE_KEY_KEY_NAME)
+            # We store the private key in the credentials file as a one-line
+            # value in which the newlines in the PEM file are replaced with
+            # '\n'. We need to replace them back as the RawConfigParser we use
+            # does not do it for us. Note that if the value in the configuration
+            # IS a PEM formatted value this is a no-op.
+            private_key = private_key.replace('\\n', '\n')
+            LOG.info("Found credentials in shared credentials file: %s",
+                     self._creds_filename)
+            return Credentials(access_key_id, private_key, method=self.METHOD)
```

### Comparing `cdpcli-0.9.89/cdpcli/data/_retry.json` & `cdpcli-0.9.9/cdpcli/data/_retry.json`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.89/cdpcli/data/datalake/datalake.yaml` & `cdpcli-0.9.9/cdpcli/data/iam/iam.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,870 +1,1160 @@
 swagger: '2.0'
-x-endpoint-name: datalake
-x-interface-model: cdp
-x-products: CDP
-x-form-factors: public
+x-endpoint-name: iam
+x-products: ALTUS,CDP
+x-altus-releases: PUBLIC
 x-cdp-releases: PUBLIC
-x-audit: true
 info:
-  version: 0.9.89
-  title: Cloudera Datalake Service
+  version: 0.1-SNAPSHOT
+  title: Cloudera IAM Service
   license:
     name: Apache 2.0
-  description: Cloudera data lake is a service for launching and managing data lake clusters powered by Cloudera Runtime.
-  termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
+  description: Cloudera Altus IAM is a web service that you can use to manage users and user permissions under your Altus account.
 schemes:
   - https
 consumes:
   - application/json
 produces:
   - application/json
 paths:
-  /api/v1/datalake/listRuntimes:
+  /iam/getUser:
     post:
-      summary: Lists the datalake versions.
-      description: Lists the available datalake runtime versions.
-      operationId: listRuntimes
-      x-mutating: false
+      summary: Gets information on a user.
+      description: Gets information on a user. If no user name is specified. The user name is determined from the access key used to make the request.
+      operationId: getUser
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/ListRuntimesRequest'
+            $ref: '#/definitions/GetUserRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ListRuntimesResponse'
+            $ref: '#/definitions/GetUserResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/createAWSDatalake:
+  /iam/listUsers:
     post:
-      summary: Creates an AWS datalake.
-      description: Creates an AWS datalake.
-      operationId: createAWSDatalake
-      x-mutating: true
+      summary: Lists users.
+      description: Lists users.
+      operationId: listUsers
+      x-right: iam/listUsers
+      x-paginates: true
+      x-paging-default-max-items: 100
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/CreateAWSDatalakeRequest'
+            $ref: '#/definitions/ListUsersRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/CreateAWSDatalakeResponse'
+            $ref: '#/definitions/ListUsersResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/createAzureDatalake:
+  /iam/createUser:
     post:
-      summary: Creates an Azure datalake.
-      description: Creates an Azure datalake.
-      operationId: createAzureDatalake
-      x-mutating: true
+      summary: Creates a user in Altus.
+      description: Creates a user in Altus.
+      operationId: createUser
+      x-right: iam/createUser
+      x-no-compatibility-guarantee: true
+      x-entitlement: IDENTITY_FEDERATION
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/CreateAzureDatalakeRequest'
+            $ref: '#/definitions/CreateUserRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/CreateAzureDatalakeResponse'
+            $ref: '#/definitions/CreateUserResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/createGCPDatalake:
+  /iam/createUserAccessKey:
     post:
-      summary: Creates an GCP Data Lake.
-      description: Creates an GCP Data Lake.
-      operationId: createGCPDatalake
-      x-mutating: true
+      summary: Creates a new access key for a user.
+      description: Creates a new access key for a user.
+      operationId: createUserAccessKey
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/CreateGCPDatalakeRequest'
+            $ref: '#/definitions/CreateUserAccessKeyRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/CreateGCPDatalakeResponse'
+            $ref: '#/definitions/CreateUserAccessKeyResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/listDatalakes:
+  /iam/createMachineUserAccessKey:
     post:
-      summary: Lists datalakes.
-      description: Lists datalakes.
-      operationId: listDatalakes
-      x-mutating: false
+      summary: Creates a new access key for a machine user.
+      description: Creates a new access key for a machine user.
+      operationId: createMachineUserAccessKey
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/ListDatalakesRequest'
+            $ref: '#/definitions/CreateMachineUserAccessKeyRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ListDatalakesResponse'
+            $ref: '#/definitions/CreateMachineUserAccessKeyResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/deleteDatalake:
+  /iam/deleteAccessKey:
     post:
-      summary: Deletes a datalake.
-      description: Deletes a datalake.
-      operationId: deleteDatalake
-      x-mutating: true
+      summary: Deletes an access key.
+      description: Deletes an access key.
+      operationId: deleteAccessKey
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/DeleteDatalakeRequest'
+            $ref: '#/definitions/DeleteAccessKeyRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/DeleteDatalakeResponse'
+            $ref: '#/definitions/DeleteAccessKeyResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/retryDatalake:
+  /iam/updateAccessKey:
     post:
-      summary: Retry last failed operation on a datalake.
-      description: Retry last failed operation on a datalake.
-      operationId: retryDatalake
-      x-mutating: true
+      summary: Updates an access key.
+      description: Updates an access key.
+      operationId: updateAccessKey
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/RetryDatalakeRequest'
+            $ref: '#/definitions/UpdateAccessKeyRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/RetryDatalakeResponse'
+            $ref: '#/definitions/UpdateAccessKeyResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/startDatalakeVerticalScaling:
+  /iam/getAccessKey:
     post:
-      summary: Initiates the vertical scaling on Data Lake.
-      description: Initiates the vertical scaling on Data Lake.
-      operationId: startDatalakeVerticalScaling
-      x-mutating: true
+      summary: Gets information on an access key.
+      description: Gets information on an access key. If no access key ID is specified. Information on the access key used to make the request is returned.
+      operationId: getAccessKey
+      x-right: iam/getAccessKey
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/StartDatalakeVerticalScalingRequest'
+            $ref: '#/definitions/GetAccessKeyRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/StartDatalakeVerticalScalingResponse'
+            $ref: '#/definitions/GetAccessKeyResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/describeDatalake:
+  /iam/listAccessKeys:
     post:
-      summary: Describes a datalake.
-      description: Describes a datalake.
-      operationId: describeDatalake
-      x-mutating: false
+      summary: Lists access keys.
+      description: Lists access keys.
+      operationId: listAccessKeys
+      x-right: iam/listAccessKeys
+      x-paginates: true
+      x-paging-default-max-items: 100
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/DescribeDatalakeRequest'
+            $ref: '#/definitions/ListAccessKeysRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/DescribeDatalakeResponse'
+            $ref: '#/definitions/ListAccessKeysResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/renewCertificate:
+  /iam/listRoles:
     post:
-      summary: Renew certificate on Datalake cluster by name or CRN
-      description: Deprecated, please use renew-public-certificate command instead. Renew certificate on Datalake cluster by name or CRN.
-      operationId: renewCertificate
-      x-deprecated: true
-      x-mutating: true
+      summary: Lists all the available roles.
+      description: Lists all the available roles. Roles grant rights to users via policies that are attached to the roles.
+      operationId: listRoles
+      x-right: iam/listRoles
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/RenewCertificateRequest'
+            $ref: '#/definitions/ListRolesRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/RenewCertificateResponse'
+            $ref: '#/definitions/ListRolesResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/renewPublicCertificate:
+  /iam/listResourceRoles:
     post:
-      summary: Renews public certificate on Datalake cluster by name or CRN.
-      description: Renews public certificate on Datalake cluster by name or CRN.
-      operationId: renewPublicCertificate
-      x-mutating: true
+      summary: Lists all the available resource roles.
+      description: Lists all the available reource roles. Resource roles grants rights over certain resources.
+      operationId: listResourceRoles
+      x-right: iam/listResourceRoles
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/RenewPublicCertificateRequest'
+            $ref: '#/definitions/ListResourceRolesRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/RenewPublicCertificateResponse'
+            $ref: '#/definitions/ListResourceRolesResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/repairDatalake:
+  /iam/assignUserRole:
     post:
-      summary: Repairs a datalake.
-      description: Repairs a datalake.
-      operationId: repairDatalake
-      x-mutating: true
+      summary: Assign a role to a user.
+      description: Assign a role to a user. If the role is already assigned to the user the request will fail.
+      operationId: assignUserRole
+      x-right: iam/assignRole
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/RepairDatalakeRequest'
+            $ref: '#/definitions/AssignUserRoleRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/RepairDatalakeResponse'
+            $ref: '#/definitions/AssignUserRoleResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/getClusterServiceStatus:
+  /iam/unassignUserRole:
     post:
-      summary: Get cluster service status.
-      description: Gets the status of the services in a cluster.
-      operationId: getClusterServiceStatus
-      x-mutating: false
+      summary: Unassign a role from a user.
+      description: Unassign a role from a user. If the role is not currently assigned to the user the request will fail.
+      operationId: unassignUserRole
+      x-right: iam/unassignRole
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/GetClusterServiceStatusRequest'
+            $ref: '#/definitions/UnassignUserRoleRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/GetClusterServiceStatusResponse'
+            $ref: '#/definitions/UnassignUserRoleResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/getClusterHostStatus:
+  /iam/assignUserResourceRole:
     post:
-      summary: Get cluster host status.
-      description: Gets the status of the hosts in a cluster.
-      operationId: getClusterHostStatus
-      x-mutating: false
+      summary: Assign a resource role to a user.
+      description: Assign a resource role to a user. If the resource role is already assigned to the user the request will fail.
+      operationId: assignUserResourceRole
+      x-right: iam/assignResourceRole
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/GetClusterHostStatusRequest'
+            $ref: '#/definitions/AssignUserResourceRoleRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/GetClusterHostStatusResponse'
+            $ref: '#/definitions/AssignUserResourceRoleResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/upgradeDatalake:
+  /iam/unassignUserResourceRole:
     post:
-      summary: OS or data platform upgrade for the SDX cluster.
-      description: OS or data platform upgrade for the SDX cluster. You have the option to either specify one of 'imageId', 'runtime' or 'lockComponents' or both 'imageId' and 'lockComponents' or none of the parameters.
-      operationId: upgradeDatalake
-      x-mutating: true
+      summary: Unassign a resource role from a user.
+      description: Unassign a resource role from a user. If the resource role is not currently assigned to the user the request will fail.
+      operationId: unassignUserResourceRole
+      x-right: iam/unassignResourceRole
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/UpgradeDatalakeRequest'
+            $ref: '#/definitions/UnassignUserResourceRoleRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/UpgradeDatalakeResponse'
+            $ref: '#/definitions/UnassignUserResourceRoleResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/prepareDatalakeUpgrade:
+  /iam/listUserAssignedRoles:
     post:
-      summary: Prepares the Data Lake cluster for upgrade.
-      description: In order to reduce the chance of upgrade failures, we're introducing a preparation phase for runtime upgrades. During this phase, we're running all validations and downloading the required parcels for the machines. You can track the progress of the parcel preparation on the Cloudera Manager UI or you can check on the Management Console as well.
-      operationId: prepareDatalakeUpgrade
-      x-mutating: true
+      summary: Lists the user's assigned roles.
+      description: Lists the user's assigned roles.
+      operationId: listUserAssignedRoles
+      x-right: iam/listAssignedRoles
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/PrepareDatalakeUpgradeRequest'
+            $ref: '#/definitions/ListUserAssignedRolesRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/PrepareDatalakeUpgradeResponse'
+            $ref: '#/definitions/ListUserAssignedRolesResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/startDatabaseUpgrade:
+  /iam/listUserAssignedResourceRoles:
     post:
-      summary: Upgrades the database of the Data Lake cluster.
-      description: This command initiates the upgrade of the database of the Data Lake cluster.
-      operationId: startDatabaseUpgrade
-      x-mutating: true
+      summary: Lists a user's assigned resource roles.
+      description: Lists a user's assigned resource roles.
+      operationId: listUserAssignedResourceRoles
+      x-right: iam/listAssignedResourceRoles
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/StartDatabaseUpgradeRequest'
+            $ref: '#/definitions/ListUserAssignedResourceRolesRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/StartDatabaseUpgradeResponse'
+            $ref: '#/definitions/ListUserAssignedResourceRolesResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/startDatalake:
+  /iam/assignMachineUserRole:
     post:
-      summary: Start Datalake
-      description: Deprecated, please use 'cdp environments start-environment' instead.
-      operationId: startDatalake
-      x-mutating: true
-      x-deprecated: true
+      summary: Assign a role to a machine user.
+      description: Assign a role to a machine user. If the role is already assigned to the machine user the request will fail.
+      operationId: assignMachineUserRole
+      x-right: iam/assignRole
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/StartDatalakeRequest'
+            $ref: '#/definitions/AssignMachineUserRoleRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/StartDatalakeResponse'
+            $ref: '#/definitions/AssignMachineUserRoleResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/stopDatalake:
+  /iam/unassignMachineUserRole:
     post:
-      summary: Stop Datalake
-      description: Deprecated, please use 'cdp environments stop-environment' instead.
-      operationId: stopDatalake
-      x-mutating: true
-      x-deprecated: true
+      summary: Unassign a role from a machine user.
+      description: Unassign a role from a machine user. If the role is not currently assigned to the machine user the request will fail.
+      operationId: unassignMachineUserRole
+      x-right: iam/unassignRole
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/StopDatalakeRequest'
+            $ref: '#/definitions/UnassignMachineUserRoleRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/StopDatalakeResponse'
+            $ref: '#/definitions/UnassignMachineUserRoleResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/backupDatalake:
+  /iam/assignMachineUserResourceRole:
     post:
-      summary: Create backup of datalake.
-      description: Takes a backup of all the data in the datalake.
-      operationId: backupDatalake
-      x-mutating: true
+      summary: Assign a resource role to a machine user.
+      description: Assign a resource role to a machine user. If the resource role is already assigned to the machine user the request will fail.
+      operationId: assignMachineUserResourceRole
+      x-right: iam/assignResourceRole
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/BackupDatalakeRequest'
+            $ref: '#/definitions/AssignMachineUserResourceRoleRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/BackupDatalakeResponse'
+            $ref: '#/definitions/AssignMachineUserResourceRoleResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/backupDatalakeStatus:
+  /iam/unassignMachineUserResourceRole:
     post:
-      summary: Check the status of a datalake backup operation performed.
-      description: Identifies the backup operation based on the inputs provided and gets the status. BackupName and BackupId are mutually exclusive. Only one of them can be provided.
-      operationId: backupDatalakeStatus
-      x-mutating: true
+      summary: Unassign a resource role from a machine user.
+      description: Unassign a resource role from a machine user. If the resource role is not currently assigned to the machine user the request will fail.
+      operationId: unassignMachineUserResourceRole
+      x-right: iam/unassignResourceRole
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/BackupDatalakeStatusRequest'
+            $ref: '#/definitions/UnassignMachineUserResourceRoleRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/BackupDatalakeStatusResponse'
+            $ref: '#/definitions/UnassignMachineUserResourceRoleResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/restoreDatalake:
+  /iam/listMachineUserAssignedRoles:
     post:
-      summary: Restore the datalake from backup taken.
-      description: Restore the datalake from a backup that was taken. Backup to be used for restore is identified based on the information provided in the restore request. BackupId and BackupName are mutually exclusive. Only one of them can be provided. If both are provided, BackupId takes precedence.
-      operationId: restoreDatalake
-      x-mutating: true
+      summary: Lists the machine user's assigned roles.
+      description: Lists the machine user's assigned roles.
+      operationId: listMachineUserAssignedRoles
+      x-right: iam/listAssignedRoles
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/RestoreDatalakeRequest'
+            $ref: '#/definitions/ListMachineUserAssignedRolesRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/RestoreDatalakeResponse'
+            $ref: '#/definitions/ListMachineUserAssignedRolesResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/restoreDatalakeStatus:
+  /iam/listMachineUserAssignedResourceRoles:
     post:
-      summary: Check the status of datalake restore operation.
-      description: Identifies the restore operation based on the inputs provided and gets the status. RestoreId and BackupName are mutually exclusive. Only one of them can be provided.
-      operationId: restoreDatalakeStatus
-      x-mutating: true
+      summary: Lists a machine user's assigned resource roles.
+      description: Lists a machine user's assigned resource roles.
+      operationId: listMachineUserAssignedResourceRoles
+      x-right: iam/listAssignedResourceRoles
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/RestoreDatalakeStatusRequest'
+            $ref: '#/definitions/ListMachineUserAssignedResourceRolesRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/RestoreDatalakeStatusResponse'
+            $ref: '#/definitions/ListMachineUserAssignedResourceRolesResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/listDatalakeBackups:
+  /iam/listResourceAssignees:
     post:
-      summary: List all the backup operations that were performed on the datalake.
-      description: List all the backup operations that were performed on the datalake.
-      operationId: listDatalakeBackups
-      x-mutating: false
+      summary: List the resource assignees and their respective resource roles for the resource.
+      description: List the resource assignees and their respective resource roles for the resource.
+      operationId: listResourceAssignees
+      x-right: iam/listResourceAssignees
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/ListDatalakeBackupsRequest'
+            $ref: '#/definitions/ListResourceAssigneesRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ListDatalakeBackupsResponse'
+            $ref: '#/definitions/ListResourceAssigneesResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/cancelBackup:
+  /iam/createMachineUser:
     post:
-      summary: Cancels the specified ongoing backup operation.
-      description: Cancels a currently running backup operation. The operation must be in a STARTED or IN_PROGRESS state. Pending sub-operations will be ignored and marked as cancelled. The operation does not wait for the currently running sub-operation(s) to complete.
-      operationId: cancelBackup
-      x-mutating: true
+      summary: Create a machine user.
+      description: Creates a machine user in the account. A machine user can be used to access Altus API. A machine user can have access keys associated with it and can be assigned roles and resource roles. A machine user cannot login to the Altus console.
+      operationId: createMachineUser
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/CancelBackupRequest'
+            $ref: '#/definitions/CreateMachineUserRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/CancelBackupResponse'
+            $ref: '#/definitions/CreateMachineUserResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/replaceRecipes:
+  /iam/listMachineUsers:
     post:
-      summary: Replaces recipes for the given instance groups.
-      description: Replaces recipes for the given instance groups.
-      operationId: replaceRecipes
-      x-mutating: true
+      summary: Lists machine users.
+      description: Lists machine users in the account.
+      operationId: listMachineUsers
+      x-right: iam/listMachineUsers
+      x-paginates: true
+      x-paging-default-max-items: 100
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/ReplaceRecipesRequest'
+            $ref: '#/definitions/ListMachineUsersRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ReplaceRecipesResponse'
+            $ref: '#/definitions/ListMachineUsersResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/getDatalakeLogDescriptors:
+  /iam/deleteMachineUser:
     post:
-      summary: Gather log descriptors that are used for diagnostics collection.
-      description: Gather log descriptors that are used for diagnostics collection.
-      operationId: getDatalakeLogDescriptors
-      x-mutating: false
+      summary: Delete a machine user.
+      description: Deletes a machine user previously created in the account.
+      operationId: deleteMachineUser
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/GetDatalakeLogDescriptorsRequest'
+            $ref: '#/definitions/DeleteMachineUserRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/GetDatalakeLogDescriptorsResponse'
+            $ref: '#/definitions/DeleteMachineUserResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/collectDatalakeDiagnostics:
+  /iam/createSamlProvider:
     post:
-      summary: Start DataLake diagnostics collection
-      description: Start Datalake diagnostics collection
-      operationId: collectDatalakeDiagnostics
-      x-mutating: false
+      summary: Creates a SAML provider in Altus.
+      description: Creates a SAML provider in Altus.
+      operationId: createSamlProvider
+      x-right: iam/createSamlProvider
+      x-no-compatibility-guarantee: true
+      x-entitlement: IDENTITY_FEDERATION
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/CollectDatalakeDiagnosticsRequest'
+            $ref: '#/definitions/CreateSamlProviderRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/CollectDatalakeDiagnosticsResponse'
+            $ref: '#/definitions/CreateSamlProviderResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/listDatalakeDiagnostics:
+  /iam/deleteSamlProvider:
     post:
-      summary: List recent Datalake diagnostics collections
-      description: List recent Datalake diagnostics collection
-      operationId: listDatalakeDiagnostics
-      x-mutating: false
+      summary: Deletes a SAML provider in Altus account.
+      description: Deletes a SAML provider in Altus account.
+      operationId: deleteSamlProvider
+      x-right: iam/deleteSamlProvider
+      x-no-compatibility-guarantee: true
+      x-entitlement: IDENTITY_FEDERATION
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/ListDatalakeDiagnosticsRequest'
+            $ref: '#/definitions/DeleteSamlProviderRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ListDatalakeDiagnosticsResponse'
+            $ref: '#/definitions/DeleteSamlProviderResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/cancelDatalakeDiagnostics:
+  /iam/listSamlProviders:
     post:
-      summary: Cancel running Datalake diagnostics collections
-      description: Cancel running Datalake diagnostics collection
-      operationId: cancelDatalakeDiagnostics
-      x-mutating: false
+      summary: Lists SAML providers in Altus account.
+      description: Lists SAML providers in Altus account.
+      operationId: listSamlProviders
+      x-no-compatibility-guarantee: true
+      x-entitlement: IDENTITY_FEDERATION
+      x-right: iam/listSamlProviders
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/CancelDatalakeDiagnosticsRequest'
+            $ref: '#/definitions/ListSamlProvidersRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/CancelDatalakeDiagnosticsResponse'
+            $ref: '#/definitions/ListSamlProvidersResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/collectCmDiagnostics:
+  /iam/updateSamlProvider:
     post:
-      summary: Start DataLake Cloudera Manager based diagnostics collection
-      description: Start Datalake Cloudera Manager based diagnostics collection
-      operationId: collectCmDiagnostics
-      x-mutating: false
+      summary: Updates a SAML provider in Altus.
+      description: Updates a SAML provider in Altus.
+      operationId: updateSamlProvider
+      x-right: iam/updateSamlProvider
+      x-no-compatibility-guarantee: true
+      x-entitlement: IDENTITY_FEDERATION
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/CollectCmDiagnosticsRequest'
+            $ref: '#/definitions/UpdateSamlProviderRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/CollectCmDiagnosticsResponse'
+            $ref: '#/definitions/UpdateSamlProviderResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/getCmRoles:
+  /iam/enableClouderaSSOLogin:
     post:
-      summary: Gather Cloudera Manager roles that can be used for filtering in CM based diagnostics collection.
-      description: Gather Cloudera Manager roles that can be used for filtering in CM based diagnostics collection.
-      operationId: getCmRoles
-      x-mutating: false
+      summary: Enables interactive login using Cloudera SSO for this account.
+      description: Enables interactive login using Cloudera SSO for this account. This is a no-op if login using Cloudera SSO are already enabled.
+      operationId: enableClouderaSSOLogin
+      x-right: iam/manageClouderaSSOLogin
+      x-no-compatibility-guarantee: true
+      x-entitlement: IDENTITY_FEDERATION
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/GetCmRolesRequest'
+            $ref: '#/definitions/EnableClouderaSSOLoginRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/GetCmRolesResponse'
+            $ref: '#/definitions/EnableClouderaSSOLoginResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/rotateAutoTlsCertificates:
+  /iam/disableClouderaSSOLogin:
     post:
-      summary: Rotate autotls certificates on the datalake's hosts
-      description: Deprecated, please use rotate-private-certificates command instead. Rotate autotls certificates on the datalake's hosts
-      operationId: rotateAutoTlsCertificates
-      x-mutating: true
-      x-deprecated: true
+      summary: Disables interactive login using Cloudera SSO for this account.
+      description: Disables interactive login using Cloudera SSO for this account. When disabled, only users who are designated account administrators will be able to use Cloudera SSO to interactively login to the Altus account. All other users will only be able to interactively login using SAML providers defined for the account. This is a no-op if login using Cloudera SSO are already disabled.
+      operationId: disableClouderaSSOLogin
+      x-right: iam/manageClouderaSSOLogin
+      x-no-compatibility-guarantee: true
+      x-entitlement: IDENTITY_FEDERATION
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/RotateAutoTlsCertificatesRequest'
+            $ref: '#/definitions/DisableClouderaSSOLoginRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/RotateAutoTlsCertificatesResponse'
+            $ref: '#/definitions/DisableClouderaSSOLoginResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/rotatePrivateCertificates:
+  /iam/getAccount:
     post:
-      summary: Rotates private certificates on the datalake's hosts.
-      description: Rotates private certificates on the datalake's hosts.
-      operationId: rotatePrivateCertificates
-      x-mutating: true
+      summary: Retrieves information about the Altus account.
+      description: Retrieves information about the Altus account.
+      operationId: getAccount
+      x-entitlement: IDENTITY_FEDERATION
+      x-right: iam/getAccount
+      x-no-compatibility-guarantee: true
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/RotatePrivateCertificatesRequest'
+            $ref: '#/definitions/GetAccountRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/RotatePrivateCertificatesResponse'
+            $ref: '#/definitions/GetAccountResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/resizeDatalake:
+  /iam/createGroup:
     post:
-      summary: Resizes the given datalake to the given target size. Currently, the only valid use of this is for resizing a light duty datalake to a medium duty datalake.
-      description: Resizes the datalake to the given size.
-      operationId: resizeDatalake
-      x-mutating: true
+      summary: Create a group.
+      description: Create a group. A group is a named collection of users and machine users. Roles and resource roles can be assigned to a group impacting all members of the group.
+      operationId: createGroup
+      x-right: iam/createGroup
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/ResizeDatalakeRequest'
+            $ref: '#/definitions/CreateGroupRequest'
       responses:
         200:
-          description: Expected response to a valid resize datalake request.
+          description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ResizeDatalakeResponse'
+            $ref: '#/definitions/CreateGroupResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/recoverDatalake:
+  /iam/deleteGroup:
     post:
-      summary: Recover data lake to the original version after a failed upgrade.
-      description: Recover data lake to the original version after a failed upgrade.
-      operationId: recoverDatalake
-      x-mutating: true
+      summary: Delete a group.
+      description: Delete a group.
+      operationId: deleteGroup
+      x-right: iam/deleteGroup
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/RecoverDatalakeRequest'
+            $ref: '#/definitions/DeleteGroupRequest'
       responses:
         200:
-          description: Expected response to a valid recover data lake request.
+          description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/RecoverDatalakeResponse'
+            $ref: '#/definitions/DeleteGroupResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/setCatalog:
+  /iam/listGroups:
     post:
-      summary: Sets a catalog for a DataLake.
-      description: Sets a catalog for a DataLake.
-      operationId: setCatalog
-      x-mutating: true
+      summary: Lists groups.
+      description: Lists groups. If no group names are specified, the call lists all groups.
+      operationId: listGroups
+      x-right: iam/listGroups
+      x-paginates: true
+      x-paging-default-max-items: 100
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/SetCatalogRequest'
+            $ref: '#/definitions/ListGroupsRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/SetCatalogResponse'
+            $ref: '#/definitions/ListGroupsResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/syncComponentVersionsFromCm:
+  /iam/updateGroup:
     post:
-      summary: Syncs component versions from CM after a failed upgrade.
-      description: Syncs component versions from CM after a failed upgrade.
+      summary: Update a group.
+      description: Update a group.
+      operationId: updateGroup
+      x-right: iam/updateGroup
       x-no-compatibility-guarantee: true
-      operationId: syncComponentVersionsFromCm
-      x-mutating: true
+      x-entitlement: IDENTITY_FEDERATION
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/UpdateGroupRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/UpdateGroupResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /iam/addUserToGroup:
+    post:
+      summary: Add a user to a group.
+      description: Add a user to group.
+      operationId: addUserToGroup
+      x-right: iam/addMemberToGroup
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/AddUserToGroupRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/AddUserToGroupResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /iam/addMachineUserToGroup:
+    post:
+      summary: Add a machine user to group.
+      description: Add a machine user to a group.
+      operationId: addMachineUserToGroup
+      x-right: iam/addMemberToGroup
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/AddMachineUserToGroupRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/AddMachineUserToGroupResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /iam/removeUserFromGroup:
+    post:
+      summary: Remove a user from a group.
+      description: Remove a user from a group.
+      operationId: removeUserFromGroup
+      x-right: iam/removeMemberFromGroup
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/RemoveUserFromGroupRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/RemoveUserFromGroupResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /iam/removeMachineUserFromGroup:
+    post:
+      summary: Remove a machine user from a group.
+      description: Remove a machine user from a group.
+      operationId: removeMachineUserFromGroup
+      x-right: iam/removeMemberFromGroup
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/SyncComponentVersionsFromCmRequest'
+            $ref: '#/definitions/RemoveMachineUserFromGroupRequest'
       responses:
         200:
-          description: Expected response to a valid sync datahub CM component versions request.
+          description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/SyncComponentVersionsFromCmResponse'
+            $ref: '#/definitions/RemoveMachineUserFromGroupResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/rotateSaltPassword:
+  /iam/listGroupMembers:
     post:
-      summary: Rotate SaltStack user password on DataLake instances.
-      description: Rotate SaltStack user password on DataLake instances.
-      operationId: rotateSaltPassword
-      x-mutating: true
-      x-entitlement: CDP_ROTATE_SALTUSER_PASSWORD
+      summary: List the members of a group.
+      description: List the members of a group.
+      operationId: listGroupMembers
+      x-right: iam/listGroupMembers
+      x-paginates: true
+      x-paging-default-max-items: 100
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/RotateSaltPasswordRequest'
+            $ref: '#/definitions/ListGroupMembersRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/RotateSaltPasswordResponse'
+            $ref: '#/definitions/ListGroupMembersResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/datalake/updateOrchestratorState:
+  /iam/listGroupsForUser:
     post:
-      summary: Run orchestrator engine state update on the Data Lake cluster.
-      description: Run orchestrator engine state update on the Data Lake cluster.
-      operationId: updateOrchestratorState
-      x-mutating: true
+      summary: List the groups that the user belongs to.
+      description: List the groups that the user belongs to.
+      operationId: listGroupsForUser
+      x-right: iam/listGroupsForActor
+      x-paginates: true
+      x-paging-default-max-items: 100
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/UpdateOrchestratorStateRequest'
+            $ref: '#/definitions/ListGroupsForUserRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/UpdateOrchestratorStateResponse'
+            $ref: '#/definitions/ListGroupsForUserResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /iam/listGroupsForMachineUser:
+    post:
+      summary: List the groups that the machine user belongs to.
+      description: List the groups that the machine user belongs to.
+      operationId: listGroupsForMachineUser
+      x-right: iam/listGroupsForActor
+      x-paginates: true
+      x-paging-default-max-items: 100
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/ListGroupsForMachineUserRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/ListGroupsForMachineUserResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /iam/assignGroupRole:
+    post:
+      summary: Assign a role to a group.
+      description: Assign a role to a group. If the role is already assigned to the group the request will fail.
+      operationId: assignGroupRole
+      x-right: iam/assignRole
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/AssignGroupRoleRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/AssignGroupRoleResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /iam/unassignGroupRole:
+    post:
+      summary: Unassign a role from a group.
+      description: Unassign a role from a group. If the role is not currently assigned to the group the request will fail.
+      operationId: unassignGroupRole
+      x-right: iam/unassignRole
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/UnassignGroupRoleRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/UnassignGroupRoleResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /iam/assignGroupResourceRole:
+    post:
+      summary: Assign a resource role to a group.
+      description: Assign a resource role to a group. If the resource role is already assigned to the group the request will fail.
+      operationId: assignGroupResourceRole
+      x-right: iam/assignResourceRole
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/AssignGroupResourceRoleRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/AssignGroupResourceRoleResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /iam/unassignGroupResourceRole:
+    post:
+      summary: Unassign a resource role from a group.
+      description: Unassign a resource role from a group. If the resource role is not currently assigned to the group the request will fail.
+      operationId: unassignGroupResourceRole
+      x-right: iam/unassignResourceRole
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/UnassignGroupResourceRoleRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/UnassignGroupResourceRoleResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /iam/listGroupAssignedRoles:
+    post:
+      summary: Lists the group's assigned roles.
+      description: Lists the group's assigned roles.
+      operationId: listGroupAssignedRoles
+      x-right: iam/listAssignedRoles
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/ListGroupAssignedRolesRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/ListGroupAssignedRolesResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /iam/listGroupAssignedResourceRoles:
+    post:
+      summary: Lists a group's assigned resource roles.
+      description: Lists a group's assigned resource roles.
+      operationId: listGroupAssignedResourceRoles
+      x-right: iam/listAssignedResourceRoles
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/ListGroupAssignedResourceRolesRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/ListGroupAssignedResourceRolesResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /iam/setWorkloadPassword:
+    post:
+      summary: Set the workload password for an actor.
+      description: Set the workload password for an actor. This will be the actor's password in all Environments they have access to, including Environments they are given access to after setting the password. The password plaintext is not kept.
+      operationId: setWorkloadPassword
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/SetWorkloadPasswordRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/SetWorkloadPasswordResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /iam/setWorkloadPasswordPolicy:
+    post:
+      summary: Set the workload password policy for the account.
+      description: Set the workload password for the account. Changes to the workload password policy only affect passwords that are set after the policy has been updated. By default, passwords never expire.
+      operationId: setWorkloadPasswordPolicy
+      x-no-compatibility-guarantee: true
+      x-right: iam/setWorkloadPasswordPolicy
+      x-entitlement: WORKLOAD_PASSWORD_POLICY
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/SetWorkloadPasswordPolicyRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/SetWorkloadPasswordPolicyResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
 definitions:
   Error:
     type: object
@@ -872,1957 +1162,1570 @@
     properties:
       code:
         type: string
         description: The error code.
       message:
         type: string
         description: The error message.
-  ClouderaManagerDetails:
-    type: object
-    description: Cloudera Manager details.
-    required:
-      - version
-      - clouderaManagerRepositoryURL
-    properties:
-      version:
-        type: string
-        description: Cloudera Manager version.
-      clouderaManagerRepositoryURL:
-        type: string
-        description: Cloudera Manager repository URL.
-      clouderaManagerServerURL:
-        type: string
-        description: Cloudera Manager server URL.
-  ProductVersion:
+  WorkloadPasswordPolicy:
     type: object
-    description: Product version.
+    description: Information about the workload password policy for an account.
+    x-no-compatibility-guarantee: true
     required:
-      - name
-      - version
-    properties:
-      name:
-        type: string
-        description: The name of the product.
-      version:
-        type: string
-        description: The version of the product.
-  AWSConfiguration:
-    type: object
-    description: AWS configuration.
-    properties:
-      instanceProfile:
-        type: string
-        description: The instance profile used for the ID Broker instance.
-  AzureConfiguration:
-    type: object
-    description: Azure configuration.
-    properties:
-      managedIdentity:
-        type: string
-        description: The managed identity used for the ID Broker instance.
-  GCPConfiguration:
-    type: object
-    description: GCP configuration.
+      - maxPasswordLifetimeDays
     properties:
-      serviceAccountEmail:
-        type: string
-        description: The email id of the service account used for the ID Broker instance.
-  StartDatalakeVerticalScalingRequest:
+      maxPasswordLifetimeDays:
+        type: integer
+        format: int32
+        description: The max lifetime, in days, of the password. If '0' passwords never expire.
+  Account:
     type: object
-    description: The request object for Data Lake vertical scaling.
+    description: Information about a Cloudera Altus account.
+    x-no-compatibility-guarantee: true
     required:
-      - datalake
-      - group
-      - instanceTemplate
-    properties:
-      datalake:
-        type: string
-        description: The name or CRN of the Data Lake.
-      group:
-        type: string
-        description: The target group that requested vertical scaling.
-      instanceTemplate:
-        description: Instance template that specifies the core information for the vertical scale.
-        $ref: '#/definitions/InstanceTemplate'
-  StartDatalakeVerticalScalingResponse:
-    type: object
-    description: The response object for Data Lake vertical scaling.
+      - clouderaSSOLoginEnabled
+      - workloadPasswordPolicy
     properties:
-      result:
-        type: string
-        description: The result of the operation.
-  InstanceTemplate:
-    type: object
-    description: Instance template that specifies the core information for the vertical scale.
-    properties:
-      instanceType:
-        type: string
-        description: The type of the instance.
-  DatalakeDetails:
+      clouderaSSOLoginEnabled:
+        type: boolean
+        description: Whether interactive login using Cloudera SSO is enabled.
+      workloadPasswordPolicy:
+        x-no-compatibility-guarantee: true
+        $ref: '#/definitions/WorkloadPasswordPolicy'
+        description: The workload password policy object.
+  User:
     type: object
-    description: Details about a datalake
+    description: Information about a Cloudera Altus user.
     required:
-      - datalakeName
+      - userId
       - crn
+      - email
+      - firstName
+      - lastName
+      - creationDate
+      - accountAdmin
+      - identityProviderCrn
+    x-limits:
+      - scope: account
+        value: 100
+        doc: The maximum number of users that can be created in an account.
     properties:
-      crn:
-        type: string
-        description: The CRN of the datalake.
-      datalakeName:
+      userId:
         type: string
-        description: The name of the datalake.
-      status:
+        description: The stable, unique identifier of the user.
+      crn:
         type: string
-        description: The status of the datalake.
-      shape:
-        $ref: '#/definitions/DatalakeScaleType'
-        description: The shape of the datalake (either LIGHT_DUTY or MEDIUM_DUTY_HA).
-      environmentCrn:
+        description: The CRN of the user.
+      email:
         type: string
-        description: The CRN of the environment.
-      credentialCrn:
+        description: The user's email address.
+      firstName:
         type: string
-        description: The CRN of credentials.
-      cloudPlatform:
+        description: The user's first name.
+      lastName:
         type: string
-        description: The cloud platform.
-      instanceGroups:
-        type: array
-        items:
-          $ref: '#/definitions/InstanceGroup'
-        description: The instance details.
+        description: The user's last name.
       creationDate:
         type: string
         format: date-time
-        description: The date when the datalake was created.
-      clouderaManager:
-        $ref: '#/definitions/ClouderaManagerDetails'
-        description: The Cloudera Manager details.
-      productVersions:
-        type: array
-        items:
-          $ref: '#/definitions/ProductVersion'
-        description: The product versions.
-      region:
-        type: string
-        description: The region of the datalake.
-      statusReason:
-        type: string
-        description: The reason for the status of the datalake.
-      awsConfiguration:
-        $ref: '#/definitions/AWSConfiguration'
-        description: The AWS configuration.
-      azureConfiguration:
-        $ref: '#/definitions/AzureConfiguration'
-        description: The Azure configuration.
-      gcpConfiguration:
-        $ref: '#/definitions/GCPConfiguration'
-        description: The GCP configuration.
-      endpoints:
-        $ref: '#/definitions/Endpoints'
-        description: The exposed service api endpoints.
-      cloudStorageBaseLocation:
-        type: string
-        description: The base location for the cloud storage used for the datalake.
-      enableRangerRaz:
+        description: The date when this user record was created.
+      accountAdmin:
         type: boolean
-        description: Whether Ranger RAZ is enabled for the datalake.
-  InstanceGroup:
-    type: object
-    description: The type of the instance group which also contains the actual instance(s)
-    required:
-      - name
-      - instances
-    properties:
-      name:
-        type: string
-        description: The name of the instance group.
-      instances:
-        type: array
-        items:
-          $ref: '#/definitions/Instance'
-        description: List of instances in this instance group.
-  Instance:
-    type: object
-    description: Object which holds some details of an instance for the given cluster.
-    required:
-      - id
-      - state
-    properties:
-      id:
-        type: string
-        description: The ID of the given instance.
-      state:
-        type: string
-        description: The actual state of the instance.
-      discoveryFQDN:
-        type: string
-        description: The FQDN of the instance.
-      instanceStatus:
-        $ref: '#/definitions/DatalakeInstanceStatus'
-        description: The status of the instance.
-      statusReason:
+        description: Whether the user is an administrator of their Altus account.
+      identityProviderCrn:
         type: string
-        description: The reason for the current status of this instance.
-      privateIp:
-        type: string
-        description: The private IP of the given instance.
-      publicIp:
+        x-no-compatibility-guarantee: true
+        description: The identity provider that the user belongs to. It can be "Cloudera-Default", "Cloudera-Administration", or a customer defined IdP.
+      lastInteractiveLogin:
         type: string
-        description: The public IP of the given instance.
-      sshPort:
-        type: integer
-        format: int32
-        description: The SSH port for the instance.
-      instanceGroup:
+        format: date-time
+        description: The date of the user's last interactive login.
+      workloadUsername:
         type: string
-        description: The name of the instance group this instance belongs to.
-      instanceTypeVal:
-        $ref: '#/definitions/DatalakeInstanceType'
-        description: The instance type.
-  DatalakeInstanceStatus:
-    type: string
-    description: The status of the instance.
-    enum:
-      - REQUESTED
-      - FAILED
-      - CREATED
-      - ORCHESTRATION_FAILED
-      - SERVICES_RUNNING
-      - SERVICES_HEALTHY
-      - SERVICES_UNHEALTHY
-      - WAITING_FOR_REPAIR
-      - STOPPED
-      - DELETED_ON_PROVIDER_SIDE
-      - DELETED_BY_PROVIDER
-      - DELETE_REQUESTED
-      - DECOMMISSIONED
-      - DECOMMISION_FAILED
-      - TERMINATED
-  DatalakeInstanceType:
-    type: string
-    description: The type of the instance.
-    enum:
-      - GATEWAY
-      - GATEWAY_PRIMARY
-      - CORE
-  Endpoints:
-    type: object
-    description: Object which holds the exposed endpoints for the given cluster.
-    required:
-      - endpoints
-    properties:
-      endpoints:
-        type: array
-        items:
-          $ref: '#/definitions/Endpoint'
-        description: The exposed API endpoints.
-  Endpoint:
-    type: object
-    description: Object which holds the exposed endpoint.
-    required:
-      - serviceName
-      - serviceUrl
-      - displayName
-      - knoxService
-      - mode
-      - open
+        description: The username used in all the workload clusters of the user.
+        x-no-compatibility-guarantee: true
+  MachineUser:
+    type: object
+    description: Information about a Cloudera Altus machine user.
+    required:
+      - machineUserName
+      - crn
+      - creationDate
+    x-limits:
+      - scope: account
+        value: 100
+        doc: The maximum number of machine users that can be created in an account.
     properties:
-      serviceName:
-        type: string
-        description: The name of the exposed service
-      serviceUrl:
+      machineUserName:
         type: string
-        description: The server url for the given exposed service's API.
-      displayName:
+        description: The machine user name.
+      crn:
         type: string
-        description: The more consumable name of the exposed service.
-      knoxService:
+        description: The CRN of the user.
+      creationDate:
         type: string
-        description: The related knox entry.
-      mode:
+        format: date-time
+        description: The date when this machine user record was created.
+      workloadUsername:
         type: string
-        description: The SSO mode of the given service.
-      open:
-        type: boolean
-        description: The access status of the given endpoint. Whether its open or not.
-  Datalake:
+        description: The username used in all the workload clusters of the machine user.
+        x-no-compatibility-guarantee: true
+  AccessKey:
     type: object
-    description: Information about a datalake.
+    description: Information about a Cloudera Altus access key.
     required:
-      - datalakeName
+      - accessKeyId
       - crn
+      - actorCrn
+      - creationDate
+    x-limits:
+      - scope: account
+        value: 200
+        doc: The maximum number of access keys that can be created in an account.
     properties:
-      datalakeName:
+      accessKeyId:
         type: string
-        description: The name of the datalake.
+        description: The ID of the access key.
       crn:
         type: string
-        description: The CRN of the datalake.
-      status:
-        type: string
-        description: The status of the datalake.
-      environmentCrn:
+        description: The CRN of the access key.
+      actorCrn:
         type: string
-        description: The CRN of the environment.
+        description: The CRN of the actor with which this access key is associated.
       creationDate:
         type: string
         format: date-time
-        description: The date when the datalake was created.
-      statusReason:
+        description: The date when the access key was created.
+      status:
         type: string
-        description: The reason for the status of the datalake.
-      enableRangerRaz:
-        type: boolean
-        description: Whether Ranger RAZ is enabled for the datalake.
-      certificateExpirationState:
+        description: The status of an access key.
+        enum:
+          - ACTIVE
+          - INACTIVE
+      type:
         type: string
-        description: Indicates the certificate status on the cluster.
+        description: The type of an access key.
         enum:
-          - VALID
-          - HOST_CERT_EXPIRING
-      multiAz:
-        type: boolean
-        description: Flag which marks that the datalake is deployed in a multi-availability zone way or not.
-  DatalakeResourceTagRequest:
+          - V1
+          - V2
+      lastUsage:
+        $ref: '#/definitions/AccessKeyLastUsage'
+        description: Information on the last time this access key was used.
+  AccessKeyLastUsage:
     type: object
-    description: Tag for a datalake resource.
-    required:
-      - key
-      - value
+    description: Information on the last time an access key was used.
     properties:
-      key:
+      lastUsageDate:
         type: string
-        description: The key of tag.
-      value:
+        format: date-time
+        description: The date when the access key was last used.
+      serviceName:
         type: string
-        description: The value of the tag.
-  DatalakeResourceGCPTagRequest:
+        description: The name of the service with which this access key was most recently used.
+  PolicyStatement:
     type: object
-    description: A label that can be attached to GCP Data Lake resources. Please refer to Google documentation for the rules https://cloud.google.com/compute/docs/labeling-resources#label_format.
+    description: A policy statement is a list of rights and zero or more resources on which the rights are granted.
     required:
-      - key
-      - value
+      - rights
+      - resources
     properties:
-      key:
-        type: string
-        description: The key of tag.
-      value:
-        type: string
-        description: The value of the tag.
-  ListRuntimesRequest:
-    type: object
-    description: Request object for list datalake runtime versions.
-  ListRuntimesResponse:
+      rights:
+        type: array
+        items:
+          type: string
+        description: The list of rights in the policy statement.
+      resources:
+        type: array
+        items:
+          type: string
+        description: The resources on which the rights are granted.
+  Policy:
     type: object
-    description: Response object for list datalake runtime versions.
+    description: A policy contains a list of one or more policy statements.
     required:
-      - versions
+      - crn
+      - policyStatements
     properties:
-      versions:
+      crn:
+        type: string
+        description: The policy crn.
+      policyStatements:
         type: array
         items:
-          $ref: '#/definitions/Runtime'
-        description: The list of datalake runtime versions.
-  Runtime:
+          $ref: '#/definitions/PolicyStatement'
+        description: The policy statements.
+  ResourceRole:
     type: object
-    description: An advertised datalake runtime version.
+    description: Information about a resource role. A resource role is a role that grants a collection of rights to a user on resources.
     required:
-      - runtimeVersion
-      - defaultRuntimeVersion
+      - crn
+      - rights
     properties:
-      runtimeVersion:
+      crn:
         type: string
-        description: The actual version number.
-      defaultRuntimeVersion:
-        type: boolean
-        description: Whether it is a default runtime version or not.
-  AWSConfigurationRequest:
+        description: The CRN of the resource role.
+      rights:
+        type: array
+        items:
+          type: string
+        description: The rights granted by this role.
+  Role:
     type: object
-    description: Request object for AWS configuration.
+    description: Information about a role.
     required:
-      - instanceProfile
-      - storageBucketLocation
+      - crn
+      - policies
     properties:
-      instanceProfile:
-        type: string
-        description: The ARN of an IAM instance profile.
-      storageBucketLocation:
+      crn:
         type: string
-        description: The location of the S3 bucket to be used as storage. The location has to start with s3a:// followed by the bucket name.
-  AzureConfigurationRequest:
+        description: The role's CRN.
+      policies:
+        type: array
+        items:
+          $ref: '#/definitions/Policy'
+        description: The list of policies that belong to the role. Cannot be empty.
+  ResourceAssignment:
     type: object
-    description: Request object for Azure configuration.
+    description: Information about a resource assignment.
     required:
-      - managedIdentity
-      - storageLocation
+      - resourceCrn
+      - resourceRoleCrn
     properties:
-      managedIdentity:
+      resourceCrn:
         type: string
-        description: The managed identity to use. The assumer should have Virtual Machine Contributor and Managed Identity Operator roles on subscription level.
-      storageLocation:
+        description: The assigned resource's CRN.
+      resourceRoleCrn:
         type: string
-        description: The storage location to use. The location has to be in the following format abfs://filesystem@storage-account-name.dfs.core.windows.net. The filesystem must already exist and the storage account must be StorageV2.
-  GCPConfigurationRequest:
+        description: The assigned resource role CRN.
+  ResourceAssignee:
     type: object
-    description: Request object for GCP configuration.
+    description: Information about the resource role assignee for the resource.
     required:
-      - serviceAccountEmail
-      - storageLocation
+      - assigneeCrn
+      - resourceRoleCrn
     properties:
-      serviceAccountEmail:
+      assigneeCrn:
         type: string
-        description: Email id of the service account to be associated with the datalake IdBroker instance. This service account should have "token.creator" role for one or more storage accounts that has access to storage.
-      storageLocation:
+        description: The CRN of the assignee.
+      resourceRoleCrn:
         type: string
-        description: The location of the GCS bucket to be used as storage. The location has to start with gs:// followed by the bucket name.
-  CreateAWSDatalakeRequest:
+        description: The assigned resource role CRN.
+  Group:
     type: object
-    description: Request object for create AWS datalake request.
+    description: Information about a group.
     required:
-      - datalakeName
-      - environmentName
-      - cloudProviderConfiguration
+      - groupName
+      - crn
+      - creationDate
     properties:
-      datalakeName:
+      groupName:
+        type: string
+        description: The group name.
+      crn:
         type: string
-        description: The datalake name. This name must be unique, must have between 5 and 100 characters, and must contain only lowercase letters, numbers and hyphens. Names are case-sensitive.
-        minLength: 5
-        maxLength: 100
-      environmentName:
+        description: The CRN of the group.
+      creationDate:
         type: string
-        description: The environment name or CRN.
-      cloudProviderConfiguration:
-        $ref: '#/definitions/AWSConfigurationRequest'
-        description: AWS configuration.
-      scale:
-        description: The scale of the datalake. Allowed values are "LIGHT_DUTY" or "MEDIUM_DUTY_HA". Defaults to "LIGHT_DUTY" if not set.
-        $ref: '#/definitions/DatalakeScaleType'
+        format: date-time
+        description: The date when this group record was created.
+      syncMembershipOnUserLogin:
         x-no-compatibility-guarantee: true
-      tags:
-        type: array
-        description: Tags to be added to Data Lake related resources.
-        items:
-          $ref: '#/definitions/DatalakeResourceTagRequest'
-      runtime:
-        type: string
-        description: Cloudera Runtime version.
-      image:
-        $ref: '#/definitions/ImageRequest'
-        description: The image to use for the datalake. This must not be set if the runtime parameter is provided.
-      enableRangerRaz:
         type: boolean
-        description: Whether to enable Ranger RAZ for the datalake. Defaults to not being enabled.
-      recipes:
-        type: array
-        items:
-          $ref: '#/definitions/InstanceGroupRecipeRequest'
-        description: Additional recipes that will be attached on the datalake instances (by instance groups, most common ones are like 'master' or 'idbroker').
-      javaVersion:
-        type: integer
-        format: int32
-        description: Configure the major version of Java on the cluster.
-  CreateAWSDatalakeResponse:
+        description: Whether group membership is synced when a user logs in. The default is to sync group membership.
+  SamlProvider:
     type: object
-    description: Response object for create AWS datalake request.
+    description: Information used to connect an Altus account to an external identity provider.
+    x-no-compatibility-guarantee: true
     required:
-      - datalake
+      - crn
+      - creationDate
+      - samlProviderName
+      - samlProviderId
+      - syncGroupsOnLogin
     properties:
-      datalake:
-        $ref: '#/definitions/Datalake'
-        description: The datalake.
-  CreateAzureDatalakeRequest:
-    type: object
-    description: Request object for create Azure datalake request.
-    required:
-      - datalakeName
-      - environmentName
-      - cloudProviderConfiguration
-    properties:
-      datalakeName:
-        type: string
-        description: The datalake name. This name must be unique, must have between 5 and 100 characters, and must contain only lowercase letters, numbers and hyphens. Names are case-sensitive.
-        minLength: 5
-        maxLength: 100
-      environmentName:
-        type: string
-        description: The environment name or CRN.
-      cloudProviderConfiguration:
-        $ref: '#/definitions/AzureConfigurationRequest'
-        description: Azure configuration.
-      scale:
-        description: The scale of the datalake. Allowed values are "LIGHT_DUTY" or "MEDIUM_DUTY_HA". Defaults to "LIGHT_DUTY" if not set.
-        $ref: '#/definitions/DatalakeScaleType'
+      crn:
+        type: string
+        description: CRN of the SAML provider in Altus.
         x-no-compatibility-guarantee: true
-      tags:
-        type: array
-        description: Tags to be added to Data Lake related resources.
-        items:
-          $ref: '#/definitions/DatalakeResourceTagRequest'
-      runtime:
+      creationDate:
         type: string
-        description: Cloudera Runtime version.
-      image:
-        $ref: '#/definitions/ImageRequest'
-        description: The image to use for the datalake. This must not be set if the runtime parameter is provided.
-      enableRangerRaz:
+        format: date-time
+        description: The date when this SAML provider record was created.
+        x-no-compatibility-guarantee: true
+      samlProviderName:
+        type: string
+        description: Name of the SAML provider.
+      samlProviderId:
+        type: string
+        description: The unique ID of the saml provider.
+      syncGroupsOnLogin:
         type: boolean
-        description: Whether to enable Ranger RAZ for the datalake. Defaults to not being enabled.
-      recipes:
-        type: array
-        items:
-          $ref: '#/definitions/InstanceGroupRecipeRequest'
-        description: Additional recipes that will be attached on the datalake instances (by instance groups, most common ones are like 'master' or 'idbroker').
-      javaVersion:
-        type: integer
-        format: int32
-        description: Configure the major version of Java on the cluster.
-  CreateAzureDatalakeResponse:
+        description: Whether users federated with this SAML provider will have their group membership synchronized. Group membership can be passed using the https://altus.cloudera.com/SAML/Attributes/groups SAML assertion.
+      samlMetadataDocument:
+        type: string
+        description: The original metadata that was passed while creating the SAML provider connector. This field will not be set for listSamlProviders API response.
+  GetUserRequest:
     type: object
-    description: Response object for create Azure datalake request.
-    required:
-      - datalake
+    description: Request object for a get user request.
     properties:
-      datalake:
-        $ref: '#/definitions/Datalake'
-        description: The datalake.
-  CreateGCPDatalakeRequest:
+      userId:
+        type: string
+        description: The ID of the user to get information about. If it is not included, it defaults to the user making the request.
+  GetUserResponse:
     type: object
-    description: Request object for create GCP Data Lake request.
+    description: Response object for a get user request.
     required:
-      - datalakeName
-      - environmentName
-      - cloudProviderConfiguration
+      - user
     properties:
-      datalakeName:
-        type: string
-        description: The datalake name. This name must be unique, must have between 5 and 100 characters, and must contain only lowercase letters, numbers and hyphens. Names are case-sensitive.
-        minLength: 5
-        maxLength: 100
-      environmentName:
-        type: string
-        description: The environment name or CRN.
-      cloudProviderConfiguration:
-        $ref: '#/definitions/GCPConfigurationRequest'
-        description: GCP configuration.
-      tags:
-        type: array
-        description: Tags that can be attached to GCP Data Lake resources. Please refer to Google documentation for the rules https://cloud.google.com/compute/docs/labeling-resources#label_format.
-        items:
-          $ref: '#/definitions/DatalakeResourceGCPTagRequest'
-      scale:
-        description: The scale of the datalake. Allowed values are "LIGHT_DUTY" or "MEDIUM_DUTY_HA". Defaults to "LIGHT_DUTY" if not set.
-        $ref: '#/definitions/DatalakeScaleType'
-        x-no-compatibility-guarantee: true
-      runtime:
-        type: string
-        description: Cloudera Runtime version.
-      image:
-        $ref: '#/definitions/ImageRequest'
-        description: The image to use for the datalake. This must not be set if the runtime parameter is provided.
-      recipes:
+      user:
+        $ref: '#/definitions/User'
+        description: Information about the user.
+  ListUsersRequest:
+    type: object
+    description: Request object for a list users request.
+    properties:
+      userIds:
         type: array
         items:
-          $ref: '#/definitions/InstanceGroupRecipeRequest'
-        description: Additional recipes that will be attached on the datalake instances (by instance groups, most common ones are like 'master' or 'idbroker').
-      javaVersion:
+          type: string
+        description: The user IDs or CRNs of the users.
+      pageSize:
         type: integer
         format: int32
-        description: Configure the major version of Java on the cluster.
-  CreateGCPDatalakeResponse:
+        minimum: 1
+        maximum: 100
+        x-paging-page-size: true
+        description: The size of each page.
+      startingToken:
+        type: string
+        x-paging-input-token: true
+        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
+  ListUsersResponse:
     type: object
-    description: Response object for create GCP Data Lake request.
+    description: Response object for a list users request.
     required:
-      - datalake
+      - users
     properties:
-      datalake:
-        $ref: '#/definitions/Datalake'
-        description: The datalake.
-  DatalakeScaleType:
-    type: string
-    description: Represents the available datalake scales. Defaults to LIGHT_DUTY if not set.
-    enum:
-      - LIGHT_DUTY
-      - MEDIUM_DUTY_HA
-  ListDatalakesRequest:
+      users:
+        type: array
+        items:
+          $ref: '#/definitions/User'
+        x-paging-result: true
+        description: The users.
+      nextToken:
+        type: string
+        x-paging-output-token: true
+        description: The token to use when requesting the next set of results. If not present, there are no additional results.
+  CreateUserAccessKeyRequest:
     type: object
-    description: Request object for list datalakes request.
+    description: Request object for a create user access key request.
     properties:
-      environmentName:
+      user:
         type: string
-        description: The name or CRN of the environment for which the datalakes will be listed.
-      datalakeName:
+        description: The ID or CRN of the user to whom this access key will be associated. If it is not included, it defaults to the user making the request.
+      type:
         type: string
-        description: The name or CRN of the datalake for which details are requested.
-  ListDatalakesResponse:
+        description: The version of an access key to create. Default is V2. Use V1 for compatibility with old CLI (< 1.6)  and SDK (< 1.3) releases.
+        enum:
+          - V1
+          - V2
+  CreateUserAccessKeyResponse:
     type: object
-    description: Response object for list datalakes request.
+    description: Response object for a create user access key request.
     required:
-      - datalakes
+      - accessKey
+      - privateKey
     properties:
-      datalakes:
-        type: array
-        items:
-          $ref: '#/definitions/Datalake'
-        description: The datalakes.
-  DeleteDatalakeRequest:
+      accessKey:
+        $ref: '#/definitions/AccessKey'
+        description: The access key that was created.
+      privateKey:
+        type: string
+        description: The private key associated with this access key. This string is the contents of a PEM file containing a PKCS#8 private key.
+        x-sensitive: true
+  CreateMachineUserAccessKeyRequest:
     type: object
-    description: Request object for delete datalake request.
+    description: Request object for a create machine user access key request.
     required:
-      - datalakeName
+      - machineUserName
     properties:
-      datalakeName:
+      machineUserName:
         type: string
-        description: The name or CRN of the datalake to be deleted.
-      force:
-        type: boolean
-        description: Whether the datalake should be force deleted. This option can be used when cluster deletion fails. This removes the entry from Cloudera Datalake service. Any lingering resources have to be deleted from the cloud provider manually. The default is false.
-  DeleteDatalakeResponse:
-    type: object
-    description: Response object for delete datalake request.
-  RetryDatalakeResponse:
-    type: object
-    description: Response object for retry datalake request.
-  RetryDatalakeRequest:
+        description: The name or CRN of the machine user to whom this access key will be associated.
+      type:
+        type: string
+        description: The version of an access key to create. Default is V2. Use V1 for compatibility with old CLI (< 1.6)  and SDK (< 1.3) releases.
+        enum:
+          - V1
+          - V2
+  CreateMachineUserAccessKeyResponse:
     type: object
-    description: Request object for retry datalake request.
+    description: Response object for a create machine user access key request.
     required:
-      - datalakeName
+      - accessKey
+      - privateKey
     properties:
-      datalakeName:
+      accessKey:
+        $ref: '#/definitions/AccessKey'
+        description: The access key that was created.
+      privateKey:
         type: string
-        description: The name or CRN of the datalake to be retry on.
-  DescribeDatalakeRequest:
+        description: The private key associated with this access key. This string is the contents of a PEM file containing a PKCS#8 private key.
+        x-sensitive: true
+  DeleteAccessKeyRequest:
     type: object
-    description: Request object for describe datalake request.
+    description: Request object for a delete access key request.
     required:
-      - datalakeName
+      - accessKeyId
     properties:
-      datalakeName:
+      accessKeyId:
         type: string
-        description: The name or CRN of the datalake.
-  DescribeDatalakeResponse:
+        description: The ID of the access key.
+  DeleteAccessKeyResponse:
     type: object
-    description: Response object for describe datalake request.
+    description: Response object for a delete access key request.
+  UpdateAccessKeyRequest:
+    type: object
+    description: Request object for an update access key request.
     required:
-      - datalake
+      - accessKeyId
+      - status
     properties:
-      datalake:
-        $ref: '#/definitions/DatalakeDetails'
-        description: The datalake.
-  RenewCertificateRequest:
+      accessKeyId:
+        type: string
+        description: The ID of the access key to update.
+      status:
+        type: string
+        description: The status to assign to the access key.
+        enum:
+          - ACTIVE
+          - INACTIVE
+  UpdateAccessKeyResponse:
     type: object
-    description: Request object for renew datalake certificate request, deprecated.
-    x-deprecated: true
+    description: Response object for an update access key request.
     required:
-      - datalakeName
+      - accessKey
     properties:
-      datalakeName:
+      accessKey:
+        $ref: '#/definitions/AccessKey'
+        description: The access key that was updated.
+  GetAccessKeyRequest:
+    type: object
+    description: Request object for a get access key request.
+    properties:
+      accessKeyId:
         type: string
-        description: The name or CRN of the datalake.
-  RepairDatalakeRequest:
+        description: The ID of the access key to get information about. If it is not included, it defaults to the access key used to make the request.
+  GetAccessKeyResponse:
     type: object
-    description: Request object for repair datalake request.
+    description: Response object for a get access key request.
     required:
-      - datalakeName
+      - accessKey
     properties:
-      datalakeName:
-        type: string
-        description: The name or CRN of the datalake.
-      instanceGroupNames:
+      accessKey:
+        $ref: '#/definitions/AccessKey'
+        description: Information about the access key.
+  ListAccessKeysRequest:
+    type: object
+    description: Request object for a list access keys request.
+    properties:
+      accessKeyIds:
         type: array
         items:
           type: string
-        description: List of instance groups where the failed instances will be repaired.
-      instanceGroupName:
+        description: The access key IDs or CRNs of the access keys.
+      pageSize:
+        type: integer
+        format: int32
+        minimum: 1
+        maximum: 100
+        x-paging-page-size: true
+        description: The size of each page.
+      startingToken:
         type: string
-        description: The instance group where the failed instances will be repaired.
-      instances:
-        $ref: '#/definitions/RepairInstancesRequest'
-        description: List of instances.
-  RepairDatalakeResponse:
-    type: object
-    description: Response object for repair datalake request.
-  RepairInstancesRequest:
+        x-paging-input-token: true
+        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
+  ListAccessKeysResponse:
     type: object
-    description: Details for repair instances.
+    description: Response object for a list access keys request.
+    required:
+      - accessKeys
     properties:
-      instanceIds:
+      accessKeys:
         type: array
         items:
-          type: string
-        description: List of instance ids.
-  GetClusterServiceStatusRequest:
+          $ref: '#/definitions/AccessKey'
+        x-paging-result: true
+        description: The access keys.
+      nextToken:
+        type: string
+        x-paging-output-token: true
+        description: The token to use when requesting the next set of results. If not present, there are no additional results.
+  CreateSamlProviderRequest:
     type: object
-    description: Request object to get service status.
+    description: Request object for creating SAML provider request.
+    x-no-compatibility-guarantee: true
     required:
-      - clusterName
+      - samlProviderName
+      - samlMetadataDocument
     properties:
-      clusterName:
+      samlProviderName:
         type: string
-        description: The name or CRN of the cluster.
-  GetClusterServiceStatusResponse:
+        description: The name of SAML provider. The name must be unique, must have a maximum of 128 characters, and must contain only alphanumeric characters, "-" and "_". Names are are not case-sensitive.
+      samlMetadataDocument:
+        type: string
+        description: SAML metadata document XML file. Length of meta data document cannot be more than 200 KB (200,000 bytes).
+        maxLength: 200000
+      syncGroupsOnLogin:
+        type: boolean
+        description: Whether to sync group information for users federated with this SAML provider. Group membership can be passed using the https://altus.cloudera.com/SAML/Attributes/groups SAML assertion. The default is to synchronize group membership.
+  CreateSamlProviderResponse:
     type: object
-    description: Response object to get service status.
+    description: Response object for a creating SAML provider request.
+    x-no-compatibility-guarantee: true
     required:
-      - services
+      - samlProvider
     properties:
-      services:
+      samlProvider:
+        $ref: '#/definitions/SamlProvider'
+        description: The SAML provider.
+  DeleteSamlProviderRequest:
+    type: object
+    description: Request object for deleting SAML provider request.
+    x-no-compatibility-guarantee: true
+    properties:
+      samlProviderName:
+        type: string
+        description: The name or CRN of the SAML provider to delete.
+  DeleteSamlProviderResponse:
+    type: object
+    description: Response object for delete SAML provider request.
+    x-no-compatibility-guarantee: true
+  ListSamlProvidersRequest:
+    type: object
+    description: Request object for a list SAML providers request.
+    x-no-compatibility-guarantee: true
+    properties:
+      samlProviderNames:
         type: array
+        description: The SAML providers names or CRNs to retrieve. If empty all SAML providers will be returned.
         items:
-          $ref: '#/definitions/ServiceStatus'
-        description: The cluster services health.
-  ServiceStatus:
+          type: string
+          description: The SAML providers names or CRNs to retrieve. If empty all SAML providers will be returned.
+      pageSize:
+        type: integer
+        format: int32
+        minimum: 1
+        maximum: 100
+        x-paging-page-size: true
+        description: The size of each page.
+      startingToken:
+        type: string
+        x-paging-input-token: true
+        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
+  ListSamlProvidersResponse:
     type: object
-    description: Information about a cluster service.
+    description: Response object for a list SAML providers request.
+    x-no-compatibility-guarantee: true
+    required:
+      - samlProviders
     properties:
-      type:
-        type: string
-        description: The service type.
-      state:
-        type: string
-        description: The service state.
-      healthSummary:
-        type: string
-        description: The service health summary.
-      healthChecks:
+      samlProviders:
         type: array
         items:
-          $ref: '#/definitions/HealthCheck'
-        description: The service health checks.
-  HealthCheck:
+          $ref: '#/definitions/SamlProvider'
+        x-paging-result: true
+        description: The SAML providers.
+      nextToken:
+        type: string
+        x-paging-output-token: true
+        description: The token to use when requesting the next set of results. If not present, there are no additional results.
+  UpdateSamlProviderRequest:
     type: object
-    description: The result of a health check.
+    description: Request object for an updating SAML provider request.
+    x-no-compatibility-guarantee: true
+    required:
+      - samlProviderName
     properties:
-      name:
+      samlProviderName:
         type: string
-        description: The name of service health check.
-      summary:
+        description: The name or CRN of SAML provider to update.
+      samlMetadataDocument:
         type: string
-        description: The service health check summary.
-  GetClusterHostStatusRequest:
+        description: SAML metadata document XML file. Length of meta data document cannot be more than 200 KB (200,000 bytes). Can be omitted if no update is required.
+        maxLength: 200000
+      syncGroupsOnLogin:
+        type: boolean
+        description: Whether to sync group information for users federated with this SAML provider. Group membership can be passed using the https://altus.cloudera.com/SAML/Attributes/groups SAML assertion. The default is to synchronize group membership. Can be omitted if no update is required.
+  UpdateSamlProviderResponse:
     type: object
-    description: Request object to get host status.
+    description: Response object for an updating SAML provider request.
+    x-no-compatibility-guarantee: true
     required:
-      - clusterName
+      - samlProvider
     properties:
-      clusterName:
-        type: string
-        description: The name or CRN of the cluster.
-  GetClusterHostStatusResponse:
+      samlProvider:
+        $ref: '#/definitions/SamlProvider'
+        description: The SAML provider.
+  ListRolesRequest:
     type: object
-    description: Response object for getting host status.
+    description: Request object for a list roles request.
+    properties:
+      roleNames:
+        type: array
+        items:
+          type: string
+        description: The roles names or CRNs to retrieve. If empty all roles will be returned.
+      pageSize:
+        type: integer
+        format: int32
+        minimum: 1
+        maximum: 100
+        x-paging-page-size: true
+        description: The size of each page.
+      startingToken:
+        type: string
+        x-paging-input-token: true
+        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
+  ListRolesResponse:
+    type: object
+    description: Response object for a list roles request.
     required:
-      - hosts
+      - roles
     properties:
-      hosts:
+      roles:
         type: array
         items:
-          $ref: '#/definitions/HostStatus'
-        description: The cluster hosts status.
-  HostStatus:
+          $ref: '#/definitions/Role'
+        x-paging-result: true
+        description: The list of roles in the account.
+      nextToken:
+        type: string
+        x-paging-output-token: true
+        description: The token to use when requesting the next set of results. If not present, there are no additional results.
+  ListResourceRolesRequest:
     type: object
-    description: Information about cluster host status.
+    description: Request object for a list resource roles request.
     properties:
-      hostid:
-        type: string
-        description: Unique identifier of the cluster host given by Cloudera Manager.
-      hostname:
-        type: string
-        description: The cluster hostname.
-      healthSummary:
+      resourceRoleNames:
+        type: array
+        items:
+          type: string
+        description: The resource roles CRNs to retrieve. If empty all resource roles will be returned.
+      pageSize:
+        type: integer
+        format: int32
+        minimum: 1
+        maximum: 100
+        x-paging-page-size: true
+        description: The size of each page.
+      startingToken:
         type: string
-        description: The host health summary.
-  StartDatalakeRequest:
+        x-paging-input-token: true
+        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
+  ListResourceRolesResponse:
     type: object
-    description: Request object to start a datalake, deprecated.
-    x-deprecated: true
+    description: Response object for a list resource roles request.
     required:
-      - datalakeName
+      - resourceRoles
     properties:
-      datalakeName:
+      resourceRoles:
+        type: array
+        items:
+          $ref: '#/definitions/ResourceRole'
+        x-paging-result: true
+        description: The list of resource roles. Cannot be empty.
+      nextToken:
         type: string
-        description: The name or CRN of the datalake.
-  StartDatalakeResponse:
+        x-paging-output-token: true
+        description: The token to use when requesting the next set of results. If not present, there are no additional results.
+  AssignUserRoleRequest:
     type: object
-    description: Response object of starting a datalake, deprecated.
-    x-deprecated: true
-  StopDatalakeRequest:
-    type: object
-    description: Request object to stop a datalake, deprecated.
-    x-deprecated: true
+    description: Request object for an assign user role request.
     required:
-      - datalakeName
+      - user
+      - role
     properties:
-      datalakeName:
+      user:
+        type: string
+        description: The user the role is assigned to. Can be the user's CRN or id.
+      role:
         type: string
-        description: The name or CRN of the datalakeName.
-  StopDatalakeResponse:
+        description: The role to assign to the user. Can be the role's CRN or name.
+  AssignUserRoleResponse:
     type: object
-    description: Response object of stopping a datalake, deprecated.
-    x-deprecated: true
-  BackupDatalakeRequest:
+    description: Response object for an assign user role request.
+  UnassignUserRoleRequest:
     type: object
-    description: Request object to perform a backup of datalake.
+    description: Request object for an unassign user role request.
     required:
-      - datalakeName
+      - user
+      - role
     properties:
-      datalakeName:
-        type: string
-        description: The name of the datalake.
-      backupLocation:
+      user:
         type: string
-        description: Location where the back-up has to be stored. For example s3a://Location/of/the/backup.
-      backupName:
+        description: The user to unassigned the roles from. Can be the user CRN or id.
+      role:
         type: string
-        description: The name of the backup.
-      closeDbConnections:
-        type: boolean
-        default: true
-        description: Close the database connections while performing backup. Default is true.
-      skipRangerHmsMetadata:
-        type: boolean
-        description: Skips the backup of the databases backing HMS/Ranger services. If this option is not provided, the HMS/Ranger services are backed up by default.
-      skipAtlasMetadata:
-        type: boolean
-        description: Skips the backup of the Atlas metadata. If this option is not provided, the Atlas metadata is backed up by default.
-      skipRangerAudits:
-        type: boolean
-        description: Skips the backup of the Ranger audits. If this option is not provided, Ranger audits are backed up by default.
-      skipAtlasIndexes:
-        type: boolean
-        description: Skips the backup of the Atlas indexes. If this option or --skipAtlasMetadata is not provided, Atlas indexes are backed up by default. Redundant if --skipAtlasMetadata is included.
-      skipValidation:
-        type: boolean
-        description: Skips the validation steps that run prior to the backup. If this option is not provided, the validations are performed by default.
-      validationOnly:
-        type: boolean
-        description: Runs only the validation steps and then returns. If this option is not provided, the backup is performed as normal by default.
-  BackupDatalakeResponse:
+        description: The role to unassigned from the user. Can be the role's CRN or name.
+  UnassignUserRoleResponse:
+    type: object
+    description: Response object for an unassign user role request.
+  AssignUserResourceRoleRequest:
     type: object
-    description: Response object to a request made for backup of datalake.
+    description: Request object for an assign user resource role request.
     required:
-      - accountId
-      - backupId
-      - userCrn
-      - internalState
-      - status
-      - startTime
-      - endTime
-      - backupLocation
-      - operationStates
+      - user
+      - resourceRoleCrn
+      - resourceCrn
     properties:
-      accountId:
-        type: string
-        description: Account where the datalake exists.
-      backupId:
-        type: string
-        description: Unique identifier for the backup requested.
-      userCrn:
-        type: string
-        description: Crn of the user who triggered this operation.
-      internalState:
-        type: string
-        description: Provides the details of the internal state where the backup operation stands.
-      status:
-        type: string
-        description: Provide the current status.
-      startTime:
-        type: string
-        description: Time when the backup operation started.
-      endTime:
-        type: string
-        description: Time when the backup operation ended.
-      backupLocation:
+      user:
         type: string
-        description: Location of the backup to be used to perform restore.
-      operationStates:
-        $ref: '#/definitions/InternalBackupRestoreState'
-        description: Provides the details of the internal state of each operation.
-      runtimeVersion:
+        description: The user to assign the resource role to. Can be the user's CRN or id.
+      resourceRoleCrn:
         type: string
-        description: The runtime version of the datalake when the backup was taken.
-      backupName:
-        type: string
-        description: Name of the backup.
-      failureReason:
+        description: The CRN of the resource role to assign to the user.
+      resourceCrn:
         type: string
-        description: Reason for the failure.
-  BackupDatalakeStatusRequest:
+        description: The resource for which the resource role rights are granted.
+  AssignUserResourceRoleResponse:
+    type: object
+    description: Response object for an assign user resource role request.
+  UnassignUserResourceRoleRequest:
     type: object
-    description: Request object to get the status of datalake backup. Returns the status of the latest backup that matches the provided input.
+    description: Request object for an unassign user role request.
     required:
-      - datalakeName
+      - user
+      - resourceRoleCrn
+      - resourceCrn
     properties:
-      datalakeName:
+      user:
         type: string
-        description: The name of the datalake. When backupName and backupId are not provided, status request will get the status of the latest backup operation performed on the given datalake.
-      backupName:
+        description: The user to unassign the resource role from.
+      resourceRoleCrn:
         type: string
-        description: The name of the backup. When provided, the status request will get the status of the latest backup performed with the given backup name on the given datalake.
-      backupId:
+        description: The CRN of the resource role to unassigned from the user.
+      resourceCrn:
         type: string
-        description: Unique identifier of the backup performed. When provided, the status request will get the status entry that has the backupid provided.
-  BackupDatalakeStatusResponse:
+        description: The CRN of the resource for which the resource role rights will be unassigned.
+  UnassignUserResourceRoleResponse:
     type: object
-    description: Response object to get the status of datalake backup status request.
-    required:
-      - accountId
-      - backupId
-      - userCrn
-      - internalState
-      - status
-      - startTime
-      - endTime
-      - backupLocation
-      - operationStates
+    description: Response object for an unassign user role request.
+  ListUserAssignedRolesRequest:
+    type: object
+    description: Request object for a list user assigned roles request.
     properties:
-      accountId:
-        type: string
-        description: Account where the datalake exists.
-      backupId:
-        type: string
-        description: Unique identifier for the backup requested.
-      userCrn:
-        type: string
-        description: Crn of the user who triggered this operation.
-      internalState:
-        type: string
-        description: Provides the details of the internal state where the backup operation stands.
-      status:
-        type: string
-        description: Provide the current status.
-      startTime:
-        type: string
-        description: Time when the backup operation started.
-      endTime:
-        type: string
-        description: Time when the backup operation ended.
-      backupLocation:
-        type: string
-        description: Location of the backup to be used to perform restore.
-      operationStates:
-        $ref: '#/definitions/InternalBackupRestoreState'
-        description: Provides the details of the internal state of each operation.
-      runtimeVersion:
-        type: string
-        description: The runtime version of the datalake when the backup was taken.
-      backupName:
+      user:
         type: string
-        description: Name of the backup.
-      failureReason:
+        description: The user to list the assigned roles for. Can be the user's CRN or id. If it is not included, it defaults to the user making the request.
+      pageSize:
+        type: integer
+        format: int32
+        minimum: 1
+        maximum: 100
+        x-paging-page-size: true
+        description: The size of each page.
+      startingToken:
         type: string
-        description: Reason for the failure.
-  RestoreDatalakeRequest:
+        x-paging-input-token: true
+        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
+  ListUserAssignedRolesResponse:
     type: object
-    description: Request to restore datalake from backup. Restore does not restore the database by default.
+    description: Response object for a list user assigned roles request.
     required:
-      - datalakeName
+      - roleCrns
     properties:
-      datalakeName:
-        type: string
-        description: The name of the datalake to be restored. When backupId is not provided, the most recent successful backup on datalake with the provided name would be used.
-      backupId:
+      roleCrns:
+        type: array
+        items:
+          type: string
+        x-paging-result: true
+        description: The role CRNs assigned to the user.
+      nextToken:
         type: string
-        description: The ID of the backup to be used to perform a restore. The ID could refer to backup of any datalake in the same account. This is the only way to restore from a backup that was taken on a datalake with a different name. This field is required if the --backup-location-override field is used.
-      backupName:
+        x-paging-output-token: true
+        description: The token to use when requesting the next set of results. If not present, there are no additional results.
+  ListUserAssignedResourceRolesRequest:
+    type: object
+    description: Request object for a list user assigned resource roles request.
+    properties:
+      user:
         type: string
-        description: The name of the backup. When provided, the restore will be performed using the latest successful backup whose name matches the parameter, and that was taken from the datalake that is being restored.
-      includeDatabase:
-        type: boolean
-        description: DEPRECATED - The database is included in the restore by default. To skip it, use the --skip-ranger-hms-metadata flag.
-      skipRangerHmsMetadata:
-        type: boolean
-        description: Skips the restore of the databases backing HMS/Ranger services. If this option is not provided, then by default the Atlas lineage will be restored if the backup used includes the Atlas lineage information.
-      skipAtlasMetadata:
-        type: boolean
-        description: Skips the restore of the Atlas metadata. If this option is not provided, then by default the Atlas metadata will be restored if the backup used includes the Atlas metadata.
-      skipRangerAudits:
-        type: boolean
-        description: Skips the restore of the Ranger audits. If this option is not provided, then by default the Ranger audits will be restored if the backup used includes the Ranger audits.
-      skipAtlasIndexes:
-        type: boolean
-        description: Skips the restore of the Atlas indexes. If this option or --skipAtlasMetadata is not provided, then by default the Atlas indexes will be restored if the backup used includes the Atlas indexes. Redundant if --skipAtlasMetadata is included.
-      backupLocationOverride:
+        description: The user to list the assigned roles for. Can be the user's CRN or id. If it is not included, it defaults to the user making the request.
+      pageSize:
+        type: integer
+        format: int32
+        minimum: 1
+        maximum: 100
+        x-paging-page-size: true
+        description: The size of each page.
+      startingToken:
         type: string
-        description: Backup location. When provided, will be used to lookup the backup. If provided, the --backup-id parameter is required.
-      skipValidation:
-        type: boolean
-        description: Skips the validation steps that run prior to the restore. If this option is not provided, the validations are performed by default.
-      validationOnly:
-        type: boolean
-        description: Runs only the validation steps and then returns. If this option is not provided, the restore is performed as normal by default.
-  RestoreDatalakeResponse:
+        x-paging-input-token: true
+        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
+  ListUserAssignedResourceRolesResponse:
     type: object
-    description: Response object to a request to perform restore of datalake.
+    description: Response object for a list user assigned roles request.
     required:
-      - accountId
-      - restoreId
-      - backupId
-      - userCrn
-      - internalState
-      - status
-      - startTime
-      - endTime
-      - backupLocation
-      - operationStates
+      - resourceAssignments
     properties:
-      accountId:
-        type: string
-        description: Account where the datalake exists.
-      restoreId:
-        type: string
-        description: Unique identifier of the restore operation performed.
-      backupId:
-        type: string
-        description: Unique identifier of the backup used to perform restore.
-      userCrn:
-        type: string
-        description: Crn of the user who triggered this operation.
-      internalState:
-        type: string
-        description: Provides the details of the internal state where the restore operation stands.
-      status:
-        type: string
-        description: Provide the current status.
-      startTime:
-        type: string
-        description: Time when the backup operation started.
-      endTime:
-        type: string
-        description: Time when the backup operation ended.
-      backupLocation:
-        type: string
-        description: Location of the backup to be used to perform restore.
-      operationStates:
-        $ref: '#/definitions/InternalBackupRestoreState'
-        description: Provides the details of the internal state of each operation.
-      backupName:
-        type: string
-        description: Name of the backup.
-      failureReason:
-        type: string
-        description: Reason for the failure.
-      runtimeVersion:
+      resourceAssignments:
+        type: array
+        items:
+          $ref: '#/definitions/ResourceAssignment'
+        x-paging-result: true
+        description: The user's resource assignments.
+      nextToken:
         type: string
-        description: The runtime version of the datalake when the restore was initiated.
-  RestoreDatalakeStatusRequest:
+        x-paging-output-token: true
+        description: The token to use when requesting the next set of results. If not present, there are no additional results.
+  AssignMachineUserRoleRequest:
     type: object
-    description: Request object to get the status of a restore operation.
+    description: Request object for an assign machine user role request.
     required:
-      - datalakeName
+      - machineUserName
+      - role
     properties:
-      datalakeName:
+      machineUserName:
         type: string
-        description: The name of the Data Lake for which the most recent restore status will be retrieved.
-      restoreId:
+        description: The machine user the role is assigned to. Can be the machine user's name or CRN.
+      role:
         type: string
-        description: Unique identifier of the restore operation performed.
-  RestoreDatalakeStatusResponse:
+        description: The role to assign to the machine user. Can be the role's name or CRN.
+  AssignMachineUserRoleResponse:
     type: object
-    description: Response object with information on last restore operation on a datalake.
+    description: Response object for an assign machine user role request.
+  UnassignMachineUserRoleRequest:
+    type: object
+    description: Request object for an unassign machine user role request.
     required:
-      - accountId
-      - restoreId
-      - backupId
-      - userCrn
-      - internalState
-      - status
-      - startTime
-      - endTime
-      - backupLocation
-      - operationStates
+      - machineUserName
+      - role
     properties:
-      accountId:
-        type: string
-        description: Account where the datalake exists.
-      restoreId:
+      machineUserName:
         type: string
-        description: Unique identifier of the restore operation performed.
-      backupId:
+        description: The machine user to unassigned the roles from. Can be the machine user's name or CRN.
+      role:
         type: string
-        description: Unique identifier of the backup used to perform restore.
-      userCrn:
-        type: string
-        description: Crn of the user who triggered this operation.
-      internalState:
-        type: string
-        description: Provides the details of the internal state where the restore operation stands.
-      status:
-        type: string
-        description: Provide the current status.
-      startTime:
+        description: The role to unassigned from the user. Can be the role's name or CRN.
+  UnassignMachineUserRoleResponse:
+    type: object
+    description: Response object for an unassign machine user role request.
+  AssignMachineUserResourceRoleRequest:
+    type: object
+    description: Request object for an assign machine user resource role request.
+    required:
+      - machineUserName
+      - resourceRoleCrn
+      - resourceCrn
+    properties:
+      machineUserName:
         type: string
-        description: Time when the backup operation started.
-      endTime:
+        description: The machine user to assign the resource role to. Can be the user's name or CRN.
+      resourceRoleCrn:
         type: string
-        description: Time when the backup operation ended.
-      backupLocation:
+        description: The CRN of the resource role to assign to the machine user.
+      resourceCrn:
         type: string
-        description: Location of the backup to be used to perform restore.
-      operationStates:
-        $ref: '#/definitions/InternalBackupRestoreState'
-        description: Provides the details of the internal state of each operation.
-      backupName:
+        description: The resource for which the resource role rights are granted.
+  AssignMachineUserResourceRoleResponse:
+    type: object
+    description: Response object for an assign machine user resource role request.
+  UnassignMachineUserResourceRoleRequest:
+    type: object
+    description: Request object for an unassign machine user role request.
+    required:
+      - machineUserName
+      - resourceRoleCrn
+      - resourceCrn
+    properties:
+      machineUserName:
         type: string
-        description: Name of the backup.
-      failureReason:
+        description: The machine user to unassign the resource role from.
+      resourceRoleCrn:
         type: string
-        description: Reason for the failure.
-      runtimeVersion:
+        description: The CRN of the resource role to unassigned from the machine user.
+      resourceCrn:
         type: string
-        description: The runtime version of the datalake when the restore was initiated.
-  ListDatalakeBackupsRequest:
+        description: The CRN of the resource for which the resource role rights will be unassigned.
+  UnassignMachineUserResourceRoleResponse:
+    type: object
+    description: Response object for an unassign machine user role request.
+  ListMachineUserAssignedRolesRequest:
     type: object
-    description: Request object to get the list of backup operations performed on a datalake.
+    description: Request object for a list machine user assigned roles request.
     required:
-      - datalakeName
+      - machineUserName
     properties:
-      datalakeName:
+      machineUserName:
+        type: string
+        description: The machine user to list the assigned roles for. Can be the machine user's name or CRN.
+      pageSize:
+        type: integer
+        format: int32
+        minimum: 1
+        maximum: 100
+        x-paging-page-size: true
+        description: The size of each page.
+      startingToken:
         type: string
-        description: The name of the datalake.
-  ListDatalakeBackupsResponse:
+        x-paging-input-token: true
+        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
+  ListMachineUserAssignedRolesResponse:
     type: object
-    description: Response object with the list of backup operations performed on a datalake.
+    description: Response object for a list machine user assigned roles request.
+    required:
+      - roleCrns
     properties:
-      backups:
+      roleCrns:
         type: array
-        description: Backup object with details of backup performed.
         items:
-          $ref: '#/definitions/DatalakeBackup'
-  CancelBackupRequest:
-    type: object
-    description: The request to cancel a backup operation.
-    required:
-      - backupId
-    properties:
-      backupId:
+          type: string
+        x-paging-result: true
+        description: The role CRNs assigned to the user.
+      nextToken:
         type: string
-        description: Backup-id that identifies the backup to be cancelled.
-      force:
-        type: boolean
-        default: false
-        description: Will mark all unfinished operations as cancelled without waiting for their result and mark backup operation as finished (cancelled, successful or failed) immediately.
-  CancelBackupResponse:
+        x-paging-output-token: true
+        description: The token to use when requesting the next set of results. If not present, there are no additional results.
+  ListMachineUserAssignedResourceRolesRequest:
     type: object
-    description: Response to the cancel backup request.
+    description: Request object for a list machine user assigned resource roles request.
     required:
-      - result
+      - machineUserName
     properties:
-      result:
+      machineUserName:
         type: string
-        description: Result of the cancel backup request. It can contain a description of the current process state or guidelines to a customer on the next steps.
-  DatalakeBackup:
+        description: The machine user to list the assigned resource roles for. Can be the machine user's name or CRN.
+      pageSize:
+        type: integer
+        format: int32
+        minimum: 1
+        maximum: 100
+        x-paging-page-size: true
+        description: The size of each page.
+      startingToken:
+        type: string
+        x-paging-input-token: true
+        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
+  ListMachineUserAssignedResourceRolesResponse:
     type: object
-    description: Backup object with details of backup performed.
+    description: Response object for a list machine user assigned roles request.
     required:
-      - backupName
-      - accountId
-      - userCrn
-      - backupId
-      - internalState
-      - status
-      - startTime
-      - endTime
-      - backupLocation
-      - failureReason
+      - resourceAssignments
     properties:
-      backupName:
-        type: string
-        description: Name of the backup.
-      accountId:
-        type: string
-        description: Account where the datalake exists.
-      userCrn:
-        type: string
-        description: Crn of the user who triggered this operation.
-      backupId:
-        type: string
-        description: Request to perform a from a specific status for a specific backup. Else, status of the last backup performed will be returned.
-      internalState:
-        type: string
-        description: Provides the details of the internal state where the backup operation stands.
-      status:
-        type: string
-        description: Provide the current status.
-      startTime:
-        type: string
-        description: Time when the backup operation started.
-      endTime:
-        type: string
-        description: Time when the backup operation ended.
-      backupLocation:
+      resourceAssignments:
+        type: array
+        items:
+          $ref: '#/definitions/ResourceAssignment'
+        x-paging-result: true
+        description: The user's resource assignments.
+      nextToken:
         type: string
-        description: Location of the backup to be used to perform restore.
-      failureReason:
-        type: string
-        description: Reason for the failure.
-  InternalBackupRestoreState:
-    type: object
-    description: Object representing the state of each service running a backup.
-    required:
-      - adminOperations
-      - hbase
-      - solr
-      - database
-    properties:
-      adminOperations:
-        $ref: '#/definitions/AdminOperationsBackupRestoreState'
-        description: Admin operations executed via Cloudera Manager for starting and stopping services.
-      hbase:
-        $ref: '#/definitions/HbaseBackupRestoreState'
-        description: Hbase operations to backup or restore Atlas metadata tables.
-      solr:
-        $ref: '#/definitions/SolrBackupRestoreState'
-        description: Solr operations to backup up the edge, fulltext, ranger_audit, and vertex tables, or to delete/restore those tables.
-      database:
-        $ref: '#/definitions/DatabaseBackupRestoreState'
-        description: Postgres operations to backup or restore the data lake metadata.
-  AdminOperationsBackupRestoreState:
-    type: object
-    description: The state of Cloudera Manager admin operations.
-    required:
-      - stopServices
-      - startServices
-      - precheckStoragePermission
-      - rangerAuditCollectionValidation
-    properties:
-      stopServices:
-        $ref: '#/definitions/BackupRestoreOperationStatus'
-        description: The status of the stop services operation that is triggered before the backup/restore is started.
-      startServices:
-        $ref: '#/definitions/BackupRestoreOperationStatus'
-        description: The status of the start services operation this is triggered after the backup/restore is complete.
-      precheckStoragePermission:
-        $ref: '#/definitions/BackupRestoreOperationStatus'
-        description: Validate storage permissions before running a backup/restore.
-      rangerAuditCollectionValidation:
-        $ref: '#/definitions/BackupRestoreOperationStatus'
-        description: Run the ranger audit collection validation in the backup precheck.
-  HbaseBackupRestoreState:
-    type: object
-    description: The state of each HBase backup/restore operation.
-    required:
-      - atlasEntityAuditEventTable
-      - atlasJanusTable
-    properties:
-      atlasEntityAuditEventTable:
-        $ref: '#/definitions/BackupRestoreOperationStatus'
-        description: The status of the ATLAS_ENTITY_AUDIT_EVENTS_TABLE backup/restore.
-      atlasJanusTable:
-        $ref: '#/definitions/BackupRestoreOperationStatus'
-        description: The status of the ATLAS_JANUS_TABLE backup/restore.
-  SolrBackupRestoreState:
-    type: object
-    description: The state of each Solr backup/restore operation.
-    required:
-      - edgeIndexCollection
-      - fulltextIndexCollection
-      - rangerAuditsCollection
-      - vertexIndexCollection
-    properties:
-      edgeIndexCollection:
-        $ref: '#/definitions/BackupRestoreOperationStatus'
-        description: The status of the EDGE_INDEX_COLLECTION backup/restore.
-      fulltextIndexCollection:
-        $ref: '#/definitions/BackupRestoreOperationStatus'
-        description: The status of the FULLTEXT_INDEX_COLLECTION backup/restore.
-      rangerAuditsCollection:
-        $ref: '#/definitions/BackupRestoreOperationStatus'
-        description: The status of the RANGER_AUDITS_COLLECTION backup/restore.
-      vertexIndexCollection:
-        $ref: '#/definitions/BackupRestoreOperationStatus'
-        description: The status of the VERTEX_INDEX_COLLECTION backup/restore.
-      edgeIndexCollectionDelete:
-        $ref: '#/definitions/BackupRestoreOperationStatus'
-        description: The status of the EDGE_INDEX_COLLECTION deletion, which is done before a restore.
-      fulltextIndexCollectionDelete:
-        $ref: '#/definitions/BackupRestoreOperationStatus'
-        description: The status of the FULLTEXT_INDEX_COLLECTION deletion, which is done before a restore.
-      rangerAuditsCollectionDelete:
-        $ref: '#/definitions/BackupRestoreOperationStatus'
-        description: The status of the RANGER_AUDITS_COLLECTION deletion, which is done before a restore.
-      vertexIndexCollectionDelete:
-        $ref: '#/definitions/BackupRestoreOperationStatus'
-        description: The status of the VERTEX_INDEX_COLLECTION deletion, which is done before a restore.
-  DatabaseBackupRestoreState:
-    type: object
-    description: The state of the database backup/restore operation.
-    required:
-      - database
-    properties:
-      database:
-        $ref: '#/definitions/BackupRestoreOperationStatus'
-        description: The status of the database backup/restore.
-  BackupRestoreOperationStatus:
+        x-paging-output-token: true
+        description: The token to use when requesting the next set of results. If not present, there are no additional results.
+  ListResourceAssigneesRequest:
     type: object
-    description: Contains the status and failure reason of an operation.
+    description: Request object for a list resource assignees request.
     required:
-      - status
+      - resourceCrn
     properties:
-      status:
-        type: string
-        description: The status of the backup or restore operation.
-      failureReason:
+      resourceCrn:
         type: string
-        description: The failure reason if the operation was not successful.
-      durationInMinutes:
+        description: The resource CRN for which to list the assignees.
+      pageSize:
+        type: integer
+        format: int32
+        minimum: 1
+        maximum: 100
+        x-paging-page-size: true
+        description: The size of each page.
+      startingToken:
         type: string
-        description: The duration of each operation, in minutes.
-  ImageComponentVersions:
+        x-paging-input-token: true
+        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
+  ListResourceAssigneesResponse:
     type: object
-    description: Versions of the image components
+    description: Response object for a list resource assignees request.
+    required:
+      - resourceAssignees
     properties:
-      cm:
-        type: string
-        description: Version of CM
-      cmGBN:
-        type: string
-        description: GBN of CM
-      cdp:
-        type: string
-        description: CDP version
-      cdpGBN:
-        type: string
-        description: CDP GBN
-      os:
-        type: string
-        description: OS name
-      osPatchLevel:
+      resourceAssignees:
+        type: array
+        items:
+          $ref: '#/definitions/ResourceAssignee'
+        x-paging-result: true
+        description: List of resource assignees and their respective resource roles for the resource.
+      nextToken:
         type: string
-        description: OS patch level
-  ImageInfo:
+        x-paging-output-token: true
+        description: The token to use when requesting the next set of results. If not present, there are no additional results.
+  CreateMachineUserRequest:
     type: object
-    description: Basic information about an image.
+    description: Request object for create machine user request.
+    required:
+      - machineUserName
     properties:
-      imageName:
-        type: string
-        description: The name of the image.
-      imageId:
+      machineUserName:
         type: string
-        description: The id of the image.
-      imageCatalogName:
-        type: string
-        description: Name of the image catalog, the image is from.
-      created:
-        type: integer
-        format: int64
-        description: Image creation timestamp
-      componentVersions:
-        $ref: '#/definitions/ImageComponentVersions'
-        description: Version of the image components
-  UpgradeDatalakeRequest:
+        description: The name to use for the new machine user. The name should be an alpha numeric string, including '-' and '_', no longer than 128 characters long. Only one machine user with this name can be exist at a given time in an account.
+  CreateMachineUserResponse:
     type: object
-    description: Request object to upgrade datalake.
+    description: Response object for create machine user request.
     required:
-      - datalakeName
+      - machineUser
     properties:
-      datalakeName:
-        type: string
-        description: The name or CRN of the datalake.
-      imageId:
-        type: string
-        description: The id of an image to upgrade to
-      runtime:
-        type: string
-        description: The runtime version to upgrade to
-      lockComponents:
-        type: boolean
-        description: Perform an os upgrade only
-      dryRun:
-        type: boolean
-        description: Checks the eligibility of an image to upgrade
-      showAvailableImages:
-        type: boolean
-        description: Returns the list of images that are eligible for the upgrade
-      showLatestAvailableImagePerRuntime:
-        type: boolean
-        description: Returns the latest image that is eligible for the upgrade for each runtime version with at least one available upgrade candidate
-      skipBackup:
-        type: boolean
-        description: If provided, will skip the backup flow for the upgrade process.
-      skipRangerHmsMetadata:
-        type: boolean
-        description: Skips the backup of the databases backing HMS/Ranger services. Redundant if --skip-backup is included. If this option is not provided, the HMS/Ranger services are backed up by default.
-      skipAtlasMetadata:
-        type: boolean
-        description: Skips the backup of the Atlas metadata. Redundant if --skip-backup is included. If this option is not provided, the Atlas metadata is backed up by default.
-      skipRangerAudits:
-        type: boolean
-        description: Skips the backup of the Ranger audits. Redundant if --skip-backup is included. If this option is not provided, Ranger audits are backed up by default.
-      skipBackupValidation:
-        type: boolean
-        description: Skips the validation steps that run prior to the backup. Redundant if --skip-backup is included. If this option is not provided, the validations are performed by default.
-  UpgradeDatalakeResponse:
+      machineUser:
+        $ref: '#/definitions/MachineUser'
+        description: Information about the machine user.
+  ListMachineUsersRequest:
     type: object
-    description: Response object for upgrade datalake request.
+    description: Request object for a list machine users request.
     properties:
-      current:
-        $ref: '#/definitions/ImageInfo'
-        description: Information about the current image
-      upgradeCandidates:
+      machineUserNames:
         type: array
-        description: List of images and components to upgrade to
         items:
-          $ref: '#/definitions/ImageInfo'
-          description: Information about an image
-      reason:
+          type: string
+        description: The machine user names or CRNs of the macihne users. If not provided all machine users for the account are retrieved.
+      pageSize:
+        type: integer
+        format: int32
+        minimum: 1
+        maximum: 100
+        x-paging-page-size: true
+        description: The size of each page.
+      startingToken:
         type: string
-        description: The reason why upgrade is not possible
-  PrepareDatalakeUpgradeRequest:
+        x-paging-input-token: true
+        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
+  ListMachineUsersResponse:
     type: object
-    description: Request object to prepare Data Lake upgrade. This command indicates the upgrade preparation for a specific image or a selected runtime version. Important to note that the imageId or the runtime parameter must be present in the request.
+    description: Response object for a list machine users request.
     required:
-      - datalake
-    properties:
-      datalake:
-        type: string
-        description: The name or CRN of the Data Lake cluster.
-      imageId:
-        type: string
-        description: The ID of an image to upgrade to
-      runtime:
-        type: string
-        description: The runtime version to upgrade to
-  PrepareDatalakeUpgradeResponse:
-    type: object
-    description: Response object for prepare Data Lake upgrade request.
+      - machineUsers
     properties:
-      current:
-        $ref: '#/definitions/ImageInfo'
-        description: Information about the current image
-      upgradeCandidates:
+      machineUsers:
         type: array
-        description: List of images and components to upgrade to
         items:
-          $ref: '#/definitions/ImageInfo'
-          description: Information about an image
-      reason:
+          $ref: '#/definitions/MachineUser'
+        x-paging-result: true
+        description: The machine users.
+      nextToken:
         type: string
-        description: The reason why upgrade is not possible
-  StartDatabaseUpgradeRequest:
+        x-paging-output-token: true
+        description: The token to use when requesting the next set of results. If not present, there are no additional results.
+  DeleteMachineUserRequest:
     type: object
-    description: Request object for Data Lake database upgrade.
+    description: Request object for delete machine user request.
     required:
-      - datalake
+      - machineUserName
     properties:
-      datalake:
-        type: string
-        description: The name or CRN of the Data Lake.
-      targetVersion:
+      machineUserName:
         type: string
-        description: The database engine major version to upgrade to.
-        enum:
-          - VERSION_11
-  StartDatabaseUpgradeResponse:
+        description: The name or CRN of the machine user to delete.
+  DeleteMachineUserResponse:
     type: object
-    description: Response object to Data Lake database upgrade.
-    properties:
-      targetVersion:
-        type: string
-        description: The database engine major version to upgrade to.
-        enum:
-          - VERSION_11
-  DatalakeVmLogRequest:
+    description: Response object for delete machine user request.
+  CreateGroupRequest:
     type: object
-    description: Log descriptor, contains a path and label pair. Used for diagnostics collections.
+    description: Request object for create group request.
     required:
-      - path
-      - label
+      - groupName
     properties:
-      path:
-        type: string
-        description: Path of the log file(s) that needs to be collected. (Can be glob wildcard)
-      label:
+      groupName:
         type: string
-        description: Label that will be used to identify a log descriptor. (will be used as a folder inside logs folder)
-  DatalakeVmLogResponse:
+        description: The name of the group. This name must be unique, must have a maximum of 32 characters, and must contain only alphanumeric characters, "-" and "_". Also, the first character of the name must be alphabetic or an underscore. Names are are not case-sensitive. The group named administrators is reserved.
+      syncMembershipOnUserLogin:
+        x-no-compatibility-guarantee: true
+        type: boolean
+        description: Whether group membership is synced when a user logs in. The default is to sync group membership.
+  CreateGroupResponse:
     type: object
-    description: Log descriptor, contains a path and label pair. Used for diagnostics collections.
+    description: Response object for create group request.
+    required:
+      - group
     properties:
-      path:
-        type: string
-        description: Path of the log file(s) that needs to be collected. (Can be glob wildcard)
-      label:
-        type: string
-        description: Label that will be used to identify a log descriptor. (will be used as a folder inside logs folder)
-  CollectDatalakeDiagnosticsRequest:
+      group:
+        $ref: '#/definitions/Group'
+        description: Information about the group.
+  DeleteGroupRequest:
     type: object
-    description: Request object for collecting DataLake diagnostics.
+    description: Request object for delete group request.
     required:
-      - crn
-      - destination
-      - description
+      - groupName
     properties:
-      crn:
-        type: string
-        description: CRN of the Datalake cluster.
-      destination:
+      groupName:
         type: string
-        enum:
-          - SUPPORT
-          - CLOUD_STORAGE
-          - ENG
-          - LOCAL
-        description: Destination of the diagnostics collection (Support, Own cloud storage, Engineering or collect only on the nodes)
-      description:
-        type: string
-        description: Additional information / title for the diagnostics collection.
-      caseNumber:
-        type: string
-        description: Optional support case number in case of SUPPORT destination, otherwise only act as additional data.
-      labels:
+        description: The name or CRN of the group to delete.
+  DeleteGroupResponse:
+    type: object
+    description: Response object for delete group request.
+  ListGroupsRequest:
+    type: object
+    description: Request object for a list groups request.
+    properties:
+      groupNames:
         type: array
-        description: Array of labels that can filter logs that are collected during diagnostics collection.
-        uniqueItems: true
         items:
           type: string
-      startDate:
-        type: string
-        format: date-time
-        description: Date timestamp - collect files only for diagnostics that has higher last modified timestamp value than this.
-      endDate:
+        description: The group names or CRNs of the groups. If not provided, all groups in the account are retrieved.
+      pageSize:
+        type: integer
+        format: int32
+        minimum: 1
+        maximum: 100
+        x-paging-page-size: true
+        description: The size of each page.
+      startingToken:
         type: string
-        format: date-time
-        description: Date timestamp - collect files only for diagnostics that has lower created timestamp value than this.
-      additionalLogs:
-        type: array
-        description: Array of log descriptors that should be additionally collected during diagnostics collection.
-        items:
-          $ref: '#/definitions/DatalakeVmLogRequest'
-      hosts:
-        type: array
-        description: Array of host names (fqdn), collection will run only on the dedicated hosts.
-        uniqueItems: true
-        items:
-          type: string
-      hostGroups:
-        type: array
-        description: Array of host groups, collection will run only on the dedicated hosts that belongs to these host groups.
-        uniqueItems: true
-        items:
-          type: string
-      excludeHosts:
+        x-paging-input-token: true
+        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
+  ListGroupsResponse:
+    type: object
+    description: Response object for a list groups request.
+    required:
+      - groups
+    properties:
+      groups:
         type: array
-        description: Array of host names (fqdn or IP address), collection will not run on the excluded hosts.
-        uniqueItems: true
         items:
-          type: string
-      skipUnresponsiveHosts:
-        type: boolean
-        description: Skip unhealthy hosts from the diagnostics collection.
-      includeNginxReport:
-        type: boolean
-        description: Include Nginx report generated by GoAccess (if available).
-      includeSaltLogs:
-        type: boolean
-        description: Include salt minion/master/api system logs in the diagnostics collection.
-      includeSarOutput:
-        type: boolean
-        description: Include SAR (System Activity Report) generated outputs in the diagnostics collection (if available).
-      updatePackage:
-        type: boolean
-        default: false
-        description: If enabled, required package (cdp-telemetry) will be upgraded or installed on the nodes. (useful if package is not installed or needs to be upgraded) Network is required for this operation.
-      storageValidation:
-        type: boolean
-        default: false
-        description: Enable/disable node level storage validation (can be disabled for example, if you have too many hosts and do not want to do too much parallel writes to s3/abfs)
-  CollectDatalakeDiagnosticsResponse:
-    type: object
-    description: Response object for collecting DataLake diagnostics.
-  ListDatalakeDiagnosticsRequest:
+          $ref: '#/definitions/Group'
+        x-paging-result: true
+        description: The list of groups.
+      nextToken:
+        type: string
+        x-paging-output-token: true
+        description: The token to use when requesting the next set of results. If not present, there are no additional results.
+  UpdateGroupRequest:
     type: object
-    description: Request object for listing recent Datalake diagnostics collections.
+    description: Request object for update group request.
+    x-no-compatibility-guarantee: true
     required:
-      - crn
+      - groupName
     properties:
-      crn:
+      groupName:
         type: string
-        description: CRN of the Datalake cluster.
-  ListDatalakeDiagnosticsResponse:
+        description: The name or CRN of the group to update.
+      syncMembershipOnUserLogin:
+        type: boolean
+        description: Whether group membership is synced when a user logs in. Can be omitted if no update is required.
+  UpdateGroupResponse:
     type: object
-    description: Response object for listing recent Datalake diagnostics collections.
+    description: Response object for update group request.
+    x-no-compatibility-guarantee: true
+    required:
+      - group
     properties:
-      collections:
-        type: array
-        description: description.
-        items:
-          $ref: '#/definitions/DatalakeDiagnosticsCollectionResponse'
-  DatalakeDiagnosticsCollectionResponse:
+      group:
+        $ref: '#/definitions/Group'
+        description: Information about the updated group.
+  AddUserToGroupRequest:
     type: object
-    description: Response object for diagnostic collection flow details.
+    description: Request object for an add user to group request.
+    required:
+      - userId
+      - groupName
     properties:
-      status:
-        type: string
-        description: Status of the diagnostics collection flow.
-        enum:
-          - RUNNING
-          - FAILED
-          - FINISHED
-          - CANCELLED
-      flowId:
-        type: string
-        description: Flow ID of the diagnostics collection flow.
-      flowState:
+      userId:
         type: string
-        description: Current state of the diagnostics collection flow.
-      created:
+        description: The ID or CRN of the user to add to the group.
+      groupName:
         type: string
-        format: date-time
-        description: Creation date of the diagnostics collection flow.
-      progressPercentage:
-        type: integer
-        description: Progress percentage of the diagnostics collection flow (maximum value if finished).
-        format: int32
-      collectionDetails:
-        $ref: '#/definitions/DatalakeDiagnosticsCollectionDetailsResponse'
-        description: Additional details about the diagnostics collection.
-  DatalakeDiagnosticsCollectionDetailsResponse:
+        description: The name or CRN of the group to add the user to.
+  AddUserToGroupResponse:
+    type: object
+    description: Response object for an add user to group request.
+  AddMachineUserToGroupRequest:
     type: object
-    description: Response object for diagnostic collection collection details.
+    description: Request object for an add machine user to group request.
+    required:
+      - machineUserName
+      - groupName
     properties:
-      case:
-        type: string
-        description: Case number for the diagnostics collection.
-      output:
+      machineUserName:
         type: string
-        description: Output destination of the diagnostics collection.
-      destination:
+        description: The name or CRN of the machine user to add to the group.
+      groupName:
         type: string
-        description: Destination type of the diagnostics collection.
-      description:
-        type: string
-        description: Description of the diagnostics collection.
-      accountId:
-        type: string
-        description: Account Id that was used for the diagnostics collection.
-      resourceCrn:
-        type: string
-        description: Crn of the cluster.
-      clusterVersion:
-        type: string
-        description: Version of the cluster that was used for the diagnostics collection.
-  CancelDatalakeDiagnosticsRequest:
+        description: The name or CRN of the group to add the machine user to.
+  AddMachineUserToGroupResponse:
+    type: object
+    description: Response object for add machine user to group request.
+  RemoveUserFromGroupRequest:
     type: object
-    description: Request object for cancel running Datalake diagnostics collections.
+    description: Request object for a remove user from group request.
     required:
-      - crn
+      - userId
+      - groupName
     properties:
-      crn:
+      userId:
+        type: string
+        description: The ID or CRN of the user to remove from the group.
+      groupName:
         type: string
-        description: CRN of the Datalake cluster.
-  CancelDatalakeDiagnosticsResponse:
+        description: The name or CRN of the group to remove the user from.
+  RemoveUserFromGroupResponse:
     type: object
-    description: Response object for cancel running Datalake diagnostics collections.
-  CollectCmDiagnosticsRequest:
+    description: Response object for a remove user from group request.
+  RemoveMachineUserFromGroupRequest:
     type: object
-    description: Request object for collecting DataLake diagnostics.
+    description: Request object for a remove machine user from group request.
     required:
-      - crn
-      - destination
+      - machineUserName
+      - groupName
     properties:
-      crn:
+      machineUserName:
         type: string
-        description: CRN of the Datalake cluster.
-      destination:
+        description: The name or CRN of the machine user to add to the group.
+      groupName:
         type: string
-        enum:
-          - SUPPORT
-          - CLOUD_STORAGE
-          - LOCAL
-        description: Destination of the diagnostics collection (Support, Own cloud storage, Engineering or collect only on the nodes)
-      description:
+        description: The name or CRN of the group to remove the machine user from.
+  RemoveMachineUserFromGroupResponse:
+    type: object
+    description: Response object for a remove machine user from group request.
+  ListGroupMembersRequest:
+    type: object
+    description: Request object for a list group members request.
+    required:
+      - groupName
+    properties:
+      groupName:
         type: string
-        description: Additional information / title for the diagnostics collection.
-      caseNumber:
+        description: The name or CRN of the group to list the membership of.
+      pageSize:
+        type: integer
+        format: int32
+        minimum: 1
+        maximum: 100
+        x-paging-page-size: true
+        description: The size of each page.
+      startingToken:
         type: string
-        description: Optional support case number in case of SUPPORT destination, otherwise only act as additional data.
-      roles:
+        x-paging-input-token: true
+        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
+  ListGroupMembersResponse:
+    type: object
+    description: Response object for a list group members request.
+    required:
+      - memberCrns
+    properties:
+      memberCrns:
         type: array
-        description: Array of roles for which to get logs and metrics. If set, this restricts the roles for log and metrics collection.
-        uniqueItems: true
         items:
           type: string
-      startDate:
-        type: string
-        format: date-time
-        description: Restrict collected logs and metrics (from the provided date timestamp).
-      endDate:
+        description: The list of group members.
+        x-paging-result: true
+      nextToken:
         type: string
-        format: date-time
-        description: Restrict collected logs and metrics (until the provided date timestamp).
-      updatePackage:
-        type: boolean
-        default: false
-        description: If enabled, required package (cdp-telemetry) will be upgraded or installed on the nodes. (useful if package is not installed or needs to be upgraded) Network is required for this operation.
-      storageValidation:
-        type: boolean
-        default: false
-        description: Enable/disable node level storage validation (can be disabled for example, if you have too many hosts and do not want to do too much parallel writes to s3/abfs)
-      monitorMetricsCollection:
-        type: boolean
-        default: false
-        description: Flag to enable collection of metrics for chart display in CM based diagnostics collection.
-      bundleSizeLimit:
-        type: integer
-        format: int32
-        description: Diagnostics bundle size limit in MB.
-  CollectCmDiagnosticsResponse:
-    type: object
-    description: Response object for collecting DataLake diagnostics.
-  GetCmRolesRequest:
+        x-paging-output-token: true
+        description: The token to use when requesting the next set of results. If not present, there are no additional results.
+  ListGroupsForUserRequest:
     type: object
-    description: Request object for obtaining Cloudera Manger roles. (that can be used for filtering in CM based diagnostics collection)
+    description: Request object for a list groups for user request.
     required:
-      - crn
+      - userId
     properties:
-      crn:
+      userId:
+        type: string
+        description: The ID or CRN of the user to list the groups of.
+      pageSize:
+        type: integer
+        format: int32
+        minimum: 1
+        maximum: 100
+        x-paging-page-size: true
+        description: The size of each page.
+      startingToken:
         type: string
-        description: CRN of the Datalake cluster.
-  GetCmRolesResponse:
+        x-paging-input-token: true
+        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
+  ListGroupsForUserResponse:
     type: object
-    description: Response object for obtaining Cloudera Manger roles. (that can be used for filtering in CM based diagnostics collection)
+    description: Response object for a list groups for user request.
+    required:
+      - groupCrns
     properties:
-      roles:
+      groupCrns:
         type: array
-        description: Array of CM roles. (useful for CM based diagnostics collection filtering)
         items:
           type: string
-  GetDatalakeLogDescriptorsRequest:
+        x-paging-result: true
+        description: The list of groups.
+      nextToken:
+        type: string
+        x-paging-output-token: true
+        description: The token to use when requesting the next set of results. If not present, there are no additional results.
+  ListGroupsForMachineUserRequest:
     type: object
-    description: Request object for obtaining log descriptors. (that are used for diagnostics collection)
-  GetDatalakeLogDescriptorsResponse:
+    description: Request object for a list groups for machine user request.
+    required:
+      - machineUserName
+    properties:
+      machineUserName:
+        type: string
+        description: The name or CRN of the machine user to list the groups of.
+      pageSize:
+        type: integer
+        format: int32
+        minimum: 1
+        maximum: 100
+        x-paging-page-size: true
+        description: The size of each page.
+      startingToken:
+        type: string
+        x-paging-input-token: true
+        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
+  ListGroupsForMachineUserResponse:
     type: object
-    description: Response object for obtaining log descriptors. (useful for diagnostics collection filtering)
+    description: Response object for a list groups for machine user request.
+    required:
+      - groupCrns
     properties:
-      logs:
+      groupCrns:
         type: array
-        description: Array of log descriptors. (useful for diagnostics collection filtering)
         items:
-          $ref: '#/definitions/DatalakeVmLogResponse'
-  RotateAutoTlsCertificatesRequest:
+          type: string
+        x-paging-result: true
+        description: The list of groups.
+      nextToken:
+        type: string
+        x-paging-output-token: true
+        description: The token to use when requesting the next set of results. If not present, there are no additional results.
+  AssignGroupRoleRequest:
     type: object
-    description: Request object to rotate autotls certificates on datalake's hosts, deprecated.
-    x-deprecated: true
+    description: Request object for an assign group role request.
     required:
-      - datalakeName
+      - groupName
+      - role
     properties:
-      datalakeName:
+      groupName:
         type: string
-        description: The name or CRN of the datalake.
-  RotateAutoTlsCertificatesResponse:
-    type: object
-    description: Response object to rotate autotls certificates on datalake's hosts, deprecated.
-    x-deprecated: true
-  RenewCertificateResponse:
+        description: The group to which the role is assigned to. Can be the group name or CRN.
+      role:
+        type: string
+        description: The role being assigned to the group. Can be the role's CRN or name.
+  AssignGroupRoleResponse:
     type: object
-    description: Response object for renew certificate request, deprecated.
-    x-deprecated: true
-  ImageRequest:
-    description: The image request for the datalake. This must not be set if the runtime parameter is provided. The image ID parameter is required if this is present, but the image catalog name is optional, defaulting to 'cdp-default' if not present.
+    description: Response object for an assign group role request.
+  UnassignGroupRoleRequest:
     type: object
+    description: Request object for an unassign group role request.
     required:
-      - id
+      - groupName
+      - role
     properties:
-      id:
+      groupName:
         type: string
-        description: The image ID from the catalog. The corresponding image will be used for the created cluster machines.
-      catalogName:
+        description: The group to unassign the role from. Can be the group name or CRN.
+      role:
         type: string
-        description: The name of the custom image catalog to use.
-        default: cdp-default
-  ResizeDatalakeRequest:
+        description: The role to unassign from the group. Can be the role's CRN or name.
+  UnassignGroupRoleResponse:
     type: object
-    description: Datalake resize request.
+    description: Response object for an unassign group role request.
+  AssignGroupResourceRoleRequest:
+    type: object
+    description: Request object for an assign group resource role request.
     required:
-      - datalakeName
-      - targetSize
+      - groupName
+      - resourceRoleCrn
+      - resourceCrn
     properties:
-      datalakeName:
+      groupName:
         type: string
-        description: The name or CRN of the datalake.
-      targetSize:
+        description: The group to assign the resource role to. Can be the group's name or CRN.
+      resourceRoleCrn:
         type: string
-        description: The target size for the datalake.
-        enum:
-          - MEDIUM_DUTY_HA
-  ResizeDatalakeResponse:
+        description: The CRN of the resource role being assigned to the group.
+      resourceCrn:
+        type: string
+        description: The resource for which the resource role rights are granted.
+  AssignGroupResourceRoleResponse:
+    type: object
+    description: Response object for an assign group resource role request.
+  UnassignGroupResourceRoleRequest:
     type: object
-    description: Datalake resize response.
+    description: Request object for an unassign group resource role request.
+    required:
+      - groupName
+      - resourceRoleCrn
+      - resourceCrn
     properties:
-      datalakeName:
+      groupName:
         type: string
-        description: The name of the datalake. This will remain the same for the datalake created by the resize process.
-      datalakeCrn:
+        description: The group to unassign the resource role from.
+      resourceRoleCrn:
         type: string
-        description: The CRN of the datalake. This will remain the same for the datalake created by the resize process.
-      environmentCrn:
-        type: string
-        description: The CRN of the environment the datalake is attached to. This will remain the same for the datalake created by the resize process.
-      runtime:
-        type: string
-        description: The runtime of the datalake. This will remain the same for the datalake created by the resize process.
-      status:
-        type: string
-        description: The current status of the datalake.
-      statusReason:
-        type: string
-        description: The reason for the current status of the datalake.
-      cloudbreakVersion:
+        description: The CRN of the resource role to unassign from the group.
+      resourceCrn:
         type: string
-        description: The Cloudbreak version used to create the data lake.
-  ReplaceRecipesRequest:
+        description: The CRN of the resource for which the resource role rights will be unassigned.
+  UnassignGroupResourceRoleResponse:
     type: object
-    description: The request for replacing recipes.
-    required:
-      - datalake
-      - instanceGroupRecipes
-    properties:
-      datalake:
-        type: string
-        description: The name or CRN of the datalake.
-      instanceGroupRecipes:
-        type: array
-        items:
-          $ref: '#/definitions/InstanceGroupRecipeRequest'
-        description: The list of instance group and recipe name pairs.
-  ReplaceRecipesResponse:
+    description: Response object for an unassign group role request.
+  ListGroupAssignedRolesRequest:
     type: object
-    description: The response for replacing recipes.
-    properties:
-      attachedRecipes:
-        type: array
-        description: The list of recipes, which will be attached to the cluster.
-        items:
-          $ref: '#/definitions/InstanceGroupRecipeResponse'
-      detachedRecipes:
-        type: array
-        description: The list of recipes, which will be detached from the cluster.
-        items:
-          $ref: '#/definitions/InstanceGroupRecipeResponse'
-  InstanceGroupRecipeRequest:
-    type: object
-    description: Represents an instance group - recipe pair (by names) request.
+    description: Request object for a list group assigned roles request.
     required:
-      - instanceGroupName
+      - groupName
     properties:
-      instanceGroupName:
+      groupName:
         type: string
-        description: A valid instance/host group name. This name must be unique.
-      recipeNames:
-        type: array
-        uniqueItems: true
-        items:
-          type: string
-        description: Names of the recipes (empty is valid).
-  InstanceGroupRecipeResponse:
+        description: The group to list the assigned roles for. Can be the group's name or CRN.
+      pageSize:
+        type: integer
+        format: int32
+        minimum: 1
+        maximum: 100
+        x-paging-page-size: true
+        description: The size of each page.
+      startingToken:
+        type: string
+        x-paging-input-token: true
+        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
+  ListGroupAssignedRolesResponse:
     type: object
-    description: Represents an instance group - recipe pair (by names) response.
+    description: Response object for a list group assigned roles request.
     required:
-      - instanceGroupName
+      - roleCrns
     properties:
-      instanceGroupName:
-        type: string
-        description: A valid instance/host group name. This name must be unique.
-      recipeNames:
+      roleCrns:
         type: array
-        uniqueItems: true
         items:
           type: string
-        description: Names of the recipes (empty is valid).
-  RecoverDatalakeRequest:
+        x-paging-result: true
+        description: The role CRNs assigned to the group.
+      nextToken:
+        type: string
+        x-paging-output-token: true
+        description: The token to use when requesting the next set of results. If not present, there are no additional results.
+  ListGroupAssignedResourceRolesRequest:
     type: object
-    description: Datalake recover request.
+    description: Request object for a list group assigned resource roles request.
     required:
-      - datalakeName
+      - groupName
     properties:
-      datalakeName:
+      groupName:
         type: string
-        description: The name or CRN of the datalake.
-      recoveryType:
+        description: The group to list the assigned resource roles for. Can be the group's name or CRN.
+      pageSize:
+        type: integer
+        format: int32
+        minimum: 1
+        maximum: 100
+        x-paging-page-size: true
+        description: The size of each page.
+      startingToken:
         type: string
-        description: The type of the recovery. The default value is RECOVER_WITHOUT_DATA. The recovery always runs with RECOVER_WITH_DATA if the on resize failure.
-        enum:
-          - RECOVER_WITH_DATA
-          - RECOVER_WITHOUT_DATA
-  RecoverDatalakeResponse:
-    type: object
-    description: Datalake recover response.
-  SetCatalogRequest:
+        x-paging-input-token: true
+        description: A token to specify where to start paginating. This is the nextToken from a previously truncated response.
+  ListGroupAssignedResourceRolesResponse:
     type: object
-    description: The request object to set catalog for a DataLake.
+    description: Response object for a list group assigned resource roles request.
     required:
-      - datalake
-      - catalogName
+      - resourceAssignments
     properties:
-      datalake:
-        type: string
-        description: The name or CRN of the affected DataLake.
-      catalogName:
+      resourceAssignments:
+        type: array
+        items:
+          $ref: '#/definitions/ResourceAssignment'
+        x-paging-result: true
+        description: The group's resource assignments.
+      nextToken:
         type: string
-        description: The name of the catalog to be used.
-  SetCatalogResponse:
+        x-paging-output-token: true
+        description: The token to use when requesting the next set of results. If not present, there are no additional results.
+  EnableClouderaSSOLoginRequest:
     type: object
-    description: The response object to set catalog for a DataLake request.
-  SyncComponentVersionsFromCmRequest:
+    description: Request object for an enable Cloudera SSO login request.
     x-no-compatibility-guarantee: true
+  EnableClouderaSSOLoginResponse:
     type: object
-    description: Datalake sync CM component versions request.
-    required:
-      - datalakeName
-    properties:
-      datalakeName:
-        type: string
-        description: The name or CRN of the datalake.
-  SyncComponentVersionsFromCmResponse:
+    description: Response object for an enable Cloudera SSO login request.
+    x-no-compatibility-guarantee: true
+  DisableClouderaSSOLoginRequest:
+    type: object
+    description: Request object for a disable Cloudera SSO login request.
     x-no-compatibility-guarantee: true
+  DisableClouderaSSOLoginResponse:
     type: object
-    description: Datalake sync CM component versions response.
-  RotatePrivateCertificatesRequest:
+    description: Response object for a disable Cloudera SSO login request.
+    x-no-compatibility-guarantee: true
+  GetAccountRequest:
+    type: object
+    description: Request object for a get account request.
+    x-no-compatibility-guarantee: true
+  GetAccountResponse:
     type: object
-    description: Request object to rotate private certificates on datalake's hosts.
+    description: Response object for a get account response.
+    x-no-compatibility-guarantee: true
     required:
-      - datalake
+      - account
     properties:
-      datalake:
-        type: string
-        description: The name or CRN of the datalake.
-  RotatePrivateCertificatesResponse:
-    type: object
-    description: Response object to rotate private certificates on datalake's hosts.
-  RenewPublicCertificateRequest:
+      account:
+        $ref: '#/definitions/Account'
+        description: The account object.
+  CreateUserRequest:
     type: object
-    description: Request object to renew the public certificate for Datalake.
+    description: Request object for creating user request.
+    x-no-compatibility-guarantee: true
     required:
-      - datalake
+      - samlProviderName
+      - identityProviderUserId
+      - email
     properties:
-      datalake:
+      samlProviderName:
+        type: string
+        description: The name or CRN of the SAML provider the user will use for login.
+      identityProviderUserId:
+        type: string
+        description: The identity provider user id for the user. This ID must match the NameId attribute value that will be passed for the user in the SAML response using the associated SAML provider.
+      email:
         type: string
-        description: The name or CRN of the datalake.
-  RenewPublicCertificateResponse:
+        description: The email address for the user. Used for display purposes only.
+      groups:
+        type: array
+        items:
+          type: string
+        description: The list of groups the user belongs to. The groups will be created if they do not exist.
+      firstName:
+        type: string
+        description: The user first name.
+      lastName:
+        type: string
+        description: The user last name.
+  CreateUserResponse:
     type: object
-    description: Response object for renew public certificate request.
-  RotateSaltPasswordRequest:
+    description: Response object for a create user request.
+    x-no-compatibility-guarantee: true
+    required:
+      - user
+    properties:
+      user:
+        $ref: '#/definitions/User'
+        description: Information about the user.
+  SetWorkloadPasswordRequest:
     type: object
-    description: Request object for rotating SaltStack user password on DataLake instances.
+    description: Request object for a set workload password request.
     required:
-      - datalake
+      - password
     properties:
-      datalake:
+      password:
         type: string
-        description: The name or CRN of the datalake.
-  RotateSaltPasswordResponse:
+        description: The password value to set
+        x-sensitive: true
+  SetWorkloadPasswordResponse:
     type: object
-    description: Response object for rotating SaltStack user password on DataLake instances.
-  UpdateOrchestratorStateRequest:
+    description: Response object for a set workload password request.
+  SetWorkloadPasswordPolicyRequest:
     type: object
-    description: Request object for running orchestrator engine state update on the Data Lake cluster.
-    required:
-      - clusterCrn
+    description: Request object for a set workload password policy request.
+    x-no-compatibility-guarantee: true
     properties:
-      clusterCrn:
-        type: string
-        description: The CRN of the Data Lake cluster.
-  UpdateOrchestratorStateResponse:
+      maxPasswordLifetimeDays:
+        type: integer
+        format: int32
+        minimum: 0
+        description: The max lifetime of passwords, in days. If set to '0' passwords never expires.
+  SetWorkloadPasswordPolicyResponse:
     type: object
-    description: Response object for running orchestrator engine state update on the Data Lake cluster.
+    description: Response object for a set workload password policy request.
+    x-no-compatibility-guarantee: true
```

### Comparing `cdpcli-0.9.89/cdpcli/data/de/de.yaml` & `cdpcli-0.9.9/cdpcli/data/ml/ml.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,254 +1,221 @@
+x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
-x-endpoint-name: de
+x-endpoint-name: ml
 x-products: CDP
-x-form-factors: public,private
 x-cdp-releases: PUBLIC
-x-audit: true
 info:
-  version: 0.9.89
-  title: Cloudera Data Engineering
+  version: 0.1-SNAPSHOT
+  title: Cloudera Machine Learning
   license:
     name: Apache 2.0
-  description: Create and manage Cloudera Data Engineering Services.
-  termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
+  description: Install and manage Cloudera Machine Learning applications.
 schemes:
   - https
 consumes:
   - application/json
 produces:
   - application/json
 paths:
-  /api/v1/de/createVc:
+  /api/v1/ml/createWorkspace:
     post:
-      summary: Create Virtual Cluster
-      description: Creates a virtual cluster and returns creation response.
-      operationId: createVc
-      x-mutating: true
+      summary: Create a Cloudera Machine Learning workspace.
+      description: Provision a Kubernetes cluster and install the Cloudera Machine Learning application in it.
+      operationId: createWorkspace
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/CreateVcRequest'
+            $ref: '#/definitions/CreateWorkspaceRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/CreateVcResponse'
+            $ref: '#/definitions/CreateWorkspaceResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/de/deleteVc:
+  /api/v1/ml/deleteWorkspace:
     post:
-      summary: Delete Virtual Cluster
-      description: Deletes a virtual cluster and returns deletion response.
-      operationId: deleteVc
-      x-mutating: true
+      summary: Delete Cloudera Machine Learning Workspace.
+      description: Deletes a Cloudera Machine Learning workspace.
+      operationId: deleteWorkspace
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/DeleteVcRequest'
+            $ref: '#/definitions/DeleteWorkspaceRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/DeleteVcResponse'
+            $ref: '#/definitions/DeleteWorkspaceResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/de/updateVc:
+  /api/v1/ml/describeWorkspace:
     post:
-      summary: Update Cloudera Data Engineering (CDE) Virtual Cluster
-      description: Updates Cloudera Data Engineering (CDE) Virtual Cluster and returns details of updated CDE service.
-      operationId: updateVc
-      x-mutating: true
+      summary: Describe Cloudera Machine Learning Workspace.
+      description: Describes a Cloudera Machine Learning workspace.
+      operationId: describeWorkspace
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/UpdateVcRequest'
+            $ref: '#/definitions/DescribeWorkspaceRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/UpdateVcResponse'
+            $ref: '#/definitions/DescribeWorkspaceResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/de/describeService:
+  /api/v1/ml/getAuditEvents:
     post:
-      summary: Describe Cloudera Data Engineering(CDE) Service
-      description: Returns details of CDE service.
-      operationId: describeService
-      x-mutating: false
+      summary: Gets all the events belong to a workspace crn.
+      description: Gets all the events belong to a workspace crn.
+      operationId: getAuditEvents
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/DescribeServiceRequest'
+            $ref: '#/definitions/GetAuditEventsRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/DescribeServiceResponse'
+            $ref: '#/definitions/GetAuditEventsResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/de/describeVc:
+  /api/v1/ml/getLatestWorkspaceVersion:
     post:
-      summary: Describe Virtual Cluster
-      description: Returns a description for the specified virtual cluster.
-      operationId: describeVc
-      x-mutating: false
+      summary: GetLatestWorkspaceVersion Cloudera Machine Learning Workspace.
+      description: Retrieves the latest version that Cloudera Machine Learning deploys to workspaces.
+      operationId: getLatestWorkspaceVersion
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/DescribeVcRequest'
+            $ref: '#/definitions/GetLatestWorkspaceVersionRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/DescribeVcResponse'
+            $ref: '#/definitions/GetLatestWorkspaceVersionResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/de/disableService:
+  /api/v1/ml/getLogs:
     post:
-      summary: Disable Cloudera Data Engineering(CDE) Service
-      description: Returns delete response.
-      operationId: disableService
-      x-mutating: true
+      summary: Gets all the logs belong to a request id.
+      description: Gets all the logs belong to a request id.
+      operationId: getLogs
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/DisableServiceRequest'
+            $ref: '#/definitions/GetLogsRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/DisableServiceResponse'
+            $ref: '#/definitions/GetLogsResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/de/enableService:
+  /api/v1/ml/grantWorkspaceAccess:
     post:
-      summary: Enable Cloudera Data Engineering(CDE) Service
-      description: Returns enabling response.
-      operationId: enableService
-      x-mutating: true
+      summary: GrantWorkspaceAccess Cloudera Machine Learning Workspace.
+      description: Grants an AWS user to perform Kubernetes operations on a Cloudera Machine Learning workspace via EKS.
+      operationId: grantWorkspaceAccess
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/EnableServiceRequest'
+            $ref: '#/definitions/GrantWorkspaceAccessRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/EnableServiceResponse'
+            $ref: '#/definitions/GrantWorkspaceAccessResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/de/updateService:
+  /api/v1/ml/listWorkspaces:
     post:
-      summary: Update Cloudera Data Engineering (CDE) Service
-      description: Returns update response consisting of operation ID that can be used to log update events.
-      operationId: updateService
-      x-mutating: true
+      summary: List Cloudera Machine Learning workspaces.
+      description: List Cloudera Machine Learning workspaces.
+      operationId: listWorkspaces
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/UpdateServiceRequest'
+            $ref: '#/definitions/ListWorkspacesRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/UpdateServiceResponse'
+            $ref: '#/definitions/ListWorkspacesResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/de/getKubeconfig:
+  /api/v1/ml/revokeWorkspaceAccess:
     post:
-      summary: Get Kubeconfig for the CDE service
-      description: Returns kubeconfig.
-      operationId: getKubeconfig
-      x-mutating: false
+      summary: RevokeWorkspaceAccess Cloudera Machine Learning Workspace.
+      description: Revokes an AWS user to perform Kubernetes operations on a Cloudera Machine Learning workspace via EKS.
+      operationId: revokeWorkspaceAccess
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/GetKubeconfigRequest'
+            $ref: '#/definitions/RevokeWorkspaceAccessRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/GetKubeconfigResponse'
+            $ref: '#/definitions/RevokeWorkspaceAccessResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/de/listServices:
+  /api/v1/ml/upgradeWorkspace:
     post:
-      summary: List Cloudera Data Engineering(CDE) Services
-      description: Returns list of cde services.
-      operationId: listServices
-      x-mutating: false
+      summary: Upgrade Cloudera Machine Learning workspace.
+      description: Upgrades a Cloudera Machine Learning workspace to the latest available version.
+      operationId: upgradeWorkspace
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/ListServicesRequest'
+            $ref: '#/definitions/UpgradeWorkspaceRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ListServicesResponse'
-        default:
-          description: The default response on an error.
-          schema:
-            $ref: '#/definitions/Error'
-  /api/v1/de/listVcs:
-    post:
-      summary: List Virtual Clusters
-      description: Returns a list of virtual clusters for a given CDE service.
-      operationId: listVcs
-      x-mutating: false
-      parameters:
-        - name: input
-          in: body
-          required: true
-          schema:
-            $ref: '#/definitions/ListVcsRequest'
-      responses:
-        200:
-          description: Expected response to a valid request.
-          schema:
-            $ref: '#/definitions/ListVcsResponse'
+            $ref: '#/definitions/UpgradeWorkspaceResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
 definitions:
   Error:
     type: object
@@ -256,722 +223,662 @@
     properties:
       code:
         type: string
         description: The error code.
       message:
         type: string
         description: The error message.
-  ServiceSummary:
+  RootVolume:
     type: object
-    description: Summary of a CDE service.
+    description: Configuration for instance root device volume
     required:
-      - name
-      - clusterId
-      - environmentName
-      - status
+      - size
     properties:
-      name:
-        type: string
-        description: Name of the CDE Service.
-      clusterId:
-        type: string
-        description: Cluster Id of the CDE Service.
-      environmentName:
-        type: string
-        description: CDP Environment Name.
-      status:
-        type: string
-        description: Status of the CDE service.
-      creatorEmail:
-        type: string
-        description: Email Address of the CDE creator.
-      enablingTime:
-        type: string
-        description: Timestamp of service enabling.
-  ServiceDescription:
+      size:
+        type: integer
+        format: int64
+        description: The volume size in GB.
+  GetLogsRequest:
     type: object
-    description: Detailed description of a CDE service.
+    description: GetLogsRequestfor getting logs for a request ID.
     required:
-      - name
-      - clusterId
-      - environmentName
+      - workspaceCrn
+      - requestID
     properties:
-      name:
-        type: string
-        description: Name of the CDE Service.
-      clusterId:
-        type: string
-        description: Cluster Id of the CDE Service.
-      environmentName:
-        type: string
-        description: CDP Environment Name.
-      environmentCrn:
-        type: string
-        description: CRN of the environment.
-      tenantId:
-        type: string
-        description: CDP tenant ID.
-      resources:
-        description: Resources details of CDE Service.
-        $ref: '#/definitions/ServiceResources'
-      status:
-        type: string
-        description: Status of the CDE service.
-      creatorEmail:
-        type: string
-        description: Email address of the creator of the CDE service.
-      creatorCrn:
-        type: string
-        description: CRN of the creator.
-      enablingTime:
-        type: string
-        description: Timestamp of service enabling.
-      clusterFqdn:
-        type: string
-        description: FQDN of the CDE service.
-      cloudPlatform:
-        type: string
-        description: The cloud platform where the CDE service is enabled.
-      dataLakeFileSystems:
-        type: string
-        description: The Data lake file system.
-      logLocation:
-        type: string
-        description: Location for the log files of jobs.
-      dataLakeAtlasUIEndpoint:
-        type: string
-        description: Endpoint of Data Lake Atlas.
-      chartValueOverrides:
-        type: array
-        items:
-          $ref: '#/definitions/ChartValueOverridesResponse'
-        description: Chart overrides for the Virtual Cluster.
-      whitelistIps:
-        type: string
-        description: List of CIDRs that would be allowed to access kubernetes master API server.
-      loadbalancerAllowlist:
+      workspaceCrn:
         type: string
-        description: Comma-separated CIDRs that would be allowed to access the load balancer.
-      subnets:
+        description: WorkspaceCrn the requestID belongs to.
+      requestID:
         type: string
-        description: List of Subnet IDs of the CDP subnets used by the kubernetes worker node.
-      privateClusterEnabled:
-        type: boolean
-        description: If true, the CDE service was created with fully private Azure services (AKS, MySQL, etc.).
-      publicEndpointEnabled:
-        type: boolean
-        description: If true, the CDE endpoint was created in a publicly accessible subnet.
-      previousVersionDeployed:
+        description: Unique Key to identify a set of logs.
+      fetchAll:
         type: boolean
-        description: The "true" value indicates that the previous version of the CDE service was requested to be deployed.
-      workloadAnalyticsEnabled:
-        type: boolean
-        description: If true, diagnostic information about job and query execution is sent to Cloudera Workload Manager.
-      ssdUsed:
-        type: boolean
-        description: If true, SSD would have been be used for workload filesystem.
-  ServiceResources:
-    type: object
-    description: Object to store resources for a CDE service.
-    properties:
-      instance_type:
-        type: string
-        description: Instance type of the CDE service.
-      min_instances:
-        type: string
-        description: Minimum Instances for the CDE service.
-      max_instances:
-        type: string
-        description: Maximum instances for the CDE service.
-      initial_instances:
-        type: string
-        description: Initial instances for the CDE service.
-      min_spot_instances:
-        type: string
-        description: Minimum number of spot instances for the CDE service.
-      max_spot_instances:
-        type: string
-        description: Maximum Number of Spot instances.
-      initial_spot_instances:
-        type: string
-        description: Initial Spot Instances for the CDE Service.
-      root_vol_size:
-        type: string
-        description: Root Volume Size.
-  VcSummary:
+        description: Flag to fetch all logs.
+      pageSize:
+        type: integer
+        format: int32
+        description: Limit the number of logs.
+      offset:
+        type: integer
+        format: int32
+        description: offset from which the logs should be fetched.
+  GetLogsResponse:
     type: object
-    description: CDE virtual cluster summary.
+    description: GetLogsResponse contains all the logs for a given request id.
     required:
-      - vcId
-      - vcName
-      - clusterId
+      - auditLogs
     properties:
-      vcId:
-        type: string
-        description: Virtual Cluster ID.
-      vcName:
-        type: string
-        description: Name of the CDE Virtual Cluster.
-      clusterId:
-        type: string
-        description: Cluster ID of the CDE service that contains the virtual cluster.
-      status:
-        type: string
-        description: Status of the Virtual Cluster.
-      VcUiUrl:
-        type: string
-        description: Url for the Virtual Cluster UI.
-      creatorEmail:
-        type: string
-        description: Email Address of the Creator.
-      creatorName:
-        type: string
-        description: Name of the Creator.
-  VcDescription:
+      auditLogs:
+        description: Contains all the logs for a given request id.
+        $ref: '#/definitions/AuditLogs'
+  AuditLogs:
     type: object
-    description: CDE virtual cluster summary.
+    description: AuditLogs contains all the logs for a given request id.
     required:
-      - vcId
-      - vcName
-      - clusterId
+      - requestID
+      - count
+      - logs
     properties:
-      vcId:
-        type: string
-        description: Virtual Cluster ID.
-      vcName:
-        type: string
-        description: Name of the CDE Virtual Cluster.
-      clusterId:
-        type: string
-        description: Cluster ID of the CDE service that contains the Virtual Cluster.
-      status:
-        type: string
-        description: Status of the Virtual Cluster.
-      resources:
-        description: Resources details of CDE Service.
-        $ref: '#/definitions/VcResources'
-      creatorEmail:
-        type: string
-        description: Email address of the creator of Virtual Cluster.
-      creatorID:
-        type: string
-        description: ID of the creator of Virtual Cluster.
-      creatorName:
-        type: string
-        description: Name of the creator of the Virtual Cluster.
-      vcApiUrl:
-        type: string
-        description: Url for the Virtual Cluster APIs.
-      VcUiUrl:
+      requestID:
         type: string
-        description: URL of the CDE Virtual Cluster UI.
-      historyServerUrl:
-        type: string
-        description: Spark History Server URL for the Virtual Cluster.
-      livyServerUrl:
-        type: string
-        description: Livy Server URL for the Virtual Cluster.
-      safariUrl:
-        type: string
-        description: Safari URL for the Virtual Cluster.
-      creationTime:
-        type: string
-        description: Time of creation of the virtual Cluster.
-      sparkVersion:
-        type: string
-        description: Spark version for the virtual cluster.
-      chartValueOverrides:
+        description: The request ID associated with a long-running operation to fetch the logs for.
+      count:
+        type: integer
+        format: int32
+        description: Total number of logs associated with the request id.
+      logs:
         type: array
         items:
-          $ref: '#/definitions/ChartValueOverridesResponse'
-        description: Chart overrides for the Virtual Cluster.
-      accessControl:
-        description: Access control object for the Virtual Cluster.
-        $ref: '#/definitions/AccessControlResponse'
-      smtpConfig:
-        description: SMTP Configurations for Airflow Email Alerts.
-        $ref: '#/definitions/SmtpConfigResponse'
-      vcTier:
-        type: string
-        description: Tier of the Virtual Cluster.
-  VcResources:
+          $ref: '#/definitions/AuditLog'
+        description: Contains all the logs for a given request id.
+  AuditLog:
     type: object
+    description: Audit log represents an individual log.
+    required:
+      - createdDate
+      - log
     properties:
-      cpuRequests:
+      createdDate:
         type: string
-        description: The CPU requests for VC for running spark jobs.
-      memRequests:
+        format: date-time
+        description: Time at which the log is created.
+      log:
         type: string
-        description: The Memory requests for VC for running spark jobs.
-      actualCpuRequests:
-        type: string
-        description: Actual CPU request for the VC. This accounts for other dex apps(eg. livy, airflow), that run in the virtual cluster.
-      actualMemoryRequests:
-        type: string
-        description: Actual Memory request for the VC. This accounts for other dex apps(eg. livy, airflow), that run in the virtual cluster.
-    description: Object to store resources for a CDE service
-  ChartValueOverridesRequest:
+        description: Log description.
+  GetAuditEventsRequest:
     type: object
+    description: GetAuditEventsRequest to get all audit events for a given workspace crn.
+    required:
+      - workspaceCrn
     properties:
-      chartName:
+      workspaceCrn:
         type: string
-        description: Name of the chart that has to be overridden, for eg- "dex-app", "dex-base".
-      overrides:
-        type: string
-        description: Space separated key-value pairs for overriding chart values. The key and the value must be separated using a colon(:) For eg- "airflow.enabled:true safari.enabled:true".
-    description: Object containing chart value overrides for enabling a CDE service or creation of virtual clusters.
-  ChartValueOverridesResponse:
+        description: Workspace crn for which audit events to be fetched.
+  GetAuditEventsResponse:
     type: object
+    description: GetAuditEventsResponse containes all the audit events for a given workspace crn.
+    required:
+      - auditEvents
     properties:
-      chartName:
-        type: string
-        description: Name of the chart that has to be overridden, for eg- "dex-app", "dex-base".
-      overrides:
+      auditEvents:
+        description: Contains all the audit events for a given workspace crn.
+        $ref: '#/definitions/AuditEvents'
+  AuditEvents:
+    type: object
+    description: AuditEvents contains all the audit events for a given workspace crn.
+    required:
+      - workspaceCrn
+      - events
+    properties:
+      workspaceCrn:
         type: string
-        description: Space separated key value-pairs for overriding chart values. The key and the value must be separated using a colon(:) For eg- "airflow.enabled:true safari.enabled:true".
-    description: Response object containing chart value overrides.
-  SmtpConfigRequest:
+        description: Workspace crn unique for the set of audit events.
+      events:
+        type: array
+        items:
+          $ref: '#/definitions/AuditEvent'
+        description: AuditEvent belong to the workspace crn.
+  AuditEvent:
     type: object
-    description: SMTP config request object.
+    description: Audit event descibes an performed or performing in a given workspace.
     required:
-      - email
-      - host
+      - workspaceCrn
+      - userCrn
+      - requestID
+      - action
+      - createdDate
     properties:
-      email:
+      workspaceCrn:
+        type: string
+        description: Workspace crn where the event observed.
+      userCrn:
         type: string
-        description: Sender's email address.
-      host:
+        description: UserCrn to track which user has caused the event.
+      requestID:
         type: string
-        description: SMTP host.
-      username:
+        description: Unique request ID to keep track of event.
+      action:
         type: string
-        description: SMTP username.
-      password:
+        description: Action the user has generated.
+      createdDate:
         type: string
-        description: SMTP password.
-        x-sensitive: true
-      port:
+        format: date-time
+        description: Time at creation of event.
+  Autoscaling:
+    type: object
+    description: Configuration for instance auto scaling.
+    required:
+      - minInstances
+      - maxInstances
+    properties:
+      minInstances:
         type: integer
         format: int32
-        default: 25
-        description: SMTP port.
-      startTls:
-        type: boolean
-        default: true
-        description: Use SMTP STARTTLS command to encrypt the mail.
-      ssl:
+        description: The minimum number of instance for auto scaling.
+      maxInstances:
+        type: integer
+        format: int32
+        description: The maximum number of instance for auto scaling.
+      enabled:
         type: boolean
-        default: false
-        description: Use SSL to secure the connection to the email server.
-  SmtpConfigResponse:
+        description: The boolean flag to enable the auto scaling.
+  InstanceGroup:
     type: object
-    description: SMTP config response object
+    description: Contains the necessary info for an instance group.
     required:
-      - email
-      - host
+      - instanceType
     properties:
-      email:
-        type: string
-        description: Sender's email address.
-      host:
+      instanceType:
         type: string
-        description: SMTP host.
-      username:
+        description: The cloud provider instance type for the node instance.
+      instanceTier:
         type: string
-        description: SMTP username.
-      port:
+        description: The tier of the instance i.e. on-demand/spot.
+      instanceCount:
         type: integer
         format: int32
-        default: 25
-        description: SMTP port.
-      startTls:
-        type: boolean
-        default: true
-        description: Use SMTP STARTTLS command to encrypt the mail.
-      ssl:
-        type: boolean
-        default: false
-        description: Use SSL to secure the connection to the email server.
-  AccessControlResponse:
-    type: object
-    description: Response object containing access control information for a Virtual Cluster.
-    properties:
-      users:
-        description: Workload usernames of CDP users granted access to the Virtual Cluster.
+        description: The initial number of instance node.
+      name:
+        type: string
+        description: The unique name of the instance group.
+      ingressRules:
         type: array
         items:
           type: string
-  ListServicesRequest:
-    type: object
-    description: Request object for ListServices method.
-    properties:
-      removeDeleted:
-        type: boolean
-        default: false
-        description: Filter out deleted CDE services from the list.
-  EnableServiceRequest:
+        description: The networking rules for the ingress.
+      rootVolume:
+        description: The root volume of the instance.
+        $ref: '#/definitions/RootVolume'
+      autoscaling:
+        description: The auto scaling configuration.
+        $ref: '#/definitions/Autoscaling'
+  WorkspaceInstanceGroup:
     type: object
-    description: Request object for Enable Service method.
+    description: Instance group information to show in workspace details.
     required:
-      - name
-      - env
       - instanceType
-      - minimumInstances
-      - maximumInstances
+      - instanceCount
+      - instanceGroupName
+      - minInstances
+      - maxInstances
+      - instances
+      - tags
     properties:
-      name:
-        type: string
-        description: Name of the CDE Service.
-      env:
-        type: string
-        description: CDP environment where cde service should be enabled.
       instanceType:
         type: string
-        description: Instance type of the cluster for CDE Service.
-      minimumInstances:
+        description: The cloud provider instance type for the node instance.
+      instanceCount:
         type: integer
         format: int32
-        description: Minimum Instances for the CDE Service.
-      maximumInstances:
-        type: integer
-        format: int32
-        description: Maximum Instances for the CDE Service.
-      minimumSpotInstances:
-        type: integer
-        format: int32
-        description: Minimum Spot instances for the CDE Service.
-      maximumSpotInstances:
-        type: integer
-        format: int32
-        description: Maximum Spot Instances for the CDE Service.
-      initialInstances:
-        type: integer
-        format: int32
-        description: Initial Instances when the service is enabled.
-      initialSpotInstances:
+        description: The initial number of instance node.
+      instanceGroupName:
+        type: string
+        description: The unique name of the instance group.
+      minInstances:
         type: integer
         format: int32
-        description: Initial spot Instances when the service is enabled.
-      rootVolumeSize:
+        description: The minimum number of instances that can be deployed to this instance group. If the value is 0, the group might be empty.
+      maxInstances:
         type: integer
         format: int32
-        description: EBS volume size in GB.
-      enablePublicEndpoint:
-        type: boolean
-        default: false
-        description: Creates a CDE endpoint (Load Balancer) in a publicly accessible subnet. If set false, the endpoint will be created in a private subnet and you will need to setup access to the endpoint manually in your cloud account.
-      deployPreviousVersion:
-        type: boolean
-        default: false
-        description: If set to "true", the previous version of the CDE service will be deployed.
-      enableWorkloadAnalytics:
-        type: boolean
-        default: false
-        description: If set false, diagnostic information about job and query execution is sent to Cloudera Workload Manager. Anonymization can be configured under Environments / Shared Resources / Telemetry. Refer documentation for more info at https://docs.cloudera.com/workload-manager/cloud/index.html.
-      useSsd:
-        type: boolean
-        description: Instance local storage (SSD) would be used for the workload filesystem (Example - spark local directory). In case the workload requires more space than what's available in the instance storage, please use an instance type with sufficient instance local storage or choose an instance type without SSD and configure the EBS volume size. Currently supported only for aws services.
-      chartValueOverrides:
+        description: The maximum number of instances that can be deployed to this instance group.
+      instances:
         type: array
         items:
-          $ref: '#/definitions/ChartValueOverridesRequest'
-        description: Chart overrides for enabling a service.
-      whitelistIps:
-        type: array
-        items:
-          type: string
-        description: List of CIDRs that would be allowed to access kubernetes master API server.
-      loadbalancerAllowlist:
-        type: array
-        items:
-          type: string
-        description: List of CIDRs that would be allowed to access the load balancer.
+          $ref: '#/definitions/Instance'
+        description: Instances in the instance group.
       tags:
-        type: object
-        description: User defined labels that tag all provisioned cloud resources.
-        additionalProperties:
-          type: string
-          description: User defined labels that tag all provisioned cloud resources.
-      skipValidation:
-        type: boolean
-        description: Skip Validation check.
-        default: false
-      enablePrivateNetwork:
-        type: boolean
-        description: Create CDE with fully private Azure services (AKS, MySQL, etc.) and enable vnet access via private endpoints and private link. This option is available only for Azure services.
-      subnets:
         type: array
         items:
-          type: string
-        description: List of Subnet IDs of CDP subnets to use for the kubernetes worker node.
-      customAzureFilesConfigs:
-        $ref: '#/definitions/CustomAzureFilesConfigs'
-        description: CDE uses a default public File Shares storage provisioned by AKS. Enable this option to use your own public/private File Shares.
-  CustomAzureFilesConfigs:
+          $ref: '#/definitions/Tag'
+        description: Tags are key/value pairs that are applied to all tag-able resources deployed in the workspace's cloud environment.
+  Instance:
     type: object
-    description: Override Azure Files Configs.
+    description: Represents each instance in an instance group.
     required:
-      - storageAccountName
-      - resourceGroup
+      - instanceId
+      - availabilityZone
     properties:
-      storageAccountName:
-        type: string
-        description: Azure Storage Account of the File Share.
-      resourceGroup:
+      instanceId:
         type: string
-        description: Resource Group of the Storage Account.
-      azureFilesFQDN:
+        description: Unique instance Id generated by the cloud provider.
+      availabilityZone:
         type: string
-        description: Azure File Share's server address. Defaults to '<storageaccount>.file.core.windows.net'.
-  EnableServiceResponse:
+        description: Availability zone the instance belongs to.
+  Tag:
     type: object
-    description: Response object for EnableService request.
+    description: Contains a single tag entry associated with a workspace.
+    required:
+      - key
+      - value
     properties:
-      service:
-        description: Service details of the created service.
-        $ref: '#/definitions/ServiceDescription'
-  UpdateServiceRequest:
+      key:
+        type: string
+        description: The name for the tag.
+      value:
+        type: string
+        description: The value for the tag.
+  ProvisionTag:
     type: object
-    description: Request object for UpdateService method.
+    description: Contains a single tag entry that will be configured on cloud resources associated with a workspace.
     required:
-      - clusterId
+      - key
+      - value
     properties:
-      clusterId:
+      key:
         type: string
-        description: Cluster ID of the service to update.
-      minimumInstances:
-        type: integer
-        format: int32
-        description: Minimum number of instances for the CDE service.
-      maximumInstances:
-        type: integer
-        format: int32
-        description: Maximum number of instances for the CDE service.
-      minimumSpotInstances:
-        type: integer
-        format: int32
-        description: Minimum number of spot instances for the CDE service.
-      maximumSpotInstances:
-        type: integer
-        format: int32
-        description: Maximum number of spot instances for the CDE service.
-      whitelistIps:
+        description: The name for the tag.
+      value:
+        type: string
+        description: The value for the tag.
+  ProvisionK8sRequest:
+    type: object
+    description: Request object for workspace provision.
+    required:
+      - instanceGroups
+      - environmentName
+    properties:
+      instanceGroups:
         type: array
         items:
-          type: string
-        description: List of CIDRs that would be allowed to access kubernetes master API server.
-      loadbalancerAllowlist:
+          $ref: '#/definitions/InstanceGroup'
+        description: The instance groups.
+      environmentName:
+        type: string
+        description: The environment for the workspace to create.
+      tags:
         type: array
         items:
-          type: string
-        description: List of CIDRs that would be allowed to access the load balancer.
-  UpdateServiceResponse:
+          $ref: '#/definitions/ProvisionTag'
+        description: Tags to add to the cloud provider resources created. This is in addition to any tags added by Cloudera.
+  CreateWorkspaceRequest:
     type: object
-    description: Response object for UpdateService request.
+    description: Request object for the CreateWorkspace method.
+    required:
+      - environmentName
+      - workspaceName
+      - usePublicLoadBalancer
+      - disableTLS
     properties:
-      operationId:
+      environmentName:
         type: string
-        description: Deprecated. The operation ID of the update request.
-        x-deprecated: true
-      status:
+        description: The environment for the workspace to create.
+      workspaceName:
         type: string
-        description: Status of update.
-  ListServicesResponse:
-    type: object
-    description: Response object for ListServices method.
-    properties:
-      services:
+        description: The name of the workspace to create.
+      usePublicLoadBalancer:
+        type: boolean
+        description: The boolean flag to request public load balancer. By default private load balancer is used.
+      disableTLS:
+        type: boolean
+        description: The boolean flag to disable TLS setup for workspace. By default the TLS is enabled.
+      provisionK8sRequest:
+        description: The request for Kubernetes workspace provision.
+        $ref: '#/definitions/ProvisionK8sRequest'
+      enableMonitoring:
+        type: boolean
+        description: The boolean flag is used to enable mlonitoring. By default monitoring is disabled.
+      existingNFS:
+        type: string
+        description: Optionally use an existing NFS by providing the hostname and desired path (Azure and Private Cloud only).
+      loadBalancerIPWhitelists:
         type: array
         items:
-          $ref: '#/definitions/ServiceSummary'
-        description: List of services.
-  DescribeServiceRequest:
+          type: string
+        description: The whitelist of ips for loadBalancer.
+  CreateWorkspaceResponse:
     type: object
-    description: Request object for DescribeService method.
-    required:
-      - clusterId
-    properties:
-      clusterId:
-        type: string
-        description: Cluster id of the service to be described.
-  DescribeServiceResponse:
+    description: Response object for the CreateWorkspace method.
+  ListWorkspacesRequest:
+    type: object
+    description: Request object for the ListWorkspaces method.
+  ListWorkspacesResponse:
     type: object
-    description: Response object for DescribeService method.
+    description: Response object for the ListWorkspaces method.
     properties:
-      service:
-        description: Description of the service
-        $ref: '#/definitions/ServiceDescription'
-  DisableServiceRequest:
+      workspaces:
+        type: array
+        items:
+          $ref: '#/definitions/WorkspaceSummary'
+        description: The list of workspaces.
+  WorkspaceSummary:
     type: object
-    description: DisableService request object.
+    description: A Cloudera Machine Learning workspace which includes the deployed configuration details.
     required:
-      - clusterId
+      - instanceName
+      - environmentName
+      - instanceStatus
+      - instanceUrl
+      - environmentCrn
+      - crn
+      - k8sClusterName
+      - creatorCrn
+      - version
+      - httpsEnabled
+      - filesystemID
+      - cloudPlatform
+      - monitoringEnabled
     properties:
-      clusterId:
+      instanceName:
         type: string
-        description: cluster Id of the service to disable.
-      force:
+        description: The name of the workspace.
+      environmentName:
+        type: string
+        description: The name of the workspace's environment.
+      instanceStatus:
+        type: string
+        description: The workspace's current status.
+      instanceUrl:
+        type: string
+        description: URL of the workspace's user interface.
+      environmentCrn:
+        type: string
+        description: CRN of the environment.
+      crn:
+        type: string
+        description: The CRN of the workspace.
+      k8sClusterName:
+        type: string
+        description: The Kubernetes cluster name.
+      creatorCrn:
+        type: string
+        description: The CRN of the creator of the workspace.
+      version:
+        type: string
+        description: The version of Cloudera Machine Learning that was installed on the workspace.
+      httpsEnabled:
         type: boolean
-        default: false
-        description: Force disable cde service.
-  DisableServiceResponse:
-    type: object
-    description: DisableService response object.
-    properties:
-      status:
+        description: Indicates if HTTPs communication was enabled on this workspace when provisioned.
+      filesystemID:
+        type: string
+        description: A filesystem ID referencing the filesystem that was created on the cloud provider environment that this workspace uses.
+      cloudPlatform:
+        type: string
+        description: The cloud platform of the environment that was used to create this workspace.
+      monitoringEnabled:
+        type: boolean
+        description: If usage monitoring is enabled or not on this workspace.
+      loadBalancerIPWhitelists:
+        type: array
+        items:
+          type: string
+        description: The whitelist of ips for loadBalancer.
+      creationDate:
         type: string
-        description: Status of deletion
-  GetKubeconfigRequest:
+        format: date-time
+        description: Creation date of workspace.
+      failureMessage:
+        type: string
+        description: Failure message from the most recent failure that has occurred during workspace provisioning.
+      healthInfoLists:
+        type: array
+        items:
+          $ref: '#/definitions/HealthInfo'
+        description: The health info information of the workspace.
+  Workspace:
     type: object
-    description: GetKubeconfig request object.
+    description: A ML workspace, which includes the cluster and storage.
     required:
-      - clusterId
+      - instanceName
+      - environmentName
+      - instanceStatus
+      - instanceUrl
+      - environmentCrn
+      - crn
+      - k8sClusterName
+      - creatorCrn
+      - version
+      - httpsEnabled
+      - endpointPublicAccess
+      - filesystemID
+      - tags
+      - instanceGroups
+      - cloudPlatform
+      - monitoringEnabled
     properties:
-      clusterId:
+      instanceName:
         type: string
-        description: cluster id of the cde service.
-  GetKubeconfigResponse:
-    type: object
-    description: GetKubeconfig response object.
-    properties:
-      kubeconfig:
+        description: The name of the workspace.
+      environmentName:
         type: string
-        description: kubeconfig for the cluster.
-  ListVcsRequest:
+        description: The name of the workspace's environment.
+      instanceStatus:
+        type: string
+        description: The workspace's current status.
+      instanceUrl:
+        type: string
+        description: URL of the workspace's user interface.
+      environmentCrn:
+        type: string
+        description: CRN of the environment.
+      crn:
+        type: string
+        description: The CRN of the workspace.
+      k8sClusterName:
+        type: string
+        description: The Kubernetes cluster name.
+      creatorCrn:
+        type: string
+        description: The CRN of the creator of the workspace.
+      version:
+        type: string
+        description: The version of Cloudera Machine Learning that was installed on the workspace.
+      httpsEnabled:
+        type: boolean
+        description: To Display if Https is enabled or not.
+      endpointPublicAccess:
+        type: boolean
+        description: To check if the cluster is publicly accessible or not.
+      filesystemID:
+        type: string
+        description: filesystemID used by the workspace
+      tags:
+        type: array
+        items:
+          $ref: '#/definitions/Tag'
+        description: Tags provided by the user at the time of workspace creation.
+      instanceGroups:
+        type: array
+        items:
+          $ref: '#/definitions/WorkspaceInstanceGroup'
+        description: The instance groups.
+      cloudPlatform:
+        type: string
+        description: The cloud platform of the environment that was used to create this workspace.
+      monitoringEnabled:
+        type: boolean
+        description: If usage monitoring is enabled or not on this workspace.
+      loadBalancerIPWhitelists:
+        type: array
+        items:
+          type: string
+        description: IP whitelist for loadBalancer.
+      creationDate:
+        type: string
+        format: date-time
+        description: Creation date of workspace.
+      healthInfoLists:
+        type: array
+        items:
+          $ref: '#/definitions/HealthInfo'
+        description: The health info information of the workspace.
+      failureMessage:
+        type: string
+        description: Failure message from the most recent failure that has occurred during workspace provisioning.
+  UpgradeWorkspaceRequest:
     type: object
-    description: ListVcs request object.
-    required:
-      - clusterId
+    description: Request object for the UpgradeWorkspace method.
     properties:
-      clusterId:
+      environmentName:
+        type: string
+        description: The environment of the workspace.
+      workspaceName:
+        type: string
+        description: The name of the workspace.
+      mlVersion:
         type: string
-        description: Cluster id of the service.
-  ListVcsResponse:
+        description: The version of workspace to upgrade to.
+      workspaceCrn:
+        type: string
+        description: The CRN of the workspace. If CRN is specified only the CRN is used for identifying the workspace, environment and name arguments are ignored.
+  UpgradeWorkspaceResponse:
     type: object
-    description: ListVcs response object.
-    properties:
-      vcs:
-        type: array
-        items:
-          $ref: '#/definitions/VcSummary'
-        description: List of virtual clusters.
-  DescribeVcRequest:
+    description: Response object for the UpgradeWorkspace method.
+  DescribeWorkspaceRequest:
     type: object
-    description: DescribeVc request object.
-    required:
-      - clusterId
-      - vcId
+    description: Request object for the DescribeWorkspace method.
     properties:
-      clusterId:
+      environmentName:
+        type: string
+        description: The environment for the workspace to describe.
+      workspaceName:
         type: string
-        description: Cluster id of the CDE service where vc was created.
-      vcId:
+        description: The name of the workspace to describe.
+      workspaceCrn:
         type: string
-        description: Virtual cluster id.
-  DescribeVcResponse:
+        description: The CRN of the workspace to describe. If CRN is specified only the CRN is used for identifying the workspace, environment and name arguments are ignored.
+  DescribeWorkspaceResponse:
     type: object
-    description: DescribeVc response object.
+    description: Response object for the DescribeWorkspace method.
+    required:
+      - workspace
     properties:
-      vc:
-        description: Description of the virtual cluster.
-        $ref: '#/definitions/VcDescription'
-  CreateVcRequest:
+      workspace:
+        description: The workspace.
+        $ref: '#/definitions/Workspace'
+  DeleteWorkspaceRequest:
     type: object
-    description: Request object for CreateVc method.
+    description: Request object for the DeleteWorkspace method.
     required:
-      - name
-      - clusterId
-      - cpuRequests
-      - memoryRequests
+      - force
+      - removeStorage
     properties:
-      name:
+      force:
+        type: boolean
+        description: Force delete a workspace even if errors occur during deletion. Force delete removes the guarantee that resources in your cloud account will be cleaned up.
+      removeStorage:
+        type: boolean
+        description: The remove storage flag indicates weather to keep the backing workspace filesystem storage or remove it during delete.
+      environmentName:
         type: string
-        description: Name of the virtual cluster.
-      clusterId:
+        description: The environment for the workspace to delete.
+      workspaceName:
         type: string
-        description: Cluster id of the CDE service where virtual cluster has to be created.
-      cpuRequests:
+        description: The name of the workspace to delete.
+      workspaceCrn:
         type: string
-        description: Cpu requests for autoscaling.
-      memoryRequests:
+        description: The CRN of the workspace to delete. If CRN is specified only the CRN is used for identifying the workspace, environment and name arguments are ignored.
+  DeleteWorkspaceResponse:
+    type: object
+    description: Response object for the DeleteWorkspace method.
+  GrantWorkspaceAccessRequest:
+    type: object
+    description: Request object for the GrantWorkspaceAccess method.
+    properties:
+      arn:
         type: string
-        description: Memory requests for autoscaling - eg. 30Gi.
-      chartValueOverrides:
-        type: array
-        items:
-          $ref: '#/definitions/ChartValueOverridesRequest'
-        description: Chart overrides for creating a virtual cluster.
-      smtpConfigs:
-        $ref: '#/definitions/SmtpConfigRequest'
-        description: SMTP Configurations for Airflow Email Alerts.
-      runtimeSpotComponent:
+        description: 'The aws user ARN to grant access to the corresponding EKS cluster. (Deprecated: Use identifier instead).'
+        x-deprecated: true
+      environmentName:
         type: string
-        description: Used to describe where the Driver and the Executors would run. By default the Driver would run on on-demand instances and the Executors on spot instances. Setting it to ALL will run both the Driver and the Executors on spot instances whereas setting it to NONE should run both the Driver and the Executor on on-demand instances. Currently applicable for aws services only. Use this option only on services with spot instances enabled.
-        enum:
-          - ALL
-          - NONE
-      sparkVersion:
+        description: The environment that the workspace is a member of.
+      workspaceName:
         type: string
-        description: Spark version for the virtual cluster. Currently supported spark versions are SPARK2(deprecated), SPARK3 and SPARK3_3. This feature is only supported in CDE-1.7.0 and beyond. SPARK3_3 is supported in CDE-1.19 and beyond.
-        enum:
-          - SPARK2
-          - SPARK3
-          - SPARK3_3
-      vcTier:
+        description: The name of the workspace to grant access to.
+      workspaceCrn:
         type: string
-        description: Tier of the virtual cluster. Currently supported tiers are CORE and ALLP. CORE tiered virtual cluster enables operational deployment via batch jobs. ALLP virtual clusters are all-purpose virtual clusters supporting both operational batch jobs and interactive sessions. This feature is only supported in CDE-1.19.0 and beyond.
-        enum:
-          - ALLP
-          - CORE
-      aclUsers:
-        description: Comma-separated Workload usernames of CDP users to be granted access to the Virtual Cluster.
+        description: The CRN of the workspace to grant access to. If CRN is specified only the CRN is used for identifying the workspace, environment and name arguments are ignored.
+      identifier:
         type: string
-  CreateVcResponse:
+        description: The cloud provider user id which will be granted access to the workspace's kubernetes cluster.
+  GrantWorkspaceAccessResponse:
     type: object
-    description: Response object for CreateVc method.
+    description: Response object for the GrantWorkspaceAccess method.
+    required:
+      - kubeconfig
     properties:
-      Vc:
-        description: Created Virtual Cluster
-        $ref: '#/definitions/VcDescription'
-  DeleteVcRequest:
+      kubeconfig:
+        type: string
+        description: The Kubernetes config file
+  RevokeWorkspaceAccessRequest:
     type: object
-    description: Request object for DeleteVc method.
-    required:
-      - clusterId
-      - vcId
+    description: Request object for the RevokeWorkspace method.
     properties:
-      clusterId:
+      arn:
+        type: string
+        description: 'The aws user ARN to revoke access to the corresponding EKS cluster. (Deprecated: Use identifier instead).'
+        x-deprecated: true
+      environmentName:
         type: string
-        description: Cluster id of the CDE service where virtual cluster was enabled.
-      vcId:
+        description: The environment that the workspace is a member of.
+      workspaceName:
         type: string
-        description: Virtual cluster id
-  DeleteVcResponse:
+        description: The name of the workspace to revoke access to.
+      workspaceCrn:
+        type: string
+        description: The CRN of the workspace to revoke access to. If CRN is specified only the CRN is used for identifying the workspace, environment and name arguments are ignored.
+      identifier:
+        type: string
+        description: The cloud provider user id which will be granted access to the workspace's kubernetes cluster.
+  RevokeWorkspaceAccessResponse:
+    type: object
+    description: Response object for the RevokeWorkspaceAccess method.
+  GetLatestWorkspaceVersionRequest:
+    type: object
+    description: Request object for GetLatestWorkspaceVersion.
+  GetLatestWorkspaceVersionResponse:
     type: object
-    description: Response object for DeleteVc method.
+    description: Response object for GetLatestWorkspaceVersion.
+    required:
+      - version
     properties:
-      status:
+      version:
         type: string
-        description: status of virtual cluster deletion.
-  UpdateVcRequest:
+        description: The latest version of a workspace that is used when deploying Cloudera Machine Learning workspaces.
+  HealthInfo:
     type: object
-    description: Request object for updateVc method.
+    description: Healthinfo object contains the health information of a resource.
     required:
-      - clusterId
-      - vcId
+      - resourceName
+      - isHealthy
+      - updatedAt
+      - message
+      - details
     properties:
-      clusterId:
+      resourceName:
         type: string
-        description: Cluster ID of the CDE service where Virtual Cluster was enabled.
-      vcId:
+        description: The resource name being checked.
+      isHealthy:
+        type: boolean
+        description: The boolean that indicates the health status.
+      updatedAt:
         type: string
-        description: Virtual Cluster ID
-      aclUsers:
-        description: Comma-separated Workload usernames of CDP users to be granted access to the Virtual Cluster.
+        format: date-time
+        description: The unix timestamp for the heartbeat.
+      message:
         type: string
-  UpdateVcResponse:
-    type: object
-    description: Response object for updateVc method.
-    properties:
-      Vc:
-        description: Updated Virtual Cluster.
-        $ref: '#/definitions/VcDescription'
+        description: The message to show for the health info.
+      details:
+        type: array
+        items:
+          type: string
+        description: The detail of the health info.
```

### Comparing `cdpcli-0.9.89/cdpcli/data/drscp/drscp.yaml` & `cdpcli-0.9.9/cdpcli/data/datalake/datalake.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,554 +1,721 @@
 swagger: '2.0'
-x-endpoint-name: drscp
+x-endpoint-name: datalake
+x-interface-model: cdp
 x-products: CDP
-x-form-factors: private
-x-audit: true
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.89
-  title: CDP Control Plane Data Recovery Service
+  version: 0.1-SNAPSHOT
+  title: Cloudera Datalake Service
   license:
     name: Apache 2.0
-  description: The API of Data Recovery Service for CDP Private Cloud Control Plane .
+  description: Cloudera data lake is a service for launching and managing data lake clusters powered by Cloudera Runtime.
 schemes:
   - https
 consumes:
   - application/json
 produces:
   - application/json
 paths:
-  /api/v1/drscp/createBackup:
+  /api/v1/datalake/createAWSDatalake:
     post:
-      summary: Creates a backup for the control plane.
-      description: Creates an on-demand backup for the control plane including embedded database, Kubernetes objects, persistent volume, etc. Backup requests are processed asynchronously and instantaneously.
-      operationId: createBackup
-      x-right: drscp/createBackup
-      x-mutating: true
+      summary: Creates an AWS datalake.
+      description: Creates an AWS datalake.
+      operationId: createAWSDatalake
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/CreateBackupRequest'
+            $ref: '#/definitions/CreateAWSDatalakeRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/CreateBackupResponse'
+            $ref: '#/definitions/CreateAWSDatalakeResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/drscp/restoreBackup:
+  /api/v1/datalake/createAzureDatalake:
     post:
-      summary: Restores backup.
-      description: Creates a new control plane from an existing backup.
-      operationId: restoreBackup
-      x-right: drscp/restoreBackup
-      x-mutating: true
+      summary: Creates an Azure datalake.
+      description: Creates an Azure datalake.
+      operationId: createAzureDatalake
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/RestoreBackupRequest'
+            $ref: '#/definitions/CreateAzureDatalakeRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/RestoreBackupResponse'
+            $ref: '#/definitions/CreateAzureDatalakeResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/drscp/deleteBackup:
+  /api/v1/datalake/listDatalakes:
     post:
-      summary: Deletes a control plane backup.
-      description: Deletes an existing control plane backup. The call returns immediately.
-      operationId: deleteBackup
-      x-right: drscp/deleteBackup
-      x-mutating: true
+      summary: Lists datalakes.
+      description: Lists datalakes.
+      operationId: listDatalakes
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/DeleteBackupRequest'
+            $ref: '#/definitions/ListDatalakesRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/DeleteBackupResponse'
+            $ref: '#/definitions/ListDatalakesResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/drscp/describeBackup:
+  /api/v1/datalake/deleteDatalake:
     post:
-      summary: Describes the backup.
-      description: Returns the description of an existing control plane backup.
-      operationId: describeBackup
-      x-right: drscp/describeBackup
-      x-mutating: false
+      summary: Deletes a datalake.
+      description: Deletes a datalake.
+      operationId: deleteDatalake
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/DescribeBackupRequest'
+            $ref: '#/definitions/DeleteDatalakeRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/DescribeBackupResponse'
+            $ref: '#/definitions/DeleteDatalakeResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/drscp/describeRestore:
+  /api/v1/datalake/describeDatalake:
     post:
-      summary: Restores the backup.
-      description: Returns the description of a control plane restore operation.
-      operationId: describeRestore
-      x-right: drscp/describeRestore
-      x-mutating: false
+      summary: Describes a datalake.
+      description: Describes a datalake.
+      operationId: describeDatalake
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/DescribeRestoreRequest'
+            $ref: '#/definitions/DescribeDatalakeRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/DescribeRestoreResponse'
+            $ref: '#/definitions/DescribeDatalakeResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/drscp/listBackupEntities:
+  /api/v1/datalake/repairDatalake:
     post:
-      summary: Lists potential backup entities associated with the control plane.
-      description: Lists potential backup entities. It includes the main control plane namespace and its corresponding vault namespace(if embedded).
-      operationId: listBackupEntities
-      x-right: drscp/listBackupEntities
-      x-mutating: false
+      summary: Repairs a datalake.
+      description: Repairs a datalake.
+      operationId: repairDatalake
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/ListBackupEntitiesRequest'
+            $ref: '#/definitions/RepairDatalakeRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ListBackupEntitiesResponse'
+            $ref: '#/definitions/RepairDatalakeResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/drscp/listBackups:
+  /api/v1/datalake/getClusterServiceStatus:
     post:
-      summary: Lists backups
-      description: Lists backups associated with the control plane.
-      operationId: listBackups
-      x-right: drscp/listBackups
-      x-mutating: false
+      summary: Get cluster service status.
+      description: Gets the status of the services in a cluster.
+      operationId: getClusterServiceStatus
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/ListBackupsRequest'
+            $ref: '#/definitions/GetClusterServiceStatusRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ListBackupsResponse'
+            $ref: '#/definitions/GetClusterServiceStatusResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/drscp/listRestores:
+  /api/v1/datalake/getClusterHostStatus:
     post:
-      summary: Lists restores.
-      description: Lists restores associated with the control plane.
-      operationId: listRestores
-      x-right: drscp/listRestores
-      x-mutating: false
+      summary: Get cluster host status.
+      description: Gets the status of the hosts in a cluster.
+      operationId: getClusterHostStatus
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/ListRestoresRequest'
+            $ref: '#/definitions/GetClusterHostStatusRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ListRestoresResponse'
+            $ref: '#/definitions/GetClusterHostStatusResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-  /api/v1/drscp/getLogs:
+  /api/v1/datalake/upgradeDatalake:
     post:
-      summary: Gets job logs.
-      description: Given the Crn, returns the corresponding job logs.
-      operationId: getLogs
-      x-right: drscp/getLogs
-      x-mutating: false
+      summary: Upgrade cluster OS.
+      description: Upgrades the datalake cluster to the latest images.
+      operationId: upgradeDatalake
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/GetLogsRequest'
+            $ref: '#/definitions/UpgradeDatalakeRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/GetLogsResponse'
+            $ref: '#/definitions/UpgradeDatalakeResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /api/v1/datalake/checkDatalakeUpgradeOptions:
+    post:
+      summary: Check upgrade options.
+      description: Checks for upgrade options.
+      operationId: checkDatalakeUpgradeOptions
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/CheckDatalakeUpgradeOptionsRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/CheckDatalakeUpgradeOptionsResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /api/v1/datalake/startDatalake:
+    post:
+      summary: Start Datalake
+      description: Starts a stopped Datalake
+      operationId: startDatalake
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/StartDatalakeRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/StartDatalakeResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /api/v1/datalake/stopDatalake:
+    post:
+      summary: Stop Datalake
+      description: Stops a running Datalake
+      operationId: stopDatalake
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/StopDatalakeRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/StopDatalakeResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
 definitions:
-  JobState:
-    type: string
-    enum:
-      - NOT_STARTED
-      - IN_PROGRESS
-      - COMPLETED
-      - PARTIALLY_FAILED
-      - FAILED
-      - TERMINATING
-    description: The current state of a Data Recovery Service job. The values are NOT_STARTED, IN_PROGRESS, COMPLETED, PARTIALLY_FAILED, FAILED and TERMINATING. NOT_STARTED indicates the job has not started. IN_PROGRESS indicates the job is running. COMPLETED indicates the job has finished running successfully. PARTIALLY_FAILED indicates the job has finished running with some warnings. FAILED indicates the job has finished running with errors and TERMINATING indicates that the entity containing this job is being deleted.
   Error:
     type: object
     description: An object returned on an error.
     properties:
       code:
         type: string
         description: The error code.
       message:
         type: string
         description: The error message.
-  ListBackupEntitiesRequest:
+  ClouderaManagerDetails:
     type: object
-    description: Request object for the list entities request.
-  ListBackupEntitiesResponse:
+    description: Cloudera Manager details.
+    required:
+      - version
+      - clouderaManagerRepositoryURL
+    properties:
+      version:
+        type: string
+        description: Cloudera Manager version.
+      clouderaManagerRepositoryURL:
+        type: string
+        description: Cloudera Manager repository URL.
+      clouderaManagerServerURL:
+        type: string
+        description: Cloudera Manager server URL.
+  ProductVersion:
     type: object
-    description: Response object for the list entities request.
+    description: Product version.
     required:
-      - items
+      - name
+      - version
     properties:
-      items:
-        type: array
-        description: The list of potential candidates for backup. It should be a single entity that indicates the namespace which the control plane is running on.
-        items:
-          type: string
-  CreateBackupRequest:
+      name:
+        type: string
+        description: The name of the product.
+      version:
+        type: string
+        description: The version of the product.
+  AWSConfiguration:
     type: object
-    description: Request object for the create backup request.
+    description: AWS configuration.
     properties:
-      backupName:
+      instanceProfile:
         type: string
-        description: Specified name for the backup.
-      itemName:
+        description: The instance profile used for the ID Broker instance.
+  AzureConfiguration:
+    type: object
+    description: Azure configuration.
+    properties:
+      managedIdentity:
         type: string
-        description: Name of the potential candidate for backup. It is optional in the case of control plane.
-  CreateBackupResponse:
+        description: The managed identity used for the ID Broker instance.
+  DatalakeDetails:
     type: object
-    description: Response object for the create backup request.
+    description: Details about a datalake
     required:
-      - backupCrn
+      - datalakeName
+      - crn
     properties:
-      backupCrn:
+      crn:
+        type: string
+        description: The CRN of the datalake.
+      datalakeName:
+        type: string
+        description: The name of the datalake.
+      status:
+        type: string
+        description: The status of the datalake.
+      environmentCrn:
         type: string
-        description: The CRN of the backup.
-  RestoreBackupRequest:
+        description: The CRN of the environment.
+      credentialCrn:
+        type: string
+        description: The CRN of credentials.
+      cloudPlatform:
+        type: string
+        description: The cloud platform.
+      creationDate:
+        type: string
+        format: date-time
+        description: The date when the datalake was created.
+      clouderaManager:
+        $ref: '#/definitions/ClouderaManagerDetails'
+        description: The Cloudera Manager details.
+      productVersions:
+        type: array
+        items:
+          $ref: '#/definitions/ProductVersion'
+        description: The product versions.
+      region:
+        type: string
+        description: The region of the datalake.
+      statusReason:
+        type: string
+        description: The reason for the status of the datalake.
+      awsConfiguration:
+        $ref: '#/definitions/AWSConfiguration'
+        description: The AWS configuration.
+      azureConfiguration:
+        $ref: '#/definitions/AzureConfiguration'
+        description: The Azure configuration.
+  Datalake:
     type: object
-    description: Request object for the restore backup request.
+    description: Information about a datalake.
     required:
-      - backupCrn
+      - datalakeName
+      - crn
     properties:
-      backupCrn:
+      datalakeName:
+        type: string
+        description: The name of the datalake.
+      crn:
         type: string
-        description: The CRN of the backup.
-  RestoreBackupResponse:
+        description: The CRN of the datalake.
+      status:
+        type: string
+        description: The status of the datalake.
+      environmentCrn:
+        type: string
+        description: The CRN of the environment.
+      creationDate:
+        type: string
+        format: date-time
+        description: The date when the datalake was created.
+      statusReason:
+        type: string
+        description: The reason for the status of the datalake.
+  DatalakeResourceTagRequest:
     type: object
-    description: Response object for the restore backup request.
+    description: Tag for a datalake resource.
     required:
-      - restoreCrn
+      - key
+      - value
     properties:
-      restoreCrn:
+      key:
+        type: string
+        description: The key of tag.
+      value:
         type: string
-        description: The CRN of the restore.
-  DeleteBackupRequest:
+        description: The value of the tag.
+  AWSConfigurationRequest:
     type: object
-    description: Request object for the delete backup request.
+    description: Request object for AWS configuration.
     required:
-      - backupCrn
+      - instanceProfile
+      - storageBucketLocation
     properties:
-      backupCrn:
+      instanceProfile:
         type: string
-        description: The CRN of the backup.
-  DeleteBackupResponse:
+        description: The ARN of an IAM instance profile.
+      storageBucketLocation:
+        type: string
+        description: The location of the S3 bucket to be used as storage. The location has to start with s3a:// followed by the bucket name.
+  AzureConfigurationRequest:
     type: object
-    description: Response object for the delete backup request.
+    description: Request object for Azure configuration.
     required:
-      - deleteBackupCrn
+      - managedIdentity
+      - storageLocation
     properties:
-      deleteBackupCrn:
+      managedIdentity:
+        type: string
+        description: The managed identity to use. The assumer should have Virtual Machine Contributor and Managed Identity Operator roles on subscription level.
+      storageLocation:
         type: string
-        description: The CRN of the kubernetes delete backup custom resource.
-  DescribeBackupRequest:
+        description: The storage location to use. The location has to be in the following format abfs://filesystem@storage-account-name.dfs.core.windows.net. The filesystem must already exist and the storage account must be StorageV2.
+  CreateAWSDatalakeRequest:
     type: object
-    description: Request object for the describe backup request.
+    description: Request object for create AWS datalake request.
     required:
-      - backupCrn
+      - datalakeName
+      - environmentName
     properties:
-      backupCrn:
+      datalakeName:
+        type: string
+        description: The datalake name. This name must be unique, must have between 5 and 100 characters, and must contain only lowercase letters, numbers and hyphens. Names are case-sensitive.
+        minLength: 5
+        maxLength: 100
+      environmentName:
+        type: string
+        description: The environment name or CRN.
+      cloudProviderConfiguration:
+        $ref: '#/definitions/AWSConfigurationRequest'
+        description: AWS configuration.
+      tags:
+        type: array
+        description: Tags to be added to Datalake related resources.
+        items:
+          $ref: '#/definitions/DatalakeResourceTagRequest'
+      scale:
         type: string
-        description: The CRN of the backup.
-  DescribeBackupResponse:
+        description: The scale of the datalake.
+  CreateAWSDatalakeResponse:
     type: object
-    description: Request object for the describe backup request.
+    description: Response object for create AWS datalake request.
     required:
-      - backup
+      - datalake
     properties:
-      backup:
-        $ref: '#/definitions/Backup'
-        description: The backup details.
-  DescribeRestoreRequest:
+      datalake:
+        $ref: '#/definitions/Datalake'
+        description: The datalake.
+  CreateAzureDatalakeRequest:
     type: object
-    description: Response object for the describe restore request.
+    description: Request object for create Azure datalake request.
     required:
-      - restoreCrn
+      - datalakeName
+      - environmentName
     properties:
-      restoreCrn:
+      datalakeName:
+        type: string
+        description: The datalake name. This name must be unique, must have between 5 and 100 characters, and must contain only lowercase letters, numbers and hyphens. Names are case-sensitive.
+        minLength: 5
+        maxLength: 100
+      environmentName:
+        type: string
+        description: The environment name or CRN.
+      cloudProviderConfiguration:
+        $ref: '#/definitions/AzureConfigurationRequest'
+        description: Azure configuration.
+      tags:
+        type: array
+        description: Tags to be added to Datalake related resources.
+        items:
+          $ref: '#/definitions/DatalakeResourceTagRequest'
+      scale:
         type: string
-        description: The unique CRN of the restore.
-  DescribeRestoreResponse:
+        description: The scale of the datalake.
+  CreateAzureDatalakeResponse:
     type: object
-    description: Response object for the describe restore request.
+    description: Response object for create Azure datalake request.
     required:
-      - restore
+      - datalake
     properties:
-      restore:
-        $ref: '#/definitions/Restore'
-        description: The restore details.
-  ListBackupsRequest:
+      datalake:
+        $ref: '#/definitions/Datalake'
+        description: The datalake.
+  ListDatalakesRequest:
     type: object
-    description: Request object for the list backups request.
+    description: Request object for list datalakes request.
     properties:
-      backupName:
+      environmentName:
         type: string
-        description: Specified name for the backup.
-      jobStates:
-        type: array
-        items:
-          $ref: '#/definitions/JobState'
-        description: The job states to filter by.
-  ListBackupsResponse:
+        description: The name or CRN of the environment for which the datalakes will be listed.
+      datalakeName:
+        type: string
+        description: The name or CRN of the datalake for which details are requested.
+  ListDatalakesResponse:
     type: object
-    description: Response object for the list backups request.
+    description: Response object for list datalakes request.
     required:
-      - backups
+      - datalakes
     properties:
-      backups:
+      datalakes:
         type: array
-        description: List of backups for the control plane.
         items:
-          $ref: '#/definitions/SimpleBackup'
-  Message:
+          $ref: '#/definitions/Datalake'
+        description: The datalakes.
+  DeleteDatalakeRequest:
     type: object
-    description: The message object used to display warnings and errors during DRS workflows
+    description: Request object for delete datalake request.
+    required:
+      - datalakeName
     properties:
-      text:
+      datalakeName:
         type: string
-        description: The text message of the warning/error.
-      timestamp:
-        type: string
-        description: The time when the warning/error is hit.
-      namespace:
-        type: string
-        description: The namespace that has the warning/error.
-  SimpleBackup:
+        description: The name or CRN of the datalake to be deleted.
+      force:
+        type: boolean
+        description: Whether the datalake should be force deleted. This option can be used when cluster deletion fails. This removes the entry from Cloudera Datalake service. Any lingering resources have to be deleted from the cloud provider manually. The default is false.
+  DeleteDatalakeResponse:
+    type: object
+    description: Response object for delete datalake request.
+  DescribeDatalakeRequest:
     type: object
-    description: A simple backup entry for listBackup usage
+    description: Request object for describe datalake request.
+    required:
+      - datalakeName
     properties:
-      backupCrn:
-        type: string
-        description: The unique CRN of the backup.
-      backupName:
+      datalakeName:
         type: string
-        description: The display name of the backup.
-      backupCreationTime:
-        type: string
-        description: The time when the backup was created.
-      backupPhase:
-        type: string
-        description: The phase of the backup operation. The values are PENDING, PRE_VALIDATION, SAVING_OBJECTS, CREATING_SNAPSHOTS and FINISHED. PENDING indicates waiting for the job to start executing. PRE_VALIDATION indicates validation of the environment before backup. SAVING_OBJECTS indicates saving all the kubernetes resources related to the backup item. CREATING_SNAPSHOTS indicates creating a snapshot of all Kubernetes PersistentVolumeClaims related to the backup item and FINISHED indicates that the backup job has finished.
-      backupJobState:
-        type: string
-        description: The current state of the backup job. The values are NOT_STARTED, IN_PROGRESS, COMPLETED, PARTIALLY_FAILED, FAILED and TERMINATING. NOT_STARTED indicates the job has not started. IN_PROGRESS indicates the job is running. COMPLETED indicates the job has finished running successfully. PARTIALLY_FAILED indicates the job has finished running with some warnings. FAILED indicates the job has finished running with errors and TERMINATING indicates that the entity containing this job is being deleted.
-  Backup:
+        description: The name or CRN of the datalake.
+  DescribeDatalakeResponse:
     type: object
-    description: Backup entry
+    description: Response object for describe datalake request.
+    required:
+      - datalake
     properties:
-      backupCrn:
-        type: string
-        description: The unique CRN of the backup.
-      backupCreationTime:
-        type: string
-        description: The time when the backup was created.
-      backupName:
-        type: string
-        description: The display name of the backup.
-      backupUpdatedTime:
-        type: string
-        description: The time when the backup was updated.
-      backupPhase:
-        type: string
-        description: The phase of the backup operation. The values are PENDING, PRE_VALIDATION, SAVING_OBJECTS, CREATING_SNAPSHOTS and FINISHED. PENDING indicates waiting for the job to start executing. PRE_VALIDATION indicates validation of the environment before backup. SAVING_OBJECTS indicates saving all the kubernetes resources related to the backup item. CREATING_SNAPSHOTS indicates creating a snapshot of all Kubernetes PersistentVolumeClaims related to the backup item and FINISHED indicates that the backup job has finished.
-      backupJobState:
+      datalake:
+        $ref: '#/definitions/DatalakeDetails'
+        description: The datalake.
+  RepairDatalakeRequest:
+    type: object
+    description: Request object for repair datalake request.
+    required:
+      - datalakeName
+      - instanceGroupName
+    properties:
+      datalakeName:
         type: string
-        description: The current state of the backup job. The values are NOT_STARTED, IN_PROGRESS, COMPLETED, PARTIALLY_FAILED, FAILED and TERMINATING. NOT_STARTED indicates the job has not started. IN_PROGRESS indicates the job is running. COMPLETED indicates the job has finished running successfully. PARTIALLY_FAILED indicates the job has finished running with some warnings. FAILED indicates the job has finished running with errors and TERMINATING indicates that the entity containing this job is being deleted.
-      backupJob:
+        description: The name or CRN of the datalake.
+      instanceGroupName:
         type: string
-        description: The backup job name.
-      includedNamespaces:
-        type: array
-        description: The list of namespaces to be included in backup.
-        items:
-          type: string
-      warnings:
-        type: array
-        description: The warnings from backup job.
-        items:
-          $ref: '#/definitions/Message'
-      errors:
-        type: array
-        description: The errors from backup job.
-        items:
-          $ref: '#/definitions/Message'
-  ListRestoresRequest:
+        description: The instance group where the failed instances will be repaired.
+  RepairDatalakeResponse:
     type: object
-    description: Request object for the list restores request.
+    description: Response object for repair datalake request.
+  GetClusterServiceStatusRequest:
+    type: object
+    description: Request object to get service status.
+    required:
+      - clusterName
     properties:
-      jobStates:
-        type: array
-        items:
-          $ref: '#/definitions/JobState'
-        description: The job states to filter by.
-      backupCrn:
+      clusterName:
         type: string
-        description: CRN of the backup.
-  ListRestoresResponse:
+        description: The name or CRN of the cluster.
+  GetClusterServiceStatusResponse:
     type: object
-    description: Response object for the list restores request.
+    description: Response object to get service status.
     required:
-      - restores
+      - services
     properties:
-      restores:
+      services:
         type: array
-        description: List of restores for the control plane.
         items:
-          $ref: '#/definitions/SimpleRestore'
-  SimpleRestore:
+          $ref: '#/definitions/ServiceStatus'
+        description: The cluster services health.
+  ServiceStatus:
     type: object
-    description: A simple Restore entry for listRestore Usage
+    description: Information about a cluster service.
     properties:
-      restoreCrn:
+      type:
         type: string
-        description: The CRN of the restore.
-      backupCrn:
+        description: The service type.
+      state:
         type: string
-        description: The CRN of the backup.
-      restoreCreationTime:
+        description: The service state.
+      healthSummary:
         type: string
-        description: The time when the restore was created.
-      includedNamespaces:
+        description: The service health summary.
+      healthChecks:
         type: array
-        description: The list of namespaces to be included in restore.
         items:
-          type: string
-      restorePhase:
-        type: string
-        description: The phase of the restore operation. The values are PENDING, PRE_VALIDATION, STOPPING_APPS, DELETING_OBJECTS, DELETING_OBJECTS_PVC, RESTORING_PVC, RESTORING_OBJECTS, STARTING_APPS and FINISHED. PENDING indicates waiting for the job to start executing. PRE_VALIDATION indicates validation of the environment before restore. STOPPING_APPS indicates stopping the microservices before data restore. DELETING_OBJECTS indicates deletion of Kubernetes resources other than PersistentVolumeClaims. DELETING_OBJECTS_PVC indicates deletion of Kubernetes PersistentVolumeClaims. RESTORING_PVC indicates creation of Kubernetes PersistentVolumeClaims. RESTORING_OBJECTS indicates creating of Kubernetes objects other than PersistentVolumeClaims. STARTING_APPS indicates starting of the microservices after data restore and FINISHED indicates the restore job has finished.
-      restoreJobState:
-        type: string
-        description: The current state of the restore job. The values are NOT_STARTED, IN_PROGRESS, COMPLETED, PARTIALLY_FAILED, FAILED and TERMINATING. NOT_STARTED indicates the job has not started. IN_PROGRESS indicates the job is running. COMPLETED indicates the job has finished running successfully. PARTIALLY_FAILED indicates the job has finished running with some warnings. FAILED indicates the job has finished running with errors and TERMINATING indicates that the entity containing this job is being deleted.
-  Restore:
+          $ref: '#/definitions/HealthCheck'
+        description: The service health checks.
+  HealthCheck:
     type: object
-    description: Restore entry
+    description: The result of a health check.
     properties:
-      restoreCrn:
+      name:
         type: string
-        description: The CRN of the restore.
-      backupCrn:
+        description: The name of service health check.
+      summary:
         type: string
-        description: The CRN of the backup.
-      restoreCreationTime:
-        type: string
-        description: The time when the restore was created.
-      restoreUpdatedTime:
+        description: The service health check summary.
+  GetClusterHostStatusRequest:
+    type: object
+    description: Request object to get host status.
+    required:
+      - clusterName
+    properties:
+      clusterName:
         type: string
-        description: The updated time of the restore.
-      excludedResources:
-        type: array
-        description: The list of resources to be excluded in restore.
-        items:
-          type: string
-      includedNamespaces:
-        type: array
-        description: The list of namespaces to be included in restore.
-        items:
-          type: string
-      successConditions:
+        description: The name or CRN of the cluster.
+  GetClusterHostStatusResponse:
+    type: object
+    description: Response object for getting host status.
+    required:
+      - hosts
+    properties:
+      hosts:
         type: array
-        description: The list of conditions to be met for a successful restore.
         items:
-          type: string
-      restorePhase:
+          $ref: '#/definitions/HostStatus'
+        description: The cluster hosts status.
+  HostStatus:
+    type: object
+    description: Information about cluster host status.
+    properties:
+      hostid:
         type: string
-        description: The phase of the restore operation. The values are PENDING, PRE_VALIDATION, STOPPING_APPS, DELETING_OBJECTS, DELETING_OBJECTS_PVC, RESTORING_PVC, RESTORING_OBJECTS, STARTING_APPS and FINISHED. PENDING indicates waiting for the job to start executing. PRE_VALIDATION indicates validation of the environment before restore. STOPPING_APPS indicates stopping the microservices before data restore. DELETING_OBJECTS indicates deletion of Kubernetes resources other than PersistentVolumeClaims. DELETING_OBJECTS_PVC indicates deletion of Kubernetes PersistentVolumeClaims. RESTORING_PVC indicates creation of Kubernetes PersistentVolumeClaims. RESTORING_OBJECTS indicates creating of Kubernetes objects other than PersistentVolumeClaims. STARTING_APPS indicates starting of the microservices after data restore and FINISHED indicates the restore job has finished.
-      restoreJobState:
+        description: Unique identifier of the cluster host given by Cloudera Manager.
+      hostname:
         type: string
-        description: The current state of the restore job. The values are NOT_STARTED, IN_PROGRESS, COMPLETED, PARTIALLY_FAILED, FAILED and TERMINATING. NOT_STARTED indicates the job has not started. IN_PROGRESS indicates the job is running. COMPLETED indicates the job has finished running successfully. PARTIALLY_FAILED indicates the job has finished running with some warnings. FAILED indicates the job has finished running with errors and TERMINATING indicates that the entity containing this job is being deleted.
-      restoreJob:
+        description: The cluster hostname.
+      healthSummary:
         type: string
-        description: The restore job name.
-      warnings:
-        type: array
-        description: The warnings from restore job.
-        items:
-          $ref: '#/definitions/Message'
-      errors:
-        type: array
-        description: The errors from restore job.
-        items:
-          $ref: '#/definitions/Message'
-  GetLogsRequest:
+        description: The host health summary.
+  UpgradeDatalakeRequest:
     type: object
-    description: Request object for the get logs request.
+    description: Request object to upgrade datalake.
     required:
-      - crn
+      - datalakeName
     properties:
-      crn:
+      datalakeName:
         type: string
-        description: The CRN of the custom resource.
-  GetLogsResponse:
+        description: The name or CRN of the datalake.
+  UpgradeDatalakeResponse:
     type: object
-    description: Response object for the get backup logs request.
+    description: Response object for upgrade datalake request.
+  CheckDatalakeUpgradeOptionsRequest:
+    type: object
+    description: Request object to check datalake upgrade options.
+    required:
+      - datalakeName
+    properties:
+      datalakeName:
+        type: string
+        description: The name or CRN of the datalake.
+  CheckDatalakeUpgradeOptionsResponse:
+    type: object
+    description: Response object to check datalake upgrade options.
     required:
-      - logs
+      - current
     properties:
-      logs:
+      current:
+        $ref: '#/definitions/ImageInfo'
+        description: Details of the image, that datalake is currently uses.
+      upgrade:
+        $ref: '#/definitions/ImageInfo'
+        description: Details of the image, that datalake can be upgraded to.
+  StartDatalakeRequest:
+    type: object
+    description: Request object to start a datalake.
+    required:
+      - datalakeName
+    properties:
+      datalakeName:
+        type: string
+        description: The name or CRN of the datalake.
+  StartDatalakeResponse:
+    type: object
+    description: Response object of starting a datalake.
+  StopDatalakeRequest:
+    type: object
+    description: Request object to stop a datalake.
+    required:
+      - datalakeName
+    properties:
+      datalakeName:
+        type: string
+        description: The name or CRN of the datalakeName.
+  StopDatalakeResponse:
+    type: object
+    description: Response object of stopping a datalake.
+  ImageInfo:
+    type: object
+    description: Basic information about an image.
+    properties:
+      imageName:
+        type: string
+        description: The name of the image.
+      imageId:
+        type: string
+        description: The id of the image.
+      imageCatalogName:
         type: string
-        description: Contains the logs of the operation.
-        x-skip-logging: true
+        description: Name of the image catalog, the image is from.
+      created:
+        type: integer
+        format: int64
+        description: Image creation timestamp
```

### Comparing `cdpcli-0.9.89/cdpcli/data/ml/ml.yaml` & `cdpcli-0.9.9/cdpcli/data/datahub/datahub.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,1676 +1,1495 @@
-x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
-x-endpoint-name: ml
+x-endpoint-name: datahub
+x-interface-model: cdp
 x-products: CDP
-x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.89
-  title: Cloudera Machine Learning
+  version: 0.1-SNAPSHOT
+  title: Cloudera Data hub Service
   license:
     name: Apache 2.0
-  description: Install and manage Cloudera Machine Learning applications.
-  termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
+  description: Cloudera data hub is a service for launching and managing workload clusters powered by Cloudera Runtime.
 schemes:
   - https
 consumes:
   - application/json
 produces:
   - application/json
 paths:
-  /api/v1/ml/backupWorkspace:
+  /api/v1/datahub/listClusters:
     post:
-      summary: Backup a workspace.
-      description: Backup a workspace.
-      operationId: backupWorkspace
+      summary: Lists workload clusters.
+      description: Lists workload clusters.
+      operationId: listClusters
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/BackupWorkspaceRequest'
+            $ref: '#/definitions/ListClustersRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/BackupWorkspaceResponse'
+            $ref: '#/definitions/ListClustersResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-      x-mutating: true
-  /api/v1/ml/createWorkspace:
+  /api/v1/datahub/createAWSCluster:
     post:
-      summary: Create a Cloudera Machine Learning workspace.
-      description: Provision a Kubernetes cluster and install the Cloudera Machine Learning application in it.
-      operationId: createWorkspace
+      summary: Creates an AWS workload cluster.
+      description: Creates an AWS workload cluster.
+      operationId: createAWSCluster
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/CreateWorkspaceRequest'
+            $ref: '#/definitions/CreateAWSClusterRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/CreateWorkspaceResponse'
+            $ref: '#/definitions/CreateAWSClusterResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-      x-mutating: true
-  /api/v1/ml/deleteBackup:
+  /api/v1/datahub/createAzureCluster:
     post:
-      summary: Deletes a backup snapshot.
-      description: Deletes a Cloudera Machine Learning workspace backup.
-      operationId: deleteBackup
+      summary: Creates an Azure workload cluster.
+      description: Creates an Azure workload cluster.
+      operationId: createAzureCluster
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/DeleteBackupRequest'
+            $ref: '#/definitions/CreateAzureClusterRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/DeleteBackupResponse'
+            $ref: '#/definitions/CreateAzureClusterResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-      x-mutating: true
-  /api/v1/ml/deleteInstanceGroup:
+  /api/v1/datahub/deleteCluster:
     post:
-      summary: Deletes an instance group from the cluster.
-      description: Deletes an instance group from a Cloudera Machine Learning workspace.
-      operationId: deleteInstanceGroup
+      summary: Deletes a workload cluster.
+      description: Deletes a workload cluster.
+      operationId: deleteCluster
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/DeleteInstanceGroupRequest'
+            $ref: '#/definitions/DeleteClusterRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/DeleteInstanceGroupResponse'
+            $ref: '#/definitions/DeleteClusterResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-      x-mutating: true
-  /api/v1/ml/deleteWorkspace:
+  /api/v1/datahub/describeCluster:
     post:
-      summary: Delete Cloudera Machine Learning Workspace.
-      description: Deletes a Cloudera Machine Learning workspace.
-      operationId: deleteWorkspace
+      summary: Describes a workload cluster.
+      description: Describes a workload cluster.
+      operationId: describeCluster
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/DeleteWorkspaceRequest'
+            $ref: '#/definitions/DescribeClusterRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/DeleteWorkspaceResponse'
+            $ref: '#/definitions/DescribeClusterResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-      x-mutating: true
-  /api/v1/ml/describeWorkspace:
+  /api/v1/datahub/getClusterServiceStatus:
     post:
-      summary: Describe Cloudera Machine Learning Workspace.
-      description: Describes a Cloudera Machine Learning workspace.
-      operationId: describeWorkspace
+      summary: Get cluster service status.
+      description: Gets the status of the services in a cluster.
+      operationId: getClusterServiceStatus
+      x-right: datahub/read
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/DescribeWorkspaceRequest'
+            $ref: '#/definitions/GetClusterServiceStatusRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/DescribeWorkspaceResponse'
+            $ref: '#/definitions/GetClusterServiceStatusResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-      x-mutating: false
-  /api/v1/ml/getAuditEvents:
+  /api/v1/datahub/getClusterHostStatus:
     post:
-      summary: Gets all the events belong to a workspace crn.
-      description: Gets all the events belong to a workspace crn.
-      operationId: getAuditEvents
+      summary: Get cluster host status.
+      description: Gets the status of the hosts in a cluster.
+      operationId: getClusterHostStatus
+      x-right: datahub/read
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/GetAuditEventsRequest'
+            $ref: '#/definitions/GetClusterHostStatusRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/GetAuditEventsResponse'
+            $ref: '#/definitions/GetClusterHostStatusResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-      x-mutating: false
-  /api/v1/ml/getKubeconfig:
+  /api/v1/datahub/stopCluster:
     post:
-      summary: ListWorkspaceAccess Cloudera Machine Learning Workspace.
-      description: Lists users that can perform Kubernetes operations on a Cloudera Machine Learning workspace via EKS.
-      operationId: getKubeconfig
+      summary: Stops a workload cluster.
+      description: Stops a workload cluster. When a cluster is put in the stopped state, cluster VMs are given back to the cloud provider. To provision new VMs, start the cluster.
+      operationId: stopCluster
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/GetKubeconfigRequest'
+            $ref: '#/definitions/StopClusterRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/GetKubeconfigResponse'
+            $ref: '#/definitions/StopClusterResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-      x-mutating: false
-  /api/v1/ml/getLatestWorkspaceVersion:
+  /api/v1/datahub/startCluster:
     post:
-      summary: GetLatestWorkspaceVersion Cloudera Machine Learning Workspace.
-      description: Retrieves the latest version that Cloudera Machine Learning deploys to workspaces.
-      operationId: getLatestWorkspaceVersion
+      summary: Starts a stopped workload cluster.
+      description: Starts a stopped workload cluster.
+      operationId: startCluster
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/GetLatestWorkspaceVersionRequest'
+            $ref: '#/definitions/StartClusterRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/GetLatestWorkspaceVersionResponse'
+            $ref: '#/definitions/StartClusterResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-      x-mutating: false
-  /api/v1/ml/getLogs:
+  /api/v1/datahub/retryCluster:
     post:
-      summary: Gets all the logs belong to a request id.
-      description: Gets all the logs belong to a request id.
-      operationId: getLogs
+      summary: Retries creation of a failed workload cluster.
+      description: When stack provisioning or cluster creation fails, retryCluster allows you to resume the process from the last failed step.
+      operationId: retryCluster
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/GetLogsRequest'
+            $ref: '#/definitions/RetryClusterRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/GetLogsResponse'
+            $ref: '#/definitions/RetryClusterResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-      x-mutating: false
-  /api/v1/ml/grantWorkspaceAccess:
+  /api/v1/datahub/repairCluster:
     post:
-      summary: GrantWorkspaceAccess Cloudera Machine Learning Workspace.
-      description: Grants an AWS user to perform Kubernetes operations on a Cloudera Machine Learning workspace via EKS.
-      operationId: grantWorkspaceAccess
+      summary: Repairs a cluster.
+      description: Repairs a cluster.
+      operationId: repairCluster
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/GrantWorkspaceAccessRequest'
+            $ref: '#/definitions/RepairClusterRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/GrantWorkspaceAccessResponse'
+            $ref: '#/definitions/RepairClusterResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-      x-mutating: true
-  /api/v1/ml/listWorkspaceAccess:
+  /api/v1/datahub/syncCluster:
     post:
-      summary: ListWorkspaceAccess Cloudera Machine Learning Workspace.
-      description: Lists users that can perform Kubernetes operations on a Cloudera Machine Learning workspace via EKS.
-      operationId: listWorkspaceAccess
+      summary: Synchronizes the state of a cluster with the cloud provider and Cloudera Manager.
+      description: Synchronizes the state of a cluster with the cloud provider and Cloudera Manager.
+      operationId: syncCluster
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/ListWorkspaceAccessRequest'
+            $ref: '#/definitions/SyncClusterRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ListWorkspaceAccessResponse'
+            $ref: '#/definitions/SyncClusterResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-      x-mutating: false
-  /api/v1/ml/listWorkspaceBackups:
+  /api/v1/datahub/scaleCluster:
     post:
-      summary: List backup snapshots of a workspace.
-      description: List backup snapshots of a workspace.
-      operationId: listWorkspaceBackups
+      summary: Scales a cluster by adding or removing cluster nodes.
+      description: Scales a cluster by adding or removing cluster nodes.
+      operationId: scaleCluster
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/ListWorkspaceBackupsRequest'
+            $ref: '#/definitions/ScaleClusterRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ListWorkspaceBackupsResponse'
+            $ref: '#/definitions/ScaleClusterResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-      x-mutating: false
-  /api/v1/ml/listWorkspaces:
+  /api/v1/datahub/listRecipes:
     post:
-      summary: List Cloudera Machine Learning workspaces.
-      description: List Cloudera Machine Learning workspaces.
-      operationId: listWorkspaces
+      summary: Lists recipes. A recipe is a script that runs on all nodes of a specified instance group.
+      description: Lists recipes. A recipe is a script that runs on all nodes of a specified instance group.
+      operationId: listRecipes
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/ListWorkspacesRequest'
+            $ref: '#/definitions/ListRecipesRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ListWorkspacesResponse'
+            $ref: '#/definitions/ListRecipesResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-      x-skip-auditing: true
-  /api/v1/ml/modifyClusterInstanceGroup:
+  /api/v1/datahub/deleteRecipes:
     post:
-      summary: Modify Cloudera Machine Learning workspace cluster instance group.
-      description: Modify a Cloudera Machine Learning workspace cluster instance group.
-      operationId: modifyClusterInstanceGroup
+      summary: Deletes recipes. A recipe is a script that runs on all nodes of a specified instance group.
+      description: Deletes recipes. A recipe is a script that runs on all nodes of a specified instance group.
+      operationId: deleteRecipes
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/ModifyClusterInstanceGroupRequest'
+            $ref: '#/definitions/DeleteRecipesRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ModifyClusterInstanceGroupResponse'
+            $ref: '#/definitions/DeleteRecipesResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-      x-mutating: true
-  /api/v1/ml/modifyClusterSecurity:
+  /api/v1/datahub/createRecipe:
     post:
-      summary: Modify Cloudera Machine Learning workspace cluster security.
-      description: Modify a Cloudera Machine Learning workspace cluster security.
-      operationId: modifyClusterSecurity
+      summary: Creates recipe. A recipe is a script that runs on all nodes of a specified instance group.
+      description: Creates recipe. A recipe is a script that runs on all nodes of a specified instance group.
+      operationId: createRecipe
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/ModifyClusterSecurityRequest'
+            $ref: '#/definitions/CreateRecipeRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ModifyClusterSecurityResponse'
+            $ref: '#/definitions/CreateRecipeResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-      x-mutating: true
-  /api/v1/ml/modifyWorkspaceLoadBalancer:
+  /api/v1/datahub/describeRecipe:
     post:
-      summary: Modify Cloudera Machine Learning workspace loadbalancer.
-      description: Modify a Cloudera Machine Learning workspace loadbalancer.
-      operationId: modifyWorkspaceLoadBalancer
+      summary: Describes recipe. A recipe is a script that runs on all nodes of a specified instance group.
+      description: Describes recipe. A recipe is a script that runs on all nodes of a specified instance group.
+      operationId: describeRecipe
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/ModifyWorkspaceLoadBalancerRequest'
+            $ref: '#/definitions/DescribeRecipeRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ModifyWorkspaceLoadBalancerResponse'
+            $ref: '#/definitions/DescribeRecipeResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-      x-mutating: true
-  /api/v1/ml/requestWorkflowCancellation:
+  /api/v1/datahub/listClusterDefinitions:
     post:
-      summary: Request a workflow cancellation.
-      description: Request a long running workflow cancellation by resource ID and workflow type.
-      operationId: requestWorkflowCancellation
+      summary: Lists cluster definitions. A cluster definition is a reusable template in JSON format that can be used for creating multiple Data Hub clusters with identical cloud provider settings.
+      description: Lists cluster definitions. A cluster definition is a reusable template in JSON format that can be used for creating multiple Data Hub clusters with identical cloud provider settings.
+      operationId: listClusterDefinitions
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/RequestWorkflowCancellationRequest'
+            $ref: '#/definitions/ListClusterDefinitionsRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/RequestWorkflowCancellationResponse'
+            $ref: '#/definitions/ListClusterDefinitionsResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-      x-mutating: true
-  /api/v1/ml/restoreWorkspace:
+  /api/v1/datahub/deleteClusterDefinitions:
     post:
-      summary: Restore a Cloudera Machine Learning workspace.
-      description: Create a new workspace based on an existing workspace backup snapshot.
-      operationId: restoreWorkspace
+      summary: Deletes cluster definitions. A cluster definition is a reusable template in JSON format that can be used for creating multiple Data Hub clusters with identical cloud provider settings.
+      description: Deletes cluster definitions. A cluster definition is a reusable template in JSON format that can be used for creating multiple Data Hub clusters with identical cloud provider settings.
+      operationId: deleteClusterDefinitions
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/RestoreWorkspaceRequest'
+            $ref: '#/definitions/DeleteClusterDefinitionsRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/RestoreWorkspaceResponse'
+            $ref: '#/definitions/DeleteClusterDefinitionsResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-      x-mutating: true
-  /api/v1/ml/resumeWorkspace:
+  /api/v1/datahub/createClusterDefinition:
     post:
-      summary: Resume Cloudera Machine Learning workspace.
-      description: Resume a Cloudera Machine Learnings workspace.
-      operationId: resumeWorkspace
+      summary: Creates a cluster definition. A cluster definition is a reusable template in JSON format that can be used for creating multiple Data Hub clusters with identical cloud provider settings.
+      description: Creates a cluster definition. A cluster definition is a reusable template in JSON format that can be used for creating multiple Data Hub clusters with identical cloud provider settings.
+      operationId: createClusterDefinition
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/ResumeWorkspaceRequest'
+            $ref: '#/definitions/CreateClusterDefinitionRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/ResumeWorkspaceResponse'
+            $ref: '#/definitions/CreateClusterDefinitionResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-      x-mutating: true
-  /api/v1/ml/revokeWorkspaceAccess:
+  /api/v1/datahub/describeClusterDefinition:
     post:
-      summary: RevokeWorkspaceAccess Cloudera Machine Learning Workspace.
-      description: Revokes an AWS user to perform Kubernetes operations on a Cloudera Machine Learning workspace via EKS.
-      operationId: revokeWorkspaceAccess
+      summary: Describes a cluster definition. A cluster definition is a reusable template in JSON format that can be used for creating multiple Data Hub clusters with identical cloud provider settings.
+      description: Describes a cluster definition. A cluster definition is a reusable template in JSON format that can be used for creating multiple Data Hub clusters with identical cloud provider settings.
+      operationId: describeClusterDefinition
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/RevokeWorkspaceAccessRequest'
+            $ref: '#/definitions/DescribeClusterDefinitionRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/RevokeWorkspaceAccessResponse'
+            $ref: '#/definitions/DescribeClusterDefinitionResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-      x-mutating: true
-  /api/v1/ml/suspendWorkspace:
+  /api/v1/datahub/listClusterTemplates:
     post:
-      summary: Suspend Cloudera Machine Learning workspace.
-      description: Suspend a Cloudera Machine Learning workspace.
-      operationId: suspendWorkspace
+      summary: Lists cluster templates. A cluster template is a reusable template in JSON format that can be used for creating multiple Data Hub clusters with identical Cloudera Runtime settings.
+      description: Lists cluster templates. A cluster template is a reusable template in JSON format that can be used for creating multiple Data Hub clusters with identical Cloudera Runtime settings.
+      operationId: listClusterTemplates
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/SuspendWorkspaceRequest'
+            $ref: '#/definitions/ListClusterTemplatesRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/SuspendWorkspaceResponse'
+            $ref: '#/definitions/ListClusterTemplatesResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-      x-mutating: true
-  /api/v1/ml/upgradeWorkspace:
+  /api/v1/datahub/deleteClusterTemplates:
     post:
-      summary: Upgrade Cloudera Machine Learning workspace.
-      description: Upgrades a Cloudera Machine Learning workspace to the latest available version.
-      operationId: upgradeWorkspace
+      summary: Deletes cluster templates. A cluster template is a reusable template in JSON format that can be used for creating multiple Data Hub clusters with identical Cloudera Runtime settings.
+      description: Deletes cluster templates. A cluster template is a reusable template in JSON format that can be used for creating multiple Data Hub clusters with identical Cloudera Runtime settings.
+      operationId: deleteClusterTemplates
       parameters:
         - name: input
           in: body
           required: true
           schema:
-            $ref: '#/definitions/UpgradeWorkspaceRequest'
+            $ref: '#/definitions/DeleteClusterTemplatesRequest'
       responses:
         200:
           description: Expected response to a valid request.
           schema:
-            $ref: '#/definitions/UpgradeWorkspaceResponse'
+            $ref: '#/definitions/DeleteClusterTemplatesResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /api/v1/datahub/createClusterTemplate:
+    post:
+      summary: Creates a cluster template. A cluster template is a reusable template in JSON format that can be used for creating multiple Data Hub clusters with identical Cloudera Runtime settings.
+      description: Creates a cluster template. A cluster template is a reusable template in JSON format that can be used for creating multiple Data Hub clusters with identical Cloudera Runtime settings.
+      operationId: createClusterTemplate
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/CreateClusterTemplateRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/CreateClusterTemplateResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /api/v1/datahub/describeClusterTemplate:
+    post:
+      summary: Describes a cluster template. A cluster template is a reusable template in JSON format that can be used for creating multiple Data Hub clusters with identical Cloudera Runtime settings.
+      description: Describes a cluster template. A cluster template is a reusable template in JSON format that can be used for creating multiple Data Hub clusters with identical Cloudera Runtime settings.
+      operationId: describeClusterTemplate
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/DescribeClusterTemplateRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/DescribeClusterTemplateResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
-      x-mutating: true
 definitions:
   Error:
     type: object
     description: An object returned on an error.
     properties:
       code:
         type: string
         description: The error code.
       message:
         type: string
         description: The error message.
-  RootVolume:
-    type: object
-    description: Configuration for instance root device volume.
-    required:
-      - size
-    properties:
-      size:
-        type: integer
-        format: int64
-        description: The volume size in GB.
-  GetLogsRequest:
+  ImageRequest:
     type: object
-    description: GetLogsRequestfor getting logs for a request ID.
+    description: The details of the image used for cluster instances.
     required:
-      - workspaceCrn
-      - requestID
+      - id
+      - catalogName
     properties:
-      workspaceCrn:
+      id:
         type: string
-        description: WorkspaceCrn the requestID belongs to.
-      requestID:
+        description: The ID of the image used for cluster instances. This is generated by the cloud provider to uniquely identify the image.
+      catalogName:
         type: string
-        description: Unique Key to identify a set of logs.
-      fetchAll:
-        type: boolean
-        description: Flag to fetch all logs.
-      pageSize:
-        type: integer
-        format: int32
-        description: Limit the number of logs.
-      offset:
-        type: integer
-        format: int32
-        description: offset from which the logs should be fetched.
-  GetLogsResponse:
+        description: The image catalog name.
+  ImageDetails:
     type: object
-    description: GetLogsResponse contains all the logs for a given request id.
-    required:
-      - auditLogs
+    description: The details of the image used for cluster instances.
     properties:
-      auditLogs:
-        description: Contains all the logs for a given request id.
-        $ref: '#/definitions/AuditLogs'
-  AuditLogs:
+      name:
+        type: string
+        description: The name of the image used for cluster instances.
+      id:
+        type: string
+        description: The ID of the image used for cluster instances. This is internally generated by the cloud provider to uniquely identify the image.
+      catalogUrl:
+        type: string
+        description: The image catalog URL.
+      catalogName:
+        type: string
+        description: The image catalog name.
+  Cluster:
     type: object
-    description: AuditLogs contains all the logs for a given request id.
+    description: Information about a cluster.
     required:
-      - requestID
-      - count
-      - logs
+      - clusterName
+      - crn
     properties:
-      requestID:
+      clusterName:
         type: string
-        description: The request ID associated with a long-running operation to fetch the logs for.
-      count:
+        description: The name of the cluster.
+      crn:
+        type: string
+        description: The CRN of the cluster.
+      creationDate:
+        type: string
+        format: date-time
+        description: The date when the cluster was created.
+      status:
+        type: string
+        description: The status of the cluster.
+      nodeCount:
         type: integer
         format: int32
-        description: Total number of logs associated with the request id.
-      logs:
-        type: array
-        items:
-          $ref: '#/definitions/AuditLog'
-        description: Contains all the logs for a given request id.
-  AuditLog:
+        description: The cluster node count.
+      workloadType:
+        type: string
+        description: The workload type for the cluster.
+      cloudPlatform:
+        type: string
+        description: The cloud platform.
+      imageDetails:
+        $ref: '#/definitions/ImageDetails'
+        description: The image details.
+      environmentCrn:
+        type: string
+        description: The CRN of the environment.
+      credentialCrn:
+        type: string
+        description: The CRN of the credential.
+      datalakeCrn:
+        type: string
+        description: The CRN of the attached datalake.
+      clusterTemplateCrn:
+        type: string
+        description: The CRN of the cluster template used for the cluster creation.
+      statusReason:
+        type: string
+        description: The status reason.
+  ClusterSummary:
     type: object
-    description: Audit log represents an individual log.
+    description: Information about a cluster.
     required:
-      - createdDate
-      - log
+      - clusterName
+      - crn
     properties:
-      createdDate:
+      clusterName:
+        type: string
+        description: The name of the cluster.
+      crn:
+        type: string
+        description: The CRN of the cluster.
+      status:
+        type: string
+        description: The status of the cluster.
+      workloadType:
+        type: string
+        description: The type of cluster.
+      environmentCrn:
+        type: string
+        description: The CRN of the environment.
+      cloudPlatform:
+        type: string
+        description: The name of the cloud platform.
+      nodeCount:
+        type: integer
+        format: int32
+        description: The cluster node count.
+      creationDate:
         type: string
         format: date-time
-        description: Time at which the log is created.
-      log:
+        description: The date when the cluster was created.
+      datalakeCrn:
         type: string
-        description: Log description.
-  GetAuditEventsRequest:
-    type: object
-    description: GetAuditEventsRequest to get all audit events for a given workspace crn.
-    required:
-      - workspaceCrn
-    properties:
-      workspaceCrn:
+        description: The CRN of the attached datalake.
+      clusterTemplateCrn:
         type: string
-        description: Workspace crn for which audit events to be fetched.
-  GetAuditEventsResponse:
+        description: The CRN of the cluster template used for the cluster creation.
+  Recipe:
     type: object
-    description: GetAuditEventsResponse containes all the audit events for a given workspace crn.
+    description: Information about a recipe.
     required:
-      - auditEvents
+      - recipeName
+      - crn
     properties:
-      auditEvents:
-        description: Contains all the audit events for a given workspace crn.
-        $ref: '#/definitions/AuditEvents'
-  AuditEvents:
+      recipeName:
+        type: string
+        description: The name of the recipe.
+      crn:
+        type: string
+        description: The CRN of the recipe.
+      recipeContent:
+        type: string
+        description: The content of the recipe.
+      type:
+        type: string
+        description: 'The type of recipe. Supported values are : PRE_CLOUDERA_MANAGER_START, PRE_TERMINATION, POST_CLOUDERA_MANAGER_START, POST_CLUSTER_INSTALL.'
+      creatorCrn:
+        type: string
+        description: The CRN of the creator of the recipe.
+      description:
+        type: string
+        description: The description of the recipe.
+  RecipeSummary:
     type: object
-    description: AuditEvents contains all the audit events for a given workspace crn.
+    description: Information about a recipe.
     required:
-      - workspaceCrn
-      - events
+      - recipeName
+      - crn
     properties:
-      workspaceCrn:
+      recipeName:
         type: string
-        description: Workspace crn unique for the set of audit events.
-      events:
-        type: array
-        items:
-          $ref: '#/definitions/AuditEvent'
-        description: AuditEvent belong to the workspace crn.
-  AuditEvent:
+        description: The name of the recipe.
+      crn:
+        type: string
+        description: The CRN of the recipe.
+      type:
+        type: string
+        description: 'The type of recipe. Supported values are : PRE_CLOUDERA_MANAGER_START, PRE_TERMINATION, POST_CLOUDERA_MANAGER_START, POST_CLUSTER_INSTALL.'
+      description:
+        type: string
+        description: The description of the recipe.
+  ClusterDefinition:
     type: object
-    description: Audit event descibes an performed or performing in a given workspace.
+    description: Information about a cluster definition.
     required:
-      - workspaceCrn
-      - userCrn
-      - requestID
-      - action
-      - createdDate
+      - clusterDefinitionName
+      - crn
     properties:
-      workspaceCrn:
+      clusterDefinitionName:
         type: string
-        description: Workspace crn where the event observed.
-      userCrn:
+        description: The name of the cluster definition.
+      crn:
         type: string
-        description: UserCrn to track which user has caused the event.
-      requestID:
+        description: The CRN of the cluster definition.
+      type:
         type: string
-        description: Unique request ID to keep track of event.
-      action:
+        description: The type of cluster definition.
+      workloadTemplate:
         type: string
-        description: Action the user has generated.
-      createdDate:
+        description: The workload template.
+      cloudPlatform:
         type: string
-        format: date-time
-        description: Time at creation of event.
-  Autoscaling:
+        description: The cloud platform.
+      environmentCrn:
+        type: string
+        description: The CRN of the environment.
+      description:
+        type: string
+        description: The description of the cluster definition.
+  ClusterDefinitionSummary:
     type: object
-    description: Configuration for instance auto scaling.
+    description: Information about a cluster definition.
     required:
-      - minInstances
-      - maxInstances
+      - clusterDefinitionName
+      - crn
     properties:
-      minInstances:
-        type: integer
-        format: int32
-        description: The minimum number of instance for auto scaling.
-      maxInstances:
+      clusterDefinitionName:
+        type: string
+        description: The name of the cluster definition.
+      crn:
+        type: string
+        description: The CRN of the cluster definition.
+      type:
+        type: string
+        description: The type of cluster definition.
+      nodeCount:
         type: integer
         format: int32
-        description: The maximum number of instance for auto scaling.
-      enabled:
-        type: boolean
-        description: The boolean flag to enable the auto scaling.
-  InstanceGroup:
+        description: The node count of the cluster.
+      cloudPlatform:
+        type: string
+        description: The cloud platform.
+      productVersion:
+        type: string
+        description: The product version.
+      environmentCrn:
+        type: string
+        description: The CRN of the environment.
+      description:
+        type: string
+        description: The description of the cluster definition.
+  ClusterTemplate:
     type: object
-    description: Contains the necessary info for an instance group.
+    description: Information about a cluster template.
     required:
-      - instanceType
+      - clusterTemplateName
+      - crn
     properties:
-      instanceType:
+      clusterTemplateName:
+        type: string
+        description: The name of the cluster template.
+      crn:
         type: string
-        description: The cloud provider instance type for the node instance.
-      instanceTier:
+        description: The CRN of the cluster template.
+      description:
         type: string
-        description: The tier of the instance i.e. on-demand/spot.
-      instanceCount:
+        description: The description of the cluster template.
+      instanceGroupCount:
         type: integer
         format: int32
-        description: The initial number of instance node.
-      name:
+        description: The instance group count of the cluster.
+      status:
         type: string
-        description: The unique name of the instance group.
-      ingressRules:
+        description: The status of the cluster template.
+      tags:
         type: array
+        description: Tags added to the cluster template.
         items:
-          type: string
-        description: The networking rules for the ingress.
-      rootVolume:
-        description: The root volume of the instance.
-        $ref: '#/definitions/RootVolume'
-      autoscaling:
-        description: The auto scaling configuration.
-        $ref: '#/definitions/Autoscaling'
-  WorkspaceInstanceGroup:
+          $ref: '#/definitions/DatahubResourceTag'
+      clusterTemplateContent:
+        type: string
+        description: The content of the cluster template.
+  ClusterTemplateSummary:
     type: object
-    description: Instance group information to show in workspace details.
+    description: Information about a cluster template.
     required:
-      - instanceType
-      - instanceCount
-      - instanceGroupName
-      - minInstances
-      - maxInstances
-      - instances
-      - tags
+      - clusterTemplateName
+      - crn
     properties:
-      instanceType:
+      clusterTemplateName:
         type: string
-        description: The cloud provider instance type for the node instance.
-      instanceCount:
-        type: integer
-        format: int32
-        description: The initial number of instance node.
-      instanceGroupName:
+        description: The name of the cluster template.
+      crn:
         type: string
-        description: The unique name of the instance group.
-      minInstances:
-        type: integer
-        format: int32
-        description: The minimum number of instances that can be deployed to this instance group. If the value is 0, the group might be empty.
-      maxInstances:
+        description: The CRN of the cluster template.
+      description:
+        type: string
+        description: The description of the cluster template.
+      productVersion:
+        type: string
+        description: The product version.
+      instanceGroupCount:
         type: integer
         format: int32
-        description: The maximum number of instances that can be deployed to this instance group.
-      instances:
-        type: array
-        items:
-          $ref: '#/definitions/Instance'
-        description: Instances in the instance group.
+        description: The instance group count of the cluster.
+      status:
+        type: string
+        description: The status of the cluster template.
       tags:
         type: array
+        description: Tags added to the cluster template.
         items:
-          $ref: '#/definitions/Tag'
-        description: Tags are key/value pairs that are applied to all tag-able resources deployed in the workspace's cloud environment.
-  Instance:
+          $ref: '#/definitions/DatahubResourceTag'
+  ListClustersRequest:
     type: object
-    description: Represents each instance in an instance group.
-    required:
-      - instanceId
-      - availabilityZone
+    description: Request object for list clusters request.
     properties:
-      instanceId:
-        type: string
-        description: Unique instance Id generated by the cloud provider.
-      availabilityZone:
+      environmentName:
         type: string
-        description: Availability zone the instance belongs to.
-  Tag:
+        description: The name or CRN of the environment for which the clusters will be listed.
+  ListClustersResponse:
     type: object
-    description: Contains a single tag entry associated with a workspace.
+    description: Response object for list clusters request.
     required:
-      - key
-      - value
+      - clusters
     properties:
-      key:
-        type: string
-        description: The name for the tag.
-      value:
-        type: string
-        description: The value for the tag.
-  ProvisionTag:
+      clusters:
+        type: array
+        items:
+          $ref: '#/definitions/ClusterSummary'
+        description: The clusters.
+  AttachedVolumeRequest:
     type: object
-    description: Contains a single tag entry that will be configured on cloud resources associated with a workspace.
+    description: Configurations for additional attached volumes.
     required:
-      - key
-      - value
+      - volumeSize
+      - volumeCount
+      - volumeType
     properties:
-      key:
+      volumeSize:
+        type: integer
+        format: int32
+        description: The attached volume size.
+      volumeCount:
+        type: integer
+        format: int32
+        description: The attached volume count.
+      volumeType:
         type: string
-        description: The name for the tag.
-      value:
+        description: The attached volume type.
+  VolumeEncryptionRequest:
+    type: object
+    description: Configurations for volume encryption.
+    properties:
+      enableEncryption:
+        type: boolean
+        description: Enable encyrption for all volumes in the instance group. Default is false.
+      encryptionKey:
         type: string
-        description: The value for the tag.
-  ProvisionK8sRequest:
+        description: The ARN of the encryption key to use. If nothing is specified, the default key will be used.
+  InstanceGroupRequest:
     type: object
-    description: Request object for workspace provision.
+    description: Configurations for instance group
     required:
-      - instanceGroups
-      - environmentName
+      - nodeCount
+      - instanceGroupName
+      - instanceGroupType
+      - instanceType
+      - rootVolumeSize
+      - attachedVolumeConfiguration
     properties:
-      instanceGroups:
-        type: array
-        items:
-          $ref: '#/definitions/InstanceGroup'
-        description: The instance groups.
-      environmentName:
+      nodeCount:
+        type: integer
+        format: int32
+        description: Number of instances in the instance group
+      instanceGroupName:
         type: string
-        description: The name of the environment for the workspace to create.
-      tags:
+        description: The instance group name.
+      instanceGroupType:
+        type: string
+        description: The instance group type.
+      instanceType:
+        type: string
+        description: The cloud provider specific instance type to be used.
+      rootVolumeSize:
+        type: integer
+        format: int32
+        description: The root volume size.
+      attachedVolumeConfiguration:
         type: array
         items:
-          $ref: '#/definitions/ProvisionTag'
-        description: Tags to add to the cloud provider resources created. This is in addition to any tags added by Cloudera.
-      network:
-        description: The overlay network for an AWS Kubernetes cluster's CNI.
-        $ref: '#/definitions/OverlayNetwork'
-  OverlayNetwork:
-    type: object
-    description: Contains the information about overlay network.
-    properties:
-      plugin:
-        type: string
-        description: 'The plugin specifies specific cni vendor, ex: calico, weave etc.'
-      topology:
-        description: The options for overlay topology.
-        $ref: '#/definitions/Topology'
-  Topology:
-    type: object
-    description: Contains the information about topology.
-    properties:
-      subnets:
+          $ref: '#/definitions/AttachedVolumeRequest'
+        description: The attached volume configuration. This does not include root volume.
+      recipeNames:
         type: array
         items:
           type: string
-        description: The options for subnets.
-  ExistingDatabaseConfig:
+        description: The names or CRNs of the recipes that would be applied to the instance group.
+      recoveryMode:
+        type: string
+        description: Recovery mode for the instance group.
+      volumeEncryption:
+        $ref: '#/definitions/VolumeEncryptionRequest'
+        description: The volume encryption settings. This setting does not apply to Azure which always encrypts volumes.
+  CreateAWSClusterRequest:
     type: object
-    description: Configurations for bringing an existing database for model metrics
+    description: Request object for create AWS cluster request.
     properties:
-      existingDatabaseHost:
+      clusterName:
         type: string
-        description: Optionally provide a Postgresql database host to export model metrics to.
-      existingDatabasePort:
+        description: The name of the cluster. This name must be unique, must have between 5 and 40 characters, and must contain only lowercase letters, numbers and hyphens. Names are case-sensitive.
+        minLength: 5
+        maxLength: 40
+      clusterDefinitionName:
         type: string
-        description: Optionally provide a Postgresql database port to export model metrics to.
-      existingDatabaseName:
+        description: The name or CRN of the cluster definition to use for cluster creation.
+      environmentName:
         type: string
-        description: Optionally provide a Postgresql database name to export model metrics to.
-      existingDatabaseUser:
+        description: Name or CRN of the environment to use when creating the cluster. The environment must be an AWS environment.
+      clusterTemplateName:
         type: string
-        description: Optionally provide a Postgresql database user to use when exporting model metrics.
-      existingDatabasePassword:
+        description: Name or CRN of the cluster template to use for cluster creation.
+      instanceGroups:
+        type: array
+        items:
+          $ref: '#/definitions/InstanceGroupRequest'
+        description: Instance group details.
+      subnetId:
+        type: string
+        description: The subnet ID.
+      image:
+        $ref: '#/definitions/ImageRequest'
+        description: The image to be used for cluster creation.
+      tags:
+        type: array
+        description: Tags to be added to Datahub related resources.
+        items:
+          $ref: '#/definitions/DatahubResourceTagRequest'
+      requestTemplate:
         type: string
-        description: Optionally provide a Postgresql database password to use when exporting model metrics.
-        x-sensitive: true
-  CreateWorkspaceRequest:
+        description: JSON template to use for cluster creation. This is different from cluster template and would be removed in the future.
+  CreateAWSClusterResponse:
     type: object
-    description: Request object for the CreateWorkspace method.
+    description: Response object for create AWS cluster request.
     required:
-      - environmentName
-      - workspaceName
+      - cluster
     properties:
-      environmentName:
+      cluster:
+        $ref: '#/definitions/Cluster'
+        description: The cluster.
+  CreateAzureClusterRequest:
+    type: object
+    description: Request object for create Azure cluster request.
+    properties:
+      clusterName:
         type: string
-        description: The environment for the workspace to create.
-      workspaceName:
+        description: The name of the cluster. This name must be unique, must have between 5 and 40 characters, and must contain only lowercase letters, numbers and hyphens. Names are case-sensitive.
+        minLength: 5
+        maxLength: 40
+      clusterDefinitionName:
         type: string
-        description: The name of the workspace to create.
-      usePublicLoadBalancer:
-        type: boolean
-        description: The boolean flag to request public load balancer. By default, private load balancer is used.
-      disableTLS:
-        type: boolean
-        description: The boolean flag to disable TLS setup for workspace. By default, the TLS is enabled.
-      provisionK8sRequest:
-        description: The request for Kubernetes workspace provision. Required in public cloud.
-        $ref: '#/definitions/ProvisionK8sRequest'
-      enableMonitoring:
-        type: boolean
-        description: The boolean flag is used to enable monitoring. By default, monitoring is disabled.
-      enableGovernance:
-        type: boolean
-        description: Enables Cloudera Machine Learning governance by integrating with Cloudera Atlas. By default, this flag is disabled.
-      existingNFS:
+        description: The name or CRN of the cluster definition to use for cluster creation.
+      environmentName:
         type: string
-        description: Optionally use an existing NFS by providing the hostname and desired path (Azure and Private Cloud only).
-      loadBalancerIPWhitelists:
-        type: array
-        items:
-          type: string
-        description: The whitelist of IPs for load balancer.
-      nfsVersion:
+        description: Name or CRN of the environment to use when creating the cluster. The environment must be an Azure environment.
+      clusterTemplateName:
         type: string
-        description: The NFS Protocol version of the NFS server we are using for Azure and Private Cloud.
-      enableModelMetrics:
-        type: boolean
-        description: Enables the model metrics service for exporting metrics for models to a metrics store.
-      existingDatabaseConfig:
-        description: Optional configurations for an existing Postgres to export model metrics to.
-        $ref: '#/definitions/ExistingDatabaseConfig'
-      whitelistAuthorizedIPRanges:
-        type: boolean
-        description: Whether to whitelist only 'authorizedIPRanges' given or all public IPs.
-      authorizedIPRanges:
-        type: array
-        items:
-          type: string
-        description: The whitelist of CIDR blocks which can access the API server.
-      skipValidation:
-        type: boolean
-        description: Skip pre-flight validations if requested
-      subnetsForLoadBalancers:
+        description: Name or CRN of the cluster template to use for cluster creation.
+      instanceGroups:
         type: array
         items:
-          type: string
-        description: The list of subnets used for the load balancer that CML creates.
-      staticSubdomain:
-        type: string
-        description: The static subdomain to be used for the workspace.
-      cdswMigrationMode:
-        type: string
-        description: Toggle for cdsw migration preflight validation
-      outboundTypes:
+          $ref: '#/definitions/InstanceGroupRequest'
+        description: Instance group details.
+      subnetId:
+        type: string
+        description: The subnet ID.
+      image:
+        $ref: '#/definitions/ImageRequest'
+        description: The image to be used for cluster creation.
+      tags:
         type: array
+        description: Tags to be added to Datahub related resources.
         items:
-          $ref: '#/definitions/OutboundTypes'
-        description: Outbound Types provided for the workspace.
-  OutboundTypes:
-    type: string
-    description: List of possible Outbound types.
-    enum:
-      - UNKNOWN
-      - OUTBOUND_TYPE_UDR
-  RestoreWorkspaceRequest:
-    type: object
-    description: Request object for RestoreWorkspace method.
-    properties:
-      newWorkspaceParameters:
-        description: The parameters required for a new Cloudera Machine Learning workspace.
-        $ref: '#/definitions/CreateWorkspaceRequest'
-      backupCrn:
+          $ref: '#/definitions/DatahubResourceTagRequest'
+      requestTemplate:
         type: string
-        description: The CRN of the backup snapshot to used for restoring.
-      useStaticSubdomain:
-        type: boolean
-        description: A boolean value to check if subdomain must be used or not.
-      restoreJobTimeoutMinutes:
-        type: integer
-        format: int32
-        description: The timeout to restore the backup snapshots, in minutes.
-  CreateWorkspaceResponse:
+        description: JSON template to use for cluster creation. This is different from cluster template and would be removed in the future.
+  CreateAzureClusterResponse:
     type: object
-    description: Response object for the CreateWorkspace method.
-  RestoreWorkspaceResponse:
-    type: object
-    description: Response object for the RestoreWorkspace method.
+    description: Response object for create Azure cluster request.
+    required:
+      - cluster
     properties:
-      workspaceCrn:
-        type: string
-        description: The CRN of the Cloudera Machine Learning workspace being provisioned.
-  ListWorkspacesRequest:
+      cluster:
+        $ref: '#/definitions/Cluster'
+        description: The cluster.
+  DeleteClusterRequest:
     type: object
-    description: Request object for the ListWorkspaces method.
+    description: Request object for delete cluster request.
+    required:
+      - clusterName
     properties:
-      queryOptions:
-        type: array
-        items:
-          type: string
-        description: Additional query options.
-  ListWorkspacesResponse:
+      clusterName:
+        type: string
+        description: The name or CRN of the cluster to be deleted.
+      force:
+        type: boolean
+        description: Whether the cluster should be force deleted. This option can be used when cluster deletion fails. This removes the entry from Cloudera Datahub service. Any lingering resources have to be deleted from the cloud provider manually. The default is false.
+  DeleteClusterResponse:
     type: object
-    description: Response object for the ListWorkspaces method.
-    properties:
-      workspaces:
-        type: array
-        items:
-          $ref: '#/definitions/WorkspaceSummary'
-        description: The list of workspaces.
-  ListWorkspaceBackupsQueryOptions:
+    description: Response object for delete cluster request.
+  DescribeClusterRequest:
     type: object
-    description: Query options object for ListWorkspaceBackups method.
+    description: Request object for describe cluster request.
+    required:
+      - clusterName
     properties:
-      expandEnvironmentMetadata:
-        type: boolean
-        description: When set to true, will return the metadata of the environment where the backed-up workspace is/was present.
-  ListWorkspaceBackupsRequest:
+      clusterName:
+        type: string
+        description: The name or CRN of the cluster.
+  DescribeClusterResponse:
     type: object
-    description: Request object for ListWorkspaceBackups method.
+    description: Response object for describe cluster request.
+    required:
+      - cluster
     properties:
-      environmentName:
-        type: string
-        description: The environment for the workspace to list backups for.
-      workspaceName:
-        type: string
-        description: The name of the workspace to list backups for.
-      workspaceCrn:
-        type: string
-        description: The CRN of the workspace to list backups for. If this field is specified, environmentName and workspaceName are ignored.
-      queryOptions:
-        description: Additional query options to enhance/mutate the API response.
-        $ref: '#/definitions/ListWorkspaceBackupsQueryOptions'
-  BackupDetail:
+      cluster:
+        $ref: '#/definitions/Cluster'
+        description: The cluster.
+  GetClusterServiceStatusRequest:
     type: object
-    description: Backup Detail response object for listing backups.
+    description: Request object to get service status.
+    required:
+      - clusterName
     properties:
-      backupCrn:
-        type: string
-        description: The CRN of the backup snapshot.
-      backupName:
-        type: string
-        description: The name of the backup snapshot.
-      createdAt:
-        type: string
-        format: date-time
-        description: The creation time of the backup snapshot.
-      creatorCrn:
+      clusterName:
         type: string
-        description: The CRN of the creator.
-      workspaceVersionAtBackup:
-        type: string
-        description: The version of the backed-up workspace at the time of backup.
-      backupStatus:
-        type: string
-        description: The status of the backup.
-  ListWorkspaceBackupsResponse:
+        description: The name or CRN of the cluster.
+  GetClusterServiceStatusResponse:
     type: object
-    description: Response object for ListWorkspaceBackups method.
+    description: Response object to get service status.
+    required:
+      - services
     properties:
-      backups:
+      services:
         type: array
         items:
-          $ref: '#/definitions/BackupDetail'
-        description: The list of backups along with their details.
-  UpgradeState:
+          $ref: '#/definitions/ServiceStatus'
+        description: The cluster services health.
+  ServiceStatus:
     type: object
-    description: Response object for the workspace summary.
+    description: Information about a cluster service.
     properties:
+      type:
+        type: string
+        description: The service type.
       state:
         type: string
-        description: The current upgrade state of the workspace.
-      reason:
+        description: The service state.
+      healthSummary:
         type: string
-        description: The reason for the current state.
-  BackupMetadata:
+        description: The service health summary.
+      healthChecks:
+        type: array
+        items:
+          $ref: '#/definitions/HealthCheck'
+        description: The service health checks.
+  HealthCheck:
     type: object
-    description: Backup metadata response object for the workspace summary.
+    description: The result of a health check.
     properties:
-      backupVaultName:
-        type: string
-        description: The backup vault name.
-      lastSuccessfulBackupTime:
+      name:
         type: string
-        format: date-time
-        description: The time when the last successful backup was taken.
-      isSuccessfulBackupAvailable:
-        type: boolean
-        description: Whether successful backups are available for the workspace.
-      lastBackupStatus:
+        description: The name of service health check.
+      summary:
         type: string
-        description: The status of the last backup initiated.
-      numberOfAvailableBackups:
-        type: integer
-        format: int64
-        description: The number of backups available.
-  WorkspaceSummary:
-    type: object
-    description: A Cloudera Machine Learning workspace which includes the deployed configuration details.
-    required:
-      - instanceName
-      - environmentName
-      - instanceStatus
-      - instanceUrl
-      - environmentCrn
-      - crn
-      - k8sClusterName
-      - creatorCrn
-      - version
-      - httpsEnabled
-      - filesystemID
-      - cloudPlatform
-      - monitoringEnabled
+        description: The service health check summary.
+  GetClusterHostStatusRequest:
+    type: object
+    description: Request object to get host status.
+    required:
+      - clusterName
     properties:
-      instanceName:
-        type: string
-        description: The name of the workspace.
-      environmentName:
-        type: string
-        description: The name of the workspace's environment.
-      instanceStatus:
-        type: string
-        description: The workspace's current status.
-      instanceUrl:
-        type: string
-        description: URL of the workspace's user interface.
-      environmentCrn:
-        type: string
-        description: CRN of the environment.
-      crn:
-        type: string
-        description: The CRN of the workspace.
-      k8sClusterName:
-        type: string
-        description: The Kubernetes cluster name.
-      creatorCrn:
-        type: string
-        description: The CRN of the creator of the workspace.
-      version:
-        type: string
-        description: The version of Cloudera Machine Learning that was installed on the workspace.
-      httpsEnabled:
-        type: boolean
-        description: Indicates if HTTPs communication was enabled on this workspace when provisioned.
-      filesystemID:
-        type: string
-        description: A filesystem ID referencing the filesystem that was created on the cloud provider environment that this workspace uses.
-      cloudPlatform:
-        type: string
-        description: The cloud platform of the environment that was used to create this workspace.
-      monitoringEnabled:
-        type: boolean
-        description: If usage monitoring is enabled or not on this workspace.
-      loadBalancerIPWhitelists:
-        type: array
-        items:
-          type: string
-        description: The whitelist of IPs for load balancer.
-      creationDate:
+      clusterName:
         type: string
-        format: date-time
-        description: Creation date of workspace.
-      failureMessage:
-        type: string
-        description: Failure message from the most recent failure that has occurred during workspace provisioning.
-      healthInfoLists:
-        type: array
-        items:
-          $ref: '#/definitions/HealthInfo'
-        description: The health info information of the workspace.
-      upgradeState:
-        description: The upgrade state contains the workspace upgrade information.
-        $ref: '#/definitions/UpgradeState'
-      nfsVersion:
-        type: string
-        description: NFS Version of the filesystem.
-      backupMetadata:
-        description: The Backup Metadata for the workspace.
-        $ref: '#/definitions/BackupMetadata'
-      clusterID:
-        type: string
-        description: The Cluster ID for the workspace.
-      isPrivate:
-        type: boolean
-        description: The value to indicate if the cluster is private or not.
-  Workspace:
+        description: The name or CRN of the cluster.
+  GetClusterHostStatusResponse:
     type: object
-    description: A ML workspace, which includes the cluster and storage.
+    description: Response object for getting host status.
     required:
-      - instanceName
-      - environmentName
-      - instanceStatus
-      - instanceUrl
-      - environmentCrn
-      - crn
-      - k8sClusterName
-      - creatorCrn
-      - version
-      - httpsEnabled
-      - endpointPublicAccess
-      - filesystemID
-      - tags
-      - instanceGroups
-      - cloudPlatform
-      - monitoringEnabled
+      - hosts
     properties:
-      instanceName:
-        type: string
-        description: The name of the workspace.
-      environmentName:
-        type: string
-        description: The name of the workspace's environment.
-      instanceStatus:
-        type: string
-        description: The workspace's current status.
-      instanceUrl:
-        type: string
-        description: URL of the workspace's user interface.
-      environmentCrn:
-        type: string
-        description: CRN of the environment.
-      crn:
-        type: string
-        description: The CRN of the workspace.
-      k8sClusterName:
-        type: string
-        description: The Kubernetes cluster name.
-      creatorCrn:
-        type: string
-        description: The CRN of the creator of the workspace.
-      version:
-        type: string
-        description: The version of Cloudera Machine Learning that was installed on the workspace.
-      httpsEnabled:
-        type: boolean
-        description: To Display if Https is enabled or not.
-      endpointPublicAccess:
-        type: boolean
-        description: To check if the cluster is publicly accessible or not.
-      filesystemID:
-        type: string
-        description: filesystemID used by the workspace
-      tags:
+      hosts:
         type: array
         items:
-          $ref: '#/definitions/Tag'
-        description: Tags provided by the user at the time of workspace creation.
-      instanceGroups:
-        type: array
-        items:
-          $ref: '#/definitions/WorkspaceInstanceGroup'
-        description: The instance groups.
-      cloudPlatform:
-        type: string
-        description: The cloud platform of the environment that was used to create this workspace.
-      monitoringEnabled:
-        type: boolean
-        description: If usage monitoring is enabled or not on this workspace.
-      loadBalancerIPWhitelists:
-        type: array
-        items:
-          type: string
-        description: IP whitelist for loadBalancer.
-      creationDate:
+          $ref: '#/definitions/HostStatus'
+        description: The cluster hosts status.
+  HostStatus:
+    type: object
+    description: Information about cluster host status.
+    properties:
+      hostid:
         type: string
-        format: date-time
-        description: Creation date of workspace.
-      healthInfoLists:
-        type: array
-        items:
-          $ref: '#/definitions/HealthInfo'
-        description: The health info information of the workspace.
-      failureMessage:
+        description: Unique identifier of the cluster host given by Cloudera Manager.
+      hostname:
         type: string
-        description: Failure message from the most recent failure that has occurred during workspace provisioning.
-      clusterBaseDomain:
+        description: The cluster hostname.
+      healthSummary:
         type: string
-        description: The basedomain of the cluster.
-      modelMetricsEnabled:
-        type: boolean
-        description: Whether model metrics is enabled.
-      governanceEnabled:
-        type: boolean
-        description: Whether governance is enabled.
-      subnets:
-        type: array
-        items:
-          type: string
-        description: The subnets of the workspace.
-      whitelistAuthorizedIPRanges:
-        type: boolean
-        description: Whether to whitelist only 'authorizedIPRanges' given or all public IPs.
-      authorizedIPRanges:
-        type: array
-        items:
-          type: string
-        description: The whitelist of CIDR blocks which can access the API server.
-      nfsVersion:
-        type: string
-        description: NFS Version of the filesystem.
-      subnetsForLoadBalancers:
+        description: The host health summary.
+  RepairInstancesRequest:
+    type: object
+    description: Details for repair instances.
+    properties:
+      instanceIds:
         type: array
         items:
           type: string
-        description: The list of subnets used for the load balancer that CML creates.
-      upgradeState:
-        description: The upgrade state contains the workspace upgrade information.
-        $ref: '#/definitions/UpgradeState'
-      backupMetadata:
-        description: The Backup MetaData for this Workspace
-        $ref: '#/definitions/BackupMetadata'
-      clusterID:
-        type: string
-        description: The Cluster ID for the workspace.
-      isPrivate:
+        description: List of instance ids.
+      deleteVolumes:
         type: boolean
-        description: The value to indicate if the cluster is private or not.
-  UpgradeWorkspaceRequest:
+        description: The existing disk volumes on the instances will be re-created if the deleteVolumes is true. Otherwise, the volumes will be reattached to the new instances.
+  StartClusterRequest:
     type: object
-    description: Request object for the UpgradeWorkspace method.
+    description: Request object for start cluster request.
+    required:
+      - clusterName
     properties:
-      environmentName:
-        type: string
-        description: The environment of the workspace.
-      workspaceName:
-        type: string
-        description: The name of the workspace.
-      mlVersion:
-        type: string
-        description: The version of workspace to upgrade to. (Deprecated).
-        x-deprecated: true
-      workspaceCrn:
+      clusterName:
         type: string
-        description: The CRN of the workspace. If CRN is specified only the CRN is used for identifying the workspace, environment and name arguments are ignored.
-  UpgradeWorkspaceResponse:
+        description: The name or CRN of the cluster to be started.
+  StartClusterResponse:
     type: object
-    description: Response object for the UpgradeWorkspace method.
-  DescribeWorkspaceRequest:
+    description: Response object for start cluster request.
+  StopClusterRequest:
     type: object
-    description: Request object for the DescribeWorkspace method.
+    description: Request object for stop cluster request.
+    required:
+      - clusterName
     properties:
-      environmentName:
-        type: string
-        description: The environment for the workspace to describe.
-      workspaceName:
-        type: string
-        description: The name of the workspace to describe.
-      workspaceCrn:
+      clusterName:
         type: string
-        description: The CRN of the workspace to describe. If CRN is specified only the CRN is used for identifying the workspace, environment and name arguments are ignored.
-  DescribeWorkspaceResponse:
+        description: The name or CRN of the cluster to be stopped.
+  StopClusterResponse:
     type: object
-    description: Response object for the DescribeWorkspace method.
-    required:
-      - workspace
-    properties:
-      workspace:
-        description: The workspace.
-        $ref: '#/definitions/Workspace'
-  DeleteInstanceGroupRequest:
+    description: Response object for stop cluster request.
+  RetryClusterRequest:
     type: object
-    description: Request object for the DeleteInstanceGroup method.
+    description: Request object for retry cluster request.
     required:
-      - workspaceCrn
-      - instanceGroupName
+      - clusterName
     properties:
-      workspaceCrn:
+      clusterName:
         type: string
-        description: The CRN of the workspace from which instance group is to be deleted.
-      instanceGroupName:
-        type: string
-        description: The instance group that we want to delete from the workspace.
-  DeleteInstanceGroupResponse:
+        description: The name or CRN of the cluster for which the operations need to be retried.
+  RetryClusterResponse:
     type: object
-    description: Response object for the DeleteInstanceGroup method.
-  DeleteWorkspaceRequest:
+    description: Response object for retry cluster request.
+  RepairClusterRequest:
     type: object
-    description: Request object for the DeleteWorkspace method.
+    description: Request object for repair cluster request.
     required:
-      - force
+      - clusterName
     properties:
-      force:
-        type: boolean
-        description: Force delete a workspace even if errors occur during deletion. Force delete removes the guarantee that resources in your cloud account will be cleaned up.
-      removeStorage:
-        type: boolean
-        description: The remove storage flag indicates weather to keep the backing workspace filesystem storage or remove it during delete.
-      environmentName:
-        type: string
-        description: The environment for the workspace to delete.
-      workspaceName:
+      clusterName:
         type: string
-        description: The name of the workspace to delete.
-      workspaceCrn:
-        type: string
-        description: The CRN of the workspace to delete. If CRN is specified only the CRN is used for identifying the workspace, environment and name arguments are ignored.
-  DeleteWorkspaceResponse:
+        description: The name or CRN of the cluster to be repaired.
+      instanceGroupNames:
+        type: array
+        items:
+          type: string
+        description: List of instance groups where the failed instances will be repaired.
+      instances:
+        $ref: '#/definitions/RepairInstancesRequest'
+        description: List of instances.
+      removeOnly:
+        type: boolean
+        description: If true, the failed instances will only be removed, otherwise the failed instances will be removed and new instances will be started.
+  RepairClusterResponse:
     type: object
-    description: Response object for the DeleteWorkspace method.
-  GrantWorkspaceAccessRequest:
+    description: Response object for repair cluster request.
+  SyncClusterRequest:
     type: object
-    description: Request object for the GrantWorkspaceAccess method.
+    description: Request object for sync cluster request.
+    required:
+      - clusterName
     properties:
-      arn:
+      clusterName:
         type: string
-        description: 'The aws user ARN to grant access to the corresponding EKS cluster. (Deprecated: Use identifier instead).'
-        x-deprecated: true
-      environmentName:
-        type: string
-        description: The environment that the workspace is a member of.
-      workspaceName:
-        type: string
-        description: The name of the workspace to grant access to.
-      workspaceCrn:
-        type: string
-        description: The CRN of the workspace to grant access to. If CRN is specified only the CRN is used for identifying the workspace, environment and name arguments are ignored.
-      identifier:
-        type: string
-        description: The cloud provider user id which will be granted access to the workspace's Kubernetes cluster.
-  GrantWorkspaceAccessResponse:
+        description: The name or CRN of the cluster to be synced.
+  SyncClusterResponse:
     type: object
-    description: Response object for the GrantWorkspaceAccess method.
+    description: Response object for sync cluster request.
+  ScaleClusterRequest:
+    type: object
+    description: Request object for scale cluster request.
     required:
-      - kubeconfig
+      - clusterName
+      - instanceGroupName
+      - instanceGroupDesiredCount
     properties:
-      kubeconfig:
+      clusterName:
         type: string
-        description: The Kubernetes config file
-        x-sensitive: true
-  RevokeWorkspaceAccessRequest:
+        description: The name or CRN of the cluster to be scaled.
+      instanceGroupName:
+        type: string
+        description: The name of the instance group which needs to be scaled.
+      instanceGroupDesiredCount:
+        type: integer
+        format: int32
+        description: The desired number of instances in the instance group.
+  ScaleClusterResponse:
+    type: object
+    description: Response object for scale cluster request.
+  CreateRecipeRequest:
     type: object
-    description: Request object for the RevokeWorkspace method.
+    description: Request object for create recipe request.
+    required:
+      - recipeName
+      - recipeContent
+      - type
     properties:
-      arn:
-        type: string
-        description: 'The aws user ARN to revoke access to the corresponding EKS cluster. (Deprecated: Use identifier instead).'
-        x-deprecated: true
-      environmentName:
+      recipeName:
         type: string
-        description: The environment that the workspace is a member of.
-      workspaceName:
+        description: The name of the recipe. This name must be unique, must have between 5 and 100 characters, and must contain only lowercase letters, numbers and hyphens. Names are case-sensitive.
+        minLength: 5
+        maxLength: 1000
+      recipeContent:
         type: string
-        description: The name of the workspace to revoke access to.
-      workspaceCrn:
+        description: The content of the recipe.
+      type:
         type: string
-        description: The CRN of the workspace to revoke access to. If CRN is specified only the CRN is used for identifying the workspace, environment and name arguments are ignored.
-      identifier:
+        description: 'The type of recipe. Supported values are : PRE_CLOUDERA_MANAGER_START, PRE_TERMINATION, POST_CLOUDERA_MANAGER_START, POST_CLUSTER_INSTALL.'
+      description:
         type: string
-        description: The cloud provider user id which will be granted access to the workspace's Kubernetes cluster.
-  RevokeWorkspaceAccessResponse:
+        description: The description of the recipe. The description can have a maximum of 1000 characters.
+        maxLength: 1000
+  CreateRecipeResponse:
     type: object
-    description: Response object for the RevokeWorkspaceAccess method.
-  ListWorkspaceAccessRequest:
-    type: object
-    description: Request object for the ListWorkspace method.
+    description: Response object for create recipe request.
+    required:
+      - recipe
     properties:
-      environmentName:
-        type: string
-        description: The environment that the workspace is a member of.
-      workspaceName:
-        type: string
-        description: The name of the workspace to list access.
-      workspaceCrn:
-        type: string
-        description: The CRN of the workspace to list access. If CRN is specified only the CRN is used for identifying the workspace, environment and name arguments are ignored.
-  ListWorkspaceAccessResponse:
+      recipe:
+        $ref: '#/definitions/Recipe'
+        description: The recipe.
+  DeleteRecipesRequest:
     type: object
-    description: Response object for the ListWorkspaceAccess method.
+    description: Request object for delete recipe request.
     required:
-      - users
+      - recipeNames
     properties:
-      users:
+      recipeNames:
         type: array
         items:
           type: string
-          x-sensitive: true
-        description: The list of users that have access.
-        x-sensitive: true
-  GetKubeconfigRequest:
+        description: The names or CRNs of the recipes to be deleted.
+  DeleteRecipesResponse:
     type: object
-    description: Request object for the GetKubeconfig method.
+    description: Response object for delete recipe request.
+    required:
+      - recipes
     properties:
-      environmentName:
-        type: string
-        description: The environment that the workspace is a member of.
-      workspaceName:
-        type: string
-        description: The name of the workspace to list access.
-      workspaceCrn:
-        type: string
-        description: The CRN of the workspace to list access.
-  GetKubeconfigResponse:
+      recipes:
+        type: array
+        items:
+          $ref: '#/definitions/Recipe'
+        description: The recipes.
+  DescribeRecipeRequest:
     type: object
-    description: Response object for the GetKubeconfig method.
+    description: Request object for describe recipe request.
     required:
-      - kubeconfig
+      - recipeName
     properties:
-      kubeconfig:
+      recipeName:
         type: string
-        description: The list of users that have access.
-        x-sensitive: true
-  GetLatestWorkspaceVersionRequest:
+        description: The name or CRN of the recipe.
+  DescribeRecipeResponse:
     type: object
-    description: Request object for GetLatestWorkspaceVersion.
-  GetLatestWorkspaceVersionResponse:
-    type: object
-    description: Response object for GetLatestWorkspaceVersion.
+    description: Response object for describe recipe request.
     required:
-      - version
+      - recipe
     properties:
-      version:
-        type: string
-        description: The latest version of a workspace that is used when deploying Cloudera Machine Learning workspaces.
-  HealthInfo:
+      recipe:
+        $ref: '#/definitions/Recipe'
+        description: The recipe.
+  ListRecipesRequest:
     type: object
-    description: Healthinfo object contains the health information of a resource.
+    description: Request object for list recipes request.
+  ListRecipesResponse:
+    type: object
+    description: Response object for list recipes request.
     required:
-      - resourceName
-      - isHealthy
-      - updatedAt
-      - message
-      - details
+      - recipes
     properties:
-      resourceName:
-        type: string
-        description: The resource name being checked.
-      isHealthy:
-        type: boolean
-        description: The boolean that indicates the health status.
-      updatedAt:
-        type: string
-        format: date-time
-        description: The timestamp for the heartbeat.
-      message:
-        type: string
-        description: The message to show for the health info.
-      details:
+      recipes:
         type: array
         items:
-          type: string
-        description: The detail of the health info.
-  ModifyClusterInstanceGroupRequest:
+          $ref: '#/definitions/RecipeSummary'
+        description: The recipes.
+  CreateClusterDefinitionRequest:
     type: object
-    description: Request object for ModifyClusterInstanceGroup.
+    description: Request object for create cluster definition request.
     required:
-      - workspaceCrn
-      - instanceGroupName
-      - min
-      - max
-      - instanceType
+      - clusterDefinitionName
+      - workloadTemplate
     properties:
-      workspaceCrn:
+      clusterDefinitionName:
         type: string
-        description: The CRN of the workspace cluster to modify.
-      instanceGroupName:
+        description: The name of the cluster definition. This name must be unique, must have between 5 and 100 characters, and must contain only lowercase letters, numbers and hyphens. Names are case-sensitive.
+        minLength: 5
+        maxLength: 1000
+      workloadTemplate:
         type: string
-        description: The name of the instance group of the workspace cluster to modify.
-      min:
-        type: integer
-        format: int32
-        description: The desired autoscaling min of the workspace cluster instance group.
-      max:
-        type: integer
-        format: int32
-        description: The desired autoscaling min of the workspace cluster instance group.
-      instanceType:
+        description: The workload template.
+      description:
         type: string
-        description: The desired instance type of the workspace cluster instance group.
-  ModifyClusterInstanceGroupResponse:
+        description: The description of the cluster definition. The description can have a maximum of 1000 characters.
+        maxLength: 1000
+  CreateClusterDefinitionResponse:
     type: object
-    description: Response object for ModifyClusterInstanceGroup.
-  ModifyClusterSecurityRequest:
+    description: Response object for create cluster definition request.
+    required:
+      - clusterDefinition
+    properties:
+      clusterDefinition:
+        $ref: '#/definitions/ClusterDefinition'
+        description: The clusterDefinition.
+  DeleteClusterDefinitionsRequest:
     type: object
-    description: Request object for ModifyClusterSecurity.
+    description: Request object for delete cluster definition request.
     required:
-      - workspaceCrn
-      - allowlistAuthorizedIPRanges
-      - authorizedIPRanges
+      - clusterDefinitionNames
     properties:
-      workspaceCrn:
-        type: string
-        description: The CRN of the workspace cluster to modify.
-      allowlistAuthorizedIPRanges:
-        type: boolean
-        description: Whether to allow only authorized IP ranges given or all public IPs.
-      authorizedIPRanges:
+      clusterDefinitionNames:
         type: array
         items:
           type: string
-        description: The allowlist of CIDR blocks which can access the API server.
-  ModifyClusterSecurityResponse:
-    type: object
-    description: Response object for ModifyClusterSecurity.
-  ModifyWorkspaceLoadBalancerRequest:
+        description: The name or CRN of the cluster definitions to be deleted.
+  DeleteClusterDefinitionsResponse:
     type: object
-    description: Request object for ModifyWorkspaceLoadBalancer.
+    description: Response object for delete cluster definition request.
     required:
-      - workspaceCrn
-      - loadBalancerIPAllowLists
+      - clusterDefinitions
     properties:
-      workspaceCrn:
-        type: string
-        description: The CRN of the workspace cluster to modify.
-      loadBalancerIPAllowLists:
+      clusterDefinitions:
         type: array
         items:
-          type: string
-        description: The allowlist of CIDR blocks which can access the loadbalancer.
-  ModifyWorkspaceLoadBalancerResponse:
+          $ref: '#/definitions/ClusterDefinition'
+        description: The clusterDefinitions.
+  DescribeClusterDefinitionRequest:
     type: object
-    description: Response object for ModifyWorkspaceLoadBalancer.
-  SuspendWorkspaceRequest:
-    type: object
-    description: Request object for SuspendWorkspace.
+    description: Request object for describe cluster definition request.
     required:
-      - workspaceCrn
+      - clusterDefinitionName
     properties:
-      workspaceCrn:
+      clusterDefinitionName:
         type: string
-        description: The CRN of the workspace to suspend.
-  SuspendWorkspaceResponse:
-    type: object
-    description: Response object for SuspendWorkspace.
-  ResumeWorkspaceRequest:
+        description: The name or CRN of the cluster definition.
+  DescribeClusterDefinitionResponse:
     type: object
-    description: Request object for ResumeWorkspace.
+    description: Response object for describe cluster definition response.
     required:
-      - workspaceCrn
+      - clusterDefinition
     properties:
-      workspaceCrn:
-        type: string
-        description: The CRN of the workspace to resume.
-  ResumeWorkspaceResponse:
+      clusterDefinition:
+        $ref: '#/definitions/ClusterDefinition'
+        description: The clusterDefinition.
+  ListClusterDefinitionsRequest:
     type: object
-    description: Response object for ResumeWorkspace.
-  BackupWorkspaceRequest:
+    description: Request object for list cluster definitions request.
+  ListClusterDefinitionsResponse:
     type: object
-    description: The request object for workspace backup.
+    description: Response object for list cluster definition response.
     required:
-      - workspaceCrn
-      - backupName
+      - clusterDefinitions
     properties:
-      workspaceCrn:
-        type: string
-        description: CRN of the workspace to backup.
-      backupName:
-        type: string
-        description: Backup name.
-      backupJobTimeoutMinutes:
-        type: integer
-        format: int32
-        description: The timeout(in minutes) to use for the execution of the backup jobs.
-      skipValidation:
-        type: boolean
-        description: Skip pre-flight validations if requested.
-  BackupWorkspaceResponse:
+      clusterDefinitions:
+        type: array
+        items:
+          $ref: '#/definitions/ClusterDefinitionSummary'
+        description: The clusterDefinitions.
+  CreateClusterTemplateRequest:
     type: object
-    description: The response object for workspace backup.
+    description: Request object for create cluster template request.
+    required:
+      - clusterTemplateName
+      - clusterTemplateContent
     properties:
-      backupCrn:
+      clusterTemplateName:
+        type: string
+        description: The name of the cluster template. This name must be unique, must have between 5 and 100 characters, and must contain only lowercase letters, numbers and hyphens. Names are case-sensitive.
+        minLength: 5
+        maxLength: 1000
+      clusterTemplateContent:
         type: string
-        description: CRN of the backup generated.
-      vaultName:
+        description: The cluster template content.
+      description:
         type: string
-        description: Name of the vault where backup related volumes are stored.
-  DeleteBackupRequest:
+        description: The description of the cluster template. The description can have a maximum of 1000 characters.
+        maxLength: 1000
+      tags:
+        type: array
+        description: Tags to be added to the cluster template.
+        items:
+          $ref: '#/definitions/DatahubResourceTagRequest'
+  CreateClusterTemplateResponse:
     type: object
-    description: The request object for DeleteBackup operation.
+    description: Response object for create cluster template request.
     required:
-      - backupCrn
+      - clusterTemplate
     properties:
-      backupCrn:
-        type: string
-        description: The CRN of the backup to be deleted.
-      skipValidation:
-        type: boolean
-        description: Skip pre-flight validations if requested.
-  DeleteBackupResponse:
+      clusterTemplate:
+        $ref: '#/definitions/ClusterTemplate'
+        description: The cluster template.
+  DeleteClusterTemplatesRequest:
     type: object
-    description: The response object for DeleteBackup operation.
+    description: Request object for delete cluster templates request.
+    required:
+      - clusterTemplateNames
     properties:
-      workflowId:
-        type: string
-        description: The ID of the delete-backup workflow.
-  WorkflowMetadata:
+      clusterTemplateNames:
+        type: array
+        items:
+          type: string
+        description: The names or CRNs of the cluster templates to be deleted.
+  DeleteClusterTemplatesResponse:
     type: object
-    description: The workflow metadata.
+    description: Response object for delete cluster templates request.
+    required:
+      - clusterTemplates
     properties:
-      resourceId:
-        type: string
-        description: The unique identifier of the resource.
-      workflowIndex:
-        type: integer
-        format: int64
-        description: The workflow index. Monotonically increases for each subsequent workflow for a resource.
-      workflowType:
-        type: string
-        description: The workflow type.
-      workflowId:
-        type: string
-        description: The workflow identifier.
-      lastKnownStatus:
-        type: string
-        description: The last known status of the workflow.
-  RequestWorkflowCancellationRequest:
+      clusterTemplates:
+        type: array
+        items:
+          $ref: '#/definitions/ClusterTemplate'
+        description: The cluster templates.
+  DescribeClusterTemplateRequest:
     type: object
-    description: Request object for RequestWorkflowCancellation.
+    description: Request object for describe cluster template request.
+    required:
+      - clusterTemplateName
     properties:
-      resourceId:
+      clusterTemplateName:
         type: string
-        description: The unique identifier of the resource.
-      workflowType:
-        type: string
-        description: The workflow type.
-  RequestWorkflowCancellationResponse:
+        description: The name or CRN of the cluster template.
+  DescribeClusterTemplateResponse:
+    type: object
+    description: Response object for describe cluster template request.
+    required:
+      - clusterTemplate
+    properties:
+      clusterTemplate:
+        $ref: '#/definitions/ClusterTemplate'
+        description: The cluster template.
+  ListClusterTemplatesRequest:
+    type: object
+    description: Request object for list cluster templates request.
+  ListClusterTemplatesResponse:
     type: object
-    description: Response object for RequestWorkflowCancellation.
+    description: Response object for list cluster templates request.
+    required:
+      - clusterTemplates
     properties:
-      workflowMetadata:
+      clusterTemplates:
         type: array
         items:
-          $ref: '#/definitions/WorkflowMetadata'
-        description: The list of workflow metedata for cancelled workflows.
-x-audit: true
+          $ref: '#/definitions/ClusterTemplateSummary'
+        description: The cluster templates.
+  DatahubResourceTagRequest:
+    type: object
+    description: Tag for a datahub resource.
+    required:
+      - key
+      - value
+    properties:
+      key:
+        type: string
+        description: The key of tag.
+      value:
+        type: string
+        description: The value of the tag.
+  DatahubResourceTag:
+    type: object
+    description: Tag for a datahub resource.
+    required:
+      - key
+      - value
+    properties:
+      key:
+        type: string
+        description: The key of tag.
+      value:
+        type: string
+        description: The value of the tag.
```

### Comparing `cdpcli-0.9.89/cdpcli/doc/docstringparser.py` & `cdpcli-0.9.9/cdpcli/doc/docstringparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.89/cdpcli/doc/restdoc.py` & `cdpcli-0.9.9/cdpcli/doc/restdoc.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.89/cdpcli/doc/style.py` & `cdpcli-0.9.9/cdpcli/doc/style.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,19 +117,14 @@
             self.end_bold()
 
     def ref(self, title, link=None):
         if link is None:
             link = title
         self.doc.write(':doc:`%s <%s>`' % (title, link))
 
-    def simple_field(self, field_name, field_value):
-        self.new_paragraph()
-        self.doc.write(':%s: %s' % (field_name, field_value))
-        self.new_paragraph()
-
     def _heading(self, s, border_char):
         border = border_char * len(s)
         self.new_paragraph()
         self.doc.write('%s\n%s\n%s' % (border, s, border))
         self.new_paragraph()
 
     def h1(self, s):
```

### Comparing `cdpcli-0.9.89/cdpcli/docs.py` & `cdpcli-0.9.9/cdpcli/docs.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,79 +16,65 @@
 
 import os
 
 from cdpcli import LIST_TYPE
 from cdpcli import MAP_TYPE
 from cdpcli import OBJECT_TYPE
 from cdpcli import SCALAR_TYPES
-from cdpcli import VERSION
 from cdpcli import xform_name
 from cdpcli.argprocess import ParamShorthandDocGen
 from cdpcli.extensions.paginate import add_paging_description
 from cdpcli.model import StringShape
 
 
-MANUAL_SECTION = '1'
-MANUAL_GROUP = 'CDP CLI'
-
-
-def _is_hidden(item):
-    if getattr(item, '_UNDOCUMENTED', False):
-        return True
-    if getattr(item, 'is_deprecated', False):
+def _is_argument_hidden(argument):
+    if getattr(argument, '_UNDOCUMENTED', False):
         return True
     return False
 
 
 def generate_doc(generator, help_command):
     generator.doc_title(help_command)
-    generator.doc_docinfo(help_command)
     generator.doc_description(help_command)
     generator.doc_synopsis_start(help_command)
     if help_command.arg_table:
         for arg_name in help_command.arg_table:
             generator.doc_synopsis_option(arg_name, help_command)
     generator.doc_synopsis_end(help_command)
     generator.doc_options_start(help_command)
     if help_command.arg_table:
         for arg_name in help_command.arg_table:
-            if not generator.show_hidden and \
-               _is_hidden(help_command.arg_table[arg_name]):
+            if _is_argument_hidden(help_command.arg_table[arg_name]):
                 continue
-            generator.doc_option_start(arg_name, help_command)
             generator.doc_option(arg_name, help_command)
             generator.doc_option_example(arg_name, help_command)
-            generator.doc_option_form_factors(arg_name, help_command)
-            generator.doc_option_end(arg_name, help_command)
     generator.doc_options_end(help_command)
     generator.doc_subitems_start(help_command)
     if help_command.command_table:
         for command_name in sorted(help_command.command_table.keys()):
-            if not generator.show_hidden and \
-               _is_hidden(help_command.command_table[command_name]):
+            if hasattr(help_command.command_table[command_name],
+                       '_UNDOCUMENTED'):
                 continue
             generator.doc_subitem(command_name, help_command)
     generator.doc_subitems_end(help_command)
     generator.doc_examples(help_command)
     generator.doc_output(help_command)
-    generator.doc_form_factors(help_command)
     generator.doc_relateditems_start(help_command)
     if help_command.related_items:
         for related_item in sorted(help_command.related_items):
             generator.doc_relateditem(help_command, related_item)
 
 
 class CLIDocumentGenerator(object):
 
-    def __init__(self, help_command, show_hidden=False):
+    def __init__(self, help_command):
         self.help_command = help_command
         self.help_command.doc.translation_map = self.build_translation_map()
         self._arg_groups = self._build_arg_table_groups(help_command)
         self._documented_arg_groups = []
-        self.show_hidden = show_hidden
 
     def _build_arg_table_groups(self, help_command):
         arg_groups = {}
         for name, arg in help_command.arg_table.items():
             if arg.group_name is not None:
                 arg_groups.setdefault(arg.group_name, []).append(arg)
         return arg_groups
@@ -103,17 +89,14 @@
         doc.style.new_paragraph()
         reference = help_command.command_lineage.replace('.', ' ')
         if reference != 'cdp':
             reference = 'cdp ' + reference
         doc.writeln('.. _cli:%s:' % reference)
         doc.style.h1(help_command.name)
 
-    def doc_docinfo(self, help_command):
-        pass
-
     def doc_description(self, help_command):
         doc = help_command.doc
         doc.style.h2('Description')
         doc.include_doc_string(help_command.description)
         doc.style.new_paragraph()
 
     def doc_synopsis_start(self, help_command):
@@ -122,26 +105,24 @@
         doc.style.h2('Synopsis')
         doc.style.start_codeblock()
         doc.writeln('%s' % help_command.name)
 
     def doc_synopsis_option(self, arg_name, help_command):
         doc = help_command.doc
         argument = help_command.arg_table[arg_name]
-        if not self.show_hidden and _is_hidden(argument):
+        if _is_argument_hidden(argument):
             return
         if argument.group_name in self._arg_groups:
             if argument.group_name in self._documented_arg_groups:
                 # This arg is already documented so we can move on.
                 return
             option_str = ' | '.join(
                 [a.cli_name for a in
                  self._arg_groups[argument.group_name]])
             self._documented_arg_groups.append(argument.group_name)
-        elif argument.cli_type_name == 'blob':
-            option_str = '%s <blob>' % argument.cli_name
         else:
             option_str = '%s <value>' % argument.cli_name
         if not argument.required:
             option_str = '[%s]' % option_str
         doc.writeln('%s' % option_str)
 
     def doc_synopsis_end(self, help_command):
@@ -149,63 +130,90 @@
         doc.style.end_codeblock()
         # Reset the documented arg groups for other sections
         # that may document args (the detailed docs following
         # the synopsis).
         self._documented_arg_groups = []
 
     def doc_options_start(self, help_command):
-        pass
+        doc = help_command.doc
+        doc.style.h2('Options')
+        if not help_command.arg_table:
+            doc.write('*None*\n')
 
-    def doc_option_start(self, arg_name, help_command):
+    def doc_options_end(self, help_command):
         pass
 
     def doc_option(self, arg_name, help_command):
-        pass
+        doc = help_command.doc
+        argument = help_command.arg_table[arg_name]
+        if _is_argument_hidden(argument):
+            return
+        if argument.group_name in self._arg_groups:
+            if argument.group_name in self._documented_arg_groups:
+                # This arg is already documented so we can move on.
+                return
+            name = ' | '.join(
+                ['``%s``' % a.cli_name for a in
+                 self._arg_groups[argument.group_name]])
+            self._documented_arg_groups.append(argument.group_name)
+        else:
+            name = '``%s``' % argument.cli_name
+        doc.write('%s (%s)\n' % (name, argument.cli_type_name))
+        doc.style.indent()
+        doc.include_doc_string(argument.documentation)
+        self._document_enums(argument, doc)
+        doc.style.dedent()
+        doc.style.new_paragraph()
 
     def doc_option_example(self, arg_name, help_command):
         pass
 
-    def doc_option_form_factors(self, arg_name, help_command):
-        pass
-
-    def doc_option_end(self, arg_name, help_command):
-        pass
-
-    def doc_options_end(self, help_command):
-        pass
-
     def doc_relateditems_start(self, help_command):
         if help_command.related_items:
             doc = help_command.doc
             doc.style.h2('See Also')
 
     def doc_relateditem(self, help_command, related_item):
         doc = help_command.doc
         doc.write('* ')
         doc.style.sphinx_reference_label(
             label='cli:%s' % related_item,
             text=related_item
         )
         doc.write('\n')
 
+    def _document_enums(self, argument, doc):
+        if hasattr(argument, 'argument_model'):
+            model = argument.argument_model
+            if isinstance(model, StringShape):
+                if model.enum:
+                    self._write_possible_values(doc, model.enum)
+                if model.supported_options:
+                    self._write_possible_values(doc, model.supported_options)
+
+    def _write_possible_values(self, doc, possible_values):
+        doc.style.new_paragraph()
+        doc.write('Possible values:')
+        doc.style.start_ul()
+        for value in possible_values:
+            doc.style.li('``%s``' % value)
+        doc.style.end_ul()
+
     def doc_subitems_start(self, help_command):
         pass
 
     def doc_subitems_end(self, help_command):
         pass
 
     def doc_examples(self, help_command):
         pass
 
     def doc_output(self, help_command):
         pass
 
-    def doc_form_factors(self, help_command):
-        pass
-
 
 class ProviderDocumentGenerator(CLIDocumentGenerator):
 
     def doc_synopsis_start(self, help_command):
         doc = help_command.doc
         doc.style.h2('Synopsis')
         doc.style.codeblock(help_command.synopsis)
@@ -218,52 +226,35 @@
         doc = help_command.doc
         doc.style.new_paragraph()
 
     def doc_options_start(self, help_command):
         doc = help_command.doc
         doc.style.h2('Options')
 
-    def doc_option_start(self, arg_name, help_command):
-        pass
-
     def doc_option(self, arg_name, help_command):
         doc = help_command.doc
         argument = help_command.arg_table[arg_name]
         doc.writeln('``%s`` (%s)' % (argument.cli_name,
                                      argument.cli_type_name))
         doc.include_doc_string(argument.documentation)
         if argument.choices:
             doc.style.start_ul()
             for choice in argument.choices:
                 doc.style.li(choice)
             doc.style.end_ul()
 
-    def doc_option_example(self, arg_name, help_command):
-        pass
-
-    def doc_option_form_factors(self, arg_name, help_command):
-        pass
-
-    def doc_option_end(self, arg_name, help_command):
-        pass
-
-    def doc_options_end(self, help_command):
-        pass
-
     def doc_subitems_start(self, help_command):
         doc = help_command.doc
-        doc.style.h2('Available Commands')
+        doc.style.h2('Available Services')
         doc.style.toctree()
 
     def doc_subitem(self, command_name, help_command):
         doc = help_command.doc
-        command = help_command.command_table[command_name]
-        is_deprecated = ' (deprecated)' if _is_hidden(command) else ''
         file_name = '%s/index' % command_name
-        doc.style.tocitem(command_name + is_deprecated, file_name=file_name)
+        doc.style.tocitem(command_name, file_name=file_name)
 
 
 class ServiceDocumentGenerator(CLIDocumentGenerator):
 
     def build_translation_map(self):
         d = {}
         service_model = self.help_command.obj
@@ -281,70 +272,47 @@
     def doc_synopsis_end(self, help_command):
         pass
 
     # A service document has no option section.
     def doc_options_start(self, help_command):
         pass
 
-    def doc_option_start(self, arg_name, help_command):
-        pass
-
     def doc_option(self, arg_name, help_command):
         pass
 
     def doc_option_example(self, arg_name, help_command):
         pass
 
-    def doc_option_form_factors(self, arg_name, help_command):
-        pass
-
-    def doc_option_end(self, arg_name, help_command):
-        pass
-
     def doc_options_end(self, help_command):
         pass
 
-    def doc_docinfo(self, help_command):
-        doc = help_command.doc
-        service_model = help_command.obj
-        doc.style.simple_field('subtitle', service_model.service_title)
-        service_version = service_model.service_version
-        # Goes away once each service has its own version number
-        if service_version == '__API_VERSION__':
-            service_version = VERSION
-        doc.style.simple_field('version', service_version)
-        if help_command.include_man_fields:
-            doc.style.simple_field('manual_section', MANUAL_SECTION)
-            doc.style.simple_field('manual_group', MANUAL_GROUP)
-
     def doc_description(self, help_command):
         doc = help_command.doc
         service_model = help_command.obj
         doc.style.h2('Description')
         # TODO: need a documentation attribute.
         doc.include_doc_string(service_model.documentation)
 
     def doc_subitems_start(self, help_command):
         doc = help_command.doc
-        doc.style.h2('Available Subcommands')
+        doc.style.h2('Available Commands')
         doc.style.toctree()
 
     def doc_subitem(self, command_name, help_command):
         doc = help_command.doc
         subcommand = help_command.command_table[command_name]
-        is_deprecated = ' (deprecated)' if _is_hidden(subcommand) else ''
         subcommand_table = getattr(subcommand, 'subcommand_table', {})
         # If the subcommand table has commands in it,
         # direct the subitem to the command's index because
         # it has more subcommands to be documented.
         if (len(subcommand_table) > 0):
             file_name = '%s/index' % command_name
-            doc.style.tocitem(command_name + is_deprecated, file_name=file_name)
+            doc.style.tocitem(command_name, file_name=file_name)
         else:
-            doc.style.tocitem(command_name + is_deprecated)
+            doc.style.tocitem(command_name)
 
 
 class OperationDocumentGenerator(CLIDocumentGenerator):
 
     def build_translation_map(self):
         operation_model = self.help_command.obj
         d = {}
@@ -366,48 +334,27 @@
                         d[argument_name] = cli_name
                 else:
                     d[argument_name] = cli_name
         for operation_name in operation_model.service_model.operation_names:
             d[operation_name] = xform_name(operation_name, '-')
         return d
 
-    def doc_docinfo(self, help_command):
-        doc = help_command.doc
-        operation_model = help_command.obj
-        # Internal commands like "configure" may lack these (see BasicDocHandler)
-        if hasattr(operation_model, 'summary'):
-            doc.style.simple_field('subtitle', operation_model.summary)
-        if hasattr(operation_model, 'service_model') and\
-                hasattr(operation_model.service_model, 'service_version'):
-            service_version = operation_model.service_model.service_version
-            # Goes away once each service has its own version number
-            if service_version == '__API_VERSION__':
-                service_version = VERSION
-            doc.style.simple_field('version', service_version)
-        if help_command.include_man_fields:
-            doc.style.simple_field('manual_section', MANUAL_SECTION)
-            doc.style.simple_field('manual_group', MANUAL_GROUP)
-
     def doc_description(self, help_command):
         doc = help_command.doc
         operation_model = help_command.obj
         doc.style.h2('Description')
         doc.include_doc_string(operation_model.documentation)
         add_paging_description(help_command)
 
     def _json_example_value_name(self, argument_model, include_enum_values=True):
         # If include_enum_values is True, then the valid enum values
         # are included as the sample JSON value.
         if isinstance(argument_model, StringShape):
             if argument_model.enum and include_enum_values:
                 choices = argument_model.enum
-                if not self.show_hidden and argument_model.deprecated_enum_values:
-                    choices = [item
-                               for item in choices
-                               if item not in argument_model.deprecated_enum_values]
                 return '|'.join(['"%s"' % c for c in choices])
             elif argument_model.supported_options and include_enum_values:
                 choices = argument_model.supported_options
                 return '|'.join(['"%s"' % c for c in choices])
             else:
                 return '"string"'
         elif argument_model.type_name == 'boolean':
@@ -499,57 +446,18 @@
                 if need_comma:
                     doc.write(',')
                     doc.style.new_line()
                 doc.write('"%s": ' % member_name)
                 self._json_example(doc, member_model, stack)
                 need_comma = True
 
-    def doc_options_start(self, help_command):
-        doc = help_command.doc
-        doc.style.h2('Options')
-        if not help_command.arg_table:
-            doc.write('*None*\n')
-
-    def doc_option_start(self, arg_name, help_command):
-        pass
-
-    def doc_option(self, arg_name, help_command):
-        doc = help_command.doc
-        argument = help_command.arg_table[arg_name]
-        is_deprecated = ''
-        if _is_hidden(argument):
-            if not self.show_hidden:
-                return
-            else:
-                is_deprecated = ' (deprecated)'
-        if argument.group_name in self._arg_groups:
-            if argument.group_name in self._documented_arg_groups:
-                # This arg is already documented so we can move on.
-                return
-            name = ' | '.join(
-                ['``%s``' % a.cli_name for a in
-                 self._arg_groups[argument.group_name]])
-        else:
-            name = '``%s``' % argument.cli_name
-        doc.write('%s (%s)%s\n' % (name, argument.cli_type_name, is_deprecated))
-        doc.style.indent()
-        doc.style.new_paragraph()
-        doc.include_doc_string(argument.documentation)
-        self._document_enums(argument, doc)
-        if hasattr(argument.argument_model, 'members'):
-            doc.style.new_paragraph()
-            for member_name, member_shape in argument.argument_model.members.items():
-                self.doc_member(doc, member_name, member_shape, stack=[])
-        doc.style.dedent()
-        doc.style.new_paragraph()
-
     def doc_option_example(self, arg_name, help_command):
         doc = help_command.doc
         cli_argument = help_command.arg_table[arg_name]
-        if not self.show_hidden and _is_hidden(cli_argument):
+        if _is_argument_hidden(cli_argument):
             return
         if cli_argument.group_name in self._arg_groups:
             if cli_argument.group_name in self._documented_arg_groups:
                 # Args with group_names (boolean args) don't
                 # need to generate example syntax.
                 return
         argument_model = cli_argument.argument_model
@@ -583,154 +491,85 @@
             doc.write('Syntax')
             doc.style.start_codeblock()
             example_type = self._json_example_value_name(
                 member, include_enum_values=False)
             doc.write('%s %s ...' % (example_type, example_type))
             if isinstance(member, StringShape):
                 if member.enum:
-                    enum_values = member.enum
-                    if not self.show_hidden and member.deprecated_enum_values:
-                        enum_values = [v for v in enum_values
-                                       if v not in member.deprecated_enum_values]
-                    self._write_possible_values(doc, enum_values)
+                    self._write_possible_values(doc, member.enum)
                 if member.supported_options:
                     self._write_possible_values(doc, member.supported_options)
             doc.style.end_codeblock()
             doc.style.new_paragraph()
         elif cli_argument.cli_type_name not in SCALAR_TYPES:
             doc.style.new_paragraph()
             doc.write('JSON Syntax')
             doc.style.start_codeblock()
             self._json_example(doc, argument_model, stack=[])
             doc.style.end_codeblock()
             doc.style.new_paragraph()
 
-    def doc_option_form_factors(self, arg_name, help_command):
-        doc = help_command.doc
-        argument = help_command.arg_table[arg_name]
-        if not self.show_hidden and _is_hidden(argument):
-            return
-        if argument.group_name in self._arg_groups:
-            if argument.group_name in self._documented_arg_groups:
-                # This arg is already documented so we can move on.
-                return
-        if argument.argument_model.form_factors is not None:
-            self._write_form_factors(doc, argument.argument_model.form_factors)
-
-    def doc_option_end(self, arg_name, help_command):
-        argument = help_command.arg_table[arg_name]
-        if argument.group_name in self._arg_groups:
-            if argument.group_name in self._documented_arg_groups:
-                # This arg is already documented so we can move on.
-                return
-            self._documented_arg_groups.append(argument.group_name)
-
-    def doc_options_end(self, help_command):
-        pass
+    def _write_possible_values(self, doc, possible_values):
+        doc.style.new_paragraph()
+        doc.write("Possible values:\n")
+        for value in possible_values:
+            doc.write("    %s\n" % value)
+        doc.write("\n")
 
     def doc_output(self, help_command):
         doc = help_command.doc
         doc.style.h2('Output')
         operation_model = help_command.obj
         output_shape = operation_model.output_shape
         if output_shape is None:
             doc.write('None')
         else:
             for member_name, member_shape in output_shape.members.items():
-                self.doc_member(doc, member_name, member_shape, stack=[])
-
-    def doc_examples(self, help_command):
-        operation = help_command.command_lineage.replace('.', os.path.sep)
-        doc_path = os.path.dirname(os.path.abspath(__file__))
-        doc_path = os.path.join(doc_path, 'examples')
-        doc_path = os.path.join(doc_path, operation) + '.rst'
-        if os.path.isfile(doc_path):
-            help_command.doc.style.h2('Examples')
-            fp = open(doc_path)
-            for line in fp.readlines():
-                help_command.doc.write(line)
-
-    def doc_form_factors(self, help_command):
-        operation_model = help_command.obj
-        form_factors = getattr(operation_model, 'form_factors', None)
-        if not form_factors:
-            service_model = getattr(operation_model, 'service_model', None)
-            if service_model:
-                form_factors = getattr(service_model, 'form_factors', None)
-        if form_factors:
-            doc = help_command.doc
-            doc.style.h2('Form Factors')
-            doc.write(', '.join(form_factors))
-            doc.style.new_paragraph()
+                self._doc_member_for_output(doc, member_name, member_shape, stack=[])
 
-    def doc_member(self, doc, member_name, member_shape, stack):
+    def _doc_member_for_output(self, doc, member_name, member_shape, stack):
         if member_shape.name in stack:
             # Document the recursion once, otherwise just
             # note the fact that it's recursive and return.
             if stack.count(member_shape.name) > 1:
                 if member_shape.type_name == OBJECT_TYPE:
                     doc.write('( ... recursive ... )')
                 return
         stack.append(member_shape.name)
         try:
-            self._do_doc_member(doc, member_name,
-                                member_shape, stack)
+            self._do_doc_member_for_output(doc, member_name,
+                                           member_shape, stack)
         finally:
             stack.pop()
 
-    def _do_doc_member(self, doc, member_name, member_shape, stack):
-        is_deprecated = ''
-        if _is_hidden(member_shape):
-            if not self.show_hidden:
-                return
-            else:
-                is_deprecated = ' (deprecated)'
+    def _do_doc_member_for_output(self, doc, member_name, member_shape, stack):
         docs = member_shape.documentation
         if member_name:
-            doc.write('%s -> (%s)%s' %
-                      (member_name, member_shape.type_name, is_deprecated))
+            doc.write('%s -> (%s)' % (member_name, member_shape.type_name))
         else:
-            doc.write('(%s)%s' % member_shape.type_name, is_deprecated)
+            doc.write('(%s)' % member_shape.type_name)
         doc.style.indent()
         doc.style.new_paragraph()
         doc.include_doc_string(docs)
-        if member_shape.form_factors is not None:
-            self._write_form_factors(doc, member_shape.form_factors)
         doc.style.new_paragraph()
         member_type_name = member_shape.type_name
         if member_type_name == OBJECT_TYPE:
             for sub_name, sub_shape in member_shape.members.items():
-                self.doc_member(doc, sub_name, sub_shape, stack)
+                self._doc_member_for_output(doc, sub_name, sub_shape, stack)
         elif member_type_name == LIST_TYPE:
-            self.doc_member(doc, 'item', member_shape.member, stack)
+            self._doc_member_for_output(doc, '', member_shape.member, stack)
         elif member_type_name == MAP_TYPE:
-            self.doc_member(doc, 'key', member_shape.key, stack)
-            self.doc_member(doc, 'value', member_shape.value, stack)
+            self._doc_member_for_output(doc, 'key', member_shape.key, stack)
+            self._doc_member_for_output(doc, 'value', member_shape.value, stack)
         doc.style.dedent()
         doc.style.new_paragraph()
 
-    def _document_enums(self, argument, doc):
-        if hasattr(argument, 'argument_model'):
-            model = argument.argument_model
-            if isinstance(model, StringShape):
-                if model.enum:
-                    enum_values = model.enum
-                    if not self.show_hidden and model.deprecated_enum_values:
-                        enum_values = [v for v in enum_values
-                                       if v not in model.deprecated_enum_values]
-                    self._write_possible_values(doc, enum_values)
-                if model.supported_options:
-                    self._write_possible_values(doc, model.supported_options)
-
-    def _write_possible_values(self, doc, possible_values):
-        doc.style.new_paragraph()
-        doc.write('Possible values:')
-        doc.style.start_ul()
-        for value in possible_values:
-            doc.style.li('``%s``' % value)
-        doc.style.end_ul()
-
-    def _write_form_factors(self, doc, form_factors):
-        doc.style.new_paragraph()
-        doc.write('Form Factors: ')
-        doc.write(', '.join(form_factors))
-        doc.style.new_paragraph()
+    def doc_examples(self, help_command):
+        operation = help_command.command_lineage.replace('.', os.path.sep)
+        doc_path = os.path.dirname(os.path.abspath(__file__))
+        doc_path = os.path.join(doc_path, 'examples')
+        doc_path = os.path.join(doc_path, operation) + '.rst'
+        if os.path.isfile(doc_path):
+            help_command.doc.style.h2('Examples')
+            fp = open(doc_path)
+            for line in fp.readlines():
+                help_command.doc.write(line)
```

### Comparing `cdpcli-0.9.89/cdpcli/examples/configure/get/_description.rst` & `cdpcli-0.9.9/cdpcli/examples/configure/get/_description.rst`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 An unqualified configuration name refers to a name that is not scoped to a
 specific section in the configuration file.  Sections are specified by
 separating parts with the ``"."`` character (``section.config-name``).  An
 unqualified name will be scoped to the current profile.  For example,
 ``cdp configure get cdp_access_key_id`` will retrieve the ``cdp_access_key_id``
 from the current profile,  or the ``default`` profile if no profile is
 specified.  You can still provide a ``--profile`` argument to the ``cdp
-configure get`` command.  For example, ``cdp configure get cdp_region --profile
+configure get`` command.  For example, ``cdp configure get region --profile
 testing`` will print the region value for the ``testing`` profile.
 
 
 Qualified Names
 ---------------
 
 A qualified name is a name that has at least one ``"."`` character in the name.
```

### Comparing `cdpcli-0.9.89/cdpcli/examples/configure/get/_examples.rst` & `cdpcli-0.9.9/cdpcli/examples/configure/get/_examples.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.89/cdpcli/examples/configure/set/_description.rst` & `cdpcli-0.9.9/cdpcli/examples/configure/set/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.89/cdpcli/examples/configure/set/_examples.rst` & `cdpcli-0.9.9/cdpcli/examples/configure/set/_examples.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.89/cdpcli/exceptions.py` & `cdpcli-0.9.9/cdpcli/exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -70,25 +70,17 @@
         msg = self.MSG_TEMPLATE.format(
             error_code=error_response['error'].get('code', 'Unknown'),
             error_message=error_response['error'].get('message', 'Unknown'),
             operation_name=operation_name,
             service_name=service_name,
             http_status_code=http_status_code,
             request_id=request_id)
-        msg = self.cleanup_error_msg(msg)
         super(ClientError, self).__init__(msg)
-        self.http_status_code = http_status_code
         self.response = error_response
 
-    def cleanup_error_msg(self, msg):
-        msg = msg.replace('&quot;', '"').replace("&#39;", "'")\
-            .replace("/&lt;", "<").replace("&gt;", ">")
-
-        return msg
-
 
 class UnseekableStreamError(CdpCLIError):
     """
     Need to seek a stream, but stream does not support seeking.
     """
     fmt = ('Need to rewind the stream {stream_object}, but stream '
            'is not seekable.')
@@ -125,15 +117,15 @@
     fmt = 'Signature version is not supported: {signature_version}'
 
 
 class NoCredentialsError(CdpCLIError):
     """
     No credentials could be found.
     """
-    fmt = 'Unable to locate CDP credentials: {err_msg}.'
+    fmt = 'Unable to locate CDP credentials'
 
 
 class UnknownCredentialError(CdpCLIError):
     """
     Tried to insert before/after an unregistered credential type.
     """
     fmt = 'Credential named {name} not found.'
@@ -190,22 +182,14 @@
 class ConfigParseError(CdpCLIError):
     """
     The configuration file could not be parsed.
     """
     fmt = 'Unable to parse config file: {path}'
 
 
-class InvalidConfiguredFormFactor(CdpCLIError):
-    """
-    The configured form factor is not a valid value.
-    """
-    fmt = ('The configured form factor {form_factor} is invalid. '
-           'Valid values are: {valid_form_factors}')
-
-
 class ClusterTerminatingError(CdpCLIError):
 
     """
     The cluster is terminating or has already terminated.
     """
     fmt = 'Cluster {cluster_name} is terminating.'
 
@@ -252,92 +236,7 @@
 
 class WrongPuttyKeyError(CdpCLIError):
 
     """
     A wrong key has been used with a compatible program.
     """
     fmt = 'Key file file format is incorrect. Putty expects a ppk file.'
-
-
-class MissingArgumentError(CdpCLIError):
-
-    """
-    The following argument is required.
-    """
-    fmt = 'The following argument is required: {arg_name}.'
-
-
-class InteractiveLoginError(CdpCLIError):
-
-    """
-    Login failed.
-    """
-    fmt = 'Login failed: {err_msg}.'
-
-
-class WrongSvcFormFactorError(CdpCLIError):
-
-    """
-    The service does not work under the current form factor.
-    """
-    fmt = ('The command {service_name} is not available under the {form_factor}'
-           ' CDP form factor. It is only available for these form factors: '
-           '{service_form_factors}. Check that your profile configuration '
-           'specifies the correct form factor, or that the endpoint URL in '
-           'profile configuration or on the command line points to the correct '
-           'control plane.')
-
-
-class WrongOpFormFactorError(CdpCLIError):
-
-    """
-    The operation does not work under the current form factor.
-    """
-    fmt = ('The subcommand {operation_name} under the command {service_name} is '
-           'not available under the {form_factor} CDP form factor. It is only '
-           'available for these form factors: {operation_form_factors}. Check '
-           'that your profile configuration or explicit endpoint URL points to '
-           'the correct control plane.')
-
-
-class WrongArgFormFactorError(CdpCLIError):
-
-    """
-    The argument does not work under the current form factor.
-    """
-    fmt = ('The argument {arg_name} is not available under the {form_factor} '
-           'CDP form factor. It is only available for these form factors: '
-           '{arg_form_factors}. Check that your profile configuration '
-           'or explicit endpoint URL points to the correct control plane.')
-
-
-class ExtensionImportError(CdpCLIError):
-
-    """
-    Failed to import CLI extension.
-    """
-    fmt = 'Failed to import CLI extension \'{ext_name}\': {err}.'
-
-
-class WorkloadServiceDiscoveryError(CdpCLIError):
-
-    """
-    The workload service-discovery failed.
-    """
-    fmt = 'Workload service-discovery error: {err_msg}.'
-
-
-class RedirectExtensionError(CdpCLIError):
-
-    """
-    The redirect extension failed.
-    """
-    fmt = 'The redirect extension failed: {err_msg}.'
-
-
-class DfExtensionError(CdpCLIError):
-
-    """
-    The DF extension failed.
-    """
-    fmt = ('The DF extension failed: {err_msg} '
-           'Service name: {service_name}, operation name: {operation_name}')
```

### Comparing `cdpcli-0.9.89/cdpcli/extensions/__init__.py` & `cdpcli-0.9.9/cdpcli/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.89/cdpcli/extensions/arguments.py` & `cdpcli-0.9.9/cdpcli/extensions/arguments.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,16 +47,16 @@
         # Set all ``Argument`` objects in ``argument_table`` to not required
         # if this argument's name is present in the command line.
         if name_in_cmdline in args:
             for arg_name in argument_table.keys():
                 argument_table[arg_name].required = False
 
     def invoke(self,
-               client_creator,
-               operation_model,
+               client,
+               operation_name,
                parameters,
                parsed_args,
                parsed_globals):
         """
         Invokes the argument handler. Returns 'True' if other operation call
         handlers should be invoked after it, 'False' to indicate that no other
         invocations should be made.
```

### Comparing `cdpcli-0.9.89/cdpcli/extensions/cliinputjson.py` & `cdpcli-0.9.9/cdpcli/extensions/cliinputjson.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,42 +43,42 @@
     }
 
     def __init__(self, operation_model):
         super(CliInputJSONArgument, self).__init__()
         self._operation_model = operation_model
 
     def invoke(self,
-               client_creator,
-               operation_model,
+               client,
+               operation_name,
                parameters,
                parsed_args,
                parsed_globals):
-        return self.add_to_call_parameters(parameters, parsed_args, parsed_globals)
+        return self.add_to_call_parameters(parameters, parsed_args)
 
-    def add_to_call_parameters(self, call_parameters, parsed_args, parsed_globals):
+    def add_to_call_parameters(self, call_parameters, parsed_args):
 
         # Check if ``--cli-input-json`` was specified in the command line.
         input_json = getattr(parsed_args, 'cli_input_json', None)
         if input_json is not None:
             # Retrieve the JSON from the file if needed.
-            retrieved_json = get_paramfile(input_json, parsed_globals)
+            retrieved_json = get_paramfile(input_json)
             # Nothing was retrieved from the file. So assume the argument
             # is already a JSON string.
             if retrieved_json is None:
                 retrieved_json = input_json
             try:
                 # Try to load the JSON string into a python dictionary
                 input_data = json.loads(retrieved_json)
             except ValueError as e:
                 raise ParamError(
                     self.name, "Invalid JSON: %s\nJSON received: %s"
                                % (e, retrieved_json))
             # We run the ParamFileVisitor over the input data to resolve any
             # paramfile references in it.
-            input_data = ParamFileVisitor(parsed_globals).visit(
+            input_data = ParamFileVisitor().visit(
                 input_data, self._operation_model.input_shape)
             # Add the members from the input JSON to the call parameters.
             self._update_call_parameters(call_parameters, input_data)
         return True
 
     def _update_call_parameters(self, call_parameters, input_data):
         for input_key in input_data.keys():
```

### Comparing `cdpcli-0.9.89/cdpcli/extensions/commands.py` & `cdpcli-0.9.9/cdpcli/extensions/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,29 +139,29 @@
     def __call__(self, client_creator, args, parsed_globals):
         # args is the remaining unparsed args.
         # We might be able to parse these args so we need to create
         # an arg parser and parse them.
         self._subcommand_table = self._build_subcommand_table()
         self._arg_table = self._build_arg_table()
         self._handle_override_required_args(args)
-        parser = ArgTableArgParser(self.arg_table, command_table=self.subcommand_table)
+        parser = ArgTableArgParser(self.arg_table, self.subcommand_table)
         parsed_args, remaining = parser.parse_known_args(args)
 
         # Unpack arguments
         for key, value in vars(parsed_args).items():
             cli_argument = None
 
             # Convert the name to use dashes instead of underscore
             # as these are how the parameters are stored in the
             # `arg_table`.
             xformed = key.replace('_', '-')
             if xformed in self.arg_table:
                 cli_argument = self.arg_table[xformed]
 
-            value = unpack_argument(cli_argument, value, parsed_globals)
+            value = unpack_argument(cli_argument, value)
 
             # If this parameter has a schema defined, then allow plugins
             # a chance to process and override its value.
             if self._should_allow_override(cli_argument, value):
                 # Unpack the argument, which is a string, into the
                 # correct Python type (dict, list, etc)
                 value = unpack_cli_arg(cli_argument, value)
@@ -297,16 +297,16 @@
     @lineage.setter
     def lineage(self, value):
         self._lineage = value
 
 
 class BasicDocHandler(OperationDocumentGenerator):
 
-    def __init__(self, help_command, show_hidden=False):
-        super(BasicDocHandler, self).__init__(help_command, show_hidden=show_hidden)
+    def __init__(self, help_command):
+        super(BasicDocHandler, self).__init__(help_command)
         self.doc = help_command.doc
 
     def build_translation_map(self):
         return {}
 
     def doc_description(self, help_command, **kwargs):
         self.doc.style.h2('Description')
@@ -439,10 +439,9 @@
         else:
             return value
 
     def __call__(self, client_creator, args, parsed_globals):
         # Now generate all of the events for a Provider document.
         # We pass ourselves along so that we can, in turn, get passed
         # to all event handlers.
-        generate_doc(self.GeneratorClass(self, show_hidden=parsed_globals.deprecated),
-                     self)
+        generate_doc(self.GeneratorClass(self), self)
         self.renderer.render(self.doc.getvalue())
```

### Comparing `cdpcli-0.9.89/cdpcli/extensions/configure/configure.py` & `cdpcli-0.9.9/cdpcli/extensions/configure/configure.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,15 @@
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 import os
 
-from cdpcli import CDP_ACCESS_KEY_ID_KEY_NAME, \
-                   CDP_ACCESS_TOKEN_KEY_NAME, \
-                   CDP_PRIVATE_KEY_KEY_NAME, \
-                   CDP_REGION_KEY_NAME
+from cdpcli import CDP_ACCESS_KEY_ID_KEY_NAME, CDP_PRIVATE_KEY_KEY_NAME
 from cdpcli.compat import compat_input
 from cdpcli.endpoint import EndpointResolver
 from cdpcli.exceptions import ProfileNotFound
 from cdpcli.extensions.commands import BasicCommand
 from cdpcli.extensions.configure import CREDENTIAL_FILE_COMMENT
 from cdpcli.extensions.configure.get import ConfigureGetCommand
 from cdpcli.extensions.configure.list import ConfigureListCommand
@@ -54,35 +51,37 @@
 
 
 class ConfigureCommand(BasicCommand):
     NAME = 'configure'
     DESCRIPTION = BasicCommand.FROM_FILE()
     SYNOPSIS = ('cdp configure [--profile profile-name]')
     EXAMPLES = (
-        'To create a new default configuration for CDP Public Cloud::\n'
+        'To create a new configuration::\n'
         '\n'
         '    $ cdp configure\n'
         '    CDP Access Key ID [None]: accesskey\n'
         '    CDP Private Key [None]: privatekey\n'
-        '    CDP Endpoint URL (blank for public cloud) [None]:\n'
+        '\n'
+        'To update just the access key id::\n'
+        '\n'
+        '    $ cdp configure\n'
+        '    CDP Access Key ID [***]:\n'
+        '    CDP Private Key [****]:\n'
     )
     SUBCOMMANDS = [
         {'name': 'list', 'command_class': ConfigureListCommand},
         {'name': 'get', 'command_class': ConfigureGetCommand},
         {'name': 'set', 'command_class': ConfigureSetCommand},
     ]
 
     # If you want to add new values to prompt, update this list here.
     VALUES_TO_PROMPT = [
-        # (config_name, prompt_text)
+        # (logical_name, config_name, prompt_text)
         (CDP_ACCESS_KEY_ID_KEY_NAME, "CDP Access Key ID"),
-        (CDP_PRIVATE_KEY_KEY_NAME, "CDP Private Key"),
-        (CDP_REGION_KEY_NAME, "CDP Region"),
-        (EndpointResolver.CDP_ENDPOINT_URL_KEY_NAME,
-         "CDP Endpoint URL (blank for public cloud)")
+        (CDP_PRIVATE_KEY_KEY_NAME, "CDP Private Key")
     ]
 
     def __init__(self, prompter=None, config_writer=None):
         super(ConfigureCommand, self).__init__()
         if prompter is None:
             prompter = InteractivePrompter()
         self._prompter = prompter
@@ -103,38 +102,43 @@
         for config_name, prompt_text in self.VALUES_TO_PROMPT:
             current_value = config.get(config_name)
             new_value = self._prompter.get_value(current_value, config_name,
                                                  prompt_text)
             if new_value is not None and new_value != current_value:
                 new_values[config_name] = new_value
 
+        if parsed_globals.endpoint_url is not None:
+            new_values[EndpointResolver.ENDPOINT_URL_KEY_NAME] = \
+                parsed_globals.endpoint_url
+
+        if parsed_globals.cdp_endpoint_url is not None:
+            new_values[EndpointResolver.CDP_ENDPOINT_URL_KEY_NAME] = \
+                parsed_globals.cdp_endpoint_url
+
         config_filename = os.path.expanduser(
             context.get_config_variable('config_file'))
         if new_values:
             self._write_out_creds_file_values(context,
                                               new_values,
                                               parsed_globals.profile)
             if parsed_globals.profile is not None:
                 new_values['__section__'] = (
                     'profile %s' % parsed_globals.profile)
             self._config_writer.update_config(new_values, config_filename)
 
     def _write_out_creds_file_values(self, context, new_values, profile_name):
-        # The access_key/private_key/access_token are now *always* written to the shared
+        # The access_key/private_key are now *always* written to the shared
         # credentials file (~/.cdp/credentials).
         credential_file_values = {}
         if CDP_ACCESS_KEY_ID_KEY_NAME in new_values:
             credential_file_values[CDP_ACCESS_KEY_ID_KEY_NAME] = new_values.pop(
                 CDP_ACCESS_KEY_ID_KEY_NAME)
         if CDP_PRIVATE_KEY_KEY_NAME in new_values:
             credential_file_values[CDP_PRIVATE_KEY_KEY_NAME] = new_values.pop(
                 CDP_PRIVATE_KEY_KEY_NAME)
-        if CDP_ACCESS_TOKEN_KEY_NAME in new_values:
-            credential_file_values[CDP_ACCESS_TOKEN_KEY_NAME] = new_values.pop(
-                CDP_ACCESS_TOKEN_KEY_NAME)
         if credential_file_values:
             if profile_name is not None:
                 credential_file_values['__section__'] = profile_name
             shared_credentials_filename = os.path.expanduser(
                 context.get_config_variable('credentials_file'))
             self._config_writer.update_config(
                 credential_file_values,
```

### Comparing `cdpcli-0.9.89/cdpcli/extensions/configure/get.py` & `cdpcli-0.9.9/cdpcli/extensions/configure/get.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.89/cdpcli/extensions/configure/list.py` & `cdpcli-0.9.9/cdpcli/extensions/configure/list.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,94 +11,72 @@
 #
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 import sys
 
-from cdpcli import CDP_ACCESS_KEY_ID_KEY_NAME,\
-    CDP_ENDPOINT_URL_KEY_NAME,\
-    CDP_PRIVATE_KEY_KEY_NAME,\
-    CDP_REGION_KEY_NAME,\
-    ENDPOINT_URL_KEY_NAME,\
-    FORM_FACTOR_KEY_NAME
+from cdpcli import CDP_ACCESS_KEY_ID_KEY_NAME, CDP_PRIVATE_KEY_KEY_NAME
 from cdpcli.extensions.commands import BasicCommand
 
 from . import ConfigValue, NOT_SET
 
 
 class ConfigureListCommand(BasicCommand):
     NAME = 'list'
     DESCRIPTION = (
-        'List CDP CLI configuration data. Each configuration item\'s name, '
-        'value, source type, and source location are listed. For example, if '
-        'you provide the CDP access key in an environment variable, this '
-        'command will list the access key value and its source as the '
-        'environment.\n'
+        'List the CDP CLI configuration data.  This command will '
+        'show you the current configuration data.  For each configuration '
+        'item, it will show you the value, where the configuration value '
+        'was retrieved, and the configuration variable name.  For example, '
+        'if you provide the CDP access key in an environment variable, this '
+        'command will show you the key information you\'ve configured, '
+        'it will tell you that this value came from an environment '
+        'variable, and it will tell you the name of the environment '
+        'variable.\n'
     )
     SYNOPSIS = 'cdp configure list [--profile profile-name]'
     EXAMPLES = (
         'To show your current configuration values::\n'
         '\n'
         '  $ cdp configure list\n'
-        '                Name                Value'
-        '              Source Type    Source\n'
-        '                ----                -----'
-        '              -----------    ------\n'
-        '             profile            <not set>'
-        '                     None    None\n'
-        '   cdp_access_key_id ****************ABCD  shared-credentials-file\n'
-        '     cdp_private_key ****************EFGH  shared-credentials-file\n'
-        '    cdp_endpoint_url            <not set>'
-        '                     None    None\n'
-        '        endpoint_url            <not set>'
-        '                     None    None\n'
-        '         form_factor            <not set>'
-        '                     None    None\n'
+        '        Name                    Value             Type    Location\n'
+        '        ----                    -----             ----    --------\n'
+        '     profile                <not set>             None    None\n'
+        '  access_key     ****************ABCD      config_file    ~/.cdp/config\n'
+        '  private_key    ****************ABCD      config_file    ~/.cdp/config\n'
         '\n'
     )
 
     def __init__(self, stream=sys.stdout):
         super(ConfigureListCommand, self).__init__()
         self._stream = stream
 
     def _run_main(self, client_creator, args, parsed_globals):
         context = client_creator.context
 
-        self._display_config_value(ConfigValue('Value', 'Source Type', 'Source'),
+        self._display_config_value(ConfigValue('Value', 'Type', 'Location'),
                                    'Name')
-        self._display_config_value(ConfigValue('-----', '-----------', '------'),
+        self._display_config_value(ConfigValue('-----', '----', '--------'),
                                    '----')
 
         if context.profile is not None:
             profile = ConfigValue(context.profile, 'manual', '--profile')
         else:
             profile = self._lookup_config(context, 'profile')
         self._display_config_value(profile, 'profile')
 
         access_key, private_key = self._lookup_credentials(context)
-        self._display_config_value(access_key, CDP_ACCESS_KEY_ID_KEY_NAME)
-        self._display_config_value(private_key, CDP_PRIVATE_KEY_KEY_NAME)
-
-        self._display_config_value(self._lookup_config(context, CDP_REGION_KEY_NAME),
-                                   CDP_REGION_KEY_NAME)
-        self._display_config_value(self._lookup_config(context,
-                                                       CDP_ENDPOINT_URL_KEY_NAME),
-                                   CDP_ENDPOINT_URL_KEY_NAME)
-        self._display_config_value(self._lookup_config(context, ENDPOINT_URL_KEY_NAME),
-                                   ENDPOINT_URL_KEY_NAME)
-        self._display_config_value(self._lookup_config(context, FORM_FACTOR_KEY_NAME),
-                                   FORM_FACTOR_KEY_NAME)
+        self._display_config_value(access_key, 'access_key')
+        self._display_config_value(private_key, 'private_key')
 
     def _display_config_value(self, config_value, config_name):
-        truncated_value = (config_value.value[:27] + '...')\
-            if len(config_value.value) > 30 else config_value.value
-        self._stream.write('%20s %30s %24s    %s\n' % (
-            config_name, truncated_value, config_value.source_type,
-            config_value.source))
+        self._stream.write('%10s %24s %16s    %s\n' % (
+            config_name, config_value.value, config_value.config_type,
+            config_value.config_variable))
 
     def _lookup_credentials(self, context):
         # First try it with _lookup_config.  It's possible
         # that we don't find credentials this way.
         access_key = self._lookup_config(context, CDP_ACCESS_KEY_ID_KEY_NAME)
         if access_key.value is not NOT_SET:
             private_key = self._lookup_config(context, CDP_PRIVATE_KEY_KEY_NAME)
```

### Comparing `cdpcli-0.9.89/cdpcli/extensions/configure/set.py` & `cdpcli-0.9.9/cdpcli/extensions/configure/set.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 import os
 
 from cdpcli import CDP_ACCESS_KEY_ID_KEY_NAME
-from cdpcli import CDP_ACCESS_TOKEN_KEY_NAME
 from cdpcli import CDP_PRIVATE_KEY_KEY_NAME
 from cdpcli import DEFAULT_PROFILE_NAME
 from cdpcli.extensions.commands import BasicCommand
 from cdpcli.extensions.writer import ConfigFileWriter
 
 from . import PREDEFINED_SECTION_NAMES
 
@@ -41,15 +40,14 @@
          'action': 'store',
          'no_paramfile': True,  # To disable the default paramfile behavior
          'cli_type_name': 'string', 'positional_arg': True},
     ]
     # Any variables specified in this list will be written to
     # the ~/.cdp/credentials file instead of ~/.cdp/config.
     _WRITE_TO_CREDS_FILE = [CDP_ACCESS_KEY_ID_KEY_NAME,
-                            CDP_ACCESS_TOKEN_KEY_NAME,
                             CDP_PRIVATE_KEY_KEY_NAME]
 
     def __init__(self, config_writer=None):
         super(ConfigureSetCommand, self).__init__()
         if config_writer is None:
             config_writer = ConfigFileWriter()
         self._config_writer = config_writer
@@ -98,17 +96,14 @@
                     value = {parts[1]: value}
             elif len(parts) == 2:
                 # Otherwise it's something like "set preview.service true"
                 # of something in the [plugin] section.
                 section, varname = parts
         config_filename = os.path.expanduser(
             context.get_config_variable('config_file'))
-        if varname == CDP_PRIVATE_KEY_KEY_NAME:
-            # V3/ECDSA private key has '\n' in the string.
-            value = value.replace('\n', '\\n')
         updated_config = {'__section__': section, varname: value}
         if varname in self._WRITE_TO_CREDS_FILE:
             config_filename = os.path.expanduser(
                 context.get_config_variable('credentials_file'))
             section_name = updated_config['__section__']
             if section_name.startswith('profile '):
                 updated_config['__section__'] = section_name[8:]
```

### Comparing `cdpcli-0.9.89/cdpcli/extensions/generatecliskeleton.py` & `cdpcli-0.9.9/cdpcli/extensions/generatecliskeleton.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,16 @@
     }
 
     def __init__(self, operation_model):
         super(GenerateCliSkeletonArgument, self).__init__()
         self._operation_model = operation_model
 
     def invoke(self,
-               client_creator,
-               operation_model,
+               client,
+               operation_name,
                parameters,
                parsed_args,
                parsed_globals):
         return self._generate_json_skeleton(parsed_args)
 
     def _generate_json_skeleton(self, parsed_args):
```

### Comparing `cdpcli-0.9.89/cdpcli/extensions/paginate.py` & `cdpcli-0.9.9/cdpcli/extensions/paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.89/cdpcli/extensions/refdoc.py` & `cdpcli-0.9.9/cdpcli/help.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,145 +1,226 @@
-# Copyright 2021 Cloudera, Inc. All rights reserved.
+# Copyright 2012-2013 Amazon.com, Inc. or its affiliates. All Rights Reserved.
+#
+# Modifications made by Cloudera are:
+#     Copyright (c) 2016 Cloudera, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"). You
 # may not use this file except in compliance with the License. A copy of
 # the License is located at
 #
 #     http://aws.amazon.com/apache2.0/
 #
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 import os
+import platform
+import shlex
+from subprocess import PIPE
+from subprocess import Popen
 
-from cdpcli import VERSION
+from cdpcli.argparser import ArgTableArgParser
+from cdpcli.argprocess import ParamShorthand
 from cdpcli.doc.restdoc import ReSTDocument
-from cdpcli.extensions.commands import BasicCommand
-from cdpcli.help import HelpCommand
-from cdpcli.help import NullRenderer
+from cdpcli.docs import generate_doc
+from cdpcli.docs import OperationDocumentGenerator
+from cdpcli.docs import ProviderDocumentGenerator
+from cdpcli.docs import ServiceDocumentGenerator
+from cdpcli.exceptions import ExecutableNotFoundError
+from cdpcli.textwriter import TextWriter
+from cdpcli.utils import ignore_ctrl_c
+from docutils.core import publish_string
+from docutils.writers import manpage
 
 
-class RefdocCommand(BasicCommand):
+def get_renderer():
     """
-    The 'cdp refdoc' command handler.
+    Return the appropriate HelpRenderer implementation for the
+    current platform.
     """
+    if platform.system() == 'Windows':
+        return WindowsHelpRenderer()
+    else:
+        return PosixHelpRenderer()
+
+
+class PagingHelpRenderer(object):
+    PAGER = None
+
+    def get_pager_cmdline(self):
+        pager = self.PAGER
+        if 'MANPAGER' in os.environ:
+            pager = os.environ['MANPAGER']
+        elif 'PAGER' in os.environ:
+            pager = os.environ['PAGER']
+        return shlex.split(pager)
 
-    NAME = 'refdoc'
-    DESCRIPTION = ('Generate reference documentation. Files formatted as '
-                   'reStructuredText are written to the output directory. They '
-                   'may be used as input to the Sphinx documentation generator '
-                   'to produce a readable documentation site in any of several '
-                   'formats.')
-    EXAMPLES = (
-        'To generate reference documentation::\n'
-        '\n'
-        '    $ cdp refdoc --output-directory sphinx/source\n'
-    )
-    SUBCOMMANDS = []
-    ARG_TABLE = [
-        {
-            'name': 'output-directory',
-            'help_text': 'Directory where generated files are written.',
-            'action': 'store',
-            'required': True,
-            'cli_type_name': 'string'
-        }
-    ]
-
-    def __init__(self):
-        super(RefdocCommand, self).__init__()
-
-    def _write_ref_docs(self, command, output_dir, client_creator, parsed_args,
-                        parsed_globals):
-        """
-        Write all of the documents for one command. If the command has
-        subcommands, then documents for those are generated recursively.
-        """
-        self._write_ref_doc(command, output_dir, client_creator, parsed_args,
-                            parsed_globals)
-        if hasattr(command, '_get_command_table'):
-            subcommand_table = command._get_command_table()
-        elif hasattr(command, 'subcommand_table'):
-            subcommand_table = command.subcommand_table
-        else:
-            subcommand_table = None
-        if subcommand_table:
-            for subcommand in subcommand_table.values():
-                self._write_ref_docs(subcommand, output_dir, client_creator,
-                                     parsed_args, parsed_globals)
-
-    def _write_ref_doc(self, command, output_dir, client_creator, parsed_args,
-                       parsed_globals):
+    def render(self, contents):
         """
-        Write the document for a single command.
+        Each implementation of HelpRenderer must implement this
+        render method.
         """
+        converted_content = self._convert_doc_content(contents)
+        self._send_output_to_pager(converted_content)
 
-        # Get the help command for the command to be documented.
-        if isinstance(command, HelpCommand):
-            help_command = command
-        else:
-            help_command = command.create_help_command()
-
-        # Derive the path of the command's documentation file, relative to the
-        # output directory.
-        # - Top-level commands, and any other commands that have subcommands,
-        #   get index.rst files in directories of their own. Examples:
-        #   - command foo => foo/index.rst (whether it has subcommands or not)
-        #   - subcommand bar, which itself has subcommands, of command foo =>
-        #     foo/bar/index.rst
-        # - Leaf subcommands get files named after themselves inside the
-        #   directory of their parent command. Example:
-        #   - subcommand baz of command foo => foo/baz.rst
-        # - Commands with no lineage (just cdp!) go to index.rst. If there are
-        #   ever multiple lineage-less commands, this needs to be changed!
-        if hasattr(command, 'lineage'):
-            lineage = command.lineage
-        else:
-            lineage = []
-        if len(lineage) > 0:
-            ref_doc_partial_path = '/'.join(map(lambda c: c.name, lineage))
-            if (hasattr(command, '_get_command_table') and  # has subcommands
-                command._get_command_table()) or \
-               (hasattr(command, 'subcommand_table') and  # has subcommands
-                command.subcommand_table) or \
-               len(lineage) == 1:  # is a top-level command (force this case)
-                ref_doc_path = '{}/index.rst'.format(ref_doc_partial_path)
-            else:
-                ref_doc_path = '{}.rst'.format(ref_doc_partial_path)
-        else:
-            ref_doc_path = 'index.rst'  # the cdp command itself
-        print('- {}'.format(ref_doc_path))
-
-        # Run the help command to generate a ReST document suitable for HTML
-        # conversion.
-        help_command.doc = ReSTDocument(target='html')
-        help_command.renderer = NullRenderer()
-        help_command.include_man_fields = False
-        help_command(client_creator, [], parsed_globals)
-
-        # Create the directory for the document, if it doesn't already exist.
-        ref_doc_dir = os.path.join(output_dir, os.path.dirname(ref_doc_path))
-        if not os.path.exists(ref_doc_dir):
-            os.makedirs(ref_doc_dir)
-
-        # Write out the doc "value", which is the ReST string, to the file.
-        content = help_command.doc.getvalue()
-        with open(os.path.join(output_dir, ref_doc_path), 'w') as ref_doc:
-            ref_doc.write(str(content, encoding='utf-8'))
-
-    def _run_main(self, client_creator, parsed_args, parsed_globals):
-        if not os.path.exists(parsed_args.output_directory):
-            os.makedirs(parsed_args.output_directory)
-
-        # Write documents for every known command.
-        command_table = parsed_globals.command_table  # uses argparser hack
-        for command in command_table.values():
-            self._write_ref_docs(command, parsed_args.output_directory,
-                                 client_creator, parsed_args, parsed_globals)
-
-        # Write a file with the version string. This may be passed as a Sphinx
-        # configuration value for use in generated documentation.
-        with open(os.path.join(parsed_args.output_directory,
-                               '_version'), 'w') as version_file:
-            version_file.write(VERSION)
+    def _send_output_to_pager(self, output):
+        cmdline = self.get_pager_cmdline()
+        p = self._popen(cmdline, stdin=PIPE)
+        p.communicate(input=output)
+
+    def _popen(self, *args, **kwargs):
+        return Popen(*args, **kwargs)
+
+    def _convert_doc_content(self, contents):
+        return contents
+
+
+class PosixHelpRenderer(PagingHelpRenderer):
+    PAGER = 'less -R'
+
+    def _convert_doc_content(self, contents):
+        man_contents = publish_string(contents, writer=manpage.Writer())
+        if not self._exists_on_path('groff'):
+            raise ExecutableNotFoundError(executable_name='groff')
+        cmdline = ['groff', '-man', '-T', 'ascii']
+        p3 = self._popen(cmdline, stdin=PIPE, stdout=PIPE, stderr=PIPE)
+        groff_output = p3.communicate(input=man_contents)[0]
+        return groff_output
+
+    def _send_output_to_pager(self, output):
+        cmdline = self.get_pager_cmdline()
+        with ignore_ctrl_c():
+            # We can't rely on the KeyboardInterrupt from
+            # the CLIDriver being caught because when we
+            # send the output to a pager it will use various
+            # control characters that need to be cleaned
+            # up gracefully.  Otherwise if we simply catch
+            # the Ctrl-C and exit, it will likely leave the
+            # users terminals in a bad state and they'll need
+            # to manually run ``reset`` to fix this issue.
+            # Ignoring Ctrl-C solves this issue.  It's also
+            # the default behavior of less (you can't ctrl-c
+            # out of a manpage).
+            p = self._popen(cmdline, stdin=PIPE)
+            p.communicate(input=output)
+
+    def _exists_on_path(self, name):
+        # Since we're only dealing with POSIX systems, we can
+        # ignore things like PATHEXT.
+        return any([os.path.exists(os.path.join(p, name))
+                    for p in os.environ.get('PATH', '').split(os.pathsep)])
+
+
+class WindowsHelpRenderer(PagingHelpRenderer):
+    """Render help content on a Windows platform."""
+
+    PAGER = 'more'
+
+    def _convert_doc_content(self, contents):
+        text_output = publish_string(contents,
+                                     writer=TextWriter())
+        return text_output
+
+    def _popen(self, *args, **kwargs):
+        # Also set the shell value to True.  To get any of the
+        # piping to a pager to work, we need to use shell=True.
+        kwargs['shell'] = True
+        return Popen(*args, **kwargs)
+
+
+class HelpCommand(object):
+    GeneratorClass = None
+
+    def __init__(self, obj, command_table, arg_table):
+        self.obj = obj
+        if command_table is None:
+            command_table = {}
+        self.command_table = command_table
+        if arg_table is None:
+            arg_table = {}
+        self.arg_table = arg_table
+        self._subcommand_table = {}
+        self._related_items = []
+        self.renderer = get_renderer()
+        self.doc = ReSTDocument(target='man')
+
+    @property
+    def command_lineage(self):
+        pass
+
+    @property
+    def name(self):
+        pass
+
+    @property
+    def subcommand_table(self):
+        return self._subcommand_table
+
+    @property
+    def related_items(self):
+        return self._related_items
+
+    def __call__(self, client_creator, args, parsed_globals):
+        if args:
+            subcommand_parser = ArgTableArgParser({}, self.subcommand_table)
+            parsed, remaining = subcommand_parser.parse_known_args(args)
+            if getattr(parsed, 'subcommand', None) is not None:
+                return self.subcommand_table[parsed.subcommand](remaining,
+                                                                parsed_globals)
+
+        generate_doc(self.GeneratorClass(self), self)
+        self.renderer.render(self.doc.getvalue())
+
+
+class ProviderHelpCommand(HelpCommand):
+    GeneratorClass = ProviderDocumentGenerator
+
+    def __init__(self, command_table, arg_table, description, synopsis, usage):
+        HelpCommand.__init__(self, None, command_table, arg_table)
+        self.description = description
+        self.synopsis = synopsis
+        self.help_usage = usage
+
+    @property
+    def command_lineage(self):
+        return 'cdp'
+
+    @property
+    def name(self):
+        return 'cdp'
+
+
+class ServiceHelpCommand(HelpCommand):
+    GeneratorClass = ServiceDocumentGenerator
+
+    def __init__(self, obj, command_table, arg_table, name, command_lineage):
+        super(ServiceHelpCommand, self).__init__(obj, command_table, arg_table)
+        self._name = name
+        self._command_lineage = command_lineage
+
+    @property
+    def command_lineage(self):
+        return self._command_lineage
+
+    @property
+    def name(self):
+        return self._name
+
+
+class OperationHelpCommand(HelpCommand):
+    GeneratorClass = OperationDocumentGenerator
+
+    def __init__(self, operation_model, arg_table, name, command_lineage):
+        HelpCommand.__init__(self, operation_model, None, arg_table)
+        self.param_shorthand = ParamShorthand()
+        self._name = name
+        self._command_lineage = command_lineage
+
+    @property
+    def command_lineage(self):
+        return self._command_lineage
+
+    @property
+    def name(self):
+        return self._name
```

### Comparing `cdpcli-0.9.89/cdpcli/extensions/writer.py` & `cdpcli-0.9.9/cdpcli/extensions/writer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.89/cdpcli/formatter.py` & `cdpcli-0.9.9/cdpcli/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,19 +69,16 @@
 
     def _format_response(self, command_name, response, stream):
         # For operations that have no response body (e.g. s3 put-object)
         # the response will be an empty string.  We don't want to print
         # that out to the user but other "falsey" values like an empty
         # dictionary should be printed.
         if response != {}:
-            ensure_ascii = self._args.ensure_ascii
-            if ensure_ascii is None:
-                ensure_ascii = False
             json.dump(response, stream, indent=4, default=json_encoder,
-                      ensure_ascii=ensure_ascii)
+                      ensure_ascii=False)
             stream.write('\n')
 
 
 class TableFormatter(FullyBufferedFormatter):
     """Pretty print a table from a given response.
 
     The table formatter is able to take any generic response
```

### Comparing `cdpcli-0.9.89/cdpcli/loader.py` & `cdpcli-0.9.9/cdpcli/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,15 @@
     # returns a list of actual existing directories among search paths
     def _potential_locations(self):
         for path in self._search_paths:
             if os.path.isdir(path):
                 yield path
 
     # lists potential service names in a given search path
-    # which is obtained by shallow listing of subdirectories
+    # which is obtained by sallow listing of subdirectories
     def _potential_services(self, path):
         for child in os.listdir(path):
             full_path = os.path.join(path, child)
             if os.path.isdir(full_path):
                 yield (child, full_path)
 
     def _load_builtin_aliases(self):
```

### Comparing `cdpcli-0.9.89/cdpcli/main.py` & `cdpcli-0.9.9/cdpcli/main.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.89/cdpcli/model.py` & `cdpcli-0.9.9/cdpcli/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,16 +45,14 @@
 
 
 def _get_shape_type(shape_data):
     shape_type = shape_data['type']
     if shape_type == 'string':
         if shape_data.get('format', None) == 'date-time':
             return 'datetime'
-        if shape_data.get('format', None) == 'byte':
-            return 'blob'
     if shape_type == 'number':
         return shape_data.get('format')
     if shape_type == 'object':
         if ADDITIONAL_PROPERTIES in shape_data:
             return 'map'
     return shape_type
 
@@ -108,31 +106,26 @@
         return self._shape_data.get('x-paging-page-size', False)
 
     @CachedProperty
     def is_no_paramfile(self):
         return self._shape_data.get('x-no-paramfile', False)
 
     @CachedProperty
-    def is_deprecated(self):
+    def is_undocumented(self):
         return self._shape_data.get('x-deprecated', False)
 
-    @CachedProperty
-    def form_factors(self):
-        if "x-form-factors" in self._shape_data:
-            return self._shape_data['x-form-factors'].split(',')
-        return None
-
     def _get_shape(self, name, shape_data):
         if REF_KEY in shape_data:
             # Reference value type
             # $ref: '#/definitions/SomeObject'
             return self._shape_resolver.resolve_shape_ref(name,
                                                           shape_data[REF_KEY])
         elif TYPE_KEY in shape_data:
-            # Explicit value type, e.g., SomeShapeType
+            # Explicit value type
+            # type: SomeShapeType
             return self._shape_resolver.get_shape(name, shape_data)
         else:
             raise InvalidShapeError("Unknown %s content: %s"
                                     % shape_data, self.name)
 
 
 class ObjectShape(Shape):
@@ -168,18 +161,14 @@
 
 class StringShape(Shape):
     @CachedProperty
     def enum(self):
         return self._shape_data.get('enum', [])
 
     @CachedProperty
-    def deprecated_enum_values(self):
-        return self._shape_data.get('x-deprecated-enum-values', [])
-
-    @CachedProperty
     def supported_options(self):
         return self._shape_data.get('x-supported-options', [])
 
 
 class ShapeResolver(object):
 
     def __init__(self, definitions):
@@ -196,16 +185,15 @@
                 shape_cls = ArrayShape
             elif shape_type == 'string':
                 shape_cls = StringShape
             elif shape_type in ['integer',
                                 'float',
                                 'double',
                                 'boolean',
-                                'datetime',
-                                'blob']:
+                                'datetime']:
                 shape_cls = Shape
             else:
                 raise InvalidShapeError("Unknown shape type: %s" % shape_type)
         except KeyError:
             raise InvalidShapeError("Shape is missing required key 'type': %s"
                                     % (shape_data))
         return shape_cls(name, shape_data, self)
@@ -242,25 +230,20 @@
         return self._name
 
     @property
     def service_model(self):
         return self._service_model
 
     @CachedProperty
-    def summary(self):
-        return self._operation_data["summary"]
-
-    @CachedProperty
     def documentation(self):
         return self._operation_data["description"]
 
     @CachedProperty
     def can_paginate(self):
-        # A valid paginating operation always has x-paging-default-max-items
-        return "x-paging-default-max-items" in self._operation_data
+        return self._operation_data.get("x-paginates", False)
 
     @CachedProperty
     def paging_input_token(self):
         if self.can_paginate:
             for name, shape in self.input_shape.members.items():
                 if shape.is_paging_input_token:
                     return name
@@ -293,42 +276,22 @@
     @CachedProperty
     def paging_default_max_items(self):
         if self.can_paginate:
             return int(self._operation_data.get("x-paging-default-max-items"))
         return None
 
     @CachedProperty
-    def is_deprecated(self):
-        return self._operation_data.get('x-deprecated', False)
-
-    @CachedProperty
-    def form_factors(self):
-        if "x-form-factors" in self._operation_data:
-            return self._operation_data['x-form-factors'].split(',')
-        return None
-
-    @CachedProperty
-    def extensions(self):
-        if "x-extensions" in self._operation_data:
-            return self._operation_data['x-extensions'].split(',')
-        return None
-
-    @CachedProperty
     def input_shape(self):
         return self._service_model.resolve_shape_ref(
             "input", self._operation_data['parameters'][0]['schema'][REF_KEY])
 
     @CachedProperty
     def output_shape(self):
-        if '200' in self._operation_data['responses']:
-            return self._service_model.resolve_shape_ref(
-                "output", self._operation_data['responses']['200']['schema'][REF_KEY])
-        else:
-            return self._service_model.resolve_shape_ref(
-                "output", self._operation_data['responses'][200]['schema'][REF_KEY])
+        return self._service_model.resolve_shape_ref(
+            "output", self._operation_data['responses'][200]['schema'][REF_KEY])
 
 
 class ServiceModel(object):
 
     def __init__(self, service_data, service_name):
         self._service_data = service_data
         self._service_name = service_name
@@ -336,76 +299,50 @@
         self._shape_resolver = ShapeResolver(service_data.get('definitions', {}))
 
     @CachedProperty
     def service_name(self):
         return self._service_name
 
     @CachedProperty
-    def service_version(self):
-        return self._service_data["info"]["version"]
-
-    @CachedProperty
-    def service_title(self):
-        return self._service_data["info"]["title"]
-
-    @CachedProperty
     def documentation(self):
         return self._service_data["info"]["description"]
 
     @instance_cache
     def operation_model(self, operation_name):
         for request_uri in self._service_data["paths"]:
             for http_method in self._service_data["paths"][request_uri]:
                 operation_data = self._service_data["paths"][request_uri][http_method]
                 if operation_data["operationId"] == operation_name:
                     return OperationModel(operation_data,
                                           self,
                                           operation_name,
                                           http_method,
                                           request_uri)
-                if operation_data.get("x-alt-operation-id", None) == operation_name:
-                    operation_data = operation_data.copy()
-                    operation_data["x-deprecated"] = True
-                    return OperationModel(operation_data,
-                                          self,
-                                          operation_name,
-                                          http_method,
-                                          request_uri)
         raise OperationNotFoundError(operation_name)
 
     @CachedProperty
     def operation_names(self):
         operation_names = []
         for path in self._service_data["paths"]:
             for operation in self._service_data["paths"][path]:
-                operation_data = self._service_data["paths"][path][operation]
-                operation_names.append(operation_data["operationId"])
-                if "x-alt-operation-id" in operation_data:
-                    operation_names.append(operation_data["x-alt-operation-id"])
+                operation_names.append(
+                    self._service_data["paths"][path][operation]["operationId"])
         return operation_names
 
     def resolve_shape_ref(self, name, shape_ref):
         return self._shape_resolver.resolve_shape_ref(name, shape_ref)
 
     @CachedProperty
     def endpoint_name(self):
         return self._service_data["x-endpoint-name"]
 
     @CachedProperty
-    def endpoint_prefix(self):
-        return self._service_data.get("x-endpoint-prefix", 'api')
-
-    @CachedProperty
     def products(self):
         return self._service_data.get("x-products", "ALTUS").split(',')
 
-    @CachedProperty
-    def form_factors(self):
-        return self._service_data.get("x-form-factors", "public").split(',')
-
 
 class DenormalizedStructureBuilder(object):
     """Build a StructureShape from a denormalized model.
 
     This is a convenience builder class that makes it easy to construct
     ``StructureShape``s based on a denormalized model.
 
@@ -463,16 +400,15 @@
         elif shape_type == LIST_TYPE:
             shapes[shape_name] = self._build_array(model, shapes)
         elif shape_type in ['string',
                             'integer',
                             'float',
                             'double',
                             'boolean',
-                            'datetime',
-                            'blob']:
+                            'datetime']:
             shapes[shape_name] = self._build_scalar(model)
         else:
             raise InvalidShapeError("Unknown shape type: %s" % model['type'])
 
     def _build_object(self, model, shapes):
         members = OrderedDict()
         shape = self._build_initial_shape(model)
@@ -502,16 +438,14 @@
         shape = {
             'type': model['type'],
         }
         if 'documentation' in model:
             shape['documentation'] = model['documentation']
         if 'enum' in model:
             shape['enum'] = model['enum']
-        if 'x-deprecated-enum-values' in model:
-            shape['x-deprecated-enum-values'] = model['x-deprecated-enum-values']
         if 'x-supported-options' in model:
             shape['x-supported-options'] = model['x-supported-options']
         if 'x-no-paramfile' in model:
             shape['x-no-paramfile'] = model['x-no-paramfile']
         return shape
 
     def _build_scalar(self, model):
```

### Comparing `cdpcli-0.9.89/cdpcli/paginate.py` & `cdpcli-0.9.9/cdpcli/paginate.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,25 +100,17 @@
             # advance to the next page
             self._op_kwargs[self._input_token_key] = \
                 previous_next_token = next_token
 
     # builds a full operation result object by iterating over pages which are
     # fetched using multiple requests to service
     def build_full_result(self):
-        first_response = True
         result = {}
         # iterate over service responses, one response per page of results
         for response in self:
-            if first_response:
-                result = copy(response)
-                if self._result_key in result:
-                    del result[self._result_key]
-                if self._output_token_key in result:
-                    del result[self._output_token_key]
-                first_response = False
             response_value = response.get(self._result_key, None)
             if response_value is None:
                 continue
             existing_value = result.get(self._result_key, None)
             if existing_value is None:
                 result[self._result_key] = copy(response_value)
             elif isinstance(response_value, list):
```

### Comparing `cdpcli-0.9.89/cdpcli/paramfile.py` & `cdpcli-0.9.9/cdpcli/paramfile.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,27 +9,26 @@
 #
 #     http://aws.amazon.com/apache2.0/
 #
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
-
 import os
 
 from cdpcli.compat import compat_open
 from cdpcli.compat import six
-import requests
+from cdpcli.thirdparty import requests
 
 
 class ResourceLoadingError(Exception):
     pass
 
 
-def get_paramfile(path, parsed_globals):
+def get_paramfile(path):
     """Load parameter based on a resource URI.
 
     It is possible to pass parameters to operations by referring
     to files or URI's.  If such a reference is detected, this
     function attempts to retrieve the data from the file or URI
     and returns it.  If there are any errors or if the ``path``
     does not appear to refer to a file or URI, a ``None`` is
@@ -37,44 +36,36 @@
 
     """
     data = None
     if isinstance(path, six.string_types):
         for prefix, function_spec in PREFIX_MAP.items():
             if path.startswith(prefix):
                 function, kwargs = function_spec
-                kwargs['parsed_globals'] = parsed_globals
                 data = function(prefix, path, **kwargs)
     return data
 
 
-def get_file(prefix, path, mode, parsed_globals):
+def get_file(prefix, path, mode):
     file_path = os.path.expandvars(os.path.expanduser(path[len(prefix):]))
     try:
         with compat_open(file_path, mode) as f:
             return f.read()
     except UnicodeDecodeError:
         raise ResourceLoadingError(
             'Unable to load paramfile (%s), text contents could '
             'not be decoded.  If this is a binary file, please use the '
             'fileb:// prefix instead of the file:// prefix.' % file_path)
     except (OSError, IOError) as e:
         raise ResourceLoadingError('Unable to load paramfile %s: %s' % (
             path, e))
 
 
-def get_uri(prefix, uri, parsed_globals):
+def get_uri(prefix, uri):
     try:
-        # The TLS verification value can be a boolean or a CA_BUNDLE path. This
-        # is a little odd, but ultimately comes from the python HTTP requests
-        # library we're using.
-        tls_verification = getattr(parsed_globals, 'verify_tls', True)
-        ca_bundle = getattr(parsed_globals, 'ca_bundle', None)
-        if tls_verification and ca_bundle is not None:
-            tls_verification = ca_bundle
-        r = requests.get(uri, verify=tls_verification)
+        r = requests.get(uri)
         if r.status_code == 200:
             return r.text
         else:
             raise ResourceLoadingError(
                 "received non 200 status code of %s" % (
                     r.status_code))
     except Exception as e:
@@ -86,17 +77,14 @@
     'fileb://': (get_file, {'mode': 'rb'}),
     'http://': (get_uri, {}),
     'https://': (get_uri, {}),
 }
 
 
 class ParamFileVisitor(object):
-    def __init__(self, parsed_globals):
-        self._parsed_globals = parsed_globals
-
     """
     This visitor's visit method will walk the input params object of the input
     shape, visiting all fields and recursing through complex fields. Any string
     field encountered will get paramfile resolution unless it is marked in the
     model as being x-no-paramfile.
     """
 
@@ -135,34 +123,22 @@
     def _visit_float(self, param, shape, name):
         return param
 
     def _visit_double(self, param, shape, name):
         return param
 
     def _visit_string(self, param, shape, name):
-        if not getattr(self._parsed_globals, 'expand_param', True):
-            return param
         if shape.is_no_paramfile:
             return param
-        override = get_paramfile(param, self._parsed_globals)
+        override = get_paramfile(param)
         if override is not None:
             return override
         return param
 
     def _visit_array(self, param, shape, name):
         visited = []
         for i, item in enumerate(param):
             visited.append(self._visit(item, shape.member, '%s[%s]' % (name, i)))
         return visited
 
     def _visit_datetime(self, param, shape, name):
         return param
-
-    def _visit_blob(self, param, shape, name):
-        if not getattr(self._parsed_globals, 'expand_param', True):
-            return param
-        if shape.is_no_paramfile:
-            return param
-        override = get_paramfile(param, self._parsed_globals)
-        if override is not None:
-            return override
-        return param
```

### Comparing `cdpcli-0.9.89/cdpcli/retryhandler.py` & `cdpcli-0.9.9/cdpcli/retryhandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 import functools
 import logging
 
 from cdpcli.exceptions import EndpointConnectionError
-from requests import ConnectionError, Timeout
-from urllib3.exceptions import ClosedPoolError
+from cdpcli.thirdparty.requests import ConnectionError, Timeout
+from cdpcli.thirdparty.requests.packages.urllib3.exceptions \
+    import ClosedPoolError
 
 
 LOG = logging.getLogger('cdpcli.retryhandler')
 # The only supported error for now is GENERAL_CONNECTION_ERROR
 # which maps to requests generic ConnectionError.  If we're able
 # to get more specific exceptions from requests we can update
 # this mapping with more specific exceptions.
```

### Comparing `cdpcli-0.9.89/cdpcli/schema.py` & `cdpcli-0.9.9/cdpcli/schema.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.89/cdpcli/serialize.py` & `cdpcli-0.9.9/cdpcli/serialize.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,40 +10,28 @@
 #     http://aws.amazon.com/apache2.0/
 #
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
-import base64
-
 from cdpcli import validate
 from cdpcli.compat import json
 from cdpcli.compat import OrderedDict
-from cdpcli.compat import six
 
 
 def create_serializer():
     serializer = Serializer()
     validator = validate.ParamValidator()
     return validate.ParamValidationDecorator(validator, serializer)
 
 
 class Serializer(object):
     DEFAULT_ENCODING = 'utf-8'
 
-    def _get_base64(self, value):
-        # Returns the base64-encoded version of value, handling
-        # both strings and bytes. The returned value is a string
-        # via the default encoding.
-        if isinstance(value, six.string_types):
-            value = value.encode(self.DEFAULT_ENCODING)
-        return base64.b64encode(value).strip().decode(
-            self.DEFAULT_ENCODING)
-
     def serialize_to_request(self, parameters, operation_model):
         # Don't serialize any parameter with a None value.
         filtered_parameters = OrderedDict(
             (k, v) for k, v in parameters.items() if v is not None)
 
         serialized = {}
         serialized['method'] = operation_model.http['method']
@@ -85,20 +73,9 @@
             # JSON list serialization is the only case where we aren't setting
             # a key on a dict.  We handle this by using a __current__ key on a
             # wrapper dict to serialize each list item before appending it to
             # the serialized list.
             self._serialize(wrapper, array_item, shape.member, "__current__")
             array_obj.append(wrapper["__current__"])
 
-    def _serialize_type_blob(self, serialized, value, shape, key):
-        # Blob args must be base64 encoded.
-        # If value type is string/text, it is already base64 encoded, verified
-        # in validate.py.
-        # Use isinstance(six.string_types) because a string could be either str
-        # or unicode in python2.
-        if isinstance(value, six.string_types):
-            serialized[key] = value
-        else:
-            serialized[key] = self._get_base64(value)
-
     def _default_serialize(self, serialized, value, shape, key):
         serialized[key] = value
```

### Comparing `cdpcli-0.9.89/cdpcli/shorthand.py` & `cdpcli-0.9.9/cdpcli/shorthand.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,17 @@
 #     http://aws.amazon.com/apache2.0/
 #
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
-import logging
 import re
 import string
 
-LOG = logging.getLogger('cdpcli.shorthand')
 _EOF = object()
 
 
 class _NamedRegex(object):
     def __init__(self, name, regex_str):
         self.name = name
         self.regex = re.compile(regex_str, re.UNICODE)
@@ -76,17 +74,17 @@
     Note that this parser does not rely on any JSON models to control
     how to parse the shorthand syntax.
 
     """
 
     _SINGLE_QUOTED = _NamedRegex('singled quoted', r'\'(?:\\\\|\\\'|[^\'])*\'')
     _DOUBLE_QUOTED = _NamedRegex('double quoted', r'"(?:\\\\|\\"|[^"])*"')
-    _START_WORD = u'\\!\\#-&\\(-\\+\\--\\<\\>-Z\\\\-z\u007c-\uffff'
-    _FIRST_FOLLOW_CHARS = u'\\s\\!\\#-&\\(-\\+\\--\\\\\\^-\\|~-\uffff'
-    _SECOND_FOLLOW_CHARS = u'\\s\\!\\#-&\\(-\\+\\--\\<\\>-\uffff'
+    _START_WORD = u'\!\#-&\(-\+\--\<\>-Z\\\\-z\u007c-\uffff'
+    _FIRST_FOLLOW_CHARS = u'\s\!\#-&\(-\+\--\\\\\^-\|~-\uffff'
+    _SECOND_FOLLOW_CHARS = u'\s\!\#-&\(-\+\--\<\>-\uffff'
     _ESCAPED_COMMA = '(\\\\,)'
     _FIRST_VALUE = _NamedRegex(
         'first',
         u'({escaped_comma}|[{start_word}])'
         u'({escaped_comma}|[{follow_chars}])*'.format(
             escaped_comma=_ESCAPED_COMMA,
             start_word=_START_WORD,
@@ -124,22 +122,15 @@
 
     def _parameter(self):
         # parameter = keyval *("," keyval)
         params = {}
         params.update(self._keyval())
         while self._index < len(self._input_value):
             self._expect(',', consume_whitespace=True)
-            keyval = self._keyval()
-            for key in keyval.keys():
-                if key in params:
-                    LOG.warn('A value for the key "%s" was given more than '
-                             'once. Only the last value listed will be used. '
-                             'Separate multiple sets of key-value pairs with '
-                             'spaces.', key)
-            params.update(keyval)
+            params.update(self._keyval())
         return params
 
     def _keyval(self):
         # keyval = key "=" [values]
         key = self._key()
         self._expect('=', consume_whitespace=True)
         values = self._values()
```

### Comparing `cdpcli-0.9.89/cdpcli/signers.py` & `cdpcli-0.9.9/cdpcli/signers.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,12 +48,12 @@
         cls = cdpcli.auth.AUTH_TYPE_MAPS.get(signature_version)
         if cls is None:
             raise UnknownSignatureVersionError(
                 signature_version=signature_version)
         # If there's no credentials provided (i.e credentials is None),
         # then we'll pass a value of "None" over to the auth classes,
         # which already handle the cases where no credentials have
-        # been provided (by failing ...).
+        # been provided.
         frozen_credentials = self._credentials.get_frozen_credentials()
         kwargs['credentials'] = frozen_credentials
         auth = cls(**kwargs)
         return auth
```

### Comparing `cdpcli-0.9.89/cdpcli/table.py` & `cdpcli-0.9.9/cdpcli/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,17 +147,17 @@
 
     def style_indentation_char(self, text):
         return text
 
 
 class ColorizedStyler(Styler):
     def __init__(self):
-        # `autoreset` allows us to not have to sent reset sequences for every
-        # string. `strip` lets us preserve color when redirecting.
-        colorama.init(autoreset=True, strip=False)
+        # autoreset allows us to not have to sent
+        # reset sequences for every string.
+        colorama.init(autoreset=True)
 
     def style_title(self, text):
         # Originally bold + underline
         return text
 
     def style_header_column(self, text):
         # Originally underline
```

### Comparing `cdpcli-0.9.89/cdpcli/text.py` & `cdpcli-0.9.9/cdpcli/text.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.89/cdpcli/textwriter.py` & `cdpcli-0.9.9/cdpcli/textwriter.py`

 * *Files 0% similar despite different names*

```diff
@@ -766,20 +766,14 @@
         raise nodes.SkipNode
 
     def visit_raw(self, node):
         if 'text' in node.get('format', '').split():
             self.body.append(node.astext())
         raise nodes.SkipNode
 
-    def visit_docinfo(self, node):
-        raise nodes.SkipNode
-
-    def visit_version(self, node):
-        raise nodes.SkipNode
-
     def _visit_admonition(self, node):
         self.new_state(2)
 
     def _make_depart_admonition(name):
         def depart_admonition(self, node):
             self.end_state(first=name.capitalize() + ': ')
         return depart_admonition
```

### Comparing `cdpcli-0.9.89/cdpcli/thirdparty/six.py` & `cdpcli-0.9.9/cdpcli/thirdparty/six.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.89/cdpcli/translate.py` & `cdpcli-0.9.9/cdpcli/translate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.89/cdpcli/utils.py` & `cdpcli-0.9.9/cdpcli/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,63 +13,34 @@
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 import contextlib
 import datetime
 import functools
-import importlib
 import re
 import signal
-import urllib.parse as urlparse
 
 from cdpcli import LIST_TYPE
 from cdpcli import MAP_TYPE
 from cdpcli import OBJECT_TYPE
 from cdpcli.compat import compat_tzlocal
 from cdpcli.compat import OrderedDict
 import dateutil.parser
 from dateutil.tz import tzutc
 
 # These are chars that do not need to be urlencoded based on rfc2986, section 2.3.
 SAFE_CHARS = '-._~'
 
 
-def import_module(module_name):
-    try:
-        return importlib.import_module(module_name)
-    except ImportError:
-        return None
-
-
-def get_extension_registers(name):
-    module = import_module('cdpcli.extensions.%s.register' % name)
-    if module is None:
-        module = import_module('cdpcli.extensions.%s' % name)
-    if module is None:
-        return None, None
-
-    register = getattr(module, 'register', None)
-    if register is not None:
-        return register, None
-
-    register_ext = getattr(module, 'register_extension', None)
-    register_cmd = getattr(module, 'register_command', None)
-    return register_ext, register_cmd
-
-
-def is_absolute_url(url):
-    return bool(urlparse.urlparse(url).netloc)
-
-
 def get_service_module_name(service_model):
     name = service_model.service_name
     name = name.replace('Cloudera', '')
     name = name.replace('CDP', '')
-    name = re.sub('\\W+', '', name)
+    name = re.sub('\W+', '', name)
     return name
 
 
 def json_encoder(obj):
     """JSON encoder that formats datetimes as ISO8601 format."""
     if isinstance(obj, datetime.datetime):
         return obj.isoformat()
@@ -115,15 +86,14 @@
             cache_key = (func_name, args, kwarg_items)
         result = self._instance_cache.get(cache_key)
         if result is not None:
             return result
         result = func(self, *args, **kwargs)
         self._instance_cache[cache_key] = result
         return result
-
     return _cache_guard
 
 
 def parse_timestamp(value):
     """Parse a timestamp into a datetime object.
 
     Supported formats:
@@ -217,15 +187,15 @@
     if dt.tzinfo is None:
         if default_timezone is None:
             default_timezone = tzutc()
         dt = dt.replace(tzinfo=default_timezone)
     d = dt.replace(tzinfo=None) - dt.utcoffset() - epoch
     if hasattr(d, "total_seconds"):
         return d.total_seconds()  # Works in Python 2.7+
-    return (d.microseconds + (d.seconds + d.days * 24 * 3600) * 10 ** 6) / 10 ** 6
+    return (d.microseconds + (d.seconds + d.days * 24 * 3600) * 10**6) / 10**6
 
 
 class ArgumentGenerator(object):
     """Generate sample input based on a shape model.
 
     This class contains a ``generate_skeleton`` method that will take
     an input shape (created from ``cdpcli.model``) and generate
@@ -247,15 +217,14 @@
         ddb = clidriver.get_service_model('dataeng')
         arg_gen = ArgumentGenerator()
         sample_input = arg_gen.generate_skeleton(
             ddb.operation_model('createAWSCluster').input_shape)
         print("Sample input for dataeng.createAWSCluster: %s" % sample_input)
 
     """
-
     def __init__(self):
         pass
 
     def generate_skeleton(self, shape):
         if shape.type_name == OBJECT_TYPE:
             return self._generate_type_object(shape)
         elif shape.type_name == LIST_TYPE:
@@ -268,16 +237,14 @@
             return 0
         elif shape.type_name in ['float', 'double']:
             return 0.0
         elif shape.type_name == 'boolean':
             return True
         elif shape.type_name == 'datetime':
             return '2002-10-02T13:00:00+00:00'
-        elif shape.type_name == 'blob':
-            return ''
         else:
             raise Exception("Unknown shape type: %s" % shape.type_name)
 
     def _generate_type_object(self, shape):
         skeleton = OrderedDict()
         for member_name, member_shape in shape.members.items():
             skeleton[member_name] = self.generate_skeleton(member_shape)
```

### Comparing `cdpcli-0.9.89/cdpcli/validate.py` & `cdpcli-0.9.9/cdpcli/validate.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 #     http://aws.amazon.com/apache2.0/
 #
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
-import base64
 import datetime
 import decimal
 
 from cdpcli.compat import six
 from cdpcli.exceptions import ParamValidationError
 from cdpcli.utils import parse_to_aware_datetime
 
@@ -135,17 +134,14 @@
                                min_allowed, max_allowed))
         elif error_type == 'invalid length':
             min_allowed = additional['valid_range'][0]
             max_allowed = additional['valid_range'][1]
             return ('Invalid length for parameter %s, value: %s, valid range: '
                     '%s-%s' % (name, additional['param'],
                                min_allowed, max_allowed))
-        elif error_type == 'invalid base64':
-            return 'Invalid base64 value for parameter %s, error: %s' \
-                % (name, additional['error'])
 
     def _get_name(self, name):
         if not name:
             return 'input'
         elif name.startswith('.'):
             return name[1:]
         else:
@@ -226,25 +222,14 @@
         # to a datetime.
         is_valid_type = self._type_check_datetime(param)
         if not is_valid_type:
             valid_type_names = [six.text_type(datetime), 'timestamp-string']
             errors.report(name, 'invalid type', param=param,
                           valid_types=valid_type_names)
 
-    @type_check(valid_types=(bytes, bytearray, six.string_types))
-    def _validate_blob(self, param, shape, errors, name):
-        if isinstance(param, six.string_types):
-            try:
-                bytes = base64.b64decode(param)
-                length_check(name, len(bytes), shape, 'invalid length', errors)
-            except Exception as err:
-                errors.report(name, 'invalid base64', error=err)
-        else:
-            length_check(name, len(param), shape, 'invalid length', errors)
-
     def _type_check_datetime(self, value):
         try:
             parse_to_aware_datetime(value)
             return True
         except (TypeError, ValueError, AttributeError):
             # Yes, dateutil can sometimes raise an AttributeError when parsing
             # timestamps.
```

### Comparing `cdpcli-0.9.89/tests/unit/__init__.py` & `cdpcli-0.9.9/tests/unit/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,24 +45,14 @@
 zU0IHNaprGxO+yZuMvdyfxcJVuFQf22mujPI8GluXyfA5i2IZjScNf5Awccu8HS5
 mzJp12+5oAZ+tJE1scpVoaVdZloY8XA1u0aCt2BhZavjIizTyzY4L8clo2iGIO1x
 yj5v7z/1wWTorT4w3/IHcwM=
 -----END PRIVATE KEY-----"""
 
 ED25519_KEY = 'VHswlNpwJnMpuXhIq7LYDfzs+R9pHvVLqgBGbhcnbSE='
 
-ECDSA_KEY = \
-    """-----BEGIN PRIVATE KEY-----
-MIH3AgEAMBAGByqGSM49AgEGBSuBBAAjBIHfMIHcAgEBBEIB/VhgNb6ccDq9hV/s
-TD8f1hSZo2Y7A7zZbCK0418vU0HYOi4Ic8TKjKIYw8cMQN7+2fGLQTkGezgu9NBw
-gzR/LGKgBwYFK4EEACOhgYkDgYYABAGxMOPpk3m7wgXPRHBCSpW9as4tuCv38UJQ
-37xSJqmim6LlF6s/eFRpRktNO98fLuAvAFt+97iYwOfhix4h/uVCSgFR0xloJtMe
-MEQft1ColfYUlGSiNuMsGyugK/ilkmulX52Y7z3RY6hxlFAegHI8d9uzeVqUL+KO
-1xtgNBDXVMnQCA==
------END PRIVATE KEY-----"""
-
 
 class FakeContext(object):
 
     def __init__(self,
                  all_variables,
                  profile_does_not_exist=False,
                  config_file_vars={},
@@ -75,15 +65,15 @@
         self.environment_vars = environment_vars
         self._credentials = credentials
         self.profile = None
         self.effective_profile = None
         # This lets us use the FakeContext as both context and "client_creator"
         self.context = self
 
-    def get_credentials(self, parsed_globals=None):
+    def get_credentials(self):
         return self._credentials
 
     def get_scoped_config(self):
         if self.profile_does_not_exist:
             raise ProfileNotFound(profile='foo')
         return self.config
```

### Comparing `cdpcli-0.9.89/tests/unit/cdp/__init__.py` & `cdpcli-0.9.9/tests/unit/cdp/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.89/tests/unit/extensions/__init__.py` & `cdpcli-0.9.9/tests/unit/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.89/tests/unit/extensions/configure/test_configure.py` & `cdpcli-0.9.9/tests/unit/extensions/configure/test_configure.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 import os
 
-from cdpcli import CDP_ACCESS_KEY_ID_KEY_NAME, \
-                   CDP_PRIVATE_KEY_KEY_NAME, \
-                   CDP_REGION_KEY_NAME
+from cdpcli import CDP_ACCESS_KEY_ID_KEY_NAME, CDP_PRIVATE_KEY_KEY_NAME
 from cdpcli.compat import six
 from cdpcli.endpoint import EndpointResolver
 from cdpcli.extensions.configure import configure
 from cdpcli.extensions.configure import ConfigValue
 from cdpcli.extensions.configure import CREDENTIAL_FILE_COMMENT
 from cdpcli.extensions.configure import NOT_SET
 import mock
@@ -32,18 +30,17 @@
 
 class TestConfigureCommand(unittest.TestCase):
 
     def setUp(self):
         self.writer = mock.Mock()
         self.global_args = mock.Mock()
         self.global_args.profile = None
-        self.precanned = PrecannedPrompter(access_key_id='new_access_key_id',
-                                           private_key='new_private_key',
-                                           cdp_region=None,
-                                           cdp_endpoint_url=None)
+        self.global_args.endpoint_url = None
+        self.global_args.cdp_endpoint_url = None
+        self.precanned = PrecannedPrompter(value='new_value')
         self.context = FakeContext({'config_file': 'myconfigfile'})
         self.configure = configure.ConfigureCommand(prompter=self.precanned,
                                                     config_writer=self.writer)
 
     def assert_credentials_file_updated_with(self,
                                              new_values,
                                              config_file_comment=None):
@@ -55,59 +52,80 @@
                                    expected_creds_file,
                                    config_file_comment=config_file_comment))
 
     def test_configure_command_sends_values_to_writer(self):
         self.configure(self.context, args=[], parsed_globals=self.global_args)
         # Credentials are always written to the shared credentials file.
         self.assert_credentials_file_updated_with(
-            {CDP_ACCESS_KEY_ID_KEY_NAME: 'new_access_key_id',
-             CDP_PRIVATE_KEY_KEY_NAME: 'new_private_key'},
+            {CDP_ACCESS_KEY_ID_KEY_NAME: 'new_value',
+             CDP_PRIVATE_KEY_KEY_NAME: 'new_value'},
             config_file_comment=CREDENTIAL_FILE_COMMENT)
 
         # Non-credentials config is written to the config file.
         self.writer.update_config.assert_called_with(
             {}, 'myconfigfile')
 
-    def test_configure_command_with_new_values(self):
-        self.precanned = PrecannedPrompter(access_key_id='new_access_key_id',
-                                           private_key='new_private_key',
-                                           cdp_region='us-west-2',
-                                           cdp_endpoint_url='http://foo.com')
-        self.configure = configure.ConfigureCommand(prompter=self.precanned,
-                                                    config_writer=self.writer)
+    def test_configure_command_with_endpoint_url(self):
+        self.global_args.endpoint_url = "http://foo.com"
+        self.configure(self.context, args=[], parsed_globals=self.global_args)
+        # Credentials are always written to the shared credentials file.
+        self.assert_credentials_file_updated_with(
+            {CDP_ACCESS_KEY_ID_KEY_NAME: 'new_value',
+             CDP_PRIVATE_KEY_KEY_NAME: 'new_value'},
+            config_file_comment=CREDENTIAL_FILE_COMMENT)
+
+        # Non-credentials config is written to the config file.
+        self.writer.update_config.assert_called_with(
+            {EndpointResolver.ENDPOINT_URL_KEY_NAME: "http://foo.com"}, 'myconfigfile')
+
+    def test_configure_command_with_cdp_endpoint_url(self):
+        self.global_args.cdp_endpoint_url = "http://foo.com"
         self.configure(self.context, args=[], parsed_globals=self.global_args)
         # Credentials are always written to the shared credentials file.
         self.assert_credentials_file_updated_with(
-            {CDP_ACCESS_KEY_ID_KEY_NAME: 'new_access_key_id',
-             CDP_PRIVATE_KEY_KEY_NAME: 'new_private_key'},
+            {CDP_ACCESS_KEY_ID_KEY_NAME: 'new_value',
+             CDP_PRIVATE_KEY_KEY_NAME: 'new_value'},
             config_file_comment=CREDENTIAL_FILE_COMMENT)
 
         # Non-credentials config is written to the config file.
         self.writer.update_config.assert_called_with(
-            {CDP_REGION_KEY_NAME: "us-west-2",
-             EndpointResolver.CDP_ENDPOINT_URL_KEY_NAME: "http://foo.com"},
+            {EndpointResolver.CDP_ENDPOINT_URL_KEY_NAME: "http://foo.com"},
+            'myconfigfile')
+
+    def test_configure_command_with_both_endpoint_urls(self):
+        self.global_args.endpoint_url = "http://foo.com"
+        self.global_args.cdp_endpoint_url = "http://bar.com"
+        self.configure(self.context, args=[], parsed_globals=self.global_args)
+        # Credentials are always written to the shared credentials file.
+        self.assert_credentials_file_updated_with(
+            {CDP_ACCESS_KEY_ID_KEY_NAME: 'new_value',
+             CDP_PRIVATE_KEY_KEY_NAME: 'new_value'},
+            config_file_comment=CREDENTIAL_FILE_COMMENT)
+
+        # Non-credentials config is written to the config file.
+        self.writer.update_config.assert_called_with(
+            {EndpointResolver.ENDPOINT_URL_KEY_NAME: "http://foo.com",
+             EndpointResolver.CDP_ENDPOINT_URL_KEY_NAME: "http://bar.com"},
             'myconfigfile')
 
     def test_same_values_are_not_changed(self):
         # If the user enters the same value as the current value, we don't need
         # to write anything to the config.
         self.configure = configure.ConfigureCommand(prompter=EchoPrompter(),
                                                     config_writer=self.writer)
         self.configure(self.context, args=[], parsed_globals=self.global_args)
         self.assertFalse(self.writer.update_config.called)
 
     def test_none_values_are_not_changed(self):
         # If a user hits enter, this will result in a None value which means
         # don't change the existing values.  In this case, we don't need
         # to write anything out to the config.
-        self.precanned = PrecannedPrompter(access_key_id=None,
-                                           private_key=None,
-                                           cdp_region=None,
-                                           cdp_endpoint_url=None)
-        self.configure = configure.ConfigureCommand(prompter=self.precanned,
+        user_presses_enter = None
+        precanned = PrecannedPrompter(value=user_presses_enter)
+        self.configure = configure.ConfigureCommand(prompter=precanned,
                                                     config_writer=self.writer)
         self.configure(self.context, args=[], parsed_globals=self.global_args)
         self.assertFalse(self.writer.update_config.called)
 
     def test_create_configure_cmd(self):
         self.configure = configure.ConfigureCommand()
         self.assertIsInstance(self.configure, configure.ConfigureCommand)
@@ -115,16 +133,16 @@
     def test_section_name_can_be_changed_for_profiles(self):
         # If the user specifies "--profile myname" we need to write
         # this out to the [profile myname] section.
         self.global_args.profile = 'myname'
         self.configure(self.context, args=[], parsed_globals=self.global_args)
         # Note the __section__ key name.
         self.assert_credentials_file_updated_with(
-            {CDP_ACCESS_KEY_ID_KEY_NAME: 'new_access_key_id',
-             CDP_PRIVATE_KEY_KEY_NAME: 'new_private_key',
+            {CDP_ACCESS_KEY_ID_KEY_NAME: 'new_value',
+             CDP_PRIVATE_KEY_KEY_NAME: 'new_value',
              '__section__': 'myname'},
             config_file_comment=CREDENTIAL_FILE_COMMENT)
         self.writer.update_config.assert_called_with(
             {'__section__': 'profile myname'}, 'myconfigfile')
 
     def test_context_says_profile_does_not_exist(self):
         # Whenever you try to get a config value from botocore,
@@ -134,16 +152,16 @@
         context = FakeContext({'config_file': 'myconfigfile'},
                               profile_does_not_exist=True)
         self.configure = configure.ConfigureCommand(prompter=self.precanned,
                                                     config_writer=self.writer)
         self.global_args.profile = 'profile-does-not-exist'
         self.configure(context, args=[], parsed_globals=self.global_args)
         self.assert_credentials_file_updated_with(
-            {CDP_ACCESS_KEY_ID_KEY_NAME: 'new_access_key_id',
-             CDP_PRIVATE_KEY_KEY_NAME: 'new_private_key',
+            {CDP_ACCESS_KEY_ID_KEY_NAME: 'new_value',
+             CDP_PRIVATE_KEY_KEY_NAME: 'new_value',
              '__section__': 'profile-does-not-exist'},
             config_file_comment=CREDENTIAL_FILE_COMMENT)
         self.writer.update_config.assert_called_with(
             {'__section__': 'profile profile-does-not-exist'}, 'myconfigfile')
 
 
 class TestInteractivePrompter(unittest.TestCase):
@@ -195,15 +213,15 @@
         self.assertRegexpMatches(prompt_text, r'\[\*\*\*\*.*\]')
 
     def test_non_secret_keys_are_not_masked(self):
         prompter = configure.InteractivePrompter()
         prompter.get_value(
             current_value='mycurrentvalue', config_name='not_a_secret_key',
             prompt_text='Enter value')
-        # We should display the entire non-secret key.
+        # We should also not display the entire priate key.
         prompt_text = self.stdout.getvalue()
         self.assertIn('mycurrentvalue', prompt_text)
         self.assertRegexpMatches(prompt_text, r'\[mycurrentvalue\]')
 
     def test_user_hits_enter_returns_none(self):
         # If a user hits enter, then raw_input returns the empty string.
         self.mock_raw_input.return_value = ''
@@ -252,30 +270,27 @@
         self.assertEqual(no_config.value, NOT_SET)
         no_config.mask_value()
         self.assertEqual(no_config.value, NOT_SET)
 
 
 class PrecannedPrompter(object):
 
-    def __init__(self, access_key_id, private_key, cdp_region, cdp_endpoint_url):
-        self._access_key_id = access_key_id
-        self._private_key = private_key
-        self._cdp_region = cdp_region
-        self._cdp_endpoint_url = cdp_endpoint_url
+    def __init__(self, value):
+        self._value = value
 
-    def get_value(self, current_value, config_name, prompt_text=''):
-        if config_name == CDP_ACCESS_KEY_ID_KEY_NAME:
-            return self._access_key_id
-        elif config_name == CDP_PRIVATE_KEY_KEY_NAME:
-            return self._private_key
-        elif config_name == CDP_REGION_KEY_NAME:
-            return self._cdp_region
-        elif config_name == EndpointResolver.CDP_ENDPOINT_URL_KEY_NAME:
-            return self._cdp_endpoint_url
-        else:
-            return None
+    def get_value(self, current_value, logical_name, prompt_text=''):
+        return self._value
 
 
 class EchoPrompter(object):
 
-    def get_value(self, current_value, config_name, prompt_text=''):
+    def get_value(self, current_value, logical_name, prompt_text=''):
         return current_value
+
+
+class KeyValuePrompter(object):
+
+    def __init__(self, mapping):
+        self.mapping = mapping
+
+    def get_value(self, current_value, config_name, prompt_text=''):
+        return self.mapping.get(prompt_text)
```

### Comparing `cdpcli-0.9.89/tests/unit/extensions/configure/test_get.py` & `cdpcli-0.9.9/tests/unit/extensions/configure/test_get.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.89/tests/unit/extensions/configure/test_list.py` & `cdpcli-0.9.9/tests/unit/extensions/configure/test_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,147 +10,132 @@
 #     http://aws.amazon.com/apache2.0/
 #
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
-from cdpcli import CDP_ACCESS_KEY_ID_KEY_NAME, \
-                   CDP_PRIVATE_KEY_KEY_NAME, \
-                   CDP_REGION_KEY_NAME
+from cdpcli import CDP_ACCESS_KEY_ID_KEY_NAME, CDP_PRIVATE_KEY_KEY_NAME
 from cdpcli.compat import six
 from cdpcli.extensions.configure.list import ConfigureListCommand
 import mock
 from tests import unittest
 from tests.unit import FakeContext
 
 
 class TestConfigureListCommand(unittest.TestCase):
 
     def test_configure_list_command_nothing_set(self):
         # Test the case where the user only wants to change a single_value.
         context = FakeContext(
             all_variables={'config_file': '/config/location'})
         context.full_config = {
-            'profiles': {'default': {}}}
+            'profiles': {'default': {'region': 'CDP_REGION'}}}
         stream = six.StringIO()
         self.configure_list = ConfigureListCommand(stream)
         self.configure_list(context, args=[], parsed_globals=None)
         rendered = stream.getvalue()
-        self.assertRegexpMatches(rendered, 'profile\\s+<not set>')
-        self.assertRegexpMatches(rendered, 'cdp_region\\s+<not set>')
-        self.assertRegexpMatches(rendered, 'cdp_access_key_id\\s+<not set>')
-        self.assertRegexpMatches(rendered, 'cdp_private_key\\s+<not set>')
+        self.assertRegexpMatches(rendered, 'profile\s+<not set>')
+        self.assertRegexpMatches(rendered, 'access_key\s+<not set>')
+        self.assertRegexpMatches(rendered, 'private_key\s+<not set>')
 
     def test_configure_from_env(self):
         env_vars = {
             'profile': 'myprofilename'
         }
         context = FakeContext(
             all_variables={'config_file': '/config/location'},
             environment_vars=env_vars)
         context.context_var_map = {'profile': (None, "PROFILE_ENV_VAR")}
         context.full_config = {
-            'profiles': {'default': {}}}
+            'profiles': {'default': {'region': 'CDP_REGION'}}}
         stream = six.StringIO()
         self.configure_list = ConfigureListCommand(stream)
         self.configure_list(context, args=[], parsed_globals=None)
         rendered = stream.getvalue()
         self.assertRegexpMatches(
-            rendered, 'profile\\s+myprofilename\\s+env\\s+PROFILE_ENV_VAR')
+            rendered, 'profile\s+myprofilename\s+env\s+PROFILE_ENV_VAR')
 
     def test_configure_from_config_file(self):
+        # this is not a known configuration so this is ignored.
         config_file_vars = {
-            # this is not a known configuration so this is ignored.
             'foo': 'bar',
-            CDP_REGION_KEY_NAME: 'eu-1',
             CDP_ACCESS_KEY_ID_KEY_NAME: 'key_id',
             CDP_PRIVATE_KEY_KEY_NAME: 'mysecretkey'
         }
         context = FakeContext(
             all_variables={'config_file': '/config/location'},
             config_file_vars=config_file_vars)
-        context.context_var_map = {'region': ()}
+        context.context_var_map = {'region': ('region', "CDP_REGION")}
         context.full_config = {
-            'profiles': {'default': {}}}
+            'profiles': {'default': {'region': 'CDP_REGION'}}}
         stream = six.StringIO()
         self.configure_list = ConfigureListCommand(stream)
         self.configure_list(context, args=[], parsed_globals=None)
         rendered = stream.getvalue()
         self.assertRegexpMatches(
-            rendered, 'profile\\s+<not set>\\s+None\\s+None')
+            rendered, 'profile\s+<not set>\s+None\s+None')
         self.assertRegexpMatches(
-            rendered, 'cdp_region\\s+eu-1\\s+config-file')
+            rendered, r'access_key\s+\*+y_id\s+config-file')
         self.assertRegexpMatches(
-            rendered, 'cdp_access_key_id\\s+\\*+y_id\\s+config-file')
-        self.assertRegexpMatches(
-            rendered, 'cdp_private_key\\s+\\*+tkey\\s+config-file')
+            rendered, r'private_key\s+\*+tkey\s+config-file')
 
     def test_configure_from_multiple_sources(self):
         # Here the profile is from an env var, the
         # region is from the config file, and the credentials
         # are from an iam-role.
         env_vars = {
             'profile': 'myprofilename'
         }
-        config_file_vars = {
-            CDP_REGION_KEY_NAME: 'eu-1'
-        }
         credentials = mock.Mock()
         credentials.access_key_id = 'access_key'
         credentials.private_key = 'private_key'
-        credentials.access_token = None
         credentials.method = 'foobar'
         context = FakeContext(
             all_variables={'config_file': '/config/location'},
             environment_vars=env_vars,
-            config_file_vars=config_file_vars,
+            config_file_vars={},
             credentials=credentials)
         context.context_var_map = {
+            'region': ('region', 'CDP_REGION'),
             'profile': ('profile', 'CDP_DEFAULT_PROFILE')}
         context.full_config = {
-            'profiles': {'default': {}}}
+            'profiles': {'default': {'region': 'CDP_REGION'}}}
         stream = six.StringIO()
         self.configure_list = ConfigureListCommand(stream)
         self.configure_list(context, args=[], parsed_globals=None)
         rendered = stream.getvalue()
         # The profile came from an env var.
         self.assertRegexpMatches(
-            rendered, 'profile\\s+myprofilename\\s+env\\s+CDP_DEFAULT_PROFILE')
-        # The cdp_region came from config file.
-        self.assertRegexpMatches(
-            rendered, 'cdp_region\\s+eu-1\\s+config-file')
+            rendered, 'profile\s+myprofilename\s+env\s+CDP_DEFAULT_PROFILE')
         # The credentials came from 'foobar'.  Note how we're
         # also checking that the access_key/private_key are masked
         # with '*' chars except for the last 4 chars.
         self.assertRegexpMatches(
-            rendered, r'cdp_access_key_id\s+\*+_key\s+foobar')
+            rendered, r'access_key\s+\*+_key\s+foobar')
         self.assertRegexpMatches(
-            rendered, r'cdp_private_key\s+\*+_key\s+foobar')
+            rendered, r'private_key\s+\*+_key\s+foobar')
 
     def test_profile_set_in_context(self):
+        # this is not a known configuration so this is ignored.
         config_file_vars = {
-            # this is not a known configuration so this is ignored.
             'foo': 'bar',
-            CDP_REGION_KEY_NAME: 'eu-1',
             CDP_ACCESS_KEY_ID_KEY_NAME: 'key_id',
             CDP_PRIVATE_KEY_KEY_NAME: 'mysecretkey'
         }
         context = FakeContext(
             all_variables={'config_file': '/config/location'},
             config_file_vars=config_file_vars)
         context.profile = 'dev'
-        context.context_var_map = {}
+        context.context_var_map = {'region': ('region', "CDP_REGION")}
         context.full_config = {
-            'profiles': {'dev': {}}}
+            'profiles': {'dev': {'region': 'CDP_REGION'}}}
         stream = six.StringIO()
         self.configure_list = ConfigureListCommand(stream)
         self.configure_list(context, args=[], parsed_globals=None)
         rendered = stream.getvalue()
         self.assertRegexpMatches(
-            rendered, 'profile\\s+dev\\s+manual\\s+--profile')
-        self.assertRegexpMatches(
-            rendered, 'cdp_region\\s+eu-1\\s+config-file')
+            rendered, 'profile\s+dev\s+manual\s+--profile')
         self.assertRegexpMatches(
-            rendered, r'cdp_access_key_id\s+\*+y_id\s+config-file')
+            rendered, r'access_key\s+\*+y_id\s+config-file')
         self.assertRegexpMatches(
-            rendered, r'cdp_private_key\s+\*+tkey\s+config-file')
+            rendered, r'private_key\s+\*+tkey\s+config-file')
```

### Comparing `cdpcli-0.9.89/tests/unit/extensions/configure/test_set.py` & `cdpcli-0.9.9/tests/unit/extensions/configure/test_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 import os
 
-from cdpcli import CDP_ACCESS_KEY_ID_KEY_NAME, \
-                   CDP_ACCESS_TOKEN_KEY_NAME, \
-                   CDP_PRIVATE_KEY_KEY_NAME
+from cdpcli import CDP_ACCESS_KEY_ID_KEY_NAME, CDP_PRIVATE_KEY_KEY_NAME
 from cdpcli.extensions.configure.set import ConfigureSetCommand
 import mock
 from tests import unittest
 from tests.unit import FakeContext
 
 
 class TestConfigureSetCommand(unittest.TestCase):
@@ -114,33 +112,15 @@
         set_command(self.context,
                     args=[CDP_PRIVATE_KEY_KEY_NAME, 'foo'],
                     parsed_globals=None)
         self.config_writer.update_config.assert_called_with(
             {'__section__': 'default',
              CDP_PRIVATE_KEY_KEY_NAME: 'foo'}, self.fake_credentials_filename)
 
-    def test_access_token_written_to_shared_credentials_file(self):
-        set_command = ConfigureSetCommand(self.config_writer)
-        set_command(self.context,
-                    args=[CDP_ACCESS_TOKEN_KEY_NAME, 'foo'],
-                    parsed_globals=None)
-        self.config_writer.update_config.assert_called_with(
-            {'__section__': 'default',
-             CDP_ACCESS_TOKEN_KEY_NAME: 'foo'}, self.fake_credentials_filename)
-
     def test_access_key_written_to_shared_credentials_file_profile(self):
         set_command = ConfigureSetCommand(self.config_writer)
         set_command(self.context,
                     args=['profile.foo.cdp_access_key_id', 'bar'],
                     parsed_globals=None)
         self.config_writer.update_config.assert_called_with(
             {'__section__': 'foo',
              CDP_ACCESS_KEY_ID_KEY_NAME: 'bar'}, self.fake_credentials_filename)
-
-    def test_configure_set_command_access_key_v3(self):
-        set_command = ConfigureSetCommand(self.config_writer)
-        set_command(self.context,
-                    args=[CDP_PRIVATE_KEY_KEY_NAME, 'foo\nbar'],
-                    parsed_globals=None)
-        self.config_writer.update_config.assert_called_with(
-            {'__section__': 'default',
-             CDP_PRIVATE_KEY_KEY_NAME: 'foo\\nbar'}, self.fake_credentials_filename)
```

### Comparing `cdpcli-0.9.89/tests/unit/extensions/test_cliinputjson.py` & `cdpcli-0.9.9/tests/unit/extensions/test_cliinputjson.py`

 * *Files 22% similar despite different names*

```diff
@@ -62,90 +62,78 @@
         add_cli_input_json(self.operation_model, argument_table)
         arg_handler = argument_table['cli-input-json']
         self.assertIsNotNone(arg_handler)
         self.assertTrue(isinstance(arg_handler, CliInputJSONArgument))
 
     def test_add_to_call_parameters_no_file(self):
         parsed_args = mock.Mock()
-        parsed_globals = mock.Mock()
         # Make the value a JSON string
         parsed_args.cli_input_json = self.input_json
         call_parameters = {}
         self.argument.add_to_call_parameters(
             call_parameters=call_parameters,
-            parsed_args=parsed_args,
-            parsed_globals=parsed_globals
+            parsed_args=parsed_args
         )
         self.assertEqual(call_parameters, {'A': 'foo', 'B': 'bar'})
 
     def test_add_to_call_parameters_with_file(self):
         parsed_args = mock.Mock()
-        parsed_globals = mock.Mock()
         # Make the value a file with JSON located inside.
         parsed_args.cli_input_json = 'file://' + self.temp_file
         call_parameters = {}
         self.argument.add_to_call_parameters(
             call_parameters=call_parameters,
-            parsed_args=parsed_args,
-            parsed_globals=parsed_globals
+            parsed_args=parsed_args
         )
         self.assertEqual(call_parameters, {'A': 'foo', 'B': 'bar'})
 
     def test_add_to_call_parameters_with_file_from_visitor(self):
         temp_file1 = os.path.join(self.temp_dir, 'foo.json')
         with open(temp_file1, 'w') as f:
             f.write("baz")
         temp_file1 = _make_file_uri(temp_file1)
         temp_file2 = os.path.join(self.temp_dir, 'bar.json')
         with open(temp_file2, 'w') as f:
             f.write('{"A": "foo", "B": "file://%s"}' % temp_file1)
         temp_file2 = _make_file_uri(temp_file2)
         parsed_args = mock.Mock()
         parsed_args.cli_input_json = 'file://' + temp_file2
-        parsed_globals = mock.Mock()
         call_parameters = {}
         self.argument.add_to_call_parameters(
             call_parameters=call_parameters,
-            parsed_args=parsed_args,
-            parsed_globals=parsed_globals
+            parsed_args=parsed_args
         )
         self.assertEqual(call_parameters, {'A': 'foo', 'B': 'baz'})
 
     def test_add_to_call_parameters_bad_json(self):
         parsed_args = mock.Mock()
         # Create a bad JSON input
         parsed_args.cli_input_json = self.input_json + ','
-        parsed_globals = mock.Mock()
         call_parameters = {}
         with self.assertRaises(ParamError):
             self.argument.add_to_call_parameters(
                 call_parameters=call_parameters,
-                parsed_args=parsed_args,
-                parsed_globals=parsed_globals
+                parsed_args=parsed_args
             )
 
     def test_add_to_call_parameters_no_clobber(self):
         parsed_args = mock.Mock()
         parsed_args.cli_input_json = self.input_json
-        parsed_globals = mock.Mock()
         # The value for ``A`` should not be clobbered by the input JSON
         call_parameters = {'A': 'baz'}
         self.argument.add_to_call_parameters(
             call_parameters=call_parameters,
-            parsed_args=parsed_args,
-            parsed_globals=parsed_globals
+            parsed_args=parsed_args
         )
         self.assertEqual(call_parameters, {'A': 'baz', 'B': 'bar'})
 
     def test_no_add_to_call_parameters(self):
         parsed_args = mock.Mock()
         parsed_args.cli_input_json = None
-        parsed_globals = mock.Mock()
         call_parameters = {'A': 'baz'}
         self.argument.add_to_call_parameters(
             call_parameters=call_parameters,
-            parsed_args=parsed_args,
-            parsed_globals=parsed_globals
+            parsed_args=parsed_args
         )
         # Nothing should have been added to the call parameters because
         # ``cli_input_json`` is not in the ``parsed_args``
         self.assertEqual(call_parameters, {'A': 'baz'})
```

### Comparing `cdpcli-0.9.89/tests/unit/extensions/test_generatecliskeleton.py` & `cdpcli-0.9.9/tests/unit/extensions/test_generatecliskeleton.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.89/tests/unit/extensions/test_paginate.py` & `cdpcli-0.9.9/tests/unit/extensions/test_paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.89/tests/unit/extensions/test_writer.py` & `cdpcli-0.9.9/tests/unit/extensions/test_writer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.89/tests/unit/test_argparser.py` & `cdpcli-0.9.9/tests/unit/test_argparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # Copyright (c) 2016 Cloudera, Inc. All rights reserved.
 
 import os
 
 from cdpcli.argparser import ArgTableArgParser
 from cdpcli.argparser import ServiceArgParser
-from cdpcli.clidriver import CLIDriver, ServiceOperation
+from cdpcli.clidriver import ServiceOperation
 from cdpcli.model import ServiceModel
-from mock import Mock
 from tests import unittest
 import yaml
 
 MODEL_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)),
                          'argparser')
 TEST_ARGS = ['submit-spark-job',
              '--jars',
@@ -43,15 +42,14 @@
 class TestArgTableArgParser(unittest.TestCase):
 
     def setUp(self):
         self.args = TEST_ARGS[1:]
         model = yaml.safe_load(open(os.path.join(MODEL_DIR, 'service.yaml')))
         service_model = ServiceModel(model, 'servicename')
         service_operation = ServiceOperation(
-            Mock(spec=CLIDriver),
             'submit-spark-job',
             'dataeng',
             '',
             service_model.operation_model('submitSparkJob'))
         self.parser = ArgTableArgParser(service_operation.arg_table)
 
     def testArsParsedCorrectly(self):
```

### Comparing `cdpcli-0.9.89/tests/unit/test_auth.py` & `cdpcli-0.9.9/tests/unit/test_auth.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,32 +21,27 @@
 from cdpcli.compat import HTTPHeaders
 from cdpcli.compat import json
 from cdpcli.compat import urlsplit
 import cdpcli.credentials
 from cdpcli.exceptions import NoCredentialsError
 import mock
 from tests import unittest
-from tests.unit import ECDSA_KEY, ED25519_KEY, RSA_KEY
+from tests.unit import ED25519_KEY, RSA_KEY
 
 
 EXPECTED_RSA_SIG = \
     'VLlOczaMiHdAHfW7-0axYWAxpFPqHR2sR22XRh98AlVTBjj8QJTModpzNUQxb1N0F94pMP6U' \
     'BI-flm-rl3vHJaRBfcWbaDglD02YcuqD87CmOIpZ6Z3TUTbkOcxTsMSkgOaPqQkO1p49WRl3' \
     'P_v3Q9z5y6Mh7ZDbQeonQcagKhoIYQnCXYrEmAAHhTGwuxanuAsPu2y8svUBKNd9fXZ7stQ0' \
     'Pom2J2aQZnegBM6I_QJICP7ZEd0Roga0AcGoL1OsZo_fANkUV9eUvtw8CfTw11G2c1YS__pq' \
     'PVuW4iPSYONoUN5NrL6x3RtGOea0Xo__9B5ki0_TLsYMyhF37it6qA=='
 
 EXPECTED_ED25519_SIG = \
     'et_Ueu_w3QuQbqvDdwy9aT8HLzsXBdJfRRRHe4fEK_RZ-qR-xvM35XG8J8q-YMz70GunK82JoSt5ztz0lAuCBg=='  # noqa
 
-EXPECTED_ECDSA_SIG = \
-    'MIGIAkIBPOgngVp4-uyWzLTCKcsCBeYezoedjN-Tj2KI78aIn6huJEJwG-6ZiVcEyO-mI1wN' \
-    'tbVu7H-iQDMPFKyBdpezjxYCQgEY32q1WTQUPHj_JNYN33QhCMPjJHIaBcHTdMp0SO3iVzLD' \
-    'Xi1MmHoMGsIYnUq3Q8Y1Z5JiyFr0NO6XzfnrF_OYCQ=='
-
 
 class BaseTestWithFixedDate(unittest.TestCase):
     def setUp(self):
         self.datetime_patch = mock.patch('cdpcli.auth.datetime')
         self.datetime_mock = self.datetime_patch.start()
         self.fixed_date = datetime.datetime(2014, 3, 10, 17, 2, 55, 0)
         self.datetime_mock.datetime.utcnow.return_value = self.fixed_date
@@ -65,17 +60,17 @@
 
 class TestRSAV1(unittest.TestCase):
     maxDiff = None
 
     def setUp(self):
         access_key_id = 'ABCD-EFGH-IJKL-MNOP-QRST'
         self.credentials = cdpcli.credentials.Credentials(
-            access_key_id=access_key_id,
-            private_key=RSA_KEY,
-            method='test')
+            access_key_id,
+            RSA_KEY,
+            'test')
         self.rsav1 = cdpcli.auth.RSAv1Auth(self.credentials)
         self.date_mock = mock.patch('cdpcli.auth.formatdate')
         self.formatdate = self.date_mock.start()
         self.formatdate.return_value = 'Thu, 17 Nov 2005 18:49:58 GMT'
 
     def tearDown(self):
         self.date_mock.stop()
@@ -160,17 +155,17 @@
     """
     We're not retesting aspects that are identical to what RSA tests cover
     """
 
     def setUp(self):
         access_key_id = 'ABCD-EFGH-IJKL-MNOP-QRST'
         self.credentials = cdpcli.credentials.Credentials(
-            access_key_id=access_key_id,
-            private_key=ED25519_KEY,
-            method='test')
+            access_key_id,
+            ED25519_KEY,
+            'test')
         self.ed25519v1 = cdpcli.auth.Ed25519v1Auth(self.credentials)
         self.date_mock = mock.patch('cdpcli.auth.formatdate')
         self.formatdate = self.date_mock.start()
         self.formatdate.return_value = 'Thu, 17 Nov 2005 18:49:58 GMT'
 
     def tearDown(self):
         self.date_mock.stop()
@@ -204,86 +199,7 @@
 
         json_metadata = json.loads(
             urlsafe_b64decode(metadata.encode('utf-8')).decode('utf-8'))
         self.assertEqual(self.credentials.access_key_id,
                          json_metadata['access_key_id'])
         self.assertEqual("ed25519v1",
                          json_metadata['auth_method'])
-
-
-class TestECDSAV1(unittest.TestCase):
-    """
-    We're not retesting aspects that are identical to what RSA tests cover
-    """
-
-    def setUp(self):
-        access_key_id = 'ABCD-EFGH-IJKL-MNOP-QRST'
-        self.credentials = cdpcli.credentials.Credentials(
-            access_key_id=access_key_id,
-            private_key=ECDSA_KEY,
-            method='test')
-        self.ecdsav1 = cdpcli.auth.ECDSAv1Auth(self.credentials)
-        self.date_mock = mock.patch('cdpcli.auth.formatdate')
-        self.formatdate = self.date_mock.start()
-        self.formatdate.return_value = 'Thu, 17 Nov 2005 18:49:58 GMT'
-
-    def tearDown(self):
-        self.date_mock.stop()
-
-    def test_no_credentials_raises_error(self):
-        ecdsav1 = cdpcli.auth.ECDSAv1Auth(None)
-        with self.assertRaises(NoCredentialsError):
-            ecdsav1.add_auth("pass someting")
-
-    def test_put(self):
-        http_headers = HTTPHeaders.from_dict({})
-        split = urlsplit('/foo/bar')
-        cs = self.ecdsav1._canonical_string('PUT', split, http_headers)
-        expected_canonical = "PUT\n\nThu, 17 Nov 2005 18:49:58 GMT\n/foo/bar\necdsav1"
-        self.assertEqual(expected_canonical, cs)
-        sig = self.ecdsav1._get_signature('PUT', split, HTTPHeaders.from_dict({}))
-        self.assertEqual(EXPECTED_ECDSA_SIG, sig)
-
-    def test_auth_header_string(self):
-        http_headers = HTTPHeaders.from_dict({})
-        split = urlsplit('/foo/bar')
-        sig = self.ecdsav1._get_signature('PUT', split, http_headers)
-        self.assertEqual(EXPECTED_ECDSA_SIG, sig)
-
-        auth_header_string = self.ecdsav1._get_signature_header(sig)
-        expected_metadata = 'eyJhY2Nlc3Nfa2V5X2lkIjogIkFCQ0QtRUZHSC1JSktMLU1O' \
-                            'T1AtUVJTVCIsICJhdXRoX21ldGhvZCI6ICJlY2RzYXYxIn0='
-        metadata, sig = auth_header_string.split(".")
-        self.assertEqual(expected_metadata, metadata)
-        self.assertEqual(EXPECTED_ECDSA_SIG, sig)
-
-        json_metadata = json.loads(
-            urlsafe_b64decode(metadata.encode('utf-8')).decode('utf-8'))
-        self.assertEqual(self.credentials.access_key_id, json_metadata['access_key_id'])
-        self.assertEqual("ecdsav1", json_metadata['auth_method'])
-
-
-class TestAccessToken(unittest.TestCase):
-    def test_no_credentials_raises_error(self):
-        access_token_auth = cdpcli.auth.AccessTokenAuth(None)
-        with self.assertRaises(NoCredentialsError):
-            access_token_auth.add_auth("pass something")
-
-    def test_auth_header_string(self):
-        access_token = 'Bearer ABC.DEF'
-        credentials = cdpcli.credentials.Credentials(
-            access_token=access_token,
-            method='test')
-        access_token_auth = cdpcli.auth.AccessTokenAuth(credentials)
-
-        request = CdpRequest()
-        request.headers['Content-Type'] = 'text/html'
-        request.method = 'PUT'
-        request.url = 'https://altus.cloudera.com/service/op'
-
-        access_token_auth.add_auth(request)
-        self.assertEqual(request.headers['Authorization'], access_token)
-
-    def test_is_access_token(self):
-        self.assertFalse(cdpcli.auth.AccessTokenAuth.is_access_token(None))
-        self.assertFalse(cdpcli.auth.AccessTokenAuth.is_access_token(''))
-        self.assertTrue(cdpcli.auth.AccessTokenAuth.is_access_token('Bearer A.B'))
```

### Comparing `cdpcli-0.9.89/tests/unit/test_client.py` & `cdpcli-0.9.9/tests/unit/test_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,270 +1,350 @@
-# Copyright 2012-2013 Amazon.com, Inc. or its affiliates. All Rights Reserved.
+# Copyright 2012-2014 Amazon.com, Inc. or its affiliates. All Rights Reserved.
 #
 # Modifications made by Cloudera are:
 #     Copyright (c) 2016 Cloudera, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"). You
 # may not use this file except in compliance with the License. A copy of
 # the License is located at
 #
-#     http://aws.amazon.com/apache2.0/
+# http://aws.amazon.com/apache2.0/
 #
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
-import os
+import datetime
 
-from cdpcli.client import ClientCreator
-from cdpcli.exceptions import ClientError
-from cdpcli.exceptions import OperationNotPageableError
-from cdpcli.exceptions import ParamValidationError
-from cdpcli.parser import ResponseParserFactory
-from mock import Mock
+from cdpcli import OBJECT_TYPE
+from cdpcli import xform_name
+from cdpcli.model import DenormalizedStructureBuilder
+from cdpcli.model import ServiceModel
+from cdpcli.utils import ArgumentGenerator
+from cdpcli.utils import CachedProperty
+from cdpcli.utils import datetime2timestamp
+from cdpcli.utils import get_service_module_name
+from cdpcli.utils import instance_cache
+from cdpcli.utils import parse_timestamp
+from cdpcli.utils import parse_to_aware_datetime
+from dateutil.tz import tzoffset, tzutc
 from tests import unittest
-from tests.unit import FakeContext
-import yaml
 
 
-USE_DEFAULT_ENDPOINT_URL = None
-DEFAULT_REGION = 'us-west-1'
-VERIFY_TLS = True
-CLIENT_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'client')
+class TestTransformName(unittest.TestCase):
+    def test_upper_camel_case(self):
+        self.assertEqual(xform_name('UpperCamelCase'), 'upper_camel_case')
+        self.assertEqual(xform_name('UpperCamelCase', '-'), 'upper-camel-case')
+
+    def test_lower_camel_case(self):
+        self.assertEqual(xform_name('lowerCamelCase'), 'lower_camel_case')
+        self.assertEqual(xform_name('lowerCamelCase', '-'), 'lower-camel-case')
+
+    def test_consecutive_upper_case(self):
+        self.assertEqual(xform_name('HTTPHeaders'), 'http_headers')
+        self.assertEqual(xform_name('HTTPHeaders', '-'), 'http-headers')
+
+    def test_consecutive_upper_case_middle_string(self):
+        self.assertEqual(xform_name('MainHTTPHeaders'), 'main_http_headers')
+        self.assertEqual(xform_name('MainHTTPHeaders', '-'), 'main-http-headers')
+
+    def test_s3_prefix(self):
+        self.assertEqual(xform_name('S3BucketName'), 's3_bucket_name')
+
+    def test_already_snake_cased(self):
+        self.assertEqual(xform_name('leave_alone'), 'leave_alone')
+        self.assertEqual(xform_name('s3_bucket_name'), 's3_bucket_name')
+        self.assertEqual(xform_name('bucket_s3_name'), 'bucket_s3_name')
+
+    def test_special_case_ends_with_s(self):
+        self.assertEqual(xform_name('GatewayCRNs', '-'), 'gateway-crns')
+
+
+class TestParseTimestamps(unittest.TestCase):
+    def test_parse_iso8601(self):
+        self.assertEqual(
+            parse_timestamp('1970-01-01T00:10:00.000Z'),
+            datetime.datetime(1970, 1, 1, 0, 10, tzinfo=tzutc()))
+
+    def test_parse_epoch(self):
+        self.assertEqual(
+            parse_timestamp(1222172800),
+            datetime.datetime(2008, 9, 23, 12, 26, 40, tzinfo=tzutc()))
+
+    def test_parse_epoch_zero_time(self):
+        self.assertEqual(
+            parse_timestamp(0),
+            datetime.datetime(1970, 1, 1, 0, 0, 0, tzinfo=tzutc()))
+
+    def test_parse_epoch_as_string(self):
+        self.assertEqual(
+            parse_timestamp('1222172800'),
+            datetime.datetime(2008, 9, 23, 12, 26, 40, tzinfo=tzutc()))
+
+    def test_parse_rfc822(self):
+        self.assertEqual(
+            parse_timestamp('Wed, 02 Oct 2002 13:00:00 GMT'),
+            datetime.datetime(2002, 10, 2, 13, 0, tzinfo=tzutc()))
+
+    def test_parse_invalid_timestamp(self):
+        with self.assertRaises(ValueError):
+            parse_timestamp('invalid date')
+
+
+class TestDatetime2Timestamp(unittest.TestCase):
+    def test_datetime2timestamp_naive(self):
+        self.assertEqual(
+            datetime2timestamp(datetime.datetime(1970, 1, 2)), 86400)
+
+    def test_datetime2timestamp_aware(self):
+        tzinfo = tzoffset("BRST", -10800)
+        self.assertEqual(
+            datetime2timestamp(datetime.datetime(1970, 1, 2, tzinfo=tzinfo)),
+            97200)
+
+
+class TestParseToUTCDatetime(unittest.TestCase):
+    def test_handles_utc_time(self):
+        original = datetime.datetime(1970, 1, 1, 0, 0, 0, tzinfo=tzutc())
+        self.assertEqual(parse_to_aware_datetime(original), original)
+
+    def test_handles_other_timezone(self):
+        tzinfo = tzoffset("BRST", -10800)
+        original = datetime.datetime(2014, 1, 1, 0, 0, 0, tzinfo=tzinfo)
+        self.assertEqual(parse_to_aware_datetime(original), original)
+
+    def test_handles_naive_datetime(self):
+        original = datetime.datetime(1970, 1, 1, 0, 0, 0)
+        expected = datetime.datetime(1970, 1, 1, 0, 0, 0, tzinfo=tzutc())
+        self.assertEqual(parse_to_aware_datetime(original), expected)
+
+    def test_handles_string_epoch(self):
+        expected = datetime.datetime(1970, 1, 1, 0, 0, 0, tzinfo=tzutc())
+        self.assertEqual(parse_to_aware_datetime('0'), expected)
+
+    def test_handles_int_epoch(self):
+        expected = datetime.datetime(1970, 1, 1, 0, 0, 0, tzinfo=tzutc())
+        self.assertEqual(parse_to_aware_datetime(0), expected)
+
+    def test_handles_full_iso_8601(self):
+        expected = datetime.datetime(1970, 1, 1, 0, 0, 0, tzinfo=tzutc())
+        self.assertEqual(
+            parse_to_aware_datetime('1970-01-01T00:00:00Z'),
+            expected)
+
+    def test_year_only_iso_8601(self):
+        expected = datetime.datetime(1970, 1, 1, 0, 0, 0, tzinfo=tzutc())
+        self.assertEqual(parse_to_aware_datetime('1970-01-01'), expected)
+
+
+class TestCachedProperty(unittest.TestCase):
+    def test_cached_property_same_value(self):
+        class CacheMe(object):
+            @CachedProperty
+            def foo(self):
+                return 'foo'
+
+        c = CacheMe()
+        self.assertEqual(c.foo, 'foo')
+        self.assertEqual(c.foo, 'foo')
+
+    def test_cached_property_only_called_once(self):
+        # Note: you would normally never want to cache
+        # a property that returns a new value each time,
+        # but this is done to demonstrate the caching behavior.
+
+        class NoIncrement(object):
+            def __init__(self):
+                self.counter = 0
+
+            @CachedProperty
+            def current_value(self):
+                self.counter += 1
+                return self.counter
+
+        c = NoIncrement()
+        self.assertEqual(c.current_value, 1)
+        # If the property wasn't cached, the next value should be
+        # be 2, but because it's cached, we know the value will be 1.
+        self.assertEqual(c.current_value, 1)
 
 
-class TestClient(unittest.TestCase):
+class TestArgumentGenerator(unittest.TestCase):
+    def setUp(self):
+        self.arg_generator = ArgumentGenerator()
+
+    def assert_skeleton_from_model_is(self, model, generated_skeleton):
+        shape = DenormalizedStructureBuilder().with_members(
+            model).build_model()
+        actual = self.arg_generator.generate_skeleton(shape)
+        self.assertEqual(actual, generated_skeleton)
+
+    def test_generate_string(self):
+        self.assert_skeleton_from_model_is(
+            model={
+                'A': {'type': 'string'}
+            },
+            generated_skeleton={
+                'A': ''
+            }
+        )
+
+    def test_generate_scalars(self):
+        self.assert_skeleton_from_model_is(
+            model={
+                'A': {'type': 'string'},
+                'B': {'type': 'integer'},
+                'C': {'type': 'float'},
+                'D': {'type': 'double'},
+                'E': {'type': 'boolean'},
+                'F': {'type': 'datetime'}
+            },
+            generated_skeleton={
+                'A': '',
+                'B': 0,
+                'C': 0.0,
+                'D': 0.0,
+                'E': True,
+                'F': '2002-10-02T13:00:00+00:00'
+            }
+        )
+
+    def test_generate_nested_objects(self):
+        self.assert_skeleton_from_model_is(
+            model={
+                'A': {
+                    'type': OBJECT_TYPE,
+                    'properties': {
+                        'B': {'type': 'string'},
+                    }
+                }
+            },
+            generated_skeleton={
+                'A': {'B': ''}
+            }
+        )
+
+    def test_generate_scalar_list(self):
+        self.assert_skeleton_from_model_is(
+            model={
+                'A': {
+                    'type': 'array',
+                    'items': {
+                        'type': 'string'
+                    }
+                },
+            },
+            generated_skeleton={
+                'A': [''],
+            }
+        )
+
+    def test_generate_scalar_map(self):
+        self.assert_skeleton_from_model_is(
+            model={
+                'A': {
+                    'type': 'object',
+                    'additionalProperties': {
+                        'type': 'string'
+                    }
+                }
+            },
+            generated_skeleton={
+                'A': {
+                    'KeyName': '',
+                }
+            }
+        )
+
+
+class TestInstanceCache(unittest.TestCase):
+    class DummyClass(object):
+        def __init__(self, cache):
+            self._instance_cache = cache
+
+        @instance_cache
+        def add(self, x, y):
+            return x + y
+
+        @instance_cache
+        def sub(self, x, y):
+            return x - y
+
+    def setUp(self):
+        self.cache = {}
 
+    def test_cache_single_method_call(self):
+        adder = self.DummyClass(self.cache)
+        self.assertEqual(adder.add(2, 1), 3)
+        # This should result in one entry in the cache.
+        self.assertEqual(len(self.cache), 1)
+        # When we call the method with the same args,
+        # we should reuse the same entry in the cache.
+        self.assertEqual(adder.add(2, 1), 3)
+        self.assertEqual(len(self.cache), 1)
+
+    def test_can_cache_multiple_methods(self):
+        adder = self.DummyClass(self.cache)
+        adder.add(2, 1)
+
+        # A different method results in a new cache entry,
+        # so now there should be two elements in the cache.
+        self.assertEqual(adder.sub(2, 1), 1)
+        self.assertEqual(len(self.cache), 2)
+        self.assertEqual(adder.sub(2, 1), 1)
+
+    def test_can_cache_kwargs(self):
+        adder = self.DummyClass(self.cache)
+        adder.add(x=2, y=1)
+        self.assertEqual(adder.add(x=2, y=1), 3)
+        self.assertEqual(len(self.cache), 1)
+
+
+class TestGetServiceModuleName(unittest.TestCase):
     def setUp(self):
-        self.loader = Mock()
-        self.loader.load_service_data.return_value = yaml.safe_load(
-            open(os.path.join(CLIENT_DIR, 'service.yaml')))
-        self.endpoint = Mock()
-        self.endpoint.host = 'http://thunderhead.cloudera.altus.cloudera.com'
-        self.endpoint.make_request.return_value = (Mock(status_code=200), {})
-
-        self.endpoint_creator = Mock()
-        self.endpoint_creator.create_endpoint.return_value = self.endpoint
-        self.retryhandler = Mock()
-        self.context = FakeContext({})
-        self.client_creator = ClientCreator(self.loader,
-                                            self.context,
-                                            self.endpoint_creator,
-                                            'user-agent-header',
-                                            ResponseParserFactory(),
-                                            self.retryhandler)
-        self.credentials = Mock()
-        self.credentials.private_key = "A Private Key"
-
-    def _create_client(self):
-        return self.client_creator.create_client(
-            'thunderhead', USE_DEFAULT_ENDPOINT_URL, DEFAULT_REGION,
-            VERIFY_TLS, self.credentials)
-
-    def _get_request_params(self):
-        self.assertTrue(self.endpoint.make_request.called)
-        return dict((k.lower(), v) for k, v in
-                    self.endpoint.make_request.call_args[0][1].items())
-
-    def test_client_name(self):
-        client = self._create_client()
-        self.assertEquals(client.__class__.__name__, 'thunderhead')
-
-    def test_client_meta(self):
-        client = self._create_client()
-        self.assertTrue(client.meta is not None)
-        self.assertTrue(client.meta.service_model is not None)
-        self.assertEquals(client.meta.endpoint_url,
-                          'http://thunderhead.cloudera.altus.cloudera.com')
-
-    def test_client_operations(self):
-        client = self._create_client()
-        self.assertTrue(hasattr(client, 'create_director'))
-        self.assertFalse(hasattr(client, 'non_existent_operation'))
-
-    def test_client_method_to_api_mapping(self):
-        client = self._create_client()
-        self.assertEqual(client.meta.method_to_api_mapping['create_director'],
-                         'createDirector')
-
-    def test_client_call(self):
-        client = self._create_client()
-        response = client.describe_directors()
-        self.assertTrue(self.endpoint.make_request.called)
-        self.assertEqual(response, {})
-
-    def test_get_paginator(self):
-        client = self._create_client()
-        self.assertTrue(client.get_paginator('describe_directors') is not None)
-        with self.assertRaises(OperationNotPageableError):
-            client.get_paginator('create_director')
-
-    def test_client_user_agent_in_request(self):
-        client = self._create_client()
-        client.describe_directors()
-        self.assertTrue(self.endpoint.make_request.called)
-        params = self._get_request_params()
-        self.assertEqual(params['headers']['User-Agent'], 'user-agent-header')
-
-    def test_additional_headers_not_in_request_by_default(self):
-        client = self._create_client()
-        client.describe_directors()
-        self.assertTrue(self.endpoint.make_request.called)
-        params = self._get_request_params()
-        self.assertEquals(2, len(params['headers']))
-
-    def test_additional_headers_from_config(self):
-        self.context.config['request_headers'] = \
-            'x-test-1=crn:altus:iam,x-test-2=generate::uuid'
-        client = self._create_client()
-        client.describe_directors()
-        self.assertTrue(self.endpoint.make_request.called)
-        params = self._get_request_params()
-        self.assertEquals('crn:altus:iam', params['headers']['x-test-1'])
-        self.assertTrue('x-test-2' in params['headers'])
-        self.assertNotEquals('generate::uuid', params['headers']['x-test-2'])
-
-    def test_client_error_message_for_positional_args(self):
-        client = self._create_client()
-        with self.assertRaisesRegexp(TypeError, 'only accepts keyword arguments'):
-            client.create_director('foo')
-
-    def test_client_error(self):
-        client = self._create_client()
-        error = {'error': {'code': 'test-code', 'message': 'test-message'}}
-        mock_response = Mock(
-            status_code=400,
-            headers={'x-altus-request-id': '00000000-0000-0000-0000-000000000000'})
-        self.endpoint.make_request.return_value = (mock_response, error)
-        re = (
-            'An error occurred: test-message '
-            '\\(Status Code: 400; '
-            'Error Code: test-code; '
-            'Service: thunderhead; '
-            'Operation: describeDirectors; '
-            'Request ID: 00000000-0000-0000-0000-000000000000;\\)')
-        with self.assertRaisesRegexp(ClientError, re) as e:
-            client.describe_directors()
-        self.assertEqual(e.exception.response['error']['code'], 'test-code')
-        self.assertEqual(e.exception.response['error']['message'], 'test-message')
-
-    def test_client_error_cdp_request_id(self):
-        client = self._create_client()
-        error = {'error': {'code': 'test-code', 'message': 'test-message'}}
-        mock_response = Mock(
-            status_code=400,
-            headers={'x-cdp-request-id': '0000000a-0000-0000-0000-000000000001'})
-        self.endpoint.make_request.return_value = (mock_response, error)
-        re = 'Request ID: 0000000a-0000-0000-0000-000000000001;'
-        with self.assertRaisesRegexp(ClientError, re):
-            client.describe_directors()
-
-    def test_client_validates_params(self):
-        client = self._create_client()
-        with self.assertRaises(ParamValidationError):
-            client.create_director()
-
-    def test_operation_cannot_paginate(self):
-        client = self._create_client()
-        self.assertTrue(hasattr(client, 'create_director'))
-        self.assertFalse(client.can_paginate('create_director'))
-
-    def test_operation_can_paginate(self):
-        client = self._create_client()
-        self.assertTrue(hasattr(client, 'describe_directors'))
-        self.assertTrue(client.can_paginate('describe_directors'))
-
-    def test_make_request(self):
-        client = self._create_client()
-        response = {'foo': 'bar'}
-        self.endpoint.make_request.return_value = (Mock(status_code=200), response)
-        http, parsed_response = client.make_request('describeDirectors',
-                                                    'post',
-                                                    '/directors/describeDirectors',
-                                                    {'test': 'value'},
-                                                    b'body')
-        self.assertTrue(self.endpoint.make_request.called)
-        params = self._get_request_params()
-        self.assertEquals('post', params['method'])
-        self.assertEquals('/directors/describeDirectors', params['url_path'])
-        self.assertEquals(
-            'http://thunderhead.cloudera.altus.cloudera.com/directors/describeDirectors',
-            params['url'])
-        self.assertEquals('value', params['headers']['test'])
-        self.assertEquals(b'body', params['body'])
-        kwargs = self.endpoint.make_request.call_args[1]
-        self.assertEquals({'allow_redirects': True}, kwargs)
-        self.assertEquals(200, http.status_code)
-        self.assertEquals(response, parsed_response)
-
-    def test_make_request_get_request(self):
-        client = self._create_client()
-        client.make_request('describeDirectors', 'get', '/get_request_path', {}, None)
-        self.assertTrue(self.endpoint.make_request.called)
-        params = self._get_request_params()
-        self.assertEquals('get', params['method'])
-        self.assertEquals('/get_request_path', params['url_path'])
-        self.assertIsNone(params['body'])
-
-    def test_make_request_absolute_url(self):
-        client = self._create_client()
-        client.make_request('describeDirectors', 'post', 'https://host/path', {}, None)
-        self.assertTrue(self.endpoint.make_request.called)
-        params = self._get_request_params()
-        self.assertEquals('post', params['method'])
-        self.assertEquals('https://host/path', params['url_path'])
-
-    def test_make_request_no_redirects(self):
-        client = self._create_client()
-        client.make_request('describeDirectors', 'post', '/path', {}, None,
-                            allow_redirects=False)
-        self.assertTrue(self.endpoint.make_request.called)
-        kwargs = self.endpoint.make_request.call_args[1]
-        self.assertEquals({'allow_redirects': False}, kwargs)
-
-    def test_make_request_error_with_no_redirects(self):
-        client = self._create_client()
-        error = {'error': {'code': 'test-code', 'message': 'test-message'}}
-        mock_response = Mock(
-            status_code=400,
-            headers={'x-altus-request-id': '00000000-0000-0000-0000-000000000000'})
-        self.endpoint.make_request.return_value = (mock_response, error)
-        re = (
-            'An error occurred: test-message '
-            '\\(Status Code: 400; '
-            'Error Code: test-code; '
-            'Service: thunderhead; '
-            'Operation: describeDirectors; '
-            'Request ID: 00000000-0000-0000-0000-000000000000;\\)')
-        with self.assertRaisesRegexp(ClientError, re) as e:
-            client.make_request('describeDirectors',
-                                'post',
-                                '/directors/describeDirectors',
-                                {},
-                                None,
-                                allow_redirects=False)
-        self.assertEqual(e.exception.response['error']['code'], 'test-code')
-        self.assertEqual(e.exception.response['error']['message'], 'test-message')
-
-    def test_make_request_error(self):
-        client = self._create_client()
-        error = {'error': {'code': 'test-code', 'message': 'test-message'}}
-        mock_response = Mock(
-            status_code=400,
-            headers={'x-altus-request-id': '00000000-0000-0000-0000-000000000000'})
-        self.endpoint.make_request.return_value = (mock_response, error)
-        re = (
-            'An error occurred: test-message '
-            '\\(Status Code: 400; '
-            'Error Code: test-code; '
-            'Service: thunderhead; '
-            'Operation: describeDirectors; '
-            'Request ID: 00000000-0000-0000-0000-000000000000;\\)')
-        with self.assertRaisesRegexp(ClientError, re) as e:
-            client.make_request('describeDirectors',
-                                'post',
-                                '/directors/describeDirectors',
-                                {},
-                                None)
-        self.assertEqual(e.exception.response['error']['code'], 'test-code')
-        self.assertEqual(e.exception.response['error']['message'], 'test-message')
+        self.service_description = {
+            'metadata': {
+                'serviceFullName': 'CDP MyService',
+                'apiVersion': '2014-01-01',
+                'endpointPrefix': 'myservice',
+                'signatureVersion': 'v4',
+                'protocol': 'query'
+            },
+            'operations': {},
+            'shapes': {},
+        }
+        self.service_model = ServiceModel(
+            self.service_description, 'myservice')
+
+    def test_default(self):
+        self.assertEqual(
+            get_service_module_name(self.service_model),
+            'myservice'
+        )
+
+    def test_client_name_with_cloudera(self):
+        self.service_description['metadata']['serviceFullName'] = (
+            'Cloudera MyService')
+        self.assertEqual(
+            get_service_module_name(self.service_model),
+            'myservice'
+        )
+
+    def test_client_name_with_non_alphabet_characters(self):
+        self.service_description['metadata']['serviceFullName'] = (
+            'Cloudera My-Service')
+        self.assertEqual(
+            get_service_module_name(self.service_model),
+            'myservice'
+        )
+
+    def test_client_name_with_no_full_name_or_abbreviation(self):
+        del self.service_description['metadata']['serviceFullName']
+        self.assertEqual(
+            get_service_module_name(self.service_model),
+            'myservice'
+        )
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `cdpcli-0.9.89/tests/unit/test_completer.py` & `cdpcli-0.9.9/tests/unit/test_completer.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,49 +98,14 @@
             },
             'arguments': []
         }
         completer = Completer(
             self.clidriver_creator.create_clidriver(commands))
         self.assert_completion(completer, 'cdp bin', [])
 
-    def test_complete_cli_enum_options(self):
-        commands = {
-            'subcommands': {},
-            'arguments': ['version', 'output', 'color']
-        }
-        clidriver = self.clidriver_creator.create_clidriver(commands)
-        clidriver._cli_data = {
-            "options": {
-                "version": {
-                    "action": "version",
-                    "help": "<p>Display the version of this tool.</p>"
-                },
-                "output": {
-                    "choices": [
-                        "json",
-                        "text",
-                        "table"
-                    ],
-                    "help": "<p>The formatting style for command output.</p>"
-                },
-                "color": {
-                    "choices": [
-                        "on",
-                        "off",
-                        "auto"
-                    ],
-                    "default": "auto",
-                    "help": "<p>Turn on/off color output.</p>"
-                }
-            }
-        }
-        completer = Completer(clidriver)
-        self.assert_completion(completer, 'cdp --output ', ['json', 'text', 'table'])
-        self.assert_completion(completer, 'cdp --color ', ['on', 'off', 'auto'])
-
     def test_complete_top_level_args(self):
         commands = {
             'subcommands': {},
             'arguments': ['foo', 'bar']
         }
         completer = Completer(
             self.clidriver_creator.create_clidriver(commands))
@@ -324,15 +289,14 @@
         completer = Completer(
             self.clidriver_creator.create_clidriver(commands))
         self.assert_completion(completer, 'cdp ', ['foo'])
 
 
 class MockModel:
     is_hidden = False
-    is_deprecated = False
 
 
 class MockCLIDriverFactory(object):
     def create_clidriver(self, commands=None):
         clidriver = mock.Mock(spec=CLIDriver)
         clidriver._create_help_command.return_value = \
             self._create_top_level_help(clidriver, commands)
@@ -356,15 +320,15 @@
         service_command._service_model = {}
         service_command._command_table = command_table
         return service_command
 
     def _create_operation_command(self, clidriver, name, command):
         argument_table = self.create_argument_table(
             command.get('arguments', []))
-        operation = ServiceOperation(clidriver, name, 'parent', None, MockModel())
+        operation = ServiceOperation(name, 'parent', None, MockModel())
         operation._arg_table = argument_table
         return operation
 
     def create_command_table(self, clidriver, commands, command_creator):
         if not commands:
             return OrderedDict()
         command_table = OrderedDict()
```

### Comparing `cdpcli-0.9.89/tests/unit/test_credentials.py` & `cdpcli-0.9.9/tests/unit/test_credentials.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,46 +48,36 @@
     'private_key': raw_metadata['foobar']['PrivateKey'],
     'expiry_time': raw_metadata['foobar']['Expiration'],
 }
 context = Context()
 
 
 class TestCredentials(BaseEnvVar):
-    def _ensure_credential_is_normalized_as_unicode(self, access, secret, token):
-        c = credentials.Credentials(access_key_id=access,
-                                    private_key=secret,
-                                    access_token=token,
-                                    method='test')
+    def _ensure_credential_is_normalized_as_unicode(self, access, secret):
+        c = credentials.Credentials(access, secret, 'test')
         self.assertTrue(isinstance(c.access_key_id, type(u'u')))
         self.assertTrue(isinstance(c.private_key, type(u'u')))
-        self.assertTrue(isinstance(c.access_token, type(u'u')))
 
     def test_detect_nonascii_character(self):
         self._ensure_credential_is_normalized_as_unicode(
-            'foo\xe2\x80\x99', 'bar\xe2\x80\x99', 'tea\xe2\x80\x99')
+            'foo\xe2\x80\x99', 'bar\xe2\x80\x99')
 
     def test_unicode_input(self):
         self._ensure_credential_is_normalized_as_unicode(
-            u'foo', u'bar', u'tea')
+            u'foo', u'bar')
 
     def test_frozen_credentials(self):
-        cred = credentials.Credentials(access_key_id="key",
-                                       private_key="secret",
-                                       access_token='token',
-                                       method="test")
+        cred = credentials.Credentials("key", "secret", "test")
         frozen_creds = cred.get_frozen_credentials()
         self.assertEqual("key", frozen_creds.access_key_id)
         self.assertEqual("secret", frozen_creds.private_key)
-        self.assertEqual("token", frozen_creds.access_token)
         cred.access_key_id = "foobar"
         cred.private_key = "foo"
-        cred.access_token = "bar"
         self.assertEqual("key", frozen_creds.access_key_id)
         self.assertEqual("secret", frozen_creds.private_key)
-        self.assertEqual("token", frozen_creds.access_token)
 
 
 class TestBaseCredentialProvider(BaseEnvVar):
     def test_load(self):
         cred_provider = credentials.CredentialProvider()
         self.assertTrue(cred_provider.load())
 
@@ -112,24 +102,14 @@
         provider = credentials.EnvProvider(environ)
         creds = provider.load()
         self.assertIsNotNone(creds)
         self.assertEqual(creds.access_key_id, 'foo')
         self.assertEqual(creds.private_key, TestEnvVar.PEM)
         self.assertEqual(creds.method, 'env')
 
-    def test_envvars_are_found_access_token(self):
-        environ = {
-            'CDP_ACCESS_TOKEN': 'tea'
-        }
-        provider = credentials.EnvProvider(environ)
-        creds = provider.load()
-        self.assertIsNotNone(creds)
-        self.assertEqual(creds.access_token, 'tea')
-        self.assertEqual(creds.method, 'env')
-
     def test_envvars_not_found(self):
         provider = credentials.EnvProvider(environ={})
         cred = provider.load()
         self.assertTrue(cred is None)
 
     def test_can_override_env_var_mapping(self):
         # We can change the env var provider to
@@ -145,29 +125,14 @@
         provider = credentials.EnvProvider(
             environ, mapping
         )
         creds = provider.load()
         self.assertEqual(creds.access_key_id, 'foo')
         self.assertEqual(creds.private_key, TestEnvVar.PEM)
 
-    def test_can_override_env_var_mapping_access_token(self):
-        # We can change the env var provider to
-        # use our specified env var names.
-        environ = {
-            'FOO_ACCESS_token': 'foo'
-        }
-        mapping = {
-            'access_token': 'FOO_ACCESS_token'
-        }
-        provider = credentials.EnvProvider(
-            environ, mapping
-        )
-        creds = provider.load()
-        self.assertEqual(creds.access_token, 'foo')
-
     def test_can_override_partial_env_var_mapping(self):
         # Only changing the access key mapping.
         # The other 2 use the default values of
         # CDP_SECRET_ACCESS_KEY and CDP_SESSION_TOKEN
         # use our specified env var names.
         environ = {
             'FOO_ACCESS_KEY_ID': 'foo',
@@ -196,21 +161,14 @@
         # use our specified env var names.
         self.environ['CDP_ACCESS_KEY_ID'] = 'foo'
         self.environ['CDP_PRIVATE_KEY'] = self.pem_file
         creds = credentials.get_credentials(context)
         self.assertEqual(creds.access_key_id, 'foo')
         self.assertEqual(creds.private_key, TestEnvVar.PEM)
 
-    def test_credential_with_envprovider_access_token(self):
-        # We can change the env var provider to
-        # use our specified env var names.
-        self.environ['CDP_ACCESS_TOKEN'] = 'foo'
-        creds = credentials.get_credentials(context)
-        self.assertEqual(creds.access_token, 'foo')
-
     def test_raise_if_not_a_file(self):
         environ = {
             'CDP_ACCESS_KEY_ID': 'foo',
             'CDP_PRIVATE_KEY': self.pem_file + "dose_not_exist",
         }
         provider = credentials.EnvProvider(environ)
         with self.assertRaises(NoCredentialsError):
@@ -232,17 +190,15 @@
 class CredentialResolverTest(BaseEnvVar):
     def setUp(self):
         super(CredentialResolverTest, self).setUp()
         self.provider1 = mock.Mock()
         self.provider1.METHOD = 'provider1'
         self.provider2 = mock.Mock()
         self.provider2.METHOD = 'provider2'
-        self.fake_creds = credentials.Credentials(access_key_id='a',
-                                                  private_key='b',
-                                                  method='test')
+        self.fake_creds = credentials.Credentials('a', 'b', 'test')
 
     def test_load_credentials_single_provider(self):
         self.provider1.load.return_value = self.fake_creds
         resolver = credentials.CredentialResolver(providers=[self.provider1])
         creds = resolver.load_credentials()
         self.assertEqual(creds.access_key_id, 'a')
         self.assertEqual(creds.private_key, 'b')
@@ -289,17 +245,15 @@
         # Now, if we were to call resolver.load() now, provider2 would
         # win because it's returning a non None response.
         # However we can inject a new provider before provider2 to
         # override this process.
         # Providers can be added by the METHOD name of each provider.
         new_provider = mock.Mock()
         new_provider.METHOD = 'new_provider'
-        new_provider.load.return_value = credentials.Credentials(access_key_id='d',
-                                                                 private_key='e',
-                                                                 method='test')
+        new_provider.load.return_value = credentials.Credentials('d', 'e', 'test')
 
         resolver.insert_after('provider1', new_provider)
 
         creds = resolver.load_credentials()
         self.assertIsNotNone(creds)
 
         self.assertEqual(creds.access_key_id, 'd')
@@ -309,32 +263,28 @@
         # a non-None response.
         self.provider1.load.assert_called_with()
         self.assertTrue(not self.provider2.called)
 
     def test_inject_provider_before_existing(self):
         new_provider = mock.Mock()
         new_provider.METHOD = 'override'
-        new_provider.load.return_value = credentials.Credentials(access_key_id='x',
-                                                                 private_key='y',
-                                                                 method='test')
+        new_provider.load.return_value = credentials.Credentials('x', 'y', 'test')
 
         resolver = credentials.CredentialResolver(providers=[self.provider1,
                                                              self.provider2])
         resolver.insert_before(self.provider1.METHOD, new_provider)
         creds = resolver.load_credentials()
         self.assertEqual(creds.access_key_id, 'x')
         self.assertEqual(creds.private_key, 'y')
 
     def test_can_remove_providers(self):
-        self.provider1.load.return_value = credentials.Credentials(access_key_id='a',
-                                                                   private_key='b',
-                                                                   method='test')
-        self.provider2.load.return_value = credentials.Credentials(access_key_id='d',
-                                                                   private_key='e',
-                                                                   method='test')
+        self.provider1.load.return_value = credentials.Credentials(
+            'a', 'b', 'test')
+        self.provider2.load.return_value = credentials.Credentials(
+            'd', 'e', 'test')
         resolver = credentials.CredentialResolver(providers=[self.provider1,
                                                              self.provider2])
         resolver.remove('provider1')
         creds = resolver.load_credentials()
         self.assertIsNotNone(creds)
         self.assertEqual(creds.access_key_id, 'd')
         self.assertEqual(creds.private_key, 'e')
@@ -406,25 +356,14 @@
         provider = credentials.AuthConfigFile(self.conf_file)
         creds = provider.load()
         self.assertIsNotNone(creds)
         self.assertEqual(creds.access_key_id, 'key_id')
         self.assertEqual(creds.private_key, 'secret')
         self.assertEqual(creds.method, 'auth_config_file')
 
-    def test_config_is_found_access_token(self):
-        def validate(path):
-            provider = credentials.AuthConfigFile(path)
-            cred = provider.load()
-            self.assertIsNotNone(cred)
-            self.assertEqual(cred.access_token, 'Bearer A.B.C')
-            self.assertEqual(cred.method, 'auth_config_file')
-
-        conf = '{"access_token": "Bearer A.B.C"}'
-        _run_test(conf, validate)
-
     def test_config_not_found(self):
         with self.assertRaises(NoCredentialsError):
             provider = credentials.AuthConfigFile(
                 self.conf_file + "_does_not_exist")
             provider.load()
 
     def test_bad_json(self):
@@ -552,52 +491,7 @@
 
         conf = """
 [default]
 cdp_private_key = secret\\nwith\\na\\nfew\\nnewlines
 cdp_access_key_id = the_key
 """
         _run_test(conf, validate)
-
-    def test_credentials_file_access_token(self):
-        def validate(path):
-            provider = credentials.SharedCredentialProvider(
-                creds_filename=path, profile_name=DEFAULT_PROFILE_NAME)
-            creds = provider.load()
-            self.assertIsNotNone(creds)
-            self.assertEqual(creds.access_token, 'Bearer A.B.C')
-            self.assertEqual(creds.method, 'shared-credentials-file')
-
-        conf = """
-[default]
-cdp_access_token = Bearer A.B.C
-"""
-        _run_test(conf, validate)
-
-
-class TestParamsProvider(unittest.TestCase):
-    def test_no_param(self):
-        provider = credentials.ParamsProvider(None)
-        creds = provider.load()
-        self.assertIsNone(creds)
-
-    def test_no_access_token_param(self):
-        params = {}
-        provider = credentials.ParamsProvider(params)
-        creds = provider.load()
-        self.assertIsNone(creds)
-
-    def test_empty_access_token_param(self):
-        params = mock.Mock()
-        params.access_token = ''
-        provider = credentials.ParamsProvider(params)
-        creds = provider.load()
-        self.assertIsNone(creds)
-
-    def test_access_token_param(self):
-        access_token = 'Bearer A.B'
-        params = mock.Mock()
-        params.access_token = access_token
-        provider = credentials.ParamsProvider(params)
-        creds = provider.load()
-        self.assertIsNotNone(creds)
-        self.assertEqual(creds.access_token, access_token)
-        self.assertEqual(creds.method, 'params')
```

### Comparing `cdpcli-0.9.89/tests/unit/test_loaders.py` & `cdpcli-0.9.9/tests/unit/test_loaders.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.89/tests/unit/test_model.py` & `cdpcli-0.9.9/tests/unit/test_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,55 +42,33 @@
         service_model = ServiceModel(self.model, 'myservice')
         self.assertEqual(service_model.service_name, 'myservice')
 
     def test_products(self):
         service_model = ServiceModel(self.model, 'myservice')
         self.assertEqual(service_model.products, ['ALTUS'])
 
-    def test_form_factors(self):
-        service_model = ServiceModel(self.model, 'myservice')
-        self.assertEqual(service_model.form_factors, ['public', 'private'])
-
-    def test_endpoint_prefix(self):
-        service_model = ServiceModel(self.model, 'myservice')
-        self.assertEqual(service_model.endpoint_prefix, 'api')
-
     def test_operations(self):
         self.assertTrue(self.service_model.operation_model(
                 'createDirector') is not None)
         self.assertTrue(self.service_model.operation_model(
                 'deleteDirector') is not None)
         self.assertTrue(self.service_model.operation_model(
                 'describeDirectors') is not None)
-        self.assertTrue(self.service_model.operation_model(
-                'getDirectors') is not None)
         with self.assertRaises(OperationNotFoundError):
             self.service_model.operation_model('NonExistentOperation')
 
-    def test_multiple_operation_ids(self):
-        self.assertFalse(self.service_model.operation_model(
-                'describeDirectors').is_deprecated)
-        self.assertTrue(self.service_model.operation_model(
-                'getDirectors').is_deprecated)
-        self.assertEquals(self.service_model.operation_model(
-                'getDirectors').name, 'getDirectors')
-        self.assertEquals(
-                self.service_model.operation_model('getDirectors').http,
-                self.service_model.operation_model('describeDirectors').http)
-
     def test_documentation(self):
         self.assertTrue(self.service_model.documentation.startswith(
                 'Cloudera CDP Test Service Description'))
 
     def test_operation_names(self):
-        self.assertEquals(len(self.service_model.operation_names), 4)
+        self.assertEquals(len(self.service_model.operation_names), 3)
         self.assertTrue('createDirector' in self.service_model.operation_names)
         self.assertTrue('deleteDirector' in self.service_model.operation_names)
         self.assertTrue('describeDirectors' in self.service_model.operation_names)
-        self.assertTrue('getDirectors' in self.service_model.operation_names)
 
 
 class TestOperationModel(unittest.TestCase):
     def setUp(self):
         self.model = yaml.safe_load(open(os.path.join(MODEL_DIR, 'service.yaml')))
         self.service_model = ServiceModel(self.model, 'servicename')
 
@@ -106,20 +84,14 @@
         self.assertEqual(operation_model.paging_result, 'directors')
         operation_model = self.service_model.operation_model('createDirector')
         self.assertEqual(operation_model.can_paginate, False)
         self.assertEqual(operation_model.paging_input_token, None)
         self.assertEqual(operation_model.paging_output_token, None)
         self.assertEqual(operation_model.paging_result, None)
 
-    def test_form_factors(self):
-        operation_model = self.service_model.operation_model('describeDirectors')
-        self.assertIsNone(operation_model.form_factors)
-        operation_model = self.service_model.operation_model('deleteDirector')
-        self.assertEqual(operation_model.form_factors, ['public'])
-
     def test_operation_input(self):
         operation_model = self.service_model.operation_model('createDirector')
         self.assertEqual(operation_model.http['method'], 'post')
         self.assertEqual(operation_model.http['requestUri'], '/directors/createDirector')
         self.assertEqual(operation_model.input_shape.name, 'input')
         self.assertEqual(list(operation_model.input_shape.members), ['name'])
 
@@ -205,18 +177,18 @@
 
     def test_invalid_shape_type(self):
         with self.assertRaises(InvalidShapeError):
             self.resolver.get_shape_by_name('invalid', 'MissingShapeType')
         with self.assertRaises(InvalidShapeError):
             self.resolver.get_shape_by_name('invalid', 'InvalidShapeType')
 
-    def test_deprecated_param(self):
+    def test_undocumented_param(self):
         shape = self.resolver.get_shape_by_name('shape', 'UndocumentedParmTest')
-        self.assertEqual(shape.members['undocumentedParam'].is_deprecated, True)
-        self.assertEqual(shape.members['documentedParam'].is_deprecated, False)
+        self.assertEqual(shape.members['undocumentedParam'].is_undocumented, True)
+        self.assertEqual(shape.members['documentedParam'].is_undocumented, False)
 
     def test_referenced_map(self):
         shape = self.resolver.get_shape_by_name('shape', 'ReferencedMapTest')
         self.assertEqual(shape.members['endpoints'].type_name, 'map')
         self.assertEqual(shape.members['endpoints'].key.type_name, 'string')
         self.assertEqual(shape.members['endpoints'].value.type_name, 'object')
         self.assertTrue(self._compare_lists(
@@ -240,18 +212,14 @@
             shape.members['endpoints'].value
 
     def test_no_freeform_map_true_shape(self):
         with self.assertRaises(InvalidShapeError):
             shape = self.resolver.get_shape_by_name('invalid', 'NoFreeformMapTrueTest')
             shape.members['endpoints'].value
 
-    def test_blob_shape(self):
-        shape = self.resolver.get_shape_by_name('shape', 'BlobTest')
-        self.assertEqual(shape.members['blobparam'].type_name, 'blob')
-
     def _compare_lists(self, x, y):
         return collections.Counter(x) == collections.Counter(y)
 
 
 class TestBuilders(unittest.TestCase):
 
     def test_structure_shape_builder_with_scalar_types(self):
```

### Comparing `cdpcli-0.9.89/tests/unit/test_paginate.py` & `cdpcli-0.9.9/tests/unit/test_paginate.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,34 +87,14 @@
         responses = [{'Foo': 'foo', 'NextToken': 'm1'},
                      {'NextToken': 'm2'},
                      {'Foo': 'bar'}]
         self.method.side_effect = responses
         result = self.paginator.paginate().build_full_result()
         self.assertEqual(result, {'Foo': 'foobar'})
 
-    def test_build_full_result_extra_field(self):
-        responses = [{'Extra': 'hello', 'Foo': 0.0, 'NextToken': 'm1'},
-                     {'Extra': 'hello', 'Foo': 0.0}]
-        self.method.side_effect = responses
-        result = self.paginator.paginate().build_full_result()
-        self.assertEqual(result, {'Extra': 'hello', 'Foo': 0.0})
-
-    def test_build_full_result_extra_field_from_first_response(self):
-        responses = [{'Extra': 'hello', 'Foo': 0.0, 'NextToken': 'm1'},
-                     {'Field': 'world', 'Foo': 0.0}]
-        self.method.side_effect = responses
-        result = self.paginator.paginate().build_full_result()
-        self.assertEqual(result, {'Extra': 'hello', 'Foo': 0.0})
-
-    def test_build_full_result_extra_field_only(self):
-        responses = [{'Extra': 'hello'}]
-        self.method.side_effect = responses
-        result = self.paginator.paginate().build_full_result()
-        self.assertEqual(result, {'Extra': 'hello'})
-
     def test_exception_raised_if_same_next_token(self):
         responses = [{'NextToken': 'token1'},
                      {'NextToken': 'token2'},
                      {'NextToken': 'token2'}]
         self.method.side_effect = responses
         with self.assertRaises(PaginationError):
             list(self.paginator.paginate())
```

### Comparing `cdpcli-0.9.89/tests/unit/test_protocol.py` & `cdpcli-0.9.9/tests/unit/test_protocol.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 import datetime
 import os
-import sys
 
 from cdpcli.compat import json
 from cdpcli.compat import six
 from cdpcli.exceptions import ParamValidationError
 from cdpcli.model import ServiceModel
 from cdpcli.parser import ResponseParserFactory
 from cdpcli.serialize import create_serializer
@@ -96,38 +95,14 @@
                                 'crn': 'test-crn-1'},
                                {'name': 'test-name-2',
                                 'crn': 'test-crn-1'}]
         operation_model = self.service_model.operation_model('arrayOfObjects')
         request = self.serializer.serialize_to_request(params, operation_model)
         self._validate_request(request, '/directors/arrayOfObjects', params)
 
-    if sys.version_info.major >= 3:  # bytes is introduced in python3
-        def test_blob_param_bytes(self):
-            params = {}
-            params['data'] = b'Hello World'
-            operation_model = self.service_model.operation_model('blobObject')
-            request = self.serializer.serialize_to_request(params, operation_model)
-            params['data'] = 'SGVsbG8gV29ybGQ='
-            self._validate_request(request, '/directors/blobObject', params)
-
-    def test_blob_param_bytearray(self):
-        params = {}
-        params['data'] = bytearray(b'Hello World')
-        operation_model = self.service_model.operation_model('blobObject')
-        request = self.serializer.serialize_to_request(params, operation_model)
-        params['data'] = 'SGVsbG8gV29ybGQ='
-        self._validate_request(request, '/directors/blobObject', params)
-
-    def test_blob_param_base64(self):
-        params = {}
-        params['data'] = 'SGVsbG8gV29ybGQ='
-        operation_model = self.service_model.operation_model('blobObject')
-        request = self.serializer.serialize_to_request(params, operation_model)
-        self._validate_request(request, '/directors/blobObject', params)
-
 
 class TestParser(unittest.TestCase):
 
     def setUp(self):
         self.model = yaml.safe_load(open(os.path.join(PROTOCOL_DIR, 'service.yaml')))
         self.service_model = ServiceModel(self.model, 'servicename')
         self.parser = ResponseParserFactory().create_parser()
@@ -144,36 +119,14 @@
         body['code'] = code
         body['message'] = message
         response = {}
         response["status_code"] = 301
         response["body"] = json.dumps(body).encode(UTF8)
         return response
 
-    def _create_error_response_2(self, messages):
-        body = {}
-        body['errorMessages'] = messages
-        response = {}
-        response["status_code"] = 401
-        response["body"] = json.dumps(body).encode(UTF8)
-        return response
-
-    def _create_error_response_3(self, message):
-        body = {}
-        body['error'] = message
-        response = {}
-        response["status_code"] = 400
-        response["body"] = json.dumps(body).encode(UTF8)
-        return response
-
-    def _create_error_response_4(self, message):
-        response = {}
-        response["status_code"] = 409
-        response["body"] = message.encode(UTF8)
-        return response
-
     def _assert_same(self, v1, v2, path=""):
         if type(v1) is dict:
             for k in v1.keys():
                 self.assertTrue(k in v2)
                 self._assert_same(v1[k], v2[k])
             for k in v2.keys():
                 self.assertTrue(k in v1)
@@ -290,43 +243,7 @@
     def test_error(self):
         response = self._create_error_response(
             "YouMessedUpException",
             "You, sir, have messed up.")
         operation_model = self.service_model.operation_model('createDirector')
         parsed_response = self.parser.parse(response, operation_model.output_shape)
         self._validate_error_response(response, parsed_response)
-
-    def test_error_2(self):
-        response = self._create_error_response_2([
-            "YouMessedUpException",
-            "You, sir, have messed up."])
-        operation_model = self.service_model.operation_model('createDirector')
-        parsed_response = self.parser.parse(response, operation_model.output_shape)
-        self.assertEquals({
-            'error': {
-                'code': '',
-                'message': 'YouMessedUpException You, sir, have messed up.'}},
-            parsed_response)
-
-    def test_error_3(self):
-        response = self._create_error_response_3(
-            "YouMessedUpException "
-            "You, sir, have messed up.")
-        operation_model = self.service_model.operation_model('createDirector')
-        parsed_response = self.parser.parse(response, operation_model.output_shape)
-        self.assertEquals({
-            'error': {
-                'code': '',
-                'message': 'YouMessedUpException You, sir, have messed up.'}},
-            parsed_response)
-
-    def test_error_4(self):
-        response = self._create_error_response_4(
-            "YouMessedUpException "
-            "You, sir, have messed up.")
-        operation_model = self.service_model.operation_model('createDirector')
-        parsed_response = self.parser.parse(response, operation_model.output_shape)
-        self.assertEquals({
-            'error': {
-                'code': 'UNKNOWN_ERROR',
-                'message': 'YouMessedUpException You, sir, have messed up.'}},
-            parsed_response)
```

### Comparing `cdpcli-0.9.89/tests/unit/test_retryhandler.py` & `cdpcli-0.9.9/tests/unit/test_retryhandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,20 @@
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 
 from cdpcli import retryhandler
+from cdpcli.thirdparty.requests import ConnectionError, Timeout
+from cdpcli.thirdparty.requests.packages.urllib3.exceptions \
+    import ClosedPoolError
 import mock
-from requests import ConnectionError, Timeout
 from tests import unittest
-from urllib3.exceptions import ClosedPoolError
+
 
 HTTP_500_RESPONSE = mock.Mock()
 HTTP_500_RESPONSE.status_code = 500
 
 HTTP_400_RESPONSE = mock.Mock()
 HTTP_400_RESPONSE.status_code = 400
```

### Comparing `cdpcli-0.9.89/tests/unit/test_shorthand.py` & `cdpcli-0.9.9/tests/unit/test_shorthand.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,27 +221,24 @@
     def test_can_convert_scalar_types_from_string(self):
         m = model.DenormalizedStructureBuilder().with_members({
             'A': {'type': 'integer'},
             'B': {'type': 'string'},
             'C': {'type': 'float'},
             'D': {'type': 'boolean'},
             'E': {'type': 'boolean'},
-            'F': {'type': 'blob'},
         }).build_model()
         b = shorthand.BackCompatVisitor()
 
         params = {'A': '24', 'B': '24', 'C': '24.12345',
-                  'D': 'true', 'E': 'false',
-                  'F': 'SGVsbG8gV29ybGQ='}
+                  'D': 'true', 'E': 'false'}
         b.visit(params, m)
         self.assertEqual(
             params,
             {'A': 24, 'B': '24', 'C': float('24.12345'),
-             'D': True, 'E': False,
-             'F': 'SGVsbG8gV29ybGQ='})
+             'D': True, 'E': False})
 
     def test_empty_values_not_added(self):
         m = model.DenormalizedStructureBuilder().with_members({
             'A': {'type': 'boolean'},
         }).build_model()
         b = shorthand.BackCompatVisitor()
```

### Comparing `cdpcli-0.9.89/tests/unit/test_signers.py` & `cdpcli-0.9.9/tests/unit/test_signers.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,17 +21,15 @@
 from cdpcli.signers import RequestSigner
 import mock
 from tests import unittest
 
 
 class BaseSignerTest(unittest.TestCase):
     def setUp(self):
-        self.credentials = Credentials(access_key_id='key',
-                                       private_key='secret',
-                                       method='test')
+        self.credentials = Credentials('key', 'secret', 'test')
         self.signer = RequestSigner('rsav1', self.credentials)
         self.fixed_credentials = self.credentials.get_frozen_credentials()
 
 
 class TestSigner(BaseSignerTest):
 
     def test_signature_version(self):
```

### Comparing `cdpcli-0.9.89/tests/unit/test_table_formatter.py` & `cdpcli-0.9.9/tests/unit/test_table_formatter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.89/tests/unit/test_validate.py` & `cdpcli-0.9.9/tests/unit/test_validate.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 from datetime import datetime
 import decimal
 import os
-import sys
 
 from cdpcli.model import ServiceModel
 from cdpcli.model import ShapeResolver
 from cdpcli.validate import ParamValidator
 from tests import unittest
 import yaml
 
@@ -80,25 +79,23 @@
             {'stringparam': 24,
              'intparam': 'notint',
              'boolparam': 'notbool',
              'numberparam': 'notnumber',
              'datetimeparam': 'notdatetime',
              'arrayparam': 'notarray',
              'objectparam': 'notobject',
-             'mapparam': 'notmap',
-             'blobparam': 123},
+             'mapparam': 'notmap'},
             ['Invalid type for parameter stringparam',
              'Invalid type for parameter intparam',
              'Invalid type for parameter boolparam',
              'Invalid type for parameter numberparam',
              'Invalid type for parameter datetimeparam',
              'Invalid type for parameter arrayparam',
              'Invalid type for parameter objectparam',
-             'Invalid type for parameter mapparam',
-             'Invalid type for parameter blobparam'])
+             'Invalid type for parameter mapparam'])
 
     def test_datetime_type_accepts_datetime_object(self):
         errors = self.get_validation_error_message(
             self.resolver.get_shape_by_name('typestest', 'TypesTest'),
             {'datetimeparam': datetime.now()})
         self.assertEqual(errors.generate_report(), '')
 
@@ -134,58 +131,14 @@
 
     def test_invalid_value_map(self):
         self.assert_has_validation_errors(
             self.resolver.get_shape_by_name('typestest', 'TypesTest'),
             {'mapparam': {'key1': 'value1', 'key2': 2}},
             ["Invalid type for parameter mapparam.key2, value: 2"])
 
-    def test_valid_blob_base64(self):
-        errors = self.get_validation_error_message(
-            self.resolver.get_shape_by_name('typestest', 'TypesTest'),
-            {'blobparam': 'SGVsbG8gV29ybGQ='})
-        self.assertEqual(errors.generate_report(), '')
-
-    def test_valid_blob_empty_base64(self):
-        errors = self.get_validation_error_message(
-            self.resolver.get_shape_by_name('typestest', 'TypesTest'),
-            {'blobparam': ''})
-        self.assertEqual(errors.generate_report(), '')
-
-    def test_invalid_value_blob_base64(self):
-        self.assert_has_validation_errors(
-            self.resolver.get_shape_by_name('typestest', 'TypesTest'),
-            {'blobparam': 'ABC'},
-            ["Invalid base64 value for parameter blobparam, error: Incorrect padding"])
-
-    if sys.version_info.major >= 3:  # bytes is introduced in python3
-        def test_valid_blob_bytes(self):
-            errors = self.get_validation_error_message(
-                self.resolver.get_shape_by_name('typestest', 'TypesTest'),
-                {'blobparam': b'BlobTest'})
-            self.assertEqual(errors.generate_report(), '')
-
-    if sys.version_info.major >= 3:  # bytes is introduced in python3
-        def test_valid_blob_empty_bytes(self):
-            errors = self.get_validation_error_message(
-                self.resolver.get_shape_by_name('typestest', 'TypesTest'),
-                {'blobparam': b''})
-            self.assertEqual(errors.generate_report(), '')
-
-    def test_valid_blob_bytearray(self):
-        errors = self.get_validation_error_message(
-            self.resolver.get_shape_by_name('typestest', 'TypesTest'),
-            {'blobparam': bytearray(b'BlobTest')})
-        self.assertEqual(errors.generate_report(), '')
-
-    def test_valid_blob_empty_bytearray(self):
-        errors = self.get_validation_error_message(
-            self.resolver.get_shape_by_name('typestest', 'TypesTest'),
-            {'blobparam': bytearray(b'')})
-        self.assertEqual(errors.generate_report(), '')
-
 
 class TestValidateRanges(BaseTestValidate):
 
     def test_less_than_range(self):
         self.assert_has_validation_errors(
             self.resolver.get_shape_by_name('rangetest', 'RangeTest'),
             {'intparam': -10,
@@ -240,52 +193,14 @@
 
     def test_only_max_value_specified(self):
         self.assert_has_validation_errors(
             self.resolver.get_shape_by_name('rangetest', 'RangeTest'),
             {'maxonlystringparam': 'thisistoolong'},
             ['Invalid length for parameter maxonlystringparam'])
 
-    if sys.version_info.major >= 3:  # bytes is introduced in python3
-        def test_blob_min_length_contraint_bytes(self):
-            self.assert_has_validation_errors(
-                self.resolver.get_shape_by_name('rangetest', 'RangeTest'),
-                {'blobparam': b''},
-                ['Invalid length for parameter blobparam'])
-
-    if sys.version_info.major >= 3:  # bytes is introduced in python3
-        def test_blob_max_length_contraint_bytes(self):
-            self.assert_has_validation_errors(
-                self.resolver.get_shape_by_name('rangetest', 'RangeTest'),
-                {'blobparam': b'thisistoolong'},
-                ['Invalid length for parameter blobparam'])
-
-    def test_blob_min_length_contraint_bytearray(self):
-        self.assert_has_validation_errors(
-            self.resolver.get_shape_by_name('rangetest', 'RangeTest'),
-            {'blobparam': bytearray(b'')},
-            ['Invalid length for parameter blobparam'])
-
-    def test_blob_max_length_contraint_bytearray(self):
-        self.assert_has_validation_errors(
-            self.resolver.get_shape_by_name('rangetest', 'RangeTest'),
-            {'blobparam': bytearray(b'thisistoolong')},
-            ['Invalid length for parameter blobparam'])
-
-    def test_blob_min_length_contraint_base64(self):
-        self.assert_has_validation_errors(
-            self.resolver.get_shape_by_name('rangetest', 'RangeTest'),
-            {'blobparam': ''},
-            ['Invalid length for parameter blobparam'])
-
-    def test_blob_max_length_contraint_base64(self):
-        self.assert_has_validation_errors(
-            self.resolver.get_shape_by_name('rangetest', 'RangeTest'),
-            {'blobparam': 'dGhpc2lzdG9vbG9uZw=='},
-            ['Invalid length for parameter blobparam'])
-
 
 class TestValidationNumberType(BaseTestValidate):
 
     def test_range_number(self):
         self.assert_has_validation_errors(
             self.resolver.get_shape_by_name('numbertest', 'NumberTest'),
             {'numberparam': 1},
```

### Comparing `cdpcli-0.9.89/versioneer.py` & `cdpcli-0.9.9/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -558,23 +558,23 @@
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
     keywords = {}
     try:
         f = open(versionfile_abs, "r")
         for line in f.readlines():
             if line.strip().startswith("git_refnames ="):
-                mo = re.search('=\\s*"(.*)"', line)
+                mo = re.search(r'=\s*"(.*)"', line)
                 if mo:
                     keywords["refnames"] = mo.group(1)
             if line.strip().startswith("git_full ="):
-                mo = re.search('=\\s*"(.*)"', line)
+                mo = re.search(r'=\s*"(.*)"', line)
                 if mo:
                     keywords["full"] = mo.group(1)
             if line.strip().startswith("git_date ="):
-                mo = re.search('=\\s*"(.*)"', line)
+                mo = re.search(r'=\s*"(.*)"', line)
                 if mo:
                     keywords["date"] = mo.group(1)
         f.close()
     except EnvironmentError:
         pass
     return keywords
 
@@ -607,15 +607,15 @@
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %%d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search('\\d', r)])
+        tags = set([r for r in refs if re.search(r'\d', r)])
         if verbose:
             print("discarding '%%s', no digits" %% ",".join(refs - tags))
     if verbose:
         print("likely tags: %%s" %% ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
@@ -683,15 +683,15 @@
     if dirty:
         git_describe = git_describe[:git_describe.rindex("-dirty")]
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
-        mo = re.search('^(.+)-(\\d+)-g([0-9a-f]+)$', git_describe)
+        mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
             # unparseable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%%s'"
                                %% describe_out)
             return pieces
 
         # tag
```

