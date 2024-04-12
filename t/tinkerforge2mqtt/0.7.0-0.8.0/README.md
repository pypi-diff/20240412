# Comparing `tmp/tinkerforge2mqtt-0.7.0.tar.gz` & `tmp/tinkerforge2mqtt-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinkerforge2mqtt-0.7.0.tar", last modified: Wed Mar 27 11:37:14 2024, max compression
+gzip compressed data, was "tinkerforge2mqtt-0.8.tar", last modified: Fri Apr 12 16:47:54 2024, max compression
```

## Comparing `tinkerforge2mqtt-0.7.0.tar` & `tinkerforge2mqtt-0.8.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-03-27 11:37:14.151917 tinkerforge2mqtt-0.7.0/
--rw-rw-r--   0 jens      (1000) users      (100)      310 2024-03-08 19:27:47.000000 tinkerforge2mqtt-0.7.0/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2024-03-08 19:27:47.000000 tinkerforge2mqtt-0.7.0/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-03-27 11:37:14.147917 tinkerforge2mqtt-0.7.0/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-03-27 11:37:14.147917 tinkerforge2mqtt-0.7.0/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1670 2024-03-12 08:31:19.000000 tinkerforge2mqtt-0.7.0/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      116 2024-03-08 19:27:47.000000 tinkerforge2mqtt-0.7.0/.gitignore
--rw-r--r--   0 jens      (1000) users      (100)     3731 2024-03-27 11:37:14.151917 tinkerforge2mqtt-0.7.0/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)     2404 2024-03-26 08:26:20.000000 tinkerforge2mqtt-0.7.0/README.md
--rwxrwxr-x   0 jens      (1000) users      (100)     3159 2024-03-13 18:56:57.000000 tinkerforge2mqtt-0.7.0/cli.py
--rwxrwxr-x   0 jens      (1000) users      (100)     3089 2024-03-12 08:31:08.000000 tinkerforge2mqtt-0.7.0/dev-cli.py
--rw-rw-r--   0 jens      (1000) users      (100)     4935 2024-03-27 11:29:05.000000 tinkerforge2mqtt-0.7.0/pyproject.toml
--rw-rw-r--   0 jens      (1000) users      (100)    74913 2024-03-27 11:29:38.000000 tinkerforge2mqtt-0.7.0/requirements.dev.txt
--rw-rw-r--   0 jens      (1000) users      (100)    11451 2024-03-27 11:29:21.000000 tinkerforge2mqtt-0.7.0/requirements.txt
--rw-rw-r--   0 jens      (1000) users      (100)       38 2024-03-27 11:37:14.151917 tinkerforge2mqtt-0.7.0/setup.cfg
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-03-27 11:37:14.147917 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/
--rw-rw-r--   0 jens      (1000) users      (100)      137 2024-03-27 11:31:37.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      178 2024-03-12 08:25:52.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/__main__.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-03-27 11:37:14.147917 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/cli_app/
--rw-rw-r--   0 jens      (1000) users      (100)     1364 2024-03-12 08:25:52.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/cli_app/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     3981 2024-03-13 18:56:57.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/cli_app/discovering.py
--rw-rw-r--   0 jens      (1000) users      (100)     2563 2024-03-23 12:12:57.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/cli_app/publish.py
--rw-rw-r--   0 jens      (1000) users      (100)     1395 2024-03-12 08:36:23.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/cli_app/settings.py
--rw-rw-r--   0 jens      (1000) users      (100)     2486 2024-03-12 08:36:51.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/cli_app/systemd.py
--rw-rw-r--   0 jens      (1000) users      (100)      806 2024-03-12 08:25:52.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/cli_app/update_readme_history.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-03-27 11:37:14.151917 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/cli_dev/
--rw-rw-r--   0 jens      (1000) users      (100)     2163 2024-03-23 12:13:34.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/cli_dev/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      968 2024-03-12 08:25:52.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/cli_dev/code_style.py
--rw-rw-r--   0 jens      (1000) users      (100)     2325 2024-03-16 07:49:08.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/cli_dev/packaging.py
--rw-rw-r--   0 jens      (1000) users      (100)     1520 2024-03-12 08:25:52.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/cli_dev/testing.py
--rw-rw-r--   0 jens      (1000) users      (100)      179 2024-03-10 18:32:00.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/constants.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-03-27 11:37:14.151917 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_map/
--rw-rw-r--   0 jens      (1000) users      (100)     1236 2024-03-13 18:56:57.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_map/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1949 2024-03-27 11:30:50.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_map/brick_hat_zero.py
--rw-rw-r--   0 jens      (1000) users      (100)     2820 2024-03-27 11:30:50.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_map/bricklet_humidity_v2.py
--rw-rw-r--   0 jens      (1000) users      (100)     2817 2024-03-27 11:30:50.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_map/bricklet_industrial_dual_relay.py
--rw-rw-r--   0 jens      (1000) users      (100)     1998 2024-03-27 11:30:50.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_map/bricklet_motion_detector_v2.py
--rw-rw-r--   0 jens      (1000) users      (100)     2332 2024-03-27 11:30:50.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_map/bricklet_solid_state_relay_v2.py
--rw-rw-r--   0 jens      (1000) users      (100)     1903 2024-03-27 11:30:50.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_map/bricklet_temperature_v2.py
--rw-rw-r--   0 jens      (1000) users      (100)     3677 2024-03-27 11:30:50.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_map/bricklet_voltage_current_v2.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-03-27 11:37:14.151917 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_map_utils/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2024-03-13 18:56:57.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_map_utils/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     4214 2024-03-27 11:30:50.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_map_utils/base.py
--rw-rw-r--   0 jens      (1000) users      (100)      566 2024-03-13 18:56:57.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_map_utils/generics.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-03-27 11:37:14.151917 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_registry/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2024-03-13 18:56:57.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_registry/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2664 2024-03-25 16:32:13.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_registry/devices_handler.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-03-27 11:37:14.151917 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/tests/
--rw-rw-r--   0 jens      (1000) users      (100)     1197 2024-03-08 19:27:47.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      227 2024-03-10 18:32:00.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/tests/test_doctests.py
--rw-rw-r--   0 jens      (1000) users      (100)     1478 2024-03-12 08:25:52.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/tests/test_project_setup.py
--rw-rw-r--   0 jens      (1000) users      (100)     1227 2024-03-25 16:26:57.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/user_settings.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-03-27 11:37:14.151917 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt.egg-info/
--rw-r--r--   0 jens      (1000) users      (100)     3731 2024-03-27 11:37:14.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)     1676 2024-03-27 11:37:14.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1000) users      (100)        1 2024-03-27 11:37:14.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1000) users      (100)      125 2024-03-27 11:37:14.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt.egg-info/entry_points.txt
--rw-rw-r--   0 jens      (1000) users      (100)      270 2024-03-27 11:37:14.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt.egg-info/requires.txt
--rw-rw-r--   0 jens      (1000) users      (100)       17 2024-03-27 11:37:14.000000 tinkerforge2mqtt-0.7.0/tinkerforge2mqtt.egg-info/top_level.txt
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-12 16:47:54.287756 tinkerforge2mqtt-0.8/
+-rw-rw-r--   0 jens      (1000) users      (100)      310 2024-03-08 19:27:47.000000 tinkerforge2mqtt-0.8/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2024-03-08 19:27:47.000000 tinkerforge2mqtt-0.8/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-12 16:47:54.283756 tinkerforge2mqtt-0.8/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-12 16:47:54.287756 tinkerforge2mqtt-0.8/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1670 2024-03-12 08:31:19.000000 tinkerforge2mqtt-0.8/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      116 2024-03-08 19:27:47.000000 tinkerforge2mqtt-0.8/.gitignore
+-rw-r--r--   0 jens      (1000) users      (100)     3731 2024-04-12 16:47:54.287756 tinkerforge2mqtt-0.8/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     2404 2024-03-26 08:26:20.000000 tinkerforge2mqtt-0.8/README.md
+-rwxrwxr-x   0 jens      (1000) users      (100)     3159 2024-03-13 18:56:57.000000 tinkerforge2mqtt-0.8/cli.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     3089 2024-03-12 08:31:08.000000 tinkerforge2mqtt-0.8/dev-cli.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4935 2024-03-27 11:29:05.000000 tinkerforge2mqtt-0.8/pyproject.toml
+-rw-rw-r--   0 jens      (1000) users      (100)    75311 2024-04-12 16:47:21.000000 tinkerforge2mqtt-0.8/requirements.dev.txt
+-rw-rw-r--   0 jens      (1000) users      (100)    11451 2024-04-12 16:47:21.000000 tinkerforge2mqtt-0.8/requirements.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       38 2024-04-12 16:47:54.287756 tinkerforge2mqtt-0.8/setup.cfg
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-12 16:47:54.287756 tinkerforge2mqtt-0.8/tinkerforge2mqtt/
+-rw-rw-r--   0 jens      (1000) users      (100)      137 2024-04-12 16:43:07.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      178 2024-03-12 08:25:52.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/__main__.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-12 16:47:54.287756 tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_app/
+-rw-rw-r--   0 jens      (1000) users      (100)     1364 2024-03-12 08:25:52.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_app/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3981 2024-03-13 18:56:57.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_app/discovering.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2563 2024-03-23 12:12:57.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_app/publish.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1395 2024-03-12 08:36:23.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_app/settings.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2486 2024-03-12 08:36:51.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_app/systemd.py
+-rw-rw-r--   0 jens      (1000) users      (100)      806 2024-03-12 08:25:52.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_app/update_readme_history.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-12 16:47:54.287756 tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_dev/
+-rw-rw-r--   0 jens      (1000) users      (100)     2163 2024-03-23 12:13:34.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_dev/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      968 2024-03-12 08:25:52.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_dev/code_style.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2325 2024-03-16 07:49:08.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_dev/packaging.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1520 2024-03-12 08:25:52.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_dev/testing.py
+-rw-rw-r--   0 jens      (1000) users      (100)      179 2024-03-10 18:32:00.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/constants.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-12 16:47:54.287756 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/
+-rw-rw-r--   0 jens      (1000) users      (100)     1236 2024-03-13 18:56:57.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1949 2024-03-27 11:30:50.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/brick_hat_zero.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2848 2024-04-12 16:46:27.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/bricklet_analog_in_v3.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2820 2024-03-27 11:30:50.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/bricklet_humidity_v2.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2817 2024-03-27 11:30:50.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/bricklet_industrial_dual_relay.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1998 2024-03-27 11:30:50.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/bricklet_motion_detector_v2.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2332 2024-03-27 11:30:50.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/bricklet_solid_state_relay_v2.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1903 2024-03-27 11:30:50.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/bricklet_temperature_v2.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3677 2024-03-27 11:30:50.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/bricklet_voltage_current_v2.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-12 16:47:54.287756 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map_utils/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2024-03-13 18:56:57.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map_utils/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4214 2024-03-27 11:30:50.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map_utils/base.py
+-rw-rw-r--   0 jens      (1000) users      (100)      566 2024-03-13 18:56:57.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map_utils/generics.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-12 16:47:54.287756 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_registry/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2024-03-13 18:56:57.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_registry/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2664 2024-03-25 16:32:13.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_registry/devices_handler.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-12 16:47:54.287756 tinkerforge2mqtt-0.8/tinkerforge2mqtt/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)     1197 2024-03-08 19:27:47.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      227 2024-03-10 18:32:00.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/tests/test_doctests.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1478 2024-03-12 08:25:52.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/tests/test_project_setup.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1227 2024-03-25 16:26:57.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/user_settings.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-12 16:47:54.287756 tinkerforge2mqtt-0.8/tinkerforge2mqtt.egg-info/
+-rw-r--r--   0 jens      (1000) users      (100)     3731 2024-04-12 16:47:54.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     1729 2024-04-12 16:47:54.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        1 2024-04-12 16:47:54.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      125 2024-04-12 16:47:54.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt.egg-info/entry_points.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      270 2024-04-12 16:47:54.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       17 2024-04-12 16:47:54.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt.egg-info/top_level.txt
```

### Comparing `tinkerforge2mqtt-0.7.0/.github/workflows/tests.yml` & `tinkerforge2mqtt-0.8/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/PKG-INFO` & `tinkerforge2mqtt-0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinkerforge2mqtt
-Version: 0.7.0
+Version: 0.8.0
 Summary: Emit MQTT events from Tinkerforge devices
 Author-email: Jens Diemer <git@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/tinkerforge2mqtt
 Project-URL: Source, https://github.com/jedie/tinkerforge2mqtt
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `tinkerforge2mqtt-0.7.0/README.md` & `tinkerforge2mqtt-0.8/README.md`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/cli.py` & `tinkerforge2mqtt-0.8/cli.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/dev-cli.py` & `tinkerforge2mqtt-0.8/dev-cli.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/pyproject.toml` & `tinkerforge2mqtt-0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/requirements.dev.txt` & `tinkerforge2mqtt-0.8/requirements.dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,18 @@
     # via manageprojects
 autopep8==2.1.0 \
     --hash=sha256:1fa8964e4618929488f4ec36795c7ff12924a68b8bf01366c094fc52f770b6e7 \
     --hash=sha256:2bb76888c5edbcafe6aabab3c47ba534f5a2c2d245c2eddced4a30c4b4946357
     # via
     #   manageprojects
     #   tinkerforge2mqtt (pyproject.toml)
