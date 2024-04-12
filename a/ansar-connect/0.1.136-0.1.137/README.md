# Comparing `tmp/ansar-connect-0.1.136.tar.gz` & `tmp/ansar-connect-0.1.137.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar-connect-0.1.136.tar", last modified: Sun Apr  7 04:19:05 2024, max compression
+gzip compressed data, was "ansar-connect-0.1.137.tar", last modified: Fri Apr 12 00:43:55 2024, max compression
```

## Comparing `ansar-connect-0.1.136.tar` & `ansar-connect-0.1.137.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-07 04:19:05.187583 ansar-connect-0.1.136/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar-connect-0.1.136/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-07 04:19:05.187583 ansar-connect-0.1.136/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar-connect-0.1.136/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar-connect-0.1.136/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-07 04:19:05.187583 ansar-connect-0.1.136/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar-connect-0.1.136/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-07 04:19:05.187583 ansar-connect-0.1.136/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-07 04:19:05.187583 ansar-connect-0.1.136/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-07 04:19:05.187583 ansar-connect-0.1.136/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14427 2024-03-29 02:37:30.000000 ansar-connect-0.1.136/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3072 2024-03-04 07:28:05.000000 ansar-connect-0.1.136/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-03-26 18:46:17.000000 ansar-connect-0.1.136/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8658 2024-03-29 22:32:03.000000 ansar-connect-0.1.136/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-07 04:19:05.187583 ansar-connect-0.1.136/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-04-07 04:19:02.000000 ansar-connect-0.1.136/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    13865 2024-04-07 03:44:19.000000 ansar-connect-0.1.136/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    77328 2024-04-07 00:39:18.000000 ansar-connect-0.1.136/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar-connect-0.1.136/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar-connect-0.1.136/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2119 2024-03-23 19:35:11.000000 ansar-connect-0.1.136/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar-connect-0.1.136/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar-connect-0.1.136/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar-connect-0.1.136/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar-connect-0.1.136/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar-connect-0.1.136/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar-connect-0.1.136/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    37271 2024-04-04 20:50:42.000000 ansar-connect-0.1.136/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2323 2024-03-29 22:32:03.000000 ansar-connect-0.1.136/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    36421 2024-03-26 19:24:58.000000 ansar-connect-0.1.136/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar-connect-0.1.136/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2065 2023-09-27 02:08:10.000000 ansar-connect-0.1.136/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6367 2024-04-07 03:37:54.000000 ansar-connect-0.1.136/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-07 04:19:05.187583 ansar-connect-0.1.136/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-07 04:19:05.000000 ansar-connect-0.1.136/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-07 04:19:05.000000 ansar-connect-0.1.136/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-07 04:19:05.000000 ansar-connect-0.1.136/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-07 04:19:05.000000 ansar-connect-0.1.136/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-07 04:19:05.000000 ansar-connect-0.1.136/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-07 04:19:05.000000 ansar-connect-0.1.136/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 00:43:55.840062 ansar-connect-0.1.137/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar-connect-0.1.137/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-12 00:43:55.840062 ansar-connect-0.1.137/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar-connect-0.1.137/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar-connect-0.1.137/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-12 00:43:55.840062 ansar-connect-0.1.137/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar-connect-0.1.137/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 00:43:55.840062 ansar-connect-0.1.137/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 00:43:55.840062 ansar-connect-0.1.137/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 00:43:55.840062 ansar-connect-0.1.137/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14427 2024-03-29 02:37:30.000000 ansar-connect-0.1.137/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3562 2024-04-11 23:48:03.000000 ansar-connect-0.1.137/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10088 2024-04-11 23:51:57.000000 ansar-connect-0.1.137/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9236 2024-04-12 00:33:17.000000 ansar-connect-0.1.137/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 00:43:55.840062 ansar-connect-0.1.137/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3055 2024-04-12 00:43:52.000000 ansar-connect-0.1.137/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    13941 2024-04-11 23:33:25.000000 ansar-connect-0.1.137/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    77714 2024-04-11 23:32:28.000000 ansar-connect-0.1.137/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar-connect-0.1.137/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar-connect-0.1.137/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar-connect-0.1.137/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar-connect-0.1.137/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar-connect-0.1.137/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar-connect-0.1.137/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar-connect-0.1.137/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar-connect-0.1.137/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar-connect-0.1.137/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    37547 2024-04-11 23:51:57.000000 ansar-connect-0.1.137/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2323 2024-03-29 22:32:03.000000 ansar-connect-0.1.137/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    38262 2024-04-11 01:07:01.000000 ansar-connect-0.1.137/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar-connect-0.1.137/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2205 2024-04-11 00:02:31.000000 ansar-connect-0.1.137/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6367 2024-04-07 03:37:54.000000 ansar-connect-0.1.137/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 00:43:55.840062 ansar-connect-0.1.137/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-12 00:43:55.000000 ansar-connect-0.1.137/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-12 00:43:55.000000 ansar-connect-0.1.137/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-12 00:43:55.000000 ansar-connect-0.1.137/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-12 00:43:55.000000 ansar-connect-0.1.137/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-12 00:43:55.000000 ansar-connect-0.1.137/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-12 00:43:55.000000 ansar-connect-0.1.137/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar-connect-0.1.136/LICENSE` & `ansar-connect-0.1.137/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.136/PKG-INFO` & `ansar-connect-0.1.137/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.136
+Version: 0.1.137
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-connect-0.1.136/README.md` & `ansar-connect-0.1.137/README.md`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.136/pyproject.toml` & `ansar-connect-0.1.137/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.136/setup.py` & `ansar-connect-0.1.137/setup.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.136/src/ansar/command/ansar_command.py` & `ansar-connect-0.1.137/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.136/src/ansar/command/ansar_directory.py` & `ansar-connect-0.1.137/src/ansar/command/ansar_directory.py`

 * *Files 26% similar despite different names*

