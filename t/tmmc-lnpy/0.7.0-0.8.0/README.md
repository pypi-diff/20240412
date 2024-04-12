# Comparing `tmp/tmmc_lnpy-0.7.0.tar.gz` & `tmp/tmmc_lnpy-0.8.0.tar.gz`

## Comparing `tmmc_lnpy-0.7.0.tar` & `tmmc_lnpy-0.8.0.tar`

### file list

```diff
@@ -1,143 +1,140 @@
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/.cruft.json
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/.editorconfig
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/.gitattributes
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/.markdownlint.yaml
--rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/.prettierignore
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/.prettierrc.yaml
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/AUTHORS.md
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0    16048 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     8734 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/Makefile
--rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/README.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/conftest.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/environment.yaml
--rw-r--r--   0        0        0    35498 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/noxfile.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/changelog.d/README.txt
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/changelog.d/templates/new_fragment.md.j2
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/changelog.d/templates/auto-changelog/macros.jinja2
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/changelog.d/templates/auto-changelog/template.jinja2
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/config/README.md
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/config/nbval.ini
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/config/recipe-append.yaml
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/config/userconfig.example.toml
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/build.txt
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/dev-complete.txt
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/dev.txt
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/docs.txt
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/pipxrun-tools.txt
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/py310-test-extras.yaml
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/py310-test.yaml
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/py310-typing.yaml
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/py311-dev-complete.yaml
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/py311-dev.yaml
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/py311-docs.yaml
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/py311-test-extras.yaml
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/py311-test-notebook.yaml
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/py311-test.yaml
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/py311-typing.yaml
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/py312-test-extras.yaml
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/py312-test.yaml
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/py312-typing.yaml
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/py38-test-extras.yaml
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/py38-test.yaml
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/py38-typing.yaml
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/py39-test-extras.yaml
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/py39-test.yaml
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/py39-typing.yaml
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/test-extras.txt
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/test-notebook.txt
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/test.txt
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/typing.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/.empty
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py310-test.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py310-test.txt.hash.json
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py310-typing.txt
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py310-typing.txt.hash.json
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py311-dev-base.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py311-dev-base.txt.hash.json
--rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py311-dev-complete.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py311-dev-complete.txt.hash.json
--rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py311-dev.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py311-dev.txt.hash.json
--rw-r--r--   0        0        0     5414 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py311-docs.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py311-docs.txt.hash.json
--rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py311-pipxrun-tools.txt
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py311-pipxrun-tools.txt.hash.json
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py311-test-notebook.txt
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py311-test-notebook.txt.hash.json
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py311-test.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py311-test.txt.hash.json
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py311-typing.txt
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py311-typing.txt.hash.json
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py312-test.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py312-test.txt.hash.json
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py312-typing.txt
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py312-typing.txt.hash.json
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py38-test.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py38-test.txt.hash.json
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py38-typing.txt
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py38-typing.txt.hash.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py39-test.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py39-test.txt.hash.json
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py39-typing.txt
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/requirements/lock/py39-typing.txt.hash.json
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnPi/__init__.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnPi/collectionlnpiutils.py
--rw-r--r--   0        0        0    15787 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnPi/maskedlnpi_legacy.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnPi/stability.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnpy/__init__.py
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnpy/_compat.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnpy/_typing.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnpy/_typing_compat.py
--rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnpy/bracket.py
--rw-r--r--   0        0        0    10356 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnpy/combine.py
--rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnpy/docstrings.py
--rw-r--r--   0        0        0    41138 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnpy/ensembles.py
--rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnpy/examples.py
--rw-r--r--   0        0        0    15123 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnpy/extensions.py
--rw-r--r--   0        0        0    15749 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnpy/lnpicollectionutils.py
--rw-r--r--   0        0        0    21828 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnpy/lnpidata.py
--rw-r--r--   0        0        0    26641 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnpy/lnpienergy.py
--rw-r--r--   0        0        0    37330 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnpy/lnpiseries.py
--rw-r--r--   0        0        0     7128 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnpy/molfrac.py
--rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnpy/options.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnpy/py.typed
--rw-r--r--   0        0        0    31857 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnpy/segment.py
--rw-r--r--   0        0        0    34066 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnpy/stability.py
--rw-r--r--   0        0        0    20146 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnpy/utils.py
--rw-r--r--   0        0        0   243309 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnpy/data/hsmix_example.json.gz
--rw-r--r--   0        0        0    38953 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnpy/data/lj_sub_example.json
--rw-r--r--   0        0        0    38751 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnpy/data/lj_sup_example.json
--rw-r--r--   0        0        0   450917 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnpy/data/ljmix_sup_example.json.gz
--rw-r--r--   0        0        0    61595 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/src/lnpy/data/watermof_example.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/tests/conftest.py
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/tests/test_combine.py
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/tests/test_hs_mix.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/tests/test_import.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/tests/test_lj_mix_0.py
--rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/tests/test_lnPi.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/tests/test_lnpicollectionutils.py
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/tests/test_single_comp_sub.py
--rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/tests/test_single_comp_super.py
--rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/tests/test_water_cluster.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/tests/water_cluster/data_0.csv
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/tests/water_cluster/data_0_dw.csv
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/tests/water_cluster/data_1.csv
--rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/tests/water_cluster/data_1_dw.csv
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/tests/water_cluster/water_MOF_ensemble.json
--rw-r--r--   0        0        0    29453 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/tests/water_cluster/water_MOF_example.csv
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/tools/__init__.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/tools/clean_kernelspec.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/tools/common_utils.py
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/tools/create_pythons.py
--rw-r--r--   0        0        0    10810 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/tools/dataclass_parser.py
--rw-r--r--   0        0        0    42224 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/tools/noxtools.py
--rw-r--r--   0        0        0    24193 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/tools/pipxrun.py
--rw-r--r--   0        0        0     8863 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/tools/projectconfig.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/.gitignore
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/LICENSE
--rw-r--r--   0        0        0    10766 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    12431 2020-02-02 00:00:00.000000 tmmc_lnpy-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/.cruft.json
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/.editorconfig
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/.gitattributes
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/.markdownlint.yaml
+-rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/.prettierignore
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/.prettierrc.yaml
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/AUTHORS.md
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0    16048 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     8734 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/Makefile
+-rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/README.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/conftest.py
+-rw-r--r--   0        0        0    35498 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/noxfile.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/changelog.d/README.txt
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/changelog.d/templates/new_fragment.md.j2
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/config/README.md
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/config/nbval.ini
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/config/recipe-append.yaml
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/config/userconfig.example.toml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/build.txt
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/dev-complete.txt
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/dev.txt
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/docs.txt
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/pipxrun-tools.txt
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/py310-test-extras.yaml
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/py310-test.yaml
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/py310-typing.yaml
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/py311-dev-complete.yaml
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/py311-dev.yaml
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/py311-docs.yaml
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/py311-test-extras.yaml
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/py311-test-notebook.yaml
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/py311-test.yaml
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/py311-typing.yaml
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/py312-test-extras.yaml
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/py312-test.yaml
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/py312-typing.yaml
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/py38-test-extras.yaml
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/py38-test.yaml
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/py38-typing.yaml
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/py39-test-extras.yaml
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/py39-test.yaml
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/py39-typing.yaml
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/test-extras.txt
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/test-notebook.txt
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/test.txt
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/typing.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/.empty
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py310-test.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py310-test.txt.hash.json
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py310-typing.txt
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py310-typing.txt.hash.json
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py311-dev-complete.txt
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py311-dev-complete.txt.hash.json
+-rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py311-dev.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py311-dev.txt.hash.json
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py311-docs.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py311-docs.txt.hash.json
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py311-pipxrun-tools.txt
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py311-pipxrun-tools.txt.hash.json
+-rw-r--r--   0        0        0     3472 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py311-test-notebook.txt
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py311-test-notebook.txt.hash.json
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py311-test.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py311-test.txt.hash.json
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py311-typing.txt
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py311-typing.txt.hash.json
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py312-test.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py312-test.txt.hash.json
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py312-typing.txt
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py312-typing.txt.hash.json
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py38-test.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py38-test.txt.hash.json
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py38-typing.txt
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py38-typing.txt.hash.json
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py39-test.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py39-test.txt.hash.json
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py39-typing.txt
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/requirements/lock/py39-typing.txt.hash.json
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnPi/__init__.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnPi/collectionlnpiutils.py
+-rw-r--r--   0        0        0    15787 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnPi/maskedlnpi_legacy.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnPi/stability.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnpy/__init__.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnpy/_compat.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnpy/_typing.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnpy/_typing_compat.py
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnpy/bracket.py
+-rw-r--r--   0        0        0    23581 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnpy/combine.py
+-rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnpy/docstrings.py
+-rw-r--r--   0        0        0    41173 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnpy/ensembles.py
+-rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnpy/examples.py
+-rw-r--r--   0        0        0    15123 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnpy/extensions.py
+-rw-r--r--   0        0        0    15749 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnpy/lnpicollectionutils.py
+-rw-r--r--   0        0        0    21828 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnpy/lnpidata.py
+-rw-r--r--   0        0        0    26646 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnpy/lnpienergy.py
+-rw-r--r--   0        0        0    37212 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnpy/lnpiseries.py
+-rw-r--r--   0        0        0     7128 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnpy/molfrac.py
+-rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnpy/options.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnpy/py.typed
+-rw-r--r--   0        0        0    31857 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnpy/segment.py
+-rw-r--r--   0        0        0    34066 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnpy/stability.py
+-rw-r--r--   0        0        0    20146 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnpy/utils.py
+-rw-r--r--   0        0        0   243309 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnpy/data/hsmix_example.json.gz
+-rw-r--r--   0        0        0    38953 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnpy/data/lj_sub_example.json
+-rw-r--r--   0        0        0    38751 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnpy/data/lj_sup_example.json
+-rw-r--r--   0        0        0   450917 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnpy/data/ljmix_sup_example.json.gz
+-rw-r--r--   0        0        0    61595 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/src/lnpy/data/watermof_example.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/tests/conftest.py
+-rw-r--r--   0        0        0    11257 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/tests/test_combine.py
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/tests/test_hs_mix.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/tests/test_import.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/tests/test_lj_mix_0.py
+-rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/tests/test_lnPi.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/tests/test_lnpicollectionutils.py
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/tests/test_single_comp_sub.py
+-rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/tests/test_single_comp_super.py
+-rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/tests/test_water_cluster.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/tests/water_cluster/data_0.csv
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/tests/water_cluster/data_0_dw.csv
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/tests/water_cluster/data_1.csv
+-rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/tests/water_cluster/data_1_dw.csv
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/tests/water_cluster/water_MOF_ensemble.json
+-rw-r--r--   0        0        0    29453 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/tests/water_cluster/water_MOF_example.csv
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/tools/__init__.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/tools/clean_kernelspec.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/tools/common_utils.py
+-rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/tools/create_pythons.py
+-rw-r--r--   0        0        0    10810 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/tools/dataclass_parser.py
+-rw-r--r--   0        0        0    42224 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/tools/noxtools.py
+-rw-r--r--   0        0        0    24193 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/tools/pipxrun.py
+-rw-r--r--   0        0        0     8863 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/tools/projectconfig.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/LICENSE
+-rw-r--r--   0        0        0    10912 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    12600 2020-02-02 00:00:00.000000 tmmc_lnpy-0.8.0/PKG-INFO
```

