# Comparing `tmp/gammarer.aws-secure-cloudfront-origin-bucket-1.4.1.tar.gz` & `tmp/gammarer.aws-secure-cloudfront-origin-bucket-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-secure-cloudfront-origin-bucket-1.4.1.tar", last modified: Sun Apr  7 18:25:23 2024, max compression
+gzip compressed data, was "gammarer.aws-secure-cloudfront-origin-bucket-1.4.2.tar", last modified: Fri Apr 12 11:49:02 2024, max compression
```

## Comparing `gammarer.aws-secure-cloudfront-origin-bucket-1.4.1.tar` & `gammarer.aws-secure-cloudfront-origin-bucket-1.4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:25:23.165246 gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-07 18:25:12.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-07 18:25:12.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-04-07 18:25:23.165246 gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-07 18:25:12.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-07 18:25:12.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 18:25:23.165246 gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-07 18:25:12.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:25:23.165246 gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:25:23.165246 gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:25:23.165246 gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/src/gammarer/aws_secure_cloudfront_origin_bucket/
--rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-04-07 18:25:12.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/src/gammarer/aws_secure_cloudfront_origin_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:25:23.165246 gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-07 18:25:12.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32551 2024-04-07 18:25:12.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/aws-secure-cloudfront-origin-bucket@1.4.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 18:25:12.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/src/gammarer/aws_secure_cloudfront_origin_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:25:23.165246 gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-04-07 18:25:23.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-07 18:25:23.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 18:25:23.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-07 18:25:23.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 18:25:23.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:49:02.714943 gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-12 11:48:51.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 11:48:51.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-12 11:49:02.714943 gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-12 11:48:51.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-12 11:48:51.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 11:49:02.714943 gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-12 11:48:51.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:49:02.714943 gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:49:02.714943 gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:49:02.714943 gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/src/gammarer/aws_secure_cloudfront_origin_bucket/
+-rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-04-12 11:48:51.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/src/gammarer/aws_secure_cloudfront_origin_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:49:02.714943 gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-12 11:48:51.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32545 2024-04-12 11:48:51.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/aws-secure-cloudfront-origin-bucket@1.4.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:48:51.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/src/gammarer/aws_secure_cloudfront_origin_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:49:02.714943 gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-12 11:49:02.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-12 11:49:02.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:49:02.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-12 11:49:02.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 11:49:02.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/top_level.txt
```

### Comparing `gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/LICENSE` & `gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/PKG-INFO` & `gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-cloudfront-origin-bucket
-Version: 1.4.1
+Version: 1.4.2
 Summary: AWS CloudFront distribution origin S3 bucket.
 Home-page: https://github.com/gammarer/aws-secure-cloudfront-origin-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-secure-cloudfront-origin-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -89,19 +89,19 @@
 ```
 
 ### for OAC(Origin Access Control)
 
 ```python
 import { SecureCloudFrontOriginBucket, SecureCloudFrontOriginType } from '@gammarer/aws-secure-cloudfront-origin-bucket';
 
-declare const s3Bucket: cloudfront.Distribution;
+declare const distribution: cloudfront.Distribution;
 
 new SecureCloudFrontOriginBucket(stack, 'SecureCloudFrontOriginBucket', {
   bucketName: 'example-origin-bucket',
   cloudFrontOriginType: SecureCloudFrontOriginType.ORIGIN_ACCESS_CONTROL,
-  cloudFrontArn: 'arn:aws:cloudfront::123456789:distribution/DISTRIBUTIONID',
+  cloudFrontArn: `arn:aws:cloudfront::123456789:distribution/${distribution.distributionId}`,
 });
 ```
 
 ## License
 
 This project is licensed under the Apache-2.0 License.
```

### Comparing `gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/README.md` & `gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -66,19 +66,19 @@
 ```
 
 ### for OAC(Origin Access Control)
 
 ```python
 import { SecureCloudFrontOriginBucket, SecureCloudFrontOriginType } from '@gammarer/aws-secure-cloudfront-origin-bucket';
 
-declare const s3Bucket: cloudfront.Distribution;
+declare const distribution: cloudfront.Distribution;
 
 new SecureCloudFrontOriginBucket(stack, 'SecureCloudFrontOriginBucket', {
   bucketName: 'example-origin-bucket',
   cloudFrontOriginType: SecureCloudFrontOriginType.ORIGIN_ACCESS_CONTROL,
-  cloudFrontArn: 'arn:aws:cloudfront::123456789:distribution/DISTRIBUTIONID',
+  cloudFrontArn: `arn:aws:cloudfront::123456789:distribution/${distribution.distributionId}`,
 });
 ```
 
 ## License
 
 This project is licensed under the Apache-2.0 License.
```