+backports-tarfile==1.0.0 \
+    --hash=sha256:2688f159c21afd56a07b75f01306f9f52c79aebcc5f4a117fb8fbb4445352c75 \
+    --hash=sha256:bcd36290d9684beb524d3fe74f4a2db056824c47746583f090b8e55daf0776e4
+    # via jaraco-context
 binaryornot==0.4.4 \
     --hash=sha256:359501dfc9d40632edc9fac890e19542db1a287bbcfa58175b66658392018061 \
     --hash=sha256:b8b71173c917bddcd2c16070412e369c3ed7f0528926f70cac18a6c97fd563e4
     # via cookiecutter
 black==24.3.0 \
     --hash=sha256:2818cf72dfd5d289e48f37ccfa08b460bf469e67fb7c4abb07edc2e9f16fb63f \
     --hash=sha256:41622020d7120e01d377f74249e677039d20e6344ff5851de8a10f11f513bf93 \
@@ -61,20 +65,18 @@
     --hash=sha256:b5991d523eee14756f3c8d5df5231550ae8993e2286b8014e2fdea7156ed0959 \
     --hash=sha256:bf21b7b230718a5f08bd32d5e4f1db7fc8788345c8aea1d155fc17852b3410f5 \
     --hash=sha256:c45f8dff244b3c431b36e3224b6be4a127c6aca780853574c00faf99258041eb \
     --hash=sha256:c7ed6668cbbfcd231fa0dc1b137d3e40c04c7f786e626b405c62bcd5db5857e4 \
     --hash=sha256:d7de8d330763c66663661a1ffd432274a2f92f07feeddd89ffd085b5744f85e7 \
     --hash=sha256:e19cb1c6365fd6dc38a6eae2dcb691d7d83935c10215aef8e6c38edee3f77abd \
     --hash=sha256:e2af80566f43c85f5797365077fb64a393861a3730bd110971ab7a0c94e873e7
-    # via
-    #   darker
-    #   darkgraylib
-build==1.1.1 \
-    --hash=sha256:8ed0851ee76e6e38adce47e4bee3b51c771d86c64cf578d0c2245567ee200e73 \
-    --hash=sha256:8eea65bb45b1aac2e734ba2cc8dad3a6d97d97901a395bd0ed3e7b46953d2a31
+    # via darker
+build==1.2.1 \
+    --hash=sha256:526263f4870c26f26c433545579475377b2b7588b6f1eac76a001e873ae3e19d \
+    --hash=sha256:75e10f767a433d9a86e50d83f418e83efc18ede923ee5ff7df93b6cb0306c5d4
     # via pip-tools
 bx-py-utils==92 \
     --hash=sha256:38641b2e1a09ed0c64cd6ba0e03c97fea347302439db0234a0492c365ae32719 \
     --hash=sha256:849c59429af6ca0bf35265569884193c60be578285a66b533146e5782a10637b
     # via
     #   cli-base-utilities
     #   tinkerforge2mqtt (pyproject.toml)
@@ -359,48 +361,48 @@
     --hash=sha256:e4985a790f921508f36f81831817cbc03b102d643b5fcb81cd33df3fa291a1a1 \
     --hash=sha256:e807b3188f9eb0eaa7bbb579b462c5ace579f1cedb28107ce8b48a9f7ad3679e \
     --hash=sha256:f12764b8fffc7a123f641d7d049d382b73f96a34117e0b637b80643169cec8ac \
     --hash=sha256:f8837fe1d6ac4a8052a9a8ddab256bc006242696f03368a4009be7ee3075cdb7
     # via
     #   authlib
     #   secretstorage
-darker[color,flynt,isort]==2.0.0 \
-    --hash=sha256:d3f01a7cd777aa6e37a96ee35651926629dfb31e3d14adb1ae174aa2214f79eb \
-    --hash=sha256:d420bcd6058a46a3966ee15630bc20d24279a960460fe6904f3a90ab7cad0496
+darker[color,flynt,isort]==2.1.0 \
+    --hash=sha256:13ce2f14ac416d3032b7bc12d650a098416794df1f40308bd7818a17162fb639 \
+    --hash=sha256:29eaaeb00d0dc6b15e0fd64f00ed6359707b35b8962a387794a26b59da281057
     # via
     #   manageprojects
     #   tinkerforge2mqtt (pyproject.toml)
-darkgraylib==1.0.0 \
-    --hash=sha256:6807988669d206f4b0339e1be0176cd43480e92916c569fdcd1c12548ebe18c2 \
-    --hash=sha256:7cb05ce909ad7ec6c794b2de3912d500a1679cfb244c5ca21b286b461453a242
+darkgraylib==1.1.1 \
+    --hash=sha256:240b993a5492b3f6f68f305a409e87d146fc55768368dd783483bda0ae38ea5d \
+    --hash=sha256:471c7934907a99bb282bb8649dad5ab71e028cdbef51d01c160f63f958709ec6
     # via
     #   darker
     #   graylint
 distlib==0.3.8 \
     --hash=sha256:034db59a0b96f8ca18035f36290806a9a6e6bd9d1ff91e45a7f172eb17e51784 \
     --hash=sha256:1530ea13e350031b6312d8580ddb6b27a104275a31106523b8f123787f494f64
     # via virtualenv
-docutils==0.20.1 \
-    --hash=sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6 \
-    --hash=sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b
+docutils==0.21.1 \
+    --hash=sha256:14c8d34a55b46c88f9f714adb29cefbdd69fb82f3fef825e59c5faab935390d8 \
+    --hash=sha256:65249d8a5345bc95e0f40f280ba63c98eb24de35c6c8f5b662e3e8948adea83f
     # via readme-renderer
 dparse==0.6.4b0 \
     --hash=sha256:592ff183348b8a5ea0a18442a7965e29445d3a26063654ec2c7e8ef42cd5753c \
     --hash=sha256:f8d49b41a527f3d16a269f854e6665245b325e50e41d2c213810cb984553e5c8
     # via
     #   safety
     #   safety-schemas
 editorconfig==0.12.4 \
     --hash=sha256:24857fa1793917dd9ccf0c7810a07e05404ce9b823521c7dce22a4fb5d125f80
     # via
     #   manageprojects
     #   tinkerforge2mqtt (pyproject.toml)
