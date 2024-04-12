# Comparing `tmp/CADET-Process-0.8.0.tar.gz` & `tmp/CADET-Process-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CADET-Process-0.8.0.tar", last modified: Mon Oct 16 07:44:13 2023, max compression
+gzip compressed data, was "CADET-Process-0.9.0.tar", last modified: Fri Apr 12 13:00:53 2024, max compression
```

## Comparing `CADET-Process-0.8.0.tar` & `CADET-Process-0.9.0.tar`

### file list

```diff
@@ -1,143 +1,148 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 07:44:13.505309 CADET-Process-0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 07:44:13.481308 CADET-Process-0.8.0/CADETProcess/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/CADETProcessError.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 07:44:13.481308 CADET-Process-0.8.0/CADETProcess/comparison/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/comparison/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11673 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/comparison/comparator.py
--rw-r--r--   0 runner    (1001) docker     (127)    29078 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/comparison/difference.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/comparison/peaks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6833 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/comparison/shape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 07:44:13.485309 CADET-Process-0.8.0/CADETProcess/dataStructure/
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/dataStructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/dataStructure/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/dataStructure/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    14411 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/dataStructure/dataStructure.py
--rw-r--r--   0 runner    (1001) docker     (127)     5053 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/dataStructure/diskcache.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/dataStructure/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/dataStructure/nested_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    46751 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/dataStructure/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/dataStructure/parameter_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 07:44:13.485309 CADET-Process-0.8.0/CADETProcess/dynamicEvents/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/dynamicEvents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46243 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/dynamicEvents/event.py
--rw-r--r--   0 runner    (1001) docker     (127)    23378 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/dynamicEvents/section.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 07:44:13.485309 CADET-Process-0.8.0/CADETProcess/equilibria/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/equilibria/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11300 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/equilibria/buffer_capacity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/equilibria/initial_conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5195 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/equilibria/ptc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/equilibria/reaction_equilibria.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 07:44:13.485309 CADET-Process-0.8.0/CADETProcess/fractionation/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/fractionation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12186 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/fractionation/fractionationOptimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23022 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/fractionation/fractionator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/fractionation/fractions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 07:44:13.489308 CADET-Process-0.8.0/CADETProcess/modelBuilder/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/modelBuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14993 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/modelBuilder/carouselBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10546 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/modelBuilder/compartmentBuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 07:44:13.489308 CADET-Process-0.8.0/CADETProcess/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4722 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/optimization/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    10672 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/optimization/individual.py
--rw-r--r--   0 runner    (1001) docker     (127)   119671 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/optimization/optimizationProblem.py
--rw-r--r--   0 runner    (1001) docker     (127)    20571 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/optimization/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/optimization/parallelizationBackend.py
--rw-r--r--   0 runner    (1001) docker     (127)    29162 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/optimization/population.py
--rw-r--r--   0 runner    (1001) docker     (127)     9610 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/optimization/pymooAdapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    28723 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/optimization/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    22295 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/optimization/scipyAdapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11535 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/performance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8400 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 07:44:13.493309 CADET-Process-0.8.0/CADETProcess/processModel/
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/processModel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34199 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/processModel/binding.py
--rw-r--r--   0 runner    (1001) docker     (127)    10658 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/processModel/componentSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)    23039 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/processModel/discretization.py
--rw-r--r--   0 runner    (1001) docker     (127)    31917 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/processModel/flowSheet.py
--rw-r--r--   0 runner    (1001) docker     (127)    25767 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/processModel/process.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24710 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/processModel/reaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/processModel/solutionRecorder.py
--rw-r--r--   0 runner    (1001) docker     (127)    33316 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/processModel/unitOperation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     8049 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/simulationResults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 07:44:13.493309 CADET-Process-0.8.0/CADETProcess/simulator/
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    62713 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/simulator/cadetAdapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13718 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/simulator/simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8797 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/smoothing2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    51188 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/solution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/stationarity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 07:44:13.493309 CADET-Process-0.8.0/CADETProcess/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7458 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/tools/yamamoto.py
--rw-r--r--   0 runner    (1001) docker     (127)    15233 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/CADETProcess/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 07:44:13.493309 CADET-Process-0.8.0/CADET_Process.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2023-10-16 07:44:13.000000 CADET-Process-0.8.0/CADET_Process.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2023-10-16 07:44:13.000000 CADET-Process-0.8.0/CADET_Process.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-16 07:44:13.000000 CADET-Process-0.8.0/CADET_Process.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      381 2023-10-16 07:44:13.000000 CADET-Process-0.8.0/CADET_Process.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-10-16 07:44:13.000000 CADET-Process-0.8.0/CADET_Process.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2023-10-16 07:44:13.505309 CADET-Process-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 07:44:13.493309 CADET-Process-0.8.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 07:44:13.493309 CADET-Process-0.8.0/examples/batch_elution/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/examples/batch_elution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/examples/batch_elution/optimization_multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/examples/batch_elution/optimization_single.py
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/examples/batch_elution/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 07:44:13.493309 CADET-Process-0.8.0/examples/characterize_chromatographic_system/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/examples/characterize_chromatographic_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/examples/characterize_chromatographic_system/binding_model_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6514 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/examples/characterize_chromatographic_system/column_transport_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/examples/characterize_chromatographic_system/particle_porosity.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/examples/characterize_chromatographic_system/system_periphery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 07:44:13.497309 CADET-Process-0.8.0/examples/load_wash_elute/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/examples/load_wash_elute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/examples/load_wash_elute/lwe_concentration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/examples/load_wash_elute/lwe_flow_rate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 07:44:13.497309 CADET-Process-0.8.0/examples/recycling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/examples/recycling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/examples/recycling/clr_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     6013 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/examples/recycling/mrssr_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2023-10-16 07:44:13.505309 CADET-Process-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 07:44:13.505309 CADET-Process-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8330 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/optimization_problem_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)     8104 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_buffer_capacity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_cadet_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_cadet_reactions.py
--rw-r--r--   0 runner    (1001) docker     (127)    20739 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_carousel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_compartment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_components.py
--rw-r--r--   0 runner    (1001) docker     (127)    12176 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_difference.py
--rw-r--r--   0 runner    (1001) docker     (127)     7228 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_equilibrium.py
--rw-r--r--   0 runner    (1001) docker     (127)    32476 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    18558 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_flow_sheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_fractions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_individual.py
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_optimization_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    40653 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_optimization_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_optimization_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_parallelization_adapter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19779 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_performance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7710 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_population.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_pymoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     9786 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_reaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    15034 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_sections.py
--rw-r--r--   0 runner    (1001) docker     (127)    19464 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_solution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2023-10-16 07:44:01.000000 CADET-Process-0.8.0/tests/test_unit_operation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.299767 CADET-Process-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.279767 CADET-Process-0.9.0/CADETProcess/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/CADETProcessError.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.279767 CADET-Process-0.9.0/CADETProcess/comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/comparison/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11838 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/comparison/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29103 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/comparison/difference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/comparison/peaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/comparison/shape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.283767 CADET-Process-0.9.0/CADETProcess/dataStructure/
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/dataStructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/dataStructure/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/dataStructure/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14411 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/dataStructure/dataStructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/dataStructure/diskcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/dataStructure/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/dataStructure/nested_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46781 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/dataStructure/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/dataStructure/parameter_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.283767 CADET-Process-0.9.0/CADETProcess/dynamicEvents/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/dynamicEvents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46703 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/dynamicEvents/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23338 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/dynamicEvents/section.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.283767 CADET-Process-0.9.0/CADETProcess/equilibria/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/equilibria/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11300 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/equilibria/buffer_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/equilibria/initial_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/equilibria/ptc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/equilibria/reaction_equilibria.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.283767 CADET-Process-0.9.0/CADETProcess/fractionation/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/fractionation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/fractionation/fractionationOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23970 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/fractionation/fractionator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/fractionation/fractions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.283767 CADET-Process-0.9.0/CADETProcess/modelBuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/modelBuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46700 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/modelBuilder/carouselBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10546 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/modelBuilder/compartmentBuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.287767 CADET-Process-0.9.0/CADETProcess/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19931 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/optimization/axAdapater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/optimization/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11294 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/optimization/individual.py
+-rw-r--r--   0 runner    (1001) docker     (127)   123858 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/optimization/optimizationProblem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22925 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/optimization/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/optimization/parallelizationBackend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30874 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/optimization/population.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9313 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/optimization/pymooAdapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29548 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/optimization/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20819 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/optimization/scipyAdapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11521 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10918 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.287767 CADET-Process-0.9.0/CADETProcess/processModel/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/processModel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40576 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/processModel/binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10658 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/processModel/componentSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23039 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/processModel/discretization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30805 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/processModel/flowSheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25841 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/processModel/process.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24710 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/processModel/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/processModel/solutionRecorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33320 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/processModel/unitOperation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8075 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/simulationResults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.287767 CADET-Process-0.9.0/CADETProcess/simulator/
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63873 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/simulator/cadetAdapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13718 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/simulator/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/smoothing2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    51247 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/stationarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/sysinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.291767 CADET-Process-0.9.0/CADETProcess/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/tools/yamamoto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.299767 CADET-Process-0.9.0/CADET_Process.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-04-12 13:00:53.000000 CADET-Process-0.9.0/CADET_Process.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-12 13:00:53.000000 CADET-Process-0.9.0/CADET_Process.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:00:53.000000 CADET-Process-0.9.0/CADET_Process.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-12 13:00:53.000000 CADET-Process-0.9.0/CADET_Process.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-12 13:00:53.000000 CADET-Process-0.9.0/CADET_Process.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-04-12 13:00:53.299767 CADET-Process-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.291767 CADET-Process-0.9.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.291767 CADET-Process-0.9.0/examples/batch_elution/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/batch_elution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/batch_elution/optimization_multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/batch_elution/optimization_single.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/batch_elution/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.291767 CADET-Process-0.9.0/examples/characterize_chromatographic_system/
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/characterize_chromatographic_system/Yamamoto_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/characterize_chromatographic_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/characterize_chromatographic_system/binding_model_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/characterize_chromatographic_system/column_transport_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/characterize_chromatographic_system/particle_porosity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/characterize_chromatographic_system/system_periphery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.291767 CADET-Process-0.9.0/examples/load_wash_elute/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/load_wash_elute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/load_wash_elute/lwe_concentration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/load_wash_elute/lwe_flow_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/load_wash_elute/lwe_hic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.291767 CADET-Process-0.9.0/examples/recycling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/recycling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/recycling/clr_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/recycling/mrssr_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-12 13:00:53.303767 CADET-Process-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.299767 CADET-Process-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22567 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/optimization_problem_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_buffer_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_cadet_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_cadet_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20831 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_carousel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_compartment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_difference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_equilibrium.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34020 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30279 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_flow_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_fractions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_individual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_optimization_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46428 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_optimization_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_optimization_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_optimizer_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_parallelization_adapter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19841 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7710 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_population.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_pymoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9786 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16395 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_sections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19464 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_unit_operation.py
```

### Comparing `CADET-Process-0.8.0/CADETProcess/__init__.py` & `CADET-Process-0.9.0/CADETProcess/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 CADET-Process is a Python package for modelling, simulating and optimizing
 advanced chromatographic systems. It serves as an inteface for CADET, but also
 for other solvers.
 
 See https://cadet-process.readthedocs.io for complete documentation.
 """
 # Version information
-name = 'CADET-Process'
-__version__ = '0.8.0'
+name = "CADET-Process"
+__version__ = "0.9.0"
 
 # Imports
 from .CADETProcessError import *
 
 from . import log
 
 from .settings import Settings
+
 settings = Settings()
 
+from . import sysinfo
 from . import dataStructure
 from . import transform
 from . import plotting
 from . import dynamicEvents
 from . import processModel
 from . import smoothing
 from . import solution
```

### Comparing `CADET-Process-0.8.0/CADETProcess/comparison/__init__.py` & `CADET-Process-0.9.0/CADETProcess/comparison/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/comparison/comparator.py` & `CADET-Process-0.9.0/CADETProcess/comparison/comparator.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,14 +78,19 @@
 
     @property
     def metrics(self):
         """list: List of difference metrics."""
         return self._metrics
 
     @property
+    def n_diffference_metrics(self):
+        """int: Number of difference metrics in the Comparator."""
+        return len(self.metrics)
+
+    @property
     def n_metrics(self):
         """int: Number of metrics to be evaluated."""
         return sum([metric.n_metrics for metric in self.metrics])
 
     @property
     def bad_metrics(self):
         """list: Worst case metrics for all difference metrics."""
@@ -229,30 +234,28 @@
             Default is False.
 
         Returns
         -------
         tuple
             A tuple of the comparison figure(s) and axes object(s).
         """
-        n = len(self.metrics)
-
-        if n == 0:
+        if self.n_diffference_metrics == 0:
             return (None, None)
 
