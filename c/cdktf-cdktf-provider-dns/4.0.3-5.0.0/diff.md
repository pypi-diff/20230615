# Comparing `tmp/cdktf-cdktf-provider-dns-4.0.3.tar.gz` & `tmp/cdktf-cdktf-provider-dns-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-dns-4.0.3.tar", last modified: Thu Jun  1 14:14:55 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-dns-5.0.0.tar", last modified: Thu Jun 15 11:20:10 2023, max compression
```

## Comparing `cdktf-cdktf-provider-dns-4.0.3.tar` & `cdktf-cdktf-provider-dns-5.0.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:55.216738 cdktf-cdktf-provider-dns-4.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-01 14:14:40.000000 cdktf-cdktf-provider-dns-4.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 14:14:40.000000 cdktf-cdktf-provider-dns-4.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-06-01 14:14:55.216738 cdktf-cdktf-provider-dns-4.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-06-01 14:14:40.000000 cdktf-cdktf-provider-dns-4.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 14:14:40.000000 cdktf-cdktf-provider-dns-4.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:14:55.216738 cdktf-cdktf-provider-dns-4.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-01 14:14:40.000000 cdktf-cdktf-provider-dns-4.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:55.204738 cdktf-cdktf-provider-dns-4.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:55.208738 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-06-01 14:14:40.000000 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:55.212738 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-01 14:14:40.000000 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71881 2023-06-01 14:14:40.000000 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/_jsii/provider-dns@4.0.3.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:55.212738 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/a_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    24858 2023-06-01 14:14:40.000000 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/a_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:55.212738 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/aaaa_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    24999 2023-06-01 14:14:40.000000 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/aaaa_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:55.212738 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/cname_record/
--rw-r--r--   0 runner    (1001) docker     (123)    21468 2023-06-01 14:14:40.000000 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/cname_record/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:55.212738 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/data_dns_a_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    15014 2023-06-01 14:14:40.000000 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/data_dns_a_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:55.212738 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/data_dns_aaaa_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    15083 2023-06-01 14:14:40.000000 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/data_dns_aaaa_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:55.212738 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/data_dns_cname_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-06-01 14:14:40.000000 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/data_dns_cname_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:55.212738 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/data_dns_mx_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    23949 2023-06-01 14:14:40.000000 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/data_dns_mx_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:55.212738 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/data_dns_ns_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    15055 2023-06-01 14:14:40.000000 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/data_dns_ns_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:55.212738 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/data_dns_ptr_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-06-01 14:14:40.000000 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/data_dns_ptr_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:55.212738 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/data_dns_srv_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    24360 2023-06-01 14:14:40.000000 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/data_dns_srv_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:55.212738 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/data_dns_txt_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    15232 2023-06-01 14:14:40.000000 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/data_dns_txt_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:55.216738 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/mx_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    36579 2023-06-01 14:14:40.000000 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/mx_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:55.216738 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/ns_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    21884 2023-06-01 14:14:40.000000 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/ns_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:55.216738 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    26543 2023-06-01 14:14:40.000000 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:55.216738 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/ptr_record/
--rw-r--r--   0 runner    (1001) docker     (123)    21564 2023-06-01 14:14:40.000000 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/ptr_record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:14:40.000000 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:55.216738 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/srv_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    39920 2023-06-01 14:14:40.000000 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/srv_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:55.216738 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/txt_record_set/
--rw-r--r--   0 runner    (1001) docker     (123)    21911 2023-06-01 14:14:40.000000 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/txt_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:55.212738 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-06-01 14:14:55.000000 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-01 14:14:55.000000 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:14:55.000000 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 14:14:55.000000 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-01 14:14:55.000000 cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:10.540142 cdktf-cdktf-provider-dns-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-15 11:19:52.000000 cdktf-cdktf-provider-dns-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 11:19:52.000000 cdktf-cdktf-provider-dns-5.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-06-15 11:20:10.540142 cdktf-cdktf-provider-dns-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-06-15 11:19:52.000000 cdktf-cdktf-provider-dns-5.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 11:19:52.000000 cdktf-cdktf-provider-dns-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:20:10.540142 cdktf-cdktf-provider-dns-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-15 11:19:52.000000 cdktf-cdktf-provider-dns-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:10.528143 cdktf-cdktf-provider-dns-5.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:10.532142 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-06-15 11:19:52.000000 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:10.536142 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-15 11:19:52.000000 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71877 2023-06-15 11:19:52.000000 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/_jsii/provider-dns@5.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:10.536142 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/a_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    24858 2023-06-15 11:19:52.000000 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/a_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:10.536142 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/aaaa_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    24999 2023-06-15 11:19:52.000000 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/aaaa_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:10.536142 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/cname_record/
+-rw-r--r--   0 runner    (1001) docker     (123)    21468 2023-06-15 11:19:52.000000 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/cname_record/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:10.536142 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/data_dns_a_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    15014 2023-06-15 11:19:52.000000 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/data_dns_a_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:10.536142 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/data_dns_aaaa_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    15083 2023-06-15 11:19:52.000000 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/data_dns_aaaa_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:10.536142 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/data_dns_cname_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-06-15 11:19:52.000000 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/data_dns_cname_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:10.536142 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/data_dns_mx_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    23949 2023-06-15 11:19:52.000000 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/data_dns_mx_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:10.536142 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/data_dns_ns_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    15055 2023-06-15 11:19:52.000000 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/data_dns_ns_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:10.536142 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/data_dns_ptr_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-06-15 11:19:52.000000 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/data_dns_ptr_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:10.536142 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/data_dns_srv_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    24360 2023-06-15 11:19:52.000000 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/data_dns_srv_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:10.536142 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/data_dns_txt_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    15232 2023-06-15 11:19:52.000000 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/data_dns_txt_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:10.536142 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/mx_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    36579 2023-06-15 11:19:52.000000 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/mx_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:10.536142 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/ns_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    21884 2023-06-15 11:19:52.000000 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/ns_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:10.536142 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    26543 2023-06-15 11:19:52.000000 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:10.540142 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/ptr_record/
+-rw-r--r--   0 runner    (1001) docker     (123)    21564 2023-06-15 11:19:52.000000 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/ptr_record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:19:52.000000 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:10.540142 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/srv_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    39920 2023-06-15 11:19:52.000000 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/srv_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:10.540142 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/txt_record_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    21911 2023-06-15 11:19:52.000000 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/txt_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:10.536142 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-06-15 11:20:10.000000 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-15 11:20:10.000000 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:20:10.000000 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 11:20:10.000000 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 11:20:10.000000 cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-dns-4.0.3/LICENSE` & `cdktf-cdktf-provider-dns-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dns-4.0.3/PKG-INFO` & `cdktf-cdktf-provider-dns-5.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-dns
-Version: 4.0.3
+Version: 5.0.0
 Summary: Prebuilt dns Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-dns.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-dns.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-dns-4.0.3/README.md` & `cdktf-cdktf-provider-dns-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dns-4.0.3/setup.py` & `cdktf-cdktf-provider-dns-5.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-dns",
