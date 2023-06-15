# Comparing `tmp/jax-sgmc-0.1.1.tar.gz` & `tmp/jax-sgmc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax-sgmc-0.1.1.tar", last modified: Thu Jan  5 10:52:31 2023, max compression
+gzip compressed data, was "jax-sgmc-0.1.3.tar", last modified: Thu Jun 15 07:10:07 2023, max compression
```

## Comparing `jax-sgmc-0.1.1.tar` & `jax-sgmc-0.1.3.tar`

### file list

```diff
@@ -1,35 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 10:52:31.439511 jax-sgmc-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-05 10:52:21.000000 jax-sgmc-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-01-05 10:52:21.000000 jax-sgmc-0.1.1/LICENSE_SHORT
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-01-05 10:52:31.439511 jax-sgmc-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-01-05 10:52:21.000000 jax-sgmc-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 10:52:31.435511 jax-sgmc-0.1.1/jax_sgmc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 10:52:21.000000 jax-sgmc-0.1.1/jax_sgmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-01-05 10:52:21.000000 jax-sgmc-0.1.1/jax_sgmc/adaption.py
--rw-r--r--   0 runner    (1001) docker     (123)    23805 2023-01-05 10:52:21.000000 jax-sgmc-0.1.1/jax_sgmc/alias.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 10:52:31.435511 jax-sgmc-0.1.1/jax_sgmc/data/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-01-05 10:52:21.000000 jax-sgmc-0.1.1/jax_sgmc/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38795 2023-01-05 10:52:21.000000 jax-sgmc-0.1.1/jax_sgmc/data/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-01-05 10:52:21.000000 jax-sgmc-0.1.1/jax_sgmc/data/hdf5_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    16112 2023-01-05 10:52:21.000000 jax-sgmc-0.1.1/jax_sgmc/data/numpy_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-01-05 10:52:21.000000 jax-sgmc-0.1.1/jax_sgmc/data/tensorflow_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    29127 2023-01-05 10:52:21.000000 jax-sgmc-0.1.1/jax_sgmc/integrator.py
--rw-r--r--   0 runner    (1001) docker     (123)    29093 2023-01-05 10:52:21.000000 jax-sgmc-0.1.1/jax_sgmc/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-01-05 10:52:21.000000 jax-sgmc-0.1.1/jax_sgmc/potential.py
--rw-r--r--   0 runner    (1001) docker     (123)    22367 2023-01-05 10:52:21.000000 jax-sgmc-0.1.1/jax_sgmc/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19501 2023-01-05 10:52:21.000000 jax-sgmc-0.1.1/jax_sgmc/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 10:52:31.439511 jax-sgmc-0.1.1/jax_sgmc/util/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-01-05 10:52:21.000000 jax-sgmc-0.1.1/jax_sgmc/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-01-05 10:52:21.000000 jax-sgmc-0.1.1/jax_sgmc/util/list_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-05 10:52:21.000000 jax-sgmc-0.1.1/jax_sgmc/util/stop_vmap.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-01-05 10:52:21.000000 jax-sgmc-0.1.1/jax_sgmc/util/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-01-05 10:52:21.000000 jax-sgmc-0.1.1/jax_sgmc/util/tree_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-01-05 10:52:21.000000 jax-sgmc-0.1.1/jax_sgmc/util/uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 10:52:31.435511 jax-sgmc-0.1.1/jax_sgmc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-01-05 10:52:31.000000 jax-sgmc-0.1.1/jax_sgmc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-01-05 10:52:31.000000 jax-sgmc-0.1.1/jax_sgmc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 10:52:31.000000 jax-sgmc-0.1.1/jax_sgmc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-01-05 10:52:31.000000 jax-sgmc-0.1.1/jax_sgmc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-05 10:52:31.000000 jax-sgmc-0.1.1/jax_sgmc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-01-05 10:52:21.000000 jax-sgmc-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-05 10:52:31.439511 jax-sgmc-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:10:07.584935 jax-sgmc-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/LICENSE_SHORT
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-15 07:10:07.584935 jax-sgmc-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:10:07.580935 jax-sgmc-0.1.3/jax_sgmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/jax_sgmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/jax_sgmc/adaption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23805 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/jax_sgmc/alias.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:10:07.580935 jax-sgmc-0.1.3/jax_sgmc/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/jax_sgmc/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39015 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/jax_sgmc/data/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/jax_sgmc/data/hdf5_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16112 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/jax_sgmc/data/numpy_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/jax_sgmc/data/tensorflow_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29127 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/jax_sgmc/integrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29093 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/jax_sgmc/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/jax_sgmc/potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22367 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/jax_sgmc/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19501 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/jax_sgmc/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:10:07.580935 jax-sgmc-0.1.3/jax_sgmc/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/jax_sgmc/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/jax_sgmc/util/list_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/jax_sgmc/util/stop_vmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/jax_sgmc/util/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/jax_sgmc/util/tree_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/jax_sgmc/util/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/jax_sgmc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:10:07.580935 jax-sgmc-0.1.3/jax_sgmc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-15 07:10:07.000000 jax-sgmc-0.1.3/jax_sgmc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-15 07:10:07.000000 jax-sgmc-0.1.3/jax_sgmc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:10:07.000000 jax-sgmc-0.1.3/jax_sgmc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-15 07:10:07.000000 jax-sgmc-0.1.3/jax_sgmc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 07:10:07.000000 jax-sgmc-0.1.3/jax_sgmc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 07:10:07.584935 jax-sgmc-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:10:07.584935 jax-sgmc-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/tests/test_adaption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/tests/test_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35860 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14047 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/tests/test_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-15 07:09:41.000000 jax-sgmc-0.1.3/tests/test_tree_operations.py
```

### Comparing `jax-sgmc-0.1.1/LICENSE` & `jax-sgmc-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jax-sgmc-0.1.1/LICENSE_SHORT` & `jax-sgmc-0.1.3/LICENSE_SHORT`

 * *Files identical despite different names*

### Comparing `jax-sgmc-0.1.1/PKG-INFO` & `jax-sgmc-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-sgmc
-Version: 0.1.1
+Version: 0.1.3
 Summary: Stochastic Gradient Monte Carlo in Jax
 Author-email: Paul Fuchs <paul.fuchs@tum.de>, Stephan Thaler <stephan.thaler@tum.de>
 License: Apache-2.0
 Project-URL: Documentation, https://jax-sgmc.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/tummfm/jax-sgmc
 Project-URL: Bug Tracker, https://github.com/tummfm/jax-sgmc/issues
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `jax-sgmc-0.1.1/README.md` & `jax-sgmc-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `jax-sgmc-0.1.1/jax_sgmc/adaption.py` & `jax-sgmc-0.1.3/jax_sgmc/adaption.py`

 * *Files identical despite different names*

### Comparing `jax-sgmc-0.1.1/jax_sgmc/alias.py` & `jax-sgmc-0.1.3/jax_sgmc/alias.py`

 * *Files identical despite different names*

### Comparing `jax-sgmc-0.1.1/jax_sgmc/data/__init__.py` & `jax-sgmc-0.1.3/jax_sgmc/data/__init__.py`

 * *Files identical despite different names*

### Comparing `jax-sgmc-0.1.1/jax_sgmc/data/core.py` & `jax-sgmc-0.1.3/jax_sgmc/data/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -411,15 +411,15 @@
     self._host_data_loaders: Dict[Any, HostDataLoader] = {}
 
     self._lock = threading.Lock()
 
   def __call__(self,
                chain_id: int,
                token: JaxUUID,
-               device: jax.xla.Device,
+               device: jax.Device,
                callback_uuid: JaxUUID,
                device_count: int = 1,
                strict: bool = False):
     with self._lock:
       if callback_uuid.as_uuid not in self._requests.keys():
         self._requests[callback_uuid.as_uuid] = {}
 
