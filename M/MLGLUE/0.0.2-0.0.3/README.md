# Comparing `tmp/MLGLUE-0.0.2.tar.gz` & `tmp/MLGLUE-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLGLUE-0.0.2.tar", last modified: Fri Oct 27 08:09:49 2023, max compression
+gzip compressed data, was "MLGLUE-0.0.3.tar", last modified: Fri Apr 12 08:00:49 2024, max compression
```

## Comparing `MLGLUE-0.0.2.tar` & `MLGLUE-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-10-27 08:09:49.712663 MLGLUE-0.0.2/
--rw-rw-rw-   0        0        0     1126 2023-10-18 08:35:00.000000 MLGLUE-0.0.2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-10-27 08:09:49.681367 MLGLUE-0.0.2/MLGLUE/
--rw-rw-rw-   0        0        0     9168 2023-10-18 08:22:38.000000 MLGLUE-0.0.2/MLGLUE/Likelihoods.py
--rw-rw-rw-   0        0        0    36004 2023-10-18 08:18:30.000000 MLGLUE-0.0.2/MLGLUE/MLGLUE.py
--rw-rw-rw-   0        0        0      143 2023-04-18 14:23:30.000000 MLGLUE-0.0.2/MLGLUE/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-27 08:09:49.697041 MLGLUE-0.0.2/MLGLUE.egg-info/
--rw-rw-rw-   0        0        0      691 2023-10-27 08:09:49.000000 MLGLUE-0.0.2/MLGLUE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-10-27 08:09:49.000000 MLGLUE-0.0.2/MLGLUE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-27 08:09:49.000000 MLGLUE-0.0.2/MLGLUE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-10-27 08:09:49.000000 MLGLUE-0.0.2/MLGLUE.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-10-27 08:09:49.000000 MLGLUE-0.0.2/MLGLUE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      691 2023-10-27 08:09:49.697041 MLGLUE-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-10-27 07:42:01.000000 MLGLUE-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-10-27 08:09:49.712663 MLGLUE-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      954 2023-10-27 08:09:43.000000 MLGLUE-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:00:49.285384 MLGLUE-0.0.3/
+-rw-rw-rw-   0        0        0     1126 2023-10-18 08:35:00.000000 MLGLUE-0.0.3/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-12 08:00:49.254135 MLGLUE-0.0.3/MLGLUE/
+-rw-rw-rw-   0        0        0     9156 2024-04-12 07:57:57.000000 MLGLUE-0.0.3/MLGLUE/Likelihoods.py
+-rw-rw-rw-   0        0        0    37269 2024-04-12 07:54:23.000000 MLGLUE-0.0.3/MLGLUE/MLGLUE.py
+-rw-rw-rw-   0        0        0      143 2023-04-18 14:23:30.000000 MLGLUE-0.0.3/MLGLUE/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:00:49.269764 MLGLUE-0.0.3/MLGLUE.egg-info/
+-rw-rw-rw-   0        0        0      691 2024-04-12 08:00:48.000000 MLGLUE-0.0.3/MLGLUE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2024-04-12 08:00:49.000000 MLGLUE-0.0.3/MLGLUE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 08:00:48.000000 MLGLUE-0.0.3/MLGLUE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-12 08:00:48.000000 MLGLUE-0.0.3/MLGLUE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-12 08:00:48.000000 MLGLUE-0.0.3/MLGLUE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      691 2024-04-12 08:00:49.285384 MLGLUE-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2184 2023-10-27 08:49:15.000000 MLGLUE-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 08:00:49.285384 MLGLUE-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      954 2024-04-12 07:58:52.000000 MLGLUE-0.0.3/setup.py
```

### Comparing `MLGLUE-0.0.2/LICENSE` & `MLGLUE-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `MLGLUE-0.0.2/MLGLUE/Likelihoods.py` & `MLGLUE-0.0.3/MLGLUE/Likelihoods.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
         Compute the likelihood according to Beven & Binley (1991), i.e., the
         inverse error variance likelihood
 
         :param obs: a 1D list-like corresponding to the observation y-values;
             list-like
         :param sim: a 1D list-like corresponding to the simulation y-values;
             list-like
-
-        :return: likelihood, a float value for the likelihood
+        
+        :return likelihood: a float value for the likelihood
         """
 
         try:
             if obs is None and sim is None:
                 msg = ("No observations and no simulated values are given!")
                 raise ValueError(msg)
             elif obs is None and sim is not None:
@@ -48,15 +48,14 @@
             raise
 
         try:
             if len(sim) != len(obs):
                 msg = ("Length mismatch! Observed values have length {} but "
                        " simulated values have length {}".format(len(obs),
                                                                  len(sim)))
-                # raise ValueError(msg)
                 return 0.
         except ValueError:
             raise
 
         if self.weights is None:
             weights = np.ones(len(obs))
         else:
@@ -109,16 +108,16 @@
         """
         Compute the model efficiency, i.e., the relative variance likelihood
 
         :param obs: a 1D list-like corresponding to the observation y-values;
             list-like
         :param sim: a 1D list-like corresponding to the simulation y-values;
             list-like
-
-        :return: likelihood, a float value for the likelihood
+        
+        :return likelihood: a float value for the likelihood
         """
 
         try:
             if obs is None and sim is None:
                 msg = ("No observations and no simulated values are given!")
                 raise ValueError(msg)
             elif obs is None and sim is not None:
@@ -187,21 +186,21 @@
         self.weights = weights
 
         return
 
     def likelihood(self, obs=None, sim=None):
         """
         Compute the Gaussian log-likelihood
-
+        
         :param obs: a 1D list-like corresponding to the observation y-values;
             list-like
         :param sim: a 1D list-like corresponding to the simulation y-values;
             list-like
-
-        :return: likelihood, a float value for the likelihood
+        
+        :return likelihood: a float value for the likelihood
         """
 
         try:
             if obs is None and sim is None:
                 msg = ("No observations and no simulated values are given!")
                 raise ValueError(msg)
             elif obs is None and sim is not None:
```

