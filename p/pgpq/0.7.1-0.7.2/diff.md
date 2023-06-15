# Comparing `tmp/pgpq-0.7.1.tar.gz` & `tmp/pgpq-0.7.2.tar.gz`

## Comparing `pgpq-0.7.1.tar` & `pgpq-0.7.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 pgpq-0.7.1/local_dependencies/pgpq/Cargo.toml
--rw-r--r--   0      501       20      104 2023-03-31 16:34:53.000000 pgpq-0.7.1/local_dependencies/pgpq/README.md
--rw-r--r--   0      501       20    10455 2023-03-31 16:34:53.000000 pgpq-0.7.1/local_dependencies/pgpq/benches/experiments.rs
--rw-r--r--   0      501       20     2765 2023-03-31 16:34:53.000000 pgpq-0.7.1/local_dependencies/pgpq/benches/yellow_cab_dataset.rs
--rw-r--r--   0      501       20    39783 2023-03-31 16:34:53.000000 pgpq-0.7.1/local_dependencies/pgpq/src/encoders.rs
--rw-r--r--   0      501       20     2495 2023-03-31 16:34:53.000000 pgpq-0.7.1/local_dependencies/pgpq/src/error.rs
--rw-r--r--   0      501       20     7733 2023-03-31 16:34:53.000000 pgpq-0.7.1/local_dependencies/pgpq/src/lib.rs
--rw-r--r--   0      501       20     3352 2023-03-31 16:34:53.000000 pgpq-0.7.1/local_dependencies/pgpq/src/pg_schema.rs
--rw-r--r--   0        0        0      408 1970-01-01 00:00:00.000000 pgpq-0.7.1/Cargo.toml
--rw-r--r--   0      501       20     1579 2023-03-31 16:34:53.000000 pgpq-0.7.1/README.md
--rw-r--r--   0      501       20     3040 2023-03-31 16:34:53.000000 pgpq-0.7.1/benches/encode.ipynb
--rw-r--r--   0      501       20     1490 2023-03-31 16:34:53.000000 pgpq-0.7.1/example.py
--rw-r--r--   0      501       20     1361 2023-03-31 16:34:53.000000 pgpq-0.7.1/pyproject.toml
--rw-r--r--   0      501       20      139 2023-03-31 16:34:53.000000 pgpq-0.7.1/python/pgpq/__init__.py
--rw-r--r--   0      501       20     6078 2023-03-31 16:34:53.000000 pgpq-0.7.1/python/pgpq/_pgpq.pyi
--rw-r--r--   0      501       20     1770 2023-03-31 16:34:53.000000 pgpq-0.7.1/python/pgpq/encoders.py
--rw-r--r--   0      501       20        0 2023-03-31 16:34:53.000000 pgpq-0.7.1/python/pgpq/py.typed
--rw-r--r--   0      501       20      581 2023-03-31 16:34:53.000000 pgpq-0.7.1/python/pgpq/schema.py
--rw-r--r--   0      501       20    39649 2023-03-31 16:34:53.000000 pgpq-0.7.1/src/encoders.rs
--rw-r--r--   0      501       20     5784 2023-03-31 16:34:53.000000 pgpq-0.7.1/src/lib.rs
--rw-r--r--   0      501       20    13016 2023-03-31 16:34:53.000000 pgpq-0.7.1/src/pg_schema.rs
--rw-r--r--   0      501       20     1864 2023-03-31 16:34:53.000000 pgpq-0.7.1/src/template.py
--rw-r--r--   0      501       20       96 2023-03-31 16:34:53.000000 pgpq-0.7.1/src/utils.rs
--rw-r--r--   0      501       20        0 2023-03-31 16:34:53.000000 pgpq-0.7.1/test_pgpq/__init__.py
--rw-r--r--   0      501       20     7208 2023-03-31 16:34:53.000000 pgpq-0.7.1/test_pgpq/test_pgpq.py
--rw-r--r--   0        0        0     2832 1970-01-01 00:00:00.000000 pgpq-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 pgpq-0.7.2/local_dependencies/pgpq/Cargo.toml
+-rw-r--r--   0      501       20      104 2023-06-15 05:00:42.000000 pgpq-0.7.2/local_dependencies/pgpq/README.md
+-rw-r--r--   0      501       20    10455 2023-06-15 05:00:42.000000 pgpq-0.7.2/local_dependencies/pgpq/benches/experiments.rs
+-rw-r--r--   0      501       20     2765 2023-06-15 05:00:42.000000 pgpq-0.7.2/local_dependencies/pgpq/benches/yellow_cab_dataset.rs
+-rw-r--r--   0      501       20    40799 2023-06-15 05:00:42.000000 pgpq-0.7.2/local_dependencies/pgpq/src/encoders.rs
+-rw-r--r--   0      501       20     2495 2023-06-15 05:00:42.000000 pgpq-0.7.2/local_dependencies/pgpq/src/error.rs
+-rw-r--r--   0      501       20     7733 2023-06-15 05:00:42.000000 pgpq-0.7.2/local_dependencies/pgpq/src/lib.rs
+-rw-r--r--   0      501       20     3516 2023-06-15 05:00:42.000000 pgpq-0.7.2/local_dependencies/pgpq/src/pg_schema.rs
+-rw-r--r--   0        0        0      408 1970-01-01 00:00:00.000000 pgpq-0.7.2/Cargo.toml
+-rw-r--r--   0      501       20     2191 2023-06-15 05:00:42.000000 pgpq-0.7.2/README.md
+-rw-r--r--   0      501       20     3034 2023-06-15 05:00:42.000000 pgpq-0.7.2/benches/encode.ipynb
+-rw-r--r--   0      501       20     2136 2023-06-15 05:00:42.000000 pgpq-0.7.2/example.py
+-rw-r--r--   0      501       20     1362 2023-06-15 05:00:42.000000 pgpq-0.7.2/pyproject.toml
+-rw-r--r--   0      501       20      139 2023-06-15 05:00:42.000000 pgpq-0.7.2/python/pgpq/__init__.py
+-rw-r--r--   0      501       20     6078 2023-06-15 05:00:42.000000 pgpq-0.7.2/python/pgpq/_pgpq.pyi
+-rw-r--r--   0      501       20     1770 2023-06-15 05:00:42.000000 pgpq-0.7.2/python/pgpq/encoders.py
+-rw-r--r--   0      501       20        0 2023-06-15 05:00:42.000000 pgpq-0.7.2/python/pgpq/py.typed
+-rw-r--r--   0      501       20      581 2023-06-15 05:00:42.000000 pgpq-0.7.2/python/pgpq/schema.py
+-rw-r--r--   0      501       20    39649 2023-06-15 05:00:42.000000 pgpq-0.7.2/src/encoders.rs
+-rw-r--r--   0      501       20     5784 2023-06-15 05:00:42.000000 pgpq-0.7.2/src/lib.rs
+-rw-r--r--   0      501       20    13436 2023-06-15 05:00:42.000000 pgpq-0.7.2/src/pg_schema.rs
+-rw-r--r--   0      501       20     1876 2023-06-15 05:00:42.000000 pgpq-0.7.2/src/template.py
+-rw-r--r--   0      501       20       96 2023-06-15 05:00:42.000000 pgpq-0.7.2/src/utils.rs
+-rw-r--r--   0      501       20        0 2023-06-15 05:00:42.000000 pgpq-0.7.2/test_pgpq/__init__.py
+-rw-r--r--   0      501       20     7253 2023-06-15 05:00:42.000000 pgpq-0.7.2/test_pgpq/test_pgpq.py
+-rw-r--r--   0        0        0     3444 1970-01-01 00:00:00.000000 pgpq-0.7.2/PKG-INFO
```

### Comparing `pgpq-0.7.1/local_dependencies/pgpq/Cargo.toml` & `pgpq-0.7.2/local_dependencies/pgpq/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pgpq"
-version = "0.7.1"
+version = "0.7.2"
 edition = "2021"
 description = "Encode Apache Arrow `RecordBatch`es to Postgres' native binary format"
 license = "MIT"
 readme = "README.md"
 exclude = ["/tests"]
 homepage = "https://github.com/adriangb/pgpq"
 repository = "https://github.com/adriangb/pgpq"
