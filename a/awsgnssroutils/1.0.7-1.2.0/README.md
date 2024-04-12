# Comparing `tmp/awsgnssroutils-1.0.7.tar.gz` & `tmp/awsgnssroutils-1.2.0.tar.gz`

## Comparing `awsgnssroutils-1.0.7.tar` & `awsgnssroutils-1.2.0.tar`

### file list

```diff
@@ -1,6 +1,24 @@
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.7/src/awsgnssroutils/__init__.py
--rw-r--r--   0        0        0    50569 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.7/src/awsgnssroutils/database.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.7/LICENSE
--rw-r--r--   0        0        0     7757 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.7/README.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     8470 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/config.yaml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/__init__.py
+-rw-r--r--   0        0        0    50883 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/database.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/__init__.py
+-rw-r--r--   0        0        0    18371 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/rotcol.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/__init__.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/awsro.py
+-rwxr-xr-x   0        0        0     8082 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/brute_force.py
+-rw-r--r--   0        0        0    11946 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/celestrak.py
+-rwxr-xr-x   0        0        0    23003 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/collocation.py
+-rwxr-xr-x   0        0        0     6273 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/constants_and_utils.py
+-rw-r--r--   0        0        0    14615 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/eumetsat.py
+-rw-r--r--   0        0        0    19255 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/nadir_satellite.py
+-rw-r--r--   0        0        0    15639 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/nasa_earthdata.py
+-rwxr-xr-x   0        0        0    10076 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/rotation_collocation.py
+-rw-r--r--   0        0        0    18531 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/spacetrack.py
+-rw-r--r--   0        0        0    27555 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/timestandards.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/instruments/__init__.py
+-rw-r--r--   0        0        0    12623 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/instruments/amsua.py
+-rw-r--r--   0        0        0    13134 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/instruments/atms.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/LICENSE
+-rw-r--r--   0        0        0    17356 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/README.md
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    18290 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/PKG-INFO
```

### Comparing `awsgnssroutils-1.0.7/src/awsgnssroutils/database.py` & `awsgnssroutils-1.2.0/src/awsgnssroutils/database.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """database.py
 
 Authors: Amy McVey (amcvey@aer.com) and Stephen Leroy (sleroy@aer.com)
 Date: 10 January 2024
 
 ================================================================================
 
-This module contains utilities to query the AWS Registry of Open Data repository
+This module contains utilities to query the AWS Registry of Open Data metadata_root
 of GNSS radio occultation data. It does so using database files posted in the
-AWS repository.
+AWS metadata_root.
 
 Functionality
 =============
 This module defines two classes: RODatabaseClient and OccList. The first
 creates a portal to a database of RO metadata, and the second is an instance
 of a list of radio occultations (ROs). Each are described below.
 
 RODatabaseClient:
     Create an instance of a portal to a metadata on all RO data in the AWS
-    Registry of Open Data. It provides an option to create a repository of
-    the RO metadata on the local file system as keyword "repository".
+    Registry of Open Data. It provides an option to create a metadata_root of
+    the RO metadata on the local file system as keyword "metadata_root".
 
 OccList:
     An instance of the class OccList is contains the metadata on a list of RO
     soundings along with pointers to the RO data files in the AWS Registry of
     Open Data S3 bucket. AWS functionality is completely embedded in the
     methods of the OccList class. Those methods include the ability to
     subset/filter the list according to geolocation and time,
@@ -32,58 +32,51 @@
     restoration by RODatabaseClient.restore, and even download RO data files.
 
 Very useful utilities...
 
 setdefaults: 
     A function that sets defaults for use of RODatabaseClient and OccList. 
     It allows the user to specify defaults for storage of RO metadata 
-    database files ("repository") and for downloads of RO data files 
-    ("rodata"). In doing so, the user won't have to specify the repository 
+    database files ("metadata_root") and for downloads of RO data files 
+    ("data_root"). In doing so, the user won't have to specify the metadata_root 
     every time an instance of RODatabaseClient is created nor specify a 
     data download path every time the OccList.download method is called. 
 
 populate:
     Pre-populate the metadata database in the default metadata storage 
     directory. This will greatly accelerate all queries of the database, 
     including first queries. Be sure to have run setdefaults in advance. 
 
 See README documentation for further instruction on usage. 
-
-********************************************************************************
-Note to developer: Be certain to provide access to s3fs.S3FileSystem that 
-is auto-authenticating. See use_S3FileSystem definition, etc. 
-********************************************************************************
-
 """
 
 #  Define parameters of the database.
 
 AWSregion = "us-east-1"
 databaseS3bucket = "gnss-ro-data"
 float_fill_value = -999.99
 defaults_filename = ".awsgnssroutilsrc"
 
 #  Imports.
 
 import os
 import datetime
 import numpy as np
-import s3fs
+import boto3
 import json
 import re
 import time
 from tqdm import tqdm
 import subprocess
 from botocore import UNSIGNED
 
 
-#  Logging output. 
+#  Linux epoch. 
 
-import logging
-LOGGER = logging.getLogger( __name__ )
+linux_epoch = datetime.datetime( 1970, 1, 1, tzinfo=datetime.timezone.utc )
 
 #  Exception handling.
 
 class Error( Exception ):
     pass
 
 class AWSgnssroutilsError( Error ):
@@ -92,192 +85,240 @@
         self.comment = comment
 
 
 ################################################################################
 #  Useful utility functions and classes.
 ################################################################################
 
-def unsigned_S3FileSystem() -> s3fs.S3FileSystem :
+def unsigned_S3Client():
     """This is a custom function that contains code to generate an authenticated
