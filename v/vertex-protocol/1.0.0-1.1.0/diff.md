# Comparing `tmp/vertex_protocol-1.0.0.tar.gz` & `tmp/vertex_protocol-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vertex_protocol-1.0.0.tar", max compression
+gzip compressed data, was "vertex_protocol-1.1.0.tar", max compression
```

## Comparing `vertex_protocol-1.0.0.tar` & `vertex_protocol-1.1.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     3338 2023-06-11 00:18:19.920212 vertex_protocol-1.0.0/README.md
--rw-r--r--   0        0        0     1665 2023-06-11 00:18:19.924212 vertex_protocol-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-11 00:18:19.924212 vertex_protocol-1.0.0/vertex_protocol/__init__.py
--rw-r--r--   0        0        0     6628 2023-06-11 00:18:19.924212 vertex_protocol-1.0.0/vertex_protocol/client/__init__.py
--rw-r--r--   0        0        0      580 2023-06-11 00:18:19.924212 vertex_protocol-1.0.0/vertex_protocol/client/apis/__init__.py
--rw-r--r--   0        0        0     1394 2023-06-11 00:18:19.924212 vertex_protocol-1.0.0/vertex_protocol/client/apis/base.py
--rw-r--r--   0        0        0     1108 2023-06-11 00:18:19.924212 vertex_protocol-1.0.0/vertex_protocol/client/apis/market/__init__.py
--rw-r--r--   0        0        0     3404 2023-06-11 00:18:19.924212 vertex_protocol-1.0.0/vertex_protocol/client/apis/market/execute.py
--rw-r--r--   0        0        0    10070 2023-06-11 00:18:19.924212 vertex_protocol-1.0.0/vertex_protocol/client/apis/market/query.py
--rw-r--r--   0        0        0      746 2023-06-11 00:18:19.924212 vertex_protocol-1.0.0/vertex_protocol/client/apis/perp/__init__.py
--rw-r--r--   0        0        0     1438 2023-06-11 00:18:19.924212 vertex_protocol-1.0.0/vertex_protocol/client/apis/perp/query.py
--rw-r--r--   0        0        0     1027 2023-06-11 00:18:19.924212 vertex_protocol-1.0.0/vertex_protocol/client/apis/spot/__init__.py
--rw-r--r--   0        0        0     1191 2023-06-11 00:18:19.924212 vertex_protocol-1.0.0/vertex_protocol/client/apis/spot/base.py
--rw-r--r--   0        0        0     4745 2023-06-11 00:18:19.924212 vertex_protocol-1.0.0/vertex_protocol/client/apis/spot/execute.py
--rw-r--r--   0        0        0     2933 2023-06-11 00:18:19.924212 vertex_protocol-1.0.0/vertex_protocol/client/apis/spot/query.py
--rw-r--r--   0        0        0     1307 2023-06-11 00:18:19.924212 vertex_protocol-1.0.0/vertex_protocol/client/apis/subaccount/__init__.py
--rw-r--r--   0        0        0     2023 2023-06-11 00:18:19.924212 vertex_protocol-1.0.0/vertex_protocol/client/apis/subaccount/execute.py
--rw-r--r--   0        0        0     3162 2023-06-11 00:18:19.924212 vertex_protocol-1.0.0/vertex_protocol/client/apis/subaccount/query.py
--rw-r--r--   0        0        0     2551 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/client/context.py
--rw-r--r--   0        0        0     8264 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/contracts/__init__.py
--rw-r--r--   0        0        0    11702 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/contracts/abis/Endpoint.json
--rw-r--r--   0        0        0    55374 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/contracts/abis/FQuerier.json
--rw-r--r--   0        0        0    16980 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/contracts/abis/IClearinghouse.json
--rw-r--r--   0        0        0     3385 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/contracts/abis/IERC20.json
--rw-r--r--   0        0        0     4723 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/contracts/abis/IEndpoint.json
--rw-r--r--   0        0        0    13112 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/contracts/abis/IOffchainBook.json
--rw-r--r--   0        0        0    21812 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/contracts/abis/IPerpEngine.json
--rw-r--r--   0        0        0     8410 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/contracts/abis/IProductEngine.json
--rw-r--r--   0        0        0    18858 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/contracts/abis/ISpotEngine.json
--rw-r--r--   0        0        0     5698 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/contracts/abis/MockERC20.json
--rw-r--r--   0        0        0     1013 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json
--rw-r--r--   0        0        0      993 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json
--rw-r--r--   0        0        0      908 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/contracts/deployments/deployment.test.json
--rw-r--r--   0        0        0      426 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/contracts/eip712/__init__.py
--rw-r--r--   0        0        0     1189 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/contracts/eip712/domain.py
--rw-r--r--   0        0        0     2484 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/contracts/eip712/sign.py
--rw-r--r--   0        0        0     4636 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/contracts/eip712/types.py
--rw-r--r--   0        0        0     1526 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/contracts/loader.py
--rw-r--r--   0        0        0     2747 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/contracts/types.py
--rw-r--r--   0        0        0     1127 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/engine_client/__init__.py
--rw-r--r--   0        0        0    18437 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/engine_client/execute.py
--rw-r--r--   0        0        0    11077 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/engine_client/query.py
--rw-r--r--   0        0        0     5739 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/engine_client/types/__init__.py
--rw-r--r--   0        0        0    18331 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/engine_client/types/execute.py
--rw-r--r--   0        0        0     3426 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/engine_client/types/models.py
--rw-r--r--   0        0        0     9473 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/engine_client/types/query.py
--rw-r--r--   0        0        0      926 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/indexer_client/__init__.py
--rw-r--r--   0        0        0    11025 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/indexer_client/query.py
--rw-r--r--   0        0        0     2979 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/indexer_client/types/__init__.py
--rw-r--r--   0        0        0     5588 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/indexer_client/types/models.py
--rw-r--r--   0        0        0    12079 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/indexer_client/types/query.py
--rw-r--r--   0        0        0      933 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/utils/__init__.py
--rw-r--r--   0        0        0      341 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/utils/backend.py
--rw-r--r--   0        0        0     5216 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/utils/bytes32.py
--rw-r--r--   0        0        0       99 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/utils/enum.py
--rw-r--r--   0        0        0     1136 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/utils/exceptions.py
--rw-r--r--   0        0        0     1094 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/utils/expiration.py
--rw-r--r--   0        0        0      927 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/utils/math.py
--rw-r--r--   0        0        0     1887 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/utils/model.py
--rw-r--r--   0        0        0      809 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/utils/nonce.py
--rw-r--r--   0        0        0      491 2023-06-11 00:18:19.928212 vertex_protocol-1.0.0/vertex_protocol/utils/subaccount.py
--rw-r--r--   0        0        0     4071 1970-01-01 00:00:00.000000 vertex_protocol-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3337 2023-06-15 02:42:30.431570 vertex_protocol-1.1.0/README.md
+-rw-r--r--   0        0        0     1664 2023-06-15 02:42:30.435571 vertex_protocol-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-15 02:42:30.435571 vertex_protocol-1.1.0/vertex_protocol/__init__.py
+-rw-r--r--   0        0        0     6634 2023-06-15 02:42:30.435571 vertex_protocol-1.1.0/vertex_protocol/client/__init__.py
+-rw-r--r--   0        0        0      580 2023-06-15 02:42:30.435571 vertex_protocol-1.1.0/vertex_protocol/client/apis/__init__.py
+-rw-r--r--   0        0        0     1394 2023-06-15 02:42:30.435571 vertex_protocol-1.1.0/vertex_protocol/client/apis/base.py
+-rw-r--r--   0        0        0     1108 2023-06-15 02:42:30.435571 vertex_protocol-1.1.0/vertex_protocol/client/apis/market/__init__.py
+-rw-r--r--   0        0        0     3404 2023-06-15 02:42:30.435571 vertex_protocol-1.1.0/vertex_protocol/client/apis/market/execute.py
+-rw-r--r--   0        0        0    10101 2023-06-15 02:42:30.435571 vertex_protocol-1.1.0/vertex_protocol/client/apis/market/query.py
+-rw-r--r--   0        0        0      746 2023-06-15 02:42:30.435571 vertex_protocol-1.1.0/vertex_protocol/client/apis/perp/__init__.py
+-rw-r--r--   0        0        0     1438 2023-06-15 02:42:30.435571 vertex_protocol-1.1.0/vertex_protocol/client/apis/perp/query.py
+-rw-r--r--   0        0        0     1027 2023-06-15 02:42:30.435571 vertex_protocol-1.1.0/vertex_protocol/client/apis/spot/__init__.py
+-rw-r--r--   0        0        0     1191 2023-06-15 02:42:30.435571 vertex_protocol-1.1.0/vertex_protocol/client/apis/spot/base.py
+-rw-r--r--   0        0        0     4782 2023-06-15 02:42:30.435571 vertex_protocol-1.1.0/vertex_protocol/client/apis/spot/execute.py
+-rw-r--r--   0        0        0     2964 2023-06-15 02:42:30.435571 vertex_protocol-1.1.0/vertex_protocol/client/apis/spot/query.py
+-rw-r--r--   0        0        0     1307 2023-06-15 02:42:30.435571 vertex_protocol-1.1.0/vertex_protocol/client/apis/subaccount/__init__.py
+-rw-r--r--   0        0        0     2023 2023-06-15 02:42:30.435571 vertex_protocol-1.1.0/vertex_protocol/client/apis/subaccount/execute.py
+-rw-r--r--   0        0        0     3193 2023-06-15 02:42:30.435571 vertex_protocol-1.1.0/vertex_protocol/client/apis/subaccount/query.py
+-rw-r--r--   0        0        0     2554 2023-06-15 02:42:30.435571 vertex_protocol-1.1.0/vertex_protocol/client/context.py
+-rw-r--r--   0        0        0     8264 2023-06-15 02:42:30.435571 vertex_protocol-1.1.0/vertex_protocol/contracts/__init__.py
+-rw-r--r--   0        0        0    11702 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/contracts/abis/Endpoint.json
+-rw-r--r--   0        0        0    55374 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/contracts/abis/FQuerier.json
+-rw-r--r--   0        0        0    16980 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/contracts/abis/IClearinghouse.json
+-rw-r--r--   0        0        0     3385 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/contracts/abis/IERC20.json
+-rw-r--r--   0        0        0     4723 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/contracts/abis/IEndpoint.json
+-rw-r--r--   0        0        0    13112 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/contracts/abis/IOffchainBook.json
+-rw-r--r--   0        0        0    21812 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/contracts/abis/IPerpEngine.json
+-rw-r--r--   0        0        0     8410 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/contracts/abis/IProductEngine.json
+-rw-r--r--   0        0        0    18858 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/contracts/abis/ISpotEngine.json
+-rw-r--r--   0        0        0     5698 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/contracts/abis/MockERC20.json
+-rw-r--r--   0        0        0     1013 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json
+-rw-r--r--   0        0        0      993 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json
+-rw-r--r--   0        0        0      908 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/contracts/deployments/deployment.test.json
+-rw-r--r--   0        0        0      426 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/contracts/eip712/__init__.py
+-rw-r--r--   0        0        0     1189 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/contracts/eip712/domain.py
+-rw-r--r--   0        0        0     2484 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/contracts/eip712/sign.py
+-rw-r--r--   0        0        0     4636 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/contracts/eip712/types.py
+-rw-r--r--   0        0        0     1526 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/contracts/loader.py
+-rw-r--r--   0        0        0     2747 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/contracts/types.py
+-rw-r--r--   0        0        0     1127 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/engine_client/__init__.py
+-rw-r--r--   0        0        0    18507 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/engine_client/execute.py
+-rw-r--r--   0        0        0    11206 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/engine_client/query.py
+-rw-r--r--   0        0        0     5739 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/engine_client/types/__init__.py
+-rw-r--r--   0        0        0    18440 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/engine_client/types/execute.py
+-rw-r--r--   0        0        0     3429 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/engine_client/types/models.py
+-rw-r--r--   0        0        0     9598 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/engine_client/types/query.py
+-rw-r--r--   0        0        0      926 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/indexer_client/__init__.py
+-rw-r--r--   0        0        0    11233 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/indexer_client/query.py
+-rw-r--r--   0        0        0     2979 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/indexer_client/types/__init__.py
+-rw-r--r--   0        0        0     5625 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/indexer_client/types/models.py
+-rw-r--r--   0        0        0    12117 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/indexer_client/types/query.py
+-rw-r--r--   0        0        0      933 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/utils/__init__.py
+-rw-r--r--   0        0        0      341 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/utils/backend.py
+-rw-r--r--   0        0        0     5301 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/utils/bytes32.py
+-rw-r--r--   0        0        0       99 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/utils/enum.py
+-rw-r--r--   0        0        0     1136 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/utils/exceptions.py
+-rw-r--r--   0        0        0     1094 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/utils/expiration.py
+-rw-r--r--   0        0        0      927 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/utils/math.py
+-rw-r--r--   0        0        0     2089 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/utils/model.py
+-rw-r--r--   0        0        0      843 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/utils/nonce.py
+-rw-r--r--   0        0        0      503 2023-06-15 02:42:30.439571 vertex_protocol-1.1.0/vertex_protocol/utils/subaccount.py
+-rw-r--r--   0        0        0     4119 1970-01-01 00:00:00.000000 vertex_protocol-1.1.0/PKG-INFO
```

### Comparing `vertex_protocol-1.0.0/README.md` & `vertex_protocol-1.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This is the Python SDK for the [Vertex Protocol API](https://vertex-protocol.gitbook.io/docs/developer-resources/api).
 
 See [SDK docs](https://vertex-protocol.github.io/vertex-python-sdk/index.html) to get started.
 
 ## Requirements
 
-- Python 3.10 or above
+- Python 3.9 or above
 
 ## Installation
 
 You can install the SDK via pip:
 
 ```bash
 pip install vertex-protocol
```

### Comparing `vertex_protocol-1.0.0/pyproject.toml` & `vertex_protocol-1.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "vertex-protocol"
-version = "1.0.0"
+version = "1.1.0"
 description = "Vertex Protocol SDK"
 authors = ["Jeury Mejia <jeury@vertexprotocol.com>"]
 homepage = "https://vertexprotocol.com/"
 maintainers = [
   "Frank Jia <frank@vertexprotocol.com>",
   "Clark Oh-Willeke <clark@vertexprotocol.com>"
 ]
 documentation = "https://vertex-protocol.github.io/vertex-python-sdk/"
 readme = "README.md"
 packages = [{include = "vertex_protocol"}]
 include = ["vertex_protocol/*.json"]
 keywords = ["vertex protocol", "vertex sdk", "vertex protocol api"]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 pydantic = "^1.10.7"
 web3 = "^6.4.0"
 eth-account = "^0.8.0"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "*"
 black = "*"
```

### Comparing `vertex_protocol-1.0.0/vertex_protocol/client/__init__.py` & `vertex_protocol-1.1.0/vertex_protocol/client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,16 +81,16 @@
         self.subaccount = SubaccountAPI(context)
         self.spot = SpotAPI(context)
         self.perp = PerpAPI(context)
 
 
 def create_vertex_client(
     mode: VertexClientMode,
-    signer: Signer | None = None,
-    context_opts: VertexClientContextOpts | None = None,
+    signer: Optional[Signer] = None,
+    context_opts: Optional[VertexClientContextOpts] = None,
 ) -> VertexClient:
     """
     Create a new VertexClient based on the given mode and signer.
 
     This function will create a new VertexClientContext based on the provided mode, and then
     initialize a new VertexClient with that context.
```

### Comparing `vertex_protocol-1.0.0/vertex_protocol/client/apis/__init__.py` & `vertex_protocol-1.1.0/vertex_protocol/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/client/apis/base.py` & `vertex_protocol-1.1.0/vertex_protocol/client/apis/base.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/client/apis/market/__init__.py` & `vertex_protocol-1.1.0/vertex_protocol/client/apis/market/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/client/apis/market/execute.py` & `vertex_protocol-1.1.0/vertex_protocol/client/apis/market/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/client/apis/market/query.py` & `vertex_protocol-1.1.0/vertex_protocol/client/apis/market/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Optional
 from vertex_protocol.client.apis.base import VertexBaseAPI
 from vertex_protocol.engine_client.types.query import (
     AllProductsData,
     MarketLiquidityData,
     MarketPriceData,
     MaxLpMintableData,
     MaxOrderSizeData,
@@ -147,15 +148,15 @@
 
         Returns:
             MaxOrderSizeData: The maximum size of the order that can be placed.
         """
         return self.context.engine_client.get_max_order_size(params)
 
     def get_max_lp_mintable(
-        self, product_id: int, sender: str, spot_leverage: bool | None = None
+        self, product_id: int, sender: str, spot_leverage: Optional[bool] = None
     ) -> MaxLpMintableData:
         """
         Queries the engine to determine the maximum base amount that can be contributed for minting LPs.
 
         Args:
             product_id (int): The identifier for the spot/perp product.
```

### Comparing `vertex_protocol-1.0.0/vertex_protocol/client/apis/perp/__init__.py` & `vertex_protocol-1.1.0/vertex_protocol/client/apis/perp/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/client/apis/perp/query.py` & `vertex_protocol-1.1.0/vertex_protocol/client/apis/perp/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/client/apis/spot/__init__.py` & `vertex_protocol-1.1.0/vertex_protocol/client/apis/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/client/apis/spot/base.py` & `vertex_protocol-1.1.0/vertex_protocol/client/apis/spot/base.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/client/apis/spot/execute.py` & `vertex_protocol-1.1.0/vertex_protocol/client/apis/spot/execute.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Optional
 from vertex_protocol.contracts.types import DepositCollateralParams
 from eth_account.signers.local import LocalAccount
 from vertex_protocol.client.apis.spot.base import BaseSpotAPI
 from vertex_protocol.engine_client.types.execute import (
     ExecuteResponse,
     WithdrawCollateralParams,
 )
@@ -16,15 +17,15 @@
     such as depositing a specified amount into a spot product.
 
     Inheritance:
         BaseSpotAPI: Base class for Spot operations. Inherits connectivity context and base functionalities.
     """
 
     def deposit(
-        self, params: DepositCollateralParams, signer: LocalAccount | None = None
+        self, params: DepositCollateralParams, signer: Optional[LocalAccount] = None
     ) -> str:
         """
         Executes the operation of depositing a specified amount into a spot product.
 
         Args:
             params (DepositCollateralParams): Parameters required for depositing collateral.
 
@@ -55,15 +56,15 @@
 
         Raises:
             Exception: If there is an error during the execution or the response status is not "success".
         """
         return self.context.engine_client.withdraw_collateral(params)
 
     def approve_allowance(
-        self, product_id: int, amount: int, signer: LocalAccount | None = None
+        self, product_id: int, amount: int, signer: Optional[LocalAccount] = None
     ) -> str:
         """
         Approves an allowance for a certain amount of tokens for a spot product.
 
         Args:
             product_id (int): The identifier of the spot product for which to approve an allowance.
 
@@ -83,15 +84,15 @@
             raise MissingSignerException(
                 "A signer must be provided or set via the context."
             )
         token = self.get_token_contract_for_product(product_id)
         return self.context.contracts.approve_allowance(token, amount, signer)
 
     def _mint_mock_erc20(
-        self, product_id: int, amount: int, signer: LocalAccount | None = None
+        self, product_id: int, amount: int, signer: Optional[LocalAccount] = None
     ):
         """
         Mints a specified amount of mock ERC20 tokens for testing purposes.
 
         Args:
             product_id (int): The identifier for the spot product.
```

### Comparing `vertex_protocol-1.0.0/vertex_protocol/client/apis/spot/query.py` & `vertex_protocol-1.1.0/vertex_protocol/client/apis/spot/query.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Optional
 from vertex_protocol.client.apis.spot.base import BaseSpotAPI
 from vertex_protocol.engine_client.types.query import MaxWithdrawableData
 from vertex_protocol.utils.math import from_pow_10
 
 
 class SpotQueryAPI(BaseSpotAPI):
     """
@@ -11,15 +12,15 @@
     such as getting wallet token balance of a given spot product.
 
     Inheritance:
         BaseSpotAPI: Base class for Spot operations. Inherits connectivity context and base functionalities.
     """
 
     def get_max_withdrawable(
-        self, product_id: int, sender: str, spot_leverage: bool | None = None
+        self, product_id: int, sender: str, spot_leverage: Optional[bool] = None
     ) -> MaxWithdrawableData:
         """
         Retrieves the estimated maximum withdrawable amount for a provided spot product.
 
         Args:
             product_id (int): The identifier for the spot product.
```

### Comparing `vertex_protocol-1.0.0/vertex_protocol/client/apis/subaccount/__init__.py` & `vertex_protocol-1.1.0/vertex_protocol/client/apis/subaccount/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/client/apis/subaccount/execute.py` & `vertex_protocol-1.1.0/vertex_protocol/client/apis/subaccount/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/client/apis/subaccount/query.py` & `vertex_protocol-1.1.0/vertex_protocol/client/apis/subaccount/query.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Optional
 from vertex_protocol.client.apis.base import VertexBaseAPI
 from vertex_protocol.engine_client.types.query import (
     FeeRatesData,
     QuerySubaccountInfoTx,
     SubaccountInfoData,
 )
 from vertex_protocol.indexer_client.types.query import (
@@ -18,15 +19,15 @@
     This class extends the base class to provide specific functionalities for querying data related to subaccounts.
 
     Attributes:
         context (VertexClientContext): Provides connectivity details for accessing Vertex APIs.
     """
 
     def get_engine_subaccount_summary(
-        self, subaccount: str, txs: list[QuerySubaccountInfoTx] | None = None
+        self, subaccount: str, txs: Optional[list[QuerySubaccountInfoTx]] = None
     ) -> SubaccountInfoData:
         """
         Retrieve a comprehensive summary of the specified subaccount's state as per the off-chain engine.
 
         You can optionally provide a list of txs to get an estimated view of your subaccount.
 
         Args:
```

### Comparing `vertex_protocol-1.0.0/vertex_protocol/client/context.py` & `vertex_protocol-1.1.0/vertex_protocol/client/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     contracts_context: VertexContractsContext
     rpc_node_url: AnyUrl
     engine_endpoint_url: AnyUrl
     indexer_endpoint_url: AnyUrl
 
 
 def create_vertex_client_context(
-    opts: VertexClientContextOpts, signer: Signer | None = None
+    opts: VertexClientContextOpts, signer: Optional[Signer] = None
 ) -> VertexClientContext:
     """
     Initializes a VertexClientContext instance with the provided signer and options.
 
     Args:
         opts (VertexClientContextOpts): Options including endpoints for the engine and indexer clients.
```

### Comparing `vertex_protocol-1.0.0/vertex_protocol/contracts/__init__.py` & `vertex_protocol-1.1.0/vertex_protocol/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/contracts/abis/Endpoint.json` & `vertex_protocol-1.1.0/vertex_protocol/contracts/abis/Endpoint.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/contracts/abis/FQuerier.json` & `vertex_protocol-1.1.0/vertex_protocol/contracts/abis/FQuerier.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/contracts/abis/IClearinghouse.json` & `vertex_protocol-1.1.0/vertex_protocol/contracts/abis/IClearinghouse.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/contracts/abis/IERC20.json` & `vertex_protocol-1.1.0/vertex_protocol/contracts/abis/IERC20.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/contracts/abis/IEndpoint.json` & `vertex_protocol-1.1.0/vertex_protocol/contracts/abis/IEndpoint.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/contracts/abis/IOffchainBook.json` & `vertex_protocol-1.1.0/vertex_protocol/contracts/abis/IOffchainBook.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/contracts/abis/IPerpEngine.json` & `vertex_protocol-1.1.0/vertex_protocol/contracts/abis/IPerpEngine.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/contracts/abis/IProductEngine.json` & `vertex_protocol-1.1.0/vertex_protocol/contracts/abis/IProductEngine.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/contracts/abis/ISpotEngine.json` & `vertex_protocol-1.1.0/vertex_protocol/contracts/abis/ISpotEngine.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/contracts/abis/MockERC20.json` & `vertex_protocol-1.1.0/vertex_protocol/contracts/abis/MockERC20.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json` & `vertex_protocol-1.1.0/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json` & `vertex_protocol-1.1.0/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/contracts/deployments/deployment.test.json` & `vertex_protocol-1.1.0/vertex_protocol/contracts/deployments/deployment.test.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/contracts/eip712/domain.py` & `vertex_protocol-1.1.0/vertex_protocol/contracts/eip712/domain.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/contracts/eip712/sign.py` & `vertex_protocol-1.1.0/vertex_protocol/contracts/eip712/sign.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/contracts/eip712/types.py` & `vertex_protocol-1.1.0/vertex_protocol/contracts/eip712/types.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/contracts/loader.py` & `vertex_protocol-1.1.0/vertex_protocol/contracts/loader.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/contracts/types.py` & `vertex_protocol-1.1.0/vertex_protocol/contracts/types.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/engine_client/__init__.py` & `vertex_protocol-1.1.0/vertex_protocol/engine_client/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/engine_client/execute.py` & `vertex_protocol-1.1.0/vertex_protocol/engine_client/execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from copy import deepcopy
 import requests
 from functools import singledispatchmethod
 
-from typing import Type
+from typing import Optional, Type, Union
 from eth_account.signers.local import LocalAccount
 from vertex_protocol.contracts.eip712.sign import (
     get_eip712_typed_data_digest,
     sign_eip712_typed_data,
     build_eip712_typed_data,
 )
 from vertex_protocol.engine_client.query import EngineQueryClient
@@ -31,26 +31,26 @@
 )
 from vertex_protocol.contracts.types import VertexExecuteType
 
 from vertex_protocol.utils.exceptions import (
     BadStatusCodeException,
     ExecuteFailedException,
 )
-from vertex_protocol.utils.model import VertexBaseModel
+from vertex_protocol.utils.model import VertexBaseModel, is_instance_of_union
 from vertex_protocol.utils.nonce import gen_order_nonce
 from vertex_protocol.utils.subaccount import SubaccountParams
 
 
 class EngineExecuteClient:
     """
     Client class for executing operations against the off-chain engine.
     """
 
     def __init__(
-        self, opts: EngineClientOpts, querier: EngineQueryClient | None = None
+        self, opts: EngineClientOpts, querier: Optional[EngineQueryClient] = None
     ):
         """
         Initialize the EngineExecuteClient with provided options.
 
         Args:
             opts (EngineClientOpts): Options for the client.
 
@@ -97,15 +97,15 @@
         Get the transaction nonce. Used to perform executes such as `withdraw_collateral`.
 
         Returns:
             int: The transaction nonce.
         """
         return int(self._querier.get_nonces(self.signer.address).tx_nonce)
 
-    def order_nonce(self, recv_time_ms: int | None = None) -> int:
+    def order_nonce(self, recv_time_ms: Optional[int] = None) -> int:
         """
         Generate the order nonce. Used for oder placements and cancellations.
 
         Args:
             recv_time_ms (int, optional): Received time in milliseconds.
 
         Returns:
@@ -125,26 +125,26 @@
         """
         params = deepcopy(params)
         params = self._inject_owner_if_needed(params)
         params = self._inject_nonce_if_needed(params)
         return params
 
     @singledispatchmethod
-    def execute(self, params: ExecuteParams | ExecuteRequest) -> ExecuteResponse:
+    def execute(self, params: Union[ExecuteParams, ExecuteRequest]) -> ExecuteResponse:
         """
         Executes the operation defined by the provided parameters.
 
         Args:
             params (ExecuteParams): The parameters for the operation to execute. This can represent a variety of operations, such as placing orders, cancelling orders, and more.
 
         Returns:
             ExecuteResponse: The response from the executed operation.
         """
         req: ExecuteRequest = (
-            params if isinstance(params, ExecuteRequest) else to_execute_request(params)  # type: ignore
+            params if is_instance_of_union(params, ExecuteRequest) else to_execute_request(params)  # type: ignore
         )
         return self._execute(req)
 
     @execute.register
     def _(self, req: dict) -> ExecuteResponse:
         """
         Overloaded method to execute the operation defined by the provided request.
@@ -206,15 +206,15 @@
     @property
     def chain_id(self) -> int:
         if self._opts.chain_id is None:
             raise AttributeError("Chain ID is not set.")
         return self._opts.chain_id
 
     @chain_id.setter
-    def chain_id(self, chain_id: int | str) -> None:
+    def chain_id(self, chain_id: Union[int, str]) -> None:
         self._opts.chain_id = int(chain_id)
 
     @property
     def signer(self) -> LocalAccount:
         if self._opts.signer is None:
             raise AttributeError("Signer is not set.")
         assert isinstance(self._opts.signer, LocalAccount)
@@ -277,15 +277,15 @@
             VertexExecuteType.PLACE_ORDER,
             order.dict(),
             self.book_addr(product_id),
             self.chain_id,
         )
 
     def _sign(
-        self, execute: VertexExecuteType, msg: dict, product_id: int | None = None
+        self, execute: VertexExecuteType, msg: dict, product_id: Optional[int] = None
     ) -> str:
         """
         Internal method to create an EIP-712 signature for the given operation type and message.
 
         Args:
             execute (VertexExecuteType): The Vertex execute type to sign.
```

### Comparing `vertex_protocol-1.0.0/vertex_protocol/engine_client/query.py` & `vertex_protocol-1.1.0/vertex_protocol/engine_client/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Optional
 import requests
 from urllib.parse import urlencode
 
 from vertex_protocol.engine_client import EngineClientOpts
 from vertex_protocol.engine_client.types.query import (
     AllProductsData,
     ContractsData,
@@ -72,15 +73,18 @@
         Raises:
             BadStatusCodeException: If the response status code is not 200.
             QueryFailedException: If the query status is not "success".
         """
         res = requests.get(f"{self.url}/query?{urlencode(req.dict())}")
         if res.status_code != 200:
             raise BadStatusCodeException(res.text)
-        query_res = QueryResponse(**res.json())
+        try:
+            query_res = QueryResponse(**res.json())
+        except Exception:
+            raise QueryFailedException(res.text)
         if query_res.status != "success":
             raise QueryFailedException(res.text)
         return query_res
 
     def get_status(self) -> StatusData:
         """
         Query the engine for its status.
@@ -129,15 +133,15 @@
         """
         return ensure_data_type(
             self.query(QueryOrderParams(product_id=product_id, digest=digest)).data,
             OrderData,
         )
 
     def get_subaccount_info(
-        self, subaccount: str, txs: list[QuerySubaccountInfoTx] | None = None
+        self, subaccount: str, txs: Optional[list[QuerySubaccountInfoTx]] = None
     ) -> SubaccountInfoData:
         """
         Query the engine for the state of a subaccount, including balances.
 
         Args:
             subaccount (str): Identifier of the subaccount (owner's address + subaccount name) sent as a hex string.
 
@@ -234,15 +238,15 @@
             for the given subaccount and product.
         """
         return ensure_data_type(
             self.query(QueryMaxOrderSizeParams.parse_obj(params)).data, MaxOrderSizeData
         )
 
     def get_max_withdrawable(
-        self, product_id: int, sender: str, spot_leverage: bool | None = None
+        self, product_id: int, sender: str, spot_leverage: Optional[bool] = None
     ) -> MaxWithdrawableData:
         """
         Retrieves the maximum withdrawable amount for a given spot product for a subaccount.
 
         Args:
             product_id (int): ID of the spot product.
 
@@ -259,15 +263,15 @@
                     product_id=product_id, sender=sender, spot_leverage=spot_leverage
                 )
             ).data,
             MaxWithdrawableData,
         )
 
     def get_max_lp_mintable(
-        self, product_id: int, sender: str, spot_leverage: bool | None = None
+        self, product_id: int, sender: str, spot_leverage: Optional[bool] = None
     ) -> MaxLpMintableData:
         """
         Retrieves the maximum LP token amount mintable for a given product for a subaccount.
 
         Args:
             product_id (int): ID of the product.
```

### Comparing `vertex_protocol-1.0.0/vertex_protocol/engine_client/types/__init__.py` & `vertex_protocol-1.1.0/vertex_protocol/engine_client/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/engine_client/types/execute.py` & `vertex_protocol-1.1.0/vertex_protocol/engine_client/types/execute.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from typing import Optional, Type
+from typing import Optional, Type, Union
 from pydantic import validator
 from vertex_protocol.contracts.types import VertexExecuteType
 from vertex_protocol.engine_client.types.models import ResponseStatus
 from vertex_protocol.utils.model import VertexBaseModel
 from vertex_protocol.utils.bytes32 import (
     bytes32_to_hex,
     hex_to_bytes32,
     subaccount_to_bytes32,
 )
 from vertex_protocol.utils.nonce import gen_order_nonce
 from vertex_protocol.utils.subaccount import Subaccount, SubaccountParams
 
 
-Digest = str | bytes
+Digest = Union[str, bytes]
 
 
 class BaseParams(VertexBaseModel):
     """
     Base class for defining request parameters to be sent to the Vertex API.
 
     Attributes:
@@ -30,15 +30,15 @@
     sender: Subaccount
     nonce: Optional[int]
 
     class Config:
         validate_assignment = True
 
     @validator("sender")
-    def serialize_sender(cls, v: Subaccount) -> bytes | Subaccount:
+    def serialize_sender(cls, v: Subaccount) -> Union[bytes, Subaccount]:
         """
         Validates and serializes the sender to bytes32 format.
 
         Args:
             v (Subaccount): The sender's subaccount identifier.
 
         Returns:
@@ -252,24 +252,24 @@
     signer: Subaccount
 
     @validator("signer")
     def serialize_signer(cls, v: Subaccount) -> bytes:
         return subaccount_to_bytes32(v)
 
 
-ExecuteParams = (
-    PlaceOrderParams
-    | CancelOrdersParams
-    | CancelProductOrdersParams
-    | WithdrawCollateralParams
-    | LiquidateSubaccountParams
-    | MintLpParams
-    | BurnLpParams
-    | LinkSignerParams
-)
+ExecuteParams = Union[
+    PlaceOrderParams,
+    CancelOrdersParams,
+    CancelProductOrdersParams,
+    WithdrawCollateralParams,
+    LiquidateSubaccountParams,
+    MintLpParams,
+    BurnLpParams,
+    LinkSignerParams,
+]
 
 
 class PlaceOrderRequest(VertexBaseModel):
     """
     Parameters for a request to place an order.
 
     Attributes:
@@ -524,24 +524,24 @@
     def serialize(cls, v: LinkSignerParams) -> LinkSignerParams:
         v.serialize_dict(["signer"], bytes32_to_hex)
         return v
 
     _validator = validator("link_signer", allow_reuse=True)(to_tx_request)
 
 
-ExecuteRequest = (
-    PlaceOrderRequest
-    | CancelOrdersRequest
-    | CancelProductOrdersRequest
-    | WithdrawCollateralRequest
-    | LiquidateSubaccountRequest
-    | MintLpRequest
-    | BurnLpRequest
-    | LinkSignerRequest
-)
+ExecuteRequest = Union[
+    PlaceOrderRequest,
+    CancelOrdersRequest,
+    CancelProductOrdersRequest,
+    WithdrawCollateralRequest,
+    LiquidateSubaccountRequest,
+    MintLpRequest,
+    BurnLpRequest,
+    LinkSignerRequest,
+]
 
 
 class ExecuteResponse(VertexBaseModel):
     """
     Represents the response returned from executing a request.
 
     Attributes:
@@ -549,21 +549,24 @@
 
         signature (Optional[str]): The signature of the response. Only present if the request was successfully executed.
 
         error_code (Optional[int]): The error code, if any error occurred during the execution of the request.
 
         error (Optional[str]): The error message, if any error occurred during the execution of the request.
 
+        request_type (Optional[str]): Type of the request.
+
         req (Optional[dict]): The original request that was executed.
     """
 
     status: ResponseStatus
     signature: Optional[str]
     error_code: Optional[int]
     error: Optional[str]
