# Comparing `tmp/modular_rl-0.3.2.tar.gz` & `tmp/modular_rl-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modular_rl-0.3.2.tar", last modified: Thu Jun  8 11:25:20 2023, max compression
+gzip compressed data, was "modular_rl-0.3.3.tar", last modified: Thu Jun 15 14:19:25 2023, max compression
```

## Comparing `modular_rl-0.3.2.tar` & `modular_rl-0.3.3.tar`

### file list

```diff
@@ -1,60 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 11:25:20.557843 modular_rl-0.3.2/
--rw-rw-rw-   0        0        0     1089 2023-05-04 06:13:20.000000 modular_rl-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     5688 2023-06-08 11:25:20.555754 modular_rl-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     4182 2023-06-08 11:09:02.000000 modular_rl-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 11:25:20.478416 modular_rl-0.3.2/modular_rl/
--rw-rw-rw-   0        0        0       37 2023-05-07 14:51:41.000000 modular_rl-0.3.2/modular_rl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 11:25:20.497466 modular_rl-0.3.2/modular_rl/agents/
--rw-rw-rw-   0        0        0      108 2023-06-06 21:28:14.000000 modular_rl-0.3.2/modular_rl/agents/__init__.py
--rw-rw-rw-   0        0        0    10432 2023-06-07 12:17:24.000000 modular_rl-0.3.2/modular_rl/agents/_agent.py
--rw-rw-rw-   0        0        0     4838 2023-06-06 21:35:21.000000 modular_rl-0.3.2/modular_rl/agents/_custom.py
--rw-rw-rw-   0        0        0    11741 2023-06-08 11:22:46.000000 modular_rl-0.3.2/modular_rl/agents/mcis.py
--rw-rw-rw-   0        0        0    12121 2023-06-07 22:13:39.000000 modular_rl-0.3.2/modular_rl/agents/mcts.py
--rw-rw-rw-   0        0        0    20686 2023-06-06 22:24:07.000000 modular_rl-0.3.2/modular_rl/agents/mim.py
--rw-rw-rw-   0        0        0    14958 2023-06-06 21:36:06.000000 modular_rl-0.3.2/modular_rl/agents/ppo.py
-drwxrwxrwx   0        0        0        0 2023-06-08 11:25:20.500609 modular_rl-0.3.2/modular_rl/envs/
--rw-rw-rw-   0        0        0        0 2023-06-04 21:09:01.000000 modular_rl-0.3.2/modular_rl/envs/__init__.py
--rw-rw-rw-   0        0        0      133 2023-06-04 21:09:01.000000 modular_rl-0.3.2/modular_rl/envs/_custom.py
-drwxrwxrwx   0        0        0        0 2023-06-08 11:25:20.505421 modular_rl-0.3.2/modular_rl/envs/mim/
--rw-rw-rw-   0        0        0       25 2023-06-04 21:09:01.000000 modular_rl-0.3.2/modular_rl/envs/mim/__init__.py
--rw-rw-rw-   0        0        0    15402 2023-06-04 21:09:01.000000 modular_rl-0.3.2/modular_rl/envs/mim/card_evaluator.py
--rw-rw-rw-   0        0        0     4474 2023-06-04 21:09:01.000000 modular_rl-0.3.2/modular_rl/envs/mim/mim.py
-drwxrwxrwx   0        0        0        0 2023-06-08 11:25:20.510270 modular_rl-0.3.2/modular_rl/networks/
--rw-rw-rw-   0        0        0       68 2023-05-07 14:51:41.000000 modular_rl-0.3.2/modular_rl/networks/__init__.py
--rw-rw-rw-   0        0        0     2174 2023-05-07 14:51:41.000000 modular_rl-0.3.2/modular_rl/networks/actor_critic.py
--rw-rw-rw-   0        0        0     2878 2023-05-04 23:35:18.000000 modular_rl-0.3.2/modular_rl/networks/policy.py
--rw-rw-rw-   0        0        0     2688 2023-05-04 23:33:52.000000 modular_rl-0.3.2/modular_rl/networks/value.py
-drwxrwxrwx   0        0        0        0 2023-06-08 11:25:20.519638 modular_rl-0.3.2/modular_rl/params/
--rw-rw-rw-   0        0        0       85 2023-06-04 21:09:01.000000 modular_rl-0.3.2/modular_rl/params/__init__.py
--rw-rw-rw-   0        0        0     2161 2023-06-04 21:09:01.000000 modular_rl-0.3.2/modular_rl/params/mcis.py
--rw-rw-rw-   0        0        0     2294 2023-06-08 11:07:34.000000 modular_rl-0.3.2/modular_rl/params/mcts.py
--rw-rw-rw-   0        0        0     1938 2023-06-06 22:34:44.000000 modular_rl-0.3.2/modular_rl/params/mim.py
--rw-rw-rw-   0        0        0     2053 2023-05-07 14:51:41.000000 modular_rl-0.3.2/modular_rl/params/ppo.py
--rw-rw-rw-   0        0        0     1377 2023-06-06 22:36:03.000000 modular_rl-0.3.2/modular_rl/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-08 11:25:20.531473 modular_rl-0.3.2/modular_rl/tester/
--rw-rw-rw-   0        0        0       61 2023-05-07 14:51:41.000000 modular_rl-0.3.2/modular_rl/tester/__init__.py
--rw-rw-rw-   0        0        0     1036 2023-06-07 12:42:45.000000 modular_rl-0.3.2/modular_rl/tester/mcis.py
--rw-rw-rw-   0        0        0     1270 2023-06-07 21:24:00.000000 modular_rl-0.3.2/modular_rl/tester/mcts.py
--rw-rw-rw-   0        0        0      689 2023-06-06 22:45:16.000000 modular_rl-0.3.2/modular_rl/tester/mim.py
--rw-rw-rw-   0        0        0     1552 2023-05-05 00:05:02.000000 modular_rl-0.3.2/modular_rl/tester/ppo.py
-drwxrwxrwx   0        0        0        0 2023-06-08 11:25:20.536152 modular_rl-0.3.2/modular_rl/util/
--rw-rw-rw-   0        0        0        0 2023-05-04 23:35:52.000000 modular_rl-0.3.2/modular_rl/util/__init__.py
--rw-rw-rw-   0        0        0     2533 2023-06-04 21:09:01.000000 modular_rl-0.3.2/modular_rl/util/node.py
-drwxrwxrwx   0        0        0        0 2023-06-08 11:25:20.488046 modular_rl-0.3.2/modular_rl.egg-info/
--rw-rw-rw-   0        0        0     5688 2023-06-08 11:25:20.000000 modular_rl-0.3.2/modular_rl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1220 2023-06-08 11:25:20.000000 modular_rl-0.3.2/modular_rl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 11:25:20.000000 modular_rl-0.3.2/modular_rl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-08 11:25:20.000000 modular_rl-0.3.2/modular_rl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-08 11:25:20.000000 modular_rl-0.3.2/modular_rl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1414 2023-06-08 11:25:03.000000 modular_rl-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-08 11:25:20.557843 modular_rl-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      937 2023-06-08 11:25:15.000000 modular_rl-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 11:25:20.554725 modular_rl-0.3.2/tests/
--rw-rw-rw-   0        0        0       97 2023-06-04 21:09:01.000000 modular_rl-0.3.2/tests/test_mcis.py
--rw-rw-rw-   0        0        0      105 2023-06-04 21:09:01.000000 modular_rl-0.3.2/tests/test_mcis_modular.py
--rw-rw-rw-   0        0        0       97 2023-05-07 14:51:41.000000 modular_rl-0.3.2/tests/test_mcts.py
--rw-rw-rw-   0        0        0      101 2023-06-07 12:43:41.000000 modular_rl-0.3.2/tests/test_mcts_modular.py
--rw-rw-rw-   0        0        0      107 2023-06-04 21:09:01.000000 modular_rl-0.3.2/tests/test_mim.py
--rw-rw-rw-   0        0        0      111 2023-06-06 22:42:10.000000 modular_rl-0.3.2/tests/test_mim_modular.py
--rw-rw-rw-   0        0        0       61 2023-05-05 10:03:21.000000 modular_rl-0.3.2/tests/test_ppo.py
--rw-rw-rw-   0        0        0       69 2023-05-05 10:03:28.000000 modular_rl-0.3.2/tests/test_ppo_modular.py
+drwxrwxrwx   0        0        0        0 2023-06-15 14:19:25.982962 modular_rl-0.3.3/
+-rw-rw-rw-   0        0        0     1089 2023-05-04 06:13:20.000000 modular_rl-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0     5688 2023-06-15 14:19:25.982962 modular_rl-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4182 2023-06-08 11:09:02.000000 modular_rl-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 14:19:25.925107 modular_rl-0.3.3/modular_rl/
+-rw-rw-rw-   0        0        0       37 2023-05-07 14:51:41.000000 modular_rl-0.3.3/modular_rl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 14:19:25.944071 modular_rl-0.3.3/modular_rl/agents/
+-rw-rw-rw-   0        0        0      108 2023-06-06 21:28:14.000000 modular_rl-0.3.3/modular_rl/agents/__init__.py
+-rw-rw-rw-   0        0        0    10939 2023-06-15 13:13:29.000000 modular_rl-0.3.3/modular_rl/agents/_agent.py
+-rw-rw-rw-   0        0        0     4838 2023-06-06 21:35:21.000000 modular_rl-0.3.3/modular_rl/agents/_custom.py
+-rw-rw-rw-   0        0        0    11741 2023-06-08 11:22:46.000000 modular_rl-0.3.3/modular_rl/agents/mcis.py
+-rw-rw-rw-   0        0        0    12162 2023-06-15 13:13:37.000000 modular_rl-0.3.3/modular_rl/agents/mcts.py
+-rw-rw-rw-   0        0        0    22611 2023-06-14 12:35:48.000000 modular_rl-0.3.3/modular_rl/agents/mim.py
+-rw-rw-rw-   0        0        0    14958 2023-06-06 21:36:06.000000 modular_rl-0.3.3/modular_rl/agents/ppo.py
+drwxrwxrwx   0        0        0        0 2023-06-15 14:19:25.947262 modular_rl-0.3.3/modular_rl/envs/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:09:01.000000 modular_rl-0.3.3/modular_rl/envs/__init__.py
+-rw-rw-rw-   0        0        0      133 2023-06-04 21:09:01.000000 modular_rl-0.3.3/modular_rl/envs/_custom.py
+drwxrwxrwx   0        0        0        0 2023-06-15 14:19:25.951690 modular_rl-0.3.3/modular_rl/envs/mim/
+-rw-rw-rw-   0        0        0       25 2023-06-04 21:09:01.000000 modular_rl-0.3.3/modular_rl/envs/mim/__init__.py
+-rw-rw-rw-   0        0        0    15402 2023-06-04 21:09:01.000000 modular_rl-0.3.3/modular_rl/envs/mim/card_evaluator.py
+-rw-rw-rw-   0        0        0     4413 2023-06-14 12:37:11.000000 modular_rl-0.3.3/modular_rl/envs/mim/mim.py
+drwxrwxrwx   0        0        0        0 2023-06-15 14:19:25.958218 modular_rl-0.3.3/modular_rl/networks/
+-rw-rw-rw-   0        0        0       68 2023-05-07 14:51:41.000000 modular_rl-0.3.3/modular_rl/networks/__init__.py
+-rw-rw-rw-   0        0        0     2174 2023-05-07 14:51:41.000000 modular_rl-0.3.3/modular_rl/networks/actor_critic.py
+-rw-rw-rw-   0        0        0     2878 2023-05-04 23:35:18.000000 modular_rl-0.3.3/modular_rl/networks/policy.py
+-rw-rw-rw-   0        0        0     2688 2023-05-04 23:33:52.000000 modular_rl-0.3.3/modular_rl/networks/value.py
+drwxrwxrwx   0        0        0        0 2023-06-15 14:19:25.965168 modular_rl-0.3.3/modular_rl/params/
+-rw-rw-rw-   0        0        0       85 2023-06-04 21:09:01.000000 modular_rl-0.3.3/modular_rl/params/__init__.py
+-rw-rw-rw-   0        0        0     2161 2023-06-04 21:09:01.000000 modular_rl-0.3.3/modular_rl/params/mcis.py
+-rw-rw-rw-   0        0        0     2294 2023-06-08 11:07:34.000000 modular_rl-0.3.3/modular_rl/params/mcts.py
+-rw-rw-rw-   0        0        0     2933 2023-06-13 11:17:09.000000 modular_rl-0.3.3/modular_rl/params/mim.py
+-rw-rw-rw-   0        0        0     2053 2023-05-07 14:51:41.000000 modular_rl-0.3.3/modular_rl/params/ppo.py
+-rw-rw-rw-   0        0        0     1377 2023-06-06 22:36:03.000000 modular_rl-0.3.3/modular_rl/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-15 14:19:25.968433 modular_rl-0.3.3/modular_rl/util/
+-rw-rw-rw-   0        0        0        0 2023-05-04 23:35:52.000000 modular_rl-0.3.3/modular_rl/util/__init__.py
+-rw-rw-rw-   0        0        0     2533 2023-06-04 21:09:01.000000 modular_rl-0.3.3/modular_rl/util/node.py
+drwxrwxrwx   0        0        0        0 2023-06-15 14:19:25.933520 modular_rl-0.3.3/modular_rl.egg-info/
+-rw-rw-rw-   0        0        0     5688 2023-06-15 14:19:25.000000 modular_rl-0.3.3/modular_rl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1088 2023-06-15 14:19:25.000000 modular_rl-0.3.3/modular_rl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 14:19:25.000000 modular_rl-0.3.3/modular_rl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-15 14:19:25.000000 modular_rl-0.3.3/modular_rl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-15 14:19:25.000000 modular_rl-0.3.3/modular_rl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1414 2023-06-12 13:39:56.000000 modular_rl-0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-15 14:19:25.983983 modular_rl-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      937 2023-06-12 13:39:35.000000 modular_rl-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 14:19:25.980433 modular_rl-0.3.3/tests/
+-rw-rw-rw-   0        0        0      383 2023-06-11 10:42:57.000000 modular_rl-0.3.3/tests/test_mcis.py
+-rw-rw-rw-   0        0        0      725 2023-06-11 10:42:57.000000 modular_rl-0.3.3/tests/test_mcis_modular.py
+-rw-rw-rw-   0        0        0      383 2023-06-11 10:42:57.000000 modular_rl-0.3.3/tests/test_mcts.py
+-rw-rw-rw-   0        0        0     1077 2023-06-11 10:42:57.000000 modular_rl-0.3.3/tests/test_mcts_modular.py
+-rw-rw-rw-   0        0        0      342 2023-06-11 10:42:57.000000 modular_rl-0.3.3/tests/test_mim.py
+-rw-rw-rw-   0        0        0      567 2023-06-11 10:42:57.000000 modular_rl-0.3.3/tests/test_mim_modular.py
+-rw-rw-rw-   0        0        0      912 2023-06-11 10:42:57.000000 modular_rl-0.3.3/tests/test_ppo.py
+-rw-rw-rw-   0        0        0     1470 2023-06-11 10:42:57.000000 modular_rl-0.3.3/tests/test_ppo_modular.py
```

### Comparing `modular_rl-0.3.2/LICENSE` & `modular_rl-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.2/PKG-INFO` & `modular_rl-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modular_rl
-Version: 0.3.2
+Version: 0.3.3
 Summary: ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm.
 Home-page: https://github.com/horrible-gh/ModularRL
 Author: sjm
 Author-email: horrible <shinjpn1@gmail.com>
 Project-URL: Homepage, https://github.com/horrible-gh/ModularRL
 Project-URL: Bug Tracker, https://github.com/horrible-gh/ModularRL/issues
 Keywords: ModularRL,Modular-RL,Modular_RL,Modular RL,modularrl,modular_rl,modular-rl,modular rl,mrl,modular,learn,learning,pytorch learn,pytorch learning
