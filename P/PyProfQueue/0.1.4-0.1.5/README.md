# Comparing `tmp/PyProfQueue-0.1.4.tar.gz` & `tmp/PyProfQueue-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyProfQueue-0.1.4.tar", last modified: Wed Apr 10 13:28:35 2024, max compression
+gzip compressed data, was "PyProfQueue-0.1.5.tar", last modified: Fri Apr 12 12:31:42 2024, max compression
```

## Comparing `PyProfQueue-0.1.4.tar` & `PyProfQueue-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-10 13:28:35.488657 PyProfQueue-0.1.4/
--rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     5681 2024-04-10 13:28:35.488657 PyProfQueue-0.1.4/PKG-INFO
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-10 13:28:35.488657 PyProfQueue-0.1.4/PyProfQueue/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      330 2024-04-09 11:17:32.000000 PyProfQueue-0.1.4/PyProfQueue/__init__.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-10 13:28:35.488657 PyProfQueue-0.1.4/PyProfQueue/data/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1453 2024-04-10 09:16:59.000000 PyProfQueue-0.1.4/PyProfQueue/data/likwid_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      811 2024-04-10 13:27:21.000000 PyProfQueue-0.1.4/PyProfQueue/data/prometheus_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     4517 2024-04-09 09:21:10.000000 PyProfQueue-0.1.4/PyProfQueue/data/read_prometheus.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    34226 2024-04-10 10:49:27.000000 PyProfQueue-0.1.4/PyProfQueue/script.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2367 2024-04-09 10:03:39.000000 PyProfQueue-0.1.4/PyProfQueue/submission.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-10 13:28:35.488657 PyProfQueue-0.1.4/PyProfQueue.egg-info/
--rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     5681 2024-04-10 13:28:35.000000 PyProfQueue-0.1.4/PyProfQueue.egg-info/PKG-INFO
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      393 2024-04-10 13:28:35.000000 PyProfQueue-0.1.4/PyProfQueue.egg-info/SOURCES.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)        1 2024-04-10 13:28:35.000000 PyProfQueue-0.1.4/PyProfQueue.egg-info/dependency_links.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       48 2024-04-10 13:28:35.000000 PyProfQueue-0.1.4/PyProfQueue.egg-info/requires.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       12 2024-04-10 13:28:35.000000 PyProfQueue-0.1.4/PyProfQueue.egg-info/top_level.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     4981 2024-04-10 08:22:46.000000 PyProfQueue-0.1.4/ReadMe.md
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       38 2024-04-10 13:28:35.488657 PyProfQueue-0.1.4/setup.cfg
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1196 2024-04-10 13:28:16.000000 PyProfQueue-0.1.4/setup.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-12 12:31:42.060063 PyProfQueue-0.1.5/
+-rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     5389 2024-04-12 12:31:42.060063 PyProfQueue-0.1.5/PKG-INFO
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-12 12:31:42.060063 PyProfQueue-0.1.5/PyProfQueue/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      330 2024-04-09 11:17:32.000000 PyProfQueue-0.1.5/PyProfQueue/__init__.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-12 12:31:42.060063 PyProfQueue-0.1.5/PyProfQueue/data/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1382 2024-04-12 11:54:50.000000 PyProfQueue-0.1.5/PyProfQueue/data/likwid_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      811 2024-04-10 13:27:21.000000 PyProfQueue-0.1.5/PyProfQueue/data/prometheus_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     5801 2024-04-12 10:47:29.000000 PyProfQueue-0.1.5/PyProfQueue/data/read_prometheus.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    37444 2024-04-12 11:53:45.000000 PyProfQueue-0.1.5/PyProfQueue/script.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2367 2024-04-09 10:03:39.000000 PyProfQueue-0.1.5/PyProfQueue/submission.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-12 12:31:42.060063 PyProfQueue-0.1.5/PyProfQueue.egg-info/
+-rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     5389 2024-04-12 12:31:42.000000 PyProfQueue-0.1.5/PyProfQueue.egg-info/PKG-INFO
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      393 2024-04-12 12:31:42.000000 PyProfQueue-0.1.5/PyProfQueue.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)        1 2024-04-12 12:31:42.000000 PyProfQueue-0.1.5/PyProfQueue.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       48 2024-04-12 12:31:42.000000 PyProfQueue-0.1.5/PyProfQueue.egg-info/requires.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       12 2024-04-12 12:31:42.000000 PyProfQueue-0.1.5/PyProfQueue.egg-info/top_level.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     4689 2024-04-11 12:23:42.000000 PyProfQueue-0.1.5/ReadMe.md
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       38 2024-04-12 12:31:42.060063 PyProfQueue-0.1.5/setup.cfg
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1196 2024-04-12 12:31:40.000000 PyProfQueue-0.1.5/setup.py
```

### Comparing `PyProfQueue-0.1.4/PKG-INFO` & `PyProfQueue-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyProfQueue
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python package to inject profiling initialisation into bash scripts, translate queue options and submit jobs
 Home-page: https://github.com/Marcus-Keil/PyProfQueue
 Author: Marcus Keil
 Author-email: marcusk050291@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -25,31 +25,27 @@
 When initiating a *Script* object, the following arguments are available:
 ```
 script = PyProfQueue.Script(queue_system: str,
                             work_script: str,
                             read_queue_system: str =None,
                             queue_options: dict = None,
                             likwid: bool = False,
-                            likwid_output: str = None,
                             likwid_req: list = None,
                             prometheus: bool = False,
-                            prometheus_output: str = None,
                             prometheus_req: list = None
                             )   
 ```
 - queue_system: The intended target queue system
 - work_script: The bash script which contains the queue options and work to be done
 - read_queue_system (Optional: defaults to queue_system): The name of the queue system for which the script was written 
 if different from queue_system
 - queue_options(Optional): Any queue options to add or override when compared to the work_script 
 - likwid (Optional: defaults to False): Bool to determine if likwid should be used
