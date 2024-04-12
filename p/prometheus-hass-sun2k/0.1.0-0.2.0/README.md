# Comparing `tmp/prometheus_hass_sun2k-0.1.0.tar.gz` & `tmp/prometheus_hass_sun2k-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus_hass_sun2k-0.1.0.tar", max compression
+gzip compressed data, was "prometheus_hass_sun2k-0.2.0.tar", max compression
```

## Comparing `prometheus_hass_sun2k-0.1.0.tar` & `prometheus_hass_sun2k-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1075 2024-04-09 19:38:09.259664 prometheus_hass_sun2k-0.1.0/LICENSE
--rw-r--r--   0        0        0     3454 2024-04-10 20:55:13.660420 prometheus_hass_sun2k-0.1.0/README.md
--rw-r--r--   0        0        0     1162 2024-04-10 20:56:55.054043 prometheus_hass_sun2k-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      125 2024-04-10 20:56:55.058043 prometheus_hass_sun2k-0.1.0/src/prometheus_hass_sun2k/__init__.py
--rw-r--r--   0        0        0     3765 2024-04-10 19:59:14.495095 prometheus_hass_sun2k-0.1.0/src/prometheus_hass_sun2k/cli.py
--rw-r--r--   0        0        0     1219 2024-04-10 19:59:14.495095 prometheus_hass_sun2k-0.1.0/src/prometheus_hass_sun2k/collector.py
--rw-r--r--   0        0        0     1123 2024-04-10 19:59:14.495095 prometheus_hass_sun2k-0.1.0/src/prometheus_hass_sun2k/config.py
--rw-r--r--   0        0        0     1131 2024-04-10 20:50:25.380580 prometheus_hass_sun2k-0.1.0/src/prometheus_hass_sun2k/resources/config-example.yaml
--rw-r--r--   0        0        0      559 2024-04-10 20:50:25.384580 prometheus_hass_sun2k-0.1.0/src/prometheus_hass_sun2k/resources/systemd/prometheus-hass-sun2k.service
--rw-r--r--   0        0        0     4649 1970-01-01 00:00:00.000000 prometheus_hass_sun2k-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-04-09 19:38:09.259664 prometheus_hass_sun2k-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3454 2024-04-10 20:55:13.660420 prometheus_hass_sun2k-0.2.0/README.md
+-rw-r--r--   0        0        0     1162 2024-04-12 12:21:58.066931 prometheus_hass_sun2k-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      125 2024-04-12 12:21:58.066931 prometheus_hass_sun2k-0.2.0/src/prometheus_hass_sun2k/__init__.py
+-rw-r--r--   0        0        0     4064 2024-04-12 11:46:29.311340 prometheus_hass_sun2k-0.2.0/src/prometheus_hass_sun2k/cli.py
+-rw-r--r--   0        0        0     2087 2024-04-12 12:05:32.383516 prometheus_hass_sun2k-0.2.0/src/prometheus_hass_sun2k/collector.py
+-rw-r--r--   0        0        0     1406 2024-04-12 11:48:07.978146 prometheus_hass_sun2k-0.2.0/src/prometheus_hass_sun2k/config.py
+-rw-r--r--   0        0        0     1131 2024-04-10 20:50:25.380580 prometheus_hass_sun2k-0.2.0/src/prometheus_hass_sun2k/resources/config-example.yaml
+-rw-r--r--   0        0        0      559 2024-04-10 20:50:25.384580 prometheus_hass_sun2k-0.2.0/src/prometheus_hass_sun2k/resources/systemd/prometheus-hass-sun2k.service
+-rw-r--r--   0        0        0     4649 1970-01-01 00:00:00.000000 prometheus_hass_sun2k-0.2.0/PKG-INFO
```

### Comparing `prometheus_hass_sun2k-0.1.0/LICENSE` & `prometheus_hass_sun2k-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prometheus_hass_sun2k-0.1.0/README.md` & `prometheus_hass_sun2k-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `prometheus_hass_sun2k-0.1.0/pyproject.toml` & `prometheus_hass_sun2k-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 authors = ["Niko Ehrenfeuchter <mail@he1ix.org>"]
 description = "Prometheus exporter for HomeAssistant data on Huawei SUN2000 inverters"
 license = "MIT"
 name = "prometheus-hass-sun2k"
 readme = "README.md"
-version = "0.1.0"
+version = "0.2.0"
 
 homepage = "https://pypi.org/project/prometheus-hass-sun2k/"
 keywords = ["prometheus", "metrics", "homeassistant", "sun2k", "huawei", "solar", "solar-energy"]
 repository = "https://github.com/ehrenfeu/prometheus-hass-sun2k"
 
 [tool.poetry.urls]
 "Changelog" = "https://github.com/ehrenfeu/prometheus-hass-sun2k/blob/main/CHANGELOG.md"
```

