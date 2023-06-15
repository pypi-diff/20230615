# Comparing `tmp/skytemple-rust-1.5.3.tar.gz` & `tmp/skytemple-rust-1.6.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skytemple-rust-1.5.3.tar", last modified: Thu Jun 15 18:17:28 2023, max compression
+gzip compressed data, was "skytemple-rust-1.6.0a1.tar", last modified: Fri Jun  9 19:23:10 2023, max compression
```

## Comparing `skytemple-rust-1.5.3.tar` & `skytemple-rust-1.6.0a1.tar`

### file list

```diff
@@ -1,148 +1,150 @@
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-06-15 18:17:28.499784 skytemple-rust-1.5.3/
--rw-r--r--   0 marco     (1000) marco     (1000)    26715 2023-06-15 18:17:02.000000 skytemple-rust-1.5.3/Cargo.lock
--rw-r--r--   0 marco     (1000) marco     (1000)     1941 2023-06-15 18:17:00.000000 skytemple-rust-1.5.3/Cargo.toml
--rw-rw-rw-   0 marco     (1000) marco     (1000)    35148 2022-02-28 21:59:54.000000 skytemple-rust-1.5.3/LICENSE
--rw-r--r--   0 marco     (1000) marco     (1000)      160 2022-09-26 16:26:15.000000 skytemple-rust-1.5.3/MANIFEST.in
--rw-r--r--   0 marco     (1000) marco     (1000)     3392 2023-06-15 18:17:28.499784 skytemple-rust-1.5.3/PKG-INFO
--rw-r--r--   0 marco     (1000) marco     (1000)     2755 2023-06-15 03:42:25.000000 skytemple-rust-1.5.3/README.rst
--rw-rw-rw-   0 marco     (1000) marco     (1000)       69 2022-02-23 21:38:11.000000 skytemple-rust-1.5.3/pyproject.toml
--rw-r--r--   0 marco     (1000) marco     (1000)       38 2023-06-15 18:17:28.499784 skytemple-rust-1.5.3/setup.cfg
--rw-r--r--   0 marco     (1000) marco     (1000)     1504 2023-06-15 18:16:53.000000 skytemple-rust-1.5.3/setup.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-06-15 18:17:28.493117 skytemple-rust-1.5.3/skytemple_rust/
--rw-r--r--   0 marco     (1000) marco     (1000)      341 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/skytemple_rust/__init__.pyi
--rw-r--r--   0 marco     (1000) marco     (1000)     2512 2023-04-29 13:51:47.000000 skytemple-rust-1.5.3/skytemple_rust/pmd_wan.pyi
--rw-rw-rw-   0 marco     (1000) marco     (1000)        0 2020-05-30 09:51:40.000000 skytemple-rust-1.5.3/skytemple_rust/py.typed
--rw-rw-rw-   0 marco     (1000) marco     (1000)     1009 2022-02-28 21:59:54.000000 skytemple-rust-1.5.3/skytemple_rust/st_at3px.pyi
--rw-rw-rw-   0 marco     (1000) marco     (1000)     1020 2022-02-28 21:59:54.000000 skytemple-rust-1.5.3/skytemple_rust/st_at4pn.pyi
--rw-rw-rw-   0 marco     (1000) marco     (1000)     1009 2022-02-28 21:59:54.000000 skytemple-rust-1.5.3/skytemple_rust/st_at4px.pyi
--rw-rw-rw-   0 marco     (1000) marco     (1000)     1009 2022-02-28 21:59:54.000000 skytemple-rust-1.5.3/skytemple_rust/st_atupx.pyi
--rw-r--r--   0 marco     (1000) marco     (1000)     2302 2023-05-15 08:10:27.000000 skytemple-rust-1.5.3/skytemple_rust/st_bg_list_dat.pyi
--rw-rw-rw-   0 marco     (1000) marco     (1000)     1243 2022-02-28 21:59:54.000000 skytemple-rust-1.5.3/skytemple_rust/st_bgp.pyi
--rw-r--r--   0 marco     (1000) marco     (1000)     2743 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/skytemple_rust/st_bma.pyi
--rw-r--r--   0 marco     (1000) marco     (1000)     1748 2023-06-15 02:55:44.000000 skytemple-rust-1.5.3/skytemple_rust/st_bpa.pyi
--rw-r--r--   0 marco     (1000) marco     (1000)     3618 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/skytemple_rust/st_bpc.pyi
--rw-r--r--   0 marco     (1000) marco     (1000)     1651 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/skytemple_rust/st_bpl.pyi
--rw-rw-rw-   0 marco     (1000) marco     (1000)     1330 2022-02-28 21:59:54.000000 skytemple-rust-1.5.3/skytemple_rust/st_dbg.pyi
--rw-rw-rw-   0 marco     (1000) marco     (1000)     1642 2022-02-28 21:59:54.000000 skytemple-rust-1.5.3/skytemple_rust/st_dma.pyi
--rw-rw-rw-   0 marco     (1000) marco     (1000)     1591 2022-02-28 21:59:54.000000 skytemple-rust-1.5.3/skytemple_rust/st_dpc.pyi
--rw-rw-rw-   0 marco     (1000) marco     (1000)     1224 2022-02-28 21:59:54.000000 skytemple-rust-1.5.3/skytemple_rust/st_dpci.pyi
--rw-rw-rw-   0 marco     (1000) marco     (1000)      950 2022-02-28 21:59:54.000000 skytemple-rust-1.5.3/skytemple_rust/st_dpl.pyi
--rw-r--r--   0 marco     (1000) marco     (1000)     1614 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/skytemple_rust/st_dpla.pyi
--rw-r--r--   0 marco     (1000) marco     (1000)     1445 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/skytemple_rust/st_item_p.pyi
--rw-r--r--   0 marco     (1000) marco     (1000)     1748 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/skytemple_rust/st_kao.pyi
--rw-r--r--   0 marco     (1000) marco     (1000)     6079 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/skytemple_rust/st_mappa_bin.pyi
--rw-r--r--   0 marco     (1000) marco     (1000)     2957 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/skytemple_rust/st_md.pyi
--rw-rw-rw-   0 marco     (1000) marco     (1000)     1009 2022-02-28 21:59:54.000000 skytemple-rust-1.5.3/skytemple_rust/st_pkdpx.pyi
--rw-r--r--   0 marco     (1000) marco     (1000)      864 2023-05-15 08:28:33.000000 skytemple-rust-1.5.3/skytemple_rust/st_sir0.pyi
--rw-rw-rw-   0 marco     (1000) marco     (1000)     1988 2022-02-28 21:59:54.000000 skytemple-rust-1.5.3/skytemple_rust/st_smdl.pyi
--rw-rw-rw-   0 marco     (1000) marco     (1000)     3566 2022-02-28 21:59:54.000000 skytemple-rust-1.5.3/skytemple_rust/st_ssb.pyi
--rw-rw-rw-   0 marco     (1000) marco     (1000)      910 2022-02-28 21:59:54.000000 skytemple-rust-1.5.3/skytemple_rust/st_string.pyi
--rw-rw-rw-   0 marco     (1000) marco     (1000)     3580 2022-02-28 21:59:54.000000 skytemple-rust-1.5.3/skytemple_rust/st_swdl.pyi
--rw-r--r--   0 marco     (1000) marco     (1000)     2623 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/skytemple_rust/st_waza_p.pyi
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-06-15 18:17:28.493117 skytemple-rust-1.5.3/skytemple_rust.egg-info/
--rw-rw-rw-   0 marco     (1000) marco     (1000)     3392 2023-06-15 18:17:28.000000 skytemple-rust-1.5.3/skytemple_rust.egg-info/PKG-INFO
--rw-rw-rw-   0 marco     (1000) marco     (1000)     3007 2023-06-15 18:17:28.000000 skytemple-rust-1.5.3/skytemple_rust.egg-info/SOURCES.txt
--rw-rw-rw-   0 marco     (1000) marco     (1000)        1 2023-06-15 18:17:28.000000 skytemple-rust-1.5.3/skytemple_rust.egg-info/dependency_links.txt
--rw-rw-rw-   0 marco     (1000) marco     (1000)        1 2022-06-04 19:10:29.000000 skytemple-rust-1.5.3/skytemple_rust.egg-info/not-zip-safe
--rw-rw-rw-   0 marco     (1000) marco     (1000)       61 2023-06-15 18:17:28.000000 skytemple-rust-1.5.3/skytemple_rust.egg-info/requires.txt
--rw-rw-rw-   0 marco     (1000) marco     (1000)       15 2023-06-15 18:17:28.000000 skytemple-rust-1.5.3/skytemple_rust.egg-info/top_level.txt
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-06-15 18:17:28.493117 skytemple-rust-1.5.3/skytemple_rust_macros/
--rw-rw-rw-   0 marco     (1000) marco     (1000)      165 2022-02-28 21:59:54.000000 skytemple-rust-1.5.3/skytemple_rust_macros/Cargo.lock
--rw-rw-rw-   0 marco     (1000) marco     (1000)      325 2022-02-28 21:59:54.000000 skytemple-rust-1.5.3/skytemple_rust_macros/Cargo.toml
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-06-15 18:17:28.493117 skytemple-rust-1.5.3/skytemple_rust_macros/src/
--rw-r--r--   0 marco     (1000) marco     (1000)     3246 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/skytemple_rust_macros/src/lib.rs
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-06-15 18:17:28.493117 skytemple-rust-1.5.3/skytemple_rust_macros_no_py/
--rw-r--r--   0 marco     (1000) marco     (1000)      165 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/skytemple_rust_macros_no_py/Cargo.lock
--rw-r--r--   0 marco     (1000) marco     (1000)      331 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/skytemple_rust_macros_no_py/Cargo.toml
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-06-15 18:17:28.493117 skytemple-rust-1.5.3/skytemple_rust_macros_no_py/src/
--rw-r--r--   0 marco     (1000) marco     (1000)     2594 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/skytemple_rust_macros_no_py/src/lib.rs
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-06-15 18:17:28.496451 skytemple-rust-1.5.3/src/
--rw-r--r--   0 marco     (1000) marco     (1000)     6027 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/bytes.rs
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-06-15 18:17:28.496451 skytemple-rust-1.5.3/src/compression/
--rw-r--r--   0 marco     (1000) marco     (1000)     6134 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/compression/bma_collision_rle.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     9179 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/compression/bma_layer_nrl.rs
--rw-r--r--   0 marco     (1000) marco     (1000)    20833 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/compression/bpc_image.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     9038 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/compression/bpc_tilemap.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     6157 2023-06-15 02:55:18.000000 skytemple-rust-1.5.3/src/compression/custom_999.rs
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-06-15 18:17:28.499784 skytemple-rust-1.5.3/src/compression/generic/
--rw-r--r--   0 marco     (1000) marco     (1000)      762 2023-02-26 17:42:40.000000 skytemple-rust-1.5.3/src/compression/generic/mod.rs
--rw-r--r--   0 marco     (1000) marco     (1000)    11332 2023-02-26 17:42:40.000000 skytemple-rust-1.5.3/src/compression/generic/nrl.rs
--rw-r--r--   0 marco     (1000) marco     (1000)      888 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/compression/mod.rs
--rw-r--r--   0 marco     (1000) marco     (1000)    27022 2023-06-15 02:55:18.000000 skytemple-rust-1.5.3/src/compression/px.rs
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-06-15 18:17:28.499784 skytemple-rust-1.5.3/src/dse/
--rw-r--r--   0 marco     (1000) marco     (1000)     2475 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/dse/date.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     2389 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/dse/filename.rs
--rw-r--r--   0 marco     (1000) marco     (1000)      816 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/dse/mod.rs
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-06-15 18:17:28.499784 skytemple-rust-1.5.3/src/dse/st_smdl/
--rw-r--r--   0 marco     (1000) marco     (1000)     1837 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/dse/st_smdl/eoc.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     6908 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/dse/st_smdl/event.rs
--rw-r--r--   0 marco     (1000) marco     (1000)      869 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/dse/st_smdl/mod.rs
--rw-r--r--   0 marco     (1000) marco     (1000)    13186 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/dse/st_smdl/python.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     9306 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/dse/st_smdl/smdl.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     4266 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/dse/st_smdl/song.rs
--rw-r--r--   0 marco     (1000) marco     (1000)    11467 2023-06-15 02:55:18.000000 skytemple-rust-1.5.3/src/dse/st_smdl/trk.rs
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-06-15 18:17:28.499784 skytemple-rust-1.5.3/src/dse/st_swdl/
--rw-r--r--   0 marco     (1000) marco     (1000)     3739 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/dse/st_swdl/kgrp.rs
--rw-r--r--   0 marco     (1000) marco     (1000)      870 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/dse/st_swdl/mod.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     2639 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/dse/st_swdl/pcmd.rs
--rw-r--r--   0 marco     (1000) marco     (1000)    13039 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/dse/st_swdl/prgi.rs
--rw-r--r--   0 marco     (1000) marco     (1000)    23293 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/dse/st_swdl/python.rs
--rw-r--r--   0 marco     (1000) marco     (1000)    10638 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/dse/st_swdl/swdl.rs
--rw-r--r--   0 marco     (1000) marco     (1000)    10198 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/dse/st_swdl/wavi.rs
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-06-15 18:17:28.499784 skytemple-rust-1.5.3/src/encoding/
--rw-r--r--   0 marco     (1000) marco     (1000)     4122 2023-06-15 02:55:18.000000 skytemple-rust-1.5.3/src/encoding/mod.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     9176 2023-06-15 02:55:18.000000 skytemple-rust-1.5.3/src/encoding/pmd2_encoder.rs
--rw-r--r--   0 marco     (1000) marco     (1000)    12651 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/encoding_utils.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     1386 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/err.rs
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-06-15 18:17:28.499784 skytemple-rust-1.5.3/src/gettext/
--rw-rw-rw-   0 marco     (1000) marco     (1000)      961 2022-02-28 21:59:54.000000 skytemple-rust-1.5.3/src/gettext/macro_stub.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     1071 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/gettext/mod.rs
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-06-15 18:17:28.499784 skytemple-rust-1.5.3/src/image/
--rw-r--r--   0 marco     (1000) marco     (1000)     7613 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/image/mod.rs
--rw-r--r--   0 marco     (1000) marco     (1000)    15455 2023-06-15 18:16:38.000000 skytemple-rust-1.5.3/src/image/tiled.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     6580 2023-06-15 02:55:18.000000 skytemple-rust-1.5.3/src/image/tilemap_entry.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     2995 2023-06-15 03:42:25.000000 skytemple-rust-1.5.3/src/lib.rs
--rw-r--r--   0 marco     (1000) marco     (1000)    13777 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/macros.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     4047 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/no_python.rs
--rw-r--r--   0 marco     (1000) marco     (1000)    14050 2023-04-29 13:51:47.000000 skytemple-rust-1.5.3/src/pmd_wan.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     2265 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/python.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     6830 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/python_image.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     7690 2023-06-15 03:42:25.000000 skytemple-rust-1.5.3/src/python_module.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     1743 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/rom_source.rs
--rw-r--r--   0 marco     (1000) marco     (1000)    20876 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/romfs.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     3354 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/st_at3px.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     3001 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/st_at4pn.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     3579 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/st_at4px.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     5788 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/st_at_common.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     3157 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/st_atupx.rs
--rw-r--r--   0 marco     (1000) marco     (1000)    11592 2023-06-15 02:56:57.000000 skytemple-rust-1.5.3/src/st_bg_list_dat.rs
--rw-r--r--   0 marco     (1000) marco     (1000)    10196 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/st_bgp.rs
--rw-r--r--   0 marco     (1000) marco     (1000)    38572 2023-06-15 02:55:18.000000 skytemple-rust-1.5.3/src/st_bma.rs
--rw-r--r--   0 marco     (1000) marco     (1000)    17397 2023-06-15 02:55:44.000000 skytemple-rust-1.5.3/src/st_bpa.rs
--rw-r--r--   0 marco     (1000) marco     (1000)    47977 2023-06-15 02:55:18.000000 skytemple-rust-1.5.3/src/st_bpc.rs
--rw-r--r--   0 marco     (1000) marco     (1000)    16650 2023-06-15 02:55:18.000000 skytemple-rust-1.5.3/src/st_bpl.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     3149 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/st_dbg.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     7096 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/st_dma.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     5434 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/st_dpc.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     2983 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/st_dpci.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     3001 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/st_dpl.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     1274 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/st_dpla.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     6457 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/st_item_p.rs
--rw-r--r--   0 marco     (1000) marco     (1000)    17968 2023-06-15 02:55:18.000000 skytemple-rust-1.5.3/src/st_kao.rs
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-06-15 18:17:28.499784 skytemple-rust-1.5.3/src/st_mappa_bin/
--rw-r--r--   0 marco     (1000) marco     (1000)     3631 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/st_mappa_bin/enums_consts.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     6661 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/st_mappa_bin/floor.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     6219 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/st_mappa_bin/item_list.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     9890 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/st_mappa_bin/layout.rs
--rw-r--r--   0 marco     (1000) marco     (1000)    12732 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/st_mappa_bin/mappa.rs
--rw-r--r--   0 marco     (1000) marco     (1000)    12064 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/st_mappa_bin/minimize.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     1302 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/st_mappa_bin/mod.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     3625 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/st_mappa_bin/monster_list.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     1643 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/st_mappa_bin/pymodule.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     5344 2022-09-26 20:47:03.000000 skytemple-rust-1.5.3/src/st_mappa_bin/trap_list.rs
--rw-r--r--   0 marco     (1000) marco     (1000)    31195 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/st_md.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     3579 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/st_pkdpx.rs
--rw-r--r--   0 marco     (1000) marco     (1000)    13015 2023-06-15 02:55:18.000000 skytemple-rust-1.5.3/src/st_sir0.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     2134 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/st_string.rs
--rw-r--r--   0 marco     (1000) marco     (1000)    22916 2022-09-19 08:21:32.000000 skytemple-rust-1.5.3/src/st_waza_p.rs
--rw-r--r--   0 marco     (1000) marco     (1000)     4941 2023-06-15 02:55:18.000000 skytemple-rust-1.5.3/src/util.rs
+drwxr-xr-x   0 marco     (1000) users      (100)        0 2023-06-09 19:23:10.186249 skytemple-rust-1.6.0a1/
+-rw-r--r--   0 marco     (1000) users      (100)    26715 2023-05-29 12:38:21.000000 skytemple-rust-1.6.0a1/Cargo.lock
+-rw-r--r--   0 marco     (1000) users      (100)     1998 2023-06-09 10:23:47.000000 skytemple-rust-1.6.0a1/Cargo.toml
+-rw-rw-rw-   0 marco     (1000) users      (100)    35148 2022-02-28 21:59:54.000000 skytemple-rust-1.6.0a1/LICENSE
+-rw-r--r--   0 marco     (1000) users      (100)      160 2022-09-26 16:26:15.000000 skytemple-rust-1.6.0a1/MANIFEST.in
+-rw-r--r--   0 marco     (1000) users      (100)     3395 2023-06-09 19:23:10.186249 skytemple-rust-1.6.0a1/PKG-INFO
+-rw-rw-rw-   0 marco     (1000) users      (100)     2756 2023-05-27 21:44:12.000000 skytemple-rust-1.6.0a1/README.rst
+-rw-rw-rw-   0 marco     (1000) users      (100)       69 2022-02-23 21:38:11.000000 skytemple-rust-1.6.0a1/pyproject.toml
+-rw-r--r--   0 marco     (1000) users      (100)       38 2023-06-09 19:23:10.186249 skytemple-rust-1.6.0a1/setup.cfg
+-rw-r--r--   0 marco     (1000) users      (100)     1506 2023-06-09 10:23:52.000000 skytemple-rust-1.6.0a1/setup.py
+drwxr-xr-x   0 marco     (1000) users      (100)        0 2023-06-09 19:23:10.169583 skytemple-rust-1.6.0a1/skytemple_rust/
+-rw-r--r--   0 marco     (1000) users      (100)      341 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/skytemple_rust/__init__.pyi
+-rw-r--r--   0 marco     (1000) users      (100)     2512 2023-04-29 13:51:47.000000 skytemple-rust-1.6.0a1/skytemple_rust/pmd_wan.pyi
+-rw-rw-rw-   0 marco     (1000) users      (100)        0 2020-05-30 09:51:40.000000 skytemple-rust-1.6.0a1/skytemple_rust/py.typed
+-rw-rw-rw-   0 marco     (1000) users      (100)     1009 2022-02-28 21:59:54.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_at3px.pyi
+-rw-rw-rw-   0 marco     (1000) users      (100)     1020 2022-02-28 21:59:54.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_at4pn.pyi
+-rw-rw-rw-   0 marco     (1000) users      (100)     1009 2022-02-28 21:59:54.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_at4px.pyi
+-rw-rw-rw-   0 marco     (1000) users      (100)     1009 2022-02-28 21:59:54.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_atupx.pyi
+-rw-r--r--   0 marco     (1000) users      (100)     2302 2023-05-15 08:10:27.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_bg_list_dat.pyi
+-rw-rw-rw-   0 marco     (1000) users      (100)     1243 2022-02-28 21:59:54.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_bgp.pyi
+-rw-r--r--   0 marco     (1000) users      (100)     2743 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_bma.pyi
+-rw-r--r--   0 marco     (1000) users      (100)     1728 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_bpa.pyi
+-rw-r--r--   0 marco     (1000) users      (100)     3618 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_bpc.pyi
+-rw-r--r--   0 marco     (1000) users      (100)     1651 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_bpl.pyi
+-rw-rw-rw-   0 marco     (1000) users      (100)     1330 2022-02-28 21:59:54.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_dbg.pyi
+-rw-rw-rw-   0 marco     (1000) users      (100)     1642 2022-02-28 21:59:54.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_dma.pyi
+-rw-rw-rw-   0 marco     (1000) users      (100)     1591 2022-02-28 21:59:54.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_dpc.pyi
+-rw-rw-rw-   0 marco     (1000) users      (100)     1224 2022-02-28 21:59:54.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_dpci.pyi
+-rw-rw-rw-   0 marco     (1000) users      (100)      950 2022-02-28 21:59:54.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_dpl.pyi
+-rw-r--r--   0 marco     (1000) users      (100)     1614 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_dpla.pyi
+-rw-r--r--   0 marco     (1000) users      (100)     1445 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_item_p.pyi
+-rw-r--r--   0 marco     (1000) users      (100)     1748 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_kao.pyi
+-rw-r--r--   0 marco     (1000) users      (100)     6079 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_mappa_bin.pyi
+-rw-r--r--   0 marco     (1000) users      (100)     2957 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_md.pyi
+-rw-rw-rw-   0 marco     (1000) users      (100)     1009 2022-02-28 21:59:54.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_pkdpx.pyi
+-rw-r--r--   0 marco     (1000) users      (100)     1279 2023-06-09 10:27:01.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_script_var_table.pyi
+-rw-r--r--   0 marco     (1000) users      (100)      864 2023-05-15 08:28:33.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_sir0.pyi
+-rw-rw-rw-   0 marco     (1000) users      (100)     1988 2022-02-28 21:59:54.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_smdl.pyi
+-rw-rw-rw-   0 marco     (1000) users      (100)     3566 2022-02-28 21:59:54.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_ssb.pyi
+-rw-rw-rw-   0 marco     (1000) users      (100)      910 2022-02-28 21:59:54.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_string.pyi
+-rw-rw-rw-   0 marco     (1000) users      (100)     3580 2022-02-28 21:59:54.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_swdl.pyi
+-rw-r--r--   0 marco     (1000) users      (100)     2623 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/skytemple_rust/st_waza_p.pyi
+drwxr-xr-x   0 marco     (1000) users      (100)        0 2023-06-09 19:23:10.169583 skytemple-rust-1.6.0a1/skytemple_rust.egg-info/
+-rw-rw-rw-   0 marco     (1000) users      (100)     3395 2023-06-09 19:23:10.000000 skytemple-rust-1.6.0a1/skytemple_rust.egg-info/PKG-INFO
+-rw-rw-rw-   0 marco     (1000) users      (100)     3073 2023-06-09 19:23:10.000000 skytemple-rust-1.6.0a1/skytemple_rust.egg-info/SOURCES.txt
+-rw-rw-rw-   0 marco     (1000) users      (100)        1 2023-06-09 19:23:10.000000 skytemple-rust-1.6.0a1/skytemple_rust.egg-info/dependency_links.txt
+-rw-rw-rw-   0 marco     (1000) users      (100)        1 2022-06-04 19:10:29.000000 skytemple-rust-1.6.0a1/skytemple_rust.egg-info/not-zip-safe
+-rw-rw-rw-   0 marco     (1000) users      (100)       61 2023-06-09 19:23:10.000000 skytemple-rust-1.6.0a1/skytemple_rust.egg-info/requires.txt
+-rw-rw-rw-   0 marco     (1000) users      (100)       15 2023-06-09 19:23:10.000000 skytemple-rust-1.6.0a1/skytemple_rust.egg-info/top_level.txt
+drwxr-xr-x   0 marco     (1000) users      (100)        0 2023-06-09 19:23:10.169583 skytemple-rust-1.6.0a1/skytemple_rust_macros/
+-rw-rw-rw-   0 marco     (1000) users      (100)      165 2022-02-28 21:59:54.000000 skytemple-rust-1.6.0a1/skytemple_rust_macros/Cargo.lock
+-rw-rw-rw-   0 marco     (1000) users      (100)      325 2022-02-28 21:59:54.000000 skytemple-rust-1.6.0a1/skytemple_rust_macros/Cargo.toml
+drwxr-xr-x   0 marco     (1000) users      (100)        0 2023-06-09 19:23:10.169583 skytemple-rust-1.6.0a1/skytemple_rust_macros/src/
+-rw-r--r--   0 marco     (1000) users      (100)     3246 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/skytemple_rust_macros/src/lib.rs
+drwxr-xr-x   0 marco     (1000) users      (100)        0 2023-06-09 19:23:10.169583 skytemple-rust-1.6.0a1/skytemple_rust_macros_no_py/
+-rw-r--r--   0 marco     (1000) users      (100)      165 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/skytemple_rust_macros_no_py/Cargo.lock
+-rw-r--r--   0 marco     (1000) users      (100)      331 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/skytemple_rust_macros_no_py/Cargo.toml
+drwxr-xr-x   0 marco     (1000) users      (100)        0 2023-06-09 19:23:10.169583 skytemple-rust-1.6.0a1/skytemple_rust_macros_no_py/src/
+-rw-r--r--   0 marco     (1000) users      (100)     2594 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/skytemple_rust_macros_no_py/src/lib.rs
+drwxr-xr-x   0 marco     (1000) users      (100)        0 2023-06-09 19:23:10.179583 skytemple-rust-1.6.0a1/src/
+-rw-r--r--   0 marco     (1000) users      (100)     6027 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/bytes.rs
+drwxr-xr-x   0 marco     (1000) users      (100)        0 2023-06-09 19:23:10.179583 skytemple-rust-1.6.0a1/src/compression/
+-rw-r--r--   0 marco     (1000) users      (100)     6134 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/compression/bma_collision_rle.rs
+-rw-r--r--   0 marco     (1000) users      (100)     9179 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/compression/bma_layer_nrl.rs
+-rw-r--r--   0 marco     (1000) users      (100)    20833 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/compression/bpc_image.rs
+-rw-r--r--   0 marco     (1000) users      (100)     9038 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/compression/bpc_tilemap.rs
+-rw-r--r--   0 marco     (1000) users      (100)     6157 2023-05-29 12:33:25.000000 skytemple-rust-1.6.0a1/src/compression/custom_999.rs
+drwxr-xr-x   0 marco     (1000) users      (100)        0 2023-06-09 19:23:10.179583 skytemple-rust-1.6.0a1/src/compression/generic/
+-rw-r--r--   0 marco     (1000) users      (100)      762 2023-02-26 17:42:40.000000 skytemple-rust-1.6.0a1/src/compression/generic/mod.rs
+-rw-r--r--   0 marco     (1000) users      (100)    11332 2023-02-26 17:42:40.000000 skytemple-rust-1.6.0a1/src/compression/generic/nrl.rs
+-rw-r--r--   0 marco     (1000) users      (100)      888 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/compression/mod.rs
+-rw-r--r--   0 marco     (1000) users      (100)    27022 2023-05-29 12:33:25.000000 skytemple-rust-1.6.0a1/src/compression/px.rs
+drwxr-xr-x   0 marco     (1000) users      (100)        0 2023-06-09 19:23:10.179583 skytemple-rust-1.6.0a1/src/dse/
+-rw-r--r--   0 marco     (1000) users      (100)     2475 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/dse/date.rs
+-rw-r--r--   0 marco     (1000) users      (100)     2389 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/dse/filename.rs
+-rw-r--r--   0 marco     (1000) users      (100)      816 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/dse/mod.rs
+drwxr-xr-x   0 marco     (1000) users      (100)        0 2023-06-09 19:23:10.182916 skytemple-rust-1.6.0a1/src/dse/st_smdl/
+-rw-r--r--   0 marco     (1000) users      (100)     1837 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/dse/st_smdl/eoc.rs
+-rw-r--r--   0 marco     (1000) users      (100)     6908 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/dse/st_smdl/event.rs
+-rw-r--r--   0 marco     (1000) users      (100)      869 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/dse/st_smdl/mod.rs
+-rw-r--r--   0 marco     (1000) users      (100)    13186 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/dse/st_smdl/python.rs
+-rw-r--r--   0 marco     (1000) users      (100)     9306 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/dse/st_smdl/smdl.rs
+-rw-r--r--   0 marco     (1000) users      (100)     4266 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/dse/st_smdl/song.rs
+-rw-r--r--   0 marco     (1000) users      (100)    11467 2023-05-29 12:33:25.000000 skytemple-rust-1.6.0a1/src/dse/st_smdl/trk.rs
+drwxr-xr-x   0 marco     (1000) users      (100)        0 2023-06-09 19:23:10.182916 skytemple-rust-1.6.0a1/src/dse/st_swdl/
+-rw-r--r--   0 marco     (1000) users      (100)     3739 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/dse/st_swdl/kgrp.rs
+-rw-r--r--   0 marco     (1000) users      (100)      870 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/dse/st_swdl/mod.rs
+-rw-r--r--   0 marco     (1000) users      (100)     2639 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/dse/st_swdl/pcmd.rs
+-rw-r--r--   0 marco     (1000) users      (100)    13039 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/dse/st_swdl/prgi.rs
+-rw-r--r--   0 marco     (1000) users      (100)    23293 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/dse/st_swdl/python.rs
+-rw-r--r--   0 marco     (1000) users      (100)    10638 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/dse/st_swdl/swdl.rs
+-rw-r--r--   0 marco     (1000) users      (100)    10198 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/dse/st_swdl/wavi.rs
+drwxr-xr-x   0 marco     (1000) users      (100)        0 2023-06-09 19:23:10.182916 skytemple-rust-1.6.0a1/src/encoding/
+-rw-r--r--   0 marco     (1000) users      (100)     4122 2023-06-09 13:25:26.000000 skytemple-rust-1.6.0a1/src/encoding/mod.rs
+-rw-r--r--   0 marco     (1000) users      (100)     9176 2023-05-29 12:33:25.000000 skytemple-rust-1.6.0a1/src/encoding/pmd2_encoder.rs
+-rw-r--r--   0 marco     (1000) users      (100)    12651 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/encoding_utils.rs
+-rw-r--r--   0 marco     (1000) users      (100)     1386 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/err.rs
+drwxr-xr-x   0 marco     (1000) users      (100)        0 2023-06-09 19:23:10.182916 skytemple-rust-1.6.0a1/src/gettext/
+-rw-rw-rw-   0 marco     (1000) users      (100)      961 2022-02-28 21:59:54.000000 skytemple-rust-1.6.0a1/src/gettext/macro_stub.rs
+-rw-r--r--   0 marco     (1000) users      (100)     1071 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/gettext/mod.rs
+drwxr-xr-x   0 marco     (1000) users      (100)        0 2023-06-09 19:23:10.186249 skytemple-rust-1.6.0a1/src/image/
+-rw-r--r--   0 marco     (1000) users      (100)     7613 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/image/mod.rs
+-rw-r--r--   0 marco     (1000) users      (100)    15465 2023-06-09 13:25:26.000000 skytemple-rust-1.6.0a1/src/image/tiled.rs
+-rw-r--r--   0 marco     (1000) users      (100)     6580 2023-05-29 12:33:25.000000 skytemple-rust-1.6.0a1/src/image/tilemap_entry.rs
+-rw-r--r--   0 marco     (1000) users      (100)     3061 2023-06-09 13:25:26.000000 skytemple-rust-1.6.0a1/src/lib.rs
+-rw-r--r--   0 marco     (1000) users      (100)    13777 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/macros.rs
+-rw-r--r--   0 marco     (1000) users      (100)     4047 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/no_python.rs
+-rw-r--r--   0 marco     (1000) users      (100)    14050 2023-04-29 13:51:47.000000 skytemple-rust-1.6.0a1/src/pmd_wan.rs
+-rw-r--r--   0 marco     (1000) users      (100)     2265 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/python.rs
+-rw-r--r--   0 marco     (1000) users      (100)     6830 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/python_image.rs
+-rw-r--r--   0 marco     (1000) users      (100)     7912 2023-06-09 13:25:26.000000 skytemple-rust-1.6.0a1/src/python_module.rs
+-rw-r--r--   0 marco     (1000) users      (100)     1743 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/rom_source.rs
+-rw-r--r--   0 marco     (1000) users      (100)    20876 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/romfs.rs
+-rw-r--r--   0 marco     (1000) users      (100)     3354 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/st_at3px.rs
+-rw-r--r--   0 marco     (1000) users      (100)     3001 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/st_at4pn.rs
+-rw-r--r--   0 marco     (1000) users      (100)     3579 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/st_at4px.rs
+-rw-r--r--   0 marco     (1000) users      (100)     5788 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/st_at_common.rs
+-rw-r--r--   0 marco     (1000) users      (100)     3157 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/st_atupx.rs
+-rw-r--r--   0 marco     (1000) users      (100)    12384 2023-06-09 13:25:26.000000 skytemple-rust-1.6.0a1/src/st_bg_list_dat.rs
+-rw-r--r--   0 marco     (1000) users      (100)    10196 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/st_bgp.rs
+-rw-r--r--   0 marco     (1000) users      (100)    38572 2023-05-29 12:33:25.000000 skytemple-rust-1.6.0a1/src/st_bma.rs
+-rw-r--r--   0 marco     (1000) users      (100)    17177 2023-06-09 13:25:26.000000 skytemple-rust-1.6.0a1/src/st_bpa.rs
+-rw-r--r--   0 marco     (1000) users      (100)    47977 2023-05-29 12:33:25.000000 skytemple-rust-1.6.0a1/src/st_bpc.rs
+-rw-r--r--   0 marco     (1000) users      (100)    16650 2023-05-29 12:33:25.000000 skytemple-rust-1.6.0a1/src/st_bpl.rs
+-rw-r--r--   0 marco     (1000) users      (100)     3149 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/st_dbg.rs
+-rw-r--r--   0 marco     (1000) users      (100)     7096 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/st_dma.rs
+-rw-r--r--   0 marco     (1000) users      (100)     5434 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/st_dpc.rs
+-rw-r--r--   0 marco     (1000) users      (100)     2983 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/st_dpci.rs
+-rw-r--r--   0 marco     (1000) users      (100)     3001 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/st_dpl.rs
+-rw-r--r--   0 marco     (1000) users      (100)     1274 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/st_dpla.rs
+-rw-r--r--   0 marco     (1000) users      (100)     6457 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/st_item_p.rs
+-rw-r--r--   0 marco     (1000) users      (100)    17968 2023-05-29 12:33:25.000000 skytemple-rust-1.6.0a1/src/st_kao.rs
+drwxr-xr-x   0 marco     (1000) users      (100)        0 2023-06-09 19:23:10.186249 skytemple-rust-1.6.0a1/src/st_mappa_bin/
+-rw-r--r--   0 marco     (1000) users      (100)     3631 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/st_mappa_bin/enums_consts.rs
+-rw-r--r--   0 marco     (1000) users      (100)     6661 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/st_mappa_bin/floor.rs
+-rw-r--r--   0 marco     (1000) users      (100)     6219 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/st_mappa_bin/item_list.rs
+-rw-r--r--   0 marco     (1000) users      (100)     9890 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/st_mappa_bin/layout.rs
+-rw-r--r--   0 marco     (1000) users      (100)    12732 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/st_mappa_bin/mappa.rs
+-rw-r--r--   0 marco     (1000) users      (100)    12064 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/st_mappa_bin/minimize.rs
+-rw-r--r--   0 marco     (1000) users      (100)     1302 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/st_mappa_bin/mod.rs
+-rw-r--r--   0 marco     (1000) users      (100)     3625 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/st_mappa_bin/monster_list.rs
+-rw-r--r--   0 marco     (1000) users      (100)     1643 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/st_mappa_bin/pymodule.rs
+-rw-r--r--   0 marco     (1000) users      (100)     5344 2022-09-26 20:47:03.000000 skytemple-rust-1.6.0a1/src/st_mappa_bin/trap_list.rs
+-rw-r--r--   0 marco     (1000) users      (100)    31195 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/st_md.rs
+-rw-r--r--   0 marco     (1000) users      (100)     3579 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/st_pkdpx.rs
+-rw-r--r--   0 marco     (1000) users      (100)     6567 2023-06-09 13:25:26.000000 skytemple-rust-1.6.0a1/src/st_script_var_table.rs
+-rw-r--r--   0 marco     (1000) users      (100)    13015 2023-05-29 12:33:25.000000 skytemple-rust-1.6.0a1/src/st_sir0.rs
+-rw-r--r--   0 marco     (1000) users      (100)     2134 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/st_string.rs
+-rw-r--r--   0 marco     (1000) users      (100)    22916 2022-09-19 08:21:32.000000 skytemple-rust-1.6.0a1/src/st_waza_p.rs
+-rw-r--r--   0 marco     (1000) users      (100)     4941 2023-05-29 12:33:25.000000 skytemple-rust-1.6.0a1/src/util.rs
```

### Comparing `skytemple-rust-1.5.3/Cargo.lock` & `skytemple-rust-1.6.0a1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "addr2line"
-version = "0.17.0"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b9ecd88a8c8378ca913a680cd98f0f13ac67383d35993f86c90a70e3f137816b"
+checksum = "a76fd60b23679b7d19bd066031410fb7e458ccc5e958eb5c325888ce4baedc97"
 dependencies = [
  "gimli",
 ]
 
 [[package]]
 name = "adler"
 version = "1.0.2"
