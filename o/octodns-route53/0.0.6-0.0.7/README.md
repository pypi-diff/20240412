# Comparing `tmp/octodns-route53-0.0.6.tar.gz` & `tmp/octodns-route53-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octodns-route53-0.0.6.tar", last modified: Thu Oct 19 18:43:46 2023, max compression
+gzip compressed data, was "octodns-route53-0.0.7.tar", last modified: Thu Apr 11 23:50:56 2024, max compression
```

## Comparing `octodns-route53-0.0.6.tar` & `octodns-route53-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-10-19 18:43:46.640041 octodns-route53-0.0.6/
--rw-r--r--   0 ross       (501) staff       (20)     1129 2023-10-19 01:55:56.000000 octodns-route53-0.0.6/LICENSE
--rw-r--r--   0 ross       (501) staff       (20)     7630 2023-10-19 18:43:46.638832 octodns-route53-0.0.6/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)     6629 2023-10-19 01:55:56.000000 octodns-route53-0.0.6/README.md
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-10-19 18:43:46.631234 octodns-route53-0.0.6/octodns_route53/
--rw-r--r--   0 ross       (501) staff       (20)      272 2023-10-19 18:30:33.000000 octodns-route53-0.0.6/octodns_route53/__init__.py
--rw-r--r--   0 ross       (501) staff       (20)     2780 2023-10-19 01:55:56.000000 octodns-route53-0.0.6/octodns_route53/auth.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-10-19 18:43:46.632871 octodns-route53-0.0.6/octodns_route53/processor/
--rw-r--r--   0 ross       (501) staff       (20)      818 2023-10-19 01:55:56.000000 octodns-route53-0.0.6/octodns_route53/processor/__init__.py
--rw-r--r--   0 ross       (501) staff       (20)    70030 2023-10-19 01:55:56.000000 octodns-route53-0.0.6/octodns_route53/provider.py
--rw-r--r--   0 ross       (501) staff       (20)     3718 2023-10-19 01:55:56.000000 octodns-route53-0.0.6/octodns_route53/record.py
--rw-r--r--   0 ross       (501) staff       (20)     9348 2023-10-19 01:55:56.000000 octodns-route53-0.0.6/octodns_route53/source.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-10-19 18:43:46.632645 octodns-route53-0.0.6/octodns_route53.egg-info/
--rw-r--r--   0 ross       (501) staff       (20)     7630 2023-10-19 18:43:46.000000 octodns-route53-0.0.6/octodns_route53.egg-info/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)      510 2023-10-19 18:43:46.000000 octodns-route53-0.0.6/octodns_route53.egg-info/SOURCES.txt
--rw-r--r--   0 ross       (501) staff       (20)        1 2023-10-19 18:43:46.000000 octodns-route53-0.0.6/octodns_route53.egg-info/dependency_links.txt
--rw-r--r--   0 ross       (501) staff       (20)      241 2023-10-19 18:43:46.000000 octodns-route53-0.0.6/octodns_route53.egg-info/requires.txt
--rw-r--r--   0 ross       (501) staff       (20)       16 2023-10-19 18:43:46.000000 octodns-route53-0.0.6/octodns_route53.egg-info/top_level.txt
--rw-r--r--   0 ross       (501) staff       (20)      308 2023-10-19 01:55:56.000000 octodns-route53-0.0.6/pyproject.toml
--rw-r--r--   0 ross       (501) staff       (20)       38 2023-10-19 18:43:46.640292 octodns-route53-0.0.6/setup.cfg
--rw-r--r--   0 ross       (501) staff       (20)     2118 2023-10-19 01:55:56.000000 octodns-route53-0.0.6/setup.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-10-19 18:43:46.634372 octodns-route53-0.0.6/tests/
--rw-r--r--   0 ross       (501) staff       (20)   152756 2023-10-19 01:55:56.000000 octodns-route53-0.0.6/tests/test_octodns_provider_route53.py
--rw-r--r--   0 ross       (501) staff       (20)     9045 2023-10-19 01:55:56.000000 octodns-route53-0.0.6/tests/test_octodns_source_ec2.py
--rw-r--r--   0 ross       (501) staff       (20)     5500 2023-10-19 01:55:56.000000 octodns-route53-0.0.6/tests/test_octodns_source_elb.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-11 23:50:56.890936 octodns-route53-0.0.7/
+-rw-r--r--   0 ross       (501) staff       (20)     1129 2023-10-19 01:55:56.000000 octodns-route53-0.0.7/LICENSE
+-rw-r--r--   0 ross       (501) staff       (20)     7966 2024-04-11 23:50:56.889830 octodns-route53-0.0.7/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)     6965 2024-03-20 22:06:14.000000 octodns-route53-0.0.7/README.md
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-11 23:50:56.874954 octodns-route53-0.0.7/octodns_route53/
+-rw-r--r--   0 ross       (501) staff       (20)      349 2024-04-11 23:50:51.000000 octodns-route53-0.0.7/octodns_route53/__init__.py
+-rw-r--r--   0 ross       (501) staff       (20)     2782 2024-04-11 23:45:58.000000 octodns-route53-0.0.7/octodns_route53/auth.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-11 23:50:56.880365 octodns-route53-0.0.7/octodns_route53/processor/
+-rw-r--r--   0 ross       (501) staff       (20)      818 2023-10-19 01:55:56.000000 octodns-route53-0.0.7/octodns_route53/processor/__init__.py
+-rw-r--r--   0 ross       (501) staff       (20)    70924 2024-03-20 22:06:14.000000 octodns-route53-0.0.7/octodns_route53/provider.py
+-rw-r--r--   0 ross       (501) staff       (20)     3718 2023-10-19 01:55:56.000000 octodns-route53-0.0.7/octodns_route53/record.py
+-rw-r--r--   0 ross       (501) staff       (20)     9910 2024-03-20 22:06:14.000000 octodns-route53-0.0.7/octodns_route53/source.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-11 23:50:56.886716 octodns-route53-0.0.7/octodns_route53.egg-info/
+-rw-r--r--   0 ross       (501) staff       (20)     7966 2024-04-11 23:50:56.000000 octodns-route53-0.0.7/octodns_route53.egg-info/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)      510 2024-04-11 23:50:56.000000 octodns-route53-0.0.7/octodns_route53.egg-info/SOURCES.txt
+-rw-r--r--   0 ross       (501) staff       (20)        1 2024-04-11 23:50:56.000000 octodns-route53-0.0.7/octodns_route53.egg-info/dependency_links.txt
+-rw-r--r--   0 ross       (501) staff       (20)      241 2024-04-11 23:50:56.000000 octodns-route53-0.0.7/octodns_route53.egg-info/requires.txt
+-rw-r--r--   0 ross       (501) staff       (20)       16 2024-04-11 23:50:56.000000 octodns-route53-0.0.7/octodns_route53.egg-info/top_level.txt
+-rw-r--r--   0 ross       (501) staff       (20)     1340 2023-11-29 21:55:05.000000 octodns-route53-0.0.7/pyproject.toml
+-rw-r--r--   0 ross       (501) staff       (20)       38 2024-04-11 23:50:56.891133 octodns-route53-0.0.7/setup.cfg
+-rwxr-xr-x   0 ross       (501) staff       (20)     1692 2024-03-21 02:15:55.000000 octodns-route53-0.0.7/setup.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-11 23:50:56.886043 octodns-route53-0.0.7/tests/
+-rw-r--r--   0 ross       (501) staff       (20)   153510 2024-04-11 23:45:58.000000 octodns-route53-0.0.7/tests/test_octodns_provider_route53.py
+-rw-r--r--   0 ross       (501) staff       (20)    10812 2024-03-20 22:06:14.000000 octodns-route53-0.0.7/tests/test_octodns_source_ec2.py
+-rw-r--r--   0 ross       (501) staff       (20)     5833 2024-03-20 22:06:14.000000 octodns-route53-0.0.7/tests/test_octodns_source_elb.py
```

### Comparing `octodns-route53-0.0.6/LICENSE` & `octodns-route53-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `octodns-route53-0.0.6/PKG-INFO` & `octodns-route53-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octodns-route53
-Version: 0.0.6
+Version: 0.0.7
 Summary:  Route53Provider provider for octoDNS
 Home-page: https://github.com/octodns/octodns-route53
 Author: Ross McFarland
 Author-email: rwmcfa1@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 Requires-Dist: boto3>=1.20.26
 Requires-Dist: octodns>=0.9.18
 Requires-Dist: pycountry-convert>=0.7.2
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-network; extra == "dev"
-Requires-Dist: black<24.0.0,>=23.1.0; extra == "dev"
+Requires-Dist: black<25.0.0,>=24.3.0; extra == "dev"
 Requires-Dist: build>=0.7.0; extra == "dev"
 Requires-Dist: isort>=5.11.5; extra == "dev"
 Requires-Dist: pyflakes>=2.2.0; extra == "dev"
 Requires-Dist: readme_renderer[md]>=26.0; extra == "dev"
 Requires-Dist: twine>=3.4.2; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
@@ -89,22 +89,24 @@
     # auth options are the same as Route53Provider
     access_key_id: env/AWS_ACCESS_KEY_ID
     secret_access_key: env/AWS_SECRET_ACCESS_KEY
     # The region in which to look for EC2 instances, required.
     region: us-east-1
     # Prefix for tag keys containing fqdn(s)
     #tag_prefix: octodns
+    # String to append to all names and tag values
+    #append_to_names: mydomain.com.
     #ttl: 3600
 ```
 
 In general the account used will need read permissions on EC2 instances.
 
 Records are driven off of the tags attached to the EC2 instances. The "Name" tag and any tags starting with `tag_prefix` are considered.
 