-    instance of s3fs.S3FileSystem. In this particular case, authentication is
+    instance of a boto3 S3 client. In this particular case, authentication is
     UNSIGNED."""
 
-    s3 = s3fs.S3FileSystem( client_kwargs={ 'region_name': AWSregion },
-                                     config_kwargs={ 'signature_version': UNSIGNED } )
+    session = boto3.Session( region_name=AWSregion )
+    s3client = session.client( "s3", config = boto3.session.Config( signature_version=UNSIGNED ) )
 
-    return s3
+    return s3client
 
-class S3FileSystem():
-    """This class is a wrapper for s3fs.S3FileSystem that checks for broken
+class S3Wrapper():
+    """This class is a wrapper for a boto3 s3 cleint that checks for broken
     instances and restores them when necessary."""
 
-    def __init__( self, S3FileSystem_create_function ):
-        """Create a wrapper for s3fs.S3FileSystem. The sole argument points to a
-        function that returns an instance of s3fs.S3FileSystem that is fully
-        authenticated."""
-
-        self._s3fscreate = S3FileSystem_create_function
-        message = "Argument to S3FileSystem must be a reference to a function " + \
-                "that returns an instance of s3fs.S3FileSystem."
+    def __init__( self, S3Client_create_function, bucket ):
+        """Create a wrapper for a boto3 s3 client. The sole argument points to a
+        function that returns an instance of boto3.Session.client('s3') that is 
+        fully authenticated."""
+
+        self._s3clientcreate = S3Client_create_function
+        message = "Argument to S3Client must be a reference to a function " + \
+                "that returns an instance of a boto3 s3 client." 
 
         try:
-            self._s3 = self._s3fscreate()
+            self._s3client = self._s3clientcreate()
         except:
             raise AWSgnssroutilsError( "IncorrectArgument", message )
 
-        if not isinstance( self._s3, s3fs.S3FileSystem ):
-            raise AWSgnssroutilsError( "IncorrectArgument", message )
+        self.bucket = bucket
 
-    def info( self, x ):
+    def info( self, prefix ):
         try:
-            ret = self._s3.info( x )
+            ret = self._s3client.list_objects_v2( Bucket=self.bucket, Prefix=prefix )
         except:
-            self._s3 = self._s3fscreate()
-            ret = self._s3.info( x )
-        return ret
+            self._s3client = self._s3clientcreate()
+            ret = self._s3client.list_objects_v2( Bucket=self.bucket, Prefix=prefix )
+        return ret[0]
 
-    def download( self, x, y ):
+    def download( self, prefix, y ):
         try:
-            ret = self._s3.download( x, y )
+            ret = self._s3client.download_file( self.bucket, prefix, y )
         except:
-            self._s3 = self._s3fscreate()
-            ret = self._s3.download( x, y )
+            self._s3client = self._s3clientcreate()
+            ret = self._s3client.download_file( self.bucket, prefix, y )
         return ret
 
-    def ls( self, x ):
-        try:
-            ret = self._s3.ls( x )
-        except:
-            self._s3 = self._s3fscreate()
-            ret = self._s3.ls( x )
-        return ret
+    def ls( self, prefix ):
 
-    def open( self, x ):
-        try:
-            ret = self._s3.open( x )
+        try: 
+            paginator = self._s3client.get_paginator( "list_objects_v2" )
         except:
-            self._s3 = self._s3fscreate()
-            ret = self._s3.open( x )
-        return ret
+            self._s3client = self._s3clientcreate()
+            paginator = self._s3client.get_paginator( "list_objects_v2" )
+
+        pages = paginator.paginate( Bucket=self.bucket, Prefix=prefix, Delimiter="/" )
+        ret = { 'prefixes':[], 'keys':[] }
 
+        for page in pages: 
+            if "CommonPrefixes" in page.keys(): 
+                ret['prefixes'] += [ m['Prefix'] for m in page['CommonPrefixes'] ]
+            if "Contents" in page.keys(): 
+                ret['keys'] += [ m['Key'] for m in page['Contents'] ]
+
+        return ret
 
 ################################################################################
 #  IMPORTANT!!!!
-#  Define the auto-refresh S3FileSytem that will be used. 
+#  Define the auto-refresh S3 client that will be used. 
 ################################################################################
 
-use_S3FileSystem = unsigned_S3FileSystem
+use_S3Client = unsigned_S3Client 
 
-
-################################################################################
-#  Useful parameters. Scan the AWS RO data repository for valid versions, valid 
-#  processing centers, and valid file types. 
 ################################################################################
 
-s3 = use_S3FileSystem()
 
-valid_versions = [ entry.split("/")[-1] for entry in s3.ls(f'{databaseS3bucket}/contributed/') ]
+#  Useful parameters. Scan the AWS RO data metadata_root for valid versions 
+#  (valid_versions), valid processing centers (valid_processing_centers), 
+#  valid file types (valid_file_types), and valid missions (valid_missions). 
+#
+#  valid_versions -> a list of version identifiers
+#
+#  valid_processing_centers[version] -> a list of processing centers for a 
+#           specified version
+#
+#  valid_file_types[version] -> a list of existing file types for a 
+#           specified version
+#
+#  valid_missions[version] -> a list of missions for a specified version
+#
+#  validity_table -> a list of dictionaries defining the versions, processing 
+#           centers, file types, and missions available. 
+#
+
+s3client = use_S3Client()
+kwargs = { 'Bucket': databaseS3bucket, 'Delimiter': "/" }
+
+#  Create valid versions. 
+
+prefixes = s3client.list_objects_v2( Prefix=f'contributed/', **kwargs )['CommonPrefixes'] 
+valid_versions = [ entry['Prefix'].split("/")[-2] for entry in prefixes ]
+
+#  Initialize bookkeeping for loops over versions, centers, and missions. 
+
 valid_processing_centers = {}
 valid_file_types = {}
