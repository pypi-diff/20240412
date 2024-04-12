# Comparing `tmp/scikit_mol-0.2.1.tar.gz` & `tmp/scikit_mol-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit_mol-0.2.1.tar", last modified: Sat May  6 05:39:39 2023, max compression
+gzip compressed data, was "scikit_mol-0.3.0.tar", last modified: Fri Apr 12 12:40:56 2024, max compression
```

## Comparing `scikit_mol-0.2.1.tar` & `scikit_mol-0.3.0.tar`

### file list

```diff
@@ -1,85 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:39:39.280298 scikit_mol-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-06 05:39:39.280298 scikit_mol-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:39:39.268298 scikit_mol-0.2.1/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    15972 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/01_basic_usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/01_basic_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)    40949 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/02_descriptor_transformer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/02_descriptor_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:39:39.268298 scikit_mol-0.2.1/notebooks/02_descriptor_transformer_files/
--rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/02_descriptor_transformer_files/02_descriptor_transformer_5_0.png
--rw-r--r--   0 runner    (1001) docker     (123)    12178 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/03_example_pipeline.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/03_example_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    30287 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/04_standardizer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/04_standardizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:39:39.268298 scikit_mol-0.2.1/notebooks/04_standardizer_files/
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/04_standardizer_files/04_standardizer_3_0.png
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/04_standardizer_files/04_standardizer_3_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/05_smiles_sanitaztion.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/05_smiles_sanitaztion.py
--rw-r--r--   0 runner    (1001) docker     (123)    19466 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/06_hyperparameter_tuning.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/06_hyperparameter_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)    11229 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/07_parallel_transforms.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/07_parallel_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/08_external_library_skopt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:39:39.272298 scikit_mol-0.2.1/notebooks/images/
--rw-r--r--   0 runner    (1001) docker     (123)    66320 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/AtomPairFingerprintTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (123)    60999 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/AtomPairFingerprintTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (123)    64259 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/Desc2DTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (123)    58977 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/Desc2DTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (123)    66054 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/MACCSTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (123)    60534 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/MACCSTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (123)    65268 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/MorganTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (123)    59856 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/MorganTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (123)    65110 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/RDKitFPTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (123)    60176 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/RDKitFPTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (123)    64025 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/SECFingerprintTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (123)    60783 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/SECFingerprintTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (123)    68278 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/TopologicalTorsionFingerprintTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (123)    60915 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/TopologicalTorsionFingerprintTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/Transformer_Widget.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    52959 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/max_speedup_vs_throughput.png
--rw-r--r--   0 runner    (1001) docker     (123)    46854 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/max_speedup_vs_throughput.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/pair_notebook.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/run_notebooks.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       20 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/sync_notebooks.sh
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:39:39.264298 scikit_mol-0.2.1/ressources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:39:39.276298 scikit_mol-0.2.1/ressources/logo/
--rw-r--r--   0 runner    (1001) docker     (123)  1389097 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/ressources/logo/ScikitMol_Logo.ai
--rw-r--r--   0 runner    (1001) docker     (123)    70075 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/ressources/logo/ScikitMol_Logo_DarkBG.png
--rw-r--r--   0 runner    (1001) docker     (123)    33144 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/ressources/logo/ScikitMol_Logo_DarkBG_300px.png
--rw-r--r--   0 runner    (1001) docker     (123)   150544 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/ressources/logo/ScikitMol_Logo_DarkBG_600dpi.png
--rw-r--r--   0 runner    (1001) docker     (123)    66674 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/ressources/logo/ScikitMol_Logo_LightBG.png
--rw-r--r--   0 runner    (1001) docker     (123)    30449 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/ressources/logo/ScikitMol_Logo_LightBG_300px.png
--rw-r--r--   0 runner    (1001) docker     (123)   143920 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/ressources/logo/ScikitMol_Logo_LightBG_600dpi.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:39:39.276298 scikit_mol-0.2.1/scikit_mol/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/scikit_mol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-06 05:39:39.000000 scikit_mol-0.2.1/scikit_mol/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/scikit_mol/conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/scikit_mol/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/scikit_mol/fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/scikit_mol/standardizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/scikit_mol/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:39:39.280298 scikit_mol-0.2.1/scikit_mol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-06 05:39:39.000000 scikit_mol-0.2.1/scikit_mol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-06 05:39:39.000000 scikit_mol-0.2.1/scikit_mol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 05:39:39.000000 scikit_mol-0.2.1/scikit_mol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-06 05:39:39.000000 scikit_mol-0.2.1/scikit_mol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-06 05:39:39.000000 scikit_mol-0.2.1/scikit_mol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-06 05:39:39.280298 scikit_mol-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:39:39.280298 scikit_mol-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:39:39.280298 scikit_mol-0.2.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    18060 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/tests/data/SLC6A4_active_excapedb_subset.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/tests/test_desctransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/tests/test_fptransformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/tests/test_parameter_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/tests/test_sanitizer.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/tests/test_scikit_mol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/tests/test_smilestomol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/tests/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:40:56.475579 scikit_mol-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/CITATION.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/CONTRIBUTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-04-12 12:40:56.475579 scikit_mol-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:40:56.459579 scikit_mol-0.3.0/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    16093 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/01_basic_usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/01_basic_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41470 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/02_descriptor_transformer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/02_descriptor_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:40:56.459579 scikit_mol-0.3.0/notebooks/02_descriptor_transformer_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    14040 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/02_descriptor_transformer_files/02_descriptor_transformer_5_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/03_example_pipeline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/03_example_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/04_standardizer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/04_standardizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:40:56.459579 scikit_mol-0.3.0/notebooks/04_standardizer_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/04_standardizer_files/04_standardizer_3_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/04_standardizer_files/04_standardizer_3_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8516 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/05_smiles_sanitaztion.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/05_smiles_sanitaztion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19780 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/06_hyperparameter_tuning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9198 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/06_hyperparameter_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11673 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/07_parallel_transforms.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/07_parallel_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54904 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/08_external_library_skopt.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/08_external_library_skopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)   266596 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/09_Combinatorial_Method_Usage_with_FingerPrint_Transformers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18018 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/09_Combinatorial_Method_Usage_with_FingerPrint_Transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)   166074 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/10_pipeline_pandas_output.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11847 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/10_pipeline_pandas_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:40:56.463579 scikit_mol-0.3.0/notebooks/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    66320 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/AtomPairFingerprintTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (127)    60999 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/AtomPairFingerprintTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    64259 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/Desc2DTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (127)    58977 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/Desc2DTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    66054 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/MACCSTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (127)    60534 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/MACCSTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    65268 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/MorganTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (127)    59856 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/MorganTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    65110 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/RDKitFPTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (127)    60176 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/RDKitFPTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    64025 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/SECFingerprintTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (127)    60783 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/SECFingerprintTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    68278 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/TopologicalTorsionFingerprintTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (127)    60915 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/TopologicalTorsionFingerprintTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/Transformer_Widget.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    52959 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/max_speedup_vs_throughput.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46854 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/images/max_speedup_vs_throughput.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/pair_notebook.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      337 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/run_notebooks.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       25 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/notebooks/sync_notebooks.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:40:56.451579 scikit_mol-0.3.0/ressources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:40:56.467579 scikit_mol-0.3.0/ressources/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)  1389097 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo.ai
+-rw-r--r--   0 runner    (1001) docker     (127)    70075 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo_DarkBG.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33144 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo_DarkBG_300px.png
+-rw-r--r--   0 runner    (1001) docker     (127)   150544 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo_DarkBG_600dpi.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66674 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo_LightBG.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30449 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo_LightBG_300px.png
+-rw-r--r--   0 runner    (1001) docker     (127)   143920 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo_LightBG_600dpi.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:40:56.471579 scikit_mol-0.3.0/scikit_mol/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/scikit_mol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-12 12:40:56.000000 scikit_mol-0.3.0/scikit_mol/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/scikit_mol/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/scikit_mol/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/scikit_mol/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25344 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/scikit_mol/fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/scikit_mol/standardizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/scikit_mol/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:40:56.471579 scikit_mol-0.3.0/scikit_mol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-04-12 12:40:56.000000 scikit_mol-0.3.0/scikit_mol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-12 12:40:56.000000 scikit_mol-0.3.0/scikit_mol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:40:56.000000 scikit_mol-0.3.0/scikit_mol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-12 12:40:56.000000 scikit_mol-0.3.0/scikit_mol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 12:40:56.000000 scikit_mol-0.3.0/scikit_mol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-12 12:40:56.475579 scikit_mol-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:40:56.471579 scikit_mol-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:40:56.471579 scikit_mol-0.3.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   469987 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/tests/data/CDDD_SLC6A4_active_excapedb_subset.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    18060 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/tests/data/SLC6A4_active_excapedb_subset.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/tests/test_desctransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11081 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/tests/test_fptransformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/tests/test_parameter_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/tests/test_sanitizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/tests/test_scikit_mol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/tests/test_smilestomol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-04-12 12:40:50.000000 scikit_mol-0.3.0/tests/test_transformers.py
```

### Comparing `scikit_mol-0.2.1/PKG-INFO` & `scikit_mol-0.3.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,113 +1,102 @@
-Metadata-Version: 2.1
-Name: scikit_mol
-Version: 0.2.1
-Summary: scikit-learn classes for molecule transformation
-Home-page: https://github.com/EBjerrum/scikit-mol
-Download-URL: https://github.com/EBjerrum/scikit-mol
-Author: Esben Jannik Bjerrum
-Author-email: esben@cheminformania.com
-License: Apache-2.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Utilities
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # scikit-mol
+
 ![Fancy logo](./ressources/logo/ScikitMol_Logo_DarkBG_300px.png#gh-dark-mode-only)
 ![Fancy logo](./ressources/logo/ScikitMol_Logo_LightBG_300px.png#gh-light-mode-only)
+
 ## Scikit-Learn classes for molecular vectorization using RDKit
 
 The intended usage is to be able to add molecular vectorization directly into scikit-learn pipelines, so that the final model directly predict on RDKit molecules or SMILES strings
 
-As example with the needed scikit-learn and -mol imports and RDKit mol objects in the mol_list_train and _test lists:
+As example with the needed scikit-learn and -mol imports and RDKit mol objects in the mol_list_train and \_test lists:
 
-    pipe = Pipeline([('mol_transformer', MorganTransformer()), ('Regressor', Ridge())])
+    pipe = Pipeline([('mol_transformer', MorganFingerprintTransformer()), ('Regressor', Ridge())])
     pipe.fit(mol_list_train, y_train)
     pipe.score(mol_list_test, y_test)
     pipe.predict([Chem.MolFromSmiles('c1ccccc1C(=O)C')])
 
     >>> array([4.93858815])
 
 The scikit-learn compatibility should also make it easier to include the fingerprinting step in hyperparameter tuning with scikit-learns utilities
 
 The first draft for the project was created at the [RDKIT UGM 2022 hackathon](https://github.com/rdkit/UGM_2022) 2022-October-14
 
-
 ## Implemented
-* descriptors
-    * MolecularDescriptorTransformer
+
+- Descriptors
+  - MolecularDescriptorTransformer
+
 <br>
-* fingerprints
-    * MorganFingerprintTransformer
-    * MACCSKeysFingerprintTransformer
-    * RDKitFingerprintTransformer
-    * AtomPairFingerprintTransformer
-    * TopologicalTorsionFingerprintTransformer
-    * MHFingerprintTransformer
-    * SECFingerprintTransformer
-    * AvalonFingerprintTransformer
+
+- Fingerprints
+  - MorganFingerprintTransformer
+  - MACCSKeysFingerprintTransformer
+  - RDKitFingerprintTransformer
+  - AtomPairFingerprintTransformer
+  - TopologicalTorsionFingerprintTransformer
+  - MHFingerprintTransformer
+  - SECFingerprintTransformer
+  - AvalonFingerprintTransformer
+
 <br>
-* conversions
-    * SmilesToMol
+
+- Conversions
+  - SmilesToMol
+
 <br>
-* standardizer
-    * Standardizer
+
+- Standardizer
+  - Standardizer
+
 <br>
-* utilities
-    * CheckSmilesSanitazion
 
+- Utilities
+  - CheckSmilesSanitazion
 
 ## Installation
+
 Users can install latest tagged release from pip
 
     pip install scikit-mol
 
 Bleeding edge
 
     pip install git+https://github.com:EBjerrum/scikit-mol.git
 
-Developers 
-
-    git clone git@github.com:EBjerrum/scikit-mol.git
-    pip install -e .
-
 ## Documentation
 
 There are a collection of notebooks in the notebooks directory which demonstrates some different aspects and use cases
 
-* [Basic Usage and fingerprint transformers](https://github.com/EBjerrum/scikit-mol/blob/main/notebooks/01_basic_usage.ipynb)
-* [Descriptor transformer](https://github.com/EBjerrum/scikit-mol/blob/main/notebooks/02_descriptor_transformer.ipynb)
-* [Pipelining with Scikit-Learn classes](https://github.com/EBjerrum/scikit-mol/blob/main/notebooks/03_example_pipeline.ipynb)
-* [Molecular standardization](https://github.com/EBjerrum/scikit-mol/blob/main/notebooks/04_standardizer.ipynb)
-* [Sanitizing SMILES input](https://github.com/EBjerrum/scikit-mol/blob/main/notebooks/05_smiles_sanitaztion.ipynb)
-* [Integrated hyperparameter tuning of Scikit-Learn estimator and Scikit-Mol transformer](https://github.com/EBjerrum/scikit-mol/blob/main/notebooks/06_hyperparameter_tuning.ipynb)
-* [Using parallel execution to speed up descriptor and fingerprint calculations](https://github.com/EBjerrum/scikit-mol/blob/main/notebooks/07_parallel_transforms.ipynb)
+- [Basic Usage and fingerprint transformers](https://github.com/EBjerrum/scikit-mol/tree/main/notebooks/01_basic_usage.ipynb)
+- [Descriptor transformer](https://github.com/EBjerrum/scikit-mol/tree/main/notebooks/02_descriptor_transformer.ipynb)
+- [Pipelining with Scikit-Learn classes](https://github.com/EBjerrum/scikit-mol/tree/main/notebooks/03_example_pipeline.ipynb)
+- [Molecular standardization](https://github.com/EBjerrum/scikit-mol/tree/main/notebooks/04_standardizer.ipynb)
+- [Sanitizing SMILES input](https://github.com/EBjerrum/scikit-mol/tree/main/notebooks/05_smiles_sanitaztion.ipynb)
+- [Integrated hyperparameter tuning of Scikit-Learn estimator and Scikit-Mol transformer](https://github.com/EBjerrum/scikit-mol/tree/main/notebooks/06_hyperparameter_tuning.ipynb)
+- [Using parallel execution to speed up descriptor and fingerprint calculations](https://github.com/EBjerrum/scikit-mol/tree/main/notebooks/07_parallel_transforms.ipynb)
+- [Using skopt for hyperparameter tuning](https://github.com/EBjerrum/scikit-mol/tree/main/notebooks/08_external_library_skopt.ipynb)
+- [Testing different fingerprints as part of the hyperparameter optimization](https://github.com/EBjerrum/scikit-mol/blob/main/notebooks/09_Combinatorial_Method_Usage_with_FingerPrint_Transformers.ipynb)
+- [Using pandas output for easy feature importance analysis and combine pre-exisitng values with new computations](https://github.com/EBjerrum/scikit-mol/blob/main/notebooks/10_pipeline_pandas_output.ipynb)
 
+  We also put a software note on ChemRxiv. [https://doi.org/10.26434/chemrxiv-2023-fzqwd](https://doi.org/10.26434/chemrxiv-2023-fzqwd)
+
+## Contributing
+
+There are more information about how to contribute to the project in [CONTRIBUTION.md](https://github.com/EBjerrum/scikit-mol/CONTRIBUTION.md)
 
 ## BUGS
+
 Probably still, please check issues at GitHub and report there
 
 ## Contributers:
-* Esben Jannik Bjerrum [@ebjerrum](https://github.com/ebjerrum), esben@cheminformania.com
-* Carmen Esposito [@cespos](https://github.com/cespos)
-* Son Ha, sonha@uni-mainz.de
-* Oh-hyeon Choung, ohhyeon.choung@gmail.com
-* Andreas Poehlmann, [@ap--](https://github.com/ap--)
-* Ya Chen, [@anya-chen](https://github.com/anya-chen)
-* Rafał Bachorz [@rafalbachorz](https://github.com/rafalbachorz)
-* Adrien Chaton [@adrienchaton](https://github.com/adrienchaton)
+
+- Esben Jannik Bjerrum [@ebjerrum](https://github.com/ebjerrum), esbenbjerrum+scikit_mol@gmail.com
+- Carmen Esposito [@cespos](https://github.com/cespos)
+- Son Ha, sonha@uni-mainz.de
+- Oh-hyeon Choung, ohhyeon.choung@gmail.com
+- Andreas Poehlmann, [@ap--](https://github.com/ap--)
+- Ya Chen, [@anya-chen](https://github.com/anya-chen)
+- Rafał Bachorz [@rafalbachorz](https://github.com/rafalbachorz)
+- Adrien Chaton [@adrienchaton](https://github.com/adrienchaton)
+- [@VincentAlexanderScholz](https://github.com/VincentAlexanderScholz)
+- [@RiesBen](https://github.com/RiesBen)
+- [@enricogandini](https://github.com/enricogandini)
```

### Comparing `scikit_mol-0.2.1/notebooks/01_basic_usage.ipynb` & `scikit_mol-0.3.0/notebooks/01_basic_usage.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967415282999165%*

 * *Differences: {"'cells'": "{2: {'metadata': {'execution': {'iopub.execute_input': '2024-04-12T12:10:09.802220Z', "*

 * *            "'iopub.status.busy': '2024-04-12T12:10:09.802030Z', 'iopub.status.idle': "*

 * *            "'2024-04-12T12:10:09.808949Z', 'shell.execute_reply': "*

 * *            "'2024-04-12T12:10:09.808440Z'}}}, 3: {'metadata': {'execution': "*

 * *            "{'iopub.execute_input': '2024-04-12T12:10:09.811277Z', 'iopub.status.busy': "*

 * *            "'2024-04-12T12:10:09.811060Z', 'iopub.status.idle': '2024-04-12T12:10:0 […]*

```diff
@@ -21,35 +21,35 @@
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "f8025236",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:22.197918Z",
-                    "iopub.status.busy": "2023-03-19T08:54:22.197263Z",
-                    "iopub.status.idle": "2023-03-19T08:54:22.205876Z",
-                    "shell.execute_reply": "2023-03-19T08:54:22.205379Z"
+                    "iopub.execute_input": "2024-04-12T12:10:09.802220Z",
+                    "iopub.status.busy": "2024-04-12T12:10:09.802030Z",
+                    "iopub.status.idle": "2024-04-12T12:10:09.808949Z",
+                    "shell.execute_reply": "2024-04-12T12:10:09.808440Z"
                 }
             },
             "outputs": [],
             "source": [
                 "from IPython.core.display import HTML"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "58a33f4d",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:22.208372Z",
-                    "iopub.status.busy": "2023-03-19T08:54:22.208130Z",
-                    "iopub.status.idle": "2023-03-19T08:54:22.428376Z",
-                    "shell.execute_reply": "2023-03-19T08:54:22.427474Z"
+                    "iopub.execute_input": "2024-04-12T12:10:09.811277Z",
+                    "iopub.status.busy": "2024-04-12T12:10:09.811060Z",
+                    "iopub.status.idle": "2024-04-12T12:10:09.936897Z",
+                    "shell.execute_reply": "2024-04-12T12:10:09.936201Z"
                 }
             },
             "outputs": [],
             "source": [
                 "from rdkit import Chem\n",
                 "\n",
                 "smiles_strings = [\"C12C([C@@H](OC(C=3C=CC(=CC3)F)C=4C=CC(=CC4)F)CC(N1CCCCCC5=CC=CC=C5)CC2)C(=O)OC\", \n",
@@ -72,26 +72,26 @@
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "id": "cdb821a1",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:22.431905Z",
-                    "iopub.status.busy": "2023-03-19T08:54:22.431641Z",
-                    "iopub.status.idle": "2023-03-19T08:54:22.962569Z",
-                    "shell.execute_reply": "2023-03-19T08:54:22.961792Z"
+                    "iopub.execute_input": "2024-04-12T12:10:09.939980Z",
+                    "iopub.status.busy": "2024-04-12T12:10:09.939552Z",
+                    "iopub.status.idle": "2024-04-12T12:10:10.505528Z",
+                    "shell.execute_reply": "2024-04-12T12:10:10.504885Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "MorganTransformer(radius=3)\n"
+                        "MorganFingerprintTransformer(radius=3)\n"
                     ]
                 }
             ],
             "source": [
                 "from scikit_mol.fingerprints import MorganFingerprintTransformer\n",
                 "\n",
                 "transformer = MorganFingerprintTransformer(radius=3)\n",
@@ -112,28 +112,28 @@
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "id": "c3a24f4e",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:22.965768Z",
-                    "iopub.status.busy": "2023-03-19T08:54:22.965105Z",
-                    "iopub.status.idle": "2023-03-19T08:54:22.971941Z",
-                    "shell.execute_reply": "2023-03-19T08:54:22.971327Z"
+                    "iopub.execute_input": "2024-04-12T12:10:10.508400Z",
+                    "iopub.status.busy": "2024-04-12T12:10:10.508055Z",
+                    "iopub.status.idle": "2024-04-12T12:10:10.514636Z",
+                    "shell.execute_reply": "2024-04-12T12:10:10.514117Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<style>#sk-container-id-1 {color: black;background-color: white;}#sk-container-id-1 pre{padding: 0;}#sk-container-id-1 div.sk-toggleable {background-color: white;}#sk-container-id-1 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-1 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-1 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-1 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-1 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-1 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-1 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-1 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-1 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-1 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-1 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-1 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-1 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-1 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-1 div.sk-item {position: relative;z-index: 1;}#sk-container-id-1 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-1 div.sk-item::before, #sk-container-id-1 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-1 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-1 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-1 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-1 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-1 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-1 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-1 div.sk-label-container {text-align: center;}#sk-container-id-1 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-1 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-1\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>MorganTransformer(radius=3)</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br />On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class=\"sk-container\" hidden><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-1\" type=\"checkbox\" checked><label for=\"sk-estimator-id-1\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">MorganTransformer</label><div class=\"sk-toggleable__content\"><pre>MorganTransformer(radius=3)</pre></div></div></div></div></div>"
+                            "<style>#sk-container-id-1 {color: black;}#sk-container-id-1 pre{padding: 0;}#sk-container-id-1 div.sk-toggleable {background-color: white;}#sk-container-id-1 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-1 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-1 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-1 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-1 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-1 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-1 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-1 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-1 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-1 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-1 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-1 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-1 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-1 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-1 div.sk-item {position: relative;z-index: 1;}#sk-container-id-1 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-1 div.sk-item::before, #sk-container-id-1 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-1 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-1 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-1 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-1 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-1 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-1 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-1 div.sk-label-container {text-align: center;}#sk-container-id-1 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-1 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-1\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>MorganFingerprintTransformer(radius=3)</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br />On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class=\"sk-container\" hidden><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-1\" type=\"checkbox\" checked><label for=\"sk-estimator-id-1\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">MorganFingerprintTransformer</label><div class=\"sk-toggleable__content\"><pre>MorganFingerprintTransformer(radius=3)</pre></div></div></div></div></div>"
                         ],
                         "text/plain": [
-                            "MorganTransformer(radius=3)"
+                            "MorganFingerprintTransformer(radius=3)"
                         ]
                     },
                     "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -151,18 +151,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "112afff2",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:22.974458Z",
-                    "iopub.status.busy": "2023-03-19T08:54:22.974238Z",
-                    "iopub.status.idle": "2023-03-19T08:54:22.978835Z",
-                    "shell.execute_reply": "2023-03-19T08:54:22.978252Z"
+                    "iopub.execute_input": "2024-04-12T12:10:10.517110Z",
+                    "iopub.status.busy": "2024-04-12T12:10:10.516867Z",
+                    "iopub.status.idle": "2024-04-12T12:10:10.521207Z",
+                    "shell.execute_reply": "2024-04-12T12:10:10.520689Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "{'nBits': 2048,\n",
@@ -194,26 +194,26 @@
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "id": "4229d3d3",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:22.981502Z",
-                    "iopub.status.busy": "2023-03-19T08:54:22.981247Z",
-                    "iopub.status.idle": "2023-03-19T08:54:22.985186Z",
-                    "shell.execute_reply": "2023-03-19T08:54:22.984526Z"
+                    "iopub.execute_input": "2024-04-12T12:10:10.523546Z",
+                    "iopub.status.busy": "2024-04-12T12:10:10.523347Z",
+                    "iopub.status.idle": "2024-04-12T12:10:10.527067Z",
+                    "shell.execute_reply": "2024-04-12T12:10:10.526450Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "MorganTransformer(nBits=256)\n"
+                        "MorganFingerprintTransformer(nBits=256)\n"
                     ]
                 }
             ],
             "source": [
                 "parameters[\"radius\"] = 2\n",
                 "parameters[\"nBits\"] = 256\n",
                 "transformer.set_params(**parameters)\n",
@@ -230,18 +230,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "id": "d2276e30",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:22.987984Z",
-                    "iopub.status.busy": "2023-03-19T08:54:22.987693Z",
-                    "iopub.status.idle": "2023-03-19T08:54:22.992008Z",
-                    "shell.execute_reply": "2023-03-19T08:54:22.991412Z"
+                    "iopub.execute_input": "2024-04-12T12:10:10.529451Z",
+                    "iopub.status.busy": "2024-04-12T12:10:10.529229Z",
+                    "iopub.status.idle": "2024-04-12T12:10:10.533310Z",
+                    "shell.execute_reply": "2024-04-12T12:10:10.532819Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -264,18 +264,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "id": "d3b01806",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:22.994560Z",
-                    "iopub.status.busy": "2023-03-19T08:54:22.994348Z",
-                    "iopub.status.idle": "2023-03-19T08:54:22.999695Z",
-                    "shell.execute_reply": "2023-03-19T08:54:22.999044Z"
+                    "iopub.execute_input": "2024-04-12T12:10:10.535668Z",
+                    "iopub.status.busy": "2024-04-12T12:10:10.535455Z",
+                    "iopub.status.idle": "2024-04-12T12:10:10.540535Z",
+                    "shell.execute_reply": "2024-04-12T12:10:10.539917Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[0, 1, 0, ..., 0, 0, 0],\n",
@@ -306,26 +306,26 @@
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "id": "26081bb2",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:23.002288Z",
-                    "iopub.status.busy": "2023-03-19T08:54:23.002005Z",
-                    "iopub.status.idle": "2023-03-19T08:54:23.006182Z",
-                    "shell.execute_reply": "2023-03-19T08:54:23.005653Z"
+                    "iopub.execute_input": "2024-04-12T12:10:10.542876Z",
+                    "iopub.status.busy": "2024-04-12T12:10:10.542661Z",
+                    "iopub.status.idle": "2024-04-12T12:10:10.546656Z",
+                    "shell.execute_reply": "2024-04-12T12:10:10.546143Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "SmilesToMol()\n"
+                        "SmilesToMolTransformer()\n"
                     ]
                 }
             ],
             "source": [
                 "from scikit_mol.conversions import SmilesToMolTransformer\n",
                 "smi2mol = SmilesToMolTransformer()\n",
                 "print(smi2mol)"
@@ -333,26 +333,31 @@
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "id": "6b0e5f4a",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:23.009239Z",
-                    "iopub.status.busy": "2023-03-19T08:54:23.008966Z",
-                    "iopub.status.idle": "2023-03-19T08:54:23.014260Z",
-                    "shell.execute_reply": "2023-03-19T08:54:23.013537Z"
+                    "iopub.execute_input": "2024-04-12T12:10:10.548964Z",
+                    "iopub.status.busy": "2024-04-12T12:10:10.548714Z",
+                    "iopub.status.idle": "2024-04-12T12:10:10.553416Z",
+                    "shell.execute_reply": "2024-04-12T12:10:10.552805Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "[<rdkit.Chem.rdchem.Mol object at 0x7fb1ac449af0>, <rdkit.Chem.rdchem.Mol object at 0x7fb1ac449b60>, <rdkit.Chem.rdchem.Mol object at 0x7fb1ac449bd0>, <rdkit.Chem.rdchem.Mol object at 0x7fb1ac449c40>, <rdkit.Chem.rdchem.Mol object at 0x7fb1ac449cb0>, <rdkit.Chem.rdchem.Mol object at 0x7fb1ac449d20>]\n"
+                        "[[<rdkit.Chem.rdchem.Mol object at 0x798ebb81ee30>]\n",
+                        " [<rdkit.Chem.rdchem.Mol object at 0x798ebb81eea0>]\n",
+                        " [<rdkit.Chem.rdchem.Mol object at 0x798ebb81ef10>]\n",
+                        " [<rdkit.Chem.rdchem.Mol object at 0x798ebb81ef80>]\n",
+                        " [<rdkit.Chem.rdchem.Mol object at 0x798ebb81eff0>]\n",
+                        " [<rdkit.Chem.rdchem.Mol object at 0x798ebb81f060>]]\n"
                     ]
                 }
             ],
             "source": [
                 "print(smi2mol.transform(smiles_strings))"
             ]
         }
@@ -372,13 +377,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.9"
+            "version": "3.10.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `scikit_mol-0.2.1/notebooks/01_basic_usage.py` & `scikit_mol-0.3.0/notebooks/01_basic_usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # jupyter:
 #   jupytext:
 #     formats: ipynb,py:percent
 #     text_representation:
 #       extension: .py
 #       format_name: percent
 #       format_version: '1.3'
-#       jupytext_version: 1.14.5
+#       jupytext_version: 1.16.1
 #   kernelspec:
 #     display_name: Python 3.9.4 ('rdkit')
 #     language: python
 #     name: python3
 # ---
 
 # %% [markdown]
```

### Comparing `scikit_mol-0.2.1/notebooks/02_descriptor_transformer.ipynb` & `scikit_mol-0.3.0/notebooks/02_descriptor_transformer.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970914502164503%*

 * *Differences: {"'cells'": "{1: {'metadata': {'execution': {'iopub.execute_input': '2024-04-12T12:10:11.861457Z', "*

 * *            "'iopub.status.busy': '2024-04-12T12:10:11.861246Z', 'iopub.status.idle': "*

 * *            "'2024-04-12T12:10:12.860086Z', 'shell.execute_reply': "*

 * *            "'2024-04-12T12:10:12.859376Z'}}}, 3: {'metadata': {'execution': "*

 * *            "{'iopub.execute_input': '2024-04-12T12:10:12.863149Z', 'iopub.status.busy': "*

 * *            "'2024-04-12T12:10:12.862837Z', 'iopub.status.idle': '2024-04-12T12:10:1 […]*

```diff
@@ -12,18 +12,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "51b69a7e",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:24.680576Z",
-                    "iopub.status.busy": "2023-03-19T08:54:24.680106Z",
-                    "iopub.status.idle": "2023-03-19T08:54:25.564119Z",
-                    "shell.execute_reply": "2023-03-19T08:54:25.563257Z"
+                    "iopub.execute_input": "2024-04-12T12:10:11.861457Z",
+                    "iopub.status.busy": "2024-04-12T12:10:11.861246Z",
+                    "iopub.status.idle": "2024-04-12T12:10:12.860086Z",
+                    "shell.execute_reply": "2024-04-12T12:10:12.859376Z"
                 },
                 "lines_to_next_cell": 0
             },
             "outputs": [],
             "source": [
                 "from rdkit import Chem\n",
                 "import numpy as np\n",
@@ -41,27 +41,27 @@
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "f1d8fc37",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:25.567192Z",
-                    "iopub.status.busy": "2023-03-19T08:54:25.566898Z",
-                    "iopub.status.idle": "2023-03-19T08:54:25.573408Z",
-                    "shell.execute_reply": "2023-03-19T08:54:25.572679Z"
+                    "iopub.execute_input": "2024-04-12T12:10:12.863149Z",
+                    "iopub.status.busy": "2024-04-12T12:10:12.862837Z",
+                    "iopub.status.idle": "2024-04-12T12:10:12.868668Z",
+                    "shell.execute_reply": "2024-04-12T12:10:12.868151Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "There are 208 available descriptors\n",
-                        "The first five descriptor names: ['MaxEStateIndex', 'MinEStateIndex', 'MaxAbsEStateIndex', 'MinAbsEStateIndex', 'qed']\n"
+                        "There are 209 available descriptors\n",
+                        "The first five descriptor names: ['MaxAbsEStateIndex', 'MaxEStateIndex', 'MinAbsEStateIndex', 'MinEStateIndex', 'qed']\n"
                     ]
                 }
             ],
             "source": [
                 "descriptor = MolecularDescriptorTransformer()\n",
                 "available_descriptors = descriptor.available_descriptors\n",
                 "print(f\"There are {len(available_descriptors)} available descriptors\")\n",
@@ -78,24 +78,24 @@
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "id": "702168a7",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:25.576081Z",
-                    "iopub.status.busy": "2023-03-19T08:54:25.575815Z",
-                    "iopub.status.idle": "2023-03-19T08:54:25.788390Z",
-                    "shell.execute_reply": "2023-03-19T08:54:25.787540Z"
+                    "iopub.execute_input": "2024-04-12T12:10:12.871338Z",
+                    "iopub.status.busy": "2024-04-12T12:10:12.870842Z",
+                    "iopub.status.idle": "2024-04-12T12:10:13.031911Z",
+                    "shell.execute_reply": "2024-04-12T12:10:13.031258Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAh8AAAGdCAYAAACyzRGfAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguMCwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy81sbWrAAAACXBIWXMAAA9hAAAPYQGoP6dpAABn50lEQVR4nO3deXwb9Zk/8M/M6PAV27lsx8QJIQ0knC0pDS60peASssDCkm2BZVugbNm2gS4JvbK/BlraEmB3gUJDaPtLA/21lDbsQgtb0gVDwlKSAAHKHRIIJODYIYdvW9d8f3/MoZnRyLakGWnkfN6vl7EtKaORZDSPnuf5PiMJIQSIiIiIikQu9Q4QERHRoYXBBxERERUVgw8iIiIqKgYfREREVFQMPoiIiKioGHwQERFRUTH4ICIioqJi8EFERERFFSr1DjipqoqOjg5MmDABkiSVeneIiIhoDIQQ6OvrQ3NzM2R55NxG4IKPjo4OtLS0lHo3iIiIKA+7d+/G9OnTR7xN4IKPCRMmANB2vra2tsR7Q0RERGPR29uLlpYW8zg+ksAFH0appba2lsEHERFRmRlLywQbTomIiKiocgo+UqkUVqxYgVmzZqGyshKzZ8/GD3/4Q1hPjCuEwHXXXYdp06ahsrISbW1t2L59u+c7TkREROUpp+Dj5ptvxurVq/HTn/4Ub7zxBm6++WbccsstuPPOO83b3HLLLbjjjjtw9913Y8uWLaiursbChQsxPDzs+c4TERFR+ZGENW0xinPOOQeNjY1Ys2aNednixYtRWVmJX//61xBCoLm5Gddeey2++c1vAgB6enrQ2NiIe+65BxdddNGo99Hb24u6ujr09PSw54OIiKhM5HL8zinz8clPfhLt7e146623AAB//etf8fTTT2PRokUAgJ07d6KzsxNtbW3mv6mrq8OCBQuwadOmXB8HERERjUM5rXb57ne/i97eXsydOxeKoiCVSuHHP/4xLrnkEgBAZ2cnAKCxsdH27xobG83rnGKxGGKxmPl7b29vTg+AiIiIyktOmY/f//73+M1vfoP77rsPL7zwAu699178+7//O+699968d2DlypWoq6szvzhgjIiIaHzLKfj41re+he9+97u46KKLcNxxx+GLX/wili5dipUrVwIAmpqaAABdXV22f9fV1WVe57R8+XL09PSYX7t3787ncRAREVGZ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sQWNjz32GGpra3H00UcX54HkqtQdr8Vw//33i2g0Ku655x7x+uuviyuvvFLU19fbOoOpdK699lqxYcMGsXPnTvGXv/xFtLW1iSlTpoi9e/cKIYT46le/KmbMmCGeeOIJ8fzzz4vW1lbR2tpa4r0+dPT19YkXX3xRvPjiiwKAuPXWW8WLL74o3nvvPSGEEDfddJOor68Xf/jDH8TLL78szjvvPDFr1iwxNDRkbuOss84SH/vYx8SWLVvE008/LebMmSMuvvjiUj2kcW2k16uvr09885vfFJs2bRI7d+4Ujz/+uDjxxBPFnDlzxPDwsLkNvl7F87WvfU3U1dWJDRs2iD179phfg4OD5m1Gew9MJpPi2GOPFWeeeaZ46aWXxPr168XUqVPF8uXLS/GQxuSQCD6EEOLOO+8UM2bMEJFIRHziE58QmzdvLvUuke7CCy8U06ZNE5FIRBx22GHiwgsvFDt27DCvHxoaEl//+tfFxIkTRVVVlfi7v/s7sWfPnhLu8aHlySefFAAyvi699FIhhLbcdsWKFaKxsVFEo1FxxhlniG3bttm2sX//fnHxxReLmpoaUVtbKy6//HLR19dXgkcz/o30eg0ODoozzzxTTJ06VYTDYTFz5kzxla98JeODGF+v4nF7rQCItWvXmrcZy3vgu+++KxYtWiQqKyvFlClTxLXXXisSiUSRH83YSUIIUexsCxERER26xn3PBxEREQULgw8iIiIqKgYfREREVFQMPoiIiKioGHwQERFRUTH4ICIioqJi8EFERERFxeCDiIiIiorBBxERERUVgw8iIiIqKgYfREREVFQMPoiIiKio/j+HZKvLSQUNfwAAAABJRU5ErkJggg==",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -118,18 +118,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "id": "ab72d398",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:25.791190Z",
-                    "iopub.status.busy": "2023-03-19T08:54:25.790956Z",
-                    "iopub.status.idle": "2023-03-19T08:54:25.795456Z",
-                    "shell.execute_reply": "2023-03-19T08:54:25.794734Z"
+                    "iopub.execute_input": "2024-04-12T12:10:13.034545Z",
+                    "iopub.status.busy": "2024-04-12T12:10:13.034315Z",
+                    "iopub.status.idle": "2024-04-12T12:10:13.038330Z",
+                    "shell.execute_reply": "2024-04-12T12:10:13.037823Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -153,26 +153,27 @@
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "4af5488d",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:25.798138Z",
-                    "iopub.status.busy": "2023-03-19T08:54:25.797654Z",
-                    "iopub.status.idle": "2023-03-19T08:54:25.802521Z",
-                    "shell.execute_reply": "2023-03-19T08:54:25.801949Z"
+                    "iopub.execute_input": "2024-04-12T12:10:13.040697Z",
+                    "iopub.status.busy": "2024-04-12T12:10:13.040482Z",
+                    "iopub.status.idle": "2024-04-12T12:10:13.044948Z",
+                    "shell.execute_reply": "2024-04-12T12:10:13.044445Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Desc2DTransformer(desc_list=['HeavyAtomCount', 'FractionCSP3', 'RingCount'])\n"
+                        "MolecularDescriptorTransformer(desc_list=['HeavyAtomCount', 'FractionCSP3',\n",
+                        "                                          'RingCount'])\n"
                     ]
                 }
             ],
             "source": [
                 "print(some_descriptors.set_params(desc_list=['HeavyAtomCount', 'FractionCSP3', 'RingCount']))"
             ]
         },
@@ -201,13 +202,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.9"
+            "version": "3.10.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `scikit_mol-0.2.1/notebooks/02_descriptor_transformer.py` & `scikit_mol-0.3.0/notebooks/02_descriptor_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #   jupytext:
 #     cell_metadata_filter: -all
 #     formats: ipynb,py:percent
 #     text_representation:
 #       extension: .py
 #       format_name: percent
 #       format_version: '1.3'
-#       jupytext_version: 1.14.5
+#       jupytext_version: 1.16.1
 #   kernelspec:
 #     display_name: Python 3.9.4 ('rdkit')
 #     language: python
 #     name: python3
 # ---
 
 # %% [markdown]
```

### Comparing `scikit_mol-0.2.1/notebooks/02_descriptor_transformer_files/02_descriptor_transformer_5_0.png` & `scikit_mol-0.3.0/notebooks/02_descriptor_transformer_files/02_descriptor_transformer_5_0.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/notebooks/03_example_pipeline.ipynb` & `scikit_mol-0.3.0/notebooks/03_example_pipeline.ipynb`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9972095862309678%*

 * *Differences: {"'cells'": "{1: {'metadata': {'execution': {'iopub.execute_input': '2024-04-12T12:10:14.474481Z', "*

 * *            "'iopub.status.busy': '2024-04-12T12:10:14.474256Z', 'iopub.status.idle': "*

 * *            "'2024-04-12T12:10:15.156429Z', 'shell.execute_reply': "*

 * *            "'2024-04-12T12:10:15.155756Z'}}}, 2: {'metadata': {'execution': "*

 * *            "{'iopub.execute_input': '2024-04-12T12:10:15.159285Z', 'iopub.status.busy': "*

 * *            "'2024-04-12T12:10:15.158830Z', 'iopub.status.idle': '2024-04-12T12:10:1 […]*

```diff
@@ -14,18 +14,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "b92c5a96",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:27.653561Z",
-                    "iopub.status.busy": "2023-03-19T08:54:27.653105Z",
-                    "iopub.status.idle": "2023-03-19T08:54:28.385099Z",
-                    "shell.execute_reply": "2023-03-19T08:54:28.384146Z"
+                    "iopub.execute_input": "2024-04-12T12:10:14.474481Z",
+                    "iopub.status.busy": "2024-04-12T12:10:14.474256Z",
+                    "iopub.status.idle": "2024-04-12T12:10:15.156429Z",
+                    "shell.execute_reply": "2024-04-12T12:10:15.155756Z"
                 }
             },
             "outputs": [],
             "source": [
                 "import os\n",
                 "import rdkit\n",
                 "from rdkit import Chem\n",
@@ -38,18 +38,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "0d79bc45",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:28.388213Z",
-                    "iopub.status.busy": "2023-03-19T08:54:28.387874Z",
-                    "iopub.status.idle": "2023-03-19T08:54:28.394786Z",
-                    "shell.execute_reply": "2023-03-19T08:54:28.394110Z"
+                    "iopub.execute_input": "2024-04-12T12:10:15.159285Z",
+                    "iopub.status.busy": "2024-04-12T12:10:15.158830Z",
+                    "iopub.status.idle": "2024-04-12T12:10:15.164599Z",
+                    "shell.execute_reply": "2024-04-12T12:10:15.163957Z"
                 },
                 "lines_to_next_cell": 0
             },
             "outputs": [],
             "source": [
                 "csv_file = \"../tests/data/SLC6A4_active_excapedb_subset.csv\" # Hmm, maybe better to download directly\n",
                 "data = pd.read_csv(csv_file)"
@@ -67,18 +67,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "id": "594f45ba",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:28.397967Z",
-                    "iopub.status.busy": "2023-03-19T08:54:28.397752Z",
-                    "iopub.status.idle": "2023-03-19T08:54:28.436822Z",
-                    "shell.execute_reply": "2023-03-19T08:54:28.436140Z"
+                    "iopub.execute_input": "2024-04-12T12:10:15.167046Z",
+                    "iopub.status.busy": "2024-04-12T12:10:15.166800Z",
+                    "iopub.status.idle": "2024-04-12T12:10:15.202826Z",
+                    "shell.execute_reply": "2024-04-12T12:10:15.202180Z"
                 },
                 "lines_to_next_cell": 0
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
@@ -102,18 +102,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "id": "ed19f736",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:28.439485Z",
-                    "iopub.status.busy": "2023-03-19T08:54:28.439232Z",
-                    "iopub.status.idle": "2023-03-19T08:54:28.834836Z",
-                    "shell.execute_reply": "2023-03-19T08:54:28.833932Z"
+                    "iopub.execute_input": "2024-04-12T12:10:15.205344Z",
+                    "iopub.status.busy": "2024-04-12T12:10:15.205135Z",
+                    "iopub.status.idle": "2024-04-12T12:10:15.593454Z",
+                    "shell.execute_reply": "2024-04-12T12:10:15.592778Z"
                 },
                 "lines_to_next_cell": 0
             },
             "outputs": [],
             "source": [
                 "from sklearn.pipeline import Pipeline\n",
                 "from sklearn.linear_model import Ridge\n",
@@ -124,18 +124,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "c4a255f4",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:28.838155Z",
-                    "iopub.status.busy": "2023-03-19T08:54:28.837767Z",
-                    "iopub.status.idle": "2023-03-19T08:54:28.842399Z",
-                    "shell.execute_reply": "2023-03-19T08:54:28.841851Z"
+                    "iopub.execute_input": "2024-04-12T12:10:15.596462Z",
+                    "iopub.status.busy": "2024-04-12T12:10:15.595952Z",
+                    "iopub.status.idle": "2024-04-12T12:10:15.601122Z",
+                    "shell.execute_reply": "2024-04-12T12:10:15.600608Z"
                 }
             },
             "outputs": [],
             "source": [
                 "mol_list_train, mol_list_test, y_train, y_test = train_test_split(data.ROMol, data.pXC50, random_state=0)"
             ]
         },
@@ -149,26 +149,26 @@
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "id": "0ddbf668",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:28.845331Z",
-                    "iopub.status.busy": "2023-03-19T08:54:28.845041Z",
-                    "iopub.status.idle": "2023-03-19T08:54:28.851043Z",
-                    "shell.execute_reply": "2023-03-19T08:54:28.850277Z"
+                    "iopub.execute_input": "2024-04-12T12:10:15.603558Z",
+                    "iopub.status.busy": "2024-04-12T12:10:15.603329Z",
+                    "iopub.status.idle": "2024-04-12T12:10:15.608527Z",
+                    "shell.execute_reply": "2024-04-12T12:10:15.608014Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Pipeline(steps=[('mol_transformer', MorganTransformer()),\n",
+                        "Pipeline(steps=[('mol_transformer', MorganFingerprintTransformer()),\n",
                         "                ('Regressor', Ridge())])\n"
                     ]
                 }
             ],
             "source": [
                 "pipe = Pipeline([('mol_transformer', MorganFingerprintTransformer()), ('Regressor', Ridge())])\n",
                 "print(pipe)"
@@ -184,18 +184,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "id": "231d0534",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:28.853975Z",
-                    "iopub.status.busy": "2023-03-19T08:54:28.853718Z",
-                    "iopub.status.idle": "2023-03-19T08:54:28.944670Z",
-                    "shell.execute_reply": "2023-03-19T08:54:28.943808Z"
+                    "iopub.execute_input": "2024-04-12T12:10:15.610826Z",
+                    "iopub.status.busy": "2024-04-12T12:10:15.610623Z",
+                    "iopub.status.idle": "2024-04-12T12:10:15.735973Z",
+                    "shell.execute_reply": "2024-04-12T12:10:15.735308Z"
                 },
                 "lines_to_next_cell": 0
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
@@ -221,18 +221,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "id": "5d1e9220",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:28.949968Z",
-                    "iopub.status.busy": "2023-03-19T08:54:28.949504Z",
-                    "iopub.status.idle": "2023-03-19T08:54:28.964037Z",
-                    "shell.execute_reply": "2023-03-19T08:54:28.963010Z"
+                    "iopub.execute_input": "2024-04-12T12:10:15.738365Z",
+                    "iopub.status.busy": "2024-04-12T12:10:15.738132Z",
+                    "iopub.status.idle": "2024-04-12T12:10:15.744818Z",
+                    "shell.execute_reply": "2024-04-12T12:10:15.744279Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([6.00400299])"
@@ -257,28 +257,29 @@
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "id": "eb8ce486",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:28.969289Z",
-                    "iopub.status.busy": "2023-03-19T08:54:28.968614Z",
-                    "iopub.status.idle": "2023-03-19T08:54:28.983422Z",
-                    "shell.execute_reply": "2023-03-19T08:54:28.982473Z"
+                    "iopub.execute_input": "2024-04-12T12:10:15.747499Z",
+                    "iopub.status.busy": "2024-04-12T12:10:15.746917Z",
+                    "iopub.status.idle": "2024-04-12T12:10:15.754613Z",
+                    "shell.execute_reply": "2024-04-12T12:10:15.754088Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Pipeline(steps=[('smiles_transformer', SmilesToMol()),\n",
+                        "Pipeline(steps=[('smiles_transformer', SmilesToMolTransformer()),\n",
                         "                ('pipe',\n",
-                        "                 Pipeline(steps=[('mol_transformer', MorganTransformer()),\n",
+                        "                 Pipeline(steps=[('mol_transformer',\n",
+                        "                                  MorganFingerprintTransformer()),\n",
                         "                                 ('Regressor', Ridge())]))])\n"
                     ]
                 }
             ],
             "source": [
                 "smiles_pipe = Pipeline([('smiles_transformer', SmilesToMolTransformer()), ('pipe', pipe)])\n",
                 "print(smiles_pipe)"
@@ -286,18 +287,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "id": "1444b605",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:28.988161Z",
-                    "iopub.status.busy": "2023-03-19T08:54:28.987478Z",
-                    "iopub.status.idle": "2023-03-19T08:54:28.995432Z",
-                    "shell.execute_reply": "2023-03-19T08:54:28.994415Z"
+                    "iopub.execute_input": "2024-04-12T12:10:15.757246Z",
+                    "iopub.status.busy": "2024-04-12T12:10:15.756914Z",
+                    "iopub.status.idle": "2024-04-12T12:10:15.761416Z",
+                    "shell.execute_reply": "2024-04-12T12:10:15.760858Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([6.00400299])"
@@ -322,40 +323,40 @@
         },
         {
             "cell_type": "code",
             "execution_count": 11,
             "id": "1eacda8f",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:29.000764Z",
-                    "iopub.status.busy": "2023-03-19T08:54:29.000309Z",
-                    "iopub.status.idle": "2023-03-19T08:54:29.015001Z",
-                    "shell.execute_reply": "2023-03-19T08:54:29.014049Z"
+                    "iopub.execute_input": "2024-04-12T12:10:15.765023Z",
+                    "iopub.status.busy": "2024-04-12T12:10:15.764682Z",
+                    "iopub.status.idle": "2024-04-12T12:10:15.772249Z",
+                    "shell.execute_reply": "2024-04-12T12:10:15.771692Z"
                 },
                 "lines_to_next_cell": 2
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "{'memory': None,\n",
-                            " 'steps': [('smiles_transformer', SmilesToMol()),\n",
+                            " 'steps': [('smiles_transformer', SmilesToMolTransformer()),\n",
                             "  ('pipe',\n",
-                            "   Pipeline(steps=[('mol_transformer', MorganTransformer()),\n",
+                            "   Pipeline(steps=[('mol_transformer', MorganFingerprintTransformer()),\n",
                             "                   ('Regressor', Ridge())]))],\n",
                             " 'verbose': False,\n",
-                            " 'smiles_transformer': SmilesToMol(),\n",
-                            " 'pipe': Pipeline(steps=[('mol_transformer', MorganTransformer()),\n",
+                            " 'smiles_transformer': SmilesToMolTransformer(),\n",
+                            " 'pipe': Pipeline(steps=[('mol_transformer', MorganFingerprintTransformer()),\n",
                             "                 ('Regressor', Ridge())]),\n",
                             " 'smiles_transformer__parallel': False,\n",
                             " 'pipe__memory': None,\n",
-                            " 'pipe__steps': [('mol_transformer', MorganTransformer()),\n",
+                            " 'pipe__steps': [('mol_transformer', MorganFingerprintTransformer()),\n",
                             "  ('Regressor', Ridge())],\n",
                             " 'pipe__verbose': False,\n",
-                            " 'pipe__mol_transformer': MorganTransformer(),\n",
+                            " 'pipe__mol_transformer': MorganFingerprintTransformer(),\n",
                             " 'pipe__Regressor': Ridge(),\n",
                             " 'pipe__mol_transformer__nBits': 2048,\n",
                             " 'pipe__mol_transformer__parallel': False,\n",
                             " 'pipe__mol_transformer__radius': 2,\n",
                             " 'pipe__mol_transformer__useBondTypes': True,\n",
                             " 'pipe__mol_transformer__useChirality': False,\n",
                             " 'pipe__mol_transformer__useCounts': False,\n",
@@ -396,13 +397,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.9"
+            "version": "3.10.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `scikit_mol-0.2.1/notebooks/03_example_pipeline.py` & `scikit_mol-0.3.0/notebooks/03_example_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #   jupytext:
 #     cell_metadata_filter: title,-all
 #     formats: ipynb,py:percent
 #     text_representation:
 #       extension: .py
 #       format_name: percent
 #       format_version: '1.3'
-#       jupytext_version: 1.14.5
+#       jupytext_version: 1.16.1
 #   kernelspec:
 #     display_name: Python 3.9.4 ('rdkit')
 #     language: python
 #     name: python3
 # ---
 
 # %% [markdown]
```

### Comparing `scikit_mol-0.2.1/notebooks/04_standardizer.py` & `scikit_mol-0.3.0/notebooks/04_standardizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #   jupytext:
 #     cell_metadata_filter: -all
 #     formats: ipynb,py:percent
 #     text_representation:
 #       extension: .py
 #       format_name: percent
 #       format_version: '1.3'
-#       jupytext_version: 1.14.5
+#       jupytext_version: 1.16.1
 #   kernelspec:
 #     display_name: Python 3.9.4 ('rdkit')
 #     language: python
 #     name: python3
 # ---
 
 # %% [markdown]
```

### Comparing `scikit_mol-0.2.1/notebooks/04_standardizer_files/04_standardizer_3_0.png` & `scikit_mol-0.3.0/notebooks/04_standardizer_files/04_standardizer_3_0.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/notebooks/04_standardizer_files/04_standardizer_3_1.png` & `scikit_mol-0.3.0/notebooks/04_standardizer_files/04_standardizer_3_1.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/notebooks/05_smiles_sanitaztion.ipynb` & `scikit_mol-0.3.0/notebooks/04_standardizer.ipynb`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.945271164021164%*

 * *Differences: {"'cells'": '{0: {\'id\': \'be682e9c\', \'source\': [\'# Molecule standardization\\n\', "When '*

 * *            'building machine learning models of molecules, it is important to standardize the '*

 * *            "molecules. We often don't want different predictions just because things are drawn in "*

 * *            'slightly different forms, such as protonated or deprotanted carboxylic acids. '*

 * *            'Scikit-mol provides a very basic standardize transformer based on the molvs '*

 * *            'implementation in RDK […]*

```diff
@@ -1,299 +1,229 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "b6fe4dbd",
+            "id": "be682e9c",
             "metadata": {},
             "source": [
-                "# SMILES sanitation\n",
-                "Sometimes we are faced with datasets which has SMILES that rdkit doesn't want to sanitize. This can be human entry errors, or differences between RDKits more strict sanitazion and other toolkits implementations of the parser. e.g. RDKit will not handle a tetravalent nitrogen when it has no charge, where other toolkits may simply build the graph anyway, disregarding the issues with the valence rules or guessing that the nitrogen should have a charge, where it could also by accident instead have a methyl group too many."
+                "# Molecule standardization\n",
+                "When building machine learning models of molecules, it is important to standardize the molecules. We often don't want different predictions just because things are drawn in slightly different forms, such as protonated or deprotanted carboxylic acids. Scikit-mol provides a very basic standardize transformer based on the molvs implementation in RDKit"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
-            "id": "c46f479f",
+            "id": "2aa91923",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:33.431115Z",
-                    "iopub.status.busy": "2023-03-19T08:54:33.430360Z",
-                    "iopub.status.idle": "2023-03-19T08:54:33.801123Z",
-                    "shell.execute_reply": "2023-03-19T08:54:33.800330Z"
+                    "iopub.execute_input": "2024-04-12T12:10:17.122184Z",
+                    "iopub.status.busy": "2024-04-12T12:10:17.121928Z",
+                    "iopub.status.idle": "2024-04-12T12:10:17.878455Z",
+                    "shell.execute_reply": "2024-04-12T12:10:17.877770Z"
                 }
             },
             "outputs": [],
             "source": [
-                "import pandas as pd\n",
-                "from rdkit.Chem import PandasTools\n",
-                "\n",
-                "csv_file = \"../tests/data/SLC6A4_active_excapedb_subset.csv\" # Hmm, maybe better to download directly\n",
-                "data = pd.read_csv(csv_file)\n",
-                "\n"
+                "from rdkit import Chem\n",
+                "from scikit_mol.standardizer import Standardizer\n",
+                "from scikit_mol.fingerprints import MorganFingerprintTransformer\n",
+                "from scikit_mol.conversions import SmilesToMolTransformer\n",
+                "from sklearn.pipeline import make_pipeline\n",
+                "from sklearn.linear_model import Ridge"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "5db46e76",
+            "id": "0fed8d0b",
             "metadata": {},
             "source": [
-                "Now, this example dataset contain all sanitizable SMILES, so for demonstration purposes, we will corrupt one of them"
+                "For demonstration let's create some molecules with different protonation states. The two first molecules are Benzoic acid and Sodium benzoate."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
-            "id": "a7bc5ff6",
+            "id": "934c031b",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:33.804206Z",
-                    "iopub.status.busy": "2023-03-19T08:54:33.803981Z",
-                    "iopub.status.idle": "2023-03-19T08:54:33.807721Z",
-                    "shell.execute_reply": "2023-03-19T08:54:33.807162Z"
+                    "iopub.execute_input": "2024-04-12T12:10:17.881422Z",
+                    "iopub.status.busy": "2024-04-12T12:10:17.881092Z",
+                    "iopub.status.idle": "2024-04-12T12:10:17.889228Z",
+                    "shell.execute_reply": "2024-04-12T12:10:17.888702Z"
                 }
             },
-            "outputs": [],
-            "source": [
-                "data.loc[1,'SMILES'] = 'CN(C)(C)(C)'"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 3,
-            "id": "a792f370",
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:33.810589Z",
-                    "iopub.status.busy": "2023-03-19T08:54:33.810336Z",
-                    "iopub.status.idle": "2023-03-19T08:54:33.849855Z",
-                    "shell.execute_reply": "2023-03-19T08:54:33.849118Z"
-                },
-                "lines_to_next_cell": 2
-            },
             "outputs": [
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Dataset contains 1 unparsable mols\n"
-                    ]
+                    "data": {
+                        "text/plain": [
+                            "array([<rdkit.Chem.rdchem.Mol object at 0x7da9b28bb060>], dtype=object)"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
                 },
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[09:54:33] Explicit valence for atom # 1 N, 4, is greater than permitted\n"
-                    ]
+                    "data": {
+                        "text/plain": [
+                            "array([<rdkit.Chem.rdchem.Mol object at 0x7da9b28bb0d0>], dtype=object)"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
                 }
             ],
             "source": [
+                "smiles_strings = ('c1ccccc1C(=O)[OH]','c1ccccc1C(=O)[O-].[Na+]','CC[NH+](C)C','CC[N+](C)(C)C',\n",
+                "       '[O-]CC(C(=O)[O-])C[NH+](C)C','[O-]CC(C(=O)[O-])C[N+](C)(C)C')\n",
+                "\n",
+                "smi2mol = SmilesToMolTransformer()\n",
                 "\n",
-                "PandasTools.AddMoleculeColumnToFrame(data, smilesCol=\"SMILES\")\n",
-                "print(f'Dataset contains {data.ROMol.isna().sum()} unparsable mols')"
+                "mols  = smi2mol.transform(smiles_strings)\n",
+                "for mol in mols[0:2]:\n",
+                "    display(mol)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "54341ece",
+            "id": "e68b0eff",
             "metadata": {},
             "source": [
-                "If we use these SMILES for the scikit-learn pipeline, we would face an error, so we need to check and clean the dataset first. The CheckSmilesSanitation can help us with that."
+                "We can simply use the transformer directly and get a list of standardized molecules"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
-            "id": "849b643f",
+            "execution_count": 3,
+            "id": "c18bbd3e",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:33.852625Z",
-                    "iopub.status.busy": "2023-03-19T08:54:33.852342Z",
-                    "iopub.status.idle": "2023-03-19T08:54:33.894579Z",
-                    "shell.execute_reply": "2023-03-19T08:54:33.893765Z"
+                    "iopub.execute_input": "2024-04-12T12:10:17.891559Z",
+                    "iopub.status.busy": "2024-04-12T12:10:17.891342Z",
+                    "iopub.status.idle": "2024-04-12T12:10:17.906792Z",
+                    "shell.execute_reply": "2024-04-12T12:10:17.906295Z"
                 }
             },
             "outputs": [
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Error in parsing 1 SMILES. Unparsable SMILES can be found in self.errors\n"
-                    ]
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[09:54:33] Explicit valence for atom # 1 N, 4, is greater than permitted\n"
-                    ]
+                    "data": {
+                        "text/plain": [
+                            "array([['O=C(O)c1ccccc1'],\n",
+                            "       ['O=C(O)c1ccccc1'],\n",
+                            "       ['CCN(C)C'],\n",
+                            "       ['CC[N+](C)(C)C'],\n",
+                            "       ['CN(C)CC(CO)C(=O)O'],\n",
+                            "       ['C[N+](C)(C)CC(CO)C(=O)[O-]']], dtype='<U26')"
+                        ]
+                    },
+                    "execution_count": 3,
+                    "metadata": {},
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
-                "from scikit_mol.utilities import CheckSmilesSanitazion\n",
-                "smileschecker = CheckSmilesSanitazion()\n",
-                "\n",
-                "smiles_list_valid, y_valid, smiles_errors, y_errors = smileschecker.sanitize(list(data.SMILES), list(data.pXC50))"
+                "# You can just run straight up like this. Note that neutralising is optional\n",
+                "standardizer = Standardizer(neutralize=True)\n",
+                "standard_mols = standardizer.transform(mols)\n",
+                "standard_smiles = smi2mol.inverse_transform(standard_mols)\n",
+                "standard_smiles"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "5e410e4c",
+            "id": "da3fc3e2",
             "metadata": {},
             "source": [
-                "Now the smiles_list_valid should be all valid and the y_values filtered as well. Errors are returned, but also accesible after the call to .sanitize() in the .errors property"
+                "Some of the molecules were desalted and neutralized.\n",
+                "\n",
+                "A typical usecase would be to add the standardizer to a pipeline for prediction"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
-            "id": "2145530c",
+            "execution_count": 4,
+            "id": "d03be7dc",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:33.897271Z",
-                    "iopub.status.busy": "2023-03-19T08:54:33.896965Z",
-                    "iopub.status.idle": "2023-03-19T08:54:33.910201Z",
-                    "shell.execute_reply": "2023-03-19T08:54:33.909540Z"
-                }
+                    "iopub.execute_input": "2024-04-12T12:10:17.909344Z",
+                    "iopub.status.busy": "2024-04-12T12:10:17.909132Z",
+                    "iopub.status.idle": "2024-04-12T12:10:17.939678Z",
+                    "shell.execute_reply": "2024-04-12T12:10:17.939104Z"
+                },
+                "lines_to_next_cell": 2
             },
             "outputs": [
                 {
-                    "data": {
-                        "text/html": [
-                            "<div>\n",
-                            "<style scoped>\n",
-                            "    .dataframe tbody tr th:only-of-type {\n",
-                            "        vertical-align: middle;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe tbody tr th {\n",
-                            "        vertical-align: top;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe thead th {\n",
-                            "        text-align: right;\n",
-                            "    }\n",
-                            "</style>\n",
-                            "<table border=\"1\" class=\"dataframe\">\n",
-                            "  <thead>\n",
-                            "    <tr style=\"text-align: right;\">\n",
-                            "      <th></th>\n",
-                            "      <th>SMILES</th>\n",
-                            "      <th>y</th>\n",
-                            "    </tr>\n",
-                            "  </thead>\n",
-                            "  <tbody>\n",
-                            "    <tr>\n",
-                            "      <th>0</th>\n",
-                            "      <td>CN(C)(C)(C)</td>\n",
-                            "      <td>7.18046</td>\n",
-                            "    </tr>\n",
-                            "  </tbody>\n",
-                            "</table>\n",
-                            "</div>"
-                        ],
-                        "text/plain": [
-                            "        SMILES        y\n",
-                            "0  CN(C)(C)(C)  7.18046"
-                        ]
-                    },
-                    "execution_count": 5,
-                    "metadata": {},
-                    "output_type": "execute_result"
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Predictions with no standardization: [0.51983795 0.51983795 2.06562022 3.01206795 3.95446692 4.92816899]\n",
+                        "Predictions with standardization:    [0.51983795 0.61543701 2.31738354 3.01206795 3.44085399 4.37516731]\n"
+                    ]
                 }
             ],
             "source": [
-                "smileschecker.errors"
+                "# Typical use case is to use it in an sklearn pipeline, like below \n",
+                "predictor = Ridge()\n",
+                "\n",
+                "std_pipe = make_pipeline(SmilesToMolTransformer(), Standardizer(), MorganFingerprintTransformer(useCounts=True), predictor)\n",
+                "nonstd_pipe = make_pipeline(SmilesToMolTransformer(), MorganFingerprintTransformer(useCounts=True), predictor)\n",
+                "\n",
+                "fake_y = range(len(smiles_strings))\n",
+                "\n",
+                "std_pipe.fit(smiles_strings, fake_y)\n",
+                "\n",
+                "\n",
+                "print(f'Predictions with no standardization: {std_pipe.predict(smiles_strings)}')\n",
+                "print(f'Predictions with standardization:    {nonstd_pipe.predict(smiles_strings)}')"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "c9906a45",
+            "id": "9cfab56c",
             "metadata": {},
             "source": [
-                "The checker can also be used only on X"
+                "As we can see, the predictions with the standardizer and without are different. The two first molecules were benzoic acid and sodium benzoate, which with the standardized pipeline is predicted as the same, but differently with the nonstandardized pipeline. Wheter we want to make the prediction on the parent compound, or predict the exact form, will of course depend on the use-case, but now there is at least a way to handle it easily in pipelined predictors.\n",
+                "\n",
+                "The example also demonstrate another feature. We created the ridge regressor before creating the two pipelines. Fitting one of the pipelines thus also updated the object in the other pipeline. This can be useful for building inference pipelines that takes in SMILES molecules, but rather do the fitting on already converted and standardized molecules. However, be aware that the crossvalidation classes of scikit-learn may clone the estimators internally when doing the search loop, which would break this interdependence, and necessitate the rebuilding of the inference pipeline.\n",
+                "\n",
+                "If we had fitted the non standardizing pipeline, the model would have been different as shown below, as some of the molecules would be perceived different by the Ridge regressor."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
-            "id": "d5fd425e",
+            "execution_count": 5,
+            "id": "e5f8495f",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:33.913053Z",
-                    "iopub.status.busy": "2023-03-19T08:54:33.912806Z",
-                    "iopub.status.idle": "2023-03-19T08:54:33.956093Z",
-                    "shell.execute_reply": "2023-03-19T08:54:33.955470Z"
+                    "iopub.execute_input": "2024-04-12T12:10:17.942493Z",
+                    "iopub.status.busy": "2024-04-12T12:10:17.942248Z",
+                    "iopub.status.idle": "2024-04-12T12:10:17.961792Z",
+                    "shell.execute_reply": "2024-04-12T12:10:17.961206Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Error in parsing 1 SMILES. Unparsable SMILES can be found in self.errors\n"
+                        "Predictions with no standardization: [0.07445775 0.07445775 2.32132164 3.00857908 2.68502208 4.30275549]\n",
+                        "Predictions with standardization:    [0.07445775 0.96053374 2.05993278 3.00857908 3.96365443 4.93284221]\n"
                     ]
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[09:54:33] Explicit valence for atom # 1 N, 4, is greater than permitted\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "text/html": [
-                            "<div>\n",
-                            "<style scoped>\n",
-                            "    .dataframe tbody tr th:only-of-type {\n",
-                            "        vertical-align: middle;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe tbody tr th {\n",
-                            "        vertical-align: top;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe thead th {\n",
-                            "        text-align: right;\n",
-                            "    }\n",
-                            "</style>\n",
-                            "<table border=\"1\" class=\"dataframe\">\n",
-                            "  <thead>\n",
-                            "    <tr style=\"text-align: right;\">\n",
-                            "      <th></th>\n",
-                            "      <th>SMILES</th>\n",
-                            "    </tr>\n",
-                            "  </thead>\n",
-                            "  <tbody>\n",
-                            "    <tr>\n",
-                            "      <th>0</th>\n",
-                            "      <td>CN(C)(C)(C)</td>\n",
-                            "    </tr>\n",
-                            "  </tbody>\n",
-                            "</table>\n",
-                            "</div>"
-                        ],
-                        "text/plain": [
-                            "        SMILES\n",
-                            "0  CN(C)(C)(C)"
-                        ]
-                    },
-                    "execution_count": 6,
-                    "metadata": {},
-                    "output_type": "execute_result"
                 }
             ],
             "source": [
-                "smiles_list_valid, X_errors = smileschecker.sanitize(list(data.SMILES))\n",
-                "smileschecker.errors"
+                "nonstd_pipe.fit(smiles_strings, fake_y)\n",
+                "print(f'Predictions with no standardization: {std_pipe.predict(smiles_strings)}')\n",
+                "print(f'Predictions with standardization:    {nonstd_pipe.predict(smiles_strings)}')"
             ]
         }
     ],
     "metadata": {
         "jupytext": {
+            "cell_metadata_filter": "-all",
             "formats": "ipynb,py:percent"
         },
         "kernelspec": {
             "display_name": "Python 3.9.4 ('rdkit')",
             "language": "python",
             "name": "python3"
         },
@@ -303,13 +233,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.9"
+            "version": "3.10.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `scikit_mol-0.2.1/notebooks/05_smiles_sanitaztion.py` & `scikit_mol-0.3.0/notebooks/05_smiles_sanitaztion.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # jupyter:
 #   jupytext:
 #     formats: ipynb,py:percent
 #     text_representation:
 #       extension: .py
 #       format_name: percent
 #       format_version: '1.3'
-#       jupytext_version: 1.14.5
+#       jupytext_version: 1.16.1
 #   kernelspec:
 #     display_name: Python 3.9.4 ('rdkit')
 #     language: python
 #     name: python3
 # ---
 
 # %% [markdown]
```

### Comparing `scikit_mol-0.2.1/notebooks/06_hyperparameter_tuning.ipynb` & `scikit_mol-0.3.0/notebooks/06_hyperparameter_tuning.ipynb`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965534749779541%*

 * *Differences: {"'cells'": "{1: {'metadata': {'execution': {'iopub.execute_input': '2024-04-12T12:10:21.479028Z', "*

 * *            "'iopub.status.busy': '2024-04-12T12:10:21.478831Z', 'iopub.status.idle': "*

 * *            "'2024-04-12T12:10:22.543557Z', 'shell.execute_reply': "*

 * *            "'2024-04-12T12:10:22.542929Z'}}}, 3: {'metadata': {'execution': "*

 * *            "{'iopub.execute_input': '2024-04-12T12:10:22.546506Z', 'iopub.status.busy': "*

 * *            "'2024-04-12T12:10:22.546207Z', 'iopub.status.idle': '2024-04-12T12:10:2 […]*

```diff
@@ -12,18 +12,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "7df4793c",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:35.701525Z",
-                    "iopub.status.busy": "2023-03-19T08:54:35.700822Z",
-                    "iopub.status.idle": "2023-03-19T08:54:37.014139Z",
-                    "shell.execute_reply": "2023-03-19T08:54:37.013259Z"
+                    "iopub.execute_input": "2024-04-12T12:10:21.479028Z",
+                    "iopub.status.busy": "2024-04-12T12:10:21.478831Z",
+                    "iopub.status.idle": "2024-04-12T12:10:22.543557Z",
+                    "shell.execute_reply": "2024-04-12T12:10:22.542929Z"
                 }
             },
             "outputs": [],
             "source": [
                 "import os\n",
                 "import rdkit\n",
                 "from rdkit import Chem\n",
@@ -49,18 +49,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "45a8ebf1",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:37.017824Z",
-                    "iopub.status.busy": "2023-03-19T08:54:37.017350Z",
-                    "iopub.status.idle": "2023-03-19T08:54:37.022818Z",
-                    "shell.execute_reply": "2023-03-19T08:54:37.022080Z"
+                    "iopub.execute_input": "2024-04-12T12:10:22.546506Z",
+                    "iopub.status.busy": "2024-04-12T12:10:22.546207Z",
+                    "iopub.status.idle": "2024-04-12T12:10:22.550011Z",
+                    "shell.execute_reply": "2024-04-12T12:10:22.549526Z"
                 }
             },
             "outputs": [],
             "source": [
                 "full_set = False\n",
                 "\n",
                 "if full_set:\n",
@@ -83,18 +83,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "id": "08c233a7",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:37.025520Z",
-                    "iopub.status.busy": "2023-03-19T08:54:37.025310Z",
-                    "iopub.status.idle": "2023-03-19T08:54:37.077231Z",
-                    "shell.execute_reply": "2023-03-19T08:54:37.076469Z"
+                    "iopub.execute_input": "2024-04-12T12:10:22.552652Z",
+                    "iopub.status.busy": "2024-04-12T12:10:22.552186Z",
+                    "iopub.status.idle": "2024-04-12T12:10:22.591597Z",
+                    "shell.execute_reply": "2024-04-12T12:10:22.591017Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -120,25 +120,25 @@
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "id": "5363d05a",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:37.080021Z",
-                    "iopub.status.busy": "2023-03-19T08:54:37.079756Z",
-                    "iopub.status.idle": "2023-03-19T08:54:37.084574Z",
-                    "shell.execute_reply": "2023-03-19T08:54:37.084021Z"
+                    "iopub.execute_input": "2024-04-12T12:10:22.594077Z",
+                    "iopub.status.busy": "2024-04-12T12:10:22.593866Z",
+                    "iopub.status.idle": "2024-04-12T12:10:22.598774Z",
+                    "shell.execute_reply": "2024-04-12T12:10:22.598212Z"
                 },
                 "lines_to_next_cell": 2
             },
             "outputs": [],
             "source": [
                 "\n",
-                "mol_list_train, mol_list_test, y_train, y_test = train_test_split(data.ROMol, data.pXC50, random_state=0)"
+                "mol_list_train, mol_list_test, y_train, y_test = train_test_split(data.ROMol, data.pXC50, random_state=42)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "bf9e8c8d",
             "metadata": {},
             "source": [
@@ -147,18 +147,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "885daf12",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:37.087530Z",
-                    "iopub.status.busy": "2023-03-19T08:54:37.087275Z",
-                    "iopub.status.idle": "2023-03-19T08:54:37.454935Z",
-                    "shell.execute_reply": "2023-03-19T08:54:37.454153Z"
+                    "iopub.execute_input": "2024-04-12T12:10:22.601148Z",
+                    "iopub.status.busy": "2024-04-12T12:10:22.600938Z",
+                    "iopub.status.idle": "2024-04-12T12:10:22.967869Z",
+                    "shell.execute_reply": "2024-04-12T12:10:22.967178Z"
                 }
             },
             "outputs": [],
             "source": [
                 "# Probably the recommended way would be to prestandardize the data if there's no changes to the transformer, \n",
                 "# and then add the standardizer in the inference pipeline.\n",
                 "\n",
@@ -178,18 +178,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "id": "8fd14250",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:37.458340Z",
-                    "iopub.status.busy": "2023-03-19T08:54:37.458092Z",
-                    "iopub.status.idle": "2023-03-19T08:54:37.461663Z",
-                    "shell.execute_reply": "2023-03-19T08:54:37.461052Z"
+                    "iopub.execute_input": "2024-04-12T12:10:22.970766Z",
+                    "iopub.status.busy": "2024-04-12T12:10:22.970539Z",
+                    "iopub.status.idle": "2024-04-12T12:10:22.973715Z",
+                    "shell.execute_reply": "2024-04-12T12:10:22.973234Z"
                 }
             },
             "outputs": [],
             "source": [
                 "\n",
                 "moltransformer = MorganFingerprintTransformer()\n",
                 "regressor = Ridge()\n",
@@ -208,25 +208,26 @@
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "id": "fa082078",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:37.464188Z",
-                    "iopub.status.busy": "2023-03-19T08:54:37.463905Z",
-                    "iopub.status.idle": "2023-03-19T08:54:37.467187Z",
-                    "shell.execute_reply": "2023-03-19T08:54:37.466548Z"
+                    "iopub.execute_input": "2024-04-12T12:10:22.976061Z",
+                    "iopub.status.busy": "2024-04-12T12:10:22.975846Z",
+                    "iopub.status.idle": "2024-04-12T12:10:22.978721Z",
+                    "shell.execute_reply": "2024-04-12T12:10:22.978155Z"
                 },
                 "title": "Now hyperparameter tuning"
             },
             "outputs": [],
             "source": [
                 "from sklearn.model_selection import RandomizedSearchCV\n",
-                "from sklearn.utils.fixes import loguniform"
+                "#from sklearn.utils.fixes import loguniform\n",
+                "from scipy.stats import loguniform"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "fa2a316a",
             "metadata": {},
             "source": [
@@ -235,26 +236,26 @@
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "id": "046e24d3",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:37.470133Z",
-                    "iopub.status.busy": "2023-03-19T08:54:37.469879Z",
-                    "iopub.status.idle": "2023-03-19T08:54:37.476370Z",
-                    "shell.execute_reply": "2023-03-19T08:54:37.475763Z"
+                    "iopub.execute_input": "2024-04-12T12:10:22.981002Z",
+                    "iopub.status.busy": "2024-04-12T12:10:22.980797Z",
+                    "iopub.status.idle": "2024-04-12T12:10:22.986820Z",
+                    "shell.execute_reply": "2024-04-12T12:10:22.986344Z"
                 },
                 "title": "Which keys do we have?"
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "dict_keys(['memory', 'steps', 'verbose', 'morgantransformer', 'ridge', 'morgantransformer__nBits', 'morgantransformer__parallel', 'morgantransformer__radius', 'morgantransformer__useBondTypes', 'morgantransformer__useChirality', 'morgantransformer__useCounts', 'morgantransformer__useFeatures', 'ridge__alpha', 'ridge__copy_X', 'ridge__fit_intercept', 'ridge__max_iter', 'ridge__positive', 'ridge__random_state', 'ridge__solver', 'ridge__tol'])"
+                            "dict_keys(['memory', 'steps', 'verbose', 'morganfingerprinttransformer', 'ridge', 'morganfingerprinttransformer__nBits', 'morganfingerprinttransformer__parallel', 'morganfingerprinttransformer__radius', 'morganfingerprinttransformer__useBondTypes', 'morganfingerprinttransformer__useChirality', 'morganfingerprinttransformer__useCounts', 'morganfingerprinttransformer__useFeatures', 'ridge__alpha', 'ridge__copy_X', 'ridge__fit_intercept', 'ridge__max_iter', 'ridge__positive', 'ridge__random_state', 'ridge__solver', 'ridge__tol'])"
                         ]
                     },
                     "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -273,29 +274,29 @@
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "id": "cf2c45d7",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:37.478959Z",
-                    "iopub.status.busy": "2023-03-19T08:54:37.478683Z",
-                    "iopub.status.idle": "2023-03-19T08:54:37.483305Z",
-                    "shell.execute_reply": "2023-03-19T08:54:37.482688Z"
+                    "iopub.execute_input": "2024-04-12T12:10:22.989460Z",
+                    "iopub.status.busy": "2024-04-12T12:10:22.988970Z",
+                    "iopub.status.idle": "2024-04-12T12:10:22.993117Z",
+                    "shell.execute_reply": "2024-04-12T12:10:22.992622Z"
                 },
                 "lines_to_next_cell": 1
             },
             "outputs": [],
             "source": [
                 "\n",
                 "param_dist = {'ridge__alpha': loguniform(1e-2, 1e3),\n",
-                "            \"morgantransformer__nBits\": [256,512,1024,2048,4096],\n",
-                "            'morgantransformer__radius':[1,2,3,4],\n",
-                "            'morgantransformer__useCounts': [True,False],\n",
-                "            'morgantransformer__useFeatures':[True,False]}"
+                "            \"morganfingerprinttransformer__nBits\": [256,512,1024,2048,4096],\n",
+                "            'morganfingerprinttransformer__radius':[1,2,3,4],\n",
+                "            'morganfingerprinttransformer__useCounts': [True,False],\n",
+                "            'morganfingerprinttransformer__useFeatures':[True,False]}"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d61fc18c",
             "metadata": {},
             "source": [
@@ -304,18 +305,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "id": "fbb2cacd",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:37.485906Z",
-                    "iopub.status.busy": "2023-03-19T08:54:37.485645Z",
-                    "iopub.status.idle": "2023-03-19T08:54:37.489973Z",
-                    "shell.execute_reply": "2023-03-19T08:54:37.489382Z"
+                    "iopub.execute_input": "2024-04-12T12:10:22.995477Z",
+                    "iopub.status.busy": "2024-04-12T12:10:22.995281Z",
+                    "iopub.status.idle": "2024-04-12T12:10:22.999317Z",
+                    "shell.execute_reply": "2024-04-12T12:10:22.998769Z"
                 },
                 "title": "From https://scikit-learn.org/stable/auto_examples/model_selection/plot_randomized_search.html#sphx-glr-auto-examples-model-selection-plot-randomized-search-py"
             },
             "outputs": [],
             "source": [
                 "# Utility function to report best scores\n",
                 "def report(results, n_top=3):\n",
@@ -343,26 +344,26 @@
         },
         {
             "cell_type": "code",
             "execution_count": 11,
             "id": "bc66efa3",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:37.492677Z",
-                    "iopub.status.busy": "2023-03-19T08:54:37.492327Z",
-                    "iopub.status.idle": "2023-03-19T08:54:44.019837Z",
-                    "shell.execute_reply": "2023-03-19T08:54:44.018820Z"
+                    "iopub.execute_input": "2024-04-12T12:10:23.001598Z",
+                    "iopub.status.busy": "2024-04-12T12:10:23.001400Z",
+                    "iopub.status.idle": "2024-04-12T12:10:27.149245Z",
+                    "shell.execute_reply": "2024-04-12T12:10:27.148640Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Runtime: 6.52 for 25 iterations)\n"
+                        "Runtime: 4.14 for 25 iterations)\n"
                     ]
                 }
             ],
             "source": [
                 "n_iter_search = 25\n",
                 "random_search = RandomizedSearchCV(\n",
                 "    optimization_pipe, param_distributions=param_dist, n_iter=n_iter_search, cv=3\n",
@@ -376,37 +377,37 @@
         },
         {
             "cell_type": "code",
             "execution_count": 12,
             "id": "b2b3d623",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:44.026632Z",
-                    "iopub.status.busy": "2023-03-19T08:54:44.024799Z",
-                    "iopub.status.idle": "2023-03-19T08:54:44.034480Z",
-                    "shell.execute_reply": "2023-03-19T08:54:44.033518Z"
+                    "iopub.execute_input": "2024-04-12T12:10:27.153307Z",
+                    "iopub.status.busy": "2024-04-12T12:10:27.152284Z",
+                    "iopub.status.idle": "2024-04-12T12:10:27.157929Z",
+                    "shell.execute_reply": "2024-04-12T12:10:27.157394Z"
                 },
                 "lines_to_next_cell": 0
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Model with rank: 1\n",
-                        "Mean validation score: 0.492 (std: 0.048)\n",
-                        "Parameters: {'morgantransformer__nBits': 2048, 'morgantransformer__radius': 4, 'morgantransformer__useCounts': False, 'morgantransformer__useFeatures': False, 'ridge__alpha': 18.49687467370123}\n",
+                        "Mean validation score: 0.539 (std: 0.090)\n",
+                        "Parameters: {'morganfingerprinttransformer__nBits': 2048, 'morganfingerprinttransformer__radius': 1, 'morganfingerprinttransformer__useCounts': False, 'morganfingerprinttransformer__useFeatures': False, 'ridge__alpha': 10.016632822744322}\n",
                         "\n",
                         "Model with rank: 2\n",
-                        "Mean validation score: 0.446 (std: 0.188)\n",
-                        "Parameters: {'morgantransformer__nBits': 256, 'morgantransformer__radius': 2, 'morgantransformer__useCounts': False, 'morgantransformer__useFeatures': False, 'ridge__alpha': 0.22311472368521185}\n",
+                        "Mean validation score: 0.534 (std: 0.145)\n",
+                        "Parameters: {'morganfingerprinttransformer__nBits': 2048, 'morganfingerprinttransformer__radius': 3, 'morganfingerprinttransformer__useCounts': False, 'morganfingerprinttransformer__useFeatures': False, 'ridge__alpha': 0.7814453905088184}\n",
                         "\n",
                         "Model with rank: 3\n",
-                        "Mean validation score: 0.440 (std: 0.025)\n",
-                        "Parameters: {'morgantransformer__nBits': 4096, 'morgantransformer__radius': 3, 'morgantransformer__useCounts': False, 'morgantransformer__useFeatures': True, 'ridge__alpha': 6.023414585108017}\n",
+                        "Mean validation score: 0.526 (std: 0.090)\n",
+                        "Parameters: {'morganfingerprinttransformer__nBits': 4096, 'morganfingerprinttransformer__radius': 1, 'morganfingerprinttransformer__useCounts': False, 'morganfingerprinttransformer__useFeatures': False, 'ridge__alpha': 11.295262712617353}\n",
                         "\n"
                     ]
                 }
             ],
             "source": [
                 "report(random_search.cv_results_)"
             ]
@@ -429,27 +430,27 @@
         },
         {
             "cell_type": "code",
             "execution_count": 13,
             "id": "cb369a0e",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:44.041562Z",
-                    "iopub.status.busy": "2023-03-19T08:54:44.039729Z",
-                    "iopub.status.idle": "2023-03-19T08:54:44.258048Z",
-                    "shell.execute_reply": "2023-03-19T08:54:44.256978Z"
+                    "iopub.execute_input": "2024-04-12T12:10:27.161728Z",
+                    "iopub.status.busy": "2024-04-12T12:10:27.160746Z",
+                    "iopub.status.idle": "2024-04-12T12:10:27.316434Z",
+                    "shell.execute_reply": "2024-04-12T12:10:27.315830Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "No Standardization 0.5222\n",
-                        "With Standardization 0.5222\n"
+                        "No Standardization 0.5379\n",
+                        "With Standardization 0.5379\n"
                     ]
                 }
             ],
             "source": [
                 "inference_pipe = make_pipeline(standardizer, random_search.best_estimator_)\n",
                 "\n",
                 "print(f'No Standardization {random_search.best_estimator_.score(mol_list_test, y_test):0.4F}')\n",
@@ -473,27 +474,27 @@
         },
         {
             "cell_type": "code",
             "execution_count": 14,
             "id": "f6426b23",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:44.264895Z",
-                    "iopub.status.busy": "2023-03-19T08:54:44.264460Z",
-                    "iopub.status.idle": "2023-03-19T08:54:44.295917Z",
-                    "shell.execute_reply": "2023-03-19T08:54:44.294841Z"
+                    "iopub.execute_input": "2024-04-12T12:10:27.320951Z",
+                    "iopub.status.busy": "2024-04-12T12:10:27.319924Z",
+                    "iopub.status.idle": "2024-04-12T12:10:27.337918Z",
+                    "shell.execute_reply": "2024-04-12T12:10:27.337344Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Predictions with no standardization: [6.29056823 6.31806374 6.34706809 6.44119607 6.41499794]\n",
-                        "Predictions with standardization:    [6.29056823 6.29056823 6.29056823 6.29056823 6.29056823]\n"
+                        "Predictions with no standardization: [5.95334818 5.99768591 5.99768591 6.31509408 6.09785566]\n",
+                        "Predictions with standardization:    [5.95334818 5.95334818 5.95334818 5.95334818 5.95334818]\n"
                     ]
                 }
             ],
             "source": [
                 "# Intergrating the Standardizer and challenge it with some different forms and salts of benzoic acid\n",
                 "smiles_list = ['c1ccccc1C(=O)[OH]', 'c1ccccc1C(=O)[O-]', 'c1ccccc1C(=O)[O-].[Na+]', 'c1ccccc1C(=O)[O][Na]', 'c1ccccc1C(=O)[O-].C[N+](C)C']\n",
                 "mols_list = [Chem.MolFromSmiles(smiles) for smiles in smiles_list]\n",
@@ -535,13 +536,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.9"
+            "version": "3.10.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `scikit_mol-0.2.1/notebooks/06_hyperparameter_tuning.py` & `scikit_mol-0.3.0/notebooks/06_hyperparameter_tuning.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #   jupytext:
 #     cell_metadata_filter: title,-all
 #     formats: ipynb,py:percent
 #     text_representation:
 #       extension: .py
 #       format_name: percent
 #       format_version: '1.3'
-#       jupytext_version: 1.14.5
+#       jupytext_version: 1.16.1
 #   kernelspec:
 #     display_name: Python 3.9.4 ('rdkit')
 #     language: python
 #     name: python3
 # ---
 
 # %% [markdown]
@@ -60,15 +60,15 @@
 print(f"{data.ROMol.isna().sum()} out of {len(data)} SMILES failed in conversion")
 
 # %% [markdown]
 # We use the train_test_split to, well, split the dataframe's molecule columns and pXC50 column into lists for train and testing
 
 # %%
 
-mol_list_train, mol_list_test, y_train, y_test = train_test_split(data.ROMol, data.pXC50, random_state=0)
+mol_list_train, mol_list_test, y_train, y_test = train_test_split(data.ROMol, data.pXC50, random_state=42)
 
 
 # %% [markdown]
 # We will standardize the molecules before modelling. This is best done before the hyperparameter optimizatiion of the featurization with the scikit-mol transformer and regression modelling, as the standardization is otherwise done for every loop in the hyperparameter optimization, which will make it take longer time.
 
 # %%
 # Probably the recommended way would be to prestandardize the data if there's no changes to the transformer, 
@@ -92,33 +92,34 @@
 
 
 # %% [markdown]
 # For hyperparameter optimization we import the RandomizedSearchCV class from Scikit-Learn. It will try different random combinations of settings and use internal cross-validation to find the best model. In the end, it will fit the best found parameters on the full set. We also import loguniform, to get a better sampling of some of the parameters.
 
 # %% Now hyperparameter tuning
 from sklearn.model_selection import RandomizedSearchCV
-from sklearn.utils.fixes import loguniform
+#from sklearn.utils.fixes import loguniform
+from scipy.stats import loguniform
 
 # %% [markdown]
 # With the pipelines, getting the names of the parameters to tune is a bit more tricky, as they are concatenations of the name of the step and the parameter with double underscores in between. We can get the available parameters from the pipeline with the get_params() method, and select the parameters we want to change from there.
 
 # %% Which keys do we have?
 
 optimization_pipe.get_params().keys()
 
 # %% [markdown]
 # We will tune the regularization strength of the Ridge regressor, and try out different parameters for the Morgan fingerprint, namely the number of bits, the radius of the fingerprint, wheter to use counts or bits and features.
 
 # %%
 
 param_dist = {'ridge__alpha': loguniform(1e-2, 1e3),
-            "morgantransformer__nBits": [256,512,1024,2048,4096],
-            'morgantransformer__radius':[1,2,3,4],
-            'morgantransformer__useCounts': [True,False],
-            'morgantransformer__useFeatures':[True,False]}
+            "morganfingerprinttransformer__nBits": [256,512,1024,2048,4096],
+            'morganfingerprinttransformer__radius':[1,2,3,4],
+            'morganfingerprinttransformer__useCounts': [True,False],
+            'morganfingerprinttransformer__useFeatures':[True,False]}
 
 # %% [markdown]
 # The report function was taken from [this example](https://scikit-learn.org/stable/auto_examples/model_selection/plot_randomized_search.html#sphx-glr-auto-examples-model-selection-plot-randomized-search-py) from the scikit learn documentation.
 
 # %% From https://scikit-learn.org/stable/auto_examples/model_selection/plot_randomized_search.html#sphx-glr-auto-examples-model-selection-plot-randomized-search-py
 # Utility function to report best scores
 def report(results, n_top=3):