@@ -63,17 +63,17 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "backtrace"
-version = "0.3.65"
+version = "0.3.67"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11a17d453482a265fd5f8479f2a3f405566e6ca627837aaddb85af8b1ab8ef61"
+checksum = "233d376d6d185f2a3093e58f283f60f880315b6c60075b01f36b3b85154564ca"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
@@ -344,17 +344,17 @@
 dependencies = [
  "cc",
  "temp-dir",
 ]
 
 [[package]]
 name = "gimli"
-version = "0.26.1"
+version = "0.27.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "78cc372d058dcf6d5ecd98510e7fbc9e5aec4d21de70f65fea8fecebcd881bd4"
+checksum = "ad0a93d233ebf96623465aad4046a8d3aa4da22d4f4beba5388838c8a434bbb4"
 
 [[package]]
 name = "hermit-abi"
 version = "0.1.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
 dependencies = [
@@ -500,17 +500,17 @@
 checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "miniz_oxide"
-version = "0.5.3"
+version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f5c75688da582b8ffc1f1799e9db273f32133c49e048f614d22ec3256773ccc"
+checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "nitro_fs"
 version = "0.1.1"
@@ -611,17 +611,17 @@
 checksum = "c92d4ddb4bd7b50d730c215ff871754d0da6b2178849f8a2a2ab69712d0c073b"
 dependencies = [
  "objc",
 ]
 
 [[package]]
 name = "object"
-version = "0.28.4"
+version = "0.30.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e42c982f2d955fac81dd7e1d0e1426a7d702acd9c98d19ab01083a6a0328c424"
+checksum = "ea86265d3d3dcb6a27fc51bd29a4bf387fae9d2986b823079d4986af253eb439"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.12.0"
@@ -864,17 +864,17 @@
 name = "regex-syntax"
 version = "0.6.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49b3de9ec5dc0a3417da371aab17d729997c15010e7fd24ff707773a33bddb64"
 
 [[package]]
 name = "rustc-demangle"
-version = "0.1.21"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ef03e0a2b150c7a90d01faf6254c9c48a41e95fb2a8c2ac1c6f0d2b9aefc342"
+checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
 
 [[package]]
 name = "rustversion"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a0a5f7c728f5d284929a1cccb5bc19884422bfe6ef4d6c409da2c41838983fcf"
 
@@ -888,15 +888,15 @@
 name = "serde"
 version = "1.0.137"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "61ea8d54c77f8315140a05f4c7237403bf38b72704d031543aa1d16abbf517d1"
 
 [[package]]
 name = "skytemple_rust"
-version = "1.5.3"
+version = "1.6.0"
 dependencies = [
  "anyhow",
  "arr_macro",
  "bytes",
  "encoding",
  "encoding-index-singlebyte",
  "gettext-rs",
@@ -1014,17 +1014,17 @@
 name = "unicode-ident"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5bd2fe26506023ed7b5e1e315add59d6f584c621d037f9368fea9cfb988f368c"
 
 [[package]]
 name = "unicode-xid"
-version = "0.2.3"
+version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "957e51f3646910546462e67d5f7599b9e4fb8acdd304b087a6494730f9eebf04"
+checksum = "f962df74c8c05a667b5ee8bcf162993134c104e96440b663c8daa176dc772d8c"
 
 [[package]]
 name = "unindent"
 version = "0.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "52fee519a3e570f7df377a06a1a7775cdbfb7aa460be7e08de2b1f0e69973a44"
```

### Comparing `skytemple-rust-1.5.3/Cargo.toml` & `skytemple-rust-1.6.0a1/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [package]
 name = "skytemple_rust"
-version = "1.5.3"
+version = "1.6.0"
 authors = ["Marco 'Capypara' Köpcke <hello@capypara.de>"]
 edition = "2021"
 repository = "https://github.com/SkyTemple/skytemple-rust"
 license = "GPL-3.0-or-later"
 
 [lib]
 crate-type = ["cdylib", "rlib"]
 name = "skytemple_rust"
 
 [features]
 default = [
     "python", "strings", "compression", "image",
     "sir0", "kao", "map_bg", "dungeon_graphics", "misc_graphics", "dse",
     "md", "item_p", "waza_p", "mappa_bin",
-    "with_pmd_wan"
+    "with_pmd_wan", "script_var_table"
 ]
 # non default: romfs
 
 python = ["pyo3", "pyo3-log"]
 
 strings = ["encoding-index-singlebyte"]
 compression = []
@@ -31,14 +31,15 @@
 misc_graphics = ["image"]
 dungeon_graphics = ["image"]
 dse = ["time"]
 md = ["packed_struct"]
 item_p = ["packed_struct", "sir0"]
 waza_p = ["packed_struct", "sir0", "md"]
 mappa_bin = ["packed_struct", "sir0"]
+script_var_table = ["packed_struct"]
 
 with_pmd_wan = ["pmd_wan", "anyhow", "python"]
 
 romfs = ["nitro_fs", "memmap2", "strings"]
 
 [dependencies]
 skytemple_rust_macros = { path = "skytemple_rust_macros" }
```

### Comparing `skytemple-rust-1.5.3/LICENSE` & `skytemple-rust-1.6.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/PKG-INFO` & `skytemple-rust-1.6.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skytemple-rust
-Version: 1.5.3
+Version: 1.6.0a1
 Summary: Binary Rust extension for skytemple-files
 Home-page: https://github.com/SkyTemple/skytemple-rust/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Rust
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -16,15 +16,15 @@
 License-File: LICENSE
 
 SkyTemple Rust Extensions
 =========================
 
 |build| |pypi-version| |pypi-downloads| |pypi-license| |pypi-pyversions| |discord|
 
-.. |build| image:: https://img.shields.io/github/workflow/status/SkyTemple/skytemple-rust/Build,%20test%20and%20publish
+.. |build| image:: https://img.shields.io/github/actions/workflow/status/SkyTemple/skytemple-rust/build-test-publish.yml
     :target: https://pypi.org/project/skytemple-rust/
     :alt: Build Status
 
 .. |pypi-version| image:: https://img.shields.io/pypi/v/skytemple-rust
     :target: https://pypi.org/project/skytemple-rust/
     :alt: Version
```

### Comparing `skytemple-rust-1.5.3/README.rst` & `skytemple-rust-1.6.0a1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 SkyTemple Rust Extensions
 =========================
 
 |build| |pypi-version| |pypi-downloads| |pypi-license| |pypi-pyversions| |discord|
 
-.. |build| image:: https://img.shields.io/github/workflow/status/SkyTemple/skytemple-rust/Build,%20test%20and%20publish
+.. |build| image:: https://img.shields.io/github/actions/workflow/status/SkyTemple/skytemple-rust/build-test-publish.yml
     :target: https://pypi.org/project/skytemple-rust/
     :alt: Build Status
 
 .. |pypi-version| image:: https://img.shields.io/pypi/v/skytemple-rust
     :target: https://pypi.org/project/skytemple-rust/
     :alt: Version
```

### Comparing `skytemple-rust-1.5.3/setup.py` & `skytemple-rust-1.6.0a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.5.3'
+__version__ = '1.6.0a1'
 
 from setuptools import setup
 from setuptools_rust import Binding, RustExtension
 
 # README read-in
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
```

### Comparing `skytemple-rust-1.5.3/skytemple_rust/pmd_wan.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/pmd_wan.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_at3px.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_at3px.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_at4pn.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_at4pn.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_at4px.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_at4px.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_atupx.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_atupx.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_bg_list_dat.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_bg_list_dat.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_bgp.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_bgp.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_bma.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_bma.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_bpa.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_bpa.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #  SkyTemple is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with SkyTemple.  If not, see <https://www.gnu.org/licenses/>.
-from typing import List, Sequence, Optional
+from typing import List, Sequence
 
 from PIL import Image
 from range_typed_integers import *
 
 
 class BpaFrameInfo:
     duration_per_frame: u16
@@ -33,15 +33,15 @@
     frame_info: Sequence[BpaFrameInfo]
 
     def __init__(self, data: bytes): ...
     @classmethod
     def new_empty(cls) -> 'Bpa': ...
     def get_tile(self, tile_idx: int, frame_idx: int) -> bytes: ...
     def tiles_to_pil_separate(self, palette: Sequence[int], width_in_tiles: int = 20) -> List[Image.Image]: ...
-    def tiles_to_pil(self, palette: Sequence[int]) -> Optional[Image.Image]: ...
+    def tiles_to_pil(self, palette: Sequence[int]) -> Image.Image: ...
     def pil_to_tiles(self, image: Image.Image) -> None: ...
     def pil_to_tiles_separate(self, images: List[Image.Image]) -> None: ...
     def tiles_for_frame(self, frame: int) -> Sequence[bytes]: ...
 
 
 class BpaWriter:
     def __new__(cls): ...
```

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_bpc.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_bpc.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_bpl.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_bpl.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_dbg.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_dbg.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_dma.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_dma.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_dpc.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_dpc.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_dpci.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_dpci.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_dpl.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_dpl.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_dpla.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_dpla.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_item_p.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_item_p.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_kao.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_kao.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_mappa_bin.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_mappa_bin.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_md.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_md.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_pkdpx.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_pkdpx.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_sir0.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_sir0.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_smdl.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_smdl.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_ssb.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_ssb.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_string.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_string.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_swdl.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_swdl.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust/st_waza_p.pyi` & `skytemple-rust-1.6.0a1/skytemple_rust/st_waza_p.pyi`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust.egg-info/PKG-INFO` & `skytemple-rust-1.6.0a1/skytemple_rust.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skytemple-rust
-Version: 1.5.3
+Version: 1.6.0a1
 Summary: Binary Rust extension for skytemple-files
 Home-page: https://github.com/SkyTemple/skytemple-rust/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Rust
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -16,15 +16,15 @@
 License-File: LICENSE
 
 SkyTemple Rust Extensions
 =========================
 
 |build| |pypi-version| |pypi-downloads| |pypi-license| |pypi-pyversions| |discord|
 
-.. |build| image:: https://img.shields.io/github/workflow/status/SkyTemple/skytemple-rust/Build,%20test%20and%20publish
+.. |build| image:: https://img.shields.io/github/actions/workflow/status/SkyTemple/skytemple-rust/build-test-publish.yml
     :target: https://pypi.org/project/skytemple-rust/
     :alt: Build Status
 
 .. |pypi-version| image:: https://img.shields.io/pypi/v/skytemple-rust
     :target: https://pypi.org/project/skytemple-rust/
     :alt: Version
```

### Comparing `skytemple-rust-1.5.3/skytemple_rust.egg-info/SOURCES.txt` & `skytemple-rust-1.6.0a1/skytemple_rust.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 skytemple_rust/st_dpl.pyi
 skytemple_rust/st_dpla.pyi
 skytemple_rust/st_item_p.pyi
 skytemple_rust/st_kao.pyi
 skytemple_rust/st_mappa_bin.pyi
 skytemple_rust/st_md.pyi
 skytemple_rust/st_pkdpx.pyi
+skytemple_rust/st_script_var_table.pyi
 skytemple_rust/st_sir0.pyi
 skytemple_rust/st_smdl.pyi
 skytemple_rust/st_ssb.pyi
 skytemple_rust/st_string.pyi
 skytemple_rust/st_swdl.pyi
 skytemple_rust/st_waza_p.pyi
 skytemple_rust.egg-info/PKG-INFO
@@ -76,14 +77,15 @@
 src/st_dpci.rs
 src/st_dpl.rs
 src/st_dpla.rs
 src/st_item_p.rs
 src/st_kao.rs
 src/st_md.rs
 src/st_pkdpx.rs
+src/st_script_var_table.rs
 src/st_sir0.rs
 src/st_string.rs
 src/st_waza_p.rs
 src/util.rs
 src/compression/bma_collision_rle.rs
 src/compression/bma_layer_nrl.rs
 src/compression/bpc_image.rs
```

### Comparing `skytemple-rust-1.5.3/skytemple_rust_macros/src/lib.rs` & `skytemple-rust-1.6.0a1/skytemple_rust_macros/src/lib.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/skytemple_rust_macros_no_py/src/lib.rs` & `skytemple-rust-1.6.0a1/skytemple_rust_macros_no_py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/bytes.rs` & `skytemple-rust-1.6.0a1/src/bytes.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/compression/bma_collision_rle.rs` & `skytemple-rust-1.6.0a1/src/compression/bma_collision_rle.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/compression/bma_layer_nrl.rs` & `skytemple-rust-1.6.0a1/src/compression/bma_layer_nrl.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/compression/bpc_image.rs` & `skytemple-rust-1.6.0a1/src/compression/bpc_image.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/compression/bpc_tilemap.rs` & `skytemple-rust-1.6.0a1/src/compression/bpc_tilemap.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/compression/custom_999.rs` & `skytemple-rust-1.6.0a1/src/compression/custom_999.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/compression/generic/mod.rs` & `skytemple-rust-1.6.0a1/src/compression/generic/mod.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/compression/generic/nrl.rs` & `skytemple-rust-1.6.0a1/src/compression/generic/nrl.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/compression/mod.rs` & `skytemple-rust-1.6.0a1/src/compression/mod.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/compression/px.rs` & `skytemple-rust-1.6.0a1/src/compression/px.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/dse/date.rs` & `skytemple-rust-1.6.0a1/src/dse/date.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/dse/filename.rs` & `skytemple-rust-1.6.0a1/src/dse/filename.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/dse/mod.rs` & `skytemple-rust-1.6.0a1/src/dse/mod.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/dse/st_smdl/eoc.rs` & `skytemple-rust-1.6.0a1/src/dse/st_smdl/eoc.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/dse/st_smdl/event.rs` & `skytemple-rust-1.6.0a1/src/dse/st_smdl/event.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/dse/st_smdl/mod.rs` & `skytemple-rust-1.6.0a1/src/dse/st_smdl/mod.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/dse/st_smdl/python.rs` & `skytemple-rust-1.6.0a1/src/dse/st_smdl/python.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/dse/st_smdl/smdl.rs` & `skytemple-rust-1.6.0a1/src/dse/st_smdl/smdl.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/dse/st_smdl/song.rs` & `skytemple-rust-1.6.0a1/src/dse/st_smdl/song.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/dse/st_smdl/trk.rs` & `skytemple-rust-1.6.0a1/src/dse/st_smdl/trk.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/dse/st_swdl/kgrp.rs` & `skytemple-rust-1.6.0a1/src/dse/st_swdl/kgrp.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/dse/st_swdl/mod.rs` & `skytemple-rust-1.6.0a1/src/dse/st_swdl/mod.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/dse/st_swdl/pcmd.rs` & `skytemple-rust-1.6.0a1/src/dse/st_swdl/pcmd.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/dse/st_swdl/prgi.rs` & `skytemple-rust-1.6.0a1/src/dse/st_swdl/prgi.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/dse/st_swdl/python.rs` & `skytemple-rust-1.6.0a1/src/dse/st_swdl/python.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/dse/st_swdl/swdl.rs` & `skytemple-rust-1.6.0a1/src/dse/st_swdl/swdl.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/dse/st_swdl/wavi.rs` & `skytemple-rust-1.6.0a1/src/dse/st_swdl/wavi.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/encoding/mod.rs` & `skytemple-rust-1.6.0a1/src/encoding/mod.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/encoding/pmd2_encoder.rs` & `skytemple-rust-1.6.0a1/src/encoding/pmd2_encoder.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/encoding_utils.rs` & `skytemple-rust-1.6.0a1/src/encoding_utils.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/err.rs` & `skytemple-rust-1.6.0a1/src/err.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/gettext/macro_stub.rs` & `skytemple-rust-1.6.0a1/src/gettext/macro_stub.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/gettext/mod.rs` & `skytemple-rust-1.6.0a1/src/gettext/mod.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/image/mod.rs` & `skytemple-rust-1.6.0a1/src/image/mod.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/image/tiled.rs` & `skytemple-rust-1.6.0a1/src/image/tiled.rs`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
                         tile_palette_indices[tile_id],
                     ))
                 });
         } else {
             final_tiles_with_sum = tiles_with_sum;
         }
         if final_tiles_with_sum.len() > 1024 {
-            return Err(create_value_user_error(gettext!(
+            return Err(exceptions::PyValueError::new_err(gettext!(
                 "An image selected to import is too complex. It has too many unique tiles ({}, max allowed are 1024).\nTry to have less unique tiles. Unique tiles are 8x8 sections of the images that can't be found anywhere else in the image (including flipped or with a different sub-palette).",
                 final_tiles_with_sum.len()
             )));
         }
 
         Ok((
             final_tiles_with_sum.into_iter().map(|x| x.1).collect(),
```

### Comparing `skytemple-rust-1.5.3/src/image/tilemap_entry.rs` & `skytemple-rust-1.6.0a1/src/image/tilemap_entry.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/lib.rs` & `skytemple-rust-1.6.0a1/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,16 @@
 pub mod st_kao;
 #[cfg(feature = "mappa_bin")]
 pub mod st_mappa_bin;
 #[cfg(feature = "md")]
 pub mod st_md;
 #[cfg(feature = "compression")]
 pub mod st_pkdpx;
+#[cfg(feature = "script_var_table")]
+pub mod st_script_var_table;
 #[cfg(feature = "sir0")]
 pub mod st_sir0;
 #[cfg(feature = "strings")]
 pub mod st_string;
 #[cfg(feature = "waza_p")]
 pub mod st_waza_p;
```

### Comparing `skytemple-rust-1.5.3/src/macros.rs` & `skytemple-rust-1.6.0a1/src/macros.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/no_python.rs` & `skytemple-rust-1.6.0a1/src/no_python.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/pmd_wan.rs` & `skytemple-rust-1.6.0a1/src/pmd_wan.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/python.rs` & `skytemple-rust-1.6.0a1/src/python.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/python_image.rs` & `skytemple-rust-1.6.0a1/src/python_image.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/python_module.rs` & `skytemple-rust-1.6.0a1/src/python_module.rs`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,16 @@
 use crate::st_kao::create_st_kao_module;
 #[cfg(feature = "mappa_bin")]
 use crate::st_mappa_bin::create_st_mappa_bin_module;
 #[cfg(feature = "md")]
 use crate::st_md::create_st_md_module;
 #[cfg(feature = "compression")]
 use crate::st_pkdpx::create_st_pkdpx_module;
+#[cfg(feature = "script_var_table")]
+use crate::st_script_var_table::create_st_script_var_table_module;
 #[cfg(feature = "sir0")]
 use crate::st_sir0::create_st_sir0_module;
 #[cfg(feature = "strings")]
 use crate::st_string::create_st_string_module;
 #[cfg(feature = "waza_p")]
 use crate::st_waza_p::create_st_waza_p_module;
 
@@ -147,14 +149,16 @@
     add_submodule(module, create_st_mappa_bin_module(py)?, modules)?;
     #[cfg(feature = "dse")]
     add_submodule(module, create_st_smdl_module(py)?, modules)?;
     #[cfg(feature = "dse")]
     add_submodule(module, create_st_swdl_module(py)?, modules)?;
     #[cfg(feature = "strings")]
     add_submodule(module, create_st_string_module(py)?, modules)?;
+    #[cfg(feature = "script_var_table")]
+    add_submodule(module, create_st_script_var_table_module(py)?, modules)?;
 
     #[cfg(feature = "compression")]
     add_submodule(
         module,
         create_st_generic_nrl_compression_module(py)?,
         modules,
     )?;
```

### Comparing `skytemple-rust-1.5.3/src/rom_source.rs` & `skytemple-rust-1.6.0a1/src/rom_source.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/romfs.rs` & `skytemple-rust-1.6.0a1/src/romfs.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_at3px.rs` & `skytemple-rust-1.6.0a1/src/st_at3px.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_at4pn.rs` & `skytemple-rust-1.6.0a1/src/st_at4pn.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_at4px.rs` & `skytemple-rust-1.6.0a1/src/st_at4px.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_at_common.rs` & `skytemple-rust-1.6.0a1/src/st_at_common.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_atupx.rs` & `skytemple-rust-1.6.0a1/src/st_atupx.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_bg_list_dat.rs` & `skytemple-rust-1.6.0a1/src/st_bg_list_dat.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-// this is fixed by upgrading pyo3.
-#![allow(clippy::needless_option_as_deref)]
-/*
- * Copyright 2021-2022 Capypara and the SkyTemple Contributors
- *
- * This file is part of SkyTemple.
- *
- * SkyTemple is free software: you can redistribute it and/or modify
- * it under the terms of the GNU General Public License as published by
- * the Free Software Foundation, either version 3 of the License, or
- * (at your option) any later version.
- *
- * SkyTemple is distributed in the hope that it will be useful,
- * but WITHOUT ANY WARRANTY; without even the implied warranty of
- * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
- * GNU General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License
- * along with SkyTemple.  If not, see <https://www.gnu.org/licenses/>.
- */
+#![allow(clippy::needless_option_as_deref)] // this is fixed by upgrading pyo3.
+                                            /*
+                                             * Copyright 2021-2022 Capypara and the SkyTemple Contributors
+                                             *
+                                             * This file is part of SkyTemple.
+                                             *
+                                             * SkyTemple is free software: you can redistribute it and/or modify
+                                             * it under the terms of the GNU General Public License as published by
+                                             * the Free Software Foundation, either version 3 of the License, or
+                                             * (at your option) any later version.
+                                             *
+                                             * SkyTemple is distributed in the hope that it will be useful,
+                                             * but WITHOUT ANY WARRANTY; without even the implied warranty of
+                                             * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+                                             * GNU General Public License for more details.
+                                             *
+                                             * You should have received a copy of the GNU General Public License
+                                             * along with SkyTemple.  If not, see <https://www.gnu.org/licenses/>.
+                                             */
 use crate::bytes::StBytes;
 use crate::encoding::{BufEncoding, BufMutEncoding};
 use crate::err::convert_io_err;
 use crate::python::*;
 use crate::rom_source::{RomFileProvider, RomSource};
 use crate::st_bma::Bma;
 use crate::st_bpa::Bpa;
```

### Comparing `skytemple-rust-1.5.3/src/st_bgp.rs` & `skytemple-rust-1.6.0a1/src/st_bgp.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_bma.rs` & `skytemple-rust-1.6.0a1/src/st_bma.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_bpa.rs` & `skytemple-rust-1.6.0a1/src/st_bpa.rs`

 * *Files 1% similar despite different names*

```diff
@@ -99,20 +99,15 @@
     }
     /// Returns the tile data of tile no. tile_idx for frame frame_idx.
     pub fn get_tile(&self, tile_idx: usize, frame_idx: usize) -> StBytes {
         self.tiles[frame_idx * self.number_of_tiles as usize + tile_idx].clone()
     }
     /// Exports the BPA as an image, where each row of 8x8 tiles is the
     /// animation set for a single tile. The 16 color palette passed is used to color the image.
-    ///
-    /// Returns None if the BPA has no tiles.
-    pub fn tiles_to_pil(&self, palette: StBytes) -> Option<IndexedImage> {
-        if self.number_of_tiles < 1 {
-            return None;
-        }
+    pub fn tiles_to_pil(&self, palette: StBytes) -> IndexedImage {
         // Create a dummy tile map containing all the tiles.
         // The tiles in the BPA are stored so, that each tile of the each frame is next
         // to each other. So the second frame of the first tile is at self.number_of_images + 1.
         let mut dummy_chunks =
             Vec::with_capacity((self.number_of_tiles * self.number_of_frames) as usize);
         for tile_idx in 0..self.number_of_tiles {
             for frame_idx in 0..self.number_of_frames {
@@ -125,35 +120,32 @@
             }
         }
 
         let etr = (self.number_of_frames * self.number_of_tiles) as usize;
         let width = self.number_of_frames as usize * BPA_TILE_DIM;
         let height = ((etr as f32 / self.number_of_frames as f32).ceil()) as usize * BPA_TILE_DIM;
 
-        Some(TiledImage::tiled_to_native(
+        TiledImage::tiled_to_native(
             dummy_chunks.into_iter(),
             PixelGenerator::tiled4bpp(&self.tiles[..]),
             palette.iter().copied(),
             BPA_TILE_DIM,
             width,
             height,
             1,
-        ))
+        )
     }
     #[args(width_in_tiles = "20")]
     /// Exports the BPA as an image, where each row of 8x8 tiles is the
     /// animation set for a single tile. The 16 color palette passed is used to color the image.
     pub fn tiles_to_pil_separate(
         &self,
         palette: Vec<u8>,
         width_in_tiles: usize,
     ) -> PyResult<Vec<IndexedImage>> {
-        if self.number_of_tiles < 1 {
-            return Ok(vec![]);
-        }
         let dummy_chunks = (0..(self.number_of_tiles * self.number_of_frames))
             .map(|tile_idx| TilemapEntry(tile_idx as usize, false, false, 0))
             .collect::<Vec<TilemapEntry>>();
         let dummy_chunks_chunked = dummy_chunks.chunks(self.number_of_tiles as usize);
 
         let width = width_in_tiles * BPA_TILE_DIM;
         let height =
```

### Comparing `skytemple-rust-1.5.3/src/st_bpc.rs` & `skytemple-rust-1.6.0a1/src/st_bpc.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_bpl.rs` & `skytemple-rust-1.6.0a1/src/st_bpl.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_dbg.rs` & `skytemple-rust-1.6.0a1/src/st_dbg.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_dma.rs` & `skytemple-rust-1.6.0a1/src/st_dma.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_dpc.rs` & `skytemple-rust-1.6.0a1/src/st_dpc.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_dpci.rs` & `skytemple-rust-1.6.0a1/src/st_dpci.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_dpl.rs` & `skytemple-rust-1.6.0a1/src/st_dpl.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_dpla.rs` & `skytemple-rust-1.6.0a1/src/st_dpla.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_item_p.rs` & `skytemple-rust-1.6.0a1/src/st_item_p.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_kao.rs` & `skytemple-rust-1.6.0a1/src/st_kao.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_mappa_bin/enums_consts.rs` & `skytemple-rust-1.6.0a1/src/st_mappa_bin/enums_consts.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_mappa_bin/floor.rs` & `skytemple-rust-1.6.0a1/src/st_mappa_bin/floor.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_mappa_bin/item_list.rs` & `skytemple-rust-1.6.0a1/src/st_mappa_bin/item_list.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_mappa_bin/layout.rs` & `skytemple-rust-1.6.0a1/src/st_mappa_bin/layout.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_mappa_bin/mappa.rs` & `skytemple-rust-1.6.0a1/src/st_mappa_bin/mappa.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_mappa_bin/minimize.rs` & `skytemple-rust-1.6.0a1/src/st_mappa_bin/minimize.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_mappa_bin/mod.rs` & `skytemple-rust-1.6.0a1/src/st_mappa_bin/mod.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_mappa_bin/monster_list.rs` & `skytemple-rust-1.6.0a1/src/st_mappa_bin/monster_list.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_mappa_bin/pymodule.rs` & `skytemple-rust-1.6.0a1/src/st_mappa_bin/pymodule.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_mappa_bin/trap_list.rs` & `skytemple-rust-1.6.0a1/src/st_mappa_bin/trap_list.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_md.rs` & `skytemple-rust-1.6.0a1/src/st_md.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_pkdpx.rs` & `skytemple-rust-1.6.0a1/src/st_pkdpx.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_sir0.rs` & `skytemple-rust-1.6.0a1/src/st_sir0.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_string.rs` & `skytemple-rust-1.6.0a1/src/st_string.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/st_waza_p.rs` & `skytemple-rust-1.6.0a1/src/st_waza_p.rs`

 * *Files identical despite different names*

### Comparing `skytemple-rust-1.5.3/src/util.rs` & `skytemple-rust-1.6.0a1/src/util.rs`

 * *Files identical despite different names*