-- likwid_output (Optional): Likwid output directory, if a specific one is to be used
 - likwid_req (Optional): Likwid requirements, details can be found in the section about **add_likwid**
 - prometheus (Optional: defaults to False): Bool to determine if prometheus should be used
-- prometheus_output (Optional): Prometheus output directory, if a specific one is to be used
 - prometheus_req (Optional): Prometheus requirements, details can be found in the section about **add_prometheus**
 
 The *Script* class has a few methods that are intended for external use, these are:
 
 - **add_likwid**(likwid_req: list, likwid_output: str ='./')
   - Adds necessary initiation to use likwid to create a roof-line model and plot the work_script onto the model
   - This can be used if a *Script* object was not initiated with likwid options, or if they are to be changed
```

### Comparing `PyProfQueue-0.1.4/PyProfQueue/data/likwid_commands.txt` & `PyProfQueue-0.1.5/PyProfQueue/data/likwid_commands.txt`

 * *Files 22% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 likwid-bench -t load -W N:8GB:${THREAD_COUNT} | grep 'MByte/s:' >> ${LIK_OUTPUT}
 echo 'SSE MByte/s' >> ${LIK_OUTPUT}
 likwid-bench -t load_sse -W N:8GB:${THREAD_COUNT} | grep 'MByte/s:' >> ${LIK_OUTPUT}
 echo 'AVX MByte/s' >> ${LIK_OUTPUT}
 likwid-bench -t load_avx -W N:8GB:${THREAD_COUNT} | grep 'MByte/s:' >> ${LIK_OUTPUT}
 # *=*
 echo 'Program Performance' >> ${LIK_OUTPUT}
-grep -e 'MFLOP/s STAT' -e 'Operational intensity STAT' /cosma5/data/do011/dc-keil1/TestFiles/Results/First/${SLURM_JOB_NAME}-${SLURM_JOB_ID}/job_output_setup.txt >> ${LIK_OUTPUT}
+grep -e 'MFLOP/s STAT' -e 'Operational intensity STAT' ${WORKING_DIR}/job_output_setup.txt >> ${LIK_OUTPUT}
```

### Comparing `PyProfQueue-0.1.4/PyProfQueue/data/prometheus_commands.txt` & `PyProfQueue-0.1.5/PyProfQueue/data/prometheus_commands.txt`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1.4/PyProfQueue/script.py` & `PyProfQueue-0.1.5/PyProfQueue/script.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,25 +21,21 @@
             str of the queue system that the work_script was written for, if not specified it is assumed
             it is the same as queue_system. [sbatch, torque]
         queue_options : dict = None
             dictionary of options to be passed to the queue system.
         likwid : bool = False
             bool determining if likwid should be used to measure the performance such that a roofline
             model can be plotted
