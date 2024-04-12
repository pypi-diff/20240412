# Comparing `tmp/gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4.tar.gz` & `tmp/gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4.tar", last modified: Sun Apr  7 18:21:17 2024, max compression
+gzip compressed data, was "gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0.tar", last modified: Fri Apr 12 11:56:06 2024, max compression
```

## Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4.tar` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:21:17.628636 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-07 18:21:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-07 18:21:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-07 18:21:17.628636 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-07 18:21:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-07 18:21:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 18:21:17.628636 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-07 18:21:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:21:17.624636 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:21:17.624636 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:21:17.624636 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/
--rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-04-07 18:21:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:21:17.628636 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-07 18:21:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22234 2024-04-07 18:21:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@1.1.4.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 18:21:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:21:17.624636 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-07 18:21:17.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-07 18:21:17.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 18:21:17.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-07 18:21:17.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 18:21:17.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:56:06.326172 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-12 11:55:55.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 11:55:55.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-12 11:56:06.326172 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-12 11:55:55.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-12 11:55:55.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 11:56:06.326172 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-12 11:55:55.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:56:06.322172 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:56:06.322172 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:56:06.326172 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)    18745 2024-04-12 11:55:55.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:56:06.326172 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-12 11:55:55.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24445 2024-04-12 11:55:55.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@1.2.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:55:55.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:56:06.326172 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-12 11:56:06.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-12 11:56:06.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:56:06.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-12 11:56:06.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 11:56:06.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/top_level.txt
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/LICENSE` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/PKG-INFO` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,16 @@
-Metadata-Version: 2.1
-Name: gammarer.aws-secure-frontend-web-app-cloudfront-distribution
-Version: 1.1.4
-Summary: AWS CloudFront distribution for frontend web app (spa) optimized.
-Home-page: https://github.com/gammarer/aws-secure-frontend-web-app-cloudfront-distribution.git
-Author: yicr<yicr@users.noreply.github.com>
-License: Apache-2.0
-Project-URL: Source, https://github.com/gammarer/aws-secure-frontend-web-app-cloudfront-distribution.git
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: JavaScript
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Typing :: Typed
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved
-Requires-Python: ~=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # AWS Secure Frontend Web App CloudFront Distribution (for AWS CDK v2)
 
