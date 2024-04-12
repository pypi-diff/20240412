# Comparing `tmp/geniac-3.2.1.tar.gz` & `tmp/geniac-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geniac-3.2.1.tar", last modified: Fri Oct 13 13:54:16 2023, max compression
+gzip compressed data, was "geniac-3.3.0.tar", last modified: Fri Apr 12 09:07:36 2024, max compression
```

## Comparing `geniac-3.2.1.tar` & `geniac-3.3.0.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:16.052518 geniac-3.2.1/
--rw-rw-rw-   0 root         (0) nobody   (65534)      589 2023-10-12 15:13:53.000000 geniac-3.2.1/.coveragerc
--rw-rw-rw-   0 root         (0) nobody   (65534)       47 2023-10-12 15:13:53.000000 geniac-3.2.1/.gitattributes
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:14.354647 geniac-3.2.1/.github/
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:14.671891 geniac-3.2.1/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0 root         (0) nobody   (65534)      511 2023-10-12 15:13:53.000000 geniac-3.2.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-rw-   0 root         (0) nobody   (65534)      265 2023-10-12 15:13:53.000000 geniac-3.2.1/.github/ISSUE_TEMPLATE/new_feature.md
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:14.682144 geniac-3.2.1/.github/PULL_REQUEST_TEMPLATE/
--rw-rw-rw-   0 root         (0) nobody   (65534)      298 2023-10-12 15:13:53.000000 geniac-3.2.1/.github/PULL_REQUEST_TEMPLATE/merge_request_template.md
--rw-rw-rw-   0 root         (0) nobody   (65534)      623 2023-10-12 15:13:53.000000 geniac-3.2.1/.gitignore
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:14.363431 geniac-3.2.1/.gitlab/
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:14.703111 geniac-3.2.1/.gitlab/issue_templates/
--rw-rw-rw-   0 root         (0) nobody   (65534)      511 2023-10-12 15:13:53.000000 geniac-3.2.1/.gitlab/issue_templates/bug_report.md
--rw-rw-rw-   0 root         (0) nobody   (65534)      265 2023-10-12 15:13:53.000000 geniac-3.2.1/.gitlab/issue_templates/new_feature.md
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:14.713662 geniac-3.2.1/.gitlab/merge_request_templates/
--rw-rw-rw-   0 root         (0) nobody   (65534)      298 2023-10-12 15:13:53.000000 geniac-3.2.1/.gitlab/merge_request_templates/merge_request_template.md
--rw-rw-rw-   0 root         (0) nobody   (65534)      765 2023-10-12 15:13:53.000000 geniac-3.2.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) nobody   (65534)       54 2023-10-12 15:13:53.000000 geniac-3.2.1/.isort.cfg
--rw-rw-rw-   0 root         (0) nobody   (65534)     1355 2023-10-12 15:13:53.000000 geniac-3.2.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) nobody   (65534)      554 2023-10-12 15:13:53.000000 geniac-3.2.1/.readthedocs.yml
--rw-rw-rw-   0 root         (0) nobody   (65534)    11910 2023-10-12 15:13:53.000000 geniac-3.2.1/CHANGELOG
--rw-rw-rw-   0 root         (0) nobody   (65534)     4555 2023-10-12 15:13:53.000000 geniac-3.2.1/CMakeLists.txt
--rw-rw-rw-   0 root         (0) nobody   (65534)     2567 2023-10-12 15:13:53.000000 geniac-3.2.1/INSTALL.md
--rw-rw-rw-   0 root         (0) nobody   (65534)    21778 2023-10-12 15:13:53.000000 geniac-3.2.1/LICENSE
--rw-r--r--   0 root         (0) nobody   (65534)    36424 2023-10-13 13:54:16.046801 geniac-3.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) nobody   (65534)     1532 2023-10-12 15:13:53.000000 geniac-3.2.1/README.md
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:14.883320 geniac-3.2.1/cmake/
--rw-rw-rw-   0 root         (0) nobody   (65534)     2824 2023-10-12 15:13:53.000000 geniac-3.2.1/cmake/CMakeLists.txt
--rw-rw-rw-   0 root         (0) nobody   (65534)     2780 2023-10-12 15:13:53.000000 geniac-3.2.1/cmake/FindApptainer.cmake
--rw-rw-rw-   0 root         (0) nobody   (65534)     2683 2023-10-12 15:13:53.000000 geniac-3.2.1/cmake/FindDocker.cmake
--rw-rw-rw-   0 root         (0) nobody   (65534)     2834 2023-10-12 15:13:53.000000 geniac-3.2.1/cmake/FindNextflow.cmake
--rw-rw-rw-   0 root         (0) nobody   (65534)     2683 2023-10-12 15:13:53.000000 geniac-3.2.1/cmake/FindPodman.cmake
--rw-rw-rw-   0 root         (0) nobody   (65534)     2994 2023-10-12 15:13:53.000000 geniac-3.2.1/cmake/FindSingularity.cmake
--rw-rw-rw-   0 root         (0) nobody   (65534)     2082 2023-10-12 15:13:53.000000 geniac-3.2.1/cmake/checkConfigFiles.cmake
--rw-rw-rw-   0 root         (0) nobody   (65534)     1099 2023-10-12 15:13:53.000000 geniac-3.2.1/cmake/createPathDirectories.cmake
--rw-rw-rw-   0 root         (0) nobody   (65534)     1987 2023-10-12 15:13:53.000000 geniac-3.2.1/cmake/createWorkDir.cmake
--rw-rw-rw-   0 root         (0) nobody   (65534)     2086 2023-10-12 15:13:53.000000 geniac-3.2.1/cmake/functionColorMessage.cmake
--rw-rw-rw-   0 root         (0) nobody   (65534)     1293 2023-10-12 15:13:53.000000 geniac-3.2.1/cmake/initCmakePreload.sh
--rw-rw-rw-   0 root         (0) nobody   (65534)     2136 2023-10-12 15:13:53.000000 geniac-3.2.1/cmake/stepAddTestTargets.cmake
--rw-rw-rw-   0 root         (0) nobody   (65534)     5530 2023-10-12 15:13:53.000000 geniac-3.2.1/cmake/stepCheckOptions.cmake
--rw-rw-rw-   0 root         (0) nobody   (65534)     2310 2023-10-12 15:13:53.000000 geniac-3.2.1/cmake/stepFindPackages.cmake
--rw-rw-rw-   0 root         (0) nobody   (65534)     4031 2023-10-12 15:13:53.000000 geniac-3.2.1/cmake/stepGitInfo.cmake
--rw-rw-rw-   0 root         (0) nobody   (65534)    16624 2023-10-12 15:13:53.000000 geniac-3.2.1/cmake/stepMainCoreScript.cmake
--rw-rw-rw-   0 root         (0) nobody   (65534)     5649 2023-10-12 15:13:53.000000 geniac-3.2.1/cmake/stepSetVariables.cmake
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:14.913105 geniac-3.2.1/data/
--rw-rw-rw-   0 root         (0) nobody   (65534)     4052 2023-10-12 15:13:53.000000 geniac-3.2.1/data/CMakeLists.txt
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:15.015801 geniac-3.2.1/data/conf/
--rw-rw-rw-   0 root         (0) nobody   (65534)      228 2023-10-12 15:13:53.000000 geniac-3.2.1/data/conf/cluster.config
--rw-rw-rw-   0 root         (0) nobody   (65534)      593 2023-10-12 15:13:53.000000 geniac-3.2.1/data/conf/conda.config
--rw-rw-rw-   0 root         (0) nobody   (65534)      590 2023-10-12 15:13:53.000000 geniac-3.2.1/data/conf/docker.config
--rw-rw-rw-   0 root         (0) nobody   (65534)     2497 2023-10-12 15:13:53.000000 geniac-3.2.1/data/conf/geniac.config
--rw-rw-rw-   0 root         (0) nobody   (65534)      431 2023-10-12 15:13:53.000000 geniac-3.2.1/data/conf/genomes.config
--rw-rw-rw-   0 root         (0) nobody   (65534)      606 2023-10-12 15:13:53.000000 geniac-3.2.1/data/conf/multiconda.config
--rw-rw-rw-   0 root         (0) nobody   (65534)     1468 2023-10-12 15:13:53.000000 geniac-3.2.1/data/conf/multipath.config
--rw-rw-rw-   0 root         (0) nobody   (65534)      807 2023-10-12 15:13:53.000000 geniac-3.2.1/data/conf/path.config
--rw-rw-rw-   0 root         (0) nobody   (65534)      590 2023-10-12 15:13:53.000000 geniac-3.2.1/data/conf/podman.config
--rw-rw-rw-   0 root         (0) nobody   (65534)     1676 2023-10-12 15:13:53.000000 geniac-3.2.1/data/conf/singularity.config
--rw-rw-rw-   0 root         (0) nobody   (65534)     2639 2023-10-12 15:13:53.000000 geniac-3.2.1/data/createSubmodule.bash
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:14.376609 geniac-3.2.1/data/modules/
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:15.026766 geniac-3.2.1/data/modules/fromSource/
--rw-rw-rw-   0 root         (0) nobody   (65534)     1943 2023-10-12 15:13:53.000000 geniac-3.2.1/data/modules/fromSource/CMakeLists.txt
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:14.383076 geniac-3.2.1/data/nf-modules/
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:14.386764 geniac-3.2.1/data/nf-modules/local/
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:15.040673 geniac-3.2.1/data/nf-modules/local/process/
--rw-rw-rw-   0 root         (0) nobody   (65534)     2013 2023-10-12 15:13:53.000000 geniac-3.2.1/data/nf-modules/local/process/renvInit.nf
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:14.402483 geniac-3.2.1/data/recipes/
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:14.395391 geniac-3.2.1/data/recipes/dependencies/
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:15.052810 geniac-3.2.1/data/recipes/dependencies/renvGlad/
--rw-rw-rw-   0 root         (0) nobody   (65534)     1875 2023-10-12 15:13:53.000000 geniac-3.2.1/data/recipes/dependencies/renvGlad/renv.lock
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:15.064805 geniac-3.2.1/data/recipes/docker/
--rw-rw-rw-   0 root         (0) nobody   (65534)     1261 2023-10-12 15:13:53.000000 geniac-3.2.1/data/recipes/docker/r.Dockerfile
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:15.075751 geniac-3.2.1/data/recipes/singularity/
--rw-rw-rw-   0 root         (0) nobody   (65534)     1241 2023-10-12 15:13:53.000000 geniac-3.2.1/data/recipes/singularity/r.def
--rw-rw-rw-   0 root         (0) nobody   (65534)     3818 2023-10-12 15:13:53.000000 geniac-3.2.1/data/useCases.bash
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:15.308214 geniac-3.2.1/docs/
--rw-rw-rw-   0 root         (0) nobody   (65534)     1180 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/Makefile
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:15.319523 geniac-3.2.1/docs/_static/
--rw-rw-rw-   0 root         (0) nobody   (65534)       18 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/_static/.gitignore
--rw-rw-rw-   0 root         (0) nobody   (65534)     4148 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/admin.rst
--rw-rw-rw-   0 root         (0) nobody   (65534)      321 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/check.rst
--rw-rw-rw-   0 root         (0) nobody   (65534)     3977 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/cli.rst
--rw-rw-rw-   0 root         (0) nobody   (65534)    14570 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/conda.rst
--rw-rw-rw-   0 root         (0) nobody   (65534)     5327 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/conf.py
--rw-rw-rw-   0 root         (0) nobody   (65534)     4538 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/customcmd.rst
--rw-rw-rw-   0 root         (0) nobody   (65534)     6257 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/devcycle.rst
--rw-rw-rw-   0 root         (0) nobody   (65534)     1678 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/environment.yml
--rw-rw-rw-   0 root         (0) nobody   (65534)    18295 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/faq.rst
--rw-rw-rw-   0 root         (0) nobody   (65534)     8034 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/from-source-examples.rst
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:15.447708 geniac-3.2.1/docs/images/
--rw-rw-rw-   0 root         (0) nobody   (65534)   102057 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/images/bash-startup.png
--rw-rw-rw-   0 root         (0) nobody   (65534)   184337 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/images/geniac-cli-uml.png
--rw-rw-rw-   0 root         (0) nobody   (65534)    10972 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/images/geniac-logo.png
--rw-rw-rw-   0 root         (0) nobody   (65534)     7514 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/images/geniac-logo.svg
--rw-rw-rw-   0 root         (0) nobody   (65534)    12102 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/images/geniac.uml
--rw-rw-rw-   0 root         (0) nobody   (65534)    50235 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/images/git-workflow.png
--rw-rw-rw-   0 root         (0) nobody   (65534)    24741 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/images/git-workflow.svg
--rw-rw-rw-   0 root         (0) nobody   (65534)      127 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/images/image-source.txt
--rw-rw-rw-   0 root         (0) nobody   (65534)    22607 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/images/install.png
--rw-rw-rw-   0 root         (0) nobody   (65534)     9413 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/images/installed.png
--rw-rw-rw-   0 root         (0) nobody   (65534)     7719 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/images/path.png
--rw-rw-rw-   0 root         (0) nobody   (65534)      536 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/index.rst
--rw-rw-rw-   0 root         (0) nobody   (65534)    16975 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/install.rst
--rw-rw-rw-   0 root         (0) nobody   (65534)     4000 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/intro.rst
--rw-rw-rw-   0 root         (0) nobody   (65534)      646 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/linux.rst
--rw-rw-rw-   0 root         (0) nobody   (65534)      133 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/misc.rst
--rw-rw-rw-   0 root         (0) nobody   (65534)     3365 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/overview.rst
--rw-rw-rw-   0 root         (0) nobody   (65534)    24883 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/process.rst
--rw-rw-rw-   0 root         (0) nobody   (65534)     1381 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/profiles.rst
--rw-rw-rw-   0 root         (0) nobody   (65534)     4641 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/renv.rst
--rw-rw-rw-   0 root         (0) nobody   (65534)      342 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/requirements.txt
--rw-rw-rw-   0 root         (0) nobody   (65534)    15909 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/run.rst
--rw-rw-rw-   0 root         (0) nobody   (65534)     2849 2023-10-12 15:13:53.000000 geniac-3.2.1/docs/substitutions.rst
--rw-rw-rw-   0 root         (0) nobody   (65534)      722 2023-10-12 15:13:53.000000 geniac-3.2.1/environment.yml
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:15.490952 geniac-3.2.1/install/
--rw-rw-rw-   0 root         (0) nobody   (65534)     1371 2023-10-12 15:13:53.000000 geniac-3.2.1/install/cmake-init-default.cmake
--rw-rw-rw-   0 root         (0) nobody   (65534)    16595 2023-10-12 15:13:53.000000 geniac-3.2.1/install/docker.nf
--rw-rw-rw-   0 root         (0) nobody   (65534)     2126 2023-10-12 15:13:53.000000 geniac-3.2.1/install/nextflow.config.in
--rw-rw-rw-   0 root         (0) nobody   (65534)    34355 2023-10-12 15:13:53.000000 geniac-3.2.1/install/singularity.nf
--rw-rw-rw-   0 root         (0) nobody   (65534)      311 2023-10-12 15:13:53.000000 geniac-3.2.1/pyproject.toml
--rw-rw-rw-   0 root         (0) nobody   (65534)     2033 2023-10-13 13:54:16.061337 geniac-3.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) nobody   (65534)      703 2023-10-12 15:13:53.000000 geniac-3.2.1/setup.py
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:14.421677 geniac-3.2.1/src/
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:15.503113 geniac-3.2.1/src/geniac/
--rw-rw-rw-   0 root         (0) nobody   (65534)      392 2023-10-12 15:13:53.000000 geniac-3.2.1/src/geniac/__init__.py
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:15.600826 geniac-3.2.1/src/geniac/cli/
--rw-rw-rw-   0 root         (0) nobody   (65534)       46 2023-10-12 15:13:53.000000 geniac-3.2.1/src/geniac/cli/__init__.py
--rw-rw-rw-   0 root         (0) nobody   (65534)    15278 2023-10-12 15:13:53.000000 geniac-3.2.1/src/geniac/cli/__main__.py
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:15.706446 geniac-3.2.1/src/geniac/cli/commands/
--rw-rw-rw-   0 root         (0) nobody   (65534)       77 2023-10-12 15:13:53.000000 geniac-3.2.1/src/geniac/cli/commands/__init__.py
--rw-rw-rw-   0 root         (0) nobody   (65534)     2668 2023-10-12 15:13:53.000000 geniac-3.2.1/src/geniac/cli/commands/base.py
--rw-rw-rw-   0 root         (0) nobody   (65534)     1057 2023-10-12 15:13:53.000000 geniac-3.2.1/src/geniac/cli/commands/clean.py
--rw-rw-rw-   0 root         (0) nobody   (65534)     2209 2023-10-12 15:13:53.000000 geniac-3.2.1/src/geniac/cli/commands/configs.py
--rw-rw-rw-   0 root         (0) nobody   (65534)     2436 2023-10-12 15:13:53.000000 geniac-3.2.1/src/geniac/cli/commands/init.py
--rw-rw-rw-   0 root         (0) nobody   (65534)    10068 2023-10-12 15:13:53.000000 geniac-3.2.1/src/geniac/cli/commands/install.py
--rw-rw-rw-   0 root         (0) nobody   (65534)    66083 2023-10-12 15:13:54.000000 geniac-3.2.1/src/geniac/cli/commands/lint.py
--rw-rw-rw-   0 root         (0) nobody   (65534)     2354 2023-10-12 15:13:54.000000 geniac-3.2.1/src/geniac/cli/commands/options.py
--rw-rw-rw-   0 root         (0) nobody   (65534)     2723 2023-10-12 15:13:54.000000 geniac-3.2.1/src/geniac/cli/commands/recipes.py
--rw-rw-rw-   0 root         (0) nobody   (65534)     1454 2023-10-12 15:13:54.000000 geniac-3.2.1/src/geniac/cli/commands/test.py
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:14.439886 geniac-3.2.1/src/geniac/cli/data/
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:15.729250 geniac-3.2.1/src/geniac/cli/data/conf/
--rw-rw-rw-   0 root         (0) nobody   (65534)    16475 2023-10-12 15:13:54.000000 geniac-3.2.1/src/geniac/cli/data/conf/geniac.ini
--rw-rw-rw-   0 root         (0) nobody   (65534)     1709 2023-10-12 15:13:54.000000 geniac-3.2.1/src/geniac/cli/data/conf/logging.json
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:15.739795 geniac-3.2.1/src/geniac/cli/data/scripts/
--rw-rw-rw-   0 root         (0) nobody   (65534)     7387 2023-10-12 15:13:54.000000 geniac-3.2.1/src/geniac/cli/data/scripts/geniac.bash
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:15.781487 geniac-3.2.1/src/geniac/cli/parsers/
--rw-rw-rw-   0 root         (0) nobody   (65534)       76 2023-10-12 15:13:54.000000 geniac-3.2.1/src/geniac/cli/parsers/__init__.py
--rw-rw-rw-   0 root         (0) nobody   (65534)     5747 2023-10-12 15:13:54.000000 geniac-3.2.1/src/geniac/cli/parsers/base.py
--rw-rw-rw-   0 root         (0) nobody   (65534)    15057 2023-10-12 15:13:54.000000 geniac-3.2.1/src/geniac/cli/parsers/config.py
--rw-rw-rw-   0 root         (0) nobody   (65534)     6596 2023-10-12 15:13:54.000000 geniac-3.2.1/src/geniac/cli/parsers/scripts.py
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:15.812717 geniac-3.2.1/src/geniac/cli/utils/
--rw-rw-rw-   0 root         (0) nobody   (65534)       74 2023-10-12 15:13:54.000000 geniac-3.2.1/src/geniac/cli/utils/__init__.py
--rw-rw-rw-   0 root         (0) nobody   (65534)    25129 2023-10-12 15:13:54.000000 geniac-3.2.1/src/geniac/cli/utils/base.py
--rw-rw-rw-   0 root         (0) nobody   (65534)     1919 2023-10-12 15:13:54.000000 geniac-3.2.1/src/geniac/cli/utils/logging.py
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:15.579987 geniac-3.2.1/src/geniac.egg-info/
--rw-r--r--   0 root         (0) nobody   (65534)    36424 2023-10-13 13:54:14.000000 geniac-3.2.1/src/geniac.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) nobody   (65534)     3993 2023-10-13 13:54:14.000000 geniac-3.2.1/src/geniac.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) nobody   (65534)        1 2023-10-13 13:54:14.000000 geniac-3.2.1/src/geniac.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) nobody   (65534)       52 2023-10-13 13:54:14.000000 geniac-3.2.1/src/geniac.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) nobody   (65534)        1 2023-10-13 13:54:13.000000 geniac-3.2.1/src/geniac.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) nobody   (65534)      188 2023-10-13 13:54:14.000000 geniac-3.2.1/src/geniac.egg-info/requires.txt
--rw-r--r--   0 root         (0) nobody   (65534)        7 2023-10-13 13:54:14.000000 geniac-3.2.1/src/geniac.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:15.864016 geniac-3.2.1/tests/
--rw-rw-rw-   0 root         (0) nobody   (65534)       77 2023-10-12 15:13:54.000000 geniac-3.2.1/tests/__init__.py
--rw-rw-rw-   0 root         (0) nobody   (65534)      322 2023-10-12 15:13:54.000000 geniac-3.2.1/tests/conftest.py
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:15.883221 geniac-3.2.1/tests/data/
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:16.010108 geniac-3.2.1/tests/data/conf/
--rw-rw-rw-   0 root         (0) nobody   (65534)      254 2023-10-12 15:13:54.000000 geniac-3.2.1/tests/data/conf/README.md
--rw-rw-rw-   0 root         (0) nobody   (65534)      394 2023-10-12 15:13:54.000000 geniac-3.2.1/tests/data/conf/base.config
--rwxrwxrwx   0 root         (0) nobody   (65534)      226 2023-10-12 15:13:54.000000 geniac-3.2.1/tests/data/conf/cluster.config
--rw-rw-rw-   0 root         (0) nobody   (65534)      252 2023-10-12 15:13:54.000000 geniac-3.2.1/tests/data/conf/conda.config
--rw-rw-rw-   0 root         (0) nobody   (65534)      287 2023-10-12 15:13:54.000000 geniac-3.2.1/tests/data/conf/docker.config
--rw-rw-rw-   0 root         (0) nobody   (65534)     1155 2023-10-12 15:13:54.000000 geniac-3.2.1/tests/data/conf/geniac.config
--rw-rw-rw-   0 root         (0) nobody   (65534)      430 2023-10-12 15:13:54.000000 geniac-3.2.1/tests/data/conf/genomes.config
--rw-rw-rw-   0 root         (0) nobody   (65534)      253 2023-10-12 15:13:54.000000 geniac-3.2.1/tests/data/conf/multiconda.config
--rw-rw-rw-   0 root         (0) nobody   (65534)     1064 2023-10-12 15:13:54.000000 geniac-3.2.1/tests/data/conf/multipath.config
--rw-rw-rw-   0 root         (0) nobody   (65534)      808 2023-10-12 15:13:54.000000 geniac-3.2.1/tests/data/conf/path.config
--rw-rw-rw-   0 root         (0) nobody   (65534)     3692 2023-10-12 15:13:54.000000 geniac-3.2.1/tests/data/conf/process.config
--rw-rw-rw-   0 root         (0) nobody   (65534)     1259 2023-10-12 15:13:54.000000 geniac-3.2.1/tests/data/conf/singularity.config
--rw-rw-rw-   0 root         (0) nobody   (65534)      797 2023-10-12 15:13:54.000000 geniac-3.2.1/tests/data/conf/test.config
--rw-rw-rw-   0 root         (0) nobody   (65534)    15327 2023-10-12 15:13:54.000000 geniac-3.2.1/tests/data/main.nf
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:14.461727 geniac-3.2.1/tests/data/modules/
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:16.020877 geniac-3.2.1/tests/data/modules/fromSource/
--rw-rw-rw-   0 root         (0) nobody   (65534)        0 2023-10-12 15:13:54.000000 geniac-3.2.1/tests/data/modules/fromSource/CMakeLists.txt
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:16.029173 geniac-3.2.1/tests/data/modules/fromSource/dolorSit/
--rw-rw-rw-   0 root         (0) nobody   (65534)        0 2023-10-12 15:13:54.000000 geniac-3.2.1/tests/data/modules/fromSource/dolorSit/CMakeLists.txt
-drwxr-xr-x   0 root         (0) nobody   (65534)        0 2023-10-13 13:54:16.037095 geniac-3.2.1/tests/data/modules/fromSource/helloWorld/
--rw-rw-rw-   0 root         (0) nobody   (65534)        0 2023-10-12 15:13:54.000000 geniac-3.2.1/tests/data/modules/fromSource/helloWorld/CMakeLists.txt
--rw-rw-rw-   0 root         (0) nobody   (65534)     1689 2023-10-12 15:13:54.000000 geniac-3.2.1/tests/data/nextflow.config
--rw-rw-rw-   0 root         (0) nobody   (65534)     1646 2023-10-12 15:13:54.000000 geniac-3.2.1/tests/test_base.py
--rw-rw-rw-   0 root         (0) nobody   (65534)      595 2023-10-12 15:13:54.000000 geniac-3.2.1/tests/test_commands_lint.py
--rw-rw-rw-   0 root         (0) nobody   (65534)      280 2023-10-12 15:13:54.000000 geniac-3.2.1/tests/test_main.py
--rw-rw-rw-   0 root         (0) nobody   (65534)     1921 2023-10-12 15:13:54.000000 geniac-3.2.1/tox.ini
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:35.997072 geniac-3.3.0/
+-rw-rw-rw-   0 root         (0) nobody   (65534)      589 2024-04-12 08:57:31.000000 geniac-3.3.0/.coveragerc
+-rw-rw-rw-   0 root         (0) nobody   (65534)       47 2024-04-12 08:57:31.000000 geniac-3.3.0/.gitattributes
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:33.562896 geniac-3.3.0/.github/
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:34.150796 geniac-3.3.0/.github/ISSUE_TEMPLATE/
+-rw-rw-rw-   0 root         (0) nobody   (65534)      511 2024-04-12 08:57:31.000000 geniac-3.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-rw-   0 root         (0) nobody   (65534)      265 2024-04-12 08:57:31.000000 geniac-3.3.0/.github/ISSUE_TEMPLATE/new_feature.md
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:34.168092 geniac-3.3.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-rw-rw-   0 root         (0) nobody   (65534)      298 2024-04-12 08:57:31.000000 geniac-3.3.0/.github/PULL_REQUEST_TEMPLATE/merge_request_template.md
+-rw-rw-rw-   0 root         (0) nobody   (65534)      623 2024-04-12 08:57:31.000000 geniac-3.3.0/.gitignore
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:33.570326 geniac-3.3.0/.gitlab/
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:34.209918 geniac-3.3.0/.gitlab/issue_templates/
+-rw-rw-rw-   0 root         (0) nobody   (65534)      511 2024-04-12 08:57:31.000000 geniac-3.3.0/.gitlab/issue_templates/bug_report.md
+-rw-rw-rw-   0 root         (0) nobody   (65534)      265 2024-04-12 08:57:31.000000 geniac-3.3.0/.gitlab/issue_templates/new_feature.md
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:34.227519 geniac-3.3.0/.gitlab/merge_request_templates/
+-rw-rw-rw-   0 root         (0) nobody   (65534)      298 2024-04-12 08:57:31.000000 geniac-3.3.0/.gitlab/merge_request_templates/merge_request_template.md
+-rw-rw-rw-   0 root         (0) nobody   (65534)      765 2024-04-12 08:57:31.000000 geniac-3.3.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) nobody   (65534)       54 2024-04-12 08:57:31.000000 geniac-3.3.0/.isort.cfg
+-rw-rw-rw-   0 root         (0) nobody   (65534)     1355 2024-04-12 08:57:31.000000 geniac-3.3.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) nobody   (65534)      682 2024-04-12 08:57:31.000000 geniac-3.3.0/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) nobody   (65534)    12181 2024-04-12 08:57:31.000000 geniac-3.3.0/CHANGELOG
+-rw-rw-rw-   0 root         (0) nobody   (65534)     4555 2024-04-12 08:57:31.000000 geniac-3.3.0/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) nobody   (65534)     2567 2024-04-12 08:57:31.000000 geniac-3.3.0/INSTALL.md
+-rw-rw-rw-   0 root         (0) nobody   (65534)    21778 2024-04-12 08:57:31.000000 geniac-3.3.0/LICENSE
+-rw-r--r--   0 root         (0) nobody   (65534)    36695 2024-04-12 09:07:35.991356 geniac-3.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) nobody   (65534)     1532 2024-04-12 08:57:31.000000 geniac-3.3.0/README.md
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:34.485122 geniac-3.3.0/cmake/
+-rw-rw-rw-   0 root         (0) nobody   (65534)     2824 2024-04-12 08:57:31.000000 geniac-3.3.0/cmake/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) nobody   (65534)     2780 2024-04-12 08:57:31.000000 geniac-3.3.0/cmake/FindApptainer.cmake
+-rw-rw-rw-   0 root         (0) nobody   (65534)     2683 2024-04-12 08:57:31.000000 geniac-3.3.0/cmake/FindDocker.cmake
+-rw-rw-rw-   0 root         (0) nobody   (65534)     2834 2024-04-12 08:57:31.000000 geniac-3.3.0/cmake/FindNextflow.cmake
+-rw-rw-rw-   0 root         (0) nobody   (65534)     2683 2024-04-12 08:57:31.000000 geniac-3.3.0/cmake/FindPodman.cmake
+-rw-rw-rw-   0 root         (0) nobody   (65534)     2994 2024-04-12 08:57:31.000000 geniac-3.3.0/cmake/FindSingularity.cmake
+-rw-rw-rw-   0 root         (0) nobody   (65534)     2082 2024-04-12 08:57:31.000000 geniac-3.3.0/cmake/checkConfigFiles.cmake
+-rw-rw-rw-   0 root         (0) nobody   (65534)     1099 2024-04-12 08:57:31.000000 geniac-3.3.0/cmake/createPathDirectories.cmake
+-rw-rw-rw-   0 root         (0) nobody   (65534)     1987 2024-04-12 08:57:31.000000 geniac-3.3.0/cmake/createWorkDir.cmake
+-rw-rw-rw-   0 root         (0) nobody   (65534)     2086 2024-04-12 08:57:31.000000 geniac-3.3.0/cmake/functionColorMessage.cmake
+-rw-rw-rw-   0 root         (0) nobody   (65534)     1293 2024-04-12 08:57:31.000000 geniac-3.3.0/cmake/initCmakePreload.sh
+-rw-rw-rw-   0 root         (0) nobody   (65534)     2136 2024-04-12 08:57:31.000000 geniac-3.3.0/cmake/stepAddTestTargets.cmake
+-rw-rw-rw-   0 root         (0) nobody   (65534)     5530 2024-04-12 08:57:31.000000 geniac-3.3.0/cmake/stepCheckOptions.cmake
+-rw-rw-rw-   0 root         (0) nobody   (65534)     2310 2024-04-12 08:57:31.000000 geniac-3.3.0/cmake/stepFindPackages.cmake
+-rw-rw-rw-   0 root         (0) nobody   (65534)     4031 2024-04-12 08:57:31.000000 geniac-3.3.0/cmake/stepGitInfo.cmake
+-rw-rw-rw-   0 root         (0) nobody   (65534)    16624 2024-04-12 08:57:31.000000 geniac-3.3.0/cmake/stepMainCoreScript.cmake
+-rw-rw-rw-   0 root         (0) nobody   (65534)     5651 2024-04-12 08:57:31.000000 geniac-3.3.0/cmake/stepSetVariables.cmake
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:34.521160 geniac-3.3.0/data/
+-rw-rw-rw-   0 root         (0) nobody   (65534)     4052 2024-04-12 08:57:31.000000 geniac-3.3.0/data/CMakeLists.txt
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:34.658049 geniac-3.3.0/data/conf/
+-rw-rw-rw-   0 root         (0) nobody   (65534)      228 2024-04-12 08:57:31.000000 geniac-3.3.0/data/conf/cluster.config
+-rw-rw-rw-   0 root         (0) nobody   (65534)      593 2024-04-12 08:57:31.000000 geniac-3.3.0/data/conf/conda.config
+-rw-rw-rw-   0 root         (0) nobody   (65534)      590 2024-04-12 08:57:31.000000 geniac-3.3.0/data/conf/docker.config
+-rw-rw-rw-   0 root         (0) nobody   (65534)     2497 2024-04-12 08:57:31.000000 geniac-3.3.0/data/conf/geniac.config
+-rw-rw-rw-   0 root         (0) nobody   (65534)      431 2024-04-12 08:57:31.000000 geniac-3.3.0/data/conf/genomes.config
+-rw-rw-rw-   0 root         (0) nobody   (65534)      606 2024-04-12 08:57:31.000000 geniac-3.3.0/data/conf/multiconda.config
+-rw-rw-rw-   0 root         (0) nobody   (65534)     1468 2024-04-12 08:57:31.000000 geniac-3.3.0/data/conf/multipath.config
+-rw-rw-rw-   0 root         (0) nobody   (65534)      807 2024-04-12 08:57:31.000000 geniac-3.3.0/data/conf/path.config
+-rw-rw-rw-   0 root         (0) nobody   (65534)      590 2024-04-12 08:57:31.000000 geniac-3.3.0/data/conf/podman.config
+-rw-rw-rw-   0 root         (0) nobody   (65534)     1676 2024-04-12 08:57:31.000000 geniac-3.3.0/data/conf/singularity.config
+-rw-rw-rw-   0 root         (0) nobody   (65534)     2639 2024-04-12 08:57:31.000000 geniac-3.3.0/data/createSubmodule.bash
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:33.585498 geniac-3.3.0/data/modules/
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:34.669999 geniac-3.3.0/data/modules/fromSource/
+-rw-rw-rw-   0 root         (0) nobody   (65534)     1943 2024-04-12 08:57:31.000000 geniac-3.3.0/data/modules/fromSource/CMakeLists.txt
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:33.592895 geniac-3.3.0/data/nf-modules/
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:33.595823 geniac-3.3.0/data/nf-modules/local/
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:34.686194 geniac-3.3.0/data/nf-modules/local/process/
+-rw-rw-rw-   0 root         (0) nobody   (65534)     2013 2024-04-12 08:57:31.000000 geniac-3.3.0/data/nf-modules/local/process/renvInit.nf
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:33.611209 geniac-3.3.0/data/recipes/
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:33.604770 geniac-3.3.0/data/recipes/dependencies/
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:34.700057 geniac-3.3.0/data/recipes/dependencies/renvGlad/
+-rw-rw-rw-   0 root         (0) nobody   (65534)     1875 2024-04-12 08:57:31.000000 geniac-3.3.0/data/recipes/dependencies/renvGlad/renv.lock
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:34.713030 geniac-3.3.0/data/recipes/docker/
+-rw-rw-rw-   0 root         (0) nobody   (65534)     1261 2024-04-12 08:57:31.000000 geniac-3.3.0/data/recipes/docker/r.Dockerfile
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:34.731879 geniac-3.3.0/data/recipes/singularity/
+-rw-rw-rw-   0 root         (0) nobody   (65534)     1241 2024-04-12 08:57:31.000000 geniac-3.3.0/data/recipes/singularity/r.def
+-rw-rw-rw-   0 root         (0) nobody   (65534)     3818 2024-04-12 08:57:31.000000 geniac-3.3.0/data/useCases.bash
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:35.036818 geniac-3.3.0/docs/
+-rw-rw-rw-   0 root         (0) nobody   (65534)     1180 2024-04-12 08:57:31.000000 geniac-3.3.0/docs/Makefile
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:35.049967 geniac-3.3.0/docs/_static/
+-rw-rw-rw-   0 root         (0) nobody   (65534)       18 2024-04-12 08:57:31.000000 geniac-3.3.0/docs/_static/.gitignore
+-rw-rw-rw-   0 root         (0) nobody   (65534)     4148 2024-04-12 08:57:31.000000 geniac-3.3.0/docs/admin.rst
+-rw-rw-rw-   0 root         (0) nobody   (65534)      321 2024-04-12 08:57:31.000000 geniac-3.3.0/docs/check.rst
+-rw-rw-rw-   0 root         (0) nobody   (65534)     3977 2024-04-12 08:57:31.000000 geniac-3.3.0/docs/cli.rst
+-rw-rw-rw-   0 root         (0) nobody   (65534)    14575 2024-04-12 08:57:31.000000 geniac-3.3.0/docs/conda.rst
+-rw-rw-rw-   0 root         (0) nobody   (65534)     5327 2024-04-12 08:57:31.000000 geniac-3.3.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) nobody   (65534)     4540 2024-04-12 08:57:31.000000 geniac-3.3.0/docs/customcmd.rst
+-rw-rw-rw-   0 root         (0) nobody   (65534)     6257 2024-04-12 08:57:31.000000 geniac-3.3.0/docs/devcycle.rst
+-rw-rw-rw-   0 root         (0) nobody   (65534)     1678 2024-04-12 08:57:31.000000 geniac-3.3.0/docs/environment.yml
+-rw-rw-rw-   0 root         (0) nobody   (65534)    18295 2024-04-12 08:57:31.000000 geniac-3.3.0/docs/faq.rst
+-rw-rw-rw-   0 root         (0) nobody   (65534)     8034 2024-04-12 08:57:31.000000 geniac-3.3.0/docs/from-source-examples.rst
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:35.205513 geniac-3.3.0/docs/images/
+-rw-rw-rw-   0 root         (0) nobody   (65534)   102057 2024-04-12 08:57:31.000000 geniac-3.3.0/docs/images/bash-startup.png
+-rw-rw-rw-   0 root         (0) nobody   (65534)   184337 2024-04-12 08:57:31.000000 geniac-3.3.0/docs/images/geniac-cli-uml.png
+-rw-rw-rw-   0 root         (0) nobody   (65534)    10972 2024-04-12 08:57:31.000000 geniac-3.3.0/docs/images/geniac-logo.png
+-rw-rw-rw-   0 root         (0) nobody   (65534)     7514 2024-04-12 08:57:31.000000 geniac-3.3.0/docs/images/geniac-logo.svg
+-rw-rw-rw-   0 root         (0) nobody   (65534)    12102 2024-04-12 08:57:31.000000 geniac-3.3.0/docs/images/geniac.uml
+-rw-rw-rw-   0 root         (0) nobody   (65534)    50235 2024-04-12 08:57:31.000000 geniac-3.3.0/docs/images/git-workflow.png
+-rw-rw-rw-   0 root         (0) nobody   (65534)    24741 2024-04-12 08:57:31.000000 geniac-3.3.0/docs/images/git-workflow.svg
+-rw-rw-rw-   0 root         (0) nobody   (65534)      127 2024-04-12 08:57:31.000000 geniac-3.3.0/docs/images/image-source.txt
+-rw-rw-rw-   0 root         (0) nobody   (65534)    22607 2024-04-12 08:57:32.000000 geniac-3.3.0/docs/images/install.png
+-rw-rw-rw-   0 root         (0) nobody   (65534)     9413 2024-04-12 08:57:32.000000 geniac-3.3.0/docs/images/installed.png
+-rw-rw-rw-   0 root         (0) nobody   (65534)     7719 2024-04-12 08:57:32.000000 geniac-3.3.0/docs/images/path.png
+-rw-rw-rw-   0 root         (0) nobody   (65534)      536 2024-04-12 08:57:32.000000 geniac-3.3.0/docs/index.rst
+-rw-rw-rw-   0 root         (0) nobody   (65534)    16976 2024-04-12 08:57:32.000000 geniac-3.3.0/docs/install.rst
+-rw-rw-rw-   0 root         (0) nobody   (65534)     4000 2024-04-12 08:57:32.000000 geniac-3.3.0/docs/intro.rst
+-rw-rw-rw-   0 root         (0) nobody   (65534)      646 2024-04-12 08:57:32.000000 geniac-3.3.0/docs/linux.rst
+-rw-rw-rw-   0 root         (0) nobody   (65534)      133 2024-04-12 08:57:32.000000 geniac-3.3.0/docs/misc.rst
+-rw-rw-rw-   0 root         (0) nobody   (65534)     3365 2024-04-12 08:57:32.000000 geniac-3.3.0/docs/overview.rst
+-rw-rw-rw-   0 root         (0) nobody   (65534)    24883 2024-04-12 08:57:32.000000 geniac-3.3.0/docs/process.rst
+-rw-rw-rw-   0 root         (0) nobody   (65534)     1381 2024-04-12 08:57:32.000000 geniac-3.3.0/docs/profiles.rst
+-rw-rw-rw-   0 root         (0) nobody   (65534)     4641 2024-04-12 08:57:32.000000 geniac-3.3.0/docs/renv.rst
+-rw-rw-rw-   0 root         (0) nobody   (65534)      349 2024-04-12 08:57:32.000000 geniac-3.3.0/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) nobody   (65534)    15909 2024-04-12 08:57:32.000000 geniac-3.3.0/docs/run.rst
+-rw-rw-rw-   0 root         (0) nobody   (65534)     2849 2024-04-12 08:57:32.000000 geniac-3.3.0/docs/substitutions.rst
+-rw-rw-rw-   0 root         (0) nobody   (65534)      722 2024-04-12 08:57:32.000000 geniac-3.3.0/environment.yml
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:35.267988 geniac-3.3.0/install/
+-rw-rw-rw-   0 root         (0) nobody   (65534)     1371 2024-04-12 08:57:32.000000 geniac-3.3.0/install/cmake-init-default.cmake
+-rw-rw-rw-   0 root         (0) nobody   (65534)    16595 2024-04-12 08:57:32.000000 geniac-3.3.0/install/docker.nf
+-rw-rw-rw-   0 root         (0) nobody   (65534)     2126 2024-04-12 08:57:32.000000 geniac-3.3.0/install/nextflow.config.in
+-rw-rw-rw-   0 root         (0) nobody   (65534)    34355 2024-04-12 08:57:32.000000 geniac-3.3.0/install/singularity.nf
+-rw-rw-rw-   0 root         (0) nobody   (65534)      311 2024-04-12 08:57:32.000000 geniac-3.3.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) nobody   (65534)     2033 2024-04-12 09:07:36.006604 geniac-3.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) nobody   (65534)      703 2024-04-12 08:57:32.000000 geniac-3.3.0/setup.py
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:33.631388 geniac-3.3.0/src/
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:35.281749 geniac-3.3.0/src/geniac/
+-rw-rw-rw-   0 root         (0) nobody   (65534)      392 2024-04-12 08:57:32.000000 geniac-3.3.0/src/geniac/__init__.py
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:35.399582 geniac-3.3.0/src/geniac/cli/
+-rw-rw-rw-   0 root         (0) nobody   (65534)       46 2024-04-12 08:57:32.000000 geniac-3.3.0/src/geniac/cli/__init__.py
+-rw-rw-rw-   0 root         (0) nobody   (65534)    15278 2024-04-12 08:57:32.000000 geniac-3.3.0/src/geniac/cli/__main__.py
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:35.542552 geniac-3.3.0/src/geniac/cli/commands/
+-rw-rw-rw-   0 root         (0) nobody   (65534)       77 2024-04-12 08:57:32.000000 geniac-3.3.0/src/geniac/cli/commands/__init__.py
+-rw-rw-rw-   0 root         (0) nobody   (65534)     2668 2024-04-12 08:57:32.000000 geniac-3.3.0/src/geniac/cli/commands/base.py
+-rw-rw-rw-   0 root         (0) nobody   (65534)     1057 2024-04-12 08:57:32.000000 geniac-3.3.0/src/geniac/cli/commands/clean.py
+-rw-rw-rw-   0 root         (0) nobody   (65534)     2209 2024-04-12 08:57:32.000000 geniac-3.3.0/src/geniac/cli/commands/configs.py
+-rw-rw-rw-   0 root         (0) nobody   (65534)     2436 2024-04-12 08:57:32.000000 geniac-3.3.0/src/geniac/cli/commands/init.py
+-rw-rw-rw-   0 root         (0) nobody   (65534)    10068 2024-04-12 08:57:32.000000 geniac-3.3.0/src/geniac/cli/commands/install.py
+-rw-rw-rw-   0 root         (0) nobody   (65534)    66083 2024-04-12 08:57:32.000000 geniac-3.3.0/src/geniac/cli/commands/lint.py
+-rw-rw-rw-   0 root         (0) nobody   (65534)     2354 2024-04-12 08:57:32.000000 geniac-3.3.0/src/geniac/cli/commands/options.py
+-rw-rw-rw-   0 root         (0) nobody   (65534)     2723 2024-04-12 08:57:32.000000 geniac-3.3.0/src/geniac/cli/commands/recipes.py
+-rw-rw-rw-   0 root         (0) nobody   (65534)     1454 2024-04-12 08:57:32.000000 geniac-3.3.0/src/geniac/cli/commands/test.py
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:33.647896 geniac-3.3.0/src/geniac/cli/data/
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:35.578367 geniac-3.3.0/src/geniac/cli/data/conf/
+-rw-rw-rw-   0 root         (0) nobody   (65534)    16475 2024-04-12 08:57:32.000000 geniac-3.3.0/src/geniac/cli/data/conf/geniac.ini
+-rw-rw-rw-   0 root         (0) nobody   (65534)     1709 2024-04-12 08:57:32.000000 geniac-3.3.0/src/geniac/cli/data/conf/logging.json
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:35.595696 geniac-3.3.0/src/geniac/cli/data/scripts/
+-rw-rw-rw-   0 root         (0) nobody   (65534)     7387 2024-04-12 08:57:32.000000 geniac-3.3.0/src/geniac/cli/data/scripts/geniac.bash
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:35.647774 geniac-3.3.0/src/geniac/cli/parsers/
+-rw-rw-rw-   0 root         (0) nobody   (65534)       76 2024-04-12 08:57:32.000000 geniac-3.3.0/src/geniac/cli/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) nobody   (65534)     5747 2024-04-12 08:57:32.000000 geniac-3.3.0/src/geniac/cli/parsers/base.py
+-rw-rw-rw-   0 root         (0) nobody   (65534)    15057 2024-04-12 08:57:32.000000 geniac-3.3.0/src/geniac/cli/parsers/config.py
+-rw-rw-rw-   0 root         (0) nobody   (65534)     6596 2024-04-12 08:57:32.000000 geniac-3.3.0/src/geniac/cli/parsers/scripts.py
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:35.683588 geniac-3.3.0/src/geniac/cli/utils/
+-rw-rw-rw-   0 root         (0) nobody   (65534)       74 2024-04-12 08:57:32.000000 geniac-3.3.0/src/geniac/cli/utils/__init__.py
+-rw-rw-rw-   0 root         (0) nobody   (65534)    25129 2024-04-12 08:57:32.000000 geniac-3.3.0/src/geniac/cli/utils/base.py
+-rw-rw-rw-   0 root         (0) nobody   (65534)     1919 2024-04-12 08:57:32.000000 geniac-3.3.0/src/geniac/cli/utils/logging.py
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:35.976618 geniac-3.3.0/src/geniac.egg-info/
+-rw-r--r--   0 root         (0) nobody   (65534)    36695 2024-04-12 09:07:33.000000 geniac-3.3.0/src/geniac.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) nobody   (65534)     3993 2024-04-12 09:07:33.000000 geniac-3.3.0/src/geniac.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) nobody   (65534)        1 2024-04-12 09:07:33.000000 geniac-3.3.0/src/geniac.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) nobody   (65534)       52 2024-04-12 09:07:33.000000 geniac-3.3.0/src/geniac.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) nobody   (65534)        1 2024-04-12 09:07:32.000000 geniac-3.3.0/src/geniac.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) nobody   (65534)      188 2024-04-12 09:07:33.000000 geniac-3.3.0/src/geniac.egg-info/requires.txt
+-rw-r--r--   0 root         (0) nobody   (65534)        7 2024-04-12 09:07:33.000000 geniac-3.3.0/src/geniac.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:35.750099 geniac-3.3.0/tests/
+-rw-rw-rw-   0 root         (0) nobody   (65534)       77 2024-04-12 08:57:32.000000 geniac-3.3.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) nobody   (65534)      322 2024-04-12 08:57:32.000000 geniac-3.3.0/tests/conftest.py
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:35.776405 geniac-3.3.0/tests/data/
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:35.927727 geniac-3.3.0/tests/data/conf/
+-rw-rw-rw-   0 root         (0) nobody   (65534)      254 2024-04-12 08:57:32.000000 geniac-3.3.0/tests/data/conf/README.md
+-rw-rw-rw-   0 root         (0) nobody   (65534)      394 2024-04-12 08:57:32.000000 geniac-3.3.0/tests/data/conf/base.config
+-rwxrwxrwx   0 root         (0) nobody   (65534)      226 2024-04-12 08:57:32.000000 geniac-3.3.0/tests/data/conf/cluster.config
+-rw-rw-rw-   0 root         (0) nobody   (65534)      252 2024-04-12 08:57:32.000000 geniac-3.3.0/tests/data/conf/conda.config
+-rw-rw-rw-   0 root         (0) nobody   (65534)      287 2024-04-12 08:57:32.000000 geniac-3.3.0/tests/data/conf/docker.config
+-rw-rw-rw-   0 root         (0) nobody   (65534)     1155 2024-04-12 08:57:32.000000 geniac-3.3.0/tests/data/conf/geniac.config
+-rw-rw-rw-   0 root         (0) nobody   (65534)      430 2024-04-12 08:57:32.000000 geniac-3.3.0/tests/data/conf/genomes.config
+-rw-rw-rw-   0 root         (0) nobody   (65534)      253 2024-04-12 08:57:32.000000 geniac-3.3.0/tests/data/conf/multiconda.config
+-rw-rw-rw-   0 root         (0) nobody   (65534)     1064 2024-04-12 08:57:32.000000 geniac-3.3.0/tests/data/conf/multipath.config
+-rw-rw-rw-   0 root         (0) nobody   (65534)      808 2024-04-12 08:57:32.000000 geniac-3.3.0/tests/data/conf/path.config
+-rw-rw-rw-   0 root         (0) nobody   (65534)     3692 2024-04-12 08:57:32.000000 geniac-3.3.0/tests/data/conf/process.config
+-rw-rw-rw-   0 root         (0) nobody   (65534)     1259 2024-04-12 08:57:32.000000 geniac-3.3.0/tests/data/conf/singularity.config
+-rw-rw-rw-   0 root         (0) nobody   (65534)      797 2024-04-12 08:57:32.000000 geniac-3.3.0/tests/data/conf/test.config
+-rw-rw-rw-   0 root         (0) nobody   (65534)    15327 2024-04-12 08:57:32.000000 geniac-3.3.0/tests/data/main.nf
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:33.671318 geniac-3.3.0/tests/data/modules/
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:35.940411 geniac-3.3.0/tests/data/modules/fromSource/
+-rw-rw-rw-   0 root         (0) nobody   (65534)        0 2024-04-12 08:57:32.000000 geniac-3.3.0/tests/data/modules/fromSource/CMakeLists.txt
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:35.951371 geniac-3.3.0/tests/data/modules/fromSource/dolorSit/
+-rw-rw-rw-   0 root         (0) nobody   (65534)        0 2024-04-12 08:57:32.000000 geniac-3.3.0/tests/data/modules/fromSource/dolorSit/CMakeLists.txt
+drwxr-xr-x   0 root         (0) nobody   (65534)        0 2024-04-12 09:07:35.964478 geniac-3.3.0/tests/data/modules/fromSource/helloWorld/
+-rw-rw-rw-   0 root         (0) nobody   (65534)        0 2024-04-12 08:57:32.000000 geniac-3.3.0/tests/data/modules/fromSource/helloWorld/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) nobody   (65534)     1689 2024-04-12 08:57:32.000000 geniac-3.3.0/tests/data/nextflow.config
+-rw-rw-rw-   0 root         (0) nobody   (65534)     1646 2024-04-12 08:57:32.000000 geniac-3.3.0/tests/test_base.py
+-rw-rw-rw-   0 root         (0) nobody   (65534)      595 2024-04-12 08:57:32.000000 geniac-3.3.0/tests/test_commands_lint.py
+-rw-rw-rw-   0 root         (0) nobody   (65534)      280 2024-04-12 08:57:32.000000 geniac-3.3.0/tests/test_main.py
+-rw-rw-rw-   0 root         (0) nobody   (65534)     1852 2024-04-12 08:57:32.000000 geniac-3.3.0/tox.ini
```

### Comparing `geniac-3.2.1/.coveragerc` & `geniac-3.3.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/.gitignore` & `geniac-3.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/.gitlab-ci.yml` & `geniac-3.3.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/.pre-commit-config.yaml` & `geniac-3.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/.readthedocs.yml` & `geniac-3.3.0/.readthedocs.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # Read the Docs configuration file
 # See https://docs.readthedocs.io/en/stable/config-file/v2.html for details
 
 # Required
 version: 2
