# Comparing `tmp/cutadapt-4.7.tar.gz` & `tmp/cutadapt-4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cutadapt-4.7.tar", last modified: Thu Mar 14 14:16:52 2024, max compression
+gzip compressed data, was "cutadapt-4.8.tar", last modified: Fri Apr 12 13:30:14 2024, max compression
```

## Comparing `cutadapt-4.7.tar` & `cutadapt-4.8.tar`

### file list

```diff
@@ -1,332 +1,332 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:16:52.919765 cutadapt-4.7/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-14 14:16:47.000000 cutadapt-4.7/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-14 14:16:47.000000 cutadapt-4.7/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:16:52.871765 cutadapt-4.7/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-14 14:16:47.000000 cutadapt-4.7/.github/issue_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:16:52.871765 cutadapt-4.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-03-14 14:16:47.000000 cutadapt-4.7/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-14 14:16:47.000000 cutadapt-4.7/.github/workflows/pyinstaller.yml
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-14 14:16:47.000000 cutadapt-4.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-14 14:16:47.000000 cutadapt-4.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-14 14:16:47.000000 cutadapt-4.7/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    46051 2024-03-14 14:16:47.000000 cutadapt-4.7/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-14 14:16:47.000000 cutadapt-4.7/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-03-14 14:16:47.000000 cutadapt-4.7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-03-14 14:16:47.000000 cutadapt-4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-14 14:16:47.000000 cutadapt-4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-03-14 14:16:52.915765 cutadapt-4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-03-14 14:16:47.000000 cutadapt-4.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:16:52.871765 cutadapt-4.7/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-03-14 14:16:47.000000 cutadapt-4.7/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:16:52.871765 cutadapt-4.7/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    18174 2024-03-14 14:16:47.000000 cutadapt-4.7/doc/_static/adapters.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-03-14 14:16:47.000000 cutadapt-4.7/doc/_static/cutadapt-logo.inkscape.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-03-14 14:16:47.000000 cutadapt-4.7/doc/_static/cutadapt-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-14 14:16:47.000000 cutadapt-4.7/doc/_static/cutadapt-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-03-14 14:16:47.000000 cutadapt-4.7/doc/algorithms.rst
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-14 14:16:47.000000 cutadapt-4.7/doc/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-14 14:16:47.000000 cutadapt-4.7/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-03-14 14:16:47.000000 cutadapt-4.7/doc/develop.rst
--rw-r--r--   0 runner    (1001) docker     (127)   100211 2024-03-14 14:16:47.000000 cutadapt-4.7/doc/guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-03-14 14:16:47.000000 cutadapt-4.7/doc/ideas.rst
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-14 14:16:47.000000 cutadapt-4.7/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-03-14 14:16:47.000000 cutadapt-4.7/doc/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14008 2024-03-14 14:16:47.000000 cutadapt-4.7/doc/recipes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    31840 2024-03-14 14:16:47.000000 cutadapt-4.7/doc/reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-14 14:16:47.000000 cutadapt-4.7/doc/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-03-14 14:16:47.000000 cutadapt-4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 14:16:52.919765 cutadapt-4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-14 14:16:47.000000 cutadapt-4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:16:52.867765 cutadapt-4.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:16:52.879765 cutadapt-4.7/src/cutadapt/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/_align.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    32717 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/_align.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/_kmer_finder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/_kmer_finder.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/_match_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-14 14:16:52.000000 cutadapt-4.7/src/cutadapt/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    49631 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/adapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/align.py
--rw-r--r--   0 runner    (1001) docker     (127)    53894 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/expected_errors.h
--rw-r--r--   0 runner    (1001) docker     (127)    10735 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/info.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9241 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/kmer_heuristic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    32585 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/modifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/predicates.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/qualtrim.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/qualtrim.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    32660 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/report.py
--rw-r--r--   0 runner    (1001) docker     (127)    15759 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/runners.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    18679 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-03-14 14:16:47.000000 cutadapt-4.7/src/cutadapt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:16:52.915765 cutadapt-4.7/src/cutadapt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-03-14 14:16:52.000000 cutadapt-4.7/src/cutadapt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8810 2024-03-14 14:16:52.000000 cutadapt-4.7/src/cutadapt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:16:52.000000 cutadapt-4.7/src/cutadapt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-14 14:16:52.000000 cutadapt-4.7/src/cutadapt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-14 14:16:52.000000 cutadapt-4.7/src/cutadapt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-14 14:16:52.000000 cutadapt-4.7/src/cutadapt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:16:52.883765 cutadapt-4.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:16:52.903765 cutadapt-4.7/tests/cut/
--rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/454.fa
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/SRR2040271_1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/action_lowercase.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/action_retain.fasta
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/adapterorder-ag.fasta
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/adapterorder-ga.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/adapterx.fasta
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/anchored-back.fasta
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/anchored.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/anchored_no_indels.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/anchored_no_indels_wildcard.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/anywhere_repeat.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/casava.fastq
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:16:52.903765 cutadapt-4.7/tests/cut/combinatorial/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/combinatorial/combinatorial.A_G.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/combinatorial/combinatorial.A_G.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/combinatorial/combinatorial.A_T.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/combinatorial/combinatorial.A_T.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/combinatorial/combinatorial.A_unknown.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/combinatorial/combinatorial.A_unknown.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/combinatorial/combinatorial.C_G.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/combinatorial/combinatorial.C_G.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/combinatorial/combinatorial.C_T.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/combinatorial/combinatorial.C_T.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/combinatorial/combinatorial.C_unknown.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/combinatorial/combinatorial.C_unknown.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/combinatorial/combinatorial.unknown_G.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/combinatorial/combinatorial.unknown_G.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/combinatorial/combinatorial.unknown_T.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/combinatorial/combinatorial.unknown_T.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/combinatorial/combinatorial.unknown_unknown.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/combinatorial/combinatorial.unknown_unknown.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/demultiplexed.first.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/demultiplexed.first.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/demultiplexed.second.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/demultiplexed.second.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/demultiplexed.unknown.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/demultiplexed.unknown.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/discard-untrimmed.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/discard.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/dos.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/dual-i1.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/dual-i1.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/dual-i2.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/dual-i2.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/dual-unknown.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/dual-unknown.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/empty.fasta
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/empty.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/example.fa
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/examplefront.fa
--rw-r--r--   0 runner    (1001) docker     (127)    17780 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/illumina.fastq
--rw-r--r--   0 runner    (1001) docker     (127)    25093 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/illumina.info.txt
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/illumina5.fastq
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/illumina5.info.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/illumina64.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/info-rc.txt
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/interleaved.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/issue46.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/linked-anchored.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/linked-discard-g.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/linked-discard.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/linked-info.txt
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/linked-lowercase.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/linked-not-anchored.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/linked.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/lowercase.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/lowqual.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/lowqual.unchanged.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/maxee.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/maxlen.fa
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/maxn0.2.fasta
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/maxn0.4.fasta
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/maxn0.fasta
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/maxn1.fasta
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/maxn2.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/minlen.fa
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/minlen.noprimer.fa
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/multiprefix.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/multisuffix.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/nextseq.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/no-trim.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/no_indels.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/overlapb.fa
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/pair-adapters.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/pair-adapters.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/paired-filterboth.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/paired-filterboth.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/paired-filterfirst.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/paired-filterfirst.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/paired-m27.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/paired-m27.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/paired-onlyA.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/paired-onlyA.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/paired-separate.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/paired-separate.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/paired-too-short.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/paired-too-short.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/paired-trimmed.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/paired-trimmed.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/paired-untrimmed.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/paired-untrimmed.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/paired.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/paired.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/paired.m14.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/paired.m14.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/pairedq.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/pairedq.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/pairedu.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/pairedu.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/plus.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/polya.1.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/polya.2.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/polya.legacy.1.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/rename.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/rename.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/rename.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/rest.fa
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/restfront.fa
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/revcomp-r1r2.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/revcomp-r1r2.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/revcomp-single-normalize.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/revcomp-single.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/revcomp.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/revcomp.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/s_1_sequence.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/shortened-negative.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/shortened.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/simple.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/small-no-trim.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/small.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/small.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/small.trimmed.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/small.untrimmed.fastq
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/solid-no-zerocap.fastq
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/solidqual.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/sra.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/stripped.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/suffix.fastq
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/trim-n.fasta
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/trimN3.fasta
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/trimN5.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/twoadapters.fasta
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/twoadapters.first.fasta
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/twoadapters.second.fasta
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/twoadapters.unknown.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/unconditional-back.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/unconditional-both.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/unconditional-front.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/wildcard.fa
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/wildcardN.fa
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/wildcard_adapter.fa
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/wildcard_adapter_anywhere.fa
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/cut/xadapter.fasta
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:16:52.915765 cutadapt-4.7/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/454.fa
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/E3M.fasta
--rw-r--r--   0 runner    (1001) docker     (127)     8630 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/E3M.qual
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/action_lowercase.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/action_retain.fasta
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/adapter-empty-name.fasta
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/adapter.fasta
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/adapterorder.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/anchored-back.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/anchored.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/anchored_no_indels.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/anywhere_repeat.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/casava.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/combinatorial.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/combinatorial.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/dos.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/dual-index.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/dual-index.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/empty.fasta
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/empty.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/example.fa
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/format-error.fastq
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/illumina.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/illumina5.fastq
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/illumina64.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/info-rc.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/interleaved.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/issue46.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/lengths.fa
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/linked.fasta
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/lowqual.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/maxee.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/maxn.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/multi.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/multiblock.fastq.bz2
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/multiblock.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/nextseq.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/no_indels.fasta
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/onlycomment.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/overlapb.fa
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/paired.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/paired.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/polya.1.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/polya.2.fasta
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/prefix-adapter.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/rest.fa
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/rest.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/restfront.txt
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/revcomp.1.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/revcomp.2.fastq
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/s_1_sequence.txt.gz
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/simple.fasta
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/simple.fasta.gz
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/simple.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/small.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/small.fastq.bz2
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/small.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/small.fastq.xz
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/suffix-adapter.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/suffix.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/toolong.fa
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/tooshort.fa
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/tooshort.noprimer.fa
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/trim-n.fasta
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/trimN3.fasta
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/trimN5.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/twoadapters.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/underscore_fastq.gz
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/wildcard.fa
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/wildcardN.fa
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/wildcard_adapter.fa
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/withplus.fastq
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/data/xadapterx.fasta
--rw-r--r--   0 runner    (1001) docker     (127)    18451 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/test_adapters.py
--rw-r--r--   0 runner    (1001) docker     (127)    14621 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (127)    30150 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/test_commandline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/test_kmer_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/test_kmer_heuristic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    16511 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/test_modifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)    24496 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/test_paired.py
--rw-r--r--   0 runner    (1001) docker     (127)    15661 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/test_predicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/test_qualtrim.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/test_testutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/test_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/test_trim.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-03-14 14:16:47.000000 cutadapt-4.7/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-03-14 14:16:47.000000 cutadapt-4.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:30:14.367740 cutadapt-4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-12 13:30:08.000000 cutadapt-4.8/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-12 13:30:08.000000 cutadapt-4.8/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:30:14.315739 cutadapt-4.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-12 13:30:08.000000 cutadapt-4.8/.github/issue_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:30:14.315739 cutadapt-4.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-12 13:30:08.000000 cutadapt-4.8/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-12 13:30:08.000000 cutadapt-4.8/.github/workflows/pyinstaller.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-12 13:30:08.000000 cutadapt-4.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-12 13:30:08.000000 cutadapt-4.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-12 13:30:08.000000 cutadapt-4.8/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    46288 2024-04-12 13:30:08.000000 cutadapt-4.8/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-12 13:30:08.000000 cutadapt-4.8/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-12 13:30:08.000000 cutadapt-4.8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-12 13:30:08.000000 cutadapt-4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-12 13:30:08.000000 cutadapt-4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-12 13:30:14.367740 cutadapt-4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-12 13:30:08.000000 cutadapt-4.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:30:14.319739 cutadapt-4.8/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-04-12 13:30:08.000000 cutadapt-4.8/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:30:14.319739 cutadapt-4.8/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    18174 2024-04-12 13:30:08.000000 cutadapt-4.8/doc/_static/adapters.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-12 13:30:08.000000 cutadapt-4.8/doc/_static/cutadapt-logo.inkscape.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-04-12 13:30:08.000000 cutadapt-4.8/doc/_static/cutadapt-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-12 13:30:08.000000 cutadapt-4.8/doc/_static/cutadapt-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-04-12 13:30:08.000000 cutadapt-4.8/doc/algorithms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-12 13:30:08.000000 cutadapt-4.8/doc/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-12 13:30:08.000000 cutadapt-4.8/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-12 13:30:08.000000 cutadapt-4.8/doc/develop.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   100211 2024-04-12 13:30:08.000000 cutadapt-4.8/doc/guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-12 13:30:08.000000 cutadapt-4.8/doc/ideas.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-12 13:30:08.000000 cutadapt-4.8/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7811 2024-04-12 13:30:08.000000 cutadapt-4.8/doc/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14008 2024-04-12 13:30:08.000000 cutadapt-4.8/doc/recipes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    31840 2024-04-12 13:30:08.000000 cutadapt-4.8/doc/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-12 13:30:08.000000 cutadapt-4.8/doc/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-12 13:30:08.000000 cutadapt-4.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 13:30:14.367740 cutadapt-4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-12 13:30:08.000000 cutadapt-4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:30:14.311739 cutadapt-4.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:30:14.323739 cutadapt-4.8/src/cutadapt/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/_align.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    32717 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/_align.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/_kmer_finder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/_kmer_finder.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/_match_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-12 13:30:14.000000 cutadapt-4.8/src/cutadapt/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49631 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/align.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53894 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/expected_errors.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10791 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/info.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/info.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9241 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/kmer_heuristic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32585 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/modifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/qualtrim.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/qualtrim.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    32660 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16006 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18679 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-04-12 13:30:08.000000 cutadapt-4.8/src/cutadapt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:30:14.363740 cutadapt-4.8/src/cutadapt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-12 13:30:14.000000 cutadapt-4.8/src/cutadapt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8810 2024-04-12 13:30:14.000000 cutadapt-4.8/src/cutadapt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:30:14.000000 cutadapt-4.8/src/cutadapt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-12 13:30:14.000000 cutadapt-4.8/src/cutadapt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-12 13:30:14.000000 cutadapt-4.8/src/cutadapt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 13:30:14.000000 cutadapt-4.8/src/cutadapt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:30:14.327739 cutadapt-4.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:30:14.351740 cutadapt-4.8/tests/cut/
+-rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/454.fa
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/SRR2040271_1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/action_lowercase.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/action_retain.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/adapterorder-ag.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/adapterorder-ga.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/adapterx.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/anchored-back.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/anchored.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/anchored_no_indels.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/anchored_no_indels_wildcard.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/anywhere_repeat.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/casava.fastq
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:30:14.351740 cutadapt-4.8/tests/cut/combinatorial/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/combinatorial/combinatorial.A_G.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/combinatorial/combinatorial.A_G.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/combinatorial/combinatorial.A_T.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/combinatorial/combinatorial.A_T.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/combinatorial/combinatorial.A_unknown.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/combinatorial/combinatorial.A_unknown.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/combinatorial/combinatorial.C_G.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/combinatorial/combinatorial.C_G.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/combinatorial/combinatorial.C_T.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/combinatorial/combinatorial.C_T.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/combinatorial/combinatorial.C_unknown.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/combinatorial/combinatorial.C_unknown.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/combinatorial/combinatorial.unknown_G.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/combinatorial/combinatorial.unknown_G.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/combinatorial/combinatorial.unknown_T.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/combinatorial/combinatorial.unknown_T.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/combinatorial/combinatorial.unknown_unknown.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/combinatorial/combinatorial.unknown_unknown.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/demultiplexed.first.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/demultiplexed.first.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/demultiplexed.second.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/demultiplexed.second.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/demultiplexed.unknown.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/demultiplexed.unknown.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/discard-untrimmed.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/discard.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/dos.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/dual-i1.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/dual-i1.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/dual-i2.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/dual-i2.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/dual-unknown.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/dual-unknown.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/empty.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/empty.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/example.fa
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/examplefront.fa
+-rw-r--r--   0 runner    (1001) docker     (127)    17780 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/illumina.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)    25093 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/illumina.info.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/illumina5.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/illumina5.info.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/illumina64.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/info-rc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/interleaved.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/issue46.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/linked-anchored.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/linked-discard-g.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/linked-discard.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/linked-info.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/linked-lowercase.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/linked-not-anchored.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/linked.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/lowercase.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/lowqual.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/lowqual.unchanged.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/maxee.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/maxlen.fa
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/maxn0.2.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/maxn0.4.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/maxn0.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/maxn1.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/maxn2.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/minlen.fa
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/minlen.noprimer.fa
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/multiprefix.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/multisuffix.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/nextseq.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/no-trim.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/no_indels.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/overlapb.fa
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/pair-adapters.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/pair-adapters.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/paired-filterboth.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/paired-filterboth.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/paired-filterfirst.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/paired-filterfirst.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/paired-m27.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/paired-m27.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/paired-onlyA.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/paired-onlyA.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/paired-separate.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/paired-separate.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/paired-too-short.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/paired-too-short.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/paired-trimmed.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/paired-trimmed.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/paired-untrimmed.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/paired-untrimmed.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/paired.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/paired.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/paired.m14.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/paired.m14.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/pairedq.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/pairedq.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/pairedu.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/pairedu.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/plus.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/polya.1.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/polya.2.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/polya.legacy.1.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/rename.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/rename.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/rename.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/rest.fa
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/restfront.fa
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/revcomp-r1r2.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/revcomp-r1r2.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/revcomp-single-normalize.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/revcomp-single.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/revcomp.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/revcomp.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/s_1_sequence.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/shortened-negative.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/shortened.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/simple.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/small-no-trim.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/small.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/small.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/small.trimmed.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/small.untrimmed.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/solid-no-zerocap.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/solidqual.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/sra.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/stripped.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/suffix.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/trim-n.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/trimN3.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/trimN5.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/twoadapters.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/twoadapters.first.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/twoadapters.second.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/twoadapters.unknown.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/unconditional-back.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/unconditional-both.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/unconditional-front.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/wildcard.fa
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/wildcardN.fa
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/wildcard_adapter.fa
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/wildcard_adapter_anywhere.fa
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/cut/xadapter.fasta
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:30:14.363740 cutadapt-4.8/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/454.fa
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/E3M.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)     8630 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/E3M.qual
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/action_lowercase.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/action_retain.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/adapter-empty-name.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/adapter.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/adapterorder.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/anchored-back.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/anchored.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/anchored_no_indels.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/anywhere_repeat.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/casava.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/combinatorial.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/combinatorial.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/dos.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/dual-index.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/dual-index.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/empty.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/empty.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/example.fa
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/format-error.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/illumina.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/illumina5.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/illumina64.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/info-rc.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/interleaved.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/issue46.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/lengths.fa
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/linked.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/lowqual.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/maxee.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/maxn.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/multi.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/multiblock.fastq.bz2
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/multiblock.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/nextseq.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/no_indels.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/onlycomment.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/overlapb.fa
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/paired.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/paired.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/polya.1.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/polya.2.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/prefix-adapter.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/rest.fa
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/rest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/restfront.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/revcomp.1.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/revcomp.2.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/s_1_sequence.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/simple.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/simple.fasta.gz
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/simple.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/small.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/small.fastq.bz2
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/small.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/small.fastq.xz
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/suffix-adapter.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/suffix.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/toolong.fa
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/tooshort.fa
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/tooshort.noprimer.fa
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/trim-n.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/trimN3.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/trimN5.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/twoadapters.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/underscore_fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/wildcard.fa
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/wildcardN.fa
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/wildcard_adapter.fa
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/withplus.fastq
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/data/xadapterx.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)    18451 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/test_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14621 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30999 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/test_commandline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/test_kmer_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/test_kmer_heuristic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16511 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/test_modifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24496 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/test_paired.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15661 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/test_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/test_qualtrim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/test_testutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/test_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/test_trim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-12 13:30:08.000000 cutadapt-4.8/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-12 13:30:08.000000 cutadapt-4.8/tox.ini
```

### Comparing `cutadapt-4.7/.github/workflows/ci.yml` & `cutadapt-4.8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/.github/workflows/pyinstaller.yml` & `cutadapt-4.8/.github/workflows/pyinstaller.yml`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/CHANGES.rst` & `cutadapt-4.8/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =========
 Changelog
 =========
 
+v4.8 (2024-04-12)
+-------------------
+
+* :issue:`772`: Restore ability to provide input files via
+  process substitution.
+* :issue:`773`: Fix crash when writing interleaved data to stdout
+  (that is, when no ``-o`` option is provided).
+
 v4.7 (2024-03-14)
 -----------------
 
 * :issue:`767`: Error messages are always sent to stderr. They were
   previously sent to stdout when using `-o`.
 * Cutadapt can now read single-end data from unaligned BAM files (uBAM).
 * Dropped support for Python 3.7.
```

