# Comparing `tmp/bmsdna_lakeapi-0.8.3.tar.gz` & `tmp/bmsdna_lakeapi-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.8.3.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.8.4.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.8.3.tar` & `bmsdna_lakeapi-0.8.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1081 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/LICENSE
--rw-r--r--   0        0        0     8929 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/README.md
--rw-r--r--   0        0        0      337 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1138 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      566 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     6965 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0    10460 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     6042 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    11027 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    12557 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/dataframe.py
--rw-r--r--   0        0        0     7443 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/detail_endpoint.py
--rw-r--r--   0        0        0     9751 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6887 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     1479 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/partition_utils.py
--rw-r--r--   0        0        0     6763 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     4319 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     3748 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/sql_endpoint.py
--rw-r--r--   0        0        0     3136 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2456 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1837 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      339 2023-06-14 07:23:35.807083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1784 2023-06-14 07:23:35.811083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1084 2023-06-14 07:23:35.811083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     3535 2023-06-14 07:23:35.811083 bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/utils/fast_api_utils.py
--rw-r--r--   0        0        0     2017 2023-06-14 07:23:35.811083 bmsdna_lakeapi-0.8.3/pyproject.toml
--rw-r--r--   0        0        0    10127 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/LICENSE
+-rw-r--r--   0        0        0     8929 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/README.md
+-rw-r--r--   0        0        0      337 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1138 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      625 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     7183 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0    10630 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     6255 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    11269 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    12557 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/dataframe.py
+-rw-r--r--   0        0        0     7474 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/detail_endpoint.py
+-rw-r--r--   0        0        0    10144 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6887 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     1479 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/partition_utils.py
+-rw-r--r--   0        0        0     6813 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     4437 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     3781 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/sql_endpoint.py
+-rw-r--r--   0        0        0     3136 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2456 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1837 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      339 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1784 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1084 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     3535 2023-06-15 08:07:04.220869 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/utils/fast_api_utils.py
+-rw-r--r--   0        0        0     2017 2023-06-15 08:07:04.220869 bmsdna_lakeapi-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0    10127 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.8.4/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.8.3/LICENSE` & `bmsdna_lakeapi-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.3/README.md` & `bmsdna_lakeapi-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/api/api.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/context/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from bmsdna.lakeapi.context.df_base import ExecutionContext
 from bmsdna.lakeapi.core.types import Engines
 
 
-def get_context_by_engine(engine: Engines) -> ExecutionContext:
+def get_context_by_engine(engine: Engines, chunk_size: int) -> ExecutionContext:
     match engine.lower():
         case "duckdb":
             from bmsdna.lakeapi.context.df_duckdb import DuckDbExecutionContext
 
-            return DuckDbExecutionContext()
+            return DuckDbExecutionContext(chunk_size=chunk_size)
         case "polars":
             from bmsdna.lakeapi.context.df_polars import PolarsExecutionContext
 
-            return PolarsExecutionContext()
+            return PolarsExecutionContext(chunk_size=chunk_size)
         case _:
             raise Exception(f"Unknown engine {engine}")
```

### Comparing `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/context/df_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,18 @@
         return sql_or_pypika
     if len(sql_or_pypika._selects) == 0:
         return sql_or_pypika.select("*").get_sql()
     return sql_or_pypika.get_sql()
 
 
 class ResultData(ABC):
+    def __init__(self, chunk_size: int) -> None:
+        super().__init__()
+        self.chunk_size = chunk_size
+
     @abstractmethod
     def columns(self) -> List[str]:
         ...
 
     @abstractmethod
     def arrow_schema(self) -> pa.Schema:
         ...
@@ -62,52 +66,53 @@
             t = pl.from_arrow(arrow_table)
             assert isinstance(t, pl.DataFrame)
             t.write_json(f, row_oriented=True)
 
     def write_nd_json(self, file_name: str):
         import polars as pl
 
-        batches = self.to_arrow_recordbatch()
+        batches = self.to_arrow_recordbatch(self.chunk_size)
         with open(file_name, mode="wb") as f:
             for batch in batches:
                 t = pl.from_arrow(batch)
                 assert isinstance(t, pl.DataFrame)
                 t.write_ndjson(f)
 
     @abstractmethod
     def to_pandas(self) -> "pd.DataFrame":
         ...
 
     def write_parquet(self, file_name: str):
         import pyarrow.parquet as paparquet
 