+# Set the OS, Python version and other tools you might need
+
+build:
+  os: "ubuntu-22.04"
+  tools:
+    python: "mambaforge-22.9"
 
 # Build documentation in the docs/ directory with Sphinx
 sphinx:
   configuration: docs/conf.py
 
 conda:
   environment: docs/environment.yml
```

### Comparing `geniac-3.2.1/CHANGELOG` & `geniac-3.3.0/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+version-3.3.0
+04/12/2024
+
+NEW FEATURES
+   - almalinux:9.3 set as default for the containers
+   - conda 23.10.0 set as default for the containers
+
+BUGFIX
+   - singularity/docker recipes: post command were printed twice.
+
+DOCUMENTATION
+   - Update readthedocs config file
+
 version-3.2.1
 10/12/2023
 
 BUGFIX
    - singularity/docker profiles:
      * post commands were written twice in the recipes generated by geniac
 
@@ -17,15 +30,15 @@
       * Update conda env with new tool versions
 
 version-3.1.0
 08/14/2023
 
 NEW FEATURES
    - almalinux:8.8 set as default for the containers
-   - conda 25.3.1 set as default for the containers
+   - conda 23.5.1 set as default for the containers
    - micromamba is used to create conda envs and install conda packages
    - conda/multiconda profiles:
 	 * conda.enable has been added
    - Geniac CLI:
       *  Conda env with apptainer 1.2.2, nextflow 22.10.6, pip 23.2.1
 
 DOCUMENTATION
