# Comparing `tmp/blackscholes-0.1.3.tar.gz` & `tmp/blackscholes-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackscholes-0.1.3.tar", max compression
+gzip compressed data, was "blackscholes-0.1.4.tar", max compression
```

## Comparing `blackscholes-0.1.3.tar` & `blackscholes-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     2615 2022-12-26 13:11:12.753657 blackscholes-0.1.3/.github/README.MD
--rw-r--r--   0        0        0     1065 2022-12-16 00:32:50.227092 blackscholes-0.1.3/LICENSE
--rw-r--r--   0        0        0     1069 2022-12-25 21:50:07.012322 blackscholes-0.1.3/blackscholes/__init__.py
--rw-r--r--   0        0        0    18417 2023-06-15 20:15:48.324717 blackscholes-0.1.3/blackscholes/base.py
--rw-r--r--   0        0        0     4559 2022-12-25 21:04:57.343636 blackscholes-0.1.3/blackscholes/butterfly.py
--rw-r--r--   0        0        0     5085 2023-06-15 20:15:48.325380 blackscholes-0.1.3/blackscholes/call.py
--rw-r--r--   0        0        0     4907 2022-12-25 21:53:11.338043 blackscholes-0.1.3/blackscholes/iron_butterfly.py
--rw-r--r--   0        0        0     4948 2022-12-25 21:04:57.336856 blackscholes-0.1.3/blackscholes/iron_condor.py
--rw-r--r--   0        0        0     4643 2023-06-15 20:15:48.325025 blackscholes-0.1.3/blackscholes/put.py
--rw-r--r--   0        0        0     3517 2022-12-25 21:04:57.348936 blackscholes-0.1.3/blackscholes/spread.py
--rw-r--r--   0        0        0     2986 2022-12-25 21:04:57.360596 blackscholes-0.1.3/blackscholes/straddle.py
--rw-r--r--   0        0        0     3530 2022-12-25 21:04:57.356473 blackscholes-0.1.3/blackscholes/strangle.py
--rw-r--r--   0        0        0        0 2022-12-03 15:33:29.510748 blackscholes-0.1.3/blackscholes/tests/__init__.py
--rw-r--r--   0        0        0     6640 2023-06-15 19:55:02.922009 blackscholes-0.1.3/blackscholes/tests/test_base.py
--rw-r--r--   0        0        0     2929 2022-12-23 17:07:16.664773 blackscholes-0.1.3/blackscholes/tests/test_butterfly.py
--rw-r--r--   0        0        0     7672 2023-06-15 20:15:50.924398 blackscholes-0.1.3/blackscholes/tests/test_call.py
--rw-r--r--   0        0        0     4869 2022-12-25 21:53:22.902241 blackscholes-0.1.3/blackscholes/tests/test_iron_butterfly.py
--rw-r--r--   0        0        0     4451 2022-12-25 21:35:16.300406 blackscholes-0.1.3/blackscholes/tests/test_iron_condor.py
--rw-r--r--   0        0        0     7200 2023-06-15 20:15:50.922889 blackscholes-0.1.3/blackscholes/tests/test_put.py
--rw-r--r--   0        0        0     1788 2022-12-25 21:19:56.874737 blackscholes-0.1.3/blackscholes/tests/test_spread.py
--rw-r--r--   0        0        0     1271 2022-12-23 16:06:33.794443 blackscholes-0.1.3/blackscholes/tests/test_straddle.py
--rw-r--r--   0        0        0     1836 2022-12-23 16:07:20.353283 blackscholes-0.1.3/blackscholes/tests/test_strangle.py
--rw-r--r--   0        0        0      627 2023-06-15 20:15:20.388997 blackscholes-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3132 1970-01-01 00:00:00.000000 blackscholes-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2615 2022-12-26 13:11:12.753657 blackscholes-0.1.4/.github/README.MD
+-rw-r--r--   0        0        0     1065 2022-12-16 00:32:50.227092 blackscholes-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1069 2022-12-25 21:50:07.012322 blackscholes-0.1.4/blackscholes/__init__.py
+-rw-r--r--   0        0        0    18483 2023-06-15 20:48:41.202205 blackscholes-0.1.4/blackscholes/base.py
+-rw-r--r--   0        0        0     4559 2022-12-25 21:04:57.343636 blackscholes-0.1.4/blackscholes/butterfly.py
+-rw-r--r--   0        0        0     4947 2023-06-15 20:47:14.538021 blackscholes-0.1.4/blackscholes/call.py
+-rw-r--r--   0        0        0     4907 2022-12-25 21:53:11.338043 blackscholes-0.1.4/blackscholes/iron_butterfly.py
+-rw-r--r--   0        0        0     4948 2022-12-25 21:04:57.336856 blackscholes-0.1.4/blackscholes/iron_condor.py
+-rw-r--r--   0        0        0     4575 2023-06-15 20:47:24.179402 blackscholes-0.1.4/blackscholes/put.py
+-rw-r--r--   0        0        0     3517 2022-12-25 21:04:57.348936 blackscholes-0.1.4/blackscholes/spread.py
+-rw-r--r--   0        0        0     2986 2022-12-25 21:04:57.360596 blackscholes-0.1.4/blackscholes/straddle.py
+-rw-r--r--   0        0        0     3530 2022-12-25 21:04:57.356473 blackscholes-0.1.4/blackscholes/strangle.py
+-rw-r--r--   0        0        0        0 2022-12-03 15:33:29.510748 blackscholes-0.1.4/blackscholes/tests/__init__.py
+-rw-r--r--   0        0        0     6637 2023-06-15 20:48:57.836625 blackscholes-0.1.4/blackscholes/tests/test_base.py
+-rw-r--r--   0        0        0     2929 2022-12-23 17:07:16.664773 blackscholes-0.1.4/blackscholes/tests/test_butterfly.py
+-rw-r--r--   0        0        0     7645 2023-06-15 20:50:32.524093 blackscholes-0.1.4/blackscholes/tests/test_call.py
+-rw-r--r--   0        0        0     4869 2022-12-25 21:53:22.902241 blackscholes-0.1.4/blackscholes/tests/test_iron_butterfly.py
+-rw-r--r--   0        0        0     4451 2022-12-25 21:35:16.300406 blackscholes-0.1.4/blackscholes/tests/test_iron_condor.py
+-rw-r--r--   0        0        0     7173 2023-06-15 20:50:27.335599 blackscholes-0.1.4/blackscholes/tests/test_put.py
+-rw-r--r--   0        0        0     1788 2022-12-25 21:19:56.874737 blackscholes-0.1.4/blackscholes/tests/test_spread.py
+-rw-r--r--   0        0        0     1271 2022-12-23 16:06:33.794443 blackscholes-0.1.4/blackscholes/tests/test_straddle.py
+-rw-r--r--   0        0        0     1836 2022-12-23 16:07:20.353283 blackscholes-0.1.4/blackscholes/tests/test_strangle.py
+-rw-r--r--   0        0        0      627 2023-06-15 20:51:03.969491 blackscholes-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3132 1970-01-01 00:00:00.000000 blackscholes-0.1.4/PKG-INFO
```

### Comparing `blackscholes-0.1.3/.github/README.MD` & `blackscholes-0.1.4/.github/README.MD`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.3/LICENSE` & `blackscholes-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.3/blackscholes/__init__.py` & `blackscholes-0.1.4/blackscholes/__init__.py`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.3/blackscholes/base.py` & `blackscholes-0.1.4/blackscholes/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,18 +57,18 @@
     def delta(self) -> float:
         """Rate of change in option price
         with respect to the forward price (1st derivative).
         """
         ...
 
     @abstractmethod