### Comparing `MLGLUE-0.0.2/MLGLUE/MLGLUE.py` & `MLGLUE-0.0.3/MLGLUE/MLGLUE.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
             n_samples=1000,
             samples=None,
             tuning=0.2,
             n_levels=1,
             coarsening_factor=2,
             obs_x=None,
             obs_y=None,
+            thresholds=None,
             multiprocessing=False,
             n_processors=4,
             variance_analysis=None,
             savefigs="my_model",
             model_returns_all=False
     ):
         """
@@ -58,14 +59,18 @@
         :param coarsening_factor: the coarsening factor between levels (assuming
             geometric MLMC, may be defined as M_l = coarsening_factor * M_{l-1}
             for all l); int
         :param obs_x: a 1D list-like corresponding to the observation x-values;
             list-like
         :param obs_y: a 1D list-like corresponding to the observation y-values;
             list-like
+        :param thresholds: a 1D list-like of floats representing the level-
+            dependent likelihood thresholds; if thresholds is not None, the
+            tuning phase is skipped (take this effect into account when
+            defining the total number of calculation steps)
         :param multiprocessing: whether to use multiprocessing or not; bool
         :param n_processors: number of processors to use if multiprocessing is
             True; int
         :param variance_analysis: variance analysis methodology after the
             tuning phase, valid options are "strong", "weak", None; str or None
         :param savefigs: whether to save variance analysis figures. if None,
             figures will not be saved, if str, figures will be saved with
@@ -94,36 +99,42 @@
         self.n_processors = n_processors
         self.variance_analysis = variance_analysis
         self.normalized_likelihoods = None
         self.savefigs = savefigs
         self.model_returns_all = model_returns_all
 
         # initialize output data structures
-        self.results = [] # --> holds only the highest level model outputs
-        self.selected_samples = [] # --> holds behavioural samples (samples that are accepted on the highest level)
-        self.likelihoods = [] # --> holds highest level likelihood values corresponding to selected_samples
-        self.likelihoods_tuning = [[] for i in range(self.n_levels)] # --> holds likelihood values for all levels from tuning
+        self.results = [] # --> this holds only the final results (i.e., from the finest level)
+        self.selected_samples = []
+        self.likelihoods = []
+        self.likelihoods_tuning = [[] for i in range(self.n_levels)]
         self.results_analysis = [[] for i in range(self.n_levels)] # --> holds results from all levels during sampling
         self.results_analysis_tuning = [[] for i in range(self.n_levels)] # --> holds results from all levels during tuning
-        self.thresholds = [] # --> holds likelihood thresholds on all levels
+        self.highest_level_calls = [] # --> holds identifiers for highest level calls (1 corresponds to a highest level call)
+
+        if thresholds is not None:
+            self.thresholds = thresholds
+            self.thresholds_predefined = True
+        else:
+            self.thresholds = []
+            self.thresholds_predefined = False
         self.full_results = [] # --> holds full model results (i.e., full array of heads for all model cells instead of
                                 #   simulated equivalents of observed values)
 
         return
 
     def MLGLUE_tuning(self, samples):
         """
         Perform the tuning phase of MLGLUE
 
         :param samples: list-like with parameter samples for tuning with shape
