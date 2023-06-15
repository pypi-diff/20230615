# Comparing `tmp/cvxportfolio-0.3.1.tar.gz` & `tmp/cvxportfolio-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxportfolio-0.3.1.tar", last modified: Tue May 16 17:39:56 2023, max compression
+gzip compressed data, was "cvxportfolio-0.3.2.tar", last modified: Thu Jun 15 03:37:08 2023, max compression
```

## Comparing `cvxportfolio-0.3.1.tar` & `cvxportfolio-0.3.2.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-05-16 17:39:56.418780 cvxportfolio-0.3.1/
--rw-r--r--   0 enzo       (501) staff       (20)      199 2023-04-08 05:48:25.000000 cvxportfolio-0.3.1/AUTHORS
--rw-r--r--   0 enzo       (501) staff       (20)      599 2023-04-08 05:48:25.000000 cvxportfolio-0.3.1/LICENSE
--rw-r--r--   0 enzo       (501) staff       (20)      329 2023-05-16 17:39:56.418449 cvxportfolio-0.3.1/PKG-INFO
--rw-r--r--   0 enzo       (501) staff       (20)     3650 2023-05-13 03:51:33.000000 cvxportfolio-0.3.1/README.md
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-05-16 17:39:56.396634 cvxportfolio-0.3.1/cvxportfolio/
--rw-r--r--   0 enzo       (501) staff       (20)      888 2023-05-16 17:39:49.000000 cvxportfolio-0.3.1/cvxportfolio/__init__.py
--rw-r--r--   0 enzo       (501) staff       (20)     6972 2023-05-12 04:06:18.000000 cvxportfolio-0.3.1/cvxportfolio/constraints.py
--rw-r--r--   0 enzo       (501) staff       (20)     9746 2023-05-12 05:19:45.000000 cvxportfolio-0.3.1/cvxportfolio/costs.py
--rw-r--r--   0 enzo       (501) staff       (20)    19617 2023-05-16 16:47:47.000000 cvxportfolio-0.3.1/cvxportfolio/data.py
--rw-r--r--   0 enzo       (501) staff       (20)     1004 2023-05-11 16:35:10.000000 cvxportfolio-0.3.1/cvxportfolio/errors.py
--rw-r--r--   0 enzo       (501) staff       (20)    10412 2023-05-16 16:47:47.000000 cvxportfolio-0.3.1/cvxportfolio/estimator.py
--rw-r--r--   0 enzo       (501) staff       (20)     7597 2023-05-16 17:30:00.000000 cvxportfolio-0.3.1/cvxportfolio/forecast.py
--rw-r--r--   0 enzo       (501) staff       (20)    19854 2023-05-11 19:03:54.000000 cvxportfolio-0.3.1/cvxportfolio/policies.py
--rw-r--r--   0 enzo       (501) staff       (20)     6959 2023-05-16 16:47:47.000000 cvxportfolio-0.3.1/cvxportfolio/result.py
--rw-r--r--   0 enzo       (501) staff       (20)    11140 2023-05-16 16:47:47.000000 cvxportfolio-0.3.1/cvxportfolio/returns.py
--rw-r--r--   0 enzo       (501) staff       (20)    20012 2023-05-16 16:47:47.000000 cvxportfolio-0.3.1/cvxportfolio/risks.py
--rw-r--r--   0 enzo       (501) staff       (20)    25533 2023-05-16 16:47:47.000000 cvxportfolio-0.3.1/cvxportfolio/simulator.py
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-05-16 17:39:56.416552 cvxportfolio-0.3.1/cvxportfolio/tests/
--rw-r--r--   0 enzo       (501) staff       (20)        0 2023-05-16 17:39:49.000000 cvxportfolio-0.3.1/cvxportfolio/tests/__init__.py
--rw-r--r--   0 enzo       (501) staff       (20)     1626 2023-05-11 16:35:10.000000 cvxportfolio-0.3.1/cvxportfolio/tests/base.py
--rw-r--r--   0 enzo       (501) staff       (20)   156730 2023-05-11 16:35:10.000000 cvxportfolio-0.3.1/cvxportfolio/tests/returns.csv
--rw-r--r--   0 enzo       (501) staff       (20)   149356 2023-05-11 16:35:10.000000 cvxportfolio-0.3.1/cvxportfolio/tests/sigmas.csv
--rw-r--r--   0 enzo       (501) staff       (20)     8855 2023-05-11 16:35:10.000000 cvxportfolio-0.3.1/cvxportfolio/tests/test_constraints.py
--rw-r--r--   0 enzo       (501) staff       (20)     8310 2023-05-16 16:47:47.000000 cvxportfolio-0.3.1/cvxportfolio/tests/test_costs.py
--rw-r--r--   0 enzo       (501) staff       (20)    10329 2023-05-11 16:35:10.000000 cvxportfolio-0.3.1/cvxportfolio/tests/test_data.py
--rw-r--r--   0 enzo       (501) staff       (20)     6718 2023-05-16 16:47:47.000000 cvxportfolio-0.3.1/cvxportfolio/tests/test_estimator.py
--rw-r--r--   0 enzo       (501) staff       (20)     6567 2023-05-16 16:47:47.000000 cvxportfolio-0.3.1/cvxportfolio/tests/test_forecast.py
--rw-r--r--   0 enzo       (501) staff       (20)    21909 2023-05-16 16:47:47.000000 cvxportfolio-0.3.1/cvxportfolio/tests/test_policies.py
--rw-r--r--   0 enzo       (501) staff       (20)     4381 2023-05-16 16:47:47.000000 cvxportfolio-0.3.1/cvxportfolio/tests/test_returns.py
--rw-r--r--   0 enzo       (501) staff       (20)     9070 2023-05-16 16:47:47.000000 cvxportfolio-0.3.1/cvxportfolio/tests/test_risks.py
--rw-r--r--   0 enzo       (501) staff       (20)    10591 2023-05-16 16:47:47.000000 cvxportfolio-0.3.1/cvxportfolio/tests/test_simulator.py
--rw-r--r--   0 enzo       (501) staff       (20)   116620 2023-05-11 16:35:10.000000 cvxportfolio-0.3.1/cvxportfolio/tests/volumes.csv
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-05-16 17:39:56.399470 cvxportfolio-0.3.1/cvxportfolio.egg-info/
--rw-r--r--   0 enzo       (501) staff       (20)      329 2023-05-16 17:39:56.000000 cvxportfolio-0.3.1/cvxportfolio.egg-info/PKG-INFO
--rw-r--r--   0 enzo       (501) staff       (20)      971 2023-05-16 17:39:56.000000 cvxportfolio-0.3.1/cvxportfolio.egg-info/SOURCES.txt
--rw-r--r--   0 enzo       (501) staff       (20)        1 2023-05-16 17:39:56.000000 cvxportfolio-0.3.1/cvxportfolio.egg-info/dependency_links.txt
--rw-r--r--   0 enzo       (501) staff       (20)       64 2023-05-16 17:39:56.000000 cvxportfolio-0.3.1/cvxportfolio.egg-info/requires.txt
--rw-r--r--   0 enzo       (501) staff       (20)       13 2023-05-16 17:39:56.000000 cvxportfolio-0.3.1/cvxportfolio.egg-info/top_level.txt
--rw-r--r--   0 enzo       (501) staff       (20)       38 2023-05-16 17:39:56.418868 cvxportfolio-0.3.1/setup.cfg
--rw-r--r--   0 enzo       (501) staff       (20)      788 2023-05-16 17:39:49.000000 cvxportfolio-0.3.1/setup.py
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-15 03:37:08.857925 cvxportfolio-0.3.2/
+-rw-r--r--   0 enzo       (501) staff       (20)      199 2023-04-08 05:48:25.000000 cvxportfolio-0.3.2/AUTHORS
+-rw-r--r--   0 enzo       (501) staff       (20)      599 2023-04-08 05:48:25.000000 cvxportfolio-0.3.2/LICENSE
+-rw-r--r--   0 enzo       (501) staff       (20)      329 2023-06-15 03:37:08.857583 cvxportfolio-0.3.2/PKG-INFO
+-rw-r--r--   0 enzo       (501) staff       (20)     5665 2023-05-30 16:04:26.000000 cvxportfolio-0.3.2/README.md
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-15 03:37:08.841769 cvxportfolio-0.3.2/cvxportfolio/
+-rw-r--r--   0 enzo       (501) staff       (20)      912 2023-06-15 03:37:01.000000 cvxportfolio-0.3.2/cvxportfolio/__init__.py
+-rw-r--r--   0 enzo       (501) staff       (20)     2053 2023-06-14 04:09:34.000000 cvxportfolio-0.3.2/cvxportfolio/benchmark.py
+-rw-r--r--   0 enzo       (501) staff       (20)    10850 2023-05-28 07:36:34.000000 cvxportfolio-0.3.2/cvxportfolio/constraints.py
+-rw-r--r--   0 enzo       (501) staff       (20)    14017 2023-06-14 04:09:34.000000 cvxportfolio-0.3.2/cvxportfolio/costs.py
+-rw-r--r--   0 enzo       (501) staff       (20)    20123 2023-06-10 04:38:54.000000 cvxportfolio-0.3.2/cvxportfolio/data.py
+-rw-r--r--   0 enzo       (501) staff       (20)     1004 2023-05-11 16:35:10.000000 cvxportfolio-0.3.2/cvxportfolio/errors.py
+-rw-r--r--   0 enzo       (501) staff       (20)    13721 2023-05-28 07:37:04.000000 cvxportfolio-0.3.2/cvxportfolio/estimator.py
+-rw-r--r--   0 enzo       (501) staff       (20)     9446 2023-06-10 04:38:54.000000 cvxportfolio-0.3.2/cvxportfolio/forecast.py
+-rw-r--r--   0 enzo       (501) staff       (20)    21131 2023-06-14 04:09:34.000000 cvxportfolio-0.3.2/cvxportfolio/policies.py
+-rw-r--r--   0 enzo       (501) staff       (20)     6483 2023-06-14 04:09:34.000000 cvxportfolio-0.3.2/cvxportfolio/result.py
+-rw-r--r--   0 enzo       (501) staff       (20)     8731 2023-06-15 03:34:41.000000 cvxportfolio-0.3.2/cvxportfolio/returns.py
+-rw-r--r--   0 enzo       (501) staff       (20)    17814 2023-06-14 04:09:34.000000 cvxportfolio-0.3.2/cvxportfolio/risks.py
+-rw-r--r--   0 enzo       (501) staff       (20)    35304 2023-06-14 04:09:34.000000 cvxportfolio-0.3.2/cvxportfolio/simulator.py
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-15 03:37:08.855323 cvxportfolio-0.3.2/cvxportfolio/tests/
+-rw-r--r--   0 enzo       (501) staff       (20)        0 2023-06-15 03:37:01.000000 cvxportfolio-0.3.2/cvxportfolio/tests/__init__.py
+-rw-r--r--   0 enzo       (501) staff       (20)     1623 2023-05-27 05:39:35.000000 cvxportfolio-0.3.2/cvxportfolio/tests/base.py
+-rw-r--r--   0 enzo       (501) staff       (20)   156730 2023-05-11 16:35:10.000000 cvxportfolio-0.3.2/cvxportfolio/tests/returns.csv
+-rw-r--r--   0 enzo       (501) staff       (20)   149356 2023-05-11 16:35:10.000000 cvxportfolio-0.3.2/cvxportfolio/tests/sigmas.csv
+-rw-r--r--   0 enzo       (501) staff       (20)     9929 2023-05-27 05:39:35.000000 cvxportfolio-0.3.2/cvxportfolio/tests/test_constraints.py
+-rw-r--r--   0 enzo       (501) staff       (20)     8359 2023-06-14 04:09:34.000000 cvxportfolio-0.3.2/cvxportfolio/tests/test_costs.py
+-rw-r--r--   0 enzo       (501) staff       (20)    10308 2023-05-27 05:39:35.000000 cvxportfolio-0.3.2/cvxportfolio/tests/test_data.py
+-rw-r--r--   0 enzo       (501) staff       (20)     6698 2023-05-27 05:39:35.000000 cvxportfolio-0.3.2/cvxportfolio/tests/test_estimator.py
+-rw-r--r--   0 enzo       (501) staff       (20)     8877 2023-06-10 04:38:54.000000 cvxportfolio-0.3.2/cvxportfolio/tests/test_forecast.py
+-rw-r--r--   0 enzo       (501) staff       (20)    21842 2023-06-14 04:09:34.000000 cvxportfolio-0.3.2/cvxportfolio/tests/test_policies.py
+-rw-r--r--   0 enzo       (501) staff       (20)     5754 2023-06-10 04:38:54.000000 cvxportfolio-0.3.2/cvxportfolio/tests/test_returns.py
+-rw-r--r--   0 enzo       (501) staff       (20)     9065 2023-05-27 05:39:35.000000 cvxportfolio-0.3.2/cvxportfolio/tests/test_risks.py
+-rw-r--r--   0 enzo       (501) staff       (20)    25275 2023-06-14 04:09:34.000000 cvxportfolio-0.3.2/cvxportfolio/tests/test_simulator.py
+-rw-r--r--   0 enzo       (501) staff       (20)   116620 2023-05-11 16:35:10.000000 cvxportfolio-0.3.2/cvxportfolio/tests/volumes.csv
+-rw-r--r--   0 enzo       (501) staff       (20)     1074 2023-06-14 04:09:34.000000 cvxportfolio-0.3.2/cvxportfolio/utils.py
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-15 03:37:08.843520 cvxportfolio-0.3.2/cvxportfolio.egg-info/
+-rw-r--r--   0 enzo       (501) staff       (20)      329 2023-06-15 03:37:08.000000 cvxportfolio-0.3.2/cvxportfolio.egg-info/PKG-INFO
+-rw-r--r--   0 enzo       (501) staff       (20)     1019 2023-06-15 03:37:08.000000 cvxportfolio-0.3.2/cvxportfolio.egg-info/SOURCES.txt
+-rw-r--r--   0 enzo       (501) staff       (20)        1 2023-06-15 03:37:08.000000 cvxportfolio-0.3.2/cvxportfolio.egg-info/dependency_links.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       59 2023-06-15 03:37:08.000000 cvxportfolio-0.3.2/cvxportfolio.egg-info/requires.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       13 2023-06-15 03:37:08.000000 cvxportfolio-0.3.2/cvxportfolio.egg-info/top_level.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       38 2023-06-15 03:37:08.858009 cvxportfolio-0.3.2/setup.cfg
+-rw-r--r--   0 enzo       (501) staff       (20)      783 2023-06-15 03:37:01.000000 cvxportfolio-0.3.2/setup.py
```

### Comparing `cvxportfolio-0.3.1/LICENSE` & `cvxportfolio-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.1/README.md` & `cvxportfolio-0.3.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -31,23 +31,31 @@
 python -m unittest discover cvxportfolio
 ```
 
 
 Example
 ------------
 To get a sneak preview of `cvxportfolio` you may try the following code. This is available in `examples/hello_world.py` and runs 
-with `cvxportfolio >= 0.3.0`
+with `cvxportfolio >= 0.3.0`. All objects in `cvxportfolio` can either be provided data (in a variety of forms, but preferably pandas
+series or dataframes) or infer/download it. For example in the following example, market data is downloaded by a public source
+(Yahoo finance) and the forecasts are computed iteratively, at each point in the backtest, from past data. The logic used
+matches what is described in Chapter 7 of the book. For example, returns are forecasted as the historical mean returns 
+and covariances as historical covariances (both ignoring `np.nan`'s). The logic used is detailed in the `forecast` module. Many optimizations
+are applied to make sure the system works well with real data. 
 
 
 ```python
 import cvxportfolio as cvx
 import matplotlib.pyplot as plt
 
-objective = cvx.ReturnsForecast() - 3 * (cvx.FullCovariance() + \
-	0.05 * cvx.RiskForecastError()) - cvx.TransactionCost()
+gamma = 3       # risk aversion parameter (Chapter 4.2)
+kappa = 0.05    # covariance forecast error risk parameter (Chapter 4.3)
+objective = cvx.ReturnsForecast() - gamma * (
+	cvx.FullCovariance() + kappa * cvx.RiskForecastError()
+) - cvx.TransactionCost()
 constraints = [cvx.LeverageLimit(3)]
 
 policy = cvx.MultiPeriodOptimization(objective, constraints, planning_horizon=2)
 
 simulator = cvx.MarketSimulator(['AAPL', 'AMZN', 'TSLA', 'GM', 'CVX', 'NKE'])
 
 result = simulator.backtest(policy, start_time='2020-01-01')