+    request_type: Optional[str]
     req: Optional[dict]
 
 
 def to_execute_request(params: ExecuteParams) -> ExecuteRequest:
     """
     Maps `ExecuteParams` to its corresponding `ExecuteRequest` object based on the parameter type.
```

### Comparing `vertex_protocol-1.0.0/vertex_protocol/engine_client/types/models.py` & `vertex_protocol-1.1.0/vertex_protocol/engine_client/types/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 class PerpProductState(VertexBaseModel):
     cumulative_funding_long_x18: str
     cumulative_funding_short_x18: str
     available_settle: str
     open_interest: str
 
 
-class PerpProductLpState(VertexBaseModel):
+class PerpProductLpState(BaseProductLpState):
     last_cumulative_funding_x18: str
     cumulative_funding_per_lp_x18: str
     base: str
     quote: str
 
 
 class PerpProduct(BaseProduct):
```

### Comparing `vertex_protocol-1.0.0/vertex_protocol/engine_client/types/query.py` & `vertex_protocol-1.1.0/vertex_protocol/engine_client/types/query.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from vertex_protocol.utils.enum import StrEnum
-from typing import Optional
+from typing import Optional, Union
 from pydantic import validator
 from vertex_protocol.utils.model import VertexBaseModel
 from vertex_protocol.engine_client.types.models import (
     ApplyDeltaTx,
     BurnLpTx,
     EngineStatus,
     Liquidity,
@@ -71,15 +71,15 @@
     """
 
     type = EngineQueryType.ORDER.value
     product_id: int
     digest: str
 
 
