# Comparing `tmp/vedro-replay-1.0.0.tar.gz` & `tmp/vedro-replay-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vedro-replay-1.0.0.tar", last modified: Fri Nov  3 13:11:14 2023, max compression
+gzip compressed data, was "vedro-replay-1.1.0.tar", last modified: Fri Apr 12 07:37:06 2024, max compression
```

## Comparing `vedro-replay-1.0.0.tar` & `vedro-replay-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 13:11:14.244307 vedro-replay-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2023-11-03 13:11:03.000000 vedro-replay-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-03 13:11:03.000000 vedro-replay-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7917 2023-11-03 13:11:14.244307 vedro-replay-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7078 2023-11-03 13:11:03.000000 vedro-replay-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      286 2023-11-03 13:11:14.244307 vedro-replay-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2023-11-03 13:11:03.000000 vedro-replay-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 13:11:14.240306 vedro-replay-1.0.0/vedro_replay/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2023-11-03 13:11:03.000000 vedro-replay-1.0.0/vedro_replay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2023-11-03 13:11:03.000000 vedro-replay-1.0.0/vedro_replay/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2023-11-03 13:11:03.000000 vedro-replay-1.0.0/vedro_replay/exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2023-11-03 13:11:03.000000 vedro-replay-1.0.0/vedro_replay/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     7483 2023-11-03 13:11:03.000000 vedro-replay-1.0.0/vedro_replay/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2023-11-03 13:11:03.000000 vedro-replay-1.0.0/vedro_replay/parse_excludes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2023-11-03 13:11:03.000000 vedro-replay-1.0.0/vedro_replay/parse_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2023-11-03 13:11:03.000000 vedro-replay-1.0.0/vedro_replay/replay.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-11-03 13:11:03.000000 vedro-replay-1.0.0/vedro_replay/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2023-11-03 13:11:03.000000 vedro-replay-1.0.0/vedro_replay/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 13:11:14.240306 vedro-replay-1.0.0/vedro_replay/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-11-03 13:11:03.000000 vedro-replay-1.0.0/vedro_replay/templates/config.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      614 2023-11-03 13:11:03.000000 vedro-replay-1.0.0/vedro_replay/templates/contexts.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      245 2023-11-03 13:11:03.000000 vedro-replay-1.0.0/vedro_replay/templates/helper_method.j2
--rw-r--r--   0 runner    (1001) docker     (127)      172 2023-11-03 13:11:03.000000 vedro-replay-1.0.0/vedro_replay/templates/helpers.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      448 2023-11-03 13:11:03.000000 vedro-replay-1.0.0/vedro_replay/templates/interfaces.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2023-11-03 13:11:03.000000 vedro-replay-1.0.0/vedro_replay/templates/scenario.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-11-03 13:11:03.000000 vedro-replay-1.0.0/vedro_replay/templates/vedro.cfg.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 13:11:14.240306 vedro-replay-1.0.0/vedro_replay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7917 2023-11-03 13:11:14.000000 vedro-replay-1.0.0/vedro_replay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      793 2023-11-03 13:11:14.000000 vedro-replay-1.0.0/vedro_replay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 13:11:14.000000 vedro-replay-1.0.0/vedro_replay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-11-03 13:11:14.000000 vedro-replay-1.0.0/vedro_replay.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-11-03 13:11:14.000000 vedro-replay-1.0.0/vedro_replay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-03 13:11:14.000000 vedro-replay-1.0.0/vedro_replay.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:37:06.076913 vedro-replay-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-12 07:36:58.000000 vedro-replay-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-12 07:36:58.000000 vedro-replay-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-04-12 07:37:06.076913 vedro-replay-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-12 07:36:58.000000 vedro-replay-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-12 07:37:06.080913 vedro-replay-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-12 07:36:58.000000 vedro-replay-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:37:06.076913 vedro-replay-1.1.0/vedro_replay/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-12 07:36:58.000000 vedro-replay-1.1.0/vedro_replay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-12 07:36:58.000000 vedro-replay-1.1.0/vedro_replay/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-12 07:36:58.000000 vedro-replay-1.1.0/vedro_replay/exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-12 07:36:58.000000 vedro-replay-1.1.0/vedro_replay/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-04-12 07:36:58.000000 vedro-replay-1.1.0/vedro_replay/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-12 07:36:58.000000 vedro-replay-1.1.0/vedro_replay/parse_excludes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-12 07:36:58.000000 vedro-replay-1.1.0/vedro_replay/parse_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-12 07:36:58.000000 vedro-replay-1.1.0/vedro_replay/replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-12 07:36:58.000000 vedro-replay-1.1.0/vedro_replay/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-12 07:36:58.000000 vedro-replay-1.1.0/vedro_replay/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:37:06.076913 vedro-replay-1.1.0/vedro_replay/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-12 07:36:58.000000 vedro-replay-1.1.0/vedro_replay/templates/config.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-12 07:36:58.000000 vedro-replay-1.1.0/vedro_replay/templates/contexts.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-12 07:36:58.000000 vedro-replay-1.1.0/vedro_replay/templates/helper_method.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-12 07:36:58.000000 vedro-replay-1.1.0/vedro_replay/templates/helpers.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-12 07:36:58.000000 vedro-replay-1.1.0/vedro_replay/templates/interfaces.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-12 07:36:58.000000 vedro-replay-1.1.0/vedro_replay/templates/scenario.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-12 07:36:58.000000 vedro-replay-1.1.0/vedro_replay/templates/vedro.cfg.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:37:06.076913 vedro-replay-1.1.0/vedro_replay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-04-12 07:37:06.000000 vedro-replay-1.1.0/vedro_replay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-12 07:37:06.000000 vedro-replay-1.1.0/vedro_replay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 07:37:06.000000 vedro-replay-1.1.0/vedro_replay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-12 07:37:06.000000 vedro-replay-1.1.0/vedro_replay.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-12 07:37:06.000000 vedro-replay-1.1.0/vedro_replay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 07:37:06.000000 vedro-replay-1.1.0/vedro_replay.egg-info/top_level.txt
```

### Comparing `vedro-replay-1.0.0/LICENSE` & `vedro-replay-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vedro-replay-1.0.0/PKG-INFO` & `vedro-replay-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vedro-replay
-Version: 1.0.0
+Version: 1.1.0
 Summary: vedro-replay package
 Home-page: https://github.com/kvs8/vedro-replay
 Author: Konstantin Shefer
 Author-email: kostya.shefer.999@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `vedro-replay-1.0.0/README.md` & `vedro-replay-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `vedro-replay-1.0.0/setup.py` & `vedro-replay-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def find_required():
     with open("requirements.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="vedro-replay",
-    version="1.0.0",
+    version="1.1.0",
     description="vedro-replay package",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Konstantin Shefer",
     author_email="kostya.shefer.999@gmail.com",
     python_requires=">=3.8",
     url="https://github.com/kvs8/vedro-replay",
```

### Comparing `vedro-replay-1.0.0/vedro_replay/command.py` & `vedro-replay-1.1.0/vedro_replay/command.py`

 * *Files identical despite different names*

### Comparing `vedro-replay-1.0.0/vedro_replay/exclude.py` & `vedro-replay-1.1.0/vedro_replay/exclude.py`

 * *Files identical despite different names*

### Comparing `vedro-replay-1.0.0/vedro_replay/filtering.py` & `vedro-replay-1.1.0/vedro_replay/filtering.py`

 * *Files identical despite different names*

### Comparing `vedro-replay-1.0.0/vedro_replay/generator.py` & `vedro-replay-1.1.0/vedro_replay/generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import logging
 import os
 from abc import ABC, abstractmethod
-from pathlib import Path, PurePosixPath
+from pathlib import Path
 from types import FunctionType
 from typing import Any, List
 
 from jinja2 import Environment, FileSystemLoader, Template
 
-from .parse_requests import parse_requests
-
 
 class GeneratorException(Exception):
     pass
 
 
 class DirectoryWithRequestsNotFound(GeneratorException):
     pass
@@ -30,35 +28,35 @@
     def _generate_by_template(self, file_path: str, template_name: str, **kwargs: Any) -> None:
         if not os.path.exists(file_path) or self.force:
             self.log.info(f'Generate: "{file_path}"')
             template = self._get_template(template_name=template_name)
             with open(file_path, 'w') as file:
                 file.write(template.render(**kwargs))
 
-    def _create_package(self, dir_name: str) -> None:
-        self._create_dir(dir_name=dir_name)
-        init_file_path = f'{dir_name}/__init__.py'
+    def _create_package(self, dirname: str) -> None:
+        self._create_dir(dirname)
+        init_file_path = os.path.join(dirname, '__init__.py')
         if not os.path.exists(init_file_path):
             self.log.info(f'Create: "{init_file_path}"')
             Path(init_file_path).touch()
 
-    def _create_dir(self, dir_name: str) -> None:
-        if not os.path.exists(dir_name):
-            self.log.info(f'Create directory: "{dir_name}"')
-            os.mkdir(dir_name)
+    def _create_dir(self, dirname: str) -> None:
+        if dirname and not os.path.exists(dirname):
+            self.log.info(f'Create directory: "{dirname}"')
+            os.makedirs(dirname)
 
     @classmethod
     def generation_options(cls) -> List[str]:
         return [
             key for key, value in cls.__dict__.items() if isinstance(value, FunctionType) and not key.startswith('_')
         ]
 
 
 class MainGenerator(Generator):
-    __PATH_TEMPLATES = os.path.dirname(os.path.realpath(__file__)) + '/templates'
+    __PATH_TEMPLATES = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'templates')
     __TEMPLATE_INTERFACES = 'interfaces.py.j2'
     __TEMPLATE_SCENARIO = 'scenario.py.j2'
     __TEMPLATE_CONTEXTS = 'contexts.py.j2'
     __TEMPLATE_HELPERS = 'helpers.py.j2'
     __TEMPLATE_HELPER_METHOD = 'helper_method.j2'
     __TEMPLATE_VEDRO_CFG = 'vedro.cfg.py.j2'
     __TEMPLATE_CONFIG = 'config.py.j2'