@@ -67,34 +75,57 @@
 
 print('\ntotal tcost ($)', result.tcost.sum())
 print('total borrow cost ($)', result.hcost_stocks.sum())
 print('total cash return + cost ($)', result.hcost_cash.sum())
 
 ```
 
+Development
+-----------
+Cvxportfolio is under development and things might change (quite fast), however you are (most) welcome to 
+read the code, play with it, and contribute. To set up a development environment locally you should
+
+```
+git clone https://github.com/cvxgrp/cvxportfolio.git
+cd cvxportfolio
+make env
+```
+This will replicate our [development environment](https://docs.python.org/3/library/venv.html). From there you can test with
+
+```
+make test
+```
+
+You activate the shell environment with one of scripts in `env/bin` (or `env\Scripts` on windows), for example if you use bash on POSIX
+```
+source env/bin/activate
+```
+and from the environment you can run any of the scripts in the examples (the cvxportfolio package is installed in [editable mode](https://setuptools.pypa.io/en/latest/userguide/development_mode.html)). 
+Or, if you don't want to activate the environment, you can just run scripts directly using `env/bin/python` or `env\Scripts\python` on windows, like we do in the Makefile.
+
+
 Examples from the book
---------------------
+----------------------
 In branch [0.0.X](https://github.com/cvxgrp/cvxportfolio/tree/0.0.X) you can find the original material used to generate plots
-and results in the book. 
+and results in the book. Those are being restored, and (slowly) translated in the new framework. As you may see from those
+ipython notebooks a lot of the logic that was implemented there, outside of cvxportfolio proper, is being included and made automatic
+in newer versions of cvxportfolio. 
 
 
 Academic
 ------------
 
 If you use `cvxportfolio` in your academic work please cite our book:
 ```
 @book{BBDKKNS:17,
     author       = {S. Boyd and E. Busseti and S. Diamond and R. Kahn and K. Koh and P. Nystrup and J. Speth},
     title        = {Multi-Period Trading via Convex Optimization},
-    journal      = {Foundations and Trends in Optimization},
+    series       = {Foundations and Trends in Optimization},
     year         = {2017},
     month        = {August},
-    volume       = {3},
-    number       = {1},
-    pages        = {1--76},
     publisher    = {Now Publishers},
     url          = {http://stanford.edu/~boyd/papers/cvx_portfolio.html},
 }
 ```
 
 
 License
```

### Comparing `cvxportfolio-0.3.1/cvxportfolio/__init__.py` & `cvxportfolio-0.3.2/cvxportfolio/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 from .data import *
 from .simulator import *
 from .result import *
 from .policies import *
 from .constraints import *
 from .costs import *
 from .returns import *
 from .estimator import DataEstimator
 from .risks import *
 from .returns import *
-
+from .benchmark import *
```

### Comparing `cvxportfolio-0.3.1/cvxportfolio/constraints.py` & `cvxportfolio-0.3.2/cvxportfolio/constraints.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,31 +12,36 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """This module implements realistic constraints to be used with SinglePeriodOptimization
 and MultiPeriodOptimization policies, or other Cvxpy-based policies.
 """
 
 
-import cvxpy as cvx
+import cvxpy as cp
 import numpy as np
 
-from .estimator import CvxpyExpressionEstimator, ParameterEstimator
-
+from .estimator import CvxpyExpressionEstimator, ParameterEstimator, DataEstimator
+from .forecast import HistoricalFactorizedCovariance
 
 __all__ = [
     "LongOnly",
     "LeverageLimit",
     "LongCash",
     "DollarNeutral",
     "ParticipationRateLimit",
     "MaxWeights",
     "MinWeights",
     "FactorMaxLimit",
     "FactorMinLimit",
     "FixedFactorLoading",
+    "MarketNeutral",
+    "MinWeightsAtTimes",
+    "MaxWeightsAtTimes",
+    "TurnoverLimit",
+    "MinCashBalance"
 ]
 
 
 class BaseConstraint(CvxpyExpressionEstimator):
     """Base cvxpy constraint class."""
 
 
@@ -52,14 +57,58 @@
     Here we can implement a method to pass benchmark weights
     and make the constraint relative to it rather than to the null
     portfolio.
     """
 
     pass
 
+class MarketNeutral(BaseWeightConstraint):
+    """Initial implementation of market neutrality.
+    
+    The benchmark portfolio weights are computed here 
+    (weighting by rolling averages of the market volumes)
+    but instead should be their own class (used as well
+    by risk models, ...).
+    """
+    
+    def __init__(self):
+        self.covarianceforecaster = HistoricalFactorizedCovariance()
+    
+    def pre_evaluation(self, universe, backtest_times):
+        super().pre_evaluation(universe=universe, backtest_times=backtest_times)
+        self.market_vector = cp.Parameter(len(universe)-1)
+    
+    def values_in_time(self, t, past_volumes, past_returns, **kwargs):
+        super().values_in_time(past_volumes=past_volumes, past_returns=past_returns, t=t, **kwargs)
+        tmp = past_volumes.iloc[-250:].mean()
+        tmp /= sum(tmp)
+        
+        tmp2 = self.covarianceforecaster.current_value @ (self.covarianceforecaster.current_value.T @ tmp)
+        # print(tmp2)
+        self.market_vector.value = np.array(tmp2)
+        
+    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+        return w_plus[:-1].T @ self.market_vector == 0
+        
+        
+class TurnoverLimit(BaseTradeConstraint):
+    """Turnover limit as a fraction of the portfolio value.
+    
+    See page 37 of the book.
+    
+    :param delta: constant or changing in time turnover limit 
+    :type delta: float or pd.Series 
+    """
+    
+    def __init__(self, delta):
+        self.delta = ParameterEstimator(delta)
+        
+    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+        return .5 * cp.norm1(z[:-1]) <= self.delta
+        
 
 class ParticipationRateLimit(BaseTradeConstraint):
     """A limit on maximum trades size as a fraction of market volumes.
     
 
     :param volumes: per-stock and per-day market volume estimates, or constant in time
     :type volumes: pd.Series or pd.DataFrame
@@ -67,23 +116,23 @@
     :type max_fraction_of_volumes: float, pd.Series, pd.DataFrame
     """
 
     def __init__(self, volumes, max_fraction_of_volumes=0.05):
         self.volumes = ParameterEstimator(volumes)
         self.max_participation_rate = ParameterEstimator(
             max_fraction_of_volumes)
-        self.portfolio_value = cvx.Parameter(nonneg=True)
+        self.portfolio_value = cp.Parameter(nonneg=True)
 
     def values_in_time(self, current_portfolio_value, **kwargs):
         self.portfolio_value.value = current_portfolio_value
         super().values_in_time(current_portfolio_value=current_portfolio_value, **kwargs)
         
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
-        return cvx.multiply(cvx.abs(z[:-1]), self.portfolio_value) <= cvx.multiply(
+        return cp.multiply(cp.abs(z[:-1]), self.portfolio_value) <= cp.multiply(
             self.volumes, self.max_participation_rate
         )
 
 
 class LongOnly(BaseWeightConstraint):
     """A long only constraint.
     
@@ -108,23 +157,45 @@
     """
 
     def __init__(self, limit):
         self.limit = ParameterEstimator(limit)
 
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
-        return cvx.norm(w_plus[:-1], 1) <= self.limit
+        return cp.norm(w_plus[:-1], 1) <= self.limit
 
 
-class LongCash(BaseWeightConstraint):
-    """Requires that cash be non-negative."""
-
+class MinCashBalance(BaseWeightConstraint):
+    """Requires that the cash account is larger than c_min dollars.
+    
+    This uses logic to subtract cash used as margin for the short 
+    positions that is not documented in the book but is
+    equivalent to the book definition's for long-only stock positions.
+    """
+    
+    def __init__(self, c_min):
+        self.c_min = DataEstimator(c_min)
+        self.rhs = cp.Parameter()
+    
+    def values_in_time(self, current_portfolio_value, **kwargs):
+        super().values_in_time(current_portfolio_value=current_portfolio_value, **kwargs)
+        self.rhs.value = self.c_min.current_value/current_portfolio_value
+    
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
-        return w_plus[-1] >= 0
+        # TODO clarify this
+        realcash = (w_plus[-1] - 2 * cp.sum(cp.neg(w_plus[:-1])))
+        return realcash >= self.rhs
+        
+    
+class LongCash(MinCashBalance):
+    """Requires that cash be non-negative."""
+    
+    def __init__(self):
+        super().__init__(0.)
 
 
 class DollarNeutral(BaseWeightConstraint):
     """Long-short dollar neutral strategy."""
 
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
@@ -156,14 +227,51 @@
     def __init__(self, limit):
         self.limit = ParameterEstimator(limit)
 
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return w_plus[:-1] >= self.limit
 
+class MinMaxWeightsAtTimes(BaseWeightConstraint):
+
+    def __init__(self, limit, times):
+        self.base_limit = limit
+        self.times = times
+    
+    def pre_evaluation(self, universe, backtest_times):
+        super().pre_evaluation(universe=universe, backtest_times = backtest_times)
+        self.backtest_times = backtest_times
+        self.limit = cp.Parameter()
+        
+    def values_in_time(self, t, mpo_step, **kwargs):
+        super().values_in_time(t=t, mpo_step=mpo_step, **kwargs)
+        tidx = self.backtest_times.get_loc(t)
+        nowtidx = tidx + mpo_step
+        if (nowtidx < len(self.backtest_times)) and self.backtest_times[nowtidx] in self.times:
+            self.limit.value = self.base_limit
+        else:
+            self.limit.value = 100 * self.sign
+
+
+class MinWeightsAtTimes(MinMaxWeightsAtTimes):
+    
+    sign = -1.
+
+    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+        """Return a Cvxpy constraint."""
+        return w_plus[:-1] >= self.limit
+        
+class MaxWeightsAtTimes(MinMaxWeightsAtTimes):
+
+    sign = 1.
+    
+    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+        """Return a Cvxpy constraint."""
+        return w_plus[:-1] <= self.limit
+        
 
 class FactorMaxLimit(BaseWeightConstraint):
     """A max limit on portfolio-wide factor (e.g. beta) exposure.
 
     Args:
         factor_exposure: An (n * r) matrix giving the factor exposure per asset
         per factor, where n represents # of assets and r represents # of factors
```

### Comparing `cvxportfolio-0.3.1/cvxportfolio/costs.py` & `cvxportfolio-0.3.2/cvxportfolio/costs.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,21 +16,22 @@
 
 Currently these are two: :class:`TransactionCost` and :class:`HoldingCost`.
 
 The default parameters are chosen to approximate real market costs as well as
 possible. 
 """
 
-import cvxpy as cvx
+import cvxpy as cp
 import numpy as np
 import pandas as pd
 import copy
+import inspect
 
 from .estimator import CvxpyExpressionEstimator, ParameterEstimator, DataEstimator
-
+from .utils import periods_per_year
 __all__ = ["HoldingCost", "TransactionCost"]
 
 
 class BaseCost(CvxpyExpressionEstimator):
     """Base class for cost objects (and also risks).
 
     Here there is some logic used to implement the algebraic operations.
@@ -84,16 +85,15 @@
     :var multipliers: floats that multiply the ``costs``
     :type var: list
     """
 
     def __init__(self, costs, multipliers):
         for cost in costs:
             if not isinstance(cost, BaseCost):
-                raise SyntaxError(
-      "You can only sum `BaseCost` instances to other `BaseCost` instances.")
+                raise SyntaxError("You can only sum `BaseCost` instances to other `BaseCost` instances.")
         self.costs = costs
         self.multipliers = multipliers
         
     def __add__(self, other):
         """Add other (combined) cost to self."""
         if isinstance(other, CombinedCosts):
             return CombinedCosts(self.costs + other.costs, self.multipliers + other.multipliers)
@@ -104,142 +104,215 @@
         """Multiply by constant."""
         return CombinedCosts(self.costs, [el * other for el in self.multipliers])
 
     def pre_evaluation(self, *args, **kwargs):
         """Iterate over constituent costs."""
         [el.pre_evaluation(*args, **kwargs) for el in self.costs]
 
-    def values_in_time(self, *args, **kwargs):
+    def values_in_time(self, **kwargs):
         """Iterate over constituent costs."""
-        [el.values_in_time(*args, **kwargs) for el in self.costs]
+        [el.values_in_time(**kwargs) for el in self.costs ]
 
     def compile_to_cvxpy(self, w_plus, z, portfolio_value):
         """Iterate over constituent costs."""
         self.expression = 0
         for multiplier, cost in zip(self.multipliers, self.costs):
-            self.expression += multiplier * \
-                cost.compile_to_cvxpy(w_plus, z, portfolio_value)
-
+            self.expression += multiplier * cost.compile_to_cvxpy(w_plus, z, portfolio_value) 
         return self.expression
 
 
 class HoldingCost(BaseCost):
     """A model for holding costs.
 
-    :param borrow_spread: spread on top of cash return payed for borrowing assets,
+    :param spread_on_borrowing_stocks_percent: spread on top of cash return payed for borrowing assets,
         including cash. If ``None``, the default, it gets from :class:`Backtest` the
         value for the period.
-    :type borrow_spread: float or pd.Series or pd.DataFrame or None
-    :param cash_lending_spread: spread that subtracts from the cash return for
-        uninvested cash. If ``None``, the default, it gets from :class:`Backtest` the
-        value for the period.
-    :type cash_lending_spread: float or pd.Series or None
+    :type spread_on_borrowing_stocks_percent: float or pd.Series or pd.DataFrame or None
+    :param spread_on_lending_cash_percent: spread that subtracts from the cash return for
+        uninvested cash.
+    :type spread_on_lending_cash_percent: float or pd.Series or None
+    :param spread_on_borrowing_cash_percent: spread that adds to the cash return as rate payed for
+        borrowed cash. This is not used as a policy optimization cost but is for the simulator cost.
+    :type spread_on_borrowing_cash_percent: float or pd.Series or None
     :param dividends: dividends payed (expressed as fraction of the stock value)
         for each period.  If ``None``, the default, it gets from :class:`Backtest` the
         value for the period.
     :type dividends: pd.DataFrame or None
+    :param periods_per_year: period per year (used in calculation of per-period cost). If None it is calculated
+        automatically.
+    :type periods_per_year: int or None
+    :param cash_return_on_borrow: whether to add (negative of) cash return to borrow cost of assets
+    :type cash_return_on_borrow: bool
     """
 
     def __init__(self, 
         spread_on_borrowing_stocks_percent=.5,
-        dividends=None,
-        ):
+        spread_on_lending_cash_percent=.5,
+        spread_on_borrowing_cash_percent=.5,
+        periods_per_year=None,
+        cash_return_on_borrow=True, #TODO revisit this plus spread_on_borrowing_stocks_percent syntax 
+        dividends=0.):
         
         self.spread_on_borrowing_stocks_percent = None if spread_on_borrowing_stocks_percent is None else \
             DataEstimator(spread_on_borrowing_stocks_percent)
-        self.dividends = None if dividends is None else \
-            ParameterEstimator(dividends)
-
+        if dividends is None:
+            self.dividends = None
+        else:
+            self.dividends = DataEstimator(dividends)
+            self.dividends_parameter = ParameterEstimator(dividends)
+        
+        self.spread_on_lending_cash_percent = None if spread_on_lending_cash_percent is None else \
+            DataEstimator(spread_on_lending_cash_percent)        
+        self.spread_on_borrowing_cash_percent = None if spread_on_borrowing_cash_percent is None else \
+            DataEstimator(spread_on_borrowing_cash_percent)
+            
+        self.periods_per_year = periods_per_year
+        self.cash_return_on_borrow = cash_return_on_borrow
         
     def pre_evaluation(self, universe, backtest_times):
         super().pre_evaluation(universe=universe, backtest_times=backtest_times)
         
         if not (self.spread_on_borrowing_stocks_percent is None):
-            self.borrow_cost_stocks = cvx.Parameter(len(universe) - 1, nonneg=True)
+            self.borrow_cost_stocks = cp.Parameter(len(universe) - 1, nonneg=True)
         
         
     def values_in_time(self, t, past_returns, **kwargs):
         """We use yesterday's value of the cash return here while in the simulator
         we use today's. In the US, updates to the FED rate are published outside
         of trading hours so we might as well use the actual value for today's. The difference
         is very small so for now we do this. 
         """
         super().values_in_time(t=t, past_returns=past_returns, **kwargs)
+        ppy = periods_per_year(past_returns.index) if self.periods_per_year is None else \
+            self.periods_per_year
                                
         cash_return = past_returns.iloc[-1,-1]
 
         if not (self.spread_on_borrowing_stocks_percent is None):
-            self.borrow_cost_stocks.value = np.ones(past_returns.shape[1] - 1) * (cash_return) + \
-                self.spread_on_borrowing_stocks_percent.current_value / (100 * 252)
-        
+            self.borrow_cost_stocks.value = np.ones(past_returns.shape[1] - 1) * (
+                    cash_return if self.cash_return_on_borrow else 0.) + \
+                self.spread_on_borrowing_stocks_percent.current_value / (100 * ppy)
+                
+    def simulate(self, t, h_plus, current_and_past_returns, **kwargs):
+        
+        ppy = periods_per_year(current_and_past_returns.index) if self.periods_per_year is None else \
+            self.periods_per_year
+        
+        cash_return = current_and_past_returns.iloc[-1,-1]        
+        multiplier = 1 / (100 * ppy)
+        result = 0.
+        borrowed_stock_positions = np.minimum(h_plus.iloc[:-1], 0.)
+        result += np.sum(((cash_return if self.cash_return_on_borrow else 0.) + 
+            self.spread_on_borrowing_stocks_percent.values_in_time(t) * multiplier) * borrowed_stock_positions)
+        result += np.sum(h_plus[:-1] * self.dividends.values_in_time(t))
+          
+        # lending_spread = DataEstimator(spread_on_lending_cash_percent).values_in_time(t) * multiplier
+        # borrowing_spread = DataEstimator(spread_on_borrowing_cash_percent).values_in_time(t) * multiplier
+
+        # cash_return = current_and_past_returns.iloc[-1,-1]
+        real_cash = h_plus.iloc[-1] + sum(np.minimum(h_plus.iloc[:-1], 0.))
 
+        if real_cash > 0:
+            result += real_cash * (max(cash_return - self.spread_on_lending_cash_percent.values_in_time(t) * multiplier, 0.) - cash_return)
+        else:
+            result += real_cash * self.spread_on_borrowing_cash_percent.values_in_time(t) * multiplier
+            
+        return result
+            
+            
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Compile cost to cvxpy expression."""
         
         expression = 0. 
         
         if not (self.spread_on_borrowing_stocks_percent is None):
-           expression += cvx.multiply(self.borrow_cost_stocks, cvx.neg(w_plus)[:-1])
+           expression += cp.multiply(self.borrow_cost_stocks, cp.neg(w_plus)[:-1])
         
         if not (self.dividends is None):
-            expression -= cvx.multiply(self.dividends, w_plus[:-1])
-        assert cvx.sum(expression).is_convex()
-        return cvx.sum(expression)
+            expression -= cp.multiply(self.dividends_parameter, w_plus[:-1])
+        assert cp.sum(expression).is_convex()
+        return cp.sum(expression)
 
 
 class TransactionCost(BaseCost):
     """A model for transaction costs.
 
     See pages 10-11 in `the book <https://stanford.edu/~boyd/papers/pdf/cvx_portfolio.pdf>`_.
     We don't include the short-term alpha term `c` here because it
     can be expressed with a separate `ReturnsForecast` object. 
 
-    :param spreads:
-    :type spreads: float or pd.Series or pd.DataFrame
+    :param a:
+    :type a: float or pd.Series or pd.DataFrame
     :param pershare_cost: per-share trade cost, as as in :class:`MarketSimulator`
     :type pershare_cost: float or pd.Series or pd.DataFrame
     :param b: coefficient of the second term
     :type b: float or pd.Series or pd.DataFrame
     :param window_sigma_est: length of the window standard deviation of past returns used to estimate :math:`\sigma`
     :type window_sigma_est: int
     :param window_volume_est: length of the window mean of past volumes used as volume estimate
     :type window_volume_est: int
     :param exponent: exponent of the non-linear term, default 1.5
     :type exponent: float
     """
 
-    def __init__(self, spreads=0., pershare_cost=0.005, b=1.0, window_sigma_est=250, window_volume_est=250, exponent=1.5):
-
-        self.spreads = DataEstimator(spreads)
-        self.pershare_cost = DataEstimator(pershare_cost)
+    def __init__(self, a=0., pershare_cost=0.005, b=1.0, window_sigma_est=250, window_volume_est=250, exponent=1.5):
 
-        self.b = DataEstimator(b)
+        self.a = None if a is None else DataEstimator(a)
+        self.pershare_cost = None if pershare_cost is None else DataEstimator(pershare_cost)
+        self.b = None if b is None else DataEstimator(b)
         self.window_sigma_est = window_sigma_est
         self.window_volume_est = window_volume_est
         self.exponent = exponent
             
     def pre_evaluation(self, universe, backtest_times):
         super().pre_evaluation(universe=universe, backtest_times=backtest_times)
-        self.first_term_multiplier = cvx.Parameter(len(universe)-1, nonneg=True)
-        self.second_term_multiplier = cvx.Parameter(len(universe)-1, nonneg=True)
+        self.first_term_multiplier = cp.Parameter(len(universe)-1, nonneg=True)
+        if not (self.b is None):
+            self.second_term_multiplier = cp.Parameter(len(universe)-1, nonneg=True)
 
     def values_in_time(self, t,  current_portfolio_value, past_returns, past_volumes, current_prices, **kwargs):
         
         super().values_in_time(t=t, current_portfolio_value=current_portfolio_value, 
             past_returns=past_returns, past_volumes=past_volumes, 
             current_prices=current_prices, **kwargs)
             
-        self.first_term_multiplier.value = self.spreads.current_value/2. + self.pershare_cost.current_value / current_prices
-        sigma_est = np.sqrt((past_returns.iloc[-self.window_sigma_est:, :-1]**2).mean()).values
-        volume_est = past_volumes.iloc[-self.window_volume_est:].mean().values
+        self.first_term_multiplier.value = self.a.current_value + self.pershare_cost.current_value / current_prices.values
+        if not (self.b is None):
+            sigma_est = np.sqrt((past_returns.iloc[-self.window_sigma_est:, :-1]**2).mean()).values
+            volume_est = past_volumes.iloc[-self.window_volume_est:].mean().values
+
+            self.second_term_multiplier.value = self.b.current_value * sigma_est * \
+                (current_portfolio_value / volume_est) ** (self.exponent - 1)
+                
+    def simulate(self, t, u, current_and_past_returns, current_and_past_volumes, current_prices, **kwargs):
+        
+        sigma = np.std(current_and_past_returns.iloc[-self.window_sigma_est:, :-1], axis=0)
+
+        result = 0.
+        if not (self.pershare_cost is None):
+            if current_prices is None:
+                raise SyntaxError("If you don't provide prices you should set persharecost to None")
+            result += self.pershare_cost.values_in_time(t) * int(sum(np.abs(u.iloc[:-1] + 1E-6) / current_prices.values))
+
+        result += sum(self.a.values_in_time(t) * np.abs(u.iloc[:-1]))
+
+        if not (self.b is None):
+            if current_and_past_volumes is None:
+                raise SyntaxError("If you don't provide volumes you should set b to None")
+            # we add 1 to the volumes to prevent 0 volumes error (trades are cancelled on 0 volumes)
+            result += (np.abs(u.iloc[:-1])**self.exponent) @ (self.b.values_in_time(t)  *
+                sigma / ((current_and_past_volumes.iloc[-1] + 1) ** (self.exponent - 1)))
 
-        self.second_term_multiplier.value = self.b.current_value * sigma_est * \
-            (current_portfolio_value / volume_est) ** (self.exponent - 1)
+        assert not np.isnan(result)
+        assert not np.isinf(result)
+
+        return -result
+        
         
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
 
-        expression = cvx.abs(z[:-1]).T @ self.first_term_multiplier
-        assert expression.is_convex()
-        expression += (cvx.abs(z[:-1]) ** self.exponent).T @ self.second_term_multiplier
+        expression = cp.abs(z[:-1]).T @ self.first_term_multiplier
         assert expression.is_convex()
+        if not (self.b is None):
+            expression += (cp.abs(z[:-1]) ** self.exponent).T @ self.second_term_multiplier
+            assert expression.is_convex()
         return expression
-
```

### Comparing `cvxportfolio-0.3.1/cvxportfolio/data.py` & `cvxportfolio-0.3.2/cvxportfolio/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from pathlib import Path
 import yfinance as yf
 import pandas as pd
 import numpy as np
-import pandas_datareader
 import sqlite3
 
 from .estimator import DataEstimator
 
 __all__ = ["YfinanceTimeSeries", "FredTimeSeries", "FredRateTimeSeries", "BASE_LOCATION"]
 
 BASE_LOCATION = Path.home() / "cvxportfolio_data"
@@ -130,20 +129,19 @@
         intraday_logreturn = np.log(data["Close"]) - np.log(data["Open"])
         close_to_close_logreturn = np.log(data["Adj Close"]).diff().shift(-1)
         open_to_open_logreturn = (
             close_to_close_logreturn + intraday_logreturn - intraday_logreturn.shift(-1)
         )
         data["Return"] = np.exp(open_to_open_logreturn) - 1
         del data["Adj Close"]
-        # eliminate intraday data
+        # eliminate last period's intraday data
         data.loc[data.index[-1], ["High", "Low", "Close", "Return", "Volume"]] = np.nan
         return data
 
-    @classmethod
-    def download(cls, symbol, current=None, overlap=5, **kwargs):
+    def download(self, symbol, current=None, overlap=5, grace_period='5d', **kwargs):
         """Download single stock from Yahoo Finance.
 
         If data was already downloaded we only download
         the most recent missing portion.
 
         Args:
 
@@ -154,20 +152,20 @@
             kwargs (dict): extra arguments passed to yfinance.download
 
         Returns:
             updated (pandas.DataFrame): updated DataFrame for the symbol
         """
         if (current is None) or (len(current) < overlap):
             updated = yf.download(symbol, progress=False, **kwargs)
-            return cls.internal_process(updated)
+            return self.internal_process(updated)
         else:
-            if (pd.Timestamp.today() - current.index[-1]) < pd.Timedelta('5d'):
+            if (pd.Timestamp.today() - current.index[-1]) < pd.Timedelta(grace_period):
                 return current
             new = yf.download(symbol, progress=False, start=current.index[-overlap], **kwargs)
-            new = cls.internal_process(new)
+            new = self.internal_process(new)
             return pd.concat([current.iloc[:-overlap], new])
 
     @staticmethod
     def preload(data):
         """Prepare data for use by Cvxportfolio.
 
         We drop the 'Volume' column expressed in number of stocks
@@ -396,86 +394,98 @@
             self.location / f"{symbol}___dtypes.csv"
         )
         data.to_csv(self.location / f"{symbol}.csv", **kwargs)
 
 
 class FredBase(BaseData):
     """Base class for FRED data access."""
+    
+    URL = "https://fred.stlouisfed.org/graph/fredgraph.csv"
+    
+    def _download(self, symbol):
+        return pd.read_csv(self.URL + f'?id={symbol}', index_col=0, parse_dates=[0])[symbol]
 
-    @staticmethod
-    def download(symbol="DFF", current=None):
+    def download(self, symbol="DFF", current=None, grace_period='5d'):
+        """Download or update pandas Series from FRED. 
+        
+        If already downloaded don't change data stored locally and only
+        add new entries at the end. 
+        
+        Additionally, we allow for a `grace period`, if the data already downloaded
+        has a last entry not older than the grace period, we don't download new data.
+        """
         if current is None:
-            end = pd.Timestamp.today()
-            return pandas_datareader.get_data_fred(
-                symbol, start="1900-01-01", end=pd.Timestamp.today()
-            )[symbol]
+            return self._download(symbol)
         else:
-            new = pandas_datareader.get_data_fred(
-                symbol, start=current.index[-1], end=pd.Timestamp.today()
-            )[symbol]
-            assert new.index[0] == current.index[-1]
-            return pd.concat([current.iloc[:-1], new])
+            if (pd.Timestamp.today() - current.index[-1]) < pd.Timedelta(grace_period):
+                return current
+                
+            new = self._download(symbol)
+            new = new.loc[new.index > current.index[-1]]
+            
+            if new.empty:
+                return current
+
+            assert new.index[0] > current.index[-1]
+            return pd.concat([current, new])
 
 
 class RateBase(BaseData):
     """Manipulate rate data from percent annualized to daily."""
 
     trading_days = 252
 
-    @classmethod
-    def preload(cls, data):
-        return np.exp(np.log(1 + data / 100) / cls.trading_days) - 1
+    def preload(self, data):
+        return np.exp(np.log(1 + data / 100) / self.trading_days) - 1
 
 
 class Yfinance(YfinanceBase, LocalDataStore):
 
     """Yahoo Finance data interface using local data store.
 
     Args:
         base_location (pathlib.Path): filesystem directory where to store files.
     """
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
 
     def update_and_load(self, symbol):
         """Update data for symbol and load it."""
         return super().update_and_load(symbol)
 
 
 class FredRate(FredBase, RateBase, SqliteDataStore):
     """Load and store FRED rates like DFF."""
 
     pass
 
 
 class YfinanceTimeSeries(DataEstimator, YfinanceBase, PickleStore):
     
-    def __init__(self, symbol, use_last_available_time=False, base_location=None):
+    def __init__(self, symbol, use_last_available_time=False, base_location=BASE_LOCATION):
         self.symbol = symbol
         self.base_location = base_location
         self.use_last_available_time = use_last_available_time
 
     def pre_evaluation(self, *args, **kwargs):
         self.data = self.update_and_load(self.symbol)
         
         
 class FredTimeSeries(DataEstimator, FredBase, PickleStore):
     
-    def __init__(self, symbol, use_last_available_time=False, base_location=None):
+    def __init__(self, symbol, use_last_available_time=False, base_location=BASE_LOCATION):
         self.symbol = symbol
         self.base_location = base_location
         self.use_last_available_time = use_last_available_time
 
     def pre_evaluation(self, *args, **kwargs):
         self.data = self.update_and_load(self.symbol)
     
 class FredRateTimeSeries(DataEstimator, FredBase, RateBase, PickleStore):
     
-    def __init__(self, symbol, use_last_available_time=False, base_location=None):
+    def __init__(self, symbol, use_last_available_time=False, base_location=BASE_LOCATION):
         self.symbol = symbol
         self.base_location = base_location
         self.use_last_available_time = use_last_available_time
 
     def pre_evaluation(self, *args, **kwargs):
         self.data = self.update_and_load(self.symbol)
```

### Comparing `cvxportfolio-0.3.1/cvxportfolio/errors.py` & `cvxportfolio-0.3.2/cvxportfolio/errors.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.1/cvxportfolio/estimator.py` & `cvxportfolio-0.3.2/cvxportfolio/estimator.py`

 * *Files 19% similar despite different names*

```diff
@@ -31,26 +31,14 @@
     the `super()` corresponding method. It can make sense to call it before
     some logic, after, or not calling it at all. Also, any subclass of this that uses
     logic defined here should be careful to put estimator subclasses at the class
     attribute level, so that the two methods defined here get called recursively
     on them.
     """
 
-    def pre_evaluation(self, universe, backtest_times):
-        """Initialize estimator and its sub-estimators.
-
-        :param universe: names of assets to be traded 
-        :type universe: pandas.Index
-        :param backtest_times: times at which the estimator will be evaluated
-        :type backtest_time: pandas.DatetimeIndex
-        """
-        for _, subestimator in self.__dict__.items():
-            if hasattr(subestimator, "pre_evaluation"):
-                subestimator.pre_evaluation(universe, backtest_times)
-
     def values_in_time(self, **kwargs):
         """Evaluates estimator at a point in time recursively on its sub-estimators.
 
         This function is called by Simulator classes on Policy classes
         returning the current trades list. Policy classes, if
         they contain internal estimators, should declare them as attributes
         and call this base function (via `super()`) before
@@ -60,15 +48,32 @@
         Once we finalize the interface all parameters will be listed here.
         """
         for _, subestimator in self.__dict__.items():
             if hasattr(subestimator, "values_in_time"):
                 subestimator.values_in_time(**kwargs)
 
 
-class CvxpyExpressionEstimator(Estimator):
+class PolicyEstimator(Estimator):
+    """Base class for (most) estimators that are part of policy objects."""
+    
+
+    def pre_evaluation(self, universe, backtest_times):
+        """Initialize estimator and its sub-estimators.
+
+        :param universe: names of assets to be traded 
+        :type universe: pandas.Index
+        :param backtest_times: times at which the estimator will be evaluated
+        :type backtest_time: pandas.DatetimeIndex
+        """
+        for _, subestimator in self.__dict__.items():
+            if hasattr(subestimator, "pre_evaluation"):
+                subestimator.pre_evaluation(universe, backtest_times)
+    
+
+class CvxpyExpressionEstimator(PolicyEstimator):
     """Base class for estimators that are Cvxpy expressions."""
 
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Compile term to cvxpy expression.
 
         This is called by a Policy class on its terms before the start of the backtest
         to compile its Cvxpy problem. If the Policy changes in time
@@ -142,15 +147,15 @@
             else:
                 return result
 
         if isinstance(result, np.ndarray):
             if np.any(np.isnan(result)) and not self.allow_nans:
                 message = f"{self.__class__.__name__}.values_in_time result is an array with np.nan's."
                 if hasattr(self.data, 'columns') and len(self.data.columns) == len(result):
-                    message += "Specifically, the problem is with symbol(s)", list(self.data.columns[np.isnan(result)])
+                    message += "Specifically, the problem is with symbol(s): " + str(self.data.columns[np.isnan(result)])
                 raise MissingValuesError(message)
             else:
                 return result
 
         raise DataError(
             f"{self.__class__.__name__}.values_in_time result is not a scalar or array."
         )
@@ -220,15 +225,84 @@
 #     """Cvxpy constant that uses the pre_evalution method to be initialized."""
 #
 #     def pre_evaluation(self, returns, volumes, start_time, end_time, **kwargs):
 #         """You should call super().__init__ it here."""
 #         raise NotImplementedError
 
 
-class ParameterEstimator(cvxpy.Parameter, DataEstimator):
+# class KnownData(DataEstimator):
+#     """Data known beforehand to use in backtest.
+#
+#     :param data: user-provided data (known beforehand) in the form of time-indexed
+#         Series or DataFrame (points-in-time are used in the backtest),
+#         non-time indexed Series of DataFrame (treated as constant in time),
+#         or float. If time-indexed, it can be multi-indexed (for example for
+#         covariance matrices at points in time).
+#     :type data: pd.DataFrame, pd.Series, float
+#     :param use_last_available_time: if True, use last available time in the data
+#         at each point in the backtest
+#     :type use_last_available_time: bool
+#
+#     :ivar value: current point-in-time value populated during a backtest
+#
+#     :raises MissingValueError: if data retrieved at a point in time contains nan's
+#     """
+#
+#     def __init__(self, data, use_last_available_time=False):
+#         self.data = data
+#         self.use_last_available_time = use_last_available_time
+#
+#     def values_in_time(self, t, **kwargs):
+#         self.value = self.internal_values_in_time(t, *args, **kwargs)
+#
+#
+# class KnownDataParameter(KnownData):
+#     """Data known beforehand to use in backtest as Cvxpy parameter.
+#
+#     :param data: user-provided data (known beforehand) in the form of time-indexed
+#         Series or DataFrame (points-in-time are used in the backtest),
+#         non-time indexed Series of DataFrame (treated as constant in time),
+#         or float. If time-indexed, it can be multi-indexed (for example for
+#         covariance matrices at points in time).
+#     :type data: pd.DataFrame, pd.Series, float
+#     :param use_last_available_time: if True, use last available time in the data
+#         at each point in the backtest
+#     :type use_last_available_time: bool
+#     :param cvxpy: if True, creates a Cvxpy parameter as self.parameter
+#         with the shape of the provided data at the first point in time, and optional
+#         attributes positive_semi_definite and non_negative
+#     :type cvxpy: bool
+#     :param positive_semi_definite: if True, make a PSD Cvxpy parameter
+#     :type positive_semi_definite: bool
+#     :param non_negative: if True, make a non negative Cvxpy parameter
+#     :type non_negative: bool
+#
+#     :ivar parameter: Cvxpy parameter (if :param cvxpy: is True) with
+#         value equal to :ivar value:
+#
+#     :raises MissingValueError: if data retrieved at a point in time contains nan's
+#     """
+#
+#     def __init__(self, data, positive_semi_definite=False, non_negative=False, **kwargs):
+#         super().__init__(data, **kwargs)
+#         self.positive_semi_definite = positive_semi_definite
+#         self.non_negative = non_negative
+#
+#     def pre_evaluation(self, universe, backtest_times):
+#         value = super().internal_values_in_time(t=backtest_times[0])
+#         self.parameter = cp.Parameter(
+#             value if hasattr(value, "shape") else (),
+#             PSD=self.positive_semi_definite, nonneg=self.non_negative)
+#
+#     def values_in_time(self, t, **kwargs):
+#         self.parameter.value = self.internal_values_in_time(t, **kwargs)
+        
+        
+
+class ParameterEstimator(cvxpy.Parameter, DataEstimator, PolicyEstimator):
     """Data estimator of point-in-time values that contains a Cvxpy Parameter.
 
     Attributes:
         parameter (cvxpy.Parameter): the parameter object to use with cvxpy
             expressions
     Args:
         same as cvxportfolio.DataEstimator
```

### Comparing `cvxportfolio-0.3.1/cvxportfolio/policies.py` & `cvxportfolio-0.3.2/cvxportfolio/policies.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,22 +15,23 @@
 
 import datetime as dt
 import copy
 import logging
 
 import pandas as pd
 import numpy as np
-import cvxpy as cvx
+import cvxpy as cp
 
 from .costs import BaseCost
 from .returns import BaseReturnsModel
 from .constraints import BaseConstraint
-from .estimator import Estimator, DataEstimator
+from .estimator import PolicyEstimator, DataEstimator
 from .errors import MissingValuesError, PortfolioOptimizationError
-from .returns import ReturnsForecast
+from .returns import ReturnsForecast, CashReturn
+from .benchmark import *
 
 __all__ = [
     "Hold",
     "SellAll",
     "FixedTrades",
     "PeriodicRebalance",
     "ProportionalRebalance",
@@ -40,15 +41,15 @@
     "ProportionalTradeToTargets",
     "RankAndLongShort",
     "FixedWeights",
     "Uniform",
 ]
 
 
-class BaseTradingPolicy(Estimator):
+class BaseTradingPolicy(PolicyEstimator):
     """Base class for a trading policy."""
 
 
 class Hold(BaseTradingPolicy):
     """Hold initial portfolio, don't trade."""
 
     def values_in_time(self, current_weights, **kwargs):
@@ -285,14 +286,15 @@
           self.tracking_error.current_value:
             return self.target.current_value - current_weights
         else:
             return pd.Series(0., current_weights.index)
 
 
 
+
 class MultiPeriodOptimization(BaseTradingPolicy):
     """Multi Period Optimization policy.
 
     Implements the model developed in Chapter 5, in particular
     at page 49, of the book. You specify the objective terms
     using classes such as ReturnsForecast and TcostModel, each
     multiplied by its multiplier. You also specify lists
@@ -326,29 +328,33 @@
             (default is None) it will impose that at the last step of the multi
             period optimization the post-trade weights are equal to this.
         **kwargs: these will be passed to cvxpy.Problem.solve,
             so you can choose your own solver and pass
             parameters to it.
     """
 
-    def __init__(self, objective, constraints=[], planning_horizon=None,terminal_constraint=None,**kwargs):
+    def __init__(self, objective, constraints=[], include_cash_return=True, planning_horizon=None, terminal_constraint=None, benchmark=CashBenchmark, **kwargs):
         if hasattr(objective, '__iter__'):
             if not (hasattr(constraints, '__iter__') and len(constraints) and (hasattr(constraints[0], '__iter__') and len(objective) == len(constraints))):
                 raise SyntaxError('If you pass objective as a list, constraints should be a list of lists of the same length.')
             self.planning_horizon = len(objective)
             self.objective = objective
             self.constraints = constraints
         else:
             if not np.isscalar(planning_horizon):
                 raise SyntaxError('If `objective` and `constraints` are the same for all steps you must specify `planning_horizon`.')
             self.planning_horizon = planning_horizon
             self.objective = [copy.deepcopy(objective) for i in range(planning_horizon)] if planning_horizon > 1 else [objective]
             self.constraints = [copy.deepcopy(constraints) for i in range(planning_horizon)] if planning_horizon > 1 else [constraints]
-                
+        
+        self.include_cash_return = include_cash_return
+        if self.include_cash_return:
+            self.objective = [el + CashReturn() for el in self.objective]
         self.terminal_constraint = terminal_constraint
+        self.benchmark = benchmark() if isinstance(benchmark, type) else benchmark
         self.cvxpy_kwargs = kwargs
 
     def compile_to_cvxpy(self):#, w_plus, z, value):
         """Compile all cvxpy expressions and the problem."""
         self.cvxpy_objective = [
             el.compile_to_cvxpy(self.w_plus_at_lags[i], self.z_at_lags[i], self.w_plus_minus_w_bm_at_lags[i]) 
             for i, el in enumerate(self.objective)]
@@ -356,72 +362,86 @@
         assert self.cvxpy_objective.is_dcp()  # dpp=True)
         assert self.cvxpy_objective.is_concave()
         self.cvxpy_constraints = [
             [constr.compile_to_cvxpy(self.w_plus_at_lags[i], self.z_at_lags[i], self.w_plus_minus_w_bm_at_lags[i]) 
                 for constr in el]
             for i, el in enumerate(self.constraints)]
         self.cvxpy_constraints = sum(self.cvxpy_constraints, [])
-        self.cvxpy_constraints += [cvx.sum(z) == 0 for z in self.z_at_lags]
+        self.cvxpy_constraints += [cp.sum(z) == 0 for z in self.z_at_lags]
         w = self.w_current
         for i in range(self.planning_horizon):
             self.cvxpy_constraints.append(self.w_plus_at_lags[i] == self.z_at_lags[i] + w)
             self.cvxpy_constraints.append(self.w_plus_at_lags[i] - self.w_bm == self.w_plus_minus_w_bm_at_lags[i])
             w = self.w_plus_at_lags[i]
         if not self.terminal_constraint is None:
             self.cvxpy_constraints.append(w == self.terminal_constraint)
-        self.problem = cvx.Problem(cvx.Maximize(self.cvxpy_objective), self.cvxpy_constraints)
+        self.problem = cp.Problem(cp.Maximize(self.cvxpy_objective), self.cvxpy_constraints)
         assert self.problem.is_dcp()  # dpp=True)
 
     def pre_evaluation(self, universe, backtest_times):
         """Pass a full view of the data to initialize objects that need it."""
         for obj in self.objective:
             obj.pre_evaluation(universe=universe, backtest_times=backtest_times)
         for constr_at_lag in self.constraints:
             for constr in constr_at_lag:
                 constr.pre_evaluation(universe=universe, backtest_times=backtest_times)
+        
+        self.benchmark.pre_evaluation(universe=universe, backtest_times=backtest_times)
+        self.w_bm = cp.Parameter(len(universe))
 
         # temporary
-        self.w_bm = np.zeros(len(universe))
-        self.w_bm[-1] = 1.
+        # self.w_bm = np.zeros(len(universe))
+        # self.w_bm[-1] = 1.
         
         # initialize the problem
-        # self.portfolio_value = cvx.Parameter(nonneg=True)
-        self.w_current = cvx.Parameter(len(universe))
-        self.z_at_lags = [cvx.Variable(len(universe)) for i in range(self.planning_horizon)] 
-        self.w_plus_at_lags = [cvx.Variable(len(universe)) for i in range(self.planning_horizon)]
-        self.w_plus_minus_w_bm_at_lags = [cvx.Variable(len(universe)) for i in range(self.planning_horizon)]
+        # self.portfolio_value = cp.Parameter(nonneg=True)
+        self.w_current = cp.Parameter(len(universe))
+        self.z_at_lags = [cp.Variable(len(universe)) for i in range(self.planning_horizon)] 
+        self.w_plus_at_lags = [cp.Variable(len(universe)) for i in range(self.planning_horizon)]
+        self.w_plus_minus_w_bm_at_lags = [cp.Variable(len(universe)) for i in range(self.planning_horizon)]
+
+        # simulator will overwrite this with cached loaded from disk
+        self.cache = {}
 
         # self.compile_to_cvxpy()#self.w_plus, self.z, self.portfolio_value)
         
 
 
     def values_in_time(self, t, current_weights, current_portfolio_value, past_returns, past_volumes, current_prices, **kwargs):
         """Update all cvxpy parameters and solve."""
         
         assert current_portfolio_value > 0
         assert np.isclose(sum(current_weights), 1)
                 
-        for obj in self.objective:
+        for i, obj in enumerate(self.objective):
             obj.values_in_time(t=t, current_weights=current_weights, 
                     current_portfolio_value=current_portfolio_value, 
                     past_returns=past_returns, past_volumes=past_volumes, 
-                    current_prices=current_prices, **kwargs)      
-        for constr_at_lag in self.constraints:
+                    current_prices=current_prices, mpo_step=i, cache=self.cache, **kwargs)     
+                     
+        for i, constr_at_lag in enumerate(self.constraints):
             for constr in constr_at_lag:
                 constr.values_in_time(t=t, current_weights=current_weights, 
                     current_portfolio_value=current_portfolio_value, 
                     past_returns=past_returns, past_volumes=past_volumes, 
-                    current_prices=current_prices, **kwargs)        
+                    current_prices=current_prices, mpo_step=i, cache=self.cache, **kwargs)   
+                    
+        self.benchmark.values_in_time(t=t, current_weights=current_weights, 
+                    current_portfolio_value=current_portfolio_value, 
+                    past_returns=past_returns, past_volumes=past_volumes, 
+                    current_prices=current_prices, mpo_step=i, cache=self.cache, **kwargs) 
+                    
+        self.w_bm.value = self.benchmark.current_value
 
         # self.portfolio_value.value = 1. # not used current_portfolio_value
         self.w_current.value = current_weights.values
         try:
             self.problem.solve(#ignore_dpp=True, 
                 **self.cvxpy_kwargs)
