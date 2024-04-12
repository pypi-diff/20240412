# Comparing `tmp/pcgym-0.0.7.tar.gz` & `tmp/pcgym-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcgym-0.0.7.tar", last modified: Sun Mar 10 17:05:25 2024, max compression
+gzip compressed data, was "pcgym-0.0.8.tar", last modified: Fri Apr 12 11:41:33 2024, max compression
```

## Comparing `pcgym-0.0.7.tar` & `pcgym-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-03-10 17:05:25.011623 pcgym-0.0.7/
--rw-rw-rw-   0        0        0     1094 2024-03-06 13:10:13.000000 pcgym-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     4864 2024-03-10 17:05:25.010626 pcgym-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2349 2024-03-10 16:18:36.000000 pcgym-0.0.7/README.md
--rw-rw-rw-   0        0        0     1198 2024-03-10 17:05:09.000000 pcgym-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       93 2024-03-08 16:41:43.000000 pcgym-0.0.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-03-10 17:05:25.011623 pcgym-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-10 17:05:24.961789 pcgym-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-03-10 17:05:24.980726 pcgym-0.0.7/src/pcgym/
--rw-rw-rw-   0        0        0       27 2024-03-08 18:30:09.000000 pcgym-0.0.7/src/pcgym/__init__.py
--rw-rw-rw-   0        0        0    28271 2024-01-26 15:18:15.000000 pcgym-0.0.7/src/pcgym/case_studies.py
--rw-rw-rw-   0        0        0     5108 2024-03-08 18:30:24.000000 pcgym-0.0.7/src/pcgym/integrator.py
--rw-rw-rw-   0        0        0     7438 2024-03-07 14:30:48.000000 pcgym-0.0.7/src/pcgym/model_classes.py
--rw-rw-rw-   0        0        0     8449 2024-03-07 15:30:38.000000 pcgym-0.0.7/src/pcgym/oracle.py
--rw-rw-rw-   0        0        0    12503 2024-03-10 17:02:26.000000 pcgym-0.0.7/src/pcgym/pcgym.py
--rw-rw-rw-   0        0        0     9365 2024-03-10 17:02:38.000000 pcgym-0.0.7/src/pcgym/policy_Evaluation.py
-drwxrwxrwx   0        0        0        0 2024-03-10 17:05:25.008632 pcgym-0.0.7/src/pcgym.egg-info/
--rw-rw-rw-   0        0        0     4864 2024-03-10 17:05:24.000000 pcgym-0.0.7/src/pcgym.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2024-03-10 17:05:24.000000 pcgym-0.0.7/src/pcgym.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-10 17:05:24.000000 pcgym-0.0.7/src/pcgym.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2024-03-10 17:05:24.000000 pcgym-0.0.7/src/pcgym.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-10 17:05:24.000000 pcgym-0.0.7/src/pcgym.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 11:41:33.435200 pcgym-0.0.8/
+-rw-rw-rw-   0        0        0     1094 2024-03-06 13:10:13.000000 pcgym-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     6056 2024-04-12 11:41:33.434199 pcgym-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3316 2024-04-02 11:41:27.000000 pcgym-0.0.8/README.md
+-rw-rw-rw-   0        0        0     1309 2024-04-12 11:35:26.000000 pcgym-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       95 2024-04-02 11:41:57.000000 pcgym-0.0.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 11:41:33.435200 pcgym-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-12 11:41:33.397238 pcgym-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-12 11:41:33.414236 pcgym-0.0.8/src/pcgym/
+-rw-rw-rw-   0        0        0        0 2024-04-02 11:41:34.000000 pcgym-0.0.8/src/pcgym/__init__.py
+-rw-rw-rw-   0        0        0     7262 2024-04-12 11:15:27.000000 pcgym-0.0.8/src/pcgym/evaluation_metrics.py
+-rw-rw-rw-   0        0        0     5142 2024-04-12 11:17:30.000000 pcgym-0.0.8/src/pcgym/integrator.py
+-rw-rw-rw-   0        0        0     8666 2024-04-12 11:20:55.000000 pcgym-0.0.8/src/pcgym/model_classes.py
+-rw-rw-rw-   0        0        0     8782 2024-04-12 11:18:31.000000 pcgym-0.0.8/src/pcgym/oracle.py
+-rw-rw-rw-   0        0        0    15378 2024-04-12 11:27:09.000000 pcgym-0.0.8/src/pcgym/pcgym.py
+-rw-rw-rw-   0        0        0    10657 2024-04-12 11:25:21.000000 pcgym-0.0.8/src/pcgym/policy_evaluation.py
+drwxrwxrwx   0        0        0        0 2024-04-12 11:41:33.433271 pcgym-0.0.8/src/pcgym.egg-info/
+-rw-rw-rw-   0        0        0     6056 2024-04-12 11:41:33.000000 pcgym-0.0.8/src/pcgym.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2024-04-12 11:41:33.000000 pcgym-0.0.8/src/pcgym.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 11:41:33.000000 pcgym-0.0.8/src/pcgym.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-04-12 11:41:33.000000 pcgym-0.0.8/src/pcgym.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-12 11:41:33.000000 pcgym-0.0.8/src/pcgym.egg-info/top_level.txt
```

### Comparing `pcgym-0.0.7/LICENSE` & `pcgym-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pcgym-0.0.7/PKG-INFO` & `pcgym-0.0.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcgym
-Version: 0.0.7
+Version: 0.0.8
 Summary: Reinforcement learning suite of process control problems.
 Author-email: Max Bloor <max.bloor@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Maximilian Bloor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,14 +47,19 @@
 Requires-Dist: cloudpickle
 Requires-Dist: matplotlib
 Requires-Dist: gymnasium
 Requires-Dist: casadi
 Requires-Dist: jax[cpu]
 Requires-Dist: equinox
 Requires-Dist: diffrax
+Provides-Extra: optional
+Requires-Dist: jupyterlab; extra == "optional"
+Requires-Dist: torch; extra == "optional"
+Requires-Dist: stable-baselines3; extra == "optional"
+Requires-Dist: mkdocs-material; extra == "optional"
 
 <h1 align="center">
   <a href="https://github.com/MaximilianB2/pc-gym/blob/main/docs/img/pc-gym-blue-Ai.png">
     <img src="https://github.com/MaximilianB2/pc-gym/blob/main/docs/img/pc-gym-blue-Ai.png"/></a><br>
   <b>Reinforcement learning environments for process control </b><br>
 </h1>
 <p align="center">
@@ -65,14 +70,19 @@
 </p>
 
 
 ## Quick start ⚡
 Setup a CSTR environment with a setpoint change
 
 ```python 
+import pcgym
+
+# Simulation variables
+nsteps = 100
+T = 25
 
 # Setpoint
 SP = {'Ca': [0.85 for i in range(int(nsteps/2))] + [0.9 for i in range(int(nsteps/2))]} 
 
 # Action and observation Space
 action_space = {'low': np.array([295]), 'high': np.array([302])}
 observation_space = {'low': np.array([0.7,300,0.8]),'high': np.array([1,350,0.9])}
@@ -112,26 +122,33 @@
 pip install pcgym
 ```
 
 ## Examples
 
 TODO: Link example notebooks here
 
-## Implemented Process Control Environments
-
-TODO: Add table of environments
+## Implemented Process Control Environments 🎛️
 
