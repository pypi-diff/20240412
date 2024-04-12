# Comparing `tmp/protkit-0.2.2.tar.gz` & `tmp/protkit-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protkit-0.2.2.tar", last modified: Wed Apr  3 08:16:43 2024, max compression
+gzip compressed data, was "protkit-0.2.3.tar", last modified: Fri Apr 12 10:46:07 2024, max compression
```

## Comparing `protkit-0.2.2.tar` & `protkit-0.2.3.tar`

### file list

```diff
@@ -1,84 +1,99 @@
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.289593 protkit-0.2.2/
--rw-rw-r--   0 fred      (1000) fred      (1000)    35149 2024-02-20 10:58:14.000000 protkit-0.2.2/LICENSE
--rw-r--r--   0 fred      (1000) fred      (1000)    18905 2024-04-03 08:16:43.289593 protkit-0.2.2/PKG-INFO
--rw-rw-r--   0 fred      (1000) fred      (1000)    17718 2024-03-06 07:08:30.000000 protkit-0.2.2/README.md
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.285593 protkit-0.2.2/protkit/
--rw-rw-r--   0 fred      (1000) fred      (1000)     5279 2024-03-08 06:45:24.000000 protkit-0.2.2/protkit/__init__.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.285593 protkit-0.2.2/protkit/core/
--rw-rw-r--   0 fred      (1000) fred      (1000)      135 2024-02-20 13:59:59.000000 protkit-0.2.2/protkit/core/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     2609 2024-01-30 10:27:10.000000 protkit-0.2.2/protkit/core/extend_attributes.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.285593 protkit-0.2.2/protkit/download/
--rw-rw-r--   0 fred      (1000) fred      (1000)      395 2024-02-20 11:32:28.000000 protkit-0.2.2/protkit/download/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    12986 2024-03-11 08:37:40.000000 protkit-0.2.2/protkit/download/download.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.285593 protkit-0.2.2/protkit/file_io/
--rw-rw-r--   0 fred      (1000) fred      (1000)      786 2024-02-20 11:40:22.000000 protkit-0.2.2/protkit/file_io/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     3870 2024-03-11 10:09:24.000000 protkit-0.2.2/protkit/file_io/fasta_io.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     3532 2024-02-20 11:40:22.000000 protkit-0.2.2/protkit/file_io/mmcif_io.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     3405 2024-02-20 11:40:22.000000 protkit-0.2.2/protkit/file_io/mmtf_io.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    44013 2024-04-02 14:47:49.000000 protkit-0.2.2/protkit/file_io/pdb_io.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     1134 2024-02-20 11:40:22.000000 protkit-0.2.2/protkit/file_io/pqr_io.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     9969 2024-02-20 11:40:22.000000 protkit-0.2.2/protkit/file_io/prot_io.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.285593 protkit-0.2.2/protkit/geometry/
--rw-rw-r--   0 fred      (1000) fred      (1000)      147 2024-02-23 12:55:57.000000 protkit-0.2.2/protkit/geometry/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     7717 2024-02-15 08:53:21.000000 protkit-0.2.2/protkit/geometry/math.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     5103 2024-02-15 12:04:44.000000 protkit-0.2.2/protkit/geometry/space_query.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.289593 protkit-0.2.2/protkit/metrics/
--rw-rw-r--   0 fred      (1000) fred      (1000)     1160 2024-02-23 12:57:26.000000 protkit-0.2.2/protkit/metrics/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)      272 2024-01-24 11:20:02.000000 protkit-0.2.2/protkit/metrics/classification_eval.py
--rw-rw-r--   0 fred      (1000) fred      (1000)      259 2024-01-24 11:20:02.000000 protkit-0.2.2/protkit/metrics/regression_eval.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     5566 2024-02-23 12:57:27.000000 protkit-0.2.2/protkit/metrics/scoring_matrix.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     6063 2024-02-02 14:13:32.000000 protkit-0.2.2/protkit/metrics/sequence_eval.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     3172 2024-01-31 09:20:40.000000 protkit-0.2.2/protkit/metrics/structure_eval.py
--rw-rw-r--   0 fred      (1000) fred      (1000)      339 2024-01-24 11:18:08.000000 protkit-0.2.2/protkit/metrics/utility_eval.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.289593 protkit-0.2.2/protkit/properties/
--rw-rw-r--   0 fred      (1000) fred      (1000)     1076 2024-04-03 08:07:25.000000 protkit-0.2.2/protkit/properties/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     9887 2024-02-14 09:21:12.000000 protkit-0.2.2/protkit/properties/bond_angles.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    10870 2024-02-14 09:21:12.000000 protkit-0.2.2/protkit/properties/bond_lengths.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    10763 2024-03-07 14:33:32.000000 protkit-0.2.2/protkit/properties/bounds.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     4785 2024-02-06 10:51:06.000000 protkit-0.2.2/protkit/properties/charge.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     4652 2024-03-06 08:28:16.000000 protkit-0.2.2/protkit/properties/chemical_class.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     4661 2024-03-06 15:04:02.000000 protkit-0.2.2/protkit/properties/circular_variance.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     8207 2024-02-15 09:39:07.000000 protkit-0.2.2/protkit/properties/dihedral_angles.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    18567 2024-03-06 09:40:04.000000 protkit-0.2.2/protkit/properties/donors_acceptors.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    11621 2024-03-06 08:07:46.000000 protkit-0.2.2/protkit/properties/hydrophobicity.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     6987 2024-02-15 13:14:20.000000 protkit-0.2.2/protkit/properties/interface.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    12504 2024-03-06 08:11:59.000000 protkit-0.2.2/protkit/properties/mass.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     5162 2024-03-06 08:38:24.000000 protkit-0.2.2/protkit/properties/polarity.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     4202 2024-02-28 11:35:22.000000 protkit-0.2.2/protkit/properties/surface_area.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     3595 2024-02-23 13:15:30.000000 protkit-0.2.2/protkit/properties/vdw_radius.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     9901 2024-03-06 11:18:19.000000 protkit-0.2.2/protkit/properties/volume.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.289593 protkit-0.2.2/protkit/seq/
--rw-rw-r--   0 fred      (1000) fred      (1000)      682 2024-02-20 13:57:49.000000 protkit-0.2.2/protkit/seq/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)      952 2024-02-20 11:40:22.000000 protkit-0.2.2/protkit/seq/antibody_sequence.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     1220 2024-02-20 11:40:22.000000 protkit-0.2.2/protkit/seq/nucleotide_sequence.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     3624 2024-02-20 11:40:22.000000 protkit-0.2.2/protkit/seq/protein_sequence.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     5710 2024-03-11 10:00:59.000000 protkit-0.2.2/protkit/seq/sequence.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     5473 2024-02-20 11:40:22.000000 protkit-0.2.2/protkit/seq/sequence_alignment.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.289593 protkit-0.2.2/protkit/structure/
--rw-rw-r--   0 fred      (1000) fred      (1000)      516 2024-01-22 13:13:22.000000 protkit-0.2.2/protkit/structure/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    11726 2024-02-20 11:51:26.000000 protkit-0.2.2/protkit/structure/atom.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    19490 2024-03-06 15:18:38.000000 protkit-0.2.2/protkit/structure/chain.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    24100 2024-03-06 12:09:29.000000 protkit-0.2.2/protkit/structure/protein.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    20645 2024-03-06 15:24:06.000000 protkit-0.2.2/protkit/structure/residue.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.289593 protkit-0.2.2/protkit/tasks/
--rw-rw-r--   0 fred      (1000) fred      (1000)      139 2024-04-03 08:07:09.000000 protkit-0.2.2/protkit/tasks/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     1369 2024-03-08 13:46:26.000000 protkit-0.2.2/protkit/tasks/protonator.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     1619 2024-02-23 13:58:40.000000 protkit-0.2.2/protkit/tasks/surface_area_calculator.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.289593 protkit-0.2.2/protkit/tools/
--rw-rw-r--   0 fred      (1000) fred      (1000)      218 2024-03-08 06:50:53.000000 protkit-0.2.2/protkit/tools/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     3946 2024-03-08 06:54:34.000000 protkit-0.2.2/protkit/tools/freesasa_adaptor.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     8569 2024-04-03 07:58:04.000000 protkit-0.2.2/protkit/tools/reduce_adaptor.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.289593 protkit-0.2.2/protkit.egg-info/
--rw-r--r--   0 fred      (1000) fred      (1000)    18905 2024-04-03 08:16:43.000000 protkit-0.2.2/protkit.egg-info/PKG-INFO
--rw-rw-r--   0 fred      (1000) fred      (1000)     1954 2024-04-03 08:16:43.000000 protkit-0.2.2/protkit.egg-info/SOURCES.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)        1 2024-04-03 08:16:43.000000 protkit-0.2.2/protkit.egg-info/dependency_links.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)      160 2024-04-03 08:16:43.000000 protkit-0.2.2/protkit.egg-info/requires.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)       40 2024-04-03 08:16:43.000000 protkit-0.2.2/protkit.egg-info/top_level.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)     1334 2024-04-03 08:16:03.000000 protkit-0.2.2/pyproject.toml
--rw-rw-r--   0 fred      (1000) fred      (1000)       38 2024-04-03 08:16:43.289593 protkit-0.2.2/setup.cfg
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.289593 protkit-0.2.2/tests/
--rw-rw-r--   0 fred      (1000) fred      (1000)    22661 2024-03-11 14:12:17.000000 protkit-0.2.2/tests/quick_start_guide.py
--rw-rw-r--   0 fred      (1000) fred      (1000)      564 2024-03-26 13:48:46.000000 protkit-0.2.2/tests/test_reduce.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.281593 protkit-0.2.2/venv/
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.289593 protkit-0.2.2/venv/bin/
--rw-rw-r--   0 fred      (1000) fred      (1000)     1336 2024-02-20 10:55:31.000000 protkit-0.2.2/venv/bin/activate_this.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-12 10:46:07.824400 protkit-0.2.3/
+-rw-rw-r--   0 fred      (1000) fred      (1000)    35149 2024-02-20 10:58:14.000000 protkit-0.2.3/LICENSE
+-rw-r--r--   0 fred      (1000) fred      (1000)    18935 2024-04-12 10:46:07.824400 protkit-0.2.3/PKG-INFO
+-rw-rw-r--   0 fred      (1000) fred      (1000)    17718 2024-03-06 07:08:30.000000 protkit-0.2.3/README.md
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-12 10:46:07.816400 protkit-0.2.3/protkit/
+-rw-rw-r--   0 fred      (1000) fred      (1000)     5279 2024-03-08 06:45:24.000000 protkit-0.2.3/protkit/__init__.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-12 10:46:07.816400 protkit-0.2.3/protkit/core/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      135 2024-02-20 13:59:59.000000 protkit-0.2.3/protkit/core/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     2609 2024-01-30 10:27:10.000000 protkit-0.2.3/protkit/core/extend_attributes.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-12 10:46:07.820400 protkit-0.2.3/protkit/download/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      395 2024-02-20 11:32:28.000000 protkit-0.2.3/protkit/download/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    12986 2024-03-11 08:37:40.000000 protkit-0.2.3/protkit/download/download.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-12 10:46:07.820400 protkit-0.2.3/protkit/file_io/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      786 2024-02-20 11:40:22.000000 protkit-0.2.3/protkit/file_io/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3870 2024-03-11 10:09:24.000000 protkit-0.2.3/protkit/file_io/fasta_io.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3532 2024-02-20 11:40:22.000000 protkit-0.2.3/protkit/file_io/mmcif_io.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3405 2024-02-20 11:40:22.000000 protkit-0.2.3/protkit/file_io/mmtf_io.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    49122 2024-04-11 08:41:57.000000 protkit-0.2.3/protkit/file_io/pdb_io.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1134 2024-02-20 11:40:22.000000 protkit-0.2.3/protkit/file_io/pqr_io.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     9969 2024-02-20 11:40:22.000000 protkit-0.2.3/protkit/file_io/prot_io.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-12 10:46:07.820400 protkit-0.2.3/protkit/geometry/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      147 2024-02-23 12:55:57.000000 protkit-0.2.3/protkit/geometry/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     7717 2024-02-15 08:53:21.000000 protkit-0.2.3/protkit/geometry/math.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     5103 2024-02-15 12:04:44.000000 protkit-0.2.3/protkit/geometry/space_query.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-12 10:46:07.820400 protkit-0.2.3/protkit/metrics/
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1160 2024-02-23 12:57:26.000000 protkit-0.2.3/protkit/metrics/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)      272 2024-01-24 11:20:02.000000 protkit-0.2.3/protkit/metrics/classification_eval.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)      259 2024-01-24 11:20:02.000000 protkit-0.2.3/protkit/metrics/regression_eval.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     5566 2024-02-23 12:57:27.000000 protkit-0.2.3/protkit/metrics/scoring_matrix.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     6063 2024-02-02 14:13:32.000000 protkit-0.2.3/protkit/metrics/sequence_eval.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3172 2024-01-31 09:20:40.000000 protkit-0.2.3/protkit/metrics/structure_eval.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)      339 2024-01-24 11:18:08.000000 protkit-0.2.3/protkit/metrics/utility_eval.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-12 10:46:07.820400 protkit-0.2.3/protkit/properties/
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1076 2024-04-11 09:05:09.000000 protkit-0.2.3/protkit/properties/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     9887 2024-02-14 09:21:12.000000 protkit-0.2.3/protkit/properties/bond_angles.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    10870 2024-02-14 09:21:12.000000 protkit-0.2.3/protkit/properties/bond_lengths.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    10763 2024-03-07 14:33:32.000000 protkit-0.2.3/protkit/properties/bounds.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     4785 2024-02-06 10:51:06.000000 protkit-0.2.3/protkit/properties/charge.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     4652 2024-03-06 08:28:16.000000 protkit-0.2.3/protkit/properties/chemical_class.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     4661 2024-03-06 15:04:02.000000 protkit-0.2.3/protkit/properties/circular_variance.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     8207 2024-02-15 09:39:07.000000 protkit-0.2.3/protkit/properties/dihedral_angles.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    18567 2024-03-06 09:40:04.000000 protkit-0.2.3/protkit/properties/donors_acceptors.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    11621 2024-03-06 08:07:46.000000 protkit-0.2.3/protkit/properties/hydrophobicity.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     6987 2024-02-15 13:14:20.000000 protkit-0.2.3/protkit/properties/interface.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    12504 2024-03-06 08:11:59.000000 protkit-0.2.3/protkit/properties/mass.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     5162 2024-03-06 08:38:24.000000 protkit-0.2.3/protkit/properties/polarity.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     4290 2024-04-11 11:55:05.000000 protkit-0.2.3/protkit/properties/surface_area.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3595 2024-02-23 13:15:30.000000 protkit-0.2.3/protkit/properties/vdw_radius.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     9901 2024-03-06 11:18:19.000000 protkit-0.2.3/protkit/properties/volume.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-12 10:46:07.820400 protkit-0.2.3/protkit/seq/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      682 2024-02-20 13:57:49.000000 protkit-0.2.3/protkit/seq/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)      952 2024-02-20 11:40:22.000000 protkit-0.2.3/protkit/seq/antibody_sequence.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1220 2024-02-20 11:40:22.000000 protkit-0.2.3/protkit/seq/nucleotide_sequence.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3624 2024-02-20 11:40:22.000000 protkit-0.2.3/protkit/seq/protein_sequence.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     5710 2024-03-11 10:00:59.000000 protkit-0.2.3/protkit/seq/sequence.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     5473 2024-02-20 11:40:22.000000 protkit-0.2.3/protkit/seq/sequence_alignment.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-12 10:46:07.820400 protkit-0.2.3/protkit/structure/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      516 2024-01-22 13:13:22.000000 protkit-0.2.3/protkit/structure/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    13382 2024-04-12 10:30:44.000000 protkit-0.2.3/protkit/structure/atom.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    19490 2024-03-06 15:18:38.000000 protkit-0.2.3/protkit/structure/chain.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    24100 2024-03-06 12:09:29.000000 protkit-0.2.3/protkit/structure/protein.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    20645 2024-03-06 15:24:06.000000 protkit-0.2.3/protkit/structure/residue.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-12 10:46:07.820400 protkit-0.2.3/protkit/tasks/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      139 2024-04-03 08:07:09.000000 protkit-0.2.3/protkit/tasks/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1369 2024-03-08 13:46:26.000000 protkit-0.2.3/protkit/tasks/protonator.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1619 2024-02-23 13:58:40.000000 protkit-0.2.3/protkit/tasks/surface_area_calculator.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-12 10:46:07.820400 protkit-0.2.3/protkit/tools/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      302 2024-04-12 10:39:42.000000 protkit-0.2.3/protkit/tools/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3946 2024-03-08 06:54:34.000000 protkit-0.2.3/protkit/tools/freesasa_adaptor.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     5488 2024-04-11 08:41:57.000000 protkit-0.2.3/protkit/tools/pdb2pqr_adaptor.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     8569 2024-04-03 07:58:04.000000 protkit-0.2.3/protkit/tools/reduce_adaptor.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-12 10:46:07.824400 protkit-0.2.3/protkit.egg-info/
+-rw-r--r--   0 fred      (1000) fred      (1000)    18935 2024-04-12 10:46:07.000000 protkit-0.2.3/protkit.egg-info/PKG-INFO
+-rw-rw-r--   0 fred      (1000) fred      (1000)     2310 2024-04-12 10:46:07.000000 protkit-0.2.3/protkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)        1 2024-04-12 10:46:07.000000 protkit-0.2.3/protkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)      175 2024-04-12 10:46:07.000000 protkit-0.2.3/protkit.egg-info/requires.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)       45 2024-04-12 10:46:07.000000 protkit-0.2.3/protkit.egg-info/top_level.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1356 2024-04-12 08:46:07.000000 protkit-0.2.3/pyproject.toml
+-rw-rw-r--   0 fred      (1000) fred      (1000)       38 2024-04-12 10:46:07.824400 protkit-0.2.3/setup.cfg
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-12 10:46:07.820400 protkit-0.2.3/tests/
+-rw-rw-r--   0 fred      (1000) fred      (1000)    23316 2024-04-11 12:12:53.000000 protkit-0.2.3/tests/quick_start_guide.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)      192 2024-04-12 10:25:26.000000 protkit-0.2.3/tests/test_occupancy_claudio.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)      638 2024-04-10 12:06:45.000000 protkit-0.2.3/tests/test_pdb2pqr.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)      565 2024-04-10 08:46:58.000000 protkit-0.2.3/tests/test_reduce.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-12 10:46:07.816400 protkit-0.2.3/venv/
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-12 10:46:07.824400 protkit-0.2.3/venv/bin/
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1336 2024-02-20 10:55:31.000000 protkit-0.2.3/venv/bin/activate_this.py
+-rwxrwxr-x   0 fred      (1000) fred      (1000)      612 2024-04-03 10:09:30.000000 protkit-0.2.3/venv/bin/rst2html.py
+-rwxrwxr-x   0 fred      (1000) fred      (1000)      732 2024-04-03 10:09:30.000000 protkit-0.2.3/venv/bin/rst2html4.py
+-rwxrwxr-x   0 fred      (1000) fred      (1000)     1100 2024-04-03 10:09:30.000000 protkit-0.2.3/venv/bin/rst2html5.py
+-rwxrwxr-x   0 fred      (1000) fred      (1000)      809 2024-04-03 10:09:30.000000 protkit-0.2.3/venv/bin/rst2latex.py
+-rwxrwxr-x   0 fred      (1000) fred      (1000)      617 2024-04-03 10:09:30.000000 protkit-0.2.3/venv/bin/rst2man.py
+-rwxrwxr-x   0 fred      (1000) fred      (1000)      782 2024-04-03 10:09:30.000000 protkit-0.2.3/venv/bin/rst2odt.py
+-rwxrwxr-x   0 fred      (1000) fred      (1000)     1744 2024-04-03 10:09:30.000000 protkit-0.2.3/venv/bin/rst2odt_prepstyles.py
+-rwxrwxr-x   0 fred      (1000) fred      (1000)      619 2024-04-03 10:09:30.000000 protkit-0.2.3/venv/bin/rst2pseudoxml.py
+-rwxrwxr-x   0 fred      (1000) fred      (1000)      655 2024-04-03 10:09:30.000000 protkit-0.2.3/venv/bin/rst2s5.py
+-rwxrwxr-x   0 fred      (1000) fred      (1000)      889 2024-04-03 10:09:30.000000 protkit-0.2.3/venv/bin/rst2xetex.py
+-rwxrwxr-x   0 fred      (1000) fred      (1000)      620 2024-04-03 10:09:30.000000 protkit-0.2.3/venv/bin/rst2xml.py
+-rwxrwxr-x   0 fred      (1000) fred      (1000)      688 2024-04-03 10:09:30.000000 protkit-0.2.3/venv/bin/rstpep2html.py
```

### Comparing `protkit-0.2.2/LICENSE` & `protkit-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/PKG-INFO` & `protkit-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protkit
-Version: 0.2.2
+Version: 0.2.3
 Summary: A unified toolkit for structural protein engineering.
 Author-email: Fred Senekal <fred@silicogenesis.com>
 Maintainer-email: Fred Senekal <fred@silicogenesis.com>
 Project-URL: Homepage, https://protkit.silicogenesis.com
 Project-URL: Repository, https://github.com/silicogenesis/protkit
 Project-URL: Documentation, https://silicogenesis.github.io/protkit
 Keywords: protein,protein engineering,structural biology,computational biology,biology,bioinformatics,sequence,amino acid,residue,dataset,PDB,antibody,antibody engineering,cdr