@@ -96,100 +94,95 @@
     def config(self) -> None:
         self._generate_by_template(
             file_path=self.__FILE_CONFIG,
             template_name=self.__TEMPLATE_CONFIG
         )
 
     def interfaces(self) -> None:
-        self._create_package(dir_name=self.__DIRECTORY_INTERFACES)
+        self._create_package(dirname=self.__DIRECTORY_INTERFACES)
         self._generate_by_template(
-            file_path=f'{self.__DIRECTORY_INTERFACES}/{self.__FILE_INTERFACES}',
+            file_path=os.path.join(self.__DIRECTORY_INTERFACES, self.__FILE_INTERFACES),
             template_name=self.__TEMPLATE_INTERFACES
         )
 
     def contexts(self) -> None:
-        self._create_package(dir_name=self.__DIRECTORY_CONTEXTS)
+        self._create_package(dirname=self.__DIRECTORY_CONTEXTS)
         self._generate_by_template(
-            file_path=f'{self.__DIRECTORY_CONTEXTS}/{self.__FILE_CONTEXTS}',
+            file_path=os.path.join(self.__DIRECTORY_CONTEXTS, self.__FILE_CONTEXTS),
             template_name=self.__TEMPLATE_CONTEXTS
         )
 
     def helpers(self) -> None:
-        self._create_package(dir_name=self.__DIRECTORY_HELPERS)
+        self._create_package(dirname=self.__DIRECTORY_HELPERS)
         self._generate_by_template(
-            file_path=f'{self.__DIRECTORY_HELPERS}/{self.__FILE_HELPERS}',
+            file_path=os.path.join(self.__DIRECTORY_HELPERS, self.__FILE_HELPERS),
             template_name=self.__TEMPLATE_HELPERS
         )
         self.helpers_methods()
 
     def helpers_methods(self) -> None:
-        file_path = f'{self.__DIRECTORY_HELPERS}/{self.__FILE_HELPERS}'
+        file_path = os.path.join(self.__DIRECTORY_HELPERS, self.__FILE_HELPERS)
 
         with open(file_path, 'r') as file:
             content_helpers = file.read()
 
         with open(file_path, 'a') as f:
-            for route in self._get_unique_routes():
-                helper_method_name = self._get_helper_method_name(route)
+            for file_with_requests in self._get_file_paths_with_requests():
+                helper_method_name = self._get_helper_method_name(file_with_requests)
                 if helper_method_name not in content_helpers:
-                    self.log.info(f'Generate helper: "{helper_method_name}" for route {route}')
+                    self.log.info(f'Generate helper: "{helper_method_name}" for file {file_with_requests}')
                     template = self._get_template(self.__TEMPLATE_HELPER_METHOD)
                     f.write(template.render(helper_method_name=helper_method_name))
 
     def scenarios(self) -> None:
         self._create_dir(self.__DIRECTORY_SCENARIOS)
