# Comparing `tmp/edwh_sshfs_plugin-0.1.5.tar.gz` & `tmp/edwh_sshfs_plugin-0.2.0.tar.gz`

## Comparing `edwh_sshfs_plugin-0.1.5.tar` & `edwh_sshfs_plugin-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     5517 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.5/CHANGELOG.md
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.5/src/edwh_sshfs_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.5/src/edwh_sshfs_plugin/__init__.py
--rw-r--r--   0        0        0     8067 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.5/src/edwh_sshfs_plugin/fabfile.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.5/tests/conftest.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.5/tests/test_sshfs.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.5/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.5/LICENSE.txt
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.5/README.md
--rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     5803 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.2.0/src/edwh_sshfs_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.2.0/src/edwh_sshfs_plugin/__init__.py
+-rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.2.0/src/edwh_sshfs_plugin/fabfile.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.2.0/tests/test_sshfs.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.2.0/README.md
+-rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.2.0/PKG-INFO
```

### Comparing `edwh_sshfs_plugin-0.1.5/CHANGELOG.md` & `edwh_sshfs_plugin-0.2.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.2.0 (2024-04-12)
+
+### Feature
+
+* Add `ensure-sshfs` subcommand to make sure sshfs is installed when required + use new `require_sudo` for better sudo prompting ([`3a45117`](https://github.com/educationwarehouse/edwh-sshfs-plugin/commit/3a451176a7cffaa6af51b052436a34644c79d831))
+
 ## v0.1.5 (2023-09-19)
 ### Performance
 * Slighly sped up import for plugin by using everything from invoke instead of invoke + fabric (fab can still be used!) ([`a931f7a`](https://github.com/educationwarehouse/edwh-sshfs-plugin/commit/a931f7acdee27905077c2c54ea64626980a11ec7))
 
 ## v0.1.4 (2023-09-19)
 ### Performance
 * Removed anyio import by default because it seems to be unused and slowed down plugin performance ([`864a958`](https://github.com/educationwarehouse/edwh-sshfs-plugin/commit/864a958daea419f53479014bf8956dabfa678823))
```

### Comparing `edwh_sshfs_plugin-0.1.5/src/edwh_sshfs_plugin/fabfile.py` & `edwh_sshfs_plugin-0.2.0/src/edwh_sshfs_plugin/fabfile.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,34 @@
+import asyncio
+import getpass
 import os
 import socket
-import getpass
-import warnings
 
-from invoke import task, context
-from plumbum import BG
-from plumbum.commands.processes import CommandNotFound
+import edwh.tasks
+from invoke import Context, context, task
+from plumbum import BG, local
 
-# import anyio
-import asyncio
 
-try:
-    from plumbum.cmd import ssh, sshfs
-except (ImportError, CommandNotFound):
-    warnings.warn(
-        "edwh sshfs plugin is installed but sshfs is missing. "
-        "Please check README.md#installation on how to fix this! "
-        "The commands in this plugin will NOT work unless this is fixed."
-    )
+def get_remote_available_ports(c: Context):
+    """
+    Retrieves the list of available ports on the remote server.
+
+    Args:
+        c: The connection object used to communicate with the remote server.
+
+    Returns:
+        list: A list of available port numbers on the remote server.
+    """
 
-STOP_RUNNING = False
+    port_cmd = c.run("nc -z -v 127.0.0.1 2220-2300 2>&1 | grep refused | cut -d ' ' -f 6", hide=True)
+    # return available_port
+    return port_cmd.stdout.split("\n")
 
 
-def get_available_port(c):
+def get_available_port(c: Context):
     """
     Retrieves an available port that is both locally and remotely accessible.
 
     Args:
         c: The connection object used to communicate with the remote server.
 
     Returns:
@@ -37,32 +39,16 @@
 
     # check if a local port is in a remote port
     for local_port in get_local_available_port():
         if local_port in remote_ports:
             return local_port
 
 
-def get_remote_available_ports(c):
-    """
-    Retrieves the list of available ports on the remote server.
-
-    Args:
-        c: The connection object used to communicate with the remote server.
-
-    Returns:
-        list: A list of available port numbers on the remote server.
-    """
-
-    port_cmd = c.run("nc -z -v 127.0.0.1 2220-2300 2>&1 | grep refused | cut -d ' ' -f 6", hide=True)
-    # return available_port
-    return port_cmd.stdout.split("\n")
-
-
 # check if there are any available ports
-def get_local_available_port(start_port=2222):
+def get_local_available_port(start_port: int = 2222):
     """
     Retrieves a list of available ports on the local machine.
 
     Args:
         start_port (optional): The starting port number to search for available ports.
             Defaults to 2222.
 
@@ -73,81 +59,100 @@
 
     # check all ports between start_port and 60000
     for port in range(start_port, 2300):
         s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         s.settimeout(0.5)
         try:
             s.connect(("127.0.0.1", port))
-            s.close()
             continue
-        except:
-            s.close()
+        except Exception:
             available_ports.append(str(port))
+        finally:
+            s.close()
 
     return available_ports
 
 
-def getuid():
-    return os.getuid()
+@task()
+def setup(c: Context):
+    """
+    Installs the necessary packages for SSHFS.
+    """
+    if edwh.tasks.require_sudo(c):
+        c.sudo("apt update")
+        c.sudo("apt install -y openssh-client openssh-server sshfs")
+        c.sudo("systemctl enable ssh")
+        c.sudo("ufw allow ssh")
 
 
-def getgid():
-    return os.getgid()
+@task()
+def ensure_sshfs(c: Context):
+    """
+    Ensures that SSHFS is installed on the local machine.
+    """
+    if not c.run("which sshfs", hide=True, warn=True).ok:
+        setup(c)
 
 
-@task(help={'dir': "The directory path to be unmounted."})
-def unmount_dir(c, dir):
+@task(help={'folder': "The directory path to be unmounted."}, pre=[ensure_sshfs])
+def unmount_dir(c, folder):
     """
     Unmounts a directory on the server.
 
     Returns:
         None
     """
 
-    umount_server_dir = f"umount {dir}"
+    umount_server_dir = f"umount {folder}"
     print(f"running {umount_server_dir}")
     if not c.run(umount_server_dir, warn=True).ok:
         print("cannot unmount because following processes are still running and using the mount")
-        c.run(f"lsof -n {dir} 2>/dev/null")
+        c.run(f"lsof -n {folder} 2>/dev/null")
         pids = c.run("lsof -t -n /home/ubuntu/testing 2>/dev/null", hide=True).stdout.strip().split('\n')
-        print(f'Terminate with: kill {" ".join(pids)}; sleep 2; umount {dir}')
+        print(f'Terminate with: kill {" ".join(pids)}; sleep 2; umount {folder}')
     else:
-        print("successfully exited :)")
+        print("suFccessfully exited :)")
 
 
 @task(
     help={
         'workstation-dir': "The directory path on the local machine to mount the server directory.",
         'server-dir': "The directory path on the remote server to be mounted.",
         'queue': "An optional queue object used for synchronization. Defaults to None, optional",
-    }
+    },
+    pre=[ensure_sshfs],
 )
-def remote_mount(c, workstation_dir, server_dir, queue=None):
+def remote_mount(
+    c,
+    workstation_dir,
+    server_dir,
+    queue=None,
+):
     """
     The remote_mount function is an asynchronous Python task that allows you to mount a remote directory
     on your local machine using SSHFS (SSH Filesystem). It establishes a secure connection to a remote server,
     forwards a port, and mounts the remote directory on the local machine.
 
     Returns:
         None
     """
     if not hasattr(c, "host"):
-        print("please give up a host using -H")
+        print("please provide a host using -H")
         exit(255)
 
     # get an available port that is usable on local and remote so we can setup a connection with the ports
     port = get_available_port(c)
-    ssh_cmd = ssh["-A", f"-R {port}:127.0.0.1:22", f"{c.user}@{c.host}"]
+    ssh_cmd = local['ssh']["-A", f"-R {port}:127.0.0.1:22", f"{c.user}@{c.host}"]
     sshfs_cmd = ssh_cmd[
         "sshfs",
         "-f",
         f"-p {port}",
         "-o allow_root,default_permissions",
         "-o StrictHostKeyChecking=no,reconnect,ServerAliveInterval=3,ServerAliveCountMax=3,"
-        f"uid={getuid()},gid={getgid()}",
+        f"uid={os.getuid()},gid={os.getgid()}",
         f"{getpass.getuser()}@127.0.0.1:{workstation_dir}",
         f"{server_dir}",
     ]
 
     if not queue:
         print(f"starting sshfs with(started when nothing happens): {str(sshfs_cmd)}")
     try:
@@ -157,34 +162,37 @@
 
 
 @task(
     help={
         'workstation-dir': 'The directory path on the local machine to be mounted.',
         'server-dir': 'The directory path on the remote server to mount the workstation directory.',
         'queue': 'An optional queue object used for synchronization. Defaults to None, optional',
-    }
+    },
+    pre=[ensure_sshfs],
 )
 def local_mount(c, workstation_dir, server_dir, queue=None):
     """
     The local_mount function is a Python task that enables the mounting of a remote directory on a local workstation
     using SSHFS (SSH Filesystem). It establishes a secure connection to a remote server and mounts a specified
     directory from the server onto a local directory on the workstation.
 
     Returns:
         None
     """
     # os.popen(f"lsof -n {workstation_dir} 2>/dev/null")
     if not hasattr(c, "host"):
-        print("please give up a host using -H")
+        print("please provide a host using -H")
         exit(255)
+
     # TODO: remove mount on exit
-    sshfs_cmd = sshfs[
+    sshfs_cmd = local['sshfs'][
         "-f",
         "-o",
-        "allow_root,default_permissions,umask=000,StrictHostKeyChecking=no,reconnect," f"uid={getuid()},gid={getgid()}",
+        "allow_root,default_permissions,umask=000,StrictHostKeyChecking=no,reconnect,"
+        f"uid={os.getuid()},gid={os.getgid()}",
         f"{c.user}@{c.host}:{server_dir}",
         workstation_dir,
     ]
 
     if not queue:
         print("running sshfs...")
 
@@ -200,21 +208,22 @@
 
 
 async def async_local_mount(c, workstation_dir, server_dir, event=None):
     """
     async version of local_mount
     """
     if not hasattr(c, "host"):
-        print("please give up a host using -H")
+        print("please provide a host using -H")
         exit(255)
 
-    sshfs_cmd = sshfs[
+    sshfs_cmd = local['sshfs'][
         "-f",
         "-o",
-        "allow_root,default_permissions,umask=000,StrictHostKeyChecking=no,reconnect," f"uid={getuid()},gid={getgid()}",
+        "allow_root,default_permissions,umask=000,StrictHostKeyChecking=no,reconnect,"
+        f"uid={os.getuid()},gid={os.getgid()}",
         f"{c.user}@{c.host}:{server_dir}",
         workstation_dir,
     ]
 
     if not event:
         print("running sshfs...")
 
@@ -231,27 +240,27 @@
 
 
 async def async_remote_mount(c, workstation_dir, server_dir, event=None):
     """
     async version of remote_mount
     """
     if not hasattr(c, "host"):
-        print("please give up a host using -H")
+        print("please provide a host using -H")
         exit(255)
 
     # get an available port that is usable on local and remote so we can setup a connection with the ports
     port = get_available_port(c)
-    ssh_cmd = ssh["-A", f"-R {port}:127.0.0.1:22", f"{c.user}@{c.host}"]
+    ssh_cmd = local['ssh']["-A", f"-R {port}:127.0.0.1:22", f"{c.user}@{c.host}"]
     sshfs_cmd = ssh_cmd[
         "sshfs",
         "-f",
         f"-p {port}",
         "-o allow_root,default_permissions",
         "-o StrictHostKeyChecking=no,reconnect,ServerAliveInterval=3,ServerAliveCountMax=3,"
-        f"uid={getuid()},gid={getgid()}",
+        f"uid={os.getuid()},gid={os.getgid()}",
         f"{getpass.getuser()}@127.0.0.1:{workstation_dir}",
         f"{server_dir}",
     ]
 
     if not event:
         print(f"starting sshfs with(started when nothing happens): {str(sshfs_cmd)}")
     try:
```

### Comparing `edwh_sshfs_plugin-0.1.5/tests/test_sshfs.py` & `edwh_sshfs_plugin-0.2.0/tests/test_sshfs.py`

 * *Files identical despite different names*

### Comparing `edwh_sshfs_plugin-0.1.5/LICENSE.txt` & `edwh_sshfs_plugin-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_sshfs_plugin-0.1.5/README.md` & `edwh_sshfs_plugin-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `edwh_sshfs_plugin-0.1.5/pyproject.toml` & `edwh_sshfs_plugin-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,23 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = ['fabric', "plumbum>=1.8.1"]
+dependencies = [
+    "edwh",
+    "plumbum>=1.8.1",
+]
 
 [project.optional-dependencies]
 dev = [
     "hatch",
-    # "python-semantic-release",
+    "python-semantic-release<8",
     "black",
     "pytest",
 ]
 
 async = [
     "anyio",
     "trio"
```

### Comparing `edwh_sshfs_plugin-0.1.5/PKG-INFO` & `edwh_sshfs_plugin-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: edwh-sshfs-plugin
-Version: 0.1.5
+Version: 0.2.0
 Summary: sshfs project with a plugin to be discovered from the edwh package
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-sshfs-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-sshfs-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-sshfs-plugin
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -12,23 +12,24 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
-Requires-Dist: fabric
+Requires-Dist: edwh
 Requires-Dist: plumbum>=1.8.1
 Provides-Extra: async
 Requires-Dist: anyio; extra == 'async'
 Requires-Dist: trio; extra == 'async'
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: python-semantic-release<8; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # edwh-sshfs-plugin
 
 [![PyPI - Version](https://img.shields.io/pypi/v/edwh-sshfs-plugin.svg)](https://pypi.org/project/edwh-sshfs-plugin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edwh-sshfs-plugin.svg)](https://pypi.org/project/edwh-sshfs-plugin)
```