-filelock==3.13.3 \
-    --hash=sha256:5ffa845303983e7a0b7ae17636509bc97997d58afeafa72fb141a17b152284cb \
-    --hash=sha256:a79895a25bbefdf55d1a2a0a80968f7dbb28edcd6d4234a0afb3f37ecde4b546
+filelock==3.13.4 \
+    --hash=sha256:404e5e9253aa60ad457cae1be07c0f0ca90a63931200a47d9b6a6af84fd7b45f \
+    --hash=sha256:d13f466618bfde72bd2c18255e269f72542c6e70e7bac83a0232d6b1cc5c8cf4
     # via
     #   tox
     #   virtualenv
 flake8==7.0.0 \
     --hash=sha256:33f96621059e65eec474169085dc92bf26e7b2d47366b70be2f67ab80dc25132 \
     --hash=sha256:a6dfbb75e03252917f2473ea9653f7cd799c3064e54d4c8140044c5c065f53c3
     # via
@@ -409,85 +411,85 @@
     #   tinkerforge2mqtt (pyproject.toml)
 flake8-bugbear==24.2.6 \
     --hash=sha256:663ef5de80cd32aacd39d362212983bc4636435a6f83700b4ed35acbd0b7d1b8 \
     --hash=sha256:f9cb5f2a9e792dd80ff68e89a14c12eed8620af8b41a49d823b7a33064ac9658
     # via
     #   manageprojects
     #   tinkerforge2mqtt (pyproject.toml)
-flynt==0.77 \
-    --hash=sha256:2863ac8ec19d6ec8d29e760546e6ced644baf6dff3c7cdc77e03abbd29b80f14 \
-    --hash=sha256:2bd1b37043ad88a3f3c3c34a76fc0b64d24e5f03d36ea6b48cb69cc642bff17e
+flynt==1.0.1 \
+    --hash=sha256:65d1c546434827275123222a98408e9561bcd67db832dd58f530ff17b8329ec1 \
+    --hash=sha256:988aac00672a5469726cc0a17cef7d1178c284a9fe8563458db2475d0aaed965
     # via darker
-frozendict==2.4.0 \
-    --hash=sha256:05c5a77957ecba4286c7ab33861a8f4f2badc7ea86fc82b834fb360d3aa4c108 \
-    --hash=sha256:0615ed71570eec3cc96df063930ea6e563211efeeac86e3f3cc8bdfc9c9bfab7 \
-    --hash=sha256:08d9c7c1aa92b94538b3a79c43999f999012e174588435f197794d5e5a80e0f5 \
-    --hash=sha256:09ba8ee37d260adde311b8eb4cd12bf27f64071242f736757ae6a11d331eb860 \
-    --hash=sha256:0b75e5e231621dedaef88334997e79fbd137dd89895543d3862fe0220fc3572c \
-    --hash=sha256:1875e7b70a5724bf964354da8fd542240d2cead0d80053ac96bf4494ce3517fa \
-    --hash=sha256:204f2c5c10fc018d1ba8ccc67758aa83fe769c782547bd26dc250317a7ccba71 \
-    --hash=sha256:23a52bbea30c9e35b89291273944393770fb031e522a172e3aff19b62cc50047 \
-    --hash=sha256:2607e82efdd2c277224a58bda3994d4cd48e49eff7fa31e404cf3066e8dbfeae \
-    --hash=sha256:2804ea4bd2179bb33b99483cc8d69246630cc00632b9affe2914e8666f1cc7e5 \
-    --hash=sha256:2fd4583194baabe100c135883017da76259a315d34e303eddf198541b7e02e44 \
-    --hash=sha256:3909df909516cfd7bcefd9a3003948970a12a50c5648d8bbddafcef171f2117f \
-    --hash=sha256:42a9b33ccf9d417b22146e59803c53d5c39d7d9151d2df8df59c235f6a1a5ed7 \
-    --hash=sha256:475c65202a6f5421df8cacb8a2f29c5087134a0542b0540ae95fbf4db7af2ff9 \
-    --hash=sha256:4925c8e82d2bd23d45996cd0827668a52b9c51103897c98ce409a763d0c00c61 \
-    --hash=sha256:5bb5b62d4e2bce12e91800496d94de41bec8f16e4d8a7b16e8f263676ae2031a \
-    --hash=sha256:809f1cffb602cf06e5186c69c0e3b74bec7a3684593145331f9aa2a65b5ba3b7 \
-    --hash=sha256:8fab616e7c0fea2ac928f107c740bd9ba516fc083adfcd1c391d6bfc9164403d \
-    --hash=sha256:9e530658134e88607ff8c2c8934a07b2bb5e9fffab5045f127746f6542c6c77e \
-    --hash=sha256:9fc4cba1ced988ce9020dfcaae6fe3f5521eebc00c5772b511aaf691b0be91e6 \
-    --hash=sha256:a1d232f092dc686e6ef23d436bde30f82c018f31cef1b89b31caef03814b1617 \
-    --hash=sha256:a3f51bfa64e0c4a6608e3f2878bab1211a6b3b197de6fa57151bbe73f1184457 \
-    --hash=sha256:a60f353496637ca21396289a7d969af1eb4ec4d11a7c37a0e7f25fc1761a0c97 \
-    --hash=sha256:aa86325da6a6071284b4ed3d9d2cd9db068560aebad503b658d6a889a0575683 \
-    --hash=sha256:b017cba5f73869b04c2977139ad08e57a7480de1e384c34193939698119baa1d \
-    --hash=sha256:b666f9c6c8a9e794d2713a944b10a65480ff459579d75b5f686c75031c2c2dfc \
-    --hash=sha256:bd4700c3f0aebdc8f4375c35590135794b1dbf2aca132f4756b584fa9910af2d \
-    --hash=sha256:c26758198e403337933a92b01f417a8240c954f553e1d4b5e0f8e39d9c8e3f0a \
-    --hash=sha256:c8af8a6a39e0050d3f3193cda56c42b43534a9b3995c44241bb9527e3c3fd451 \
-    --hash=sha256:cc754117a7d60ba8e55b3c39abd67f37fbc05dd63cdcb03d1717a382fe0a3421 \
-    --hash=sha256:d8d1d269874c94b1ed2b6667e5e43dcf4541838019b1caa4c48f848ac73634df \
-    --hash=sha256:da4406d95c340e0b1cc43a3858fac729f52689325bcf61a9182eb94aff7451dc \
-    --hash=sha256:df3819a5d48ab3aae1548e62093d0111ad7c3b62ff9392421b7bbf149c08b629 \
-    --hash=sha256:efca7281184b54f7abab6980cf25837b709f72ced62791f62dabcd7b184d958a \
-    --hash=sha256:f91acaff475d0ef0d3436b805c9b91fc627a6a8a281771a24f7ab7f458a0b34f \
-    --hash=sha256:f9d81fb396ea81fcba3b3dde4a4b51adcb74ff31632014fbfd030f8acd5a7292
+frozendict==2.4.1 \
+    --hash=sha256:0187974c3cfc0ac77dc20f9af272f69c8436d2e994dfce85eb7cca269f4d0b7a \
+    --hash=sha256:107a9953272410cd05fcfba4dcf31f01825cd6b3c17f3cf616072e9611480034 \
+    --hash=sha256:1b01ebe8772ab30ab593e72dfe3f06e5d97db508bfd72613c243fd08f5ba96e4 \
+    --hash=sha256:1b32eb2f30bb734b7a699ee7003c86f81964f1c3b6e0e0f18efcbbdeb5b220bf \
+    --hash=sha256:1ed0f607c73e6482e8a8080ea22d9d9f057f0624225e04e7e3e16a94ec215827 \
+    --hash=sha256:2dfeca22e383d64d92301378ca5d10265d7ef05d989501ea5f37520052a0c9fd \
+    --hash=sha256:2f7b202617b410f9b8d528ce82cdb4b16a7e80ccd58601d0d1d8e15231e49292 \
+    --hash=sha256:2fa000d16b1af7315b8d9fbc15e6929303e1c447a9f06c10bfef62b7c9ea266f \
+    --hash=sha256:42077b882ed0e117e1b7f9c7b00453aecddbe268a80f5ca1a73c163c79025dbb \
+    --hash=sha256:42b3906ac43cf2c77f1e69fe7bdd93347044d1a0bc15bf5b733d47c39bfe2e3a \
+    --hash=sha256:4d2d2987b280fae3b46a77cbc3d51394b671c8d8b7270ab2e6d767a42dac15b1 \
+    --hash=sha256:4e8477396a166f5b8cfaaebd623ff05b7bacca830afa8e8d377ad3ed951a8bb2 \
+    --hash=sha256:4fc7b05120500e13a2f319ba4cbfba7f832c04441348ca20dbdcf776b5d2332f \
+    --hash=sha256:53eb5d19ff5b71d3f7806620000e80c1d2478a22c481799ea7b16fb218d42923 \
+    --hash=sha256:5b64b5c6ac3542a4028a431c01d39c60bfb809316cdd8c940d252d084437787f \
+    --hash=sha256:7bd5b958264646ca0c5589a4c82ec4be2bf7ff0d4d1202b9d9599f24be4d51c7 \
+    --hash=sha256:7cc4f1be80760080ca9ee83977c43ad202db91d0ee1e46e9f7c44ebcc05a3b81 \
+    --hash=sha256:7d6b51d2a726ecb169765261bd7e73f63669cf849e882d94d382d8ff682f0292 \
+    --hash=sha256:81ffbac40077c6f56355d47e18adb36e11816ae114ca9d9ee90b842b907d92f5 \
+    --hash=sha256:884a3cbaff8cfd1b36f07a8749b48a6cfebd7fca196e13b9664d33df38b38d27 \
+    --hash=sha256:9030e487d0d433aeaf2d7f741a47d9b890e2572951588f80f29d0161cfd5553a \
+    --hash=sha256:971017c706db1b76abdd7db285592d9f232aff6e8f47dffbd1cd0a020873b164 \
+    --hash=sha256:992cc157b6cdf788c1f24ab9531ba37104aba2d21f1520949a03bf3f9af7935e \
+    --hash=sha256:9f0172c1c3a52714b6530ec56621a6be2962776fa1a4638c4e40576b32e33355 \
+    --hash=sha256:a571fbbe8c0cb0d0d31dce24b1026301013d3884b2fc3099741ba7a9bd5764df \
+    --hash=sha256:accdebc212ef31e0de5b54fbeb275f79c5380e02b250b3d1c4341f6ccf73e876 \
+    --hash=sha256:ace99e4430802bb3d52969870a9432d68919cd33af18f9086ccd6a3a46ac6e7c \
+    --hash=sha256:b06df1995b14fca1e9acc53b1423a4c2dca072517acd619c1576fc6b352428ec \
+    --hash=sha256:c113eb12f0713b53f6d0bbf3bced19dd429e17cac1cf3c350bf05c82c573613d \
+    --hash=sha256:ccf4943a5276a99ff98000890fcbc76fcbc5f43f51250270ddab65da0ee61883 \
+    --hash=sha256:d1b02f873866f5d245a4bc4f9f2647aacb0d5f9a4d47e1de52c46cf03368c8cc \
+    --hash=sha256:d5619bd7f092b1f7ab69163ddcdff674e6786b7a19aea1217a6a46b942430631 \
+    --hash=sha256:d8312598598c9e79653da50c49315fc89d017dbaa4406160958c64d85a707edd \
+    --hash=sha256:de9f7194f4edbacdc609c66f49f583a658ec130e0f68e482fccae35d1befddaf \
+    --hash=sha256:ee12840600814adf4fb1fb84eafb8098bf1701d536949ead096158e3b11cf6f8 \
+    --hash=sha256:eebe6b4c054f987d83477f797f24a149ed409e8dc1c11c1fedc98d721f6ea905
     # via ha-services
