# Comparing `tmp/droidlysis-3.4.5.tar.gz` & `tmp/droidlysis-3.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "droidlysis-3.4.5.tar", last modified: Mon May 15 16:01:30 2023, max compression
+gzip compressed data, was "droidlysis-3.4.7.tar", last modified: Fri Apr 12 11:11:52 2024, max compression
```

## Comparing `droidlysis-3.4.5.tar` & `droidlysis-3.4.7.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxrwxr-x   0 axelle    (1000) axelle    (1000)        0 2023-05-15 16:01:30.391940 droidlysis-3.4.5/
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     1057 2021-08-19 09:28:51.000000 droidlysis-3.4.5/LICENSE
--rw-rw-r--   0 axelle    (1000) axelle    (1000)       45 2021-08-19 09:28:51.000000 droidlysis-3.4.5/MANIFEST.in
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     9760 2023-05-15 16:01:30.391940 droidlysis-3.4.5/PKG-INFO
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     9169 2023-05-15 15:59:40.000000 droidlysis-3.4.5/README.md
-drwxrwxr-x   0 axelle    (1000) axelle    (1000)        0 2023-05-15 16:01:30.391940 droidlysis-3.4.5/conf/
--rw-rw-r--   0 axelle    (1000) axelle    (1000)        0 2021-08-19 09:28:51.000000 droidlysis-3.4.5/conf/__init__.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     1768 2021-08-19 09:28:51.000000 droidlysis-3.4.5/conf/arm.conf
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     3346 2021-08-19 09:28:51.000000 droidlysis-3.4.5/conf/exodustrack.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)      349 2023-05-15 15:35:24.000000 droidlysis-3.4.5/conf/general.conf
--rw-rw-r--   0 axelle    (1000) axelle    (1000)    60591 2023-03-10 15:08:56.000000 droidlysis-3.4.5/conf/kit.conf
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     1935 2021-08-19 09:28:51.000000 droidlysis-3.4.5/conf/manifest.conf
--rw-rw-r--   0 axelle    (1000) axelle    (1000)    14426 2022-06-28 05:53:13.000000 droidlysis-3.4.5/conf/smali.conf
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     1853 2021-08-19 09:28:51.000000 droidlysis-3.4.5/conf/sortconf.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     2396 2022-06-14 09:05:27.000000 droidlysis-3.4.5/conf/wide.conf
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     5690 2023-05-15 15:46:42.000000 droidlysis-3.4.5/droidconfig.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     6075 2023-02-23 13:17:45.000000 droidlysis-3.4.5/droidcountry.py
--rwxrwxr-x   0 axelle    (1000) axelle    (1000)      226 2023-02-23 13:17:45.000000 droidlysis-3.4.5/droidlysis
-drwxrwxr-x   0 axelle    (1000) axelle    (1000)        0 2023-05-15 16:01:30.391940 droidlysis-3.4.5/droidlysis.egg-info/
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     9760 2023-05-15 16:01:30.000000 droidlysis-3.4.5/droidlysis.egg-info/PKG-INFO
--rw-rw-r--   0 axelle    (1000) axelle    (1000)      515 2023-05-15 16:01:30.000000 droidlysis-3.4.5/droidlysis.egg-info/SOURCES.txt
--rw-rw-r--   0 axelle    (1000) axelle    (1000)        1 2023-05-15 16:01:30.000000 droidlysis-3.4.5/droidlysis.egg-info/dependency_links.txt
--rw-rw-r--   0 axelle    (1000) axelle    (1000)       94 2023-05-15 16:01:30.000000 droidlysis-3.4.5/droidlysis.egg-info/requires.txt
--rw-rw-r--   0 axelle    (1000) axelle    (1000)      122 2023-05-15 16:01:30.000000 droidlysis-3.4.5/droidlysis.egg-info/top_level.txt
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     9508 2023-05-15 15:25:16.000000 droidlysis-3.4.5/droidlysis3.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     9831 2023-05-15 15:57:21.000000 droidlysis-3.4.5/droidproperties.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)    13295 2023-02-23 13:17:45.000000 droidlysis-3.4.5/droidreport.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)    52901 2023-05-15 14:59:10.000000 droidlysis-3.4.5/droidsample.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     1191 2023-03-10 15:08:56.000000 droidlysis-3.4.5/droidsql.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     5140 2023-02-23 13:17:45.000000 droidlysis-3.4.5/droidurl.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)    10903 2023-02-23 13:17:45.000000 droidlysis-3.4.5/droidutil.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     4907 2023-02-23 13:17:45.000000 droidlysis-3.4.5/droidziprar.py
--rw-rw-r--   0 axelle    (1000) axelle    (1000)       38 2023-05-15 16:01:30.391940 droidlysis-3.4.5/setup.cfg
--rw-rw-r--   0 axelle    (1000) axelle    (1000)     1359 2023-05-15 16:01:18.000000 droidlysis-3.4.5/setup.py
+drwxrwxr-x   0 axelle    (1000) axelle    (1000)        0 2024-04-12 11:11:52.463220 droidlysis-3.4.7/
+-rw-r--r--   0 axelle    (1000) axelle    (1000)     1057 2019-06-03 07:49:35.000000 droidlysis-3.4.7/LICENSE
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)       45 2020-03-02 08:15:52.000000 droidlysis-3.4.7/MANIFEST.in
+-rw-r--r--   0 axelle    (1000) axelle    (1000)    11015 2024-04-12 11:11:52.459220 droidlysis-3.4.7/PKG-INFO
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)    10240 2024-04-12 10:59:58.000000 droidlysis-3.4.7/README.md
+drwxrwxr-x   0 axelle    (1000) axelle    (1000)        0 2024-04-12 11:11:52.431220 droidlysis-3.4.7/conf/
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)        0 2020-03-02 08:09:36.000000 droidlysis-3.4.7/conf/__init__.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     2013 2024-02-12 10:50:28.000000 droidlysis-3.4.7/conf/arm.conf
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     3346 2021-02-18 13:02:54.000000 droidlysis-3.4.7/conf/exodustrack.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)      294 2024-04-12 10:46:49.000000 droidlysis-3.4.7/conf/general.conf
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)    63381 2024-04-12 11:10:44.000000 droidlysis-3.4.7/conf/kit.conf
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     1935 2024-02-12 10:37:07.000000 droidlysis-3.4.7/conf/manifest.conf
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)    17417 2024-04-12 10:56:21.000000 droidlysis-3.4.7/conf/smali.conf
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     1853 2021-02-18 13:02:54.000000 droidlysis-3.4.7/conf/sortconf.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     2396 2022-06-13 09:28:37.000000 droidlysis-3.4.7/conf/wide.conf
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     6605 2024-04-12 10:59:58.000000 droidlysis-3.4.7/droidconfig.py
+-rw-r--r--   0 axelle    (1000) axelle    (1000)     6075 2023-02-21 13:28:16.000000 droidlysis-3.4.7/droidcountry.py
+-rwxrw-r--   0 axelle    (1000) axelle    (1000)      226 2022-01-27 12:02:01.000000 droidlysis-3.4.7/droidlysis
+drwxrwxr-x   0 axelle    (1000) axelle    (1000)        0 2024-04-12 11:11:52.459220 droidlysis-3.4.7/droidlysis.egg-info/
+-rw-r--r--   0 axelle    (1000) axelle    (1000)    11015 2024-04-12 11:11:52.000000 droidlysis-3.4.7/droidlysis.egg-info/PKG-INFO
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)      565 2024-04-12 11:11:52.000000 droidlysis-3.4.7/droidlysis.egg-info/SOURCES.txt
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)        1 2024-04-12 11:11:52.000000 droidlysis-3.4.7/droidlysis.egg-info/dependency_links.txt
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)       94 2024-04-12 11:11:52.000000 droidlysis-3.4.7/droidlysis.egg-info/requires.txt
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)      122 2024-04-12 11:11:52.000000 droidlysis-3.4.7/droidlysis.egg-info/top_level.txt
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     9175 2024-04-12 11:02:15.000000 droidlysis-3.4.7/droidlysis3.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     9912 2024-02-12 10:37:07.000000 droidlysis-3.4.7/droidproperties.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)    13295 2023-03-10 13:39:17.000000 droidlysis-3.4.7/droidreport.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)    53952 2024-04-12 10:59:58.000000 droidlysis-3.4.7/droidsample.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     1191 2023-03-10 13:12:53.000000 droidlysis-3.4.7/droidsql.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     5140 2023-02-21 14:30:46.000000 droidlysis-3.4.7/droidurl.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)    10903 2023-02-21 14:43:02.000000 droidlysis-3.4.7/droidutil.py
+-rw-r--r--   0 axelle    (1000) axelle    (1000)     4907 2023-02-21 14:43:02.000000 droidlysis-3.4.7/droidziprar.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)       38 2024-04-12 11:11:52.463220 droidlysis-3.4.7/setup.cfg
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)     1359 2024-04-12 10:42:09.000000 droidlysis-3.4.7/setup.py
+drwxrwxr-x   0 axelle    (1000) axelle    (1000)        0 2024-04-12 11:11:52.451220 droidlysis-3.4.7/test/
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)      546 2023-05-16 09:22:18.000000 droidlysis-3.4.7/test/test_droidconfig.py
+-rw-rw-r--   0 axelle    (1000) axelle    (1000)      673 2023-05-16 09:28:52.000000 droidlysis-3.4.7/test/test_droidlysis3.py
```

### Comparing `droidlysis-3.4.5/LICENSE` & `droidlysis-3.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.5/PKG-INFO` & `droidlysis-3.4.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,91 +1,60 @@
-Metadata-Version: 2.1
-Name: droidlysis
-Version: 3.4.5
-Summary: DroidLysis: pre-analysis of suspicious Android samples
-Home-page: https://github.com/cryptax/droidlysis
-Author: @cryptax
-Author-email: aafortinet@gmail.com
-License: MIT
-Keywords: android malware reverse
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Development Status :: 3 - Alpha
-Classifier: Operating System :: Unix
-Classifier: Topic :: Software Development :: Disassemblers
-Requires-Python: >=3.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # DroidLysis
 
 DroidLysis is a **pre-analysis tool for Android apps**: it performs repetitive and boring tasks we'd typically do at the beginning of any reverse engineering. It disassembles the Android sample, organizes output in directories, and searches for suspicious spots in the code to look at.
 The output helps the reverse engineer speed up the first few steps of analysis.
 
 DroidLysis can be used over Android packages (apk), Dalvik executables (dex), Zip files (zip), Rar files (rar) or directories of files.
 
