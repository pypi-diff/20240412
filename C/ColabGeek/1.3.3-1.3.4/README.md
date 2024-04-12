# Comparing `tmp/ColabGeek-1.3.3.tar.gz` & `tmp/ColabGeek-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ColabGeek-1.3.3.tar", last modified: Mon Mar 11 10:07:35 2024, max compression
+gzip compressed data, was "ColabGeek-1.3.4.tar", last modified: Fri Apr 12 03:16:51 2024, max compression
```

## Comparing `ColabGeek-1.3.3.tar` & `ColabGeek-1.3.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-03-11 10:07:35.912924 ColabGeek-1.3.3/
--rw-rw-r--   0 sunym     (1000) sunym     (1000)     1067 2024-03-11 10:04:40.000000 ColabGeek-1.3.3/LICENSE
--rw-r--r--   0 sunym     (1000) sunym     (1000)     8758 2024-03-11 10:07:35.912924 ColabGeek-1.3.3/PKG-INFO
--rw-rw-r--   0 sunym     (1000) sunym     (1000)     8022 2024-03-11 10:04:40.000000 ColabGeek-1.3.3/README.md
--rw-rw-r--   0 sunym     (1000) sunym     (1000)      940 2024-03-11 10:04:40.000000 ColabGeek-1.3.3/pyproject.toml
--rw-rw-r--   0 sunym     (1000) sunym     (1000)       38 2024-03-11 10:07:35.912924 ColabGeek-1.3.3/setup.cfg
-drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-03-11 10:07:35.909924 ColabGeek-1.3.3/src/
-drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-03-11 10:07:35.910924 ColabGeek-1.3.3/src/ColabGeek/
--rw-rw-r--   0 sunym     (1000) sunym     (1000)    27436 2024-03-11 10:04:40.000000 ColabGeek-1.3.3/src/ColabGeek/ColabGeek.py
--rw-rw-r--   0 sunym     (1000) sunym     (1000)       25 2024-03-11 10:04:40.000000 ColabGeek-1.3.3/src/ColabGeek/__init__.py
-drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-03-11 10:07:35.911924 ColabGeek-1.3.3/src/ColabGeek/shell_scripts/
--rw-rw-r--   0 sunym     (1000) sunym     (1000)      817 2024-03-11 10:04:40.000000 ColabGeek-1.3.3/src/ColabGeek/shell_scripts/Install_Homebrew.exp
--rw-rw-r--   0 sunym     (1000) sunym     (1000)      325 2024-03-11 10:04:40.000000 ColabGeek-1.3.3/src/ColabGeek/shell_scripts/Install_Jekyll.exp
--rw-rw-r--   0 sunym     (1000) sunym     (1000)      486 2024-03-11 10:04:40.000000 ColabGeek-1.3.3/src/ColabGeek/shell_scripts/Install_Ruby.exp
--rw-rw-r--   0 sunym     (1000) sunym     (1000)      443 2024-03-11 10:04:40.000000 ColabGeek-1.3.3/src/ColabGeek/shell_scripts/Install_rbenv.exp
--rw-rw-r--   0 sunym     (1000) sunym     (1000)      382 2024-03-11 10:04:40.000000 ColabGeek-1.3.3/src/ColabGeek/shell_scripts/Run_Rstudio_server.sh
--rw-rw-r--   0 sunym     (1000) sunym     (1000)     1193 2024-03-11 10:04:40.000000 ColabGeek-1.3.3/src/ColabGeek/shell_scripts/Run_code_server.exp
-drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-03-11 10:07:35.912924 ColabGeek-1.3.3/src/ColabGeek.egg-info/
--rw-r--r--   0 sunym     (1000) sunym     (1000)     8758 2024-03-11 10:07:35.000000 ColabGeek-1.3.3/src/ColabGeek.egg-info/PKG-INFO
--rw-rw-r--   0 sunym     (1000) sunym     (1000)      518 2024-03-11 10:07:35.000000 ColabGeek-1.3.3/src/ColabGeek.egg-info/SOURCES.txt
--rw-rw-r--   0 sunym     (1000) sunym     (1000)        1 2024-03-11 10:07:35.000000 ColabGeek-1.3.3/src/ColabGeek.egg-info/dependency_links.txt
--rw-rw-r--   0 sunym     (1000) sunym     (1000)       10 2024-03-11 10:07:35.000000 ColabGeek-1.3.3/src/ColabGeek.egg-info/top_level.txt
+drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-04-12 03:16:51.252305 ColabGeek-1.3.4/
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)     1067 2024-04-12 03:12:54.000000 ColabGeek-1.3.4/LICENSE
+-rw-r--r--   0 sunym     (1000) sunym     (1000)     8758 2024-04-12 03:16:51.251305 ColabGeek-1.3.4/PKG-INFO
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)     8022 2024-04-12 03:12:54.000000 ColabGeek-1.3.4/README.md
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)      940 2024-04-12 03:12:54.000000 ColabGeek-1.3.4/pyproject.toml
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)       38 2024-04-12 03:16:51.252305 ColabGeek-1.3.4/setup.cfg
+drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-04-12 03:16:51.247305 ColabGeek-1.3.4/src/
+drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-04-12 03:16:51.248305 ColabGeek-1.3.4/src/ColabGeek/
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)    28805 2024-04-12 03:12:54.000000 ColabGeek-1.3.4/src/ColabGeek/ColabGeek.py
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)       25 2024-04-12 03:12:54.000000 ColabGeek-1.3.4/src/ColabGeek/__init__.py
+drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-04-12 03:16:51.251305 ColabGeek-1.3.4/src/ColabGeek/shell_scripts/
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)      817 2024-04-12 03:12:54.000000 ColabGeek-1.3.4/src/ColabGeek/shell_scripts/Install_Homebrew.exp
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)      325 2024-04-12 03:12:54.000000 ColabGeek-1.3.4/src/ColabGeek/shell_scripts/Install_Jekyll.exp
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)      621 2024-04-12 03:12:54.000000 ColabGeek-1.3.4/src/ColabGeek/shell_scripts/Install_Miniconda.sh
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)      486 2024-04-12 03:12:54.000000 ColabGeek-1.3.4/src/ColabGeek/shell_scripts/Install_Ruby.exp
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)      443 2024-04-12 03:12:54.000000 ColabGeek-1.3.4/src/ColabGeek/shell_scripts/Install_rbenv.exp
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)      382 2024-04-12 03:12:54.000000 ColabGeek-1.3.4/src/ColabGeek/shell_scripts/Run_Rstudio_server.sh
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)     1193 2024-04-12 03:12:54.000000 ColabGeek-1.3.4/src/ColabGeek/shell_scripts/Run_code_server.exp
+drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-04-12 03:16:51.251305 ColabGeek-1.3.4/src/ColabGeek.egg-info/
+-rw-r--r--   0 sunym     (1000) sunym     (1000)     8758 2024-04-12 03:16:51.000000 ColabGeek-1.3.4/src/ColabGeek.egg-info/PKG-INFO
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)      567 2024-04-12 03:16:51.000000 ColabGeek-1.3.4/src/ColabGeek.egg-info/SOURCES.txt
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)        1 2024-04-12 03:16:51.000000 ColabGeek-1.3.4/src/ColabGeek.egg-info/dependency_links.txt
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)       10 2024-04-12 03:16:51.000000 ColabGeek-1.3.4/src/ColabGeek.egg-info/top_level.txt
```

### Comparing `ColabGeek-1.3.3/LICENSE` & `ColabGeek-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ColabGeek-1.3.3/PKG-INFO` & `ColabGeek-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ColabGeek
-Version: 1.3.3
+Version: 1.3.4
 Summary: ColabGeek is designed to help run useful tools on Google Colab, including port forwarding, web IDE and so on. It is worth noting that this package is also compatible with other Ubuntu operating system servers, so try on other platforms as well.
 Author-email: Yiming Sun <yiming.sun12138@gmail.com>
 Project-URL: Homepage, https://github.com/yimingsun12138/ColabGeek
 Project-URL: Bug Tracker, https://github.com/yimingsun12138/ColabGeek/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `ColabGeek-1.3.3/README.md` & `ColabGeek-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `ColabGeek-1.3.3/pyproject.toml` & `ColabGeek-1.3.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 where = ["src"]
 
 [tool.setuptools.package-data]
 "ColabGeek.shell_scripts" = ["*"]
 
 [project]
 name = "ColabGeek"
