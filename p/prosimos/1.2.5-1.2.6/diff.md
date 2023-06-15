# Comparing `tmp/prosimos-1.2.5.tar.gz` & `tmp/prosimos-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosimos-1.2.5.tar", max compression
+gzip compressed data, was "prosimos-1.2.6.tar", max compression
```

## Comparing `prosimos-1.2.5.tar` & `prosimos-1.2.6.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0    15059 2023-06-14 13:10:19.975922 prosimos-1.2.5/README.md
--rw-r--r--   0        0        0        0 2023-06-14 13:10:19.995922 prosimos-1.2.5/bpdfr_discovery/__init__.py
--rw-r--r--   0        0        0     3478 2023-06-14 13:10:19.995922 prosimos-1.2.5/bpdfr_discovery/emd_metric.py
--rw-r--r--   0        0        0      489 2023-06-14 13:10:19.995922 prosimos-1.2.5/bpdfr_discovery/exceptions.py
--rw-r--r--   0        0        0     7248 2023-06-14 13:10:19.995922 prosimos-1.2.5/bpdfr_discovery/inter_arrival_cases_discovery.py
--rw-r--r--   0        0        0     5615 2023-06-14 13:10:19.995922 prosimos-1.2.5/bpdfr_discovery/log_comparison_metrics.py
--rw-r--r--   0        0        0    44084 2023-06-14 13:10:19.995922 prosimos-1.2.5/bpdfr_discovery/log_parser.py
--rw-r--r--   0        0        0        0 2023-06-14 13:10:19.995922 prosimos-1.2.5/cli/__init__.py
--rw-r--r--   0        0        0     3539 2023-06-14 13:10:19.995922 prosimos-1.2.5/cli/diff_res_bpsim.py
--rw-r--r--   0        0        0        0 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/__init__.py
--rw-r--r--   0        0        0    44577 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/batch_processing.py
--rw-r--r--   0        0        0     4383 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/batch_processing_parser.py
--rw-r--r--   0        0        0     2626 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/case_attributes.py
--rw-r--r--   0        0        0    48440 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/control_flow_manager.py
--rw-r--r--   0        0        0      487 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/exceptions.py
--rw-r--r--   0        0        0     7340 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/execution_info.py
--rw-r--r--   0        0        0     1109 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/file_manager.py
--rw-r--r--   0        0        0     3147 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/prioritisation.py
--rw-r--r--   0        0        0     1345 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/prioritisation_parser.py
--rw-r--r--   0        0        0     3009 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/prioritisation_rules.py
--rw-r--r--   0        0        0     8585 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/probability_distributions.py
--rw-r--r--   0        0        0      467 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/resource_profile.py
--rw-r--r--   0        0        0    29275 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/simulation_engine.py
--rw-r--r--   0        0        0    22072 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/simulation_properties_parser.py
--rw-r--r--   0        0        0     6298 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/simulation_queues_ds.py
--rw-r--r--   0        0        0     6005 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/simulation_setup.py
--rw-r--r--   0        0        0    15565 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/simulation_stats.py
--rw-r--r--   0        0        0    14171 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/simulation_stats_calculator.py
--rw-r--r--   0        0        0     1730 2023-06-14 13:10:20.111923 prosimos-1.2.5/prosimos/weekday_helper.py
--rw-r--r--   0        0        0      637 2023-06-14 13:10:20.111923 prosimos-1.2.5/pyproject.toml
--rw-r--r--   0        0        0    15765 1970-01-01 00:00:00.000000 prosimos-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0    15559 2023-06-15 18:05:44.750312 prosimos-1.2.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-15 18:05:44.766312 prosimos-1.2.6/bpdfr_discovery/__init__.py
+-rw-r--r--   0        0        0     3478 2023-06-15 18:05:44.766312 prosimos-1.2.6/bpdfr_discovery/emd_metric.py
+-rw-r--r--   0        0        0      489 2023-06-15 18:05:44.766312 prosimos-1.2.6/bpdfr_discovery/exceptions.py
+-rw-r--r--   0        0        0     7248 2023-06-15 18:05:44.766312 prosimos-1.2.6/bpdfr_discovery/inter_arrival_cases_discovery.py
+-rw-r--r--   0        0        0     5615 2023-06-15 18:05:44.766312 prosimos-1.2.6/bpdfr_discovery/log_comparison_metrics.py
+-rw-r--r--   0        0        0    44127 2023-06-15 18:05:44.766312 prosimos-1.2.6/bpdfr_discovery/log_parser.py
+-rw-r--r--   0        0        0        0 2023-06-15 18:05:44.766312 prosimos-1.2.6/cli/__init__.py
+-rw-r--r--   0        0        0     3539 2023-06-15 18:05:44.766312 prosimos-1.2.6/cli/diff_res_bpsim.py
+-rw-r--r--   0        0        0        0 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/__init__.py
+-rw-r--r--   0        0        0    44604 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/batch_processing.py
+-rw-r--r--   0        0        0     4401 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/batch_processing_parser.py
+-rw-r--r--   0        0        0     2409 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/case_attributes.py
+-rw-r--r--   0        0        0    48417 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/control_flow_manager.py
+-rw-r--r--   0        0        0      623 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/exceptions.py
+-rw-r--r--   0        0        0     7340 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/execution_info.py
+-rw-r--r--   0        0        0     1109 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/file_manager.py
+-rw-r--r--   0        0        0      555 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/histogram_distribution.py
+-rw-r--r--   0        0        0     3147 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/prioritisation.py
+-rw-r--r--   0        0        0     1345 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/prioritisation_parser.py
+-rw-r--r--   0        0        0     3009 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/prioritisation_rules.py
+-rw-r--r--   0        0        0     6974 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/probability_distributions.py
+-rw-r--r--   0        0        0      467 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/resource_profile.py
+-rw-r--r--   0        0        0    29277 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/simulation_engine.py
+-rw-r--r--   0        0        0    21739 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/simulation_properties_parser.py
+-rw-r--r--   0        0        0     6298 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/simulation_queues_ds.py
+-rw-r--r--   0        0        0     6584 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/simulation_setup.py
+-rw-r--r--   0        0        0    15565 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/simulation_stats.py
+-rw-r--r--   0        0        0    14171 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/simulation_stats_calculator.py
+-rw-r--r--   0        0        0     1730 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/weekday_helper.py
+-rw-r--r--   0        0        0      668 2023-06-15 18:05:44.870312 prosimos-1.2.6/pyproject.toml
+-rw-r--r--   0        0        0    16305 1970-01-01 00:00:00.000000 prosimos-1.2.6/PKG-INFO
```

### Comparing `prosimos-1.2.5/README.md` & `prosimos-1.2.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -334,8 +334,20 @@
 Then check the information printed in the terminal. 
 
 ## Running tests and receive a coverage report 
 
 ```
 pytest --cov-config=.coveragerc --cov --cov-report=html --cov-branch
 ```
