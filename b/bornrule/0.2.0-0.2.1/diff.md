# Comparing `tmp/bornrule-0.2.0.tar.gz` & `tmp/bornrule-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bornrule-0.2.0.tar", max compression
+gzip compressed data, was "bornrule-0.2.1.tar", max compression
```

## Comparing `bornrule-0.2.0.tar` & `bornrule-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2022-02-17 15:07:25.514146 bornrule-0.2.0/LICENSE
--rw-r--r--   0        0        0     1919 2023-03-09 23:35:03.712307 bornrule-0.2.0/README.min.md
--rw-r--r--   0        0        0       62 2022-11-22 14:45:52.298028 bornrule-0.2.0/bornrule/__init__.py
--rw-r--r--   0        0        0    15645 2022-11-22 12:34:29.983982 bornrule-0.2.0/bornrule/born.py
--rw-r--r--   0        0        0       70 2022-03-18 22:15:10.938536 bornrule-0.2.0/bornrule/sql/__init__.py
--rw-r--r--   0        0        0    15498 2023-03-14 11:26:47.555704 bornrule-0.2.0/bornrule/sql/born.py
--rw-r--r--   0        0        0    18043 2023-03-14 13:55:27.483039 bornrule-0.2.0/bornrule/sql/database.py
--rw-r--r--   0        0        0      120 2023-03-14 10:07:39.656021 bornrule-0.2.0/bornrule/sql/postgresql.py
--rw-r--r--   0        0        0      541 2023-03-14 10:07:46.660157 bornrule-0.2.0/bornrule/sql/sqlite.py
--rw-r--r--   0        0        0       42 2022-02-18 12:44:02.006465 bornrule-0.2.0/bornrule/torch/__init__.py
--rw-r--r--   0        0        0     3138 2022-10-16 14:20:33.656418 bornrule-0.2.0/bornrule/torch/born.py
--rw-r--r--   0        0        0      534 2023-03-13 17:02:06.791717 bornrule-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2722 1970-01-01 00:00:00.000000 bornrule-0.2.0/setup.py
--rw-r--r--   0        0        0     2912 1970-01-01 00:00:00.000000 bornrule-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-02-17 15:07:25.514146 bornrule-0.2.1/LICENSE
+-rw-r--r--   0        0        0      379 2023-03-28 13:25:05.932038 bornrule-0.2.1/README.min.md
+-rw-r--r--   0        0        0       62 2022-11-22 14:45:52.298028 bornrule-0.2.1/bornrule/__init__.py
+-rw-r--r--   0        0        0    15645 2022-11-22 12:34:29.983982 bornrule-0.2.1/bornrule/born.py
+-rw-r--r--   0        0        0       70 2022-03-18 22:15:10.938536 bornrule-0.2.1/bornrule/sql/__init__.py
+-rw-r--r--   0        0        0    15208 2023-06-14 21:08:12.886183 bornrule-0.2.1/bornrule/sql/born.py
+-rw-r--r--   0        0        0    18607 2023-06-14 21:39:35.203788 bornrule-0.2.1/bornrule/sql/database.py
+-rw-r--r--   0        0        0      120 2023-03-14 10:07:39.656021 bornrule-0.2.1/bornrule/sql/postgresql.py
+-rw-r--r--   0        0        0      541 2023-03-14 10:07:46.660157 bornrule-0.2.1/bornrule/sql/sqlite.py
+-rw-r--r--   0        0        0       42 2022-02-18 12:44:02.006465 bornrule-0.2.1/bornrule/torch/__init__.py
+-rw-r--r--   0        0        0     3111 2023-03-28 13:39:18.510897 bornrule-0.2.1/bornrule/torch/born.py
+-rw-r--r--   0        0        0      534 2023-06-14 21:40:32.787890 bornrule-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1124 1970-01-01 00:00:00.000000 bornrule-0.2.1/setup.py
+-rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 bornrule-0.2.1/PKG-INFO
```

### Comparing `bornrule-0.2.0/LICENSE` & `bornrule-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bornrule-0.2.0/bornrule/born.py` & `bornrule-0.2.1/bornrule/born.py`

 * *Files identical despite different names*

### Comparing `bornrule-0.2.0/bornrule/sql/born.py` & `bornrule-0.2.1/bornrule/sql/born.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,45 +98,44 @@
         else:
             raise ValueError(
                 f"Backend {slug} is not implemented yet. Please open an issue at "
                 f"https://github.com/eguidotti/bornrule/issues "
                 f"to add support for {slug}."
             )
 
