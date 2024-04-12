# Comparing `tmp/ansar-connect-0.1.137.tar.gz` & `tmp/ansar-connect-0.1.138.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar-connect-0.1.137.tar", last modified: Fri Apr 12 00:43:55 2024, max compression
+gzip compressed data, was "ansar-connect-0.1.138.tar", last modified: Fri Apr 12 03:05:03 2024, max compression
```

## Comparing `ansar-connect-0.1.137.tar` & `ansar-connect-0.1.138.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 00:43:55.840062 ansar-connect-0.1.137/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar-connect-0.1.137/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-12 00:43:55.840062 ansar-connect-0.1.137/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar-connect-0.1.137/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar-connect-0.1.137/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-12 00:43:55.840062 ansar-connect-0.1.137/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar-connect-0.1.137/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 00:43:55.840062 ansar-connect-0.1.137/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 00:43:55.840062 ansar-connect-0.1.137/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 00:43:55.840062 ansar-connect-0.1.137/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14427 2024-03-29 02:37:30.000000 ansar-connect-0.1.137/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3562 2024-04-11 23:48:03.000000 ansar-connect-0.1.137/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10088 2024-04-11 23:51:57.000000 ansar-connect-0.1.137/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9236 2024-04-12 00:33:17.000000 ansar-connect-0.1.137/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 00:43:55.840062 ansar-connect-0.1.137/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3055 2024-04-12 00:43:52.000000 ansar-connect-0.1.137/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    13941 2024-04-11 23:33:25.000000 ansar-connect-0.1.137/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    77714 2024-04-11 23:32:28.000000 ansar-connect-0.1.137/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar-connect-0.1.137/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar-connect-0.1.137/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar-connect-0.1.137/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar-connect-0.1.137/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar-connect-0.1.137/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar-connect-0.1.137/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar-connect-0.1.137/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar-connect-0.1.137/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar-connect-0.1.137/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    37547 2024-04-11 23:51:57.000000 ansar-connect-0.1.137/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2323 2024-03-29 22:32:03.000000 ansar-connect-0.1.137/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    38262 2024-04-11 01:07:01.000000 ansar-connect-0.1.137/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar-connect-0.1.137/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2205 2024-04-11 00:02:31.000000 ansar-connect-0.1.137/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6367 2024-04-07 03:37:54.000000 ansar-connect-0.1.137/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 00:43:55.840062 ansar-connect-0.1.137/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-12 00:43:55.000000 ansar-connect-0.1.137/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-12 00:43:55.000000 ansar-connect-0.1.137/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-12 00:43:55.000000 ansar-connect-0.1.137/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-12 00:43:55.000000 ansar-connect-0.1.137/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-12 00:43:55.000000 ansar-connect-0.1.137/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-12 00:43:55.000000 ansar-connect-0.1.137/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 03:05:03.254572 ansar-connect-0.1.138/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar-connect-0.1.138/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-12 03:05:03.254572 ansar-connect-0.1.138/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar-connect-0.1.138/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar-connect-0.1.138/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-12 03:05:03.254572 ansar-connect-0.1.138/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar-connect-0.1.138/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 03:05:03.250573 ansar-connect-0.1.138/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 03:05:03.250573 ansar-connect-0.1.138/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 03:05:03.250573 ansar-connect-0.1.138/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14427 2024-03-29 02:37:30.000000 ansar-connect-0.1.138/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3554 2024-04-12 02:38:54.000000 ansar-connect-0.1.138/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10084 2024-04-12 02:38:59.000000 ansar-connect-0.1.138/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9228 2024-04-12 02:39:03.000000 ansar-connect-0.1.138/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 03:05:03.254572 ansar-connect-0.1.138/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3055 2024-04-12 03:05:00.000000 ansar-connect-0.1.138/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14046 2024-04-12 02:39:06.000000 ansar-connect-0.1.138/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    78172 2024-04-12 02:39:12.000000 ansar-connect-0.1.138/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar-connect-0.1.138/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar-connect-0.1.138/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar-connect-0.1.138/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar-connect-0.1.138/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar-connect-0.1.138/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar-connect-0.1.138/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar-connect-0.1.138/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar-connect-0.1.138/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar-connect-0.1.138/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    37539 2024-04-12 02:39:15.000000 ansar-connect-0.1.138/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2323 2024-03-29 22:32:03.000000 ansar-connect-0.1.138/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    38262 2024-04-11 01:07:01.000000 ansar-connect-0.1.138/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar-connect-0.1.138/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2205 2024-04-11 00:02:31.000000 ansar-connect-0.1.138/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6465 2024-04-12 01:38:18.000000 ansar-connect-0.1.138/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-12 03:05:03.254572 ansar-connect-0.1.138/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-12 03:05:03.000000 ansar-connect-0.1.138/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-12 03:05:03.000000 ansar-connect-0.1.138/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-12 03:05:03.000000 ansar-connect-0.1.138/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-12 03:05:03.000000 ansar-connect-0.1.138/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-12 03:05:03.000000 ansar-connect-0.1.138/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-12 03:05:03.000000 ansar-connect-0.1.138/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar-connect-0.1.137/LICENSE` & `ansar-connect-0.1.138/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.137/PKG-INFO` & `ansar-connect-0.1.138/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.137
+Version: 0.1.138
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-connect-0.1.137/README.md` & `ansar-connect-0.1.138/README.md`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.137/pyproject.toml` & `ansar-connect-0.1.138/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.137/setup.py` & `ansar-connect-0.1.138/setup.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.137/src/ansar/command/ansar_command.py` & `ansar-connect-0.1.138/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.137/src/ansar/command/ansar_directory.py` & `ansar-connect-0.1.138/src/ansar/command/ansar_directory.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,25 +50,25 @@
 }
 
 ar.bind(Settings, object_schema=SETTINGS_SCHEMA)
 
 # Just need an object to stay "on duty" while the 
 # global ServiceDirectory does its work.
 def directory(self, settings):
-	encryption_above = None
-	encryption_below = None
+	encrypted_above = None
+	encrypted_below = None
 
 	if settings.SNI:
-		encryption_above = ar.TlsClient(SNI=settings.SNI)
+		encrypted_above = ar.TlsClient(SNI=settings.SNI)
 	if settings.certificate_file and settings.key_file:
-		encryption_below = ar.TlsServer(certificate_file=settings.certificate_file, key_file=settings.key_file)
+		encrypted_below = ar.TlsServer(certificate_file=settings.certificate_file, key_file=settings.key_file)
 
 	a = self.create(ar.ServiceDirectory, settings.directory_scope,
 		settings.connect_above, settings.accept_below,
-		encryption_above=encryption_above, encryption_below=encryption_below)
+		encrypted_above=encrypted_above, encrypted_below=encrypted_below)
 	m = self.select(ar.HostPort, ar.Completed, ar.Stop)
 	if isinstance(m, ar.Completed):
 		return m.value
 	elif isinstance(m, ar.Stop):
 		self.send(m, a)
 		self.select(ar.Completed)
 		return ar.Aborted()
```