-* If one wants to skip running the tests and just overview a coverage report, one needs to unzip **htmlcov.zip** archive. Unpacked folder **htmlcov** contains HTML coverage report, in general and per each file. 
+* If one wants to skip running the tests and just overview a coverage report, one needs to unzip **htmlcov.zip** archive. Unpacked folder **htmlcov** contains HTML coverage report, in general and per each file.
+
+<details><summary>Development notes</summary>
+
+#### Use local version of `pix-framework`
+
+In case you want to introduce and test changes both to `pix-framework` and `Prosimos`, we need to install local version of `pix-framework` instead of the PyPI released version. For this, the following command needs to be run:
+
+```
+poetry add --editable <relative-path> 
+```
+, where `<relative-path>` should be changed with the path to the root folder of `pix-framework` (e.g., ...`/pix-framework`).
+</details>
```

### Comparing `prosimos-1.2.5/bpdfr_discovery/emd_metric.py` & `prosimos-1.2.6/bpdfr_discovery/emd_metric.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.5/bpdfr_discovery/inter_arrival_cases_discovery.py` & `prosimos-1.2.6/bpdfr_discovery/inter_arrival_cases_discovery.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.5/bpdfr_discovery/log_comparison_metrics.py` & `prosimos-1.2.6/bpdfr_discovery/log_comparison_metrics.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.5/bpdfr_discovery/log_parser.py` & `prosimos-1.2.6/bpdfr_discovery/log_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -809,14 +809,15 @@
             arrival[i].to_start_dist - arrival[i - 1].to_start_dist if arrival[i].in_same_interval(arrival[i - 1])
             else arrival[i].to_start_dist + arrival[i - 1].to_end_dist)
     if print_info:
         print("In Calendar Event Ratio: %.2f" % (len(arrival) / len(initial_events)))
         print('---------------------------------------------------')
     # If we want to use the observed arrival times instead of fitting them to a distribution
     if use_observed_arrival_times:
+        # TODO: use pix_framework for this
         # The arrival distribution is "histogram_sampling" so we compute the CDF and BINs of the observations histogram
         num_bins = 20
         filtered_durations = _reject_outliers(durations)
         bins = np.linspace(min(filtered_durations), max(filtered_durations), num_bins + 1)
         hist, _ = np.histogram(filtered_durations, bins=bins)
         cdf = np.cumsum(hist)
         cdf = cdf / cdf[-1]
```

### Comparing `prosimos-1.2.5/cli/diff_res_bpsim.py` & `prosimos-1.2.6/cli/diff_res_bpsim.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.5/prosimos/batch_processing.py` & `prosimos-1.2.6/prosimos/batch_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from datetime import date, datetime, time, timedelta
 from enum import Enum
 from random import choices
 from typing import List
 
 from pix_framework.calendar.resource_calendar import str_week_days
 