-The value of the tag should be one or more fqdns separated by a `/` character.
+The value of the tag should be one or more fqdns separated by a `/` character. You can append a string to the name and all tag values with `append_to_names`.
 
 When a zone is being populated any fqdns matching the zone name will result in records. When the instance has a private IPv4 address an A record will be created. When the instance has an IPv6 address a AAAA record will be created.
 
 When the zone is a sub-zone of in-addr.arpa. PTR records will be created for private IPv4 addresses that match the zone. The value(s) will be the fqdn(s) associated with that private IPv4 address.
 
 When the zone is a sub-zone of ip6.arpa. PTR records will be created for IPv6 addresses that match the zone. The value(s) will be the fqdn(s) associated with that IPv6 address.
 
@@ -117,22 +119,24 @@
     # auth options are the same as Route53Provider
     access_key_id: env/AWS_ACCESS_KEY_ID
     secret_access_key: env/AWS_SECRET_ACCESS_KEY
     # The region in which to look for ELB instances, required.
     region: us-east-1
     # Prefix for tag keys containing fqdn(s)
     #tag_prefix: octodns
+    # String to append to all names and tag values
+    #append_to_names: mydomain.com.
     #ttl: 3600
 ```
 
 In general the account used will need read permissions on ELB instances and tags.
 
 Records are driven off of the ELB name and the tags attached to the ELB instances. Any tag with `tag_prefix` is considered.
 
-The value of the tag should be one or more fqdns separated by a `/` character.
+The value of the tag should be one or more fqdns separated by a `/` character. You can append a string to the name and all tag values with `append_to_names`.
 
 When a zone is being populated any fqdns matching the zone name will result in records CNAME records with the target value being the DNSName of the ELB instance.
 
 #### Example Tags for EC2/ELB
 
 ```yaml
 # This will result in an ALIAS record for example.com. -> DNSName
@@ -169,15 +173,15 @@
     ...
 ```
 
 ### Support Information
 
 #### Records
 
-A, AAAA, CAA, CNAME, MX, NAPTR, NS, PTR, SPF, SRV, TXT
+A, AAAA, CAA, CNAME, DS, MX, NAPTR, NS, PTR, SPF, SRV, TXT
 
 #### Root NS Records
 
 Route53Provider supports full root NS record management.
 
 #### Dynamic
```

### Comparing `octodns-route53-0.0.6/README.md` & `octodns-route53-0.0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -60,22 +60,24 @@
     # auth options are the same as Route53Provider
     access_key_id: env/AWS_ACCESS_KEY_ID
     secret_access_key: env/AWS_SECRET_ACCESS_KEY
     # The region in which to look for EC2 instances, required.
     region: us-east-1
     # Prefix for tag keys containing fqdn(s)
     #tag_prefix: octodns