-        comparison_fig_all, comparison_axs_all = plt.subplots(
-            nrows=n,
-            figsize=(8 + 4 + 2, n*8 + 2),
+        comparison_fig_all, comparison_axs_all = plotting.setup_figure(
+            n_rows=self.n_diffference_metrics,
             squeeze=False
         )
+
         plt.close(comparison_fig_all)
         comparison_axs_all = comparison_axs_all.reshape(-1)
 
         comparison_fig_ind = []
         comparison_axs_ind = []
-        for i in range(n):
+        for i in range(self.n_diffference_metrics):
             fig, axs = plt.subplots()
             comparison_fig_ind.append(fig)
             comparison_axs_ind.append(axs)
             plt.close(fig)
 
         comparison_axs_ind = \
             np.array(comparison_axs_ind).reshape(comparison_axs_all.shape)
```

### Comparing `CADET-Process-0.8.0/CADETProcess/comparison/difference.py` & `CADET-Process-0.9.0/CADETProcess/comparison/difference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import abstractmethod
 import copy
 from functools import wraps
 from warnings import warn
 
 import numpy as np
-from scipy.integrate import simps
+from scipy.integrate import simpson
 from scipy.special import expit
 
 from CADETProcess import CADETProcessError
 from CADETProcess.dataStructure import UnsignedInteger
 from CADETProcess.solution import SolutionBase, slice_solution
 from CADETProcess.metric import MetricBase
 from .shape import pearson, pearson_offset
@@ -173,15 +173,15 @@
             self._reference.resample()
         if self.normalize and not self._reference.is_normalized:
             self._reference.normalize()
         if self.smooth and not self._reference.is_smoothed:
             self._reference.smooth_data()
         reference = slice_solution(
             self._reference,
-            None,
+            self.components,
             self.use_total_concentration,
             self.use_total_concentration_components,
             coordinates={'time': (self.start, self.end)}
         )
 
         self._reference_sliced_and_transformed = reference
 
@@ -403,18 +403,18 @@
 
         Parameters
         ----------
         solution : SolutionIO
             Concentration profile of simulation.
 
         """
-        area_ref = simps(
+        area_ref = simpson(
             self.reference.solution, self.reference.time, axis=0
         )
-        area_sol = simps(solution.solution, solution.time, axis=0)
+        area_sol = simpson(solution.solution, solution.time, axis=0)
 
         return abs(area_ref - area_sol)
 
 
 class RelativeArea(DifferenceBase):
     """Relative difference in area difference metric."""
 
@@ -423,18 +423,18 @@
 
         Parameters
         ----------
         solution : SolutionIO
             Concentration profile of simulation.
 
         """
-        area_ref = simps(
-            self.reference.solution, self.reference.time, axis=0
+        area_ref = simpson(
+            self.reference.solution, x=self.reference.time, axis=0
         )
-        area_new = simps(solution.solution, solution.time, axis=0)
+        area_new = simpson(solution.solution, x=solution.time, axis=0)
 
         return abs(area_ref - area_new)/area_ref
 
 
 class Shape(DifferenceBase):
     """Shape similarity difference metric.
```

### Comparing `CADET-Process-0.8.0/CADETProcess/comparison/peaks.py` & `CADET-Process-0.9.0/CADETProcess/comparison/peaks.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/comparison/shape.py` & `CADET-Process-0.9.0/CADETProcess/comparison/shape.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/dataStructure/__init__.py` & `CADET-Process-0.9.0/CADETProcess/dataStructure/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/dataStructure/aggregator.py` & `CADET-Process-0.9.0/CADETProcess/dataStructure/aggregator.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/dataStructure/cache.py` & `CADET-Process-0.9.0/CADETProcess/dataStructure/cache.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/dataStructure/dataStructure.py` & `CADET-Process-0.9.0/CADETProcess/dataStructure/dataStructure.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/dataStructure/diskcache.py` & `CADET-Process-0.9.0/CADETProcess/dataStructure/diskcache.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/dataStructure/nested_dict.py` & `CADET-Process-0.9.0/CADETProcess/dataStructure/nested_dict.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/dataStructure/parameter.py` & `CADET-Process-0.9.0/CADETProcess/dataStructure/parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     Switch
     Typed
     Bool
     Integer
     Tuple
     Float
     String
-    Dict
+    Dictionary
     """
 
     def __init__(
             self,
             *args,
             default=None,
             is_optional=False,
@@ -374,15 +374,15 @@
     --------
     Parameter
     Bool
     Integer
     Tuple
     Float
     String
-    Dict
+    Dictionary
     """
 
     def __init__(self, *args, ty=None, **kwargs):
         """
         Initialize a Typed instance.
 
         Parameters
@@ -564,23 +564,16 @@
 
 class List(Typed):
     """Parameter descriptor constrained to list values."""
 
     ty = list
 
 
-class Dict(Typed):
-    """
-    Parameter descriptor constrained to dictionary (`dict`) values.
-
-    Notes
-    -----
-    When integrating with libraries like `addict`, be cautious about potential
-    name collisions with `addict.Dict`.
-    """
+class Dictionary(Typed):
+    """Parameter descriptor constrained to dictionary (`dict`) values."""
 
     ty = dict
 
 
 class NdArray(Typed):
     """
     Parameter descriptor constrained to np.ndarray values.
@@ -1032,18 +1025,18 @@
         ValueError
             If the value's size does not match the expected size.
         """
         if np.array(value).size == 1:
             return
 
         size = self.get_size(value)
-        exptected_size = self.get_expected_size(instance)
+        expected_size = self.get_expected_size(instance)
 
-        if size != exptected_size:
-            raise ValueError(f"Expected size {exptected_size}")
+        if size != expected_size:
+            raise ValueError(f"Expected size {expected_size}")
 
     def _prepare(self, instance, value, recursive=False):
         """
         Prepare the value by typecasting and adjusting its size.
 
         This method handles typecasting of the provided value to the expected type
         (`self.ty`) and potentially adjusts its size. If the size of the parameter
@@ -1525,15 +1518,15 @@
             n_coeff = dims[1]
             single_entry = False
 
         if single_entry and n_entries > 1:
             raise ValueError("Can only set single entry if n_entries == 1.")
 
         if isinstance(value, np.ndarray) and value.size == 1:
-            value = float(value)
+            value = float(value.squeeze())
 
         if isinstance(value, (int, float)):
             value = n_entries * [value]
         elif isinstance(value, np.ndarray):
             value = value.tolist()
 
         if len(value) != n_entries:
@@ -1646,19 +1639,24 @@
 
         Raises
         ------
         ValueError
             If the modulo condition of the size does not meet the expected criteria.
         """
         size = self.get_size(value)
-        exptected_size = self.get_expected_size(instance)
+        expected_size = self.get_expected_size(instance)
 
-        size %= exptected_size
+        size %= expected_size
 
         if size != 0:
-            raise ValueError("Size mod exptected size is not 0")
+            raise ValueError(
+                f"The size of the value modulo the expected size is not zero. "
+                f"Size: {size}, Expected Size: {expected_size}"
+            )
+
+    check_size = check_mod_value
 
 
 class DependentlyModulatedUnsignedList(UnsignedList, SizedList, DependentlyModulated):
     """List of unsigned values whose size is dependent on other attributes."""
 
     pass
```

### Comparing `CADET-Process-0.8.0/CADETProcess/dataStructure/parameter_group.py` & `CADET-Process-0.9.0/CADETProcess/dataStructure/parameter_group.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/dynamicEvents/__init__.py` & `CADET-Process-0.9.0/CADETProcess/dynamicEvents/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/dynamicEvents/event.py` & `CADET-Process-0.9.0/CADETProcess/dynamicEvents/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,14 @@
     n_sections : int
         Total number of sections derived from the section times.
     section_states : dict
         A dictionary providing the state of event parameters at the beginning of every section.
     parameter_events : dict
         A dictionary mapping each parameter to the list of events that affect it.
 
-
     Notes
     -----
     The class relies heavily on the concept of "events", which are instances
     of dynamic changes that can influence parameters in the system. These events
     can be independent or based on other events, creating intricate relationships
     to capture complex scenarios.
 
@@ -91,30 +90,30 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self._events = []
         self._durations = []
         self._lock = False
 
-    @property
+    @cached_property_if_locked
     def events(self):
         """list: All Events ordered by event time.
 
         See Also
         --------
         Event
         add_event
         remove_event
         event_dependencies
         Durations
 
         """
         return sorted(self._events, key=lambda evt: evt.time)
 
-    @property
+    @cached_property_if_locked
     def events_dict(self):
         """dict: Events and Durations orderd by name."""
         evts = {evt.name: evt for evt in self.events}
         durs = {dur.name: dur for dur in self.durations}
         return {**evts, **durs}
 
     def add_event(
@@ -153,14 +152,15 @@
         CADETProcessError
             If EventPerformer is not found in EventHandler
 
         See Also
         --------
         events
         remove_event
+        add_event_dependency
         Event
         Event.add_dependency
         add_duration
         """
         if name in self.events_dict:
             raise CADETProcessError("Event already exists")
         evt = Event(name, self, parameter_path, state, time=time, indices=indices)
@@ -272,15 +272,15 @@
             dur = self.events_dict[duration_name]
         except KeyError:
             raise CADETProcessError("Duration does not exist")
 
         self._durations.remove(dur)
         self.__dict__.pop(duration_name)
 
-    @property
+    @cached_property_if_locked
     def durations(self):
         """List of all durations in the process."""
         return self._durations
 
     def add_event_dependency(
             self, dependent_event, independent_events,
             factors=None, transforms=None):
@@ -388,45 +388,45 @@
             raise CADETProcessError(
                 "Cannot find one or more independent events"
             )
 
         for indep in independent_events:
             self.events[dependent_event].remove_dependency(indep)
 
-    @property
+    @cached_property_if_locked
     def independent_events(self):
         """list: All events that are not dependent on other events."""
         return list(filter(lambda evt: evt.is_independent, self.events))
 
-    @property
+    @cached_property_if_locked
     def dependent_events(self):
         """list: All events that are dependent on other events."""
         return list(
             filter(lambda evt: evt.is_independent is False, self.events)
         )
 
-    @property
+    @cached_property_if_locked
     def event_parameters(self):
         """list: Event parameters."""
         return list({evt.parameter_path for evt in self.events})
 
-    @property
+    @cached_property_if_locked
     def event_performers(self):
         """list: Event peformers."""
         return list({evt.performer for evt in self.events})
 
-    @property
+    @cached_property_if_locked
     def event_times(self):
         """list: Time of events, sorted by Event time."""
         event_times = list({evt.time for evt in self.events})
         event_times.sort()
 
         return event_times
 
-    @property
+    @cached_property_if_locked
     def section_times(self):
         """list: Section times.
 
         Includes 0 and cycle_time if they do not coincide with event time.
 
         """
         if len(self.event_times) == 0:
@@ -630,14 +630,17 @@
         from durations, and the cycle time.
         """
         parameters = super().parameters
 
         events = {evt.name: evt.parameters for evt in self.independent_events}
         parameters.update(events)
 
+        events = {evt.name: evt.parameters for evt in self.dependent_events}
+        parameters.update(events)
+
         durations = {dur.name: dur.parameters for dur in self.durations}
         parameters.update(durations)
 
         parameters['cycle_time'] = self.cycle_time
 
         return parameters
 
@@ -650,17 +653,17 @@
             pass
 
         for evt_name, evt_parameters in parameters.items():
             try:
                 evt = self.events_dict[evt_name]
             except AttributeError:
                 raise CADETProcessError('Not a valid event')
-            if evt not in self.independent_events + self.durations:
+            if "time" in evt_parameters and evt not in self.independent_events + self.durations:
                 raise CADETProcessError(
-                    f'{str(evt)} is not a valid event'
+                    f'Cannot set "time" for {str(evt)} because it is not an independent event.'
                 )
 
             evt.parameters = evt_parameters
 
     @property
     def sized_parameters(self):
         """dict: Compilation of parameters from events with indices.
@@ -1282,14 +1285,16 @@
 
                 if any(isinstance(i, slice) for i in ind):
                     if new_slice.size != np.prod(expected_shape):
                         new_slice = np.broadcast_to(new_slice, expected_shape)
                     else:
                         new_slice = np.reshape(new_slice, expected_shape)
 
+                if len(expected_shape) == 0:
+                    new_slice = new_slice.squeeze()
                 new_value[ind] = new_slice
 
             if self.parameter_type is not np.ndarray:
                 new_value = self.parameter_type(new_value.tolist())
 
         # Set the value:
         self.set_value(new_value)
```

### Comparing `CADET-Process-0.8.0/CADETProcess/dynamicEvents/section.py` & `CADET-Process-0.9.0/CADETProcess/dynamicEvents/section.py`

 * *Files 4% similar despite different names*

```diff
@@ -626,23 +626,26 @@
             coeffs = tl.coefficients(end)
 
         return tl
 
 
 def generate_indices(shape, indices=None):
     """
-    Generate indices for indexing a parameter array from a list of indices.
+    Generate tuples representing indices for an array with a given shape.
+
+    This method allows specifying a list of indices where each entry can also contain
+    slices.
 
     Parameters
     ----------
-    parameter : array_like
-        An array which is to be indexed. Scalar parameters are not supported.
-    indices : array_like
-        A 2D array or list of lists, where each inner list is a set of indices
-        into the 'parameter' array. None can be used in place of a full slice (:).
+    shape : tuple of int
+        The shape of the array to be indexed.
+    indices : list of list of int, optional
+        A list where each sub-list contains indices for one dimension of the array.
+        'None' indicates a full slice (':') for that dimension.
 
     Raises
     ------
     ValueError
         If 'parameter' is a scalar or if an index in 'indices' is out of bounds.
 
     Returns
@@ -654,17 +657,16 @@
     Examples
     --------
     >>> parameter = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
     >>> indices = [[0, 1], [1, 2]]
     >>> generate_indices(parameter, indices)
     [(0, 1), (1, 2)]
     """
-    size = np.prod(shape)
-    if size == 1:
-        raise ValueError("Scalar parameters cannot have index slices.")
+    if not shape:
+        raise ValueError("Shape must not be empty, scalar parameters are not supported.")
 
     if indices is None:
         indices = np.s_[:]
 
     if not isinstance(indices, list):
         indices = [indices, ]
 
@@ -778,19 +780,14 @@
         except (ValueError, VisibleDeprecationWarning):
             pass
 
     shape = []
 
     for i in value:
         i_shape = get_inhomogeneous_shape(i)
-        # if len(i_shape) == 0:
-        #     i_shape = (1, )
-
-        # i_shape = (1, ) + i_shape
-
         shape.append(i_shape)
 
     return shape
 
 
 def get_full_shape(inhomogeneous_shape):
     """Create full shape from inhomogeneous shape to be used with numpy arrays."""
```

### Comparing `CADET-Process-0.8.0/CADETProcess/equilibria/__init__.py` & `CADET-Process-0.9.0/CADETProcess/equilibria/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/equilibria/buffer_capacity.py` & `CADET-Process-0.9.0/CADETProcess/equilibria/buffer_capacity.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/equilibria/initial_conditions.py` & `CADET-Process-0.9.0/CADETProcess/equilibria/initial_conditions.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/equilibria/ptc.py` & `CADET-Process-0.9.0/CADETProcess/equilibria/ptc.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/equilibria/reaction_equilibria.py` & `CADET-Process-0.9.0/CADETProcess/equilibria/reaction_equilibria.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/fractionation/fractionationOptimizer.py` & `CADET-Process-0.9.0/CADETProcess/fractionation/fractionationOptimizer.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,17 +51,18 @@
             If no value is specified, a default COBYLA optimizer will be used.
         log_level: {'WARNING', 'INFO', 'DEBUG', 'ERROR'}
             Log level for the fractionation optimization process.
             The default is 'WARNING'.
         """
         if optimizer is None:
             optimizer = COBYLA()
-            optimizer.tol = 0.1
-            optimizer.catol = 1e-4
-            optimizer.rhobeg = 5e-4
+            optimizer.tol = 1e-3
+            optimizer.catol = 5e-3
+            optimizer.rhobeg = 1e-4
+
         self.optimizer = optimizer
         self.log_level = log_level
 
     @property
     def optimizer(self):
         """OptimizerBase: Optimizer for optimizing the fractionation times."""
         return self._optimizer
@@ -120,15 +121,18 @@
             simulation_results,
             components=components,
             use_total_concentration_components=use_total_concentration_components,
         )
 
         frac.initial_values(purity_required)
 
-        if not allow_empty_fractions:
+        if not np.any(frac.n_fractions_per_pool[:-1]):
+            raise CADETProcessError("No areas found with sufficient purity.")
+
+        if not allow_empty_fractions :
             empty_fractions = []
             for i, comp in enumerate(purity_required):
                 if comp > 0:
                     if frac.fraction_pools[i].n_fractions == 0:
                         empty_fractions.append(i)
             if len(empty_fractions) != 0:
                 raise CADETProcessError(
@@ -138,33 +142,45 @@
 
         return frac
 
     def _setup_optimization_problem(
             self,
             frac,
             purity_required,
+            allow_empty_fractions=True,
             ranking=1,
             obj_fun=None,
+            minimize=True,
+            bad_metrics=None,
             n_objectives=1):
         """Set up the OptimizationProblem for optimizing the fractionation times.
 
         Parameters
         ----------
         frac : Fractionator
             The Fractionator object.
         purity_required : list
             Minimum purity required for the components in the fractionation.
-        ranking : {float, list, None}
+        allow_empty_fractions: bool, optional
+            If True, allow empty fractions. The default is True.
+        ranking : list, 1 or None, optional
             Weighting factors for individual components.
-            If float, the same value is used for all components.
+            If 1, the same value is assumed for all components.
             If None, no ranking is used and the problem is solved as multi-objective.
+            The default is 1.
         obj_fun : callable, optional
             Alternative objective function.
             If no function is provided, the fraction mass is maximized.
             The default is None.
+        bad_metrics : float or list of floats, optional
+            Values to be returned if evaluation of objective function failes.
+            The default is 0.
+        minimize : bool, optional
+            If True, the obj_fun is assumed to return a value that is to be minimized.
+            The default it True.
         n_objectives : int
             Number of objectives. The default is 1.
 
         Raises
         ------
         CADETProcessError
             If the optimization problem setup fails.
@@ -172,39 +188,54 @@
         Returns
         -------
         OptimizationProblem
             The configured OptimizationProblem object.
         list
             The initial values for the optimization variables.
         """
+        # Handle empty fractions
+        n_fractions = np.array([pool.n_fractions for pool in frac.fraction_pools])
+        empty_fractions = np.where(n_fractions[0:-1] == 0)[0]
+        if len(empty_fractions) > 0 and allow_empty_fractions:
+            for empty_fraction in empty_fractions:
+                purity_required[empty_fraction] = 0
+
+        # Setup Optimization Problem
         opt = OptimizationProblem(
             'FractionationOptimization',
             log_level=self.log_level,
             use_diskcache=False,
         )
 
         opt.add_evaluation_object(frac)
 
         frac_evaluator = FractionationEvaluator()
-        opt.add_evaluator(frac_evaluator, cache=True)
+        opt.add_evaluator(frac_evaluator)
 
         if obj_fun is None:
             obj_fun = Mass(ranking=ranking)
+            minimize = False
+            bad_metrics = 0
+
         opt.add_objective(
-            obj_fun, requires=frac_evaluator, n_objectives=n_objectives,
-            bad_metrics=0
+            obj_fun,
+            requires=frac_evaluator,
+            n_objectives=n_objectives,
+            minimize=minimize,
+            bad_metrics=bad_metrics,
         )
 
         purity = Purity()
         purity.n_metrics = frac.component_system.n_comp
-        constraint_bounds = -np.array(purity_required, ndmin=1)
-        constraint_bounds = constraint_bounds.tolist()
         opt.add_nonlinear_constraint(
-            purity, n_nonlinear_constraints=len(constraint_bounds),
-            bounds=constraint_bounds, requires=frac_evaluator
+            purity,
+            n_nonlinear_constraints=len(purity_required),
+            bounds=purity_required,
+            comparison_operator='ge',
+            requires=frac_evaluator,
         )
 
         for evt in frac.events:
             opt.add_variable(
                 evt.name, parameter_path=evt.name + '.time',
                 lb=-frac.cycle_time, ub=2*frac.cycle_time,
                 transform='linear'
@@ -235,35 +266,48 @@
             simulation_results,
             purity_required,
             components=None,
             use_total_concentration_components=True,
             ranking=1,
             obj_fun=None,
             n_objectives=1,
+            bad_metrics=0,
+            minimize=True,
             allow_empty_fractions=True,
             ignore_failed=False,
             return_optimization_results=False,
             save_results=False):
         """Optimize the fractionation times with respect to purity constraints.
 
         Parameters
         ----------
         simulation_results : SimulationResults
             Results containing the chromatograms for fractionation.
         purity_required :  float or array_like
             Minimum required purity for components. If is float, the same
             value is assumed for all components.
-        ranking : float or array_like
-            Relative value of components.
+        components : list
+            List of components to consider in the fractionation process.
+        ranking : list, 1 or None, optional
+            Weighting factors for individual components.
+            If 1, the same value is assumed for all components.
+            If None, no ranking is used and the problem is solved as multi-objective.
+            The default is 1.
         obj_fun : function, optional
             Objective function used for OptimizationProblem.
             If COBYLA is used, must return single objective.
             If is None, the mass of all components is maximized.
         n_objectives : int, optional
             Number of objectives returned by obj_fun. The default is 1.
+        bad_metrics : float or list of floats, optional
+            Values to be returned if evaluation of objective function failes.
+            The default is 0.
+        minimize : bool, optional
+            If True, the obj_fun is assumed to return a value that is to be minimized.
+            The default it True.
         allow_empty_fractions: bool, optional
             If True, allow empty fractions. The default is True.
         ignore_failed : bool, optional
             Ignore failed optimization and use initial values.
             The default is False.
         return_optimization_results : bool, optional
             If True, return optimization results.
@@ -317,39 +361,45 @@
             simulation_results,
             purity_required,
             components=components,
             use_total_concentration_components=use_total_concentration_components,
             allow_empty_fractions=allow_empty_fractions
         )
 
+        opt, x0 = self._setup_optimization_problem(
+            frac,
+            purity_required,
+            allow_empty_fractions,
+            ranking,
+            obj_fun,
+            n_objectives,
+            bad_metrics,
+            minimize,
+        )
+
         # Lock to enable caching
         simulation_results.process.lock = True
-
         try:
-            opt, x0 = self._setup_optimization_problem(
-                frac, purity_required, ranking, obj_fun, n_objectives
-            )
             results = self.optimizer.optimize(
                 opt, x0,
                 save_results=save_results,
                 log_level=self.log_level,
                 delete_cache=True,
             )
+            opt.set_variables(results.x[0])
+            frac.reset()
         except CADETProcessError as e:
             if ignore_failed:
                 warnings.warn('Optimization failed. Returning initial values')
                 frac.initial_values(purity_required)
             else:
                 raise CADETProcessError(str(e))
-
-        opt.set_variables(results.x[0])
-        frac.reset()
-
-        # Restore previous lock state
-        simulation_results.process.lock = lock_state
+        finally:
+            # Restore previous lock state
+            simulation_results.process.lock = lock_state
 
         if return_optimization_results:
             return results
         else:
             return frac
 
     evaluate = optimize_fractionation
```

### Comparing `CADET-Process-0.8.0/CADETProcess/fractionation/fractionator.py` & `CADET-Process-0.9.0/CADETProcess/fractionation/fractionator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections import defaultdict
 from functools import wraps
 import os
 
 from addict import Dict
 import numpy as np
 
 from CADETProcess import CADETProcessError
@@ -259,15 +260,15 @@
 
         _,  ax = chromatogram.plot(show=False, ax=ax, *args, **kwargs)
 
         y_max = 1.1*np.max(chromatogram.solution)
 
         fill_regions = []
         for sec in time_line.sections:
-            comp_index = int(np.where(sec.coeffs)[0])
+            comp_index = int(np.where(sec.coeffs)[0].squeeze())
             if comp_index == self.n_comp:
                 color_index = -1
                 text = 'W'
             else:
                 color_index = comp_index
                 text = str(comp_index + 1)
 
@@ -375,15 +376,15 @@
             self._fraction_pools = [
                 FractionPool(self.n_comp) for _ in range(self.n_comp + 1)
             ]
 
             for chrom_index, chrom in enumerate(self.chromatograms):
                 chrom_events = self.chromatogram_events[chrom]
                 for evt_index, evt in enumerate(chrom_events):
-                    target = int(np.nonzero(evt.full_state)[0])
+                    target = np.nonzero(evt.full_state)[0].squeeze()
 
                     frac_start = evt.time
 
                     if evt_index < len(chrom_events) - 1:
                         frac_end = chrom_events[evt_index + 1].time
                         fraction = self._create_fraction(
                             chrom_index, frac_start, frac_end
@@ -556,23 +557,29 @@
 
         Raises
         ------
         CADETProcessError
             If the chromatogram is not found.
 
         """
-        if chromatogram is None and self.n_chromatograms == 1:
+        if chromatogram is None and self.n_chromatograms > 1:
+            raise CADETProcessError(
+                "Missing chromatogram for which the fractionation is added."
+            )
+        elif chromatogram is None and self.n_chromatograms == 1:
             chromatogram = self.chromatograms[0]
-        elif isinstance(chromatogram, str):
+
+        if isinstance(chromatogram, str):
             try:
                 chromatogram = self.chromatograms_dict[f"{chromatogram}"]
             except KeyError:
                 raise CADETProcessError("Could not find chromatogram.")
-        else:
-            raise CADETProcessError("Expected chromatogram.")
+
+        if chromatogram not in self.chromatograms:
+            raise CADETProcessError("Could not find chromatogram.")
 
         param_path = f'fractionation_states.{chromatogram.name}'
         evt = self.add_event(
             event_name, param_path, target, time
         )
         self._chromatogram_events[chromatogram].append(evt)
 
@@ -642,14 +649,29 @@
                             '_end_' + str(index)
                         param_path = f'fractionation_states.{chrom.name}'
                         evt = self.add_event(
                             event_name, param_path, self.n_comp, time
                         )
                         self._chromatogram_events[chrom].append(evt)
 
+        if not self.check_duplicate_events():
+            chrom_events = self._chromatogram_events.copy()
+            for chrom, events in chrom_events.items():
+                events_at_time = defaultdict(list)
+                for event in events:
+                    events_at_time[event.time].append(event)
+
+                for events in events_at_time.values():
+                    if len(events) == 1:
+                        continue
+                    for evt in events:
+                        if evt.state == self.n_comp:
+                            self.remove_event(evt.name)
+                            self._chromatogram_events[chrom].remove(evt)
+
     @property
     def parameters(self):
         parameters = super().parameters
         parameters['fractionation_states'] = {
             chrom.name: self.fractionation_states[chrom]
             for chrom in self.chromatograms
         }
```

### Comparing `CADET-Process-0.8.0/CADETProcess/fractionation/fractions.py` & `CADET-Process-0.9.0/CADETProcess/fractionation/fractions.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/log.py` & `CADET-Process-0.9.0/CADETProcess/log.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/modelBuilder/__init__.py` & `CADET-Process-0.9.0/CADETProcess/modelBuilder/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/modelBuilder/compartmentBuilder.py` & `CADET-Process-0.9.0/CADETProcess/modelBuilder/compartmentBuilder.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/optimization/cache.py` & `CADET-Process-0.9.0/CADETProcess/optimization/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
             self.directory.mkdir(exist_ok=True, parents=True)
 
             self.cache = Cache(
                self.directory.as_posix(),
                disk=DillDisk,
                disk_min_file_size=2**18,    # 256 kb
                size_limit=2**36,            # 64 GB
+               tag_index=True,
             )
             self.directory = self.cache.directory
         else:
             self.cache = {}
 
     def set(self, key, value, tag=None, close=True):
         """Add entry to cache.
@@ -126,15 +127,15 @@
                 raise KeyError(key)
         else:
             self.cache.pop(key)
 
         if close:
             self.close()
 
-    def prune(self, tag='temp'):
+    def prune(self, tag):
         """Remove tagged entries from cache.
 
         Parameters
         ----------
         tag : str, optional
             Tag to be removed. The default is 'temp'.
         """
```

### Comparing `CADET-Process-0.8.0/CADETProcess/optimization/individual.py` & `CADET-Process-0.9.0/CADETProcess/optimization/individual.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,65 +38,79 @@
     ----------
     x : list
         Variable values in untransformed space.
     x_transformed : list
         Independent variable values in transformed space.
     f : list
         Objective values.
+    f_min : list
+        Minimized objective values.
     g : list
         Nonlinear constraint values.
-    m : list
-        Meta score values.
     cv : list
         Nonlinear constraints violation.
     cv_tol : float
         Tolerance for constraints violation.
+    m : list
+        Meta score values.
+    m_min : list
+        Minimized meta score values.
 
     See Also
     --------
     CADETProcess.optimization.Population
     """
 
     x = Vector()
     x_transformed = Vector()
     f = Vector()
+    f_min = Vector()
     g = Vector()
-    m = Vector()
     cv = Vector()
     cv_tol = Float()
+    m = Vector()
+    m_min = Vector()
 
     def __init__(
             self,
             x,
             f=None,
             g=None,
             m=None,
+            x_transformed=None,
+            f_min=None,
             cv=None,
             cv_tol=0,
-            x_transformed=None,
+            m_min=None,
             independent_variable_names=None,
             objective_labels=None,
             contraint_labels=None,
             meta_score_labels=None,
             variable_names=None):
         self.x = x
+        if x_transformed is None:
+            x_transformed = x
+            independent_variable_names = variable_names
+        self.x_transformed = x_transformed
+
         self.f = f
-        self.g = g
-        self.m = m
+        if f_min is None:
+            f_min = f
+        self.f_min = f_min
 
+        self.g = g
         if g is not None and cv is None:
             cv = g
         self.cv = cv
         self.cv_tol = cv_tol
 
-        if x_transformed is None:
-            x_transformed = x
-            independent_variable_names = variable_names
-
-        self.x_transformed = x_transformed
+        self.m = m
+        if m_min is None:
+            m_min = m
+        self.m_min = m_min
 
         if isinstance(variable_names, np.ndarray):
             variable_names = [s.decode() for s in variable_names]
         self.variable_names = variable_names
         if isinstance(independent_variable_names, np.ndarray):
             independent_variable_names = [s.decode() for s in independent_variable_names]
         self.independent_variable_names = independent_variable_names
@@ -109,14 +123,18 @@
         if isinstance(meta_score_labels, np.ndarray):
             meta_score_labels = [s.decode() for s in meta_score_labels]
         self.meta_score_labels = meta_score_labels
 
         self.id = hash_array(self.x)
 
     @property
+    def id_short(self):
+        return self.id[0:7]
+
+    @property
     def is_evaluated(self):
         """bool: Return True if individual has been evaluated. False otherwise."""
         if self.f is None:
             return False
         else:
             return True
 
@@ -154,17 +172,25 @@
         if self.m is None:
             return 0
         else:
             return len(self.m)
 
     @property
     def dimensions(self):
-        """tuple: Individual dimensions (n_x, n_f, n_g)"""
+        """tuple: Individual dimensions (n_x, n_f, n_g, n_m)"""
         return (self.n_x, self.n_f, self.n_g, self.n_m)
 
+    @property
+    def objectives_minimization_factors(self):
+        return self.f_min / self.f
+
+    @property
+    def meta_scores_minimization_factors(self):
+        return self.m_min / self.m
+
     def dominates(self, other):
         """Determine if individual dominates other.
 
         Parameters
         ----------
         other : Individual
             Other individual
@@ -187,16 +213,16 @@
             if np.any(self.cv < other.cv):
                 return True
 
         if self.m is not None:
             self_values = self.m
             other_values = other.m
         else:
-            self_values = self.f
-            other_values = other.f
+            self_values = self.f_min
+            other_values = other.f_min
 
         if np.any(self_values > other_values):
             return False
 
         if np.any(self_values < other_values):
             return True
```

### Comparing `CADET-Process-0.8.0/CADETProcess/optimization/optimizationProblem.py` & `CADET-Process-0.9.0/CADETProcess/optimization/optimizationProblem.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 from CADETProcess.optimization.parallelizationBackend import SequentialBackend
 from CADETProcess.transform import (
     NoTransform, AutoTransform, NormLinearTransform, NormLogTransform
 )
 
 from CADETProcess.metric import MetricBase
-
+from CADETProcess.optimization import Individual, Population
 from CADETProcess.optimization import ResultsCache
 
 
 @frozen_attributes
 class OptimizationProblem(Structure):
     """Class for configuring optimization problems.
 
@@ -107,15 +107,14 @@
         """
         self.name = name
         self.logger = log.get_logger(self.name, level=log_level)
 
         self._evaluation_objects_dict = {}
         self._evaluators = []
 
-        self.cached_evaluators = []
         self.use_diskcache = use_diskcache
         self.cache_directory = cache_directory
         self.setup_cache()
 
         self._variables = []
         self._dependent_variables = []
         self._objectives = []
@@ -126,15 +125,14 @@
         self._multi_criteria_decision_functions = []
         self._callbacks = []
 
     def untransforms(func):
         """Untransform population or individual before calling function."""
         @wraps(func)
         def wrapper(self, x, *args, untransform=False, **kwargs):
-            """Untransform population or individual before calling function."""
             x = np.array(x, ndmin=1)
             if untransform:
                 x = self.untransform(x)
 
             return func(self, x, *args, **kwargs)
 
         return wrapper
@@ -156,14 +154,47 @@
         def wrapper(self, population, *args, **kwargs):
             population = np.array(population, ndmin=2)
 
             return func(self, population, *args, **kwargs)
 
         return wrapper
 
+    def ensures_minimization(scores):
+        """Convert maximization problems to minimization problems."""
+        def wrap(func):
+            @wraps(func)
+            def wrapper(self, *args, ensure_minimization=False, **kwargs):
+                s = func(self, *args, **kwargs)
+
+                if ensure_minimization:
+                    s = self.transform_maximization(s, scores)
+
+                return s
+
+            return wrapper
+        return wrap
+
+    def transform_maximization(self, s, scores):
+        """Transform maximization problems to minimization problems."""
+        factors = []
+        if scores == 'objectives':
+            scores = self.objectives
+        elif scores == 'meta_scores':
+            scores = self.meta_scores
+        else:
+            raise ValueError(f'Unknown scores: {scores}.')
+
+        for score in scores:
+            factor = 1 if score.minimize else -1
+            factors += score.n_total_metrics * [factor]
+
+        s = np.multiply(factors, s)
+
+        return s
+
     @property
     def evaluation_objects(self):
         """list: Objects to be evaluated during optimization.
 
         See Also
         --------
         OptimizatonVariable
@@ -273,19 +304,20 @@
     def variables_dict(self):
         """dict: All optimization variables indexed by variable name."""
         return {var.name: var for var in self.variables}
 
     @property
     def variable_values(self):
         """list: Values of optimization variables."""
-        return [var.value for var in self.variables]
+        return np.array([var.value for var in self.variables])
 
     def add_variable(
             self, name, evaluation_objects=-1, parameter_path=None,
-            lb=-math.inf, ub=math.inf, transform=None, indices=None):
+            lb=-math.inf, ub=math.inf, transform=None, indices=None,
+            pre_processing=None):
         """Add optimization variable to the OptimizationProblem.
 
         The function encapsulates the creation of OptimizationVariable objects
         in order to prevent invalid OptimizationVariables.
 
         Parameters
         ----------
@@ -304,14 +336,17 @@
         ub : float
             Upper bound of the variable value.
         transform : {'auto', 'log', 'linear', None}:
             Variable transform. The default is auto.
         indices : int  or tuple, optional
             Indices for variables that modify entries of a parameter array.
             If None, variable is assumed to be index independent.
+        pre_processing : callable, optional
+            Additional step to process the value before setting it. This function must
+            accept a single argument (the value) and return the processed value.
 
         Raises
         ------
         CADETProcessError
             If the Variable already exists in the dictionary.
 
         See Also
@@ -344,14 +379,15 @@
                 "Cannot set parameter_path for variable without evaluation object "
             )
 
         var = OptimizationVariable(
             name, evaluation_objects, parameter_path,
             lb=lb, ub=ub, transform=transform,
             indices=indices,
+            pre_processing=pre_processing,
         )
 
         self._variables.append(var)
 
         with warnings.catch_warnings():
             warnings.simplefilter('error')  # Treat warnings as errors
 
@@ -521,25 +557,25 @@
 
     @untransforms
     def get_dependent_values(self, x):
         """Determine values of dependent optimization variables.
 
         Parameters
         ----------
-        x : list
+        x : array_like
             Value of the optimization variables in untransformed space.
 
         Raises
         ------
         CADETProcessError
             If length of parameters does not match.
 
         Returns
         -------
-        x : list
+        x : np.ndarray
             Value of all optimization variables in untransformed space.
 
         """
         if len(x) != self.n_independent_variables:
             raise CADETProcessError(
                 f'Expected {self.n_independent_variables} value(s)'
             )
@@ -556,41 +592,41 @@
 
     @untransforms
     def get_independent_values(self, x):
         """Remove dependent values from x.
 
         Parameters
         ----------
-        x : list
+        x : array_like
             Value of all optimization variables.
             Works for transformed and untransformed space.
 
         Raises
         ------
         CADETProcessError
             If length of parameters does not match.
 
         Returns
         -------
-        x_independent : list
+        x_independent : np.ndarray
             Values of all independent optimization variables.
 
         """
         if len(x) != self.n_variables:
             raise CADETProcessError(
-                f'Expected {self.n_variables} value(s)'
+                f'Expected {self.n_variables} value(s), got {len(x)}'
             )
 
         x_independent = []
 
         for variable, value in zip(self.variables, x):
             if variable.is_independent:
                 x_independent.append(value)
 
-        return x_independent
+        return np.array(x_independent)
 
     @untransforms
     def set_variables(self, x, evaluation_objects=-1):
         """Set the values from the x-vector to the EvaluationObjects.
 
         Parameters
         ----------
@@ -638,15 +674,15 @@
         x : array_like
             Value of all optimization variables in untransformed space.
         force : bool
             If True, do not use cached results. The default is False.
 
         Returns
         -------
-        results : list
+        results : np.ndarray
             Values of the evaluation functions at point x.
 
         See Also
         --------
         evaluate_objectives
         evaluate_nonlinear_constraints
         _evaluate
@@ -681,20 +717,20 @@
             If True, do not use cached values. The default is False.
         parallelization_backend : ParallelizationBackendBase, optional
             Adapter to parallelization backend library for parallel evaluation of population.
 
         Raises
         ------
         CADETProcessError
-            DESCRIPTION.
+            If dictcache is used for parallelized evaluation.
 
         Returns
         -------
-        results : list
-            DESCRIPTION.
+        results : np.ndarray
+            Results of the evaluation functions.
 
         """
         if parallelization_backend is None:
             parallelization_backend = SequentialBackend()
 
         if not self.cache.use_diskcache and parallelization_backend.n_cores != 1:
             raise CADETProcessError(
@@ -725,29 +761,30 @@
         func : Evaluator or Objective, or Nonlinear Constraint, or Callback
             Evaluation function.
         force : bool
             If True, do not use cached results. The default is False.
 
         Returns
         -------
-        results : TYPE
-            DESCRIPTION.
+        results : np.ndarray
+            Results of the evaluation functions.
 
         """
         self.logger.debug(f'evaluate {str(func)} at {x}')
 
         results = np.empty((0,))
+        x_key = np.array(x).tobytes()
 
         if func.evaluators is not None:
             requires = [*func.evaluators, func]
         else:
             requires = [func]
 
         self.set_variables(x)
-        evaluation_objects = self.evaluation_objects
+        evaluation_objects = func.evaluation_objects
 
         if len(evaluation_objects) == 0:
             evaluation_objects = [None]
 
         for eval_obj in evaluation_objects:
             self.logger.debug(
                 f"Evaluating {func}. "
@@ -759,15 +796,15 @@
             else:
                 current_request = eval_obj
 
             if not force:
                 remaining = []
                 for step in reversed(requires):
                     try:
-                        key = (str(eval_obj), step.id, str(x))
+                        key = (str(eval_obj), step.id, x_key)
                         result = self.cache.get(key)
                         self.logger.debug(
                             f'Got {str(step)} results from cache.'
                         )
                         current_request = result
                         break
                     except KeyError:
@@ -784,20 +821,18 @@
 
             for step in remaining:
                 if isinstance(step, Callback):
                     step.evaluate(current_request, eval_obj)
                     result = np.empty((0))
                 else:
                     result = step.evaluate(current_request)
-                if step not in self.cached_steps:
-                    tag = 'temp'
-                else:
-                    tag = None
-                key = (str(eval_obj), step.id, str(x))
-                self.cache.set(key, result, tag=tag)
+
+                key = (str(eval_obj), step.id, x_key)
+                if not isinstance(step, Callback):
+                    self.cache.set(key, result, tag=x_key)
                 current_request = result
 
             if len(result) != func.n_metrics:
                 raise CADETProcessError(
                     f"Got results with length {len(result)}. "
                     f"Expected length {func.n_metrics} from {str(func)}"
                 )
@@ -817,28 +852,26 @@
         return {evaluator.evaluator: evaluator for evaluator in self.evaluators}
 
     @property
     def evaluators_dict(self):
         """dict: Evaluator objects indexed by name."""
         return {evaluator.name: evaluator for evaluator in self.evaluators}
 
-    def add_evaluator(self, evaluator, name=None, cache=False, args=None, kwargs=None):
+    def add_evaluator(self, evaluator, name=None, args=None, kwargs=None):
         """Add Evaluator to OptimizationProblem.
 
         Evaluators can be referenced by objective and constraint functions to
         perform preprocessing steps.
 
         Parameters
         ----------
         evaluator : callable
             Evaluation function.
         name : str, optional
             Name of the evaluator.
-        cache : bool, optional
-            If True, results of the evaluator are cached. The default is False.
         args : tuple, optional
             Additional arguments for evaluation function.
         kwargs : dict, optional
             Additional keyword arguments for evaluation function.
 
         Raises
         ------
@@ -864,17 +897,14 @@
             evaluator,
             name,
             args=args,
             kwargs=kwargs,
         )
         self._evaluators.append(evaluator)
 
-        if cache:
-            self.cached_evaluators.append(evaluator)
-
     @property
     def objectives(self):
         """list: Objective functions."""
         return self._objectives
 
     @property
     def objective_names(self):
@@ -889,30 +919,22 @@
             labels += obj.labels
 
         return labels
 
     @property
     def n_objectives(self):
         """int: Number of objectives."""
-        n_objectives = 0
-
-        for objective in self.objectives:
-            if len(objective.evaluation_objects) != 0:
-                factor = len(objective.evaluation_objects)
-            else:
-                factor = 1
-            n_objectives += factor*objective.n_objectives
-
-        return n_objectives
+        return sum([obj.n_total_metrics for obj in self.objectives])
 
     def add_objective(
             self,
             objective,
             name=None,
             n_objectives=1,
+            minimize=True,
             bad_metrics=None,
             evaluation_objects=-1,
             labels=None,
             requires=None,
             *args, **kwargs):
         """Add objective function to optimization problem.
 
@@ -921,14 +943,16 @@
         objective : callable or MetricBase
             Objective function.
         name : str, optional
             Name of the objective.
         n_objectives : int, optional
             Number of metrics returned by objective function.
             The default is 1.
+        minimize : bool, optional
+            If True, objective is treated as minimization problem. The default is True.
         bad_metrics : flot or list of floats, optional
             Value which is returned when evaluation fails.
         evaluation_objects : {EvaluationObject, None, -1, list}
             EvaluationObjects which are evaluated by objective.
             If None, no EvaluationObject is used.
             If -1, all EvaluationObjects are used.
         labels : str, optional
@@ -990,39 +1014,40 @@
             evaluators = [self.evaluators_dict_reference[req] for req in requires]
         except KeyError as e:
             raise CADETProcessError(f"Unknown Evaluator: {str(e)}")
 
         objective = Objective(
             objective,
             name,
-            type='minimize',
             n_objectives=n_objectives,
+            minimize=minimize,
             bad_metrics=bad_metrics,
             evaluation_objects=evaluation_objects,
             evaluators=evaluators,
             labels=labels,
             args=args,
             kwargs=kwargs
         )
         self._objectives.append(objective)
 
     @untransforms
+    @ensures_minimization(scores='objectives')
     def evaluate_objectives(self, x, force=False):
         """Evaluate objective functions at point x.
 
         Parameters
         ----------
         x : array_like
             Value of the optimization variables in untransformed space.
         force : bool
             If True, do not use cached results. The default is False.
 
         Returns
         -------
-        f : list
+        f : np.ndarray
             Values of the objective functions at point x.
 
         See Also
         --------
         add_objective
         evaluate_objectives_population
         _call_evaluate_fun
@@ -1033,30 +1058,36 @@
 
         f = self._evaluate_individual(self.objectives, x, force=force)
 
         return f
 
     @untransforms
     @ensures2d
-    def evaluate_objectives_population(self, population, force=False, parallelization_backend=None):
+    @ensures_minimization(scores='objectives')
+    def evaluate_objectives_population(
+            self,
+            population,
+            force=False,
+            parallelization_backend=None
+            ):
         """Evaluate objective functions for each point x in population.
 
         Parameters
         ----------
         population : list
             Population.
         force : bool, optional
             If True, do not use cached values. The default is False.
         parallelization_backend : RunnerBase, optional
             Runner to use for the evaluation of the population in
             sequential or parallel mode.
 
         Returns
         -------
-        results : list
+        results : np.ndarray
             Objective function values.
 
         See Also
         --------
         add_objective
         evaluate_objectives
         _evaluate_individual
@@ -1065,36 +1096,41 @@
         results = self._evaluate_population(
             self.evaluate_objectives, population, force, parallelization_backend
         )
 
         return results
 
     @untransforms
-    def objective_jacobian(self, x, dx=1e-3):
+    def objective_jacobian(self, x, ensure_minimization=False, dx=1e-3):
         """Compute jacobian of objective functions using finite differences.
 
         Parameters
         ----------
         x : array_like
             Value of the optimization variables in untransformed space.
         dx : float
             Increment to x to use for determining the function gradient.
 
         Returns
         -------
-        jacobian: list
+        jacobian: np.array
             Value of the partial derivatives at point x.
 
         See Also
         --------
         objectives
         approximate_jac
 
         """
-        jacobian = approximate_jac(x, self.evaluate_objectives, dx)
+        jacobian = approximate_jac(
+            x,
+            self.evaluate_objectives,
+            dx,
+            ensure_minimization=ensure_minimization
+        )
 
         return jacobian
 
     @property
     def nonlinear_constraints(self):
         """list: Nonlinear constraint functions."""
         return self._nonlinear_constraints
@@ -1121,33 +1157,27 @@
             bounds += nonlincon.bounds
 
         return bounds
 
     @property
     def n_nonlinear_constraints(self):
         """int: Number of nonlinear_constraints."""
-        n_nonlinear_constraints = 0
-
-        for nonlincon in self.nonlinear_constraints:
-            if len(nonlincon.evaluation_objects) != 0:
-                factor = len(nonlincon.evaluation_objects)
-            else:
-                factor = 1
-            n_nonlinear_constraints += factor*nonlincon.n_nonlinear_constraints
-
-        return n_nonlinear_constraints
+        return sum(
+            [nonlincon.n_total_metrics for nonlincon in self.nonlinear_constraints]
+        )
 
     def add_nonlinear_constraint(
             self,
             nonlincon,
             name=None,
             n_nonlinear_constraints=1,
             bad_metrics=None,
             evaluation_objects=-1,
             bounds=0,
+            comparison_operator='le',
             labels=None,
             requires=None,
             *args, **kwargs):
         """Add nonliner constraint function to optimization problem.
 
         Parameters
         ----------
@@ -1164,14 +1194,18 @@
             EvaluationObjects which are evaluated by objective.
             If None, no EvaluationObject is used.
             If -1, all EvaluationObjects are used.
         bounds : scalar or list of scalars, optional
             Upper limits of constraint function.
             If only one value is given, the same value is assumed for all
             constraints. The default is 0.
+        comparison_operator : {'ge', 'le'}, optional
+            Comparator to define whether metric should be greater or equal to, or less
+            than or equal to the specified bounds.
+            The default is 'le' (lower or equal).
         labels : str, optional
             Names of the individual metrics.
         requires : {None, Evaluator, list}, optional
             Evaluators used for preprocessing.
             If None, no preprocessing is required.
             The default is None.
         args : tuple, optional
@@ -1235,16 +1269,17 @@
             evaluators = [self.evaluators_dict_reference[req]for req in requires]
         except KeyError as e:
             raise CADETProcessError(f"Unknown Evaluator: {str(e)}")
 
         nonlincon = NonlinearConstraint(
             nonlincon,
             name,
-            bounds=bounds,
             n_nonlinear_constraints=n_nonlinear_constraints,
+            bounds=bounds,
+            comparison_operator=comparison_operator,
             bad_metrics=bad_metrics,
             evaluation_objects=evaluation_objects,
             evaluators=evaluators,
             labels=labels,
             args=args,
             kwargs=kwargs
         )
@@ -1259,15 +1294,15 @@
         x : array_like
             Value of the optimization variables in untransformed space.
         force : bool
             If True, do not use cached results. The default is False.
 
         Returns
         -------
-        g : list
+        g : np.ndarray
             Nonlinear constraint function values.
 
         See Also
         --------
         add_nonlinear_constraint
         evaluate_nonlinear_constraints_violation
         evaluate_nonlinear_constraints_population
@@ -1295,15 +1330,15 @@
             If True, do not use cached values. The default is False.
         parallelization_backend : RunnerBase, optional
             Runner to use for the evaluation of the population in
             sequential or parallel mode.
 
         Returns
         -------
-        results : list
+        results : np.ndarray
             Nonlinear constraints.
 
         See Also
         --------
         add_nonlinear_constraint
         evaluate_nonlinear_constraints
         _evaluate_individual
@@ -1342,16 +1377,25 @@
         evaluate_nonlinear_constraints_violation_population
         _call_evaluate_fun
         _evaluate
 
         """
         self.logger.debug(f'Evaluate nonlinear constraints violation at {x}.')
 
+        factors = []
+        for constr in self.nonlinear_constraints:
+            factor = -1 if constr.comparison_operator == 'ge' else 1
+            factors += constr.n_total_metrics * [factor]
+
         g = self._evaluate_individual(self.nonlinear_constraints, x, force=False)
-        cv = np.array(g) - np.array(self.nonlinear_constraints_bounds)
+        g_transformed = np.multiply(factors, g)
+
+        bounds_transformed = np.multiply(factors, self.nonlinear_constraints_bounds)
+
+        cv = g_transformed - bounds_transformed
 
         return cv
 
     @untransforms
     @ensures2d
     def evaluate_nonlinear_constraints_violation_population(
             self, population, force=False, parallelization_backend=None):
@@ -1369,15 +1413,15 @@
             If True, do not use cached values. The default is False.
         parallelization_backend : RunnerBase, optional
             Runner to use for the evaluation of the population in
             sequential or parallel mode.
 
         Returns
         -------
-        results : list
+        results : np.ndarray
             Nonlinear constraints violation.
 
         See Also
         --------
         add_nonlinear_constraint
         evaluate_nonlinear_constraints_violation
         evaluate_nonlinear_constraints
@@ -1581,15 +1625,15 @@
                     current_iteration % callback.frequency == 0):
                 continue
 
             callback._ind = ind
             callback._current_iteration = current_iteration
 
             try:
-                self._evaluate(ind.x, callback, force)
+                self._evaluate(ind.x_transformed, callback, force, untransform=True)
             except CADETProcessError:
                 self.logger.warning(
                     f'Evaluation of {callback} failed at {ind.x}.'
                 )
 
     def evaluate_callbacks_population(
             self, population, current_iteration, force=False, parallelization_backend=None):
@@ -1603,19 +1647,14 @@
             Current iteration step.
         force : bool, optional
             If True, do not use cached values. The default is False.
         parallelization_backend : RunnerBase, optional
             Runner to use for the evaluation of the population in
             sequential or parallel mode.
 
-        Returns
-        -------
-        results : list
-            Nonlinear constraint function values.
-
         See Also
         --------
         add_callback
         evaluate_callbacks
         """
         if parallelization_backend is None:
             parallelization_backend = SequentialBackend()
@@ -1653,43 +1692,37 @@
             labels += meta_score.labels
 
         return labels
 
     @property
     def n_meta_scores(self):
         """int: Number of meta score functions."""
-        n_meta_scores = 0
-
-        for meta_score in self.meta_scores:
-            if len(meta_score.evaluation_objects) != 0:
-                factor = len(meta_score.evaluation_objects)
-            else:
-                factor = 1
-            n_meta_scores += factor*meta_score.n_meta_scores
-
-        return n_meta_scores
+        return sum([meta_score.n_total_metrics for meta_score in self.meta_scores])
 
     def add_meta_score(
             self,
             meta_score,
             name=None,
             n_meta_scores=1,
+            minimize=True,
             evaluation_objects=-1,
             requires=None):
         """Add Meta score to the OptimizationProblem.
 
         Parameters
         ----------
         meta_score : callable
             Objective function.
         name : str, optional
             Name of the meta score.
         n_meta_scores : int, optional
             Number of meta scores returned by callable.
             The default is 1.
+        minimize : bool, optional
+            If True, meta score is treated as minimization problem. The default is True.
         evaluation_objects : {EvaluationObject, None, -1, list}
             EvaluationObjects which are evaluated by objective.
             If None, no EvaluationObject is used.
             If -1, all EvaluationObjects are used.
         requires : {None, Evaluator, list}
             Evaluators used for preprocessing.
             If None, no preprocessing is required.
@@ -1747,27 +1780,28 @@
             n_meta_scores=n_meta_scores,
             evaluation_objects=evaluation_objects,
             evaluators=evaluators,
         )
         self._meta_scores.append(meta_score)
 
     @untransforms
+    @ensures_minimization(scores='meta_scores')
     def evaluate_meta_scores(self, x, force=False):
         """Evaluate meta functions at point x.
 
         Parameters
         ----------
         x : array_like
             Value of the optimization variables in untransformed space.
         force : bool
             If True, do not use cached results. The default is False.
 
         Returns
         -------
-        m : list
+        m : np.ndarray
             Meta scores.
 
         See Also
         --------
         add_meta_score
         evaluate_nonlinear_constraints_population
         _call_evaluate_fun
@@ -1777,29 +1811,30 @@
 
         m = self._evaluate_individual(self.meta_scores, x, force=force)
 
         return m
 
     @untransforms
     @ensures2d
+    @ensures_minimization(scores='meta_scores')
     def evaluate_meta_scores_population(self, population, force=False, parallelization_backend=None):
         """Evaluate meta score functions for each point x in population.
 
         Parameters
         ----------
         population : list
             Population.
         force : bool, optional
             If True, do not use cached values. The default is False.
         parallelization_backend : RunnerBase, optional
             Runner to use for the evaluation of the population in
             sequential or parallel mode.
         Returns
         -------
-        results : list
+        results : np.ndarray
             Meta scores.
 
         See Also
         --------
         add_meta_score
         evaluate_meta_scores
         _evaluate_individual
@@ -1873,15 +1908,15 @@
         Parameters
         ----------
         pareto_population : Population
             Pareto optimal solution
 
         Returns
         -------
-        x_pareto : list
+        x_pareto : np.ndarray
             Value of the optimization variables.
 
         See Also
         --------
         add_multi_criteria_decision_function
         add_multi_criteria_decision_function
         """
@@ -2125,15 +2160,15 @@
         A_t = self.A.copy()
         for a in A_t:
             for j, v in enumerate(self.variables):
                 t = v.transform
                 if isinstance(t, NoTransform):
                     continue
 
-                if not t.is_linear:
+                if a[j] != 0 and not t.is_linear:
                     raise CADETProcessError(
                         "Non-linear transform was used in linear constraints."
                     )
 
                 scale = (t.ub_input - t.lb_input) / (t.ub - t.lb)
                 # this is fine, because it will squish more when the bounds are
                 # larger prior to transformation
@@ -2205,15 +2240,15 @@
         A_t = self.A.copy()
         for i, a in enumerate(A_t):
             for j, v in enumerate(self.variables):
                 t = v.transform
                 if isinstance(t, NoTransform):
                     continue
 
-                if not t.is_linear:
+                if a[j] != 0 and not t.is_linear:
                     raise CADETProcessError(
                         "Non-linear transform was used in linear constraints."
                     )
                 # I realize: This sounds an awful lot like transforms that sklear offers
                 # center and scale
 
                 # FUTURE: move to transforms module
@@ -2237,15 +2272,15 @@
         Parameters
         ----------
         x : array_like
             Value of the optimization variables in untransformed space.
 
         Returns
         -------
-        constraints: np.array
+        constraints: np.ndarray
             Value of the linear constraints at point x
 
         See Also
         --------
         A
         b
         linear_constraints
@@ -2402,29 +2437,42 @@
         Aeq_t = self.Aeq.copy()
         for aeq in Aeq_t:
             for j, v in enumerate(self.variables):
                 t = v.transform
                 if isinstance(t, NoTransform):
                     continue
 
-                if not t.is_linear:
+                if aeq[j] != 0 and not t.is_linear:
                     raise CADETProcessError(
                         "Non-linear transform was used in linear constraints."
                     )
 
                 scale = (t.ub_input - t.lb_input) / (t.ub - t.lb)
                 # this is fine, because it will squish more when the bounds are
                 # larger prior to transformation
                 # FUTURE: move to transforms module
                 # *= (range old bounds) / (range new bounds)
                 aeq[j] *= scale
 
         return Aeq_t
 
     @property
+    def Aeq_independent(self):
+        """np.ndarray: LHS Matrix of linear inequality constraints for indep variables.
+
+        See Also
+        --------
+        Aeq
+        Aeq_transformed
+        Aeq_independent_transformed
+
+        """
+        return self.Aeq[:, self.independent_variable_indices]
+
+    @property
     def Aeq_independent_transformed(self):
         """np.ndarray: LHS of lin ineqs for indep variables in transformed space.
 
         See Also
         --------
         Aeq
         Aeq_transformed
@@ -2469,15 +2517,15 @@
         Aeq_t = self.Aeq.copy()
         for i, aeq in enumerate(Aeq_t):
             for j, v in enumerate(self.variables):
                 t = v.transform
                 if isinstance(t, NoTransform):
                     continue
 
-                if not t.is_linear:
+                if aeq[j] != 0 and not t.is_linear:
                     raise CADETProcessError(
                         "Non-linear transform was used in linear constraints."
                     )
                 # I realize: This sounds an awful lot like transforms that sklear offers
                 # center and scale
 
                 # FUTURE: move to transforms module
@@ -2551,71 +2599,71 @@
 
         lhs = self.evaluate_linear_equality_constraints(x)
         if np.any(np.abs(lhs) >= self.eps_eq):
             flag = False
 
         return flag
 
-    def transform(self, x):
-        """Transform the optimization variables from untransformed parameter space.
+    def transform(self, x_independent):
+        """Transform the independent optimization variables from untransformed parameter space.
 
         Parameters
         ----------
-        x : list
-            Value of the optimization variables in untransformed space.
+        x_independent : list
+            Value of the independent optimization variables in untransformed space.
 
         Returns
         -------
-        list
+        np.ndarray
             Optimization variables in transformed parameter space.
         """
-        x = np.array(x)
-        x_2d = np.array(x, ndmin=2)
+        x_independent = np.array(x_independent)
+        x_2d = np.array(x_independent, ndmin=2)
         transform = np.zeros(x_2d.shape)
 
         for i, ind in enumerate(x_2d):
             transform[i, :] = [
                 var.transform_fun(value)
                 for value, var in zip(ind, self.independent_variables)
             ]
 
-        return transform.reshape(x.shape).tolist()
+        return transform.reshape(x_independent.shape)
 
     def untransform(self, x_transformed):
         """Untransform the optimization variables from transformed parameter space.
 
         Parameters
         ----------
         x_transformed : list
             Optimization variables in transformed parameter space.
 
         Returns
         -------
-        list
+        np.ndarray
             Optimization variables in untransformed parameter space.
         """
         x_transformed = np.array(x_transformed)
         x_transformed_2d = np.array(x_transformed, ndmin=2)
         untransform = np.zeros(x_transformed_2d.shape)
 
         for i, ind in enumerate(x_transformed_2d):
             untransform[i, :] = [
                 var.untransform_fun(value)
                 for value, var in zip(ind, self.independent_variables)
             ]
 
-        return untransform.reshape(x_transformed.shape).tolist()
+        return untransform.reshape(x_transformed.shape)
 
     @property
     def cached_steps(self):
         """list: Cached evaluation steps."""
         return \
-            self.cached_evaluators + \
             self.objectives + \
-            self.nonlinear_constraints
+            self.nonlinear_constraints + \
+            self.meta_scores
 
     @property
     def cache_directory(self):
         """pathlib.Path: Path for results cache database."""
         if self._cache_directory is None:
             _cache_directory = settings.working_directory / f'diskcache_{self.name}'
         else:
@@ -2639,172 +2687,285 @@
         try:
             self.cache.delete_database()
         except AttributeError:
             pass
         if reinit:
             self.setup_cache()
 
-    def prune_cache(self):
+    def prune_cache(self, tag=None):
         """Prune cache with (intermediate) results."""
-        self.cache.prune()
+        self.cache.prune(tag)
+
+    def create_hopsy_problem(
+            self,
+            include_dependent_variables=True,
+            simplify=False,
+            use_custom_model=False
+            ):
+        """Creates a hopsy problem from the optimization problem.
+
+        Parameters
+        ----------
+        include_dependent_variables : bool, optional
+            If True, only use the hopsy problem. The default is False.
+        simplify : bool, optional
+            If True, simplify the hopsy problem. The default is False.
+        use_custom_model : bool, optional
+            If True, use custom model to improve sampling of log normalized parameters.
+            The default is False.
+
+        Returns
+        -------
+        problem
+            hopsy.Problem
+
+        """
+        class CustomModel():
+            def __init__(self, log_space_indices: list):
+                self.log_space_indices = log_space_indices
+
+            def compute_negative_log_likelihood(self, x):
+                return np.sum(np.log(x[self.log_space_indices]))
+
+        if include_dependent_variables:
+            variables = self.variables
+        else:
+            variables = self.independent_variables
+
+        log_space_indices = []
+
+        for i, var in enumerate(variables):
+            if (
+                    isinstance(var._transform, NormLogTransform)
+                    or
+                    (
+                        isinstance(var._transform, AutoTransform) and
+                        var._transform.use_log
+                    )
+            ):
+                log_space_indices.append(i)
+
+        lp = hopsy.LP()
+        lp.reset()
+        lp.settings.thresh = 1e-15
+
+        if len(log_space_indices) and use_custom_model > 0:
+            model = CustomModel(log_space_indices)
+        else:
+            model = None
+
+        if include_dependent_variables:
+            A = self.A
+            b = self.b
+            lower_bounds = self.lower_bounds
+            upper_bounds = self.upper_bounds
+            Aeq = self.Aeq
+            beq = self.beq
+        else:
+            A = self.A_independent
+            b = self.b
+            lower_bounds = self.lower_bounds_independent
+            upper_bounds = self.upper_bounds_independent
+            Aeq = self.Aeq_independent
+            beq = self.beq
+
+        problem = hopsy.Problem(
+            A,
+            b,
+            model,
+        )
+
+        problem = hopsy.add_box_constraints(
+            problem,
+            lower_bounds,
+            upper_bounds,
+            simplify=simplify,
+        )
+
+        if self.n_linear_equality_constraints > 0:
+            problem = hopsy.add_equality_constraints(
+                problem,
+                Aeq,
+                beq
+            )
+
+        return problem
+
+    def get_chebyshev_center(self, include_dependent_variables=True):
+        """Compute chebychev center.
+
+        The Chebyshev center is the center of the largest Euclidean ball that is fully
+        contained within the polytope of the parameter space.
+
+        Parameters
+        ----------
+        include_dependent_variables : bool, optional
+            If True, include dependent variables in population.
+
+        Returns
+        -------
+        chebyshev : list
+            Chebyshev center.
+        """
+        problem = self.create_hopsy_problem(
+            include_dependent_variables=False, simplify=False, use_custom_model=True
+        )
+        # !!! Additional checks in place to handle PolyRound.round()
+        # removing "small" dimensions.
+        # Bug reported, Check for future release!
+        chebyshev_orig = hopsy.compute_chebyshev_center(
+            problem, original_space=True
+        )[:, 0]
+
+        try:
+            problem_rounded = hopsy.round(problem)
+        except ValueError:
+            problem_rounded = problem
+
+        if problem_rounded.A.shape[1] == problem.A.shape[1]:
+            chebyshev_rounded = hopsy.compute_chebyshev_center(
+                problem_rounded, original_space=True
+            )[:, 0]
+
+            if np.all(np.greater(chebyshev_rounded, self.lower_bounds_independent)):
+                problem = problem_rounded
+                chebyshev = chebyshev_rounded
+            else:
+                chebyshev = chebyshev_orig
+        else:
+            chebyshev = chebyshev_orig
+
+        if include_dependent_variables:
+            chebyshev = self.get_dependent_values(chebyshev)
+
+        return chebyshev
 
     def create_initial_values(
-            self, n_samples=1, method='random', seed=None, burn_in=100000):
+            self, n_samples=1, seed=None, burn_in=100000,
+            include_dependent_variables=True):
         """Create initial value within parameter space.
 
         Uses hopsy (Highly Optimized toolbox for Polytope Sampling) to retrieve
         uniformly distributed samples from the parameter space.
 
         Parameters
         ----------
         n_samples : int
             Number of initial values to be drawn
-        method : str, optional
-            chebyshev: Return center of the minimal-radius ball enclosing the entire set .
-            random: Any random valid point in the parameter space.
         seed : int, optional
             Seed to initialize random numbers. Only used if method == 'random'
-        burn_in: int, optional
+        burn_in : int, optional
             Number of samples that are created to ensure uniform sampling.
             The actual initial values are then drawn from this set.
             The default is 100000.
+        include_dependent_variables : bool, optional
+            If True, include dependent variables in population.
+            The default is True.
 
         Raises
         ------
         CADETProcessError
             If method is not known.
 
         Returns
         -------
         values : list
             Initial values for starting the optimization.
 
         """
         burn_in = int(burn_in)
 
-        class CustomModel():
-            def __init__(self, log_space_indices: list):
-                self.log_space_indices = log_space_indices
-
-            def compute_negative_log_likelihood(self, x):
-                return np.sum(np.log(x[self.log_space_indices]))
-
-        log_space_indices = []
-        for i, var in enumerate(self.variables):
-            if (
-                    isinstance(var._transform, NormLogTransform)
-                    or
-                    (
-                        isinstance(var._transform, AutoTransform) and
-                        var._transform.use_log
-                    )
-            ):
-                log_space_indices.append(i)
-
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
 
-            lp = hopsy.LP()
-            lp.reset()
-            lp.settings.thresh = 1e-15
-
-            if len(log_space_indices) > 0:
-                model = CustomModel(log_space_indices)
-            else:
-                model = None
-
-            problem = hopsy.Problem(
-                self.A,
-                self.b,
-                model,
+            problem = self.create_hopsy_problem(
+                include_dependent_variables=False,
+                simplify=False,
+                use_custom_model=True,
             )
 
-            problem = hopsy.add_box_constraints(
-                problem,
-                self.lower_bounds,
-                self.upper_bounds,
-                simplify=False,
+            chebychev_center = self.get_chebyshev_center(
+                include_dependent_variables=False
             )
 
-            # !!! Additional checks in place to handle PolyRound.round()
-            # removing "small" dimensions.
-            # Bug reported, Check for future release!
-            chebyshev_orig = hopsy.compute_chebyshev_center(problem)[:, 0]
+            if seed is None:
+                seed = random.randint(0, 255)
 
-            try:
-                problem_rounded = hopsy.round(problem)
-            except ValueError:
-                problem_rounded = problem
-
-            if problem_rounded.A.shape[1] == problem.A.shape[1]:
-                chebyshev_rounded = hopsy.compute_chebyshev_center(problem_rounded)[:, 0]
-
-                if np.all(np.greater(chebyshev_rounded, self.lower_bounds)):
-                    problem = problem_rounded
-                    chebyshev = chebyshev_rounded
-                else:
-                    chebyshev = chebyshev_orig
+            rng = np.random.default_rng(seed)
 
-            if n_samples == 1 and method == 'chebyshev':
-                values = np.array(chebyshev_orig, ndmin=2)
-            else:
-                if seed is None:
-                    seed = random.randint(0, 255)
+            mc = hopsy.MarkovChain(
+                problem,
+                proposal=hopsy.UniformCoordinateHitAndRunProposal,
+                starting_point=chebychev_center
+            )
+            rng_hopsy = hopsy.RandomNumberGenerator(seed=seed)
 
-                rng = np.random.default_rng(seed)
+            acceptance_rate, states = hopsy.sample(
+                mc, rng_hopsy, n_samples=burn_in, thinning=2
+            )
+            independent_values = states[0, ...]
 
-                mc = hopsy.MarkovChain(
-                    problem,
-                    proposal=hopsy.UniformCoordinateHitAndRunProposal,
-                    starting_point=chebyshev
+        values = []
+        counter = 0
+        while len(values) < n_samples:
+            if counter > burn_in:
+                raise CADETProcessError(
+                    "Cannot find individuals that fulfill constraints."
                 )
-                rng_hopsy = hopsy.RandomNumberGenerator(seed=seed)
 
-                acceptance_rate, states = hopsy.sample(
-                    mc, rng_hopsy, n_samples=burn_in, thinning=2
+            counter += 1
+            i = rng.integers(0, burn_in)
+            ind = []
+            for i_var, var in enumerate(self.independent_variables):
+                ind.append(
+                    float(np.format_float_positional(
+                        independent_values[i, i_var],
+                        precision=var.precision, fractional=False
+                    ))
                 )
-                values = states[0, ...]
 
-        independent_indices = [
-            i for i, variable in enumerate(self.variables)
-            if variable in self.independent_variables
-        ]
-        independent_values = values[:, independent_indices]
+            ind = self.get_dependent_values(ind)
 
-        if n_samples == 1 and method == 'chebyshev':
-            values = independent_values
-        else:
-            values = []
-            counter = 0
-            while len(values) < n_samples:
-                if counter > burn_in:
-                    raise CADETProcessError(
-                        "Cannot find invididuals that fulfill constraints."
-                    )
+            if not self.check_individual(ind, silent=True):
+                continue
 
-                counter += 1
-                i = rng.integers(0, burn_in)
-                ind = []
-                for i_var, var in enumerate(self.independent_variables):
-                    ind.append(
-                        float(np.format_float_positional(
-                            independent_values[i, i_var],
-                            precision=var.precision, fractional=False
-                        ))
-                    )
+            if not include_dependent_variables:
+                ind = self.get_independent_values(ind)
 
-                if not self.check_bounds(ind, get_dependent_values=True):
-                    continue
-                if not self.check_linear_constraints(ind, get_dependent_values=True):
-                    continue
-                if not self.check_linear_equality_constraints(ind, get_dependent_values=True):
-                    continue
-                values.append(ind)
+            values.append(ind)
+
+        return np.array(values, ndmin=2)
+
+    @untransforms
+    @gets_dependent_values
+    def create_individual(
+            self,
+            x,
+            f=None,
+            g=None,
+            m=None,
+            x_transformed=None,
+            f_min=None,
+            cv=None,
+            cv_tol=None,
+            m_min=None,
+            ):
+        x_indep = self.get_independent_values(x)
+        x_transformed = self.transform(x_indep)
 
-        return np.array(values)
+        ind = Individual(
+            x, f, g, m, x_transformed, f_min, cv, cv_tol, m_min,
+            self.independent_variable_names,
+            self.objective_labels,
+            self.nonlinear_constraint_labels,
+            self.meta_score_labels,
+            self.variable_names,
+        )
+
+        return ind
 
     @property
     def parameters(self):
         parameters = Dict()
 
         parameters.variables = {
             opt.name: opt.parameters for opt in self.variables
@@ -2893,24 +3054,58 @@
             flag = False
 
         if not self.check_duplicate_variables():
             flag = False
 
         if self.n_objectives == 0:
             flag = False
+
         if self.n_linear_constraints + self.n_linear_equality_constraints > 0 \
                 and not ignore_linear_constraints:
             if not self.check_linear_constraints_transforms():
                 flag = False
 
             if not self.check_linear_constraints_dependency():
                 flag = False
 
         return flag
 
+    @untransforms
+    @gets_dependent_values
+    def check_individual(self, x, silent=False):
+        """Check if individual is valid.
+
+        Parameters
+        ----------
+        x : array_like
+            Value of the optimization variables in untransformed space.
+
+        Returns
+        -------
+        bool
+            True if the individual is valid correctly, False otherwise.
+
+        """
+        flag = True
+
+        if not self.check_bounds(x):
+            if not silent:
+                warnings.warn("Individual does not satisfy bounds.")
+            flag = False
+        if not self.check_linear_constraints(x):
+            if not silent:
+                warnings.warn("Individual does not satisfy linear constraints.")
+            flag = False
+        if not self.check_linear_equality_constraints(x):
+            if not silent:
+                warnings.warn("Individual does not satisfy linear equality constraints.")
+            flag = False
+
+        return flag
+
     def __str__(self):
         return self.name
 
 
 class OptimizationVariable:
     """Class for setting the values for the optimization variables.
 
@@ -2934,26 +3129,30 @@
         Transformation function for parameter normalization.
     indices : int, or slice
         Indices for variables that modify an entry of a parameter array.
         If None, variable is assumed to be index independent.
     precision : int, optional
         Number of significant figures to which variable can be rounded.
         If None, variable is not rounded. The default is None.
+    pre_processing : callable, optional
+        Additional step to process the value before setting it. This function must
+        accept a single argument (the value) and return the processed value.
 
     Raises
     ------
     CADETProcessError
         If the attribute is not valid.
     ValueError
         If the lower bound is larger than or equal to the upper bound.
     """
 
     def __init__(
         self, name, evaluation_objects=None, parameter_path=None,
         lb=-math.inf, ub=math.inf, transform=None, indices=None, precision=None,
+        pre_processing=None
     ):
         self.name = name
         self._value = None
 
         if evaluation_objects is not None:
             if not isinstance(evaluation_objects, list):
                 evaluation_objects = [evaluation_objects]
@@ -2986,14 +3185,16 @@
 
         self._transform = transform
         self.precision = precision
 
         self._dependencies = []
         self._dependency_transform = None
 
+        self.pre_processing = pre_processing
+
     @property
     def parameter_path(self):
         """str: Path of the evaluation_object parameter in dot notation."""
         return self._parameter_path
 
     @parameter_path.setter
     def parameter_path(self, parameter_path):
@@ -3345,14 +3546,16 @@
                     new_value = parameter_type(new_value.tolist())
 
             # Set the value:
             self._set_value(eval_obj, new_value)
 
     def _set_value(self, evaluation_object, value):
         """Set the value to the evaluation object."""
+        if self.pre_processing is not None:
+            value = self.pre_processing(value)
         parameter_descriptor = self._parameter_descriptor(evaluation_object)
         if parameter_descriptor is not None:
             performer_obj = self._performer_obj(evaluation_object)
             setattr(performer_obj, self.parameter_sequence[-1], value)
         else:
             parameters = generate_nested_dict(self.parameter_sequence, value)
             evaluation_object.parameters = parameters
@@ -3415,196 +3618,160 @@
 
     evaluate = __call__
 
     def __str__(self):
         return self.name
 
 
-class Objective(Structure):
-    """Wrapper class to evaluate objective functions."""
+class Metric(Structure):
+    """Wrapper class to evaluate metrics (e.g. objective/nonlincon) functions."""
 
-    objective = Callable()
+    func = Callable()
     name = String()
-    # TODO: umbennennen
-    type = Switch(valid=['minimize', 'maximize'])
-    n_objectives = RangedInteger(lb=1)
-    n_metrics = n_objectives
+    n_metrics = RangedInteger(lb=1)
     bad_metrics = SizedNdArray(size='n_metrics', default=np.inf)
 
     def __init__(
             self,
-            objective,
+            func,
             name,
-            type='minimize',
-            n_objectives=1,
+            n_metrics=1,
             bad_metrics=np.inf,
             evaluation_objects=None,
             evaluators=None,
             labels=None,
             args=None,
             kwargs=None):
 
-        self.objective = objective
+        self.func = func
         self.name = name
 
-        self.type = type
-        self.n_objectives = n_objectives
+        self.n_metrics = n_metrics
 
         if np.isscalar(bad_metrics):
-            bad_metrics = np.tile(bad_metrics, n_objectives)
+            bad_metrics = np.tile(bad_metrics, n_metrics)
         self.bad_metrics = bad_metrics
 
         self.evaluation_objects = evaluation_objects
         self.evaluators = evaluators
 
         self.labels = labels
 
         self.args = args
         self.kwargs = kwargs
 
         self.id = uuid.uuid4()
 
     @property
+    def n_total_metrics(self):
+        """int: Total number of objectives."""
+        n_eval_objects = len(self.evaluation_objects) if self.evaluation_objects else 1
+        return n_eval_objects * self.n_metrics
+
+    @property
     def labels(self):
         """list: List of metric labels."""
         if self._labels is not None:
             return self._labels
 
         try:
-            labels = self.objective.labels
+            labels = self.func.labels
         except AttributeError:
             labels = [f'{self.name}']
             if self.n_metrics > 1:
                 labels = [
                     f'{self.name}_{i}'
                     for i in range(self.n_metrics)
                 ]
+
+        if len(self.evaluation_objects) > 1:
+            labels = [
+                f"{eval_obj}_{label}"
+                for label in labels
+                for eval_obj in self.evaluation_objects
+            ]
         return labels
 
     @labels.setter
     def labels(self, labels):
         if labels is not None:
 
             if len(labels) != self.n_metrics:
                 raise CADETProcessError(
                     f"Expected {self.n_metrics} labels."
                 )
 
         self._labels = labels
 
     def __call__(self, request):
+        """
+        Evaluate the metric function with the given request and predefined arguments.
+
+        Parameters
+        ----------
+        request
+            The input to the metric function, typically representing the current state
+            or results of intermediate steps in the optimization process.
+
+        Returns
+        -------
+        ndarray
+            The evaluated metric values, returned as a NumPy array.
+        """
         if self.args is None:
             args = ()
         else:
             args = self.args
 
         if self.kwargs is None:
             kwargs = {}
         else:
             kwargs = self.kwargs
 
-        f = self.objective(request, *args, **kwargs)
+        f = self.func(request, *args, **kwargs)
 
         return np.array(f, ndmin=1)
 
     evaluate = __call__
 
     def __str__(self):
         return self.name
 
 
-class NonlinearConstraint(Structure):
+class Objective(Metric):
+    """Wrapper class to evaluate objective functions."""
+    objective = Metric.func
+    n_objectives = Metric.n_metrics
+    minimize = Bool(default=True)
+
+    def __init__(self, *args, n_objectives=1, minimize=True, **kwargs):
+        self.minimize = minimize
+
+        super().__init__(*args, n_metrics=n_objectives, **kwargs)
+
+
+class NonlinearConstraint(Metric):
     """Wrapper class to evaluate nonlinear constraint functions."""
 
-    nonlinear_constraint = Callable()
-    name = String()
-    n_nonlinear_constraints = RangedInteger(lb=1)
-    n_metrics = n_nonlinear_constraints
-    bad_metrics = SizedNdArray(size='n_metrics', default=np.inf)
+    nonlinear_constraint = Metric.func
+    n_nonlinear_constraints = Metric.n_metrics
+    comparison_operator = Switch(valid=['le', 'ge'], default='le')
 
     def __init__(
             self,
-            nonlinear_constraint,
-            name,
-            bounds=0,
+            *args,
             n_nonlinear_constraints=1,
-            bad_metrics=np.inf,
-            evaluation_objects=None,
-            evaluators=None,
-            labels=None,
-            args=None,
-            kwargs=None):
-
-        self.nonlinear_constraint = nonlinear_constraint
-        self.name = name
-
+            bounds=0,
+            comparison_operator='le',
+            **kwargs
+            ):
         self.bounds = bounds
-        self.n_nonlinear_constraints = n_nonlinear_constraints
-
-        if np.isscalar(bad_metrics):
-            bad_metrics = np.tile(bad_metrics, n_nonlinear_constraints)
-        self.bad_metrics = bad_metrics
-
-        self.evaluation_objects = evaluation_objects
-        self.evaluators = evaluators
-
-        self.labels = labels
-
-        self.args = args
-        self.kwargs = kwargs
-
-        self.id = uuid.uuid4()
-
-    @property
-    def labels(self):
-        """list: List of metric labels."""
-        if self._labels is not None:
-            return self._labels
-
-        try:
-            labels = self.nonlinear_constraint.labels
-        except AttributeError:
-            labels = [f'{self.name}']
-            if self.n_metrics > 1:
-                labels = [
-                    f'{self.name}_{i}'
-                    for i in range(self.n_metrics)
-                ]
-        return labels
-
-    @labels.setter
-    def labels(self, labels):
-        if labels is not None:
+        self.comparison_operator = comparison_operator
 
-            if len(labels) != self.n_metrics:
-                raise CADETProcessError(
-                    f"Expected {self.n_metrics} labels."
-                )
-
-        self._labels = labels
-
-    def __call__(self, request):
-        if self.args is None:
-            args = ()
-        else:
-            args = self.args
-
-        if self.kwargs is None:
-            kwargs = {}
-        else:
-            kwargs = self.kwargs
-
-        g = self.nonlinear_constraint(request, *args, **kwargs)
-
-        return np.array(g, ndmin=1)
-
-    evaluate = __call__
-
-    def __str__(self):
-        return self.name
+        super().__init__(*args, n_metrics=n_nonlinear_constraints, **kwargs)
 
 
 class Callback(Structure):
     """Wrapper class to evaluate callbacks.
 
     Callable must implement function with the following signature:
         results : obj
@@ -3707,86 +3874,24 @@
 
     evaluate = __call__
 
     def __str__(self):
         return self.name
 
 
-class MetaScore(Structure):
+class MetaScore(Metric):
     """Wrapper class to evaluate meta scores."""
+    meta_score = Metric.func
+    n_meta_scores = Metric.n_metrics
+    minimize = Bool(default=True)
 
-    meta_score = Callable()
-    name = String()
-    n_meta_scores = RangedInteger(lb=1)
-    n_metrics = n_meta_scores
-    bad_metrics = SizedNdArray(size='n_metrics', default=np.inf)
+    def __init__(self, *args, n_meta_scores=1, minimize=True, **kwargs):
+        self.minimize = minimize
 
-    def __init__(
-            self,
-            meta_score,
-            name,
-            n_meta_scores=1,
-            bad_metrics=np.inf,
-            evaluation_objects=None,
-            evaluators=None,
-            labels=None):
-
-        self.meta_score = meta_score
-        self.name = name
-
-        self.n_meta_scores = n_meta_scores
-
-        if np.isscalar(bad_metrics):
-            bad_metrics = np.tile(bad_metrics, n_meta_scores)
-        self.bad_metrics = bad_metrics
-
-        self.evaluation_objects = evaluation_objects
-        self.evaluators = evaluators
-
-        self.labels = labels
-
-        self.id = uuid.uuid4()
-
-    @property
-    def labels(self):
-        """list: List of metric labels."""
-        if self._labels is not None:
-            return self._labels
-
-        try:
-            labels = self.meta_score.labels
-        except AttributeError:
-            labels = [f'{self.name}']
-            if self.n_metrics > 1:
-                labels = [
-                    f'{self.name}_{i}'
-                    for i in range(self.n_metrics)
-                ]
-        return labels
-
-    @labels.setter
-    def labels(self, labels):
-        if labels is not None:
-
-            if len(labels) != self.n_metrics:
-                raise CADETProcessError(
-                    f"Expected {self.n_metrics} labels."
-                )
-
-        self._labels = labels
-
-    def __call__(self, *args, **kwargs):
-        m = self.meta_score(*args, **kwargs)
-
-        return np.array(m, ndmin=1)
-
-    evaluate = __call__
-
-    def __str__(self):
-        return self.name
+        super().__init__(*args, n_metrics=n_meta_scores, **kwargs)
 
 
 class MultiCriteriaDecisionFunction(Structure):
     """Wrapper class to evaluate multi-criteria decision functions."""
 
     decision_function = Callable()
     name = String()
@@ -3802,16 +3907,15 @@
         return self.decision_function(*args, **kwargs)
 
     evaluate = __call__
 
     def __str__(self):
         return self.name
 
-
-def approximate_jac(xk, f, epsilon, args=()):
+def approximate_jac(xk, f, epsilon, args=(), **kwargs):
     """Finite-difference approximation of the jacobian of a vector function
 
     Parameters
     ----------
     xk : array_like
         The coordinate vector at which to determine the jacobian of `f`.
     f : callable
@@ -3845,12 +3949,12 @@
     f0 = np.array(f(*((xk,) + args)))
 
     jac = np.zeros((len(f0), len(xk)), float)
     ei = np.zeros((len(xk),), float)
     for k in range(len(xk)):
         ei[k] = 1.0
         d = epsilon * ei
-        f_k = np.array(f(*((xk + d,) + args)))
+        f_k = np.array(f(*((xk + d,) + args), **kwargs))
         jac[:, k] = (f_k - f0) / d[k]
         ei[k] = 0.0
 
     return jac
```

### Comparing `CADET-Process-0.8.0/CADETProcess/optimization/optimizer.py` & `CADET-Process-0.9.0/CADETProcess/optimization/optimizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import shutil
 import time
 import warnings
 
 from cadet import H5
 import numpy as np
 import matplotlib.pyplot as plt
+import numpy as np
 
 from CADETProcess import settings
 from CADETProcess import log
 from CADETProcess import CADETProcessError
 from CADETProcess.dataStructure import Structure
 from CADETProcess.dataStructure import (
     Typed, UnsignedInteger, RangedInteger, UnsignedFloat
@@ -65,19 +66,21 @@
     n_max_iter : int, optional
         Maximum number of iterations (e.g. generations).
     parallelization_backend : ParallelizationBackendBase, optional
         Class used to handle parallelized (and also sequential) evaluation of eval_fun
         functions for each individual in a given population.
         The default parallelization backend is 'Joblib', which provides parallel
         execution using multiple cores.
-    n_cores
+    n_cores : int, optional
+        Proxy to the number of cores used by the parallelization backend.
     """
 
     is_population_based = False
 
+    supports_single_objective = True
     supports_multi_objective = False
     supports_linear_constraints = False
     supports_linear_equality_constraints = False
     supports_nonlinear_constraints = False
     supports_bounds = False
 
     ignore_linear_constraints_config = False
@@ -163,14 +166,16 @@
         See Also
         --------
         OptimizationProblem
         OptimizationResults
         CADETProcess.optimization.ResultsCache
 
         """
+        self._current_cache_entries = []
+
         self.logger = log.get_logger(str(self), level=log_level)
 
         # Check OptimizationProblem
         if not isinstance(optimization_problem, OptimizationProblem):
             raise TypeError('Expected OptimizationProblem')
 
         if not self.check_optimization_problem(optimization_problem):
@@ -228,58 +233,59 @@
         else:
             callbacks_dir = None
         self.callbacks_dir = callbacks_dir
 
         if reinit_cache:
             self.optimization_problem.setup_cache()
 
-        if x0 is None:
-            if optimization_problem.n_linear_equality_constraints > 0:
-                raise CADETProcessError(
-                    "x0 should be set by the user if linear equality "
-                    "constraints are specified."
-                )
-        else:
-            x0check = np.array(x0, ndmin=2)
-            for x in x0check:
-                if not optimization_problem.check_bounds(x):
-                    raise CADETProcessError(f"x0 = {x} does not satisfy bounds.")
-                if not optimization_problem.check_linear_constraints(x):
-                    raise CADETProcessError(f"x0 = {x} does not satisfy linear constraints.")
-                if not optimization_problem.check_linear_equality_constraints(x):
-                    raise CADETProcessError(f"x0 = {x} does not satisfy linear equality constraints.")
+        if x0 is not None:
+            flag, x0 = self.check_x0(optimization_problem, x0)
+
+            if not flag:
+                raise ValueError("x0 contains invalid entries.")
 
         log.log_time('Optimization', self.logger.level)(self.run)
         log.log_results('Optimization', self.logger.level)(self.run)
         log.log_exceptions('Optimization', self.logger.level)(self.run)
 
         backend = plt.get_backend()
         plt.switch_backend('agg')
 
         start = time.time()
-
         self.run(self.optimization_problem, x0, *args, **kwargs)
+        time_elapsed = time.time() - start
 
-        self.results.time_elapsed = time.time() - start
+        self.results.time_elapsed = time_elapsed
+        self.results.cpu_time = self.n_cores * time_elapsed
+
+        self.run_final_processing()
 
         if delete_cache:
             optimization_problem.delete_cache(reinit=True)
+        self._current_cache_entries = []
 
         plt.switch_backend(backend)
 
+        if not self.results.success:
+            raise CADETProcessError(
+                f"Optimizaton failed with message: {self.results.exit_message}"
+            )
+
         return self.results
 
     @abstractmethod
-    def run(optimization_problem, *args, **kwargs):
+    def run(optimization_problem, x0=None, *args, **kwargs):
         """Abstract Method for solving an optimization problem.
 
         Parameters
         ----------
         optimization_problem : OptimizationProblem
             Optimization problem to be solved.
+        x0 : list, optional
+            Initial population of independent variables in untransformed space.
 
         Returns
         -------
         results : OptimizationResults
             Optimization results including OptimizationProblem and Optimizer
             configuration.
 
@@ -309,14 +315,20 @@
         """
         flag = True
         if not optimization_problem.check_config(
                 ignore_linear_constraints=self.ignore_linear_constraints_config):
             # Warnings are raised internally
             flag = False
 
+        if optimization_problem.n_objectives == 1 and not self.supports_single_objective:
+            warnings.warn(
+                "Optimizer does not support single-objective problems"
+            )
+            flag = False
+
         if optimization_problem.n_objectives > 1 and not self.supports_multi_objective:
             warnings.warn(
                 "Optimizer does not support multi-objective problems"
             )
             flag = False
 
         if (
@@ -348,201 +360,256 @@
             warnings.warn(
                 "Optimizer does not support problems with nonlinear constraints."
             )
             flag = False
 
         return flag
 
-    def _run_post_processing(self, current_iteration):
-        if self.optimization_problem.n_multi_criteria_decision_functions > 0:
-            pareto_front = self.results.pareto_front
-
-            X_meta_front = \
-                self.optimization_problem.evaluate_multi_criteria_decision_functions(
-                    pareto_front
-                )
-
-            meta_front = Population()
-            for x in X_meta_front:
-                meta_front.add_individual(pareto_front[x])
-
-            self.results.update_meta(meta_front)
-
-        if current_iteration % self.progress_frequency == 0:
-            self.results.plot_figures(show=False)
-
-        for callback in self.optimization_problem.callbacks:
-            if self.optimization_problem.n_callbacks > 1:
-                _callbacks_dir = self.callbacks_dir / str(callback)
-            else:
-                _callbacks_dir = self.callbacks_dir
-            callback.cleanup(_callbacks_dir, current_iteration)
-            callback._callbacks_dir = _callbacks_dir
-
-        self.optimization_problem.evaluate_callbacks_population(
-            self.results.meta_front,
-            current_iteration,
-            parallelization_backend=self.parallelization_backend,
-        )
-
-        self.results.save_results()
-
-        self.optimization_problem.prune_cache()
-
-    def run_post_evaluation_processing(
-            self, x_transformed, f, g, cv, current_evaluation, x_opt_transformed=None):
-        """Run post-processing of individual evaluation.
+    def check_x0(self, optimization_problem, x0):
+        """Check the initial guess x0 for an optimization problem.
 
         Parameters
         ----------
-        x_transformed : list
-            Optimization variable values of individual in independent transformed space.
-        f : list
-            Objective function values of individual.
-        g : list
-            Nonlinear constraint function of individual.
-        cv : list
-            Nonlinear constraints violation of individual.
-        current_evaluation : int
-            Current evaluation.
-        x_opt_transformed : list, optional
-            Best individual(s) at current iteration in independent transformed space.
-            If None, internal pareto front is used to determine best indiviudal.
+        optimization_problem : OptimizationProblem
+            The optimization problem instance to which x0 is related.
+        x0 : array_like
+            The initial guess for the optimization problem.
+            It can be a single individual or a population.
 
+        Returns
+        -------
+        tuple
+            A tuple containing a boolean flag indicating if x0 is valid, and the
+            potentially modified x0.
         """
-        if self.optimization_problem.n_meta_scores > 0:
-            m = self.optimization_problem.evaluate_meta_scores(
-                x_transformed,
-                untransform=True,
-            )
-        else:
-            m = None
+        flag = True
 
-        x = self.optimization_problem.get_dependent_values(
-                x_transformed, untransform=True
-            )
+        shape = np.array(x0).shape
 
-        ind = Individual(
-            x, f, g, m, cv, self.cv_tol, x_transformed,
-            self.optimization_problem.independent_variable_names,
-            self.optimization_problem.objective_labels,
-            self.optimization_problem.nonlinear_constraint_labels,
-            self.optimization_problem.meta_score_labels,
-            self.optimization_problem.variable_names,
-        )
+        is_x0_1d = len(shape) == 1
 
-        self.results.update_individual(ind)
+        x0 = np.array(x0, ndmin=2)
 
-        if x_opt_transformed is None:
-            self.results.update_pareto()
-        else:
-            x_opt = self.optimization_problem.get_dependent_values(
-                x_opt_transformed, untransform=True
+        n_dependent_variables = optimization_problem.n_dependent_variables
+        n_independent_variables = optimization_problem.n_independent_variables
+        n_variables = n_dependent_variables + n_independent_variables
+
+        if x0.shape[1] != n_variables and x0.shape[1] != n_independent_variables:
+            warnings.warn(
+                f"x0 for optimization problem is expected to be of length "
+                f"{n_independent_variables} or"
+                f"{n_variables}. Got {x0.shape[1]}"
             )
-            pareto_front = Population()
-            ind = self.results.population_all[x_opt]
-            pareto_front.add_individual(ind)
+            flag = False
 
-            self.results.update_pareto(pareto_front)
+        if n_dependent_variables > 0 and x0.shape[1] == n_variables:
+            x0 = [optimization_problem.get_independent_values(ind) for ind in x0]
+            warnings.warn(
+                "x0 contains dependent values. Will recompute dependencies for consistency."
+            )
+            x0 = np.array(x0)
 
-        self._run_post_processing(current_evaluation)
+        for x in x0:
+            if not optimization_problem.check_individual(x, get_dependent_values=True):
+                flag = False
+                break
 
-        self.logger.info(
-            f'Finished Evaluation {current_evaluation}.'
-        )
-        for ind in self.results.pareto_front:
-            message = f'x: {ind.x}, f: {ind.f}'
+        if is_x0_1d:
+            x0 = x0[0]
 
-            if self.optimization_problem.n_nonlinear_constraints > 0:
-                message += f', g: {ind.g}'
-
-            if self.optimization_problem.n_meta_scores > 0:
-                message += f', m: {ind.m}'
-            self.logger.info(message)
+        x0 = x0.tolist()
 
-    def run_post_generation_processing(
-            self, X_transformed, F, G, CV, current_generation, X_opt_transformed=None):
-        """Run post-processing of generation.
+        return flag, x0
 
-        Parameters
-        ----------
-        X_transformed : list
-            Optimization variable values of generation in independent transformed space.
-        F : list
-            Objective function values of generation.
-        G : list
-            Nonlinear constraint function values of generation.
-        CV : list
-            Nonlinear constraints violation of of generation.
-        current_generation : int
-            Current generation.
-        X_opt_transformed : list, optional
-            (Currently) best variable values in independent transformed space.
-            If None, internal pareto front is used to determine best values.
+    def _create_population(self, X_transformed, F, F_min, G, CV):
+        """Create new population from current generation for post procesing."""
+        X_transformed = np.array(X_transformed, ndmin=2)
+        F = np.array(F, ndmin=2)
+        F_min = np.array(F_min, ndmin=2)
+        G = np.array(G, ndmin=2)
+        CV = np.array(CV, ndmin=2)
 
-        """
         if self.optimization_problem.n_meta_scores > 0:
-            M = self.optimization_problem.evaluate_meta_scores_population(
+            M_min = self.optimization_problem.evaluate_meta_scores_population(
                 X_transformed,
                 untransform=True,
+                ensure_minimization=True,
                 parallelization_backend=self.parallelization_backend,
             )
+            M = self.optimization_problem.transform_maximization(M_min, scores='meta_scores')
         else:
+            M_min = len(X_transformed)*[None]
             M = len(X_transformed)*[None]
 
         if self.optimization_problem.n_nonlinear_constraints == 0:
             G = len(X_transformed)*[None]
             CV = len(X_transformed)*[None]
 
         population = Population()
-        for x_transformed, f, g, cv, m in zip(X_transformed, F, G, CV, M):
+        for x_transformed, f, f_min, g, cv, m, m_min in zip(X_transformed, F, F_min, G, CV, M, M_min):
             x = self.optimization_problem.get_dependent_values(
                 x_transformed, untransform=True
             )
             ind = Individual(
-                x, f, g, m, cv, self.cv_tol, x_transformed,
+                x, f, g, m, x_transformed, f_min, cv, self.cv_tol, m_min,
                 self.optimization_problem.independent_variable_names,
                 self.optimization_problem.objective_labels,
                 self.optimization_problem.nonlinear_constraint_labels,
                 self.optimization_problem.meta_score_labels,
                 self.optimization_problem.variable_names,
             )
             population.add_individual(ind)
 
-        self.results.update_population(population)
+        return population
 
+    def _create_pareto_front(self, X_opt_transformed):
+        """Create new pareto front from current generation for post procesing."""
         if X_opt_transformed is None:
-            self.results.update_pareto()
+            pareto_front = None
         else:
             pareto_front = Population()
 
             for x_opt_transformed in X_opt_transformed:
                 x_opt = self.optimization_problem.get_dependent_values(
                     x_opt_transformed, untransform=True
                 )
                 ind = self.results.population_all[x_opt]
                 pareto_front.add_individual(ind)
 
-            self.results.update_pareto(pareto_front)
+        return pareto_front
+
+    def _create_meta_front(self):
+        """Create new meta front from current generation for post procesing."""
+        if self.optimization_problem.n_multi_criteria_decision_functions == 0:
+            meta_front = None
+        else:
+            pareto_front = self.results.pareto_front
+
+            X_meta_front = \
+                self.optimization_problem.evaluate_multi_criteria_decision_functions(
+                    pareto_front
+                )
+
+            meta_front = Population()
+            for x in X_meta_front:
+                meta_front.add_individual(pareto_front[x])
+
+        return meta_front
 
-        self._run_post_processing(current_generation)
+    def _evaluate_callbacks(self, current_generation, sub_dir=None):
+        if sub_dir is not None:
+            callbacks_dir = self.callbacks_dir / sub_dir
+            callbacks_dir.mkdir(exist_ok=True, parents=True)
+        else:
+            callbacks_dir = self.callbacks_dir
+
+        for callback in self.optimization_problem.callbacks:
+            if self.optimization_problem.n_callbacks > 1:
+                _callbacks_dir = callbacks_dir / str(callback)
+            else:
+                _callbacks_dir = callbacks_dir
 
+            callback.cleanup(_callbacks_dir, current_generation)
+            callback._callbacks_dir = _callbacks_dir
+
+        self.optimization_problem.evaluate_callbacks_population(
+            self.results.meta_front,
+            current_generation,
+            parallelization_backend=self.parallelization_backend,
+        )
+
+    def _log_results(self, current_generation):
         self.logger.info(
             f'Finished Generation {current_generation}.'
         )
-        for ind in self.results.pareto_front:
+        for ind in self.results.meta_front:
             message = f'x: {ind.x}, f: {ind.f}'
 
             if self.optimization_problem.n_nonlinear_constraints > 0:
                 message += f', g: {ind.g}'
 
             if self.optimization_problem.n_meta_scores > 0:
                 message += f', m: {ind.m}'
             self.logger.info(message)
 
+    def run_post_processing(
+            self,
+            X_transformed,
+            F_minimized,
+            G,
+            CV,
+            current_generation,
+            X_opt_transformed=None
+            ):
+        """Run post-processing of generation.
+
+        Notes
+        -----
+        This method also works for optimizers that only perform a single evaluation per
+        "generation".
+
+        Parameters
+        ----------
+        X_transformed : list
+            Optimization variable values of generation in independent transformed space.
+        F_minimized : list
+            Objective function values of generation.
+            This assumes that all objective function values are minimized.
+        G : list
+            Nonlinear constraint function values of generation.
+        CV : list
+            Nonlinear constraints violation of of generation.
+        current_generation : int
+            Current generation.
+        X_opt_transformed : list, optional
+            (Currently) best variable values in independent transformed space.
+            If None, internal pareto front is used to determine best values.
+
+        """
+        F = self.optimization_problem.transform_maximization(F_minimized, scores='objectives')
+        population = self._create_population(X_transformed, F, F_minimized, G, CV)
+        self.results.update(population)
+
+        pareto_front = self._create_pareto_front(X_opt_transformed)
+        self.results.update_pareto(pareto_front)
+
+        meta_front = self._create_meta_front()
+        if meta_front is not None:
+            self.results.update_meta(meta_front)
+
+        if current_generation % self.progress_frequency == 0:
+            self.results.plot_figures(show=False)
+
+        self._evaluate_callbacks(current_generation)
+
+        self.results.save_results('checkpoint')
+
+        # Remove new entries from cache that didn't make it to the meta front
+        for x in population.x:
+            x_key = x.tobytes()
+            if x not in self.results.meta_front.x:
+                self.optimization_problem.prune_cache(x_key)
+            else:
+                self._current_cache_entries.append(x_key)
+
+        # Remove old meta front entries from cache that were replaced by better ones
+        for x_key in self._current_cache_entries:
+            x = np.frombuffer(x_key)
+            if not np.all(np.isin(x, self.results.meta_front.x)):
+                self.optimization_problem.prune_cache(x_key)
+                self._current_cache_entries.remove(x_key)
+
+        self._log_results(current_generation)
+
+    def run_final_processing(self):
+        self.results.plot_figures(show=False)
+        if self.optimization_problem.n_callbacks > 0:
+            self._evaluate_callbacks(0, 'final')
+        self.results.save_results('final')
+
     @property
     def options(self):
         """dict: Optimizer options."""
         return {
             opt: getattr(self, opt)
             for opt in (self._general_options + self._specific_options)
         }
@@ -555,20 +622,23 @@
             for opt in (self._specific_options)
         }
 
     @property
     def n_cores(self):
         """int: Proxy to the number of cores used by the parallelization backend.
 
+        Note, this will always return the actual number of cores used, even if negative
+        values are set.
+
         See Also
         --------
         parallelization_backend
 
         """
-        return self.parallelization_backend.n_cores
+        return self.parallelization_backend._n_cores
 
     @n_cores.setter
     def n_cores(self, n_cores):
         self.parallelization_backend.n_cores = n_cores
 
     def __str__(self):
         return self.__class__.__name__
```

### Comparing `CADET-Process-0.8.0/CADETProcess/optimization/parallelizationBackend.py` & `CADET-Process-0.9.0/CADETProcess/optimization/parallelizationBackend.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/optimization/population.py` & `CADET-Process-0.9.0/CADETProcess/optimization/population.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,14 +86,22 @@
         """tuple: Individual dimensions (n_x, n_f, n_g, n_m)"""
         if self.n_individuals == 0:
             return None
 
         return self.individuals[0].dimensions
 
     @property
+    def objectives_minimization_factors(self):
+        return self.individuals[0].objectives_minimization_factors
+
+    @property
+    def meta_scores_minimization_factors(self):
+        return self.individuals[0].meta_scores_minimization_factors
+
+    @property
     def variable_names(self):
         """list: Names of the optimization variables."""
         if self.individuals[0].variable_names is None:
             return [f'x_{i}' for i in range(self.n_x)]
         else:
             return self.individuals[0].variable_names
 
@@ -238,14 +246,25 @@
 
     @property
     def f(self):
         """np.array: All evaluated objective function values."""
         return np.array([ind.f for ind in self.individuals])
 
     @property
+    def f_minimized(self):
+        """np.array: All evaluated objective function values, transformed to be minimized."""
+        return np.array([ind.f_min for ind in self.individuals])
+
+    @property
+    def f_best(self):
+        """np.array: Best objective values."""
+        f_best = np.min(self.f_minimized, axis=0)
+        return np.multiply(self.objectives_minimization_factors, f_best)
+
+    @property
     def f_min(self):
         """np.array: Minimum objective values."""
         return np.min(self.f, axis=0)
 
     @property
     def f_max(self):
         """np.array: Maximum objective values."""
@@ -259,29 +278,36 @@
     @property
     def g(self):
         """np.array: All evaluated nonlinear constraint function values."""
         if self.dimensions[2] > 0:
             return np.array([ind.g for ind in self.individuals])
 
     @property
+    def g_best(self):
+        """np.array: Best nonlinear constraint values."""
+        indices = np.argmin(self.cv, axis=0)
+        return [self.g[ind, i] for i, ind in enumerate(indices)]
+
+    @property
     def g_min(self):
         """np.array: Minimum nonlinear constraint values."""
         if self.dimensions[2] > 0:
             return np.min(self.g, axis=0)
 
     @property
     def g_max(self):
         """np.array: Maximum nonlinear constraint values."""
         if self.dimensions[2] > 0:
             return np.max(self.g, axis=0)
 
     @property
     def g_avg(self):
         """np.array: Average nonlinear constraint values."""
-        return np.mean(self.g, axis=0)
+        if self.dimensions[2] > 0:
+            return np.mean(self.g, axis=0)
 
     @property
     def cv(self):
         """np.array: All evaluated nonlinear constraint function values."""
         if self.dimensions[2] > 0:
             return np.array([ind.cv for ind in self.individuals])
 
@@ -296,42 +322,57 @@
         """np.array: Maximum nonlinearconstraint violation values."""
         if self.dimensions[2] > 0:
             return np.max(self.cv, axis=0)
 
     @property
     def cv_avg(self):
         """np.array: Average nonlinear constraint violation values."""
-        return np.mean(self.cv, axis=0)
+        if self.dimensions[2] > 0:
+            return np.mean(self.cv, axis=0)
 
     @property
     def m(self):
-        """np.array: All evaluated metas core values."""
+        """np.array: All evaluated meta scores."""
         if self.dimensions[3] > 0:
             return np.array([ind.m for ind in self.individuals])
 
     @property
+    def m_minimized(self):
+        """np.array: All evaluated meta scores, transformed to be minimized."""
+        if self.dimensions[3] > 0:
+            return np.array([ind.m_min for ind in self.individuals])
+
+    @property
+    def m_best(self):
+        """np.array: Best meta scores."""
+        if self.dimensions[3] > 0:
+            m_best = np.min(self.m_minimized, axis=0)
+            return np.multiply(self.meta_scores_minimization_factors, m_best)
+
+    @property
     def m_min(self):
-        """np.array: Minimum meta score values."""
+        """np.array: Minimum meta scores."""
         if self.dimensions[3] > 0:
             return np.min(self.m, axis=0)
 
     @property
     def m_max(self):
-        """np.array: Maximum meta score values."""
+        """np.array: Maximum meta scores."""
         if self.dimensions[3] > 0:
             return np.max(self.m, axis=0)
 
     @property
     def m_avg(self):
-        """np.array: Average meta score values."""
-        return np.mean(self.m, axis=0)
+        """np.array: Average meta scores."""
+        if self.dimensions[3] > 0:
+            return np.mean(self.m, axis=0)
 
     @property
     def is_feasilbe(self):
-        """np.array: Average meta score values."""
+        """np.array: False if any constraint is not met. True otherwise."""
         return np.array([ind.is_feasible for ind in self.individuals])
 
     def setup_objectives_figure(self, include_meta=True, plot_individual=False):
         """Set up figure and axes for plotting objectives.
 
         Parameters
         ----------
@@ -432,16 +473,23 @@
         variables = self.variable_names
         feasible = self.feasible
         infeasible = self.infeasible
         x_feas = feasible.x
         x_infeas = infeasible.x
 
         if include_meta and self.m is not None:
-            values_feas = np.hstack((feasible.f, feasible.m))
-            values_infeas = np.hstack((infeasible.f, infeasible.m))
+            if len(feasible) > 0:
+                values_feas = np.hstack((feasible.f, feasible.m))
+            else:
+                values_infeas = np.empty((0, self.n_f + self.n_m))
+            if len(infeasible) > 0:
+                values_infeas = np.hstack((infeasible.f, infeasible.m))
+            else:
+                values_infeas = np.empty((0, self.n_f + self.n_m))
+
             labels = self.objective_labels + self.meta_score_labels
         else:
             values_feas = feasible.f
             values_infeas = infeasible.f
             labels = self.objective_labels
 
         for i_var, var in enumerate(variables):
```

### Comparing `CADET-Process-0.8.0/CADETProcess/optimization/pymooAdapter.py` & `CADET-Process-0.9.0/CADETProcess/optimization/pymooAdapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         """Solve optimization problem using functional pymoo implementation.
 
         Parameters
         ----------
         optimization_problem : OptimizationProblem
             DESCRIPTION.
         x0 : list, optional
-            Initial population
+            Initial population of independent variables in untransformed space.
 
         Returns
         -------
         results : OptimizationResults
             Optimization results including optimization_problem and solver
             configuration.
 
@@ -68,34 +68,31 @@
         --------
         evaluate_objectives
         options
 
         """
         pop_size = self.get_population_size(optimization_problem)
 
-        # equality constraints make it more difficult to find feasible samples
-        # in the parameter space. Therefore increase burnin
-        # this gets very expensive with lots of constraints
-        burn_in = 1e5 * 10 ** optimization_problem.n_linear_equality_constraints
-
         if x0 is not None:
             pop = x0
         else:
             pop = optimization_problem.create_initial_values(
-                pop_size, method='chebyshev', seed=self.seed,
-                burn_in=burn_in
+                pop_size, seed=self.seed, include_dependent_variables=False
             )
 
         pop = np.array(pop, ndmin=2)
 
         if len(pop) < pop_size:
+            warnings.warn(
+                "Initial population smaller than popsize. "
+                "Creating missing entries."
+            )
             n_remaining = pop_size - len(pop)
             remaining = optimization_problem.create_initial_values(
-                n_remaining, method='chebyshev', seed=self.seed,
-                burn_in=burn_in
+                n_remaining, seed=self.seed, include_dependent_variables=False
             )
             pop = np.vstack((pop, remaining))
         elif len(pop) > pop_size:
             warnings.warn("Initial population larger than popsize. Omitting overhead.")
             pop = pop[0:pop_size]
 
         pop = np.array(optimization_problem.transform(pop))
@@ -165,23 +162,26 @@
             # Handle issue of pymoo not handling np.inf
             pop.set("F", np.nan_to_num(F, posinf=1e300))
 
             algorithm.tell(infills=pop)
 
             # Post generation processing
             X_opt = algorithm.opt.get("X").tolist()
-            self.run_post_generation_processing(X, F, G, CV, algorithm.n_gen-1, X_opt)
+            self.run_post_processing(X, F, G, CV, algorithm.n_gen-1, X_opt)
 
         if algorithm.n_gen >= n_max_gen:
-            exit_message = 'Max number of generations exceeded.'
+            success = True
             exit_flag = 1
+            exit_message = 'Max number of generations exceeded.'
         else:
+            success = True
             exit_flag = 0
-            exit_message = 'success'
+            exit_message = 'Success'
 
+        self.results.success = success
         self.results.exit_flag = exit_flag
         self.results.exit_message = exit_message
 
         return self.results
 
     def get_population_size(self, optimization_problem):
         if self.pop_size is None:
@@ -234,14 +234,15 @@
 
     def _evaluate(self, X, out, *args, **kwargs):
         opt = self.optimization_problem
         if opt.n_objectives > 0:
             F = opt.evaluate_objectives_population(
                 X,
                 untransform=True,
+                ensure_minimization=True,
                 parallelization_backend=self.parallelization_backend,
             )
             out["F"] = np.array(F)
 
         if opt.n_nonlinear_constraints > 0:
             G = opt.evaluate_nonlinear_constraints_population(
                 X,
@@ -264,23 +265,17 @@
         self.optimization_problem = optimization_problem
         super().__init__(*args, **kwargs)
 
     def _do(self, problem, X, **kwargs):
         # Check if linear (equality) constraints are met
         X_new = None
         for i, ind in enumerate(X):
-            if (
-                    not self.optimization_problem.check_linear_constraints(
-                        ind, untransform=True, get_dependent_values=True
-                    )
-                    or
-                    not self.optimization_problem.check_linear_equality_constraints(
-                        ind, untransform=True, get_dependent_values=True
-                    )
-            ):
+            if not self.optimization_problem.check_individual(
+                    ind, untransform=True, get_dependent_values=True):
                 if X_new is None:
-                    burn_in = 1e5 * 10 ** self.optimization_problem.n_linear_equality_constraints
-                    X_new = self.optimization_problem.create_initial_values(len(X), burn_in)
+                    X_new = self.optimization_problem.create_initial_values(
+                        len(X), include_dependent_variables=False
+                    )
                 x_new = X_new[i, :]
                 X[i, :] = self.optimization_problem.transform(x_new)
 
         return X
```

### Comparing `CADET-Process-0.8.0/CADETProcess/optimization/results.py` & `CADET-Process-0.9.0/CADETProcess/optimization/results.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,36 +10,43 @@
 cmap_infeas = plt.get_cmap('autumn_r')
 import numpy as np
 
 from cadet import H5
 from CADETProcess import plotting
 from CADETProcess.dataStructure import Structure
 from CADETProcess.dataStructure import (
-    NdArray, String, UnsignedInteger, UnsignedFloat
+    Bool, Dictionary, NdArray, String, UnsignedInteger, UnsignedFloat
 )
 
 from CADETProcess import CADETProcessError
+from CADETProcess.sysinfo import system_information
 from CADETProcess.optimization import Individual, Population, ParetoFront
 
 
 class OptimizationResults(Structure):
     """Optimization results.
 
     Attributes
     ----------
     optimization_problem : OptimizationProblem
         Optimization problem.
     optimizer : OptimizerBase
         Optimizer used to optimize the OptimizationProblem.
+    success : bool
+        True if optimization was successfully terminated. False otherwise.
     exit_flag : int
         Information about the solver termination.
     exit_message : str
         Additional information about the solver status.
     time_elapsed : float
         Execution time of simulation.
+    cpu_time : float
+        CPU run time, taking into account the number of cores used for the optimiation.
+    system_information : dict
+        Information about the system on which the optimization was performed.
     x : list
         Values of optimization variables at optimum.
     f : np.ndarray
         Value of objective function at x.
     g : np.ndarray
         Values of constraint function at x
     population_last : Population
@@ -47,17 +54,20 @@
     pareto_front : ParetoFront
         Pareto optimal solutions.
     meta_front : ParetoFront
         Reduced pareto optimal solutions using meta scores and multi-criteria decision
         functions.
 
     """
+    success = Bool(default=False)
     exit_flag = UnsignedInteger()
     exit_message = String()
     time_elapsed = UnsignedFloat()
+    cpu_time = UnsignedFloat()
+    system_information = Dictionary()
 
     def __init__(
             self, optimization_problem, optimizer,
             similarity_tol=0, cv_tol=1e-6):
         self.optimization_problem = optimization_problem
         self.optimizer = optimizer
 
@@ -72,14 +82,16 @@
         if optimization_problem.n_multi_criteria_decision_functions > 0:
             self._meta_fronts = []
         else:
             self._meta_fronts = None
 
         self.results_directory = None
 
+        self.system_information = system_information
+
     @property
     def results_directory(self):
         return self._results_directory
 
     @results_directory.setter
     def results_directory(self, results_directory):
         if results_directory is not None:
@@ -132,50 +144,34 @@
     @property
     def meta_front(self):
         if self._meta_fronts is None:
             return self.pareto_front
         else:
             return self._meta_fronts[-1]
 
-    def update_individual(self, individual):
+    def update(self, new):
         """Update Results.
 
         Parameters
         ----------
-        individual : Individual
-            Latest individual.
+        new : Individual, Population
+            New results
 
         Raises
         ------
         CADETProcessError
-            If individual is not an instance of Individual
+            If new is not an instance of Individual or Population
         """
-        if not isinstance(individual, Individual):
-            raise CADETProcessError("Expected Individual")
-
-        population = Population()
-        population.add_individual(individual)
-        self._populations.append(population)
-        self.population_all.add_individual(individual, ignore_duplicate=True)
-
-    def update_population(self, population):
-        """Update Results.
-
-        Parameters
-        ----------
-        population : Population
-            Current population
-
-        Raises
-        ------
-        CADETProcessError
-            If population is not an instance of Population
-        """
-        if not isinstance(population, Population):
-            raise CADETProcessError("Expected Population")
+        if isinstance(new, Individual):
+            population = Population()
+            population.add_individual(new)
+        elif isinstance(new, Population):
+            population = new
+        else:
+            raise CADETProcessError("Expected Population or Individual")
         self._populations.append(population)
         self.population_all.update(population)
 
     def update_pareto(self, pareto_new=None):
         """Update pareto front with new population.
 
         Parameters
@@ -253,14 +249,19 @@
     @property
     def n_evals_history(self):
         """int: Number of evaluations per generation."""
         n_evals = [len(pop) for pop in self.populations]
         return np.cumsum(n_evals)
 
     @property
+    def f_best_history(self):
+        """np.array: Best objective values per generation."""
+        return np.array([pop.f_best for pop in self.meta_fronts])
+
+    @property
     def f_min_history(self):
         """np.array: Minimum objective values per generation."""
         return np.array([pop.f_min for pop in self.meta_fronts])
 
     @property
     def f_max_history(self):
         """np.array: Maximum objective values per generation."""
@@ -268,14 +269,19 @@
 
     @property
     def f_avg_history(self):
         """np.array: Average objective values per generation."""
         return np.array([pop.f_avg for pop in self.meta_fronts])
 
     @property
+    def g_best_history(self):
+        """np.array: Best nonlinear constraint per generation."""
+        return np.array([pop.g_best for pop in self.meta_fronts])
+
+    @property
     def g_min_history(self):
         """np.array: Minimum nonlinear constraint values per generation."""
         if self.optimization_problem.n_nonlinear_constraints == 0:
             return None
         else:
             return np.array([pop.g_min for pop in self.meta_fronts])
 
@@ -316,32 +322,37 @@
         """np.array: Average nonlinear constraint violation values per generation."""
         if self.optimization_problem.n_nonlinear_constraints == 0:
             return None
         else:
             return np.array([pop.cv_avg for pop in self.meta_fronts])
 
     @property
+    def m_best_history(self):
+        """np.array: Best meta scores per generation."""
+        return np.array([pop.m_best for pop in self.meta_fronts])
+
+    @property
     def m_min_history(self):
-        """np.array: Minimum meta score values per generation."""
+        """np.array: Minimum meta scores per generation."""
         if self.optimization_problem.n_meta_scores == 0:
             return None
         else:
             return np.array([pop.m_min for pop in self.meta_fronts])
 
     @property
     def m_max_history(self):
-        """np.array: Maximum meta score values per generation."""
+        """np.array: Maximum meta scores per generation."""
         if self.optimization_problem.n_meta_scores == 0:
             return None
         else:
             return np.array([pop.m_max for pop in self.meta_fronts])
 
     @property
     def m_avg_history(self):
-        """np.array: Average meta score values per generation."""
+        """np.array: Average meta scores per generation."""
         if self.optimization_problem.n_meta_scores == 0:
             return None
         else:
             return np.array([pop.m_avg for pop in self.meta_fronts])
 
     def plot_figures(self, show=True):
         """Plot result figures.
@@ -383,15 +394,16 @@
             if self.optimization_problem.n_variables > 1 and len(self.x) > 1:
                 self.plot_corner(
                     show=show, plot_directory=self.plot_directory
                 )
 
             if self.optimization_problem.n_objectives > 1:
                 self.plot_pareto(
-                    show=show, plot_directory=self.plot_directory
+                    show=show, plot_directory=self.plot_directory,
+                    plot_evolution=True, plot_pareto=False,
                 )
 
     def plot_objectives(
             self,
             include_meta=True,
             plot_pareto=False,
             plot_infeasible=True,
@@ -636,23 +648,23 @@
             figs = [figs]
 
         layout = plotting.Layout()
         layout.x_label = '$n_{Evaluations}$'
 
         if target == 'objectives':
             funcs = self.optimization_problem.objectives
-            values_min = self.f_min_history
+            values_min = self.f_best_history
             values_avg = self.f_avg_history
         elif target == 'nonlinear_constraints':
             funcs = self.optimization_problem.nonlinear_constraints
-            values_min = self.g_min_history
+            values_min = self.g_best_history
             values_avg = self.g_avg_history
         elif target == 'meta_scores':
             funcs = self.optimization_problem.meta_scores
-            values_min = self.m_min_history
+            values_min = self.m_best_history
             values_avg = self.m_avg_history
         else:
             raise CADETProcessError("Unknown target.")
 
         if len(funcs) == 0:
             return
 
@@ -748,46 +760,50 @@
                     )
             else:
                 figname = f'convergence_{target}'
                 figs[0].savefig(
                     f'{plot_directory / figname}.png'
                 )
 
-    def save_results(self):
+    def save_results(self, name):
         if self.results_directory is not None:
             self._update_csv(self.population_last, 'results_all', mode='a')
             self._update_csv(self.population_last, 'results_last', mode='w')
             self._update_csv(self.pareto_front, 'results_pareto', mode='w')
             if self.optimization_problem.n_meta_scores > 0:
                 self._update_csv(self.meta_front, 'results_meta', mode='w')
 
             results = H5()
             results.root = Dict(self.to_dict())
-            results.filename = self.results_directory / 'checkpoint.h5'
+            results.filename = self.results_directory / f'{name}.h5'
             results.save()
 
     def to_dict(self):
         """Convert Results to a dictionary.
 
         Returns
         -------
         addict.Dict
             Results as a dictionary with populations stored as list of dictionaries.
         """
         data = Dict()
+        data.system_information = self.system_information
         data.optimizer_state = self.optimizer_state
         data.population_all_id = str(self.population_all.id)
         data.populations = {i: pop.to_dict() for i, pop in enumerate(self.populations)}
         data.pareto_fronts = {
             i: front.to_dict() for i, front in enumerate(self.pareto_fronts)
         }
         if self._meta_fronts is not None:
             data.meta_fronts = {
                 i: front.to_dict() for i, front in enumerate(self.meta_fronts)
             }
+        if self.time_elapsed is not None:
+            data.time_elapsed = self.time_elapsed
+            data.cpu_time = self.cpu_time
 
         return data
 
     def update_from_dict(self, data):
         """Update internal state from dictionary.
 
         Parameters
@@ -796,15 +812,15 @@
             Serialized data.
         """
         self._optimizer_state = data['optimizer_state']
         self._population_all = Population(id=data['population_all_id'])
 
         for pop_dict in data['populations'].values():
             pop = Population.from_dict(pop_dict)
-            self.update_population(pop)
+            self.update(pop)
 
         self._pareto_fronts = [
             ParetoFront.from_dict(d) for d in data['pareto_fronts'].values()
         ]
         if self._meta_fronts is not None:
             self._meta_fronts = [
                 ParetoFront.from_dict(d) for d in data['meta_fronts'].values()
```

### Comparing `CADET-Process-0.8.0/CADETProcess/optimization/scipyAdapter.py` & `CADET-Process-0.9.0/CADETProcess/optimization/scipyAdapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
         Returns
         -------
         results : OptimizationResults
             Optimization results including optimization_problem and solver
             configuration.
         x0 : list, optional
-            Initial values.
+            Initial values of independent variables in untransformed space.
 
         See Also
         --------
         COBYLA
         TrustConstr
         NelderMead
         SLSQP
@@ -74,15 +74,17 @@
         """
         self.n_evals = 0
 
         if optimization_problem.n_objectives > 1:
             raise CADETProcessError("Can only handle single objective.")
 
         def objective_function(x):
-            return optimization_problem.evaluate_objectives(x, untransform=True)[0]
+            return optimization_problem.evaluate_objectives(
+                x, untransform=True, ensure_minimization=True,
+            )[0]
 
         def callback_function(x, state=None):
             """Internal callback to report progress after evaluation.
 
             Notes
             -----
             Currently, this evaluates all functions again. This should not be a problem
@@ -90,28 +92,34 @@
 
             Unfortunately, only `trust-constr` returns a `state` which contains the
             current best point. Hence, the internal pareto front is used.
             """
             self.n_evals += 1
 
             x = x.tolist()
-            f = optimization_problem.evaluate_objectives(x, untransform=True)
+            f = optimization_problem.evaluate_objectives(
+                x,
+                untransform=True,
+                ensure_minimization=True,
+            )
             g = optimization_problem.evaluate_nonlinear_constraints(
                 x, untransform=True
             )
             cv = optimization_problem.evaluate_nonlinear_constraints_violation(
                 x, untransform=True
             )
 
-            self.run_post_evaluation_processing(x, f, g, cv, self.n_evals)
+            self.run_post_processing(x, f, g, cv, self.n_evals)
 
             return False
 
         if x0 is None:
-            x0 = optimization_problem.create_initial_values(1, method='chebyshev')[0]
+            x0 = optimization_problem.create_initial_values(
+                1, include_dependent_variables=False
+            )[0]
 
         x0_transformed = optimization_problem.transform(x0)
 
         options = self.specific_options
         if self.results.n_gen > 0:
             x0 = self.results.population_last.x[0, :]
             self.n_evals = self.results.n_evals
@@ -130,14 +138,15 @@
                 jac=self.jac,
                 constraints=self.get_constraint_objects(optimization_problem),
                 bounds=self.get_bounds(optimization_problem),
                 options=options,
                 callback=callback_function,
             )
 
+        self.results.success = bool(scipy_results.success)
         self.results.exit_flag = scipy_results.status
         self.results.exit_message = scipy_results.message
 
     def get_bounds(self, optimization_problem):
         """Returns the optimized bounds of a given optimization_problem as a
         Bound object.
 
@@ -152,25 +161,21 @@
         return optimize.Bounds(
             optimization_problem.lower_bounds_independent_transformed,
             optimization_problem.upper_bounds_independent_transformed,
             keep_feasible=True
         )
 
     def get_constraint_objects(self, optimization_problem):
-        """Defines the constraints of the optimization_problem and resturns
-        them into a list.
-
-        First defines the lincon, the linequon and the nonlincon constraints.
-        Returns the constrainst in a list.
+        """Return constraints as objets.
 
         Returns
         -------
         constraint_objects : list
-            List containing  a sorted list of all constraints of an
-            optimization_problem, if they're not None.
+            List containing lists of all constraint types of the optimization_problem.
+            If type of constraints is not defined, it is replaced with None.
 
         See Also
         --------
         lincon_obj
         lincon_obj
         nonlincon_obj
         """
@@ -179,24 +184,21 @@
         nonlincon = self.get_nonlincon_obj(optimization_problem)
 
         constraints = [lincon, lineqcon, *nonlincon]
 
         return [con for con in constraints if con is not None]
 
     def get_lincon_obj(self, optimization_problem):
-        """Returns the optimized linear constraint as an object.
-
-        Sets the lower and upper bounds of the optimization_problem and returns
-        optimized linear constraints. Keep_feasible is set to True.
+        """Return the linear constraints as an object.
 
         Returns
         -------
         lincon_obj : LinearConstraint
-            Linear Constraint object with optimized upper and lower bounds of b
-            of the optimization_problem.
+            Linear Constraint object with lower and upper bounds of b of the
+            optimization_problem.
 
         See Also
         --------
         constraint_objects
         A
         b
         """
@@ -207,28 +209,21 @@
         ub = optimization_problem.b_transformed
 
         return optimize.LinearConstraint(
             optimization_problem.A_independent_transformed, lb, ub, keep_feasible=True
         )
 
     def get_lineqcon_obj(self, optimization_problem):
-        """Returns the optimized linear equality constraints as an object.
-
-        Checks the length of the beq first, before setting the bounds of the
-        constraint. Sets the lower and upper bounds of the
-        optimization_problem and returns optimized linear equality constraints.
-        Keep_feasible is set to True.
+        """Return the linear equality constraints as an object.
 
         Returns
         -------
-        None: bool
-            If the length of the beq of the optimization_problem is equal zero.
         lineqcon_obj : LinearConstraint
-            Linear equality Constraint object with optimized upper and lower
-            bounds of beq of the optimization_problem.
+            Linear equality Constraint object with lower and upper bounds of beq of the
+            optimization_problem.
 
         See Also
         --------
         constraint_objects
         Aeq
         beq
         """
@@ -240,37 +235,20 @@
 
         return optimize.LinearConstraint(
             optimization_problem.Aeq_independent_transformed, lb, ub,
             keep_feasible=True
         )
 
     def get_nonlincon_obj(self, optimization_problem):
-        """Returns the optimized nonlinear constraints as an object.
-
-        Checks the length of the nonlinear_constraints first, before setting
-        the bounds of the constraint. Tries to set the bounds from the list
-        nonlinear_constraints from the optimization_problem for the lower
-        bounds and sets the upper bounds for the length of the
-        nonlinear_constraints list. If a TypeError is excepted it sets the
-        lower bound by the first entry of the nonlinear_constraints list and
-        the upper bound to infinity. Then a local variable named
-        finite_diff_rel_step is defined. After setting the bounds it returns
-        the optimized nonlinear constraints as an object with the
-        finite_diff_rel_step and the jacobian matrix. The jacobian matrix is
-        got by calling the method nonlinear_constraint_jacobian from the
-        optimization_problem. Keep_feasible is set to True.
+        """Return the optimized nonlinear constraints as an object.
 
         Returns
         -------
-        None: bool
-            If the length of the nonlinear_constraints of the
-            optimization_problem is equal zero.
-        nonlincon_obj : NonlinearConstraint
-            Linear equality Constraint object with optimized upper and lower
-            bounds of beq of the optimization_problem.
+        nonlincon_obj : list
+            Nonlinear constraint violation objects with bounds the optimization_problem.
 
         See Also
         --------
         constraint_objects
         nonlinear_constraints
         """
         if optimization_problem.n_nonlinear_constraints == 0:
@@ -293,19 +271,19 @@
 
             Notes
             -----
             Note, this is necessary to avoid side effects when creating the function
             in the main loop.
             """
             constr = optimize.NonlinearConstraint(
-                lambda x: opt.evaluate_nonlinear_constraints(x, untransform=True)[i],
-                lb=-np.inf, ub=opt.nonlinear_constraints_bounds[i],
+                lambda x: opt.evaluate_nonlinear_constraints_violation(x, untransform=True)[i],
+                lb=-np.inf, ub=0,
                 finite_diff_rel_step=self.finite_diff_rel_step,
                 keep_feasible=True
-                )
+            )
             return constr
 
         constraints = []
         for i in range(opt.n_nonlinear_constraints):
             constraints.append(makeConstraint(i))
 
         return constraints
```

### Comparing `CADET-Process-0.8.0/CADETProcess/performance.py` & `CADET-Process-0.9.0/CADETProcess/performance.py`

 * *Files 2% similar despite different names*

```diff
@@ -305,80 +305,80 @@
     See Also
     --------
     PerformanceIndicator
 
     """
 
     def _evaluate(self, performance):
-        return - performance.mass
+        return performance.mass
 
 
 class Recovery(PerformanceIndicator):
     """Performance indicator based on the recovery of each component in the system.
 
     See Also
     --------
     PerformanceIndicator
 
     """
 
     def _evaluate(self, performance):
-        return - performance.recovery
+        return performance.recovery
 
 
 class Productivity(PerformanceIndicator):
     """Performance indicator based on the productivity of each component in the system.
 
     See Also
     --------
     PerformanceIndicator
 
     """
 
     def _evaluate(self, performance):
-        return - performance.productivity
+        return performance.productivity
 
 
 class EluentConsumption(PerformanceIndicator):
     """Performance indicator based on the specific eluent consumption of each component.
 
     See Also
     --------
     PerformanceIndicator
 
     """
 
     def _evaluate(self, performance):
-        return - performance.eluent_consumption
+        return performance.eluent_consumption
 
 
 class Purity(PerformanceIndicator):
     """Performance indicator based on the purity of each component in the system.
 
     See Also
     --------
     PerformanceIndicator
 
     """
 
     def _evaluate(self, performance):
-        return - performance.purity
+        return performance.purity
 
 
 class Concentration(PerformanceIndicator):
     """Performance indicator based on the concentration of each component in the system.
 
     See Also
     --------
     PerformanceIndicator
 
     """
 
     def _evaluate(self, performance):
-        return - performance.concentration
+        return performance.concentration
 
 
 class PerformanceProduct(PerformanceIndicator):
     """Performance indicator based on the product of several performance indicators.
 
     See Also
     --------
@@ -387,15 +387,15 @@
     EluentConsumption
     PerformanceIndicator
 
     """
 
     def _evaluate(self, performance):
         return \
-            - performance.productivity \
+            performance.productivity \
             * performance.recovery \
             * performance.eluent_consumption
 
 
 class MassBalanceDifference(PerformanceIndicator):
     """Performance indicator based on the mass balance of each component in the system.
```

### Comparing `CADET-Process-0.8.0/CADETProcess/processModel/__init__.py` & `CADET-Process-0.9.0/CADETProcess/processModel/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/processModel/binding.py` & `CADET-Process-0.9.0/CADETProcess/processModel/binding.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,38 +18,41 @@
 
 __all__ = [
     'BindingBaseClass',
     'NoBinding',
     'Linear',
     'Langmuir',
     'LangmuirLDF',
+    'LangmuirLDFLiquidPhase',
     'BiLangmuir',
     'BiLangmuirLDF',
     'FreundlichLDF',
     'StericMassAction',
     'AntiLangmuir',
     'Spreading',
     'MobilePhaseModulator',
     'ExtendedMobilePhaseModulator',
     'SelfAssociation',
     'BiStericMassAction',
     'MultistateStericMassAction',
     'SimplifiedMultistateStericMassAction',
     'Saska',
     'GeneralizedIonExchange',
+    'HICConstantWaterActivity',
+    'HICWaterOnHydrophobicSurfaces',
 ]
 
 
 @frozen_attributes
 class BindingBaseClass(Structure):
     """Abstract base class for parameters of binding models.
 
     Attributes
     ----------
-    name : String
+    name : str
         name of the binding model.
     component_system : ComponentSystem
         system of components.
     n_comp : int
         number of components.
     n_binding_sites : int
         Number of binding sites.
@@ -145,18 +148,18 @@
 
 
 class Linear(BindingBaseClass):
     """Parameters for Linear binding model.
 
     Attributes
     ----------
-    adsorption_rate : list of unsigned floats. Length depends on n_comp.
-        Adsorption rate constants.
-    desorption_rate : list of unsigned floats. Length depends on n_comp.
-        Desorption rate constants.
+    adsorption_rate : list of unsigned floats.
+        Adsorption rate constants. Length depends on `n_comp`.
+    desorption_rate : list of unsigned floats.
+        Desorption rate constants. Length depends on `n_comp`.
 
     """
 
     adsorption_rate = SizedUnsignedList(size='n_comp')
     desorption_rate = SizedUnsignedList(size='n_comp')
 
     _parameters = [
@@ -166,20 +169,20 @@
 
 
 class Langmuir(BindingBaseClass):
     """Parameters for Multi Component Langmuir binding model.
 
     Attributes
     ----------
-    adsorption_rate : list of unsigned floats. Length depends on n_comp.
-        Adsorption rate constants.
-    desorption_rate : list of unsigned floats. Length depends on n_comp.
-        Desorption rate constants.
-    capacity : list of unsigned floats. Length depends on n_comp.
-        Maximum adsorption capacities.
+    adsorption_rate : list of unsigned floats.
+        Adsorption rate constants. Length depends on `n_comp`.
+    desorption_rate : list of unsigned floats.
+        Desorption rate constants. Length depends on `n_comp`.
+    capacity : list of unsigned floats.
+        Maximum adsorption capacities. Length depends on `n_comp`.
 
     """
 
     adsorption_rate = SizedUnsignedList(size='n_comp')
     desorption_rate = SizedUnsignedList(size='n_comp')
     capacity = SizedUnsignedList(size='n_comp')
 
@@ -187,24 +190,51 @@
         'adsorption_rate',
         'desorption_rate',
         'capacity',
     ]
 
 
 class LangmuirLDF(BindingBaseClass):
-    """Parameters for Multi Component Langmuir binding model.
+    """Parameters for Multi Component Langmuir binding model using a linear driving
+    force approximation based on the equilibrium concentration q* for given c.
+
+    Attributes
+    ----------
+    equilibrium_constant : list of unsigned floats.
+        Adsorption rate constants. Length depends on `n_comp`.
+    driving_force_coefficient : list of unsigned floats.
+        Desorption rate constants. Length depends on `n_comp`.
+    capacity : list of unsigned floats.
+        Maximum adsorption capacities. Length depends on `n_comp`.
+
+    """
+
+    equilibrium_constant = SizedUnsignedList(size='n_comp')
+    driving_force_coefficient = SizedUnsignedList(size='n_comp')
+    capacity = SizedUnsignedList(size='n_comp')
+
+    _parameters = [
+        'equilibrium_constant',
+        'driving_force_coefficient',
+        'capacity',
+    ]
+
+
+class LangmuirLDFLiquidPhase(BindingBaseClass):
+    """Parameters for Multi Component Langmuir binding model using a linear driving
+    force approximation based on the equilibrium concentration c* for given q.
 
     Attributes
     ----------
-    equilibrium_constant : list of unsigned floats. Length depends on n_comp.
-        Adsorption rate constants.
-    driving_force_coefficient : list of unsigned floats. Length depends on n_comp.
-        Desorption rate constants
-    capacity : list of unsigned floats. Length depends on n_comp.
-        Maximum adsorption capacities.
+    equilibrium_constant : list of unsigned floats.
+        Adsorption rate constants. Length depends on `n_comp`.
+    driving_force_coefficient : list of unsigned floats.
+        Desorption rate constants. Length depends on `n_comp`.
+    capacity : list of unsigned floats.
+        Maximum adsorption capacities. Length depends on `n_comp`.
 
     """
 
     equilibrium_constant = SizedUnsignedList(size='n_comp')
     driving_force_coefficient = SizedUnsignedList(size='n_comp')
     capacity = SizedUnsignedList(size='n_comp')
 
@@ -216,20 +246,23 @@
 
 
 class BiLangmuir(BindingBaseClass):
     """Parameters for Multi Component Bi-Langmuir binding model.
 
     Attributes
     ----------
-    adsorption_rate : list of unsigned floats. Length depends on n_comp.
-        Adsorption rate constants.
-    desorption_rate : list of unsigned floats. Length depends on n_comp.
-        Desorption rate constants
-    capacity : list of unsigned floats. Length depends on n_comp.
-        Maximum adsorption capacities.
+    adsorption_rate : list of unsigned floats.
+        Adsorption rate constants in state-major ordering.
+        Length depends on `n_bound_states`.
+    desorption_rate : list of unsigned floats.
+        Desorption rate constants in state-major ordering.
+        Length depends on `n_bound_states`.
+    capacity : list of unsigned floats.
+        Maximum adsorption capacities in state-major ordering.
+        Length depends on `n_bound_states`.
 
     """
 
     n_binding_sites = UnsignedInteger(default=2)
 
     adsorption_rate = SizedUnsignedList(size='n_bound_states')
     desorption_rate = SizedUnsignedList(size='n_bound_states')
@@ -248,20 +281,23 @@
 
 
 class BiLangmuirLDF(BindingBaseClass):
     """Parameters for Multi Component Bi-Langmuir binding model.
 
     Attributes
     ----------
-    equilibrium_constant : list of unsigned floats. Length depends on n_comp.
-        Adsorption rate constants.
-    driving_force_coefficient : list of unsigned floats. Length depends on n_comp.
-        Desorption rate constants
-    capacity : list of unsigned floats. Length depends on n_comp.
-        Maximum adsorption capacities.
+    equilibrium_constant : list of unsigned floats.
+        Adsorption rate constants in state-major ordering.
+        Length depends on `n_bound_states`.
+    driving_force_coefficient : list of unsigned floats.
+        Desorption rate constants in state-major ordering.
+        Length depends on `n_bound_states`.
+    capacity : list of unsigned floats.
+        Maximum adsorption capacities in state-major ordering.
+        Length depends on `n_bound_states`.
 
     """
 
     n_binding_sites = UnsignedInteger(default=2)
 
     equilibrium_constant = SizedUnsignedList(size='n_bound_states')
     driving_force_coefficient = SizedUnsignedList(size='n_bound_states')
@@ -281,19 +317,19 @@
 
 class FreundlichLDF(BindingBaseClass):
     """Parameters for the Freundlich isotherm model.
 
     Attributes
     ----------
     driving_force_coefficient : list of unsigned floats.
-        Adsorption rate constants. Length depends on n_comp.
+        Driving force coefficient for each component. Length depends on `n_comp`.
     freundlich_coefficient : list of unsigned floats.
-        Freundlich coefficient for each component. Length depends on n_comp.
+        Freundlich coefficient for each component. Length depends on `n_comp`.
     exponent : list of unsigned floats.
-        Exponent for each component. Length depends on n_comp.
+        Freundlich exponent for each component. Length depends on `n_comp`.
 
     """
 
     driving_force_coefficient = SizedUnsignedList(size='n_comp')
     freundlich_coefficient = SizedUnsignedList(size='n_comp')
     exponent = SizedUnsignedList(size='n_comp')
 
@@ -305,25 +341,27 @@
 
 
 class StericMassAction(BindingBaseClass):
     """Parameters for Steric Mass Action Law binding model.
 
     Attributes
     ----------
-    adsorption_rate : list of unsigned floats. Length depends on n_comp.
-        Adsorption rate constants.
-    desorption_rate : list of unsigned floats. Length depends on n_comp.
-        Desorption rate constants.
-    characteristic_charge : list of unsigned floats. Length depends on n_comp.
-        The characteristic charge of the protein: The number sites v that
-        protein interacts on the resin surface.
-    steric_factor : list of unsigned floats. Length depends on n_comp.
-        Steric factors of the protein: The number of sites o on the surface
-        that are shileded by the protein and prevented from exchange with salt
+    adsorption_rate : list of unsigned floats.
+        Adsorption rate constants. Length depends on `n_comp`.
+    desorption_rate : list of unsigned floats.
+        Desorption rate constants. Length depends on `n_comp`.
+    characteristic_charge : list of unsigned floats.
+        Characteristic charges of the protein; The number of sites $\nu$ that the
+        protein interacts with on the resin surface.
+        Length depends on `n_comp`.
+    steric_factor : list of unsigned floats.
+        Steric factors of the protein: The number of sites $\sigma$ on the surface
+        that are shielded by the protein and prevented from exchange with salt
         counterions in solution.
+        Length depends on `n_comp`.
     capacity : unsigned float.
         Stationary phase capacity (monovalent salt counterions); The total
         number of binding sites available on the resin surface.
     reference_liquid_phase_conc : unsigned float.
         Reference liquid phase concentration.
         The default is 1.0
     reference_solid_phase_conc : unsigned float.
@@ -390,26 +428,26 @@
         self.desorption_rate = (
             (desorption_rate_untransformed
              / self.reference_liquid_phase_conc ** (-nu)
              ).tolist())
 
 
 class AntiLangmuir(BindingBaseClass):
-    """Multi Component Anti-Langmuir adsoprtion isotherm.
+    """Multi Component Anti-Langmuir adsorption isotherm.
 
     Attributes
     ----------
     adsorption_rate : list of unsigned floats.
-        Adsorption rate constants. Length depends on n_comp.
-    desorption_rate : list of unsigned floats. Length depends on n_comp.
-        Desorption rate constants. Length depends on n_comp.
+        Adsorption rate constants. Length depends on `n_comp`.
+    desorption_rate : list of unsigned floats
+        Desorption rate constants. Length depends on `n_comp`.
     capacity : list of unsigned floats.
-        Maximum adsorption capacities. Length depends on n_comp.
+        Maximum adsorption capacities. Length depends on `n_comp`.
     antilangmuir : list of unsigned floats, optional.
-        Anti-Langmuir coefficients. Length depends on n_comp.
+        Anti-Langmuir coefficients. Length depends on `n_comp`.
 
     """
 
     adsorption_rate = SizedUnsignedList(size='n_comp')
     desorption_rate = SizedUnsignedList(size='n_comp')
     capacity = SizedUnsignedList(size='n_comp')
     antilangmuir = SizedUnsignedList(size='n_comp')
@@ -419,28 +457,33 @@
         'desorption_rate',
         'capacity',
         'antilangmuir'
     ]
 
 
 class Spreading(BindingBaseClass):