-from prosimos.exceptions import InvalidRuleDefinition
+from prosimos.exceptions import InvalidRuleDefinitionException
 from prosimos.weekday_helper import CustomDatetimeAndSeconds, get_nearest_abs_day, get_nearest_past_day
 
 
 def _get_operator_symbols(operator_str: str, eq_operator: operator):
     OPERATOR_SYMBOLS = {
         '<': operator.lt,
         '<=': operator.le,
@@ -401,17 +401,17 @@
         for rule in self.rules:
             if rule.variable1 == RULE_TYPE.WEEK_DAY.value:
                 week_day_count += 1
             elif rule.variable1 == RULE_TYPE.DAILY_HOUR.value:
                 daily_hour_count += 1
 
         if week_day_count > 1:
-            raise InvalidRuleDefinition("Only one WEEK_DAY subrule is allowed inside AND rule.")
+            raise InvalidRuleDefinitionException("Only one WEEK_DAY subrule is allowed inside AND rule.")
         elif daily_hour_count > 2:
-            raise InvalidRuleDefinition("Only one or two subrules of DAILY_HOUR type is allowed inside AND rule.")
+            raise InvalidRuleDefinitionException("Only one or two subrules of DAILY_HOUR type is allowed inside AND rule.")
 
 
     def _get_low_and_high_boundaries(self, rule_name: RULE_TYPE, diff_units):
         if isinstance(diff_units, timedelta):
             low_boundary, high_boundary = self.daily_hour_range
         else:
             low_boundary, high_boundary = (None, None)
```

### Comparing `prosimos-1.2.5/prosimos/batch_processing_parser.py` & `prosimos-1.2.6/prosimos/batch_processing_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     BATCH_TYPE,
     RULE_TYPE,
     AndFiringRule,
     BatchConfigPerTask,
     FiringSubRule,
     OrFiringRule,
 )
-from prosimos.exceptions import InvalidRuleDefinition
+from prosimos.exceptions import InvalidRuleDefinitionException
 
 
 class BatchProcessingParser:
     def __init__(self, json_data_with_batch_info):
         self.data = json_data_with_batch_info
 
     def parse(self):
@@ -98,15 +98,15 @@
             formatted_value = int(value)
         else:
             # all others should have the number as the value
             formatted_value = float(value)
 
         if attribute == RULE_TYPE.WEEK_DAY.value and comparison != "=":
             # only "=" operator is allowed to be used with the week_day type of rule
