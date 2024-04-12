# Comparing `tmp/quacc-0.7.3.tar.gz` & `tmp/quacc-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quacc-0.7.3.tar", last modified: Tue Apr  9 21:38:43 2024, max compression
+gzip compressed data, was "quacc-0.7.4.tar", last modified: Fri Apr 12 18:24:01 2024, max compression
```

## Comparing `quacc-0.7.3.tar` & `quacc-0.7.4.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.347089 quacc-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-09 21:36:28.000000 quacc-0.7.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-09 21:36:28.000000 quacc-0.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6760 2024-04-09 21:38:43.347089 quacc-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-09 21:36:28.000000 quacc-0.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-09 21:36:28.000000 quacc-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 21:38:43.347089 quacc-0.7.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.311089 quacc-0.7.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.315089 quacc-0.7.3/src/quacc/
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.315089 quacc-0.7.3/src/quacc/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/_cli/quacc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.319089 quacc-0.7.3/src/quacc/atoms/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/atoms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/atoms/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/atoms/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/atoms/deformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/atoms/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)    13785 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/atoms/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.319089 quacc-0.7.3/src/quacc/calculators/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.319089 quacc-0.7.3/src/quacc/calculators/espresso/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17278 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/espresso.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.319089 quacc-0.7.3/src/quacc/calculators/espresso/presets/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/presets/esm_metal_slab_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/presets/esm_metal_slab_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/presets/metal_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/presets/metal_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/presets/molecule_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/presets/semiconductors_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/presets/semiconductors_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.323089 quacc-0.7.3/src/quacc/calculators/qchem/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/qchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/qchem/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/qchem/params.py
--rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/qchem/qchem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/qchem/qchem_custodian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.323089 quacc-0.7.3/src/quacc/calculators/vasp/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.323089 quacc-0.7.3/src/quacc/calculators/vasp/presets/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/presets/BulkSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/presets/QMOFSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/presets/SlabSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/presets/magmoms_MP.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/presets/magmoms_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/presets/setups_pbe54.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/presets/setups_qmof.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/vasp_custodian.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.323089 quacc-0.7.3/src/quacc/recipes/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.327089 quacc-0.7.3/src/quacc/recipes/common/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/common/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/common/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/common/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/common/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.327089 quacc-0.7.3/src/quacc/recipes/dftb/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/dftb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/dftb/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/dftb/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.327089 quacc-0.7.3/src/quacc/recipes/emt/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/emt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/emt/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/emt/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/emt/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/emt/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/emt/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.327089 quacc-0.7.3/src/quacc/recipes/espresso/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/espresso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/espresso/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12481 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/espresso/bands.py
--rw-r--r--   0 runner    (1001) docker     (127)    13569 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/espresso/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9598 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/espresso/dos.py
--rw-r--r--   0 runner    (1001) docker     (127)    23059 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/espresso/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.327089 quacc-0.7.3/src/quacc/recipes/gaussian/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/gaussian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/gaussian/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/gaussian/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.331089 quacc-0.7.3/src/quacc/recipes/gulp/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/gulp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/gulp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/gulp/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.331089 quacc-0.7.3/src/quacc/recipes/lj/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/lj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/lj/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.331089 quacc-0.7.3/src/quacc/recipes/mlp/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/mlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/mlp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/mlp/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/mlp/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.331089 quacc-0.7.3/src/quacc/recipes/newtonnet/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/newtonnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/newtonnet/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/newtonnet/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.331089 quacc-0.7.3/src/quacc/recipes/onetep/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/onetep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/onetep/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/onetep/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.331089 quacc-0.7.3/src/quacc/recipes/orca/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/orca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/orca/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/orca/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.331089 quacc-0.7.3/src/quacc/recipes/psi4/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/psi4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/psi4/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/psi4/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.335089 quacc-0.7.3/src/quacc/recipes/qchem/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/qchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/qchem/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/qchem/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/qchem/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.335089 quacc-0.7.3/src/quacc/recipes/tblite/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/tblite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/tblite/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/tblite/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.335089 quacc-0.7.3/src/quacc/recipes/vasp/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/vasp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/vasp/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    14585 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/vasp/mp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/vasp/qmof.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/vasp/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.335089 quacc-0.7.3/src/quacc/runners/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/runners/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/runners/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/runners/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/runners/thermo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.339089 quacc-0.7.3/src/quacc/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.339089 quacc-0.7.3/src/quacc/schemas/_aliases/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/_aliases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/_aliases/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/_aliases/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/_aliases/cclib.py
--rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/_aliases/emmet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/_aliases/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/_aliases/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)    15490 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)    18083 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/cclib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)    12848 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)    16763 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.339089 quacc-0.7.3/src/quacc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/utils/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/utils/kpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/utils/lists.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.339089 quacc-0.7.3/src/quacc/wflow_tools/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/wflow_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/wflow_tools/customizers.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/wflow_tools/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/wflow_tools/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.339089 quacc-0.7.3/src/quacc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6760 2024-04-09 21:38:43.000000 quacc-0.7.3/src/quacc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-09 21:38:43.000000 quacc-0.7.3/src/quacc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 21:38:43.000000 quacc-0.7.3/src/quacc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-09 21:38:43.000000 quacc-0.7.3/src/quacc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-09 21:38:43.000000 quacc-0.7.3/src/quacc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 21:38:43.000000 quacc-0.7.3/src/quacc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.500677 quacc-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-12 18:21:59.000000 quacc-0.7.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 18:21:59.000000 quacc-0.7.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-04-12 18:24:01.500677 quacc-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-12 18:21:59.000000 quacc-0.7.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-04-12 18:22:00.000000 quacc-0.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 18:24:01.500677 quacc-0.7.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.464677 quacc-0.7.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.468677 quacc-0.7.4/src/quacc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.472677 quacc-0.7.4/src/quacc/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/_cli/quacc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.472677 quacc-0.7.4/src/quacc/atoms/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/atoms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/atoms/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/atoms/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/atoms/deformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/atoms/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13785 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/atoms/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.472677 quacc-0.7.4/src/quacc/calculators/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.472677 quacc-0.7.4/src/quacc/calculators/espresso/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17250 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/espresso.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.476677 quacc-0.7.4/src/quacc/calculators/espresso/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/presets/esm_metal_slab_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/presets/esm_metal_slab_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/presets/metal_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/presets/metal_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/presets/molecule_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/presets/semiconductors_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/presets/semiconductors_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/espresso/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.476677 quacc-0.7.4/src/quacc/calculators/qchem/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/qchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/qchem/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/qchem/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/qchem/qchem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/qchem/qchem_custodian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.476677 quacc-0.7.4/src/quacc/calculators/vasp/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.480677 quacc-0.7.4/src/quacc/calculators/vasp/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/presets/BulkSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/presets/QMOFSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/presets/SlabSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/presets/magmoms_MP.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/presets/magmoms_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/presets/setups_pbe54.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/presets/setups_qmof.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/calculators/vasp/vasp_custodian.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.480677 quacc-0.7.4/src/quacc/recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.480677 quacc-0.7.4/src/quacc/recipes/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/common/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/common/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/common/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/common/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.480677 quacc-0.7.4/src/quacc/recipes/dftb/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/dftb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/dftb/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/dftb/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.480677 quacc-0.7.4/src/quacc/recipes/emt/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/emt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/emt/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/emt/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/emt/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/emt/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/emt/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.484677 quacc-0.7.4/src/quacc/recipes/espresso/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/espresso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/espresso/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12481 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/espresso/bands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13569 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/espresso/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9598 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/espresso/dos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23059 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/espresso/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.484677 quacc-0.7.4/src/quacc/recipes/gaussian/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/gaussian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/gaussian/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/gaussian/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.484677 quacc-0.7.4/src/quacc/recipes/gulp/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/gulp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/gulp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/gulp/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.484677 quacc-0.7.4/src/quacc/recipes/lj/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/lj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/lj/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.484677 quacc-0.7.4/src/quacc/recipes/mlp/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/mlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/mlp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/mlp/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/mlp/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.484677 quacc-0.7.4/src/quacc/recipes/newtonnet/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/newtonnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/newtonnet/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/newtonnet/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.488677 quacc-0.7.4/src/quacc/recipes/onetep/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/onetep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/onetep/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/onetep/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.488677 quacc-0.7.4/src/quacc/recipes/orca/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/orca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/orca/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/orca/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.488677 quacc-0.7.4/src/quacc/recipes/psi4/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/psi4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/psi4/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/psi4/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.488677 quacc-0.7.4/src/quacc/recipes/qchem/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/qchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/qchem/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/qchem/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/qchem/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.488677 quacc-0.7.4/src/quacc/recipes/tblite/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/tblite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/tblite/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/tblite/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.488677 quacc-0.7.4/src/quacc/recipes/vasp/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/vasp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/vasp/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14585 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/vasp/mp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/vasp/qmof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/recipes/vasp/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.492677 quacc-0.7.4/src/quacc/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/runners/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/runners/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/runners/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/runners/thermo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.492677 quacc-0.7.4/src/quacc/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.492677 quacc-0.7.4/src/quacc/schemas/_aliases/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/_aliases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/_aliases/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/_aliases/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/_aliases/cclib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/_aliases/emmet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/_aliases/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/_aliases/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15500 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18073 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/cclib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/schemas/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16763 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.496677 quacc-0.7.4/src/quacc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/utils/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/utils/kpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/utils/lists.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.496677 quacc-0.7.4/src/quacc/wflow_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/wflow_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/wflow_tools/customizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/wflow_tools/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-04-12 18:22:00.000000 quacc-0.7.4/src/quacc/wflow_tools/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:24:01.496677 quacc-0.7.4/src/quacc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-04-12 18:24:01.000000 quacc-0.7.4/src/quacc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-12 18:24:01.000000 quacc-0.7.4/src/quacc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:24:01.000000 quacc-0.7.4/src/quacc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 18:24:01.000000 quacc-0.7.4/src/quacc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-12 18:24:01.000000 quacc-0.7.4/src/quacc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 18:24:01.000000 quacc-0.7.4/src/quacc.egg-info/top_level.txt
```

### Comparing `quacc-0.7.3/LICENSE.md` & `quacc-0.7.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/PKG-INFO` & `quacc-0.7.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quacc
-Version: 0.7.3
+Version: 0.7.4
 Summary: A platform to enable high-throughput, database-driven quantum chemistry and computational materials science
 Author-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 Maintainer-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 License: BSD-3
 Project-URL: repository, https://github.com/Quantum-Accelerators/quacc
 Project-URL: documentation, https://quantum-accelerators.github.io/quacc/
 Project-URL: changelog, https://github.com/Quantum-Accelerators/quacc/blob/main/CHANGELOG.md