+valid_missions = {}
+valid_table = []
 
 for version in valid_versions: 
-    valid_processing_centers.update( { version: list( { entry.split("/")[-1] for entry in 
-                    s3.ls(f'{databaseS3bucket}/contributed/{version}/') } ) } )
-    fts = []
+
+    prefixes = s3client.list_objects_v2( Prefix=f'contributed/{version}/', **kwargs )['CommonPrefixes'] 
+    valid_processing_centers.update( { version: list( { entry['Prefix'].split("/")[-2] for entry in prefixes } ) } )
+    valid_missions.update( { version: [] } )
+
+    all_filetypes = []
+
     for center in valid_processing_centers[version]: 
-        missions = [ entry.split("/")[-1] for entry in 
-                    s3.ls(f'{databaseS3bucket}/contributed/{version}/{center}/') ]
+
+        prefixes = s3client.list_objects_v2( Prefix=f'contributed/{version}/{center}/', **kwargs )['CommonPrefixes'] 
+        missions = [ entry['Prefix'].split("/")[-2] for entry in prefixes ]
+        valid_missions[version] += missions
+
         for mission in missions: 
-            fts += [ entry.split("/")[-1] for entry in 
-                    s3.ls(f'{databaseS3bucket}/contributed/{version}/{center}/{mission}/') ]
-    valid_file_types.update( { version: list( set( fts ) ) } )
+
+            prefixes = s3client.list_objects_v2( Prefix=f'contributed/{version}/{center}/{mission}/', **kwargs )['CommonPrefixes'] 
+            filetypes = [ entry['Prefix'].split("/")[-2] for entry in prefixes ]
+
+            all_filetypes += [ entry['Prefix'].split("/")[-2] for entry in prefixes ]
+            valid_table += [ { 'version': version, 'center': center, 'mission': mission, 'filetype': ft } for ft in filetypes ] 
+
+    valid_file_types.update( { version: list( set( all_filetypes ) ) } )
+
+valid_missions = { version: sorted( list( set( missions ) ) ) for version, missions in valid_missions.items() }
 
 
 ################################################################################
-#  Resources utilities: create a defaults file, populate metadata database. 
+#  Resources utilities: Create a defaults file, populate metadata database. 
 ################################################################################
 
-def setdefaults( repository:str=None, rodata:str=None, version:str=None ) -> dict: 
-    """Create a local repository for a history database queries. 
+def setdefaults( metadata_root:str=None, data_root:str=None, version:str=None ) -> dict: 
+    """Create a local metadata_root for a history database queries. 
 
-    Create a local repository of prior database queries and record the 
+    Create a local metadata_root of prior database queries and record the 
     directory path in a defaults file that can be found in the user's home 
     directory. Also, one can specify a default path for RO data downloads. 
 
-    repository          An absolute path to a directory containing 
-                        information from all previous searches. 
+    metadata_root       An absolute path to a directory containing 
+                        RO metadata information from all previous searches. 
 
-    rodata              The default path for downloading RO data. If 
+    data_root           The default path for downloading RO data. If 
                         it is not provided here, then it must be provided 
-                        when the method OccList.download is called. "rodata" 
+                        when the method OccList.download is called. "data_root" 
                         must be an absolute path.
 
     version             The default RO format version. The available versions 
                         can be found in s3://gnss-ro-data/dynamo. 
     """
 
-    defaults = { 'repository': "", 'rodata': "", 'version': "" }
+    # defaults = { 'metadata_root': "", 'data_root': "", 'version': "" }
+    new_defaults = {}
+
+    #  Check for existence of defaults file. Get existing defaults. 
+
+    HOME = os.path.expanduser( "~" )
+    defaults_file_path = os.path.join( HOME, defaults_filename )
+
+    if os.path.exists( defaults_file_path ): 
+        with open( defaults_file_path, 'r' ) as fp: 
+            defaults = json.load( fp )
+    else: 
+        defaults = {}
 
     #  Be sure the paths are absolute paths. Also, create paths if they 
     #  don't already exist. 
 
-    if repository is not None: 
-        if repository != os.path.abspath( repository ): 
+    if metadata_root is not None: 
+        if metadata_root != os.path.abspath( metadata_root ): 
             raise AWSgnssroutilsError( "BadPathName", 
-                    f'Path to repository ({repository}) must be an absolute path' )
+                    f'Path to metadata_root ({metadata_root}) must be an absolute path' )
         else: 
-            defaults['repository'] = repository
-            os.makedirs( repository, exist_ok=True )
+            defaults.update( { 'metadata_root': metadata_root } )
+            os.makedirs( metadata_root, exist_ok=True )
 
-    if rodata is not None: 
-        if rodata != os.path.abspath( rodata ): 
+    if data_root is not None: 
+        if data_root != os.path.abspath( data_root ): 
             raise AWSgnssroutilsError( "BadPathName", 
-                    f'Path to rodata ({rodata}) must be an absolute path' )
+                    f'Path to data_root ({data_root}) must be an absolute path' )
         else: 
-            defaults['rodata'] = rodata
-            os.makedirs( rodata, exist_ok=True )
+            defaults.update( { 'data_root': data_root } )
+            os.makedirs( data_root, exist_ok=True )
 
 
     #  Check for a valid version. 
 
     if version is not None: 
 
         if version not in valid_versions: 
             raise AWSgnssroutilsError( "InvalidVersion", f'Version "{version}" is invalid; ' + \
                     'valid versions are ' + ", ".join( valid_versions ) )
 
-        defaults['version'] = version
+        defaults.update( { 'version': version } )
 
-        if repository is not None: 
-            os.makedirs( os.path.join( repository, version ), exist_ok=True )
+        if metadata_root is not None: 
+            os.makedirs( os.path.join( metadata_root, version ), exist_ok=True )
 
-    #  Record repository and rodata paths and version to resource file. 
-
-    HOME = os.path.expanduser( "~" )
-    defaults_file_path = os.path.join( HOME, defaults_filename )
+    #  Record new set of defaults. 
 
     with open( defaults_file_path, 'w' ) as fp: 
         json.dump( defaults, fp )
 
     #  Done. 
 
     return defaults
 
 
 def populate() -> subprocess.CompletedProcess : 
     """Populate the metadata database in the path established by 
     setdefaults. 
 
