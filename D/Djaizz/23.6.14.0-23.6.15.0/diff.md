# Comparing `tmp/Djaizz-23.6.14.0.tar.gz` & `tmp/Djaizz-23.6.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Djaizz-23.6.14.0.tar", last modified: Wed Jun 14 21:54:48 2023, max compression
+gzip compressed data, was "Djaizz-23.6.15.0.tar", last modified: Thu Jun 15 17:48:56 2023, max compression
```

## Comparing `Djaizz-23.6.14.0.tar` & `Djaizz-23.6.15.0.tar`

### file list

```diff
@@ -1,182 +1,182 @@
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.393320 Djaizz-23.6.14.0/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1092 2023-02-09 04:49:59.000000 Djaizz-23.6.14.0/LICENSE
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     5702 2023-06-14 21:54:48.393090 Djaizz-23.6.14.0/PKG-INFO
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      187 2023-02-28 01:51:17.000000 Djaizz-23.6.14.0/README.md
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.302869 Djaizz-23.6.14.0/metadata/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     2584 2023-03-09 04:40:50.000000 Djaizz-23.6.14.0/metadata/classifiers
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       52 2023-02-28 04:56:41.000000 Djaizz-23.6.14.0/metadata/description
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       65 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/metadata/entry-points
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.304092 Djaizz-23.6.14.0/metadata/requirements/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     6282 2023-06-14 21:25:21.000000 Djaizz-23.6.14.0/metadata/requirements/base.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       16 2023-02-28 04:56:41.000000 Djaizz-23.6.14.0/metadata/requirements/build.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       40 2023-06-14 20:47:00.000000 Djaizz-23.6.14.0/metadata/requirements/dev.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      215 2023-06-14 21:42:52.000000 Djaizz-23.6.14.0/metadata/requirements/doc.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      225 2023-06-14 19:57:11.000000 Djaizz-23.6.14.0/metadata/requirements/lint.txt
--rwxr--r--   0 thevinhluong102   (501) staff       (20)       15 2023-02-28 04:56:41.000000 Djaizz-23.6.14.0/metadata/requirements/publish.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       85 2023-06-13 01:17:31.000000 Djaizz-23.6.14.0/metadata/requirements/test.txt
--rwxr-xr-x   0 thevinhluong102   (501) staff       (20)      150 2023-06-13 01:17:55.000000 Djaizz-23.6.14.0/metadata/requirements/viz.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       10 2023-06-14 20:00:31.000000 Djaizz-23.6.14.0/metadata/version
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     3129 2023-06-14 20:38:47.000000 Djaizz-23.6.14.0/pyproject.toml
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       38 2023-06-14 21:54:48.393384 Djaizz-23.6.14.0/setup.cfg
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.298295 Djaizz-23.6.14.0/src/
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.305152 Djaizz-23.6.14.0/src/Djaizz.egg-info/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     5702 2023-06-14 21:54:48.000000 Djaizz-23.6.14.0/src/Djaizz.egg-info/PKG-INFO
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     5814 2023-06-14 21:54:48.000000 Djaizz-23.6.14.0/src/Djaizz.egg-info/SOURCES.txt
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        1 2023-06-14 21:54:48.000000 Djaizz-23.6.14.0/src/Djaizz.egg-info/dependency_links.txt
--rwxr--r--   0 thevinhluong102   (501) staff       (20)       50 2023-06-14 21:54:48.000000 Djaizz-23.6.14.0/src/Djaizz.egg-info/entry_points.txt
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     3893 2023-06-14 21:54:48.000000 Djaizz-23.6.14.0/src/Djaizz.egg-info/requires.txt
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        7 2023-06-14 21:54:48.000000 Djaizz-23.6.14.0/src/Djaizz.egg-info/top_level.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        1 2023-03-01 01:27:25.000000 Djaizz-23.6.14.0/src/Djaizz.egg-info/zip-safe
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.306645 Djaizz-23.6.14.0/src/djaizz/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      300 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.307220 Djaizz-23.6.14.0/src/djaizz/client/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      270 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/client/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.309140 Djaizz-23.6.14.0/src/djaizz/data/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      873 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/data/admin.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.309786 Djaizz-23.6.14.0/src/djaizz/data/api/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      816 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/data/api/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.310254 Djaizz-23.6.14.0/src/djaizz/data/api/gql/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/api/gql/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.310426 Djaizz-23.6.14.0/src/djaizz/data/api/json/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/api/json/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.310595 Djaizz-23.6.14.0/src/djaizz/data/api/rest/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/api/rest/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     2703 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/data/apps.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.312795 Djaizz-23.6.14.0/src/djaizz/data/migrations/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     6026 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/migrations/0001_DataSchema_DataSet.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1730 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/migrations/0002_InDBJSONDataSet.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1537 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/migrations/0003_Django4.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/migrations/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.329470 Djaizz-23.6.14.0/src/djaizz/data/models/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1005 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      542 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/audio.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     8019 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/data/models/base.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      534 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/csv.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      534 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/hdf.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      542 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/image.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     2596 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/data/models/json.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      528 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/live_api.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      585 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/numpy.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      534 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/orc.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      595 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/pandas.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      550 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/parquet.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.334832 Djaizz-23.6.14.0/src/djaizz/data/models/public/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       37 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/public/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       35 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/public/gov.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       37 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/public/hugging_face.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       50 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/public/intl_dev.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       31 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/public/kaggle.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       35 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/public/tf.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       30 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/public/torch.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       51 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/public/weather.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      538 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/text.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      554 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/tfrecord.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      542 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/video.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      294 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/urls.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.337023 Djaizz-23.6.14.0/src/djaizz/model/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     2559 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/model/admin.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.341411 Djaizz-23.6.14.0/src/djaizz/model/api/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1821 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/model/api/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.342006 Djaizz-23.6.14.0/src/djaizz/model/api/gql/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/api/gql/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.342148 Djaizz-23.6.14.0/src/djaizz/model/api/json/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/api/json/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.342283 Djaizz-23.6.14.0/src/djaizz/model/api/rest/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/api/rest/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     3259 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/model/apps.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.349570 Djaizz-23.6.14.0/src/djaizz/model/migrations/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     3211 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/migrations/0001_AIModel.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     2941 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/migrations/0002_PreTrainedKerasImageNetClassifier.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)    18732 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/migrations/0003_PreTrainedHuggingFaceTransformers.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1226 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/migrations/0004_CloudAIService.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1237 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/migrations/0005_GoogleTranslate.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     8705 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/migrations/0006_Django4.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/migrations/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.358789 Djaizz-23.6.14.0/src/djaizz/model/models/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1867 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)    22789 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/base.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.360350 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      340 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.361069 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/amazon/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       56 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/amazon/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1021 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/base.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.362278 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/google/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      286 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/google/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     8461 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/google/translation.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.362545 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/hugging_face/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       58 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/hugging_face/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.363135 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/ibm_watson/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       56 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/ibm_watson/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.363567 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/meta/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       72 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/meta/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.365053 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/microsoft/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       61 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/microsoft/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.365594 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/wolfram_alpha/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       59 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/wolfram_alpha/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.366755 Djaizz-23.6.14.0/src/djaizz/model/models/ml/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1769 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1849 2023-06-06 18:00:24.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/base.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.374283 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1905 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     9221 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/audio_classification.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1205 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/base.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     8955 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/image_classification.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     9778 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/mask_filling.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     9748 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/object_detection.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)    10400 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/question_answering.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     8633 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/speech_recognition.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     9303 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/table_question_answering.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     9572 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/text2text_generation.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     8648 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/text_classification.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)    10268 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/text_generation.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     9509 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/text_summarization.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     8748 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/token_classification.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)    10158 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/translation.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)    10300 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/zero_shot_classification.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.375283 Djaizz-23.6.14.0/src/djaizz/model/models/ml/keras/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      386 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/keras/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     2127 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/keras/base.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.375759 Djaizz-23.6.14.0/src/djaizz/model/models/ml/keras/pre_trained/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      322 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/keras/pre_trained/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.376787 Djaizz-23.6.14.0/src/djaizz/model/models/ml/keras/pre_trained/vision/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      343 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/keras/pre_trained/vision/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)    12235 2023-06-06 18:00:24.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/keras/pre_trained/vision/image_classification.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1446 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/skl.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.377568 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      265 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      814 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/base.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.378052 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/pre_trained/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       46 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/pre_trained/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.379318 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/pre_trained/audio/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       61 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/pre_trained/audio/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       74 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/pre_trained/audio/text_to_speech.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.384334 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/pre_trained/vision/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       53 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/pre_trained/vision/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       68 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/pre_trained/vision/image_classification.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       71 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/pre_trained/vision/instance_segmentation.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       69 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/pre_trained/vision/keypoint_detection.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       67 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/pre_trained/vision/object_detection.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       70 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/pre_trained/vision/semantic_segmentation.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)       68 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/pre_trained/vision/video_classification.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.386250 Djaizz-23.6.14.0/src/djaizz/model/scripts/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      401 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/model/scripts/setup_google_cloud_ai_svcs.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)    19753 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/model/scripts/setup_pretrained_huggingface_models.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     8394 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/model/scripts/setup_pretrained_keras_models.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      705 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/model/urls.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     5267 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/views.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      838 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/urls.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.388759 Djaizz-23.6.14.0/src/djaizz/util/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1018 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/util/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.390666 Djaizz-23.6.14.0/src/djaizz/util/cli/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      735 2023-05-26 21:52:35.000000 Djaizz-23.6.14.0/src/djaizz/util/cli/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.392113 Djaizz-23.6.14.0/src/djaizz/util/cli/_server_files/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      554 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/util/cli/_server_files/asgi.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      426 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/util/cli/_server_files/manage.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      553 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/util/cli/_server_files/wsgi.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.392645 Djaizz-23.6.14.0/src/djaizz/util/cli/aws_eb/
--rwxr-xr-x   0 thevinhluong102   (501) staff       (20)    11074 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/util/cli/aws_eb/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1022 2023-06-14 19:36:12.000000 Djaizz-23.6.14.0/src/djaizz/util/cli/deps.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     4374 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/util/cli/run_cmd.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1310 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/util/git.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1261 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/util/pip.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1740 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/util/views.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.640157 Djaizz-23.6.15.0/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1092 2023-02-09 04:49:59.000000 Djaizz-23.6.15.0/LICENSE
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     5702 2023-06-15 17:48:56.639834 Djaizz-23.6.15.0/PKG-INFO
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      187 2023-02-28 01:51:17.000000 Djaizz-23.6.15.0/README.md
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.495182 Djaizz-23.6.15.0/metadata/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     2584 2023-03-09 04:40:50.000000 Djaizz-23.6.15.0/metadata/classifiers
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       52 2023-02-28 04:56:41.000000 Djaizz-23.6.15.0/metadata/description
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       65 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/metadata/entry-points
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.496548 Djaizz-23.6.15.0/metadata/requirements/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     6496 2023-06-15 17:26:24.000000 Djaizz-23.6.15.0/metadata/requirements/base.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       16 2023-02-28 04:56:41.000000 Djaizz-23.6.15.0/metadata/requirements/build.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       40 2023-06-14 20:47:00.000000 Djaizz-23.6.15.0/metadata/requirements/dev.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      215 2023-06-14 21:42:52.000000 Djaizz-23.6.15.0/metadata/requirements/doc.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      225 2023-06-14 19:57:11.000000 Djaizz-23.6.15.0/metadata/requirements/lint.txt
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)       15 2023-02-28 04:56:41.000000 Djaizz-23.6.15.0/metadata/requirements/publish.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       85 2023-06-13 01:17:31.000000 Djaizz-23.6.15.0/metadata/requirements/test.txt
+-rwxr-xr-x   0 thevinhluong102   (501) staff       (20)      150 2023-06-13 01:17:55.000000 Djaizz-23.6.15.0/metadata/requirements/viz.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       10 2023-06-15 17:26:33.000000 Djaizz-23.6.15.0/metadata/version
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     3129 2023-06-14 20:38:47.000000 Djaizz-23.6.15.0/pyproject.toml
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       38 2023-06-15 17:48:56.640246 Djaizz-23.6.15.0/setup.cfg
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.487714 Djaizz-23.6.15.0/src/
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.497726 Djaizz-23.6.15.0/src/Djaizz.egg-info/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     5702 2023-06-15 17:48:56.000000 Djaizz-23.6.15.0/src/Djaizz.egg-info/PKG-INFO
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     5814 2023-06-15 17:48:56.000000 Djaizz-23.6.15.0/src/Djaizz.egg-info/SOURCES.txt
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        1 2023-06-15 17:48:56.000000 Djaizz-23.6.15.0/src/Djaizz.egg-info/dependency_links.txt
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)       50 2023-06-15 17:48:56.000000 Djaizz-23.6.15.0/src/Djaizz.egg-info/entry_points.txt
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     3924 2023-06-15 17:48:56.000000 Djaizz-23.6.15.0/src/Djaizz.egg-info/requires.txt
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        7 2023-06-15 17:48:56.000000 Djaizz-23.6.15.0/src/Djaizz.egg-info/top_level.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        1 2023-03-01 01:27:25.000000 Djaizz-23.6.15.0/src/Djaizz.egg-info/zip-safe
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.500050 Djaizz-23.6.15.0/src/djaizz/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      300 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.500618 Djaizz-23.6.15.0/src/djaizz/client/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      270 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/client/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.502615 Djaizz-23.6.15.0/src/djaizz/data/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      873 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/data/admin.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.503120 Djaizz-23.6.15.0/src/djaizz/data/api/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      816 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/data/api/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.503618 Djaizz-23.6.15.0/src/djaizz/data/api/gql/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/api/gql/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.503771 Djaizz-23.6.15.0/src/djaizz/data/api/json/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/api/json/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.503898 Djaizz-23.6.15.0/src/djaizz/data/api/rest/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/api/rest/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     2703 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/data/apps.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.505876 Djaizz-23.6.15.0/src/djaizz/data/migrations/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     6026 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/migrations/0001_DataSchema_DataSet.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1730 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/migrations/0002_InDBJSONDataSet.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1537 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/migrations/0003_Django4.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/migrations/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.540875 Djaizz-23.6.15.0/src/djaizz/data/models/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1005 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      542 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/audio.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     8019 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/data/models/base.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      534 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/csv.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      534 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/hdf.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      542 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/image.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     2596 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/data/models/json.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      528 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/live_api.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      585 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/numpy.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      534 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/orc.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      595 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/pandas.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      550 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/parquet.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.554483 Djaizz-23.6.15.0/src/djaizz/data/models/public/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       37 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/public/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       35 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/public/gov.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       37 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/public/hugging_face.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       50 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/public/intl_dev.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       31 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/public/kaggle.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       35 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/public/tf.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       30 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/public/torch.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       51 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/public/weather.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      538 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/text.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      554 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/tfrecord.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      542 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/video.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      294 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/urls.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.557150 Djaizz-23.6.15.0/src/djaizz/model/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     2559 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/model/admin.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.558199 Djaizz-23.6.15.0/src/djaizz/model/api/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1821 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/model/api/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.558791 Djaizz-23.6.15.0/src/djaizz/model/api/gql/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/api/gql/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.558961 Djaizz-23.6.15.0/src/djaizz/model/api/json/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/api/json/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.559109 Djaizz-23.6.15.0/src/djaizz/model/api/rest/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/api/rest/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     3259 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/model/apps.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.583880 Djaizz-23.6.15.0/src/djaizz/model/migrations/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     3211 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/migrations/0001_AIModel.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     2941 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/migrations/0002_PreTrainedKerasImageNetClassifier.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)    18732 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/migrations/0003_PreTrainedHuggingFaceTransformers.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1226 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/migrations/0004_CloudAIService.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1237 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/migrations/0005_GoogleTranslate.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     8705 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/migrations/0006_Django4.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/migrations/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.584626 Djaizz-23.6.15.0/src/djaizz/model/models/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1867 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)    22789 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/base.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.586207 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      340 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.586665 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/amazon/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       56 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/amazon/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1021 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/base.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.587585 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/google/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      286 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/google/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     8461 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/google/translation.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.587995 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/hugging_face/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       58 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/hugging_face/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.588364 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/ibm_watson/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       56 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/ibm_watson/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.590230 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/meta/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       72 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/meta/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.590844 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/microsoft/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       61 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/microsoft/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.591227 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/wolfram_alpha/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       59 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/wolfram_alpha/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.593007 Djaizz-23.6.15.0/src/djaizz/model/models/ml/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1769 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1849 2023-06-06 18:00:24.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/base.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.604649 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1905 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     9221 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/audio_classification.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1205 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/base.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     8955 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/image_classification.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     9778 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/mask_filling.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     9748 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/object_detection.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)    10400 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/question_answering.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     8633 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/speech_recognition.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     9303 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/table_question_answering.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     9572 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/text2text_generation.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     8648 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/text_classification.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)    10268 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/text_generation.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     9509 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/text_summarization.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     8748 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/token_classification.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)    10158 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/translation.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)    10300 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/zero_shot_classification.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.606225 Djaizz-23.6.15.0/src/djaizz/model/models/ml/keras/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      386 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/keras/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     2127 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/keras/base.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.607055 Djaizz-23.6.15.0/src/djaizz/model/models/ml/keras/pre_trained/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      322 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/keras/pre_trained/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.608014 Djaizz-23.6.15.0/src/djaizz/model/models/ml/keras/pre_trained/vision/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      343 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/keras/pre_trained/vision/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)    12235 2023-06-06 18:00:24.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/keras/pre_trained/vision/image_classification.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1446 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/skl.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.610072 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      265 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      814 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/base.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.610708 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/pre_trained/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       46 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/pre_trained/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.612701 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/pre_trained/audio/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       61 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/pre_trained/audio/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       74 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/pre_trained/audio/text_to_speech.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.630737 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/pre_trained/vision/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       53 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/pre_trained/vision/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       68 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/pre_trained/vision/image_classification.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       71 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/pre_trained/vision/instance_segmentation.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       69 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/pre_trained/vision/keypoint_detection.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       67 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/pre_trained/vision/object_detection.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       70 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/pre_trained/vision/semantic_segmentation.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)       68 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/pre_trained/vision/video_classification.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.633707 Djaizz-23.6.15.0/src/djaizz/model/scripts/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      401 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/model/scripts/setup_google_cloud_ai_svcs.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)    19753 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/model/scripts/setup_pretrained_huggingface_models.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     8394 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/model/scripts/setup_pretrained_keras_models.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      705 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/model/urls.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     5267 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/views.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      838 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/urls.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.635117 Djaizz-23.6.15.0/src/djaizz/util/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1018 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/util/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.636557 Djaizz-23.6.15.0/src/djaizz/util/cli/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      735 2023-05-26 21:52:35.000000 Djaizz-23.6.15.0/src/djaizz/util/cli/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.638372 Djaizz-23.6.15.0/src/djaizz/util/cli/_server_files/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      554 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/util/cli/_server_files/asgi.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      426 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/util/cli/_server_files/manage.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      553 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/util/cli/_server_files/wsgi.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.639070 Djaizz-23.6.15.0/src/djaizz/util/cli/aws_eb/
+-rwxr-xr-x   0 thevinhluong102   (501) staff       (20)    11074 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/util/cli/aws_eb/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1065 2023-06-15 17:20:24.000000 Djaizz-23.6.15.0/src/djaizz/util/cli/deps.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     4374 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/util/cli/run_cmd.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1310 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/util/git.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1261 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/util/pip.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1740 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/util/views.py
```

### Comparing `Djaizz-23.6.14.0/LICENSE` & `Djaizz-23.6.15.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/PKG-INFO` & `Djaizz-23.6.15.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Djaizz
-Version: 23.6.14.0
+Version: 23.6.15.0
 Summary: Artificial Intelligence (AI) in Django Applications
 Author-email: "STEAM for Vietnam Foundation: AI, IoT & Robotics Educational Initiative" <Edu.AI@STEAMforVietNam.org>
 Maintainer-email: "STEAM for Vietnam Foundation: AI, IoT & Robotics Educational Initiative" <Edu.AI@STEAMforVietNam.org>
 License: MIT License
         
         Copyright (c) 2021 The Vinh LUONG (LƯƠNG Thế Vinh)