-            raise InvalidRuleDefinition(
+            raise InvalidRuleDefinitionException(
                 f"'{comparison}' is not allowed operator for the week_day type of rule."
             )
 
         return FiringSubRule(attribute, comparison, formatted_value)
 
     @staticmethod
     def _move_size_to_end(list: List[FiringSubRule]):
```

### Comparing `prosimos-1.2.5/prosimos/case_attributes.py` & `prosimos-1.2.6/prosimos/case_attributes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from enum import Enum
 from functools import reduce
+from random import choices
 from typing import List
+
+from pix_framework.statistics.distribution import DurationDistribution
+
 from prosimos.exceptions import InvalidCaseAttributeException
-from prosimos.probability_distributions import generate_number_from
-from random import choices
+
 
 class CASE_ATTR_TYPE(Enum):
     DISCRETE = "discrete"
     CONTINUOUS = "continuous"
 
 def parse_discrete_value(value_info_arr):
     prob_arr = []
@@ -17,23 +20,16 @@
         prob_arr.append(float(item["value"]))
 
     return {
         "options": options_arr,
         "probabilities": prob_arr
     }
 
-def parse_continuous_value(value_info):
-    dist_params = []
-    for param_info in value_info["distribution_params"]:
-        dist_params.append(float(param_info["value"]))
-    
-    return {
-        "distribution_name": value_info["distribution_name"],
-        "distribution_params": dist_params
-    }
+def parse_continuous_value(value_info) -> "DurationDistribution":
+    return DurationDistribution.from_dict(value_info)
 
 
 class CaseAttribute():
     def __init__(self, name, case_atrr_type, value):
         self.name: str = name
         self.case_atrr_type: CASE_ATTR_TYPE = CASE_ATTR_TYPE(case_atrr_type)
 
@@ -47,15 +43,15 @@
         self.validate()
 
     def get_next_value(self):
         if self.case_atrr_type == CASE_ATTR_TYPE.DISCRETE:
             one_choice_arr = choices(self.value["options"], self.value["probabilities"])
             return one_choice_arr[0]
         else:
-            return generate_number_from(self.value["distribution_name"], self.value["distribution_params"])
+            return self.value.generate_one_value_with_boundaries()
 
     def validate(self):
         if self.case_atrr_type == CASE_ATTR_TYPE.DISCRETE:
             actual_sum_probabilities = reduce(lambda acc, item: acc + item, self.value["probabilities"], 0) 
             
             if actual_sum_probabilities != 1:
                 raise InvalidCaseAttributeException(f"Case attribute ${self.name}: probabilities' sum should be equal to 1")
```

### Comparing `prosimos-1.2.5/prosimos/control_flow_manager.py` & `prosimos-1.2.6/prosimos/control_flow_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import copy
+import random
+import secrets
 import sys
 from collections import deque
 from enum import Enum
 from typing import List
 
-import random
-import secrets
-from prosimos.batch_processing import BATCH_TYPE, AndFiringRule, BatchConfigPerTask
-from prosimos.probability_distributions import generate_number_from
+from pix_framework.statistics.distribution import DurationDistribution
 
+from prosimos.batch_processing import (BATCH_TYPE, AndFiringRule,
+                                       BatchConfigPerTask)
 from prosimos.exceptions import InvalidBpmnModelException
 from prosimos.weekday_helper import CustomDatetimeAndSeconds
 
 seconds_per_unit = {"s": 1, "m": 60, "h": 3600, "d": 86400, "w": 604800}
 
 class BatchInfoForExecution:
     def __init__(self, all_case_ids, task_batch_info, curr_task_id, batch_spec, start_time_from_rule):
@@ -459,15 +460,16 @@
         :param gateway_element_info: object of type ElementInfo which is gateway
         :param completed_datetime_prev_event: datetime of the previously finished event
         :return: flow name that will be executed
         """
         all_gateway_choices = dict()
         for outgoing_flow in gateway_element_info.outgoing_flows:
             event_id = self.flow_arcs[outgoing_flow][1]
-            all_gateway_choices[outgoing_flow] = self.event_duration(event_id)
+            [duration] = self.event_duration(event_id)
+            all_gateway_choices[outgoing_flow] = duration
         
         min_value = min(all_gateway_choices.values())
         res = [(key, value) for key, value in all_gateway_choices.items() if value == min_value]
 
         # return randomly selected outgoing flow
         # in case of same value for multiple flows
         return secrets.choice(res)
@@ -476,19 +478,16 @@
     def event_duration(self, event_id):
         """
         Find event duration of all types except TIMER
 
         :event_id: id of the event element
         :return: duration in seconds 
         """
-        distribution = self.event_distribution[event_id]
-        val = generate_number_from(distribution["distribution_name"],
-                                   distribution["distribution_params"]
-        )
-        return val
+        distribution: DurationDistribution = self.event_distribution[event_id]
+        return distribution.generate_sample(1)
 
 
     def reply_trace(self, task_sequence, f_arcs_frequency, post_p=True, trace=None):
         self._c_trace = trace
         task_enabling = list()
         p_state = ProcessState(self)
         fired_tasks = list()
```

### Comparing `prosimos-1.2.5/prosimos/execution_info.py` & `prosimos-1.2.6/prosimos/execution_info.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.5/prosimos/file_manager.py` & `prosimos-1.2.6/prosimos/file_manager.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.5/prosimos/prioritisation.py` & `prosimos-1.2.6/prosimos/prioritisation.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.5/prosimos/prioritisation_parser.py` & `prosimos-1.2.6/prosimos/prioritisation_parser.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.5/prosimos/prioritisation_rules.py` & `prosimos-1.2.6/prosimos/prioritisation_rules.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.5/prosimos/probability_distributions.py` & `prosimos-1.2.6/prosimos/probability_distributions.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import math
 import statistics
 import sys
 import warnings
 
 import numpy as np
-import numpy.random
 import scipy.stats as st
 from numpy import random
 from scipy.stats import wasserstein_distance
 
 
+# NOTE: default distribution becoming obsolete due to no support with pix_framework
 def create_default_distribution(min_value, max_value):
     return {"distribution_name": "default", "distribution_params": [min_value, max_value]}
 
 
+# TODO: consider using get_best_fitting_distribution from pix_framework
 # Create models from data
 def best_fit_distribution(data, bins=50):
     fix_value = check_fix(data)
     if fix_value is not None:
         return {"distribution_name": "fix", "distribution_params": [fix_value]}
 
     """Model data by finding best fit distribution to data"""
@@ -107,63 +108,14 @@
             if abs(d1 - d2) < delta:
                 count += 1
         if count / len(data_list) > 0.9:
             return d1
     return None
 
 
-def generate_number_from(distribution_name, params):
-    while True:
-        duration = evaluate_distribution_function(distribution_name, params)
-        if duration >= 0:
-            return duration
-
-
-def evaluate_distribution_function(distribution_name, params):
-    if distribution_name == "fix":
-        return params[0]
-    elif distribution_name == 'default':
-        return numpy.random.uniform(params[0], params[1])
-    elif distribution_name == "histogram_sampling":
-        value = np.random.rand(1)[0]
-        value_bin = np.searchsorted(params['cdf'], value)
-        return params['bin_midpoints'][value_bin]
-
-    arg = params[:-4]
-    loc = params[-4]
-    scale = params[-3]
-    d_min = params[-2]
-    d_max = params[-1]
-
-    dist = getattr(st, distribution_name)
-    num_param = len(arg)
-
-    f_dist = 0
-    while True:
-        if num_param == 0:
-            f_dist = dist.rvs(loc=loc, scale=scale, size=1)[0]
-        elif num_param == 1:
-            f_dist = dist.rvs(arg[0], loc=loc, scale=scale, size=1)[0]
-        elif num_param == 2:
-            f_dist = dist.rvs(arg[0], arg[1], loc=loc, scale=scale, size=1)[0]
-        elif num_param == 3:
-            f_dist = dist.rvs(arg[0], arg[1], arg[2], loc=loc, scale=scale, size=1)[0]
-        elif num_param == 4:
-            f_dist = dist.rvs(arg[0], arg[1], arg[2], arg[3], loc=loc, scale=scale, size=1)[0]
-        elif num_param == 5:
-            f_dist = dist.rvs(arg[0], arg[1], arg[2], arg[3], arg[4], loc=loc, scale=scale, size=1)[0]
-        elif num_param == 6:
-            f_dist = dist.rvs(arg[0], arg[1], arg[2], arg[3], arg[4], arg[5], loc=loc, scale=scale, size=1)[0]
-        elif num_param == 7:
-            f_dist = dist.rvs(arg[0], arg[1], arg[2], arg[3], arg[4], arg[5], arg[6], loc=loc, scale=scale, size=1)[0]
-        if d_min <= f_dist <= d_max:
-            break
-    return f_dist
-
-
 class Choice:
     def __init__(self, candidates_list, probability_list):
         self.candidates_list = candidates_list
         self.probability_list = probability_list
 
     def get_outgoing_flow(self):
         return random.choice(self.candidates_list, 1, p=self.probability_list)[0]
@@ -173,54 +125,55 @@
         for i in range(0, len(self.candidates_list)):
             if random.choice([True, False], 1, p=[self.probability_list[i], 1 - self.probability_list[i]]):
                 selected.append((self.candidates_list[i], None))
         return selected if len(selected) > 0 else [(self.get_outgoing_flow(), None)]
 
 
 def random_uniform(start, end):
-    return numpy.random.uniform(low=start, high=end)
+    return random.uniform(low=start, high=end)
 
 
-def best_fit_distribution_1(data):
-    fix_value = check_fix(data)
-    if fix_value is not None:
-        return {"distribution_name": "fix", "distribution_params": [check_fix(data)]}
-
-    mean = statistics.mean(data)
-    variance = statistics.variance(data)
-    st_dev = statistics.pstdev(data)
-    d_min = min(data)
-    d_max = max(data)
-
-    dist_candidates = [
-        {"distribution_name": "expon", "distribution_params": [0, mean, d_min, d_max]},
-        {"distribution_name": "norm", "distribution_params": [mean, st_dev, d_min, d_max]},
-        {"distribution_name": "uniform", "distribution_params": [d_min, d_max - d_min, d_min, d_max]},
-        {"distribution_name": "default", "distribution_params": [d_min, d_max]}
-    ]
-
-    if mean != 0:
-        mean_2 = mean ** 2
-        phi = math.sqrt(variance + mean_2)
-        mu = math.log(mean_2 / phi)
-        sigma = math.sqrt(math.log(phi ** 2 / mean_2))
-
-        dist_candidates.append({"distribution_name": "lognorm",
-                                "distribution_params": [sigma, 0, math.exp(mu), d_min, d_max]}, )
-
-    if mean != 0 and variance != 0:
-        dist_candidates.append({"distribution_name": "gamma",
-                                "distribution_params": [pow(mean, 2) / variance, 0, variance / mean, d_min, d_max]}, )
-
-    best_dist = None
-    best_emd = sys.float_info.max
-    for dist_c in dist_candidates:
-        ev_list = list()
-        for i in range(0, len(data)):
-            ev_list.append(evaluate_distribution_function(dist_c["distribution_name"], dist_c["distribution_params"]))
-
-        emd = wasserstein_distance(data, ev_list)
-        if emd < best_emd:
-            best_emd = emd
-            best_dist = dist_c
+# TODO: consider for removal, not being used anywhere
+# def best_fit_distribution_1(data):
+#     fix_value = check_fix(data)
+#     if fix_value is not None:
+#         return {"distribution_name": "fix", "distribution_params": [check_fix(data)]}
+
+#     mean = statistics.mean(data)
+#     variance = statistics.variance(data)
+#     st_dev = statistics.pstdev(data)
+#     d_min = min(data)
+#     d_max = max(data)
+
+#     dist_candidates = [
+#         {"distribution_name": "expon", "distribution_params": [0, mean, d_min, d_max]},
+#         {"distribution_name": "norm", "distribution_params": [mean, st_dev, d_min, d_max]},
+#         {"distribution_name": "uniform", "distribution_params": [d_min, d_max - d_min, d_min, d_max]},
+#         {"distribution_name": "default", "distribution_params": [d_min, d_max]}
+#     ]
+
+#     if mean != 0:
+#         mean_2 = mean ** 2
+#         phi = math.sqrt(variance + mean_2)
+#         mu = math.log(mean_2 / phi)
+#         sigma = math.sqrt(math.log(phi ** 2 / mean_2))
+
+#         dist_candidates.append({"distribution_name": "lognorm",
+#                                 "distribution_params": [sigma, 0, math.exp(mu), d_min, d_max]}, )
+
+#     if mean != 0 and variance != 0:
+#         dist_candidates.append({"distribution_name": "gamma",
+#                                 "distribution_params": [pow(mean, 2) / variance, 0, variance / mean, d_min, d_max]}, )
+
+#     best_dist = None
+#     best_emd = sys.float_info.max
+#     for dist_c in dist_candidates:
+#         ev_list = list()
+#         for i in range(0, len(data)):
+#             ev_list.append(evaluate_distribution_function(dist_c["distribution_name"], dist_c["distribution_params"]))
+
+#         emd = wasserstein_distance(data, ev_list)
+#         if emd < best_emd:
+#             best_emd = emd
+#             best_dist = dist_c
 
-    return best_dist
+#     return best_dist
```

### Comparing `prosimos-1.2.5/prosimos/simulation_engine.py` & `prosimos-1.2.6/prosimos/simulation_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -527,15 +527,15 @@
 
         return completed_at, completed_datetime
 
     def execute_event(self, c_event):
         # Handle event types separately (they don't need assigned resource)
         event_duration_seconds = None
         event_element = self.sim_setup.bpmn_graph.element_info[c_event.task_id]
-        event_duration_seconds = self.sim_setup.bpmn_graph.event_duration(
+        [event_duration_seconds] = self.sim_setup.bpmn_graph.event_duration(
             event_element.id
         )
 
         completed_at = c_event.enabled_at + event_duration_seconds
         completed_datetime = c_event.enabled_datetime + timedelta(
             seconds=event_duration_seconds
         )
```

### Comparing `prosimos-1.2.5/prosimos/simulation_properties_parser.py` & `prosimos-1.2.6/prosimos/simulation_properties_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import json
 import xml.etree.ElementTree as ET
 
 from numpy import exp, log, sqrt
 from pix_framework.calendar.resource_calendar import RCalendar
+from pix_framework.statistics.distribution import DurationDistribution
 
 from prosimos.batch_processing_parser import BatchProcessingParser
 from prosimos.case_attributes import AllCaseAttributes, CaseAttribute
-from prosimos.control_flow_manager import (
-    BPMN,
-    EVENT_TYPE,
-    BPMNGraph,
-    ElementInfo,
-)
+from prosimos.control_flow_manager import (BPMN, EVENT_TYPE, BPMNGraph,
+                                           ElementInfo)
+from prosimos.histogram_distribution import HistogramDistribution
 from prosimos.prioritisation import AllPriorityRules
 from prosimos.prioritisation_parser import PrioritisationParser
-from prosimos.probability_distributions import *
+from prosimos.probability_distributions import Choice
 from prosimos.resource_profile import PoolInfo, ResourceProfile
 
 bpmn_schema_url = "http://www.omg.org/spec/BPMN/20100524/MODEL"
 simod_ns = {"qbp": "http://www.qbp-simulator.com/Schema201212"}
 bpmn_element_ns = {"xmlns": bpmn_schema_url}
 
 EVENT_DISTRIBUTION_SECTION = "event_distribution"
@@ -140,45 +138,30 @@
 def parse_task_resource_distributions(json_data, res_pool):
     task_resource_distribution = dict()
     for perf_info in json_data:
         t_id = perf_info["task_id"]
         if t_id not in task_resource_distribution:
             task_resource_distribution[t_id] = dict()
         for r_info in perf_info["resources"]:
-            dist_params = []
-            for param_info in r_info["distribution_params"]:
-                dist_params.append(float(param_info["value"]))
             for r_id in res_pool[r_info["resource_id"]]:
-                task_resource_distribution[t_id][r_id] = {
-                    "distribution_name": r_info["distribution_name"],
-                    "distribution_params": dist_params,
-                }
-    return task_resource_distribution
+                task_resource_distribution[t_id][r_id] = DurationDistribution.from_dict(r_info)
 
+    return task_resource_distribution
 
 def parse_event_distribution(event_json_data):
     """
     Parse "event_distribution" section of json data
     """
     event_distibution = dict()
 
     for event_info in event_json_data:
         e_id = event_info["event_id"]
 
         if e_id not in event_distibution:
-            event_distibution[e_id] = dict()
-            dist_params = []
-
-            for param_info in event_info["distribution_params"]:
-                dist_params.append(float(param_info["value"]))
-
-            event_distibution[e_id] = {
-                "distribution_name": event_info["distribution_name"],
-                "distribution_params": dist_params,
-            }
+            event_distibution[e_id] = DurationDistribution.from_dict(event_info)
 
     return event_distibution
 
 
 def parse_case_attr(json_data) -> AllCaseAttributes:
     case_attributes = []
     for curr_case_attr in json_data:
@@ -203,28 +186,26 @@
 #         calendars_map[r_calendar.calendar_id] = r_calendar
 #     return resources_map, calendars_map
 
 
 def parse_arrival_branching_probabilities(arrival_json, gateway_json):
     element_distribution = dict()
 
-    dist_params = []
-    if arrival_json["distribution_name"] == "histogram_sampling":
+    dist_name = arrival_json["distribution_name"] 
+    if dist_name == "histogram_sampling":
         # Custom distribution: we expect a list of inter-arrival interval values (floats),
         # prosimos will take randomly a value from this list each time it needs a new
         # observation, so the output will follow (if the sample is big enough) the same
         # "unknown distribution" than the specified data.
-        dist_params = arrival_json["histogram_data"]
+        element_distribution["arrivalTime"] = HistogramDistribution.from_dict(arrival_json)
     else:
-        for param_info in arrival_json["distribution_params"]:
-            dist_params.append(float(param_info["value"]))
-    element_distribution["arrivalTime"] = {
-        "distribution_name": arrival_json["distribution_name"],
-        "distribution_params": dist_params,
-    }
+        # handling all other types apart from "histogram_sampling"
+        # since end-user provides user-friendly parameters,
+        # we transform them to ones suitable for being used with Scipy library
+        element_distribution["arrivalTime"] = DurationDistribution.from_dict(arrival_json)
 
     for g_info in gateway_json:
         g_id = g_info["gateway_id"]
         probability_list = list()
         out_arc = list()
         for prob_info in g_info["probabilities"]:
             out_arc.append(prob_info["path_id"])
@@ -485,14 +466,19 @@
         "gateway_branching_probabilities": gateways_branching,
         "task_resource_distribution": task_resource_dist,
         "resource_calendars": resource_calendars,
     }
     with open(out_file, "w") as file_writter:
         json.dump(to_save, file_writter)
 
+def format_date(date_str):
+    date_splt = date_str.split("+")
+    if len(date_splt) == 2 and date_splt[1] == "00:00":
+        return date_splt[0]
+    return date_str
 
 def extract_dist_params(dist_info):
     # time_unit = dist_info.find("qbp:timeUnit", simod_ns).text
     # The time_tables produced by bimp always have the parameters in seconds, although it shouws other time units in
     # the XML file.
     dist_params = {
         "mean": float(dist_info.attrib["mean"]),
@@ -519,15 +505,15 @@
         }
     if dist_name == "UNIFORM":
         # input: loc = from, scale = to - from
         return {
             "distribution_name": "uniform",
             "distribution_params": [
                 dist_params["arg1"],
-                dist_params["arg2"] - dist_params["arg2"],
+                dist_params["arg2"] - dist_params["arg1"],
             ],
         }
     if dist_name == "GAMMA":
         # input: shape, loc=0, scale
         mean, variance = dist_params["mean"], dist_params["arg1"]
         return {
             "distribution_name": "gamma",
@@ -552,14 +538,7 @@
 
         # input: s = sigma = standard deviation, loc = 0, scale = exp(mu)
         return {
             "distribution_name": "lognorm",
             "distribution_params": [sigma, 0, exp(mu)],
         }
     return None
-
-
-def format_date(date_str):
-    date_splt = date_str.split("+")
-    if len(date_splt) == 2 and date_splt[1] == "00:00":
-        return date_splt[0]
-    return date_str
```

### Comparing `prosimos-1.2.5/prosimos/simulation_queues_ds.py` & `prosimos-1.2.6/prosimos/simulation_queues_ds.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.5/prosimos/simulation_setup.py` & `prosimos-1.2.6/prosimos/simulation_setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import datetime
 import ntpath
 from datetime import timedelta
 from typing import Optional
 
 import pytz
 from pix_framework.calendar.resource_calendar import RCalendar
+from pix_framework.statistics.distribution import DurationDistribution
 
 from prosimos.batch_processing import BatchConfigPerTask
-from prosimos.control_flow_manager import ProcessState, ElementInfo, BPMN
-from prosimos.probability_distributions import generate_number_from
-from prosimos.simulation_properties_parser import parse_simulation_model, parse_json_sim_parameters
+from prosimos.control_flow_manager import BPMN, ElementInfo, ProcessState
+from prosimos.exceptions import InvalidSimScenarioException
+from prosimos.histogram_distribution import HistogramDistribution
+from prosimos.simulation_properties_parser import (parse_json_sim_parameters,
+                                                   parse_simulation_model)
 
 
 class SimDiffSetup:
     def __init__(self, bpmn_path, json_path, is_event_added_to_log, total_cases):
         self.process_name = ntpath.basename(bpmn_path).split(".")[0]
         self.start_datetime = datetime.datetime.now(pytz.utc)
 
@@ -49,17 +52,25 @@
 
     def next_resting_time(self, resource_id, starting_from):
         if resource_id in self.resources_map:
             return self.calendars_map[self.resources_map[resource_id].calendar_id].next_available_time(starting_from)
         return 0
 
     def next_arrival_time(self, starting_from):
-        val = generate_number_from(self.element_probability['arrivalTime']['distribution_name'],
-                                   self.element_probability['arrivalTime']['distribution_params'])
-        return val + self.arrival_calendar.next_available_time(starting_from + timedelta(seconds=val))
+        duration: float = 0.0
+        
+        # decide how to calculate value based on whether it is function distribution or histogram one
+        if isinstance(self.element_probability['arrivalTime'], DurationDistribution):
+            [duration] = self.element_probability['arrivalTime'].generate_sample(1)
+        elif isinstance(self.element_probability['arrivalTime'], HistogramDistribution):
+            duration = self.element_probability['arrivalTime'].generate_value()
+        else:
+            raise InvalidSimScenarioException("Not supported arrival distribution")
+
+        return duration + self.arrival_calendar.next_available_time(starting_from + timedelta(seconds=duration))
 
     def initial_state(self):
         return ProcessState(self.bpmn_graph)
 
     def is_enabled(self, e_id, p_state):
         return self.bpmn_graph.is_enabled(e_id, p_state)
 
@@ -85,27 +96,27 @@
                 if r_id in starter_resources:
                     continue
                 arrival_calendar.combine_calendar(self.calendars_map[self.resources_map[r_id].calendar_id])
                 starter_resources.add(r_id)
         return arrival_calendar
 
     def ideal_task_duration(self, task_id, resource_id, num_tasks_in_batch):
-        val = generate_number_from(self.task_resource[task_id][resource_id]['distribution_name'],
-                                   self.task_resource[task_id][resource_id]['distribution_params'])
-
+        # calculate duration based on defined distribution for the resource allocation
+        [duration] = self.task_resource[task_id][resource_id].generate_sample(1)
+                        
         if num_tasks_in_batch == 0:
             # task executed NOT in batch
-            return val
+            return duration
         else:
             # task executed as a part of the batch
             curr_batch_info: Optional[BatchConfigPerTask] = self.batch_processing.get(task_id, None)
             if curr_batch_info == None:
                 print(f"WARNING: Could not find info about batch_processing for task {task_id}")
 
-            return curr_batch_info.calculate_ideal_duration(val, num_tasks_in_batch)
+            return curr_batch_info.calculate_ideal_duration(duration, num_tasks_in_batch)
 
     def real_task_duration(self, task_duration, resource_id, enabled_at):
         return self.calendars_map[self.resources_map[resource_id].calendar_id].find_idle_time(enabled_at, task_duration)
 
     def set_starting_datetime(self, new_datetime):
         (
             is_inside_arrival_calendar,
```

### Comparing `prosimos-1.2.5/prosimos/simulation_stats.py` & `prosimos-1.2.6/prosimos/simulation_stats.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.5/prosimos/simulation_stats_calculator.py` & `prosimos-1.2.6/prosimos/simulation_stats_calculator.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.5/prosimos/weekday_helper.py` & `prosimos-1.2.6/prosimos/weekday_helper.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.5/pyproject.toml` & `prosimos-1.2.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prosimos"
-version = "1.2.5"
+version = "1.2.6"
 description = ""
 authors = ["Iryna Halenok, Orlenys López Pintado"]
 readme = "README.md"
 packages = [
     {include = "cli"},
     {include = "prosimos"},
     {include = "bpdfr_discovery"}
@@ -16,17 +16,18 @@
 numpy = "^1.24.3"
 pandas = "^2.0.1"
 python-dateutil = "^2.8.2"
 pytz = "^2023.3"
 scipy = "^1.10.1"
 pm4py = "^2.7.4"
 pix-framework = "^0.9.0"
+pylint = "^2.17.4"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 
 [tool.poetry.scripts]
 prosimos = "cli.diff_res_bpsim:cli"
 
 [build-system]
-requires = ["poetry>=1.0"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `prosimos-1.2.5/PKG-INFO` & `prosimos-1.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: prosimos
-Version: 1.2.5
+Version: 1.2.6
 Summary: 
 Author: Iryna Halenok, Orlenys López Pintado
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pix-framework (>=0.9.0,<0.10.0)
 Requires-Dist: pm4py (>=2.7.4,<3.0.0)
+Requires-Dist: pylint (>=2.17.4,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: pytz (>=2023.3,<2024.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Prosimos
 
@@ -354,9 +355,21 @@
 Then check the information printed in the terminal. 
 
 ## Running tests and receive a coverage report 
 
 ```
 pytest --cov-config=.coveragerc --cov --cov-report=html --cov-branch
 ```
-* If one wants to skip running the tests and just overview a coverage report, one needs to unzip **htmlcov.zip** archive. Unpacked folder **htmlcov** contains HTML coverage report, in general and per each file. 
+* If one wants to skip running the tests and just overview a coverage report, one needs to unzip **htmlcov.zip** archive. Unpacked folder **htmlcov** contains HTML coverage report, in general and per each file.
+
+<details><summary>Development notes</summary>
+
+#### Use local version of `pix-framework`
+
+In case you want to introduce and test changes both to `pix-framework` and `Prosimos`, we need to install local version of `pix-framework` instead of the PyPI released version. For this, the following command needs to be run:
+
+```
+poetry add --editable <relative-path> 
+```
+, where `<relative-path>` should be changed with the path to the root folder of `pix-framework` (e.g., ...`/pix-framework`).
+</details>
```