-            (n_samples, n_parameters); list-ike
-        
-        :return: likelihoods_tuning (the likelihoods corresponding to the
-            samples)
-        :return: results_analysis_tuning (the model outputs on each level for each sample)
+            (n_samples, n_parameters); list-ike     
+            
+        :return likelihoods_tuning: the likelihoods corresponding to the samples; list-like
+        :return results_analysis_tuning: the model outputs on each level for each sample; list-like
 
         Note: if the model function only has one level, it should be the finest /
             target level.
         """
         run_id = 0
         for sample in samples:
             # start at the coarsest / lowest level
@@ -175,25 +186,27 @@
 
                 run_id += 1
 
         return self.likelihoods_tuning, self.results_analysis_tuning
 
     def analyze_variances_likelihoods_strong(self):
         """
+        Analyze the variances from the tuning phase and test whether the strong
+        variance inequality holds.
         Analyze the relationships between levels in terms of variances:
             - variances of likelihood values on each individual level
             - covariances of likelihoods across levels
             - variances of the difference between likelihood values on subsequent levels
 
         Specifically, the following inequality is evaluated for all levels:
             Var[L_(l) - L_(l-1)] = Var[L_(l)] + Var[L_(l-1)] - 2 * Cov[L_(l), L_(l-1)]
-
-        MLGLUE is stopped if 2 * Cov[L_(l), L_(l-1)] < Var[L_(l-1)] for any l
-
-        :return: None
+            
+        Note that variances within levels as well as variances of differences between
+            levels are printed as logarithms with the base equal to the coarsening
+            factor!
         """
 
         self.likelihoods_tuning = np.asarray(self.likelihoods_tuning)
 
         # get number of likelihoods in every level
         # n_vals = len(self.likelihoods_tuning[0, :])
         lens = []
@@ -231,15 +244,15 @@
 
         # initialize list to store booleans representing whether the veriance
         #   inequality holds or not
         ineq = []
         # initialize list to store booleans representing whether the cross-level
         #   variance decays
         decay = []
-        print("Covariances across levels: ", covs_cross_levels)
+        print("Covs across levels: ", covs_cross_levels)
         print("Variances within levels: ", vars_within_levels)
         print("Variances across levels: ", rhs)
         # iterate over levels to check variance inequality
         for i in range(self.n_levels - 1):
             if vars_within_levels[i + 1] >= rhs[i]:
                 print("The variance inequality holds between levels ",
                       "{} and {}: {:1.5f} >= {:1.5e}".format(i, i + 1,
@@ -262,38 +275,34 @@
 
         # throw error if the inequality does not hold for one level combination
         try:
             if not np.array(ineq).all():
                 msg = ("The variance inequality does not hold for all two "
                        "subsequent levels!")
                 print(msg)
-                raise ValueError(msg)
+                # raise ValueError(msg)
             else:
                 print("The variance inequality holds between all two "
                       "subsequent levels!")
 
             if not np.array(decay).all():
                 msg = ("The cross-level variance does not decay monotonically!")
                 print(msg)
-                raise ValueError(msg)
+                # raise ValueError(msg)
             else:
                 print("The cross-level variance decays monotonically!")
 
         except ValueError:
             raise
 
         return
 
     def analyze_means_likelihoods_strong(self):
         """