```

### Comparing `Djaizz-23.6.14.0/metadata/classifiers` & `Djaizz-23.6.15.0/metadata/classifiers`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/metadata/requirements/base.txt` & `Djaizz-23.6.15.0/metadata/requirements/base.txt`

 * *Files 2% similar despite different names*

```diff
@@ -256,15 +256,16 @@
 Channels >= 4.0.0
 Daphne >= 4.0.0
 GUnicorn >= 20.1.0
 H11 >= 0.9
   # let higher dependencies figure
 Hypercorn >= 0.14.3
 Quart >= 0.18.4
-Starlette >= 0.28.0
+Starlette >= 0.27
+  # let higher dependencies figure
 Uvicorn >= 0.22.0
 
 
 # COMMAND-LINE INTERFACE (CLI)
 # ============================
 CLICK >= 8.1.3
 Colored >= 1.4.4
@@ -306,7 +307,13 @@
 PSUtil >= 5.9.5
 Python-DateUtil >= 2.8.2
 Python-DotEnv >= 1.0.0
 PyTZ >= 2023.3
 Requests >= 2.31.0
 Ruamel.YAML >= 0.17.31
 Tqdm >= 4.65.0
+
+
+# INDIRECT DEPENDENCIES: explicitly specify to avoid outdated versions
+# ====================================================================
+FastAPI >= 0.97.0
+Pydantic >= 1.10.9
```