```diff
@@ -30,31 +30,45 @@
 __all__ = [
 	'main',
 ]
 
 #
 #
 class Settings(object):
-	def __init__(self, directory_scope=None, connect_above=None, accept_below=None):
+	def __init__(self, directory_scope=None, connect_above=None, accept_below=None,
+			certificate_file=None, key_file=None, SNI=None):
 		self.directory_scope = directory_scope or ar.ScopeOfService.HOST
 		self.connect_above = connect_above or ar.HostPort()
 		self.accept_below = accept_below or ar.HostPort()
 
 SETTINGS_SCHEMA = {
 	'directory_scope': ar.ScopeOfService,
 	'connect_above': ar.Any(),
 	'accept_below': ar.UserDefined(ar.HostPort),
+	'certificate_file': ar.Unicode(),
+	'key_file': ar.Unicode(),
+	'SNI': ar.Unicode(),
 }
 
 ar.bind(Settings, object_schema=SETTINGS_SCHEMA)
 
 # Just need an object to stay "on duty" while the 
 # global ServiceDirectory does its work.
 def directory(self, settings):
-	a = self.create(ar.ServiceDirectory, settings.directory_scope, settings.connect_above, settings.accept_below)
+	encryption_above = None
+	encryption_below = None
+
+	if settings.SNI:
+		encryption_above = ar.TlsClient(SNI=settings.SNI)
+	if settings.certificate_file and settings.key_file:
+		encryption_below = ar.TlsServer(certificate_file=settings.certificate_file, key_file=settings.key_file)
+
+	a = self.create(ar.ServiceDirectory, settings.directory_scope,
+		settings.connect_above, settings.accept_below,
+		encryption_above=encryption_above, encryption_below=encryption_below)
 	m = self.select(ar.HostPort, ar.Completed, ar.Stop)
 	if isinstance(m, ar.Completed):
 		return m.value
 	elif isinstance(m, ar.Stop):
 		self.send(m, a)
 		self.select(ar.Completed)
 		return ar.Aborted()
```

### Comparing `ansar-connect-0.1.136/src/ansar/command/ansar_group.py` & `ansar-connect-0.1.137/src/ansar/command/ansar_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,15 +196,19 @@
 		hb = hr.home
 		if hb.role_exists(self.main_role):
 			tr = hb.open_role(self.main_role, None, None, ar.NodeProperties())
 			if series(hr.properties.retry) or series(tr.properties.retry):
 				r = ar.Rejected(forwarding_retry=(f'main role "{self.main_role}" is configured to retry', 'not supported'))
 				self.complete(r)
 
-	a = self.create(ar.ServiceDirectory, ar.ScopeOfService.GROUP, connect_above, accept_below)
+	if self.settings.SNI:
+		encryption_above = ar.TlsClient(SNI=self.settings.SNI)
+	else:
+		encryption_above = None
+	a = self.create(ar.ServiceDirectory, ar.ScopeOfService.GROUP, connect_above, accept_below, encryption_above=encryption_above)
 	self.assign(a, None)
 	self.directory = a
 	return OPENING
 
 def Group_OPENING_HostPort(self, message):
 	self.directory_ipp = message
 	self.group_start = ar.world_now()
```

### Comparing `ansar-connect-0.1.136/src/ansar/command/shared_directory.py` & `ansar-connect-0.1.137/src/ansar/command/shared_directory.py`

 * *Files 14% similar despite different names*

```diff
@@ -79,15 +79,20 @@
 	
 	self.store = store
 	self.recover = recover
 
 	# Initial load.
 	self.recover()
 