-        batches = self.to_arrow_recordbatch()
+        batches = self.to_arrow_recordbatch(self.chunk_size)
 
         with paparquet.ParquetWriter(file_name, batches.schema) as writer:
             for batch in batches:
                 writer.write_batch(batch)
 
     def write_csv(self, file_name: str, *, separator: str):
         import pyarrow.csv as pacsv
         import decimal
 
-        batches = self.to_arrow_recordbatch()
+        batches = self.to_arrow_recordbatch(self.chunk_size)
         with pacsv.CSVWriter(
             file_name,
             batches.schema,
             write_options=pacsv.WriteOptions(delimiter=separator),
         ) as writer:
             for batch in batches:
                 writer.write_batch(batch)
 
 
 class ExecutionContext(ABC):
-    def __init__(self) -> None:
+    def __init__(self, chunk_size: int) -> None:
         super().__init__()
         self.modified_dates: dict[str, datetime] = {}
+        self.chunk_size = chunk_size
 
     @abstractmethod
     def __enter__(self) -> "ExecutionContext":
         ...
 
     @abstractmethod
     def __exit__(self, *args, **kwargs):
```

### Comparing `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,17 @@
 
 
 class DuckDBResultData(ResultData):
     def __init__(
         self,
         original_sql: Union[pypika.queries.QueryBuilder, str],
         con: duckdb.DuckDBPyConnection,
+        chunk_size: int,
     ) -> None:
-        super().__init__()
+        super().__init__(chunk_size=chunk_size)
         self.original_sql = original_sql
         self.con = con
         self._arrow_schema = None
         self._df = None
 
     def columns(self):
         return self.arrow_schema().names
@@ -125,16 +126,16 @@
         sql = f"fts_main_{self.source_view}.match_bm25({self.field.get_sql()}, {search_txt}{field_or_not})"
         if self.alias is not None:
             sql += " AS " + self.alias
         return sql
 
 
 class DuckDbExecutionContextBase(ExecutionContext):
-    def __init__(self, con: duckdb.DuckDBPyConnection):
-        super().__init__()
+    def __init__(self, con: duckdb.DuckDBPyConnection, chunk_size: int):
+        super().__init__(chunk_size=chunk_size)
         self.con = con
         self.res_con = None
         self.persistance_file_name = None
 
     def register_arrow(self, name: str, ds: Union[pyarrow.dataset.Dataset, pyarrow.Table]):
         # self.con.from_arrow(ds).create_view(name, replace=True)
         self.con.register(name, ds)
@@ -147,16 +148,16 @@
         sql: Union[
             pypika.queries.QueryBuilder,
             str,
         ],
     ) -> DuckDBResultData:
         if self.persistance_file_name is not None:
             self.res_con = duckdb.connect(self.persistance_file_name, read_only=True)
