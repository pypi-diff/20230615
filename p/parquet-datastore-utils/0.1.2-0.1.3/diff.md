# Comparing `tmp/parquet_datastore_utils-0.1.2-py3-none-any.whl.zip` & `tmp/parquet_datastore_utils-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 4008 bytes, number of entries: 6
+Zip file size: 4072 bytes, number of entries: 6
 -rw-r--r--  2.0 fat       37 b- defN 80-Jan-01 00:00 parquet_datastore_utils/__init__.py
 -rw-r--r--  2.0 fat      570 b- defN 80-Jan-01 00:00 parquet_datastore_utils/cleaner.py
--rw-r--r--  2.0 fat     5884 b- defN 80-Jan-01 00:00 parquet_datastore_utils/read_write.py
--rw-r--r--  2.0 fat      419 b- defN 80-Jan-01 00:00 parquet_datastore_utils-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 parquet_datastore_utils-0.1.2.dist-info/WHEEL
-?rw-r--r--  2.0 fat      527 b- defN 16-Jan-01 00:00 parquet_datastore_utils-0.1.2.dist-info/RECORD
-6 files, 7525 bytes uncompressed, 3040 bytes compressed:  59.6%
+-rw-r--r--  2.0 fat     6026 b- defN 80-Jan-01 00:00 parquet_datastore_utils/read_write.py
+-rw-r--r--  2.0 fat      626 b- defN 80-Jan-01 00:00 parquet_datastore_utils-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 parquet_datastore_utils-0.1.3.dist-info/WHEEL
+?rw-r--r--  2.0 fat      527 b- defN 16-Jan-01 00:00 parquet_datastore_utils-0.1.3.dist-info/RECORD
+6 files, 7874 bytes uncompressed, 3104 bytes compressed:  60.6%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: parquet_datastore_utils/cleaner.py
 Comment: 
 
 Filename: parquet_datastore_utils/read_write.py
 Comment: 
 
-Filename: parquet_datastore_utils-0.1.2.dist-info/METADATA
+Filename: parquet_datastore_utils-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: parquet_datastore_utils-0.1.2.dist-info/WHEEL
+Filename: parquet_datastore_utils-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: parquet_datastore_utils-0.1.2.dist-info/RECORD
+Filename: parquet_datastore_utils-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## parquet_datastore_utils/read_write.py

```diff
@@ -112,21 +112,28 @@
 
     update_tables = []
     for fragment in current_ds.fragments:
         parts = ds._get_partition_keys(fragment.partition_expression)
         if all([(data[key]==value).any() for key, value in parts.items()]):
             update_tables.append(fragment.to_table())
 
-    ind = data.index.name
-    filtered_table = pa.concat_tables(update_tables, promote=True).filter(
-        (pc.field(ind) < data.index.min()), (pc.field(ind) > data.index.max()))
-
     new_table = pa.table(data)
-    filtered_table = filtered_table.set_column(filtered_table.column_names.index(ind), ind, filtered_table[ind].cast(new_table[ind].type))
-    out = pa.concat_tables([filtered_table, new_table], promote=True)  # Promote=True to allow for mismatched schemas
+
+    if len(update_tables) > 0:
+    # Data overlaps data in exsiting fragments
+        ind = data.index.name
+        filtered_table = pa.concat_tables(update_tables, promote=True).filter(
+            (pc.field(ind) < data.index.min()), (pc.field(ind) > data.index.max()))
+
+        filtered_table = filtered_table.set_column(filtered_table.column_names.index(ind), ind, filtered_table[ind].cast(new_table[ind].type))
+
+        out = pa.concat_tables([filtered_table, new_table], promote=True)  # Promote=True to allow for mismatched schemas
+    else:
+        out = new_table
 
     pq.write_to_dataset(out, uri, partition_cols=partition_cols, use_legacy_dataset=False)
 
     dirs = set([os.path.dirname(fragment.path) for fragment in current_ds.fragments])
 
     for dir in dirs:
         delete_all_except_newest(dir)
+
```

## Comparing `parquet_datastore_utils-0.1.2.dist-info/RECORD` & `parquet_datastore_utils-0.1.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 parquet_datastore_utils/__init__.py,sha256=XxoVYuFy3yGwKLNGU2tMsNEzP4gvKgE_cQmzcjmzthY,37
 parquet_datastore_utils/cleaner.py,sha256=nBjY8IYPN9hGTUbgwVsi0iCb3EC42dE6HRojcfHfZdg,570
-parquet_datastore_utils/read_write.py,sha256=W3gX9MEuer7ca0jCJ3DpHlDj7f6MxDkYkieW8G74lcU,5884
-parquet_datastore_utils-0.1.2.dist-info/METADATA,sha256=F8HQwRSK9Jimd08ik02rFL77Aa7-Sg2MReL-8i4MMxc,419
-parquet_datastore_utils-0.1.2.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-parquet_datastore_utils-0.1.2.dist-info/RECORD,,
+parquet_datastore_utils/read_write.py,sha256=p5UMmZcfV1CRnBMYALTa_NfWUhnnVmXL7xJ7pH9PUc8,6026
+parquet_datastore_utils-0.1.3.dist-info/METADATA,sha256=YRk8GOD3DZMc4pnEZnR7Qb9XJBXcQLCIfBl_NkCCiuM,626
+parquet_datastore_utils-0.1.3.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
+parquet_datastore_utils-0.1.3.dist-info/RECORD,,
```

