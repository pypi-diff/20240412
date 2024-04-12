# Comparing `tmp/pantarei-0.1.0.tar.gz` & `tmp/pantarei-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pantarei-0.1.0.tar", last modified: Tue Nov  7 16:14:53 2023, max compression
+gzip compressed data, was "pantarei-0.2.tar", last modified: Fri Apr 12 20:20:17 2024, max compression
```

## Comparing `pantarei-0.1.0.tar` & `pantarei-0.2.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-11-07 16:14:53.462272 pantarei-0.1.0/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    35147 2023-03-25 17:07:32.000000 pantarei-0.1.0/LICENSE
--rw-r--r--   0 coslo     (1000) coslo     (1000)     2330 2023-11-07 16:14:53.462272 pantarei-0.1.0/PKG-INFO
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1798 2023-11-07 15:59:40.000000 pantarei-0.1.0/README.md
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-11-07 16:14:53.462272 pantarei-0.1.0/pantarei/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      140 2023-11-04 06:56:07.000000 pantarei-0.1.0/pantarei/__init__.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     5371 2023-10-30 17:01:57.000000 pantarei-0.1.0/pantarei/_attempt.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1405 2023-11-07 12:31:36.000000 pantarei-0.1.0/pantarei/cache.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2996 2023-11-04 06:56:07.000000 pantarei-0.1.0/pantarei/cluster.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2418 2023-11-07 14:00:32.000000 pantarei-0.1.0/pantarei/helpers.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     3692 2023-11-07 15:48:03.000000 pantarei-0.1.0/pantarei/job.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2176 2023-11-07 15:48:03.000000 pantarei-0.1.0/pantarei/scheduler.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1958 2023-11-07 15:09:05.000000 pantarei-0.1.0/pantarei/task.py
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-11-07 16:14:53.462272 pantarei-0.1.0/pantarei.egg-info/
--rw-r--r--   0 coslo     (1000) coslo     (1000)     2330 2023-11-07 16:14:53.000000 pantarei-0.1.0/pantarei.egg-info/PKG-INFO
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      370 2023-11-07 16:14:53.000000 pantarei-0.1.0/pantarei.egg-info/SOURCES.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)        1 2023-11-07 16:14:53.000000 pantarei-0.1.0/pantarei.egg-info/dependency_links.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)        5 2023-11-07 16:14:53.000000 pantarei-0.1.0/pantarei.egg-info/requires.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)        9 2023-11-07 16:14:53.000000 pantarei-0.1.0/pantarei.egg-info/top_level.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      603 2023-11-07 16:14:45.000000 pantarei-0.1.0/pyproject.toml
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      173 2023-11-07 16:14:53.466272 pantarei-0.1.0/setup.cfg
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-11-07 16:14:53.462272 pantarei-0.1.0/tests/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1804 2023-11-07 15:48:03.000000 pantarei-0.1.0/tests/test.py
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-12 20:20:17.365712 pantarei-0.2/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    35147 2023-03-25 17:07:32.000000 pantarei-0.2/LICENSE
+-rw-r--r--   0 coslo     (1000) coslo     (1000)     3694 2024-04-12 20:20:17.365712 pantarei-0.2/PKG-INFO
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3102 2024-04-09 18:30:04.000000 pantarei-0.2/README.md
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-12 20:20:17.361712 pantarei-0.2/pantarei/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      246 2024-04-11 21:27:17.000000 pantarei-0.2/pantarei/__init__.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     5417 2024-04-10 21:22:43.000000 pantarei-0.2/pantarei/_attempt.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2208 2024-04-11 20:42:29.000000 pantarei-0.2/pantarei/backends.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2427 2024-04-11 21:27:17.000000 pantarei-0.2/pantarei/cache.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     8326 2024-04-11 21:27:17.000000 pantarei-0.2/pantarei/core.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    19978 2024-04-11 21:27:17.000000 pantarei-0.2/pantarei/database.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     8329 2024-04-11 21:27:17.000000 pantarei-0.2/pantarei/helpers.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1111 2024-04-11 20:42:29.000000 pantarei-0.2/pantarei/hooks.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     9579 2024-04-11 21:27:17.000000 pantarei-0.2/pantarei/job.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     6587 2024-04-11 20:42:29.000000 pantarei-0.2/pantarei/parsers.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     5395 2024-04-11 20:42:29.000000 pantarei-0.2/pantarei/scheduler.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     5381 2024-04-11 20:42:29.000000 pantarei-0.2/pantarei/task.py
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-12 20:20:17.361712 pantarei-0.2/pantarei.egg-info/
+-rw-r--r--   0 coslo     (1000) coslo     (1000)     3694 2024-04-12 20:20:17.000000 pantarei-0.2/pantarei.egg-info/PKG-INFO
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      464 2024-04-12 20:20:17.000000 pantarei-0.2/pantarei.egg-info/SOURCES.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)        1 2024-04-12 20:20:17.000000 pantarei-0.2/pantarei.egg-info/dependency_links.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       25 2024-04-12 20:20:17.000000 pantarei-0.2/pantarei.egg-info/requires.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)        9 2024-04-12 20:20:17.000000 pantarei-0.2/pantarei.egg-info/top_level.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      719 2024-04-12 20:19:49.000000 pantarei-0.2/pyproject.toml
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      178 2024-04-12 20:20:17.365712 pantarei-0.2/setup.cfg
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-12 20:20:17.361712 pantarei-0.2/tests/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     6625 2024-04-11 21:27:17.000000 pantarei-0.2/tests/test.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    13119 2024-04-11 21:27:17.000000 pantarei-0.2/tests/test_db.py
```

### Comparing `pantarei-0.1.0/LICENSE` & `pantarei-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pantarei-0.1.0/PKG-INFO` & `pantarei-0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,21 @@
-Metadata-Version: 2.1
-Name: pantarei
-Version: 0.1.0
-Summary: A minimal and flexible workflow manager
-Author-email: Daniele Coslovich <daniele.coslovich@umontpellier.fr>
-License: GPLv3
-Project-URL: repository, https://framagit.org/coslo/pantarei
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: dill
-
 # Pantarei
 
 [![license](https://img.shields.io/pypi/l/atooms.svg)](https://en.wikipedia.org/wiki/GNU_General_Public_License)
-[![pipeline status](https://framagit.org/coslo/pantarei/badges/main/pipeline.svg)](https://framagit.org/coslo/pantarei/-/commits/main)
-[![coverage report](https://framagit.org/coslo/pantarei/badges/main/coverage.svg)](https://framagit.org/coslo/pantarei/-/commits/main)
-
-A minimal and flexible workflow manager
+[![pipeline status](https://framagit.org/coslo/pantarei/badges/master/pipeline.svg)](https://framagit.org/coslo/pantarei/-/commits/master)
+[![coverage report](https://framagit.org/coslo/pantarei/badges/master/coverage.svg)](https://framagit.org/coslo/pantarei/-/commits/master)
 
-## Features
-
-- [X] submit jobs on local slurm scheduler
-- [ ] handle task dependencies
-- [ ] submit on remote cluster
+A general-purpose workflow manager - because *everything* flows
 
 ## Quick start
 
-Pantarei builds on three different execution units:
+Pantarei builds on three kinds of execution units:
 - **functions** are stateless, Python callables
-- **tasks** are wrapped functions for shared-memory environments (single node)
-- **jobs** are wrapped tasks for distributed-memory environments (HPC clusters)
+- **tasks** are stateful wrapped functions that cache execution results
+- **jobs** are stateful wrapped tasks for distributed-memory parallel environments
 
 To see it in action, say you have a Python function
 ```python
 def f(x):
     import time
     time.sleep(2)
     return x
@@ -47,15 +26,15 @@
 from pantarei import *
 
 task = Task(f)
 for x in [1, 2]:
     task(x=x)
 ```
 
-The task's results are cached: a successive execution will just the results
+The task's results are cached: a successive execution will just fetch the results
 ```python
 results = task(x=1)
 ```
 
 We wrap the task with a Job and submit jobs to a local scheduler (like SLURM)
 ```python
 job = Job(task)
@@ -65,14 +44,72 @@
 
 Once the jobs are done, we can get the results (which are cached too)
 ```python
 job.scheduler.wait()
 results = job(x=3)
 ```
 
+To see a summary of the jobs from the Python intepreter, add the following line at the end
+```python
+pantarei()
+```
+
+From the command line, you can check the state of the jobs by changing the execution mode ('safe', 'brave', 'timid') like this
+```bash
+pantarei=timid python script.py
+```
+
+## TODO
+
+- [X] parametrize scheduler commands other than slurm
+- [ ] add command line tool
+- [ ] handle task dependencies
+- [ ] add Workflow / Queue
+- [ ] allow job submission within function
+- [ ] submit on remote cluster
+- [ ] perhaps add signac-like view() or checkout() method to check out a view of cache as folders
+- [ ] handle same function name from multiple modules/scripts
+
+## Mockups
+
+Handle task dependencies
+```python
+def run(path):
+    pass
+def analyze(path):
+    pass
+
+# TODO: how to use results of dependent tasks?
+run = Task(run, path='output.txt')
+analyze = Task(analyze, depends=[run], path='output.txt')
+
+for task in Workflow([run, analyze]):
+    task()
+```
+
+Jobs inherit task dependencies
+```python
+run = Job(run, wall_time=24, cores=8)
+analyze = Job(analyze, wall_time=1, cores=1)
+
+for job in Workflow([run, analyze]):
+    job()
+
+# Wait for analyze job to end
+job.scheduler.wait(analyze.fully_qualified_name())
+```
+
+Remote scheduler
+```python
+scheduler = Scheduler(host='login.m100.cineca.it', user='john_doe')
+job = Job(f, scheduler=scheduler)
+job(x=1)
+job.scheduler.wait()
+```
+
 ## Documentation
 
 Check out the [tutorial]() for more examples and the [public API]() for full details.
 
 ## Installation
 
 From pypi
@@ -83,8 +120,7 @@
 ## Contributing
 
 Contributions to the project are welcome. If you wish to contribute, check out [these guidelines]().
 
 ## Authors
 
 - Daniele Coslovich
-
```

### Comparing `pantarei-0.1.0/pantarei/_attempt.py` & `pantarei-0.2/pantarei/_attempt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,41 @@
+"""."""
 def submit_attempt(func, *args, **kwargs):
+    """."""
     import pickle
     import inspect
     import subprocess
     import traceback
-    
+
     stacks = inspect.stack()
     for i in range(len(stacks)):
         s = stacks[i]
         print('STACK', i+1, 'out of ', len(stacks))
         print('__code' in s.frame.f_locals)
         print(s.filename)
         print(s.frame.f_code, s.frame.f_code.co_firstlineno, s.frame.f_lineno, s.frame.f_code.co_filename)
-        #print(s.frame.f_locals)
+        # print(s.frame.f_locals)
         i = s.frame.f_code.co_firstlineno - 1
         j = s.frame.f_lineno - 1
         print(i, j, '-'*50)
         if s.frame.f_code.co_filename != '<stdin>':
-            with open(s.frame.f_code.co_filename)  as fh:
+            with open(s.frame.f_code.co_filename) as fh:
                 for _, line in enumerate(fh):
                     if i <= _ < j:
                         print(_, '>>', line.strip('\n'))
-                    elif i-3 <= _  <=  j+3:
+                    elif i-3 <= _ <= j+3:
                         print(_, '  ', line.strip('\n'))
         else:
             print('===== STDIN =====')
         print('-'*50)
         print()
-    
-    #frm = inspect.stack()[level]
-    #mod = inspect.getmodule(frm[0])
-    #s = inspect.stack()[2]
+
+    # frm = inspect.stack()[level]
+    # mod = inspect.getmodule(frm[0])
+    # s = inspect.stack()[2]
     s = stacks[-1]
     print('+++++', s.frame.f_code.co_filename, '__code' in s.frame.f_locals)
 
     PIK = "pickle.dat"
 
     # Remove modules
     # TODO: ignore callables like task and job instances
@@ -58,52 +60,54 @@
     for key in data:
         print('----', key, type(full[key]), callable(full[key]), key.startswith('__'))
         with open('/tmp/1.pkl', "wb") as f:
             try:
                 pickle.dump(full[key], f)
             except:
                 print('no pickle', key, full[key])
- 
+
     mods = {key: full[key] for key in full if (type(full[key]) != type(inspect))}
 
     with open(PIK, "wb") as f:
         pickle.dump(data, f)
 
     print('+++++', s.frame.f_code.co_filename, '__code' in s.frame.f_locals)
     code = ''
     if '__code' not in s.frame.f_locals:
         print('====== NOT found __code!')
         assert s.frame.f_code.co_filename != '<stdin>'
         i = s.frame.f_code.co_firstlineno - 1
         j = s.frame.f_lineno - 1
-        with open(s.frame.f_code.co_filename)  as fh:
+        with open(s.frame.f_code.co_filename) as fh:
             for _, line in enumerate(fh):
-                #if i <= _ <= j:
+                # if i <= _ <= j:
                 if i <= _ < j:
                     code += line
     else:
         print('====== USING __code!')
         for line in s.frame.f_locals['__code'].decode().split('\n'):
             # TODO: this is fragile
-            if line.strip().startswith('job('): continue
+            if line.strip().startswith('job('):
+                continue
             code += line + '\n'
 
     args = []
     for key in kwargs:
         if isinstance(kwargs[key], str):
             args.append(f'{key}="{kwargs[key]}"')
         else:
             args.append(f'{key}={kwargs[key]}')
     kwargs = ','.join(args)
 
     imports = []
     funcs_paste = []
     for key in funcs:
-        if key.startswith('_'): continue
-        #print('IMPRT ', key, funcs[key])
+        if key.startswith('_'):
+            continue
+        # print('IMPRT ', key, funcs[key])
         # These functions are defined locally in the session, we paste their code
         # TODO: it may duplicate the {code} below, we can fix it
         # One option is to store the bytecode and then import it
         # Or just simply accept that functions must be in modules.
         # if funcs[key] == '__main__': continue
         imports.append(f'from {funcs[key]} import {key}')
     imports = '\n'.join(imports)
@@ -131,15 +135,15 @@
 with open("{PIK}", "rb") as __fh:
     globals().update(pickle.load(__fh))
 {code}
 {func.__name__}({kwargs})
 """
     # TODO: we should return the results (pickling it)
     print(script)
-    #subprocess.run(f"""sbatch <<'EOF'
-    #print(f"""sbatch <<'EOF'
+    # subprocess.run(f"""sbatch <<'EOF'
+    # print(f"""sbatch <<'EOF'
     subprocess.run(f"""python - <<'EOF'
 {script}
 EOF""", shell=True)
-    #print(f"""python - <<EOF
-#{s.frame.f_locals['__code'].decode()}
-#EOF""")
+    # print(f"""python - <<EOF
+# {s.frame.f_locals['__code'].decode()}
+# EOF""")
```

### Comparing `pantarei-0.1.0/pantarei.egg-info/PKG-INFO` & `pantarei-0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 Metadata-Version: 2.1
 Name: pantarei
-Version: 0.1.0
-Summary: A minimal and flexible workflow manager
+Version: 0.2.0
+Summary: A general-purpose workflow manager
 Author-email: Daniele Coslovich <daniele.coslovich@umontpellier.fr>
 License: GPLv3
 Project-URL: repository, https://framagit.org/coslo/pantarei
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: tinydb
 Requires-Dist: dill
+Requires-Dist: pyyaml
 
 # Pantarei
 
 [![license](https://img.shields.io/pypi/l/atooms.svg)](https://en.wikipedia.org/wiki/GNU_General_Public_License)
-[![pipeline status](https://framagit.org/coslo/pantarei/badges/main/pipeline.svg)](https://framagit.org/coslo/pantarei/-/commits/main)
-[![coverage report](https://framagit.org/coslo/pantarei/badges/main/coverage.svg)](https://framagit.org/coslo/pantarei/-/commits/main)
+[![pipeline status](https://framagit.org/coslo/pantarei/badges/master/pipeline.svg)](https://framagit.org/coslo/pantarei/-/commits/master)
+[![coverage report](https://framagit.org/coslo/pantarei/badges/master/coverage.svg)](https://framagit.org/coslo/pantarei/-/commits/master)
 
-A minimal and flexible workflow manager
-
-## Features
-
-- [X] submit jobs on local slurm scheduler
-- [ ] handle task dependencies
-- [ ] submit on remote cluster
+A general-purpose workflow manager - because *everything* flows
 
 ## Quick start
 
-Pantarei builds on three different execution units:
+Pantarei builds on three kinds of execution units:
 - **functions** are stateless, Python callables
-- **tasks** are wrapped functions for shared-memory environments (single node)
-- **jobs** are wrapped tasks for distributed-memory environments (HPC clusters)
+- **tasks** are stateful wrapped functions that cache execution results
+- **jobs** are stateful wrapped tasks for distributed-memory parallel environments
 
 To see it in action, say you have a Python function
 ```python
 def f(x):
     import time
     time.sleep(2)
     return x
@@ -47,15 +44,15 @@
 from pantarei import *
 
 task = Task(f)
 for x in [1, 2]:
     task(x=x)
 ```
 
-The task's results are cached: a successive execution will just the results
+The task's results are cached: a successive execution will just fetch the results
 ```python
 results = task(x=1)
 ```
 
 We wrap the task with a Job and submit jobs to a local scheduler (like SLURM)
 ```python
 job = Job(task)
@@ -65,14 +62,72 @@
 
 Once the jobs are done, we can get the results (which are cached too)
 ```python
 job.scheduler.wait()
 results = job(x=3)
 ```
 
+To see a summary of the jobs from the Python intepreter, add the following line at the end
+```python
+pantarei()
+```
+
+From the command line, you can check the state of the jobs by changing the execution mode ('safe', 'brave', 'timid') like this
+```bash
+pantarei=timid python script.py
+```
+
+## TODO
+
+- [X] parametrize scheduler commands other than slurm
+- [ ] add command line tool
+- [ ] handle task dependencies
+- [ ] add Workflow / Queue
+- [ ] allow job submission within function
+- [ ] submit on remote cluster
+- [ ] perhaps add signac-like view() or checkout() method to check out a view of cache as folders
+- [ ] handle same function name from multiple modules/scripts
+
+## Mockups
+
+Handle task dependencies
+```python
+def run(path):
+    pass
+def analyze(path):
+    pass
+
+# TODO: how to use results of dependent tasks?
+run = Task(run, path='output.txt')
+analyze = Task(analyze, depends=[run], path='output.txt')
+
+for task in Workflow([run, analyze]):
+    task()
+```
+
+Jobs inherit task dependencies
+```python
+run = Job(run, wall_time=24, cores=8)
+analyze = Job(analyze, wall_time=1, cores=1)
+
+for job in Workflow([run, analyze]):
+    job()
+
+# Wait for analyze job to end
+job.scheduler.wait(analyze.fully_qualified_name())
+```
+
+Remote scheduler
+```python
+scheduler = Scheduler(host='login.m100.cineca.it', user='john_doe')
+job = Job(f, scheduler=scheduler)
+job(x=1)
+job.scheduler.wait()
+```
+
 ## Documentation
 
 Check out the [tutorial]() for more examples and the [public API]() for full details.
 
 ## Installation
 
 From pypi
@@ -83,8 +138,7 @@
 ## Contributing
 
 Contributions to the project are welcome. If you wish to contribute, check out [these guidelines]().
 
 ## Authors
 
 - Daniele Coslovich
-
```

### Comparing `pantarei-0.1.0/pyproject.toml` & `pantarei-0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 [project]
 name = "pantarei"
-description = "A minimal and flexible workflow manager"
+description = "A general-purpose workflow manager"
 readme = "README.md"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
     {name = "Daniele Coslovich", email = "daniele.coslovich@umontpellier.fr"}
 ]
 requires-python = ">=3.8"
 license = {text = "GPLv3"}
 dependencies = [
+    "numpy",
+    "tinydb",
     "dill",
+    "pyyaml"
 ]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3",
     "Development Status :: 5 - Production/Stable"
 ]
 
 [project.urls]
 repository = "https://framagit.org/coslo/pantarei"
 # homepage = ""
 # documentation = ""
 # changelog = ""
+
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
```