-        Analyze the relationships between levels in terms of mean values:
-            - means of likelihood values on each individual level
-            - means of the difference between likelihood values on subsequent levels
-
-        :return: None
+        Analyze the means from the tuning phase.
         """
 
         self.likelihoods_tuning = np.asarray(self.likelihoods_tuning)
 
         # get number of likelihoods in every level
         # n_vals = len(self.likelihoods_tuning[0, :])
         lens = []
@@ -325,21 +334,16 @@
         print("Means within levels: ", means_within_levels)
         print("Means values of difference between levels: ", rhs)
 
         return
 
     def analyze_variances_likelihoods_weak(self):
         """
-        Analyze the relationships between levels in terms of the correlation between
-        subsequent levels.
-
-        MLGLUE is stopped if there is zero or negative correlation between
-        subsequent levels.
-
-        :return: None
+        Analyze the variances from the tuning phase and test whether all
+        levels are correlated (check for positive correlation)
         """
 
         self.likelihoods_tuning = np.asarray(self.likelihoods_tuning)
 
         # get number of likelihoods in every level
         n_vals = len(self.likelihoods_tuning[0, :])
 
@@ -380,41 +384,33 @@
         return
 
     def calculate_threshold(self):
         """
         Calculate the thresholds according to the threshold fraction given by
         the likelihood function
 
-        :return: thresholds (list-like specifying the float threshold values
-            on each level)
+        :return threshold: list-like specifying the scalar threshold values
+            on each level; list-like
         """
 
         counter = 0
         for level in self.likelihoods_tuning:
             threshold = np.quantile(level, 1 - self.likelihood.threshold)
             self.thresholds.append(threshold)
             counter += 1
-
-        # get the maximum threshold and use that for all levels
-        # self.thresholds = [max(self.thresholds)] * self.n_levels
-
         print("\nThe calculated thresholds are: {}".format(self.thresholds))
 
         return self.thresholds
 
     def MLGLUE_sampling(self, samples):
         """
         Perform the sampling phase of MLGLUE
 
-        :param samples: list-like of parameter samples to evaluate with shape
-            (n_samples, n_parameters); list-like
-
-        :return: selected_samples, list-like of behavioural parameter samples
-        :return: likelihoods, list-like of likelihood values corresponding to the
-            selected_samples
+        :return selected_samples: selected samples; list-like
+        :return likelihoods: the likelihoods corresponding to the selected samples; list-like
 
         Note: if the model function only has one level, it should be the finest /
             target level.
         """
 
         run_id = 0
         for sample in samples:
@@ -466,14 +462,17 @@
 
                     # if the likelihood in the current level is below a
                     #   threshold, do not use the sample, break the level
                     #   iteration, and go to the next sample
                     else:
                         break
 
+                    if level_checker == self.n_levels - 1:
+                        self.highest_level_calls.append(1)
+
                 if (likelihood_ is not None and
                         likelihood_ >= self.thresholds[-1] and
                         level_checker == self.n_levels - 1):
                     if self.model_returns_all == True:
                         self.full_results.append(results_full)
                     self.selected_samples.append(sample)
                     self.likelihoods.append(likelihood_)
@@ -481,30 +480,37 @@
 
                 run_id += 1
 
         # the number of selected samples is equal to the number of model results
         #     for the highest level
         return self.selected_samples, self.likelihoods
 
-    # @ray.remote
     def evaluate_sample(self, sample, run_id):
         """
         A function for evaluate a sample that can be used in a multiprocessing
         framework; used during the sampling phase
 
         :param sample: the current sample; list-like