### Comparing `cutadapt-4.7/CITATION.cff` & `cutadapt-4.8/CITATION.cff`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/CONTRIBUTING.rst` & `cutadapt-4.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/LICENSE` & `cutadapt-4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/PKG-INFO` & `cutadapt-4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cutadapt
-Version: 4.7
+Version: 4.8
 Summary: Adapter trimming and other preprocessing of high-throughput sequencing reads
 Author-email: Marcel Martin <marcel.martin@scilifelab.se>
 License: MIT
 Project-URL: Homepage, https://cutadapt.readthedocs.io/
 Project-URL: Changelog, https://cutadapt.readthedocs.io/en/stable/changes.html
 Project-URL: Repository, https://github.com/marcelm/cutadapt/
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cutadapt-4.7/README.rst` & `cutadapt-4.8/README.rst`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/doc/Makefile` & `cutadapt-4.8/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/doc/_static/adapters.svg` & `cutadapt-4.8/doc/_static/adapters.svg`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/doc/_static/cutadapt-logo.inkscape.svg` & `cutadapt-4.8/doc/_static/cutadapt-logo.inkscape.svg`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/doc/_static/cutadapt-logo.png` & `cutadapt-4.8/doc/_static/cutadapt-logo.png`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/doc/_static/cutadapt-logo.svg` & `cutadapt-4.8/doc/_static/cutadapt-logo.svg`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/doc/algorithms.rst` & `cutadapt-4.8/doc/algorithms.rst`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/doc/conf.py` & `cutadapt-4.8/doc/conf.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/doc/develop.rst` & `cutadapt-4.8/doc/develop.rst`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/doc/guide.rst` & `cutadapt-4.8/doc/guide.rst`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/doc/ideas.rst` & `cutadapt-4.8/doc/ideas.rst`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/doc/installation.rst` & `cutadapt-4.8/doc/installation.rst`

 * *Files 6% similar despite different names*