@@ -677,20 +677,23 @@
 
   # The definition requires passing an argument to the host function. The shape
   # of the returned data must be known before the first call. The chain id
   # determines whether the data is collected randomly or sequentially.
 
   def get_data(req, device):
     chain_id, callback_uuid, token, device_count = req
+    # The data request class takes care of assigning the request to the right
+    # data loader and verifies it.
     (new_data, mask), new_token = _data_requests(
       chain_id, token, device, callback_uuid, device_count,
       strict=verify_calls)
     if mask is None:
-      # Assume all samples to be valid
-      mask = jnp.ones(mask_shape, dtype=jnp.bool_)
+      # Assume all samples to be valid. It is important to perform the creation
+      # of the array on the host, as otherwise a deadlock will occur.
+      mask = onp.ones(mask_shape, dtype=jnp.bool_)
     return new_data, mask, new_token
 
   def _new_cache_fn(req: Tuple[CacheState, int]) -> CacheState:
     """This function is called if the cache must be refreshed."""
     state, device_count = req
     new_data, masks, token = hcb.call(
       get_data,
```

### Comparing `jax-sgmc-0.1.1/jax_sgmc/data/hdf5_loader.py` & `jax-sgmc-0.1.3/jax_sgmc/data/hdf5_loader.py`

 * *Files identical despite different names*

### Comparing `jax-sgmc-0.1.1/jax_sgmc/data/numpy_loader.py` & `jax-sgmc-0.1.3/jax_sgmc/data/numpy_loader.py`

 * *Files identical despite different names*

### Comparing `jax-sgmc-0.1.1/jax_sgmc/data/tensorflow_loader.py` & `jax-sgmc-0.1.3/jax_sgmc/data/tensorflow_loader.py`

 * *Files identical despite different names*

### Comparing `jax-sgmc-0.1.1/jax_sgmc/integrator.py` & `jax-sgmc-0.1.3/jax_sgmc/integrator.py`

 * *Files identical despite different names*

### Comparing `jax-sgmc-0.1.1/jax_sgmc/io.py` & `jax-sgmc-0.1.3/jax_sgmc/io.py`

 * *Files identical despite different names*

### Comparing `jax-sgmc-0.1.1/jax_sgmc/potential.py` & `jax-sgmc-0.1.3/jax_sgmc/potential.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,15 +91,16 @@
 
 # Todo: Possibly support soft-vmap (numpyro)
 
 def minibatch_potential(prior: Prior,
                         likelihood: Callable,
                         strategy: AnyStr = "map",
                         has_state: bool = False,
-                        is_batched: bool = False) -> StochasticPotential:
+                        is_batched: bool = False,
+                        temperature: float = 1.) -> StochasticPotential:
   """Initializes the potential function for a minibatch of data.
 
   Args:
     prior: Log-prior function which is evaluated for a single
       sample.
     likelihood: Log-likelihood function. If ``has_state = True``, then the
       first argument is the model state, otherwise the arguments are ``sample,
@@ -111,14 +112,15 @@
       - ``'vmap'`` parallel evaluation via vectorization
       - ``'pmap'`` parallel evaluation on multiple devices
 
     has_state: If an additional state is provided for the model evaluation
     is_batched: If likelihood expects a batch of observations instead of a
       single observation. If the likelihood is batched, choosing the strategy
       has no influence on the computation.
+    temperature: Posterior temperature. T = 1 is the Bayesian posterior.
 
   Returns:
     Returns a function which evaluates the stochastic potential for a mini-batch
     of data. The first argument are the latent variables and the second is the
     mini-batch.
   """
 