```

### Comparing `geniac-3.2.1/CMakeLists.txt` & `geniac-3.3.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/INSTALL.md` & `geniac-3.3.0/INSTALL.md`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/LICENSE` & `geniac-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/PKG-INFO` & `geniac-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geniac
-Version: 3.2.1
+Version: 3.3.0
 Summary: Automatic Configuration GENerator and Installer for nextflow pipeline
 Home-page: https://gitlab.curie.fr/bioinfo-guidelines/geniac
 Author: Philippe Hupé, Julien Roméjon, Fabrice Allain
 Author-email: philippe.hupe@curie.fr
 License: CeCILL
 Project-URL: Documentation, https://geniac.readthedocs.io/en/latest/
 Project-URL: Demonstration, https://github.com/bioinfo-pf-curie/geniac-demo.git
@@ -52,14 +52,27 @@
 * [Centre national de la recherche scientifique](http://www.cnrs.fr)
 * This project has received funding from the European Union’s Horizon 2020 research and innovation programme and the Canadian Institutes of Health Research under the grant agreement No 825835 in the framework on the [European-Canadian Cancer Network](https://eucancan.com/)
 
 ## Citation
 
 [Allain F, Roméjon J, La Rosa P et al. Geniac: Automatic Configuration GENerator and Installer for nextflow pipelines. Open Research Europe 2021, 1:76](https://open-research-europe.ec.europa.eu/articles/1-76)
 
+version-3.3.0
+04/12/2024
+
+NEW FEATURES
+   - almalinux:9.3 set as default for the containers
+   - conda 23.10.0 set as default for the containers
+
+BUGFIX
+   - singularity/docker recipes: post command were printed twice.
+
+DOCUMENTATION
+   - Update readthedocs config file
+
 version-3.2.1
 10/12/2023
 
 BUGFIX
    - singularity/docker profiles:
      * post commands were written twice in the recipes generated by geniac
 
@@ -75,15 +88,15 @@
       * Update conda env with new tool versions
 
 version-3.1.0
 08/14/2023
 
 NEW FEATURES
    - almalinux:8.8 set as default for the containers
-   - conda 25.3.1 set as default for the containers
+   - conda 23.5.1 set as default for the containers
    - micromamba is used to create conda envs and install conda packages
    - conda/multiconda profiles:
 	 * conda.enable has been added
    - Geniac CLI:
       *  Conda env with apptainer 1.2.2, nextflow 22.10.6, pip 23.2.1
 
 DOCUMENTATION
```

