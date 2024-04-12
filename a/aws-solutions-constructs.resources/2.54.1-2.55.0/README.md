# Comparing `tmp/aws-solutions-constructs.resources-2.54.1.tar.gz` & `tmp/aws-solutions-constructs.resources-2.55.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-solutions-constructs.resources-2.54.1.tar", last modified: Thu Apr  4 20:59:43 2024, max compression
+gzip compressed data, was "aws-solutions-constructs.resources-2.55.0.tar", last modified: Fri Apr 12 16:15:38 2024, max compression
```

## Comparing `aws-solutions-constructs.resources-2.54.1.tar` & `aws-solutions-constructs.resources-2.55.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:59:43.902614 aws-solutions-constructs.resources-2.54.1/
--rw-r--r--   0 root         (0) root         (0)    10279 2024-04-04 20:59:12.000000 aws-solutions-constructs.resources-2.54.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-04 20:59:12.000000 aws-solutions-constructs.resources-2.54.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2425 2024-04-04 20:59:43.854613 aws-solutions-constructs.resources-2.54.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1554 2024-04-04 20:59:12.000000 aws-solutions-constructs.resources-2.54.1/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2024-04-04 20:59:12.000000 aws-solutions-constructs.resources-2.54.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 20:59:43.902614 aws-solutions-constructs.resources-2.54.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1891 2024-04-04 20:59:12.000000 aws-solutions-constructs.resources-2.54.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:59:43.850613 aws-solutions-constructs.resources-2.54.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:59:43.850613 aws-solutions-constructs.resources-2.54.1/src/aws_solutions_constructs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:59:43.854613 aws-solutions-constructs.resources-2.54.1/src/aws_solutions_constructs/resources/
--rw-r--r--   0 root         (0) root         (0)    19179 2024-04-04 20:59:12.000000 aws-solutions-constructs.resources-2.54.1/src/aws_solutions_constructs/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:59:43.854613 aws-solutions-constructs.resources-2.54.1/src/aws_solutions_constructs/resources/_jsii/
--rw-r--r--   0 root         (0) root         (0)      584 2024-04-04 20:59:12.000000 aws-solutions-constructs.resources-2.54.1/src/aws_solutions_constructs/resources/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)  2063942 2024-04-04 20:59:12.000000 aws-solutions-constructs.resources-2.54.1/src/aws_solutions_constructs/resources/_jsii/resources@2.54.1.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 20:59:12.000000 aws-solutions-constructs.resources-2.54.1/src/aws_solutions_constructs/resources/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:59:43.854613 aws-solutions-constructs.resources-2.54.1/src/aws_solutions_constructs.resources.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2425 2024-04-04 20:59:43.000000 aws-solutions-constructs.resources-2.54.1/src/aws_solutions_constructs.resources.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      589 2024-04-04 20:59:43.000000 aws-solutions-constructs.resources-2.54.1/src/aws_solutions_constructs.resources.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 20:59:43.000000 aws-solutions-constructs.resources-2.54.1/src/aws_solutions_constructs.resources.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      188 2024-04-04 20:59:43.000000 aws-solutions-constructs.resources-2.54.1/src/aws_solutions_constructs.resources.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-04 20:59:43.000000 aws-solutions-constructs.resources-2.54.1/src/aws_solutions_constructs.resources.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:15:38.512487 aws-solutions-constructs.resources-2.55.0/
+-rw-r--r--   0 root         (0) root         (0)    10279 2024-04-12 16:15:07.000000 aws-solutions-constructs.resources-2.55.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-12 16:15:07.000000 aws-solutions-constructs.resources-2.55.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2425 2024-04-12 16:15:38.512487 aws-solutions-constructs.resources-2.55.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1554 2024-04-12 16:15:07.000000 aws-solutions-constructs.resources-2.55.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2024-04-12 16:15:07.000000 aws-solutions-constructs.resources-2.55.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 16:15:38.512487 aws-solutions-constructs.resources-2.55.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1891 2024-04-12 16:15:07.000000 aws-solutions-constructs.resources-2.55.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:15:38.504487 aws-solutions-constructs.resources-2.55.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:15:38.504487 aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:15:38.508487 aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs/resources/
+-rw-r--r--   0 root         (0) root         (0)    19179 2024-04-12 16:15:07.000000 aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:15:38.508487 aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs/resources/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      584 2024-04-12 16:15:07.000000 aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs/resources/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  2063939 2024-04-12 16:15:07.000000 aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs/resources/_jsii/resources@2.55.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 16:15:07.000000 aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs/resources/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:15:38.508487 aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs.resources.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2425 2024-04-12 16:15:38.000000 aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs.resources.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      589 2024-04-12 16:15:38.000000 aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs.resources.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 16:15:38.000000 aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs.resources.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      188 2024-04-12 16:15:38.000000 aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs.resources.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-12 16:15:38.000000 aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs.resources.egg-info/top_level.txt
```

### Comparing `aws-solutions-constructs.resources-2.54.1/LICENSE` & `aws-solutions-constructs.resources-2.55.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-solutions-constructs.resources-2.54.1/PKG-INFO` & `aws-solutions-constructs.resources-2.55.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-solutions-constructs.resources
-Version: 2.54.1
+Version: 2.55.0
 Summary: Resource CDK Constructs for patterns library
 Home-page: https://github.com/awslabs/aws-solutions-constructs.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-solutions-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-solutions-constructs.resources-2.54.1/README.md` & `aws-solutions-constructs.resources-2.55.0/README.md`

 * *Files identical despite different names*