-QuerySubaccountInfoTx = MintLpTx | BurnLpTx | ApplyDeltaTx
+QuerySubaccountInfoTx = Union[MintLpTx, BurnLpTx, ApplyDeltaTx]
 
 
 class QuerySubaccountInfoParams(VertexBaseModel):
     """
     Parameters for querying the subaccount summary from engine, including balances.
     """
 
@@ -186,31 +186,31 @@
     Parameters for querying the signer linked to a specified subaccount.
     """
 
     type = EngineQueryType.LINKED_SIGNER.value
     subaccount: str
 
 
-QueryRequest = (
-    QueryStatusParams
-    | QueryContractsParams
-    | QueryNoncesParams
-    | QueryOrderParams
-    | QuerySubaccountInfoParams
-    | QuerySubaccountOpenOrdersParams
-    | QueryMarketLiquidityParams
-    | QueryAllProductsParams
-    | QueryMarketPriceParams
-    | QueryMaxOrderSizeParams
-    | QueryMaxWithdrawableParams
-    | QueryMaxLpMintableParams
-    | QueryFeeRatesParams
-    | QueryHealthGroupsParams
-    | QueryLinkedSignerParams
-)
+QueryRequest = Union[
+    QueryStatusParams,
+    QueryContractsParams,
+    QueryNoncesParams,
+    QueryOrderParams,
+    QuerySubaccountInfoParams,
+    QuerySubaccountOpenOrdersParams,
+    QueryMarketLiquidityParams,
+    QueryAllProductsParams,
+    QueryMarketPriceParams,
+    QueryMaxOrderSizeParams,
+    QueryMaxWithdrawableParams,
+    QueryMaxLpMintableParams,
+    QueryFeeRatesParams,
+    QueryHealthGroupsParams,
+    QueryLinkedSignerParams,
+]
 
 StatusData = EngineStatus
 
 
 class ContractsData(VertexBaseModel):
     """
     Data model for Vertex's contract addresses.