@@ -201,27 +203,29 @@
       state, sample, reference_data, mask)
 
     # The prior has to be evaluated only once, therefore the extra call
     prior_value = prior(sample)
 
     if likelihoods:
       return (
-        jnp.squeeze(batch_likelihood - prior_value),
+        jnp.squeeze(batch_likelihood - prior_value) / temperature,
         (observation_likelihoods, new_state))
     else:
-      return jnp.squeeze(batch_likelihood - prior_value), new_state
+      return (jnp.squeeze(batch_likelihood - prior_value) / temperature,
+              new_state)
 
   return potential_function
 
 
 def full_potential(prior: Callable[[PyTree], Array],
                    likelihood: Callable[[PyTree, PyTree], Array],
                    strategy: AnyStr = "map",
-                   has_state = False,
-                   is_batched = False
+                   has_state: bool = False,
+                   is_batched: bool = False,
+                   temperature: float = 1.,
                    ) -> FullPotential:
   """Transforms a pdf to compute the full potential over all reference data.
 
   Args:
     prior: Log-prior function which is evaluated for a single
       sample.
     likelihood: Log-likelihood function. If ``has_state = True``, then the
@@ -236,14 +240,15 @@
 
     has_state: If an additional state is provided for the model evaluation
     is_batched: If likelihood expects a batch of observations instead of a
       single observation. If the likelihood is batched, choosing the strategy
       has no influence on the computation. In this case, the last argument of
       the likelihood should be an optional mask. The mask is an arrays with ones
       for valid observations and zeros for non-valid observations.
+    temperature: Posterior temperature. T = 1 is the Bayesian posterior.
 
   Returns:
     Returns a function which evaluates the potential over the full dataset via
     a dataset mapping from the :mod:`jax_sgmc.data` module.
 
   """
   assert strategy != 'pmap', "Pmap is currently not supported"