```

### Comparing `pgpq-0.7.1/local_dependencies/pgpq/benches/experiments.rs` & `pgpq-0.7.2/local_dependencies/pgpq/benches/experiments.rs`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.1/local_dependencies/pgpq/benches/yellow_cab_dataset.rs` & `pgpq-0.7.2/local_dependencies/pgpq/benches/yellow_cab_dataset.rs`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.1/local_dependencies/pgpq/src/encoders.rs` & `pgpq-0.7.2/local_dependencies/pgpq/src/encoders.rs`

 * *Files 2% similar despite different names*

```diff
@@ -432,36 +432,46 @@
 type BinaryEncoder<'a> = GenericBinaryEncoder<'a, i32>;
 type LargeBinaryEncoder<'a> = GenericBinaryEncoder<'a, i64>;
 
 #[derive(Debug)]
 pub struct GenericStringEncoder<'a, T: OffsetSizeTrait> {
     arr: &'a arrow_array::GenericStringArray<T>,
     field: String,
+    output: StringOutputType,
 }
 
 impl<'a, T: OffsetSizeTrait> Encode for GenericStringEncoder<'a, T> {
     fn encode(&self, row: usize, buf: &mut BytesMut) -> Result<(), ErrorKind> {
         if self.arr.is_null(row) {
             buf.put_i32(-1);
         } else {
             let v = self.arr.value(row).as_bytes();
-            let len = v.len();
+            let mut len = v.len();
+            if matches!(self.output, StringOutputType::Jsonb) {
+                len += 1;
+            }
             match i32::try_from(len) {
                 Ok(l) => buf.put_i32(l),
                 Err(_) => return Err(ErrorKind::field_too_large(&self.field, len)),
             }
+            if matches!(self.output, StringOutputType::Jsonb) {
+                buf.put_u8(1) // JSONB format version
+            }
             buf.extend_from_slice(v);
         }
         Ok(())
     }
     fn size_hint(&self) -> Result<usize, ErrorKind> {
         let mut total = 0;
         for row in 0..self.arr.len() {
             total += self.arr.value(row).len();
         }
+        if matches!(self.output, StringOutputType::Jsonb) {
+            total += self.arr.len() // For JSONB format version
+        }
         Ok(total)
     }
 }
 
 type StringEncoder<'a> = GenericStringEncoder<'a, i32>;
 type LargeStringEncoder<'a> = GenericStringEncoder<'a, i64>;
 