```

### Comparing `modular_rl-0.3.2/README.md` & `modular_rl-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.2/modular_rl/agents/_agent.py` & `modular_rl-0.3.3/modular_rl/agents/_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,18 +94,21 @@
 
     def init_policy_value(self):
         """
         Initializes policy and value networks, and their respective optimizers.
         """
 
         # Create neural network instances and optimizer
+        networks_size = self.setting.get('networks', 'middle')
+        Logger.verb('_agent:init_policy_value',
+                    f'Initialize policy and value networks to {networks_size}')
         self.policy_net = PolicyNetwork(
-            self.state_dim, self.action_dim, self.setting.get('networks', 'middle'))
+            self.state_dim, self.action_dim, networks_size)
         self.value_net = ValueNetwork(
-            self.state_dim, self.setting.get('networks', 'middle'))
+            self.state_dim, networks_size)
         self.policy_optimizer = optim.Adam(
             self.policy_net.parameters(), lr=self.setting.get('optimizer_speed', 3e-4))
         self.value_optimizer = optim.Adam(
             self.value_net.parameters(), lr=self.setting.get('optimizer_speed', 3e-4))
 
     def init_actor_critic(self):
         """
@@ -276,7 +279,19 @@
         self.episode_reward += reward
         self.total_reward += reward
         self.prev_reward = reward
 
     def update_episode(self):
         self.episode += 1
         self.episode_reward = 0
+
+    def convert_float_to_double(self, input_tensor):
+        if input_tensor.dtype == torch.float32:
+            return input_tensor.double()
+        else:
+            return input_tensor
+
+    def ensure_float(self, input_tensor):
+        if input_tensor.dtype == torch.float64:
+            return input_tensor.float()
+        else:
+            return input_tensor
```

### Comparing `modular_rl-0.3.2/modular_rl/agents/_custom.py` & `modular_rl-0.3.3/modular_rl/agents/_custom.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.2/modular_rl/agents/mcis.py` & `modular_rl-0.3.3/modular_rl/agents/mcis.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.2/modular_rl/agents/mcts.py` & `modular_rl-0.3.3/modular_rl/agents/mcts.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,14 +185,15 @@
         :param action: The action taken in the current state.
         :param reward: The reward received for taking the action in the current state.
         :param next_state: The state resulting from taking the action in the current state.
         :param done: A flag indicating whether the episode has ended.
         :return: The computed actor and critic loss values.
         '''
         # Predict action probabilities and values
+        state = self.ensure_float(state)
         action_probs, values = self.actor_critic_net(state)
 
         # Compute the value loss
         # Convert reward to tensor
         reward = torch.tensor(reward, device=self.device)
         # Convert total_value to tensor
         total_value = torch.tensor(self.total_value, device=self.device)
```

### Comparing `modular_rl-0.3.2/modular_rl/agents/mim.py` & `modular_rl-0.3.3/modular_rl/agents/mim.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,21 @@
             'score_column', ParamMIM.default['score_column'])
         self.simulation_iterations = setting.get(  # The number of iterations for each simulation.
             'simulation_iterations', ParamMIM.default['simulation_iterations'])
         self.superior_rank_adjustment_factor = setting.get(  # The adjustment factor applied to actions that are ranked superior.
             'superior_rank_adjustment_factor', ParamMIM.default['superior_rank_adjustment_factor'])
         self.inferior_rank_adjustment_factor = setting.get(  # The adjustment factor applied to actions that are ranked inferior.
             'inferior_rank_adjustment_factor', ParamMIM.default['inferior_rank_adjustment_factor'])
+        self.std_deviation_factor = setting.get(
+            'std_deviation_factor', ParamMIM.default['std_deviation_factor'])
+        self.skewness_factor = setting.get(
+            'skewness_factor', ParamMIM.default['skewness_factor'])
+        self.kurtosis_factor = setting.get(
+            'kurtosis_factor', ParamMIM.default['kurtosis_factor'])
+
         # Counter for the number of simulation iterations.
         self.simulation_iteration_indexes_count = 0
         # Average of standard deviations for all simulations.
         self.standard_deviations_avg = 0
         self.skews_avg = 0  # Average skewness for all simulations.
         self.kurtosises_avg = 0  # Average kurtosis for all simulations.
         self.reset()  # Reset the simulation results.
@@ -90,14 +97,15 @@
         fixed_states = state[self.fixed_states_name]
         unknown_spaces = state[self.unknown_spaces_name]
         simulation_states = state[self.simulation_states_name]
         excluded_states = state[self.excluded_states_name]
         score_calculation_callback = state[self.score_calculation_callback_name]
         self.my_simulation_number = state[self.my_simulation_number_name]
         score_table = state[self.score_table_name]
+        self.risk_table = state.get('risk_table', None)
         remaining_states = set(simulation_states) - set(excluded_states)
         simulation_table = []
 
         Logger.verb(
             'mim:simulate', f'{self.simulation_states_name},{list(remaining_states)}, {simulation_states}')
 
         self.reset()
@@ -129,15 +137,15 @@
                     break
 
         Logger.verb('mim:simulation_table', simulation_table)
         for index in range(len(simulation_table)):
             sim_result = 0
             for sub_index in range(len(simulation_table[index])):
                 sim_result += simulation_table[index][sub_index] * \
-                    sub_index + 0.001
+                    sub_index + 0.0001
             self.simulation_totals.append(sim_result)
             self.simulation_averages.append(
                 sim_result / self.simulation_iteration_indexes[index])
             self.standard_deviations.append(np.std(simulation_table[index]))
             skewness, kurtosis = self.calc_skewness_kurtosis(
                 simulation_table[index])
             self.skews.append(skewness)
@@ -191,15 +199,19 @@
         :param simulation_size: The size of the simulation.
         :type simulation_size: int
         :return: The adjustment factors for the weights of the simulations.
         :rtype: list
         """
 
         weight_adjustment_factors = [1] * simulation_size