```diff
@@ -137,14 +137,34 @@
 4. Test whether it worked by running ``py -m cutadapt --version``. You should
    see the version number of Cutadapt.
 
 When running Cutadapt this way, you will need to remember to write
 ``py -m cutadapt`` instead of just ``cutadapt``.
 
 
+FreeBSD ports and pkgsrc
+------------------------
+
+Cutadapt can be installed via the FreeBSD ports system.
+To install from a binary package, run::
+
+    pkg install py39-cutadapt
+
+The ``p39`` will change from time to time (``py310``, ``py311`` etc.).
+Alternatively, peruse the `FreeBSD ports documentation <https://www.freebsd.org/ports/index.html>`_
+to install from source, which may result in better optimized binaries.
+
+To install a binary package via the pkgsrc system (for example on NetBSD), run ::
+
+    pkgin install py311-cutadapt
+
+The pkgsrc system also allows installation from source on any POSIX platform
+(including macOS), see the `https://pkgsrc.org/ <pkgsrc home page>`_.
+
+
 Shared installation (on a cluster)
 ----------------------------------
 
 If you have a larger installation and want to provide Cutadapt as a module
 that can be loaded and unloaded (with the Lmod system, for example), we
 recommend that you create a virtual environment and 'pip install' Cutadapt into
 it. These instructions work on a SLURM cluster that uses the Lmod system
