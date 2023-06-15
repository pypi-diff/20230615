# Comparing `tmp/peewee_migrate-1.8.1.tar.gz` & `tmp/peewee_migrate-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peewee_migrate-1.8.1.tar", max compression
+gzip compressed data, was "peewee_migrate-1.9.0.tar", max compression
```

## Comparing `peewee_migrate-1.8.1.tar` & `peewee_migrate-1.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     4456 2023-05-30 14:09:43.371776 peewee_migrate-1.8.1/README.rst
--rw-r--r--   0        0        0      146 2023-05-30 14:09:43.371776 peewee_migrate-1.8.1/peewee_migrate/__init__.py
--rw-r--r--   0        0        0       78 2023-05-30 14:09:43.371776 peewee_migrate-1.8.1/peewee_migrate/__main__.py
--rw-r--r--   0        0        0    12050 2023-05-30 14:09:43.371776 peewee_migrate-1.8.1/peewee_migrate/auto.py
--rw-r--r--   0        0        0     6597 2023-05-30 14:09:43.375776 peewee_migrate-1.8.1/peewee_migrate/cli.py
--rw-r--r--   0        0        0      146 2023-05-30 14:09:43.375776 peewee_migrate-1.8.1/peewee_migrate/logs.py
--rw-r--r--   0        0        0    19578 2023-05-30 14:09:43.375776 peewee_migrate-1.8.1/peewee_migrate/migrator.py
--rw-r--r--   0        0        0      461 2023-05-30 14:09:43.375776 peewee_migrate-1.8.1/peewee_migrate/models.py
--rw-r--r--   0        0        0        0 2023-05-30 14:09:43.375776 peewee_migrate-1.8.1/peewee_migrate/py.typed
--rw-r--r--   0        0        0    12235 2023-05-30 14:09:43.375776 peewee_migrate-1.8.1/peewee_migrate/router.py
--rw-r--r--   0        0        0     1802 2023-05-30 14:09:43.375776 peewee_migrate-1.8.1/peewee_migrate/template.py
--rw-r--r--   0        0        0      249 2023-05-30 14:09:43.375776 peewee_migrate-1.8.1/peewee_migrate/types.py
--rw-r--r--   0        0        0      325 2023-05-30 14:09:43.375776 peewee_migrate-1.8.1/peewee_migrate/utils.py
--rw-r--r--   0        0        0     1589 2023-05-30 14:09:43.375776 peewee_migrate-1.8.1/pyproject.toml
--rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 peewee_migrate-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     4456 2023-05-30 15:12:32.895942 peewee_migrate-1.9.0/README.rst
+-rw-r--r--   0        0        0      146 2023-05-30 15:12:32.895942 peewee_migrate-1.9.0/peewee_migrate/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-30 15:12:32.895942 peewee_migrate-1.9.0/peewee_migrate/__main__.py
+-rw-r--r--   0        0        0    12050 2023-05-30 15:12:32.895942 peewee_migrate-1.9.0/peewee_migrate/auto.py
+-rw-r--r--   0        0        0     6597 2023-05-30 15:12:32.895942 peewee_migrate-1.9.0/peewee_migrate/cli.py
+-rw-r--r--   0        0        0      146 2023-05-30 15:12:32.895942 peewee_migrate-1.9.0/peewee_migrate/logs.py
+-rw-r--r--   0        0        0    18807 2023-05-30 15:12:32.895942 peewee_migrate-1.9.0/peewee_migrate/migrator.py
+-rw-r--r--   0        0        0      461 2023-05-30 15:12:32.895942 peewee_migrate-1.9.0/peewee_migrate/models.py
+-rw-r--r--   0        0        0        0 2023-05-30 15:12:32.895942 peewee_migrate-1.9.0/peewee_migrate/py.typed
+-rw-r--r--   0        0        0    12235 2023-05-30 15:12:32.895942 peewee_migrate-1.9.0/peewee_migrate/router.py
+-rw-r--r--   0        0        0     1802 2023-05-30 15:12:32.895942 peewee_migrate-1.9.0/peewee_migrate/template.py
+-rw-r--r--   0        0        0      249 2023-05-30 15:12:32.895942 peewee_migrate-1.9.0/peewee_migrate/types.py
+-rw-r--r--   0        0        0      325 2023-05-30 15:12:32.895942 peewee_migrate-1.9.0/peewee_migrate/utils.py
+-rw-r--r--   0        0        0     1589 2023-05-30 15:12:32.895942 peewee_migrate-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 peewee_migrate-1.9.0/PKG-INFO
```

### Comparing `peewee_migrate-1.8.1/README.rst` & `peewee_migrate-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.8.1/peewee_migrate/auto.py` & `peewee_migrate-1.9.0/peewee_migrate/auto.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.8.1/peewee_migrate/cli.py` & `peewee_migrate-1.9.0/peewee_migrate/cli.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.8.1/peewee_migrate/migrator.py` & `peewee_migrate-1.9.0/peewee_migrate/migrator.py`

 * *Files 16% similar despite different names*

```diff
@@ -79,17 +79,21 @@
                 op()
         self.__ops__ = []
 
     def __iter__(self):
         """Iterate over models."""
         return iter(self.orm)
 
