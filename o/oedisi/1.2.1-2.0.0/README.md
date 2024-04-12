# Comparing `tmp/oedisi-1.2.1.tar.gz` & `tmp/oedisi-2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oedisi-1.2.1.tar", last modified: Mon Feb  5 18:03:11 2024, max compression
+gzip compressed data, was "oedisi-2.tar", last modified: Fri Apr 12 17:37:19 2024, max compression
```

## Comparing `oedisi-1.2.1.tar` & `oedisi-2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-02-05 18:03:11.842470 oedisi-1.2.1/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1523 2023-03-15 22:40:58.000000 oedisi-1.2.1/LICENSE.md
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     3305 2024-02-05 18:03:11.841928 oedisi-1.2.1/PKG-INFO
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1433 2023-11-14 18:52:46.000000 oedisi-1.2.1/README.md
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     2374 2024-02-05 18:02:54.000000 oedisi-1.2.1/pyproject.toml
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       38 2024-02-05 18:03:11.842633 oedisi-1.2.1/setup.cfg
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-02-05 18:03:11.788052 oedisi-1.2.1/src/
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-02-05 18:03:11.791200 oedisi-1.2.1/src/oedisi/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       22 2024-02-05 18:02:54.000000 oedisi-1.2.1/src/oedisi/__init__.py
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-02-05 18:03:11.798639 oedisi-1.2.1/src/oedisi/componentframework/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       22 2024-02-05 18:02:54.000000 oedisi-1.2.1/src/oedisi/componentframework/__init__.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     3694 2024-02-01 20:13:20.000000 oedisi-1.2.1/src/oedisi/componentframework/basic_component.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     4413 2024-01-31 22:17:06.000000 oedisi-1.2.1/src/oedisi/componentframework/mock_component.py
--rwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       63 2024-01-31 15:23:02.000000 oedisi-1.2.1/src/oedisi/componentframework/mock_component.sh
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     9675 2024-02-01 20:13:20.000000 oedisi-1.2.1/src/oedisi/componentframework/system_configuration.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     3976 2024-01-31 22:17:06.000000 oedisi-1.2.1/src/oedisi/componentframework/wiring_diagram_utils.py
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-02-05 18:03:11.805230 oedisi-1.2.1/src/oedisi/tools/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       47 2024-02-05 18:02:54.000000 oedisi-1.2.1/src/oedisi/tools/__init__.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-01-31 15:23:02.000000 oedisi-1.2.1/src/oedisi/tools/api.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      951 2024-02-01 20:13:20.000000 oedisi-1.2.1/src/oedisi/tools/broker_utils.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)    17623 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/tools/cli_tools.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     5124 2024-01-31 22:17:06.000000 oedisi-1.2.1/src/oedisi/tools/metrics.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1090 2024-01-31 15:23:02.000000 oedisi-1.2.1/src/oedisi/tools/pausing_broker.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     2018 2024-01-31 22:17:06.000000 oedisi-1.2.1/src/oedisi/tools/testing_broker.py
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-02-05 18:03:11.808329 oedisi-1.2.1/src/oedisi/types/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       22 2024-02-05 18:02:54.000000 oedisi-1.2.1/src/oedisi/types/__init__.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      477 2024-02-01 20:13:20.000000 oedisi-1.2.1/src/oedisi/types/common.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     7547 2024-02-01 20:13:20.000000 oedisi-1.2.1/src/oedisi/types/data_types.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1088 2024-01-31 15:23:02.000000 oedisi-1.2.1/src/oedisi/types/generate_schema.py
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-02-05 18:03:11.838303 oedisi-1.2.1/src/oedisi/types/schemas/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1006 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/AdmittanceMatrix.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1285 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/AdmittanceSparse.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      695 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/CapacitorStates.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1349 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/Command.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1973 2024-01-31 15:23:02.000000 oedisi-1.2.1/src/oedisi/types/schemas/CommandList.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      963 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/CostArray.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1397 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/CurrentsAngle.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1395 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/CurrentsImaginary.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1395 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/CurrentsMagnitude.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1390 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/CurrentsReal.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)    13378 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/Injection.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     3833 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/InverterControl.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     4270 2024-01-31 18:05:05.000000 oedisi-1.2.1/src/oedisi/types/schemas/InverterControlList.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1149 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/MeasurementArray.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      970 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/OperationalCosts.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1534 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/PowersAngle.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1535 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/PowersImaginary.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1534 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/PowersMagnitude.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1528 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/PowersReal.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      975 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/ReactiveCostFunctions.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      977 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/ReactiveWholesalePrices.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      971 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/RealCostFunctions.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      973 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/RealWholesalePrices.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      695 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/RegulatorStates.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1399 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/SolarIrradiances.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      690 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/StateArray.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1398 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/StatesOfCharge.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      692 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/SwitchStates.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1390 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/Temperatures.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)    22562 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/Topology.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1540 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/VVControl.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      680 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/VWControl.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1193 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/VoltagesAngle.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1192 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/VoltagesImaginary.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1192 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/VoltagesMagnitude.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1187 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/VoltagesReal.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1390 2024-01-31 22:18:41.000000 oedisi-1.2.1/src/oedisi/types/schemas/WindSpeeds.json
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-02-05 18:03:11.839239 oedisi-1.2.1/src/oedisi.egg-info/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     3305 2024-02-05 18:03:11.000000 oedisi-1.2.1/src/oedisi.egg-info/PKG-INFO
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     2556 2024-02-05 18:03:11.000000 oedisi-1.2.1/src/oedisi.egg-info/SOURCES.txt
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        1 2024-02-05 18:03:11.000000 oedisi-1.2.1/src/oedisi.egg-info/dependency_links.txt
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       44 2024-02-05 18:03:11.000000 oedisi-1.2.1/src/oedisi.egg-info/entry_points.txt
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      277 2024-02-05 18:03:11.000000 oedisi-1.2.1/src/oedisi.egg-info/requires.txt
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        7 2024-02-05 18:03:11.000000 oedisi-1.2.1/src/oedisi.egg-info/top_level.txt
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-04-12 17:37:19.524960 oedisi-2/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1523 2023-03-15 22:40:58.000000 oedisi-2/LICENSE.md
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     3337 2024-04-12 17:37:19.523977 oedisi-2/PKG-INFO
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1433 2023-11-14 18:52:46.000000 oedisi-2/README.md
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     2396 2024-04-12 17:36:29.000000 oedisi-2/pyproject.toml
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       38 2024-04-12 17:37:19.525177 oedisi-2/setup.cfg
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-04-12 17:37:19.456334 oedisi-2/src/
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-04-12 17:37:19.459841 oedisi-2/src/oedisi/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       22 2024-04-12 17:36:29.000000 oedisi-2/src/oedisi/__init__.py
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-04-12 17:37:19.470725 oedisi-2/src/oedisi/componentframework/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       22 2024-04-12 17:36:29.000000 oedisi-2/src/oedisi/componentframework/__init__.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     3694 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/componentframework/basic_component.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     4413 2024-01-31 22:17:06.000000 oedisi-2/src/oedisi/componentframework/mock_component.py
+-rwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       63 2024-01-31 15:23:02.000000 oedisi-2/src/oedisi/componentframework/mock_component.sh
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     9766 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/componentframework/system_configuration.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     3976 2024-01-31 22:17:06.000000 oedisi-2/src/oedisi/componentframework/wiring_diagram_utils.py
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-04-12 17:37:19.477165 oedisi-2/src/oedisi/tools/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       47 2024-04-12 17:36:29.000000 oedisi-2/src/oedisi/tools/__init__.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-01-31 15:23:02.000000 oedisi-2/src/oedisi/tools/api.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      951 2024-02-16 20:51:42.000000 oedisi-2/src/oedisi/tools/broker_utils.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)    19042 2024-04-11 14:59:42.000000 oedisi-2/src/oedisi/tools/cli_tools.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     5124 2024-03-01 22:51:51.000000 oedisi-2/src/oedisi/tools/metrics.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1090 2024-01-31 15:23:02.000000 oedisi-2/src/oedisi/tools/pausing_broker.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     2018 2024-01-31 22:17:06.000000 oedisi-2/src/oedisi/tools/testing_broker.py
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-04-12 17:37:19.480519 oedisi-2/src/oedisi/types/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       22 2024-04-12 17:36:29.000000 oedisi-2/src/oedisi/types/__init__.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      681 2024-04-11 14:59:42.000000 oedisi-2/src/oedisi/types/common.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     7493 2024-04-11 14:59:37.000000 oedisi-2/src/oedisi/types/data_types.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1088 2024-01-31 15:23:02.000000 oedisi-2/src/oedisi/types/generate_schema.py
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-04-12 17:37:19.518616 oedisi-2/src/oedisi/types/schemas/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1006 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/AdmittanceMatrix.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1285 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/AdmittanceSparse.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      695 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/CapacitorStates.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1349 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/Command.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1973 2024-01-31 15:23:02.000000 oedisi-2/src/oedisi/types/schemas/CommandList.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      963 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/CostArray.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1397 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/CurrentsAngle.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1395 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/CurrentsImaginary.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1395 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/CurrentsMagnitude.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1390 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/CurrentsReal.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)    13378 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/Injection.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     3833 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/InverterControl.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     4270 2024-01-31 18:05:05.000000 oedisi-2/src/oedisi/types/schemas/InverterControlList.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1149 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/MeasurementArray.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      970 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/OperationalCosts.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1534 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/PowersAngle.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1535 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/PowersImaginary.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1534 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/PowersMagnitude.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1528 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/PowersReal.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      975 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/ReactiveCostFunctions.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      977 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/ReactiveWholesalePrices.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      971 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/RealCostFunctions.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      973 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/RealWholesalePrices.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      695 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/RegulatorStates.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1399 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/SolarIrradiances.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      690 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/StateArray.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1398 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/StatesOfCharge.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      692 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/SwitchStates.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1390 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/Temperatures.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)    22562 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/Topology.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1540 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/VVControl.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      680 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/VWControl.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1193 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/VoltagesAngle.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1192 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/VoltagesImaginary.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1192 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/VoltagesMagnitude.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1187 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/VoltagesReal.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1390 2024-02-20 17:41:43.000000 oedisi-2/src/oedisi/types/schemas/WindSpeeds.json
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2024-04-12 17:37:19.519780 oedisi-2/src/oedisi.egg-info/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     3337 2024-04-12 17:37:19.000000 oedisi-2/src/oedisi.egg-info/PKG-INFO
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     2556 2024-04-12 17:37:19.000000 oedisi-2/src/oedisi.egg-info/SOURCES.txt
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        1 2024-04-12 17:37:19.000000 oedisi-2/src/oedisi.egg-info/dependency_links.txt
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       44 2024-04-12 17:37:19.000000 oedisi-2/src/oedisi.egg-info/entry_points.txt
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      294 2024-04-12 17:37:19.000000 oedisi-2/src/oedisi.egg-info/requires.txt
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        7 2024-04-12 17:37:19.000000 oedisi-2/src/oedisi.egg-info/top_level.txt
```

### Comparing `oedisi-1.2.1/LICENSE.md` & `oedisi-2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/PKG-INFO` & `oedisi-2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oedisi
-Version: 1.2.1
+Version: 2.0.0
 Summary: Orchestration interface for HELICS power simulations
 Author-email: Joseph McKinsey <joseph.mckinsey@nrel.gov>
 License: BSD 3-Clause
 Keywords: oedisi,gadal,helics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -20,14 +20,15 @@
 License-File: LICENSE.md
 Requires-Dist: helics-apps>=3.2.1
 Requires-Dist: helics>=3.2.1
 Requires-Dist: pydantic<2,>=1.7
 Requires-Dist: psutil
 Requires-Dist: click
 Requires-Dist: pyyaml~=6.0