-graylint==1.0.0 \
-    --hash=sha256:d79504a51d921b3b92182f096dd05126238f3f48e2d41ebbc8278c8e4b1a7f9c \
-    --hash=sha256:f7e1296cd1595d818259fdfc13b484856889c2bbe81f4ac4724e3bc39b43e973
+graylint==1.0.1 \
+    --hash=sha256:857c84bd430ccf261b0acd80d565b6d16dba6fa5055ddbe6d738eda5a59a59ba \
+    --hash=sha256:ab433865aacd5f072edd5fc2db3938aaf10d869c2e5d266821f2d1fb87574dd6
     # via darker
 ha-services==2.5.0 \
     --hash=sha256:7dce3cb3804f52aa66b5b737661b0f6618a8af24ceb7575574ac03f56d371248 \
     --hash=sha256:fab10eacd2cb910b29b64fe6d8708f255da98d12f53ce08f5293790ab13b5e16
     # via tinkerforge2mqtt (pyproject.toml)
-idna==3.6 \
-    --hash=sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca \
-    --hash=sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f
+idna==3.7 \
+    --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
+    --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
     # via requests
 importlib-metadata==7.1.0 \
     --hash=sha256:30962b96c0c223483ed6cc7280e7f0199feb01a0e40cfae4d4450fc6fab1f570 \
     --hash=sha256:b78938b926ee8d5f020fc4772d487045805a55ddbad2ecf21c6d60938dc7fcd2
     # via
     #   keyring
     #   twine
 isort==5.13.2 \
     --hash=sha256:48fdfcb9face5d58a4f6dde2e72a1fb8dcaf8ab26f95ab49fab84c2ddefb0109 \
     --hash=sha256:8ca5e72a8d85860d5a3fa69b8745237f2939afe12dbf656afbcb47fe72d947a6
     # via darker
-jaraco-classes==3.3.1 \
-    --hash=sha256:86b534de565381f6b3c1c830d13f931d7be1a75f0081c57dff615578676e2206 \
-    --hash=sha256:cb28a5ebda8bc47d8c8015307d93163464f9f2b91ab4006e09ff0ce07e8bfb30
+jaraco-classes==3.4.0 \
+    --hash=sha256:47a024b51d0239c0dd8c8540c6c7f484be3b8fcf0b2d85c13825780d3b3f3acd \
+    --hash=sha256:f662826b6bed8cace05e7ff873ce0f9283b5c924470fe664fff1c2f00f581790
     # via keyring
-jaraco-context==4.3.0 \
-    --hash=sha256:4dad2404540b936a20acedec53355bdaea223acb88fd329fa6de9261c941566e \
-    --hash=sha256:5d9e95ca0faa78943ed66f6bc658dd637430f16125d86988e77844c741ff2f11
+jaraco-context==5.3.0 \
+    --hash=sha256:3e16388f7da43d384a1a7cd3452e72e14732ac9fe459678773a3608a812bf266 \
+    --hash=sha256:c2f67165ce1f9be20f32f650f25d8edfc1646a8aeee48ae06fb35f90763576d2
     # via keyring
 jaraco-functools==4.0.0 \
     --hash=sha256:c279cb24c93d694ef7270f970d499cab4d3813f4e08273f95398651a634f0925 \
     --hash=sha256:daf276ddf234bea897ef14f43c4e1bf9eefeac7b7a82a4dd69228ac20acff68d
     # via keyring
 jeepney==0.8.0 \
     --hash=sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806 \
@@ -497,17 +499,17 @@
     #   secretstorage
 jinja2==3.1.3 \
     --hash=sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa \
     --hash=sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90
     # via
     #   cookiecutter
     #   safety
-keyring==25.0.0 \
-    --hash=sha256:9a15cd280338920388e8c1787cb8792b9755dabb3e7c61af5ac1f8cd437cefde \
-    --hash=sha256:fc024ed53c7ea090e30723e6bd82f58a39dc25d9a6797d866203ecd0ee6306cb
+keyring==25.1.0 \
+    --hash=sha256:26fc12e6a329d61d24aa47b22a7c5c3f35753df7d8f2860973cf94f4e1fb3427 \
+    --hash=sha256:7230ea690525133f6ad536a9b5def74a4bd52642abe594761028fc044d7c7893
     # via twine
 manageprojects==0.17.1 \
     --hash=sha256:355d970261f14b53b574d102e7e82462fe6769baa06c479f00f07a0bcfcb8e4d \
     --hash=sha256:4662ff7f0e64ea9b420b67c270594c88542858a1434ebe8b5f93b7bf2ae2e706
     # via tinkerforge2mqtt (pyproject.toml)
 markdown-it-py==3.0.0 \
     --hash=sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1 \
@@ -746,104 +748,104 @@
     # via ha-services
 pycodestyle==2.11.1 \
     --hash=sha256:41ba0e7afc9752dfb53ced5489e89f8186be00e599e712660695b7a75ff2663f \
     --hash=sha256:44fe31000b2d866f2e41841b18528a505fbd7fef9017b04eff4e2648a0fadc67
     # via
     #   autopep8
     #   flake8
-pycparser==2.21 \
-    --hash=sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9 \
-    --hash=sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206
+pycparser==2.22 \
+    --hash=sha256:491c8be9c040f5390f5bf44a5b07752bd07f56edf992381b05c701439eec10f6 \
+    --hash=sha256:c3702b6d3dd8c7abc1afa565d7e63d53a1d0bd86cdc24edd75470f4de499cfcc
     # via cffi
-pydantic==2.6.4 \
-    --hash=sha256:b1704e0847db01817624a6b86766967f552dd9dbf3afba4004409f908dcc84e6 \
-    --hash=sha256:cc46fce86607580867bdc3361ad462bab9c222ef042d3da86f2fb333e1d916c5
+pydantic==2.7.0 \
+    --hash=sha256:9dee74a271705f14f9a1567671d144a851c675b072736f0a7b2608fd9e495352 \
+    --hash=sha256:b5ecdd42262ca2462e2624793551e80911a1e989f462910bb81aef974b4bb383
     # via
     #   safety
     #   safety-schemas
