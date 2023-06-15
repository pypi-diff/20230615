# Comparing `tmp/cvxrisk-0.0.2.tar.gz` & `tmp/cvxrisk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxrisk-0.0.2.tar", max compression
+gzip compressed data, was "cvxrisk-0.0.3.tar", max compression
```

## Comparing `cvxrisk-0.0.2.tar` & `cvxrisk-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0    11375 2023-06-14 05:23:32.191506 cvxrisk-0.0.2/LICENSE
--rw-r--r--   0        0        0     4855 2023-06-14 05:23:32.191506 cvxrisk-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-06-14 05:23:32.195506 cvxrisk-0.0.2/cvx/risk/__init__.py
--rw-r--r--   0        0        0       83 2023-06-14 05:23:32.195506 cvxrisk-0.0.2/cvx/risk/cvar/__init__.py
--rw-r--r--   0        0        0      705 2023-06-14 05:23:32.195506 cvxrisk-0.0.2/cvx/risk/cvar/cvar.py
--rw-r--r--   0        0        0      162 2023-06-14 05:23:32.195506 cvxrisk-0.0.2/cvx/risk/factor/__init__.py
--rw-r--r--   0        0        0      755 2023-06-14 05:23:32.195506 cvxrisk-0.0.2/cvx/risk/factor/_model.py
--rw-r--r--   0        0        0      498 2023-06-14 05:23:32.195506 cvxrisk-0.0.2/cvx/risk/factor/fundamental.py
--rw-r--r--   0        0        0        0 2023-06-14 05:23:32.195506 cvxrisk-0.0.2/cvx/risk/factor/linalg/__init__.py
--rw-r--r--   0        0        0      820 2023-06-14 05:23:32.195506 cvxrisk-0.0.2/cvx/risk/factor/linalg/pca.py
--rw-r--r--   0        0        0     1655 2023-06-14 05:23:32.195506 cvxrisk-0.0.2/cvx/risk/factor/timeseries.py
--rw-r--r--   0        0        0        0 2023-06-14 05:23:32.195506 cvxrisk-0.0.2/cvx/risk/factor/util/__init__.py
--rw-r--r--   0        0        0      343 2023-06-14 05:23:32.195506 cvxrisk-0.0.2/cvx/risk/model.py
--rw-r--r--   0        0        0      142 2023-06-14 05:23:32.195506 cvxrisk-0.0.2/cvx/risk/sample/__init__.py
--rw-r--r--   0        0        0      914 2023-06-14 05:23:32.195506 cvxrisk-0.0.2/cvx/risk/sample/sample.py
--rw-r--r--   0        0        0      581 2023-06-14 05:24:06.360278 cvxrisk-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5463 1970-01-01 00:00:00.000000 cvxrisk-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11375 2023-06-15 00:11:52.856834 cvxrisk-0.0.3/LICENSE
+-rw-r--r--   0        0        0     4832 2023-06-15 00:11:52.856834 cvxrisk-0.0.3/README.md
+-rw-r--r--   0        0        0       97 2023-06-15 00:11:52.860834 cvxrisk-0.0.3/cvx/risk/__init__.py
+-rw-r--r--   0        0        0       83 2023-06-15 00:11:52.860834 cvxrisk-0.0.3/cvx/risk/cvar/__init__.py
+-rw-r--r--   0        0        0      705 2023-06-15 00:11:52.860834 cvxrisk-0.0.3/cvx/risk/cvar/cvar.py
+-rw-r--r--   0        0        0      162 2023-06-15 00:11:52.860834 cvxrisk-0.0.3/cvx/risk/factor/__init__.py
+-rw-r--r--   0        0        0      755 2023-06-15 00:11:52.860834 cvxrisk-0.0.3/cvx/risk/factor/_model.py
+-rw-r--r--   0        0        0      498 2023-06-15 00:11:52.860834 cvxrisk-0.0.3/cvx/risk/factor/fundamental.py
+-rw-r--r--   0        0        0        0 2023-06-15 00:11:52.860834 cvxrisk-0.0.3/cvx/risk/factor/linalg/__init__.py
+-rw-r--r--   0        0        0      820 2023-06-15 00:11:52.860834 cvxrisk-0.0.3/cvx/risk/factor/linalg/pca.py
+-rw-r--r--   0        0        0     1655 2023-06-15 00:11:52.860834 cvxrisk-0.0.3/cvx/risk/factor/timeseries.py
+-rw-r--r--   0        0        0      343 2023-06-15 00:11:52.860834 cvxrisk-0.0.3/cvx/risk/model.py
+-rw-r--r--   0        0        0      142 2023-06-15 00:11:52.860834 cvxrisk-0.0.3/cvx/risk/sample/__init__.py
+-rw-r--r--   0        0        0      914 2023-06-15 00:11:52.860834 cvxrisk-0.0.3/cvx/risk/sample/sample.py
+-rw-r--r--   0        0        0      581 2023-06-15 00:12:25.752431 cvxrisk-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 cvxrisk-0.0.3/PKG-INFO
```

### Comparing `cvxrisk-0.0.2/LICENSE` & `cvxrisk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxrisk-0.0.2/README.md` & `cvxrisk-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -73,37 +73,34 @@
 
 
 ### Factor risk models
 
 Factor risk models use the projection of the weight vector into a lower
 dimensional subspace, e.g. each asset is the linear combination of $k$ factors.
 ```math
-r_i = \sum_{j=1}^k \beta_{ij} f_j + \epsilon_i
+r_i = \sum_{j=1}^k f_j \beta_{ji} + \epsilon_i
 ```