-    def __process__(self, *ops, db: bool = True):
-        if db:
-            self.__ops__.extend(ops)
+    def fake(self):
+        """Sync the current snapshot but not run operations.
+
+        >> with migrator.sync():
+        >>  # ... do changes
+        """
+        return SyncContext(self)
 
     @overload
     def __get_model__(self, model: TVModelType) -> TVModelType:
         ...
 
     @overload
     def __get_model__(self, model: str) -> TModelType:
@@ -112,202 +116,184 @@
         op = cast(Operation, self.__migrator__.sql(sql, *params))
         self.__ops__.append(op)
 
     def python(self, func: Callable, *args, **kwargs):
         """Run a python function."""
         self.__ops__.append(lambda: func(*args, **kwargs))
 
-    def create_model(self, model: TVModelType, *, pw_db=True) -> TVModelType:
+    def create_model(self, model: TVModelType) -> TVModelType:
         """Create model and table in database.
 
         :param model: Model class
-        :param pw_db(true): Create table in database
 
         >> migrator.create_model(Model)
         """
         meta = model._meta  # type: ignore[]
         self.orm.add(model)
 
         meta.database = self.__database__
-        self.__process__(model.create_table, db=pw_db)
+        self.__ops__.append(model.create_table)
         return model
 
     create_table = depricated_method(create_model, "create_table")
 
-    def remove_model(
-        self, model: Union[str, TModelType], *, cascade: bool = True, pw_db: bool = True
-    ):
+    def remove_model(self, model: Union[str, TModelType], *, cascade: bool = True):
         """Drop model and table from database.
 
         :param model: Model class or table name
         :param cascade(true): Drop table with cascade
-        :param pw_db(true): Drop table from database
 
         >> migrator.remove_model(Model, cascade=True)
         """
         model = self.__get_model__(model)
         self.orm.remove(model)
-        self.__process__(self.__migrator__.drop_table(model, cascade=cascade), db=pw_db)
+        self.__ops__.append(self.__migrator__.drop_table(model, cascade=cascade))
 
     drop_table = depricated_method(remove_model, "drop_table")
 
-    def add_fields(
-        self, model: Union[str, TModelType], *, pw_db: bool = True, **fields: pw.Field
-    ) -> TModelType:
+    def add_fields(self, model: Union[str, TModelType], **fields: pw.Field) -> TModelType:
         """Change fields.
 
         :param model: Model class or table name
-        :param pw_db(true): Change fields in database
 
         >> migrator.change_fields(Model, name=pw.CharField(null=True))
         """
         model = self.__get_model__(model)
         meta = model._meta  # type: ignore[]
         for name, field in fields.items():
             meta.add_field(name, field)
-            if not pw_db:
-                continue
 
             self.__ops__.append(
                 self.__migrator__.add_column(  # type: ignore[]
                     meta.table_name, field.column_name, field
                 )
             )
             if field.unique:
                 self.__ops__.append(
                     self.__migrator__.add_index(meta.table_name, (field.column_name,), unique=True)
                 )
         return model
 
     add_columns = depricated_method(add_fields, "add_columns")
 
-    def change_fields(
-        self, model: Union[str, TModelType], *, pw_db: bool = True, **fields: pw.Field
-    ) -> TModelType:
+    def change_fields(self, model: Union[str, TModelType], **fields: pw.Field) -> TModelType:
         """Change fields.
 
         :param model: Model class or table name
-        :param pw_db(true): Change fields in database
 
         >> migrator.change_fields(Model, name=pw.CharField(null=True))
         """
         model = self.__get_model__(model)
         meta: pw.Metadata = model._meta  # type: ignore[]
         for name, field in fields.items():
             old_field = meta.fields.get(name, field)
             old_column_name = old_field and old_field.column_name
 
             meta.add_field(name, field)
 