-pydantic-core==2.16.3 \
-    --hash=sha256:00ee1c97b5364b84cb0bd82e9bbf645d5e2871fb8c58059d158412fee2d33d8a \
-    --hash=sha256:0d32576b1de5a30d9a97f300cc6a3f4694c428d956adbc7e6e2f9cad279e45ed \
-    --hash=sha256:0df446663464884297c793874573549229f9eca73b59360878f382a0fc085979 \
-    --hash=sha256:0f56ae86b60ea987ae8bcd6654a887238fd53d1384f9b222ac457070b7ac4cff \
-    --hash=sha256:13dcc4802961b5f843a9385fc821a0b0135e8c07fc3d9949fd49627c1a5e6ae5 \
-    --hash=sha256:162e498303d2b1c036b957a1278fa0899d02b2842f1ff901b6395104c5554a45 \
-    --hash=sha256:1b662180108c55dfbf1280d865b2d116633d436cfc0bba82323554873967b340 \
-    --hash=sha256:1cac689f80a3abab2d3c0048b29eea5751114054f032a941a32de4c852c59cad \
-    --hash=sha256:21b888c973e4f26b7a96491c0965a8a312e13be108022ee510248fe379a5fa23 \
-    --hash=sha256:287073c66748f624be4cef893ef9174e3eb88fe0b8a78dc22e88eca4bc357ca6 \
-    --hash=sha256:2a1ef6a36fdbf71538142ed604ad19b82f67b05749512e47f247a6ddd06afdc7 \
-    --hash=sha256:2a72fb9963cba4cd5793854fd12f4cfee731e86df140f59ff52a49b3552db241 \
-    --hash=sha256:2acca2be4bb2f2147ada8cac612f8a98fc09f41c89f87add7256ad27332c2fda \
-    --hash=sha256:2f583bd01bbfbff4eaee0868e6fc607efdfcc2b03c1c766b06a707abbc856187 \
-    --hash=sha256:33809aebac276089b78db106ee692bdc9044710e26f24a9a2eaa35a0f9fa70ba \
-    --hash=sha256:36fa178aacbc277bc6b62a2c3da95226520da4f4e9e206fdf076484363895d2c \
-    --hash=sha256:4204e773b4b408062960e65468d5346bdfe139247ee5f1ca2a378983e11388a2 \
-    --hash=sha256:4384a8f68ddb31a0b0c3deae88765f5868a1b9148939c3f4121233314ad5532c \
-    --hash=sha256:456855f57b413f077dff513a5a28ed838dbbb15082ba00f80750377eed23d132 \
-    --hash=sha256:49d5d58abd4b83fb8ce763be7794d09b2f50f10aa65c0f0c1696c677edeb7cbf \
-    --hash=sha256:4ac6b4ce1e7283d715c4b729d8f9dab9627586dafce81d9eaa009dd7f25dd972 \
-    --hash=sha256:4df8a199d9f6afc5ae9a65f8f95ee52cae389a8c6b20163762bde0426275b7db \
-    --hash=sha256:500960cb3a0543a724a81ba859da816e8cf01b0e6aaeedf2c3775d12ee49cade \
-    --hash=sha256:519ae0312616026bf4cedc0fe459e982734f3ca82ee8c7246c19b650b60a5ee4 \
-    --hash=sha256:578114bc803a4c1ff9946d977c221e4376620a46cf78da267d946397dc9514a8 \
-    --hash=sha256:5c5cbc703168d1b7a838668998308018a2718c2130595e8e190220238addc96f \
-    --hash=sha256:6162f8d2dc27ba21027f261e4fa26f8bcb3cf9784b7f9499466a311ac284b5b9 \
-    --hash=sha256:704d35ecc7e9c31d48926150afada60401c55efa3b46cd1ded5a01bdffaf1d48 \
-    --hash=sha256:716b542728d4c742353448765aa7cdaa519a7b82f9564130e2b3f6766018c9ec \
-    --hash=sha256:72282ad4892a9fb2da25defeac8c2e84352c108705c972db82ab121d15f14e6d \
-    --hash=sha256:7233d65d9d651242a68801159763d09e9ec96e8a158dbf118dc090cd77a104c9 \
-    --hash=sha256:732da3243e1b8d3eab8c6ae23ae6a58548849d2e4a4e03a1924c8ddf71a387cb \
-    --hash=sha256:75b81e678d1c1ede0785c7f46690621e4c6e63ccd9192af1f0bd9d504bbb6bf4 \
-    --hash=sha256:75f76ee558751746d6a38f89d60b6228fa174e5172d143886af0f85aa306fd89 \
-    --hash=sha256:7ee8d5f878dccb6d499ba4d30d757111847b6849ae07acdd1205fffa1fc1253c \
-    --hash=sha256:7f752826b5b8361193df55afcdf8ca6a57d0232653494ba473630a83ba50d8c9 \
-    --hash=sha256:86b3d0033580bd6bbe07590152007275bd7af95f98eaa5bd36f3da219dcd93da \
-    --hash=sha256:8d62da299c6ecb04df729e4b5c52dc0d53f4f8430b4492b93aa8de1f541c4aac \
-    --hash=sha256:8e47755d8152c1ab5b55928ab422a76e2e7b22b5ed8e90a7d584268dd49e9c6b \
-    --hash=sha256:9091632a25b8b87b9a605ec0e61f241c456e9248bfdcf7abdf344fdb169c81cf \
-    --hash=sha256:936e5db01dd49476fa8f4383c259b8b1303d5dd5fb34c97de194560698cc2c5e \
-    --hash=sha256:99b6add4c0b39a513d323d3b93bc173dac663c27b99860dd5bf491b240d26137 \
-    --hash=sha256:9c865a7ee6f93783bd5d781af5a4c43dadc37053a5b42f7d18dc019f8c9d2bd1 \
-    --hash=sha256:a425479ee40ff021f8216c9d07a6a3b54b31c8267c6e17aa88b70d7ebd0e5e5b \
-    --hash=sha256:a4b2bf78342c40b3dc830880106f54328928ff03e357935ad26c7128bbd66ce8 \
-    --hash=sha256:a6b1bb0827f56654b4437955555dc3aeeebeddc47c2d7ed575477f082622c49e \
-    --hash=sha256:aaf09e615a0bf98d406657e0008e4a8701b11481840be7d31755dc9f97c44053 \
-    --hash=sha256:b1f6f5938d63c6139860f044e2538baeee6f0b251a1816e7adb6cbce106a1f01 \
-    --hash=sha256:b29eeb887aa931c2fcef5aa515d9d176d25006794610c264ddc114c053bf96fe \
-    --hash=sha256:b3992a322a5617ded0a9f23fd06dbc1e4bd7cf39bc4ccf344b10f80af58beacd \
-    --hash=sha256:b5b6079cc452a7c53dd378c6f881ac528246b3ac9aae0f8eef98498a75657805 \
-    --hash=sha256:b60cc1a081f80a2105a59385b92d82278b15d80ebb3adb200542ae165cd7d183 \
-    --hash=sha256:b926dd38db1519ed3043a4de50214e0d600d404099c3392f098a7f9d75029ff8 \
-    --hash=sha256:bd87f48924f360e5d1c5f770d6155ce0e7d83f7b4e10c2f9ec001c73cf475c99 \
-    --hash=sha256:bda1ee3e08252b8d41fa5537413ffdddd58fa73107171a126d3b9ff001b9b820 \
-    --hash=sha256:be0ec334369316fa73448cc8c982c01e5d2a81c95969d58b8f6e272884df0074 \
-    --hash=sha256:c6119dc90483a5cb50a1306adb8d52c66e447da88ea44f323e0ae1a5fcb14256 \
-    --hash=sha256:c9803edf8e29bd825f43481f19c37f50d2b01899448273b3a7758441b512acf8 \
-    --hash=sha256:c9bd22a2a639e26171068f8ebb5400ce2c1bc7d17959f60a3b753ae13c632975 \
-    --hash=sha256:cbcc558401de90a746d02ef330c528f2e668c83350f045833543cd57ecead1ad \
-    --hash=sha256:cf6204fe865da605285c34cf1172879d0314ff267b1c35ff59de7154f35fdc2e \
-    --hash=sha256:d33dd21f572545649f90c38c227cc8631268ba25c460b5569abebdd0ec5974ca \
-    --hash=sha256:d89ca19cdd0dd5f31606a9329e309d4fcbb3df860960acec32630297d61820df \
-    --hash=sha256:d8f99b147ff3fcf6b3cc60cb0c39ea443884d5559a30b1481e92495f2310ff2b \
-    --hash=sha256:d937653a696465677ed583124b94a4b2d79f5e30b2c46115a68e482c6a591c8a \
-    --hash=sha256:dcca5d2bf65c6fb591fff92da03f94cd4f315972f97c21975398bd4bd046854a \
-    --hash=sha256:ded1c35f15c9dea16ead9bffcde9bb5c7c031bff076355dc58dcb1cb436c4721 \
-    --hash=sha256:e3e70c94a0c3841e6aa831edab1619ad5c511199be94d0c11ba75fe06efe107a \
-    --hash=sha256:e56f8186d6210ac7ece503193ec84104da7ceb98f68ce18c07282fcc2452e76f \
-    --hash=sha256:e7774b570e61cb998490c5235740d475413a1f6de823169b4cf94e2fe9e9f6b2 \
-    --hash=sha256:e7c6ed0dc9d8e65f24f5824291550139fe6f37fac03788d4580da0d33bc00c97 \
-    --hash=sha256:ec08be75bb268473677edb83ba71e7e74b43c008e4a7b1907c6d57e940bf34b6 \
-    --hash=sha256:ecdf6bf5f578615f2e985a5e1f6572e23aa632c4bd1dc67f8f406d445ac115ed \
-    --hash=sha256:ed25e1835c00a332cb10c683cd39da96a719ab1dfc08427d476bce41b92531fc \
-    --hash=sha256:f4cb85f693044e0f71f394ff76c98ddc1bc0953e48c061725e540396d5c8a2e1 \
-    --hash=sha256:f53aace168a2a10582e570b7736cc5bef12cae9cf21775e3eafac597e8551fbe \
-    --hash=sha256:f651dd19363c632f4abe3480a7c87a9773be27cfe1341aef06e8759599454120 \
-    --hash=sha256:fc4ad7f7ee1a13d9cb49d8198cd7d7e3aa93e425f371a68235f784e99741561f \
-    --hash=sha256:fee427241c2d9fb7192b658190f9f5fd6dfe41e02f3c1489d2ec1e6a5ab1e04a
+pydantic-core==2.18.1 \
+    --hash=sha256:030e4f9516f9947f38179249778709a460a3adb516bf39b5eb9066fcfe43d0e6 \
+    --hash=sha256:09f03dfc0ef8c22622eaa8608caa4a1e189cfb83ce847045eca34f690895eccb \
+    --hash=sha256:12a05db5013ec0ca4a32cc6433f53faa2a014ec364031408540ba858c2172bb0 \
+    --hash=sha256:14fe73881cf8e4cbdaded8ca0aa671635b597e42447fec7060d0868b52d074e6 \
+    --hash=sha256:1a0c3e718f4e064efde68092d9d974e39572c14e56726ecfaeebbe6544521f47 \
+    --hash=sha256:1be91ad664fc9245404a789d60cba1e91c26b1454ba136d2a1bf0c2ac0c0505a \
+    --hash=sha256:201713f2f462e5c015b343e86e68bd8a530a4f76609b33d8f0ec65d2b921712a \
+    --hash=sha256:2027493cc44c23b598cfaf200936110433d9caa84e2c6cf487a83999638a96ac \
+    --hash=sha256:250ae39445cb5475e483a36b1061af1bc233de3e9ad0f4f76a71b66231b07f88 \
+    --hash=sha256:2533ad2883f001efa72f3d0e733fb846710c3af6dcdd544fe5bf14fa5fe2d7db \
+    --hash=sha256:25595ac311f20e5324d1941909b0d12933f1fd2171075fcff763e90f43e92a0d \
+    --hash=sha256:2684a94fdfd1b146ff10689c6e4e815f6a01141781c493b97342cdc5b06f4d5d \
+    --hash=sha256:27f1009dc292f3b7ca77feb3571c537276b9aad5dd4efb471ac88a8bd09024e9 \
+    --hash=sha256:2adaeea59849ec0939af5c5d476935f2bab4b7f0335b0110f0f069a41024278e \
+    --hash=sha256:2ae80f72bb7a3e397ab37b53a2b49c62cc5496412e71bc4f1277620a7ce3f52b \
+    --hash=sha256:2d5728e93d28a3c63ee513d9ffbac9c5989de8c76e049dbcb5bfe4b923a9739d \
+    --hash=sha256:2e91711e36e229978d92642bfc3546333a9127ecebb3f2761372e096395fc649 \
+    --hash=sha256:2fe0c1ce5b129455e43f941f7a46f61f3d3861e571f2905d55cdbb8b5c6f5e2c \
+    --hash=sha256:38a5024de321d672a132b1834a66eeb7931959c59964b777e8f32dbe9523f6b1 \
+    --hash=sha256:3e352f0191d99fe617371096845070dee295444979efb8f27ad941227de6ad09 \
+    --hash=sha256:48dd883db92e92519201f2b01cafa881e5f7125666141a49ffba8b9facc072b0 \
+    --hash=sha256:54764c083bbe0264f0f746cefcded6cb08fbbaaf1ad1d78fb8a4c30cff999a90 \
+    --hash=sha256:54c7375c62190a7845091f521add19b0f026bcf6ae674bdb89f296972272e86d \
+    --hash=sha256:561cf62c8a3498406495cfc49eee086ed2bb186d08bcc65812b75fda42c38294 \
+    --hash=sha256:56823a92075780582d1ffd4489a2e61d56fd3ebb4b40b713d63f96dd92d28144 \
+    --hash=sha256:582cf2cead97c9e382a7f4d3b744cf0ef1a6e815e44d3aa81af3ad98762f5a9b \
+    --hash=sha256:58aca931bef83217fca7a390e0486ae327c4af9c3e941adb75f8772f8eeb03a1 \
+    --hash=sha256:5f7973c381283783cd1043a8c8f61ea5ce7a3a58b0369f0ee0ee975eaf2f2a1b \
+    --hash=sha256:6395a4435fa26519fd96fdccb77e9d00ddae9dd6c742309bd0b5610609ad7fb2 \
+    --hash=sha256:63d7523cd95d2fde0d28dc42968ac731b5bb1e516cc56b93a50ab293f4daeaad \
+    --hash=sha256:641a018af4fe48be57a2b3d7a1f0f5dbca07c1d00951d3d7463f0ac9dac66622 \
+    --hash=sha256:667880321e916a8920ef49f5d50e7983792cf59f3b6079f3c9dac2b88a311d17 \
+    --hash=sha256:684d840d2c9ec5de9cb397fcb3f36d5ebb6fa0d94734f9886032dd796c1ead06 \
+    --hash=sha256:68717c38a68e37af87c4da20e08f3e27d7e4212e99e96c3d875fbf3f4812abfc \
+    --hash=sha256:6b7bbb97d82659ac8b37450c60ff2e9f97e4eb0f8a8a3645a5568b9334b08b50 \
+    --hash=sha256:72722ce529a76a4637a60be18bd789d8fb871e84472490ed7ddff62d5fed620d \
+    --hash=sha256:73c1bc8a86a5c9e8721a088df234265317692d0b5cd9e86e975ce3bc3db62a59 \
+    --hash=sha256:76909849d1a6bffa5a07742294f3fa1d357dc917cb1fe7b470afbc3a7579d539 \
+    --hash=sha256:76b86e24039c35280ceee6dce7e62945eb93a5175d43689ba98360ab31eebc4a \
+    --hash=sha256:7a5d83efc109ceddb99abd2c1316298ced2adb4570410defe766851a804fcd5b \
+    --hash=sha256:80e0e57cc704a52fb1b48f16d5b2c8818da087dbee6f98d9bf19546930dc64b5 \
+    --hash=sha256:85233abb44bc18d16e72dc05bf13848a36f363f83757541f1a97db2f8d58cfd9 \
+    --hash=sha256:907a4d7720abfcb1c81619863efd47c8a85d26a257a2dbebdb87c3b847df0278 \
+    --hash=sha256:9376d83d686ec62e8b19c0ac3bf8d28d8a5981d0df290196fb6ef24d8a26f0d6 \
+    --hash=sha256:94b9769ba435b598b547c762184bcfc4783d0d4c7771b04a3b45775c3589ca44 \
+    --hash=sha256:9a29726f91c6cb390b3c2338f0df5cd3e216ad7a938762d11c994bb37552edb0 \
+    --hash=sha256:9b6431559676a1079eac0f52d6d0721fb8e3c5ba43c37bc537c8c83724031feb \
+    --hash=sha256:9ece8a49696669d483d206b4474c367852c44815fca23ac4e48b72b339807f80 \
+    --hash=sha256:a139fe9f298dc097349fb4f28c8b81cc7a202dbfba66af0e14be5cfca4ef7ce5 \
+    --hash=sha256:a32204489259786a923e02990249c65b0f17235073149d0033efcebe80095570 \
+    --hash=sha256:a3982b0a32d0a88b3907e4b0dc36809fda477f0757c59a505d4e9b455f384b8b \
+    --hash=sha256:aad17e462f42ddbef5984d70c40bfc4146c322a2da79715932cd8976317054de \
+    --hash=sha256:b560b72ed4816aee52783c66854d96157fd8175631f01ef58e894cc57c84f0f6 \
+    --hash=sha256:b6b0e4912030c6f28bcb72b9ebe4989d6dc2eebcd2a9cdc35fefc38052dd4fe8 \
+    --hash=sha256:baf1c7b78cddb5af00971ad5294a4583188bda1495b13760d9f03c9483bb6203 \
+    --hash=sha256:c0295d52b012cbe0d3059b1dba99159c3be55e632aae1999ab74ae2bd86a33d7 \
+    --hash=sha256:c562b49c96906b4029b5685075fe1ebd3b5cc2601dfa0b9e16c2c09d6cbce048 \
+    --hash=sha256:c69567ddbac186e8c0aadc1f324a60a564cfe25e43ef2ce81bcc4b8c3abffbae \
+    --hash=sha256:ca71d501629d1fa50ea7fa3b08ba884fe10cefc559f5c6c8dfe9036c16e8ae89 \
+    --hash=sha256:ca976884ce34070799e4dfc6fbd68cb1d181db1eefe4a3a94798ddfb34b8867f \
+    --hash=sha256:d0491006a6ad20507aec2be72e7831a42efc93193d2402018007ff827dc62926 \
+    --hash=sha256:d074b07a10c391fc5bbdcb37b2f16f20fcd9e51e10d01652ab298c0d07908ee2 \
+    --hash=sha256:d2ce426ee691319d4767748c8e0895cfc56593d725594e415f274059bcf3cb76 \
+    --hash=sha256:d4284c621f06a72ce2cb55f74ea3150113d926a6eb78ab38340c08f770eb9b4d \
+    --hash=sha256:d5e6b7155b8197b329dc787356cfd2684c9d6a6b1a197f6bbf45f5555a98d411 \
+    --hash=sha256:d816f44a51ba5175394bc6c7879ca0bd2be560b2c9e9f3411ef3a4cbe644c2e9 \
+    --hash=sha256:dd3f79e17b56741b5177bcc36307750d50ea0698df6aa82f69c7db32d968c1c2 \
+    --hash=sha256:dd63cec4e26e790b70544ae5cc48d11b515b09e05fdd5eff12e3195f54b8a586 \
+    --hash=sha256:de9d3e8717560eb05e28739d1b35e4eac2e458553a52a301e51352a7ffc86a35 \
+    --hash=sha256:df4249b579e75094f7e9bb4bd28231acf55e308bf686b952f43100a5a0be394c \
+    --hash=sha256:e178e5b66a06ec5bf51668ec0d4ac8cfb2bdcb553b2c207d58148340efd00143 \
+    --hash=sha256:e60defc3c15defb70bb38dd605ff7e0fae5f6c9c7cbfe0ad7868582cb7e844a6 \
+    --hash=sha256:ee2794111c188548a4547eccc73a6a8527fe2af6cf25e1a4ebda2fd01cdd2e60 \
+    --hash=sha256:ee7ccc7fb7e921d767f853b47814c3048c7de536663e82fbc37f5eb0d532224b \
+    --hash=sha256:ee9cf33e7fe14243f5ca6977658eb7d1042caaa66847daacbd2117adb258b226 \
+    --hash=sha256:f0f17814c505f07806e22b28856c59ac80cee7dd0fbb152aed273e116378f519 \
+    --hash=sha256:f3202a429fe825b699c57892d4371c74cc3456d8d71b7f35d6028c96dfecad31 \
+    --hash=sha256:f7054fdc556f5421f01e39cbb767d5ec5c1139ea98c3e5b350e02e62201740c7 \
+    --hash=sha256:fd1a9edb9dd9d79fbeac1ea1f9a8dd527a6113b18d2e9bcc0d541d308dae639b
     # via pydantic
 pyflakes==3.2.0 \
     --hash=sha256:1c61603ff154621fb2a9172037d84dca3500def8c8b630657d1701f026f8af3f \
     --hash=sha256:84b5be138a2dfbb40689ca07e2152deb896a65c3a3e24c251c5c62489568074a
     # via
     #   autoflake
     #   flake8
