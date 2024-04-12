# Comparing `tmp/spcm-1.0.6.tar.gz` & `tmp/spcm-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spcm-1.0.6.tar", last modified: Fri Mar 22 12:56:38 2024, max compression
+gzip compressed data, was "spcm-1.1.0.tar", last modified: Fri Apr 12 11:28:29 2024, max compression
```

## Comparing `spcm-1.0.6.tar` & `spcm-1.1.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 12:56:38.445688 spcm-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-22 12:56:34.000000 spcm-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-22 12:56:34.000000 spcm-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17596 2024-03-22 12:56:38.445688 spcm-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16227 2024-03-22 12:56:34.000000 spcm-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-03-22 12:56:34.000000 spcm-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 12:56:38.445688 spcm-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-22 12:56:34.000000 spcm-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 12:56:38.437687 spcm-1.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 12:56:38.441687 spcm-1.0.6/src/spcm/
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-03-22 12:56:34.000000 spcm-1.0.6/src/spcm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-22 12:56:38.445688 spcm-1.0.6/src/spcm/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-03-22 12:56:34.000000 spcm-1.0.6/src/spcm/classes_block_average.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-03-22 12:56:34.000000 spcm-1.0.6/src/spcm/classes_boxcar.py
--rw-r--r--   0 runner    (1001) docker     (127)     9610 2024-03-22 12:56:34.000000 spcm-1.0.6/src/spcm/classes_card.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-03-22 12:56:34.000000 spcm-1.0.6/src/spcm/classes_card_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)    18677 2024-03-22 12:56:34.000000 spcm-1.0.6/src/spcm/classes_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-03-22 12:56:34.000000 spcm-1.0.6/src/spcm/classes_clock.py
--rw-r--r--   0 runner    (1001) docker     (127)    22190 2024-03-22 12:56:34.000000 spcm-1.0.6/src/spcm/classes_data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)    37847 2024-03-22 12:56:34.000000 spcm-1.0.6/src/spcm/classes_dds.py
--rw-r--r--   0 runner    (1001) docker     (127)    17545 2024-03-22 12:56:34.000000 spcm-1.0.6/src/spcm/classes_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-03-22 12:56:34.000000 spcm-1.0.6/src/spcm/classes_error_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-22 12:56:34.000000 spcm-1.0.6/src/spcm/classes_functionality.py
--rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-03-22 12:56:34.000000 spcm-1.0.6/src/spcm/classes_multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-03-22 12:56:34.000000 spcm-1.0.6/src/spcm/classes_multi_purpose_ios.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-03-22 12:56:34.000000 spcm-1.0.6/src/spcm/classes_netbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    17355 2024-03-22 12:56:34.000000 spcm-1.0.6/src/spcm/classes_pulse_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-03-22 12:56:34.000000 spcm-1.0.6/src/spcm/classes_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-03-22 12:56:34.000000 spcm-1.0.6/src/spcm/classes_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-03-22 12:56:34.000000 spcm-1.0.6/src/spcm/classes_time_stamp.py
--rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-03-22 12:56:34.000000 spcm-1.0.6/src/spcm/classes_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-22 12:56:34.000000 spcm-1.0.6/src/spcm/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    13312 2024-03-22 12:56:34.000000 spcm-1.0.6/src/spcm/pyspcm.py
--rw-r--r--   0 runner    (1001) docker     (127)    89313 2024-03-22 12:56:34.000000 spcm-1.0.6/src/spcm/regs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-03-22 12:56:34.000000 spcm-1.0.6/src/spcm/spcerr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 12:56:38.445688 spcm-1.0.6/src/spcm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17596 2024-03-22 12:56:38.000000 spcm-1.0.6/src/spcm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-22 12:56:38.000000 spcm-1.0.6/src/spcm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 12:56:38.000000 spcm-1.0.6/src/spcm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-22 12:56:38.000000 spcm-1.0.6/src/spcm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-22 12:56:38.000000 spcm-1.0.6/src/spcm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-03-22 12:56:34.000000 spcm-1.0.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:28:29.490815 spcm-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-12 11:28:25.000000 spcm-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 11:28:25.000000 spcm-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21586 2024-04-12 11:28:29.490815 spcm-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20191 2024-04-12 11:28:25.000000 spcm-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-12 11:28:25.000000 spcm-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 11:28:29.490815 spcm-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-12 11:28:25.000000 spcm-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:28:29.482815 spcm-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:28:29.490815 spcm-1.1.0/src/spcm/
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-12 11:28:25.000000 spcm-1.1.0/src/spcm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-12 11:28:29.490815 spcm-1.1.0/src/spcm/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-12 11:28:25.000000 spcm-1.1.0/src/spcm/classes_block_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-12 11:28:25.000000 spcm-1.1.0/src/spcm/classes_boxcar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9985 2024-04-12 11:28:25.000000 spcm-1.1.0/src/spcm/classes_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-04-12 11:28:25.000000 spcm-1.1.0/src/spcm/classes_card_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28176 2024-04-12 11:28:25.000000 spcm-1.1.0/src/spcm/classes_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-12 11:28:25.000000 spcm-1.1.0/src/spcm/classes_clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28626 2024-04-12 11:28:25.000000 spcm-1.1.0/src/spcm/classes_data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43006 2024-04-12 11:28:25.000000 spcm-1.1.0/src/spcm/classes_dds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18266 2024-04-12 11:28:25.000000 spcm-1.1.0/src/spcm/classes_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-04-12 11:28:25.000000 spcm-1.1.0/src/spcm/classes_error_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-12 11:28:25.000000 spcm-1.1.0/src/spcm/classes_functionality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-04-12 11:28:25.000000 spcm-1.1.0/src/spcm/classes_multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-04-12 11:28:25.000000 spcm-1.1.0/src/spcm/classes_multi_purpose_ios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-04-12 11:28:25.000000 spcm-1.1.0/src/spcm/classes_netbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25635 2024-04-12 11:28:25.000000 spcm-1.1.0/src/spcm/classes_pulse_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-04-12 11:28:25.000000 spcm-1.1.0/src/spcm/classes_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-12 11:28:25.000000 spcm-1.1.0/src/spcm/classes_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-12 11:28:25.000000 spcm-1.1.0/src/spcm/classes_time_stamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15868 2024-04-12 11:28:25.000000 spcm-1.1.0/src/spcm/classes_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-12 11:28:25.000000 spcm-1.1.0/src/spcm/classes_unit_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-12 11:28:25.000000 spcm-1.1.0/src/spcm/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13302 2024-04-12 11:28:25.000000 spcm-1.1.0/src/spcm/pyspcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89313 2024-04-12 11:28:25.000000 spcm-1.1.0/src/spcm/regs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-12 11:28:25.000000 spcm-1.1.0/src/spcm/spcerr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:28:29.490815 spcm-1.1.0/src/spcm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21586 2024-04-12 11:28:29.000000 spcm-1.1.0/src/spcm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-12 11:28:29.000000 spcm-1.1.0/src/spcm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:28:29.000000 spcm-1.1.0/src/spcm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 11:28:29.000000 spcm-1.1.0/src/spcm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-12 11:28:29.000000 spcm-1.1.0/src/spcm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-12 11:28:25.000000 spcm-1.1.0/versioneer.py
```

### Comparing `spcm-1.0.6/LICENSE` & `spcm-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spcm-1.0.6/PKG-INFO` & `spcm-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,7 @@
-Metadata-Version: 2.1
-Name: spcm
-Version: 1.0.6
-Summary: Package for Spectrum Instrumentation GmbH cards
-Author-email: Spectrum Instrumentation GmbH <info@spec.de>
-Project-URL: Homepage, https://spectrum-instrumentation.com/
-Project-URL: API, https://spectruminstrumentation.github.io/spcm/spcm.html
-Project-URL: Repository, https://github.com/SpectrumInstrumentation/spcm
-Project-URL: Examples, https://github.com/SpectrumInstrumentation/spcm/tree/master/src/examples
-Project-URL: Knowledge Base, https://spectrum-instrumentation.com/support/knowledgebase/index.php
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: System :: Hardware
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy>=1.25.2
-Requires-Dist: h5py>=3.10.0
-
 <div style="margin-bottom: 20px; text-align: center">
 <a href="https://spectrum-instrumentation.com">
     <img src="https://spectrum-instrumentation.com/img/logo-complete.png"  width=400 />
 </a>
 </div>
 
 # spcm