-    """Multi Component Spreading adsoprtion isotherm.
+    """Multi Component Spreading adsorption isotherm.
 
     Attributes
     ----------
     adsorption_rate : list of unsigned floats.
-        Adsorption rate constants.
+        Adsorption rate constants in state-major ordering.
+        Length depends on `n_total_bound`.
     desorption_rate : list of unsigned floats.
-        Desorption rate constants.
+        Desorption rate constants in state-major ordering.
+        Length depends on `n_total_bound`.
     capacity : list of unsigned floats.
-        Maximum adsoprtion capacities in state-major ordering.
+        Maximum adsorption capacities in state-major ordering.
+        Length depends on `n_total_bound`.
     exchange_from_1_2 : list of unsigned floats.
         Exchange rates from the first to the second bound state.
+        Length depends on `n_comp`.
     exchange_from_2_1 : list of unsigned floats.
         Exchange rates from the second to the first bound state.
+        Length depends on `n_comp`.
 
     """
 
     n_binding_sites = RangedInteger(lb=2, ub=2, default=2)
 
     adsorption_rate = SizedUnsignedList(size='n_total_bound')
     desorption_rate = SizedUnsignedList(size='n_total_bound')
@@ -454,29 +497,30 @@
         'capacity',
         'exchange_from_1_2',
         'exchange_from_2_1'
     ]
 
 
 class MobilePhaseModulator(BindingBaseClass):
-    """Mobile Phase Modulator adsoprtion isotherm.
+    """Mobile Phase Modulator adsorption isotherm.
 
     Attributes
     ----------
     adsorption_rate : list of unsigned floats.
-        Adsorption rate constants.
+        Adsorption rate constants. Length depends on `n_comp`.
     desorption_rate : list of unsigned floats.
-        Desorption rate constants.
+        Desorption rate constants. Length depends on `n_comp`.
     capacity : list of unsigned floats.
-        Maximum adsorption capacities.
+        Maximum adsorption capacities. Length depends on `n_comp`.
     ion_exchange_characteristic : list of unsigned floats.
         Parameters describing the ion-exchange characteristics (IEX).
+        Length depends on `n_comp`.
     hydrophobicity : list of unsigned floats.
         Parameters describing the hydrophobicity (HIC).
-
+        Length depends on `n_comp`.
     """
 
     adsorption_rate = SizedUnsignedList(size='n_comp')
     desorption_rate = SizedUnsignedList(size='n_comp')
     capacity = SizedUnsignedList(size='n_comp')
     ion_exchange_characteristic = SizedUnsignedList(size='n_comp')
     beta = ion_exchange_characteristic