+Requires-Dist: kubernetes>=29.0
 Provides-Extra: test
 Requires-Dist: black; extra == "test"
 Requires-Dist: bump-my-version; extra == "test"
 Requires-Dist: ipython; extra == "test"
 Requires-Dist: ipdb; extra == "test"
 Requires-Dist: gamspy; extra == "test"
 Requires-Dist: memory_profiler; extra == "test"
```

### Comparing `oedisi-1.2.1/README.md` & `oedisi-2/README.md`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/pyproject.toml` & `oedisi-2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "oedisi"
-version = "1.2.1"
+version = "2.0.0"
 description = "Orchestration interface for HELICS power simulations"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["oedisi", "gadal", "helics"]
 authors = [{ name = "Joseph McKinsey", email = "joseph.mckinsey@nrel.gov" }]
 classifiers = [
   "Development Status :: 4 - Beta",
@@ -25,14 +25,15 @@
 dependencies = [
   "helics-apps>=3.2.1",
   "helics>=3.2.1",
   "pydantic>=1.7,<2",
   "psutil",
   "click",
   "pyyaml~=6.0",
+  "kubernetes>=29.0",
 ]
 
 [project.license]
 text = "BSD 3-Clause"
 
 [project.optional-dependencies]
 test = [
```

### Comparing `oedisi-1.2.1/src/oedisi/componentframework/basic_component.py` & `oedisi-2/src/oedisi/componentframework/basic_component.py`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/componentframework/mock_component.py` & `oedisi-2/src/oedisi/componentframework/mock_component.py`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/componentframework/system_configuration.py` & `oedisi-2/src/oedisi/componentframework/system_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,17 +116,20 @@
 
     def port(self, port_name: str):
         return Port(name=self.name, port_name=port_name)
 
     @validator("image", pre=True, always=True)
     def validate_image(cls, v, values, **kwargs):
         if not v:
-            return f"{DOCKER_HUB_USER}/{APP_NAME}_{values['name']}:latest"
+            return f"{DOCKER_HUB_USER}/{APP_NAME}_{values['type'].lower()}:latest"
         return v
 
+class ComponentStruct(BaseModel):
+    component : Component
+    links : List[Link]
 
 class WiringDiagram(BaseModel):
     "Cosimulation configuration. This may end up wrapped in another interface"
     name: str
     components: List[Component]
     links: List[Link]
```

### Comparing `oedisi-1.2.1/src/oedisi/componentframework/wiring_diagram_utils.py` & `oedisi-2/src/oedisi/componentframework/wiring_diagram_utils.py`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/tools/broker_utils.py` & `oedisi-2/src/oedisi/tools/broker_utils.py`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/tools/cli_tools.py` & `oedisi-2/src/oedisi/tools/cli_tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 import subprocess
 import shutil
 import click
 import yaml
 import json
 import os
 from pathlib import Path
-
-
-from distutils.dir_util import copy_tree
+from kubernetes import client
+from typing import Any, Dict
 
 from oedisi.componentframework.basic_component import (
     basic_component,
     ComponentDescription,
 )
+
 from oedisi.componentframework.mock_component import MockComponent
 from oedisi.componentframework.system_configuration import (
     RunnerConfig,
     generate_runner_config,
     WiringDiagram,
     Component,
 )
