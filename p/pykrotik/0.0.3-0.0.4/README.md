# Comparing `tmp/pykrotik-0.0.3.tar.gz` & `tmp/pykrotik-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykrotik-0.0.3.tar", last modified: Thu Apr 11 05:22:44 2024, max compression
+gzip compressed data, was "pykrotik-0.0.4.tar", last modified: Thu Apr 11 06:42:44 2024, max compression
```

## Comparing `pykrotik-0.0.3.tar` & `pykrotik-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 05:22:44.427713 pykrotik-0.0.3/
--rw-r--r--   0 root         (0) root         (0)      254 2024-04-11 05:22:44.426840 pykrotik-0.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      792 2024-04-10 16:25:46.000000 pykrotik-0.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 05:22:44.417094 pykrotik-0.0.3/pykrotik/
--rw-r--r--   0 root         (0) root         (0)    35349 2024-04-11 05:21:36.000000 pykrotik-0.0.3/pykrotik/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 05:22:44.425675 pykrotik-0.0.3/pykrotik.egg-info/
--rw-r--r--   0 root         (0) root         (0)      254 2024-04-11 05:22:44.000000 pykrotik-0.0.3/pykrotik.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      232 2024-04-11 05:22:44.000000 pykrotik-0.0.3/pykrotik.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 05:22:44.000000 pykrotik-0.0.3/pykrotik.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2024-04-11 05:22:44.000000 pykrotik-0.0.3/pykrotik.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-11 05:22:44.000000 pykrotik-0.0.3/pykrotik.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      335 2024-04-11 05:22:32.000000 pykrotik-0.0.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 05:22:44.427935 pykrotik-0.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 16:25:46.000000 pykrotik-0.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 05:22:44.424602 pykrotik-0.0.3/tests/
--rw-r--r--   0 root         (0) root         (0)     9887 2024-04-11 05:19:02.000000 pykrotik-0.0.3/tests/test_init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:42:44.612691 pykrotik-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)      254 2024-04-11 06:42:44.611719 pykrotik-0.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      792 2024-04-10 16:25:46.000000 pykrotik-0.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:42:44.604656 pykrotik-0.0.4/pykrotik/
+-rw-r--r--   0 root         (0) root         (0)    35708 2024-04-11 06:42:03.000000 pykrotik-0.0.4/pykrotik/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:42:44.610636 pykrotik-0.0.4/pykrotik.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      254 2024-04-11 06:42:44.000000 pykrotik-0.0.4/pykrotik.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      232 2024-04-11 06:42:44.000000 pykrotik-0.0.4/pykrotik.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 06:42:44.000000 pykrotik-0.0.4/pykrotik.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2024-04-11 06:42:44.000000 pykrotik-0.0.4/pykrotik.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-11 06:42:44.000000 pykrotik-0.0.4/pykrotik.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      335 2024-04-11 06:42:40.000000 pykrotik-0.0.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 06:42:44.613597 pykrotik-0.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 16:25:46.000000 pykrotik-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:42:44.609690 pykrotik-0.0.4/tests/
+-rw-r--r--   0 root         (0) root         (0)     9887 2024-04-11 06:42:24.000000 pykrotik-0.0.4/tests/test_init.py
```

### Comparing `pykrotik-0.0.3/README.md` & `pykrotik-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pykrotik-0.0.3/pykrotik/__init__.py` & `pykrotik-0.0.4/pykrotik/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     Ip firewall filter actions supported by routeros
     """
 
     Accept = "accept"
     AddDstToAddressList = "add-dst-to-address-list"
     AddSrcToAddressList = "add-src-to-address-list"
     Drop = "drop"
+    FasttrackConnection = "fasttrack-connection"
     Jump = "jump"
     Log = "log"
     Passthrough = "passthrough"
     Reject = "reject"
     Return = "return"
     Tarpit = "tarpit"
 
@@ -125,14 +126,24 @@
     """
     Firewall filter for a 'drop' action
     """
 
     action: Literal[IpFirewallFilterAction.Drop] = IpFirewallFilterAction.Drop
 
 
+class IpFirewallFasttrackConnectionFilter(BaseIpFirewallFilter):
+    """
+    Firewall filter for a 'fasttrack-connection' action
+    """
+
+    action: Literal[IpFirewallFilterAction.FasttrackConnection] = (
+        IpFirewallFilterAction.FasttrackConnection
+    )
+
+
 class IpFirewallJumpFilter(BaseIpFirewallFilter):
     """
     Firewall filter for a 'jump' action
     """
 
     # the target chain to jump to
     jump_target: str
@@ -176,14 +187,15 @@
 # annotated discriminating union to help with parsing ip firewall filter actions
 IpFirewallFilter = Annotated[
     Union[
         IpFirewallAcceptFilter,
         IpFirewallAddDstToAddressListFilter,
         IpFirewallAddSrcToAddressListFilter,
         IpFirewallDropFilter,
+        IpFirewallFasttrackConnectionFilter,
         IpFirewallJumpFilter,
         IpFirewallPassthroughFilter,
         IpFirewallRejectFilter,
         IpFirewallReturnFilter,
         IpFirewallTarpitFilter,
     ],
     pydantic.Discriminator("action"),
```

### Comparing `pykrotik-0.0.3/tests/test_init.py` & `pykrotik-0.0.4/tests/test_init.py`

 * *Files identical despite different names*

