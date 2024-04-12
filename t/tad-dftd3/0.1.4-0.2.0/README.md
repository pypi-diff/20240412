# Comparing `tmp/tad_dftd3-0.1.4.tar.gz` & `tmp/tad_dftd3-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tad_dftd3-0.1.4.tar", last modified: Wed Jul 26 06:04:17 2023, max compression
+gzip compressed data, was "tad_dftd3-0.2.0.tar", last modified: Fri Apr 12 09:28:01 2024, max compression
```

## Comparing `tad_dftd3-0.1.4.tar` & `tad_dftd3-0.2.0.tar`

### file list

```diff
@@ -1,42 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:04:17.908684 tad_dftd3-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-07-26 06:04:17.908684 tad_dftd3-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-26 06:04:17.908684 tad_dftd3-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:04:17.896684 tad_dftd3-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:04:17.904684 tad_dftd3-0.1.4/src/tad_dftd3/
--rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:04:17.904684 tad_dftd3-0.1.4/src/tad_dftd3/damping/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/damping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/damping/atm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/damping/rational.py
--rw-r--r--   0 runner    (1001) docker     (123)    75727 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/disp.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/ncoord.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   893128 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/reference-c6.npy
--rw-r--r--   0 runner    (1001) docker     (123)    12173 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:04:17.904684 tad_dftd3-0.1.4/src/tad_dftd3/util/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/util/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/util/grad.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/util/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:04:17.904684 tad_dftd3-0.1.4/src/tad_dftd3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-07-26 06:04:17.000000 tad_dftd3-0.1.4/src/tad_dftd3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-26 06:04:17.000000 tad_dftd3-0.1.4/src/tad_dftd3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 06:04:17.000000 tad_dftd3-0.1.4/src/tad_dftd3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-26 06:04:17.000000 tad_dftd3-0.1.4/src/tad_dftd3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 06:04:17.000000 tad_dftd3-0.1.4/src/tad_dftd3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:04:17.908684 tad_dftd3-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/tests/test_dftd3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/tests/test_disp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/tests/test_ncoord.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 09:28:01.055168 tad_dftd3-0.2.0/
+-rw-rw-r--   0 friede    (1000) friede    (1000)    11358 2023-05-19 08:14:21.000000 tad_dftd3-0.2.0/LICENSE
+-rw-rw-r--   0 friede    (1000) friede    (1000)    11047 2024-04-12 09:28:01.055168 tad_dftd3-0.2.0/PKG-INFO
+-rw-rw-r--   0 friede    (1000) friede    (1000)    10167 2024-01-09 09:30:05.000000 tad_dftd3-0.2.0/README.rst
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1306 2024-01-17 12:28:41.000000 tad_dftd3-0.2.0/pyproject.toml
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1324 2024-04-12 09:28:01.059168 tad_dftd3-0.2.0/setup.cfg
+-rw-rw-r--   0 friede    (1000) friede    (1000)      679 2023-07-25 07:00:47.000000 tad_dftd3-0.2.0/setup.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 09:28:01.051168 tad_dftd3-0.2.0/src/
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 09:28:01.055168 tad_dftd3-0.2.0/src/tad_dftd3/
+-rw-rw-r--   0 friede    (1000) friede    (1000)     3485 2024-03-28 15:55:01.000000 tad_dftd3-0.2.0/src/tad_dftd3/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)      672 2024-04-12 09:27:58.000000 tad_dftd3-0.2.0/src/tad_dftd3/__version__.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 09:28:01.055168 tad_dftd3-0.2.0/src/tad_dftd3/damping/
+-rw-rw-r--   0 friede    (1000) friede    (1000)      762 2024-01-09 09:30:05.000000 tad_dftd3-0.2.0/src/tad_dftd3/damping/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     4772 2024-01-09 09:30:05.000000 tad_dftd3-0.2.0/src/tad_dftd3/damping/atm.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1990 2024-01-09 09:30:05.000000 tad_dftd3-0.2.0/src/tad_dftd3/damping/rational.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 09:28:01.055168 tad_dftd3-0.2.0/src/tad_dftd3/data/
+-rw-rw-r--   0 friede    (1000) friede    (1000)      761 2024-01-09 09:30:05.000000 tad_dftd3-0.2.0/src/tad_dftd3/data/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2464 2024-01-09 09:30:05.000000 tad_dftd3-0.2.0/src/tad_dftd3/data/r4r2.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1761 2024-01-09 09:30:05.000000 tad_dftd3-0.2.0/src/tad_dftd3/data/radii.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)    87275 2024-01-09 09:30:05.000000 tad_dftd3-0.2.0/src/tad_dftd3/data/vdw-d3.pt
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1671 2024-03-28 15:55:01.000000 tad_dftd3-0.2.0/src/tad_dftd3/defaults.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)    10612 2024-03-28 15:55:01.000000 tad_dftd3-0.2.0/src/tad_dftd3/disp.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)      832 2024-03-28 12:03:56.000000 tad_dftd3-0.2.0/src/tad_dftd3/exception.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     7059 2024-03-28 15:55:01.000000 tad_dftd3-0.2.0/src/tad_dftd3/model.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 09:28:01.055168 tad_dftd3-0.2.0/src/tad_dftd3/ncoord/
+-rw-rw-r--   0 friede    (1000) friede    (1000)      861 2024-03-28 15:55:01.000000 tad_dftd3-0.2.0/src/tad_dftd3/ncoord/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)        0 2023-07-25 07:00:43.000000 tad_dftd3-0.2.0/src/tad_dftd3/py.typed
+-rw-rw-r--   0 friede    (1000) friede    (1000)  4240619 2024-01-09 09:30:05.000000 tad_dftd3-0.2.0/src/tad_dftd3/reference-c6.pt
+-rw-rw-r--   0 friede    (1000) friede    (1000)    15344 2024-03-28 15:55:01.000000 tad_dftd3-0.2.0/src/tad_dftd3/reference.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 09:28:01.055168 tad_dftd3-0.2.0/src/tad_dftd3/typing/
+-rw-rw-r--   0 friede    (1000) friede    (1000)      756 2024-01-09 09:30:05.000000 tad_dftd3-0.2.0/src/tad_dftd3/typing/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)      899 2024-01-09 09:30:05.000000 tad_dftd3-0.2.0/src/tad_dftd3/typing/builtin.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)      822 2024-01-09 09:30:05.000000 tad_dftd3-0.2.0/src/tad_dftd3/typing/d3.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1075 2024-01-09 09:30:05.000000 tad_dftd3-0.2.0/src/tad_dftd3/typing/pytorch.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 09:28:01.055168 tad_dftd3-0.2.0/src/tad_dftd3.egg-info/
+-rw-r--r--   0 friede    (1000) friede    (1000)    11047 2024-04-12 09:28:00.000000 tad_dftd3-0.2.0/src/tad_dftd3.egg-info/PKG-INFO
+-rw-rw-r--   0 friede    (1000) friede    (1000)      838 2024-04-12 09:28:01.000000 tad_dftd3-0.2.0/src/tad_dftd3.egg-info/SOURCES.txt
+-rw-rw-r--   0 friede    (1000) friede    (1000)        1 2024-04-12 09:28:00.000000 tad_dftd3-0.2.0/src/tad_dftd3.egg-info/dependency_links.txt
+-rw-rw-r--   0 friede    (1000) friede    (1000)      205 2024-04-12 09:28:00.000000 tad_dftd3-0.2.0/src/tad_dftd3.egg-info/requires.txt
+-rw-rw-r--   0 friede    (1000) friede    (1000)       10 2024-04-12 09:28:00.000000 tad_dftd3-0.2.0/src/tad_dftd3.egg-info/top_level.txt
```

### Comparing `tad_dftd3-0.1.4/LICENSE` & `tad_dftd3-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.4/PKG-INFO` & `tad_dftd3-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: tad_dftd3
-Version: 0.1.4
+Version: 0.2.0
 Summary: Torch autodiff DFT-D3 implementation
 License: Apache-2.0
 Project-URL: Documentation, https://tad-dftd3.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/dftd3/tad-dftd3
 Project-URL: Tracker, https://github.com/dftd3/tad-dftd3/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
+Provides-Extra: tox
 License-File: LICENSE
 
 Torch autodiff for DFT-D3
 =========================
 
 .. image:: https://img.shields.io/github/v/release/dftd3/tad-dftd3
    :target: https://github.com/dftd3/tad-dftd3/releases/latest
@@ -76,193 +78,219 @@
 pip
 ~~~
 
 The project can easily be installed with ``pip``.
 
 .. code::
 
-   pip install tad-dftd3
-
+    pip install tad-dftd3
 
 From source
 ~~~~~~~~~~~
 
 This project is hosted on GitHub at `dftd3/tad-dftd3 <https://github.com/dftd3/tad-dftd3>`__.
 Obtain the source by cloning the repository with
 
 .. code::
 
-   git clone https://github.com/dftd3/tad-dftd3
-   cd tad-dftd3
+    git clone https://github.com/dftd3/tad-dftd3
+    cd tad-dftd3
 
 We recommend using a `conda <https://conda.io/>`__ environment to install the package.
 You can setup the environment manager using a `mambaforge <https://github.com/conda-forge/miniforge>`__ installer.
 Install the required dependencies from the conda-forge channel.
 
 .. code::
 
-   mamba env create -n torch -f environment.yml
-   mamba activate torch
+    mamba env create -n torch -f environment.yml
+    mamba activate torch
 
-For development, install the following additional dependencies
+Install this project with ``pip`` in the environment
 
 .. code::
 