-	ar.listen(self, self.settings.public_access)
+	settings = self.settings
+	encryption = None
+	if settings.certificate_file and settings.key_file:
+		encryption = ar.TlsServer(certificate_file=settings.certificate_file, key_file=settings.key_file)
+
+	ar.listen(self, self.settings.public_access, encryption=encryption)
 	return STARTING
 
 # Verify access
 def ProductDirectory_STARTING_Listening(self, message):
 	self.public_access = message
 	return READY
 
@@ -168,18 +173,23 @@
 			self.trace(f'Unknown upward key "{k}" for child [{r}]')
 			# Default upward access is disabled but a hint that it
 			# should adopt the same nature.
 			c = ProductAccess(product_name=product_name, product_instance=product_instance)
 			self.connect_above[k] = c
 			self.store()
 
+		encryption_above = None
+		if settings.SNI:
+			encryption_above = ar.TlsClient(SNI=settings.SNI)
+
 		d = self.create(ar.ServiceDirectory,
 			scope=settings.directory_scope,			# All at same scope.
 			connect_above=c,
-			accept_below=ar.HostPort())				# Disabled.
+			accept_below=ar.HostPort(),				# Disabled.
+			encryption_above=encryption_above)
 
 		self.assign(d, k)
 		self.directory[k] = d
 
 	self.child_of[r] = d
 	accepted = self.accepted.get(r)
 	if accepted:
@@ -270,21 +280,27 @@
 
 ar.bind(ProductDirectory, PRODUCT_DIRECTORY_DISPATCH)
 
 
 # Allow configuration of network details.
 #
 class Settings(object):
-	def __init__(self, directory_scope=None, public_access=None):
+	def __init__(self, directory_scope=None, public_access=None, certificate_file=None, key_file=None, SNI=None):
 		self.directory_scope = directory_scope
 		self.public_access = public_access or ar.HostPort()