+
+
 from .pausing_broker import PausingBroker
 from .testing_broker import TestingBroker
 from .metrics import evaluate_estimate
 
 from oedisi.types.common import (
     APP_NAME,
     BASE_DOCKER_IMAGE,
     BROKER_SERVICE,
     DOCKER_HUB_USER,
+    KUBERNETES_SERVICE_NAME,
 )
 
-
 @click.group()
 def cli():
     pass
 
 
 def bad_type_checker(type, x):
     "Does not check types"
@@ -82,15 +84,14 @@
 )
 def build(
     target_directory,
     system,
     component_dict,
     multi_container,
     broker_port,
-    node_port=30000,
 ):
     """Build to the simulation folder
 
     Examples::
 
         oedisi build
 
@@ -106,168 +107,213 @@
         path to wiring diagram json
     component_dict : str (default="components.json")
         path to JSON dictionary of component folders
     multi_container: bool
         A boolean specifying whether or not we're using the multi-container approach
     broker_port: float
         The port of the broker. If using kubernetes, is internal to k8s
-    node_port: float (default=30000)
-        The port exposed externally from k8s for external access on localhost
     """
     click.echo(f"Loading the components defined in {component_dict}")
     with open(component_dict, "r") as f:
         component_dict_of_files = json.load(f)
         component_types = {
             name: get_basic_component(component_file)
             for name, component_file in component_dict_of_files.items()
         }
-
+    
     click.echo(f"Loading system json {system}")
     wiring_diagram = WiringDiagram.parse_file(system)
 
     click.echo(f"Building system in {target_directory}")