-        except cvx.SolverError:
+        except cp.SolverError:
             raise PortfolioOptimizationError(
                 f"Numerical solver for policy {self.__class__.__name__} at time {t} failed;"
                 "try changing it, relaxing some constraints, or dropping some costs.")
         if self.problem.status in ["unbounded", "unbounded_inaccurate"]:
             raise PortfolioOptimizationError(
                 f"Policy {self.__class__.__name__} at time {t} resulted in an unbounded problem."
             )
@@ -429,29 +449,30 @@
             raise PortfolioOptimizationError(
                 f"Policy {self.__class__.__name__} at time {t} resulted in an infeasible problem."
             )
 
         return pd.Series(self.z_at_lags[0].value, current_weights.index)
 
 
+    
 class SinglePeriodOptimization(MultiPeriodOptimization):
     """Single Period Optimization policy.
 
     Implements the model developed in Chapter 4, in particular
     at page 43, of the book. You specify the objective term
     using classes such as ReturnsForecast and TcostModel, each
     multiplied by its multiplier. You also specify a list
     of constraints.
 
-    Args:
-        objective (algebra of BaseCost): this will be maximized.
-        constraints (list of BaseConstraints): these will be
-            imposed on the optimization. Default [].
-        **kwargs: these will be passed to cvxpy.Problem.solve,
-            so you can choose your own solver and pass
-            parameters to it.
+    :param objective: this algebraic combination of cvxportfolio cost objects will be maximized
+    :type objective: CombinedCost
+    :param constraints: these will be imposed on the optimization. Default [].
+    :type constraints: list of BaseConstraints
+    :param **kwargs: these will be passed to cvxpy.Problem.solve, so you can choose your own solver and pass
+        parameters to it.
     """
 
