# Comparing `tmp/hepdata_lib-0.8.1.tar.gz` & `tmp/hepdata_lib-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hepdata_lib-0.8.1.tar", last modified: Wed Sep  1 09:59:41 2021, max compression
+gzip compressed data, was "hepdata_lib-0.9.0.tar", last modified: Fri Oct 29 08:39:25 2021, max compression
```

## Comparing `hepdata_lib-0.8.1.tar` & `hepdata_lib-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 clange     (501) staff       (20)        0 2021-09-01 09:59:41.269075 hepdata_lib-0.8.1/
--rw-r--r--   0 clange     (501) staff       (20)     1070 2021-06-14 14:36:49.000000 hepdata_lib-0.8.1/LICENSE
--rw-r--r--   0 clange     (501) staff       (20)       79 2021-06-14 14:36:49.000000 hepdata_lib-0.8.1/MANIFEST.in
--rw-r--r--   0 clange     (501) staff       (20)     5672 2021-09-01 09:59:41.269274 hepdata_lib-0.8.1/PKG-INFO
--rw-r--r--   0 clange     (501) staff       (20)     4248 2021-06-14 14:36:49.000000 hepdata_lib-0.8.1/README.md
-drwxr-xr-x   0 clange     (501) staff       (20)        0 2021-09-01 09:59:41.265598 hepdata_lib-0.8.1/hepdata_lib/
--rw-r--r--   0 clange     (501) staff       (20)    23360 2021-09-01 09:59:09.000000 hepdata_lib-0.8.1/hepdata_lib/__init__.py
--rw-r--r--   0 clange     (501) staff       (20)    14586 2021-06-14 14:36:49.000000 hepdata_lib-0.8.1/hepdata_lib/c_file_reader.py
--rw-r--r--   0 clange     (501) staff       (20)    10306 2021-08-31 07:44:26.000000 hepdata_lib-0.8.1/hepdata_lib/helpers.py
--rw-r--r--   0 clange     (501) staff       (20)    16423 2021-06-14 14:36:49.000000 hepdata_lib-0.8.1/hepdata_lib/root_utils.py
-drwxr-xr-x   0 clange     (501) staff       (20)        0 2021-09-01 09:59:41.268718 hepdata_lib-0.8.1/hepdata_lib.egg-info/
--rw-r--r--   0 clange     (501) staff       (20)     5672 2021-09-01 09:59:41.000000 hepdata_lib-0.8.1/hepdata_lib.egg-info/PKG-INFO
--rw-r--r--   0 clange     (501) staff       (20)      358 2021-09-01 09:59:41.000000 hepdata_lib-0.8.1/hepdata_lib.egg-info/SOURCES.txt
--rw-r--r--   0 clange     (501) staff       (20)        1 2021-09-01 09:59:41.000000 hepdata_lib-0.8.1/hepdata_lib.egg-info/dependency_links.txt
--rw-r--r--   0 clange     (501) staff       (20)        1 2021-06-14 14:41:57.000000 hepdata_lib-0.8.1/hepdata_lib.egg-info/not-zip-safe
--rw-r--r--   0 clange     (501) staff       (20)       42 2021-09-01 09:59:41.000000 hepdata_lib-0.8.1/hepdata_lib.egg-info/requires.txt
--rw-r--r--   0 clange     (501) staff       (20)       12 2021-09-01 09:59:41.000000 hepdata_lib-0.8.1/hepdata_lib.egg-info/top_level.txt
--rw-r--r--   0 clange     (501) staff       (20)      135 2021-09-01 09:59:41.269804 hepdata_lib-0.8.1/setup.cfg
--rw-r--r--   0 clange     (501) staff       (20)     1646 2021-09-01 09:59:09.000000 hepdata_lib-0.8.1/setup.py
+drwxr-xr-x   0 clange     (501) staff       (20)        0 2021-10-29 08:39:25.063357 hepdata_lib-0.9.0/
+-rw-r--r--   0 clange     (501) staff       (20)     1070 2021-06-14 14:36:49.000000 hepdata_lib-0.9.0/LICENSE
+-rw-r--r--   0 clange     (501) staff       (20)       79 2021-06-14 14:36:49.000000 hepdata_lib-0.9.0/MANIFEST.in
+-rw-r--r--   0 clange     (501) staff       (20)     5147 2021-10-29 08:39:25.063495 hepdata_lib-0.9.0/PKG-INFO
+-rw-r--r--   0 clange     (501) staff       (20)     4248 2021-06-14 14:36:49.000000 hepdata_lib-0.9.0/README.md
+drwxr-xr-x   0 clange     (501) staff       (20)        0 2021-10-29 08:39:25.059416 hepdata_lib-0.9.0/hepdata_lib/
+-rw-r--r--   0 clange     (501) staff       (20)    23360 2021-10-29 08:37:39.000000 hepdata_lib-0.9.0/hepdata_lib/__init__.py
+-rw-r--r--   0 clange     (501) staff       (20)    14586 2021-06-14 14:36:49.000000 hepdata_lib-0.9.0/hepdata_lib/c_file_reader.py
+-rw-r--r--   0 clange     (501) staff       (20)    10306 2021-10-28 17:44:20.000000 hepdata_lib-0.9.0/hepdata_lib/helpers.py
+-rw-r--r--   0 clange     (501) staff       (20)    17242 2021-10-28 18:04:44.000000 hepdata_lib-0.9.0/hepdata_lib/root_utils.py
+drwxr-xr-x   0 clange     (501) staff       (20)        0 2021-10-29 08:39:25.063083 hepdata_lib-0.9.0/hepdata_lib.egg-info/
+-rw-r--r--   0 clange     (501) staff       (20)     5147 2021-10-29 08:39:25.000000 hepdata_lib-0.9.0/hepdata_lib.egg-info/PKG-INFO
+-rw-r--r--   0 clange     (501) staff       (20)      358 2021-10-29 08:39:25.000000 hepdata_lib-0.9.0/hepdata_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 clange     (501) staff       (20)        1 2021-10-29 08:39:25.000000 hepdata_lib-0.9.0/hepdata_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 clange     (501) staff       (20)        1 2021-06-14 14:41:57.000000 hepdata_lib-0.9.0/hepdata_lib.egg-info/not-zip-safe
+-rw-r--r--   0 clange     (501) staff       (20)       28 2021-10-29 08:39:25.000000 hepdata_lib-0.9.0/hepdata_lib.egg-info/requires.txt
+-rw-r--r--   0 clange     (501) staff       (20)       12 2021-10-29 08:39:25.000000 hepdata_lib-0.9.0/hepdata_lib.egg-info/top_level.txt
+-rw-r--r--   0 clange     (501) staff       (20)      135 2021-10-29 08:39:25.064152 hepdata_lib-0.9.0/setup.cfg
+-rw-r--r--   0 clange     (501) staff       (20)     1762 2021-10-29 08:37:39.000000 hepdata_lib-0.9.0/setup.py
```

### Comparing `hepdata_lib-0.8.1/LICENSE` & `hepdata_lib-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hepdata_lib-0.8.1/PKG-INFO` & `hepdata_lib-0.9.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,89 +1,92 @@
 Metadata-Version: 2.1
 Name: hepdata_lib