-
-    runner_config = generate_runner_config(
-        wiring_diagram, component_types, target_directory=target_directory
-    )
-
-    with open(f"{target_directory}/system_runner.json", "w") as f:
-        f.write(runner_config.json(indent=2))
-
-    yaml_file_path = f"{target_directory}/docker-compose.yml"
-
+    
     if multi_container:
+        if not Path(target_directory).exists():
+            os.mkdir(target_directory)
         validate_optional_inputs(wiring_diagram, component_dict_of_files)
-        edit_docker_files(wiring_diagram, target_directory)
-        create_docker_compose_file(wiring_diagram, target_directory, broker_port)
-        clone_broker(yaml_file_path, target_directory)
+        edit_docker_files(wiring_diagram, component_types)
+        create_docker_compose_file(wiring_diagram, target_directory, broker_port, component_types)
         create_kubernetes_deployment(
-            wiring_diagram, target_directory, broker_port, node_port
+            wiring_diagram, target_directory, broker_port
         )
 
+    else:
+        runner_config = generate_runner_config(
+            wiring_diagram, component_types, target_directory=target_directory
+        )
+
+        with open(f"{target_directory}/system_runner.json", "w") as f:
+            f.write(runner_config.json(indent=2))
 
 def validate_optional_inputs(
     wiring_diagram: WiringDiagram, component_dict_of_files: dict
 ):
     for component in wiring_diagram.components:
         assert hasattr(
             component, "host"
         ), f"host parameter required for component {component.name} for multi-continer model build"
         assert hasattr(
             component, "container_port"
         ), f"post parameter required for component {component.name} for multi-continer model build"
 
 
+def drop_null_values(model: Any)-> dict:
+    clean_model = {}
+    assert isinstance(model, dict), "input to this function should be a dict"
+    for k, v in model.items():
+        if "_" in k:
+            key_name = k.split("_")
+            if len(key_name[1]) > 2:
+                key_name[1] = key_name[1].capitalize()
+            else:
+                key_name[1] = key_name[1].upper()
+            key_name = "".join(key_name)
+        else:
+            key_name = k    
+                
+        if isinstance(v, dict):
+            clean_model[key_name] = drop_null_values(v)
+        elif isinstance(v, list):
+            new_list = []
+            for val in v:
+                new_list.append(drop_null_values(val))
+            clean_model[key_name] = new_list
+        elif v is not None:
+            clean_model[key_name] = v
+    return clean_model
+
 def create_kubernetes_deployment(
-    wiring_diagram: WiringDiagram, target_directory, broker_port, node_port
+    wiring_diagram: WiringDiagram, target_directory:Path|str, broker_port:int
 ):
     kube_folder = os.path.join(target_directory, "kubernetes")
     if not os.path.exists(kube_folder):
         os.mkdir(kube_folder)
+    
+    service = client.V1Service(
+        api_version="v1",
+        kind="Service",
+        metadata= client.V1ObjectMeta(
+            name = KUBERNETES_SERVICE_NAME
+        ),
+        spec=client.V1ServiceSpec(
+            cluster_ip="None",
+            selector={"app" : APP_NAME},
+        ),
+    )
 
-    service = {
-        "apiVersion": "v1",
-        "kind": "Service",
-        "metadata": {
-            "name": f"{APP_NAME}-service",
-        },
-        "spec": {
-            "type": "NodePort",
-            "selector": {"app": APP_NAME},
-            "ports": [{"port": broker_port, "nodePort": node_port}],
-        },
-    }
+    service_dict = drop_null_values(service.to_dict())
+    with open(os.path.join(kube_folder, f"service.yml"), "w") as f:
+        yaml.dump(service_dict, f)
+
+    broker_component = Component(
+        name=BROKER_SERVICE,
+        container_port=broker_port,
+        type = BROKER_SERVICE,
+        parameters={}
+    )
+    create_single_kubernestes_deyployment(broker_component, kube_folder)
+    for component in wiring_diagram.components:
+        create_single_kubernestes_deyployment(component, kube_folder)
+        
 