@@ -961,14 +963,15 @@
     #   cookiecutter
     #   ha-services
     #   manageprojects
     #   rich-click
     #   safety
     #   tinkerforge2mqtt (pyproject.toml)
     #   twine
+    #   typer
 rich-click==1.7.4 \
     --hash=sha256:7ce5de8e4dc0333aec946113529b3eeb349f2e5d2fafee96b9edf8ee36a01395 \
     --hash=sha256:e363655475c60fec5a3e16a1eb618118ed79e666c365a36006b107c17c93ac4e
     # via
     #   cli-base-utilities
     #   ha-services
     #   manageprojects
@@ -1039,14 +1042,18 @@
     --hash=sha256:277c077ce6e53221874a87c29515ffdd2f3773a6db4d035a9f67cc98db3b8c7f \
     --hash=sha256:7d1b040ec06480f05cff6b45ea7a93e09c8942df864fb0d01ddeb67c323cfa8c
     # via safety
 secretstorage==3.3.3 \
     --hash=sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77 \
     --hash=sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99
     # via keyring
+shellingham==1.5.4 \
+    --hash=sha256:7ecfff8f2fd72616f7481040475a65b2bf8af90a56c89140852d1120324e8686 \
+    --hash=sha256:8dbca0739d487e5bd35ab3ca4b36e11c4078f3a234bfce294b0a0291363404de
+    # via typer
 six==1.16.0 \
     --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
     # via python-dateutil
 text-unidecode==1.3 \
     --hash=sha256:1311f10e8b895935241623731c2ba64f4c455287888b18189350b67134a822e8 \
     --hash=sha256:bad6603bb14d279193107714b288be206cac565dfa49aa5b105294dd5c4aab93
