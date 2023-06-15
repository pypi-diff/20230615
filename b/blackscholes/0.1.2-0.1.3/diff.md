# Comparing `tmp/blackscholes-0.1.2.tar.gz` & `tmp/blackscholes-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackscholes-0.1.2.tar", max compression
+gzip compressed data, was "blackscholes-0.1.3.tar", max compression
```

## Comparing `blackscholes-0.1.2.tar` & `blackscholes-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0     2616 2022-12-25 22:12:24.056498 blackscholes-0.1.2/.github/README.MD
--rw-r--r--   0        0        0     1065 2022-12-16 00:32:50.227092 blackscholes-0.1.2/LICENSE
--rw-r--r--   0        0        0     1069 2022-12-25 21:50:07.012322 blackscholes-0.1.2/blackscholes/__init__.py
--rw-r--r--   0        0        0    17901 2022-12-25 20:48:33.871295 blackscholes-0.1.2/blackscholes/base.py
--rw-r--r--   0        0        0     4559 2022-12-25 21:04:57.343636 blackscholes-0.1.2/blackscholes/butterfly.py
--rw-r--r--   0        0        0     4703 2022-12-23 21:45:29.889276 blackscholes-0.1.2/blackscholes/call.py
--rw-r--r--   0        0        0     4907 2022-12-25 21:53:11.338043 blackscholes-0.1.2/blackscholes/iron_butterfly.py
--rw-r--r--   0        0        0     4948 2022-12-25 21:04:57.336856 blackscholes-0.1.2/blackscholes/iron_condor.py
--rw-r--r--   0        0        0     4251 2022-12-22 17:33:47.165875 blackscholes-0.1.2/blackscholes/put.py
--rw-r--r--   0        0        0     3517 2022-12-25 21:04:57.348936 blackscholes-0.1.2/blackscholes/spread.py
--rw-r--r--   0        0        0     2986 2022-12-25 21:04:57.360596 blackscholes-0.1.2/blackscholes/straddle.py
--rw-r--r--   0        0        0     3530 2022-12-25 21:04:57.356473 blackscholes-0.1.2/blackscholes/strangle.py
--rw-r--r--   0        0        0        0 2022-12-03 15:33:29.510748 blackscholes-0.1.2/blackscholes/tests/__init__.py
--rw-r--r--   0        0        0     6598 2022-12-22 22:43:02.238774 blackscholes-0.1.2/blackscholes/tests/test_base.py
--rw-r--r--   0        0        0     2929 2022-12-23 17:07:16.664773 blackscholes-0.1.2/blackscholes/tests/test_butterfly.py
--rw-r--r--   0        0        0     7055 2022-12-21 21:45:05.302905 blackscholes-0.1.2/blackscholes/tests/test_call.py
--rw-r--r--   0        0        0     4869 2022-12-25 21:53:22.902241 blackscholes-0.1.2/blackscholes/tests/test_iron_butterfly.py
--rw-r--r--   0        0        0     4451 2022-12-25 21:35:16.300406 blackscholes-0.1.2/blackscholes/tests/test_iron_condor.py
--rw-r--r--   0        0        0     6581 2022-12-21 21:45:05.299990 blackscholes-0.1.2/blackscholes/tests/test_put.py
--rw-r--r--   0        0        0     1788 2022-12-25 21:19:56.874737 blackscholes-0.1.2/blackscholes/tests/test_spread.py
--rw-r--r--   0        0        0     1271 2022-12-23 16:06:33.794443 blackscholes-0.1.2/blackscholes/tests/test_straddle.py
--rw-r--r--   0        0        0     1836 2022-12-23 16:07:20.353283 blackscholes-0.1.2/blackscholes/tests/test_strangle.py
--rw-r--r--   0        0        0      627 2022-12-25 21:57:24.358424 blackscholes-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3312 1970-01-01 00:00:00.000000 blackscholes-0.1.2/setup.py
--rw-r--r--   0        0        0     3133 1970-01-01 00:00:00.000000 blackscholes-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2615 2022-12-26 13:11:12.753657 blackscholes-0.1.3/.github/README.MD
+-rw-r--r--   0        0        0     1065 2022-12-16 00:32:50.227092 blackscholes-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1069 2022-12-25 21:50:07.012322 blackscholes-0.1.3/blackscholes/__init__.py
+-rw-r--r--   0        0        0    18417 2023-06-15 20:15:48.324717 blackscholes-0.1.3/blackscholes/base.py
+-rw-r--r--   0        0        0     4559 2022-12-25 21:04:57.343636 blackscholes-0.1.3/blackscholes/butterfly.py
+-rw-r--r--   0        0        0     5085 2023-06-15 20:15:48.325380 blackscholes-0.1.3/blackscholes/call.py
+-rw-r--r--   0        0        0     4907 2022-12-25 21:53:11.338043 blackscholes-0.1.3/blackscholes/iron_butterfly.py
+-rw-r--r--   0        0        0     4948 2022-12-25 21:04:57.336856 blackscholes-0.1.3/blackscholes/iron_condor.py
+-rw-r--r--   0        0        0     4643 2023-06-15 20:15:48.325025 blackscholes-0.1.3/blackscholes/put.py
+-rw-r--r--   0        0        0     3517 2022-12-25 21:04:57.348936 blackscholes-0.1.3/blackscholes/spread.py
+-rw-r--r--   0        0        0     2986 2022-12-25 21:04:57.360596 blackscholes-0.1.3/blackscholes/straddle.py
+-rw-r--r--   0        0        0     3530 2022-12-25 21:04:57.356473 blackscholes-0.1.3/blackscholes/strangle.py
+-rw-r--r--   0        0        0        0 2022-12-03 15:33:29.510748 blackscholes-0.1.3/blackscholes/tests/__init__.py
+-rw-r--r--   0        0        0     6640 2023-06-15 19:55:02.922009 blackscholes-0.1.3/blackscholes/tests/test_base.py
+-rw-r--r--   0        0        0     2929 2022-12-23 17:07:16.664773 blackscholes-0.1.3/blackscholes/tests/test_butterfly.py
+-rw-r--r--   0        0        0     7672 2023-06-15 20:15:50.924398 blackscholes-0.1.3/blackscholes/tests/test_call.py
+-rw-r--r--   0        0        0     4869 2022-12-25 21:53:22.902241 blackscholes-0.1.3/blackscholes/tests/test_iron_butterfly.py
+-rw-r--r--   0        0        0     4451 2022-12-25 21:35:16.300406 blackscholes-0.1.3/blackscholes/tests/test_iron_condor.py
+-rw-r--r--   0        0        0     7200 2023-06-15 20:15:50.922889 blackscholes-0.1.3/blackscholes/tests/test_put.py
+-rw-r--r--   0        0        0     1788 2022-12-25 21:19:56.874737 blackscholes-0.1.3/blackscholes/tests/test_spread.py
+-rw-r--r--   0        0        0     1271 2022-12-23 16:06:33.794443 blackscholes-0.1.3/blackscholes/tests/test_straddle.py
+-rw-r--r--   0        0        0     1836 2022-12-23 16:07:20.353283 blackscholes-0.1.3/blackscholes/tests/test_strangle.py
+-rw-r--r--   0        0        0      627 2023-06-15 20:15:20.388997 blackscholes-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3132 1970-01-01 00:00:00.000000 blackscholes-0.1.3/PKG-INFO
```

### Comparing `blackscholes-0.1.2/.github/README.MD` & `blackscholes-0.1.3/.github/README.MD`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 put.price()  ## 1.2470
 put.delta()  ## -0.2381
 put.vomma()  ## 45.1347
 ```
 
 ### Structures
 
