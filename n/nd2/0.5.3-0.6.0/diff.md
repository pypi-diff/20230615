# Comparing `tmp/nd2-0.5.3.tar.gz` & `tmp/nd2-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nd2-0.5.3.tar", last modified: Fri Dec  9 16:42:30 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `nd2-0.5.3.tar` & `nd2-0.6.0.tar`

### file list

```diff
@@ -1,85 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-09 16:42:30.983221 nd2-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (122)      677 2022-12-09 16:32:19.000000 nd2-0.5.3/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (122)      268 2022-12-09 16:32:19.000000 nd2-0.5.3/.github_changelog_generator
--rw-r--r--   0 runner    (1001) docker     (122)     1413 2022-12-09 16:32:19.000000 nd2-0.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)    14639 2022-12-09 16:32:19.000000 nd2-0.5.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1744 2022-12-09 16:32:19.000000 nd2-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      434 2022-12-09 16:32:19.000000 nd2-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    30322 2022-12-09 16:42:30.983221 nd2-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    29458 2022-12-09 16:32:19.000000 nd2-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     5823 2022-12-09 16:32:19.000000 nd2-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-09 16:42:30.983221 nd2-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1903 2022-12-09 16:32:19.000000 nd2-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-09 16:42:30.947221 nd2-0.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-09 16:42:30.951221 nd2-0.5.3/src/nd2/
--rw-r--r--   0 runner    (1001) docker     (122)      578 2022-12-09 16:32:19.000000 nd2-0.5.3/src/nd2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8356 2022-12-09 16:32:19.000000 nd2-0.5.3/src/nd2/_binary.py
--rw-r--r--   0 runner    (1001) docker     (122)    12229 2022-12-09 16:32:19.000000 nd2-0.5.3/src/nd2/_chunkmap.py
--rw-r--r--   0 runner    (1001) docker     (122)    13005 2022-12-09 16:32:19.000000 nd2-0.5.3/src/nd2/_legacy.py
--rw-r--r--   0 runner    (1001) docker     (122)     4616 2022-12-09 16:32:19.000000 nd2-0.5.3/src/nd2/_nd2decode.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-09 16:42:30.955221 nd2-0.5.3/src/nd2/_sdk/
--rw-r--r--   0 runner    (1001) docker     (122)       43 2022-12-09 16:32:19.000000 nd2-0.5.3/src/nd2/_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2774 2022-12-09 16:32:19.000000 nd2-0.5.3/src/nd2/_sdk/latest.pxd
--rw-r--r--   0 runner    (1001) docker     (122)     2034 2022-12-09 16:32:19.000000 nd2-0.5.3/src/nd2/_sdk/latest.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    15546 2022-12-09 16:32:19.000000 nd2-0.5.3/src/nd2/_sdk/latest.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     3401 2022-12-09 16:32:19.000000 nd2-0.5.3/src/nd2/_util.py
--rw-r--r--   0 runner    (1001) docker     (122)      176 2022-12-09 16:42:30.000000 nd2-0.5.3/src/nd2/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     2307 2022-12-09 16:32:19.000000 nd2-0.5.3/src/nd2/_xml.py
--rw-r--r--   0 runner    (1001) docker     (122)    32806 2022-12-09 16:32:19.000000 nd2-0.5.3/src/nd2/nd2file.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-09 16:32:19.000000 nd2-0.5.3/src/nd2/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    10949 2022-12-09 16:32:19.000000 nd2-0.5.3/src/nd2/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-09 16:42:30.951221 nd2-0.5.3/src/nd2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    30322 2022-12-09 16:42:30.000000 nd2-0.5.3/src/nd2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1812 2022-12-09 16:42:30.000000 nd2-0.5.3/src/nd2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-09 16:42:30.000000 nd2-0.5.3/src/nd2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-09 16:41:52.000000 nd2-0.5.3/src/nd2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      620 2022-12-09 16:42:30.000000 nd2-0.5.3/src/nd2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        4 2022-12-09 16:42:30.000000 nd2-0.5.3/src/nd2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-09 16:42:30.955221 nd2-0.5.3/src/sdk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-09 16:42:30.947221 nd2-0.5.3/src/sdk/Darwin/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-09 16:42:30.947221 nd2-0.5.3/src/sdk/Darwin/arm64/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-09 16:42:30.955221 nd2-0.5.3/src/sdk/Darwin/arm64/include/
--rw-r--r--   0 runner    (1001) docker     (122)    26158 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Darwin/arm64/include/Nd2ReadSdk.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-09 16:42:30.959221 nd2-0.5.3/src/sdk/Darwin/arm64/lib/
--rwxr-xr-x   0 runner    (1001) docker     (122)    50632 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Darwin/arm64/lib/libjbig.a
--rwxr-xr-x   0 runner    (1001) docker     (122)   344448 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Darwin/arm64/lib/libjpeg.a
--rwxr-xr-x   0 runner    (1001) docker     (122)  2770416 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Darwin/arm64/lib/liblimfile.a
--rwxr-xr-x   0 runner    (1001) docker     (122)   222736 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Darwin/arm64/lib/liblzma.a
--rw-r--r--   0 runner    (1001) docker     (122)   317128 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Darwin/arm64/lib/libnd2readsdk-static.a
--rwxr-xr-x   0 runner    (1001) docker     (122)   583400 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Darwin/arm64/lib/libtiff.a
--rwxr-xr-x   0 runner    (1001) docker     (122)    10968 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Darwin/arm64/lib/libtiffxx.a
--rwxr-xr-x   0 runner    (1001) docker     (122)   108200 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Darwin/arm64/lib/libz.a
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-09 16:42:30.947221 nd2-0.5.3/src/sdk/Darwin/x86_64/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-09 16:42:30.959221 nd2-0.5.3/src/sdk/Darwin/x86_64/include/
--rw-r--r--   0 runner    (1001) docker     (122)    26158 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Darwin/x86_64/include/Nd2ReadSdk.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-09 16:42:30.963221 nd2-0.5.3/src/sdk/Darwin/x86_64/lib/
--rwxr-xr-x   0 runner    (1001) docker     (122)    61440 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Darwin/x86_64/lib/libjbig.a
--rwxr-xr-x   0 runner    (1001) docker     (122)   373272 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Darwin/x86_64/lib/libjpeg.a
--rwxr-xr-x   0 runner    (1001) docker     (122)  2803480 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Darwin/x86_64/lib/liblimfile.a
--rwxr-xr-x   0 runner    (1001) docker     (122)   247800 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Darwin/x86_64/lib/liblzma.a
--rw-r--r--   0 runner    (1001) docker     (122)   355440 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Darwin/x86_64/lib/libnd2readsdk-static.a
--rwxr-xr-x   0 runner    (1001) docker     (122)   624384 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Darwin/x86_64/lib/libtiff.a
--rwxr-xr-x   0 runner    (1001) docker     (122)    11272 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Darwin/x86_64/lib/libtiffxx.a
--rwxr-xr-x   0 runner    (1001) docker     (122)   117624 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Darwin/x86_64/lib/libz.a
--rw-r--r--   0 runner    (1001) docker     (122)      555 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-09 16:42:30.947221 nd2-0.5.3/src/sdk/Linux/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-09 16:42:30.951221 nd2-0.5.3/src/sdk/Linux/x86_64/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-09 16:42:30.963221 nd2-0.5.3/src/sdk/Linux/x86_64/include/
--rw-r--r--   0 runner    (1001) docker     (122)    26158 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Linux/x86_64/include/Nd2ReadSdk.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-09 16:42:30.967221 nd2-0.5.3/src/sdk/Linux/x86_64/lib/
--rwxr-xr-x   0 runner    (1001) docker     (122)  2246416 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Linux/x86_64/lib/liblimfile.so
--rw-r--r--   0 runner    (1001) docker     (122)   419352 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Linux/x86_64/lib/libnd2readsdk-shared.so
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-09 16:42:30.951221 nd2-0.5.3/src/sdk/Windows/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-09 16:42:30.951221 nd2-0.5.3/src/sdk/Windows/x86_64/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-09 16:42:30.967221 nd2-0.5.3/src/sdk/Windows/x86_64/include/
--rw-r--r--   0 runner    (1001) docker     (122)    26158 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Windows/x86_64/include/Nd2ReadSdk.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-09 16:42:30.983221 nd2-0.5.3/src/sdk/Windows/x86_64/lib/
--rw-r--r--   0 runner    (1001) docker     (122)    74720 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Windows/x86_64/lib/jbig.lib
--rw-r--r--   0 runner    (1001) docker     (122)   469244 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Windows/x86_64/lib/libjpeg.lib
--rw-r--r--   0 runner    (1001) docker     (122) 12157896 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Windows/x86_64/lib/limfile.lib
--rw-r--r--   0 runner    (1001) docker     (122)  1128356 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Windows/x86_64/lib/lzma.lib
--rw-r--r--   0 runner    (1001) docker     (122)   444418 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Windows/x86_64/lib/nd2readsdk-static.lib
--rw-r--r--   0 runner    (1001) docker     (122)  1176986 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Windows/x86_64/lib/tiff.lib
--rw-r--r--   0 runner    (1001) docker     (122)    17790 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Windows/x86_64/lib/tiffxx.lib
--rw-r--r--   0 runner    (1001) docker     (122)   178860 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/Windows/x86_64/lib/zlib.lib
--rw-r--r--   0 runner    (1001) docker     (122)       65 2022-12-09 16:32:19.000000 nd2-0.5.3/src/sdk/version.txt
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nd2-0.6.0/.github_changelog_generator
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 nd2-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    16851 2020-02-02 00:00:00.000000 nd2-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 nd2-0.6.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 nd2-0.6.0/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 nd2-0.6.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 nd2-0.6.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 nd2-0.6.0/.github/workflows/cron.yml
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 nd2-0.6.0/scripts/bf_describe.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 nd2-0.6.0/scripts/compare.py
+-rw-r--r--   0        0        0    23338 2020-02-02 00:00:00.000000 nd2-0.6.0/scripts/comparison.json
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 nd2-0.6.0/scripts/download_samples.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 nd2-0.6.0/scripts/gather.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 nd2-0.6.0/scripts/nd2_describe.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/__init__.py
+-rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/_binary.py
+-rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/_clx_lite.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/_clx_xml.py
+-rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/_util.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/_version.py
+-rw-r--r--   0        0        0    29445 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/nd2file.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/py.typed
+-rw-r--r--   0        0        0    12135 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/structures.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/_legacy/__init__.py
+-rw-r--r--   0        0        0    11849 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/_legacy/_legacy.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/_legacy/_legacy_xml.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/_pysdk/__init__.py
+-rw-r--r--   0        0        0    14676 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/_pysdk/_chunk_decode.py
+-rw-r--r--   0        0        0    22012 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/_pysdk/_parse.py
+-rw-r--r--   0        0        0    18816 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/_pysdk/_pysdk.py
+-rw-r--r--   0        0        0    14497 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/_pysdk/_sdk_types.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/conftest.py
+-rw-r--r--   0        0        0  5234229 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/readlim_output.json
+-rw-r--r--   0        0        0   513829 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/samples_metadata.json
+-rw-r--r--   0        0        0     6728 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/test_aicsimage.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/test_binary.py
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/test_dask_dispatch.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/test_deprecations.py
+-rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/test_metadata.py
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/test_parse.py
+-rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/test_reader.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/test_readme.py
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/test_rescue.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/test_rois.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/test_segfaults.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/test_xml.py
+-rw-r--r--   0        0        0    34639 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/variant.xml
+-rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/variant_CustomDataV2_0.xml
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 nd2-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 nd2-0.6.0/LICENSE
+-rw-r--r--   0        0        0    30192 2020-02-02 00:00:00.000000 nd2-0.6.0/README.md
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 nd2-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    32443 2020-02-02 00:00:00.000000 nd2-0.6.0/PKG-INFO
```

### Comparing `nd2-0.5.3/.gitignore` & `nd2-0.6.0/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 sdist/
 var/
 wheels/
 *.egg-info/
 .installed.cfg
 *.egg
 