-Version: 0.8.1
+Version: 0.9.0
 Summary: Library for getting your data into HEPData
 Home-page: https://github.com/HEPData/hepdata_lib
 Author: Andreas Albert, Clemens Lange
 Author-email: hepdata-lib@cern.ch
 License: UNKNOWN
 Project-URL: Documentation, https://hepdata-lib.readthedocs.io
 Project-URL: Bug Reports, https://github.com/HEPData/hepdata_lib/issues
 Project-URL: Source, https://github.com/HEPData/hepdata_lib
-Description: # hepdata_lib
-        
-        [![DOI](https://zenodo.org/badge/129248575.svg)](https://zenodo.org/badge/latestdoi/129248575)
-        [![PyPI version](https://badge.fury.io/py/hepdata-lib.svg)](https://badge.fury.io/py/hepdata-lib)
-        [![Actions Status](https://github.com/HEPData/hepdata_lib/workflows/tests/badge.svg)](https://github.com/HEPData/hepdata_lib/actions)
-        [![Coverage Status](https://coveralls.io/repos/github/HEPData/hepdata_lib/badge.svg?branch=master)](https://coveralls.io/github/HEPData/hepdata_lib?branch=master)
-        [![Documentation Status](https://readthedocs.org/projects/hepdata-lib/badge/)](http://hepdata-lib.readthedocs.io/)
-        [![Docker Hub](https://images.microbadger.com/badges/image/clelange/hepdata_lib.svg)](https://hub.docker.com/r/clelange/hepdata_lib/)
-        
-        Library for getting your data into HEPData
-        
-        ## Installation
-        
-        It is highly recommended you install `hepdata_lib` into a [virtual environment](https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/).
-        
-        ```shell
-        pip install hepdata_lib
-        ```
-        
-        If you are not sure about your Python environment, please also see below how to use `hepdata_lib` in a Docker or Singularity container.
-        
-        ## Getting started
-        
-        For using `hepdata_lib`, you don't even need to install it, but can use the [binder](https://mybinder.org/) or [SWAN](https://swan.cern.ch/) (CERN-only) services using one of the buttons below and following the instructions in the notebook with name [Getting_started](examples/Getting_started.ipynb):
-        
-        [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/HEPData/hepdata_lib/master?filepath=examples/Getting_started.ipynb)
-        [![SWAN](https://swanserver.web.cern.ch/swanserver/images/badge_swan_white_150.png)](https://cern.ch/swanserver/cgi-bin/go/?projurl=https://github.com/HEPData/hepdata_lib.git)
-        
-        You can also use the Docker image:
-        
-        ```shell
-        docker run --rm -it -p 8888:8888 -v ${PWD}:/home/hepdata clelange/hepdata_lib
-        ```
-        
-        And then point your browser to [http://localhost:8888](http://localhost:8888) and use the token that is printed out. The output will end up in your current working directory (`${PWD}`).
-        
-        If you prefer a shell, instead run:
-        
-        ```shell
-        docker run --rm -it -p 8888:8888 -v ${PWD}:/home/hepdata clelange/hepdata_lib bash
-        ```
-        
-        If on CERN LXPLUS or anywhere else where there is Singularity available but not Docker, you can still use the docker image:
-        
-        ```shell
-        export SINGULARITY_CACHEDIR="/tmp/$(whoami)/singularity"
-        singularity shell -B /afs -B /eos docker://clelange/hepdata_lib bash
-        ```
-        
-        Unpacking the image can take a few minutes the first time you use it. Please be patient. Both EOS and AFS should be available and the output will be in your current working directory.
-        
-        ## Further examples
-        
-        There are a few more examples available that can directly be run using the [binder](https://mybinder.org/) links below or using [SWAN](https://swan.cern.ch/) (CERN-only, please use LCG release LCG_94 or later) and selecting the corresponding notebook manually:
-        
-        - [Reading in text files](examples/Getting_started.ipynb) [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/HEPData/hepdata_lib/master?filepath=examples/Getting_started.ipynb)
-        - [Reading in a CMS combine ntuple](examples/combine_limits.ipynb) [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/HEPData/hepdata_lib/master?filepath=examples/combine_limits.ipynb)
-        - [Reading in ROOT histograms](examples/reading_histograms.ipynb) [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/HEPData/hepdata_lib/master?filepath=examples/reading_histograms.ipynb)
-        - [Reading a correlation matrix](examples/correlation.ipynb) [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/HEPData/hepdata_lib/master?filepath=examples/correlation.ipynb)
-        - [Reading TGraph and TGraphError from '.C' files](examples/read_c_file.ipynb) [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/HEPData/hepdata_lib/master?filepath=examples/read_c_file.ipynb)
-        
-        ## External dependencies
-        
-        - [ROOT](https://root.cern.ch)
-        - [ImageMagick](https://www.imagemagick.org)
-        
-        Make sure that you have `ROOT` in your `$PYTHONPATH` and that the `convert` command is available by adding its location to your `$PATH` if needed.
-        
 Keywords: HEPData physics OpenData
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# hepdata_lib
+
+[![DOI](https://zenodo.org/badge/129248575.svg)](https://zenodo.org/badge/latestdoi/129248575)
+[![PyPI version](https://badge.fury.io/py/hepdata-lib.svg)](https://badge.fury.io/py/hepdata-lib)
+[![Actions Status](https://github.com/HEPData/hepdata_lib/workflows/tests/badge.svg)](https://github.com/HEPData/hepdata_lib/actions)
+[![Coverage Status](https://coveralls.io/repos/github/HEPData/hepdata_lib/badge.svg?branch=master)](https://coveralls.io/github/HEPData/hepdata_lib?branch=master)
+[![Documentation Status](https://readthedocs.org/projects/hepdata-lib/badge/)](http://hepdata-lib.readthedocs.io/)
+[![Docker Hub](https://images.microbadger.com/badges/image/clelange/hepdata_lib.svg)](https://hub.docker.com/r/clelange/hepdata_lib/)
+
+Library for getting your data into HEPData
+
+## Installation
+
+It is highly recommended you install `hepdata_lib` into a [virtual environment](https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/).
+
+```shell
+pip install hepdata_lib
+```
+
+If you are not sure about your Python environment, please also see below how to use `hepdata_lib` in a Docker or Singularity container.
+
+## Getting started
+
+For using `hepdata_lib`, you don't even need to install it, but can use the [binder](https://mybinder.org/) or [SWAN](https://swan.cern.ch/) (CERN-only) services using one of the buttons below and following the instructions in the notebook with name [Getting_started](examples/Getting_started.ipynb):
+
+[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/HEPData/hepdata_lib/master?filepath=examples/Getting_started.ipynb)
+[![SWAN](https://swanserver.web.cern.ch/swanserver/images/badge_swan_white_150.png)](https://cern.ch/swanserver/cgi-bin/go/?projurl=https://github.com/HEPData/hepdata_lib.git)
+
+You can also use the Docker image:
+
+```shell
+docker run --rm -it -p 8888:8888 -v ${PWD}:/home/hepdata clelange/hepdata_lib
+```
+
+And then point your browser to [http://localhost:8888](http://localhost:8888) and use the token that is printed out. The output will end up in your current working directory (`${PWD}`).
+
+If you prefer a shell, instead run:
+
+```shell
+docker run --rm -it -p 8888:8888 -v ${PWD}:/home/hepdata clelange/hepdata_lib bash
+```
+
+If on CERN LXPLUS or anywhere else where there is Singularity available but not Docker, you can still use the docker image:
+
+```shell
+export SINGULARITY_CACHEDIR="/tmp/$(whoami)/singularity"
+singularity shell -B /afs -B /eos docker://clelange/hepdata_lib bash
+```
+
+Unpacking the image can take a few minutes the first time you use it. Please be patient. Both EOS and AFS should be available and the output will be in your current working directory.
+
+## Further examples
+
+There are a few more examples available that can directly be run using the [binder](https://mybinder.org/) links below or using [SWAN](https://swan.cern.ch/) (CERN-only, please use LCG release LCG_94 or later) and selecting the corresponding notebook manually:
+
+- [Reading in text files](examples/Getting_started.ipynb) [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/HEPData/hepdata_lib/master?filepath=examples/Getting_started.ipynb)
+- [Reading in a CMS combine ntuple](examples/combine_limits.ipynb) [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/HEPData/hepdata_lib/master?filepath=examples/combine_limits.ipynb)
+- [Reading in ROOT histograms](examples/reading_histograms.ipynb) [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/HEPData/hepdata_lib/master?filepath=examples/reading_histograms.ipynb)
+- [Reading a correlation matrix](examples/correlation.ipynb) [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/HEPData/hepdata_lib/master?filepath=examples/correlation.ipynb)
+- [Reading TGraph and TGraphError from '.C' files](examples/read_c_file.ipynb) [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/HEPData/hepdata_lib/master?filepath=examples/read_c_file.ipynb)
+
+## External dependencies
+
+- [ROOT](https://root.cern.ch)
+- [ImageMagick](https://www.imagemagick.org)
+
+Make sure that you have `ROOT` in your `$PYTHONPATH` and that the `convert` command is available by adding its location to your `$PATH` if needed.
+
+
```

### Comparing `hepdata_lib-0.8.1/README.md` & `hepdata_lib-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `hepdata_lib-0.8.1/hepdata_lib/__init__.py` & `hepdata_lib-0.9.0/hepdata_lib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                        SafeRepresenter.represent_str)
 yaml.add_representer(np.str_,
                        SafeRepresenter.represent_str)
 
 # Display deprecation warnings
 warnings.filterwarnings("always", category=DeprecationWarning, module="hepdata_lib")
 
-__version__ = "0.8.1"
+__version__ = "0.9.0"
 
 class AdditionalResourceMixin(object):
     """Functionality related to additional materials."""
 
     def __init__(self):
         self.files_to_copy = []
         self.additional_resources = []
```

### Comparing `hepdata_lib-0.8.1/hepdata_lib/c_file_reader.py` & `hepdata_lib-0.9.0/hepdata_lib/c_file_reader.py`

 * *Files identical despite different names*

### Comparing `hepdata_lib-0.8.1/hepdata_lib/helpers.py` & `hepdata_lib-0.9.0/hepdata_lib/helpers.py`

 * *Files identical despite different names*

### Comparing `hepdata_lib-0.8.1/hepdata_lib/root_utils.py` & `hepdata_lib-0.9.0/hepdata_lib/root_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,20 +48,23 @@
         if not self._tfile:
             raise IOError("RootReader: File not opened properly.")
 
     def retrieve_object(self, path_to_object):
         """
         Generalized function to retrieve a TObject from a file.
 
-        There are two use cases:
+        There are three use cases:
         1)  The object is saved under the exact path given.
         In this case, the function behaves identically to TFile.Get.
         2)  The object is saved as a primitive in a TCanvas.
         In this case, the path has to be formatted as
         PATH_TO_CANVAS/NAME_OF_PRIMITIVE
+        3)  The object is saved as a primitive in a TPad that is nested
+        in a TCanvas.  In this case, the path has to be formatted as
+        CANVAS/PAD1/PAD2.../NAME_OF_PRIMITIVE
 
 
         :param path_to_object: Absolute path in current TFile.
         :type path_to_object: str.
         :returns: TObject -- The object corresponding to the given path.
         """
         obj = self.tfile.Get(path_to_object)
@@ -85,20 +88,41 @@
             print("Available primitives in TCanvas '{0}':".format(
                 path_to_canvas))
             for entry in list(canv.GetListOfPrimitives()):
                 print("Name: '{0}', Type: '{1}'.".format(
                     entry.GetName(), type(entry)))
             assert False
 
+        except AssertionError:
+            # This is ok, it might be nested TPads
+            pass
+
+        # If the above didn't work, try nested tpads
+        try:
+            obj = self.tfile.Get(parts[0])
+            for part in parts[1:]:
+                obj = obj.GetPrimitive(part)
+
+            assert obj
+
+            return obj
         except AssertionError as err:
-            msg="Cannot find any object in file {0} with path {1}".format(
-                    self.tfile, path_to_object)
+            msg="Cannot find any object in file {0} using path {1} or interpreting it as a TCanvas"\
+                "with TPads.".format(self.tfile, path_to_object)
             raise_from(IOError(msg), err)
+
+        except AttributeError as err:
+            msg="Cannot find any object in file {0} using path {1} or interpreting it as a TCanvas"\
+                "with TPads.".format(self.tfile, path_to_object)
+            raise_from(IOError(msg), err)
+
         return None
 
+
+
     def read_graph(self, path_to_graph):
         """Extract lists of X and Y values from a TGraph.
 
         :param path_to_graph: Absolute path in the current TFile.
         :type path_to_graph: str
 
         :returns: dict -- For a description of the contents,
```

### Comparing `hepdata_lib-0.8.1/hepdata_lib.egg-info/PKG-INFO` & `hepdata_lib-0.9.0/hepdata_lib.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,89 +1,92 @@
 Metadata-Version: 2.1
 Name: hepdata-lib
-Version: 0.8.1
+Version: 0.9.0
 Summary: Library for getting your data into HEPData
 Home-page: https://github.com/HEPData/hepdata_lib
 Author: Andreas Albert, Clemens Lange
 Author-email: hepdata-lib@cern.ch
 License: UNKNOWN
 Project-URL: Documentation, https://hepdata-lib.readthedocs.io
 Project-URL: Bug Reports, https://github.com/HEPData/hepdata_lib/issues
 Project-URL: Source, https://github.com/HEPData/hepdata_lib
-Description: # hepdata_lib
-        
-        [![DOI](https://zenodo.org/badge/129248575.svg)](https://zenodo.org/badge/latestdoi/129248575)
-        [![PyPI version](https://badge.fury.io/py/hepdata-lib.svg)](https://badge.fury.io/py/hepdata-lib)
-        [![Actions Status](https://github.com/HEPData/hepdata_lib/workflows/tests/badge.svg)](https://github.com/HEPData/hepdata_lib/actions)
-        [![Coverage Status](https://coveralls.io/repos/github/HEPData/hepdata_lib/badge.svg?branch=master)](https://coveralls.io/github/HEPData/hepdata_lib?branch=master)
-        [![Documentation Status](https://readthedocs.org/projects/hepdata-lib/badge/)](http://hepdata-lib.readthedocs.io/)
-        [![Docker Hub](https://images.microbadger.com/badges/image/clelange/hepdata_lib.svg)](https://hub.docker.com/r/clelange/hepdata_lib/)
-        
-        Library for getting your data into HEPData
-        
-        ## Installation
-        
-        It is highly recommended you install `hepdata_lib` into a [virtual environment](https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/).
-        
-        ```shell
-        pip install hepdata_lib
-        ```
-        
-        If you are not sure about your Python environment, please also see below how to use `hepdata_lib` in a Docker or Singularity container.
-        
-        ## Getting started
-        
-        For using `hepdata_lib`, you don't even need to install it, but can use the [binder](https://mybinder.org/) or [SWAN](https://swan.cern.ch/) (CERN-only) services using one of the buttons below and following the instructions in the notebook with name [Getting_started](examples/Getting_started.ipynb):
-        
-        [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/HEPData/hepdata_lib/master?filepath=examples/Getting_started.ipynb)
-        [![SWAN](https://swanserver.web.cern.ch/swanserver/images/badge_swan_white_150.png)](https://cern.ch/swanserver/cgi-bin/go/?projurl=https://github.com/HEPData/hepdata_lib.git)
-        
-        You can also use the Docker image:
-        
-        ```shell
-        docker run --rm -it -p 8888:8888 -v ${PWD}:/home/hepdata clelange/hepdata_lib
-        ```
-        
-        And then point your browser to [http://localhost:8888](http://localhost:8888) and use the token that is printed out. The output will end up in your current working directory (`${PWD}`).
-        
-        If you prefer a shell, instead run:
-        
-        ```shell
-        docker run --rm -it -p 8888:8888 -v ${PWD}:/home/hepdata clelange/hepdata_lib bash
-        ```
-        
-        If on CERN LXPLUS or anywhere else where there is Singularity available but not Docker, you can still use the docker image:
-        
-        ```shell
-        export SINGULARITY_CACHEDIR="/tmp/$(whoami)/singularity"
-        singularity shell -B /afs -B /eos docker://clelange/hepdata_lib bash
-        ```
-        
-        Unpacking the image can take a few minutes the first time you use it. Please be patient. Both EOS and AFS should be available and the output will be in your current working directory.
-        
-        ## Further examples
-        
-        There are a few more examples available that can directly be run using the [binder](https://mybinder.org/) links below or using [SWAN](https://swan.cern.ch/) (CERN-only, please use LCG release LCG_94 or later) and selecting the corresponding notebook manually:
-        
-        - [Reading in text files](examples/Getting_started.ipynb) [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/HEPData/hepdata_lib/master?filepath=examples/Getting_started.ipynb)
-        - [Reading in a CMS combine ntuple](examples/combine_limits.ipynb) [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/HEPData/hepdata_lib/master?filepath=examples/combine_limits.ipynb)
-        - [Reading in ROOT histograms](examples/reading_histograms.ipynb) [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/HEPData/hepdata_lib/master?filepath=examples/reading_histograms.ipynb)
-        - [Reading a correlation matrix](examples/correlation.ipynb) [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/HEPData/hepdata_lib/master?filepath=examples/correlation.ipynb)
-        - [Reading TGraph and TGraphError from '.C' files](examples/read_c_file.ipynb) [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/HEPData/hepdata_lib/master?filepath=examples/read_c_file.ipynb)
-        
-        ## External dependencies
-        
-        - [ROOT](https://root.cern.ch)
-        - [ImageMagick](https://www.imagemagick.org)
-        
-        Make sure that you have `ROOT` in your `$PYTHONPATH` and that the `convert` command is available by adding its location to your `$PATH` if needed.
-        
 Keywords: HEPData physics OpenData
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# hepdata_lib
+
+[![DOI](https://zenodo.org/badge/129248575.svg)](https://zenodo.org/badge/latestdoi/129248575)
+[![PyPI version](https://badge.fury.io/py/hepdata-lib.svg)](https://badge.fury.io/py/hepdata-lib)
+[![Actions Status](https://github.com/HEPData/hepdata_lib/workflows/tests/badge.svg)](https://github.com/HEPData/hepdata_lib/actions)
+[![Coverage Status](https://coveralls.io/repos/github/HEPData/hepdata_lib/badge.svg?branch=master)](https://coveralls.io/github/HEPData/hepdata_lib?branch=master)
+[![Documentation Status](https://readthedocs.org/projects/hepdata-lib/badge/)](http://hepdata-lib.readthedocs.io/)
+[![Docker Hub](https://images.microbadger.com/badges/image/clelange/hepdata_lib.svg)](https://hub.docker.com/r/clelange/hepdata_lib/)
+
+Library for getting your data into HEPData
+
+## Installation
+
+It is highly recommended you install `hepdata_lib` into a [virtual environment](https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/).
+
+```shell
+pip install hepdata_lib
+```
+
+If you are not sure about your Python environment, please also see below how to use `hepdata_lib` in a Docker or Singularity container.
+
+## Getting started
+
+For using `hepdata_lib`, you don't even need to install it, but can use the [binder](https://mybinder.org/) or [SWAN](https://swan.cern.ch/) (CERN-only) services using one of the buttons below and following the instructions in the notebook with name [Getting_started](examples/Getting_started.ipynb):
+
+[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/HEPData/hepdata_lib/master?filepath=examples/Getting_started.ipynb)
+[![SWAN](https://swanserver.web.cern.ch/swanserver/images/badge_swan_white_150.png)](https://cern.ch/swanserver/cgi-bin/go/?projurl=https://github.com/HEPData/hepdata_lib.git)
+
+You can also use the Docker image:
+
+```shell
+docker run --rm -it -p 8888:8888 -v ${PWD}:/home/hepdata clelange/hepdata_lib
+```
+
+And then point your browser to [http://localhost:8888](http://localhost:8888) and use the token that is printed out. The output will end up in your current working directory (`${PWD}`).
+
+If you prefer a shell, instead run:
+
+```shell
+docker run --rm -it -p 8888:8888 -v ${PWD}:/home/hepdata clelange/hepdata_lib bash
+```
+
+If on CERN LXPLUS or anywhere else where there is Singularity available but not Docker, you can still use the docker image:
+
+```shell
+export SINGULARITY_CACHEDIR="/tmp/$(whoami)/singularity"
+singularity shell -B /afs -B /eos docker://clelange/hepdata_lib bash
+```
+
+Unpacking the image can take a few minutes the first time you use it. Please be patient. Both EOS and AFS should be available and the output will be in your current working directory.
+
+## Further examples
+
+There are a few more examples available that can directly be run using the [binder](https://mybinder.org/) links below or using [SWAN](https://swan.cern.ch/) (CERN-only, please use LCG release LCG_94 or later) and selecting the corresponding notebook manually:
+
+- [Reading in text files](examples/Getting_started.ipynb) [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/HEPData/hepdata_lib/master?filepath=examples/Getting_started.ipynb)
+- [Reading in a CMS combine ntuple](examples/combine_limits.ipynb) [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/HEPData/hepdata_lib/master?filepath=examples/combine_limits.ipynb)
+- [Reading in ROOT histograms](examples/reading_histograms.ipynb) [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/HEPData/hepdata_lib/master?filepath=examples/reading_histograms.ipynb)
+- [Reading a correlation matrix](examples/correlation.ipynb) [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/HEPData/hepdata_lib/master?filepath=examples/correlation.ipynb)
+- [Reading TGraph and TGraphError from '.C' files](examples/read_c_file.ipynb) [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/HEPData/hepdata_lib/master?filepath=examples/read_c_file.ipynb)
+
+## External dependencies
+
+- [ROOT](https://root.cern.ch)
+- [ImageMagick](https://www.imagemagick.org)
+
+Make sure that you have `ROOT` in your `$PYTHONPATH` and that the `convert` command is available by adding its location to your `$PATH` if needed.
+
+
```

### Comparing `hepdata_lib-0.8.1/setup.py` & `hepdata_lib-0.9.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 from os import path
 from setuptools import setup, find_packages
 try:
     import ROOT  # pylint: disable=W0611
 except ImportError:
     print("ROOT is required by this library.")
 
-DEPS = ['numpy', 'PyYAML>4.*', 'future', 'six', 'pylint==2.9.6']
+DEPS = ['numpy', 'PyYAML>4.*', 'future', 'six']
 
 HERE = path.abspath(path.dirname(__file__))
 
 with codecs.open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name='hepdata_lib',
-    version='0.8.1',
+    version='0.9.0',
     description='Library for getting your data into HEPData',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     url='https://github.com/HEPData/hepdata_lib',
     author='Andreas Albert, Clemens Lange',
     author_email='hepdata-lib@cern.ch',
     classifiers=[
@@ -34,13 +34,16 @@
         'Programming Language :: Python :: 3.7',
     ],
     keywords='HEPData physics OpenData',
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),
     zip_safe=False,
     install_requires=DEPS,
     setup_requires=['pytest-runner', 'pytest-cov'],
-    tests_require=['pytest', 'papermill', 'six'],
+    tests_require=['pytest', 'papermill', 'six',
+                   'pylint==1.9.5; python_version<"3"',
+                   'pylint==2.9.6; python_version>="3"',
+                  ],
     project_urls={
         'Documentation': 'https://hepdata-lib.readthedocs.io',
         'Bug Reports': 'https://github.com/HEPData/hepdata_lib/issues',
         'Source': 'https://github.com/HEPData/hepdata_lib',
     }, )
```