@@ -24,21 +24,21 @@
 Requires-Python: <3.13,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: ase>3.22.1
 Requires-Dist: cclib>=1.8
 Requires-Dist: custodian>=2024.3.12
 Requires-Dist: emmet-core>=0.80.0
-Requires-Dist: maggma<=0.63.4
+Requires-Dist: maggma>=0.64.0
 Requires-Dist: monty>=2024.2.26
 Requires-Dist: numpy>=1.25.0
 Requires-Dist: psutil
 Requires-Dist: pydantic>=2.0.1
 Requires-Dist: pydantic-settings>=2.2.0
-Requires-Dist: pymatgen>=2024.2.20
+Requires-Dist: pymatgen>=2024.4.12
 Requires-Dist: typer>=0.12.1
 Provides-Extra: covalent
 Requires-Dist: covalent>=0.234.0rc0; extra == "covalent"
 Requires-Dist: covalent-cloud>=0.39.0; extra == "covalent"
 Provides-Extra: dask
 Requires-Dist: dask[distributed]>=2023.12.1; extra == "dask"
 Requires-Dist: dask-jobqueue>=0.8.2; extra == "dask"
@@ -71,15 +71,14 @@
 Provides-Extra: redun
 Requires-Dist: redun>=0.16.2; extra == "redun"
 Provides-Extra: sella
 Requires-Dist: sella>=2.3.3; extra == "sella"
 Provides-Extra: tblite
 Requires-Dist: tblite[ase]>=0.3.0; platform_system == "Linux" and extra == "tblite"
 Provides-Extra: dev