@@ -1065,15 +1072,14 @@
     #   darker
     #   darkgraylib
 tomli==2.0.1 \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
     # via
     #   cli-base-utilities
-    #   flynt
     #   tinkerforge2mqtt (pyproject.toml)
 tomlkit==0.12.4 \
     --hash=sha256:5cd82d48a3dd89dee1f9d64420aa20ae65cfbd00668d6f094d7578a78efbb77b \
     --hash=sha256:7ca1cfc12232806517a8515047ba66a19369e71edf2439d0f5824f91032b6cc3
     # via
     #   cli-base-utilities
     #   ha-services
@@ -1086,25 +1092,25 @@
     --hash=sha256:89b0cc7d370a4b66421cc6102f269aa910fe0f1861c124f573cf2ddedbc10cf4 \
     --hash=sha256:a262933de0b484c53408f9edae2e7821c1c45a3314ff2df9bdd343aa7ab8edc0
     # via tinkerforge2mqtt (pyproject.toml)
 typeguard==4.2.1 \
     --hash=sha256:7da3bd46e61f03e0852f8d251dcbdc2a336aa495d7daff01e092b55327796eb8 \
     --hash=sha256:c556a1b95948230510070ca53fa0341fb0964611bd05d598d87fb52115d65fee
     # via tinkerforge2mqtt (pyproject.toml)
-typer==0.11.0 \
-    --hash=sha256:049cc47bef39f46b043eddd9165492209fdd9bc7d79afa7ba9cc5cd017caa817 \
-    --hash=sha256:a6ce173c0f03d3a41b49c0a945874cc489e91f88faabf76517b2b91c670fcde7
+typer==0.12.3 \
+    --hash=sha256:070d7ca53f785acbccba8e7d28b08dcd88f79f1fbda035ade0aecec71ca5c914 \
+    --hash=sha256:49e73131481d804288ef62598d97a1ceef3058905aa536a1134f90891ba35482
     # via safety
 types-python-dateutil==2.9.0.20240316 \
     --hash=sha256:5d2f2e240b86905e40944dd787db6da9263f0deabef1076ddaed797351ec0202 \
     --hash=sha256:6b8cb66d960771ce5ff974e9dd45e38facb81718cc1e208b10b1baccbfdbee3b
     # via arrow
-typing-extensions==4.10.0 \
-    --hash=sha256:69b1a937c3a517342112fb4c6df7e72fc39a38e7891a5730ed4985b5214b5475 \
-    --hash=sha256:b0abd7c89e8fb96f98db18d86106ff1d90ab692004eb746cf6eda2682f91b3cb
+typing-extensions==4.11.0 \
+    --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
+    --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
     # via
     #   mypy
     #   pydantic
     #   pydantic-core
     #   rich-click
     #   safety
     #   safety-schemas
@@ -1132,13 +1138,13 @@
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 pip==24.0 \
     --hash=sha256:ba0d021a166865d2265246961bec0152ff124de910c5cc39f1156ce3fa7c69dc \
     --hash=sha256:ea9bd1a847e8c5774a5777bb398c19e80bcd4e2aa16a4b301b718fe6f593aba2
     # via pip-tools
-setuptools==69.2.0 \
-    --hash=sha256:0ff4183f8f42cd8fa3acea16c45205521a4ef28f73c6391d8a25e92893134f2e \
-    --hash=sha256:c21c49fb1042386df081cb5d86759792ab89efca84cf114889191cd09aacc80c
+setuptools==69.3.0 \
+    --hash=sha256:48c518e350470d98cfa2944a31edbfc897c9a7d8fa4847da66d89f0f5fb64b57 \
+    --hash=sha256:e1fd0ca7ba442e4be8a415dcca867b8018777dd5f95f4492bb4dc7d77dbc8bd8
     # via
     #   pip-tools
     #   safety
```

### Comparing `tinkerforge2mqtt-0.7.0/requirements.txt` & `tinkerforge2mqtt-0.8/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -24,51 +24,51 @@
     --hash=sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28 \
     --hash=sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de
     # via
     #   cli-base-utilities
     #   ha-services
     #   rich-click
     #   tinkerforge2mqtt (pyproject.toml)
