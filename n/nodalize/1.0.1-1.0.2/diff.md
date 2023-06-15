# Comparing `tmp/nodalize-1.0.1-py3-none-any.whl.zip` & `tmp/nodalize-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 66390 bytes, number of entries: 43
+Zip file size: 66712 bytes, number of entries: 43
 -rw-r--r--  2.0 unx      102 b- defN 23-Jun-04 09:32 nodalize/__init__.py
 -rw-r--r--  2.0 unx    13455 b- defN 23-Jun-14 20:31 nodalize/datanode.py
--rw-r--r--  2.0 unx     5436 b- defN 23-Jun-14 20:24 nodalize/dependency.py
+-rw-r--r--  2.0 unx     6443 b- defN 23-Jun-15 16:57 nodalize/dependency.py
 -rw-r--r--  2.0 unx     2673 b- defN 23-Jun-04 09:22 nodalize/dependency_loader.py
 -rw-r--r--  2.0 unx       58 b- defN 22-Sep-01 17:05 nodalize/calculators/__init__.py
 -rw-r--r--  2.0 unx     9656 b- defN 23-Jun-10 15:25 nodalize/calculators/calculator.py
 -rw-r--r--  2.0 unx    14888 b- defN 23-Jun-04 17:18 nodalize/calculators/dask_calculator.py
 -rw-r--r--  2.0 unx    12382 b- defN 23-Jun-04 17:19 nodalize/calculators/pandas_calculator.py
 -rw-r--r--  2.0 unx    13967 b- defN 23-Jun-10 15:25 nodalize/calculators/polars_calculator.py
 -rw-r--r--  2.0 unx    19052 b- defN 23-Jun-10 15:25 nodalize/calculators/pyarrow_calculator.py
@@ -24,22 +24,22 @@
 -rw-r--r--  2.0 unx    13798 b- defN 23-Jun-11 17:07 nodalize/data_management/delta_lake_data_manager.py
 -rw-r--r--  2.0 unx    29878 b- defN 23-Jun-10 15:26 nodalize/data_management/kdb_data_manager.py
 -rw-r--r--  2.0 unx     8213 b- defN 23-Jun-10 15:25 nodalize/data_management/local_file_data_manager.py
 -rw-r--r--  2.0 unx     8415 b- defN 23-Jun-10 15:25 nodalize/data_management/s3_file_data_manager.py
 -rw-r--r--  2.0 unx    15158 b- defN 23-Jun-10 15:24 nodalize/data_management/sqlite_data_manager.py
 -rw-r--r--  2.0 unx       47 b- defN 22-Sep-01 17:05 nodalize/orchestration/__init__.py
 -rw-r--r--  2.0 unx     2899 b- defN 23-Jun-04 09:32 nodalize/orchestration/calculator_factory.py
--rw-r--r--  2.0 unx    11867 b- defN 23-Jun-14 20:20 nodalize/orchestration/coordinator.py
+-rw-r--r--  2.0 unx    12816 b- defN 23-Jun-15 16:25 nodalize/orchestration/coordinator.py
 -rw-r--r--  2.0 unx     1784 b- defN 23-Jun-04 09:21 nodalize/orchestration/data_manager_factory.py
 -rw-r--r--  2.0 unx     3790 b- defN 23-Jun-04 09:22 nodalize/orchestration/data_node_cache.py
 -rw-r--r--  2.0 unx       37 b- defN 22-Sep-01 17:05 nodalize/tools/__init__.py
 -rw-r--r--  2.0 unx     1942 b- defN 23-Apr-16 11:18 nodalize/tools/dates.py
 -rw-r--r--  2.0 unx     1772 b- defN 22-Dec-30 16:50 nodalize/tools/static_func_tools.py
 -rw-r--r--  2.0 unx     4112 b- defN 22-Sep-01 17:05 nodalize/tools/tree.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-22 14:42 sandbox/__init__.py
 -rw-r--r--  2.0 unx       81 b- defN 23-Jun-10 14:57 sandbox/test_anything.py
--rw-r--r--  2.0 unx     1060 b- defN 23-Jun-14 20:35 nodalize-1.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     6033 b- defN 23-Jun-14 20:35 nodalize-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-14 20:35 nodalize-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jun-14 20:35 nodalize-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3907 b- defN 23-Jun-14 20:35 nodalize-1.0.1.dist-info/RECORD
-43 files, 253552 bytes uncompressed, 60050 bytes compressed:  76.3%
+-rw-r--r--  2.0 unx     1060 b- defN 23-Jun-15 17:17 nodalize-1.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6033 b- defN 23-Jun-15 17:17 nodalize-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 17:17 nodalize-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-15 17:17 nodalize-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3907 b- defN 23-Jun-15 17:17 nodalize-1.0.2.dist-info/RECORD
+43 files, 255508 bytes uncompressed, 60372 bytes compressed:  76.4%
```

## zipnote {}

```diff
@@ -108,23 +108,23 @@
 
 Filename: sandbox/__init__.py
 Comment: 
 
 Filename: sandbox/test_anything.py
 Comment: 
 