-    def forward_delta(self) -> float:
+    def spot_delta(self) -> float:
         """
         Delta discounted for interest rates.
-        For the cash/spot delta, use `delta`.
+        For the forward delta, use `delta`.
         """
         ...
 
     @abstractmethod
     def dual_delta(self) -> float:
         """1st derivative of option price with respect to the strike price."""
         ...
@@ -233,15 +233,15 @@
         return {"in_the_money": self.in_the_money(), "dual_delta": self.dual_delta()}
 
     def get_all_greeks(self) -> Dict[str, float]:
         """Retrieve all Greeks for the Black-Scholes-Merton model
         implemented as a dictionary."""
         return {
             "delta": self.delta(),
-            "forward_delta": self.forward_delta(),
+            "spot_delta": self.spot_delta(),
             "gamma": self.gamma(),
             "vega": self.vega(),
             "theta": self.theta(),
             "epsilon": self.epsilon(),
             "rho": self.rho(),
             "lambda_greek": self.lambda_greek(),
             "vanna": self.vanna(),
@@ -416,23 +416,25 @@
     def price(self) -> float:
         """Fair value of Black-Scholes option structure."""
         return self._calc_attr(attribute_name="price")
 
     def delta(self) -> float:
         """Rate of change in structure price
         with respect to the asset price (1st derivative).
+        Note that this is the forward delta.
+        For the spot delta, use `spot_delta`.
         """
         return self._calc_attr(attribute_name="delta")
 
-    def forward_delta(self) -> float:
+    def spot_delta(self) -> float:
         """
         Delta discounted for interest rates.
-        For the cash/spot delta, use `delta`.
+        For the forward delta, use `delta`.
         """
-        return self._calc_attr(attribute_name="forward_delta")
+        return self._calc_attr(attribute_name="spot_delta")
 
     def dual_delta(self) -> float:
         """1st derivative in structure price
         with respect to strike price.
         """
         return self._calc_attr(attribute_name="dual_delta")
 
@@ -537,15 +539,15 @@
         }
 
     def get_all_greeks(self) -> Dict[str, float]:
         """Retrieve all Greeks for the compound
         implemented as a dictionary."""
         return {
             "delta": self.delta(),
-            "forward_delta": self.forward_delta(),
+            "spot_delta": self.spot_delta(),
             "gamma": self.gamma(),
             "vega": self.vega(),
             "theta": self.theta(),
             "epsilon": self.epsilon(),
             "rho": self.rho(),
             "lambda_greek": self.lambda_greek(),
             "vanna": self.vanna(),
```

### Comparing `blackscholes-0.1.3/blackscholes/butterfly.py` & `blackscholes-0.1.4/blackscholes/butterfly.py`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.3/blackscholes/call.py` & `blackscholes-0.1.4/blackscholes/call.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,25 +27,23 @@
             self.S * exp(-self.q * self.T) * self._cdf(self._d1)
             - self._cdf(self._d2) * exp(-self.r * self.T) * self.K
         )
 
     def delta(self) -> float:
         """Rate of change in option price
         with respect to the forward price (1st derivative).
-        In other words, delta discounted for interest rates.
-        Proxy for probability of the option expiring in the money.
         Note that this is the forward delta.
-        For the cash/spot delta, use `spot_delta`.
+        For the spot delta, use `spot_delta`.
         """
         return exp(-self.q * self.T) * self._cdf(self._d1)
 
-    def forward_delta(self) -> float:
+    def spot_delta(self) -> float:
         """
         Delta discounted for interest rates.
-        For the cash/spot delta, use `delta`.
+        For the forward delta, use `delta`.
         """
         return exp((self.r - self.q) * self.T) * self._cdf(self._d1)
 
     def dual_delta(self) -> float:
         """1st derivative in option price
         with respect to strike price.
         """
```

### Comparing `blackscholes-0.1.3/blackscholes/iron_butterfly.py` & `blackscholes-0.1.4/blackscholes/iron_butterfly.py`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.3/blackscholes/iron_condor.py` & `blackscholes-0.1.4/blackscholes/iron_condor.py`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.3/blackscholes/put.py` & `blackscholes-0.1.4/blackscholes/put.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,24 +27,23 @@
             -self.q * self.T
         ) * self._cdf(-self._d1)
 
     def delta(self) -> float:
         """
         Rate of change in option price
         with respect to the forward price (1st derivative).
-        In other words, delta discounted for interest rates.
-        Note that this is the forward delta.
-        For the cash/spot delta, use `spot_delta`.
+        Note that this is the spot delta.
+        For the forward delta, use `forward_delta`.
         """
         return exp(-self.q * self.T) * (self._cdf(self._d1) - 1)
 