-        :param run_id: a run identifier; string or int
-        :return: a tuple of (selected_sample, likelihood, results, results_analysis_sample, results_full),
-            if the sample is accepted; None is returned if the sample is not accepted
-
-        Note: the selected sample as well as the corresponding likelihood are
-            appended to a global list that is returned by the perform_MLGLUE
-            method
+        :param run_id: an integer identifier for the current model run, which is passed to the model function; int
+
+        :return sample: the parameter sample (returned if selected); list-like
+        :return likelihood_: the likelihood corresponding to the sample (returned if sample is selected); float
+        :return results: model results corresponding to obs_y (returned if sample is selected); list-like
+        :return results_analysis_sample: results on all model levels (returned if sample is selected); list-like
+        :return highest_level_call: 0 if no highest level call, 1 if highest level call; int
+        :return results_full: if model returns more results, they are returned here as well (if sample is selected);
+            list-like
+
+        Note: the selected sample as well as the corresponding likelihood are appended to a global list that is
+            returned by the perform_MLGLUE method
         """
 
+        # define highest level call
+        highest_level_call = 0
+
         # start at the coarsest / lowest level
         level_ = 0
 
         # initialize results
         results = None
         results_analysis_sample = []
 
@@ -526,15 +532,16 @@
             # iterate over the higher levels
             for level__ in range(1, self.n_levels):
                 # check if the likelihood from the next coarser level is above a
                 #     certain threshold
                 level_checker = level__
                 if likelihood_ is not None and likelihood_ >= self.thresholds[level__ - 1]:
                     if level__ == self.n_levels - 1:
-                        print("highest level call: ", run_id)
+                        # print("highest level call: ", run_id)
+                        highest_level_call = 1
                     # if the likelihood was above a threshold in the lower
                     #   level, go up one level and compute the likelihood again
                     if self.model_returns_all == False:
                         likelihood_, results = self.model(sample, level__,
                                                           self.n_levels,
                                                           self.obs_x, self.obs_y,
                                                           self.likelihood,
@@ -557,34 +564,30 @@
                     #   happen below that unwillingly a sample results in a likelihood
                     #   (from a lower level) above the threshold and the level_checker
                     #   corresponding to the highest level. To circumvent this problem,
                     #   the level_checker needs to be reduced by one
                     level_checker -= 1
                     break
 
-            if (likelihood_ is not None and
-                    likelihood_ >= self.thresholds[-1] and
-                    level_checker == self.n_levels - 1):
+            if (likelihood_ is not None and likelihood_ >= self.thresholds[-1] and level_checker == self.n_levels - 1):
                 if self.model_returns_all == True:
                     # append full results
-                    return (sample, likelihood_, results, results_analysis_sample, results_full)
+                    return (sample, likelihood_, results, results_analysis_sample, highest_level_call, results_full)
                 else:
-                    return (sample, likelihood_, results, results_analysis_sample)
+                    return (sample, likelihood_, results, results_analysis_sample, highest_level_call)
             else:
-                return None
+                return (highest_level_call, False)
 
-    # @ray.remote
     def evaluate_sample_tuning(self, sample, run_id):
         """
         A function for evaluating a sample that can be used in a multiprocessing
         framework; used during the tuning phase
 
         :param sample: the current sample; list-like
-        :return: a tuple of (selected_sample, likelihood), if the sample is
-            accepted; None is returned if the sample is not accepted
+        :param run_id: an integer identifier for the current model run, which is passed to the model function; int
         """
 
         likelihoods_sample = []
         results_analysis_tuning_sample = []
 
         # start at the coarsest / lowest level
         level_ = 0
@@ -623,28 +626,33 @@
         if np.isnan(likelihoods_sample).any():
             return None
         else:
             return likelihoods_sample, results_analysis_tuning_sample
 
     def perform_MLGLUE(self):
         """
-        Perform the full MLGLUE, including a tuning phase where the
+        Perform the full MLGLUE sampling, including a tuning phase where the
         inequality regarding variances is checked
 