-    def __init__(self, objective, constraints=[], **kwargs):
-        super().__init__([objective], [constraints], **kwargs)
+    def __init__(self, objective, constraints=[], include_cash_return=True, benchmark=CashBenchmark, **kwargs):
+        super().__init__([objective], [constraints], include_cash_return=include_cash_return, 
+            benchmark=benchmark, **kwargs)
```

### Comparing `cvxportfolio-0.3.1/cvxportfolio/result.py` & `cvxportfolio-0.3.2/cvxportfolio/result.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from __future__ import print_function
 import collections
 import numpy as np
 import pandas as pd
 import copy
 
 from .estimator import Estimator
+from .utils import periods_per_year
 
 __all__ = ['BacktestResult']
 
 
 
 def getFiscalQuarter(dt):
     """Convert a time to a fiscal quarter."""
@@ -30,43 +31,42 @@
     quarter = (dt.month - 1) // 3 + 1
     return "Q%i %s" % (quarter, year)
     
     
 class BacktestResult(Estimator):
     """Holds the data from a Backtest and producs metrics and plots."""
     
-    # Periods per year.
-    # When we generalize to intra- or multi-day 
-    # trading we won't have this constant.
-    PPY = 252
-    
-    def __init__(self, h, u, z, tcost, hcost_stocks, hcost_cash, cash_returns, policy_times, simulator_times):
-        self.h = h
-        self.u = u
-        self.z = z
-        self.tcost = tcost
-        self.hcost_stocks = hcost_stocks
-        self.hcost_cash = hcost_cash
-        self.cash_returns = cash_returns
-        self.policy_times = policy_times
-        self.simulator_times = simulator_times
+    
+    def __init__(self, universe, backtest_times, costs):
+        """Initialization of backtest result."""
+        self.h = pd.DataFrame(index=backtest_times, columns=universe, dtype=float)
+        self.u = pd.DataFrame(index=backtest_times, columns=universe, dtype=float)
+        self.z = pd.DataFrame(index=backtest_times, columns=universe, dtype=float)
+        self.costs = {cost.__class__.__name__:pd.Series(index=backtest_times, dtype=float) for cost in costs}
+        self.policy_times = pd.Series(index=backtest_times, dtype=float)
+        self.simulator_times = pd.Series(index=backtest_times, dtype=float)
+    
+    
+    @property
+    def PPY(self):
+        return periods_per_year(self.h.index)
 
     @property
     def v(self):
         """The value of the portfolio over time."""
         return self.h.sum(axis=1)
 
     @property
     def profit(self):
         """The profit made, in dollars."""
         return self.v[-1] - self.v[0]
 
     @property
     def w(self):
-        """The weights of the portfolio over time."""
+        """The weights of the portfolio in time."""
         return (self.h.T / self.v).T
 
     @property
     def leverage(self):
         """Portfolio leverage"""
         return np.abs(self.w.iloc[:, :-1]).sum(1)
 
@@ -85,120 +85,102 @@
         """The returns R_t = (v_{t+1}-v_t)/v_t"""
         val = self.v
         return pd.Series(
             data=val.values[1:] / val.values[:-1] - 1, index=val.index[:-1]
         )
 
     @property
+    def excess_returns(self):
+        return self.returns - self.cash_returns
+        
+    @property
     def growth_rates(self):
         """The growth rate log(v_{t+1}/v_t)"""
         return np.log(self.returns + 1)
         
     @property
     def excess_growth_rates(self):
         """The growth rate log(v_{t+1}/v_t)"""
         return np.log(self.excess_returns + 1)
     
-    @property
-    def annual_growth_rate(self):
-        """The annualized growth rate PPY/T sum_{t=1}^T log(v_{t+1}/v_t)"""
-        return self.growth_rates.sum() * self.PPY / self.growth_rates.size
-
-    @property
-    def annual_return(self):
-        """The annualized return in percent."""
-        ret = self.growth_rates
-        return self._growth_to_return(ret.mean())
-
-    def _growth_to_return(self, growth):
-        """Convert growth to annualized percentage return."""
-        return 100 * (np.exp(self.PPY * growth) - 1)
-
-    def get_quarterly_returns(self, benchmark=None):
-        """The annualized returns for each fiscal quarter."""
-        ret = self.growth_rates
-        quarters = ret.groupby(getFiscalQuarter).aggregate(np.mean)
-        return self._growth_to_return(quarters)
-
-    def get_best_quarter(self, benchmark=None):
-        ret = self.get_quarterly_returns(benchmark)
-        return (ret.argmax(), ret.max())
-
-    def get_worst_quarter(self, benchmark=None):
-        ret = self.get_quarterly_returns(benchmark)
-        return (ret.argmin(), ret.min())
+    # @property
+    # def annual_growth_rate(self):
+    #     """The annualized growth rate PPY/T sum_{t=1}^T log(v_{t+1}/v_t)"""
+    #     return self.growth_rates.mean() * self.PPY
+    #
+    # @property
+    # def annual_return(self):
+    #     """The annualized return in percent."""
+    #     ret = self.growth_rates
+    #     return self._growth_to_return(ret.mean())
+    #
+    # def _growth_to_return(self, growth_rates):
+    #     """Convert growth to annualized percentage return."""
+    #     return 100 * (np.exp(self.PPY * growth) - 1)
+
+    # def get_quarterly_returns(self, benchmark=None):
+    #     """The annualized returns for each fiscal quarter."""
+    #     ret = self.growth_rates
+    #     quarters = ret.groupby(getFiscalQuarter).aggregate(np.mean)
+    #     return self._growth_to_return(quarters)
+    #
+    # def get_best_quarter(self, benchmark=None):
+    #     ret = self.get_quarterly_returns(benchmark)
+    #     return (ret.argmax(), ret.max())
+    #
+    # def get_worst_quarter(self, benchmark=None):
+    #     ret = self.get_quarterly_returns(benchmark)
+    #     return (ret.argmin(), ret.min())
 
     @property
     def sharpe_ratio(self):
         return (
             np.sqrt(self.PPY)
-            * np.mean(self.excess_growth_rates)
-            / np.std(self.excess_growth_rates)
+            * np.mean(self.excess_returns)
+            / np.std(self.excess_returns)
         )
 
     @property
     def turnover(self):
-        """Turnover ||u_t||_1/v_t"""
-        return np.abs(self.u.iloc[:,:-1]).sum(axis=1) / self.v.loc[self.u.index]
+        """Turnover ||u_t||_1/(2*v_t)"""
+        return np.abs(self.u.iloc[:,:-1]).sum(axis=1) / (2*self.v.loc[self.u.index])
 
     @property
     def trading_days(self):
         """The fraction of days with nonzero turnover."""
         return (self.turnover.values > 0).sum() / self.turnover.size
         
     @property
     def drawdown(self):
-        return (1 - (self.v / self.v.cummax()))
-
-    # @property
-    # def max_drawdown(self):
-    #     """The maximum peak to trough drawdown in percent."""
-    #     val_arr = self.v.values
-    #     max_dd_so_far = 0
-    #     cur_max = val_arr[0]
-    #     for val in val_arr[1:]:
-    #         if val >= cur_max:
-    #             cur_max = val
-    #         elif 100 * (cur_max - val) / cur_max > max_dd_so_far:
-    #             max_dd_so_far = 100 * (cur_max - val) / cur_max
-    #     return max_dd_so_far
-        
-    @property
-    def excess_returns(self):
-        return self.returns - self.cash_returns
+        return -(1 - (self.v / self.v.cummax()))
 
 
     def __repr__(self):
         data = collections.OrderedDict({
             "Number of periods": self.u.shape[0],
             "Initial timestamp": self.h.index[0],
+            "Universe size": self.h.shape[1],
             "Final timestamp": self.h.index[-1],
             "Total profit (PnL)": self.profit,
             "Annualized portfolio return (%)": self.returns.mean() * 100 * self.PPY,
             "Annualized excess return (%)": self.excess_returns.mean() * 100 * self.PPY,
-            "Annualized excess risk (%)": self.excess_returns.std() * 100 * np.sqrt(self.PPY),
+            "Annualized excess risk (%)": self.excess_returns.std() * 100 * np.sqrt(self.PPY),            
             "Sharpe ratio": self.sharpe_ratio,
-            "Max. drawdown (%)": self.drawdown.max() * 100,
+            "Worst drawdown (%)": self.drawdown.min() * 100,
             "Average drawdown (%)": self.drawdown.mean() * 100,
             "Daily Turnover (%)": self.turnover.mean() * 100,
             "Annualized Turnover (%)": self.turnover.mean() * 100 * self.PPY,
             
             "Average leverage (%)": self.leverage.mean() * 100,
-            "Max leverage (%)": self.leverage.max() * 100,
-            
-            "Average daily tcost (bp)": (self.tcost / self.v).mean()*1E4,
-            "Average daily tcost ($)": (self.tcost).mean(),
-            "Average daily stock borrow cost (bp)": (self.hcost_stocks / self.v).mean()*1E4,
-            "Average daily stock borrow cost ($)": (self.hcost_stocks).mean(),
-            "Average daily cash return or cost (bp)": (self.hcost_cash / self.v).mean()*1E4,
-            "Average daily cash return or cost ($)": (self.hcost_cash).mean(),
-            
-            "Average policy time (sec)": self.policy_times.mean(),
-            "Average simulator time (sec)": self.simulator_times.mean(),
-            
-            
-            })
+            "Max leverage (%)": self.leverage.max() * 100})
+        
+        data.update(collections.OrderedDict({f'Average of {cost} per period (bp)': (self.costs[cost]/self.v).mean()*1E4 for cost in self.costs}))
+        
+        data.update(collections.OrderedDict(
+            {"Average policy time (sec)": self.policy_times.mean(),
+            "Average simulator time (sec)": self.simulator_times.mean()
+            }))
 
         return 'Backtest Result:\n' + pd.Series(data=data).to_string(float_format="{:,.3f}".format)
```

### Comparing `cvxportfolio-0.3.1/cvxportfolio/returns.py` & `cvxportfolio-0.3.2/cvxportfolio/returns.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,202 +11,154 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """This module contains classes that define return models for
 portfolio optimization policies, and related objects.
 """
 
-import cvxpy as cvx
+import cvxpy as cp
 import numpy as np
 import pandas as pd
 
 
 from .costs import BaseCost, CombinedCosts
 from .risks import BaseRiskModel
 from .estimator import DataEstimator, ParameterEstimator
 from .forecast import HistoricalMeanReturn, HistoricalMeanError
 
 __all__ = [
     "ReturnsForecast",
     "ReturnsForecastError",
+    "CashReturn",
 ]
 
 
 class BaseReturnsModel(BaseCost):
     """Base class for return models.
 
     Use this to define any logic common to return models.
     """
 
 
-# class Kelly(BaseReturnsModel):
-#     r"""Maximize historical log-returns."""
-#
-#     def __init__(self, rolling):
-#         self.rolling = rolling
-#
-#     def pre_evaluation(self, returns, volumes, start_time, end_time, **kwargs):
-#         self.past_returns = cvx.Parameter((returns.shape[1], self.rolling))
-#
-#     def values_in_time(self, t, current_weights, current_portfolio_value, past_returns, past_volumes, **kwargs):
-#         self.past_returns.value = past_returns.iloc[-self.rolling:].values.T
-#
-#     def compile_to_cvxpy(self, w_plus, z, v):
-#         return cvx.sum(cvx.log(w_plus.T @ self.past_returns + 1)) / self.rolling
+class CashReturn(BaseReturnsModel):
+    r"""Objective term representing cash return.
     
-
-class ReturnsForecast(BaseReturnsModel):
-    r"""Returns forecast, either provided by the user or computed from the data.
+    The forecast of cash return :math:`{\left(\hat{r}_t\right)}_n` is the observed value
+    from last period :math:`{\left({r}_{t-1}\right)}_n`.
     