### Comparing `prometheus_hass_sun2k-0.1.0/src/prometheus_hass_sun2k/cli.py` & `prometheus_hass_sun2k-0.2.0/src/prometheus_hass_sun2k/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,14 +32,22 @@
     # re-add a new one with the desired log-level:
     log.remove()
     log.add(sys.stderr, level=level)
     log.info(f"Set logging level to [{level}] ({verbose}).")
 
 
 def prepare_export(config):
+    """Start the exporter's HTTP server and provide basic information.
+
+    Parameters
+    ----------
+    config : Box
+        The service configuration object, see config.load_config_file() for
+        more details.
+    """
     start_http_server(port=config.listen.port, addr=config.listen.addr)
     info = Info(
         name=f"{config.metric_pfx}_collector",
         documentation="SUN2000 inverter series metrics collector (via HomeAssistant)",
     )
     info.info(
         {
@@ -92,30 +100,30 @@
         log.info("Updating metrics...")
 
         log.debug("Processing counters...")
         for name in config.counters:
             value = 0
             try:
                 state = fetch_entity_state(name, config)
-                value = state["state"]
+                value = float(state["state"])
                 log.info(f"{name} -> {value}")
-            except:
+            except Exception:
                 log.error(f"ERROR: fetching [{name}] failed, setting to -> {value}")
             if name not in counters:
                 counters[name] = new_metric(state, Counter, config)
-            counters[name]._value.set(value)
+            counters[name]._value.set(value)  # pylint: disable-msg=protected-access
 
         log.debug("Processing gauges...")
         for name in config.gauges:
             value = 0
             try:
                 state = fetch_entity_state(name, config)
-                value = state["state"]
+                value = float(state["state"])
                 log.info(f"{name} -> {value}")
-            except:
+            except Exception:
                 log.error(f"ERROR: fetching [{name}] failed, setting to -> {value}")
             if name not in gauges:
                 gauges[name] = new_metric(state, Gauge, config)
             gauges[name].set(value)
 
         log.success(f"Updated metrics, sleeping for {config.scrape_interval}s.")
         sleep(config.scrape_interval)
```

### Comparing `prometheus_hass_sun2k-0.1.0/src/prometheus_hass_sun2k/resources/config-example.yaml` & `prometheus_hass_sun2k-0.2.0/src/prometheus_hass_sun2k/resources/config-example.yaml`

 * *Files identical despite different names*

### Comparing `prometheus_hass_sun2k-0.1.0/src/prometheus_hass_sun2k/resources/systemd/prometheus-hass-sun2k.service` & `prometheus_hass_sun2k-0.2.0/src/prometheus_hass_sun2k/resources/systemd/prometheus-hass-sun2k.service`

 * *Files identical despite different names*

### Comparing `prometheus_hass_sun2k-0.1.0/PKG-INFO` & `prometheus_hass_sun2k-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-hass-sun2k
-Version: 0.1.0
+Version: 0.2.0
 Summary: Prometheus exporter for HomeAssistant data on Huawei SUN2000 inverters
 Home-page: https://pypi.org/project/prometheus-hass-sun2k/
 License: MIT
 Keywords: prometheus,metrics,homeassistant,sun2k,huawei,solar,solar-energy
 Author: Niko Ehrenfeuchter
 Author-email: mail@he1ix.org
 Requires-Python: >=3.8,<4.0
```

