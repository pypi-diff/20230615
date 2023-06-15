# Comparing `tmp/sentry_cli-2.19.0.tar.gz` & `tmp/sentry_cli-2.19.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_cli-2.19.0.tar", last modified: Wed Jun 14 08:24:55 2023, max compression
+gzip compressed data, was "sentry_cli-2.19.1.tar", last modified: Thu Jun 15 07:53:02 2023, max compression
```

## Comparing `sentry_cli-2.19.0.tar` & `sentry_cli-2.19.1.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.784309 sentry_cli-2.19.0/
--rw-r--r--   0 runner    (1001) docker     (123)    80839 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-14 08:24:55.784309 sentry_cli-2.19.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.768309 sentry_cli-2.19.0/sentry_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-14 08:24:55.000000 sentry_cli-2.19.0/sentry_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-14 08:24:55.000000 sentry_cli-2.19.0/sentry_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:24:55.000000 sentry_cli-2.19.0/sentry_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:24:55.000000 sentry_cli-2.19.0/sentry_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-14 08:24:55.788309 sentry_cli-2.19.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.768309 sentry_cli-2.19.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)    87192 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/api.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/bashsupport.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.768309 sentry_cli-2.19.0/src/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/bash_hook.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.772309 sentry_cli-2.19.0/src/commands/debug_files/
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/debug_files/bundle_jvm.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/debug_files/bundle_sources.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/debug_files/check.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/debug_files/find.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/debug_files/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/debug_files/print_sources.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14830 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/debug_files/upload.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.772309 sentry_cli-2.19.0/src/commands/deploys/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/deploys/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/deploys/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/deploys/new.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.772309 sentry_cli-2.19.0/src/commands/events/
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/events/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/events/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.772309 sentry_cli-2.19.0/src/commands/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/files/delete.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/files/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/files/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/files/upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/info.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.772309 sentry_cli-2.19.0/src/commands/issues/
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/issues/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/issues/mute.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/issues/resolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/issues/unresolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/login.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.776309 sentry_cli-2.19.0/src/commands/monitors/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/monitors/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/monitors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/monitors/run.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.776309 sentry_cli-2.19.0/src/commands/organizations/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/organizations/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/organizations/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.776309 sentry_cli-2.19.0/src/commands/projects/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/projects/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/projects/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.776309 sentry_cli-2.19.0/src/commands/react_native/
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/react_native/appcenter.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/react_native/gradle.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/react_native/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/react_native/xcode.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.776309 sentry_cli-2.19.0/src/commands/releases/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/releases/archive.rs
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/releases/delete.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/releases/finalize.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/releases/info.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/releases/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/releases/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/releases/new.rs
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/releases/propose_version.rs
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/releases/restore.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/releases/set_commits.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.780309 sentry_cli-2.19.0/src/commands/repos/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/repos/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/repos/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/send_envelope.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/send_event.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.780309 sentry_cli-2.19.0/src/commands/sourcemaps/
--rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/sourcemaps/explain.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/sourcemaps/inject.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/sourcemaps/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/sourcemaps/resolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/sourcemaps/upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/uninstall.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/update.rs
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/upload_dif.rs
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/upload_dsym.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/upload_proguard.rs
--rw-r--r--   0 runner    (1001) docker     (123)    20882 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/config.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/constants.rs
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.784309 sentry_cli-2.19.0/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/android.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/appcenter.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/args.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/chunks.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/codepush.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/cordova.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/dif.rs
--rw-r--r--   0 runner    (1001) docker     (123)    72888 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/dif_upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/enc.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/event.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/file_search.rs
--rw-r--r--   0 runner    (1001) docker     (123)    17036 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/file_upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/formatting.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/fs.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/http.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/logging.rs
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/progress.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/releases.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/retry.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.784309 sentry_cli-2.19.0/src/utils/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_previous_commit.snap
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.784309 sentry_cli-2.19.0/src/utils/sourcemaps/
--rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/sourcemaps/inject.rs
--rw-r--r--   0 runner    (1001) docker     (123)    38886 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/sourcemaps.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/system.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/ui.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/update.rs
--rw-r--r--   0 runner    (1001) docker     (123)    36048 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/vcs.rs
--rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/xcode.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.050466 sentry_cli-2.19.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    80839 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-15 07:53:02.050466 sentry_cli-2.19.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.038466 sentry_cli-2.19.1/sentry_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-15 07:53:02.000000 sentry_cli-2.19.1/sentry_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-15 07:53:02.000000 sentry_cli-2.19.1/sentry_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:53:02.000000 sentry_cli-2.19.1/sentry_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:53:02.000000 sentry_cli-2.19.1/sentry_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-15 07:53:02.050466 sentry_cli-2.19.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.038466 sentry_cli-2.19.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    87192 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/api.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/bashsupport.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.042466 sentry_cli-2.19.1/src/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/bash_hook.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.042466 sentry_cli-2.19.1/src/commands/debug_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/debug_files/bundle_jvm.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/debug_files/bundle_sources.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/debug_files/check.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/debug_files/find.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/debug_files/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/debug_files/print_sources.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14830 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/debug_files/upload.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.042466 sentry_cli-2.19.1/src/commands/deploys/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/deploys/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/deploys/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/deploys/new.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.042466 sentry_cli-2.19.1/src/commands/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/events/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/events/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.042466 sentry_cli-2.19.1/src/commands/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/files/delete.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/files/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/files/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/files/upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/info.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.042466 sentry_cli-2.19.1/src/commands/issues/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/issues/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/issues/mute.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/issues/resolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/issues/unresolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/login.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.046466 sentry_cli-2.19.1/src/commands/monitors/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/monitors/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/monitors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/monitors/run.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.046466 sentry_cli-2.19.1/src/commands/organizations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/organizations/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/organizations/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.046466 sentry_cli-2.19.1/src/commands/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/projects/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/projects/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.046466 sentry_cli-2.19.1/src/commands/react_native/
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/react_native/appcenter.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/react_native/gradle.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/react_native/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/react_native/xcode.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.046466 sentry_cli-2.19.1/src/commands/releases/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/releases/archive.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/releases/delete.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/releases/finalize.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/releases/info.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/releases/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/releases/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/releases/new.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/releases/propose_version.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/releases/restore.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/releases/set_commits.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.046466 sentry_cli-2.19.1/src/commands/repos/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/repos/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/repos/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/send_envelope.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/send_event.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.046466 sentry_cli-2.19.1/src/commands/sourcemaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/sourcemaps/explain.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/sourcemaps/inject.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/sourcemaps/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/sourcemaps/resolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/sourcemaps/upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/uninstall.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/update.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/upload_dif.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/upload_dsym.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/commands/upload_proguard.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    20882 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/config.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/constants.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.050466 sentry_cli-2.19.1/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/android.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/appcenter.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/args.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/chunks.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/codepush.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/cordova.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/dif.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    72888 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/dif_upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/enc.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/event.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/file_search.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    17036 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/file_upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/formatting.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/fs.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/http.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/logging.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/progress.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/releases.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/retry.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.050466 sentry_cli-2.19.1/src/utils/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_previous_commit.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:53:02.050466 sentry_cli-2.19.1/src/utils/sourcemaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    19220 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/sourcemaps/inject.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    38886 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/sourcemaps.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/system.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/ui.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/update.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    36048 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/vcs.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-06-15 07:52:47.000000 sentry_cli-2.19.1/src/utils/xcode.rs
```

### Comparing `sentry_cli-2.19.0/Cargo.lock` & `sentry_cli-2.19.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2191,15 +2191,15 @@
  "once_cell",
  "regex",
  "sentry-core",
 ]
 
 [[package]]
 name = "sentry-cli"