-        self._default_params = dict(a=0.5, b=1, h=1)
-        self._params = None
+        self.params = None
 
     def get_params(self):
         """Get parameters
 
         Returns
         -------
         params : dict
             Model's hyper-parameters `a`, `b`, `h`.
 
         """
-        if self._params is None:
+        if self.params is None:
             with self.db.connect() as con:
-                self._params = self.db.read_params(con) or self._default_params.copy()
+                self.params = self.db.read_params(con)
 
-        return self._params
+        return self.params
 
     def set_params(self, **kwargs):
         """Set parameters
 
         Parameters
         ----------
         **kwargs
              Model's hyper-parameters: `a` (>0), `b` (>=0), and `h` (>=0).
 
         """
         params = self.get_params()
         params.update(kwargs)
 
-        valid = self._default_params.keys()
+        valid = self.db.default_params.keys()
         invalid = set(params.keys()) - set(valid)
         if invalid:
             raise ValueError(
                 f"Invalid parameter(s): {', '.join(invalid)}. "
                 f"Valid parameters are: {', '.join(valid)}."
             )
 
@@ -155,15 +154,15 @@
                 "The parameter 'h' must be non-negative."
             )
 
         with self.db.connect() as con:
             with con.begin():
                 self.db.check_editable(con)
                 self.db.write_params(con, **params)
-                self._params = params
+                self.params = params
 
     def fit(self, X, y, sample_weight=None):
         """Fit the classifier according to the training data X, y
 
         Parameters
         ----------
         X : list of dict of length n_samples
@@ -211,24 +210,18 @@
         -------
         self : object
             Returns the instance itself.
 
         """
         self._validate(X=X, y=y, sample_weight=sample_weight)
 
-        if sample_weight is None:
-            sample_weight = [1] * len(X)
-
         with self.db.connect() as con:
             with con.begin():
                 self.db.check_editable(con)
-                self.db.write_corpus(con, X=X, y=y, sample_weight=sample_weight)
-
-                if not self.db.is_params(con):
-                    self.db.write_params(con, **self._default_params)
+                self.db.partial_fit(con, X=X, y=y, sample_weight=sample_weight)
 
         return self
 
     def predict(self, X):
         """Perform classification on the test data X
 
         Parameters
@@ -362,15 +355,15 @@
 
         """
         with self.db.connect() as con:
             with con.begin():
                 self.db.undeploy(con, deep=deep)
 
         if deep:
-            self._params = None
+            self.params = None
 
     def is_fitted(self):
         """Is fitted?
 
         Checks whether the instance is fitted.
 
         Returns
```

### Comparing `bornrule-0.2.0/bornrule/sql/database.py` & `bornrule-0.2.1/bornrule/sql/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,20 @@
         self.type_class = type_class
 
         self.j = self.field_feature = field_feature
         self.k = self.field_class = field_class
         self.n = self.field_item = field_item
         self.w = self.field_weight = field_weight
 
+        self.default_params = {
+            'a': 0.5,
+            'b': 1,
+            'h': 1,
+        }
+
         self.table_params = Table(
             table_params, MetaData(),
             Column(self.field_id, String, primary_key=True),
             Column('a', Float, nullable=False),
             Column('b', Float, nullable=False),
             Column('h', Float, nullable=False),
         )
@@ -142,15 +148,15 @@
             keys = cursor.keys()
 
             if values:
                 params = dict(zip(keys, values))
                 params.pop(self.field_id)
                 return params
 
-        return None
+        return self.default_params
 
     def read_sql(self, sql, con):
         cur = con.execute(text(sql) if isinstance(sql, str) else sql)
         data = [tuple(row) for row in cur.fetchall()]
         columns = cur.keys()
 
         return pd.DataFrame(data, columns=columns)
@@ -184,30 +190,33 @@
 
         if values is not None:
             insert = getattr(self, "insert" if if_exists in ['fail', 'replace', 'ignore'] else if_exists)
             insert(con, table, values, **kwargs)
 
         return table
 
-    def write_params(self, con, **kwargs):
+    def write_params(self, con, **params):
         if_exists = {
             'if_exists': 'insert_or_replace',
             'conflict': [self.field_id],
-            'replace': list(kwargs.keys())
+            'replace': list(params.keys())
         }
 
-        return self.write(con, table=self.table_params, values=[{self.field_id: self.id, **kwargs}], **if_exists)
+        return self.write(con, table=self.table_params, values=[{self.field_id: self.id, **params}], **if_exists)
 
     def write_corpus(self, con, X, y, sample_weight):
         if_exists = {
             'if_exists': 'insert_or_sum',
             'conflict': [self.field_class, self.field_feature],
             'sum': [self.field_weight]
         }
 
+        if sample_weight is None:
+            sample_weight = [1] * len(X)
+
         corpus = defaultdict(lambda: defaultdict(int))
         for x, y, w in zip(X, y, sample_weight):
             if not isinstance(y, dict):
                 y = {y: 1}
 
             n = sum(x.values())
             for k, p in y.items():
@@ -233,15 +242,16 @@
             for i, x in enumerate(X)
             for f, w in x.items()
         ]
 
         return self.write(con, table=table, values=values)
 
     def is_params(self, con):
-        return self.read_params(con) is not None
+        sql = f"SELECT COUNT(*) FROM {self.table_params} WHERE {self.field_id}='{self.id}'"
+        return self.exists(con, self.table_params) and con.execute(text(sql)).fetchone()[0]
 
     def is_corpus(self, con):
         return self.exists(con, self.table_corpus)
 
     def is_deployed(self, con):
         return self.exists(con, self.table_weights)
 
@@ -297,14 +307,19 @@
 
             if self.is_params(con):
                 con.execute(text(f"DELETE FROM {self.table_params} WHERE {self.field_id}='{self.id}'"))
 
                 if con.execute(text(f"SELECT COUNT(*) FROM {self.table_params}")).fetchone()[0] == 0:
                     self.table_params.drop(con)
 
+    def partial_fit(self, con, X, y, sample_weight):
+        self.write_corpus(con, X=X, y=y, sample_weight=sample_weight)
+        if not self.is_params(con):
+            self.write_params(con, **self.default_params)
+
     def predict(self, con, X):
         cache = self.is_deployed(con)
         items = self.write_items(con, X)
         sql = self._sql_predict(cache, items)
 
         return self.read_sql(sql, con)
```

### Comparing `bornrule-0.2.0/bornrule/sql/sqlite.py` & `bornrule-0.2.1/bornrule/sql/sqlite.py`

 * *Files identical despite different names*

### Comparing `bornrule-0.2.0/bornrule/torch/born.py` & `bornrule-0.2.1/bornrule/torch/born.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,22 +57,21 @@
             dtype = torch.get_default_dtype()
 
         weight = torch.complex(real, imag) if self.is_complex(dtype) else torch.stack((real, imag))
         weight = weight.to(device=device, dtype=dtype)
         self.weight = torch.nn.Parameter(weight)
         
     def forward(self, x):
-        r"""Applies the following transformation to the incoming data:
+        r"""Applies the following transformation to each input sample:
 
         ```math
-        y = \dfrac{\operatorname{Mod}(xW)^2}{|| \operatorname{Mod}(xW)^2 ||_1}
+        y_k = \dfrac{\operatorname{Mod}(\sum_j W_{jk}x_j)^2}{\sum_k \operatorname{Mod}(\sum_j W_{jk}x_j)^2}
         ```
 
-        where $`\operatorname{Mod}`$ is the modulus of complex numbers,
-        and $`||\cdot||_1`$ is the L1-norm of a vector.
+        where $`\operatorname{Mod}`$ is the modulus of complex numbers.
 
         Parameters
         ----------
         x : torch.Tensor
             Input samples of shape (`n_samples`, `in_features`).
 
         Returns
```

### Comparing `bornrule-0.2.0/pyproject.toml` & `bornrule-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bornrule"
-version = "0.2.0"
+version = "0.2.1"
 license = "GPL-3.0-or-later"
 description = "Classification with Born's rule"
 authors = ["Emanuele Guidotti <emanuele.guidotti@unine.ch>"]
 readme = "README.min.md"
 repository = "https://github.com/eguidotti/bornrule"
 documentation = "https://bornrule.eguidotti.com"
```