-    def forward_delta(self) -> float:
+    def spot_delta(self) -> float:
         """
         Delta discounted for interest rates.
-        For the cash/spot delta, use `delta`.
+        For the forward delta, use `delta`.
         """
         return exp((self.r - self.q) * self.T) * (self._cdf(self._d1) - 1)
 
     def dual_delta(self) -> float:
         """1st derivative in option price
         with respect to strike price.
         """
```

### Comparing `blackscholes-0.1.3/blackscholes/spread.py` & `blackscholes-0.1.4/blackscholes/spread.py`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.3/blackscholes/straddle.py` & `blackscholes-0.1.4/blackscholes/straddle.py`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.3/blackscholes/strangle.py` & `blackscholes-0.1.4/blackscholes/strangle.py`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.3/blackscholes/tests/test_base.py` & `blackscholes-0.1.4/blackscholes/tests/test_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     def in_the_money(self):
         ...
 
     def delta(self):
         ...
 
-    def forward_delta(self):
+    def spot_delta(self):
         ...
 
     def dual_delta(self):
         ...
 
     def theta(self):
         ...
```

### Comparing `blackscholes-0.1.3/blackscholes/tests/test_butterfly.py` & `blackscholes-0.1.4/blackscholes/tests/test_butterfly.py`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.3/blackscholes/tests/test_call.py` & `blackscholes-0.1.4/blackscholes/tests/test_call.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,31 +27,31 @@
             K=test_K,
             T=test_T,
             r=test_r,
             sigma=test_sigma,
         )
         np.testing.assert_almost_equal(call_delta - put.delta(), 1.0, decimal=5)
 
