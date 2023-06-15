# Comparing `tmp/cdpcli-beta-0.9.88.tar.gz` & `tmp/cdpcli-beta-0.9.89.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdpcli-beta-0.9.88.tar", last modified: Thu Jun  1 21:08:34 2023, max compression
+gzip compressed data, was "cdpcli-beta-0.9.89.tar", last modified: Wed Jun 14 22:47:31 2023, max compression
```

## Comparing `cdpcli-beta-0.9.88.tar` & `cdpcli-beta-0.9.89.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.370914 cdpcli-beta-0.9.88/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11358 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/LICENSE.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2309 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      301 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/MANIFEST.in
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-06-01 21:08:34.370914 cdpcli-beta-0.9.88/PKG-INFO
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5510 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/README.md
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.370914 cdpcli-beta-0.9.88/cdpcli/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3972 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      497 2023-06-01 21:08:34.370914 cdpcli-beta-0.9.88/cdpcli/_version.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8594 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/argparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    16126 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/argprocess.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    13419 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/arguments.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11535 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/auth.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    16324 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/cdprequest.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1207 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/clicommand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31143 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/clidriver.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    22668 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/client.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6574 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/compat.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6562 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/completer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4116 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/config.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8338 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/configloader.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    15597 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/credentials.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.358914 cdpcli-beta-0.9.88/cdpcli/data/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1002 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/data/_retry.json
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      246 2023-06-01 21:08:33.000000 cdpcli-beta-0.9.88/cdpcli/data/aliases.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.358914 cdpcli-beta-0.9.88/cdpcli/data/audit/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    32709 2023-06-01 21:08:33.000000 cdpcli-beta-0.9.88/cdpcli/data/audit/audit.yaml
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3965 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/data/cli.json
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.358914 cdpcli-beta-0.9.88/cdpcli/data/cloudprivatelinks/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8803 2023-06-01 21:08:30.000000 cdpcli-beta-0.9.88/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.358914 cdpcli-beta-0.9.88/cdpcli/data/compute/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    95423 2023-06-01 21:08:29.000000 cdpcli-beta-0.9.88/cdpcli/data/compute/compute.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.358914 cdpcli-beta-0.9.88/cdpcli/data/datacatalog/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4002 2023-06-01 21:08:33.000000 cdpcli-beta-0.9.88/cdpcli/data/datacatalog/datacatalog.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.358914 cdpcli-beta-0.9.88/cdpcli/data/datahub/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   148743 2023-06-01 21:08:32.000000 cdpcli-beta-0.9.88/cdpcli/data/datahub/datahub.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.358914 cdpcli-beta-0.9.88/cdpcli/data/datalake/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   104133 2023-06-01 21:08:30.000000 cdpcli-beta-0.9.88/cdpcli/data/datalake/datalake.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.358914 cdpcli-beta-0.9.88/cdpcli/data/de/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31670 2023-06-01 21:08:32.000000 cdpcli-beta-0.9.88/cdpcli/data/de/de.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.358914 cdpcli-beta-0.9.88/cdpcli/data/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    91702 2023-06-01 21:08:31.000000 cdpcli-beta-0.9.88/cdpcli/data/df/df.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.358914 cdpcli-beta-0.9.88/cdpcli/data/dfworkload/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    81768 2023-06-01 21:08:32.000000 cdpcli-beta-0.9.88/cdpcli/data/dfworkload/dfworkload.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.358914 cdpcli-beta-0.9.88/cdpcli/data/drscp/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    21583 2023-06-01 21:08:30.000000 cdpcli-beta-0.9.88/cdpcli/data/drscp/drscp.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.358914 cdpcli-beta-0.9.88/cdpcli/data/dw/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   193260 2023-06-01 21:08:30.000000 cdpcli-beta-0.9.88/cdpcli/data/dw/dw.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.362914 cdpcli-beta-0.9.88/cdpcli/data/environments/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   175998 2023-06-01 21:08:29.000000 cdpcli-beta-0.9.88/cdpcli/data/environments/environments.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.362914 cdpcli-beta-0.9.88/cdpcli/data/iam/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   149065 2023-06-01 21:08:31.000000 cdpcli-beta-0.9.88/cdpcli/data/iam/iam.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.362914 cdpcli-beta-0.9.88/cdpcli/data/imagecatalog/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    25663 2023-06-01 21:08:30.000000 cdpcli-beta-0.9.88/cdpcli/data/imagecatalog/imagecatalog.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.362914 cdpcli-beta-0.9.88/cdpcli/data/ml/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    56911 2023-06-01 21:08:33.000000 cdpcli-beta-0.9.88/cdpcli/data/ml/ml.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.362914 cdpcli-beta-0.9.88/cdpcli/data/opdb/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    72034 2023-06-01 21:08:32.000000 cdpcli-beta-0.9.88/cdpcli/data/opdb/opdb.yaml
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        4 2023-06-01 21:08:33.000000 cdpcli-beta-0.9.88/cdpcli/data/release.txt
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.362914 cdpcli-beta-0.9.88/cdpcli/data/replicationmanager/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    30963 2023-06-01 21:08:33.000000 cdpcli-beta-0.9.88/cdpcli/data/replicationmanager/replicationmanager.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.362914 cdpcli-beta-0.9.88/cdpcli/doc/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/doc/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1857 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/doc/docstringparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7269 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/doc/restdoc.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10873 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/doc/style.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    29420 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/docs.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17043 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/endpoint.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.350914 cdpcli-beta-0.9.88/cdpcli/examples/
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.362914 cdpcli-beta-0.9.88/cdpcli/examples/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1942 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/examples/configure/_description.rst
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.362914 cdpcli-beta-0.9.88/cdpcli/examples/configure/get/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1940 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/examples/configure/get/_description.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      764 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/examples/configure/get/_examples.rst
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.362914 cdpcli-beta-0.9.88/cdpcli/examples/configure/set/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      862 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/examples/configure/set/_description.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      560 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/examples/configure/set/_examples.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9213 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/exceptions.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.362914 cdpcli-beta-0.9.88/cdpcli/extensions/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      971 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2650 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/arguments.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3908 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/cliinputjson.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17226 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/commands.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.366914 cdpcli-beta-0.9.88/cdpcli/extensions/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1330 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/configure/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2047 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/configure/classify.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6210 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/configure/configure.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3749 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/configure/get.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6414 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/configure/list.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5108 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/configure/set.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.366914 cdpcli-beta-0.9.88/cdpcli/extensions/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12046 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/df/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    29050 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/df/createdeployment.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1575 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/df/register.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3353 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/generatecliskeleton.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10396 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/interactivelogin.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2154 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/logout.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9335 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2642 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/redirect.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6277 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/refdoc.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3771 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/workload.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11071 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/extensions/writer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9343 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/formatter.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8083 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/help.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9314 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/loader.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      771 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/main.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    18902 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/model.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7307 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5898 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/paramfile.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3218 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/paramformfactor.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4085 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/parser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11836 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/retryhandler.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5732 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/schema.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4322 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/serialize.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14202 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/shorthand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2258 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/signers.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14828 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/table.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4389 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/text.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    20981 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/textwriter.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.366914 cdpcli-beta-0.9.88/cdpcli/thirdparty/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/thirdparty/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    27344 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/thirdparty/six.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1652 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/translate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10165 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/utils.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10637 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/cdpcli/validate.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.366914 cdpcli-beta-0.9.88/cdpcli_beta.egg-info/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-06-01 21:08:34.000000 cdpcli-beta-0.9.88/cdpcli_beta.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4297 2023-06-01 21:08:34.000000 cdpcli-beta-0.9.88/cdpcli_beta.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        1 2023-06-01 21:08:34.000000 cdpcli-beta-0.9.88/cdpcli_beta.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)       85 2023-06-01 21:08:34.000000 cdpcli-beta-0.9.88/cdpcli_beta.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      190 2023-06-01 21:08:34.000000 cdpcli-beta-0.9.88/cdpcli_beta.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)       13 2023-06-01 21:08:34.000000 cdpcli-beta-0.9.88/cdpcli_beta.egg-info/top_level.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      271 2023-06-01 21:08:34.370914 cdpcli-beta-0.9.88/setup.cfg
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1429 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/setup.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2655 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/setup_common.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.354914 cdpcli-beta-0.9.88/tests/
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.366914 cdpcli-beta-0.9.88/tests/unit/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4604 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.370914 cdpcli-beta-0.9.88/tests/unit/cdp/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1815 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/cdp/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.370914 cdpcli-beta-0.9.88/tests/unit/extensions/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      732 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.370914 cdpcli-beta-0.9.88/tests/unit/extensions/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/configure/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2290 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/configure/test_classify.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12860 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/configure/test_configure.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5637 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/configure/test_get.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6675 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/configure/test_list.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6656 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/configure/test_set.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-01 21:08:34.370914 cdpcli-beta-0.9.88/tests/unit/extensions/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/df/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    38131 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/df/test_createdeployment.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2253 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/df/test_upload_file.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5854 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/test_cliinputjson.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    18795 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/test_df.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3807 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/test_generatecliskeleton.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17115 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/test_interactivelogin.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2556 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/test_logout.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8305 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/test_operation_extension.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10918 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/test_paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4828 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/test_redirect.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9041 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/test_workload.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11649 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/extensions/test_writer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2709 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_argparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4768 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_argprocess.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11931 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_auth.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4421 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_cli_data.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12187 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_client.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14018 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_completer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    23039 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_credentials.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7271 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_docs.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31273 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_endpoint.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10750 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_help.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12035 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_loaders.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14102 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_model.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    15246 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8243 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_paramfile.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14417 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_protocol.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    13714 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_retryhandler.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11240 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_shorthand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3227 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_signers.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    22467 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_table_formatter.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12971 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_utils.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12772 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/tests/unit/test_validate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    68612 2023-06-01 20:56:05.000000 cdpcli-beta-0.9.88/versioneer.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.528537 cdpcli-beta-0.9.89/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11358 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/LICENSE.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2309 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      301 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/MANIFEST.in
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-06-14 22:47:31.528537 cdpcli-beta-0.9.89/PKG-INFO
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5510 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/README.md
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.528537 cdpcli-beta-0.9.89/cdpcli/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3972 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      497 2023-06-14 22:47:31.528537 cdpcli-beta-0.9.89/cdpcli/_version.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8594 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/argparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    16126 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/argprocess.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    13419 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/arguments.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11535 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/auth.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    16324 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/cdprequest.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1207 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/clicommand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    31143 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/clidriver.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    22668 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/client.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6574 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/compat.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6562 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/completer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4116 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/config.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8338 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/configloader.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    15597 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/credentials.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1002 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/data/_retry.json
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      246 2023-06-14 22:47:30.000000 cdpcli-beta-0.9.89/cdpcli/data/aliases.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/audit/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    32709 2023-06-14 22:47:30.000000 cdpcli-beta-0.9.89/cdpcli/data/audit/audit.yaml
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3965 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/data/cli.json
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/cloudprivatelinks/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8803 2023-06-14 22:47:27.000000 cdpcli-beta-0.9.89/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/compute/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    97819 2023-06-14 22:47:26.000000 cdpcli-beta-0.9.89/cdpcli/data/compute/compute.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/datacatalog/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4002 2023-06-14 22:47:30.000000 cdpcli-beta-0.9.89/cdpcli/data/datacatalog/datacatalog.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/datahub/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   148743 2023-06-14 22:47:28.000000 cdpcli-beta-0.9.89/cdpcli/data/datahub/datahub.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/datalake/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   104375 2023-06-14 22:47:27.000000 cdpcli-beta-0.9.89/cdpcli/data/datalake/datalake.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/de/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    32532 2023-06-14 22:47:29.000000 cdpcli-beta-0.9.89/cdpcli/data/de/de.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    91702 2023-06-14 22:47:28.000000 cdpcli-beta-0.9.89/cdpcli/data/df/df.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/dfworkload/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    81768 2023-06-14 22:47:29.000000 cdpcli-beta-0.9.89/cdpcli/data/dfworkload/dfworkload.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/drscp/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    21583 2023-06-14 22:47:27.000000 cdpcli-beta-0.9.89/cdpcli/data/drscp/drscp.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/dw/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   193260 2023-06-14 22:47:27.000000 cdpcli-beta-0.9.89/cdpcli/data/dw/dw.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/environments/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   177206 2023-06-14 22:47:26.000000 cdpcli-beta-0.9.89/cdpcli/data/environments/environments.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/iam/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   149065 2023-06-14 22:47:28.000000 cdpcli-beta-0.9.89/cdpcli/data/iam/iam.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/imagecatalog/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    25663 2023-06-14 22:47:27.000000 cdpcli-beta-0.9.89/cdpcli/data/imagecatalog/imagecatalog.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.516537 cdpcli-beta-0.9.89/cdpcli/data/ml/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    56911 2023-06-14 22:47:29.000000 cdpcli-beta-0.9.89/cdpcli/data/ml/ml.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.520537 cdpcli-beta-0.9.89/cdpcli/data/opdb/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    72034 2023-06-14 22:47:29.000000 cdpcli-beta-0.9.89/cdpcli/data/opdb/opdb.yaml
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        4 2023-06-14 22:47:30.000000 cdpcli-beta-0.9.89/cdpcli/data/release.txt
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.520537 cdpcli-beta-0.9.89/cdpcli/data/replicationmanager/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    30963 2023-06-14 22:47:30.000000 cdpcli-beta-0.9.89/cdpcli/data/replicationmanager/replicationmanager.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.520537 cdpcli-beta-0.9.89/cdpcli/doc/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/doc/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1857 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/doc/docstringparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7269 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/doc/restdoc.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10873 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/doc/style.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    29420 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/docs.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17043 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/endpoint.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.508536 cdpcli-beta-0.9.89/cdpcli/examples/
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.520537 cdpcli-beta-0.9.89/cdpcli/examples/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1942 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/examples/configure/_description.rst
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.520537 cdpcli-beta-0.9.89/cdpcli/examples/configure/get/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1940 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/examples/configure/get/_description.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      764 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/examples/configure/get/_examples.rst
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.520537 cdpcli-beta-0.9.89/cdpcli/examples/configure/set/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      862 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/examples/configure/set/_description.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      560 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/examples/configure/set/_examples.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9213 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/exceptions.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.520537 cdpcli-beta-0.9.89/cdpcli/extensions/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      971 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2650 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/arguments.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3908 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/cliinputjson.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17226 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/commands.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.520537 cdpcli-beta-0.9.89/cdpcli/extensions/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1330 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/configure/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2047 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/configure/classify.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6210 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/configure/configure.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3749 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/configure/get.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6414 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/configure/list.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5108 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/configure/set.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.520537 cdpcli-beta-0.9.89/cdpcli/extensions/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12046 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/df/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    29050 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/df/createdeployment.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1575 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/df/register.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3353 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/generatecliskeleton.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10396 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/interactivelogin.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2154 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/logout.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9335 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2642 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/redirect.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6277 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/refdoc.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3771 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/workload.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11071 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/extensions/writer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9343 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/formatter.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8083 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/help.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9314 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/loader.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      771 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/main.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    18902 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/model.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7307 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5898 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/paramfile.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3218 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/paramformfactor.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4085 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/parser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11836 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/retryhandler.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5732 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/schema.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4322 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/serialize.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14202 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/shorthand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2258 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/signers.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14828 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/table.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4389 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/text.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    20981 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/textwriter.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.520537 cdpcli-beta-0.9.89/cdpcli/thirdparty/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/thirdparty/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    27344 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/thirdparty/six.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1652 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/translate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10165 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/utils.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10637 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/cdpcli/validate.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.524537 cdpcli-beta-0.9.89/cdpcli_beta.egg-info/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-06-14 22:47:30.000000 cdpcli-beta-0.9.89/cdpcli_beta.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4297 2023-06-14 22:47:30.000000 cdpcli-beta-0.9.89/cdpcli_beta.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        1 2023-06-14 22:47:30.000000 cdpcli-beta-0.9.89/cdpcli_beta.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)       85 2023-06-14 22:47:30.000000 cdpcli-beta-0.9.89/cdpcli_beta.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      190 2023-06-14 22:47:30.000000 cdpcli-beta-0.9.89/cdpcli_beta.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)       13 2023-06-14 22:47:30.000000 cdpcli-beta-0.9.89/cdpcli_beta.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      271 2023-06-14 22:47:31.528537 cdpcli-beta-0.9.89/setup.cfg
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1429 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/setup.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2655 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/setup_common.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.508536 cdpcli-beta-0.9.89/tests/
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.524537 cdpcli-beta-0.9.89/tests/unit/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4604 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.524537 cdpcli-beta-0.9.89/tests/unit/cdp/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1815 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/cdp/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.524537 cdpcli-beta-0.9.89/tests/unit/extensions/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      732 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.528537 cdpcli-beta-0.9.89/tests/unit/extensions/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/configure/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2290 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/configure/test_classify.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12860 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/configure/test_configure.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5637 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/configure/test_get.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6675 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/configure/test_list.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6656 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/configure/test_set.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:47:31.528537 cdpcli-beta-0.9.89/tests/unit/extensions/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/df/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    38131 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/df/test_createdeployment.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2253 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/df/test_upload_file.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5854 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/test_cliinputjson.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    18795 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/test_df.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3807 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/test_generatecliskeleton.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17115 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/test_interactivelogin.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2556 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/test_logout.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8305 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/test_operation_extension.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10918 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/test_paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4828 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/test_redirect.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9041 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/test_workload.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11649 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/extensions/test_writer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2709 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_argparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4768 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_argprocess.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11931 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_auth.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4421 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_cli_data.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12187 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_client.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14018 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_completer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    23039 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_credentials.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7271 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_docs.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    31273 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_endpoint.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10750 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_help.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12035 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_loaders.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14102 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_model.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    15246 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8243 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_paramfile.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14417 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_protocol.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    13714 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_retryhandler.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11240 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_shorthand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3227 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_signers.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    22467 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_table_formatter.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12971 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_utils.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12772 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/tests/unit/test_validate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    68612 2023-06-14 22:34:55.000000 cdpcli-beta-0.9.89/versioneer.py
```

### Comparing `cdpcli-beta-0.9.88/LICENSE.txt` & `cdpcli-beta-0.9.89/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt` & `cdpcli-beta-0.9.89/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/PKG-INFO` & `cdpcli-beta-0.9.89/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdpcli-beta
-Version: 0.9.88
+Version: 0.9.89
 Summary: Cloudera CDP Command Line Interface (BETA)
 Home-page: https://console.cdp.cloudera.com/
 Author: Cloudera, Inc.
 License: Apache License 2.0
 Description: # Cloudera CDP Command Line Interface
         
         This package provides a unified command line interface to the Cloudera Data