```

### Comparing `cutadapt-4.7/doc/recipes.rst` & `cutadapt-4.8/doc/recipes.rst`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/doc/reference.rst` & `cutadapt-4.8/doc/reference.rst`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/pyproject.toml` & `cutadapt-4.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/src/cutadapt/_align.pyi` & `cutadapt-4.8/src/cutadapt/_align.pyi`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/src/cutadapt/_align.pyx` & `cutadapt-4.8/src/cutadapt/_align.pyx`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/src/cutadapt/_kmer_finder.pyx` & `cutadapt-4.8/src/cutadapt/_kmer_finder.pyx`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/src/cutadapt/_match_tables.py` & `cutadapt-4.8/src/cutadapt/_match_tables.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/src/cutadapt/adapters.py` & `cutadapt-4.8/src/cutadapt/adapters.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/src/cutadapt/align.py` & `cutadapt-4.8/src/cutadapt/align.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/src/cutadapt/cli.py` & `cutadapt-4.8/src/cutadapt/cli.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/src/cutadapt/expected_errors.h` & `cutadapt-4.8/src/cutadapt/expected_errors.h`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/src/cutadapt/files.py` & `cutadapt-4.8/src/cutadapt/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,14 +252,16 @@
         )
         if len(paths) not in (1, 2):
             raise ValueError("Expected one or two paths")
         if interleaved and len(paths) != 1:
             raise ValueError("Cannot write to two files when interleaved is True")
         if len(paths) == 1 and paths[0] == "-" and force_fasta:
             kwargs["fileformat"] = "fasta"