@@ -489,77 +533,80 @@
         'capacity',
         'ion_exchange_characteristic',
         'hydrophobicity',
     ]
 
 
 class ExtendedMobilePhaseModulator(BindingBaseClass):
-    """Mobile Phase Modulator adsoprtion isotherm.
+    """Mobile Phase Modulator adsorption isotherm.
 
     Attributes
     ----------
     adsorption_rate : list of unsigned floats.
-        Adsorption rate constants.
+        Adsorption rate constants. Length depends on `n_comp`.
     desorption_rate : list of unsigned floats.
-        Desorption rate constants.
+        Desorption rate constants. Length depends on `n_comp`.
     capacity : list of unsigned floats.
-        Maximum adsorption capacities.
+        Maximum adsorption capacities. Length depends on `n_comp`.
     ion_exchange_characteristic : list of unsigned floats.
         Parameters describing the ion-exchange characteristics (IEX).
+        Length depends on `n_comp`.
     hydrophobicity : list of unsigned floats.
         Parameters describing the hydrophobicity (HIC).
-    component_mode : list of unsigned floats.
+        Length depends on `n_comp`.
+    component_mode : list of unsigned integers.
         Mode of each component;
         0 denotes the modifier component,
         1 is linear binding,
         2 is modified Langmuir binding.
