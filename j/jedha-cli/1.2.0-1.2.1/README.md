# Comparing `tmp/jedha_cli-1.2.0.tar.gz` & `tmp/jedha_cli-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jedha_cli-1.2.0.tar", max compression
+gzip compressed data, was "jedha_cli-1.2.1.tar", max compression
```

## Comparing `jedha_cli-1.2.0.tar` & `jedha_cli-1.2.1.tar`

### file list

```diff
@@ -1,50 +1,55 @@
--rw-r--r--   0        0        0    35149 2024-01-25 10:09:15.321100 jedha_cli-1.2.0/LICENSE
--rw-r--r--   0        0        0     1574 2024-01-25 10:09:15.321257 jedha_cli-1.2.0/README.md
--rw-r--r--   0        0        0      687 2024-04-05 15:17:06.206387 jedha_cli-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-25 10:09:15.322437 jedha_cli-1.2.0/src/__init__.py
--rw-r--r--   0        0        0      284 2024-04-05 15:13:58.979330 jedha_cli-1.2.0/src/labs/backdoor.yaml
--rw-r--r--   0        0        0      347 2024-02-22 16:27:32.696922 jedha_cli-1.2.0/src/labs/bypass-login.yaml
--rw-r--r--   0        0        0      322 2024-04-05 15:16:44.100571 jedha_cli-1.2.0/src/labs/covering-tracks-linux.yaml
--rw-r--r--   0        0        0      675 2024-04-05 15:16:44.100708 jedha_cli-1.2.0/src/labs/covering-tracks.yaml
--rw-r--r--   0        0        0      571 2024-01-25 10:09:15.322806 jedha_cli-1.2.0/src/labs/dns_zone_transfer.yaml
--rw-r--r--   0        0        0      684 2024-02-19 14:17:57.490868 jedha_cli-1.2.0/src/labs/docker_evasion_1.yaml
--rw-r--r--   0        0        0      357 2024-02-19 14:17:57.491309 jedha_cli-1.2.0/src/labs/docker_evasion_2.yaml
--rw-r--r--   0        0        0      358 2024-02-19 14:17:57.491623 jedha_cli-1.2.0/src/labs/docker_evasion_3.yaml
--rw-r--r--   0        0        0      323 2024-02-22 16:27:32.697055 jedha_cli-1.2.0/src/labs/format_string.yaml
--rw-r--r--   0        0        0      295 2024-04-05 15:13:58.979678 jedha_cli-1.2.0/src/labs/gash.yaml
--rw-r--r--   0        0        0      318 2024-01-25 10:09:15.323286 jedha_cli-1.2.0/src/labs/hid.yaml
--rw-r--r--   0        0        0      359 2024-02-22 16:27:32.697156 jedha_cli-1.2.0/src/labs/idor.yaml
--rw-r--r--   0        0        0      356 2024-02-22 16:27:32.697260 jedha_cli-1.2.0/src/labs/insecure_design.yaml
--rw-r--r--   0        0        0      329 2024-01-25 10:44:56.612899 jedha_cli-1.2.0/src/labs/linux_privesc.yaml
--rw-r--r--   0        0        0      452 2024-04-05 15:13:58.980008 jedha_cli-1.2.0/src/labs/little_big_ctf.yaml
--rw-r--r--   0        0        0      353 2024-01-25 10:09:15.323660 jedha_cli-1.2.0/src/labs/manual_audit.yaml
--rw-r--r--   0        0        0      371 2024-03-07 14:30:23.918539 jedha_cli-1.2.0/src/labs/msf_1.yaml
--rw-r--r--   0        0        0      304 2024-02-22 16:27:32.697647 jedha_cli-1.2.0/src/labs/msf_2.yaml
--rw-r--r--   0        0        0      297 2024-04-05 15:13:58.980275 jedha_cli-1.2.0/src/labs/my_first_ctf.yaml
--rw-r--r--   0        0        0      300 2024-04-05 15:13:58.980554 jedha_cli-1.2.0/src/labs/my_second_ctf.yaml
--rw-r--r--   0        0        0      352 2024-02-22 16:27:32.697771 jedha_cli-1.2.0/src/labs/path_traversal.yaml
--rw-r--r--   0        0        0     2445 2024-03-15 13:38:48.454766 jedha_cli-1.2.0/src/labs/pentesting_network_services.yaml
--rw-r--r--   0        0        0      322 2024-04-05 15:16:44.100841 jedha_cli-1.2.0/src/labs/pivoting-introduction.yaml
--rw-r--r--   0        0        0      599 2024-04-05 15:16:44.100972 jedha_cli-1.2.0/src/labs/pivoting.yaml
--rw-r--r--   0        0        0      280 2024-04-05 15:16:44.101115 jedha_cli-1.2.0/src/labs/reverse.yaml
--rw-r--r--   0        0        0      284 2024-04-05 15:13:58.980672 jedha_cli-1.2.0/src/labs/sambacry.yaml
--rw-r--r--   0        0        0      380 2024-02-22 16:27:32.698222 jedha_cli-1.2.0/src/labs/security_misconfiguration.yaml
--rw-r--r--   0        0        0      290 2024-04-05 15:13:58.980788 jedha_cli-1.2.0/src/labs/shellshock.yaml
--rw-r--r--   0        0        0      751 2024-03-13 10:00:54.999558 jedha_cli-1.2.0/src/labs/sqli.yaml
--rw-r--r--   0        0        0      893 2024-02-22 16:27:32.698691 jedha_cli-1.2.0/src/labs/ssrf.yaml
--rw-r--r--   0        0        0      272 2024-02-22 16:27:32.699086 jedha_cli-1.2.0/src/labs/sudo_1.yaml
--rw-r--r--   0        0        0      276 2024-03-20 09:49:04.648517 jedha_cli-1.2.0/src/labs/sudo_2.yaml
--rw-r--r--   0        0        0      276 2024-01-25 10:09:15.324618 jedha_cli-1.2.0/src/labs/sudo_3.yaml
--rw-r--r--   0        0        0      272 2024-02-22 16:27:32.699334 jedha_cli-1.2.0/src/labs/suid.yaml
--rw-r--r--   0        0        0      276 2024-01-25 10:09:15.324914 jedha_cli-1.2.0/src/labs/suid_2.yaml
--rw-r--r--   0        0        0      628 2024-02-22 16:27:32.699456 jedha_cli-1.2.0/src/labs/template_injection.yaml
--rw-r--r--   0        0        0      279 2024-04-05 15:13:58.980933 jedha_cli-1.2.0/src/labs/vim_fu.yaml
--rw-r--r--   0        0        0      998 2024-04-05 15:13:58.981147 jedha_cli-1.2.0/src/labs/vuln_web_app.yaml
--rw-r--r--   0        0        0     1119 2024-02-22 16:27:32.699708 jedha_cli-1.2.0/src/labs/vulnerable_and_outdated_software.yaml
--rw-r--r--   0        0        0      290 2024-01-25 10:09:15.325298 jedha_cli-1.2.0/src/labs/wifi_wpa2_cracking.yaml
--rw-r--r--   0        0        0      352 2024-01-25 10:09:15.325420 jedha_cli-1.2.0/src/labs/windows_box.yaml
--rw-r--r--   0        0        0      320 2024-02-22 16:27:32.699823 jedha_cli-1.2.0/src/labs/xss.yaml
--rw-r--r--   0        0        0     5075 2024-04-05 15:16:44.100417 jedha_cli-1.2.0/src/labs.yaml
--rw-r--r--   0        0        0     9983 2024-04-05 15:13:58.981430 jedha_cli-1.2.0/src/main.py
--rw-r--r--   0        0        0     6363 2024-03-13 14:11:35.442529 jedha_cli-1.2.0/src/misc.py
--rw-r--r--   0        0        0     2138 1970-01-01 00:00:00.000000 jedha_cli-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-01-25 10:09:15.321100 jedha_cli-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1574 2024-01-25 10:09:15.321257 jedha_cli-1.2.1/README.md
+-rw-r--r--   0        0        0      687 2024-04-12 15:11:45.564622 jedha_cli-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-25 10:09:15.322437 jedha_cli-1.2.1/src/__init__.py
+-rw-r--r--   0        0        0      284 2024-04-05 15:13:58.979330 jedha_cli-1.2.1/src/labs/backdoor.yaml
+-rw-r--r--   0        0        0      347 2024-02-22 16:27:32.696922 jedha_cli-1.2.1/src/labs/bypass-login.yaml
+-rw-r--r--   0        0        0      322 2024-04-05 15:16:44.100571 jedha_cli-1.2.1/src/labs/covering-tracks-linux.yaml
+-rw-r--r--   0        0        0      675 2024-04-05 15:16:44.100708 jedha_cli-1.2.1/src/labs/covering-tracks.yaml
+-rw-r--r--   0        0        0      571 2024-01-25 10:09:15.322806 jedha_cli-1.2.1/src/labs/dns_zone_transfer.yaml
+-rw-r--r--   0        0        0      684 2024-02-19 14:17:57.490868 jedha_cli-1.2.1/src/labs/docker_evasion_1.yaml
+-rw-r--r--   0        0        0      357 2024-02-19 14:17:57.491309 jedha_cli-1.2.1/src/labs/docker_evasion_2.yaml
+-rw-r--r--   0        0        0      358 2024-02-19 14:17:57.491623 jedha_cli-1.2.1/src/labs/docker_evasion_3.yaml
+-rw-r--r--   0        0        0      292 2024-04-12 12:18:56.955573 jedha_cli-1.2.1/src/labs/echo_server.yaml
+-rw-r--r--   0        0        0      323 2024-02-22 16:27:32.697055 jedha_cli-1.2.1/src/labs/format_string.yaml
+-rw-r--r--   0        0        0      493 2024-04-12 12:41:35.581865 jedha_cli-1.2.1/src/labs/ftp_server.yaml
+-rw-r--r--   0        0        0      295 2024-04-05 15:13:58.979678 jedha_cli-1.2.1/src/labs/gash.yaml
+-rw-r--r--   0        0        0      318 2024-01-25 10:09:15.323286 jedha_cli-1.2.1/src/labs/hid.yaml
+-rw-r--r--   0        0        0      359 2024-02-22 16:27:32.697156 jedha_cli-1.2.1/src/labs/idor.yaml
+-rw-r--r--   0        0        0      356 2024-02-22 16:27:32.697260 jedha_cli-1.2.1/src/labs/insecure_design.yaml
+-rw-r--r--   0        0        0      329 2024-01-25 10:44:56.612899 jedha_cli-1.2.1/src/labs/linux_privesc.yaml
+-rw-r--r--   0        0        0      452 2024-04-05 15:13:58.980008 jedha_cli-1.2.1/src/labs/little_big_ctf.yaml
+-rw-r--r--   0        0        0      353 2024-01-25 10:09:15.323660 jedha_cli-1.2.1/src/labs/manual_audit.yaml
+-rw-r--r--   0        0        0      371 2024-03-07 14:30:23.918539 jedha_cli-1.2.1/src/labs/msf_1.yaml
+-rw-r--r--   0        0        0      304 2024-02-22 16:27:32.697647 jedha_cli-1.2.1/src/labs/msf_2.yaml
+-rw-r--r--   0        0        0      297 2024-04-05 15:13:58.980275 jedha_cli-1.2.1/src/labs/my_first_ctf.yaml
+-rw-r--r--   0        0        0      300 2024-04-05 15:13:58.980554 jedha_cli-1.2.1/src/labs/my_second_ctf.yaml
+-rw-r--r--   0        0        0      408 2024-04-12 12:55:06.466685 jedha_cli-1.2.1/src/labs/nfs_server.yaml
+-rw-r--r--   0        0        0      352 2024-02-22 16:27:32.697771 jedha_cli-1.2.1/src/labs/path_traversal.yaml
+-rw-r--r--   0        0        0     2445 2024-03-15 13:38:48.454766 jedha_cli-1.2.1/src/labs/pentesting_network_services.yaml
+-rw-r--r--   0        0        0      322 2024-04-05 15:16:44.100841 jedha_cli-1.2.1/src/labs/pivoting-introduction.yaml
+-rw-r--r--   0        0        0      599 2024-04-05 15:16:44.100972 jedha_cli-1.2.1/src/labs/pivoting.yaml
+-rw-r--r--   0        0        0      282 2024-04-12 12:11:07.144861 jedha_cli-1.2.1/src/labs/proxmark.yaml
+-rw-r--r--   0        0        0      280 2024-04-05 15:16:44.101115 jedha_cli-1.2.1/src/labs/reverse.yaml
+-rw-r--r--   0        0        0      284 2024-04-05 15:13:58.980672 jedha_cli-1.2.1/src/labs/sambacry.yaml
+-rw-r--r--   0        0        0      380 2024-02-22 16:27:32.698222 jedha_cli-1.2.1/src/labs/security_misconfiguration.yaml
+-rw-r--r--   0        0        0      290 2024-04-05 15:13:58.980788 jedha_cli-1.2.1/src/labs/shellshock.yaml
+-rw-r--r--   0        0        0      343 2024-04-12 12:48:27.848816 jedha_cli-1.2.1/src/labs/smb_server.yaml
+-rw-r--r--   0        0        0      751 2024-03-13 10:00:54.999558 jedha_cli-1.2.1/src/labs/sqli.yaml
+-rw-r--r--   0        0        0      893 2024-02-22 16:27:32.698691 jedha_cli-1.2.1/src/labs/ssrf.yaml
+-rw-r--r--   0        0        0      272 2024-02-22 16:27:32.699086 jedha_cli-1.2.1/src/labs/sudo_1.yaml
+-rw-r--r--   0        0        0      276 2024-03-20 09:49:04.648517 jedha_cli-1.2.1/src/labs/sudo_2.yaml
+-rw-r--r--   0        0        0      276 2024-01-25 10:09:15.324618 jedha_cli-1.2.1/src/labs/sudo_3.yaml
+-rw-r--r--   0        0        0      272 2024-02-22 16:27:32.699334 jedha_cli-1.2.1/src/labs/suid.yaml
+-rw-r--r--   0        0        0      276 2024-01-25 10:09:15.324914 jedha_cli-1.2.1/src/labs/suid_2.yaml
+-rw-r--r--   0        0        0      628 2024-02-22 16:27:32.699456 jedha_cli-1.2.1/src/labs/template_injection.yaml
+-rw-r--r--   0        0        0      279 2024-04-05 15:13:58.980933 jedha_cli-1.2.1/src/labs/vim_fu.yaml
+-rw-r--r--   0        0        0      998 2024-04-05 15:13:58.981147 jedha_cli-1.2.1/src/labs/vuln_web_app.yaml
+-rw-r--r--   0        0        0     1119 2024-02-22 16:27:32.699708 jedha_cli-1.2.1/src/labs/vulnerable_and_outdated_software.yaml
+-rw-r--r--   0        0        0      290 2024-01-25 10:09:15.325298 jedha_cli-1.2.1/src/labs/wifi_wpa2_cracking.yaml
+-rw-r--r--   0        0        0      352 2024-01-25 10:09:15.325420 jedha_cli-1.2.1/src/labs/windows_box.yaml
+-rw-r--r--   0        0        0      320 2024-02-22 16:27:32.699823 jedha_cli-1.2.1/src/labs/xss.yaml
+-rw-r--r--   0        0        0     5483 2024-04-12 12:54:45.309558 jedha_cli-1.2.1/src/labs.yaml
+-rw-r--r--   0        0        0     9983 2024-04-05 15:13:58.981430 jedha_cli-1.2.1/src/main.py
+-rw-r--r--   0        0        0     6363 2024-03-13 14:11:35.442529 jedha_cli-1.2.1/src/misc.py
+-rw-r--r--   0        0        0     2138 1970-01-01 00:00:00.000000 jedha_cli-1.2.1/PKG-INFO
```

### Comparing `jedha_cli-1.2.0/LICENSE` & `jedha_cli-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jedha_cli-1.2.0/README.md` & `jedha_cli-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `jedha_cli-1.2.0/pyproject.toml` & `jedha_cli-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jedha-cli"
-version = "1.2.0"
+version = "1.2.1"
 description = "A CLI to start cybersecurity labs and practice your skills"
 authors = ["ademenet <alain@jedha.co>"]
 readme = "README.md"
 packages = [
     { include = "src" },
 ]
```