-XXX: Check whether $\beta_{ij}$ or $\beta_{ji}$.
-The factor time series are $f_1, \ldots, f_k$. The loadings are the coefficients $\beta_{ij}$.
+The factor time series are $f_1, \ldots, f_k$. The loadings are the coefficients $\beta_{ji}$.
 The residual returns $\epsilon_i$ are assumed to be uncorrelated with the factors.
 
-Any position $w$ in weight space corresponds to a position $f = \beta w$ in factor space.
+Any position $w$ in weight space projects to a position $y = \beta w$ in factor space.
 Factor space has only $k$ dimensions, whereas weight space has $n$ dimensions.
 The variance for a position $w$ is the sum of the variance of the
 systemic returns explained by the factors and the variance by the idiosyncratic returns.
 
 ```math
 Var(r) = Var(\beta w) + Var(\epsilon w)
 ```
 
 We assume the residual returns are uncorrelated and hence
 
 ```math
-Var(r) = f^T \Sigma_f f + \sum_i w_i^2 Var(\epsilon_i)
+Var(r) = y^T \Sigma_f y + \sum_i w_i^2 Var(\epsilon_i)
 ```
 
-XXX: Explore alignment of equations.
-
 where $\Sigma_f$ is the covariance matrix of the factors and $Var(\epsilon_i)$
 is the variance of the idiosyncratic returns.
 
 Again we offer two variants of the factor risk model reflecting what is widely used in practice.
 The first variant is the `FundamentalFactorRiskModel` class.
 Here the user provides the factor covariance matrix $\Sigma_f$,
 the loadings $\beta$ and the volatilities of the idiosyncratic returns $\epsilon_i$. Often such
@@ -113,14 +110,16 @@
 Here the user provides the factor time series $f_1, \ldots, f_k$, usually obtained from
 a principal component analysis (PCA) of the asset returns. The loadings $\beta$ are computed
 via a linear regression of the asset returns on the factor time series.
 The volatilities of the idiosyncratic returns $\epsilon_i$ are computed as the standard deviation
 of the residuals of the linear regression.
 The factor covariance matrix $\Sigma_f$ may even be diagonal in this case as the factors are orthogonal.
 
+We expose a method to compute the first $k$ principal components.
+
 ### cvar
 
 XXX: Conditional value at risk
 Relies on cxxpy's `sum_largest` function.