-    def test_forward_delta(self):
-        call_forward_delta = self.call.forward_delta()
+    def test_spot_delta(self):
+        call_spot_delta = self.call.spot_delta()
 
         np.testing.assert_almost_equal(
-            call_forward_delta, 0.7683262250522389, decimal=6
+            call_spot_delta, 0.7683262250522389, decimal=6
         )
 
-        # Due to put-call parity, Call forward delta + Put forward delta should be 1.
+        # Due to put-call parity, Call spot delta + Put spot delta should be 1.
         put = BlackScholesPut(
             S=test_S,
             K=test_K,
             T=test_T,
             r=test_r,
             sigma=test_sigma,
         )
         np.testing.assert_almost_equal(
-            call_forward_delta - put.forward_delta(), 1.0, decimal=2
+            call_spot_delta - put.spot_delta(), 1.0, decimal=2
         )
 
     def test_dual_delta(self):
         call_delta = self.call.dual_delta()
         assert 0.0 < call_delta < 1.0
         np.testing.assert_almost_equal(call_delta, 0.7162603034383217, decimal=6)
 
@@ -127,15 +127,15 @@
         charm = self.call.charm()
         np.testing.assert_almost_equal(charm, 0.0832677717846717, decimal=6)
 
     def test_all_greeks(self):
         all_greeks = self.call.get_all_greeks()
         expected_result = {
             "delta": 0.766407808509462,
-            "forward_delta": 0.7683262250522389,
+            "spot_delta": 0.7683262250522389,
             "gamma": 0.03712496688031454,
             "vega": 16.84545372194272,
             "theta": -1.3529415670754943,
             "epsilon": -42.15242946802041,
             "rho": 35.813015171916085,
             "lambda_greek": 6.6492624553539255,
             "vanna": -1.178299396409533,
```

### Comparing `blackscholes-0.1.3/blackscholes/tests/test_iron_butterfly.py` & `blackscholes-0.1.4/blackscholes/tests/test_iron_butterfly.py`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.3/blackscholes/tests/test_iron_condor.py` & `blackscholes-0.1.4/blackscholes/tests/test_iron_condor.py`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.3/blackscholes/tests/test_put.py` & `blackscholes-0.1.4/blackscholes/tests/test_put.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,30 +27,30 @@
             K=test_K,
             T=test_T,
             r=test_r,
             sigma=test_sigma,
         )
         np.testing.assert_almost_equal(call.delta() - put_delta, 1.0, decimal=5)
 
