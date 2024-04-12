# Comparing `tmp/OSBModelValidation-0.2.18.tar.gz` & `tmp/OSBModelValidation-0.2.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OSBModelValidation-0.2.18.tar", last modified: Thu Apr 11 09:46:56 2024, max compression
+gzip compressed data, was "OSBModelValidation-0.2.19.tar", last modified: Fri Apr 12 09:03:23 2024, max compression
```

## Comparing `OSBModelValidation-0.2.18.tar` & `OSBModelValidation-0.2.19.tar`

### file list

```diff
@@ -1,140 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:46:56.258583 OSBModelValidation-0.2.18/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:46:56.258583 OSBModelValidation-0.2.18/OSBModelValidation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10809 2024-04-11 09:46:56.000000 OSBModelValidation-0.2.18/OSBModelValidation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-11 09:46:56.000000 OSBModelValidation-0.2.18/OSBModelValidation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:46:56.000000 OSBModelValidation-0.2.18/OSBModelValidation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-11 09:46:56.000000 OSBModelValidation-0.2.18/OSBModelValidation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-11 09:46:56.000000 OSBModelValidation-0.2.18/OSBModelValidation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-11 09:46:56.000000 OSBModelValidation-0.2.18/OSBModelValidation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10809 2024-04-11 09:46:56.258583 OSBModelValidation-0.2.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9791 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:46:56.238583 OSBModelValidation-0.2.18/omv/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:46:56.242583 OSBModelValidation-0.2.18/omv/analyzers/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/analyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/analyzers/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/analyzers/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/analyzers/dryrun.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/analyzers/input_resistance.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/analyzers/morphology.py
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/analyzers/rates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/analyzers/resting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/analyzers/spikes.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/analyzers/temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/analyzers/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:46:56.242583 OSBModelValidation-0.2.18/omv/analyzers/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/analyzers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/analyzers/utils/filenode.py
--rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/analyzers/utils/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/autogen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:46:56.242583 OSBModelValidation-0.2.18/omv/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/common/inout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:46:56.254583 OSBModelValidation-0.2.18/omv/engines/
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/arbor_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/brian1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/brian2_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/eden_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/genesis.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/getarbor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/getbrian1.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/getbrian2.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/geteden.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/getgenesis.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/getjlems.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/getjnml.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/getlibsbml.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/getmoose.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/getnest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/getnetpyne.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/getneuroconstruct.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/getnml2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/getnrn.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/getoctave.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/getpylems.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/getpyneuroml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/getpynn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/jlems.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/jneuroml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/jneuromlbrian.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/jneuromlbrian2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/jneuromleden.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/jneuromlmoose.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/jneuromlnetpyne.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/jneuromlnetpyne_np2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/jneuromlnetpyne_np4.py
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/jneuromlnrn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/jneuromlpynnnrn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/jneuromlvalidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/jneuromlvalidatev1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/moose_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/nestsli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/netpyne_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/netpyne__np2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/netpyne__np4.py
--rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/neuron_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/octave.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/pylems.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/pylemsnml2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/pynest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/pyneuroconstruct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/pyneuroml_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/pyneuromlvalidatesbml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/pyneuron.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/pynn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/pynnbrian1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/pynnbrian2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/pynnnest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/pynnneuroml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/pynnneuron.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:46:56.254583 OSBModelValidation-0.2.18/omv/engines/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/utils/genesis_utils.g
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/engines/utils/wdir.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/find_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/omt_mep_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    14466 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/omv_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/parse_omt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:46:56.254583 OSBModelValidation-0.2.18/omv/schemata/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/schemata/mep.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:46:56.254583 OSBModelValidation-0.2.18/omv/schemata/types/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:46:56.254583 OSBModelValidation-0.2.18/omv/schemata/types/base/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/schemata/types/base/observable_datafile.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/schemata/types/base/observable_literal.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/schemata/types/base/observables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:46:56.258583 OSBModelValidation-0.2.18/omv/schemata/types/base/test/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/schemata/types/base/test/observable_datafile.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/schemata/types/base/test/observable_literal.1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/schemata/types/base/test/observable_literal.3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/schemata/types/expected.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/schemata/types/experiment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/schemata/types/observable.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/schemata/types/protocol.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/schemata/types/protocol_properties.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:46:56.258583 OSBModelValidation-0.2.18/omv/schemata/types/test/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/schemata/types/test/expected.1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/schemata/types/test/expected.2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/schemata/types/test/expected.3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/schemata/types/test/expected.4.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/schemata/types/test/experiment.1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/schemata/types/test/experiment.2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/schemata/types/test/observable.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/schemata/types/test/protocol.1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/schemata/types/test/protocol.2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/tally.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:46:56.258583 OSBModelValidation-0.2.18/omv/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/test/test_rates.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/test/test_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:46:56.258583 OSBModelValidation-0.2.18/omv/validation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/validation/rx_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/validation/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/validation/validate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      380 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/omv/validation/validate_mep.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-11 09:46:52.000000 OSBModelValidation-0.2.18/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-11 09:46:56.258583 OSBModelValidation-0.2.18/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:03:23.619694 OSBModelValidation-0.2.19/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/LICENSE.lesser
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:03:23.619694 OSBModelValidation-0.2.19/OSBModelValidation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10830 2024-04-12 09:03:23.000000 OSBModelValidation-0.2.19/OSBModelValidation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-12 09:03:23.000000 OSBModelValidation-0.2.19/OSBModelValidation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:03:23.000000 OSBModelValidation-0.2.19/OSBModelValidation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-12 09:03:23.000000 OSBModelValidation-0.2.19/OSBModelValidation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-12 09:03:23.000000 OSBModelValidation-0.2.19/OSBModelValidation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-12 09:03:23.000000 OSBModelValidation-0.2.19/OSBModelValidation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10830 2024-04-12 09:03:23.619694 OSBModelValidation-0.2.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9783 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:03:23.599694 OSBModelValidation-0.2.19/omv/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:03:23.599694 OSBModelValidation-0.2.19/omv/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/analyzers/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/analyzers/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/analyzers/dryrun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/analyzers/input_resistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/analyzers/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/analyzers/rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/analyzers/resting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/analyzers/spikes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/analyzers/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/analyzers/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:03:23.603694 OSBModelValidation-0.2.19/omv/analyzers/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/analyzers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/analyzers/utils/filenode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/analyzers/utils/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/autogen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:03:23.603694 OSBModelValidation-0.2.19/omv/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/common/inout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:03:23.611694 OSBModelValidation-0.2.19/omv/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/arbor_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/brian1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/brian2_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/eden_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/genesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/getarbor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/getbrian1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/getbrian2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/geteden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/getgenesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/getjlems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/getjnml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/getlibsbml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/getmoose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/getnest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/getnetpyne.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/getneuroconstruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/getnml2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/getnrn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/getoctave.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/getpylems.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/getpyneuroml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/getpynn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/jlems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/jneuroml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/jneuromlbrian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/jneuromlbrian2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/jneuromleden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/jneuromlmoose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/jneuromlnetpyne.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/jneuromlnetpyne_np2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/jneuromlnetpyne_np4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/jneuromlnrn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/jneuromlpynnnrn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/jneuromlvalidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/jneuromlvalidatev1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/moose_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/nestsli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/netpyne_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/netpyne__np2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/netpyne__np4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/neuron_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/octave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/pylems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/pylemsnml2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/pynest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/pyneuroconstruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/pyneuroml_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/pyneuromlvalidatesbml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/pyneuron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/pynn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/pynnbrian1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/pynnbrian2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/pynnnest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/pynnneuroml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/pynnneuron.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:03:23.611694 OSBModelValidation-0.2.19/omv/engines/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/utils/genesis_utils.g
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/engines/utils/wdir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/find_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/omt_mep_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14890 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/omv_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/parse_omt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:03:23.611694 OSBModelValidation-0.2.19/omv/schemata/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/schemata/mep.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:03:23.615694 OSBModelValidation-0.2.19/omv/schemata/types/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:03:23.615694 OSBModelValidation-0.2.19/omv/schemata/types/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/schemata/types/base/observable_datafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/schemata/types/base/observable_literal.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/schemata/types/base/observables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:03:23.615694 OSBModelValidation-0.2.19/omv/schemata/types/base/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/schemata/types/base/test/observable_datafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/schemata/types/base/test/observable_literal.1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/schemata/types/base/test/observable_literal.3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/schemata/types/expected.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/schemata/types/experiment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/schemata/types/observable.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/schemata/types/protocol.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/schemata/types/protocol_properties.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:03:23.615694 OSBModelValidation-0.2.19/omv/schemata/types/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/schemata/types/test/expected.1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/schemata/types/test/expected.2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/schemata/types/test/expected.3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/schemata/types/test/expected.4.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/schemata/types/test/experiment.1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/schemata/types/test/experiment.2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/schemata/types/test/observable.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/schemata/types/test/protocol.1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/schemata/types/test/protocol.2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/tally.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:03:23.615694 OSBModelValidation-0.2.19/omv/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/test/test_rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/test/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:03:23.619694 OSBModelValidation-0.2.19/omv/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/validation/rx_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/validation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/validation/validate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      380 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/omv/validation/validate_mep.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-12 09:03:20.000000 OSBModelValidation-0.2.19/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-12 09:03:23.619694 OSBModelValidation-0.2.19/setup.cfg
```

### Comparing `OSBModelValidation-0.2.18/OSBModelValidation.egg-info/PKG-INFO` & `OSBModelValidation-0.2.19/OSBModelValidation.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OSBModelValidation
-Version: 0.2.18
+Version: 0.2.19
 Summary: Open Source Brain Model validation
 Home-page: https://github.com/OpenSourceBrain/osb-model-validation
 Author: Boris Marin, Padraig Gleeson
 Author-email: borismarin@gmail.com
 License: LGPL-3.0-only
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -13,24 +13,25 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
+License-File: LICENSE.lesser
 Requires-Dist: PyYAML
 Requires-Dist: numpy
 Requires-Dist: pyrx
 Requires-Dist: pathlib; python_version < "3.4"
 Requires-Dist: docopt
 Requires-Dist: importlib-metadata; python_version < "3.8"
 
 [![Continuous builds](https://github.com/OpenSourceBrain/osb-model-validation/actions/workflows/ci.yml/badge.svg)](https://github.com/OpenSourceBrain/osb-model-validation/actions/workflows/ci.yml)
-[![PyPI](https://img.shields.io/pypi/v/osb-model-validation)](https://pypi.org/project/osb-model-validation/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/osb-model-validation)](https://pypi.org/project/osb-model-validation/)
+[![PyPI](https://img.shields.io/pypi/v/OSBModelValidation)](https://pypi.org/project/OSBModelValidation/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/OSBModelValidation)](https://pypi.org/project/OSBModelValidation/)
 [![GitHub](https://img.shields.io/github/license/OpenSourceBrain/osb-model-validation)](https://github.com/OpenSourceBrain/osb-model-validation/blob/master/LICENSE.lesser)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/OpenSourceBrain/osb-model-validation)](https://github.com/OpenSourceBrain/osb-model-validation/pulls)
 [![GitHub issues](https://img.shields.io/github/issues/OpenSourceBrain/osb-model-validation)](https://github.com/OpenSourceBrain/osb-model-validation/issues)
 [![Gitter](https://badges.gitter.im/NeuroML/community.svg)](https://gitter.im/NeuroML/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 ------------------------------------------
 
 # OSB Model Validation
```

### Comparing `OSBModelValidation-0.2.18/OSBModelValidation.egg-info/SOURCES.txt` & `OSBModelValidation-0.2.19/OSBModelValidation.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.lesser
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 OSBModelValidation.egg-info/PKG-INFO
 OSBModelValidation.egg-info/SOURCES.txt
 OSBModelValidation.egg-info/dependency_links.txt
```

### Comparing `OSBModelValidation-0.2.18/PKG-INFO` & `OSBModelValidation-0.2.19/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OSBModelValidation
-Version: 0.2.18
+Version: 0.2.19
 Summary: Open Source Brain Model validation
 Home-page: https://github.com/OpenSourceBrain/osb-model-validation
 Author: Boris Marin, Padraig Gleeson
 Author-email: borismarin@gmail.com
 License: LGPL-3.0-only
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -13,24 +13,25 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
+License-File: LICENSE.lesser
 Requires-Dist: PyYAML
 Requires-Dist: numpy
 Requires-Dist: pyrx
 Requires-Dist: pathlib; python_version < "3.4"
 Requires-Dist: docopt
 Requires-Dist: importlib-metadata; python_version < "3.8"
 
 [![Continuous builds](https://github.com/OpenSourceBrain/osb-model-validation/actions/workflows/ci.yml/badge.svg)](https://github.com/OpenSourceBrain/osb-model-validation/actions/workflows/ci.yml)
-[![PyPI](https://img.shields.io/pypi/v/osb-model-validation)](https://pypi.org/project/osb-model-validation/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/osb-model-validation)](https://pypi.org/project/osb-model-validation/)
+[![PyPI](https://img.shields.io/pypi/v/OSBModelValidation)](https://pypi.org/project/OSBModelValidation/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/OSBModelValidation)](https://pypi.org/project/OSBModelValidation/)
 [![GitHub](https://img.shields.io/github/license/OpenSourceBrain/osb-model-validation)](https://github.com/OpenSourceBrain/osb-model-validation/blob/master/LICENSE.lesser)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/OpenSourceBrain/osb-model-validation)](https://github.com/OpenSourceBrain/osb-model-validation/pulls)
 [![GitHub issues](https://img.shields.io/github/issues/OpenSourceBrain/osb-model-validation)](https://github.com/OpenSourceBrain/osb-model-validation/issues)
 [![Gitter](https://badges.gitter.im/NeuroML/community.svg)](https://gitter.im/NeuroML/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 ------------------------------------------
 
 # OSB Model Validation
```

### Comparing `OSBModelValidation-0.2.18/README.md` & `OSBModelValidation-0.2.19/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [![Continuous builds](https://github.com/OpenSourceBrain/osb-model-validation/actions/workflows/ci.yml/badge.svg)](https://github.com/OpenSourceBrain/osb-model-validation/actions/workflows/ci.yml)
-[![PyPI](https://img.shields.io/pypi/v/osb-model-validation)](https://pypi.org/project/osb-model-validation/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/osb-model-validation)](https://pypi.org/project/osb-model-validation/)
+[![PyPI](https://img.shields.io/pypi/v/OSBModelValidation)](https://pypi.org/project/OSBModelValidation/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/OSBModelValidation)](https://pypi.org/project/OSBModelValidation/)
 [![GitHub](https://img.shields.io/github/license/OpenSourceBrain/osb-model-validation)](https://github.com/OpenSourceBrain/osb-model-validation/blob/master/LICENSE.lesser)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/OpenSourceBrain/osb-model-validation)](https://github.com/OpenSourceBrain/osb-model-validation/pulls)
 [![GitHub issues](https://img.shields.io/github/issues/OpenSourceBrain/osb-model-validation)](https://github.com/OpenSourceBrain/osb-model-validation/issues)
 [![Gitter](https://badges.gitter.im/NeuroML/community.svg)](https://gitter.im/NeuroML/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 ------------------------------------------
 
 # OSB Model Validation
```

### Comparing `OSBModelValidation-0.2.18/omv/analyzers/__init__.py` & `OSBModelValidation-0.2.19/omv/analyzers/__init__.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/analyzers/activation.py` & `OSBModelValidation-0.2.19/omv/analyzers/activation.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/analyzers/analyzer.py` & `OSBModelValidation-0.2.19/omv/analyzers/analyzer.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/analyzers/input_resistance.py` & `OSBModelValidation-0.2.19/omv/analyzers/input_resistance.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/analyzers/morphology.py` & `OSBModelValidation-0.2.19/omv/analyzers/morphology.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/analyzers/rates.py` & `OSBModelValidation-0.2.19/omv/analyzers/rates.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/analyzers/resting.py` & `OSBModelValidation-0.2.19/omv/analyzers/resting.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/analyzers/spikes.py` & `OSBModelValidation-0.2.19/omv/analyzers/spikes.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/analyzers/timeseries.py` & `OSBModelValidation-0.2.19/omv/analyzers/timeseries.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/analyzers/utils/filenode.py` & `OSBModelValidation-0.2.19/omv/analyzers/utils/filenode.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/analyzers/utils/timeseries.py` & `OSBModelValidation-0.2.19/omv/analyzers/utils/timeseries.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/autogen.py` & `OSBModelValidation-0.2.19/omv/autogen.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/common/inout.py` & `OSBModelValidation-0.2.19/omv/common/inout.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/__init__.py` & `OSBModelValidation-0.2.19/omv/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/arbor_.py` & `OSBModelValidation-0.2.19/omv/engines/arbor_.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/brian1.py` & `OSBModelValidation-0.2.19/omv/engines/brian1.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/brian2_.py` & `OSBModelValidation-0.2.19/omv/engines/brian2_.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         ret = True
         try:
             import brian2
 
             inform(
                 "Brian2 version %s is correctly installed..." % brian2.__version__,
                 indent=2,
-                verbosity=2,
+                verbosity=1,
             )
 
             ret = "v%s" % brian2.__version__
 
         except Exception as err:
             inform("Couldn't import Brian2 into Python: ", err, indent=1, verbosity=1)
             ret = False
```

### Comparing `OSBModelValidation-0.2.18/omv/engines/eden_.py` & `OSBModelValidation-0.2.19/omv/engines/eden_.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/engine.py` & `OSBModelValidation-0.2.19/omv/engines/engine.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/genesis.py` & `OSBModelValidation-0.2.19/omv/engines/genesis.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/getbrian1.py` & `OSBModelValidation-0.2.19/omv/engines/getbrian1.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/getgenesis.py` & `OSBModelValidation-0.2.19/omv/engines/getgenesis.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/getjlems.py` & `OSBModelValidation-0.2.19/omv/engines/getjlems.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/getjnml.py` & `OSBModelValidation-0.2.19/omv/engines/getjnml.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/getnest.py` & `OSBModelValidation-0.2.19/omv/engines/getnest.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/getnetpyne.py` & `OSBModelValidation-0.2.19/omv/engines/getnetpyne.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/getneuroconstruct.py` & `OSBModelValidation-0.2.19/omv/engines/getneuroconstruct.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/getnml2.py` & `OSBModelValidation-0.2.19/omv/engines/getnml2.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/getnrn.py` & `OSBModelValidation-0.2.19/omv/engines/getnrn.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/getpynn.py` & `OSBModelValidation-0.2.19/omv/engines/getpynn.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/jlems.py` & `OSBModelValidation-0.2.19/omv/engines/jlems.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/jneuroml.py` & `OSBModelValidation-0.2.19/omv/engines/jneuroml.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/jneuromlbrian.py` & `OSBModelValidation-0.2.19/omv/engines/jneuromlbrian.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/jneuromlbrian2.py` & `OSBModelValidation-0.2.19/omv/engines/jneuromlbrian2.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/jneuromleden.py` & `OSBModelValidation-0.2.19/omv/engines/jneuromleden.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/jneuromlmoose.py` & `OSBModelValidation-0.2.19/omv/engines/jneuromlmoose.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,38 +4,41 @@
 from omv.engines.jneuroml import JNeuroMLEngine
 from omv.engines.moose_ import MooseEngine
 from omv.common.inout import inform, trim_path, check_output, is_verbose
 from omv.engines.engine import EngineExecutionError
 
 
 class JNeuroMLMooseEngine(JNeuroMLEngine):
+
     name = "jNeuroML_Moose"
 
     @staticmethod
     def is_installed():
         if is_verbose():
             inform(
                 "Checking whether %s is installed..." % JNeuroMLMooseEngine.name,
                 indent=1,
             )
         return JNeuroMLEngine.is_installed() and MooseEngine.is_installed()
 
     @staticmethod
     def install(version):
+
         if not JNeuroMLEngine.is_installed():
             JNeuroMLEngine.install(None)
         if not MooseEngine.is_installed():
-            MooseEngine.install(None)
+            MooseEngine.install(version)
 
         JNeuroMLMooseEngine.path = JNeuroMLEngine.path + ":" + JNeuroMLMooseEngine.path
         JNeuroMLMooseEngine.environment_vars = {}
         JNeuroMLMooseEngine.environment_vars.update(JNeuroMLEngine.environment_vars)
         JNeuroMLMooseEngine.environment_vars.update(MooseEngine.environment_vars)
         inform("PATH: " + JNeuroMLMooseEngine.path)
         inform("Env vars: %s" % JNeuroMLMooseEngine.environment_vars)
+        
 
     def run(self):
         try:
             inform(
                 "Running file %s with %s"
                 % (trim_path(self.modelpath), JNeuroMLMooseEngine.name),
                 indent=1,
```

### Comparing `OSBModelValidation-0.2.18/omv/engines/jneuromlnetpyne.py` & `OSBModelValidation-0.2.19/omv/engines/jneuromlnetpyne.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/jneuromlnetpyne_np2.py` & `OSBModelValidation-0.2.19/omv/engines/jneuromlnetpyne_np2.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/jneuromlnetpyne_np4.py` & `OSBModelValidation-0.2.19/omv/engines/jneuromlnetpyne_np4.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/jneuromlnrn.py` & `OSBModelValidation-0.2.19/omv/engines/jneuromlnrn.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/jneuromlpynnnrn.py` & `OSBModelValidation-0.2.19/omv/engines/jneuromlpynnnrn.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/jneuromlvalidate.py` & `OSBModelValidation-0.2.19/omv/engines/jneuromlvalidate.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/jneuromlvalidatev1.py` & `OSBModelValidation-0.2.19/omv/engines/jneuromlvalidatev1.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/moose_.py` & `OSBModelValidation-0.2.19/omv/engines/moose_.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,52 +6,32 @@
 from omv.common.inout import inform, trim_path, check_output, is_verbose
 from omv.engines.engine import OMVEngine, EngineExecutionError
 
 
 class MooseEngine(OMVEngine):
     name = "Moose"
 
+
     @staticmethod
     def is_installed():
-        if is_verbose():
-            inform(
-                "Checking whether the engine %s has been installed correctly..."
-                % MooseEngine.name,
-                indent=1,
-            )
-
         ret = True
         try:
-            ret_str = sp.check_output(
-                ['python -c "import moose; print(moose.__version__)"'],
-                shell=True,
-                stderr=sp.STDOUT,
-            )
-            ret = len(ret_str) > 0
+            import moose
 
-            if isinstance(ret_str, bytes):
-                ret_str = ret_str.decode("utf-8").strip()
+            inform(
+                "Moose version %s is correctly installed..." % moose.__version__,
+                indent=2,
+                verbosity=1,
+            )
 
-            if ret and is_verbose():
-                inform(
-                    "%s is correctly installed (%s)..." % (MooseEngine.name, ret_str),
-                    indent=2,
-                )
-            if ret:
-                # import moose
-                ret = "v%s" % ret_str
+            ret = "v%s" % moose.__version__
 
         except Exception as err:
-            if is_verbose():
-                inform("Couldn't import moose into Python: ", err, indent=1)
+            inform("Couldn't import Moose into Python: ", err, indent=1, verbosity=1)
             ret = False
-        if not ret or not PyNeuroMLEngine.is_installed():
-            ret = False
-
-        inform("Moose is_installed(): %s" % ret, "", indent=1, verbosity=2)
         return ret
 
     @staticmethod
     def install(version):
         if not PyNeuroMLEngine.is_installed():
             PyNeuroMLEngine.install(None)
             inform(
```

### Comparing `OSBModelValidation-0.2.18/omv/engines/nestsli.py` & `OSBModelValidation-0.2.19/omv/engines/nestsli.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/netpyne_.py` & `OSBModelValidation-0.2.19/omv/engines/netpyne_.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/netpyne__np2.py` & `OSBModelValidation-0.2.19/omv/engines/netpyne__np2.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/netpyne__np4.py` & `OSBModelValidation-0.2.19/omv/engines/netpyne__np4.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/neuron_.py` & `OSBModelValidation-0.2.19/omv/engines/neuron_.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/octave.py` & `OSBModelValidation-0.2.19/omv/engines/octave.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/pylems.py` & `OSBModelValidation-0.2.19/omv/engines/pylems.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/pylemsnml2.py` & `OSBModelValidation-0.2.19/omv/engines/pylemsnml2.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/pynest.py` & `OSBModelValidation-0.2.19/omv/engines/pynest.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/pyneuroconstruct.py` & `OSBModelValidation-0.2.19/omv/engines/pyneuroconstruct.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/pyneuroml_.py` & `OSBModelValidation-0.2.19/omv/engines/pyneuroml_.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/pyneuromlvalidatesbml.py` & `OSBModelValidation-0.2.19/omv/engines/pyneuromlvalidatesbml.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/pyneuron.py` & `OSBModelValidation-0.2.19/omv/engines/pyneuron.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/pynn.py` & `OSBModelValidation-0.2.19/omv/engines/pynn.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/pynnbrian1.py` & `OSBModelValidation-0.2.19/omv/engines/pynnbrian1.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/pynnbrian2.py` & `OSBModelValidation-0.2.19/omv/engines/pynnbrian2.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/pynnnest.py` & `OSBModelValidation-0.2.19/omv/engines/pynnnest.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/pynnneuroml.py` & `OSBModelValidation-0.2.19/omv/engines/pynnneuroml.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/pynnneuron.py` & `OSBModelValidation-0.2.19/omv/engines/pynnneuron.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/engines/utils/genesis_utils.g` & `OSBModelValidation-0.2.19/omv/engines/utils/genesis_utils.g`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/experiment.py` & `OSBModelValidation-0.2.19/omv/experiment.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/find_tests.py` & `OSBModelValidation-0.2.19/omv/find_tests.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/omt_mep_parser.py` & `OSBModelValidation-0.2.19/omv/omt_mep_parser.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/omv_util.py` & `OSBModelValidation-0.2.19/omv/omv_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -335,47 +335,61 @@
             if engine_version is not None:
                 raise Exception(
                     "Currently, cannot install a specific version of engine %s" % eng
                 )
             from omv.engines.getgenesis import install_genesis
 
             install_genesis()
+
         elif eng.lower() == "Moose".lower():
-            if engine_version is not None:
-                raise Exception(
-                    "Currently, cannot install a specific version of engine %s" % eng
-                )
-            from omv.engines.getmoose import install_moose
 
-            install_moose(engine_version)
+            from omv.engines.moose_ import MooseEngine as ee
+
+            if ee.is_installed():
+                already_installed = True
+            else:
+                from omv.engines.getmoose import install_moose
+
+                install_moose(engine_version)
+
         elif eng.lower() == "NetPyNE".lower():
             from omv.engines.getnetpyne import install_netpyne
 
             install_netpyne(engine_version)
+
         elif eng.lower() == "Brian".lower():
+
             if engine_version is not None:
                 raise Exception(
                     "Currently, cannot install a specific version of engine %s" % eng
                 )
             from omv.engines.getbrian1 import install_brian
 
             install_brian()
+
         elif eng.lower() == "Brian2".lower():
-            from omv.engines.getbrian2 import install_brian2
+            from omv.engines.brian2_ import Brian2Engine as ee
+
+            if ee.is_installed():
+                already_installed = True
+            else:
+                from omv.engines.getbrian2 import install_brian2
+
+                install_brian2(engine_version)
 
-            install_brian2(engine_version)
         elif eng.lower() == "NEST".lower():
             from omv.engines.nestsli import NestEngine as ee
 
             if ee.is_installed():
                 already_installed = True
             else:
                 from omv.engines.getnest import install_nest
 
                 install_nest(engine_version)
+
         elif eng.lower() == "PyNEST".lower():
             from omv.engines.pynest import PyNestEngine as ee
 
             if ee.is_installed():
                 already_installed = True
             else:
                 from omv.engines.getnest import install_nest
@@ -399,14 +413,22 @@
             from omv.engines.jneuromlbrian2 import JNeuroMLBrian2Engine as ee
 
             if ee.is_installed():
                 already_installed = True
             else:
                 ee.install(engine_version)
 
+        elif eng.lower() == "jNeuroML_Moose".lower():
+            from omv.engines.jneuromlmoose import JNeuroMLMooseEngine as ee
+
+            if ee.is_installed():
+                already_installed = True
+            else:
+                ee.install(engine_version)
+
         elif eng.lower() == "jNeuroML_NEURON".lower():
             from omv.engines.jneuromlnrn import JNeuroMLNRNEngine as ee
 
             if ee.is_installed():
                 already_installed = True
             else:
                 ee.install(engine_version)
```

### Comparing `OSBModelValidation-0.2.18/omv/parse_omt.py` & `OSBModelValidation-0.2.19/omv/parse_omt.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/schemata/types/test/experiment.2.yaml` & `OSBModelValidation-0.2.19/omv/schemata/types/test/experiment.2.yaml`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/tally.py` & `OSBModelValidation-0.2.19/omv/tally.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/test/test_rates.py` & `OSBModelValidation-0.2.19/omv/test/test_rates.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/test/test_types.py` & `OSBModelValidation-0.2.19/omv/test/test_types.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/validation/rx_validator.py` & `OSBModelValidation-0.2.19/omv/validation/rx_validator.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/validation/utils.py` & `OSBModelValidation-0.2.19/omv/validation/utils.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/omv/validation/validate.py` & `OSBModelValidation-0.2.19/omv/validation/validate.py`

 * *Files identical despite different names*

### Comparing `OSBModelValidation-0.2.18/setup.cfg` & `OSBModelValidation-0.2.19/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = OSBModelValidation
-version = 0.2.18
+version = 0.2.19
 author = Boris Marin, Padraig Gleeson
 author_email = borismarin@gmail.com
 url = https://github.com/OpenSourceBrain/osb-model-validation
 license = LGPL-3.0-only
 description = Open Source Brain Model validation
 long_description = file: README.md
 long_description_content_type = text/markdown
```

