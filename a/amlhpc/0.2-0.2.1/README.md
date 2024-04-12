# Comparing `tmp/amlhpc-0.2.tar.gz` & `tmp/amlhpc-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amlhpc-0.2.tar", max compression
+gzip compressed data, was "amlhpc-0.2.1.tar", max compression
```

## Comparing `amlhpc-0.2.tar` & `amlhpc-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3099 2023-12-31 10:57:42.563176 amlhpc-0.2/README.md
--rw-r--r--   0        0        0        0 2023-12-24 18:49:13.493853 amlhpc-0.2/amlhpc/__init__.py
--rw-r--r--   0        0        0      670 2023-12-24 18:49:13.502339 amlhpc-0.2/amlhpc/__main__.py
--rw-r--r--   0        0        0       55 2023-12-24 18:49:13.517634 amlhpc-0.2/amlhpc/pbs/qsub.py
--rw-r--r--   0        0        0    11823 2024-01-10 10:44:27.664244 amlhpc-0.2/amlhpc/slurm/sbatch.py
--rw-r--r--   0        0        0     2108 2024-01-10 10:43:30.441895 amlhpc-0.2/amlhpc/slurm/sinfo.py
--rw-r--r--   0        0        0     1949 2024-01-10 10:43:51.706120 amlhpc-0.2/amlhpc/slurm/squeue.py
--rw-r--r--   0        0        0      746 2024-01-11 07:13:10.909897 amlhpc-0.2/pyproject.toml
--rw-r--r--   0        0        0     3682 1970-01-01 00:00:00.000000 amlhpc-0.2/PKG-INFO
+-rw-r--r--   0        0        0     3099 2024-01-11 17:06:17.001526 amlhpc-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-12-24 18:49:13.493853 amlhpc-0.2.1/amlhpc/__init__.py
+-rw-r--r--   0        0        0      670 2023-12-24 18:49:13.502339 amlhpc-0.2.1/amlhpc/__main__.py
+-rw-r--r--   0        0        0       55 2023-12-24 18:49:13.517634 amlhpc-0.2.1/amlhpc/pbs/qsub.py
+-rw-r--r--   0        0        0    12395 2024-04-12 07:38:38.124804 amlhpc-0.2.1/amlhpc/slurm/sbatch.py
+-rw-r--r--   0        0        0     2108 2024-01-10 10:43:30.441895 amlhpc-0.2.1/amlhpc/slurm/sinfo.py
+-rw-r--r--   0        0        0     1949 2024-01-10 10:43:51.706120 amlhpc-0.2.1/amlhpc/slurm/squeue.py
+-rw-r--r--   0        0        0      748 2024-04-04 13:02:19.654720 amlhpc-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3684 1970-01-01 00:00:00.000000 amlhpc-0.2.1/PKG-INFO
```

### Comparing `amlhpc-0.2/README.md` & `amlhpc-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -62,8 +62,8 @@
   -p PARTITION, --partition PARTITION
                         set compute partition where the job should be run. Use <sinfo> to view available partitions
   -N NODES, --nodes NODES
                         amount of nodes to use for the job
   -w WRAP, --wrap WRAP  command line to be executed, should be enclosed with quotes
 ```
 
-If you encounter a scenario or option that is not supoprted yet or behaves unexpected, please create an issue and explain the option and the scenario.
+If you encounter a scenario or option that is not supported yet or behaves unexpected, please create an issue and explain the option and the scenario.
```

### Comparing `amlhpc-0.2/amlhpc/__main__.py` & `amlhpc-0.2.1/amlhpc/__main__.py`

 * *Files identical despite different names*