-    This function will synchronize the default repository path 
+    This function will synchronize the default metadata_root path 
     "{respository}/{version}" with the contents in the AWS S3 path 
     s3://gnss-ro-data/dynamo/{version}/export_subsets. 
     """
 
     defaults = get_defaults()
-    repository, version = defaults['repository'], defaults['version']
+    metadata_root, version = defaults['metadata_root'], defaults['version']
 
     if version is None: 
         raise AWSgnssroutilsError( "InvalidVersion", 'A default version must ' + \
                 'be specified using the awsgnssroutils.database.setdefaults function.' )
 
     #  Check for validity of version. 
 
@@ -285,15 +326,15 @@
         raise AWSgnssroutilsError( "InvalidVersion", f'Version "{version}" is invalid; ' + \
                 'valid versions are ' + ", ".join( valid_versions ) )
 
     #  Create command to sync the metadata database. 
 
     command = [ 'aws', 's3', 'sync', 
                f's3://{databaseS3bucket}/dynamo/{version}/export_subsets/', 
-               os.path.join(repository,version), '--no-sign-request', '--delete' ]
+               os.path.join(metadata_root,version), '--no-sign-request', '--delete' ]
 
     #  Synchronize using subprocess.
 
     ret = subprocess.run( command, capture_output=True )
 
     return
 
@@ -323,14 +364,24 @@
         defaults = json.load( fp )
 
     #  Replace emptry strings with Nones. 
 
     for key, value in defaults.items(): 
         if value == "": defaults.update( { key: None } )
 
+    #  Backward compatibility. 
+
+    keys = defaults.keys()
+
+    if "repository" in keys and "metadata_root" not in keys: 
+        defaults.update( { 'metadata_root': defaults['repository'] } )
+
+    if "rodata" in keys and "data_root" not in keys: 
+        defaults.update( { 'data_root': defaults['rodata'] } )
+
     #  Done. 
 
     return defaults
 
 
 ################################################################################
 #  Define the OccList class, which defines a list of occultations together with
@@ -342,37 +393,37 @@
     in the AWS Registry of Open Data for GNSS RO data. It provides methods
     to filter/subset the list, get metadata on the occultations in the list,
     save the list for future use, download relevant database metadata for
     future inquiries directly from the AWS Open Data S3 bucket, and download
     all RO data associated with the entries in the list to the local file
     system."""
 
-    def __init__( self, data:list, s3, version:str ):
+    def __init__( self, data:list, s3wrapper:S3Wrapper, version:str ):
         """Create an instance of OccList. 
 
         Arguments
         =========
         data        A list of items/RO soundings from the RO database. 
 
-        s3          An instance of S3FileSystem that enables access to the 
-                    AWS repository of RO data.
+        s3wrapper   An instance of S3Wrapper that provides access to the AWS 
+                    metadata_root of RO data.
 
-        version     The AWS repository version.
+        version     The AWS metadata_root version.
         """
 
         if isinstance( data, list ):
             self._data = data
         else:
             raise AWSgnssroutilsError( "BadInput", "Input argument data must be a list." )
 