-    deployment = {
-        "apiVersion": "apps/v1",
-        "kind": "Deployment",
-        "metadata": {"name": f"{APP_NAME}-deployment", "labels": {"app": APP_NAME}},
-        "spec": {
-            "replicas": 1,
-            "selector": {"matchLabels": {"app": APP_NAME}},
-            "template": {
-                "metadata": {"labels": {"app": APP_NAME}},
-                "spec": {"containers": []},
-            },
-        },
-    }
+def create_single_kubernestes_deyployment(component:Component, kube_folder:Path|str):
 
-    container = {}
-    for component in wiring_diagram.components:
-        container["name"] = component.name.replace("_", "-")
-        container["image"] = component.image
-        container["ports"] = [{"containerPort": component.container_port}]
-        deployment["spec"]["template"]["spec"]["containers"].append(container.copy())
-
-    container["name"] = BROKER_SERVICE.replace("_", "-")
-    container["image"] = f"{DOCKER_HUB_USER}/{APP_NAME}_{BROKER_SERVICE}:latest"
-    container["ports"] = [{"containerPort": broker_port}]
-    deployment["spec"]["template"]["spec"]["containers"].append(container.copy())
-
-    with open(os.path.join(kube_folder, "deployment.yml"), "w") as f:
-        yaml.dump(deployment, f)
-    with open(os.path.join(kube_folder, "service.yml"), "w") as f:
-        yaml.dump(service, f)
-
-
-def clone_broker(yaml_file_path, target_directory):
-    broker_folder = os.path.join(target_directory, "broker")
-    if not os.path.exists(broker_folder):
-        os.makedirs(broker_folder)
-    copy_tree("./broker", broker_folder)
-    shutil.copy(yaml_file_path, broker_folder)
-    return
+    fixed_container_name =  component.name.replace("_", "-")
+    my_container = client.V1Container(            
+        name = fixed_container_name,
+        image = component.image,
+        env = [
+            client.V1EnvVar(
+                name="PORT", 
+                value=str(component.container_port)
+            ),
+            client.V1EnvVar(
+                name="SERVICE_NAME", 
+                value=KUBERNETES_SERVICE_NAME,
+            )
+        ],
+        ports =  [
+            client.V1ContainerPort(
+                container_port = component.container_port
+            )],
+        )
+    
+    pod = client.V1Pod(
+        api_version="v1",
+        kind="Pod",
+        metadata=client.V1ObjectMeta(
+            name=f"{fixed_container_name}-pod",
+            labels ={"app" : APP_NAME},
+        ),
+        spec=client.V1PodSpec(
+            containers=[my_container],
+            hostname=component.name.replace("_", "-"),
+            subdomain="oedisi-service",
+            ),
+        )
 
+    pod_dict = drop_null_values(pod.to_dict())
+    with open(os.path.join(kube_folder, f"{component.name}.yml"), "w") as f:
+        yaml.dump(pod_dict, f)
 
 def edit_docker_file(file_path, component: Component):
+ 
     dir_path = os.path.abspath(os.path.join(file_path, os.pardir))
     server_file = os.path.join(dir_path, "server.py")
     assert os.path.exists(
         server_file
     ), f"Server.py file missing for {component.name}.REST API implementation expected in a server.py file"
 
     with open(file_path, "w") as f:
         f.write(f"FROM {BASE_DOCKER_IMAGE}\n")
         f.write(f"RUN apt-get update\n")
         f.write(f"RUN apt-get install -y git ssh\n")
-        f.write(f"RUN mkdir {component.name}\n")
-        f.write(f"COPY  . ./{component.name}\n")
-        f.write(f"WORKDIR ./{component.name}\n")
+        f.write(f"RUN mkdir {component.type}\n")
+        f.write(f"COPY  . ./{component.type}\n")
+        f.write(f"WORKDIR ./{component.type}\n")
         f.write(f"RUN pip install -r requirements.txt\n")
         f.write(f"EXPOSE {component.container_port}/tcp\n")
-        cmd = f'CMD {["python", "server.py", component.host, str(component.container_port)]}\n'
+        cmd = f'CMD {["python", "server.py"]}\n'
         cmd = cmd.replace("'", '"')
         f.write(cmd)
     pass
 
 
-def edit_docker_files(wiring_diagram: WiringDiagram, target_directory: str):
+def edit_docker_files(wiring_diagram: WiringDiagram, component_types: Dict):
+    parsed_components  = []
     for component in wiring_diagram.components:
-        docker_path = os.path.join(target_directory, component.name, "Dockerfile")
-        edit_docker_file(docker_path, component)
+        if component.type not in parsed_components:
+            parsed_components.append(component.type)
+            component_type = component_types[component.type]
+            docker_path = os.path.join(component_type._origin_directory, "Dockerfile")
+            edit_docker_file(docker_path, component)
 
 
 def create_docker_compose_file(
-    wiring_diagram: WiringDiagram, target_directory: str, broker_port: int
+    wiring_diagram: WiringDiagram, target_directory: str, broker_port: int, component_types: Dict
 ):
     config = {"services": {}, "networks": {}}
 
     config["services"][f"{APP_NAME}_{BROKER_SERVICE}"] = {
-        "build": {"context": f"./broker/."},
+        "build": {"context": f"../{BROKER_SERVICE}/."},
         "image": f"{DOCKER_HUB_USER}/{APP_NAME}_{BROKER_SERVICE}",
+        "hostname" : f"{BROKER_SERVICE}",
+        "environment" : {"PORT": str(broker_port)},
         "ports": [f"{broker_port}:{broker_port}"],
-        "networks": {"custom-network": {"ipv4_address": "10.5.0.2"}},
+        "networks": {"custom-network": {}},
     }
 
     for component in wiring_diagram.components:
+        component_type = component_types[component.type]
         config["services"][f"{APP_NAME}_{component.name}"] = {
-            "build": {"context": f"./{component.name}/."},
+            "build": {"context": f"../{component_type._origin_directory}/."},
             "image": f"{component.image}",
+            "hostname" : f"{component.name.replace("_", "-")}",
+            "environment" : {"PORT": str(component.container_port)},
             "ports": [f"{component.container_port}:{component.container_port}"],
-            "networks": {"custom-network": {"ipv4_address": component.host}},
+            "networks": {"custom-network": {}},
         }
 
     config["networks"] = {
         "custom-network": {
             "driver": "bridge",
             "ipam": {
                 "config": [
@@ -278,14 +324,15 @@
                 ]
             },
         }
     }
     yaml_file_path = f"{target_directory}/docker-compose.yml"
     with open(yaml_file_path, "w") as file:
         yaml.dump(config, file)