@@ -639,63 +649,14 @@
             fn field(&self) -> Field {
                 self.field.clone()
             }
         }
     };
 }
 
-macro_rules! impl_encoder_builder_with_variable_output {
-    ($struct_name:ident, $enum_name:expr, $encoder_name:ident, $pg_data_type:expr, $allowed_pg_data_types:expr, $check_data_type:expr) => {
-        impl $struct_name {
-            pub fn new(field: Field) -> Result<Self, ErrorKind> {
-                if !$check_data_type(field.data_type()) {
-                    return Err(ErrorKind::FieldTypeNotSupported {
-                        encoder: stringify!($struct_name).to_string(),
-                        tp: field.data_type().clone(),
-                        field: field.name().clone(),
-                    });
-                }
-                Ok(Self {
-                    field,
-                    output: $pg_data_type,
-                })
-            }
-            pub fn new_with_output(field: Field, output: PostgresType) -> Result<Self, ErrorKind> {
-                if !$allowed_pg_data_types.contains(&output) {
-                    return Err(ErrorKind::unsupported_encoding(
-                        &field.name(),
-                        &output,
-                        &[PostgresType::Text, PostgresType::Jsonb],
-                    ));
-                }
-                Ok(Self { field, output })
-            }
-        }
-        impl BuildEncoder for $struct_name {
-            fn try_new<'a, 'b: 'a>(&'b self, arr: &'a dyn Array) -> Result<Encoder<'a>, ErrorKind> {
-                let field = self.field.name();
-                let arr = downcast_checked(arr, &field)?;
-                Ok($enum_name($encoder_name {
-                    field: self.field.name().clone(),
-                    arr,
-                }))
-            }
-            fn schema(&self) -> Column {
-                Column {
-                    data_type: self.output.clone(),
-                    nullable: self.field.is_nullable(),
-                }
-            }
-            fn field(&self) -> Field {
-                self.field.clone()
-            }
-        }
-    };
-}
-
 #[derive(Debug, Clone, PartialEq)]
 pub struct BooleanEncoderBuilder {
     field: Field,
 }
 impl_encoder_builder_stateless!(
     BooleanEncoderBuilder,
     Encoder::Boolean,
@@ -955,38 +916,108 @@
     Encoder::DurationSecond,
     DurationSecondEncoder,
     PostgresType::Interval,
     |dt: &DataType| matches!(dt, DataType::Duration(TimeUnit::Second))
 );
 
 #[derive(Debug, Clone, PartialEq)]
+enum StringOutputType {
+    Text,
+    Json,
+    Jsonb,
+}
+
+impl StringOutputType {
+    pub fn from_postgres_type(tp: PostgresType, field: &Field) -> Result<Self, ErrorKind> {
+        match tp {
+            PostgresType::Text => Ok(StringOutputType::Text),
+            PostgresType::Json => Ok(StringOutputType::Json),
+            PostgresType::Jsonb => Ok(StringOutputType::Jsonb),
+            other => Err(ErrorKind::EncodingNotSupported {
+                field: field.name().clone(),
+                tp: other,
+                allowed: vec![PostgresType::Text, PostgresType::Json, PostgresType::Jsonb],
+            }),
+        }
+    }
+    pub fn postgres_datatype(&self) -> PostgresType {
+        match self {
+            StringOutputType::Text => PostgresType::Text,
+            StringOutputType::Json => PostgresType::Json,
+            StringOutputType::Jsonb => PostgresType::Jsonb,
+        }
+    }
+}
+
+macro_rules! impl_encoder_builder_with_variable_output {
+    ($struct_name:ident, $enum_name:expr, $encoder_name:ident, $check_data_type:expr) => {
+        impl $struct_name {
+            pub fn new(field: Field) -> Result<Self, ErrorKind> {
+                if !$check_data_type(field.data_type()) {
+                    return Err(ErrorKind::FieldTypeNotSupported {
+                        encoder: stringify!($struct_name).to_string(),
+                        tp: field.data_type().clone(),
+                        field: field.name().clone(),
+                    });
+                }
+                Ok(Self {
+                    field,
+                    output: StringOutputType::Text,
+                })
+            }
+            pub fn new_with_output(field: Field, output: PostgresType) -> Result<Self, ErrorKind> {
+                let output = StringOutputType::from_postgres_type(output, &field)?;
+                Ok(Self { field, output })
+            }
+        }
+        impl BuildEncoder for $struct_name {
+            fn try_new<'a, 'b: 'a>(&'b self, arr: &'a dyn Array) -> Result<Encoder<'a>, ErrorKind> {
+                let field = self.field.name();
+                let arr = downcast_checked(arr, &field)?;
+                Ok($enum_name($encoder_name {
+                    field: self.field.name().clone(),
+                    arr,
+                    output: self.output.clone(),
+                }))
+            }
+            fn schema(&self) -> Column {
+                Column {
+                    data_type: self.output.postgres_datatype().clone(),
+                    nullable: self.field.is_nullable(),
+                }
+            }
+            fn field(&self) -> Field {
+                self.field.clone()
+            }
+        }
+    };
+}
+
+#[derive(Debug, Clone, PartialEq)]
 pub struct StringEncoderBuilder {
     field: Field,
-    output: PostgresType,
+    output: StringOutputType,
 }
 impl_encoder_builder_with_variable_output!(
     StringEncoderBuilder,
     Encoder::String,
     StringEncoder,
-    PostgresType::Text,
-    vec![PostgresType::Text, PostgresType::Jsonb],
     |dt: &DataType| matches!(dt, DataType::Utf8)
 );
 
 #[derive(Debug, Clone, PartialEq)]
 pub struct LargeStringEncoderBuilder {
     field: Field,
-    output: PostgresType,
+    output: StringOutputType,
 }