-<img src="https://img.shields.io/badge/PyPi%20-3.4.5-blue">
-
-## Quick setup
-
-Can't wait to use DroidLysis? Then, use a Docker container:
-
-```
-$ docker pull cryptax/droidlysis:2023.05
-$ docker run -it --rm -v /tmp/share:/share cryptax/droidlysis:2023.05  /bin/bash
-$ cd /opt/droidlysis
-$ python3 ./droidlysis3.py --help
-```
+<img src="https://img.shields.io/badge/PyPi%20-3.4.7-blue">
 
 ## Installing DroidLysis
 
 1. Install required system packages
 
 ```
 sudo apt-get install default-jre git python3 python3-pip unzip wget libmagic-dev libxml2-dev libxslt-dev
 ```
 
 
 2. Install Android disassembly tools
 
-[Apktool](https://ibotpeaches.github.io/Apktool/) , 
-[Baksmali](https://bitbucket.org/JesusFreke/smali/downloads), and optionally 
-[Dex2jar](https://github.com/pxb1988/dex2jar) and  
-[Procyon](https://bitbucket.org/mstrobel/procyon/wiki/Java%20Decompiler) (note that Procyon only works with Java 8, not Java 11).
+- [Apktool](https://ibotpeaches.github.io/Apktool/) , 
+- [Baksmali](https://bitbucket.org/JesusFreke/smali/downloads), and optionally 
+- [Dex2jar](https://github.com/pxb1988/dex2jar) and 
 
 ```
 $ mkdir -p ~/softs
 $ cd ~/softs
-$ wget https://bitbucket.org/iBotPeaches/apktool/downloads/apktool_2.7.0.jar
+$ wget https://bitbucket.org/iBotPeaches/apktool/downloads/apktool_2.9.3.jar
 $ wget https://bitbucket.org/JesusFreke/smali/downloads/baksmali-2.5.2.jar
-$ wget https://github.com/pxb1988/dex2jar/releases/download/v2.2-SNAPSHOT-2021-10-31/dex-tools-2.2-SNAPSHOT-2021-10-31.zip
-$ unzip dex-tools-2.2-SNAPSHOT-2021-10-31.zip 
-$ rm -f dex-tools-2.2-SNAPSHOT-2021-10-31.zip 
+$ wget https://github.com/pxb1988/dex2jar/releases/download/v2.4/dex-tools-v2.4.zip
+$ unzip dex-tools-v2.4.zip 
+$ rm -f dex-tools-v2.4.zip 
 ```
 
 3. Get DroidLysis from the Git repository (preferred) or from pip
 
-Install from Git in a Python virtual environment:
+Install from Git in a Python virtual environment (`python3 -m venv`, or pyenv virtual environments etc).
 
 ```
 $ python3 -m venv venv
 $ source ./venv/bin/activate
 (venv) $ pip3 install git+https://github.com/cryptax/droidlysis
 ```
 
 Alternatively, you can install DroidLysis directly from PyPi (`pip3 install droidlysis`).
 
 4. Configure `conf/general.conf`. In particular make sure to change `/home/axelle` with your appropriate directories.
 
 ```
 [tools]
-apktool = /home/axelle/softs/apktool_2.7.0.jar
+apktool = /home/axelle/softs/apktool_2.9.3.jar
 baksmali = /home/axelle/softs/baksmali-2.5.2.jar
-dex2jar = /home/axelle/softs/dex-tools-2.2-SNAPSHOT/d2j-dex2jar.sh
-procyon = /home/axelle/softs/procyon-decompiler-0.5.30.jar
+dex2jar = /home/axelle/softs/dex-tools-v2.4/d2j-dex2jar.sh
 keytool = /usr/bin/keytool
 ...
 ```
 
 5. Run it:
 
 ```
@@ -110,15 +79,15 @@
 ```
 droidlysis --help
 ```
 
 For example, test it on [Signal's APK](https://signal.org/android/apk/):
 
 ```
-droidlysis --input Signal-website-universal-release-4.52.4.apk --output /tmp
+droidlysis --input Signal-website-universal-release-6.26.3.apk --output /tmp --config /PATH/TO/DROIDLYSIS/conf/general.conf
 ```
 
 ![](./images/example.png)
 
 DroidLysis outputs:
 
 - A summary on the console (see image above)
@@ -129,16 +98,14 @@
 
 Get usage with `droidlysis --help`
 
 - The input can be a file or a directory of files to recursively look into. DroidLysis knows how to process Android packages, DEX, ODEX and ARM executables, ZIP, RAR. DroidLysis won't fail on other type of files (unless there is a bug...) but won't be able to understand the content.
 
 - When processing directories of files, it is typically quite helpful to move processed samples to another location to know what has been processed. This is handled by option `--movein`.  Also, if you are only interested in statistics, you should probably clear the output directory which contains detailed information for each sample: this is option `--clearoutput`. If you want to store all statistics in a SQL database, use `--enable-sql` (see [here](#sqlite_database))
 
-- DEX decompilation is quite long with Procyon, so this option is *disabled* by default. If you want to decompile to Java, use `--enable-procyon`.
-
 - DroidLysis's analysis does not inspect known 3rd party SDK by default, i.e. for instance it won't report any suspicious activity from these. If you want them to be inspected, use option `--no-kit-exception`. This usually creates many more detected properties for the sample, as SDKs (e.g. advertisment) use lots of flagged APIs (get GPS location, get IMEI, get IMSI, HTTP POST...).
 
 ## Sample output directory (`--output DIR`)
 
 This directory contains (when applicable):
 
 - A readable `AndroidManifest.xml`
@@ -152,14 +119,32 @@
 The following files are generated by DroidLysis:
 
 - `autoanalysis.md`: lists each pattern DroidLysis detected and where.
 - `report.md`: same as what was printed on the console
 
 If you do not need the sample output directory to be generated, use the option `--clearoutput`.
 
+## Import trackers from Exodus etc (`--import-exodus`)
+
+```
+$ python3 ./droidlysis3.py --import-exodus --verbose
+Processing file: ./droidurl.pyc ...
+DEBUG:droidconfig.py:Reading configuration file: './conf/./smali.conf'
+DEBUG:droidconfig.py:Reading configuration file: './conf/./wide.conf'
+DEBUG:droidconfig.py:Reading configuration file: './conf/./arm.conf'
+DEBUG:droidconfig.py:Reading configuration file: '/home/axelle/.cache/droidlysis/./kit.conf'
+DEBUG:droidproperties.py:Importing ETIP Exodus trackers from https://etip.exodus-privacy.eu.org/api/trackers/?format=json
+DEBUG:connectionpool.py:Starting new HTTPS connection (1): etip.exodus-privacy.eu.org:443
+DEBUG:connectionpool.py:https://etip.exodus-privacy.eu.org:443 "GET /api/trackers/?format=json HTTP/1.1" 200 None
+DEBUG:droidproperties.py:Appending imported trackers to /home/axelle/.cache/droidlysis/./kit.conf
+```
+
+Trackers from Exodus which are not present in your initial `kit.conf` are appended to `~/.cache/droidlysis/kit.conf`. Diff the 2 files and check what trackers you wish to add.
+
+
 ## SQLite database{#sqlite_database}
 
 If you want to process a directory of samples, you'll probably like to store the properties DroidLysis found in a database, to easily parse and query the findings. In that case, use the option `--enable-sql`. This will automatically dump all results in a database named `droidlysis.db`, in a table named `samples`. Each entry in the table is relative to a given sample. Each column is properties DroidLysis tracks.
 
 For example, to retrieve all filename, SHA256 sum and smali properties of the database:
 
 ```
@@ -201,17 +186,24 @@
 config.read(os.path.expanduser('~/.cache/droidlysis/kit.conf'))
 # Order all sections alphabetically
 config._sections = collections.OrderedDict(sorted(config._sections.items(), key=lambda t: t[0] ))
 with open('sorted.conf','w') as f:
     config.write(f)
 ```    
 
+## JEB script for smali properties
+
+This script helps you search for methods on JEB UI that contain code that matches the smali pattern and easily navigates to those functions. When you load the script and select `details.md` file among the droidlysis analysis files, a search box will appear. Once moved, you can easily bring up the search windows again by using recent script execution shortcut.
+
+- JEB > File > Scripts > Script selector > `script/DroidlysisSearch.py`
+- JEB > File > Scripts > Run last Script
 
 ## Updates
 
+- v3.4.6 - Detecting manifest feature that automatically loads APK at install
 - v3.4.5 - Creating a writable user kit.conf file
 - v3.4.4 - Bug fix #14
 - v3.4.3 - Using configuration files
 - v3.4.2 - Adding import of Exodus Privacy Trackers
 - v3.4.1 - Removed dependency to Androguard
 - v3.4.0 - Multidex support
 - v3.3.1 - Improving detection of Base64 strings
```

### Comparing `droidlysis-3.4.5/README.md` & `droidlysis-3.4.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,84 @@
+Metadata-Version: 2.1
+Name: droidlysis
+Version: 3.4.7
+Summary: DroidLysis: pre-analysis of suspicious Android samples
+Home-page: https://github.com/cryptax/droidlysis
+Author: @cryptax
+Author-email: aafortinet@gmail.com
+License: MIT
+Keywords: android malware reverse
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Development Status :: 3 - Alpha
+Classifier: Operating System :: Unix
+Classifier: Topic :: Software Development :: Disassemblers
+Requires-Python: >=3.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: configparser>=4.0.2
+Requires-Dist: python-magic==0.4.12
+Requires-Dist: requests
+Requires-Dist: SQLAlchemy>=1.1.1
+Requires-Dist: rarfile>=3.0
+Requires-Dist: platformdirs
+
 # DroidLysis
 
 DroidLysis is a **pre-analysis tool for Android apps**: it performs repetitive and boring tasks we'd typically do at the beginning of any reverse engineering. It disassembles the Android sample, organizes output in directories, and searches for suspicious spots in the code to look at.
 The output helps the reverse engineer speed up the first few steps of analysis.
 
 DroidLysis can be used over Android packages (apk), Dalvik executables (dex), Zip files (zip), Rar files (rar) or directories of files.
 
-<img src="https://img.shields.io/badge/PyPi%20-3.4.5-blue">
-
-## Quick setup
-
-Can't wait to use DroidLysis? Then, use a Docker container:
-
-```
-$ docker pull cryptax/droidlysis:2023.05
-$ docker run -it --rm -v /tmp/share:/share cryptax/droidlysis:2023.05  /bin/bash
-$ cd /opt/droidlysis
-$ python3 ./droidlysis3.py --help
-```
+<img src="https://img.shields.io/badge/PyPi%20-3.4.7-blue">
 
 ## Installing DroidLysis
 
 1. Install required system packages
 
 ```
 sudo apt-get install default-jre git python3 python3-pip unzip wget libmagic-dev libxml2-dev libxslt-dev
 ```
 
 
 2. Install Android disassembly tools
 
-[Apktool](https://ibotpeaches.github.io/Apktool/) , 
-[Baksmali](https://bitbucket.org/JesusFreke/smali/downloads), and optionally 
-[Dex2jar](https://github.com/pxb1988/dex2jar) and  
-[Procyon](https://bitbucket.org/mstrobel/procyon/wiki/Java%20Decompiler) (note that Procyon only works with Java 8, not Java 11).
+- [Apktool](https://ibotpeaches.github.io/Apktool/) , 
+- [Baksmali](https://bitbucket.org/JesusFreke/smali/downloads), and optionally 
+- [Dex2jar](https://github.com/pxb1988/dex2jar) and 
 
 ```
 $ mkdir -p ~/softs
 $ cd ~/softs
-$ wget https://bitbucket.org/iBotPeaches/apktool/downloads/apktool_2.7.0.jar
+$ wget https://bitbucket.org/iBotPeaches/apktool/downloads/apktool_2.9.3.jar
 $ wget https://bitbucket.org/JesusFreke/smali/downloads/baksmali-2.5.2.jar
-$ wget https://github.com/pxb1988/dex2jar/releases/download/v2.2-SNAPSHOT-2021-10-31/dex-tools-2.2-SNAPSHOT-2021-10-31.zip
-$ unzip dex-tools-2.2-SNAPSHOT-2021-10-31.zip 
-$ rm -f dex-tools-2.2-SNAPSHOT-2021-10-31.zip 
+$ wget https://github.com/pxb1988/dex2jar/releases/download/v2.4/dex-tools-v2.4.zip
+$ unzip dex-tools-v2.4.zip 
+$ rm -f dex-tools-v2.4.zip 
 ```
 
 3. Get DroidLysis from the Git repository (preferred) or from pip
 
-Install from Git in a Python virtual environment:
+Install from Git in a Python virtual environment (`python3 -m venv`, or pyenv virtual environments etc).
 
 ```
 $ python3 -m venv venv
 $ source ./venv/bin/activate
 (venv) $ pip3 install git+https://github.com/cryptax/droidlysis
 ```
 
 Alternatively, you can install DroidLysis directly from PyPi (`pip3 install droidlysis`).
 
 4. Configure `conf/general.conf`. In particular make sure to change `/home/axelle` with your appropriate directories.
 
 ```
 [tools]
-apktool = /home/axelle/softs/apktool_2.7.0.jar
+apktool = /home/axelle/softs/apktool_2.9.3.jar
 baksmali = /home/axelle/softs/baksmali-2.5.2.jar
-dex2jar = /home/axelle/softs/dex-tools-2.2-SNAPSHOT/d2j-dex2jar.sh
-procyon = /home/axelle/softs/procyon-decompiler-0.5.30.jar
+dex2jar = /home/axelle/softs/dex-tools-v2.4/d2j-dex2jar.sh
 keytool = /usr/bin/keytool
 ...
 ```
 
 5. Run it:
 
 ```
@@ -92,15 +103,15 @@
 ```
 droidlysis --help
 ```
 
 For example, test it on [Signal's APK](https://signal.org/android/apk/):
 
 ```
-droidlysis --input Signal-website-universal-release-4.52.4.apk --output /tmp
+droidlysis --input Signal-website-universal-release-6.26.3.apk --output /tmp --config /PATH/TO/DROIDLYSIS/conf/general.conf
 ```
 
 ![](./images/example.png)
 
 DroidLysis outputs:
 
 - A summary on the console (see image above)
@@ -111,16 +122,14 @@
 
 Get usage with `droidlysis --help`
 
 - The input can be a file or a directory of files to recursively look into. DroidLysis knows how to process Android packages, DEX, ODEX and ARM executables, ZIP, RAR. DroidLysis won't fail on other type of files (unless there is a bug...) but won't be able to understand the content.
 
 - When processing directories of files, it is typically quite helpful to move processed samples to another location to know what has been processed. This is handled by option `--movein`.  Also, if you are only interested in statistics, you should probably clear the output directory which contains detailed information for each sample: this is option `--clearoutput`. If you want to store all statistics in a SQL database, use `--enable-sql` (see [here](#sqlite_database))
 
-- DEX decompilation is quite long with Procyon, so this option is *disabled* by default. If you want to decompile to Java, use `--enable-procyon`.
-
 - DroidLysis's analysis does not inspect known 3rd party SDK by default, i.e. for instance it won't report any suspicious activity from these. If you want them to be inspected, use option `--no-kit-exception`. This usually creates many more detected properties for the sample, as SDKs (e.g. advertisment) use lots of flagged APIs (get GPS location, get IMEI, get IMSI, HTTP POST...).
 
 ## Sample output directory (`--output DIR`)
 
 This directory contains (when applicable):
 
 - A readable `AndroidManifest.xml`
@@ -134,14 +143,32 @@
 The following files are generated by DroidLysis:
 
 - `autoanalysis.md`: lists each pattern DroidLysis detected and where.
 - `report.md`: same as what was printed on the console
 
 If you do not need the sample output directory to be generated, use the option `--clearoutput`.
 
+## Import trackers from Exodus etc (`--import-exodus`)
+
+```
+$ python3 ./droidlysis3.py --import-exodus --verbose
+Processing file: ./droidurl.pyc ...
+DEBUG:droidconfig.py:Reading configuration file: './conf/./smali.conf'
+DEBUG:droidconfig.py:Reading configuration file: './conf/./wide.conf'
+DEBUG:droidconfig.py:Reading configuration file: './conf/./arm.conf'
+DEBUG:droidconfig.py:Reading configuration file: '/home/axelle/.cache/droidlysis/./kit.conf'
+DEBUG:droidproperties.py:Importing ETIP Exodus trackers from https://etip.exodus-privacy.eu.org/api/trackers/?format=json
+DEBUG:connectionpool.py:Starting new HTTPS connection (1): etip.exodus-privacy.eu.org:443
+DEBUG:connectionpool.py:https://etip.exodus-privacy.eu.org:443 "GET /api/trackers/?format=json HTTP/1.1" 200 None
+DEBUG:droidproperties.py:Appending imported trackers to /home/axelle/.cache/droidlysis/./kit.conf
+```
+
+Trackers from Exodus which are not present in your initial `kit.conf` are appended to `~/.cache/droidlysis/kit.conf`. Diff the 2 files and check what trackers you wish to add.
+
+
 ## SQLite database{#sqlite_database}
 
 If you want to process a directory of samples, you'll probably like to store the properties DroidLysis found in a database, to easily parse and query the findings. In that case, use the option `--enable-sql`. This will automatically dump all results in a database named `droidlysis.db`, in a table named `samples`. Each entry in the table is relative to a given sample. Each column is properties DroidLysis tracks.
 
 For example, to retrieve all filename, SHA256 sum and smali properties of the database:
 
 ```
@@ -183,17 +210,24 @@
 config.read(os.path.expanduser('~/.cache/droidlysis/kit.conf'))
 # Order all sections alphabetically
 config._sections = collections.OrderedDict(sorted(config._sections.items(), key=lambda t: t[0] ))
 with open('sorted.conf','w') as f:
     config.write(f)
 ```    
 
+## JEB script for smali properties
+
+This script helps you search for methods on JEB UI that contain code that matches the smali pattern and easily navigates to those functions. When you load the script and select `details.md` file among the droidlysis analysis files, a search box will appear. Once moved, you can easily bring up the search windows again by using recent script execution shortcut.
+
+- JEB > File > Scripts > Script selector > `script/DroidlysisSearch.py`
+- JEB > File > Scripts > Run last Script
 
 ## Updates
 
+- v3.4.6 - Detecting manifest feature that automatically loads APK at install
 - v3.4.5 - Creating a writable user kit.conf file
 - v3.4.4 - Bug fix #14
 - v3.4.3 - Using configuration files
 - v3.4.2 - Adding import of Exodus Privacy Trackers
 - v3.4.1 - Removed dependency to Androguard
 - v3.4.0 - Multidex support
 - v3.3.1 - Improving detection of Base64 strings
```

### Comparing `droidlysis-3.4.5/conf/arm.conf` & `droidlysis-3.4.7/conf/arm.conf`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 
 [geteuid]
 pattern=geteuid
 
 [adb]
 pattern=sbin/adb
 
+[anti-frida]
+pattern=gum-js-loop|frida-helper|frida-server|frida-agent|re.frida.server|linjector|gdbus|frida-gadget|pool-frida|frida-main-loop|frida_agent_main|pool-spawner|DetectFrida
+description=Anti runtime analysis - Detect frida framework
+
 [pm_install]
 pattern=pm install
 
 [pm_list]
 pattern=pm list
 
 [am_broadcast]
```

### Comparing `droidlysis-3.4.5/conf/exodustrack.py` & `droidlysis-3.4.7/conf/exodustrack.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.5/conf/kit.conf` & `droidlysis-3.4.7/conf/kit.conf`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 [acrarium]
 description = Acrarium (from ETIP Exodus Privacy list)
 pattern = com/faendir/acra
 
 [acrcloud]
 pattern = com/acrcloud
 
+[actmobile]
+pattern = com/actmobile
+description = ActMobile Network licensing
+
 [actv8me]
 pattern = me/actv8
 
 [acuant]
 pattern = com/acuant/acuantcamera
 
 [ad2]
@@ -324,15 +328,15 @@
 pattern = com/amazon/identity/auth
 
 [amap]
 pattern = com/amap/api
 description = Amap Map Provider
 
 [amazon]
-pattern = com/amazon/venezia/service|com/amazon/inapp/purchasing|com/amazonaws/services|com/amazon/device|com/amazon/insights
+pattern = com/amazon/venezia/service|com/amazon/inapp/purchasing|com/amazonaws/services|com/amazon/device|com/amazon/insights|com/amazon/aps
 
 [amazonads]
 pattern = com/amazon/device/ads
 description = Amazon DTB Ads API
 
 [amazonmobileanalyticsamplify]
 description = Amazon Mobile Analytics (Amplify) (from ETIP Exodus Privacy list)
@@ -398,20 +402,25 @@
 description = Basic For Android (B4A)
 
 [anzu]
 description = Anzu (from ETIP Exodus Privacy list)
 pattern = com/anzu/sdk
 
 [apache]
-pattern = org/apache/commons/
+pattern = org/apache/|schemaorg_apache_xmlbeans
+description = Apache library (HTTP, XML...)
 
 [apicloud]
 description = APICloud (from ETIP Exodus Privacy list)
 pattern = com/apicloud
 
+[apm]
+pattern = com/apm/insight
+description = APM Insight crash analytics
+
 [appanalytics]
 pattern = io/appanalytics/sdk
 
 [appbrain]
 pattern = com/appbrain
 description = AppBrain marketplace
 
@@ -460,14 +469,18 @@
 
 [applovin]
 pattern = com/applovin
 
 [appmedia]
 pattern = cn/appmedia/ad/
 
+[appmattus]
+pattern = com/appmattus/certificatetransparency
+description = Certificate Transparency library
+
 [appmonet]
 pattern = com/monet
 
 [appnext]
 pattern = com/appnext
 
 [appnexus]
@@ -526,14 +539,17 @@
 [areametrics]
 pattern = com/areametrics/areametricssdk
 
 [askingpoint]
 description = Askingpoint (from ETIP Exodus Privacy list)
 pattern = com/askingpoint
 
+[aspose]
+pattern = com/aspose
+
 [atinternet]
 pattern = com/atinternet
 
 [auditude]
 pattern = com/auditude/ads
 
 [avazuanative]
@@ -568,14 +584,18 @@
 
 [badlogic]
 pattern = com/badlogic/gdx
 
 [baidu]
 pattern = com/baidu/
 
+[balysv]
+pattern = com/balysv/
+description = Animations for Android L
+
 [bangcle]
 pattern = com/secapk/wrapper
 
 [batch]
 pattern = com/batch/android
 
 [bazaarvoice]
@@ -602,14 +622,18 @@
 [bidmachine]
 description = BidMachine (from ETIP Exodus Privacy list)
 pattern = io/bidmachine
 
 [bigkoo]
 pattern = com/bigkoo/pickerview
 
+[bilibili]
+pattern = com/bapis/bilibili|tv/danmaku
+description = Bilibili marketing platform
+
 [bitlabs]
 description = BitLabs (from ETIP Exodus Privacy list)
 pattern = ai/bitlabs/sdk
 
 [bitly]
 pattern = com/bitly/Bitly
 
@@ -683,14 +707,17 @@
 [bugsnag]
 pattern = com/bugsnag
 
 [bumptech]
 pattern = com/bumptech/glide
 description = Bumptech Glide Image loading and caching library
 
+[burhanrashid]
+pattern = ja/burhanrashid52/photoeditor
+
 [burstly]
 pattern = com/burstly/lib
 
 [butterknife]
 pattern = butterknife/internal
 
 [buzzadbenefit]
@@ -713,14 +740,18 @@
 
 [carnival]
 pattern = com/carnival/sdk|com/canivalmobile
 
 [carto]
 pattern = com/nutiteq|com/carto
 
+[caverock]
+pattern = com/caverock/androidsvg
+description = CaveRock Android SVG parser and renderer
+
 [cauly]
 pattern = com/fsn/cauly|com/trid/tridad
 
 [cedexisradar]
 description = Cedexis Radar (from ETIP Exodus Privacy list)
 pattern = com/cedexis
 
@@ -776,14 +807,17 @@
 pattern = com/microsoft/codepush
 description = CodePush - to update apps live
 
 [codewaves]
 pattern = com/codewaves/stickyheadergrid
 description = Sticky header grid layout manager for RecycleView
 
+[colorpicker]
+pattern = com/github/danielnilsson9/colorpickerview
+
 [comscore]
 pattern = com/comscore
 
 [contentsquare]
 description = Contentsquare (from ETIP Exodus Privacy list)
 pattern = com/contentsquare/android
 
@@ -840,14 +874,19 @@
 [dagger]
 pattern = dagger/internal
 
 [daochengthinkyeah]
 description = DaoCheng(Thinkyeah) (from ETIP Exodus Privacy list)
 pattern = com/thinkyeah/common
 
+[darkside]
+pattern = com/avstaim/darkside
+description = Dark Side - Android developer tools for Kotlin
+
+
 [databox]
 description = Databox (from ETIP Exodus Privacy list)
 pattern = com/databox
 
 [datadog]
 description = Datadog (from ETIP Exodus Privacy list)
 pattern = com/datadoghq
@@ -896,34 +935,41 @@
 description = Discord Telemetry (from ETIP Exodus Privacy list)
 pattern = com/discord/analytics
 
 [display]
 pattern = io/display
 
 [dom4j]
-pattern = org/dom4j/dom
+pattern = org/dom4j/
 description = Dom4j
 
 [domob]
 pattern = cn/domob/android
 description = Domob.cn
 
+[dooboo]
+pattern = com/dooboolab/tauengine
+
 [dove]
 pattern = com/dv/
 description = DOV-E
 
 [duapps]
 pattern = com/duapps
 
 [dynamicyield]
 pattern = com/dynamicyield
 
 [dynatrace]
 pattern = com/dynatrace/android/app
 
+[eftimov]
+description = View Pager transformers
+pattern = com/eftimoff/
+
 [ehawk]
 pattern = com/hawk
 
 [elonen]
 pattern = fi/iki/elonen
 description = Simple Web Server
 
@@ -931,15 +977,16 @@
 pattern = com/elvishew/xlog
 description = Elvishew Logger
 
 [emagsoft]
 pattern = cn/emagsoftware/gamebilling
 
 [emarsys]
-pattern = com/emarsys/predict
+pattern = com/emarsys/predict|com/emarsys/core
+description = Emarsys Engage
 
 [embrace]
 description = Embrace (from ETIP Exodus Privacy list)
 pattern = io/embrace/android/embracesdk
 
 [energysource]
 pattern = com/energysource/szj/embeded
@@ -1031,16 +1078,24 @@
 pattern = jp/fluct/fluctsdk
 
 [flurry]
 pattern = com/flurry
 description = Flurry analytics
 
 [flutter]
-pattern = com/wisecrab/wc_flutter_share|com/pichillilorenzo/flutter_inappwebview
-description = Flutter or its plugins
+pattern = io/flutter/plugin/common|io/flutter/embedding/android
+description = Flutter SDK
+
+[flutter_libphonenumber]
+description = Libphonenumber - Asynchronous and synchronous formatting of phone numbers in Flutter apps - https://github.com/acoutts/flutter_libphonenumber
+pattern = com/bottlepay/flutter_libphonenumber
+
+[flutter_local_notifications]
+description = Flutter Local Notifications
+pattern = com/dexterous/flutterlocalnotifications - https://github.com/MaikuB/flutter_local_notifications
 
 [fluzo]
 pattern = com/fluzo/sdk
 
 [flymob]
 pattern = com/flymob/sdk
 
@@ -1142,55 +1197,36 @@
 description = GOM Factory AdPie (from ETIP Exodus Privacy list)
 pattern = com/gomfactory/adpie
 
 [googleads]
 pattern = com/google/ads
 
 [googleapis]
-pattern = com/google/api/services|com/google/api/client/googleapis|com/google/api/client/
+pattern = com/google/api/services|com/google/api/client/googleapis|com/google/api/client/|com/google/common/
 description = Google API Services
 
-[googleauth]
-pattern = com/google/api/client/auth
-
 [googlec2dm]
 description = Google C2DM
 pattern = com/google/android/c2dm
 
-[googlecloudaudit]
-description = Google Cloud Audit (from ETIP Exodus Privacy list)
-pattern = com/google/cloud/audit
-
 [googlecrashlytics]
 description = Google CrashLytics (from ETIP Exodus Privacy list)
 pattern = io/fabric|com/crashlytics|com/google/firebase/crashlytics|com/google/firebase/crash|io/invertase/firebase/crashlytics
 
 [googledrive]
 pattern = com/google/api/services/drive
 
-[googlegcm]
-pattern = com/google/android/gcm
-
-[googlegson]
-pattern = com/google/gson/
-
-[googlehttp]
-pattern = com/google/api/http/
-
-[googlelibraries]
-pattern = com/google/android/libraries
+[googlemisc]
+pattern = com/google/android/gcm|com/google/android/gms|com/google/gson/|com/google/api/http/|com/google/android/libraries|com/google/mlkit|com/google/cloud/audit|com/google/api/client/auth
+description = Google various services
 
 [googlemaps]
 pattern = com/google/android/maps|com/google/android/geo|com/google/android/gms/maps
 description = Google Maps
 
-[googlemlkit]
-description = Google ML Kit (from ETIP Exodus Privacy list)
-pattern = com/google/mlkit
-
 [googleplay]
 pattern = com/google/android/play/core
 description = Google Play Core
 
 [googleplaybilling]
 pattern = com/android/billing
 description = Google Play Billing Library Service
@@ -1291,17 +1327,14 @@
 [houndify]
 pattern = com/hound
 
 [houseads]
 description = Houseads (from ETIP Exodus Privacy list)
 pattern = houseads
 
-[http]
-pattern = org/apache/http/
-
 [huawei]
 pattern = com/huawei/hms/analytics
 description = Huawei Mobile Services
 
 [huntmads]
 pattern = com/huntmads/admobadaptor
 
@@ -1403,14 +1436,18 @@
 description = IntroMi (from ETIP Exodus Privacy list)
 pattern = com/ad/intromi
 
 [ipquality]
 pattern = com/ipqualityscore
 description = IP Quality Score
 
+[iproov]
+pattern = com/iproov/sdk
+description = Biometric face verification SDK (https://github.com/iProov/android)
+
 [iqv]
 description = IQV (from ETIP Exodus Privacy list)
 pattern = com/iqv
 
 [iqzone]
 pattern = com/iqzone
 
@@ -1418,14 +1455,18 @@
 description = iridge popinfo (from ETIP Exodus Privacy list)
 pattern = jp/iridge/popinfo
 
 [ironsource]
 description = ironSource tracking API
 pattern = com/ironsource
 
+[itextpdf]
+pattern = com/itextpdf/
+description = iText PDF Library
+
 [iusys828]
 pattern = net/iusys828
 description = Iusys
 
 [izp]
 pattern = com/izp/views/
 
@@ -1435,26 +1476,37 @@
 
 [jackpal]
 pattern = jackpal/androidterm/Exec
 
 [jackson]
 pattern = org/codehaus/jackson/
 
+[jailmonkey]
+pattern = com/gantix/JailMonkey
+description = React Native JailMonkey root detection
+
 [janrain]
 pattern = com/janrain/android
 
+[javaxml]
+pattern = javax/xml/
+description = Java XML
+
 [jaxen]
 pattern = org/jaxen/
 
 [jcip]
 pattern = net/jcip/
 
 [jetbrains]
 pattern = org/jetbrains/
 
+[journeyapps]
+pattern = com/journeyapps/barcodescanner
+
 [jose]
 pattern = com/nimbusds/jose
 description = Nimbus JOSE
 
 [jpush]
 pattern = cn/jpush/android
 description = JiGuang Aurora Mobile JPush
@@ -1472,14 +1524,18 @@
 
 [jumio]
 pattern = com/jumio/MobileSDK
 
 [jumptap]
 pattern = com/jumptap/adtag
 
+[junit]
+pattern = junit|org/junit/
+description = JUnit
+
 [junrar]
 pattern = com/github/junrar
 
 [jwplayer]
 pattern = com/longtailvideo/jwplayer
 
 [jwt]
@@ -1516,16 +1572,20 @@
 
 [kochava]
 pattern = com/kochava/base
 
 [kontakt]
 pattern = com/kontakt/sdk/android
 
+[koom]
+description = Koom performance online memory monitoring
+pattern = com/kwai/koom/javaoom
+
 [kotlin]
-pattern = kotlin/coroutines/jvm|kotlin/internal|kotlinx/coroutines
+pattern = kotlin/coroutines/jvm|kotlin/internal|kotlinx/coroutines|kotlin/jvm/internal|kotlin/collections
 description = Kotlin framework
 
 [krux]
 pattern = com/krux/androidsdk
 description = Audience Studio
 
 [kuaiyou]
@@ -1644,15 +1704,15 @@
 description = Mapbox Location Telemetry
 
 [marketo]
 pattern = com/marketo
 description = Marketo (an Adobe company)
 
 [material]
-pattern = com/google/android/material
+pattern = com/google/android/material|me/zhanghai/android/materialprogressbar
 description = Material.IO design system
 
 [matomopiwik]
 description = Matomo (Piwik) (from ETIP Exodus Privacy list)
 pattern = org/piwik|org/piwik/mobile|org/matomo
 
 [mdotm]
@@ -1779,25 +1839,33 @@
 [mopub]
 pattern = com/mopub/mobileads
 
 [morgoopacker]
 description = Morgoo Packer (from ETIP Exodus Privacy list)
 pattern = com/morgoo/droidplugin
 
+[morphingbutton]
+description = Android Morphing Button
+pattern = com/dd/morphingbutton/
+
 [mozilla]
 pattern = org/mozilla/telemetry
 description = Mozilla Telemetry
 
 [mozillacrashreport]
 description = Mozilla Crashreport (from ETIP Exodus Privacy list)
 pattern = mozilla/components/lib/crash/service
 
 [mparticle]
 pattern = com/mparticle
 
+[msebera]
+pattern = com/msebera/android/httpclient
+description = MSebera Http Client
+
 [mtractionmfaas]
 description = mTraction (mFaaS) (from ETIP Exodus Privacy list)
 pattern = com/mtraction/mtractioninapptracker
 
 [mytarget]
 pattern = com/my/target
 
@@ -1876,16 +1944,16 @@
 description = React Native Keychain and Vector icons
 
 [offertoro]
 description = OfferToro (from ETIP Exodus Privacy list)
 pattern = com/offertoro/sdk
 
 [ogury]
-description = Ogury (from ETIP Exodus Privacy list)
-pattern = com/ogury/cm|com/ogury/analytics|com/ogury/consent|com/ogury/sdk
+description = Ogury Content Manager
+pattern = com/ogury
 
 [ogurypresage]
 pattern = io/presage
 
 [okhttp]
 description = Square OkHttp client for Android
 pattern = okhttp3
@@ -1945,14 +2013,18 @@
 [opentracker]
 pattern = net/opentracker/android
 
 [openudid]
 description = OpenUDID (from ETIP Exodus Privacy list)
 pattern = org/openudid|org/OpenUDID
 
+[openvk]
+pattern = com/bykv/vk/openvk
+description = OpenVK implementations
+
 [openx]
 pattern = com/openx/view/plugplay
 
 [optimizely]
 pattern = com/optimizely
 
 [orhanobut]
@@ -1968,17 +2040,21 @@
 
 [outbrain]
 pattern = com/outbrain
 
 [oztam]
 pattern = au/com/oztam
 
+[pablo]
+pattern = pablo/team/viewer
+description = Pablo Team Viewer
+
 [pangle]
-description = Pangle (from ETIP Exodus Privacy list)
-pattern = com/bytedance/sdk/openadsdk|com/bytedance/tea/crash|com/bytedance/embedapplog|com/bytedance/applog
+description = Pangle SDK
+pattern = com/pgl|com/bytedance|com/pangle/global
 
 [papaya]
 pattern = com/papaya/social|com/papaya/offer
 
 [parse]
 description = Parse (from ETIP Exodus Privacy list)
 pattern = com/parse/Parse|com/parse/PushServiceApi
@@ -2172,14 +2248,18 @@
 description = Raygun (from ETIP Exodus Privacy list)
 pattern = com/mindscapehq/android/raygun4android
 
 [react]
 pattern = com/react|com/reactnative|com/reactnativecommunity
 description = React Native
 
+[reactivestreams]
+pattern = org/reactivestreams
+description = Reactive Streams
+
 [reactnativefabric]
 description = react-native-fabric (from ETIP Exodus Privacy list)
 pattern = com/smixx/fabric
 
 [receptiv]
 pattern = com/mediabrix/android
 description = Receptiv (formerly Mediabrix)
@@ -2300,14 +2380,17 @@
 [sentiance]
 pattern = com/sentiance/sdk
 
 [sentry]
 pattern = io/sentry
 description = Application Monitoring and Error Tracking Software
 
+[sephiroth]
+pattern = it/sephiroth/android/library
+
 [seventynine]
 description = Seventynine (from ETIP Exodus Privacy list)
 pattern = seventynine/sdk
 
 [shallwead]
 pattern = com/jm/co/shallwead/sdk
 
@@ -2406,15 +2489,15 @@
 [split]
 pattern = io/split/android
 
 [splunkmint]
 pattern = com/splunk/mint
 
 [spongycastle]
-pattern = org/spngycastle
+pattern = org/spongycastle
 
 [sponsorpay]
 pattern = com/sponsorpay/sdk/android/advertiser
 description = Fyber SponsorPay
 
 [spoteerarc]
 description = Spoteer Arc (from ETIP Exodus Privacy list)
@@ -2563,18 +2646,25 @@
 [tenjin]
 pattern = com/tenjin/android
 
 [thalitor]
 pattern = com/msopentech/thali/android/toronionproxy
 description = Tor Onion Proxy Library
 
+[theartofdev]
+pattern = com/theartofdev/edmodo/cropper
+
 [theoremreach]
 description = TheoremReach (from ETIP Exodus Privacy list)
 pattern = theoremreach/com/theoremreach
 
+[thindownloadmanager]
+pattern = com/thin/downloadmanager
+description = ThinDownloadManager download library - https://github.com/smanikandan14/ThinDownloadManager - bypasses DOWNLOAD_WITHOUT_NOTIFICATION
+
 [thinkingdataanalytics]
 description = ThinkingData Analytics (from ETIP Exodus Privacy list)
 pattern = cn/thinkingdata
 
 [tiktoksdk]
 description = TikTok SDK (from ETIP Exodus Privacy list)
 pattern = com/muf/sdk/tiktok
@@ -2669,14 +2759,18 @@
 
 [umeng]
 pattern = com/umeng/
 
 [unacastpure]
 pattern = com/pure/internal
 
+[unionpay]
+pattern = com/unionpay/tsmservice
+description = UnionPay Trusted Service component
+
 [unity]
 description = Unity 3D Game Development
 pattern = com/unity3d/player|com/unity3d/ads|com/unity3d/services
 
 [unknowntrackers]
 description = Unknown Trackers (from ETIP Exodus Privacy list)
 pattern = qwapi/adclient/android/view|/MediaPlayerWrapper|/nbpcorp|com/ad/sdk|com/sen/sdk/sen|com/sen/websdk|/service/TrackerService|/service/Analytics|com/nextapps/naswall|/BannerActivity|/InterstitialActivity|com/bestgo/adsplugin|com/zero/ta/common|com/zjsoft/baseadlib|de/rocketinternet/android|com/yoc/sdk|com/yt/promolib|com/growstarry
@@ -2751,15 +2845,15 @@
 pattern = com/vpon/ads|com/vpon/adon/android
 
 [vserv]
 description = Vserv mobile advertising
 pattern = mobi/vserv/
 
 [vungle]
-pattern = com/vungle/publisher
+pattern = com/vungle/publisher|com/vungle/warren
 
 [walkmeabbiio]
 description = WalkMe/Abbi.io (from ETIP Exodus Privacy list)
 pattern = com/walkme/wmads|com/walkme/wmanalytics|com/walkme/wmcrosspromotion|abbi/io/abbisdk
 
 [wannads]
 description = Wannads (from ETIP Exodus Privacy list)
@@ -2769,14 +2863,18 @@
 description = Waps
 pattern = com/waps|cn/waps
 
 [wapstartplus1]
 description = WapStart.Plus1 (from ETIP Exodus Privacy list)
 pattern = ru/wapstart/plus1/sdk
 
+[wasabeef]
+pattern = jp/wasabeef/picasso
+description = Transformations for Glide
+
 [weather]
 pattern = com/go/weather/
 
 [webkit]
 pattern = org/webkit/
 
 [weborama]
@@ -2787,14 +2885,18 @@
 
 [webtrends]
 pattern = com/webtrends/mobile/analytics
 
 [wechatlocation]
 pattern = com/tencent/map/geolocation
 
+[weplan]
+description = Weplan (from ETIP Exodus Privacy list)
+pattern = com/cumberland/weplansdk
+
 [weibodeviceid]
 pattern = com/sina/deviceidjnisdk
 
 [widespace]
 pattern = com/widespace
 
 [wiyun]
@@ -2831,14 +2933,18 @@
 [ximad]
 pattern = com/ximad/ad
 
 [xmode]
 pattern = io/xmode
 description = X Mode SDK
 
+[xml]
+pattern = org/openxmlformats|org/xml/
+description = Open XML
+
 [xtremelabs]
 description = Xtreme Labs Image Utilities
 pattern = com/xtremelabs/imageutils|com/xtremelabs/utilities
 
 [xylink]
 pattern = com/xylink
 description = Video meetings
@@ -2917,14 +3023,18 @@
 
 [zestadz]
 pattern = com/zestadz/android
 
 [zhidian]
 pattern = com/adzhidian/ui
 
+[zhihu]
+pattern = com/zhihu/matisse
+description = Video selector for Android
+
 [zohoanalytics]
 description = Zoho Analytics (from ETIP Exodus Privacy list)
 pattern = com/zoho/zanalytics
 
 [zong]
 pattern = com/zong/android/engine
```

### Comparing `droidlysis-3.4.5/conf/manifest.conf` & `droidlysis-3.4.7/conf/manifest.conf`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.5/conf/sortconf.py` & `droidlysis-3.4.7/conf/sortconf.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.5/conf/wide.conf` & `droidlysis-3.4.7/conf/wide.conf`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.5/droidconfig.py` & `droidlysis-3.4.7/droidconfig.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,48 @@
 import os
+import errno
 import configparser
 import logging
 import shutil
+import filecmp 
 from platformdirs import *
 
 
 logging.basicConfig(format='%(levelname)s:%(filename)s:%(message)s',
                     level=logging.INFO)
 
 
 # ------------------------- Reading *.conf configuration files -----------
 class generalconfig:
-    def __init__(self, filename='./conf/general.conf', verbose=False):
+    def __init__(self, filename, verbose=False):
+        if not filename:
+            filename = './conf/general.conf'
+        if not os.path.exists(filename):
+            try:
+                from xdg.BaseDirectory import xdg_config_home
+
+                config = xdg_config_home
+            except ImportError:
+                config = os.path.join(os.getenv('HOME'), '.config')
+            if not os.path.exists(config):
+                config = '/etc'
+            config = os.path.join(config, 'droidlysis')
+            if os.path.exists(config):
+                filename = os.path.join(config, 'general.conf')
+        logging.debug(f'Reading config from {filename}')
+
+        if not os.path.exists(filename):
+            raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), filename)
         self.config = configparser.ConfigParser()
         self.config.read(filename)
 
         # get config
         self.APKTOOL_JAR = os.path.expanduser(self.config['tools']['apktool'])
         self.BAKSMALI_JAR = os.path.expanduser(self.config['tools']['baksmali'])
         self.DEX2JAR_CMD = os.path.expanduser(self.config['tools']['dex2jar'])
-        self.PROCYON_JAR = os.path.expanduser(self.config['tools']['procyon'])
         self.KEYTOOL = os.path.expanduser(self.config['tools']['keytool'])
         self.SMALI_CONFIGFILE = os.path.join(os.path.dirname(filename),
                                              self.config['general']['smali_config'])
         self.WIDE_CONFIGFILE = os.path.join(os.path.dirname(filename),
                                             self.config['general']['wide_config'])
         self.ARM_CONFIGFILE = os.path.join(os.path.dirname(filename),
                                            self.config['general']['arm_config'])
@@ -33,23 +52,25 @@
         # duplicate kit configuration for edition
         cache_dir = user_cache_dir('droidlysis', 'cryptax')
         if not os.path.exists(cache_dir):
             os.makedirs(cache_dir)
         self.KIT_CONFIGFILE = os.path.join(cache_dir,
                                            self.config['general']['kit_config'])
         if not os.path.exists(self.KIT_CONFIGFILE):
-            logging.verbose(f'Copying {self.DISTRIB_KIT_CONFIGFILE}'
-                            'to {self.KIT_CONFIGFILE}')
+            logging.debug(f'Copying {self.DISTRIB_KIT_CONFIGFILE}'
+                          f' to {self.KIT_CONFIGFILE}')
             shutil.copyfile(self.DISTRIB_KIT_CONFIGFILE, self.KIT_CONFIGFILE)
+        elif not filecmp.cmp(self.KIT_CONFIGFILE, self.DISTRIB_KIT_CONFIGFILE):
+            logging.warning(f'Cached kit configuration {self.KIT_CONFIGFILE} != general distrib config {self.DISTRIB_KIT_CONFIGFILE}. Using cached config. Check this is ok')
 
         self.SQLALCHEMY = f'sqlite:///{self.config["general"]["db_file"]}'
 
         # check files are accessible
         for f in [self.APKTOOL_JAR, self.BAKSMALI_JAR,
-                  self.DEX2JAR_CMD, self.PROCYON_JAR,
+                  self.DEX2JAR_CMD, 
                   self.SMALI_CONFIGFILE, self.WIDE_CONFIGFILE,
                   self.ARM_CONFIGFILE, self.KIT_CONFIGFILE]:
             if not os.access(f, os.R_OK):
                 logging.warning(f'Cannot access {f} - check your configuration file {filename}')
 
         if not os.access(self.KEYTOOL, os.X_OK):
             logging.warning(f'Cannot access keytool at {self.KEYTOOL} - check your configuration file {filename}')
```

### Comparing `droidlysis-3.4.5/droidcountry.py` & `droidlysis-3.4.7/droidcountry.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.5/droidlysis.egg-info/PKG-INFO` & `droidlysis-3.4.7/droidlysis.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,91 +1,84 @@
 Metadata-Version: 2.1
 Name: droidlysis
-Version: 3.4.5
+Version: 3.4.7
 Summary: DroidLysis: pre-analysis of suspicious Android samples
 Home-page: https://github.com/cryptax/droidlysis
 Author: @cryptax
 Author-email: aafortinet@gmail.com
 License: MIT
 Keywords: android malware reverse
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: Unix
 Classifier: Topic :: Software Development :: Disassemblers
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: configparser>=4.0.2
+Requires-Dist: python-magic==0.4.12
+Requires-Dist: requests
+Requires-Dist: SQLAlchemy>=1.1.1
+Requires-Dist: rarfile>=3.0
+Requires-Dist: platformdirs
 
 # DroidLysis
 
 DroidLysis is a **pre-analysis tool for Android apps**: it performs repetitive and boring tasks we'd typically do at the beginning of any reverse engineering. It disassembles the Android sample, organizes output in directories, and searches for suspicious spots in the code to look at.
 The output helps the reverse engineer speed up the first few steps of analysis.
 
 DroidLysis can be used over Android packages (apk), Dalvik executables (dex), Zip files (zip), Rar files (rar) or directories of files.
 
-<img src="https://img.shields.io/badge/PyPi%20-3.4.5-blue">
-
-## Quick setup
-
-Can't wait to use DroidLysis? Then, use a Docker container:
-
-```
-$ docker pull cryptax/droidlysis:2023.05
-$ docker run -it --rm -v /tmp/share:/share cryptax/droidlysis:2023.05  /bin/bash
-$ cd /opt/droidlysis
-$ python3 ./droidlysis3.py --help
-```
+<img src="https://img.shields.io/badge/PyPi%20-3.4.7-blue">
 
 ## Installing DroidLysis
 
 1. Install required system packages
 
 ```
 sudo apt-get install default-jre git python3 python3-pip unzip wget libmagic-dev libxml2-dev libxslt-dev
 ```
 
 
 2. Install Android disassembly tools
 
-[Apktool](https://ibotpeaches.github.io/Apktool/) , 
-[Baksmali](https://bitbucket.org/JesusFreke/smali/downloads), and optionally 
-[Dex2jar](https://github.com/pxb1988/dex2jar) and  
-[Procyon](https://bitbucket.org/mstrobel/procyon/wiki/Java%20Decompiler) (note that Procyon only works with Java 8, not Java 11).
+- [Apktool](https://ibotpeaches.github.io/Apktool/) , 
+- [Baksmali](https://bitbucket.org/JesusFreke/smali/downloads), and optionally 
+- [Dex2jar](https://github.com/pxb1988/dex2jar) and 
 
 ```
 $ mkdir -p ~/softs
 $ cd ~/softs
-$ wget https://bitbucket.org/iBotPeaches/apktool/downloads/apktool_2.7.0.jar
+$ wget https://bitbucket.org/iBotPeaches/apktool/downloads/apktool_2.9.3.jar
 $ wget https://bitbucket.org/JesusFreke/smali/downloads/baksmali-2.5.2.jar
-$ wget https://github.com/pxb1988/dex2jar/releases/download/v2.2-SNAPSHOT-2021-10-31/dex-tools-2.2-SNAPSHOT-2021-10-31.zip
-$ unzip dex-tools-2.2-SNAPSHOT-2021-10-31.zip 
-$ rm -f dex-tools-2.2-SNAPSHOT-2021-10-31.zip 
+$ wget https://github.com/pxb1988/dex2jar/releases/download/v2.4/dex-tools-v2.4.zip
+$ unzip dex-tools-v2.4.zip 
+$ rm -f dex-tools-v2.4.zip 
 ```
 
 3. Get DroidLysis from the Git repository (preferred) or from pip
 
-Install from Git in a Python virtual environment:
+Install from Git in a Python virtual environment (`python3 -m venv`, or pyenv virtual environments etc).
 
 ```
 $ python3 -m venv venv
 $ source ./venv/bin/activate
 (venv) $ pip3 install git+https://github.com/cryptax/droidlysis
 ```
 
 Alternatively, you can install DroidLysis directly from PyPi (`pip3 install droidlysis`).
 
 4. Configure `conf/general.conf`. In particular make sure to change `/home/axelle` with your appropriate directories.
 
 ```
 [tools]
-apktool = /home/axelle/softs/apktool_2.7.0.jar
+apktool = /home/axelle/softs/apktool_2.9.3.jar
 baksmali = /home/axelle/softs/baksmali-2.5.2.jar
-dex2jar = /home/axelle/softs/dex-tools-2.2-SNAPSHOT/d2j-dex2jar.sh
-procyon = /home/axelle/softs/procyon-decompiler-0.5.30.jar
+dex2jar = /home/axelle/softs/dex-tools-v2.4/d2j-dex2jar.sh
 keytool = /usr/bin/keytool
 ...
 ```
 
 5. Run it:
 
 ```
@@ -110,15 +103,15 @@
 ```
 droidlysis --help
 ```
 
 For example, test it on [Signal's APK](https://signal.org/android/apk/):
 
 ```
-droidlysis --input Signal-website-universal-release-4.52.4.apk --output /tmp
+droidlysis --input Signal-website-universal-release-6.26.3.apk --output /tmp --config /PATH/TO/DROIDLYSIS/conf/general.conf
 ```
 
 ![](./images/example.png)
 
 DroidLysis outputs:
 
 - A summary on the console (see image above)
@@ -129,16 +122,14 @@
 
 Get usage with `droidlysis --help`
 
 - The input can be a file or a directory of files to recursively look into. DroidLysis knows how to process Android packages, DEX, ODEX and ARM executables, ZIP, RAR. DroidLysis won't fail on other type of files (unless there is a bug...) but won't be able to understand the content.
 
 - When processing directories of files, it is typically quite helpful to move processed samples to another location to know what has been processed. This is handled by option `--movein`.  Also, if you are only interested in statistics, you should probably clear the output directory which contains detailed information for each sample: this is option `--clearoutput`. If you want to store all statistics in a SQL database, use `--enable-sql` (see [here](#sqlite_database))
 
-- DEX decompilation is quite long with Procyon, so this option is *disabled* by default. If you want to decompile to Java, use `--enable-procyon`.
-
 - DroidLysis's analysis does not inspect known 3rd party SDK by default, i.e. for instance it won't report any suspicious activity from these. If you want them to be inspected, use option `--no-kit-exception`. This usually creates many more detected properties for the sample, as SDKs (e.g. advertisment) use lots of flagged APIs (get GPS location, get IMEI, get IMSI, HTTP POST...).
 
 ## Sample output directory (`--output DIR`)
 
 This directory contains (when applicable):
 
 - A readable `AndroidManifest.xml`
@@ -152,14 +143,32 @@
 The following files are generated by DroidLysis:
 
 - `autoanalysis.md`: lists each pattern DroidLysis detected and where.
 - `report.md`: same as what was printed on the console
 
 If you do not need the sample output directory to be generated, use the option `--clearoutput`.
 
+## Import trackers from Exodus etc (`--import-exodus`)
+
+```
+$ python3 ./droidlysis3.py --import-exodus --verbose
+Processing file: ./droidurl.pyc ...
+DEBUG:droidconfig.py:Reading configuration file: './conf/./smali.conf'
+DEBUG:droidconfig.py:Reading configuration file: './conf/./wide.conf'
+DEBUG:droidconfig.py:Reading configuration file: './conf/./arm.conf'
+DEBUG:droidconfig.py:Reading configuration file: '/home/axelle/.cache/droidlysis/./kit.conf'
+DEBUG:droidproperties.py:Importing ETIP Exodus trackers from https://etip.exodus-privacy.eu.org/api/trackers/?format=json
+DEBUG:connectionpool.py:Starting new HTTPS connection (1): etip.exodus-privacy.eu.org:443
+DEBUG:connectionpool.py:https://etip.exodus-privacy.eu.org:443 "GET /api/trackers/?format=json HTTP/1.1" 200 None
+DEBUG:droidproperties.py:Appending imported trackers to /home/axelle/.cache/droidlysis/./kit.conf
+```
+
+Trackers from Exodus which are not present in your initial `kit.conf` are appended to `~/.cache/droidlysis/kit.conf`. Diff the 2 files and check what trackers you wish to add.
+
+
 ## SQLite database{#sqlite_database}
 
 If you want to process a directory of samples, you'll probably like to store the properties DroidLysis found in a database, to easily parse and query the findings. In that case, use the option `--enable-sql`. This will automatically dump all results in a database named `droidlysis.db`, in a table named `samples`. Each entry in the table is relative to a given sample. Each column is properties DroidLysis tracks.
 
 For example, to retrieve all filename, SHA256 sum and smali properties of the database:
 
 ```
@@ -201,17 +210,24 @@
 config.read(os.path.expanduser('~/.cache/droidlysis/kit.conf'))
 # Order all sections alphabetically
 config._sections = collections.OrderedDict(sorted(config._sections.items(), key=lambda t: t[0] ))
 with open('sorted.conf','w') as f:
     config.write(f)
 ```    
 
+## JEB script for smali properties
+
+This script helps you search for methods on JEB UI that contain code that matches the smali pattern and easily navigates to those functions. When you load the script and select `details.md` file among the droidlysis analysis files, a search box will appear. Once moved, you can easily bring up the search windows again by using recent script execution shortcut.
+
+- JEB > File > Scripts > Script selector > `script/DroidlysisSearch.py`
+- JEB > File > Scripts > Run last Script
 
 ## Updates
 
+- v3.4.6 - Detecting manifest feature that automatically loads APK at install
 - v3.4.5 - Creating a writable user kit.conf file
 - v3.4.4 - Bug fix #14
 - v3.4.3 - Using configuration files
 - v3.4.2 - Adding import of Exodus Privacy Trackers
 - v3.4.1 - Removed dependency to Androguard
 - v3.4.0 - Multidex support
 - v3.3.1 - Improving detection of Base64 strings
```

### Comparing `droidlysis-3.4.5/droidlysis.egg-info/SOURCES.txt` & `droidlysis-3.4.7/droidlysis.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -22,8 +22,10 @@
 conf/smali.conf
 conf/sortconf.py
 conf/wide.conf
 droidlysis.egg-info/PKG-INFO
 droidlysis.egg-info/SOURCES.txt
 droidlysis.egg-info/dependency_links.txt
 droidlysis.egg-info/requires.txt
-droidlysis.egg-info/top_level.txt
+droidlysis.egg-info/top_level.txt
+test/test_droidconfig.py
+test/test_droidlysis3.py
```

### Comparing `droidlysis-3.4.5/droidlysis3.py` & `droidlysis-3.4.7/droidlysis3.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import logging
 from droidsql import DroidSql
 from droidconfig import generalconfig
 
 property_dump_file = 'details.md'
 report_file = 'report.md'
 json_file = 'report.json'
-__version__ = "3.4.5"
+__version__ = "3.4.7"
 
 logging.basicConfig(format='%(levelname)s:%(filename)s:%(message)s',
                     level=logging.INFO)
 
 
 def get_arguments():
     """Read arguments for the program and returns the ArgumentParser"""
@@ -61,33 +61,31 @@
                         action='version',
                         version="%(prog)s "+__version__)
     parser.add_argument('--no-kit-exception',
                         help='by default, ad/dev/stats kits are ruled '
                         'out for searches. '
                         'Use this option to treat them as regular namespaces',
                         action='store_true')
-    parser.add_argument('--enable-procyon',
-                        help='enable procyon decompilation',
-                        action='store_true')
     parser.add_argument('--disable-report',
                         help='do not generate automatic report',
                         action='store_true')
     parser.add_argument('--enable-sql',
                         help='write analysis to SQL database',
                         action='store_true')
     parser.add_argument('--disable-json',
                         help='do not dump analysis to JSON',
                         action='store_true')
     parser.add_argument('--import-exodus',
                         help='import ETIP Exodus Privacy trackers '
                         'and add them to kit config file',
                         action='store_true')
     parser.add_argument('--config',
-                        help='general configuration file for DroidLysis',
-                        action='store', default='./conf/general.conf')
+                        help='general configuration file for DroidLysis. Default: ./conf/general.conf',
+                        default='./conf/general.conf',
+                        action='store')
 
     args = parser.parse_args()
     if args.verbose:
         logging.getLogger().setLevel(logging.DEBUG)
     # create output dir if necessary
     droidutil.mkdir_if_necessary(args.output)
     # create movein dir if necessary
@@ -113,15 +111,14 @@
             listing = os.listdir(element)
             for file in listing:
                 process_file(config,
                              os.path.join(element, file),
                              outdir=args.output,
                              verbose=args.verbose,
                              clear=args.clearoutput,
-                             enable_procyon=args.enable_procyon,
                              disable_report=args.disable_report,
                              no_kit_exception=args.no_kit_exception,
                              sql=sql,
                              disable_json=args.disable_json,
                              import_exodus=args.import_exodus)
                 if args.movein:
                     logging.debug("Moving %s to %s" %
@@ -136,15 +133,14 @@
 
         if os.path.isfile(element):
             process_file(config,
                          os.path.join('.', element),
                          outdir=args.output,
                          verbose=args.verbose,
                          clear=args.clearoutput,
-                         enable_procyon=args.enable_procyon,
                          disable_report=args.disable_report,
                          silent=args.silent,
                          no_kit_exception=args.no_kit_exception,
                          sql=sql,
                          disable_json=args.disable_json,
                          import_exodus=args.import_exodus
                          )
@@ -156,15 +152,14 @@
 
 
 def process_file(config,
                  infile,
                  outdir='/tmp/analysis',
                  verbose=False,
                  clear=False,
-                 enable_procyon=False,
                  disable_report=False,
                  silent=False,
                  no_kit_exception=False,
                  sql=None,
                  disable_json=False,
                  import_exodus=False):
     """Static analysis of a given file"""
@@ -173,15 +168,14 @@
         if not silent:
             print("Processing file: " + infile + " ...")
         sample = droidsample.droidsample(config=config,
                                          filename=infile,
                                          output=outdir,
                                          verbose=verbose,
                                          clear=clear,
-                                         enable_procyon=enable_procyon,
                                          disable_description=disable_report,
                                          silent=silent,
                                          no_kit_exception=no_kit_exception,
                                          import_exodus=import_exodus)
         sample.unzip()
         sample.disassemble()
         sample.extract_file_properties()
```

### Comparing `droidlysis-3.4.5/droidproperties.py` & `droidlysis-3.4.7/droidproperties.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,15 @@
                     'bad_adler32': False,
                     'big_header': False,
                     'thuxnder': False
                     }
 
         # automatically set to False kit properties
         self.kits.clear()
+        logging.debug(f'Reading Kit Config file = {self.config.KIT_CONFIGFILE}')
         self.kitsconfig = droidconfig.droidconfig(self.config.KIT_CONFIGFILE,
                                                   self.verbose)
         for section in self.kitsconfig.get_sections():
             self.kits[section] = False
 
         if self.import_exodus:
             self.import_exodus_trackers()
```

### Comparing `droidlysis-3.4.5/droidreport.py` & `droidlysis-3.4.7/droidreport.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.5/droidsample.py` & `droidlysis-3.4.7/droidsample.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,28 +34,26 @@
 
     def __init__(self,
                  config,
                  filename,
                  output='/tmp/analysis',
                  verbose=False,
                  clear=False,
-                 enable_procyon=False,
                  disable_description=False,
                  silent=False,
                  no_kit_exception=False,
                  import_exodus=False):
         # Setup analysis of a given sample.
         # This does not perform the analysis in itself
 
         assert filename is not None, "Filename is invalid"
 
         self.config = config
         self.absolute_filename = filename
         self.clear = clear
-        self.enable_procyon = enable_procyon
         # we need those for recursive calls to process_file
         self.disable_description = disable_description
         self.silent = silent
         self.no_kit_exception = no_kit_exception
         self.ziprar = None  # zip file or rar file file handle
         self.verbose = verbose
         if verbose:
@@ -166,15 +164,14 @@
                         logging.debug("Recursively processing "
                                       + os.path.join(self.outdir, element))
                         # TODO: this is probably buggy: we
                         # should be providing enable_sql too etc.
                         droidlysis3.process_file(
                             os.path.join(self.outdir, element),
                             self.outdir, self.verbose, self.clear,
-                            self.enable_procyon,
                             self.disable_description,
                             self.no_kit_exception)
                     except:
                         logging.warning("Cannot extract %s : %s"
                                         % (element, sys.exc_info()[0]))
 
         if self.properties.filetype == droidutil.APK:
@@ -210,31 +207,29 @@
 
         DEX:
                 java -jar baksmali.jar -o outdir/smali classes.dex
                 if clear unset,
                       make sure classes.dex is readable
                       dex2jar classes.dex -o classes-dex2jar.jar
                       unzip -qq classes-dex2jar.jar -d outdir/unjarred
-                      procyon classes-dex2jar.jar -o outdir/procyon
 
         What we'll find:
-        APK, clear unset: ./smali AndroidManifest.xml ./unzipped classes.dex classes-dex2jar.jar ./unjarred ./procyon
+        APK, clear unset: ./smali AndroidManifest.xml ./unzipped classes.dex classes-dex2jar.jar ./unjarred 
         APK, clear set  : ./smali AndroidManifest.xml classes.dex
 
         DEX, clear unset: classes.dex ./smali
-        DEX, clear set  : classes.dex ./smali classes-dex2jar.jar ./unjarred ./procyon
+        DEX, clear set  : classes.dex ./smali classes-dex2jar.jar ./unjarred
 
         """
         logging.debug("------------- Disassembling")
 
         if self.properties.filetype == droidutil.ARM or \
                 self.properties.filetype == droidutil.RAR or \
                 self.properties.filetype == droidutil.CLASS or \
                 self.properties.filetype == droidutil.UNKNOWN:
-            # TODO: we could be running procyon on a class file.
             logging.debug("Nothing to disassemble for "
                           + self.absolute_filename)
             return
 
         if self.properties.filetype == droidutil.APK:
             # APKTOOL won't output to an existing
             # dir unless you use the -f switch. But then, -f erases the contents
@@ -264,27 +259,27 @@
             # we want all smali_classes? dir in smali
             if os.path.exists(os.path.join(self.outdir, "smali_classes2")):
                 # we have multidex - we are going to move
                 # all smali classes in the same directory
                 logging.debug("Moving multidex smali classes to ./smali")
 
                 os.system("cp -R "
-                          + os.path.join(self.outdir, "./smali_classes?/*")
+                          + os.path.join(self.outdir, "./smali_classes*/*")
                           + " " + os.path.join(self.outdir, "./smali"))
                 os.system("rm -r "
-                          + os.path.join(self.outdir, "./smali_classes?"))
+                          + os.path.join(self.outdir, "./smali_classes*"))
                 
             if self.verbose:
                 logging.debug("Apktool finished")
 
             # extract classes.dex whatever happens, we'll use it
             logging.debug("Extracting classes*.dex")
             try:
                 self.ziprar.extract_one_file('classes.dex', self.outdir)
-                for i in range(2, 10):
+                for i in range(2, 1000):
                     self.ziprar.extract_one_file('classes{}.dex'.format(i), self.outdir)
                     if not os.path.exists(os.path.join(self.outdir, 'classes{}.dex'.format(i))):
                         break
                     self.properties.smali['multidex'].append('classes{}.dex'.format(i))
                     
             except:
                 logging.debug("Extracting classes.dex failed: %s" % (sys.exc_info()[0]))
@@ -332,20 +327,14 @@
                                                 stdout=self.process_output, stderr=self.process_output)
                             except:
                                 logging.warning("[-] Dex2jar failed on {}".format(d))
                     else:
                         logging.warning("Dex2jar software is not executable, skipping (file: {0})".format(self.config.DEX2JAR_CMD))
                     
                     if os.access(jar_file, os.R_OK):
-                        if self.enable_procyon and os.access(self.config.PROCYON_JAR, os.R_OK):
-                            logging.debug("Procyon decompiler on " + jar_file)
-                            subprocess.call(["java", "-jar", self.config.PROCYON_JAR,
-                                            jar_file, "-o", os.path.join(self.outdir, 'procyon')],
-                                            stdout=self.process_output, stderr=self.process_output)
-
                         logging.debug("Unjarring " + jar_file)
                         jarziprar = droidziprar.droidziprar(jar_file, zipmode=True, verbose=self.verbose)
                         if jarziprar.handle is None:
                             logging.debug("Bad Jar / Failed to unjar " + jar_file)
                         else:
                             try:
                                 jarziprar.extract_all(os.path.join(self.outdir, 'unjarred'))
@@ -510,15 +499,15 @@
             filename = os.path.join(smali_dir, self.properties.manifest['main_activity'].replace('.', os.path.sep)
                                     .replace('\'', '') + '.smali')
             if not os.access(filename, os.R_OK):
                 logging.debug("Unable to find Main Activitity: {} filename={}".format(self.properties.manifest['main_activity'],
                                                                                       filename))
                 missing = True
 
-        if missing and (self.properties.smali['dex_class_loader'] or self.properties.smali['dex_file']):
+        if missing and (self.properties.smali['dex_class_loader'] or self.properties.smali['dex_file'] or self.properties.smali['load_library'] or self.properties.smali['class_loader']):
             self.properties.smali['packed'] = True
 
     def extract_manifest_properties(self):
         """Extracting services, receivers, activities etc from manifest"""
         manifest = os.path.join(self.outdir, 'AndroidManifest.xml')
         if self.properties.filetype == droidutil.APK and os.access(manifest, os.R_OK) and os.path.getsize(manifest)>0:
             try:
@@ -575,15 +564,23 @@
                 if 'multidex' in t:
                     self.properties.manifest['multidex'] = True
                     break
 
             self.properties.manifest['maxSDK'] = droidutil.get_element(xmldoc, 'uses-sdk', 'android:maxSdkVersion')
             self.properties.manifest['minSDK'] = droidutil.get_element(xmldoc, 'uses-sdk', 'android:minSdkVersion')
             self.properties.manifest['targetSDK'] = droidutil.get_element(xmldoc, 'uses-sdk', 'android:targetSdkVersion')
-            droidutil.get_elements(xmldoc, 'meta-data', 'android:value')
+            tab = droidutil.get_elements(xmldoc, 'meta-data', 'android:name')
+            if self.verbose:
+                logging.debug('meta-data: ' + ''.join(tab))
+            for t in tab:
+                if 'android.content.ContactDirectory' in t:
+                    self.properties.manifest['auto_load'] = True
+                    if self.verbose:
+                        logging.debug('Suspicious ContactDirectory meta-data trick')
+                    break
 
             if self.verbose:
                 logging.debug("MinSDK=%s MaxSDK=%s TargetSDK=%s" % (self.properties.manifest['minSDK'],
                                                                     self.properties.manifest['maxSDK'],
                                                                     self.properties.manifest['targetSDK']))
                 for perm in self.properties.manifest['permissions']:
                     logging.debug("Requires permission " + perm)
@@ -763,26 +760,41 @@
 
                 analysis_file = open(os.path.join(self.outdir, droidlysis3.property_dump_file), 'a')
                 # let's not dump for nops
                 if not (mykey == ' nop'):
                     if match[mykey]:
                         analysis_file.write("## %s\n" % mykey)
                     for element in match[mykey]:
-                        analysis_file.write("- "+str(element)+"\n")
+                        append = self.extract_method_name(str(element))
+                        analysis_file.write("- "+append+str(element)+"\n")
                     analysis_file.write('\n')
                     analysis_file.close()
 
             # test if sample is likely to be packed
             self.is_packed()
         else:
             logging.debug("Cannot extract smali properties, because directory %s not found" % smali_dir)
             # all smali properties should then be set to unknown
             for key in sorted(self.properties.smali.keys()):
                 self.properties.smali[key] = 'unknown'
-                                 
+
+    def extract_method_name(self, element):
+        m = re.findall(r'file=(.*?)\s+no=\s*(\d+)', element)
+        if m:
+            file_path, line_no = m[0]
+            with open(file_path, 'r') as f:
+                lines = f.readlines()
+                for i in range(int(line_no), 0, -1):
+                    line = lines[i]
+                    if line.startswith('.method'):
+                        clazz = (lines[0].split(' ')[-1]).strip()
+                        method = (line.split(' ')[-1]).strip()
+                        return f'path={clazz}->{method} '
+        return ''
+
     def extract_wide_properties(self, list_of_kits):
         """Will look for given properties (e.g GPS usage, presence of executables
         in all subdirectories (smali, assets, resources, library...)"""
 
         logging.debug("------------- Extracting Wide properties")
 
         # detecting presence of ijiami packer
@@ -790,14 +802,28 @@
         if os.access(ijiami, os.R_OK):
             self.properties.wide['ijiami'] = True
 
         # detecting Flutter debug mode
         flutter_debug = os.path.join(self.outdir, 'unzipped/assets/flutter_assets/kernel_blob.bin')
         if os.access(flutter_debug, os.R_OK):
             self.properties.kits['flutter'] = True
+        
+        # detecting react native framework using index.android.bundle
+        react_assets = os.path.join(self.outdir, 'unzipped/assets/index.android.bundle')
+        if os.access(react_assets, os.R_OK):
+            self.properties.wide['react_asset'] = True
+        
+        # Run "file" to detect hermes bytecode version
+        proc = subprocess.Popen(['file', react_assets], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        output = proc.communicate()[0]
+
+        analysis_file = open(os.path.join(self.outdir, droidlysis3.property_dump_file), 'a')
+        analysis_file.write('# Hermes Bytecode version\n')
+        analysis_file.write(output.decode() + '\n')
+        analysis_file.close()
 
         # detect executables in resources
         self.find_exec_in_resources()
 
         # other properties
         if self.properties.filetype == droidutil.APK or self.properties.filetype == droidutil.DEX:
             exceptions = []
@@ -963,15 +989,15 @@
                     if found_arm:
                         for arm in found_arm:
                             logging.debug("Recursively processing " + arm)
                             self.extract_arm_properties(arm)
                     if found_apk:
                         for apk in found_apk:
                             logging.debug("Recursively processing " + apk)
-                            droidlysis3.process_file(apk, self.outdir, self.verbose, self.clear, self.enable_procyon, 
+                            droidlysis3.process_file(apk, self.outdir, self.verbose, self.clear, 
                                                      disable_report=self.disable_description,
                                                      no_kit_exception=self.no_kit_exception)
 
     def interesting_url(self, url):
         """Rules out meaningless URLs to keep only those which might be useful for attackers.
         
         input: url - typically starting with http://
```

### Comparing `droidlysis-3.4.5/droidsql.py` & `droidlysis-3.4.7/droidsql.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.5/droidurl.py` & `droidlysis-3.4.7/droidurl.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.5/droidutil.py` & `droidlysis-3.4.7/droidutil.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.5/droidziprar.py` & `droidlysis-3.4.7/droidziprar.py`

 * *Files identical despite different names*

### Comparing `droidlysis-3.4.5/setup.py` & `droidlysis-3.4.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     long_description_content_type="text/markdown",
     author='@cryptax',
     author_email='aafortinet@gmail.com',
     url='https://github.com/cryptax/droidlysis',
     license='MIT',
     keywords="android malware reverse",
     python_requires='>=3.0',
-    version='3.4.5',
+    version='3.4.7',
     packages=['conf'],
     py_modules=[
         'droidconfig',
         'droidcountry',
         'droidlysis3',
         'droidproperties',
         'droidreport',
```

