# Comparing `tmp/snakemake_executor_plugin_slurm-0.4.2.tar.gz` & `tmp/snakemake_executor_plugin_slurm-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_executor_plugin_slurm-0.4.2.tar", max compression
+gzip compressed data, was "snakemake_executor_plugin_slurm-0.4.3.tar", max compression
```

## Comparing `snakemake_executor_plugin_slurm-0.4.2.tar` & `snakemake_executor_plugin_slurm-0.4.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1076 2024-03-11 20:58:11.712047 snakemake_executor_plugin_slurm-0.4.2/LICENSE
--rw-r--r--   0        0        0      319 2024-03-11 20:58:11.712047 snakemake_executor_plugin_slurm-0.4.2/README.md
--rw-r--r--   0        0        0     1152 2024-03-11 20:58:11.712047 snakemake_executor_plugin_slurm-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    19994 2024-03-11 20:58:11.712047 snakemake_executor_plugin_slurm-0.4.2/snakemake_executor_plugin_slurm/__init__.py
--rw-r--r--   0        0        0     1381 1970-01-01 00:00:00.000000 snakemake_executor_plugin_slurm-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-12 08:17:08.233040 snakemake_executor_plugin_slurm-0.4.3/LICENSE
+-rw-r--r--   0        0        0      319 2024-04-12 08:17:08.233040 snakemake_executor_plugin_slurm-0.4.3/README.md
+-rw-r--r--   0        0        0     1152 2024-04-12 08:17:08.233040 snakemake_executor_plugin_slurm-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0    20487 2024-04-12 08:17:08.233040 snakemake_executor_plugin_slurm-0.4.3/snakemake_executor_plugin_slurm/__init__.py
+-rw-r--r--   0        0        0     1381 1970-01-01 00:00:00.000000 snakemake_executor_plugin_slurm-0.4.3/PKG-INFO
```

### Comparing `snakemake_executor_plugin_slurm-0.4.2/LICENSE` & `snakemake_executor_plugin_slurm-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemake_executor_plugin_slurm-0.4.2/pyproject.toml` & `snakemake_executor_plugin_slurm-0.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snakemake-executor-plugin-slurm"
-version = "0.4.2"
+version = "0.4.3"
 description = "A Snakemake executor plugin for submitting jobs to a SLURM cluster."
 authors = [
     "Christian Meesters <meesters@uni-mainz.de>",
     "David Lähnemann <david.laehnemann@dkfz-heidelberg.de>",
     "Johannes Koester <johannes.koester@uni-due.de>",
 ]
 readme = "README.md"
```

### Comparing `snakemake_executor_plugin_slurm-0.4.2/snakemake_executor_plugin_slurm/__init__.py` & `snakemake_executor_plugin_slurm-0.4.3/snakemake_executor_plugin_slurm/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,25 +61,33 @@
         # You can access the job's resources, etc.
         # via the job object.
         # After submitting the job, you have to call
         # self.report_job_submission(job_info).
         # with job_info being of type
         # snakemake_interface_executor_plugins.executors.base.SubmittedJobInfo.
 
-        log_folder = f"group_{job.name}" if job.is_group() else f"rule_{job.name}"
+        group_or_rule = f"group_{job.name}" if job.is_group() else f"rule_{job.name}"
 
         try:
             wildcard_str = f"_{'_'.join(job.wildcards)}" if job.wildcards else ""
         except AttributeError:
             wildcard_str = ""
 
         slurm_logfile = os.path.abspath(
-            f".snakemake/slurm_logs/{log_folder}/%j{wildcard_str}.log"
+            f".snakemake/slurm_logs/{group_or_rule}/{wildcard_str}/%j.log"
         )
-        os.makedirs(os.path.dirname(slurm_logfile), exist_ok=True)
+        logdir = os.path.dirname(slurm_logfile)
+        # this behavior has been fixed in slurm 23.02, but there might be plenty of
+        # older versions around, hence we should rather be conservative here.
+        assert "%j" not in logdir, (
+            "bug: jobid placeholder in parent dir of logfile. This does not work as "
+            "we have to create that dir before submission in order to make sbatch "
+            "happy. Otherwise we get silent fails without logfiles being created."
+        )
+        os.makedirs(logdir, exist_ok=True)
 
         # generic part of a submission string:
         # we use a run_uuid as the job-name, to allow `--name`-based
         # filtering in the job status checks (`sacct --name` and `squeue --name`)
         call = (
             f"sbatch --job-name {self.run_uuid} --output {slurm_logfile} --export=ALL "
             f"--comment {job.name}"
```

### Comparing `snakemake_executor_plugin_slurm-0.4.2/PKG-INFO` & `snakemake_executor_plugin_slurm-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemake-executor-plugin-slurm
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Snakemake executor plugin for submitting jobs to a SLURM cluster.
 Home-page: https://github.com/snakemake/snakemake-executor-plugin-slurm
 License: MIT
 Keywords: snakemake,plugin,executor,cluster,slurm
 Author: Christian Meesters
 Author-email: meesters@uni-mainz.de
 Requires-Python: >=3.11,<4.0
```