-        likwid_output: str = None
-            str of the path and name of the file to which the likwid values should be written to
         likwid_req: list = None
             list of the required lines that need to be added to a bash script in order to allow likwid
             to be used. For example, lines that load the likwid module if modules is being used on the
             system.
         prometheus : bool = False
             bool determining if prometheus should be used to measure the metrics of the node on which
             the script is being run.
-        prometheus_output: str = None
-            str of the path and name of the file to which the prometheus values should be written to
         prometheus_req: list = None
             list of the required lines that need to be added to a bash script in order to allow prometheus
             to be used. In order to run prometheus this list will need at least one entry:
                 'export PROMETHEUS_SOFTWARE=<path to the Prometheus software to be used>'
             with an optional entry to change the python executable to use by declaring:
                 'export PROMETHEUS_PYTHON=<path to the Python version to be used to scrape the prometheus database>'
             any additional entries will be added, but are at users discretion
@@ -60,49 +56,47 @@
         Examples
         -------- # As of now this example doesn't apply to this class.
         #>>> from PyProfQueue.script import Script
         #>>> ProfileScript = Script(queue_system='slurm',
                                     work_script='./example.sh',
                                     read_queue_system='slurm',
                                     likwid=True,
-                                    likwid_output='./',
                                     likwid_req=['module load oneAPI_comp',
                                                 'module load likwid'],
                                     prometheus=True,