+        Length depends on `n_comp`.
 
     """
 
     adsorption_rate = SizedUnsignedList(size='n_comp')
     desorption_rate = SizedUnsignedList(size='n_comp')
     capacity = SizedUnsignedList(size='n_comp')
     ion_exchange_characteristic = SizedUnsignedList(size='n_comp')
     beta = ion_exchange_characteristic
     hydrophobicity = SizedUnsignedList(size='n_comp')
     gamma = hydrophobicity
-    component_mode = SizedUnsignedList(size='n_comp')
+    component_mode = SizedUnsignedIntegerList(size='n_comp', ub=2)
 
     _parameters = [
         'adsorption_rate',
         'desorption_rate',
         'capacity',
         'ion_exchange_characteristic',
         'hydrophobicity',
         'component_mode',
     ]
 
 
 class SelfAssociation(BindingBaseClass):
-    """Self Association adsoprtion isotherm.
+    """Self Association adsorption isotherm.
 
     Attributes
     ----------
     adsorption_rate : list of unsigned floats.
-        Adsorption rate constants.
+        Adsorption rate constants. Length depends on `n_comp`.
     adsorption_rate_dimerization : list of unsigned floats.
-        Adsorption rate constants of dimerization.
+        Adsorption rate constants of dimerization. Length depends on `n_comp`.
     desorption_rate : list of unsigned floats.
-        Desorption rate constants.
+        Desorption rate constants. Length depends on `n_comp`.
     characteristic_charge : list of unsigned floats.
-        The characteristic charge v of the protein.
+        The characteristic charge $\nu$ of the protein. Length depends on `n_comp`.
     steric_factor : list of unsigned floats.
-        Steric factor of of the protein.
+        Steric factor of of the protein. Length depends on `n_comp`.
     capacity : unsigned float.
-        Stationary phase capacity (monovalent salt counterions); The total
-        number of binding sites available on the resin surface.
-    reference_liquid_phase_conc : unsigned float
+        Stationary phase capacity (monovalent salt counterions); The total number of
+        binding sites available on the resin surface.
+    reference_liquid_phase_conc : unsigned float.
         Reference liquid phase concentration (optional, default value = 1.0).
         The default = 1.0
-    reference_solid_phase_conc : unsigned float
+    reference_solid_phase_conc : unsigned float.
         Reference liquid phase concentration (optional)
         The default = 1.0
 
     """
 
     adsorption_rate = SizedUnsignedList(size='n_comp')
     adsorption_rate_dimerization = SizedUnsignedList(size='n_comp')
@@ -579,31 +626,36 @@
         'capacity',
         'reference_liquid_phase_conc',
         'reference_solid_phase_conc'
     ]
 
 
 class BiStericMassAction(BindingBaseClass):
-    """Bi Steric Mass Action adsoprtion isotherm.
+    """Bi Steric Mass Action adsorption isotherm.
 
     Attributes
     ----------
     adsorption_rate : list of unsigned floats.
         Adsorption rate constants in state-major ordering.
+        Length depends on `n_bound_states`.
     desorption_rate : list of unsigned floats.
         Desorption rate constants in state-major ordering.
+        Length depends on `n_bound_states`.
     characteristic_charge : list of unsigned floats.
         Characteristic charges v(i,j) of the it-h protein with respect to the
         j-th binding site type in state-major ordering.
+        Length depends on `n_bound_states`.
     steric_factor : list of unsigned floats.
         Steric factor o (i,j) of the it-h protein with respect to the j-th
         binding site type in state-major ordering.
+        Length depends on `n_bound_states`.
     capacity : unsigned float.
         Stationary phase capacity (monovalent salt counterions); The total
         number of binding sites available on the resin surface.
+        Length depends on `n_binding_sites`.
     reference_liquid_phase_conc : list of unsigned floats.
         Reference liquid phase concentration for each binding site type or one
         value for all types.
         The default is 1.0
     reference_solid_phase_conc : list of unsigned floats.
         Reference solid phase concentration for each binding site type or one
         value for all types.
@@ -634,37 +686,41 @@
 
     def __init__(self, *args, n_states=2, **kwargs):
         self.n_states = n_states
         super().__init__(*args, **kwargs)
 
 
 class MultistateStericMassAction(BindingBaseClass):
-    """Multistate Steric Mass Action adsoprtion isotherm.
+    """Multistate Steric Mass Action adsorption isotherm.
 
     Attributes
     ----------
     adsorption_rate : list of unsigned floats.
-        Adsorption rate constants of the components to different bound states
-        in component-major ordering.
+        Adsorption rate constants of the components to different bound states in
+        component-major ordering.
+        Length depends on `n_bound_states`.
     desorption_rate : list of unsigned floats.
-        Desorption rate constants of the components to different bound states
-        in component-major ordering.
+        Desorption rate constants of the components to different bound states in
+        component-major ordering.
+        Length depends on `n_bound_states`.
     characteristic_charge : list of unsigned floats.
         Characteristic charges of the components to different bound states in
         component-major ordering.
+        Length depends on `n_bound_states`.
     steric_factor : list of unsigned floats.
-        Steric factor of the components to different bound states in
-        component-major ordering.
+        Steric factor of the components to different bound states in component-major
+        ordering.
+        Length depends on `n_bound_states`.
     conversion_rate : list of unsigned floats.
         Conversion rates between different bound states in
         component-major ordering.
         Length: $sum_{i=1}^{n_{comp}} n_{bound, i}$
     capacity : unsigned float.
-        Stationary phase capacity (monovalent salt counterions); The total
-        number of binding sites available on the resin surface.
+        Stationary phase capacity (monovalent salt counterions); The total number of
+        binding sites available on the resin surface.
     reference_liquid_phase_conc : unsigned float.
         Reference liquid phase concentration.
         The default = 1.0
     reference_solid_phase_conc : unsigned float, optional
         Reference solid phase concentration.
         The default = 1.0
 
@@ -693,68 +749,78 @@
         'reference_liquid_phase_conc',
         'reference_solid_phase_conc'
     ]
 
     @property
     def _conversion_entries(self):
         n = 0
-        for state in self.bound_states[1:]:
+        for state in self.bound_states:
             n += state**2
 
         return n
 
 
 class SimplifiedMultistateStericMassAction(BindingBaseClass):
-    """Simplified multistate Steric Mass Action adsoprtion isotherm.
+    """Simplified multistate Steric Mass Action adsorption isotherm.
 
     Attributes
     ----------
-    adsorption_rate :list of unsigned floats.
+    adsorption_rate : list of unsigned floats.
         Adsorption rate constants of the components to different bound states
         in component-major ordering.
+        Length depends on `n_bound_states`.
     desorption_rate : list of unsigned floats.
         Desorption rate constants of the components to different bound states
         in component-major ordering.
+        Length depends on `n_bound_states`.
     characteristic_charge_first : list of unsigned floats.
-        Characteristic charges of the components in the first (weakest) bound
-        state.
+        Characteristic charges of the components in the first (weakest) bound state.
+        Length depends on `n_comp`.
     characteristic_charge_last : list of unsigned floats.
-        Characteristic charges of the components in the last (strongest) bound
-        state.
+        Characteristic charges of the components in the last (strongest) bound state.
+        Length depends on `n_comp`.
     quadratic_modifiers_charge : list of unsigned floats.
-        Quadratic modifiers of the characteristic charges of the different
-        components depending on the index of the bound state.
+        Quadratic modifiers of the characteristic charges of the different components
+        depending on the index of the bound state.
+        Length depends on `n_comp`.
     steric_factor_first : list of unsigned floats.
         Steric factor of the components in the first (weakest) bound state.
+        Length depends on `n_comp`.
     steric_factor_last : list of unsigned floats.
         Steric factor of the components in the last (strongest) bound state.
+        Length depends on `n_comp`.
     quadratic_modifiers_steric : list of unsigned floats.
-        Quadratic modifiers of the sterif factors of the different components
-        depending on the index of the bound state.
-    capacity : unsigned floats.
-        Stationary phase capacity (monovalent salt counterions): The total
-        number of binding sites available on the resin surface.
+        Quadratic modifiers of the sterif factors of the different components depending
+        on the index of the bound state.
+        Length depends on `n_comp`.
+    capacity : unsigned float.
+        Stationary phase capacity (monovalent salt counterions): The total number of
+        binding sites available on the resin surface.
     exchange_from_weak_stronger : list of unsigned floats.
-        Exchangde rated from a weakly bound state to the next stronger bound
-        state.
+        Exchangde rated from a weakly bound state to the next stronger bound state.
     linear_exchange_ws : list of unsigned floats.
-        Linear exchange rate coefficients from a weakly bound state to the next
-        stronger bound state.
+        Linear exchange rate coefficients from a weakly bound state to the next stronger
+        bound state.
+        Length depends on `n_comp`.
     quadratic_exchange_ws : list of unsigned floats.
-        Quadratic exchange rate coefficients from a weakly bound state to the
-        next stronger bound state.
+        Quadratic exchange rate coefficients from a weakly bound state to the next
+        stronger bound state.
+        Length depends on `n_comp`.
     exchange_from_stronger_weak : list of unsigned floats.
-        Exchange rate coefficients from a strongly bound state to the next
-        weaker bound state.
+        Exchange rate coefficients from a strongly bound state to the next weaker bound
+        state.
+        Length depends on `n_comp`.
     linear_exchange_sw : list of unsigned floats.
-        Linear exchange rate coefficients from a strongly bound state to the
-        next weaker bound state.
+        Linear exchange rate coefficients from a strongly bound state to the next weaker
+        bound state.
+        Length depends on `n_comp`.
     quadratic_exchange_sw : list of unsigned floats.
-        Quadratic exchange rate coefficients from a strongly bound state to the
-        next weaker bound state.
+        Quadratic exchange rate coefficients from a strongly bound state to the next
+        weaker bound state.
+        Length depends on `n_comp`.
     reference_liquid_phase_conc : list of unsigned floats.
         Reference liquid phase concentration (optional, default value = 1.0).
     reference_solid_phase_conc : list of unsigned floats.
         Reference solid phase concentration (optional, default value = 1.0).
 
     """
 
@@ -803,17 +869,17 @@
 
 class Saska(BindingBaseClass):
     """Quadratic Isotherm.
 
     Attributes
     ----------
     henry_const : list of unsigned floats.
-        The Henry coefficient.
+        The Henry coefficient. Length depends on `n_comp`.
     quadratic_factor : list of unsigned floats.
-        Quadratic factors.
+        Quadratic factors. Length depends on `n_comp`.
 
     """
 
     henry_const = SizedUnsignedList(size='n_comp')
     quadratic_factor = SizedUnsignedList(size=('n_comp', 'n_comp'))
 
     _parameters = [
@@ -823,60 +889,77 @@
 
 
 class GeneralizedIonExchange(BindingBaseClass):
     """Generalized Ion Exchange isotherm model.
 
     Attributes
     ----------
-    adsorption_rate : list of unsigned floats. Length depends on n_comp.
-        Adsorption rate constants.
-    adsorption_rate_linear : list of unsigned floats. Length depends on n_comp.
+    adsorption_rate : list of unsigned floats.
+        Adsorption rate constants. Length depends on `n_comp`.
+    adsorption_rate_linear : list of unsigned floats.
         Linear dependence coefficient of adsorption rate on modifier component
-    adsorption_rate_quadratic : list of unsigned floats. Length depends on n_comp.
+        Length depends on `n_comp`.
+    adsorption_rate_quadratic : list of unsigned floats.
         Quadratic dependence coefficient of adsorption rate on modifier component.
-    adsorption_rate_cubic : list of unsigned floats. Length depends on n_comp.
+        Length depends on `n_comp`.
+    adsorption_rate_cubic : list of unsigned floats.
         Cubic dependence coefficient of adsorption rate on modifier component.
-    adsorption_rate_salt : list of unsigned floats. Length depends on n_comp.
+        Length depends on `n_comp`.
+    adsorption_rate_salt : list of unsigned floats.
         Salt coefficient of adsorption rate;
         difference of water-protein and salt-protein interactions.
-    adsorption_rate_protein : list of unsigned floats. Length depends on n_comp.
+        Length depends on `n_comp`.
+    adsorption_rate_protein : list of unsigned floats.
         Protein coefficient of adsorption rate;
         difference of water-protein and protein-protein interactions.
-    desorption_rate : list of unsigned floats. Length depends on n_comp.
-        Desorption rate constants.
-    desorption_rate_linear : list of unsigned floats. Length depends on n_comp.
+        Length depends on `n_comp`.
+    desorption_rate : list of unsigned floats.
+        Desorption rate constants. Length depends on `n_comp`.
+    desorption_rate_linear : list of unsigned floats.
         Linear dependence coefficient of desorption rate on modifier component.
-    desorption_rate_quadratic : list of unsigned floats. Length depends on n_comp.
+        Length depends on `n_comp`.
+    desorption_rate_quadratic : list of unsigned floats.
         Quadratic dependence coefficient of desorption rate on modifier component.
-    desorption_rate_cubic : list of unsigned floats. Length depends on n_comp.
+        Length depends on `n_comp`.
+    desorption_rate_cubic : list of unsigned floats.
         Cubic dependence coefficient of desorption rate on modifier component.
-    desorption_rate_salt : list of unsigned floats. Length depends on n_comp.
+        Length depends on `n_comp`.
+    desorption_rate_salt : list of unsigned floats.
         Salt coefficient of desorption rate;
         difference of water-protein and salt-protein interactions.
-    desorption_rate_protein : list of unsigned floats. Length depends on n_comp.
+        Length depends on `n_comp`.
+    desorption_rate_protein : list of unsigned floats.
         Protein coefficient of desorption rate;
         difference of water-protein and protein-protein interactions