-Requires-Dist: codecov-cli>=0.4.1; extra == "dev"
 Requires-Dist: pytest>=7.4.0; extra == "dev"
 Requires-Dist: pytest-cov>=3.0.0; extra == "dev"
 Requires-Dist: ruff>=0.0.285; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: blacken-docs>=1.16.0; extra == "docs"
 Requires-Dist: mkdocs-material>=9.5.16; extra == "docs"
 Requires-Dist: mkdocstrings[python]>=0.22.0; extra == "docs"
```

### Comparing `quacc-0.7.3/README.md` & `quacc-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/pyproject.toml` & `quacc-0.7.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quacc"
 description="A platform to enable high-throughput, database-driven quantum chemistry and computational materials science"
-version = "0.7.3"
+version = "0.7.4"
 readme = "README.md"
 license = { text = "BSD-3" }
 authors = [{ name = "Andrew S. Rosen", email = "asrosen@princeton.edu" }]
 maintainers = [{ name = "Andrew S. Rosen", email = "asrosen@princeton.edu" }]
 keywords = ["high-throughput", "automated", "workflow", "dft"]
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -27,21 +27,21 @@
 ]
 requires-python = ">=3.9, <3.13"
 dependencies = [
     "ase>3.22.1", # for Atoms object and calculators
     "cclib>=1.8", # for I/O parsing of molecular DFT codes
     "custodian>=2024.3.12", # for automated error corrections
     "emmet-core>=0.80.0", # for pre-made schemas
-    "maggma<=0.63.4", # for database handling
+    "maggma>=0.64.0", # for database handling
     "monty>=2024.2.26", # miscellaneous Python utilities
     "numpy>=1.25.0", # for array handling
     "psutil", # for getting compute architecture details
     "pydantic>=2.0.1", # for settings management
     "pydantic-settings>=2.2.0", # for settings management
-    "pymatgen>=2024.2.20", # for structure manipulation
+    "pymatgen>=2024.4.12", # for structure manipulation
     "typer>=0.12.1", # for the CLI
 ]
 
 [project.optional-dependencies]
 covalent = ["covalent>=0.234.0rc0", "covalent-cloud>=0.39.0"]
 dask = ["dask[distributed]>=2023.12.1", "dask-jobqueue>=0.8.2"]
 defects = ["pymatgen-analysis-defects>=2023.8.22", "shakenbreak>=3.2.0"]
@@ -51,15 +51,15 @@
 newtonnet = ["newtonnet>=1.1"]
 parsl = ["parsl[monitoring]>=2023.10.23"]
 phonons = ["phonopy>=2.20.0", "seekpath>=2.1.0"]
 prefect = ["prefect>=2.14.14", "prefect-dask>=0.2.6", "dask-jobqueue>=0.8.2"]
 redun = ["redun>=0.16.2"]
 sella = ["sella>=2.3.3"]
 tblite = ["tblite[ase]>=0.3.0; platform_system=='Linux'"]