@@ -260,15 +260,15 @@
     spot_balances: list[SpotProductBalance]
     perp_balances: list[PerpProductBalance]
     spot_products: list[SpotProduct]
     perp_products: list[PerpProduct]
 
     def parse_subaccount_balance(
         self, product_id: int
-    ) -> SpotProductBalance | PerpProductBalance:
+    ) -> Union[SpotProductBalance, PerpProductBalance]:
         """
         Parses the balance of a subaccount for a given product.
 
         Args:
             product_id (int): The ID of the product to lookup.
 
         Returns:
@@ -345,14 +345,15 @@
 
 class MaxLpMintableData(VertexBaseModel):
     """
     Data model for the maximum liquidity that can be minted.
     """
 
     max_base_amount: str
+    max_quote_amount: str
 
 
 class FeeRatesData(VertexBaseModel):
     """
     Data model for various fee rates associated with transactions.
     """
 
@@ -376,37 +377,39 @@
     """
     Data model for the signer linked to a subaccount.
     """
 
     linked_signer: str
 
 
-QueryResponseData = (
-    StatusData
-    | ContractsData
-    | NoncesData
-    | OrderData
-    | SubaccountInfoData
-    | SubaccountOpenOrdersData
-    | MarketLiquidityData
-    | AllProductsData
-    | MarketPriceData
-    | MaxOrderSizeData
-    | MaxWithdrawableData
-    | MaxLpMintableData
-    | FeeRatesData
-    | HealthGroupsData
-    | LinkedSignerData
-)
+QueryResponseData = Union[
+    StatusData,
+    ContractsData,
+    NoncesData,
+    OrderData,
+    SubaccountInfoData,
+    SubaccountOpenOrdersData,
+    MarketLiquidityData,
+    AllProductsData,
+    MarketPriceData,
+    MaxOrderSizeData,
+    MaxWithdrawableData,
+    MaxLpMintableData,
+    FeeRatesData,
+    HealthGroupsData,
+    LinkedSignerData,
+]
 
 
 class QueryResponse(VertexBaseModel):
     """
     Represents a response to a query request.
 
     Attributes:
         status (ResponseStatus): The status of the query response.
         data (QueryResponseData | str): The data returned from the query, or an error message if the query failed.
+        request_type (Optional[str]): Type of the request.
     """
 
     status: ResponseStatus
-    data: QueryResponseData | str
+    request_type: Optional[str]
+    data: Union[QueryResponseData, str]
```

### Comparing `vertex_protocol-1.0.0/vertex_protocol/indexer_client/__init__.py` & `vertex_protocol-1.1.0/vertex_protocol/indexer_client/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/indexer_client/query.py` & `vertex_protocol-1.1.0/vertex_protocol/indexer_client/query.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Optional, Union
 import requests
 from functools import singledispatchmethod
 from vertex_protocol.indexer_client.types import IndexerClientOpts
 from vertex_protocol.indexer_client.types.query import (
     IndexerCandlesticksParams,
     IndexerCandlesticksData,
     IndexerEventsParams,
@@ -30,15 +31,19 @@
     IndexerResponse,
     IndexerSubaccountSummaryParams,
     IndexerSubaccountSummaryData,
     IndexerTokenRewardsData,
     IndexerTokenRewardsParams,
     to_indexer_request,
 )
-from vertex_protocol.utils.model import VertexBaseModel, ensure_data_type
+from vertex_protocol.utils.model import (
+    VertexBaseModel,
+    ensure_data_type,
+    is_instance_of_union,
+)
 
 
 class IndexerQueryClient:
     """
     Client for querying data from the indexer service.
 
     Attributes:
@@ -53,42 +58,46 @@
         Args:
             opts (IndexerClientOpts): Client configuration options for connecting and interacting with the indexer service.
         """
         self._opts = IndexerClientOpts.parse_obj(opts)
         self.url = self._opts.url
 
     @singledispatchmethod
-    def query(self, params: IndexerParams | IndexerRequest) -> IndexerResponse:
+    def query(self, params: Union[IndexerParams, IndexerRequest]) -> IndexerResponse:
         """
         Sends a query request to the indexer service and returns the response.
 
         The `query` method is overloaded to accept either `IndexerParams` or a dictionary or `IndexerRequest`
         as the input parameters. Based on the type of the input, the appropriate internal method is invoked
         to process the query request.
 
         Args:
             params (IndexerParams | dict | IndexerRequest): The parameters for the query request.
 
         Returns:
             IndexerResponse: The response from the indexer service.
         """
         req: IndexerRequest = (
-            params if isinstance(params, IndexerRequest) else to_indexer_request(params)  # type: ignore
+            params if is_instance_of_union(params, IndexerRequest) else to_indexer_request(params)  # type: ignore
         )
         return self._query(req)
 
     @query.register
     def _(self, req: dict) -> IndexerResponse:
         return self._query(VertexBaseModel.parse_obj(req))  # type: ignore
 
     def _query(self, req: IndexerRequest) -> IndexerResponse:
         res = requests.post(f"{self.url}/indexer", json=req.dict())
         if res.status_code != 200:
             raise Exception(res.text)
-        return IndexerResponse(data=res.json())
+        try:
+            indexer_res = IndexerResponse(data=res.json())
+        except Exception:
+            raise Exception(res.text)
+        return indexer_res
 
     def get_subaccount_historical_orders(
         self, params: IndexerSubaccountHistoricalOrdersParams
     ) -> IndexerHistoricalOrdersData:
         """
         Retrieves the historical orders associated with a specific subaccount.
 
@@ -145,15 +154,15 @@
             IndexerEventsData: The event data corresponding to the provided parameters.
         """
         return ensure_data_type(
             self.query(IndexerEventsParams.parse_obj(params)).data, IndexerEventsData
         )
 
     def get_subaccount_summary(
-        self, subaccount: str, timestamp: int | None = None
+        self, subaccount: str, timestamp: Optional[int] = None
     ) -> IndexerSubaccountSummaryData:
         """
         Retrieves a summary of a specified subaccount at a certain timestamp.
 
         Args:
             subaccount (str): The identifier for the subaccount.