### Comparing `Djaizz-23.6.14.0/pyproject.toml` & `Djaizz-23.6.15.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/Djaizz.egg-info/PKG-INFO` & `Djaizz-23.6.15.0/src/Djaizz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Djaizz
-Version: 23.6.14.0
+Version: 23.6.15.0
 Summary: Artificial Intelligence (AI) in Django Applications
 Author-email: "STEAM for Vietnam Foundation: AI, IoT & Robotics Educational Initiative" <Edu.AI@STEAMforVietNam.org>
 Maintainer-email: "STEAM for Vietnam Foundation: AI, IoT & Robotics Educational Initiative" <Edu.AI@STEAMforVietNam.org>
 License: MIT License
         
         Copyright (c) 2021 The Vinh LUONG (LƯƠNG Thế Vinh)
```

### Comparing `Djaizz-23.6.14.0/src/Djaizz.egg-info/SOURCES.txt` & `Djaizz-23.6.15.0/src/Djaizz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/Djaizz.egg-info/requires.txt` & `Djaizz-23.6.15.0/src/Djaizz.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 ASGIRef>=3.7.2
 Channels>=4.0.0
 Daphne>=4.0.0
 GUnicorn>=20.1.0
 H11>=0.9
 Hypercorn>=0.14.3
 Quart>=0.18.4