+        if paths == (None,):
+            paths = ("-",)
         for path in paths:
             assert path is not None
         binary_files = []
         for path in paths:
             binary_file = self._file_opener.xopen(path, "wb")
             binary_files.append(binary_file)
             self._binary_files.append(binary_file)
```

### Comparing `cutadapt-4.7/src/cutadapt/info.pyx` & `cutadapt-4.8/src/cutadapt/info.pyx`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/src/cutadapt/json.py` & `cutadapt-4.8/src/cutadapt/json.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/src/cutadapt/kmer_heuristic.py` & `cutadapt-4.8/src/cutadapt/kmer_heuristic.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/src/cutadapt/log.py` & `cutadapt-4.8/src/cutadapt/log.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/src/cutadapt/modifiers.py` & `cutadapt-4.8/src/cutadapt/modifiers.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/src/cutadapt/parser.py` & `cutadapt-4.8/src/cutadapt/parser.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/src/cutadapt/pipeline.py` & `cutadapt-4.8/src/cutadapt/pipeline.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/src/cutadapt/predicates.py` & `cutadapt-4.8/src/cutadapt/predicates.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/src/cutadapt/qualtrim.pyx` & `cutadapt-4.8/src/cutadapt/qualtrim.pyx`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/src/cutadapt/report.py` & `cutadapt-4.8/src/cutadapt/report.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/src/cutadapt/runners.py` & `cutadapt-4.8/src/cutadapt/runners.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 )
 from cutadapt.pipeline import Pipeline
 from cutadapt.report import Statistics
 from cutadapt.utils import Progress
 
 logger = logging.getLogger()
 