### Comparing `ansar-connect-0.1.137/src/ansar/command/ansar_group.py` & `ansar-connect-0.1.138/src/ansar/command/ansar_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,18 +197,18 @@
 		if hb.role_exists(self.main_role):
 			tr = hb.open_role(self.main_role, None, None, ar.NodeProperties())
 			if series(hr.properties.retry) or series(tr.properties.retry):
 				r = ar.Rejected(forwarding_retry=(f'main role "{self.main_role}" is configured to retry', 'not supported'))
 				self.complete(r)
 
 	if self.settings.SNI:
-		encryption_above = ar.TlsClient(SNI=self.settings.SNI)
+		encrypted_above = ar.TlsClient(SNI=self.settings.SNI)
 	else:
-		encryption_above = None
-	a = self.create(ar.ServiceDirectory, ar.ScopeOfService.GROUP, connect_above, accept_below, encryption_above=encryption_above)
+		encrypted_above = None
+	a = self.create(ar.ServiceDirectory, ar.ScopeOfService.GROUP, connect_above, accept_below, encrypted_above=encrypted_above)
 	self.assign(a, None)
 	self.directory = a
 	return OPENING
 
 def Group_OPENING_HostPort(self, message):
 	self.directory_ipp = message
 	self.group_start = ar.world_now()
