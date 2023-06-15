# Comparing `tmp/ncagg-0.8.8-py2.py3-none-any.whl.zip` & `tmp/ncagg-0.8.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 33684 bytes, number of entries: 13
+Zip file size: 33797 bytes, number of entries: 13
 -rw-r--r--  2.0 unx       72 b- defN 19-Feb-06 16:56 ncagg/__init__.py
 -rw-r--r--  2.0 unx       27 b- defN 19-Feb-06 16:56 ncagg/__main__.py
--rw-r--r--  2.0 unx    17950 b- defN 19-Feb-15 20:27 ncagg/aggregator.py
+-rw-r--r--  2.0 unx    18288 b- defN 19-Feb-21 01:07 ncagg/aggregator.py
 -rw-r--r--  2.0 unx    26998 b- defN 19-Feb-16 00:24 ncagg/aggrelist.py
 -rw-r--r--  2.0 unx    11795 b- defN 19-Feb-06 16:56 ncagg/attributes.py
 -rw-r--r--  2.0 unx     8085 b- defN 19-Feb-06 16:56 ncagg/cli.py
 -rw-r--r--  2.0 unx    13438 b- defN 19-Feb-06 16:56 ncagg/config.py
--rw-r--r--  2.0 unx     1072 b- defN 19-Feb-16 00:25 ncagg-0.8.8.dist-info/LICENSE
--rw-r--r--  2.0 unx    20862 b- defN 19-Feb-16 00:25 ncagg-0.8.8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 19-Feb-16 00:25 ncagg-0.8.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 19-Feb-16 00:25 ncagg-0.8.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 19-Feb-16 00:25 ncagg-0.8.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      986 b- defN 19-Feb-16 00:25 ncagg-0.8.8.dist-info/RECORD
-13 files, 101460 bytes uncompressed, 32066 bytes compressed:  68.4%
+-rw-r--r--  2.0 unx     1072 b- defN 19-Feb-21 01:08 ncagg-0.8.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx    20862 b- defN 19-Feb-21 01:08 ncagg-0.8.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 19-Feb-21 01:08 ncagg-0.8.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 19-Feb-21 01:08 ncagg-0.8.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 19-Feb-21 01:08 ncagg-0.8.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      986 b- defN 19-Feb-21 01:08 ncagg-0.8.9.dist-info/RECORD
+13 files, 101798 bytes uncompressed, 32179 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: ncagg/cli.py
 Comment: 
 
 Filename: ncagg/config.py
 Comment: 
 
-Filename: ncagg-0.8.8.dist-info/LICENSE
+Filename: ncagg-0.8.9.dist-info/LICENSE
 Comment: 
 
-Filename: ncagg-0.8.8.dist-info/METADATA
+Filename: ncagg-0.8.9.dist-info/METADATA
 Comment: 
 
-Filename: ncagg-0.8.8.dist-info/WHEEL
+Filename: ncagg-0.8.9.dist-info/WHEEL
 Comment: 
 
-Filename: ncagg-0.8.8.dist-info/entry_points.txt
+Filename: ncagg-0.8.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: ncagg-0.8.8.dist-info/top_level.txt
+Filename: ncagg-0.8.9.dist-info/top_level.txt
 Comment: 
 
-Filename: ncagg-0.8.8.dist-info/RECORD
+Filename: ncagg-0.8.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ncagg/aggregator.py

```diff
@@ -140,27 +140,32 @@
         else:
             # CASE: first file, take the bound and subtract a min time step so that
             # the first time step greater than or equal to the bound will be included.
             # Historical: numerical issues here? What happened... was I mistaken? .. probably.
             prev_end = first_along_primary - dt_min
             gap_between = next_start - prev_end
 
-        # gap too big if skips 1.5 of the largest possible expected dt...
-        if gap_between > 1.5 * dt_max:  # <----------- CASE: gap-too-big
+        # gap too big if skips 1.62 of the largest possible expected dt...
+        # The value 1.62 is picked somewhat artfully... just make sure all the tests pass.
+        if gap_between > 1.6 * dt_max and next_start - dt_nom > first_along_primary:  # <----------- CASE: gap-too-big
             # if the gap is too big, insert an appropriate fill value.
             if len(final) > 0:  # <-------------- CASE: exists-previous-file
                 size = int(max(1, np.round((gap_between-dt_nom) * cadence_hz)))  # probably correct
                 # when there is a previous file, make timestamps even from end of that one
                 start_from = prev_end
             else:  # <------------- CASE: no-previous-file
                 size = int(max(1, np.floor((gap_between-dt_nom) * cadence_hz)))  # probably correct
                 # otherwise look at the next timestamp, and go backward _size_ from there to get the start_from.
                 start_from = next_start - ((size+1) * dt_nom)
                 # note: start_from must be greater than first_along_primary
-                assert start_from + dt_nom >= first_along_primary
+                try:
+                    assert start_from + dt_nom >= first_along_primary, "{} + {}, {}".format(start_from,
+                            dt_nom, first_along_primary)
+                except Exception:
+                    import ipdb; ipdb.set_trace()
 
             fill_node = FillNode(config)
             fill_node.set_udim(primary_index_by, size, start_from)
             final.append(fill_node)
 
         # if the gap is too small, chop some off this next file to make it fit...
         if gap_between < dt_min:  # <----------- CASE: gap-too-small
```