-mpctx = multiprocessing.get_context("spawn")
+mpctx = multiprocessing.get_context()
 
 # See https://github.com/python/typeshed/issues/9860
 if TYPE_CHECKING:
     mpctx_Process = multiprocessing.Process
 else:
     mpctx_Process = mpctx.Process
 
@@ -86,19 +86,24 @@
 
     def run(self):
         if self.stdin_fd != -1:
             sys.stdin.close()
             sys.stdin = os.fdopen(self.stdin_fd)
         try:
             with ExitStack() as stack:
-                files = [
-                    stack.enter_context(xopen_rb_raise_limit(path))
-                    for path in self._paths
-                ]
-                file_format = detect_file_format(files[0])
+                try:
+                    files = [
+                        stack.enter_context(xopen_rb_raise_limit(path))
+                        for path in self._paths
+                    ]
+                    file_format = detect_file_format(files[0])
+                except Exception as e:
+                    self._file_format_connection.send(-2)
+                    self._file_format_connection.send((e, traceback.format_exc()))
+                    raise
                 self._file_format_connection.send(file_format)
                 if file_format is not None:
                     for index, chunks in enumerate(self._read_chunks(*files)):
                         self.send_to_worker(index, *chunks)
             self.shutdown()
         except Exception as e:
             # TODO better send this to a common "something went wrong" Queue