+    # String to append to all names and tag values
+    #append_to_names: mydomain.com.
     #ttl: 3600
 ```
 
 In general the account used will need read permissions on EC2 instances.
 
 Records are driven off of the tags attached to the EC2 instances. The "Name" tag and any tags starting with `tag_prefix` are considered.
 
-The value of the tag should be one or more fqdns separated by a `/` character.
+The value of the tag should be one or more fqdns separated by a `/` character. You can append a string to the name and all tag values with `append_to_names`.
 
 When a zone is being populated any fqdns matching the zone name will result in records. When the instance has a private IPv4 address an A record will be created. When the instance has an IPv6 address a AAAA record will be created.
 
 When the zone is a sub-zone of in-addr.arpa. PTR records will be created for private IPv4 addresses that match the zone. The value(s) will be the fqdn(s) associated with that private IPv4 address.
 
 When the zone is a sub-zone of ip6.arpa. PTR records will be created for IPv6 addresses that match the zone. The value(s) will be the fqdn(s) associated with that IPv6 address.
 
@@ -88,22 +90,24 @@
     # auth options are the same as Route53Provider
     access_key_id: env/AWS_ACCESS_KEY_ID
     secret_access_key: env/AWS_SECRET_ACCESS_KEY
     # The region in which to look for ELB instances, required.
     region: us-east-1
     # Prefix for tag keys containing fqdn(s)
     #tag_prefix: octodns
+    # String to append to all names and tag values
+    #append_to_names: mydomain.com.
     #ttl: 3600
 ```
 
 In general the account used will need read permissions on ELB instances and tags.
 
 Records are driven off of the ELB name and the tags attached to the ELB instances. Any tag with `tag_prefix` is considered.
 
-The value of the tag should be one or more fqdns separated by a `/` character.
+The value of the tag should be one or more fqdns separated by a `/` character. You can append a string to the name and all tag values with `append_to_names`.
 
 When a zone is being populated any fqdns matching the zone name will result in records CNAME records with the target value being the DNSName of the ELB instance.
 
 #### Example Tags for EC2/ELB
 
 ```yaml
 # This will result in an ALIAS record for example.com. -> DNSName
@@ -140,15 +144,15 @@
     ...
 ```
 
 ### Support Information
 
 #### Records
 
-A, AAAA, CAA, CNAME, MX, NAPTR, NS, PTR, SPF, SRV, TXT
+A, AAAA, CAA, CNAME, DS, MX, NAPTR, NS, PTR, SPF, SRV, TXT
 
 #### Root NS Records
 
 Route53Provider supports full root NS record management.
 
 #### Dynamic
```

### Comparing `octodns-route53-0.0.6/octodns_route53/auth.py` & `octodns-route53-0.0.7/octodns_route53/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             )
 
             # and get new auth info for that role assumption, replacing the
             # stuff that was passed in and continue on to get the requested
             # client with the new auth
             access_key_id = credentials['Credentials']['AccessKeyId']
             secret_access_key = credentials['Credentials']['SecretAccessKey']
-            session_token = credentials['Credentials']['Expiration']
+            session_token = credentials['Credentials']['SessionToken']
 
         use_fallback_auth = (
             access_key_id is None
             and secret_access_key is None
             and session_token is None
         )
         if use_fallback_auth:
```

### Comparing `octodns-route53-0.0.6/octodns_route53/processor/__init__.py` & `octodns-route53-0.0.7/octodns_route53/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `octodns-route53-0.0.6/octodns_route53/provider.py` & `octodns-route53-0.0.7/octodns_route53/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,17 +308,23 @@
 
     _values_for_SPF = _values_for_quoted
     _values_for_TXT = _values_for_quoted
 
     def _value_for_SRV(self, value, record):
         return f'{value.priority} {value.weight} {value.port} {value.target}'
 
+    def _value_for_DS(self, value, record):
+        return f'{value.key_tag} {value.algorithm} {value.digest_type} {value.digest}'
+
     def _values_for_SRV(self, record):
         return [self._value_for_SRV(v, record) for v in record.values]
 
+    def _values_for_DS(self, record):
+        return [self._value_for_DS(v, record) for v in record.values]
+
 
 class _Route53Alias(_Route53Record):
     def __init__(self, provider, hosted_zone_id, record, value, creating):
         super().__init__(provider, record, creating)
         self.hosted_zone_id = hosted_zone_id
         self.fqdn = record.fqdn
         name = value.name
@@ -748,14 +754,15 @@
     SUPPORTS_ROOT_NS = True
     SUPPORTS = set(
         (
             'A',
             'AAAA',
             'CAA',
             'CNAME',
+            'DS',
             'MX',
             'NAPTR',
             'NS',
             'PTR',
             'SPF',
             'SRV',
             'TXT',
@@ -995,14 +1002,35 @@
                 }
             )
         return {
             'type': rrset['Type'],
             'values': values,
             'ttl': int(rrset['TTL']),
         }
+
+    def _data_for_DS(self, rrset):
+        values = []
+        for rr in rrset['ResourceRecords']:
+            # digest may contain whitespace
+            key_tag, algorithm, digest_type, digest = rr['Value'].split(
+                maxsplit=3
+            )
+            values.append(
+                {
+                    'key_tag': key_tag,
+                    'algorithm': algorithm,
+                    'digest_type': digest_type,
+                    'digest': digest,
+                }
+            )
+        return {
+            'type': rrset['Type'],
+            'values': values,
+            'ttl': int(rrset['TTL']),
+        }
 
     def _load_records(self, zone_id):
         if zone_id not in self._r53_rrsets:
             self.log.debug('_load_records: zone_id=%s loading', zone_id)
             rrsets = []
             more = True
             start = {}
```

### Comparing `octodns-route53-0.0.6/octodns_route53/record.py` & `octodns-route53-0.0.7/octodns_route53/record.py`

 * *Files identical despite different names*

### Comparing `octodns-route53-0.0.6/octodns_route53/source.py` & `octodns-route53-0.0.7/octodns_route53/source.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,28 +23,31 @@
         access_key_id=None,
         secret_access_key=None,
         session_token=None,
         role_arn=None,
         client_max_attempts=None,
         ttl=3600,
         tag_prefix='octodns',
+        append_to_names="",
         *args,
         **kwargs,
     ):
         self.log = getLogger(f'Ec2Source[{id}]')
         self.log.info(
-            '__init__: id=%s, region=%s, access_key_id=%s, ttl=%d, tag_prefix=%s',
+            '__init__: id=%s, region=%s, access_key_id=%s, ttl=%d, tag_prefix=%s, append_to_names=%s',
             id,
             region,
             access_key_id,
             ttl,
             tag_prefix,
+            append_to_names,
         )
         self.ttl = ttl
         self.tag_prefix = tag_prefix
