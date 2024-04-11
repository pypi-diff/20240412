# Comparing `tmp/sshpyk-0.11.tar.gz` & `tmp/sshpyk-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sshpyk-0.11.tar", last modified: Thu Apr 11 22:43:13 2024, max compression
+gzip compressed data, was "sshpyk-0.9.tar", last modified: Thu Apr 11 22:23:11 2024, max compression
```

## Comparing `sshpyk-0.11.tar` & `sshpyk-0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1516 2024-04-11 22:42:54.327204 sshpyk-0.11/LICENSE
--rw-r--r--   0        0        0     8823 2024-04-11 22:42:54.327204 sshpyk-0.11/README.rst
--rw-r--r--   0        0        0      537 2024-04-11 22:42:54.327204 sshpyk-0.11/pyproject.toml
--rw-r--r--   0        0        0     3011 2024-04-11 22:42:54.327204 sshpyk-0.11/sshpyk/__init__.py
--rw-r--r--   0        0        0     4521 2024-04-11 22:42:54.327204 sshpyk-0.11/sshpyk/__main__.py
--rw-r--r--   0        0        0     1762 2024-04-11 22:42:54.327204 sshpyk-0.11/sshpyk/kernel/add.py
--rw-r--r--   0        0        0     4972 2024-04-11 22:42:54.327204 sshpyk-0.11/sshpyk/kernel/ls.py
--rw-r--r--   0        0        0     9057 1970-01-01 00:00:00.000000 sshpyk-0.11/PKG-INFO
+-rw-r--r--   0        0        0     1516 2024-04-11 22:22:50.384929 sshpyk-0.9/LICENSE
+-rw-r--r--   0        0        0     8855 2024-04-11 22:22:50.384929 sshpyk-0.9/README.rst
+-rw-r--r--   0        0        0      536 2024-04-11 22:22:50.384929 sshpyk-0.9/pyproject.toml
+-rw-r--r--   0        0        0     3011 2024-04-11 22:22:50.384929 sshpyk-0.9/sshpyk/__init__.py
+-rw-r--r--   0        0        0     4521 2024-04-11 22:22:50.384929 sshpyk-0.9/sshpyk/__main__.py
+-rw-r--r--   0        0        0     1762 2024-04-11 22:22:50.384929 sshpyk-0.9/sshpyk/kernel/add.py
+-rw-r--r--   0        0        0     4972 2024-04-11 22:22:50.384929 sshpyk-0.9/sshpyk/kernel/ls.py
+-rw-r--r--   0        0        0     9088 1970-01-01 00:00:00.000000 sshpyk-0.9/PKG-INFO
```

### Comparing `sshpyk-0.11/LICENSE` & `sshpyk-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sshpyk-0.11/README.rst` & `sshpyk-0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,37 @@
+Metadata-Version: 2.1
+Name: sshpyk
+Version: 0.9
+Summary: remote jupyter kernels via ssh tunnels
+License: BSD-3-Clause
+Author-email: Darrell Schiebel <darrell@schiebel.us>
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+
 Remote Jupyter Kernels via SSH tunnels
 ######################################
 
-The design of this pakage is based upon `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_ which
-in turn is based upon `remote_ikernel <https://bitbucket.org/tdaff/remote_ikernel>`_. This implementation shares
-a common set of command line parameters with `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_, but it was
-implemented from scratch to support Python 3.10. This package adds an :code:`ls` implementation which allows
-listing info about the available kernel specifications.
+The design of this pakage is based upon `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_ which is
+in turn based upon `remote_ikernel <https://bitbucket.org/tdaff/remote_ikernel>`_. This implementation shares
+the same command line parameters as `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_, but it was
+reimplemented from scratch to support Python 3.10. It also includes an :code:`ls` implementation which allows
+checking on the available kernel specifications.
 
 While there are modest additions to `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_, there are
-also modest subtractions. There are fewer configuration options for things like the internal name used
-by `Jupyter Client <https://jupyter-client.readthedocs.io/en/stable/#>`_ to refer to the created
-kernel.
+also modest subtractions. There are fewer configuration options for things like the name that
+`Jupyter Client <https://jupyter-client.readthedocs.io/en/stable/#>`_ uses to refer to the
+kernel. This is still based on the kernel description that the user sees, but the entire name
+is no longer completely configurable.
 
 Listing the Jupyter Kernels that are available
 **********************************************
 
-It can be difficult to know which Jupyter Kernels are available because there are multiple locations where
+It can be difficult to know which Jupyter Kernels are available because there is more than one location that
 the `Kernel Spec files <https://jupyter-client.readthedocs.io/en/latest/kernels.html#kernel-specs>`_ can be
