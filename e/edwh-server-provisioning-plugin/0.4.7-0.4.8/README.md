# Comparing `tmp/edwh_server_provisioning_plugin-0.4.7.tar.gz` & `tmp/edwh_server_provisioning_plugin-0.4.8.tar.gz`

## Comparing `edwh_server_provisioning_plugin-0.4.7.tar` & `edwh_server_provisioning_plugin-0.4.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    23482 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.4.7/.dcignore
--rw-r--r--   0        0        0    18229 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.4.7/CHANGELOG.md
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.4.7/old_documentation_in_dutch.md
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.4.7/src/edwh_server_provisioning_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.4.7/src/edwh_server_provisioning_plugin/__init__.py
--rw-r--r--   0        0        0    48534 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.4.7/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.4.7/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.4.7/LICENSE.txt
--rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.4.7/readme.md
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0    23482 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.4.8/.dcignore
+-rw-r--r--   0        0        0    18433 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.4.8/CHANGELOG.md
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.4.8/old_documentation_in_dutch.md
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.4.8/src/edwh_server_provisioning_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.4.8/src/edwh_server_provisioning_plugin/__init__.py
+-rw-r--r--   0        0        0    48987 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.4.8/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.4.8/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.4.8/LICENSE.txt
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.4.8/readme.md
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.4.8/PKG-INFO
```

### Comparing `edwh_server_provisioning_plugin-0.4.7/.dcignore` & `edwh_server_provisioning_plugin-0.4.8/.dcignore`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.4.7/CHANGELOG.md` & `edwh_server_provisioning_plugin-0.4.8/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.4.8 (2024-04-12)
+
+### Fix
+
+* Use require_sudo to improve password prompting ([`91694a4`](https://github.com/educationwarehouse/server_provisioning/commit/91694a464135a90fc5b93fa57051ab07e6ec6025))
+
 ## v0.4.7 (2024-03-15)
 ### Fix
 * Deprecated '_prepare_generic_server' because it had no reason to exist ([`6d94f77`](https://github.com/educationwarehouse/server_provisioning/commit/6d94f7752cbe5248148e366d363483f9baec8501))
 
 ## v0.4.6 (2024-02-08)
 ### Fix
 * Ubuntu verise Check gebeurt nu alleen bij server setup, niet bij repo install ([`05f943e`](https://github.com/educationwarehouse/server_provisioning/commit/05f943e93f6c20b919e9a67f286ffc7f0fa2db31))
```

### Comparing `edwh_server_provisioning_plugin-0.4.7/old_documentation_in_dutch.md` & `edwh_server_provisioning_plugin-0.4.8/old_documentation_in_dutch.md`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.4.7/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py` & `edwh_server_provisioning_plugin-0.4.8/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import warnings
 from abc import ABC
 from datetime import datetime
 from io import StringIO
 from pathlib import Path
 from textwrap import dedent
 
+import edwh.tasks
 import yaml
 from fabric import Connection, Result, task
 from tabulate import tabulate
 from termcolor import cprint
 from yaml.loader import SafeLoader
 
 DOT_XONSH = """
@@ -406,16 +407,15 @@
             cls.evaluate(c)
             print(cls.__name__, "succesful")
 
         cls.tested = True
 
     @classmethod
     @abc.abstractmethod
-    def evaluate(cls, c: Connection):
-        ...
+    def evaluate(cls, c: Connection): ...
 
 
 class Xonsh(TestOnce):
     @classmethod
     def evaluate(cls, c: Connection):
         if c.run("env | grep XONSH", hide=True, warn=True).stdout.strip():
             # xonsh is incompatbible met `cat filename` en dan de .ok uitlezen.
@@ -462,23 +462,23 @@
     list the files from large to smallest
     :param head: amount of files to be listed by the large file search
     """
     print("searching for large files...(this can take a minute)")
     c.run(f"du -aBM 2>/dev/null | sort -nr | head -n {head}")
 
 
-@task
+@task(pre=[edwh.tasks.require_sudo])
 def apt_install(c, packages):
     if isinstance(packages, str):
         packages = [packages]
 
     failsafe(lambda: c.sudo("apt install -y " + " ".join(packages)))
 
 
-@task
+@task(pre=[edwh.tasks.require_sudo])
 def apt_upgrade(c, dist=False):
     failsafe(lambda: c.sudo("apt update -y"))
     if dist:
         failsafe(lambda: c.sudo("apt dist-upgrade -y"))
     else:
         failsafe(lambda: c.sudo("apt upgrade -y"))
 
@@ -497,29 +497,29 @@
             "software-properties-common",
             "curl",
             "gnupg",
         ],
     )
 
 