-            return DuckDBResultData(sql, self.res_con)
-        return DuckDBResultData(sql, con=self.con)
+            return DuckDBResultData(sql, self.res_con, self.chunk_size)
+        return DuckDBResultData(sql, con=self.con, chunk_size=self.chunk_size)
 
     def search_score_function(
         self,
         source_view: str,
         search_text: str,
         search_config: SearchConfig,
         alias: Optional[str],
@@ -239,16 +240,16 @@
 
     def __exit__(self, *args, **kwargs):
         if self.res_con:
             self.res_con.__exit__(*args, **kwargs)
 
 
 class DuckDbExecutionContext(DuckDbExecutionContextBase):
-    def __init__(self):
-        super().__init__(duckdb.connect())
+    def __init__(self, chunk_size: int):
+        super().__init__(duckdb.connect(), chunk_size=chunk_size)
 
     def __enter__(self):
         super().__enter__()
         self.con.__enter__()
         self.con.execute("SET memory_limit='200MB'")
         self.con.execute("SET threads =2")
         self.con.execute("SET enable_object_cache=true")
```

### Comparing `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/context/df_polars.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 from uuid import uuid4
 
 if TYPE_CHECKING:
     import polars  # we want to lazy import in case we one day no longer rely on polars if only duckdb is needed
 
 
 class PolarsResultData(ResultData):
-    def __init__(self, df: "Union[polars.DataFrame, polars.LazyFrame]", sql_context: "polars.SQLContext"):
+    def __init__(
+        self, df: "Union[polars.DataFrame, polars.LazyFrame]", sql_context: "polars.SQLContext", chunk_size: int
+    ):
+        super().__init__(chunk_size=chunk_size)
         self.df = df
         self.random_name = "tbl_" + str(uuid4())
         self.registred_df = False
         self.sql_context = sql_context
 
     def columns(self):
         return self.df.columns
@@ -99,16 +102,16 @@
 
         if isinstance(self.df, pl.LazyFrame):
             self.df = self.df.collect(streaming=True)
         self.df.write_ndjson(file_name)
 
 
 class PolarsExecutionContext(ExecutionContext):
-    def __init__(self, sql_context: "Optional[polars.SQLContext]" = None):
-        super().__init__()
+    def __init__(self, chunk_size: int, sql_context: "Optional[polars.SQLContext]" = None):
+        super().__init__(chunk_size=chunk_size)
         import polars as pl
 
         self.sql_context = sql_context or pl.SQLContext()
 
     def register_arrow(self, name: str, ds: Union[pyarrow.dataset.Dataset, pyarrow.Table]):
         import polars as pl
 
@@ -134,15 +137,18 @@
         self.modified_dates[name] = self.get_modified_date(uri, file_type)
         match file_type:
             case "delta":
                 from bmsdna.lakeapi.polars_extensions.delta import scan_delta2
 
                 df = pl.scan_delta2(  # type: ignore
                     uri,
-                    pyarrow_options={"partitions": partitions, "parquet_read_options":{"coerce_int96_timestamp_unit": "us"}}
+                    pyarrow_options={
+                        "partitions": partitions,
+                        "parquet_read_options": {"coerce_int96_timestamp_unit": "us"},
+                    },
                 )
             case "parquet":
                 df = pl.scan_parquet(uri)
             case "arrow":
                 df = pl.scan_ipc(uri)
             case "avro":
                 df = cast(pl.LazyFrame, pl.read_avro(uri))
@@ -164,15 +170,15 @@
         ],
     ) -> PolarsResultData:
         import polars as pl
 
         df = self.sql_context.execute(get_sql(sql))
         if isinstance(df, pl.LazyFrame):
             df = df.collect()
-        return PolarsResultData(df, self.sql_context)
+        return PolarsResultData(df, self.sql_context, self.chunk_size)
 
     def list_tables(self) -> ResultData:
         return self.execute_sql("SHOW TABLES")
 
     def __enter__(self):
         return self
```

### Comparing `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,24 +35,26 @@
 @dataclass(frozen=True)
 class BasicConfig:
     enable_sql_endpoint: bool
     temp_folder_path: str
     data_path: str
     min_search_length: int
     default_engine: Engines
+    default_chunk_size: int
     prepare_sql_db_hook: "Callable[[ExecutionContext], Any] | None"
 
 
 def get_default_config():
     return BasicConfig(
         enable_sql_endpoint=os.getenv("ENABLE_SQL_ENDPOINT", "0") == "1",
         temp_folder_path=os.getenv("TEMP", "/tmp"),
         data_path=os.environ.get("DATA_PATH", "data"),
         min_search_length=3,
         default_engine="duckdb",
+        default_chunk_size=10000,
         prepare_sql_db_hook=None,
     )
 
 
 @dataclass
 class Filter:
     key: str
@@ -109,14 +111,15 @@
     api_method: Union[Literal["get", "post"], List[Literal["get", "post"]]] = "get"
     params: Optional[List[Union[Param, str]]] = None
     timestamp: Optional[datetime] = None
     cache_expiration_time_seconds: Optional[int] = CACHE_EXPIRATION_TIME_SECONDS
     allow_get_all_pages: Optional[bool] = False
     search: Optional[List[SearchConfig]] = None
     engine: Optional[Engines] = None
+    chunk_size: Optional[int] = None
 
     def __post_init__(self):
         self.version_str = (
             str(self.version) if str(self.version or 1).startswith("v") else "v" + str(self.version or 1)
         )
         self.route = "/api/" + self.version_str + "/" + self.tag + "/" + self.name
 