-    "version": "4.0.3",
+    "version": "5.0.0",
     "description": "Prebuilt dns Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-dns.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -39,25 +39,25 @@
         "cdktf_cdktf_provider_dns.provider",
         "cdktf_cdktf_provider_dns.ptr_record",
         "cdktf_cdktf_provider_dns.srv_record_set",
         "cdktf_cdktf_provider_dns.txt_record_set"
     ],
     "package_data": {
         "cdktf_cdktf_provider_dns._jsii": [
-            "provider-dns@4.0.3.jsii.tgz"
+            "provider-dns@5.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_dns": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "cdktf>=0.16.3, <0.17.0",
+        "cdktf>=0.17.0, <0.18.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.81.0, <2.0.0",
+        "jsii>=1.84.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/__init__.py` & `cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/a_record_set/__init__.py` & `cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/a_record_set/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/aaaa_record_set/__init__.py` & `cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/aaaa_record_set/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/cname_record/__init__.py` & `cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/cname_record/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/data_dns_a_record_set/__init__.py` & `cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/data_dns_a_record_set/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/data_dns_aaaa_record_set/__init__.py` & `cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/data_dns_aaaa_record_set/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/data_dns_cname_record_set/__init__.py` & `cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/data_dns_cname_record_set/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/data_dns_mx_record_set/__init__.py` & `cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/data_dns_mx_record_set/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/data_dns_ns_record_set/__init__.py` & `cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/data_dns_ns_record_set/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/data_dns_ptr_record_set/__init__.py` & `cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/data_dns_ptr_record_set/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/data_dns_srv_record_set/__init__.py` & `cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/data_dns_srv_record_set/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/data_dns_txt_record_set/__init__.py` & `cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/data_dns_txt_record_set/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/mx_record_set/__init__.py` & `cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/mx_record_set/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/ns_record_set/__init__.py` & `cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/ns_record_set/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/provider/__init__.py` & `cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/ptr_record/__init__.py` & `cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/ptr_record/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/srv_record_set/__init__.py` & `cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/srv_record_set/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns/txt_record_set/__init__.py` & `cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns/txt_record_set/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns.egg-info/PKG-INFO` & `cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-dns
-Version: 4.0.3
+Version: 5.0.0
 Summary: Prebuilt dns Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-dns.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-dns.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-dns-4.0.3/src/cdktf_cdktf_provider_dns.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-dns-5.0.0/src/cdktf_cdktf_provider_dns.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_dns/py.typed
 src/cdktf_cdktf_provider_dns.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_dns.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_dns.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_dns.egg-info/requires.txt
 src/cdktf_cdktf_provider_dns.egg-info/top_level.txt
 src/cdktf_cdktf_provider_dns/_jsii/__init__.py
-src/cdktf_cdktf_provider_dns/_jsii/provider-dns@4.0.3.jsii.tgz
+src/cdktf_cdktf_provider_dns/_jsii/provider-dns@5.0.0.jsii.tgz
 src/cdktf_cdktf_provider_dns/a_record_set/__init__.py
 src/cdktf_cdktf_provider_dns/aaaa_record_set/__init__.py
 src/cdktf_cdktf_provider_dns/cname_record/__init__.py
 src/cdktf_cdktf_provider_dns/data_dns_a_record_set/__init__.py
 src/cdktf_cdktf_provider_dns/data_dns_aaaa_record_set/__init__.py
 src/cdktf_cdktf_provider_dns/data_dns_cname_record_set/__init__.py
 src/cdktf_cdktf_provider_dns/data_dns_mx_record_set/__init__.py
```