@@ -278,10 +283,11 @@
     else:
       data_state, (results, new_state) = full_data_map_fn(
         body_fn, data_state, state, masking=True, information=True)
 
     # The prior needs just a single evaluation
     prior_eval = prior(sample)
 
-    return jnp.squeeze(jnp.sum(results) - prior_eval), (data_state, new_state)
+    return (jnp.squeeze(jnp.sum(results) - prior_eval) / temperature,
+            (data_state, new_state))
 
   return sum_batched_evaluations
```

### Comparing `jax-sgmc-0.1.1/jax_sgmc/scheduler.py` & `jax-sgmc-0.1.3/jax_sgmc/scheduler.py`

 * *Files identical despite different names*

### Comparing `jax-sgmc-0.1.1/jax_sgmc/solver.py` & `jax-sgmc-0.1.3/jax_sgmc/solver.py`

 * *Files identical despite different names*

### Comparing `jax-sgmc-0.1.1/jax_sgmc/util/list_map.py` & `jax-sgmc-0.1.3/jax_sgmc/util/list_map.py`

 * *Files identical despite different names*

### Comparing `jax-sgmc-0.1.1/jax_sgmc/util/tree_util.py` & `jax-sgmc-0.1.3/jax_sgmc/util/tree_util.py`

 * *Files identical despite different names*

### Comparing `jax-sgmc-0.1.1/jax_sgmc/util/uuid.py` & `jax-sgmc-0.1.3/jax_sgmc/util/uuid.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,25 +10,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import uuid
 
+import numpy as onp
+
 import jax.numpy as jnp
 from jax import tree_util
 
+from jax import Array
+
 @tree_util.register_pytree_node_class
 class JaxUUID:
 
-  def __init__(self, ints: jnp.array = None):
+  def __init__(self, ints: Array = None):
     if ints is None:
       uuid_int = uuid.uuid4().int
       ints = [(uuid_int >> bits) & 0xFFFFFFFF for bits in range(0, 128, 32)]