-[![GitHub](https://img.shields.io/github/license/yicr/aws-secure-frontend-web-app-cloudfront-distribution?style=flat-square)](https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution/blob/main/LICENSE)
+[![GitHub](https://img.shields.io/github/license/gammarer/aws-secure-frontend-web-app-cloudfront-distribution?style=flat-square)](https://github.com/gammarer/aws-secure-frontend-web-app-cloudfront-distribution/blob/main/LICENSE)
 [![npm (scoped)](https://img.shields.io/npm/v/@gammarer/aws-secure-frontend-web-app-cloudfront-distribution?style=flat-square)](https://www.npmjs.com/package/@gammarer/aws-secure-frontend-web-app-cloudfront-distribution)
 [![PyPI](https://img.shields.io/pypi/v/gammarer.aws-secure-frontend-web-app-cloudfront-distribution?style=flat-square)](https://pypi.org/project/gammarer.aws-secure-frontend-web-app-cloudfront-distribution/)
 [![Nuget](https://img.shields.io/nuget/v/Gammarer.CDK.AWS.SecureFrontendWebAppCloudFrontDistribution?style=flat-square)](https://www.nuget.org/packages/Gammarer.CDK.AWS.SecureFrontendWebAppCloudFrontDistribution/)
 [![Sonatype Nexus (Releases)](https://img.shields.io/nexus/r/com.gammarer/aws-secure-frontend-web-app-cloudfront-distribution?server=https%3A%2F%2Fs01.oss.sonatype.org%2F&style=flat-square)](https://s01.oss.sonatype.org/content/repositories/releases/com/gammarer/aws-secure-frontend-web-app-cloudfront-distribution/)
-[![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/yicr/aws-secure-frontend-web-app-cloudfront-distribution/release.yml?branch=main&label=release&style=flat-square)](https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution/actions/workflows/release.yml)
-[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/yicr/aws-secure-frontend-web-app-cloudfront-distribution?sort=semver&style=flat-square)](https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution/releases)
+[![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/gammarer/aws-secure-frontend-web-app-cloudfront-distribution/release.yml?branch=main&label=release&style=flat-square)](https://github.com/gammarer/aws-secure-frontend-web-app-cloudfront-distribution/actions/workflows/release.yml)
+[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/gammarer/aws-secure-frontend-web-app-cloudfront-distribution?sort=semver&style=flat-square)](https://github.com/gammarer/aws-secure-frontend-web-app-cloudfront-distribution/releases)
 
 [![View on Construct Hub](https://constructs.dev/badge?package=@gammarer/aws-secure-frontend-web-app-cloudfront-distribution)](https://constructs.dev/packages/@gammarer/aws-secure-frontend-web-app-cloudfront-distribution)
 
 AWS CloudFront distribution for frontend web app (spa) optimized.
 
 ## Install
 
@@ -66,25 +43,52 @@
   <groupId>com.gammarer</groupId>
   <artifactId>aws-secure-frontend-web-app-cloudfront-distribution</artifactId>
 </dependency>
 ```
 
 ## Example
 
+### for Origin Access Control
+
 ```python
-import { SecureFrontendWebAppCloudFrontDistribution } from '@gammarer/aws-secure-frontend-web-app-cloudfront-distribution';
+import { SecureFrontendWebAppCloudFrontDistribution, S3OriginAccessType } from '@gammarer/aws-secure-frontend-web-app-cloudfront-distribution';
+
+declare const originBucket: s3.Bucket;
+declare const accessLogBucket: s3.Bucket;
+declare const certificate: acm.Certificate;
+declare const cfnOriginAccessControl: cloudfront.CfnOriginAccessControl
+
+new SecureFrontendWebAppCloudFrontDistribution(stack, 'SecureFrontendWebAppCloudFrontDistribution', {
+  comment: 'frontend web app distribution.', // optional
+  accessLogBucket: accessLogBucket, // optional
+  certificate: certificate,
+  distributionDomainName: 'example.com',
+  s3OriginAccessType: S3OriginAccessType.ORIGIN_ACCESS_CONTROL,
+  originAccessControlId: cfnOriginAccessControl.attrId,
+  originBucket: originBucket,
+});
+```
+
+### for Origin Access Identity
+
+```python
+import { SecureFrontendWebAppCloudFrontDistribution, S3OriginAccessType } from '@gammarer/aws-secure-frontend-web-app-cloudfront-distribution';
+
+declare const originBucket: s3.Bucket;
+declare const accessLogBucket: s3.Bucket;
+declare const certificate: acm.Certificate;
+declare const originAccessIdentity: cloudfront.OriginAccessIdentity;
 
 new SecureFrontendWebAppCloudFrontDistribution(stack, 'SecureFrontendWebAppCloudFrontDistribution', {
   comment: 'frontend web app distribution.', // optional
-  accessLogBucket: new s3.Bucket(stack, 'LogBucket'), // optional
-  certificate: new acm.Certificate(stack, 'Certificate', {
-    domainName: 'example.com',
-  }),
+  accessLogBucket: accessLogBucket, // optional
+  certificate: certificate,
   distributionDomainName: 'example.com',
-  originAccessIdentity: new cloudfront.OriginAccessIdentity(stack, 'OriginAccessIdentity'),
-  originBucket: new s3.Bucket(stack, 'OriginBucket'),
+  s3OriginAccessType: S3OriginAccessType.ORIGIN_ACCESS_IDENTITY,
+  originAccessIdentity: originAccessIdentity,
+  originBucket: originBucket,
 });
 ```
 
 ## License
 
 This project is licensed under the Apache-2.0 License.
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/setup.py` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-secure-frontend-web-app-cloudfront-distribution",
-    "version": "1.1.4",
+    "version": "1.2.0",
     "description": "AWS CloudFront distribution for frontend web app (spa) optimized.",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarer/aws-secure-frontend-web-app-cloudfront-distribution.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution",
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution._jsii"
     ],
     "package_data": {
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution._jsii": [
-            "aws-secure-frontend-web-app-cloudfront-distribution@1.1.4.jsii.tgz"
+            "aws-secure-frontend-web-app-cloudfront-distribution@1.2.0.jsii.tgz"
         ],
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 '''
 # AWS Secure Frontend Web App CloudFront Distribution (for AWS CDK v2)
 
-[![GitHub](https://img.shields.io/github/license/yicr/aws-secure-frontend-web-app-cloudfront-distribution?style=flat-square)](https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution/blob/main/LICENSE)
+[![GitHub](https://img.shields.io/github/license/gammarer/aws-secure-frontend-web-app-cloudfront-distribution?style=flat-square)](https://github.com/gammarer/aws-secure-frontend-web-app-cloudfront-distribution/blob/main/LICENSE)
 [![npm (scoped)](https://img.shields.io/npm/v/@gammarer/aws-secure-frontend-web-app-cloudfront-distribution?style=flat-square)](https://www.npmjs.com/package/@gammarer/aws-secure-frontend-web-app-cloudfront-distribution)
 [![PyPI](https://img.shields.io/pypi/v/gammarer.aws-secure-frontend-web-app-cloudfront-distribution?style=flat-square)](https://pypi.org/project/gammarer.aws-secure-frontend-web-app-cloudfront-distribution/)
 [![Nuget](https://img.shields.io/nuget/v/Gammarer.CDK.AWS.SecureFrontendWebAppCloudFrontDistribution?style=flat-square)](https://www.nuget.org/packages/Gammarer.CDK.AWS.SecureFrontendWebAppCloudFrontDistribution/)
 [![Sonatype Nexus (Releases)](https://img.shields.io/nexus/r/com.gammarer/aws-secure-frontend-web-app-cloudfront-distribution?server=https%3A%2F%2Fs01.oss.sonatype.org%2F&style=flat-square)](https://s01.oss.sonatype.org/content/repositories/releases/com/gammarer/aws-secure-frontend-web-app-cloudfront-distribution/)
-[![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/yicr/aws-secure-frontend-web-app-cloudfront-distribution/release.yml?branch=main&label=release&style=flat-square)](https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution/actions/workflows/release.yml)
-[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/yicr/aws-secure-frontend-web-app-cloudfront-distribution?sort=semver&style=flat-square)](https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution/releases)
+[![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/gammarer/aws-secure-frontend-web-app-cloudfront-distribution/release.yml?branch=main&label=release&style=flat-square)](https://github.com/gammarer/aws-secure-frontend-web-app-cloudfront-distribution/actions/workflows/release.yml)
+[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/gammarer/aws-secure-frontend-web-app-cloudfront-distribution?sort=semver&style=flat-square)](https://github.com/gammarer/aws-secure-frontend-web-app-cloudfront-distribution/releases)
 
 [![View on Construct Hub](https://constructs.dev/badge?package=@gammarer/aws-secure-frontend-web-app-cloudfront-distribution)](https://constructs.dev/packages/@gammarer/aws-secure-frontend-web-app-cloudfront-distribution)
 
 AWS CloudFront distribution for frontend web app (spa) optimized.
 
 ## Install
 
@@ -44,26 +44,53 @@
   <groupId>com.gammarer</groupId>
   <artifactId>aws-secure-frontend-web-app-cloudfront-distribution</artifactId>
 </dependency>
 ```
 
 ## Example
 
+### for Origin Access Control
+
+```python
+import { SecureFrontendWebAppCloudFrontDistribution, S3OriginAccessType } from '@gammarer/aws-secure-frontend-web-app-cloudfront-distribution';
+
+declare const originBucket: s3.Bucket;
+declare const accessLogBucket: s3.Bucket;
+declare const certificate: acm.Certificate;
+declare const cfnOriginAccessControl: cloudfront.CfnOriginAccessControl
+
+new SecureFrontendWebAppCloudFrontDistribution(stack, 'SecureFrontendWebAppCloudFrontDistribution', {
+  comment: 'frontend web app distribution.', // optional
+  accessLogBucket: accessLogBucket, // optional
+  certificate: certificate,
+  distributionDomainName: 'example.com',
+  s3OriginAccessType: S3OriginAccessType.ORIGIN_ACCESS_CONTROL,
+  originAccessControlId: cfnOriginAccessControl.attrId,
+  originBucket: originBucket,
+});
+```
+
+### for Origin Access Identity
+
 ```python
-import { SecureFrontendWebAppCloudFrontDistribution } from '@gammarer/aws-secure-frontend-web-app-cloudfront-distribution';
+import { SecureFrontendWebAppCloudFrontDistribution, S3OriginAccessType } from '@gammarer/aws-secure-frontend-web-app-cloudfront-distribution';
+
+declare const originBucket: s3.Bucket;
+declare const accessLogBucket: s3.Bucket;
+declare const certificate: acm.Certificate;
+declare const originAccessIdentity: cloudfront.OriginAccessIdentity;
 
 new SecureFrontendWebAppCloudFrontDistribution(stack, 'SecureFrontendWebAppCloudFrontDistribution', {
   comment: 'frontend web app distribution.', // optional
-  accessLogBucket: new s3.Bucket(stack, 'LogBucket'), // optional
-  certificate: new acm.Certificate(stack, 'Certificate', {
-    domainName: 'example.com',
-  }),
+  accessLogBucket: accessLogBucket, // optional
+  certificate: certificate,
   distributionDomainName: 'example.com',
-  originAccessIdentity: new cloudfront.OriginAccessIdentity(stack, 'OriginAccessIdentity'),
-  originBucket: new s3.Bucket(stack, 'OriginBucket'),
+  s3OriginAccessType: S3OriginAccessType.ORIGIN_ACCESS_IDENTITY,
+  originAccessIdentity: originAccessIdentity,
+  originBucket: originBucket,
 });
 ```
 
 ## License
 
 This project is licensed under the Apache-2.0 License.
 '''
@@ -86,101 +113,202 @@
 
 import aws_cdk.aws_certificatemanager as _aws_cdk_aws_certificatemanager_ceddda9d
 import aws_cdk.aws_cloudfront as _aws_cdk_aws_cloudfront_ceddda9d
 import aws_cdk.aws_s3 as _aws_cdk_aws_s3_ceddda9d
 import constructs as _constructs_77d1e7e8
 
 
+@jsii.enum(
+    jsii_type="@gammarer/aws-secure-frontend-web-app-cloudfront-distribution.S3OriginAccessType"
+)
+class S3OriginAccessType(enum.Enum):
+    ORIGIN_ACCESS_IDENTITY = "ORIGIN_ACCESS_IDENTITY"
+    ORIGIN_ACCESS_CONTROL = "ORIGIN_ACCESS_CONTROL"
+
+
 class SecureFrontendWebAppCloudFrontDistribution(
     _aws_cdk_aws_cloudfront_ceddda9d.Distribution,
     metaclass=jsii.JSIIMeta,
     jsii_type="@gammarer/aws-secure-frontend-web-app-cloudfront-distribution.SecureFrontendWebAppCloudFrontDistribution",
 ):
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
+        props: typing.Union[typing.Union["SecureFrontendWebAppCloudFrontDistributionOriginAccessIdentityProps", typing.Dict[builtins.str, typing.Any]], typing.Union["SecureFrontendWebAppCloudFrontDistributionOriginAccessControlProps", typing.Dict[builtins.str, typing.Any]]],
+    ) -> None:
+        '''
+        :param scope: -
+        :param id: -
+        :param props: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__ab68d83b630cc02546d77e48c8646f50b0e2f872bcc124abfd93eb26fa3bfc75)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+        jsii.create(self.__class__, self, [scope, id, props])
+
+
+@jsii.data_type(
+    jsii_type="@gammarer/aws-secure-frontend-web-app-cloudfront-distribution.SecureFrontendWebAppCloudFrontDistributionOriginAccessControlProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "certificate": "certificate",
+        "domain_name": "domainName",
+        "origin_access_control_id": "originAccessControlId",
+        "origin_bucket": "originBucket",
+        "s3_origin_access_type": "s3OriginAccessType",
+        "access_log_bucket": "accessLogBucket",
+        "comment": "comment",
+    },
+)
+class SecureFrontendWebAppCloudFrontDistributionOriginAccessControlProps:
+    def __init__(
+        self,
         *,
         certificate: _aws_cdk_aws_certificatemanager_ceddda9d.ICertificate,
         domain_name: builtins.str,
-        origin_access_identity: _aws_cdk_aws_cloudfront_ceddda9d.IOriginAccessIdentity,
+        origin_access_control_id: builtins.str,
         origin_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+        s3_origin_access_type: S3OriginAccessType,
         access_log_bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
         comment: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param scope: -
-        :param id: -
         :param certificate: 
         :param domain_name: 
-        :param origin_access_identity: 
+        :param origin_access_control_id: 
         :param origin_bucket: 
+        :param s3_origin_access_type: 
         :param access_log_bucket: 
         :param comment: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ab68d83b630cc02546d77e48c8646f50b0e2f872bcc124abfd93eb26fa3bfc75)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-        props = SecureFrontendWebAppCloudFrontDistributionProps(
-            certificate=certificate,
-            domain_name=domain_name,
-            origin_access_identity=origin_access_identity,
-            origin_bucket=origin_bucket,
-            access_log_bucket=access_log_bucket,
-            comment=comment,
-        )
+            type_hints = typing.get_type_hints(_typecheckingstub__b2c7e099c315e5352ee2115eb2ffd3113cfcdda8d574cb86a92a3fdca60152ac)
+            check_type(argname="argument certificate", value=certificate, expected_type=type_hints["certificate"])
+            check_type(argname="argument domain_name", value=domain_name, expected_type=type_hints["domain_name"])
+            check_type(argname="argument origin_access_control_id", value=origin_access_control_id, expected_type=type_hints["origin_access_control_id"])
+            check_type(argname="argument origin_bucket", value=origin_bucket, expected_type=type_hints["origin_bucket"])
+            check_type(argname="argument s3_origin_access_type", value=s3_origin_access_type, expected_type=type_hints["s3_origin_access_type"])
+            check_type(argname="argument access_log_bucket", value=access_log_bucket, expected_type=type_hints["access_log_bucket"])
+            check_type(argname="argument comment", value=comment, expected_type=type_hints["comment"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "certificate": certificate,
+            "domain_name": domain_name,
+            "origin_access_control_id": origin_access_control_id,
+            "origin_bucket": origin_bucket,
+            "s3_origin_access_type": s3_origin_access_type,
+        }
+        if access_log_bucket is not None:
+            self._values["access_log_bucket"] = access_log_bucket
+        if comment is not None:
+            self._values["comment"] = comment
 
-        jsii.create(self.__class__, self, [scope, id, props])
+    @builtins.property
+    def certificate(self) -> _aws_cdk_aws_certificatemanager_ceddda9d.ICertificate:
+        result = self._values.get("certificate")
+        assert result is not None, "Required property 'certificate' is missing"
+        return typing.cast(_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate, result)
+
+    @builtins.property
+    def domain_name(self) -> builtins.str:
+        result = self._values.get("domain_name")
+        assert result is not None, "Required property 'domain_name' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def origin_access_control_id(self) -> builtins.str:
+        result = self._values.get("origin_access_control_id")
+        assert result is not None, "Required property 'origin_access_control_id' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def origin_bucket(self) -> _aws_cdk_aws_s3_ceddda9d.IBucket:
+        result = self._values.get("origin_bucket")
+        assert result is not None, "Required property 'origin_bucket' is missing"
+        return typing.cast(_aws_cdk_aws_s3_ceddda9d.IBucket, result)
+
+    @builtins.property
+    def s3_origin_access_type(self) -> S3OriginAccessType:
+        result = self._values.get("s3_origin_access_type")
+        assert result is not None, "Required property 's3_origin_access_type' is missing"
+        return typing.cast(S3OriginAccessType, result)
+
+    @builtins.property
+    def access_log_bucket(self) -> typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket]:
+        result = self._values.get("access_log_bucket")
+        return typing.cast(typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket], result)
+
+    @builtins.property
+    def comment(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("comment")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "SecureFrontendWebAppCloudFrontDistributionOriginAccessControlProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
 
 
 @jsii.data_type(
-    jsii_type="@gammarer/aws-secure-frontend-web-app-cloudfront-distribution.SecureFrontendWebAppCloudFrontDistributionProps",
+    jsii_type="@gammarer/aws-secure-frontend-web-app-cloudfront-distribution.SecureFrontendWebAppCloudFrontDistributionOriginAccessIdentityProps",
     jsii_struct_bases=[],
     name_mapping={
         "certificate": "certificate",
         "domain_name": "domainName",
         "origin_access_identity": "originAccessIdentity",
         "origin_bucket": "originBucket",
+        "s3_origin_access_type": "s3OriginAccessType",
         "access_log_bucket": "accessLogBucket",
         "comment": "comment",
     },
 )
-class SecureFrontendWebAppCloudFrontDistributionProps:
+class SecureFrontendWebAppCloudFrontDistributionOriginAccessIdentityProps:
     def __init__(
         self,
         *,
         certificate: _aws_cdk_aws_certificatemanager_ceddda9d.ICertificate,
         domain_name: builtins.str,
         origin_access_identity: _aws_cdk_aws_cloudfront_ceddda9d.IOriginAccessIdentity,
         origin_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+        s3_origin_access_type: S3OriginAccessType,
         access_log_bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
         comment: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param certificate: 
         :param domain_name: 
         :param origin_access_identity: 
         :param origin_bucket: 
+        :param s3_origin_access_type: 
         :param access_log_bucket: 
         :param comment: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__46fcd4037c1afe9dd0632bd9133c92d55839ac1c45b0d25a564b359716dceb26)
+            type_hints = typing.get_type_hints(_typecheckingstub__51ab04636ec4ac1bd79426d68b913ddb44fcecef50d9426e371f6be93f8c67d7)
             check_type(argname="argument certificate", value=certificate, expected_type=type_hints["certificate"])
             check_type(argname="argument domain_name", value=domain_name, expected_type=type_hints["domain_name"])
             check_type(argname="argument origin_access_identity", value=origin_access_identity, expected_type=type_hints["origin_access_identity"])
             check_type(argname="argument origin_bucket", value=origin_bucket, expected_type=type_hints["origin_bucket"])
+            check_type(argname="argument s3_origin_access_type", value=s3_origin_access_type, expected_type=type_hints["s3_origin_access_type"])
             check_type(argname="argument access_log_bucket", value=access_log_bucket, expected_type=type_hints["access_log_bucket"])
             check_type(argname="argument comment", value=comment, expected_type=type_hints["comment"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "certificate": certificate,
             "domain_name": domain_name,
             "origin_access_identity": origin_access_identity,
             "origin_bucket": origin_bucket,
+            "s3_origin_access_type": s3_origin_access_type,
         }
         if access_log_bucket is not None:
             self._values["access_log_bucket"] = access_log_bucket
         if comment is not None:
             self._values["comment"] = comment
 
     @builtins.property
@@ -206,14 +334,20 @@
     @builtins.property
     def origin_bucket(self) -> _aws_cdk_aws_s3_ceddda9d.IBucket:
         result = self._values.get("origin_bucket")
         assert result is not None, "Required property 'origin_bucket' is missing"
         return typing.cast(_aws_cdk_aws_s3_ceddda9d.IBucket, result)
 
     @builtins.property
+    def s3_origin_access_type(self) -> S3OriginAccessType:
+        result = self._values.get("s3_origin_access_type")
+        assert result is not None, "Required property 's3_origin_access_type' is missing"
+        return typing.cast(S3OriginAccessType, result)
+
+    @builtins.property
     def access_log_bucket(self) -> typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket]:
         result = self._values.get("access_log_bucket")
         return typing.cast(typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket], result)
 
     @builtins.property
     def comment(self) -> typing.Optional[builtins.str]:
         result = self._values.get("comment")
@@ -222,44 +356,54 @@
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "SecureFrontendWebAppCloudFrontDistributionProps(%s)" % ", ".join(
+        return "SecureFrontendWebAppCloudFrontDistributionOriginAccessIdentityProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 __all__ = [
+    "S3OriginAccessType",
     "SecureFrontendWebAppCloudFrontDistribution",
-    "SecureFrontendWebAppCloudFrontDistributionProps",
+    "SecureFrontendWebAppCloudFrontDistributionOriginAccessControlProps",
+    "SecureFrontendWebAppCloudFrontDistributionOriginAccessIdentityProps",
 ]
 
 publication.publish()
 
 def _typecheckingstub__ab68d83b630cc02546d77e48c8646f50b0e2f872bcc124abfd93eb26fa3bfc75(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
+    props: typing.Union[typing.Union[SecureFrontendWebAppCloudFrontDistributionOriginAccessIdentityProps, typing.Dict[builtins.str, typing.Any]], typing.Union[SecureFrontendWebAppCloudFrontDistributionOriginAccessControlProps, typing.Dict[builtins.str, typing.Any]]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__b2c7e099c315e5352ee2115eb2ffd3113cfcdda8d574cb86a92a3fdca60152ac(
     *,
     certificate: _aws_cdk_aws_certificatemanager_ceddda9d.ICertificate,
     domain_name: builtins.str,
-    origin_access_identity: _aws_cdk_aws_cloudfront_ceddda9d.IOriginAccessIdentity,
+    origin_access_control_id: builtins.str,
     origin_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+    s3_origin_access_type: S3OriginAccessType,
     access_log_bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
     comment: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__46fcd4037c1afe9dd0632bd9133c92d55839ac1c45b0d25a564b359716dceb26(
+def _typecheckingstub__51ab04636ec4ac1bd79426d68b913ddb44fcecef50d9426e371f6be93f8c67d7(
     *,
     certificate: _aws_cdk_aws_certificatemanager_ceddda9d.ICertificate,
     domain_name: builtins.str,
     origin_access_identity: _aws_cdk_aws_cloudfront_ceddda9d.IOriginAccessIdentity,
     origin_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+    s3_origin_access_type: S3OriginAccessType,
     access_log_bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
     comment: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from typeguard import check_type
 
 import aws_cdk._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarer/aws-secure-frontend-web-app-cloudfront-distribution",
-    "1.1.4",
+    "1.2.0",
     __name__[0:-6],
-    "aws-secure-frontend-web-app-cloudfront-distribution@1.1.4.jsii.tgz",
+    "aws-secure-frontend-web-app-cloudfront-distribution@1.2.0.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.2.0/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/dependency_links.txt
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/requires.txt
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/top_level.txt
 src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py
 src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/py.typed
 src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py
-src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@1.1.4.jsii.tgz
+src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@1.2.0.jsii.tgz
```