-    characteristic_charge : list of unsigned floats. Length depends on n_comp.
-        The characteristic charge of the protein: The number sites v that
-        protein interacts on the resin surface.
-    characteristic_charge_linear : list of unsigned floats. Length depends on n_comp.
+        Length depends on `n_comp`.
+    characteristic_charge_breaks : list of unsigned floats, optional
+        Breaks of the characteristic charge pieces in component-major ordering.
+        Optional, only required if a piecewise cubic polynomial is used for $\nu$.
+        Length must be a multiple of `n_comp`.
+    characteristic_charge : list of unsigned floats.
+        Base value for characteristic charges of the protein; The number of sites $\nu$
+        that the protein interacts with on the resin surface.
+        Length depends on `n_comp` * `n_pieces`.
+    characteristic_charge_linear : list of unsigned floats.
         Linear dependence coefficient of characteristic charge on modifier component.
-    characteristic_charge_quadratic : list of unsigned floats. Length depends on n_comp.
+        Length depends on `n_comp` * `n_pieces`.
+    characteristic_charge_quadratic : list of unsigned floats.
         Quadratic dependence coefficient of characteristic charge on modifier component.
-    characteristic_charge_cubic : list of unsigned floats. Length depends on n_comp.
-        Cubic dependence coefficient of characteristic charge on modifier component .
-    characteristic_charge_breaks : list of unsigned floats. Length depends on n_comp.
-        Cubic dependence coefficient of characteristic charge on modifier component .
-    steric_factor : list of unsigned floats. Length depends on n_comp.
-        Steric factors of the protein: The number of sites o on the surface
-        that are shileded by the protein and prevented from exchange with salt
-        counterions in solution.
+        Length depends on `n_comp` * `n_pieces`.
+    characteristic_charge_cubic : list of unsigned floats.
+        Cubic dependence coefficient of characteristic charge on modifier component.
+        Length depends on `n_comp` * `n_pieces`.
+    steric_factor : list of unsigned floats.
+        Steric factors of the protein: The number of sites $\sigma$ on the surface that
+        are shielded by the protein and prevented from exchange with salt counterions in
+        solution.
+        Length depends on `n_comp`.
     capacity : unsigned float.
-        Stationary phase capacity (monovalent salt counterions); The total
-        number of binding sites available on the resin surface.
+        Stationary phase capacity (monovalent salt counterions); The total number of
+        binding sites available on the resin surface.
     reference_liquid_phase_conc : unsigned float.
         Reference liquid phase concentration (optional, default value = 1.0).
     reference_solid_phase_conc : unsigned float.
         Reference liquid phase concentration (optional, default value = 1.0).
 
     """
 
@@ -890,15 +973,17 @@
     adsorption_rate_protein = SizedList(size='n_comp', default=0)
     desorption_rate = SizedList(size='n_comp')
     desorption_rate_linear = SizedList(size='n_comp', default=0)
     desorption_rate_quadratic = SizedList(size='n_comp', default=0)
     desorption_rate_cubic = SizedList(size='n_comp', default=0)
     desorption_rate_salt = SizedList(size='n_comp', default=0)
     desorption_rate_protein = SizedList(size='n_comp', default=0)
-    characteristic_charge_breaks = DependentlyModulatedUnsignedList(size='n_comp')
+    characteristic_charge_breaks = DependentlyModulatedUnsignedList(
+        size='n_comp', is_optional=True
+    )
     characteristic_charge = SizedList(size=('n_pieces', 'n_comp'),)
     characteristic_charge_linear = SizedList(size=('n_pieces', 'n_comp'), default=0)
     characteristic_charge_quadratic = SizedList(size=('n_pieces', 'n_comp'), default=0)
     characteristic_charge_cubic = SizedList(size=('n_pieces', 'n_comp'), default=0)
     steric_factor = SizedUnsignedList(size='n_comp')
     capacity = UnsignedFloat()
     reference_liquid_phase_conc = UnsignedFloat(default=1)
@@ -934,7 +1019,87 @@
         if self.characteristic_charge_breaks is None:
             return 1
 
         n_pieces_all = len(self.characteristic_charge_breaks) - self.n_comp
         n_pieces_comp = int(n_pieces_all / self.n_comp)
 
         return n_pieces_comp
+
+
+class HICConstantWaterActivity(BindingBaseClass):
+    """HIC based on Constant Water Activity adsorption isotherm.
+
+    Attributes
+    ----------
+    adsorption_rate : list of unsigned floats.
+        Adsorption rate constants. Size depends on `n_comp`.
+    desorption_rate : list of unsigned floats.
+        Desorption rate constants. Size depends on `n_comp`.
+    capacity : list of unsigned floats.
+        Maximum adsorption capacities. Size depends on `n_comp`.
+    hic_characteristic : list of unsigned floats.
+        Parameters describing the number of ligands per ligand-protein interaction. Size depends on `n_comp`.
+    beta_0 : unsigned float.
+        Parameter describing the number of highly ordered water molecules that stabilize
+        the hydrophobic surfaces at infinitely diluted salt concentration.
+    beta_1 : unsigned float.
+        Parameter describing the change in the number of highly ordered water molecules that stabilize
+        the hydrophobic surfaces with respect to changes in the salt concentration.
+
+    """
+
+    adsorption_rate = SizedList(size='n_comp')
+    desorption_rate = SizedList(size='n_comp')
+    capacity = SizedList(size='n_comp')
+    hic_characteristic = SizedList(size='n_comp')
+
+    beta_0 = UnsignedFloat()
+    beta_1 = UnsignedFloat()
+
+    _parameters = [
+        'adsorption_rate',
+        'desorption_rate',
+        'hic_characteristic',
+        'capacity',
+        'beta_0',
+        'beta_1',
+    ]
+
+
+class HICWaterOnHydrophobicSurfaces(BindingBaseClass):
+    """HIC isotherm by Wang et al. based on their 2016 paper.
+
+    Attributes
+    ----------
+    adsorption_rate : list of unsigned floats.
+        Adsorption rate constants. Size depends on `n_comp`.
+    desorption_rate : list of unsigned floats.
+        Desorption rate constants. Size depends on `n_comp`.
+    capacity : list of unsigned floats.
+        Maximum adsorption capacities. Size depends on `n_comp`.
+    hic_characteristic : list of unsigned floats.
+        Parameters describing the number of ligands per ligand-protein interaction. Size depends on `n_comp`.
+    beta_0 : unsigned float.
+        Parameter describing the number of highly ordered water molecules that stabilize
+        the hydrophobic surfaces at infinitely diluted salt concentration.
+    beta_1 : unsigned float.
+        Parameter describing the change in the number of highly ordered water molecules that stabilize
+        the hydrophobic surfaces with respect to changes in the salt concentration.
+
+    """
+
+    adsorption_rate = SizedList(size='n_comp')
+    desorption_rate = SizedList(size='n_comp')
+    capacity = SizedList(size='n_comp')
+    hic_characteristic = SizedList(size='n_comp')
+
+    beta_0 = UnsignedFloat()
+    beta_1 = UnsignedFloat()
+
+    _parameters = [
+        'adsorption_rate',
+        'desorption_rate',
+        'hic_characteristic',
+        'capacity',
+        'beta_0',
+        'beta_1',
+    ]
```

### Comparing `CADET-Process-0.8.0/CADETProcess/processModel/componentSystem.py` & `CADET-Process-0.9.0/CADETProcess/processModel/componentSystem.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/processModel/discretization.py` & `CADET-Process-0.9.0/CADETProcess/processModel/discretization.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/processModel/flowSheet.py` & `CADET-Process-0.9.0/CADETProcess/processModel/flowSheet.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from collections import defaultdict
 from functools import wraps
 from warnings import warn
 
 import numpy as np
-import sympy as sym
 from addict import Dict
 
 from CADETProcess import CADETProcessError
 from CADETProcess.dataStructure import frozen_attributes
 from CADETProcess.dataStructure import Structure, UnsignedInteger, String
 from .componentSystem import ComponentSystem
 from .unitOperation import UnitBaseClass
@@ -515,19 +513,19 @@
         if state_length == 0:
             output_state = []
 
         if isinstance(state, (int, np.integer)):
             if state >= state_length:
                 raise CADETProcessError('Index exceeds destinations')
 
-            output_state = [0] * state_length
-            output_state[state] = 1
+            output_state = [0.0] * state_length
+            output_state[state] = 1.0
 
         elif isinstance(state, dict):
-            output_state = [0] * state_length
+            output_state = [0.0] * state_length
             for dest, value in state.items():
                 try:
                     assert self.connection_exists(unit, dest)
                 except AssertionError:
                     raise CADETProcessError(f'{unit} does not connect to {dest}.')
                 dest = self[dest]
                 index = self.connections[unit].destinations.index(dest)
@@ -538,38 +536,62 @@
                 raise CADETProcessError(f'Expected length {state_length}.')
 
             output_state = state
 
         else:
             raise TypeError("Output state must be integer, list or dict.")
 
-        if not np.isclose(sum(output_state), 1):
+        if state_length != 0 and not np.isclose(sum(output_state), 1):
             raise CADETProcessError('Sum of fractions must be 1')
 
         self._output_states[unit] = output_state
 
     def get_flow_rates(self, state=None):
-        """Calculate flow rate for all connections.
-
-        Optionally, an additional output state can be passed to update the
-        current output states.
+        """
+        Calculate the volumetric flow rate for all connections in the process.
 
         Parameters
         ----------
         state : Dict, optional
-            Output states
+            Updated flow rates and output states for process sections.
+            Default is None.
 
         Returns
         -------
-        flow_rates : Dict
-            Volumetric flow rate of each unit operation.
+        Dict
+            Volumetric flow rate for each unit operation.
+
+        Notes
+        -----
+        To calculate the flow rates, a system of equations is set up:
+
+        .. math::
+
+            Q_i = \sum_{j=1}^{n_{units}} q_{ji} = \sum_{j=1}^{n_{units}} Q_j * w_{ji},
+
+        where :math:`Q_i` is the total flow exiting unit :math:`i`, and :math:`w_{ij}`
+        is the percentile of the total flow of unit :math:`j` directed to unit
+        :math:`i`. If the unit is an `Inlet` or a `Cstr` with a given flow rate,
+        :math:`Q_i` is given and the system is simplified. This system is solved using
+        `numpy.linalg.solve`. Then, the individual flows :math:`q_{ji}` are extracted.
+
+        Raises
+        ------
+        CADETProcessError
+            If flow sheet connectivity matrix is singular, indicating a potential issue
+            in flow sheet configuration.
 
+        References
+        ----------
+        Forum discussion on flow rate calculation:
+        https://forum.cadet-web.de/t/improving-the-flowrate-calculation/795
         """
         flow_rates = {
-            unit.name: unit.flow_rate for unit in (self.inlets + self.cstrs)
+            unit.name: unit.flow_rate
+            for unit in (self.inlets + self.cstrs)
             if unit.flow_rate is not None
         }
 
         output_states = self.output_states
 
         if state is not None:
             for param, value in state.items():
@@ -578,185 +600,120 @@
                 param_name = param[-1]
                 if param_name == 'flow_rate':
                     flow_rates[unit_name] = value[0]
                 elif unit_name == 'output_states':
                     unit = self.units_dict[param_name]
                     output_states[unit] = list(value.ravel())
 
-        def list_factory():
-            return [0, 0, 0, 0]
-
-        destination_flow_rates = {
-            unit.name: defaultdict(list_factory) for unit in self.units
-        }
-        origin_flow_rates = {
-            unit.name: defaultdict(list_factory) for unit in self.units
-        }
+        n_units = self.number_of_units
 
-        for i in range(4):
-            solution = self.solve_flow_rates(flow_rates, output_states, i)
-            if solution is not None:
-                for unit_index, unit in enumerate(self.units):
-                    for destination in self.connections[unit].destinations:
-                        destination_index = self.get_unit_index(destination)
-                        value = float(
-                            solution[f'Q_{unit_index}_{destination_index}']
-                        )
-                        destination_flow_rates[unit.name][destination.name][i] = value
-                        origin_flow_rates[destination.name][unit.name][i] = value
+        # Setup matrix with output states.
+        w_out = np.zeros((n_units, n_units))
 
-        flow_rates = Dict()
         for unit in self.units:
-            for destination, flow_rate in destination_flow_rates[unit.name].items():
-                flow_rates[unit.name].destinations[destination] = np.array(flow_rate)
-            for origin, flow_rate in origin_flow_rates[unit.name].items():
-                flow_rates[unit.name].origins[origin] = np.array(flow_rate)
+            unit_index = self.get_unit_index(unit)
+            if unit.name in flow_rates:
+                w_out[unit_index, unit_index] = 1
+            else:
+                for origin in self.connections[unit]['origins']:
+                    o_index = self.get_unit_index(origin)
+                    local_d_index = self.connections[origin].destinations.index(unit)
+                    w_out[unit_index, o_index] = output_states[origin][local_d_index]
+                w_out[unit_index, unit_index] += -1
+
+        # Check for a singular matrix before the loop
+        if np.linalg.cond(w_out) == np.inf:
+            raise CADETProcessError(
+                "Flow sheet connectivity matrix is singular, which may be due to "
+                "unconnected units or missing flow rates. Please ensure all units are "
+                "correctly connected and all necessary flow rates are set."
+            )
 
-        for unit in self.units:
-            if not isinstance(unit, Inlet):
-                flow_rate_in = np.sum(
-                    list(flow_rates[unit.name].origins.values()), axis=0
-                )
-                flow_rates[unit.name].total_in = flow_rate_in
-            if not isinstance(unit, Outlet):
-                flow_rate_out = np.sum(
-                    list(flow_rates[unit.name].destinations.values()), axis=0
-                )
-                flow_rates[unit.name].total_out = flow_rate_out
+        # Solve system of equations for each polynomial coefficient
+        total_flow_rate_coefficents = np.zeros((4, n_units))
+        for i in range(4):
+            if len(flow_rates) == 0:
+                continue
 
-        return flow_rates
+            coeffs = np.array(list(flow_rates.values()), ndmin=2)[:, i]
+            if not np.any(coeffs):
+                continue
 
-    def solve_flow_rates(self, inlet_flow_rates, output_states, coeff=0):
-        """Solve flow rates of system using sympy.
+            Q_vec = np.zeros(n_units)
+            for unit_name in flow_rates:
+                unit_index = self.get_unit_index(self.units_dict[unit_name])
+                Q_vec[unit_index] = flow_rates[unit_name][i]
+            try:
+                total_flow_rate_coefficents[i, :] = np.linalg.solve(w_out, Q_vec)
+            except np.linalg.LinAlgError:
+                raise CADETProcessError(
+                    "Unexpected error in flow rate calculation. "
+                    "Please check the flow sheet setup."
+                )
 
-        Because a simple 'push' algorithm cannot be used when closed loops are
-        present in a FlowSheet (e.g. SMBs), sympy is used to set up and solve
-        the system of equations.
+        # w_out_help is the same as w_out but it contains the origin flow for every unit
+        w_out_help = np.zeros((n_units, n_units))
 
-        Parameters
-        ----------
-        inlet_flow_rates: dict
-            Flow rates of Inlet UnitOperations.
-        output_states: dict
-            Output states of all UnitOperations.
-        coeff: int
-            Polynomial coefficient of flow rates to be solved.
+        for unit in self.connections:
+            unit_index = self.get_unit_index(unit)
+            for origin in self.connections[unit]['origins']:
+                o_index = self.get_unit_index(origin)
+                local_d_index = self.connections[origin].destinations.index(unit)
+                w_out_help[unit_index, o_index] = output_states[origin][local_d_index]
+
+        # Calculate total_in as a matrix in "one" step rather than iterating manually.
+        total_in_matrix = w_out_help @ total_flow_rate_coefficents.T
+
+        # Generate output dict
+        return_flow_rates = Dict()
+        for index, unit in enumerate(self.units):
+            unit_solution_dict = Dict()
 
-        Returns
-        -------
-        solution : dict
-            Solution of the flow rates in the system
+            if not isinstance(unit, Inlet):
+                unit_solution_dict['total_in'] = list(total_in_matrix[index])
 
-        Notes
-        -----
-            Since dynamic flow rates can be described as cubic polynomials, the
-            flow rates are solved individually for all coefficients.
-            To comply to the interface, the flow rates are always computed for the first
-            (constant) coefficient. For higher orders, the function returns None if all
-            coefficients are zero.
-
-            The problem could definitely be solved more elegantly (and efficiently) by
-            using proper liner algebra.
-        """
-        if len(inlet_flow_rates) == 0:
-            return None
-
-        coeffs = np.array(list(inlet_flow_rates.values()), ndmin=2)[:, coeff]
-        if coeff > 0 and not np.any(coeffs):
-            return None
-
-        # Setup lists for symbols
-        unit_total_flow_symbols = sym.symbols(
-            f'Q_total_0:{self.number_of_units}'
-        )
-        unit_inflow_symbols = []
-        unit_outflow_symbols = []
-
-        unit_total_flow_eq = []
-        unit_outflow_eq = []
-
-        # Setup symbolic equations
-        for unit_index, unit in enumerate(self.units):
-            if \
-                    isinstance(unit, Inlet) or \
-                    isinstance(unit, Cstr) and (
-                        unit.flow_rate is not None
-                        or
-                        unit.name in inlet_flow_rates
-                    ):
-                unit_total_flow_eq.append(
-                    sym.Add(
-                        unit_total_flow_symbols[unit_index],
-                        - float(inlet_flow_rates[unit.name][coeff])
-                    )
-                )
-            else:
-                unit_i_inflow_symbols = []
+            if not isinstance(unit, Outlet):
+                unit_solution_dict['total_out'] = list(total_flow_rate_coefficents[:, index])
 