-Starlette>=0.28.0
+Starlette>=0.27
 Uvicorn>=0.22.0
 CLICK>=8.1.3
 Colored>=1.4.4
 Jupyter>=1.0.0
 S3FS>=2023.6.0
 ADLFS>=2023.4.0
 GCSFS>=2023.6.0
@@ -149,14 +149,16 @@
 PSUtil>=5.9.5
 Python-DateUtil>=2.8.2
 Python-DotEnv>=1.0.0
 PyTZ>=2023.3
 Requests>=2.31.0
 Ruamel.YAML>=0.17.31
 Tqdm>=4.65.0
+FastAPI>=0.97.0
+Pydantic>=1.10.9
 
 [:python_version < "3.11"]
 Kedro>=0.18.10
 Ray>=2.5.0
 Giotto-TDA>=0.6.0
 CausalNex>=0.12.0
 Django-ForestAdmin>=1.5.0
```

### Comparing `Djaizz-23.6.14.0/src/djaizz/data/admin.py` & `Djaizz-23.6.15.0/src/djaizz/data/admin.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/data/api/__init__.py` & `Djaizz-23.6.15.0/src/djaizz/data/api/__init__.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/data/apps.py` & `Djaizz-23.6.15.0/src/djaizz/data/apps.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/data/migrations/0001_DataSchema_DataSet.py` & `Djaizz-23.6.15.0/src/djaizz/data/migrations/0001_DataSchema_DataSet.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/data/migrations/0002_InDBJSONDataSet.py` & `Djaizz-23.6.15.0/src/djaizz/data/migrations/0002_InDBJSONDataSet.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/data/migrations/0003_Django4.py` & `Djaizz-23.6.15.0/src/djaizz/data/migrations/0003_Django4.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/data/models/__init__.py` & `Djaizz-23.6.15.0/src/djaizz/data/models/__init__.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/data/models/audio.py` & `Djaizz-23.6.15.0/src/djaizz/data/models/audio.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/data/models/base.py` & `Djaizz-23.6.15.0/src/djaizz/data/models/base.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/data/models/csv.py` & `Djaizz-23.6.15.0/src/djaizz/data/models/csv.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/data/models/hdf.py` & `Djaizz-23.6.15.0/src/djaizz/data/models/hdf.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/data/models/image.py` & `Djaizz-23.6.15.0/src/djaizz/data/models/image.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/data/models/json.py` & `Djaizz-23.6.15.0/src/djaizz/data/models/json.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/data/models/live_api.py` & `Djaizz-23.6.15.0/src/djaizz/data/models/live_api.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/data/models/numpy.py` & `Djaizz-23.6.15.0/src/djaizz/data/models/numpy.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/data/models/orc.py` & `Djaizz-23.6.15.0/src/djaizz/data/models/orc.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/data/models/pandas.py` & `Djaizz-23.6.15.0/src/djaizz/data/models/pandas.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/data/models/parquet.py` & `Djaizz-23.6.15.0/src/djaizz/data/models/parquet.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/data/models/text.py` & `Djaizz-23.6.15.0/src/djaizz/data/models/text.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/data/models/tfrecord.py` & `Djaizz-23.6.15.0/src/djaizz/data/models/tfrecord.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/data/models/video.py` & `Djaizz-23.6.15.0/src/djaizz/data/models/video.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/admin.py` & `Djaizz-23.6.15.0/src/djaizz/model/admin.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/api/__init__.py` & `Djaizz-23.6.15.0/src/djaizz/model/api/__init__.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/apps.py` & `Djaizz-23.6.15.0/src/djaizz/model/apps.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/migrations/0001_AIModel.py` & `Djaizz-23.6.15.0/src/djaizz/model/migrations/0001_AIModel.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/migrations/0002_PreTrainedKerasImageNetClassifier.py` & `Djaizz-23.6.15.0/src/djaizz/model/migrations/0002_PreTrainedKerasImageNetClassifier.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/migrations/0003_PreTrainedHuggingFaceTransformers.py` & `Djaizz-23.6.15.0/src/djaizz/model/migrations/0003_PreTrainedHuggingFaceTransformers.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/migrations/0004_CloudAIService.py` & `Djaizz-23.6.15.0/src/djaizz/model/migrations/0004_CloudAIService.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/migrations/0005_GoogleTranslate.py` & `Djaizz-23.6.15.0/src/djaizz/model/migrations/0005_GoogleTranslate.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/migrations/0006_Django4.py` & `Djaizz-23.6.15.0/src/djaizz/model/migrations/0006_Django4.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/models/__init__.py` & `Djaizz-23.6.15.0/src/djaizz/model/models/__init__.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/models/base.py` & `Djaizz-23.6.15.0/src/djaizz/model/models/base.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/base.py` & `Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/base.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/google/translation.py` & `Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/google/translation.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/models/ml/__init__.py` & `Djaizz-23.6.15.0/src/djaizz/model/models/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/models/ml/base.py` & `Djaizz-23.6.15.0/src/djaizz/model/models/ml/base.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/__init__.py` & `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/__init__.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/audio_classification.py` & `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/audio_classification.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/base.py` & `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/base.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/image_classification.py` & `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/image_classification.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/mask_filling.py` & `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/mask_filling.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/object_detection.py` & `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/object_detection.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/question_answering.py` & `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/question_answering.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/speech_recognition.py` & `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/speech_recognition.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/table_question_answering.py` & `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/table_question_answering.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/text2text_generation.py` & `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/text2text_generation.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/text_classification.py` & `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/text_classification.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/text_generation.py` & `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/text_generation.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/text_summarization.py` & `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/text_summarization.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/token_classification.py` & `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/token_classification.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/translation.py` & `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/translation.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/zero_shot_classification.py` & `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/zero_shot_classification.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/models/ml/keras/base.py` & `Djaizz-23.6.15.0/src/djaizz/model/models/ml/keras/base.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/models/ml/keras/pre_trained/vision/image_classification.py` & `Djaizz-23.6.15.0/src/djaizz/model/models/ml/keras/pre_trained/vision/image_classification.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/models/ml/skl.py` & `Djaizz-23.6.15.0/src/djaizz/model/models/ml/skl.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/base.py` & `Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/base.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/scripts/setup_pretrained_huggingface_models.py` & `Djaizz-23.6.15.0/src/djaizz/model/scripts/setup_pretrained_huggingface_models.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/scripts/setup_pretrained_keras_models.py` & `Djaizz-23.6.15.0/src/djaizz/model/scripts/setup_pretrained_keras_models.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/urls.py` & `Djaizz-23.6.15.0/src/djaizz/model/urls.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/model/views.py` & `Djaizz-23.6.15.0/src/djaizz/model/views.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/urls.py` & `Djaizz-23.6.15.0/src/djaizz/urls.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/util/__init__.py` & `Djaizz-23.6.15.0/src/djaizz/util/__init__.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/util/cli/__init__.py` & `Djaizz-23.6.15.0/src/djaizz/util/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/util/cli/_server_files/asgi.py` & `Djaizz-23.6.15.0/src/djaizz/util/cli/_server_files/asgi.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/util/cli/_server_files/wsgi.py` & `Djaizz-23.6.15.0/src/djaizz/util/cli/_server_files/wsgi.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/util/cli/aws_eb/__init__.py` & `Djaizz-23.6.15.0/src/djaizz/util/cli/aws_eb/__init__.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/util/cli/deps.py` & `Djaizz-23.6.15.0/src/djaizz/util/cli/deps.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 import click
 
 
 CAPPED_DEPS: Sequence[str] = ('Dash',
                               'H11',
                               'NumPy',
-                              'Pandas')
+                              'Pandas',
+                              'Starlette')
 
 
 @click.command(name='capped-deps',
                cls=click.Command,
                context_settings=None,
                help=('Djaizz Capped Dependencies CLI >>>'),
                epilog=('^^^ Djaizz Capped Dependencies CLI'),
```

### Comparing `Djaizz-23.6.14.0/src/djaizz/util/cli/run_cmd.py` & `Djaizz-23.6.15.0/src/djaizz/util/cli/run_cmd.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/util/git.py` & `Djaizz-23.6.15.0/src/djaizz/util/git.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/util/pip.py` & `Djaizz-23.6.15.0/src/djaizz/util/pip.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.14.0/src/djaizz/util/views.py` & `Djaizz-23.6.15.0/src/djaizz/util/views.py`

 * *Files identical despite different names*