-dev = ["codecov-cli>=0.4.1", "pytest>=7.4.0", "pytest-cov>=3.0.0", "ruff>=0.0.285"]
+dev = ["pytest>=7.4.0", "pytest-cov>=3.0.0", "ruff>=0.0.285"]
 docs = [
     "blacken-docs>=1.16.0",
     "mkdocs-material>=9.5.16",
     "mkdocstrings[python]>=0.22.0",
     "mkdocs-gen-files>=0.5.0",
     "mkdocs-literate-nav>=0.6.0",
     "pillow>=10.0.0",
@@ -138,15 +138,14 @@
   "Q",      # flake8-quotes
   "RET",    # flake8-return
   "RSE",    # flake8-raise
   "RUF",    # Ruff-specific rules
   "SIM",    # flake8-simplify
   "SLOT",   # flake8-slots
   "TCH",    # flake8-type-checking
-  "TID",    # tidy imports
   "TID",    # flake8-tidy-imports
   "UP",     # pyupgrade
   "W",      # pycodestyle warning
   "YTT",    # flake8-2020
 ]
 lint.ignore = [
   "PLR",    # Design related pylint codes
```

### Comparing `quacc-0.7.3/src/quacc/__init__.py` & `quacc-0.7.4/src/quacc/__init__.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/_cli/quacc.py` & `quacc-0.7.4/src/quacc/_cli/quacc.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/atoms/core.py` & `quacc-0.7.4/src/quacc/atoms/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -233,22 +233,24 @@
     logger.debug(
         f"Setting charge to {mol.charge} and spin multiplicity to {mol.spin_multiplicity}"
     )
 
     return mol.charge, mol.spin_multiplicity
 
 
-def get_final_atoms_from_dyn(dyn: Dynamics) -> Atoms:
+def get_final_atoms_from_dynamics(dynamics: Dynamics) -> Atoms:
     """
     Get the final atoms object from a dynamics run.
 
     Parameters
     ----------
-    dyn
+    dynamics
         ASE dynamics object
 
     Returns
     -------
     Atoms
         Atoms object
     """
-    return dyn.atoms.atoms if isinstance(dyn.atoms, Filter) else dyn.atoms
+    return (
+        dynamics.atoms.atoms if isinstance(dynamics.atoms, Filter) else dynamics.atoms
+    )
```

### Comparing `quacc-0.7.3/src/quacc/atoms/defects.py` & `quacc-0.7.4/src/quacc/atoms/defects.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/atoms/deformation.py` & `quacc-0.7.4/src/quacc/atoms/deformation.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/atoms/phonons.py` & `quacc-0.7.4/src/quacc/atoms/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/atoms/slabs.py` & `quacc-0.7.4/src/quacc/atoms/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/calculators/espresso/espresso.py` & `quacc-0.7.4/src/quacc/calculators/espresso/espresso.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,15 +294,15 @@
         if self.binary == "pw":
             system = input_data.get("system", {})
 
             occupations = system.get("occupations", "fixed")
             smearing = system.get("smearing", None)
             degauss = system.get("degauss", None)
 
-            if occupations == "fixed" and not (smearing is None and degauss is None):
+            if occupations == "fixed" and (smearing is not None or degauss is not None):
                 LOGGER.warning(
                     "The occupations are set to 'fixed' but smearing or degauss is also set. This will be ignored."
                 )
                 system["smearing"] = Remove
                 system["degauss"] = Remove
 
             parameters["input_data"]["system"] = system
@@ -393,15 +393,15 @@
         -------
         None
         """
         self.input_atoms = input_atoms or Atoms()
         self.preset = preset
         self.parallel_info = parallel_info
         self.kwargs = kwargs
-        self._user_calc_params = {}
+        self.user_calc_params = {}
 
         template = template or EspressoTemplate("pw")
 
         self._binary = template.binary
 
         full_path = Path(
             SETTINGS.ESPRESSO_BIN_DIR, SETTINGS.ESPRESSO_BINARIES[self._binary]
@@ -412,31 +412,31 @@
             self._cleanup_params()
         else:
             LOGGER.warning(
                 f"the binary you requested, `{self._binary}`, is not supported by ASE. This means that presets and usual checks will not be carried out, your `input_data` must be provided in nested format."
             )
 
             self.kwargs["input_data"] = Namelist(self.kwargs.get("input_data"))
-            self._user_calc_params = self.kwargs
+            self.user_calc_params = self.kwargs
 
         self._pseudo_path = (
-            self._user_calc_params.get("input_data", {})
+            self.user_calc_params.get("input_data", {})
             .get("control", {})
             .get("pseudo_dir", str(SETTINGS.ESPRESSO_PSEUDO))
         )
         self.profile = profile or EspressoProfile(
             binary=self._bin_path,
             parallel_info=parallel_info,
             pseudo_dir=self._pseudo_path,
         )
 
         super().__init__(
             profile=self.profile,
             parallel_info=self.parallel_info,
-            **self._user_calc_params,
+            **self.user_calc_params,
         )
 
         self.template = template
 
     def _cleanup_params(self) -> None:
         """
         Function that handles the kwargs. It will merge the user-supplied kwargs with
@@ -464,26 +464,24 @@
             calc_preset["input_data"].to_nested(binary=self._binary, **calc_preset)
             if "pseudopotentials" in calc_preset:
                 ecutwfc, ecutrho, pseudopotentials = get_pseudopotential_info(
                     calc_preset["pseudopotentials"], self.input_atoms
                 )
                 calc_preset.pop("pseudopotentials", None)
                 calc_preset = remove_conflicting_kpts_kspacing(calc_preset, self.kwargs)
-                self._user_calc_params = recursive_dict_merge(
+                self.user_calc_params = recursive_dict_merge(
                     calc_preset,
                     {
                         "input_data": {
                             "system": {"ecutwfc": ecutwfc, "ecutrho": ecutrho}
                         },
                         "pseudopotentials": pseudopotentials,
                     },
                     self.kwargs,
                 )
             else:
-                self._user_calc_params = recursive_dict_merge(calc_preset, self.kwargs)
+                self.user_calc_params = recursive_dict_merge(calc_preset, self.kwargs)
         else:
-            self._user_calc_params = self.kwargs
+            self.user_calc_params = self.kwargs
 
-        if self._user_calc_params.get("kpts") and self._user_calc_params.get(
-            "kspacing"
-        ):
+        if self.user_calc_params.get("kpts") and self.user_calc_params.get("kspacing"):
             raise ValueError("Cannot specify both kpts and kspacing.")
```

### Comparing `quacc-0.7.3/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml` & `quacc-0.7.4/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml` & `quacc-0.7.4/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml` & `quacc-0.7.4/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/calculators/espresso/utils.py` & `quacc-0.7.4/src/quacc/calculators/espresso/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,15 +264,15 @@
         if need_wfc:
             to_copy.append(Path("pwscf.save", "wfc*.*"))
 
         to_copy.extend(
             [Path("pwscf.save", "data-file-schema.*"), Path("pwscf.save", "paw.*")]
         )
 
-    elif binary in ["ph", "phcg"]:
+    elif binary in {"ph", "phcg"}:
         to_copy.extend(pw_base)
         to_copy.append(Path("pwscf.save", "wfc*.*"))
 
         inputph = input_data.get("inputph", {})
         ldisp = inputph.get("ldisp", False)
         fildvscf = inputph.get("fildvscf", "")
         recover = inputph.get("recover", False)
@@ -292,24 +292,22 @@
                     ]
                 )
 
         if recover:
             to_copy.append(Path("_ph*", "pwscf.phsave"))
 
         if ldvscf_interpolate:
-            to_copy.append(Path("_ph*", "pwscf.dvscf*"))
-            to_copy.append(Path("w_pot"))
-
+            to_copy.extend((Path("_ph*", "pwscf.dvscf*"), Path("w_pot")))
             if lqdir:
                 to_copy.append(Path("_ph*", "pwscf.q_*", "pwscf.dvscf*"))
 
-    elif binary in ["dos", "fs"]:
+    elif binary in {"dos", "fs"}:
         to_copy.extend(pw_base)
 