-frozendict==2.4.0 \
-    --hash=sha256:05c5a77957ecba4286c7ab33861a8f4f2badc7ea86fc82b834fb360d3aa4c108 \
-    --hash=sha256:0615ed71570eec3cc96df063930ea6e563211efeeac86e3f3cc8bdfc9c9bfab7 \
-    --hash=sha256:08d9c7c1aa92b94538b3a79c43999f999012e174588435f197794d5e5a80e0f5 \
-    --hash=sha256:09ba8ee37d260adde311b8eb4cd12bf27f64071242f736757ae6a11d331eb860 \
-    --hash=sha256:0b75e5e231621dedaef88334997e79fbd137dd89895543d3862fe0220fc3572c \
-    --hash=sha256:1875e7b70a5724bf964354da8fd542240d2cead0d80053ac96bf4494ce3517fa \
-    --hash=sha256:204f2c5c10fc018d1ba8ccc67758aa83fe769c782547bd26dc250317a7ccba71 \
-    --hash=sha256:23a52bbea30c9e35b89291273944393770fb031e522a172e3aff19b62cc50047 \
-    --hash=sha256:2607e82efdd2c277224a58bda3994d4cd48e49eff7fa31e404cf3066e8dbfeae \
-    --hash=sha256:2804ea4bd2179bb33b99483cc8d69246630cc00632b9affe2914e8666f1cc7e5 \
-    --hash=sha256:2fd4583194baabe100c135883017da76259a315d34e303eddf198541b7e02e44 \
-    --hash=sha256:3909df909516cfd7bcefd9a3003948970a12a50c5648d8bbddafcef171f2117f \
-    --hash=sha256:42a9b33ccf9d417b22146e59803c53d5c39d7d9151d2df8df59c235f6a1a5ed7 \
-    --hash=sha256:475c65202a6f5421df8cacb8a2f29c5087134a0542b0540ae95fbf4db7af2ff9 \
-    --hash=sha256:4925c8e82d2bd23d45996cd0827668a52b9c51103897c98ce409a763d0c00c61 \
-    --hash=sha256:5bb5b62d4e2bce12e91800496d94de41bec8f16e4d8a7b16e8f263676ae2031a \
-    --hash=sha256:809f1cffb602cf06e5186c69c0e3b74bec7a3684593145331f9aa2a65b5ba3b7 \
-    --hash=sha256:8fab616e7c0fea2ac928f107c740bd9ba516fc083adfcd1c391d6bfc9164403d \
-    --hash=sha256:9e530658134e88607ff8c2c8934a07b2bb5e9fffab5045f127746f6542c6c77e \
-    --hash=sha256:9fc4cba1ced988ce9020dfcaae6fe3f5521eebc00c5772b511aaf691b0be91e6 \
-    --hash=sha256:a1d232f092dc686e6ef23d436bde30f82c018f31cef1b89b31caef03814b1617 \
-    --hash=sha256:a3f51bfa64e0c4a6608e3f2878bab1211a6b3b197de6fa57151bbe73f1184457 \
-    --hash=sha256:a60f353496637ca21396289a7d969af1eb4ec4d11a7c37a0e7f25fc1761a0c97 \
-    --hash=sha256:aa86325da6a6071284b4ed3d9d2cd9db068560aebad503b658d6a889a0575683 \
-    --hash=sha256:b017cba5f73869b04c2977139ad08e57a7480de1e384c34193939698119baa1d \
-    --hash=sha256:b666f9c6c8a9e794d2713a944b10a65480ff459579d75b5f686c75031c2c2dfc \
-    --hash=sha256:bd4700c3f0aebdc8f4375c35590135794b1dbf2aca132f4756b584fa9910af2d \
-    --hash=sha256:c26758198e403337933a92b01f417a8240c954f553e1d4b5e0f8e39d9c8e3f0a \
-    --hash=sha256:c8af8a6a39e0050d3f3193cda56c42b43534a9b3995c44241bb9527e3c3fd451 \
-    --hash=sha256:cc754117a7d60ba8e55b3c39abd67f37fbc05dd63cdcb03d1717a382fe0a3421 \
-    --hash=sha256:d8d1d269874c94b1ed2b6667e5e43dcf4541838019b1caa4c48f848ac73634df \
-    --hash=sha256:da4406d95c340e0b1cc43a3858fac729f52689325bcf61a9182eb94aff7451dc \
-    --hash=sha256:df3819a5d48ab3aae1548e62093d0111ad7c3b62ff9392421b7bbf149c08b629 \
-    --hash=sha256:efca7281184b54f7abab6980cf25837b709f72ced62791f62dabcd7b184d958a \
-    --hash=sha256:f91acaff475d0ef0d3436b805c9b91fc627a6a8a281771a24f7ab7f458a0b34f \
-    --hash=sha256:f9d81fb396ea81fcba3b3dde4a4b51adcb74ff31632014fbfd030f8acd5a7292
+frozendict==2.4.1 \
+    --hash=sha256:0187974c3cfc0ac77dc20f9af272f69c8436d2e994dfce85eb7cca269f4d0b7a \
+    --hash=sha256:107a9953272410cd05fcfba4dcf31f01825cd6b3c17f3cf616072e9611480034 \
+    --hash=sha256:1b01ebe8772ab30ab593e72dfe3f06e5d97db508bfd72613c243fd08f5ba96e4 \
+    --hash=sha256:1b32eb2f30bb734b7a699ee7003c86f81964f1c3b6e0e0f18efcbbdeb5b220bf \
+    --hash=sha256:1ed0f607c73e6482e8a8080ea22d9d9f057f0624225e04e7e3e16a94ec215827 \
+    --hash=sha256:2dfeca22e383d64d92301378ca5d10265d7ef05d989501ea5f37520052a0c9fd \
+    --hash=sha256:2f7b202617b410f9b8d528ce82cdb4b16a7e80ccd58601d0d1d8e15231e49292 \
+    --hash=sha256:2fa000d16b1af7315b8d9fbc15e6929303e1c447a9f06c10bfef62b7c9ea266f \
+    --hash=sha256:42077b882ed0e117e1b7f9c7b00453aecddbe268a80f5ca1a73c163c79025dbb \
+    --hash=sha256:42b3906ac43cf2c77f1e69fe7bdd93347044d1a0bc15bf5b733d47c39bfe2e3a \
+    --hash=sha256:4d2d2987b280fae3b46a77cbc3d51394b671c8d8b7270ab2e6d767a42dac15b1 \
+    --hash=sha256:4e8477396a166f5b8cfaaebd623ff05b7bacca830afa8e8d377ad3ed951a8bb2 \
+    --hash=sha256:4fc7b05120500e13a2f319ba4cbfba7f832c04441348ca20dbdcf776b5d2332f \
+    --hash=sha256:53eb5d19ff5b71d3f7806620000e80c1d2478a22c481799ea7b16fb218d42923 \
+    --hash=sha256:5b64b5c6ac3542a4028a431c01d39c60bfb809316cdd8c940d252d084437787f \
+    --hash=sha256:7bd5b958264646ca0c5589a4c82ec4be2bf7ff0d4d1202b9d9599f24be4d51c7 \
+    --hash=sha256:7cc4f1be80760080ca9ee83977c43ad202db91d0ee1e46e9f7c44ebcc05a3b81 \
+    --hash=sha256:7d6b51d2a726ecb169765261bd7e73f63669cf849e882d94d382d8ff682f0292 \
+    --hash=sha256:81ffbac40077c6f56355d47e18adb36e11816ae114ca9d9ee90b842b907d92f5 \
+    --hash=sha256:884a3cbaff8cfd1b36f07a8749b48a6cfebd7fca196e13b9664d33df38b38d27 \
+    --hash=sha256:9030e487d0d433aeaf2d7f741a47d9b890e2572951588f80f29d0161cfd5553a \
+    --hash=sha256:971017c706db1b76abdd7db285592d9f232aff6e8f47dffbd1cd0a020873b164 \
+    --hash=sha256:992cc157b6cdf788c1f24ab9531ba37104aba2d21f1520949a03bf3f9af7935e \
+    --hash=sha256:9f0172c1c3a52714b6530ec56621a6be2962776fa1a4638c4e40576b32e33355 \
+    --hash=sha256:a571fbbe8c0cb0d0d31dce24b1026301013d3884b2fc3099741ba7a9bd5764df \
+    --hash=sha256:accdebc212ef31e0de5b54fbeb275f79c5380e02b250b3d1c4341f6ccf73e876 \
+    --hash=sha256:ace99e4430802bb3d52969870a9432d68919cd33af18f9086ccd6a3a46ac6e7c \
+    --hash=sha256:b06df1995b14fca1e9acc53b1423a4c2dca072517acd619c1576fc6b352428ec \
+    --hash=sha256:c113eb12f0713b53f6d0bbf3bced19dd429e17cac1cf3c350bf05c82c573613d \
+    --hash=sha256:ccf4943a5276a99ff98000890fcbc76fcbc5f43f51250270ddab65da0ee61883 \
+    --hash=sha256:d1b02f873866f5d245a4bc4f9f2647aacb0d5f9a4d47e1de52c46cf03368c8cc \
+    --hash=sha256:d5619bd7f092b1f7ab69163ddcdff674e6786b7a19aea1217a6a46b942430631 \
+    --hash=sha256:d8312598598c9e79653da50c49315fc89d017dbaa4406160958c64d85a707edd \
+    --hash=sha256:de9f7194f4edbacdc609c66f49f583a658ec130e0f68e482fccae35d1befddaf \
+    --hash=sha256:ee12840600814adf4fb1fb84eafb8098bf1701d536949ead096158e3b11cf6f8 \
+    --hash=sha256:eebe6b4c054f987d83477f797f24a149ed409e8dc1c11c1fedc98d721f6ea905
     # via ha-services
 ha-services==2.5.0 \
     --hash=sha256:7dce3cb3804f52aa66b5b737661b0f6618a8af24ceb7575574ac03f56d371248 \
     --hash=sha256:fab10eacd2cb910b29b64fe6d8708f255da98d12f53ce08f5293790ab13b5e16
     # via tinkerforge2mqtt (pyproject.toml)
 markdown-it-py==3.0.0 \
     --hash=sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1 \
@@ -170,11 +170,11 @@
     # via cli-base-utilities
 tomlkit==0.12.4 \
     --hash=sha256:5cd82d48a3dd89dee1f9d64420aa20ae65cfbd00668d6f094d7578a78efbb77b \
     --hash=sha256:7ca1cfc12232806517a8515047ba66a19369e71edf2439d0f5824f91032b6cc3
     # via
     #   cli-base-utilities
     #   ha-services
-typing-extensions==4.10.0 \
-    --hash=sha256:69b1a937c3a517342112fb4c6df7e72fc39a38e7891a5730ed4985b5214b5475 \
-    --hash=sha256:b0abd7c89e8fb96f98db18d86106ff1d90ab692004eb746cf6eda2682f91b3cb
+typing-extensions==4.11.0 \
+    --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
+    --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
     # via rich-click
```

### Comparing `tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/cli_app/__init__.py` & `tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_app/__init__.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/cli_app/discovering.py` & `tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_app/discovering.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/cli_app/publish.py` & `tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_app/publish.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/cli_app/settings.py` & `tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_app/settings.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/cli_app/systemd.py` & `tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_app/systemd.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/cli_app/update_readme_history.py` & `tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_app/update_readme_history.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/cli_dev/__init__.py` & `tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_dev/__init__.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/cli_dev/code_style.py` & `tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_dev/code_style.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/cli_dev/packaging.py` & `tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_dev/packaging.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/cli_dev/testing.py` & `tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_dev/testing.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_map/__init__.py` & `tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/__init__.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_map/brick_hat_zero.py` & `tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/brick_hat_zero.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_map/bricklet_humidity_v2.py` & `tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/bricklet_humidity_v2.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_map/bricklet_industrial_dual_relay.py` & `tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/bricklet_industrial_dual_relay.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_map/bricklet_motion_detector_v2.py` & `tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/bricklet_motion_detector_v2.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_map/bricklet_solid_state_relay_v2.py` & `tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/bricklet_solid_state_relay_v2.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_map/bricklet_temperature_v2.py` & `tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/bricklet_temperature_v2.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_map/bricklet_voltage_current_v2.py` & `tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/bricklet_voltage_current_v2.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_map_utils/base.py` & `tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map_utils/base.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_map_utils/generics.py` & `tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map_utils/generics.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/device_registry/devices_handler.py` & `tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_registry/devices_handler.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/tests/__init__.py` & `tinkerforge2mqtt-0.8/tinkerforge2mqtt/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/tests/test_project_setup.py` & `tinkerforge2mqtt-0.8/tinkerforge2mqtt/tests/test_project_setup.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/tinkerforge2mqtt/user_settings.py` & `tinkerforge2mqtt-0.8/tinkerforge2mqtt/user_settings.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.7.0/tinkerforge2mqtt.egg-info/PKG-INFO` & `tinkerforge2mqtt-0.8/tinkerforge2mqtt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinkerforge2mqtt
-Version: 0.7.0
+Version: 0.8.0
 Summary: Emit MQTT events from Tinkerforge devices
 Author-email: Jens Diemer <git@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/tinkerforge2mqtt
 Project-URL: Source, https://github.com/jedie/tinkerforge2mqtt
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `tinkerforge2mqtt-0.7.0/tinkerforge2mqtt.egg-info/SOURCES.txt` & `tinkerforge2mqtt-0.8/tinkerforge2mqtt.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 tinkerforge2mqtt/cli_app/update_readme_history.py
 tinkerforge2mqtt/cli_dev/__init__.py
 tinkerforge2mqtt/cli_dev/code_style.py
 tinkerforge2mqtt/cli_dev/packaging.py
 tinkerforge2mqtt/cli_dev/testing.py
 tinkerforge2mqtt/device_map/__init__.py
 tinkerforge2mqtt/device_map/brick_hat_zero.py
+tinkerforge2mqtt/device_map/bricklet_analog_in_v3.py
 tinkerforge2mqtt/device_map/bricklet_humidity_v2.py
 tinkerforge2mqtt/device_map/bricklet_industrial_dual_relay.py
 tinkerforge2mqtt/device_map/bricklet_motion_detector_v2.py
 tinkerforge2mqtt/device_map/bricklet_solid_state_relay_v2.py
 tinkerforge2mqtt/device_map/bricklet_temperature_v2.py
 tinkerforge2mqtt/device_map/bricklet_voltage_current_v2.py
 tinkerforge2mqtt/device_map_utils/__init__.py
```

