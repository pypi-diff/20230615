# Comparing `tmp/btg_investment_flow_portfolio_optimization-0.0.1.tar.gz` & `tmp/btg_investment_flow_portfolio_optimization-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btg_investment_flow_portfolio_optimization-0.0.1.tar", max compression
+gzip compressed data, was "btg_investment_flow_portfolio_optimization-0.0.2.tar", max compression
```

## Comparing `btg_investment_flow_portfolio_optimization-0.0.1.tar` & `btg_investment_flow_portfolio_optimization-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-07 00:32:09.864536 btg_investment_flow_portfolio_optimization-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-06-07 00:32:09.864536 btg_investment_flow_portfolio_optimization-0.0.1/btg_investment_flow_portfolio_optimization/__init__.py
--rw-r--r--   0        0        0     3454 2023-06-07 00:32:09.841536 btg_investment_flow_portfolio_optimization-0.0.1/btg_investment_flow_portfolio_optimization/btg_api.py
--rw-r--r--   0        0        0     7953 2023-06-07 00:32:09.841536 btg_investment_flow_portfolio_optimization-0.0.1/btg_investment_flow_portfolio_optimization/portfolio_optimization.py
--rw-r--r--   0        0        0     3846 2023-06-07 00:32:09.842536 btg_investment_flow_portfolio_optimization-0.0.1/btg_investment_flow_portfolio_optimization/standard.py
--rw-r--r--   0        0        0      345 2023-06-07 00:32:09.842536 btg_investment_flow_portfolio_optimization-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 btg_investment_flow_portfolio_optimization-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-15 19:57:03.034514 btg_investment_flow_portfolio_optimization-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-15 19:57:03.035514 btg_investment_flow_portfolio_optimization-0.0.2/btg_investment_flow_portfolio_optimization/__init__.py
+-rw-r--r--   0        0        0     3454 2023-06-15 19:57:03.012514 btg_investment_flow_portfolio_optimization-0.0.2/btg_investment_flow_portfolio_optimization/btg_api.py
+-rw-r--r--   0        0        0     7953 2023-06-15 19:57:03.012514 btg_investment_flow_portfolio_optimization-0.0.2/btg_investment_flow_portfolio_optimization/portfolio_optimization.py
+-rw-r--r--   0        0        0     4701 2023-06-15 19:57:03.012514 btg_investment_flow_portfolio_optimization-0.0.2/btg_investment_flow_portfolio_optimization/standard.py
+-rw-r--r--   0        0        0      345 2023-06-15 19:57:03.012514 btg_investment_flow_portfolio_optimization-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 btg_investment_flow_portfolio_optimization-0.0.2/PKG-INFO
```

### Comparing `btg_investment_flow_portfolio_optimization-0.0.1/btg_investment_flow_portfolio_optimization/btg_api.py` & `btg_investment_flow_portfolio_optimization-0.0.2/btg_investment_flow_portfolio_optimization/btg_api.py`

 * *Files identical despite different names*

### Comparing `btg_investment_flow_portfolio_optimization-0.0.1/btg_investment_flow_portfolio_optimization/portfolio_optimization.py` & `btg_investment_flow_portfolio_optimization-0.0.2/btg_investment_flow_portfolio_optimization/portfolio_optimization.py`

 * *Files identical despite different names*

### Comparing `btg_investment_flow_portfolio_optimization-0.0.1/btg_investment_flow_portfolio_optimization/standard.py` & `btg_investment_flow_portfolio_optimization-0.0.2/btg_investment_flow_portfolio_optimization/standard.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from btg_investment_flow_portfolio_optimization.portfolio_optimization import (
     PortfolioOptimizer,
 )
 
 import pandas as pd
-
+from datetime import datetime
+from typing import List, Tuple
 
 class StandardPortfolioOptimizer(PortfolioOptimizer):
     @staticmethod
     def sum_between_dates(df, start_date, end_date, quantile):
         """Calculate the sum of a quantile between two dates."""
         df.index = pd.to_datetime(df.index)
         start_date = pd.to_datetime(start_date)