```

### Comparing `cdpcli-beta-0.9.88/README.md` & `cdpcli-beta-0.9.89/README.md`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/__init__.py` & `cdpcli-beta-0.9.89/cdpcli/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/argparser.py` & `cdpcli-beta-0.9.89/cdpcli/argparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/argprocess.py` & `cdpcli-beta-0.9.89/cdpcli/argprocess.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/arguments.py` & `cdpcli-beta-0.9.89/cdpcli/arguments.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/auth.py` & `cdpcli-beta-0.9.89/cdpcli/auth.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/cdprequest.py` & `cdpcli-beta-0.9.89/cdpcli/cdprequest.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/clicommand.py` & `cdpcli-beta-0.9.89/cdpcli/clicommand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/clidriver.py` & `cdpcli-beta-0.9.89/cdpcli/clidriver.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/client.py` & `cdpcli-beta-0.9.89/cdpcli/client.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/compat.py` & `cdpcli-beta-0.9.89/cdpcli/compat.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/completer.py` & `cdpcli-beta-0.9.89/cdpcli/completer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/config.py` & `cdpcli-beta-0.9.89/cdpcli/config.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/configloader.py` & `cdpcli-beta-0.9.89/cdpcli/configloader.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/credentials.py` & `cdpcli-beta-0.9.89/cdpcli/credentials.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/data/_retry.json` & `cdpcli-beta-0.9.89/cdpcli/data/_retry.json`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/data/audit/audit.yaml` & `cdpcli-beta-0.9.89/cdpcli/data/audit/audit.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: audit
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.88
+  version: 0.9.89
   title: Cloudera Audit Service
   license:
     name: Apache 2.0
   description: Cloudera CDP Auditing is a web service for interacting with the audit subsystem.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.88/cdpcli/data/cli.json` & `cdpcli-beta-0.9.89/cdpcli/data/cli.json`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml` & `cdpcli-beta-0.9.89/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: cloudprivatelinks
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: BETA
 info:
-  version: 0.9.88
+  version: 0.9.89
   title: Cloudera CloudPrivateLinks API Service
   license:
     name: Apache 2.0
   description: Provisions PrivateLink Endpoints on the cloud environments.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.88/cdpcli/data/compute/compute.yaml` & `cdpcli-beta-0.9.89/cdpcli/data/compute/compute.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: compute
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.88
+  version: 0.9.89
   title: Cloudera Compute Service
   license:
     name: Apache 2.0
   description: Defining service of compute public API service
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -1469,14 +1469,67 @@
         description: Compute cluster creation time in ISO format.
       clusterId:
         type: string
         description: Compute cluster ID.
       envCrn:
         type: string
         description: CDP environment CRN.
+      apiEndPoint:
+        type: string
+        description: API endpoint.
+        x-form-factors: public
+      clusterStateVersion:
+        type: integer
+        format: int32
+        description: Cluster state version.
+        x-form-factors: public
+      deletionTime:
+        type: string
+        description: Compute cluster deletion time in ISO format.
+        x-form-factors: public
+      updateTime:
+        type: string
+        description: Compute cluster update time in ISO format.
+        x-form-factors: public
+      workloads:
+        type: array
+        items:
+          type: string
+        description: Workloads.
+        x-form-factors: public
+      clusterOwner:
+        description: Cluster owner.
+        $ref: '#/definitions/ComputeClusterOwner'
+        x-form-factors: public
+      region:
+        type: string
+        description: Region.
+        x-form-factors: public
+      message:
+        type: string
+        description: Message with additional details about the cluster status.
+        x-form-factors: public
+      account:
+        type: string
+        description: CDP account ID.
+        x-form-factors: public
+      availableUpgrades:
+        type: array
+        items:
+          type: string
+        description: List of available kubernetes upgrades.
+        x-form-factors: public
+      imageCatalog:
+        description: The image catalog details.
+        $ref: '#/definitions/CommonImageCatalogResp'
+        x-form-factors: public
+      storage:
+        description: The storage specifications.
+        $ref: '#/definitions/CommonStorageSpecResp'
+        x-form-factors: public
       labels:
         type: object
         description: Map of labels associated with this cluster.
         additionalProperties:
           type: string
       bootstrapScript:
         type: string
@@ -1485,14 +1538,18 @@
         description: AKS state.
         $ref: '#/definitions/AksState'
         x-form-factors: public
       eks:
         description: EKS state.
         $ref: '#/definitions/EksState'
         x-form-factors: public
+      nodeImageUpgradeAvailable:
+        type: boolean
+        description: Is a node image upgrade available.
+        x-form-factors: public
   ListClustersRequest:
     type: object
     description: Request object to list clusters.
     properties:
       envNameOrCrn:
         type: string
         description: Environment name or crn.
@@ -1514,14 +1571,19 @@
         default: 100
         x-form-factors: public
       startingToken:
         type: string
         x-paging-input-token: true
         description: A token to specify where to start paginating. This is the nextToken from a previously truncated response. 1 or empty for first page.
         x-form-factors: public
+      includeDeleted:
+        type: boolean
+        description: Include deleted clusters in the response. Optional.
+        default: false
+        x-form-factors: public
   ListClusterItem:
     type: object
     description: List clusters item structure.
     properties:
       envName:
         type: string
         description: CDP environment name.
@@ -2520,14 +2582,17 @@
         description: The version of this chart (which is not the version of the components being deployed).
       description:
         type: string
         description: The chart description.
       name:
         type: string
         description: The chart name.
+      values:
+        type: string
+        description: Escaped JSON for values.yaml of that chart.
   AvailableDeploymentUpgrade:
     type: object
     description: Available deployment upgrade structure.
     properties:
       applicationVersion:
         type: string
         description: The version of the components which would be installed from this deployment.
@@ -2558,28 +2623,34 @@
         type: string
         description: Status of the deployment. Currently supported values are UNKNOWN, DEPLOYED, UNINSTALLED, SUPERSEDED, FAILED, PENDING-INSTALL, PENDING-UPGRADE and PENDING-ROLLBACK. New values may be added in the future.
       upgrades:
         type: array
         items:
           $ref: '#/definitions/AvailableDeploymentUpgrade'
         description: Any upgrades available for this deployment.
+      overrides:
+        type: string
+        description: Escaped JSON overrides for the deployment's properties.
   History:
     type: object
     description: History structure.
     properties:
       revision:
         type: integer
         format: int32
         description: Helm revision.
       status:
         type: string
         description: Status of the deployment. Currently supported values are UNKNOWN, DEPLOYED, UNINSTALLED, SUPERSEDED, FAILED, PENDING-INSTALL, PENDING-UPGRADE and PENDING-ROLLBACK. New values may be added in the future.
       chart:
         description: Chart that the deployment was created from.
         $ref: '#/definitions/Chart'
+      overrides:
+        type: string
+        description: Escaped JSON overrides for the deployment's properties for given revision.
   DescribeDeploymentResponse:
     type: object
     description: Response structure for describing a deployment.
     properties:
       deployment:
         description: Deployment details.
         $ref: '#/definitions/Deployment'
@@ -2674,14 +2745,17 @@
     properties:
       clusterCrn:
         type: string
         description: Compute cluster CRN.
       namespace:
         type: string
         description: The namespace of the deployment. Lists deployments in all namespaces if not specified.
+      verbose:
+        type: boolean
+        description: Set true to get detailed chart response. Default is false.
   ListDeploymentsResponse:
     type: object
     description: Response structure to list deployments in the cluster.
     properties:
       availableCharts:
         type: array
         items:
```

