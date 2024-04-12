# Comparing `tmp/kulprit-0.0.1.tar.gz` & `tmp/kulprit-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kulprit-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "kulprit-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `kulprit-0.0.1.tar` & `kulprit-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0      543 2023-10-10 18:49:54.346175 kulprit-0.0.1/README.md
--rw-r--r--   0        0        0      221 2023-10-10 18:49:54.350175 kulprit-0.0.1/kulprit/__init__.py
--rw-r--r--   0        0        0       35 2023-10-10 18:49:54.350175 kulprit-0.0.1/kulprit/data/__init__.py
--rw-r--r--   0        0        0     1048 2023-10-10 18:49:54.350175 kulprit-0.0.1/kulprit/data/submodel.py
--rw-r--r--   0        0        0     1783 2023-10-10 18:49:54.350175 kulprit-0.0.1/kulprit/datasets.py
--rw-r--r--   0        0        0       94 2023-10-10 18:49:54.350175 kulprit-0.0.1/kulprit/plots/__init__.py
--rw-r--r--   0        0        0     5009 2023-10-10 18:49:54.350175 kulprit-0.0.1/kulprit/plots/plots.py
--rw-r--r--   0        0        0       35 2023-10-10 18:49:54.350175 kulprit-0.0.1/kulprit/projection/__init__.py
--rw-r--r--   0        0        0     2289 2023-10-10 18:49:54.350175 kulprit-0.0.1/kulprit/projection/likelihood.py
--rw-r--r--   0        0        0     9795 2023-10-10 18:49:54.350175 kulprit-0.0.1/kulprit/projection/projector.py
--rw-r--r--   0        0        0     9859 2023-10-10 18:49:54.350175 kulprit-0.0.1/kulprit/projection/solver.py
--rw-r--r--   0        0        0    12024 2023-10-10 18:49:54.350175 kulprit-0.0.1/kulprit/reference.py
--rw-r--r--   0        0        0      230 2023-10-10 18:49:54.350175 kulprit-0.0.1/kulprit/search/__init__.py
--rw-r--r--   0        0        0     4052 2023-10-10 18:49:54.350175 kulprit-0.0.1/kulprit/search/forward.py
--rw-r--r--   0        0        0     4952 2023-10-10 18:49:54.350175 kulprit-0.0.1/kulprit/search/l1.py
--rw-r--r--   0        0        0     2282 2023-10-10 18:49:54.350175 kulprit-0.0.1/kulprit/search/searcher.py
--rw-r--r--   0        0        0     1326 2023-10-10 18:49:54.350175 kulprit-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1496 1970-01-01 00:00:00.000000 kulprit-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3320 2024-04-12 15:22:06.045039 kulprit-0.1.0/README.md
+-rw-r--r--   0        0        0      221 2024-04-12 15:22:06.045039 kulprit-0.1.0/kulprit/__init__.py
+-rw-r--r--   0        0        0       35 2024-04-12 15:22:06.045039 kulprit-0.1.0/kulprit/data/__init__.py
+-rw-r--r--   0        0        0     1048 2024-04-12 15:22:06.045039 kulprit-0.1.0/kulprit/data/submodel.py
+-rw-r--r--   0        0        0     1783 2024-04-12 15:22:06.045039 kulprit-0.1.0/kulprit/datasets.py
+-rw-r--r--   0        0        0       94 2024-04-12 15:22:06.045039 kulprit-0.1.0/kulprit/plots/__init__.py
+-rw-r--r--   0        0        0     5009 2024-04-12 15:22:06.045039 kulprit-0.1.0/kulprit/plots/plots.py
+-rw-r--r--   0        0        0       35 2024-04-12 15:22:06.045039 kulprit-0.1.0/kulprit/projection/__init__.py
+-rw-r--r--   0        0        0     9795 2024-04-12 15:22:06.045039 kulprit-0.1.0/kulprit/projection/projector.py
+-rw-r--r--   0        0        0     9199 2024-04-12 15:22:06.045039 kulprit-0.1.0/kulprit/projection/solver.py
+-rw-r--r--   0        0        0    12024 2024-04-12 15:22:06.045039 kulprit-0.1.0/kulprit/reference.py
+-rw-r--r--   0        0        0      230 2024-04-12 15:22:06.045039 kulprit-0.1.0/kulprit/search/__init__.py
+-rw-r--r--   0        0        0     4052 2024-04-12 15:22:06.045039 kulprit-0.1.0/kulprit/search/forward.py
+-rw-r--r--   0        0        0     4952 2024-04-12 15:22:06.045039 kulprit-0.1.0/kulprit/search/l1.py
+-rw-r--r--   0        0        0     2282 2024-04-12 15:22:06.045039 kulprit-0.1.0/kulprit/search/searcher.py
+-rw-r--r--   0        0        0     1367 2024-04-12 15:22:06.045039 kulprit-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4331 1970-01-01 00:00:00.000000 kulprit-0.1.0/PKG-INFO
```

### Comparing `kulprit-0.0.1/kulprit/data/submodel.py` & `kulprit-0.1.0/kulprit/data/submodel.py`

 * *Files identical despite different names*

### Comparing `kulprit-0.0.1/kulprit/datasets.py` & `kulprit-0.1.0/kulprit/datasets.py`

 * *Files identical despite different names*

### Comparing `kulprit-0.0.1/kulprit/plots/plots.py` & `kulprit-0.1.0/kulprit/plots/plots.py`

 * *Files identical despite different names*

### Comparing `kulprit-0.0.1/kulprit/projection/projector.py` & `kulprit-0.1.0/kulprit/projection/projector.py`

 * *Files identical despite different names*

### Comparing `kulprit-0.0.1/kulprit/projection/solver.py` & `kulprit-0.1.0/kulprit/projection/solver.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """optimization module."""
 