-`blackscholes` offers the following four option structures:
+`blackscholes` offers the following six option structures:
 - Straddle
 - Strangle
 - Butterfly
 - Iron Condor
 - Spreads
 - Iron Butterfly
```

### Comparing `blackscholes-0.1.2/LICENSE` & `blackscholes-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.2/blackscholes/__init__.py` & `blackscholes-0.1.3/blackscholes/__init__.py`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.2/blackscholes/base.py` & `blackscholes-0.1.3/blackscholes/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,24 @@
     def in_the_money(self) -> float:
         """Naive probability that option will be in the money at maturity."""
         ...
 
     @abstractmethod
     def delta(self) -> float:
         """Rate of change in option price
-        with respect to the asset price (1st derivative)."""
+        with respect to the forward price (1st derivative).
+        """
+        ...
+
+    @abstractmethod
+    def forward_delta(self) -> float:
+        """
+        Delta discounted for interest rates.
+        For the cash/spot delta, use `delta`.
+        """
         ...
 
     @abstractmethod
     def dual_delta(self) -> float:
         """1st derivative of option price with respect to the strike price."""
         ...
 
@@ -224,14 +233,15 @@
         return {"in_the_money": self.in_the_money(), "dual_delta": self.dual_delta()}
 
     def get_all_greeks(self) -> Dict[str, float]:
         """Retrieve all Greeks for the Black-Scholes-Merton model
         implemented as a dictionary."""
         return {
             "delta": self.delta(),
+            "forward_delta": self.forward_delta(),
             "gamma": self.gamma(),
             "vega": self.vega(),
             "theta": self.theta(),
             "epsilon": self.epsilon(),
             "rho": self.rho(),
             "lambda_greek": self.lambda_greek(),
             "vanna": self.vanna(),
@@ -409,14 +419,21 @@
 
     def delta(self) -> float:
         """Rate of change in structure price
         with respect to the asset price (1st derivative).
         """
         return self._calc_attr(attribute_name="delta")
 
+    def forward_delta(self) -> float:
+        """
+        Delta discounted for interest rates.
+        For the cash/spot delta, use `delta`.
+        """
+        return self._calc_attr(attribute_name="forward_delta")
+
     def dual_delta(self) -> float:
         """1st derivative in structure price
         with respect to strike price.
         """
         return self._calc_attr(attribute_name="dual_delta")
 
     def theta(self) -> float:
@@ -520,14 +537,15 @@
         }
 
     def get_all_greeks(self) -> Dict[str, float]:
         """Retrieve all Greeks for the compound
         implemented as a dictionary."""
         return {
             "delta": self.delta(),
+            "forward_delta": self.forward_delta(),
             "gamma": self.gamma(),
             "vega": self.vega(),
             "theta": self.theta(),
             "epsilon": self.epsilon(),
             "rho": self.rho(),
             "lambda_greek": self.lambda_greek(),
             "vanna": self.vanna(),
```