-@task
+@task(pre=[edwh.tasks.require_sudo])
 def add_apt_repository(c, gpg_url, repo_url):
     c.run(f"curl -fsSL {gpg_url} | sudo apt-key add -")
     c.sudo(f'add-apt-repository "deb [arch=amd64] {repo_url} $(lsb_release -cs) stable"')
     apt_upgrade(c)
 
 
-@task
+@task(pre=[edwh.tasks.require_sudo])
 def add_user_to_group(c, group):
     current_groups = c.run("groups").stdout
     if group not in current_groups:
         failsafe(lambda: c.sudo(f"gpasswd -a `whoami` {group} "))
 
 
-@task
+@task(pre=[edwh.tasks.require_sudo])
 def install_docker(c):
     if execution_fails(c, "docker compose version"):
         c.sudo("install -m 0755 -d /etc/apt/keyrings")
         c.sudo(
             "sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg"
         )
         c.sudo("chmod a+r /etc/apt/keyrings/docker.gpg")
@@ -541,15 +541,15 @@
 
 
 @task
 def show_user_groups(c):
     print(c.run("groups").stdout)
 
 
-@task
+@task(pre=[edwh.tasks.require_sudo])
 def install_python(c):
     if execution_fails(c, "python3 --version"):
         apt_install(c, ["python3"])
     if execution_fails(c, "pip3 -V"):
         apt_install(c, ["python3-pip"])
     # wonderbaarlijk genoeg schijnt virtualenv nu ook al geinstalleerd te zijn.
     # maar alsnog:
@@ -650,18 +650,18 @@
     # respond_to_security=Responder(r'Are you sure you want to continue connecting \(yes/no/\[fingerprint\]\)\?.*','yes\n')
 
     # check als machine correcte git ssh verbinding kan maken
     # fingerprint
     if (
         "Permission denied (publickey)"
         in c.run(
-        "ssh-key -R github.com && ssh -tt -o StrictHostKeyChecking=accept-new git@github.com",
-        hide=True,
-        warn=True,
-    ).stderr
+            "ssh-key -R github.com && ssh -tt -o StrictHostKeyChecking=accept-new git@github.com",
+            hide=True,
+            warn=True,
+        ).stderr
     ):
         raise Exception(
             "github key klopt niet, CHECK ALS GITHUB_KNOWN_HOSTS KEY KLOPT IN DE server_provisioning_plugin.py"
         )
 
     # test if the repo exists:
     if "fatal:" in c.run(f"cd {target_directory or git_repo}; git status", warn=True, hide=True).stderr:
@@ -672,15 +672,15 @@
         c.run(f"cd {target_directory}; git checkout {branch}")
 
 
 class SecurityException(Exception):
     pass
 
 
-@task()
+@task(pre=[edwh.tasks.require_sudo])
 def assert_root_disabled_on_ssh(c):
     print(f"Validating SSHd config file disallows root on {c.host}.")
     sshd_config_parts = (
         c.sudo("grep -i PermitRootLogin /etc/ssh/sshd_config", warn=True, hide=True).stdout.strip().split("\n")
     )
     if sshd_config_parts:
         enabled_linecount = sum(1 for line in sshd_config_parts if not line.startswith("#"))
@@ -697,15 +697,15 @@
     if len(authorized_keys) > 1:
         raise SecurityException("There should only be one key in /root/.ssh/authorized_keys")
     if "command=" not in authorized_keys[0].lower():
         raise SecurityException("Missing a blocking command section in /root/.ssh/authorized_keys")
     print("Good, root seems unable to login.")
 
 
-@task()
+@task(pre=[edwh.tasks.require_sudo])
 def assert_passwords_disabled_on_ssh(c):
     print(f"Validating SSHd config file disallows passwords on {c.host}.")
     sshd_config_parts = (
         c.sudo("grep -i PasswordAuthentication /etc/ssh/sshd_config", hide=True, warn=True).stdout.strip().split("\n")
     )
     if sshd_config_parts:
         for line in sshd_config_parts:
@@ -719,15 +719,15 @@
                     print("From /etc/ssh/sshd_config:", "\n".join(sshd_config_parts))
                     raise SecurityException(
                         "PasswordAuthentication found enabled in /etc/ssh/sshd_config on target host. Disable manually. "
                     )
     print("Good, password authentication seems disabled")
 
 
-@task()
+@task(pre=[edwh.tasks.require_sudo])
 def set_root_password(c, password=None, overwrite=False):
     """Sets remote root password to given password, or asks the user for one."""
     shadow = [line.strip().split(":") for line in c.sudo("cat /etc/shadow", hide=True).stdout.strip().split("\n")]
     for username, password_hash, *_ in shadow:
         if username == "root":
             if len(password_hash) > 1:
                 # Some password exists for root