@@ -309,15 +314,15 @@
             connections=connw,
             queue=self._need_work_queue,
             buffer_size=self._buffer_size,
             stdin_fd=fileno,
         )
         self._reader_process.daemon = True
         self._reader_process.start()
-        file_format: Optional[FileFormat] = file_format_connection_r.recv()
+        file_format: Optional[FileFormat] = self._try_receive(file_format_connection_r)
         if file_format is None:
             raise dnaio.exceptions.UnknownFileFormat(
                 f"Format of input file '{self._inpaths.paths[0]}' not recognized."
             )
         self._input_file_format = file_format
 
     def _start_workers(
@@ -371,15 +376,15 @@
         self._reader_process.join()
         progress.close()
         return stats
 
     @staticmethod
     def _try_receive(connection):
         """
-        Try to receive data over `self.connection` and return it.
+        Try to receive data over `connection` and return it.
         If an exception was received, raise it.
         """
         result = connection.recv()
         if result == -2:
             # An exception has occurred on the other end
             e, tb_str = connection.recv()
             # The other end does not send an actual traceback object because these are
```

### Comparing `cutadapt-4.7/src/cutadapt/statistics.py` & `cutadapt-4.8/src/cutadapt/statistics.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/src/cutadapt/steps.py` & `cutadapt-4.8/src/cutadapt/steps.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/src/cutadapt/tokenizer.py` & `cutadapt-4.8/src/cutadapt/tokenizer.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/src/cutadapt/utils.py` & `cutadapt-4.8/src/cutadapt/utils.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/src/cutadapt.egg-info/PKG-INFO` & `cutadapt-4.8/src/cutadapt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cutadapt
-Version: 4.7
+Version: 4.8
 Summary: Adapter trimming and other preprocessing of high-throughput sequencing reads
 Author-email: Marcel Martin <marcel.martin@scilifelab.se>
 License: MIT
 Project-URL: Homepage, https://cutadapt.readthedocs.io/
 Project-URL: Changelog, https://cutadapt.readthedocs.io/en/stable/changes.html
 Project-URL: Repository, https://github.com/marcelm/cutadapt/
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cutadapt-4.7/src/cutadapt.egg-info/SOURCES.txt` & `cutadapt-4.8/src/cutadapt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/conftest.py` & `cutadapt-4.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/cut/454.fa` & `cutadapt-4.8/tests/cut/454.fa`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/cut/anywhere_repeat.fastq` & `cutadapt-4.8/tests/cut/anywhere_repeat.fastq`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/cut/illumina.fastq` & `cutadapt-4.8/tests/cut/illumina.fastq`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/cut/illumina.info.txt` & `cutadapt-4.8/tests/cut/illumina.info.txt`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/cut/illumina5.fastq` & `cutadapt-4.8/tests/cut/illumina5.fastq`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/cut/illumina5.info.txt` & `cutadapt-4.8/tests/cut/illumina5.info.txt`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/cut/illumina64.fastq` & `cutadapt-4.8/tests/cut/illumina64.fastq`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/cut/linked-info.txt` & `cutadapt-4.8/tests/cut/linked-info.txt`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/cut/overlapb.fa` & `cutadapt-4.8/tests/cut/overlapb.fa`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/cut/solid-no-zerocap.fastq` & `cutadapt-4.8/tests/cut/solid-no-zerocap.fastq`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/cut/solidqual.fastq` & `cutadapt-4.8/tests/cut/solidqual.fastq`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/data/454.fa` & `cutadapt-4.8/tests/data/454.fa`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/data/E3M.fasta` & `cutadapt-4.8/tests/data/E3M.fasta`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/data/E3M.qual` & `cutadapt-4.8/tests/data/E3M.qual`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/data/anywhere_repeat.fastq` & `cutadapt-4.8/tests/data/anywhere_repeat.fastq`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/data/illumina.fastq.gz` & `cutadapt-4.8/tests/data/illumina.fastq.gz`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/data/illumina5.fastq` & `cutadapt-4.8/tests/data/illumina5.fastq`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/data/illumina64.fastq` & `cutadapt-4.8/tests/data/illumina64.fastq`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/data/interleaved.fastq` & `cutadapt-4.8/tests/data/interleaved.fastq`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/data/nextseq.fastq` & `cutadapt-4.8/tests/data/nextseq.fastq`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/data/overlapb.fa` & `cutadapt-4.8/tests/data/overlapb.fa`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/test_adapters.py` & `cutadapt-4.8/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/test_align.py` & `cutadapt-4.8/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/test_api.py` & `cutadapt-4.8/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/test_command.py` & `cutadapt-4.8/tests/test_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,38 @@
             ],
             stdout=out_file,
         )
         _ = py.communicate()
     assert_files_equal(cutpath("small.fastq"), out_path)
 
 
+def test_write_interleaved_to_standard_output(tmp_path, cores):
+    out_path = os.fspath(tmp_path / "out.fastq")
+    with open(out_path, "w") as out_file:
+        py = subprocess.Popen(
+            [
+                sys.executable,
+                "-m",
+                "cutadapt",
+                "--cores",
+                str(cores),
+                *"-q 20 -a TTAGACATAT -A CAGTGGAGTA -m 14 -M 90".split(),
+                "-a",
+                "TTAGACATAT",
+                "--interleaved",
+                datapath("paired.1.fastq"),
+                datapath("paired.2.fastq"),
+            ],
+            stdout=out_file,
+        )
+        _ = py.communicate()
+
+    assert_files_equal(cutpath("interleaved.fastq"), out_path)
+
+
 def test_errors_are_printed_to_stderr(tmp_path):
     out_path = os.fspath(tmp_path / "out.fastq")
     py = subprocess.Popen(
         [
             sys.executable,
             "-m",
             "cutadapt",
```

### Comparing `cutadapt-4.7/tests/test_commandline.py` & `cutadapt-4.8/tests/test_commandline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1124,7 +1124,36 @@
             "-o",
             str(tmp_path / "{name}.fastq"),
             datapath("illumina.fastq.gz"),
         ]
     )
     assert stats.n == 100
     assert stats.written == 64