@@ -20,45 +21,49 @@
 
         return subset_df[quantile].sum()
 
     def generate_time_slots(self, start_date, end_date):
         """Generate a list of intervals representing the starting and ending points of each time slot"""
         time_slots = []
         current_date = start_date
+
+        def calculate_interval_end_and_hour(current_date: datetime, end_date: datetime, days_to_add: int, hour_if_within_period: int, hour_if_exceeds_period: int) -> Tuple[datetime, int]:
+            proposed_end_date = current_date + pd.DateOffset(days=days_to_add)
+
+            if proposed_end_date <= end_date or current_date == end_date:
+                return proposed_end_date, hour_if_within_period
+            else:
+                return end_date, hour_if_exceeds_period
+
+        def append_time_slot(time_slots: List[Tuple[datetime, datetime]], interval_start: datetime, start_hour: int, interval_end: datetime, end_hour: int):
+            start = interval_start.replace(hour=start_hour, minute=0, second=0)
+            end = interval_end.replace(hour=end_hour, minute=0, second=0)
+            time_slots.append((start, end))
+
+
+        if start_date.weekday() not in [0,4]:
+            days_to_next_monday = (-start_date.weekday()) % 7
+            days_to_next_friday =(4-start_date.weekday()) % 7
+            offset = min(days_to_next_monday,days_to_next_friday)
+            next_recommendation = current_date + pd.DateOffset(days=offset)
+            next_recommendation_hour = 16 if days_to_next_monday > days_to_next_friday else 8
+            append_time_slot(time_slots, start_date, 9, next_recommendation, next_recommendation_hour)
+
         while current_date <= end_date:
-            if current_date.weekday() < 4:  # It's a weekday, but not Friday
-                time_slots.append(
-                    (
-                        current_date.replace(hour=9, minute=0, second=0),
-                        current_date.replace(hour=16, minute=0, second=0),
-                    )
-                )
-                next_day = current_date + pd.DateOffset(days=1)
-                time_slots.append(
-                    (
-                        current_date.replace(hour=17, minute=0, second=0),
-                        next_day.replace(hour=8, minute=0, second=0),
-                    )
-                )
-            elif current_date.weekday() == 4:  # It's Friday
-                time_slots.append(
-                    (
-                        current_date.replace(hour=9, minute=0, second=0),
-                        current_date.replace(hour=16, minute=0, second=0),
-                    )
-                )
-                next_monday = current_date + pd.DateOffset(
-                    days=(7 - current_date.weekday() % 7)
-                )
-                time_slots.append(
-                    (
-                        current_date.replace(hour=17, minute=0, second=0),
-                        next_monday.replace(hour=8, minute=0, second=0),
-                    )
-                )
+            if current_date.weekday() == 0:  # Monday
+                interval_start = current_date
+                interval_end, interval_end_hour = calculate_interval_end_and_hour(current_date, end_date, days_to_add=4, hour_if_within_period=16, hour_if_exceeds_period=16)
+                append_time_slot(time_slots, interval_start, 9, interval_end, interval_end_hour)
+
+            elif current_date.weekday() == 4:  # Friday
+                interval_start = current_date
+                interval_end, interval_end_hour = calculate_interval_end_and_hour(current_date, end_date, days_to_add=3, hour_if_within_period=8, hour_if_exceeds_period=16)
+                append_time_slot(time_slots, interval_start, 17, interval_end, interval_end_hour)
+
+                
             current_date += pd.DateOffset(days=1)
         return time_slots
 
     def optimize(self, quantile="0.5"):
         recommendations = {}
 
         # Convert date to datetime
```

### Comparing `btg_investment_flow_portfolio_optimization-0.0.1/PKG-INFO` & `btg_investment_flow_portfolio_optimization-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btg-investment-flow-portfolio-optimization
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: NG.CASH
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