-        factors = [0.125, 0.075, 0.05]
+        factors = [
+            self.std_deviation_factor,
+            self.skewness_factor,
+            self.kurtosis_factor,
+        ]
         averages = [self.standard_deviations_avg,
                     self.skews_avg, self.kurtosises_avg]
         values = [self.standard_deviations, self.skews, self.kurtosises]
 
         for index in range(simulation_size):
             for factor, average, value in zip(factors, averages, values):
                 if average < value[index]:
@@ -257,14 +269,18 @@
                     f'{base_weight},{action_scale},{action_weights}')
 
         my_rank = ranks[0]
         my_average = self.my_simulation_average
         my_action_rank = my_rank
         my_action_rank = self.env.action_space - \
             round(my_rank * action_scale)
+        if my_rank == 1 and action_scale >= 1.5:
+            my_action_rank = self.env.action_space - 1
+        if my_action_rank < 0:
+            my_action_rank = 0
 
         for rank_idx in range(len(ranks)):
             Logger.verb('mim:calculate_action_weights:rank_idx',
                         rank_idx)
             if rank_idx != 0:
                 rank_diff = abs(my_rank - ranks[rank_idx])
                 Logger.verb('mim:calculate_action_weights:rank_diff',
@@ -277,14 +293,18 @@
                                       averages_table[rank_idx]) * (self.inferior_rank_adjustment_factor ** rank_diff)
 
                 Logger.verb('mim:calculate_action_weights:scale,num',
                             f'{action_scale}, {rank_idx}, {average_weight}')
 
                 action_num = self.env.action_space - \
                     round(ranks[rank_idx] * action_scale)