-                                    prometheus_output='./',
                                     prometheus_req=['export PROMETHEUS_SOFTWARE=~/Software/prometheus'],
                                     queue_options={'user': 'user_name'})
     """
     def __init__(self, queue_system: str,
                  work_script: str,
                  read_queue_system: str = None,
                  queue_options: dict = None,
-                 likwid: bool = False, likwid_output: str = None, likwid_req: list = None,
-                 prometheus: bool = False, prometheus_output: str = None, prometheus_req: list = None):
+                 likwid: bool = False, likwid_req: list = None,
+                 prometheus: bool = False, prometheus_req: list = None):
         if True: # If statement added to allow for the collapse of the initiation of variables
             self.queue_system = queue_system
             self.work_script = work_script
             self.tmp_work_script = None
             self.tmp_profile_script = None
             self.works = None
+            self.work_dir = None
             self.likwid = likwid
             self.likwid_file = None
             self.likwid_initEndSplit = None
-            self.likwid_location = None
             self.likwid_req = None
             self.prometheus = prometheus
             self.prometheus_file = None
             self.prometheus_initEndSplit = None
             self.prometheus_location = None
             self.read_queue_system = read_queue_system
 
         if self.likwid:
-            self.add_likwid(likwid_req, likwid_output)
+            self.add_likwid(likwid_req)
         if self.prometheus:
-            self.add_prometheus(prometheus_req, prometheus_output)
+            self.add_prometheus(prometheus_req)
 
         if bool(queue_options):
             self.obj_options = self.Options(queue_options)
         else:
             self.obj_options = self.Options()
 
         # Queue System specifics {1}
@@ -147,14 +141,19 @@
         match self.queue_system:
             case 'slurm':
                 self.option_start = '#SBATCH '
                 self.submission = 'sbatch'
             case 'torque':
                 self.option_start = '#PBS '
                 self.submission = 'qsub'
+            case None:
+                if queue_options is None:
+
+                    print("No queue system was selected, therefore only queue_options['workdir'] is needed.")
+
             case _:
                 exit('No queue system chosen')
 
         match self.read_queue_system:
             case 'slurm':
                 self.read_option_start = '#SBATCH '
                 options = self.option_pass()
@@ -162,33 +161,35 @@
                 self.outputvariable_convert()
             case 'torque':
                 self.read_option_start = '#PBS '
                 options = self.option_pass()
                 self.obj_options.torque_options(options)
                 self.outputvariable_convert()
             case None:
-                if queue_options is None:
+                if self.queue_system is None:
+                    if self.obj_options.workdir is None:
+                        self.obj_options.workdir = './'
+                elif queue_options is None:
                     exit('"read_queue_system" was left as None, but no queue options were provided with "queue_options"')
                 else:
                     self.outputvariable_convert()
 
             case _:
                 exit('Provided queue system, {}, is not supported in the initialisation '
                      '"match self.read_queue_system"'.format(self.read_queue_system))
         # ==========================
         self.obj_options.remove_empty_options()
 
-    def add_likwid(self, likwid_req, likwid_output='./'):
+    def add_likwid(self, likwid_req):
         self.likwid = True
         self.likwid_file = impresources.files(data) / "likwid_commands.txt"
         self.likwid_initEndSplit = -1
-        self.likwid_location = likwid_output
         self.likwid_req = likwid_req
 
-    def add_prometheus(self, prometheus_req, prometheus_output='./'):
+    def add_prometheus(self, prometheus_req):
         contains_ps = False
         contains_pp = False
         for req in prometheus_req:
             if 'PROMETHEUS_SOFTWARE' in req:
                 contains_ps = True
                 continue
             if 'PROMETHEUS_PYTHON' in req:
@@ -203,15 +204,14 @@
             contains_pp = True
 
         if not contains_ps or not contains_pp:
             exit('When requesting prometheus profiling, prometheus_req must include "export PROMETHEUS_SOFTWARE=".')
         self.prometheus = True
         self.prometheus_file = impresources.files(data) / "prometheus_commands.txt"
         self.prometheus_initEndSplit = -1
-        self.prometheus_location = prometheus_output
         self.prometheus_req = prometheus_req
 
     def option_pass(self):
         options, self.works = self.read_script()
         return options
 
     # Queue System specifics {2}
@@ -235,21 +235,54 @@
     slurm needs to use ${SLURM_JOB_NAME} or ${SLURM_JOB_ID} for %x and %j respectively.
     #####
     Template for new read_queue_system case:
     =====
     case '<queue_name>':
         match self.queue_system:
             case 'slurm':
-                self.obj_options.output = self.obj_options.output.replace(<'<special format>' or job_directory>, '%x.%j')
-                working_dir = self.obj_options.output[:-4]
+                self.obj_options.output = self.obj_options.output\
+                    .replace('<Job_Name_Variable>', '%x')\
+                    .replace('<Job_ID_Variable>', '%j')
+                if self.obj_options.workdir is not None:
+                    self.work_dir = self.obj_options.workdir\
+                        .replace('%x', '${SLURM_JOB_NAME}')\
+                        .replace('%j', '${SLURM_JOB_ID}')
+                else:
+                    self.work_dir = self.obj_options.output[:-4]\
+                        .replace('%x', '<Job_Name_Variable>')\
+                        .replace('%j', '<Job_ID_Variable>')
             case 'torque':
-                self.obj_options.output = self.obj_options.output.replace('<special format>', job_directory)
-                working_dir = self.obj_options.output[:-4]
+                self.obj_options.output = self.obj_options.output \
+                    .replace('<Job_Name_Variable>', '${PBS_JOBNAME}') \
+                    .replace('<Job_ID_Variable>', '${PBS_JOBID}')
+                if self.obj_options.workdir is not None:
+                    self.work_dir = self.obj_options.workdir
+                else:
+                    self.work_dir = self.obj_options.output[:-4]
             case '<queue_name>':
-                working_dir = self.obj_options.output[:-4] # .replace('<special format>', job_directory) # if this queue system has a special format
+                # if the new queue system doesn't have special formats for designating Job_Name and Job_ID in options
+                # like slurm does, use this:
+                if self.obj_options.workdir is not None:
+                    self.work_dir = self.obj_options.workdir
+                else:
+                    self.work_dir = self.obj_options.output[:-4]
+                # if, like slurm, it has a special option only format for Job_Name and Job_ID use:
+                self.obj_options.output = self.obj_options.output\
+                    .replace('<Script_Job_Name_Variable>', '<Option_Job_Name_Variable>')\
+                    .replace('<Script_Job_ID_Variable>', '<Option_Job_ID_Variable>')
+                if self.obj_options.workdir is not None:
+                    self.work_dir = self.obj_options.workdir\
+                        .replace('<Script_Job_Name_Variable>', '<Option_Job_Name_Variable>')\
+                        .replace('<Script_Job_ID_Variable>', '<Option_Job_ID_Variable>')
+                else:
+                    self.work_dir = self.obj_options.output[:-4]\
+                        .replace('<Script_Job_Name_Variable>', '<Option_Job_Name_Variable>')\
+                        .replace('<Script_Job_ID_Variable>', '<Option_Job_ID_Variable>')
+            case None:
+                pass
             case _:
                 exit('queue_system was unknown  when translating from <queue_name> to {}'.format(self.queue_system))
     =====
     Template for the nested case in old queue systems:
     =====
     # For Slurm
     case '<queue_name>':
@@ -258,61 +291,85 @@
     # For systems like Torque that don't have special formating in the option section
     case '<queue_name>':
         self.obj_options.output = self.obj_options.output.replace(job_directory, <'<special format>' or job_directory>)
         working_dir = self.obj_options.output[:-4]
     =====
     -----
     '''
+    # ==========================
     def outputvariable_convert(self):
         match self.read_queue_system:
             case 'slurm':
                 match self.queue_system:
                     case 'slurm':
-                        working_dir = self.obj_options.output[:-4]\
-                            .replace('%x', '${SLURM_JOB_NAME}')\
-                            .replace('%j', '${SLURM_JOB_ID}')
+                        if self.obj_options.workdir is not None:
+                            self.work_dir = self.obj_options.workdir\
+                                .replace('%x', '${SLURM_JOB_NAME}')\
+                                .replace('%j', '${SLURM_JOB_ID}')
+                        else:
+                            self.work_dir = self.obj_options.output[:-4]\
+                                .replace('%x', '${SLURM_JOB_NAME}')\
+                                .replace('%j', '${SLURM_JOB_ID}')
                     case 'torque':
-                        self.obj_options.output = self.obj_options.output\
-                            .replace('%x', '${PBS_JOBNAME}')\
+                        self.obj_options.output = self.obj_options.output \
+                            .replace('%x', '${PBS_JOBNAME}') \
                             .replace('%j', '${PBS_JOBID}')
-                        working_dir = self.obj_options.output[:-4]
+                        if self.obj_options.workdir is not None:
+                            self.work_dir = self.obj_options.workdir
+                        else:
+                            self.work_dir = self.obj_options.output[:-4]
+                    case None:
+                        pass
                     case _:
                         exit('queue_system was unknown when translating from slurm to {}'.format(self.queue_system))
             case 'torque':
                 match self.queue_system:
                     case 'slurm':
                         self.obj_options.output = self.obj_options.output\
                             .replace('${PBS_JOBNAME}', '%x')\
                             .replace('${PBS_JOBID}', '%j')
-                        working_dir = self.obj_options.output[:-4]\
-                            .replace('%x', '${SLURM_JOB_NAME}')\
-                            .replace('%j', '${SLURM_JOB_ID}')
+                        if self.obj_options.workdir is not None:
+                            self.work_dir = self.obj_options.workdir\
+                                .replace('%x', '${SLURM_JOB_NAME}')\
+                                .replace('%j', '${SLURM_JOB_ID}')
+                        else:
+                            self.work_dir = self.obj_options.output[:-4]\
+                                .replace('%x', '${SLURM_JOB_NAME}')\
+                                .replace('%j', '${SLURM_JOB_ID}')
                     case 'torque':
-                        working_dir = self.obj_options.output[:-4]
+                        if self.obj_options.workdir is not None:
+                            self.work_dir = self.obj_options.workdir
+                        else:
+                            self.work_dir = self.obj_options.output[:-4]
+                    case None:
+                        pass
                     case _:
                         exit('queue_system was unknown when translating from torque to {}'.format(self.queue_system))
             case None:
                 match self.queue_system:
                     case 'slurm':
-                        working_dir = self.obj_options.output[:-4] \
-                            .replace('%x', '${SLURM_JOB_NAME}') \
-                            .replace('%j', '${SLURM_JOB_ID}')
+                        if self.obj_options.workdir is not None:
+                            self.work_dir = self.obj_options.workdir\
+                                .replace('%x', '${SLURM_JOB_NAME}')\
+                                .replace('%j', '${SLURM_JOB_ID}')
+                        else:
+                            self.work_dir = self.obj_options.output[:-4] \
+                                .replace('%x', '${SLURM_JOB_NAME}') \
+                                .replace('%j', '${SLURM_JOB_ID}')
                     case 'torque':
-                        working_dir = self.obj_options.output[:-4]
+                        if self.obj_options.workdir is not None:
+                            self.work_dir = self.obj_options.workdir
+                        else:
+                            self.work_dir = self.obj_options.output[:-4]
                     case _:
                         exit('queue_system was unknown when translating from no queue '
                              'system to {}'.format(self.queue_system))
             case _:
                 exit('read_queue_system was unknown with value: {}'.format(self.read_queue_system))
-
-        if self.obj_options.workdir is None:
-            self.output_dir = working_dir
-        else:
-            self.output_dir = self.obj_options.workdir
-
+    # ==========================
     class Options:
         def __init__(self, queue_options: dict = None):
             self.user = None
             self.nodes = None
             self.cores = None
             self.tasks = None
             self.time = None
@@ -346,14 +403,21 @@
                     case 'workdir':
                         self.workdir = value
                     case 'output':
                         self.output = value
                     case _:
                         exit('Unknown option value in key: {}, with value: {} passed to pass_options'.format(key, value))
 
+        def remove_empty_options(self):
+            empty_attributes = [a for a in dir(self) if (not a.startswith('__') and
+                                                         not callable(getattr(self, a)) and
+                                                         getattr(self, a) is None)]
+            for attribute in empty_attributes:
+                delattr(self, attribute)
+
         # Queue System specifics {3}
         '''
         -----
         To add a new queue system, this section needs to have a new function declared.
         This function needs to take self and a dictionary of options. This dictionary will use the queue options
         from the bash script provided as keys, with the values being the declared options in the bash script.
         The match function will then match each option to the correct variables. These variables are:
@@ -423,14 +487,15 @@
                             continue
                         else:
                             self.output = value
                     case _:
                         exit('Unknown option value in key: {}, with value: {} passed to <queue_name>_options'.format(key, value))
         =====
         '''
+        # ==========================
         def slurm_options(self, slurm_options):
             for key, value in slurm_options.items():
                 match key:
                     case 'uid':
                         if self.user is not None:
                             continue
                         else:
@@ -534,21 +599,15 @@
                     case 'o':
                         if self.output is not None:
                             continue
                         else:
                             self.output = value
                     case _:
                         exit('Unknown option value in key: {}, with value: {} passed to torque_options'.format(key, value))
-
-        def remove_empty_options(self):
-            empty_attributes = [a for a in dir(self) if (not a.startswith('__') and
-                                                         not callable(getattr(self, a)) and
-                                                         getattr(self, a) is None)]
-            for attribute in empty_attributes:
-                delattr(self, attribute)
+        # ==========================
 
     def change_options(self, queue_options: dict):
         self.obj_options.pass_options(queue_options)
 
     # Queue System specifics {4}
     '''
     -----
@@ -600,16 +659,16 @@
                 return ''
             case 'workdir':
                 return ''
             case 'output':
                 return ''
     =====
     '''
+    # ==========================
     def option_converter(self, option):
-        # ==========================
         match self.queue_system:
             case 'slurm':
                 match option:
                     case 'user':
                         return '--uid='
                     case 'nodes':
                         return '-N '
@@ -647,15 +706,15 @@
                         return '-A '
                     case 'subname':
                         return '-N '
                     case 'workdir':
                         return '-d '
                     case 'output':
                         return '-o '
-        # ==========================
+    # ==========================
 
     def read_script(self):
         options = {}
         work = []
         with open(self.work_script, 'r') as script:
             for line in script.readlines():
                 if self.read_option_start in line:
@@ -693,19 +752,22 @@
         else:
             self.tmp_work_script = self.work_script
         self.tmp_profile_script = tmp_profile_script
 
         with open(self.tmp_profile_script, 'w') as profilefile:
             profilefile.seek(0)
             profilefile.write('#!/bin/bash\n')
-            self.add_options(profilefile)
-            if self.prometheus or self.likwid:
-                profilefile.write('export WORKING_DIR={}\n'.format(self.output_dir))
-                profilefile.write('mkdir ${WORKING_DIR}\n')
-                profilefile.write('\n')
+            if self.queue_system is not None:
+                self.add_options(profilefile)
+
+            profilefile.write('export WORKING_DIR={}\n'.format(self.work_dir))
+            profilefile.write('mkdir ${WORKING_DIR}\n')
+            if self.queue_system is None:
+                profilefile.write('cd ${WORKING_DIR}\n')
+            profilefile.write('\n')
 
             if self.likwid:
                 self.init_likwid(profilefile)
 
             if self.prometheus:
                 self.init_prometheus(profilefile)
```

### Comparing `PyProfQueue-0.1.4/PyProfQueue/submission.py` & `PyProfQueue-0.1.5/PyProfQueue/submission.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1.4/PyProfQueue.egg-info/PKG-INFO` & `PyProfQueue-0.1.5/PyProfQueue.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyProfQueue
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python package to inject profiling initialisation into bash scripts, translate queue options and submit jobs
 Home-page: https://github.com/Marcus-Keil/PyProfQueue
 Author: Marcus Keil
 Author-email: marcusk050291@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -25,31 +25,27 @@
 When initiating a *Script* object, the following arguments are available:
 ```
 script = PyProfQueue.Script(queue_system: str,
                             work_script: str,
                             read_queue_system: str =None,
                             queue_options: dict = None,
                             likwid: bool = False,
-                            likwid_output: str = None,
                             likwid_req: list = None,
                             prometheus: bool = False,
-                            prometheus_output: str = None,
                             prometheus_req: list = None
                             )   
 ```
 - queue_system: The intended target queue system
 - work_script: The bash script which contains the queue options and work to be done
 - read_queue_system (Optional: defaults to queue_system): The name of the queue system for which the script was written 
 if different from queue_system
 - queue_options(Optional): Any queue options to add or override when compared to the work_script 
 - likwid (Optional: defaults to False): Bool to determine if likwid should be used
-- likwid_output (Optional): Likwid output directory, if a specific one is to be used
 - likwid_req (Optional): Likwid requirements, details can be found in the section about **add_likwid**
 - prometheus (Optional: defaults to False): Bool to determine if prometheus should be used
-- prometheus_output (Optional): Prometheus output directory, if a specific one is to be used
 - prometheus_req (Optional): Prometheus requirements, details can be found in the section about **add_prometheus**
 
 The *Script* class has a few methods that are intended for external use, these are:
 
 - **add_likwid**(likwid_req: list, likwid_output: str ='./')
   - Adds necessary initiation to use likwid to create a roof-line model and plot the work_script onto the model
   - This can be used if a *Script* object was not initiated with likwid options, or if they are to be changed
```

### Comparing `PyProfQueue-0.1.4/ReadMe.md` & `PyProfQueue-0.1.5/ReadMe.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,31 +6,27 @@
 When initiating a *Script* object, the following arguments are available:
 ```
 script = PyProfQueue.Script(queue_system: str,
                             work_script: str,
                             read_queue_system: str =None,
                             queue_options: dict = None,
                             likwid: bool = False,
-                            likwid_output: str = None,
                             likwid_req: list = None,
                             prometheus: bool = False,
-                            prometheus_output: str = None,
                             prometheus_req: list = None
                             )   
 ```
 - queue_system: The intended target queue system
 - work_script: The bash script which contains the queue options and work to be done
 - read_queue_system (Optional: defaults to queue_system): The name of the queue system for which the script was written 
 if different from queue_system
 - queue_options(Optional): Any queue options to add or override when compared to the work_script 
 - likwid (Optional: defaults to False): Bool to determine if likwid should be used
-- likwid_output (Optional): Likwid output directory, if a specific one is to be used
 - likwid_req (Optional): Likwid requirements, details can be found in the section about **add_likwid**
 - prometheus (Optional: defaults to False): Bool to determine if prometheus should be used
-- prometheus_output (Optional): Prometheus output directory, if a specific one is to be used
 - prometheus_req (Optional): Prometheus requirements, details can be found in the section about **add_prometheus**
 
 The *Script* class has a few methods that are intended for external use, these are:
 
 - **add_likwid**(likwid_req: list, likwid_output: str ='./')
   - Adds necessary initiation to use likwid to create a roof-line model and plot the work_script onto the model
   - This can be used if a *Script* object was not initiated with likwid options, or if they are to be changed
```

### Comparing `PyProfQueue-0.1.4/setup.py` & `PyProfQueue-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "ReadMe.md").read_text()
 
 setup(
     name='PyProfQueue',
-    version='0.1.4',
+    version='0.1.5',
     url='https://github.com/Marcus-Keil/PyProfQueue',
     author='Marcus Keil',
     author_email='marcusk050291@gmail.com',
     license='MIT License',
     packages=['PyProfQueue'],
     package_dir={'PyProfQueue': 'PyProfQueue'},
     package_data={'PyProfQueue': ['../ReadMe.md', 'data/*.txt', 'data/read_prometheus.py']},
```

