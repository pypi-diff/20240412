# Comparing `tmp/lbrlabs_pulumi_tailscalebastion-0.6.0.tar.gz` & `tmp/lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lbrlabs_pulumi_tailscalebastion-0.6.0.tar", last modified: Tue Mar 26 00:52:35 2024, max compression
+gzip compressed data, was "dist/lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188.tar", last modified: Fri Apr 12 18:11:04 2024, max compression
```

## Comparing `lbrlabs_pulumi_tailscalebastion-0.6.0.tar` & `lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 00:52:35.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-03-26 00:52:35.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-03-26 00:52:34.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 00:52:35.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion/
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-03-26 00:52:34.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8090 2024-03-26 00:52:34.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 00:52:35.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-26 00:52:34.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15956 2024-03-26 00:52:34.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion/aws/bastion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 00:52:35.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-26 00:52:34.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11715 2024-03-26 00:52:34.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion/azure/bastion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 00:52:35.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-26 00:52:34.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-03-26 00:52:34.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion/kubernetes/bastion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-03-26 00:52:34.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-26 00:52:34.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 00:52:34.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 00:52:35.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-03-26 00:52:35.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-26 00:52:35.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 00:52:35.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 00:52:35.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-26 00:52:35.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-26 00:52:35.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 00:52:35.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-03-26 00:52:34.000000 lbrlabs_pulumi_tailscalebastion-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion/
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8090 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15956 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion/aws/bastion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion/azure/bastion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion/kubernetes/bastion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-12 18:11:04.000000 lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/setup.py
```

### Comparing `lbrlabs_pulumi_tailscalebastion-0.6.0/PKG-INFO` & `lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lbrlabs_pulumi_tailscalebastion
-Version: 0.6.0
+Name: lbrlabs-pulumi-tailscalebastion
+Version: 0.6.1a1712945188
 Summary: A Pulumi package for creating a tailscale bastion in AWS.
 Home-page: UNKNOWN
 License: UNKNOWN
 Project-URL: Repository, https://github.com/lbrlabs/pulumi-tailscale-bastion
 Description: # Pulumi Tailscale Bastion
         
         This repo provides a [multi-language](https://www.pulumi.com/blog/pulumiup-pulumi-packages-multi-language-components/) component that creates a [Tailscale](https://tailscale.com/) [Subnet Router](https://tailscale.com/kb/1019/subnets/) in your chosen cloud provider
```

### Comparing `lbrlabs_pulumi_tailscalebastion-0.6.0/README.md` & `lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/README.md`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion/__init__.py` & `lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion/__init__.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion/_utilities.py` & `lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion/_utilities.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion/aws/bastion.py` & `lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion/aws/bastion.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion/azure/bastion.py` & `lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion/azure/bastion.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,25 +17,27 @@
                  high_availability: Optional[pulumi.Input[bool]] = None,
                  location: pulumi.Input[str],
                  resource_group_name: pulumi.Input[str],
                  route: pulumi.Input[str],
                  subnet_id: pulumi.Input[str],
                  tailscale_tags: pulumi.Input[Sequence[pulumi.Input[str]]],
                  enable_ssh: Optional[pulumi.Input[bool]] = None,
-                 instance_sku: Optional[pulumi.Input[str]] = None):
+                 instance_sku: Optional[pulumi.Input[str]] = None,
+                 public: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Bastion resource.
         :param pulumi.Input[bool] high_availability: Whether the bastion should be highly available.
         :param pulumi.Input[str] location: The Azure region you're using.
         :param pulumi.Input[str] resource_group_name: The Azure resource group to create the bastion in.
         :param pulumi.Input[str] route: The route you'd like to advertise via tailscale.
         :param pulumi.Input[str] subnet_id: The subnet Ids to launch instances in.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tailscale_tags: The tags to apply to the tailnet device andauth key. This tag should be added to your oauth key and ACL.
         :param pulumi.Input[bool] enable_ssh: Whether to enable SSH access to the bastion.
         :param pulumi.Input[str] instance_sku: The Azure instance SKU to use for the bastion.
+        :param pulumi.Input[bool] public: Whether the bastion should have a public IP.
         """
         if high_availability is None:
             high_availability = False
         pulumi.set(__self__, "high_availability", high_availability)
         pulumi.set(__self__, "location", location)
         pulumi.set(__self__, "resource_group_name", resource_group_name)
         pulumi.set(__self__, "route", route)
@@ -43,14 +45,18 @@
         pulumi.set(__self__, "tailscale_tags", tailscale_tags)
         if enable_ssh is None:
             enable_ssh = True
         if enable_ssh is not None:
             pulumi.set(__self__, "enable_ssh", enable_ssh)
         if instance_sku is not None:
             pulumi.set(__self__, "instance_sku", instance_sku)
+        if public is None:
+            public = False
+        if public is not None:
+            pulumi.set(__self__, "public", public)
 
     @property
     @pulumi.getter(name="highAvailability")
     def high_availability(self) -> pulumi.Input[bool]:
         """
         Whether the bastion should be highly available.
         """
@@ -140,37 +146,51 @@
         """
         return pulumi.get(self, "instance_sku")
 
     @instance_sku.setter
     def instance_sku(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "instance_sku", value)
 
+    @property
+    @pulumi.getter
+    def public(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether the bastion should have a public IP.
+        """
+        return pulumi.get(self, "public")
+
+    @public.setter
+    def public(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "public", value)
+
 
 class Bastion(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  enable_ssh: Optional[pulumi.Input[bool]] = None,
                  high_availability: Optional[pulumi.Input[bool]] = None,
                  instance_sku: Optional[pulumi.Input[str]] = None,
                  location: Optional[pulumi.Input[str]] = None,
+                 public: Optional[pulumi.Input[bool]] = None,
                  resource_group_name: Optional[pulumi.Input[str]] = None,
                  route: Optional[pulumi.Input[str]] = None,
                  subnet_id: Optional[pulumi.Input[str]] = None,
                  tailscale_tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Create a Bastion resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] enable_ssh: Whether to enable SSH access to the bastion.
         :param pulumi.Input[bool] high_availability: Whether the bastion should be highly available.
         :param pulumi.Input[str] instance_sku: The Azure instance SKU to use for the bastion.
         :param pulumi.Input[str] location: The Azure region you're using.
+        :param pulumi.Input[bool] public: Whether the bastion should have a public IP.
         :param pulumi.Input[str] resource_group_name: The Azure resource group to create the bastion in.
         :param pulumi.Input[str] route: The route you'd like to advertise via tailscale.
         :param pulumi.Input[str] subnet_id: The subnet Ids to launch instances in.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tailscale_tags: The tags to apply to the tailnet device andauth key. This tag should be added to your oauth key and ACL.
         """
         ...
     @overload
@@ -195,14 +215,15 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  enable_ssh: Optional[pulumi.Input[bool]] = None,
                  high_availability: Optional[pulumi.Input[bool]] = None,
                  instance_sku: Optional[pulumi.Input[str]] = None,
                  location: Optional[pulumi.Input[str]] = None,
+                 public: Optional[pulumi.Input[bool]] = None,
                  resource_group_name: Optional[pulumi.Input[str]] = None,
                  route: Optional[pulumi.Input[str]] = None,
                  subnet_id: Optional[pulumi.Input[str]] = None,
                  tailscale_tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
@@ -222,14 +243,17 @@
             if high_availability is None and not opts.urn:
                 raise TypeError("Missing required property 'high_availability'")
             __props__.__dict__["high_availability"] = high_availability
             __props__.__dict__["instance_sku"] = instance_sku
             if location is None and not opts.urn:
                 raise TypeError("Missing required property 'location'")
             __props__.__dict__["location"] = location
+            if public is None:
+                public = False
+            __props__.__dict__["public"] = public
             if resource_group_name is None and not opts.urn:
                 raise TypeError("Missing required property 'resource_group_name'")
             __props__.__dict__["resource_group_name"] = resource_group_name
             if route is None and not opts.urn:
                 raise TypeError("Missing required property 'route'")
             __props__.__dict__["route"] = route
             if subnet_id is None and not opts.urn:
```

### Comparing `lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion/kubernetes/bastion.py` & `lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion/kubernetes/bastion.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion/provider.py` & `lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion/provider.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion.egg-info/PKG-INFO` & `lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lbrlabs-pulumi-tailscalebastion
-Version: 0.6.0
+Name: lbrlabs_pulumi_tailscalebastion
+Version: 0.6.1a1712945188
 Summary: A Pulumi package for creating a tailscale bastion in AWS.
 Home-page: UNKNOWN
 License: UNKNOWN
 Project-URL: Repository, https://github.com/lbrlabs/pulumi-tailscale-bastion
 Description: # Pulumi Tailscale Bastion
         
         This repo provides a [multi-language](https://www.pulumi.com/blog/pulumiup-pulumi-packages-multi-language-components/) component that creates a [Tailscale](https://tailscale.com/) [Subnet Router](https://tailscale.com/kb/1019/subnets/) in your chosen cloud provider
```

### Comparing `lbrlabs_pulumi_tailscalebastion-0.6.0/lbrlabs_pulumi_tailscalebastion.egg-info/SOURCES.txt` & `lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/lbrlabs_pulumi_tailscalebastion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_tailscalebastion-0.6.0/setup.py` & `lbrlabs_pulumi_tailscalebastion-0.6.1a1712945188/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.6.0"
+VERSION = "0.6.1a1712945188"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "tailscale-bastion Pulumi Package - Development Version"
```