+
 impl_encoder_builder_with_variable_output!(
     LargeStringEncoderBuilder,
     Encoder::LargeString,
     LargeStringEncoder,
-    PostgresType::Text,
-    vec![PostgresType::Text, PostgresType::Jsonb],
     |dt: &DataType| matches!(dt, DataType::LargeUtf8)
 );
 
 #[derive(Debug, Clone, PartialEq)]
 pub struct BinaryEncoderBuilder {
     field: Field,
 }
@@ -1194,19 +1225,19 @@
                 TimeUnit::Millisecond => {
                     Self::DurationMillisecond(DurationMillisecondEncoderBuilder { field })
                 }
                 TimeUnit::Second => Self::DurationSecond(DurationSecondEncoderBuilder { field }),
             },
             DataType::Utf8 => Self::String(StringEncoderBuilder {
                 field,
-                output: PostgresType::Text,
+                output: StringOutputType::Text,
             }),
             DataType::LargeUtf8 => Self::LargeString(LargeStringEncoderBuilder {
                 field,
-                output: PostgresType::Text,
+                output: StringOutputType::Text,
             }),
             DataType::Binary => Self::Binary(BinaryEncoderBuilder { field }),
             DataType::LargeBinary | DataType::FixedSizeBinary(_) => {
                 Self::LargeBinary(LargeBinaryEncoderBuilder { field })
             }
             DataType::List(inner) => {
                 if matches!(
```

### Comparing `pgpq-0.7.1/local_dependencies/pgpq/src/error.rs` & `pgpq-0.7.2/local_dependencies/pgpq/src/error.rs`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.1/local_dependencies/pgpq/src/lib.rs` & `pgpq-0.7.2/local_dependencies/pgpq/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.1/local_dependencies/pgpq/src/pg_schema.rs` & `pgpq-0.7.2/local_dependencies/pgpq/src/pg_schema.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Bool,
     Bytea,
     Int8,
     Int2,
     Int4,
     Char,
     Text,
+    Json,
     Jsonb,
     Float4,
     Float8,
     Date,
     Time,
     Timestamp,
     Interval,
@@ -29,14 +30,15 @@
             PostgresType::Bool => TypeSize::Fixed(1),
             PostgresType::Bytea => TypeSize::Variable,
             PostgresType::Int2 => TypeSize::Fixed(2),
             PostgresType::Int4 => TypeSize::Fixed(4),
             PostgresType::Int8 => TypeSize::Fixed(8),
             PostgresType::Char => TypeSize::Fixed(2),
             PostgresType::Text => TypeSize::Variable,
+            PostgresType::Json => TypeSize::Variable,
             PostgresType::Jsonb => TypeSize::Variable,
             PostgresType::Float4 => TypeSize::Fixed(4),
             PostgresType::Float8 => TypeSize::Fixed(8),
             PostgresType::Date => TypeSize::Fixed(4),
             PostgresType::Time => TypeSize::Fixed(8),
             PostgresType::Timestamp => TypeSize::Fixed(8),
             PostgresType::Interval => TypeSize::Fixed(16),
@@ -48,14 +50,15 @@
             PostgresType::Bool => Some(16),
             PostgresType::Bytea => Some(17),
             PostgresType::Int8 => Some(20),
             PostgresType::Int2 => Some(21),
             PostgresType::Int4 => Some(23),
             PostgresType::Char => Some(18),
             PostgresType::Text => Some(25),
+            PostgresType::Json => Some(3802),
             PostgresType::Jsonb => Some(3802),
             PostgresType::Float4 => Some(700),
             PostgresType::Float8 => Some(701),
             PostgresType::Date => Some(1082),
             PostgresType::Time => Some(1083),
             PostgresType::Timestamp => Some(1114),
             PostgresType::Interval => Some(1186),
@@ -67,14 +70,15 @@
             PostgresType::Bool => "BOOL".to_string(),
             PostgresType::Bytea => "BYTEA".to_string(),
             PostgresType::Int8 => "INT8".to_string(),
             PostgresType::Int2 => "INT2".to_string(),
             PostgresType::Int4 => "INT4".to_string(),
             PostgresType::Char => "CHAR".to_string(),
             PostgresType::Text => "TEXT".to_string(),
+            PostgresType::Json => "JSON".to_string(),
             PostgresType::Jsonb => "JSONB".to_string(),
             PostgresType::Float4 => "FLOAT4".to_string(),
             PostgresType::Float8 => "FLOAT8".to_string(),
             PostgresType::Date => "DATE".to_string(),
             PostgresType::Time => "TIME".to_string(),
             PostgresType::Timestamp => "TIMESTAMP".to_string(),
             PostgresType::Interval => "INTERVAL".to_string(),
```

### Comparing `pgpq-0.7.1/README.md` & `pgpq-0.7.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,51 @@
 # pgpq
 
 Convert PyArrow RecordBatches to Postgres' native binary format.
 
 ## Usage
 
 ```python
+"""Example for README.md"""
+from tempfile import mkdtemp
 import psycopg
 import pyarrow.dataset as ds
+import requests
 from pgpq import ArrowToPostgresBinaryEncoder
 
+# let's get some example data
+tmpdir = mkdtemp()
+with open(f"{tmpdir}/yellow_tripdata_2023-01.parquet", mode="wb") as f:
+    resp = requests.get(
+        "https://d37ci6vzurychx.cloudfront.net/trip-data/yellow_tripdata_2023-01.parquet"
+    )
+    resp.raise_for_status()
+    f.write(resp.content)
+
+# load an arrow dataset
+# arrow can load datasets from partitioned parquet files locally or in S3/GCS
+# it handles buffering, matching globs, etc.
+dataset = ds.dataset(tmpdir)
 
-dataset = ds.dataset("tests/testdata/")
-
+# create an encoder object which will do the encoding
+# and give us the expected Postgres table schema
 encoder = ArrowToPostgresBinaryEncoder(dataset.schema)
-# get the expected postgres destination schema
+# get the expected Postgres destination schema
 # note that this is _not_ the same as the incoming arrow schema
 # and not necessarily the schema of your permanent table
 # instead it's the schema of the data that will be sent over the wire
 # which for example does not have timezones on any timestamps
 pg_schema = encoder.schema()
 # assemble ddl for a temporary table
 # it's often a good idea to bulk load into a temp table to:
 # (1) Avoid indexes
 # (2) Stay in-memory as long as possible
-# (3) Be more flexible with types (you can't load a SMALLINT into a BIGINT column without casting)
-cols = [f"\"{col['name']}\" {col['data_type']['ddl']}" for col in pg_schema["columns"]]
+# (3) Be more flexible with types
+#     (you can't load a SMALLINT into a BIGINT column without casting)
+cols = [f'"{col_name}" {col.data_type.ddl()}' for col_name, col in pg_schema.columns]
 ddl = f"CREATE TEMP TABLE data ({','.join(cols)})"
 
 with psycopg.connect("postgres://postgres:postgres@localhost:5432/postgres") as conn:
     with conn.cursor() as cursor:
         cursor.execute(ddl)  # type: ignore
         with cursor.copy("COPY data FROM STDIN WITH (FORMAT BINARY)") as copy:
             copy.write(encoder.write_header())
```

### Comparing `pgpq-0.7.1/benches/encode.ipynb` & `pgpq-0.7.2/benches/encode.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9868055555555555%*

 * *Differences: {"'cells'": "{0: {'execution_count': 2}, 1: {'execution_count': 3}, 2: {'execution_count': 4}, 3: "*

 * *            "{'execution_count': 5}, 4: {'execution_count': 6, 'outputs': {0: {'text': ['803 ms ± "*

 * *            "5.25 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)\\n']}}}, 5: "*

 * *            "{'execution_count': 7, 'outputs': {0: {'text': ['0.3498361110687256\\n']}}}}"}*

```diff
@@ -1,22 +1,22 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 25,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import pyarrow.parquet as pq\n",
                 "from pgpq import ArrowToPostgresBinaryEncoder"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from pathlib import Path\n",
                 "import requests\n",
                 "\n",
                 "file = Path(\".\").resolve().parent.parent / \"yellow_tripdata_2022-01.parquet\"\n",
@@ -26,15 +26,15 @@
                 "        with file.open(\"wb\") as f:\n",
                 "            for chunk in r.iter_content(chunk_size=1024 * 1024):\n",
                 "                f.write(chunk)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 27,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [],
             "source": [
                 "arrow_table = pq.read_table(file)\n",
                 "\n",
                 "batches = arrow_table.to_batches()\n",
                 "small_batches = batches[:100]\n",
@@ -48,53 +48,53 @@
                 "            yield batch\n",
                 "            if total > 1_000_000:\n",
                 "                return"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 28,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def encode(batches) -> None:\n",
                 "    encoder = ArrowToPostgresBinaryEncoder(arrow_table.schema)\n",
                 "    encoder.write_header()\n",
                 "    for batch in batches:\n",
                 "        encoder.write_batch(batch)\n",
                 "    encoder.finish()\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 29,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "778 ms \u00b1 6.68 ms per loop (mean \u00b1 std. dev. of 7 runs, 1 loop each)\n"
+                        "803 ms \u00b1 5.25 ms per loop (mean \u00b1 std. dev. of 7 runs, 1 loop each)\n"
                     ]
                 }
             ],
             "source": [
                 "%timeit encode(small_batches)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 30,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "0.3342421054840088\n"
+                        "0.3498361110687256\n"
                     ]
                 }
             ],
             "source": [
                 "from time import time\n",
                 "\n",
                 "start = time()\n",
```

### Comparing `pgpq-0.7.1/example.py` & `pgpq-0.7.2/example.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,53 @@
 """Example for README.md"""
+from shutil import rmtree
+from tempfile import mkdtemp
 import psycopg
 import pyarrow.dataset as ds
+import requests
 from pgpq import ArrowToPostgresBinaryEncoder
 
 
-dataset = ds.dataset("tests/testdata/")
+# let's get some example data
+tmpdir = mkdtemp()
+with open(f"{tmpdir}/yellow_tripdata_2023-01.parquet", mode="wb") as f:
+    resp = requests.get(
+        "https://d37ci6vzurychx.cloudfront.net/trip-data/yellow_tripdata_2023-01.parquet"
+    )
+    resp.raise_for_status()
+    f.write(resp.content)
 
+# load an arrow dataset
+# arrow can load datasets from partitioned parquet files locally or in S3/GCS
+# it handles buffering, matching globs, etc.
+dataset = ds.dataset(tmpdir)
+
+# create an encoder object which will do the encoding
+# and give us the expected Postgres table schema
 encoder = ArrowToPostgresBinaryEncoder(dataset.schema)
-# get the expected postgres destination schema
+# get the expected Postgres destination schema
 # note that this is _not_ the same as the incoming arrow schema
 # and not necessarily the schema of your permanent table
 # instead it's the schema of the data that will be sent over the wire
 # which for example does not have timezones on any timestamps
 pg_schema = encoder.schema()
 # assemble ddl for a temporary table
 # it's often a good idea to bulk load into a temp table to:
 # (1) Avoid indexes
 # (2) Stay in-memory as long as possible
-# (3) Be more flexible with types (you can't load a SMALLINT into a BIGINT col)
-cols = [f"\"{col['name']}\" {col['data_type']['ddl']}" for col in pg_schema["columns"]]
+# (3) Be more flexible with types
+#     (you can't load a SMALLINT into a BIGINT column without casting)
+cols = [f'"{col_name}" {col.data_type.ddl()}' for col_name, col in pg_schema.columns]
 ddl = f"CREATE TEMP TABLE data ({','.join(cols)})"
 
 with psycopg.connect("postgres://postgres:postgres@localhost:5432/postgres") as conn:
     with conn.cursor() as cursor:
         cursor.execute(ddl)  # type: ignore
         with cursor.copy("COPY data FROM STDIN WITH (FORMAT BINARY)") as copy:
             copy.write(encoder.write_header())
             for batch in dataset.to_batches():
                 copy.write(encoder.write_batch(batch))
             copy.write(encoder.finish())
         # load into your actual table, possibly doing type casts
         # cursor.execute("INSERT INTO \"table\" SELECT * FROM data")
+
+rmtree(tmpdir)
```

### Comparing `pgpq-0.7.1/pyproject.toml` & `pgpq-0.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 [project.urls]
 homepage = "https://github.com/adriangb/pgpq"
 documentation = "https://github.com/adriangb/pgpq/README.md"
 repository = "https://github.com/adriangb/pgpq"
 
 [build-system]
-requires = ["maturin>=0.14.6<15"]
+requires = ["maturin>=0.14.0,<15"]
 build-backend = "maturin"
 
 [tool.maturin]
 sdist-include = ["Cargo.lock"]
 strip = true
 python-source = "python"
 profile = "release"
```

### Comparing `pgpq-0.7.1/python/pgpq/_pgpq.pyi` & `pgpq-0.7.2/python/pgpq/_pgpq.pyi`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.1/python/pgpq/encoders.py` & `pgpq-0.7.2/python/pgpq/encoders.py`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.1/python/pgpq/schema.py` & `pgpq-0.7.2/python/pgpq/schema.py`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.1/src/encoders.rs` & `pgpq-0.7.2/src/encoders.rs`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.1/src/lib.rs` & `pgpq-0.7.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.1/src/pg_schema.rs` & `pgpq-0.7.2/src/pg_schema.rs`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,19 @@
 #[pyclass(module = "pgpq._pgpq")]
 #[derive(Debug, Clone, PartialEq)]
 pub struct Text;
 impl_simple!(Text, pgpq::pg_schema::PostgresType::Text);
 
 #[pyclass(module = "pgpq._pgpq")]
 #[derive(Debug, Clone, PartialEq)]
+pub struct Json;
+impl_simple!(Json, pgpq::pg_schema::PostgresType::Json);
+
+#[pyclass(module = "pgpq._pgpq")]
+#[derive(Debug, Clone, PartialEq)]
 pub struct Jsonb;
 impl_simple!(Jsonb, pgpq::pg_schema::PostgresType::Jsonb);
 
 #[pyclass(module = "pgpq._pgpq")]
 #[derive(Debug, Clone, PartialEq)]
 pub struct Float4;
 impl_simple!(Float4, pgpq::pg_schema::PostgresType::Float4);
@@ -168,14 +173,15 @@
     Bool(Bool),
     Bytea(Bytea),
     Int2(Int2),
     Int4(Int4),
     Int8(Int8),
     Char(Char),
     Text(Text),
+    Json(Json),
     Jsonb(Jsonb),
     Float4(Float4),
     Float8(Float8),
     Date(Date),
     Time(Time),
     Timestamp(Timestamp),
     Interval(Interval),
@@ -188,14 +194,15 @@
             PostgresType::Bool(inner) => inner.into(),
             PostgresType::Bytea(inner) => inner.into(),
             PostgresType::Int2(inner) => inner.into(),
             PostgresType::Int4(inner) => inner.into(),
             PostgresType::Int8(inner) => inner.into(),
             PostgresType::Char(inner) => inner.into(),
             PostgresType::Text(inner) => inner.into(),
+            PostgresType::Json(inner) => inner.into(),
             PostgresType::Jsonb(inner) => inner.into(),
             PostgresType::Float4(inner) => inner.into(),
             PostgresType::Float8(inner) => inner.into(),
             PostgresType::Date(inner) => inner.into(),
             PostgresType::Time(inner) => inner.into(),
             PostgresType::Timestamp(inner) => inner.into(),
             PostgresType::Interval(inner) => inner.into(),
@@ -210,14 +217,15 @@
             pgpq::pg_schema::PostgresType::Bool => PostgresType::Bool(Bool),
             pgpq::pg_schema::PostgresType::Bytea => PostgresType::Bytea(Bytea),
             pgpq::pg_schema::PostgresType::Int2 => PostgresType::Int2(Int2),
             pgpq::pg_schema::PostgresType::Int4 => PostgresType::Int4(Int4),
             pgpq::pg_schema::PostgresType::Int8 => PostgresType::Int8(Int8),
             pgpq::pg_schema::PostgresType::Char => PostgresType::Char(Char),
             pgpq::pg_schema::PostgresType::Text => PostgresType::Text(Text),
+            pgpq::pg_schema::PostgresType::Json => PostgresType::Json(Json),
             pgpq::pg_schema::PostgresType::Jsonb => PostgresType::Jsonb(Jsonb),
             pgpq::pg_schema::PostgresType::Float4 => PostgresType::Float4(Float4),
             pgpq::pg_schema::PostgresType::Float8 => PostgresType::Float8(Float8),
             pgpq::pg_schema::PostgresType::Date => PostgresType::Date(Date),
             pgpq::pg_schema::PostgresType::Time => PostgresType::Time(Time),
             pgpq::pg_schema::PostgresType::Timestamp => PostgresType::Timestamp(Timestamp),
             pgpq::pg_schema::PostgresType::Interval => PostgresType::Interval(Interval),
@@ -234,14 +242,15 @@
             PostgresType::Bool(inner) => inner.py_repr(py),
             PostgresType::Bytea(inner) => inner.py_repr(py),
             PostgresType::Int2(inner) => inner.py_repr(py),
             PostgresType::Int4(inner) => inner.py_repr(py),
             PostgresType::Int8(inner) => inner.py_repr(py),
             PostgresType::Char(inner) => inner.py_repr(py),
             PostgresType::Text(inner) => inner.py_repr(py),
+            PostgresType::Json(inner) => inner.py_repr(py),
             PostgresType::Jsonb(inner) => inner.py_repr(py),
             PostgresType::Float4(inner) => inner.py_repr(py),
             PostgresType::Float8(inner) => inner.py_repr(py),
             PostgresType::Date(inner) => inner.py_repr(py),
             PostgresType::Time(inner) => inner.py_repr(py),
             PostgresType::Timestamp(inner) => inner.py_repr(py),
             PostgresType::Interval(inner) => inner.py_repr(py),
@@ -273,14 +282,15 @@
             PostgresType::Bool(inner) => inner.clone().into_py(py),
             PostgresType::Bytea(inner) => inner.clone().into_py(py),
             PostgresType::Int2(inner) => inner.clone().into_py(py),
             PostgresType::Int4(inner) => inner.clone().into_py(py),
             PostgresType::Int8(inner) => inner.clone().into_py(py),
             PostgresType::Char(inner) => inner.clone().into_py(py),
             PostgresType::Text(inner) => inner.clone().into_py(py),
+            PostgresType::Json(inner) => inner.clone().into_py(py),
             PostgresType::Jsonb(inner) => inner.clone().into_py(py),
             PostgresType::Float4(inner) => inner.clone().into_py(py),
             PostgresType::Float8(inner) => inner.clone().into_py(py),
             PostgresType::Date(inner) => inner.clone().into_py(py),
             PostgresType::Time(inner) => inner.clone().into_py(py),
             PostgresType::Timestamp(inner) => inner.clone().into_py(py),
             PostgresType::Interval(inner) => inner.clone().into_py(py),
```

### Comparing `pgpq-0.7.1/src/template.py` & `pgpq-0.7.2/src/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     "Bool",
     "Bytea",
     "Int8",
     "Int2",
     "Int4",
     "Char",
     "Text",
+    "Json",
     "Jsonb",
     "Float4",
     "Float8",
     "Date",
     "Time",
     "Timestamp",
     "Interval",
```

### Comparing `pgpq-0.7.1/test_pgpq/test_pgpq.py` & `pgpq-0.7.2/test_pgpq/test_pgpq.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,22 +212,22 @@
         ),
     )
 
     encoders = {
         "json_list": pgpq.encoders.ListEncoderBuilder.new_with_inner(
             batch.schema.field("json_list"),
             pgpq.encoders.StringEncoderBuilder.new_with_output(
-                batch.schema.field("json_list").type.value_field, pgpq.schema.Text()
+                batch.schema.field("json_list").type.value_field, pgpq.schema.Jsonb()
             ),
         )
     }
 
     encoder = ArrowToPostgresBinaryEncoder.new_with_encoders(batch.schema, encoders)
     buffer = bytearray()
     buffer.extend(encoder.write_header())
     buffer.extend(encoder.write_batch(batch))
     buffer.extend(encoder.finish())
 
     pg_schema = encoder.schema()
 
     rows = copy_buffer_and_get_rows(pg_schema, buffer, dbconn)