+        self.append_to_names = append_to_names
 
         super().__init__(id, *args, **kwargs)
 
         self._conn = self.client(
             service_name='ec2',
             access_key_id=access_key_id,
             secret_access_key=secret_access_key,
@@ -65,17 +68,20 @@
                 for instance in reservation['Instances']:
                     # process tags
                     fqdns = []
                     for tag in instance.get('Tags', []):
                         key = tag['Key']
                         val = tag['Value']
                         if key == 'Name':
-                            fqdns.append(val)
+                            fqdns.append(val + self.append_to_names)
                         elif key.startswith(self.tag_prefix):
-                            fqdns.extend(val.split('/'))
+                            fqdns.extend(
+                                fqdn + self.append_to_names
+                                for fqdn in val.split('/')
+                            )
 
                     fqdns = [f'{i}.' if i[-1] != '.' else i for i in fqdns]
                     instances[instance['InstanceId']] = {
                         'private_v4': instance.get('PrivateIpAddress'),
                         'v6': instance.get('Ipv6Address'),
                         'fqdns': fqdns,
                     }
@@ -195,28 +201,31 @@
         access_key_id=None,
         secret_access_key=None,
         session_token=None,
         role_arn=None,
         client_max_attempts=None,
         ttl=3600,
         tag_prefix='octodns',
+        append_to_names="",
         *args,
         **kwargs,
     ):
         self.log = getLogger(f'ElbSource[{id}]')
         self.log.info(
-            '__init__: id=%s, region=%s, access_key_id=%s, ttl=%d, tag_prefix=%s',
+            '__init__: id=%s, region=%s, access_key_id=%s, ttl=%d, tag_prefix=%s, append_to_names=%s',
             id,
             region,
             access_key_id,
             ttl,
             tag_prefix,
+            append_to_names,
         )
         self.ttl = ttl
         self.tag_prefix = tag_prefix