@@ -17,14 +17,15 @@
 Requires-Dist: requests>=2.31.0
 Requires-Dist: joblib>=1.3.2
 Requires-Dist: numpy>=1.20.3
 Requires-Dist: scikit-learn>=1.4.1.post1
 Requires-Dist: biopython>=1.83
 Requires-Dist: mmtf-python>=1.1.3
 Requires-Dist: freesasa>=2.2.1
+Requires-Dist: pdb2pqr>=3.6.2
 Provides-Extra: dev
 Requires-Dist: pytest>=6.2.5; extra == "dev"
 Requires-Dist: setuptools>=61.0; extra == "dev"
 
 <p align="center">
     <!--img src="media/logo/protkit800px.png" width="400"-->
     <img src="https://raw.githubusercontent.com/silicogenesis/protkit/main/media/logo/protkit800px.png" width="400px">
```

### Comparing `protkit-0.2.2/README.md` & `protkit-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/__init__.py` & `protkit-0.2.3/protkit/__init__.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/core/extend_attributes.py` & `protkit-0.2.3/protkit/core/extend_attributes.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/download/download.py` & `protkit-0.2.3/protkit/download/download.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/file_io/__init__.py` & `protkit-0.2.3/protkit/file_io/__init__.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/file_io/fasta_io.py` & `protkit-0.2.3/protkit/file_io/fasta_io.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/file_io/mmcif_io.py` & `protkit-0.2.3/protkit/file_io/mmcif_io.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/file_io/mmtf_io.py` & `protkit-0.2.3/protkit/file_io/mmtf_io.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/file_io/pdb_io.py` & `protkit-0.2.3/protkit/file_io/pdb_io.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 - `load()` to load a protein from a PDB file.
 - `save()` to save a protein to a PDB file.
 
 <font color="red">Saving a file in PQR format is not supported yet.</font>
 
 """
 
-from typing import List, Optional
+from typing import List, Dict, Optional
 from protkit.structure.protein import Protein
 from protkit.structure.chain import Chain
 from protkit.structure.residue import Residue
 from protkit.structure.atom import Atom
 
 
 class PDBIO():
@@ -329,22 +329,26 @@
                 "assigned_charge": None,
                 "calculated_charge": float(line[54:62]),
                 "radius": float(line[62:70])
             }
         return pdb_atom_dict
 
     @staticmethod
-    def create_pdb_atom_line(atom, serial: int, record_name="ATOM"):
+    def create_pdb_atom_line(atom: Dict, serial: int, record_name="ATOM") -> str:
         """