-            if pw_db:
-                if isinstance(old_field, pw.ForeignKeyField):
-                    self.__ops__.append(
-                        self.__migrator__.drop_foreign_key_constraint(
-                            meta.table_name, old_column_name
-                        )
-                    )
-
-                if old_column_name != field.column_name:
-                    self.__ops__.append(
-                        self.__migrator__.rename_column(
-                            meta.table_name, old_column_name, field.column_name
-                        )
-                    )
+            if isinstance(old_field, pw.ForeignKeyField):
+                self.__ops__.append(
+                    self.__migrator__.drop_foreign_key_constraint(meta.table_name, old_column_name)
+                )
 
-                if isinstance(field, pw.ForeignKeyField):
-                    on_delete = field.on_delete if field.on_delete else "RESTRICT"
-                    on_update = field.on_update if field.on_update else "RESTRICT"
-                    self.__ops__.append(
-                        self.__migrator__.add_foreign_key_constraint(
-                            meta.table_name,
-                            field.column_name,
-                            field.rel_model._meta.table_name,
-                            field.rel_field.name,
-                            on_delete,
-                            on_update,
-                        )
+            if old_column_name != field.column_name:
+                self.__ops__.append(
+                    self.__migrator__.rename_column(
+                        meta.table_name, old_column_name, field.column_name
                     )
-                    continue
+                )
 
+            if isinstance(field, pw.ForeignKeyField):
+                on_delete = field.on_delete if field.on_delete else "RESTRICT"
+                on_update = field.on_update if field.on_update else "RESTRICT"
                 self.__ops__.append(
-                    self.__migrator__.change_column(  # type: ignore[]
-                        meta.table_name, field.column_name, field
+                    self.__migrator__.add_foreign_key_constraint(
+                        meta.table_name,
+                        field.column_name,
+                        field.rel_model._meta.table_name,
+                        field.rel_field.name,
+                        on_delete,
+                        on_update,
                     )
                 )
+                continue
+
+            self.__ops__.append(
+                self.__migrator__.change_column(  # type: ignore[]
+                    meta.table_name, field.column_name, field
+                )
+            )
 
             if field.unique == old_field.unique:
                 continue
 
             if field.unique:
                 index = (field.column_name,), field.unique
                 meta.indexes.append(index)
-                self.__process__(self.__migrator__.add_index(meta.table_name, *index), db=pw_db)
+                self.__ops__.append(self.__migrator__.add_index(meta.table_name, *index))
             else:
                 index = field.column_name
                 with suppress(ValueError):
                     meta.indexes.remove(((field.column_name,), True))
-                self.__process__(self.__migrator__.drop_index(meta.table_name, index), db=pw_db)
+                self.__ops__.append(self.__migrator__.drop_index(meta.table_name, index))
 
         return model
 
     change_columns = depricated_method(change_fields, "change_columns")
 
     def remove_fields(
-        self, model: Union[str, TModelType], *names: str, cascade: bool = True, pw_db: bool = True
+        self, model: Union[str, TModelType], *names: str, cascade: bool = True
     ) -> TModelType:
         """Remove fields from model.
 
         :param model: Model class or table name
         :param cascade(true): Drop columns with cascade
-        :param pw_db(true): Remove fields from Database
 
         >> migrator.remove_fields(Model, "name", "age", cascade=True)
         """
         model = self.__get_model__(model)
         meta = model._meta  # type: ignore[]
         fields = [field for field in meta.fields.values() if field.name in names]
         for field in fields:
             self.__del_field__(model, field)
-            if pw_db:
-                if field.unique:
-                    index_name = make_index_name(meta.table_name, [field.column_name])
-                    self.__ops__.append(self.__migrator__.drop_index(meta.table_name, index_name))
-                self.__ops__.append(
-                    self.__migrator__.drop_column(  # type: ignore[]
-                        meta.table_name, field.column_name, cascade=cascade
-                    )
+            if field.unique:
+                index_name = make_index_name(meta.table_name, [field.column_name])
+                self.__ops__.append(self.__migrator__.drop_index(meta.table_name, index_name))
+            self.__ops__.append(
+                self.__migrator__.drop_column(  # type: ignore[]
+                    meta.table_name, field.column_name, cascade=cascade
                 )
+            )
         return model
 
     drop_columns = depricated_method(remove_fields, "drop_columns")
 
     def rename_field(
-        self, model: Union[str, TModelType], old_name: str, new_name: str, *, pw_db=True
+        self, model: Union[str, TModelType], old_name: str, new_name: str
     ) -> TModelType:
         """Rename field in model.
 
         :param model: Model class or table name
         :param old_name: Old field name
         :param new_name: New field name
-        :param pw_db(true): Rename field in Database
 
         >> migrator.rename_field(Model, "name", "full_name")
         """
         model = self.__get_model__(model)
         meta = model._meta  # type: ignore[]
         field = meta.fields[old_name]
         if isinstance(field, pw.ForeignKeyField):
             old_name = field.column_name
         self.__del_field__(model, field)
         field.name = field.column_name = new_name
         if isinstance(field, pw.ForeignKeyField):
             field.column_name = field.column_name + "_id"
         meta.add_field(new_name, field)
-        self.__process__(
-            self.__migrator__.rename_column(meta.table_name, old_name, field.column_name), db=pw_db
+        self.__ops__.append(
+            self.__migrator__.rename_column(meta.table_name, old_name, field.column_name)
         )
         return model
 
     rename_column = depricated_method(rename_field, "rename_column")
 
     def __del_field__(self, model: TModelType, field: pw.Field):
         """Delete field from model."""
@@ -318,50 +304,44 @@
             obj_id_name = field.column_name
             if field.column_name == field.name:
                 obj_id_name += "_id"
             if hasattr(model, obj_id_name):
                 delattr(model, obj_id_name)
             delattr(field.rel_model, field.backref)
 
-    def rename_table(
-        self, model: Union[str, TModelType], new_name: str, *, pw_db=True
-    ) -> TModelType:
+    def rename_table(self, model: Union[str, TModelType], new_name: str) -> TModelType:
         """Rename table in database."""
         model = self.__get_model__(model)
         meta = model._meta  # type: ignore[]
         old_name = meta.table_name
         self.orm.remove(model)
         meta.table_name = new_name
         self.orm.add(model)
-        self.__process__(self.__migrator__.rename_table(old_name, new_name), db=pw_db)
+        self.__ops__.append(self.__migrator__.rename_table(old_name, new_name))
         return model
 
-    def add_index(
-        self, model: Union[str, TModelType], *columns: str, unique=False, pw_db: bool = True
-    ) -> TModelType:
+    def add_index(self, model: Union[str, TModelType], *columns: str, unique=False) -> TModelType:
         """Create indexes."""
         model = self.__get_model__(model)
         meta = model._meta  # type: ignore[]
         meta.indexes.append((columns, unique))
         columns_ = []
         for col in columns:
             field = meta.fields.get(col)
 
             if len(columns) == 1:
                 field.unique = unique
                 field.index = not unique
 
             columns_.append(field.column_name)
 
-        self.__process__(
-            self.__migrator__.add_index(meta.table_name, columns_, unique=unique), db=pw_db
-        )
+        self.__ops__.append(self.__migrator__.add_index(meta.table_name, columns_, unique=unique))
         return model
 
-    def drop_index(self, model: Union[str, TModelType], *columns: str, pw_db=True) -> TModelType:
+    def drop_index(self, model: Union[str, TModelType], *columns: str) -> TModelType:
         """Drop indexes."""
         model = self.__get_model__(model)
         meta = model._meta  # type: ignore[]
         columns_ = []
         for col in columns:
             field = meta.fields.get(col)
             if not field:
@@ -370,70 +350,59 @@
             if len(columns) == 1:
                 field.unique = field.index = False
 
             columns_.append(field.column_name)
 
         index_name = make_index_name(meta.table_name, columns_)
         meta.indexes = [(cols, _) for (cols, _) in meta.indexes if columns != cols]
-        self.__process__(self.__migrator__.drop_index(meta.table_name, index_name), db=pw_db)
+        self.__ops__.append(self.__migrator__.drop_index(meta.table_name, index_name))
         return model
 
-    def add_not_null(self, model: Union[str, TModelType], *names: str, pw_db=True) -> TModelType:
+    def add_not_null(self, model: Union[str, TModelType], *names: str) -> TModelType:
         """Add not null."""
         model = self.__get_model__(model)
         meta = model._meta  # type: ignore[]
         for name in names:
             field = meta.fields[name]
             field.null = False
-            self.__process__(
-                self.__migrator__.add_not_null(meta.table_name, field.column_name), db=pw_db
-            )
+            self.__ops__.append(self.__migrator__.add_not_null(meta.table_name, field.column_name))
         return model
 
-    def drop_not_null(self, model: Union[str, TModelType], *names: str, pw_db=True) -> TModelType:
+    def drop_not_null(self, model: Union[str, TModelType], *names: str) -> TModelType:
         """Drop not null."""
         model = self.__get_model__(model)
         meta = model._meta  # type: ignore[]
         for name in names:
             field = meta.fields[name]
             field.null = True
-            self.__process__(
-                self.__migrator__.drop_not_null(meta.table_name, field.column_name), db=pw_db
-            )
+            self.__ops__.append(self.__migrator__.drop_not_null(meta.table_name, field.column_name))
         return model
 
-    def add_default(
-        self, model: Union[str, TModelType], name: str, default: Any, *, pw_db=True
-    ) -> TModelType:
+    def add_default(self, model: Union[str, TModelType], name: str, default: Any) -> TModelType:
         """Add default."""
         model = self.__get_model__(model)
         meta = model._meta  # type: ignore[]
         field = meta.fields[name]
         meta.defaults[field] = field.default = default
-        self.__process__(self.__migrator__.apply_default(meta.table_name, name, field), db=pw_db)
+        self.__ops__.append(self.__migrator__.apply_default(meta.table_name, name, field))
         return model
 
-    def add_constraint(self, model: Union[str, TModelType], name, constraint, *, pw_db=True):
+    def add_constraint(self, model: Union[str, TModelType], name, constraint):
         """Add constraint."""
         model = self.__get_model__(model)
         meta = model._meta  # type: ignore[]
-        self.__process__(
-            self.__migrator__.add_constraint(meta.table_name, name, constraint), db=pw_db
-        )
+        self.__ops__.append(self.__migrator__.add_constraint(meta.table_name, name, constraint))
         return model
 
-    def drop_constraints(
-        self, model: Union[str, TModelType], *names: str, pw_db=True
-    ) -> TModelType:
+    def drop_constraints(self, model: Union[str, TModelType], *names: str) -> TModelType:
         """Drop constraints."""
         model = self.__get_model__(model)
         meta = model._meta  # type: ignore[]
-        self.__process__(
-            *[self.__migrator__.drop_constraint(meta.table_name, name) for name in names],
-            db=pw_db,
+        self.__ops__.extend(
+            [self.__migrator__.drop_constraint(meta.table_name, name) for name in names]
         )
         return model
 
 
 class SchemaMigrator(ScM):
     """Implement migrations."""
 
@@ -550,7 +519,20 @@
 
         def fn(c_name, c_def):
             ctx = self.make_context()
             ctx.sql(field.ddl(ctx))
             return ctx.query()[0]
 
         return [self._update_column(table, column, fn)]  # type: ignore[]
+
+
+class SyncContext:
+    def __init__(self, migrator):
+        self.migrator = migrator
+        self.ops = None
+
+    def __enter__(self):
+        self.ops = list(self.migrator.__ops__)
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.migrator.__ops__ = self.ops
```

### Comparing `peewee_migrate-1.8.1/peewee_migrate/router.py` & `peewee_migrate-1.9.0/peewee_migrate/router.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.8.1/peewee_migrate/template.py` & `peewee_migrate-1.9.0/peewee_migrate/template.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.8.1/pyproject.toml` & `peewee_migrate-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peewee-migrate"
-version = "1.8.1"
+version = "1.9.0"
 homepage = "https://github.com/klen/peewee_migrate"
 repository = "https://github.com/klen/peewee_migrate"
 description = "Support for migrations in Peewee ORM"
 readme = "README.rst"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 keywords = ["peewee", "migrations", "orm"]
```

### Comparing `peewee_migrate-1.8.1/PKG-INFO` & `peewee_migrate-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peewee-migrate
-Version: 1.8.1
+Version: 1.9.0
 Summary: Support for migrations in Peewee ORM
 Home-page: https://github.com/klen/peewee_migrate
 License: MIT
 Keywords: peewee,migrations,orm
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