+# pylint: disable=protected-access
 from typing import List, Optional
 import warnings
 
 import arviz as az
 import bambi as bmb
 import numpy as np
 import xarray as xr
+import preliz as pz
 
 from scipy.optimize import minimize
 
 from kulprit.data.submodel import SubModel
-from kulprit.projection.likelihood import LIKELIHOODS
 
 
 class Solver:
     """The primary solver class, used to perform the projection."""
 
     def __init__(
         self,
@@ -32,19 +33,16 @@
         self.response_name = self.ref_model.response_name
         self.ref_family = self.ref_model.family.name
 
         # define sampling options
         self.num_chain = self.ref_idata.posterior.dims["chain"]
         self.num_samples = self.num_chain * 100
 
-        try:
-            # define the negative log likelihood function of the submodel
-            self.neg_log_likelihood = LIKELIHOODS[self.ref_family]
-        except KeyError:
-            raise NotImplementedError from None
+        if self.ref_family not in ["gaussian", "poisson", "bernoulli", "binomial"]:
+            raise NotImplementedError(f"Family {self.ref_family} not supported")
 
     @property
     def pps(self):
         # make in-sample predictions with the reference model if not available
         if "posterior_predictive" not in self.ref_idata.groups():
             self.ref_model.predict(self.ref_idata, kind="pps", inplace=True)
 
@@ -111,36 +109,37 @@
             float: The negative log-likelihood of the reference posterior predictive under the
         restricted model
         """
 
         # Gaussian observation likelihood
         if self.ref_family == "gaussian":
             linear_predictor = _linear_predict(beta_x=params[:-1], X=X)
-            neg_llk = self.neg_log_likelihood(points=obs, mean=linear_predictor, sigma=params[-1])
+            neg_llk = pz.Normal(mu=linear_predictor, sigma=params[-1])._neg_logpdf(obs)
 
         # Binomial observation likelihood
         elif self.ref_family == "binomial":
             trials = self.ref_model.response.data[:, 1]
             linear_predictor = _linear_predict(beta_x=params, X=X)
             probs = self.ref_model.family.link["p"].linkinv(linear_predictor)
-            neg_llk = self.neg_log_likelihood(points=obs, probs=probs, trials=trials)
+            neg_llk = pz.Binomial(n=trials, p=probs)._neg_logpdf(obs)
 
         # Bernoulli observation likelihood
         elif self.ref_family == "bernoulli":
             linear_predictor = _linear_predict(beta_x=params, X=X)
             probs = self.ref_model.family.link["p"].linkinv(linear_predictor)
-            neg_llk = self.neg_log_likelihood(points=obs, probs=probs)
+            neg_llk = pz.Binomial(p=probs)._neg_logpdf(obs)
 
         # Poisson observation likelihood
         elif self.ref_family == "poisson":
             with warnings.catch_warnings():
                 warnings.filterwarnings("ignore", message="overflow encountered in exp")
                 linear_predictor = _linear_predict(beta_x=params, X=X)
                 lam = self.ref_model.family.link["mu"].linkinv(np.float64(linear_predictor))
-                neg_llk = self.neg_log_likelihood(points=obs, lam=lam)
+                neg_llk = pz.Poisson(mu=lam)._neg_logpdf(obs)
+
         return neg_llk
 
     def solve(self, term_names: List[str], X: np.ndarray, slices: dict) -> SubModel:
         """The primary projection method in the procedure.
 
         The projection is performed with a mean-field approximation rather than concatenating
         posterior draw-wise optimization solutions as is suggested by Piironen (2018).
@@ -156,42 +155,29 @@
             Slices of the common term design matrix
 
         Returns:
         -------
             SubModel: The projected submodel object
         """
         # build the optimization parameter bounds
-        init = np.hstack(
-            [self.ref_idata.posterior.mean(["chain", "draw"])[term].values for term in term_names]
-        )
-        bounds = self._build_bounds(init)
+        term_values = az.extract(self.ref_idata.posterior, num_samples=self.pps.shape[0])
+        init = np.stack([term_values[key].values.flatten() for key in term_names]).T
+        bounds = self._build_bounds(init[0])
 
-        # perform mean-field variational projection predictive inference
+        # perform projection predictive inference
         res_posterior = []
         objectives = []
 
-        chains = np.random.randint(0, self.ref_idata.posterior.dims["chain"], self.pps.shape[0])
-        draws = np.random.randint(0, self.ref_idata.posterior.dims["draw"], self.pps.shape[0])
-
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", message="Values in x were outside bounds")
             for idx, obs in enumerate(self.pps):
-                # use samples from reference model posterior as initial guess
-                init = np.hstack(
-                    [
-                        self.ref_idata.posterior.sel({"chain": chains[idx], "draw": draws[idx]})[
-                            term
-                        ].values
-                        for term in term_names
-                    ]
-                )
                 opt = minimize(
                     self.objective,
                     args=(obs, X),
-                    x0=init,
+                    x0=init[idx],
                     tol=0.001,
                     bounds=bounds,
                     method="SLSQP",
                 )
                 res_posterior.append(opt.x)
                 objectives.append(opt.fun)
```

### Comparing `kulprit-0.0.1/kulprit/reference.py` & `kulprit-0.1.0/kulprit/reference.py`

 * *Files identical despite different names*

### Comparing `kulprit-0.0.1/kulprit/search/forward.py` & `kulprit-0.1.0/kulprit/search/forward.py`

 * *Files identical despite different names*

### Comparing `kulprit-0.0.1/kulprit/search/l1.py` & `kulprit-0.1.0/kulprit/search/l1.py`

 * *Files identical despite different names*

### Comparing `kulprit-0.0.1/kulprit/search/searcher.py` & `kulprit-0.1.0/kulprit/search/searcher.py`

 * *Files identical despite different names*

### Comparing `kulprit-0.0.1/pyproject.toml` & `kulprit-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,19 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dynamic = ["version"]
 description = "Kullback-Leibler projections for Bayesian model selection."
 dependencies = [
+    "arviz>=0.17.1",
     "bambi>=0.12.0",
     "scikit-learn>=1.0.2",
     "numba>=0.56.0",
+    "preliz>=0.4.1"
 ]
 
 [tool.flit.module]
 name = "kulprit"
 
 [project.urls]
 source = "https://github.com/bambinos/kulprit"
```