@@ -195,14 +198,15 @@
                         new_params = _with_implicit_parameters(_params, file_type, basic_config, datasource_obj.uri)
                         ls.append(
                             cls(
                                 name=it.name,
                                 tag=tag,
                                 version=version,
                                 engine=config.get("engine", None),
+                                chunk_size=config.get("chunk_size", None),
                                 api_method=api_method,
                                 search=search_config,
                                 params=new_params,  # type: ignore
                                 allow_get_all_pages=config.get("allow_get_all_pages", False),
                                 datasource=datasource_obj,
                                 cache_expiration_time_seconds=cache_expiration_time_seconds,
                             )
@@ -225,14 +229,15 @@
                 cls(
                     name=name,
                     tag=tag,
                     version=version,
                     search=search_config,
                     api_method=api_method,
                     engine=config.get("engine", None),
+                    chunk_size=config.get("chunk_size", None),
                     params=new_params,  # type: ignore
                     allow_get_all_pages=config.get("allow_get_all_pages", False),
                     datasource=datasource_obj,
                     cache_expiration_time_seconds=cache_expiration_time_seconds,
                 )
             ]
```

### Comparing `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/dataframe.py` & `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/detail_endpoint.py` & `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/detail_endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         jsonify_complex: bool = Query(title="jsonify_complex", include_in_schema=has_complex, default=False),
     ) -> MetadataDetailResult:
         import json
 
         req.state.lake_api_basic_config = basic_config
         from bmsdna.lakeapi.context.df_duckdb import DuckDbExecutionContext
 
-        with DuckDbExecutionContext() as context:
+        with DuckDbExecutionContext(basic_config.default_chunk_size) as context:
             realdataframe = Dataframe(
                 config.version_str, config.tag, config.name, config.datasource, context, basic_config=basic_config
             )
 
             if not realdataframe.file_exists():
                 raise HTTPException(404)
             partition_columns = []
```

### Comparing `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,23 @@
 
 
 def is_complex_type(schema: pa.Schema, col_name: str):
     f = schema.field(col_name)
     return pa.types.is_nested(f.type)
 
 
+def split_csv(csv_str: str) -> list[str]:
+    import csv
+
+    reader = csv.reader([csv_str], delimiter=",", quotechar='"')
+    for i in reader:
+        return i
+    raise ValueError("cannot happen")
+
+
 def create_config_endpoint(
     metamodel: Optional[ResultData],
     apimethod: Literal["get", "post"],
     config: Config,
     router: APIRouter,
     response_model: Type,
     basic_config: BasicConfig,
@@ -145,15 +154,15 @@
     ):  # type: ignore
         logger.info(f"{params.dict(exclude_unset=True) if params else None}Union[ ,  ]{request.url.path}")
 
         engine = engine or basic_config.default_engine
 
         logger.info(f"Engine: {engine}")
 
-        with get_context_by_engine(engine) as context:
+        with get_context_by_engine(engine, chunk_size=config.chunk_size or basic_config.default_chunk_size) as context:
             realdataframe = Dataframe(
                 config.version_str, config.tag, config.name, config.datasource, context, basic_config=basic_config
             )
             parts = await get_partitions(realdataframe, params, config)
             df = realdataframe.get_df(parts or None)
 
             expr = await get_params_filter_expr(df.columns(), config, params)
@@ -170,15 +179,17 @@
                     if k.lower() in search_dict and v is not None and len(v) >= basic_config.min_search_length
                 }
 
             import pypika
 
             columns = exclude_cols(df.columns())
             if select:
-                columns = [c for c in columns if c in select.split(",")]
+                columns = [
+                    c for c in columns if c in split_csv(select)
+                ]  # split , is a bit naive, we might want to support real CSV with quotes here
             if config.datasource.exclude and len(config.datasource.exclude) > 0:
                 columns = [c for c in columns if c not in config.datasource.exclude]
             if config.datasource.sortby and len(searches) == 0:
                 for s in config.datasource.sortby:
                     new_query = new_query.orderby(
                         s.by,
                         order=pypika.Order.desc if s.direction and s.direction.lower() == "desc" else pypika.Order.asc,
```

### Comparing `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/model.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/partition_utils.py` & `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/partition_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/response.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 def write_frame(
     url: URL, content: ResultData, format: OutputFormats, out: str, basic_config: BasicConfig
 ) -> list[str]:
     if format == OutputFormats.AVRO:
         import polars as pl
 
-        ds = pl.from_arrow(content.to_arrow_recordbatch())
+        ds = pl.from_arrow(content.to_arrow_recordbatch(content.chunk_size))
         assert isinstance(ds, pl.DataFrame)
         ds.write_avro(out)
     elif format == OutputFormats.CSV:
         content.write_csv(out, separator=",")
     elif format == OutputFormats.SEMI_CSV:
         content.write_csv(out, separator=";")
     elif format == OutputFormats.CSV4EXCEL:  # need to write sep=, on first line
@@ -103,24 +103,24 @@
         assert isinstance(ds, pl.DataFrame)
         ds.write_excel(out, autofit=True)
     elif format == OutputFormats.HTML:
         content.to_pandas().to_html(out, index=False)
 
     elif format == OutputFormats.XML:
         content.to_pandas().to_xml(out, index=False, parser="etree")
-    
+
     elif format == OutputFormats.ARROW_IPC:
-        with content.to_arrow_recordbatch() as batches:
+        with content.to_arrow_recordbatch(content.chunk_size) as batches:
             with pa.OSFile(out, "wb") as sink:
                 with pa.ipc.new_file(sink, batches.schema) as writer:
                     for batch in batches:
                         writer.write(batch)
 
     elif format == OutputFormats.ARROW_STREAM:
-        with content.to_arrow_recordbatch() as batches:
+        with content.to_arrow_recordbatch(content.chunk_size) as batches:
             with pa.OSFile(out, "wb") as sink:
                 with pa.ipc.new_stream(sink, batches.schema) as writer:
                     for batch in batches:
                         writer.write_batch(batch)
 
     elif format == OutputFormats.ND_JSON:
         content.write_nd_json(out)
```

### Comparing `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/route.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     from bmsdna.lakeapi.core.detail_endpoint import create_detailed_meta_endpoint
     from bmsdna.lakeapi.core.sql_endpoint import create_sql_endpoint
 
     all_lake_api_routers.append((basic_config, configs))
     router = APIRouter()
     metadata = []
 
-    with DuckDbExecutionContext() as context:
+    with DuckDbExecutionContext(basic_config.default_chunk_size) as context:
         for config in configs:
             methods = (
                 cast(list[Literal["get", "post"]], [config.api_method])
                 if isinstance(config.api_method, str)
                 else config.api_method
             )
             try:
@@ -101,11 +101,13 @@
                 if config.search:
                     from bmsdna.lakeapi.core.dataframe import Dataframe
 
                     realdataframe = Dataframe(
                         config.version_str, config.tag, config.name, config.datasource, context, basic_config
                     )
                     if realdataframe.file_exists():
-                        with get_context_by_engine(basic_config.default_engine) as ctx:
+                        with get_context_by_engine(
+                            basic_config.default_engine, basic_config.default_chunk_size
+                        ) as ctx:
                             ctx.init_search(realdataframe.tablename, config.search)
 
         return router
```

### Comparing `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/sql_endpoint.py` & `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/sql_endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         if df.file_exists():
             con.register_dataframe(df.tablename, df.uri, df.config.file_type, None)
 
 
 def get_sql_context(engine: Engines, basic_config: BasicConfig, configs: Configs):
     global sql_contexts
     if not engine in sql_contexts:
-        sql_contexts[engine] = get_context_by_engine(engine)
+        sql_contexts[engine] = get_context_by_engine(engine, basic_config.default_chunk_size)
         init_duck_con(sql_contexts[engine], basic_config, configs)
         if basic_config.prepare_sql_db_hook is not None:
             basic_config.prepare_sql_db_hook(sql_contexts[engine])
 
     return sql_contexts[engine]
```

### Comparing `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/uservalidation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/tools/useradd.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.3/bmsdna/lakeapi/utils/fast_api_utils.py` & `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/utils/fast_api_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.3/pyproject.toml` & `bmsdna_lakeapi-0.8.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.8.3"
+version = "0.8.4"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
```

### Comparing `bmsdna_lakeapi-0.8.3/PKG-INFO` & `bmsdna_lakeapi-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.8.3
+Version: 0.8.4
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

