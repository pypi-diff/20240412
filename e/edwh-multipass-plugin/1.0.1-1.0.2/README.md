# Comparing `tmp/edwh_multipass_plugin-1.0.1.tar.gz` & `tmp/edwh_multipass_plugin-1.0.2.tar.gz`

## Comparing `edwh_multipass_plugin-1.0.1.tar` & `edwh_multipass_plugin-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.1/CHANGELOG.md
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.1/src/edwh_multipass_plugin/__about__.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.1/src/edwh_multipass_plugin/__init__.py
--rw-r--r--   0        0        0     6883 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.1/src/edwh_multipass_plugin/tasks.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.1/.gitignore
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.1/README.md
--rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.2/src/edwh_multipass_plugin/__about__.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.2/src/edwh_multipass_plugin/__init__.py
+-rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.2/src/edwh_multipass_plugin/tasks.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.2/README.md
+-rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.2/PKG-INFO
```

### Comparing `edwh_multipass_plugin-1.0.1/src/edwh_multipass_plugin/tasks.py` & `edwh_multipass_plugin-1.0.2/src/edwh_multipass_plugin/tasks.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,34 @@
 import json
 import pathlib
 import re
 import sys
 
+import edwh
 import invoke
+import yaml
 from invoke import task
 
 
-@task(name="install")
+@task(name="install", pre=[edwh.tasks.require_sudo])
 def install_multipass(c):
     if not c.run("multipass --version", warn=True, hide=True).ok:
         print(" [ ] Multipass not found. installing...")
         c.sudo("snap install multipass")
         print(" [x] Multipass installed")
     else:
         print(" [x] Multipass already installed")
 
 
 def generate_key(c, comment: str, filename: str):
     c.run(f'ssh-keygen -t ed25519 -C "{comment}" -f {filename} -N ""')
 
 