-    :param r_hat: constant or time varying returns estimates, or, if None, fitted
-        from the data as historical means
-    :type r_hat: pd.Series or pd.DataFrame or None
+    This object is included automatically in :class:`SinglePeriodOptimization`
+    and :class:`MultiPeriodOptimization` policies. You can change
+    this behavior by setting their ``include_cash_return`` to False.
+    
+    :param short_margin_requirement: fraction of value of a short positions
+        that is margined by portfolio cash
+    :type short_margin_requirement: float
     """
-    # r"""Returns forecast, either provided by the user or computed from the data.
-    #
-    # This class represents the term :math:`\hat{r}_t`,
-    # the forecast of assets' returns at time :math:`t`.
-    # :ref:`Optimization-based policies` use this, typically as the first
-    # element of their objectives.
-    # See Chapters 4 and 5 of the `book <https://web.stanford.edu/~boyd/papers/pdf/cvx_portfolio.pdf>`_
-    # for more details.
-    #
-    # It can either get return forecasts from the user, for example
-    # computed with some machine learning technique, or it can estimate them
-    # automatically from the data.
-    #
-    # In the first case ``r_hat`` is specified as
-    #
-    # * :class:`float`, if :math:`\hat{r}_t` is the same for all times and assets
-    # * :class:`pandas.Series` with :class:`pandas.DatetimeIndex`, if :math:`\hat{r}_t` is the same for all assets but changes in time
-    # * :class:`pandas.Series` indexed by assets' names, if :math:`\hat{r}_t` is constant in time and changes across assets
-    # * :class:`pandas.DataFrame` with :class:`pandas.DatetimeIndex`, if :math:`\hat{r}_t` changes across time and assets.
-    #
-    # The returns' forecast provided by the user must be supplied for all assets
-    # including cash (unless it is constant across all assets, so, also cash).
-    #
-    # If instead ``r_hat`` is not speficied it defaults to None. This instructs
-    # this class to compute :math:`\hat{r}_t` instead. It is
-    # done, at each step of a :class:`BackTest`, by evaluating an average of the
-    # past returns (*i.e.,* the real returns :math:`{r}_{t-1}, {r}_{t-2}, \ldots`,
-    # where :math:`t` is the current time). This class implements three ways to do so.
-    #
-    # * The full average of all available past returns skipping :class:`numpy.nan` values.
-    #   This is the default mode if no parameters are passed.
-    # * a *rolling window*  average of recent returns. This is specified by setting
-    #   the ``rolling`` parameter to a positive integer. If specified it takes precedence
-    #   over ``ewm``. See the documentation of :class:`pandas.DataFrame.rolling` for
-    #   details. It fails if the specified window contains :class:`numpy.nan` values.
-    # * an *exponential moving window* average of past returns. This is specified
-    #   by setting the ``halflife`` parameter to a positive integer.
-    #   The exponential moving window is a weighted
-    #   average where the most recent returns have a larger weight than the older
-    #   ones. This is done by calling :class:`pandas.DataFrame.ewm` with the
-    #   `halflife`` argument, which represents the number of periods over which
-    #   the weight decays by a factor of 2. See the relevant ``pandas`` documentation
-    #   for more details.
-    #
-    #
-    # The only exception to the above is the forecast of cash return
-    # :math:`{\left(\hat{r}_t\right)}_n`, for which the observed value
-    # from last period :math:`{\left({r}_{t-1}\right)}_n`
-    # is typically chosen. This is
-    # the default behavior and is done by setting ``lastforcash`` to ``True``.
-    # (If instead ``lastforcash`` is ``False``, the same averaging of past
-    # returns is used to forecast the cash return as well.)
-    #
-    # :param r_hat: return forecasts supplied by the user, default is None
-    # :type r_hat: float or pandas.Series or pandas.DataFrame or None
-    # :param rolling: size of rolling window, it takes precendence over
-    #     ``halflife`` if both are specified
-    # :type rolling: int or None
-    # :param halflife: half-life of exponential moving window
-    # :type halflife: int or None
-    # :param lastforcash: use last value to estimate cash return
-    # :type lastforcash: bool
-    #
-    # :raises cvxportfolio.MissingValuesError: If the class accesses
-    #     user-provided elements of ``r_hat`` that are :class:`numpy.nan`,
-    #     or the rolling window used for averaging contains :class:`numpy.nan`.
-    # :raises ValueError: If the data passed by the user is not of the right
-    #     size (for example the cash returns' columns is missing).
-    #
-    # :Example:
-    #
-    # >>> import cvxportfolio as cp
-    # >>> policy = cp.SinglePeriod(cp.ReturnsForecast() - \
-    #     0.5 * cp.FullCovariance())
-    #
-    # Defines a single period optimization policy where the returns' forecasts
-    # :math:`\hat{r}_t` are the full average of past returns at each point in time
-    # and the risk model is the full covariance, also computed from the past returns.
-    # """
-
-    def __init__(self, r_hat=None, #rolling=None, halflife=None, 
-                lastforcash=True, 
-                subtractshorts=True):
-        
-        if not r_hat is None:
-            self.r_hat = DataEstimator(r_hat)
-        else:
-            self.r_hat = HistoricalMeanReturn(lastforcash=lastforcash)
-            
-        # self.lastforcash = True
-        self.subtractshorts = subtractshorts
-        
-        if self.subtractshorts:
-            self.cash_return = cvx.Parameter(nonneg=True)
-        
-       
-    # @classmethod # we make it a classmethod so that also covariances can use it
-    # def update_full_mean(cls, past_returns, last_estimation, last_counts, last_time):
-    #
-    #     if last_time is None: # full estimation
-    #         estimation = past_returns.sum()
-    #         counts = past_returns.count()
-    #     else:
-    #         assert last_time == past_returns.index[-2]
-    #         estimation = last_estimation * last_counts + past_returns.iloc[-1].fillna(0.)
-    #         counts = last_counts + past_returns.iloc[-1:].count()
-    #
-    #     return estimation/counts, counts, past_returns.index[-1]
-            
+    
+    def __init__(self, cash_returns=None, short_margin_requirement=1.):
+        self.cash_returns = cash_returns
+        self.short_margin_requirement = short_margin_requirement
         
     def pre_evaluation(self, universe, backtest_times):
+        self.cash_return_parameter = cp.Parameter(nonneg=True) if self.cash_returns is None \
+            else ParameterEstimator(self.cash_returns, non_negative=True)
+        super().pre_evaluation(universe, backtest_times)
         
-        self.r_hat_parameter = cvx.Parameter(len(universe))
-        
-    
     def values_in_time(self, t, past_returns, **kwargs):
-        
+        """Update cash return parameter as last cash return."""
         super().values_in_time(t=t, past_returns=past_returns, **kwargs)
+        if self.cash_returns is None:
+            self.cash_return_parameter.value = past_returns.iloc[-1,-1]
         
-        # if self.r_hat is None:
-        #     tmp = past_returns.mean()
-        #     if self.lastforcash:
-        #         tmp.iloc[-1] = past_returns.iloc[-1, -1]
-        #     self.r_hat_parameter.value = tmp.values
-        # else:
-        #     self.r_hat_parameter.value = self.r_hat.current_value
+    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+        """Apply cash return to "real" cash position (without shorts and margins)."""
+        realcash = (w_plus[-1] - (1 + self.short_margin_requirement) * cp.sum(cp.neg(w_plus[:-1])))
+        result = realcash * self.cash_return_parameter
+        assert result.is_concave()
+        return result
         
-        self.r_hat_parameter.value = self.r_hat.current_value
-            
-        if self.subtractshorts:
-            self.cash_return.value = self.r_hat_parameter.value[-1]
+    
+    
+class ReturnsForecast(BaseReturnsModel):
+    r"""Returns forecast for non-cash assets, provided by the user or computed from the data.
 
+    This class represents the term :math:`\hat{r}_t`,
+    the forecast of non-cash assets' returns at time :math:`t`.
+    :ref:`Optimization-based policies` use this, typically as the first
+    element of their objectives.
+    See Chapters 4 and 5 of the `book <https://web.stanford.edu/~boyd/papers/pdf/cvx_portfolio.pdf>`_
+    for more details.
+
+    It can either get return forecasts from the user, for example
+    computed with some machine learning technique, or it can estimate them
+    automatically from the data.
+
+    In the first case ``r_hat`` is specified as
+
+    * :class:`float`, if :math:`\hat{r}_t` is the same for all times and non-cash assets
+    * :class:`pandas.Series` with :class:`pandas.DatetimeIndex`, if :math:`\hat{r}_t` is the same for all assets but changes in time
+    * :class:`pandas.Series` indexed by assets' names, if :math:`\hat{r}_t` is constant in time and changes across assets
+    * :class:`pandas.DataFrame` with :class:`pandas.DatetimeIndex`, if :math:`\hat{r}_t` changes across time and assets.
+
+    The returns' forecast provided by the user must be supplied for all assets
+    excluding cash.
+
+    If instead ``r_hat`` is not speficied it defaults to None. This instructs
+    this class to compute :math:`\hat{r}_t` instead. It is
+    done, at each step of a :class:`BackTest`, by evaluating the full average of the
+    past returns (*i.e.,* the real returns :math:`{r}_{t-1}, {r}_{t-2}, \ldots`,
+    where :math:`t` is the current time),  skipping :class:`numpy.nan` values.
+    This is the default mode if no parameters are passed.
+
+    :param r_hat: constant or time varying returns estimates, provided in the form of
+        a pandas DataFrame indexed by timestamps of trading period and whose columns
+        are all non-cash assets. Alternatively it can be a pandas Series indexed by the
+        assets' names (so it is constant in time), a pandas Series indexed by time (so it is 
+        constant across assets), or a float (constant for all times and assets). 
+        If it is None, the default, the return forecasts are fitted from the data as historical means.
+    :type r_hat: pd.Series or pd.DataFrame or float or None
+    :param decay: decay factor used in :class:`MultiPeriodOptimization` policies.
+        It is as a number in :math:`[0,1]`. At step :math:`\tau` of the MPO policy, where 
+        :math:`\tau=t` is the initial one, the return predictions are multiplied by 
+        :math:`\texttt{decay}^{\tau-t}`. So, ``decay`` close to zero models a `fast` signal
+        while ``decay`` close to one a `slow` signal. The default value is 1.    
+    :type decay: float
+
+    :raises cvxportfolio.MissingValuesError: If the class accesses
+        user-provided elements of ``r_hat`` that are :class:`numpy.nan`.
+
+    :Example:
+
+    >>> import cvxportfolio as cvx
+    >>> policy = cp.SinglePeriod(cvx.ReturnsForecast() - \
+        0.5 * cvx.FullCovariance())
+
+    Defines a single period optimization policy where the returns' forecasts
+    :math:`\hat{r}_t` are the full average of past returns at each point in time
+    and the risk model is the full covariance, also computed from the past returns.
+    """
+
+    def __init__(self, r_hat=None, decay=1.):
         
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
-        if self.subtractshorts:
-            noncash = w_plus[:-1].T @ self.r_hat_parameter[:-1]
-            cash = (w_plus[-1] - cvx.sum(cvx.neg(w_plus[:-1]))) * self.cash_return
-            # print(cash)
-            assert cash.is_concave()
-            return noncash + cash
+        if not r_hat is None:
+            self.r_hat = DataEstimator(r_hat)
         else:
-            return w_plus.T @ self.r_hat_parameter
+            self.r_hat = HistoricalMeanReturn()
+        self.decay = decay
+        
+    def pre_evaluation(self, universe, backtest_times):
+        self.r_hat_parameter = cp.Parameter(len(universe)-1)
+        
+    def values_in_time(self, t, past_returns, mpo_step=0, **kwargs):
+        super().values_in_time(t=t, past_returns=past_returns, mpo_step=mpo_step, **kwargs)
+        self.r_hat_parameter.value = self.r_hat.current_value * self.decay**(mpo_step)
+
+    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+        """Cvxpy expression acts on non-cash assets."""
+        return w_plus[:-1].T @ self.r_hat_parameter 
         
 
 
 class ReturnsForecastError(BaseRiskModel):
     """Simple return forecast error risk with values provided by the user.
 
     Implements the model described in pages 31-32 of the paper. You
@@ -220,41 +172,31 @@
         errors on the returns forecasts (if Series),
         or varying in time (if DataFrame), 
         or fitted from the data as the standard deviation
         of the historical mean estimator 
     :type deltas_errors: pd.DataFrame or pd.Series or None
     """
 
-    def __init__(self, deltas=None):#, zeroforcash=True, # rolling=None, halflife=None
+    def __init__(self, deltas=None):
         
         if not deltas is None:
             self.deltas = DataEstimator(deltas)
         else:
-            self.deltas = HistoricalMeanError()#zeroforcash)
-        # self.zeroforcash = zeroforcash
-
+            self.deltas = HistoricalMeanError()
             
     def pre_evaluation(self, universe, backtest_times):
         super().pre_evaluation(universe=universe, backtest_times=backtest_times)
-        self.deltas_parameter = cvx.Parameter(len(universe)-1, nonneg=True)
+        self.deltas_parameter = cp.Parameter(len(universe)-1, nonneg=True)
 
 
     def values_in_time(self, t, past_returns, **kwargs):
         super().values_in_time(t=t, past_returns=past_returns, **kwargs)
-        # if self.deltas is None:
-        #     # if self.mode == 'full':
-        #     tmp = (past_returns.iloc[:,:].std() / np.sqrt(past_returns.iloc[:,:].count())).values
-        #     if self.zeroforcash:
-        #         tmp[-1] = 0.
-        #     self.deltas_parameter.value = tmp
-        # else:
-        #     self.deltas_parameter.value = self.deltas.current_value
         self.deltas_parameter.value = self.deltas.current_value
 
 
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Compile to cvxpy expression."""
-        return cvx.abs(w_plus_minus_w_bm[:-1]).T @ self.deltas_parameter
+        return cp.abs(w_plus_minus_w_bm[:-1]).T @ self.deltas_parameter
```

### Comparing `cvxportfolio-0.3.1/cvxportfolio/risks.py` & `cvxportfolio-0.3.2/cvxportfolio/risks.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,49 +14,33 @@
 
 from .estimator import ParameterEstimator, DataEstimator 
 import logging
 import warnings
 
 import scipy.linalg
 
-import cvxpy as cvx
+import cvxpy as cp
 import numpy as np
 import pandas as pd
 
 from .costs import BaseCost
-from .errors import ForeCastError
 from .forecast import HistoricalVariance, HistoricalFactorizedCovariance
 
 logger = logging.getLogger(__name__)
 
 
 __all__ = [
     "FullCovariance",
     "DiagonalCovariance",
     "FactorModelCovariance",
     "RiskForecastError",
     "WorstCaseRisk",
 ]
 
 
-# class CashBenchMark(ConstantEstimator):
-#     """Default benchmark weights for cvxportfolio risk models.
-#     """
-#
-#     def __init__(self):
-#         pass
-#
-#     def pre_evaluation(self, returns, volumes, start_time, end_time, **kwargs):
-#         """Initialize it using the size of the returns.
-#         """
-#         size = returns.shape[1]
-#         value = np.zeros(size)
-#         value[-1] = 1.
-#         super().__init__(value)
-#         super().pre_evaluation(returns, volumes, start_time, end_time, **kwargs)
 
 
 class BaseRiskModel(BaseCost):
     pass
 
 
 
@@ -115,92 +99,51 @@
     #     will be used for estimation.
     # :type halflife: int or None
     # :param kappa: the multiplier for the associated forecast error risk
     #     (see pages 32-33 of the `book <https://web.stanford.edu/~boyd/papers/pdf/cvx_portfolio.pdf>`_).
     #     If ``float`` a passed it is treated as a constant, if ``pandas.Series`` with ``pandas.DateTime`` index
     #     it varies in time, if ``None`` the forecast error risk term will not be compiled.
     # :type kappa: float or pandas.Series or None
-    # :param addmean: correct the covariance matrix with the term :math:`\mu\mu^T`, as is explained
+    # :param kelly: correct the covariance matrix with the term :math:`\mu\mu^T`, as is explained
     #     in page 28 of the `book <https://web.stanford.edu/~boyd/papers/pdf/cvx_portfolio.pdf>`_,
     #     to match the second term of the Taylor expansion of the portfolio log-return. Default
     #     is ``False``, corresponding to classical mean-variance optimization. If ``True``, it
     #     estimates :math:`\mu` with the same technique as :math:`\Sigma`, *i.e.*, with rolling window
     #     average, exponential moving window average, or an average of the full history.
-    # :type addmean: bool
+    # :type kelly: bool
     # """
 
-    def __init__(self, Sigma=None, addmean=True):
+    def __init__(self, Sigma=None, kelly=True):
 
         if not Sigma is None:
             self.Sigma = DataEstimator(Sigma)
             self.alreadyfactorized = False
         else:
-            self.Sigma = HistoricalFactorizedCovariance(# zeroforcash=True, 
-                addmean=addmean) #Sigma
+            self.Sigma = HistoricalFactorizedCovariance(kelly=kelly) 
             self.alreadyfactorized = True
             
-        # self.zeroforcash = True
-        # self.addmean = addmean
-
-
     def pre_evaluation(self, universe, backtest_times):
         super().pre_evaluation(universe, backtest_times)
         
-        
-        self.Sigma_sqrt = cvx.Parameter((len(universe)-1, len(universe)-1))#+self.addmean))
-
-        #super().pre_evaluation(returns, volumes, start_time, end_time, **kwargs)
-        
-    # @classmethod
-    # def get_count_matrix(cls, past_returns):
-    #     """We obtain the matrix of non-null joint counts."""
-    #     tmp = ~past_returns.isnull()
-    #     return len(past_returns) * (tmp.cov(ddof=0) + np.outer(tmp.mean(), tmp.mean()))
-    #
-    # @classmethod # we make it a classmethod so that also covariances can use it
-    # def update_full_covariance(cls, past_returns, last_estimation, last_counts, last_time):
-    #
-    #     if last_time is None: # full estimation
-    #         estimation = past_returns.iloc[:,:-1].cov()
-    #         counts = self.get_count_matrix(past_returns)
-    #     else:
-    #         assert last_time == past_returns.index[-2]
-    #
-    #         estimation = last_estimation * last_counts + past_returns.iloc[-1:].fillna(0.)
-    #         counts = last_counts + past_returns.iloc[-1:].count()
-    #
-    #     return estimation, counts, past_returns.index[-1]
+        self.Sigma_sqrt = cp.Parameter((len(universe)-1, len(universe)-1))
 
     def values_in_time(self, t, past_returns, **kwargs):
         """Update forecast error risk here, and take square root of Sigma."""
         super().values_in_time(t=t, past_returns=past_returns, **kwargs)
         
-        # if self.Sigma is None:
-        #     Sigma = past_returns.cov(ddof=0)
-        #     if self.addmean:
-        #         mean = past_returns.mean()
-        #         Sigma += np.outer(mean, mean)
-        #     if self.zeroforcash:
-        #         Sigma.iloc[:, -1] = 0
-        #         Sigma.iloc[-1, :] = 0
-        # else:
-        #     Sigma = self.Sigma.current_value
-
         if self.alreadyfactorized:
             self.Sigma_sqrt.value = self.Sigma.current_value
         else:
             Sigma = self.Sigma.current_value
             eigval, eigvec = np.linalg.eigh(Sigma)
             eigval = np.maximum(eigval, 0.)
             self.Sigma_sqrt.value = eigvec @ np.diag(np.sqrt(eigval))
 
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
-        # TODO change benchmark weights passing
-        self.cvxpy_expression = cvx.sum_squares(self.Sigma_sqrt.T @ w_plus_minus_w_bm[:-1])
-    
+        self.cvxpy_expression = cp.sum_squares(self.Sigma_sqrt.T @ w_plus_minus_w_bm[:-1])
         return self.cvxpy_expression
 
 class RiskForecastError(BaseRiskModel):
     """Risk forecast error. 
     
     Implements the model defined in page 31 of the book. Takes same arguments
     as :class:`DiagonalCovariance`.
@@ -208,95 +151,93 @@
     :param sigma_squares: per-stock variances, indexed by time if DataFrame.
         If None it will be fitted on past data.
     :type sigma_squares: pd.DataFrame or pd.Series or None
     """
 
     def __init__(self, sigma_squares=None):
         if sigma_squares is None:
-            self.sigma_squares = HistoricalVariance(addmean=True) #None None
+            self.sigma_squares = HistoricalVariance(kelly=True) #None None
         else:
             self.sigma_squares = DataEstimator(sigma_squares)
         # self.standard_deviations = ParameterEstimator(standard_deviations)
         # self.zeroforcash=True
-        # self.addmean=True
+        # self.kelly=True
         
     def pre_evaluation(self, universe, backtest_times):
         super().pre_evaluation(universe, backtest_times)
-        self.sigmas_parameter = cvx.Parameter(len(universe)-1, nonneg=True)#+self.addmean))
+        self.sigmas_parameter = cp.Parameter(len(universe)-1, nonneg=True)#+self.kelly))
 
     def values_in_time(self, t, past_returns, **kwargs):
         """Update forecast error risk here, and take square root of Sigma."""
         super().values_in_time(t=t, past_returns=past_returns)
         
         # if self.sigma_squares is None:
         #     sigma_squares = past_returns.var(ddof=0)
-        #     if self.addmean:
+        #     if self.kelly:
         #         mean = past_returns.mean()
         #         sigma_squares += mean**2
         #     if self.zeroforcash:
         #         sigma_squares.iloc[-1] = 0.
         #     sigma_squares = sigma_squares.values
         # else:
         #     sigma_squares = self.sigma_squares.current_value
             
         sigma_squares = self.sigma_squares.current_value
         
         self.sigmas_parameter.value = np.sqrt(sigma_squares)
 
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
 
-        return cvx.square(cvx.abs(w_plus_minus_w_bm[:-1]).T @ self.sigmas_parameter)
+        return cp.square(cp.abs(w_plus_minus_w_bm[:-1]).T @ self.sigmas_parameter)
                 
-                
-
 
 class DiagonalCovariance(BaseRiskModel):
     """Diagonal covariance matrix, user-provided or fit from data.
 
     :param sigma_squares: per-stock variances, indexed by time if DataFrame.
         If None it will be fitted on past data.
     :type sigma_squares: pd.DataFrame or pd.Series or None 
     """
 
     def __init__(self, sigma_squares=None):
         if not sigma_squares is None:
             self.sigma_squares = DataEstimator(sigma_squares)
         else:
-            self.sigma_squares = HistoricalVariance(addmean=True) #None
+            self.sigma_squares = HistoricalVariance(kelly=True) #None
         #self.zeroforcash = True
-        #self.addmean = True
+        #self.kelly = True
         # self.standard_deviations = ParameterEstimator(standard_deviations)
         
     def pre_evaluation(self, universe, backtest_times):
         super().pre_evaluation(universe, backtest_times)
-        self.sigmas_parameter = cvx.Parameter(len(universe)-1) #+self.addmean))
+        self.sigmas_parameter = cp.Parameter(len(universe)-1) #+self.kelly))
 
     def values_in_time(self, t, past_returns, **kwargs):
         """Update forecast error risk here, and take square root of Sigma."""
         #super().values_in_time(t, current_weights, current_portfolio_value, past_returns, past_volumes, **kwargs)
         super().values_in_time(t=t, past_returns=past_returns, **kwargs)
         
         # if self.sigma_squares is None:
         #     sigma_squares = past_returns.var(ddof=0)
-        #     if self.addmean:
+        #     if self.kelly:
         #         mean = past_returns.mean()
         #         sigma_squares += mean**2
         #     if self.zeroforcash:
         #         sigma_squares[-1] = 0.
         #     sigma_squares = sigma_squares.values
         # else:
         #     sigma_squares = self.sigma_squares.current_value
         
         sigma_squares = self.sigma_squares.current_value
 
         self.sigmas_parameter.value = np.sqrt(sigma_squares)
 
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
 
-        return cvx.sum_squares(cvx.multiply(w_plus_minus_w_bm[:-1], self.sigmas_parameter))
+        return cp.sum_squares(cp.multiply(w_plus_minus_w_bm[:-1], self.sigmas_parameter))
 
 
 class FactorModelCovariance(BaseRiskModel):
     """Factor model covariance, either user-provided or fitted from the data.
     
     It has the structure
     
@@ -327,24 +268,24 @@
     #     forecast_error_kappa (float or pd.Series): uncertainty on the
     #         assets' correlations. See the paper, pages 32-33.
 
     # """
 
     factor_Sigma = None
 
-    def __init__(self, F=None, d=None, num_factors=1):#, normalize=False):
+    def __init__(self, F=None, d=None, num_factors=1, kelly=True):#, normalize=False):
         self.F = F if F is None else ParameterEstimator(F) 
         self.d = d if d is None else DataEstimator(d) 
         if (self.F is None) or (self.d is None):
             self.fit = True
-            self.Sigma = HistoricalFactorizedCovariance(addmean=True) #Sigma
+            self.Sigma = HistoricalFactorizedCovariance(kelly=kelly) #Sigma
         else:
             self.fit = False
         self.num_factors = num_factors
-        # self.addmean = True
+        # self.kelly = True
         # self.zeroforcash = True
         # self.normalize = normalize
 
     # @staticmethod
     # def build_low_rank_model(rets, num_factors=10, iters=10, normalize=True, shrink=True):
     #     r"""Build a low rank risk model from past returns that include NaNs.
     #
@@ -380,25 +321,25 @@
     #     if not np.all(idyosyncratic >= 0.):
     #         raise ForeCastError("Low rank risk estimation with iterative SVD did not work.")
     #     return F, idyosyncratic
 
     def pre_evaluation(self, universe, backtest_times):
         super().pre_evaluation(universe, backtest_times)
         # super().pre_evaluation(returns, volumes, start_time, end_time, **kwargs)
-        self.idyosync_sqrt_parameter = cvx.Parameter(len(universe)-1)
-        self.F_parameter = cvx.Parameter((self.num_factors, len(universe)-1)) if self.F is None else self.F
+        self.idyosync_sqrt_parameter = cp.Parameter(len(universe)-1)
+        self.F_parameter = cp.Parameter((self.num_factors, len(universe)-1)) if self.F is None else self.F
         # if not (self.factor_Sigma is None):
-        #     self.factor_Sigma_sqrt = cvx.Parameter(self.factor_Sigma.shape, PSD=True)
-        # self.forecast_error_penalizer = cvx.Parameter(returns.shape[1], nonneg=True)
+        #     self.factor_Sigma_sqrt = cp.Parameter(self.factor_Sigma.shape, PSD=True)
+        # self.forecast_error_penalizer = cp.Parameter(returns.shape[1], nonneg=True)
 
     def values_in_time(self, t, past_returns, **kwargs):
         super().values_in_time(t=t, past_returns=past_returns, **kwargs)
         
         # if self.F is None:
-        #     if not self.addmean:
+        #     if not self.kelly:
         #         past_returns = past_returns - past_returns.mean()
         #     if self.zeroforcash:
         #         past_returns = pd.DataFrame(past_returns, copy=True)
         #         past_returns.iloc[:, -1] = 0.
         #     F, d = self.build_low_rank_model(past_returns, num_factors=self.num_factors, normalize=self.normalize)
         #     self.F_parameter.value = F.values
         #     d = d.values
@@ -411,18 +352,18 @@
             d = (Sigmasqrt[:, :-self.num_factors]**2).sum(1)
         else:
             d = self.d.current_value
         self.idyosync_sqrt_parameter.value = np.sqrt(d)
 
 
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
-        self.expression = cvx.sum_squares(cvx.multiply(self.idyosync_sqrt_parameter, w_plus_minus_w_bm[:-1]))
+        self.expression = cp.sum_squares(cp.multiply(self.idyosync_sqrt_parameter, w_plus_minus_w_bm[:-1]))
         assert self.expression.is_dcp(dpp=True)
 
-        self.expression += cvx.sum_squares(self.F_parameter @ w_plus_minus_w_bm[:-1])
+        self.expression += cp.sum_squares(self.F_parameter @ w_plus_minus_w_bm[:-1])
         assert self.expression.is_dcp(dpp=True)
 
         return self.expression
         
 
 class WorstCaseRisk(BaseRiskModel):
     """Select the most restrictive risk model for each value of the allocation vector.
@@ -448,8 +389,8 @@
         """Update parameters."""
         for risk in self.riskmodels:
             risk.values_in_time(**kwargs)
 
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         risks = [risk.compile_to_cvxpy(w_plus, z, w_plus_minus_w_bm)
                  for risk in self.riskmodels]
-        return cvx.max(cvx.hstack(risks))
+        return cp.max(cp.hstack(risks))
```

### Comparing `cvxportfolio-0.3.1/cvxportfolio/tests/base.py` & `cvxportfolio-0.3.2/cvxportfolio/tests/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 # limitations under the License.
 
 import unittest
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
-import cvxpy as cvx
-import cvxportfolio as cp
+import cvxpy as cp
+import cvxportfolio as cvx
 
 
 class BaseTestClass(unittest.TestCase):
     
     @classmethod
     def setUpClass(cls):
         """Load the data and initialize cvxpy vars."""
         cls.sigma = pd.read_csv(Path(__file__).parent / "sigmas.csv", index_col=0, parse_dates=[0])
         cls.returns = pd.read_csv(Path(__file__).parent / "returns.csv", index_col=0, parse_dates=[0])
         cls.volumes = pd.read_csv(Path(__file__).parent / "volumes.csv", index_col=0, parse_dates=[0])
-        cls.w_plus = cvx.Variable(cls.returns.shape[1])
-        cls.w_plus_minus_w_bm = cvx.Variable(cls.returns.shape[1])
-        cls.z = cvx.Variable(cls.returns.shape[1])
+        cls.w_plus = cp.Variable(cls.returns.shape[1])
+        cls.w_plus_minus_w_bm = cp.Variable(cls.returns.shape[1])
+        cls.z = cp.Variable(cls.returns.shape[1])
         cls.N = cls.returns.shape[1]
     
     def boilerplate(self, model):
         model.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
         return model.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
```

### Comparing `cvxportfolio-0.3.1/cvxportfolio/tests/returns.csv` & `cvxportfolio-0.3.2/cvxportfolio/tests/returns.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.1/cvxportfolio/tests/sigmas.csv` & `cvxportfolio-0.3.2/cvxportfolio/tests/sigmas.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.1/cvxportfolio/tests/test_constraints.py` & `cvxportfolio-0.3.2/cvxportfolio/tests/test_constraints.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,232 +15,259 @@
 """Unit tests for the constraints objects."""
 
 import unittest
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
-import cvxpy as cvx
-import cvxportfolio as cp
+import cvxpy as cp
+import cvxportfolio as cvx
 
 
 class TestConstraints(unittest.TestCase):
     
     @classmethod
     def setUpClass(cls):
         """Load the data and initialize cvxpy vars."""
         cls.sigma = pd.read_csv(Path(__file__).parent / "sigmas.csv", index_col=0, parse_dates=[0])
         cls.returns = pd.read_csv(Path(__file__).parent / "returns.csv", index_col=0, parse_dates=[0])
         cls.volumes = pd.read_csv(Path(__file__).parent / "volumes.csv", index_col=0, parse_dates=[0])
-        cls.w_plus = cvx.Variable(cls.returns.shape[1])
-        cls.w_plus_minus_w_bm = cvx.Variable(cls.returns.shape[1])
-        cls.z = cvx.Variable(cls.returns.shape[1])
+        cls.w_plus = cp.Variable(cls.returns.shape[1])
+        cls.w_plus_minus_w_bm = cp.Variable(cls.returns.shape[1])
+        cls.z = cp.Variable(cls.returns.shape[1])
         cls.N = cls.returns.shape[1]
         
     def build_constraint(self, constraint, t=None):
         """Initialize constraint, build expression, and point it to given time."""
         constraint.pre_evaluation(self.returns.columns, self.returns.index)
         cvxpy_expression = constraint.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
-        constraint.values_in_time(t=pd.Timestamp("2020-01-01") if t is None else t)
+        constraint.values_in_time(t=pd.Timestamp("2020-01-01") if t is None else t, current_portfolio_value=1000)
         return cvxpy_expression
         
     def test_long_only(self):
-        model = cp.LongOnly()
+        model = cvx.LongOnly()
         cons = self.build_constraint(model)
         self.w_plus.value = np.ones(self.N)
         self.assertTrue(cons.value())
         self.w_plus.value = -np.ones(self.N)
         self.assertFalse(cons.value())
         
     
     def test_long_cash(self):
-        model = cp.LongCash()
+        model = cvx.LongCash()
         cons = self.build_constraint(model)
         self.w_plus.value = np.ones( self.N)
         self.assertTrue(cons.value())
         tmp = np.ones( self.N)
         tmp[-1] = -1
         self.w_plus.value = tmp
+        self.assertTrue(cons.is_dcp())
         self.assertFalse(cons.value())
         
+    def test_min_cash(self):
+        model = cvx.MinCashBalance(10000) # USD
+        cons = self.build_constraint(model)
+        self.w_plus.value = np.zeros( self.N)
+        self.w_plus.value[-1] = 1
+        model.values_in_time(t=pd.Timestamp("2020-01-01"), current_portfolio_value=10001)
+        self.assertTrue(cons.value())
+        model.values_in_time(t=pd.Timestamp("2020-01-01"), current_portfolio_value=9999)
+        self.assertFalse(cons.value())        
+        
+
     def test_dollar_neutral(self):
-        model = cp.DollarNeutral()
+        model = cvx.DollarNeutral()
         cons = self.build_constraint(model)
         tmpvalue = np.zeros( self.N)
         tmpvalue[-1] = 1 - sum(tmpvalue[:-1])
         self.w_plus.value = tmpvalue
         self.assertTrue(cons.value())
         tmpvalue = np.ones(self.N)
         tmpvalue[-1] = 1 - sum(tmpvalue[:-1])
         self.w_plus.value = tmpvalue
         self.assertFalse(cons.value())
         
     def test_leverage_limit(self):
-        model = cp.LeverageLimit(2)
+        model = cvx.LeverageLimit(2)
         cons = self.build_constraint(model)
         self.w_plus.value = np.ones(self.N) / self.N
         self.assertTrue(cons.value())
         tmp = np.zeros(self.N)
         tmp[0] = 4
         tmp[-1] = -3
         self.w_plus.value = tmp
         self.assertFalse(cons.value())
-        model = cp.LeverageLimit(7)
+        model = cvx.LeverageLimit(7)
         cons = self.build_constraint(model)
         tmp = np.zeros(self.N)
         tmp[0] = 4
         tmp[-1] = -3
         self.w_plus.value = tmp
         self.assertTrue(cons.value())
     
     def test_leverage_limit_in_time(self):
         limits = pd.Series(index=self.returns.index, data=2)
         limits.iloc[1] = 7
-        model = cp.LeverageLimit(limits)
+        model = cvx.LeverageLimit(limits)
         cons = self.build_constraint(model, t=self.returns.index[1])
         tmp = np.zeros(self.N)
         tmp[0] = 4
         tmp[-1] = -3
         self.w_plus.value = tmp
         self.assertTrue(cons.value())
         model.values_in_time(t=self.returns.index[2])
         self.assertFalse(cons.value())
         
     def test_max_weights(self):
-        model = cp.MaxWeights(2)
+        model = cvx.MaxWeights(2)
         cons = self.build_constraint(model)
         self.w_plus.value = np.ones(self.N) / self.N
         self.assertTrue(cons.value())
         tmp = np.zeros(self.N)
         tmp[0] = 4
         tmp[-1] = -3
         self.w_plus.value = tmp
         self.assertFalse(cons.value())
 
-        model = cp.MaxWeights(7)
+        model = cvx.MaxWeights(7)
         cons = self.build_constraint(model)
 
         tmp = np.zeros(self.N)
         tmp[0] = 4
         tmp[-1] = -3
         self.w_plus.value = tmp
         self.assertTrue(cons.value())
 
         limits = pd.Series(index=self.returns.index, data=2)
         limits.iloc[1] = 7
 
-        model = cp.MaxWeights(limits)
+        model = cvx.MaxWeights(limits)
         cons = self.build_constraint(model, t=self.returns.index[1])
 
         tmp = np.zeros(self.N)
         tmp[0] = 4
         tmp[-1] = -3
         self.w_plus.value = tmp
         self.assertTrue(cons.value())
         model.values_in_time(t=self.returns.index[2])
         self.assertFalse(cons.value())
         
     def test_min_weights(self):
-        model = cp.MinWeights(2)
+        model = cvx.MinWeights(2)
         cons = self.build_constraint(model, self.returns.index[1])
 
         self.w_plus.value = np.ones(self.N) / self.N
         self.assertFalse(cons.value())
         tmp = np.zeros(self.N)
         tmp[0] = 4
         tmp[-1] = -3
         self.w_plus.value = tmp
         self.assertFalse(cons.value())
-        model = cp.MinWeights(-3)
+        model = cvx.MinWeights(-3)
         cons = self.build_constraint(model, self.returns.index[1])
         tmp = np.zeros(self.N)
         tmp[0] = 4
         tmp[-1] = -3
         self.w_plus.value = tmp
         self.assertTrue(cons.value())
 
         limits = pd.Series(index=self.returns.index, data=2)
         limits.iloc[1] = -3
-        model = cp.MinWeights(limits)
+        model = cvx.MinWeights(limits)
         cons = self.build_constraint(model, t=self.returns.index[1])
         tmp = np.zeros(self.N)
         tmp[0] = 4
         tmp[-1] = -3
         self.w_plus.value = tmp
         self.assertTrue(cons.value())
         model.values_in_time(t=self.returns.index[2])
         self.assertFalse(cons.value())
 
     def test_factor_max_limit(self):
         
-        model = cp.FactorMaxLimit(np.ones((self.N - 1, 2)), np.array([0.5, 1]))
+        model = cvx.FactorMaxLimit(np.ones((self.N - 1, 2)), np.array([0.5, 1]))
         cons = self.build_constraint(model, self.returns.index[1])
 
         self.w_plus.value = np.ones(self.N) / self.N
         self.assertFalse(cons.value())
         tmp = np.zeros(self.N)
         tmp[0] = 4
         tmp[1] = -3
         self.w_plus.value = tmp
         self.assertFalse(cons.value())
         
 
-        model = cp.FactorMaxLimit(np.ones((self.N - 1, 2)), np.array([4, 4]))
+        model = cvx.FactorMaxLimit(np.ones((self.N - 1, 2)), np.array([4, 4]))
         cons = self.build_constraint(model,self.returns.index[1])
 
         tmp = np.zeros(self.N)
         tmp[0] = 4
         tmp[1] = -3
         self.w_plus.value = tmp
         self.assertTrue(cons.value())
 
     def test_factor_min_limit(self):
         
-        model = cp.FactorMinLimit(np.ones((self.N - 1, 2)), np.array([0.5, 1]))
+        model = cvx.FactorMinLimit(np.ones((self.N - 1, 2)), np.array([0.5, 1]))
         cons = self.build_constraint(model, self.returns.index[1])
 
         self.w_plus.value = np.ones(self.N) / self.N
         self.assertFalse(cons.value())
         tmp = np.zeros(self.N)
         tmp[0] = 4
         tmp[1] = -3
         
         self.w_plus.value = tmp
         self.assertTrue(cons.value())
         
-        model = cp.FactorMinLimit(np.ones((self.N - 1, 2)), np.array([4, 4]))
+        model = cvx.FactorMinLimit(np.ones((self.N - 1, 2)), np.array([4, 4]))
         cons = self.build_constraint(model, self.returns.index[1])
         # cons = model.weight_expr(t, self.w_plus, None, None)[0]
         tmp = np.zeros(self.N)
         tmp[0] = 4
         # tmp[1] = -3
         self.w_plus.value = tmp
         self.assertTrue(cons.value())
 
     def test_fixed_alpha(self):
-        model = cp.FixedFactorLoading(np.ones((self.N - 1, 1)), 1)
+        model = cvx.FixedFactorLoading(np.ones((self.N - 1, 1)), 1)
         cons = self.build_constraint(model, self.returns.index[1])
 
         self.w_plus.value = np.ones(self.N) / self.N
         self.assertFalse(cons.value())
         tmp = np.zeros(self.N)
         tmp[0] = 4
         tmp[1] = -3
         self.w_plus.value = tmp
         self.assertTrue(cons.value())
+        
+    def test_turnover_limit(self):
+        model = cvx.TurnoverLimit(0.1)
+        cons = self.build_constraint(model)
+        self.z.value = np.zeros(self.N)
+        self.z.value[-1] = -sum(self.z.value[:-1])
+        self.assertTrue(cons.value())
+        
+        self.z.value[1] = 0.2
+        self.z.value[-1] = -sum(self.z.value[:-1])
+        self.assertTrue(cons.value())
+        
+        self.z.value[2] = -0.01
+        self.z.value[-1] = -sum(self.z.value[:-1])
+        self.assertFalse(cons.value())
 
         
     def test_participation_rate(self):
         """Test trading constraints."""
 
         t = self.returns.index[1]
 
         # avg daily value limits.
         value = 1e6
-        model = cp.ParticipationRateLimit(self.volumes, max_fraction_of_volumes=0.1)
+        model = cvx.ParticipationRateLimit(self.volumes, max_fraction_of_volumes=0.1)
         model.pre_evaluation(self.returns.columns, self.returns.index)
         cons = model.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
         model.values_in_time(t=t, current_portfolio_value=value)
         print(model.portfolio_value.value)
         # cons = model.weight_expr(t, None, z, value)[0]
         tmp = np.zeros(self.N)
         tmp[:-1] = self.volumes.loc[t].values / value * 0.05
```

### Comparing `cvxportfolio-0.3.1/cvxportfolio/tests/test_costs.py` & `cvxportfolio-0.3.2/cvxportfolio/tests/test_costs.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,18 +83,19 @@
     def test_hcost(self):
         """Test holding cost model."""
         dividends = pd.Series(np.random.randn(self.N-1), self.returns.columns[:-1])
         dividends *= 0.
         hcost = HoldingCost(spread_on_borrowing_stocks_percent=.5,
                             dividends=dividends)
         
+        t = 100 # this is picked so that periods_per_year evaluates to 252
         hcost.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
         expression = hcost.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
-        hcost.values_in_time(t=self.returns.index[12], past_returns=self.returns.iloc[:12])
-        cash_ret = self.returns.iloc[11][-1]
+        hcost.values_in_time(t=self.returns.index[t], past_returns=self.returns.iloc[:t])
+        cash_ret = self.returns.iloc[t-1][-1]
         
         for i in range(10):
             self.w_plus.value = np.random.randn(self.N)
             self.w_plus.value[-1] = 1 - np.sum(self.w_plus.value[:-1])
         
             print(expression.value)
 
@@ -114,42 +115,42 @@
         """Test tcost model."""
         value = 1e6
         
         pershare_cost = pd.Series([0., 0.005, 0.], [self.returns.index[12], self.returns.index[23], self.returns.index[34]])
         b = pd.Series([0., 0., 1.], [self.returns.index[12], self.returns.index[23], self.returns.index[34]])
         
         tcost = TransactionCost(
-            spreads=0.001, pershare_cost=pershare_cost, b=b, window_sigma_est=250, window_volume_est=250, exponent=1.5)
+            a=0.001/2, pershare_cost=pershare_cost, b=b, window_sigma_est=250, window_volume_est=250, exponent=1.5)
         
         t = self.returns.index[12]
         
         tcost.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
         expression = tcost.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
         
         # only spread
         
         tcost.values_in_time(t=self.returns.index[12], 
             current_portfolio_value = value,
             past_returns=self.returns.iloc[:12], 
             past_volumes=self.volumes.iloc[:12],
-            current_prices=pd.Series(np.ones(self.returns.shape[1]-1), self.returns.columns[:-1]).values)
+            current_prices=pd.Series(np.ones(self.returns.shape[1]-1), self.returns.columns[:-1]))
         
         
         self.z.value = np.random.randn(self.returns.shape[1])
         self.z.value[-1] = -np.sum(self.z.value[:-1])
         
         est_tcost_lin = sum(np.abs(self.z.value[:-1]) * 0.0005)
         print(est_tcost_lin)
         print(expression.value)
         self.assertTrue(np.isclose(expression.value, est_tcost_lin))
         
         
         # spread and fixed cost
         
-        prices = pd.Series(np.random.uniform(1, 100, size=self.returns.shape[1]-1), self.returns.columns[:-1]).values
+        prices = pd.Series(np.random.uniform(1, 100, size=self.returns.shape[1]-1), self.returns.columns[:-1])
         
         tcost.values_in_time(t=self.returns.index[23], 
             current_portfolio_value = value,
             past_returns=self.returns.iloc[:23], 
             past_volumes=self.volumes.iloc[:23],
             current_prices=prices)
         
@@ -165,15 +166,15 @@
         
         # spread and nonlin cost
         
         tcost.values_in_time(t=self.returns.index[34], 
             current_portfolio_value = value,
             past_returns=self.returns.iloc[:34], 
             past_volumes=self.volumes.iloc[:34],
-            current_prices=pd.Series(np.ones(self.returns.shape[1]-1), self.returns.columns[:-1]).values)
+            current_prices=pd.Series(np.ones(self.returns.shape[1]-1), self.returns.columns[:-1]))
         
         
         self.z.value = np.random.randn(self.returns.shape[1])
         self.z.value[-1] = -np.sum(self.z.value[:-1])
         
         est_tcost_lin = sum(np.abs(self.z.value[:-1]) * 0.0005)
         volumes_est = self.volumes.iloc[:34].mean().values
```

### Comparing `cvxportfolio-0.3.1/cvxportfolio/tests/test_data.py` & `cvxportfolio-0.3.2/cvxportfolio/tests/test_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 
 """Unit tests for the data interfaces."""
 
 import unittest
 import shutil, tempfile
 from pathlib import Path
 
-
-import cvxpy as cvx
 import numpy as np
 import pandas as pd
 
 from cvxportfolio.data import (
     YfinanceBase,
     LocalDataStore,
     Yfinance,
```

### Comparing `cvxportfolio-0.3.1/cvxportfolio/tests/test_estimator.py` & `cvxportfolio-0.3.2/cvxportfolio/tests/test_estimator.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Unit tests for the data and parameter estimator objects."""
 