### Comparing `amlhpc-0.2/amlhpc/slurm/sbatch.py` & `amlhpc-0.2.1/amlhpc/slurm/sbatch.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     parser = argparse.ArgumentParser(description='sbatch: submit jobs to Azure Machine Learning')
     parser.prog = "sbatch"
     parser.add_argument('-a', '--array', default="None", type=str, help='index for array jobs')
     parser.add_argument('--container', default="None", type=str, help='container environment for the job to run in')
     parser.add_argument('--datamover', default="None", type=str, help='use "simple" for moving the (recursive) data along with the runscript')
     parser.add_argument('-e', '--environment', default="None", type=str, help='Azure Machine Learning environment, should be enclosed in quotes, may use @latest')
     parser.add_argument('-N', '--nodes', default=1, type=int, help='amount of nodes to use for the job')
-    parser.add_argument('-p', '--partition', type=str, required=True,
+    parser.add_argument('-p', '--partition', default="None", type=str, 
                         help='set compute partition where the job should be run. Use <sinfo> to view available partitions')
     #parser.add_argument('--parallel', default="single", type=str, help='command line to be executed, should be enclosed with quotes')
     parser.add_argument('-v', '--verbose', action='count', default=0,  help='provide output on found settings and job properties')
     parser.add_argument('-w', '--wrap', type=str, help='command line to be executed, should be enclosed with quotes')
     parser.add_argument('script', nargs='?', default="None", type=str, help='runscript to be executed')
     args = parser.parse_args(vargs)
     args.parallel="single"
@@ -74,14 +74,27 @@
         print("Missing: provide either script to execute as argument or commandline to execute through --wrap option")
         exit(-1)
 
     if (args.script != "None") and (args.wrap is not None):
         print("Conflict: provide either script to execute as argument or commandline to execute through --wrap option")
         exit(-1)
 
+    if (args.script != "None"):
+        f = open(args.script, "r")
+        lines = f.readlines()
+        for line in lines:
+            if line.startswith('#SBATCH -p ') or line.startswith('#SBATCH --partition '):
+                words = list(line.split(" "))
+                args.partition = words[2] 
+                if (args.verbose): print("partition argument from runscript: " + args.partition) 
+
+    if (args.partition == "None"):
+        print("Missing: provide partition to run the job, either as -p argument or as configuration in runscript")
+        exit(-1)
+
     if (args.container != "None") and (args.environment != "None"):
         print("Conflict: provide either container or environment, cannot be used together")
         exit(-1)
 
     if (args.container != "None"):
         if (args.verbose): print("using container: " + args.container) 
         env_docker_image = Environment(
```

### Comparing `amlhpc-0.2/amlhpc/slurm/sinfo.py` & `amlhpc-0.2.1/amlhpc/slurm/sinfo.py`

 * *Files identical despite different names*

### Comparing `amlhpc-0.2/amlhpc/slurm/squeue.py` & `amlhpc-0.2.1/amlhpc/slurm/squeue.py`

 * *Files identical despite different names*

### Comparing `amlhpc-0.2/pyproject.toml` & `amlhpc-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "amlhpc"
-version = "0.2"
+version = "0.2.1"
 authors = [ "Hugo Meiland <hugo.meiland@microsoft.com>", "Utkarsh Ayachit <uayachit@microsoft.com>" ]
 description = "Emulate Slurm/PBS/LSF HPC scheduler in Azure ML"
 readme = "README.md"
 packages = [
     { include = "amlhpc" }
 ]
```

### Comparing `amlhpc-0.2/PKG-INFO` & `amlhpc-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amlhpc
-Version: 0.2
+Version: 0.2.1
 Summary: Emulate Slurm/PBS/LSF HPC scheduler in Azure ML
 Author: Hugo Meiland
 Author-email: hugo.meiland@microsoft.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -78,9 +78,9 @@
   -p PARTITION, --partition PARTITION
                         set compute partition where the job should be run. Use <sinfo> to view available partitions
   -N NODES, --nodes NODES
                         amount of nodes to use for the job
   -w WRAP, --wrap WRAP  command line to be executed, should be enclosed with quotes
 ```
 
-If you encounter a scenario or option that is not supoprted yet or behaves unexpected, please create an issue and explain the option and the scenario.
+If you encounter a scenario or option that is not supported yet or behaves unexpected, please create an issue and explain the option and the scenario.
```