+		self.certificate_file = certificate_file
+		self.key_file = key_file
+		self.SNI = SNI
 
 SETTINGS_SCHEMA = {
 	'directory_scope': ar.ScopeOfService,
 	'public_access': ar.UserDefined(ar.HostPort),
+	'certificate_file': ar.Unicode(),
+	'key_file': ar.Unicode(),
+	'SNI': ar.Unicode(),
 }
 
 ar.bind(Settings, object_schema=SETTINGS_SCHEMA)
 
 #
 #
 factory_settings = Settings(directory_scope=ar.ScopeOfService.HOST,
```

### Comparing `ansar-connect-0.1.136/src/ansar/connect/__init__.py` & `ansar-connect-0.1.137/src/ansar/connect/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,29 +21,30 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 3dda573a75708fd4a61d6a9d00c224478c2d1e93
-Version: 0.1.135 (2024-04-07@16:19:02+NZST)
+Commit: 58eb33b821cd0a8737502a52624c6715473ceee2
+Version: 0.1.136 (2024-04-12@12:43:52+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
 
 from .socketry import HostPort, LocalPort
 from .socketry import ScopeOfIP, local_private_public
 from .socketry import Blob, CreateFrame
 from .socketry import Listening, NotListening, Accepted, NotAccepted, StopListening
 from .socketry import Connected, NotConnected
 from .socketry import Close, Closed, Abandoned
+from .socketry import TlsServer, TlsClient
 from .transporting import listen, connect, stop_listen
 
 from .plumbing import RETRY_LOCAL, RETRY_PRIVATE, RETRY_PUBLIC
 from .plumbing import ip_retry
 
 from .directory_if import ScopeOfService
 from .directory_if import Published, NotPublished, Subscribed
```

### Comparing `ansar-connect-0.1.136/src/ansar/connect/connect_directory.py` & `ansar-connect-0.1.137/src/ansar/connect/connect_directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,20 +48,21 @@
 class GLARING: pass
 class CONNECTING: pass
 class REDIRECTING: pass
 class ASSIGNING: pass
 class CLOSING: pass
 
 class ConnectToDirectory(ar.Point, ar.StateMachine):
-	def __init__(self, connect_above, session=None, group_address=None):
+	def __init__(self, connect_above, session=None, group_address=None, encryption=None):
 		ar.Point.__init__(self)
 		ar.StateMachine.__init__(self, INITIAL)
 		self.connect_above = connect_above
 		self.session = session
 		self.group_address = group_address
+		self.encryption = encryption
 
 		self.started = None
 		self.attempts = 0
 
 		self.connected = None
 		self.remote = None
 		self.redirect = None
@@ -82,15 +83,15 @@
 			ipp = c.access_ipp
 			next = CLOUDY
 		else:
 			return DISABLED
 
 		if ipp.host is None:
 			return DISABLED
-		connect(self, ipp, session=self.session)
+		connect(self, ipp, session=self.session, encryption=self.encryption)
 		self.start(ar.T1, seconds=8.0)
 		return next
 
 	def reschedule(self):
 		if self.intervals is None:
 			c = self.connect_above
 			if isinstance(c, HostPort):
```

### Comparing `ansar-connect-0.1.136/src/ansar/connect/directory.py` & `ansar-connect-0.1.137/src/ansar/connect/directory.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,14 +243,17 @@
 		self.key = key
 		self.find_address = find_address
 		self.listing_address = listing_address
 		self.connection = connection
 
 def ServiceRoute_INITIAL_Start(self, message):
 	if isinstance(self.connection, ServiceByRelay):
+		# Start creating the relay. This goes to the
+		# object that created this instance of a
+		# directory, e.g. an instance of wan process.
 		relay_id = uuid.uuid4()
 		self.send(RelayLookup(relay_id=relay_id), self.connection.relay_address)
 		self.start(ar.T1, 5.0)
 		return RELAYING
 	outbound = self.connection.outbound(self.key)
 	inbound = self.connection.inbound(self.key)
 
@@ -495,20 +498,22 @@
 			return False
 	return True
 
 CONNECT_ABOVE = 'connect-above'
 ACCEPT_BELOW = 'accept-below'
 
 class ServiceDirectory(ar.Threaded, ar.StateMachine):
-	def __init__(self, scope=None, connect_above=None, accept_below=None):
+	def __init__(self, scope=None, connect_above=None, accept_below=None, encryption_above=None, encryption_below=None):
 		ar.Threaded.__init__(self)
 		ar.StateMachine.__init__(self, INITIAL)
 		self.scope = scope or ScopeOfService.PROCESS
 		self.connect_above = connect_above
 		self.accept_below = accept_below or HostPort()
+		self.encryption_above = encryption_above
+		self.encryption_below = encryption_below
 		self.ctd = None
 		self.directory = {}
 		self.find = {}
 		self.matched = {}
 		self.connected_up = None
 		self.not_connected = None
 		self.connected = None
@@ -768,23 +773,23 @@
 def ServiceDirectory_INITIAL_Start(self, message):
 	self.started = ar.world_now()
 
 	self.trace(f'Scope of {ScopeOfService.to_name(self.scope)}')
 	self.trace(f'Connecting up to "{ar.tof(self.connect_above)}"')
 	self.trace(f'Listening below at "{ar.tof(self.accept_below)}"')
 
-	self.ctd = self.create(ConnectToDirectory, self.connect_above)
+	self.ctd = self.create(ConnectToDirectory, self.connect_above, encryption=self.encryption_above)
 	self.assign(self.ctd, CONNECT_ABOVE)
 
 	# Acceptance of connections from lower directories.
 	if isinstance(self.accept_below, HostPort):
 		if self.accept_below.host is None:
 			self.send(HostPort(host=None), self.parent_address)
 		else:
-			listen(self, self.accept_below, tag='directory-accept')
+			listen(self, self.accept_below, tag='directory-accept', encryption=self.encryption_below)
 			return OPENING
 	else:
 		pass	# Acceptance arranged externally. May be a
 				# Listening object for diagnosis.
 
 	return NORMAL
 
@@ -1195,39 +1200,39 @@
 ### PS-pub-8 Loop terminates by remote close.
 def PublisherLoop_LOOPED_CloseLoop(self, message):
 	if self.created_session:
 		self.send(ar.Stop(), self.created_session)
 		return CLEARING
 	self.close_route()
 
-	self.forward(Dropped(), self.publisher_address, self.origin_address)
+	self.forward(Dropped('abandoned by remote'), self.publisher_address, self.origin_address)
 	self.complete(ar.Aborted())
 
 ### PS-pub-8 Loop terminates by local exit.
 def PublisherLoop_LOOPED_Stop(self, message):
 	self.send(CloseLoop(self.key), self.remote_loop)
 	if self.created_session:
 		self.send(message, self.created_session)
 		return CLEARING
 	self.close_route()
 
-	self.forward(Dropped(), self.publisher_address, self.origin_address)
+	self.forward(Dropped('aborted'), self.publisher_address, self.origin_address)
 	self.complete(ar.Aborted())
 
 def PublisherLoop_CLEARING_Completed(self, message):
 	if self.created_session is None or self.return_address != self.created_session:
 		return CLEARING
 
 	self.create_session = None
 	self.close_route()
 
 	if self.closing:
 		self.forward(Cleared(self.value), self.publisher_address, self.origin_address)
 	else:
-		self.forward(Dropped(), self.publisher_address, self.origin_address)
+		self.forward(Dropped('aborted'), self.publisher_address, self.origin_address)
 
 	self.complete(ar.Aborted())
 
 PUBLISHER_LOOP_DISPATCH = {
 	INITIAL: (
 		(ar.Start,), ()
 	),
@@ -1753,15 +1758,15 @@
 		self.abort()
 		self.clearing_value = True
 		return CLEARING
 	self.complete(True)
 
 # Remote termination.
 def SubscriberLoop_LOOPED_CloseLoop(self, message):
-	self.forward(Dropped('Closed by remote'), self.subscriber_address, self.origin_address)
+	self.forward(Dropped('abandoned by remote'), self.subscriber_address, self.origin_address)
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
 	self.complete(False)
 
@@ -1880,26 +1885,26 @@
 	if self.working():
 		self.abort()
 		self.clearing_value = True
 		return CLEARING
 	self.complete(True)
 
 def SubscriberLoop_CONNECTION_LOOPED_CloseLoop(self, message):
-	self.forward(Dropped('Closed by remote'), self.subscriber_address, self.origin_address)
+	self.forward(Dropped('abandoned by remote'), self.subscriber_address, self.origin_address)
 
 	self.close_peer()
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
 	self.complete(False)
 
 def SubscriberLoop_CONNECTION_LOOPED_PeerLost(self, message):
-	self.forward(Dropped('Abandoned by peer'), self.subscriber_address, self.origin_address)
+	self.forward(Dropped('abandoned by peer'), self.subscriber_address, self.origin_address)
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
 	self.complete(False)
 
@@ -2027,28 +2032,28 @@
 		self.abort()
 		self.clearing_value = True
 		return CLEARING
 	self.complete(True)
 
 # Remote termination.
 def SubscriberLoop_RELAY_LOOPED_CloseLoop(self, message):
-	self.forward(Dropped('Closed by remote'), self.subscriber_address, self.origin_address)
+	self.forward(Dropped('abandoned by remote'), self.subscriber_address, self.origin_address)
 
 	self.close_relay()
 	self.close_peer()
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
 	self.complete(False)
 
 # Termination by loss of peer.
 def SubscriberLoop_RELAY_LOOPED_PeerLost(self, message):
-	self.forward(Dropped('Abandoned by peer'), self.subscriber_address, self.origin_address)
+	self.forward(Dropped('abandoned by peer'), self.subscriber_address, self.origin_address)
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
 	self.complete(False)
```

### Comparing `ansar-connect-0.1.136/src/ansar/connect/directory_if.py` & `ansar-connect-0.1.137/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.136/src/ansar/connect/foh_if.py` & `ansar-connect-0.1.137/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.136/src/ansar/connect/group_if.py` & `ansar-connect-0.1.137/src/ansar/connect/group_if.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,27 +31,29 @@
 
 __all__ = [
 	'GroupSettings',
 ]
 
 class GroupSettings(object):
 	def __init__(self, connect_above=None, roles=None, main_role=None, forwarding=False,
-		show_scopes=None, connect_scope=None, connect_file=None):
+		show_scopes=None, connect_scope=None, connect_file=None, SNI=None):
 		self.connect_above = connect_above or HostPort()
 		self.roles = roles
 		self.main_role = main_role
 		self.forwarding = forwarding
 		self.show_scopes = show_scopes
 		self.connect_scope = connect_scope
 		self.connect_file = connect_file
+		self.SNI = SNI
 
 GROUP_SETTINGS_SCHEMA = {
 	'connect_above': ar.Any(),
 	'roles': ar.Unicode(),
 	'main_role': ar.Unicode(),
 	'forwarding': ar.Boolean(),
 	'show_scopes': ar.Boolean(),
 	'connect_scope': ScopeOfService,
 	'connect_file': ar.Unicode(),
+	'SNI': ar.Unicode(),
 }
 
 ar.bind(GroupSettings, object_schema=GROUP_SETTINGS_SCHEMA)
```

### Comparing `ansar-connect-0.1.136/src/ansar/connect/grouping.py` & `ansar-connect-0.1.137/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.136/src/ansar/connect/moving.py` & `ansar-connect-0.1.137/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.136/src/ansar/connect/networking.py` & `ansar-connect-0.1.137/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.136/src/ansar/connect/networking_if.py` & `ansar-connect-0.1.137/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.136/src/ansar/connect/node.py` & `ansar-connect-0.1.137/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.136/src/ansar/connect/plumbing.py` & `ansar-connect-0.1.137/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.136/src/ansar/connect/procedure.py` & `ansar-connect-0.1.137/src/ansar/connect/procedure.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,15 +202,19 @@
 		e = ar.Failed(group_running=(f'group "{group}" is already running', None))
 		raise ar.Incomplete(e)
 
 	settings = hr.role_settings[2]				# From the group.
 	connect_above = settings.connect_above
 	accept_below = ar.LocalPort(0)				# Grab an ephemeral for consistency.
 
-	a = self.create(ar.ServiceDirectory, ar.ScopeOfService.GROUP, connect_above, accept_below)
+	if settings.SNI:
+		encryption_above = ar.TlsClient(SNI=settings.SNI)
+	else:
+		encryption_above = None
+	a = self.create(ar.ServiceDirectory, ar.ScopeOfService.GROUP, connect_above, accept_below, encryption_above=encryption_above)
 	self.directory = a
 
 	try:
 		# Directory responds with a HostPort.
 		m = self.select(ar.HostPort, ar.Stop)
 		if isinstance(m, ar.HostPort):
 			connect_above = m
@@ -540,15 +544,19 @@
 	settings = GroupSettings()
 	hr = hb.open_role(group_role, settings, None, ar.NodeProperties())
 
 	settings = hr.role_settings[2]				# From the group.
 	connect_above = settings.connect_above
 	accept_below = ar.LocalPort(0)				# Disabled.
 
-	a = self.create(ar.ServiceDirectory, ar.ScopeOfService.GROUP, connect_above, accept_below)
+	if settings.SNI:
+		encryption_above = ar.TlsClient(SNI=settings.SNI)
+	else:
+		encryption_above = None
+	a = self.create(ar.ServiceDirectory, ar.ScopeOfService.GROUP, connect_above, accept_below, encryption_above=encryption_above)
 	self.assign(a, None)
 	self.directory = a
 
 	try:
 		# Directory responds with a HostPort
 		# Then wait for a grace period.
 		m = self.select(ar.HostPort, ar.Stop)
```

### Comparing `ansar-connect-0.1.136/src/ansar/connect/product.py` & `ansar-connect-0.1.137/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.136/src/ansar/connect/socketry.py` & `ansar-connect-0.1.137/src/ansar/connect/socketry.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 import queue as sq
 import threading as thr
 import errno
 import socket
 import select
 import re
+import ssl
 import ansar.create as ar
 
 from copy import copy
 
 __all__ = [
 	'HostPort',
 	'LocalPort',
@@ -47,20 +48,30 @@
 	'Connected',
 	'NotListening',
 	'NotAccepted',
 	'NotConnected',
 	'Close',
 	'Closed',
 	'Abandoned',
+	'TlsServer',
+	'TlsClient',
 	'SocketSelect',
 	'SocketChannel',
 ]
 
 #
 #
+# server_context = ssl.create_default_context()
+#server_context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
+#erver_context.load_cert_chain(CERTIFICATE_FILE, keyfile=KEY_FILE)
+
+#tls_client_context = ssl.create_default_context()
+#tls_client_context.load_verify_locations(CERT)
+#
+#
 LOCAL_HOST = '127.0.0.1'
 
 class HostPort(object):
 	def __init__(self, host=None, port=None):
 		self.host = host
 		self.port = port
 	
@@ -127,37 +138,40 @@
 		self.object_type = object_type
 		self.args = args
 		self.kw = kw
 
 # Control messages sent to the sockets thread
 # via the control channel.
 class ListenForStream(object):
-	def __init__(self, requested_ipp=None, create_session=None, tag=None, upgrade=None):
+	def __init__(self, requested_ipp=None, create_session=None, tag=None, upgrade=None, encrypted=None):
 		self.requested_ipp = requested_ipp or HostPort()
 		self.create_session = create_session
 		self.tag = tag
 		self.upgrade = upgrade
+		self.encrypted = encrypted
 
 class ConnectStream(object):
-	def __init__(self, requested_ipp=None, create_session=None, tag=None, upgrade=None):
+	def __init__(self, requested_ipp=None, create_session=None, tag=None, upgrade=None, encrypted=None):
 		self.requested_ipp = requested_ipp or HostPort()
 		self.create_session = create_session
 		self.tag = tag
 		self.upgrade = upgrade
+		self.encrypted = encrypted
 
 class StopListening(object):
 	def __init__(self, listening_ipp=None):
 		self.listening_ipp = listening_ipp or HostPort()
 
 # Update messages from sockets thread to app.
 class Listening(object):
-	def __init__(self, requested_ipp=None, listening_ipp=None, tag=None):
+	def __init__(self, requested_ipp=None, listening_ipp=None, tag=None, context=None):
 		self.requested_ipp = requested_ipp or HostPort()
 		self.listening_ipp = listening_ipp or HostPort()
 		self.tag = tag
+		self.context = context
 
 class Accepted(object):
 	def __init__(self, listening_ipp=None, accepted_ipp=None, remote_address=None, opened_at=None, tag=None):
 		self.listening_ipp = listening_ipp or HostPort()
 		self.accepted_ipp = accepted_ipp or HostPort()
 		self.remote_address = remote_address
 		self.opened_at = opened_at
@@ -215,20 +229,22 @@
 	'connected_ipp': ar.UserDefined(HostPort),
 	'listening_ipp': ar.UserDefined(HostPort),
 	'accepted_ipp': ar.UserDefined(HostPort),
 	'condition': ar.Unicode(),
 	'explanation': ar.Unicode(),
 	'error_code': ar.Integer8(),
 	'error_text': ar.Unicode(),
+	'encrypted': ar.Any(),
+	'context': ar.Any(),
 }
 
 ar.bind(ListenForStream, object_schema=CONTROL_SCHEMA)
 ar.bind(ConnectStream, object_schema=CONTROL_SCHEMA)
 ar.bind(StopListening, object_schema=CONTROL_SCHEMA)
-ar.bind(Listening, object_schema=CONTROL_SCHEMA)
+ar.bind(Listening, object_schema=CONTROL_SCHEMA, copy_before_sending=False)
 ar.bind(Accepted, object_schema=CONTROL_SCHEMA)
 ar.bind(Connected, object_schema=CONTROL_SCHEMA)
 ar.bind(NotListening, object_schema=CONTROL_SCHEMA)
 ar.bind(NotAccepted, object_schema=CONTROL_SCHEMA)
 ar.bind(NotConnected, object_schema=CONTROL_SCHEMA)
 
 # Session termination messages. Handshake between app
@@ -267,14 +283,27 @@
 	'closed_at': ar.WorldTime(),
 }
 
 ar.bind(Close, object_schema=ENDING_SCHEMA, copy_before_sending=False)
 ar.bind(Closed, object_schema=ENDING_SCHEMA, copy_before_sending=False)
 ar.bind(Abandoned, object_schema=ENDING_SCHEMA, copy_before_sending=False)
 