### Comparing `jedha_cli-1.2.0/src/labs/covering-tracks.yaml` & `jedha_cli-1.2.1/src/labs/covering-tracks.yaml`

 * *Files identical despite different names*

### Comparing `jedha_cli-1.2.0/src/labs/dns_zone_transfer.yaml` & `jedha_cli-1.2.1/src/labs/dns_zone_transfer.yaml`

 * *Files identical despite different names*

### Comparing `jedha_cli-1.2.0/src/labs/docker_evasion_1.yaml` & `jedha_cli-1.2.1/src/labs/docker_evasion_1.yaml`

 * *Files identical despite different names*

### Comparing `jedha_cli-1.2.0/src/labs/pentesting_network_services.yaml` & `jedha_cli-1.2.1/src/labs/pentesting_network_services.yaml`

 * *Files identical despite different names*

### Comparing `jedha_cli-1.2.0/src/labs/pivoting.yaml` & `jedha_cli-1.2.1/src/labs/pivoting.yaml`

 * *Files identical despite different names*

### Comparing `jedha_cli-1.2.0/src/labs/sqli.yaml` & `jedha_cli-1.2.1/src/labs/sqli.yaml`

 * *Files identical despite different names*

### Comparing `jedha_cli-1.2.0/src/labs/ssrf.yaml` & `jedha_cli-1.2.1/src/labs/ssrf.yaml`

 * *Files identical despite different names*