```

### Comparing `ansar-connect-0.1.137/src/ansar/command/shared_directory.py` & `ansar-connect-0.1.138/src/ansar/command/shared_directory.py`

 * *Files 11% similar despite different names*

```diff
@@ -80,19 +80,19 @@
 	self.store = store
 	self.recover = recover
 
 	# Initial load.
 	self.recover()
 
 	settings = self.settings
-	encryption = None
+	encrypted = None
 	if settings.certificate_file and settings.key_file:
-		encryption = ar.TlsServer(certificate_file=settings.certificate_file, key_file=settings.key_file)
+		encrypted = ar.TlsServer(certificate_file=settings.certificate_file, key_file=settings.key_file)
 
-	ar.listen(self, self.settings.public_access, encryption=encryption)
+	ar.listen(self, self.settings.public_access, encrypted=encrypted)
 	return STARTING
 
 # Verify access
 def ProductDirectory_STARTING_Listening(self, message):
 	self.public_access = message
 	return READY
 
@@ -173,23 +173,23 @@
 			self.trace(f'Unknown upward key "{k}" for child [{r}]')
 			# Default upward access is disabled but a hint that it
 			# should adopt the same nature.
 			c = ProductAccess(product_name=product_name, product_instance=product_instance)
 			self.connect_above[k] = c
 			self.store()
 
-		encryption_above = None
+		encrypted_above = None
 		if settings.SNI:
-			encryption_above = ar.TlsClient(SNI=settings.SNI)
+			encrypted_above = ar.TlsClient(SNI=settings.SNI)
 
 		d = self.create(ar.ServiceDirectory,
 			scope=settings.directory_scope,			# All at same scope.
 			connect_above=c,
 			accept_below=ar.HostPort(),				# Disabled.
-			encryption_above=encryption_above)
+			encrypted_above=encrypted_above)
 
 		self.assign(d, k)
 		self.directory[k] = d
 
 	self.child_of[r] = d
 	accepted = self.accepted.get(r)
 	if accepted:
```

### Comparing `ansar-connect-0.1.137/src/ansar/connect/__init__.py` & `ansar-connect-0.1.138/src/ansar/connect/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 58eb33b821cd0a8737502a52624c6715473ceee2
-Version: 0.1.136 (2024-04-12@12:43:52+NZST)
+Commit: 2a7262bc028b519a13fcedc25aaeafdd7db8368e
+Version: 0.1.137 (2024-04-12@15:05:00+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar-connect-0.1.137/src/ansar/connect/connect_directory.py` & `ansar-connect-0.1.138/src/ansar/connect/connect_directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,21 +48,21 @@
 class GLARING: pass
 class CONNECTING: pass
 class REDIRECTING: pass
 class ASSIGNING: pass
 class CLOSING: pass
 
 class ConnectToDirectory(ar.Point, ar.StateMachine):
-	def __init__(self, connect_above, session=None, group_address=None, encryption=None):
+	def __init__(self, connect_above, session=None, group_address=None, encrypted=None):
 		ar.Point.__init__(self)
 		ar.StateMachine.__init__(self, INITIAL)
 		self.connect_above = connect_above
 		self.session = session
 		self.group_address = group_address
-		self.encryption = encryption
+		self.encrypted = encrypted
 
 		self.started = None
 		self.attempts = 0
 
 		self.connected = None
 		self.remote = None
 		self.redirect = None
@@ -83,15 +83,15 @@
 			ipp = c.access_ipp
 			next = CLOUDY
 		else:
 			return DISABLED
 
 		if ipp.host is None:
 			return DISABLED
-		connect(self, ipp, session=self.session, encryption=self.encryption)
+		connect(self, ipp, session=self.session, encrypted=self.encrypted)
 		self.start(ar.T1, seconds=8.0)
 		return next
 
 	def reschedule(self):
 		if self.intervals is None:
 			c = self.connect_above
 			if isinstance(c, HostPort):
@@ -266,15 +266,20 @@
 	# Connected could be orphaned here.
 	self.complete(ar.Aborted())
 
 def ConnectToDirectory_LOOKING_WideAreaRedirect(self, message):
 	self.redirect = message
 	ipp = message.redirect_ipp
 	self.trace(f'Redirecting from FOH to WAN ({ipp})')
-	connect(self, ipp)
+	if message.SNI:
+		encrypted = ar.TlsClient(message.SNI)
+		connect(self, ipp, encrypted=encrypted)
+	else:
+		connect(self, ipp)
+		
 	self.reply(Close())
 	return REDIRECTING
 
 def ConnectToDirectory_LOOKING_Faulted(self, message):
 	self.trace(f'Access denied - {message}')
 	self.send(Close(message), self.connected.remote_address)
 	if self.reschedule():
```

### Comparing `ansar-connect-0.1.137/src/ansar/connect/directory.py` & `ansar-connect-0.1.138/src/ansar/connect/directory.py`

 * *Files 2% similar despite different names*

```diff
@@ -372,17 +372,18 @@
 ar.bind(InboundOverAccepted, object_schema=IO_SCHEMA)
 ar.bind(RouteByRelay, object_schema=IO_SCHEMA)
 ar.bind(InboundByRelay, object_schema=IO_SCHEMA)
 
 #
 #
 class OpenPeer(object):
-	def __init__(self, connecting_ipp=None, key=None):
+	def __init__(self, connecting_ipp=None, key=None, encrypted=None):
 		self.connecting_ipp = connecting_ipp or HostPort()
 		self.key = key
+		self.encrypted = encrypted
 
 class PeerOpened(object):
 	def __init__(self, connecting_ipp=None, key=None):
 		self.connecting_ipp = connecting_ipp or HostPort()
 		self.key = key
 
 class NotPeered(object):
@@ -401,14 +402,15 @@
 		self.connecting_ipp = connecting_ipp or HostPort()
 		self.key = key
 
 PEER_SCHEMA = {
 	'connecting_ipp': ar.UserDefined(HostPort),
 	'key': str,
 	'reason': str,
+	'encrypted': ar.Any(),
 }
 
 ar.bind(OpenPeer, object_schema=PEER_SCHEMA)
 ar.bind(PeerOpened, object_schema=PEER_SCHEMA)
 ar.bind(NotPeered, object_schema=PEER_SCHEMA)
 ar.bind(PeerLost, object_schema=PEER_SCHEMA)
 ar.bind(ClosePeer, object_schema=PEER_SCHEMA)
@@ -498,22 +500,22 @@
 			return False
 	return True
 
 CONNECT_ABOVE = 'connect-above'
 ACCEPT_BELOW = 'accept-below'
 
 class ServiceDirectory(ar.Threaded, ar.StateMachine):
-	def __init__(self, scope=None, connect_above=None, accept_below=None, encryption_above=None, encryption_below=None):
+	def __init__(self, scope=None, connect_above=None, accept_below=None, encrypted_above=None, encrypted_below=None):
 		ar.Threaded.__init__(self)
 		ar.StateMachine.__init__(self, INITIAL)
 		self.scope = scope or ScopeOfService.PROCESS
 		self.connect_above = connect_above
 		self.accept_below = accept_below or HostPort()
-		self.encryption_above = encryption_above
-		self.encryption_below = encryption_below
+		self.encrypted_above = encrypted_above
+		self.encrypted_below = encrypted_below
 		self.ctd = None
 		self.directory = {}
 		self.find = {}
 		self.matched = {}
 		self.connected_up = None
 		self.not_connected = None
 		self.connected = None
@@ -773,23 +775,23 @@
 def ServiceDirectory_INITIAL_Start(self, message):
 	self.started = ar.world_now()
 
 	self.trace(f'Scope of {ScopeOfService.to_name(self.scope)}')
 	self.trace(f'Connecting up to "{ar.tof(self.connect_above)}"')
 	self.trace(f'Listening below at "{ar.tof(self.accept_below)}"')
 
-	self.ctd = self.create(ConnectToDirectory, self.connect_above, encryption=self.encryption_above)
+	self.ctd = self.create(ConnectToDirectory, self.connect_above, encrypted=self.encrypted_above)
 	self.assign(self.ctd, CONNECT_ABOVE)
 
 	# Acceptance of connections from lower directories.
 	if isinstance(self.accept_below, HostPort):
 		if self.accept_below.host is None:
 			self.send(HostPort(host=None), self.parent_address)
 		else:
-			listen(self, self.accept_below, tag='directory-accept', encryption=self.encryption_below)
+			listen(self, self.accept_below, tag='directory-accept', encrypted=self.encrypted_below)
 			return OPENING
 	else:
 		pass	# Acceptance arranged externally. May be a
 				# Listening object for diagnosis.
 
 	return NORMAL
 
@@ -1375,15 +1377,20 @@
 		n = len(r[1])
 		self.trace(f'Peer for relay "{key}" already known ({n} routes pending)')
 	except KeyError:
 		r = [None, {key: relay}]
 		self.peered[k] = r
 
 		self.trace(f'Opening peer "{k}" (relay {key})')
-		self.send(OpenPeer(ipp, key), pb.house)
+		if message.redirect.SNI:
+			encrypted = ar.TlsClient(SNI=message.redirect.SNI)
+			open = OpenPeer(ipp, key, encrypted=encrypted)
+		else:
+			open = OpenPeer(ipp, key)
+		self.send(open, pb.house)
 		return READY
 
 	if r[0] is None:
 		return READY
 
 	self.send(relay, r[0])
 	self.relay_address[key] = r[0]
@@ -1628,15 +1635,20 @@
 		self.start(ar.T2, SECONDS_OF_PEERING)
 
 	def open_relay(self):
 		key = self.route.key
 		ipp = self.route.redirect.redirect_ipp
 		self.peer_ipp = ipp
 		self.trace(f'Requests relay {ipp} for "{key}"')
-		self.send(OpenPeer(ipp, key), pb.house)
+		if self.route.redirect.SNI:
+			encrypted = ar.TlsClient(SNI=self.route.redirect.SNI)
+			open = OpenPeer(ipp, key, encrypted=encrypted)
+		else:
+			open = OpenPeer(ipp, key)
+		self.send(open, pb.house)
 		self.start(ar.T2, SECONDS_OF_PEERING)
 
 	def open_latch(self, message):
 		self.remote_loop = self.return_address
 		self.remote_session = message.publisher_session
 		if self.create_session:
 			cs = self.create_session
@@ -2342,26 +2354,27 @@
 
 # WARNING agent and loop MUST be on same thread.
 ar.bind(SubscriptionAgent, SUBSCRIPTION_AGENT_DISPATCH, thread='subscribed')
 
 #
 #
 class ConnectToPeer(ar.Point, ar.StateMachine):
-	def __init__(self, connecting_ipp, key, client_address):
+	def __init__(self, connecting_ipp, key, client_address, encrypted):
 		ar.Point.__init__(self)
 		ar.StateMachine.__init__(self, INITIAL)
 		self.connecting_ipp = connecting_ipp
 		self.key = key
 		self.connected = None
 		self.not_connected = None
 		self.client_address = set()
 		self.client_address.add(client_address)
+		self.encrypted = encrypted
 
 def ConnectToPeer_INITIAL_Start(self, message):
-	connect(self, self.connecting_ipp)
+	connect(self, self.connecting_ipp, encrypted=self.encrypted)
 	return CONNECTING
 
 # CONNECTING
 #
 def ConnectToPeer_CONNECTING_Connected(self, message):
 	self.connected = message
 
@@ -2551,15 +2564,15 @@
 		self.warning(f'Completion of unknown type {type(m)}')
 	return NORMAL
 
 def PubSub_NORMAL_OpenPeer(self, message):
 	inet = message.connecting_ipp.inet()
 	connecting = self.connecting.get(inet, None)
 	if connecting is None:
-		connecting = self.create(ConnectToPeer, message.connecting_ipp, message.key, self.return_address)
+		connecting = self.create(ConnectToPeer, message.connecting_ipp, message.key, self.return_address, message.encrypted)
 		p = [message.connecting_ipp, self.return_address]
 		self.assign(connecting, p)
 		self.connecting[inet] = connecting
 	else:
 		self.forward(message, connecting, self.return_address)
 	return NORMAL
```

### Comparing `ansar-connect-0.1.137/src/ansar/connect/directory_if.py` & `ansar-connect-0.1.138/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.137/src/ansar/connect/foh_if.py` & `ansar-connect-0.1.138/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.137/src/ansar/connect/group_if.py` & `ansar-connect-0.1.138/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.137/src/ansar/connect/grouping.py` & `ansar-connect-0.1.138/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.137/src/ansar/connect/moving.py` & `ansar-connect-0.1.138/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.137/src/ansar/connect/networking.py` & `ansar-connect-0.1.138/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.137/src/ansar/connect/networking_if.py` & `ansar-connect-0.1.138/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.137/src/ansar/connect/node.py` & `ansar-connect-0.1.138/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.137/src/ansar/connect/plumbing.py` & `ansar-connect-0.1.138/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.137/src/ansar/connect/procedure.py` & `ansar-connect-0.1.138/src/ansar/connect/procedure.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,18 +203,18 @@
 		raise ar.Incomplete(e)
 
 	settings = hr.role_settings[2]				# From the group.
 	connect_above = settings.connect_above
 	accept_below = ar.LocalPort(0)				# Grab an ephemeral for consistency.
 
 	if settings.SNI:
-		encryption_above = ar.TlsClient(SNI=settings.SNI)
+		encrypted_above = ar.TlsClient(SNI=settings.SNI)
 	else:
-		encryption_above = None
-	a = self.create(ar.ServiceDirectory, ar.ScopeOfService.GROUP, connect_above, accept_below, encryption_above=encryption_above)
+		encrypted_above = None
+	a = self.create(ar.ServiceDirectory, ar.ScopeOfService.GROUP, connect_above, accept_below, encrypted_above=encrypted_above)
 	self.directory = a
 
 	try:
 		# Directory responds with a HostPort.
 		m = self.select(ar.HostPort, ar.Stop)
 		if isinstance(m, ar.HostPort):
 			connect_above = m
@@ -545,18 +545,18 @@
 	hr = hb.open_role(group_role, settings, None, ar.NodeProperties())
 
 	settings = hr.role_settings[2]				# From the group.
 	connect_above = settings.connect_above
 	accept_below = ar.LocalPort(0)				# Disabled.
 
 	if settings.SNI:
-		encryption_above = ar.TlsClient(SNI=settings.SNI)
+		encrypted_above = ar.TlsClient(SNI=settings.SNI)
 	else:
-		encryption_above = None
-	a = self.create(ar.ServiceDirectory, ar.ScopeOfService.GROUP, connect_above, accept_below, encryption_above=encryption_above)
+		encrypted_above = None
+	a = self.create(ar.ServiceDirectory, ar.ScopeOfService.GROUP, connect_above, accept_below, encrypted_above=encrypted_above)
 	self.assign(a, None)
 	self.directory = a
 
 	try:
 		# Directory responds with a HostPort
 		# Then wait for a grace period.
 		m = self.select(ar.HostPort, ar.Stop)
```

### Comparing `ansar-connect-0.1.137/src/ansar/connect/product.py` & `ansar-connect-0.1.138/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.137/src/ansar/connect/socketry.py` & `ansar-connect-0.1.138/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.137/src/ansar/connect/standard.py` & `ansar-connect-0.1.138/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.137/src/ansar/connect/transporting.py` & `ansar-connect-0.1.138/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.137/src/ansar/connect/wan.py` & `ansar-connect-0.1.138/src/ansar/connect/wan.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,18 +110,19 @@
 		self.account_id = account_id
 		self.directory_id = directory_id
 		self.access_token = access_token
 		self.product_name = product_name
 		self.product_instance = product_instance
 
 class WideAreaRedirect(object):
-	def __init__(self, redirect_ipp=None, directory_id=None, assignment_token=None):
+	def __init__(self, redirect_ipp=None, directory_id=None, assignment_token=None, SNI=None):
 		self.redirect_ipp = redirect_ipp or HostPort()
 		self.directory_id = directory_id
 		self.assignment_token = assignment_token
+		self.SNI = SNI
 
 class WideAreaAssignment(object):
 	def __init__(self, directory_id=None, assignment_token=None):
 		self.directory_id = directory_id
 		self.assignment_token = assignment_token
 
 class YourWideArea(object):
@@ -134,14 +135,15 @@
 	"account_id": ar.UUID(),
 	"directory_id": ar.UUID(),
 	"redirect_ipp": ar.UserDefined(HostPort),
 	"assignment_token": ar.UUID(),
 	"address": ar.Address(),
 	"product_name": ar.Unicode(),
 	"product_instance": InstanceOfProduct,
+	"SNI": ar.Unicode(),
 }
 
 ar.bind(WideAreaAccess, object_schema=WIDE_AREA_SCHEMA)
 ar.bind(WideAreaLookup, object_schema=WIDE_AREA_SCHEMA)
 ar.bind(WideAreaRedirect, object_schema=WIDE_AREA_SCHEMA)
 ar.bind(WideAreaAssignment, object_schema=WIDE_AREA_SCHEMA)
 ar.bind(YourWideArea, object_schema=WIDE_AREA_SCHEMA)
