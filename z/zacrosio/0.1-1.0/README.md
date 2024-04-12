# Comparing `tmp/zacrosio-0.1.tar.gz` & `tmp/zacrosio-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zacrosio-0.1.tar", last modified: Wed Apr 10 18:19:26 2024, max compression
+gzip compressed data, was "zacrosio-1.0.tar", last modified: Fri Apr 12 14:34:21 2024, max compression
```

## Comparing `zacrosio-0.1.tar` & `zacrosio-1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 install    (505) staff       (20)        0 2024-04-10 18:19:26.798982 zacrosio-0.1/
--rw-r--r--   0 install    (505) staff       (20)     1076 2024-04-10 17:13:06.000000 zacrosio-0.1/LICENSE.txt
--rw-r--r--   0 install    (505) staff       (20)      386 2024-04-10 18:19:26.798480 zacrosio-0.1/PKG-INFO
--rw-r--r--   0 install    (505) staff       (20)     3312 2024-04-10 18:11:19.000000 zacrosio-0.1/README.md
--rw-r--r--   0 install    (505) staff       (20)       79 2024-04-10 18:19:26.803706 zacrosio-0.1/setup.cfg
--rw-r--r--   0 install    (505) staff       (20)      484 2024-04-10 18:16:19.000000 zacrosio-0.1/setup.py
-drwxr-xr-x   0 install    (505) staff       (20)        0 2024-04-10 18:19:26.779986 zacrosio-0.1/zacrosio/
--rw-r--r--   0 install    (505) staff       (20)        0 2024-04-10 17:11:33.000000 zacrosio-0.1/zacrosio/__init__.py
--rw-r--r--   0 install    (505) staff       (20)     3852 2024-04-10 17:40:23.000000 zacrosio-0.1/zacrosio/input_functions.py
--rw-r--r--   0 install    (505) staff       (20)     7179 2024-04-10 17:43:00.000000 zacrosio-0.1/zacrosio/kmc_job.py
-drwxr-xr-x   0 install    (505) staff       (20)        0 2024-04-10 18:19:26.797527 zacrosio-0.1/zacrosio.egg-info/
--rw-r--r--   0 install    (505) staff       (20)      386 2024-04-10 18:19:26.000000 zacrosio-0.1/zacrosio.egg-info/PKG-INFO
--rw-r--r--   0 install    (505) staff       (20)      268 2024-04-10 18:19:26.000000 zacrosio-0.1/zacrosio.egg-info/SOURCES.txt
--rw-r--r--   0 install    (505) staff       (20)        1 2024-04-10 18:19:26.000000 zacrosio-0.1/zacrosio.egg-info/dependency_links.txt
--rw-r--r--   0 install    (505) staff       (20)        7 2024-04-10 18:19:26.000000 zacrosio-0.1/zacrosio.egg-info/requires.txt
--rw-r--r--   0 install    (505) staff       (20)        9 2024-04-10 18:19:26.000000 zacrosio-0.1/zacrosio.egg-info/top_level.txt
+drwxr-xr-x   0 install    (505) staff       (20)        0 2024-04-12 14:34:21.025378 zacrosio-1.0/
+-rw-r--r--   0 install    (505) staff       (20)     1076 2024-04-10 17:13:06.000000 zacrosio-1.0/LICENSE.txt
+-rw-r--r--   0 install    (505) staff       (20)     4898 2024-04-12 14:34:21.024619 zacrosio-1.0/PKG-INFO
+-rw-r--r--   0 install    (505) staff       (20)     4473 2024-04-11 16:26:14.000000 zacrosio-1.0/README.md
+-rw-r--r--   0 install    (505) staff       (20)       79 2024-04-12 14:34:21.027182 zacrosio-1.0/setup.cfg
+-rw-r--r--   0 install    (505) staff       (20)      621 2024-04-12 14:33:46.000000 zacrosio-1.0/setup.py
+drwxr-xr-x   0 install    (505) staff       (20)        0 2024-04-12 14:34:21.011122 zacrosio-1.0/zacrosio/
+-rw-r--r--   0 install    (505) staff       (20)        0 2024-04-12 11:04:42.000000 zacrosio-1.0/zacrosio/__init__.py
+-rw-r--r--   0 install    (505) staff       (20)     3852 2024-04-11 13:34:55.000000 zacrosio-1.0/zacrosio/input_functions.py
+-rw-r--r--   0 install    (505) staff       (20)     6001 2024-04-11 16:26:14.000000 zacrosio-1.0/zacrosio/kmc_job.py
+drwxr-xr-x   0 install    (505) staff       (20)        0 2024-04-12 14:34:21.023784 zacrosio-1.0/zacrosio.egg-info/
+-rw-r--r--   0 install    (505) staff       (20)     4898 2024-04-12 14:34:20.000000 zacrosio-1.0/zacrosio.egg-info/PKG-INFO
+-rw-r--r--   0 install    (505) staff       (20)      268 2024-04-12 14:34:20.000000 zacrosio-1.0/zacrosio.egg-info/SOURCES.txt
+-rw-r--r--   0 install    (505) staff       (20)        1 2024-04-12 14:34:20.000000 zacrosio-1.0/zacrosio.egg-info/dependency_links.txt
+-rw-r--r--   0 install    (505) staff       (20)       13 2024-04-12 14:34:20.000000 zacrosio-1.0/zacrosio.egg-info/requires.txt
+-rw-r--r--   0 install    (505) staff       (20)        9 2024-04-12 14:34:20.000000 zacrosio-1.0/zacrosio.egg-info/top_level.txt
```

### Comparing `zacrosio-0.1/LICENSE.txt` & `zacrosio-1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zacrosio-0.1/zacrosio/input_functions.py` & `zacrosio-1.0/zacrosio/input_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 k_eV = physical_constants["Boltzmann constant in eV/K"][0]
 atomic_mass = physical_constants["atomic mass constant"][0]
 
 
 def write_header(path):
     with open(path, 'w') as infile:
         infile.write('############################################################################\n')