-version = "1.3.3"
+version = "1.3.4"
 authors = [
     {name = "Yiming Sun",email = "yiming.sun12138@gmail.com"},
 ]
 description = "ColabGeek is designed to help run useful tools on Google Colab, including port forwarding, web IDE and so on. It is worth noting that this package is also compatible with other Ubuntu operating system servers, so try on other platforms as well."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `ColabGeek-1.3.3/src/ColabGeek/ColabGeek.py` & `ColabGeek-1.3.4/src/ColabGeek/ColabGeek.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,16 @@
         Install Ruby on Colab.
     Install_Jekyll(Ruby_version = None,verbose = True)
         Install and run Jekyll on Colab.
     Run_stable_diffusion_webui(path = None,port = None,verbose = True,args = None,**kwargs)
         Install and run Stable Diffusion WebUI on Colab.
     busy_session(busy = None)
         Keep the Colab session active.
+    Install_Miniconda(path = None,verbose = True)
+        Install Miniconda on Colab.
     """
     
     def __init__(self,user,password,sudo = True,port = 8787,mount_GD = False,keep_busy = True):
         """
         Initialize the ColabSession object.
 
         Initialize the ColabSession object by adding the system user, mounting Google Drive and setting temp directory.
@@ -754,14 +756,49 @@
         # while loop
         while busy:
             i = "round" + " " + str(ii)
             print(i)
             ii = ii + 1
             time.sleep(60)
 
+    # install Miniconda
+    def Install_Miniconda(self,path = None,verbose = True):
+        """
+        Install Miniconda on Colab.
+
+        Miniconda is a free and minimal installer for the conda package manager and frequently used in scientific computing.
+        This function helps to install Miniconda on Colab.
+
+        Parameters
+        ----------
+        path : str, optional
+            The directory to install Miniconda.
+        verbose : bool, optional
+            Whether to show the running logs.
+        """
+
+        # check param
+        if (path is None):
+            path = "/home/" + str(self.user)
+        else:
+            char_cmd = "sudo -u" + " " + str(self.user) + " " + "mkdir -p" + " " + str(path)
+            os.system(char_cmd)
+
+        # get shell script path
+        script_path = os.path.dirname(__file__)
+        script_path = os.path.join(script_path,'shell_scripts','Install_Miniconda.sh')
+
+        # install Miniconda
+        char_cmd = "sudo -u" + " " + str(self.user) + " " + "bash" + " " + str(script_path) + " " + str(self.user) + " " + str(path)
+        exec_logging = os.popen(char_cmd)
+        exec_logging = ''.join(exec_logging.readlines())
+        if verbose:
+            print("Install Miniconda: \n")
+            print(exec_logging)
+
 ##########################
 ## define other methods ##
 ##########################
 
 # update environment
 def update_environment(verbose = True):
     """
```