@@ -48,33 +18,37 @@
 # Supported devices
 
 See the [SUPPORTED_DEVICES.md](https://github.com/SpectrumInstrumentation/spcm/blob/master/src/spcm/SUPPORTED_DEVICES.md) file for a list of supported devices.
 
 # Requirements
 [![Python](https://img.shields.io/pypi/pyversions/spcm.svg)](https://badge.fury.io/py/spcm)
 [![Static Badge](https://img.shields.io/badge/NumPy-1.25-green)](https://numpy.org/)
+[![Static Badge](https://img.shields.io/badge/h5py-3.10-orange)](https://www.h5py.org/)
 
 `spcm` requires the Spectrum Instrumentation [driver](https://spectrum-instrumentation.com/support/downloads.php) which is available for Windows and Linux. 
 Please have a look in the manual of your product for more information about installing the driver on the different plattforms.
 
 # Installation and dependencies
 [![Pip Package](https://img.shields.io/pypi/v/spcm?logo=PyPI)](https://pypi.org/project/spcm)
+[![Publish to PyPI](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/spcm-publish-to-pypi.yml/badge.svg)](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/spcm-publish-to-pypi.yml)
 
 Start by installing Python 3.9 or higher. We recommend using the latest version. You can download Python from [https://www.python.org/](https://www.python.org/).
 
 You would probably also like to install and use a virtual environment, although it's not strictly necessary. See the examples [README.md](https://github.com/SpectrumInstrumentation/spcm/blob/master/src/examples/README.md) for a more detailed explanation on how to use `spcm` in a virtual environment.
 
 To install the latest release using `pip`:
 ```bash
 $ pip install spcm
 ```
-Note that: this will automatically install all the dependencies (e.g. NumPy).
+Note that: this will automatically install all the dependencies.
 
 # Documentation
 [![Documentation](https://img.shields.io/badge/api-reference-blue.svg)](https://spectruminstrumentation.github.io/spcm/spcm.html)
+[![Build dosc](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/spcm-docs-pages.yml/badge.svg)](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/spcm-docs-pages.yml)
+[![Publish docs](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/pages/pages-build-deployment)
 
 The API documentation for the latest [stable release](https://spectruminstrumentation.github.io/spcm/spcm.html) is available for reading on GitHub pages.
 
 Please also see the hardware user manuals for your specific card for more information about the provided functionality.
 
 # Using spcm
 
@@ -159,14 +133,40 @@
 See the register `SPC_PCISERIALNO` in the reference manual of your specific device for more information.
 
 If the `device_identifier` is given that card is opened, if at the same time `card_type` or `serial_number` are given then these behave as an additional check too see if the opened card is of a certain type or has that specific serial number.
 
 ### Demo devices
 To test the Spectrum Instrumentation API with user code without hardware, the Control Center gives the user the option to create [demo devices](https://spectrum-instrumentation.com/support/knowledgebase/software/How_to_set_up_a_demo_card.php). These demo devices can be used in the same manner as real devices. Simply change the device identifier string to the string as shown in the Control Center.
 
+## Units and quantities
+
+`spcm` uses [pint](https://pint.readthedocs.io/en/stable/) to handle all quantities that have a physical unit. To enable the use of qunatities simply import the units module from `spcm`:
+
+```python
+from spcm import units
+```
+
+This import the `units` object from `spcm`. which is a `UnitRegistry` object from  `pint`. Defining a quantity is as simples as:
+
+```python
+from spcm import units
+
+frequency = 100 * units.MHz
+amplitude = 1 * units.V
+# etc...
+```
+
+All methods within the `spcm` that expect a value that is related to a physical quantity support the quantities, for example setting a timeout:
+
+```python
+card.timeout(5 * units.s)
+```
+
+See our dedicated examples for more information about where units can be used.
+
 ## Card Functionality
 After opening a card, StarHub or group of card, specific functionality of the cards can be accessed through `CardFunctionality` classes. 
 
 | Name                | Description                                                         |
 |---------------------|---------------------------------------------------------------------|
 | `Channels`          | class for setting up the in- or output stage of the channels of a card |
 | `Clock`             | class for setting up the clock engine of the card                   |
@@ -196,52 +196,78 @@
     # (or)
     data_transfer = spcm.DataTransfer(card)
     # etc ...
 
 ```
 Each of these functionalities typically corresponds to a chapter in your device manual, so for further reference please have a look in the device manual.
 
+## Setting up Channels
+
+The Channels functionality allows the user to setup individual channels on a Card or a CardStack. The channels object is also a Python iterator, hence if a channels object is used it a for-loop, each iteration provides a Channel object:
+
+```python
+channels = spcm.Channels(card, card_enable=spcm.CHANNEL0 | CHANNEL1)
+for channel in channels:
+    # do something with each channel
+```
+
+In addition, the user can define the output load connected to the channel (standard value 50 Ohm), to any resistor value or high impedance (`units.highZ`). With this output load, the amplitude setting can be done with the repect to this output load:
+
+```python
+channels = Channels(card, card_enable=spcm.CHANNEL0 | CHANNEL1)
+channels[0].output_load(units.highZ)
+channels[0].amp(1 * units.V)
+# or for all channels
+channels.output_load(units.highZ)
+channels.amp(1 * units.V)
+```
+
+This information allows the user to convert the data coming from `DataTransfer`, using the `convert_data()` method. See the section "Setting up a data transfer buffer ..." for more details.
+
 ## Setting up the Clock engine
 
 The Clock engine is used to generate a clock signal that is used as the source for all timing critical processes on the card.
 
 ### Sample rate
 To get the maximum sample rate of the active card and set the sample rate to the maximum, this is an example using internal PLL clock mode:
 ```python
 clock = spcm.Clock(card)
 clock.mode(spcm.SPC_CM_INTPLL)
-sample_rate = clock.sample_rate(max=True) # (or) sample_rate = clock.sample_rate(20e6) # for a 20 MHz sample rate (see reference manual for allowed values)
-print("Current sample rate: {}S/s".format(sample_rate))
+sample_rate = clock.sample_rate(max=True) 
+# (or) 
+sample_rate = clock.sample_rate(20 * units.MHz) # for a 20 MHz sample rate (see reference manual for allowed values)
+print("Current sample rate: {}".format(sample_rate, return_unit=units.MS/units.s))
 ```
 
 ## Setting up the Trigger engine
 
 ### External trigger
 
 The Trigger engine can be configured for a multitude of different configurations (see the hardware manual for more information about the specific configurations for your device). Here we've given an example for an external trigger arriving at input port ext0, that is DC-coupled. The card is waiting for positiv edge that excedes 1.5 V:
 
 ```python
 trigger = spcm.Trigger(card)
 trigger.or_mask(spcm.SPC_TMASK_EXT0) # set the ext0 hardware input as trigger source
 trigger.ext0_mode(spcm.SPC_TM_POS) # wait for a positive edge
-trigger.ext0_level0(1500) # Trigger level is 1.5 V (1500 mV)
+trigger.ext0_level0(1.5 * units.V)
 trigger.ext0_coupling(spcm.COUPLING_DC) # set DC coupling
 ```
 
 ## Setting up the multi-purpose I/O lines
 
 See the hardware manual, for the multi-purpose I/O lines functionality that can be programmed.
 
 ## Setting up a data transfer buffer for recording (digitizer) or replay (AWG)
 
 ### Recording (Digitizing)
 To transfer data to or from the card, we have to setup a data transfer object. This object allocates an amount the memory of the card (`memory_size`) and a Direct Memory Access (DMA) buffer on the host pc (`allocate_buffer`). Half of the samples are taken before the trigger, as configured by the trigger engine, and half of the samples are recorded afterwards. Then the transfer from the card to the host pc is started and the program waits until the DMA is filled.
 
 ```python
 # define the data buffer
+num_samples = 4 * units.KiS # 1 KiS = 1 KibiSamples = 1024 Samples
 data_transfer = spcm.DataTransfer(card)
 data_transfer.memory_size(num_samples)
 data_transfer.allocate_buffer(num_samples)
 data_transfer.post_trigger(num_samples // 2)
 # Start DMA transfer
 data_transfer.start_buffer_transfer(spcm.M2CMD_DATA_STARTDMA)
 
@@ -263,32 +289,55 @@
 
 This data can be further processed or plotted using, for example, [`matplotlib`](https://matplotlib.org/).
 
 ### Replay (Generation)
 
 The setup of the DMA for replay is very similar. First card memory is allocated with `memory_size` and then a DMA buffer is allocated (`allocated_buffer`) and made accessible though the NumPy object `data_transfer.buffer`, which can then be written to using standard NumPy methods. Finally, data transfer from the host PC to the card is started and the programming is waiting until all the data is transferred:
 ```python
+num_samples = 4 * units.KiS # 1 KiS = 1 KibiSamples = 1024 Samples
 data_transfer = spcm.DataTransfer(card)
 data_transfer.memory_size(num_samples)
 data_transfer.allocate_buffer(num_samples)
 data_transfer.loops(0) # loop continuously
 # simple linear ramp for analog output cards
-data_transfer.buffer[:] = np.arange(-num_samples//2, num_samples//2).astype(np.int16)
+num_samples_magnitude = num_samples.to(units.S).magnitude
+data_transfer.buffer[:] = np.arange(-num_samples_magnitude//2, num_samples_magnitude//2).astype(np.int16)
 
 data_transfer.start_buffer_transfer(spcm.M2CMD_DATA_STARTDMA, spcm.M2CMD_DATA_WAITDMA)
 ```
 
+#### Data transfer
+
+In the above it's assume that all the data has been transferred from the card into the buffer object, however if you're working in FIFO mode or you've defined the buffer to be smaller then the assigned card memory size, then the card will write to parts of the memory and tell you were it wrote. 
+
+This can be either handled manually (see the reference manual of your card, or the methods `avail_card_len()`, `avail_user_pos()` and `avail_user_len()`).
+
+Secondly, it can also be handled with Python iterators functionality. If the `data_transfer` object is handed to a for-loop, then in each iteration a view of the current active memory part is given in the form of a NumPy array and the user can do calculations on that.
+
+```python
+# Get a block of data
+for data_block in data_transfer:
+    # data_block is a NumPy array view of the currently active buffer part
+    for channel in channels:
+        data_units = channel.convert_data(data_block[:, channel])
+        minimum = np.min(data_units)
+        maximum = np.max(data_units)
+        print(f"Minimum: {minimum} - maximum: {maximum}")
+```
+
+The same principle also works with generator cards (see the example `2_gen_fifo.py`).
+
 ## Multiple recording / replay
 
 In case of multiple recording / replay, the memory is divided in equally sized segments, that are populated / replayed when a trigger is detected. Multiple triggers each trigger the next segment to be populated or replayed.
 
 The following code snippet shows how to setup the buffer for 4 segments with each 128 Samples:
 
 ```python
-samples_per_segment = 128
+samples_per_segment = 128 * units.S
 num_segments = 4
 multiple_recording = spcm.Multi(card)
 multiple_recording.memory_size(samples_per_segment*num_segments)
 multiple_recording.allocate_buffer(segment_samples=samples_per_segment, num_segments=num_segments)
 multiple_recording.post_trigger(samples_per_segment // 2)
 multiple_recording.start_buffer_transfer(spcm.M2CMD_DATA_STARTDMA)
 ```
@@ -314,26 +363,25 @@
 
 Please see the folder `4_pulse-generator` in the `examples` folder for several dedicated examples. In the following, there is a simple example for setting up a single pulse generator on x0.
 
 Create a pulse generators object and get the clock rate used by the pulse generator. Use that to calculate the period of a 1 MHz signal and the half of that period we'll have a high signal (hence 50% duty cycle). The pulse generator will start if the trigger condition is met without delay and loops infinitely many times. The triggering condition is set to the card software trigger. See more details in the pulse generator chapter in the specific hardware manual.
 
 ```python
 pulse_generators = spcm.PulseGenerators(card)
-# get the clock of the card
-pulse_gen_clock_Hz = pulse_generators.get_clock()
 
 # generate a continuous signal with 1 MHz
-len_for_1MHz = pulse_gen_clock_Hz // spcm.MEGA(1)
-pulse_generators[0].mode(spcm.SPCM_PULSEGEN_MODE_TRIGGERED)
-pulse_generators[0].period_length(len_for_1MHz)
-pulse_generators[0].high_length(len_for_1MHz // 2) # 50% HIGH, 50% LOW
-pulse_generators[0].delay(0)
-pulse_generators[0].num_loops(0) # 0: infinite
-pulse_generators[0].mux1(spcm.SPCM_PULSEGEN_MUX1_SRC_UNUSED)
-pulse_generators[0].mux2(spcm.SPCM_PULSEGEN_MUX2_SRC_SOFTWARE) # started by software force command
+pulse_generators[0].pulse_period(1 * units.us)
+# pulse_generators[0].repetition_rate(1 * units.MHz) # (or)
+pulse_generators[0].duty_cycle(50 * units.percent)
+# pulse_generators[0].pulse_length(0.5 * units.us) # (or)
+pulse_generators[0].start_delay(0 * units.us)
+pulse_generators[0].repetitions(0) # 0: infinite
+pulse_generators[0].start_condition_state_signal(spcm.SPCM_PULSEGEN_MUX1_SRC_UNUSED)
+pulse_generators[0].start_condition_trigger_signal(spcm.SPCM_PULSEGEN_MUX2_SRC_SOFTWARE)
+pulse_generators[0].invert_start_condition(False)
 
 # and write the pulse generator settings
 pulse_generators.write_setup()
 
 # start all pulse generators that wait for a software command
 pulse_generators.force()
 ```
@@ -354,8 +402,8 @@
 
 ### Block average (Digitizer only)
 
 See the corresponding chapter in the hardware manual for more information about block averaging and the registers used.
 
 # Acknowledgements
 
-We would like to thank [Christian Baker](https://github.com/crnbaker) for fruitful discussions and inspiration on how to setup the `spcm` package.
+We would like to thank [Christian Baker](https://github.com/crnbaker) for fruitful discussions and inspiration on how to setup the `spcm` package.
```

#### html2text {}

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1 Name: spcm Version: 1.0.6 Summary: Package for Spectrum
-Instrumentation GmbH cards Author-email: Spectrum Instrumentation GmbH
-spec.de> Project-URL: Homepage, https://spectrum-instrumentation.com/ Project-
-URL: API, https://spectruminstrumentation.github.io/spcm/spcm.html Project-URL:
-Repository, https://github.com/SpectrumInstrumentation/spcm Project-URL:
-Examples, https://github.com/SpectrumInstrumentation/spcm/tree/master/src/
-examples Project-URL: Knowledge Base, https://spectrum-instrumentation.com/
-support/knowledgebase/index.php Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
-Natural Language :: English Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows Classifier: Programming
-Language :: Python Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Scientific/Engineering Classifier: Topic :: System ::
-Hardware Requires-Python: >=3.9 Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: numpy>=1.25.2 Requires-Dist: h5py>=3.10.0
 _[_h_t_t_p_s_:_/_/_s_p_e_c_t_r_u_m_-_i_n_s_t_r_u_m_e_n_t_a_t_i_o_n_._c_o_m_/_i_m_g_/_l_o_g_o_-_c_o_m_p_l_e_t_e_._p_n_g_]
 # spcm [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)]
 (https://opensource.org/licenses/MIT) [![PyPI - Version](https://
 img.shields.io/pypi/v/spcm)](https://pypi.org/project/spcm) [![PyPi Downloads]
 (https://img.shields.io/pypi/dm/spcm?label=downloads%20%7C%20pip&logo=PyPI)]
 (https://pypi.org/project/spcm) [![Follow](https://img.shields.io/twitter/
 follow/
@@ -29,58 +11,67 @@
 oriented Python package for interfacing with Spectrum Instrumentation GmbH
 devices. `spcm` can handle individual cards (`Card`), StarHubs (`Sync`), groups
 of cards (`CardStack`) and Netboxes (`Netbox`). # Supported devices See the
 [SUPPORTED_DEVICES.md](https://github.com/SpectrumInstrumentation/spcm/blob/
 master/src/spcm/SUPPORTED_DEVICES.md) file for a list of supported devices. #
 Requirements [![Python](https://img.shields.io/pypi/pyversions/spcm.svg)]
 (https://badge.fury.io/py/spcm) [![Static Badge](https://img.shields.io/badge/
-NumPy-1.25-green)](https://numpy.org/) `spcm` requires the Spectrum
+NumPy-1.25-green)](https://numpy.org/) [![Static Badge](https://img.shields.io/
+badge/h5py-3.10-orange)](https://www.h5py.org/) `spcm` requires the Spectrum
 Instrumentation [driver](https://spectrum-instrumentation.com/support/
 downloads.php) which is available for Windows and Linux. Please have a look in
 the manual of your product for more information about installing the driver on
 the different plattforms. # Installation and dependencies [![Pip Package]
 (https://img.shields.io/pypi/v/spcm?logo=PyPI)](https://pypi.org/project/spcm)
-Start by installing Python 3.9 or higher. We recommend using the latest
-version. You can download Python from [https://www.python.org/](https://
-www.python.org/). You would probably also like to install and use a virtual
-environment, although it's not strictly necessary. See the examples [README.md]
-(https://github.com/SpectrumInstrumentation/spcm/blob/master/src/examples/
-README.md) for a more detailed explanation on how to use `spcm` in a virtual
-environment. To install the latest release using `pip`: ```bash $ pip install
-spcm ``` Note that: this will automatically install all the dependencies (e.g.
-NumPy). # Documentation [![Documentation](https://img.shields.io/badge/api-
-reference-blue.svg)](https://spectruminstrumentation.github.io/spcm/spcm.html)
-The API documentation for the latest [stable release](https://
-spectruminstrumentation.github.io/spcm/spcm.html) is available for reading on
-GitHub pages. Please also see the hardware user manuals for your specific card
-for more information about the provided functionality. # Using spcm The `spcm`
-package is a high-level object-oriented programming library for controlling
-Spectrum Instrumentation devices. ## Examples For detailed examples see the
-`src\examples` directory. There are several sub-directories each corresponding
-to a certain kind of functionality. See also the examples on [GitHub](https://
-github.com/SpectrumInstrumentation/spcm/tree/master/src/examples). ## Hardware
-interfaces `spcm` provides the following classes for interfacing with the
-different devices. | Name | Description | |-------------|----------------------
--------------------------------------------------------------| | `Card` | a
-class to control the low-level API of Spectrum Instrumentation cards. | |
-`Sync` | a class for controling StarHub devices. | | `CardStack` | a class that
-handles the opening and closing of a combination of different cards either with
-or without a StarHub that synchronizes the cards. | | `Netbox` | a class that
-handles the opening and closing of the cards in a Netbox | ## Connect to a
-device Opening and closing of cards is handled using the python [`with`](https:
-//peps.python.org/pep-0343/) statement. This creates a context manager that
-safely handles opening and closing of a card or a group of cards. ### Using
-device identifiers Connect to local cards: ```python import spcm with spcm.Card
-('/dev/spcm0') as card: # (add your code here) ``` Connect to remote cards (you
-can find a card's IP using the [Spectrum Control Center](https://spectrum-
-instrumentation.com/en/spectrum-control-center) software): ```python import
-spcm with spcm.Card('TCPIP::192.168.1.10::inst0::INSTR') as card: # (add your
-code here) ``` Connect to a group of cards synchronized using a StarHub:
-```python import spcm card_identifiers = ["/dev/spcm0", "/dev/spcm1"]
-sync_identifier = "sync0" with spcm.CardStack
+[![Publish to PyPI](https://github.com/SpectrumInstrumentation/spcm/actions/
+workflows/spcm-publish-to-pypi.yml/badge.svg)](https://github.com/
+SpectrumInstrumentation/spcm/actions/workflows/spcm-publish-to-pypi.yml) Start
+by installing Python 3.9 or higher. We recommend using the latest version. You
+can download Python from [https://www.python.org/](https://www.python.org/).
+You would probably also like to install and use a virtual environment, although
+it's not strictly necessary. See the examples [README.md](https://github.com/
+SpectrumInstrumentation/spcm/blob/master/src/examples/README.md) for a more
+detailed explanation on how to use `spcm` in a virtual environment. To install
+the latest release using `pip`: ```bash $ pip install spcm ``` Note that: this
+will automatically install all the dependencies. # Documentation [!
+[Documentation](https://img.shields.io/badge/api-reference-blue.svg)](https://
+spectruminstrumentation.github.io/spcm/spcm.html) [![Build dosc](https://
+github.com/SpectrumInstrumentation/spcm/actions/workflows/spcm-docs-pages.yml/
+badge.svg)](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/
+spcm-docs-pages.yml) [![Publish docs](https://github.com/
+SpectrumInstrumentation/spcm/actions/workflows/pages/pages-build-deployment/
+badge.svg)](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/
+pages/pages-build-deployment) The API documentation for the latest [stable
+release](https://spectruminstrumentation.github.io/spcm/spcm.html) is available
+for reading on GitHub pages. Please also see the hardware user manuals for your
+specific card for more information about the provided functionality. # Using
+spcm The `spcm` package is a high-level object-oriented programming library for
+controlling Spectrum Instrumentation devices. ## Examples For detailed examples
+see the `src\examples` directory. There are several sub-directories each
+corresponding to a certain kind of functionality. See also the examples on
+[GitHub](https://github.com/SpectrumInstrumentation/spcm/tree/master/src/
+examples). ## Hardware interfaces `spcm` provides the following classes for
+interfacing with the different devices. | Name | Description | |-------------|-
+-------------------------------------------------------------------------------
+---| | `Card` | a class to control the low-level API of Spectrum
+Instrumentation cards. | | `Sync` | a class for controling StarHub devices. | |
+`CardStack` | a class that handles the opening and closing of a combination of
+different cards either with or without a StarHub that synchronizes the cards. |
+| `Netbox` | a class that handles the opening and closing of the cards in a
+Netbox | ## Connect to a device Opening and closing of cards is handled using
+the python [`with`](https://peps.python.org/pep-0343/) statement. This creates
+a context manager that safely handles opening and closing of a card or a group
+of cards. ### Using device identifiers Connect to local cards: ```python import
+spcm with spcm.Card('/dev/spcm0') as card: # (add your code here) ``` Connect
+to remote cards (you can find a card's IP using the [Spectrum Control Center]
+(https://spectrum-instrumentation.com/en/spectrum-control-center) software):
+```python import spcm with spcm.Card('TCPIP::192.168.1.10::inst0::INSTR') as
+card: # (add your code here) ``` Connect to a group of cards synchronized using
+a StarHub: ```python import spcm card_identifiers = ["/dev/spcm0", "/dev/
+spcm1"] sync_identifier = "sync0" with spcm.CardStack
 (card_identifiers=card_identifiers, sync_identifier=sync_identifier) as stack:
 # (add your code here) ``` The `CardStack` object contains a list of `Card`
 objects in the `stack.cards` parameter and a `Sync` object in the parameter
 `stack.sync`. ### Using card type or serial number Apart from connecting to a
 device directly through a device identifier it's also possible to connect to
 local devices using the card type or serial number. To find the first card of
 type analog out (`SPCM_TYPE_AO`) you can do the following: ```python import
@@ -95,62 +86,87 @@
 given then these behave as an additional check too see if the opened card is of
 a certain type or has that specific serial number. ### Demo devices To test the
 Spectrum Instrumentation API with user code without hardware, the Control
 Center gives the user the option to create [demo devices](https://spectrum-
 instrumentation.com/support/knowledgebase/software/
 How_to_set_up_a_demo_card.php). These demo devices can be used in the same
 manner as real devices. Simply change the device identifier string to the
-string as shown in the Control Center. ## Card Functionality After opening a
-card, StarHub or group of card, specific functionality of the cards can be
-accessed through `CardFunctionality` classes. | Name | Description | |---------
-------------|------------------------------------------------------------------
----| | `Channels` | class for setting up the in- or output stage of the
-channels of a card | | `Clock` | class for setting up the clock engine of the
-card | | `Trigger` | class for setting up the trigger engine of the card | |
-`MultiPurposeIOs` | class for setting up the multi purpose i/o of the card | |
-`DataTransfer` | class for handling data transfer functionality | | `Multi` |
-class for handling multiple recording and replay mode functionality | |
-`Sequence` | class for handling sequence mode functionality | | `TimeStamp` |
-class for handling time stamped data | | `Boxcar` | class for handling boxcar
-averaging | | `BlockAverage` | class for handling block averaging functionality
-| | `PulseGenerators` | class for setting up the pulse generator functionality
-| | `DDS` | class for handling DDS functionality | To use a specific
-functionality simply initiate an instance of one of the classes and pass a
-device object: ```python import spcm with spcm.Card('/dev/spcm0') as card:
-clock = spcm.Clock(card) # (or) trigger = spcm.Trigger(card) # (or) multi_io =
+string as shown in the Control Center. ## Units and quantities `spcm` uses
+[pint](https://pint.readthedocs.io/en/stable/) to handle all quantities that
+have a physical unit. To enable the use of qunatities simply import the units
+module from `spcm`: ```python from spcm import units ``` This import the
+`units` object from `spcm`. which is a `UnitRegistry` object from `pint`.
+Defining a quantity is as simples as: ```python from spcm import units
+frequency = 100 * units.MHz amplitude = 1 * units.V # etc... ``` All methods
+within the `spcm` that expect a value that is related to a physical quantity
+support the quantities, for example setting a timeout: ```python card.timeout(5
+* units.s) ``` See our dedicated examples for more information about where
+units can be used. ## Card Functionality After opening a card, StarHub or group
+of card, specific functionality of the cards can be accessed through
+`CardFunctionality` classes. | Name | Description | |---------------------|----
+-----------------------------------------------------------------| | `Channels`
+| class for setting up the in- or output stage of the channels of a card | |
+`Clock` | class for setting up the clock engine of the card | | `Trigger` |
+class for setting up the trigger engine of the card | | `MultiPurposeIOs` |
+class for setting up the multi purpose i/o of the card | | `DataTransfer` |
+class for handling data transfer functionality | | `Multi` | class for handling
+multiple recording and replay mode functionality | | `Sequence` | class for
+handling sequence mode functionality | | `TimeStamp` | class for handling time
+stamped data | | `Boxcar` | class for handling boxcar averaging | |
+`BlockAverage` | class for handling block averaging functionality | |
+`PulseGenerators` | class for setting up the pulse generator functionality | |
+`DDS` | class for handling DDS functionality | To use a specific functionality
+simply initiate an instance of one of the classes and pass a device object:
+```python import spcm with spcm.Card('/dev/spcm0') as card: clock = spcm.Clock
+(card) # (or) trigger = spcm.Trigger(card) # (or) multi_io =
 spcm.MultiPurposeIOs(card) # (or) data_transfer = spcm.DataTransfer(card) # etc
 ... ``` Each of these functionalities typically corresponds to a chapter in
 your device manual, so for further reference please have a look in the device
-manual. ## Setting up the Clock engine The Clock engine is used to generate a
-clock signal that is used as the source for all timing critical processes on
-the card. ### Sample rate To get the maximum sample rate of the active card and
-set the sample rate to the maximum, this is an example using internal PLL clock
-mode: ```python clock = spcm.Clock(card) clock.mode(spcm.SPC_CM_INTPLL)
-sample_rate = clock.sample_rate(max=True) # (or) sample_rate =
-clock.sample_rate(20e6) # for a 20 MHz sample rate (see reference manual for
-allowed values) print("Current sample rate: {}S/s".format(sample_rate)) ``` ##
-Setting up the Trigger engine ### External trigger The Trigger engine can be
-configured for a multitude of different configurations (see the hardware manual
-for more information about the specific configurations for your device). Here
-we've given an example for an external trigger arriving at input port ext0,
-that is DC-coupled. The card is waiting for positiv edge that excedes 1.5 V:
-```python trigger = spcm.Trigger(card) trigger.or_mask(spcm.SPC_TMASK_EXT0) #
-set the ext0 hardware input as trigger source trigger.ext0_mode
-(spcm.SPC_TM_POS) # wait for a positive edge trigger.ext0_level0(1500) #
-Trigger level is 1.5 V (1500 mV) trigger.ext0_coupling(spcm.COUPLING_DC) # set
-DC coupling ``` ## Setting up the multi-purpose I/O lines See the hardware
+manual. ## Setting up Channels The Channels functionality allows the user to
+setup individual channels on a Card or a CardStack. The channels object is also
+a Python iterator, hence if a channels object is used it a for-loop, each
+iteration provides a Channel object: ```python channels = spcm.Channels(card,
+card_enable=spcm.CHANNEL0 | CHANNEL1) for channel in channels: # do something
+with each channel ``` In addition, the user can define the output load
+connected to the channel (standard value 50 Ohm), to any resistor value or high
+impedance (`units.highZ`). With this output load, the amplitude setting can be
+done with the repect to this output load: ```python channels = Channels(card,
+card_enable=spcm.CHANNEL0 | CHANNEL1) channels[0].output_load(units.highZ)
+channels[0].amp(1 * units.V) # or for all channels channels.output_load
+(units.highZ) channels.amp(1 * units.V) ``` This information allows the user to
+convert the data coming from `DataTransfer`, using the `convert_data()` method.
+See the section "Setting up a data transfer buffer ..." for more details. ##
+Setting up the Clock engine The Clock engine is used to generate a clock signal
+that is used as the source for all timing critical processes on the card. ###
+Sample rate To get the maximum sample rate of the active card and set the
+sample rate to the maximum, this is an example using internal PLL clock mode:
+```python clock = spcm.Clock(card) clock.mode(spcm.SPC_CM_INTPLL) sample_rate =
+clock.sample_rate(max=True) # (or) sample_rate = clock.sample_rate(20 *
+units.MHz) # for a 20 MHz sample rate (see reference manual for allowed values)
+print("Current sample rate: {}".format(sample_rate, return_unit=units.MS/
+units.s)) ``` ## Setting up the Trigger engine ### External trigger The Trigger
+engine can be configured for a multitude of different configurations (see the
+hardware manual for more information about the specific configurations for your
+device). Here we've given an example for an external trigger arriving at input
+port ext0, that is DC-coupled. The card is waiting for positiv edge that
+excedes 1.5 V: ```python trigger = spcm.Trigger(card) trigger.or_mask
+(spcm.SPC_TMASK_EXT0) # set the ext0 hardware input as trigger source
+trigger.ext0_mode(spcm.SPC_TM_POS) # wait for a positive edge
+trigger.ext0_level0(1.5 * units.V) trigger.ext0_coupling(spcm.COUPLING_DC) #
+set DC coupling ``` ## Setting up the multi-purpose I/O lines See the hardware
 manual, for the multi-purpose I/O lines functionality that can be programmed.
 ## Setting up a data transfer buffer for recording (digitizer) or replay (AWG)
 ### Recording (Digitizing) To transfer data to or from the card, we have to
 setup a data transfer object. This object allocates an amount the memory of the
 card (`memory_size`) and a Direct Memory Access (DMA) buffer on the host pc
 (`allocate_buffer`). Half of the samples are taken before the trigger, as
 configured by the trigger engine, and half of the samples are recorded
 afterwards. Then the transfer from the card to the host pc is started and the
 program waits until the DMA is filled. ```python # define the data buffer
+num_samples = 4 * units.KiS # 1 KiS = 1 KibiSamples = 1024 Samples
 data_transfer = spcm.DataTransfer(card) data_transfer.memory_size(num_samples)
 data_transfer.allocate_buffer(num_samples) data_transfer.post_trigger
 (num_samples // 2) # Start DMA transfer data_transfer.start_buffer_transfer
 (spcm.M2CMD_DATA_STARTDMA) # start card and wait until the memory is filled
 card.start(spcm.M2CMD_CARD_ENABLETRIGGER, spcm.M2CMD_DATA_WAITDMA) # (your code
 handling the recorded data comes here) ``` To access the recorded data, the
 data transfer object holds a [NumPy](https://numpy.org/) array object
@@ -161,25 +177,42 @@
 axis=1) ``` This data can be further processed or plotted using, for example,
 [`matplotlib`](https://matplotlib.org/). ### Replay (Generation) The setup of
 the DMA for replay is very similar. First card memory is allocated with
 `memory_size` and then a DMA buffer is allocated (`allocated_buffer`) and made
 accessible though the NumPy object `data_transfer.buffer`, which can then be
 written to using standard NumPy methods. Finally, data transfer from the host
 PC to the card is started and the programming is waiting until all the data is
-transferred: ```python data_transfer = spcm.DataTransfer(card)
-data_transfer.memory_size(num_samples) data_transfer.allocate_buffer
-(num_samples) data_transfer.loops(0) # loop continuously # simple linear ramp
-for analog output cards data_transfer.buffer[:] = np.arange(-num_samples//2,
-num_samples//2).astype(np.int16) data_transfer.start_buffer_transfer
-(spcm.M2CMD_DATA_STARTDMA, spcm.M2CMD_DATA_WAITDMA) ``` ## Multiple recording /
-replay In case of multiple recording / replay, the memory is divided in equally
-sized segments, that are populated / replayed when a trigger is detected.
-Multiple triggers each trigger the next segment to be populated or replayed.
-The following code snippet shows how to setup the buffer for 4 segments with
-each 128 Samples: ```python samples_per_segment = 128 num_segments = 4
+transferred: ```python num_samples = 4 * units.KiS # 1 KiS = 1 KibiSamples =
+1024 Samples data_transfer = spcm.DataTransfer(card) data_transfer.memory_size
+(num_samples) data_transfer.allocate_buffer(num_samples) data_transfer.loops(0)
+# loop continuously # simple linear ramp for analog output cards
+num_samples_magnitude = num_samples.to(units.S).magnitude data_transfer.buffer
+[:] = np.arange(-num_samples_magnitude//2, num_samples_magnitude//2).astype
+(np.int16) data_transfer.start_buffer_transfer(spcm.M2CMD_DATA_STARTDMA,
+spcm.M2CMD_DATA_WAITDMA) ``` #### Data transfer In the above it's assume that
+all the data has been transferred from the card into the buffer object, however
+if you're working in FIFO mode or you've defined the buffer to be smaller then
+the assigned card memory size, then the card will write to parts of the memory
+and tell you were it wrote. This can be either handled manually (see the
+reference manual of your card, or the methods `avail_card_len()`,
+`avail_user_pos()` and `avail_user_len()`). Secondly, it can also be handled
+with Python iterators functionality. If the `data_transfer` object is handed to
+a for-loop, then in each iteration a view of the current active memory part is
+given in the form of a NumPy array and the user can do calculations on that.
+```python # Get a block of data for data_block in data_transfer: # data_block
+is a NumPy array view of the currently active buffer part for channel in
+channels: data_units = channel.convert_data(data_block[:, channel]) minimum =
+np.min(data_units) maximum = np.max(data_units) print(f"Minimum: {minimum} -
+maximum: {maximum}") ``` The same principle also works with generator cards
+(see the example `2_gen_fifo.py`). ## Multiple recording / replay In case of
+multiple recording / replay, the memory is divided in equally sized segments,
+that are populated / replayed when a trigger is detected. Multiple triggers
+each trigger the next segment to be populated or replayed. The following code
+snippet shows how to setup the buffer for 4 segments with each 128 Samples:
+```python samples_per_segment = 128 * units.S num_segments = 4
 multiple_recording = spcm.Multi(card) multiple_recording.memory_size
 (samples_per_segment*num_segments) multiple_recording.allocate_buffer
 (segment_samples=samples_per_segment, num_segments=num_segments)
 multiple_recording.post_trigger(samples_per_segment // 2)
 multiple_recording.start_buffer_transfer(spcm.M2CMD_DATA_STARTDMA) ``` Again
 there are half the samples before and half the samples after the trigger. ##
 Timestamps See the example `6_acq_fifo_multi_ts_poll.py` in the examples folder
@@ -194,30 +227,30 @@
 is a simple example for setting up a single pulse generator on x0. Create a
 pulse generators object and get the clock rate used by the pulse generator. Use
 that to calculate the period of a 1 MHz signal and the half of that period
 we'll have a high signal (hence 50% duty cycle). The pulse generator will start
 if the trigger condition is met without delay and loops infinitely many times.
 The triggering condition is set to the card software trigger. See more details
 in the pulse generator chapter in the specific hardware manual. ```python
-pulse_generators = spcm.PulseGenerators(card) # get the clock of the card
-pulse_gen_clock_Hz = pulse_generators.get_clock() # generate a continuous
-signal with 1 MHz len_for_1MHz = pulse_gen_clock_Hz // spcm.MEGA(1)
-pulse_generators[0].mode(spcm.SPCM_PULSEGEN_MODE_TRIGGERED) pulse_generators
-[0].period_length(len_for_1MHz) pulse_generators[0].high_length(len_for_1MHz /
-/ 2) # 50% HIGH, 50% LOW pulse_generators[0].delay(0) pulse_generators
-[0].num_loops(0) # 0: infinite pulse_generators[0].mux1
-(spcm.SPCM_PULSEGEN_MUX1_SRC_UNUSED) pulse_generators[0].mux2
-(spcm.SPCM_PULSEGEN_MUX2_SRC_SOFTWARE) # started by software force command #
-and write the pulse generator settings pulse_generators.write_setup() # start
-all pulse generators that wait for a software command pulse_generators.force()
-``` This will start the pulse generator to continuously output a 1 MHz signal.
-### Sequence replay mode (AWG only) Please see the example `3_gen_sequence.py`
-in the folder `2_generation` of the examples to see an example dedicated to the
-Sequence replay mode. ### DDS (AWG only) Please see the examples in the
-dedicated examples folder `3_dds` for all the functionality provided by the DDS
+pulse_generators = spcm.PulseGenerators(card) # generate a continuous signal
+with 1 MHz pulse_generators[0].pulse_period(1 * units.us) # pulse_generators
+[0].repetition_rate(1 * units.MHz) # (or) pulse_generators[0].duty_cycle(50 *
+units.percent) # pulse_generators[0].pulse_length(0.5 * units.us) # (or)
+pulse_generators[0].start_delay(0 * units.us) pulse_generators[0].repetitions
+(0) # 0: infinite pulse_generators[0].start_condition_state_signal
+(spcm.SPCM_PULSEGEN_MUX1_SRC_UNUSED) pulse_generators
+[0].start_condition_trigger_signal(spcm.SPCM_PULSEGEN_MUX2_SRC_SOFTWARE)
+pulse_generators[0].invert_start_condition(False) # and write the pulse
+generator settings pulse_generators.write_setup() # start all pulse generators
+that wait for a software command pulse_generators.force() ``` This will start
+the pulse generator to continuously output a 1 MHz signal. ### Sequence replay
+mode (AWG only) Please see the example `3_gen_sequence.py` in the folder
+`2_generation` of the examples to see an example dedicated to the Sequence
+replay mode. ### DDS (AWG only) Please see the examples in the dedicated
+examples folder `3_dds` for all the functionality provided by the DDS
 framework. Moreover, please also have a look at the corresponding hardware
 manual. ### Boxcar (Digitizer only) See the corresponding chapter in the
 hardware manual for more information about boxcar averaging and the registers
 used. ### Block average (Digitizer only) See the corresponding chapter in the
 hardware manual for more information about block averaging and the registers
 used. # Acknowledgements We would like to thank [Christian Baker](https://
 github.com/crnbaker) for fruitful discussions and inspiration on how to setup
```

### Comparing `spcm-1.0.6/README.md` & `spcm-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,38 @@
+Metadata-Version: 2.1
+Name: spcm
+Version: 1.1.0
+Summary: Package for Spectrum Instrumentation GmbH cards
+Author-email: Spectrum Instrumentation GmbH <info@spec.de>
+Project-URL: Homepage, https://spectrum-instrumentation.com/
+Project-URL: API, https://spectruminstrumentation.github.io/spcm/spcm.html
+Project-URL: Repository, https://github.com/SpectrumInstrumentation/spcm
+Project-URL: Examples, https://github.com/SpectrumInstrumentation/spcm/tree/master/src/examples
+Project-URL: Knowledge Base, https://spectrum-instrumentation.com/support/knowledgebase/index.php
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: System :: Hardware
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>=1.25.2
+Requires-Dist: h5py>=3.10.0
+Requires-Dist: pint>=0.23
+
 <div style="margin-bottom: 20px; text-align: center">
 <a href="https://spectrum-instrumentation.com">
     <img src="https://spectrum-instrumentation.com/img/logo-complete.png"  width=400 />
 </a>
 </div>
 
 # spcm
@@ -18,33 +49,37 @@
 # Supported devices
 
 See the [SUPPORTED_DEVICES.md](https://github.com/SpectrumInstrumentation/spcm/blob/master/src/spcm/SUPPORTED_DEVICES.md) file for a list of supported devices.
 
 # Requirements
 [![Python](https://img.shields.io/pypi/pyversions/spcm.svg)](https://badge.fury.io/py/spcm)
 [![Static Badge](https://img.shields.io/badge/NumPy-1.25-green)](https://numpy.org/)
+[![Static Badge](https://img.shields.io/badge/h5py-3.10-orange)](https://www.h5py.org/)
 
 `spcm` requires the Spectrum Instrumentation [driver](https://spectrum-instrumentation.com/support/downloads.php) which is available for Windows and Linux. 
 Please have a look in the manual of your product for more information about installing the driver on the different plattforms.
 
 # Installation and dependencies
 [![Pip Package](https://img.shields.io/pypi/v/spcm?logo=PyPI)](https://pypi.org/project/spcm)
+[![Publish to PyPI](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/spcm-publish-to-pypi.yml/badge.svg)](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/spcm-publish-to-pypi.yml)
 
 Start by installing Python 3.9 or higher. We recommend using the latest version. You can download Python from [https://www.python.org/](https://www.python.org/).
 
 You would probably also like to install and use a virtual environment, although it's not strictly necessary. See the examples [README.md](https://github.com/SpectrumInstrumentation/spcm/blob/master/src/examples/README.md) for a more detailed explanation on how to use `spcm` in a virtual environment.
 
 To install the latest release using `pip`:
 ```bash
 $ pip install spcm
 ```
-Note that: this will automatically install all the dependencies (e.g. NumPy).
+Note that: this will automatically install all the dependencies.
 
 # Documentation
 [![Documentation](https://img.shields.io/badge/api-reference-blue.svg)](https://spectruminstrumentation.github.io/spcm/spcm.html)
+[![Build dosc](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/spcm-docs-pages.yml/badge.svg)](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/spcm-docs-pages.yml)
+[![Publish docs](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/pages/pages-build-deployment)
 
 The API documentation for the latest [stable release](https://spectruminstrumentation.github.io/spcm/spcm.html) is available for reading on GitHub pages.
 
 Please also see the hardware user manuals for your specific card for more information about the provided functionality.
 
 # Using spcm
 
@@ -129,14 +164,40 @@
 See the register `SPC_PCISERIALNO` in the reference manual of your specific device for more information.
 
 If the `device_identifier` is given that card is opened, if at the same time `card_type` or `serial_number` are given then these behave as an additional check too see if the opened card is of a certain type or has that specific serial number.
 
 ### Demo devices
 To test the Spectrum Instrumentation API with user code without hardware, the Control Center gives the user the option to create [demo devices](https://spectrum-instrumentation.com/support/knowledgebase/software/How_to_set_up_a_demo_card.php). These demo devices can be used in the same manner as real devices. Simply change the device identifier string to the string as shown in the Control Center.
 
+## Units and quantities
+
+`spcm` uses [pint](https://pint.readthedocs.io/en/stable/) to handle all quantities that have a physical unit. To enable the use of qunatities simply import the units module from `spcm`:
+
+```python
+from spcm import units
+```
+
+This import the `units` object from `spcm`. which is a `UnitRegistry` object from  `pint`. Defining a quantity is as simples as:
+
+```python
+from spcm import units
+
+frequency = 100 * units.MHz
+amplitude = 1 * units.V
+# etc...
+```
+
+All methods within the `spcm` that expect a value that is related to a physical quantity support the quantities, for example setting a timeout:
+
+```python
+card.timeout(5 * units.s)
+```
+
+See our dedicated examples for more information about where units can be used.
+
 ## Card Functionality
 After opening a card, StarHub or group of card, specific functionality of the cards can be accessed through `CardFunctionality` classes. 
 
 | Name                | Description                                                         |
 |---------------------|---------------------------------------------------------------------|
 | `Channels`          | class for setting up the in- or output stage of the channels of a card |
 | `Clock`             | class for setting up the clock engine of the card                   |
@@ -166,52 +227,78 @@
     # (or)
     data_transfer = spcm.DataTransfer(card)
     # etc ...
 
 ```
 Each of these functionalities typically corresponds to a chapter in your device manual, so for further reference please have a look in the device manual.
 
+## Setting up Channels
+
+The Channels functionality allows the user to setup individual channels on a Card or a CardStack. The channels object is also a Python iterator, hence if a channels object is used it a for-loop, each iteration provides a Channel object:
+
+```python
+channels = spcm.Channels(card, card_enable=spcm.CHANNEL0 | CHANNEL1)
+for channel in channels:
+    # do something with each channel
+```
+
+In addition, the user can define the output load connected to the channel (standard value 50 Ohm), to any resistor value or high impedance (`units.highZ`). With this output load, the amplitude setting can be done with the repect to this output load:
+
+```python
+channels = Channels(card, card_enable=spcm.CHANNEL0 | CHANNEL1)
+channels[0].output_load(units.highZ)
+channels[0].amp(1 * units.V)
+# or for all channels
+channels.output_load(units.highZ)
+channels.amp(1 * units.V)
+```
+
+This information allows the user to convert the data coming from `DataTransfer`, using the `convert_data()` method. See the section "Setting up a data transfer buffer ..." for more details.
+
 ## Setting up the Clock engine
 
 The Clock engine is used to generate a clock signal that is used as the source for all timing critical processes on the card.
 
 ### Sample rate
 To get the maximum sample rate of the active card and set the sample rate to the maximum, this is an example using internal PLL clock mode:
 ```python
 clock = spcm.Clock(card)
 clock.mode(spcm.SPC_CM_INTPLL)
-sample_rate = clock.sample_rate(max=True) # (or) sample_rate = clock.sample_rate(20e6) # for a 20 MHz sample rate (see reference manual for allowed values)
-print("Current sample rate: {}S/s".format(sample_rate))
+sample_rate = clock.sample_rate(max=True) 
+# (or) 
+sample_rate = clock.sample_rate(20 * units.MHz) # for a 20 MHz sample rate (see reference manual for allowed values)
+print("Current sample rate: {}".format(sample_rate, return_unit=units.MS/units.s))
 ```
 
 ## Setting up the Trigger engine
 
 ### External trigger
 
 The Trigger engine can be configured for a multitude of different configurations (see the hardware manual for more information about the specific configurations for your device). Here we've given an example for an external trigger arriving at input port ext0, that is DC-coupled. The card is waiting for positiv edge that excedes 1.5 V:
 
 ```python
 trigger = spcm.Trigger(card)
 trigger.or_mask(spcm.SPC_TMASK_EXT0) # set the ext0 hardware input as trigger source
 trigger.ext0_mode(spcm.SPC_TM_POS) # wait for a positive edge
-trigger.ext0_level0(1500) # Trigger level is 1.5 V (1500 mV)
+trigger.ext0_level0(1.5 * units.V)
 trigger.ext0_coupling(spcm.COUPLING_DC) # set DC coupling
 ```
 
 ## Setting up the multi-purpose I/O lines
 
 See the hardware manual, for the multi-purpose I/O lines functionality that can be programmed.
 
 ## Setting up a data transfer buffer for recording (digitizer) or replay (AWG)
 
 ### Recording (Digitizing)
 To transfer data to or from the card, we have to setup a data transfer object. This object allocates an amount the memory of the card (`memory_size`) and a Direct Memory Access (DMA) buffer on the host pc (`allocate_buffer`). Half of the samples are taken before the trigger, as configured by the trigger engine, and half of the samples are recorded afterwards. Then the transfer from the card to the host pc is started and the program waits until the DMA is filled.
 
 ```python
 # define the data buffer
+num_samples = 4 * units.KiS # 1 KiS = 1 KibiSamples = 1024 Samples
 data_transfer = spcm.DataTransfer(card)
 data_transfer.memory_size(num_samples)
 data_transfer.allocate_buffer(num_samples)
 data_transfer.post_trigger(num_samples // 2)
 # Start DMA transfer
 data_transfer.start_buffer_transfer(spcm.M2CMD_DATA_STARTDMA)
 
@@ -233,32 +320,55 @@
 
 This data can be further processed or plotted using, for example, [`matplotlib`](https://matplotlib.org/).
 
 ### Replay (Generation)
 
 The setup of the DMA for replay is very similar. First card memory is allocated with `memory_size` and then a DMA buffer is allocated (`allocated_buffer`) and made accessible though the NumPy object `data_transfer.buffer`, which can then be written to using standard NumPy methods. Finally, data transfer from the host PC to the card is started and the programming is waiting until all the data is transferred:
 ```python
+num_samples = 4 * units.KiS # 1 KiS = 1 KibiSamples = 1024 Samples
 data_transfer = spcm.DataTransfer(card)
 data_transfer.memory_size(num_samples)
 data_transfer.allocate_buffer(num_samples)
 data_transfer.loops(0) # loop continuously
 # simple linear ramp for analog output cards
-data_transfer.buffer[:] = np.arange(-num_samples//2, num_samples//2).astype(np.int16)
+num_samples_magnitude = num_samples.to(units.S).magnitude
+data_transfer.buffer[:] = np.arange(-num_samples_magnitude//2, num_samples_magnitude//2).astype(np.int16)
 
 data_transfer.start_buffer_transfer(spcm.M2CMD_DATA_STARTDMA, spcm.M2CMD_DATA_WAITDMA)
 ```
 
+#### Data transfer
+
+In the above it's assume that all the data has been transferred from the card into the buffer object, however if you're working in FIFO mode or you've defined the buffer to be smaller then the assigned card memory size, then the card will write to parts of the memory and tell you were it wrote. 
+
+This can be either handled manually (see the reference manual of your card, or the methods `avail_card_len()`, `avail_user_pos()` and `avail_user_len()`).
+
+Secondly, it can also be handled with Python iterators functionality. If the `data_transfer` object is handed to a for-loop, then in each iteration a view of the current active memory part is given in the form of a NumPy array and the user can do calculations on that.
+
+```python
+# Get a block of data
+for data_block in data_transfer:
+    # data_block is a NumPy array view of the currently active buffer part
+    for channel in channels:
+        data_units = channel.convert_data(data_block[:, channel])
+        minimum = np.min(data_units)
+        maximum = np.max(data_units)
+        print(f"Minimum: {minimum} - maximum: {maximum}")
+```
+
+The same principle also works with generator cards (see the example `2_gen_fifo.py`).
+
 ## Multiple recording / replay
 
 In case of multiple recording / replay, the memory is divided in equally sized segments, that are populated / replayed when a trigger is detected. Multiple triggers each trigger the next segment to be populated or replayed.
 
 The following code snippet shows how to setup the buffer for 4 segments with each 128 Samples:
 
 ```python
-samples_per_segment = 128
+samples_per_segment = 128 * units.S
 num_segments = 4
 multiple_recording = spcm.Multi(card)
 multiple_recording.memory_size(samples_per_segment*num_segments)
 multiple_recording.allocate_buffer(segment_samples=samples_per_segment, num_segments=num_segments)
 multiple_recording.post_trigger(samples_per_segment // 2)
 multiple_recording.start_buffer_transfer(spcm.M2CMD_DATA_STARTDMA)
 ```
@@ -284,26 +394,25 @@
 
 Please see the folder `4_pulse-generator` in the `examples` folder for several dedicated examples. In the following, there is a simple example for setting up a single pulse generator on x0.
 
 Create a pulse generators object and get the clock rate used by the pulse generator. Use that to calculate the period of a 1 MHz signal and the half of that period we'll have a high signal (hence 50% duty cycle). The pulse generator will start if the trigger condition is met without delay and loops infinitely many times. The triggering condition is set to the card software trigger. See more details in the pulse generator chapter in the specific hardware manual.
 
 ```python
 pulse_generators = spcm.PulseGenerators(card)
-# get the clock of the card
-pulse_gen_clock_Hz = pulse_generators.get_clock()
 
 # generate a continuous signal with 1 MHz
-len_for_1MHz = pulse_gen_clock_Hz // spcm.MEGA(1)
-pulse_generators[0].mode(spcm.SPCM_PULSEGEN_MODE_TRIGGERED)
-pulse_generators[0].period_length(len_for_1MHz)
-pulse_generators[0].high_length(len_for_1MHz // 2) # 50% HIGH, 50% LOW
-pulse_generators[0].delay(0)
-pulse_generators[0].num_loops(0) # 0: infinite
-pulse_generators[0].mux1(spcm.SPCM_PULSEGEN_MUX1_SRC_UNUSED)
-pulse_generators[0].mux2(spcm.SPCM_PULSEGEN_MUX2_SRC_SOFTWARE) # started by software force command
+pulse_generators[0].pulse_period(1 * units.us)
+# pulse_generators[0].repetition_rate(1 * units.MHz) # (or)
+pulse_generators[0].duty_cycle(50 * units.percent)
+# pulse_generators[0].pulse_length(0.5 * units.us) # (or)
+pulse_generators[0].start_delay(0 * units.us)
+pulse_generators[0].repetitions(0) # 0: infinite
+pulse_generators[0].start_condition_state_signal(spcm.SPCM_PULSEGEN_MUX1_SRC_UNUSED)
+pulse_generators[0].start_condition_trigger_signal(spcm.SPCM_PULSEGEN_MUX2_SRC_SOFTWARE)
+pulse_generators[0].invert_start_condition(False)
 
 # and write the pulse generator settings
 pulse_generators.write_setup()
 
 # start all pulse generators that wait for a software command
 pulse_generators.force()
 ```
@@ -324,8 +433,8 @@
 
 ### Block average (Digitizer only)
 
 See the corresponding chapter in the hardware manual for more information about block averaging and the registers used.
 
 # Acknowledgements
 
-We would like to thank [Christian Baker](https://github.com/crnbaker) for fruitful discussions and inspiration on how to setup the `spcm` package.
+We would like to thank [Christian Baker](https://github.com/crnbaker) for fruitful discussions and inspiration on how to setup the `spcm` package.
```

#### html2text {}

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1 Name: spcm Version: 1.1.0 Summary: Package for Spectrum
+Instrumentation GmbH cards Author-email: Spectrum Instrumentation GmbH
+spec.de> Project-URL: Homepage, https://spectrum-instrumentation.com/ Project-
+URL: API, https://spectruminstrumentation.github.io/spcm/spcm.html Project-URL:
+Repository, https://github.com/SpectrumInstrumentation/spcm Project-URL:
+Examples, https://github.com/SpectrumInstrumentation/spcm/tree/master/src/
+examples Project-URL: Knowledge Base, https://spectrum-instrumentation.com/
+support/knowledgebase/index.php Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
+Natural Language :: English Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows Classifier: Programming
+Language :: Python Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering Classifier: Topic :: System ::
+Hardware Requires-Python: >=3.9 Description-Content-Type: text/markdown
+License-File: LICENSE Requires-Dist: numpy>=1.25.2 Requires-Dist: h5py>=3.10.0
+Requires-Dist: pint>=0.23
 _[_h_t_t_p_s_:_/_/_s_p_e_c_t_r_u_m_-_i_n_s_t_r_u_m_e_n_t_a_t_i_o_n_._c_o_m_/_i_m_g_/_l_o_g_o_-_c_o_m_p_l_e_t_e_._p_n_g_]
 # spcm [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)]
 (https://opensource.org/licenses/MIT) [![PyPI - Version](https://
 img.shields.io/pypi/v/spcm)](https://pypi.org/project/spcm) [![PyPi Downloads]
 (https://img.shields.io/pypi/dm/spcm?label=downloads%20%7C%20pip&logo=PyPI)]
 (https://pypi.org/project/spcm) [![Follow](https://img.shields.io/twitter/
 follow/
@@ -11,58 +30,67 @@
 oriented Python package for interfacing with Spectrum Instrumentation GmbH
 devices. `spcm` can handle individual cards (`Card`), StarHubs (`Sync`), groups
 of cards (`CardStack`) and Netboxes (`Netbox`). # Supported devices See the
 [SUPPORTED_DEVICES.md](https://github.com/SpectrumInstrumentation/spcm/blob/
 master/src/spcm/SUPPORTED_DEVICES.md) file for a list of supported devices. #
 Requirements [![Python](https://img.shields.io/pypi/pyversions/spcm.svg)]
 (https://badge.fury.io/py/spcm) [![Static Badge](https://img.shields.io/badge/
-NumPy-1.25-green)](https://numpy.org/) `spcm` requires the Spectrum
+NumPy-1.25-green)](https://numpy.org/) [![Static Badge](https://img.shields.io/
+badge/h5py-3.10-orange)](https://www.h5py.org/) `spcm` requires the Spectrum
 Instrumentation [driver](https://spectrum-instrumentation.com/support/
 downloads.php) which is available for Windows and Linux. Please have a look in
 the manual of your product for more information about installing the driver on
 the different plattforms. # Installation and dependencies [![Pip Package]
 (https://img.shields.io/pypi/v/spcm?logo=PyPI)](https://pypi.org/project/spcm)
-Start by installing Python 3.9 or higher. We recommend using the latest
-version. You can download Python from [https://www.python.org/](https://
-www.python.org/). You would probably also like to install and use a virtual
-environment, although it's not strictly necessary. See the examples [README.md]
-(https://github.com/SpectrumInstrumentation/spcm/blob/master/src/examples/
-README.md) for a more detailed explanation on how to use `spcm` in a virtual
-environment. To install the latest release using `pip`: ```bash $ pip install
-spcm ``` Note that: this will automatically install all the dependencies (e.g.
-NumPy). # Documentation [![Documentation](https://img.shields.io/badge/api-
-reference-blue.svg)](https://spectruminstrumentation.github.io/spcm/spcm.html)
-The API documentation for the latest [stable release](https://
-spectruminstrumentation.github.io/spcm/spcm.html) is available for reading on
-GitHub pages. Please also see the hardware user manuals for your specific card
-for more information about the provided functionality. # Using spcm The `spcm`
-package is a high-level object-oriented programming library for controlling
-Spectrum Instrumentation devices. ## Examples For detailed examples see the
-`src\examples` directory. There are several sub-directories each corresponding
-to a certain kind of functionality. See also the examples on [GitHub](https://
-github.com/SpectrumInstrumentation/spcm/tree/master/src/examples). ## Hardware
-interfaces `spcm` provides the following classes for interfacing with the
-different devices. | Name | Description | |-------------|----------------------
--------------------------------------------------------------| | `Card` | a
-class to control the low-level API of Spectrum Instrumentation cards. | |
-`Sync` | a class for controling StarHub devices. | | `CardStack` | a class that
-handles the opening and closing of a combination of different cards either with
-or without a StarHub that synchronizes the cards. | | `Netbox` | a class that
-handles the opening and closing of the cards in a Netbox | ## Connect to a
-device Opening and closing of cards is handled using the python [`with`](https:
-//peps.python.org/pep-0343/) statement. This creates a context manager that
-safely handles opening and closing of a card or a group of cards. ### Using
-device identifiers Connect to local cards: ```python import spcm with spcm.Card
-('/dev/spcm0') as card: # (add your code here) ``` Connect to remote cards (you
-can find a card's IP using the [Spectrum Control Center](https://spectrum-
-instrumentation.com/en/spectrum-control-center) software): ```python import
-spcm with spcm.Card('TCPIP::192.168.1.10::inst0::INSTR') as card: # (add your
-code here) ``` Connect to a group of cards synchronized using a StarHub:
-```python import spcm card_identifiers = ["/dev/spcm0", "/dev/spcm1"]
-sync_identifier = "sync0" with spcm.CardStack
+[![Publish to PyPI](https://github.com/SpectrumInstrumentation/spcm/actions/
+workflows/spcm-publish-to-pypi.yml/badge.svg)](https://github.com/
+SpectrumInstrumentation/spcm/actions/workflows/spcm-publish-to-pypi.yml) Start
+by installing Python 3.9 or higher. We recommend using the latest version. You
+can download Python from [https://www.python.org/](https://www.python.org/).
+You would probably also like to install and use a virtual environment, although
+it's not strictly necessary. See the examples [README.md](https://github.com/
+SpectrumInstrumentation/spcm/blob/master/src/examples/README.md) for a more
+detailed explanation on how to use `spcm` in a virtual environment. To install
+the latest release using `pip`: ```bash $ pip install spcm ``` Note that: this
+will automatically install all the dependencies. # Documentation [!
+[Documentation](https://img.shields.io/badge/api-reference-blue.svg)](https://
+spectruminstrumentation.github.io/spcm/spcm.html) [![Build dosc](https://
+github.com/SpectrumInstrumentation/spcm/actions/workflows/spcm-docs-pages.yml/
+badge.svg)](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/
+spcm-docs-pages.yml) [![Publish docs](https://github.com/
+SpectrumInstrumentation/spcm/actions/workflows/pages/pages-build-deployment/
+badge.svg)](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/
+pages/pages-build-deployment) The API documentation for the latest [stable
+release](https://spectruminstrumentation.github.io/spcm/spcm.html) is available
+for reading on GitHub pages. Please also see the hardware user manuals for your
+specific card for more information about the provided functionality. # Using
+spcm The `spcm` package is a high-level object-oriented programming library for
+controlling Spectrum Instrumentation devices. ## Examples For detailed examples
+see the `src\examples` directory. There are several sub-directories each
+corresponding to a certain kind of functionality. See also the examples on
+[GitHub](https://github.com/SpectrumInstrumentation/spcm/tree/master/src/
+examples). ## Hardware interfaces `spcm` provides the following classes for
+interfacing with the different devices. | Name | Description | |-------------|-
+-------------------------------------------------------------------------------
+---| | `Card` | a class to control the low-level API of Spectrum
+Instrumentation cards. | | `Sync` | a class for controling StarHub devices. | |
+`CardStack` | a class that handles the opening and closing of a combination of
+different cards either with or without a StarHub that synchronizes the cards. |
+| `Netbox` | a class that handles the opening and closing of the cards in a
+Netbox | ## Connect to a device Opening and closing of cards is handled using
+the python [`with`](https://peps.python.org/pep-0343/) statement. This creates
+a context manager that safely handles opening and closing of a card or a group
+of cards. ### Using device identifiers Connect to local cards: ```python import
+spcm with spcm.Card('/dev/spcm0') as card: # (add your code here) ``` Connect
+to remote cards (you can find a card's IP using the [Spectrum Control Center]
+(https://spectrum-instrumentation.com/en/spectrum-control-center) software):
+```python import spcm with spcm.Card('TCPIP::192.168.1.10::inst0::INSTR') as
+card: # (add your code here) ``` Connect to a group of cards synchronized using
+a StarHub: ```python import spcm card_identifiers = ["/dev/spcm0", "/dev/
+spcm1"] sync_identifier = "sync0" with spcm.CardStack
 (card_identifiers=card_identifiers, sync_identifier=sync_identifier) as stack:
 # (add your code here) ``` The `CardStack` object contains a list of `Card`
 objects in the `stack.cards` parameter and a `Sync` object in the parameter
 `stack.sync`. ### Using card type or serial number Apart from connecting to a
 device directly through a device identifier it's also possible to connect to
 local devices using the card type or serial number. To find the first card of
 type analog out (`SPCM_TYPE_AO`) you can do the following: ```python import
@@ -77,62 +105,87 @@
 given then these behave as an additional check too see if the opened card is of
 a certain type or has that specific serial number. ### Demo devices To test the
 Spectrum Instrumentation API with user code without hardware, the Control
 Center gives the user the option to create [demo devices](https://spectrum-
 instrumentation.com/support/knowledgebase/software/
 How_to_set_up_a_demo_card.php). These demo devices can be used in the same
 manner as real devices. Simply change the device identifier string to the
-string as shown in the Control Center. ## Card Functionality After opening a
-card, StarHub or group of card, specific functionality of the cards can be
-accessed through `CardFunctionality` classes. | Name | Description | |---------
-------------|------------------------------------------------------------------
----| | `Channels` | class for setting up the in- or output stage of the
-channels of a card | | `Clock` | class for setting up the clock engine of the
-card | | `Trigger` | class for setting up the trigger engine of the card | |
-`MultiPurposeIOs` | class for setting up the multi purpose i/o of the card | |
-`DataTransfer` | class for handling data transfer functionality | | `Multi` |
-class for handling multiple recording and replay mode functionality | |
-`Sequence` | class for handling sequence mode functionality | | `TimeStamp` |
-class for handling time stamped data | | `Boxcar` | class for handling boxcar
-averaging | | `BlockAverage` | class for handling block averaging functionality
-| | `PulseGenerators` | class for setting up the pulse generator functionality
-| | `DDS` | class for handling DDS functionality | To use a specific
-functionality simply initiate an instance of one of the classes and pass a
-device object: ```python import spcm with spcm.Card('/dev/spcm0') as card:
-clock = spcm.Clock(card) # (or) trigger = spcm.Trigger(card) # (or) multi_io =
+string as shown in the Control Center. ## Units and quantities `spcm` uses
+[pint](https://pint.readthedocs.io/en/stable/) to handle all quantities that
+have a physical unit. To enable the use of qunatities simply import the units
+module from `spcm`: ```python from spcm import units ``` This import the
+`units` object from `spcm`. which is a `UnitRegistry` object from `pint`.
+Defining a quantity is as simples as: ```python from spcm import units
+frequency = 100 * units.MHz amplitude = 1 * units.V # etc... ``` All methods
+within the `spcm` that expect a value that is related to a physical quantity
+support the quantities, for example setting a timeout: ```python card.timeout(5
+* units.s) ``` See our dedicated examples for more information about where
+units can be used. ## Card Functionality After opening a card, StarHub or group
+of card, specific functionality of the cards can be accessed through
+`CardFunctionality` classes. | Name | Description | |---------------------|----
+-----------------------------------------------------------------| | `Channels`
+| class for setting up the in- or output stage of the channels of a card | |
+`Clock` | class for setting up the clock engine of the card | | `Trigger` |
+class for setting up the trigger engine of the card | | `MultiPurposeIOs` |
+class for setting up the multi purpose i/o of the card | | `DataTransfer` |
+class for handling data transfer functionality | | `Multi` | class for handling
+multiple recording and replay mode functionality | | `Sequence` | class for
+handling sequence mode functionality | | `TimeStamp` | class for handling time
+stamped data | | `Boxcar` | class for handling boxcar averaging | |
+`BlockAverage` | class for handling block averaging functionality | |
+`PulseGenerators` | class for setting up the pulse generator functionality | |
+`DDS` | class for handling DDS functionality | To use a specific functionality
+simply initiate an instance of one of the classes and pass a device object:
+```python import spcm with spcm.Card('/dev/spcm0') as card: clock = spcm.Clock
+(card) # (or) trigger = spcm.Trigger(card) # (or) multi_io =
 spcm.MultiPurposeIOs(card) # (or) data_transfer = spcm.DataTransfer(card) # etc
 ... ``` Each of these functionalities typically corresponds to a chapter in
 your device manual, so for further reference please have a look in the device
-manual. ## Setting up the Clock engine The Clock engine is used to generate a
-clock signal that is used as the source for all timing critical processes on
-the card. ### Sample rate To get the maximum sample rate of the active card and
-set the sample rate to the maximum, this is an example using internal PLL clock
-mode: ```python clock = spcm.Clock(card) clock.mode(spcm.SPC_CM_INTPLL)
-sample_rate = clock.sample_rate(max=True) # (or) sample_rate =
-clock.sample_rate(20e6) # for a 20 MHz sample rate (see reference manual for
-allowed values) print("Current sample rate: {}S/s".format(sample_rate)) ``` ##
-Setting up the Trigger engine ### External trigger The Trigger engine can be
-configured for a multitude of different configurations (see the hardware manual
-for more information about the specific configurations for your device). Here
-we've given an example for an external trigger arriving at input port ext0,
-that is DC-coupled. The card is waiting for positiv edge that excedes 1.5 V:
-```python trigger = spcm.Trigger(card) trigger.or_mask(spcm.SPC_TMASK_EXT0) #
-set the ext0 hardware input as trigger source trigger.ext0_mode
-(spcm.SPC_TM_POS) # wait for a positive edge trigger.ext0_level0(1500) #
-Trigger level is 1.5 V (1500 mV) trigger.ext0_coupling(spcm.COUPLING_DC) # set
-DC coupling ``` ## Setting up the multi-purpose I/O lines See the hardware
+manual. ## Setting up Channels The Channels functionality allows the user to
+setup individual channels on a Card or a CardStack. The channels object is also
+a Python iterator, hence if a channels object is used it a for-loop, each
+iteration provides a Channel object: ```python channels = spcm.Channels(card,
+card_enable=spcm.CHANNEL0 | CHANNEL1) for channel in channels: # do something
+with each channel ``` In addition, the user can define the output load
+connected to the channel (standard value 50 Ohm), to any resistor value or high
+impedance (`units.highZ`). With this output load, the amplitude setting can be
+done with the repect to this output load: ```python channels = Channels(card,
+card_enable=spcm.CHANNEL0 | CHANNEL1) channels[0].output_load(units.highZ)
+channels[0].amp(1 * units.V) # or for all channels channels.output_load
+(units.highZ) channels.amp(1 * units.V) ``` This information allows the user to
+convert the data coming from `DataTransfer`, using the `convert_data()` method.
+See the section "Setting up a data transfer buffer ..." for more details. ##
+Setting up the Clock engine The Clock engine is used to generate a clock signal
+that is used as the source for all timing critical processes on the card. ###
+Sample rate To get the maximum sample rate of the active card and set the
+sample rate to the maximum, this is an example using internal PLL clock mode:
+```python clock = spcm.Clock(card) clock.mode(spcm.SPC_CM_INTPLL) sample_rate =
+clock.sample_rate(max=True) # (or) sample_rate = clock.sample_rate(20 *
+units.MHz) # for a 20 MHz sample rate (see reference manual for allowed values)
+print("Current sample rate: {}".format(sample_rate, return_unit=units.MS/
+units.s)) ``` ## Setting up the Trigger engine ### External trigger The Trigger
+engine can be configured for a multitude of different configurations (see the
+hardware manual for more information about the specific configurations for your
+device). Here we've given an example for an external trigger arriving at input
+port ext0, that is DC-coupled. The card is waiting for positiv edge that
+excedes 1.5 V: ```python trigger = spcm.Trigger(card) trigger.or_mask
+(spcm.SPC_TMASK_EXT0) # set the ext0 hardware input as trigger source
+trigger.ext0_mode(spcm.SPC_TM_POS) # wait for a positive edge
+trigger.ext0_level0(1.5 * units.V) trigger.ext0_coupling(spcm.COUPLING_DC) #
+set DC coupling ``` ## Setting up the multi-purpose I/O lines See the hardware
 manual, for the multi-purpose I/O lines functionality that can be programmed.
 ## Setting up a data transfer buffer for recording (digitizer) or replay (AWG)
 ### Recording (Digitizing) To transfer data to or from the card, we have to
 setup a data transfer object. This object allocates an amount the memory of the
 card (`memory_size`) and a Direct Memory Access (DMA) buffer on the host pc
 (`allocate_buffer`). Half of the samples are taken before the trigger, as
 configured by the trigger engine, and half of the samples are recorded
 afterwards. Then the transfer from the card to the host pc is started and the
 program waits until the DMA is filled. ```python # define the data buffer
+num_samples = 4 * units.KiS # 1 KiS = 1 KibiSamples = 1024 Samples
 data_transfer = spcm.DataTransfer(card) data_transfer.memory_size(num_samples)
 data_transfer.allocate_buffer(num_samples) data_transfer.post_trigger
 (num_samples // 2) # Start DMA transfer data_transfer.start_buffer_transfer
 (spcm.M2CMD_DATA_STARTDMA) # start card and wait until the memory is filled
 card.start(spcm.M2CMD_CARD_ENABLETRIGGER, spcm.M2CMD_DATA_WAITDMA) # (your code
 handling the recorded data comes here) ``` To access the recorded data, the
 data transfer object holds a [NumPy](https://numpy.org/) array object
@@ -143,25 +196,42 @@
 axis=1) ``` This data can be further processed or plotted using, for example,
 [`matplotlib`](https://matplotlib.org/). ### Replay (Generation) The setup of
 the DMA for replay is very similar. First card memory is allocated with
 `memory_size` and then a DMA buffer is allocated (`allocated_buffer`) and made
 accessible though the NumPy object `data_transfer.buffer`, which can then be
 written to using standard NumPy methods. Finally, data transfer from the host
 PC to the card is started and the programming is waiting until all the data is
-transferred: ```python data_transfer = spcm.DataTransfer(card)
-data_transfer.memory_size(num_samples) data_transfer.allocate_buffer
-(num_samples) data_transfer.loops(0) # loop continuously # simple linear ramp
-for analog output cards data_transfer.buffer[:] = np.arange(-num_samples//2,
-num_samples//2).astype(np.int16) data_transfer.start_buffer_transfer
-(spcm.M2CMD_DATA_STARTDMA, spcm.M2CMD_DATA_WAITDMA) ``` ## Multiple recording /
-replay In case of multiple recording / replay, the memory is divided in equally
-sized segments, that are populated / replayed when a trigger is detected.
-Multiple triggers each trigger the next segment to be populated or replayed.
-The following code snippet shows how to setup the buffer for 4 segments with
-each 128 Samples: ```python samples_per_segment = 128 num_segments = 4
+transferred: ```python num_samples = 4 * units.KiS # 1 KiS = 1 KibiSamples =
+1024 Samples data_transfer = spcm.DataTransfer(card) data_transfer.memory_size
+(num_samples) data_transfer.allocate_buffer(num_samples) data_transfer.loops(0)
+# loop continuously # simple linear ramp for analog output cards
+num_samples_magnitude = num_samples.to(units.S).magnitude data_transfer.buffer
+[:] = np.arange(-num_samples_magnitude//2, num_samples_magnitude//2).astype
+(np.int16) data_transfer.start_buffer_transfer(spcm.M2CMD_DATA_STARTDMA,
+spcm.M2CMD_DATA_WAITDMA) ``` #### Data transfer In the above it's assume that
+all the data has been transferred from the card into the buffer object, however
+if you're working in FIFO mode or you've defined the buffer to be smaller then
+the assigned card memory size, then the card will write to parts of the memory
+and tell you were it wrote. This can be either handled manually (see the
+reference manual of your card, or the methods `avail_card_len()`,
+`avail_user_pos()` and `avail_user_len()`). Secondly, it can also be handled
+with Python iterators functionality. If the `data_transfer` object is handed to
+a for-loop, then in each iteration a view of the current active memory part is
+given in the form of a NumPy array and the user can do calculations on that.
+```python # Get a block of data for data_block in data_transfer: # data_block
+is a NumPy array view of the currently active buffer part for channel in
+channels: data_units = channel.convert_data(data_block[:, channel]) minimum =
+np.min(data_units) maximum = np.max(data_units) print(f"Minimum: {minimum} -
+maximum: {maximum}") ``` The same principle also works with generator cards
+(see the example `2_gen_fifo.py`). ## Multiple recording / replay In case of
+multiple recording / replay, the memory is divided in equally sized segments,
+that are populated / replayed when a trigger is detected. Multiple triggers
+each trigger the next segment to be populated or replayed. The following code
+snippet shows how to setup the buffer for 4 segments with each 128 Samples:
+```python samples_per_segment = 128 * units.S num_segments = 4
 multiple_recording = spcm.Multi(card) multiple_recording.memory_size
 (samples_per_segment*num_segments) multiple_recording.allocate_buffer
 (segment_samples=samples_per_segment, num_segments=num_segments)
 multiple_recording.post_trigger(samples_per_segment // 2)
 multiple_recording.start_buffer_transfer(spcm.M2CMD_DATA_STARTDMA) ``` Again
 there are half the samples before and half the samples after the trigger. ##
 Timestamps See the example `6_acq_fifo_multi_ts_poll.py` in the examples folder
@@ -176,30 +246,30 @@
 is a simple example for setting up a single pulse generator on x0. Create a
 pulse generators object and get the clock rate used by the pulse generator. Use
 that to calculate the period of a 1 MHz signal and the half of that period
 we'll have a high signal (hence 50% duty cycle). The pulse generator will start
 if the trigger condition is met without delay and loops infinitely many times.
 The triggering condition is set to the card software trigger. See more details
 in the pulse generator chapter in the specific hardware manual. ```python
-pulse_generators = spcm.PulseGenerators(card) # get the clock of the card
-pulse_gen_clock_Hz = pulse_generators.get_clock() # generate a continuous
-signal with 1 MHz len_for_1MHz = pulse_gen_clock_Hz // spcm.MEGA(1)
-pulse_generators[0].mode(spcm.SPCM_PULSEGEN_MODE_TRIGGERED) pulse_generators
-[0].period_length(len_for_1MHz) pulse_generators[0].high_length(len_for_1MHz /
-/ 2) # 50% HIGH, 50% LOW pulse_generators[0].delay(0) pulse_generators
-[0].num_loops(0) # 0: infinite pulse_generators[0].mux1
-(spcm.SPCM_PULSEGEN_MUX1_SRC_UNUSED) pulse_generators[0].mux2
-(spcm.SPCM_PULSEGEN_MUX2_SRC_SOFTWARE) # started by software force command #
-and write the pulse generator settings pulse_generators.write_setup() # start
-all pulse generators that wait for a software command pulse_generators.force()
-``` This will start the pulse generator to continuously output a 1 MHz signal.
-### Sequence replay mode (AWG only) Please see the example `3_gen_sequence.py`
-in the folder `2_generation` of the examples to see an example dedicated to the
-Sequence replay mode. ### DDS (AWG only) Please see the examples in the
-dedicated examples folder `3_dds` for all the functionality provided by the DDS
+pulse_generators = spcm.PulseGenerators(card) # generate a continuous signal
+with 1 MHz pulse_generators[0].pulse_period(1 * units.us) # pulse_generators
+[0].repetition_rate(1 * units.MHz) # (or) pulse_generators[0].duty_cycle(50 *
+units.percent) # pulse_generators[0].pulse_length(0.5 * units.us) # (or)
+pulse_generators[0].start_delay(0 * units.us) pulse_generators[0].repetitions
+(0) # 0: infinite pulse_generators[0].start_condition_state_signal
+(spcm.SPCM_PULSEGEN_MUX1_SRC_UNUSED) pulse_generators
+[0].start_condition_trigger_signal(spcm.SPCM_PULSEGEN_MUX2_SRC_SOFTWARE)
+pulse_generators[0].invert_start_condition(False) # and write the pulse
+generator settings pulse_generators.write_setup() # start all pulse generators
+that wait for a software command pulse_generators.force() ``` This will start
+the pulse generator to continuously output a 1 MHz signal. ### Sequence replay
+mode (AWG only) Please see the example `3_gen_sequence.py` in the folder
+`2_generation` of the examples to see an example dedicated to the Sequence
+replay mode. ### DDS (AWG only) Please see the examples in the dedicated
+examples folder `3_dds` for all the functionality provided by the DDS
 framework. Moreover, please also have a look at the corresponding hardware
 manual. ### Boxcar (Digitizer only) See the corresponding chapter in the
 hardware manual for more information about boxcar averaging and the registers
 used. ### Block average (Digitizer only) See the corresponding chapter in the
 hardware manual for more information about block averaging and the registers
 used. # Acknowledgements We would like to thank [Christian Baker](https://
 github.com/crnbaker) for fruitful discussions and inspiration on how to setup
```

### Comparing `spcm-1.0.6/pyproject.toml` & `spcm-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
     "Topic :: System :: Hardware",
 ]
 dependencies = [
   "numpy >= 1.25.2",
   "h5py >= 3.10.0",
+  "pint >= 0.23",
 ]
 
 [project.urls]
 Homepage = "https://spectrum-instrumentation.com/"
 API = "https://spectruminstrumentation.github.io/spcm/spcm.html"
 Repository = "https://github.com/SpectrumInstrumentation/spcm"
 Examples = "https://github.com/SpectrumInstrumentation/spcm/tree/master/src/examples"
```

### Comparing `spcm-1.0.6/src/spcm/__init__.py` & `spcm-1.1.0/src/spcm/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,32 @@
 """
 .. include:: ./README.md
 
 .. include:: ./SUPPORTED_DEVICES.md
 """
 
 __docformat__ = "numpy"
+import numpy as np
+
+# Units available
+from pint import UnitRegistry
+try:
+    import matplotlib.pyplot as plt
+    mpl = True
+except ImportError:
+    mpl = False
+units = UnitRegistry(autoconvert_offset_to_baseunit=True)
+units.setup_matplotlib(mpl)
+units.define("sample = 1 = Sa = Sample = Samples = S")
+units.define("promille = 0.001 = ‰ = permille = perthousand = perthousands = ppt")
+units.define("fraction = 1 = frac = Frac = Fracs = Fraction = Fractions = Frac = Fracs")
+units.highZ = np.inf * units.ohm
+units.default_format = "~P" # see https://pint.readthedocs.io/en/stable/user/formatting.html
+units.mpl_formatter = "{:~P}" # see https://pint.readthedocs.io/en/stable/user/plotting.html
+__all__ = ["units"]
 
 # Import all registery entries and spectrum card errors into the module's name space
 from .constants import *
 
 # Import all the public classes into the module's namespace
 from .classes_device import Device
 from .classes_card import Card
@@ -27,15 +45,15 @@
 from .classes_time_stamp import TimeStamp
 from .classes_sequence import Sequence
 from .classes_dds import DDS, DDSCore
 from .classes_pulse_generators import PulseGenerator, PulseGenerators
 from .classes_block_average import BlockAverage
 from .classes_boxcar import Boxcar
 
-__all__ = [
+__all__ = [*__all__,
     "Device", "Card", "Sync", "CardStack", "Netbox", "CardFunctionality", "Channels", "Channel", "Clock", "Trigger", "MultiPurposeIOs", "MultiPurposeIO",
     "DataTransfer", "DDS", "DDSCore", "PulseGenerator", "PulseGenerators", "Multi", "TimeStamp", "Sequence", "BlockAverage", "Boxcar",
     "SpcmException", "SpcmTimeout", "SpcmError",
 ]
 
 # Versioning support using versioneer
 from . import _version
@@ -50,9 +68,7 @@
     if (driver_version.value & 0x0000FFFF) < 21797:
         raise OSError("Driver version {} does not support writing spcm version to log".format(driver_version))
     version_str = bytes("Python package spcm v{}".format(__version__), "utf-8")
     version_ptr = create_string_buffer(version_str)
     dwErr = spcm_dwSetParam_ptr(None, SPC_WRITE_TO_LOG, version_ptr, len(version_str))
 except OSError as e:
     print(e)
-
-#print(__version__)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `spcm-1.0.6/src/spcm/classes_block_average.py` & `spcm-1.1.0/src/spcm/classes_block_average.py`

 * *Files identical despite different names*

### Comparing `spcm-1.0.6/src/spcm/classes_boxcar.py` & `spcm-1.1.0/src/spcm/classes_boxcar.py`

 * *Files identical despite different names*

### Comparing `spcm-1.0.6/src/spcm/classes_card.py` & `spcm-1.1.0/src/spcm/classes_card.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,21 @@
     """
     a high-level class to control Spectrum Instrumentation cards
 
     For more information about what setups are available, please have a look at the user manual
     for your specific card.
 
     """
+
     _std_device_identifier : str = "/dev/spcm{}"
     _max_cards : int = 64
     
     _function_type : int = 0
     _card_type : int = 0
+    _max_sample_value : int = 0
 
     def __enter__(self) -> 'Card':
         """
         Context manager entry function
 
         Returns
         -------
@@ -66,17 +68,30 @@
             if self._handle:
                 print("Found '{}': {} sn {:05d}".format(self.device_identifier, self.product_name(), self.sn()))
 
         # Get the function type of the card
         self._function_type = self.get_i(SPC_FNCTYPE)
         self._card_type = self.get_i(SPC_PCITYP)
         self._features = self.get_i(SPC_PCIFEATURES)
+        self._max_sample_value = self.get_i(SPC_MIINST_MAXADCVALUE)
         
         return self
     
+    def __str__(self) -> str:
+        """
+        String representation of the card
+
+        Returns
+        -------
+        str
+            String representation of the card
+        """
+        return "Card: {} sn {:05d}".format(self.product_name(), self.sn())
+    __repr__ = __str__
+    
     def find(self, card_type : int = 0, serial_number : int = 0) -> Union[bool, int]:
         """
         Find first card that is connected to the computer, with either the given card type or serial number
 
         Parameters
         ----------
         card_type : int = 0
@@ -297,15 +312,15 @@
             number of bytes per sample
         """
         return self.get_i(SPC_MIINST_BYTESPERSAMPLE)
     
     def max_sample_value(self) -> int:
         """
         Get the maximum ADC value of the card (see register `SPC_MIINST_MAXADCVALUE` in the manual)
-    
+
         Returns
         -------
         int
             The maximum ADC value of the card
         """
 
-        return self.get_i(SPC_MIINST_MAXADCVALUE)
+        return self._max_sample_value
```

### Comparing `spcm-1.0.6/src/spcm/classes_card_stack.py` & `spcm-1.1.0/src/spcm/classes_card_stack.py`

 * *Files identical despite different names*

### Comparing `spcm-1.0.6/src/spcm/classes_channels.py` & `spcm-1.1.0/src/spcm/classes_channels.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,64 @@
 # -*- coding: utf-8 -*-
 
 from .constants import *
 
+import numpy as np
+import numpy.typing as npt
+
 from .classes_card import Card
 from .classes_card_stack import CardStack
 
 from .classes_error_exception import SpcmException
 
+from .classes_unit_conversion import UnitConversion
+from . import units
+import pint
 
 class Channel:
     """A class to represent a channel of a card only used inside the Channels class in the list of channels"""
 
     card : Card
     index : int
 
+    _conversion_amp : pint.Quantity = None
+    _conversion_offset : pint.Quantity = None
+    _output_load : pint.Quantity = None
+    _series_impedance : pint.Quantity = None
+
     def __init__(self, index : int, card : Card) -> None:
         """
         Constructor of the Channel class
     
         Parameters
         ----------
         index : int
             The index of the channel
         card : Card
             The card of the channel
         """
 
         self.card = card
         self.index = index
+        self._conversion_amp = None
+        self._conversion_offset = 0 * units.percent
+        self._output_load = 50 * units.ohm
+        self._series_impedance = 50 * units.ohm
     
     def __str__(self) -> str:
         """
         String representation of the Channel class
     
         Returns
         -------
         str
             String representation of the Channel class
         """
         
-        return f"Channel({self.index}, {self.card})"
+        return f"Channel {self.index}"
     
     __repr__ = __str__
 
     def __int__(self) -> int:
         """
         The Channel object acts like an int and returns the index of the channel and can also be used as the index in an array
 
@@ -105,52 +120,144 @@
         int
             The input path of the specific channel
         """
 
         if value is not None:
             self.card.set_i(SPC_PATH0 + (SPC_PATH1 - SPC_PATH0) * self.index, value)
         return self.card.get_i(SPC_PATH0 + (SPC_PATH1 - SPC_PATH0) * self.index)
-        
-    def amp(self, value : int = None) -> int:
+    
+    def amp(self, value : int = None, return_unit = None) -> int:
         """
         Sets the output/input range (amplitude) of the analog front-end of the channel of the card in mV (see register `SPC_AMP` in the manual)
     
         Parameters
         ----------
         value : int
             The output range (amplitude) of the specific channel in millivolts
+        unit : pint.Unit = None
+            The unit of the return value
             
         Returns
         -------
-        int
-            The output range (amplitude) of the specific channel in millivolts
+        int | pint.Quantity
+            The output range (amplitude) of the specific channel in millivolts or the unit specified
         """
 
         if value is not None:
+            if isinstance(value, pint.Quantity):
+                value = self.voltage_conversion(value)
+            self._conversion_amp = UnitConversion.force_unit(value, units.mV)
+            value = UnitConversion.convert(value, units.mV, int)
             self.card.set_i(SPC_AMP0 + (SPC_AMP1 - SPC_AMP0) * self.index, value)
-        return self.card.get_i(SPC_AMP0 + (SPC_AMP1 - SPC_AMP0) * self.index)
+        value = self.card.get_i(SPC_AMP0 + (SPC_AMP1 - SPC_AMP0) * self.index)
+        value = UnitConversion.to_unit(value * units.mV, return_unit)
+        return value
 
-    def offset(self, value : int = None) -> int:
+    def offset(self, value : int = None, return_unit = None) -> int:
         """
-        Sets the offset of the analog front-end of the channel of the card in mV (see register `SPC_OFFSET` in the manual)
+        Sets the offset of the analog front-end of the channel of the card in % of the full range o rmV (see register `SPC_OFFS0` in the manual)
+        If the value is given and has a unit, then this unit is converted to the unit of the card (mV or %)
     
         Parameters
         ----------
-        value : int
-            The offset of the specific channel in millivolts
+        value : int | pint.Quantity = None
+            The offset of the specific channel as integer in % or as a Quantity in % or mV
+        unit : pint.Unit = None
+            The unit of the return value
             
         Returns
         -------
-        int
-            The offset of the specific channel in millivolts
+        int | pint.Quantity
+            The offset of the specific channel in % or the unit specified by return_unit
         """
 
+        # Analog in cards are programmed in percent of the full range and analog output cards in mV (in the M2p, M4i/x and M5i families)
+        card_unit = 1
+        fnc_type = self.card.function_type()
+        if fnc_type == SPCM_TYPE_AI:
+            card_unit = units.percent
+        elif fnc_type == SPCM_TYPE_AO:
+            card_unit = units.mV
+
         if value is not None:
+            # The user gives a value as a Quantity
+            if isinstance(value, pint.Quantity):
+                if fnc_type == SPCM_TYPE_AO:
+                    # The card expects a value in mV
+                    if value.check('[]'):
+                        # Convert from percent to mV
+                        value = (value * self._conversion_amp).to(card_unit)
+                    else:
+                        value = value.to(card_unit)
+                elif fnc_type == SPCM_TYPE_AI:
+                    # The card expects a value in percent
+                    if value.check('[electric_potential]'):
+                        # Convert from mV to percent
+                        value = (value / self._conversion_amp).to(card_unit)
+                    else:
+                        value = value.to(card_unit)
+            else:
+                # Value is given as a number
+                pass
+
+            value = UnitConversion.convert(value, card_unit, int)
             self.card.set_i(SPC_OFFS0 + (SPC_OFFS1 - SPC_OFFS0) * self.index, value)
-        return self.card.get_i(SPC_OFFS0 + (SPC_OFFS1 - SPC_OFFS0) * self.index)
+        
+        return_value = self.card.get_i(SPC_OFFS0 + (SPC_OFFS1 - SPC_OFFS0) * self.index)
+        # Turn the return value into a quantity
+        return_quantity = UnitConversion.to_unit(return_value, return_unit)
+        # Save the conversion offset to be able to convert the data to a quantity with the correct unit
+        self._conversion_offset = UnitConversion.force_unit(return_value, card_unit)
+        return return_quantity
+    
+    def convert_data(self, data : npt.NDArray, return_unit : pint.Unit = units.mV) -> npt.NDArray:
+        """
+        Converts the data to the correct unit in units of electrical potential
+        
+        Parameters
+        ----------
+        data : numpy.ndarray
+            The data to be converted
+        return_unit : pint.Unit = None
+            The unit of the return value
+            
+        Returns
+        -------
+        numpy.ndarray
+            The converted data in units of electrical potential
+        """
+
+        max_value = self.card.max_sample_value()
+        if self._conversion_offset.check('[]'):
+            return_data = (data / max_value - self._conversion_offset) * self._conversion_amp
+        else:
+            return_data = (data / max_value) * self._conversion_amp - self._conversion_offset
+        return_data = UnitConversion.to_unit(return_data, return_unit)
+        return return_data
+    
+    def reconvert_data(self, data : npt.NDArray) -> npt.NDArray:
+        """
+        Convert data with units back to integer values in units of electrical potential
+        
+        Parameters
+        ----------
+        data : numpy.ndarray
+            The data to be reconverted
+            
+        Returns
+        -------
+        numpy.ndarray
+            The reconverted data as integer in mV
+        """
+
+        if self._conversion_offset.check('[]'):
+            return_data = int((data / self._conversion_amp + self._conversion_offset) * self.card.max_sample_value())
+        else:
+            return_data = int(((data + self._conversion_offset) / self._conversion_amp) * self.card.max_sample_value())
+        return return_data
 
     def termination(self, value : int) -> None:
         """
         Sets the termination of the analog front-end of the channel of the card (see register `SPC_50OHM0` in the manual)
     
         Parameters
         ----------
@@ -189,25 +296,25 @@
 
         if value is not None:
             self.card.set_i(SPC_ACDC0 + (SPC_ACDC1 - SPC_ACDC0) * self.index, value)
         return self.card.get_i(SPC_ACDC0 + (SPC_ACDC1 - SPC_ACDC0) * self.index)
     
     def coupling_offset_compensation(self, value : int = None) -> int:
         """
-        Sets the coupling offset compensation of the analog front-end of the channel of the card (see register `SPC_ACDC_OFFS_COMPENSATION0` in the manual)
+        Enables or disables the coupling offset compensation of the analog front-end of the channel of the card (see register `SPC_ACDC_OFFS_COMPENSATION0` in the manual)
     
         Parameters
         ----------
         value : int
-            The coupling offset compensation of the specific channel
+            Enables the coupling offset compensation of the specific channel
             
         Returns
         -------
         int
-            The coupling offset compensation of the specific channel
+            return if the coupling offset compensation of the specific channel is enabled ("1") or disabled ("0")
         """
 
         if value is not None:
             self.card.set_i(SPC_ACDC_OFFS_COMPENSATION0 + (SPC_ACDC_OFFS_COMPENSATION1 - SPC_ACDC_OFFS_COMPENSATION0) * self.index, value)
         return self.card.get_i(SPC_ACDC_OFFS_COMPENSATION0 + (SPC_ACDC_OFFS_COMPENSATION1 - SPC_ACDC_OFFS_COMPENSATION0) * self.index)
     
     def filter(self, value : int = None) -> int:
@@ -264,20 +371,125 @@
         value : int
             The custom stop value
 
         Returns
         -------
         int
             The custom stop value of the specific channel
+        
+        TODO: change this to a specific unit?
         """
 
         if value is not None:
             self.card.set_i(SPC_CH0_CUSTOM_STOP + self.index * (SPC_CH1_CUSTOM_STOP - SPC_CH0_CUSTOM_STOP), value)
         return self.card.get_i(SPC_CH0_CUSTOM_STOP + self.index * (SPC_CH1_CUSTOM_STOP - SPC_CH0_CUSTOM_STOP))
     
+    def ch_mask(self) -> int:
+        """
+        Gets mask for the "or"- or "and"-mask
+
+        Returns
+        -------
+        int
+            The mask for the "or"- or "and"-mask
+        """
+
+        return 1 << self.index
+    
+    def output_load(self, value : pint.Quantity = None) -> pint.Quantity:
+        """
+        Sets the electrical load of the user system connect the channel of the card. This is important for the correct
+        calculation of the output power. Typically, the load would be 50 Ohms, but it can be different.
+
+        Parameters
+        ----------
+        value : pint.Quantity
+            The electrical load connected by the user to the specific channel
+
+        Returns
+        -------
+        pint.Quantity
+            The electrical load connected by the user to the specific channel
+        """
+        if value is not None:
+            self._output_load = value
+        return self._output_load
+    
+    def voltage_conversion(self, value : pint.Quantity) -> pint.Quantity:
+        """
+        Convert the voltage that is needed at a certain output load to the voltage setting of the card if the load would be 50 Ohm
+
+        Parameters
+        ----------
+        value : pint.Quantity
+            The voltage that is needed at a certain output load
+
+        Returns
+        -------
+        pint.Quantity
+            The corresponding voltage at an output load of 50 Ohm
+        """
+
+        # The two at the end is because the value expected by the card is defined for a 50 Ohm load
+        if self._output_load == np.inf * units.ohm:
+            return value / 2
+        return value / (self._output_load / (self._output_load + self._series_impedance)) / 2
+
+    def to_amplitude_fraction(self, value) -> float:
+        """
+        Convert the voltage, percentage or power to percentage of the full range of the card
+
+        Parameters
+        ----------
+        value : pint.Quantity | float
+            The voltage that should be outputted at a certain output load
+
+        Returns
+        -------
+        float
+            The corresponding fraction of the full range of the card
+        """
+
+        if isinstance(value, units.Quantity) and value.check("[power]"):
+            # U_pk = U_rms * sqrt(2)
+            value = np.sqrt(2 * value.to('mW') * self._output_load) / self._conversion_amp * 100 * units.percent
+        elif isinstance(value, units.Quantity) and value.check("[electric_potential]"):
+            # value in U_pk
+            value = self.voltage_conversion(value) / self._conversion_amp * 100 * units.percent
+        value = UnitConversion.convert(value, units.fraction, float, rounding=None)
+        return value
+    
+    def from_amplitude_fraction(self, fraction, return_unit : pint.Quantity = None) -> pint.Quantity:
+        """
+        Convert the percentage of the full range to voltage, percentage or power
+
+        Parameters
+        ----------
+        fraction : float
+            The percentage of the full range of the card
+        return_unit : pint.Quantity
+            The unit of the return value
+
+        Returns
+        -------
+        pint.Quantity
+            The corresponding voltage, percentage or power
+        """
+
+        return_value = fraction
+        if isinstance(return_unit, units.Unit) and (1*return_unit).check("[power]"):
+            return_value = (np.power(self._conversion_amp * fraction, 2) / self._output_load / 2).to(return_unit)
+            # U_pk = U_rms * sqrt(2)
+        elif isinstance(return_unit, units.Unit) and (1*return_unit).check("[electric_potential]"):
+            return_value = (self._conversion_amp * fraction / 100).to(return_unit)
+            # value in U_pk
+            # value = self.voltage_conversion(value) / self._conversion_amp * 100 * units.percent
+        elif isinstance(return_unit, units.Unit) and (1*return_unit).check("[]"):
+            return_value = UnitConversion.force_unit(fraction, return_unit)
+        return return_value
 
 
 class Channels:
     """
     a higher-level abstraction of the CardFunctionality class to implement the Card's channel settings
     """
     
@@ -453,15 +665,15 @@
         ----------
         value : int
             The input path of the specific channel
         """
 
         for channel in self.channels:
             channel.path(value)
-        
+    
     def amp(self, value : int) -> None:
         """
         Sets the output/input range (amplitude) of the analog front-end of all channels of the card in mV (see register `SPC_AMP` in the manual)
     
         Parameters
         ----------
         value : int
@@ -563,8 +775,33 @@
         Parameters
         ----------
         value : int
             The custom stop value
         """
     
         for channel in self.channels:
-            channel.custom_stop(value)
+            channel.custom_stop(value)
+    
+    def output_load(self, value : pint.Quantity) -> None:
+        """
+        Sets the electrical load of the user system connect the channel of the card. This is important for the correct
+        calculation of the output power. Typically, the load would be 50 Ohms, but it can be different.
+
+        Parameters
+        ----------
+        value : pint.Quantity
+            The electrical load connected by the user to the specific channel
+        """
+        for channel in self.channels:
+            channel.output_load(value)
+    
+    def ch_mask(self) -> int:
+        """
+        Gets mask for the "or"- or "and"-mask
+
+        Returns
+        -------
+        int
+            The mask for the "or"- or "and"-mask
+        """
+
+        return sum([channel.ch_mask() for channel in self.channels])
```

### Comparing `spcm-1.0.6/src/spcm/classes_clock.py` & `spcm-1.1.0/src/spcm/classes_sync.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,119 +1,99 @@
 # -*- coding: utf-8 -*-
 
 from .constants import *
 
-from .classes_functionality import CardFunctionality 
+from .classes_device import Device
 
-class Clock(CardFunctionality):
-    """a higher-level abstraction of the CardFunctionality class to implement the Card's clock engine"""
-    
-    def __str__(self) -> str:
-        """
-        String representation of the Clock class
-    
-        Returns
-        -------
-        str
-            String representation of the Clock class
-        """
-        
-        return f"Clock(card={self.card})"
-    
-    __repr__ = __str__
-    
-    def write_setup(self) -> None:
-        """Write the setup to the card"""
-        self.card.write_setup()
-    
+class Sync(Device):
+    """a class to control Spectrum Instrumentation Starhub synchronization devices
+
+    For more information about what setups are available, please have a look at the user manual
+    for your specific Starhub.
     
-    def mode(self, mode : int = None) -> int:
+    Exceptions
+    ----------
+    SpcmException
+    SpcmTimeout
+    """
+
+    def enable(self, enable : int = None) -> int:
         """
-        Set the clock mode of the card (see register `SPC_CLOCKMODE` in the manual)
-    
+        Enable or disable the Starthub (see register 'SPC_SYNC_ENABLEMASK' in chapter `Star-Hub` in the manual)
+
         Parameters
         ----------
-        mode : int
-            The clock mode of the card
-        
-        Returns
-        -------
-        int
-            The clock mode of the card
+        enable : int or bool
+            enable or disable the Starthub
         """
 
-        if mode is not None:
-            self.card.set_i(SPC_CLOCKMODE, mode)
-        return self.card.get_i(SPC_CLOCKMODE)
+        if enable is not None:
+            enable_mask = 0
+            if isinstance(enable, bool):
+                num_cards = self.sync_count()
+                enable_mask = ((1 << num_cards) - 1) if enable else 0
+            elif isinstance(enable, int):
+                enable_mask = enable
+            else:
+                raise ValueError("The enable parameter must be a boolean or an integer")
+            self.set_i(SPC_SYNC_ENABLEMASK, enable_mask)
+        return self.get_i(SPC_SYNC_ENABLEMASK)
     
-    def max_sample_rate(self) -> int:
+    def num_connectors(self) -> int:
         """
-        Returns the maximum sample rate of the active card (see register `SPC_MIINST_MAXADCLOCK` in the manual)
-    
+        Number of connectors that the Star-Hub offers at max. (see register 'SPC_SYNC_READ_NUMCONNECTORS' in chapter `Star-Hub` in the manual)
+
         Returns
         -------
         int
+            number of connectors on the StarHub
         """
-        
-        return self.card.get_i(SPC_MIINST_MAXADCLOCK)
 
-    def sample_rate(self, sample_rate : int = 0, max : bool = False) -> int:
+        return self.get_i(SPC_SYNC_READ_NUMCONNECTORS)
+    
+    def sync_count(self) -> int:
         """
-        Sets or gets the current sample rate of the handled card (see register `SPC_SAMPLERATE` in the manual)
+        Number of cards that are connected to this Star-Hub (see register 'SPC_SYNC_READ_SYNCCOUNT' in chapter `Star-Hub` in the manual)
 
-        Parameters
-        ----------
-        sample_rate : int = 0
-            if the parameter sample_rate is given with the function call, then the card's sample rate is set to that value
-        max : bool = False
-            if max is True, the method sets the maximum sample rate of the card
-    
         Returns
         -------
         int
-            the current sample rate in Samples/s
+            number of synchronized cards
         """
-        
-        if max:
-            sample_rate = self.max_sample_rate()
-        if sample_rate:
-            self.card.set_i(SPC_SAMPLERATE, int(sample_rate))
-        return self.card.get_i(SPC_SAMPLERATE)
+
+        return self.get_i(SPC_SYNC_READ_SYNCCOUNT)
     
-    def clock_output(self, clock_output : int = None) -> int:
+    def card_index(self, index) -> int:
         """
-        Set the clock output of the card (see register `SPC_CLOCKOUT` in the manual)
-        
+        Index of the card that is connected to the Star-Hub at the given local index (see register 'SPC_SYNC_READ_CARDIDX0' in chapter `Star-Hub` in the manual)
+
         Parameters
         ----------
-        clock_output : int
-            the clock output of the card
-        
+        index : int
+            connector index
+
         Returns
         -------
         int
-            the clock output of the card
+            card index
         """
-        
-        if clock_output is not None:
-            self.card.set_i(SPC_CLOCKOUT, clock_output)
-        return self.card.get_i(SPC_CLOCKOUT)
-    output = clock_output
+
+        return self.get_i(SPC_SYNC_READ_CARDIDX0 + index)
     
-    def reference_clock(self, reference_clock : int = None) -> int:
+    def cable_connection(self, index) -> int:
         """
-        Set the reference clock of the card (see register `SPC_REFERENCECLOCK` in the manual)
-        
+        Returns the index of the cable connection that is used for the logical connection `index`. (see register 'SPC_SYNC_READ_CABLECON0' in chapter `Star-Hub` in the manual)
+        The cable connections can be seen printed on the PCB of the star-hub. Use these cable connection information in case 
+        that there are hardware failures with the star-hub cabeling.
+
         Parameters
         ----------
-        reference_clock : int
-            the reference clock of the card in Hz
-        
+        index : int
+            connector index
+
         Returns
         -------
         int
-            the reference clock of the card in Hz
+            cable index
         """
-        
-        if reference_clock is not None:
-            self.card.set_i(SPC_REFERENCECLOCK, reference_clock)
-        return self.card.get_i(SPC_REFERENCECLOCK)
+
+        return self.get_i(SPC_SYNC_READ_CABLECON0 + index)
```

### Comparing `spcm-1.0.6/src/spcm/classes_data_transfer.py` & `spcm-1.1.0/src/spcm/classes_pulse_generators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,625 +1,766 @@
 # -*- coding: utf-8 -*-
 
-import numpy as np
-import numpy.typing as npt
-
-import h5py
-from pathlib import Path
+# TODO: implement units here and test that!
 
 from .constants import *
 
-from .pyspcm import c_void_p, spcm_dwDefTransfer_i64
+import numpy as np
 
+from .classes_error_exception import SpcmException
+from .classes_card import Card
 from .classes_functionality import CardFunctionality
 
-from .classes_error_exception import SpcmException, SpcmTimeout
+import pint
+from .classes_unit_conversion import UnitConversion
+from . import units
 
-class DataTransfer(CardFunctionality):
+class PulseGenerator:
     """
-    A high-level class to control Data Transfer to and from Spectrum Instrumentation cards.
-
-    This class is an iterator class that implements the functions `__iter__` and `__next__`.
-    This allows the user to supply the class to a for loop and iterate over the data that 
-    is transferred from or to the card. Each iteration will return a numpy array with a data
-    block of size `notify_samples`. In case of a digitizer you can read the data from that 
-    block and process it. In case of a generator you can write data to the block and it's 
-    then transferred.
-
-    For more information about what setups are available, please have a look at the user manual
-    for your specific card.
-
+    a class to implement a single pulse generator
+    
     Parameters
     ----------
-    `buffer` : NDArray[np.int_]
-        numpy object that can be used to write data into the spcm buffer
-    `buffer_size`: int
-        defines the size of the current buffer shared between the PC and the card
-    `buffer_type`: int
-        defines the type of data in the buffer that is used for the transfer
-    `num_channels`: int
-        defines the number of channels that are used for the transfer
-    `bytes_per_sample`: int
-        defines the number of bytes per sample
-    `bits_per_sample`: int
-        defines the number of bits per sample
-
+    card : Card
+        the card object that is used by the functionality
+    pg_index : int
+        the index of the used pulse generator
     """
-    # public
-    buffer_size : int = 0
-    buffer_type : int
-    num_channels : int = 0
-    bytes_per_sample : int = 0
-    bits_per_sample : int = 0
-
-    # private
-    _num_samples : int = 0
-    _notify_samples : int = 0
-
-    @property
-    def buffer(self) -> npt.NDArray[np.int_]:
-        """The numpy buffer object that interfaces the Card and can be written and read from"""
-        return self._np_buffer
-    
-    @buffer.setter
-    def buffer(self, value) -> None:
-        self._np_buffer = value
-    
-    @buffer.deleter
-    def buffer(self) -> None:
-        del self._np_buffer
-
-    # private
-    _memory_size : int = 0
-    _c_buffer = None # Internal numpy ctypes buffer object
-    _buffer_alignment : int = 4096
-    _np_buffer : npt.NDArray[np.int_] # Internal object on which the getter setter logic is working
-    _8bit_mode : bool = False
-    _12bit_mode : bool = False
 
-    def __init__(self, card, *args, **kwargs) -> None:
+    card : Card
+    pg_index : int
+    """The index of the pulse generator"""
+
+    _reg_distance : int = 100
+
+    def __init__(self, card : Card, pg_index : int, *args, **kwargs) -> None:
         """
-        Initialize the DataTransfer object with a card object and additional arguments
+        The constructor of the PulseGenerator class
 
         Parameters
         ----------
         card : Card
-            the card object that is used for the data transfer
-        *args : list
-            list of additional arguments
-        **kwargs : dict
-            dictionary of additional keyword arguments
-        """
-        
-        self.buffer_size = 0
-        self.num_channels = 0
-        self.bytes_per_sample = 0
-        self.bits_per_sample = 0
-        self._num_samples = 0
-        self._notify_samples = 0
-        self._memory_size = 0
-        self._c_buffer = None
-        self._buffer_alignment = 4096
-        self._np_buffer = None
-        self._8bit_mode = False
-        self._12bit_mode = False
+            the card object that is used by the functionality
+        pg_index : int
+            the index of the used pulse generator
+        """
         
-        super().__init__(card, *args, **kwargs)
-        self.buffer_type = SPCM_BUF_DATA
-        self._bytes_per_sample()
-        self._bits_per_sample()
-        self.num_channels = self.card.active_channels()
+        self.card = card
+        self.pg_index = pg_index
 
-    def _sample_rate(self) -> int:
+    def __str__(self) -> str:
+        """
+        String representation of the PulseGenerator class
+    
+        Returns
+        -------
+        str
+            String representation of the PulseGenerator class
+        """
+        
+        return f"PulseGenerator(card={self.card}, pg_index={self.pg_index})"
+    
+    __repr__ = __str__
+    
+    # The trigger behavior of the pulse generator
+    def mode(self, mode : int = None) -> int:
         """
-        Get the sample rate of the card
+        Set the trigger mode of the pulse generator (see register 'SPC_XIO_PULSEGEN0_MODE' in chapter `Pulse Generator` in the manual)
 
+        Parameters
+        ----------
+        mode : int
+            The trigger mode
+        
         Returns
         -------
         int
-            the sample rate of the card
+            The trigger mode
         """
-        return self.card.get_i(SPC_SAMPLERATE)
 
-    def memory_size(self, memory_size : int = None) -> int:
+        if mode is not None:
+            self.card.set_i(SPC_XIO_PULSEGEN0_MODE + self._reg_distance*self.pg_index, mode)
+        return self.card.get_i(SPC_XIO_PULSEGEN0_MODE + self._reg_distance*self.pg_index)
+    
+    # The duration of a single period
+    def period_length(self, length : int = None) -> int:
         """
-        Sets the memory size in samples per channel. The memory size setting must be set before transferring 
-        data to the card. (see register `SPC_MEMSIZE` in the manual)
-        
+        Set the period length of the pulse generator (see register 'SPC_XIO_PULSEGEN0_LEN' in chapter `Pulse Generator` in the manual)
+
         Parameters
         ----------
-        memory_size : int
-            the size of the memory in Bytes
+        length : int
+            The period length in clock cycles
+        
+        Returns
+        -------
+        int
+            The period length in clock cycles
         """
 
-        if memory_size is not None:
-            self.card.set_i(SPC_MEMSIZE, memory_size)
-        self._memory_size = self.card.get_i(SPC_MEMSIZE)
-        return self._memory_size
+        if length is not None:
+            self.card.set_i(SPC_XIO_PULSEGEN0_LEN + self._reg_distance*self.pg_index, length)
+        return self.card.get_i(SPC_XIO_PULSEGEN0_LEN + self._reg_distance*self.pg_index)
+
+    def avail_length_min(self) -> int:
+        """
+        Returns the minimum length (period) of the pulse generator’s output pulses in clock cycles. (see register 'SPC_XIO_PULSEGEN_AVAILLEN_MIN' in chapter `Pulse Generator` in the manual)
+
+        Returns
+        -------
+        int
+            The available minimal length in clock cycles
+        """
+        return self.card.get_i(SPC_XIO_PULSEGEN_AVAILLEN_MIN)
     
-    def notify_samples(self, notify_samples : int) -> None:
+    def avail_length_max(self) -> int:
         """
-        Set the number of samples to notify the user about
-        
+        Returns the maximum length (period) of the pulse generator’s output pulses in clock cycles. (see register 'SPC_XIO_PULSEGEN_AVAILLEN_MAX' in chapter `Pulse Generator` in the manual)
+
+        Returns
+        -------
+        int
+            The available maximal length in clock cycles
+        """
+        return self.card.get_i(SPC_XIO_PULSEGEN_AVAILLEN_MAX)
+    
+    def avail_length_step(self) -> int:
+        """
+        Returns the step size of the pulse generator’s output pulses in clock cycles. (see register 'SPC_XIO_PULSEGEN_AVAILLEN_STEP' in chapter `Pulse Generator` in the manual)
+
+        Returns
+        -------
+        int
+            The available step size in clock cycles
+        """
+        return self.card.get_i(SPC_XIO_PULSEGEN_AVAILLEN_STEP)
+    
+    # The time that the signal is high during one period
+    def high_length(self, length : int = None) -> int:
+        """
+        Set the high length of the pulse generator (see register 'SPC_XIO_PULSEGEN0_HIGH' in chapter `Pulse Generator` in the manual)
+
         Parameters
         ----------
-        notify_samples : int
-            the number of samples to notify the user about
+        pg_index : int
+            The index of the pulse generator
+        length : int
+            The high length in clock cycles
+        
+        Returns
+        -------
+        int
+            The high length in clock cycles
         """
-        self._notify_samples = notify_samples
+
+        if length is not None:
+            self.card.set_i(SPC_XIO_PULSEGEN0_HIGH + self._reg_distance*self.pg_index, length)
+        return self.card.get_i(SPC_XIO_PULSEGEN0_HIGH + self._reg_distance*self.pg_index)
     
-    def loops(self, loops : int = None) -> int:
+    def avail_high_min(self) -> int:
         """
-        Set the number of times the memory is replayed. If set to zero the generation will run continuously until it is 
-        stopped by the user.  (see register `SPC_LOOPS` in the manual)
-        
+        Returns the minimum high length of the pulse generator’s output pulses in clock cycles. (see register 'SPC_XIO_PULSEGEN_AVAILHIGH_MIN' in chapter `Pulse Generator` in the manual)
+
+        Returns
+        -------
+        int
+            The available minimal high length in clock cycles
+        """
+        return self.card.get_i(SPC_XIO_PULSEGEN_AVAILHIGH_MIN)
+    
+    def avail_high_max(self) -> int:
+        """
+        Returns the maximum high length of the pulse generator’s output pulses in clock cycles. (see register 'SPC_XIO_PULSEGEN_AVAILHIGH_MAX' in chapter `Pulse Generator` in the manual)
+
+        Returns
+        -------
+        int
+            The available maximal high length in clock cycles
+        """
+        return self.card.get_i(SPC_XIO_PULSEGEN_AVAILHIGH_MAX)
+    
+    def avail_high_step(self) -> int:
+        """
+        Returns the step size of the pulse generator’s output pulses in clock cycles. (see register 'SPC_XIO_PULSEGEN_AVAILHIGH_STEP' in chapter `Pulse Generator` in the manual)
+
+        Returns
+        -------
+        int
+            The available step size in clock cycles
+        """
+        return self.card.get_i(SPC_XIO_PULSEGEN_AVAILHIGH_STEP)
+    
+    # The number of times that a single period is repeated
+    def num_loops(self, loops : int = None) -> int:
+        """
+        Set the number of loops of a single period on the pulse generator (see register 'SPC_XIO_PULSEGEN0_LOOPS' in chapter `Pulse Generator` in the manual)
+
         Parameters
         ----------
         loops : int
-            the number of loops that the card should perform
+            The number of loops
+        
+        Returns
+        -------
+        int
+            The number of loops
         """
 
         if loops is not None:
-            self.card.set_i(SPC_LOOPS, loops)
-        return self.card.get_i(SPC_LOOPS)
+            self.card.set_i(SPC_XIO_PULSEGEN0_LOOPS + self._reg_distance*self.pg_index, loops)
+        return self.card.get_i(SPC_XIO_PULSEGEN0_LOOPS + self._reg_distance*self.pg_index)
+    
+    def avail_loops_min(self) -> int:
+        """
+        Returns the minimum number of loops of the pulse generator’s output pulses. (see register 'SPC_XIO_PULSEGEN_AVAILLOOPS_MIN' in chapter `Pulse Generator` in the manual)
 
-    def _bits_per_sample(self) -> int:
+        Returns
+        -------
+        int
+            The available minimal number of loops
+        """
+        return self.card.get_i(SPC_XIO_PULSEGEN_AVAILLOOPS_MIN)
+    
+    def avail_loops_max(self) -> int:
         """
-        Get the number of bits per sample
+        Returns the maximum number of loops of the pulse generator’s output pulses. (see register 'SPC_XIO_PULSEGEN_AVAILLOOPS_MAX' in chapter `Pulse Generator` in the manual)
 
         Returns
         -------
         int
-            number of bits per sample
+            The available maximal number of loops
         """
-        if self._8bit_mode:
-            self.bits_per_sample = 8
-        elif self._12bit_mode:
-            self.bits_per_sample = 12        
-        else:
-            self.bits_per_sample = self.card.bits_per_sample()
+        return self.card.get_i(SPC_XIO_PULSEGEN_AVAILLOOPS_MAX)
     
-    def _bytes_per_sample(self) -> int:
+    def avail_loops_step(self) -> int:
         """
-        Get the number of bytes per sample
+        Returns the step size of the pulse generator’s output pulses. (see register 'SPC_XIO_PULSEGEN_AVAILLOOPS_STEP' in chapter `Pulse Generator` in the manual)
 
         Returns
         -------
         int
-            number of bytes per sample
+            Returns the step size when defining the repetition of pulse generator’s output.
         """
-        if self._8bit_mode:
-            self.bytes_per_sample = 1
-        elif self._12bit_mode:
-            self.bytes_per_sample = 1.5
-        else:
-            self.bytes_per_sample = self.card.bytes_per_sample()
+        return self.card.get_i(SPC_XIO_PULSEGEN_AVAILLOOPS_STEP)
     
-    def pre_trigger(self, num_samples : int = None) -> int:
+    # The delay between the start of the pulse generator and the first pulse
+    def delay(self, delay : int = None) -> int:
         """
-        Set the number of pre trigger samples (see register `SPC_PRETRIGGER` in the manual)
-        
+        Set the delay of the pulse generator (see register 'SPC_XIO_PULSEGEN0_DELAY' in chapter `Pulse Generator` in the manual)
+
         Parameters
         ----------
-        num_samples : int
-            the number of pre trigger samples
+        delay : int
+            The delay in clock cycles
+        
+        Returns
+        -------
+        int
+            The delay in clock cycles
         """
 
-        if num_samples is not None:
-            self.card.set_i(SPC_PRETRIGGER, num_samples)
-        return self.card.get_i(SPC_PRETRIGGER)
+        if delay is not None:
+            self.card.set_i(SPC_XIO_PULSEGEN0_DELAY + self._reg_distance*self.pg_index, delay)
+        return self.card.get_i(SPC_XIO_PULSEGEN0_DELAY + self._reg_distance*self.pg_index)
     
-    def post_trigger(self, num_samples : int = None) -> int:
+    def avail_delay_min(self) -> int:
         """
-        Set the number of post trigger samples (see register `SPC_POSTTRIGGER` in the manual)
-        
-        Parameters
-        ----------
-        num_samples : int
-            the number of post trigger samples
+        Returns the minimum delay of the pulse generator’s output pulses in clock cycles. (see register 'SPC_XIO_PULSEGEN_AVAILDELAY_MIN' in chapter `Pulse Generator` in the manual)
+
+        Returns
+        -------
+        int
+            The available minimal delay in clock cycles
+        """
+        return self.card.get_i(SPC_XIO_PULSEGEN_AVAILDELAY_MIN)
+    
+    def avail_delay_max(self) -> int:
         """
+        Returns the maximum delay of the pulse generator’s output pulses in clock cycles. (see register 'SPC_XIO_PULSEGEN_AVAILDELAY_MAX' in chapter `Pulse Generator` in the manual)
 
-        if num_samples is not None:
-            self.card.set_i(SPC_POSTTRIGGER, num_samples)
-        return self.card.get_i(SPC_POSTTRIGGER)
+        Returns
+        -------
+        int
+            The available maximal delay in clock cycles
+        """
+        return self.card.get_i(SPC_XIO_PULSEGEN_AVAILDELAY_MAX)
     
-    def allocate_buffer(self, num_samples : int) -> None:
+    def avail_delay_step(self) -> int:
         """
-        Memory allocation for the buffer that is used for communicating with the card
+        Returns the step size of the delay of the pulse generator’s output pulses in clock cycles. (see register 'SPC_XIO_PULSEGEN_AVAILDELAY_STEP' in chapter `Pulse Generator` in the manual)
 
-        Parameters
-        ----------
-        num_samples : int = None
-            use the number of samples an get the number of active channels and bytes per samples directly from the card
+        Returns
+        -------
+        int
+            The available step size of the delay in clock cycles
         """
-        
-        self._num_samples = num_samples
+        return self.card.get_i(SPC_XIO_PULSEGEN_AVAILDELAY_STEP)
 
-        sample_type = self.numpy_type()
+    # Trigger muxes
+    def mux1(self, mux : int = None) -> int:
+        """
+        Set the trigger mux 1 of the pulse generator (see register 'SPC_XIO_PULSEGEN0_MUX1_SRC' in chapter `Pulse Generator` in the manual)
 
-        if self.bits_per_sample > 1:
-            self.buffer_size = int(self._num_samples * self.bytes_per_sample * self.num_channels)
-        else:
-            self.buffer_size = int(self._num_samples * self.num_channels // 8)
+        Parameters
+        ----------
+        mux : int
+            The trigger mux 1
+        
+        Returns
+        -------
+        int
+            The trigger mux 1
+        """
 
-        dwMask = self._buffer_alignment - 1
+        if mux is not None:
+            self.card.set_i(SPC_XIO_PULSEGEN0_MUX1_SRC + self._reg_distance*self.pg_index, mux)
+        return self.card.get_i(SPC_XIO_PULSEGEN0_MUX1_SRC + self._reg_distance*self.pg_index)
+    
+    def mux2(self, mux : int = None) -> int:
+        """
+        Set the trigger mux 2 of the pulse generator (see register 'SPC_XIO_PULSEGEN0_MUX2_SRC' in chapter `Pulse Generator` in the manual)
 
-        item_size = sample_type(0).itemsize
-        # allocate a buffer (numpy array) for DMA transfer: a little bigger one to have room for address alignment
-        databuffer_unaligned = np.empty(((self._buffer_alignment + self.buffer_size) // item_size, ), dtype = sample_type)   # byte count to sample (// = integer division)
-        # two numpy-arrays may share the same memory: skip the begin up to the alignment boundary (ArrayVariable[SKIP_VALUE:])
-        # Address of data-memory from numpy-array: ArrayVariable.__array_interface__['data'][0]
-        start_pos_samples = ((self._buffer_alignment - (databuffer_unaligned.__array_interface__['data'][0] & dwMask)) // item_size)
-        self.buffer = databuffer_unaligned[start_pos_samples:start_pos_samples + (self.buffer_size // item_size)]   # byte address to sample size
-        if self.bits_per_sample > 1:
-            if not self._12bit_mode:
-                self.buffer = self.buffer.reshape((self.num_channels, num_samples), order='F')
-    
-    def start_buffer_transfer(self, *args, buffer_type=SPCM_BUF_DATA, direction=None, notify_samples=0, transfer_offset=0, transfer_length=None, exception_num_samples=False) -> None:
-        """
-        Start the transfer of the data to or from the card  (see the API function `spcm_dwDefTransfer_i64` in the manual)
-        
         Parameters
         ----------
-        *args : list
-            list of additonal arguments that are added as flags to the start dma command
-        buffer_type : int
-            the type of buffer that is used for the transfer
-        direction : int
-            the direction of the transfer
-        notify_samples : int
-            the number of samples to notify the user about
-        transfer_offset : int
-            the offset of the transfer
-        transfer_length : int
-            the length of the transfer
-        exception_num_samples : bool
-            if True, an exception is raised if the number of samples is not a multiple of the notify samples. The automatic buffer handling only works with the number of samples being a multiple of the notify samples.
+        mux : int
+            The trigger mux 2
 
-        Raises
-        ------
-        SpcmException
+        Returns
+        -------
+        int
+            The trigger mux 2
         """
 
-        if self.buffer is None: 
-            raise SpcmException(text="No buffer defined for transfer")
-        if buffer_type: 
-            self.buffer_type = buffer_type
-        if direction is None:
-            if self.function_type == SPCM_TYPE_AI or self.function_type == SPCM_TYPE_DI:
-                direction = SPCM_DIR_CARDTOPC
-            elif self.function_type == SPCM_TYPE_AO or self.function_type == SPCM_TYPE_DO:
-                direction = SPCM_DIR_PCTOCARD
-            else:
-                raise SpcmException(text="Please define a direction for transfer (SPCM_DIR_CARDTOPC or SPCM_DIR_PCTOCARD)")
-        
-        notify_size = 0
-        if notify_samples: 
-            self._notify_samples = notify_samples
-        if self._notify_samples: 
-            notify_size = int(self._notify_samples * self.bytes_per_sample * self.num_channels)
-        
-        if self._notify_samples != 0 and np.remainder(self._num_samples, self._notify_samples) and exception_num_samples:
-            raise SpcmException("The number of samples needs to be a multiple of the notify samples.")
+        if mux is not None:
+            self.card.set_i(SPC_XIO_PULSEGEN0_MUX2_SRC + self._reg_distance*self.pg_index, mux)
+        return self.card.get_i(SPC_XIO_PULSEGEN0_MUX2_SRC + self._reg_distance*self.pg_index)
+    
+    def config(self, config : int = None) -> int:
+        """
+        Set the configuration of the pulse generator (see register 'SPC_XIO_PULSEGEN0_CONFIG' in chapter `Pulse Generator` in the manual)
 
-        if transfer_offset:
-            transfer_offset_bytes = transfer_offset * self.bytes_per_sample * self.num_channels
-        else:
-            transfer_offset_bytes = 0
+        Parameters
+        ----------
+        config : int
+            The configuration of the pulse generator
 
-        if transfer_length is not None: 
-            transfer_length_bytes = transfer_length * self.bytes_per_sample * self.num_channels
-        else:
-            transfer_length_bytes = self.buffer_size
-        
-        # we define the buffer for transfer and start the DMA transfer
-        self.card._print("Starting the DMA transfer and waiting until data is in board memory")
-        self._c_buffer = self.buffer.ctypes.data_as(c_void_p)
-        spcm_dwDefTransfer_i64(self.card._handle, self.buffer_type, direction, notify_size, self._c_buffer, transfer_offset_bytes, transfer_length_bytes)
-        cmd = 0
-        for arg in args:
-            cmd |= arg
-        self.card.cmd(cmd)
-        self.card._print("... data transfer started")
+        Returns
+        -------
+        int
+            The configuration of the pulse generator
+        """
+
+        if config is not None:
+            self.card.set_i(SPC_XIO_PULSEGEN0_CONFIG + self._reg_distance*self.pg_index, config)
+        return self.card.get_i(SPC_XIO_PULSEGEN0_CONFIG + self._reg_distance*self.pg_index)
     
-    def unpack_12bit_buffer(self, data : npt.NDArray[np.int_] = None) -> npt.NDArray[np.int_]:
+    def _get_clock(self, return_unit : pint.Unit = None) -> int:
         """
-        Unpack the 12bit buffer to a 16bit buffer
+        Get the clock rate of the pulse generator (see register 'SPC_XIO_PULSEGEN_CLOCK' in chapter `Pulse Generator` in the manual)
 
         Returns
         -------
-        numpy array
-            the unpacked 16bit buffer
+        int
+            The clock rate in Hz
         """
 
-        if not self._12bit_mode:
-            raise SpcmException("The card is not in 12bit packed mode")
-        
-        if data is None:
-            data = self.buffer
-
-        fst_int8, mid_int8, lst_int8 = np.reshape(data, (data.shape[0] // 3, 3)).astype(np.int16).T
-        nibble_h = (mid_int8 >> 0) & 0x0F
-        nibble_m = (fst_int8 >> 4) & 0x0F
-        nibble_l = (fst_int8 >> 0) & 0x0F
-        fst_int12 = ((nibble_h << 12) >> 4) | (nibble_m << 4) | (nibble_l << 0)
-        nibble_h = (lst_int8 >> 4) & 0x0F
-        nibble_m = (lst_int8 >> 0) & 0x0F
-        nibble_l = (mid_int8 >> 4) & 0x0F
-        snd_int12 = ((nibble_h << 12) >> 4) | (nibble_m << 4) | (nibble_l << 0)
-        data_int12 = np.concatenate((fst_int12[:, None], snd_int12[:, None]), axis=1).reshape((-1,))
-        data_int12 = data_int12.reshape((self.num_channels, self._num_samples), order='F')
-        return data_int12
+        return_value = self.card.get_i(SPC_XIO_PULSEGEN_CLOCK)
+        return_value = UnitConversion.to_unit(return_value * units.Hz, return_unit)
+        return return_value
+    
+    # Higher abtraction functions
 
-    def tofile(self, filename : str, **kwargs) -> None:
+    def pulse_period(self, period : pint.Quantity = None, return_unit : pint.Unit = units.s) -> pint.Quantity:
         """
-        Export the buffer to a file. The file format is determined by the file extension
-        Supported file formats are: 
-        * .bin: raw binary file
-        * .csv: comma-separated values file
-        * .npy: numpy binary file
-        * .npz: compressed numpy binary file
-        * .txt: whitespace-delimited text file
-        * .h5: hdf5 file format
+        Set the period length of the pulse generator signal in a time unit
 
         Parameters
         ----------
-        filename : str
-            the name of the file that the buffer should be exported to
+        period : pint.Quantity
+            The period length in seconds
         
-        Raises
-        ------
-        ImportError
-            if the file format is not supported
+        Returns
+        -------
+        pint.Quantity
+            The period length in seconds
         """
 
-        file_path = Path(filename)
-        if file_path.suffix == '.bin':
-            dtype = kwargs.get('dtype', self.numpy_type())
-            self.buffer.tofile(file_path, dtype=dtype)
-        elif file_path.suffix == '.csv':
-            delimiter = kwargs.get('delimiter', ',')
-            np.savetxt(file_path, self.buffer, delimiter=delimiter)
-        elif file_path.suffix == '.npy':
-            np.save(file_path, self.buffer)
-        elif file_path.suffix == '.npz':
-            np.savez_compressed(file_path, self.buffer)
-        elif file_path.suffix == '.txt':
-            np.savetxt(file_path, self.buffer, fmt='%d')
-        elif file_path.suffix == '.h5' or file_path.suffix == '.hdf5':
-            with h5py.File(file_path, 'w') as f:
-                f.create_dataset('data', data=self.buffer)
-        else:
-            raise ImportError("File format not supported")
-        
-    def fromfile(self, filename : str, **kwargs) -> None:
+        if period is not None:
+            if isinstance(period, pint.Quantity):
+                period = int((period * self._get_clock(units.Hz)).to_base_units().magnitude)
+            else:
+                raise ValueError("The period must be a pint.Quantity")
+            self.period_length(period)
+        return_value = self.period_length()
+        return_value = UnitConversion.to_unit((return_value / self._get_clock(units.Hz)), return_unit)
+        return return_value
+    
+    def repetition_rate(self, rate : pint.Quantity = None, return_unit : pint.Unit = units.Hz) -> pint.Quantity:
         """
-        Import the buffer from a file. The file format is determined by the file extension
-        Supported file formats are: 
-        * .bin: raw binary file
-        * .csv: comma-separated values file
-        * .npy: numpy binary file
-        * .npz: compressed numpy binary file
-        * .txt: whitespace-delimited text file
-        * .h5: hdf5 file format
+        Set the repetition rate of the pulse generator signal in a frequency unit
 
         Parameters
         ----------
-        filename : str
-            the name of the file that the buffer should be imported from
+        rate : pint.Quantity
+            The repetition rate in Hz
         
-        Raises
-        ------
-        ImportError
-            if the file format is not supported
+        Returns
+        -------
+        pint.Quantity
+            The repetition rate in Hz
         """
 
-        file_path = Path(filename)
-        if file_path.suffix == '.bin':
-            dtype = kwargs.get('dtype', self.numpy_type())
-            shape = kwargs.get('shape', (self.num_channels, self.buffer_size // self.num_channels))
-            buffer = np.fromfile(file_path, dtype=dtype)
-            self.buffer[:] = buffer.reshape(shape, order='C')
-        elif file_path.suffix == '.csv':
-            delimiter = kwargs.get('delimiter', ',')
-            self.buffer[:] = np.loadtxt(file_path, delimiter=delimiter)
-        elif file_path.suffix == '.npy':
-            self.buffer[:] = np.load(file_path)
-        elif file_path.suffix == '.npz':
-            data = np.load(file_path)
-            self.buffer[:] = data['arr_0']
-        elif file_path.suffix == '.txt':
-            self.buffer[:] = np.loadtxt(file_path)
-        elif file_path.suffix == '.h5' or file_path.suffix == '.hdf5':
-            with h5py.File(file_path, 'r') as f:
-                self.buffer[:] = f['data'][()]
-        else:
-            raise ImportError("File format not supported")
-
-    def avail_card_len(self, lAvailSamples : int = 0) -> None:
+        if rate is not None:
+            if isinstance(rate, pint.Quantity):
+                period = int(np.rint((self._get_clock(units.Hz) / rate).to_base_units().magnitude))
+            else:
+                raise ValueError("The rate must be a pint.Quantity")
+            self.period_length(period)
+        return_value = self.period_length()
+        return_value = UnitConversion.to_unit((self._get_clock(units.Hz) / return_value), return_unit)
+        return return_value
+    
+    def pulse_length(self, length : pint.Quantity, return_unit : pint.Unit = units.s) -> pint.Quantity:
         """
-        Set the amount of data that has been read out of the data buffer (see register `SPC_DATA_AVAIL_CARD_LEN` in the manual)
+        Set the pulse length of the pulse generator signal in a time unit
 
         Parameters
         ----------
-        lAvailSamples : int
-            the amount of data that is available for reading
+        length : pint.Quantity
+            The pulse length in seconds
+        
+        Returns
+        -------
+        pint.Quantity
+            The pulse length in seconds
         """
 
-        self.card.set_i(SPC_DATA_AVAIL_CARD_LEN, lAvailSamples * self.bytes_per_sample * self.num_channels)
+        if length is not None:
+            if isinstance(length, pint.Quantity):
+                length = int((length * self._get_clock(units.Hz)).to_base_units().magnitude)
+            else:
+                raise ValueError("The length must be a pint.Quantity")
+            self.high_length(length)
+        return_value = self.high_length()
+        return_value = UnitConversion.to_unit((return_value / self._get_clock(units.Hz)), return_unit)
+        return return_value
     
-    def avail_user_pos(self, bytes : bool = False) -> int:
+    def duty_cycle(self, duty_cycle : pint.Quantity = None, return_unit : pint.Unit = units.percent) -> pint.Quantity:
         """
-        Get the current position of the pointer in the data buffer (see register `SPC_DATA_AVAIL_USER_POS` in the manual)
+        Set the duty cycle of the pulse generator signal in a percentage unit
 
+        Parameters
+        ----------
+        duty_cycle : pint.Quantity
+            The duty cycle in percentage
+        
         Returns
         -------
-        int
-            pointer position
+        pint.Quantity
+            The duty cycle in percentage
         """
 
-        user_pos = self.card.get_i(SPC_DATA_AVAIL_USER_POS)
-        if not bytes:
-            user_pos = user_pos // self.bytes_per_sample // self.num_channels
-        return user_pos
+        period_length = self.period_length()
+        if duty_cycle is not None:
+            if isinstance(duty_cycle, pint.Quantity):
+                high_length = int(np.rint(period_length * duty_cycle))
+            else:
+                raise ValueError("The cycle must be a pint.Quantity")
+            self.high_length(high_length)
+        return_value = self.high_length()
+        return_value = UnitConversion.to_unit((return_value / period_length) * 100 * units.percent, return_unit)
+        return return_value
     
-    def avail_user_len(self, bytes : bool = False) -> int:
+    def start_delay(self, delay : pint.Unit = None, return_unit : pint.Unit = units.s) -> pint.Unit:
         """
-        Get the current length of the data in the data buffer (see register `SPC_DATA_AVAIL_USER_LEN` in the manual)
+        Set the start delay of the pulse generator signal in a time unit
 
+        Parameters
+        ----------
+        delay : pint.Unit
+            The start delay in a pint quantity with time unit
+        
         Returns
         -------
-        int
-            data length available
+        pint.Unit
+            The start delay in a pint quantity with time unit
         """
 
-        user_len = self.card.get_i(SPC_DATA_AVAIL_USER_LEN)
-        if not bytes:
-            user_len = user_len // self.bytes_per_sample // self.num_channels
-        return user_len
+        if delay is not None:
+            if isinstance(delay, pint.Quantity):
+                delay = int((delay * self._get_clock(units.Hz)).to_base_units().magnitude)
+            else:
+                raise ValueError("The delay must be a pint.Quantity")
+        return_value = self.delay(delay)
+        return_value = UnitConversion.to_unit((return_value / self._get_clock(units.Hz)), return_unit)
+        return return_value
     
-    def fill_size_promille(self) -> int:
+    repetitions = num_loops
+
+    def start_condition_state_signal(self, signal : int = 0, invert : bool = False) -> int:
         """
-        Get the fill size of the data buffer (see register `SPC_FILLSIZEPROMILLE` in the manual)
+        Set the start condition state signal of the pulse generator (see register 'SPC_XIO_PULSEGEN0_MUX1' in chapter `Pulse Generator` in the manual)
 
+        NOTE
+        ----
+        The Pulse Generator is started when the combined signal of both start condition signals are true and a rising edge
+        is detected. The invert parameter inverts the start condition state signal.
+        
+        Parameters
+        ----------
+        signal : int
+            The start condition state signal
+        invert : bool
+            Invert the start condition state signal
+        
         Returns
         -------
         int
-            fill size
+            The start condition state signal
         """
 
-        return self.card.get_i(SPC_FILLSIZEPROMILLE)
-    
-    def wait_dma(self) -> None:
-        """
-        Wait for the DMA transfer to finish (see register `M2CMD_DATA_WAITDMA` in the manual)
+        return_signal = self.mux1(signal)
+        return_invert = self.config()
+        if invert:
+            return_invert |= SPCM_PULSEGEN_CONFIG_MUX1_INVERT
+        else:
+            return_invert &= ~SPCM_PULSEGEN_CONFIG_MUX1_INVERT
+        return_invert = self.config(return_invert)
+        return return_signal, ((return_invert & SPCM_PULSEGEN_CONFIG_MUX1_INVERT) != 0)
+
+    def start_condition_trigger_signal(self, signal : int = 0, invert : bool = False) -> int:
         """
+        Set the start condition trigger signal of the pulse generator (see register 'SPC_XIO_PULSEGEN0_MUX2' in chapter `Pulse Generator` in the manual)
+
+        NOTE
+        ----
+        The Pulse Generator is started when the combined signal of both start condition signals are true and a rising edge
+        is detected. The invert parameter inverts the start condition state signal.
         
-        self.card.cmd(M2CMD_DATA_WAITDMA)
-    wait = wait_dma
+        Parameters
+        ----------
+        signal : int
+            The start condition trigger signal
+        invert : bool
+            Invert the start condition trigger signal
+        
+        Returns
+        -------
+        int
+            The start condition trigger signal
+        """
 
-    def numpy_type(self) -> npt.NDArray[np.int_]:
+        return_signal = self.mux2(signal)
+        return_invert = self.config()
+        if invert:
+            return_invert |= SPCM_PULSEGEN_CONFIG_MUX2_INVERT
+        else:
+            return_invert &= ~SPCM_PULSEGEN_CONFIG_MUX2_INVERT
+        return_invert = self.config(return_invert)
+        return return_signal, ((return_invert & SPCM_PULSEGEN_CONFIG_MUX2_INVERT) != 0)
+    
+    def invert_start_condition(self, invert : bool = None) -> bool:
         """
-        Get the type of numpy data from number of bytes
+        Invert the start condition of the pulse generator
 
+        Parameters
+        ----------
+        invert : bool
+            Invert the start condition
+        
         Returns
         -------
-        numpy data type
-            the type of data that is used by the card
+        bool
+            The start condition inversion
         """
 
-        if self._8bit_mode:
-            return np.uint8
-        if self._12bit_mode:
-            return np.int8
-        if self.bits_per_sample == 1:
-            if self.num_channels <= 8:
-                return np.uint8
-            elif self.num_channels <= 16:
-                return np.uint16
-            elif self.num_channels <= 32:
-                return np.uint32
-            return np.uint64
-        if self.bits_per_sample <= 8:
-            return np.int8
-        elif self.bits_per_sample <= 16:
-            return np.int16
-        elif self.bits_per_sample <= 32:
-            return np.int32
-        return np.int64
+        if invert is not None:
+            return_invert = self.config()
+            if invert:
+                return_invert |= SPCM_PULSEGEN_CONFIG_INVERT
+            else:
+                return_invert &= ~SPCM_PULSEGEN_CONFIG_INVERT
+            self.config(return_invert)
+        return ((self.config() & SPCM_PULSEGEN_CONFIG_INVERT) != 0)
 
-    # Data conversion mode
-    def data_conversion(self, mode : int = None) -> int:
+class PulseGenerators(CardFunctionality):
+    """
+    a higher-level abstraction of the CardFunctionality class to implement Pulse generator functionality
+
+    Parameters
+    ----------
+    generators : list[PulseGenerator]
+        a list of pulse generators
+    num_generators : int
+        the number of pulse generators on the card
+    """
+    
+    generators : list[PulseGenerator]
+    num_generators = 4
+
+    def __init__(self, card : Card, enable : int = 0, *args, **kwargs) -> None:
         """
-        Set the data conversion mode (see register `SPC_DATACONVERSION` in the manual)
-        
+        The constructor of the PulseGenerators class
+
         Parameters
         ----------
-        mode : int
-            the data conversion mode
+        card : Card
+            the card object that is used by the functionality
+        enable : int or bool
+            Enable or disable (all) the different pulse generators, by default all are turned off
+        
+        Raises
+        ------
+        SpcmException
         """
 
-        if mode is not None:
-            self.card.set_i(SPC_DATACONVERSION, mode)
-        mode = self.card.get_i(SPC_DATACONVERSION)
-        self._8bit_mode = (mode == SPCM_DC_12BIT_TO_8BIT or mode == SPCM_DC_14BIT_TO_8BIT or mode == SPCM_DC_16BIT_TO_8BIT)
-        self._12bit_mode = (mode == SPCM_DC_12BIT_TO_12BITPACKED)
-        self._bits_per_sample()
-        self._bytes_per_sample()
-        return mode
+        super().__init__(card, *args, **kwargs)
+        # Check for the pulse generator option on the card
+        features = self.card.get_i(SPC_PCIEXTFEATURES)
+        if features & SPCM_FEAT_EXTFW_PULSEGEN:
+            self.card._print(f"Pulse generator option available")
+        else:
+            raise SpcmException(text="This card doesn't have the pulse generator functionality installed. Please contact sales@spec.de to get more information about this functionality.")
+        
+        self.load()
+        self.enable(enable)
     
-    def avail_data_conversion(self) -> int:
+    def load(self) -> None:
+        """Load the pulse generators"""
+        self.generators = [PulseGenerator(self.card, i) for i in range(self.num_generators)]
+
+    # TODO in the next driver release there will be a register to get the number of pulse generators
+    def get_num_generators(self) -> int:
         """
-        Get the available data conversion modes (see register `SPC_AVAILDATACONVERSION` in the manual)
+        Get the number of pulse generators on the card
 
         Returns
         -------
         int
-            the available data conversion modes
+            The number of pulse generators
         """
-        return self.card.get_i(SPC_AVAILDATACONVERSION)
-    
-    # Iterator methods
-
-    _max_timeout = 64
 
-    _to_transfer_samples = 0
-    _current_samples = 0
-
-    def to_transfer_samples(self, samples: int) -> None:
+        return self.num_generators
+    
+    def __str__(self) -> str:
         """
-        This method sets the number of samples to transfer
-
-        Parameters
-        ----------
-        samples : int
-            the number of samples to transfer
+        String representation of the PulseGenerators class
+    
+        Returns
+        -------
+        str
+            String representation of the PulseGenerators class
         """
-        self._to_transfer_samples = samples
+        
+        return f"PulseGenerators(card={self.card})"
+    
+    __repr__ = __str__
     
-    def __iter__(self):
+
+    def __iter__(self) -> "PulseGenerators":
+        """Define this class as an iterator"""
+        return self
+    
+    def __getitem__(self, index : int) -> PulseGenerator:
         """
-        This method is called when the iterator is initialized
+        Get the pulse generator at the given index
 
+        Parameters
+        ----------
+        index : int
+            The index of the pulse generator
+        
         Returns
         -------
-        DataIterator
-            the iterator itself
+        PulseGenerator
+            The pulse generator at the given index
         """
-        return self
+
+        return self.generators[index]
     
-    def __next__(self) -> npt.ArrayLike:
+    _generator_iterator_index = -1
+    def __next__(self) -> PulseGenerator:
         """
         This method is called when the next element is requested from the iterator
 
         Returns
         -------
-        npt.ArrayLike
-            the next data block
+        PulseGenerator
+            the next available pulse generator
         
         Raises
         ------
         StopIteration
         """
-        timeout_counter = 0
-        while True:
-            try:
-                # print(self.card.status())
-                self.wait_dma()
-            except SpcmTimeout:
-                self.card._print("... Timeout ({})".format(timeout_counter), end='\r')
-                timeout_counter += 1
-                if timeout_counter > self._max_timeout:
-                    raise StopIteration
-            else:
-                user_len = self.avail_user_len()
-                user_pos = self.avail_user_pos()
+        self._generator_iterator_index += 1
+        if self._generator_iterator_index >= len(self.channels):
+            self._generator_iterator_index = -1
+            raise StopIteration
+        return self.generators[self._generator_iterator_index]
+    
+    def __len__(self) -> int:
+        """Returns the number of available pulse generators"""
+        return len(self.generators)
+    
+    def write_setup(self) -> None:
+        """Write the setup to the card"""
+        self.card.write_setup()
+
+    # The pulse generator can be enabled or disabled
+    def enable(self, enable : int = None) -> int:
+        """
+        Enable or disable (all) the pulse generators (see register 'SPC_XIO_PULSEGEN_ENABLE' in chapter `Pulse Generator` in the manual)
 
-                self._current_samples += self._notify_samples
-                if self._to_transfer_samples != 0 and self._to_transfer_samples < self._current_samples:
-                    raise StopIteration
+        Parameters
+        ----------
+        enable : int or bool
+            Enable or disable (all) the different pulse generators, by default all are turned off
+        
+        Returns
+        -------
+        int
+            The enable state of the pulse generators
+        """
 
-                fill_size = self.fill_size_promille()
-                self.card._print("Fill size: {}%  Pos:{:08x} Len:{:08x} Total:{:.2f} MiS / {:.2f} MiS".format(fill_size/10, user_pos, user_len, self._current_samples / MEBI(1), self._to_transfer_samples / MEBI(1)), end='\r')
+        
+        if isinstance(enable, bool):
+            enable = (1 << self.num_generators) - 1 if enable else 0
+        if enable is not None:
+            self.card.set_i(SPC_XIO_PULSEGEN_ENABLE, enable)
+        return self.card.get_i(SPC_XIO_PULSEGEN_ENABLE)
+    
+    def cmd(self, cmd : int) -> None:
+        """
+        Execute a command on the pulse generator (see register 'SPC_XIO_PULSEGEN_COMMAND' in chapter `Pulse Generator` in the manual)
+
+        Parameters
+        ----------
+        cmd : int
+            The command to execute
+        """
+        self.card.set_i(SPC_XIO_PULSEGEN_COMMAND, cmd)
+    
+    def force(self) -> None:
+        """
+        Generate a single rising edge, that is common for all pulse generator engines. This allows to start/trigger the output 
+        of all enabled pulse generators synchronously by issuing a software command. (see register 'SPC_XIO_PULSEGEN_COMMAND' in chapter `Pulse Generator` in the manual)
+        """
+        self.cmd(SPCM_PULSEGEN_CMD_FORCE)
+    
+    def write_setup(self) -> None:
+        """Write the setup of the pulse generator to the card"""
+        self.card.write_setup()
+    
+    # The clock rate in Hz of the pulse generator
+    def get_clock(self) -> int:
+        """
+        Get the clock rate of the pulse generator (see register 'SPC_XIO_PULSEGEN_CLOCK' in chapter `Pulse Generator` in the manual)
+
+        Returns
+        -------
+        int
+            The clock rate in Hz
+        """
+        return self.card.get_i(SPC_XIO_PULSEGEN_CLOCK)
+    
 
-                self.avail_card_len(self._notify_samples)
-                return self.buffer[:, user_pos:user_pos+self._notify_samples]
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `spcm-1.0.6/src/spcm/classes_dds.py` & `spcm-1.1.0/src/spcm/classes_dds.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,58 @@
 # -*- coding: utf-8 -*-
 
 from .constants import *
 
 from .classes_error_exception import SpcmException
 from .classes_functionality import CardFunctionality
+from .classes_channels import Channels, Channel
+
+from .classes_unit_conversion import UnitConversion
+from . import units
 
 import ctypes
 
 class DDSCore:
     """
     a class for controlling a single DDS core
     """
 
     dds : "DDS"
     index : int
+    channel : Channel
 
     def __init__(self, core_index, dds, *args, **kwargs) -> None:
         self.dds = dds
         self.index = core_index
+        self.channel = kwargs.get("channel", None)
     
     def __int__(self) -> int:
         """
         get the index of the core
 
         Returns
         -------
         int
             the index of the core
         """
         return self.index
     __index__ = __int__
 
+    def __str__(self) -> str:
+        """
+        get the string representation of the core
+
+        Returns
+        -------
+        str
+            the string representation of the core
+        """
+        return f"Core {self.index}"
+    __repr__ = __str__
+
     def __add__(self, other) -> int:
         """
         add the index of the core to another index
 
         Parameters
         ----------
         other : int
@@ -50,142 +68,184 @@
     # DDS "static" parameters
     def amp(self, amplitude : float) -> None:
         """
         set the amplitude of the sine wave of a specific core (see register `SPC_DDS_CORE0_AMP` in the manual)
         
         Parameters
         ----------
-        amplitude : float
+        amplitude : float | pint.Quantity
             the value between 0 and 1 corresponding to the amplitude
         """
 
+        if self.channel is not None:
+            amplitude = self.channel.to_amplitude_fraction(amplitude)
+        elif isinstance(amplitude, units.Quantity) and amplitude.check("[]"):
+            amplitude = UnitConversion.convert(amplitude, units.fraction, float, rounding=None)
         self.dds.set_d(SPC_DDS_CORE0_AMP + self.index, float(amplitude))
     # aliases
     amplitude = amp
 
-    def get_amp(self) -> float:
+    def get_amp(self, return_unit = None) -> float:
         """
         gets the amplitude of the sine wave of a specific core (see register `SPC_DDS_CORE0_AMP` in the manual)
 
+        Parameters
+        ----------
+        return_unit : pint.Unit = None
+            the unit of the returned amplitude, by default None
+
         Returns
         -------
         float
             the value between 0 and 1 corresponding to the amplitude
         """
 
-        return self.dds.card.get_d(SPC_DDS_CORE0_AMP + self.index)
+        return_value = self.dds.card.get_d(SPC_DDS_CORE0_AMP + self.index)
+        if self.channel is not None:
+            return_value = self.channel.from_amplitude_fraction(return_value, return_unit)
+        else:
+            return_value = UnitConversion.to_unit(return_value, return_unit)
+        return return_value
     # aliases
     get_amplitude = get_amp
 
     def freq(self, frequency : float) -> None:
         """
         set the frequency of the sine wave of a specific core (see register `SPC_DDS_CORE0_FREQ` in the manual)
         
         Parameters
         ----------
-        frequency : float
+        frequency : float | pint.Quantity
             the value of the frequency in Hz
         """
 
+        frequency = UnitConversion.convert(frequency, units.Hz, float, rounding=None)
         self.dds.set_d(SPC_DDS_CORE0_FREQ + self.index, float(frequency))
     # aliases
     frequency = freq
 
-    def get_freq(self) -> float:
+    def get_freq(self, return_unit = None) -> float:
         """
         gets the frequency of the sine wave of a specific core (see register `SPC_DDS_CORE0_FREQ` in the manual)
         
+        Parameters
+        ----------
+        return_unit : pint.Unit = None
+            the unit of the returned frequency, by default None
+
         Returns
         -------
-        float
+        float | pint.Quantity
             the value of the frequency in Hz the specific core
         """
 
-        return self.dds.card.get_d(SPC_DDS_CORE0_FREQ + self.index)
+        return_value = self.dds.card.get_d(SPC_DDS_CORE0_FREQ + self.index)
+        if return_unit is not None: return_value = UnitConversion.to_unit(return_value * units.Hz, return_unit)
+        return return_value
     # aliases
     get_frequency = get_freq
 
     def phase(self, phase : float) -> None:
         """
         set the phase of the sine wave of a specific core (see register `SPC_DDS_CORE0_PHASE` in the manual)
         
         Parameters
         ----------
-        phase : float
+        phase : float | pint.Quantity
             the value between 0 and 360 degrees of the phase
         """
 
+        phase = UnitConversion.convert(phase, units.deg, float, rounding=None)
         self.dds.set_d(SPC_DDS_CORE0_PHASE + self.index, float(phase))
 
-    def get_phase(self) -> float:
+    def get_phase(self, return_unit = None) -> float:
         """
         gets the phase of the sine wave of a specific core (see register `SPC_DDS_CORE0_PHASE` in the manual)
         
         Returns
         -------
         float
             the value between 0 and 360 degrees of the phase
         """
 
-        return self.dds.card.get_d(SPC_DDS_CORE0_PHASE + self.index)
+        return_value = self.dds.card.get_d(SPC_DDS_CORE0_PHASE + self.index)
+        if return_unit is not None: return_value = UnitConversion.to_unit(return_value * units.deg, return_unit)
+        return return_value
 
     # DDS dynamic parameters
     def freq_slope(self, slope : float) -> None:
         """
         set the frequency slope of the linearly changing frequency of the sine wave of a specific core (see register `SPC_DDS_CORE0_FREQ_SLOPE` in the manual)
         
         Parameters
         ----------
-        slope : float
-            the rate of frequency change in Hz/s
+        slope : float | pint.Quantity
+            the rate of frequency change in Hz/s (positive or negative) or specified unit
         """
 
+        slope = UnitConversion.convert(slope, units.Hz/units.s, float, rounding=None)
         self.dds.set_d(SPC_DDS_CORE0_FREQ_SLOPE + self.index, float(slope))
     # aliases
     frequency_slope = freq_slope
 
-    def get_freq_slope(self) -> float:
+    def get_freq_slope(self, return_unit = None) -> float:
         """
         get the frequency slope of the linearly changing frequency of the sine wave of a specific core (see register `SPC_DDS_CORE0_FREQ_SLOPE` in the manual)
         
+        Parameters
+        ----------
+        return_unit : pint.Unit = None
+            the unit of the returned frequency slope, by default None
+
         Returns
         -------
         float
             the rate of frequency change in Hz/s
         """
 
-        return self.dds.card.get_d(SPC_DDS_CORE0_FREQ_SLOPE + self.index)
+        return_value = self.dds.card.get_d(SPC_DDS_CORE0_FREQ_SLOPE + self.index)
+        if return_unit is not None: return_value = UnitConversion.to_unit(return_value * units.Hz/units.s, return_unit)
+        return return_value
     # aliases
     get_frequency_slope = get_freq_slope
 
     def amp_slope(self, slope : float) -> None:
         """
         set the amplitude slope of the linearly changing amplitude of the sine wave of a specific core (see register `SPC_DDS_CORE0_AMP_SLOPE` in the manual)
         
         Parameters
         ----------
-        slope : float
-            the rate of amplitude change in 1/s
+        slope : float | pint.Quantity
+            the rate of amplitude change in 1/s (positive or negative) or specified unit
         """
 
+        slope = UnitConversion.convert(slope, 1/units.s, float, rounding=None)
         self.dds.set_d(SPC_DDS_CORE0_AMP_SLOPE + self.index, float(slope))
     # aliases
     amplitude_slope = amp_slope
 
-    def get_amp_slope(self) -> float:
+    def get_amp_slope(self, return_unit = None) -> float:
         """
         set the amplitude slope of the linearly changing amplitude of the sine wave of a specific core (see register `SPC_DDS_CORE0_AMP_SLOPE` in the manual)
         
+        Parameters
+        ----------
+        return_unit : pint.Unit = None
+            the unit of the returned amplitude slope, by default None
+
         Returns
         -------
         float
             the rate of amplitude change in 1/s
         """
 
-        self.dds.card.get_d(SPC_DDS_CORE0_AMP_SLOPE + self.index)
+
+        return_value = self.dds.card.get_d(SPC_DDS_CORE0_AMP_SLOPE + self.index)
+        if return_unit is not None: return_value = UnitConversion.to_unit(return_value / units.s, return_unit)
+        return return_value
     # aliases
     amplitude_slope = amp_slope
 
 
 class DDS(CardFunctionality):
     """a higher-level abstraction of the SpcmCardFunctionality class to implement DDS functionality
 
@@ -230,36 +290,53 @@
     also the trigger source setting happens when a trigger comes. Hence a change of
     the trigger mode only happens after an 'arm()' command was send and an internal trigger was
     received.
  
     """
 
     cores : list[DDSCore] = []
+    channels : Channels = None
 
     _dtm : int = 0
     _register_list : ctypes._Pointer
     _rl_size : int = MEBI(2)
     _rl_current : int = 0
 
     _current_core : int = -1
 
+    _channel_from_core : dict[int, int] = {}
+
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
+        self.channels = kwargs.get("channels", None)
         self.cores = []
         self.load_cores()
     
     def load_cores(self):
         """
         load the cores of the DDS functionality
         """
 
         self.cores = []
         num_cores = self.num_cores()
+        
+        if self.channels is not None:
+            for channel in self.channels:
+                cores_on_channel = self.get_cores_on_channel(channel.index)
+                for core in range(num_cores):
+                    if cores_on_channel & (1 << core):
+                        self._channel_from_core[core] = channel
+                    # else:
+                    #     self._channel_from_core[core] = None
+        
         for core in range(num_cores):
-            self.cores.append(DDSCore(core, self))
+            if core in self._channel_from_core:
+                self.cores.append(DDSCore(core, self, channel=self._channel_from_core[core]))
+            else:
+                self.cores.append(DDSCore(core, self))
         
     def __len__(self) -> int:
         """
         get the number of cores
 
         Returns
         -------
@@ -483,14 +560,16 @@
 
         Parameters
         ----------
         channel : int
             the channel number
         *args : int
             the cores that are connected to the channel
+        
+        TODO: change the channel associated with each core
         """
 
         mask = 0
         for core in args:
             mask |= core
         self.set_i(SPC_DDS_CORES_ON_CH0 + channel, mask)
     
@@ -561,35 +640,43 @@
 
         NOTE
         ----
         only used in conjecture with the trigger source set to SPCM_DDS_TRG_SRC_TIMER ---
         
         Parameters
         ----------
-        period : float
+        period : float | pint.Quantity
             the time between DDS trigger events in seconds
         """
 
+        period = UnitConversion.convert(period, units.s, float, rounding=None)
         self.set_d(SPC_DDS_TRG_TIMER, float(period))
     
-    def get_trg_timer(self) -> float:
+    def get_trg_timer(self, return_unit = None) -> float:
         """
         get the period at which the timer should raise DDS trigger events. (see register `SPC_DDS_TRG_TIMER` in the manual)
 
         NOTE
         ----
         only used in conjecture with the trigger source set to SPCM_DDS_TRG_SRC_TIMER ---
+
+        Parameters
+        ----------
+        return_unit : pint.Unit = None
+            the unit of the returned time between DDS trigger events, by default None
         
         Returns
         ----------
         float
             the time between DDS trigger events in seconds
         """
 
-        return self.card.get_d(SPC_DDS_TRG_TIMER)
+        return_value = self.card.get_d(SPC_DDS_TRG_TIMER)
+        if return_unit is not None: return_value = UnitConversion.to_unit(return_value * units.s, return_unit)
+        return return_value
 
     def x_mode(self, xio : int, mode : int) -> None:
         """
         setup the kind of output that the XIO outputs will give (see register `SPC_DDS_X0_MODE` in the manual)
 
         Parameters
         ----------
@@ -717,66 +804,74 @@
             self.cores[core_index].amp(amplitude)
         else:
             raise TypeError("amp() takes 1 or 2 positional arguments ({} given)".format(len(args) + 1))
         # self.set_d(SPC_DDS_CORE0_AMP + core_index, float(amplitude))
     # aliases
     amplitude = amp
 
-    def get_amp(self, core_index : int) -> float:
+    def get_amp(self, core_index : int, return_unit = None) -> float:
         """
         gets the amplitude of the sine wave of a specific core (see register `SPC_DDS_CORE0_AMP` in the manual)
         
         Parameters
         ----------
         core_index : int
             the index of the core to be changed
+        return_unit : pint.Unit = None
+            the unit of the returned amplitude, by default None
 
         Returns
         -------
-        float
-            the value between 0 and 1 corresponding to the amplitude
+        float | pint.Quantity
+            the value between 0 and 1 corresponding to the amplitude of the specific core or in the specified unit
         """
 
-        return self.cores[core_index].get_amp()
+        return self.cores[core_index].get_amp(return_unit)
         # return self.card.get_d(SPC_DDS_CORE0_AMP + core_index)
     # aliases
     get_amplitude = get_amp
 
     def avail_amp_min(self) -> float:
         """
         get the minimum available amplitude (see register `SPC_DDS_AVAIL_AMP_MIN` in the manual)
 
         Returns
         -------
         float
             the minimum available amplitude
+        
+        TODO: unitize!
         """
 
         return self.card.get_d(SPC_DDS_AVAIL_AMP_MIN)
     
     def avail_amp_max(self) -> float:
         """
         get the maximum available amplitude (see register `SPC_DDS_AVAIL_AMP_MAX` in the manual)
 
         Returns
         -------
         float
             the maximum available amplitude
+        
+        TODO: unitize!
         """
 
         return self.card.get_d(SPC_DDS_AVAIL_AMP_MAX)
     
     def avail_amp_step(self) -> float:
         """
         get the step size of the available amplitudes (see register `SPC_DDS_AVAIL_AMP_STEP` in the manual)
 
         Returns
         -------
         float
             the step size of the available amplitudes
+        
+        TODO: unitize!
         """
 
         return self.card.get_d(SPC_DDS_AVAIL_AMP_STEP)
 
     # def freq(self, core_index : int, frequency : float) -> None:
     def freq(self, *args) -> None:
         """
@@ -799,65 +894,73 @@
             self.cores[core_index].freq(frequency)
         else:
             raise TypeError("freq() takes 1 or 2 positional arguments ({} given)".format(len(args) + 1))
         # self.set_d(SPC_DDS_CORE0_FREQ + core_index, float(frequency))
     # aliases
     frequency = freq
 
-    def get_freq(self, core_index : int) -> float:
+    def get_freq(self, core_index : int, return_unit = None) -> float:
         """
         gets the frequency of the sine wave of a specific core (see register `SPC_DDS_CORE0_FREQ` in the manual)
         
         Parameters
         ----------
         core_index : int
             the index of the core to be changed
+        return_unit : pint.Unit = None
+            the unit of the returned frequency, by default None
         
         Returns
         -------
-        float
-            the value of the frequency in Hz the specific core
+        float | pint.Quantity
+            the value of the frequency in Hz the specific core or in the specified unit
         """
 
-        return self.cores[core_index].get_freq()
+        return self.cores[core_index].get_freq(return_unit)
     # aliases
     get_frequency = get_freq
 
     def avail_freq_min(self) -> float:
         """
         get the minimum available frequency (see register `SPC_DDS_AVAIL_FREQ_MIN` in the manual)
 
         Returns
         -------
         float
             the minimum available frequency
+        
+        TODO: unitize!
         """
 
         return self.card.get_d(SPC_DDS_AVAIL_FREQ_MIN)
     
     def avail_freq_max(self) -> float:
         """
         get the maximum available frequency (see register `SPC_DDS_AVAIL_FREQ_MAX` in the manual)
 
         Returns
         -------
         float
             the maximum available frequency
+        
+        TODO: unitize!
         """
 
         return self.card.get_d(SPC_DDS_AVAIL_FREQ_MAX)
     
     def avail_freq_step(self) -> float:
         """
         get the step size of the available frequencies (see register `SPC_DDS_AVAIL_FREQ_STEP` in the manual)
 
         Returns
         -------
         float
             the step size of the available frequencies
+        
+        TODO: unitize!
         """
 
         return self.card.get_d(SPC_DDS_AVAIL_FREQ_STEP)
 
     # def phase(self, core_index : int, phase : float) -> None:
     def phase(self, *args) -> None:
         """
@@ -877,65 +980,72 @@
                 core.phase(phase)
         elif len(args) == 2:
             core_index, phase = args
             self.cores[core_index].phase(phase)
         else:
             raise TypeError("phase() takes 1 or 2 positional arguments ({} given)".format(len(args) + 1))
         # self.set_d(SPC_DDS_CORE0_PHASE + core_index, float(phase))
-        self.set_d(SPC_DDS_CORE0_PHASE + core_index, float(phase))
 
-    def get_phase(self, core_index : int) -> float:
+    def get_phase(self, core_index : int, return_unit = None) -> float:
         """
         gets the phase of the sine wave of a specific core (see register `SPC_DDS_CORE0_PHASE` in the manual)
         
         Parameters
         ----------
         core_index : int
             the index of the core to be changed
+        return_unit : pint.Unit = None
+            the unit of the returned phase, by default None
         
         Returns
         -------
         float
             the value between 0 and 360 degrees of the phase
         """
 
-        return self.card.get_d(SPC_DDS_CORE0_PHASE + core_index)
-    
+        return self.cores[core_index].get_phase(return_unit)
+      
     def avail_phase_min(self) -> float:
         """
         get the minimum available phase (see register `SPC_DDS_AVAIL_PHASE_MIN` in the manual)
 
         Returns
         -------
         float
             the minimum available phase
+        
+        TODO: unitize!
         """
 
         return self.card.get_d(SPC_DDS_AVAIL_PHASE_MIN)
     
     def avail_phase_max(self) -> float:
         """
         get the maximum available phase (see register `SPC_DDS_AVAIL_PHASE_MAX` in the manual)
 
         Returns
         -------
         float
             the maximum available phase
+        
+        TODO: unitize!
         """
 
         return self.card.get_d(SPC_DDS_AVAIL_PHASE_MAX)
     
     def avail_phase_step(self) -> float:
         """
         get the step size of the available phases (see register `SPC_DDS_AVAIL_PHASE_STEP` in the manual)
 
         Returns
         -------
         float
             the step size of the available phases
+        
+        TODO: unitize!
         """
 
         return self.card.get_d(SPC_DDS_AVAIL_PHASE_STEP)
 
     def x_manual_output(self, state_mask : int) -> None:
         """
         set the output of the xio channels using a bit mask (see register `SPC_DDS_X_MANUAL_OUTPUT` in the manual)
@@ -983,65 +1093,73 @@
             self.cores[core_index].freq_slope(slope)
         else:
             raise TypeError("freq_slope() takes 1 or 2 positional arguments ({} given)".format(len(args) + 1))
         # self.set_d(SPC_DDS_CORE0_FREQ_SLOPE + core_index, float(slope))
     # aliases
     frequency_slope = freq_slope
 
-    def get_freq_slope(self, core_index : int) -> float:
+    def get_freq_slope(self, core_index : int, return_unit=None) -> float:
         """
         get the frequency slope of the linearly changing frequency of the sine wave of a specific core (see register `SPC_DDS_CORE0_FREQ_SLOPE` in the manual)
         
         Parameters
         ----------
         core_index : int
             the index of the core to be changed
+        return_unit : pint.Unit = None
+            the unit of the returned frequency slope, by default None
         
         Returns
         -------
         float
             the rate of frequency change in Hz/s
         """
 
-        return self.card.get_d(SPC_DDS_CORE0_FREQ_SLOPE + core_index)
+        return self.cores[core_index].get_freq_slope(return_unit)
     # aliases
     get_frequency_slope = get_freq_slope
 
     def avail_freq_slope_min(self) -> float:
         """
         get the minimum available frequency slope (see register `SPC_DDS_AVAIL_FREQ_SLOPE_MIN` in the manual)
 
         Returns
         -------
         float
             the minimum available frequency slope
+        
+        TODO: unitize!
         """
 
         return self.card.get_d(SPC_DDS_AVAIL_FREQ_SLOPE_MIN)
     
     def avail_freq_slope_max(self) -> float:
         """
         get the maximum available frequency slope (see register `SPC_DDS_AVAIL_FREQ_SLOPE_MAX` in the manual)
 
         Returns
         -------
         float
             the maximum available frequency slope
+        
+        TODO: unitize!
         """
 
         return self.card.get_d(SPC_DDS_AVAIL_FREQ_SLOPE_MAX)
     
     def avail_freq_slope_step(self) -> float:
         """
         get the step size of the available frequency slopes (see register `SPC_DDS_AVAIL_FREQ_SLOPE_STEP` in the manual)
 
         Returns
         -------
         float
             the step size of the available frequency slopes
+        
+        TODO: unitize!
         """
 
         return self.card.get_d(SPC_DDS_AVAIL_FREQ_SLOPE_STEP)
 
     # def amp_slope(self, core_index : int, slope : float) -> None:
     def amp_slope(self, *args) -> None:
         """
@@ -1064,65 +1182,73 @@
             self.cores[core_index].amp_slope(slope)
         else:
             raise TypeError("amp_slope() takes 1 or 2 positional arguments ({} given)".format(len(args) + 1))
         # self.set_d(SPC_DDS_CORE0_AMP_SLOPE + core_index, float(slope))
     # aliases
     amplitude_slope = amp_slope
 
-    def get_amp_slope(self, core_index : int) -> float:
+    def get_amp_slope(self, core_index : int, return_unit = None) -> float:
         """
         set the amplitude slope of the linearly changing amplitude of the sine wave of a specific core (see register `SPC_DDS_CORE0_AMP_SLOPE` in the manual)
         
         Parameters
         ----------
         core_index : int
             the index of the core to be changed
+        return_unit : pint.Unit = None
+            the unit of the returned amplitude slope, by default None
         
         Returns
         -------
         float
             the rate of amplitude change in 1/s
         """
 
-        self.card.get_d(SPC_DDS_CORE0_AMP_SLOPE + core_index)
+        return self.cores[core_index].get_amp_slope(return_unit)
     # aliases
     amplitude_slope = amp_slope
 
     def avail_amp_slope_min(self) -> float:
         """
         get the minimum available amplitude slope (see register `SPC_DDS_AVAIL_AMP_SLOPE_MIN` in the manual)
 
         Returns
         -------
         float
             the minimum available amplitude slope
+        
+        TODO: unitize!
         """
 
         return self.card.get_d(SPC_DDS_AVAIL_AMP_SLOPE_MIN)
     
     def avail_amp_slope_max(self) -> float:
         """
         get the maximum available amplitude slope (see register `SPC_DDS_AVAIL_AMP_SLOPE_MAX` in the manual)
 
         Returns
         -------
         float
             the maximum available amplitude slope
+        
+        TODO: unitize!
         """
 
         return self.card.get_d(SPC_DDS_AVAIL_AMP_SLOPE_MAX)
     
     def avail_amp_slope_step(self) -> float:
         """
         get the step size of the available amplitude slopes (see register `SPC_DDS_AVAIL_AMP_SLOPE_STEP` in the manual)
 
         Returns
         -------
         float
             the step size of the available amplitude slopes
+        
+        TODO: unitize!
         """
 
         return self.card.get_d(SPC_DDS_AVAIL_AMP_SLOPE_STEP)
 
     # DDS control
     def cmd(self, command : int) -> None:
         """
```

### Comparing `spcm-1.0.6/src/spcm/classes_device.py` & `spcm-1.1.0/src/spcm/classes_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from .pyspcm import (int64, c_double, c_void_p, create_string_buffer, spcm_hOpen, spcm_vClose, 
                      spcm_dwGetParam_i64, spcm_dwSetParam_i64, 
                      spcm_dwGetParam_d64, spcm_dwSetParam_d64,
                      spcm_dwGetParam_ptr, spcm_dwSetParam_ptr,
                     byref)
 
 from .classes_error_exception import SpcmError, SpcmException, SpcmTimeout
+from .classes_unit_conversion import UnitConversion
+from . import units
 
 
 class Device():
     """
     a class to control the low-level API interface of Spectrum Instrumentation devices
 
     For more information about what setups are available, please have a look at the user manual
@@ -64,14 +66,15 @@
         handle = False
             directly supply the object with an existing handle
         """
         self.device_identifier = device_identifier
         self._handle = handle
         self._kwargs = kwargs
         self._throw_error = kwargs.get("throw_error", True)
+        self._verbose = kwargs.get("verbose", False)
     
     def __del__(self) -> None:
         """Destructor that closes the connection associated with the handle"""
         if not self._closed:
             self.stop()
             self._closed = True
             self.close(self._handle)
@@ -266,15 +269,16 @@
         """
 
         cmd = 0
         for arg in args:
             cmd |= arg
         self.set_i(SPC_M2CMD, cmd)
     
-    def timeout(self, timeout : int = None) -> int:
+    #@Decorators.unitize(units.ms, "timeout", int)
+    def timeout(self, timeout : int = None, return_unit = None) -> int:
         """
         Sets the timeout in ms (see register `SPC_TIMEOUT` in the manual)
         
         Parameters
         ----------
         timeout : int
             The timeout in ms
@@ -282,16 +286,19 @@
         Returns
         -------
         int
             returns the current timeout in ms
         """
 
         if timeout is not None:
+            timeout = UnitConversion.convert(timeout, units.ms, int)
             self.set_i(SPC_TIMEOUT, timeout)
-        return self.get_i(SPC_TIMEOUT)
+        return_value = self.get_i(SPC_TIMEOUT)
+        if return_unit is not None: return_value = UnitConversion.to_unit(return_value, return_unit)
+        return return_value
     
     def start(self, *args) -> None:
         """
         Starts the connected card and enables triggering on the card (see command `M2CMD_CARD_START` in the manual)
 
         Parameters
         ----------
@@ -516,21 +523,30 @@
         if self._closed:
             error_text = "The connection to the card has been closed. Please reopen the connection before sending commands."
             if self._throw_error:
                 raise SpcmException(text=error_text)
             else:
                 self._print(error_text)
     
-    def _print(self, text : str, **kwargs) -> None:
+    def _print(self, text : str, verbose : bool = False, **kwargs) -> None:
         """
         Print information
+
+        Parameters
+        ----------
+        text : str
+            The text that is printed
+        verbose : bool
+            A boolean that indicates if the text should forced to be printed
+        **kwargs
+            Additional parameters that are passed to the print function
     
         """
 
-        if self._verbose:
+        if self._verbose or verbose:
             print(text, **kwargs)
 
     def open(self, device_identifier : str) -> None:
         """
         Open a connection to the card and return the handle (see the user manual of your specific device on how to find out the device_identifier string)
     
         Parameters
```

### Comparing `spcm-1.0.6/src/spcm/classes_error_exception.py` & `spcm-1.1.0/src/spcm/classes_error_exception.py`

 * *Files identical despite different names*

### Comparing `spcm-1.0.6/src/spcm/classes_functionality.py` & `spcm-1.1.0/src/spcm/classes_functionality.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class CardFunctionality:
     """
     A prototype class for card specific functionality that needs it's own namespace
     """
     card : Card
     function_type = 0
 
-    def __init__(self, card : Card) -> None:
+    def __init__(self, card : Card, *args, **kwargs) -> None:
         """
         Takes a Card object that is used by the functionality
 
         Parameters
         ----------
         card : Card
             a Card object on which the functionality works
```

### Comparing `spcm-1.0.6/src/spcm/classes_multi.py` & `spcm-1.1.0/src/spcm/classes_multi.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 import numpy as np
 import numpy.typing as npt
 
 from .constants import *
 
 from .classes_data_transfer import DataTransfer
 
+from .classes_unit_conversion import UnitConversion
+from . import units
+
 from .classes_error_exception import SpcmTimeout
 
 class Multi(DataTransfer):
     """a high-level class to control Multiple Recording and Replay functionality on Spectrum Instrumentation cards
 
     For more information about what setups are available, please have a look at the user manual
     for your specific card.
@@ -30,44 +33,83 @@
     def segment_samples(self, segment_size : int = None) -> None:
         """
         Sets the memory size in samples per channel. The memory size setting must be set before transferring 
         data to the card. (see register `SPC_MEMSIZE` in the manual)
         
         Parameters
         ----------
-        segment_size : int
-            the size of a single segment in memory in Bytes
+        segment_size : int | pint.Quantity
+            the size of a single segment in memory in Samples
         """
 
         if segment_size is not None:
+            segment_size = UnitConversion.convert(segment_size, units.S, int)
             self.card.set_i(SPC_SEGMENTSIZE, segment_size)
         segment_size = self.card.get_i(SPC_SEGMENTSIZE)
         self._segment_size = segment_size
     
+    def post_trigger(self, num_samples : int = None) -> int:
+        """
+        Set the number of post trigger samples (see register `SPC_POSTTRIGGER` in the manual)
+        
+        Parameters
+        ----------
+        num_samples : int | pint.Quantity
+            the number of post trigger samples
+        
+        Returns
+        -------
+        int
+            the number of post trigger samples
+        """
+
+        post_trigger = super().post_trigger(num_samples)
+        self._pre_trigger = self._segment_size - post_trigger
+        return post_trigger
+
     def allocate_buffer(self, segment_samples : int, num_segments : int = None) -> None:
-        """Memory allocation for the buffer that is used for communicating with the card
+        """
+        Memory allocation for the buffer that is used for communicating with the card
 
         Parameters
         ----------
-        segment_samples : int = None
+        segment_samples : int | pint.Quantity
             use the number of samples and get the number of active channels and bytes per samples directly from the card
-        num_segments : int
+        num_segments : int = None
             the number of segments that are used for the multiple recording mode
         """
         
+        segment_samples = UnitConversion.convert(segment_samples, units.S, int)
+        num_segments = UnitConversion.convert(num_segments, units.S, int)
         self.segment_samples(segment_samples)
         if num_segments is None:
             self._num_segments = self._memory_size // segment_samples
         else:
             self._num_segments = num_segments
         super().allocate_buffer(segment_samples * self._num_segments)
         num_channels = self.card.active_channels()
         if self.bits_per_sample > 1 and not self._12bit_mode:
-            self.buffer = self.buffer.reshape((self._num_segments, num_channels, segment_samples), order='F')
+            self.buffer = self.buffer.reshape((self._num_segments, segment_samples, num_channels), order='C') # index definition: [segment, sample, channel] !
     
+    def time_data(self, total_num_samples : int = None) -> npt.NDArray[np.float_]:
+        """
+        Get the time array for the data buffer
+        
+        Returns
+        -------
+        numpy array
+            the time array
+        """
+
+        sample_rate = self._sample_rate()
+        if total_num_samples is None:
+            total_num_samples = self._num_samples // self._num_segments
+        total_num_samples = UnitConversion.convert(total_num_samples, units.Sa, int)
+        return (np.arange(total_num_samples) - self._pre_trigger) / sample_rate
+
     def unpack_12bit_buffer(self) -> npt.NDArray[np.int_]:
         """
         Unpacks the 12-bit packed data to 16-bit data
 
         Returns
         -------
         npt.NDArray[np.int_]
@@ -86,14 +128,15 @@
         npt.ArrayLike
             the next data block
         
         Raises
         ------
         StopIteration
         """
+        
         timeout_counter = 0
         # notify the card that data is available or read, but only after the first block
         if self._current_samples >= self._notify_samples:
             self.avail_card_len(self._notify_samples)
         while True:
             try:
                 self.wait_dma()
@@ -104,18 +147,18 @@
                     raise StopIteration
             else:
                 user_len = self.avail_user_len()
                 user_pos = self.avail_user_pos()
 
                 current_segment = user_pos // self._segment_size
                 current_pos_in_segment = user_pos % self._segment_size
-                final_segment = ((user_pos+user_len) // self._segment_size) + 1
+                final_segment = ((user_pos+user_len) // self._segment_size)
                 final_pos_in_segment = (user_pos+user_len) % self._segment_size
 
-                print("NumSamples = {}, CurrentSegment = {}, CurrentPos = {},  FinalSegment = {}, FinalPos = {}, UserLen = {}".format(self._notify_samples, current_segment, current_pos_in_segment, final_segment, final_pos_in_segment, user_len))
+                self.card._print("NumSamples = {}, CurrentSegment = {}, CurrentPos = {},  FinalSegment = {}, FinalPos = {}, UserLen = {}".format(self._notify_samples, current_segment, current_pos_in_segment, final_segment, final_pos_in_segment, user_len))
 
                 self._current_samples += self._notify_samples
                 if self._to_transfer_samples != 0 and self._to_transfer_samples < self._current_samples:
                     raise StopIteration
 
                 fill_size = self.fill_size_promille()
                 self.card._print("Fill size: {}%  Pos:{:08x} Len:{:08x} Total:{:.2f} MiS / {:.2f} MiS".format(fill_size/10, user_pos, user_len, self._current_samples / MEBI(1), self._to_transfer_samples / MEBI(1)), end='\r')
```

### Comparing `spcm-1.0.6/src/spcm/classes_multi_purpose_ios.py` & `spcm-1.1.0/src/spcm/classes_multi_purpose_ios.py`

 * *Files identical despite different names*

### Comparing `spcm-1.0.6/src/spcm/classes_netbox.py` & `spcm-1.1.0/src/spcm/classes_netbox.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,14 +56,28 @@
         Returns
         -------
         bool
             True if the Netbox is connected
         """
 
         return self.is_netbox
+    
+    def __str__(self) -> str:
+        """
+        Returns the string representation of the Netbox
+
+        Returns
+        -------
+        str
+            The string representation of the Netbox
+        """
+
+        netbox_type = self.type()
+        netbox_str = "DN{series:x}.{family:x}{speed:x}-{channel:d}".format(**netbox_type)
+        return f"Netbox: {netbox_str} at {self.ip()} sn {self.sn():05d}"
         
     def type(self) -> dict[int, int, int, int]:
         """
         Returns the type of the Netbox (see register 'SPC_NETBOX_TYPE' in chapter `Netbox` in the manual)
 
         Returns
         -------
```

### Comparing `spcm-1.0.6/src/spcm/classes_sequence.py` & `spcm-1.1.0/src/spcm/classes_sequence.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # -*- coding: utf-8 -*-
 
 from .constants import *
 
 from .classes_data_transfer import DataTransfer
 
+from .classes_unit_conversion import UnitConversion
+from . import units
+
 class Sequence(DataTransfer):
     """
     a high-level class to control the sequence mode on Spectrum Instrumentation cards
 
     For more information about what setups are available, please have a look at the user manual
     for your specific card.
 
@@ -49,32 +52,35 @@
             The segment to be addresses
         """
 
         if segment is not None:
             self.card.set_i(SPC_SEQMODE_WRITESEGMENT, segment)
         return self.card.get_i(SPC_SEQMODE_WRITESEGMENT)
     
-    def segment_size(self, segment_size : int = None) -> int:
+    def segment_size(self, segment_size : int = None, return_unit = None) -> int:
         """
         Defines the number of valid/to be replayed samples for the current selected memory segment in samples per channel. (see register 'SPC_SEQMODE_SEGMENTSIZE' in chapter `Sequence Mode` in the manual)
 
         Parameters
         ----------
-        segment_size : int
+        segment_size : int | pint.Quantity
             The size of the segment in samples
 
         Returns
         -------
         segment_size : int
             The size of the segment in samples
         """
 
         if segment_size is not None:
+            segment_size = UnitConversion.convert(segment_size, units.Sa, int)
             self.card.set_i(SPC_SEQMODE_SEGMENTSIZE, segment_size)
-        return self.card.get_i(SPC_SEQMODE_SEGMENTSIZE)
+        return_value = self.card.get_i(SPC_SEQMODE_SEGMENTSIZE)
+        if return_unit is not None: return UnitConversion.to_unit(return_value, return_unit)
+        return return_value
     
     def step_memory(self, step_index : int, next_step_index : int = None, segment_index : int = None, loops : int = None, flags : int = None) -> tuple[int, int, int, int]:
         """
         Defines the step memory for the current selected memory segment. (see register 'SPC_SEQMODE_STEPMEM0' in chapter `Sequence Mode` in the manual)
 
         Parameters
         ----------
```

### Comparing `spcm-1.0.6/src/spcm/classes_time_stamp.py` & `spcm-1.1.0/src/spcm/classes_time_stamp.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,27 +109,27 @@
         databuffer_unaligned = np.empty(((self._buffer_alignment + self.buffer_size) // item_size, ), dtype = sample_type)   # half byte count at int16 sample (// = integer division)
         # two numpy-arrays may share the same memory: skip the begin up to the alignment boundary (ArrayVariable[SKIP_VALUE:])
         # Address of data-memory from numpy-array: ArrayVariable.__array_interface__['data'][0]
         start_pos_samples = ((self._buffer_alignment - (databuffer_unaligned.__array_interface__['data'][0] & dwMask)) // item_size)
         self.buffer = databuffer_unaligned[start_pos_samples:start_pos_samples + (self.buffer_size // item_size)]   # byte address but int16 sample: therefore / 2
         self.buffer = self.buffer.reshape((num_timestamps, 2), order='C') # array items per timestamp, because the maximum item size is 8 bytes = 64 bits
     
-    def start_buffer_transfer(self, *args, direction=SPCM_DIR_CARDTOPC, notify_samples=0, transfer_offset=0, transfer_length=None) -> None:
+    def start_buffer_transfer(self, *args, direction=SPCM_DIR_CARDTOPC, notify_timestamps=0, transfer_offset=0, transfer_length=None) -> None:
         """
         Start the transfer of the timestamp data to the card
         
         Parameters
         ----------
         *args : list
             list of additonal arguments that are added as flags to the start dma command
         """
         
         notify_size = 0
-        if notify_samples: 
-            self._notify_timestamps = notify_samples
+        if notify_timestamps: 
+            self._notify_timestamps = notify_timestamps
         if self._notify_timestamps: 
             notify_size = self._notify_timestamps * self.bytes_per_ts
 
         if transfer_offset:
             transfer_offset_bytes = transfer_offset * self.bytes_per_ts
         else:
             transfer_offset_bytes = 0
```

### Comparing `spcm-1.0.6/src/spcm/classes_trigger.py` & `spcm-1.1.0/src/spcm/classes_trigger.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,38 @@
 # -*- coding: utf-8 -*-
 
+import numpy as np
+
 from .constants import *
 
-from .classes_functionality import CardFunctionality 
+from .classes_functionality import CardFunctionality
+from .classes_card import Card
+from .classes_channels import Channels, Channel
+
+from .classes_unit_conversion import UnitConversion
+from . import units
+import pint
 
 class Trigger(CardFunctionality):
     """a higher-level abstraction of the CardFunctionality class to implement the Card's Trigger engine"""
+
+    channels : Channels = None
+
+    def __init__(self, card : 'Card', **kwargs) -> None:
+        """
+        Constructor of the Trigger class
+        
+        Parameters
+        ----------
+        card : Card
+            The card to use for the Trigger class
+        """
+
+        super().__init__(card)
+        self.channels = kwargs.get('channels', None)
     
     def __str__(self) -> str:
         """
         String representation of the Trigger class
     
         Returns
         -------
@@ -74,57 +97,118 @@
         """
 
         if mask is not None:
             self.card.set_i(SPC_TRIG_ANDMASK, mask)
         return self.card.get_i(SPC_TRIG_ANDMASK)
 
     # Channel triggering
-    def ch_mode(self, channel : int, mode : int = None) -> int:
+    def ch_mode(self, channel, mode : int = None) -> int:
         """
         Set the mode for the trigger input lines (see register 'SPC_TRIG_CH0_MODE' in chapter `Trigger` in the manual)
         
         Parameters
         ----------
-        channel : int
+        channel : int | Channel
             The channel to set the mode for
         mode : int
             The mode for the trigger input lines
         
         Returns
         -------
         int
             The mode for the trigger input lines
+        
         """
 
+        channel_index = int(channel)
         if mode is not None:
-            self.card.set_i(SPC_TRIG_CH0_MODE + channel, mode)
-        return self.card.get_i(SPC_TRIG_CH0_MODE + channel)
+            self.card.set_i(SPC_TRIG_CH0_MODE + channel_index, mode)
+        return self.card.get_i(SPC_TRIG_CH0_MODE + channel_index)
 
-    def ch_level(self, channel : int, level : int, trigger_level = None) -> int:
+    def ch_level(self, channel : int, level_num : int, level_value = None, return_unit : pint.Unit = None) -> int:
         """
         Set the level for the trigger input lines (see register 'SPC_TRIG_CH0_LEVEL0' in chapter `Trigger` in the manual)
         
         Parameters
         ----------
-        channel : int
+        channel : int | Channel
             The channel to set the level for
-        level : int
+        level_num : int
             The level 0 or level 1
-        trigger_level : int
+        level_value : int | pint.Quantity | None
             The level for the trigger input lines
         
         Returns
         -------
         int
             The level for the trigger input lines
         """
 
-        if level is not None:
-            self.card.set_i(SPC_TRIG_CH0_LEVEL0 + channel + 100 * level, trigger_level)
-        return self.card.get_i(SPC_TRIG_CH0_LEVEL0 + channel + 100 * level)
+        channel_index = int(channel)
+        # if a level value is given in the form of a quantity, convert it to the card's unit as a integer value
+        if isinstance(level_value, units.Quantity):
+            if isinstance(channel, Channel):
+                level_value = channel.reconvert_data(level_value)
+            elif self.channels and isinstance(self.channels[channel_index], Channel):
+                level_value = self.channels[channel_index].reconvert_data(level_value)
+            else:
+                raise ValueError("No channel information available to convert the trigger level value. Please provide a channel object or set the channel information in the Trigger object.")
+        
+        if isinstance(level_value, int):
+            self.card.set_i(SPC_TRIG_CH0_LEVEL0 + channel_index + 100 * level_num, level_value)
+
+        return_value = self.card.get_i(SPC_TRIG_CH0_LEVEL0 + channel_index + 100 * level_num)
+        # if a return unit is given, convert the value to the given unit if a channel object is available
+        if isinstance(return_unit, pint.Unit):
+            if isinstance(channel, Channel):
+                return_value = channel.convert_data(return_value, return_unit=return_unit)
+            elif self.channels and isinstance(self.channels[channel_index], Channel):
+                return_value = self.channels[channel_index].convert_data(return_value, return_unit=return_unit)
+            else:
+                raise ValueError("No channel information available to convert the returning trigger level value. Please provide a channel object or set the channel information in the Trigger object.")
+            
+        return return_value
+
+    def ch_level0(self, channel : int, level_value = None, return_unit : pint.Unit = None) -> int:
+        """
+        Set the level 0 for the trigger input lines (see register 'SPC_TRIG_CH0_LEVEL0' in chapter `Trigger` in the manual)
+        
+        Parameters
+        ----------
+        channel : int | Channel
+            The channel to set the level for
+        level_value : int | pint.Quantity | None
+            The level for the trigger input lines
+        
+        Returns
+        -------
+        int
+            The level for the trigger input lines
+        """
+
+        return self.ch_level(channel, 0, level_value, return_unit)
+    
+    def ch_level1(self, channel : int, level_value = None, return_unit : pint.Unit = None) -> int:
+        """
+        Set the level 1 for the trigger input lines (see register 'SPC_TRIG_CH0_LEVEL1' in chapter `Trigger` in the manual)
+        
+        Parameters
+        ----------
+        channel : int | Channel
+            The channel to set the level for
+        level_value : int | pint.Quantity | None
+            The level for the trigger input lines
+        
+        Returns
+        -------
+        int
+            The level for the trigger input lines
+        """
+
+        return self.ch_level(channel, 1, level_value, return_unit)
 
     # Channel OR Mask0
     def ch_or_mask0(self, mask : int = None) -> int:
         """
         Set the channel OR mask0 for the trigger input lines (see register 'SPC_TRIG_CH_ORMASK0' in chapter `Trigger` in the manual)
         
         Parameters
@@ -159,32 +243,59 @@
         """
 
         if mask is not None:
             self.card.set_i(SPC_TRIG_CH_ANDMASK0, mask)
         return self.card.get_i(SPC_TRIG_CH_ANDMASK0)
     
     # Delay
-    def delay(self, delay : int = None) -> int:
+    def delay(self, delay : int = None, return_unit : pint.Unit = None) -> int:
         """
         Set the delay for the trigger input lines in number of sample clocks (see register 'SPC_TRIG_DELAY' in chapter `Trigger` in the manual)
         
         Parameters
         ----------
-        delay : int
+        delay : int | pint.Quantity
             The delay for the trigger input lines
+        return_unit : pint.Unit
+            The unit to return the value in
 
         Returns
         -------
-        int
+        int | pint.Quantity
             The delay for the trigger input lines
+
+        NOTE
+        ----
+        different cards have different step sizes for the delay. 
+        If a delay with unit is given, this function takes the value, 
+        calculates the integer value and rounds to the nearest allowed delay value
         """
 
+        sr = self.card.get_i(SPC_SAMPLERATE) * units.Hz
         if delay is not None:
+            if isinstance(delay, units.Quantity):
+                delay_step = self.card.get_i(SPC_TRIG_AVAILDELAY_STEP)
+                delay = np.rint(int(delay * sr) / delay_step).astype(np.int64) * delay_step
             self.card.set_i(SPC_TRIG_DELAY, delay)
-        return self.card.get_i(SPC_TRIG_DELAY)
+        return_value = self.card.get_i(SPC_TRIG_DELAY)
+        if return_unit is not None: 
+            return_value = UnitConversion.to_unit(return_value / sr, return_unit)
+        return return_value
+    
+    def trigger_counter(self) -> int:
+        """
+        Get the number of trigger events since acquisition start (see register 'SPC_TRIGGERCOUNTER' in chapter `Trigger` in the manual)
+        
+        Returns
+        -------
+        int
+            The trigger counter
+        """
+
+        return self.card.get_i(SPC_TRIGGERCOUNTER)
     
     # Main external window trigger (ext0/Trg0)
     def ext0_mode(self, mode : int = None) -> int:
         """
         Set the mode for the main external window trigger (ext0/Trg0) (see register 'SPC_TRIG_EXT0_MODE' in chapter `Trigger` in the manual)
         
         Parameters
@@ -261,63 +372,78 @@
         """
 
         if mode is not None:
             self.card.set_i(SPC_TRIG_EXT1_MODE, mode)
         return self.card.get_i(SPC_TRIG_EXT1_MODE)
     
     # Trigger level
-    def ext0_level0(self, level : int = None) -> int:
+    def ext0_level0(self, level = None, return_unit = None) -> int:
         """
         Set the trigger level 0 for the ext0 trigger (see register 'SPC_TRIG_EXT0_LEVEL0' in chapter `Trigger` in the manual)
         
         Parameters
         ----------
         level : int
             The trigger level 0 for the ext0 trigger in mV
+        return_unit : pint.Unit
+            The unit to return the value in
         
         Returns
         -------
-        int
-            The trigger level 0 for the ext0 trigger in mV
+        int | pint.Quantity
+            The trigger level 0 for the ext0 trigger in mV or in the specified unit
         """
 
         if level is not None:
+            level = UnitConversion.convert(level, units.mV, int)
             self.card.set_i(SPC_TRIG_EXT0_LEVEL0, level)
-        return self.card.get_i(SPC_TRIG_EXT0_LEVEL0)
+        return_value = self.card.get_i(SPC_TRIG_EXT0_LEVEL0)
+        if return_unit is not None: return UnitConversion.to_unit(return_value * units.mV, return_unit)
+        return return_value
     
-    def ext0_level1(self, level : int = None) -> int:
+    def ext0_level1(self, level = None, return_unit = None) -> int:
         """
         Set the trigger level 1 for the ext0 trigger (see register 'SPC_TRIG_EXT0_LEVEL1' in chapter `Trigger` in the manual)
         
         Parameters
         ----------
         level : int
             The trigger level for the ext0 trigger in mV
+        return_unit : pint.Unit
+            The unit to return the value in
         
         Returns
         -------
-        int
-            The trigger level for the ext0 trigger in mV
+        int | pint.Quantity
+            The trigger level for the ext0 trigger in mV or in the specified unit
         """
 
         if level is not None:
+            level = UnitConversion.convert(level, units.mV, int)
             self.card.set_i(SPC_TRIG_EXT0_LEVEL1, level)
-        return self.card.get_i(SPC_TRIG_EXT0_LEVEL1)
+        return_value = self.card.get_i(SPC_TRIG_EXT0_LEVEL1)
+        if return_unit is not None: return UnitConversion.to_unit(return_value * units.mV, return_unit)
+        return return_value
     
-    def ext1_level0(self, level : int = None) -> int:
+    def ext1_level0(self, level = None, return_unit = None) -> int:
         """
         Set the trigger level 0 for the ext1 trigger (see register 'SPC_TRIG_EXT1_LEVEL0' in chapter `Trigger` in the manual)
         
         Parameters
         ----------
         level : int
             The trigger level 0 for the ext1 trigger in mV
+        return_unit : pint.Unit
+            The unit to return the value in
         
         Returns
         -------
-        int
-            The trigger level 0 for the ext1 trigger in mV
+        int | pint.Quantity
+            The trigger level 0 for the ext1 trigger in mV or in the specified unit
         """
 
         if level is not None:
+            level = UnitConversion.convert(level, units.mV, int)
             self.card.set_i(SPC_TRIG_EXT1_LEVEL0, level)
-        return self.card.get_i(SPC_TRIG_EXT1_LEVEL0)
+        return_value = self.card.get_i(SPC_TRIG_EXT1_LEVEL0)
+        if return_unit is not None: return UnitConversion.to_unit(return_value * units.mV, return_unit)
+        return return_value
```

### Comparing `spcm-1.0.6/src/spcm/pyspcm.py` & `spcm-1.1.0/src/spcm/pyspcm.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,19 +319,19 @@
         spcm_dwSendIDNRequest.argtype = [POINTER(c_char_p), uint32, uint32]
         spcm_dwSendIDNRequest.restype = uint32
 
     else:
         raise Exception('Operating system not supported')
 
 except OSError as e:
-    raise Exception(text="The Spectrum Instrumentation device driver is not found. Please install the driver and try again.\nFor the newest drivers, see https://spectrum-instrumentation.com/support/downloads.php")
+    raise Exception("The Spectrum Instrumentation device driver is not found. Please install the driver and try again.\nFor the newest drivers, see https://spectrum-instrumentation.com/support/downloads.php")
 
 except AttributeError as e:
     minimum_driver_version = "7.0"
-    raise Exception(text="Driver version not supported. Minimum version required: {}.\n For the newest drivers, see https://spectrum-instrumentation.com/support/downloads.php".format(minimum_driver_version))
+    raise Exception("Driver version not supported. Minimum version required: {}.\n For the newest drivers, see https://spectrum-instrumentation.com/support/downloads.php".format(minimum_driver_version))
 
 def spcm_dwSetParam_i64(hDrv, lReg, Val):
     try:
         llVal = int64(Val.value)
     except AttributeError:
         llVal = int64(Val)
     return spcm_dwSetParam_i64_ (hDrv, lReg, llVal)
```

### Comparing `spcm-1.0.6/src/spcm/regs.py` & `spcm-1.1.0/src/spcm/regs.py`

 * *Files identical despite different names*

### Comparing `spcm-1.0.6/src/spcm/spcerr.py` & `spcm-1.1.0/src/spcm/spcerr.py`

 * *Files identical despite different names*

### Comparing `spcm-1.0.6/src/spcm.egg-info/PKG-INFO` & `spcm-1.1.0/src/spcm.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spcm
-Version: 1.0.6
+Version: 1.1.0
 Summary: Package for Spectrum Instrumentation GmbH cards
 Author-email: Spectrum Instrumentation GmbH <info@spec.de>
 Project-URL: Homepage, https://spectrum-instrumentation.com/
 Project-URL: API, https://spectruminstrumentation.github.io/spcm/spcm.html
 Project-URL: Repository, https://github.com/SpectrumInstrumentation/spcm
 Project-URL: Examples, https://github.com/SpectrumInstrumentation/spcm/tree/master/src/examples
 Project-URL: Knowledge Base, https://spectrum-instrumentation.com/support/knowledgebase/index.php
@@ -23,14 +23,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Hardware
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.25.2
 Requires-Dist: h5py>=3.10.0
+Requires-Dist: pint>=0.23
 
 <div style="margin-bottom: 20px; text-align: center">
 <a href="https://spectrum-instrumentation.com">
     <img src="https://spectrum-instrumentation.com/img/logo-complete.png"  width=400 />
 </a>
 </div>
 
@@ -48,33 +49,37 @@
 # Supported devices
 
 See the [SUPPORTED_DEVICES.md](https://github.com/SpectrumInstrumentation/spcm/blob/master/src/spcm/SUPPORTED_DEVICES.md) file for a list of supported devices.
 
 # Requirements
 [![Python](https://img.shields.io/pypi/pyversions/spcm.svg)](https://badge.fury.io/py/spcm)
 [![Static Badge](https://img.shields.io/badge/NumPy-1.25-green)](https://numpy.org/)
+[![Static Badge](https://img.shields.io/badge/h5py-3.10-orange)](https://www.h5py.org/)
 
 `spcm` requires the Spectrum Instrumentation [driver](https://spectrum-instrumentation.com/support/downloads.php) which is available for Windows and Linux. 
 Please have a look in the manual of your product for more information about installing the driver on the different plattforms.
 
 # Installation and dependencies
 [![Pip Package](https://img.shields.io/pypi/v/spcm?logo=PyPI)](https://pypi.org/project/spcm)
+[![Publish to PyPI](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/spcm-publish-to-pypi.yml/badge.svg)](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/spcm-publish-to-pypi.yml)
 
 Start by installing Python 3.9 or higher. We recommend using the latest version. You can download Python from [https://www.python.org/](https://www.python.org/).
 
 You would probably also like to install and use a virtual environment, although it's not strictly necessary. See the examples [README.md](https://github.com/SpectrumInstrumentation/spcm/blob/master/src/examples/README.md) for a more detailed explanation on how to use `spcm` in a virtual environment.
 
 To install the latest release using `pip`:
 ```bash
 $ pip install spcm
 ```
-Note that: this will automatically install all the dependencies (e.g. NumPy).
+Note that: this will automatically install all the dependencies.
 
 # Documentation
 [![Documentation](https://img.shields.io/badge/api-reference-blue.svg)](https://spectruminstrumentation.github.io/spcm/spcm.html)
+[![Build dosc](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/spcm-docs-pages.yml/badge.svg)](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/spcm-docs-pages.yml)
+[![Publish docs](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/pages/pages-build-deployment)
 
 The API documentation for the latest [stable release](https://spectruminstrumentation.github.io/spcm/spcm.html) is available for reading on GitHub pages.
 
 Please also see the hardware user manuals for your specific card for more information about the provided functionality.
 
 # Using spcm
 
@@ -159,14 +164,40 @@
 See the register `SPC_PCISERIALNO` in the reference manual of your specific device for more information.
 
 If the `device_identifier` is given that card is opened, if at the same time `card_type` or `serial_number` are given then these behave as an additional check too see if the opened card is of a certain type or has that specific serial number.
 
 ### Demo devices
 To test the Spectrum Instrumentation API with user code without hardware, the Control Center gives the user the option to create [demo devices](https://spectrum-instrumentation.com/support/knowledgebase/software/How_to_set_up_a_demo_card.php). These demo devices can be used in the same manner as real devices. Simply change the device identifier string to the string as shown in the Control Center.
 
+## Units and quantities
+
+`spcm` uses [pint](https://pint.readthedocs.io/en/stable/) to handle all quantities that have a physical unit. To enable the use of qunatities simply import the units module from `spcm`:
+
+```python
+from spcm import units
+```
+
+This import the `units` object from `spcm`. which is a `UnitRegistry` object from  `pint`. Defining a quantity is as simples as:
+
+```python
+from spcm import units
+
+frequency = 100 * units.MHz
+amplitude = 1 * units.V
+# etc...
+```
+
+All methods within the `spcm` that expect a value that is related to a physical quantity support the quantities, for example setting a timeout:
+
+```python
+card.timeout(5 * units.s)
+```
+
+See our dedicated examples for more information about where units can be used.
+
 ## Card Functionality
 After opening a card, StarHub or group of card, specific functionality of the cards can be accessed through `CardFunctionality` classes. 
 
 | Name                | Description                                                         |
 |---------------------|---------------------------------------------------------------------|
 | `Channels`          | class for setting up the in- or output stage of the channels of a card |
 | `Clock`             | class for setting up the clock engine of the card                   |
@@ -196,52 +227,78 @@
     # (or)
     data_transfer = spcm.DataTransfer(card)
     # etc ...
 
 ```
 Each of these functionalities typically corresponds to a chapter in your device manual, so for further reference please have a look in the device manual.
 
+## Setting up Channels
+
+The Channels functionality allows the user to setup individual channels on a Card or a CardStack. The channels object is also a Python iterator, hence if a channels object is used it a for-loop, each iteration provides a Channel object:
+
+```python
+channels = spcm.Channels(card, card_enable=spcm.CHANNEL0 | CHANNEL1)
+for channel in channels:
+    # do something with each channel
+```
+
+In addition, the user can define the output load connected to the channel (standard value 50 Ohm), to any resistor value or high impedance (`units.highZ`). With this output load, the amplitude setting can be done with the repect to this output load:
+
+```python
+channels = Channels(card, card_enable=spcm.CHANNEL0 | CHANNEL1)
+channels[0].output_load(units.highZ)
+channels[0].amp(1 * units.V)
+# or for all channels
+channels.output_load(units.highZ)
+channels.amp(1 * units.V)
+```
+
+This information allows the user to convert the data coming from `DataTransfer`, using the `convert_data()` method. See the section "Setting up a data transfer buffer ..." for more details.
+
 ## Setting up the Clock engine
 
 The Clock engine is used to generate a clock signal that is used as the source for all timing critical processes on the card.
 
 ### Sample rate
 To get the maximum sample rate of the active card and set the sample rate to the maximum, this is an example using internal PLL clock mode:
 ```python
 clock = spcm.Clock(card)
 clock.mode(spcm.SPC_CM_INTPLL)
-sample_rate = clock.sample_rate(max=True) # (or) sample_rate = clock.sample_rate(20e6) # for a 20 MHz sample rate (see reference manual for allowed values)
-print("Current sample rate: {}S/s".format(sample_rate))
+sample_rate = clock.sample_rate(max=True) 
+# (or) 
+sample_rate = clock.sample_rate(20 * units.MHz) # for a 20 MHz sample rate (see reference manual for allowed values)
+print("Current sample rate: {}".format(sample_rate, return_unit=units.MS/units.s))
 ```
 
 ## Setting up the Trigger engine
 
 ### External trigger
 
 The Trigger engine can be configured for a multitude of different configurations (see the hardware manual for more information about the specific configurations for your device). Here we've given an example for an external trigger arriving at input port ext0, that is DC-coupled. The card is waiting for positiv edge that excedes 1.5 V:
 
 ```python
 trigger = spcm.Trigger(card)
 trigger.or_mask(spcm.SPC_TMASK_EXT0) # set the ext0 hardware input as trigger source
 trigger.ext0_mode(spcm.SPC_TM_POS) # wait for a positive edge
-trigger.ext0_level0(1500) # Trigger level is 1.5 V (1500 mV)
+trigger.ext0_level0(1.5 * units.V)
 trigger.ext0_coupling(spcm.COUPLING_DC) # set DC coupling
 ```
 
 ## Setting up the multi-purpose I/O lines
 
 See the hardware manual, for the multi-purpose I/O lines functionality that can be programmed.
 
 ## Setting up a data transfer buffer for recording (digitizer) or replay (AWG)
 
 ### Recording (Digitizing)
 To transfer data to or from the card, we have to setup a data transfer object. This object allocates an amount the memory of the card (`memory_size`) and a Direct Memory Access (DMA) buffer on the host pc (`allocate_buffer`). Half of the samples are taken before the trigger, as configured by the trigger engine, and half of the samples are recorded afterwards. Then the transfer from the card to the host pc is started and the program waits until the DMA is filled.
 
 ```python
 # define the data buffer
+num_samples = 4 * units.KiS # 1 KiS = 1 KibiSamples = 1024 Samples
 data_transfer = spcm.DataTransfer(card)
 data_transfer.memory_size(num_samples)
 data_transfer.allocate_buffer(num_samples)
 data_transfer.post_trigger(num_samples // 2)
 # Start DMA transfer
 data_transfer.start_buffer_transfer(spcm.M2CMD_DATA_STARTDMA)
 
@@ -263,32 +320,55 @@
 
 This data can be further processed or plotted using, for example, [`matplotlib`](https://matplotlib.org/).
 
 ### Replay (Generation)
 
 The setup of the DMA for replay is very similar. First card memory is allocated with `memory_size` and then a DMA buffer is allocated (`allocated_buffer`) and made accessible though the NumPy object `data_transfer.buffer`, which can then be written to using standard NumPy methods. Finally, data transfer from the host PC to the card is started and the programming is waiting until all the data is transferred:
 ```python
+num_samples = 4 * units.KiS # 1 KiS = 1 KibiSamples = 1024 Samples
 data_transfer = spcm.DataTransfer(card)
 data_transfer.memory_size(num_samples)
 data_transfer.allocate_buffer(num_samples)
 data_transfer.loops(0) # loop continuously
 # simple linear ramp for analog output cards
-data_transfer.buffer[:] = np.arange(-num_samples//2, num_samples//2).astype(np.int16)
+num_samples_magnitude = num_samples.to(units.S).magnitude
+data_transfer.buffer[:] = np.arange(-num_samples_magnitude//2, num_samples_magnitude//2).astype(np.int16)
 
 data_transfer.start_buffer_transfer(spcm.M2CMD_DATA_STARTDMA, spcm.M2CMD_DATA_WAITDMA)
 ```
 
+#### Data transfer
+
+In the above it's assume that all the data has been transferred from the card into the buffer object, however if you're working in FIFO mode or you've defined the buffer to be smaller then the assigned card memory size, then the card will write to parts of the memory and tell you were it wrote. 
+
+This can be either handled manually (see the reference manual of your card, or the methods `avail_card_len()`, `avail_user_pos()` and `avail_user_len()`).
+
+Secondly, it can also be handled with Python iterators functionality. If the `data_transfer` object is handed to a for-loop, then in each iteration a view of the current active memory part is given in the form of a NumPy array and the user can do calculations on that.
+
+```python
+# Get a block of data
+for data_block in data_transfer:
+    # data_block is a NumPy array view of the currently active buffer part
+    for channel in channels:
+        data_units = channel.convert_data(data_block[:, channel])
+        minimum = np.min(data_units)
+        maximum = np.max(data_units)
+        print(f"Minimum: {minimum} - maximum: {maximum}")
+```
+
+The same principle also works with generator cards (see the example `2_gen_fifo.py`).
+
 ## Multiple recording / replay
 
 In case of multiple recording / replay, the memory is divided in equally sized segments, that are populated / replayed when a trigger is detected. Multiple triggers each trigger the next segment to be populated or replayed.
 
 The following code snippet shows how to setup the buffer for 4 segments with each 128 Samples:
 
 ```python
-samples_per_segment = 128
+samples_per_segment = 128 * units.S
 num_segments = 4
 multiple_recording = spcm.Multi(card)
 multiple_recording.memory_size(samples_per_segment*num_segments)
 multiple_recording.allocate_buffer(segment_samples=samples_per_segment, num_segments=num_segments)
 multiple_recording.post_trigger(samples_per_segment // 2)
 multiple_recording.start_buffer_transfer(spcm.M2CMD_DATA_STARTDMA)
 ```
@@ -314,26 +394,25 @@
 
 Please see the folder `4_pulse-generator` in the `examples` folder for several dedicated examples. In the following, there is a simple example for setting up a single pulse generator on x0.
 
 Create a pulse generators object and get the clock rate used by the pulse generator. Use that to calculate the period of a 1 MHz signal and the half of that period we'll have a high signal (hence 50% duty cycle). The pulse generator will start if the trigger condition is met without delay and loops infinitely many times. The triggering condition is set to the card software trigger. See more details in the pulse generator chapter in the specific hardware manual.
 
 ```python
 pulse_generators = spcm.PulseGenerators(card)
-# get the clock of the card
-pulse_gen_clock_Hz = pulse_generators.get_clock()
 
 # generate a continuous signal with 1 MHz
-len_for_1MHz = pulse_gen_clock_Hz // spcm.MEGA(1)
-pulse_generators[0].mode(spcm.SPCM_PULSEGEN_MODE_TRIGGERED)
-pulse_generators[0].period_length(len_for_1MHz)
-pulse_generators[0].high_length(len_for_1MHz // 2) # 50% HIGH, 50% LOW
-pulse_generators[0].delay(0)
-pulse_generators[0].num_loops(0) # 0: infinite
-pulse_generators[0].mux1(spcm.SPCM_PULSEGEN_MUX1_SRC_UNUSED)
-pulse_generators[0].mux2(spcm.SPCM_PULSEGEN_MUX2_SRC_SOFTWARE) # started by software force command
+pulse_generators[0].pulse_period(1 * units.us)
+# pulse_generators[0].repetition_rate(1 * units.MHz) # (or)
+pulse_generators[0].duty_cycle(50 * units.percent)
+# pulse_generators[0].pulse_length(0.5 * units.us) # (or)
+pulse_generators[0].start_delay(0 * units.us)
+pulse_generators[0].repetitions(0) # 0: infinite
+pulse_generators[0].start_condition_state_signal(spcm.SPCM_PULSEGEN_MUX1_SRC_UNUSED)
+pulse_generators[0].start_condition_trigger_signal(spcm.SPCM_PULSEGEN_MUX2_SRC_SOFTWARE)
+pulse_generators[0].invert_start_condition(False)
 
 # and write the pulse generator settings
 pulse_generators.write_setup()
 
 # start all pulse generators that wait for a software command
 pulse_generators.force()
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spcm Version: 1.0.6 Summary: Package for Spectrum
+Metadata-Version: 2.1 Name: spcm Version: 1.1.0 Summary: Package for Spectrum
 Instrumentation GmbH cards Author-email: Spectrum Instrumentation GmbH
 spec.de> Project-URL: Homepage, https://spectrum-instrumentation.com/ Project-
 URL: API, https://spectruminstrumentation.github.io/spcm/spcm.html Project-URL:
 Repository, https://github.com/SpectrumInstrumentation/spcm Project-URL:
 Examples, https://github.com/SpectrumInstrumentation/spcm/tree/master/src/
 examples Project-URL: Knowledge Base, https://spectrum-instrumentation.com/
 support/knowledgebase/index.php Classifier: Development Status :: 4 - Beta
@@ -12,14 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering Classifier: Topic :: System ::
 Hardware Requires-Python: >=3.9 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: numpy>=1.25.2 Requires-Dist: h5py>=3.10.0
+Requires-Dist: pint>=0.23
 _[_h_t_t_p_s_:_/_/_s_p_e_c_t_r_u_m_-_i_n_s_t_r_u_m_e_n_t_a_t_i_o_n_._c_o_m_/_i_m_g_/_l_o_g_o_-_c_o_m_p_l_e_t_e_._p_n_g_]
 # spcm [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)]
 (https://opensource.org/licenses/MIT) [![PyPI - Version](https://
 img.shields.io/pypi/v/spcm)](https://pypi.org/project/spcm) [![PyPi Downloads]
 (https://img.shields.io/pypi/dm/spcm?label=downloads%20%7C%20pip&logo=PyPI)]
 (https://pypi.org/project/spcm) [![Follow](https://img.shields.io/twitter/
 follow/
@@ -29,58 +30,67 @@
 oriented Python package for interfacing with Spectrum Instrumentation GmbH
 devices. `spcm` can handle individual cards (`Card`), StarHubs (`Sync`), groups
 of cards (`CardStack`) and Netboxes (`Netbox`). # Supported devices See the
 [SUPPORTED_DEVICES.md](https://github.com/SpectrumInstrumentation/spcm/blob/
 master/src/spcm/SUPPORTED_DEVICES.md) file for a list of supported devices. #
 Requirements [![Python](https://img.shields.io/pypi/pyversions/spcm.svg)]
 (https://badge.fury.io/py/spcm) [![Static Badge](https://img.shields.io/badge/
-NumPy-1.25-green)](https://numpy.org/) `spcm` requires the Spectrum
+NumPy-1.25-green)](https://numpy.org/) [![Static Badge](https://img.shields.io/
+badge/h5py-3.10-orange)](https://www.h5py.org/) `spcm` requires the Spectrum
 Instrumentation [driver](https://spectrum-instrumentation.com/support/
 downloads.php) which is available for Windows and Linux. Please have a look in
 the manual of your product for more information about installing the driver on
 the different plattforms. # Installation and dependencies [![Pip Package]
 (https://img.shields.io/pypi/v/spcm?logo=PyPI)](https://pypi.org/project/spcm)
-Start by installing Python 3.9 or higher. We recommend using the latest
-version. You can download Python from [https://www.python.org/](https://
-www.python.org/). You would probably also like to install and use a virtual
-environment, although it's not strictly necessary. See the examples [README.md]
-(https://github.com/SpectrumInstrumentation/spcm/blob/master/src/examples/
-README.md) for a more detailed explanation on how to use `spcm` in a virtual
-environment. To install the latest release using `pip`: ```bash $ pip install
-spcm ``` Note that: this will automatically install all the dependencies (e.g.
-NumPy). # Documentation [![Documentation](https://img.shields.io/badge/api-
-reference-blue.svg)](https://spectruminstrumentation.github.io/spcm/spcm.html)
-The API documentation for the latest [stable release](https://
-spectruminstrumentation.github.io/spcm/spcm.html) is available for reading on
-GitHub pages. Please also see the hardware user manuals for your specific card
-for more information about the provided functionality. # Using spcm The `spcm`
-package is a high-level object-oriented programming library for controlling
-Spectrum Instrumentation devices. ## Examples For detailed examples see the
-`src\examples` directory. There are several sub-directories each corresponding
-to a certain kind of functionality. See also the examples on [GitHub](https://
-github.com/SpectrumInstrumentation/spcm/tree/master/src/examples). ## Hardware
-interfaces `spcm` provides the following classes for interfacing with the
-different devices. | Name | Description | |-------------|----------------------
--------------------------------------------------------------| | `Card` | a
-class to control the low-level API of Spectrum Instrumentation cards. | |
-`Sync` | a class for controling StarHub devices. | | `CardStack` | a class that
-handles the opening and closing of a combination of different cards either with
-or without a StarHub that synchronizes the cards. | | `Netbox` | a class that
-handles the opening and closing of the cards in a Netbox | ## Connect to a
-device Opening and closing of cards is handled using the python [`with`](https:
-//peps.python.org/pep-0343/) statement. This creates a context manager that
-safely handles opening and closing of a card or a group of cards. ### Using
-device identifiers Connect to local cards: ```python import spcm with spcm.Card
-('/dev/spcm0') as card: # (add your code here) ``` Connect to remote cards (you
-can find a card's IP using the [Spectrum Control Center](https://spectrum-
-instrumentation.com/en/spectrum-control-center) software): ```python import
-spcm with spcm.Card('TCPIP::192.168.1.10::inst0::INSTR') as card: # (add your
-code here) ``` Connect to a group of cards synchronized using a StarHub:
-```python import spcm card_identifiers = ["/dev/spcm0", "/dev/spcm1"]
-sync_identifier = "sync0" with spcm.CardStack
+[![Publish to PyPI](https://github.com/SpectrumInstrumentation/spcm/actions/
+workflows/spcm-publish-to-pypi.yml/badge.svg)](https://github.com/
+SpectrumInstrumentation/spcm/actions/workflows/spcm-publish-to-pypi.yml) Start
+by installing Python 3.9 or higher. We recommend using the latest version. You
+can download Python from [https://www.python.org/](https://www.python.org/).
+You would probably also like to install and use a virtual environment, although
+it's not strictly necessary. See the examples [README.md](https://github.com/
+SpectrumInstrumentation/spcm/blob/master/src/examples/README.md) for a more
+detailed explanation on how to use `spcm` in a virtual environment. To install
+the latest release using `pip`: ```bash $ pip install spcm ``` Note that: this
+will automatically install all the dependencies. # Documentation [!
+[Documentation](https://img.shields.io/badge/api-reference-blue.svg)](https://
+spectruminstrumentation.github.io/spcm/spcm.html) [![Build dosc](https://
+github.com/SpectrumInstrumentation/spcm/actions/workflows/spcm-docs-pages.yml/
+badge.svg)](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/
+spcm-docs-pages.yml) [![Publish docs](https://github.com/
+SpectrumInstrumentation/spcm/actions/workflows/pages/pages-build-deployment/
+badge.svg)](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/
+pages/pages-build-deployment) The API documentation for the latest [stable
+release](https://spectruminstrumentation.github.io/spcm/spcm.html) is available
+for reading on GitHub pages. Please also see the hardware user manuals for your
+specific card for more information about the provided functionality. # Using
+spcm The `spcm` package is a high-level object-oriented programming library for
+controlling Spectrum Instrumentation devices. ## Examples For detailed examples
+see the `src\examples` directory. There are several sub-directories each
+corresponding to a certain kind of functionality. See also the examples on
+[GitHub](https://github.com/SpectrumInstrumentation/spcm/tree/master/src/
+examples). ## Hardware interfaces `spcm` provides the following classes for
+interfacing with the different devices. | Name | Description | |-------------|-
+-------------------------------------------------------------------------------
+---| | `Card` | a class to control the low-level API of Spectrum
+Instrumentation cards. | | `Sync` | a class for controling StarHub devices. | |
+`CardStack` | a class that handles the opening and closing of a combination of
+different cards either with or without a StarHub that synchronizes the cards. |
+| `Netbox` | a class that handles the opening and closing of the cards in a
+Netbox | ## Connect to a device Opening and closing of cards is handled using
+the python [`with`](https://peps.python.org/pep-0343/) statement. This creates
+a context manager that safely handles opening and closing of a card or a group
+of cards. ### Using device identifiers Connect to local cards: ```python import
+spcm with spcm.Card('/dev/spcm0') as card: # (add your code here) ``` Connect
+to remote cards (you can find a card's IP using the [Spectrum Control Center]
+(https://spectrum-instrumentation.com/en/spectrum-control-center) software):
+```python import spcm with spcm.Card('TCPIP::192.168.1.10::inst0::INSTR') as
+card: # (add your code here) ``` Connect to a group of cards synchronized using
+a StarHub: ```python import spcm card_identifiers = ["/dev/spcm0", "/dev/
+spcm1"] sync_identifier = "sync0" with spcm.CardStack
 (card_identifiers=card_identifiers, sync_identifier=sync_identifier) as stack:
 # (add your code here) ``` The `CardStack` object contains a list of `Card`
 objects in the `stack.cards` parameter and a `Sync` object in the parameter
 `stack.sync`. ### Using card type or serial number Apart from connecting to a
 device directly through a device identifier it's also possible to connect to
 local devices using the card type or serial number. To find the first card of
 type analog out (`SPCM_TYPE_AO`) you can do the following: ```python import
@@ -95,62 +105,87 @@
 given then these behave as an additional check too see if the opened card is of
 a certain type or has that specific serial number. ### Demo devices To test the
 Spectrum Instrumentation API with user code without hardware, the Control
 Center gives the user the option to create [demo devices](https://spectrum-
 instrumentation.com/support/knowledgebase/software/
 How_to_set_up_a_demo_card.php). These demo devices can be used in the same
 manner as real devices. Simply change the device identifier string to the
-string as shown in the Control Center. ## Card Functionality After opening a
-card, StarHub or group of card, specific functionality of the cards can be
-accessed through `CardFunctionality` classes. | Name | Description | |---------
-------------|------------------------------------------------------------------
----| | `Channels` | class for setting up the in- or output stage of the
-channels of a card | | `Clock` | class for setting up the clock engine of the
-card | | `Trigger` | class for setting up the trigger engine of the card | |
-`MultiPurposeIOs` | class for setting up the multi purpose i/o of the card | |
-`DataTransfer` | class for handling data transfer functionality | | `Multi` |
-class for handling multiple recording and replay mode functionality | |
-`Sequence` | class for handling sequence mode functionality | | `TimeStamp` |
-class for handling time stamped data | | `Boxcar` | class for handling boxcar
-averaging | | `BlockAverage` | class for handling block averaging functionality
-| | `PulseGenerators` | class for setting up the pulse generator functionality
-| | `DDS` | class for handling DDS functionality | To use a specific
-functionality simply initiate an instance of one of the classes and pass a
-device object: ```python import spcm with spcm.Card('/dev/spcm0') as card:
-clock = spcm.Clock(card) # (or) trigger = spcm.Trigger(card) # (or) multi_io =
+string as shown in the Control Center. ## Units and quantities `spcm` uses
+[pint](https://pint.readthedocs.io/en/stable/) to handle all quantities that
+have a physical unit. To enable the use of qunatities simply import the units
+module from `spcm`: ```python from spcm import units ``` This import the
+`units` object from `spcm`. which is a `UnitRegistry` object from `pint`.
+Defining a quantity is as simples as: ```python from spcm import units
+frequency = 100 * units.MHz amplitude = 1 * units.V # etc... ``` All methods
+within the `spcm` that expect a value that is related to a physical quantity
+support the quantities, for example setting a timeout: ```python card.timeout(5
+* units.s) ``` See our dedicated examples for more information about where
+units can be used. ## Card Functionality After opening a card, StarHub or group
+of card, specific functionality of the cards can be accessed through
+`CardFunctionality` classes. | Name | Description | |---------------------|----
+-----------------------------------------------------------------| | `Channels`
+| class for setting up the in- or output stage of the channels of a card | |
+`Clock` | class for setting up the clock engine of the card | | `Trigger` |
+class for setting up the trigger engine of the card | | `MultiPurposeIOs` |
+class for setting up the multi purpose i/o of the card | | `DataTransfer` |
+class for handling data transfer functionality | | `Multi` | class for handling
+multiple recording and replay mode functionality | | `Sequence` | class for
+handling sequence mode functionality | | `TimeStamp` | class for handling time
+stamped data | | `Boxcar` | class for handling boxcar averaging | |
+`BlockAverage` | class for handling block averaging functionality | |
+`PulseGenerators` | class for setting up the pulse generator functionality | |
+`DDS` | class for handling DDS functionality | To use a specific functionality
+simply initiate an instance of one of the classes and pass a device object:
+```python import spcm with spcm.Card('/dev/spcm0') as card: clock = spcm.Clock
+(card) # (or) trigger = spcm.Trigger(card) # (or) multi_io =
 spcm.MultiPurposeIOs(card) # (or) data_transfer = spcm.DataTransfer(card) # etc
 ... ``` Each of these functionalities typically corresponds to a chapter in
 your device manual, so for further reference please have a look in the device
-manual. ## Setting up the Clock engine The Clock engine is used to generate a
-clock signal that is used as the source for all timing critical processes on
-the card. ### Sample rate To get the maximum sample rate of the active card and
-set the sample rate to the maximum, this is an example using internal PLL clock
-mode: ```python clock = spcm.Clock(card) clock.mode(spcm.SPC_CM_INTPLL)
-sample_rate = clock.sample_rate(max=True) # (or) sample_rate =
-clock.sample_rate(20e6) # for a 20 MHz sample rate (see reference manual for
-allowed values) print("Current sample rate: {}S/s".format(sample_rate)) ``` ##
-Setting up the Trigger engine ### External trigger The Trigger engine can be
-configured for a multitude of different configurations (see the hardware manual
-for more information about the specific configurations for your device). Here
-we've given an example for an external trigger arriving at input port ext0,
-that is DC-coupled. The card is waiting for positiv edge that excedes 1.5 V:
-```python trigger = spcm.Trigger(card) trigger.or_mask(spcm.SPC_TMASK_EXT0) #
-set the ext0 hardware input as trigger source trigger.ext0_mode
-(spcm.SPC_TM_POS) # wait for a positive edge trigger.ext0_level0(1500) #
-Trigger level is 1.5 V (1500 mV) trigger.ext0_coupling(spcm.COUPLING_DC) # set
-DC coupling ``` ## Setting up the multi-purpose I/O lines See the hardware
+manual. ## Setting up Channels The Channels functionality allows the user to
+setup individual channels on a Card or a CardStack. The channels object is also
+a Python iterator, hence if a channels object is used it a for-loop, each
+iteration provides a Channel object: ```python channels = spcm.Channels(card,
+card_enable=spcm.CHANNEL0 | CHANNEL1) for channel in channels: # do something
+with each channel ``` In addition, the user can define the output load
+connected to the channel (standard value 50 Ohm), to any resistor value or high
+impedance (`units.highZ`). With this output load, the amplitude setting can be
+done with the repect to this output load: ```python channels = Channels(card,
+card_enable=spcm.CHANNEL0 | CHANNEL1) channels[0].output_load(units.highZ)
+channels[0].amp(1 * units.V) # or for all channels channels.output_load
+(units.highZ) channels.amp(1 * units.V) ``` This information allows the user to
+convert the data coming from `DataTransfer`, using the `convert_data()` method.
+See the section "Setting up a data transfer buffer ..." for more details. ##
+Setting up the Clock engine The Clock engine is used to generate a clock signal
+that is used as the source for all timing critical processes on the card. ###
+Sample rate To get the maximum sample rate of the active card and set the
+sample rate to the maximum, this is an example using internal PLL clock mode:
+```python clock = spcm.Clock(card) clock.mode(spcm.SPC_CM_INTPLL) sample_rate =
+clock.sample_rate(max=True) # (or) sample_rate = clock.sample_rate(20 *
+units.MHz) # for a 20 MHz sample rate (see reference manual for allowed values)
+print("Current sample rate: {}".format(sample_rate, return_unit=units.MS/
+units.s)) ``` ## Setting up the Trigger engine ### External trigger The Trigger
+engine can be configured for a multitude of different configurations (see the
+hardware manual for more information about the specific configurations for your
+device). Here we've given an example for an external trigger arriving at input
+port ext0, that is DC-coupled. The card is waiting for positiv edge that
+excedes 1.5 V: ```python trigger = spcm.Trigger(card) trigger.or_mask
+(spcm.SPC_TMASK_EXT0) # set the ext0 hardware input as trigger source
+trigger.ext0_mode(spcm.SPC_TM_POS) # wait for a positive edge
+trigger.ext0_level0(1.5 * units.V) trigger.ext0_coupling(spcm.COUPLING_DC) #
+set DC coupling ``` ## Setting up the multi-purpose I/O lines See the hardware
 manual, for the multi-purpose I/O lines functionality that can be programmed.
 ## Setting up a data transfer buffer for recording (digitizer) or replay (AWG)
 ### Recording (Digitizing) To transfer data to or from the card, we have to
 setup a data transfer object. This object allocates an amount the memory of the
 card (`memory_size`) and a Direct Memory Access (DMA) buffer on the host pc
 (`allocate_buffer`). Half of the samples are taken before the trigger, as
 configured by the trigger engine, and half of the samples are recorded
 afterwards. Then the transfer from the card to the host pc is started and the
 program waits until the DMA is filled. ```python # define the data buffer
+num_samples = 4 * units.KiS # 1 KiS = 1 KibiSamples = 1024 Samples
 data_transfer = spcm.DataTransfer(card) data_transfer.memory_size(num_samples)
 data_transfer.allocate_buffer(num_samples) data_transfer.post_trigger
 (num_samples // 2) # Start DMA transfer data_transfer.start_buffer_transfer
 (spcm.M2CMD_DATA_STARTDMA) # start card and wait until the memory is filled
 card.start(spcm.M2CMD_CARD_ENABLETRIGGER, spcm.M2CMD_DATA_WAITDMA) # (your code
 handling the recorded data comes here) ``` To access the recorded data, the
 data transfer object holds a [NumPy](https://numpy.org/) array object
@@ -161,25 +196,42 @@
 axis=1) ``` This data can be further processed or plotted using, for example,
 [`matplotlib`](https://matplotlib.org/). ### Replay (Generation) The setup of
 the DMA for replay is very similar. First card memory is allocated with
 `memory_size` and then a DMA buffer is allocated (`allocated_buffer`) and made
 accessible though the NumPy object `data_transfer.buffer`, which can then be
 written to using standard NumPy methods. Finally, data transfer from the host
 PC to the card is started and the programming is waiting until all the data is
-transferred: ```python data_transfer = spcm.DataTransfer(card)
-data_transfer.memory_size(num_samples) data_transfer.allocate_buffer
-(num_samples) data_transfer.loops(0) # loop continuously # simple linear ramp
-for analog output cards data_transfer.buffer[:] = np.arange(-num_samples//2,
-num_samples//2).astype(np.int16) data_transfer.start_buffer_transfer
-(spcm.M2CMD_DATA_STARTDMA, spcm.M2CMD_DATA_WAITDMA) ``` ## Multiple recording /
-replay In case of multiple recording / replay, the memory is divided in equally
-sized segments, that are populated / replayed when a trigger is detected.
-Multiple triggers each trigger the next segment to be populated or replayed.
-The following code snippet shows how to setup the buffer for 4 segments with
-each 128 Samples: ```python samples_per_segment = 128 num_segments = 4
+transferred: ```python num_samples = 4 * units.KiS # 1 KiS = 1 KibiSamples =
+1024 Samples data_transfer = spcm.DataTransfer(card) data_transfer.memory_size
+(num_samples) data_transfer.allocate_buffer(num_samples) data_transfer.loops(0)
+# loop continuously # simple linear ramp for analog output cards
+num_samples_magnitude = num_samples.to(units.S).magnitude data_transfer.buffer
+[:] = np.arange(-num_samples_magnitude//2, num_samples_magnitude//2).astype
+(np.int16) data_transfer.start_buffer_transfer(spcm.M2CMD_DATA_STARTDMA,
+spcm.M2CMD_DATA_WAITDMA) ``` #### Data transfer In the above it's assume that
+all the data has been transferred from the card into the buffer object, however
+if you're working in FIFO mode or you've defined the buffer to be smaller then
+the assigned card memory size, then the card will write to parts of the memory
+and tell you were it wrote. This can be either handled manually (see the
+reference manual of your card, or the methods `avail_card_len()`,
+`avail_user_pos()` and `avail_user_len()`). Secondly, it can also be handled
+with Python iterators functionality. If the `data_transfer` object is handed to
+a for-loop, then in each iteration a view of the current active memory part is
+given in the form of a NumPy array and the user can do calculations on that.
+```python # Get a block of data for data_block in data_transfer: # data_block
+is a NumPy array view of the currently active buffer part for channel in
+channels: data_units = channel.convert_data(data_block[:, channel]) minimum =
+np.min(data_units) maximum = np.max(data_units) print(f"Minimum: {minimum} -
+maximum: {maximum}") ``` The same principle also works with generator cards
+(see the example `2_gen_fifo.py`). ## Multiple recording / replay In case of
+multiple recording / replay, the memory is divided in equally sized segments,
+that are populated / replayed when a trigger is detected. Multiple triggers
+each trigger the next segment to be populated or replayed. The following code
+snippet shows how to setup the buffer for 4 segments with each 128 Samples:
+```python samples_per_segment = 128 * units.S num_segments = 4
 multiple_recording = spcm.Multi(card) multiple_recording.memory_size
 (samples_per_segment*num_segments) multiple_recording.allocate_buffer
 (segment_samples=samples_per_segment, num_segments=num_segments)
 multiple_recording.post_trigger(samples_per_segment // 2)
 multiple_recording.start_buffer_transfer(spcm.M2CMD_DATA_STARTDMA) ``` Again
 there are half the samples before and half the samples after the trigger. ##
 Timestamps See the example `6_acq_fifo_multi_ts_poll.py` in the examples folder
@@ -194,30 +246,30 @@
 is a simple example for setting up a single pulse generator on x0. Create a
 pulse generators object and get the clock rate used by the pulse generator. Use
 that to calculate the period of a 1 MHz signal and the half of that period
 we'll have a high signal (hence 50% duty cycle). The pulse generator will start
 if the trigger condition is met without delay and loops infinitely many times.
 The triggering condition is set to the card software trigger. See more details
 in the pulse generator chapter in the specific hardware manual. ```python
-pulse_generators = spcm.PulseGenerators(card) # get the clock of the card
-pulse_gen_clock_Hz = pulse_generators.get_clock() # generate a continuous
-signal with 1 MHz len_for_1MHz = pulse_gen_clock_Hz // spcm.MEGA(1)
-pulse_generators[0].mode(spcm.SPCM_PULSEGEN_MODE_TRIGGERED) pulse_generators
-[0].period_length(len_for_1MHz) pulse_generators[0].high_length(len_for_1MHz /
-/ 2) # 50% HIGH, 50% LOW pulse_generators[0].delay(0) pulse_generators
-[0].num_loops(0) # 0: infinite pulse_generators[0].mux1
-(spcm.SPCM_PULSEGEN_MUX1_SRC_UNUSED) pulse_generators[0].mux2
-(spcm.SPCM_PULSEGEN_MUX2_SRC_SOFTWARE) # started by software force command #
-and write the pulse generator settings pulse_generators.write_setup() # start
-all pulse generators that wait for a software command pulse_generators.force()
-``` This will start the pulse generator to continuously output a 1 MHz signal.
-### Sequence replay mode (AWG only) Please see the example `3_gen_sequence.py`
-in the folder `2_generation` of the examples to see an example dedicated to the
-Sequence replay mode. ### DDS (AWG only) Please see the examples in the
-dedicated examples folder `3_dds` for all the functionality provided by the DDS
+pulse_generators = spcm.PulseGenerators(card) # generate a continuous signal
+with 1 MHz pulse_generators[0].pulse_period(1 * units.us) # pulse_generators
+[0].repetition_rate(1 * units.MHz) # (or) pulse_generators[0].duty_cycle(50 *
+units.percent) # pulse_generators[0].pulse_length(0.5 * units.us) # (or)
+pulse_generators[0].start_delay(0 * units.us) pulse_generators[0].repetitions
+(0) # 0: infinite pulse_generators[0].start_condition_state_signal
+(spcm.SPCM_PULSEGEN_MUX1_SRC_UNUSED) pulse_generators
+[0].start_condition_trigger_signal(spcm.SPCM_PULSEGEN_MUX2_SRC_SOFTWARE)
+pulse_generators[0].invert_start_condition(False) # and write the pulse
+generator settings pulse_generators.write_setup() # start all pulse generators
+that wait for a software command pulse_generators.force() ``` This will start
+the pulse generator to continuously output a 1 MHz signal. ### Sequence replay
+mode (AWG only) Please see the example `3_gen_sequence.py` in the folder
+`2_generation` of the examples to see an example dedicated to the Sequence
+replay mode. ### DDS (AWG only) Please see the examples in the dedicated
+examples folder `3_dds` for all the functionality provided by the DDS
 framework. Moreover, please also have a look at the corresponding hardware
 manual. ### Boxcar (Digitizer only) See the corresponding chapter in the
 hardware manual for more information about boxcar averaging and the registers
 used. ### Block average (Digitizer only) See the corresponding chapter in the
 hardware manual for more information about block averaging and the registers
 used. # Acknowledgements We would like to thank [Christian Baker](https://
 github.com/crnbaker) for fruitful discussions and inspiration on how to setup
```

### Comparing `spcm-1.0.6/src/spcm.egg-info/SOURCES.txt` & `spcm-1.1.0/src/spcm.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 src/spcm/classes_multi_purpose_ios.py
 src/spcm/classes_netbox.py
 src/spcm/classes_pulse_generators.py
 src/spcm/classes_sequence.py
 src/spcm/classes_sync.py
 src/spcm/classes_time_stamp.py
 src/spcm/classes_trigger.py
+src/spcm/classes_unit_conversion.py
 src/spcm/constants.py
 src/spcm/pyspcm.py
 src/spcm/regs.py
 src/spcm/spcerr.py
 src/spcm.egg-info/PKG-INFO
 src/spcm.egg-info/SOURCES.txt
 src/spcm.egg-info/dependency_links.txt
```

### Comparing `spcm-1.0.6/versioneer.py` & `spcm-1.1.0/versioneer.py`

 * *Files identical despite different names*