+ 
     return yaml_file_path
 
 
 @cli.command()
 @click.option(
     "--runner",
     default="build/system_runner.json",
```

### Comparing `oedisi-1.2.1/src/oedisi/tools/metrics.py` & `oedisi-2/src/oedisi/tools/metrics.py`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/tools/pausing_broker.py` & `oedisi-2/src/oedisi/tools/pausing_broker.py`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/tools/testing_broker.py` & `oedisi-2/src/oedisi/tools/testing_broker.py`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/data_types.py` & `oedisi-2/src/oedisi/types/data_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,15 +269,15 @@
     obj_name -- name of the object.
     obj_prop -- name of the property.
     obj_val -- val of the property.
     """
 
     obj_name: str
     obj_property: str
-    val: Union[int, float, str, List[int], List[float], List[str]]
+    val: str
 
 
 class CommandList(BaseModel):
     """List[Command] with JSON parsing."""
 
     __root__: List[Command]
```

### Comparing `oedisi-1.2.1/src/oedisi/types/generate_schema.py` & `oedisi-2/src/oedisi/types/generate_schema.py`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/AdmittanceMatrix.json` & `oedisi-2/src/oedisi/types/schemas/AdmittanceMatrix.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/AdmittanceSparse.json` & `oedisi-2/src/oedisi/types/schemas/AdmittanceSparse.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/CapacitorStates.json` & `oedisi-2/src/oedisi/types/schemas/CapacitorStates.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/Command.json` & `oedisi-2/src/oedisi/types/schemas/Command.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/CommandList.json` & `oedisi-2/src/oedisi/types/schemas/CommandList.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/CostArray.json` & `oedisi-2/src/oedisi/types/schemas/CostArray.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/CurrentsAngle.json` & `oedisi-2/src/oedisi/types/schemas/CurrentsAngle.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/CurrentsImaginary.json` & `oedisi-2/src/oedisi/types/schemas/CurrentsImaginary.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/CurrentsMagnitude.json` & `oedisi-2/src/oedisi/types/schemas/CurrentsMagnitude.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/CurrentsReal.json` & `oedisi-2/src/oedisi/types/schemas/CurrentsReal.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/Injection.json` & `oedisi-2/src/oedisi/types/schemas/Injection.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/InverterControl.json` & `oedisi-2/src/oedisi/types/schemas/InverterControl.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/InverterControlList.json` & `oedisi-2/src/oedisi/types/schemas/InverterControlList.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/MeasurementArray.json` & `oedisi-2/src/oedisi/types/schemas/MeasurementArray.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/OperationalCosts.json` & `oedisi-2/src/oedisi/types/schemas/OperationalCosts.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/PowersAngle.json` & `oedisi-2/src/oedisi/types/schemas/PowersAngle.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/PowersImaginary.json` & `oedisi-2/src/oedisi/types/schemas/PowersImaginary.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/PowersMagnitude.json` & `oedisi-2/src/oedisi/types/schemas/PowersMagnitude.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/PowersReal.json` & `oedisi-2/src/oedisi/types/schemas/PowersReal.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/ReactiveCostFunctions.json` & `oedisi-2/src/oedisi/types/schemas/ReactiveCostFunctions.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/ReactiveWholesalePrices.json` & `oedisi-2/src/oedisi/types/schemas/ReactiveWholesalePrices.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/RealCostFunctions.json` & `oedisi-2/src/oedisi/types/schemas/RealCostFunctions.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/RealWholesalePrices.json` & `oedisi-2/src/oedisi/types/schemas/RealWholesalePrices.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/RegulatorStates.json` & `oedisi-2/src/oedisi/types/schemas/RegulatorStates.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/SolarIrradiances.json` & `oedisi-2/src/oedisi/types/schemas/SolarIrradiances.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/StateArray.json` & `oedisi-2/src/oedisi/types/schemas/StateArray.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/StatesOfCharge.json` & `oedisi-2/src/oedisi/types/schemas/StatesOfCharge.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/SwitchStates.json` & `oedisi-2/src/oedisi/types/schemas/SwitchStates.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/Temperatures.json` & `oedisi-2/src/oedisi/types/schemas/Temperatures.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/Topology.json` & `oedisi-2/src/oedisi/types/schemas/Topology.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/VVControl.json` & `oedisi-2/src/oedisi/types/schemas/VVControl.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/VWControl.json` & `oedisi-2/src/oedisi/types/schemas/VWControl.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/VoltagesAngle.json` & `oedisi-2/src/oedisi/types/schemas/VoltagesAngle.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/VoltagesImaginary.json` & `oedisi-2/src/oedisi/types/schemas/VoltagesImaginary.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/VoltagesMagnitude.json` & `oedisi-2/src/oedisi/types/schemas/VoltagesMagnitude.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/VoltagesReal.json` & `oedisi-2/src/oedisi/types/schemas/VoltagesReal.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi/types/schemas/WindSpeeds.json` & `oedisi-2/src/oedisi/types/schemas/WindSpeeds.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.2.1/src/oedisi.egg-info/PKG-INFO` & `oedisi-2/src/oedisi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oedisi
-Version: 1.2.1
+Version: 2.0.0
 Summary: Orchestration interface for HELICS power simulations
 Author-email: Joseph McKinsey <joseph.mckinsey@nrel.gov>
 License: BSD 3-Clause
 Keywords: oedisi,gadal,helics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -20,14 +20,15 @@
 License-File: LICENSE.md
 Requires-Dist: helics-apps>=3.2.1
 Requires-Dist: helics>=3.2.1
 Requires-Dist: pydantic<2,>=1.7
 Requires-Dist: psutil
 Requires-Dist: click
 Requires-Dist: pyyaml~=6.0
+Requires-Dist: kubernetes>=29.0
 Provides-Extra: test
 Requires-Dist: black; extra == "test"
 Requires-Dist: bump-my-version; extra == "test"
 Requires-Dist: ipython; extra == "test"
 Requires-Dist: ipdb; extra == "test"
 Requires-Dist: gamspy; extra == "test"
 Requires-Dist: memory_profiler; extra == "test"
```

### Comparing `oedisi-1.2.1/src/oedisi.egg-info/SOURCES.txt` & `oedisi-2/src/oedisi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