-        :return: selected_samples; list-like of behavioural samples
-        :return: likelihoods; list-like of likelihoods corresponding to the behavioural samples
-        :return: results; list-like of model outputs on all levels for the behavioural samples
-        :return: results_full; list-like of full model results (optional)
+        :return selected_samples: the selected samples of MLGLUE; list-like
+        :return likelihoods: the likelihoods corresponding to the selected samples; list-like
+        :return results: the model resoults (corresponding to obs_y) corresponding to the selected
+            samples; list-like
+        :return results_full: if the model returns more than simulated observation equivalents,
+            these results corresponding to the selected samples are also returned; list-like
         """
+        
+        try:
+            ray.shutdown()
+        except:
+            pass
 
         if self.samples is None:
             print("No samples provided, using uniform sampling...")
             # generate samples
-            # np.random.seed(2)
-            # np.random.seed(42)
             self.samples = np.random.uniform(
                 low=self.lower_bounds,
                 high=self.upper_bounds,
                 size=(int(self.n_samples), len(self.lower_bounds))
             )
 
         else:
@@ -662,49 +670,49 @@
         #   sample index
         if self.multiprocessing:
             iterable_tuning = [(s, idx) for s, idx in zip(samples_tuning,
                                                           [i for i in range(samples_divide)])]
             iterable_sampling = [(s, idx) for s, idx in zip(samples_sampling,
                                                             [i + samples_divide for i in range(self.n_samples - samples_divide)])]
 
-        if not self.multiprocessing:
-            # perform tuning
-            print("\nStarting tuning without multiprocessing...")
-            _ = self.MLGLUE_tuning(samples_tuning)
-
-        elif self.multiprocessing:
-            ray.shutdown()
-            ray.init(num_cpus=self.n_processors)
-            # perform tuning with multiprocessing
-            print("\nStarting tuning with multiprocessing...")
-            with Pool(processes=self.n_processors) as pool: # map # maxtasksperchild=1
-                for result in pool.starmap(self.evaluate_sample_tuning, iterable_tuning):
-                    if result is not None:
-                        for num, i in enumerate(zip(result[0], result[1])):
-                            self.likelihoods_tuning[num].append(i[0])
-                            self.results_analysis_tuning[num].append(i[1])
-            ray.shutdown()
-            ray.shutdown()
-
-        # analyze variances and mean values
-        if self.variance_analysis == "strong":
-            self.analyze_variances_likelihoods_strong()
-            self.analyze_means_likelihoods_strong()
-        elif self.variance_analysis == "weak":
-            self.analyze_variances_likelihoods_weak()
-            self.analyze_means_likelihoods_strong()
-        elif self.variance_analysis is None:
-            pass
-        else:
-            print("No valid variance analysis methodology selected; "
-                  "continuing without analysis!")
-
-        # compute thresholds
-        self.thresholds = self.calculate_threshold()
-        # self.thresholds = [0., 0., 0.]
+        if self.thresholds_predefined == False:
+            if not self.multiprocessing:
+                # perform tuning
+                print("\nStarting tuning without multiprocessing...")
+                _ = self.MLGLUE_tuning(samples_tuning)
+
+            elif self.multiprocessing:
+                ray.shutdown()
+                ray.init(num_cpus=self.n_processors)
+                # perform tuning with multiprocessing
+                print("\nStarting tuning with multiprocessing...")
+                with Pool(processes=self.n_processors) as pool: # map # maxtasksperchild=1
+                    for result in pool.starmap(self.evaluate_sample_tuning, iterable_tuning):
+                        if result is not None:
+                            for num, i in enumerate(zip(result[0], result[1])):
+                                self.likelihoods_tuning[num].append(i[0])
+                                self.results_analysis_tuning[num].append(i[1])
+                ray.shutdown()
+                ray.shutdown()
+            
+            # analyze variances and mean values
+            if self.variance_analysis == "strong":
+                self.analyze_variances_likelihoods_strong()
+                self.analyze_means_likelihoods_strong()
+            elif self.variance_analysis == "weak":
+                self.analyze_variances_likelihoods_weak()
+                self.analyze_means_likelihoods_strong()
+            elif self.variance_analysis is None:
+                pass
+            else:
+                print("No valid variance analysis methodology selected; "
+                      "continuing without analysis!")
+            
+            # compute thresholds
+            self.thresholds = self.calculate_threshold()
 
         if not self.multiprocessing:
             # perform sampling
             print("\nStarting sampling without multiprocessing...")
             selected_samples, likelihoods = self.MLGLUE_sampling(
                 samples_sampling)
 
@@ -715,41 +723,45 @@
 
         elif self.multiprocessing:
             ray.shutdown()
             ray.init(num_cpus=self.n_processors)
             print("\nStarting sampling with multiprocessing...")
             with Pool(processes=self.n_processors) as pool: # maxtasksperchild=1
                 for eval_ in pool.starmap(self.evaluate_sample, iterable_sampling):
-                    # TODO: this has to be improved somehow; sometimes,
-                    #  eval_[2] is None here but the result for the model
-                    #  call is not actually None
-                    if eval_ is not None and eval_[2] is not None:
+                    if eval_ is not None and eval_[1] is not False:
                         self.selected_samples.append(eval_[0])
                         self.likelihoods.append(eval_[1])
                         self.results.append(eval_[2])
                         for num, i in enumerate(eval_[3]):
                             self.results_analysis[num].append(i)
+                        if eval_[4] == 1:
+                            self.highest_level_calls.append(eval_[4])
                         if self.model_returns_all == True:
-                            self.full_results.append(eval_[4])
+                            self.full_results.append(eval_[5])
+                    elif eval_ is not None and eval_[1] is False:
+                        if eval_[0] == 1:
+                            self.highest_level_calls.append(eval_[0])
             ray.shutdown()
 
             if self.model_returns_all == False:
                 return self.selected_samples, self.likelihoods, self.results
             else:
                 return self.selected_samples, self.likelihoods, self.results, self.full_results
 
     def estimate_uncertainty(self, quantiles=None):
         """
         Estimate the simulation uncertainty, i.e., normalize likelihoods,
         and create a probability density for the model output
 
         :param quantiles: the quantiles to return for the prediction;
             list-like of three float values [lower q., 0.5, upper q.]