@@ -749,15 +749,15 @@
     c.sudo(
         "passwd root",
         hide=False,
         in_stream=StringIO(password + "\n" + password + "\n"),
     )
 
 
-@task()
+@task(pre=[edwh.tasks.require_sudo])
 def enable_firewall(c, portmapping):
     """
     open ports with ufw, and docker-ufw.
     portmapping is a ';' seperated list of ':' seperated service_name:port tuples
     if no service_name is given, it will be applied just to UFW
     if a service_name is given, it will be aplied to ufw-docker as well.
 
@@ -799,15 +799,15 @@
                 f"git clone https://github.com/chaifeng/ufw-docker.git; cd ufw-docker; ./ufw-docker install; systemctl restart ufw"
             )
         )
         for service, port in service_ports.items():
             failsafe(lambda: c.run(f""))
 
 
-@task()
+@task(pre=[edwh.tasks.require_sudo])
 def get_open_ports(c):
     print("Checking", c.host)
     c.sudo("ufw status verbose")
 
 
 @task()
 def install_edwh(c):
@@ -877,16 +877,18 @@
 
         print("-------------------------------------------------------------------------------------", file=sys.stderr)
         print("--------------------------------------- Done! ---------------------------------------", file=sys.stderr)
         print("-------------------------------------------------------------------------------------", file=sys.stderr)
 
 
 def _prepare_generic_server(c: Connection, silent: bool):
-    warnings.warn("'_prepare_generic_server' is deprecated. Please use 'prepare_generic_server' instead.",
-                  category=DeprecationWarning)
+    warnings.warn(
+        "'_prepare_generic_server' is deprecated. Please use 'prepare_generic_server' instead.",
+        category=DeprecationWarning,
+    )
     return prepare_generic_server(c, silent)
 
 
 @task
 def install_joplin(c):
     c: Connection = c
     c.run("mkdir services", warn=True)
@@ -1055,15 +1057,15 @@
             "WithSecure linux server Subscription Key (https://elements.f-secure.com/apps/psb/c556915/subscription) [blank=ignore]: "
         )
         if subscription_key.strip():
             install_antivirus(c, subscription_key=subscription_key)
             print("/!\ Denk eraan, hier moet nog een profiel aan gekoppeld worden in de withsecure website! ")
 
 
-@task
+@task(pre=[edwh.tasks.require_sudo])
 def install_antivirus(c, subscription_key):
     c: Connection
     subscription_key: str
     c.run(
         "curl https://download.sp.f-secure.com/linuxsecurity64/f-secure-linuxsecurity.deb -o f-secure-linuxsecurity.deb"
     )
     c.sudo("dpkg -i f-secure-linuxsecurity.deb")
@@ -1126,27 +1128,27 @@
             try:
                 time.sleep(3)
             except KeyboardInterrupt:
                 print("closing connection.")
                 break
 
 
-@task
+@task(pre=[edwh.tasks.require_sudo])
 def require_npx(c):
     # npm installs npx
     c.sudo("npm --version > /dev/null || sudo apt install npm -y")
 
 
 def background_run(c, command):
     # command = 'nohup %s &> /dev/null &' % command
     command = "nohup '%s' >& /dev/null < /dev/null &" % command
     c.run(command, pty=False)
 
 
-@task()
+@task(pre=[edwh.tasks.require_sudo])
 def kill_ungit(c):
     c.sudo("ps aux | grep ungit | cut -d' ' -f5 | xargs kill", hide=True, warn=True)
 
 
 @task(pre=[require_npx])
 def ungit(c, omgeving="ontwikkelstraat", port=8111):
     """
```

### Comparing `edwh_server_provisioning_plugin-0.4.7/LICENSE.txt` & `edwh_server_provisioning_plugin-0.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.4.7/pyproject.toml` & `edwh_server_provisioning_plugin-0.4.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.4.7/readme.md` & `edwh_server_provisioning_plugin-0.4.8/readme.md`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.4.7/PKG-INFO` & `edwh_server_provisioning_plugin-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: edwh-server-provisioning-plugin
-Version: 0.4.7
+Version: 0.4.8
 Summary: Fabric-based remote server management plugin for `edwh`
 Project-URL: Documentation, https://github.com/educationwarehouse/server_provisioning#readme
 Project-URL: Issues, https://github.com/educationwarehouse/server_provisioning/issues
 Project-URL: Source, https://github.com/educationwarehouse/server_provisioning
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