-   mamba install black coverage covdefaults mypy pre-commit pylint pytest tox
+    pip install .
+
+The following dependencies are required
+
+- `numpy <https://numpy.org/>`__
+- `tad-mctc <https://github.com/tad-mctc/tad-mctc/>`__
+- `torch <https://pytorch.org/>`__
+- `pytest <https://docs.pytest.org/>`__ (tests only)
+
 
+Development
+-----------
 
-Install this project with pip in the environment
+For development, additionally install the following tools in your environment.
 
 .. code::
 
-   pip install .
+    mamba install black covdefaults mypy pre-commit pylint pytest pytest-cov pytest-xdist tox
+    pip install pytest-random-order
 
-Add the option ``-e`` for installing in development mode.
+With pip, add the option ``-e`` for installing in development mode, and add ``[dev]`` for the development dependencies
 
-The following dependencies are required
+.. code::
 
-- `numpy <https://numpy.org/>`__
-- `torch <https://pytorch.org/>`__
-- `pytest <https://docs.pytest.org/>`__ (tests only)
+    pip install -e .[dev]
 
-You can check your installation by running the test suite with pytest
+The pre-commit hooks are initialized by running the following command in the root of the repository.
 
 .. code::
 
-   pytest tests/ --pyargs tad_dftd3
+    pre-commit install
 
-or tox for testing multiple Python versions
+For testing all Python environments, simply run `tox`.
 
 .. code::
 
-  tox
+    tox
+
+Note that this randomizes the order of tests but skips "large" tests. To modify this behavior, `tox` has to skip the optional *posargs*.
+
+.. code::
+
+    tox -- test
 
 
 Example
 -------
 
 The following example shows how to calculate the DFT-D3 dispersion energy for a single structure.
 
 .. code:: python
 
-   import torch
-   import tad_dftd3 as d3
-
-   numbers = d3.util.to_number(symbols="C C C C N C S H H H H H".split())
-   positions = torch.tensor(
-       [
-           [-2.56745685564671, -0.02509985979910, 0.00000000000000],
-           [-1.39177582455797, +2.27696188880014, 0.00000000000000],
-           [+1.27784995624894, +2.45107479759386, 0.00000000000000],
-           [+2.62801937615793, +0.25927727028120, 0.00000000000000],
-           [+1.41097033661123, -1.99890996077412, 0.00000000000000],
-           [-1.17186102298849, -2.34220576284180, 0.00000000000000],
-           [-2.39505990368378, -5.22635838332362, 0.00000000000000],
-           [+2.41961980455457, -3.62158019253045, 0.00000000000000],
-           [-2.51744374846065, +3.98181713686746, 0.00000000000000],
-           [+2.24269048384775, +4.24389473203647, 0.00000000000000],
-           [+4.66488984573956, +0.17907568006409, 0.00000000000000],
-           [-4.60044244782237, -0.17794734637413, 0.00000000000000],
-       ]
-   )
-   param = {
-       "a1": torch.tensor(0.49484001),
-       "s8": torch.tensor(0.78981345),
-       "a2": torch.tensor(5.73083694),
-   }
-
-   energy = d3.dftd3(numbers, positions, param)
-
-   torch.set_printoptions(precision=10)
-   print(energy)
-   # tensor([-0.0004075971, -0.0003940886, -0.0003817684, -0.0003949536,
-   #         -0.0003577212, -0.0004110279, -0.0005385976, -0.0001808242,
-   #         -0.0001563670, -0.0001503394, -0.0001577045, -0.0001764488])
+    import torch
+    import tad_dftd3 as d3
+    import tad_mctc as mctc
+
+    numbers = mctc.convert.symbol_to_number(symbols="C C C C N C S H H H H H".split())
+    positions = torch.tensor(
+        [
+            [-2.56745685564671, -0.02509985979910, 0.00000000000000],
+            [-1.39177582455797, +2.27696188880014, 0.00000000000000],
+            [+1.27784995624894, +2.45107479759386, 0.00000000000000],
+            [+2.62801937615793, +0.25927727028120, 0.00000000000000],
+            [+1.41097033661123, -1.99890996077412, 0.00000000000000],
+            [-1.17186102298849, -2.34220576284180, 0.00000000000000],
+            [-2.39505990368378, -5.22635838332362, 0.00000000000000],
+            [+2.41961980455457, -3.62158019253045, 0.00000000000000],
+            [-2.51744374846065, +3.98181713686746, 0.00000000000000],
+            [+2.24269048384775, +4.24389473203647, 0.00000000000000],
+            [+4.66488984573956, +0.17907568006409, 0.00000000000000],
+            [-4.60044244782237, -0.17794734637413, 0.00000000000000],
+        ]
+    )
+    param = {
+        "a1": torch.tensor(0.49484001),
+        "s8": torch.tensor(0.78981345),
+        "a2": torch.tensor(5.73083694),
+    }
+
+    energy = d3.dftd3(numbers, positions, param)
+
+    torch.set_printoptions(precision=10)
+    print(energy)
+    # tensor([-0.0004075971, -0.0003940886, -0.0003817684, -0.0003949536,
+    #         -0.0003577212, -0.0004110279, -0.0005385976, -0.0001808242,
+    #         -0.0001563670, -0.0001503394, -0.0001577045, -0.0001764488])
 
 
 The next example shows the calculation of dispersion energies for a batch of structures, while retaining access to all intermediates used for calculating the dispersion energy.
 
 .. code:: python
 
-   import torch
-   import tad_dftd3 as d3
-
-   sample1 = dict(
-       numbers=d3.util.to_number("Pb H H H H Bi H H H".split()),
-       positions=torch.tensor(
-           [
-               [-0.00000020988889, -4.98043478877778, +0.00000000000000],
-               [+3.06964045311111, -6.06324400177778, +0.00000000000000],
-               [-1.53482054188889, -6.06324400177778, -2.65838526500000],
-               [-1.53482054188889, -6.06324400177778, +2.65838526500000],
-               [-0.00000020988889, -1.72196703577778, +0.00000000000000],
-               [-0.00000020988889, +4.77334244722222, +0.00000000000000],
-               [+1.35700257511111, +6.70626379422222, -2.35039772300000],
-               [-2.71400388988889, +6.70626379422222, +0.00000000000000],
-               [+1.35700257511111, +6.70626379422222, +2.35039772300000],
-           ]
-       ),
-   )
-   sample2 = dict(
-       numbers=d3.util.to_number("C C C C C C I H H H H H S H C H H H".split(" ")),
-       positions=torch.tensor(
-           [
-               [-1.42754169820131, -1.50508961850828, -1.93430551124333],
-               [+1.19860572924150, -1.66299114873979, -2.03189643761298],
-               [+2.65876001301880, +0.37736955363609, -1.23426391650599],
-               [+1.50963368042358, +2.57230374419743, -0.34128058818180],
-               [-1.12092277855371, +2.71045691257517, -0.25246348639234],
-               [-2.60071517756218, +0.67879949508239, -1.04550707592673],
-               [-2.86169588073340, +5.99660765711210, +1.08394899986031],
-               [+2.09930989272956, -3.36144811062374, -2.72237695164263],
-               [+2.64405246349916, +4.15317840474646, +0.27856972788526],
-               [+4.69864865613751, +0.26922271535391, -1.30274048619151],
-               [-4.63786461351839, +0.79856258572808, -0.96906659938432],
-               [-2.57447518692275, -3.08132039046931, -2.54875517521577],
-               [-5.88211879210329, 11.88491819358157, +2.31866455902233],
-               [-8.18022701418703, 10.95619984550779, +1.83940856333092],
-               [-5.08172874482867, 12.66714386256482, -0.92419491629867],
-               [-3.18311711399702, 13.44626574330220, -0.86977613647871],
-               [-5.07177399637298, 10.99164969235585, -2.10739192258756],
-               [-6.35955320518616, 14.08073002965080, -1.68204314084441],
-           ]
-       ),
-   )
-   numbers = d3.util.pack(
-       (
-           sample1["numbers"],
-           sample2["numbers"],
-       )
-   )
-   positions = d3.util.pack(
-       (
-           sample1["positions"],
-           sample2["positions"],
-       )
-   )
-   ref = d3.reference.Reference()
-   rcov = d3.data.covalent_rad_d3[numbers]
-   rvdw = d3.data.vdw_rad_d3[numbers.unsqueeze(-1), numbers.unsqueeze(-2)]
-   r4r2 = d3.data.sqrt_z_r4_over_r2[numbers]
-   param = {
-       "a1": torch.tensor(0.49484001),
-       "s8": torch.tensor(0.78981345),
-       "a2": torch.tensor(5.73083694),
-   }
-
-   cn = d3.ncoord.coordination_number(numbers, positions, rcov, d3.ncoord.exp_count)
-   weights = d3.model.weight_references(numbers, cn, ref, d3.model.gaussian_weight)
-   c6 = d3.model.atomic_c6(numbers, weights, ref)
-   energy = d3.disp.dispersion(
-       numbers, positions, c6, rvdw, r4r2, d3.disp.rational_damping, **param
-   )
-
-   torch.set_printoptions(precision=10)
-   print(torch.sum(energy, dim=-1))
-   # tensor([-0.0014092578, -0.0057840119])
+    import torch
+    import tad_dftd3 as d3
+    import tad_mctc as mctc
+
+    sample1 = dict(
+        numbers=mctc.convert.symbol_to_number("Pb H H H H Bi H H H".split()),
+        positions=torch.tensor(
+            [
+                [-0.00000020988889, -4.98043478877778, +0.00000000000000],
+                [+3.06964045311111, -6.06324400177778, +0.00000000000000],
+                [-1.53482054188889, -6.06324400177778, -2.65838526500000],
+                [-1.53482054188889, -6.06324400177778, +2.65838526500000],
+                [-0.00000020988889, -1.72196703577778, +0.00000000000000],
+                [-0.00000020988889, +4.77334244722222, +0.00000000000000],
+                [+1.35700257511111, +6.70626379422222, -2.35039772300000],
+                [-2.71400388988889, +6.70626379422222, +0.00000000000000],
+                [+1.35700257511111, +6.70626379422222, +2.35039772300000],
+            ]
+        ),
+    )
+    sample2 = dict(
+        numbers=mctc.convert.symbol_to_number(
+            "C C C C C C I H H H H H S H C H H H".split(" ")
+        ),
+        positions=torch.tensor(
+            [
+                [-1.42754169820131, -1.50508961850828, -1.93430551124333],
+                [+1.19860572924150, -1.66299114873979, -2.03189643761298],
+                [+2.65876001301880, +0.37736955363609, -1.23426391650599],
+                [+1.50963368042358, +2.57230374419743, -0.34128058818180],
+                [-1.12092277855371, +2.71045691257517, -0.25246348639234],
+                [-2.60071517756218, +0.67879949508239, -1.04550707592673],
+                [-2.86169588073340, +5.99660765711210, +1.08394899986031],
+                [+2.09930989272956, -3.36144811062374, -2.72237695164263],
+                [+2.64405246349916, +4.15317840474646, +0.27856972788526],
+                [+4.69864865613751, +0.26922271535391, -1.30274048619151],
+                [-4.63786461351839, +0.79856258572808, -0.96906659938432],
+                [-2.57447518692275, -3.08132039046931, -2.54875517521577],
+                [-5.88211879210329, 11.88491819358157, +2.31866455902233],
+                [-8.18022701418703, 10.95619984550779, +1.83940856333092],
+                [-5.08172874482867, 12.66714386256482, -0.92419491629867],
+                [-3.18311711399702, 13.44626574330220, -0.86977613647871],
+                [-5.07177399637298, 10.99164969235585, -2.10739192258756],
+                [-6.35955320518616, 14.08073002965080, -1.68204314084441],
+            ]
+        ),
+    )
+    numbers = mctc.batch.pack(
+        (
+            sample1["numbers"],
+            sample2["numbers"],
+        )
+    )
+    positions = mctc.batch.pack(
+        (
+            sample1["positions"],
+            sample2["positions"],
+        )
+    )
+    ref = d3.reference.Reference()
+    rcov = d3.data.COV_D3[numbers]
+    rvdw = d3.data.VDW_D3[numbers.unsqueeze(-1), numbers.unsqueeze(-2)]
+    r4r2 = d3.data.R4R2[numbers]
+    param = {
+        "a1": torch.tensor(0.49484001),
+        "s8": torch.tensor(0.78981345),
+        "a2": torch.tensor(5.73083694),
+    }
+
+    cn = mctc.ncoord.cn_d3(
+        numbers, positions, counting_function=mctc.ncoord.exp_count, rcov=rcov
+    )
+    weights = d3.model.weight_references(numbers, cn, ref, d3.model.gaussian_weight)
+    c6 = d3.model.atomic_c6(numbers, weights, ref)
+    energy = d3.disp.dispersion(
+        numbers,
+        positions,
+        param,
+        c6,
+        rvdw,
+        r4r2,
+        d3.disp.rational_damping,
+    )
+
+    torch.set_printoptions(precision=10)
+    print(torch.sum(energy, dim=-1))
+    # tensor([-0.0014092578, -0.0057840119])
 
 
 Contributing
 ------------
 
 This is a volunteer open source projects and contributions are always welcome.
 Please, take a moment to read the `contributing guidelines <CONTRIBUTING.md>`__.