+.DS_Store
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
 *.manifest
 *.spec
 
 # Installer logs
@@ -105,15 +106,12 @@
 .vscode/
 
 tests/data
 wheelhouse
 src/nd2/_nd2file.c
 src/nd2/_nd2file_legacy.c
 src/nd2/_version.py
-src/nd2/_sdk/picture.c
-src/nd2/_sdk/v9.c
-src/nd2/_sdk/latest.c
 
 # allow these
 !src/sdk/**/*.so
 !src/sdk/**/lib/
 !src/sdk/**/*.a
```

### Comparing `nd2-0.5.3/CHANGELOG.md` & `nd2-0.6.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,47 @@
 # Changelog
 
-## [0.5.2](https://github.com/tlambert03/nd2/tree/0.5.2) (2022-12-08)
+## [0.6.0](https://github.com/tlambert03/nd2/tree/0.6.0) (2023-06-15)
 
-[Full Changelog](https://github.com/tlambert03/nd2/compare/v0.5.1...0.5.2)
+[Full Changelog](https://github.com/tlambert03/nd2/compare/v0.5.3...0.6.0)
+
+**Implemented enhancements:**
+
+- feat: Remove sdk, use all python [\#135](https://github.com/tlambert03/nd2/pull/135) ([tlambert03](https://github.com/tlambert03))
+
+**Fixed bugs:**
+
+- fix: Make 'periodDiff' optional in TimeLoopParams construction [\#131](https://github.com/tlambert03/nd2/pull/131) ([SeanLeRoy](https://github.com/SeanLeRoy))
+
+**Tests & CI:**
+
+- feat: add more typed dicts to parsing [\#139](https://github.com/tlambert03/nd2/pull/139) ([tlambert03](https://github.com/tlambert03))
+- ci: enable Strict mypy typing [\#138](https://github.com/tlambert03/nd2/pull/138) ([tlambert03](https://github.com/tlambert03))
+- test: update rescue test [\#137](https://github.com/tlambert03/nd2/pull/137) ([tlambert03](https://github.com/tlambert03))
+
+**Merged pull requests:**
+
+- refactor: cleaning up reader [\#141](https://github.com/tlambert03/nd2/pull/141) ([tlambert03](https://github.com/tlambert03))
+- chore: adding nd2\_describe script [\#136](https://github.com/tlambert03/nd2/pull/136) ([tlambert03](https://github.com/tlambert03))
+- ci\(dependabot\): bump pypa/cibuildwheel from 2.12.1 to 2.12.3 [\#130](https://github.com/tlambert03/nd2/pull/130) ([dependabot[bot]](https://github.com/apps/dependabot))
+- ci\(dependabot\): bump pypa/cibuildwheel from 2.12.0 to 2.12.1 [\#128](https://github.com/tlambert03/nd2/pull/128) ([dependabot[bot]](https://github.com/apps/dependabot))
+- ci\(dependabot\): bump pypa/cibuildwheel from 2.11.3 to 2.12.0 [\#125](https://github.com/tlambert03/nd2/pull/125) ([dependabot[bot]](https://github.com/apps/dependabot))
+- ci\(dependabot\): bump pypa/cibuildwheel from 2.11.2 to 2.11.3 [\#120](https://github.com/tlambert03/nd2/pull/120) ([dependabot[bot]](https://github.com/apps/dependabot))
+
+## [v0.5.3](https://github.com/tlambert03/nd2/tree/v0.5.3) (2022-12-08)
+
+[Full Changelog](https://github.com/tlambert03/nd2/compare/v0.5.2...v0.5.3)
+
+**Merged pull requests:**
+
+- fix: catch exception on file open and release handle [\#117](https://github.com/tlambert03/nd2/pull/117) ([tlambert03](https://github.com/tlambert03))
+
+## [v0.5.2](https://github.com/tlambert03/nd2/tree/v0.5.2) (2022-12-08)
+
+[Full Changelog](https://github.com/tlambert03/nd2/compare/v0.5.1...v0.5.2)
 
 **Fixed bugs:**
 
 - fix: close handles on object deletion [\#116](https://github.com/tlambert03/nd2/pull/116) ([tlambert03](https://github.com/tlambert03))
 
 **Merged pull requests:**
 
@@ -100,15 +135,15 @@
 
 **Implemented enhancements:**
 
 - feat: Add native macosx-arm64 \(M1\) support [\#87](https://github.com/tlambert03/nd2/pull/87) ([tlambert03](https://github.com/tlambert03))
 
 **Fixed bugs:**
 
-- fix: Typo in legacy requirements [\#79](https://github.com/tlambert03/nd2/pull/79) ([c0deizbae](https://github.com/c0deizbae))
+- fix: Typo in legacy requirements [\#79](https://github.com/tlambert03/nd2/pull/79) ([ghost](https://github.com/ghost))
 
 **Merged pull requests:**
 
 - ci\(dependabot\): bump pypa/cibuildwheel from 2.8.1 to 2.9.0 [\#84](https://github.com/tlambert03/nd2/pull/84) ([dependabot[bot]](https://github.com/apps/dependabot))
 - ci\(dependabot\): bump pypa/cibuildwheel from 2.8.0 to 2.8.1 [\#81](https://github.com/tlambert03/nd2/pull/81) ([dependabot[bot]](https://github.com/apps/dependabot))
 - ci\(dependabot\): bump pypa/cibuildwheel from 2.7.0 to 2.8.0 [\#80](https://github.com/tlambert03/nd2/pull/80) ([dependabot[bot]](https://github.com/apps/dependabot))
 
@@ -186,34 +221,34 @@
 
 **Merged pull requests:**
 
 - update SDK license [\#43](https://github.com/tlambert03/nd2/pull/43) ([tlambert03](https://github.com/tlambert03))
 
 ## [v0.2.0](https://github.com/tlambert03/nd2/tree/v0.2.0) (2022-02-20)
 
-[Full Changelog](https://github.com/tlambert03/nd2/compare/v0.1.6...v0.2.0)
+[Full Changelog](https://github.com/tlambert03/nd2/compare/v0.1.5-1...v0.2.0)
 
 **Merged pull requests:**
 
 - add gh release action [\#42](https://github.com/tlambert03/nd2/pull/42) ([tlambert03](https://github.com/tlambert03))
 - make 2 utils public [\#41](https://github.com/tlambert03/nd2/pull/41) ([tlambert03](https://github.com/tlambert03))
 - Use resource-backed-dask-array, copy dask chunks by default [\#40](https://github.com/tlambert03/nd2/pull/40) ([tlambert03](https://github.com/tlambert03))
 - \[pre-commit.ci\] pre-commit autoupdate [\#37](https://github.com/tlambert03/nd2/pull/37) ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
 - \[pre-commit.ci\] pre-commit autoupdate [\#36](https://github.com/tlambert03/nd2/pull/36) ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
 - \[pre-commit.ci\] pre-commit autoupdate [\#35](https://github.com/tlambert03/nd2/pull/35) ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
 - \[pre-commit.ci\] pre-commit autoupdate [\#34](https://github.com/tlambert03/nd2/pull/34) ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
 - \[pre-commit.ci\] pre-commit autoupdate [\#33](https://github.com/tlambert03/nd2/pull/33) ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
 
-## [v0.1.6](https://github.com/tlambert03/nd2/tree/v0.1.6) (2021-11-12)
+## [v0.1.5-1](https://github.com/tlambert03/nd2/tree/v0.1.5-1) (2021-11-12)
 
-[Full Changelog](https://github.com/tlambert03/nd2/compare/v0.1.5-1...v0.1.6)
+[Full Changelog](https://github.com/tlambert03/nd2/compare/v0.1.6...v0.1.5-1)
 
-## [v0.1.5-1](https://github.com/tlambert03/nd2/tree/v0.1.5-1) (2021-11-12)
+## [v0.1.6](https://github.com/tlambert03/nd2/tree/v0.1.6) (2021-11-12)
 
-[Full Changelog](https://github.com/tlambert03/nd2/compare/v0.1.5...v0.1.5-1)
+[Full Changelog](https://github.com/tlambert03/nd2/compare/v0.1.5...v0.1.6)
 
 ## [v0.1.5](https://github.com/tlambert03/nd2/tree/v0.1.5) (2021-11-12)
 
 [Full Changelog](https://github.com/tlambert03/nd2/compare/v0.1.4...v0.1.5)
 
 **Merged pull requests:**
```

### Comparing `nd2-0.5.3/LICENSE` & `nd2-0.6.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,8 @@
-ND2 SDK libraries are distributed by permission of Mirek Svoboda,
-Laboratory Imaging, Inc.  (see LICENSE file in sdk folder)
-https://www.lim.cz/
-https://www.nd2sdk.com
-
-
-The remainder of the code is distributed under the following BSD License
-
-Copyright (c) 2021, Talley Lambert
-All rights reserved.
+Copyright (c) 2021 Talley Lambert
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `nd2-0.5.3/PKG-INFO` & `nd2-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,70 +1,65 @@
-Metadata-Version: 2.1
-Name: nd2
-Version: 0.5.3
-Summary: Yet another nd2 (Nikon NIS Elements) file reader
-Author: Talley Lambert
-Author-email: talley.lambert@gmail.com
-License: BSD 3-Clause License
-Project-URL: homepage, https://github.com/tlambert03/nd2
-Project-URL: repository, https://github.com/tlambert03/nd2
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: <3.12,>=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: legacy
-Provides-Extra: test
-Provides-Extra: dev
-License-File: LICENSE
-
 # nd2
 
 [![License](https://img.shields.io/pypi/l/nd2.svg?color=green)](https://github.com/tlambert03/nd2/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/nd2.svg?color=green)](https://pypi.org/project/nd2)
 [![Python Version](https://img.shields.io/pypi/pyversions/nd2.svg?color=green)](https://python.org)
 [![Tests](https://github.com/tlambert03/nd2/actions/workflows/ci.yml/badge.svg)](https://github.com/tlambert03/nd2/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/tlambert03/nd2/branch/main/graph/badge.svg)](https://codecov.io/gh/tlambert03/nd2)
 
-Yet another `.nd2` (Nikon NIS Elements) file reader.
-
-This reader provides a Cython wrapper for the official Nikon SDK.
-(The actual reading of image frames, however, uses a direct memmap approach, instead of the SDK,
-for performance reasons and to avoid occasional segfaults from the SDK.)
+`.nd2` (Nikon NIS Elements) file reader.
 
-Features good metadata retrieval, and direct `to_dask` and `to_xarray` options for lazy and/or annotated arrays.
+This reader provides a pure python implementation the official Nikon ND2 SDK.
 
-This library is tested against many nd2 files with the goal of maximizing compatibility and data extraction.
-(If you find an nd2 file that fails in some way, please open an issue with the file!)
+> It *used* to wrap the official SDK with Cython, but has since been completely
+> rewritten to be pure python (for performance, ease of distribution, and
+> maintenance) while retaining complete API parity with the official SDK.
+>
+> **Note:** This library is not affiliated with Nikon in any way, but we are
+> grateful for assistance from the SDK developers at Laboratory Imaging.
+
+Features good metadata retrieval, and direct `to_dask` and `to_xarray` options
+for lazy and/or annotated arrays.
+
+This library is tested against many nd2 files with the goal of maximizing
+compatibility and data extraction. (If you find an nd2 file that fails in some
+way, please [open an issue](https://github.com/tlambert03/nd2/issues/new) with
+the file!)
 
 ## install
 
 ```sh
 pip install nd2
 ```
 
 or from conda:
 
 ```sh
 conda install -c conda-forge nd2
 ```
 
-### extras
+### Legacy nd2 file support
 
-Legacy nd2 (JPEG2000) files are also supported, but require `imagecodecs`.  To install with support for these files use:
+Legacy nd2 (JPEG2000) files are also supported, but require `imagecodecs`.  To
+install with support for these files use the `legacy` extra:
 
 ```sh
 pip install nd2[legacy]
 ```
 
+### Faster XML parsing
+
+Much of the metadata in the file stored as XML.  If found in the environment,
+`nd2` will use [`lxml`](https://pypi.org/project/lxml/) which is much faster
+than the built-in `xml` module.  To install with support for `lxml` use:
+
+```sh
+pip install nd2 lxml
+```
+
 ## usage and API
 
 ```python
 import nd2
 import numpy as np
 
 my_array = nd2.imread('some_file.nd2')                          # read to numpy array
@@ -113,14 +108,15 @@
 f.recorded_data     # returns a dict of lists (passable to pandas.DataFrame) that
                     # the tabular "Recorded Data" view from in NIS Elements/Viewer
                     # with info for each frame in the experiment.
 
 # allll the metadata we can find...
 # no attempt made to standardize or parse it
 # look in here if you're searching for metdata that isn't exposed in the above
+# but try not to rely on it, as it's not guaranteed to be stable
 f.unstructured_metadata()
 
 f.close()           # don't forget to close when not using a contet manager!
 f.closed            # boolean, whether the file is closed
 ```
 
 ## Metadata structures
@@ -702,15 +698,14 @@
 ```python
 >>> binary_layer = binary_layers[0]
 >>> np.asarray(binary_layer)
 ```
 
 </details>
 
-
 ## Contributing / Development
 
 To test locally and contribute.  Clone this repo, then:
 
 ```
 pip install -e .[dev]
 ```
@@ -728,18 +723,26 @@
 pytest
 ```
 
 (and feel free to open an issue if that doesn't work!)
 
 ## alternatives
 
-- [pims_nd2](https://github.com/soft-matter/pims_nd2) - *pims-based reader. ctypes wrapper around the v9.00 (2015) SDK*
-- [nd2reader](https://github.com/rbnvrw/nd2reader) - *pims-based reader, using reverse-engineered file headers. mostly tested on NIS Elements 4.30.02*
-- [nd2file](https://github.com/csachs/nd2file) - *another pure-python, chunk map reader, unmaintained?*
-- [pyND2SDK](https://github.com/aarpon/pyND2SDK) - *windows-only cython wrapper around the v9.00 (2015) SDK. not on PyPI*
+Here are some other nd2 readers that I know of, though many
+of them are unmaintained:
+
+- [pims_nd2](https://github.com/soft-matter/pims_nd2) - *pims-based reader.
+  ctypes wrapper around the v9.00 (2015) SDK*
+- [nd2reader](https://github.com/rbnvrw/nd2reader) - *pims-based reader, using
+  reverse-engineered file headers. mostly tested on files from NIS Elements
+  4.30.02*
+- [nd2file](https://github.com/csachs/nd2file) - *another pure-python, chunk map
+  reader, unmaintained?*
+- [pyND2SDK](https://github.com/aarpon/pyND2SDK) - *windows-only cython wrapper
+  around the v9.00 (2015) SDK. not on PyPI*
 
 The motivating factors for this library were:
 
 - support for as many nd2 files as possible, with a large test suite
+  an and emphasis on correctness
 - pims-independent delayed reader based on dask
 - axis-associated metadata via xarray
-- combined approach of SDK and direct binary reads
```

### Comparing `nd2-0.5.3/README.md` & `nd2-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,119 @@
+Metadata-Version: 2.1
+Name: nd2
+Version: 0.6.0
+Summary: Yet another nd2 (Nikon NIS Elements) file reader
+Project-URL: homepage, https://github.com/tlambert03/nd2
+Project-URL: repository, https://github.com/tlambert03/nd2
+Project-URL: changelog, https://github.com/tlambert03/nd2/blob/main/CHANGELOG.md
+Author-email: Talley Lambert <talley.lambert@gmail.com>
+License: BSD 3-Clause License
+License-File: LICENSE
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Requires-Dist: numpy
+Requires-Dist: resource-backed-dask-array
+Requires-Dist: typing-extensions
+Provides-Extra: dev
+Requires-Dist: aicsimageio; extra == 'dev'
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: dask[array]; extra == 'dev'
+Requires-Dist: imagecodecs; extra == 'dev'
+Requires-Dist: ipython; extra == 'dev'
+Requires-Dist: lxml-stubs; extra == 'dev'
+Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: pre-commit; extra == 'dev'
+Requires-Dist: psutil; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: pytest-cov; extra == 'dev'
+Requires-Dist: rich; extra == 'dev'
+Requires-Dist: ruff; extra == 'dev'
+Requires-Dist: wurlitzer; extra == 'dev'
+Requires-Dist: xarray; extra == 'dev'
+Provides-Extra: legacy
+Requires-Dist: imagecodecs; extra == 'legacy'
+Requires-Dist: wurlitzer; extra == 'legacy'
+Provides-Extra: test
+Requires-Dist: aicsimageio; python_version < '3.11' and extra == 'test'
+Requires-Dist: dask[array]; extra == 'test'
+Requires-Dist: imagecodecs; platform_system == 'Windows' or python_version < '3.11' and extra == 'test'
+Requires-Dist: lxml; python_version < '3.11' and extra == 'test'
+Requires-Dist: psutil; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Requires-Dist: pytest-pretty; extra == 'test'
+Requires-Dist: pytest>=6.0; extra == 'test'
+Requires-Dist: wurlitzer; extra == 'test'
+Requires-Dist: xarray; extra == 'test'
+Description-Content-Type: text/markdown
+
 # nd2
 
 [![License](https://img.shields.io/pypi/l/nd2.svg?color=green)](https://github.com/tlambert03/nd2/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/nd2.svg?color=green)](https://pypi.org/project/nd2)
 [![Python Version](https://img.shields.io/pypi/pyversions/nd2.svg?color=green)](https://python.org)
 [![Tests](https://github.com/tlambert03/nd2/actions/workflows/ci.yml/badge.svg)](https://github.com/tlambert03/nd2/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/tlambert03/nd2/branch/main/graph/badge.svg)](https://codecov.io/gh/tlambert03/nd2)
 
-Yet another `.nd2` (Nikon NIS Elements) file reader.
-
-This reader provides a Cython wrapper for the official Nikon SDK.
-(The actual reading of image frames, however, uses a direct memmap approach, instead of the SDK,
-for performance reasons and to avoid occasional segfaults from the SDK.)
+`.nd2` (Nikon NIS Elements) file reader.
 
-Features good metadata retrieval, and direct `to_dask` and `to_xarray` options for lazy and/or annotated arrays.
+This reader provides a pure python implementation the official Nikon ND2 SDK.
 
-This library is tested against many nd2 files with the goal of maximizing compatibility and data extraction.
-(If you find an nd2 file that fails in some way, please open an issue with the file!)
+> It *used* to wrap the official SDK with Cython, but has since been completely
+> rewritten to be pure python (for performance, ease of distribution, and
+> maintenance) while retaining complete API parity with the official SDK.
+>
+> **Note:** This library is not affiliated with Nikon in any way, but we are
+> grateful for assistance from the SDK developers at Laboratory Imaging.
+
+Features good metadata retrieval, and direct `to_dask` and `to_xarray` options
+for lazy and/or annotated arrays.
+
+This library is tested against many nd2 files with the goal of maximizing
+compatibility and data extraction. (If you find an nd2 file that fails in some
+way, please [open an issue](https://github.com/tlambert03/nd2/issues/new) with
+the file!)
 
 ## install
 
 ```sh
 pip install nd2
 ```
 
 or from conda:
 
 ```sh
 conda install -c conda-forge nd2
 ```
 
-### extras
+### Legacy nd2 file support
 
-Legacy nd2 (JPEG2000) files are also supported, but require `imagecodecs`.  To install with support for these files use:
+Legacy nd2 (JPEG2000) files are also supported, but require `imagecodecs`.  To
+install with support for these files use the `legacy` extra:
 
 ```sh
 pip install nd2[legacy]
 ```
 
+### Faster XML parsing
+
+Much of the metadata in the file stored as XML.  If found in the environment,
+`nd2` will use [`lxml`](https://pypi.org/project/lxml/) which is much faster
+than the built-in `xml` module.  To install with support for `lxml` use:
+
+```sh
+pip install nd2 lxml
+```
+
 ## usage and API
 
 ```python
 import nd2
 import numpy as np
 
 my_array = nd2.imread('some_file.nd2')                          # read to numpy array
@@ -89,14 +162,15 @@
 f.recorded_data     # returns a dict of lists (passable to pandas.DataFrame) that
                     # the tabular "Recorded Data" view from in NIS Elements/Viewer
                     # with info for each frame in the experiment.
 
 # allll the metadata we can find...
 # no attempt made to standardize or parse it
 # look in here if you're searching for metdata that isn't exposed in the above
+# but try not to rely on it, as it's not guaranteed to be stable
 f.unstructured_metadata()
 
 f.close()           # don't forget to close when not using a contet manager!
 f.closed            # boolean, whether the file is closed
 ```
 
 ## Metadata structures
@@ -678,15 +752,14 @@
 ```python
 >>> binary_layer = binary_layers[0]
 >>> np.asarray(binary_layer)
 ```
 
 </details>
 
-
 ## Contributing / Development
 
 To test locally and contribute.  Clone this repo, then:
 
 ```
 pip install -e .[dev]
 ```
@@ -704,18 +777,26 @@
 pytest
 ```
 
 (and feel free to open an issue if that doesn't work!)
 
 ## alternatives
 
-- [pims_nd2](https://github.com/soft-matter/pims_nd2) - *pims-based reader. ctypes wrapper around the v9.00 (2015) SDK*
-- [nd2reader](https://github.com/rbnvrw/nd2reader) - *pims-based reader, using reverse-engineered file headers. mostly tested on NIS Elements 4.30.02*
-- [nd2file](https://github.com/csachs/nd2file) - *another pure-python, chunk map reader, unmaintained?*
-- [pyND2SDK](https://github.com/aarpon/pyND2SDK) - *windows-only cython wrapper around the v9.00 (2015) SDK. not on PyPI*
+Here are some other nd2 readers that I know of, though many
+of them are unmaintained:
+
+- [pims_nd2](https://github.com/soft-matter/pims_nd2) - *pims-based reader.
+  ctypes wrapper around the v9.00 (2015) SDK*
+- [nd2reader](https://github.com/rbnvrw/nd2reader) - *pims-based reader, using
+  reverse-engineered file headers. mostly tested on files from NIS Elements
+  4.30.02*
+- [nd2file](https://github.com/csachs/nd2file) - *another pure-python, chunk map
+  reader, unmaintained?*
+- [pyND2SDK](https://github.com/aarpon/pyND2SDK) - *windows-only cython wrapper
+  around the v9.00 (2015) SDK. not on PyPI*
 
 The motivating factors for this library were:
 
 - support for as many nd2 files as possible, with a large test suite
+  an and emphasis on correctness
 - pims-independent delayed reader based on dask
 - axis-associated metadata via xarray
-- combined approach of SDK and direct binary reads
```

### Comparing `nd2-0.5.3/src/nd2/_binary.py` & `nd2-0.6.0/src/nd2/_binary.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 import struct
 import warnings
 from typing import TYPE_CHECKING, Iterator, NamedTuple, Sequence, cast, overload
 
 import numpy as np
 
 if TYPE_CHECKING:
-    from ._sdk.latest import ND2Reader as LatestSDKReader
+    from numpy.typing import DTypeLike
+
+    from ._pysdk._pysdk import ND2Reader as LatestSDKReader
     from .nd2file import ND2File
 
 I7 = struct.Struct("<" + "I" * 7)
 I9 = struct.Struct("<" + "I" * 9)
 I2 = struct.Struct("<" + "I" * 2)
 
 
@@ -85,15 +87,17 @@
 
         # TODO: this is a bit of a hack (takes up memory), but it works for now
         # could do something with dask
         d = [
             i if i is not None else np.zeros(frame_shape, dtype="uint16")
             for i in self.data
         ]
-        return np.stack(d).reshape(self.coordinate_shape + frame_shape)
+        return cast(
+            "np.ndarray", np.stack(d).reshape(self.coordinate_shape + frame_shape)
+        )
 
     def __repr__(self) -> str:
         """Return a nicely formatted string."""
         field_names = (f for f in self._fields if f != "data")
         repr_fmt = "(" + ", ".join(f"{name}=%r" for name in field_names) + ")"
         return self.__class__.__name__ + repr_fmt % self[1:]
 
@@ -149,43 +153,48 @@
             if d is not None:
                 out.append(d)
         return np.stack(out)
 
     @classmethod
     def from_nd2file(cls, nd2file: ND2File) -> BinaryLayers | None:
         """Extract binary layers from an ND2 file."""
-        if nd2file.is_legacy:
+        if nd2file.is_legacy:  # pragma: no cover
             warnings.warn(
-                "`binary_data` is not supported for legacy ND2 files", UserWarning
+                "`binary_data` is not supported for legacy ND2 files",
+                UserWarning,
+                stacklevel=2,
             )
             return None
         rdr = cast("LatestSDKReader", nd2file._rdr)
 
-        binary_meta = nd2file.custom_data.get("BinaryMetadata_v1")
-        if binary_meta is None:
-            return None
         try:
-            items: list[dict] = binary_meta["BinaryMetadata_v1"]["BinaryItem"]
+            binary_meta = rdr._decode_chunk(
+                b"CustomDataVar|BinaryMetadata_v1!", strip_prefix=True
+            )
         except KeyError:
+            return None
+
+        try:
+            items: dict = binary_meta["BinaryMetadata_v1"]
+        except KeyError:  # pragma: no cover
             warnings.warn(
-                "Could not find 'BinaryMetadata_v1->BinaryItem' tag, please open an "
+                "Could not find 'BinaryMetadata_v1' tag, please open an "
                 "issue with this file at https://github.com/tlambert03/nd2/issues/new",
+                stacklevel=2,
             )
             return None
-        if isinstance(items, dict):
-            items = [items]
 
-        binseqs = sorted(x for x in rdr._meta_map if "RleZipBinarySequence" in x)
+        binseqs = sorted(x for x in rdr.chunkmap if b"RleZipBinarySequence" in x)
         mask_items = []
-        for item in items:
-            key = item["FileTag"]
+        for _, item in sorted(items.items()):
+            key = item["FileTag"].encode()
             _masks: list[np.ndarray | None] = []
             for bs in binseqs:
                 if key in bs:
-                    data = rdr._get_meta_chunk(bs)[4:]
+                    data = rdr._load_chunk(bs)[4:]
                     _masks.append(_decode_binary_mask(data) if data else None)
             mask_items.append(
                 BinaryLayer(
                     data=_masks,
                     name=item["Name"],
                     comp_name=item["CompName"],
                     comp_order=item["CompOrder"],
@@ -197,37 +206,37 @@
                     coordinate_shape=nd2file._coord_shape,
                 )
             )
 
         return cls(mask_items)
 
 
-def _unpack(stream: io.BufferedIOBase, strct: struct.Struct):
+def _unpack(stream: io.BufferedIOBase, strct: struct.Struct) -> tuple:
     return strct.unpack(stream.read(strct.size))
 
 
-def _decode_binary_mask(data: bytes, dtype="uint16") -> np.ndarray:
+def _decode_binary_mask(data: bytes, dtype: DTypeLike = "uint16") -> np.ndarray:
     # this receives data as would be extracted from a
     # `CustomDataSeq|RleZipBinarySequence...` section in the metadata
-    # data = f._rdr._get_meta_chunk('CustomDataSeq|RleZipBinarySequence_1_v1|0')[:4]
 
     # NOTE it is up to ND2File to strip the first 4 bytes... and not call this if there
     # is no data (i.e. if the chunk is just '\x00')
     import zlib
 
     decomp = zlib.decompress(data)
     stream = io.BytesIO(decomp)
 
     # still not sure what _q is
     # tot_bytes should be length of the stream remaining after this
     (v, ncols, nrows, nmasks, tot_bytes, _q, _zero) = _unpack(stream, I7)
     if v != 3:
         warnings.warn(
             f"Expected first byte to be 3 but got {v}. "
-            "Please submit this file :) https://github.com/tlambert03/nd2/issues/."
+            "Please submit this file :) https://github.com/tlambert03/nd2/issues/.",
+            stacklevel=2,
         )
 
     output = np.zeros((nrows, ncols), dtype=dtype)
     for _m in range(nmasks):
         # (1,     1,  0, 15, 11,       412,      12, 396, 0)
         (roi_id, c0, r0, c1, r1, roi_bytes, maskrows, _y, _zero) = _unpack(stream, I9)
         for _r in range(maskrows):
```

### Comparing `nd2-0.5.3/src/nd2/_legacy.py` & `nd2-0.6.0/src/nd2/_legacy/_legacy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,30 @@
+from __future__ import annotations
+
 import contextlib
 import re
 import struct
 import threading
-from pathlib import Path
-from typing import BinaryIO, DefaultDict, Dict, List, Optional, Tuple, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    BinaryIO,
+    DefaultDict,
+)
 
 import numpy as np
 
-from . import structures as strct
-from ._util import VoxelSize, dims_from_description
-from ._xml import parse_xml_block
+from nd2 import structures as strct
+from nd2._util import AXIS, VoxelSize
+
+from ._legacy_xml import parse_xml_block
+
+if TYPE_CHECKING:
+    from collections import defaultdict
+    from pathlib import Path
 
 try:
     from functools import cached_property
 except ImportError:
     cached_property = property  # type: ignore
 
 
@@ -21,15 +32,15 @@
 JP2_MAP_CHUNK = struct.Struct("<4s4sI")
 IHDR = struct.Struct(">iihBB")  # yxc-dtype in jpeg 2000
 
 
 class LegacyND2Reader:
     _fh: BinaryIO
 
-    def __init__(self, path: Union[Path, str]):
+    def __init__(self, path: Path | str):
         self._path = str(path)
         self._fh = open(self._path, mode="rb")
         length, box_type = I4s.unpack(self._fh.read(I4s.size))
         if length != 12 and box_type == b"jP  ":
             raise ValueError("File not recognized as Legacy ND2 (JPEG2000) format.")
         self._chunkmap = legacy_nd2_chunkmap(self._fh)
         self.lock = threading.RLock()
@@ -42,26 +53,26 @@
         if not self.closed:
             self._fh.close()
 
     @property
     def closed(self) -> bool:
         return self._fh.closed
 
-    def __enter__(self) -> "LegacyND2Reader":
+    def __enter__(self) -> LegacyND2Reader:
         self.open()
         return self
 
-    def __exit__(self, *_) -> None:
+    def __exit__(self, *_: Any) -> None:
         self.close()
 
     @cached_property
     def ddim(self) -> dict:
-        return dims_from_description(self.text_info().get("description"))
+        return _dims_from_description(self.text_info().get("description"))
 
-    def experiment(self) -> List[strct.ExpLoop]:
+    def experiment(self) -> list[strct.ExpLoop]:
         meta = self._metadata
         exp = []
         if "LoopNo00" in meta:
             # old style:
             for i, (k, v) in enumerate(meta.items()):
                 if k != "Version":
                     loop = self._make_loop(v, i)
@@ -78,21 +89,19 @@
                 loop = self._make_loop(meta, i)
                 if loop:
                     exp.append(loop)
                 meta = meta.get("NextLevelEx")  # type: ignore
                 i += 1
         return exp
 
-    def _coord_info(self) -> List[Tuple[int, str, int]]:
+    def _coord_info(self) -> list[tuple[int, str, int]]:
         return [(i, x.type, x.count) for i, x in enumerate(self.experiment())]
 
-    def _make_loop(
-        self, meta_level: dict, nest_level: int = 0
-    ) -> Optional[strct.ExpLoop]:
-        """converts an old style metadata loop dict to a new ExpLoop structure."""
+    def _make_loop(self, meta_level: dict, nest_level: int = 0) -> strct.ExpLoop | None:
+        """Converts an old style metadata loop dict to a new ExpLoop structure."""
         type_ = meta_level.get("Type")
         params: dict = meta_level["LoopPars"]
         if type_ == 2:  # XYPosLoop
             poscount = len(params["PosX"])
             # empirically, it appears that some files list more positions in the
             # metadata than are actually recorded in the textinfo -> description.
             # NIS viewer seems to agree more with the description
@@ -183,15 +192,15 @@
             widthBytes=widthPx * bpcim // 8 * compCount,
             pixelDataType="unsigned",
             sequenceCount=len(self._chunkmap[b"VCAL"]),
             compressionLevel=head.get("compression"),
             channelCount=nC,
         )
 
-    def _get_xml_dict(self, key: bytes, index=0) -> dict:
+    def _get_xml_dict(self, key: bytes, index: int = 0) -> dict:
         try:
             bxml = self._read_chunk(self._chunkmap[key][index])
             return parse_xml_block(bxml)
         except KeyError:
             return {}
 
     @cached_property
@@ -230,15 +239,15 @@
     def metadata(self) -> dict:
         return self._metadata
 
     @property
     def calibration(self) -> dict:
         return self._get_xml_dict(b"ACAL")
 
-    def _read_chunk(self, pos) -> bytes:
+    def _read_chunk(self, pos: int) -> bytes:
         with self.lock:
             self._fh.seek(pos)
             length, box_type = I4s.unpack(self._fh.read(I4s.size))
             return self._fh.read(length - I4s.size)
 
     def _read_image(self, index: int) -> np.ndarray:
         try:
@@ -259,49 +268,34 @@
 
     def frame_metadata(self, index: int) -> dict:
         return {
             **self._get_xml_dict(b"VCAL", index),
             **self._get_xml_dict(b"VIMD", index),
         }
 
-    def _scan_vimd(self):
-        zs = set()
-        xys = set()
-        ts = set()
-        cs = set()
-        for i in range(len(self._chunkmap[b"VIMD"])):
-            xml = self._get_xml_dict(b"VIMD", i)
-            ts.add(xml["TimeMSec"])
-            xys.add((xml["XPos"], xml["YPos"]))
-            for p in xml["PicturePlanes"]["Plane"].values():
-                cs.add(p["OpticalConfigName"])
-                zs.add(p["OpticalConfigFull"]["ZPosition0"])
-        return (zs, xys, ts, cs)
-
     def voxel_size(self) -> VoxelSize:
-
-        z: Optional[float] = None
+        z: float | None = None
         d = self.text_info().get("description") or ""
         _z = re.search(r"Z Stack Loop: 5\s+-\s+Step\s+([.\d]+)", d)
         if _z:
             with contextlib.suppress(Exception):
                 z = float(_z.groups()[0])
         if z is None:
             for e in self.experiment():
                 if e.type == "ZStackLoop":
                     z = e.parameters.stepUm
                     break
         xy = self._get_xml_dict(b"VIMD", 0).get("Calibration") or 1
         return VoxelSize(xy, xy, z or 1)
 
-    def channel_names(self) -> List[str]:
+    def channel_names(self) -> list[str]:
         xml = self._get_xml_dict(b"VIMD", 0)
         return [p["OpticalConfigName"] for p in xml["PicturePlanes"]["Plane"].values()]
 
-    def time_stamps(self) -> List[str]:
+    def time_stamps(self) -> list[str]:
         xml = self._get_xml_dict(b"VIMD", 0)
         return [p["OpticalConfigName"] for p in xml["PicturePlanes"]["Plane"].values()]
 
     @cached_property
     def header(self) -> dict:
         try:
             pos = self._chunkmap[b"jp2h"][0]
@@ -320,57 +314,38 @@
             "compression": z,
         }
 
     def _custom_data(self) -> dict:
         return {}
 
 
-def legacy_nd2_chunkmap(fh: BinaryIO) -> Dict[bytes, List[int]]:
+def legacy_nd2_chunkmap(fh: BinaryIO) -> dict[bytes, list[int]]:
     fh.seek(-40, 2)
     sig, map_start = struct.unpack("<32sQ", fh.read())
     if sig != b"LABORATORY IMAGING ND BOX MAP 00":
         raise ValueError("Not a legacy ND2 file")
     fh.seek(-map_start, 2)
     n_chunks = int.from_bytes(fh.read(4), "big")
     data = fh.read()
-    d: DefaultDict[bytes, List[int]] = DefaultDict(list)
+    d: defaultdict[bytes, list[int]] = DefaultDict(list)
     for i in range(n_chunks):
         box_type, lim_type, offset = JP2_MAP_CHUNK.unpack_from(data, i * 16)
         if box_type in {b"jP  ", b"ftyp", b"jp2h"}:
             d[box_type].append(offset)
         else:
             d[lim_type].append(offset)
     return dict(d)
 
 
-# def jp2_chunkmap(fh: io.BufferedReader) -> Dict[bytes, List[Tuple[int, int]]]:
-#     """Retrieve chunk positions and shape from jpeg 2000 (legacy ND2) format
-
-#     https://www.file-recovery.com/jp2-signature-format.htm
+DIMSIZE = re.compile(r"(\w+)'?\((\d+)\)")
 
-#     ISO/IEC 15444
 
-#     The JPEG 2000 file format specification was based on the QuickTime
-#     container format specification. A JPEG 2000 file is always big-endian.
-
-#     JPEG 2000 files consist of consecutive chunks. Each chunk has 8 byte header:
-#     4-byte chunk size (big-endian, high byte first) and 4-byte chunk type -
-#     one of pre-defined signatures: "jP " or "jP2 ".
-
-#     """
-#     out = DefaultDict(list)
-#     for box_type, pos, length in iter_jp2_chunks(fh):
-#         out[box_type].append((pos, length))
-#     return dict(out)
-
-
-# def iter_jp2_chunks(fh: io.BufferedReader) -> Iterator[Tuple[bytes, int, int]]:
-#     file_size = fh.seek(0, 2)
-#     fh.seek(0)
-#     pos = 0
-#     while True:
-#         length, box_type = I4s.unpack(fh.read(I4s.size))
-#         yield box_type, pos, length
-#         pos += length
-#         if pos >= file_size:
-#             break
-#         fh.seek(pos)  # jump to next box
+def _dims_from_description(desc: str | None) -> dict:
+    if not desc:
+        return {}
+    match = re.search(r"Dimensions:\s?([^\r]+)\r?\n", desc)
+    if not match:
+        return {}
+    dims = match.groups()[0]
+    dims = dims.replace("λ", AXIS.CHANNEL)
+    dims = dims.replace("XY", AXIS.POSITION)
+    return {k: int(v) for k, v in DIMSIZE.findall(dims)}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nd2-0.5.3/src/nd2/_util.py` & `nd2-0.6.0/src/nd2/_util.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,30 @@
+from __future__ import annotations
+
 import re
 from datetime import datetime
-from typing import IO, TYPE_CHECKING, Any, Callable, NamedTuple, Optional, Union
+from typing import IO, TYPE_CHECKING, Any, Callable, NamedTuple, Union
 
 if TYPE_CHECKING:
     from os import PathLike
 
     from ._legacy import LegacyND2Reader
-    from ._sdk.latest import ND2Reader
+    from ._pysdk._pysdk import ND2Reader
 
     StrOrBytesPath = Union[str, bytes, PathLike[str], PathLike[bytes]]
 
 
 NEW_HEADER_MAGIC = b"\xda\xce\xbe\n"
 OLD_HEADER_MAGIC = b"\x00\x00\x00\x0c"
 VERSION = re.compile(r"^ND2 FILE SIGNATURE CHUNK NAME01!Ver([\d\.]+)$")
 
 
 def is_supported_file(
-    path: "StrOrBytesPath", open_: Callable[["StrOrBytesPath", str], IO[Any]] = open
-):
+    path: StrOrBytesPath, open_: Callable[[StrOrBytesPath, str], IO[Any]] = open
+) -> bool:
     """Return `True` if `path` can be opened as an nd2 file.
 
     Parameters
     ----------
     path : Union[str, bytes, PathLike]
         A path to query
     open_ : Callable[[StrOrBytesPath, str], IO[Any]]
@@ -33,15 +35,15 @@
     bool
         Whether the can be opened.
     """
     with open_(path, "rb") as fh:
         return fh.read(4) in (NEW_HEADER_MAGIC, OLD_HEADER_MAGIC)
 
 
-def is_legacy(path: "StrOrBytesPath") -> bool:
+def is_legacy(path: StrOrBytesPath) -> bool:
     """Return `True` if `path` is a legacy ND2 file.
 
     Parameters
     ----------
     path : Union[str, bytes, PathLike]
         A path to query
 
@@ -54,69 +56,52 @@
         return fh.read(4) == OLD_HEADER_MAGIC
 
 
 def get_reader(
     path: str,
     validate_frames: bool = False,
     search_window: int = 100,
-    read_using_sdk: Optional[bool] = None,
-) -> Union["ND2Reader", "LegacyND2Reader"]:
+) -> ND2Reader | LegacyND2Reader:
     with open(path, "rb") as fh:
         magic_num = fh.read(4)
         if magic_num == NEW_HEADER_MAGIC:
-            from ._sdk.latest import ND2Reader
+            from ._pysdk._pysdk import ND2Reader
 
             return ND2Reader(
                 path,
                 validate_frames=validate_frames,
                 search_window=search_window,
-                read_using_sdk=read_using_sdk,
             )
         elif magic_num == OLD_HEADER_MAGIC:
-            from ._legacy import LegacyND2Reader
+            from ._legacy._legacy import LegacyND2Reader
 
             return LegacyND2Reader(path)
         raise OSError(
             f"file {path} not recognized as ND2.  First 4 bytes: {magic_num!r}"
         )
 
 
 def is_new_format(path: str) -> bool:
     # TODO: this is just for dealing with missing test data
     with open(path, "rb") as fh:
         return fh.read(4) == NEW_HEADER_MAGIC
 
 
-def jdn_to_datetime_local(jdn):
+def jdn_to_datetime_local(jdn: float) -> datetime:
     return datetime.fromtimestamp((jdn - 2440587.5) * 86400.0)
 
 
-def jdn_to_datetime_utc(jdn):
+def jdn_to_datetime_utc(jdn: float) -> datetime:
     return datetime.utcfromtimestamp((jdn - 2440587.5) * 86400.0)
 
 
-def rgb_int_to_tuple(rgb):
+def rgb_int_to_tuple(rgb: int) -> tuple[int, int, int]:
     return ((rgb & 255), (rgb >> 8 & 255), (rgb >> 16 & 255))
 
 
-DIMSIZE = re.compile(r"(\w+)'?\((\d+)\)")
-
-
-def dims_from_description(desc) -> dict:
-    if not desc:
-        return {}
-    match = re.search(r"Dimensions:\s?([^\r]+)\r?\n", desc)
-    if not match:
-        return {}
-    dims = match.groups()[0]
-    dims = dims.replace("λ", AXIS.CHANNEL)
-    dims = dims.replace("XY", AXIS.POSITION)
-    return {k: int(v) for k, v in DIMSIZE.findall(dims)}
-
-
 class AXIS:
     X = "X"
     Y = "Y"
     Z = "Z"
     CHANNEL = "C"
     RGB = "S"
     TIME = "T"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nd2-0.5.3/src/nd2/_xml.py` & `nd2-0.6.0/src/nd2/_legacy/_legacy_xml.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,63 +1,72 @@
+"""XML parsing utilities for legacy ND2 files.
+
+Todo:
+----
+all of this logic is duplicated in _clx_xml.py.
+_legacy.py just needs some slight updates to deal with different parsing results.
+"""
+from __future__ import annotations
+
 import re
 from functools import partial
-from typing import Any, Callable, Dict, Optional
+from typing import Any, Callable
 
 try:
     from lxml import etree
 except ImportError:
     import xml.etree.ElementTree as etree  # type: ignore
 
 
-def parse_xml_block(bxml: bytes) -> Dict[str, Any]:
+def parse_xml_block(bxml: bytes) -> dict[str, Any]:
     node = etree.XML(bxml.split(b"?>", 1)[-1])
-    return elem2dict(node)
+    return elem2dict(node)  # type: ignore
 
 
 lower = re.compile("^[a-z_]+")
-_TYPEMAP: Dict[Optional[str], Callable] = {
+_TYPEMAP: dict[str | bytes | None, Callable] = {
     "bool": bool,
     "lx_uint32": int,
     "lx_uint64": int,
     "lx_int32": int,
     "lx_int64": int,
     "double": float,
     "CLxStringW": str,
     "CLxByteArray": partial(bytes, encoding="utf-8"),
     "unknown": str,
     None: str,
 }
 
 
-def elem2dict(node: "etree._Element") -> Dict[str, Any]:
+def elem2dict(node: etree._Element) -> Any:
     """Convert an lxml.etree node tree into a dict."""
-    result: Dict[str, Any] = {}
+    result: dict[str, Any] = {}
 
     if "value" in node.attrib:
         type_ = _TYPEMAP[node.attrib.get("runtype")]
         try:
             return type_(node.attrib["value"])
         except ValueError:
             return node.attrib["value"]
 
     attrs = node.attrib
-    attrs.pop("runtype", None)
-    attrs.pop("version", None)
-    result.update(node.attrib)
+    attrs.pop("runtype", "")
+    attrs.pop("version", "")
+    result.update(node.attrib)  # type: ignore
 
     # [<Element CustomTagDescription_v1.0 at 0x12a29ac40>]
     for element in node:
         # Remove namespace prefix
         key = element.tag.split("}")[1] if "}" in element.tag else element.tag
         key = lower.sub("", key) or key
 
         # Process element as tree element if the inner XML contains non-whitespace
         # content
         if element.text and element.text.strip():
-            value = element.text
+            value: str | dict = element.text
         else:
             value = elem2dict(element)
         if key in result:
             if type(result[key]) is list:
                 result[key].append(value)
             else:
                 result[key] = [result[key], value]
```

### Comparing `nd2-0.5.3/src/nd2/nd2file.py` & `nd2-0.6.0/src/nd2/nd2file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,131 +1,118 @@
 from __future__ import annotations
 
-import contextlib
-import mmap
 import threading
 import warnings
-from enum import Enum
 from itertools import product
 from pathlib import Path
-from typing import (
-    TYPE_CHECKING,
-    Sequence,
-    Sized,
-    SupportsInt,
-    Union,
-    cast,
-    no_type_check,
-    overload,
-)
+from typing import TYPE_CHECKING, cast, overload
 
 import numpy as np
 
-from ._nd2decode import _decode_custom_data, decode_metadata, unnest_experiments
+from ._pysdk._chunk_decode import ND2_FILE_SIGNATURE
 from ._util import AXIS, VoxelSize, get_reader, is_supported_file
-from .structures import (
-    ROI,
-    Attributes,
-    ExpLoop,
-    FrameMetadata,
-    Metadata,
-    XYPosLoop,
-    ZStackLoop,
-)
+from .structures import ROI
 
 try:
     from functools import cached_property
 except ImportError:
     cached_property = property  # type: ignore
 
 
 if TYPE_CHECKING:
-    from typing import Any
+    import mmap
+    from typing import Any, Sequence, Sized, SupportsInt
 
     import dask.array.core
     import xarray as xr
     from typing_extensions import Literal
 
     from ._binary import BinaryLayers
-    from ._sdk.latest import ND2Reader as LatestSDKReader
-    from .structures import Position
+    from ._pysdk._pysdk import ND2Reader as LatestSDKReader
+    from ._util import StrOrBytesPath
+    from .structures import (
+        Attributes,
+        ExpLoop,
+        FrameMetadata,
+        Metadata,
+        TextInfo,
+        XYPosLoop,
+    )
 
+__all__ = ["ND2File", "imread"]
 
-Index = Union[int, slice]
 
-ROI_METADATA = "CustomData|RoiMetadata_v1"
-IMG_METADATA = "ImageMetadataLV"
-
-
-class ReadMode(str, Enum):
-    MMAP = "mmap"
-    SDK = "sdk"
+class ND2File:
+    """Main objecting for opening and extracting data from an nd2 file.
 
+    Parameters
+    ----------
+    path : Path | str
+        Filename of an nd2 file.
+    validate_frames : bool
+        Whether to verify (and attempt to fix) frames whose positions have been
+        shifted relative to the predicted offset (i.e. in a corrupted file).
+        This comes at a slight performance penalty at file open, but may "rescue"
+        some corrupt files. by default False.
+    search_window : int
+        When validate_frames is true, this is the search window (in KB) that will
+        be used to try to find the actual chunk position. by default 100 KB
+    read_using_sdk : Optional[bool]
+        DEPRECATED.  No longer does anything.
+        If `True`, use the SDK to read the file. If `False`, inspects the chunkmap
+        and reads from a `numpy.memmap`. If `None` (the default), uses the SDK if
+        the file is compressed, otherwise uses the memmap. Note: using
+        `read_using_sdk=False` on a compressed file will result in a ValueError.
+    """
 
-class ND2File:
     _memmap: mmap.mmap
     _is_legacy: bool
 
     def __init__(
         self,
         path: Path | str,
         *,
         validate_frames: bool = False,
         search_window: int = 100,
         read_using_sdk: bool | None = None,
     ) -> None:
-        """Open an nd2 file.
-
-        Parameters
-        ----------
-        path : Union[Path, str]
-            Filename of an nd2 file.
-        validate_frames : bool
-            Whether to verify (and attempt to fix) frames whose positions have been
-            shifted relative to the predicted offset (i.e. in a corrupted file).
-            This comes at a slight performance penalty at file open, but may "rescue"
-            some corrupt files. by default False.
-        search_window : int
-            When validate_frames is true, this is the search window (in KB) that will
-            be used to try to find the actual chunk position. by default 100 KB
-        read_using_sdk : Optional[bool]
-            If `True`, use the SDK to read the file. If `False`, inspects the chunkmap
-            and reads from a `numpy.memmap`. If `None` (the default), uses the SDK if
-            the file is compressed, otherwise uses the memmap. Note: using
-            `read_using_sdk=False` on a compressed file will result in a ValueError.
-
-        """
+        if read_using_sdk is not None:
+            warnings.warn(
+                "The `read_using_sdk` argument is deprecated and will be removed in "
+                "a future version.",
+                FutureWarning,
+                stacklevel=2,
+            )
         self._path = str(path)
         self._rdr = get_reader(
             self._path,
             validate_frames=validate_frames,
             search_window=search_window,
-            read_using_sdk=read_using_sdk,
         )
         self._closed = False
         self._is_legacy = "Legacy" in type(self._rdr).__name__
         self._lock = threading.RLock()
 
     @staticmethod
-    def is_supported_file(path) -> bool:
+    def is_supported_file(path: StrOrBytesPath) -> bool:
         """Return True if the file is supported by this reader."""
         return is_supported_file(path)
 
     @property
-    def path(self):
+    def path(self) -> str:
         """Path of the image."""
         return self._path
 
     @property
     def is_legacy(self) -> bool:
         """Whether file is a legacy nd2 (JPEG2000) file."""
         return self._is_legacy
 
     def open(self) -> None:
-        """open file for reading."""
+        """Open file for reading."""
         if self.closed:
             self._rdr.open()
             self._closed = False
 
     def close(self) -> None:
         """Close file (may cause segfault if read when closed in some cases)."""
         if not self.closed:
@@ -134,100 +121,85 @@
 
     @property
     def closed(self) -> bool:
         """Whether the file is closed."""
         return self._closed
 
     def __enter__(self) -> ND2File:
+        """Open file for reading."""
         self.open()
         return self
 
     def __del__(self) -> None:
         """Delete file handle on garbage collection."""
         if not getattr(self, "_closed", True):
             warnings.warn(
                 "ND2File file not closed before garbage collection. "
                 "Please use `with ND2File(...):` context or call `.close()`.",
                 stacklevel=2,
             )
             self._rdr.close()
 
-    def __exit__(self, *_) -> None:
+    def __exit__(self, *_: Any) -> None:
+        """Exit context manager and close file."""
         self.close()
 
-    def __getstate__(self):
+    def __getstate__(self) -> dict[str, Any]:
+        """Return state for pickling."""
         state = self.__dict__.copy()
         del state["_rdr"]
         del state["_lock"]
         return state
 
-    def __setstate__(self, d):
+    def __setstate__(self, d: dict[str, Any]) -> None:
+        """Load state from pickling."""
         self.__dict__ = d
         self._lock = threading.RLock()
         self._rdr = get_reader(self._path)
         if self._closed:
             self._rdr.close()
 
     @cached_property
     def attributes(self) -> Attributes:
         """Core image attributes."""
         return self._rdr.attributes
 
     @cached_property
-    def text_info(self) -> dict[str, Any]:
+    def text_info(self) -> TextInfo | dict:
         """Misc text info."""
         return self._rdr.text_info()
 
     @cached_property
     def rois(self) -> dict[int, ROI]:
         """Return dict of {id: ROI} for all ROIs found in the metadata."""
-        if self.is_legacy or ROI_METADATA not in self._rdr._meta_map:  # type: ignore
-            return {}
-        data = self.unstructured_metadata(include={ROI_METADATA})
-        data = data.get(ROI_METADATA, {}).get("RoiMetadata_v1", {})
+        key = b"CustomData|RoiMetadata_v1!"
+        if self.is_legacy or key not in self._rdr.chunkmap:  # type: ignore
+            return {}  # pragma: no cover
+
+        data = cast("LatestSDKReader", self._rdr)._decode_chunk(key)
+        data = data.get("RoiMetadata_v1", {}).copy()
         data.pop("Global_Size", None)
         try:
-            _rois = (ROI._from_meta_dict(d) for d in data.values())
-            rois = {r.id: r for r in _rois}
-        except Exception as e:
+            _rois = [ROI._from_meta_dict(d) for d in data.values()]
+        except Exception as e:  # pragma: no cover
             raise ValueError(f"Could not parse ROI metadata: {e}") from e
-        return rois
+        return {r.id: r for r in _rois}
 
     @cached_property
     def experiment(self) -> list[ExpLoop]:
         """Loop information for each nd axis."""
-        exp = self._rdr.experiment()
-
-        # https://github.com/tlambert03/nd2/issues/78
-        # the SDK doesn't always do a good job of pulling position names from metadata
-        # here, we try to extract it manually.  Might be error prone, so currently
-        # we just ignore errors.
-        if not self.is_legacy and IMG_METADATA in self._rdr._meta_map:  # type: ignore
-            for n, item in enumerate(exp):
-                if isinstance(item, XYPosLoop):
-                    names = {
-                        tuple(p.stagePositionUm): p.name for p in item.parameters.points
-                    }
-                    if not any(names.values()):
-                        _exp = self.unstructured_metadata(
-                            include={IMG_METADATA}, unnest=True
-                        )[IMG_METADATA]
-                        if n >= len(_exp):
-                            continue
-                        with contextlib.suppress(Exception):
-                            _fix_names(_exp[n], item.parameters.points)
-        return exp
+        return self._rdr.experiment()
 
     def unstructured_metadata(
         self,
         *,
-        unnest: bool = False,
         strip_prefix: bool = True,
         include: set[str] | None = None,
         exclude: set[str] | None = None,
+        unnest: bool | None = None,
     ) -> dict[str, Any]:
         """Exposes, and attempts to decode, each metadata chunk in the file.
 
         This is provided as a *experimental* fallback in the event that
         `ND2File.experiment` does not contain all of the information you need. No
         attempt is made to parse or validate the metadata, and the format of various
         sections, *may* change in future versions of nd2. Consumption of this metadata
@@ -235,69 +207,70 @@
 
         The 'ImageMetadataLV' chunk is the most likely to contain useful information,
         but if you're generally looking for "hidden" metadata, it may be helpful to
         look at the full output.
 
         Parameters
         ----------
-        unnest : bool, optional
-            If `True` the nested `NextLevelEx` keys of each Experiment loop level will
-            be flattened into a list, and the return type will be `list`. by default
-            `False`.
         strip_prefix : bool, optional
             Whether to strip the type information from the front of the keys in the
             dict. For example, if `True`: `uiModeFQ` becomes `ModeFQ` and `bUsePFS`
             becomes `UsePFS`, etc... by default `True`
         include : Optional[Set[str]], optional
             If provided, only include the specified keys in the output. by default,
             all metadata sections found in the file are included.
         exclude : Optional[Set[str]], optional
             If provided, exclude the specified keys from the output. by default `None`
+        unnest : bool, optional
+            DEPRECATED.  No longer does anything.
 
         Returns
         -------
         Dict[str, Any]
             A dict of the unstructured metadata, with keys that are the type of the
             metadata chunk (things like 'CustomData|RoiMetadata_v1' or
             'ImageMetadataLV'), and values that are associated metadata chunk.
         """
-        if self.is_legacy:
+        if self.is_legacy:  # pragma: no cover
             raise NotImplementedError(
                 "unstructured_metadata not available for legacy files"
             )
 
-        output: dict[str, Any] = {}
+        if unnest is not None:
+            warnings.warn(
+                "The unnest parameter is deprecated, and no longer has any effect.",
+                FutureWarning,
+                stacklevel=2,
+            )
 
         rdr = cast("LatestSDKReader", self._rdr)
-        keys = set(rdr._meta_map)
+        keys = {
+            k.decode()[:-1]
+            for k in rdr.chunkmap
+            if not k.startswith((b"ImageDataSeq", b"CustomData", ND2_FILE_SIGNATURE))
+        }
+
         if include:
             _keys: set[str] = set()
             for i in include:
                 if i not in keys:
-                    warnings.warn(f"Key {i!r} not found in metadata")
+                    warnings.warn(f"Key {i!r} not found in metadata", stacklevel=2)
                 else:
                     _keys.add(i)
             keys = _keys
         if exclude:
             keys = {k for k in keys if k not in exclude}
 
+        output: dict[str, Any] = {}
         for key in sorted(keys):
+            name = f"{key}!".encode()
             try:
-                meta: bytes = rdr._get_meta_chunk(key)
-                if meta.startswith(b"<"):
-                    # probably xml
-                    decoded: Any = meta.decode("utf-8")
-                else:
-                    decoded = decode_metadata(meta, strip_prefix=strip_prefix)
-                    if key == IMG_METADATA and unnest:
-                        decoded = unnest_experiments(decoded)
-            except Exception:
-                decoded = meta
-
-            output[key] = decoded
+                output[key] = rdr._decode_chunk(name, strip_prefix=strip_prefix)
+            except Exception:  # pragma: no cover
+                output[key] = rdr._load_chunk(name)
         return output
 
     @cached_property
     def metadata(self) -> Metadata | dict:
         """Various metadata (will be dict if legacy format)."""
         return self._rdr.metadata()
 
@@ -328,25 +301,25 @@
     @cached_property
     def custom_data(self) -> dict[str, Any]:
         """Dict of various unstructured custom metadata."""
         return self._rdr._custom_data()
 
     @cached_property
     def ndim(self) -> int:
-        """number of dimensions."""
+        """Number of dimensions."""
         return len(self.shape)
 
     @cached_property
     def shape(self) -> tuple[int, ...]:
-        """size of each axis."""
+        """Size of each axis."""
         return self._coord_shape + self._frame_shape
 
     @cached_property
     def sizes(self) -> dict[str, int]:
-        """names and sizes for each axis."""
+        """Names and sizes for each axis."""
         attrs = self.attributes
         dims = {AXIS._MAP[c[1]]: c[2] for c in self._rdr._coord_info()}
         dims[AXIS.CHANNEL] = (
             dims.pop(AXIS.CHANNEL)
             if AXIS.CHANNEL in dims
             else (attrs.channelCount or 1)
         )
@@ -363,15 +336,15 @@
     def is_rgb(self) -> bool:
         """Whether the image is rgb."""
         return self.components_per_channel in (3, 4)
 
     @property
     def components_per_channel(self) -> int:
         """Number of components per channel (e.g. 3 for rgb)."""
-        attrs = cast(Attributes, self.attributes)
+        attrs = self.attributes
         return attrs.componentCount // (attrs.channelCount or 1)
 
     @property
     def size(self) -> int:
         """Total number of pixels in the volume."""
         return int(np.prod(self.shape))
 
@@ -431,41 +404,41 @@
                 except ValueError as e:
                     raise ValueError(
                         f"{position!r} is not a valid position name"
                     ) from e
             try:
                 pidx = list(self.sizes).index(AXIS.POSITION)
             except ValueError as exc:
-                if position > 0:
+                if position > 0:  # pragma: no cover
                     raise IndexError(
                         f"Position {position} is out of range. "
                         f"Only 1 position available"
                     ) from exc
                 seqs = range(self._frame_count)
             else:
                 if position >= self.sizes[AXIS.POSITION]:
-                    raise IndexError(
+                    raise IndexError(  # pragma: no cover
                         f"Position {position} is out of range. "
                         f"Only {self.sizes[AXIS.POSITION]} positions available"
                     )
 
                 ranges: list[range | tuple] = [range(x) for x in self._coord_shape]
                 ranges[pidx] = (position,)
                 coords = list(zip(*product(*ranges)))
                 seqs = self._seq_index_from_coords(coords)  # type: ignore
                 final_shape[pidx] = 1
 
         arr: np.ndarray = np.stack([self._get_frame(i) for i in seqs])
         return arr.reshape(final_shape)
 
     def __array__(self) -> np.ndarray:
-        """array protocol."""
+        """Array protocol."""
         return self.asarray()
 
-    def to_dask(self, wrapper=True, copy=True) -> dask.array.core.Array:
+    def to_dask(self, wrapper: bool = True, copy: bool = True) -> dask.array.core.Array:
         """Create dask array (delayed reader) representing image.
 
         This generally works well, but it remains to be seen whether performance
         is optimized, or if we're duplicating safety mechanisms. You may try
         various combinations of `wrapper` and `copy`, setting both to `False`
         will very likely cause segmentation faults in many cases.  But setting
         one of them to `False`, may slightly improve read speed in certain
@@ -488,15 +461,15 @@
             an array copy. This can avoid segfaults in certain cases, though it
             may also add overhead.
 
         Returns
         -------
         dask.array.core.Array
         """
-        from dask.array import map_blocks
+        from dask.array.core import map_blocks
 
         chunks = [(1,) * x for x in self._coord_shape]
         chunks += [(x,) for x in self._frame_shape]
         dask_arr = map_blocks(
             self._dask_block,
             copy=copy,
             chunks=chunks,
@@ -511,29 +484,29 @@
         return dask_arr
 
     _NO_IDX = -1
 
     def _seq_index_from_coords(self, coords: Sequence) -> Sequence[int] | SupportsInt:
         if not self._coord_shape:
             return self._NO_IDX
-        return np.ravel_multi_index(coords, self._coord_shape)
+        return np.ravel_multi_index(coords, self._coord_shape)  # type: ignore
 
     def _dask_block(self, copy: bool, block_id: tuple[int]) -> np.ndarray:
         if isinstance(block_id, np.ndarray):
-            return
+            return None
         with self._lock:
             was_closed = self.closed
             if self.closed:
                 self.open()
             try:
                 ncoords = len(self._coord_shape)
                 idx = self._seq_index_from_coords(block_id[:ncoords])
 
                 if idx == self._NO_IDX:
-                    if any(block_id):
+                    if any(block_id):  # pragma: no cover
                         raise ValueError(
                             f"Cannot get chunk {block_id} for single frame image."
                         )
                     idx = 0
                 data = self._get_frame(int(idx))  # type: ignore
                 data = data.copy() if copy else data
                 return data[(np.newaxis,) * ncoords]
@@ -606,31 +579,31 @@
 
     @property
     def _frame_coords(self) -> set[str]:
         return {AXIS.X, AXIS.Y, AXIS.CHANNEL, AXIS.RGB}
 
     @property
     def _raw_frame_shape(self) -> tuple[int, int, int, int]:
-        """sizes of each frame coordinate, prior to reshape."""
+        """Sizes of each frame coordinate, prior to reshape."""
         attr = self.attributes
         return (
             attr.heightPx,
             attr.widthPx or -1,
             attr.channelCount or 1,
             self.components_per_channel,
         )
 
     @property
     def _frame_shape(self) -> tuple[int, ...]:
-        """sizes of each frame coordinate, after reshape & squeeze."""
+        """Sizes of each frame coordinate, after reshape & squeeze."""
         return tuple(v for k, v in self.sizes.items() if k in self._frame_coords)
 
     @cached_property
     def _coord_shape(self) -> tuple[int, ...]:
-        """sizes of each *non-frame* coordinate."""
+        """Sizes of each *non-frame* coordinate."""
         return tuple(v for k, v in self.sizes.items() if k not in self._frame_coords)
 
     @property
     def _frame_count(self) -> int:
         return int(np.prod(self._coord_shape))
 
     def _get_frame(self, index: SupportsInt) -> np.ndarray:
@@ -675,19 +648,20 @@
 
         if self.components_per_channel > 1:
             coords[AXIS.RGB] = ["Red", "Green", "Blue", "alpha"][
                 : self.components_per_channel
             ]
 
         # fix for Z axis missing from experiment:
+        # TODO: this isn't hit by coverage... maybe it's not needed?
         if AXIS.Z in self.sizes and AXIS.Z not in coords:
             coords[AXIS.Z] = np.arange(self.sizes[AXIS.Z]) * dz
 
         if squeeze:
-            return {k: v for k, v in coords.items() if len(v) > 1}
+            coords = {k: v for k, v in coords.items() if len(v) > 1}
         return coords
 
     def _position_names(self, loop: XYPosLoop | None = None) -> list[str]:
         if loop is None:
             for c in self.experiment:
                 if c.type == "XYPosLoop":
                     loop = c
@@ -697,14 +671,15 @@
         return [p.name or f"XYPos:{i}" for i, p in enumerate(loop.parameters.points)]
 
     @property
     def _channel_names(self) -> list[str]:
         return self._rdr.channel_names()
 
     def __repr__(self) -> str:
+        """Return a string representation of the ND2File."""
         try:
             details = " (closed)" if self.closed else f" {self.dtype}: {self.sizes!r}"
             extra = f": {Path(self.path).name!r}{details}"
         except Exception:
             extra = ""
         return f"<ND2File at {hex(id(self))}{extra}>"
 
@@ -717,79 +692,22 @@
         Recorded Data tab of the NIS Viewer.
 
         (There will be a column for each tag in the `CustomDataV2_0` section of
         `ND2File.custom_data`)
 
         Legacy ND2 files are not supported.
         """
-        if self.is_legacy:
-            warnings.warn(
-                "`recorded_data` is not supported for legacy ND2 files", UserWarning
-            )
-            return {}
-        rdr = cast("LatestSDKReader", self._rdr)
-
-        cd = self.custom_data
-        if "CustomDataV2_0" not in cd:
-            return {}
-        try:
-            tags: dict = cd["CustomDataV2_0"]["CustomTagDescription_v1.0"]
-        except KeyError:
+        if self.is_legacy:  # pragma: no cover
             warnings.warn(
-                "Could not find 'CustomTagDescription_v1' tag, please open an issue "
-                "with this nd2 file at https://github.com/tlambert03/nd2/issues/new",
+                "`recorded_data` is not supported for legacy ND2 files",
+                UserWarning,
+                stacklevel=2,
             )
             return {}
-
-        # tags will be a dict of dicts: eg:
-        # {'Tag0': {'ID': 'X', 'Type': 3, 'Group': 1, 'Size': 5000, 'Desc': 'X Coord', 'Unit': 'µm'}}  # noqa
-        # FIXME: technically, it is possible to have multiple tags with the same Desc
-        # (e.g. for IDs PFS_OFFSET and Z2). In the current implementation, the
-        # 2nd tag will overwrite the first one.
-        data: dict[str, np.ndarray | Sequence] = {}
-        with contextlib.suppress(KeyError):
-            chunk = rdr._get_meta_chunk("CustomData|AcqTimesCache")
-            data["Time [s]"] = np.frombuffer(chunk) / 1000
-
-        try:
-            z_idx = [AXIS._MAP[c[1]] for c in self._rdr._coord_info()].index(AXIS.Z)
-        except ValueError:
-            pass
-        else:
-            # TODO: this is probably slow... and could definitely be improved
-            z_loop = cast("ZStackLoop", self.experiment[z_idx])
-            z_positions = [
-                z_loop.parameters.stepUm * (i - z_loop.parameters.homeIndex)
-                for i in range(z_loop.count)
-            ]
-            if not z_loop.parameters.bottomToTop:
-                z_positions = list(reversed(z_positions))
-
-            data["Z-Series"] = np.array(
-                [
-                    z_positions[rdr._coords_from_seq_index(i)[z_idx]]
-                    for i in range(self.attributes.sequenceCount)
-                ]
-            )
-
-        for tag in tags.values():
-            header = f"{tag['Desc']}"
-            if tag["Unit"]:
-                header += f" [{tag['Unit']}]"
-            raw = rdr._get_meta_chunk(f"CustomData|{tag['ID']}")
-            _type = tag["Type"]
-            if _type == 1:
-                warnings.warn(
-                    f"{header!r} column skipped: "
-                    "(parsing string data is not yet implemented)"
-                )
-            else:
-                data[header] = _decode_custom_data(raw, _type, tag["Size"])
-
-        return data
+        return cast("LatestSDKReader", self._rdr).recorded_data()
 
     @cached_property
     def binary_data(self) -> BinaryLayers | None:
         """Return binary layers embedded in the file.
 
         The returned `BinaryLayers` object is an immutable sequence of `BinaryLayer`
         objects, one for each binary layer in the file.  Each `BinaryLayer` object in
@@ -865,15 +783,15 @@
 def imread(
     file: Path | str,
     *,
     dask: bool = False,
     xarray: bool = False,
     validate_frames: bool = False,
     read_using_sdk: bool | None = None,
-):
+) -> np.ndarray | xr.DataArray | dask.array.core.Array:
     """Open `file`, return requested array type, and close `file`.
 
     Parameters
     ----------
     file : Union[Path, str]
         Filepath (`str`) or `Path` object to ND2 file.
     dask : bool
@@ -888,14 +806,15 @@
         By default `False`.
     validate_frames : bool
         Whether to verify (and attempt to fix) frames whose positions have been
         shifted relative to the predicted offset (i.e. in a corrupted file).
         This comes at a slight performance penalty at file open, but may "rescue"
         some corrupt files. by default False.
     read_using_sdk : Optional[bool]
+        DEPRECATED: no longer used.
         If `True`, use the SDK to read the file. If `False`, inspects the chunkmap and
         reads from a `numpy.memmap`. If `None` (the default), uses the SDK if the file
         is compressed, otherwise uses the memmap.
         Note: using `read_using_sdk=False` on a compressed file will result in a
         ValueError.
 
     Returns
@@ -908,24 +827,7 @@
     ) as nd2:
         if xarray:
             return nd2.to_xarray(delayed=dask)
         elif dask:
             return nd2.to_dask()
         else:
             return nd2.asarray()
-
-
-@no_type_check
-def _fix_names(xy_exp, points: list[Position]) -> None:
-    """Attempt to fix missing XYPosLoop position names."""
-    if not isinstance(xy_exp, dict) or xy_exp.get("Type", "") != 2:
-        raise ValueError("Invalid XY experiment")
-    _points = xy_exp["LoopPars"]["Points"]
-    if len(_points) == 1 and "" in _points:
-        _points = _points[""]
-    if not isinstance(_points, list):
-        _points = [_points]
-    _names = {(p["PosX"], p["PosY"], p["PosZ"]): p["PosName"] for p in _points}
-
-    for p in points:
-        if p.name is None:
-            p.name = _names.get(tuple(p.stagePositionUm), p.name)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nd2-0.5.3/src/nd2/structures.py` & `nd2-0.6.0/src/nd2/structures.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,105 +1,133 @@
 from __future__ import annotations
 
 import builtins
 from dataclasses import dataclass, field
-from enum import Enum, IntEnum
-from typing import TYPE_CHECKING, NamedTuple, Union
+from enum import IntEnum
+from typing import NamedTuple, Union
 
-from typing_extensions import Literal
+from typing_extensions import Literal, TypeAlias, TypedDict
 
-if TYPE_CHECKING:
-    pass
 
-# enums
+class TextInfo(TypedDict, total=False):
+    imageId: str
+    type: str
+    group: str
+    sampleId: str
+    author: str
+    description: str
+    capturing: str
+    sampling: str
+    location: str
+    date: str
+    conclusion: str
+    info1: str
+    info2: str
+    optics: str
+    appVersion: str
 
 
 class LoopType(IntEnum):
-    NETimeLoop = 8
+    Unknown = 0
+    TimeLoop = 1
     XYPosLoop = 2
-    ZStackLoop = 6
-    TimeLoop = 1  # not sure about this
-    Unknown = 4  # not sure about this
+    XYDiscrLoop = 3
+    ZStackLoop = 4
+    PolarLoop = 5
+    SpectLoop = 6
+    CustomLoop = 7
+    NETimeLoop = 8
+    ManTimeLoop = 9
+    ZStackLoopAccurate = 10
 
 
-class AxisInterpretation(str, Enum):
-    distance = "distance"
-    time = "time"
+AxisInterpretation: TypeAlias = Literal["distance", "time"]
 
 
 # tuples
 
 
 class Attributes(NamedTuple):
     bitsPerComponentInMemory: int
     bitsPerComponentSignificant: int
     componentCount: int
     heightPx: int
-    pixelDataType: str
+    pixelDataType: Literal["float", "unsigned"]
     sequenceCount: int
     widthBytes: int | None = None
     widthPx: int | None = None
-    compressionLevel: int | None = None
-    compressionType: str | None = None
+    compressionLevel: float | None = None
+    compressionType: Literal["lossless", "lossy", "none"] | None = None
     tileHeightPx: int | None = None
     tileWidthPx: int | None = None
     channelCount: int | None = None
 
 
 class ImageInfo(NamedTuple):
     width: int
     height: int
     components: int
     bits_per_pixel: int
 
 
 # experiment #################
 
-
-LoopTypeString = Union[
-    Literal["TimeLoop"],
-    Literal["NETimeLoop"],
-    Literal["XYPosLoop"],
-    Literal["ZStackLoop"],
+LoopTypeString = Literal[
+    "Unknown",
+    "TimeLoop",
+    "XYPosLoop",
+    "XYDiscrLoop",
+    "ZStackLoop",
+    "PolarLoop",
+    "SpectLoop",
+    "CustomLoop",
+    "NETimeLoop",
+    "ManTimeLoop",
+    "ZStackLoopAccurate",
 ]
 
 
 @dataclass
 class _Loop:
     count: int
     nestingLevel: int
     parameters: LoopParams
     type: LoopTypeString
 
-    @classmethod
-    def create(cls, obj: dict) -> ExpLoop:
-        return globals()[obj["type"]](**obj)
+
+@dataclass
+class SpectLoop:
+    count: int
+    type: Literal["SpectLoop"] = "SpectLoop"
 
 
 #####
 
 
 @dataclass
 class TimeLoop(_Loop):
     parameters: TimeLoopParams
     type: Literal["TimeLoop"] = "TimeLoop"
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
+        # TODO: make superclass do this
         if isinstance(self.parameters, dict):
+            if "periodDiff" not in self.parameters:
+                self.parameters["periodDiff"] = None
             self.parameters = TimeLoopParams(**self.parameters)
 
 
 @dataclass
 class TimeLoopParams:
     startMs: float
     periodMs: float
     durationMs: float
     periodDiff: PeriodDiff
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         if isinstance(self.periodDiff, dict):
             self.periodDiff = PeriodDiff(**self.periodDiff)
 
 
 @dataclass
 class PeriodDiff:
     avg: float = 0
@@ -111,24 +139,24 @@
 
 
 @dataclass
 class NETimeLoop(_Loop):
     parameters: NETimeLoopParams
     type: Literal["NETimeLoop"] = "NETimeLoop"
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         if isinstance(self.parameters, dict):
             self.parameters = NETimeLoopParams(**self.parameters)
 
 
 @dataclass
 class NETimeLoopParams:
     periods: list[Period]
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         self.periods = [Period(**i) if isinstance(i, dict) else i for i in self.periods]
 
 
 @dataclass
 class Period(TimeLoopParams):
     count: int
 
@@ -137,37 +165,39 @@
 
 
 @dataclass
 class XYPosLoop(_Loop):
     parameters: XYPosLoopParams
     type: Literal["XYPosLoop"] = "XYPosLoop"
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         if isinstance(self.parameters, dict):
             self.parameters = XYPosLoopParams(**self.parameters)
 
 
 @dataclass
 class XYPosLoopParams:
     isSettingZ: bool
     points: list[Position]
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         self.points = [Position(**i) if isinstance(i, dict) else i for i in self.points]
 
 
 @dataclass
 class Position:
     stagePositionUm: StagePosition
     pfsOffset: float | None = None
     name: str | None = None
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         if isinstance(self.stagePositionUm, dict):
             self.stagePositionUm = StagePosition(*self.stagePositionUm)
+        elif isinstance(self.stagePositionUm, (tuple, list)):
+            self.stagePositionUm = StagePosition(*self.stagePositionUm)
 
 
 class StagePosition(NamedTuple):
     x: float
     y: float
     z: float
 
@@ -176,15 +206,15 @@
 
 
 @dataclass
 class ZStackLoop(_Loop):
     parameters: ZStackLoopParams
     type: Literal["ZStackLoop"] = "ZStackLoop"
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         if isinstance(self.parameters, dict):
             self.parameters = ZStackLoopParams(**self.parameters)
 
 
 @dataclass
 class ZStackLoopParams:
     homeIndex: int
@@ -202,15 +232,15 @@
 
 
 @dataclass
 class Metadata:
     contents: Contents | None = None
     channels: list[Channel] | None = None
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         if isinstance(self.contents, dict):
             self.contents = Contents(**self.contents)
         if self.channels:
             self.channels = [
                 Channel(**i) if isinstance(i, dict) else i for i in self.channels
             ]
 
@@ -224,19 +254,22 @@
 @dataclass
 class Channel:
     channel: ChannelMeta
     loops: LoopIndices | None
     microscope: Microscope
     volume: Volume
 
-    def __post_init__(self):
-        self.channel = ChannelMeta(**self.channel)
-        self.microscope = Microscope(**self.microscope)
-        self.volume = Volume(**self.volume)
-        if self.loops:
+    def __post_init__(self) -> None:
+        if isinstance(self.channel, dict):
+            self.channel = ChannelMeta(**self.channel)
+        if isinstance(self.microscope, dict):
+            self.microscope = Microscope(**self.microscope)
+        if isinstance(self.volume, dict):
+            self.volume = Volume(**self.volume)
+        if isinstance(self.loops, dict):
             self.loops = LoopIndices(**self.loops)
 
 
 @dataclass
 class ChannelMeta:
     name: str
     index: int
@@ -272,60 +305,60 @@
     axesInterpretation: tuple[
         AxisInterpretation, AxisInterpretation, AxisInterpretation
     ]
     bitsPerComponentInMemory: int
     bitsPerComponentSignificant: int
     cameraTransformationMatrix: tuple[float, float, float, float]
     componentCount: int
-    componentDataType: Literal["unsigned"] | Literal["float"]
+    componentDataType: Literal["unsigned", "float"]
     voxelCount: tuple[int, int, int]
     componentMaxima: list[float] | None = None
     componentMinima: list[float] | None = None
     pixelToStageTransformationMatrix: tuple[
         float, float, float, float, float, float
     ] | None = None
 
     # NIS Microscope Absolute frame in um =
     # pixelToStageTransformationMatrix * (X_in_px,  Y_in_px,  1) + stagePositionUm
 
-    def __post_init__(self):
-        self.axesInterpretation = tuple(  # type: ignore
-            AxisInterpretation(i) for i in self.axesInterpretation
-        )
-
 
 @dataclass
 class TimeStamp:
     absoluteJulianDayNumber: float
     relativeTimeMs: float
 
 
 @dataclass
 class FrameChannel(Channel):
     position: Position
     time: TimeStamp
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         super().__post_init__()
-        self.position = Position(**self.position)
-        self.time = TimeStamp(**self.time)
+        if isinstance(self.position, dict):
+            self.position = Position(**self.position)
+        if isinstance(self.time, dict):
+            self.time = TimeStamp(**self.time)
 
 
 @dataclass
 class FrameMetadata:
     contents: Contents
     channels: list[FrameChannel]
 
-    def __post_init__(self):
-        self.contents = Contents(**self.contents)
-        self.channels = [FrameChannel(**i) for i in self.channels]
+    def __post_init__(self) -> None:
+        if isinstance(self.contents, dict):
+            self.contents = Contents(**self.contents)
+        self.channels = [
+            FrameChannel(**i) if isinstance(i, dict) else i for i in self.channels
+        ]
 
 
 class Coordinate(NamedTuple):
-    index: int
+    index: int  # type: ignore
     type: str
     size: int
 
 
 def _lower0(x: str) -> str:
     return x[0].lower() + x[1:]
 
@@ -367,46 +400,47 @@
     """ROI object from NIS Elements."""
 
     id: int
     info: RoiInfo
     guid: str
     animParams: list[AnimParam] = field(default_factory=list)
 
-    def __post_init__(self):
-        self.info = RoiInfo(**self.info)
-        self.animParams = [AnimParam(**i) for i in self.animParams]
+    def __post_init__(self) -> None:
+        if isinstance(self.info, dict):
+            self.info = RoiInfo(**self.info)
+        self.animParams = [AnimParam(**i) for i in self.animParams]  # type: ignore
 
     @classmethod
     def _from_meta_dict(cls, val: dict) -> ROI:
         anim_params = [
             {_lower0(k): v for k, v in val[f"AnimParams_{i}"].items()}
             for i in range(val.pop("AnimParams_Size", 0))
         ]
         return cls(
             id=val["Id"],
-            info={_lower0(k): v for k, v in val["Info"].items()},
+            info={_lower0(k): v for k, v in val["Info"].items()},  # type: ignore
             guid=val.get("GUID", ""),
-            animParams=anim_params,
+            animParams=anim_params,  # type: ignore
         )
 
 
 @dataclass
 class AnimParam:
     """Parameters of ROI position/shape."""
 
     timeMs: float = 0
     enabled: bool = True
     centerX: float = 0
     centerY: float = 0
     centerZ: float = 0
     rotationZ: float = 0
-    boxShape: BoxShape = BoxShape()
-    extrudedShape: ExtrudedShape = ExtrudedShape()
+    boxShape: BoxShape = field(default_factory=BoxShape)
+    extrudedShape: ExtrudedShape = field(default_factory=ExtrudedShape)
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         if isinstance(self.boxShape, dict):
             self.boxShape = BoxShape(
                 **{_lower0(k): v for k, v in self.boxShape.items()}
             )
         if isinstance(self.extrudedShape, dict):
             self.extrudedShape = ExtrudedShape._from_meta_dict(self.extrudedShape)
 
@@ -460,15 +494,15 @@
     bpc: int = 16
     autodetected: bool = False
     gradientStimulation: bool = False
     gradientStimulationBitDepth: int = 0
     gradientStimulationLo: float = 0.0
     gradientStimulationHi: float = 0.0
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         # coerce types
         for key, anno in self.__annotations__.items():
             if key == "shapeType":
                 self.shapeType = RoiShapeType(self.shapeType)
             elif key == "interpType":
                 self.interpType = InterpType(self.interpType)
             else:
```