## Comparing `ncagg-0.8.8.dist-info/LICENSE` & `ncagg-0.8.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ncagg-0.8.8.dist-info/METADATA` & `ncagg-0.8.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncagg
-Version: 0.8.8
+Version: 0.8.9
 Summary: Utility for aggregation of NetCDF data.
 Home-page: https://github.com/5tefan/ncagg
 Author: Stefan Codrescu
 Author-email: stefan.codrescu@noaa.gov
 License: UNKNOWN
 Project-URL: Documentation, http://ncagg.readthedocs.io/en/latest/
 Platform: UNKNOWN
```

## Comparing `ncagg-0.8.8.dist-info/RECORD` & `ncagg-0.8.9.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ncagg/__init__.py,sha256=KKhqFPynKFNc63uoMaOOsRxKbGFMfUOr4Qer7J67jCI,72
 ncagg/__main__.py,sha256=D2AYEG813n93eaC7YLDkD_BKi2BSMYl9Kl0RuB6kJAk,27
-ncagg/aggregator.py,sha256=TIVkkFJI3HLRh3qFwDFROGsDXgdzxNcnFNm149fFJWk,17950
+ncagg/aggregator.py,sha256=nUfvxbRGvrliKtWAGhsCiel9nMF7yf2m5eotIy38Pw0,18288
 ncagg/aggrelist.py,sha256=mAJpX-OFTARvKiRyqopkgwNwldfWlFpQKnF9qFgDuGY,26998
 ncagg/attributes.py,sha256=Lw_93qJ0yyCyGVgvGIEpB7eUiLZG1vsz7Tn1VT4TX3I,11795
 ncagg/cli.py,sha256=ydliysxyCojMpf-6WTBF7tXL3vDLIUP7ZQWdSQfGczU,8085
 ncagg/config.py,sha256=DckfFpuHdYJFvCs2KvDGMqC0nJTzwpBjL07V3LcbCes,13438
-ncagg-0.8.8.dist-info/LICENSE,sha256=FR4g-DHkTR6Oj8-ahKLmNZ-587K6c28teb2YpAvJ2pk,1072
-ncagg-0.8.8.dist-info/METADATA,sha256=v7H-neSTTVJqEoxvPXDno2y8KV2hWxgD3SJdb_olfqw,20862
-ncagg-0.8.8.dist-info/WHEEL,sha256=_wJFdOYk7i3xxT8ElOkUJvOdOvfNGbR9g-bf6UQT6sU,110
-ncagg-0.8.8.dist-info/entry_points.txt,sha256=xFUQNGslRcOvRy6jYHNhj4iISajdVn7FPTxhyWAMhTI,59
-ncagg-0.8.8.dist-info/top_level.txt,sha256=JSeELqO4UZVuu9GihZMepQluq9aCzki2otfSMboEerQ,6
-ncagg-0.8.8.dist-info/RECORD,,
+ncagg-0.8.9.dist-info/LICENSE,sha256=FR4g-DHkTR6Oj8-ahKLmNZ-587K6c28teb2YpAvJ2pk,1072
+ncagg-0.8.9.dist-info/METADATA,sha256=Wp6sjNJOf-S-Uel6rj8EboLKgAzxDezVcK1Ic8pJQ8w,20862
+ncagg-0.8.9.dist-info/WHEEL,sha256=_wJFdOYk7i3xxT8ElOkUJvOdOvfNGbR9g-bf6UQT6sU,110
+ncagg-0.8.9.dist-info/entry_points.txt,sha256=xFUQNGslRcOvRy6jYHNhj4iISajdVn7FPTxhyWAMhTI,59
+ncagg-0.8.9.dist-info/top_level.txt,sha256=JSeELqO4UZVuu9GihZMepQluq9aCzki2otfSMboEerQ,6
+ncagg-0.8.9.dist-info/RECORD,,
```