-    print(rows)
+    assert rows == [([[]],), ([{"foo": "bar"}],), ([123],)]
```

### Comparing `pgpq-0.7.1/PKG-INFO` & `pgpq-0.7.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgpq
-Version: 0.7.1
+Version: 0.7.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: pyarrow>=11
@@ -20,45 +20,62 @@
 Provides-Extra: bench
 Provides-Extra: test
 Summary: Arrow -> PostgreSQL encoder
 Author: Adrian Garcia Badaracco
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: documentation, https://github.com/adriangb/pgpq/README.md
 Project-URL: homepage, https://github.com/adriangb/pgpq
+Project-URL: documentation, https://github.com/adriangb/pgpq/README.md
 Project-URL: repository, https://github.com/adriangb/pgpq
 
 # pgpq
 
 Convert PyArrow RecordBatches to Postgres' native binary format.
 
 ## Usage
 
 ```python
+"""Example for README.md"""
+from tempfile import mkdtemp
 import psycopg
 import pyarrow.dataset as ds
+import requests
 from pgpq import ArrowToPostgresBinaryEncoder
 
+# let's get some example data
+tmpdir = mkdtemp()
+with open(f"{tmpdir}/yellow_tripdata_2023-01.parquet", mode="wb") as f:
+    resp = requests.get(
+        "https://d37ci6vzurychx.cloudfront.net/trip-data/yellow_tripdata_2023-01.parquet"
+    )
+    resp.raise_for_status()
+    f.write(resp.content)
+
+# load an arrow dataset
+# arrow can load datasets from partitioned parquet files locally or in S3/GCS
+# it handles buffering, matching globs, etc.
+dataset = ds.dataset(tmpdir)
 
-dataset = ds.dataset("tests/testdata/")
-
+# create an encoder object which will do the encoding
+# and give us the expected Postgres table schema
 encoder = ArrowToPostgresBinaryEncoder(dataset.schema)
-# get the expected postgres destination schema
+# get the expected Postgres destination schema
 # note that this is _not_ the same as the incoming arrow schema
 # and not necessarily the schema of your permanent table
 # instead it's the schema of the data that will be sent over the wire
 # which for example does not have timezones on any timestamps
 pg_schema = encoder.schema()
 # assemble ddl for a temporary table
 # it's often a good idea to bulk load into a temp table to:
 # (1) Avoid indexes
 # (2) Stay in-memory as long as possible
-# (3) Be more flexible with types (you can't load a SMALLINT into a BIGINT column without casting)
-cols = [f"\"{col['name']}\" {col['data_type']['ddl']}" for col in pg_schema["columns"]]
+# (3) Be more flexible with types
+#     (you can't load a SMALLINT into a BIGINT column without casting)
+cols = [f'"{col_name}" {col.data_type.ddl()}' for col_name, col in pg_schema.columns]
 ddl = f"CREATE TEMP TABLE data ({','.join(cols)})"
 
 with psycopg.connect("postgres://postgres:postgres@localhost:5432/postgres") as conn:
     with conn.cursor() as cursor:
         cursor.execute(ddl)  # type: ignore
         with cursor.copy("COPY data FROM STDIN WITH (FORMAT BINARY)") as copy:
             copy.write(encoder.write_header())
```