-    elif binary in ["projwfc", "bands"]:
+    elif binary in {"projwfc", "bands"}:
         to_copy.extend(pw_base)
         to_copy.append(Path("pwscf.save", "wfc*.*"))
 
     elif binary == "pp":
         plotnum = input_data.get("plot_num", 0)
         wfc_needed = [3, 7, 10]
```

### Comparing `quacc-0.7.3/src/quacc/calculators/qchem/io.py` & `quacc-0.7.4/src/quacc/calculators/qchem/io.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/calculators/qchem/params.py` & `quacc-0.7.4/src/quacc/calculators/qchem/params.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/calculators/qchem/qchem.py` & `quacc-0.7.4/src/quacc/calculators/qchem/qchem.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/calculators/qchem/qchem_custodian.py` & `quacc-0.7.4/src/quacc/calculators/qchem/qchem_custodian.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/calculators/vasp/io.py` & `quacc-0.7.4/src/quacc/calculators/vasp/io.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/calculators/vasp/params.py` & `quacc-0.7.4/src/quacc/calculators/vasp/params.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml` & `quacc-0.7.4/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/calculators/vasp/presets/setups_pbe54.yaml` & `quacc-0.7.4/src/quacc/calculators/vasp/presets/setups_pbe54.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/calculators/vasp/presets/setups_qmof.yaml` & `quacc-0.7.4/src/quacc/calculators/vasp/presets/setups_qmof.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/calculators/vasp/vasp.py` & `quacc-0.7.4/src/quacc/calculators/vasp/vasp.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/calculators/vasp/vasp_custodian.py` & `quacc-0.7.4/src/quacc/calculators/vasp/vasp_custodian.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/common/defects.py` & `quacc-0.7.4/src/quacc/recipes/common/defects.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/common/elastic.py` & `quacc-0.7.4/src/quacc/recipes/common/elastic.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/common/phonons.py` & `quacc-0.7.4/src/quacc/recipes/common/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/common/slabs.py` & `quacc-0.7.4/src/quacc/recipes/common/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/dftb/_base.py` & `quacc-0.7.4/src/quacc/recipes/dftb/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/dftb/core.py` & `quacc-0.7.4/src/quacc/recipes/dftb/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/emt/core.py` & `quacc-0.7.4/src/quacc/recipes/emt/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/emt/defects.py` & `quacc-0.7.4/src/quacc/recipes/emt/defects.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/emt/elastic.py` & `quacc-0.7.4/src/quacc/recipes/emt/elastic.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/emt/phonons.py` & `quacc-0.7.4/src/quacc/recipes/emt/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/emt/slabs.py` & `quacc-0.7.4/src/quacc/recipes/emt/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/espresso/_base.py` & `quacc-0.7.4/src/quacc/recipes/espresso/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         calc_defaults=calc_defaults,
         calc_swaps=calc_swaps,
         parallel_info=parallel_info,
     )
 
     updated_copy_files = _prepare_copy(
         copy_files=copy_files,
-        calc_params=atoms.calc._user_calc_params,
+        calc_params=atoms.calc.user_calc_params,
         binary=atoms.calc.template.binary,
     )
 
     geom_file = template.outputname if template.binary == "pw" else None
 
     final_atoms = run_calc(atoms, geom_file=geom_file, copy_files=updated_copy_files)
 