```

### Comparing `vertex_protocol-1.0.0/vertex_protocol/indexer_client/types/__init__.py` & `vertex_protocol-1.1.0/vertex_protocol/indexer_client/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/indexer_client/types/models.py` & `vertex_protocol-1.1.0/vertex_protocol/indexer_client/types/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import IntEnum
 from vertex_protocol.utils.enum import StrEnum
 
-from typing import Any, Optional
+from typing import Any, Optional, Union
 from vertex_protocol.engine_client.types.models import (
     PerpProduct,
     PerpProductBalance,
     SpotProduct,
     SpotProductBalance,
 )
 
@@ -41,16 +41,16 @@
     timestamp: Optional[str]
 
 
 class IndexerBaseOrder(VertexBaseModel):
     sender: str
     priceX18: str
     amount: str
-    expiration: str | int
-    nonce: str | int
+    expiration: Union[str, int]
+    nonce: Union[str, int]
 
 
 class IndexerOrderFill(IndexerBaseModel):
     digest: str
     base_filled: str
     quote_filled: str
     fee: str
@@ -132,49 +132,49 @@
     nonce: int
 
 
 class IndexerBurnLpTx(VertexBaseModel):
     burn_lp: IndexerBurnLpTxData
 
 
-IndexerTxData = (
-    IndexerMatchOrdersTx
-    | IndexerWithdrawCollateralTx
-    | IndexerLiquidateSubaccountTx
-    | IndexerMintLpTx
-    | IndexerBurnLpTx
-)
+IndexerTxData = Union[
+    IndexerMatchOrdersTx,
+    IndexerWithdrawCollateralTx,
+    IndexerLiquidateSubaccountTx,
+    IndexerMintLpTx,
+    IndexerBurnLpTx,
+]
 
 
 class IndexerTx(IndexerBaseModel):
-    tx: IndexerTxData | Any
+    tx: Union[IndexerTxData, Any]
 
 
 class IndexerSpotProductBalanceData(VertexBaseModel):
     spot: SpotProductBalance
 
 
 class IndexerPerpProductBalanceData(VertexBaseModel):
     perp: PerpProductBalance
 
 
-IndexerProductBalanceData = (
-    IndexerSpotProductBalanceData | IndexerPerpProductBalanceData
-)
+IndexerProductBalanceData = Union[
+    IndexerSpotProductBalanceData, IndexerPerpProductBalanceData
+]
 
 
 class IndexerSpotProductData(VertexBaseModel):
     spot: SpotProduct
 
 
 class IndexerPerpProductData(VertexBaseModel):
     perp: PerpProduct
 
 
-IndexerProductData = IndexerSpotProductData | IndexerPerpProductData
+IndexerProductData = Union[IndexerSpotProductData, IndexerPerpProductData]
 
 
 class IndexerEventTrackedData(VertexBaseModel):
     net_interest_unrealized: str
     net_interest_cumulative: str
     net_funding_unrealized: str
     net_funding_cumulative: str