### Comparing `cdpcli-beta-0.9.88/cdpcli/data/datacatalog/datacatalog.yaml` & `cdpcli-beta-0.9.89/cdpcli/data/datacatalog/datacatalog.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: datacatalog
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.88
+  version: 0.9.89
   title: Cloudera DataCatalog Service
   license:
     name: Apache 2.0
   description: Cloudera DataCatalog Service is a web service, using this service a user can execute operations like launching profilers in DataCatalog.
 schemes:
   - https
 consumes:
```

### Comparing `cdpcli-beta-0.9.88/cdpcli/data/datahub/datahub.yaml` & `cdpcli-beta-0.9.89/cdpcli/data/datahub/datahub.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: datahub
 x-interface-model: cdp
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.88
+  version: 0.9.89
   title: Cloudera Data hub Service
   license:
     name: Apache 2.0
   description: Cloudera data hub is a service for launching and managing workload clusters powered by Cloudera Runtime.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.88/cdpcli/data/datalake/datalake.yaml` & `cdpcli-beta-0.9.89/cdpcli/data/datalake/datalake.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: datalake
 x-interface-model: cdp
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.88
+  version: 0.9.89
   title: Cloudera Datalake Service
   license:
     name: Apache 2.0
   description: Cloudera data lake is a service for launching and managing data lake clusters powered by Cloudera Runtime.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -2300,14 +2300,17 @@
         description: Skips the backup of the Atlas metadata. Redundant if --skip-backup is included. If this option is not provided, the Atlas metadata is backed up by default.
       skipRangerAudits:
         type: boolean
         description: Skips the backup of the Ranger audits. Redundant if --skip-backup is included. If this option is not provided, Ranger audits are backed up by default.
       skipDatahubValidation:
         type: boolean
         description: With this option, the Data Lake upgrade can be performed with running Data Hub clusters. This option may cause problems on the running Data Hub clusters during the Data Lake upgrade.