### Comparing `blackscholes-0.1.2/blackscholes/butterfly.py` & `blackscholes-0.1.3/blackscholes/butterfly.py`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.2/blackscholes/call.py` & `blackscholes-0.1.3/blackscholes/call.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,19 +26,29 @@
         return (
             self.S * exp(-self.q * self.T) * self._cdf(self._d1)
             - self._cdf(self._d2) * exp(-self.r * self.T) * self.K
         )
 
     def delta(self) -> float:
         """Rate of change in option price
-        with respect to the asset price (1st derivative).
+        with respect to the forward price (1st derivative).
+        In other words, delta discounted for interest rates.
         Proxy for probability of the option expiring in the money.
+        Note that this is the forward delta.
+        For the cash/spot delta, use `spot_delta`.
         """
         return exp(-self.q * self.T) * self._cdf(self._d1)
 
+    def forward_delta(self) -> float:
+        """
+        Delta discounted for interest rates.
+        For the cash/spot delta, use `delta`.
+        """
+        return exp((self.r - self.q) * self.T) * self._cdf(self._d1)
+
     def dual_delta(self) -> float:
         """1st derivative in option price
         with respect to strike price.
         """
         return exp(-self.r * self.T) * self._cdf(self._d2)
 
     def theta(self) -> float:
```

### Comparing `blackscholes-0.1.2/blackscholes/iron_butterfly.py` & `blackscholes-0.1.3/blackscholes/iron_butterfly.py`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.2/blackscholes/iron_condor.py` & `blackscholes-0.1.3/blackscholes/iron_condor.py`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.2/blackscholes/put.py` & `blackscholes-0.1.3/blackscholes/put.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,17 +26,27 @@
         return self._cdf(-self._d2) * self.K * exp(-self.r * self.T) - self.S * exp(
             -self.q * self.T
         ) * self._cdf(-self._d1)
 
     def delta(self) -> float:
         """
         Rate of change in option price
-        with respect to the asset price (1st derivative).
+        with respect to the forward price (1st derivative).
+        In other words, delta discounted for interest rates.
+        Note that this is the forward delta.
+        For the cash/spot delta, use `spot_delta`.
         """
-        return -exp(-self.q * self.T) * self._cdf(-self._d1)
+        return exp(-self.q * self.T) * (self._cdf(self._d1) - 1)
+
+    def forward_delta(self) -> float:
+        """
+        Delta discounted for interest rates.
+        For the cash/spot delta, use `delta`.
+        """
+        return exp((self.r - self.q) * self.T) * (self._cdf(self._d1) - 1)
 
     def dual_delta(self) -> float:
         """1st derivative in option price
         with respect to strike price.
         """
         return exp(-self.r * self.T) * self._cdf(-self._d2)