-        :return: uncertainty; list-like with shape (n_outputs, 3) with the
-            uncertainty estimates
+            
+        :return: numpy array of shape (len(obs_x), 3) having the lower
+            quantile in the first, the median in the second, and the
+            upper quantile in the third column; numpy array
         """
 
         # normalize likelihoods
         if quantiles is None:
             quantiles = [0.05, 0.5, 0.95]
         self.normalized_likelihoods = np.asarray(self.likelihoods) / np.sum(
             np.asarray(self.likelihoods))
```

### Comparing `MLGLUE-0.0.2/MLGLUE.egg-info/PKG-INFO` & `MLGLUE-0.0.3/MLGLUE.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MLGLUE
-Version: 0.0.2
+Version: 0.0.3
 Summary: a Python implementation of the (M)ulti(l)evel (G)eneralized (L)ikelihood (U)ncertainty (E)stimation (MLGLUE) algorithm and utility functions
 Home-page: https://github.com/iGW-TU-Dresden/MLGLUE
 Author: M. G. Rudolph
 Author-email: max_gustav.rudolph@tu-dresden.de
 License: MIT
 Platform: Windows
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `MLGLUE-0.0.2/PKG-INFO` & `MLGLUE-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MLGLUE
-Version: 0.0.2
+Version: 0.0.3
 Summary: a Python implementation of the (M)ulti(l)evel (G)eneralized (L)ikelihood (U)ncertainty (E)stimation (MLGLUE) algorithm and utility functions
 Home-page: https://github.com/iGW-TU-Dresden/MLGLUE
 Author: M. G. Rudolph
 Author-email: max_gustav.rudolph@tu-dresden.de
 License: MIT
 Platform: Windows
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `MLGLUE-0.0.2/setup.py` & `MLGLUE-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 setup(
     name = "MLGLUE",
     author = "M. G. Rudolph",
-    version = "0.0.2",
+    version = "0.0.3",
     description = "a Python implementation of the (M)ulti(l)evel (G)eneralized (L)ikelihood (U)ncertainty (E)stimation (MLGLUE) algorithm and utility functions",
     url = "https://github.com/iGW-TU-Dresden/MLGLUE",
     author_email = "max_gustav.rudolph@tu-dresden.de",
     license = "MIT",
     classifiers = [
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
```