-import cvxpy as cvx
 import numpy as np
 import pandas as pd
 import unittest
 
 from cvxportfolio.estimator import DataEstimator, ParameterEstimator
 from cvxportfolio.errors import MissingValuesError, DataError
```

### Comparing `cvxportfolio-0.3.1/cvxportfolio/tests/test_forecast.py` & `cvxportfolio-0.3.2/cvxportfolio/tests/test_forecast.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,56 +14,56 @@
 
 """Unit tests for the data and parameter estimator objects."""
 
 import unittest
 from pathlib import Path
 
 
-import cvxpy as cvx
+import cvxpy as cp
 import numpy as np
 import pandas as pd
 
 
 from cvxportfolio.forecast import HistoricalMeanReturn, HistoricalMeanError, HistoricalVariance, HistoricalFactorizedCovariance
 
 class TestEstimators(unittest.TestCase):
     
     @classmethod
     def setUpClass(cls):
         """Load the data and initialize cvxpy vars."""
         # cls.sigma = pd.read_csv(Path(__file__).parent / "sigmas.csv", index_col=0, parse_dates=[0])
         cls.returns = pd.read_csv(Path(__file__).parent / "returns.csv", index_col=0, parse_dates=[0])
         # cls.volumes = pd.read_csv(Path(__file__).parent / "volumes.csv", index_col=0, parse_dates=[0])
-        cls.w_plus = cvx.Variable(cls.returns.shape[1])
-        cls.w_plus_minus_w_bm = cvx.Variable(cls.returns.shape[1])
-        cls.z = cvx.Variable(cls.returns.shape[1])
+        cls.w_plus = cp.Variable(cls.returns.shape[1])
+        cls.w_plus_minus_w_bm = cp.Variable(cls.returns.shape[1])
+        cls.z = cp.Variable(cls.returns.shape[1])
         cls.N = cls.returns.shape[1]
     
     # def boilerplate(self, model):
     #     model.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
     #     return model.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
          
     
     def test_mean_update(self):
-        forecaster = HistoricalMeanReturn(lastforcash=True)
+        forecaster = HistoricalMeanReturn()#lastforcash=True)
         
         returns = pd.DataFrame(self.returns, copy=True)
         returns.iloc[:20, 3:10] = np.nan
         
         for tidx in [50,51,52,55,56,57]:
             t = returns.index[tidx]
             past_returns = returns.loc[returns.index<t]
             mean = forecaster.values_in_time(t=t, past_returns=past_returns)
-            print(mean)
-            self.assertTrue(mean[-1] == past_returns.iloc[-1,-1])
-            self.assertTrue(np.allclose(mean[:-1], past_returns.iloc[:,:-1].mean()))
+            # print(mean)
+            # self.assertTrue(mean[-1] == past_returns.iloc[-1,-1])
+            self.assertTrue(np.allclose(mean, past_returns.iloc[:,:-1].mean()))
         
     
     def test_variance_update(self):
-        forecaster = HistoricalVariance(addmean=False)
+        forecaster = HistoricalVariance(kelly=False)
         
         returns = pd.DataFrame(self.returns, copy=True)
         returns.iloc[:20, 3:10] = np.nan
         
         for tidx in [50,51,52,55,56,57]:
             t = returns.index[tidx]
             past_returns = returns.loc[returns.index<t]
@@ -83,29 +83,29 @@
             past_returns = returns.loc[returns.index<t]
             val = forecaster.values_in_time(t=t, past_returns=past_returns)
             print(val)
             #self.assertTrue(mean[-1] == past_returns.iloc[-1,-1])
             self.assertTrue(np.allclose(val, past_returns.std(ddof=0)[:-1] / np.sqrt(past_returns.count()[:-1]) ))  
             
     def test_counts_matrix(self):
-        forecaster = HistoricalFactorizedCovariance()#addmean=True)
+        forecaster = HistoricalFactorizedCovariance()#kelly=True)
         returns = pd.DataFrame(self.returns, copy=True)
         returns.iloc[:20, 3:10] = np.nan
         returns.iloc[10:15, 10:20] = np.nan
         
         count_matrix = forecaster.get_count_matrix(returns)
         
         for indexes in [(1,2), (4,5), (1,5), (7, 18), (7,24), (1,15), (13,22)]:
             print(count_matrix.iloc[indexes[0], indexes[1]])
             print(len((returns.iloc[:,indexes[0]] * returns.iloc[:,indexes[1]]).dropna()))
             self.assertTrue(np.isclose(count_matrix.iloc[indexes[0], indexes[1]],
                 len((returns.iloc[:,indexes[0]] * returns.iloc[:,indexes[1]]).dropna())))
                 
     def test_sum_matrix(self):
-        forecaster = HistoricalFactorizedCovariance()#addmean=True)
+        forecaster = HistoricalFactorizedCovariance()#kelly=True)
         returns = pd.DataFrame(self.returns, copy=True)
         returns.iloc[:20, 3:10] = np.nan
         returns.iloc[10:15, 10:20] = np.nan
         
         forecaster.values_in_time(t=pd.Timestamp('2022-01-01'), past_returns=returns)
          
         sum_matrix = forecaster.last_sum_matrix
@@ -116,16 +116,17 @@
             print( (returns.iloc[:,indexes[0]] * returns.iloc[:,indexes[1]]).sum())
             self.assertTrue(np.isclose(
                 sum_matrix[indexes[0], indexes[1]],
                 (returns.iloc[:,indexes[0]] * returns.iloc[:,indexes[1]]).sum()
                 ))
         
     def test_covariance_update(self):
+        """Test covariance forecast estimator."""
         
-        forecaster = HistoricalFactorizedCovariance()#addmean=False)
+        forecaster = HistoricalFactorizedCovariance()
         
         returns = pd.DataFrame(self.returns.iloc[:, :4], copy=True)
         returns.iloc[:20, 1] = np.nan
         returns.iloc[10:30, 0] = np.nan
         returns.iloc[25:40, 2] = np.nan
         
         def compute_Sigma(rets):
@@ -144,14 +145,66 @@
         for tidx in [50,51,52,55,56,57]:
             t = returns.index[tidx]
             past_returns = returns.loc[returns.index<t]
             val = forecaster.values_in_time(t=t, past_returns=past_returns)
             Sigma = val @ val.T
             self.assertTrue(np.allclose(Sigma, compute_Sigma(past_returns)))
 
+    def test_covariance_update_nokelly(self):
+        """Test covariance forecast estimator.
+        
+        NOTE: due to a bug in pandas we can't test against pandas.DataFrame.cov, 
+        see https://github.com/pandas-dev/pandas/issues/45814 . In fact with the
+        current bug in pandas 
+        ``past_returns.iloc[:,:-1].cov(ddof=0)`` returns ``past_returns.iloc[:,:-1].cov(ddof=1)``
+        whenever there are missing values.
+        """
+        
+        forecaster = HistoricalFactorizedCovariance(kelly=False)
+        
+        returns = pd.DataFrame(self.returns.iloc[:, :4], copy=True)
+        returns.iloc[:20, 1] = np.nan
+        returns.iloc[10:30, 0] = np.nan
+        returns.iloc[25:40, 2] = np.nan
+        
+        def cov_ij(i, j, rets):
+            i_nanmasker = np.zeros(len(rets))
+            i_nanmasker[rets.iloc[:, i].isnull()] = np.nan
+            i_nanmasker[~(rets.iloc[:, i].isnull())] = 1.
+            j_nanmasker = np.zeros(len(rets))
+            j_nanmasker[rets.iloc[:, j].isnull()] = np.nan
+            j_nanmasker[~(rets.iloc[:, j].isnull())] = 1.
+            print(i_nanmasker, j_nanmasker)
+            return np.nanmean(rets.iloc[:, i] * rets.iloc[:, j]) - np.nanmean(rets.iloc[:, i] * j_nanmasker) * np.nanmean(rets.iloc[:, j] * i_nanmasker)
+        
+        def compute_Sigma(rets):
+            res = np.zeros((3,3))
+            res[0,0] = cov_ij(0,0, rets)
+            res[1,1] = cov_ij(1,1, rets)
+            res[2,2] = cov_ij(2,2, rets)
+            res[0,1] = cov_ij(0,1, rets)
+            res[0,2] = cov_ij(0,2, rets)
+            res[1,2] = cov_ij(1,2, rets)
+            res[1,0] = res[0,1]
+            res[2,0] = res[0,2]
+            res[2,1] = res[1,2]
+            return res
+        
+        
+        for tidx in [50,51,52,55,56,57]:
+            t = returns.index[tidx]
+            past_returns = returns.loc[returns.index<t]
+            val = forecaster.values_in_time(t=t, past_returns=past_returns)
+            Sigma = val @ val.T
+
+            self.assertTrue(np.allclose(Sigma, compute_Sigma(past_returns)))
+            # pandasSigma = past_returns.iloc[:,:-1].cov(ddof=0)
+            # self.assertTrue(np.allclose(Sigma, pandasSigma))
+            self.assertTrue(np.allclose(np.diag(Sigma), past_returns.iloc[:,:-1].var(ddof=0)))
+
             
         
         
     
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cvxportfolio-0.3.1/cvxportfolio/tests/test_policies.py` & `cvxportfolio-0.3.2/cvxportfolio/tests/test_policies.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 """Unit tests for the policy objects."""
 
 import unittest
 
 from pathlib import Path
 
-import cvxpy as cvx
+import cvxpy as cp
 import numpy as np
 import pandas as pd
 
 from cvxportfolio.policies import *
 # from cvxportfolio.policies import SinglePeriodOptOLD, SinglePeriodOptNEW
 from cvxportfolio.returns import *
 from cvxportfolio.risks import *
@@ -35,17 +35,17 @@
     
     @classmethod
     def setUpClass(cls):
         """Load the data and initialize cvxpy vars."""
         # cls.sigma = pd.read_csv(Path(__file__).parent / "sigmas.csv", index_col=0, parse_dates=[0])
         cls.returns = pd.read_csv(Path(__file__).parent / "returns.csv", index_col=0, parse_dates=[0])
         cls.volumes = pd.read_csv(Path(__file__).parent / "volumes.csv", index_col=0, parse_dates=[0])
-        cls.w_plus = cvx.Variable(cls.returns.shape[1])
-        cls.w_plus_minus_w_bm = cvx.Variable(cls.returns.shape[1])
-        cls.z = cvx.Variable(cls.returns.shape[1])
+        cls.w_plus = cp.Variable(cls.returns.shape[1])
+        cls.w_plus_minus_w_bm = cp.Variable(cls.returns.shape[1])
+        cls.z = cp.Variable(cls.returns.shape[1])
         cls.N = cls.returns.shape[1]
 
     def test_hold(self):
         hold = Hold()
         w = pd.Series(0.5, ["AAPL", "CASH"])
         self.assertTrue(np.all(
             hold.values_in_time(current_weights=w).values == np.zeros(2)))
@@ -260,26 +260,26 @@
             policy = AdaptiveRebalance(target, tracking_error=tracking_error)
             trade = policy.values_in_time(t=self.returns.index[1], current_weights=init)
             self.assertTrue(np.allclose(trade, 0.))
 
 
     def test_single_period_optimization(self):
 
-        return_forecast = ReturnsForecast(lastforcash=False)
-        risk_forecast = FullCovariance(addmean=False)
-        tcost = TransactionCost(spreads=1E-3, pershare_cost=0., b=0., exponent=2)
-        
+        return_forecast = ReturnsForecast()
+        risk_forecast = FullCovariance(kelly=False)
+        tcost = TransactionCost(a=1E-3/2, pershare_cost=0., b=None, exponent=2)
         
         policy = SinglePeriodOptimization(
             return_forecast
             - 2 * risk_forecast
             -tcost
             #- TcostModel(half_spread=5 * 1E-4)  # , power=2)
             ,
             constraints=[LongOnly(), LeverageLimit(1)],
+            include_cash_return=False,
             # verbose=True,
             solver='ECOS')
             
 
         policy.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
         policy.compile_to_cvxpy()
         