### Comparing `jedha_cli-1.2.0/src/labs/template_injection.yaml` & `jedha_cli-1.2.1/src/labs/template_injection.yaml`

 * *Files identical despite different names*

### Comparing `jedha_cli-1.2.0/src/labs/vuln_web_app.yaml` & `jedha_cli-1.2.1/src/labs/vuln_web_app.yaml`

 * *Files identical despite different names*

### Comparing `jedha_cli-1.2.0/src/labs/vulnerable_and_outdated_software.yaml` & `jedha_cli-1.2.1/src/labs/vulnerable_and_outdated_software.yaml`

 * *Files identical despite different names*

### Comparing `jedha_cli-1.2.0/src/labs.yaml` & `jedha_cli-1.2.1/src/labs.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+- name: ftp_server
+  ip: "10.10.1.13"
+  description: What is FTP?
+- name: smb_server
+  ip: "10.10.1.14"
+  description: What is SMB?
+- name: nfs_server
+  ip: "10.10.1.15"
+  description: What is NFS?
+- name: echo_server
+  ip: "10.10.1.11"
+  description: "A simple echo server to practice with netcat!"
+- name: proxmark
+  ip: "10.10.8.2"
+  description: 'Analyze RFID! (username: "iceman", password: "nfc2022")'
 - name: msf_1
   ip: "10.10.3.12"
   description: Will you be able to get a Remote Command Execution using Metasploit?
 - name: msf_2
   ip: "10.10.3.11"
   description: Will you be able to get a Remote Command Execution using Metasploit? Bonus machine!
 - name: dns_zone_transfer
```

### Comparing `jedha_cli-1.2.0/src/main.py` & `jedha_cli-1.2.1/src/main.py`

 * *Files identical despite different names*

### Comparing `jedha_cli-1.2.0/src/misc.py` & `jedha_cli-1.2.1/src/misc.py`

 * *Files identical despite different names*

### Comparing `jedha_cli-1.2.0/PKG-INFO` & `jedha_cli-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jedha-cli
-Version: 1.2.0
+Version: 1.2.1
 Summary: A CLI to start cybersecurity labs and practice your skills
 Author: ademenet
 Author-email: alain@jedha.co
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