-        Creates a ATOM line for a PDB file.
+        Creates a ATOM or HETATM line for a PDB file.
 
-        The record_name is expected to be ATOM or HETATM
+        Args:
+            atom (Dict): The atom information.
+            serial (int): The serial number of the atom.
+            record_name (str): The record name, should be ATOM or HETATM.
+
+        Returns:
+            str: The ATOM or HETATM line.
         """
-        # text = "ATOM".ljust(6)
-        # text += atom["serial"].rjust(5) + " "
         text = record_name.ljust(6)
         text += str(serial).rjust(5) + " "
 
         # The PDB spec says that if the element has two characters, e.g. Fe (iron)
         # it should start at the position 13, otherwise it should start at position 14.
         # This seems a little problematic, as some atoms could use 4 characters
         # for example, HG11. The implementation here is consistent with observed PDBs
@@ -361,15 +365,67 @@
         text += f'{atom["x"]:8.3f}'
         text += f'{atom["y"]:8.3f}'
         text += f'{atom["z"]:8.3f}'
         text += f'{1.0 if atom["occupancy"] is None else atom["occupancy"]:6.2f}'
         text += f'{0.0 if atom["temp_factor"] is None else atom["temp_factor"]:6.2f}'
         text += "".ljust(10)
         text += atom["element"].rjust(2)
-        text += ("" if atom["charge"] is None else atom["charge"]).rjust(2)
+        text += ("" if atom["assigned_charge"] is None else atom["assigned_charge"]).rjust(2)
+        return text
+
+    @staticmethod
+    def create_pqr_atom_line(atom: Dict, serial: int, record_name="ATOM") -> str:
+        """
+        Creates a ATOM or HETATM line for a PQR file.
+
+        The PQR line is similar to the PDB ATOM line, but with additional fields
+        for atomic charge and radius. The occupancy, temperature factor,
+        charge and element fields from the PDB file are not used in the PQR file.
+
+        See: https://pdb2pqr.readthedocs.io/en/latest/formats/pqr.html
+        The order of fields in a PQR file is as follows:
+        Field_name Atom_number Atom_name Residue_name Chain_ID Residue_number
+        X Y Z Charge Radius
+
+        Args:
+            atom (Dict): The atom information.
+            serial (int): The serial number of the atom.
+            record_name (str): The record name, should be ATOM or HETATM.
+
+        Returns:
+            str: The PQR ATOM or HETATM line.
+        """
+        text = record_name.ljust(6)
+        text += str(serial).rjust(5) + " "
+
+        # The PDB spec says that if the element has two characters, e.g. Fe (iron)
+        # it should start at the position 13, otherwise it should start at position 14.
+        # This seems a little problematic, as some atoms could use 4 characters
+        # for example, HG11. The implementation here is consistent with observed PDBs
+        # from the RCSB.
+        if len(atom["element"]) == 2 or len(atom["atom_name"]) == 4:
+            text += atom["atom_name"].ljust(4)
+        else:
+            text += " " + atom["atom_name"].ljust(3)
+        text += ("" if atom["alt_loc"] is None else atom["alt_loc"]).ljust(1)
+        text += atom["res_name"].rjust(3) + " "
+        text += atom["chain_id"]
+        text += atom["res_seq"].rjust(4)
+        text += atom["icode"].ljust(1) + "   "
+        text += f'{atom["x"]:8.3f}'
+        text += f'{atom["y"]:8.3f}'
+        text += f'{atom["z"]:8.3f}'
+        text += f'{0.0 if atom["calculated_charge"] is None else atom["calculated_charge"]:8.4f}'
+        text += f'{0.0 if atom["radius"] is None else atom["radius"]:7.4f}'
+        # text += f'{1.0 if atom["occupancy"] is None else atom["occupancy"]:6.2f}'
+        # text += f'{0.0 if atom["temp_factor"] is None else atom["temp_factor"]:6.2f}'
+        # text += "".ljust(10)
+        # text += atom["element"].rjust(2)
+        # text += ("" if atom["charge"] is None else atom["charge"]).rjust(2)
+
         return text
 
     # --------------------------------------------------------------------------------
     # Main parsing and saving functions
     # --------------------------------------------------------------------------------
 
     @staticmethod
@@ -389,15 +445,15 @@
         lines = pdb_string.split("\n")
 
         # Parse every line into dictionary information
         entries = []
         for line in lines:
             record_name = line[0:6].strip().upper()
             if record_name == "ATOM":
-                pdb_atom_dict = PDBIO.parse_pdb_atom_line(line)
+                pdb_atom_dict = PDBIO.parse_pdb_atom_line(line, is_pqr_format=is_pqr_format)
                 entries.append(pdb_atom_dict)
             elif record_name == "HETATM":
                 pdb_atom_dict = PDBIO.parse_pdb_atom_line(line, is_pqr_format=is_pqr_format)
                 entries.append(pdb_atom_dict)
             elif record_name == "TER":
                 pdb_ter_dict = PDBIO.parse_pdb_ter_line(line)
                 entries.append(pdb_ter_dict)
@@ -526,17 +582,16 @@
                     # Serial is dependent on the atom ordering,
                     # so it is not used in the Atom class
                     # pdb_serial=entry["serial"],
                     alt_loc=entry["alt_loc"],
                     occupancy=entry["occupancy"],
                     temp_factor=entry["temp_factor"],
                     assigned_charge=entry["assigned_charge"],
-                    # pqr_calculated_charge=entry["calculated_charge"],
-                    # pqr_radius=entry["radius"],
-                    #
+                    calculated_charge=entry["calculated_charge"],
+                    radius=entry["radius"],
                     is_hetero=(record_name == "HETATM"),
 
                     residue=current_residue
                 )
 
                 # current_residue.add_atom(atom_id, atom)
                 current_residue.add_atom(atom.atom_type, atom)
@@ -579,14 +634,15 @@
                        is_pqr_format=False) -> str:
         text_entries = []
         num_seqres = 0
         num_atoms = 0
         num_hetatoms = 0
         num_ter = 0
         serial = 1
+        atom_entry = None
 
         for chain in protein.chains:
             for residue in chain.residues:
                 for atom in residue.atoms:
                     if not atom.is_hetero:
                         atom_entry = {
                             "element": atom.element,
@@ -598,20 +654,66 @@
                             "icode": residue.insertion_code,
                             "x": atom.x,
                             "y": atom.y,
                             "z": atom.z,
                             "occupancy": atom.get_attribute("occupancy"),
                             # "temp_factor": atom._pdb_temp_factor if atom._pdb_temp_factor is not None else 0.0,
                             "temp_factor": atom.get_attribute("temp_factor"),
-                            "charge": atom.get_attribute("assigned_charge")
+                            "assigned_charge": atom.get_attribute("assigned_charge"),
+                            "calculated_charge": atom.get_attribute("calculated_charge"),
+                            "radius": atom.get_attribute("radius")
                         }
-                        text_entries.append(PDBIO.create_pdb_atom_line(atom_entry, serial))
+                        if not is_pqr_format:
+                            text_entries.append(PDBIO.create_pdb_atom_line(atom_entry, serial))
+                        else:
+                            text_entries.append(PDBIO.create_pqr_atom_line(atom_entry, serial))
+
                         serial += 1
                         num_atoms += 1
 
+            # TER entry
+            if atom_entry is not None:
+                text_entries.append(PDBIO.create_pdb_ter_line(serial,
+                                                              atom_entry["res_name"],
+                                                              atom_entry["chain_id"],
+                                                              atom_entry["res_seq"],
+                                                              atom_entry["icode"]))
+                serial = serial + 1
+                num_ter += 1
+
+        for chain in protein.chains:
+            for residue in chain.residues:
+                # HETATM entries
+                for atom in residue.atoms:
+                    if atom.is_hetero:
+                        atom_entry = {
+                            "element": atom.element,
+                            "atom_name": atom.atom_type,
+                            "alt_loc": atom.get_attribute("pdb_alt_loc"),
+                            "res_name": residue.residue_type,
+                            "chain_id": chain.chain_id,
+                            "res_seq": str(residue.sequence_no),
+                            "icode": residue.insertion_code,
+                            "x": atom.x,
+                            "y": atom.y,
+                            "z": atom.z,
+                            "occupancy": atom.get_attribute("occupancy"),
+                            # "temp_factor": atom._pdb_temp_factor if atom._pdb_temp_factor is not None else 0.0,
+                            "temp_factor": atom.get_attribute("temp_factor"),
+                            "charge": atom.get_attribute("assigned_charge")
+                        }
+                        if not is_pqr_format:
+                            text_entries.append(PDBIO.create_pdb_atom_line(atom_entry, serial, record_name="HETATM"))
+                        else:
+                            text_entries.append(PDBIO.create_pqr_atom_line(atom_entry, serial, record_name="HETATM"))
+
+                        serial += 1
+                        num_hetatoms += 1
+            # Hetero residues have no TER records, so no need to write a termination code.
+
         # Bookkeeping records
         text_entries.append(PDBIO.create_pdb_master_line(num_atoms, num_hetatoms, num_ter, num_seqres=num_seqres))
         text_entries.append("END".ljust(80))
 
         return "\n".join(text_entries)
 
     @staticmethod
```

### Comparing `protkit-0.2.2/protkit/file_io/pqr_io.py` & `protkit-0.2.3/protkit/file_io/pqr_io.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/file_io/prot_io.py` & `protkit-0.2.3/protkit/file_io/prot_io.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/geometry/math.py` & `protkit-0.2.3/protkit/geometry/math.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/geometry/space_query.py` & `protkit-0.2.3/protkit/geometry/space_query.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/metrics/__init__.py` & `protkit-0.2.3/protkit/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/metrics/scoring_matrix.py` & `protkit-0.2.3/protkit/metrics/scoring_matrix.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/metrics/sequence_eval.py` & `protkit-0.2.3/protkit/metrics/sequence_eval.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/metrics/structure_eval.py` & `protkit-0.2.3/protkit/metrics/structure_eval.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/properties/__init__.py` & `protkit-0.2.3/protkit/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/properties/bond_angles.py` & `protkit-0.2.3/protkit/properties/bond_angles.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/properties/bond_lengths.py` & `protkit-0.2.3/protkit/properties/bond_lengths.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/properties/bounds.py` & `protkit-0.2.3/protkit/properties/bounds.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/properties/charge.py` & `protkit-0.2.3/protkit/properties/charge.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/properties/chemical_class.py` & `protkit-0.2.3/protkit/properties/chemical_class.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/properties/circular_variance.py` & `protkit-0.2.3/protkit/properties/circular_variance.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/properties/dihedral_angles.py` & `protkit-0.2.3/protkit/properties/dihedral_angles.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/properties/donors_acceptors.py` & `protkit-0.2.3/protkit/properties/donors_acceptors.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/properties/hydrophobicity.py` & `protkit-0.2.3/protkit/properties/hydrophobicity.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/properties/interface.py` & `protkit-0.2.3/protkit/properties/interface.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/properties/mass.py` & `protkit-0.2.3/protkit/properties/mass.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/properties/polarity.py` & `protkit-0.2.3/protkit/properties/polarity.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/properties/surface_area.py` & `protkit-0.2.3/protkit/properties/surface_area.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,14 @@
 Provides C implementations of the Lee-Richards and Shrake-Rupley algorithms
 with implementation hooks for Python.
 
 """
 
 from typing import TYPE_CHECKING
 from protkit.structure import Protein
