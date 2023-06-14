# Comparing `tmp/grai_source_redshift-0.0.6.tar.gz` & `tmp/grai_source_redshift-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_redshift-0.0.6.tar", max compression
+gzip compressed data, was "grai_source_redshift-0.0.7.tar", max compression
```

## Comparing `grai_source_redshift-0.0.6.tar` & `grai_source_redshift-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0      141 2023-04-30 17:49:45.933526 grai_source_redshift-0.0.6/README.md
--rw-r--r--   0        0        0      970 2023-05-18 16:42:47.288134 grai_source_redshift-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      145 2023-04-25 21:23:43.339413 grai_source_redshift-0.0.6/src/grai_source_redshift/__init__.py
--rw-r--r--   0        0        0     6787 2023-05-18 17:19:35.536213 grai_source_redshift-0.0.6/src/grai_source_redshift/adapters.py
--rw-r--r--   0        0        0     1185 2023-04-25 21:23:43.339552 grai_source_redshift-0.0.6/src/grai_source_redshift/base.py
--rw-r--r--   0        0        0     7371 2023-05-18 17:17:34.029390 grai_source_redshift-0.0.6/src/grai_source_redshift/loader.py
--rw-r--r--   0        0        0     4369 2023-04-25 21:23:43.339688 grai_source_redshift-0.0.6/src/grai_source_redshift/models.py
--rw-r--r--   0        0        0      186 2023-04-25 21:23:43.339739 grai_source_redshift-0.0.6/src/grai_source_redshift/package_definitions.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 grai_source_redshift-0.0.6/setup.py
--rw-r--r--   0        0        0     1071 1970-01-01 00:00:00.000000 grai_source_redshift-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      141 2023-05-19 11:07:12.940719 grai_source_redshift-0.0.7/README.md
+-rw-r--r--   0        0        0     1066 2023-06-14 22:46:26.213086 grai_source_redshift-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-06-14 21:10:34.451009 grai_source_redshift-0.0.7/src/grai_source_redshift/__init__.py
+-rw-r--r--   0        0        0     8770 2023-06-14 22:10:38.520511 grai_source_redshift-0.0.7/src/grai_source_redshift/adapters.py
+-rw-r--r--   0        0        0     1749 2023-06-14 21:02:53.255449 grai_source_redshift-0.0.7/src/grai_source_redshift/base.py
+-rw-r--r--   0        0        0     8092 2023-06-14 21:02:53.295511 grai_source_redshift-0.0.7/src/grai_source_redshift/loader.py
+-rw-r--r--   0        0        0     5080 2023-06-01 16:01:43.268316 grai_source_redshift-0.0.7/src/grai_source_redshift/models.py
+-rw-r--r--   0        0        0      199 2023-06-01 16:01:43.268442 grai_source_redshift-0.0.7/src/grai_source_redshift/package_definitions.py
+-rw-r--r--   0        0        0     1117 1970-01-01 00:00:00.000000 grai_source_redshift-0.0.7/PKG-INFO
```

### Comparing `grai_source_redshift-0.0.6/pyproject.toml` & `grai_source_redshift-0.0.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "grai_source_redshift"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_redshift", from = "src" },
 ]
 readme = "README.md"
 homepage = "https://www.grai.io/"
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-redshift"
 documentation = "https://docs.grai.io/"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-grai-client = "^0.2.4"
+grai-client = "^0.2.18"
 multimethod = "^1.8"
-grai-schemas = "^0.1.5"
-redshift-connector = "^2.0.910"
+grai-schemas = "^0.1.15"
 pydantic = {extras = ["dotenv"], version = "^1.10.7"}
+botocore = "^1.29.153"
+redshift-connector = "^2.0.911"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
 mypy = "^0.971"
 isort = "^5.10.1"
 types-PyYAML = "^6.0.11"
 types-psycopg2 = "^2.9.18"
@@ -34,7 +35,9 @@
 
     [tool.black]
 line-length = 120
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry_bumpversion.file."src/grai_source_bigquery/__init__.py"]
```

### Comparing `grai_source_redshift-0.0.6/src/grai_source_redshift/base.py` & `grai_source_redshift-0.0.7/src/grai_source_redshift/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,14 +6,25 @@
 
 from grai_source_redshift.adapters import adapt_to_client
 from grai_source_redshift.loader import RedshiftConnector
 from grai_source_redshift.package_definitions import config
 
 
 def get_nodes_and_edges(connector: RedshiftConnector, version: Literal["v1"]) -> Tuple[List[Node], List[Edge]]:
+    """
+
+    Args:
+        connector (RedshiftConnector):
+        version (Literal["v1"]):
+
+    Returns:
+
+    Raises:
+
+    """
     with connector as conn:
         nodes, edges = conn.get_nodes_and_edges()
 
     nodes = adapt_to_client(nodes, version)
     edges = adapt_to_client(edges, version)
     return nodes, edges
 
@@ -23,14 +34,30 @@
     namespace: str,
     database: Optional[str] = None,
     user: Optional[str] = None,
     password: Optional[str] = None,
     host: Optional[str] = None,
     port: Optional[str] = None,
 ):
+    """
+
+    Args:
+        client (BaseClient):
+        namespace (str):
+        database (Optional[str], optional):  (Default value = None)
+        user (Optional[str], optional):  (Default value = None)
+        password (Optional[str], optional):  (Default value = None)
+        host (Optional[str], optional):  (Default value = None)
+        port (Optional[str], optional):  (Default value = None)
+
+    Returns:
+
+    Raises:
+
+    """
     conn = RedshiftConnector(
         database=database,
         user=user,
         password=password,
         host=host,
         port=port,
         namespace=namespace,
```

### Comparing `grai_source_redshift-0.0.6/src/grai_source_redshift/loader.py` & `grai_source_redshift-0.0.7/src/grai_source_redshift/loader.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,26 +14,32 @@
     EdgeQuery,
     RedshiftNode,
     Table,
 )
 
 
 class RedshiftConfig(BaseSettings):
+    """ """
+
     user: Optional[str] = None
     password: Optional[SecretStr] = None
     database: Optional[str] = None
     host: Optional[str] = None
     port: Optional[int] = None
 
     class Config:
+        """ """
+
         env_prefix = "grai_redshift_"
         env_file = ".env"
 
 
 class RedshiftConnector:
+    """ """
+
     def __init__(
         self,
         namespace: str,
         user: Optional[str] = None,
         password: Optional[str] = None,
         database: Optional[str] = None,
         host: Optional[str] = None,
@@ -61,46 +67,73 @@
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if not self._is_connected:
             self.close()
 
     def connect(self):
+        """ """
         conn_params = {k: v for k, v in self.config.dict().items() if v is not None}
         if "password" in conn_params:
             conn_params["password"] = conn_params["password"].get_secret_value()
 
         if self._connection is None:
             self._connection = redshift_connector.connect(**conn_params, **self.redshift_params)
             self._is_connected = True
         return self
 
     @property
     def connection(self):
+        """ """
         if self._connection is None:
             raise Exception("Not connected, call `.connect()")
         return self._connection
 
     def close(self) -> None:
+        """
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
         self.connection.close()
         self._connection = None
         self._is_connected = False
 
     def query_runner(self, query: str) -> List[Dict]:
+        """
+
+        Args:
+            query (str):
+
+        Returns:
+
+        Raises:
+
+        """
         cursor = self.connection.cursor()
         cursor.execute(query)
         columns = [column[0] for column in cursor.description]
         return [dict(zip(columns, item)) for item in cursor.fetchall()]
 
     @cached_property
     def tables(self) -> List[Table]:
-        """
-        Create and return a list of dictionaries with the
+        """Create and return a list of dictionaries with the
         schemas and names of tables in the database
         connected to by the connection argument.
+
+        Args:
+
+        Returns:
+
+        Raises:
+
         """
 
         query = """
             SELECT table_catalog, table_schema, table_name, table_type
             FROM information_schema.tables
             WHERE table_schema NOT IN ('pg_catalog', 'information_schema', 'pg_internal')
             ORDER BY table_schema, table_name
@@ -109,17 +142,23 @@
         tables = [Table(**result, namespace=self.namespace) for result in self.query_runner(query)]
         for table in tables:
             table.columns = self.get_table_columns(table)
         return tables
 
     @cached_property
     def columns(self) -> List[Column]:
-        """
-        Creates and returns a list of dictionaries for the specified
+        """Creates and returns a list of dictionaries for the specified
         schema.table in the database connected to.
+
+        Args:
+
+        Returns:
+
+        Raises:
+
         """
         query = f"""
             SELECT table_catalog,
                    table_schema AS column_schema,
                    table_name,
                    column_name,
                    column_default,
@@ -130,35 +169,58 @@
             FROM information_schema.columns
             WHERE table_schema NOT IN ('pg_catalog', 'information_schema', 'pg_internal')
             ORDER BY ordinal_position;
         """
         return [Column(**result, namespace=self.namespace) for result in self.query_runner(query)]
 
     def get_table_columns(self, table: Table):
+        """
+
+        Args:
+            table (Table):
+
+        Returns:
+
+        Raises:
+
+        """
         table_id = (table.table_schema, table.name)
         if table_id in self.column_map:
             return self.column_map[table_id]
         else:
             raise Exception(f"No columns found for table with schema={table.table_schema} and name={table.name}")
 
     @cached_property
     def column_map(self) -> Dict[Tuple[str, str], List[Column]]:
+        """
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
         result_map: Dict[Tuple[str, str], List[Column]] = {}
         for col in self.columns:
             table_id = (col.column_schema, col.table)
             result_map.setdefault(table_id, [])
             result_map[table_id].append(col)
         return result_map
 
     @cached_property
     def foreign_keys(self) -> List[Edge]:
         """This needs to be tested / evaluated
-        :param connection:
-        :param table:
-        :return:
+
+        Args:
+
+        Returns:
+
+        Raises:
+
         """
         # query is from https://alberton.info/postgresql_meta_info.html
         # detailed constraint info section
         query = """
             SELECT tc.constraint_name,
                    tc.constraint_type,
                    tc.table_catalog AS self_catalog,
@@ -186,17 +248,44 @@
         addtl_args = {"namespace": self.namespace}
         results = self.query_runner(query)
         filtered_results = (result for result in results if result["constraint_type"] == "FOREIGN KEY")
         result = [EdgeQuery(**fk, **addtl_args).to_edge() for fk in filtered_results]
         return [r for r in result if r is not None]
 
     def get_nodes(self) -> List[RedshiftNode]:
+        """
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
         return list(chain(self.tables, self.columns))
 
     def get_edges(self) -> List[Edge]:
+        """
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
         return list(chain(*[t.get_edges() for t in self.tables], self.foreign_keys))
 
     def get_nodes_and_edges(self) -> Tuple[List[RedshiftNode], List[Edge]]:
+        """
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
         nodes = self.get_nodes()
         edges = self.get_edges()
 
         return nodes, edges
```

### Comparing `grai_source_redshift-0.0.6/src/grai_source_redshift/models.py` & `grai_source_redshift-0.0.7/src/grai_source_redshift/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,127 +1,196 @@
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
 from pydantic import BaseModel, Field, root_validator, validator
 
 
 class RedshiftNode(BaseModel):
+    """ """
+
     pass
 
 
 class ID(RedshiftNode):
+    """ """
+
     name: str
     namespace: str
     full_name: str
 
     class Config:
+        """ """
+
         extra = "forbid"
 
 
 class TableID(ID):
+    """ """
+
     table_schema: str
     name: str
 
     @root_validator(pre=True)
     def make_full_name(cls, values):
+        """
+
+        Args:
+            values:
+
+        Returns:
+
+        Raises:
+
+        """
         full_name = values.get("full_name", None)
         if values.get("full_name", None) is None:
             values["full_name"] = f"{values['table_schema']}.{values['name']}"
         return values
 
 
 class ColumnID(ID):
+    """ """
+
     table_schema: str
     table_name: str
     name: str
 
     @root_validator(pre=True)
     def make_full_name(cls, values):
+        """
+
+        Args:
+            values:
+
+        Returns:
+
+        Raises:
+
+        """
         full_name = values.get("full_name", None)
         if values.get("full_name", None) is None:
             values["full_name"] = f"{values['table_schema']}.{values['table_name']}.{values['name']}"
         return values
 
 
 class ColumnConstraint(Enum):
+    """ """
+
     primary_key = "p"
     unique = "u"
     foreign_key = "f"
     check = "c"
     trigger = "t"
     exclusion = "x"
 
 
 UNIQUE_COLUMN_CONSTRAINTS = {ColumnConstraint.primary_key.value, ColumnConstraint.unique.value}
 
 
 class Column(RedshiftNode):
+    """ """
+
     name: str = Field(alias="column_name")
     table: str = Field(alias="table_name")
     column_schema: str = Field(alias="schema")
     data_type: str
     is_nullable: bool
     namespace: str
     default_value: Any = Field(alias="column_default")
     column_constraint: Optional[ColumnConstraint]
     is_pk: Optional[bool] = False
     full_name: Optional[str] = None
 
     class Config:
+        """ """
+
         allow_population_by_field_name = True
 
     @validator("full_name", always=True)
     def make_full_name(cls, full_name, values):
+        """
+
+        Args:
+            full_name:
+            values:
+
+        Returns:
+
+        Raises:
+
+        """
         if full_name is not None:
             return full_name
         result = f"{values['column_schema']}.{values['table']}.{values['name']}"
         return result
 
 
 class Constraint(str, Enum):
+    """ """
+
     foreign_key = "FOREIGN KEY"
     primary_key = "PRIMARY KEY"
     belongs_to = "bt"
 
 
 class Edge(BaseModel):
+    """ """
+
     source: Union[ColumnID, TableID]
     destination: Union[ColumnID, TableID]
     definition: Optional[str]
     constraint_type: Constraint
     metadata: Optional[Dict] = None
 
 
 class TableType(str, Enum):
+    """ """
+
     Table = "BASE TABLE"
     View = "VIEW"
     ForeignTable = "FOREIGN"
     TemporaryTable = "LOCAL TEMPORARY"
 
 
 class Table(RedshiftNode):
+    """ """
+
     name: str = Field(alias="table_name")
     table_schema: str = Field(alias="schema")
     table_type: TableType
     namespace: str
     columns: Optional[List[Column]] = []
     metadata: Dict = {}
     full_name: Optional[str] = None
 
     class Config:
+        """ """
+
         allow_population_by_field_name = True
 
     @validator("full_name", always=True)
     def make_full_name(cls, full_name, values):
+        """
+
+        Args:
+            full_name:
+            values:
+
+        Returns:
+
+        Raises:
+
+        """
         if full_name is not None:
             return full_name
 
         return f"{values['table_schema']}.{values['name']}"
 
     def get_edges(self):
+        """ """
         return [
             Edge(
                 constraint_type=Constraint("bt"),
                 source=TableID(
                     table_schema=self.table_schema,
                     name=self.name,
                     namespace=self.namespace,
@@ -134,25 +203,36 @@
                 ),
             )
             for column in self.columns
         ]
 
 
 class EdgeQuery(BaseModel):
+    """ """
+
     namespace: str
     constraint_name: str
     constraint_type: str
     self_schema: str
     self_table: str
     self_column: str
     foreign_schema: str
     foreign_table: str
     foreign_column: str
 
     def to_edge(self) -> Edge:
+        """
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
         destination = ColumnID(
             table_schema=self.self_schema,
             table_name=self.self_table,
             name=self.self_column,
             namespace=self.namespace,
         )
         source = ColumnID(
```

### Comparing `grai_source_redshift-0.0.6/PKG-INFO` & `grai_source_redshift-0.0.7/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: grai-source-redshift
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: grai-client (>=0.2.4,<0.3.0)
-Requires-Dist: grai-schemas (>=0.1.5,<0.2.0)
+Requires-Dist: botocore (>=1.29.153,<2.0.0)
+Requires-Dist: grai-client (>=0.2.18,<0.3.0)
+Requires-Dist: grai-schemas (>=0.1.15,<0.2.0)
 Requires-Dist: multimethod (>=1.8,<2.0)
 Requires-Dist: pydantic[dotenv] (>=1.10.7,<2.0.0)
-Requires-Dist: redshift-connector (>=2.0.910,<3.0.0)
+Requires-Dist: redshift-connector (>=2.0.911,<3.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-redshift
 Description-Content-Type: text/markdown
 
 # Grai Redshift Integration
 
 The Redshift integration synchronizes metadata from a Redshift datawarehouse into your Grai data lineage graph.
```