```

### Comparing `cvxrisk-0.0.2/cvx/risk/cvar/cvar.py` & `cvxrisk-0.0.3/cvx/risk/cvar/cvar.py`

 * *Files identical despite different names*

### Comparing `cvxrisk-0.0.2/cvx/risk/factor/_model.py` & `cvxrisk-0.0.3/cvx/risk/factor/_model.py`

 * *Files identical despite different names*

### Comparing `cvxrisk-0.0.2/cvx/risk/factor/linalg/pca.py` & `cvxrisk-0.0.3/cvx/risk/factor/linalg/pca.py`

 * *Files identical despite different names*

### Comparing `cvxrisk-0.0.2/cvx/risk/factor/timeseries.py` & `cvxrisk-0.0.3/cvx/risk/factor/timeseries.py`

 * *Files identical despite different names*

### Comparing `cvxrisk-0.0.2/cvx/risk/sample/sample.py` & `cvxrisk-0.0.3/cvx/risk/sample/sample.py`

 * *Files identical despite different names*

### Comparing `cvxrisk-0.0.2/pyproject.toml` & `cvxrisk-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cvxrisk"
-version = "v0.0.2"
+version = "v0.0.3"
 description = "Simple riskengine for cvxpy"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/cvxrisk"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cvxrisk-0.0.2/PKG-INFO` & `cvxrisk-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxrisk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple riskengine for cvxpy
 Home-page: https://github.com/cvxgrp/cvxrisk
 Author: Thomas Schmelzer
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -91,37 +91,34 @@
 
 
 ### Factor risk models
 
 Factor risk models use the projection of the weight vector into a lower
 dimensional subspace, e.g. each asset is the linear combination of $k$ factors.
 ```math
-r_i = \sum_{j=1}^k \beta_{ij} f_j + \epsilon_i
+r_i = \sum_{j=1}^k f_j \beta_{ji} + \epsilon_i
 ```
-XXX: Check whether $\beta_{ij}$ or $\beta_{ji}$.
-The factor time series are $f_1, \ldots, f_k$. The loadings are the coefficients $\beta_{ij}$.
+The factor time series are $f_1, \ldots, f_k$. The loadings are the coefficients $\beta_{ji}$.
 The residual returns $\epsilon_i$ are assumed to be uncorrelated with the factors.
 
-Any position $w$ in weight space corresponds to a position $f = \beta w$ in factor space.
+Any position $w$ in weight space projects to a position $y = \beta w$ in factor space.
 Factor space has only $k$ dimensions, whereas weight space has $n$ dimensions.
 The variance for a position $w$ is the sum of the variance of the
 systemic returns explained by the factors and the variance by the idiosyncratic returns.
 
 ```math
 Var(r) = Var(\beta w) + Var(\epsilon w)
 ```
 
 We assume the residual returns are uncorrelated and hence
 
 ```math
-Var(r) = f^T \Sigma_f f + \sum_i w_i^2 Var(\epsilon_i)
+Var(r) = y^T \Sigma_f y + \sum_i w_i^2 Var(\epsilon_i)
 ```
 
-XXX: Explore alignment of equations.
-
 where $\Sigma_f$ is the covariance matrix of the factors and $Var(\epsilon_i)$
 is the variance of the idiosyncratic returns.
 
 Again we offer two variants of the factor risk model reflecting what is widely used in practice.
 The first variant is the `FundamentalFactorRiskModel` class.
 Here the user provides the factor covariance matrix $\Sigma_f$,
 the loadings $\beta$ and the volatilities of the idiosyncratic returns $\epsilon_i$. Often such
@@ -131,14 +128,16 @@
 Here the user provides the factor time series $f_1, \ldots, f_k$, usually obtained from
 a principal component analysis (PCA) of the asset returns. The loadings $\beta$ are computed
 via a linear regression of the asset returns on the factor time series.
 The volatilities of the idiosyncratic returns $\epsilon_i$ are computed as the standard deviation
 of the residuals of the linear regression.
 The factor covariance matrix $\Sigma_f$ may even be diagonal in this case as the factors are orthogonal.
 
+We expose a method to compute the first $k$ principal components.
+
 ### cvar
 
 XXX: Conditional value at risk
 Relies on cxxpy's `sum_largest` function.
```