-## Other Great Gyms 🔍
+|          Environment          | Reference | Source | Documentation |
+|:-----------------------------:|:---------:|:------:|---------------|
+|              CSTR             | [Hedengren, 2022](https://github.com/APMonitor/pdc/blob/master/CSTR_Control.ipynb)     | [Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/model_classes.py)      |               |
+|       First Order Sytem       |      N/A  | [Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/model_classes.py)        |               |
+| Multistage Extraction Column  |  [Ingham et al, 2007 (pg 471)](https://onlinelibrary.wiley.com/doi/book/10.1002/9783527614219)         | [Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/model_classes.py)        |               |
 
-TODO: Link other gyms such as Jumanji, safety gymnasium etc.
 
+ 
 ## Citing `pc-gym`
 If you use `pc-gym` in your research, please cite using the following 
 ```
 @software{pcgym2024,
   author = {Max Bloor and ...},
   title = {{pc-gym}: Reinforcement Learning Envionments for Process Control},
   url = {https://github.com/MaximilianB2/pc-gym},
   version = {0.0.4},
   year = {2024},
 }
 ```
+
+## Other Great Gyms 🔍
+- ✨[safe-control-gym](https://github.com/utiasDSL/safe-control-gym) 
+- ✨[safety-gymnasium](https://github.com/PKU-Alignment/safety-gymnasium)
+- ✨[gymnax](https://github.com/RobertTLange/gymnax)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pcgym Version: 0.0.7 Summary: Reinforcement
+Metadata-Version: 2.1 Name: pcgym Version: 0.0.8 Summary: Reinforcement
 learning suite of process control problems. Author-email: Max Bloor
 gmail.com> License: MIT License Copyright (c) 2024 Maximilian Bloor Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -24,36 +24,50 @@
 :: English Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
 Scientific/Engineering :: Information Analysis Classifier: Topic :: Scientific/
 Engineering :: Mathematics Requires-Python: ~=3.10 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: ruff Requires-Dist: numpy
 Requires-Dist: tqdm Requires-Dist: cloudpickle Requires-Dist: matplotlib
 Requires-Dist: gymnasium Requires-Dist: casadi Requires-Dist: jax[cpu]
-Requires-Dist: equinox Requires-Dist: diffrax
+Requires-Dist: equinox Requires-Dist: diffrax Provides-Extra: optional
+Requires-Dist: jupyterlab; extra == "optional" Requires-Dist: torch; extra ==
+"optional" Requires-Dist: stable-baselines3; extra == "optional" Requires-Dist:
+mkdocs-material; extra == "optional"
 ************ _[[_hh_tt_tt_pp_ss_::_//_//_gg_ii_tt_hh_uu_bb_.._cc_oo_mm_//_MM_aa_xx_ii_mm_ii_ll_ii_aa_nn_BB_22_//_pp_cc_--_gg_yy_mm_//_bb_ll_oo_bb_//_mm_aa_ii_nn_//_dd_oo_cc_ss_//_ii_mm_gg_//_pp_cc_--_gg_yy_mm_--_bb_ll_uu_ee_--
                                     _AA_ii_.._pp_nn_gg_]]
             RReeiinnffoorrcceemmeenntt lleeaarrnniinngg eennvviirroonnmmeennttss ffoorr pprroocceessss ccoonnttrrooll
                                      ************
   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-_3_._1_0_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
                            _b_a_d_g_e_/_l_i_c_e_n_s_e_-_M_I_T_-_o_r_a_n_g_e_]
-## Quick start â¡ Setup a CSTR environment with a setpoint change ```python #
-Setpoint SP = {'Ca': [0.85 for i in range(int(nsteps/2))] + [0.9 for i in range
-(int(nsteps/2))]} # Action and observation Space action_space = {'low':
-np.array([295]), 'high': np.array([302])} observation_space = {'low': np.array(
-[0.7,300,0.8]),'high': np.array([1,350,0.9])} # Construct the environment
-parameter dictionary env_params = { 'N': nsteps, # Number of time steps 'tsim':
-T, # Simulation Time 'SP' :SP, 'o_space' : observation_space, 'a_space' :
-action_space, 'x0': np.array([0.8, 330, 0.8]), # Initial conditions [Ca, T,
-Ca_SP] 'model': 'cstr_ode', # Select the model } # Create environment env =
-pcgym.make_env(env_params) # Reset the environment obs, state = env.reset() #
-Sample a random action action = env.action_space.sample() # Perform a step in
-the environment obs, rew, done, term, info = env.step(action) ``` ##
-Documentation You can read the full documentation [here](https://
-maximilianb2.github.io/pc-gym/)! ## Installation â³ The latest pc-gym version
-can be installed from PyPI: ```bash pip install pcgym ``` ## Examples TODO:
-Link example notebooks here ## Implemented Process Control Environments TODO:
-Add table of environments ## Other Great Gyms ð TODO: Link other gyms such
-as Jumanji, safety gymnasium etc. ## Citing `pc-gym` If you use `pc-gym` in
-your research, please cite using the following ``` @software{pcgym2024, author
-= {Max Bloor and ...}, title = {{pc-gym}: Reinforcement Learning Envionments
-for Process Control}, url = {https://github.com/MaximilianB2/pc-gym}, version =
-{0.0.4}, year = {2024}, } ```
+## Quick start â¡ Setup a CSTR environment with a setpoint change ```python
+import pcgym # Simulation variables nsteps = 100 T = 25 # Setpoint SP = {'Ca':
+[0.85 for i in range(int(nsteps/2))] + [0.9 for i in range(int(nsteps/2))]} #
+Action and observation Space action_space = {'low': np.array([295]), 'high':
+np.array([302])} observation_space = {'low': np.array([0.7,300,0.8]),'high':
+np.array([1,350,0.9])} # Construct the environment parameter dictionary
+env_params = { 'N': nsteps, # Number of time steps 'tsim':T, # Simulation Time
+'SP' :SP, 'o_space' : observation_space, 'a_space' : action_space, 'x0':
+np.array([0.8, 330, 0.8]), # Initial conditions [Ca, T, Ca_SP] 'model':
+'cstr_ode', # Select the model } # Create environment env = pcgym.make_env
+(env_params) # Reset the environment obs, state = env.reset() # Sample a random
+action action = env.action_space.sample() # Perform a step in the environment
+obs, rew, done, term, info = env.step(action) ``` ## Documentation You can read
+the full documentation [here](https://maximilianb2.github.io/pc-gym/)! ##
+Installation â³ The latest pc-gym version can be installed from PyPI: ```bash
+pip install pcgym ``` ## Examples TODO: Link example notebooks here ##
+Implemented Process Control Environments ðï¸ | Environment | Reference |
+Source | Documentation | |:-----------------------------:|:---------:|:------:
+|---------------| | CSTR | [Hedengren, 2022](https://github.com/APMonitor/pdc/
+blob/master/CSTR_Control.ipynb) | [Source](https://github.com/MaximilianB2/pc-
+gym/blob/main/src/pcgym/model_classes.py) | | | First Order Sytem | N/A |
+[Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/
+model_classes.py) | | | Multistage Extraction Column | [Ingham et al, 2007 (pg
+471)](https://onlinelibrary.wiley.com/doi/book/10.1002/9783527614219) |
+[Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/
+model_classes.py) | | ## Citing `pc-gym` If you use `pc-gym` in your research,
+please cite using the following ``` @software{pcgym2024, author = {Max Bloor
+and ...}, title = {{pc-gym}: Reinforcement Learning Envionments for Process
+Control}, url = {https://github.com/MaximilianB2/pc-gym}, version = {0.0.4},
+year = {2024}, } ``` ## Other Great Gyms ð - â¨[safe-control-gym](https://
+github.com/utiasDSL/safe-control-gym) - â¨[safety-gymnasium](https://
+github.com/PKU-Alignment/safety-gymnasium) - â¨[gymnax](https://github.com/
+RobertTLange/gymnax)
```

### Comparing `pcgym-0.0.7/pyproject.toml` & `pcgym-0.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pcgym"
-version = "0.0.7"
+version = "0.0.8"
 description = "Reinforcement learning suite of process control problems."
 requires-python = "~=3.10"
 license = { file = "LICENSE" }
 readme = "README.md"
 authors = [{ name = "Max Bloor", email = "max.bloor@gmail.com" }]
 keywords = [
   "reinforcement-learning",
@@ -34,7 +34,10 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [tool.setuptools.dynamic]
 dependencies = { file = ["requirements.txt"] }
+
+[project.optional-dependencies]
+optional = ["jupyterlab", "torch", "stable-baselines3", "mkdocs-material"]
```

### Comparing `pcgym-0.0.7/src/pcgym/integrator.py` & `pcgym-0.0.8/src/pcgym/integrator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from casadi import SX, vertcat, Function, integrator
 from diffrax import diffeqsolve, ODETerm, Tsit5, PIDController 
 import jax.numpy as jnp
-import jax
 
 class integration_engine:
     '''
     Integration class
     Contains both the casadi and JAX integration wrappers.
 
     Inputs: Environment, x0, dt,u_t
@@ -13,26 +12,26 @@
     Output: x+  
     '''
 
     def __init__(self,make_env,env_params):
         self.env = make_env(env_params)
         try:
             integration_method = env_params['integration_method']
-        except:
+        except Exception:
             integration_method = 'casadi'
         assert integration_method in ['jax', 'casadi'], "integration_method must be either 'jax' or 'casadi'"
         
         # NOTE common ode model signature
         # all self.env.model currently have the signature ODE(states, controls)
         # diffrax expects the signature ode(t, states, params)
         # the parameters are fixed within the models so the controllers are the inputs instead
 
         if integration_method == 'casadi':
             # Generate casadi model
-            self.sym_x = self.gen_casadi_variable(self.env.Nx, "x")
+            self.sym_x = self.gen_casadi_variable(self.env.Nx_oracle, "x")
             self.sym_u = self.gen_casadi_variable(self.env.Nu, "u")    
             self.casadi_sym_model = self.casadify(self.env.model, self.sym_x, self.sym_u)
             self.casadi_model_func = self.gen_casadi_function([self.sym_x, self.sym_u],[self.casadi_sym_model],
                                                             "model_func", ["x","u"], ["model_rhs"])
         
         if integration_method == 'jax':
             def autonomous_model(t,x,u): # ignore time
@@ -47,31 +46,32 @@
     def jax_step(self, state, uk):
         '''
         Integrate one time step with JAX.
 
         input: x0, uk
         output: x+
         '''
-        y0 = jnp.array(state[:self.env.Nx]) # Only pass the states of the model (exclude the setpoints)
+        y0 = jnp.array(state[:self.env.Nx_oracle]) # Only pass the states of the model (exclude the setpoints)
         uk = jnp.array(uk)
         solution = diffeqsolve(self.jax_ode, self.jax_solver, self.t0, self.tf, self.dt0, y0, args=uk,stepsize_controller=self.step_controller)
         return solution.ys[-1, :]  # return only final state
 
     def casadi_step(self,state,uk):
 
         '''
         Integrate one time step with casadi.
 
         input: x0, uk
         output: x+
         '''
         plant_func = self.casadi_model_func
         discretised_plant = self.discretise_model(plant_func, self.env.dt)
-      
-        xk = state[:self.env.Nx]
+   
+        xk = state[:self.env.Nx_oracle]
+
         Fk = discretised_plant(x0=xk, p=uk)
         return Fk
 
     def casadify(self, model, sym_x, sym_u):
         """
         Given a model with Nx states and Nu inputs and returns rhs of ode,
         return casadi symbolic model (Not function!)
@@ -129,15 +129,16 @@
         """
         Input:
             casadi_func to be discretised
         
         Output:
             discretised casadi func
         """
-        x = SX.sym("x", self.env.Nx)
+        x = SX.sym("x", self.env.Nx_oracle)
+       
         u = SX.sym("u", self.env.Nu)
         xdot = casadi_func(x, u)
 
         dae = {'x':x, 'p':u, 'ode':xdot} 
         t0 = 0
         tf = delta_t
         discrete_model = integrator('discrete_model', 'cvodes', dae,t0,tf)
```

### Comparing `pcgym-0.0.7/src/pcgym/model_classes.py` & `pcgym-0.0.8/src/pcgym/model_classes.py`

 * *Files 13% similar despite different names*

```diff
@@ -216,7 +216,55 @@
         'parameters': self.__dict__.copy(), 
         'states': ['X1', 'Y1', 'X2', 'Y2', 'X3', 'Y3', 'X4', 'Y4', 'X5', 'Y5'],
         'inputs': ['L','G'],
         'disturbances': ['X0', 'Y6'],
     }
     info['parameters'].pop('int_method', None)  # Remove 'int_method' from the dictionary since it is not a parameter of the model
     return info
+
+
+# ==== Bang-Bang Control Model ====#
+@dataclass(frozen=False, kw_only=True)
+class nonsmooth_control_ode:
+  # Parameters
+  int_method:str = 'jax'
+  a_11:float = 0
+  a_12:float = 1
+  a_21:float = -2
+  a_22:float = -3
+  b_1:float = 0
+  b_2:float = 1
+
+  def __call__(self, x, u):
+    # JAX requires jnp functions and arrays hence two versions
+    if self.int_method == 'jax':
+      # states
+      x1, x2 = x[0], x[1]
+
+      # ode system
+      dxdt = jnp.array([
+          self.a_11*x1 + self.a_12*x2 + self.b_1*u,
+          self.a_21*x1 + self.a_22*x2 + self.b_2*u
+      ])
+        
+      return dxdt
+    else:
+      # states
+      x1, x2 = x[0], x[1]
+
+      dxdt = [
+          self.a_11*x1 + self.a_12*x2 + self.b_1*u,
+          self.a_21*x1 + self.a_22*x2 + self.b_2*u
+      ]
+        
+      return dxdt
+    
+  def info(self):
+    # Return a dictionary with the model information
+    info = {
+        'parameters': self.__dict__.copy(), 
+        'states': ['X1', 'X2'],
+        'inputs': ['U'],
+        'disturbances': ['None'],
+    }
+    info['parameters'].pop('int_method', None)  # Remove 'int_method' from the dictionary since it is not a parameter of the model
+    return info
```

### Comparing `pcgym-0.0.7/src/pcgym/oracle.py` & `pcgym-0.0.8/src/pcgym/oracle.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from casadi import *
+from casadi import MX, Function, integrator, Opti, vertcat, sum1, sum2
 import numpy as np
 
 class oracle():
     '''
     Oracle Class - Class to solve the optimal control problem with perfect 
     knowledge of the environment.
+    Oracle is a nonlinear model predictive controller (nMPC), 
+    using the multiple shooting method.
 
     Inputs: Env
 
     Outputs: Optimal control and state trajectories
     '''
 
     def __init__(self,env,env_params,MPC_params = False):  
@@ -30,15 +32,15 @@
       Generates a model for the given environment.
 
       Returns:
       f: A casadi function that can be used to solve the differential equations defined by the model.
       '''
 
       self.u  = MX.sym('u',self.env.Nu)
-      self.x = MX.sym('x',self.env.Nx)
+      self.x = MX.sym('x',self.env.Nx_oracle)
       dxdt = self.env.model(self.x,self.u)
       dxdt = vertcat(*dxdt)
       f = Function('f',[self.x,self.u],[dxdt],['x','u'],['dxdt'])
       return f
     
     def integrator_gen(self):
       '''
@@ -93,17 +95,17 @@
       Returns:
       - M: A function that takes current state x_0 (p) and returns the optimal control input u.
 
       """
 
       opti = Opti()
       F = self.integrator_gen()
-      x = opti.variable(self.env.Nx, self.N+1)
+      x = opti.variable(self.env.Nx_oracle, self.N+1)
       u = opti.variable(self.env.Nu, self.N)       
-      p = opti.parameter(self.env.Nx, 1)
+      p = opti.parameter(self.env.Nx_oracle, 1)
       setpoint = opti.parameter(len(self.env_params['SP']), self.N+1)
     
       # Cost function sum of squared error plus control penalty. 
       # Both states and controls are normalised to errors equally
       cost = 0
       Sp_i = 0
       for k in self.env_params['SP']:
@@ -126,15 +128,16 @@
       opti.minimize(cost)
 
       # Dynamics
       for k in range(self.N):
         opti.subject_to(x[:, k+1] == F(x[:, k], u[:, k]))
       
       # Control constraints
-      for i in range(self.env.Nu - self.env.Nd):
+     
+      for i in range(self.env.Nu - self.env.Nd_model):
         opti.subject_to(u[i,:] >= self.env_params['a_space']['low'][i])
         opti.subject_to(u[i,:] <= self.env_params['a_space']['high'][i])
       
       # Define disturbance as a control input equality constraint
       # TODO: Add an option to foresee any disturbance.
       if self.env_params.get('disturbances') is not None:
         for i, k in enumerate(self.env.model.info()['disturbances'], start=0):
@@ -147,40 +150,42 @@
       
       # Initial condition
       opti.subject_to(x[:, 0] == p )
       
       # Add user-defined constraint
       if self.env_params.get('constraints') is not None:
         for k in self.env_params['constraints']:
-          if self.env_params['cons_type'][k] == '<=':
-            opti.subject_to(x[self.model_info['states'].index(k),:] <= self.env_params['constraints'][k])
-          elif self.env_params['cons_type'][k] == '>=':
-            opti.subject_to(x[self.model_info['states'].index(k),:] >= self.env_params['constraints'][k])
-          else:
-            raise ValueError('Invalid constraint type')
+          for j in range(len(k)):
+            if self.env_params['cons_type'][k][j] == '<=':
+              opti.subject_to(x[self.model_info['states'].index(k),:] <= self.env_params['constraints'][k][j])
+            elif self.env_params['cons_type'][k][j] == '>=':
+              opti.subject_to(x[self.model_info['states'].index(k),:] >= self.env_params['constraints'][k][j])
+            else:
+              raise ValueError('Invalid constraint type')
       
       # Define the setpoint for the cost function
       SP_i = np.fromiter({k: v[t_step] for k, v in self.env_params['SP'].items()}.values(),dtype=float)
       setpoint_value = SP_i*np.ones((self.N+1,1))  
       opti.set_value(setpoint, setpoint_value.T)
       
       # Initial values
-      opti.set_value(p, self.x0[:self.env.Nx])
-      initial_x_values = np.zeros((self.env.Nx, self.N+1))
-      initial_x_values = (self.x0[:self.env.Nx]*np.ones((self.N+1,self.env.Nx))).T  
+      opti.set_value(p, self.x0[:self.env.Nx_oracle])
+      initial_x_values = np.zeros((self.env.Nx_oracle, self.N+1))
+      initial_x_values = (self.x0[:self.env.Nx_oracle]*np.ones((self.N+1,self.env.Nx_oracle))).T  
       opti.set_initial(x, initial_x_values)
-      for i in range(self.env.Nu - self.env.Nd):     
+      for i in range(self.env.Nu - self.env.Nd_model):     
         opti.set_initial(u[i,:], self.env_params['a_space']['low'][i]*np.ones((1,self.N))) 
      
       # Silence the solver
       opts = {
       'ipopt.print_level': 0,
       'ipopt.sb': 'no',
       'print_time': 0,
-      'ipopt.print_user_options': 'no'
+      'ipopt.print_user_options': 'no',
+
       }
 
       opti.solver('ipopt', opts)
 
       # Make the opti object a function 
       M = opti.to_function('M', [p], [u[:,1]], ['p'], ['u'])
       return M
@@ -196,30 +201,30 @@
       
       regen_index = self.disturbance_index()
       
       M = self.ocp(t_step=0)
       F = self.integrator_gen()
       
       u_log = np.zeros((self.env.Nu, self.env.N))
-      x_log = np.zeros((self.env.Nx, self.env.N))
-      x = np.array(self.x0[:self.env.Nx])
+      x_log = np.zeros((self.env.Nx_oracle, self.env.N))
+      x = np.array(self.x0[:self.env.Nx_oracle])
       for i in range(self.env.N):
           if i-1 in regen_index:
             M = self.ocp(t_step=i)          
           try:
               x_log[:,i] = x
-          except:
+          except Exception:
               x_log[:,i] = x.reshape(-1)
+
           if self.env_params.get('noise', False):
               noise_percentage = self.env_params.get('noise_percentage', 0)
               try:
+                x += np.random.normal(0,1,(self.env.Nx_oracle)) * x * noise_percentage
 
-                x += np.random.normal(0,1,(self.env.Nx)) * x * noise_percentage
-
-              except:
+              except Exception:
 
-                x += np.random.normal(0,1,(self.env.Nx,1)) * x * noise_percentage
+                x += np.random.normal(0,1,(self.env.Nx_oracle,1)) * x * noise_percentage
           u = M(x).full()
           u_log[:,i] = u[0]
           x = F(x,u).full() 
       return x_log, u_log
```

### Comparing `pcgym-0.0.7/src/pcgym/pcgym.py` & `pcgym-0.0.8/src/pcgym/pcgym.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import numpy as np
-from casadi import *
-import numpy as np
 import gymnasium as gym
 from gymnasium import spaces
-from .model_classes import *
-from .policy_Evaluation import policy_eval
-from .integrator import integration_engine
+from pcgym.model_classes import cstr_ode, first_order_system_ode, multistage_extraction_ode, nonsmooth_control_ode
+from pcgym.policy_evaluation import policy_eval
+from pcgym.integrator import integration_engine
 import copy 
     
 class make_env(gym.Env):
     '''
     Class for RL-Gym Environment
     '''
     def __init__(self,env_params):
@@ -17,34 +15,36 @@
         Constructor for the class
         '''
         
         self.env_params = copy.deepcopy(env_params)
         try:
             self.normalise_a = env_params['normalise_a']
             self.normalise_o = env_params['normalise_o']
-        except:
+        except Exception:
             self.normalise_a = True
             self.normalise_o = True
         
         # Define action and observation space
         if self.normalise_a is True:
             self.action_space = spaces.Box(low = np.array([-1]*env_params['a_space']['low'].shape[0]), high = np.array([1]*env_params['a_space']['high'].shape[0]))
         else:
             self.action_space = spaces.Box(low=env_params['a_space']['low'],high = env_params['a_space']['high'])
-        
-        self.observation_space = spaces.Box(low = env_params['o_space']['low'],high = env_params['o_space']['high'])  
+            
         self.SP = env_params['SP']
         self.N = env_params['N']
         self.tsim = env_params['tsim']
         self.x0 = env_params['x0']
-
+        # Initial setup for observation space based on user-defined bounds
+        base_obs_low = env_params['o_space']['low']
+        base_obs_high = env_params['o_space']['high']
+        self.observation_space = spaces.Box(low=base_obs_low, high=base_obs_high)
 
         try :
             self.integration_method = env_params['integration_method']
-        except:
+        except Exception:
             self.integration_method = 'casadi'
 
         self.dt =  self.tsim/self.N
         self.done = False
 
         
 
@@ -73,26 +73,16 @@
 
     
 
         #Select model 
         model_mapping = {
         'cstr_ode': cstr_ode,
         'first_order_system_ode': first_order_system_ode,
-        # 'second_order_system_ode': second_order_system_ode,
-        # 'large_scale_ode': large_scale_ode,
-        # 'cstr_series_recycle_ode': cstr_series_recycle_ode,
-        # 'cstr_series_recycle_two_ode': cstr_series_recycle_two_ode,
-        # 'distillation_ode': distillation_ode,
-         'multistage_extraction_ode': multistage_extraction_ode,
-        # 'multistage_extraction_reactive_ode': multistage_extraction_reactive_ode,
-        # 'heat_ex_ode': heat_ex_ode,
-        # 'biofilm_reactor_ode': biofilm_reactor_ode,
-        # 'polymerisation_ode': polymerisation_ode,
-        # 'four_tank_ode': four_tank_ode,
-        # 'cstr_ode_jax': cstr_ode_jax,
+        'nonsmooth_control_ode': nonsmooth_control_ode,
+        'multistage_extraction_ode': multistage_extraction_ode,
         }   
 
         # Load custom model if it is provide else load the selected standard model.
         if self.env_params.get('custom_model') is not None:
             m = self.env_params.get('custom_model')
         else:
             m = model_mapping.get(env_params['model'], None)
@@ -100,43 +90,70 @@
 
 
         # Handle the case where the model is not found (do this for all)
         if self.model is None:
             raise ValueError(f"Model '{env_params['model']}' not found in model_mapping.")
         
         # Import states and controls from model info
-        self.Nx = len(self.model.info()['states'])
+        self.Nx = len(self.model.info()['states']) + len(self.SP)
+        self.Nx_oracle = len(self.model.info()['states'])
         self.Nu = len(self.model.info()['inputs'])
 
         # Disturbances
         self.disturbance_active = False
         self.Nd = 0
+        self.Nd_model = 0
         if env_params.get('disturbances') is not None:
             self.disturbance_active = True
             self.disturbances = env_params['disturbances']
-            self.Nd = len(self.model.info()['disturbances'])
-            self.Nu += self.Nd
+            self.Nd = len(self.disturbances)
+            self.Nd_model = len(self.model.info()['disturbances'])
+            self.Nu += len(self.model.info()['disturbances'])
+        
+            # Extend the state size by the number of disturbances
+            self.Nx += self.Nd
+            # user has defined disturbance_bounds within env_params
+            disturbance_low = env_params['disturbance_bounds']['low']
+            disturbance_high = env_params['disturbance_bounds']['high']
+            # Extend the observation space bounds to include disturbances
+            extended_obs_low = np.concatenate((base_obs_low, disturbance_low))
+            extended_obs_high = np.concatenate((base_obs_high, disturbance_high))
+            # Define the extended observation space
+            self.observation_space = spaces.Box(low=extended_obs_low, high=extended_obs_high, dtype=np.float32)
+          
         
         
-       
-    
     def reset(self, seed=None, **kwargs):  # Accept arbitrary keyword arguments
         """
         Resets the state of the system 
 
         Returns the state of the system
         """
         self.t = 0
         self.int_eng = integration_engine(make_env,self.env_params)
         
         state = copy.deepcopy(self.env_params['x0'])
-        r_init = self.reward_fn(state,False)
         
-        self.done = False
+        # If disturbances are active, expand the initial state with disturbances
+        if self.disturbance_active:
+            initial_disturbances = [] 
+            for k in self.model.info()['disturbances']:
+                if k in self.disturbances:
+                    initial_disturbances.append(self.disturbances[k][0])
+              
+            
+            # Append initial disturbances to the state
+            state = np.concatenate((state, initial_disturbances))
+
         self.state = state
+
+        r_init = self.reward_fn(state,False)
+
+        self.done = False
+
         if self.normalise_o is True:
             self.normstate = 2 * (self.state - self.observation_space.low) / (self.observation_space.high - self.observation_space.low) - 1
             return self.normstate, {'r_init':r_init}
         else:
             return self.state,{'r_init':r_init}
     
     def step(self, action):
@@ -164,28 +181,38 @@
         uk = np.zeros(self.Nu)
         if self.normalise_a is True:
             action = (action + 1)*(self.env_params['a_space']['high'] - self.env_params['a_space']['low'])/2 + self.env_params['a_space']['low']
         
         # Add disturbance to control vector
         if self.disturbance_active:
             uk[:self.Nu-len(self.model.info()['disturbances'])] = action # Add action to control vector
-            for i, k in enumerate(self.model.info()['disturbances'], start=0):
+            disturbance_values = []
+            disturbance_values_state = []
+            for i, k in enumerate(self.model.info()['disturbances'], start=0):     
                 if k in self.disturbances:
-                    uk[self.Nu-self.Nd+i] = self.disturbances[k][self.t] # Add disturbance to control vector
+                    current_disturbance_value = self.disturbances[k][self.t]
+                    uk[self.Nu-self.Nd_model+i] = self.disturbances[k][self.t] # Add disturbance to control vector
+                    disturbance_values_state.append(current_disturbance_value)
+                    disturbance_values.append(current_disturbance_value)
                 else:
-                    uk[self.Nu-self.Nd+i] = self.model.info()['parameters'][str(k)] # if there is no disturbance at this timestep, use the default value
+                    default_value = self.model.info()['parameters'][str(k)]
+                    uk[self.Nu-self.Nd_model+i] = self.model.info()['parameters'][str(k)] # if there is no disturbance at this timestep, use the default value
+                    disturbance_values.append(default_value)
+      
+            # Update the state vector with current disturbance values
+            self.state[self.Nx_oracle+len(self.SP):] = disturbance_values_state
         else:
             uk = action  # Add action to control vector
 
         # Simulate one timestep
         if self.integration_method == 'casadi':
             Fk = self.int_eng.casadi_step(self.state,uk)
-            self.state[:self.Nx] = np.array(Fk['xf'].full()).reshape(self.Nx)
+            self.state[:self.Nx_oracle] = np.array(Fk['xf'].full()).reshape(self.Nx_oracle)
         elif self.integration_method == 'jax':
-            self.state[:self.Nx] = self.int_eng.jax_step(self.state,uk)
+            self.state[:self.Nx_oracle] = self.int_eng.jax_step(self.state,uk)
 
         # Check if constraints are violated
         constraint_violated = False
         if self.constraint_active or self.custom_constraint_active:
             constraint_violated = self.constraint_check(self.state,uk)
         
         # Compute reward
@@ -204,15 +231,15 @@
     
         if self.t == self.N:
             self.done = True
       
         # add noise to state
         if self.env_params.get('noise', False):
             noise_percentage = self.env_params.get('noise_percentage', 0)
-            self.state[:self.Nx] += np.random.normal(0, 1, self.Nx) * self.state[:self.Nx] * noise_percentage
+            self.state[:self.Nx_oracle] += np.random.normal(0, 1, self.Nx_oracle) * self.state[:self.Nx_oracle] * noise_percentage
 
 
         if self.normalise_o is True:
             self.normstate = 2 * (self.state - self.observation_space.low) / (self.observation_space.high - self.observation_space.low) - 1
             return self.normstate, rew, self.done, False, self.info
         else:
             return self.state, rew, self.done, False, self.info
@@ -292,29 +319,52 @@
         elif self.custom_constraint_active:
             constraint_violated = custom_con_vio
 
         self.done = self.done_on_constraint 
         return constraint_violated
             
               
+    def get_rollouts(self, policies, reps, oracle = False, dist_reward = False, MPC_params = False, cons_viol = False):
+        '''
+        Plot the rollout of the given policy.
+
+        Parameters:
+        - policies: dictionary of policies to evaluate
+        - reps: The number of rollouts to perform.
+        - oracle: Whether to use an oracle model for evaluation. Default is False.
+        - dist_reward: Whether to use reward distribution for plotting. Default is False.
+        - MPC_params: Whether to use MPC parameters. Default is False.
+        '''
+        # construct evaluator
+        evaluator = policy_eval(make_env, policies, reps, self.env_params, oracle, MPC_params)
+        # generate rollouts 
+        data = evaluator.get_rollouts()
+        # return evaluator and data
+        return evaluator, data
 
-   
 
-    def plot_rollout(self, policy, reps, oracle = False, dist_reward = False, MPC_params = False, cons_viol = False):
+    def plot_rollout(self, policies, reps, oracle = False, dist_reward = False, MPC_params = False, cons_viol = False):
         '''
         Plot the rollout of the given policy.
 
         Parameters:
-        - policy: The policy to evaluate.
+        - policies: dictionary of policies to evaluate
         - reps: The number of rollouts to perform.
         - oracle: Whether to use an oracle model for evaluation. Default is False.
         - dist_reward: Whether to use reward distribution for plotting. Default is False.
         - MPC_params: Whether to use MPC parameters. Default is False.
         '''
-        policy_eval(make_env,policy,reps,self.env_params,oracle,MPC_params).plot_rollout(dist_reward, cons_viol)
+        # construct evaluator
+        evaluator = policy_eval(make_env, policies, reps, self.env_params, oracle, MPC_params, cons_viol)
+        # generate rollouts 
+        data = evaluator.get_rollouts()
+        # plot data from rollouts via the evaluator method
+        evaluator.plot_data(data, dist_reward)
+        # return constructed evaluator and data
+        return evaluator, data
```

### Comparing `pcgym-0.0.7/src/pcgym/policy_Evaluation.py` & `pcgym-0.0.8/src/pcgym/policy_evaluation.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,192 +9,215 @@
 
     Inputs: Environment, policy and number of policy repitions
 
     Outputs: Plots of states/control/constraints/setpoints (complete),
              return distribution (incomplete), expected return (incomplete),
              oracle trajectories (incomplete) and lower confidence bounds (incomplete)
     '''
-    def __init__(self,make_env,policy,reps,env_params, oracle = False, MPC_params = False):
+    def __init__(self,make_env,policies,reps,env_params, oracle = False, MPC_params = False, cons_viol = False):
         self.make_env = make_env
         self.env_params = env_params
         self.env = make_env(env_params)
-        
-        self.policy = policy
+        self.policies = policies
+        self.n_pi = len(policies)
         self.reps = reps
         self.oracle = oracle
+        self.cons_viol = cons_viol
  
         self.MPC_params  = MPC_params  
         
 
-    def rollout(self):
+    def rollout(self,policy_i):
         '''
         Rollout the policy for N steps and return the total reward, states and actions
 
         Input:
             policy - policy to be rolled out
 
         Outputs:
             total_reward - total reward obtained
             states - states obtained from rollout
             actions - actions obtained from rollout
 
         '''
         
         total_reward = 0
-        s_rollout = np.zeros((self.env.x0.shape[0], self.env.N))
+        s_rollout = np.zeros((self.env.Nx, self.env.N))
         actions = np.zeros((self.env.env_params['a_space']['low'].shape[0], self.env.N))
         
         o, r = self.env.reset()
         total_reward = r['r_init']
-        s_rollout[:,0] = (o + 1)*(self.env.env_params['o_space']['high'] - self.env.env_params['o_space']['low'])/2 + self.env.env_params['o_space']['low']
+        s_rollout[:,0] = (o + 1)*(self.env.observation_space.high - self.env.observation_space.low)/2 + self.env.observation_space.low
         for i in range(self.env.N-1):
-            a, _s = self.policy.predict(o, deterministic = True) # Rollout with a deterministic policy
+            a, _s = policy_i.predict(o, deterministic = True) # Rollout with a deterministic policy
             o, r, term, trunc, info = self.env.step(a)
             
             actions[:, i] = (a + 1)*(self.env.env_params['a_space']['high'] - self.env.env_params['a_space']['low'])/2 + self.env.env_params['a_space']['low']
-            s_rollout[:, i+1] = (o + 1)*(self.env.env_params['o_space']['high'] - self.env.env_params['o_space']['low'])/2 + self.env.env_params['o_space']['low']
+            s_rollout[:, i+1] = (o + 1)*(self.env.observation_space.high - self.env.observation_space.low)/2 + self.env.observation_space.low
+            
             total_reward += r
 
         if self.env.constraint_active:
             cons_info = info['cons_info']
         else:
             cons_info = np.zeros((1,self.env.N,1))
-        a, _s = self.policy.predict(o)
+        a, _s = policy_i.predict(o, deterministic = True)
         actions[:,self.env.N-1] = (a + 1)*(self.env.env_params['a_space']['high'] - self.env.env_params['a_space']['low'])/2 + self.env.env_params['a_space']['low']
         
         return total_reward, s_rollout, actions,cons_info
     
-    def plot_rollout(self, reward_dist = False, cons_viol = False):
+    def get_rollouts(self):
         '''
         Function to plot the rollout of the policy
 
         Inputs:
             policy - policy to be rolled out
             reps - number of rollouts to be performed
 
         Outputs:
             Plot of states and actions with setpoints and constraints if they exist]
 
         '''
         data = {}
         action_space_shape = self.env.env_params['a_space']['low'].shape[0]
-        num_states = self.env.x0.shape[0]
+        num_states = self.env.Nx
         
-        states = np.zeros((num_states, self.env.N, self.reps))
-        actions = np.zeros((action_space_shape, self.env.N, self.reps))
-        rew = np.zeros((1, self.reps))
+
 
         # Collect Oracle data
         if self.oracle:
             r_opt = np.zeros((1,self.reps))
-            x_opt = np.zeros((self.env.Nx, self.env.N, self.reps))
+            x_opt = np.zeros((self.env.Nx_oracle, self.env.N, self.reps))
             u_opt = np.zeros((self.env.Nu, self.env.N, self.reps))
             oracle_instance = oracle(self.make_env, self.env_params,self.MPC_params)
             for i in range(self.reps):
                 x_opt[:, :, i], u_opt[:, :, i] = oracle_instance.mpc()
                 for k in self.env.SP:
                     state_i = self.env.model.info()['states'].index(k)
                     r_scale = self.env_params.get('r_scale', {})
                     r_opt[:,i] += np.sum((x_opt[state_i,:,i] - self.env.SP[k])**2)*-1*r_scale.get(k, 1)
-            data.update({'r_opt':r_opt,'x_opt':x_opt,'u_opt':u_opt})   
-     
-        try:
-            cons_info = np.zeros((self.env.n_con,self.env.N,1,self.reps))
-        except:
-            cons_info = np.zeros((1,self.env.N,1,self.reps))
-
-        # Collect RL rollouts
-        for r_i in range(self.reps):
-            rew[:, r_i], states[:, :, r_i], actions[:, :, r_i], cons_info[:,:,:,r_i]= self.rollout()
-        data.update({'r_RL':rew,'x_RL':states,'u_RL':actions})
-        if self.env.constraint_active:
-            data.update({'cons_viol_RL':cons_info})
+            data.update({'oracle': {'r':r_opt,'x':x_opt,'u':u_opt}})   
+           
+      
+
+        # Collect RL rollouts for all policies
+        for pi_name, pi_i in self.policies.items():
+            states = np.zeros((num_states, self.env.N, self.reps))
+            actions = np.zeros((action_space_shape, self.env.N, self.reps))
+            rew = np.zeros((1, self.reps))
+            try:
+                cons_info = np.zeros((self.env.n_con,self.env.N,1,self.reps))
+            except Exception:
+                cons_info = np.zeros((1,self.env.N,1,self.reps))
+            for r_i in range(self.reps):
+                rew[:, r_i], states[:, :, r_i], actions[:, :, r_i], cons_info[:,:,:,r_i] = self.rollout(pi_i)
+            data.update({pi_name:{'r' :rew,
+                         'x' : states,
+                         'u' : actions}})
+            if self.env.constraint_active:
+                data[pi_name].update({'g' : cons_info})
+        self.data = data
+        return data
 
+    def plot_data(self, data, reward_dist = False):
         t = np.linspace(0, self.env.tsim, self.env.N)
         len_d = 0
 
         if self.env.disturbance_active:
             len_d = len(self.env.model.info()['disturbances'])
 
-        plt.figure(figsize=(10, 2*(self.env.Nx+self.env.Nu+len_d)))
-        for i in range(self.env.Nx):
-            plt.subplot(self.env.Nx + self.env.Nu+len_d,1,i+1)
-            plt.plot(t, np.median(states[i,:,:],axis=1), color='tab:red', lw=3,label = self.env.model.info()['states'][i])
-            plt.gca().fill_between(t, np.min(states[i,:,:],axis=1), np.max(states[i,:,:],axis=1), color='tab:red', alpha=0.2, edgecolor = 'none')
+        col = ['tab:red','tab:purple','tab:olive','tab:gray','tab:cyan']
+        if self.n_pi > len(col):
+            raise ValueError(f"Number of policies ({self.n_pi}) is greater than the number of available colors ({len(col)})")
+
+
+        plt.figure(figsize=(10, 2*(self.env.Nx_oracle+self.env.Nu-self.env.Nd)))
+        for i in range(self.env.Nx_oracle):
+            plt.subplot(self.env.Nx_oracle + self.env.Nu-self.env.Nd,1,i+1)
+            for ind, (pi_name, pi_i) in enumerate(self.policies.items()):
+                plt.plot(t, np.median(data[pi_name]['x'][i,:,:], axis=1), color=col[ind], lw=3, label = self.env.model.info()['states'][i] + ' (' + pi_name + ')' )
+                plt.gca().fill_between(t, np.min(data[pi_name]['x'][i,:,:], axis=1), np.max(data[pi_name]['x'][i,:,:], axis=1), color=col[ind], alpha=0.2, edgecolor = 'none')
             if self.oracle:
-                plt.plot(t, np.median(x_opt[i,:,:],axis=1), color='tab:blue', lw=3,label = 'Oracle '+ self.env.model.info()['states'][i])
-                plt.gca().fill_between(t, np.min(x_opt[i,:,:],axis=1), np.max(x_opt[i,:,:],axis=1), color='tab:blue', alpha=0.2,edgecolor = 'none' )
+                plt.plot(t, np.median(data['oracle']['x'][i,:,:],axis=1), color='tab:blue', lw=3,label = 'Oracle '+ self.env.model.info()['states'][i])
+                plt.gca().fill_between(t, np.min(data['oracle']['x'][i,:,:],axis=1), np.max(data['oracle']['x'][i,:,:],axis=1), color='tab:blue', alpha=0.2,edgecolor = 'none' )
             if self.env.model.info()['states'][i] in self.env.SP:
                 plt.step(t, self.env.SP[self.env.model.info()['states'][i]],where = 'post', color = 'black', linestyle = '--', label='Set Point')
             if self.env.constraint_active:
                 if self.env.model.info()['states'][i] in self.env.constraints:
                     plt.hlines(self.env.constraints[self.env.model.info()['states'][i]], 0, self.env.tsim, color = 'black',label='Constraint')
             plt.ylabel(self.env.model.info()['states'][i])
             plt.xlabel('Time (min)')
             plt.legend(loc='best')
             plt.grid('True')
             plt.xlim(min(t), max(t))
 
         for j in range(self.env.Nu-len_d):
-            plt.subplot(self.env.Nx+self.env.Nu+len_d,1,j+self.env.Nx+1)
-            plt.step(t, np.median(actions[j,:,:],axis=1), color='tab:red', lw=3, label=self.env.model.info()['inputs'][j])
+            plt.subplot(self.env.Nx_oracle + self.env.Nu - self.env.Nd, 1, j+self.env.Nx_oracle+1)
+            for ind, (pi_name, pi_i) in enumerate(self.policies.items()):
+                plt.step(t, np.median(data[pi_name]['u'][j,:,:], axis=1), color=col[ind], lw=3, label=self.env.model.info()['inputs'][j] + ' (' + pi_name + ')')
             if self.oracle:
-                plt.step(t, np.median(u_opt[j,:,:],axis=1), color='tab:blue', lw=3, label='Oracle '+ str(self.env.model.info()['inputs'][j]))
+                plt.step(t, np.median(data['oracle']['u'][j,:,:],axis=1), color='tab:blue', lw=3, label='Oracle '+ str(self.env.model.info()['inputs'][j]))
             if self.env.constraint_active:
                 for con_i in self.env.constraints:
                     if self.env.model.info()['inputs'][j] == con_i:
                         plt.hlines(self.env.constraints[self.env.model.info()['inputs'][j]], 0,self.env.tsim,'black',label='Constraint')
             plt.ylabel(self.env.model.info()['inputs'][j])
             plt.xlabel('Time (min)')
             plt.legend(loc='best')
             plt.grid('True')
             plt.xlim(min(t), max(t))
 
         if self.env.disturbance_active:
-            for i, k in enumerate(self.env.disturbances.keys()):
+            for k in self.env.disturbances.keys():
+                i = 1
                 if self.env.disturbances[k].any() is not None:
-                    plt.subplot(self.env.Nx+self.env.Nu+len_d,1,i+self.env.Nx+self.env.Nu-len_d+1)
+                    plt.subplot(self.env.Nx_oracle+self.env.Nu-self.env.Nd,1,i+j+self.env.Nx_oracle+1)
                     plt.step(t, self.env.disturbances[k], color = 'tab:orange',label=k)
                     plt.xlabel('Time (min)')
                     plt.ylabel(k)
                     plt.xlim(min(t), max(t))
+                    i += 1 
         plt.tight_layout()
         plt.show()
-        if cons_viol:
+        
+        if self.cons_viol:
             plt.figure(figsize=(12, 3 * self.env.n_con))
             con_i = 0
             for i, con in enumerate(self.env.constraints):
                 for j in range(len(self.env.constraints[str(con)])):
                     plt.subplot(self.env.n_con,1,con_i+1)
                     plt.title(f'{con} Constraint')
-                    plt.step(t, np.sum(cons_info[con_i,:,:,:],axis=2), color = 'tab:green', label = f'{con} Violation (Sum over Repetitions)')
+                    for ind, (pi_name, pi_i) in enumerate(self.policies.items()):
+                        plt.step(t, np.sum(data[pi_name]['g'][con_i,:,:,:],axis=2), color = col[ind], label = f'{con} ({pi_name}) Violation (Sum over Repetitions)')
                     plt.grid('True')
                     plt.xlabel('Time (min)')
                     plt.ylabel(con)
                     plt.xlim(min(t), max(t))
                     plt.legend(loc = 'best')
                     con_i += 1
             plt.tight_layout()
             plt.show()
 
         if reward_dist:
-            min_val = min(r_opt.min(), rew.min())
-            max_val = max(r_opt.max(), rew.max())
-            bins = np.linspace(min_val, max_val, 50)  
-
             plt.figure(figsize=(12, 8))  
             plt.grid(True, linestyle='--', alpha=0.6)  
+            all_data = np.concatenate([data[key]['r'].flatten() for key in data.keys()])
+
+            min_value = np.min(all_data)
+            max_value = np.max(all_data)
 
+            bins = np.linspace(min_value, max_value, self.reps)
             if self.oracle:
-                plt.hist(r_opt.flatten(), bins=bins, color='tab:blue', alpha=0.5, label='Oracle', edgecolor='black')  
-            plt.hist(rew.flatten(), bins=bins, color='tab:red', alpha=0.5, label='RL Algorithm', edgecolor='black')  
+                plt.hist(data['oracle']['r'].flatten(), bins=bins, color='tab:blue', alpha=0.5, label='Oracle', edgecolor='black')  
+            for ind, (pi_name, pi_i) in enumerate(self.policies.items()):
+                plt.hist(data[pi_name]['r'].flatten(), bins=bins, color=col[ind], alpha=0.5, label=pi_name, edgecolor='black')  
 
             plt.xlabel('Return', fontsize=14)  
             plt.ylabel('Frequency', fontsize=14)  
             plt.title('Distribution of Expected Return', fontsize=16)  
             plt.legend(fontsize=12)  
 
             plt.show()
 
-        return data
+        return
```

### Comparing `pcgym-0.0.7/src/pcgym.egg-info/PKG-INFO` & `pcgym-0.0.8/src/pcgym.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcgym
-Version: 0.0.7
+Version: 0.0.8
 Summary: Reinforcement learning suite of process control problems.
 Author-email: Max Bloor <max.bloor@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Maximilian Bloor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,14 +47,19 @@
 Requires-Dist: cloudpickle
 Requires-Dist: matplotlib
 Requires-Dist: gymnasium
 Requires-Dist: casadi
 Requires-Dist: jax[cpu]
 Requires-Dist: equinox
 Requires-Dist: diffrax
+Provides-Extra: optional
+Requires-Dist: jupyterlab; extra == "optional"
+Requires-Dist: torch; extra == "optional"
+Requires-Dist: stable-baselines3; extra == "optional"
+Requires-Dist: mkdocs-material; extra == "optional"
 
 <h1 align="center">
   <a href="https://github.com/MaximilianB2/pc-gym/blob/main/docs/img/pc-gym-blue-Ai.png">
     <img src="https://github.com/MaximilianB2/pc-gym/blob/main/docs/img/pc-gym-blue-Ai.png"/></a><br>
   <b>Reinforcement learning environments for process control </b><br>
 </h1>
 <p align="center">
@@ -65,14 +70,19 @@
 </p>
 
 
 ## Quick start ⚡
 Setup a CSTR environment with a setpoint change
 
 ```python 
+import pcgym
+
+# Simulation variables
+nsteps = 100
+T = 25
 
 # Setpoint
 SP = {'Ca': [0.85 for i in range(int(nsteps/2))] + [0.9 for i in range(int(nsteps/2))]} 
 
 # Action and observation Space
 action_space = {'low': np.array([295]), 'high': np.array([302])}
 observation_space = {'low': np.array([0.7,300,0.8]),'high': np.array([1,350,0.9])}
@@ -112,26 +122,33 @@
 pip install pcgym
 ```
 
 ## Examples
 
 TODO: Link example notebooks here
 
-## Implemented Process Control Environments
-
-TODO: Add table of environments
+## Implemented Process Control Environments 🎛️
 
-## Other Great Gyms 🔍
+|          Environment          | Reference | Source | Documentation |
+|:-----------------------------:|:---------:|:------:|---------------|
+|              CSTR             | [Hedengren, 2022](https://github.com/APMonitor/pdc/blob/master/CSTR_Control.ipynb)     | [Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/model_classes.py)      |               |
+|       First Order Sytem       |      N/A  | [Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/model_classes.py)        |               |
+| Multistage Extraction Column  |  [Ingham et al, 2007 (pg 471)](https://onlinelibrary.wiley.com/doi/book/10.1002/9783527614219)         | [Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/model_classes.py)        |               |
 
-TODO: Link other gyms such as Jumanji, safety gymnasium etc.
 
+ 
 ## Citing `pc-gym`
 If you use `pc-gym` in your research, please cite using the following 
 ```
 @software{pcgym2024,
   author = {Max Bloor and ...},
   title = {{pc-gym}: Reinforcement Learning Envionments for Process Control},
   url = {https://github.com/MaximilianB2/pc-gym},
   version = {0.0.4},
   year = {2024},
 }
 ```
+
+## Other Great Gyms 🔍
+- ✨[safe-control-gym](https://github.com/utiasDSL/safe-control-gym) 
+- ✨[safety-gymnasium](https://github.com/PKU-Alignment/safety-gymnasium)
+- ✨[gymnax](https://github.com/RobertTLange/gymnax)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pcgym Version: 0.0.7 Summary: Reinforcement
+Metadata-Version: 2.1 Name: pcgym Version: 0.0.8 Summary: Reinforcement
 learning suite of process control problems. Author-email: Max Bloor
 gmail.com> License: MIT License Copyright (c) 2024 Maximilian Bloor Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -24,36 +24,50 @@
 :: English Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
 Scientific/Engineering :: Information Analysis Classifier: Topic :: Scientific/
 Engineering :: Mathematics Requires-Python: ~=3.10 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: ruff Requires-Dist: numpy
 Requires-Dist: tqdm Requires-Dist: cloudpickle Requires-Dist: matplotlib
 Requires-Dist: gymnasium Requires-Dist: casadi Requires-Dist: jax[cpu]
-Requires-Dist: equinox Requires-Dist: diffrax
+Requires-Dist: equinox Requires-Dist: diffrax Provides-Extra: optional
+Requires-Dist: jupyterlab; extra == "optional" Requires-Dist: torch; extra ==
+"optional" Requires-Dist: stable-baselines3; extra == "optional" Requires-Dist:
+mkdocs-material; extra == "optional"
 ************ _[[_hh_tt_tt_pp_ss_::_//_//_gg_ii_tt_hh_uu_bb_.._cc_oo_mm_//_MM_aa_xx_ii_mm_ii_ll_ii_aa_nn_BB_22_//_pp_cc_--_gg_yy_mm_//_bb_ll_oo_bb_//_mm_aa_ii_nn_//_dd_oo_cc_ss_//_ii_mm_gg_//_pp_cc_--_gg_yy_mm_--_bb_ll_uu_ee_--
                                     _AA_ii_.._pp_nn_gg_]]
             RReeiinnffoorrcceemmeenntt lleeaarrnniinngg eennvviirroonnmmeennttss ffoorr pprroocceessss ccoonnttrrooll
                                      ************
   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-_3_._1_0_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
                            _b_a_d_g_e_/_l_i_c_e_n_s_e_-_M_I_T_-_o_r_a_n_g_e_]
-## Quick start â¡ Setup a CSTR environment with a setpoint change ```python #
-Setpoint SP = {'Ca': [0.85 for i in range(int(nsteps/2))] + [0.9 for i in range
-(int(nsteps/2))]} # Action and observation Space action_space = {'low':
-np.array([295]), 'high': np.array([302])} observation_space = {'low': np.array(
-[0.7,300,0.8]),'high': np.array([1,350,0.9])} # Construct the environment
-parameter dictionary env_params = { 'N': nsteps, # Number of time steps 'tsim':
-T, # Simulation Time 'SP' :SP, 'o_space' : observation_space, 'a_space' :
-action_space, 'x0': np.array([0.8, 330, 0.8]), # Initial conditions [Ca, T,
-Ca_SP] 'model': 'cstr_ode', # Select the model } # Create environment env =
-pcgym.make_env(env_params) # Reset the environment obs, state = env.reset() #
-Sample a random action action = env.action_space.sample() # Perform a step in
-the environment obs, rew, done, term, info = env.step(action) ``` ##
-Documentation You can read the full documentation [here](https://
-maximilianb2.github.io/pc-gym/)! ## Installation â³ The latest pc-gym version
-can be installed from PyPI: ```bash pip install pcgym ``` ## Examples TODO:
-Link example notebooks here ## Implemented Process Control Environments TODO:
-Add table of environments ## Other Great Gyms ð TODO: Link other gyms such
-as Jumanji, safety gymnasium etc. ## Citing `pc-gym` If you use `pc-gym` in
-your research, please cite using the following ``` @software{pcgym2024, author
-= {Max Bloor and ...}, title = {{pc-gym}: Reinforcement Learning Envionments
-for Process Control}, url = {https://github.com/MaximilianB2/pc-gym}, version =
-{0.0.4}, year = {2024}, } ```
+## Quick start â¡ Setup a CSTR environment with a setpoint change ```python
+import pcgym # Simulation variables nsteps = 100 T = 25 # Setpoint SP = {'Ca':
+[0.85 for i in range(int(nsteps/2))] + [0.9 for i in range(int(nsteps/2))]} #
+Action and observation Space action_space = {'low': np.array([295]), 'high':
+np.array([302])} observation_space = {'low': np.array([0.7,300,0.8]),'high':
+np.array([1,350,0.9])} # Construct the environment parameter dictionary
+env_params = { 'N': nsteps, # Number of time steps 'tsim':T, # Simulation Time
+'SP' :SP, 'o_space' : observation_space, 'a_space' : action_space, 'x0':
+np.array([0.8, 330, 0.8]), # Initial conditions [Ca, T, Ca_SP] 'model':
+'cstr_ode', # Select the model } # Create environment env = pcgym.make_env
+(env_params) # Reset the environment obs, state = env.reset() # Sample a random
+action action = env.action_space.sample() # Perform a step in the environment
+obs, rew, done, term, info = env.step(action) ``` ## Documentation You can read
+the full documentation [here](https://maximilianb2.github.io/pc-gym/)! ##
+Installation â³ The latest pc-gym version can be installed from PyPI: ```bash
+pip install pcgym ``` ## Examples TODO: Link example notebooks here ##
+Implemented Process Control Environments ðï¸ | Environment | Reference |
+Source | Documentation | |:-----------------------------:|:---------:|:------:
+|---------------| | CSTR | [Hedengren, 2022](https://github.com/APMonitor/pdc/
+blob/master/CSTR_Control.ipynb) | [Source](https://github.com/MaximilianB2/pc-
+gym/blob/main/src/pcgym/model_classes.py) | | | First Order Sytem | N/A |
+[Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/
+model_classes.py) | | | Multistage Extraction Column | [Ingham et al, 2007 (pg
+471)](https://onlinelibrary.wiley.com/doi/book/10.1002/9783527614219) |
+[Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/
+model_classes.py) | | ## Citing `pc-gym` If you use `pc-gym` in your research,
+please cite using the following ``` @software{pcgym2024, author = {Max Bloor
+and ...}, title = {{pc-gym}: Reinforcement Learning Envionments for Process
+Control}, url = {https://github.com/MaximilianB2/pc-gym}, version = {0.0.4},
+year = {2024}, } ``` ## Other Great Gyms ð - â¨[safe-control-gym](https://
+github.com/utiasDSL/safe-control-gym) - â¨[safety-gymnasium](https://
+github.com/PKU-Alignment/safety-gymnasium) - â¨[gymnax](https://github.com/
+RobertTLange/gymnax)
```