### Comparing `geniac-3.2.1/README.md` & `geniac-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/cmake/CMakeLists.txt` & `geniac-3.3.0/cmake/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/cmake/FindApptainer.cmake` & `geniac-3.3.0/cmake/FindApptainer.cmake`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/cmake/FindDocker.cmake` & `geniac-3.3.0/cmake/FindDocker.cmake`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/cmake/FindNextflow.cmake` & `geniac-3.3.0/cmake/FindNextflow.cmake`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/cmake/FindPodman.cmake` & `geniac-3.3.0/cmake/FindPodman.cmake`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/cmake/FindSingularity.cmake` & `geniac-3.3.0/cmake/FindSingularity.cmake`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/cmake/checkConfigFiles.cmake` & `geniac-3.3.0/cmake/checkConfigFiles.cmake`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/cmake/createPathDirectories.cmake` & `geniac-3.3.0/cmake/createPathDirectories.cmake`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/cmake/createWorkDir.cmake` & `geniac-3.3.0/cmake/createWorkDir.cmake`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/cmake/functionColorMessage.cmake` & `geniac-3.3.0/cmake/functionColorMessage.cmake`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/cmake/initCmakePreload.sh` & `geniac-3.3.0/cmake/initCmakePreload.sh`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/cmake/stepAddTestTargets.cmake` & `geniac-3.3.0/cmake/stepAddTestTargets.cmake`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/cmake/stepCheckOptions.cmake` & `geniac-3.3.0/cmake/stepCheckOptions.cmake`

 * *Files 0% similar despite different names*