-found. :code:`sshpyk` has an :code:`ls` option which lists the kernels that are available (even those which are
+stored. :code:`sshpyk` has an :code:`ls` option to all for seeing which kernels are available (even if they are
 **not** `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_ or :code:`sshpyk` kernels::
 
   bash$
   bash$ python -m sshpyk.kernel.ls --no-check -a
   python3                                   /Users/drs/develop/python/conda/envs/py310/share/jupyter/kernels/python3
   python3.8                                 /usr/local/share/jupyter/kernels/python3.8
   python3dbg                                /Users/drs/Library/Jupyter/kernels/python3dbg
@@ -31,20 +41,19 @@
   bash$
 
 The :code:`--no-check` (or alternatively :code:`-nc`) flag indicates that the validity of the kernel spec files
 should **not** be checked. The :code:`-a` (or :code:`--all`) flag indicates that it should show **all** kernel
 specifications rather than just the ones for `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_ or
 :code:`sshpyk` kernel specification files.
 
-If :code:`--no-check` is **not** supplied, part of listing the kernel information will include 
+If :code:`--no-check` is **not** supplied, then as part of listing the kernel information :code:`sshpyk` will
 verify that the Python executable specified in the kernel specification exist on the local and remote systems.
-This check allows the ouput to be colorized so red text indicates a problem. :code:`--local` will limit the
-check to just the local Python executable and :code:`--remote` will limit the check to only the remote Python
-executable. These options also list the local or remote Python path **instead** of the path to the kernel
-specification directory.
+:code:`--local` will limit the check to just the local Python executable and :code:`--remote` will limit the
+check to only the remote Python executable. These options also list the local or remote Python path **instead**
+of the path to the kernel specification directory.
 
 
 Command line "ls" options
 =========================
 
 The following options are available for listing the Jupyter kernel specifications:
 
@@ -105,15 +114,15 @@
   bash$
 
 Unlike the example above, here we have asked that the remote Python path be displayed
 instead of showing the kernel specificaton directory. Since we again asked that *all kernels*
 be displayed instead of only the SSH kernels, a Python path is displayed for the
 non-SSH kernels, but it is the local Python path as indicated by :code:`localhost:`.
 Because these three kernels are non-SSH kernels this is the only Python path that is
-available. However for the SSH kernels, we can see the remote Python path listed.
+available. However for the SSH kernels, we can see the remote Pyton path listed.
 These paths are prefixed with the hostname, here :code:`host06:`. We can also see
 the newly added kernel listed as :code:`ssh_host06_host06kernel`. This name is an internal
 name created from the :code:`--display-name` string which the end user will typically
 never see.
 
 Command line "add" options
 ==========================
@@ -182,7 +191,8 @@
 is on some protected network behind :code:`ssh.example.com`. When the *local* account
 runs :code:`ssh host06`, SSH will first connect as :code:`BASTION-USERNAME` on
 :code:`ssh.example.com` and then it connect to host :code:`host06` as username
 :code:`HOST06-USERNAME`.
 
 This sort of configuration will allow :code:`host06` to be allowed as a hostname
 for remote kernels.
+
```

### Comparing `sshpyk-0.11/pyproject.toml` & `sshpyk-0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     { name = "Darrell Schiebel", email = "darrell@schiebel.us" },
 ]
 dependencies = [
     "jupyter-client",
 ]
 requires-python = ">=3.8"
 readme = "README.rst"
-version = "0.11"
+version = "0.9"
 
 [project.license]
 text = "BSD-3-Clause"
 
 [tool.pdm.build]
 
 [tool.pdm.version]
```

### Comparing `sshpyk-0.11/sshpyk/__init__.py` & `sshpyk-0.9/sshpyk/__init__.py`

 * *Files identical despite different names*

### Comparing `sshpyk-0.11/sshpyk/__main__.py` & `sshpyk-0.9/sshpyk/__main__.py`

 * *Files identical despite different names*

### Comparing `sshpyk-0.11/sshpyk/kernel/add.py` & `sshpyk-0.9/sshpyk/kernel/add.py`

 * *Files identical despite different names*

### Comparing `sshpyk-0.11/sshpyk/kernel/ls.py` & `sshpyk-0.9/sshpyk/kernel/ls.py`

 * *Files identical despite different names*

### Comparing `sshpyk-0.11/PKG-INFO` & `sshpyk-0.9/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,28 @@
-Metadata-Version: 2.1
-Name: sshpyk
-Version: 0.11
-Summary: remote jupyter kernels via ssh tunnels
-License: BSD-3-Clause
-Author-email: Darrell Schiebel <darrell@schiebel.us>
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-
 Remote Jupyter Kernels via SSH tunnels
 ######################################
 
-The design of this pakage is based upon `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_ which
-in turn is based upon `remote_ikernel <https://bitbucket.org/tdaff/remote_ikernel>`_. This implementation shares
-a common set of command line parameters with `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_, but it was
-implemented from scratch to support Python 3.10. This package adds an :code:`ls` implementation which allows
-listing info about the available kernel specifications.
+The design of this pakage is based upon `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_ which is
+in turn based upon `remote_ikernel <https://bitbucket.org/tdaff/remote_ikernel>`_. This implementation shares
+the same command line parameters as `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_, but it was
+reimplemented from scratch to support Python 3.10. It also includes an :code:`ls` implementation which allows
+checking on the available kernel specifications.
 
 While there are modest additions to `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_, there are
-also modest subtractions. There are fewer configuration options for things like the internal name used
-by `Jupyter Client <https://jupyter-client.readthedocs.io/en/stable/#>`_ to refer to the created
-kernel.
+also modest subtractions. There are fewer configuration options for things like the name that
+`Jupyter Client <https://jupyter-client.readthedocs.io/en/stable/#>`_ uses to refer to the
+kernel. This is still based on the kernel description that the user sees, but the entire name
+is no longer completely configurable.
 
 Listing the Jupyter Kernels that are available
 **********************************************
 
-It can be difficult to know which Jupyter Kernels are available because there are multiple locations where
+It can be difficult to know which Jupyter Kernels are available because there is more than one location that
 the `Kernel Spec files <https://jupyter-client.readthedocs.io/en/latest/kernels.html#kernel-specs>`_ can be
-found. :code:`sshpyk` has an :code:`ls` option which lists the kernels that are available (even those which are
+stored. :code:`sshpyk` has an :code:`ls` option to all for seeing which kernels are available (even if they are
 **not** `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_ or :code:`sshpyk` kernels::
 
   bash$
   bash$ python -m sshpyk.kernel.ls --no-check -a
   python3                                   /Users/drs/develop/python/conda/envs/py310/share/jupyter/kernels/python3
   python3.8                                 /usr/local/share/jupyter/kernels/python3.8
   python3dbg                                /Users/drs/Library/Jupyter/kernels/python3dbg
@@ -40,20 +32,19 @@
   bash$
 
 The :code:`--no-check` (or alternatively :code:`-nc`) flag indicates that the validity of the kernel spec files
 should **not** be checked. The :code:`-a` (or :code:`--all`) flag indicates that it should show **all** kernel
 specifications rather than just the ones for `SSH Kernel <https://github.com/bernhard-42/ssh_ipykernel>`_ or
 :code:`sshpyk` kernel specification files.
 
-If :code:`--no-check` is **not** supplied, part of listing the kernel information will include 
+If :code:`--no-check` is **not** supplied, then as part of listing the kernel information :code:`sshpyk` will
 verify that the Python executable specified in the kernel specification exist on the local and remote systems.
-This check allows the ouput to be colorized so red text indicates a problem. :code:`--local` will limit the
-check to just the local Python executable and :code:`--remote` will limit the check to only the remote Python
-executable. These options also list the local or remote Python path **instead** of the path to the kernel
-specification directory.
+:code:`--local` will limit the check to just the local Python executable and :code:`--remote` will limit the
+check to only the remote Python executable. These options also list the local or remote Python path **instead**
+of the path to the kernel specification directory.
 
 
 Command line "ls" options
 =========================
 
 The following options are available for listing the Jupyter kernel specifications:
 
@@ -114,15 +105,15 @@
   bash$
 
 Unlike the example above, here we have asked that the remote Python path be displayed
 instead of showing the kernel specificaton directory. Since we again asked that *all kernels*
 be displayed instead of only the SSH kernels, a Python path is displayed for the
 non-SSH kernels, but it is the local Python path as indicated by :code:`localhost:`.
 Because these three kernels are non-SSH kernels this is the only Python path that is
-available. However for the SSH kernels, we can see the remote Python path listed.
+available. However for the SSH kernels, we can see the remote Pyton path listed.
 These paths are prefixed with the hostname, here :code:`host06:`. We can also see
 the newly added kernel listed as :code:`ssh_host06_host06kernel`. This name is an internal
 name created from the :code:`--display-name` string which the end user will typically
 never see.
 
 Command line "add" options
 ==========================
@@ -191,8 +182,7 @@
 is on some protected network behind :code:`ssh.example.com`. When the *local* account
 runs :code:`ssh host06`, SSH will first connect as :code:`BASTION-USERNAME` on
 :code:`ssh.example.com` and then it connect to host :code:`host06` as username
 :code:`HOST06-USERNAME`.
 
 This sort of configuration will allow :code:`host06` to be allowed as a hostname
 for remote kernels.
-
```