```

### Comparing `tad_dftd3-0.1.4/README.rst` & `tad_dftd3-0.2.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -56,193 +56,219 @@
 pip
 ~~~
 
 The project can easily be installed with ``pip``.
 
 .. code::
 
-   pip install tad-dftd3
-
+    pip install tad-dftd3
 
 From source
 ~~~~~~~~~~~
 
 This project is hosted on GitHub at `dftd3/tad-dftd3 <https://github.com/dftd3/tad-dftd3>`__.
 Obtain the source by cloning the repository with
 
 .. code::
 
-   git clone https://github.com/dftd3/tad-dftd3
-   cd tad-dftd3
+    git clone https://github.com/dftd3/tad-dftd3
+    cd tad-dftd3
 
 We recommend using a `conda <https://conda.io/>`__ environment to install the package.
 You can setup the environment manager using a `mambaforge <https://github.com/conda-forge/miniforge>`__ installer.
 Install the required dependencies from the conda-forge channel.
 
 .. code::
 
-   mamba env create -n torch -f environment.yml
-   mamba activate torch
+    mamba env create -n torch -f environment.yml
+    mamba activate torch
 
-For development, install the following additional dependencies
+Install this project with ``pip`` in the environment
 
 .. code::
 
-   mamba install black coverage covdefaults mypy pre-commit pylint pytest tox
+    pip install .
+
+The following dependencies are required
+
+- `numpy <https://numpy.org/>`__
+- `tad-mctc <https://github.com/tad-mctc/tad-mctc/>`__
+- `torch <https://pytorch.org/>`__
+- `pytest <https://docs.pytest.org/>`__ (tests only)
+
 
+Development
+-----------
 
-Install this project with pip in the environment
+For development, additionally install the following tools in your environment.
 
 .. code::
 
-   pip install .
+    mamba install black covdefaults mypy pre-commit pylint pytest pytest-cov pytest-xdist tox
+    pip install pytest-random-order
 
-Add the option ``-e`` for installing in development mode.
+With pip, add the option ``-e`` for installing in development mode, and add ``[dev]`` for the development dependencies
 
-The following dependencies are required
+.. code::
 
-- `numpy <https://numpy.org/>`__
-- `torch <https://pytorch.org/>`__
-- `pytest <https://docs.pytest.org/>`__ (tests only)
+    pip install -e .[dev]
 
-You can check your installation by running the test suite with pytest
+The pre-commit hooks are initialized by running the following command in the root of the repository.
 
 .. code::
 
-   pytest tests/ --pyargs tad_dftd3
+    pre-commit install
 
-or tox for testing multiple Python versions
+For testing all Python environments, simply run `tox`.
 
 .. code::
 
-  tox
+    tox
+
+Note that this randomizes the order of tests but skips "large" tests. To modify this behavior, `tox` has to skip the optional *posargs*.
+
+.. code::
+
+    tox -- test
 
 
 Example
 -------
 
 The following example shows how to calculate the DFT-D3 dispersion energy for a single structure.
 
 .. code:: python
 
-   import torch
-   import tad_dftd3 as d3
-
-   numbers = d3.util.to_number(symbols="C C C C N C S H H H H H".split())
-   positions = torch.tensor(
-       [
-           [-2.56745685564671, -0.02509985979910, 0.00000000000000],
-           [-1.39177582455797, +2.27696188880014, 0.00000000000000],
-           [+1.27784995624894, +2.45107479759386, 0.00000000000000],
-           [+2.62801937615793, +0.25927727028120, 0.00000000000000],
-           [+1.41097033661123, -1.99890996077412, 0.00000000000000],
-           [-1.17186102298849, -2.34220576284180, 0.00000000000000],
-           [-2.39505990368378, -5.22635838332362, 0.00000000000000],
-           [+2.41961980455457, -3.62158019253045, 0.00000000000000],
-           [-2.51744374846065, +3.98181713686746, 0.00000000000000],
-           [+2.24269048384775, +4.24389473203647, 0.00000000000000],
-           [+4.66488984573956, +0.17907568006409, 0.00000000000000],
-           [-4.60044244782237, -0.17794734637413, 0.00000000000000],
-       ]
-   )
-   param = {
-       "a1": torch.tensor(0.49484001),
-       "s8": torch.tensor(0.78981345),
-       "a2": torch.tensor(5.73083694),
-   }
-
-   energy = d3.dftd3(numbers, positions, param)
-
-   torch.set_printoptions(precision=10)
-   print(energy)
-   # tensor([-0.0004075971, -0.0003940886, -0.0003817684, -0.0003949536,
-   #         -0.0003577212, -0.0004110279, -0.0005385976, -0.0001808242,
-   #         -0.0001563670, -0.0001503394, -0.0001577045, -0.0001764488])
+    import torch
+    import tad_dftd3 as d3
+    import tad_mctc as mctc
+
+    numbers = mctc.convert.symbol_to_number(symbols="C C C C N C S H H H H H".split())
+    positions = torch.tensor(
+        [
+            [-2.56745685564671, -0.02509985979910, 0.00000000000000],
+            [-1.39177582455797, +2.27696188880014, 0.00000000000000],
+            [+1.27784995624894, +2.45107479759386, 0.00000000000000],
+            [+2.62801937615793, +0.25927727028120, 0.00000000000000],
+            [+1.41097033661123, -1.99890996077412, 0.00000000000000],
+            [-1.17186102298849, -2.34220576284180, 0.00000000000000],
+            [-2.39505990368378, -5.22635838332362, 0.00000000000000],
+            [+2.41961980455457, -3.62158019253045, 0.00000000000000],
+            [-2.51744374846065, +3.98181713686746, 0.00000000000000],
+            [+2.24269048384775, +4.24389473203647, 0.00000000000000],
+            [+4.66488984573956, +0.17907568006409, 0.00000000000000],
+            [-4.60044244782237, -0.17794734637413, 0.00000000000000],
+        ]
+    )
+    param = {
+        "a1": torch.tensor(0.49484001),
+        "s8": torch.tensor(0.78981345),
+        "a2": torch.tensor(5.73083694),
+    }
+
+    energy = d3.dftd3(numbers, positions, param)
+
+    torch.set_printoptions(precision=10)
+    print(energy)
+    # tensor([-0.0004075971, -0.0003940886, -0.0003817684, -0.0003949536,
+    #         -0.0003577212, -0.0004110279, -0.0005385976, -0.0001808242,
+    #         -0.0001563670, -0.0001503394, -0.0001577045, -0.0001764488])
 
 
 The next example shows the calculation of dispersion energies for a batch of structures, while retaining access to all intermediates used for calculating the dispersion energy.
 
 .. code:: python
 