-from protkit.tools.freesasa_adaptor import FreeSASAAdaptor
-
 
 class SurfaceArea:
     MAX_ASA_MILLER = {
         "ALA": 113.0,
         "ARG": 241.0,
         "ASN": 158.0,
         "ASP": 151.0,
@@ -100,14 +98,16 @@
             key (str): The attribute key to use when assigning the surface area to the protein object.
 
         Returns:
             float: The surface area of the protein.
         """
 
         # Calculate the solvent accessible surface area using Lee Richards
+        # Note the import of the adaptor is done here to avoid circular imports.
+        from protkit.tools.freesasa_adaptor import FreeSASAAdaptor
         freesasa_adaptor = FreeSASAAdaptor(algorithm=FreeSASAAdaptor.LEE_RICHARDS)
         sasa = freesasa_adaptor.calculate_surface_area(list(protein.atoms))
 
         if assign_attribute:
             index = 0
             protein_surface_area = 0
             for chain in protein.chains:
```

### Comparing `protkit-0.2.2/protkit/properties/vdw_radius.py` & `protkit-0.2.3/protkit/properties/vdw_radius.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/properties/volume.py` & `protkit-0.2.3/protkit/properties/volume.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/seq/__init__.py` & `protkit-0.2.3/protkit/seq/__init__.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/seq/antibody_sequence.py` & `protkit-0.2.3/protkit/seq/antibody_sequence.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/seq/nucleotide_sequence.py` & `protkit-0.2.3/protkit/seq/nucleotide_sequence.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/seq/protein_sequence.py` & `protkit-0.2.3/protkit/seq/protein_sequence.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/seq/sequence.py` & `protkit-0.2.3/protkit/seq/sequence.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/seq/sequence_alignment.py` & `protkit-0.2.3/protkit/seq/sequence_alignment.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/structure/__init__.py` & `protkit-0.2.3/protkit/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/structure/atom.py` & `protkit-0.2.3/protkit/structure/atom.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,14 +33,18 @@
 
                  # Optional
                  alt_loc: Optional[str] = None,
                  occupancy: Optional[float] = None,
                  temp_factor: Optional[float] = None,
                  assigned_charge: Optional[str] = None,
 
+                 # Optional PQR attributes
+                 calculated_charge: Optional[float] = None,
+                 radius: Optional[float] = None,
+
                  residue: Optional[Residue] = None):
         """
         Constructor for the Atom class.
 
         Args:
             element (str): The element associated with the atom.
             atom_type (str): The atom type.
@@ -49,40 +53,63 @@
             z (float): The z coordinate of the atom.
             is_hetero (bool, optional): The hetero flag. Defaults to False.
             is_disordered (bool, optional): The disordered flag. Defaults to False.
             alt_loc (Optional[str], optional): The alt_loc identifier. Defaults to None.
             occupancy (Optional[float], optional): The occupancy. Defaults to None.
             temp_factor (Optional[float], optional): The temperature factor. Defaults to None.
             assigned_charge (Optional[str], optional): The assigned charge. Defaults to None.
+            calculated_charge (Optional[float], optional): The calculated charge (PQR). Defaults to None.
+            radius (Optional[float], optional): The radius (PQR). Defaults to None.
             residue (Optional[Residue], optional): The residue the atom forms part of. Defaults to None.
 
         Returns:
             None
         """
 
         # Core properties
         self._x: float = x
         self._y: float = y
         self._z: float = z
         self._element: str = element
         self._atom_type: str = atom_type
 
+        # It could happen that the element is not set. For example, PQR files
+        # do not have an element field.
+        # In this case, the element is set to the first character of the atom type.
+        # This should generally work, although some programs use naming conventions for
+        # atom types that are not standard, for example starting a hydrogen with
+        # a numerical value rather than H. There may also be complications for
+        # two-letter element names. For example "CA" could be Calcium or Alpha Carbon.
+        # Further improvements should be made to handle these cases.
+        if self._element is None or self._element == "":
+            if self._atom_type is not None and self._atom_type != "":
+                self._element = self._atom_type[0]
+
         # Derived properties
         self._is_hetero: bool = is_hetero
         self._is_disordered: bool = is_disordered
 
         # Optional attributes
         if alt_loc is not None and alt_loc != "":
             self.set_attribute("alt_loc", alt_loc)
+            # If alt_loc is set, occupancy is also set
+            # There are examples where alt_loc is set, even though occupancy is 1.0.
+            # In these cases, the if statement below will not set the occupancy
+            # to 1.0, which is why it needs to be set here.
+            self.set_attribute("occupancy", occupancy)
         if occupancy is not None and occupancy != 1.0:
             self.set_attribute("occupancy", occupancy)
         if temp_factor is not None:
             self.set_attribute("temp_factor", temp_factor)
         if assigned_charge is not None and assigned_charge != "":
             self.set_attribute("assigned_charge", assigned_charge)
+        if calculated_charge is not None:
+            self.set_attribute("calculated_charge", calculated_charge)
+        if radius is not None:
+            self.set_attribute("radius", radius)
 
         # If alt_loc is specified, the atom is disordered
         # Keep track of all disordered states.
         if self.get_attribute("alt_loc") is not None:
             self._is_disordered = True
             self._disordered_states = [{
                 "alt_loc": self.get_attribute("alt_loc"),
```

### Comparing `protkit-0.2.2/protkit/structure/chain.py` & `protkit-0.2.3/protkit/structure/chain.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/structure/protein.py` & `protkit-0.2.3/protkit/structure/protein.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/structure/residue.py` & `protkit-0.2.3/protkit/structure/residue.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/tasks/protonator.py` & `protkit-0.2.3/protkit/tasks/protonator.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/tasks/surface_area_calculator.py` & `protkit-0.2.3/protkit/tasks/surface_area_calculator.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/tools/freesasa_adaptor.py` & `protkit-0.2.3/protkit/tools/freesasa_adaptor.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit/tools/reduce_adaptor.py` & `protkit-0.2.3/protkit/tools/reduce_adaptor.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.2/protkit.egg-info/PKG-INFO` & `protkit-0.2.3/protkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protkit
-Version: 0.2.2
+Version: 0.2.3
 Summary: A unified toolkit for structural protein engineering.
 Author-email: Fred Senekal <fred@silicogenesis.com>
 Maintainer-email: Fred Senekal <fred@silicogenesis.com>
 Project-URL: Homepage, https://protkit.silicogenesis.com
 Project-URL: Repository, https://github.com/silicogenesis/protkit
 Project-URL: Documentation, https://silicogenesis.github.io/protkit
 Keywords: protein,protein engineering,structural biology,computational biology,biology,bioinformatics,sequence,amino acid,residue,dataset,PDB,antibody,antibody engineering,cdr
@@ -17,14 +17,15 @@
 Requires-Dist: requests>=2.31.0
 Requires-Dist: joblib>=1.3.2
 Requires-Dist: numpy>=1.20.3
 Requires-Dist: scikit-learn>=1.4.1.post1
 Requires-Dist: biopython>=1.83
 Requires-Dist: mmtf-python>=1.1.3
 Requires-Dist: freesasa>=2.2.1
+Requires-Dist: pdb2pqr>=3.6.2
 Provides-Extra: dev
 Requires-Dist: pytest>=6.2.5; extra == "dev"
 Requires-Dist: setuptools>=61.0; extra == "dev"
 
 <p align="center">
     <!--img src="media/logo/protkit800px.png" width="400"-->
     <img src="https://raw.githubusercontent.com/silicogenesis/protkit/main/media/logo/protkit800px.png" width="400px">
```

### Comparing `protkit-0.2.2/pyproject.toml` & `protkit-0.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 package-dir = "protkit"
 
 [tool.setuptools.packages]
 find = {}
 
 [project]
 name = "protkit"
-version = "0.2.2"
+version = "0.2.3"
 requires-python = ">=3.6"
 authors = [
     { name="Fred Senekal", email="fred@silicogenesis.com"},
 ]
 maintainers = [
     { name="Fred Senekal", email="fred@silicogenesis.com"},
 ]
@@ -29,14 +29,15 @@
     "requests>=2.31.0",
     "joblib>=1.3.2",
     "numpy>=1.20.3",
     "scikit-learn>=1.4.1.post1",
     "biopython>=1.83",
     "mmtf-python>=1.1.3",
     "freesasa>=2.2.1",
+    "pdb2pqr>=3.6.2",
 ]
 keywords = ["protein", "protein engineering", "structural biology", "computational biology", "biology", "bioinformatics", "sequence", "amino acid", "residue", "dataset", "PDB", "antibody", "antibody engineering", "cdr"]
 
 [project.optional-dependencies]
 dev = [
     "pytest>=6.2.5",
     "setuptools>=61.0",
```

### Comparing `protkit-0.2.2/tests/quick_start_guide.py` & `protkit-0.2.3/tests/quick_start_guide.py`

 * *Files 3% similar despite different names*

```diff
@@ -407,18 +407,14 @@
     print(f"{protein.num_hydrogen_atoms} hydrogen atoms")
 
     protein.remove_hydrogen_atoms()
 
     print(f"{protein.num_hydrogen_atoms} hydrogen atoms after removal")
 
 
-# prep_data()
-quality_removing_hydrogen_atoms()
-
-
 def properties_hydrophobicity():
     from protkit.file_io import ProtIO
     from protkit.properties import Hydrophobicity
 
     protein = ProtIO.load("1ahw.prot")[0]
     Hydrophobicity.hydrophobicity_of_protein(protein, assign_attribute=True)
 
@@ -662,33 +658,60 @@
         if residue.get_attribute("in_interface"):
             print(residue.id)
 
     for residue in residues1:
         if residue.get_attribute("ca_in_interface"):
             print(residue.id)
 
+def tools_reduce():
+    from protkit.tools.reduce_adaptor import ReduceAdaptor
+    from protkit.file_io import ProtIO
+
+    reduce_bin_path = "/usr/local/bin/reduce"
+    reduce = ReduceAdaptor(reduce_bin_path)
+
+    protein = ProtIO.load("1ahw.prot")[0]
+    protein_protonated = reduce.protonate(protein)
+    protein_deprotonated = reduce.deprotonate(protein)
+
+def tools_freesasa():
+    from protkit.tools.freesasa_adaptor import FreeSASAAdaptor
+    from protkit.file_io import ProtIO
+
+    freesasa = FreeSASAAdaptor()
+    protein = ProtIO.load("1ahw.prot")[0]
+
+    atoms = list(protein.atoms)
+    atom_areas = freesasa.calculate_surface_area(atoms)
+    protein_area = sum(atom_areas)
+    print(protein_area)
+
+
 # prep_data()
 
-# quick_start_example()
+quick_start_example()
 
-# download_pdb_example()
-# download_fasta_example()
-# download_cif_example()
-
-# properties_hydrophobicity()
-# properties_hydrophobicity_class()
-# properties_mass()
-# properties_chemical_class()
-# properties_charge()
-# properties_polarity()
-# properties_donors_acceptors()
-# properties_surface_area()
-# properties_volume()
-# properties_volume_class()
-# properties_bounds_and_center()
-# properties_bond_lengths()
-# properties_peptide_lengths()
-# properties_bond_angles()
-# properties_dihedral_angles()
-# properties_circular_variance() -> double check first residue
+download_pdb_example()
+download_fasta_example()
+download_cif_example()
+
+properties_hydrophobicity()
+properties_hydrophobicity_class()
+properties_mass()
+properties_chemical_class()
+properties_charge()
+properties_polarity()
+properties_donors_acceptors()
+properties_surface_area()
+properties_volume()
+properties_volume_class()
+properties_bounds_and_center()
+properties_bond_lengths()
+properties_peptide_lengths()
+properties_bond_angles()
+properties_dihedral_angles()
+properties_circular_variance()  # -> double check first residue
 # properties_interface_atoms()
-# properties_interface_residues()
+# properties_interface_residues()
+
+tools_reduce()
+tools_freesasa()
```

### Comparing `protkit-0.2.2/tests/test_reduce.py` & `protkit-0.2.3/tests/test_reduce.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,9 @@
     protein = PDBIO.load(file_unprotonated)[0]
     reduce = ReduceAdaptor("/usr/local/bin/reduce", quiet=True)
 
     protein2 = reduce.protonate(protein, reduce_output_pdb_file_path=file_temp_protonated)
     print(protein2)
     PDBIO.save(protein2, file_protonated)
 
+
 test_reduce()
```

### Comparing `protkit-0.2.2/venv/bin/activate_this.py` & `protkit-0.2.3/venv/bin/activate_this.py`

 * *Files identical despite different names*