-                for origin in self.connections[unit].origins:
-                    origin_index = self.get_unit_index(origin)
-                    unit_i_inflow_symbols.append(
-                        sym.symbols(f'Q_{origin_index}_{unit_index}')
-                    )
-
-                symbols = (
-                    *unit_i_inflow_symbols,
-                    -unit_total_flow_symbols[unit_index]
+            if not isinstance(unit, Inlet):
+                unit_solution_dict['origins'] = Dict(
+                    {
+                        origin.name: list(
+                            total_flow_rate_coefficents[:, self.get_unit_index(origin)]
+                            * w_out_help[index, self.get_unit_index(origin)]
+                        )
+                        for origin in self.connections[unit].origins
+                    }
                 )
-                unit_i_total_flow_eq = sym.Add(*symbols)
-
-                unit_inflow_symbols += unit_i_inflow_symbols
-                unit_total_flow_eq.append(unit_i_total_flow_eq)
 
             if not isinstance(unit, Outlet):
-                output_state = output_states[unit]
-                unit_i_outflow_symbols = []
-
-                for destination in self.connections[unit].destinations:
-                    destination_index = self.get_unit_index(destination)
-                    unit_i_outflow_symbols.append(
-                        sym.symbols(f'Q_{unit_index}_{destination_index}')
-                    )
-
-                unit_i_outflow_eq = [
-                    sym.Add(
-                        unit_i_outflow_symbols[dest],
-                        -unit_total_flow_symbols[unit_index]*output_state[dest]
-                    )
-                    for dest in range(len(self.connections[unit].destinations))
-                ]
-
-                unit_outflow_symbols += unit_i_outflow_symbols
-                unit_outflow_eq += unit_i_outflow_eq
-
-        # Solve system of equations
-        symbols = (
-            *unit_total_flow_symbols,
-            *unit_inflow_symbols,
-            *unit_outflow_symbols
-        )
-        symbols = set(symbols)
+                unit_solution_dict['destinations'] = Dict(
+                    {
+                        destination.name: list(
+                            total_flow_rate_coefficents[:, index]
+                            * w_out_help[self.get_unit_index(destination), index]
+                        )
+                        for destination in self.connections[unit].destinations
+                    }
+                )
 
-        solution = sym.solve(unit_total_flow_eq + unit_outflow_eq, symbols)
-        solution = {str(key): value for key, value in solution.items()}
+            return_flow_rates[unit.name] = unit_solution_dict
 
-        return solution
+        return return_flow_rates
 
     def check_flow_rates(self, state=None):
         flow_rates = self.get_flow_rates(state)
         for unit, q in flow_rates.items():
             if isinstance(unit, (Inlet, Outlet)):
                 continue
             elif isinstance(unit, Cstr) and Cstr.flow_rate is not None:
                 continue
 
             if not np.all(q.total_in == q.total_out):
-                raise CADETProcessError(
-                    f"Unbalanced flow rate for unit '{unit}'."
-                )
+                raise CADETProcessError(f"Unbalanced flow rate for unit '{unit}'.")
 
     @property
     def feed_inlets(self):
         """list: Inlets considered for calculating recovery yield."""
         return self._feed_inlets
 
     @unit_name_decorator
```

### Comparing `CADET-Process-0.8.0/CADETProcess/processModel/process.py` & `CADET-Process-0.9.0/CADETProcess/processModel/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     def V_eluent(self):
         """float: Volume of the eluent entering the system in one cycle."""
         flow_rate_timelines = self.flow_rate_timelines
 
         V_all = 0
         for eluent in self.flow_sheet.eluent_inlets:
             eluent_time_line = flow_rate_timelines[eluent.name]['total_out']
-            V_eluent = eluent_time_line.integral()
+            V_eluent = eluent_time_line.integral().squeeze()
             V_all += V_eluent
 
         return float(V_all)
 
     @cached_property_if_locked
     def V_solid(self):
         """float: Volume of all solid phase material used in flow sheet."""
@@ -681,14 +681,16 @@
         -------
         flag : bool
             False if any of the CSTRs run empty. True otherwise.
 
         """
         flag = True
         for cstr in self.flow_sheet.cstrs:
+            if cstr.flow_rate is None:
+                continue
             V_0 = cstr.V
             V_in = self.flow_rate_timelines[cstr.name].total_in.integral()
             V_out = self.flow_rate_timelines[cstr.name].total_out.integral()
             if V_0 + V_in - V_out < 0:
                 flag = False
                 warn(f'CSTR {cstr.name} runs empty during process.')
```

### Comparing `CADET-Process-0.8.0/CADETProcess/processModel/reaction.py` & `CADET-Process-0.9.0/CADETProcess/processModel/reaction.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/processModel/solutionRecorder.py` & `CADET-Process-0.9.0/CADETProcess/processModel/solutionRecorder.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/processModel/unitOperation.py` & `CADET-Process-0.9.0/CADETProcess/processModel/unitOperation.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 __all__ = [
     'UnitBaseClass',
     'SourceMixin',
     'SinkMixin',
     'Inlet',
     'Outlet',
+    'Cstr',
     'TubularReactorBase',
     'TubularReactor',
     'LumpedRateModelWithoutPores',
     'LumpedRateModelWithPores',
     'GeneralRateModel',
 ]
 
@@ -1032,16 +1033,16 @@
     ----------
     c : List of unsigned floats. Length depends on n_comp
         Initial concentration of the reactor.
     q : List of unsigned floats. Length depends on n_comp
         Initial concentration of the bound phase.
     V : unsigned float
         Initial volume of the reactor.
-    total_porosity : UnsignedFloat between 0 and 1.
-        Total porosity of the column.
+    porosity : UnsignedFloat between 0 and 1.
+        Total porosity of the Cstr.
     flow_rate_filter: float
         Flow rate of pure liquid without components to reduce volume.
     solution_recorder : CSTRRecorder
         Solution recorder for the unit operation.
 
     Notes
     -----
```

### Comparing `CADET-Process-0.8.0/CADETProcess/reference.py` & `CADET-Process-0.9.0/CADETProcess/reference.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         Parameters
         ----------
         name : str
             The name of the reference.
         time : array-like
             The time points for the reference.
         solution : array-like
-            The reference solution values.
+            The reference solution values with shape = (n_time, n_comp).
         flow_rate : array-like or float, optional
             The flow rates for the reference.
             If not provided, flow rate of 1 is assumed.
         component_system : ComponentSystem, optional
             The reference component system.
             If not provided, a ComponentSystem with the same number of components as the
             solution is created.
@@ -87,14 +87,20 @@
             If the provided time, solution, or flow rate are not array-like.
         ValueError
             If the time and solution arrays are not the same length.
             If the flow rate array and time array are not the same length.
 
         """
         time = np.array(time, dtype=np.float64).reshape(-1)
+
+        if solution.shape[0] != len(time):
+            raise ValueError(
+                "Solution had the wrong shape. Solution needs the shape (time, n_comp)."
+            )
+
         solution = np.array(solution, ndmin=2, dtype=np.float64).reshape(len(time), -1)
 
         if component_system is None:
             n_comp = solution.shape[1]
             component_system = ComponentSystem(n_comp)
 
         if flow_rate is None:
```

### Comparing `CADET-Process-0.8.0/CADETProcess/settings.py` & `CADET-Process-0.9.0/CADETProcess/settings.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/simulationResults.py` & `CADET-Process-0.9.0/CADETProcess/simulationResults.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 
 """
 
 import copy
 import os
 
 import numpy as np
-import addict
+from addict import Dict
 
 from CADETProcess import CADETProcessError
 from CADETProcess import settings
 from CADETProcess.dataStructure import Structure
 from CADETProcess.dataStructure import (
-    Dict, String, List, UnsignedInteger, UnsignedFloat
+    Dictionary, String, List, UnsignedInteger, UnsignedFloat
 )
 
 
 __all__ = ['SimulationResults']
 
 
 class SimulationResults(Structure):
@@ -68,21 +68,21 @@
     -----
         Ideally, the final state for each unit operation should be saved.
         However, CADET does currently provide this functionality.
 
     """
 
     solver_name = String()
-    solver_parameters = Dict()
+    solver_parameters = Dictionary()
     exit_flag = UnsignedInteger()
     exit_message = String()
     time_elapsed = UnsignedFloat()
-    solution_cycles = Dict()
-    sensitivity_cycles = Dict()
-    system_state = Dict()
+    solution_cycles = Dictionary()
+    sensitivity_cycles = Dictionary()
+    system_state = Dictionary()
     chromatograms = List()
 
     def __init__(
             self,
             solver_name, solver_parameters,
             exit_flag, exit_message, time_elapsed,
             process,
@@ -136,15 +136,15 @@
     def solution(self):
         """Construct complete solution from individual cyles."""
         if self._solution is not None:
             return self._solution
 
         time_complete = self.time_complete
 
-        solution = addict.Dict()
+        solution = Dict()
         for unit, solutions in self.solution_cycles.items():
             for sol, cycles in solutions.items():
                 solution[unit][sol] = copy.deepcopy(cycles[0])
                 solution_complete = cycles[0].solution_original
                 for i in range(1, self.n_cycles):
                     solution_complete = np.vstack((
                         solution_complete, cycles[i].solution_original[1:]
@@ -161,15 +161,15 @@
     def sensitivity(self):
         """Construct complete sensitivity from individual cyles."""
         if self._sensitivity is not None:
             return self._sensitivity
 
         time_complete = self.time_complete
 
-        sensitivity = addict.Dict()
+        sensitivity = Dict()
         for unit, sensitivities in self.sensitivity_cycles.items():
             for sens_name, sensitivities in sensitivities.items():
                 for sens, cycles in sensitivities.items():
                     sensitivity[unit][sens_name][sens] = copy.deepcopy(cycles[0])
                     sensitivity_complete = cycles[0].solution_original
                     for i in range(1, self.n_cycles):
                         sensitivity_complete = np.vstack((
```

### Comparing `CADET-Process-0.8.0/CADETProcess/simulator/__init__.py` & `CADET-Process-0.9.0/CADETProcess/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/simulator/cadetAdapter.py` & `CADET-Process-0.9.0/CADETProcess/simulator/cadetAdapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1424,14 +1424,23 @@
         'parameters': {
             'IS_KINETIC': 'is_kinetic',
             'MCLLDF_KEQ': 'equilibrium_constant',
             'MCLLDF_KKIN': 'driving_force_coefficient',
             'MCLLDF_QMAX': 'capacity'
         },
     },
+    'LangmuirLDFLiquidPhase': {
+        'name': 'MULTI_COMPONENT_LANGMUIR_LDF_LIQUID_PHASE',
+        'parameters': {
+            'IS_KINETIC': 'is_kinetic',
+            'MCLLDFC_KEQ': 'equilibrium_constant',
+            'MCLLDFC_KKIN': 'driving_force_coefficient',
+            'MCLLDFC_QMAX': 'capacity'
+        },
+    },
     'BiLangmuir': {
         'name': 'MULTI_COMPONENT_BILANGMUIR',
         'parameters': {
             'IS_KINETIC': 'is_kinetic',
             'MCBL_KA': 'adsorption_rate',
             'MCBL_KD': 'desorption_rate',
             'MCBL_QMAX': 'capacity'
@@ -1606,15 +1615,39 @@
             'GIEX_NU_QUAD': 'characteristic_charge_quadratic',
             'GIEX_NU_CUBE': 'characteristic_charge_cubic',
             'GIEX_SIGMA': 'steric_factor',
             'GIEX_LAMBDA': 'capacity',
             'GIEX_REFC0': 'reference_liquid_phase_conc',
             'GIEX_REFQ': 'reference_solid_phase_conc',
         },
-    }
+    },
+    'HICConstantWaterActivity': {
+        'name': 'HIC_CONSTANT_WATER_ACTIVITY',
+        'parameters': {
+            'IS_KINETIC': 'is_kinetic',
+            'HICCWA_KA': 'adsorption_rate',
+            'HICCWA_KD': 'desorption_rate',
+            'HICCWA_NU': 'hic_characteristic',
+            'HICCWA_QMAX': 'capacity',
+            'HICCWA_BETA0': 'beta_0',
+            'HICCWA_BETA1': 'beta_1',
+        },
+    },
+    'HICWaterOnHydrophobicSurfaces': {
+        'name': 'HIC_WATER_ON_HYDROPHOBIC_SURFACES',
+        'parameters': {
+            'IS_KINETIC': 'is_kinetic',
+            'HICWHS_KA': 'adsorption_rate',
+            'HICWHS_KD': 'desorption_rate',
+            'HICWHS_NU': 'hic_characteristic',
+            'HICWHS_QMAX': 'capacity',
+            'HICWHS_BETA0': 'beta_0',
+            'HICWHS_BETA1': 'beta_1',
+        },
+    },
 }
 
 inv_adsorption_parameters_map = {
     model: {
         'name': values['name'],
         'parameters': {
             v: k for k, v in values['parameters'].items()
```

### Comparing `CADET-Process-0.8.0/CADETProcess/simulator/simulator.py` & `CADET-Process-0.9.0/CADETProcess/simulator/simulator.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/smoothing.py` & `CADET-Process-0.9.0/CADETProcess/smoothing.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/smoothing2.py` & `CADET-Process-0.9.0/CADETProcess/smoothing2.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/solution.py` & `CADET-Process-0.9.0/CADETProcess/solution.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,14 +210,17 @@
         with np.errstate(divide='ignore', invalid='ignore'):
             purity = solution/c_total
 
         purity = np.nan_to_num(purity)
 
         return purity
 
+    def __str__(self):
+        return self.name
+
 
 class SolutionIO(SolutionBase):
     """Solution representing streams at the inlet or outlet of a ``UnitOperation``.
 
     Notes
     -----
     The `flow_rate` attribute is implemented as TimeLine to improve interpolation of
@@ -502,15 +505,15 @@
         fraction_volume : np.ndarray
             Volume of the fraction
 
         """
         if end is None:
             end = self.cycle_time
 
-        return float(self.flow_rate.integral(start, end))
+        return float(self.flow_rate.integral(start, end).squeeze())
 
     @plotting.create_and_save_figure
     def plot(
             self,
             start=None,
             end=None,
             components=None,
```

### Comparing `CADET-Process-0.8.0/CADETProcess/stationarity.py` & `CADET-Process-0.9.0/CADETProcess/stationarity.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/CADETProcess/tools/yamamoto.py` & `CADET-Process-0.9.0/CADETProcess/tools/yamamoto.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,11 +251,11 @@
     """
     bounds = ((0, 1e-10), (1000, 1000))
 
     def yamamoto_wrapper(c_s, nu, k_eq):
         return yamamoto_equation(c_s, lambda_, nu, k_eq)
 
     results, pcov = curve_fit(
-        yamamoto_wrapper, log_c_salt_at_max_M, log_gradient_slope, bounds=bounds
+        yamamoto_wrapper, log_c_salt_at_max_M, log_gradient_slope, bounds=bounds, p0=(1, 1)
     )
 
     return results
```

### Comparing `CADET-Process-0.8.0/CADETProcess/transform.py` & `CADET-Process-0.9.0/CADETProcess/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,17 @@
     AutoTransform
 
 """
 
 from abc import ABC, abstractmethod, abstractproperty
 
 import numpy as np
+import matplotlib.pyplot as plt
+
+from CADETProcess import plotting
 
 
 class TransformBase(ABC):
     """
     Base class for parameter transformation.
 
     This class provides an interface for transforming an input parameter space to some
@@ -52,15 +55,15 @@
     ------
     ValueError
         If lb_input and ub_input have different shapes.
 
     Notes
     -----
     - This is an abstract base class and cannot be instantiated directly.
-    - The `transform` method is not implemented in this class and must be implemented by a subclass.
+    - The `transform` method must be implemented by a subclass.
 
     Examples
     --------
     >>> class MyTransform(TransformBase):
     ...     def transform(self, x):
     ...         return x ** 2
     ...
@@ -225,14 +228,42 @@
         Returns
         -------
         {float, array}
             Transformed parameter values.
         """
         pass
 
+    @plotting.create_and_save_figure
+    def plot(self, ax, use_log_scale=False):
+        """
+        Plot the transformed space against the input space.
+
+        Parameters
+        ----------
+        ax : matplotlib.axes.Axes
+            The axes object to plot on.
+        use_log_scale : bool, optional
+            If True, use a logarithmic scale for the x-axis.
+        """
+        allow_extended_input = self.allow_extended_input
+        self.allow_extended_input = True
+
+        y = np.linspace(self.lb, self.ub)
+        x = self.untransform(y)
+
+        ax.plot(x, y)
+
+        ax.set_xlabel('Input Space')
+        ax.set_ylabel('Transformed Space')
+
+        if use_log_scale:
+            ax.set_xscale('log')
+
+        self.allow_extended_input = allow_extended_input
+
     def __str__(self):
         """Return the class name as a string."""
         return self.__class__.__name__
 
 
 class NoTransform(TransformBase):
     """A class that implements no transformation.
@@ -403,15 +434,15 @@
             The input value(s) to be transformed.
 
         Returns
         -------
         {float, array-like}
             The transformed output value(s).
         """
-        if self.lb_input < 0:
+        if self.lb_input <= 0:
             return \
                 np.exp(x * np.log(self.ub_input - self.lb_input + 1)) \
                 + self.lb_input - 1
         else:
             return \
                 self.lb_input * np.exp(x * np.log(self.ub_input/self.lb_input))
```

### Comparing `CADET-Process-0.8.0/CADET_Process.egg-info/PKG-INFO` & `CADET-Process-0.9.0/CADET_Process.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 Metadata-Version: 2.1
 Name: CADET-Process
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Framework for Modelling and Optimizing Advanced Chromatographic Processes
 Home-page: https://github.com/fau-advanced-separations/CADET-Process
 Author: Johannes Schmölder
 Author-email: j.schmoelder@fz-juelich.de
 Project-URL: Bug Tracker, https://github.com/fau-advanced-separations/CADET-Process/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE
+License-File: LICENSE.md
 Requires-Dist: numpy>=1.21
 Requires-Dist: scipy>=1.11
 Requires-Dist: matplotlib>=3.4
 Requires-Dist: corner>=2.2.1
 Requires-Dist: sympy>=1.8
 Requires-Dist: pathos>=0.2.8
 Requires-Dist: addict==2.3
 Requires-Dist: cadet-python>=0.14
-Requires-Dist: hopsy>=1.3.0
+Requires-Dist: hopsy>=1.4.0
 Requires-Dist: pymoo>=0.6
 Requires-Dist: numba>=0.55.1
 Requires-Dist: diskcache>=5.4.0
 Requires-Dist: joblib>=1.3.0
+Requires-Dist: psutil>=5.9.8
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: certifi; extra == "testing"
 Requires-Dist: pre-commit; extra == "testing"
 Requires-Dist: flake8; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: ax-platform>=0.3.5; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx>=5.3.0; extra == "docs"
 Requires-Dist: sphinxcontrib-bibtex>=2.5.0; extra == "docs"
 Requires-Dist: sphinx_book_theme>=1.0.0; extra == "docs"
 Requires-Dist: sphinx_copybutton>=0.5.1; extra == "docs"
 Requires-Dist: sphinx-sitemap>=2.5.0; extra == "docs"
 Requires-Dist: numpydoc>=1.5.0; extra == "docs"
 Requires-Dist: myst-nb>=0.17.1; extra == "docs"
+Provides-Extra: ax
+Requires-Dist: ax-platform>=0.3.5; extra == "ax"
 
 # CADET-Process
 
 The [**CADET**](https://cadet.github.io) core simulator is a very powerful numerical engine that can simulate a large variety of physico-chemical models used in chromatography and other biochemical processes.
 However, the configuration files of **CADET** can be complex and difficult to work with.
 This is especially relevant when multiple unit operations are involved which is often the case for complex integrated processes.
 Moreover, the structure of the configuration file may change during process optimization, for example when the order of dynamic events changes, making the direct use of **CADET** impossible without another layer of abstraction.
@@ -74,29 +79,38 @@
   volume  = {8},
   journal = {Processes},
   year    = {2020},
 }
 ```
 
 ## Installation
+
 **CADET-Process** can be installed with the following command:
 
 ```
 pip install CADET-Process
 ```
 
 To use **CADET-Process**, make sure, that **CADET** is also installed.
 This can for example be done using [conda](https://docs.conda.io/en/latest/):
+
 ```
 conda install -c conda-forge cadet
 ```
+
 For more information, see the [CADET Documentation](https://cadet.github.io/master/getting_started/installation.html).
 
 ## Free software
-CADET-Process is free software: you can redistribute it and/or modify it under the terms of the [GNU General Public License version 3](https://github.com/fau-advanced-separations/CADET-Process/blob/master/LICENSE).
+
+CADET-Process is free software: you can redistribute it and/or modify it under the terms of the [GNU General Public License version 3](https://github.com/fau-advanced-separations/CADET-Process/blob/master/LICENSE.md).
 
 ## Note
+
 This software is work in progress and being actively developed.
 Breaking changes and extensive restructuring may occur in any commit and release.
 If you encounter problems or if you have questions, feel free to ask for support in the [**CADET-Forum**](https://forum.cadet-web.de).
 Please report any bugs that you find [here](https://github.com/fau-advanced-separations/CADET-Process/issues).
 Pull requests on [GitHub](https://github.com/fau-advanced-separations/CADET-Process) are also welcome.
+
+## Acknowledgments
+
+Please refer to the [list of contributors](CONTRIBUTORS.md) who helped building and funding this project.
```

### Comparing `CADET-Process-0.8.0/CADET_Process.egg-info/SOURCES.txt` & `CADET-Process-0.9.0/CADET_Process.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-LICENSE
+LICENSE.md
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 CADETProcess/CADETProcessError.py
 CADETProcess/__init__.py
 CADETProcess/log.py
@@ -12,14 +12,15 @@
 CADETProcess/reference.py
 CADETProcess/settings.py
 CADETProcess/simulationResults.py
 CADETProcess/smoothing.py
 CADETProcess/smoothing2.py
 CADETProcess/solution.py
 CADETProcess/stationarity.py
+CADETProcess/sysinfo.py
 CADETProcess/transform.py
 CADETProcess/comparison/__init__.py
 CADETProcess/comparison/comparator.py
 CADETProcess/comparison/difference.py
 CADETProcess/comparison/peaks.py
 CADETProcess/comparison/shape.py
 CADETProcess/dataStructure/__init__.py
@@ -43,14 +44,15 @@
 CADETProcess/fractionation/fractionationOptimizer.py
 CADETProcess/fractionation/fractionator.py
 CADETProcess/fractionation/fractions.py
 CADETProcess/modelBuilder/__init__.py
 CADETProcess/modelBuilder/carouselBuilder.py
 CADETProcess/modelBuilder/compartmentBuilder.py
 CADETProcess/optimization/__init__.py
+CADETProcess/optimization/axAdapater.py
 CADETProcess/optimization/cache.py
 CADETProcess/optimization/individual.py
 CADETProcess/optimization/optimizationProblem.py
 CADETProcess/optimization/optimizer.py
 CADETProcess/optimization/parallelizationBackend.py
 CADETProcess/optimization/population.py
 CADETProcess/optimization/pymooAdapter.py
@@ -76,22 +78,24 @@
 CADET_Process.egg-info/requires.txt
 CADET_Process.egg-info/top_level.txt
 examples/__init__.py
 examples/batch_elution/__init__.py
 examples/batch_elution/optimization_multi.py
 examples/batch_elution/optimization_single.py
 examples/batch_elution/process.py
+examples/characterize_chromatographic_system/Yamamoto_method.py
 examples/characterize_chromatographic_system/__init__.py
 examples/characterize_chromatographic_system/binding_model_parameters.py
 examples/characterize_chromatographic_system/column_transport_parameters.py
 examples/characterize_chromatographic_system/particle_porosity.py
 examples/characterize_chromatographic_system/system_periphery.py
 examples/load_wash_elute/__init__.py
 examples/load_wash_elute/lwe_concentration.py
 examples/load_wash_elute/lwe_flow_rate.py
+examples/load_wash_elute/lwe_hic.py
 examples/recycling/__init__.py
 examples/recycling/clr_process.py
 examples/recycling/mrssr_process.py
 tests/__init__.py
 tests/optimization_problem_fixtures.py
 tests/test_binding.py
 tests/test_buffer_capacity.py
@@ -106,14 +110,15 @@
 tests/test_events.py
 tests/test_flow_sheet.py
 tests/test_fractions.py
 tests/test_individual.py
 tests/test_optimization_integration.py
 tests/test_optimization_problem.py
 tests/test_optimization_results.py
+tests/test_optimizer_behavior.py
 tests/test_parallelization_adapter.py
 tests/test_parameters.py
 tests/test_performance.py
 tests/test_population.py
 tests/test_process.py
 tests/test_pymoo.py
 tests/test_reaction.py
```

### Comparing `CADET-Process-0.8.0/LICENSE` & `CADET-Process-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/PKG-INFO` & `CADET-Process-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 Metadata-Version: 2.1
 Name: CADET-Process
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Framework for Modelling and Optimizing Advanced Chromatographic Processes
 Home-page: https://github.com/fau-advanced-separations/CADET-Process
 Author: Johannes Schmölder
 Author-email: j.schmoelder@fz-juelich.de
 Project-URL: Bug Tracker, https://github.com/fau-advanced-separations/CADET-Process/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE
+License-File: LICENSE.md
 Requires-Dist: numpy>=1.21
 Requires-Dist: scipy>=1.11
 Requires-Dist: matplotlib>=3.4
 Requires-Dist: corner>=2.2.1
 Requires-Dist: sympy>=1.8
 Requires-Dist: pathos>=0.2.8
 Requires-Dist: addict==2.3
 Requires-Dist: cadet-python>=0.14
-Requires-Dist: hopsy>=1.3.0
+Requires-Dist: hopsy>=1.4.0
 Requires-Dist: pymoo>=0.6
 Requires-Dist: numba>=0.55.1
 Requires-Dist: diskcache>=5.4.0
 Requires-Dist: joblib>=1.3.0
+Requires-Dist: psutil>=5.9.8
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: certifi; extra == "testing"
 Requires-Dist: pre-commit; extra == "testing"
 Requires-Dist: flake8; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: ax-platform>=0.3.5; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx>=5.3.0; extra == "docs"
 Requires-Dist: sphinxcontrib-bibtex>=2.5.0; extra == "docs"
 Requires-Dist: sphinx_book_theme>=1.0.0; extra == "docs"
 Requires-Dist: sphinx_copybutton>=0.5.1; extra == "docs"
 Requires-Dist: sphinx-sitemap>=2.5.0; extra == "docs"
 Requires-Dist: numpydoc>=1.5.0; extra == "docs"
 Requires-Dist: myst-nb>=0.17.1; extra == "docs"
+Provides-Extra: ax
+Requires-Dist: ax-platform>=0.3.5; extra == "ax"
 
 # CADET-Process
 
 The [**CADET**](https://cadet.github.io) core simulator is a very powerful numerical engine that can simulate a large variety of physico-chemical models used in chromatography and other biochemical processes.
 However, the configuration files of **CADET** can be complex and difficult to work with.
 This is especially relevant when multiple unit operations are involved which is often the case for complex integrated processes.
 Moreover, the structure of the configuration file may change during process optimization, for example when the order of dynamic events changes, making the direct use of **CADET** impossible without another layer of abstraction.
@@ -74,29 +79,38 @@
   volume  = {8},
   journal = {Processes},
   year    = {2020},
 }
 ```
 
 ## Installation
+
 **CADET-Process** can be installed with the following command:
 
 ```
 pip install CADET-Process
 ```
 
 To use **CADET-Process**, make sure, that **CADET** is also installed.
 This can for example be done using [conda](https://docs.conda.io/en/latest/):
+
 ```
 conda install -c conda-forge cadet
 ```
+
 For more information, see the [CADET Documentation](https://cadet.github.io/master/getting_started/installation.html).
 
 ## Free software
-CADET-Process is free software: you can redistribute it and/or modify it under the terms of the [GNU General Public License version 3](https://github.com/fau-advanced-separations/CADET-Process/blob/master/LICENSE).
+
+CADET-Process is free software: you can redistribute it and/or modify it under the terms of the [GNU General Public License version 3](https://github.com/fau-advanced-separations/CADET-Process/blob/master/LICENSE.md).
 
 ## Note
+
 This software is work in progress and being actively developed.
 Breaking changes and extensive restructuring may occur in any commit and release.
 If you encounter problems or if you have questions, feel free to ask for support in the [**CADET-Forum**](https://forum.cadet-web.de).
 Please report any bugs that you find [here](https://github.com/fau-advanced-separations/CADET-Process/issues).
 Pull requests on [GitHub](https://github.com/fau-advanced-separations/CADET-Process) are also welcome.
+
+## Acknowledgments
+
+Please refer to the [list of contributors](CONTRIBUTORS.md) who helped building and funding this project.
```

### Comparing `CADET-Process-0.8.0/README.md` & `CADET-Process-0.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -33,29 +33,38 @@
   volume  = {8},
   journal = {Processes},
   year    = {2020},
 }
 ```
 
 ## Installation
+
 **CADET-Process** can be installed with the following command:
 
 ```
 pip install CADET-Process
 ```
 
 To use **CADET-Process**, make sure, that **CADET** is also installed.
 This can for example be done using [conda](https://docs.conda.io/en/latest/):
+
 ```
 conda install -c conda-forge cadet
 ```
+
 For more information, see the [CADET Documentation](https://cadet.github.io/master/getting_started/installation.html).
 
 ## Free software
-CADET-Process is free software: you can redistribute it and/or modify it under the terms of the [GNU General Public License version 3](https://github.com/fau-advanced-separations/CADET-Process/blob/master/LICENSE).
+
+CADET-Process is free software: you can redistribute it and/or modify it under the terms of the [GNU General Public License version 3](https://github.com/fau-advanced-separations/CADET-Process/blob/master/LICENSE.md).
 
 ## Note
+
 This software is work in progress and being actively developed.
 Breaking changes and extensive restructuring may occur in any commit and release.
 If you encounter problems or if you have questions, feel free to ask for support in the [**CADET-Forum**](https://forum.cadet-web.de).
 Please report any bugs that you find [here](https://github.com/fau-advanced-separations/CADET-Process/issues).
 Pull requests on [GitHub](https://github.com/fau-advanced-separations/CADET-Process) are also welcome.
+
+## Acknowledgments
+
+Please refer to the [list of contributors](CONTRIBUTORS.md) who helped building and funding this project.
```

### Comparing `CADET-Process-0.8.0/examples/batch_elution/optimization_multi.py` & `CADET-Process-0.9.0/examples/batch_elution/optimization_single.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,27 +5,26 @@
 #     text_representation:
 #       extension: .py
 #       format_name: percent
 #       format_version: '1.3'
 #       jupytext_version: 1.14.5
 #   kernelspec:
 #     display_name: Python 3
-#     language: python
 #     name: python3
 # ---
 
 # %% [markdown]
-# (batch_elution_optimization_multi)=
-# # Optimize Batch Elution Process (Multi-Objective)
+# (batch_elution_optimization_single)=
+# # Optimize Batch Elution Process (Single Objective)
 #
 # ## Setup Optimization Problem
 
 # %%
 from CADETProcess.optimization import OptimizationProblem
-optimization_problem = OptimizationProblem('batch_elution_multi')
+optimization_problem = OptimizationProblem('batch_elution_single')
 
 from examples.batch_elution.process import process
 optimization_problem.add_evaluation_object(process)
 
 optimization_problem.add_variable('cycle_time', lb=10, ub=600)
 optimization_problem.add_variable('feed_duration.time', lb=10, ub=300)
 
@@ -55,41 +54,14 @@
     kwargs={
         'purity_required': [0.95, 0.95],
         'ignore_failed': False,
         'allow_empty_fractions': False,
     }
 )
 
-# %% [markdown]
-# ## Setup Objectives
-
-# %%
-from CADETProcess.performance import Productivity, Recovery, EluentConsumption
-
-productivity = Productivity()
-optimization_problem.add_objective(
-    productivity,
-    n_objectives=2,
-    requires=[process_simulator, frac_opt]
-)
-
-recovery = Recovery()
-optimization_problem.add_objective(
-    recovery,
-    n_objectives=2,
-    requires=[process_simulator, frac_opt]
-)
-
-eluent_consumption = EluentConsumption()
-optimization_problem.add_objective(
-    eluent_consumption,
-    n_objectives=2,
-    requires=[process_simulator, frac_opt]
-)
-
 
 # %% [markdown]
 # ## Add callback for post-processing
 
 # %%
 def callback(fractionation, individual, evaluation_object, callbacks_dir):
     fractionation.plot_fraction_signal(
@@ -98,14 +70,26 @@
     )
 
 optimization_problem.add_callback(
     callback, requires=[process_simulator, frac_opt]
 )
 
 # %% [markdown]
+# ## Setup Objectives
+
+# %%
+from CADETProcess.performance import PerformanceProduct
+ranking = [1, 1]
+performance = PerformanceProduct(ranking=ranking)
+
+optimization_problem.add_objective(
+    performance, requires=[process_simulator, frac_opt], minimize=False,
+)
+
+# %% [markdown]
 # ## Configure Optimizer
 
 # %%
 from CADETProcess.optimization import U_NSGA3
 optimizer = U_NSGA3()
 
 # %% [markdown]
@@ -113,13 +97,12 @@
 #
 # ```{note}
 # For performance reasons, the optimization is currently not run when building the documentation.
 # In future, we will try to sideload pre-computed results to also discuss them here.
 # ```
 #
 # ```
-# if __name__ == '__main__':
-#     results = optimizer.optimize(
-#         optimization_problem,
-#         use_checkpoint=True,
-#     )
+# results = optimizer.optimize(
+#     optimization_problem,
+#     use_checkpoint=True,
+# )
 # ```
```

### Comparing `CADET-Process-0.8.0/examples/batch_elution/optimization_single.py` & `CADET-Process-0.9.0/examples/batch_elution/optimization_multi.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 #     text_representation:
 #       extension: .py
 #       format_name: percent
 #       format_version: '1.3'
 #       jupytext_version: 1.14.5
 #   kernelspec:
 #     display_name: Python 3
+#     language: python
 #     name: python3
 # ---
 
 # %% [markdown]
-# (batch_elution_optimization_single)=
-# # Optimize Batch Elution Process (Single Objective)
+# (batch_elution_optimization_multi)=
+# # Optimize Batch Elution Process (Multi-Objective)
 #
 # ## Setup Optimization Problem
 
 # %%
 from CADETProcess.optimization import OptimizationProblem
-optimization_problem = OptimizationProblem('batch_elution_single')
+optimization_problem = OptimizationProblem('batch_elution_multi')
 
 from examples.batch_elution.process import process
 optimization_problem.add_evaluation_object(process)
 
 optimization_problem.add_variable('cycle_time', lb=10, ub=600)
 optimization_problem.add_variable('feed_duration.time', lb=10, ub=300)
 
@@ -54,14 +55,44 @@
     kwargs={
         'purity_required': [0.95, 0.95],
         'ignore_failed': False,
         'allow_empty_fractions': False,
     }
 )
 
+# %% [markdown]
+# ## Setup Objectives
+
+# %%
+from CADETProcess.performance import Productivity, Recovery, EluentConsumption
+
+productivity = Productivity()
+optimization_problem.add_objective(
+    productivity,
+    n_objectives=2,
+    requires=[process_simulator, frac_opt],
+    minimize=False,
+)
+
+recovery = Recovery()
+optimization_problem.add_objective(
+    recovery,
+    n_objectives=2,
+    requires=[process_simulator, frac_opt],
+    minimize=False,
+)
+
+eluent_consumption = EluentConsumption()
+optimization_problem.add_objective(
+    eluent_consumption,
+    n_objectives=2,
+    requires=[process_simulator, frac_opt],
+    minimize=False,
+)
+
 
 # %% [markdown]
 # ## Add callback for post-processing
 
 # %%
 def callback(fractionation, individual, evaluation_object, callbacks_dir):
     fractionation.plot_fraction_signal(
@@ -70,26 +101,14 @@
     )
 
 optimization_problem.add_callback(
     callback, requires=[process_simulator, frac_opt]
 )
 
 # %% [markdown]
-# ## Setup Objectives
-
-# %%
-from CADETProcess.performance import PerformanceProduct
-ranking = [1, 1]
-performance = PerformanceProduct(ranking=ranking)
-
-optimization_problem.add_objective(
-    performance, requires=[process_simulator, frac_opt]
-)
-
-# %% [markdown]
 # ## Configure Optimizer
 
 # %%
 from CADETProcess.optimization import U_NSGA3
 optimizer = U_NSGA3()
 
 # %% [markdown]
@@ -97,12 +116,13 @@
 #
 # ```{note}
 # For performance reasons, the optimization is currently not run when building the documentation.
 # In future, we will try to sideload pre-computed results to also discuss them here.
 # ```
 #
 # ```
-# results = optimizer.optimize(
-#     optimization_problem,
-#     use_checkpoint=True,
-# )
+# if __name__ == '__main__':
+#     results = optimizer.optimize(
+#         optimization_problem,
+#         use_checkpoint=True,
+#     )
 # ```
```

### Comparing `CADET-Process-0.8.0/examples/batch_elution/process.py` & `CADET-Process-0.9.0/examples/batch_elution/process.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/examples/characterize_chromatographic_system/column_transport_parameters.py` & `CADET-Process-0.9.0/examples/characterize_chromatographic_system/column_transport_parameters.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/examples/characterize_chromatographic_system/particle_porosity.py` & `CADET-Process-0.9.0/examples/characterize_chromatographic_system/particle_porosity.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/examples/load_wash_elute/lwe_concentration.py` & `CADET-Process-0.9.0/examples/load_wash_elute/lwe_concentration.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/examples/load_wash_elute/lwe_flow_rate.py` & `CADET-Process-0.9.0/examples/load_wash_elute/lwe_flow_rate.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/examples/recycling/clr_process.py` & `CADET-Process-0.9.0/examples/recycling/clr_process.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/examples/recycling/mrssr_process.py` & `CADET-Process-0.9.0/examples/recycling/mrssr_process.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/setup.cfg` & `CADET-Process-0.9.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = CADET-Process
-version = 0.8.0
+version = 0.9.0
 author = Johannes Schmölder
 author_email = j.schmoelder@fz-juelich.de
 description = A Framework for Modelling and Optimizing Advanced Chromatographic Processes
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/fau-advanced-separations/CADET-Process
 project_urls = 
@@ -22,40 +22,48 @@
 	scipy>=1.11
 	matplotlib>=3.4
 	corner>=2.2.1
 	sympy>=1.8
 	pathos>=0.2.8
 	addict==2.3
 	cadet-python>=0.14
-	hopsy>=1.3.0
+	hopsy>=1.4.0
 	pymoo>=0.6
 	numba>=0.55.1
 	diskcache>=5.4.0
 	joblib>=1.3.0
+	psutil>=5.9.8
 
 [options.extras_require]
 testing = 
 	setuptools
 	certifi     # tries to prevent certificate problems on windows
 	pre-commit  # system tests run pre-commit
 	flake8      # system tests run flake8
+	pytest
+	ax-platform>=0.3.5
 docs = 
 	sphinx>=5.3.0
 	sphinxcontrib-bibtex>=2.5.0
 	sphinx_book_theme>=1.0.0
 	sphinx_copybutton>=0.5.1
 	sphinx-sitemap>=2.5.0
 	numpydoc>=1.5.0
 	myst-nb>=0.17.1
+ax = 
+	ax-platform>=0.3.5
 
 [flake8]
 max_line_length = 88
 exclude = 
 	build
 	dist
 	.eggs
 	docs/conf.py
 
+[tool.pytest]
+pythonpath = tests
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `CADET-Process-0.8.0/tests/test_binding.py` & `CADET-Process-0.9.0/tests/test_binding.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/tests/test_buffer_capacity.py` & `CADET-Process-0.9.0/tests/test_buffer_capacity.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/tests/test_cache.py` & `CADET-Process-0.9.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/tests/test_cadet_adapter.py` & `CADET-Process-0.9.0/tests/test_cadet_adapter.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/tests/test_cadet_reactions.py` & `CADET-Process-0.9.0/tests/test_cadet_reactions.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/tests/test_carousel.py` & `CADET-Process-0.9.0/tests/test_carousel.py`

 * *Files 4% similar despite different names*

```diff
@@ -402,86 +402,86 @@
             'column_3', 'zone_III_outlet')
         )
         self.assertTrue(flow_sheet.connection_exists(
             'column_3', 'zone_IV_outlet')
         )
 
     def test_column_position_indices(self):
-        """Test column position index."""
+        """Test column position indices."""
         builder = self.create_smb()
 
         # Initial state, position 0
         carousel_position = 0
         carousel_state = 0
-        index_expected = 0
+        indices_expected = 0
 
-        index = builder.column_index_at_state(
+        indices = builder.column_indices_at_state(
             carousel_position, carousel_state
         )
-        self.assertEqual(index_expected, index)
+        self.assertEqual(indices_expected, indices)
 
         time = carousel_state * builder.switch_time
-        index = builder.column_index_at_time(time, carousel_position)
-        self.assertEqual(index_expected, index)
+        indices = builder.column_indices_at_time(time, carousel_position)
+        self.assertEqual(indices_expected, indices)
 
         # Initial state, position 1
         carousel_position = 1
         carousel_state = 0
-        index_expected = 1
+        indices_expected = 1
 
-        index = builder.column_index_at_state(
+        indices = builder.column_indices_at_state(
             carousel_position, carousel_state
         )
-        self.assertEqual(index_expected, index)
+        self.assertEqual(indices_expected, indices)
 
         time = carousel_state * builder.switch_time
-        index = builder.column_index_at_time(time, carousel_position)
-        self.assertEqual(index_expected, index)
+        indices = builder.column_indices_at_time(time, carousel_position)
+        self.assertEqual(indices_expected, indices)
 
         # First state, position 0
         carousel_position = 0
         carousel_state = 1
-        index_expected = 1
+        indices_expected = 1
 
-        index = builder.column_index_at_state(
+        indices = builder.column_indices_at_state(
             carousel_position, carousel_state
         )
-        self.assertEqual(index_expected, index)
+        self.assertEqual(indices_expected, indices)
 
         time = carousel_state * builder.switch_time
-        index = builder.column_index_at_time(time, carousel_position)
-        self.assertEqual(index_expected, index)
+        indices = builder.column_indices_at_time(time, carousel_position)
+        self.assertEqual(indices_expected, indices)
 
         # First state, position 1
         carousel_position = 1
         carousel_state = 1
-        index_expected = 2
+        indices_expected = 2
 
-        index = builder.column_index_at_state(
+        indices = builder.column_indices_at_state(
             carousel_position, carousel_state
         )
-        self.assertEqual(index_expected, index)
+        self.assertEqual(indices_expected, indices)
 
         time = carousel_state * builder.switch_time
-        index = builder.column_index_at_time(time, carousel_position)
-        self.assertEqual(index_expected, index)
+        indices = builder.column_indices_at_time(time, carousel_position)
+        self.assertEqual(indices_expected, indices)
 
         # 4th state (back to initial state), position 0
         carousel_position = 0
         carousel_state = 4
-        index_expected = 0
+        indices_expected = 0
 
-        index = builder.column_index_at_state(
+        indices = builder.column_indices_at_state(
             carousel_position, carousel_state
         )
-        self.assertEqual(index_expected, index)
+        self.assertEqual(indices_expected, indices)
 
         time = carousel_state * builder.switch_time
-        index = builder.column_index_at_time(time, carousel_position)
-        self.assertEqual(index_expected, index)
+        indices = builder.column_indices_at_time(time, carousel_position)
+        self.assertEqual(indices_expected, indices)
 
     def test_carousel_state(self):
         """Test carousel state."""
 
         builder = self.create_smb()
 
         # Initial state
```

### Comparing `CADET-Process-0.8.0/tests/test_compartment.py` & `CADET-Process-0.9.0/tests/test_compartment.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/tests/test_components.py` & `CADET-Process-0.9.0/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/tests/test_difference.py` & `CADET-Process-0.9.0/tests/test_difference.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,34 +134,34 @@
             'simple', time, solution_2_gaussian_different_height,
             component_system=comp_2
         )
 
     def test_metric(self):
         # Compare with itself
         difference = PeakHeight(
-            self.reference_single, components=['A']
+            self.reference, components=['A']
         )
         metrics_expected = [0]
         metrics = difference.evaluate(self.reference)
         np.testing.assert_almost_equal(metrics, metrics_expected)
 
         # Compare with other Gauss Peak
         difference = PeakHeight(
-            self.reference_single,
-            components=['B'],
+            self.reference_switched,
+            components=['A'],
             normalize_metrics=False
         )
         metrics_expected = [0]
         metrics = difference.evaluate(self.reference)
         np.testing.assert_almost_equal(metrics, metrics_expected)
 
         # Compare with other Gauss Peak, normalize_metrics
         difference = PeakHeight(
-            self.reference_single,
-            components=['B'],
+            self.reference_switched,
+            components=['A'],
             normalize_metrics=True
         )
         metrics_expected = [0]
         metrics = difference.evaluate(self.reference)
         np.testing.assert_almost_equal(metrics, metrics_expected)
 
         # Multi-component, compare with self.
@@ -219,33 +219,33 @@
             'simple', time, solution_2_gaussian_switched,
             component_system=comp_2
         )
 
     def test_metric(self):
         # Compare with itself
         difference = PeakPosition(
-            self.reference_single, components=['A']
+            self.reference, components=['A']
         )
         metrics_expected = [0]
         metrics = difference.evaluate(self.reference)
         np.testing.assert_almost_equal(metrics, metrics_expected)
 
         # Compare with other Gauss Peak
         difference = PeakPosition(
-            self.reference_single,
-            components=['B'],
+            self.reference_switched,
+            components=['A'],
             normalize_metrics=False
         )
         metrics_expected = [10]
         metrics = difference.evaluate(self.reference)
         np.testing.assert_almost_equal(metrics, metrics_expected)
 
         # Compare with other Gauss Peak, normalize_metrics
         difference = PeakPosition(
-            self.reference_single,
+            self.reference_switched,
             components=['B'],
             normalize_metrics=True
         )
         metrics_expected = [0.1651404]
         metrics = difference.evaluate(self.reference)
         np.testing.assert_almost_equal(metrics, metrics_expected)
 
@@ -292,60 +292,60 @@
             'simple', time, solution_2_gaussian_switched,
             component_system=comp_2
         )
 
     def test_metric(self):
         # Compare with itself
         difference = Shape(
-            self.reference_single,
+            self.reference,
             use_derivative=False,
             components=['A']
         )
         metrics_expected = [0, 0, 0]
         metrics = difference.evaluate(self.reference)
         np.testing.assert_almost_equal(metrics, metrics_expected)
 
         # Compare with other Gauss Peak
         difference = Shape(
-            self.reference_single,
+            self.reference_switched,
             use_derivative=False,
-            components=['B'],
+            components=['A'],
             normalize_metrics=False
         )
         metrics_expected = [5.5511151e-16, 10, 0.0000000e+00]
         metrics = difference.evaluate(self.reference)
         np.testing.assert_almost_equal(metrics, metrics_expected)
 
         # Compare with other Gauss Peak, normalize_metrics
         difference = Shape(
-            self.reference_single,
+            self.reference_switched,
             use_derivative=False,
-            components=['B'],
+            components=['A'],
             normalize_metrics=True
         )
         metrics_expected = [0, 4.6211716e-01, 0]
         metrics = difference.evaluate(self.reference)
         np.testing.assert_almost_equal(metrics, metrics_expected)
 
         # Compare with other Gauss Peak, include derivative
         difference = Shape(
-            self.reference_single,
+            self.reference_switched,
             use_derivative=True,
-            components=['B'],
+            components=['A'],
             normalize_metrics=False
         )
         metrics_expected = [0, 10, 0, 0, 0, 0]
         metrics = difference.evaluate(self.reference)
         np.testing.assert_almost_equal(metrics, metrics_expected)
 
         # Compare with other Gauss Peak, include derivative, normalize metrics
         difference = Shape(
-            self.reference_single,
+            self.reference_switched,
             use_derivative=True,
-            components=['B'],
+            components=['A'],
             normalize_metrics=True
         )
         metrics_expected = [0, 4.6211716e-01, 0, 0, 0, 0]
         metrics = difference.evaluate(self.reference)
         np.testing.assert_almost_equal(metrics, metrics_expected)
 
         # Multi-component, currently not implemented
```

### Comparing `CADET-Process-0.8.0/tests/test_equilibrium.py` & `CADET-Process-0.9.0/tests/test_equilibrium.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/tests/test_events.py` & `CADET-Process-0.9.0/tests/test_events.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,35 +35,38 @@
     n_entries = 4
     n_coeff = 4
 
     scalar_float = Float(default=0)
     switch = Switch(valid=[-1, 1], default=1)
     sized_tuple = SizedTuple(size=2, default=(1, 1))
     array_1d = SizedList(size=4, default=0)
+    array_1d_single = SizedList(size=1, default=0)
     ndarray = SizedNdArray(size=(2, 4), default=0)
     ndarray_no_default = SizedNdArray(size=(2, 4))
     array_1d_poly = Polynomial(n_coeff=4, default=0)
     ndarray_poly = NdPolynomial(n_entries=2, n_coeff=4, default=0)
     ndarray_poly_dep = NdPolynomial(size=('n_entries', 'n_coeff'), default=0)
 
     _parameters = [
         'scalar_float',
         'sized_tuple',
         'switch',
         'array_1d',
+        'array_1d_single',
         'ndarray',
         'ndarray_no_default',
         'array_1d_poly',
         'ndarray_poly',
         'ndarray_poly_dep',
     ]
     _section_dependent_parameters = [
         'scalar_float',
         'sized_tuple',
         'array_1d',
+        'array_1d_single',
         'ndarray',
         'ndarray_no_default',
         'array_1d_poly',
         'ndarray_poly',
         'ndarray_poly_dep',
     ]
 
@@ -171,14 +174,50 @@
 
         # Raise Error for indices
         with self.assertRaises(IndexError):
             evt = event_handler.add_event(
                 'param_has_no_indices', 'performer.scalar_float', 1, time=0, indices=1
             )
 
+    def test_event_array_1d_single(self):
+        """
+        Extra test for array with single entry.
+
+        See also: https://github.com/fau-advanced-separations/CADET-Process/pull/68
+        """
+        event_handler = self.event_handler
+
+        # No index
+        evt = event_handler.add_event('trivial', 'performer.array_1d_single', 1, time=0)
+        self.assertEqual(evt.state, 1)
+        self.assertEqual(evt.full_state, [1])
+        self.assertEqual(evt.n_entries, 1)
+        self.assertEqual(evt.indices, [(slice(None, None, None),)])
+        self.assertEqual(evt.full_indices, [(0,)])
+        self.assertEqual(evt.n_indices, 1)
+        self.assertEqual(event_handler.performer.array_1d_single, [1])
+
+        # Explicit Index
+        evt = event_handler.add_event(
+            'trivial_1', 'performer.array_1d_single', 2, time=0, indices=0
+        )
+        self.assertEqual(evt.state, 2)
+        self.assertEqual(evt.full_state, [2])
+        self.assertEqual(evt.n_entries, 1)
+        self.assertEqual(evt.indices, [(0, )])
+        self.assertEqual(evt.full_indices, [(0,)])
+        self.assertEqual(evt.n_indices, 1)
+        self.assertEqual(event_handler.performer.array_1d_single, [2])
+
+        # Raise Error for exceeding indices
+        with self.assertRaises(IndexError):
+            evt = event_handler.add_event(
+                'param_has_no_indices', 'performer.array_1d_single', 1, time=0, indices=1
+            )
+
     def test_event_1D(self):
         # TODO: Check too many / few indices
         event_handler = self.event_handler
 
         # Add event for single entry in 1D list / array
         event_handler.performer.array_1d
         evt = event_handler.add_event(
```

### Comparing `CADET-Process-0.8.0/tests/test_flow_sheet.py` & `CADET-Process-0.9.0/tests/test_flow_sheet.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,26 +7,57 @@
 from CADETProcess.processModel import (
     Inlet, Cstr, LumpedRateModelWithoutPores, Outlet
 )
 from CADETProcess.processModel import FlowSheet
 
 
 def setup_single_cstr_flow_sheet(component_system=None):
+    """
+    Set up a simple `FlowSheet` with a single Continuous Stirred Tank Reactor (CSTR).
+
+    Parameters
+    ----------
+    component_system : ComponentSystem, optional
+        The component system for the CSTR.
+        Defaults to a system with two components if None.
+
+    Returns
+    -------
+    FlowSheet
+        A flow sheet with a single CSTR unit.
+
+    """
     if component_system is None:
         component_system = ComponentSystem(2)
 
     cstr = Cstr(component_system, 'cstr')
 
     flow_sheet = FlowSheet(component_system)
     flow_sheet.add_unit(cstr)
 
     return flow_sheet
 
 
 def setup_batch_elution_flow_sheet(component_system=None):
+    """
+    Set up a `FlowSheet` for a typical batch elution process.
+
+    Parameters
+    ----------
+    component_system : ComponentSystem, optional
+        The component system for the batch elution process.
+        Defaults to a system with two components if None.
+
+    Returns
+    -------
+    FlowSheet
+        A flow sheet configured for batch elution processes, including feed and eluent
+        inlets, a column, and an outlet.
+
+    """
     if component_system is None:
         component_system = ComponentSystem(2)
 
     flow_sheet = FlowSheet(component_system)
 
     feed = Inlet(component_system, name='feed')
     eluent = Inlet(component_system, name='eluent')
@@ -42,14 +73,30 @@
     flow_sheet.add_connection(eluent, column)
     flow_sheet.add_connection(column, outlet)
 
     return flow_sheet
 
 
 def setup_ssr_flow_sheet(component_system=None):
+    """
+    Set up a `FlowSheet` for a steady state recycling (SSR) process.
+
+    Parameters
+    ----------
+    component_system : ComponentSystem, optional
+        The component system for the SSR process.
+        Defaults to a system with two components if None.
+
+    Returns
+    -------
+    FlowSheet
+        A flow sheet configured for SSR elution, including feed and eluent inlets, a
+        mixer tank, a column, and an outlet.
+
+    """
     if component_system is None:
         component_system = ComponentSystem(2)
 
     flow_sheet = FlowSheet(component_system)
 
     feed = Inlet(component_system, name='feed')
     eluent = Inlet(component_system, name='eluent')
@@ -72,15 +119,16 @@
     flow_sheet.add_eluent_inlet(eluent)
     flow_sheet.add_feed_inlet(feed)
     flow_sheet.add_product_outlet(outlet)
 
     return flow_sheet
 
 
-class Test_flow_sheet(unittest.TestCase):
+class TestFlowSheet(unittest.TestCase):
+    """Test general functionatlity of `FlowSheet` class."""
 
     def __init__(self, methodName='runTest'):
         super().__init__(methodName)
 
     def setUp(self):
         self.component_system = ComponentSystem(2)
 
@@ -427,14 +475,28 @@
                 },
         }
 
         np.testing.assert_equal(
             self.ssr_flow_sheet.get_flow_rates(), expected_flow_rates
         )
 