-      ints = jnp.array(ints, dtype=jnp.int32)
+      ints = onp.array(ints, dtype=jnp.int32)
 
     self._uuid_int = ints
 
   @property
   def as_uuid(self):
     # Rearrange 4 int32 to uuid
     shifted_ints = [int(int(sint) << bits)
@@ -43,12 +47,16 @@
     return str(self.as_uuid)
 
   @property
   def as_int32s(self):
     return self._uuid_int
 
   def tree_flatten(self):
-    return (self._uuid_int, None)
+    # Wrapping the ints in a tuple ensures that they remain a single array of
+    # length 4.
+    children = (self._uuid_int,)
+    return (children, None)
 
   @classmethod
   def tree_unflatten(cls, _, children):
-    return cls(ints=children)
+    ints, = children
+    return cls(ints=ints)
```

### Comparing `jax-sgmc-0.1.1/jax_sgmc.egg-info/PKG-INFO` & `jax-sgmc-0.1.3/jax_sgmc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-sgmc
-Version: 0.1.1
+Version: 0.1.3
 Summary: Stochastic Gradient Monte Carlo in Jax
 Author-email: Paul Fuchs <paul.fuchs@tum.de>, Stephan Thaler <stephan.thaler@tum.de>
 License: Apache-2.0
 Project-URL: Documentation, https://jax-sgmc.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/tummfm/jax-sgmc
 Project-URL: Bug Tracker, https://github.com/tummfm/jax-sgmc/issues
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `jax-sgmc-0.1.1/jax_sgmc.egg-info/SOURCES.txt` & `jax-sgmc-0.1.3/jax_sgmc.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 jax_sgmc/adaption.py
 jax_sgmc/alias.py
 jax_sgmc/integrator.py
 jax_sgmc/io.py
 jax_sgmc/potential.py
 jax_sgmc/scheduler.py
 jax_sgmc/solver.py
+jax_sgmc/version.py
 jax_sgmc.egg-info/PKG-INFO
 jax_sgmc.egg-info/SOURCES.txt
 jax_sgmc.egg-info/dependency_links.txt
 jax_sgmc.egg-info/requires.txt
 jax_sgmc.egg-info/top_level.txt
 jax_sgmc/data/__init__.py
 jax_sgmc/data/core.py
@@ -21,8 +22,15 @@
 jax_sgmc/data/numpy_loader.py
 jax_sgmc/data/tensorflow_loader.py
 jax_sgmc/util/__init__.py
 jax_sgmc/util/list_map.py
 jax_sgmc/util/stop_vmap.py
 jax_sgmc/util/testing.py
 jax_sgmc/util/tree_util.py
-jax_sgmc/util/uuid.py
+jax_sgmc/util/uuid.py
+tests/test_adaption.py
+tests/test_alias.py
+tests/test_data.py
+tests/test_io.py
+tests/test_potential.py
+tests/test_scheduler.py
+tests/test_tree_operations.py
```

### Comparing `jax-sgmc-0.1.1/pyproject.toml` & `jax-sgmc-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [build-system]
 requires = ["setuptools>=61"]   # PEP 508 specifications.
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jax-sgmc"
-version = "0.1.1"
 authors = [
     {name = "Paul Fuchs", email = "paul.fuchs@tum.de"},
     {name = "Stephan Thaler", email = "stephan.thaler@tum.de"},
 ]
 description = "Stochastic Gradient Monte Carlo in Jax"
 readme = "README.md"
 license = {"text" = "Apache-2.0"}
@@ -25,14 +24,15 @@
 requires-python = ">=3.7"
 dependencies = [
     "numpy",
     "jax >= 0.1.73",
     "jaxlib >= 0.1.52",
     "dataclasses",
 ]
+dynamic = ["version"]
 
 [project.urls]
 "Documentation" = "https://jax-sgmc.readthedocs.io/en/latest/"
 "Source" = "https://github.com/tummfm/jax-sgmc"
 "Bug Tracker" = "https://github.com/tummfm/jax-sgmc/issues"
 
 [project.optional-dependencies]
@@ -55,7 +55,10 @@
     "h5py",
     "tensorflow",
     "tensorflow_datasets"
 ]
 
 [tool.setuptools.packages]
 find = {namespaces = false}
+
+[tool.setuptools.dynamic]
+version = {attr = "jax_sgmc.version.__version__"}
```