@@ -150,18 +152,19 @@
 # a publisher.
 class RelayLookup(object):
 	def __init__(self, relay_id=None, directory_id=None):
 		self.relay_id = relay_id
 		self.directory_id = directory_id
 
 class RelayRedirect(object):
-	def __init__(self, redirect_ipp=None, relay_id=None, assignment_token=None):
+	def __init__(self, redirect_ipp=None, relay_id=None, assignment_token=None, SNI=None):
 		self.redirect_ipp = redirect_ipp or HostPort()
 		self.relay_id = relay_id
 		self.assignment_token = assignment_token
+		self.SNI = SNI
 
 class RelayAssignment(object):
 	def __init__(self, relay_id=None, assignment_token=None):
 		self.relay_id = relay_id
 		self.assignment_token = assignment_token
 
 class YourRelay(object):
@@ -175,14 +178,15 @@
 RELAY_SCHEMA = {
 	"relay_id": ar.UUID(),
 	"directory_id": ar.UUID(),
 	"redirect_ipp": ar.UserDefined(HostPort),
 	"assignment_token": ar.UUID(),
 	"address": ar.Address(),
 	"account_id": ar.UUID(),
+	"SNI": ar.Unicode(),
 }
 
 ar.bind(RelayLookup, object_schema=RELAY_SCHEMA)
 ar.bind(RelayRedirect, object_schema=RELAY_SCHEMA)
 ar.bind(RelayAssignment, object_schema=RELAY_SCHEMA)
 ar.bind(YourRelay, object_schema=RELAY_SCHEMA)
```

### Comparing `ansar-connect-0.1.137/src/ansar_connect.egg-info/PKG-INFO` & `ansar-connect-0.1.138/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.137
+Version: 0.1.138
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-connect-0.1.137/src/ansar_connect.egg-info/SOURCES.txt` & `ansar-connect-0.1.138/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