-@task(name="fix-host", aliases=["fix-dns"], iterable=["hostname"])
-def fix_hosts_for_multipass_machine(c, machine_name, hostname=[]):
-    try:
-        import yaml
-    except ModuleNotFoundError:
-        # Installeer pyyaml, maar doe dat wel met de juiste pip
-        # omdat we nooit weten welke pip dat is, gaan we er maar vanuit
-        # dat pip als executable "in de buurt" staat van "invoke",
-        # wat het script is dat dit uitvoert. Dus met `which invoke` vinden
-        # we het volledige pad naar invoke, en van daaruit hebben we vermoedelijk
-        # de juiste pip te pakken. Of het nou een virtualenv van de gebruiker is, van pipx
-        # of geinstalleerd met --user of zelfs `pip install invoke` als root...
-        print("Missing pip, installing...")
-        invoke_path = c.run("which invoke", hide=True).stdout.strip()
-        pip_path = invoke_path.replace("/invoke", "/pip")
-        print(f"running: {pip_path} install pyyaml")
-        c.run(f"{pip_path} install pyyaml")
-        import yaml
+@task(name="fix-host", aliases=["fix-dns"], iterable=["hostname"], pre=[edwh.tasks.require_sudo])
+def fix_hosts_for_multipass_machine(c, machine_name, hostname=()):
     if not machine_name:
         print("Machine name required. Use -m or --machine-name", file=sys.stderr)
     output = c.run("multipass list --format yaml", hide=True).stdout.strip()
     machines = yaml.load(output, yaml.SafeLoader)
     if machine_name not in machines:
         print(
             f"'{machine_name}' not found. Choose one of: {', '.join(machines.keys())}",
@@ -63,68 +49,61 @@
     hostnames = list(hostname)
     # register the hostname
     hostnames.append(machine_name)
     # only unique values
     hostnames = list(set(hostnames))
     with open("/etc/hosts", "r") as hosts_handle:
         host_lines = hosts_handle.read().split("\n")
-        found = any(
-            name
-            for name in hostnames
-            if name in " ".join([line.split("#")[0] for line in host_lines])
-        )
+        found = any(name for name in hostnames if name in " ".join([line.split("#")[0] for line in host_lines]))
         if found:
             print("Updating hosts file")
             if len(hostname) > 1:
-                print(
-                    "You have entered hostnames, that argument is incompatible with the upgrade. "
-                )
+                print("You have entered hostnames, that argument is incompatible with the upgrade. ")
                 print("Edit /etc/hosts manually to register aliases manually")
             new_hosts = []
             for line in host_lines:
                 if any(True for name in hostnames if name in line):
                     # line found, replace ip adress: convert tabs to spaces
                     line = line.replace("\t", "    ")
                     # create a new line with the ipv, whitespace, and the remainder of the original
                     # line (everything after the first space), replacing multiple spaces with one.
-                    new_hosts.append(
-                        re.sub(
-                            r"  +", " ", f'{first_address}      {line.split(" ",1)[1]}'
-                        )
-                    )
+                    new_hosts.append(re.sub(r"  +", " ", f'{first_address}      {line.split(" ", 1)[1]}'))
                     print(new_hosts[-1])
                 else:
                     new_hosts.append(line)
             c: invoke.Context
             overwrite_hosts_command = (
                 """python3 -c "import sys \nwith open('/etc/hosts','w') as h: h.write(sys.stdin.read().strip())" <<EOFEOFEOF\n"""
                 + "\n".join(new_hosts)
             )
             overwrite_hosts_command += "\nEOFEOFEOF"
             c.sudo("ls >> /dev/null")  # force a sudo to ask for password
             c.sudo(overwrite_hosts_command)
         else:
             print("Appending to hosts file")
             c.sudo("ls >> /dev/null")  # force a sudo to ask for password
-            line_to_append = re.sub(
-                r"  +", " ", f"{first_address}  {' '.join(hostnames)}"
-            )
+            line_to_append = re.sub(r"  +", " ", f"{first_address}  {' '.join(hostnames)}")
             print(line_to_append)
             # simpelweg overschrijven via een echo of cat >> /etc/hosts mag niet. dus dan maar via een python script.
-            c.sudo(
-                f'''python3 -c "with open('/etc/hosts','a') as h: h.write('{line_to_append}')"'''
-            )
+            c.sudo(f'''python3 -c "with open('/etc/hosts','a') as h: h.write('{line_to_append}')"''')
+
+
+@task(name="list")
+def list_machines(c, quiet=False):
+    output = c.run("multipass list --format json", hide=True).stdout
+    if quiet:
+        return json.loads(output)["list"]
+    else:
+        print(output)
 
 
 @task(pre=[install_multipass], name="prepare")
 def prepare_multipass(c, machine_name):
     print(" ... Searching for vms")
-    machines = json.loads(c.run("multipass list --format json", hide=True).stdout)[
-        "list"
-    ]
+    machines = list_machines(c, quiet=True)
     # convert to lookup by name
     machines = {m["name"]: m for m in machines}
     if machine_name not in machines:
         raise KeyError(
             f'Machine name "{machine_name}" not found in multipass. Available names: {", ".join(list(machines.keys()))}'
         )
     machine = machines[machine_name]
@@ -153,11 +132,10 @@
         c.run(
             f'echo "echo {pub_key} >> .ssh/authorized_keys; exit" | multipass shell {machine_name}',
             hide=True,
         )
         print(f" [x] installed multipass keyfile on {machine_name}")
     edwh_cmd = pathlib.Path(sys.argv[0]).name
     print(f"Execute {edwh_cmd} with:")
-    fab_commands = "|".join(c.run(f"{edwh_cmd} --complete",hide=True).stdout.strip().split("\n"))
+    fab_commands = "|".join(c.run(f"{edwh_cmd} --complete", hide=True).stdout.strip().split("\n"))
     print(f"  {edwh_cmd} -eH ubuntu@{ip} [{fab_commands}]")
     print(f'  {edwh_cmd} -eH ubuntu@{ip} -- echo "or some other arbitrary bash command"')
-
```

### Comparing `edwh_multipass_plugin-1.0.1/LICENSE.txt` & `edwh_multipass_plugin-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_multipass_plugin-1.0.1/README.md` & `edwh_multipass_plugin-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `edwh_multipass_plugin-1.0.1/pyproject.toml` & `edwh_multipass_plugin-1.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,16 @@
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  'invoke'
+  "edwh",
+  "pyyaml",
 ]
 
 [project.entry-points."edwh.tasks"]
 mp = "edwh_multipass_plugin.tasks"
 
 
 [project.urls]
@@ -51,23 +52,22 @@
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
 
 [[tool.hatch.envs.all.matrix]]
-python = ["3.11"]
+python = ["3.10", "3.11"]
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
   "black>=23.1.0",
   "mypy>=1.0.0",
   "ruff>=0.0.243",
-  'pip',
 ]
 [tool.hatch.envs.lint.scripts]
 typing = "mypy --install-types --non-interactive {args:src/edwh_multipass_plugin tests}"
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
 ]
@@ -157,14 +157,16 @@
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
 
 [tool.semantic_release]
-version_variable = "src/edwh_multipass_plugin/__about__.py:__version__"
 branch = "main"
+version_variable = "src/edwh_multipass_plugin/__about__.py:__version__"
 change_log = "CHANGELOG.md"
 upload_to_repository = false
 upload_to_release = false
-build_command = "hatch build -c"
+build_command = "hatch build"
 
+parser_angular_minor_types = "feat,minor"
+parser_angular_patch_types = "fix,perf,refactor,build,chore,patch"
```

### Comparing `edwh_multipass_plugin-1.0.1/PKG-INFO` & `edwh_multipass_plugin-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: edwh-multipass-plugin
-Version: 1.0.1
+Version: 1.0.2
 Summary: An `edwh`plugin to work with multipass instances for local development.
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-multipass-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-multipass-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-multipass-plugin
 Author-email: Remco <remco@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -12,15 +12,16 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
-Requires-Dist: invoke
+Requires-Dist: edwh
+Requires-Dist: pyyaml
 Description-Content-Type: text/markdown
 
 # edwh-multipass-plugin
 
 [![PyPI - Version](https://img.shields.io/pypi/v/edwh-multipass-plugin.svg)](https://pypi.org/project/edwh-multipass-plugin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edwh-multipass-plugin.svg)](https://pypi.org/project/edwh-multipass-plugin)
```