```

### Comparing `scikit_mol-0.2.1/notebooks/07_parallel_transforms.ipynb` & `scikit_mol-0.3.0/notebooks/07_parallel_transforms.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9963083791208791%*

 * *Differences: {"'cells'": "{1: {'metadata': {'execution': {'iopub.execute_input': '2024-04-12T12:10:28.855965Z', "*

 * *            "'iopub.status.busy': '2024-04-12T12:10:28.855774Z', 'iopub.status.idle': "*

 * *            "'2024-04-12T12:10:29.593405Z', 'shell.execute_reply': "*

 * *            "'2024-04-12T12:10:29.592709Z'}}}, 3: {'metadata': {'execution': "*

 * *            "{'iopub.execute_input': '2024-04-12T12:10:29.596321Z', 'iopub.status.busy': "*

 * *            "'2024-04-12T12:10:29.596022Z', 'iopub.status.idle': '2024-04-12T12:10:2 […]*

```diff
@@ -14,18 +14,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "d34a6f7e",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:46.001221Z",
-                    "iopub.status.busy": "2023-03-19T08:54:46.000726Z",
-                    "iopub.status.idle": "2023-03-19T08:54:46.882639Z",
-                    "shell.execute_reply": "2023-03-19T08:54:46.881724Z"
+                    "iopub.execute_input": "2024-04-12T12:10:28.855965Z",
+                    "iopub.status.busy": "2024-04-12T12:10:28.855774Z",
+                    "iopub.status.idle": "2024-04-12T12:10:29.593405Z",
+                    "shell.execute_reply": "2024-04-12T12:10:29.592709Z"
                 }
             },
             "outputs": [],
             "source": [
                 "from rdkit.Chem import PandasTools\n",
                 "import pandas as pd\n",
                 "import time\n",
@@ -50,18 +50,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "f59b0883",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:46.887587Z",
-                    "iopub.status.busy": "2023-03-19T08:54:46.886796Z",
-                    "iopub.status.idle": "2023-03-19T08:54:46.891008Z",
-                    "shell.execute_reply": "2023-03-19T08:54:46.890486Z"
+                    "iopub.execute_input": "2024-04-12T12:10:29.596321Z",
+                    "iopub.status.busy": "2024-04-12T12:10:29.596022Z",
+                    "iopub.status.idle": "2024-04-12T12:10:29.600548Z",
+                    "shell.execute_reply": "2024-04-12T12:10:29.599990Z"
                 }
             },
             "outputs": [],
             "source": [
                 "full_set = False\n",
                 "\n",
                 "if full_set:\n",
@@ -76,18 +76,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "id": "9cb3cb5c",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:46.893737Z",
-                    "iopub.status.busy": "2023-03-19T08:54:46.893457Z",
-                    "iopub.status.idle": "2023-03-19T08:54:46.936836Z",
-                    "shell.execute_reply": "2023-03-19T08:54:46.936183Z"
+                    "iopub.execute_input": "2024-04-12T12:10:29.602922Z",
+                    "iopub.status.busy": "2024-04-12T12:10:29.602713Z",
+                    "iopub.status.idle": "2024-04-12T12:10:29.643748Z",
+                    "shell.execute_reply": "2024-04-12T12:10:29.643141Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -115,44 +115,44 @@
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "id": "45c042f0",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:46.939675Z",
-                    "iopub.status.busy": "2023-03-19T08:54:46.939406Z",
-                    "iopub.status.idle": "2023-03-19T08:54:46.944552Z",
-                    "shell.execute_reply": "2023-03-19T08:54:46.943846Z"
+                    "iopub.execute_input": "2024-04-12T12:10:29.646541Z",
+                    "iopub.status.busy": "2024-04-12T12:10:29.646035Z",
+                    "iopub.status.idle": "2024-04-12T12:10:29.651144Z",
+                    "shell.execute_reply": "2024-04-12T12:10:29.650588Z"
                 },
                 "title": "A demonstration of the speedup that can be had for the descriptor transformer"
             },
             "outputs": [],
             "source": [
                 "transformer = MolecularDescriptorTransformer(parallel=False)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "8f158499",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:46.947093Z",
-                    "iopub.status.busy": "2023-03-19T08:54:46.946789Z",
-                    "iopub.status.idle": "2023-03-19T08:54:49.121374Z",
-                    "shell.execute_reply": "2023-03-19T08:54:49.120448Z"
+                    "iopub.execute_input": "2024-04-12T12:10:29.653455Z",
+                    "iopub.status.busy": "2024-04-12T12:10:29.653236Z",
+                    "iopub.status.idle": "2024-04-12T12:10:31.579596Z",
+                    "shell.execute_reply": "2024-04-12T12:10:31.578985Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Calculation time on dataset of size 200  with parallel=False:\t2.17 seconds\n"
+                        "Calculation time on dataset of size 200  with parallel=False:\t1.92 seconds\n"
                     ]
                 }
             ],
             "source": [
                 "def test_transformer(transformer):\n",
                 "    t0 = time.time()\n",
                 "    X = transformer.transform(data.ROMol)\n",
@@ -172,26 +172,34 @@
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "id": "f1b48596",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:49.124419Z",
-                    "iopub.status.busy": "2023-03-19T08:54:49.124108Z",
-                    "iopub.status.idle": "2023-03-19T08:54:50.037528Z",
-                    "shell.execute_reply": "2023-03-19T08:54:50.036724Z"
+                    "iopub.execute_input": "2024-04-12T12:10:31.582218Z",
+                    "iopub.status.busy": "2024-04-12T12:10:31.581970Z",
+                    "iopub.status.idle": "2024-04-12T12:10:32.110173Z",
+                    "shell.execute_reply": "2024-04-12T12:10:32.109459Z"
                 }
             },
             "outputs": [
                 {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "/home/esben/python_envs/vscode/lib/python3.10/site-packages/numpy/core/fromnumeric.py:59: FutureWarning: 'Series.swapaxes' is deprecated and will be removed in a future version. Please use 'Series.transpose' instead.\n",
+                        "  return bound(*args, **kwds)\n"
+                    ]
+                },
+                {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Calculation time on dataset of size 200  with parallel=True:\t0.91 seconds\n"
+                        "Calculation time on dataset of size 200  with parallel=True:\t0.52 seconds\n"
                     ]
                 }
             ],
             "source": [
                 "\n",
                 "transformer = MolecularDescriptorTransformer(parallel=True)\n",
                 "test_transformer(transformer)"
@@ -211,28 +219,34 @@
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "id": "f8b61e6c",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-03-19T08:54:50.040549Z",
-                    "iopub.status.busy": "2023-03-19T08:54:50.040317Z",
-                    "iopub.status.idle": "2023-03-19T08:54:50.144137Z",
-                    "shell.execute_reply": "2023-03-19T08:54:50.143373Z"
+                    "iopub.execute_input": "2024-04-12T12:10:32.113041Z",
+                    "iopub.status.busy": "2024-04-12T12:10:32.112800Z",
+                    "iopub.status.idle": "2024-04-12T12:10:32.220711Z",
+                    "shell.execute_reply": "2024-04-12T12:10:32.219973Z"
                 },
                 "lines_to_next_cell": 2,
                 "title": "Some of the benchmarking plots"
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Calculation time on dataset of size 200  with parallel=False:\t0.02 seconds\n",
+                        "Calculation time on dataset of size 200  with parallel=False:\t0.02 seconds\n"
+                    ]
+                },
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
                         "Calculation time on dataset of size 200  with parallel=True:\t0.08 seconds\n"
                     ]
                 }
             ],
             "source": [
                 "transformer = MorganFingerprintTransformer(parallel=False)\n",
                 "test_transformer(transformer)\n",
@@ -286,13 +300,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.9"
+            "version": "3.10.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `scikit_mol-0.2.1/notebooks/07_parallel_transforms.py` & `scikit_mol-0.3.0/notebooks/07_parallel_transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #   jupytext:
 #     cell_metadata_filter: title,-all
 #     formats: ipynb,py:percent
 #     text_representation:
 #       extension: .py
 #       format_name: percent
 #       format_version: '1.3'
-#       jupytext_version: 1.14.5
+#       jupytext_version: 1.16.1
 #   kernelspec:
 #     display_name: rdkit2
 #     language: python
 #     name: python3
 # ---
 
 # %% [markdown]
```

### Comparing `scikit_mol-0.2.1/notebooks/08_external_library_skopt.py` & `scikit_mol-0.3.0/notebooks/08_external_library_skopt.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,40 @@
-#%% Needs scikit-optimize
-#!mamba install scikit-optimize -c conda-forge
+# ---
+# jupyter:
+#   jupytext:
+#     cell_metadata_filter: title,-all
+#     formats: ipynb,py:percent
+#     text_representation:
+#       extension: .py
+#       format_name: percent
+#       format_version: '1.3'
+#       jupytext_version: 1.16.1
+#   kernelspec:
+#     display_name: vscode
+#     language: python
+#     name: python3
+# ---
 
-#%%
+# %% Needs scikit-optimize
+# !pip install scikit-optimize
+
+# %%
+import os
 import numpy as np
 import pandas as pd
 # %%
 from sklearn.linear_model import Ridge
 from sklearn.model_selection import cross_val_score
 
 from scikit_mol.fingerprints import MorganFingerprintTransformer
 from scikit_mol.conversions import SmilesToMolTransformer
 
 from sklearn.pipeline import make_pipeline
 
-#%%
+# %%
 from skopt.space import Real, Integer, Categorical
 from skopt.utils import use_named_args
 
 from skopt import gp_minimize
 # %%
 full_set = False
 
@@ -27,30 +44,31 @@
         import urllib.request
         url = "https://ndownloader.figshare.com/files/25747817"
         urllib.request.urlretrieve(url, csv_file)
 else:
     csv_file = '../tests/data/SLC6A4_active_excapedb_subset.csv'
 
 data = pd.read_csv(csv_file)
-data['ROMol'] = SmilesToMolTransformer().transform(data.SMILES)
- 
-#%%
+trf = SmilesToMolTransformer()
+data['ROMol'] = trf.transform(data.SMILES.values).flatten()
+
+# %%
 pipe = make_pipeline(MorganFingerprintTransformer(), Ridge())
 pipe
 # %%
 print(pipe.get_params())
 
-#%%
+# %%
 max_bits = 4096
 
 morgan_space = [
-    Categorical([True, False], name='morgantransformer__useCounts'),
-    Categorical([True, False], name='morgantransformer__useFeatures'),
-    Integer(512,max_bits, name='morgantransformer__nBits'),
-    Integer(1,3, name='morgantransformer__radius')
+    Categorical([True, False], name='morganfingerprinttransformer__useCounts'),
+    Categorical([True, False], name='morganfingerprinttransformer__useFeatures'),
+    Integer(512,max_bits, name='morganfingerprinttransformer__nBits'),
+    Integer(1,3, name='morganfingerprinttransformer__radius')
 ]
 
 
 regressor_space = [Real(1e-2, 1e3, "log-uniform", name='ridge__alpha')]
 
 search_space = morgan_space + regressor_space
 # %%
@@ -65,10 +83,12 @@
 # %% THIS takes forever on my machine with a GradientBoostingRegressor
 
 pipe_gp = gp_minimize(objective, search_space, n_calls=10, random_state=0)
 "Best score=%.4f" % pipe_gp.fun
 # %%
 print("""Best parameters:""")
 print({param.name:value for param,value in zip(pipe_gp.space, pipe_gp.x) })
-#%%
+# %%
 from skopt.plots import plot_convergence
-plot_convergence(pipe_gp)
+plot_convergence(pipe_gp)
+
+# %%
```

### Comparing `scikit_mol-0.2.1/notebooks/images/AtomPairFingerprintTransformer_par.png` & `scikit_mol-0.3.0/notebooks/images/AtomPairFingerprintTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/notebooks/images/AtomPairFingerprintTransformer_par.svg` & `scikit_mol-0.3.0/notebooks/images/AtomPairFingerprintTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/notebooks/images/Desc2DTransformer_par.png` & `scikit_mol-0.3.0/notebooks/images/Desc2DTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/notebooks/images/Desc2DTransformer_par.svg` & `scikit_mol-0.3.0/notebooks/images/Desc2DTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/notebooks/images/MACCSTransformer_par.png` & `scikit_mol-0.3.0/notebooks/images/MACCSTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/notebooks/images/MACCSTransformer_par.svg` & `scikit_mol-0.3.0/notebooks/images/MACCSTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/notebooks/images/MorganTransformer_par.png` & `scikit_mol-0.3.0/notebooks/images/MorganTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/notebooks/images/MorganTransformer_par.svg` & `scikit_mol-0.3.0/notebooks/images/MorganTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/notebooks/images/RDKitFPTransformer_par.png` & `scikit_mol-0.3.0/notebooks/images/RDKitFPTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/notebooks/images/RDKitFPTransformer_par.svg` & `scikit_mol-0.3.0/notebooks/images/RDKitFPTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/notebooks/images/SECFingerprintTransformer_par.png` & `scikit_mol-0.3.0/notebooks/images/SECFingerprintTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/notebooks/images/SECFingerprintTransformer_par.svg` & `scikit_mol-0.3.0/notebooks/images/SECFingerprintTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/notebooks/images/TopologicalTorsionFingerprintTransformer_par.png` & `scikit_mol-0.3.0/notebooks/images/TopologicalTorsionFingerprintTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/notebooks/images/TopologicalTorsionFingerprintTransformer_par.svg` & `scikit_mol-0.3.0/notebooks/images/TopologicalTorsionFingerprintTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/notebooks/images/Transformer_Widget.jpg` & `scikit_mol-0.3.0/notebooks/images/Transformer_Widget.jpg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/notebooks/images/max_speedup_vs_throughput.png` & `scikit_mol-0.3.0/notebooks/images/max_speedup_vs_throughput.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/notebooks/images/max_speedup_vs_throughput.svg` & `scikit_mol-0.3.0/notebooks/images/max_speedup_vs_throughput.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/ressources/logo/ScikitMol_Logo.ai` & `scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo.ai`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/ressources/logo/ScikitMol_Logo_DarkBG.png` & `scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo_DarkBG.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/ressources/logo/ScikitMol_Logo_DarkBG_300px.png` & `scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo_DarkBG_300px.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/ressources/logo/ScikitMol_Logo_DarkBG_600dpi.png` & `scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo_DarkBG_600dpi.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/ressources/logo/ScikitMol_Logo_LightBG.png` & `scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo_LightBG.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/ressources/logo/ScikitMol_Logo_LightBG_300px.png` & `scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo_LightBG_300px.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/ressources/logo/ScikitMol_Logo_LightBG_600dpi.png` & `scikit_mol-0.3.0/ressources/logo/ScikitMol_Logo_LightBG_600dpi.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/scikit_mol/conversions.py` & `scikit_mol-0.3.0/scikit_mol/conversions.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,21 +2,27 @@
 import multiprocessing
 from typing import Union
 from rdkit import Chem
 
 import numpy as np
 from sklearn.base import BaseEstimator, TransformerMixin
 
+from scikit_mol.core import check_transform_input, feature_names_default_mol ,DEFAULT_MOL_COLUMN_NAME
+
 
 class SmilesToMolTransformer(BaseEstimator, TransformerMixin):
 
     def __init__(self, parallel: Union[bool, int] = False):
         self.parallel = parallel
         self.start_method = None  #TODO implement handling of start_method
 
+    @feature_names_default_mol
+    def get_feature_names_out(self, input_features=None):
+        return input_features
+
     def fit(self, X=None, y=None):
         """Included for scikit-learn compatibility, does nothing"""
         return self
 
     def transform(self, X_smiles_list, y=None):
         """Converts SMILES into RDKit mols
 
@@ -39,32 +45,33 @@
 
         if not self.parallel:
             return self._transform(X_smiles_list)
         elif self.parallel:
             n_processes = self.parallel if self.parallel > 1 else None # Pool(processes=None) autodetects
             n_chunks = n_processes*2 if n_processes is not None else multiprocessing.cpu_count()*2 #TODO, tune the number of chunks per child process
             with get_context(self.start_method).Pool(processes=n_processes) as pool:
-                    x_chunks = np.array_split(X_smiles_list, n_chunks) 
+                    x_chunks = np.array_split(X_smiles_list, n_chunks)
                     arrays = pool.map(self._transform, x_chunks) #is the helper function a safer way of handling the picklind and child process communication
-
                     arr = np.concatenate(arrays)
                     return arr
 
-    def _transform(self, X_smiles_list):
+    @check_transform_input
+    def _transform(self, X):
         X_out = []
-        for smiles in X_smiles_list:
+        for smiles in X:
             mol = Chem.MolFromSmiles(smiles)
             if mol:
                 X_out.append(mol)
             else:
                 raise ValueError(f'Issue with parsing SMILES {smiles}\nYou probably should use the scikit-mol.sanitizer.Sanitizer on your dataset first')
 
-        return X_out
+        return np.array(X_out).reshape(-1,1)
 
+    @check_transform_input
     def inverse_transform(self, X_mols_list, y=None): #TODO, maybe the inverse transform should be configurable e.g. isomericSmiles etc.?
         X_out = []
 
         for mol in X_mols_list:
             smiles = Chem.MolToSmiles(mol)
             X_out.append(smiles)
 
-        return X_out
+        return np.array(X_out).reshape(-1,1)
```

### Comparing `scikit_mol-0.2.1/scikit_mol/descriptors.py` & `scikit_mol-0.3.0/scikit_mol/descriptors.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 from rdkit.Chem.rdchem import Mol
 from rdkit.Chem import Descriptors
 from rdkit.ML.Descriptors.MoleculeDescriptors import MolecularDescriptorCalculator
 
 from sklearn.base import BaseEstimator, TransformerMixin
 
+from scikit_mol.core import check_transform_input
+
 
 
 class MolecularDescriptorTransformer(BaseEstimator, TransformerMixin):
     """Descriptor calculation transformer
     
     Parameters
     ----------
@@ -56,14 +58,17 @@
         return MolecularDescriptorCalculator(self.desc_list)
 
     @property
     def desc_list(self):
         """Descriptor names of currently selected descriptors"""
         return self._desc_list
 
+    def get_feature_names_out(self, input_features=None):
+        return np.array(self.selected_descriptors)
+
     @desc_list.setter
     def desc_list(self, desc_list):
         self._desc_list = desc_list
         self.calculators = self._get_desc_calculator()
 
     @property
     def available_descriptors(self) -> List[str]:
@@ -90,14 +95,15 @@
     def _transform_mol(self, mol: Mol) -> List[Any]:
         return list(self.calculators.CalcDescriptors(mol))
 
     def fit(self, x, y=None):
         """Included for scikit-learn compatibility, does nothing"""
         return self
 
+    @check_transform_input
     def _transform(self, x: List[Mol]) -> np.ndarray:
         arr = np.zeros((len(x), len(self.desc_list)))
         for i, mol in enumerate(x):
             arr[i, :] = self._transform_mol(mol)
         return arr
 
     def transform(self, x: List[Mol], y=None) -> np.ndarray:
@@ -120,14 +126,15 @@
         elif self.parallel:
             n_processes = self.parallel if self.parallel > 1 else None # Pool(processes=None) autodetects
             n_chunks = n_processes if n_processes is not None else multiprocessing.cpu_count() #TODO, tune the number of chunks per child process
             
             with get_context(self.start_method).Pool(processes=n_processes) as pool:
                 params = self.get_params()
                 x_chunks = np.array_split(x, n_chunks) 
+                #x_chunks = [x.reshape(-1, 1) for x in x_chunks]
                 arrays = pool.map(parallel_helper, [(params, x) for x in x_chunks]) #is the helper function a safer way of handling the picklind and child process communication
                 arr = np.concatenate(arrays)
             return arr
 
 
 # May be safer to instantiate the transformer object in the child process, and only transfer the parameters
 # There were issues with freezing when using RDKit 2022.3
```

### Comparing `scikit_mol-0.2.1/scikit_mol/fingerprints.py` & `scikit_mol-0.3.0/scikit_mol/fingerprints.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #%%
 from multiprocessing import Pool, get_context
 import multiprocessing
+import re
 from typing import Union
 from rdkit import Chem
 from rdkit import DataStructs
 #from rdkit.Chem.AllChem import GetMorganFingerprintAsBitVect
 from rdkit.Chem import rdMolDescriptors
 from rdkit.Chem import rdFingerprintGenerator
 from rdkit.Chem import rdMHFPFingerprint
@@ -12,54 +13,96 @@
 
 import numpy as np
 import pandas as pd
 from scipy.sparse import lil_matrix
 from scipy.sparse import vstack
 
 from sklearn.base import BaseEstimator, TransformerMixin
+from scikit_mol.core import check_transform_input
 
 from abc import ABC, abstractmethod
 
+_PATTERN_FINGERPRINT_TRANSFORMER = re.compile(r"^(?P<fingerprint_name>\w+)FingerprintTransformer$")
+
 #%%
 class FpsTransformer(ABC, BaseEstimator, TransformerMixin):
 
     def __init__(self, parallel: Union[bool, int] = False, start_method: str = None):
         self.parallel = parallel
         self.start_method = start_method #TODO implement handling of start_method
 
+    # The dtype of the fingerprint array computed by the transformer
+    # If needed this property can be overwritten in the child class.
+    _DTYPE_FINGERPRINT = np.int8
+
+    def _get_column_prefix(self) -> str:
+        matched = _PATTERN_FINGERPRINT_TRANSFORMER.match(type(self).__name__)
+        if matched:
+            fingerprint_name = matched.group("fingerprint_name")
+            return f"fp_{fingerprint_name.lower()}"
+        else:
+            return "fp"
+
+    def _get_n_digits_column_suffix(self) -> int:
+        return len(str(self.nBits))
+
+    def get_display_feature_names_out(self, input_features=None):
+        """Get feature names for display purposes
+
+        All feature names will have the same length,
+        since the different elements will be prefixed with zeros
+        depending on the number of bits.
+        """
+        prefix = self._get_column_prefix()
+        n_digits = self._get_n_digits_column_suffix()
+        return np.array([f"{prefix}_{str(i).zfill(n_digits)}" for i in range(1, self.nBits + 1)])
+
+    def get_feature_names_out(self, input_features=None):
+        """Get feature names for fingerprint transformers
+
+        This method is used by the scikit-learn set_output API
+        to get the column names of the transformed dataframe.
+        """
+        prefix = self._get_column_prefix()
+        return np.array([f"{prefix}_{i}" for i in range(1, self.nBits + 1)])
+
     @abstractmethod
     def _mol2fp(self, mol):
         """Generate descriptor from mol
 
         MUST BE OVERWRITTEN
         """
         raise NotImplementedError("_mol2fp not implemented")
 
     def _fp2array(self, fp):
-        arr = np.zeros((self.nBits,), dtype=np.int8)
+        arr = np.zeros((self.nBits,), dtype=self._DTYPE_FINGERPRINT)
         DataStructs.ConvertToNumpyArray(fp, arr)
         return arr
 
     def _transform_mol(self, mol):
         fp = self._mol2fp(mol)
         arr = self._fp2array(fp)
         return arr
 
     def fit(self, X, y=None):
-        """Included for scikit-learn compatibility, does nothing"""
+        """Included for scikit-learn compatibility
+
+        Also sets the column prefix for use by the transform method with dataframe output.
+        """
         return self
 
+    @check_transform_input
     def _transform(self, X):
-        arr = np.zeros((len(X), self.nBits), dtype=np.int8)
+        arr = np.zeros((len(X), self.nBits), dtype=self._DTYPE_FINGERPRINT)
         for i, mol in enumerate(X):
             arr[i,:] = self._transform_mol(mol)
         return arr
 
     def _transform_sparse(self, X):
-        arr = np.zeros((len(X), self.nBits), dtype=np.int8)
+        arr = np.zeros((len(X), self.nBits), dtype=self._DTYPE_FINGERPRINT)
         for i, mol in enumerate(X):
             arr[i,:] = self._transform_mol(mol)
         
         return lil_matrix(arr)
 
     def transform(self, X, y=None):
         """Transform a list of RDKit molecule objects into a fingerprint array
@@ -84,14 +127,17 @@
             n_chunks = n_processes if n_processes is not None else multiprocessing.cpu_count() 
             
             with get_context(self.start_method).Pool(processes=n_processes) as pool:
                 x_chunks = np.array_split(X, n_chunks)
                 #TODO check what is fastest, pickle or recreate and do this only for classes that need this
                 #arrays = pool.map(self._transform, x_chunks)
                 parameters = self.get_params()
+                # TODO: create "transform_parallel" function in the core module,
+                # and use it here and in the descriptors transformer
+                #x_chunks = [np.array(x).reshape(-1, 1) for x in x_chunks]
                 arrays = pool.map(parallel_helper, [(self.__class__.__name__, parameters, x_chunk) for x_chunk in x_chunks]) 
 
                 arr = np.concatenate(arrays)
             return arr
 
 
 class MACCSKeysFingerprintTransformer(FpsTransformer):
@@ -292,19 +338,15 @@
 
     def __setstate__(self, state):
         # Restore the state of the parent class
         super().__setstate__(state)
         # Re-create the unpicklable property
         self._recreate_encoder()
 
-    def _transform(self, X):
-        arr = np.zeros((len(X), self.nBits), dtype=np.int32)
-        for i, mol in enumerate(X):
-            arr[i,:] = self._transform_mol(mol)
-        return arr
+    _DTYPE_FINGERPRINT = np.int32
 
     def _mol2fp(self, mol):
         fp = self.mhfp_encoder.EncodeMol(mol, self.radius, self.rings, self.isomeric, self.kekulize, self.min_radius)
         return fp
     
     def _fp2array(self, fp):
         return np.array(fp)
```

### Comparing `scikit_mol-0.2.1/scikit_mol/standardizer.py` & `scikit_mol-0.3.0/scikit_mol/standardizer.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import multiprocessing
 from rdkit import Chem
 from sklearn.base import BaseEstimator, TransformerMixin
 from rdkit.Chem.MolStandardize import rdMolStandardize
 from rdkit.rdBase import BlockLogs
 import numpy as np
 
+from scikit_mol.core import check_transform_input, feature_names_default_mol
+
 
 class Standardizer(BaseEstimator, TransformerMixin):
     """ Input a list of rdkit mols, output the same list but standardised 
     """
     def __init__(self, neutralize=True, parallel=False):
         self.neutralize = neutralize
         self.parallel = parallel
@@ -35,16 +37,21 @@
                 uncharged_parent_clean_mol = uncharger.uncharge(parent_clean_mol)
             else:
                 uncharged_parent_clean_mol = parent_clean_mol
             # Add to final list
             arr.append(uncharged_parent_clean_mol)
         
         del block # Release logging block to previous state
-        return(arr)
-    
+        return np.array(arr).reshape(-1,1)
+
+    @feature_names_default_mol
+    def get_feature_names_out(self, input_features=None):
+        return input_features
+
+    @check_transform_input
     def transform(self, X, y=None):
         if not self.parallel:
             return self._transform(X)
 
         elif self.parallel:
             n_processes = self.parallel if self.parallel > 1 else None # Pool(processes=None) autodetects
             n_chunks = n_processes*2 if n_processes is not None else multiprocessing.cpu_count()*2 #TODO, tune the number of chunks per child process
```

### Comparing `scikit_mol-0.2.1/scikit_mol/utilities.py` & `scikit_mol-0.3.0/scikit_mol/utilities.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/scikit_mol.egg-info/SOURCES.txt` & `scikit_mol-0.3.0/scikit_mol.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+CITATION.bib
+CONTRIBUTION.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 notebooks/01_basic_usage.ipynb
 notebooks/01_basic_usage.py
@@ -13,15 +15,20 @@
 notebooks/04_standardizer.py
 notebooks/05_smiles_sanitaztion.ipynb
 notebooks/05_smiles_sanitaztion.py
 notebooks/06_hyperparameter_tuning.ipynb
 notebooks/06_hyperparameter_tuning.py
 notebooks/07_parallel_transforms.ipynb
 notebooks/07_parallel_transforms.py
+notebooks/08_external_library_skopt.ipynb
 notebooks/08_external_library_skopt.py
+notebooks/09_Combinatorial_Method_Usage_with_FingerPrint_Transformers.ipynb
+notebooks/09_Combinatorial_Method_Usage_with_FingerPrint_Transformers.py
+notebooks/10_pipeline_pandas_output.ipynb
+notebooks/10_pipeline_pandas_output.py
 notebooks/README.md
 notebooks/pair_notebook.sh
 notebooks/run_notebooks.sh
 notebooks/sync_notebooks.sh
 notebooks/02_descriptor_transformer_files/02_descriptor_transformer_5_0.png
 notebooks/04_standardizer_files/04_standardizer_3_0.png
 notebooks/04_standardizer_files/04_standardizer_3_1.png
@@ -48,14 +55,15 @@
 ressources/logo/ScikitMol_Logo_DarkBG_600dpi.png
 ressources/logo/ScikitMol_Logo_LightBG.png
 ressources/logo/ScikitMol_Logo_LightBG_300px.png
 ressources/logo/ScikitMol_Logo_LightBG_600dpi.png
 scikit_mol/__init__.py
 scikit_mol/_version.py
 scikit_mol/conversions.py
+scikit_mol/core.py
 scikit_mol/descriptors.py
 scikit_mol/fingerprints.py
 scikit_mol/standardizer.py
 scikit_mol/utilities.py
 scikit_mol.egg-info/PKG-INFO
 scikit_mol.egg-info/SOURCES.txt
 scikit_mol.egg-info/dependency_links.txt
@@ -66,8 +74,9 @@
 tests/test_desctransformer.py
 tests/test_fptransformers.py
 tests/test_parameter_types.py
 tests/test_sanitizer.py
 tests/test_scikit_mol.py
 tests/test_smilestomol.py
 tests/test_transformers.py
+tests/data/CDDD_SLC6A4_active_excapedb_subset.csv.gz
 tests/data/SLC6A4_active_excapedb_subset.csv
```

### Comparing `scikit_mol-0.2.1/setup.cfg` & `scikit_mol-0.3.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -30,21 +30,23 @@
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	rdkit
 	numpy
 	pandas
 	scikit-learn
+	packaging
 
 [options.packages.find]
 exclude = 
 	tests/*
 
 [options.extras_require]
 dev = 
 	pytest>=6
 	pytest-cov
+	jupytext
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `scikit_mol-0.2.1/tests/conftest.py` & `scikit_mol-0.3.0/tests/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from pathlib import Path
 from pathlib import PurePath
 from urllib.parse import urlsplit
 from urllib.request import urlopen
 
 import pandas as pd
 import pytest
+import sklearn
 
 
 TEST_DATA_URL = "https://ndownloader.figshare.com/files/25747817"
 TEST_DATA_MD5 = "1ec89bde544c3c4bc400d5b75315921e"
 
 
 def md5(fn):
@@ -41,7 +42,14 @@
             pytest.fail("incorrect md5")
 
     yield data_fn.absolute()
 
 @pytest.fixture()
 def data(data_pth) -> pd.DataFrame:
     yield pd.read_csv(data_pth)
+
+@pytest.fixture(scope="module")
+def pandas_output():
+    """Set sklearn to output pandas dataframes"""
+    sklearn.set_config(transform_output="pandas")
+    yield
+    sklearn.set_config(transform_output="default")
```

### Comparing `scikit_mol-0.2.1/tests/data/SLC6A4_active_excapedb_subset.csv` & `scikit_mol-0.3.0/tests/data/SLC6A4_active_excapedb_subset.csv`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/tests/test_fptransformers.py` & `scikit_mol-0.3.0/tests/test_fptransformers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pickle
 import tempfile
 import pytest
 import numpy as np
 import pandas as pd
 from rdkit import Chem
-from fixtures import mols_list, smiles_list, fingerprint, chiral_smiles_list, chiral_mols_list
+from fixtures import mols_list, smiles_list, mols_container, smiles_container, fingerprint, chiral_smiles_list, chiral_mols_list
 from sklearn import clone
 
 from scikit_mol.fingerprints import MorganFingerprintTransformer, MACCSKeysFingerprintTransformer, RDKitFingerprintTransformer, AtomPairFingerprintTransformer, TopologicalTorsionFingerprintTransformer, SECFingerprintTransformer, MHFingerprintTransformer, AvalonFingerprintTransformer
 
 
 
 @pytest.fixture
@@ -95,54 +95,50 @@
     for t in [mhfp_transformer]:
         params   = t.get_params()
         params['n_permutations'] = 4242
         t.set_params(n_permutations = 4242)
         params_2 = t.get_params()
         assert all([ params[key] == params_2[key] for key in params.keys()])
 
-def test_transform(mols_list, morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, secfp_transformer, mhfp_transformer, avalon_transformer):
-    #Test different types of input
-    for mols in [mols_list, np.array(mols_list), pd.Series(mols_list)]:
-        #Test the different transformers
-        for t in [morgan_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, rdkit_transformer, secfp_transformer, mhfp_transformer, avalon_transformer]:
-            params   = t.get_params()
-            fps = t.transform(mols)
-            #Assert that the same length of input and output
-            assert len(fps) == len(mols_list)
-
-            # assert that the size of the fingerprint is the expected size
-            if type(t) == type(maccs_transformer) or type(t) == type(secfp_transformer) or type(t) == type(mhfp_transformer):
-                fpsize = t.nBits
-            elif type(t) == type(rdkit_transformer):
-                fpsize = params['fpSize']
-            else:
-                fpsize = params['nBits']
-            
-            assert len(fps[0]) == fpsize
-
-def test_transform_parallel(mols_list, morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, secfp_transformer, mhfp_transformer, avalon_transformer):
-    #Test different types of input
-    for mols in [mols_list, np.array(mols_list), pd.Series(mols_list)]:
-        #Test the different transformers
-        for t in [morgan_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, rdkit_transformer, secfp_transformer, mhfp_transformer, avalon_transformer]:
-            t.set_params(parallel=True)
-            params   = t.get_params()
-            fps = t.transform(mols)
-            #Assert that the same length of input and output
-            assert len(fps) == len(mols_list)
-
-            # assert that the size of the fingerprint is the expected size
-            if type(t) == type(maccs_transformer) or type(t) == type(secfp_transformer) or type(t) == type(mhfp_transformer):
-                fpsize = t.nBits
-            elif type(t) == type(rdkit_transformer):
-                fpsize = params['fpSize']
-            else:
-                fpsize = params['nBits']
-            
-            assert len(fps[0]) == fpsize
+def test_transform(mols_container, morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, secfp_transformer, mhfp_transformer, avalon_transformer):
+    #Test the different transformers
+    for t in [morgan_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, rdkit_transformer, secfp_transformer, mhfp_transformer, avalon_transformer]:
+        params   = t.get_params()
+        fps = t.transform(mols_container)
+        #Assert that the same length of input and output
+        assert len(fps) == len(mols_container)
+
+        # assert that the size of the fingerprint is the expected size
+        if type(t) == type(maccs_transformer) or type(t) == type(secfp_transformer) or type(t) == type(mhfp_transformer):
+            fpsize = t.nBits
+        elif type(t) == type(rdkit_transformer):
+            fpsize = params['fpSize']
+        else:
+            fpsize = params['nBits']
+        
+        assert len(fps[0]) == fpsize
+
+def test_transform_parallel(mols_container, morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, secfp_transformer, mhfp_transformer, avalon_transformer):
+    #Test the different transformers
+    for t in [morgan_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, rdkit_transformer, secfp_transformer, mhfp_transformer, avalon_transformer]:
+        t.set_params(parallel=True)
+        params   = t.get_params()
+        fps = t.transform(mols_container)
+        #Assert that the same length of input and output
+        assert len(fps) == len(mols_container)
+
+        # assert that the size of the fingerprint is the expected size
+        if type(t) == type(maccs_transformer) or type(t) == type(secfp_transformer) or type(t) == type(mhfp_transformer):
+            fpsize = t.nBits
+        elif type(t) == type(rdkit_transformer):
+            fpsize = params['fpSize']
+        else:
+            fpsize = params['nBits']
+        
+        assert len(fps[0]) == fpsize
 
 
 def test_picklable(morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, secfp_transformer, avalon_transformer):
     #Test the different transformers
     for t in [morgan_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, rdkit_transformer, secfp_transformer, avalon_transformer]:
         with tempfile.NamedTemporaryFile() as f:
             pickle.dump(t, f)
```

### Comparing `scikit_mol-0.2.1/tests/test_parameter_types.py` & `scikit_mol-0.3.0/tests/test_parameter_types.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.1/tests/test_sanitizer.py` & `scikit_mol-0.3.0/tests/test_sanitizer.py`

 * *Files identical despite different names*