+
+
+@pytest.mark.timeout(1)
+def test_does_not_hang_on_error_in_reader_process(tmp_path, cores):
+    with pytest.raises(SystemExit) as e:
+        main(
+            [
+                f"--cores={cores}",
+                "-o",
+                str(tmp_path / "out.fastq"),
+                str(tmp_path / "does-not-exist.fastq"),
+            ],
+        )
+    assert e.value.args[0] == 1
+
+
+@pytest.mark.skipif(sys.platform != "linux", reason="Platform specific")
+def test_process_substitution(tmp_path, cores):
+    with open(datapath("small.fastq")) as infile:
+        inpath = f"/dev/fd/{infile.fileno()}"
+        main(
+            [
+                f"--cores={cores}",
+                "-o",
+                str(tmp_path / "out.fastq"),
+                inpath,
+            ]
+        )
+    assert_files_equal(datapath("small.fastq"), tmp_path / "out.fastq")
```

### Comparing `cutadapt-4.7/tests/test_files.py` & `cutadapt-4.8/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/test_kmer_finder.py` & `cutadapt-4.8/tests/test_kmer_finder.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/test_kmer_heuristic.py` & `cutadapt-4.8/tests/test_kmer_heuristic.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/test_main.py` & `cutadapt-4.8/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/test_modifiers.py` & `cutadapt-4.8/tests/test_modifiers.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/test_paired.py` & `cutadapt-4.8/tests/test_paired.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/test_parser.py` & `cutadapt-4.8/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/test_predicates.py` & `cutadapt-4.8/tests/test_predicates.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/test_qualtrim.py` & `cutadapt-4.8/tests/test_qualtrim.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/test_stats.py` & `cutadapt-4.8/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/test_testutils.py` & `cutadapt-4.8/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/test_tokenizer.py` & `cutadapt-4.8/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/test_trim.py` & `cutadapt-4.8/tests/test_trim.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/test_utils.py` & `cutadapt-4.8/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tests/utils.py` & `cutadapt-4.8/tests/utils.py`

 * *Files identical despite different names*

### Comparing `cutadapt-4.7/tox.ini` & `cutadapt-4.8/tox.ini`

 * *Files identical despite different names*