+      skipBackupValidation:
+        type: boolean
+        description: Skips the validation steps that run prior to the backup. Redundant if --skip-backup is included. If this option is not provided, the validations are performed by default.
       rollingUpgradeEnabled:
         type: boolean
         description: Enables the ability to perform rolling runtime upgrade.
   UpgradeDatalakeResponse:
     type: object
     description: Response object for upgrade datalake request.
     properties:
```

### Comparing `cdpcli-beta-0.9.88/cdpcli/data/de/de.yaml` & `cdpcli-beta-0.9.89/cdpcli/data/de/de.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: de
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.88
+  version: 0.9.89
   title: Cloudera Data Engineering
   license:
     name: Apache 2.0
   description: Create and manage Cloudera Data Engineering Services.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -356,14 +356,17 @@
         description: List of Subnet IDs of the CDP subnets used by the kubernetes worker node.
       privateClusterEnabled:
         type: boolean
         description: If true, the CDE service was created with fully private Azure services (AKS, MySQL, etc.).
       publicEndpointEnabled:
         type: boolean
         description: If true, the CDE endpoint was created in a publicly accessible subnet.
+      previousVersionDeployed:
+        type: boolean
+        description: The "true" value indicates that the previous version of the CDE service was requested to be deployed.
       workloadAnalyticsEnabled:
         type: boolean
         description: If true, diagnostic information about job and query execution is sent to Cloudera Workload Manager.
       ssdUsed:
         type: boolean
         description: If true, SSD would have been be used for workload filesystem.
   ServiceResources:
@@ -483,14 +486,17 @@
         description: Chart overrides for the Virtual Cluster.
       accessControl:
         description: Access control object for the Virtual Cluster.
         $ref: '#/definitions/AccessControlResponse'
       smtpConfig:
         description: SMTP Configurations for Airflow Email Alerts.
         $ref: '#/definitions/SmtpConfigResponse'
+      vcTier:
+        type: string
+        description: Tier of the Virtual Cluster.
   VcResources:
     type: object
     properties:
       cpuRequests:
         type: string
         description: The CPU requests for VC for running spark jobs.
       memRequests:
@@ -649,14 +655,18 @@
         type: integer
         format: int32
         description: EBS volume size in GB.
       enablePublicEndpoint:
         type: boolean
         default: false
         description: Creates a CDE endpoint (Load Balancer) in a publicly accessible subnet. If set false, the endpoint will be created in a private subnet and you will need to setup access to the endpoint manually in your cloud account.
+      deployPreviousVersion:
+        type: boolean
+        default: false
+        description: If set to "true", the previous version of the CDE service will be deployed.
       enableWorkloadAnalytics:
         type: boolean
         default: false
         description: If set false, diagnostic information about job and query execution is sent to Cloudera Workload Manager. Anonymization can be configured under Environments / Shared Resources / Telemetry. Refer documentation for more info at https://docs.cloudera.com/workload-manager/cloud/index.html.
       useSsd:
         type: boolean
         description: Instance local storage (SSD) would be used for the workload filesystem (Example - spark local directory). In case the workload requires more space than what's available in the instance storage, please use an instance type with sufficient instance local storage or choose an instance type without SSD and configure the EBS volume size. Currently supported only for aws services.