+#
+#
+class TlsServer(object):
+	def __init__(self, certificate_file=None, key_file=None):
+		self.certificate_file = certificate_file
+		self.key_file = key_file
+
+class TlsClient(object):
+	def __init__(self, SNI=None):
+		self.SNI = SNI
+
+#
+#
 class Shutdown(object):
 	def __init__(self, s=None, value=False):
 		self.s = s
 		self.value = value
 
 class Bump(object):
 	def __init__(self, s=None):
@@ -682,15 +711,21 @@
 
 	hap = server.getsockname()
 
 	self.trace('Listening on "%s"(%d), requested "%s"(%d)' %
 		(hap[0], hap[1],
 		requested_ipp.host, requested_ipp.port))
 
-	listening = Listening(requested_ipp, HostPort(hap[0], hap[1]), m.tag)
+	if isinstance(m.encrypted, TlsServer):
+		context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
+		context.load_cert_chain(m.encrypted.certificate_file, keyfile=m.encrypted.key_file)
+		self.trace(f'Encrypting as TLS server "{m.encrypted.certificate_file}"')
+	else:
+		context = None
+	listening = Listening(requested_ipp=requested_ipp, listening_ipp=HostPort(hap[0], hap[1]), tag=m.tag, context=context)
 
 	self.networking[server] = TcpServer(server, m, listening, r, m.upgrade)
 	self.receiving.append(server)
 	self.faulting.append(server)
 
 	self.send(listening, r)
 