-        for file_requests in self._get_file_with_requests():
-            self._scenario(file_requests=file_requests, route=self._get_route(file_requests))
+        for file_path_with_requests in self._get_file_paths_with_requests():
+            self._scenario(file_path_with_requests)
 
-    def _scenario(self, file_requests: str, route: str) -> None:
-        file_path = f'{self.__DIRECTORY_SCENARIOS}/{self._get_scenario_name(file_requests=file_requests)}.py'
-        self._generate_by_template(
-            file_path=file_path,
+    def _scenario(self, file_path_with_requests: str) -> None:
+        dirname = os.path.dirname(file_path_with_requests.replace(f'{self.__requests_dir}/', '', 1))
+        self._create_dir(os.path.join(self.__DIRECTORY_SCENARIOS, dirname))
+        self._generate_by_template(
+            file_path=os.path.join(
+                self.__DIRECTORY_SCENARIOS, dirname, f'{self._get_scenario_name(file_path_with_requests)}.py'
+            ),
             template_name=self.__TEMPLATE_SCENARIO,
-            requests_dir=self.__requests_dir,
-            api_route=route,
-            file_requests=file_requests,
-            helper_method_name=self._get_helper_method_name(route)
+            file_path_with_requests=file_path_with_requests,
+            helper_method_name=self._get_helper_method_name(file_path_with_requests)
         )
 
-    @staticmethod
-    def _get_helper_method_name(api_route: str) -> str:
-        return 'prepare' + api_route.replace('/', '_').replace('.', '').replace('-', '_')
+    @classmethod
+    def _get_helper_method_name(cls, file_path_with_requests: str) -> str:
+        return 'prepare_' + cls._get_scenario_name(file_path_with_requests)
 
     @staticmethod
-    def _get_scenario_name(file_requests: str) -> str:
-        return file_requests.split('.')[0]
+    def _get_scenario_name(file_path_with_requests: str) -> str:
+        return os.path.basename(file_path_with_requests).split('.')[0].replace('-', '_')
 
-    def _get_file_with_requests(self) -> List[str]:
+    def _get_file_paths_with_requests(self) -> List[str]:
         if not os.path.exists(self.__requests_dir):
             raise DirectoryWithRequestsNotFound(f"The directory with requests: {self.__requests_dir} was not found")
-        return [
-            file for file in os.listdir(self.__requests_dir)
-            if os.path.isfile(os.path.join(self.__requests_dir, file))
-            and PurePosixPath(file).suffix in ['.txt', '.http']
-        ]
 
-    def _get_route(self, file_path: str) -> str:
-        requests = parse_requests(f'{self.__requests_dir}/{file_path}')
-        return requests[0].path
-
-    def _get_unique_routes(self) -> List[str]:
-        routes = [self._get_route(file_requests) for file_requests in self._get_file_with_requests()]
-        return sorted(set(routes))
+        file_with_requests = []
+        for root, _, files in os.walk(self.__requests_dir):
+            for file in files:
+                if file.endswith('.txt') or file.endswith('.http'):
+                    file_with_requests.append(os.path.join(root, file))
+        return file_with_requests
 
     def _get_template(self, template_name: str) -> Template:
         return self.__templates.get_template(name=template_name)
 
 
 def generate(args: Any) -> None:
     logging.basicConfig(level=logging.INFO, format='%(message)s')
     log = logging.getLogger("Generator")
 
     try:
         getattr(MainGenerator(requests_dir=args.requests_dir, force=args.force, log=log), args.option)()
         log.info("The necessary files have been generated!\n"
                  "To run the tests, you need to specify two api url to which request will be sent."
                  "You need to set environment variables in any convenient way, for example:\n"
-                 "export GOLDEN_API_URL=https://golden.app && export TESTING_API_URL=https://test.app && vedro run")
+                 "GOLDEN_API_URL=https://golden.app TESTING_API_URL=https://test.app vedro run -v")
     except DirectoryWithRequestsNotFound as e:
         log.critical(f"{e}. By default, the 'requests' directory was expected. "
                      "Use --requests-dir to specify another")