### Comparing `ColabGeek-1.3.3/src/ColabGeek/shell_scripts/Install_Homebrew.exp` & `ColabGeek-1.3.4/src/ColabGeek/shell_scripts/Install_Homebrew.exp`

 * *Files identical despite different names*

### Comparing `ColabGeek-1.3.3/src/ColabGeek/shell_scripts/Run_code_server.exp` & `ColabGeek-1.3.4/src/ColabGeek/shell_scripts/Run_code_server.exp`

 * *Files identical despite different names*

### Comparing `ColabGeek-1.3.3/src/ColabGeek.egg-info/PKG-INFO` & `ColabGeek-1.3.4/src/ColabGeek.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ColabGeek
-Version: 1.3.3
+Version: 1.3.4
 Summary: ColabGeek is designed to help run useful tools on Google Colab, including port forwarding, web IDE and so on. It is worth noting that this package is also compatible with other Ubuntu operating system servers, so try on other platforms as well.
 Author-email: Yiming Sun <yiming.sun12138@gmail.com>
 Project-URL: Homepage, https://github.com/yimingsun12138/ColabGeek
 Project-URL: Bug Tracker, https://github.com/yimingsun12138/ColabGeek/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `ColabGeek-1.3.3/src/ColabGeek.egg-info/SOURCES.txt` & `ColabGeek-1.3.4/src/ColabGeek.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,11 +5,12 @@
 src/ColabGeek/__init__.py
 src/ColabGeek.egg-info/PKG-INFO
 src/ColabGeek.egg-info/SOURCES.txt
 src/ColabGeek.egg-info/dependency_links.txt
 src/ColabGeek.egg-info/top_level.txt
 src/ColabGeek/shell_scripts/Install_Homebrew.exp
 src/ColabGeek/shell_scripts/Install_Jekyll.exp
+src/ColabGeek/shell_scripts/Install_Miniconda.sh
 src/ColabGeek/shell_scripts/Install_Ruby.exp
 src/ColabGeek/shell_scripts/Install_rbenv.exp
 src/ColabGeek/shell_scripts/Run_Rstudio_server.sh
 src/ColabGeek/shell_scripts/Run_code_server.exp
```