@@ -731,14 +766,19 @@
 	try:
 		client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 		client.setblocking(False)
 	except socket.error as e:
 		self.send(NotConnected(requested_ipp, e.errno, str(e), m.tag), r)
 		return
 
+	if isinstance(m.encrypted, TlsClient):
+		context = ssl.create_default_context()
+		client = context.wrap_socket(client, server_side=False, do_handshake_on_connect=False, server_hostname=m.encrypted.SNI)
+		self.trace(f'Encrypting as TLS client "{m.encrypted.SNI}"')
+
 	def client_not_connected(e):
 		client.close()
 		self.send(NotConnected(requested_ipp, e.errno, str(e), m.tag), r)
 
 	try:
 		e = client.connect_ex(requested_ipp.inet())
 		if e:
@@ -876,14 +916,17 @@
 	try:
 		accepted, hap = s.accept()
 		accepted.setblocking(False)
 	except socket.error as e:
 		self.send(NotAccepted(listening.requested_ipp, e.errno, str(e), listening.tag), server.controller_address)
 		return
 
+	if listening.context:
+		accepted = listening.context.wrap_socket(accepted, server_side=True, do_handshake_on_connect=False)
+
 	self.trace( 'Accepted "%s"(%d), server at "%s"(%d)' %
 				   (hap[0], hap[1],
 				   listening.listening_ipp.host, listening.listening_ipp.port))
 
 	opened_at = ar.world_now()
 	stream, proxy_address = open_stream(self, server, accepted, None)
 	self.receiving.append(accepted)