```

### Comparing `vedro-replay-1.0.0/vedro_replay/parse_excludes.py` & `vedro-replay-1.1.0/vedro_replay/parse_excludes.py`

 * *Files identical despite different names*

### Comparing `vedro-replay-1.0.0/vedro_replay/parse_requests.py` & `vedro-replay-1.1.0/vedro_replay/parse_requests.py`

 * *Files identical despite different names*

### Comparing `vedro-replay-1.0.0/vedro_replay/request.py` & `vedro-replay-1.1.0/vedro_replay/request.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,17 +8,25 @@
             self, method: str, url: str,
             comment: str = "", headers: Optional[Dict[Any, Any]] = None, json_body: Optional[Dict[Any, Any]] = None
     ) -> None:
         self.comment = comment
         self.method = method
         self.url = url
         self.path = urlparse(url).path
-        self.headers = headers
+        self.headers = headers or {}
         self.json_body = json_body
 
+    def add_header(self, key: str, value: str) -> "Request":
+        self.headers[key] = value
+        return self
+
+    def add_json_body(self, json_body: Dict[Any, Any]) -> "Request":
+        self.json_body = json_body
+        return self
+
     def __repr__(self) -> str:
         return self.__str__()
 
     def __str__(self) -> str:
         result = f"{self.method} {self.url}\n"
 
         if self.headers:
```

### Comparing `vedro-replay-1.0.0/vedro_replay/response.py` & `vedro-replay-1.1.0/vedro_replay/response.py`

 * *Files identical despite different names*

### Comparing `vedro-replay-1.0.0/vedro_replay/templates/contexts.py.j2` & `vedro-replay-1.1.0/vedro_replay/templates/contexts.py.j2`

 * *Files identical despite different names*

### Comparing `vedro-replay-1.0.0/vedro_replay/templates/scenario.py.j2` & `vedro-replay-1.1.0/vedro_replay/templates/scenario.py.j2`

 * *Files 14% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 from d42 import from_native
 from helpers.helpers import {{helper_method_name}}
 
 from vedro_replay import Request, replay
 
 
 class Scenario(vedro.Scenario):
-    subject = "do request: {{api_route}} (comment='{comment}')"
+    subject = "do request: {request.method} {request.path} (comment='{request.comment}')"
 
-    @replay("{{requests_dir}}/{{file_requests}}")
-    def __init__(self, comment: str, request: Request):
-        self.comment = comment
+    @replay("{{file_path_with_requests}}")
+    def __init__(self, request: Request):
         self.request = request
 
     async def given_golden_response(self):
         self.golden_response = await golden_response(self.request, {{helper_method_name}})
 
     async def when_user_sends_request(self):
         self.testing_response = await testing_response(self.request, {{helper_method_name}})
```

### Comparing `vedro-replay-1.0.0/vedro_replay.egg-info/PKG-INFO` & `vedro-replay-1.1.0/vedro_replay.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vedro-replay
-Version: 1.0.0
+Version: 1.1.0
 Summary: vedro-replay package
 Home-page: https://github.com/kvs8/vedro-replay
 Author: Konstantin Shefer
 Author-email: kostya.shefer.999@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `vedro-replay-1.0.0/vedro_replay.egg-info/SOURCES.txt` & `vedro-replay-1.1.0/vedro_replay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