@@ -290,31 +290,31 @@
             t=self.returns.index[121],
             current_weights=pd.Series(
                 curw,
                 self.returns.columns),
             current_portfolio_value=1000,
             past_returns=self.returns.iloc[:121],
             past_volumes=self.volumes.iloc[:121],
-            current_prices=pd.Series(1., self.volumes.columns).values)
+            current_prices=pd.Series(1., self.volumes.columns))
             
        
 
         cvxportfolio_result = pd.Series(result, self.returns.columns)
 
         print(cvxportfolio_result)
         
         # print(np.linalg.eigh(self.returns.iloc[:121, :-1].cov().values)[0])
 
         # REPLICATE WITH CVXPY
         
         COV = self.returns.iloc[:121, :-1].cov(ddof=0).values #+ np.outer(self.returns.iloc[:121, :-1].mean(), self.returns.iloc[:121, :-1].mean())
-        w = cvx.Variable(self.N)
-        cvx.Problem(cvx.Maximize(w.T @ self.returns.iloc[:121].mean().values -
-                                 2 * cvx.quad_form(w[:-1], COV) -
-                                 5 * 1E-4 * cvx.sum(cvx.abs(w - curw)[:-1])
+        w = cp.Variable(self.N)
+        cp.Problem(cp.Maximize(w[:-1].T @ self.returns.iloc[:121, :-1].mean().values -
+                                 2 * cp.quad_form(w[:-1], COV) -
+                                 5 * 1E-4 * cp.sum(cp.abs(w - curw)[:-1])
                                  ),
                     [w >= 0, w <= 1, sum(w) == 1]
                     ).solve(solver='ECOS')
 
         cvxpy_result = pd.Series(w.value - curw, self.returns.columns)
 
         print(cvxpy_result)
@@ -328,15 +328,15 @@
 
         return_forecast = ReturnsForecast()
         risk_forecast = FullCovariance()
         
         policy = SinglePeriodOptimization(
             return_forecast
             - 2 * risk_forecast
-            - TransactionCost(spreads=10 * 1E-4, pershare_cost=0., b=0.)  # , power=2)
+            - TransactionCost(a=5 * 1E-4, pershare_cost=0., b=0.)  # , power=2)
             ,
             constraints=[LongOnly(), LeverageLimit(1)],
             # verbose=True,
             solver='ECOS')
 
         policy.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
         policy.compile_to_cvxpy()
@@ -348,15 +348,15 @@
             t=self.returns.index[134],
             current_weights=pd.Series(
                 curw,
                 self.returns.columns),
             current_portfolio_value=1000,
             past_returns=self.returns.iloc[:134],
             past_volumes=self.volumes.iloc[:134],
-            current_prices=pd.Series(1., self.volumes.columns).values)
+            current_prices=pd.Series(1., self.volumes.columns))
 
         self.assertFalse(np.allclose(result, 0.))
 
         cvxportfolio_result = pd.Series(result, self.returns.columns)
 
         curw += result
 
@@ -364,27 +364,27 @@
             t=self.returns.index[134],
             current_weights=pd.Series(
                 curw,
                 self.returns.columns),
             current_portfolio_value=1000,
             past_returns=self.returns.iloc[:134],
             past_volumes=self.volumes.iloc[:134],
-            current_prices=pd.Series(1., self.volumes.columns).values)
+            current_prices=pd.Series(1., self.volumes.columns))
 
         self.assertTrue(np.allclose(result2, 0., atol=1e-7))
         
         
     def test_single_period_optimization_infeasible(self):
 
         return_forecast = ReturnsForecast()
         risk_forecast = FullCovariance()
         policy = SinglePeriodOptimization(
             return_forecast
             - 2 * risk_forecast
-            - TransactionCost(spreads=10 * 1E-4, pershare_cost=0., b=0.)  # , power=2)
+            - TransactionCost(a=5 * 1E-4, pershare_cost=0., b=0.)  # , power=2)
             ,
             constraints=[LongOnly(), LeverageLimit(1), MaxWeights(-1)],
             # verbose=True,
             solver='ECOS')
 
         policy.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
         policy.compile_to_cvxpy()
@@ -398,15 +398,15 @@
                 t=self.returns.index[134],
                 current_weights=pd.Series(
                     curw,
                     self.returns.columns),
                 current_portfolio_value=1000,
                 past_returns=self.returns.iloc[:134],
                 past_volumes=self.volumes.iloc[:134],
-                current_prices=pd.Series(1., self.volumes.columns).values)
+                current_prices=pd.Series(1., self.volumes.columns))
             
     def test_single_period_optimization_unbounded(self):
 
         return_forecast = ReturnsForecast()
         risk_forecast = FullCovariance()
         policy = SinglePeriodOptimization(
             return_forecast
@@ -430,15 +430,15 @@
                 t=self.returns.index[134],
                 current_weights=pd.Series(
                     curw,
                     self.returns.columns),
                 current_portfolio_value=1000,
                 past_returns=self.returns.iloc[:134],
                 past_volumes=self.volumes.iloc[:134],
-                current_prices=pd.Series(1., self.volumes.columns).values)
+                current_prices=pd.Series(1., self.volumes.columns))
      
     def test_multi_period_optimization2(self):
         """Test that MPO1 and MPO2 and MPO5 return same if no tcost, and diff if tcost"""
 
         results = []
         for planning_horizon in [1,2,5]:
             return_forecast = ReturnsForecast()
@@ -478,15 +478,15 @@
         results = []
         for planning_horizon in [1,2,5]:
             return_forecast = ReturnsForecast()
             risk_forecast = FullCovariance()
             policy = MultiPeriodOptimization(
                 return_forecast
                 - 10 * risk_forecast
-                - TransactionCost(spreads=50 * 1E-4, pershare_cost=0., b=0.)
+                - TransactionCost(a=25 * 1E-4, pershare_cost=0., b=0.)
                 #- TcostModel(half_spread=5 * 1E-4)  # , power=2)
                 ,
                 constraints=[LongOnly(), LeverageLimit(1)],
                 # verbose=True,
                 planning_horizon=planning_horizon,
                 solver='ECOS')
 
@@ -500,15 +500,15 @@
                 t=self.returns.index[67],
                 current_weights=pd.Series(
                     curw,
                     self.returns.columns),
                 current_portfolio_value=1000,
                 past_returns=self.returns.iloc[:67],
                 past_volumes=self.volumes.iloc[:67],
-                current_prices=pd.Series(1., self.volumes.columns).values))
+                current_prices=pd.Series(1., self.volumes.columns)))
 
         self.assertFalse(np.allclose(results[0], results[1], atol=1e-4))
         self.assertFalse(np.allclose(results[1], results[2], atol=1e-4))
         
     def test_multi_period_optimization_syntax(self):
         with self.assertRaises(SyntaxError):
             MultiPeriodOptimization([ReturnsForecast()], [])
@@ -532,15 +532,15 @@
         for planning_horizon in [1,2,5]:
 
             return_forecast = ReturnsForecast()
             risk_forecast = FullCovariance()
             policy = MultiPeriodOptimization(
                 return_forecast
                 - 10 * risk_forecast
-                - TransactionCost(spreads=10 * 1E-4, pershare_cost=0., b=0.)  # , power=2)
+                - TransactionCost(a=5 * 1E-4, pershare_cost=0., b=0.)  # , power=2)
                 ,
                 constraints=[LongOnly(), LeverageLimit(1)],
                 #verbose=True,
                 terminal_constraint=benchmark,
                 planning_horizon=planning_horizon,
                 solver='ECOS')
 
@@ -554,15 +554,15 @@
                 t=self.returns.index[67],
                 current_weights=pd.Series(
                     curw,
                     self.returns.columns),
                 current_portfolio_value=1000,
                 past_returns=self.returns.iloc[:67],
                 past_volumes=self.volumes.iloc[:67],
-                current_prices=pd.Series(1., self.volumes.columns).values) + curw - benchmark)
+                current_prices=pd.Series(1., self.volumes.columns)) + curw - benchmark)
                                         
         self.assertTrue(np.isclose(np.linalg.norm(diff_to_benchmarks[0]), 0.))
         self.assertTrue(np.linalg.norm(diff_to_benchmarks[0]) < np.linalg.norm(diff_to_benchmarks[1]))
         self.assertTrue(np.linalg.norm(diff_to_benchmarks[1]) < np.linalg.norm(diff_to_benchmarks[2]))
     
     
 if __name__ == '__main__':
```

### Comparing `cvxportfolio-0.3.1/cvxportfolio/tests/test_returns.py` & `cvxportfolio-0.3.2/cvxportfolio/tests/test_returns.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """Unit tests for the return forecast objects."""
 
 import unittest
 from pathlib import Path
 
-import cvxpy as cvx
+import cvxpy as cp
 import numpy as np
 import pandas as pd
 import numpy as np
 
 
 
 from cvxportfolio.returns import *
@@ -30,74 +30,88 @@
     
     @classmethod
     def setUpClass(cls):
         """Load the data and initialize cvxpy vars."""
         # cls.sigma = pd.read_csv(Path(__file__).parent / "sigmas.csv", index_col=0, parse_dates=[0])
         cls.returns = pd.read_csv(Path(__file__).parent / "returns.csv", index_col=0, parse_dates=[0])
         # cls.volumes = pd.read_csv(Path(__file__).parent / "volumes.csv", index_col=0, parse_dates=[0])
-        cls.w_plus = cvx.Variable(cls.returns.shape[1])
-        cls.w_plus_minus_w_bm = cvx.Variable(cls.returns.shape[1])
-        cls.z = cvx.Variable(cls.returns.shape[1])
+        cls.w_plus = cp.Variable(cls.returns.shape[1])
+        cls.w_plus_minus_w_bm = cp.Variable(cls.returns.shape[1])
+        cls.z = cp.Variable(cls.returns.shape[1])
         cls.N = cls.returns.shape[1]
         
     def boilerplate(self, model):
+        """Initialize objects, compile cvxpy expression."""
         model.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
         return model.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
         
         
+    def test_cash_returns(self):
+        "Test CashReturn object with last return as forecast."
+        cash_model = CashReturn()
+        cvxpy_expression = self.boilerplate(cash_model)
+        self.w_plus.value = np.random.randn(self.N)
+        cash_model.values_in_time(t=None, past_returns=self.returns.iloc[:123])
+        cr = self.returns.iloc[122, -1]
+        self.assertTrue(cvxpy_expression.value == cr * (self.w_plus[-1].value + 2 * np.sum(np.minimum(self.w_plus[:-1].value, 0.))))
+        
+    def test_cash_returns_provided(self):
+        "Test CashReturn object with provided cash returns."
+        cash_model = CashReturn(self.returns.iloc[:,-1])
+        cvxpy_expression = self.boilerplate(cash_model)
+        self.w_plus.value = np.random.randn(self.N)
+        cash_model.values_in_time(t=self.returns.index[123], past_returns=None)
+        cr = self.returns.iloc[123, -1]
+        self.assertTrue(cvxpy_expression.value == cr * (self.w_plus[-1].value + 2 * np.sum(np.minimum(self.w_plus[:-1].value, 0.))))
+        
     def test_returns_forecast(self):
-        alpha_model = ReturnsForecast(self.returns)
+        "Test ReturnsForecast object with provided assets' returns."
+        alpha_model = ReturnsForecast(self.returns.iloc[:,:-1])
         cvxpy_expression = self.boilerplate(alpha_model)
         alpha_model.values_in_time(t=self.returns.index[123], past_returns=None)
         self.w_plus.value = np.random.randn(self.N)
         print(cvxpy_expression.value)
-        print(self.w_plus[:-1].value @ self.returns.iloc[123][:-1] + 
-        ((self.w_plus[-1].value + np.sum(np.minimum(self.w_plus[:-1].value, 0.))) * self.returns.iloc[123][-1]))
-        self.assertTrue(np.isclose(cvxpy_expression.value, 
-            self.w_plus[:-1].value @ self.returns.iloc[123][:-1]
-                + ((self.w_plus[-1].value + np.sum(np.minimum(self.w_plus[:-1].value, 0.))) * self.returns.iloc[123][-1])
-            ))
+        print(self.w_plus[:-1].value @ self.returns.iloc[123][:-1]) 
+        #+ ((self.w_plus[-1].value + np.sum(np.minimum(self.w_plus[:-1].value, 0.))) * self.returns.iloc[123][-1]))
+        self.assertTrue(np.isclose(cvxpy_expression.value, self.w_plus[:-1].value @ self.returns.iloc[123][:-1]))
+                #+ ((self.w_plus[-1].value + 2 * np.sum(np.minimum(self.w_plus[:-1].value, 0.))) * self.returns.iloc[123][-1])))
         
         
     def test_full_returns_forecast(self):
+        "Test ReturnsForecast object with historical mean forecasts."
         alpha_model = ReturnsForecast()
         cvxpy_expression = self.boilerplate(alpha_model)
         t = self.returns.index[123]
         alpha_model.values_in_time(t=t, past_returns = self.returns.loc[self.returns.index<t])
         self.w_plus.value = np.random.uniform(size=self.N)
         self.w_plus.value /= sum(self.w_plus.value)
-        myforecast = self.returns.loc[self.returns.index < t].mean()
-        myforecast.iloc[-1] = self.returns.iloc[122, -1]
-        self.assertTrue(np.isclose(cvxpy_expression.value, self.w_plus.value @ myforecast))
+        myforecast = self.returns.iloc[:, :-1].loc[self.returns.index < t].mean()
+        # myforecast.iloc[-1] = self.returns.iloc[122, -1]
+        self.assertTrue(np.isclose(cvxpy_expression.value, self.w_plus.value[:-1] @ myforecast))
         
     def test_returns_forecast_error(self):
-
+        "Test ReturnsForecastError object with provided values."
         delta = self.returns.iloc[:, :-1].std(ddof=0) / np.sqrt(len(self.returns))
         # delta.iloc[-1] = 0
-
         error_risk = ReturnsForecastError(delta)
         cvxpy_expression = self.boilerplate(error_risk)
         error_risk.values_in_time(t='ciao', past_returns='hello')
-
         self.w_plus_minus_w_bm.value = np.random.randn(self.N)
         self.assertTrue(np.isclose(cvxpy_expression.value, np.abs(self.w_plus_minus_w_bm.value[:-1]) @ delta))
 
 
     def test_full_returns_forecast_error(self):
-
+        "Test ReturnsForecastError object with as forecast the std of the mean estimator."
         error_risk = ReturnsForecastError()
         cvxpy_expression = self.boilerplate(error_risk)
         t = self.returns.index[123]
         past_returns = self.returns.loc[self.returns.index < t]
-        
         error_risk.values_in_time(t=t, past_returns = past_returns)
         self.w_plus_minus_w_bm.value = np.random.randn(self.N)
-        
         delta = past_returns.std(ddof=0) / np.sqrt(past_returns.count())
-
         print(cvxpy_expression.value)
         print(np.abs(self.w_plus_minus_w_bm.value[:-1]) @ delta[:-1])
         self.assertTrue(np.isclose(cvxpy_expression.value, np.abs(self.w_plus_minus_w_bm.value[:-1]) @ delta[:-1]))
     
     
 
 if __name__ == '__main__':
```

### Comparing `cvxportfolio-0.3.1/cvxportfolio/tests/test_risks.py` & `cvxportfolio-0.3.2/cvxportfolio/tests/test_risks.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,31 +13,31 @@
 # limitations under the License.
 
 """Unit tests for the risk objects."""
 
 import unittest
 from pathlib import Path
 
-import cvxpy as cvx
+import cvxpy as cp
 import numpy as np
 import pandas as pd
 
 from cvxportfolio.risks import *
 
 USED_RETURNS = 10
 
 class TestRisks(unittest.TestCase):
     
     @classmethod
     def setUpClass(cls):
         """Load the data and initialize cvxpy vars."""
         cls.returns = pd.read_csv(Path(__file__).parent / "returns.csv", index_col=0, parse_dates=[0]).iloc[:, :USED_RETURNS]
-        cls.w_plus = cvx.Variable(cls.returns.shape[1])
-        cls.w_plus_minus_w_bm = cvx.Variable(cls.returns.shape[1])
-        cls.z = cvx.Variable(cls.returns.shape[1])
+        cls.w_plus = cp.Variable(cls.returns.shape[1])
+        cls.w_plus_minus_w_bm = cp.Variable(cls.returns.shape[1])
+        cls.z = cp.Variable(cls.returns.shape[1])
         cls.N = cls.returns.shape[1]
         
     def boilerplate(self, model):
         model.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
         return model.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
 
 
@@ -63,15 +63,15 @@
         
         cvxpy_expression = self.boilerplate(risk_model)
         self.assertTrue(cvxpy_expression.is_convex())
 
         # N = returns.shape[1]
         # returns.iloc[:, -1] = 0.
 
-        # w_plus = cvx.Variable(N)
+        # w_plus = cp.Variable(N)
         # risk_model.pre_evaluation(
         #     returns.iloc[:, :], None, start_time=returns.index[50], end_time=None)
         # cvxpy_expression = risk_model.compile_to_cvxpy(w_plus, None, None)
         
         t = pd.Timestamp('2014-06-02')
         past = self.returns.loc[self.returns.index < t]
         should_be = past.iloc[:,:-1].T @ past.iloc[:,:-1] / len(past)
```

### Comparing `cvxportfolio-0.3.1/cvxportfolio/tests/volumes.csv` & `cvxportfolio-0.3.2/cvxportfolio/tests/volumes.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.1/cvxportfolio.egg-info/SOURCES.txt` & `cvxportfolio-0.3.2/cvxportfolio.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 AUTHORS
 LICENSE
 README.md
 setup.py
 cvxportfolio/__init__.py
+cvxportfolio/benchmark.py
 cvxportfolio/constraints.py
 cvxportfolio/costs.py
 cvxportfolio/data.py
 cvxportfolio/errors.py
 cvxportfolio/estimator.py
 cvxportfolio/forecast.py
 cvxportfolio/policies.py
 cvxportfolio/result.py
 cvxportfolio/returns.py
 cvxportfolio/risks.py
 cvxportfolio/simulator.py
+cvxportfolio/utils.py
 cvxportfolio.egg-info/PKG-INFO
 cvxportfolio.egg-info/SOURCES.txt
 cvxportfolio.egg-info/dependency_links.txt
 cvxportfolio.egg-info/requires.txt
 cvxportfolio.egg-info/top_level.txt
 cvxportfolio/tests/__init__.py
 cvxportfolio/tests/base.py
```

### Comparing `cvxportfolio-0.3.1/setup.py` & `cvxportfolio-0.3.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='cvxportfolio',
-    version='0.3.1',
+    version='0.3.2',
     author='Enzo Busseti, Stephen Boyd, Steven Diamond, BlackRock Inc.',
     maintainer='Enzo Busseti',
     author_email='enzo.busseti@gmail.com',
     packages=['cvxportfolio',
               'cvxportfolio.tests'],
     package_dir={'cvxportfolio': 'cvxportfolio'},
     package_data={'cvxportfolio': [
@@ -14,10 +14,10 @@
     url='https://cvxportfolio.readthedocs.io',
     license='Apache 2.0',
     description='Portfolio optimization.',
     install_requires=["pandas",
                       "numpy",
                       "matplotlib",
                       "yfinance",
-                      "pandas_datareader",
-                      "cvxpy>=1.0.6"],
+                      "cvxpy>=1.0.6",
+                      "multiprocess"],
 )
```