@@ -953,14 +996,17 @@
 		try:
 			stream.receive_and_route(scrap, self)
 		except (ar.CodecFailed, OverflowError, ValueError) as e:
 			value = ar.Faulted(condition='cannot start inbound', explanation=str(e))
 			close_session(stream, value, s)
 		return
 
+	except ssl.SSLError as e:
+		self.trace(f'SSL error "{e}" (in receive event for incomplete connect)')
+		return
 	except socket.error as e:
 		self.send(NotConnected(request.requested_ipp, e.errno, str(e), request.tag), selector.controller_address)
 		self.clear(s, TcpClient)
 		#self.send(NotConnected(request.requested_ipp, e.errno, str(e), request.tag), stream.controller_address)
 		#self.send(ar.Stop(), stream.remote_address)
 		#self.clear(s, TcpStream)
 		return
@@ -1027,14 +1073,19 @@
 		if stream.send_a_block(s):
 			return
 	except (ar.CodecFailed, OverflowError, ValueError) as e:
 		value = ar.Faulted(condition='cannot stream outbound', explanation=str(e))
 		self.warning(str(value))
 		close_session(stream, value, s)
 		return
+	except ssl.SSLError as e:
+		# Seems to occur as a natural part of negotiation.
+		# self.trace(f'SSL error [2] "{e}"')
+		return
+
 	try:
 		self.sending.remove(s)
 	except KeyError:
 		pass
 
 # A network transport for the purpose of exchanging
 # messages between machines.