```

### Comparing `blackscholes-0.1.2/blackscholes/spread.py` & `blackscholes-0.1.3/blackscholes/spread.py`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.2/blackscholes/straddle.py` & `blackscholes-0.1.3/blackscholes/straddle.py`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.2/blackscholes/strangle.py` & `blackscholes-0.1.3/blackscholes/strangle.py`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.2/blackscholes/tests/test_base.py` & `blackscholes-0.1.3/blackscholes/tests/test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 
     def in_the_money(self):
         ...
 
     def delta(self):
         ...
 
+    def forward_delta(self):
+        ...
+
     def dual_delta(self):
         ...
 
     def theta(self):
         ...
 
     def epsilon(self):
```

### Comparing `blackscholes-0.1.2/blackscholes/tests/test_butterfly.py` & `blackscholes-0.1.3/blackscholes/tests/test_butterfly.py`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.2/blackscholes/tests/test_call.py` & `blackscholes-0.1.3/blackscholes/tests/test_call.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,14 +27,33 @@
             K=test_K,
             T=test_T,
             r=test_r,
             sigma=test_sigma,
         )
         np.testing.assert_almost_equal(call_delta - put.delta(), 1.0, decimal=5)
 
+    def test_forward_delta(self):
+        call_forward_delta = self.call.forward_delta()
+
+        np.testing.assert_almost_equal(
+            call_forward_delta, 0.7683262250522389, decimal=6
+        )
+
+        # Due to put-call parity, Call forward delta + Put forward delta should be 1.
+        put = BlackScholesPut(
+            S=test_S,
+            K=test_K,
+            T=test_T,
+            r=test_r,
+            sigma=test_sigma,
+        )
+        np.testing.assert_almost_equal(
+            call_forward_delta - put.forward_delta(), 1.0, decimal=2
+        )
+
     def test_dual_delta(self):
         call_delta = self.call.dual_delta()
         assert 0.0 < call_delta < 1.0
         np.testing.assert_almost_equal(call_delta, 0.7162603034383217, decimal=6)
 
         # Due to put-call parity, Put dual delta + call dual delta should be 1.
         put = BlackScholesPut(
@@ -108,14 +127,15 @@
         charm = self.call.charm()
         np.testing.assert_almost_equal(charm, 0.0832677717846717, decimal=6)
 
     def test_all_greeks(self):
         all_greeks = self.call.get_all_greeks()
         expected_result = {
             "delta": 0.766407808509462,
+            "forward_delta": 0.7683262250522389,
             "gamma": 0.03712496688031454,
             "vega": 16.84545372194272,
             "theta": -1.3529415670754943,
             "epsilon": -42.15242946802041,
             "rho": 35.813015171916085,
             "lambda_greek": 6.6492624553539255,
             "vanna": -1.178299396409533,
```

### Comparing `blackscholes-0.1.2/blackscholes/tests/test_iron_butterfly.py` & `blackscholes-0.1.3/blackscholes/tests/test_iron_butterfly.py`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.2/blackscholes/tests/test_iron_condor.py` & `blackscholes-0.1.3/blackscholes/tests/test_iron_condor.py`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.2/blackscholes/tests/test_put.py` & `blackscholes-0.1.3/blackscholes/tests/test_put.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,14 +27,32 @@
             K=test_K,
             T=test_T,
             r=test_r,
             sigma=test_sigma,
         )
         np.testing.assert_almost_equal(call.delta() - put_delta, 1.0, decimal=5)
 
+    def test_forward_delta(self):
+        put_forward_delta = self.put.forward_delta()
+        np.testing.assert_almost_equal(
+            put_forward_delta, -0.23417690255355628, decimal=6
+        )
+
+        # Due to put-call parity, Call forward delta + Put forward delta should be 1.
+        call = BlackScholesCall(
+            S=test_S,
+            K=test_K,
+            T=test_T,
+            r=test_r,
+            sigma=test_sigma,
+        )
+        np.testing.assert_almost_equal(
+            call.forward_delta() - put_forward_delta, 1.0, decimal=2
+        )
+
     def test_dual_delta(self):
         put_delta = self.put.dual_delta()
         assert 0.0 < put_delta < 1.0
         np.testing.assert_almost_equal(put_delta, 0.2812428189591384, decimal=6)
 
         # Due to put-call parity, Call dual delta + Put dual delta should be 1.
         call = BlackScholesCall(
@@ -94,14 +112,15 @@
         assert 0.0 < itm_prob < 1.0
         np.testing.assert_almost_equal(itm_prob, 0.2819468056232066, decimal=6)
 
     def test_all_greeks(self):
         all_greeks = self.put.get_all_greeks()
         expected_result = {
             "delta": -0.233592191490538,
+            "forward_delta": -0.23417690255355628,
             "gamma": 0.03712496688031454,
             "vega": 16.84545372194272,
             "theta": -1.2282536767758119,
             "epsilon": 12.84757053197959,
             "rho": -14.062140947956918,
             "lambda_greek": -10.57787211261979,
             "vanna": -1.178299396409533,
```

### Comparing `blackscholes-0.1.2/blackscholes/tests/test_spread.py` & `blackscholes-0.1.3/blackscholes/tests/test_spread.py`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.2/blackscholes/tests/test_straddle.py` & `blackscholes-0.1.3/blackscholes/tests/test_straddle.py`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.2/blackscholes/tests/test_strangle.py` & `blackscholes-0.1.3/blackscholes/tests/test_strangle.py`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.2/pyproject.toml` & `blackscholes-0.1.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blackscholes"
-version = "0.1.2"
+version = "0.1.3"
 description = "Black Scholes calculator for Python including all Greeks"
 authors = ["CarloLepelaars <info@carlolepelaars.nl>"]
 license = "MIT"
 readme = ".github/README.MD"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `blackscholes-0.1.2/setup.py` & `blackscholes-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,117 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: blackscholes
+Version: 0.1.3
+Summary: Black Scholes calculator for Python including all Greeks
+License: MIT
+Author: CarloLepelaars
+Author-email: info@carlolepelaars.nl
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/plain
 
-packages = \
-['blackscholes', 'blackscholes.tests']
+# blackscholes
 
-package_data = \
-{'': ['*']}
+![](https://img.shields.io/pypi/dm/blackscholes) | 
+![](https://img.shields.io/pypi/pyversions/blackscholes)
 
-setup_kwargs = {
-    'name': 'blackscholes',
-    'version': '0.1.2',
-    'description': 'Black Scholes calculator for Python including all Greeks',
-    'long_description': '# blackscholes\n\n![](https://img.shields.io/pypi/dm/blackscholes) | \n![](https://img.shields.io/pypi/pyversions/blackscholes)\n\nBlack Scholes calculator for Python including all Greeks.\n\nSupports the Black-Scholes-Merton model, \nBlack-76 model and option structures.\n\n## Installation\n\n`pip install blackscholes`\n\n## Examples\n\n### Input variables\n```python3\nS = 55.0  # Asset price of 55\nK = 50.0  # Strike price of 50\nT = 1.0  # 1 Year to maturity\nr = 0.0025  # 0.25% Risk-free rate\nsigma = 0.15  # 15% Volatility\nq = 0.0 # 0% Annual Dividend Yield\n```\n\n### Call\n\n```python3\nfrom blackscholes import BlackScholesCall\ncall = BlackScholesCall(S=S, K=K, T=T, r=r, sigma=sigma, q=q)\ncall.price()  ## 6.339408\ncall.delta()  ## 0.766407\ncall.charm()  ## 0.083267\n```\n\n### Put\n\n```python3\nfrom blackscholes import BlackScholesPut\nput = BlackScholesPut(S=S, K=K, T=T, r=r, sigma=sigma, q=q)\nput.price()  ## 1.214564\nput.delta()  ## -0.23359\nput.charm()  ## 0.083267\n```\n\n### Black-76\n\nThe Black-76 model is often used specifically for options and futures and bonds.\n`blackscholes` also supports this model. To see all available greeks\ncheck out section [4. The Greeks (Black-76)](https://carlolepelaars.github.io/blackscholes/4.the_greeks_black76).\n\n**Call Example**\n```python\nfrom blackscholes import Black76Call\ncall = Black76Call(F=55, K=50, T=1, r=0.0025, sigma=0.15)\ncall.price()  ## 6.2345\ncall.delta()  ## 0.7594\ncall.vomma()  ## 45.1347\n```\n\n**Put Example**\n```python\nfrom blackscholes import Black76Put\nput = Black76Put(F=55, K=50, T=1, r=0.0025, sigma=0.15)\nput.price()  ## 1.2470\nput.delta()  ## -0.2381\nput.vomma()  ## 45.1347\n```\n\n### Structures\n\n`blackscholes` offers the following four option structures:\n- Straddle\n- Strangle\n- Butterfly\n- Iron Condor\n- Spreads\n- Iron Butterfly\n\nAll structures have a long and short version. To learn more\ncheck out section [6. Option Structures](https://carlolepelaars.github.io/blackscholes/6.option_structures).\n\n**Long Straddle Example**\n```python3\nfrom blackscholes import BlackScholesStraddleLong\n\nstraddle = BlackScholesStraddleLong(S=55, K=50, T=1.0,\n                                    r=0.0025, sigma=0.15)\nstraddle.price()  ## 7.5539\nstraddle.delta()  ## 0.5328\n```\n\n## Contributing\n\nWe very much welcome new contributions! Check out the [Github Issues](https://github.com/CarloLepelaars/blackscholes/issues)\nto see what is currently being worked on.\n\nAlso check out [Contributing](https://carlolepelaars.github.io/blackscholes/contributing) in the documentation \nto learn more about \ncontributing to [blackscholes](https://github.com/CarloLepelaars/blackscholes).\n',
-    'author': 'CarloLepelaars',
-    'author_email': 'info@carlolepelaars.nl',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.8.1,<4.0.0',
-}
+Black Scholes calculator for Python including all Greeks.
 
+Supports the Black-Scholes-Merton model, 
+Black-76 model and option structures.
+
+## Installation
+
+`pip install blackscholes`
+
+## Examples
+
+### Input variables
+```python3
+S = 55.0  # Asset price of 55
+K = 50.0  # Strike price of 50
+T = 1.0  # 1 Year to maturity
+r = 0.0025  # 0.25% Risk-free rate
+sigma = 0.15  # 15% Volatility
+q = 0.0 # 0% Annual Dividend Yield
+```
+
+### Call
+
+```python3
+from blackscholes import BlackScholesCall
+call = BlackScholesCall(S=S, K=K, T=T, r=r, sigma=sigma, q=q)
+call.price()  ## 6.339408
+call.delta()  ## 0.766407
+call.charm()  ## 0.083267
+```
+
+### Put
+
+```python3
+from blackscholes import BlackScholesPut
+put = BlackScholesPut(S=S, K=K, T=T, r=r, sigma=sigma, q=q)
+put.price()  ## 1.214564
+put.delta()  ## -0.23359
+put.charm()  ## 0.083267
+```
+
+### Black-76
+
+The Black-76 model is often used specifically for options and futures and bonds.
+`blackscholes` also supports this model. To see all available greeks
+check out section [4. The Greeks (Black-76)](https://carlolepelaars.github.io/blackscholes/4.the_greeks_black76).
+
+**Call Example**
+```python
+from blackscholes import Black76Call
+call = Black76Call(F=55, K=50, T=1, r=0.0025, sigma=0.15)
+call.price()  ## 6.2345
+call.delta()  ## 0.7594
+call.vomma()  ## 45.1347
+```
+
+**Put Example**
+```python
+from blackscholes import Black76Put
+put = Black76Put(F=55, K=50, T=1, r=0.0025, sigma=0.15)
+put.price()  ## 1.2470
+put.delta()  ## -0.2381
+put.vomma()  ## 45.1347
+```
+
+### Structures
+
+`blackscholes` offers the following six option structures:
+- Straddle
+- Strangle
+- Butterfly
+- Iron Condor
+- Spreads
+- Iron Butterfly
+
+All structures have a long and short version. To learn more
+check out section [6. Option Structures](https://carlolepelaars.github.io/blackscholes/6.option_structures).
+
+**Long Straddle Example**
+```python3
+from blackscholes import BlackScholesStraddleLong
+
+straddle = BlackScholesStraddleLong(S=55, K=50, T=1.0,
+                                    r=0.0025, sigma=0.15)
+straddle.price()  ## 7.5539
+straddle.delta()  ## 0.5328
+```
+
+## Contributing
+
+We very much welcome new contributions! Check out the [Github Issues](https://github.com/CarloLepelaars/blackscholes/issues)
+to see what is currently being worked on.
+
+Also check out [Contributing](https://carlolepelaars.github.io/blackscholes/contributing) in the documentation 
+to learn more about 
+contributing to [blackscholes](https://github.com/CarloLepelaars/blackscholes).
 
-setup(**setup_kwargs)
```