-version = "2.19.0"
+version = "2.19.1"
 dependencies = [
  "anyhow",
  "anylog",
  "backoff",
  "backtrace",
  "brotli2",
  "bytecount",
```

### Comparing `sentry_cli-2.19.0/Cargo.toml` & `sentry_cli-2.19.1/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [package]
 authors = ["Armin Ronacher <armin.ronacher@active-4.com>"]
 build = "build.rs"
 name = "sentry-cli"
-version = "2.19.0"
+version = "2.19.1"
 edition = "2021"
 rust-version = "1.65"
 
 [dependencies]
 anylog = "0.6.3"
 anyhow = { version = "1.0.69", features = ["backtrace"] }
 backoff = "0.4.0"
```

### Comparing `sentry_cli-2.19.0/LICENSE` & `sentry_cli-2.19.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/PKG-INFO` & `sentry_cli-2.19.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry_cli
-Version: 2.19.0
+Version: 2.19.1
 Summary: A command line utility to work with Sentry.
 Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry
 Author-email: oss@sentry.io
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry_cli Version: 2.19.0 Summary: A command line
+Metadata-Version: 2.1 Name: sentry_cli Version: 2.19.1 Summary: A command line
 utility to work with Sentry. Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry Author-email: oss@sentry.io License: BSD-3-Clause Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `sentry_cli-2.19.0/README.md` & `sentry_cli-2.19.1/README.md`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/build.rs` & `sentry_cli-2.19.1/build.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/sentry_cli.egg-info/PKG-INFO` & `sentry_cli-2.19.1/sentry_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-cli
-Version: 2.19.0
+Version: 2.19.1
 Summary: A command line utility to work with Sentry.
 Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry
 Author-email: oss@sentry.io
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry-cli Version: 2.19.0 Summary: A command line
+Metadata-Version: 2.1 Name: sentry-cli Version: 2.19.1 Summary: A command line
 utility to work with Sentry. Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry Author-email: oss@sentry.io License: BSD-3-Clause Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `sentry_cli-2.19.0/sentry_cli.egg-info/SOURCES.txt` & `sentry_cli-2.19.1/sentry_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/setup.cfg` & `sentry_cli-2.19.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/setup.py` & `sentry_cli-2.19.1/setup.py`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/api.rs` & `sentry_cli-2.19.1/src/api.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/bashsupport.sh` & `sentry_cli-2.19.1/src/bashsupport.sh`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/bash_hook.rs` & `sentry_cli-2.19.1/src/commands/bash_hook.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/debug_files/bundle_jvm.rs` & `sentry_cli-2.19.1/src/commands/debug_files/bundle_jvm.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/debug_files/bundle_sources.rs` & `sentry_cli-2.19.1/src/commands/debug_files/bundle_sources.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/debug_files/check.rs` & `sentry_cli-2.19.1/src/commands/debug_files/check.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/debug_files/find.rs` & `sentry_cli-2.19.1/src/commands/debug_files/find.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/debug_files/mod.rs` & `sentry_cli-2.19.1/src/commands/debug_files/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/debug_files/print_sources.rs` & `sentry_cli-2.19.1/src/commands/debug_files/print_sources.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/debug_files/upload.rs` & `sentry_cli-2.19.1/src/commands/debug_files/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/deploys/list.rs` & `sentry_cli-2.19.1/src/commands/deploys/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/deploys/mod.rs` & `sentry_cli-2.19.1/src/commands/deploys/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/deploys/new.rs` & `sentry_cli-2.19.1/src/commands/deploys/new.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/events/list.rs` & `sentry_cli-2.19.1/src/commands/events/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/events/mod.rs` & `sentry_cli-2.19.1/src/commands/events/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/files/delete.rs` & `sentry_cli-2.19.1/src/commands/files/delete.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/files/list.rs` & `sentry_cli-2.19.1/src/commands/files/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/files/mod.rs` & `sentry_cli-2.19.1/src/commands/files/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/files/upload.rs` & `sentry_cli-2.19.1/src/commands/files/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/info.rs` & `sentry_cli-2.19.1/src/commands/info.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/issues/mod.rs` & `sentry_cli-2.19.1/src/commands/issues/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/issues/mute.rs` & `sentry_cli-2.19.1/src/commands/issues/mute.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/issues/resolve.rs` & `sentry_cli-2.19.1/src/commands/issues/resolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/issues/unresolve.rs` & `sentry_cli-2.19.1/src/commands/issues/unresolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/login.rs` & `sentry_cli-2.19.1/src/commands/login.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/mod.rs` & `sentry_cli-2.19.1/src/commands/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/monitors/list.rs` & `sentry_cli-2.19.1/src/commands/monitors/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/monitors/mod.rs` & `sentry_cli-2.19.1/src/commands/monitors/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/monitors/run.rs` & `sentry_cli-2.19.1/src/commands/monitors/run.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/organizations/list.rs` & `sentry_cli-2.19.1/src/commands/organizations/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/organizations/mod.rs` & `sentry_cli-2.19.1/src/commands/organizations/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/projects/list.rs` & `sentry_cli-2.19.1/src/commands/projects/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/projects/mod.rs` & `sentry_cli-2.19.1/src/commands/projects/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/react_native/appcenter.rs` & `sentry_cli-2.19.1/src/commands/react_native/appcenter.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/react_native/gradle.rs` & `sentry_cli-2.19.1/src/commands/react_native/gradle.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/react_native/mod.rs` & `sentry_cli-2.19.1/src/commands/react_native/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/react_native/xcode.rs` & `sentry_cli-2.19.1/src/commands/react_native/xcode.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/releases/archive.rs` & `sentry_cli-2.19.1/src/commands/releases/archive.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/releases/delete.rs` & `sentry_cli-2.19.1/src/commands/releases/delete.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/releases/finalize.rs` & `sentry_cli-2.19.1/src/commands/releases/finalize.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/releases/info.rs` & `sentry_cli-2.19.1/src/commands/releases/info.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/releases/list.rs` & `sentry_cli-2.19.1/src/commands/releases/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/releases/mod.rs` & `sentry_cli-2.19.1/src/commands/releases/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/releases/new.rs` & `sentry_cli-2.19.1/src/commands/releases/new.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/releases/restore.rs` & `sentry_cli-2.19.1/src/commands/releases/restore.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/releases/set_commits.rs` & `sentry_cli-2.19.1/src/commands/releases/set_commits.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/repos/list.rs` & `sentry_cli-2.19.1/src/commands/repos/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/repos/mod.rs` & `sentry_cli-2.19.1/src/commands/repos/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/send_envelope.rs` & `sentry_cli-2.19.1/src/commands/send_envelope.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/send_event.rs` & `sentry_cli-2.19.1/src/commands/send_event.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/sourcemaps/explain.rs` & `sentry_cli-2.19.1/src/commands/sourcemaps/explain.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/sourcemaps/inject.rs` & `sentry_cli-2.19.1/src/commands/sourcemaps/inject.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/sourcemaps/mod.rs` & `sentry_cli-2.19.1/src/commands/sourcemaps/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/sourcemaps/resolve.rs` & `sentry_cli-2.19.1/src/commands/sourcemaps/resolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/sourcemaps/upload.rs` & `sentry_cli-2.19.1/src/commands/sourcemaps/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/uninstall.rs` & `sentry_cli-2.19.1/src/commands/uninstall.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/update.rs` & `sentry_cli-2.19.1/src/commands/update.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/commands/upload_proguard.rs` & `sentry_cli-2.19.1/src/commands/upload_proguard.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/config.rs` & `sentry_cli-2.19.1/src/config.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/constants.rs` & `sentry_cli-2.19.1/src/constants.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/android.rs` & `sentry_cli-2.19.1/src/utils/android.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/appcenter.rs` & `sentry_cli-2.19.1/src/utils/appcenter.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/args.rs` & `sentry_cli-2.19.1/src/utils/args.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/chunks.rs` & `sentry_cli-2.19.1/src/utils/chunks.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/codepush.rs` & `sentry_cli-2.19.1/src/utils/codepush.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/cordova.rs` & `sentry_cli-2.19.1/src/utils/cordova.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/dif.rs` & `sentry_cli-2.19.1/src/utils/dif.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/dif_upload.rs` & `sentry_cli-2.19.1/src/utils/dif_upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/enc.rs` & `sentry_cli-2.19.1/src/utils/enc.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/event.rs` & `sentry_cli-2.19.1/src/utils/event.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/file_search.rs` & `sentry_cli-2.19.1/src/utils/file_search.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/file_upload.rs` & `sentry_cli-2.19.1/src/utils/file_upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/formatting.rs` & `sentry_cli-2.19.1/src/utils/formatting.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/fs.rs` & `sentry_cli-2.19.1/src/utils/fs.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/http.rs` & `sentry_cli-2.19.1/src/utils/http.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/logging.rs` & `sentry_cli-2.19.1/src/utils/logging.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/progress.rs` & `sentry_cli-2.19.1/src/utils/progress.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/releases.rs` & `sentry_cli-2.19.1/src/utils/releases.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/retry.rs` & `sentry_cli-2.19.1/src/utils/retry.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap` & `sentry_cli-2.19.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap` & `sentry_cli-2.19.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap` & `sentry_cli-2.19.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap` & `sentry_cli-2.19.1/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/sourcemaps/inject.rs` & `sentry_cli-2.19.1/src/utils/sourcemaps/inject.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 use anyhow::{bail, Result};
 use lazy_static::lazy_static;
 use log::debug;
 use sentry::types::DebugId;
 use serde_json::Value;
 
-const CODE_SNIPPET_TEMPLATE: &str = r#"!function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="__SENTRY_DEBUG_ID__")}catch(e){}}()"#;
+const CODE_SNIPPET_TEMPLATE: &str = r#"!function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="__SENTRY_DEBUG_ID__")}catch(e){}}();"#;
 const DEBUGID_PLACEHOLDER: &str = "__SENTRY_DEBUG_ID__";
 const SOURCEMAP_DEBUGID_KEY: &str = "debug_id";
 const DEBUGID_COMMENT_PREFIX: &str = "//# debugId";
 
 lazy_static! {
     static ref USE_PRAGMA_RE: Regex = Regex::new(r#""use \w+";|'use \w+';"#).unwrap();
 }
@@ -143,15 +143,15 @@
 /// // block
 ///
 /// // another
 /// // comment
 /// // block
 ///
 /// 'use strict';
-/// !function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="00000000-0000-0000-0000-000000000000")}catch(e){}}()
+/// !function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="00000000-0000-0000-0000-000000000000")}catch(e){}}();
 /// function t(t) {
 ///   return '[object Object]' === Object.prototype.toString.call(t);
 /// }
 /// //# debugId=00000000-0000-0000-0000-000000000000
 /// //# sourceMappingURL=/path/to/sourcemap
 /// "#
 /// );
@@ -429,15 +429,15 @@
         let debug_id = DebugId::default();
 
         let mut source = Vec::from(source);
 
         fixup_js_file(&mut source, debug_id).unwrap();
 
         let expected = r#"//# sourceMappingURL=fake1
-!function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="00000000-0000-0000-0000-000000000000")}catch(e){}}()
+!function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="00000000-0000-0000-0000-000000000000")}catch(e){}}();
 some line
 //# sourceMappingURL=fake2
 something else
 //# debugId=00000000-0000-0000-0000-000000000000
 //# sourceMappingURL=real
 "#;
 
@@ -482,15 +482,15 @@
             file.write_all(&source).unwrap();
         }
 
         let result = std::fs::read_to_string(temp_file.path()).unwrap();
         let expected = r#"//# sourceMappingURL=fake
 
 
-!function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="00000000-0000-0000-0000-000000000000")}catch(e){}}()
+!function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="00000000-0000-0000-0000-000000000000")}catch(e){}}();
 some line
 //# sourceMappingURL=fake
 //# sourceMappingURL=fake
 //# sourceMappingURL=fake
 //# sourceMappingURL=fake
 //# sourceMappingURL=fake
 //# sourceMappingURL=fake
@@ -531,15 +531,15 @@
 
         let expected = r#"#!/bin/node
 //# sourceMappingURL=fake1
 
   // some other comment
  "use strict"; rest of the line
 'use strict';
-!function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="00000000-0000-0000-0000-000000000000")}catch(e){}}()
+!function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="00000000-0000-0000-0000-000000000000")}catch(e){}}();
 some line
 //# sourceMappingURL=fake2
 something else
 //# debugId=00000000-0000-0000-0000-000000000000
 //# sourceMappingURL=real
 "#;
```

### Comparing `sentry_cli-2.19.0/src/utils/sourcemaps.rs` & `sentry_cli-2.19.1/src/utils/sourcemaps.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/system.rs` & `sentry_cli-2.19.1/src/utils/system.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/ui.rs` & `sentry_cli-2.19.1/src/utils/ui.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/update.rs` & `sentry_cli-2.19.1/src/utils/update.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/vcs.rs` & `sentry_cli-2.19.1/src/utils/vcs.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.0/src/utils/xcode.rs` & `sentry_cli-2.19.1/src/utils/xcode.rs`

 * *Files identical despite different names*