-   import torch
-   import tad_dftd3 as d3
-
-   sample1 = dict(
-       numbers=d3.util.to_number("Pb H H H H Bi H H H".split()),
-       positions=torch.tensor(
-           [
-               [-0.00000020988889, -4.98043478877778, +0.00000000000000],
-               [+3.06964045311111, -6.06324400177778, +0.00000000000000],
-               [-1.53482054188889, -6.06324400177778, -2.65838526500000],
-               [-1.53482054188889, -6.06324400177778, +2.65838526500000],
-               [-0.00000020988889, -1.72196703577778, +0.00000000000000],
-               [-0.00000020988889, +4.77334244722222, +0.00000000000000],
-               [+1.35700257511111, +6.70626379422222, -2.35039772300000],
-               [-2.71400388988889, +6.70626379422222, +0.00000000000000],
-               [+1.35700257511111, +6.70626379422222, +2.35039772300000],
-           ]
-       ),
-   )
-   sample2 = dict(
-       numbers=d3.util.to_number("C C C C C C I H H H H H S H C H H H".split(" ")),
-       positions=torch.tensor(
-           [
-               [-1.42754169820131, -1.50508961850828, -1.93430551124333],
-               [+1.19860572924150, -1.66299114873979, -2.03189643761298],
-               [+2.65876001301880, +0.37736955363609, -1.23426391650599],
-               [+1.50963368042358, +2.57230374419743, -0.34128058818180],
-               [-1.12092277855371, +2.71045691257517, -0.25246348639234],
-               [-2.60071517756218, +0.67879949508239, -1.04550707592673],
-               [-2.86169588073340, +5.99660765711210, +1.08394899986031],
-               [+2.09930989272956, -3.36144811062374, -2.72237695164263],
-               [+2.64405246349916, +4.15317840474646, +0.27856972788526],
-               [+4.69864865613751, +0.26922271535391, -1.30274048619151],
-               [-4.63786461351839, +0.79856258572808, -0.96906659938432],
-               [-2.57447518692275, -3.08132039046931, -2.54875517521577],
-               [-5.88211879210329, 11.88491819358157, +2.31866455902233],
-               [-8.18022701418703, 10.95619984550779, +1.83940856333092],
-               [-5.08172874482867, 12.66714386256482, -0.92419491629867],
-               [-3.18311711399702, 13.44626574330220, -0.86977613647871],
-               [-5.07177399637298, 10.99164969235585, -2.10739192258756],
-               [-6.35955320518616, 14.08073002965080, -1.68204314084441],
-           ]
-       ),
-   )
-   numbers = d3.util.pack(
-       (
-           sample1["numbers"],
-           sample2["numbers"],
-       )
-   )
-   positions = d3.util.pack(
-       (
-           sample1["positions"],
-           sample2["positions"],
-       )
-   )
-   ref = d3.reference.Reference()
-   rcov = d3.data.covalent_rad_d3[numbers]
-   rvdw = d3.data.vdw_rad_d3[numbers.unsqueeze(-1), numbers.unsqueeze(-2)]
-   r4r2 = d3.data.sqrt_z_r4_over_r2[numbers]
-   param = {
-       "a1": torch.tensor(0.49484001),
-       "s8": torch.tensor(0.78981345),
-       "a2": torch.tensor(5.73083694),
-   }
-
-   cn = d3.ncoord.coordination_number(numbers, positions, rcov, d3.ncoord.exp_count)
-   weights = d3.model.weight_references(numbers, cn, ref, d3.model.gaussian_weight)
-   c6 = d3.model.atomic_c6(numbers, weights, ref)
-   energy = d3.disp.dispersion(
-       numbers, positions, c6, rvdw, r4r2, d3.disp.rational_damping, **param
-   )
-
-   torch.set_printoptions(precision=10)
-   print(torch.sum(energy, dim=-1))
-   # tensor([-0.0014092578, -0.0057840119])
+    import torch
+    import tad_dftd3 as d3
+    import tad_mctc as mctc
+
+    sample1 = dict(
+        numbers=mctc.convert.symbol_to_number("Pb H H H H Bi H H H".split()),
+        positions=torch.tensor(
+            [
+                [-0.00000020988889, -4.98043478877778, +0.00000000000000],
+                [+3.06964045311111, -6.06324400177778, +0.00000000000000],
+                [-1.53482054188889, -6.06324400177778, -2.65838526500000],
+                [-1.53482054188889, -6.06324400177778, +2.65838526500000],
+                [-0.00000020988889, -1.72196703577778, +0.00000000000000],
+                [-0.00000020988889, +4.77334244722222, +0.00000000000000],
+                [+1.35700257511111, +6.70626379422222, -2.35039772300000],
+                [-2.71400388988889, +6.70626379422222, +0.00000000000000],
+                [+1.35700257511111, +6.70626379422222, +2.35039772300000],
+            ]
+        ),
+    )
+    sample2 = dict(
+        numbers=mctc.convert.symbol_to_number(
+            "C C C C C C I H H H H H S H C H H H".split(" ")
+        ),
+        positions=torch.tensor(
+            [
+                [-1.42754169820131, -1.50508961850828, -1.93430551124333],
+                [+1.19860572924150, -1.66299114873979, -2.03189643761298],
+                [+2.65876001301880, +0.37736955363609, -1.23426391650599],
+                [+1.50963368042358, +2.57230374419743, -0.34128058818180],
+                [-1.12092277855371, +2.71045691257517, -0.25246348639234],
+                [-2.60071517756218, +0.67879949508239, -1.04550707592673],
+                [-2.86169588073340, +5.99660765711210, +1.08394899986031],
+                [+2.09930989272956, -3.36144811062374, -2.72237695164263],
+                [+2.64405246349916, +4.15317840474646, +0.27856972788526],
+                [+4.69864865613751, +0.26922271535391, -1.30274048619151],
+                [-4.63786461351839, +0.79856258572808, -0.96906659938432],
+                [-2.57447518692275, -3.08132039046931, -2.54875517521577],
+                [-5.88211879210329, 11.88491819358157, +2.31866455902233],
+                [-8.18022701418703, 10.95619984550779, +1.83940856333092],
+                [-5.08172874482867, 12.66714386256482, -0.92419491629867],
+                [-3.18311711399702, 13.44626574330220, -0.86977613647871],
+                [-5.07177399637298, 10.99164969235585, -2.10739192258756],
+                [-6.35955320518616, 14.08073002965080, -1.68204314084441],
+            ]
+        ),
+    )
+    numbers = mctc.batch.pack(
+        (
+            sample1["numbers"],
+            sample2["numbers"],
+        )
+    )
+    positions = mctc.batch.pack(
+        (
+            sample1["positions"],
+            sample2["positions"],
+        )
+    )
+    ref = d3.reference.Reference()
+    rcov = d3.data.COV_D3[numbers]
+    rvdw = d3.data.VDW_D3[numbers.unsqueeze(-1), numbers.unsqueeze(-2)]
+    r4r2 = d3.data.R4R2[numbers]
+    param = {
+        "a1": torch.tensor(0.49484001),
+        "s8": torch.tensor(0.78981345),
+        "a2": torch.tensor(5.73083694),
+    }
+
+    cn = mctc.ncoord.cn_d3(
+        numbers, positions, counting_function=mctc.ncoord.exp_count, rcov=rcov
+    )
+    weights = d3.model.weight_references(numbers, cn, ref, d3.model.gaussian_weight)
+    c6 = d3.model.atomic_c6(numbers, weights, ref)
+    energy = d3.disp.dispersion(
+        numbers,
+        positions,
+        param,
+        c6,
+        rvdw,
+        r4r2,
+        d3.disp.rational_damping,
+    )
+
+    torch.set_printoptions(precision=10)
+    print(torch.sum(energy, dim=-1))
+    # tensor([-0.0014092578, -0.0057840119])
 
 
 Contributing
 ------------
 
 This is a volunteer open source projects and contributions are always welcome.
 Please, take a moment to read the `contributing guidelines <CONTRIBUTING.md>`__.
```

### Comparing `tad_dftd3-0.1.4/pyproject.toml` & `tad_dftd3-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -14,30 +14,34 @@
 # limitations under the License.
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules"
-testpaths = ["tests"]
+testpaths = ["test"]
 pythonpath = ["src"]
 markers = [
   "grad: Marks tests which perform 'gradcheck' evaluations, this can be slow.",
+  "large: Marks tests for large molecules, this can be slow.",
 ]
 
 
 [tool.mypy]
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
 warn_redundant_casts = true
 warn_unreachable = true
-warn_unused_ignores = false
+warn_unused_ignores = true
+exclude = '''(?x)(
+  test/conftest.py
+)'''
 
 
 [tool.coverage.run]
 plugins = ["covdefaults"]
 source = ["./src"]
 
 [tool.coverage.report]
-fail_under = 80
+fail_under = 90
```

### Comparing `tad_dftd3-0.1.4/setup.cfg` & `tad_dftd3-0.2.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -10,46 +10,58 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: Implementation :: CPython
 project_urls = 
 	Documentation = https://tad-dftd3.readthedocs.io/en/latest/
 	Source Code = https://github.com/dftd3/tad-dftd3
 	Tracker = https://github.com/dftd3/tad-dftd3/issues
 
 [options]
 packages = find:
 install_requires = 
 	numpy