### Comparing `aws-solutions-constructs.resources-2.54.1/setup.py` & `aws-solutions-constructs.resources-2.55.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-solutions-constructs.resources",
-    "version": "2.54.1",
+    "version": "2.55.0",
     "description": "Resource CDK Constructs for patterns library",
     "license": "Apache-2.0",
     "url": "https://github.com/awslabs/aws-solutions-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,27 +22,27 @@
     },
     "packages": [
         "aws_solutions_constructs.resources",
         "aws_solutions_constructs.resources._jsii"
     ],
     "package_data": {
         "aws_solutions_constructs.resources._jsii": [
-            "resources@2.54.1.jsii.tgz"
+            "resources@2.55.0.jsii.tgz"
         ],
         "aws_solutions_constructs.resources": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.135.0, <3.0.0",
         "aws-cdk.integ-tests-alpha==2.135.0.a0",
-        "aws-solutions-constructs.core==2.54.1",
+        "aws-solutions-constructs.core==2.55.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.96.0, <2.0.0",
+        "jsii>=1.97.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `aws-solutions-constructs.resources-2.54.1/src/aws_solutions_constructs/resources/__init__.py` & `aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-solutions-constructs.resources-2.54.1/src/aws_solutions_constructs/resources/_jsii/__init__.py` & `aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs/resources/_jsii/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 import aws_cdk._jsii
 import aws_cdk.integ_tests_alpha._jsii
 import aws_solutions_constructs.core._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@aws-solutions-constructs/resources",
-    "2.54.1",
+    "2.55.0",
     __name__[0:-6],
-    "resources@2.54.1.jsii.tgz",
+    "resources@2.55.0.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `aws-solutions-constructs.resources-2.54.1/src/aws_solutions_constructs/resources/_jsii/resources@2.54.1.jsii.tgz` & `aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs/resources/_jsii/resources@2.55.0.jsii.tgz`

 * *Files 9% similar despite different names*

#### Comparing `resources@2.54.1.jsii.tgz-content` & `resources@2.55.0.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9080882352941176%*

 * *Differences: {"'dependencies'": "{'@aws-solutions-constructs/core': '2.55.0'}",*

 * * "'fingerprint'": "'qe6NuWEfNxYg0ue8AgS2eTV2PXSfg0w+36tlyrvcADs='",*

 * * "'jsiiVersion'": "'1.97.0 (build 729de35)'",*

 * * "'version'": "'2.55.0'"}*

```diff
@@ -10,15 +10,15 @@
     "bundled": {
         "@aws-sdk/client-kms": "^3.478.0",
         "@aws-sdk/client-s3": "^3.478.0",
         "aws-sdk-client-mock": "^3.0.0"
     },
     "dependencies": {
         "@aws-cdk/integ-tests-alpha": "2.135.0-alpha.0",
-        "@aws-solutions-constructs/core": "2.54.1",
+        "@aws-solutions-constructs/core": "2.55.0",
         "aws-cdk-lib": "^2.135.0",
         "constructs": "^10.0.0"
     },
     "dependencyClosure": {
         "@aws-cdk/asset-awscli-v1": {
             "targets": {
                 "dotnet": {
@@ -3717,17 +3717,17 @@
                     "distName": "constructs",
                     "module": "constructs"
                 }
             }
         }
     },
     "description": "Resource CDK Constructs for patterns library",
-    "fingerprint": "QXEo1gG9tzIhfR6cWcMlOjbCxSQnSemMe1vLD9q5fD0=",
+    "fingerprint": "qe6NuWEfNxYg0ue8AgS2eTV2PXSfg0w+36tlyrvcADs=",
     "homepage": "https://github.com/awslabs/aws-solutions-constructs.git",
-    "jsiiVersion": "1.96.0 (build 921e240)",
+    "jsiiVersion": "1.97.0 (build 729de35)",
     "license": "Apache-2.0",
     "metadata": {
         "jsii": {
             "pacmak": {
                 "hasDefaultInterfaces": true
             }
         }
@@ -4061,9 +4061,9 @@
                         "fqn": "aws-cdk-lib.Duration"
                     }
                 }
             ],
             "symbolId": "lib/template-writer:TemplateWriterProps"
         }
     },
-    "version": "2.54.1"
+    "version": "2.55.0"
 }
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'dependencies'": "{'@aws-solutions-constructs/core': '2.55.0'}",*

 * * "'peerDependencies'": "{'@aws-solutions-constructs/core': '2.55.0'}",*

 * * "'version'": "'2.55.0'"}*

```diff
@@ -9,15 +9,15 @@
         "@aws-sdk/client-s3",
         "aws-sdk-client-mock"
     ],
     "dependencies": {
         "@aws-cdk/integ-tests-alpha": "2.135.0-alpha.0",
         "@aws-sdk/client-kms": "^3.478.0",
         "@aws-sdk/client-s3": "^3.478.0",
-        "@aws-solutions-constructs/core": "2.54.1",
+        "@aws-solutions-constructs/core": "2.55.0",
         "aws-sdk-client-mock": "^3.0.0",
         "constructs": "^10.0.0"
     },
     "description": "Resource CDK Constructs for patterns library",
     "devDependencies": {
         "@types/jest": "^27.4.0",
         "@types/node": "^10.3.0",
@@ -60,15 +60,15 @@
             }
         }
     },
     "license": "Apache-2.0",
     "main": "index.js",
     "name": "@aws-solutions-constructs/resources",
     "peerDependencies": {
-        "@aws-solutions-constructs/core": "2.54.1",
+        "@aws-solutions-constructs/core": "2.55.0",
         "aws-cdk-lib": "^2.135.0",
         "constructs": "^10.0.0"
     },
     "repository": {
         "directory": "source/patterns/@aws-solutions-constructs/resources",
         "type": "git",
         "url": "https://github.com/awslabs/aws-solutions-constructs.git"
@@ -84,9 +84,9 @@
         "lint": "eslint -c ../eslintrc.yml --ext=.js,.ts . && tslint --project .",
         "lint-fix": "eslint -c ../eslintrc.yml --ext=.js,.ts --fix .",
         "snapshot-update": "npm test -- -u",
         "test": "jest --coverage",
         "watch": "tsc -b -w"
     },
     "types": "index.ts",
-    "version": "2.54.1"
+    "version": "2.55.0"
 }
```

### Comparing `aws-solutions-constructs.resources-2.54.1/src/aws_solutions_constructs.resources.egg-info/PKG-INFO` & `aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs.resources.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-solutions-constructs.resources
-Version: 2.54.1
+Version: 2.55.0
 Summary: Resource CDK Constructs for patterns library
 Home-page: https://github.com/awslabs/aws-solutions-constructs.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-solutions-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-solutions-constructs.resources-2.54.1/src/aws_solutions_constructs.resources.egg-info/SOURCES.txt` & `aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs.resources.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_solutions_constructs.resources.egg-info/SOURCES.txt
 src/aws_solutions_constructs.resources.egg-info/dependency_links.txt
 src/aws_solutions_constructs.resources.egg-info/requires.txt
 src/aws_solutions_constructs.resources.egg-info/top_level.txt
 src/aws_solutions_constructs/resources/__init__.py
 src/aws_solutions_constructs/resources/py.typed
 src/aws_solutions_constructs/resources/_jsii/__init__.py
-src/aws_solutions_constructs/resources/_jsii/resources@2.54.1.jsii.tgz
+src/aws_solutions_constructs/resources/_jsii/resources@2.55.0.jsii.tgz
```