@@ -902,14 +912,20 @@
       sparkVersion:
         type: string
         description: Spark version for the virtual cluster. Currently supported spark versions are SPARK2(deprecated), SPARK3 and SPARK3_3. This feature is only supported in CDE-1.7.0 and beyond. SPARK3_3 is supported in CDE-1.19 and beyond.
         enum:
           - SPARK2
           - SPARK3
           - SPARK3_3
+      vcTier:
+        type: string
+        description: Tier of the virtual cluster. Currently supported tiers are CORE and ALLP. CORE tiered virtual cluster enables operational deployment via batch jobs. ALLP virtual clusters are all-purpose virtual clusters supporting both operational batch jobs and interactive sessions. This feature is only supported in CDE-1.19.0 and beyond.
+        enum:
+          - ALLP
+          - CORE
       aclUsers:
         description: Comma-separated Workload usernames of CDP users to be granted access to the Virtual Cluster.
         type: string
   CreateVcResponse:
     type: object
     description: Response object for CreateVc method.
     properties:
```

### Comparing `cdpcli-beta-0.9.88/cdpcli/data/df/df.yaml` & `cdpcli-beta-0.9.89/cdpcli/data/df/df.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: df
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.88
+  version: 0.9.89
   title: Cloudera DataFlow Service
   license:
     name: Apache 2.0
   description: Manage DataFlow Services.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.88/cdpcli/data/dfworkload/dfworkload.yaml` & `cdpcli-beta-0.9.89/cdpcli/data/dfworkload/dfworkload.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 swagger: '2.0'
 x-endpoint-name: dfworkload
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
   description: "This REST API provides remote access to the DataFlow Service.\n Endpoints that are marked as [BETA] are subject to change in future releases of the application without backwards compatibility and without a major version change."
-  version: 0.9.88
+  version: 0.9.89
   title: Cloudera DataFlow Workload Service
   license:
     name: Apache 2.0
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
 consumes:
```

### Comparing `cdpcli-beta-0.9.88/cdpcli/data/drscp/drscp.yaml` & `cdpcli-beta-0.9.89/cdpcli/data/drscp/drscp.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: drscp
 x-products: CDP
 x-form-factors: private
 x-audit: true
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.88
+  version: 0.9.89
   title: CDP Control Plane Data Recovery Service
   license:
     name: Apache 2.0
   description: The API of Data Recovery Service for CDP Private Cloud Control Plane .
 schemes:
   - https
 consumes:
```

### Comparing `cdpcli-beta-0.9.88/cdpcli/data/dw/dw.yaml` & `cdpcli-beta-0.9.89/cdpcli/data/dw/dw.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 swagger: '2.0'
 x-endpoint-name: dw
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.88
+  version: 0.9.89
   title: Cloudera Data Warehouse [EXPERIMENTAL]
   license:
     name: Apache 2.0
   description: Install and manage Cloudera Data Warehouse clusters.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.88/cdpcli/data/environments/environments.yaml` & `cdpcli-beta-0.9.89/cdpcli/data/environments/environments.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: environments2
 x-display-name: environments
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.88
+  version: 0.9.89
   title: Cloudera Environments Service
   license:
     name: Apache 2.0
   description: Cloudera Environments Service is a web service that manages cloud provider access.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -1504,14 +1504,35 @@
           description: Expected response to a valid request.
           schema:
             $ref: '#/definitions/RotateSaltPasswordResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
+  /api/v1/environments2/updateOrchestratorState:
+    post:
+      summary: Run orchestrator engine state update on the FreeIPA cluster.
+      description: Run orchestrator engine state update on the FreeIPA cluster.
+      operationId: updateOrchestratorState
+      x-mutating: true
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/UpdateOrchestratorStateRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/UpdateOrchestratorStateResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
 definitions:
   Error:
     type: object
     description: An object returned on an error.
     properties:
       code:
         type: string
@@ -4869,7 +4890,19 @@
     properties:
       environment:
         type: string
         description: The name or CRN of the environment.
   RotateSaltPasswordResponse:
     type: object
     description: Response object for rotating SaltStack user password on FreeIPA instances.