@@ -1050,14 +1101,18 @@
 			stream.receive_and_route(scrap, self)
 		except (ar.CodecFailed, OverflowError, ValueError) as e:
 			value = ar.Faulted(condition='cannot stream inbound', explanation=str(e))
 			self.warning(str(value))
 			close_session(stream, value, s)
 		return
 
+	except ssl.SSLError as e:
+		# Seems to occur as a natural part of negotiation.
+		# self.trace(f'SSL error [3] "{e}"')
+		return
 	except socket.error as e:
 		if e.errno == errno.ECONNREFUSED:
 			self.fault('Unexpected connection refused')
 		elif e.errno not in SOCKET_DOWN:
 			self.fault('Unexpected socket termination [%d] %s' % (e.errno, e.strerror))
 		end_of_session(self, stream, s)
 		return
```

### Comparing `ansar-connect-0.1.136/src/ansar/connect/standard.py` & `ansar-connect-0.1.137/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.136/src/ansar/connect/transporting.py` & `ansar-connect-0.1.137/src/ansar/connect/transporting.py`

 * *Files 19% similar despite different names*

```diff
@@ -44,22 +44,22 @@
 	channel.send(ar.Stop(), root.address)
 	root.select(ar.Completed)
 
 ar.AddOn(create_sockets, stop_sockets)
 
 #
 #
-def connect(self, requested_ipp, session=None, tag=None):
+def connect(self, requested_ipp, session=None, tag=None, encrypted=None):
 	global sockets, channel
-	channel.send(ConnectStream(requested_ipp, session, tag), self.address)
+	channel.send(ConnectStream(requested_ipp=requested_ipp, create_session=session, tag=tag, encrypted=encrypted), self.address)
 
 #
 #
-def listen(self, requested_ipp, session=None, tag=None):
+def listen(self, requested_ipp, session=None, tag=None, encrypted=None):
 	global sockets, channel
-	channel.send(ListenForStream(requested_ipp, session, tag), self.address)
+	channel.send(ListenForStream(requested_ipp=requested_ipp, create_session=session, tag=tag, encrypted=encrypted), self.address)
 
 #
 #
 def stop_listen(self, requested_ipp):
 	global sockets, channel
 	channel.send(StopListening(requested_ipp), self.address)
```

### Comparing `ansar-connect-0.1.136/src/ansar/connect/wan.py` & `ansar-connect-0.1.137/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.136/src/ansar_connect.egg-info/PKG-INFO` & `ansar-connect-0.1.137/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.136
+Version: 0.1.137
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-connect-0.1.136/src/ansar_connect.egg-info/SOURCES.txt` & `ansar-connect-0.1.137/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