-Filename: nodalize-1.0.1.dist-info/LICENSE
+Filename: nodalize-1.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: nodalize-1.0.1.dist-info/METADATA
+Filename: nodalize-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: nodalize-1.0.1.dist-info/WHEEL
+Filename: nodalize-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: nodalize-1.0.1.dist-info/top_level.txt
+Filename: nodalize-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: nodalize-1.0.1.dist-info/RECORD
+Filename: nodalize-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nodalize/dependency.py

```diff
@@ -2,14 +2,39 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from nodalize.calculators.calculator import Calculator
 from nodalize.constants.column_category import ColumnCategory
 from nodalize.data_management.data_manager import DataManager
 
 
+class ParameterValue:
+    """Class to store a parameter name, to use in a filter."""
+
+    __slots__ = "_parameter_name"
+
+    def __init__(self, parameter_name: str) -> None:
+        """
+        Initialize.
+
+        Args:
+            parameter_name: name of the parameter to use
+        """
+        self._parameter_name = parameter_name
+
+    @property
+    def parameter_name(self) -> str:
+        """
+        Get name of the parameter.
+
+        Returns:
+            name of the parameter
+        """
+        return self._parameter_name
+
+
 class DependencyDefinition:
     """Class storing definition for a data node dependency."""
 
     __slots__ = (
         "_node_identifier",
         "_filters",
         "_fields",
@@ -125,15 +150,27 @@
             parameters: parameters to use for the calculation - may or may not be related to parameters columns
             parent_batch_ids: batch ids of the parent data to load
 
         Returns:
             data frame
         """
         if self.filters is not None and len(self.filters) > 0:
-            filters = self.filters
+            filters = [
+                [
+                    (
+                        filterDesc[0],
+                        filterDesc[1],
+                        parameters[filterDesc[2].parameter_name]
+                        if isinstance(filterDesc[2], ParameterValue)
+                        else filterDesc[2],
+                    )
+                    for filterDesc in andFilter
+                ]
+                for andFilter in self.filters
+            ]
         else:
             parameter_columns = set(
                 self.data_node.get_column_names([ColumnCategory.PARAMETER])
             )
             filters = [
                 [(k, "=", v) for k, v in parameters.items() if k in parameter_columns]
             ]
```

## nodalize/orchestration/coordinator.py

```diff
@@ -109,14 +109,47 @@
             identifier: identifier of the data node to find
 
         Returns:
             data node instance
         """
         return self._cache.get_data_node(identifier)
 
+    def get_data_nodes(self) -> List[DataNode]:
+        """
+        Get all data nodes.
+
+        Returns:
+            list of ndoes
+        """
+        return list(self._cache._nodes.values())
+
+    def get_data_node_identifiers(self) -> List[str]:
+        """
+        Get all data node identifiers.
+
+        Returns:
+            list of identifiers
+        """
+        return list(self._cache._nodes.keys())
+
+    def get_dependency_graph_levels(
+        self, identifiers: Optional[List[str]] = None
+    ) -> List[List[DataNode]]:
+        """
+        Get levels of dependency graph as list of lists.
+
+        Args:
+            list of ids to load, if None then load everything
+
+        Returns:
+            list of levels, each level is a list of node identifiers
+        """
+        identifiers = identifiers or self.get_data_node_identifiers()
+        return self._cache.build_downstream_tree(identifiers).levels
+
     def set_up(self):
         """Set up all nodes."""
         self._cache.build_dependency_graph()
 
     def compute_and_save_single_node(
         self,
         node: DataNode,
```

## Comparing `nodalize-1.0.1.dist-info/LICENSE` & `nodalize-1.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `nodalize-1.0.1.dist-info/METADATA` & `nodalize-1.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodalize
-Version: 1.0.1
+Version: 1.0.2
 Summary: Framework to organize data transformation flow.
 Home-page: https://github.com/Ron-Ldn/nodalize
 Author: Ronan Mouquet
 Author-email: ronan.mouquet@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

## Comparing `nodalize-1.0.1.dist-info/RECORD` & `nodalize-1.0.2.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 nodalize/__init__.py,sha256=BmDtEafssUfgezj0dhPKSbCnWmNVlvUz6OFORPwPvnA,102
 nodalize/datanode.py,sha256=D19iM-CoZyqWLf4jQj8gq9KUenFbxdJRwm8ppos4yro,13455