+  UpdateOrchestratorStateRequest:
+    type: object
+    description: Request object for running orchestrator engine state update on the FreeIPA cluster.
+    required:
+      - environment
+    properties:
+      environment:
+        type: string
+        description: The name or CRN of the environment.
+  UpdateOrchestratorStateResponse:
+    type: object
+    description: Response object for running orchestrator engine state update on the FreeIPA cluster.
```

### Comparing `cdpcli-beta-0.9.88/cdpcli/data/iam/iam.yaml` & `cdpcli-beta-0.9.89/cdpcli/data/iam/iam.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: iam
 x-products: ALTUS,CDP
 x-form-factors: public,private
 x-altus-releases: PUBLIC
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.88
+  version: 0.9.89
   title: Cloudera IAM Service
   license:
     name: Apache 2.0
   description: Cloudera CDP IAM is a web service that you can use to manage users and user permissions under your CDP account.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.88/cdpcli/data/imagecatalog/imagecatalog.yaml` & `cdpcli-beta-0.9.89/cdpcli/data/imagecatalog/imagecatalog.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: imagecatalog
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.88
+  version: 0.9.89
   title: Image catalog service
   license:
     name: Apache 2.0
   description: Service for managing custom image catalogs and their associated Cloudera Runtime and FreeIPA images.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.88/cdpcli/data/ml/ml.yaml` & `cdpcli-beta-0.9.89/cdpcli/data/ml/ml.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: ml
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.88
+  version: 0.9.89
   title: Cloudera Machine Learning
   license:
     name: Apache 2.0
   description: Install and manage Cloudera Machine Learning applications.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.88/cdpcli/data/opdb/opdb.yaml` & `cdpcli-beta-0.9.89/cdpcli/data/opdb/opdb.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: opdb
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.88
+  version: 0.9.89
   title: Operational Database service
   license:
     name: Apache 2.0
   description: Interact with the Cloudera Operational Database service
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.88/cdpcli/data/replicationmanager/replicationmanager.yaml` & `cdpcli-beta-0.9.89/cdpcli/data/replicationmanager/replicationmanager.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: replicationmanager
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.88
+  version: 0.9.89
   title: Cloudera Replication Manager Service
   license:
     name: Apache 2.0
   description: Create and manage replication policies using Cloudera Replication Manager.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.88/cdpcli/doc/docstringparser.py` & `cdpcli-beta-0.9.89/cdpcli/doc/docstringparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/doc/restdoc.py` & `cdpcli-beta-0.9.89/cdpcli/doc/restdoc.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/doc/style.py` & `cdpcli-beta-0.9.89/cdpcli/doc/style.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/docs.py` & `cdpcli-beta-0.9.89/cdpcli/docs.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/endpoint.py` & `cdpcli-beta-0.9.89/cdpcli/endpoint.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/examples/configure/_description.rst` & `cdpcli-beta-0.9.89/cdpcli/examples/configure/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/examples/configure/get/_description.rst` & `cdpcli-beta-0.9.89/cdpcli/examples/configure/get/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/examples/configure/get/_examples.rst` & `cdpcli-beta-0.9.89/cdpcli/examples/configure/get/_examples.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/examples/configure/set/_description.rst` & `cdpcli-beta-0.9.89/cdpcli/examples/configure/set/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/examples/configure/set/_examples.rst` & `cdpcli-beta-0.9.89/cdpcli/examples/configure/set/_examples.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/exceptions.py` & `cdpcli-beta-0.9.89/cdpcli/exceptions.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/extensions/__init__.py` & `cdpcli-beta-0.9.89/cdpcli/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/extensions/arguments.py` & `cdpcli-beta-0.9.89/cdpcli/extensions/arguments.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/extensions/cliinputjson.py` & `cdpcli-beta-0.9.89/cdpcli/extensions/cliinputjson.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/extensions/commands.py` & `cdpcli-beta-0.9.89/cdpcli/extensions/commands.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/extensions/configure/__init__.py` & `cdpcli-beta-0.9.89/cdpcli/extensions/configure/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/extensions/configure/classify.py` & `cdpcli-beta-0.9.89/cdpcli/extensions/configure/classify.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/extensions/configure/configure.py` & `cdpcli-beta-0.9.89/cdpcli/extensions/configure/configure.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/extensions/configure/get.py` & `cdpcli-beta-0.9.89/cdpcli/extensions/configure/get.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/extensions/configure/list.py` & `cdpcli-beta-0.9.89/cdpcli/extensions/configure/list.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/extensions/configure/set.py` & `cdpcli-beta-0.9.89/cdpcli/extensions/configure/set.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/extensions/df/__init__.py` & `cdpcli-beta-0.9.89/cdpcli/extensions/df/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/extensions/df/createdeployment.py` & `cdpcli-beta-0.9.89/cdpcli/extensions/df/createdeployment.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/extensions/df/register.py` & `cdpcli-beta-0.9.89/cdpcli/extensions/df/register.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/extensions/generatecliskeleton.py` & `cdpcli-beta-0.9.89/cdpcli/extensions/generatecliskeleton.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/extensions/interactivelogin.py` & `cdpcli-beta-0.9.89/cdpcli/extensions/interactivelogin.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/extensions/logout.py` & `cdpcli-beta-0.9.89/cdpcli/extensions/logout.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/extensions/paginate.py` & `cdpcli-beta-0.9.89/cdpcli/extensions/paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/extensions/redirect.py` & `cdpcli-beta-0.9.89/cdpcli/extensions/redirect.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/extensions/refdoc.py` & `cdpcli-beta-0.9.89/cdpcli/extensions/refdoc.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/extensions/workload.py` & `cdpcli-beta-0.9.89/cdpcli/extensions/workload.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/extensions/writer.py` & `cdpcli-beta-0.9.89/cdpcli/extensions/writer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/formatter.py` & `cdpcli-beta-0.9.89/cdpcli/formatter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/help.py` & `cdpcli-beta-0.9.89/cdpcli/help.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/loader.py` & `cdpcli-beta-0.9.89/cdpcli/loader.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/main.py` & `cdpcli-beta-0.9.89/cdpcli/main.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/model.py` & `cdpcli-beta-0.9.89/cdpcli/model.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/paginate.py` & `cdpcli-beta-0.9.89/cdpcli/paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/paramfile.py` & `cdpcli-beta-0.9.89/cdpcli/paramfile.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/paramformfactor.py` & `cdpcli-beta-0.9.89/cdpcli/paramformfactor.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/parser.py` & `cdpcli-beta-0.9.89/cdpcli/parser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/retryhandler.py` & `cdpcli-beta-0.9.89/cdpcli/retryhandler.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/schema.py` & `cdpcli-beta-0.9.89/cdpcli/schema.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/serialize.py` & `cdpcli-beta-0.9.89/cdpcli/serialize.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/shorthand.py` & `cdpcli-beta-0.9.89/cdpcli/shorthand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/signers.py` & `cdpcli-beta-0.9.89/cdpcli/signers.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/table.py` & `cdpcli-beta-0.9.89/cdpcli/table.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/text.py` & `cdpcli-beta-0.9.89/cdpcli/text.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/textwriter.py` & `cdpcli-beta-0.9.89/cdpcli/textwriter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/thirdparty/six.py` & `cdpcli-beta-0.9.89/cdpcli/thirdparty/six.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/translate.py` & `cdpcli-beta-0.9.89/cdpcli/translate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/utils.py` & `cdpcli-beta-0.9.89/cdpcli/utils.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli/validate.py` & `cdpcli-beta-0.9.89/cdpcli/validate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/cdpcli_beta.egg-info/PKG-INFO` & `cdpcli-beta-0.9.89/cdpcli_beta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdpcli-beta