### Comparing `tmmc_lnpy-0.7.0/.cruft.json` & `tmmc_lnpy-0.8.0/.cruft.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'e8aa7e52a0a9efdf215ca46471c7890641694b96'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": "develop",
-    "commit": "ad73944b9d513ebc6de10543b9dd9dbe7e48fe02",
+    "commit": "e8aa7e52a0a9efdf215ca46471c7890641694b96",
     "context": {
         "cookiecutter": {
             "__answers": "",
             "_copy_without_render": [],
             "_template": "https://github.com/usnistgov/cookiecutter-nist-python.git",
             "command_line_interface": "none",
             "conda_channel": "conda-forge",
```

### Comparing `tmmc_lnpy-0.7.0/.editorconfig` & `tmmc_lnpy-0.8.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/.pre-commit-config.yaml` & `tmmc_lnpy-0.8.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # See https://pre-commit.com/hooks.html for more hooks
 default_install_hook_types:
   - pre-commit
   - commit-msg
 repos:
   # * Top level
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
       - id: check-json
@@ -42,30 +42,30 @@
         alias: markdownlint
         stages: [commit]
         additional_dependencies:
           - prettier-plugin-toml
 
   # * Markdown
   - repo: https://github.com/DavidAnson/markdownlint-cli2
-    rev: v0.12.1
+    rev: v0.13.0
     hooks:
       - id: markdownlint-cli2
         alias: markdownlint
         args: [--style, prettier]
 
   # * Linting
   # To be replace by ruff analog when I find one ...
   - repo: https://github.com/adamchainz/blacken-docs
     rev: 1.16.0
     hooks:
       - id: blacken-docs
         additional_dependencies:
-          - black==24.2.0
+          - black==24.3.0
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.4
+    rev: v0.3.5
     hooks:
       - id: ruff
         types_or: &ruff-types-or [python, pyi, jupyter]
         args: [--fix, --show-fixes]
       - id: ruff-format
         types_or: *ruff-types-or
 
@@ -110,15 +110,15 @@
             --keep-count, # Errors with nbval without this...
             --extra-keys, # strip out kernelspec.  If use this, always have to reselect kernel when open a notebook...
             "metadata.kernelspec metadata.kernel_spec",
           ]
 
   # * Commit message
   - repo: https://github.com/commitizen-tools/commitizen
-    rev: v3.20.0
+    rev: v3.21.3
     hooks:
       - id: commitizen
         stages: [commit-msg]
 
   # * Manual Linting ------------------------------------------------------------
   - repo: https://github.com/asottile/pyupgrade
     rev: v3.15.2
@@ -133,26 +133,26 @@
         additional_dependencies: [pyupgrade]
         stages: [manual]
         args: [--py38-plus]
 
   # ** typos
   # Probably stick with codespell, but this might also be nice...
   - repo: https://github.com/crate-ci/typos
-    rev: v1.19.0
+    rev: v1.20.7
     hooks:
       - id: typos
         stages: [manual]
         exclude: "[.]ipynb$"
   - repo: https://github.com/nbQA-dev/nbQA
     rev: 1.8.5
     hooks:
       - id: nbqa
         alias: nbqa-typos
         name: nbqa-typos
-        additional_dependencies: &typos-deps [typos==1.19.0] # make sure save version as above.
+        additional_dependencies: &typos-deps [typos==1.20.7] # make sure save version as above.
         stages: [manual]
         args: [typos, --nbqa-shell]
       - id: nbqa
         alias: nbqa-typos
         name: nbqa-typos-markdown
         additional_dependencies: *typos-deps
         stages: [manual]
```

### Comparing `tmmc_lnpy-0.7.0/CHANGELOG.md` & `tmmc_lnpy-0.8.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,21 @@
 
 <!-- prettier-ignore-end -->
 
 <!-- markdownlint-enable MD013 -->
 
 <!-- scriv-insert-here -->
 
+## v0.8.0 — 2024-04-12
+
+### Added
+
+- Added methods to work with collection matrix (`lnpy.combine`).
+- Fixed some minor typing bugs
+
 ## v0.7.0 — 2024-03-28
 
 ### Added
 
 - Added submodule `lnpy.combine` to combine $\ln\Pi$ from multiple simulations.
 
 ## v0.6.0 — 2023-08-24
```

### Comparing `tmmc_lnpy-0.7.0/CONTRIBUTING.md` & `tmmc_lnpy-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/Makefile` & `tmmc_lnpy-0.8.0/Makefile`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/README.md` & `tmmc_lnpy-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/conftest.py` & `tmmc_lnpy-0.8.0/conftest.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/noxfile.py` & `tmmc_lnpy-0.8.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/changelog.d/templates/auto-changelog/template.jinja2` & `tmmc_lnpy-0.8.0/changelog.d/templates/auto-changelog/template.jinja2`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/config/recipe-append.yaml` & `tmmc_lnpy-0.8.0/config/recipe-append.yaml`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/config/userconfig.example.toml` & `tmmc_lnpy-0.8.0/config/userconfig.example.toml`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/requirements/dev-complete.txt` & `tmmc_lnpy-0.8.0/requirements/dev-complete.txt`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 #     $ pyproject2conda project --verbose
 #
 # You should not manually edit this file.
 # Instead edit the corresponding pyproject.toml file.
 #
 bottleneck
-importlib_resources
+importlib_resources;python_version<"3.10"
 ipykernel
 ipython
 ipywidgets
 joblib
 lazy_loader
 matplotlib
 module-utilities>=0.9.0
```

### Comparing `tmmc_lnpy-0.7.0/requirements/dev.txt` & `tmmc_lnpy-0.8.0/requirements/dev.txt`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 #     $ pyproject2conda project --verbose
 #
 # You should not manually edit this file.
 # Instead edit the corresponding pyproject.toml file.
 #
 bottleneck
-importlib_resources
+importlib_resources;python_version<"3.10"
 ipykernel
 ipython
 ipywidgets
 joblib
 lazy_loader
 matplotlib
 module-utilities>=0.9.0
```

### Comparing `tmmc_lnpy-0.7.0/requirements/docs.txt` & `tmmc_lnpy-0.8.0/requirements/docs.txt`

 * *Files 21% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #     $ pyproject2conda project --verbose
 #
 # You should not manually edit this file.
 # Instead edit the corresponding pyproject.toml file.
 #
 autodocsumm
 bottleneck
-importlib_resources
+importlib_resources;python_version<"3.10"
 ipywidgets
 joblib
 lazy_loader
 matplotlib
 module-utilities>=0.9.0
 myst-nb
 numpy
```

### Comparing `tmmc_lnpy-0.7.0/requirements/py310-test.yaml` & `tmmc_lnpy-0.8.0/requirements/py38-test.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # You should not manually edit this file.
 # Instead edit the corresponding pyproject.toml file.
 #
 channels:
   - conda-forge
 dependencies:
-  - python=3.10
+  - python=3.8
   - bottleneck
   - importlib_resources
   - joblib
   - lazy_loader
   - module-utilities>=0.9.0
   - numpy
   - pytest
```

### Comparing `tmmc_lnpy-0.7.0/requirements/py310-typing.yaml` & `tmmc_lnpy-0.8.0/requirements/py38-typing.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # You should not manually edit this file.
 # Instead edit the corresponding pyproject.toml file.
 #
 channels:
   - conda-forge
 dependencies:
-  - python=3.10
+  - python=3.8
   - bottleneck
   - importlib_resources
   - joblib
   - lazy_loader
   - module-utilities>=0.9.0
   - numpy
   - packaging
```

### Comparing `tmmc_lnpy-0.7.0/requirements/py311-dev-complete.yaml` & `tmmc_lnpy-0.8.0/requirements/py311-dev.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -8,37 +8,33 @@
 # Instead edit the corresponding pyproject.toml file.
 #
 channels:
   - conda-forge
 dependencies:
   - python=3.11
   - bottleneck
-  - importlib_resources
   - ipykernel
   - ipython
   - ipywidgets
   - joblib
   - lazy_loader
   - matplotlib-base
   - module-utilities>=0.9.0
   - mypy>=1.9.0
   - nbclient>=0.10.0
   - nbval
   - nox>=2024.3.2
   - numpy
   - packaging
   - pandas-stubs
-  - pipx
-  - pre-commit
   - pytest
   - pytest-cov
   - pytest-sugar
   - pytest-xdist
   - scikit-image>=0.21
   - scipy
   - tqdm
   - types-tqdm
   - xarray
   - pip
   - pip:
       - pytest-accept
-      - scriv
```

### Comparing `tmmc_lnpy-0.7.0/requirements/py311-dev.yaml` & `tmmc_lnpy-0.8.0/requirements/py311-dev-complete.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 # Instead edit the corresponding pyproject.toml file.
 #
 channels:
   - conda-forge
 dependencies:
   - python=3.11
   - bottleneck
-  - importlib_resources
   - ipykernel
   - ipython
   - ipywidgets
   - joblib
   - lazy_loader
   - matplotlib-base
   - module-utilities>=0.9.0
   - mypy>=1.9.0
   - nbclient>=0.10.0
   - nbval
   - nox>=2024.3.2
   - numpy
   - packaging
   - pandas-stubs
+  - pipx
+  - pre-commit
   - pytest
   - pytest-cov
   - pytest-sugar
   - pytest-xdist
   - scikit-image>=0.21
   - scipy
   - tqdm
   - types-tqdm
   - xarray
   - pip
   - pip:
       - pytest-accept
+      - scriv
```

### Comparing `tmmc_lnpy-0.7.0/requirements/py311-docs.yaml` & `tmmc_lnpy-0.8.0/requirements/py311-docs.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #
 channels:
   - conda-forge
 dependencies:
   - python=3.11
   - autodocsumm
   - bottleneck
-  - importlib_resources
   - ipywidgets
   - joblib
   - lazy_loader
   - matplotlib-base
   - module-utilities>=0.9.0
   - myst-nb
   - numpy
```

### Comparing `tmmc_lnpy-0.7.0/requirements/py311-test-notebook.yaml` & `tmmc_lnpy-0.8.0/requirements/py39-test.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -6,25 +6,24 @@
 #
 # You should not manually edit this file.
 # Instead edit the corresponding pyproject.toml file.
 #
 channels:
   - conda-forge
 dependencies:
-  - python=3.11
+  - python=3.9
   - bottleneck
   - importlib_resources
-  - ipywidgets
   - joblib
   - lazy_loader
-  - matplotlib-base
   - module-utilities>=0.9.0
-  - nbval
   - numpy
   - pytest
   - pytest-cov
   - pytest-sugar
   - pytest-xdist
   - scikit-image>=0.21
   - scipy
   - tqdm
+  - typing-extensions
   - xarray
+  - pip
```

### Comparing `tmmc_lnpy-0.7.0/requirements/py38-typing.yaml` & `tmmc_lnpy-0.8.0/requirements/py39-typing.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # You should not manually edit this file.
 # Instead edit the corresponding pyproject.toml file.
 #
 channels:
   - conda-forge
 dependencies:
-  - python=3.8
+  - python=3.9
   - bottleneck
   - importlib_resources
   - joblib
   - lazy_loader
   - module-utilities>=0.9.0
   - numpy
   - packaging
```

### Comparing `tmmc_lnpy-0.7.0/requirements/lock/py310-test.txt` & `tmmc_lnpy-0.8.0/requirements/lock/py39-test.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 # This file was autogenerated by uv via the following command:
-#    uv pip compile --python-version=3.10 --annotation-style=line -o requirements/lock/py310-test.txt requirements/test.txt
+#    uv pip compile --python-version=3.9 --annotation-style=line -o requirements/lock/py39-test.txt requirements/test.txt
 bottleneck==1.3.8
 coverage==7.4.4           # via pytest-cov
 exceptiongroup==1.2.0     # via pytest
-execnet==2.0.2            # via pytest-xdist
+execnet==2.1.1            # via pytest-xdist
 imageio==2.34.0           # via scikit-image
 importlib-resources==6.4.0
 iniconfig==2.0.0          # via pytest
-joblib==1.3.2
-lazy-loader==0.3          # via scikit-image
+joblib==1.4.0
+lazy-loader==0.4          # via scikit-image
 module-utilities==0.9.0
 networkx==3.2.1           # via scikit-image
 numpy==1.26.4             # via bottleneck, imageio, pandas, scikit-image, scipy, tifffile, xarray
-packaging==24.0           # via pytest, pytest-sugar, scikit-image, xarray
-pandas==2.2.1             # via xarray
-pillow==10.2.0            # via imageio, scikit-image
+packaging==24.0           # via lazy-loader, pytest, pytest-sugar, scikit-image, xarray
+pandas==2.2.2             # via xarray
+pillow==10.3.0            # via imageio, scikit-image
 pluggy==1.4.0             # via pytest
 pytest==8.1.1             # via pytest-cov, pytest-sugar, pytest-xdist
 pytest-cov==5.0.0
 pytest-sugar==1.0.0
 pytest-xdist==3.5.0
 python-dateutil==2.9.0.post0  # via pandas
 pytz==2024.1              # via pandas
 scikit-image==0.22.0
-scipy==1.12.0             # via scikit-image
+scipy==1.13.0             # via scikit-image
 six==1.16.0               # via python-dateutil
 termcolor==2.4.0          # via pytest-sugar
 tifffile==2024.2.12       # via scikit-image
 tomli==2.0.1              # via coverage, pytest
 tqdm==4.66.2
-typing-extensions==4.10.0  # via module-utilities
+typing-extensions==4.11.0  # via module-utilities
 tzdata==2024.1            # via pandas
-xarray==2024.2.0
+xarray==2024.3.0
+zipp==3.18.1              # via importlib-resources
```

### Comparing `tmmc_lnpy-0.7.0/requirements/lock/py310-typing.txt` & `tmmc_lnpy-0.8.0/requirements/lock/py38-typing.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 # This file was autogenerated by uv via the following command:
-#    uv pip compile --python-version=3.10 --annotation-style=line -o requirements/lock/py310-typing.txt requirements/typing.txt
+#    uv pip compile --python-version=3.8 --annotation-style=line -o requirements/lock/py38-typing.txt requirements/typing.txt
 bottleneck==1.3.8
 exceptiongroup==1.2.0     # via pytest
 imageio==2.34.0           # via scikit-image
 importlib-resources==6.4.0
 iniconfig==2.0.0          # via pytest
-joblib==1.3.2
-lazy-loader==0.3          # via scikit-image
+joblib==1.4.0
+lazy-loader==0.4          # via scikit-image
 module-utilities==0.9.0
-networkx==3.2.1           # via scikit-image
-numpy==1.26.4             # via bottleneck, imageio, pandas, pandas-stubs, scikit-image, scipy, tifffile, xarray
-packaging==24.0           # via pytest, scikit-image, xarray
-pandas==2.2.1             # via xarray
-pandas-stubs==2.2.1.240316
-pillow==10.2.0            # via imageio, scikit-image
+networkx==3.1             # via scikit-image
+numpy==1.24.4             # via bottleneck, imageio, pandas, pandas-stubs, pywavelets, scikit-image, scipy, tifffile, xarray
+packaging==24.0           # via lazy-loader, pytest, scikit-image, xarray
+pandas==2.0.3             # via xarray
+pandas-stubs==2.0.2.230605
+pillow==10.3.0            # via imageio, scikit-image
 pluggy==1.4.0             # via pytest
 pytest==8.1.1
 python-dateutil==2.9.0.post0  # via pandas
 pytz==2024.1              # via pandas
-scikit-image==0.22.0
-scipy==1.12.0             # via scikit-image
+pywavelets==1.4.1         # via scikit-image
+scikit-image==0.21.0
+scipy==1.10.1             # via scikit-image
 six==1.16.0               # via python-dateutil
-tifffile==2024.2.12       # via scikit-image
+tifffile==2023.7.10       # via scikit-image
 tomli==2.0.1              # via pytest
 tqdm==4.66.2
 types-pytz==2024.1.0.20240203  # via pandas-stubs
 types-tqdm==4.66.0.20240106
-typing-extensions==4.10.0  # via module-utilities
+typing-extensions==4.11.0  # via module-utilities
 tzdata==2024.1            # via pandas
-xarray==2024.2.0
+xarray==2023.1.0
+zipp==3.18.1              # via importlib-resources
```

### Comparing `tmmc_lnpy-0.7.0/requirements/lock/py311-dev-complete.txt` & `tmmc_lnpy-0.8.0/requirements/lock/py311-dev-complete.txt`

 * *Files 9% similar despite different names*

```diff
@@ -8,66 +8,65 @@
 certifi==2024.2.2         # via requests
 cfgv==3.4.0               # via pre-commit
 charset-normalizer==3.3.2  # via requests
 click==8.1.7              # via click-log, scriv, userpath
 click-log==0.4.0          # via scriv
 colorlog==6.8.2           # via nox
 comm==0.2.2               # via ipykernel, ipywidgets
-contourpy==1.2.0          # via matplotlib
+contourpy==1.2.1          # via matplotlib
 coverage==7.4.4           # via nbval, pytest-cov
 cycler==0.12.1            # via matplotlib
 debugpy==1.8.1            # via ipykernel
 decorator==5.1.1          # via ipython
 distlib==0.3.8            # via virtualenv
-execnet==2.0.2            # via pytest-xdist
+execnet==2.1.1            # via pytest-xdist
 executing==2.0.1          # via stack-data
 fastjsonschema==2.19.1    # via nbformat
-filelock==3.13.3          # via virtualenv
-fonttools==4.50.0         # via matplotlib
+filelock==3.13.4          # via virtualenv
+fonttools==4.51.0         # via matplotlib
 identify==2.5.35          # via pre-commit
-idna==3.6                 # via requests
+idna==3.7                 # via requests
 imageio==2.34.0           # via scikit-image
-importlib-resources==6.4.0
 iniconfig==2.0.0          # via pytest
 ipykernel==6.29.4         # via nbval
-ipython==8.22.2           # via ipykernel, ipywidgets
+ipython==8.23.0           # via ipykernel, ipywidgets
 ipywidgets==8.1.2
 jedi==0.19.1              # via ipython
 jinja2==3.1.3             # via scriv
-joblib==1.3.2
+joblib==1.4.0
 jsonschema==4.21.1        # via nbformat
 jsonschema-specifications==2023.12.1  # via jsonschema
 jupyter-client==8.6.1     # via ipykernel, nbclient, nbval
 jupyter-core==5.7.2       # via ipykernel, jupyter-client, nbclient, nbformat
 jupyterlab-widgets==3.0.10  # via ipywidgets
 kiwisolver==1.4.5         # via matplotlib
-lazy-loader==0.3          # via scikit-image
+lazy-loader==0.4          # via scikit-image
 markdown-it-py==3.0.0     # via scriv
 markupsafe==2.1.5         # via jinja2
-matplotlib==3.8.3
+matplotlib==3.8.4
 matplotlib-inline==0.1.6  # via ipykernel, ipython
 mdurl==0.1.2              # via markdown-it-py
 module-utilities==0.9.0
 mypy==1.9.0
 mypy-extensions==1.0.0    # via mypy
 nbclient==0.10.0
-nbformat==5.10.3          # via nbclient, nbval
+nbformat==5.10.4          # via nbclient, nbval
 nbval==0.11.0
 nest-asyncio==1.6.0       # via ipykernel
-networkx==3.2.1           # via scikit-image
+networkx==3.3             # via scikit-image
 nodeenv==1.8.0            # via pre-commit
 nox==2024.3.2
 numpy==1.26.4             # via bottleneck, contourpy, imageio, matplotlib, pandas, pandas-stubs, scikit-image, scipy, tifffile, xarray
-packaging==24.0           # via ipykernel, matplotlib, nox, pipx, pytest, pytest-sugar, scikit-image, xarray
-pandas==2.2.1             # via xarray
+packaging==24.0           # via ipykernel, lazy-loader, matplotlib, nox, pipx, pytest, pytest-sugar, scikit-image, xarray
+pandas==2.2.2             # via xarray
 pandas-stubs==2.2.1.240316
-parso==0.8.3              # via jedi
+parso==0.8.4              # via jedi
 pexpect==4.9.0            # via ipython
-pillow==10.2.0            # via imageio, matplotlib, scikit-image
-pipx==1.4.3
+pillow==10.3.0            # via imageio, matplotlib, scikit-image
+pipx==1.5.0
 platformdirs==4.2.0       # via jupyter-core, pipx, virtualenv
 pluggy==1.4.0             # via pytest
 pre-commit==3.7.0
 prompt-toolkit==3.0.43    # via ipython
 psutil==5.9.8             # via ipykernel
 ptyprocess==0.7.0         # via pexpect
 pure-eval==0.2.2          # via stack-data
@@ -81,28 +80,28 @@
 python-dateutil==2.9.0.post0  # via jupyter-client, matplotlib, pandas
 pytz==2024.1              # via pandas
 pyyaml==6.0.1             # via pre-commit
 pyzmq==25.1.2             # via ipykernel, jupyter-client
 referencing==0.34.0       # via jsonschema, jsonschema-specifications
 requests==2.31.0          # via scriv
 rpds-py==0.18.0           # via jsonschema, referencing
-scikit-image==0.22.0
-scipy==1.12.0             # via scikit-image
+scikit-image==0.23.1
+scipy==1.13.0             # via scikit-image
 scriv==1.5.1
 setuptools==69.2.0        # via nodeenv
 six==1.16.0               # via asttokens, python-dateutil
 stack-data==0.6.3         # via ipython
 termcolor==2.4.0          # via pytest-sugar
 tifffile==2024.2.12       # via scikit-image
 tornado==6.4              # via ipykernel, jupyter-client
 tqdm==4.66.2
 traitlets==5.14.2         # via comm, ipykernel, ipython, ipywidgets, jupyter-client, jupyter-core, matplotlib-inline, nbclient, nbformat
 types-pytz==2024.1.0.20240203  # via pandas-stubs
 types-tqdm==4.66.0.20240106
-typing-extensions==4.10.0  # via module-utilities, mypy
+typing-extensions==4.11.0  # via ipython, module-utilities, mypy
 tzdata==2024.1            # via pandas
 urllib3==2.2.1            # via requests
 userpath==1.9.2           # via pipx
 virtualenv==20.25.1       # via nox, pre-commit
 wcwidth==0.2.13           # via prompt-toolkit
 widgetsnbextension==4.0.10  # via ipywidgets
-xarray==2024.2.0
+xarray==2024.3.0
```

### Comparing `tmmc_lnpy-0.7.0/requirements/lock/py311-dev.txt` & `tmmc_lnpy-0.8.0/requirements/lock/py311-dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,58 +3,57 @@
 appnope==0.1.4            # via ipykernel
 argcomplete==3.2.3        # via nox
 asttokens==2.4.1          # via stack-data
 attrs==23.2.0             # via jsonschema, referencing
 bottleneck==1.3.8
 colorlog==6.8.2           # via nox
 comm==0.2.2               # via ipykernel, ipywidgets
-contourpy==1.2.0          # via matplotlib
+contourpy==1.2.1          # via matplotlib
 coverage==7.4.4           # via nbval, pytest-cov
 cycler==0.12.1            # via matplotlib
 debugpy==1.8.1            # via ipykernel
 decorator==5.1.1          # via ipython
 distlib==0.3.8            # via virtualenv
-execnet==2.0.2            # via pytest-xdist
+execnet==2.1.1            # via pytest-xdist
 executing==2.0.1          # via stack-data
 fastjsonschema==2.19.1    # via nbformat
-filelock==3.13.3          # via virtualenv
-fonttools==4.50.0         # via matplotlib
+filelock==3.13.4          # via virtualenv
+fonttools==4.51.0         # via matplotlib
 imageio==2.34.0           # via scikit-image
-importlib-resources==6.4.0
 iniconfig==2.0.0          # via pytest
 ipykernel==6.29.4         # via nbval
-ipython==8.22.2           # via ipykernel, ipywidgets
+ipython==8.23.0           # via ipykernel, ipywidgets
 ipywidgets==8.1.2
 jedi==0.19.1              # via ipython
-joblib==1.3.2
+joblib==1.4.0
 jsonschema==4.21.1        # via nbformat
 jsonschema-specifications==2023.12.1  # via jsonschema
 jupyter-client==8.6.1     # via ipykernel, nbclient, nbval
 jupyter-core==5.7.2       # via ipykernel, jupyter-client, nbclient, nbformat
 jupyterlab-widgets==3.0.10  # via ipywidgets
 kiwisolver==1.4.5         # via matplotlib
-lazy-loader==0.3          # via scikit-image
-matplotlib==3.8.3
+lazy-loader==0.4          # via scikit-image
+matplotlib==3.8.4
 matplotlib-inline==0.1.6  # via ipykernel, ipython
 module-utilities==0.9.0
 mypy==1.9.0
 mypy-extensions==1.0.0    # via mypy
 nbclient==0.10.0
-nbformat==5.10.3          # via nbclient, nbval
+nbformat==5.10.4          # via nbclient, nbval
 nbval==0.11.0
 nest-asyncio==1.6.0       # via ipykernel
-networkx==3.2.1           # via scikit-image
+networkx==3.3             # via scikit-image
 nox==2024.3.2
 numpy==1.26.4             # via bottleneck, contourpy, imageio, matplotlib, pandas, pandas-stubs, scikit-image, scipy, tifffile, xarray
-packaging==24.0           # via ipykernel, matplotlib, nox, pytest, pytest-sugar, scikit-image, xarray
-pandas==2.2.1             # via xarray
+packaging==24.0           # via ipykernel, lazy-loader, matplotlib, nox, pytest, pytest-sugar, scikit-image, xarray
+pandas==2.2.2             # via xarray
 pandas-stubs==2.2.1.240316
-parso==0.8.3              # via jedi
+parso==0.8.4              # via jedi
 pexpect==4.9.0            # via ipython
-pillow==10.2.0            # via imageio, matplotlib, scikit-image
+pillow==10.3.0            # via imageio, matplotlib, scikit-image
 platformdirs==4.2.0       # via jupyter-core, virtualenv
 pluggy==1.4.0             # via pytest
 prompt-toolkit==3.0.43    # via ipython
 psutil==5.9.8             # via ipykernel
 ptyprocess==0.7.0         # via pexpect
 pure-eval==0.2.2          # via stack-data
 pygments==2.17.2          # via ipython
@@ -65,24 +64,24 @@
 pytest-sugar==1.0.0
 pytest-xdist==3.5.0
 python-dateutil==2.9.0.post0  # via jupyter-client, matplotlib, pandas
 pytz==2024.1              # via pandas
 pyzmq==25.1.2             # via ipykernel, jupyter-client
 referencing==0.34.0       # via jsonschema, jsonschema-specifications
 rpds-py==0.18.0           # via jsonschema, referencing
-scikit-image==0.22.0
-scipy==1.12.0             # via scikit-image
+scikit-image==0.23.1
+scipy==1.13.0             # via scikit-image
 six==1.16.0               # via asttokens, python-dateutil
 stack-data==0.6.3         # via ipython
 termcolor==2.4.0          # via pytest-sugar
 tifffile==2024.2.12       # via scikit-image
 tornado==6.4              # via ipykernel, jupyter-client
 tqdm==4.66.2
 traitlets==5.14.2         # via comm, ipykernel, ipython, ipywidgets, jupyter-client, jupyter-core, matplotlib-inline, nbclient, nbformat
 types-pytz==2024.1.0.20240203  # via pandas-stubs
 types-tqdm==4.66.0.20240106
-typing-extensions==4.10.0  # via module-utilities, mypy
+typing-extensions==4.11.0  # via ipython, module-utilities, mypy
 tzdata==2024.1            # via pandas
 virtualenv==20.25.1       # via nox
 wcwidth==0.2.13           # via prompt-toolkit
 widgetsnbextension==4.0.10  # via ipywidgets
-xarray==2024.2.0
+xarray==2024.3.0
```

### Comparing `tmmc_lnpy-0.7.0/requirements/lock/py311-docs.txt` & `tmmc_lnpy-0.8.0/requirements/lock/py311-docs.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,62 +10,61 @@
 beautifulsoup4==4.12.3    # via pydata-sphinx-theme
 bottleneck==1.3.8
 certifi==2024.2.2         # via requests
 charset-normalizer==3.3.2  # via requests
 click==8.1.7              # via jupyter-cache
 colorama==0.4.6           # via sphinx-autobuild
 comm==0.2.2               # via ipykernel, ipywidgets
-contourpy==1.2.0          # via matplotlib
+contourpy==1.2.1          # via matplotlib
 cycler==0.12.1            # via matplotlib
 debugpy==1.8.1            # via ipykernel
 decorator==5.1.1          # via ipython
 docutils==0.20.1          # via myst-parser, pydata-sphinx-theme, sphinx
 executing==2.0.1          # via stack-data
 fastjsonschema==2.19.1    # via nbformat
-fonttools==4.50.0         # via matplotlib
+fonttools==4.51.0         # via matplotlib
 greenlet==3.0.3           # via sqlalchemy
-idna==3.6                 # via requests
+idna==3.7                 # via requests
 imageio==2.34.0           # via scikit-image
 imagesize==1.4.1          # via sphinx
 importlib-metadata==7.1.0  # via jupyter-cache, myst-nb
-importlib-resources==6.4.0
 ipykernel==6.29.4         # via myst-nb
-ipython==8.22.2           # via ipykernel, ipywidgets, myst-nb
+ipython==8.23.0           # via ipykernel, ipywidgets, myst-nb
 ipywidgets==8.1.2
 jedi==0.19.1              # via ipython
 jinja2==3.1.3             # via myst-parser, sphinx
-joblib==1.3.2
+joblib==1.4.0
 jsonschema==4.21.1        # via nbformat
 jsonschema-specifications==2023.12.1  # via jsonschema
 jupyter-cache==1.0.0      # via myst-nb
 jupyter-client==8.6.1     # via ipykernel, nbclient
 jupyter-core==5.7.2       # via ipykernel, jupyter-client, nbclient, nbformat
 jupyterlab-widgets==3.0.10  # via ipywidgets
 kiwisolver==1.4.5         # via matplotlib
-lazy-loader==0.3          # via scikit-image
+lazy-loader==0.4          # via scikit-image
 livereload==2.6.3         # via sphinx-autobuild
 markdown-it-py==3.0.0     # via mdit-py-plugins, myst-parser
 markupsafe==2.1.5         # via jinja2
-matplotlib==3.8.3
+matplotlib==3.8.4
 matplotlib-inline==0.1.6  # via ipykernel, ipython
 mdit-py-plugins==0.4.0    # via myst-parser
 mdurl==0.1.2              # via markdown-it-py
 module-utilities==0.9.0
-myst-nb==1.0.0
+myst-nb==1.1.0
 myst-parser==2.0.0        # via myst-nb
 nbclient==0.10.0          # via jupyter-cache, myst-nb
-nbformat==5.10.3          # via jupyter-cache, myst-nb, nbclient
+nbformat==5.10.4          # via jupyter-cache, myst-nb, nbclient
 nest-asyncio==1.6.0       # via ipykernel
-networkx==3.2.1           # via scikit-image
+networkx==3.3             # via scikit-image
 numpy==1.26.4             # via bottleneck, contourpy, imageio, matplotlib, pandas, scikit-image, scipy, tifffile, xarray
-packaging==24.0           # via ipykernel, matplotlib, pydata-sphinx-theme, scikit-image, sphinx, xarray
-pandas==2.2.1             # via xarray
-parso==0.8.3              # via jedi
+packaging==24.0           # via ipykernel, lazy-loader, matplotlib, pydata-sphinx-theme, scikit-image, sphinx, xarray
+pandas==2.2.2             # via xarray
+parso==0.8.4              # via jedi
 pexpect==4.9.0            # via ipython
-pillow==10.2.0            # via imageio, matplotlib, scikit-image
+pillow==10.3.0            # via imageio, matplotlib, scikit-image
 platformdirs==4.2.0       # via jupyter-core
 prompt-toolkit==3.0.43    # via ipython
 psutil==5.9.8             # via ipykernel
 ptyprocess==0.7.0         # via pexpect
 pure-eval==0.2.2          # via stack-data
 pydata-sphinx-theme==0.15.2  # via sphinx-book-theme
 pyenchant==3.2.2          # via sphinxcontrib-spelling
@@ -74,16 +73,16 @@
 python-dateutil==2.9.0.post0  # via jupyter-client, matplotlib, pandas
 pytz==2024.1              # via pandas
 pyyaml==6.0.1             # via jupyter-cache, myst-nb, myst-parser
 pyzmq==25.1.2             # via ipykernel, jupyter-client
 referencing==0.34.0       # via jsonschema, jsonschema-specifications
 requests==2.31.0          # via sphinx
 rpds-py==0.18.0           # via jsonschema, referencing
-scikit-image==0.22.0
-scipy==1.12.0             # via scikit-image
+scikit-image==0.23.1
+scipy==1.13.0             # via scikit-image
 six==1.16.0               # via asttokens, livereload, python-dateutil
 snowballstemmer==2.2.0    # via sphinx
 soupsieve==2.5            # via beautifulsoup4
 sphinx==7.2.6             # via autodocsumm, myst-nb, myst-parser, pydata-sphinx-theme, sphinx-autobuild, sphinx-book-theme, sphinx-copybutton, sphinxcontrib-spelling
 sphinx-autobuild==2024.2.4
 sphinx-book-theme==1.1.2
 sphinx-copybutton==0.5.2
@@ -97,14 +96,14 @@
 sqlalchemy==2.0.29        # via jupyter-cache
 stack-data==0.6.3         # via ipython
 tabulate==0.9.0           # via jupyter-cache
 tifffile==2024.2.12       # via scikit-image
 tornado==6.4              # via ipykernel, jupyter-client, livereload
 tqdm==4.66.2
 traitlets==5.14.2         # via comm, ipykernel, ipython, ipywidgets, jupyter-client, jupyter-core, matplotlib-inline, nbclient, nbformat
-typing-extensions==4.10.0  # via module-utilities, myst-nb, pydata-sphinx-theme, sqlalchemy
+typing-extensions==4.11.0  # via ipython, module-utilities, myst-nb, pydata-sphinx-theme, sqlalchemy
 tzdata==2024.1            # via pandas
 urllib3==2.2.1            # via requests
 wcwidth==0.2.13           # via prompt-toolkit
 widgetsnbextension==4.0.10  # via ipywidgets
-xarray==2024.2.0
+xarray==2024.3.0
 zipp==3.18.1              # via importlib-metadata
```

### Comparing `tmmc_lnpy-0.7.0/requirements/lock/py311-pipxrun-tools.txt` & `tmmc_lnpy-0.8.0/requirements/lock/py311-pipxrun-tools.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,75 +1,76 @@
 # This file was autogenerated by uv via the following command:
 #    uv pip compile --python-version=3.11 --annotation-style=line -o requirements/lock/py311-pipxrun-tools.txt requirements/pipxrun-tools.txt
 annotated-types==0.6.0    # via pydantic
 appdirs==1.4.4            # via ensureconda
 asttokens==2.4.1          # via stack-data
 autopep8==2.1.0           # via nbqa
+backports-tarfile==1.0.0  # via jaraco-context
 beautifulsoup4==4.12.3    # via grayskull
 cachecontrol==0.14.0      # via conda-lock
 cachy==0.3.0              # via conda-lock
 certifi==2024.2.2         # via requests
 charset-normalizer==3.3.2  # via requests
 click==8.1.7              # via click-default-group, conda-lock, ensureconda
 click-default-group==1.2.4  # via conda-lock
 clikit==0.6.2             # via conda-lock
 colorama==0.4.6           # via grayskull
 conda-lock==2.5.6
 conda-souschef==2.2.3     # via grayskull
 crashtest==0.3.1          # via clikit, conda-lock
 decorator==5.1.1          # via ipython
 distlib==0.3.8            # via virtualenv
-docutils==0.20.1          # via readme-renderer
+docutils==0.21.1          # via readme-renderer
 ensureconda==1.4.4        # via conda-lock
 executing==2.0.1          # via stack-data
-filelock==3.13.3          # via cachecontrol, ensureconda, virtualenv
+filelock==3.13.4          # via cachecontrol, ensureconda, virtualenv
 gitdb==4.0.11             # via gitpython
-gitpython==3.1.42         # via conda-lock
+gitpython==3.1.43         # via conda-lock
 grayskull==2.6.0
 html5lib==1.1             # via conda-lock
-idna==3.6                 # via requests
+idna==3.7                 # via requests
 importlib-metadata==7.1.0  # via keyring, twine
-ipython==8.22.2           # via nbqa
-jaraco-classes==3.3.1     # via keyring
-jaraco-context==4.3.0     # via keyring
+ipython==8.23.0           # via nbqa
+jaraco-classes==3.4.0     # via keyring
+jaraco-context==5.3.0     # via keyring
 jaraco-functools==4.0.0   # via keyring
 jedi==0.19.1              # via ipython
 jinja2==3.1.3             # via conda-lock
-keyring==25.0.0           # via conda-lock, twine
+keyring==25.1.0           # via conda-lock, twine
 markdown-it-py==3.0.0     # via rich
 markupsafe==2.1.5         # via jinja2
 matplotlib-inline==0.1.6  # via ipython
 mdurl==0.1.2              # via markdown-it-py
 more-itertools==10.2.0    # via jaraco-classes, jaraco-functools
 msgpack==1.0.8            # via cachecontrol
 mypy==1.9.0
 mypy-extensions==1.0.0    # via mypy
 nbqa==1.8.5
 nh3==0.2.17               # via readme-renderer
 nodeenv==1.8.0            # via pyright
 packaging==24.0           # via conda-lock, ensureconda, grayskull
-parso==0.8.3              # via jedi
+parso==0.8.4              # via jedi
 pastel==0.2.1             # via clikit
 pexpect==4.9.0            # via ipython
 pip==24.0                 # via grayskull
 pkginfo==1.10.0           # via conda-lock, grayskull, twine
 platformdirs==4.2.0       # via virtualenv
 progressbar2==4.4.2       # via grayskull
 prompt-toolkit==3.0.43    # via ipython
 ptyprocess==0.7.0         # via pexpect
 pure-eval==0.2.2          # via stack-data
 pycodestyle==2.11.1       # via autopep8
-pydantic==2.6.4           # via conda-lock
-pydantic-core==2.16.3     # via pydantic
+pydantic==2.7.0           # via conda-lock
+pydantic-core==2.18.1     # via pydantic
 pygments==2.17.2          # via ipython, readme-renderer, rich
 pylev==1.4.0              # via clikit
-pyright==1.1.356
+pyright==1.1.357
 python-utils==3.8.2       # via progressbar2
 pyyaml==6.0.1             # via conda-lock
-rapidfuzz==3.7.0          # via grayskull
+rapidfuzz==3.8.1          # via grayskull
 readme-renderer==43.0     # via twine
 requests==2.31.0          # via cachecontrol, conda-lock, ensureconda, grayskull, requests-toolbelt, twine
 requests-toolbelt==1.0.0  # via twine
 rfc3986==2.0.0            # via twine
 rich==13.7.1              # via twine
 ruamel-yaml==0.18.6       # via conda-lock, conda-souschef, grayskull, ruamel-yaml-jinja2
 ruamel-yaml-clib==0.2.8   # via ruamel-yaml
@@ -84,13 +85,13 @@
 tokenize-rt==5.2.0        # via nbqa
 tomli==2.0.1              # via grayskull, nbqa
 tomli-w==1.0.0            # via grayskull
 tomlkit==0.12.4           # via conda-lock
 toolz==0.12.1             # via conda-lock
 traitlets==5.14.2         # via ipython, matplotlib-inline
 twine==5.0.0
-typing-extensions==4.10.0  # via conda-lock, mypy, pydantic, pydantic-core, python-utils
+typing-extensions==4.11.0  # via conda-lock, ipython, mypy, pydantic, pydantic-core, python-utils
 urllib3==1.26.18          # via conda-lock, requests, twine
 virtualenv==20.25.1       # via conda-lock
 wcwidth==0.2.13           # via prompt-toolkit
 webencodings==0.5.1       # via html5lib
 zipp==3.18.1              # via importlib-metadata
```

### Comparing `tmmc_lnpy-0.7.0/requirements/lock/py311-test-notebook.txt` & `tmmc_lnpy-0.8.0/requirements/lock/py311-test-notebook.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 # This file was autogenerated by uv via the following command:
 #    uv pip compile --python-version=3.11 --annotation-style=line -o requirements/lock/py311-test-notebook.txt requirements/test-notebook.txt
 appnope==0.1.4            # via ipykernel
 asttokens==2.4.1          # via stack-data
 attrs==23.2.0             # via jsonschema, referencing
 bottleneck==1.3.8
 comm==0.2.2               # via ipykernel, ipywidgets
-contourpy==1.2.0          # via matplotlib
+contourpy==1.2.1          # via matplotlib
 coverage==7.4.4           # via nbval, pytest-cov
 cycler==0.12.1            # via matplotlib
 debugpy==1.8.1            # via ipykernel
 decorator==5.1.1          # via ipython
-execnet==2.0.2            # via pytest-xdist
+execnet==2.1.1            # via pytest-xdist
 executing==2.0.1          # via stack-data
 fastjsonschema==2.19.1    # via nbformat
-fonttools==4.50.0         # via matplotlib
+fonttools==4.51.0         # via matplotlib
 imageio==2.34.0           # via scikit-image
-importlib-resources==6.4.0
 iniconfig==2.0.0          # via pytest
 ipykernel==6.29.4         # via nbval
-ipython==8.22.2           # via ipykernel, ipywidgets
+ipython==8.23.0           # via ipykernel, ipywidgets
 ipywidgets==8.1.2
 jedi==0.19.1              # via ipython
-joblib==1.3.2
+joblib==1.4.0
 jsonschema==4.21.1        # via nbformat
 jsonschema-specifications==2023.12.1  # via jsonschema
 jupyter-client==8.6.1     # via ipykernel, nbval
 jupyter-core==5.7.2       # via ipykernel, jupyter-client, nbformat
 jupyterlab-widgets==3.0.10  # via ipywidgets
 kiwisolver==1.4.5         # via matplotlib
-lazy-loader==0.3          # via scikit-image
-matplotlib==3.8.3
+lazy-loader==0.4          # via scikit-image
+matplotlib==3.8.4
 matplotlib-inline==0.1.6  # via ipykernel, ipython
 module-utilities==0.9.0
-nbformat==5.10.3          # via nbval
+nbformat==5.10.4          # via nbval
 nbval==0.11.0
 nest-asyncio==1.6.0       # via ipykernel
-networkx==3.2.1           # via scikit-image
+networkx==3.3             # via scikit-image
 numpy==1.26.4             # via bottleneck, contourpy, imageio, matplotlib, pandas, scikit-image, scipy, tifffile, xarray
-packaging==24.0           # via ipykernel, matplotlib, pytest, pytest-sugar, scikit-image, xarray
-pandas==2.2.1             # via xarray
-parso==0.8.3              # via jedi
+packaging==24.0           # via ipykernel, lazy-loader, matplotlib, pytest, pytest-sugar, scikit-image, xarray
+pandas==2.2.2             # via xarray
+parso==0.8.4              # via jedi
 pexpect==4.9.0            # via ipython
-pillow==10.2.0            # via imageio, matplotlib, scikit-image
+pillow==10.3.0            # via imageio, matplotlib, scikit-image
 platformdirs==4.2.0       # via jupyter-core
 pluggy==1.4.0             # via pytest
 prompt-toolkit==3.0.43    # via ipython
 psutil==5.9.8             # via ipykernel
 ptyprocess==0.7.0         # via pexpect
 pure-eval==0.2.2          # via stack-data
 pygments==2.17.2          # via ipython
@@ -55,21 +54,21 @@
 pytest-sugar==1.0.0
 pytest-xdist==3.5.0
 python-dateutil==2.9.0.post0  # via jupyter-client, matplotlib, pandas
 pytz==2024.1              # via pandas
 pyzmq==25.1.2             # via ipykernel, jupyter-client
 referencing==0.34.0       # via jsonschema, jsonschema-specifications
 rpds-py==0.18.0           # via jsonschema, referencing
-scikit-image==0.22.0
-scipy==1.12.0             # via scikit-image
+scikit-image==0.23.1
+scipy==1.13.0             # via scikit-image
 six==1.16.0               # via asttokens, python-dateutil
 stack-data==0.6.3         # via ipython
 termcolor==2.4.0          # via pytest-sugar
 tifffile==2024.2.12       # via scikit-image
 tornado==6.4              # via ipykernel, jupyter-client
 tqdm==4.66.2
 traitlets==5.14.2         # via comm, ipykernel, ipython, ipywidgets, jupyter-client, jupyter-core, matplotlib-inline, nbformat
-typing-extensions==4.10.0  # via module-utilities
+typing-extensions==4.11.0  # via ipython, module-utilities
 tzdata==2024.1            # via pandas
 wcwidth==0.2.13           # via prompt-toolkit
 widgetsnbextension==4.0.10  # via ipywidgets
-xarray==2024.2.0
+xarray==2024.3.0
```

### Comparing `tmmc_lnpy-0.7.0/requirements/lock/py311-test.txt` & `tmmc_lnpy-0.8.0/requirements/lock/py39-typing.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # This file was autogenerated by uv via the following command:
-#    uv pip compile --python-version=3.11 --annotation-style=line -o requirements/lock/py311-test.txt requirements/test.txt
+#    uv pip compile --python-version=3.9 --annotation-style=line -o requirements/lock/py39-typing.txt requirements/typing.txt
 bottleneck==1.3.8
-coverage==7.4.4           # via pytest-cov
-execnet==2.0.2            # via pytest-xdist
+exceptiongroup==1.2.0     # via pytest
 imageio==2.34.0           # via scikit-image
 importlib-resources==6.4.0
 iniconfig==2.0.0          # via pytest
-joblib==1.3.2
-lazy-loader==0.3          # via scikit-image
+joblib==1.4.0
+lazy-loader==0.4          # via scikit-image
 module-utilities==0.9.0
 networkx==3.2.1           # via scikit-image
-numpy==1.26.4             # via bottleneck, imageio, pandas, scikit-image, scipy, tifffile, xarray
-packaging==24.0           # via pytest, pytest-sugar, scikit-image, xarray
-pandas==2.2.1             # via xarray
-pillow==10.2.0            # via imageio, scikit-image
+numpy==1.26.4             # via bottleneck, imageio, pandas, pandas-stubs, scikit-image, scipy, tifffile, xarray
+packaging==24.0           # via lazy-loader, pytest, scikit-image, xarray
+pandas==2.2.2             # via xarray
+pandas-stubs==2.2.1.240316
+pillow==10.3.0            # via imageio, scikit-image
 pluggy==1.4.0             # via pytest
-pytest==8.1.1             # via pytest-cov, pytest-sugar, pytest-xdist
-pytest-cov==5.0.0
-pytest-sugar==1.0.0
-pytest-xdist==3.5.0
+pytest==8.1.1
 python-dateutil==2.9.0.post0  # via pandas
 pytz==2024.1              # via pandas
 scikit-image==0.22.0
-scipy==1.12.0             # via scikit-image
+scipy==1.13.0             # via scikit-image
 six==1.16.0               # via python-dateutil
-termcolor==2.4.0          # via pytest-sugar
 tifffile==2024.2.12       # via scikit-image
+tomli==2.0.1              # via pytest
 tqdm==4.66.2
-typing-extensions==4.10.0  # via module-utilities
+types-pytz==2024.1.0.20240203  # via pandas-stubs
+types-tqdm==4.66.0.20240106
+typing-extensions==4.11.0  # via module-utilities
 tzdata==2024.1            # via pandas
-xarray==2024.2.0
+xarray==2024.3.0
+zipp==3.18.1              # via importlib-resources
```

### Comparing `tmmc_lnpy-0.7.0/requirements/lock/py311-typing.txt` & `tmmc_lnpy-0.8.0/requirements/lock/py312-typing.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # This file was autogenerated by uv via the following command:
-#    uv pip compile --python-version=3.11 --annotation-style=line -o requirements/lock/py311-typing.txt requirements/typing.txt
+#    uv pip compile --python-version=3.12 --annotation-style=line -o requirements/lock/py312-typing.txt requirements/typing.txt
 bottleneck==1.3.8
 imageio==2.34.0           # via scikit-image
-importlib-resources==6.4.0
 iniconfig==2.0.0          # via pytest
-joblib==1.3.2
-lazy-loader==0.3          # via scikit-image
+joblib==1.4.0
+lazy-loader==0.4          # via scikit-image
 module-utilities==0.9.0
-networkx==3.2.1           # via scikit-image
+networkx==3.3             # via scikit-image
 numpy==1.26.4             # via bottleneck, imageio, pandas, pandas-stubs, scikit-image, scipy, tifffile, xarray
-packaging==24.0           # via pytest, scikit-image, xarray
-pandas==2.2.1             # via xarray
+packaging==24.0           # via lazy-loader, pytest, scikit-image, xarray
+pandas==2.2.2             # via xarray
 pandas-stubs==2.2.1.240316
-pillow==10.2.0            # via imageio, scikit-image
+pillow==10.3.0            # via imageio, scikit-image
 pluggy==1.4.0             # via pytest
 pytest==8.1.1
 python-dateutil==2.9.0.post0  # via pandas
 pytz==2024.1              # via pandas
-scikit-image==0.22.0
-scipy==1.12.0             # via scikit-image
+scikit-image==0.23.1
+scipy==1.13.0             # via scikit-image
 six==1.16.0               # via python-dateutil
 tifffile==2024.2.12       # via scikit-image
 tqdm==4.66.2
 types-pytz==2024.1.0.20240203  # via pandas-stubs
 types-tqdm==4.66.0.20240106
-typing-extensions==4.10.0  # via module-utilities
+typing-extensions==4.11.0  # via module-utilities
 tzdata==2024.1            # via pandas
-xarray==2024.2.0
+xarray==2024.3.0
```

### Comparing `tmmc_lnpy-0.7.0/requirements/lock/py312-test.txt` & `tmmc_lnpy-0.8.0/requirements/lock/py310-test.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # This file was autogenerated by uv via the following command:
-#    uv pip compile --python-version=3.12 --annotation-style=line -o requirements/lock/py312-test.txt requirements/test.txt
+#    uv pip compile --python-version=3.10 --annotation-style=line -o requirements/lock/py310-test.txt requirements/test.txt
 bottleneck==1.3.8
 coverage==7.4.4           # via pytest-cov
-execnet==2.0.2            # via pytest-xdist
+exceptiongroup==1.2.0     # via pytest
+execnet==2.1.1            # via pytest-xdist
 imageio==2.34.0           # via scikit-image
-importlib-resources==6.4.0
 iniconfig==2.0.0          # via pytest
-joblib==1.3.2
-lazy-loader==0.3          # via scikit-image
+joblib==1.4.0
+lazy-loader==0.4          # via scikit-image
 module-utilities==0.9.0
-networkx==3.2.1           # via scikit-image
+networkx==3.3             # via scikit-image
 numpy==1.26.4             # via bottleneck, imageio, pandas, scikit-image, scipy, tifffile, xarray
-packaging==24.0           # via pytest, pytest-sugar, scikit-image, xarray
-pandas==2.2.1             # via xarray
-pillow==10.2.0            # via imageio, scikit-image
+packaging==24.0           # via lazy-loader, pytest, pytest-sugar, scikit-image, xarray
+pandas==2.2.2             # via xarray
+pillow==10.3.0            # via imageio, scikit-image
 pluggy==1.4.0             # via pytest
 pytest==8.1.1             # via pytest-cov, pytest-sugar, pytest-xdist
 pytest-cov==5.0.0
 pytest-sugar==1.0.0
 pytest-xdist==3.5.0
 python-dateutil==2.9.0.post0  # via pandas
 pytz==2024.1              # via pandas
-scikit-image==0.22.0
-scipy==1.12.0             # via scikit-image
+scikit-image==0.23.1
+scipy==1.13.0             # via scikit-image
 six==1.16.0               # via python-dateutil
 termcolor==2.4.0          # via pytest-sugar
 tifffile==2024.2.12       # via scikit-image
+tomli==2.0.1              # via coverage, pytest
 tqdm==4.66.2
-typing-extensions==4.10.0  # via module-utilities
+typing-extensions==4.11.0  # via module-utilities
 tzdata==2024.1            # via pandas
-xarray==2024.2.0
+xarray==2024.3.0
```

### Comparing `tmmc_lnpy-0.7.0/requirements/lock/py312-typing.txt` & `tmmc_lnpy-0.8.0/requirements/lock/py311-typing.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # This file was autogenerated by uv via the following command:
-#    uv pip compile --python-version=3.12 --annotation-style=line -o requirements/lock/py312-typing.txt requirements/typing.txt
+#    uv pip compile --python-version=3.11 --annotation-style=line -o requirements/lock/py311-typing.txt requirements/typing.txt
 bottleneck==1.3.8
 imageio==2.34.0           # via scikit-image
-importlib-resources==6.4.0
 iniconfig==2.0.0          # via pytest
-joblib==1.3.2
-lazy-loader==0.3          # via scikit-image
+joblib==1.4.0
+lazy-loader==0.4          # via scikit-image
 module-utilities==0.9.0
-networkx==3.2.1           # via scikit-image
+networkx==3.3             # via scikit-image
 numpy==1.26.4             # via bottleneck, imageio, pandas, pandas-stubs, scikit-image, scipy, tifffile, xarray
-packaging==24.0           # via pytest, scikit-image, xarray
-pandas==2.2.1             # via xarray
+packaging==24.0           # via lazy-loader, pytest, scikit-image, xarray
+pandas==2.2.2             # via xarray
 pandas-stubs==2.2.1.240316
-pillow==10.2.0            # via imageio, scikit-image
+pillow==10.3.0            # via imageio, scikit-image
 pluggy==1.4.0             # via pytest
 pytest==8.1.1
 python-dateutil==2.9.0.post0  # via pandas
 pytz==2024.1              # via pandas
-scikit-image==0.22.0
-scipy==1.12.0             # via scikit-image
+scikit-image==0.23.1
+scipy==1.13.0             # via scikit-image
 six==1.16.0               # via python-dateutil
 tifffile==2024.2.12       # via scikit-image
 tqdm==4.66.2
 types-pytz==2024.1.0.20240203  # via pandas-stubs
 types-tqdm==4.66.0.20240106
-typing-extensions==4.10.0  # via module-utilities
+typing-extensions==4.11.0  # via module-utilities
 tzdata==2024.1            # via pandas
-xarray==2024.2.0
+xarray==2024.3.0
```

### Comparing `tmmc_lnpy-0.7.0/requirements/lock/py38-test.txt` & `tmmc_lnpy-0.8.0/requirements/lock/py38-test.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # This file was autogenerated by uv via the following command:
 #    uv pip compile --python-version=3.8 --annotation-style=line -o requirements/lock/py38-test.txt requirements/test.txt
 bottleneck==1.3.8
 coverage==7.4.4           # via pytest-cov
 exceptiongroup==1.2.0     # via pytest
-execnet==2.0.2            # via pytest-xdist
+execnet==2.1.1            # via pytest-xdist
 imageio==2.34.0           # via scikit-image
 importlib-resources==6.4.0
 iniconfig==2.0.0          # via pytest
-joblib==1.3.2
-lazy-loader==0.3          # via scikit-image
+joblib==1.4.0
+lazy-loader==0.4          # via scikit-image
 module-utilities==0.9.0
 networkx==3.1             # via scikit-image
 numpy==1.24.4             # via bottleneck, imageio, pandas, pywavelets, scikit-image, scipy, tifffile, xarray
-packaging==24.0           # via pytest, pytest-sugar, scikit-image, xarray
+packaging==24.0           # via lazy-loader, pytest, pytest-sugar, scikit-image, xarray
 pandas==2.0.3             # via xarray
-pillow==10.2.0            # via imageio, scikit-image
+pillow==10.3.0            # via imageio, scikit-image
 pluggy==1.4.0             # via pytest
 pytest==8.1.1             # via pytest-cov, pytest-sugar, pytest-xdist
 pytest-cov==5.0.0
 pytest-sugar==1.0.0
 pytest-xdist==3.5.0
 python-dateutil==2.9.0.post0  # via pandas
 pytz==2024.1              # via pandas
@@ -26,11 +26,11 @@
 scikit-image==0.21.0
 scipy==1.10.1             # via scikit-image
 six==1.16.0               # via python-dateutil
 termcolor==2.4.0          # via pytest-sugar
 tifffile==2023.7.10       # via scikit-image
 tomli==2.0.1              # via coverage, pytest
 tqdm==4.66.2
-typing-extensions==4.10.0  # via module-utilities
+typing-extensions==4.11.0  # via module-utilities
 tzdata==2024.1            # via pandas
 xarray==2023.1.0
 zipp==3.18.1              # via importlib-resources
```

### Comparing `tmmc_lnpy-0.7.0/requirements/lock/py38-typing.txt` & `tmmc_lnpy-0.8.0/requirements/lock/py310-typing.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 # This file was autogenerated by uv via the following command:
-#    uv pip compile --python-version=3.8 --annotation-style=line -o requirements/lock/py38-typing.txt requirements/typing.txt
+#    uv pip compile --python-version=3.10 --annotation-style=line -o requirements/lock/py310-typing.txt requirements/typing.txt
 bottleneck==1.3.8
 exceptiongroup==1.2.0     # via pytest
 imageio==2.34.0           # via scikit-image
-importlib-resources==6.4.0
 iniconfig==2.0.0          # via pytest
-joblib==1.3.2
-lazy-loader==0.3          # via scikit-image
+joblib==1.4.0
+lazy-loader==0.4          # via scikit-image
 module-utilities==0.9.0
-networkx==3.1             # via scikit-image
-numpy==1.24.4             # via bottleneck, imageio, pandas, pandas-stubs, pywavelets, scikit-image, scipy, tifffile, xarray
-packaging==24.0           # via pytest, scikit-image, xarray
-pandas==2.0.3             # via xarray
-pandas-stubs==2.0.2.230605
-pillow==10.2.0            # via imageio, scikit-image
+networkx==3.3             # via scikit-image
+numpy==1.26.4             # via bottleneck, imageio, pandas, pandas-stubs, scikit-image, scipy, tifffile, xarray
+packaging==24.0           # via lazy-loader, pytest, scikit-image, xarray
+pandas==2.2.2             # via xarray
+pandas-stubs==2.2.1.240316
+pillow==10.3.0            # via imageio, scikit-image
 pluggy==1.4.0             # via pytest
 pytest==8.1.1
 python-dateutil==2.9.0.post0  # via pandas
 pytz==2024.1              # via pandas
-pywavelets==1.4.1         # via scikit-image
-scikit-image==0.21.0
-scipy==1.10.1             # via scikit-image
+scikit-image==0.23.1
+scipy==1.13.0             # via scikit-image
 six==1.16.0               # via python-dateutil
-tifffile==2023.7.10       # via scikit-image
+tifffile==2024.2.12       # via scikit-image
 tomli==2.0.1              # via pytest
 tqdm==4.66.2
 types-pytz==2024.1.0.20240203  # via pandas-stubs
 types-tqdm==4.66.0.20240106
-typing-extensions==4.10.0  # via module-utilities
+typing-extensions==4.11.0  # via module-utilities
 tzdata==2024.1            # via pandas
-xarray==2023.1.0
-zipp==3.18.1              # via importlib-resources
+xarray==2024.3.0
```

### Comparing `tmmc_lnpy-0.7.0/requirements/lock/py39-test.txt` & `tmmc_lnpy-0.8.0/requirements/lock/py312-test.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 # This file was autogenerated by uv via the following command:
-#    uv pip compile --python-version=3.9 --annotation-style=line -o requirements/lock/py39-test.txt requirements/test.txt
+#    uv pip compile --python-version=3.12 --annotation-style=line -o requirements/lock/py312-test.txt requirements/test.txt
 bottleneck==1.3.8
 coverage==7.4.4           # via pytest-cov
-exceptiongroup==1.2.0     # via pytest
-execnet==2.0.2            # via pytest-xdist
+execnet==2.1.1            # via pytest-xdist
 imageio==2.34.0           # via scikit-image
-importlib-resources==6.4.0
 iniconfig==2.0.0          # via pytest
-joblib==1.3.2
-lazy-loader==0.3          # via scikit-image
+joblib==1.4.0
+lazy-loader==0.4          # via scikit-image
 module-utilities==0.9.0
-networkx==3.2.1           # via scikit-image
+networkx==3.3             # via scikit-image
 numpy==1.26.4             # via bottleneck, imageio, pandas, scikit-image, scipy, tifffile, xarray
-packaging==24.0           # via pytest, pytest-sugar, scikit-image, xarray
-pandas==2.2.1             # via xarray
-pillow==10.2.0            # via imageio, scikit-image
+packaging==24.0           # via lazy-loader, pytest, pytest-sugar, scikit-image, xarray
+pandas==2.2.2             # via xarray
+pillow==10.3.0            # via imageio, scikit-image
 pluggy==1.4.0             # via pytest
 pytest==8.1.1             # via pytest-cov, pytest-sugar, pytest-xdist
 pytest-cov==5.0.0
 pytest-sugar==1.0.0
 pytest-xdist==3.5.0
 python-dateutil==2.9.0.post0  # via pandas
 pytz==2024.1              # via pandas
-scikit-image==0.22.0
-scipy==1.12.0             # via scikit-image
+scikit-image==0.23.1
+scipy==1.13.0             # via scikit-image
 six==1.16.0               # via python-dateutil
 termcolor==2.4.0          # via pytest-sugar
 tifffile==2024.2.12       # via scikit-image
-tomli==2.0.1              # via coverage, pytest
 tqdm==4.66.2
-typing-extensions==4.10.0  # via module-utilities
+typing-extensions==4.11.0  # via module-utilities
 tzdata==2024.1            # via pandas
-xarray==2024.2.0
-zipp==3.18.1              # via importlib-resources
+xarray==2024.3.0
```

### Comparing `tmmc_lnpy-0.7.0/src/lnPi/__init__.py` & `tmmc_lnpy-0.8.0/src/lnPi/__init__.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/src/lnPi/maskedlnpi_legacy.py` & `tmmc_lnpy-0.8.0/src/lnPi/maskedlnpi_legacy.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/src/lnpy/__init__.py` & `tmmc_lnpy-0.8.0/src/lnpy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """Publicly accessible classes/routines."""
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from . import ensembles, lnpienergy, segment  # noqa: TCH004
-    from .combine import combine_lnpi  # noqa: TCH004
+    from . import combine, ensembles, lnpienergy, segment  # noqa: TCH004
     from .lnpidata import lnPiMasked  # noqa: TCH004
     from .lnpiseries import lnPiCollection  # noqa: TCH004
     from .options import OPTIONS, set_options  # noqa: TCH004
     from .segment import PhaseCreator  # noqa: TCH004
 else:
     import lazy_loader as lazy
 
     __getattr__, __dir__, _ = lazy.attach(
         __name__,
-        submodules=["ensembles", "lnpienergy", "segment"],
+        submodules=["ensembles", "lnpienergy", "segment", "combine"],
         submod_attrs={
             "lnpidata": ["lnPiMasked"],
             "lnpiseries": ["lnPiCollection"],
             "options": ["OPTIONS", "set_options"],
             "segment": ["PhaseCreator"],
         },
     )
@@ -39,15 +38,15 @@
 
 __all__ = [
     "OPTIONS",
     "PhaseCreator",
     "__author__",
     "__email__",
     "__version__",
-    "combine_lnpi",
+    "combine",
     "ensembles",
     "lnPiCollection",
     "lnPiMasked",
     "lnpienergy",
     "segment",
     "set_options",
 ]
```

### Comparing `tmmc_lnpy-0.7.0/src/lnpy/_typing.py` & `tmmc_lnpy-0.8.0/src/lnpy/_typing.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/src/lnpy/bracket.py` & `tmmc_lnpy-0.8.0/src/lnpy/bracket.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/src/lnpy/docstrings.py` & `tmmc_lnpy-0.8.0/src/lnpy/docstrings.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/src/lnpy/ensembles.py` & `tmmc_lnpy-0.8.0/src/lnpy/ensembles.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 if TYPE_CHECKING:
     from typing import Any, Callable, Hashable, Mapping, Sequence
 
     import pandas as pd
     from numpy.typing import ArrayLike
 
     from ._typing import C_Ensemble, MyNDArray, P, R, T_Ensemble, xArrayLike
+    from ._typing_compat import IndexAny
 
 # from lnpy.lnpidata import lnPiMasked
 # from lnpy.lnpiseries import lnPiCollection
 
 
 # always check_use_cache here.
 cached_prop = cached.prop(check_use_cache=True)
@@ -242,20 +243,19 @@
     def _standard_attrs(self) -> dict[str, Any]:
         return self._wrapper.attrs(*self._parent.state_kws.keys())
 
     @property
     def first(self) -> lnPiMasked:
         if isinstance(self._parent, lnPiCollection):
             return self._parent.iloc[0]
-
         return self._parent
 
     # @cached_prop to much memory
     @property
-    def _rec_coords(self) -> dict[str, pd.Index[Any] | pd.MultiIndex | float | int]:
+    def _rec_coords(self) -> dict[str, IndexAny | pd.MultiIndex | float | int]:
         if isinstance(self._parent, lnPiMasked):
             return dict(self._parent._index_dict(), **self._parent.state_kws)
 
         return {
             self._parent._concat_dim: self._parent.index,
             **self._parent.state_kws,
         }
```

### Comparing `tmmc_lnpy-0.7.0/src/lnpy/examples.py` & `tmmc_lnpy-0.8.0/src/lnpy/examples.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 """
 Examples (:mod:`~lnpy.examples`)
 ================================
 """
 
 from __future__ import annotations
 
-try:
-    import importlib_resources as resources
-except ImportError:
-    from importlib import resources  # type: ignore[no-redef]
-
 import json
 from dataclasses import asdict, dataclass
 from typing import TYPE_CHECKING, TypedDict
 
 import numpy as np
 import xarray as xr
 
+from ._compat import resources
+
 # from .lnpiseries import lnPiCollection
 from .segment import BuildPhasesBase, PhaseCreator
 from .utils import dataset_to_lnpimasked
 
 if TYPE_CHECKING:
     from typing import Any, Iterator, Literal, Sequence
 
@@ -50,15 +47,21 @@
     if basename.endswith(".gz"):
         import gzip
 
         fopen = gzip.open
     else:
         fopen = open  # type: ignore[assignment]
 
-    with fopen(resources.files("lnpy.data").joinpath(basename), "r") as f:  # pyright: ignore[reportCallIssue,reportArgumentType]
+    # path = Path(resources.files("lnpy.data").joinpath(basename))
+    # with fopen(path, "r") as f:  # pyright: ignore[reportCallIssue,reportArgumentType]
+    #     return json.load(f)  # type: ignore[no-any-return]
+
+    with resources.as_file(
+        resources.files("lnpy.data").joinpath(basename)
+    ) as path, fopen(path, "r") as f:
         return json.load(f)  # type: ignore[no-any-return]
 
 
 class ExampleDict(TypedDict):
     """Example dict"""
 
     lnPi_data: MyNDArray
```

### Comparing `tmmc_lnpy-0.7.0/src/lnpy/extensions.py` & `tmmc_lnpy-0.8.0/src/lnpy/extensions.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/src/lnpy/lnpicollectionutils.py` & `tmmc_lnpy-0.8.0/src/lnpy/lnpicollectionutils.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/src/lnpy/lnpidata.py` & `tmmc_lnpy-0.8.0/src/lnpy/lnpidata.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/src/lnpy/lnpienergy.py` & `tmmc_lnpy-0.8.0/src/lnpy/lnpienergy.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from .utils import get_tqdm_calc as get_tqdm
 from .utils import labels_to_masks, masks_change_convention, parallel_map_func_starargs
 
 if TYPE_CHECKING:
     from typing import Any, Iterable, Literal, Sequence, Union
 
     from ._typing import MaskConvention, MyNDArray
-    from ._typing_compat import Self
+    from ._typing_compat import IndexAny, Self
     from .lnpiseries import lnPiCollection
 
     _FindBoundariesMode = Literal["thick", "inner", "outer", "subpixel"]
     _FindBoundariesMethod = Literal["exact", "approx"]
     _Extrema = Literal["min", "max"]
 
     _FillArg = Union[int, None]
@@ -680,15 +680,15 @@
 
     def __init__(self, parent: lnPiCollection) -> None:
         self._parent = parent
         self._use_joblib = getattr(self._parent, "_use_joblib", False)
 
         self._cache: dict[str, Any] = {}
 
-    def _get_items_ws(self) -> tuple[list[pd.Index[Any]], list[wFreeEnergy]]:
+    def _get_items_ws(self) -> tuple[list[IndexAny], list[wFreeEnergy]]:
         indexes = []
         ws = []
         for _, phases in self._parent.groupby_allbut("phase"):
             indexes.append(phases.index)
             masks = [x.mask for x in phases.to_numpy()]
 
             ws.append(
```

### Comparing `tmmc_lnpy-0.7.0/src/lnpy/lnpiseries.py` & `tmmc_lnpy-0.8.0/src/lnpy/lnpiseries.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     )
 
     from numpy.typing import ArrayLike, DTypeLike
     from pandas.core.groupby.generic import SeriesGroupBy
 
     from . import ensembles, lnpienergy, stability
     from ._typing import IndexingInt, MyNDArray, Scalar
-    from ._typing_compat import Self
+    from ._typing_compat import IndexAny, Self
     from .lnpidata import lnPiMasked
 
 
 # Accessors
 class _CallableResult:
     def __init__(self, parent: lnPiCollection, func: Callable[..., Any]) -> None:
         functools.update_wrapper(self, func)
@@ -89,15 +89,15 @@
 
     @overload
     def __getitem__(self, idx: Scalar | tuple[Scalar, ...]) -> lnPiMasked: ...
 
     @overload
     def __getitem__(
         self,
-        idx: list[Scalar] | pd.Index[Any] | slice | Callable[[pd.Series[Any]], Any],
+        idx: list[Scalar] | IndexAny | slice | Callable[[pd.Series[Any]], Any],
     ) -> lnPiCollection: ...
 
     @overload
     def __getitem__(self, idx: Any) -> lnPiMasked | lnPiCollection: ...
 
     def __getitem__(self, idx: Any) -> lnPiMasked | lnPiCollection:
         out = self._loc[idx]
@@ -123,17 +123,15 @@
         self._parent = parent
         self._iloc = self._parent._series.iloc
 
     @overload
     def __getitem__(self, idx: IndexingInt) -> lnPiMasked: ...
 
     @overload
-    def __getitem__(
-        self, idx: Sequence[int] | pd.Index[Any] | slice
-    ) -> lnPiCollection: ...
+    def __getitem__(self, idx: Sequence[int] | IndexAny | slice) -> lnPiCollection: ...
 
     @overload
     def __getitem__(self, idx: Any) -> lnPiMasked | lnPiCollection: ...
 
     def __getitem__(self, idx: Any) -> lnPiMasked | lnPiCollection:
         out = self._iloc[idx]
         if isinstance(out, pd.Series):
@@ -200,28 +198,28 @@
         self._parent = parent
         self._level = level
         self._index = self._parent.index
 
         self._index_names = set(self._index.names)
         self._loc = self._parent._series.iloc
 
-    def _get_loc_idx(self, idx: pd.MultiIndex | pd.Index[Any]) -> Any:
+    def _get_loc_idx(self, idx: pd.MultiIndex | IndexAny) -> Any:
         index = self._index
         if isinstance(idx, pd.MultiIndex):
             # names in idx and
             drop: list[Hashable] = list(self._index_names - set(idx.names))
             index = index.droplevel(drop)
             # reorder idx
             idx = idx.reorder_levels(index.names)  # type: ignore[no-untyped-call]
         else:
             drop = list(set(index.names) - {idx.name})
             index = index.droplevel(drop)
         return index.get_indexer_for(idx)  # type: ignore[no-untyped-call]
 
-    def __getitem__(self, idx: pd.MultiIndex | pd.Index[Any]) -> lnPiCollection:
+    def __getitem__(self, idx: pd.MultiIndex | IndexAny) -> lnPiCollection:
         indexer = self._get_loc_idx(idx)
         out = self._loc[indexer]
 
         if isinstance(out, pd.Series):
             out = self._parent.new_like(out)
         else:
             msg = "unknown indexer for mloc"
@@ -264,15 +262,15 @@
     _xarray_unstack = True
     _xarray_dot_kws: Final = {"optimize": "optimal"}
     _use_cache = True
 
     def __init__(
         self,
         data: Sequence[lnPiMasked] | pd.Series[Any],
-        index: ArrayLike | pd.Index[Any] | pd.MultiIndex | None = None,
+        index: ArrayLike | IndexAny | pd.MultiIndex | None = None,
         xarray_output: bool = True,
         concat_dim: str | None = None,
         concat_coords: str | None = None,
         unstack: bool = True,
         name: Hashable | None = None,
         base_class: str | type = "first",
         dtype: DTypeLike | None = None,
@@ -332,15 +330,15 @@
             # would like to do this, but
             # fails for parallel builds
             # assert lnpi._base is _base
 
     def new_like(
         self,
         data: Sequence[lnPiMasked] | pd.Series[Any] | None = None,
-        index: ArrayLike | pd.Index[Any] | pd.MultiIndex | None = None,
+        index: ArrayLike | IndexAny | pd.MultiIndex | None = None,
         **kwargs: Any,
     ) -> Self:
         """Create new object with optional new data/index"""
         if data is None:
             data = self.s
 
         return type(self)(
@@ -380,15 +378,15 @@
 
     @property
     def items(self) -> MyNDArray:
         """Alias to :attr:`values`"""
         return self.values
 
     @property
-    def index(self) -> pd.Index[Any]:
+    def index(self) -> IndexAny:
         """Series index"""
         return self._series.index
 
     @property
     def name(self) -> Hashable:
         """Series name"""
         return self._series.name
@@ -706,36 +704,32 @@
             concat_kws = {}
         s = cls._concat_to_series(objs, **concat_kws)
         return cls(s, *args, **kwargs)
 
     # Note: use property(cached.meth(func)) here
     # normal cache.prop has some logic issues
     # with this pattern.
-    @property
-    @cached.meth
+
+    @cached.prop
     def loc(self) -> _LocIndexer:
         return _LocIndexer(self)
 
-    @property
-    @cached.meth
+    @cached.prop
     def iloc(self) -> _iLocIndexer:
         return _iLocIndexer(self)
 
-    @property
-    @cached.meth
+    @cached.prop
     def query(self) -> _Query:
         return _Query(self)
 
-    @property
-    @cached.meth
+    @cached.prop
     def zloc(self) -> _LocIndexer_unstack_zloc:
         return _LocIndexer_unstack_zloc(self)
 
-    @property
-    @cached.meth
+    @cached.prop
     def mloc(self) -> _LocIndexer_unstack_mloc:
         return _LocIndexer_unstack_mloc(self)
 
     # ** lnPi Specific
     @cached.prop
     def _lnz_series(self) -> pd.Series[Any]:
         return self._series.apply(lambda x: x.lnz)  # type: ignore[no-any-return]
@@ -799,23 +793,23 @@
             (self.zloc[zloc]._series if zloc is not None else self._series).iloc[iloc]
         )
         lnz = v.lnz
         if component is not None:
             lnz = lnz[component]
         return lnz
 
-    def _get_level(self, level: str = "phase") -> pd.Index[Any]:
+    def _get_level(self, level: str = "phase") -> IndexAny:
         """Return level values from index"""
         index = self.index
         if isinstance(index, pd.MultiIndex):
             level_idx = index.names.index(level)
             index = index.levels[level_idx]
         return index
 
-    def get_index_level(self, level: str = "phase") -> pd.Index[Any]:
+    def get_index_level(self, level: str = "phase") -> IndexAny:
         """Get index values for specified level"""
         return self._get_level(level=level)
 
     # @cached.prop
     @property
     def _nrec(self) -> int:
         return len(self._series)
```

### Comparing `tmmc_lnpy-0.7.0/src/lnpy/molfrac.py` & `tmmc_lnpy-0.8.0/src/lnpy/molfrac.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/src/lnpy/options.py` & `tmmc_lnpy-0.8.0/src/lnpy/options.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/src/lnpy/segment.py` & `tmmc_lnpy-0.8.0/src/lnpy/segment.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/src/lnpy/stability.py` & `tmmc_lnpy-0.8.0/src/lnpy/stability.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/src/lnpy/utils.py` & `tmmc_lnpy-0.8.0/src/lnpy/utils.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/src/lnpy/data/hsmix_example.json.gz` & `tmmc_lnpy-0.8.0/src/lnpy/data/hsmix_example.json.gz`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/src/lnpy/data/lj_sub_example.json` & `tmmc_lnpy-0.8.0/src/lnpy/data/lj_sub_example.json`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/src/lnpy/data/lj_sup_example.json` & `tmmc_lnpy-0.8.0/src/lnpy/data/lj_sup_example.json`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/src/lnpy/data/ljmix_sup_example.json.gz` & `tmmc_lnpy-0.8.0/src/lnpy/data/ljmix_sup_example.json.gz`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/src/lnpy/data/watermof_example.json` & `tmmc_lnpy-0.8.0/src/lnpy/data/watermof_example.json`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/tests/conftest.py` & `tmmc_lnpy-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/tests/test_hs_mix.py` & `tmmc_lnpy-0.8.0/tests/test_hs_mix.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/tests/test_lj_mix_0.py` & `tmmc_lnpy-0.8.0/tests/test_lj_mix_0.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/tests/test_lnPi.py` & `tmmc_lnpy-0.8.0/tests/test_lnPi.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/tests/test_lnpicollectionutils.py` & `tmmc_lnpy-0.8.0/tests/test_lnpicollectionutils.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/tests/test_single_comp_sub.py` & `tmmc_lnpy-0.8.0/tests/test_single_comp_sub.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/tests/test_single_comp_super.py` & `tmmc_lnpy-0.8.0/tests/test_single_comp_super.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/tests/test_water_cluster.py` & `tmmc_lnpy-0.8.0/tests/test_water_cluster.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/tests/water_cluster/data_0.csv` & `tmmc_lnpy-0.8.0/tests/water_cluster/data_0.csv`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/tests/water_cluster/data_1.csv` & `tmmc_lnpy-0.8.0/tests/water_cluster/data_1.csv`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/tests/water_cluster/data_1_dw.csv` & `tmmc_lnpy-0.8.0/tests/water_cluster/data_1_dw.csv`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/tests/water_cluster/water_MOF_example.csv` & `tmmc_lnpy-0.8.0/tests/water_cluster/water_MOF_example.csv`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/tools/clean_kernelspec.py` & `tmmc_lnpy-0.8.0/tools/clean_kernelspec.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/tools/common_utils.py` & `tmmc_lnpy-0.8.0/tools/common_utils.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/tools/create_pythons.py` & `tmmc_lnpy-0.8.0/tools/create_pythons.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/tools/dataclass_parser.py` & `tmmc_lnpy-0.8.0/tools/dataclass_parser.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/tools/noxtools.py` & `tmmc_lnpy-0.8.0/tools/noxtools.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/tools/pipxrun.py` & `tmmc_lnpy-0.8.0/tools/pipxrun.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/tools/projectconfig.py` & `tmmc_lnpy-0.8.0/tools/projectconfig.py`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/.gitignore` & `tmmc_lnpy-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/LICENSE` & `tmmc_lnpy-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tmmc_lnpy-0.7.0/pyproject.toml` & `tmmc_lnpy-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ]
 dynamic = [
     "readme",
     "version",
 ]
 dependencies = [
     "bottleneck",
-    "importlib_resources",
+    "importlib_resources;python_version<'3.10'",
     "joblib",
     "lazy_loader",
     "module-utilities >= 0.9.0",
     "numpy",
     "scikit-image >= 0.21",
     "scipy",
     "tqdm",
@@ -83,15 +83,15 @@
     "packaging",
 ]
 pipxrun-tools = [
     # these used solely for specking tools to be used with tools/pipxrun.py
     "conda-lock >= 2.5.5",
     "grayskull >= 2.5.3",
     "nbqa >= 1.8.4",
-    "pyright >= 1.1.356",
+    "pyright >= 1.1.357, != 1.1.358", # note pyright == 1.1.358 breaks cached.meth of lnPiCollection.loc/iloc/etc.  Need to patch module-utilities...
     "tmmc-lnpy[mypy]",
     "twine >= 5.0.0",
 ]
 test = [
     "pytest",
     "pytest-cov",
     "pytest-sugar",
```

### Comparing `tmmc_lnpy-0.7.0/PKG-INFO` & `tmmc_lnpy-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmmc-lnpy
-Version: 0.7.0
+Version: 0.8.0
 Summary: Analysis of lnPi results from TMMC simulation
 Project-URL: Documentation, https://pages.nist.gov/tmmc-lnpy/
 Project-URL: Homepage, https://github.com/usnistgov/tmmc-lnpy
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST-PD
 License-File: LICENSE
 Keywords: tmmc-lnpy
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: <=3.12,>=3.8
 Requires-Dist: bottleneck
-Requires-Dist: importlib-resources
+Requires-Dist: importlib-resources; python_version < '3.10'
 Requires-Dist: joblib
 Requires-Dist: lazy-loader
 Requires-Dist: module-utilities>=0.9.0
 Requires-Dist: numpy
 Requires-Dist: scikit-image>=0.21
 Requires-Dist: scipy
 Requires-Dist: tqdm
@@ -58,15 +58,15 @@
 Requires-Dist: nbval; extra == 'nbval'
 Provides-Extra: pipxrun
 Requires-Dist: packaging; extra == 'pipxrun'
 Provides-Extra: pipxrun-tools
 Requires-Dist: conda-lock>=2.5.5; extra == 'pipxrun-tools'
 Requires-Dist: grayskull>=2.5.3; extra == 'pipxrun-tools'
 Requires-Dist: nbqa>=1.8.4; extra == 'pipxrun-tools'
-Requires-Dist: pyright>=1.1.356; extra == 'pipxrun-tools'
+Requires-Dist: pyright!=1.1.358,>=1.1.357; extra == 'pipxrun-tools'
 Requires-Dist: tmmc-lnpy[mypy]; extra == 'pipxrun-tools'
 Requires-Dist: twine>=5.0.0; extra == 'pipxrun-tools'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-sugar; extra == 'test'
 Requires-Dist: pytest-xdist; extra == 'test'
@@ -253,14 +253,21 @@
 
 <!-- prettier-ignore-end -->
 
 <!-- markdownlint-enable MD013 -->
 
 <!-- scriv-insert-here -->
 
+## v0.8.0 — 2024-04-12
+
+### Added
+
+- Added methods to work with collection matrix (`lnpy.combine`).
+- Fixed some minor typing bugs
+
 ## v0.7.0 — 2024-03-28
 
 ### Added
 
 - Added submodule `lnpy.combine` to combine $\ln\Pi$ from multiple simulations.
 
 ## v0.6.0 — 2023-08-24
```