@@ -167,15 +167,15 @@
         calc_defaults=calc_defaults,
         calc_swaps=calc_swaps,
         parallel_info=parallel_info,
     )
 
     updated_copy_files = _prepare_copy(
         copy_files=copy_files,
-        calc_params=atoms.calc._user_calc_params,
+        calc_params=atoms.calc.user_calc_params,
         binary=atoms.calc.template.binary,
     )
 
     opt_flags = recursive_dict_merge(opt_defaults, opt_params)
 
     dyn = run_opt(
         atoms, relax_cell=relax_cell, copy_files=updated_copy_files, **opt_flags
```

### Comparing `quacc-0.7.3/src/quacc/recipes/espresso/bands.py` & `quacc-0.7.4/src/quacc/recipes/espresso/bands.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/espresso/core.py` & `quacc-0.7.4/src/quacc/recipes/espresso/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/espresso/dos.py` & `quacc-0.7.4/src/quacc/recipes/espresso/dos.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/espresso/phonons.py` & `quacc-0.7.4/src/quacc/recipes/espresso/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/gaussian/_base.py` & `quacc-0.7.4/src/quacc/recipes/gaussian/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/gaussian/core.py` & `quacc-0.7.4/src/quacc/recipes/gaussian/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/gulp/_base.py` & `quacc-0.7.4/src/quacc/recipes/gulp/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/gulp/core.py` & `quacc-0.7.4/src/quacc/recipes/gulp/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/lj/core.py` & `quacc-0.7.4/src/quacc/recipes/lj/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/mlp/_base.py` & `quacc-0.7.4/src/quacc/recipes/mlp/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/mlp/core.py` & `quacc-0.7.4/src/quacc/recipes/mlp/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/mlp/phonons.py` & `quacc-0.7.4/src/quacc/recipes/mlp/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/newtonnet/core.py` & `quacc-0.7.4/src/quacc/recipes/newtonnet/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/newtonnet/ts.py` & `quacc-0.7.4/src/quacc/recipes/newtonnet/ts.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/onetep/_base.py` & `quacc-0.7.4/src/quacc/recipes/onetep/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/onetep/core.py` & `quacc-0.7.4/src/quacc/recipes/onetep/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/orca/_base.py` & `quacc-0.7.4/src/quacc/recipes/orca/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/orca/core.py` & `quacc-0.7.4/src/quacc/recipes/orca/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/psi4/_base.py` & `quacc-0.7.4/src/quacc/recipes/psi4/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/psi4/core.py` & `quacc-0.7.4/src/quacc/recipes/psi4/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/qchem/_base.py` & `quacc-0.7.4/src/quacc/recipes/qchem/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/qchem/core.py` & `quacc-0.7.4/src/quacc/recipes/qchem/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/qchem/ts.py` & `quacc-0.7.4/src/quacc/recipes/qchem/ts.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/tblite/core.py` & `quacc-0.7.4/src/quacc/recipes/tblite/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/tblite/phonons.py` & `quacc-0.7.4/src/quacc/recipes/tblite/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/vasp/_base.py` & `quacc-0.7.4/src/quacc/recipes/vasp/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/vasp/core.py` & `quacc-0.7.4/src/quacc/recipes/vasp/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/vasp/mp.py` & `quacc-0.7.4/src/quacc/recipes/vasp/mp.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/vasp/qmof.py` & `quacc-0.7.4/src/quacc/recipes/vasp/qmof.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/recipes/vasp/slabs.py` & `quacc-0.7.4/src/quacc/recipes/vasp/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/runners/ase.py` & `quacc-0.7.4/src/quacc/runners/ase.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from ase.io import Trajectory, read
 from ase.optimize import BFGS
 from ase.vibrations import Vibrations
 from monty.dev import requires
 from monty.os.path import zpath
 
 from quacc import SETTINGS
-from quacc.atoms.core import copy_atoms, get_final_atoms_from_dyn
+from quacc.atoms.core import copy_atoms, get_final_atoms_from_dynamics
 from quacc.runners.prep import calc_cleanup, calc_setup
 from quacc.utils.dicts import recursive_dict_merge
 
 try:
     from sella import Sella
 
 except ImportError:
@@ -231,15 +231,15 @@
         else:
             dyn.run(fmax=fmax, steps=max_steps, **run_kwargs)
 
     # Store the trajectory atoms
     dyn.traj_atoms = read(traj_file, index=":")
 
     # Perform cleanup operations
-    calc_cleanup(get_final_atoms_from_dyn(dyn), tmpdir, job_results_dir)
+    calc_cleanup(get_final_atoms_from_dynamics(dyn), tmpdir, job_results_dir)
 
     return dyn
 
 
 def run_vib(
     atoms: Atoms,
     vib_kwargs: VibKwargs | None = None,
```

### Comparing `quacc-0.7.3/src/quacc/runners/phonons.py` & `quacc-0.7.4/src/quacc/runners/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/runners/prep.py` & `quacc-0.7.4/src/quacc/runners/prep.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/runners/thermo.py` & `quacc-0.7.4/src/quacc/runners/thermo.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/schemas/_aliases/ase.py` & `quacc-0.7.4/src/quacc/schemas/_aliases/ase.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/schemas/_aliases/atoms.py` & `quacc-0.7.4/src/quacc/schemas/_aliases/atoms.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/schemas/_aliases/cclib.py` & `quacc-0.7.4/src/quacc/schemas/_aliases/cclib.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/schemas/_aliases/emmet.py` & `quacc-0.7.4/src/quacc/schemas/_aliases/emmet.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/schemas/_aliases/phonons.py` & `quacc-0.7.4/src/quacc/schemas/_aliases/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/schemas/_aliases/vasp.py` & `quacc-0.7.4/src/quacc/schemas/_aliases/vasp.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/schemas/ase.py` & `quacc-0.7.4/src/quacc/schemas/ase.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy as np
 from ase import units
 from ase.io import read
 from ase.vibrations import Vibrations
 from ase.vibrations.data import VibrationsData
 
 from quacc import SETTINGS, __version__
-from quacc.atoms.core import get_final_atoms_from_dyn
+from quacc.atoms.core import get_final_atoms_from_dynamics
 from quacc.schemas.atoms import atoms_to_metadata
 from quacc.schemas.prep import prep_next_run
 from quacc.utils.dicts import clean_task_doc, recursive_dict_merge
 from quacc.utils.files import get_uri
 from quacc.wflow_tools.db import results_to_db
 
 if TYPE_CHECKING:
@@ -184,15 +184,15 @@
         trajectory = (
             dyn.traj_atoms
             if hasattr(dyn, "traj_atoms")
             else read(dyn.trajectory.filename, index=":")
         )
 
     initial_atoms = trajectory[0]
-    final_atoms = get_final_atoms_from_dyn(dyn)
+    final_atoms = get_final_atoms_from_dynamics(dyn)
     directory = final_atoms.calc.directory
 
     # Check convergence
     is_converged = dyn.converged()
     if check_convergence and not is_converged:
         msg = f"Optimization did not converge. Refer to {directory}"
         raise RuntimeError(msg)
```

### Comparing `quacc-0.7.3/src/quacc/schemas/atoms.py` & `quacc-0.7.4/src/quacc/schemas/atoms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Schemas for storing metadata about Atoms objects."""
 
 from __future__ import annotations
 
+from copy import deepcopy
 from typing import TYPE_CHECKING
 
 from emmet.core.structure import MoleculeMetadata, StructureMetadata
-from monty.json import jsanitize
 from pymatgen.io.ase import AseAtomsAdaptor
 
 from quacc.atoms.core import (
     copy_atoms,
     get_charge_attribute,
     get_spin_multiplicity_attribute,
 )
@@ -79,17 +79,15 @@
             metadata = MoleculeMetadata().from_molecule(mol).model_dump()
             if store_pmg:
                 results["molecule"] = mol
     else:
         metadata = {}
 
     # Copy the info flags as a separate entry in the DB for easy querying
-    results["atoms_info"] = jsanitize(
-        atoms.info, enum_values=True, recursive_msonable=True
-    )
+    results["atoms_info"] = deepcopy(atoms.info)
 
     # Store Atoms object
     results["atoms"] = atoms
 
     # Combine the metadata and results dictionaries
     atoms_doc_unsorted = metadata | results | additional_fields
```

### Comparing `quacc-0.7.3/src/quacc/schemas/cclib.py` & `quacc-0.7.4/src/quacc/schemas/cclib.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,17 @@
 from inspect import getmembers, isclass
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 import cclib
 from ase.atoms import Atoms
 from cclib.io import ccread
-from monty.json import jsanitize
 
 from quacc import SETTINGS
-from quacc.atoms.core import get_final_atoms_from_dyn
+from quacc.atoms.core import get_final_atoms_from_dynamics
 from quacc.schemas.ase import summarize_opt_run, summarize_run
 from quacc.utils.dicts import clean_task_doc, recursive_dict_merge
 from quacc.utils.files import find_recent_logfile
 from quacc.wflow_tools.db import results_to_db
 
 if TYPE_CHECKING:
     from typing import Any, Literal
@@ -169,15 +168,15 @@
     if store:
         results_to_db(store, task_doc)
 
     return task_doc
 
 
 def summarize_cclib_opt_run(
-    dyn: Optimizer,
+    optimizer: Optimizer,
     logfile_extensions: str | list[str],
     trajectory: Trajectory | list[Atoms] | None = None,
     directory: Path | str | None = None,
     pop_analyses: (
         list[
             Literal[
                 "cpsa",
@@ -198,15 +197,15 @@
     store: Store | None = _DEFAULT_SETTING,
 ) -> cclibASEOptSchema:
     """
     Merges the results of a cclib run with the results of an ASE optimizer run.
 
     Parameters
     ----------
-    dyn
+    optimizer
         The ASE optimizer object
     logfile_extensions
         Possible extensions of the log file (e.g. ".log", ".out", ".txt",
         ".chk"). Note that only a partial match is needed. For instance, `.log`
         will match `.log.gz` and `.log.1.gz`. If multiple files with this
         extension are found, the one with the most recent change time will be
         used. For an exact match only, put in the full file name.
@@ -232,27 +231,27 @@
     Returns
     -------
     cclibASEOptSchema
         Dictionary representation of the task document
     """
     store = SETTINGS.STORE if store == _DEFAULT_SETTING else store
 
-    final_atoms = get_final_atoms_from_dyn(dyn)
+    final_atoms = get_final_atoms_from_dynamics(optimizer)
     directory = Path(directory or final_atoms.calc.directory)
     cclib_summary = cclib_summarize_run(
         final_atoms,
         logfile_extensions,
         directory=directory,
         pop_analyses=pop_analyses,
         check_convergence=check_convergence,
         additional_fields=additional_fields,
         store=None,
     )
     opt_run_summary = summarize_opt_run(
-        dyn,
+        optimizer,
         trajectory=trajectory,
         check_convergence=check_convergence,
         charge_and_multiplicity=(
             cclib_summary["charge"],
             cclib_summary["spin_multiplicity"],
         ),
         additional_fields=additional_fields,
@@ -324,15 +323,15 @@
     # Let's parse the log file with cclib
     cclib_obj = ccread(logfile, logging.ERROR)
     if not cclib_obj:
         msg = f"Could not parse {logfile}"
         raise RuntimeError(msg)
 
     # Fetch all the attributes (i.e. all input/outputs from cclib)
-    attributes = jsanitize(cclib_obj.getattributes())
+    attributes = cclib_obj.getattributes()
 
     # monty datetime bug workaround:
     # github.com/materialsvirtuallab/monty/issues/275
     if wall_time := attributes["metadata"].get("wall_time"):
         attributes["metadata"]["wall_time"] = [*map(str, wall_time)]
     if cpu_time := attributes["metadata"].get("cpu_time"):
         attributes["metadata"]["cpu_time"] = [*map(str, cpu_time)]
```

### Comparing `quacc-0.7.3/src/quacc/schemas/phonons.py` & `quacc-0.7.4/src/quacc/schemas/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/schemas/prep.py` & `quacc-0.7.4/src/quacc/schemas/prep.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/schemas/vasp.py` & `quacc-0.7.4/src/quacc/schemas/vasp.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from pymatgen.command_line.chargemol_caller import ChargemolAnalysis
 from pymatgen.entries.compatibility import (
     CompatibilityError,
     MaterialsProject2020Compatibility,
 )
 
 from quacc import SETTINGS
-from quacc.atoms.core import get_final_atoms_from_dyn
+from quacc.atoms.core import get_final_atoms_from_dynamics
 from quacc.schemas.ase import summarize_opt_run, summarize_run
 from quacc.utils.dicts import clean_task_doc, recursive_dict_merge
 from quacc.wflow_tools.db import results_to_db
 
 if TYPE_CHECKING:
     from typing import Any
 
@@ -183,15 +183,15 @@
     if store:
         results_to_db(store, task_doc)
 
     return task_doc
 
 
 def summarize_vasp_opt_run(
-    dyn: Optimizer,
+    optimizer: Optimizer,
     trajectory: Trajectory | list[Atoms] | None = None,
     directory: str | Path | None = None,
     move_magmoms: bool = True,
     run_bader: bool = _DEFAULT_SETTING,
     run_chargemol: bool = _DEFAULT_SETTING,
     check_convergence: bool = _DEFAULT_SETTING,
     report_mp_corrections: bool = False,
@@ -200,15 +200,15 @@
 ) -> VaspASESchema:
     """
     Merges the `vasp_summarize_run` with an `summarize_opt_run`, meant to
     be used for an ASE-based VASP relaxation.
 
     Parameters
     ----------
-    dyn
+    optimizer
         The ASE optimizer object
     trajectory
         ASE Trajectory object or list[Atoms] from reading a trajectory file. If
         None, the trajectory must be found in dyn.traj_atoms.
     directory
         Path to VASP outputs. A value of None specifies the calculator directory.
     move_magmoms
@@ -230,18 +230,18 @@
     additional_fields
         Additional fields to add to the task document.
     store
         Maggma Store object to store the results in. Defaults to `SETTINGS.STORE`,
     """
     store = SETTINGS.STORE if store == _DEFAULT_SETTING else store
 
-    final_atoms = get_final_atoms_from_dyn(dyn)
+    final_atoms = get_final_atoms_from_dynamics(optimizer)
     directory = Path(directory or final_atoms.calc.directory)
     opt_run_summary = summarize_opt_run(
-        dyn,
+        optimizer,
         trajectory=trajectory,
         check_convergence=check_convergence,
         move_magmoms=move_magmoms,
         additional_fields=additional_fields,
         store=None,
     )
     vasp_summary = vasp_summarize_run(
```

### Comparing `quacc-0.7.3/src/quacc/settings.py` & `quacc-0.7.4/src/quacc/settings.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/utils/dicts.py` & `quacc-0.7.4/src/quacc/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/utils/files.py` & `quacc-0.7.4/src/quacc/utils/files.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/utils/kpts.py` & `quacc-0.7.4/src/quacc/utils/kpts.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/utils/lists.py` & `quacc-0.7.4/src/quacc/utils/lists.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/wflow_tools/customizers.py` & `quacc-0.7.4/src/quacc/wflow_tools/customizers.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc/wflow_tools/db.py` & `quacc-0.7.4/src/quacc/wflow_tools/db.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Utility functions for interfacing with databases."""
 
 from __future__ import annotations
 
 import uuid
 from typing import TYPE_CHECKING
 
+from monty.json import jsanitize
+
 if TYPE_CHECKING:
     from typing import Any
 
     from maggma.core import Store
 
 
 def results_to_db(store: Store, results: dict[str, Any] | list[dict]) -> None:
@@ -27,12 +29,17 @@
     Returns
     -------
     None
     """
     if not isinstance(results, list):
         results = [results]
 
-    for result in results:
+    sanitized_results = [
+        jsanitize(result, enum_values=True, recursive_msonable=True)
+        for result in results
+    ]
+
+    for result in sanitized_results:
         result["uuid"] = str(uuid.uuid4())
 
     with store:
-        store.update(results, key="uuid")
+        store.update(sanitized_results, key="uuid")
```

### Comparing `quacc-0.7.3/src/quacc/wflow_tools/decorators.py` & `quacc-0.7.4/src/quacc/wflow_tools/decorators.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc.egg-info/PKG-INFO` & `quacc-0.7.4/src/quacc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quacc
-Version: 0.7.3
+Version: 0.7.4
 Summary: A platform to enable high-throughput, database-driven quantum chemistry and computational materials science
 Author-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 Maintainer-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 License: BSD-3
 Project-URL: repository, https://github.com/Quantum-Accelerators/quacc
 Project-URL: documentation, https://quantum-accelerators.github.io/quacc/
 Project-URL: changelog, https://github.com/Quantum-Accelerators/quacc/blob/main/CHANGELOG.md
@@ -24,21 +24,21 @@
 Requires-Python: <3.13,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: ase>3.22.1
 Requires-Dist: cclib>=1.8
 Requires-Dist: custodian>=2024.3.12
 Requires-Dist: emmet-core>=0.80.0
-Requires-Dist: maggma<=0.63.4
+Requires-Dist: maggma>=0.64.0
 Requires-Dist: monty>=2024.2.26
 Requires-Dist: numpy>=1.25.0
 Requires-Dist: psutil
 Requires-Dist: pydantic>=2.0.1
 Requires-Dist: pydantic-settings>=2.2.0
-Requires-Dist: pymatgen>=2024.2.20
+Requires-Dist: pymatgen>=2024.4.12
 Requires-Dist: typer>=0.12.1
 Provides-Extra: covalent
 Requires-Dist: covalent>=0.234.0rc0; extra == "covalent"
 Requires-Dist: covalent-cloud>=0.39.0; extra == "covalent"
 Provides-Extra: dask
 Requires-Dist: dask[distributed]>=2023.12.1; extra == "dask"
 Requires-Dist: dask-jobqueue>=0.8.2; extra == "dask"
@@ -71,15 +71,14 @@
 Provides-Extra: redun
 Requires-Dist: redun>=0.16.2; extra == "redun"
 Provides-Extra: sella
 Requires-Dist: sella>=2.3.3; extra == "sella"
 Provides-Extra: tblite
 Requires-Dist: tblite[ase]>=0.3.0; platform_system == "Linux" and extra == "tblite"
 Provides-Extra: dev
-Requires-Dist: codecov-cli>=0.4.1; extra == "dev"
 Requires-Dist: pytest>=7.4.0; extra == "dev"
 Requires-Dist: pytest-cov>=3.0.0; extra == "dev"
 Requires-Dist: ruff>=0.0.285; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: blacken-docs>=1.16.0; extra == "docs"
 Requires-Dist: mkdocs-material>=9.5.16; extra == "docs"
 Requires-Dist: mkdocstrings[python]>=0.22.0; extra == "docs"
```

### Comparing `quacc-0.7.3/src/quacc.egg-info/SOURCES.txt` & `quacc-0.7.4/src/quacc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quacc-0.7.3/src/quacc.egg-info/requires.txt` & `quacc-0.7.4/src/quacc.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ase>3.22.1
 cclib>=1.8
 custodian>=2024.3.12
 emmet-core>=0.80.0
-maggma<=0.63.4
+maggma>=0.64.0
 monty>=2024.2.26
 numpy>=1.25.0
 psutil
 pydantic>=2.0.1
 pydantic-settings>=2.2.0
-pymatgen>=2024.2.20
+pymatgen>=2024.4.12
 typer>=0.12.1
 
 [covalent]
 covalent>=0.234.0rc0
 covalent-cloud>=0.39.0
 
 [dask]
@@ -20,15 +20,14 @@
 dask-jobqueue>=0.8.2
 
 [defects]
 pymatgen-analysis-defects>=2023.8.22
 shakenbreak>=3.2.0
 
 [dev]
-codecov-cli>=0.4.1
 pytest>=7.4.0
 pytest-cov>=3.0.0
 ruff>=0.0.285
 
 [docs]
 blacken-docs>=1.16.0
 mkdocs-material>=9.5.16
```