+        # Single Cstr
+        expected_flow_rates = {
+            'cstr': {
+                'total_in': [0.0, 0.0, 0.0, 0.0],
+                'total_out': [0.0, 0.0, 0.0, 0.0],
+                'origins': {},
+                'destinations': {}
+            }
+        }
+
+        np.testing.assert_equal(
+            self.single_cstr_flow_sheet.get_flow_rates(), expected_flow_rates
+        )
+
     def test_check_connectivity(self):
         self.assertTrue(self.single_cstr_flow_sheet.check_connections())
         self.assertTrue(self.batch_flow_sheet.check_connections())
         self.assertTrue(self.ssr_flow_sheet.check_connections())
 
         self.batch_flow_sheet.remove_unit('outlet')
 
@@ -486,15 +548,26 @@
                 column,
                 {
                     'column': 0.1,
                     'outlet': 0.9,
                 }
             )
 
+
 class TestCstrFlowRate(unittest.TestCase):
+    """
+    Test `Cstr` behaviour.
+
+    Notes
+    -----
+    When the `flow_rate` parameter of the `Cstr` is not explicitly set, it is treated
+    just like any other `UnitOperation`. I.e., q_in == q_out. In contrast, when a value
+    is set, it has properties similar to an `Inlet`.
+    """
+
     def __init__(self, methodName='runTest'):
         super().__init__(methodName)
 
     def setUp(self):
         self.component_system = ComponentSystem(2)
 
         flow_sheet = FlowSheet(self.component_system)
@@ -534,14 +607,40 @@
         cstr_in_expected = [1., 1., 0., 0.]
         np.testing.assert_almost_equal(cstr_in, cstr_in_expected)
 
         cstr_out = flow_rates['cstr']['total_out']
         cstr_out_expected = [1., 1., 0., 0.]
         np.testing.assert_almost_equal(cstr_out, cstr_out_expected)
 
+    def test_no_flow(self):
+        self.flow_sheet.inlet.flow_rate = 0
+
+        flow_rates = self.flow_sheet.get_flow_rates()
+
+        cstr_in = flow_rates['cstr']['total_in']
+        cstr_in_expected = [0., 0., 0., 0.]
+        np.testing.assert_almost_equal(cstr_in, cstr_in_expected)
+
+        cstr_out = flow_rates['cstr']['total_out']
+        cstr_out_expected = [0., 0., 0., 0.]
+        np.testing.assert_almost_equal(cstr_out, cstr_out_expected)
+
+        self.flow_sheet.inlet.flow_rate = 0
+        self.flow_sheet.cstr.flow_rate = 0
+
+        flow_rates = self.flow_sheet.get_flow_rates()
+
+        cstr_in = flow_rates['cstr']['total_in']
+        cstr_in_expected = [0., 0., 0., 0.]
+        np.testing.assert_almost_equal(cstr_in, cstr_in_expected)
+
+        cstr_out = flow_rates['cstr']['total_out']
+        cstr_out_expected = [0., 0., 0., 0.]
+        np.testing.assert_almost_equal(cstr_out, cstr_out_expected)
+
     def test_holdup(self):
         self.flow_sheet.inlet.flow_rate = 1
         self.flow_sheet.cstr.flow_rate = 0
 
         flow_rates = self.flow_sheet.get_flow_rates()
 
         cstr_in = flow_rates['cstr']['total_in']
@@ -566,9 +665,284 @@
         np.testing.assert_almost_equal(cstr_in, cstr_in_expected)
 
         cstr_out = flow_rates['cstr']['total_out']
         cstr_out_expected = [2., 2., 0., 0.]
         np.testing.assert_almost_equal(cstr_out, cstr_out_expected)
 
 
+class TestFlowRateMatrix(unittest.TestCase):
+    """Test calculation of flow rates with another simple testcase by @daklauss"""
+
+    def __init__(self, methodName='runTest'):
+        super().__init__(methodName)
+
+    def setUp(self):
+        self.component_system = ComponentSystem(1)
+
+        flow_sheet = FlowSheet(self.component_system)
+
+        inlet = Inlet(self.component_system, name='inlet')
+        cstr1 = Cstr(self.component_system, name='cstr1')
+        cstr2 = Cstr(self.component_system, name='cstr2')
+        outlet1 = Outlet(self.component_system, name='outlet1')
+        outlet2 = Outlet(self.component_system, name='outlet2')
+
+        flow_sheet.add_unit(inlet)
+        flow_sheet.add_unit(cstr1)
+        flow_sheet.add_unit(cstr2)
+
+        flow_sheet.add_unit(outlet1)
+        flow_sheet.add_unit(outlet2)
+
+        flow_sheet.add_connection(inlet, cstr1)
+        flow_sheet.add_connection(inlet, cstr2)
+
+        flow_sheet.add_connection(cstr1, outlet1)
+        flow_sheet.add_connection(cstr2, outlet2)
+
+        flow_sheet.add_connection(cstr2, cstr1)
+
+        flow_sheet.set_output_state(inlet, [0.3, 0.7])
+        flow_sheet.set_output_state(cstr2, [0.5, 0.5])
+
+        self.flow_sheet = flow_sheet
+
+    def test_matrix_example(self):
+        self.flow_sheet.inlet.flow_rate = [1]
+
+        expected_flow_rates = {
+            'inlet': {
+                'total_out': (1, 0, 0, 0),
+                'destinations': {
+                    'cstr1': (0.3, 0, 0, 0),
+                    'cstr2': (0.7, 0, 0, 0),
+                },
+            },
+            'cstr1': {
+                'total_in': (0.65, 0, 0, 0),
+                'total_out': (0.65, 0, 0, 0),
+                'origins': {
+                    'inlet': (0.3, 0, 0, 0),
+                    'cstr2': (0.35, 0, 0, 0),
+                },
+                'destinations': {
+                    'outlet1': (0.65, 0, 0, 0),
+                },
+            },
+            'cstr2': {
+                'total_in': (0.7, 0, 0, 0),
+                'total_out': (0.7, 0, 0, 0),
+                'origins': {
+                    'inlet': (0.7, 0, 0, 0),
+                },
+                'destinations': {
+                    'cstr1': (0.35, 0, 0, 0),
+                    'outlet2': (0.35, 0, 0, 0),
+                },
+            },
+            'outlet1': {
+                'origins': {
+                    'cstr1': (0.65, 0, 0, 0),
+                },
+                'total_in': (0.65, 0, 0, 0),
+            },
+
+            'outlet2': {
+                'origins': {
+                    'cstr2': (0.35, 0, 0, 0),
+                },
+                'total_in': (0.35, 0, 0, 0),
+                }
+        }
+
+        calc_flow_rate = self.flow_sheet.get_flow_rates()
+
+        def assert_almost_equal_dict(
+                dict_actual, dict_expected, decimal=7, verbose=True):
+            """Helper function to assert nested dicts are (almost) equal.
+
+            Because of floating point calculations, it is necessary to use
+            `np.assert_almost_equal` to check the flow rates. However, this does not
+            work well with nested dicts which is why this helper function was written.
+
+            Parameters
+            ----------
+            dict_actual : dict
+                The object to check.
+            dict_expected : dict
+                The expected object.
+            decimal : int, optional
+                Desired precision, default is 7.
+            err_msg : str, optional
+                The error message to be printed in case of failure.
+            verbose : bool, optional
+                If True, the conflicting values are appended to the error message.
+
+            """
+            for key in dict_actual:
+                if isinstance(dict_actual[key], dict):
+                    assert_almost_equal_dict(dict_actual[key], dict_expected[key])
+                else:
+                    np.testing.assert_almost_equal(
+                        dict_actual[key], dict_expected[key],
+                        decimal=decimal,
+                        err_msg=f'Dicts are not equal in key {key}.',
+                        verbose=verbose
+                    )
+
+        assert_almost_equal_dict(calc_flow_rate, expected_flow_rates)
+
+
+class TestFlowRateSelfMatrix(unittest.TestCase):
+    """Test special case where one unit is connected to itself."""
+    def __init__(self, methodName='runTest'):
+        super().__init__(methodName)
+
+    def setUp(self):
+        self.component_system = ComponentSystem(1)
+
+        flow_sheet = FlowSheet(self.component_system)
+
+        inlet = Inlet(self.component_system, name='inlet')
+        cstr = Cstr(self.component_system, name='cstr')
+        outlet = Outlet(self.component_system, name='outlet')
+
+        flow_sheet.add_unit(inlet)
+        flow_sheet.add_unit(cstr)
+        flow_sheet.add_unit(outlet)
+
+        flow_sheet.add_connection(inlet, cstr)
+        flow_sheet.add_connection(cstr, outlet)
+
+        flow_sheet.add_connection(cstr, cstr)
+
+        flow_sheet.set_output_state(cstr, [0.5, 0.5])
+
+        self.flow_sheet = flow_sheet
+
+    def test_matrix_self_example(self):
+        self.flow_sheet.inlet.flow_rate = [1]
+
+        expected_flow_rates = {
+            'inlet': {
+                'total_out': (1, 0, 0, 0),
+                'destinations': {
+                    'cstr': (1, 0, 0, 0)
+                },
+            },
+            'cstr': {
+                'total_in': (2, 0, 0, 0),
+                'total_out': (2, 0, 0, 0),
+                'origins': {
+                    'inlet': (1, 0, 0, 0),
+                    'cstr': (1, 0, 0, 0),
+                },
+                'destinations': {
+                    'outlet': (1, 0, 0, 0),
+                    'cstr': (1, 0, 0, 0)
+                },
+            },
+            'outlet': {
+                'total_in': (1, 0, 0, 0),
+                'origins': {
+                    'cstr': (1, 0, 0, 0)
+                }
+            }
+        }
+        calc_flow_rate = self.flow_sheet.get_flow_rates()
+        np.testing.assert_equal(calc_flow_rate, expected_flow_rates)
+
+
+class TestSingularFlowMatrix(unittest.TestCase):
+    """Test cases with disconnected flow circles
+
+    Notes
+    -----
+    `FlowSheet`: `Inlet` connected to an `Outlet` and two `Cstr`s connected to each
+    other but not with the other units.
+
+    """
+
+    def __init__(self, methodName='runTest'):
+        super().__init__(methodName)
+
+    def setUp(self):
+
+        self.component_system = ComponentSystem(1)
+
+        flow_sheet = FlowSheet(self.component_system)
+
+        inlet = Inlet(self.component_system, name='inlet')
+        cstr1 = Cstr(self.component_system, name='cstr1')
+        cstr2 = Cstr(self.component_system, name='cstr2')
+        outlet = Outlet(self.component_system, name='outlet')
+
+        flow_sheet.add_unit(inlet)
+        flow_sheet.add_unit(cstr1)
+        flow_sheet.add_unit(cstr2)
+        flow_sheet.add_unit(outlet)
+
+        flow_sheet.add_connection(inlet, outlet)
+
+        flow_sheet.add_connection(cstr1, cstr2)
+        flow_sheet.add_connection(cstr2, cstr1)
+
+        self.flow_sheet = flow_sheet
+
+    def test_expelled_cicuit(self):
+        # Throw error even without flow, because system is singular
+        flow_sheet = self.flow_sheet
+
+        with self.assertRaises(CADETProcessError):
+            flow_sheet.get_flow_rates()
+
+        flow_sheet.inlet.flow_rate = [1]
+
+        with self.assertRaises(CADETProcessError):
+            flow_sheet.get_flow_rates()
+
+    def test_expelled_circuit_with_flow(self):
+        # Solvable because both disconnected circles have their own flow rates
+        expected_flow_rates = {
+            'inlet': {
+                'total_out': (1, 0, 0, 0),
+                'destinations': {
+                    'outlet': (1, 0, 0, 0)
+                },
+            },
+            'cstr1': {
+                'total_in': (1, 0, 0, 0),
+                'total_out': (1, 0, 0, 0),
+                'origins': {
+                    'cstr2': (1, 0, 0, 0),
+                },
+                'destinations': {
+                    'cstr2': (1, 0, 0, 0)
+                },
+            },
+            'cstr2': {
+                'total_in': (1, 0, 0, 0),
+                'total_out': (1, 0, 0, 0),
+                'origins': {
+                    'cstr1': (1, 0, 0, 0),
+                },
+                'destinations': {
+                    'cstr1': (1, 0, 0, 0)
+                },
+            },
+            'outlet': {
+                'total_in': (1, 0, 0, 0),
+                'origins': {
+                    'inlet': (1, 0, 0, 0)
+                }
+            }
+        }
+
+        flow_sheet = self.flow_sheet
+        flow_sheet.inlet.flow_rate = [1]
+        flow_sheet.cstr1.flow_rate = [1]
+
+        np.testing.assert_equal(flow_sheet.get_flow_rates(), expected_flow_rates)
+
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `CADET-Process-0.8.0/tests/test_fractions.py` & `CADET-Process-0.9.0/tests/test_fractions.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/tests/test_individual.py` & `CADET-Process-0.9.0/tests/test_individual.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/tests/test_optimization_integration.py` & `CADET-Process-0.9.0/tests/test_optimization_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 sys.path.insert(0, '../')
 
 # Set flags for which test cases to run
 test_batch_elution_single_objective_single_core = True
 test_batch_elution_single_objective_multi_core = True
 test_batch_elution_multi_objective = True
-test_fit_column_parameters = True
+test_fit_column_parameters = False
 
 
 class TestBatchElutionOptimizationSingleObjective(unittest.TestCase):
     def setUp(self):
         settings.working_directory = './test_batch'
         from examples.batch_elution.optimization_single import (
             optimization_problem, optimizer
```

### Comparing `CADET-Process-0.8.0/tests/test_optimization_problem.py` & `CADET-Process-0.9.0/tests/test_optimization_problem.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,27 +16,31 @@
     LinearEqualityConstraintsSooTestProblem
 )
 
 
 class EvaluationObject(Structure):
     uninitialized = None
     scalar_param = Float(default=1)
+    scalar_param_2 = Float(default=1)
     list_param = List()
     sized_list_param = SizedList(size=2, default=[1, 2])
+    sized_list_param_single = SizedList(size=1, default=1)
     sized_list_param_no_default = SizedList(size=2)
     nd_array = SizedNdArray(size=(2, 2))
     polynomial_param = Polynomial(n_coeff=2, default=0)
     polynomial_param_no_default = Polynomial(n_coeff=2)
     nd_polynomial_param = NdPolynomial(size=(2, 4), default=0)
 
     _parameters = [
         'uninitialized',
         'scalar_param',
+        'scalar_param_2',
         'list_param',
         'sized_list_param',
+        'sized_list_param_single',
         'sized_list_param_no_default',
         'nd_array',
         'polynomial_param',
         'polynomial_param_no_default',
         'nd_polynomial_param',
     ]
 
@@ -158,14 +162,52 @@
             var = OptimizationVariable(
                 'uninitialized_attribute',
                 evaluation_objects=[self.evaluation_object],
                 parameter_path='uninitialized',
                 indices=2
             )
 
+    def test_sized_list_single(self):
+        """
+        Extra test for array with single entry.
+
+        See also: https://github.com/fau-advanced-separations/CADET-Process/pull/68
+        """
+        # No indices
+        var = OptimizationVariable(
+            'sized_list_param_single',
+            evaluation_objects=[self.evaluation_object],
+            parameter_path='sized_list_param_single',
+        )
+        np.testing.assert_equal(var.indices, [[(slice(None, None, None),)]])
+        var.value = 1
+        np.testing.assert_equal(var.value, 1)
+        np.testing.assert_equal(self.evaluation_object.sized_list_param_single, [1])
+
+        # Explicit index
+        var = OptimizationVariable(
+            'sized_list_param_single',
+            evaluation_objects=[self.evaluation_object],
+            parameter_path='sized_list_param_single',
+            indices=0,
+        )
+        np.testing.assert_equal(var.indices, [[(0, )]])
+        var.value = 2
+        np.testing.assert_equal(var.value, 2)
+        np.testing.assert_equal(self.evaluation_object.sized_list_param_single, [2])
+
+        # Raise Exception for exceeding index
+        with self.assertRaises(IndexError):
+            var = OptimizationVariable(
+                'sized_list_param_single',
+                evaluation_objects=[self.evaluation_object],
+                parameter_path='sized_list_param_single',
+                indices=1,
+            )
+
     def test_nd_array(self):
         var = OptimizationVariable(
             'nd_array_index',
             evaluation_objects=[self.evaluation_object],
             parameter_path='nd_array',
             indices=(0, 0)
         )
@@ -691,29 +733,27 @@
             self.optimization_problem.add_linear_constraint('inexistent')
 
         # Incorrect shape
         with self.assertRaises(CADETProcessError):
             self.optimization_problem.add_linear_constraint('var_0', [])
 
     def test_initial_values(self):
-        x0_chebyshev_expected = [[0.2928932, 0.7071068]]
-        x0_chebyshev = self.optimization_problem.create_initial_values(
-            1, method='chebyshev'
+        x0_chebyshev_expected = [1/3, 2/3]
+        x0_chebyshev = self.optimization_problem.get_chebyshev_center(
+            include_dependent_variables=True
         )
         np.testing.assert_almost_equal(x0_chebyshev, x0_chebyshev_expected)
 
         x0_seed_1_expected = [[0.5666524, 0.8499365]]
         x0_seed_1 = self.optimization_problem.create_initial_values(
-            1, method='random', seed=1
+            1, seed=1
         )
         np.testing.assert_almost_equal(x0_seed_1, x0_seed_1_expected)
 
-        x0_seed_1_random = self.optimization_problem.create_initial_values(
-            1, method='random'
-        )
+        x0_seed_1_random = self.optimization_problem.create_initial_values(1)
 
         with self.assertRaises(AssertionError):
             np.testing.assert_almost_equal(x0_seed_1_random, x0_seed_1_expected)
 
         with self.assertRaises(AssertionError):
             np.testing.assert_almost_equal(x0_seed_1_random, x0_chebyshev_expected)
 
@@ -726,21 +766,19 @@
             [0.2685012584445143, 0.9067761747715452],
             [0.9701611935982989, 0.9809160496933532],
             [0.35086424227614005, 0.4668187637599064],
             [0.8928778441932161, 0.9360696751348305],
             [0.5365699848069944, 0.6516012021958184]
         ]
         x0_seed_10 = self.optimization_problem.create_initial_values(
-            10, method='random', seed=1
+            10, seed=1
         )
         np.testing.assert_almost_equal(x0_seed_10, x0_seed_10_expected)
 
-        x0_seed_10_random = self.optimization_problem.create_initial_values(
-            10, method='random'
-        )
+        x0_seed_10_random = self.optimization_problem.create_initial_values(10)
 
         with self.assertRaises(AssertionError):
             np.testing.assert_almost_equal(x0_seed_10_random, x0_seed_10_expected)
 
 
 class Test_OptimizationProblemDepVar(unittest.TestCase):
     def __init__(self, methodName='runTest'):
@@ -804,76 +842,117 @@
         dependent_variables = self.optimization_problem.dependent_variable_names
         self.assertEqual(dependent_variables_expected, dependent_variables)
 
         variables_expected = ['foo', 'bar', 'spam', 'eggs']
         variables = self.optimization_problem.variable_names
         self.assertEqual(variables_expected, variables)
 
-    def test_initial_values(self):
-        x0_chebyshev_expected = [[0.79289322, 0.20710678, 0.5]]
-        x0_chebyshev = self.optimization_problem.create_initial_values(
-            1, method='chebyshev'
+    def test_initial_values_without_dependencies(self):
+        x0_chebyshev_expected = [2/3, 0.5, 1/3]
+        x0_chebyshev = self.optimization_problem.get_chebyshev_center(
+            include_dependent_variables=False
         )
         np.testing.assert_almost_equal(x0_chebyshev, x0_chebyshev_expected)
 
-        variables_expected = [
-            0.7928932188134523,
-            0.2071067811865475,
-            0.2071067811865475,
-            0.4999999999999999
-        ]
-        variables = self.optimization_problem.get_dependent_values(
-            x0_chebyshev[0, :]
-        )
+        variables_expected = [2/3, 0.5, 0.5, 1/3]
+        variables = self.optimization_problem.get_dependent_values(x0_chebyshev)
         np.testing.assert_almost_equal(variables, variables_expected)
 
+        x0_seed_1_expected = [[0.90164487, 0.27971297, 0.70490538]]
+        x0_seed_1 = self.optimization_problem.create_initial_values(
+            1, seed=1, include_dependent_variables=False
+        )
+        np.testing.assert_almost_equal(x0_seed_1, x0_seed_1_expected)
         self.assertTrue(
             self.optimization_problem.check_linear_constraints(
-                x0_chebyshev[0, :], get_dependent_values=True
+                x0_seed_1[0], get_dependent_values=True
             )
         )
-        self.assertTrue(
-            self.optimization_problem.check_linear_constraints(variables)
+
+        x0_seed_1_random = self.optimization_problem.create_initial_values(
+            1, include_dependent_variables=False
+        )
+
+        with self.assertRaises(AssertionError):
+            np.testing.assert_almost_equal(x0_seed_1_random, x0_seed_1_expected)
+
+        with self.assertRaises(AssertionError):
+            np.testing.assert_almost_equal(x0_seed_1_random, x0_chebyshev_expected)
+
+        x0_seed_10_expected = [
+            [0.90164487, 0.27971297, 0.70490538],
+            [0.78125338, 0.17275154, 0.54650281],
+            [0.97623563, 0.19106333, 0.79016462],
+            [0.12826546, 0.03476412, 0.05270397],
+            [0.89791146, 0.29062957, 0.7429437 ],
+            [0.8703531 , 0.20575487, 0.68237913],
+            [0.92572799, 0.01653708, 0.33539715],
+            [0.96337056, 0.07106034, 0.86232007],
+            [0.85559046, 0.4824452 , 0.84474955],
+            [0.8588277 , 0.73874869, 0.80355266]
+        ]
+        x0_seed_10 = self.optimization_problem.create_initial_values(
+            10, seed=1, include_dependent_variables=False
+        )
+        np.testing.assert_almost_equal(x0_seed_10, x0_seed_10_expected)
+
+        x0_seed_10_random = self.optimization_problem.create_initial_values(
+            10, include_dependent_variables=False
+        )
+
+        with self.assertRaises(AssertionError):
+            np.testing.assert_almost_equal(x0_seed_10_random, x0_seed_10_expected)
+
+    def test_initial_values(self):
+        x0_chebyshev_expected = [2/3, 0.5, 0.5, 1/3]
+        x0_chebyshev = self.optimization_problem.get_chebyshev_center(
+            include_dependent_variables=True
         )
+        np.testing.assert_almost_equal(x0_chebyshev, x0_chebyshev_expected)
+
+        independent_variables_expected = [2/3, 0.5, 1/3]
+        independent_variables = self.optimization_problem.get_independent_values(x0_chebyshev)
+        np.testing.assert_almost_equal(independent_variables, independent_variables_expected)
 
-        x0_seed_1_expected = [[0.7311044, 0.1727515, 0.1822629]]
+        x0_seed_1_expected = [[0.9016449, 0.279713 , 0.279713 , 0.7049054]]
         x0_seed_1 = self.optimization_problem.create_initial_values(
-            1, method='random', seed=1
+            1, seed=1, include_dependent_variables=True
         )
         np.testing.assert_almost_equal(x0_seed_1, x0_seed_1_expected)
+        self.assertTrue(self.optimization_problem.check_linear_constraints(x0_seed_1[0]))
 
         x0_seed_1_random = self.optimization_problem.create_initial_values(
-            1, method='random'
-        )
+            1, include_dependent_variables=True
+        )[0]
 
         with self.assertRaises(AssertionError):
             np.testing.assert_almost_equal(x0_seed_1_random, x0_seed_1_expected)
 
         with self.assertRaises(AssertionError):
             np.testing.assert_almost_equal(x0_seed_1_random, x0_chebyshev_expected)
 
         x0_seed_10_expected = [
-            [0.7311043824888657, 0.1727515432673712, 0.18226293643057073],
-            [0.9836918383919191, 0.8152389217047241, 0.8560016844195478],
-            [0.7358144798470049, 0.2574714423019172, 0.49387609464567295],
-            [0.34919171897183954, 0.05751800197656948, 0.3237260675631758],
-            [0.9265061673265441, 0.4857572549618687, 0.8149444448089398],
-            [0.9065669851023331, 0.1513817591204391, 0.7710992332649812],
-            [0.8864554240066591, 0.4771068979697068, 0.5603893963194555],
-            [0.6845940550232432, 0.2843172686185149, 0.6792904559788712],
-            [0.923735889273789, 0.6890814170651027, 0.7366940211809302],
-            [0.8359314486227345, 0.39493879515319996, 0.8128182754300088]
+            [0.90164487, 0.27971297, 0.27971297, 0.70490538],
+            [0.78125338, 0.17275154, 0.17275154, 0.54650281],
+            [0.97623563, 0.19106333, 0.19106333, 0.79016462],
+            [0.12826546, 0.03476412, 0.03476412, 0.05270397],
+            [0.89791146, 0.29062957, 0.29062957, 0.7429437 ],
+            [0.8703531 , 0.20575487, 0.20575487, 0.68237913],
+            [0.92572799, 0.01653708, 0.01653708, 0.33539715],
+            [0.96337056, 0.07106034, 0.07106034, 0.86232007],
+            [0.85559046, 0.4824452 , 0.4824452 , 0.84474955],
+            [0.8588277 , 0.73874869, 0.73874869, 0.80355266]
         ]
         x0_seed_10 = self.optimization_problem.create_initial_values(
-            10, method='random', seed=1
+            10, seed=1, include_dependent_variables=True
         )
         np.testing.assert_almost_equal(x0_seed_10, x0_seed_10_expected)
 
         x0_seed_10_random = self.optimization_problem.create_initial_values(
-            10, method='random'
+            10, include_dependent_variables=True
         )
 
         with self.assertRaises(AssertionError):
             np.testing.assert_almost_equal(x0_seed_10_random, x0_seed_10_expected)
 
 
 class Test_OptimizationProblemJacobian(unittest.TestCase):
@@ -1168,9 +1247,84 @@
                 lb=0, ub=10, indices=1
             )
 
     def test_cache(self):
         pass
 
 
+class Test_MultiEvaluationObjects(unittest.TestCase):
+    def __init__(self, methodName='runTest'):
+        super().__init__(methodName)
+
+    def setUp(self):
+        eval_obj_1 = EvaluationObject(name='foo')
+        eval_obj_2 = EvaluationObject(name='bar')
+
+        # Simple case
+        optimization_problem = OptimizationProblem(
+            'with_evaluator', use_diskcache=False
+        )
+
+        optimization_problem.add_evaluation_object(eval_obj_1)
+        optimization_problem.add_evaluation_object(eval_obj_2)
+
+        optimization_problem.add_variable(
+            name='scalar_eval_obj_1', parameter_path='scalar_param', lb=0, ub=1,
+            evaluation_objects=[eval_obj_1]
+        )
+        optimization_problem.add_variable(
+            name='scalar_eval_obj_2', parameter_path='scalar_param', lb=0, ub=1,
+            evaluation_objects=[eval_obj_2]
+        )
+
+        optimization_problem.add_variable(
+            name='scalar_both_eval_obj', parameter_path='scalar_param_2', lb=0, ub=1,
+        )
+
+
+        def single_obj_1(eval_obj):
+            return 0
+
+        optimization_problem.add_objective(single_obj_1)
+
+
+        def single_obj_2(eval_obj):
+            return 1
+
+        optimization_problem.add_objective(single_obj_2, evaluation_objects=eval_obj_1)
+
+
+        def multi_obj(eval_obj):
+            return [2, 3]
+
+        optimization_problem.add_objective(multi_obj, n_objectives=2)
+
+
+        self.optimization_problem = optimization_problem
+
+    def test_evaluation(self):
+        f_expected = [0, 0, 1, 2, 3, 2, 3]
+        f = self.optimization_problem.evaluate_objectives([1, 1, 1])
+
+        np.testing.assert_allclose(f, f_expected)
+
+    def test_names(self):
+        names_expected = ['single_obj_1', 'single_obj_2', 'multi_obj']
+        names = self.optimization_problem.objective_names
+        self.assertEqual(names, names_expected)
+
+    def test_labels(self):
+        labels_expected = [
+            'foo_single_obj_1',
+            'bar_single_obj_1',
+            'single_obj_2',
+            'foo_multi_obj_0',
+            'bar_multi_obj_0',
+            'foo_multi_obj_1',
+            'bar_multi_obj_1'
+        ]
+        labels = self.optimization_problem.objective_labels
+        self.assertEqual(labels, labels_expected)
+
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `CADET-Process-0.8.0/tests/test_optimization_results.py` & `CADET-Process-0.9.0/tests/test_optimization_results.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     if initialize_data:
         if rng is None:
             rng = np.random.default_rng(12345)
 
         for gen in range(n_gen):
             pop = setup_population(n_ind, n_vars, n_obj, n_nonlin, n_meta, rng)
-            optimization_results.update_population(pop)
+            optimization_results.update(pop)
             optimization_results.update_pareto()
             if n_meta > 0:
                 optimization_results.update_meta()
 
     return optimization_results
```

### Comparing `CADET-Process-0.8.0/tests/test_parallelization_adapter.py` & `CADET-Process-0.9.0/tests/test_parallelization_adapter.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/tests/test_parameters.py` & `CADET-Process-0.9.0/tests/test_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -592,14 +592,16 @@
         self.model = Model()
 
     def test_value(self):
         self.model.modulated_list = [1, 2, 3, 4]
 
         np.testing.assert_equal(self.model.modulated_list, [1, 2, 3, 4])
 
+        self.model.modulated_list = [1, 2, 3, 4, 5, 6, 7, 8]
+
         with self.assertRaises(ValueError):
             self.model.modulated_list = [1, 2, 3, 4, 5]
 
         self.model.n_mod = 5
         with self.assertRaises(ValueError):
             self.model.modulated_list
```

### Comparing `CADET-Process-0.8.0/tests/test_performance.py` & `CADET-Process-0.9.0/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/tests/test_population.py` & `CADET-Process-0.9.0/tests/test_population.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/tests/test_pymoo.py` & `CADET-Process-0.9.0/tests/test_pymoo.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/tests/test_reaction.py` & `CADET-Process-0.9.0/tests/test_reaction.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/tests/test_sections.py` & `CADET-Process-0.9.0/tests/test_sections.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,49 @@
 import unittest
 
 import numpy as np
 
+from CADETProcess.dynamicEvents.section import generate_indices
 from CADETProcess.dynamicEvents import Section, TimeLine, MultiTimeLine
 
 
+class TestGenerateIndices(unittest.TestCase):
+    def __init__(self, methodName='runTest'):
+        super().__init__(methodName)
+
+    def test_generate_indices(self):
+        shape = (3, 3)
+
+        indices = [[0, 1], [1, 2]]
+        indices_tuple_expected = [(0, 1), (1, 2)]
+        indices_tuple = generate_indices(shape, indices)
+        np.testing.assert_equal(indices_tuple, indices_tuple_expected)
+
+        indices = np.s_[:]
+        indices_tuple_expected = [(slice(None, None, None),)]
+        indices_tuple = generate_indices(shape, indices)
+        np.testing.assert_equal(indices_tuple, indices_tuple_expected)
+
+        indices = np.s_[0, :]
+        indices_tuple_expected = [(0, slice(None, None, None))]
+        indices_tuple = generate_indices(shape, indices)
+        np.testing.assert_equal(indices_tuple, indices_tuple_expected)
+
+        indices = [np.s_[0, :], [1, 1]]
+        indices_tuple_expected = [(0, slice(None, None, None)), (1, 1)]
+        indices_tuple = generate_indices(shape, indices)
+        np.testing.assert_equal(indices_tuple, indices_tuple_expected)
+
+        with self.assertRaises(IndexError):
+            _ = generate_indices(shape, indices=[3, 3])
+
+        with self.assertRaises(ValueError):
+            _ = generate_indices((), indices=[[0, 1], [1, 2]])
+
+
 class TestSection(unittest.TestCase):
     def __init__(self, methodName='runTest'):
         super().__init__(methodName)
 
     def setUp(self):
         self.constant_section_single = Section(0, 1, 1)
         self.constant_section_multi = Section(1, 2, [1, 2])
```

### Comparing `CADET-Process-0.8.0/tests/test_solution.py` & `CADET-Process-0.9.0/tests/test_solution.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/tests/test_transform.py` & `CADET-Process-0.9.0/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.8.0/tests/test_unit_operation.py` & `CADET-Process-0.9.0/tests/test_unit_operation.py`

 * *Files identical despite different names*