-        if isinstance( s3, S3FileSystem ):
-            self._s3 = s3
-        else:
-            raise AWSgnssroutilsError( "BadInput", "Input argument s3 must be an " + \
-                    "instance of class s3fs.S3FileSystem" )
+        if isinstance( s3wrapper, S3Wrapper ): 
+            self._s3 = s3wrapper
+        else: 
+            raise AWSgnssroutilsError( "BadInput", "Second input argument must be " + \
+                    "an instance of S3tWrapper." )
 
         self._version = version
 
         self.size = len( self._data )
 
 
     def filter( self, missions:{str,tuple,list}=None, 
@@ -615,15 +666,15 @@
 
             if isinstance( availablefiletypes, str ):
                 f_availablefiletypes = { availablefiletypes }
             else:
                 f_availablefiletypes = set( availablefiletypes )
 
             for availablefiletype in f_availablefiletypes:
-                m = re.search( "^(\w+)_(\w+)$", availablefiletype )
+                m = re.search( r"^(\w+)_(\w+)$", availablefiletype )
                 if m:
                     center, filetype = m.group(1), m.group(2)
                     if center not in valid_processing_centers[self._version]:
                         raise AWSgnssroutilsError( "InvalidProcessingCenter",
                                 f'Processing center "{center}" in availablefiletype {availablefiletype} ' + \
                                         'is not valid.' )
                     if filetype not in valid_file_types[self._version]:
@@ -653,17 +704,17 @@
             if f_GNSSconstellations is not None:
                 keep &= ( item['transmitter'][0] in f_GNSSconstellations )
 
             if f_transmitters is not None:
                 keep &= ( item['transmitter'] in f_transmitters )
 
             if f_datetimerange is not None:
-                ms = re.search( "^(\d{4})-(\d{2})-(\d{2})-(\d{2})-(\d{2})$", item['date-time'] )
+                ms = re.match( r"\d{4}-\d{2}-\d{2}-\d{2}-\d{2}", item['date-time'] )
                 if ms: 
-                    dt = datetime.datetime( *[ int(s) for s in ms.groups() ] )
+                    dt = datetime.datetime.strptime( item['date-time'], "%Y-%m-%d-%H-%M" )
                     keep &= ( f_datetimerange[0] <= dt and dt <= f_datetimerange[1] )
                 else: 
                     keep = False 
 
             if f_longituderange is not None:
                 if item['longitude'] == float_fill_value:
                     keep = False
@@ -707,26 +758,24 @@
             #  Keep or don't keep in list.
 
             if keep:
                 keep_list.append( item )
 
         #  Generate new OccList based on kept items.
 
-        return OccList( data=keep_list, s3=self._s3, version=self._version )
+        return OccList( data=keep_list, s3wrapper=self._s3, version=self._version )
 
     def save(self, filename:str):
         """Save instance of OccList to filename in line JSON format. The OccList
         can be restored using RODatabaseClient.restore."""
 
         with open(filename,'w') as file:
             for item in self._data:
                 file.write(json.dumps(item)+'\n')
 
-        LOGGER.debug( f"Search results saved to {filename}." )
-
     def info( self, param:str ) -> { list, dict }:
         '''Provides information on the following parameters: "mission", "receiver",
         "transmitter", "datetime", "longitude", "latitude", "localtime", "geometry",
         "filetype".
 
         mission         Return a list of the missions in the OccList instance.
 
@@ -773,66 +822,66 @@
             option_list = [ item['setting'] for item in self._data ]
             display = { 'nsetting':option_list.count(True), 'nrising':option_list.count(False) }
 
         elif param == "filetype":
             display = {}
             for item in self._data:
                 for key in item.keys():
-                    m = re.search( "^(\w+)_(\w+)$", key )
+                    m = re.search( r"^(\w+)_(\w+)$", key )
                     if m:
                         if m.group(1) in valid_processing_centers[self._version] and m.group(2) in valid_file_types[self._version]:
                             if key not in display.keys():
                                 display.update( { key: 0 } )
                             display[key] += 1
 
         return display
 
-    def download(self, filetype:str, rodata:str=None, 
+    def download(self, filetype:str, data_root:str=None, 
                  keep_aws_structure:bool=True, silent:bool=False ) -> list :
-        """Download RO data files from AWS Registry of Open Data repository of RO 
+        """Download RO data files from AWS Registry of Open Data metadata_root of RO 
         data. 
 
         Download RO data of file type "filetype" from the AWS Registry of Open
-        Data. The data are downloaded into the directory "rodata" as specified in 
-        the defaults (created by setdefaults) rodata is specified by the keyword. 
+        Data. The data are downloaded into the directory "data_root" as specified in 
+        the defaults (created by setdefaults) data_root is specified by the keyword. 
 
         Arguments
         =========
 
         filetype            The filetype must be one of *_calibratedPhase, 
                             *_refractivityRetrieval, *_atmosphericRetrieval, where 
                             * is one of the valid contributed RO retrieval centers 
                             "ucar", "romsaf", "jpl", etc. 
 
-        rodata              The path to the directory for downloaded RO data files. 
+        data_root              The path to the directory for downloaded RO data files. 
                             It overrides the default download path created by 
                             setdefaults. It can be a relative or absolute path. 
 
         keep_aws_structure  If true, create a directory hierarchy in the same way 
-                            as exists in the RO repository in the AWS Registry of 
+                            as exists in the RO metadata_root in the AWS Registry of 
                             Open Data. If false, all files are downloaded into the 
                             same directory. Note that all RO files are downloaded 
-                            using the AWS hierarchy structure if rodata is not 
+                            using the AWS hierarchy structure if data_root is not 
                             specified as an argument here. 
 
         silent              By setting to True, no progress bars are displayed. 
                             Progress bars are shown by default. 
         """
 
-        if rodata is not None: 
-            rootdir = rodata
+        if data_root is not None: 
+            rootdir = data_root
 
         else: 
             defaults = get_defaults()
-            rootdir = defaults['rodata']
+            rootdir = defaults['data_root']
             if not keep_aws_structure: 
                 raise AWSgnssroutilsError( "BadArgument", 'keep_aws_structure must be ' + \
                         'true if RO data are downloaded into the default directory' )
 
-        m = re.search( "^([a-z]+)_([a-zA-Z]+)$", filetype )
+        m = re.match( r"([a-z]+)_([a-zA-Z]+)", filetype )
         if m:
             if m.group(1) not in valid_processing_centers[self._version]:
                 raise AWSgnssroutilsError( "InvalidInput", 
                         f'Invalid retrieval center "{m.group(1)}" ' + \
                         'requested; must be one of ' + \
                         ', '.join( valid_processing_centers[self._version] ) )
             elif m.group(2) not in valid_file_types[self._version]:
@@ -843,33 +892,27 @@
         else:
             raise AWSgnssroutilsError( "InvalidInput", 
                         f'You must select the "filetype" to download ' + 'as ' + \
                         ', '.join( [ f"*_{ft}" for f in valid_file_types[self._version] ] ) + \
                         ', where * is one of the processing centers ' + \
                         ', '.join( valid_processing_centers[self._version] ) )
 
-        ro_file_list = []
-        for item in self._data:
-            if filetype in item.keys():
-                ro_file_list.append(item[filetype])
-        ro_file_list = sorted( set( ro_file_list ) )
+        ro_file_list = sorted( [ item[filetype] for item in self._data if filetype in item.keys() ] )
 
         sTime = time.time()
         local_file_list = []
-        LOGGER.debug( f"Downloading {len(ro_file_list)} {filetype} files to {rootdir}." )
 
         #  Progress bar or no progress bar. 
 
         if silent: 
-            iterator = range(len(ro_file_list))
+            iterator = ro_file_list
         else: 
-            iterator = tqdm( range(len(ro_file_list)), desc="Downloading..." )
+            iterator = tqdm( ro_file_list, desc=f'Downloading {filetype}' )
 
-        for ifile in iterator: 
-            ro_file = ro_file_list[ifile]
+        for ro_file in iterator: 
 
             if keep_aws_structure:
                 local_path = os.path.join( rootdir, os.path.dirname(ro_file) )
             else:
                 local_path = rootdir
 
             local_file = os.path.join( local_path, os.path.basename(ro_file) )
@@ -877,22 +920,21 @@
             #  Make the local directory path if it doesn't already exist.
 
             os.makedirs(local_path, exist_ok=True)
 
             #  Download the file if it doesn't already exist locally.
 
             if not os.path.exists( local_file ):
-                self._s3.download( "/".join( [databaseS3bucket,ro_file] ), local_file )
+                self._s3.download( ro_file, local_file )
                 ret = True
             else:
                 ret = False
 
             local_file_list.append( local_file )
 
-        LOGGER.debug( "Download took {:} seconds.".format( round((time.time()-sTime),1 ) ) )
         return local_file_list
 
     def values( self, field:str ) -> np.ndarray :
         """Return an ndarray of values of a requested field for the data in the
         OccList. 
 
         Valid fields are "longitude", "latitude", "datetime", "localtime" and "time".  
@@ -924,30 +966,30 @@
 
     def __add__(self, occlist2):
 
         if not isinstance( occlist2, OccList ):
             raise AWSgnssroutilsError( "FaultyAddition", 
                     "Unable to concatenate; both arguments must be instances of OccList." )
 
-        return OccList( data=self._data + occlist2._data, s3=self._s3, version=self._version )
+        return OccList( data=self._data + occlist2._data, s3wrapper=self._s3, version=self._version )
 
     def __padd__(self, occlist2):
 
         if not isinstance( occlist2, OccList ):
             raise AWSgnssroutilsError( "FaultyAddition", 
                     "Unable to concatenate; both arguments must be instances of OccList." )
 
-        return OccList( data=self._data + occlist2._data, s3=self._s3, version=self._version )
+        return OccList( data=self._data + occlist2._data, s3wrapper=self._s3, version=self._version )
 
     def __getitem__(self,items):
         new = self._data[items]
         if isinstance( new, dict ):
-            out = OccList( data=[new], s3=self._s3, version=self._version )
+            out = OccList( data=[new], s3wrapper=self._s3, version=self._version )
         else:
-            out = OccList( data=new, s3=self._s3, version=self._version )
+            out = OccList( data=new, s3wrapper=self._s3, version=self._version )
         return out
 
     def __repr__(self):
         return f'OccList({len(self._data)} items)'
 
 
 ################################################################################
@@ -956,36 +998,36 @@
 ################################################################################
 
 class RODatabaseClient:
     '''Class to initialize filter of dynamo line JSON files named by mission and day.
     An instance of this class initiates a gateway to the database of GNSS radio
     occultation data in the AWS Registry of Open Data. '''
 
-    def __init__( self, repository:str=None, version:str=None, update:bool=False ):
+    def __init__( self, metadata_root:str=None, version:str=None, update:bool=False ):
         '''Create an instance of RODatabaseClient. This object serves as a portal
-        to the database contents of the AWS Registry of Open Data repository of
+        to the database contents of the AWS Registry of Open Data metadata_root of
         GNSS radio occultation data.
 
-        repository  If set, it is the path to the directory on the local file
+        metadata_root  If set, it is the path to the directory on the local file
                     system where the contents of the RO database are stored
-                    locally. If not set, the repository path is read from a 
+                    locally. If not set, the metadata_root path is read from a 
                     defaults file created by the function setdefaults. 
 
         version     The version of the contents of the AWS Registry of Open Data
                     that should be accessed. The various versions that are
                     accessible can be found in s3://gnss-ro-data/dynamo/.
 
-        update      If requested, update the contents of the local repository
-                    to what currently exists in the AWS repository.
+        update      If requested, update the contents of the local metadata_root
+                    to what currently exists in the AWS metadata_root.
         '''
 
-        #  Instantiate the s3 file system in AWS region AWSregion and with unsigned certificate
+        #  Instantiate the s3 client in AWS region AWSregion and with unsigned certificate
         #  authentication.
 
-        self._s3 = S3FileSystem( use_S3FileSystem )
+        self._s3 = S3Wrapper( use_S3Client, databaseS3bucket )
 
         #  Check version. 
 
         if version is None: 
             defaults = get_defaults()
             if defaults['version'] is None: 
                 raise( "InvalidVersion", 'Either specify a version when instantiating ' + \
@@ -997,75 +1039,60 @@
 
         if uversion not in valid_versions: 
             raise AWSgnssroutilsError( "InvalidVersion", f'Version "{uversion}" is invalid; ' + \
                     'valid versions are ' + ", ".join( valid_versions ) )
 
         self._version = uversion
 
-        #  Get location of local database repository of previous searches. 
+        #  Get location of local database metadata_root of previous searches. 
 
-        if repository is None: 
+        if metadata_root is None: 
             defaults = get_defaults()
-            self._repository = defaults['repository']
+            self._metadata_root = defaults['metadata_root']
         else: 
-            self._repository = repository
+            self._metadata_root = metadata_root
 
-        os.makedirs( os.path.join( self._repository, self._version ), exist_ok=True )
+        os.makedirs( os.path.join( self._metadata_root, self._version ), exist_ok=True )
 
-        #  Update the existing repository if requested.
+        #  Update the existing metadata_root if requested.
 
         self._update = update
         if update: 
             self.update_repo()
 
-
-
     def update_repo(self):
         '''This module will check for updated json files on the AWS Registry of Open Data.
         If there has been an update in files that are part of your local repo, they will be
         updated.'''
 
-        if not os.path.exists( self._repository ):
+        if not os.path.exists( self._metadata_root ):
             return
 
-        LOGGER.debug( f"Updating dynamo json files in {self._repository}." )
-
         sTime = time.time()
         altzone = int( time.altzone / 3600 )     #  Correct for the time zone.
-        allfiles = sorted( os.listdir( self._repository ) )
+        allfiles = sorted( os.listdir( self._metadata_root ) )
 
         for filename in allfiles:
-            local_json_info = os.stat( os.path.join( self._repository, filename ) )
-            local_LastModified_ctime = time.ctime( local_json_info.st_mtime )
-            local_LastModified_unaware = datetime.datetime.strptime( local_LastModified_ctime, "%a %b %d %H:%M:%S %Y" )
-            local_LastModified = datetime.datetime( local_LastModified_unaware.year,
-                        local_LastModified_unaware.month,
-                        local_LastModified_unaware.day,
-                        local_LastModified_unaware.hour)
-
-            s3_uri = "/".join( [ databaseS3bucket, f'dynamo/{self._version}/export_subsets', filename ] )
-            s3_info = self._s3.info( s3_uri )
-            s3_LastModified_unaware = s3_info['LastModified']
-            s3_LastModified = datetime.datetime( s3_LastModified_unaware.year,
-                                s3_LastModified_unaware.month, s3_LastModified_unaware.day,
-                                s3_LastModified_unaware.hour-altzone )
-
-            if s3_LastModified > local_LastModified:
-                LOGGER.info( f"  Updating {filename}" )
-                self._s3.download(s3_uri, os.path.join(self._repository,self._version,filename) )
 
-        LOGGER.debug( "Local repository update took {:} seconds.".format( round((time.time()-sTime),1) ) )
+            linux_time = os.path.getmtime( os.path.join( self._metadata_root, filename ) )
+            local_LastModified = linux_epoch + datetime.timedelta( seconds=linux_time )
+
+            s3_info = self._s3.info( f'dynamo/{self._version}/export_subsets/{filename}' )
+            s3_LastModified = s3_info['LastModified']
+
+            if s3_LastModified > local_LastModified + datetime.timedelta(seconds=60):
+                self._s3.download( s3_uri, os.path.join(self._metadata_root,self._version,filename) )
 
     def query(self, missions:{str,tuple,list}=None, 
               datetimerange:{tuple,list}=None, 
               silent:bool=False, **filterargs ) -> OccList:
         """Execute an query on the RO database for RO soundings. 
 
         This method obtains database JSON files from the AWS S3 bucket if the 
-        requested files are not already available in the local repository. 
+        requested files are not already available in the local metadata_root. 
         At least one of the keywords "missions" or "datetimerange" must be 
         specified. All other keywords will serve as filters on the query. 
         Return an instance of class OccList. 
 
         Arguments
         =========
         missions        The names of the missions to query, as defined in the 
@@ -1083,127 +1110,113 @@
 
         if missions is None and datetimerange is None:
             raise AWSgnssroutilsError( "InvalidInput", 
                     f"Either 'missions' or 'datetimerange' or both must be provided." )
 
         #  Get listing of all JSON database files.
 
-        initial_file_array = self._s3.ls( "/".join( 
-                    [ databaseS3bucket, f'dynamo/{self._version}/export_subsets' ] ) )
-        LOGGER.debug( f"Initial file count: {len(initial_file_array)}" )
+        file_array = self._s3.ls( f'dynamo/{self._version}/export_subsets/' )['keys']
 
-        # Filter by mission.
+        #  Filter by mission.
 
-        if missions is None:
-            file_array = initial_file_array.copy()
-        else:
-            file_array = []
-            for file in initial_file_array:
-                basename = os.path.basename(file)
-                basename_mission = basename.split('_')[0]
-                if basename_mission in missions:
-                    file_array.append( file )
-            LOGGER.debug( f"File count after filtering by mission: {len(file_array)}" )
+        if missions is not None:
+            if isinstance( missions, str ): 
+                list_missions = [ missions ]
+            elif isinstance( missions, list ) or isinstance( missions, tuple ): 
+                list_missions = list( missions )
+            file_array = [ file for file in file_array if re.split( r"_", re.split( r"/", file )[-1] )[0] in list_missions ]
 
-        # Filter by date.
+        #  Filter by date.
 
         if datetimerange is not None:
-            remove_list = []
+
             try:
                 dt = datetime.datetime.fromisoformat( datetimerange[0] )
                 rangeStart = datetime.datetime( dt.year, dt.month, dt.day )
                 dt = datetime.datetime.fromisoformat( datetimerange[1] )
                 rangeEnd = datetime.datetime( dt.year, dt.month, dt.day )
             except:
                 raise AWSgnssroutilsError( "FaultyDateFormat", "The datetimerange elements are not ISO format datetimes" )
 
+            retain_array = []
             for file in file_array:
-                m = re.search( "^\w+_(\d{4})-(\d{2})-(\d{2})\.json$", os.path.basename(file) )
-                file_datetime = datetime.datetime( int(m.group(1)), int(m.group(2)), int(m.group(3)) )
-                if file_datetime < rangeStart or file_datetime > rangeEnd:
-                    remove_list.append(file)
-
-            for f in remove_list:
-                file_array.remove(f)
-
-            LOGGER.debug( f"File count after filtering by date: {len(file_array)}" )
+                m = re.search( r"\w+_(\d{4}-\d{2}-\d{2})\.json$", file ) 
+                file_datetime = datetime.datetime.fromisoformat( m.group(1) )
+                if file_datetime >= rangeStart and file_datetime <= rangeEnd:
+                    retain_array.append( file )
+                else: 
+                    pass
+            file_array = retain_array
 
-            # self._repository should be for line JSON files only.
 
-        LOGGER.info( "Updating local database repository..." )
 
         local_file_array = []
-        os.makedirs(self._repository, exist_ok=True)
+        os.makedirs(self._metadata_root, exist_ok=True)
 
         #  Progress bar? 
 
         if silent: 
-            iterator = range(len(file_array))
+            iterator = file_array
         else: 
-            iterator = tqdm( range(len(file_array)), desc="Downloading..." )
+            iterator = tqdm( file_array, desc="Downloading metadata" )
 
-        for ifile in iterator: 
-            file = file_array[ifile]
-            local_path = os.path.join(self._repository,self._version,os.path.basename(file))
+        for file in iterator: 
+            local_path = os.path.join(self._metadata_root,self._version,os.path.basename(file))
             if not os.path.exists(local_path):
-                self._s3.download(file, local_path)
+                self._s3.download( file, local_path )
             local_file_array.append(local_path)
 
-        # Reset file_array to local path.
+        #  Reset file_array to local path.
 
         file_array = local_file_array
 
-        LOGGER.debug( "Searching files for RO events..." )
-
         #  With file array, open up and read files in to query more.
 
-        ret_list = OccList( data=[], s3=self._s3, version=self._version )
+        ret_list = OccList( data=[], s3wrapper=self._s3, version=self._version )
 
         if silent: 
-            iterator = range(len(file_array))
+            iterator = file_array
         else: 
-            iterator = tqdm( range(len(file_array)), desc="Loading..." )
+            iterator = tqdm( file_array, desc="Loading metadata" )
+
+        for file in iterator:
 
-        for ifile in iterator:
-            file = file_array[ifile]
             with open(file, 'r') as f:
                 df_dict = json.loads( f.readline() )
             df = list( df_dict.values() )
 
-            add_list = OccList( df, s3=self._s3, version=self._version ).filter( 
+            add_list = OccList( df, s3wrapper=self._s3, version=self._version ).filter( 
                     missions=missions, datetimerange=datetimerange, **filterargs )
 
             ret_list += add_list
 
         return ret_list
 
     def restore( self, datafile:str ) -> OccList :
         """Restore a previously saved OccList from datafile, which is a
         JSON format file."""
 
         if os.path.exists( datafile ):
-            LOGGER.debug( f"Restoring previously saved OccList from {datafile}." )
-            data = []
             with open( datafile, 'r' ) as f:
-                for line in f.readlines():
-                    data.append( json.loads(line) )
+                data = [ json.loads(line) for line in f.readlines() ]
         else:
             raise AWSgnssroutilsError( "FaultyData", "Argument data must be a list " + \
                     "of RO database items or a path to a previously saved OccList." )
 
-        occlist = OccList( data=data, s3=self._s3, version=self._version )
+        occlist = OccList( data=data, s3wrapper=self._s3, version=self._version )
         return occlist
 
     def __repr__( self ):
 
         output_list = []
 
-        output_list.append( f'repository="{self._repository}"' )
+        output_list.append( f'metadata_root="{self._metadata_root}"' )
         output_list.append( f'version="{self._version}"' )
 
         if self._update:
             output_list.append( "update=True" )
         else:
             output_list.append( "update=False" )
 
         ret = "RODatabaseClient({:})".format( ", ".join( output_list ) )
         return ret
+
```

### Comparing `awsgnssroutils-1.0.7/LICENSE` & `awsgnssroutils-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `awsgnssroutils-1.0.7/pyproject.toml` & `awsgnssroutils-1.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 [build-system]
-requires = [ "hatchling", "s3fs", "numpy", "tqdm" ]
+# requires = [ "hatchling", "s3fs", "numpy", "tqdm" ]
+requires = [ "hatchling>=1.22.2" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "awsgnssroutils"
-version = "1.0.7"
+version = "1.2.0"
 authors = [
 	{ name="Stephen Leroy", email="sleroy@aer.com" },
 	{ name="Amy McVey", email="amcvey@aer.com" }
 	]
 description = "Utilities for access and manipulation of GNSS radio occultation in the AWS Registry of Open Data"
 readme = "README.md"
 requires-python = ">=3.8"
-dependencies = [ "hatchling", "awscli", "s3fs", "numpy", "tqdm" ]
+dependencies = [ "hatchling", "awscli", "boto3", "tqdm", 
+	"numpy", "xarray", "astropy>=5.3", "pyerfa", "sgp4", "netCDF4", 
+	"eumdac", "earthaccess", "aiobotocore[awscli,boto3]" ]
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: BSD License",
-	"Operating System :: OS Independent",
+	"Operating System :: OS Independent"
 	]
 
 [project.urls]
-"Homepage" = "https://github.com/gnss-ro/aws-opendata"
+"Homepage" = "https://github.com/gnss-ro/aws-opendata/awsgnssroutils"
 "Bug Tracker" = "https://github.com/gnss-ro/aws-opendata/issues"
+
+[project.scripts]
+rotcol = "awsgnssroutils.collocation.rotcol:main"
+
```