+        self.append_to_names = append_to_names
 
         super().__init__(id, *args, **kwargs)
 
         self._conn = self.client(
             service_name='elbv2',
             access_key_id=access_key_id,
             secret_access_key=secret_access_key,
@@ -234,29 +243,32 @@
             # build the list of load balancers
             resp = self._conn.describe_load_balancers()
             lbs = {}
             for lb in resp['LoadBalancers']:
                 arn = lb['LoadBalancerArn']
                 lbs[arn] = {
                     'dns_name': f'{lb["DNSName"]}.',
-                    'fqdns': [lb['LoadBalancerName']],
+                    'fqdns': [lb['LoadBalancerName'] + self.append_to_names],
                 }
 
             # request tags and look through them for fqdns
             arns = list(lbs.keys())
             if arns:
                 resp = self._conn.describe_tags(ResourceArns=arns)
                 for td in resp['TagDescriptions']:
                     arn = td['ResourceArn']
                     lb = lbs[arn]
                     for tag in td.get('Tags', []):
                         key = tag['Key']
                         val = tag['Value']
                         if key.startswith(self.tag_prefix):
-                            lb['fqdns'].extend(val.split('/'))
+                            lb['fqdns'].extend(
+                                fqdn + self.append_to_names
+                                for fqdn in val.split('/')
+                            )
 
             for lb in lbs.values():
                 fqdns = lb['fqdns']
                 fqdns = [f'{i}.' if i[-1] != '.' else i for i in fqdns]
                 lb['fqdns'] = fqdns
 
             # add .'s to fqdns that don't have them
```

### Comparing `octodns-route53-0.0.6/octodns_route53.egg-info/PKG-INFO` & `octodns-route53-0.0.7/octodns_route53.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octodns-route53
-Version: 0.0.6
+Version: 0.0.7
 Summary:  Route53Provider provider for octoDNS
 Home-page: https://github.com/octodns/octodns-route53
 Author: Ross McFarland
 Author-email: rwmcfa1@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 Requires-Dist: boto3>=1.20.26
 Requires-Dist: octodns>=0.9.18
 Requires-Dist: pycountry-convert>=0.7.2
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-network; extra == "dev"
-Requires-Dist: black<24.0.0,>=23.1.0; extra == "dev"
+Requires-Dist: black<25.0.0,>=24.3.0; extra == "dev"
 Requires-Dist: build>=0.7.0; extra == "dev"
 Requires-Dist: isort>=5.11.5; extra == "dev"
 Requires-Dist: pyflakes>=2.2.0; extra == "dev"
 Requires-Dist: readme_renderer[md]>=26.0; extra == "dev"
 Requires-Dist: twine>=3.4.2; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
@@ -89,22 +89,24 @@
     # auth options are the same as Route53Provider
     access_key_id: env/AWS_ACCESS_KEY_ID
     secret_access_key: env/AWS_SECRET_ACCESS_KEY
     # The region in which to look for EC2 instances, required.
     region: us-east-1
     # Prefix for tag keys containing fqdn(s)
     #tag_prefix: octodns
+    # String to append to all names and tag values
+    #append_to_names: mydomain.com.
     #ttl: 3600
 ```
 
 In general the account used will need read permissions on EC2 instances.
 
 Records are driven off of the tags attached to the EC2 instances. The "Name" tag and any tags starting with `tag_prefix` are considered.
 
-The value of the tag should be one or more fqdns separated by a `/` character.
+The value of the tag should be one or more fqdns separated by a `/` character. You can append a string to the name and all tag values with `append_to_names`.
 
 When a zone is being populated any fqdns matching the zone name will result in records. When the instance has a private IPv4 address an A record will be created. When the instance has an IPv6 address a AAAA record will be created.
 
 When the zone is a sub-zone of in-addr.arpa. PTR records will be created for private IPv4 addresses that match the zone. The value(s) will be the fqdn(s) associated with that private IPv4 address.
 
 When the zone is a sub-zone of ip6.arpa. PTR records will be created for IPv6 addresses that match the zone. The value(s) will be the fqdn(s) associated with that IPv6 address.
 
@@ -117,22 +119,24 @@
     # auth options are the same as Route53Provider
     access_key_id: env/AWS_ACCESS_KEY_ID
     secret_access_key: env/AWS_SECRET_ACCESS_KEY
     # The region in which to look for ELB instances, required.
     region: us-east-1
     # Prefix for tag keys containing fqdn(s)
     #tag_prefix: octodns
+    # String to append to all names and tag values
+    #append_to_names: mydomain.com.
     #ttl: 3600
 ```
 
 In general the account used will need read permissions on ELB instances and tags.
 
 Records are driven off of the ELB name and the tags attached to the ELB instances. Any tag with `tag_prefix` is considered.
 
-The value of the tag should be one or more fqdns separated by a `/` character.
+The value of the tag should be one or more fqdns separated by a `/` character. You can append a string to the name and all tag values with `append_to_names`.
 
 When a zone is being populated any fqdns matching the zone name will result in records CNAME records with the target value being the DNSName of the ELB instance.
 
 #### Example Tags for EC2/ELB
 
 ```yaml
 # This will result in an ALIAS record for example.com. -> DNSName
@@ -169,15 +173,15 @@
     ...
 ```
 
 ### Support Information
 
 #### Records
 
-A, AAAA, CAA, CNAME, MX, NAPTR, NS, PTR, SPF, SRV, TXT
+A, AAAA, CAA, CNAME, DS, MX, NAPTR, NS, PTR, SPF, SRV, TXT
 
 #### Root NS Records
 
 Route53Provider supports full root NS record management.
 
 #### Dynamic
```

### Comparing `octodns-route53-0.0.6/setup.py` & `octodns-route53-0.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,25 @@
-from os import environ
-from subprocess import CalledProcessError, check_output
+#!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 
 def descriptions():
     with open('README.md') as fh:
         ret = fh.read()
         first = ret.split('\n', 1)[0].replace('#', '')
         return first, ret
 
 
 def version():
-    version = 'unknown'
     with open('octodns_route53/__init__.py') as fh:
         for line in fh:
-            if line.startswith('__VERSION__'):
-                version = line.split("'")[1]
-                break
-
-    # pep440 style public & local version numbers
-    if environ.get('OCTODNS_RELEASE', False):
-        # public
-        return version
-    try:
-        sha = check_output(['git', 'rev-parse', 'HEAD']).decode('utf-8')[:8]
-    except (CalledProcessError, FileNotFoundError):
-        sha = 'unknown'
-    # local
-    return f'{version}+{sha}'
+            if line.startswith('__version__'):
+                return line.split("'")[1]
+    return 'unknown'
 
 
 description, long_description = descriptions()
 
 tests_require = ('pytest', 'pytest-cov', 'pytest-network')
 
 setup(
@@ -42,15 +29,15 @@
     extras_require={
         'dev': tests_require
         + (
             # we need to manually/explicitely bump major versions as they're
             # likely to result in formatting changes that should happen in their
             # own PR. This will basically happen yearly
             # https://black.readthedocs.io/en/stable/the_black_code_style/index.html#stability-policy
-            'black>=23.1.0,<24.0.0',
+            'black>=24.3.0,<25.0.0',
             'build>=0.7.0',
             'isort>=5.11.5',
             'pyflakes>=2.2.0',
             'readme_renderer[md]>=26.0',
             'twine>=3.4.2',
         ),
         'test': tests_require,
```

### Comparing `octodns-route53-0.0.6/tests/test_octodns_provider_route53.py` & `octodns-route53-0.0.7/tests/test_octodns_provider_route53.py`

 * *Files 1% similar despite different names*

```diff
@@ -401,14 +401,29 @@
             {
                 'ttl': 69,
                 'type': 'CAA',
                 'value': {'flags': 0, 'tag': 'issue', 'value': 'ca.unit.tests'},
             },
         ),
         (
+            'dskey',
+            {
+                'ttl': 70,
+                'type': 'DS',
+                'values': [
+                    {
+                        'key_tag': 60485,
+                        'algorithm': 5,
+                        'digest_type': 1,
+                        'digest': '2BB183AF5F22588179A53B0A 98631FAD1A292118',
+                    }
+                ],
+            },
+        ),
+        (
             'alias',
             {
                 'ttl': 942942942,
                 'type': 'Route53Provider/ALIAS',
                 'values': [
                     {'name': '', 'type': 'A'},
                     {'name': 'naptr', 'type': 'NAPTR'},
@@ -600,18 +615,17 @@
 
         stubber.add_response('list_hosted_zones', list_hosted_zones)
 
         provider.update_r53_zones("unit.tests.")
         self.assertEqual(provider._r53_zones, {'unit.tests.': 'z40'})
 
     def test_update_r53_zones_with_get_zones_by_name(self):
-        (
-            provider,
-            stubber,
-        ) = self._get_stubbed_get_zones_by_name_enabled_provider()
+        (provider, stubber) = (
+            self._get_stubbed_get_zones_by_name_enabled_provider()
+        )
 
         list_hosted_zones_by_name_resp = {
             'HostedZones': [
                 {
                     'Id': 'z40',
                     'Name': 'unit.tests.',
                     'CallerReference': 'abc',
@@ -655,18 +669,17 @@
 
         provider.update_r53_zones("0/25.2.0.192.in-addr.arpa.")
         self.assertEqual(
             provider._r53_zones, {'0/25.2.0.192.in-addr.arpa.': 'z41'}
         )
 
     def test_update_r53_zones_with_get_zones_by_name_octal_replaced(self):
-        (
-            provider,
-            stubber,
-        ) = self._get_stubbed_get_zones_by_name_enabled_provider()
+        (provider, stubber) = (
+            self._get_stubbed_get_zones_by_name_enabled_provider()
+        )
 
         list_hosted_zones_by_name_resp = {
             'HostedZones': [
                 {
                     'Id': 'z41',
                     'Name': '0\\05725.2.0.192.in-addr.arpa.',
                     'CallerReference': 'abc',
@@ -844,14 +857,15 @@
         assume_role_mock = Mock()
         assume_role_mock.assume_role.side_effect = [
             {
                 'Credentials': {
                     'AccessKeyId': 42,
                     'SecretAccessKey': 43,
                     'Expiration': 44,
+                    'SessionToken': 45,
                 }
             }
         ]
         # first call will be for the STS client which needs to assume role,
         # the second call will be for the route53 client, it won't be used
         client_mock.side_effect = [assume_role_mock, False]
         # now create our provider
@@ -879,15 +893,15 @@
                 ),
                 # the second time, with the assumed role's key, secret,
                 # and session, this time to gets the actual route53 client
                 call(
                     service_name='route53',
                     aws_access_key_id=42,
                     aws_secret_access_key=43,
-                    aws_session_token=44,
+                    aws_session_token=45,
                     config=None,
                 ),
             ]
         )
 
     def test_list_zones(self):
         provider, stubber = self._get_stubbed_provider()
@@ -1111,14 +1125,24 @@
                 {
                     'Name': 'unit.tests.',
                     'Type': 'CAA',
                     'ResourceRecords': [{'Value': '0 issue "ca.unit.tests"'}],
                     'TTL': 69,
                 },
                 {
+                    'Name': 'dskey.unit.tests.',
+                    'Type': 'DS',
+                    'ResourceRecords': [
+                        {
+                            'Value': '60485 5 1 2BB183AF5F22588179A53B0A 98631FAD1A292118'
+                        }
+                    ],
+                    'TTL': 70,
+                },
+                {
                     'AliasTarget': {
                         'HostedZoneId': 'Z119WBBTVP5WFX',
                         'EvaluateTargetHealth': False,
                         'DNSName': 'unit.tests.',
                     },
                     'Type': 'A',
                     'Name': 'alias.unit.tests.',
@@ -1239,15 +1263,15 @@
         stubber.add_response(
             'list_resource_record_sets',
             list_resource_record_sets_resp,
             {'HostedZoneId': 'z42'},
         )
 
         plan = provider.plan(self.expected)
-        self.assertEqual(12, len(plan.changes))
+        self.assertEqual(13, len(plan.changes))
         self.assertTrue(plan.exists)
         for change in plan.changes:
             self.assertIsInstance(change, Create)
         stubber.assert_no_pending_responses()
 
         stubber.add_response(
             'list_health_checks',
@@ -1266,15 +1290,15 @@
                     'Status': 'PENDING',
                     'SubmittedAt': '2017-01-29T01:02:03Z',
                 }
             },
             {'HostedZoneId': 'z42', 'ChangeBatch': ANY},
         )
 
-        self.assertEqual(12, provider.apply(plan))
+        self.assertEqual(13, provider.apply(plan))
         stubber.assert_no_pending_responses()
 
         # Delete by monkey patching in a populate that includes an extra record
         def add_extra_populate(existing, target, lenient):
             for record in self.expected.records:
                 existing.add_record(record)
             record = Record.new(
@@ -1532,15 +1556,15 @@
             'Marker': 'm',
             'IsTruncated': False,
             'MaxItems': '100',
         }
         stubber.add_response('list_hosted_zones', list_hosted_zones_resp, {})
 
         plan = provider.plan(self.expected)
-        self.assertEqual(12, len(plan.changes))
+        self.assertEqual(13, len(plan.changes))
         self.assertFalse(plan.exists)
         for change in plan.changes:
             self.assertIsInstance(change, Create)
         stubber.assert_no_pending_responses()
 
         create_hosted_zone_resp = {
             'HostedZone': {
@@ -1604,15 +1628,15 @@
                     'Status': 'PENDING',
                     'SubmittedAt': '2017-01-29T01:02:03Z',
                 }
             },
             {'HostedZoneId': 'z42', 'ChangeBatch': ANY},
         )
 
-        self.assertEqual(12, provider.apply(plan))
+        self.assertEqual(13, provider.apply(plan))
         stubber.assert_no_pending_responses()
 
     def test_sync_create_with_delegation_set(self):
         provider, stubber = self._get_stubbed_delegation_set_provider()
 
         got = Zone('unit.tests.', [])
 
@@ -1621,15 +1645,15 @@
             'Marker': 'm',
             'IsTruncated': False,
             'MaxItems': '100',
         }
         stubber.add_response('list_hosted_zones', list_hosted_zones_resp, {})
 
         plan = provider.plan(self.expected)
-        self.assertEqual(12, len(plan.changes))
+        self.assertEqual(13, len(plan.changes))
         self.assertFalse(plan.exists)
         for change in plan.changes:
             self.assertIsInstance(change, Create)
         stubber.assert_no_pending_responses()
 
         create_hosted_zone_resp = {
             'HostedZone': {
@@ -1697,15 +1721,15 @@
                     'Status': 'PENDING',
                     'SubmittedAt': '2017-01-29T01:02:03Z',
                 }
             },
             {'HostedZoneId': 'z42', 'ChangeBatch': ANY},
         )
 
-        self.assertEqual(12, provider.apply(plan))
+        self.assertEqual(13, provider.apply(plan))
         stubber.assert_no_pending_responses()
 
     def test_health_checks_pagination(self):
         provider, stubber = self._get_stubbed_provider()
 
         health_checks_p1 = [
             {
@@ -2519,18 +2543,17 @@
         # short-circuit for unknown zone
         other = Zone('other.tests.', [])
         extra = provider._extra_changes(desired=other, changes=[])
         self.assertEqual([], extra)
         stubber.assert_no_pending_responses()
 
     def test_no_changes_with_get_zones_by_name(self):
-        (
-            provider,
-            stubber,
-        ) = self._get_stubbed_get_zones_by_name_enabled_provider()
+        (provider, stubber) = (
+            self._get_stubbed_get_zones_by_name_enabled_provider()
+        )
 
         list_hosted_zones_by_name_resp_1 = {
             'HostedZones': [
                 {
                     'Id': 'z42',
                     'Name': 'unit.tests.',
                     'CallerReference': 'abc',
@@ -2581,18 +2604,17 @@
         # empty is empty
         desired = Zone('unit2.tests.', [])
         extra = provider._extra_changes(desired=desired, changes=[])
         self.assertEqual([], extra)
         stubber.assert_no_pending_responses()
 
     def test_zone_not_found_get_zones_by_name(self):
-        (
-            provider,
-            stubber,
-        ) = self._get_stubbed_get_zones_by_name_enabled_provider()
+        (provider, stubber) = (
+            self._get_stubbed_get_zones_by_name_enabled_provider()
+        )
 
         list_hosted_zones_by_name_resp = {
             'HostedZones': [
                 {
                     'Id': 'z43',
                     'Name': 'bad.tests.',
                     'CallerReference': 'abc',
@@ -2615,18 +2637,17 @@
         # empty is empty
         desired = Zone('unit.tests.', [])
         extra = provider._extra_changes(desired=desired, changes=[])
         self.assertEqual([], extra)
         stubber.assert_no_pending_responses()
 
     def test_plan_apply_with_get_zones_by_name_zone_not_exists(self):
-        (
-            provider,
-            stubber,
-        ) = self._get_stubbed_get_zones_by_name_enabled_provider()
+        (provider, stubber) = (
+            self._get_stubbed_get_zones_by_name_enabled_provider()
+        )
 
         # this is an empty response
         # zone name not found
         list_hosted_zones_by_name_resp = {
             'HostedZones': [],
             'DNSName': 'unit.tests.',
             'HostedZoneId': 'z42',
@@ -2637,15 +2658,15 @@
         stubber.add_response(
             'list_hosted_zones_by_name',
             list_hosted_zones_by_name_resp,
             {'DNSName': 'unit.tests.', 'MaxItems': '1'},
         )
 
         plan = provider.plan(self.expected)
-        self.assertEqual(12, len(plan.changes))
+        self.assertEqual(13, len(plan.changes))
 
         create_hosted_zone_resp = {
             'HostedZone': {
                 'Name': 'unit.tests.',
                 'Id': 'z42',
                 'CallerReference': 'abc',
             },
@@ -2705,22 +2726,21 @@
                     'Status': 'PENDING',
                     'SubmittedAt': '2017-01-29T01:02:03Z',
                 }
             },
             {'HostedZoneId': 'z42', 'ChangeBatch': ANY},
         )
 
-        self.assertEqual(12, provider.apply(plan))
+        self.assertEqual(13, provider.apply(plan))
         stubber.assert_no_pending_responses()
 
     def test_plan_apply_with_get_zones_by_name_zone_exists(self):
-        (
-            provider,
-            stubber,
-        ) = self._get_stubbed_get_zones_by_name_enabled_provider()
+        (provider, stubber) = (
+            self._get_stubbed_get_zones_by_name_enabled_provider()
+        )
 
         list_hosted_zones_by_name_resp = {
             'HostedZones': [
                 {
                     'Id': 'z42',
                     'Name': 'unit.tests.',
                     'CallerReference': 'abc',
@@ -2756,15 +2776,15 @@
         stubber.add_response(
             'list_resource_record_sets',
             list_resource_record_sets_resp,
             {'HostedZoneId': 'z42'},
         )
 
         plan = provider.plan(self.expected)
-        self.assertEqual(13, len(plan.changes))
+        self.assertEqual(14, len(plan.changes))
 
         stubber.add_response(
             'list_health_checks',
             {
                 'HealthChecks': self.health_checks,
                 'IsTruncated': False,
                 'MaxItems': '100',
@@ -2780,15 +2800,15 @@
                     'Status': 'PENDING',
                     'SubmittedAt': '2017-01-29T01:02:03Z',
                 }
             },
             {'HostedZoneId': 'z42', 'ChangeBatch': ANY},
         )
 
-        self.assertEqual(13, provider.apply(plan))
+        self.assertEqual(14, provider.apply(plan))
         stubber.assert_no_pending_responses()
 
     def test_extra_change_no_health_check(self):
         provider, stubber = self._get_stubbed_provider()
 
         list_hosted_zones_resp = {
             'HostedZones': [
@@ -3446,15 +3466,15 @@
 
     # _get_test_plan() returns a plan with 11 modifications, 17 RRs
 
     @patch('octodns_route53.Route53Provider._load_records')
     @patch('octodns_route53.Route53Provider._really_apply')
     def test_apply_1(self, really_apply_mock, _):
         # 18 RRs with max of 19 should only get applied in one call
-        provider, plan = self._get_test_plan(19)
+        provider, plan = self._get_test_plan(20)
         provider.apply(plan)
         really_apply_mock.assert_called_once()
 
     @patch('octodns_route53.Route53Provider._load_records')
     @patch('octodns_route53.Route53Provider._really_apply')
     def test_apply_2(self, really_apply_mock, _):
         # 18 RRs with max of 17 should only get applied in two calls
@@ -3464,15 +3484,15 @@
 
     @patch('octodns_route53.Route53Provider._load_records')
     @patch('octodns_route53.Route53Provider._really_apply')
     def test_apply_3(self, really_apply_mock, _):
         # with a max of seven modifications, three calls
         provider, plan = self._get_test_plan(7)
         provider.apply(plan)
-        self.assertEqual(3, really_apply_mock.call_count)
+        self.assertEqual(4, really_apply_mock.call_count)
 
     @patch('octodns_route53.Route53Provider._load_records')
     @patch('octodns_route53.Route53Provider._really_apply')
     def test_apply_4(self, really_apply_mock, _):
         # with a max of 11 modifications, two calls
         provider, plan = self._get_test_plan(11)
         provider.apply(plan)
```

### Comparing `octodns-route53-0.0.6/tests/test_octodns_source_ec2.py` & `octodns-route53-0.0.7/tests/test_octodns_source_ec2.py`

 * *Files 14% similar despite different names*

```diff
@@ -175,14 +175,55 @@
         records = {r.name.split('.', 1)[0]: r for r in ip6_arpa.records}
         self.assertEqual('all.unit.tests.', records['1'].value)
         self.assertEqual(
             ['2nd-v6.unit.tests.', 'v6.unit.tests.'], records['2'].values
         )
         self.assertEqual(2, len(records))
 
+    def test_append(self):
+        source, stubber = self._get_stubbed_source(append_to_names="org.")
+
+        zone = Zone('unit.tests.org.', [])
+        in_addr_arpa = Zone('0.0.10.in-addr.arpa.', [])
+        ip6_arpa = Zone('0.0.c.f.ip6.arpa.', [])
+
+        stubber.add_response(
+            'describe_instances', {'Reservations': self.reservations}
+        )
+        source.populate(zone)
+
+        # Our append string assumes names end with . - no entries for iv4, 2nd,
+        # or 2nd-v6. So expect 3 A and 1 AAAA
+        records = {(r.name, r._type): r for r in zone.records}
+        self.assertEqual(['10.0.0.14'], records[('all', 'A')].values)
+        self.assertEqual(['10.0.1.99'], records[('iv4-other', 'A')].values)
+        self.assertEqual(['10.0.0.16'], records[('v4', 'A')].values)
+        self.assertEqual(['fc00::1'], records[('all', 'AAAA')].values)
+        self.assertEqual(['fc00::2'], records[('v6', 'AAAA')].values)
+        self.assertEqual(5, len(records))
+
+        # expect 3 ipv4 PTRs
+        source.populate(in_addr_arpa)
+        records = {r.name: r for r in in_addr_arpa.records}
+        self.assertEqual('all.unit.tests.org.', records['14'].value)
+        self.assertEqual('iv4.unit.testsorg.', records['15'].value)
+        self.assertEqual(
+            ['2nd.unit.testsorg.', 'v4.unit.tests.org.'], records['16'].values
+        )
+        self.assertEqual(3, len(records))
+
+        # expect 3 ipv6 PTRs
+        source.populate(ip6_arpa)
+        records = {r.name.split('.', 1)[0]: r for r in ip6_arpa.records}
+        self.assertEqual('all.unit.tests.org.', records['1'].value)
+        self.assertEqual(
+            ['2nd-v6.unit.testsorg.', 'v6.unit.tests.org.'], records['2'].values
+        )
+        self.assertEqual(2, len(records))
+
     def test_conflicting_fqdns(self):
         source, stubber = self._get_stubbed_source()
 
         zone = Zone('unit.tests.', [])
 
         stubber.add_response(
             'describe_instances',
```

### Comparing `octodns-route53-0.0.6/tests/test_octodns_source_elb.py` & `octodns-route53-0.0.7/tests/test_octodns_source_elb.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,95 @@
 
 from octodns.zone import Zone
 
 from octodns_route53 import ElbSource
 
 
 class TestElbSource(TestCase):
+    load_balancers = {
+        'LoadBalancers': [
+            {
+                # matches name
+                'DNSName': 'foo.aws.com',
+                'LoadBalancerArn': 'arn42',
+                'LoadBalancerName': 'service.unit.tests.',
+            },
+            {
+                # doesn't match
+                'DNSName': 'bar.aws.com',
+                'LoadBalancerArn': 'arn43',
+                'LoadBalancerName': 'this.doesnt.match.',
+            },
+            {
+                # matches, no trailing dot
+                'DNSName': 'baz.aws.com',
+                'LoadBalancerArn': 'arn44',
+                'LoadBalancerName': 'no-dot.unit.tests',
+            },
+            {
+                # name doesn't match, but tags will
+                'DNSName': 'blip.aws.com',
+                'LoadBalancerArn': 'arn45',
+                'LoadBalancerName': 'tags.will.match.',
+            },
+            {
+                # both name and tags match
+                'DNSName': 'bang.aws.com',
+                'LoadBalancerArn': 'arn46',
+                'LoadBalancerName': 'both.unit.tests.',
+            },
+        ]
+    }
+    tags = {
+        'TagDescriptions': [
+            {
+                'ResourceArn': 'arn42',
+                'Tags': [{'Key': 'irrelevant', 'Value': 'doesnt matter'}],
+            },
+            {'ResourceArn': 'arn43'},
+            {'ResourceArn': 'arn44'},
+            {
+                'ResourceArn': 'arn45',
+                'Tags': [
+                    {
+                        'Key': 'octodns',
+                        # multi-value: one matches w/dot. one matches w/o dot, one
+                        # doesn't match
+                        'Value': 'first.unit.tests./second.unit.tests/third.thing.',
+                    }
+                ],
+            },
+            {
+                'ResourceArn': 'arn46',
+                'Tags': [
+                    {
+                        'Key': 'octodns-1',
+                        # matches
+                        'Value': 'fourth.unit.tests.',
+                    },
+                    {
+                        'Key': 'octodns-2',
+                        # matches w/o dot
+                        'Value': 'fifth.unit.tests',
+                    },
+                    {
+                        'Key': 'octodns-2',
+                        # doesn't match
+                        'Value': 'sixth.doesnt.apply.',
+                    },
+                    {
+                        'Key': 'octodns-3',
+                        # apex match
+                        'Value': 'unit.tests.',
+                    },
+                ],
+            },
+        ]
+    }
+
     def _get_stubbed_source(self, **kwargs):
         source = ElbSource('test', 'us-east-1', 'abc', '123', **kwargs)
 
         # Use the stubber
         stubber = Stubber(source._conn)
         stubber.activate()
 
@@ -37,103 +118,17 @@
         self.assertEqual(0, len(zone.records))
 
     def test_lbs(self):
         source, stubber = self._get_stubbed_source()
 
         zone = Zone('unit.tests.', [])
 
-        stubber.add_response(
-            'describe_load_balancers',
-            {
-                'LoadBalancers': [
-                    {
-                        # matches name
-                        'DNSName': 'foo.aws.com',
-                        'LoadBalancerArn': 'arn42',
-                        'LoadBalancerName': 'service.unit.tests.',
-                    },
-                    {
-                        # doesn't match
-                        'DNSName': 'bar.aws.com',
-                        'LoadBalancerArn': 'arn43',
-                        'LoadBalancerName': 'this.doesnt.match.',
-                    },
-                    {
-                        # matches, no trailing dot
-                        'DNSName': 'baz.aws.com',
-                        'LoadBalancerArn': 'arn44',
-                        'LoadBalancerName': 'no-dot.unit.tests',
-                    },
-                    {
-                        # name doesn't match, but tags will
-                        'DNSName': 'blip.aws.com',
-                        'LoadBalancerArn': 'arn45',
-                        'LoadBalancerName': 'tags.will.match.',
-                    },
-                    {
-                        # both name and tags match
-                        'DNSName': 'bang.aws.com',
-                        'LoadBalancerArn': 'arn46',
-                        'LoadBalancerName': 'both.unit.tests.',
-                    },
-                ]
-            },
-        )
+        stubber.add_response('describe_load_balancers', self.load_balancers)
 
-        stubber.add_response(
-            'describe_tags',
-            {
-                'TagDescriptions': [
-                    {
-                        'ResourceArn': 'arn42',
-                        'Tags': [
-                            {'Key': 'irrelevant', 'Value': 'doesnt matter'}
-                        ],
-                    },
-                    {'ResourceArn': 'arn43'},
-                    {'ResourceArn': 'arn44'},
-                    {
-                        'ResourceArn': 'arn45',
-                        'Tags': [
-                            {
-                                'Key': 'octodns',
-                                # multi-value: one matches w/dot. one matches w/o dot, one
-                                # doesn't match
-                                'Value': 'first.unit.tests./second.unit.tests/third.thing.',
-                            }
-                        ],
-                    },
-                    {
-                        'ResourceArn': 'arn46',
-                        'Tags': [
-                            {
-                                'Key': 'octodns-1',
-                                # matches
-                                'Value': 'fourth.unit.tests.',
-                            },
-                            {
-                                'Key': 'octodns-2',
-                                # matches w/o dot
-                                'Value': 'fifth.unit.tests',
-                            },
-                            {
-                                'Key': 'octodns-2',
-                                # doesn't match
-                                'Value': 'sixth.doesnt.apply.',
-                            },
-                            {
-                                'Key': 'octodns-3',
-                                # apex match
-                                'Value': 'unit.tests.',
-                            },
-                        ],
-                    },
-                ]
-            },
-        )
+        stubber.add_response('describe_tags', self.tags)
 
         source.populate(zone)
 
         records = {r.name: r for r in zone.records}
         self.assertEqual('foo.aws.com.', records['service'].value)
         self.assertEqual('baz.aws.com.', records['no-dot'].value)
         self.assertEqual('blip.aws.com.', records['first'].value)
@@ -148,9 +143,35 @@
         # apex is an ALIAS
         record = records.pop('')
         self.assertEqual('ALIAS', record._type)
         # rest are CNAMEs
         for record in records.values():
             self.assertEqual('CNAME', record._type)
 
+    def test_append(self):
+        source, stubber = self._get_stubbed_source(append_to_names="local.")
+
+        zone = Zone('unit.tests.local.', [])
+
+        stubber.add_response('describe_load_balancers', self.load_balancers)
+
+        stubber.add_response('describe_tags', self.tags)
+
+        source.populate(zone)
+
+        # Our append string assumes names end with . - no entries for no-dot,
+        # second, or fifth
+        records = {r.name: r for r in zone.records}
+        self.assertEqual('foo.aws.com.', records['service'].value)
+        self.assertEqual('blip.aws.com.', records['first'].value)
+        self.assertEqual('bang.aws.com.', records['both'].value)
+        self.assertEqual('bang.aws.com.', records['fourth'].value)
+        self.assertEqual('bang.aws.com.', records[''].value)
+        self.assertEqual(5, len(records))
+
+        record = records.pop('')
+        self.assertEqual('ALIAS', record._type)
+        for record in records.values():
+            self.assertEqual('CNAME', record._type)
+
     def test_conflicting_fqdns(self):
         pass
```