-    def test_forward_delta(self):
-        put_forward_delta = self.put.forward_delta()
+    def test_spot_delta(self):
+        put_spot_delta = self.put.spot_delta()
         np.testing.assert_almost_equal(
-            put_forward_delta, -0.23417690255355628, decimal=6
+            put_spot_delta, -0.23417690255355628, decimal=6
         )
 
-        # Due to put-call parity, Call forward delta + Put forward delta should be 1.
+        # Due to put-call parity, Call spot delta + Put spot delta should be 1.
         call = BlackScholesCall(
             S=test_S,
             K=test_K,
             T=test_T,
             r=test_r,
             sigma=test_sigma,
         )
         np.testing.assert_almost_equal(
-            call.forward_delta() - put_forward_delta, 1.0, decimal=2
+            call.spot_delta() - put_spot_delta, 1.0, decimal=2
         )
 
     def test_dual_delta(self):
         put_delta = self.put.dual_delta()
         assert 0.0 < put_delta < 1.0
         np.testing.assert_almost_equal(put_delta, 0.2812428189591384, decimal=6)
 
@@ -112,15 +112,15 @@
         assert 0.0 < itm_prob < 1.0
         np.testing.assert_almost_equal(itm_prob, 0.2819468056232066, decimal=6)
 
     def test_all_greeks(self):
         all_greeks = self.put.get_all_greeks()
         expected_result = {
             "delta": -0.233592191490538,
-            "forward_delta": -0.23417690255355628,
+            "spot_delta": -0.23417690255355628,
             "gamma": 0.03712496688031454,
             "vega": 16.84545372194272,
             "theta": -1.2282536767758119,
             "epsilon": 12.84757053197959,
             "rho": -14.062140947956918,
             "lambda_greek": -10.57787211261979,
             "vanna": -1.178299396409533,
```

### Comparing `blackscholes-0.1.3/blackscholes/tests/test_spread.py` & `blackscholes-0.1.4/blackscholes/tests/test_spread.py`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.3/blackscholes/tests/test_straddle.py` & `blackscholes-0.1.4/blackscholes/tests/test_straddle.py`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.3/blackscholes/tests/test_strangle.py` & `blackscholes-0.1.4/blackscholes/tests/test_strangle.py`

 * *Files identical despite different names*

### Comparing `blackscholes-0.1.3/pyproject.toml` & `blackscholes-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blackscholes"
-version = "0.1.3"
+version = "0.1.4"
 description = "Black Scholes calculator for Python including all Greeks"
 authors = ["CarloLepelaars <info@carlolepelaars.nl>"]
 license = "MIT"
 readme = ".github/README.MD"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `blackscholes-0.1.3/PKG-INFO` & `blackscholes-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackscholes
-Version: 0.1.3
+Version: 0.1.4
 Summary: Black Scholes calculator for Python including all Greeks
 License: MIT
 Author: CarloLepelaars
 Author-email: info@carlolepelaars.nl
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