### Comparing `gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/setup.py` & `gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-secure-cloudfront-origin-bucket",
-    "version": "1.4.1",
+    "version": "1.4.2",
     "description": "AWS CloudFront distribution origin S3 bucket.",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarer/aws-secure-cloudfront-origin-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_secure_cloudfront_origin_bucket",
         "gammarer.aws_secure_cloudfront_origin_bucket._jsii"
     ],
     "package_data": {
         "gammarer.aws_secure_cloudfront_origin_bucket._jsii": [
-            "aws-secure-cloudfront-origin-bucket@1.4.1.jsii.tgz"
+            "aws-secure-cloudfront-origin-bucket@1.4.2.jsii.tgz"
         ],
         "gammarer.aws_secure_cloudfront_origin_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/src/gammarer/aws_secure_cloudfront_origin_bucket/__init__.py` & `gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/src/gammarer/aws_secure_cloudfront_origin_bucket/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,20 +67,20 @@
 ```
 
 ### for OAC(Origin Access Control)
 
 ```python
 import { SecureCloudFrontOriginBucket, SecureCloudFrontOriginType } from '@gammarer/aws-secure-cloudfront-origin-bucket';
 
-declare const s3Bucket: cloudfront.Distribution;
+declare const distribution: cloudfront.Distribution;
 
 new SecureCloudFrontOriginBucket(stack, 'SecureCloudFrontOriginBucket', {
   bucketName: 'example-origin-bucket',
   cloudFrontOriginType: SecureCloudFrontOriginType.ORIGIN_ACCESS_CONTROL,
-  cloudFrontArn: 'arn:aws:cloudfront::123456789:distribution/DISTRIBUTIONID',
+  cloudFrontArn: `arn:aws:cloudfront::123456789:distribution/${distribution.distributionId}`,
 });
 ```
 
 ## License
 
 This project is licensed under the Apache-2.0 License.
 '''
```

### Comparing `gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/__init__.py` & `gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 import aws_cdk._jsii
 import constructs._jsii
 import gammarer.aws_secure_bucket._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarer/aws-secure-cloudfront-origin-bucket",
-    "1.4.1",
+    "1.4.2",
     __name__[0:-6],
-    "aws-secure-cloudfront-origin-bucket@1.4.1.jsii.tgz",
+    "aws-secure-cloudfront-origin-bucket@1.4.2.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/PKG-INFO` & `gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-cloudfront-origin-bucket
-Version: 1.4.1
+Version: 1.4.2
 Summary: AWS CloudFront distribution origin S3 bucket.
 Home-page: https://github.com/gammarer/aws-secure-cloudfront-origin-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-secure-cloudfront-origin-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -89,19 +89,19 @@
 ```
 
 ### for OAC(Origin Access Control)
 
 ```python
 import { SecureCloudFrontOriginBucket, SecureCloudFrontOriginType } from '@gammarer/aws-secure-cloudfront-origin-bucket';
 
-declare const s3Bucket: cloudfront.Distribution;
+declare const distribution: cloudfront.Distribution;
 
 new SecureCloudFrontOriginBucket(stack, 'SecureCloudFrontOriginBucket', {
   bucketName: 'example-origin-bucket',
   cloudFrontOriginType: SecureCloudFrontOriginType.ORIGIN_ACCESS_CONTROL,
-  cloudFrontArn: 'arn:aws:cloudfront::123456789:distribution/DISTRIBUTIONID',
+  cloudFrontArn: `arn:aws:cloudfront::123456789:distribution/${distribution.distributionId}`,
 });
 ```
 
 ## License
 
 This project is licensed under the Apache-2.0 License.
```

### Comparing `gammarer.aws-secure-cloudfront-origin-bucket-1.4.1/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/SOURCES.txt` & `gammarer.aws-secure-cloudfront-origin-bucket-1.4.2/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/SOURCES.txt
 src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/dependency_links.txt
 src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/requires.txt
 src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/top_level.txt
 src/gammarer/aws_secure_cloudfront_origin_bucket/__init__.py
 src/gammarer/aws_secure_cloudfront_origin_bucket/py.typed
 src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/__init__.py
-src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/aws-secure-cloudfront-origin-bucket@1.4.1.jsii.tgz
+src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/aws-secure-cloudfront-origin-bucket@1.4.2.jsii.tgz
```