```diff
@@ -155,9 +155,9 @@
 if(NOT "${ap_docker_registry}" STREQUAL "")
   if(NOT "${ap_docker_registry}" MATCHES ".*/")
     message_color(ERROR "ap_docker_registry '${ap_docker_registry}' must end with '/'")
   endif()
 endif()
   
 if(NOT "${ap_linux_distro}" MATCHES ".*:.*")
-  message_color(ERROR "ap_linux_distro '${ap_linux_distro}' must be formatted like 'distro:version' (e.g. almalinux:8.4).")
+  message_color(ERROR "ap_linux_distro '${ap_linux_distro}' must be formatted like 'distro:version' (e.g. almalinux:9.3).")
 endif()
```

### Comparing `geniac-3.2.1/cmake/stepFindPackages.cmake` & `geniac-3.3.0/cmake/stepFindPackages.cmake`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/cmake/stepGitInfo.cmake` & `geniac-3.3.0/cmake/stepGitInfo.cmake`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/cmake/stepMainCoreScript.cmake` & `geniac-3.3.0/cmake/stepMainCoreScript.cmake`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/cmake/stepSetVariables.cmake` & `geniac-3.3.0/cmake/stepSetVariables.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -81,25 +81,25 @@
     "4geniac/"
     CACHE
         STRING
   "Docker registry used to build the containers from recipes automatically generated by geniac. Default is 4geniac/ (see https://hub.docker.com/u/4geniac and https://github.com/bioinfo-pf-curie/4geniac)."
 )
 
 set(ap_linux_distro
-    "almalinux:8.8"
+    "almalinux:9.3"
     CACHE
         STRING
-        "When building the docker/singularity images, geniac bootstraps from docker containers available on the docker hub registry https://hub.docker.com/u/4geniac. This variable defines which Linux distro (i.e. which repository) and which version (i.e. which tag) to use from https://hub.docker.com/u/4geniac. For details, about the docker containers see https://github.com/bioinfo-pf-curie/4geniac. Default is almalinux:8.8."
+        "When building the docker/singularity images, geniac bootstraps from docker containers available on the docker hub registry https://hub.docker.com/u/4geniac. This variable defines which Linux distro (i.e. which repository) and which version (i.e. which tag) to use from https://hub.docker.com/u/4geniac. For details, about the docker containers see https://github.com/bioinfo-pf-curie/4geniac. Default is almalinux:9.3."
 )
 
 set(ap_conda_release
-    "py311_23.5.1-0"
+    "py311_23.10.0-1"
     CACHE
         STRING
-        "When building the docker/singularity images, geniac bootstraps from docker containers available on the docker hub registry https://hub.docker.com/u/4geniac. When a tool is installed with Conda, the container obviously needs Conda. Therefore, this variable defines which Conda release to use from https://hub.docker.com/u/4geniac. For details, about the docker containers see https://github.com/bioinfo-pf-curie/4geniac. Default is py311_23.5.1-0."
+        "When building the docker/singularity images, geniac bootstraps from docker containers available on the docker hub registry https://hub.docker.com/u/4geniac. When a tool is installed with Conda, the container obviously needs Conda. Therefore, this variable defines which Conda release to use from https://hub.docker.com/u/4geniac. For details, about the docker containers see https://github.com/bioinfo-pf-curie/4geniac. Default is py311_23.10.0-1."
 )
 
 set(ap_mount_dir
     ""
     CACHE
         STRING
         "Option is deprecated."
```

### Comparing `geniac-3.2.1/data/CMakeLists.txt` & `geniac-3.3.0/data/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/data/conf/conda.config` & `geniac-3.3.0/data/conf/conda.config`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/data/conf/docker.config` & `geniac-3.3.0/data/conf/docker.config`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/data/conf/geniac.config` & `geniac-3.3.0/data/conf/geniac.config`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/data/conf/multiconda.config` & `geniac-3.3.0/data/conf/multiconda.config`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/data/conf/multipath.config` & `geniac-3.3.0/data/conf/multipath.config`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/data/conf/path.config` & `geniac-3.3.0/data/conf/path.config`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/data/conf/podman.config` & `geniac-3.3.0/data/conf/podman.config`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/data/conf/singularity.config` & `geniac-3.3.0/data/conf/singularity.config`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/data/createSubmodule.bash` & `geniac-3.3.0/data/createSubmodule.bash`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/data/modules/fromSource/CMakeLists.txt` & `geniac-3.3.0/data/modules/fromSource/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/data/nf-modules/local/process/renvInit.nf` & `geniac-3.3.0/data/nf-modules/local/process/renvInit.nf`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/data/recipes/dependencies/renvGlad/renv.lock` & `geniac-3.3.0/data/recipes/dependencies/renvGlad/renv.lock`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/data/recipes/docker/r.Dockerfile` & `geniac-3.3.0/data/recipes/docker/r.Dockerfile`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/data/recipes/singularity/r.def` & `geniac-3.3.0/data/recipes/singularity/r.def`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/data/useCases.bash` & `geniac-3.3.0/data/useCases.bash`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/docs/Makefile` & `geniac-3.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/docs/admin.rst` & `geniac-3.3.0/docs/admin.rst`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/docs/cli.rst` & `geniac-3.3.0/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/docs/conda.rst` & `geniac-3.3.0/docs/conda.rst`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 -----------------------------------------------------------------
 
 Let's consider you run ``singularity build myTool.sif myTool.def`` from this ``myTool.def`` Definition file:
 
 ::
 
    Bootstrap: docker
-   From: 4geniac/almalinux:8.8_conda-py311_23.5.1-0
+   From: 4geniac/almalinux:9.3_conda-py311_23.10.0-1
    
    %environment
        export LC_ALL=en_US.utf-8
        export LANG=en_US.utf-8
    
    %post
        mkdir -p /opt/etc
@@ -127,15 +127,15 @@
 ------------------------------------------------------------------------------------
 
 From the Definition file used in :ref:`conda-singularity-impossible`, add ``export BASH_ENV=/opt/etc/bashrc`` in the section ``%environment``. The ``myTool.def`` Definition file is now:
 
 ::
 
    Bootstrap: docker
-   From: 4geniac/almalinux:8.8_conda-py311_23.5.1-0
+   From: 4geniac/almalinux:9.3_conda-py311_23.10.0-1
    
    %environment
        export LC_ALL=en_US.utf-8
        export LANG=en_US.utf-8
        export BASH_ENV=/opt/etc/bashrc
    
    %post
@@ -189,15 +189,15 @@
 
 From the Definition file used in :ref:`conda-singularity-impossible`, add ``source /opt/etc/bashrc`` in the section ``%environment``. The ``myTool.def`` Definition file is now:
 
 
 ::
 
    Bootstrap: docker
-   From: 4geniac/almalinux:8.8_conda-py311_23.5.1-0
+   From: 4geniac/almalinux:9.3_conda-py311_23.10.0-1
    
    %environment
        export LC_ALL=en_US.utf-8
        export LANG=en_US.utf-8
        source /opt/etc/bashrc
    
    %post
@@ -251,15 +251,15 @@
 Example1
 --------
 
 Let's consider you run ``sudo docker build  -f myToolV0.Dockerfile -t mytool .`` from this ``myTool.Dockerfile``:
 
 ::
 
-   FROM 4geniac/almalinux:8.8_conda-py311_23.5.1-0
+   FROM 4geniac/almalinux:9.3_conda-py311_23.10.0-1
    
    # install conda env
    RUN yum install -y which \
    && yum clean all \
    && conda create -y -n myTool_env  \
    && echo -e "#! /bin/bash\n\n# script to activate the conda environment" > ~/.bashrc \
    && conda init bash \
@@ -298,15 +298,15 @@
 Example2
 --------
 
 Let's add ``ENV BASH_ENV ~/.bashrc`` in the Dockerfile and set the ``PS1`` variable (otherwise the shell will complain about unbound variable) as follows:
 
 ::
 
-   FROM 4geniac/almalinux:8.8_conda-py311_23.5.1-0
+   FROM 4geniac/almalinux:9.3_conda-py311_23.10.0-1
    
    # install conda env
    RUN yum install -y which \
    && yum clean all \
    && conda create -y -n myTool_env  \
    && echo -e "#! /bin/bash\n\n# script to activate the conda environment" > ~/.bashrc \
    && echo "export PS1='Docker> '" >> ~/.bashrc \
```

### Comparing `geniac-3.2.1/docs/conf.py` & `geniac-3.3.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 source_suffix = '.rst'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = u'geniac'
-copyright = u'2019-2023, Institut Curie'
+copyright = u'2019-2024, Institut Curie'
 author = u'Philippe Hupé'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
```

### Comparing `geniac-3.2.1/docs/customcmd.rst` & `geniac-3.3.0/docs/customcmd.rst`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
  
 
 The file ``recipes/singularity/fastqc.def`` which will be generated by geniac will be like this:
 
 ::
 
    Bootstrap: docker
-   From: 4geniac/almalinux:8.8_conda-py311_23.5.1-0
+   From: 4geniac/almalinux:9.3_conda-py311_23.10.0-1
    
    %labels
        gitUrl ssh://git@gitlab.curie.fr:2222/bioinfo-guidelines/geniac-demo.git
        gitCommit 35099a1c9ff4c1e038c9f67bf20a9750e36b78d3 / devel
    
    %environment
        export R_LIBS_USER="-"
@@ -92,15 +92,15 @@
 * ``params.geniac.containers.cmd.post`` will add the command in the ``RUN`` directive.
 * ``params.geniac.containers.cmd.envCustom``: will export the variables in the ``ENV`` directive.
 
 The file ``recipes/docker/fastqc.Dockerfile`` which will be generated by geniac will be like this:
 
 ::
 
-   FROM 4geniac/almalinux:8.8_conda-py311_23.5.1-0
+   FROM 4geniac/almalinux:9.3_conda-py311_23.10.0-1
    
    LABEL gitUrl="ssh://git@gitlab.curie.fr:2222/bioinfo-guidelines/geniac-demo.git"
    LABEL gitCommit="35099a1c9ff4c1e038c9f67bf20a9750e36b78d3 / devel"
    
    ENV R_LIBS_USER "-"
    ENV R_PROFILE_USER "-"
    ENV R_ENVIRON_USER "-"
```

### Comparing `geniac-3.2.1/docs/devcycle.rst` & `geniac-3.3.0/docs/devcycle.rst`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/docs/environment.yml` & `geniac-3.3.0/docs/environment.yml`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/docs/faq.rst` & `geniac-3.3.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/docs/from-source-examples.rst` & `geniac-3.3.0/docs/from-source-examples.rst`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/docs/images/bash-startup.png` & `geniac-3.3.0/docs/images/bash-startup.png`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/docs/images/geniac-cli-uml.png` & `geniac-3.3.0/docs/images/geniac-cli-uml.png`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/docs/images/geniac-logo.png` & `geniac-3.3.0/docs/images/geniac-logo.png`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/docs/images/geniac-logo.svg` & `geniac-3.3.0/docs/images/geniac-logo.svg`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/docs/images/geniac.uml` & `geniac-3.3.0/docs/images/geniac.uml`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/docs/images/git-workflow.png` & `geniac-3.3.0/docs/images/git-workflow.png`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/docs/images/git-workflow.svg` & `geniac-3.3.0/docs/images/git-workflow.svg`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/docs/images/install.png` & `geniac-3.3.0/docs/images/install.png`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/docs/images/installed.png` & `geniac-3.3.0/docs/images/installed.png`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/docs/images/path.png` & `geniac-3.3.0/docs/images/path.png`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/docs/index.rst` & `geniac-3.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/docs/install.rst` & `geniac-3.3.0/docs/install.rst`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 .. _install-ap_conda_release:
 
 ap_conda_release
 ++++++++++++++++
 
 | STRING
 | When building the docker/singularity images, geniac bootstraps from docker containers available on the docker hub registry |4geniac|_. When a tool is installed with Conda, the container obviously needs Conda. Therefore, this variable defines which Conda release to use from |4geniac|_. For details, about the docker containers see |4geniacgithub|_.
-| Default is ``py311_23.5.1-0``. See also options :ref:`install-ap_linux_distro` and :ref:`install-ap_docker_registry`.
+| Default is ``py311_23.10.0-1``. See also options :ref:`install-ap_linux_distro` and :ref:`install-ap_docker_registry`.
 
 .. _install-ap_docker_registry:
 
 ap_docker_registry
 ++++++++++++++++++
 
 | STRING
@@ -151,15 +151,15 @@
 .. _install-ap_linux_distro:
 
 ap_linux_distro
 +++++++++++++++
 
 | STRING
 | When building the docker/singularity images, geniac bootstraps from docker containers available on the docker hub registry |4geniac|_. This variable defines which Linux distro (i.e. which repository) and which version (i.e. which tag) to use from |4geniac|_. For details, about the docker containers see |4geniacgithub|_.
-| Default is ``almalinux:8.8``. See also options :ref:`install-ap_conda_release` and :ref:`install-ap_docker_registry`.
+| Default is ``almalinux:9.3``. See also options :ref:`install-ap_conda_release` and :ref:`install-ap_docker_registry`.
 
 .. _install-ap_mount_dir:
 
 ap_mount_dir
 ++++++++++++
 
 | Option is deprecated.
```

### Comparing `geniac-3.2.1/docs/intro.rst` & `geniac-3.3.0/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/docs/linux.rst` & `geniac-3.3.0/docs/linux.rst`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/docs/overview.rst` & `geniac-3.3.0/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/docs/process.rst` & `geniac-3.3.0/docs/process.rst`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/docs/profiles.rst` & `geniac-3.3.0/docs/profiles.rst`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/docs/renv.rst` & `geniac-3.3.0/docs/renv.rst`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/docs/run.rst` & `geniac-3.3.0/docs/run.rst`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/docs/substitutions.rst` & `geniac-3.3.0/docs/substitutions.rst`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/environment.yml` & `geniac-3.3.0/environment.yml`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/install/cmake-init-default.cmake` & `geniac-3.3.0/install/cmake-init-default.cmake`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/install/docker.nf` & `geniac-3.3.0/install/docker.nf`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/install/nextflow.config.in` & `geniac-3.3.0/install/nextflow.config.in`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/install/singularity.nf` & `geniac-3.3.0/install/singularity.nf`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/setup.cfg` & `geniac-3.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/setup.py` & `geniac-3.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/src/geniac/cli/__main__.py` & `geniac-3.3.0/src/geniac/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/src/geniac/cli/commands/base.py` & `geniac-3.3.0/src/geniac/cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/src/geniac/cli/commands/clean.py` & `geniac-3.3.0/src/geniac/cli/commands/clean.py`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/src/geniac/cli/commands/configs.py` & `geniac-3.3.0/src/geniac/cli/commands/configs.py`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/src/geniac/cli/commands/init.py` & `geniac-3.3.0/src/geniac/cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/src/geniac/cli/commands/install.py` & `geniac-3.3.0/src/geniac/cli/commands/install.py`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/src/geniac/cli/commands/lint.py` & `geniac-3.3.0/src/geniac/cli/commands/lint.py`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/src/geniac/cli/commands/options.py` & `geniac-3.3.0/src/geniac/cli/commands/options.py`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/src/geniac/cli/commands/recipes.py` & `geniac-3.3.0/src/geniac/cli/commands/recipes.py`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/src/geniac/cli/commands/test.py` & `geniac-3.3.0/src/geniac/cli/commands/test.py`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/src/geniac/cli/data/conf/geniac.ini` & `geniac-3.3.0/src/geniac/cli/data/conf/geniac.ini`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/src/geniac/cli/data/conf/logging.json` & `geniac-3.3.0/src/geniac/cli/data/conf/logging.json`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/src/geniac/cli/data/scripts/geniac.bash` & `geniac-3.3.0/src/geniac/cli/data/scripts/geniac.bash`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/src/geniac/cli/parsers/base.py` & `geniac-3.3.0/src/geniac/cli/parsers/base.py`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/src/geniac/cli/parsers/config.py` & `geniac-3.3.0/src/geniac/cli/parsers/config.py`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/src/geniac/cli/parsers/scripts.py` & `geniac-3.3.0/src/geniac/cli/parsers/scripts.py`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/src/geniac/cli/utils/base.py` & `geniac-3.3.0/src/geniac/cli/utils/base.py`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/src/geniac/cli/utils/logging.py` & `geniac-3.3.0/src/geniac/cli/utils/logging.py`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/src/geniac.egg-info/PKG-INFO` & `geniac-3.3.0/src/geniac.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geniac
-Version: 3.2.1
+Version: 3.3.0
 Summary: Automatic Configuration GENerator and Installer for nextflow pipeline
 Home-page: https://gitlab.curie.fr/bioinfo-guidelines/geniac
 Author: Philippe Hupé, Julien Roméjon, Fabrice Allain
 Author-email: philippe.hupe@curie.fr
 License: CeCILL
 Project-URL: Documentation, https://geniac.readthedocs.io/en/latest/
 Project-URL: Demonstration, https://github.com/bioinfo-pf-curie/geniac-demo.git
@@ -52,14 +52,27 @@
 * [Centre national de la recherche scientifique](http://www.cnrs.fr)
 * This project has received funding from the European Union’s Horizon 2020 research and innovation programme and the Canadian Institutes of Health Research under the grant agreement No 825835 in the framework on the [European-Canadian Cancer Network](https://eucancan.com/)
 
 ## Citation
 
 [Allain F, Roméjon J, La Rosa P et al. Geniac: Automatic Configuration GENerator and Installer for nextflow pipelines. Open Research Europe 2021, 1:76](https://open-research-europe.ec.europa.eu/articles/1-76)
 
+version-3.3.0
+04/12/2024
+
+NEW FEATURES
+   - almalinux:9.3 set as default for the containers
+   - conda 23.10.0 set as default for the containers
+
+BUGFIX
+   - singularity/docker recipes: post command were printed twice.
+
+DOCUMENTATION
+   - Update readthedocs config file
+
 version-3.2.1
 10/12/2023
 
 BUGFIX
    - singularity/docker profiles:
      * post commands were written twice in the recipes generated by geniac
 
@@ -75,15 +88,15 @@
       * Update conda env with new tool versions
 
 version-3.1.0
 08/14/2023
 
 NEW FEATURES
    - almalinux:8.8 set as default for the containers
-   - conda 25.3.1 set as default for the containers
+   - conda 23.5.1 set as default for the containers
    - micromamba is used to create conda envs and install conda packages
    - conda/multiconda profiles:
 	 * conda.enable has been added
    - Geniac CLI:
       *  Conda env with apptainer 1.2.2, nextflow 22.10.6, pip 23.2.1
 
 DOCUMENTATION
```

### Comparing `geniac-3.2.1/src/geniac.egg-info/SOURCES.txt` & `geniac-3.3.0/src/geniac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/tests/data/conf/geniac.config` & `geniac-3.3.0/tests/data/conf/geniac.config`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/tests/data/conf/multipath.config` & `geniac-3.3.0/tests/data/conf/multipath.config`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/tests/data/conf/path.config` & `geniac-3.3.0/tests/data/conf/path.config`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/tests/data/conf/process.config` & `geniac-3.3.0/tests/data/conf/process.config`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/tests/data/conf/singularity.config` & `geniac-3.3.0/tests/data/conf/singularity.config`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/tests/data/conf/test.config` & `geniac-3.3.0/tests/data/conf/test.config`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/tests/data/main.nf` & `geniac-3.3.0/tests/data/main.nf`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/tests/data/nextflow.config` & `geniac-3.3.0/tests/data/nextflow.config`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/tests/test_base.py` & `geniac-3.3.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/tests/test_commands_lint.py` & `geniac-3.3.0/tests/test_commands_lint.py`

 * *Files identical despite different names*

### Comparing `geniac-3.2.1/tox.ini` & `geniac-3.3.0/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -40,17 +40,15 @@
 description = invoke sphinx-build to build the docs/run doctests
 setenv =
     DOCSDIR = {toxinidir}/docs
     BUILDDIR = {toxinidir}/docs/_build
     docs: BUILD = html
     doctests: BUILD = doctest
 deps =
-    sphinx==4.4.0
-    sphinx-rtd-theme==1.0.0
-    # any docs/requirements.txt for/shared with Read The Docs?
+    -r{toxinidir}/docs/requirements.txt
 commands =
     sphinx-build -b {env:BUILD} -d "{env:BUILDDIR}/doctrees" "{env:DOCSDIR}" "{env:BUILDDIR}/{env:BUILD}" {posargs}
 
 
 [testenv:publish]
 description =
     Publish the package you have been developing to a package index server.
```