-Version: 0.9.88
+Version: 0.9.89
 Summary: Cloudera CDP Command Line Interface (BETA)
 Home-page: https://console.cdp.cloudera.com/
 Author: Cloudera, Inc.
 License: Apache License 2.0
 Description: # Cloudera CDP Command Line Interface
         
         This package provides a unified command line interface to the Cloudera Data
```

### Comparing `cdpcli-beta-0.9.88/cdpcli_beta.egg-info/SOURCES.txt` & `cdpcli-beta-0.9.89/cdpcli_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/setup.py` & `cdpcli-beta-0.9.89/setup.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/setup_common.py` & `cdpcli-beta-0.9.89/setup_common.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/__init__.py` & `cdpcli-beta-0.9.89/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/cdp/__init__.py` & `cdpcli-beta-0.9.89/tests/unit/cdp/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/extensions/__init__.py` & `cdpcli-beta-0.9.89/tests/unit/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/extensions/configure/test_classify.py` & `cdpcli-beta-0.9.89/tests/unit/extensions/configure/test_classify.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/extensions/configure/test_configure.py` & `cdpcli-beta-0.9.89/tests/unit/extensions/configure/test_configure.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/extensions/configure/test_get.py` & `cdpcli-beta-0.9.89/tests/unit/extensions/configure/test_get.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/extensions/configure/test_list.py` & `cdpcli-beta-0.9.89/tests/unit/extensions/configure/test_list.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/extensions/configure/test_set.py` & `cdpcli-beta-0.9.89/tests/unit/extensions/configure/test_set.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/extensions/df/test_createdeployment.py` & `cdpcli-beta-0.9.89/tests/unit/extensions/df/test_createdeployment.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/extensions/df/test_upload_file.py` & `cdpcli-beta-0.9.89/tests/unit/extensions/df/test_upload_file.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/extensions/test_cliinputjson.py` & `cdpcli-beta-0.9.89/tests/unit/extensions/test_cliinputjson.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/extensions/test_df.py` & `cdpcli-beta-0.9.89/tests/unit/extensions/test_df.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/extensions/test_generatecliskeleton.py` & `cdpcli-beta-0.9.89/tests/unit/extensions/test_generatecliskeleton.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/extensions/test_interactivelogin.py` & `cdpcli-beta-0.9.89/tests/unit/extensions/test_interactivelogin.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/extensions/test_logout.py` & `cdpcli-beta-0.9.89/tests/unit/extensions/test_logout.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/extensions/test_operation_extension.py` & `cdpcli-beta-0.9.89/tests/unit/extensions/test_operation_extension.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/extensions/test_paginate.py` & `cdpcli-beta-0.9.89/tests/unit/extensions/test_paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/extensions/test_redirect.py` & `cdpcli-beta-0.9.89/tests/unit/extensions/test_redirect.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/extensions/test_workload.py` & `cdpcli-beta-0.9.89/tests/unit/extensions/test_workload.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/extensions/test_writer.py` & `cdpcli-beta-0.9.89/tests/unit/extensions/test_writer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/test_argparser.py` & `cdpcli-beta-0.9.89/tests/unit/test_argparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/test_argprocess.py` & `cdpcli-beta-0.9.89/tests/unit/test_argprocess.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/test_auth.py` & `cdpcli-beta-0.9.89/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/test_cli_data.py` & `cdpcli-beta-0.9.89/tests/unit/test_cli_data.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/test_client.py` & `cdpcli-beta-0.9.89/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/test_completer.py` & `cdpcli-beta-0.9.89/tests/unit/test_completer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/test_credentials.py` & `cdpcli-beta-0.9.89/tests/unit/test_credentials.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/test_docs.py` & `cdpcli-beta-0.9.89/tests/unit/test_docs.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/test_endpoint.py` & `cdpcli-beta-0.9.89/tests/unit/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/test_help.py` & `cdpcli-beta-0.9.89/tests/unit/test_help.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/test_loaders.py` & `cdpcli-beta-0.9.89/tests/unit/test_loaders.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/test_model.py` & `cdpcli-beta-0.9.89/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/test_paginate.py` & `cdpcli-beta-0.9.89/tests/unit/test_paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/test_paramfile.py` & `cdpcli-beta-0.9.89/tests/unit/test_paramfile.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/test_protocol.py` & `cdpcli-beta-0.9.89/tests/unit/test_protocol.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/test_retryhandler.py` & `cdpcli-beta-0.9.89/tests/unit/test_retryhandler.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/test_shorthand.py` & `cdpcli-beta-0.9.89/tests/unit/test_shorthand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/test_signers.py` & `cdpcli-beta-0.9.89/tests/unit/test_signers.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/test_table_formatter.py` & `cdpcli-beta-0.9.89/tests/unit/test_table_formatter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/test_utils.py` & `cdpcli-beta-0.9.89/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/tests/unit/test_validate.py` & `cdpcli-beta-0.9.89/tests/unit/test_validate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.88/versioneer.py` & `cdpcli-beta-0.9.89/versioneer.py`

 * *Files identical despite different names*

