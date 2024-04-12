# Comparing `tmp/docker_inspector-0.1.8.tar.gz` & `tmp/docker_inspector-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_inspector-0.1.8.tar", max compression
+gzip compressed data, was "docker_inspector-0.1.9.tar", max compression
```

## Comparing `docker_inspector-0.1.8.tar` & `docker_inspector-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      851 2024-04-09 14:01:09.175177 docker_inspector-0.1.8/README.md
--rw-r--r--   0        0        0        0 2024-04-09 13:35:47.921879 docker_inspector-0.1.8/docker_inspector/__init__.py
--rw-r--r--   0        0        0     1249 2024-04-09 13:50:09.480154 docker_inspector-0.1.8/docker_inspector/app.py
--rw-r--r--   0        0        0      141 2024-04-09 13:35:47.922154 docker_inspector-0.1.8/docker_inspector/styles/main.css
--rw-r--r--   0        0        0        0 2024-04-09 13:35:47.922216 docker_inspector-0.1.8/docker_inspector/widgets/__init__.py
--rw-r--r--   0        0        0     6897 2024-04-09 13:59:49.117536 docker_inspector-0.1.8/docker_inspector/widgets/container_list.py
--rw-r--r--   0        0        0      472 2024-04-09 14:12:04.033553 docker_inspector-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1287 1970-01-01 00:00:00.000000 docker_inspector-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      851 2024-04-09 14:01:09.175177 docker_inspector-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 13:35:47.921879 docker_inspector-0.1.9/docker_inspector/__init__.py
+-rw-r--r--   0        0        0     1249 2024-04-09 13:50:09.480154 docker_inspector-0.1.9/docker_inspector/app.py
+-rw-r--r--   0        0        0      141 2024-04-09 13:35:47.922154 docker_inspector-0.1.9/docker_inspector/styles/main.css
+-rw-r--r--   0        0        0        0 2024-04-09 13:35:47.922216 docker_inspector-0.1.9/docker_inspector/widgets/__init__.py
+-rw-r--r--   0        0        0     6913 2024-04-09 16:59:34.491714 docker_inspector-0.1.9/docker_inspector/widgets/container_list.py
+-rw-r--r--   0        0        0      607 2024-04-12 06:45:00.162634 docker_inspector-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1287 1970-01-01 00:00:00.000000 docker_inspector-0.1.9/PKG-INFO
```

### Comparing `docker_inspector-0.1.8/README.md` & `docker_inspector-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `docker_inspector-0.1.8/docker_inspector/app.py` & `docker_inspector-0.1.9/docker_inspector/app.py`

 * *Files identical despite different names*

### Comparing `docker_inspector-0.1.8/docker_inspector/widgets/container_list.py` & `docker_inspector-0.1.9/docker_inspector/widgets/container_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
                     out_ip = outer[0]['HostIp']
                     out_port = outer[0]['HostPort']
                     if out_ip in ['0.0.0.0', '']:
                         open_ports.append(Text(f"*:{out_port}->{inner}", style="red bold"))
                     elif out_ip in ['127.0.0.1', 'localhost']:
                         open_ports.append(Text(f"l:{out_port}->{inner}", style="green"))
                     else:
-                        open_ports.append(Text(f"{out_ip}:{out_port}->{inner}"))
+                        open_ports.append(Text(f"{out_ip}:{out_port}->{inner}", style="orange"))
             container_info['open_ports'] = Text(", ").join(open_ports)
 
             # networks
             networks = ', '.join(result_js['NetworkSettings']['Networks'].keys())
             container_info['networks'] = networks
 
             # log size
```

### Comparing `docker_inspector-0.1.8/PKG-INFO` & `docker_inspector-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-inspector
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: antonio
 Author-email: mr.antonsilin@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