-nodalize/dependency.py,sha256=xmNxltm0CEGVBOp1K4a0WEiKf1ugzCuosgZ8Xbwzcng,5436
+nodalize/dependency.py,sha256=S9maNUsa5KHhbaT1GRa0I8CjSIJz26prQ5AsdmG-Eww,6443
 nodalize/dependency_loader.py,sha256=GKlg71LFXLp12HiK1yjvsKKCMqFVEJXdn11rGwd69Rs,2673
 nodalize/calculators/__init__.py,sha256=UuTx55ZtSkzjuC_A77uWYb6WTAFtoaJCGuWYI57L9IU,58
 nodalize/calculators/calculator.py,sha256=uOACNqM3Qr1sAfYIbothYKxFShCM8xCkHYSw04rEz1Y,9656
 nodalize/calculators/dask_calculator.py,sha256=PdgValqvy5V2ZBTrsdOAzuqPZYguxaSG58FLwX9WjBo,14888
 nodalize/calculators/pandas_calculator.py,sha256=pEVYEzzzcQs8rMrFY95obqx349kUCB4FPMSDVpW3XF0,12382
 nodalize/calculators/polars_calculator.py,sha256=e5QJKy8A4E1IWG6EqNguR3_ETn4kiLqOe8wqsGVGI3M,13967
 nodalize/calculators/pyarrow_calculator.py,sha256=xbU7avBzRw6_URPukYO7DyZMwhcb6HuvWX6-AbO0RxE,19052
@@ -23,21 +23,21 @@
 nodalize/data_management/delta_lake_data_manager.py,sha256=Umb3Nu7WuXPhgJSfKvj6oenSqBP81P2uRsyNbsXH-4Y,13798
 nodalize/data_management/kdb_data_manager.py,sha256=UBTzIhnncadfZ8YKJss0a3cFvrTVznmt_KgpdkbA7k4,29878
 nodalize/data_management/local_file_data_manager.py,sha256=3NudiFcGQmlYrHRHhMwQyVwf4ZJCF2Nz7pu7IxLSj-o,8213
 nodalize/data_management/s3_file_data_manager.py,sha256=KpLMPflzpxE1QLXLSeR5jz9l3jK01m6Kf-cg24pTUUM,8415
 nodalize/data_management/sqlite_data_manager.py,sha256=kAdaTvWRm7QurO4c5tDDXhCtNQUsuSWXT4Po2j4XwO0,15158
 nodalize/orchestration/__init__.py,sha256=QE8--MA0Su_FC-SGDKl5cffA2CST6Nf0AOEoBH_eRO0,47
 nodalize/orchestration/calculator_factory.py,sha256=zRigEqh86zJmAJrKfWrwn9A58JKGsAViuS4FfVFt2vg,2899
-nodalize/orchestration/coordinator.py,sha256=niodS8VvV_oks83zzcxgzOBiXWUS4gQtQgA4OXQZaH8,11867
+nodalize/orchestration/coordinator.py,sha256=ulF4nnUr0scW_hOI_EOvyWydG_qc3I4WvVAJYcIRcyM,12816
 nodalize/orchestration/data_manager_factory.py,sha256=MlUXqUstl0OFHmzxkwsssAJBofPwg1GSl6bM6B_hTvo,1784
 nodalize/orchestration/data_node_cache.py,sha256=sDBxAALhC5kykWQjcjzYxtUQVPAIpM9jpvh3cN456VA,3790
 nodalize/tools/__init__.py,sha256=t0FXjajsgg9zvYX5RZhatciX_tr8651HVfknbs0GEIM,37
 nodalize/tools/dates.py,sha256=BOJ3JKqxBUFkyUi6PkXsyTXOxIw5je9aLm7p0FVxkNQ,1942
 nodalize/tools/static_func_tools.py,sha256=XMMF22Ttq_aIceG9k8qlM1I42e2Wxl1ib_YJxD7jeYo,1772
 nodalize/tools/tree.py,sha256=L-xcKZ6P7EVr6j6DPj0fadzN8cJ7faJZgILPLniV4I0,4112
 sandbox/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sandbox/test_anything.py,sha256=P_sAKUwuWtO-D4saI3NSNxOtPwWh_vkZuqy_OmfbUzk,81
-nodalize-1.0.1.dist-info/LICENSE,sha256=JSLRq56-S2ilfHCBH-UGSgrmg1Wpdsgz7Ju9IkY9Qtc,1060
-nodalize-1.0.1.dist-info/METADATA,sha256=MbMrWbHKeGeaXgB1xr8Q6wzQlzM7MHDVL9vz6Wp4lBU,6033
-nodalize-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-nodalize-1.0.1.dist-info/top_level.txt,sha256=PkmomGh5hRDE5vnV0L74Ke3gk-7n0Pj5qyNLXvGV3s0,17
-nodalize-1.0.1.dist-info/RECORD,,
+nodalize-1.0.2.dist-info/LICENSE,sha256=JSLRq56-S2ilfHCBH-UGSgrmg1Wpdsgz7Ju9IkY9Qtc,1060
+nodalize-1.0.2.dist-info/METADATA,sha256=ZVRnz_BAI1E46Jzj9u9HErsFI7mvsogaG7mpUocxuC8,6033
+nodalize-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+nodalize-1.0.2.dist-info/top_level.txt,sha256=PkmomGh5hRDE5vnV0L74Ke3gk-7n0Pj5qyNLXvGV3s0,17
+nodalize-1.0.2.dist-info/RECORD,,
```