+                if ranks[rank_idx] == 1 and action_scale >= 1.5:
+                    action_num = self.env.action_space - 1
+                if action_num < 0:
+                    action_num = 0
                 Logger.verb('mim:calculate_action_weights:action_num',
                             action_num)
 
                 if check_weights[action_num] == False:
                     check_weights[action_num] = True
                     expect_weight = action_weights[action_num] * \
                         average_weight
@@ -295,20 +315,43 @@
                     if action_weights[action_num] < 1:
                         action_weights[action_num] = 1
                     action_weights[my_action_rank] += weight_diff
                     Logger.verb('mim:calculate_action_weights:scale,num',
                                 f'{action_num}, {action_weights[action_num]}, {my_action_rank}, {action_weights[my_action_rank]}, {average_weight}')
 
         for action_num in range(len(action_weights)):
-            if action_weights[action_num] == 0:
+            if action_weights[action_num] in (0, int(1 / self.env.action_space * 100)):
                 prev_action_weights = action_weights[action_num-1]
                 next_action_weights = action_weights[action_num+1]
                 middle_weight = (prev_action_weights + next_action_weights) / 2
                 action_weights[action_num] = round(middle_weight)
 
+        if self.risk_table:
+            risk_total = sum(self.risk_table)
+            if risk_total != 0:
+                action_weight_total = 0
+                action_weight = 0
+                for risk_num in range(len(self.risk_table)):
+                    action_weight += action_weights[risk_num] * \
+                        self.risk_table[risk_num]
+                    action_weights[risk_num] -= action_weight
+                    action_weight_total += action_weight
+
+                risk_weight = [risk_total-self.risk_table[risk_num]
+                               for risk_num in range(len(self.risk_table))]
+                risk_total = sum(risk_weight)
+
+                Logger.verb('mim:calculate_action_weights:risk_weight,risk_total',
+                            f'{risk_weight},{risk_total}')
+
+                for risk_num in range(len(risk_weight)):
+                    if risk_total != 0:
+                        action_weights[risk_num] += action_weight_total * \
+                            risk_weight[risk_num] / risk_total
+
         Logger.verb('mim:calculate_action_weights:action_weights',
                     action_weights)
         return action_weights
 
     def calculate_weights(self):
         """
         Calculates the weights for the actions based on the simulation results.
@@ -345,19 +388,18 @@
         action_weights = self.calculate_action_weights(
             adjusted_averages, skip_myself)
 
         return action_weights
 
     def select_action(self, state):
         action_list = []
-        if isinstance(self.env.action_space, list):
-            action_table = self.env.action_space
+        if isinstance(self.env.action_space, int) != True:
+            raise Exception("action space be not an integer")
         else:
             action_table = list(range(self.env.action_space))
-        self.env.action_space = len(action_table)
         self.simulate(state)
         action_weights = self.calculate_weights()
         Logger.verb('mim:select_action', action_weights)
         for action_index in range(len(action_weights)):
             for _ in range(int(action_weights[action_index])):
                 action_list.append(action_index)
```

### Comparing `modular_rl-0.3.2/modular_rl/agents/ppo.py` & `modular_rl-0.3.3/modular_rl/agents/ppo.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.2/modular_rl/envs/mim/card_evaluator.py` & `modular_rl-0.3.3/modular_rl/envs/mim/card_evaluator.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.2/modular_rl/envs/mim/mim.py` & `modular_rl-0.3.3/modular_rl/envs/mim/mim.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,140 +1,142 @@
-import random
-from modular_rl.envs._custom import CustomEnv
-from modular_rl.envs.mim.card_evaluator import CardEvaluator
-from LogAssist.log import Logger
-import copy
-
-
-class EnvMIM(CustomEnv):
-    def __init__(self) -> None:
-        self.players = 4
-        self.fixed_states = []
-        self.unknown_spaces = [0, 3, 3, 3]
-        self.simulation_states = []
-        self.excluded_states = []
-        self.score_table = [
-            CardEvaluator.NO_PAIR_BASE,
-            CardEvaluator.ONE_PAIR_BASE,
-            CardEvaluator.TWO_PAIR_BASE,
-            CardEvaluator.THREE_OF_A_KIND_BASE,
-            CardEvaluator.STRAIGHT_BASE,
-            CardEvaluator.BACK_STRAIGHT_BASE,
-            CardEvaluator.MOUNTAIN_BASE,
-            CardEvaluator.FLUSH_BASE,
-            CardEvaluator.FULL_HOUSE_BASE,
-            CardEvaluator.FOUR_OF_A_KIND_BASE,
-            CardEvaluator.STRAIGHT_FLUSH_BASE,
-            CardEvaluator.BACK_STRAIGHT_FLUSH_BASE,
-            CardEvaluator.ROYAL_STRAIGHT_FLUSH_BASE
-        ]
-        self.state = {
-            'fixed_states': self.fixed_states,
-            'unknown_spaces': self.unknown_spaces,
-            'simulation_states': self.simulation_states,
-            'excluded_states': self.excluded_states,
-            'my_simulation_number': 0,
-            'score_table': self.score_table,
-            'score_calculation_callback': lambda cards: CardEvaluator.card_evaluator(cards),
-        }
-
-        # self.action_space = 3
-        self.action_space = [0, 1, 2]
-
-        self.shuffle()
-
-    def shuffle(self):
-        self.simulation_states = list(range(52))
-        self.allocate_max = 52
-        random.shuffle(self.simulation_states)
-        self.current_card = 0
-
-    def reset(self):
-        self.fixed_states.clear()
-        self.simulation_states.clear()
-
-        self.shuffle()
-        self.state['simulation_states'] = self.simulation_states
-
-        for player in range(self.players):
-            self.fixed_states.append([])
-
-        for i in range(4):
-            for player in range(self.players):
-                self.fixed_states[player].append(self.card_allocate())
-
-        self.fixed_states[0].append(self.card_allocate())
-        self.fixed_states[0].append(self.card_allocate())
-        self.fixed_states[0].append(self.card_allocate())
-
-        Logger.verb('mim:reset', f'{self.simulation_states}')
-
-        return self.state
-
-    def card_allocate(self):
-        if len(self.simulation_states) == 0:
-            return None
-        else:
-            hand = random.choice(self.simulation_states)
-            self.simulation_states.remove(hand)
-            return hand
-
-    def step(self, action):
-        scores = []
-        max_p = len(self.fixed_states)
-        rank = max_p
-
-        step_states = copy.deepcopy(self.fixed_states)
-        Logger.verb('envs:mim:step', step_states)
-        for c in range(3):
-            for p in range(len(step_states)):
-                if p == 0:
-                    continue
-                step_states[p].append(self.card_allocate())
-
-        for p in range(len(step_states)):
-            scores.append(CardEvaluator.card_evaluator(
-                step_states[p])['score'])
-
-        my_score = scores[0]
-        for p in range(len(step_states)):
-            if p == 0:
-                continue
-            if my_score > scores[p]:
-                rank -= 1
-
-        if rank == 1:
-            if action == 2:
-                reward = max_p
-            elif action == 1:
-                reward = max_p / 2
-            else:
-                reward = -2
-        elif rank == 2:
-            if action == 2:
-                reward = max_p - 1
-            elif action == 1:
-                reward = max_p / 2
-            else:
-                reward = -1
-        elif rank == 3:
-            if action == 2:
-                reward = -1
-            elif action == 1:
-                reward = 1
-            else:
-                reward = 1
-        elif rank == 4:
-            if action == 2:
-                reward = -2
-            elif action == 1:
-                reward = -1
-            else:
-                reward = 1
-        elif rank == 5:
-            if action == 2:
-                reward = -2
-            elif action == 1:
-                reward = -2
-            else:
-                reward = 1
-        return step_states, reward, True
+import random
+from modular_rl.envs._custom import CustomEnv
+from modular_rl.envs.mim.card_evaluator import CardEvaluator
+from LogAssist.log import Logger
+import copy
+
+
+class EnvMIM(CustomEnv):
+    def __init__(self) -> None:
+        self.players = 4
+        self.fixed_states = []
+        self.unknown_spaces = [0, 3, 3, 3]
+        self.simulation_states = []
+        self.excluded_states = []
+        self.risk_table = [0, 0, 0]
+        self.score_table = [
+            CardEvaluator.NO_PAIR_BASE,
+            CardEvaluator.ONE_PAIR_BASE,
+            CardEvaluator.TWO_PAIR_BASE,
+            CardEvaluator.THREE_OF_A_KIND_BASE,
+            CardEvaluator.STRAIGHT_BASE,
+            CardEvaluator.BACK_STRAIGHT_BASE,
+            CardEvaluator.MOUNTAIN_BASE,
+            CardEvaluator.FLUSH_BASE,
+            CardEvaluator.FULL_HOUSE_BASE,
+            CardEvaluator.FOUR_OF_A_KIND_BASE,
+            CardEvaluator.STRAIGHT_FLUSH_BASE,
+            CardEvaluator.BACK_STRAIGHT_FLUSH_BASE,
+            CardEvaluator.ROYAL_STRAIGHT_FLUSH_BASE
+        ]
+        self.state = {
+            'fixed_states': self.fixed_states,
+            'unknown_spaces': self.unknown_spaces,
+            'simulation_states': self.simulation_states,
+            'excluded_states': self.excluded_states,
+            'my_simulation_number': 0,
+            'score_table': self.score_table,
+            'score_calculation_callback': lambda cards: CardEvaluator.card_evaluator(cards),
+            'risk_table': self.risk_table,
+        }
+
+        self.action_space = 3
+        # self.action_space = [0, 1, 2]
+
+        self.shuffle()
+
+    def shuffle(self):
+        self.simulation_states = list(range(52))
+        self.allocate_max = 52
+        random.shuffle(self.simulation_states)
+        self.current_card = 0
+
+    def reset(self):
+        self.fixed_states.clear()
+        self.simulation_states.clear()
+
+        self.shuffle()
+        self.state['simulation_states'] = self.simulation_states
+
+        for player in range(self.players):
+            self.fixed_states.append([])
+
+        for i in range(4):
+            for player in range(self.players):
+                self.fixed_states[player].append(self.card_allocate())
+
+        self.fixed_states[0].append(self.card_allocate())
+        self.fixed_states[0].append(self.card_allocate())
+        self.fixed_states[0].append(self.card_allocate())
+
+        Logger.verb('mim:reset', f'{self.simulation_states}')
+
+        return self.state
+
+    def card_allocate(self):
+        if len(self.simulation_states) == 0:
+            return None
+        else:
+            hand = random.choice(self.simulation_states)
+            self.simulation_states.remove(hand)
+            return hand
+
+    def step(self, action):
+        scores = []
+        max_p = len(self.fixed_states)
+        rank = max_p
+
+        step_states = copy.deepcopy(self.fixed_states)
+        Logger.verb('envs:mim:step', step_states)
+        for c in range(3):
+            for p in range(len(step_states)):
+                if p == 0:
+                    continue
+                step_states[p].append(self.card_allocate())
+
+        for p in range(len(step_states)):
+            scores.append(CardEvaluator.card_evaluator(
+                step_states[p])['score'])
+
+        my_score = scores[0]
+        for p in range(len(step_states)):
+            if p == 0:
+                continue
+            if my_score > scores[p]:
+                rank -= 1
+
+        if rank == 1:
+            if action == 2:
+                reward = max_p
+            elif action == 1:
+                reward = max_p / 2
+            else:
+                reward = -2
+        elif rank == 2:
+            if action == 2:
+                reward = max_p - 1
+            elif action == 1:
+                reward = max_p / 2
+            else:
+                reward = -1
+        elif rank == 3:
+            if action == 2:
+                reward = -1
+            elif action == 1:
+                reward = 1
+            else:
+                reward = 1
+        elif rank == 4:
+            if action == 2:
+                reward = -2
+            elif action == 1:
+                reward = -1
+            else:
+                reward = 1
+        elif rank == 5:
+            if action == 2:
+                reward = -2
+            elif action == 1:
+                reward = -2
+            else:
+                reward = 1
+        return step_states, reward, True
```

### Comparing `modular_rl-0.3.2/modular_rl/networks/actor_critic.py` & `modular_rl-0.3.3/modular_rl/networks/actor_critic.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.2/modular_rl/networks/policy.py` & `modular_rl-0.3.3/modular_rl/networks/policy.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.2/modular_rl/networks/value.py` & `modular_rl-0.3.3/modular_rl/networks/value.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.2/modular_rl/params/mcis.py` & `modular_rl-0.3.3/modular_rl/params/mcis.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.2/modular_rl/params/mcts.py` & `modular_rl-0.3.3/modular_rl/params/mcts.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.2/modular_rl/params/mim.py` & `modular_rl-0.3.3/modular_rl/params/mim.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,42 @@
-
 class ParamMIM:
     default = {
         # The column name used to track the score for evaluating agent's actions.
         'score_column': 'score',
         # The number of iterations for each simulation during the MIM's action selection process.
         'simulation_iterations': 30,
         # The adjustment factor applied to actions that are ranked superior (i.e., they have a higher score). Lower values result in greater down-weighting.
-        'superior_rank_adjustment_factor': 0.9,
+        'superior_rank_adjustment_factor': 0.95,
         # The adjustment factor applied to actions that are ranked inferior (i.e., they have a lower score). Lower values result in greater up-weighting.
-        'inferior_rank_adjustment_factor': 0.85,
+        'inferior_rank_adjustment_factor': 0.9,
+        # The adjustment factor for standard deviation in the weight adjustment calculation. Lower values lead to a stronger adjustment.
+        'std_deviation_factor': 0.066,
+        # The adjustment factor for skewness in the weight adjustment calculation. Lower values lead to a stronger adjustment.
+        'skewness_factor': 0.033,
+        # The adjustment factor for kurtosis in the weight adjustment calculation. Lower values lead to a stronger adjustment.
+        'kurtosis_factor': 0.025,
         'log_level': 'debug',  # Log level for the logger
         'log_init_pass': False,  # If True, skip logger initialization
         'max_episodes': 10,  # Maximum number of episodes for training
         'max_timesteps': 200,  # Maximum number of timesteps for each episode
     }
 
     default_modular = {
         # The column name used to track the score for evaluating agent's actions.
         'score_column': 'score',
         # The number of iterations for each simulation during the MIM's action selection process.
         'simulation_iterations': 1,
         # The adjustment factor applied to actions that are ranked superior (i.e., they have a higher score). Lower values result in greater down-weighting.
-        'superior_rank_adjustment_factor': 0.9,
+        'superior_rank_adjustment_factor': 0.95,
         # The adjustment factor applied to actions that are ranked inferior (i.e., they have a lower score). Lower values result in greater up-weighting.
-        'inferior_rank_adjustment_factor': 0.85,
+        'inferior_rank_adjustment_factor': 0.9,
+        # The adjustment factor for standard deviation in the weight adjustment calculation. Lower values lead to a stronger adjustment.
+        'std_deviation_factor': 0.066,
+        # The adjustment factor for skewness in the weight adjustment calculation. Lower values lead to a stronger adjustment.
+        'skewness_factor': 0.033,
+        # The adjustment factor for kurtosis in the weight adjustment calculation. Lower values lead to a stronger adjustment.
+        'kurtosis_factor': 0.025,
         'log_level': 'debug',  # Log level for the logger
         'log_init_pass': False,  # If True, skip logger initialization
         'max_episodes': 1,  # Maximum number of episodes for training
         'max_timesteps': 1,  # Maximum number of timesteps for each episode
     }
```

### Comparing `modular_rl-0.3.2/modular_rl/params/ppo.py` & `modular_rl-0.3.3/modular_rl/params/ppo.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.2/modular_rl/settings.py` & `modular_rl-0.3.3/modular_rl/settings.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.2/modular_rl/tester/mcis.py` & `modular_rl-0.3.3/tests/test_mcts_modular.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-import gym
-from modular_rl.settings import AgentSettings
-from modular_rl.agents.mcis import AgentMCIS
-
-
-def init_mcis():
-    env = gym.make('CartPole-v0')
-    setting = AgentSettings.default_mcts
-    setting['num_simulations'] = 10
-    setting['max_episodes'] = 10
-    setting['log_level'] = 'verb'
-    agent = AgentMCIS(env, setting)
-    agent.train()
-
-
-def init_mcis_modular():
-    mcis_agent = AgentMCIS(
-        env=None, setting=AgentSettings.default_mcis_modular)
-
-    mcis_agent.reset()
-
-    state = mcis_agent.learn_reset()
-    action = mcis_agent.select_action(state)
-    next_state = mcis_agent.learn_reset()
-    mcis_agent.update_step(state, action, 1, False, next_state)
-    mcis_agent.learn_check()
-
-    state = mcis_agent.learn_reset()
-    action = mcis_agent.select_action(state)
-    next_state = mcis_agent.learn_reset()
-    mcis_agent.update_step(state, action, 1, True, next_state)
-    mcis_agent.learn_check()
-
-    # update_step function automatically updates if done is given a True option
-    # mcis_agent.update()
+import gym
+from modular_rl.settings import AgentSettings
+from modular_rl.agents.mcts import AgentMCTS
+
+
+def init_mcts_modular():
+    setting = AgentSettings.default_mcts_modular
+    setting['log_level'] = 'verb'
+    mcts_agent = AgentMCTS(
+        env=None, setting=setting)
+
+    mcts_agent.reset()
+
+    state = mcts_agent.learn_reset()
+    state, action, reward, done = mcts_agent.select_action(state)
+    next_state, reward, done, _, _ = mcts_agent.env.step(action)
+    # Modular does not automatically generate the required values and stores them through update_step
+    mcts_agent.update_step(state, action, reward, done, next_state)
+
+    if done:
+        mcts_agent.update()
+
+    mcts_agent.learn_check()
+
+    state = mcts_agent.learn_reset()
+    state, action, reward, done = mcts_agent.select_action(state)
+    next_state, reward, done, _, _ = mcts_agent.env.step(action)
+    mcts_agent.update_step(state, action, reward, done, next_state)
+
+    if done:
+        mcts_agent.update()
+
+    mcts_agent.learn_check()
+
+
+init_mcts_modular()
```

### Comparing `modular_rl-0.3.2/modular_rl/tester/mim.py` & `modular_rl-0.3.3/tests/test_mim_modular.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,21 @@
-# -*- coding: utf-8 -*-
-from modular_rl.agents.mim import AgentMIM
-from modular_rl.settings import AgentSettings
-from modular_rl.envs.mim import EnvMIM
-
-
-def init_mim():
-    setting = AgentSettings.default_mim
-    setting['log_level'] = 'debug'
-    agent = AgentMIM(env=EnvMIM(), setting=setting)
-    agent.learn()
-
-
-def init_mim_modular():
-    setting = AgentSettings.default_mim_modular
-    setting['log_level'] = 'debug'
-    env = EnvMIM()
-    agent = AgentMIM(env=env, setting=setting)
-
-    agent.reset()
-    state = agent.learn_reset()
-    action = agent.select_action(state)
-    next_state, reward, done = env.step(action)
-    agent.update_step(reward, done)
-    agent.learn_check()
+# -*- coding: utf-8 -*-
+from modular_rl.agents.mim import AgentMIM
+from modular_rl.settings import AgentSettings
+from modular_rl.envs.mim import EnvMIM
+
+
+def init_mim_modular():
+    setting = AgentSettings.default_mim_modular
+    setting['log_level'] = 'verb'
+    env = EnvMIM()
+    agent = AgentMIM(env=env, setting=setting)
+
+    agent.reset()
+    state = agent.learn_reset()
+    action = agent.select_action(state)
+    next_state, reward, done = env.step(action)
+    agent.update_step(reward, done)
+    agent.learn_check()
+
+
+init_mim_modular()
```

### Comparing `modular_rl-0.3.2/modular_rl/tester/ppo.py` & `modular_rl-0.3.3/tests/test_ppo_modular.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 # -*- coding: utf-8 -*-
 from modular_rl.agents.ppo import AgentPPO
 from modular_rl.settings import AgentSettings
 
 '''
-This code is a Python script that initializes and trains an instance of the AgentPPO class with default settings using the init_ppo() function. 
+This code is a Python script that initializes and trains an instance of the AgentPPO class with default settings using the init_ppo() function.
 Additionally, the init_ppo_modular() function is provided to demonstrate the usage of the AgentPPO class with modified settings.
 
-In init_ppo_modular(), an instance of AgentPPO is created with a modified default_modular settings dictionary. 
-The function then calls various methods of the instance, such as reset(), learn_reset(), learn_next(), and update() to demonstrate the functionality of the class. 
+In init_ppo_modular(), an instance of AgentPPO is created with a modified default_modular settings dictionary.
+The function then calls various methods of the instance, such as reset(), learn_reset(), learn_next(), and update() to demonstrate the functionality of the class.
 The instance is then saved to a file using the save_model() method, which is not shown in the provided code.
 
 '''
 
 
-def init_ppo():
-    env = AgentPPO(env=None, setting=AgentSettings.default_ppo)
-    env.learn()
-
-
 def init_ppo_modular():
     env = AgentPPO(env=None, setting=AgentSettings.default_ppo_modular)
     env.reset()
     env.learn_reset()
     env.learn_next()
     env.learn_check()
     env.learn_next()
@@ -41,7 +36,10 @@
 
 
 def ppo_manual_step(env):
     initial_state = env.learn_reset()
     action, _ = env.select_action(initial_state)
     next_state = env.learn_reset()
     env.update_step(next_state, None, action, -1)
+
+
+init_ppo_modular()
```

### Comparing `modular_rl-0.3.2/modular_rl/util/node.py` & `modular_rl-0.3.3/modular_rl/util/node.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.2/modular_rl.egg-info/PKG-INFO` & `modular_rl-0.3.3/modular_rl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modular-rl
-Version: 0.3.2
+Version: 0.3.3
 Summary: ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm.
 Home-page: https://github.com/horrible-gh/ModularRL
 Author: sjm
 Author-email: horrible <shinjpn1@gmail.com>
 Project-URL: Homepage, https://github.com/horrible-gh/ModularRL
 Project-URL: Bug Tracker, https://github.com/horrible-gh/ModularRL/issues
 Keywords: ModularRL,Modular-RL,Modular_RL,Modular RL,modularrl,modular_rl,modular-rl,modular rl,mrl,modular,learn,learning,pytorch learn,pytorch learning
```

### Comparing `modular_rl-0.3.2/modular_rl.egg-info/SOURCES.txt` & `modular_rl-0.3.3/modular_rl.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -26,19 +26,14 @@
 modular_rl/networks/policy.py
 modular_rl/networks/value.py
 modular_rl/params/__init__.py
 modular_rl/params/mcis.py
 modular_rl/params/mcts.py
 modular_rl/params/mim.py
 modular_rl/params/ppo.py
-modular_rl/tester/__init__.py
-modular_rl/tester/mcis.py
-modular_rl/tester/mcts.py
-modular_rl/tester/mim.py
-modular_rl/tester/ppo.py
 modular_rl/util/__init__.py
 modular_rl/util/node.py
 tests/test_mcis.py
 tests/test_mcis_modular.py
 tests/test_mcts.py
 tests/test_mcts_modular.py
 tests/test_mim.py
```

### Comparing `modular_rl-0.3.2/pyproject.toml` & `modular_rl-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "modular_rl"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
   { name="horrible", email="shinjpn1@gmail.com" },
 ]
 description = "ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `modular_rl-0.3.2/setup.py` & `modular_rl-0.3.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='modular_rl',
-    version='0.3.2',
+    version='0.3.3',
     description='ModularRL package',
     author='sjm',
     author_email='shinjpn1@gmail.com',
     url='https://github.com/horrible-gh/ModularRL',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

