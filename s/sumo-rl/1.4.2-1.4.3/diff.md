# Comparing `tmp/sumo-rl-1.4.2.tar.gz` & `tmp/sumo-rl-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumo-rl-1.4.2.tar", last modified: Sun Feb 26 20:08:24 2023, max compression
+gzip compressed data, was "sumo-rl-1.4.3.tar", last modified: Thu Jun 15 14:08:56 2023, max compression
```

## Comparing `sumo-rl-1.4.2.tar` & `sumo-rl-1.4.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 20:08:24.499577 sumo-rl-1.4.2/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1069 2023-02-26 20:08:07.000000 sumo-rl-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-02-26 20:08:24.499577 sumo-rl-1.4.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    11149 2023-02-26 20:08:07.000000 sumo-rl-1.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-02-26 20:08:07.000000 sumo-rl-1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-26 20:08:24.499577 sumo-rl-1.4.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      433 2023-02-26 20:08:07.000000 sumo-rl-1.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 20:08:24.495577 sumo-rl-1.4.2/sumo_rl/
--rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-02-26 20:08:07.000000 sumo-rl-1.4.2/sumo_rl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 20:08:24.495577 sumo-rl-1.4.2/sumo_rl/agents/
--rwxr-xr-x   0 runner    (1001) docker     (123)      140 2023-02-26 20:08:07.000000 sumo-rl-1.4.2/sumo_rl/agents/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1351 2023-02-26 20:08:07.000000 sumo-rl-1.4.2/sumo_rl/agents/ql_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 20:08:24.499577 sumo-rl-1.4.2/sumo_rl/environment/
--rwxr-xr-x   0 runner    (1001) docker     (123)      230 2023-02-26 20:08:07.000000 sumo-rl-1.4.2/sumo_rl/environment/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23937 2023-02-26 20:08:07.000000 sumo-rl-1.4.2/sumo_rl/environment/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-02-26 20:08:07.000000 sumo-rl-1.4.2/sumo_rl/environment/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-02-26 20:08:07.000000 sumo-rl-1.4.2/sumo_rl/environment/resco_envs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13778 2023-02-26 20:08:07.000000 sumo-rl-1.4.2/sumo_rl/environment/traffic_signal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 20:08:24.499577 sumo-rl-1.4.2/sumo_rl/exploration/
--rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-02-26 20:08:07.000000 sumo-rl-1.4.2/sumo_rl/exploration/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      926 2023-02-26 20:08:07.000000 sumo-rl-1.4.2/sumo_rl/exploration/epsilon_greedy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      531 2023-02-26 20:08:07.000000 sumo-rl-1.4.2/sumo_rl/exploration/plot_epsilon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 20:08:24.499577 sumo-rl-1.4.2/sumo_rl/util/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 20:08:07.000000 sumo-rl-1.4.2/sumo_rl/util/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9411 2023-02-26 20:08:07.000000 sumo-rl-1.4.2/sumo_rl/util/gen_route.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10759 2023-02-26 20:08:07.000000 sumo-rl-1.4.2/sumo_rl/util/xml2csv.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5345 2023-02-26 20:08:07.000000 sumo-rl-1.4.2/sumo_rl/util/xsd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 20:08:24.495577 sumo-rl-1.4.2/sumo_rl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-02-26 20:08:24.000000 sumo-rl-1.4.2/sumo_rl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-02-26 20:08:24.000000 sumo-rl-1.4.2/sumo_rl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-26 20:08:24.000000 sumo-rl-1.4.2/sumo_rl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-02-26 20:08:24.000000 sumo-rl-1.4.2/sumo_rl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-26 20:08:24.000000 sumo-rl-1.4.2/sumo_rl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:56.386714 sumo-rl-1.4.3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1069 2023-06-15 14:08:43.000000 sumo-rl-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-06-15 14:08:56.386714 sumo-rl-1.4.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10994 2023-06-15 14:08:43.000000 sumo-rl-1.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-06-15 14:08:43.000000 sumo-rl-1.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 14:08:56.386714 sumo-rl-1.4.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      433 2023-06-15 14:08:43.000000 sumo-rl-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:56.386714 sumo-rl-1.4.3/sumo_rl/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      368 2023-06-15 14:08:43.000000 sumo-rl-1.4.3/sumo_rl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:56.386714 sumo-rl-1.4.3/sumo_rl/agents/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      140 2023-06-15 14:08:43.000000 sumo-rl-1.4.3/sumo_rl/agents/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1351 2023-06-15 14:08:43.000000 sumo-rl-1.4.3/sumo_rl/agents/ql_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:56.386714 sumo-rl-1.4.3/sumo_rl/environment/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      230 2023-06-15 14:08:43.000000 sumo-rl-1.4.3/sumo_rl/environment/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24203 2023-06-15 14:08:43.000000 sumo-rl-1.4.3/sumo_rl/environment/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-15 14:08:43.000000 sumo-rl-1.4.3/sumo_rl/environment/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-15 14:08:43.000000 sumo-rl-1.4.3/sumo_rl/environment/resco_envs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13778 2023-06-15 14:08:43.000000 sumo-rl-1.4.3/sumo_rl/environment/traffic_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:56.386714 sumo-rl-1.4.3/sumo_rl/exploration/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-06-15 14:08:43.000000 sumo-rl-1.4.3/sumo_rl/exploration/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      926 2023-06-15 14:08:43.000000 sumo-rl-1.4.3/sumo_rl/exploration/epsilon_greedy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      530 2023-06-15 14:08:43.000000 sumo-rl-1.4.3/sumo_rl/exploration/plot_epsilon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:56.386714 sumo-rl-1.4.3/sumo_rl/util/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:43.000000 sumo-rl-1.4.3/sumo_rl/util/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9411 2023-06-15 14:08:43.000000 sumo-rl-1.4.3/sumo_rl/util/gen_route.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10759 2023-06-15 14:08:43.000000 sumo-rl-1.4.3/sumo_rl/util/xml2csv.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5345 2023-06-15 14:08:43.000000 sumo-rl-1.4.3/sumo_rl/util/xsd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:56.386714 sumo-rl-1.4.3/sumo_rl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-06-15 14:08:56.000000 sumo-rl-1.4.3/sumo_rl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-15 14:08:56.000000 sumo-rl-1.4.3/sumo_rl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:08:56.000000 sumo-rl-1.4.3/sumo_rl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-15 14:08:56.000000 sumo-rl-1.4.3/sumo_rl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 14:08:56.000000 sumo-rl-1.4.3/sumo_rl.egg-info/top_level.txt
```

### Comparing `sumo-rl-1.4.2/LICENSE` & `sumo-rl-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sumo-rl-1.4.2/PKG-INFO` & `sumo-rl-1.4.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,31 @@
-Metadata-Version: 2.1
-Name: sumo-rl
-Version: 1.4.2
-Summary: RL environments and learning code for traffic signal control in SUMO.
-Author-email: Lucas Alegre <lucasnale@gmail.com>
-License: MIT License
-Project-URL: Homepage, https://lucasalegre.github.io/sumo-rl
-Project-URL: Repository, https://github.com/LucasAlegre/sumo-rl
-Project-URL: Documentation, https://lucasalegre.github.io/sumo-rl
-Project-URL: Bug Report, https://github.com/LucasAlegre/sumo-rl/issues
-Keywords: Reinforcement Learning,Traffic Signal Control,SUMO,RL,PettingZoo,gymnasium
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: rendering
-Provides-Extra: all
-Provides-Extra: testing
-License-File: LICENSE
-
 <img src="docs/_static/logo.png" align="right" width="30%"/>
 
 [![tests](https://github.com/LucasAlegre/sumo-rl/actions/workflows/linux-test.yml/badge.svg)](https://github.com/LucasAlegre/sumo-rl/actions/workflows/linux-test.yml)
 [![PyPI version](https://badge.fury.io/py/sumo-rl.svg)](https://badge.fury.io/py/sumo-rl)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![License](http://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://github.com/LucasAlegre/sumo-rl/blob/master/LICENSE)
+[![License](http://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://github.com/LucasAlegre/sumo-rl/blob/main/LICENSE)
 
 # SUMO-RL
 
 <!-- start intro -->
 
 SUMO-RL provides a simple interface to instantiate Reinforcement Learning (RL) environments with [SUMO](https://github.com/eclipse/sumo) for Traffic Signal Control.
 
 Goals of this repository:
 - Provide a simple interface to work with Reinforcement Learning for Traffic Signal Control using SUMO
 - Support Multiagent RL
-- Compatibility with gymnasium.Env and popular RL libraries such as [stable-baselines3](https://github.com/DLR-RM/stable-baselines3) and [RLlib](https://docs.ray.io/en/master/rllib.html)
+- Compatibility with gymnasium.Env and popular RL libraries such as [stable-baselines3](https://github.com/DLR-RM/stable-baselines3) and [RLlib](https://docs.ray.io/en/main/rllib.html)
 - Easy customisation: state and reward definitions are easily modifiable
 
-The main class is [SumoEnvironment](https://github.com/LucasAlegre/sumo-rl/blob/master/sumo_rl/environment/env.py).
+The main class is [SumoEnvironment](https://github.com/LucasAlegre/sumo-rl/blob/main/sumo_rl/environment/env.py).
 If instantiated with parameter 'single-agent=True', it behaves like a regular [Gymnasium Env](https://github.com/Farama-Foundation/Gymnasium).
-For multiagent environments, use [env](https://github.com/LucasAlegre/sumo-rl/blob/master/sumo_rl/environment/env.py) or [parallel_env](https://github.com/LucasAlegre/sumo-rl/blob/master/sumo_rl/environment/env.py) to instantiate a [PettingZoo](https://github.com/PettingZoo-Team/PettingZoo) environment with AEC or Parallel API, respectively.
-[TrafficSignal](https://github.com/LucasAlegre/sumo-rl/blob/master/sumo_rl/environment/traffic_signal.py) is responsible for retrieving information and actuating on traffic lights using [TraCI](https://sumo.dlr.de/wiki/TraCI) API.
+For multiagent environments, use [env](https://github.com/LucasAlegre/sumo-rl/blob/main/sumo_rl/environment/env.py) or [parallel_env](https://github.com/LucasAlegre/sumo-rl/blob/main/sumo_rl/environment/env.py) to instantiate a [PettingZoo](https://github.com/PettingZoo-Team/PettingZoo) environment with AEC or Parallel API, respectively.
+[TrafficSignal](https://github.com/LucasAlegre/sumo-rl/blob/main/sumo_rl/environment/traffic_signal.py) is responsible for retrieving information and actuating on traffic lights using [TraCI](https://sumo.dlr.de/wiki/TraCI) API.
 
 For more details, check the [documentation online](https://lucasalegre.github.io/sumo-rl/).
 
 <!-- end intro -->
 
 ## Install
 
@@ -94,26 +76,26 @@
     obs = [phase_one_hot, min_green, lane_1_density,...,lane_n_density, lane_1_queue,...,lane_n_queue]
 ```
 - ```phase_one_hot``` is a one-hot encoded vector indicating the current active green phase
 - ```min_green``` is a binary variable indicating whether min_green seconds have already passed in the current phase
 - ```lane_i_density``` is the number of vehicles in incoming lane i dividided by the total capacity of the lane
 - ```lane_i_queue```is the number of queued (speed below 0.1 m/s) vehicles in incoming lane i divided by the total capacity of the lane
 
-You can define your own observation by implementing a class that inherits from [ObservationFunction](https://github.com/LucasAlegre/sumo-rl/blob/master/sumo_rl/environment/observations.py) and passing it to the environment constructor.
+You can define your own observation by implementing a class that inherits from [ObservationFunction](https://github.com/LucasAlegre/sumo-rl/blob/main/sumo_rl/environment/observations.py) and passing it to the environment constructor.
 
 <!-- end observation -->
 
 ### Action
 
 <!-- start action -->
 
 The action space is discrete.
 Every 'delta_time' seconds, each traffic signal agent can choose the next green phase configuration.
 
-E.g.: In the [2-way single intersection](https://github.com/LucasAlegre/sumo-rl/blob/master/experiments/dqn_2way-single-intersection.py) there are |A| = 4 discrete actions, corresponding to the following green phase configurations:
+E.g.: In the [2-way single intersection](https://github.com/LucasAlegre/sumo-rl/blob/main/experiments/dqn_2way-single-intersection.py) there are |A| = 4 discrete actions, corresponding to the following green phase configurations:
 
 <p align="center">
 <img src="docs/_static/actions.png" align="center" width="75%"/>
 </p>
 
 Important: every time a phase change occurs, the next phase is preeceded by a yellow phase lasting ```yellow_time``` seconds.
 
@@ -127,15 +109,15 @@
 
 <p align="center">
 <img src="docs/_static/reward.png" align="center" width="25%"/>
 </p>
 
 That is, the reward is how much the total delay (sum of the waiting times of all approaching vehicles) changed in relation to the previous time-step.
 
-You can choose a different reward function (see the ones implemented in [TrafficSignal](https://github.com/LucasAlegre/sumo-rl/blob/master/sumo_rl/environment/traffic_signal.py)) with the parameter `reward_fn` in the [SumoEnvironment](https://github.com/LucasAlegre/sumo-rl/blob/master/sumo_rl/environment/env.py) constructor.
+You can choose a different reward function (see the ones implemented in [TrafficSignal](https://github.com/LucasAlegre/sumo-rl/blob/main/sumo_rl/environment/traffic_signal.py)) with the parameter `reward_fn` in the [SumoEnvironment](https://github.com/LucasAlegre/sumo-rl/blob/main/sumo_rl/environment/env.py) constructor.
 
 It is also possible to implement your own reward function:
 
 ```python
 def my_reward_fn(traffic_signal):
     return traffic_signal.get_average_speed()
 
@@ -173,58 +155,57 @@
 
 <!-- start pettingzoo -->
 
 For multi-agent environments, you can use the PettingZoo API (see [Petting Zoo API](https://pettingzoo.farama.org/api/parallel/)):
 
 ```python
 import sumo_rl
-env = sumo_rl.parallel_env(net_file='sumo_net_file.net.xml',
-                  route_file='sumo_route_file.rou.xml',
+env = sumo_rl.parallel_env(net_file='nets/RESCO/grid4x4/grid4x4.net.xml',
+                  route_file='nets/RESCO/grid4x4/grid4x4_1.rou.xml',
                   use_gui=True,
                   num_seconds=3600)
+observations = env.reset()
 while env.agents:
-    actions = {agent: parallel_env.action_space(agent).sample() for agent in parallel_env.agents}  # this is where you would insert your policy
-    observations, rewards, terminations, truncations, infos = parallel_env.step(actions)
+    actions = {agent: env.action_space(agent).sample() for agent in env.agents}  # this is where you would insert your policy
+    observations, rewards, terminations, truncations, infos = env.step(actions)
 ```
 
 <!-- end pettingzoo -->
 
 ### RESCO Benchmarks
 
-In the folder [nets/RESCO](https://github.com/LucasAlegre/sumo-rl/tree/master/nets/RESCO) you can find the network and route files from [RESCO](https://github.com/jault/RESCO) (Reinforcement Learning Benchmarks for Traffic Signal Control), which was built on top of SUMO-RL. See their [paper](https://people.engr.tamu.edu/guni/Papers/NeurIPS-signals.pdf) for results.
+In the folder [nets/RESCO](https://github.com/LucasAlegre/sumo-rl/tree/main/nets/RESCO) you can find the network and route files from [RESCO](https://github.com/jault/RESCO) (Reinforcement Learning Benchmarks for Traffic Signal Control), which was built on top of SUMO-RL. See their [paper](https://people.engr.tamu.edu/guni/Papers/NeurIPS-signals.pdf) for results.
 
 <p align="center">
 <img src="nets/RESCO/maps.png" align="center" width="60%"/>
 </p>
 
 ### Experiments
 
-WARNING: Gym 0.26 had many breaking changes, stable-baselines3 and RLlib still do not support it, but will be updated soon. See [Stable Baselines 3 PR](https://github.com/DLR-RM/stable-baselines3/pull/780) and [RLib PR](https://github.com/ray-project/ray/pull/28369).
-Hence, only the tabular Q-learning experiment is running without errors for now.
-
-Check [experiments](https://github.com/LucasAlegre/sumo-rl/tree/master/experiments) for examples on how to instantiate an environment and train your RL agent.
+Check [experiments](https://github.com/LucasAlegre/sumo-rl/tree/main/experiments) for examples on how to instantiate an environment and train your RL agent.
 
-### [Q-learning](https://github.com/LucasAlegre/sumo-rl/blob/master/agents/ql_agent.py) in a one-way single intersection:
+### [Q-learning](https://github.com/LucasAlegre/sumo-rl/blob/main/agents/ql_agent.py) in a one-way single intersection:
 ```bash
 python experiments/ql_single-intersection.py
 ```
 
-### [RLlib A3C](https://github.com/ray-project/ray/tree/master/python/ray/rllib/agents/a3c) multiagent in a 4x4 grid:
+### [RLlib PPO](https://docs.ray.io/en/latest/_modules/ray/rllib/algorithms/ppo/ppo.html) multiagent in a 4x4 grid:
 ```bash
-python experiments/a3c_4x4grid.py
+python experiments/ppo_4x4grid.py
 ```
 
 ### [stable-baselines3 DQN](https://github.com/DLR-RM/stable-baselines3/blob/master/stable_baselines3/dqn/dqn.py) in a 2-way single intersection:
+Obs: you need to install stable-baselines3 with ```pip install "stable_baselines3[extra]>=2.0.0a9"``` for [Gymnasium compatibility](https://stable-baselines3.readthedocs.io/en/master/guide/install.html).
 ```bash
 python experiments/dqn_2way-single-intersection.py
 ```
 
 ### Plotting results:
 ```bash
-python outputs/plot.py -f outputs/2way-single-intersection/a3c
+python outputs/plot.py -f outputs/4x4grid/ppo_conn0_ep2
 ```
 <p align="center">
 <img src="outputs/result.png" align="center" width="50%"/>
 </p>
 
 ## Citing
```

### Comparing `sumo-rl-1.4.2/README.md` & `sumo-rl-1.4.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,49 @@
+Metadata-Version: 2.1
+Name: sumo-rl
+Version: 1.4.3
+Summary: RL environments and learning code for traffic signal control in SUMO.
+Author-email: Lucas Alegre <lucasnale@gmail.com>
+License: MIT License
+Project-URL: Homepage, https://lucasalegre.github.io/sumo-rl
+Project-URL: Repository, https://github.com/LucasAlegre/sumo-rl
+Project-URL: Documentation, https://lucasalegre.github.io/sumo-rl
+Project-URL: Bug Report, https://github.com/LucasAlegre/sumo-rl/issues
+Keywords: Reinforcement Learning,Traffic Signal Control,SUMO,RL,PettingZoo,gymnasium
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: rendering
+Provides-Extra: all
+Provides-Extra: testing
+License-File: LICENSE
+
 <img src="docs/_static/logo.png" align="right" width="30%"/>
 
 [![tests](https://github.com/LucasAlegre/sumo-rl/actions/workflows/linux-test.yml/badge.svg)](https://github.com/LucasAlegre/sumo-rl/actions/workflows/linux-test.yml)
 [![PyPI version](https://badge.fury.io/py/sumo-rl.svg)](https://badge.fury.io/py/sumo-rl)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![License](http://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://github.com/LucasAlegre/sumo-rl/blob/master/LICENSE)
+[![License](http://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://github.com/LucasAlegre/sumo-rl/blob/main/LICENSE)
 
 # SUMO-RL
 
 <!-- start intro -->
 
 SUMO-RL provides a simple interface to instantiate Reinforcement Learning (RL) environments with [SUMO](https://github.com/eclipse/sumo) for Traffic Signal Control.
 
 Goals of this repository:
 - Provide a simple interface to work with Reinforcement Learning for Traffic Signal Control using SUMO
 - Support Multiagent RL
-- Compatibility with gymnasium.Env and popular RL libraries such as [stable-baselines3](https://github.com/DLR-RM/stable-baselines3) and [RLlib](https://docs.ray.io/en/master/rllib.html)
+- Compatibility with gymnasium.Env and popular RL libraries such as [stable-baselines3](https://github.com/DLR-RM/stable-baselines3) and [RLlib](https://docs.ray.io/en/main/rllib.html)
 - Easy customisation: state and reward definitions are easily modifiable
 
-The main class is [SumoEnvironment](https://github.com/LucasAlegre/sumo-rl/blob/master/sumo_rl/environment/env.py).
+The main class is [SumoEnvironment](https://github.com/LucasAlegre/sumo-rl/blob/main/sumo_rl/environment/env.py).
 If instantiated with parameter 'single-agent=True', it behaves like a regular [Gymnasium Env](https://github.com/Farama-Foundation/Gymnasium).
-For multiagent environments, use [env](https://github.com/LucasAlegre/sumo-rl/blob/master/sumo_rl/environment/env.py) or [parallel_env](https://github.com/LucasAlegre/sumo-rl/blob/master/sumo_rl/environment/env.py) to instantiate a [PettingZoo](https://github.com/PettingZoo-Team/PettingZoo) environment with AEC or Parallel API, respectively.
-[TrafficSignal](https://github.com/LucasAlegre/sumo-rl/blob/master/sumo_rl/environment/traffic_signal.py) is responsible for retrieving information and actuating on traffic lights using [TraCI](https://sumo.dlr.de/wiki/TraCI) API.
+For multiagent environments, use [env](https://github.com/LucasAlegre/sumo-rl/blob/main/sumo_rl/environment/env.py) or [parallel_env](https://github.com/LucasAlegre/sumo-rl/blob/main/sumo_rl/environment/env.py) to instantiate a [PettingZoo](https://github.com/PettingZoo-Team/PettingZoo) environment with AEC or Parallel API, respectively.
+[TrafficSignal](https://github.com/LucasAlegre/sumo-rl/blob/main/sumo_rl/environment/traffic_signal.py) is responsible for retrieving information and actuating on traffic lights using [TraCI](https://sumo.dlr.de/wiki/TraCI) API.
 
 For more details, check the [documentation online](https://lucasalegre.github.io/sumo-rl/).
 
 <!-- end intro -->
 
 ## Install
 
@@ -76,26 +94,26 @@
     obs = [phase_one_hot, min_green, lane_1_density,...,lane_n_density, lane_1_queue,...,lane_n_queue]
 ```
 - ```phase_one_hot``` is a one-hot encoded vector indicating the current active green phase
 - ```min_green``` is a binary variable indicating whether min_green seconds have already passed in the current phase
 - ```lane_i_density``` is the number of vehicles in incoming lane i dividided by the total capacity of the lane
 - ```lane_i_queue```is the number of queued (speed below 0.1 m/s) vehicles in incoming lane i divided by the total capacity of the lane
 
-You can define your own observation by implementing a class that inherits from [ObservationFunction](https://github.com/LucasAlegre/sumo-rl/blob/master/sumo_rl/environment/observations.py) and passing it to the environment constructor.
+You can define your own observation by implementing a class that inherits from [ObservationFunction](https://github.com/LucasAlegre/sumo-rl/blob/main/sumo_rl/environment/observations.py) and passing it to the environment constructor.
 
 <!-- end observation -->
 
 ### Action
 
 <!-- start action -->
 
 The action space is discrete.
 Every 'delta_time' seconds, each traffic signal agent can choose the next green phase configuration.
 
-E.g.: In the [2-way single intersection](https://github.com/LucasAlegre/sumo-rl/blob/master/experiments/dqn_2way-single-intersection.py) there are |A| = 4 discrete actions, corresponding to the following green phase configurations:
+E.g.: In the [2-way single intersection](https://github.com/LucasAlegre/sumo-rl/blob/main/experiments/dqn_2way-single-intersection.py) there are |A| = 4 discrete actions, corresponding to the following green phase configurations:
 
 <p align="center">
 <img src="docs/_static/actions.png" align="center" width="75%"/>
 </p>
 
 Important: every time a phase change occurs, the next phase is preeceded by a yellow phase lasting ```yellow_time``` seconds.
 
@@ -109,15 +127,15 @@
 
 <p align="center">
 <img src="docs/_static/reward.png" align="center" width="25%"/>
 </p>
 
 That is, the reward is how much the total delay (sum of the waiting times of all approaching vehicles) changed in relation to the previous time-step.
 
-You can choose a different reward function (see the ones implemented in [TrafficSignal](https://github.com/LucasAlegre/sumo-rl/blob/master/sumo_rl/environment/traffic_signal.py)) with the parameter `reward_fn` in the [SumoEnvironment](https://github.com/LucasAlegre/sumo-rl/blob/master/sumo_rl/environment/env.py) constructor.
+You can choose a different reward function (see the ones implemented in [TrafficSignal](https://github.com/LucasAlegre/sumo-rl/blob/main/sumo_rl/environment/traffic_signal.py)) with the parameter `reward_fn` in the [SumoEnvironment](https://github.com/LucasAlegre/sumo-rl/blob/main/sumo_rl/environment/env.py) constructor.
 
 It is also possible to implement your own reward function:
 
 ```python
 def my_reward_fn(traffic_signal):
     return traffic_signal.get_average_speed()
 
@@ -155,58 +173,57 @@
 
 <!-- start pettingzoo -->
 
 For multi-agent environments, you can use the PettingZoo API (see [Petting Zoo API](https://pettingzoo.farama.org/api/parallel/)):
 
 ```python
 import sumo_rl
-env = sumo_rl.parallel_env(net_file='sumo_net_file.net.xml',
-                  route_file='sumo_route_file.rou.xml',
+env = sumo_rl.parallel_env(net_file='nets/RESCO/grid4x4/grid4x4.net.xml',
+                  route_file='nets/RESCO/grid4x4/grid4x4_1.rou.xml',
                   use_gui=True,
                   num_seconds=3600)
+observations = env.reset()
 while env.agents:
-    actions = {agent: parallel_env.action_space(agent).sample() for agent in parallel_env.agents}  # this is where you would insert your policy
-    observations, rewards, terminations, truncations, infos = parallel_env.step(actions)
+    actions = {agent: env.action_space(agent).sample() for agent in env.agents}  # this is where you would insert your policy
+    observations, rewards, terminations, truncations, infos = env.step(actions)
 ```
 
 <!-- end pettingzoo -->
 
 ### RESCO Benchmarks
 
-In the folder [nets/RESCO](https://github.com/LucasAlegre/sumo-rl/tree/master/nets/RESCO) you can find the network and route files from [RESCO](https://github.com/jault/RESCO) (Reinforcement Learning Benchmarks for Traffic Signal Control), which was built on top of SUMO-RL. See their [paper](https://people.engr.tamu.edu/guni/Papers/NeurIPS-signals.pdf) for results.
+In the folder [nets/RESCO](https://github.com/LucasAlegre/sumo-rl/tree/main/nets/RESCO) you can find the network and route files from [RESCO](https://github.com/jault/RESCO) (Reinforcement Learning Benchmarks for Traffic Signal Control), which was built on top of SUMO-RL. See their [paper](https://people.engr.tamu.edu/guni/Papers/NeurIPS-signals.pdf) for results.
 
 <p align="center">
 <img src="nets/RESCO/maps.png" align="center" width="60%"/>
 </p>
 
 ### Experiments
 
-WARNING: Gym 0.26 had many breaking changes, stable-baselines3 and RLlib still do not support it, but will be updated soon. See [Stable Baselines 3 PR](https://github.com/DLR-RM/stable-baselines3/pull/780) and [RLib PR](https://github.com/ray-project/ray/pull/28369).
-Hence, only the tabular Q-learning experiment is running without errors for now.
-
-Check [experiments](https://github.com/LucasAlegre/sumo-rl/tree/master/experiments) for examples on how to instantiate an environment and train your RL agent.
+Check [experiments](https://github.com/LucasAlegre/sumo-rl/tree/main/experiments) for examples on how to instantiate an environment and train your RL agent.
 
-### [Q-learning](https://github.com/LucasAlegre/sumo-rl/blob/master/agents/ql_agent.py) in a one-way single intersection:
+### [Q-learning](https://github.com/LucasAlegre/sumo-rl/blob/main/agents/ql_agent.py) in a one-way single intersection:
 ```bash
 python experiments/ql_single-intersection.py
 ```
 
-### [RLlib A3C](https://github.com/ray-project/ray/tree/master/python/ray/rllib/agents/a3c) multiagent in a 4x4 grid:
+### [RLlib PPO](https://docs.ray.io/en/latest/_modules/ray/rllib/algorithms/ppo/ppo.html) multiagent in a 4x4 grid:
 ```bash
-python experiments/a3c_4x4grid.py
+python experiments/ppo_4x4grid.py
 ```
 
 ### [stable-baselines3 DQN](https://github.com/DLR-RM/stable-baselines3/blob/master/stable_baselines3/dqn/dqn.py) in a 2-way single intersection:
+Obs: you need to install stable-baselines3 with ```pip install "stable_baselines3[extra]>=2.0.0a9"``` for [Gymnasium compatibility](https://stable-baselines3.readthedocs.io/en/master/guide/install.html).
 ```bash
 python experiments/dqn_2way-single-intersection.py
 ```
 
 ### Plotting results:
 ```bash
-python outputs/plot.py -f outputs/2way-single-intersection/a3c
+python outputs/plot.py -f outputs/4x4grid/ppo_conn0_ep2
 ```
 <p align="center">
 <img src="outputs/result.png" align="center" width="50%"/>
 </p>
 
 ## Citing
```

### Comparing `sumo-rl-1.4.2/pyproject.toml` & `sumo-rl-1.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 ]
 
 # Linters and Test tools #######################################################
 
 [tool.black]
 safe = true
 line-length = 127
-target-version = ['py37', 'py38', 'py39', 'py310']
+target-version = ['py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 
 [tool.isort]
 atomic = true
 profile = "black"
 src_paths = ["sumo_rl", "tests", "docs/scripts"]
 extra_standard_library = ["typing_extensions"]
@@ -65,15 +65,15 @@
 
 [tool.pyright]
 include = ["sumo_rl/**", "tests/**"]
 exclude = ["**/node_modules", "**/__pycache__"]
 strict = []
 
 typeCheckingMode = "basic"
-pythonVersion = "3.7"
+pythonVersion = "3.8"
 pythonPlatform = "All"
 typeshedPath = "typeshed"
 enableTypeIgnoreComments = true
 
 # This is required as the CI pre-commit does not download the module (i.e. numpy, pygame)
 #   Therefore, we have to ignore missing imports
 reportMissingImports = "none"
```

### Comparing `sumo-rl-1.4.2/sumo_rl/agents/ql_agent.py` & `sumo-rl-1.4.3/sumo_rl/agents/ql_agent.py`

 * *Files identical despite different names*

### Comparing `sumo-rl-1.4.2/sumo_rl/environment/env.py` & `sumo-rl-1.4.3/sumo_rl/environment/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -527,15 +527,24 @@
         self.env.reset(seed=seed, options=options)
         self.agents = self.possible_agents[:]
         self.agent_selection = self._agent_selector.reset()
         self.rewards = {agent: 0 for agent in self.agents}
         self._cumulative_rewards = {agent: 0 for agent in self.agents}
         self.terminations = {a: False for a in self.agents}
         self.truncations = {a: False for a in self.agents}
-        self.infos = {agent: {} for agent in self.agents}
+        self.compute_info()
+
+    def compute_info(self):
+        """Compute the info for the current step."""
+        self.infos = {a: {} for a in self.agents}
+        infos = self.env._compute_info()
+        for a in self.agents:
+            for k, v in infos.items():
+                if k.startswith(a):
+                    self.infos[a][k] = v
 
     def observation_space(self, agent):
         """Return the observation space for the agent."""
         return self.observation_spaces[agent]
 
     def action_space(self, agent):
         """Return the action space for the agent."""
@@ -546,17 +555,17 @@
         obs = self.env.observations[agent].copy()
         return obs
 
     def close(self):
         """Close the environment and stop the SUMO simulation."""
         self.env.close()
 
-    def render(self, mode="human"):
+    def render(self):
         """Render the environment."""
-        return self.env.render(mode)
+        return self.env.render()
 
     def save_csv(self, out_csv_name, episode):
         """Save metrics of the simulation to a .csv file."""
         self.env.save_csv(out_csv_name, episode)
 
     def step(self, action):
         """Step the environment."""
@@ -571,15 +580,15 @@
 
         self.env._apply_actions({agent: action})
 
         if self._agent_selector.is_last():
             self.env._run_steps()
             self.env._compute_observations()
             self.rewards = self.env._compute_rewards()
-            self.env._compute_info()
+            self.compute_info()
         else:
             self._clear_rewards()
 
         done = self.env._compute_dones()["__all__"]
         self.truncations = {a: done for a in self.agents}
 
         self.agent_selection = self._agent_selector.next()
```

### Comparing `sumo-rl-1.4.2/sumo_rl/environment/observations.py` & `sumo-rl-1.4.3/sumo_rl/environment/observations.py`

 * *Files identical despite different names*

### Comparing `sumo-rl-1.4.2/sumo_rl/environment/resco_envs.py` & `sumo-rl-1.4.3/sumo_rl/environment/resco_envs.py`

 * *Files identical despite different names*

### Comparing `sumo-rl-1.4.2/sumo_rl/environment/traffic_signal.py` & `sumo-rl-1.4.3/sumo_rl/environment/traffic_signal.py`

 * *Files identical despite different names*

### Comparing `sumo-rl-1.4.2/sumo_rl/exploration/epsilon_greedy.py` & `sumo-rl-1.4.3/sumo_rl/exploration/epsilon_greedy.py`

 * *Files identical despite different names*

### Comparing `sumo-rl-1.4.2/sumo_rl/exploration/plot_epsilon.py` & `sumo-rl-1.4.3/sumo_rl/exploration/plot_epsilon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Plot epsilon decay."""
 import argparse
 
 import matplotlib.pyplot as plt
 
 
 if __name__ == "__main__":
-
     prs = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     prs.add_argument("-e", dest="epsilon", type=float, required=True, help="Epsilon\n")
     prs.add_argument("-d", dest="decay", type=float, required=True, help="Epsilon\n")
     args = prs.parse_args()
 
     plt.plot([i for i in range(0, 20000, 5)], [args.epsilon * args.decay**i for i in range(0, 4000)])
```

### Comparing `sumo-rl-1.4.2/sumo_rl/util/gen_route.py` & `sumo-rl-1.4.3/sumo_rl/util/gen_route.py`

 * *Files identical despite different names*

### Comparing `sumo-rl-1.4.2/sumo_rl/util/xml2csv.py` & `sumo-rl-1.4.3/sumo_rl/util/xml2csv.py`

 * *Files identical despite different names*

### Comparing `sumo-rl-1.4.2/sumo_rl/util/xsd.py` & `sumo-rl-1.4.3/sumo_rl/util/xsd.py`

 * *Files identical despite different names*

### Comparing `sumo-rl-1.4.2/sumo_rl.egg-info/PKG-INFO` & `sumo-rl-1.4.3/sumo_rl.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumo-rl
-Version: 1.4.2
+Version: 1.4.3
 Summary: RL environments and learning code for traffic signal control in SUMO.
 Author-email: Lucas Alegre <lucasnale@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://lucasalegre.github.io/sumo-rl
 Project-URL: Repository, https://github.com/LucasAlegre/sumo-rl
 Project-URL: Documentation, https://lucasalegre.github.io/sumo-rl
 Project-URL: Bug Report, https://github.com/LucasAlegre/sumo-rl/issues
@@ -18,32 +18,32 @@
 
 <img src="docs/_static/logo.png" align="right" width="30%"/>
 
 [![tests](https://github.com/LucasAlegre/sumo-rl/actions/workflows/linux-test.yml/badge.svg)](https://github.com/LucasAlegre/sumo-rl/actions/workflows/linux-test.yml)
 [![PyPI version](https://badge.fury.io/py/sumo-rl.svg)](https://badge.fury.io/py/sumo-rl)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![License](http://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://github.com/LucasAlegre/sumo-rl/blob/master/LICENSE)
+[![License](http://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://github.com/LucasAlegre/sumo-rl/blob/main/LICENSE)
 
 # SUMO-RL
 
 <!-- start intro -->
 
 SUMO-RL provides a simple interface to instantiate Reinforcement Learning (RL) environments with [SUMO](https://github.com/eclipse/sumo) for Traffic Signal Control.
 
 Goals of this repository:
 - Provide a simple interface to work with Reinforcement Learning for Traffic Signal Control using SUMO
 - Support Multiagent RL
-- Compatibility with gymnasium.Env and popular RL libraries such as [stable-baselines3](https://github.com/DLR-RM/stable-baselines3) and [RLlib](https://docs.ray.io/en/master/rllib.html)
+- Compatibility with gymnasium.Env and popular RL libraries such as [stable-baselines3](https://github.com/DLR-RM/stable-baselines3) and [RLlib](https://docs.ray.io/en/main/rllib.html)
 - Easy customisation: state and reward definitions are easily modifiable
 
-The main class is [SumoEnvironment](https://github.com/LucasAlegre/sumo-rl/blob/master/sumo_rl/environment/env.py).
+The main class is [SumoEnvironment](https://github.com/LucasAlegre/sumo-rl/blob/main/sumo_rl/environment/env.py).
 If instantiated with parameter 'single-agent=True', it behaves like a regular [Gymnasium Env](https://github.com/Farama-Foundation/Gymnasium).
-For multiagent environments, use [env](https://github.com/LucasAlegre/sumo-rl/blob/master/sumo_rl/environment/env.py) or [parallel_env](https://github.com/LucasAlegre/sumo-rl/blob/master/sumo_rl/environment/env.py) to instantiate a [PettingZoo](https://github.com/PettingZoo-Team/PettingZoo) environment with AEC or Parallel API, respectively.
-[TrafficSignal](https://github.com/LucasAlegre/sumo-rl/blob/master/sumo_rl/environment/traffic_signal.py) is responsible for retrieving information and actuating on traffic lights using [TraCI](https://sumo.dlr.de/wiki/TraCI) API.
+For multiagent environments, use [env](https://github.com/LucasAlegre/sumo-rl/blob/main/sumo_rl/environment/env.py) or [parallel_env](https://github.com/LucasAlegre/sumo-rl/blob/main/sumo_rl/environment/env.py) to instantiate a [PettingZoo](https://github.com/PettingZoo-Team/PettingZoo) environment with AEC or Parallel API, respectively.
+[TrafficSignal](https://github.com/LucasAlegre/sumo-rl/blob/main/sumo_rl/environment/traffic_signal.py) is responsible for retrieving information and actuating on traffic lights using [TraCI](https://sumo.dlr.de/wiki/TraCI) API.
 
 For more details, check the [documentation online](https://lucasalegre.github.io/sumo-rl/).
 
 <!-- end intro -->
 
 ## Install
 
@@ -94,26 +94,26 @@
     obs = [phase_one_hot, min_green, lane_1_density,...,lane_n_density, lane_1_queue,...,lane_n_queue]
 ```
 - ```phase_one_hot``` is a one-hot encoded vector indicating the current active green phase
 - ```min_green``` is a binary variable indicating whether min_green seconds have already passed in the current phase
 - ```lane_i_density``` is the number of vehicles in incoming lane i dividided by the total capacity of the lane
 - ```lane_i_queue```is the number of queued (speed below 0.1 m/s) vehicles in incoming lane i divided by the total capacity of the lane
 
-You can define your own observation by implementing a class that inherits from [ObservationFunction](https://github.com/LucasAlegre/sumo-rl/blob/master/sumo_rl/environment/observations.py) and passing it to the environment constructor.
+You can define your own observation by implementing a class that inherits from [ObservationFunction](https://github.com/LucasAlegre/sumo-rl/blob/main/sumo_rl/environment/observations.py) and passing it to the environment constructor.
 
 <!-- end observation -->
 
 ### Action
 
 <!-- start action -->
 
 The action space is discrete.
 Every 'delta_time' seconds, each traffic signal agent can choose the next green phase configuration.
 
-E.g.: In the [2-way single intersection](https://github.com/LucasAlegre/sumo-rl/blob/master/experiments/dqn_2way-single-intersection.py) there are |A| = 4 discrete actions, corresponding to the following green phase configurations:
+E.g.: In the [2-way single intersection](https://github.com/LucasAlegre/sumo-rl/blob/main/experiments/dqn_2way-single-intersection.py) there are |A| = 4 discrete actions, corresponding to the following green phase configurations:
 
 <p align="center">
 <img src="docs/_static/actions.png" align="center" width="75%"/>
 </p>
 
 Important: every time a phase change occurs, the next phase is preeceded by a yellow phase lasting ```yellow_time``` seconds.
 
@@ -127,15 +127,15 @@
 
 <p align="center">
 <img src="docs/_static/reward.png" align="center" width="25%"/>
 </p>
 
 That is, the reward is how much the total delay (sum of the waiting times of all approaching vehicles) changed in relation to the previous time-step.
 
-You can choose a different reward function (see the ones implemented in [TrafficSignal](https://github.com/LucasAlegre/sumo-rl/blob/master/sumo_rl/environment/traffic_signal.py)) with the parameter `reward_fn` in the [SumoEnvironment](https://github.com/LucasAlegre/sumo-rl/blob/master/sumo_rl/environment/env.py) constructor.
+You can choose a different reward function (see the ones implemented in [TrafficSignal](https://github.com/LucasAlegre/sumo-rl/blob/main/sumo_rl/environment/traffic_signal.py)) with the parameter `reward_fn` in the [SumoEnvironment](https://github.com/LucasAlegre/sumo-rl/blob/main/sumo_rl/environment/env.py) constructor.
 
 It is also possible to implement your own reward function:
 
 ```python
 def my_reward_fn(traffic_signal):
     return traffic_signal.get_average_speed()
 
@@ -173,58 +173,57 @@
 
 <!-- start pettingzoo -->
 
 For multi-agent environments, you can use the PettingZoo API (see [Petting Zoo API](https://pettingzoo.farama.org/api/parallel/)):
 
 ```python
 import sumo_rl
-env = sumo_rl.parallel_env(net_file='sumo_net_file.net.xml',
-                  route_file='sumo_route_file.rou.xml',
+env = sumo_rl.parallel_env(net_file='nets/RESCO/grid4x4/grid4x4.net.xml',
+                  route_file='nets/RESCO/grid4x4/grid4x4_1.rou.xml',
                   use_gui=True,
                   num_seconds=3600)
+observations = env.reset()
 while env.agents:
-    actions = {agent: parallel_env.action_space(agent).sample() for agent in parallel_env.agents}  # this is where you would insert your policy
-    observations, rewards, terminations, truncations, infos = parallel_env.step(actions)
+    actions = {agent: env.action_space(agent).sample() for agent in env.agents}  # this is where you would insert your policy
+    observations, rewards, terminations, truncations, infos = env.step(actions)
 ```
 
 <!-- end pettingzoo -->
 
 ### RESCO Benchmarks
 
-In the folder [nets/RESCO](https://github.com/LucasAlegre/sumo-rl/tree/master/nets/RESCO) you can find the network and route files from [RESCO](https://github.com/jault/RESCO) (Reinforcement Learning Benchmarks for Traffic Signal Control), which was built on top of SUMO-RL. See their [paper](https://people.engr.tamu.edu/guni/Papers/NeurIPS-signals.pdf) for results.
+In the folder [nets/RESCO](https://github.com/LucasAlegre/sumo-rl/tree/main/nets/RESCO) you can find the network and route files from [RESCO](https://github.com/jault/RESCO) (Reinforcement Learning Benchmarks for Traffic Signal Control), which was built on top of SUMO-RL. See their [paper](https://people.engr.tamu.edu/guni/Papers/NeurIPS-signals.pdf) for results.
 
 <p align="center">
 <img src="nets/RESCO/maps.png" align="center" width="60%"/>
 </p>
 
 ### Experiments
 
-WARNING: Gym 0.26 had many breaking changes, stable-baselines3 and RLlib still do not support it, but will be updated soon. See [Stable Baselines 3 PR](https://github.com/DLR-RM/stable-baselines3/pull/780) and [RLib PR](https://github.com/ray-project/ray/pull/28369).
-Hence, only the tabular Q-learning experiment is running without errors for now.
+Check [experiments](https://github.com/LucasAlegre/sumo-rl/tree/main/experiments) for examples on how to instantiate an environment and train your RL agent.
 
-Check [experiments](https://github.com/LucasAlegre/sumo-rl/tree/master/experiments) for examples on how to instantiate an environment and train your RL agent.
-
-### [Q-learning](https://github.com/LucasAlegre/sumo-rl/blob/master/agents/ql_agent.py) in a one-way single intersection:
+### [Q-learning](https://github.com/LucasAlegre/sumo-rl/blob/main/agents/ql_agent.py) in a one-way single intersection:
 ```bash
 python experiments/ql_single-intersection.py
 ```
 
-### [RLlib A3C](https://github.com/ray-project/ray/tree/master/python/ray/rllib/agents/a3c) multiagent in a 4x4 grid:
+### [RLlib PPO](https://docs.ray.io/en/latest/_modules/ray/rllib/algorithms/ppo/ppo.html) multiagent in a 4x4 grid:
 ```bash
-python experiments/a3c_4x4grid.py
+python experiments/ppo_4x4grid.py
 ```
 
 ### [stable-baselines3 DQN](https://github.com/DLR-RM/stable-baselines3/blob/master/stable_baselines3/dqn/dqn.py) in a 2-way single intersection:
+Obs: you need to install stable-baselines3 with ```pip install "stable_baselines3[extra]>=2.0.0a9"``` for [Gymnasium compatibility](https://stable-baselines3.readthedocs.io/en/master/guide/install.html).
 ```bash
 python experiments/dqn_2way-single-intersection.py
 ```
 
 ### Plotting results:
 ```bash
-python outputs/plot.py -f outputs/2way-single-intersection/a3c
+python outputs/plot.py -f outputs/4x4grid/ppo_conn0_ep2
 ```
 <p align="center">
 <img src="outputs/result.png" align="center" width="50%"/>
 </p>
 
 ## Citing
```

### Comparing `sumo-rl-1.4.2/sumo_rl.egg-info/SOURCES.txt` & `sumo-rl-1.4.3/sumo_rl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