+	opt-einsum
+	tad-mctc
 	torch
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 dev = 
 	black
 	covdefaults
-	coverage
 	mypy
 	pre-commit
 	pylint
 	pytest
+	pytest-cov
 	pytest-random-order
+	pytest-xdist
 	tox
+tox = 
+	covdefaults
+	pytest
+	pytest-cov
+	pytest-random-order
+	pytest-xdist
 
 [options.package_data]
 tad_dftd3 = 
 	py.typed
-	*.npy
+	**/*.npy
+	**/*.npz
+	**/*.pt
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `tad_dftd3-0.1.4/setup.py` & `tad_dftd3-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.4/src/tad_dftd3/__version__.py` & `tad_dftd3-0.2.0/src/tad_dftd3/damping/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-Version module for tad_dftd3.
-"""
-import torch
-
-__version__ = "0.1.4"
+Damping schemes
+===============
 
-__torch_version__ = torch.__version__
+Available damping schemes for two- and three-body dispersion terms.
+"""
+from .atm import *
+from .rational import *
```

### Comparing `tad_dftd3-0.1.4/src/tad_dftd3/constants.py` & `tad_dftd3-0.2.0/src/tad_dftd3/exception.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-This module contains fundamental constants and conversion factors.
+Exceptions
+==========
+
+Possible exceptions which can be raised by this module.
 """
+__all__ = ["DFTD3Error"]
+
 
-BOHR_TO_ANGSTROM = 0.529177210903
-"""Bohr radius in Angstroms."""
+class DFTD3Error(Exception):
+    """
+    Base class for exceptions raised by this module.
+    """
 
-ANGSTROM_TO_BOHR = 1.0 / BOHR_TO_ANGSTROM
-"""Conversion factor from Angstrom to Bohr."""
+    pass
```

### Comparing `tad_dftd3-0.1.4/src/tad_dftd3/damping/atm.py` & `tad_dftd3-0.2.0/src/tad_dftd3/damping/atm.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,18 +27,21 @@
     \dfrac{C^{\text{ABC}}_9
     \left(3 \cos\theta_\text{A} \cos\theta_\text{B} \cos\theta_\text{C} + 1 \right)}
     {\left(r_\text{AB} r_\text{BC} r_\text{AC} \right)^3} \\
     f_\text{damp} &=
     \dfrac{1}{1+ 6 \left(\overline{R}_\text{ABC}\right)^{-16}}
 """
 import torch
+from tad_mctc import storch
+from tad_mctc.batch import real_pairs, real_triples
 
 from .. import defaults
-from .._typing import DD, Tensor
-from ..util import cdist, real_pairs, real_triples
+from ..typing import DD, Tensor
+
+__all__ = ["dispersion_atm"]
 
 
 def dispersion_atm(
     numbers: Tensor,
     positions: Tensor,
     c6: Tensor,
     rvdw: Tensor,
@@ -79,39 +82,37 @@
     s9 = s9.type(positions.dtype).to(positions.device)
     rs9 = rs9.type(positions.dtype).to(positions.device)
     alp = alp.type(positions.dtype).to(positions.device)
 
     cutoff2 = cutoff * cutoff
     srvdw = rs9 * rvdw
 
-    mask_pairs = real_pairs(numbers, diagonal=False)
-    mask_triples = real_triples(numbers, self=False)
+    mask_pairs = real_pairs(numbers, mask_diagonal=True)
+    mask_triples = real_triples(numbers, mask_self=True)
 
     eps = torch.tensor(torch.finfo(positions.dtype).eps, **dd)
     zero = torch.tensor(0.0, **dd)
     one = torch.tensor(1.0, **dd)
 
     # C9_ABC = s9 * sqrt(|C6_AB * C6_AC * C6_BC|)
-    c9 = s9 * torch.sqrt(
-        torch.clamp(
-            torch.abs(c6.unsqueeze(-1) * c6.unsqueeze(-2) * c6.unsqueeze(-3)), min=eps
-        )
+    c9 = s9 * storch.sqrt(
+        torch.abs(c6.unsqueeze(-1) * c6.unsqueeze(-2) * c6.unsqueeze(-3))
     )
 
     r0ij = srvdw.unsqueeze(-1)
     r0ik = srvdw.unsqueeze(-2)
     r0jk = srvdw.unsqueeze(-3)
     r0 = r0ij * r0ik * r0jk
 
     # actually faster than other alternatives
     # very slow: (pos.unsqueeze(-2) - pos.unsqueeze(-3)).pow(2).sum(-1)
     distances = torch.pow(
         torch.where(
             mask_pairs,
-            cdist(positions, positions, p=2),
+            storch.cdist(positions, positions, p=2),
             eps,
         ),
         2.0,
     )
 
     r2ij = distances.unsqueeze(-1)
     r2ik = distances.unsqueeze(-2)
@@ -120,15 +121,15 @@
     r1 = torch.sqrt(r2)
     # add epsilon to avoid zero division later
     r3 = torch.where(mask_triples, r1 * r2, eps)
     r5 = torch.where(mask_triples, r2 * r3, eps)
 
     # dividing by tiny numbers leads to huge numbers, which result in NaN's
     # upon exponentiation in the subsequent step
-    mask = real_triples(numbers, self=False)
+    mask = real_triples(numbers, mask_self=True)
     base = r0 / torch.where(mask_triples, r1, one)
 
     # to fix the previous mask, we mask again (not strictly necessary because
     # `ang` is also masked and we later multiply with `ang`)
     fdamp = torch.where(
         mask_triples,
         1.0 / (1.0 + 6.0 * base ** ((alp + 2.0) / 3.0)),
```

### Comparing `tad_dftd3-0.1.4/src/tad_dftd3/damping/rational.py` & `tad_dftd3-0.2.0/src/tad_dftd3/damping/rational.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,18 +21,22 @@
 
 .. math::
 
     f^n_{\text{damp}}\left(R_0^{\text{AB}}\right) =
     \dfrac{R^n_{\text{AB}}}{R^n_{\text{AB}} +
     \left( a_1 R_0^{\text{AB}} + a_2 \right)^n}
 """
+from typing import Dict
+
 import torch
 
 from .. import defaults
-from .._typing import DD, Dict, Tensor
+from ..typing import DD, Tensor
+
+__all__ = ["rational_damping"]
 
 
 def rational_damping(
     order: int,
     distances: Tensor,
     qq: Tensor,
     param: Dict[str, Tensor],
```

### Comparing `tad_dftd3-0.1.4/src/tad_dftd3/defaults.py` & `tad_dftd3-0.2.0/src/tad_dftd3/typing/d3.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,33 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-Default values
-==============
+Type annotations: D3
+====================
 
-This module defines the default values for all parameters within DFT-D3.
+DFT-D3-specific type annotations.
 """
+from tad_mctc.typing import Callable, Tensor
 
-A1 = 0.4
-"""Scaling for the C8 / C6 ratio in the critical radius (0.4)."""
+__all__ = ["WeightingFunction"]
 
-A2 = 5.0
-"""Offset parameter for the critical radius (5.0)."""
 
-S6 = 1.0
-"""Scaling factor for the C6 interaction (1.0)."""
-
-S8 = 1.0
-"""Scaling factor for the C8 interaction (1.0)."""
-
-S9 = 1.0
-"""Scaling for dispersion coefficients (1.0)."""
-
-RS9 = 4.0 / 3.0
-"""Scaling for van-der-Waals radii in damping function (4.0/3.0)."""
-
-ALP = 14.0
-"""Exponent of zero damping function (14.0)."""
+WeightingFunction = Callable[[Tensor], Tensor]
```

### Comparing `tad_dftd3-0.1.4/src/tad_dftd3/disp.py` & `tad_dftd3-0.2.0/src/tad_dftd3/disp.py`

 * *Files 18% similar despite different names*

```diff
@@ -46,22 +46,118 @@
 ... )
 >>> cn = d3.ncoord.coordination_number(numbers, positions)
 >>> weights = d3.model.weight_references(numbers, cn, ref)
 >>> c6 = d3.model.atomic_c6(numbers, weights, ref)
 >>> energy = d3.disp.dispersion(numbers, positions, param, c6)
 >>> torch.set_printoptions(precision=7)
 >>> print(torch.sum(energy[0] - energy[1] - energy[2]))  # energy in Hartree
-tensor(-0.0003964)
+tensor(-0.0003964, dtype=torch.float64)
 """
+from typing import Dict, Optional
+
 import torch
+from tad_mctc import storch
+from tad_mctc.batch import real_pairs
+from tad_mctc.data import pse
 
-from . import data, defaults
-from ._typing import DD, Any, DampingFunction, Dict, Optional, Tensor
+from . import data, defaults, model, ncoord
 from .damping import dispersion_atm, rational_damping
-from .util import cdist, real_pairs
+from .reference import Reference
+from .typing import (
+    DD,
+    Any,
+    CountingFunction,
+    DampingFunction,
+    Tensor,
+    WeightingFunction,
+)
+
+__all__ = ["dftd3", "dispersion", "dispersion2", "dispersion3"]
+
+
+def dftd3(
+    numbers: Tensor,
+    positions: Tensor,
+    param: Dict[str, Tensor],
+    *,
+    ref: Optional[Reference] = None,
+    rcov: Optional[Tensor] = None,
+    rvdw: Optional[Tensor] = None,
+    r4r2: Optional[Tensor] = None,
+    cutoff: Optional[Tensor] = None,
+    counting_function: CountingFunction = ncoord.exp_count,
+    weighting_function: WeightingFunction = model.gaussian_weight,
+    damping_function: DampingFunction = rational_damping,
+) -> Tensor:
+    """
+    Evaluate DFT-D3 dispersion energy for a batch of geometries.
+
+    Parameters
+    ----------
+    numbers : torch.Tensor
+        Atomic numbers of the atoms in the system.
+    positions : torch.Tensor
+        Cartesian coordinates of the atoms in the system.
+    param : dict[str, Tensor]
+        DFT-D3 damping parameters.
+    ref : reference.Reference, optional
+        Reference C6 coefficients.
+    rcov : torch.Tensor, optional
+        Covalent radii of the atoms in the system.
+    rvdw : torch.Tensor, optional
+        Van der Waals radii of the atoms in the system.
+    r4r2 : torch.Tensor, optional
+        r⁴ over r² expectation values of the atoms in the system.
+    damping_function : Callable, optional
+        Damping function evaluate distance dependent contributions.
+    weighting_function : Callable, optional
+        Function to calculate weight of individual reference systems.
+    counting_function : Callable, optional
+        Calculates counting value in range 0 to 1 for each atom pair.
+
+    Returns
+    -------
+    Tensor
+        Atom-resolved DFT-D3 dispersion energy for each geometry.
+    """
+    dd: DD = {"device": positions.device, "dtype": positions.dtype}
+
+    if torch.max(numbers) >= defaults.MAX_ELEMENT:
+        raise ValueError(
+            f"No D3 parameters available for Z > {defaults.MAX_ELEMENT-1} "
+            f"({pse.Z2S[defaults.MAX_ELEMENT]})."
+        )
+
+    if cutoff is None:
+        cutoff = torch.tensor(defaults.D3_DISP_CUTOFF, **dd)
+    if ref is None:
+        ref = Reference(**dd)
+    if rcov is None:
+        rcov = data.COV_D3.to(**dd)[numbers]
+    if rvdw is None:
+        rvdw = data.VDW_D3.to(**dd)[numbers.unsqueeze(-1), numbers.unsqueeze(-2)]
+    if r4r2 is None:
+        r4r2 = data.R4R2.to(**dd)[numbers]
+
+    cn = ncoord.cn_d3(
+        numbers, positions, counting_function=counting_function, rcov=rcov
+    )
+    weights = model.weight_references(numbers, cn, ref, weighting_function)
+    c6 = model.atomic_c6(numbers, weights, ref)
+
+    return dispersion(
+        numbers,
+        positions,
+        param,
+        c6,
+        rvdw,
+        r4r2,
+        damping_function,
+        cutoff=cutoff,
+    )
 
 
 def dispersion(
     numbers: Tensor,
     positions: Tensor,
     param: Dict[str, Tensor],
     c6: Tensor,
@@ -96,41 +192,41 @@
     -------
     Tensor
         Atom-resolved DFT-D3 dispersion energy for each geometry.
     """
     dd: DD = {"device": positions.device, "dtype": positions.dtype}
 
     if cutoff is None:
-        cutoff = torch.tensor(50.0, **dd)
+        cutoff = torch.tensor(defaults.D3_DISP_CUTOFF, **dd)
     if r4r2 is None:
-        r4r2 = (
-            data.sqrt_z_r4_over_r2[numbers].type(positions.dtype).to(positions.device)
-        )
+        r4r2 = data.R4R2.to(**dd)[numbers]
+
     if numbers.shape != positions.shape[:-1]:
         raise ValueError(
             "Shape of positions is not consistent with atomic numbers.",
         )
     if numbers.shape != r4r2.shape:
         raise ValueError(
             "Shape of expectation values is not consistent with atomic numbers.",
         )
+    if torch.max(numbers) >= defaults.MAX_ELEMENT:
+        raise ValueError(
+            f"No D3 parameters available for Z > {defaults.MAX_ELEMENT-1} "
+            f"({pse.Z2S[defaults.MAX_ELEMENT]})."
+        )
 
     # two-body dispersion
     energy = dispersion2(
         numbers, positions, param, c6, r4r2, damping_function, cutoff, **kwargs
     )
 
     # three-body dispersion
     if "s9" in param and param["s9"] != 0.0:
         if rvdw is None:
-            rvdw = (
-                data.vdw_rad_d3[numbers.unsqueeze(-1), numbers.unsqueeze(-2)]
-                .type(positions.dtype)
-                .to(positions.device)
-            )
+            rvdw = data.VDW_D3.to(**dd)[numbers.unsqueeze(-1), numbers.unsqueeze(-2)]
 
         energy += dispersion3(numbers, positions, param, c6, rvdw, cutoff)
 
     return energy
 
 
 def dispersion2(
@@ -160,18 +256,18 @@
         r⁴ over r² expectation values of the atoms in the system.
     damping_function : Callable
         Damping function evaluate distance dependent contributions.
         Additional arguments are passed through to the function.
     """
     dd: DD = {"device": positions.device, "dtype": positions.dtype}
 
-    mask = real_pairs(numbers, diagonal=False)
+    mask = real_pairs(numbers, mask_diagonal=True)
     distances = torch.where(
         mask,
-        cdist(positions, positions, p=2),
+        storch.cdist(positions, positions, p=2),
         torch.tensor(torch.finfo(positions.dtype).eps, **dd),
     )
 
     qq = 3 * r4r2.unsqueeze(-1) * r4r2.unsqueeze(-2)
     c8 = c6 * qq
 
     t6 = torch.where(
```

### Comparing `tad_dftd3-0.1.4/src/tad_dftd3/exception.py` & `tad_dftd3-0.2.0/src/tad_dftd3/typing/builtin.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-Possible exceptions which can be raised by this module.
-"""
-
+Type annotations: Built-ins
+===========================
 
-class DFTD3Error(Exception):
-    """Base class for exceptions raised by this module."""
+Built-in type annotations are imported from the *tad-mctc* library, which
+handles some version checking.
+"""
+from tad_mctc.typing import Any, Callable, NoReturn, TypedDict
 
-    pass
+__all__ = ["Any", "Callable", "NoReturn", "TypedDict"]
```

### Comparing `tad_dftd3-0.1.4/src/tad_dftd3/model.py` & `tad_dftd3-0.2.0/src/tad_dftd3/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,63 +18,76 @@
 
 Implementation of D3 model to obtain atomic C6 coefficients for a given geometry.
 
 Examples
 --------
 >>> import torch
 >>> import tad_dftd3 as d3
->>> numbers = d3.util.to_number(["O", "H", "H"])
+>>> import tad_mctc as mctc
+>>> numbers = mctc.convert.symbol_to_number(["O", "H", "H"])
 >>> positions = torch.Tensor([
 ...     [+0.00000000000000, +0.00000000000000, -0.73578586109551],
 ...     [+1.44183152868459, +0.00000000000000, +0.36789293054775],
 ...     [-1.44183152868459, +0.00000000000000, +0.36789293054775],
 ... ])
 >>> ref = d3.reference.Reference()
 >>> rcov = d3.data.covalent_rad_d3[numbers]
->>> cn = d3.ncoord.coordination_number(numbers, positions, rcov, d3.ncoord.exp_count)
+>>> cn = mctc.ncoord.cn_d3(numbers, positions, rcov=rcov, counting_function=d3.ncoord.exp_count)
 >>> weights = d3.model.weight_references(numbers, cn, ref, d3.model.gaussian_weight)
 >>> c6 = d3.model.atomic_c6(numbers, weights, ref)
 >>> torch.set_printoptions(precision=7)
 >>> print(c6)
-tensor([[10.4130478,  5.4368815,  5.4368815],
-        [ 5.4368811,  3.0930152,  3.0930152],
-        [ 5.4368811,  3.0930152,  3.0930152]])
+tensor([[10.4130471,  5.4368822,  5.4368822],
+        [ 5.4368822,  3.0930154,  3.0930154],
+        [ 5.4368822,  3.0930154,  3.0930154]], dtype=torch.float64)
 """
 import torch
+from tad_mctc.math import einsum
 
-from ._typing import Any, Tensor, WeightingFunction
 from .reference import Reference
-from .util import real_atoms
+from .typing import Any, Tensor, WeightingFunction
+
+__all__ = ["atomic_c6", "gaussian_weight", "weight_references"]
 
 
 def atomic_c6(numbers: Tensor, weights: Tensor, reference: Reference) -> Tensor:
     """
     Calculate atomic dispersion coefficients.
 
     Parameters
     ----------
     numbers : Tensor
-        The atomic numbers of the atoms in the system.
+        The atomic numbers of the atoms in the system of shape `(..., nat)`.
     weights : Tensor
-        Weights of all reference systems.
+        Weights of all reference systems of shape `(..., nat, 7)`.
     reference : Reference
-        Reference systems for D3 model.
+        Reference systems for D3 model. Contains the reference C6 coefficients
+        of shape `(..., nelements, nelements, 7, 7)`.
 
     Returns
     -------
     Tensor
-        Atomic dispersion coefficients.
+        Atomic dispersion coefficients of shape `(..., nat, nat)`.
     """
+    # (..., nel, nel, 7, 7) -> (..., nat, nat, 7, 7)
+    rc6 = reference.c6[numbers.unsqueeze(-1), numbers.unsqueeze(-2)]
 
-    c6 = reference.c6[numbers.unsqueeze(-1), numbers.unsqueeze(-2)]
-    gw = torch.mul(
-        weights.unsqueeze(-1).unsqueeze(-3), weights.unsqueeze(-2).unsqueeze(-4)
+    # The default einsum path is fastest if the large tensors comes first.
+    # (..., n1, n2, r1, r2) * (..., n1, r1) * (..., n2, r2) -> (..., n1, n2)
+    return einsum(
+        "...ijab,...ia,...jb->...ij",
+        *(rc6, weights, weights),
+        optimize=[(0, 1), (0, 1)],
     )
 
-    return torch.sum(torch.sum(torch.mul(gw, c6), dim=-1), dim=-1)
+    # NOTE: This old version creates large intermediate tensors and builds the
+    # full matrix before the sum reduction, which requires a lot of memory.
+    #
+    # gw = w.unsqueeze(-1).unsqueeze(-3) * w.unsqueeze(-2).unsqueeze(-4)
+    # c6 = torch.sum(torch.sum(torch.mul(gw, rc6), dim=-1), dim=-1)
 
 
 def gaussian_weight(dcn: Tensor, factor: float = 4.0) -> Tensor:
     """
     Calculate weight of indivdual reference system.
 
     Parameters
@@ -115,16 +128,20 @@
         Function to calculate weight of individual reference systems.
 
     Returns
     -------
     Tensor
         Weights of all reference systems
     """
+    refcn = reference.cn[numbers]
+    mask = refcn >= 0
 
-    mask = reference.cn[numbers] >= 0
+    zero = torch.tensor(0.0, device=cn.device, dtype=cn.dtype)
+    zero_double = torch.tensor(0.0, device=cn.device, dtype=torch.double)
+    one = torch.tensor(1.0, device=cn.device, dtype=cn.dtype)
 
     # Due to the exponentiation, `norms` and `weights` may become very small.
     # This may cause problems for the division by `norms`. It may occur that
     # `weights` and `norms` are equal, in which case the result should be
     # exactly one. This might, however, not be the case and ultimately cause
     # larger deviations in the final values.
     #
@@ -132,27 +149,50 @@
     # contains higher powers, which lead to values down to 1e-300.
     # Since there are also cases in D3, we have to evaluate this portion
     # in double precision to retain the correct results and avoid nan's.
     dcn = (reference.cn[numbers] - cn.unsqueeze(-1)).type(torch.double)
     weights = torch.where(
         mask,
         weighting_function(dcn, **kwargs),
-        torch.tensor(0.0, device=dcn.device, dtype=dcn.dtype),  # not eps!
+        zero_double,  # not eps!
     )
 
-    # Nevertheless, we must avoid zero division here in batched calculations.
-    #
     # Previously, a small value was added to `norms` to prevent division by zero
     # (`norms = torch.add(torch.sum(weights, dim=-1), 1e-20)`). However, even
     # such small values can lead to relatively large deviations because the
     # small value is not added to the weights, and hence, the case where
     # `weights` and `norms` are equal does not yield one anymore. In fact, the
     # test suite fails because some elements deviate up to around 1e-4.
-    #
-    # We solve this issue by using a mask from the atoms and only add a small
-    # value, where the actual padding zeros are.
-    norms = torch.where(
-        real_atoms(numbers),
-        torch.sum(weights, dim=-1),
-        torch.tensor(torch.finfo(dcn.dtype).eps, device=cn.device, dtype=dcn.dtype),
+    # We solve this by running in double precision, adding a very small number
+    # and using multiple masks.
+
+    # normalize weights
+    norm = torch.where(
+        mask,
+        torch.sum(weights, dim=-1, keepdim=True),
+        torch.tensor(1e-300, device=cn.device, dtype=torch.double),  # double!
+    )
+
+    # back to real dtype
+    gw_temp = (weights / norm).type(cn.dtype)
+
+    # The following section handles cases with large CNs that lead to zeros in
+    # after the exponential in the weighting function. If this happens all
+    # weights become zero, which is not desired. Instead, we set the weight of
+    # the largest reference number to one.
+    # This case can occur if the CN of the current (actual) system is too far
+    # away from the largest CN of the reference systems. An example would be an
+    # atom within a fullerene (La3N@C80).
+
+    # maximum reference CN for each atom
+    maxcn = torch.max(refcn, dim=-1, keepdim=True)[0]
+
+    # prevent division by 0 and small values
+    exceptional = (torch.isnan(gw_temp)) | (gw_temp > torch.finfo(cn.dtype).max)
+
+    gw = torch.where(
+        exceptional,
+        torch.where(refcn == maxcn, one, zero),
+        gw_temp,
     )
-    return (weights / norms.unsqueeze(-1)).type(cn.dtype)
+
+    return torch.where(mask, gw, zero)
```

### Comparing `tad_dftd3-0.1.4/src/tad_dftd3.egg-info/PKG-INFO` & `tad_dftd3-0.2.0/src/tad_dftd3.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: tad-dftd3
-Version: 0.1.4
+Version: 0.2.0
 Summary: Torch autodiff DFT-D3 implementation
 License: Apache-2.0
 Project-URL: Documentation, https://tad-dftd3.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/dftd3/tad-dftd3
 Project-URL: Tracker, https://github.com/dftd3/tad-dftd3/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
+Provides-Extra: tox
 License-File: LICENSE
 
 Torch autodiff for DFT-D3
 =========================
 
 .. image:: https://img.shields.io/github/v/release/dftd3/tad-dftd3
    :target: https://github.com/dftd3/tad-dftd3/releases/latest
@@ -76,193 +78,219 @@
 pip
 ~~~
 
 The project can easily be installed with ``pip``.
 
 .. code::
 
-   pip install tad-dftd3
-
+    pip install tad-dftd3
 
 From source
 ~~~~~~~~~~~
 
 This project is hosted on GitHub at `dftd3/tad-dftd3 <https://github.com/dftd3/tad-dftd3>`__.
 Obtain the source by cloning the repository with
 
 .. code::
 
-   git clone https://github.com/dftd3/tad-dftd3
-   cd tad-dftd3
+    git clone https://github.com/dftd3/tad-dftd3
+    cd tad-dftd3
 
 We recommend using a `conda <https://conda.io/>`__ environment to install the package.
 You can setup the environment manager using a `mambaforge <https://github.com/conda-forge/miniforge>`__ installer.
 Install the required dependencies from the conda-forge channel.
 
 .. code::
 
-   mamba env create -n torch -f environment.yml
-   mamba activate torch
+    mamba env create -n torch -f environment.yml
+    mamba activate torch
 
-For development, install the following additional dependencies
+Install this project with ``pip`` in the environment
 
 .. code::
 
-   mamba install black coverage covdefaults mypy pre-commit pylint pytest tox
+    pip install .
+
+The following dependencies are required
+
+- `numpy <https://numpy.org/>`__
+- `tad-mctc <https://github.com/tad-mctc/tad-mctc/>`__
+- `torch <https://pytorch.org/>`__
+- `pytest <https://docs.pytest.org/>`__ (tests only)
+
 
+Development
+-----------
 
-Install this project with pip in the environment
+For development, additionally install the following tools in your environment.
 
 .. code::
 
-   pip install .
+    mamba install black covdefaults mypy pre-commit pylint pytest pytest-cov pytest-xdist tox
+    pip install pytest-random-order
 
-Add the option ``-e`` for installing in development mode.
+With pip, add the option ``-e`` for installing in development mode, and add ``[dev]`` for the development dependencies
 
-The following dependencies are required
+.. code::
 
-- `numpy <https://numpy.org/>`__
-- `torch <https://pytorch.org/>`__
-- `pytest <https://docs.pytest.org/>`__ (tests only)
+    pip install -e .[dev]
 
-You can check your installation by running the test suite with pytest
+The pre-commit hooks are initialized by running the following command in the root of the repository.
 
 .. code::
 
-   pytest tests/ --pyargs tad_dftd3
+    pre-commit install
 
-or tox for testing multiple Python versions
+For testing all Python environments, simply run `tox`.
 
 .. code::
 
-  tox
+    tox
+
+Note that this randomizes the order of tests but skips "large" tests. To modify this behavior, `tox` has to skip the optional *posargs*.
+
+.. code::
+
+    tox -- test
 
 
 Example
 -------
 
 The following example shows how to calculate the DFT-D3 dispersion energy for a single structure.
 
 .. code:: python
 
-   import torch
-   import tad_dftd3 as d3
-
-   numbers = d3.util.to_number(symbols="C C C C N C S H H H H H".split())
-   positions = torch.tensor(
-       [
-           [-2.56745685564671, -0.02509985979910, 0.00000000000000],
-           [-1.39177582455797, +2.27696188880014, 0.00000000000000],
-           [+1.27784995624894, +2.45107479759386, 0.00000000000000],
-           [+2.62801937615793, +0.25927727028120, 0.00000000000000],
-           [+1.41097033661123, -1.99890996077412, 0.00000000000000],
-           [-1.17186102298849, -2.34220576284180, 0.00000000000000],
-           [-2.39505990368378, -5.22635838332362, 0.00000000000000],
-           [+2.41961980455457, -3.62158019253045, 0.00000000000000],
-           [-2.51744374846065, +3.98181713686746, 0.00000000000000],
-           [+2.24269048384775, +4.24389473203647, 0.00000000000000],
-           [+4.66488984573956, +0.17907568006409, 0.00000000000000],
-           [-4.60044244782237, -0.17794734637413, 0.00000000000000],
-       ]
-   )
-   param = {
-       "a1": torch.tensor(0.49484001),
-       "s8": torch.tensor(0.78981345),
-       "a2": torch.tensor(5.73083694),
-   }
-
-   energy = d3.dftd3(numbers, positions, param)
-
-   torch.set_printoptions(precision=10)
-   print(energy)
-   # tensor([-0.0004075971, -0.0003940886, -0.0003817684, -0.0003949536,
-   #         -0.0003577212, -0.0004110279, -0.0005385976, -0.0001808242,
-   #         -0.0001563670, -0.0001503394, -0.0001577045, -0.0001764488])
+    import torch
+    import tad_dftd3 as d3
+    import tad_mctc as mctc
+
+    numbers = mctc.convert.symbol_to_number(symbols="C C C C N C S H H H H H".split())
+    positions = torch.tensor(
+        [
+            [-2.56745685564671, -0.02509985979910, 0.00000000000000],
+            [-1.39177582455797, +2.27696188880014, 0.00000000000000],
+            [+1.27784995624894, +2.45107479759386, 0.00000000000000],
+            [+2.62801937615793, +0.25927727028120, 0.00000000000000],
+            [+1.41097033661123, -1.99890996077412, 0.00000000000000],
+            [-1.17186102298849, -2.34220576284180, 0.00000000000000],
+            [-2.39505990368378, -5.22635838332362, 0.00000000000000],
+            [+2.41961980455457, -3.62158019253045, 0.00000000000000],
+            [-2.51744374846065, +3.98181713686746, 0.00000000000000],
+            [+2.24269048384775, +4.24389473203647, 0.00000000000000],
+            [+4.66488984573956, +0.17907568006409, 0.00000000000000],
+            [-4.60044244782237, -0.17794734637413, 0.00000000000000],
+        ]
+    )
+    param = {
+        "a1": torch.tensor(0.49484001),
+        "s8": torch.tensor(0.78981345),
+        "a2": torch.tensor(5.73083694),
+    }
+
+    energy = d3.dftd3(numbers, positions, param)
+
+    torch.set_printoptions(precision=10)
+    print(energy)
+    # tensor([-0.0004075971, -0.0003940886, -0.0003817684, -0.0003949536,
+    #         -0.0003577212, -0.0004110279, -0.0005385976, -0.0001808242,
+    #         -0.0001563670, -0.0001503394, -0.0001577045, -0.0001764488])
 
 
 The next example shows the calculation of dispersion energies for a batch of structures, while retaining access to all intermediates used for calculating the dispersion energy.
 
 .. code:: python
 
-   import torch
-   import tad_dftd3 as d3
-
-   sample1 = dict(
-       numbers=d3.util.to_number("Pb H H H H Bi H H H".split()),
-       positions=torch.tensor(
-           [
-               [-0.00000020988889, -4.98043478877778, +0.00000000000000],
-               [+3.06964045311111, -6.06324400177778, +0.00000000000000],
-               [-1.53482054188889, -6.06324400177778, -2.65838526500000],
-               [-1.53482054188889, -6.06324400177778, +2.65838526500000],
-               [-0.00000020988889, -1.72196703577778, +0.00000000000000],
-               [-0.00000020988889, +4.77334244722222, +0.00000000000000],
-               [+1.35700257511111, +6.70626379422222, -2.35039772300000],
-               [-2.71400388988889, +6.70626379422222, +0.00000000000000],
-               [+1.35700257511111, +6.70626379422222, +2.35039772300000],
-           ]
-       ),
-   )
-   sample2 = dict(
-       numbers=d3.util.to_number("C C C C C C I H H H H H S H C H H H".split(" ")),
-       positions=torch.tensor(
-           [
-               [-1.42754169820131, -1.50508961850828, -1.93430551124333],
-               [+1.19860572924150, -1.66299114873979, -2.03189643761298],
-               [+2.65876001301880, +0.37736955363609, -1.23426391650599],
-               [+1.50963368042358, +2.57230374419743, -0.34128058818180],
-               [-1.12092277855371, +2.71045691257517, -0.25246348639234],
-               [-2.60071517756218, +0.67879949508239, -1.04550707592673],
-               [-2.86169588073340, +5.99660765711210, +1.08394899986031],
-               [+2.09930989272956, -3.36144811062374, -2.72237695164263],
-               [+2.64405246349916, +4.15317840474646, +0.27856972788526],
-               [+4.69864865613751, +0.26922271535391, -1.30274048619151],
-               [-4.63786461351839, +0.79856258572808, -0.96906659938432],
-               [-2.57447518692275, -3.08132039046931, -2.54875517521577],
-               [-5.88211879210329, 11.88491819358157, +2.31866455902233],
-               [-8.18022701418703, 10.95619984550779, +1.83940856333092],
-               [-5.08172874482867, 12.66714386256482, -0.92419491629867],
-               [-3.18311711399702, 13.44626574330220, -0.86977613647871],
-               [-5.07177399637298, 10.99164969235585, -2.10739192258756],
-               [-6.35955320518616, 14.08073002965080, -1.68204314084441],
-           ]
-       ),
-   )
-   numbers = d3.util.pack(
-       (
-           sample1["numbers"],
-           sample2["numbers"],
-       )
-   )
-   positions = d3.util.pack(
-       (
-           sample1["positions"],
-           sample2["positions"],
-       )
-   )
-   ref = d3.reference.Reference()
-   rcov = d3.data.covalent_rad_d3[numbers]
-   rvdw = d3.data.vdw_rad_d3[numbers.unsqueeze(-1), numbers.unsqueeze(-2)]
-   r4r2 = d3.data.sqrt_z_r4_over_r2[numbers]
-   param = {
-       "a1": torch.tensor(0.49484001),
-       "s8": torch.tensor(0.78981345),
-       "a2": torch.tensor(5.73083694),
-   }
-
-   cn = d3.ncoord.coordination_number(numbers, positions, rcov, d3.ncoord.exp_count)
-   weights = d3.model.weight_references(numbers, cn, ref, d3.model.gaussian_weight)
-   c6 = d3.model.atomic_c6(numbers, weights, ref)
-   energy = d3.disp.dispersion(
-       numbers, positions, c6, rvdw, r4r2, d3.disp.rational_damping, **param
-   )
-
-   torch.set_printoptions(precision=10)
-   print(torch.sum(energy, dim=-1))
-   # tensor([-0.0014092578, -0.0057840119])
+    import torch
+    import tad_dftd3 as d3
+    import tad_mctc as mctc
+
+    sample1 = dict(
+        numbers=mctc.convert.symbol_to_number("Pb H H H H Bi H H H".split()),
+        positions=torch.tensor(
+            [
+                [-0.00000020988889, -4.98043478877778, +0.00000000000000],
+                [+3.06964045311111, -6.06324400177778, +0.00000000000000],
+                [-1.53482054188889, -6.06324400177778, -2.65838526500000],
+                [-1.53482054188889, -6.06324400177778, +2.65838526500000],
+                [-0.00000020988889, -1.72196703577778, +0.00000000000000],
+                [-0.00000020988889, +4.77334244722222, +0.00000000000000],
+                [+1.35700257511111, +6.70626379422222, -2.35039772300000],
+                [-2.71400388988889, +6.70626379422222, +0.00000000000000],
+                [+1.35700257511111, +6.70626379422222, +2.35039772300000],
+            ]
+        ),
+    )
+    sample2 = dict(
+        numbers=mctc.convert.symbol_to_number(
+            "C C C C C C I H H H H H S H C H H H".split(" ")
+        ),
+        positions=torch.tensor(
+            [
+                [-1.42754169820131, -1.50508961850828, -1.93430551124333],
+                [+1.19860572924150, -1.66299114873979, -2.03189643761298],
+                [+2.65876001301880, +0.37736955363609, -1.23426391650599],
+                [+1.50963368042358, +2.57230374419743, -0.34128058818180],
+                [-1.12092277855371, +2.71045691257517, -0.25246348639234],
+                [-2.60071517756218, +0.67879949508239, -1.04550707592673],
+                [-2.86169588073340, +5.99660765711210, +1.08394899986031],
+                [+2.09930989272956, -3.36144811062374, -2.72237695164263],
+                [+2.64405246349916, +4.15317840474646, +0.27856972788526],
+                [+4.69864865613751, +0.26922271535391, -1.30274048619151],
+                [-4.63786461351839, +0.79856258572808, -0.96906659938432],
+                [-2.57447518692275, -3.08132039046931, -2.54875517521577],
+                [-5.88211879210329, 11.88491819358157, +2.31866455902233],
+                [-8.18022701418703, 10.95619984550779, +1.83940856333092],
+                [-5.08172874482867, 12.66714386256482, -0.92419491629867],
+                [-3.18311711399702, 13.44626574330220, -0.86977613647871],
+                [-5.07177399637298, 10.99164969235585, -2.10739192258756],
+                [-6.35955320518616, 14.08073002965080, -1.68204314084441],
+            ]
+        ),
+    )
+    numbers = mctc.batch.pack(
+        (
+            sample1["numbers"],
+            sample2["numbers"],
+        )
+    )
+    positions = mctc.batch.pack(
+        (
+            sample1["positions"],
+            sample2["positions"],
+        )
+    )
+    ref = d3.reference.Reference()
+    rcov = d3.data.COV_D3[numbers]
+    rvdw = d3.data.VDW_D3[numbers.unsqueeze(-1), numbers.unsqueeze(-2)]
+    r4r2 = d3.data.R4R2[numbers]
+    param = {
+        "a1": torch.tensor(0.49484001),
+        "s8": torch.tensor(0.78981345),
+        "a2": torch.tensor(5.73083694),
+    }
+
+    cn = mctc.ncoord.cn_d3(
+        numbers, positions, counting_function=mctc.ncoord.exp_count, rcov=rcov
+    )
+    weights = d3.model.weight_references(numbers, cn, ref, d3.model.gaussian_weight)
+    c6 = d3.model.atomic_c6(numbers, weights, ref)
+    energy = d3.disp.dispersion(
+        numbers,
+        positions,
+        param,
+        c6,
+        rvdw,
+        r4r2,
+        d3.disp.rational_damping,
+    )
+
+    torch.set_printoptions(precision=10)
+    print(torch.sum(energy, dim=-1))
+    # tensor([-0.0014092578, -0.0057840119])
 
 
 Contributing
 ------------
 
 This is a volunteer open source projects and contributions are always welcome.
 Please, take a moment to read the `contributing guidelines <CONTRIBUTING.md>`__.
```