-        infile.write('# Zacros Input File generated with the ZacrosIOTools                       #\n')
+        infile.write('# Zacros Input File generated with the ZacrosIO                            #\n')
         infile.write('# https://github.com/hprats/ZacrosIO                                       #\n')
         infile.write('#                                                                          #\n')
         infile.write('# Hector Prats, PhD                                                        #\n')
         infile.write('############################################################################\n\n')
 
 
 def get_q_vib(T, vib_list):
```

### Comparing `zacrosio-0.1/zacrosio/kmc_job.py` & `zacrosio-1.0/zacrosio/kmc_job.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,95 +1,91 @@
 import os
-import pandas as pd
 from random import randint
 from zacrosio.input_files.energetics_input import EnergeticModel
 from zacrosio.input_files.mechanism_input import ReactionModel
 from zacrosio.input_files.lattice_input import LatticeModel
 from zacrosio.input_functions import write_header
-from zacrosio.read_functions import read_file, check_finished, get_data_from_general_output
-from zacrosio.plot_functions import plt_production, plt_tof
 
 
 class NewKMCJob:
     """A class that represents a new KMC job with ZACROS.
 
-        Attributes: path (str): The path of the job including the job name. Will be used as the name of the folder.
-        simulation_tags (dict): A dictionary including keywords relatred to the frequency of sampling and stopping
-        criteria, for the simulation_input.dat.
-        df_mechanism: A Pandas dataframe including the information for the mechanism_input.dat.
-        df_energetics: A Pandas dataframe including the information for the energetics_input.dat. lattice_path (str):
-        The path of the lattice_input.dat (already created).
-
-        Example:
-        >>> import pandas as pd
-        >>> from zacrosio.kmc_job import NewKMCJob
-        >>>
-        >>> my_job = NewKMCJob(
-        >>>     df_gas=pd.read_csv("gas_data.csv", index_col=0),
-        >>>     df_mechanism=pd.read_csv("mechanism_data.csv", index_col=0),
-        >>>     df_energetics=pd.read_csv("energetics_data.csv", index_col=0),
-        >>>     lattice_path="lattice_input.dat")
-        >>>
-        >>> simulation_tags = {'snapshots': 'on time 5.e-1', 'process_statistics': 'on time 1.e-2',
-        >>>                    'species_numbers': 'on time 5.e-3', 'event_report': 'off', 'max_steps': 1000000000,
-        >>>                    'max_time': 2.0, 'wall_time': 86400}
-        >>>
-        >>> for temp in range(400, 1000, 100):
-        >>>     my_job.create_job_dir(
-        >>>         path=f'./co_oxidation_{temp}K',
-        >>>         T=temp,  # in K
-        >>>         simulation_tags=simulation_tags,
-        >>>         dict_pressure={'CO': 1.2, 'O2': 0.01},  # in bar
-        >>>         repeat_cell=[10, 10],
-        >>>         dict_manual_scaling={'O_diffusion': 1e-3},
-        >>>         list_auto_scaling=['CO_adsorption'])
-        """
+    Parameters:
+
+    df_gas: Pandas dataframe
+        Informaton about the gas molecules (see README.md)
+    df_mechanism: Pandas dataframe
+        Informaton on the reaction model (see README.md)
+    df_energetics: Pandas dataframe
+        Informaton on the energetic model (see README.md)
+    lattice_path: str
+        The path of the lattice_input.dat (previously created).
+
+    Example:
+    >>> import numpy as np
+    >>> import pandas as pd
+    >>> from zacrosio.kmc_job import NewKMCJob
+    >>>
+    >>> job = NewKMCJob(
+    >>>    df_gas=pd.read_csv(f'gas_data.csv', index_col=0),
+    >>>    df_mechanism=pd.read_csv(f'mechanism.csv', index_col=0),
+    >>>    df_energetics=pd.read_csv(f'energetics.csv', index_col=0),
+    >>>    lattice_path="lattice_input.dat")
+    >>>
+    >>>for T in np.linspace(500, 1000, 6):
+    >>>    for pCO in np.logspace(-4, 0, 10):
+    >>>        for pO in np.logspace(-4, 0, 10):
+    >>>            job.create_job_dir(path=f"./co_oxidation_T_{T}_pCO_{pCO}_pO_{pO}",
+    >>>                               T=T,
+    >>>                               dict_pressure={'CO': pCO, 'O': pO},
+    >>>                               reporting='on time 5.0e-1',
+    >>>                               stopping={'max_steps': 'infinity', 'max_time': 'infinity', 'wall_time': 36000},
+    >>>                               repeat_cell=[10, 10],
+    >>>                               list_auto_scaling=['O_diffusion'])
+    """
 
     def __init__(self, df_gas, df_mechanism, df_energetics, lattice_path):
         self.path = None
         self.df_gas = df_gas
         self.reaction_model = ReactionModel(df=df_mechanism)
         self.energetic_model = EnergeticModel(df=df_energetics)
         self.lattice_model = LatticeModel(path=lattice_path)
 
-    def create_job_dir(self, path, T, simulation_tags, dict_pressure, repeat_cell=None, dict_manual_scaling=None,
+    def create_job_dir(self, path, T, dict_pressure, reporting=None, stopping=None, repeat_cell=None, dict_manual_scaling=None,
                        list_auto_scaling=None, scaling_tags=None):
         """Creates a new directory and writes there the ZACROS input files"""
         if scaling_tags is None:
             scaling_tags = {}
         if list_auto_scaling is None:
             list_auto_scaling = []
         if dict_manual_scaling is None:
             dict_manual_scaling = {}
         self.path = path
         if not os.path.exists(self.path):
             os.mkdir(self.path)
-            self.write_simulation(T=T, simulation_tags=simulation_tags, dict_pressure=dict_pressure,
+            self.write_simulation(T=T, reporting=reporting, stopping=stopping, dict_pressure=dict_pressure,
                                   list_auto_scaling=list_auto_scaling, scaling_tags=scaling_tags)
             self.reaction_model.write(path=self.path, T=T, df_gas=self.df_gas, dict_manual_scaling=dict_manual_scaling,
                                       list_auto_scaling=list_auto_scaling)
             self.energetic_model.write(path=self.path)
             if repeat_cell is not None:
                 self.lattice_model.update_size(size=repeat_cell)
             self.lattice_model.write(path=self.path)
         else:
             print(f'{self.path} already exists (nothing done)')
 
-    def write_simulation(self, T, simulation_tags, dict_pressure, list_auto_scaling, scaling_tags):
+    def write_simulation(self, T, reporting, stopping, dict_pressure, list_auto_scaling, scaling_tags):
         """Writes the simulation_input.dat file"""
         gas_specs_names = [x for x in self.df_gas.index]
         surf_specs_names = [x.replace('_point', '') for x in self.energetic_model.df.index if '_point' in x]
         surf_specs_names = [x + '*' * int(self.energetic_model.df.loc[f'{x}_point', 'sites']) for x in surf_specs_names]
         surf_specs_dent = [x.count('*') for x in surf_specs_names]
         write_header(f"{self.path}/simulation_input.dat")
         with open(f"{self.path}/simulation_input.dat", 'a') as infile:
-            if "random_seed" in simulation_tags:
-                infile.write('random_seed\t'.expandtabs(26) + str(simulation_tags["random_seed"]) + '\n')
-            else:
-                infile.write('random_seed\t'.expandtabs(26) + str(randint(100000, 999999)) + '\n')
+            infile.write('random_seed\t'.expandtabs(26) + str(randint(100000, 999999)) + '\n')
             infile.write('temperature\t'.expandtabs(26) + str(float(T)) + '\n')
             p_tot = sum(dict_pressure.values())
             infile.write('pressure\t'.expandtabs(26) + str(p_tot) + '\n')
             infile.write('n_gas_species\t'.expandtabs(26) + str(len(gas_specs_names)) + '\n')
             infile.write('gas_specs_names\t'.expandtabs(26) + " ".join(str(x) for x in gas_specs_names) + '\n')
             tags_dict = ['gas_energy', 'gas_molec_weight']
             tags_zacros = ['gas_energies', 'gas_molec_weights']
@@ -97,37 +93,16 @@
                 tag_list = [self.df_gas.loc[x, tag1] for x in gas_specs_names]
                 infile.write(f'{tag2}\t'.expandtabs(26) + " ".join(str(x) for x in tag_list) + '\n')
             gas_molar_frac_list = [dict_pressure[x] / p_tot for x in gas_specs_names]
             infile.write(f'gas_molar_fracs\t'.expandtabs(26) + " ".join(str(x) for x in gas_molar_frac_list) + '\n')
             infile.write('n_surf_species\t'.expandtabs(26) + str(len(surf_specs_names)) + '\n')
             infile.write('surf_specs_names\t'.expandtabs(26) + " ".join(str(x) for x in surf_specs_names) + '\n')
             infile.write('surf_specs_dent\t'.expandtabs(26) + " ".join(str(x) for x in surf_specs_dent) + '\n')
-            for tag in simulation_tags:
-                infile.write((tag + '\t').expandtabs(26) + str(simulation_tags[tag]) + '\n')
+            for tag in ['snapshots', 'process_statistics', 'species_numbers']:
+                infile.write((tag + '\t').expandtabs(26) + reporting + '\n')
+            for tag in ['max_steps', 'max_time', 'wall_time']:
+                infile.write((tag + '\t').expandtabs(26) + str(stopping[tag]) + '\n')
             if len(list_auto_scaling) > 0:
                 infile.write(f"enable_stiffness_scaling\n")
                 for tag in scaling_tags:
                     infile.write((tag + '\t').expandtabs(26) + str(scaling_tags[tag]) + '\n')
             infile.write(f"finish\n")
-
-
-class KMCJob:
-    """A class that represents a finished KMC job with ZACROS."""
-
-    def __init__(self, path):
-        self.path = path
-        self.finished = check_finished(path)
-
-        if self.finished:
-            # Read files
-            self.lattice_input = read_file(f"{path}/lattice_input.dat")
-            # Get basic info
-            n_surf_species, n_sites, area = get_data_from_general_output(path)
-            self.n_surf_species = n_surf_species
-            self.n_sites = n_sites
-            self.area = area
-
-    def plot_production(self, molecule=None):
-        plt_production(self.path, self.n_surf_species, molecule)
-
-    def plot_tof(self, molecule):
-        plt_tof(self.path, self.area, molecule)
```