```

### Comparing `vertex_protocol-1.0.0/vertex_protocol/indexer_client/types/query.py` & `vertex_protocol-1.1.0/vertex_protocol/indexer_client/types/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from vertex_protocol.utils.enum import StrEnum
-from typing import Optional
+from typing import Optional, Union
 
 from pydantic import Field
 from vertex_protocol.indexer_client.types.models import (
     IndexerCandlestick,
     IndexerCandlesticksGranularity,
     IndexerEvent,
     IndexerEventType,
@@ -87,15 +87,15 @@
     """
     Parameters for limiting events by transaction count.
     """
 
     txs: int
 
 
-IndexerEventsLimit = IndexerEventsRawLimit | IndexerEventsTxsLimit
+IndexerEventsLimit = Union[IndexerEventsRawLimit, IndexerEventsTxsLimit]
 
 
 class IndexerEventsParams(IndexerBaseParams):
     """
     Parameters for querying events.
     """
 
@@ -188,38 +188,40 @@
     """
     Parameters for querying linked signer rate limits.
     """
 
     subaccount: str
 
 
-IndexerParams = (
-    IndexerSubaccountHistoricalOrdersParams
-    | IndexerHistoricalOrdersByDigestParams
-    | IndexerMatchesParams
-    | IndexerEventsParams
-    | IndexerSubaccountSummaryParams
-    | IndexerProductSnapshotsParams
-    | IndexerCandlesticksParams
-    | IndexerFundingRateParams
-    | IndexerPerpPricesParams
-    | IndexerOraclePricesParams
-    | IndexerTokenRewardsParams
-    | IndexerMakerStatisticsParams
-    | IndexerLiquidationFeedParams
-    | IndexerLinkedSignerRateLimitParams
-)
+IndexerParams = Union[
+    IndexerSubaccountHistoricalOrdersParams,
+    IndexerHistoricalOrdersByDigestParams,
+    IndexerMatchesParams,
+    IndexerEventsParams,
+    IndexerSubaccountSummaryParams,
+    IndexerProductSnapshotsParams,
+    IndexerCandlesticksParams,
+    IndexerFundingRateParams,
+    IndexerPerpPricesParams,
+    IndexerOraclePricesParams,
+    IndexerTokenRewardsParams,
+    IndexerMakerStatisticsParams,
+    IndexerLiquidationFeedParams,
+    IndexerLinkedSignerRateLimitParams,
+]
 
 
 class IndexerHistoricalOrdersRequest(VertexBaseModel):
     """
     Request object for querying historical orders.
     """
 
-    orders: IndexerSubaccountHistoricalOrdersParams | IndexerHistoricalOrdersByDigestParams
+    orders: Union[
+        IndexerSubaccountHistoricalOrdersParams, IndexerHistoricalOrdersByDigestParams
+    ]
 
 
 class IndexerMatchesRequest(VertexBaseModel):
     """
     Request object for querying matches.
     """
 
@@ -310,29 +312,29 @@
     """
     Request object for querying linked signer rate limits.
     """
 
     linked_signer_rate_limit: IndexerLinkedSignerRateLimitParams
 
 
-IndexerRequest = (
-    IndexerHistoricalOrdersRequest
-    | IndexerMatchesRequest
-    | IndexerEventsRequest
-    | IndexerSubaccountSummaryRequest
-    | IndexerProductSnapshotsRequest
-    | IndexerCandlesticksRequest
-    | IndexerFundingRateRequest
-    | IndexerPerpPricesRequest
-    | IndexerOraclePricesRequest
-    | IndexerTokenRewardsRequest
-    | IndexerMakerStatisticsRequest
-    | IndexerLiquidationFeedRequest
-    | IndexerLinkedSignerRateLimitRequest
-)
+IndexerRequest = Union[
+    IndexerHistoricalOrdersRequest,
+    IndexerMatchesRequest,
+    IndexerEventsRequest,
+    IndexerSubaccountSummaryRequest,
+    IndexerProductSnapshotsRequest,
+    IndexerCandlesticksRequest,
+    IndexerFundingRateRequest,
+    IndexerPerpPricesRequest,
+    IndexerOraclePricesRequest,
+    IndexerTokenRewardsRequest,
+    IndexerMakerStatisticsRequest,
+    IndexerLiquidationFeedRequest,
+    IndexerLinkedSignerRateLimitRequest,
+]
 
 
 class IndexerHistoricalOrdersData(VertexBaseModel):
     """
     Data object for historical orders.
     """
 
@@ -431,36 +433,37 @@
 
 class IndexerLinkedSignerRateLimitData(VertexBaseModel):
     """
     Data object for linked signer rate limits.
     """
 
     remaining_tx: str
+    total_tx_limit: str
     wait_time: int
     signer: str
 
 
 IndexerLiquidationFeedData = list[IndexerLiquidatableAccount]
 
 
-IndexerResponseData = (
-    IndexerHistoricalOrdersData
-    | IndexerMatchesData
-    | IndexerEventsData
-    | IndexerSubaccountSummaryData
-    | IndexerProductSnapshotsData
-    | IndexerCandlesticksData
-    | IndexerFundingRateData
-    | IndexerPerpPricesData
-    | IndexerOraclePricesData
-    | IndexerTokenRewardsData
-    | IndexerMakerStatisticsData
-    | IndexerLinkedSignerRateLimitData
-    | IndexerLiquidationFeedData
-)
+IndexerResponseData = Union[
+    IndexerHistoricalOrdersData,
+    IndexerMatchesData,
+    IndexerEventsData,
+    IndexerSubaccountSummaryData,
+    IndexerProductSnapshotsData,
+    IndexerCandlesticksData,
+    IndexerFundingRateData,
+    IndexerPerpPricesData,
+    IndexerOraclePricesData,
+    IndexerTokenRewardsData,
+    IndexerMakerStatisticsData,
+    IndexerLinkedSignerRateLimitData,
+    IndexerLiquidationFeedData,
+]
 
 
 class IndexerResponse(VertexBaseModel):
     """
     Represents the response returned by the indexer.
 
     Attributes:
```

### Comparing `vertex_protocol-1.0.0/vertex_protocol/utils/__init__.py` & `vertex_protocol-1.1.0/vertex_protocol/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/utils/bytes32.py` & `vertex_protocol-1.1.0/vertex_protocol/utils/bytes32.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import binascii
+from typing import Optional, Union
 from vertex_protocol.utils.subaccount import Subaccount, SubaccountParams
 
 
-def hex_to_bytes32(input: str | bytes) -> bytes:
+def hex_to_bytes32(input: Union[str, bytes]) -> bytes:
     """Converts a hexadecimal string or bytes to a bytes object of length 32.
 
     Args:
         input (str | bytes): The hexadecimal string or bytes to be converted.
 
     Returns:
         bytes: The converted bytes object of length 32.
     """
     return hex_to_bytes(input, 32)
 
 
-def hex_to_bytes12(input: str | bytes) -> bytes:
+def hex_to_bytes12(input: Union[str, bytes]) -> bytes:
     """Converts a hexadecimal string or bytes to a bytes object of length 12.
 
     Args:
         input (str | bytes): The hexadecimal string or bytes to be converted.
 
     Returns:
         bytes: The converted bytes object of length 12.
     """
     return hex_to_bytes(input, 12)
 
 
-def hex_to_bytes(input: str | bytes, size: int) -> bytes:
+def hex_to_bytes(input: Union[str, bytes], size: int) -> bytes:
     """Converts a hexadecimal string or bytes to a bytes object of specified size.
 
     Args:
         input (str | bytes): The hexadecimal string or bytes to be converted.
 
         size (int): The specified size for the output bytes object.
 
@@ -57,15 +58,15 @@
     Returns:
         str: The hexadecimal representation of the input string.
     """
     return binascii.hexlify(input.encode()).decode()
 
 
 def subaccount_to_bytes32(
-    subaccount: Subaccount, name: str | bytes | None = None
+    subaccount: Subaccount, name: Optional[Union[str, bytes]] = None
 ) -> bytes:
     """Converts a subaccount representation to a bytes object of length 32.
 
     Args:
         subaccount (Subaccount): The subaccount, which can be a string, bytes, or SubaccountParams instance.
 
         name (str|bytes, optional): The subaccount name, when provided `subaccount` is expected to be the owner address.
@@ -93,15 +94,17 @@
             raise ValueError("Missing `subaccount_owner` or `subaccount_name`")
         else:
             return hex_to_bytes32(subaccount_owner + str_to_hex(subaccount_name))
     else:
         return subaccount
 
 
-def subaccount_to_hex(subaccount: Subaccount, name: str | None = None) -> str:
+def subaccount_to_hex(
+    subaccount: Subaccount, name: Optional[Union[str, bytes]] = None
+) -> str:
     """Converts a subaccount representation to its hexadecimal representation.
 
     Args:
         subaccount (Subaccount): The subaccount, which can be a string, bytes, or SubaccountParams instance.
 
         name (str|bytes, optional): Additional string, if any, to be appended to the subaccount string before conversion. Defaults to None.
```

### Comparing `vertex_protocol-1.0.0/vertex_protocol/utils/exceptions.py` & `vertex_protocol-1.1.0/vertex_protocol/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/utils/expiration.py` & `vertex_protocol-1.1.0/vertex_protocol/utils/expiration.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/utils/math.py` & `vertex_protocol-1.1.0/vertex_protocol/utils/math.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.0.0/vertex_protocol/utils/model.py` & `vertex_protocol-1.1.0/vertex_protocol/utils/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from enum import Enum
 from pydantic import BaseModel
-from typing import Callable, Type, TypeVar
+from typing import Any, Callable, Type, TypeVar, Union
 
 
 class VertexBaseModel(BaseModel):
     """
     This base model extends Pydantic's BaseModel and excludes fields with None
     values by default when serializing via .dict() or .json()
     """
@@ -44,15 +44,15 @@
 
             func (Callable): Function to apply to each field.
         """
         for field in fields:
             self.__dict__[field] = func(self.__dict__[field])
 
 
-def parse_enum_value(value: str | Enum) -> str:
+def parse_enum_value(value: Union[str, Enum]) -> str:
     """
     Utility function to parse an enum value.
 
     Args:
         value (str | Enum): Original value which may be an Enum.
 
     Returns:
@@ -68,7 +68,12 @@
 
 
 def ensure_data_type(data, expected_type: Type[T]) -> T:
     assert isinstance(
         data, expected_type
     ), f"Expected {expected_type.__name__}, but got {type(data).__name__}"
     return data
+
+
+def is_instance_of_union(obj: Any, union) -> bool:
+    """Check if `obj` is an instance of any type in the `union`."""
+    return any(isinstance(obj, cls) for cls in union.__args__)
```

### Comparing `vertex_protocol-1.0.0/vertex_protocol/utils/nonce.py` & `vertex_protocol-1.1.0/vertex_protocol/utils/nonce.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+from typing import Optional
 import datetime
 import random
 
 
 def gen_order_nonce(
-    recv_time_ms: int | None = None, random_int: int | None = None
+    recv_time_ms: Optional[int] = None, random_int: Optional[int] = None
 ) -> int:
     """
     Generates an order nonce based on a received timestamp and a random integer.
 
     Args:
         recv_time_ms (int, optional): Received timestamp in milliseconds. Defaults to the current time plus 90 seconds.
```

### Comparing `vertex_protocol-1.0.0/PKG-INFO` & `vertex_protocol-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: vertex-protocol
-Version: 1.0.0
+Version: 1.1.0
 Summary: Vertex Protocol SDK
 Home-page: https://vertexprotocol.com/
 Keywords: vertex protocol,vertex sdk,vertex protocol api
 Author: Jeury Mejia
 Author-email: jeury@vertexprotocol.com
 Maintainer: Frank Jia
 Maintainer-email: frank@vertexprotocol.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: eth-account (>=0.8.0,<0.9.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: web3 (>=6.4.0,<7.0.0)
 Project-URL: Documentation, https://vertex-protocol.github.io/vertex-python-sdk/
 Description-Content-Type: text/markdown
@@ -22,15 +23,15 @@
 
 This is the Python SDK for the [Vertex Protocol API](https://vertex-protocol.gitbook.io/docs/developer-resources/api).
 
 See [SDK docs](https://vertex-protocol.github.io/vertex-python-sdk/index.html) to get started.
 
 ## Requirements
 
-- Python 3.10 or above
+- Python 3.9 or above
 
 ## Installation
 
 You can install the SDK via pip:
 
 ```bash
 pip install vertex-protocol
```

